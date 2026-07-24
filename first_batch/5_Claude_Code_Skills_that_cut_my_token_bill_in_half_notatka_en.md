---
id: "82856f66-75ee-4a7f-be84-c268482a7190"
---
# Optimizing Claude Token Consumption via Custom Skills

This content outlines a strategic shift in how to interact with Claude to drastically reduce token expenditure without sacrificing output quality. The author demonstrates a reduction in token usage from 47 million to 19 million tokens for the same project and workload by implementing five specific "skills" (custom instructions/markdown files). The central thesis is that token waste occurs primarily through redundant context loading and incorrect large-scale implementations, both of which can be mitigated by adding "friction" and structured checkpoints to the AI's workflow.

## Skill 1: Auto Compactor
This is identified as the most impactful skill, providing the highest cost savings by addressing the "context bloat" that occurs during long sessions where the same files are read repeatedly across multiple turns.

*   **The Problem:** In a standard session, Claude re-reads the same files (e.g., login, session, j.et) every time a follow-up prompt is sent, leading to exponential token growth.
*   **The Solution:** A markdown file in the skills folder that triggers based on specific conditions:
    *   The same file is read more than twice.
    *   The session exceeds 30 turns.
    *   The user explicitly states "you're slow."
*   **The Mechanism:** Upon triggering, Claude summarizes the previous 10 turns into five bullet points, executes a `/compact` command, and continues.
*   **Concrete Impact:** Reduced token usage for a specific task from 3.2 million tokens to 780,000 tokens (approximately 4x cheaper).

**Key Quotes**
* "Same file read more than twice, session over 30 turns, or you say you're slow."
* "Without the skill, Claude burned 3.2 million tokens, with it, 780,000."

## Skill 2: Review Before Run
This skill acts as a quality gate to prevent the AI from generating massive amounts of incorrect code that the user then has to pay to debug.

*   **The Problem:** Claude may perform an "opinion-heavy refactor" touching multiple files (e.g., seven files) that contains errors, forcing the user to pay for both the wrong code and the subsequent corrections.
*   **The Solution:** A mandatory gate before any multi-file edit. Claude must output three specific bullets:
    1. What will change?
    2. What could break?
    3. Roughly how many tokens will be used?
*   **The Math:** A wrong implementation can cost 8,000 output tokens, whereas a 50-word plan costs only 80 tokens.

**Key Quotes**
* "30 seconds of friction saves you thousands of wasted tokens."
* "A wrong implementation costs 8,000 output tokens. A 50-word plan costs 80."

## Skill 3: Spec First
This skill shifts the development order to ensure that the logic is validated before any code is written, avoiding the "rewrite loop."

*   **The Problem:** The "Classic Pass" involves writing code $\rightarrow$ writing tests that match the code $\rightarrow$ discovering an edge case $\rightarrow$ rewriting everything. This results in paying for two full passes.
*   **The Solution:** A mandatory five-line specification covering:
    *   Inputs
    *   Outputs
    *   Edge cases
    *   Failure modes
    *   Acceptance criteria
*   **The Workflow:** Spec $\rightarrow$ User Approval $\rightarrow$ Tests (based on spec) $\rightarrow$ Code (passes tests).
*   **Concrete Impact:** Reduced cost from 6,500 tokens across two rewrites to 3,300 tokens (2x cheaper).

**Key Quotes**
* "Claude writes code for sign up. Then tests that match the code. Then you find the edge case Claude skipped. Everything gets rewritten."
* "One pass tests you actually trust."

## Skill 4: Test Writer
This skill leverages the fact that the AI already has the relevant file in its immediate context to automate testing.

*   **The Problem:** Users often skip tests ("I'll add tests later") or prompt for tests after the context has been cleared, which is more expensive.
*   **The Solution:** A post-tool use hook. Every time Claude saves a source file, the skill automatically:
    *   Detects the framework (e.g., Jest vs. PyTest).
    *   Writes tests matching the existing style.
    *   Runs the tests and stops if they fail.
*   **Concrete Impact:** 3x cheaper than prompting for tests after the fact.

**Key Quotes**
* "Writing tests cold is boring. but Claude just had the file in context for the edit it wrote."
* "Three times cheaper than prompting, write me tests for X after the fact."

## Skill 5: Plan or Stop
This serves as a "circuit breaker" for high-risk, large-scale architectural changes.

*   **The Problem:** Broad prompts like "refactor the auth system" can lead to a "tangle" where half-implemented ideas ruin the repository, costing more to fix than to start over.
*   **The Solution:** The skill scans for "big task signals" (keywords: rewrite, migrate, refactor everything). If found, Claude must stop and provide a 4-item plan:
    1. Files involved
    2. Order of operations
    3. Rollback plan
    4. Estimated cost
*   **Concrete Impact:** Prevents "disasters" that can cost 30,000 tokens, replacing them with a 400-token plan.

**Key Quotes**
* "The circuit breaker for big tasks."
* "A bad big task execution easily costs 30,000 tokens. The plan costs 400."

## Key Takeaways, Insights & Context

**Core Thesis:** Token efficiency in LLM coding is not about prompting "better" in a single turn, but about implementing **structural constraints** and **validation gates** that prevent redundant processing and catastrophic errors.

**Ranked Impact of Skills:**
1.  **Auto Compactor:** Highest ROI; solves the systemic issue of context window bloat.
2.  **Review Before Run:** Prevents expensive, large-scale hallucinations/errors.
3.  **Spec First:** Halves the cost of non-trivial features by eliminating rewrite loops.
4.  **Test Writer:** Increases coverage and reduces cost by utilizing "hot" context.
5.  **Plan or Stop:** Risk mitigation for repository-wide changes.

**Actionable Guidance:**
*   Implement a `skills` folder in your repository containing markdown files that define these behaviors.
*   Introduce intentional "friction" (approval steps) to avoid the high cost of correcting large-scale AI mistakes.
*   Shift from a "Code $\rightarrow$ Test" workflow to a "Spec $\rightarrow$ Test $\rightarrow$ Code" workflow.
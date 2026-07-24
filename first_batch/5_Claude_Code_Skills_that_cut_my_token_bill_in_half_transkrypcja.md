---
id: "82856f66-75ee-4a7f-be84-c268482a7190"
video: "https://youtu.be/dHaGNQVVqro?si=CF7iJwzf_5G6nx4O"
name: "5 Claude Code Skills that cut my token bill in half"
created: "2026-01-01 14:31"
---
# 5 Claude Code Skills that cut my token bill in half

- **Model:** whisper
- **Plik:** 5_Claude_Code_Skills_that_cut_my_token_bill_in_half.mp4

---

[00:00:00 - 00:00:07] Last month, my clawed code 8 through 47 million tokens.
[00:00:07 - 00:00:10] This month 19, same project, same workload.
[00:00:10 - 00:00:14] I didn't downgrade, I didn't use it less, I just added 5 skills.
[00:00:14 - 00:00:16] Here's exactly what changed.
[00:00:16 - 00:00:19] 5 skills ranked by how much each saved me.
[00:00:19 - 00:00:22] Number 1 saved more than the other 4 combined.
[00:00:22 - 00:00:24] Stick around.
[00:00:24 - 00:00:26] Skill 1: Auto Compactor.
[00:00:26 - 00:00:28] This one saved me the most by a mile.
[00:00:28 - 00:00:29] Here's what's happening.
[00:00:30 - 00:00:59] You ask Claude to refactor your auth code. It reads login, session, j.et. You follow up, it reads them again, you follow up again, same files back into context every turn. That's where your token bill goes. The fix is a markdown file in your skills folder. The description tells Claude when to run it. Same file read more than twice, session over 30 turns, or you say you're slow. When it triggers, Claude summarizes the last 10 turns in five bullets, run slash compact,
[00:01:00 - 00:01:06] and keeps going. You don't even notice it happen. Same task, same prompts. Without the skill,
[00:01:06 - 00:01:13] Claude burned 3.2 million tokens, with it, 780,000. Four times cheaper for the same output.
[00:01:14 - 00:01:21] On a long session, this one skill pays for a month of pro. Skill 2, review before run. Skill 2,
[00:01:21 - 00:01:29] review before run, stops Claude from writing the wrong 400 lines. You type, clean up auth. Claude
[00:01:30 - 00:01:59] Nine minutes later you have an opinion-heavy refactor touching seven files. Some of it is wrong. Now you're debugging tokens you already paid for. The skill adds a gate. Before any multi-file edit, Claude outputs three bullets. What will change? What could break? Roughly how many tokens? You reply go or correct it in one line. 30 seconds of friction saves you thousands of wasted tokens. A wrong implementation costs 8,000 output tokens. A 50-word plan costs
[00:02:00 - 00:02:08] 80. Catches maybe one in four bad attempts. Math still works fast. Skill 3: Spec First. Skill 3: Spec
[00:02:08 - 00:02:14] First code or tests match the spec. Code matches the tests. Classic Pass: Claude writes code for
[00:02:14 - 00:02:20] sign up. Then tests that match the code. Then you find the edge case Claude skipped. Everything gets
[00:02:20 - 00:02:29] rewritten. Two full passes paid for both. The skill forces a five-line spec first. Inputs, outputs, edge cases, failure modes, accept
[00:02:30 - 00:02:35] You approve or fix it, then tests cover the spec, then code passes tests, one pass tests
[00:02:35 - 00:02:37] you actually trust.
[00:02:37 - 00:02:47] Without 6500 tokens across 2 rewrites, with 3300, 2 times cheaper on any non-trivial feature.
[00:02:47 - 00:02:49] Skill 4: Test Writer.
[00:02:49 - 00:02:53] Skill 4: Test Writer, tests for the file you just edited, automatic.
[00:02:53 - 00:02:55] We've all said I'll add tests later.
[00:02:55 - 00:02:57] Later rarely comes.
[00:02:57 - 00:02:59] Writing tests cold is boring.
[00:03:00 - 00:03:05] but Claude just had the file in context for the edit it wrote. The tests are basically free right there.
[00:03:06 - 00:03:12] Pair the skill with a post-tool use hook. Every time Claude saves a source file, the skill runs,
[00:03:12 - 00:03:18] detects your framework, Jest vs. PyTest, writes tests that match existing style, runs them, stops if they fail.
[00:03:19 - 00:03:23] Three times cheaper than prompting, write me tests for X after the fact,
[00:03:24 - 00:03:29] and you get coverage you'd otherwise skip. Skill 5: Plan or Stop.
[00:03:30 - 00:03:59] Skill 5: Plan or Stop, the circuit breaker for big tasks. You say refactor the auth system, Claude starts. 30 minutes later your repo is a tangle. Half an idea implemented five ways. Session budget gone. Fixing it costs more than starting over. The skill scans for big task signals, rewrite, migrate, refactor everything. If it finds them Claude stops, asks for a plan with four items, files, order, rollback, cost, you review then execute. Saves one disaster
[00:04:00 - 00:04:08] or a month, easy. A bad big task execution easily costs 30,000 tokens. The plan costs 400. You don't
[00:04:08 - 00:04:15] even need a high catch rate to win. All five ranked. 1. Auto Compactor. The big win. Four times
[00:04:15 - 00:04:22] cheaper on every long session. 2. Review before run. Kills the wrong 400 line refactor. 3. Spec first.
[00:04:22 - 00:04:29] Halves every non-trivial feature. 4. Test Writer. Three times cheaper than writing tests later. 5.
[00:04:30 - 00:04:35] Plan or Stop saves you from a repo disaster every few weeks. Full markdown files in the repo linked
[00:04:35 - 00:04:42] below. If this saved you tokens, next one is about MCP servers doing the same thing for your repo
[00:04:42 - 00:04:45] context. Subscribe so you don't miss it.

---

## Pełny tekst

 Last month, my clawed code 8 through 47 million tokens. This month 19, same project, same workload. I didn't downgrade, I didn't use it less, I just added 5 skills. Here's exactly what changed. 5 skills ranked by how much each saved me. Number 1 saved more than the other 4 combined. Stick around. Skill 1: Auto Compactor. This one saved me the most by a mile. Here's what's happening. You ask Claude to refactor your auth code. It reads login, session, j.et. You follow up, it reads them again, you follow up again, same files back into context every turn. That's where your token bill goes. The fix is a markdown file in your skills folder. The description tells Claude when to run it. Same file read more than twice, session over 30 turns, or you say you're slow. When it triggers, Claude summarizes the last 10 turns in five bullets, run slash compact, and keeps going. You don't even notice it happen. Same task, same prompts. Without the skill, Claude burned 3.2 million tokens, with it, 780,000. Four times cheaper for the same output. On a long session, this one skill pays for a month of pro. Skill 2, review before run. Skill 2, review before run, stops Claude from writing the wrong 400 lines. You type, clean up auth. Claude Nine minutes later you have an opinion-heavy refactor touching seven files. Some of it is wrong. Now you're debugging tokens you already paid for. The skill adds a gate. Before any multi-file edit, Claude outputs three bullets. What will change? What could break? Roughly how many tokens? You reply go or correct it in one line. 30 seconds of friction saves you thousands of wasted tokens. A wrong implementation costs 8,000 output tokens. A 50-word plan costs 80. Catches maybe one in four bad attempts. Math still works fast. Skill 3: Spec First. Skill 3: Spec First code or tests match the spec. Code matches the tests. Classic Pass: Claude writes code for sign up. Then tests that match the code. Then you find the edge case Claude skipped. Everything gets rewritten. Two full passes paid for both. The skill forces a five-line spec first. Inputs, outputs, edge cases, failure modes, accept You approve or fix it, then tests cover the spec, then code passes tests, one pass tests you actually trust. Without 6500 tokens across 2 rewrites, with 3300, 2 times cheaper on any non-trivial feature. Skill 4: Test Writer. Skill 4: Test Writer, tests for the file you just edited, automatic. We've all said I'll add tests later. Later rarely comes. Writing tests cold is boring. but Claude just had the file in context for the edit it wrote. The tests are basically free right there. Pair the skill with a post-tool use hook. Every time Claude saves a source file, the skill runs, detects your framework, Jest vs. PyTest, writes tests that match existing style, runs them, stops if they fail. Three times cheaper than prompting, write me tests for X after the fact, and you get coverage you'd otherwise skip. Skill 5: Plan or Stop. Skill 5: Plan or Stop, the circuit breaker for big tasks. You say refactor the auth system, Claude starts. 30 minutes later your repo is a tangle. Half an idea implemented five ways. Session budget gone. Fixing it costs more than starting over. The skill scans for big task signals, rewrite, migrate, refactor everything. If it finds them Claude stops, asks for a plan with four items, files, order, rollback, cost, you review then execute. Saves one disaster or a month, easy. A bad big task execution easily costs 30,000 tokens. The plan costs 400. You don't even need a high catch rate to win. All five ranked. 1. Auto Compactor. The big win. Four times cheaper on every long session. 2. Review before run. Kills the wrong 400 line refactor. 3. Spec first. Halves every non-trivial feature. 4. Test Writer. Three times cheaper than writing tests later. 5. Plan or Stop saves you from a repo disaster every few weeks. Full markdown files in the repo linked below. If this saved you tokens, next one is about MCP servers doing the same thing for your repo context. Subscribe so you don't miss it.
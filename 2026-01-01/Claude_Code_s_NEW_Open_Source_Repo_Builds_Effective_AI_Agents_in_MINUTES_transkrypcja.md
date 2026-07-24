---
id: "ea182c2e-5237-4e5a-bb7d-8582340b4b3f"
video: "https://www.youtube.com/watch?v=D6Cfjy83MQA"
name: "Claude Code s NEW Open Source Repo Builds Effective AI Agents in MINUTES"
created: "2026-06-22 16:36"
---

# Claude Code s NEW Open Source Repo Builds Effective AI Agents in MINUTES

- **Model:** whisper
- **Plik:** Claude_Code_s_NEW_Open_Source_Repo_Builds_Effective_AI_Agents_in_MINUTES.mp4

---

[00:00:00 - 00:00:06] Anthropic just released a free open source skill for Cloud Code that will completely change the
[00:00:06 - 00:00:11] way you automate your work and build AI agents. This is the Launch Your Agent skill and it is
[00:00:11 - 00:00:17] designed to take you from idea to a live managed agent in just a couple of minutes. In this video,
[00:00:17 - 00:00:23] we'll talk about what the skill does, how it represents the new way of writing code with AI,
[00:00:23 - 00:00:29] and how to install it. And at the end, we'll even demo it live on a real use case. There's even one core feature of
[00:00:30 - 00:00:36] this skill that makes creating AI agents incredibly simple, even for beginners. So to be able to use
[00:00:36 - 00:00:39] the launch your agent skill, there are really three basic things that you need to understand.
[00:00:40 - 00:00:45] First is really like, what is an AI agent? And basically you can just think of an AI agent as an
[00:00:45 - 00:00:50] employee. You give it a task or something to do, it goes ahead, it performs that task, and it comes
[00:00:50 - 00:00:55] back with a response. There is a fundamental difference between agents and just like simple
[00:00:55 - 00:00:59] clawed chat. Basically agents have tools, a chat is just one.
[00:01:00 - 00:01:05] words. So an agent can search the web, it can write files, it can run code, it can call APIs,
[00:01:05 - 00:01:11] it chooses itself which tools to use at each step, and it just handles everything on its own.
[00:01:11 - 00:01:16] This is essentially how real automation works. If you want AI to do recurring work for you without
[00:01:16 - 00:01:20] you touching it, you need an agent, not just a better prompt. So that's the first thing.
[00:01:21 - 00:01:29] The second thing is you need to understand what a loop is. A loop is the new way to write code with AI, but don't take it from me, this is
[00:01:30 - 00:01:34] Boris Cherny. He is the creator of quad code. And this is how he says he writes code now.
[00:01:34 - 00:01:41] And so for me, the way that I coded a year ago was I wrote code with some autocomplete in IDE.
[00:01:41 - 00:01:45] At that point, I was running maybe five, 10 quads in parallel. And my coding was prompting
[00:01:45 - 00:01:50] quad to write code. Now it's actually leveled up, I think, again, to the next way of abstraction,
[00:01:50 - 00:01:55] where I don't prompt quad anymore. I have loops that are running. They're the ones that are
[00:01:55 - 00:01:59] prompting quad and figuring out what to do. My job is to write loops. He literally says I don't
[00:02:00 - 00:02:05] prompt Claude anymore. My job is to write loops and basically Claude then just prompts itself.
[00:02:05 - 00:02:11] So this is at the core of the launch your agent skill. You can think of a loop as giving Claude
[00:02:11 - 00:02:17] a goal and not a task. And this is why it gets so much more powerful because Claude often knows a
[00:02:17 - 00:02:22] better way to accomplish your goal than if you were to give it some sort of like explicit set
[00:02:22 - 00:02:29] of instructions. So the loop is what makes an agent different from a chat. It's going to run the same cycle over and over again until the
[00:02:30 - 00:02:31] task is done.
[00:02:31 - 00:02:33] So you're going to give quad a goal.
[00:02:33 - 00:02:35] Quad will think about what to do next.
[00:02:35 - 00:02:39] It will decide which tools it needs to actually accomplish that goal.
[00:02:40 - 00:02:42] It's going to try its best to do it on the first try.
[00:02:43 - 00:02:44] It's going to check itself.
[00:02:44 - 00:02:46] So it's going to read its own results.
[00:02:46 - 00:02:48] And then from there, decide what to do next.
[00:02:48 - 00:02:50] Like, are the results good enough?
[00:02:50 - 00:02:53] If they're not, go back to step two, think about how they could be better.
[00:02:53 - 00:02:54] Repeat this process.
[00:02:54 - 00:02:58] And then only if the results are actually good enough and pass the test, then it's going
[00:02:58 - 00:02:59] to present.
[00:03:00 - 00:03:05] the response back to the user. So you can think of it as this self improving feedback loop that you
[00:03:05 - 00:03:10] as the human are no longer responsible for the results of Claude, like it's responsible for its
[00:03:10 - 00:03:15] own results. And so basically, the launcher agent skill is designed to help you as the human write
[00:03:15 - 00:03:20] good quality loops. And so really, there are only three things you need to give the loop for it to
[00:03:20 - 00:03:24] understand. So one is context. Is there anything you already know that might be helpful for the
[00:03:24 - 00:03:29] agent to know going into this? Like, is there any information about your personal preferences or a
[00:03:30 - 00:03:34] database of information that exists. The second thing is a goal. Like what is it that you are
[00:03:34 - 00:03:39] actually trying to achieve? And then three success, like what does success look like? What is your
[00:03:39 - 00:03:45] ideal outcome from all of this? But it gets even better because there is a fundamental problem with
[00:03:45 - 00:03:49] loops in general is that you sort of have to like type in slash loop into quad and then you have to
[00:03:49 - 00:03:54] sit there and wait for it to run. But the launcher agent skill will actually build what's known as a
[00:03:54 - 00:03:59] CMA or a quad managed agent. And so it basically just means that Anthropic is going to run the loop
[00:04:00 - 00:04:05] for you, it's going to host it in the cloud on their servers. So it's always on so you can schedule
[00:04:05 - 00:04:09] it like as a task to run whenever you want. And it doesn't matter if you're at your computer,
[00:04:09 - 00:04:14] if your computer's on wherever you are, it is always on in the cloud in Anthropix servers.
[00:04:15 - 00:04:19] What's also cool about this is that there are no additional platform fees, you just pay the API
[00:04:19 - 00:04:23] cost to use the thing. And so the old way you would do it is you would have to build this loop
[00:04:23 - 00:04:27] yourself, you'd have to like fire up your own server, you'd have to troubleshoot your own errors,
[00:04:27 - 00:04:29] wire in all the tools and all of that.
[00:04:30 - 00:04:35] But basically this skill is going to allow you to create these quad managed agents really effortlessly
[00:04:35 - 00:04:40] and let quad and anthropic handle the workload. The other benefit is you can attach this thing
[00:04:40 - 00:04:44] called a memory store. And so your agents will actually remember things across the different
[00:04:44 - 00:04:49] sessions or across the different runs. So your agent is going to read what it learned last time.
[00:04:49 - 00:04:54] And so it's actually going to get better every single time the loop runs. And so this is how
[00:04:54 - 00:04:59] the launcher agent skill works. And the thing highlighted in red is the biggest unlock and what
[00:05:00 - 00:05:02] makes it super powerful, even for beginner users
[00:05:02 - 00:05:04] who have never built agents before.
[00:05:04 - 00:05:06] So all you have to do is run and launch your agent
[00:05:06 - 00:05:07] inside of cloud code.
[00:05:07 - 00:05:10] We're gonna set this up in a second, but then this part,
[00:05:10 - 00:05:12] the skill is going to interview you.
[00:05:12 - 00:05:13] It's gonna ask you what it should do
[00:05:13 - 00:05:15] and what success looks like,
[00:05:15 - 00:05:17] because the agent won't know if it's done,
[00:05:17 - 00:05:20] if it doesn't understand what it means to be successful.
[00:05:20 - 00:05:22] Next, it's going to make all the API calls.
[00:05:22 - 00:05:24] It's going to create your agent.
[00:05:24 - 00:05:25] It's gonna spin up the cloud environment.
[00:05:25 - 00:05:27] It's gonna set the schedule that you want.
[00:05:27 - 00:05:29] You're literally not gonna have to do any of this.
[00:05:30 - 00:05:34] So from that point on, basically like you no longer have to be inside of cloud code.
[00:05:34 - 00:05:35] The managed agent takes over.
[00:05:35 - 00:05:37] It's going to run the loop.
[00:05:37 - 00:05:40] It's going to grade the output against your success criteria.
[00:05:40 - 00:05:43] And it's literally just going to repeat until it passes.
[00:05:43 - 00:05:47] And so you get the result of this without having to write a single line of code yourself.
[00:05:47 - 00:05:51] So now that you understand how awesome this skill is, let me show you how to install it.
[00:05:51 - 00:05:52] And let's run a basic demo.
[00:05:52 - 00:05:56] What I love about cloud code is everything is just obscenely easy at this point.
[00:05:56 - 00:05:59] Like literally, I'm just going to copy this link to the GitHub
[00:06:00 - 00:06:03] repo. I'll leave a link in the description where you can access this. It's open source. It's totally
[00:06:03 - 00:06:07] free. I'm sure they're going to be improving this over time. Come back into Claude and I'm just
[00:06:07 - 00:06:13] going to say install this skill globally. Just going to paste in the link to the GitHub repo.
[00:06:13 - 00:06:17] Claude says I'll look at that repo to figure out how it's meant to be installed, then install it
[00:06:17 - 00:06:22] globally. So this just took a couple of seconds and it installed the launch your agent skill and
[00:06:22 - 00:06:25] a surprise bonus skill, which is the wrap up skill.
[00:06:25 - 00:06:29] So we can open this up inside of GitHub and come into wrap up to understand what
[00:06:30 - 00:06:34] this skill actually does. It basically just closes out the project and it's kind of just a nice way
[00:06:34 - 00:06:38] for you to wrap things up. Okay. One is going to congratulate the user, which I think is funny too.
[00:06:38 - 00:06:43] It's actually going to create an overview page of everything that you built. And then actually the
[00:06:43 - 00:06:47] thing that I think is the most impactful is this, here's what's next piece. So it's actually going
[00:06:47 - 00:06:51] to pick one to two upgrades that you could make to upgrade your agent. And it's going to tell you
[00:06:51 - 00:06:55] about them. So everything is now registered and ready to go. There is just one thing to note that
[00:06:55 - 00:06:59] you're going to need an Anthropic API key from your own account. So in order to get access,
[00:07:00 - 00:07:02] to the new skill inside of the desktop app,
[00:07:02 - 00:07:03] you need to restart it.
[00:07:03 - 00:07:05] So I'm just gonna quit and open this back up.
[00:07:05 - 00:07:06] Okay, so I'm back.
[00:07:06 - 00:07:08] If I type in slash and then type in launch,
[00:07:08 - 00:07:11] you can see now we have the launch your agent skill
[00:07:11 - 00:07:12] all ready to go.
[00:07:13 - 00:07:15] So let's test it out and see how awesome it is.
[00:07:15 - 00:07:16] I'm not gonna give it anything else.
[00:07:16 - 00:07:17] I'm just gonna run the skill
[00:07:17 - 00:07:19] because the skill is supposed to interview me
[00:07:19 - 00:07:22] to figure out what type of agent I wanna build today.
[00:07:22 - 00:07:24] So I thought it'd be fun just to try this
[00:07:24 - 00:07:25] on a simple use case.
[00:07:25 - 00:07:26] So this is pretty cool.
[00:07:26 - 00:07:27] It says, welcome.
[00:07:27 - 00:07:28] Here's what we're gonna do together.
[00:07:28 - 00:07:29] Figure out what you want an agent
[00:07:30 - 00:07:34] to do, get a first version live on your own Anthropic account today, and then grade it
[00:07:34 - 00:07:39] against your own definition of good and improve it from there. And if it's the kind of thing that
[00:07:39 - 00:07:44] should run on a clock, we'll put it on a schedule. So it works without you pretty cool. So here are
[00:07:44 - 00:07:48] a few examples of what a managed agent can be just to set the range. I really like this because this
[00:07:48 - 00:07:54] actually personalized these for me based off of past conversations I've had with Claude. So one is
[00:07:54 - 00:07:59] like a recurring digest or scan. This could run every morning sweeps your sources, file some sort of report.
[00:08:00 - 00:08:02] I definitely already do a lot of AI news
[00:08:02 - 00:08:02] and competitor work,
[00:08:02 - 00:08:04] and it says this shape fits you well.
[00:08:04 - 00:08:06] Or I could set this up to be a data analyst,
[00:08:06 - 00:08:08] like hand it a CSV or an export
[00:08:08 - 00:08:11] and get back a narrative report with charts
[00:08:11 - 00:08:11] or what's changed
[00:08:11 - 00:08:13] or anything interesting that stands out.
[00:08:13 - 00:08:15] So for someone like me who creates content,
[00:08:15 - 00:08:17] maybe having a look at my YouTube analytics
[00:08:17 - 00:08:18] and make new suggestions.
[00:08:18 - 00:08:20] I wanted to try to keep this simple today,
[00:08:20 - 00:08:22] maybe not using a whole bunch of other API keys.
[00:08:22 - 00:08:23] I think option number one,
[00:08:23 - 00:08:25] the daily news digest is helpful,
[00:08:25 - 00:08:27] maybe looking at Reddit or the news
[00:08:27 - 00:08:29] for interesting topics or trending news
[00:08:30 - 00:08:34] in my niche coming up with some sort of LinkedIn post or a hook angle or something that might
[00:08:34 - 00:08:35] be relevant to my audience.
[00:08:35 - 00:08:36] Does this make sense?
[00:08:37 - 00:08:42] So one thing I like to do sometimes is I will ask Claude if this makes sense, or I will
[00:08:42 - 00:08:45] tell it to ask me any other questions it might have, because maybe I have some blind spots
[00:08:45 - 00:08:50] and I'm not able to articulate my idea very well, but Claude can actually help me figure
[00:08:50 - 00:08:50] things out.
[00:08:50 - 00:08:51] So cool.
[00:08:51 - 00:08:55] This is asking me to give it more information like it is interviewing me so we can create
[00:08:55 - 00:08:56] the best possible agent.
[00:08:56 - 00:08:59] So a scheduled sweep that reads your sources and hands you something you can actually
[00:09:00 - 00:09:05] post, which is great. Tell me more in your own words, what would a great first version actually
[00:09:05 - 00:09:09] hand you each morning? But it didn't just leave this question like vague and open ended, it got
[00:09:09 - 00:09:14] way more specific. So like, what's the deliverable? Like when I open it, what do I want to see? Do I
[00:09:14 - 00:09:18] want to see a few raw trending stories with the link? Do I want to see fully drafted LinkedIn
[00:09:18 - 00:09:22] posts ready to paste or somewhere in between? Then it asked me about my niche or audience.
[00:09:22 - 00:09:27] It knows I'm into AI knows I like building with Claude. Is that the lens that I want to focus it
[00:09:27 - 00:09:29] through? Or should it be something else? And then what source does
[00:09:30 - 00:09:34] to use like Reddit? Are there any particular subreddits I should use? X, competitive YouTube,
[00:09:34 - 00:09:38] what do you actually check each morning that this should replay? So is there anything in your life
[00:09:38 - 00:09:43] that you are doing manually every single day or once a week that Claude could take off your plate?
[00:09:43 - 00:09:47] For the deliverable, I think I'd like to see a combination, a story with a link, a hook angle,
[00:09:48 - 00:09:51] and then yeah, why it matters to my audience, I think is really impactful and basically what they
[00:09:51 - 00:09:55] might get out of consuming that content. For my niche or audience, you understand this niche
[00:09:55 - 00:09:59] pretty well. Sources, let's start just with the Claude or
[00:10:00 - 00:10:00] quad code or
[00:10:00 - 00:10:01] anthropic subreddits
[00:10:01 - 00:10:02] cool so here's what
[00:10:02 - 00:10:03] it has for me so
[00:10:03 - 00:10:04] far and then it
[00:10:04 - 00:10:05] says it has three
[00:10:05 - 00:10:05] more quick questions
[00:10:05 - 00:10:06] for me to answer
[00:10:06 - 00:10:07] before it builds
[00:10:07 - 00:10:07] this out and so
[00:10:07 - 00:10:08] why I love this
[00:10:08 - 00:10:09] interview process is
[00:10:09 - 00:10:10] because it's
[00:10:00 - 00:10:04] you can spend 10 minutes of time now to get this part right. And it's going to save you hours of
[00:10:04 - 00:10:09] work later. So this lets me know that it basically understands the goal, but now it's asking me to
[00:10:09 - 00:10:14] more clearly define the outcome. So what does success look like? So it actually drafted this
[00:10:14 - 00:10:19] outcome rubric for me. So does the digest pass the test? If exactly five items, each with a real
[00:10:19 - 00:10:23] Reddit post and working link, each item has a distinct hook angle in your voice. Each item has
[00:10:23 - 00:10:29] a why it matters to your audience part built in items are genuinely recent and trending. This is super
[00:10:30 - 00:10:34] important. You don't want to be old news. There are no duplicate stories and the output is a clean
[00:10:34 - 00:10:39] scannable markdown file. This is awesome. So it asked me, does this look right? Do I want to
[00:10:39 - 00:10:42] tighten anything about the voice or do I want to drop the trending check? But no, this looks right
[00:10:42 - 00:10:46] to me. Do you have a past example of a digest you'd call great? I'm going to say no. Use today's
[00:10:46 - 00:10:51] first run as a baseline because again, the whole idea is that this just improves over time the more
[00:10:51 - 00:10:56] it runs. And basically what time zone am I in? I'm on the West Coast in California. So right now,
[00:10:56 - 00:10:59] it's just checking to see if I have an Anthropic API key.
[00:11:00 - 00:11:04] already set up. I know I do. So it's going to find it. But if you don't have that set up, it's super
[00:11:04 - 00:11:09] easy. Just come over to platform.claw.com and sign in with your account. From there, you can just
[00:11:09 - 00:11:14] click on the left into API keys, click create a key. And you could just name this, you know, like
[00:11:14 - 00:11:18] my agent or whatever, click add, it's going to come up with an API key, I'm going to delete this. So
[00:11:18 - 00:11:22] don't worry about it. And then all you have to do is copy this, go back into cloud code and say,
[00:11:22 - 00:11:26] hey, here's my API key. Claude just came back said everything I need is in hand. Here's the
[00:11:26 - 00:11:29] whole thing as a plan, which is pretty cool. It gives me the agent,
[00:11:30 - 00:11:31] in the CMA shape.
[00:11:31 - 00:11:34] We are setting up a daily AI digest using Opus 4.8.
[00:11:34 - 00:11:35] If you want to change the model,
[00:11:35 - 00:11:36] you can tell it to do so.
[00:11:37 - 00:11:38] This is the environment it's in,
[00:11:38 - 00:11:39] any tools that it needs,
[00:11:39 - 00:11:40] like the desired outcome,
[00:11:40 - 00:11:41] the final deliverable,
[00:11:41 - 00:11:43] the schedule that it should run on,
[00:11:43 - 00:11:45] and basically anything we need to evaluate this.
[00:11:45 - 00:11:47] But we haven't done this yet because it hasn't run.
[00:11:47 - 00:11:49] This is what's not included in version zero,
[00:11:49 - 00:11:50] which we're setting up right now.
[00:11:50 - 00:11:52] But you can see it's already making a game plan
[00:11:52 - 00:11:54] for how to improve this in the future.
[00:11:54 - 00:11:55] So does this plan look right?
[00:11:55 - 00:11:57] I'm actually going to say swap this to Sonnet
[00:11:57 - 00:11:58] because I don't think we need Opus for this.
[00:11:58 - 00:11:59] But otherwise,
[00:12:00 - 00:12:04] we are good to go. So this is awesome. Claude just went ahead and built everything for me. You can
[00:12:04 - 00:12:09] actually watch this live as it fires for the first time. You can see it actually built this managed
[00:12:09 - 00:12:15] agent for me inside of that same site, platform.claw.com. This is the system prompt that it
[00:12:15 - 00:12:19] built. If you go into sessions, these are the sessions you can check as it goes on. This is the
[00:12:19 - 00:12:24] first session right now. These are all the calls that it's making. It's going to fix itself. You can
[00:12:24 - 00:12:28] see we encounter some errors, but we know Claude's going to fix it. The other thing it did is it built
[00:12:30 - 00:12:35] overview dashboard. So if you've been building like AIOS or agentic operating systems or whatever,
[00:12:35 - 00:12:40] this is a nice way to just check in on your agent. So you can see this agent is launched and deployed.
[00:12:40 - 00:12:45] It's fully running. This is an HTML file that lives on your machine. So you can also just open this up
[00:12:45 - 00:12:49] in your browser. You could check on the outcomes or any of the next directions. And what's cool is
[00:12:49 - 00:12:53] that this will update over time as you make improvements. You can also see that we still
[00:12:53 - 00:12:59] have one running task, and this is basically just watching the loop and waiting for it to finish. And
[00:13:00 - 00:13:01] if you want to learn Claude code,
[00:13:01 - 00:13:02] like come into these things
[00:13:02 - 00:13:04] that might seem confusing at first
[00:13:04 - 00:13:05] and just read what it's saying
[00:13:05 - 00:13:07] and you can get a good understanding
[00:13:07 - 00:13:08] of what it's doing.
[00:13:08 - 00:13:10] We can see like I found two Reddit posts.
[00:13:10 - 00:13:12] I now have enough information to write the digest.
[00:13:12 - 00:13:15] Okay, the digest is written and it's saved here, right?
[00:13:15 - 00:13:16] Now we can see that all it's doing
[00:13:16 - 00:13:19] is it's actually just grading its own work.
[00:13:19 - 00:13:21] And so just by reading the response from Claude,
[00:13:21 - 00:13:23] you can actually learn a lot about how these systems work.
[00:13:23 - 00:13:24] So this is the moment of truth
[00:13:24 - 00:13:27] where we talk about the good, the bad and the ugly.
[00:13:27 - 00:13:29] So this is the digest that the system
[00:13:30 - 00:13:32] and produced, we can see it has five different articles,
[00:13:32 - 00:13:34] the story, a link, the hook angle,
[00:13:34 - 00:13:37] why this matters to my audience, et cetera, et cetera.
[00:13:37 - 00:13:38] That being said, transparently,
[00:13:38 - 00:13:40] we hit a couple of issues that honestly probably had to do
[00:13:40 - 00:13:43] a little bit with user error and a little bit with Claude,
[00:13:43 - 00:13:45] not digging deeper before building.
[00:13:45 - 00:13:47] The main issue that we hit was in this Claude managed
[00:13:47 - 00:13:50] environment, it wasn't able to actually access Reddit
[00:13:50 - 00:13:54] directly, and so this thing took 28 minutes to run,
[00:13:54 - 00:13:56] mostly because it kept getting errors
[00:13:56 - 00:13:57] when trying to access Reddit.
[00:13:57 - 00:13:59] So it actually was able to search the web
[00:14:00 - 00:14:02] and find a lot of really great relevant articles,
[00:14:02 - 00:14:04] but because it wasn't able to pull in the Reddit link
[00:14:04 - 00:14:06] directly, the system failed.
[00:14:06 - 00:14:07] Because if we come down here,
[00:14:07 - 00:14:10] we can see that one of the requirements was that each post
[00:14:10 - 00:14:12] linked to a real Reddit post.
[00:14:12 - 00:14:14] And so because we weren't able to pull those in,
[00:14:14 - 00:14:15] the system failed.
[00:14:15 - 00:14:17] And so I did spend a lot of tokens on this.
[00:14:17 - 00:14:20] You can see I spent like 27 million tokens.
[00:14:20 - 00:14:22] It was like $12 just to run this.
[00:14:22 - 00:14:24] And again, like this actually really could have been avoided.
[00:14:24 - 00:14:26] How do we know I'm going into it that we would have run
[00:14:26 - 00:14:27] into these issues with Reddit.
[00:14:27 - 00:14:29] So maybe before creating the managed agent,
[00:14:30 - 00:14:32] having the system actually check the individual pieces
[00:14:32 - 00:14:34] just to make sure that the theories are good
[00:14:34 - 00:14:38] behind the build before actually setting it up on the cloud.
[00:14:38 - 00:14:39] What's good about the system
[00:14:39 - 00:14:41] is that we have the core foundation in place.
[00:14:41 - 00:14:42] And this was sort of the whole point
[00:14:42 - 00:14:44] of running these managed agents in loop mode
[00:14:44 - 00:14:47] is that they are self-improving with every run.
[00:14:47 - 00:14:49] With each run, we learn something new
[00:14:49 - 00:14:50] about how we can make an upgrade.
[00:14:50 - 00:14:52] And so now it's just asking me,
[00:14:52 - 00:14:54] like, how do I want to fix the Reddit sourcing issue?
[00:14:55 - 00:14:56] Can I just use web search only?
[00:14:56 - 00:14:58] And this will run in like two or three minutes
[00:14:58 - 00:14:59] as opposed to 30 minutes
[00:15:00 - 00:15:01] with a bad response.
[00:15:01 - 00:15:03] And so just in setting this up for the first time today,
[00:15:03 - 00:15:04] I personally learned a lot of good lessons.
[00:15:05 - 00:15:06] If you want to continue learning Cloud Code,
[00:15:07 - 00:15:08] just check the link in the description.
[00:15:08 - 00:15:10] If you want to see how I built my own agentic OS,
[00:15:10 - 00:15:12] check out this video right here.
[00:15:12 - 00:15:13] I'll see you over there.

---

## Pełny tekst

 Anthropic just released a free open source skill for Cloud Code that will completely change the way you automate your work and build AI agents. This is the Launch Your Agent skill and it is designed to take you from idea to a live managed agent in just a couple of minutes. In this video, we'll talk about what the skill does, how it represents the new way of writing code with AI, and how to install it. And at the end, we'll even demo it live on a real use case. There's even one core feature of this skill that makes creating AI agents incredibly simple, even for beginners. So to be able to use the launch your agent skill, there are really three basic things that you need to understand. First is really like, what is an AI agent? And basically you can just think of an AI agent as an employee. You give it a task or something to do, it goes ahead, it performs that task, and it comes back with a response. There is a fundamental difference between agents and just like simple clawed chat. Basically agents have tools, a chat is just one. words. So an agent can search the web, it can write files, it can run code, it can call APIs, it chooses itself which tools to use at each step, and it just handles everything on its own. This is essentially how real automation works. If you want AI to do recurring work for you without you touching it, you need an agent, not just a better prompt. So that's the first thing. The second thing is you need to understand what a loop is. A loop is the new way to write code with AI, but don't take it from me, this is Boris Cherny. He is the creator of quad code. And this is how he says he writes code now. And so for me, the way that I coded a year ago was I wrote code with some autocomplete in IDE. At that point, I was running maybe five, 10 quads in parallel. And my coding was prompting quad to write code. Now it's actually leveled up, I think, again, to the next way of abstraction, where I don't prompt quad anymore. I have loops that are running. They're the ones that are prompting quad and figuring out what to do. My job is to write loops. He literally says I don't prompt Claude anymore. My job is to write loops and basically Claude then just prompts itself. So this is at the core of the launch your agent skill. You can think of a loop as giving Claude a goal and not a task. And this is why it gets so much more powerful because Claude often knows a better way to accomplish your goal than if you were to give it some sort of like explicit set of instructions. So the loop is what makes an agent different from a chat. It's going to run the same cycle over and over again until the task is done. So you're going to give quad a goal. Quad will think about what to do next. It will decide which tools it needs to actually accomplish that goal. It's going to try its best to do it on the first try. It's going to check itself. So it's going to read its own results. And then from there, decide what to do next. Like, are the results good enough? If they're not, go back to step two, think about how they could be better. Repeat this process. And then only if the results are actually good enough and pass the test, then it's going to present. the response back to the user. So you can think of it as this self improving feedback loop that you as the human are no longer responsible for the results of Claude, like it's responsible for its own results. And so basically, the launcher agent skill is designed to help you as the human write good quality loops. And so really, there are only three things you need to give the loop for it to understand. So one is context. Is there anything you already know that might be helpful for the agent to know going into this? Like, is there any information about your personal preferences or a database of information that exists. The second thing is a goal. Like what is it that you are actually trying to achieve? And then three success, like what does success look like? What is your ideal outcome from all of this? But it gets even better because there is a fundamental problem with loops in general is that you sort of have to like type in slash loop into quad and then you have to sit there and wait for it to run. But the launcher agent skill will actually build what's known as a CMA or a quad managed agent. And so it basically just means that Anthropic is going to run the loop for you, it's going to host it in the cloud on their servers. So it's always on so you can schedule it like as a task to run whenever you want. And it doesn't matter if you're at your computer, if your computer's on wherever you are, it is always on in the cloud in Anthropix servers. What's also cool about this is that there are no additional platform fees, you just pay the API cost to use the thing. And so the old way you would do it is you would have to build this loop yourself, you'd have to like fire up your own server, you'd have to troubleshoot your own errors, wire in all the tools and all of that. But basically this skill is going to allow you to create these quad managed agents really effortlessly and let quad and anthropic handle the workload. The other benefit is you can attach this thing called a memory store. And so your agents will actually remember things across the different sessions or across the different runs. So your agent is going to read what it learned last time. And so it's actually going to get better every single time the loop runs. And so this is how the launcher agent skill works. And the thing highlighted in red is the biggest unlock and what makes it super powerful, even for beginner users who have never built agents before. So all you have to do is run and launch your agent inside of cloud code. We're gonna set this up in a second, but then this part, the skill is going to interview you. It's gonna ask you what it should do and what success looks like, because the agent won't know if it's done, if it doesn't understand what it means to be successful. Next, it's going to make all the API calls. It's going to create your agent. It's gonna spin up the cloud environment. It's gonna set the schedule that you want. You're literally not gonna have to do any of this. So from that point on, basically like you no longer have to be inside of cloud code. The managed agent takes over. It's going to run the loop. It's going to grade the output against your success criteria. And it's literally just going to repeat until it passes. And so you get the result of this without having to write a single line of code yourself. So now that you understand how awesome this skill is, let me show you how to install it. And let's run a basic demo. What I love about cloud code is everything is just obscenely easy at this point. Like literally, I'm just going to copy this link to the GitHub repo. I'll leave a link in the description where you can access this. It's open source. It's totally free. I'm sure they're going to be improving this over time. Come back into Claude and I'm just going to say install this skill globally. Just going to paste in the link to the GitHub repo. Claude says I'll look at that repo to figure out how it's meant to be installed, then install it globally. So this just took a couple of seconds and it installed the launch your agent skill and a surprise bonus skill, which is the wrap up skill. So we can open this up inside of GitHub and come into wrap up to understand what this skill actually does. It basically just closes out the project and it's kind of just a nice way for you to wrap things up. Okay. One is going to congratulate the user, which I think is funny too. It's actually going to create an overview page of everything that you built. And then actually the thing that I think is the most impactful is this, here's what's next piece. So it's actually going to pick one to two upgrades that you could make to upgrade your agent. And it's going to tell you about them. So everything is now registered and ready to go. There is just one thing to note that you're going to need an Anthropic API key from your own account. So in order to get access, to the new skill inside of the desktop app, you need to restart it. So I'm just gonna quit and open this back up. Okay, so I'm back. If I type in slash and then type in launch, you can see now we have the launch your agent skill all ready to go. So let's test it out and see how awesome it is. I'm not gonna give it anything else. I'm just gonna run the skill because the skill is supposed to interview me to figure out what type of agent I wanna build today. So I thought it'd be fun just to try this on a simple use case. So this is pretty cool. It says, welcome. Here's what we're gonna do together. Figure out what you want an agent to do, get a first version live on your own Anthropic account today, and then grade it against your own definition of good and improve it from there. And if it's the kind of thing that should run on a clock, we'll put it on a schedule. So it works without you pretty cool. So here are a few examples of what a managed agent can be just to set the range. I really like this because this actually personalized these for me based off of past conversations I've had with Claude. So one is like a recurring digest or scan. This could run every morning sweeps your sources, file some sort of report. I definitely already do a lot of AI news and competitor work, and it says this shape fits you well. Or I could set this up to be a data analyst, like hand it a CSV or an export and get back a narrative report with charts or what's changed or anything interesting that stands out. So for someone like me who creates content, maybe having a look at my YouTube analytics and make new suggestions. I wanted to try to keep this simple today, maybe not using a whole bunch of other API keys. I think option number one, the daily news digest is helpful, maybe looking at Reddit or the news for interesting topics or trending news in my niche coming up with some sort of LinkedIn post or a hook angle or something that might be relevant to my audience. Does this make sense? So one thing I like to do sometimes is I will ask Claude if this makes sense, or I will tell it to ask me any other questions it might have, because maybe I have some blind spots and I'm not able to articulate my idea very well, but Claude can actually help me figure things out. So cool. This is asking me to give it more information like it is interviewing me so we can create the best possible agent. So a scheduled sweep that reads your sources and hands you something you can actually post, which is great. Tell me more in your own words, what would a great first version actually hand you each morning? But it didn't just leave this question like vague and open ended, it got way more specific. So like, what's the deliverable? Like when I open it, what do I want to see? Do I want to see a few raw trending stories with the link? Do I want to see fully drafted LinkedIn posts ready to paste or somewhere in between? Then it asked me about my niche or audience. It knows I'm into AI knows I like building with Claude. Is that the lens that I want to focus it through? Or should it be something else? And then what source does to use like Reddit? Are there any particular subreddits I should use? X, competitive YouTube, what do you actually check each morning that this should replay? So is there anything in your life that you are doing manually every single day or once a week that Claude could take off your plate? For the deliverable, I think I'd like to see a combination, a story with a link, a hook angle, and then yeah, why it matters to my audience, I think is really impactful and basically what they might get out of consuming that content. For my niche or audience, you understand this niche pretty well. Sources, let's start just with the Claude or quad code or anthropic subreddits cool so here's what it has for me so far and then it says it has three more quick questions for me to answer before it builds this out and so why I love this interview process is because it's

 you can spend 10 minutes of time now to get this part right. And it's going to save you hours of work later. So this lets me know that it basically understands the goal, but now it's asking me to more clearly define the outcome. So what does success look like? So it actually drafted this outcome rubric for me. So does the digest pass the test? If exactly five items, each with a real Reddit post and working link, each item has a distinct hook angle in your voice. Each item has a why it matters to your audience part built in items are genuinely recent and trending. This is super important. You don't want to be old news. There are no duplicate stories and the output is a clean scannable markdown file. This is awesome. So it asked me, does this look right? Do I want to tighten anything about the voice or do I want to drop the trending check? But no, this looks right to me. Do you have a past example of a digest you'd call great? I'm going to say no. Use today's first run as a baseline because again, the whole idea is that this just improves over time the more it runs. And basically what time zone am I in? I'm on the West Coast in California. So right now, it's just checking to see if I have an Anthropic API key. already set up. I know I do. So it's going to find it. But if you don't have that set up, it's super easy. Just come over to platform.claw.com and sign in with your account. From there, you can just click on the left into API keys, click create a key. And you could just name this, you know, like my agent or whatever, click add, it's going to come up with an API key, I'm going to delete this. So don't worry about it. And then all you have to do is copy this, go back into cloud code and say, hey, here's my API key. Claude just came back said everything I need is in hand. Here's the whole thing as a plan, which is pretty cool. It gives me the agent, in the CMA shape. We are setting up a daily AI digest using Opus 4.8. If you want to change the model, you can tell it to do so. This is the environment it's in, any tools that it needs, like the desired outcome, the final deliverable, the schedule that it should run on, and basically anything we need to evaluate this. But we haven't done this yet because it hasn't run. This is what's not included in version zero, which we're setting up right now. But you can see it's already making a game plan for how to improve this in the future. So does this plan look right? I'm actually going to say swap this to Sonnet because I don't think we need Opus for this. But otherwise, we are good to go. So this is awesome. Claude just went ahead and built everything for me. You can actually watch this live as it fires for the first time. You can see it actually built this managed agent for me inside of that same site, platform.claw.com. This is the system prompt that it built. If you go into sessions, these are the sessions you can check as it goes on. This is the first session right now. These are all the calls that it's making. It's going to fix itself. You can see we encounter some errors, but we know Claude's going to fix it. The other thing it did is it built overview dashboard. So if you've been building like AIOS or agentic operating systems or whatever, this is a nice way to just check in on your agent. So you can see this agent is launched and deployed. It's fully running. This is an HTML file that lives on your machine. So you can also just open this up in your browser. You could check on the outcomes or any of the next directions. And what's cool is that this will update over time as you make improvements. You can also see that we still have one running task, and this is basically just watching the loop and waiting for it to finish. And if you want to learn Claude code, like come into these things that might seem confusing at first and just read what it's saying and you can get a good understanding of what it's doing. We can see like I found two Reddit posts. I now have enough information to write the digest. Okay, the digest is written and it's saved here, right? Now we can see that all it's doing is it's actually just grading its own work. And so just by reading the response from Claude, you can actually learn a lot about how these systems work. So this is the moment of truth where we talk about the good, the bad and the ugly. So this is the digest that the system and produced, we can see it has five different articles, the story, a link, the hook angle, why this matters to my audience, et cetera, et cetera. That being said, transparently, we hit a couple of issues that honestly probably had to do a little bit with user error and a little bit with Claude, not digging deeper before building. The main issue that we hit was in this Claude managed environment, it wasn't able to actually access Reddit directly, and so this thing took 28 minutes to run, mostly because it kept getting errors when trying to access Reddit. So it actually was able to search the web and find a lot of really great relevant articles, but because it wasn't able to pull in the Reddit link directly, the system failed. Because if we come down here, we can see that one of the requirements was that each post linked to a real Reddit post. And so because we weren't able to pull those in, the system failed. And so I did spend a lot of tokens on this. You can see I spent like 27 million tokens. It was like $12 just to run this. And again, like this actually really could have been avoided. How do we know I'm going into it that we would have run into these issues with Reddit. So maybe before creating the managed agent, having the system actually check the individual pieces just to make sure that the theories are good behind the build before actually setting it up on the cloud. What's good about the system is that we have the core foundation in place. And this was sort of the whole point of running these managed agents in loop mode is that they are self-improving with every run. With each run, we learn something new about how we can make an upgrade. And so now it's just asking me, like, how do I want to fix the Reddit sourcing issue? Can I just use web search only? And this will run in like two or three minutes as opposed to 30 minutes with a bad response. And so just in setting this up for the first time today, I personally learned a lot of good lessons. If you want to continue learning Cloud Code, just check the link in the description. If you want to see how I built my own agentic OS, check out this video right here. I'll see you over there.
---
id: "30c14a20-063d-48b1-94f8-76c5d1660721"
video: "https://www.youtube.com/watch?v=DTCyvo6cC54"
name: "Every Level of a Claude Second Brain Explained"
created: "2026-06-22 16:30"
---

# Every Level of a Claude Second Brain Explained

- **Model:** whisper
- **Plik:** Every_Level_of_a_Claude_Second_Brain_Explained.mp4

---

[00:00:00 - 00:00:03] Today, I'm going to explain the different levels of building your own AI second brain.
[00:00:03 - 00:00:07] You can see here we have a visual of three very different types of data.
[00:00:07 - 00:00:10] This one is where we have our context really starting to form and we're starting to see
[00:00:10 - 00:00:15] some relationships and we're starting to see some different nodes and entities form.
[00:00:15 - 00:00:19] And then as we continue to scale this up, add more knowledge, more knowledge, more relationships,
[00:00:19 - 00:00:22] we start to get something that looks a little bit more like this, where we have
[00:00:22 - 00:00:26] clearly different clusters and inside of all of these nodes, we can see how they relate to each
[00:00:26 - 00:00:29] other. And then over here, we're taking all of those relationships a step farther,
[00:00:30 - 00:00:31] and we're able to then start to see
[00:00:31 - 00:00:32] how everything really pieces together,
[00:00:32 - 00:00:34] rather than just having files
[00:00:34 - 00:00:36] that sort of link back to each other,
[00:00:36 - 00:00:38] this is relationship mapping.
[00:00:38 - 00:00:41] And so really the idea of an AI second brain has blown up
[00:00:41 - 00:00:43] because we're all trying to get as much information
[00:00:43 - 00:00:46] out of our heads into our systems as possible.
[00:00:46 - 00:00:47] That's the true value.
[00:00:47 - 00:00:49] Your moat is your data, it's your IP.
[00:00:49 - 00:00:52] But the process of organizing that into a system
[00:00:52 - 00:00:54] so that you can use it with a bunch of different AI models
[00:00:54 - 00:00:56] and so that it can actually recall things
[00:00:56 - 00:00:57] in a way that makes sense,
[00:00:57 - 00:00:59] rather than just hallucinating or spending a bunch
[00:01:00 - 00:01:02] of your time and tokens trying to look through everything,
[00:01:02 - 00:01:03] that's the issue.
[00:01:03 - 00:01:05] So clearly all of this is my real data,
[00:01:05 - 00:01:06] and this is what the actual project looks like.
[00:01:06 - 00:01:08] It is my Herc2 project.
[00:01:08 - 00:01:10] I have a bunch of folders and files here.
[00:01:10 - 00:01:12] And at the end of the day, that's basically all it is.
[00:01:12 - 00:01:13] It is markdown files that are organized
[00:01:13 - 00:01:16] in a way that I understand and that my agents understand.
[00:01:16 - 00:01:18] And so yes, I'm gonna walk you guys through what I have here
[00:01:18 - 00:01:20] and how it works, but I also have this other project
[00:01:20 - 00:01:23] where I'm gonna show you if you're starting from scratch,
[00:01:23 - 00:01:25] or if you feel like maybe you're in between level two
[00:01:25 - 00:01:27] and three, how we can actually look at the differences
[00:01:27 - 00:01:29] and what it might look like
[00:01:30 - 00:01:33] to scale up your own systems and start to add context in different ways.
[00:01:33 - 00:01:37] So super excited to dig into this today, and I don't want to waste any of your guys' time,
[00:01:37 - 00:01:40] so let's just start looking at these five levels and how they differ.
[00:01:40 - 00:01:44] All right, so every level of a Claude Code second brain, and I'm going to be obviously
[00:01:44 - 00:01:48] kind of referring to Claude Code a lot, but keep in mind, this can be used with any AI model.
[00:01:48 - 00:01:50] I use my second brain all the time with Codex as well.
[00:01:50 - 00:01:51] I use it with Hermes Agent.
[00:01:51 - 00:01:56] This can be used by different agent harnesses because it's just files and folders.
[00:01:56 - 00:01:59] So what is the actual job of a second brain?
[00:02:00 - 00:02:01] A lot of people probably define this differently,
[00:02:01 - 00:02:02] but the way that I think about it
[00:02:02 - 00:02:05] is that it's a place for me to save notes,
[00:02:06 - 00:02:08] meeting recordings, click up threads, stuff like that.
[00:02:08 - 00:02:09] I can save it there.
[00:02:09 - 00:02:11] And then it helps me basically ingest it
[00:02:11 - 00:02:13] and get it into the right spots
[00:02:13 - 00:02:14] so that it can actually find it later.
[00:02:15 - 00:02:16] And so that's really the thing to think about
[00:02:16 - 00:02:18] is can your agent find it again?
[00:02:19 - 00:02:20] And could you find it again?
[00:02:20 - 00:02:21] Because if the answer is no,
[00:02:21 - 00:02:23] then you probably don't have the right routing
[00:02:23 - 00:02:25] or folder architecture set up,
[00:02:25 - 00:02:26] which is what I'm here to talk about today.
[00:02:27 - 00:02:29] And one other sort of mindset thing that I want to...
[00:02:30 - 00:02:34] get out there before we dive into these five levels is that you kind of have to work backwards.
[00:02:34 - 00:02:38] You want to reverse engineer based on the question. So this will start to make more sense as we get
[00:02:38 - 00:02:43] into it. But really what you should be thinking about is how do I want to use this data in the
[00:02:43 - 00:02:49] future? Because how it's going to be accessed and recalled determines the way that you put it in,
[00:02:49 - 00:02:55] in the first place. For example, a basketball hoop and a basketball. We know what shape the hoop is
[00:02:55 - 00:02:59] and we know that the ball needs to go through. So why would we ever design the ball to be
[00:03:00 - 00:03:03] a giant square because it just wouldn't fit through the hoop.
[00:03:03 - 00:03:04] So that would make no sense.
[00:03:05 - 00:03:07] So you need to start with the end in mind a little bit.
[00:03:07 - 00:03:10] Once again, I will show you exactly what I mean by that as we continue on.
[00:03:10 - 00:03:14] Because remember, we're trying to get to the point where your second brain knows everything
[00:03:14 - 00:03:17] about your business, about you, your relationships.
[00:03:17 - 00:03:21] It knows everything to the point where it probably can recall stuff better than you can
[00:03:21 - 00:03:24] because it has a better memory and it can search through things way faster than you
[00:03:24 - 00:03:24] can.
[00:03:24 - 00:03:29] So we've got five different levels to talk about and they each kind of have different
[00:03:29 - 00:03:29] questions.
[00:03:30 - 00:03:34] So level one is, can you find the file or the info by looking for an exact word or name?
[00:03:35 - 00:03:37] Level two is, can you pull everything on a certain topic together?
[00:03:38 - 00:03:40] Level three is, I searched for different words than I wrote.
[00:03:40 - 00:03:44] So semantic search, you're searching for meaning rather than an exact word match.
[00:03:45 - 00:03:47] And then trace relationship chains.
[00:03:47 - 00:03:52] Can you ask about topic X and then trace that all the way back to topic A?
[00:03:52 - 00:03:57] And then level five is just kind of making this whole second brain thing super autonomous
[00:03:57 - 00:03:59] to the point that you don't even have to think about it.
[00:04:00 - 00:04:04] And by the way, this isn't me saying that number five is best. I have some arguments about why I
[00:04:04 - 00:04:08] do not currently sit on level five. The point I'm trying to make here is each level is different,
[00:04:08 - 00:04:13] and you want to find the simplest level or the lowest level that actually fits your needs. If
[00:04:13 - 00:04:18] you don't have a pain point in your system, then I don't really think there's a need to go experiment
[00:04:18 - 00:04:25] or develop a new sort of, you know, architecture. If there's not pain, then why create more? Okay,
[00:04:25 - 00:04:29] so level one is pretty simple, and this is where you always start. So you start with a
[00:04:30 - 00:04:34] claw.md, or if you're using codecs or something, you would start with an agents.md. But you start
[00:04:34 - 00:04:38] with a claw.md, which is kind of, you know, that gets loaded up. That's almost like the system
[00:04:38 - 00:04:42] prompt for that session for that project. And then you've just got a bunch of folders and files. But
[00:04:42 - 00:04:46] the key part there is the claw.md is kind of treated as a router. So yes, you've got some,
[00:04:47 - 00:04:51] hey, this is your role. Here is what's important. But you also have routing rules. If you ever need
[00:04:51 - 00:04:55] to find information about me personally, look in this folder. If you need information about our
[00:04:55 - 00:04:59] quarter one priorities, look in this folder. Because if you've ever had a point where you ask
[00:05:00 - 00:05:03] Claude to do something and then it asks you, hey, can you give me more info? I don't know what you're
[00:05:03 - 00:05:08] talking about, but you know there's files and folders in your project, then you probably just
[00:05:08 - 00:05:13] didn't give Claude the knowledge to go look there. It's not just going to go search your entire code
[00:05:13 - 00:05:16] base automatically. I mean, you wouldn't want it to do that because it's going to waste your time
[00:05:16 - 00:05:20] and your tokens. So if it doesn't know if something lives somewhere, then it's probably not going to
[00:05:20 - 00:05:24] be able to find it. So when this is properly set up, you will stop having to re-explain things. You
[00:05:24 - 00:05:29] will talk to it and it will just know where to go look and why. But the problems with this is that if it
[00:05:30 - 00:05:32] It grows too big, it can start to get messy and feel ignored.
[00:05:32 - 00:05:36] And this is typically more of like an exact words type of search, depending on the way
[00:05:36 - 00:05:37] that you route.
[00:05:37 - 00:05:42] So if I open up my example project here, let's open up level one.
[00:05:42 - 00:05:45] So in level one, what you can see, pretend this is its own cloud project.
[00:05:45 - 00:05:46] We've got a cloud.md.
[00:05:46 - 00:05:47] So let me click into that.
[00:05:47 - 00:05:51] We can see here, it says, "This file loads automatically every time you open cloud code
[00:05:51 - 00:05:52] in this folder.
[00:05:52 - 00:05:55] It is the one file that tells the AI who you are, how you work and where things live.
[00:05:55 - 00:05:59] At level one, this file plus a few folders is your entire second brain.
[00:06:00 - 00:06:01] So here's kind of like that basic knowledge.
[00:06:01 - 00:06:03] And then right here, it's this simple.
[00:06:03 - 00:06:04] Where things live.
[00:06:04 - 00:06:06] In the context folder, always true background
[00:06:06 - 00:06:07] about you and how you work.
[00:06:07 - 00:06:08] Read this first.
[00:06:09 - 00:06:10] Projects, decision log.
[00:06:10 - 00:06:11] And that's basically it.
[00:06:11 - 00:06:13] So right here, you can see there's a context folder.
[00:06:13 - 00:06:15] We have an about me file, which you could grow.
[00:06:15 - 00:06:17] We have stack and conversations file.
[00:06:17 - 00:06:18] We have decisions.
[00:06:18 - 00:06:19] So this is a decision log
[00:06:19 - 00:06:21] where you can have your cloud.md
[00:06:21 - 00:06:24] always append new decisions and the dates
[00:06:24 - 00:06:25] whenever you make a big change to your project
[00:06:25 - 00:06:26] or to your life or to your business.
[00:06:27 - 00:06:28] And then we have projects.
[00:06:28 - 00:06:29] So this is where you could have
[00:06:30 - 00:06:34] a markdown file, or even folders within the projects for all of your ongoing projects,
[00:06:34 - 00:06:37] all of your ongoing clients, whatever it is, however you want to organize it, that's where
[00:06:37 - 00:06:41] you can have some projects. And you can even start to organize these things by dates if you want. So
[00:06:41 - 00:06:44] if you want to just have one that's for like May, and then you have all of those stuff, and you have
[00:06:44 - 00:06:47] one for June. The thing that I really want to stress here with level one, and the thing that
[00:06:47 - 00:06:53] I answer a lot in my community in the comments, is that there is not yet a standard way that has
[00:06:53 - 00:06:59] been proven the best way to set up your projects or your second brain. Besides some of the most
[00:07:00 - 00:07:06] cloud.md and whatnot. But the point I'm trying to make there is don't see what I do and think
[00:07:06 - 00:07:10] that that's the right way or see what someone else you watch does and think that that's the
[00:07:10 - 00:07:17] only right way. All that matters is do you have proper routing in place? And does it make sense
[00:07:17 - 00:07:21] to you? And does it make sense to your AI? Okay, so let's say I have my HER2 project right here,
[00:07:22 - 00:07:26] and I need to find something in here, but I can't ask AI for some reason. What I need to find is
[00:07:26 - 00:07:29] easy because I understand the drill downs. You know, I understand my base full.
[00:07:30 - 00:07:32] and let's say I'm looking for the HTML slide deck I built
[00:07:32 - 00:07:36] for my ranking Cloud Code features video.
[00:07:36 - 00:07:37] I would come into here and I say, okay,
[00:07:37 - 00:07:39] I know that's a project, so I'll go there.
[00:07:39 - 00:07:41] Within my projects, I've got another project
[00:07:41 - 00:07:42] for YouTube videos, I'll open that up.
[00:07:42 - 00:07:45] And now I know I made this video right here,
[00:07:45 - 00:07:48] May 30th, Cloud Code Top 50 features.
[00:07:48 - 00:07:50] In here, I have the actual tier list deck.
[00:07:50 - 00:07:52] And when I open that up, now I have the slide deck.
[00:07:52 - 00:07:54] And not only can I find it easily,
[00:07:54 - 00:07:56] but my agent can find it because it all makes sense
[00:07:56 - 00:07:57] and I have routing rules.
[00:07:57 - 00:07:59] Real quick, guys, if you're watching this video,
[00:08:00 - 00:08:04] you're probably interested in building your own AI operating system, lucky for you, I have a full
[00:08:04 - 00:08:07] free course on that in my free school community. The link for that is down in the description.
[00:08:07 - 00:08:11] Join the free school community, hop in here, take the seven day challenge, build your own AI
[00:08:11 - 00:08:15] operating system and apply these principles into building your second brain, which will make your
[00:08:15 - 00:08:18] AI operating system even more powerful. So links in the description. Let's get back to the video.
[00:08:19 - 00:08:24] Awesome. Okay. So that is how you start. Now, as you move up to level two, you might be able to start
[00:08:24 - 00:08:28] to work in some things like the LLM wiki, which is what I've got set up for a few different things.
[00:08:28 - 00:08:29] This is the whole cart.
[00:08:30 - 00:08:32] pathy LLM wiki, which I did make a full video about.
[00:08:32 - 00:08:34] If you want to check that out, I'll tag that right up here.
[00:08:34 - 00:08:37] But this is when you start to have more files
[00:08:37 - 00:08:39] and they start to take a bit of a different shape,
[00:08:39 - 00:08:40] and you want to organize them together
[00:08:40 - 00:08:42] in a bit of a different way.
[00:08:42 - 00:08:44] So it could be really good for researching all
[00:08:44 - 00:08:45] on a certain project.
[00:08:45 - 00:08:46] It could be really good for, you know,
[00:08:46 - 00:08:47] a few of the ones that I've got set up is
[00:08:47 - 00:08:50] my YouTube transcripts all live in their own wiki.
[00:08:50 - 00:08:51] I've got all of like my meeting transcripts
[00:08:51 - 00:08:53] that live in their own wiki.
[00:08:53 - 00:08:56] So for example, this is the obsidian view of my wiki
[00:08:56 - 00:08:58] for all of my YouTube video transcripts.
[00:08:58 - 00:08:59] You can see here, if I go to wiki,
[00:09:00 - 00:09:04] you can see there's main concepts like agentec workflows, AI coding market, context window,
[00:09:04 - 00:09:10] and all of these in here start to relate back to other tools and concepts and videos and stuff like
[00:09:10 - 00:09:15] that. So we've got the sources, we've got platforms, we've got context management techniques, and all
[00:09:15 - 00:09:21] of this was auto-created by our Cloud Code when I told it to ingest this YouTube transcript into
[00:09:21 - 00:09:24] our wiki. So I'm not going to dive super, super deep into all this right now, but definitely
[00:09:24 - 00:09:29] check out that YouTube video I linked. Now, what else is cool about this is this transcript
[00:09:30 - 00:09:35] Wiki actually lives within my main Herc 2 project. So here's Herc 2. If I go right here to Other
[00:09:35 - 00:09:41] Worlds, and then I go down to YouTube OS, and I click into the transcript Wiki right here, this
[00:09:41 - 00:09:45] is what we were just looking at in Obsidian. We could see the concepts, we could see the comparisons,
[00:09:45 - 00:09:50] we could see the sources, techniques. This is what we were looking at in Obsidian. So all Obsidian is,
[00:09:50 - 00:09:55] is it basically just visualizes your markdown files. You see here, Wiki, concepts, comparisons,
[00:09:55 - 00:09:59] techniques. This is what we were just looking at. All we get now is we just get a visual view
[00:10:00 - 00:10:03] view of all that. And so the reason I wanted to bring that up as well is because I think a lot
[00:10:03 - 00:10:08] of people obviously get pretty infatuated by that visual view. And obviously I started the
[00:10:08 - 00:10:12] video with that because I think that's what hooks a lot of people in, but all
[00:10:00 - 00:10:04] that really matters is can your system grab that and give it to you? If you are a visual person and
[00:10:04 - 00:10:09] you really want that view, then by all means install obsidian and set it up. It's super easy,
[00:10:09 - 00:10:13] but I'm saying that you don't always need that visual layer. If it's not beneficial to you,
[00:10:13 - 00:10:17] I hardly ever open obsidian just to be honest, because I know that it all lives here. And I know
[00:10:17 - 00:10:21] that my second brain and my OS can find all of that. So anyways, in level two here, let's look
[00:10:21 - 00:10:27] at this. It's very similar in shape to level one. It's just building on top of it because now we
[00:10:27 - 00:10:29] have our cloud.md, which starts to route to some other.
[00:10:30 - 00:10:34] things because it routes to the wiki and it still routes to context, projects, decisions, but it's
[00:10:34 - 00:10:39] also routing to references and memory.md. So we're just starting to add a bit more of these routing
[00:10:39 - 00:10:44] rules inside of the claw.md. We can grow the context, we can grow the decisions, we can grow
[00:10:44 - 00:10:49] projects and references, and we can also start to get this idea of memory. And what's really cool
[00:10:49 - 00:10:54] about this is you can turn on auto memory in claw code and the AI will basically start to write this
[00:10:54 - 00:10:57] file and update it on its own. So you don't have to think about it. If you come in here and you do
[00:10:57 - 00:10:59] slash memory, it'll say auto memory.
[00:11:00 - 00:11:04] on or off. And if it's off, if you want to turn that on, just turn it on. And now one thing to
[00:11:04 - 00:11:09] think about is I mentioned earlier that we want to make our second brains tool agnostic. And this
[00:11:09 - 00:11:14] is one thing that's pretty specific about Cloud Code is it uses claw.md and it uses this memory.md
[00:11:14 - 00:11:19] and it keeps that updated on its own. So if you wanted to move this over to codex, what you would
[00:11:19 - 00:11:23] do is you would first of all, transition your claw.md. You'd make a copy of it called agents.md.
[00:11:23 - 00:11:29] As you can see here in my Herc 2, I've got my, if I scroll down, claw.md right here, and then I've got
[00:11:30 - 00:11:33] agents.md right here. And they're essentially the exact same file, just so Codex can read this one
[00:11:33 - 00:11:38] and Cloud Code can read this one. But because Cloud Code keeps that auto memory, all you need to do is
[00:11:38 - 00:11:43] make sure you have that memory.md file and just tell Codex, "Hey, by the way, for memories,
[00:11:43 - 00:11:46] look in our memory.md file. It's all about the routing there." Anyways, just felt like that was
[00:11:46 - 00:11:51] important to throw out. But at a certain point, when you have these wikis, they do start to degrade
[00:11:51 - 00:11:56] a little bit. Because what's great about them is that they have indexes, right? So when your AI
[00:11:56 - 00:11:59] starts to look in the wiki, it knows, okay,
[00:12:00 - 00:12:02] If the user's asking about agentic workflows,
[00:12:02 - 00:12:03] I'm probably gonna start here.
[00:12:03 - 00:12:05] And then from here, I'm gonna drill down and read this
[00:12:05 - 00:12:08] to see what else is important to them.
[00:12:08 - 00:12:10] Maybe they're asking about the WAT framework
[00:12:10 - 00:12:11] and then I can drill into that.
[00:12:11 - 00:12:13] And maybe from there, I need to learn a little bit more
[00:12:13 - 00:12:14] about the Claude.MD system prompt,
[00:12:14 - 00:12:16] and then I will drill into that.
[00:12:16 - 00:12:18] So there are relationships here a little bit,
[00:12:18 - 00:12:21] but this isn't the same as like semantic relationships
[00:12:21 - 00:12:24] or knowledge graph relationships that have more meaning.
[00:12:24 - 00:12:27] This is more about just actually following a trail
[00:12:27 - 00:12:29] and reading the page in,
[00:12:30 - 00:12:30] its entirety.
[00:12:30 - 00:12:32] And I'll be fully honest with you guys.
[00:12:32 - 00:12:36] I pretty much sit my entire Herc 2 project in this level,
[00:12:36 - 00:12:37] in level two,
[00:12:37 - 00:12:39] because this has been working really well for me.
[00:12:39 - 00:12:40] Like I mentioned earlier,
[00:12:40 - 00:12:42] I haven't felt a pain yet big enough
[00:12:42 - 00:12:43] to switch over to level two.
[00:12:43 - 00:12:44] And here's what I meant by that.
[00:12:44 - 00:12:45] My wiki has links.
[00:12:45 - 00:12:46] Isn't that a knowledge graph?
[00:12:47 - 00:12:48] Not exactly,
[00:12:48 - 00:12:51] because this doesn't have connections
[00:12:51 - 00:12:52] of how they are related.
[00:12:52 - 00:12:53] Like this is endorsed by this,
[00:12:54 - 00:12:55] or this has cron to here.
[00:12:55 - 00:12:57] These just have connections
[00:12:57 - 00:12:59] because it's like a C also.
[00:13:00 - 00:13:03] It's like backlinks. So they're very similar. And yes, they can achieve a similar effect,
[00:13:04 - 00:13:08] but it's still a little bit different. Anyways, let's take a look at level three, which is where
[00:13:08 - 00:13:12] you start to do things like semantic search. Whether you do that in Obsidian, whether you do
[00:13:12 - 00:13:17] that with Pinecone or Supabase, however you start to grab the actual semantic search,
[00:13:18 - 00:13:23] that is what level three is. And so just as a quick visual for you guys, let's take a look at
[00:13:23 - 00:13:29] this quadrant cluster of images. So every one of these vector points is an image. And the
[00:13:30 - 00:13:34] what we see in here is the payload is stuff like the file name, the URL, the name of the author
[00:13:34 - 00:13:38] or the artist and the URL, but we don't actually see like what's in the image. We don't get a
[00:13:38 - 00:13:44] description. So what we have to do is we have to organize these images by meaning or by similarity.
[00:13:44 - 00:13:48] So when I open up this graph and we start to visualize this stuff here, what you see is that
[00:13:48 - 00:13:53] we have this main image, these owls, these kind of like, I don't even know. It's a very trippy
[00:13:53 - 00:13:59] style, like hallucinogenic style. Anyways, then this one is kind of similar, right? It's got those
[00:14:00 - 00:14:02] This one is also similar, but they're not the same.
[00:14:03 - 00:14:04] They just share similarities.
[00:14:04 - 00:14:06] And as we start to expand these more and more,
[00:14:06 - 00:14:08] we can start to get into different styles.
[00:14:09 - 00:14:11] So this one has like some creepy eyes and mushrooms or whatever.
[00:14:11 - 00:14:13] This one is kind of more down that fantasy lane.
[00:14:13 - 00:14:16] And as we start to build out more of these relationships and meanings,
[00:14:17 - 00:14:19] we can expand and grow away from them.
[00:14:19 - 00:14:21] And so Quadrant really just gives you a visualization here.
[00:14:21 - 00:14:24] I mean, it has clusters and vector store.
[00:14:24 - 00:14:27] But the reason I pulled this up as a demo is just because we start to see
[00:14:27 - 00:14:29] the actual relationships form here.
[00:14:30 - 00:14:31] based on meaning.
[00:14:31 - 00:14:33] And that's what's important about semantic search
[00:14:33 - 00:14:35] is that we're no longer doing keyword matching,
[00:14:35 - 00:14:36] we're searching based on meaning.
[00:14:36 - 00:14:40] So here in my YouTube transcript second brain,
[00:14:40 - 00:14:42] if I go to the smart lookup over here,
[00:14:42 - 00:14:44] this is very different from just the regular search.
[00:14:45 - 00:14:50] So for example, if I search here for feedback, let's say,
[00:14:50 - 00:14:53] we're actually doing a match on the word feedback
[00:14:53 - 00:14:56] and it's only showing me where that word actually appears
[00:14:56 - 00:14:58] inside of our second brain.
[00:14:58 - 00:14:59] But if I come over here,
[00:15:00 - 00:15:05] in the smart lookup and I search for feedback, we are getting matches that have things in here that
[00:15:05 - 00:15:10] mean feedback. So live test results, cloud code skills, which was talking about evaluations and
[00:15:10 - 00:15:14] stuff. So there's a big difference between keyword matching and semantic search, you know,
[00:15:14 - 00:15:19] similarity matching. This one over here is saying X equals X. And this one is saying X is similar to
[00:15:19 - 00:15:24] X, Y, and Z. And so this all just goes back to vector databases. I've talked so, so much about
[00:15:24 - 00:15:29] vector databases. So I'm not going to dive super deep in. I've got so many resources on my channel, but
[00:15:30 - 00:15:34] But basically what it is, is we take a document, so let's just say a YouTube transcript, we
[00:15:34 - 00:15:38] chunk it up, and then each chunk is ran through an embeddings model.
[00:15:38 - 00:15:43] And the embeddings model puts that chunk of text onto a three-dimensional space where
[00:15:43 - 00:15:45] space is related to meaning.
[00:15:45 - 00:15:49] And so it decides, okay, this chunk is about a company, so we're going to put it up here.
[00:15:49 - 00:15:51] This chunk is about finances, so it's going to go here.
[00:15:51 - 00:15:55] And we start to see these vectors form near other similar vectors.
[00:15:55 - 00:15:59] Now, do you guys remember how I said earlier, you want to think about how is the data going
[00:16:00 - 00:16:02] What type of questions are you gonna ask?
[00:16:02 - 00:16:03] This is a reason why that's so important.
[00:16:03 - 00:16:04] So think about this.
[00:16:04 - 00:16:08] Let's say I put my meeting transcript of March 5th meeting
[00:16:08 - 00:16:12] into my second brain, and I put those in as, you know,
[00:16:12 - 00:16:13] vectorized chunks.
[00:16:13 - 00:16:15] So let's say when I vectorize that meeting,
[00:16:15 - 00:16:18] we actually get, you know, like 20 chunks.
[00:16:18 - 00:16:21] It actually creates 20 chunks or however many that is.
[00:16:21 - 00:16:22] And then when I say, "Hey, Mr. AI agent,
[00:16:22 - 00:16:25] can you summarize the meeting on March 5th?"
[00:16:25 - 00:16:29] It will basically search for March 5th meeting summary.
[00:16:30 - 00:16:33] And it will pull chunks that are similar to March 5th meeting summary.
[00:16:33 - 00:16:37] And then even if it gets the right chunks, it's going to only summarize those five chunks.
[00:16:37 - 00:16:42] It's not able to look at the entire meeting summary, or sorry, like meeting transcript
[00:16:42 - 00:16:43] in entirety.
[00:16:43 - 00:16:44] So it doesn't really know a summary.
[00:16:45 - 00:16:46] It might be missing a lot of key information.
[00:16:46 - 00:16:49] Now, yes, there are things you can start to play with there, like metadata and other things
[00:16:49 - 00:16:51] like that to make these results better.
[00:16:51 - 00:16:56] But at the end of the day, people kind of assume that a vector database was some magic
[00:16:56 - 00:16:58] solution where it could always pull back what you need.
[00:16:58 - 00:16:59] But that is very false.
[00:17:00 - 00:17:01] And I mean, think about it like this.
[00:17:01 - 00:17:03] Let's say we have a table and we say,
[00:17:03 - 00:17:04] hey, which week do we have the highest sales?
[00:17:05 - 00:17:07] Okay, the agent looks for highest sales.
[00:17:07 - 00:17:10] It maybe grabs this chunk outlined in gray of data.
[00:17:10 - 00:17:13] And then it looks like, okay, week six here was the highest sales.
[00:17:13 - 00:17:14] So that must be the answer.
[00:17:15 - 00:17:17] But in reality, you can see week 14 was higher.
[00:17:17 - 00:17:18] Week 19 was higher.
[00:17:18 - 00:17:22] So when you need something that has actual full context,
[00:17:22 - 00:17:25] then you can't do the vector database chunking.
[00:17:25 - 00:17:29] That's where you'd rather just have a markdown file of March 5th
[00:17:30 - 00:17:34] And then all this agent would have to do is read that entire Markdown file and then give you a summary.
[00:17:34 - 00:17:36] And that's just going to be more accurate.
[00:17:36 - 00:17:42] So in this project, if we open up level three, you can see it's very similar because you can still have context files, decision files.
[00:17:42 - 00:17:44] You can still have all that.
[00:17:44 - 00:17:52] And then you might identify, okay, actually, this one specific unit of my business, maybe my YouTube transcripts, maybe I want just that to be a vector database.
[00:17:53 - 00:17:56] But I still want my context and my projects and my decisions to be Markdown files.
[00:18:00 - 00:18:01] Just because you have a second brain,
[00:18:01 - 00:18:04] and just because you have a massive folder here
[00:18:04 - 00:18:05] with a bunch of folders and files,
[00:18:05 - 00:18:09] doesn't mean that the whole folder needs to be one style.
[00:18:09 - 00:18:11] Doesn't mean that everything needs GraphRack.
[00:18:11 - 00:18:13] Doesn't mean that everything is just LLM wiki.
[00:18:13 - 00:18:14] It means that you're able to decide
[00:18:14 - 00:18:16] based on the type of data and the way you use it,
[00:18:17 - 00:18:19] how can you structure this specific folder
[00:18:19 - 00:18:20] in the way you want it?
[00:18:20 - 00:18:21] So here we have a vector index folder
[00:18:21 - 00:18:23] and we click on the how search works.
[00:18:23 - 00:18:27] It works by chunking, embedding, search, hybrid, re-ranking.
[00:18:27 - 00:18:29] There's some things you can get really, really nitty
[00:18:30 - 00:18:34] gritty on when it comes to semantic search. But what vector retrieval is really, really good at
[00:18:34 - 00:18:38] is looking at tons and tons of data, typically just like a lot of text. And when you need a very
[00:18:38 - 00:18:43] specific answer, something that's very similar. So if you had a thousand rules that you needed to
[00:18:43 - 00:18:49] store and you basically said, Hey, um, can you remind me what rule 17 was? That might be a really
[00:18:49 - 00:18:54] good use case for vector search because it's able to search for rule 17, pull in those chunks and
[00:18:54 - 00:18:59] just give you a little snippet because it would be a waste of time and tokens for your agent to read the entire markdown
[00:19:00 - 00:19:04] file of all a thousand rules, if you just needed rule 17. So that's kind of the difference there.
[00:19:04 - 00:19:08] Like I said, I've got so many videos on vector stuff on my channel, but really you could say,
[00:19:09 - 00:19:13] Hey, to your cloud code agent, I have this data. Here's how I want to use it. Do you think this
[00:19:13 - 00:19:17] would be better for now as markdown files? Or should I do semantic search? Like what would
[00:19:17 - 00:19:20] actually make more sense here? And it will help walk you through the way that you should actually
[00:19:20 - 00:19:26] set that up. So now I hope you guys are starting to understand why I said, you know, moving up on,
[00:19:26 - 00:19:29] or I'm sorry, like moving up on levels, moving down doesn't necessarily mean better
[00:19:30 - 00:19:32] it's all about figuring out what is the pain point
[00:19:32 - 00:19:33] with what you're currently doing
[00:19:33 - 00:19:36] and where would a different level help you out
[00:19:36 - 00:19:37] and fix that pain point.
[00:19:37 - 00:19:39] Okay, so now let's take a look at level four.
[00:19:39 - 00:19:41] This is where we start to get into like knowledge graphs
[00:19:41 - 00:19:42] and relationship graphs,
[00:19:43 - 00:19:45] which typically are gonna be the most complex
[00:19:45 - 00:19:47] and sometimes the most expensive as well.
[00:19:47 - 00:19:48] If you're doing it on a certain platform,
[00:19:48 - 00:19:49] you could always use open source software,
[00:19:50 - 00:19:52] but anyways, knowledge graphs.
[00:19:52 - 00:19:53] And I also wanna be upfront.
[00:19:53 - 00:19:54] I've played with these a lot,
[00:19:54 - 00:19:56] but I do not actually use these on the day-to-day
[00:19:56 - 00:19:59] because I found out just other ways to use
[00:20:00 - 00:20:04] routing files and wikis that fit my needs. Now, my work is very different than what a lot of your
[00:20:04 - 00:20:10] guys' work may be. Mine is very project-based and it is very, you know, content heavy. I don't have
[00:20:00 - 00:20:05] a massive CRM to manage with a bunch of different businesses and clients, you know? And if I did,
[00:20:05 - 00:20:08] maybe a knowledge graph would make a lot more sense and it probably would. But typically the
[00:20:08 - 00:20:13] cool part about that is if you identify that you needed a knowledge graph, let's say for all your
[00:20:13 - 00:20:18] projects, you needed, you wanted to put all of this in a knowledge graph, the data probably already
[00:20:18 - 00:20:23] exists here. And that's the thing about building out these relationships in your knowledge graph
[00:20:23 - 00:20:27] is that the system, whatever software you use is typically going to be pretty good at embedding that
[00:20:27 - 00:20:29] and creating that. But the problem that you're going to have, you know,
[00:20:30 - 00:20:31] you have to solve is you have to give it enough data.
[00:20:32 - 00:20:33] And so one thing that I really like to do
[00:20:33 - 00:20:35] is I like to have these brainstorm sessions,
[00:20:35 - 00:20:35] as you can see.
[00:20:36 - 00:20:38] And what I do with these brainstorm sessions
[00:20:38 - 00:20:39] is I use a skill called Grill Me.
[00:20:40 - 00:20:42] So if you see here, I have a skill called Grill Me,
[00:20:42 - 00:20:43] which I originally got from Matt Pocock.
[00:20:43 - 00:20:44] I customized it a little bit.
[00:20:45 - 00:20:47] I'll leave the skill for Grill Me
[00:20:47 - 00:20:48] in my free school community.
[00:20:48 - 00:20:49] The link for that is down in the description.
[00:20:50 - 00:20:51] All you have to do is hop in here, go to classroom,
[00:20:52 - 00:20:53] click on all YouTube resources,
[00:20:53 - 00:20:55] and you can find all the skills and everything like that.
[00:20:55 - 00:20:57] But the skill, what that does
[00:20:57 - 00:20:58] is it basically just grills me.
[00:20:58 - 00:20:59] It interviews me relentlessly.
[00:21:00 - 00:21:03] about a certain topic, and it creates a brainstorm file here.
[00:21:03 - 00:21:05] It only stops when it knows everything about it.
[00:21:05 - 00:21:07] So if you wanted to start building up a knowledge graph
[00:21:07 - 00:21:09] for all your clients and businesses,
[00:21:09 - 00:21:11] just say grill me about client A, grill me about client B,
[00:21:11 - 00:21:13] grill me about business A.
[00:21:13 - 00:21:14] And it would just ask you questions,
[00:21:14 - 00:21:16] and you can feed it files, you can give it stuff,
[00:21:16 - 00:21:17] you can feed it in transcripts,
[00:21:17 - 00:21:20] you can feed it in contracts, whatever it is.
[00:21:20 - 00:21:23] And that's how you can start to form a lot of data.
[00:21:23 - 00:21:24] Hey guys, me again, real quick.
[00:21:24 - 00:21:25] I'm editing this video, and I realized
[00:21:25 - 00:21:27] that I needed to throw out one thing here,
[00:21:27 - 00:21:29] which is that obviously,
[00:21:30 - 00:21:31] if you're putting all of this data
[00:21:31 - 00:21:33] and you're sending it all to Anthropic,
[00:21:33 - 00:21:34] to Claude Models,
[00:21:34 - 00:21:35] then that's not private.
[00:21:36 - 00:21:37] So if you feel comfortable with that,
[00:21:37 - 00:21:38] that's fine.
[00:21:38 - 00:21:40] I am putting a lot of my data in there
[00:21:40 - 00:21:41] and it is my business stuff
[00:21:41 - 00:21:43] and that's what I'm doing.
[00:21:43 - 00:21:45] But if you don't feel comfortable with that
[00:21:45 - 00:21:46] or you don't want to send client data,
[00:21:47 - 00:21:47] of course you don't,
[00:21:48 - 00:21:49] then maybe you want to do that
[00:21:49 - 00:21:50] through open source models.
[00:21:50 - 00:21:51] And maybe Claude Code
[00:21:51 - 00:21:52] isn't where you have the second brain
[00:21:52 - 00:21:54] that has every single piece of information
[00:21:54 - 00:21:56] about you and your business
[00:21:56 - 00:21:57] and your client's business.
[00:21:57 - 00:21:59] So the point I'm trying to make here is just
[00:22:00 - 00:22:00] This is what I'm doing.
[00:22:00 - 00:22:05] I'm obviously aware of the fact that my data goes to Anthropic when I process it through
[00:22:05 - 00:22:06] Claude.
[00:22:06 - 00:22:08] And if you guys are doing that, then you should also be aware of that.
[00:22:09 - 00:22:11] But there are other options if you can't do that.
[00:22:11 - 00:22:11] So I had to throw that out there.
[00:22:11 - 00:22:16] I am planning to make a ton of videos here soon about local AI and open source models
[00:22:16 - 00:22:19] and all this stuff because it's a really, really exciting space that I think is going
[00:22:19 - 00:22:20] to start becoming bigger and bigger.
[00:22:21 - 00:22:22] So yeah, keep that in mind.
[00:22:22 - 00:22:23] Back to the video.
[00:22:23 - 00:22:29] I think sometimes that's a misconception about how I got here and how people build their own
[00:22:30 - 00:22:35] AIOS or SecondBrain is that they think the problem is the system not retrieving it great,
[00:22:35 - 00:22:39] which sometimes it is, but sometimes it seems like the bigger problem is getting everything
[00:22:39 - 00:22:45] out of your brain into the system. So before you blame AI, take a look at your folders and files
[00:22:45 - 00:22:51] and say, is this actually holistic? Does this have all the nuance that I have in my brain?
[00:22:51 - 00:22:55] Anyways, from there, when you open up level four, you can see that it's very similar still.
[00:22:55 - 00:22:59] We're just adding on a few things. You can see here, we've added an agents.md.
[00:23:00 - 00:23:01] which is the exact same as the Cloud.MD.
[00:23:01 - 00:23:03] And what else is cool is you can literally just reference
[00:23:03 - 00:23:05] inside of your Cloud.MD at agents.MD,
[00:23:05 - 00:23:06] and then you can delete all this
[00:23:06 - 00:23:10] because this basically just like injects that file into here.
[00:23:10 - 00:23:11] But I just wanted to show that.
[00:23:11 - 00:23:12] But anyways, you can see
[00:23:12 - 00:23:13] we're still following the same principles.
[00:23:13 - 00:23:14] We have a wiki.
[00:23:15 - 00:23:16] We've also added a knowledge graph layer.
[00:23:17 - 00:23:19] We've still got the same where things live with the routing
[00:23:19 - 00:23:21] with all these just regular folders and boring markdown,
[00:23:21 - 00:23:23] but boring is beautiful.
[00:23:23 - 00:23:24] You can see that our memory is still here.
[00:23:24 - 00:23:25] It's starting to grow.
[00:23:25 - 00:23:27] And we just keep building on top of this.
[00:23:28 - 00:23:29] So one thing we added
[00:23:30 - 00:23:33] here, as you can see, was our knowledge graph folder. And so what happens here is we get
[00:23:33 - 00:23:37] different entities, right? So like we can see, okay, Jordan is a person, Acme is a company,
[00:23:37 - 00:23:41] and then we can start to form relationships between all these things. So Jordan works at
[00:23:41 - 00:23:47] Acme. Acme is endorsed by Postpilot. Postpilot is a competitor of Cadently. And it starts to build
[00:23:47 - 00:23:52] out not only these entities, but it shows you how they're all related. And so that's why when I said
[00:23:52 - 00:23:59] that I really like using, you know, this, um, what's it called? LLM wiki is because I have enough of that feel of all these relationships.
[00:24:00 - 00:24:02] because I've put so much time and effort
[00:24:02 - 00:24:04] into ingesting these in the right way
[00:24:04 - 00:24:05] and giving it context.
[00:24:05 - 00:24:06] The thing about this one is that
[00:24:06 - 00:24:09] it has to read every single file it wants.
[00:24:09 - 00:24:11] Maybe it was looking at AI video production
[00:24:11 - 00:24:13] and all it needed to know was 11 labs.
[00:24:14 - 00:24:16] It still would have read this entire file first.
[00:24:17 - 00:24:19] And so that's where sometimes the knowledge graph
[00:24:19 - 00:24:21] is actually more lightweight in that sense.
[00:24:21 - 00:24:22] And this is the example I showed
[00:24:22 - 00:24:24] at the beginning of the video where we have light rag
[00:24:24 - 00:24:26] and forgive me, I'm gonna have to blur some of this stuff out
[00:24:26 - 00:24:27] because this is like legitimately
[00:24:27 - 00:24:29] my entire second brain in our business.
[00:24:30 - 00:24:34] But as I really zoom in here, and this kind of slows down my computer because there's so much,
[00:24:34 - 00:24:37] but what you'll notice is that we actually start to get relationships.
[00:24:37 - 00:24:40] I probably shouldn't have done this with so much data, but you can see like,
[00:24:40 - 00:24:42] we have this collaborates with that.
[00:24:42 - 00:24:44] We have this builds that.
[00:24:44 - 00:24:49] And so if I really started to open up all of these little, you know, circles,
[00:24:49 - 00:24:52] we could see what was going on and how they're all related.
[00:24:52 - 00:24:55] We could see that our seven-day AIS challenge, it was provided from YouTube.
[00:24:55 - 00:24:59] It connects to the onboarding process of AIS+.
[00:25:00 - 00:25:01] It was developed by Aiden.
[00:25:01 - 00:25:04] And so we can basically follow around these relationships
[00:25:04 - 00:25:05] as you see.
[00:25:05 - 00:25:06] And even though it's pretty much the same data
[00:25:06 - 00:25:07] that you see here in Obsidian,
[00:25:07 - 00:25:09] we're not getting that same level of relationships
[00:25:09 - 00:25:10] between these different entities.
[00:25:10 - 00:25:13] So anyways, if you guys wanna see a full breakdown video
[00:25:13 - 00:25:16] on something like LightRag or Graphify,
[00:25:16 - 00:25:17] or all the other solutions that there are out there
[00:25:17 - 00:25:20] for more of a knowledge graph, relationship graph,
[00:25:20 - 00:25:20] then let me know.
[00:25:20 - 00:25:22] But that is kind of the difference there.
[00:25:22 - 00:25:24] So if you don't need those sort of relationship chains
[00:25:24 - 00:25:27] and you're not worried about that semantic type
[00:25:27 - 00:25:29] of relationships, then you probably don't need
[00:25:30 - 00:25:31] to use something like a knowledge graph.
[00:25:31 - 00:25:35] And then level five, we have more of the always on brain OS,
[00:25:35 - 00:25:37] and something like G-Brain.
[00:25:37 - 00:25:41] Gary Tan, CEO of Y Combinator, he created this thing called G-Brain,
[00:25:41 - 00:25:43] which pairs really well with G-Stack.
[00:25:43 - 00:25:46] But G-Brain is kind of the idea of everything we've talked about here.
[00:25:46 - 00:25:48] Wikis, routing, relationships, tools.
[00:25:48 - 00:25:51] But G-Brain has kind of that always on element,
[00:25:51 - 00:25:56] because it is like constantly syncing and refreshing memories and adding more stuff.
[00:25:56 - 00:25:59] So adding in G-Brain to something like a Hermes agent would be really, really good.
[00:26:00 - 00:26:01] You can still do it in cloud code,
[00:26:01 - 00:26:02] but you'd have to handle those crons
[00:26:02 - 00:26:03] and get all that stuff set up,
[00:26:03 - 00:26:05] which is why I don't currently run G-Brain at the moment,
[00:26:05 - 00:26:08] but I have been playing around with it with my Hermes agent.
[00:26:08 - 00:26:10] So anyways, the point here is that it's very similar
[00:26:10 - 00:26:12] to everything else we've just talked about.
[00:26:12 - 00:26:14] It's just having that auto-updating feel,
[00:26:15 - 00:26:16] more of the autonomous, always-on feel.
[00:26:17 - 00:26:20] But I will say, another thing that kind of scares me
[00:26:20 - 00:26:22] about that is you have this whole dilemma of,
[00:26:23 - 00:26:26] you know, when do you have too much context?
[00:26:26 - 00:26:27] And when does it get to the point
[00:26:27 - 00:26:29] where it's actually doing more damage than it's doing good?
[00:26:30 - 00:26:34] And the reason I bring that up is because I am in complete control of what my second
[00:26:34 - 00:26:35] brain ingests.
[00:26:35 - 00:26:38] I will run a skill to go grab all of my meeting transfers in the week.
[00:26:38 - 00:26:40] I will say, "Hey, here's something.
[00:26:40 - 00:26:43] Help me figure out, like, help me brainstorm about this and then let's ingest it together."
[00:26:43 - 00:26:47] And for me, I really like being in that control because in my mind, there's a big difference
[00:26:47 - 00:26:48] between a few types of data.
[00:26:48 - 00:26:52] If you guys remember in my like AIOS videos, I've talked about the four C's.
[00:26:52 - 00:26:54] So context, connections, capabilities, and cadence.
[00:26:54 - 00:26:57] And for the second brain, I mainly think about it as just these first two.
[00:26:57 - 00:26:59] So context and connections.
[00:27:00 - 00:27:04] And so when I think of context, that's stuff like, you know, what my business has done.
[00:27:04 - 00:27:10] So if I come into here, into my second brain, and you can see here, if I go to up at OTAs,
[00:27:10 - 00:27:14] so OTAs are basically just our projects for the quarter. And so here I can see all the Q1 ones,
[00:27:14 - 00:27:17] right? I can look at all those and I can click at them and see decisions that we've made in the
[00:27:17 - 00:27:22] statuses. And I can also see Q2 OTAs. So I can see what's going on here. And my second brain is able
[00:27:22 - 00:27:26] to see that because that has been basically, those are locked in decisions. This is what we're doing
[00:27:26 - 00:27:29] this quarter. And then I'm updating the statuses of that stuff. So that's like,
[00:27:30 - 00:27:34] context that's what's going on in the business but when it comes to connections if I go back to this
[00:27:34 - 00:27:39] this is more of like the real data that isn't as evergreen this is stuff that changes this is like
[00:27:39 - 00:27:44] slack threads this is emails this is a customer data and that type of data you don't want to
[00:27:44 - 00:27:49] ingest into a second brain because that's just noise then then you have to go back every month
[00:27:49 - 00:27:53] and like delete old stuff so the way that I like to think about my actual second brain is stuff that
[00:27:53 - 00:27:58] I'm not going to delete this is stuff that is like okay in a year will it be good for me to have this
[00:27:58 - 00:27:59] memory in here yes
[00:28:00 - 00:28:05] Otherwise, it's just adding noise. So when you're adding data into your project, think about it like
[00:28:05 - 00:28:09] the context and connections. Think about if this is kind of like more evergreen, holistic data,
[00:28:09 - 00:28:14] or if this is more things that are going to change next week. So you probably shouldn't pull it in,
[00:28:14 - 00:28:18] but you should make sure that your second brain has access to go grab it. So that way, if I said
[00:28:18 - 00:28:23] to my second brain, hey, can you just take a look real quick at what John and I were talking about
[00:28:23 - 00:28:29] last week about, you know, OTA number seven, it would first go to our OTA file and it would
[00:28:30 - 00:28:33] it would try to find it there. If it couldn't find it there, it would look through the wiki and it
[00:28:33 - 00:28:36] would look through meeting transcripts and see what we talked about there. And if it couldn't
[00:28:36 - 00:28:40] find it there, it would finally go to ClickUp itself, pull real data in from me and John's
[00:28:40 - 00:28:44] conversations and see if the answer lived there. And so that in my mind is still a second brain
[00:28:44 - 00:28:49] because I'm able to ask a vague question and the second brain knows exactly where to look in what
[00:28:49 - 00:28:53] order to find that real-time data and then give me back the answer that I need. That's the question
[00:28:53 - 00:28:57] I ask myself is, does this thing understand where my data lives and where to look and can it give me
[00:28:57 - 00:28:59] accurate answers? So as far as,
[00:29:00 - 00:29:04] finding your level, remember, your whole project doesn't fit into one level. Maybe this folder's
[00:29:04 - 00:29:07] level two, maybe this folder's level four, maybe this folder's level three. Here's some things to
[00:29:07 - 00:29:12] think about. If you are re-explaining your setup and you need to find things by exact words or files,
[00:29:12 - 00:29:16] look at level one. If you have 30 plus notes and you keep forgetting what's in them, look at level
[00:29:16 - 00:29:20] two. That's where you sort of like ingest them and get that wiki with relationships. If your project
[00:29:20 - 00:29:25] is just completely whiffing on notes that you know exist and your routing isn't working, then maybe
[00:29:25 - 00:29:29] you want to look for something more like a semantic search that doesn't rely on an exact
[00:29:30 - 00:29:59] word level match. If you're looking for relationships and to be able to follow chains of questions and thoughts, then you probably want to look for something like a knowledge graph. And if you're running agents offline and you've got so much data and you want to sync up a bunch of Hermes agents together, then you probably are looking for something like level five, something like G brain. And another topic that I get some questions about, which I'm not going to fully address in this video, but I will briefly bring up is the fact that you are building your own second brain OS. So are other people on your team. The next question is, how do you actually make sure that everyone's data
[00:30:00 - 00:30:04] is syncing together and how do you have more of like your team second brain there's a lot of
[00:30:04 - 00:30:08] different ways to solve that i think once again it's not an issue of oh do we use google drive
[00:30:08 - 00:30:11] or notion or github or cloud plugins i think the
[00:30:00 - 00:30:05] issue to figure out with your team is how do we actually make sure that we all habit shift so that
[00:30:05 - 00:30:09] this stuff is actually useful and not just noise? How do we make sure that process owners are
[00:30:09 - 00:30:13] updating their docs and syncing their stuff there? How do we make sure that other people are pulling
[00:30:13 - 00:30:18] from that rather than always just pinging the same people for questions and answers all the time?
[00:30:18 - 00:30:22] I think the adoption and the change management question is the bigger one. The tech and the way
[00:30:22 - 00:30:29] it actually functionally rolls out is a little bit less. But what I do know is that you getting set up
[00:30:30 - 00:30:31] how it works, how you should route,
[00:30:31 - 00:30:32] how you should make the decisions
[00:30:32 - 00:30:33] of where the data should live.
[00:30:34 - 00:30:35] That's the first hurdle.
[00:30:35 - 00:30:37] You can only solve the team-wide problem
[00:30:37 - 00:30:38] once you feel comfortable
[00:30:38 - 00:30:40] about the way you run it every single day
[00:30:40 - 00:30:41] and then it works for you.
[00:30:41 - 00:30:42] That is gonna do it for today.
[00:30:42 - 00:30:43] Like I said, you guys can grab all the skills
[00:30:43 - 00:30:46] and everything that you need from this free community.
[00:30:47 - 00:30:48] The link for that's down in the description.
[00:30:48 - 00:30:49] I will also include the slide deck
[00:30:49 - 00:30:50] if you guys are interested in flipping through.
[00:30:50 - 00:30:52] So if you guys enjoy the video
[00:30:52 - 00:30:52] or you learned something new,
[00:30:53 - 00:30:54] please give it a like, it helps me out a ton.
[00:30:54 - 00:30:55] And as always, I appreciate you guys
[00:30:55 - 00:30:56] making it to the end of the video
[00:30:56 - 00:30:58] and I will see you all in the next one.
[00:30:58 - 00:30:59] Thanks guys.

---

## Pełny tekst

 Today, I'm going to explain the different levels of building your own AI second brain. You can see here we have a visual of three very different types of data. This one is where we have our context really starting to form and we're starting to see some relationships and we're starting to see some different nodes and entities form. And then as we continue to scale this up, add more knowledge, more knowledge, more relationships, we start to get something that looks a little bit more like this, where we have clearly different clusters and inside of all of these nodes, we can see how they relate to each other. And then over here, we're taking all of those relationships a step farther, and we're able to then start to see how everything really pieces together, rather than just having files that sort of link back to each other, this is relationship mapping. And so really the idea of an AI second brain has blown up because we're all trying to get as much information out of our heads into our systems as possible. That's the true value. Your moat is your data, it's your IP. But the process of organizing that into a system so that you can use it with a bunch of different AI models and so that it can actually recall things in a way that makes sense, rather than just hallucinating or spending a bunch of your time and tokens trying to look through everything, that's the issue. So clearly all of this is my real data, and this is what the actual project looks like. It is my Herc2 project. I have a bunch of folders and files here. And at the end of the day, that's basically all it is. It is markdown files that are organized in a way that I understand and that my agents understand. And so yes, I'm gonna walk you guys through what I have here and how it works, but I also have this other project where I'm gonna show you if you're starting from scratch, or if you feel like maybe you're in between level two and three, how we can actually look at the differences and what it might look like to scale up your own systems and start to add context in different ways. So super excited to dig into this today, and I don't want to waste any of your guys' time, so let's just start looking at these five levels and how they differ. All right, so every level of a Claude Code second brain, and I'm going to be obviously kind of referring to Claude Code a lot, but keep in mind, this can be used with any AI model. I use my second brain all the time with Codex as well. I use it with Hermes Agent. This can be used by different agent harnesses because it's just files and folders. So what is the actual job of a second brain? A lot of people probably define this differently, but the way that I think about it is that it's a place for me to save notes, meeting recordings, click up threads, stuff like that. I can save it there. And then it helps me basically ingest it and get it into the right spots so that it can actually find it later. And so that's really the thing to think about is can your agent find it again? And could you find it again? Because if the answer is no, then you probably don't have the right routing or folder architecture set up, which is what I'm here to talk about today. And one other sort of mindset thing that I want to... get out there before we dive into these five levels is that you kind of have to work backwards. You want to reverse engineer based on the question. So this will start to make more sense as we get into it. But really what you should be thinking about is how do I want to use this data in the future? Because how it's going to be accessed and recalled determines the way that you put it in, in the first place. For example, a basketball hoop and a basketball. We know what shape the hoop is and we know that the ball needs to go through. So why would we ever design the ball to be a giant square because it just wouldn't fit through the hoop. So that would make no sense. So you need to start with the end in mind a little bit. Once again, I will show you exactly what I mean by that as we continue on. Because remember, we're trying to get to the point where your second brain knows everything about your business, about you, your relationships. It knows everything to the point where it probably can recall stuff better than you can because it has a better memory and it can search through things way faster than you can. So we've got five different levels to talk about and they each kind of have different questions. So level one is, can you find the file or the info by looking for an exact word or name? Level two is, can you pull everything on a certain topic together? Level three is, I searched for different words than I wrote. So semantic search, you're searching for meaning rather than an exact word match. And then trace relationship chains. Can you ask about topic X and then trace that all the way back to topic A? And then level five is just kind of making this whole second brain thing super autonomous to the point that you don't even have to think about it. And by the way, this isn't me saying that number five is best. I have some arguments about why I do not currently sit on level five. The point I'm trying to make here is each level is different, and you want to find the simplest level or the lowest level that actually fits your needs. If you don't have a pain point in your system, then I don't really think there's a need to go experiment or develop a new sort of, you know, architecture. If there's not pain, then why create more? Okay, so level one is pretty simple, and this is where you always start. So you start with a claw.md, or if you're using codecs or something, you would start with an agents.md. But you start with a claw.md, which is kind of, you know, that gets loaded up. That's almost like the system prompt for that session for that project. And then you've just got a bunch of folders and files. But the key part there is the claw.md is kind of treated as a router. So yes, you've got some, hey, this is your role. Here is what's important. But you also have routing rules. If you ever need to find information about me personally, look in this folder. If you need information about our quarter one priorities, look in this folder. Because if you've ever had a point where you ask Claude to do something and then it asks you, hey, can you give me more info? I don't know what you're talking about, but you know there's files and folders in your project, then you probably just didn't give Claude the knowledge to go look there. It's not just going to go search your entire code base automatically. I mean, you wouldn't want it to do that because it's going to waste your time and your tokens. So if it doesn't know if something lives somewhere, then it's probably not going to be able to find it. So when this is properly set up, you will stop having to re-explain things. You will talk to it and it will just know where to go look and why. But the problems with this is that if it It grows too big, it can start to get messy and feel ignored. And this is typically more of like an exact words type of search, depending on the way that you route. So if I open up my example project here, let's open up level one. So in level one, what you can see, pretend this is its own cloud project. We've got a cloud.md. So let me click into that. We can see here, it says, "This file loads automatically every time you open cloud code in this folder. It is the one file that tells the AI who you are, how you work and where things live. At level one, this file plus a few folders is your entire second brain. So here's kind of like that basic knowledge. And then right here, it's this simple. Where things live. In the context folder, always true background about you and how you work. Read this first. Projects, decision log. And that's basically it. So right here, you can see there's a context folder. We have an about me file, which you could grow. We have stack and conversations file. We have decisions. So this is a decision log where you can have your cloud.md always append new decisions and the dates whenever you make a big change to your project or to your life or to your business. And then we have projects. So this is where you could have a markdown file, or even folders within the projects for all of your ongoing projects, all of your ongoing clients, whatever it is, however you want to organize it, that's where you can have some projects. And you can even start to organize these things by dates if you want. So if you want to just have one that's for like May, and then you have all of those stuff, and you have one for June. The thing that I really want to stress here with level one, and the thing that I answer a lot in my community in the comments, is that there is not yet a standard way that has been proven the best way to set up your projects or your second brain. Besides some of the most cloud.md and whatnot. But the point I'm trying to make there is don't see what I do and think that that's the right way or see what someone else you watch does and think that that's the only right way. All that matters is do you have proper routing in place? And does it make sense to you? And does it make sense to your AI? Okay, so let's say I have my HER2 project right here, and I need to find something in here, but I can't ask AI for some reason. What I need to find is easy because I understand the drill downs. You know, I understand my base full. and let's say I'm looking for the HTML slide deck I built for my ranking Cloud Code features video. I would come into here and I say, okay, I know that's a project, so I'll go there. Within my projects, I've got another project for YouTube videos, I'll open that up. And now I know I made this video right here, May 30th, Cloud Code Top 50 features. In here, I have the actual tier list deck. And when I open that up, now I have the slide deck. And not only can I find it easily, but my agent can find it because it all makes sense and I have routing rules. Real quick, guys, if you're watching this video, you're probably interested in building your own AI operating system, lucky for you, I have a full free course on that in my free school community. The link for that is down in the description. Join the free school community, hop in here, take the seven day challenge, build your own AI operating system and apply these principles into building your second brain, which will make your AI operating system even more powerful. So links in the description. Let's get back to the video. Awesome. Okay. So that is how you start. Now, as you move up to level two, you might be able to start to work in some things like the LLM wiki, which is what I've got set up for a few different things. This is the whole cart. pathy LLM wiki, which I did make a full video about. If you want to check that out, I'll tag that right up here. But this is when you start to have more files and they start to take a bit of a different shape, and you want to organize them together in a bit of a different way. So it could be really good for researching all on a certain project. It could be really good for, you know, a few of the ones that I've got set up is my YouTube transcripts all live in their own wiki. I've got all of like my meeting transcripts that live in their own wiki. So for example, this is the obsidian view of my wiki for all of my YouTube video transcripts. You can see here, if I go to wiki, you can see there's main concepts like agentec workflows, AI coding market, context window, and all of these in here start to relate back to other tools and concepts and videos and stuff like that. So we've got the sources, we've got platforms, we've got context management techniques, and all of this was auto-created by our Cloud Code when I told it to ingest this YouTube transcript into our wiki. So I'm not going to dive super, super deep into all this right now, but definitely check out that YouTube video I linked. Now, what else is cool about this is this transcript Wiki actually lives within my main Herc 2 project. So here's Herc 2. If I go right here to Other Worlds, and then I go down to YouTube OS, and I click into the transcript Wiki right here, this is what we were just looking at in Obsidian. We could see the concepts, we could see the comparisons, we could see the sources, techniques. This is what we were looking at in Obsidian. So all Obsidian is, is it basically just visualizes your markdown files. You see here, Wiki, concepts, comparisons, techniques. This is what we were just looking at. All we get now is we just get a visual view view of all that. And so the reason I wanted to bring that up as well is because I think a lot of people obviously get pretty infatuated by that visual view. And obviously I started the video with that because I think that's what hooks a lot of people in, but all

 that really matters is can your system grab that and give it to you? If you are a visual person and you really want that view, then by all means install obsidian and set it up. It's super easy, but I'm saying that you don't always need that visual layer. If it's not beneficial to you, I hardly ever open obsidian just to be honest, because I know that it all lives here. And I know that my second brain and my OS can find all of that. So anyways, in level two here, let's look at this. It's very similar in shape to level one. It's just building on top of it because now we have our cloud.md, which starts to route to some other. things because it routes to the wiki and it still routes to context, projects, decisions, but it's also routing to references and memory.md. So we're just starting to add a bit more of these routing rules inside of the claw.md. We can grow the context, we can grow the decisions, we can grow projects and references, and we can also start to get this idea of memory. And what's really cool about this is you can turn on auto memory in claw code and the AI will basically start to write this file and update it on its own. So you don't have to think about it. If you come in here and you do slash memory, it'll say auto memory. on or off. And if it's off, if you want to turn that on, just turn it on. And now one thing to think about is I mentioned earlier that we want to make our second brains tool agnostic. And this is one thing that's pretty specific about Cloud Code is it uses claw.md and it uses this memory.md and it keeps that updated on its own. So if you wanted to move this over to codex, what you would do is you would first of all, transition your claw.md. You'd make a copy of it called agents.md. As you can see here in my Herc 2, I've got my, if I scroll down, claw.md right here, and then I've got agents.md right here. And they're essentially the exact same file, just so Codex can read this one and Cloud Code can read this one. But because Cloud Code keeps that auto memory, all you need to do is make sure you have that memory.md file and just tell Codex, "Hey, by the way, for memories, look in our memory.md file. It's all about the routing there." Anyways, just felt like that was important to throw out. But at a certain point, when you have these wikis, they do start to degrade a little bit. Because what's great about them is that they have indexes, right? So when your AI starts to look in the wiki, it knows, okay, If the user's asking about agentic workflows, I'm probably gonna start here. And then from here, I'm gonna drill down and read this to see what else is important to them. Maybe they're asking about the WAT framework and then I can drill into that. And maybe from there, I need to learn a little bit more about the Claude.MD system prompt, and then I will drill into that. So there are relationships here a little bit, but this isn't the same as like semantic relationships or knowledge graph relationships that have more meaning. This is more about just actually following a trail and reading the page in, its entirety. And I'll be fully honest with you guys. I pretty much sit my entire Herc 2 project in this level, in level two, because this has been working really well for me. Like I mentioned earlier, I haven't felt a pain yet big enough to switch over to level two. And here's what I meant by that. My wiki has links. Isn't that a knowledge graph? Not exactly, because this doesn't have connections of how they are related. Like this is endorsed by this, or this has cron to here. These just have connections because it's like a C also. It's like backlinks. So they're very similar. And yes, they can achieve a similar effect, but it's still a little bit different. Anyways, let's take a look at level three, which is where you start to do things like semantic search. Whether you do that in Obsidian, whether you do that with Pinecone or Supabase, however you start to grab the actual semantic search, that is what level three is. And so just as a quick visual for you guys, let's take a look at this quadrant cluster of images. So every one of these vector points is an image. And the what we see in here is the payload is stuff like the file name, the URL, the name of the author or the artist and the URL, but we don't actually see like what's in the image. We don't get a description. So what we have to do is we have to organize these images by meaning or by similarity. So when I open up this graph and we start to visualize this stuff here, what you see is that we have this main image, these owls, these kind of like, I don't even know. It's a very trippy style, like hallucinogenic style. Anyways, then this one is kind of similar, right? It's got those This one is also similar, but they're not the same. They just share similarities. And as we start to expand these more and more, we can start to get into different styles. So this one has like some creepy eyes and mushrooms or whatever. This one is kind of more down that fantasy lane. And as we start to build out more of these relationships and meanings, we can expand and grow away from them. And so Quadrant really just gives you a visualization here. I mean, it has clusters and vector store. But the reason I pulled this up as a demo is just because we start to see the actual relationships form here. based on meaning. And that's what's important about semantic search is that we're no longer doing keyword matching, we're searching based on meaning. So here in my YouTube transcript second brain, if I go to the smart lookup over here, this is very different from just the regular search. So for example, if I search here for feedback, let's say, we're actually doing a match on the word feedback and it's only showing me where that word actually appears inside of our second brain. But if I come over here, in the smart lookup and I search for feedback, we are getting matches that have things in here that mean feedback. So live test results, cloud code skills, which was talking about evaluations and stuff. So there's a big difference between keyword matching and semantic search, you know, similarity matching. This one over here is saying X equals X. And this one is saying X is similar to X, Y, and Z. And so this all just goes back to vector databases. I've talked so, so much about vector databases. So I'm not going to dive super deep in. I've got so many resources on my channel, but But basically what it is, is we take a document, so let's just say a YouTube transcript, we chunk it up, and then each chunk is ran through an embeddings model. And the embeddings model puts that chunk of text onto a three-dimensional space where space is related to meaning. And so it decides, okay, this chunk is about a company, so we're going to put it up here. This chunk is about finances, so it's going to go here. And we start to see these vectors form near other similar vectors. Now, do you guys remember how I said earlier, you want to think about how is the data going What type of questions are you gonna ask? This is a reason why that's so important. So think about this. Let's say I put my meeting transcript of March 5th meeting into my second brain, and I put those in as, you know, vectorized chunks. So let's say when I vectorize that meeting, we actually get, you know, like 20 chunks. It actually creates 20 chunks or however many that is. And then when I say, "Hey, Mr. AI agent, can you summarize the meeting on March 5th?" It will basically search for March 5th meeting summary. And it will pull chunks that are similar to March 5th meeting summary. And then even if it gets the right chunks, it's going to only summarize those five chunks. It's not able to look at the entire meeting summary, or sorry, like meeting transcript in entirety. So it doesn't really know a summary. It might be missing a lot of key information. Now, yes, there are things you can start to play with there, like metadata and other things like that to make these results better. But at the end of the day, people kind of assume that a vector database was some magic solution where it could always pull back what you need. But that is very false. And I mean, think about it like this. Let's say we have a table and we say, hey, which week do we have the highest sales? Okay, the agent looks for highest sales. It maybe grabs this chunk outlined in gray of data. And then it looks like, okay, week six here was the highest sales. So that must be the answer. But in reality, you can see week 14 was higher. Week 19 was higher. So when you need something that has actual full context, then you can't do the vector database chunking. That's where you'd rather just have a markdown file of March 5th And then all this agent would have to do is read that entire Markdown file and then give you a summary. And that's just going to be more accurate. So in this project, if we open up level three, you can see it's very similar because you can still have context files, decision files. You can still have all that. And then you might identify, okay, actually, this one specific unit of my business, maybe my YouTube transcripts, maybe I want just that to be a vector database. But I still want my context and my projects and my decisions to be Markdown files. Just because you have a second brain, and just because you have a massive folder here with a bunch of folders and files, doesn't mean that the whole folder needs to be one style. Doesn't mean that everything needs GraphRack. Doesn't mean that everything is just LLM wiki. It means that you're able to decide based on the type of data and the way you use it, how can you structure this specific folder in the way you want it? So here we have a vector index folder and we click on the how search works. It works by chunking, embedding, search, hybrid, re-ranking. There's some things you can get really, really nitty gritty on when it comes to semantic search. But what vector retrieval is really, really good at is looking at tons and tons of data, typically just like a lot of text. And when you need a very specific answer, something that's very similar. So if you had a thousand rules that you needed to store and you basically said, Hey, um, can you remind me what rule 17 was? That might be a really good use case for vector search because it's able to search for rule 17, pull in those chunks and just give you a little snippet because it would be a waste of time and tokens for your agent to read the entire markdown file of all a thousand rules, if you just needed rule 17. So that's kind of the difference there. Like I said, I've got so many videos on vector stuff on my channel, but really you could say, Hey, to your cloud code agent, I have this data. Here's how I want to use it. Do you think this would be better for now as markdown files? Or should I do semantic search? Like what would actually make more sense here? And it will help walk you through the way that you should actually set that up. So now I hope you guys are starting to understand why I said, you know, moving up on, or I'm sorry, like moving up on levels, moving down doesn't necessarily mean better it's all about figuring out what is the pain point with what you're currently doing and where would a different level help you out and fix that pain point. Okay, so now let's take a look at level four. This is where we start to get into like knowledge graphs and relationship graphs, which typically are gonna be the most complex and sometimes the most expensive as well. If you're doing it on a certain platform, you could always use open source software, but anyways, knowledge graphs. And I also wanna be upfront. I've played with these a lot, but I do not actually use these on the day-to-day because I found out just other ways to use routing files and wikis that fit my needs. Now, my work is very different than what a lot of your guys' work may be. Mine is very project-based and it is very, you know, content heavy. I don't have

 a massive CRM to manage with a bunch of different businesses and clients, you know? And if I did, maybe a knowledge graph would make a lot more sense and it probably would. But typically the cool part about that is if you identify that you needed a knowledge graph, let's say for all your projects, you needed, you wanted to put all of this in a knowledge graph, the data probably already exists here. And that's the thing about building out these relationships in your knowledge graph is that the system, whatever software you use is typically going to be pretty good at embedding that and creating that. But the problem that you're going to have, you know, you have to solve is you have to give it enough data. And so one thing that I really like to do is I like to have these brainstorm sessions, as you can see. And what I do with these brainstorm sessions is I use a skill called Grill Me. So if you see here, I have a skill called Grill Me, which I originally got from Matt Pocock. I customized it a little bit. I'll leave the skill for Grill Me in my free school community. The link for that is down in the description. All you have to do is hop in here, go to classroom, click on all YouTube resources, and you can find all the skills and everything like that. But the skill, what that does is it basically just grills me. It interviews me relentlessly. about a certain topic, and it creates a brainstorm file here. It only stops when it knows everything about it. So if you wanted to start building up a knowledge graph for all your clients and businesses, just say grill me about client A, grill me about client B, grill me about business A. And it would just ask you questions, and you can feed it files, you can give it stuff, you can feed it in transcripts, you can feed it in contracts, whatever it is. And that's how you can start to form a lot of data. Hey guys, me again, real quick. I'm editing this video, and I realized that I needed to throw out one thing here, which is that obviously, if you're putting all of this data and you're sending it all to Anthropic, to Claude Models, then that's not private. So if you feel comfortable with that, that's fine. I am putting a lot of my data in there and it is my business stuff and that's what I'm doing. But if you don't feel comfortable with that or you don't want to send client data, of course you don't, then maybe you want to do that through open source models. And maybe Claude Code isn't where you have the second brain that has every single piece of information about you and your business and your client's business. So the point I'm trying to make here is just This is what I'm doing. I'm obviously aware of the fact that my data goes to Anthropic when I process it through Claude. And if you guys are doing that, then you should also be aware of that. But there are other options if you can't do that. So I had to throw that out there. I am planning to make a ton of videos here soon about local AI and open source models and all this stuff because it's a really, really exciting space that I think is going to start becoming bigger and bigger. So yeah, keep that in mind. Back to the video. I think sometimes that's a misconception about how I got here and how people build their own AIOS or SecondBrain is that they think the problem is the system not retrieving it great, which sometimes it is, but sometimes it seems like the bigger problem is getting everything out of your brain into the system. So before you blame AI, take a look at your folders and files and say, is this actually holistic? Does this have all the nuance that I have in my brain? Anyways, from there, when you open up level four, you can see that it's very similar still. We're just adding on a few things. You can see here, we've added an agents.md. which is the exact same as the Cloud.MD. And what else is cool is you can literally just reference inside of your Cloud.MD at agents.MD, and then you can delete all this because this basically just like injects that file into here. But I just wanted to show that. But anyways, you can see we're still following the same principles. We have a wiki. We've also added a knowledge graph layer. We've still got the same where things live with the routing with all these just regular folders and boring markdown, but boring is beautiful. You can see that our memory is still here. It's starting to grow. And we just keep building on top of this. So one thing we added here, as you can see, was our knowledge graph folder. And so what happens here is we get different entities, right? So like we can see, okay, Jordan is a person, Acme is a company, and then we can start to form relationships between all these things. So Jordan works at Acme. Acme is endorsed by Postpilot. Postpilot is a competitor of Cadently. And it starts to build out not only these entities, but it shows you how they're all related. And so that's why when I said that I really like using, you know, this, um, what's it called? LLM wiki is because I have enough of that feel of all these relationships. because I've put so much time and effort into ingesting these in the right way and giving it context. The thing about this one is that it has to read every single file it wants. Maybe it was looking at AI video production and all it needed to know was 11 labs. It still would have read this entire file first. And so that's where sometimes the knowledge graph is actually more lightweight in that sense. And this is the example I showed at the beginning of the video where we have light rag and forgive me, I'm gonna have to blur some of this stuff out because this is like legitimately my entire second brain in our business. But as I really zoom in here, and this kind of slows down my computer because there's so much, but what you'll notice is that we actually start to get relationships. I probably shouldn't have done this with so much data, but you can see like, we have this collaborates with that. We have this builds that. And so if I really started to open up all of these little, you know, circles, we could see what was going on and how they're all related. We could see that our seven-day AIS challenge, it was provided from YouTube. It connects to the onboarding process of AIS+. It was developed by Aiden. And so we can basically follow around these relationships as you see. And even though it's pretty much the same data that you see here in Obsidian, we're not getting that same level of relationships between these different entities. So anyways, if you guys wanna see a full breakdown video on something like LightRag or Graphify, or all the other solutions that there are out there for more of a knowledge graph, relationship graph, then let me know. But that is kind of the difference there. So if you don't need those sort of relationship chains and you're not worried about that semantic type of relationships, then you probably don't need to use something like a knowledge graph. And then level five, we have more of the always on brain OS, and something like G-Brain. Gary Tan, CEO of Y Combinator, he created this thing called G-Brain, which pairs really well with G-Stack. But G-Brain is kind of the idea of everything we've talked about here. Wikis, routing, relationships, tools. But G-Brain has kind of that always on element, because it is like constantly syncing and refreshing memories and adding more stuff. So adding in G-Brain to something like a Hermes agent would be really, really good. You can still do it in cloud code, but you'd have to handle those crons and get all that stuff set up, which is why I don't currently run G-Brain at the moment, but I have been playing around with it with my Hermes agent. So anyways, the point here is that it's very similar to everything else we've just talked about. It's just having that auto-updating feel, more of the autonomous, always-on feel. But I will say, another thing that kind of scares me about that is you have this whole dilemma of, you know, when do you have too much context? And when does it get to the point where it's actually doing more damage than it's doing good? And the reason I bring that up is because I am in complete control of what my second brain ingests. I will run a skill to go grab all of my meeting transfers in the week. I will say, "Hey, here's something. Help me figure out, like, help me brainstorm about this and then let's ingest it together." And for me, I really like being in that control because in my mind, there's a big difference between a few types of data. If you guys remember in my like AIOS videos, I've talked about the four C's. So context, connections, capabilities, and cadence. And for the second brain, I mainly think about it as just these first two. So context and connections. And so when I think of context, that's stuff like, you know, what my business has done. So if I come into here, into my second brain, and you can see here, if I go to up at OTAs, so OTAs are basically just our projects for the quarter. And so here I can see all the Q1 ones, right? I can look at all those and I can click at them and see decisions that we've made in the statuses. And I can also see Q2 OTAs. So I can see what's going on here. And my second brain is able to see that because that has been basically, those are locked in decisions. This is what we're doing this quarter. And then I'm updating the statuses of that stuff. So that's like, context that's what's going on in the business but when it comes to connections if I go back to this this is more of like the real data that isn't as evergreen this is stuff that changes this is like slack threads this is emails this is a customer data and that type of data you don't want to ingest into a second brain because that's just noise then then you have to go back every month and like delete old stuff so the way that I like to think about my actual second brain is stuff that I'm not going to delete this is stuff that is like okay in a year will it be good for me to have this memory in here yes Otherwise, it's just adding noise. So when you're adding data into your project, think about it like the context and connections. Think about if this is kind of like more evergreen, holistic data, or if this is more things that are going to change next week. So you probably shouldn't pull it in, but you should make sure that your second brain has access to go grab it. So that way, if I said to my second brain, hey, can you just take a look real quick at what John and I were talking about last week about, you know, OTA number seven, it would first go to our OTA file and it would it would try to find it there. If it couldn't find it there, it would look through the wiki and it would look through meeting transcripts and see what we talked about there. And if it couldn't find it there, it would finally go to ClickUp itself, pull real data in from me and John's conversations and see if the answer lived there. And so that in my mind is still a second brain because I'm able to ask a vague question and the second brain knows exactly where to look in what order to find that real-time data and then give me back the answer that I need. That's the question I ask myself is, does this thing understand where my data lives and where to look and can it give me accurate answers? So as far as, finding your level, remember, your whole project doesn't fit into one level. Maybe this folder's level two, maybe this folder's level four, maybe this folder's level three. Here's some things to think about. If you are re-explaining your setup and you need to find things by exact words or files, look at level one. If you have 30 plus notes and you keep forgetting what's in them, look at level two. That's where you sort of like ingest them and get that wiki with relationships. If your project is just completely whiffing on notes that you know exist and your routing isn't working, then maybe you want to look for something more like a semantic search that doesn't rely on an exact word level match. If you're looking for relationships and to be able to follow chains of questions and thoughts, then you probably want to look for something like a knowledge graph. And if you're running agents offline and you've got so much data and you want to sync up a bunch of Hermes agents together, then you probably are looking for something like level five, something like G brain. And another topic that I get some questions about, which I'm not going to fully address in this video, but I will briefly bring up is the fact that you are building your own second brain OS. So are other people on your team. The next question is, how do you actually make sure that everyone's data is syncing together and how do you have more of like your team second brain there's a lot of different ways to solve that i think once again it's not an issue of oh do we use google drive or notion or github or cloud plugins i think the

 issue to figure out with your team is how do we actually make sure that we all habit shift so that this stuff is actually useful and not just noise? How do we make sure that process owners are updating their docs and syncing their stuff there? How do we make sure that other people are pulling from that rather than always just pinging the same people for questions and answers all the time? I think the adoption and the change management question is the bigger one. The tech and the way it actually functionally rolls out is a little bit less. But what I do know is that you getting set up how it works, how you should route, how you should make the decisions of where the data should live. That's the first hurdle. You can only solve the team-wide problem once you feel comfortable about the way you run it every single day and then it works for you. That is gonna do it for today. Like I said, you guys can grab all the skills and everything that you need from this free community. The link for that's down in the description. I will also include the slide deck if you guys are interested in flipping through. So if you guys enjoy the video or you learned something new, please give it a like, it helps me out a ton. And as always, I appreciate you guys making it to the end of the video and I will see you all in the next one. Thanks guys.
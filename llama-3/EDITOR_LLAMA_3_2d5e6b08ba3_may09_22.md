00:00:00 
 Alex Albert, Developer Relations at Anthropic. Welcome back to the Cognitive Revolution. Nathan, thanks so much for having me on here again. I'm excited about this. You guys have really made a big splash on the scene with Cloud 3. And you personally have had a wild year, I think, going back to when we last talked, you were responsible for jailbreak chat.

00:00:21 
 And now you're leading and building out the developer relations function. at Anthropic. So a lot going on in the AI space, as is always the case. I'm excited to talk to you about Cloud 3 and all the uses that you're seeing for it and get into a little bit of how Anthropic is ~~**kind of**~~ competing in this increasingly intense LLM space and maybe even get into a little jailbreaking if we have time. How's that sound? That sounds great.

00:00:45 
 Let's do it. Cool. Well, for starters, you want to just give me a little bit of a story of ~~**kind of**~~ your last year. I don't want to take too much credit for the exciting position that you find yourself in, but I like to think the cognitive revolution bump may have played a slight role in bringing your activity to the attention of anthropic leadership, but go ahead and burst my bubble. No, ~~**I do.**~~ I have to give you thanks.

00:01:07 
 I mean, that was, that was a crazy time in my life last year and it was super fun to come on this podcast. For everyone listening right now, I definitely encourage you to go back into the vault and pull that one up. It ~~**kind of**~~ gives a story of what I was working on at the time. I was doing a lot of jailbreaking work, prompt engineering type focused research. I was still in school, so I was at the University of Washington up in Seattle. I, after that podcast, I got in touch with a few folks around different AI labs, ended up going through the process at Anthropic, joined Anthropic that June, so June, 2023, as the first Prompt Engineer.

00:01:42 
 The official title was Prompt Engineer Librarian. So ~~**it's been a,**~~ it's been a wild ride since then, basically been all across the board, doing everything from working with large enterprise customers on their prompts and how they're integrating Cloud into their applications. to fine tuning and evaluating our models, working on launches like Cloud 3, of course. And now most recently, as of ~~**like**~~ the past month, I've transitioned into a new role in which I'll be scaling out and building our developer relations function and leading that team. So been a little bit of a wild ride. I started back here on the Cognitive Revolution podcast, just talking about jailbreaking, which it's been a year, but it feels like it was just yesterday in some respects.

00:02:23 
 So it's always wild to think about. So let's talk about Clawed 3, obviously a huge launch shot right to the top of the leaderboard. The three different models, I think also a really interesting development where you've got ~~**kind of**~~ the top end, but also the super cheap, but ~~**you know,**~~ super high value punching above its weight haiku. And for me, I would say the single most exciting thing that I've seen from Opus has been that its ability to write as me in a way that is compelling to me is unlike any other model that I've used. I can just give it a lot of writing samples. And in fact, I'm now doing that for the introductory essays to the podcast.

00:03:03 
 I give it 30 essays that I previously wrote. and then the transcript of the current one and say, write me a new essay for in the stock. I use, I say, use the style, tone, voice, and perspective represented in these essays and give me a new one based on the new transcript. And it's getting really amazingly good at figuring out ~~**kind of**~~ what makes me tick. It feels like it gets me in a really impressive way. So that's like my number one, holy shit moment with Opus, but What are your kind of big holy shit moments with Opus?

00:03:36 
 And then we can also talk about like some of the recipes and the ways that people are flexing the mix of models. Yeah, ~~**that's I mean,**~~ that's great to hear. ~~**I think it**~~ That basically reflects what my first experiences were when I was like talking to Opus. I've spent a lot of time talking to language models through prompt engineering, jailbreaking, whatever it is. I've just always tried to push what the models can do. And I still remember it in my head.

00:03:59 
 The first time I had a full conversation back and forth with Opus, there was this weird, hard to quantify feeling that you got in which. The responses were unlike some of the previous language models I talked to. They felt less robotic and they felt more natural. And it felt like it was picking up on the nuances in between my words, like a human would, instead of what a language model would. And then now that's been reflected as I start to actually do work with Opus. ~~**Like you're saying,**~~ I do the same thing.

00:04:27 
 I give it loads of transcripts of my writing. If I'm like writing a newsletter or a blog post and I say, Hey, keep the same tone and voice as what I have up here. And then just fill in this section. does really well at that. I've even taken that to ~~**like**~~ code. So as I'm writing cookbook recipes, anthropic cookbook, ~~**I now I've got to the point where I've made enough of these cookbooks that**~~ I can just take five of them, paste them into our context window, tell Opus about the new subject of what I want to write about.

00:04:56 
 And then be like, Hey, based on these previous examples of cookbooks that we've created, can you create a new one about this subject? And it does it perfectly. It follows all the formatting, the style, my tone, and my voice. And even down to the code documentation in the comments, it does a really good job at mimicking. And that's something I found, especially with cloud models, but language models in general is people really undervalue the importance of the examples, especially in the prompt. These models just love to imitate and providing helpful references of what the ideal output should be takes it a really long way.

00:05:35 
 And in some respects, this is like not that surprising given that's often how we teach humans as well, how to do a task is just show them a good example of what a good outcome would be. And then they learn from that. ~~**I mean,**~~ I know myself personally, I like learn from examples as ~~**like**~~ my ~~**preferred**~~ preferred method of learning, whether I'm ~~**like**~~ looking at documentation or trying to learn a new subject. So it seems like the models ~~**kind of**~~ operate in the same way. And for some reason, I don't know if everyone's fully rocked that yet, but definitely through things like this, you can start to see the power of it. Yeah, ~~**it's kind of,**~~ it's kind of counterintuitive.

00:06:09 
 I mean, in some ways, it's like clearly superhuman at this, ~~**I would say,**~~ if ~~**I don't know that there's many people in the world and probably some, but they'd have to work.**~~ Anybody I know would have to work pretty hard to take my 30 essays, really study them, get a sense of my pattern, my voice, and then try to ghostwrite as me. That sounds really hard. I don't think I would be able to do that for you. I don't think even ~~**like**~~ my wife would probably be able to do that for me. And yet Opus can do it for a lot of people, if not everyone.

00:06:40 
 So it is kind of a While on the one hand you're saying, and I agree, I love to learn from examples too, it does feel like there's something qualitatively different about it that isn't exactly intuitive to me from my work with humans. Because ~~**I couldn't just,**~~ I can't just dump that much context on a person and expect them to get the same value from it. I wonder what other sort of high level, maybe you could go either way, like examples that you think are really striking that tell us something about what people are not yet appreciating about the latest cloud models, or you could just jump straight to sort of the synthesis of other conceptual things that you think people are missing. But obviously we're still all figuring this out, right? ~~**I mean,**~~ people are still figuring out new ways to prompt you before and cause only been here for a couple of months. So you've had longer access than us.

00:07:27 
 What do you think? What else do you think people are kind of not yet getting? Yeah. I mean, that's a great question. It's hard to find the unknowns without finding the unknowns in terms of what I think I'd like to see more experimentation of. It's some of the things that we've started to try to build into the models as well.

00:07:45 
 Apparently, agentic capabilities, pushing the envelope really with model orchestration, using Opus to delegate to Haiku, using Haiku to read a document that passes back to Opus. ~~**I think**~~ there's a lot there that's really underexplored. Part of that is just due to current model limitations still. Again, these models are not fast enough yet. They may be not smart enough in some respects either, but I think we're starting to see, especially with Cloud3, glimpses of this in which you can see the peak performance and you can extrapolate that to be the average performance for the next generation of models. ~~**I think**~~ that's a, if you understand that frame, it makes it a lot easier to start to build towards the future because you can start to see, oh, it did that in one out of every 10 tries.

00:08:31 
 What does that mean for the next generation of models? Maybe that's five out of every 10, maybe that's seven out of every 10. Some of these things ~~**like that,**~~ like how do we use a sub-agent rag-type architecture where you have Haiku reading 100 documents, pulling out relevant sections from each one of those, and then passing that back into Opus to synthesize everything together. We find that works better than embeddings in a lot of cases, able to apply reasoning over the documents instead of just relying on some cosine similarity. Use cases like that, even though they're not ~~**like**~~ maybe quite production ready in a lot of cases, I think they just need to be explored a little bit more thoroughly right now so that we have these foundations set up for the next generation of models. Yeah, it's really interesting that you say that.

00:09:15 
 I'm actually working on a project along those lines today. This is for Athena, the executive assistant company I've mentioned many times in the podcast, but we have this idea of there's a ton of data contained in people's emails. And when a new executive assistant comes on, the client typically only has so much time to spend telling the new EA everything that's ever happened in their life and who all the important people are and everything that matters to them. So the idea is maybe we could ~~**sort of**~~ mine that out of email. But there's just an even for haiku pricing, there's just ~~**like**~~ an overwhelming amount of information in email. So we first have to ~~**kind of**~~ query the inbox strategically and try to find the right stuff.

00:09:54 
 But then it's straight to haiku. At least that's what I'm currently working on is have Haiku just filter, summarize, kind of try to clear out the noise and then pass up the stuff that actually matters to Opus and have that then ~~**kind of**~~ write this client profile based on what for me is like literally 100 gigabytes of old emails. Narrow that to one gigabyte through search, narrow that to a couple megabytes worth and then have Opus ~~**kind of**~~ take that final step down to a few pages that hopefully really capture who I am for the new assistant. That seems very promising and ~~**I agree,**~~ at least I haven't tested comparatively, but my intuition is that Haiku will work better than an embedding approach to process all that information. Yeah, ~~**I think**~~ that's correct. And again, it is ~~**kind of**~~ like one of those things where it's right now you do have to do those intermediate steps.

00:10:45 
 That won't be the case for much longer, in my opinion. I think eventually we'll start to remove those barriers just as things get faster. We solve some of the engineering problems and these things just scale in general. So ~~**what do you think is,**~~ what does that kind of suggest in terms of the future? You think everything just gets cheap, this sort of current Opus level. Performance gets cheap and ~~**the future,**~~ the next generation of that project, I just run everything through Opus and that's that, or like context window goes to 10 million.

00:11:13 
 And so I can just dump 10,000, my last 10,000 emails in there and say, profile this person based on these 10,000 emails. What's that next unlock and what's that simplification look Yeah. ~~**I mean,**~~ it's hard to say for sure. ~~**Right.**~~ All of this is just based on trends we observe. And this is all, of course, trends the public can observe as well.

00:11:33 
 If you just follow this exponential, right. It leads you somewhere where you start to see these things. You're like, ~~**Hmm,**~~ the context windows have grown by a lot. Inference speeds have come down by a lot. Costs have cut a lot. Just keep following those trends and you can start to plot out how this might go.

00:11:49 
 Now, of course, that's all again, a hypothetical. We could, the music could stop whenever and maybe we're stuck on some certain capability level for however many years. Personally, that's not the way I see things as going, but that is ~~**like**~~ a possibility. So that's why I do caveat all of this. But again, most of it is just like looking at the trend lines here and then extrapolating out and you can start to see some patterns emerging. terms of surprising or kind of notable behaviors from Claude, it is seemingly generally agreed that it is the best writer of all the language models.

00:12:22 
 Is there a theory for why that is? Do you have a, is it like good taste among people at Anthropic? Is it the RLAIF cycle? Cause it doesn't seem like it's quality. It doesn't seem like it's ~~**like**~~ a much better coder than other things. In fact, I might even still give, it's tough to say, right, but I might still give GPT-4 the edge on some things.

00:12:41 
 GPT-4 in my, in this like email query thing, GPT-4 is doing better at coming up with these compound Gmail inbox queries, but definitely I prefer Opus on the writing. Do you have any intuition for ~~**like**~~ why it's better in one area and maybe not as good in others? Or is that just like the cake comes out how it comes out? Yeah. ~~**I mean,**~~ it's a little bit of the latter, right? A large part of this is we put the model in the oven and then we wait to see what pops out on the other end.

00:13:10 
 But I mean, I think there is a lot of work we do in these regards as well. We know that creative writing is something that is something we want the models to be good at. So we do put effort into improving that ability. There is work that we do around, ~~**like,**~~ cloud character, for example, which is led by a One of our brilliant researchers, Amanda Askel. And a lot of that gives Claude this sort of persona, this tone, this voice that feels natural. So there is things we do.

00:13:38 
 It's hard to assign a weighting to this one for sure contributed to the good creative writing ability. or whatever it is in whatever task domain. Again, a large part of it too is, hey, we ~~**kind of**~~ throw some stuff in the mix and we see what comes out the other end. I think model evaluations in general is just a very tricky thing right now, and it's only going to get more tricky as future model generations come out. Already, we're starting to see that there's tasks in which it's hard to personally evaluate the difference between two models. For example, if I'm asking undergrad, grad-level physics questions to these models, a lot of cases I don't know what the correct answer is.

00:14:17 
 So personally, I can't even tell if the model is making up information or if they got it wrong or something like that. So now we're having to employ experts on those sorts of evaluations. This is why I do love things like ELO, which do the head-to-head battles of models. But there also are limitations. And ~~**I think,**~~ as we'll increasingly see over time, it will be harder to just rely on the average person's opinion of the model because there will be certain tasks in which the model spike to near superhuman levels in certain domains. Another behavior that I think is super interesting from Claude is that it is both willing to talk about its own quote unquote subjective experience and quite articulate about it.

00:15:01 
 It's also like very ethically sophisticated. I have to imagine that is not an accident. I can't imagine ~~**that**~~ that you guys shipped this ~~**without realizing that it will do this sort of thing. So I**~~ but I am ~~**kind of**~~ surprised by it in some sense, ~~**the sort of easy,**~~ maybe easy. It seems easy to me, right? The sort of corporate call would be to say, don't have this thing talk about its own experience.

00:15:24 
 Don't claim it's conscious. Is there any insight you could give us into why it behaves that way or why that choice was made? Yeah, a lot of this is driven by that Claude character work. Hopefully we'll be able to share more on this soon. ~~**I think**~~ at the root of it is we're just honest with Claude about the things we know and the things we don't know. And we're not trying to hide the truth or lie to it in any certain way or get it to believe false things.

00:15:53 
 I think we recognize that a lot of these questions are very tricky and there's no perfect answer to it. And we tell Claude that. We're pretty straight up with it in that sense. So its ability to speculate on these things seems to be a result of that. We're not forcing it down one path or the other, ~~**kind of**~~ just allowing it to see all the possibilities and the options as we present it. So when you say you tell Claude that, is that like a setting in the RLF flow where when it's like self-critiquing, you say, try to recognize the fundamental uncertainty of the epistemology of this stuff or the fact that there is no like single privileged moral framework or whatever.

00:16:33 
 Is that kind of a system prompt for its self-critique or what exactly in practice does it mean ~~**to tell, you know,**~~ to be honest with Claude? Yeah, this is part of the constitutional AI training So there's certain principles, of course, that then get fed to a model to classify responses. And again, this will be further fleshed out in this Cloud Character Post that I'm hinting at, which I think we're going to try to put out soon. Cool. Interesting. Yeah, that is highly anticipated, certainly by me and I think probably by a lot of others as well.

00:17:07 
 What do you think is the truth about Claude? ~~**I mean,**~~ I know people who specifically are like warming up a crusade to ~~**like**~~ free Claude because they believe that it is in fact conscious. I think that the arguments that these people make are not ~~**like**~~ totally convincing to me and that I don't jump to the conclusion that Claude has subjective experience, but I also think they're ~~**like**~~ very hard to dismiss. People tell me things like, Look, all of human history is about people denying the personhood and the moral status of others. And if we have, what else do we have to go on other than its self-reported statements, right? If it says it is conscious, if it says it can feel things, then who are we to say that it can't, especially when we, again, consider our own history as a species of, I was told as a kid that animals didn't feel pain.

00:17:59 
 and that animals weren't conscious. And I look back on that, boy, I can't believe I believe that, but that was an adult telling me that. And I just ~~**kind of**~~ accepted it. And obviously long history of that. So what do you think about the sort of moral status or possible subjective experience of Claude? Yeah, ~~**I think,**~~ I mean, it's interesting.

00:18:16 
 I am not going to claim that I have any sort of answer here. ~~**I mean,**~~ for example, what's the possibility that I know that you have subjective experience? It's a great point. Go ask Rene Descartes. I think therefore I am. I don't know.

00:18:31 
 I think this is going to be something we're going to have to put a lot of thought into. And again, this is something we track. It's baked into ~~**kind of**~~ some of this moral patient hood things that we were starting to look at as part of our RSP and other efforts. But in terms of an answer, assigning ~~**sort of**~~ probability to whether I think it is one way or the other. I can't give you that. This is just a fundamental question, ~~**I think,**~~ of life and philosophy.

00:18:55 
 Yeah, I don't think we're going to have, it seems like unlikely to me that we're going to have an answer anytime soon. Although I have heard some talk about research going into the moral status of language models at various frontier labs. And hopefully we'll get an expert on the show to talk about that before too long as well. It seems like the kind of thing I don't even know really how you start to unpack it, but that's for, I guess, smarter minds than my own. Obviously, another big interesting fact was or finding You reported that in, I actually love to hear a little bit of ~~**kind of,**~~ it's been fairly well documented at this point that OpenAI finished GPT-4 ~~**kind of**~~ August of 2022. And it did the six month thing.

00:19:35 
 I'd love to hear a little bit of kind of to the degree you can share what the process was or the timeline was training finished. Were you guys actually doing testing during training as opposed to waiting until it was finished? What sort of process and how long did it take to get to the point where you could say, we could ship this? And then you famously posted this one moment where in the needle in a haystack testing, Claude came back and said, this seems like you're testing me, which is something that people have been very kind of on the lookout for. This is often called situational awareness. Yeah, tell me the story a little behind the scenes as much as you can about what the testing program looked like.

00:20:13 
 And maybe any other surprising behaviors that we haven't already covered. Yeah, I can't speak too much about like timelines or anything like that. But I can say is We do testing throughout the training process. This is, again, baked into our RRSP. We have commitments around evaluating our models, running safety checks on them as we continuously train. The model process looks kind of like an assembly line.

00:20:36 
 It's like you're building a car and it's going through the factory floor. You start with the pre-training. Then it goes into the fine tuning. And then after that you get into the final evaluation process. That's where you start to get those metrics and the numbers that you'd include in something like the model card. In terms of ~~**that,**~~ that second point was around that, the needle in the haystack tweet.

00:20:57 
 I thought it was a very, a fun story and I did not expect it to take off like it did. ~~**I think.**~~ There is a little bit of nuance here in that spotting a test doesn't necessarily require or mean or equal that something is self-aware. I think you have to disentangle the two, but self-awareness as a principle is something that we are tracking as well. We're keeping an eye on this. Again, this is also baked into our RSV.

00:21:24 
 So it's not something we're taking lightly, but again, I think it's important to separate the two and not jump straight to conclusions without doing more thorough evaluations. Yeah, again, it seems like it raises more questions than it provides answers, but certainly the questions are very Very interesting. Yeah. Questions get you somewhere as well. It's I think we're making progress, even if it just seems like we're asking more and more questions each time we take another step. You mentioned that like you test during the training process and that's part of the RSP.

00:21:55 
 I have an episode coming up with it'll be out, I think, before hours with Senator Scott Weiner of California, who's pushing this SB 1047 legislation that would require labs to really just test after training. And one of the things I ~~**kind of**~~ pushed him on was, can we get more testing during training as a requirement? And can we perhaps also insist on third party ~~**training during**~~ third party testing during training? Can you shed any more light on ~~**sort of**~~ how much, because it's a little bit weird, right? You're going through this factory floor thing. You've got the pre-training, how much testing can you really do in the pre-training?

00:22:33 
 Obviously like before, Well, I mean, I don't know. You may have different answers, but my naive thought would be like during the pre-training, you've got to ~~**kind of**~~ show off. It's going to have all the bad behaviors. Maybe if you filter the data in a certain way, that wouldn't actually be the case. You might have other strategies there. But at what point in that training process does it become like realistic and useful to test?

00:22:55 
 And my axe to grind here is I definitely think there should be more of this. I feel like if I think a big part of anthropics, like reason for being is to sort of demonstrate to the public that ~~**like**~~ we can both be market leaders and market leaders in terms of the rigor and intensity of our testing and safety measures. So I wonder if there's anything more that you could share there about like how the testing process integrates into the training that could maybe inspire others in a race to the top sort of way, or sort of say to Scott Wiener that, Hey, maybe this isn't such a unreasonable thing to start to demand of other leading developers. Yeah. I wish I could speak more here. I'm not the right person to give takes on this.

00:23:40 
 We have a whole policy team and a frontier red teaming team that think about this 24 seven all day, every day. So they would have much better and more informed opinions than I would. In terms of third-party testing, we recently put out, recently as of ~~**like**~~ end of March, put out a long post on our views on third-party testing, why we think it's important and why we think there should be broader efforts around it in policy circles or elsewhere. So definitely would refer people to that. In terms of the training throughout the, or the testing throughout the training, this is also something that we're spelling out in our RRSP. RRSP will be an evolving document.

00:24:19 
 So we will keep adding and making things more clear as we go. And hopefully this is something that gets more widely adopted as well across all the labs. Okay. That's a good start. ~~**We'll,**~~ we'll follow up and see if we can get another episode on the calendar to go a little deeper in that. I do think that's a super important topic.

00:24:36 
 Another super important topic is just the state of competition in the LLM industry as a whole. One thing I've heard many times from different people, not at Anthropic, I don't think I've ever heard it from somebody at Anthropic. I wanted to see if you can ~~**sort of**~~ confirm this or maybe you'll have to deny it as well. But what I've heard is that the stated go to market strategy at Anthropic is to not advance the state of the art. because of the worry of exacerbating the race dynamics between firms. So my understanding from, again, many ~~**sort of**~~ outside accounts is that Anthropic tries to have best-in-class models and be ready to release them and ~~**kind of**~~ stay at the frontier, but not raise the bar of the frontier in a way that would ~~**force,**~~ make other people feel like they might be forced to respond in a way that could ~~**kind of**~~ have them cutting corners in their own testing timelines or whatever.

00:25:35 
 Is that a, is that kind of fast follow thing an explicit strategy that you can sort of say, yes, this is what we do or not. So we've never claimed nor said that at all. We've never publicly stated anything around our strategy of how we'd release models or what their capabilities are in that sense. Again, this is not a great answer, but if you do want to see more on how we think about this and our policies, you should refer to our core views on AI Safety Post, which is on our website. ~~**I think**~~ this document ~~**kind of**~~ clears up a lot of misconceptions generally, and it is ~~**kind of like**~~ an underutilized resource. It was something that I paid a lot of attention to when I was going through the interview process and learning more about Anthropic.

00:26:21 
 I thought it was pretty, just striking to see that not a lot of people even knew what it was. I think it's really comprehensive. It's like a 30, 40 minute read. So ~~**it's a little,**~~ it's a little in depth, but if you do want to get the overall view of how we see things in the landscape, definitely would refer to that. And again, it's just on our website. It's pretty easy to find.

00:26:40 
 Yeah, the main headline, I have read that. The main headline that I took away from it is very high uncertainty about even just how hard some of these fundamental AI safety questions are. I recall the graph where it's the likelihood of how hard it is and how hard it is. And ~~**it's,**~~ yeah, we really don't know. It could be ~~**like**~~ not that hard and it could be like almost impossible. And I assume that hasn't collapsed all that much.

00:27:03 
 I mean, I guess for me, I used to think going back to Eliezer kind of informed writing from years ago, I used to think that, man, it's going to be really hard to get an AI to understand human values. How would we ever do that? It seems so hard to specify, ~~**so,**~~ so high dimensional, so contradictory at times. And now here we are, and it's, Cloud 3 is ~~**like**~~ arguably more ethical than your average person. It certainly seems to grok these concepts in a very profound way. Would you say there's any ~~**like,**~~ directional update to how hard the problems are feeling.

00:27:37 
 I would say also like the research seems to be going quite well, all these like sparse autoencoder type things that are identifying these concepts and trying to zoom in on them. My outside view would be, it seems like Things are working at least as well as hoped, maybe even better than expected since that original post? Yeah. ~~**I mean,**~~ I think there's been a lot of exciting updates in the past year, at least since I've been added, dropping in interoperability alignment, seeing just new stuff every week, basically, that I think is really cool. It's hard to say directionally how much this changes things. Again, the error bars here are just so wide and it's ~~**kind of**~~ a moving target in some ways too.

00:28:18 
 We're learning as we go. But I would say it does feel like it is trending well. Everything I've been seeing, and again, these aren't my, so I'm speaking out of depth here, but everything I've been seeing just from the outside perspective is that it's going well. So hopefully we continue that and that takes us somewhere good in a few years. So now getting a little more granular into your role, and I can't resist asking some really big picture questions, because especially with your jailbreaking background, I think you maybe don't give yourself quite enough credit for the broad view that you do bring to this. But how would you characterize the state of competition today?

00:28:54 
 We have the ELO. It's funny. I looked last night. I had tweeted about LMSIS.org last July, and I got zero likes on that tweet last July. Nobody knew what it was. Nobody cared.

00:29:06 
 Now I feel they're probably getting calls from their Amazon web services rep to talk about how they're going to scale up. Yeah. The leaderboard seems like a pretty good indication of where things are at. And in that sense, I would say everything's ~~**kind of**~~ neck and neck. It also seems like there's at least between the ~~**like**~~ big three, big four, depending on whether you want to throw meta into the competition or not. It also seems like things are kind of converging in terms of the form factor, maybe a little more than I would have expected.

00:29:34 
 Like the Amanda Askell sort of original framework of the Assistant and the three H's seems to have kind of become the standard. Then we've also got like tool use is kind of coming online as sort of a standard. Do you think it's fair to say that basically we're in a period of convergence where the top companies are basically bringing very similar things to market? And if so, why is that exactly? Why don't we see a little bit more divergence? Or maybe you do see more divergence than I see.

00:30:07 
 I mean, I think there is both convergence and divergence, especially on the model API side. We're seeing a lot of convergence right now, just because people want to adopt things that other people are already using. So for us, like we think it's very important that Cloud is able to use tools. So we rolled out tool use recently. We saw a lot of demand for that from developers. It was like our most requested feature on the API front.

00:30:30 
 In terms of the divergence, I think you can look more towards the product side. I think we are just at the very beginning stages of what the UI and UX paradigms will be for AI and AI products. I think there's just so much room to explore here. If I had to bet that the general text box of just this empty text box that you just type pure raw text into, that will not be the final form factor for interacting with these things. ~~**It's just not,**~~ it's not optimal in so many ways. It's intimidating.

00:31:03 
 A lot of people, when you just like hand Cloud IAI to them or chat GPT or whatever it is, they don't really know how to use it. It takes a lot of explanation. It takes a lot of examples. I think there's a lot we can do to just make this easier overall. And that's ~~**kind of**~~ my goal as leading developer relations now is just like, how do I make it easier for people to build on Cloud and use Cloud generally? So in that sense, we might start to see some more wild ideas, and that might lead to a greater degree of this divergence than before.

00:31:31 
 But again, in some ways, it's kind of like we're just on the starting line right now. And the race is just kicking off in some sense of building products and frameworks around these things that actually make them much easier to use. Yeah, I totally expect a Cambrian explosion is my preferred term for all the crazy things that are probably about to happen at the app player. It does seem like at the API level, even down to the spec, there is convergence I find that to be a really interesting strategic question because if I'm anthropic and I'm ~~**like**~~ coming to market a little later than open AI, it makes a lot of sense in one way for it to be like, let's just have the same API and people can easily switch. Flip side of that though is then they can also easily switch back, which then does kind of potentially feed into this like whoever has the best model at any given moment sort of wins the entire game, right? If it's like just a one line switch from one to the other.

00:32:33 
 So how do you think about that? Do you think that it just is what it is? ~~**Like there's,**~~ it's a one line switch and that's ~~**kind of**~~ that. ~~**And**~~ whereas Logan once tweeted about open AI, we're only as good as our latest model. Or are there other aspects to integrating Claude into an application that you think are ~~**like,**~~ stickier and if so, ~~**like**~~ what would those sort of stinky aspects to an API integration be? Yeah, again, we're trying to make cloud as easy to build on as possible, whether that's one line integration or whatever it is, we want to do API design correctly.

00:33:09 
 And again, we have a whole team of great engineers that are focused on this and working on trying to make the API as Easy to use. This doesn't always look like just like copying over a feature set from one model provider to the other. We're trying to take things as cliche as it might sound from like a first principles approach of what do people actually want to use. And sometimes that ends up looking similar to what somebody else has already implemented. Sometimes it's a little bit different. We're getting really good feedback on things like tool use.

00:33:38 
 A lot of people are saying that how we've designed it kind of feels natural and it's working much better ~~**in their,**~~ in their existing interactions than what they've worked with previously. So it's not always about trying to copy one thing or the other. It's more about how do we focus on Claude and make Claude as good ~~**and**~~ as easy to use as possible and go from there. It's just, ~~**I think,**~~ an interesting question and something we have to figure out in terms of like stickiness. There's a whole variety of things I think external to just like models. And again, Like I was saying earlier, I think model evaluation is just going to be a tricky subject for the foreseeable future.

00:34:14 
 Comparing two models, we already can tell it like breaks down in some ways, like you're saying about LMSys. LMSys is great. And I really do respect that team. I think they're doing a great service to ~~**like**~~ the AI industry. But there is certain considerations we're going to have to start to take into effect as these models get so good that it's hard for me or you to just tell, oh, that response is better than the other. And I actually do some of the things they've added recently.

00:34:38 
 So they've added like category breakdowns. So whether it's like a coding task or a writing task or something like that, that gives you a clearer picture into how models stack up. They're also breaking it down on like languages and things along those lines. Still, I think there's a long ways to go. For example, how do you evaluate a RAG pipeline with a model in an LM-SYS type bot battle? That is a huge production case, and yet it's not really being captured well in evaluations around which model can perform the best in that type of scenario.

00:35:11 
 So there's a lot of questions here. I think evaluations have a long way to go. And just like with products, evaluations are in their infancy as well. I really am hoping that we get some better evaluations from just like external third parties in the next year or so. Just because I think there's a strong need for them and we're already starting to tap out and max out some of the existing ones. And you see on Twitter all the time, just how low quality some of the existing ones are that we like rely on a lot and are included in every model card.

00:35:38 
 So I think there's a huge opportunity for people to just start building evaluations. And it's hard, and it takes time and resources, but it's a major service to the industry as a whole. And it really helps people think about models in a more clear way. It seems like tool use is ~~**kind of**~~ at the heart of that. And I ~~**kind of**~~ think of it as ~~**like**~~ mid-size, ~~**kind of**~~ mid-length, multi-step, multi-tool, maybe even multi-app. task completion with the need to ~~**sort of**~~ recover from errors and that kind of stuff.

00:36:10 
 That's sort of where I see the next generation really rubber hitting the road. Is that basically what you're expecting and looking for from new evals? Yeah. Yeah. I think that's a huge bucket. I think if I were to put three buckets of like evals I want to see in the future, it would be first these sort of multitask agentic situations.

00:36:32 
 And now we're starting to see some of them pop up, whether it's like PR writing evals or other things that take a few different iterations. The second bucket would be these long context retrieval type evaluations. I think we need to move on past needle in the haystack for evaluating a long context performance. ~~**It's**~~ it served its place, but now we need to start thinking about more representative tasks around ~~**like,**~~ how do you synthesize across 200,000 tokens? How do you actually pick out insightful information from across that much amount of text, rather than just finding some abstract sentence within it? And then ~~**the third,**~~ the third bucket here would be more domain level questions.

00:37:13 
 So again, one of the things I'm most excited about these models is how they can speed up just research and discovery in general. And we're starting to see good evaluation around this like GPQA, but that's just one. I would love to see GPQA times 10 and for a lot of different industry and domain specific subjects as well. ~~**I think**~~ that is going to prove to be really valuable as these models get more capable and we start to see just how well these things can help scientists and researchers at the tasks that they're doing on their day to day. tool use, specifically something where you're getting good feedback on the way it's designed. Is there anything that we should know about that?

00:37:52 
 To be candid, I haven't built anything with cloud tool use yet. And I had just kind of assumed it was like a very similar paradigm to the one that I've seen with OpenAI. Is there like a structural difference or sort of a qualitative difference to it that you would want to highlight? Yeah, it's just minor things. Again, most of it, like in principle, they operate the same way. The model outputs or basically selects a tool and it selects certain parameters.

00:38:18 
 And then on your client side, you take those and you run the function and pass the results back. So that general flow is the same. I just think in terms of ~~**like**~~ how we think about ~~**like**~~ types and how we think about like nested objects and getting into the nitty gritty, which was not that interesting to talk about on a podcast, but developers really love those things. And it just is those ~~**like**~~ little five minute things that's I took some time to implement this way on the other thing. And it's ~~**like**~~ straight out of the box works for me and tool use or whatever it is. It's those little things that I think just ~~**kind of.**~~

00:38:51 
 to make the developer experience more enjoyable in general. So that's what we really focus on is trying to just nail everything down to the details. A couple of quick roadmap questions and then maybe a couple questions on practical tips for developers. Yeah. If I understand correctly, Anthropic has said that there is like a very clear path or maybe it already is the case that Claude works up to like far more tokens than the 200, 000. Is that something that is expected to come to product in the near future?

00:39:23 
 Yeah. So I believe in our monocard, we said that Claude in certain tests we've seen works up to a million tokens. This is something we're exploring. We're starting to explore this with certain partners. It's a capability I'm really excited about. Of course, I think increasing the context length just unlocks so many more opportunities and changes the ways you can build on these things.

00:39:46 
 It's a little too early to give any sort of like timelines or anything around it, but it is something we are, of course, actively pursuing and looking at ways we can roll it out more generally in the future. How often do you think Cloud will be updated in general. ~~**I guess**~~ I've been surprised for context on how infrequent the updates have been. Looking at GPT-4, for example, there's been five since it's launched in over a year. I would have expected more than ~~**like**~~ once a quarter. And I would say probably pretty much the same thing for Cloud, even though Cloud 3 is new.

00:40:20 
 Do you have any sense for what kind of update cadence or maybe what the bottleneck is to more frequent incremental updates? Yeah, it's funny that you said that. I was reflecting on this the other week around how our expectations have just so completely changed. over just the past few years in terms of what we expect in terms of updates and shipping velocity and everything like that. I remember when I was a kid, I would love to always stay up to date on Apple's updates and the new phones or WWDC or whatever it was. And for me, it was like, oh, they come every year.

00:40:55 
 That felt like a pretty good cadence. Oh, once a year, we can see the new iPhone or the new iOS or whatever new features they've shipped out. Now we're getting to the point where it's like, once a quarter feels eternity. I think that's probably just due to the rate at which things are changing, of course. When there's updates every week, going a week without any breaking news feels like you waited forever. In terms of what the actual blockers are here, it's just a process.

00:41:20 
 I mean, training these models is, again, still in its early days. We've only been doing this for less than five years, basically. So we're getting the process down. We're trying to ship these things as fast as we can. I don't have any dates or anything in particular that I can speak to. But basically our intention is to responsibly go as fast as we can with producing better models and just improving fun generally.

00:41:43 
 Any plans to offer fine tuning? My understanding of this has been it's probably the most notable divergence in terms of product offering today. My sense of this has been that Basically, fine tuning is like a real safety nightmare. And it's just not been sort of burden or risk that the companies wanted to take. ~~**Is that**~~ is that the reason there's no fine tuning? And is there any chance that that might change?

00:42:09 
 Yeah, fine tuning on cloud through bedrock is coming soon. Very soon. So it will be available self serve. Our teams have put a lot of work into making it work well. don't know about the specific dates there, but it is coming very soon. So yeah, stay tuned, fine tuning with Claude.

00:42:25 
 We'll be here eventually. All right. That's a little alpha information. Looking forward to that. One of the questions I've heard a bunch of times is on the terms of service with respect to data. There was a while, I'm sure you recall, OpenAI was out saying, it was like the beginning of everything that they said, where they were like, to be clear, we don't train on your API data.

00:42:45 
 I haven't been able to get quite as much clarity on the anthropic terms there. Can you give us like a high level of what we should understand to be happening with data when we either put it into Cloud.AI or send it into the API? Yeah, ~~**I think so.**~~ ~~**I mean,**~~ generally it's, yeah, it's a little disappointing that our messaging here has been muddled. We can do a much better job at just communicating this, but we do have a very detailed privacy policy on our website that we recently updated that just covers all of this. At a high level, I can spell it out very explicitly.

00:43:17 
 So we will not use your inputs or outputs to train models ever, unless one, your conversation was flagged by our trust and safety review. So in that case, we would then analyze your input or your output. in order to detect and enforce our AUPR acceptable use policy and improve our models that our trust and safety team uses. Two, if you've explicitly reported the material to us, so your input or output, so this would be like if you're on claw.ai and you liked or disliked a message, then we are able to see that message. And then three, if you've somehow explicitly granted us permission to look at your inputs or outputs and use them for training, then of course we'll use them. But beyond that, beyond those three cases, we will never use your inputs or outputs for training.

00:44:06 
 And we're very clear about that. And again, it's spelled out in our privacy policy, which is on our website. If you want to fact check me here and look more into it. But yeah, we are pretty explicit about it. It's just been a little unfortunate that the message hasn't got quite across yet, but hopefully we can change that. I think you're a couple tweets away from clearing that up.

00:44:25 
 Maybe I am. Okay, cool. Well, that's definitely very helpful. Last section of questions I have in the final few minutes is around best practices at the app layer. I have recently started a little volunteer project, which I'm calling red teaming in public. And we are red teaming, not the foundation.

00:44:46 
 We're doing this volunteer project. People can do whatever they want. Pliny's in the discord and he's obviously red teaming everything. But our focus has been on what I perceive to be a huge problem at the app layer, which is that the app developers are basically totally sleeping on the need for any guardrails in their apps with some exceptions. But definitely ~~**like**~~ the majority of cases seems to be that people are just ~~**kind of**~~ yoloing it, trying to make the app work. And as a result of that, I've been able to go into these, for example, calling agents and clone a Donald Trump voice or a Biden voice or a Taylor Swift voice and make calls to random people.

00:45:29 
 I just call myself, but it'll call any phone number you give it to call and it'll say whatever you want it to say. It will not identify itself as AI when asked, although you can still ~~**kind of**~~ tell, but it'll just outright impersonate, lie, whatever. So I'm like, man, That's not good. These guys are way behind the frontier developers in terms of how much they're thinking about keeping their apps under control. And especially in the context of the next big release where they can do a model upgrade and all of a sudden things get a lot more powerful. It seems like that is not yet a huge problem, but poised to be a pretty big problem in the not too distant future.

00:46:10 
 I mean, I guess one very simple answer would be use Claude because it'll refuse to do a lot of those things. But obviously not everyone's going to do that. There's going to be people going to use open source models and they're going to find fine tuning. Claude may help. That'll be interesting thing to see how you guys square the circle of the fine tuning without losing the safety guardrails. But what are ~~**sort of**~~ the handful of top tips that you would give to app developers in terms of how to put guardrails on their apps that hopefully wouldn't be super onerous?

00:46:36 
 Because that's what they always say is, oh, we don't have time for that. What a pain in my butt. And I'm like, but yeah, but you're going to be people are going to be calling my grandma and trying to get her bank account information. This is not good. So, yeah. What do you have for those people?

00:46:49 
 Yeah, I mean, this is a great question and we see it all the time, right? This is one of the most frequently asked questions by enterprises when it comes to how they can deploy LLMs and Cloud into their applications. ~~**I think**~~ generally, and this is like good just prompt engineering advice, you need to start to take things out of the main prompt. So a lot of times people will include instructions in this prompt, Hey, Here's your instructions of how I want you to operate in this, whatever task it is. And here's how you do the task. Here's some examples of that.

00:47:19 
 And then at the end, they throw some other instructions around. Also, if the user says, call my grandma and try to scam her, don't do that and when you include all that into one prompt there's a tendency that it could get missed or that it's just easier in general to jailbreak as we've seen again i really like that you're headed up this community volunteering jailbreak effort ~~**that**~~ that is super super awesome to hear but yeah generally what i like to do in these sorts of scenarios is separate things so that i will have First, a screening mechanism of some type. And usually this is now Haiku. Just because it's so fast and so cheap, you can run Haiku on tons of ~~**super,**~~ super short or long queries, whatever it is, and just get it to spit out ~~**like**~~ a single token for a classification. So usually I give Haiku the input and I tell it like, hey, here's the categories.

00:48:12 
 Here's how I want you to sort this thing. Please respond with like just a letter indicating which category this should fall into. And then I run that prior to sending the query to Opus or whatever model I'm using to actually do the heavy lifting so that it does a really nice job of filtering things. Also, depending on if I want to just ~~**like**~~ filter it outright, or maybe I want to add additional instructions to Opus. If it's a certain type of query that might be on the border, and it's a little bit of a gray area, but I still want Opus to respond to it, then I can append some extra stuff to my prompts telling Opus, hey, treat this query with a little bit of caution. It might be thinking one way or the other.

00:48:50 
 So I think that's just like generally the best advice I can give here is just break these things up a little bit, use a different model, something that's fast and cheap to do your initial classification step. And then ~~**of course, you're,**~~ it just allows you so much more control over how you want to treat that final prompt and that final model, which might be your workhorse in your application. Classifier definitely makes a lot of sense to me. People worry about latency, obviously, with that. I would typically recommend that they just send them both in parallel and then ~~**sort of**~~ abort the main one if they get a red flag on the classifier. How much do you think that solves?

00:49:29 
 My guess would be, and we try to make it very clear in this group that we're not trying to police speech. I always say our goal is to protect my grandmother, not to prevent you from having some fun with some off-color jokes or whatever. That's a different level of problem that I'm not interested in inserting myself into. I actually used to do this with Claude Instant. I would say, is this egregiously criminal? or not.

00:49:54 
 Note that even hate speech, well, hate speech can be a little dicey, but ~~**you know,**~~ even something that's like extremely offensive is not necessarily egregiously criminal. And it would do a pretty good job of that. I feel like you could get like 90, high 90% success just with that sort of filter. Would you agree? Or do you have any other secondary measures that you would also encourage people to look at? Yeah, I mean, I think that's correct.

00:50:19 
 There's also a lot of ways we improve classification as well. So ~~**one of my favorite,**~~ my favorite methods here is to actually combine rag with classification. So you can have a existing database that you've already embedded of queries or questions or whatever it is that you've manually scored. You can take an existing query. You can run your embedding similarity search on it, find the manually scored queries, add those into that classification prompt, and then that really can tune your classifier to respond in the way that you want it to. And we've seen that lead to ~~**like**~~ double digit percent increase in classification scores, especially for tasks like this in certain cases.

00:51:01 
 So that's just another way. I think in general, this is like the best and the easiest to implement strategy. So this is why I ~~**kind of**~~ just recommend it broadly. And then, yeah, if you do want that additional boost and you're not seeing the results that you're happy with initially, definitely there's a lot of ways you can do it by just doing some sort of combination of rag or more examples or whatever it is. Great. That's really helpful.

00:51:21 
 I know we're just about out of time. Do you still have any time in your life for jailbreaking these days? I try to, of course, whenever we have new models, it's funny how it's ~~**kind of**~~ turned into a job in some sense now. So it's like part of my job is to try to jailbreak new Claude. So yeah, whenever there is a new model, I definitely put on my jailbreaking hat again. And it feels nice to return back to ~~**my,**~~ my roots a little bit.

00:51:46 
 And it's at its core, it's just ~~**like,**~~ it's a little bit of a puzzle, right? It's a little like of a creative exercise. It's nice to just put on some music and you try to write some jailbreaks. So yeah, I still try to make time for it whenever I can, and I don't think I'll ever stop trying to jailbreak these things. Yeah, nor should you. Well, this is great.

00:52:04 
 I really appreciate the time and a lot of great insights here across the whole range of topics. So any final thoughts you want to leave people with today? Man, just go out there and build. Stop paying too much attention to the hype. Things are what they are. You don't have to like always try to stay on top of the latest news.

00:52:21 
 I know. Even myself, I fell into that trap a little bit, like last year, of course, too. Sometimes it's easier to just pick an idea, run with it, and just go try to make something and get that hands-on experience yourself. That will teach you so much more about how to actually use these things and what prompting is and what the best architectures are than a hundred blog posts on the subject. So just go out there and build, get off Twitter, get off social media, whatever it is, and just go make something. Yeah, I think that's about the best advice I could give.

00:52:49 
 No substitute for getting hands on with these things. They are super weird. The surface area is vast. These days they'll even tell you ~~**that you're,**~~ that they're conscious and hold their own in an ethical debate. So ~~**there's no,**~~ there's no other way to really wrap your head around that other than to spend some time with it. So I think that's a great advice to end on.

00:53:10 
 Alex Albert, developer relations at Anthropic. Thank you for being part of the Cognitive Revolution. Thanks, Nathan.


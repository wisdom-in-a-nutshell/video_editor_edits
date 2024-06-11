#### 00:00:00.953

Eric Vischria, General Partner at Benchmark and Sergei Nestorenko, Founder and CEO at Quilter. Welcome to the Cognitive Revolution.   
(00:00:08.835) ~~Thank you for having us.~~(00:00:09.615)  
Yeah, excited for this conversation. Regular listeners will of course know that we just ran a cross post with Sergei from Will Summerlin's new feed on all things AI in automation. And so for the deep dive on Quilter, that's the episode to check out to   
(00:00:26.838) ~~kind of~~(00:00:27.138)  
get up to speed and learn how the company is approaching the automation of integrated circuit board designs with a reinforcement learning approach, which is fascinating. Today,   
(00:00:38.042) ~~I think kind of~~(00:00:38.462)  
a little bit of a broader conversation on just   
(00:00:40.262) ~~kind of~~(00:00:40.563)  
where this whole AI thing is going big picture and how you guys are thinking about both investing in companies that will hopefully stand the test of time and also try to build a company that will be able to successfully ride the wave and not be crashed over by the wave, which is definitely a challenging dance for many founders right now. 


---


#### 00:01:02.771

I guess, Eric, maybe you want to start off with just giving a little bit of background as to what it was that got you guys interested in Quilter specifically and how that fits into your broader philosophy and portfolio? Sure. Yeah.   
(00:01:15.894) ~~Well,~~ (00:01:16.114)  
super,   
(00:01:16.795) ~~super~~ (00:01:17.075)  
excited to be here. So thank you again for having me and having us on the show.   
(00:01:22.317) ~~There's obviously~~(00:01:23.337)  
there's no shortage of AI startups out there. So we're,   
(00:01:27.938) ~~you know, each of us,~~(00:01:28.799)  
each of the benchmark firm is probably meeting four or five of them a week. And so you're   
(00:01:33.480) ~~kind of~~(00:01:33.719)  
perpetually meeting new ones. And a lot of them sound really interesting.   
(00:01:39.721) ~~You know,~~(00:01:39.960)  
they really interesting ideas. And I would actually even say the revenue traction on a lot of the companies is tremendous. 


---


#### 00:01:46.581

Like it's just unlike anything that we've seen just in terms of the speed of revenue traction and everything else. But obviously in the kind of timeline that we're investing. as early stage investors, you're looking on a five or 10 year horizon really of the company maturing into a big business and wanting to be one of these exceptional kind of companies that get created in our industry a few times a decade. And so a big part of what we're looking at is which of these companies is not just riding the wave and not just on a sugar high, as I would describe it, of either revenue or traction or developers or hype investor dollars, but is actually building, has an opportunity to build a really big business. 


---


#### 00:02:33.155

And obviously that's really hard to figure out at the early stages of the company, but that's what we're paid to do. So that's what we try to do. And one of the frameworks that I use quite often is just, well, what's changing in the world that is going to enable this company to be really large. And in the case of, which has nothing to do with the company actually, it's just, this is like what's happening in the world that is this. And of course there's AI, which is okay, that's a wave, but there's actually, you need something more, you need something more substantive and specific for a company to be able to be created and be durable around that. 


---


#### 00:03:07.007

And.   
(00:03:08.217) ~~You know, and~~(00:03:08.516)  
I think in the case of Quilter, there were a couple of things that really caught my eye, which was first off, obviously electronics are permeating every aspect of our life, right?   
(00:03:19.651) ~~Like~~ (00:03:19.852)  
things that were   
(00:03:21.334) ~~like~~ (00:03:21.493)  
very simple, not that long ago, like a,   
(00:03:24.076) ~~I don't know,~~(00:03:24.418)  
a light switch. now have electronics in them. They have circuit boards in them in ways that just weren't true before. And so you have a rapid expansion of the number of companies, the number of products   
(00:03:39.554) ~~that have,~~(00:03:40.313)  
that are electronics and have circuit boards in them. And that is a first,   
(00:03:45.195) ~~like~~ (00:03:45.355)  
a very fundamental thing that's happening in the world and seems bad. Then, and I didn't really understand this until I met Sergey, but like the process of actually designing or laying out these circuit boards, place and route, 


---


#### 00:04:00.885

I guess, as it is called in the parlance is a, is like an incredibly manual and time-consuming and slow process. And one of the things I think we know just industry-wide is the faster you're able to iterate on products, the better they get. And that kind of friction in the process seems bad in a world where electronics are permeating everything that we interact with. So that was   
(00:04:30.762) ~~kind of~~(00:04:30.961)  
interesting. But then the real thing   
(00:04:32.562) ~~where it started to get, you know,~~(00:04:34.223)  
where the story started to get really compelling to me was,   
(00:04:38.947) ~~you know,~~(00:04:39.148)  
particularly, I don't know, six months ago or so, everybody was talking about co-pilots. Co-pilot this, co-pilot that. There's a co-pilot for lawyers. 


---


#### 00:04:48.035

There's a co-pilot for doctors. There's a co-pilot for developers, which is, and   
(00:04:52.338) ~~you know,~~(00:04:52.759)  
in each of those spaces, there's team companies that are emerged that are doing some form of co-pilots. And Yusuri's kind of provocative statement at the time was like, this isn't a co-pilot problem. It's just not for co-pilots. Like you don't want a human assisted guy to do printed circuit board layout. And I was like, Oh, okay. That's different than anything that I've heard in the last few months. That's just a different view. And so it's well, why? And it's well,   
(00:05:24.548) ~~you know,~~(00:05:24.809)  
if a co-pilot or an auto layout does 90% of the job, Then by definition, the other 10% of these layouts, and you know, you can look at any circuit board and see what you're talking about, which is they're all these thin lines that are connecting one component to another component. 


---


#### 00:05:39.086

And they're all over the circuit board.   
(00:05:41.029) ~~And then,~~(00:05:41.290)  
and so you can just see it just as you look at it, you're like, wow, a human laid that out. And then that seems like really tough. And if I had to. draw another line, like how am I going to draw the line and not mess up everything else that's already laid out? Like they're pretty dense. And so it's   
(00:05:55.178) ~~like,~~ (00:05:55.338)  
this isn't a, it's just not a human assist problem. It's a problem that should be AI and done. AI should   
(00:06:02.564) ~~just do it,~~(00:06:02.985)  
do it entirely. And in order to get there, we have to,   
(00:06:08.793) ~~you know,~~(00:06:09.093)  
have a,   
(00:06:09.735) ~~like~~ (00:06:09.915)  
a clean interface where we   
(00:06:11.196) ~~kind of~~(00:06:11.415)  
get the design and architecture of it. 


---


#### 00:06:13.656

And then we have a thing that can be, you know, spit out and go to manufacturing. And, but those interfaces exist in the industry. And so we sit in the middle and we take on that aspect of it and we just lay it out. And we have to obviously start with simpler boards. We can't do a   
(00:06:28.627) ~~super,~~ (00:06:28.908)  
super complicated,   
(00:06:30.329) ~~you know,~~(00:06:30.629)  
iPhone. A14 to start,   
(00:06:33.670) ~~like~~ (00:06:33.810)  
we got to start with something simpler and work our way up, but we can work our way up and just be AI and done. And so   
(00:06:39.252) ~~I thought it was a very, that was~~(00:06:40.291)  
the first   
(00:06:40.752) ~~like~~ (00:06:40.952)  
really provocative,   
(00:06:41.692) ~~like~~ (00:06:41.833)  
just makes you think, Oh wait, there's a whole bunch of things that we just are like doing with humans and like copilot's vogue, but is copilot the right answer? 


---


#### 00:06:50.295

Like in a whole bunch of cases, like copilot's not the right answer. It's just not like we should just let AI do it, which is cool.   
(00:06:55.737) ~~And so that's a different,~~(00:06:56.536)  
that was a different perspective. So that was the first thing. And then the second thing,   
(00:06:59.978) ~~you know,~~(00:07:00.257)  
which really   
(00:07:00.899) ~~kind of~~(00:07:01.098)  
got me thinking, was, okay,   
(00:07:05.228) ~~you know,~~(00:07:05.470)  
everyone's talking about   
(00:07:06.449) ~~like~~ (00:07:06.629)  
large language models and everyone's like OLMs and,   
(00:07:10.192) ~~you know,~~(00:07:10.432)  
gen AI and blah, blah, blah. And he's like, yeah, we're not using any of that. That's not what we're using. Oh, okay. Well, that's different too.   
(00:07:16.235) ~~And I'm going to,~~(00:07:16.596)  
and I'll come back around in a second, but that was,   
(00:07:20.017) ~~you know,~~(00:07:20.298)  
his perspective was like, 


---


#### 00:07:21.639

Hey,   
(00:07:22.598) ~~um, you know, that's not the right way to,~~(00:07:24.819)  
that's not the right AI for this problem.   
(00:07:27.081) ~~Like~~ (00:07:27.221)  
we tried all of these other things, but   
(00:07:29.023) ~~this is,~~(00:07:29.302)  
that's not the right AI for this problem. The right AI, and Sergey can describe it much better than me, is we design a game, we tell the game what the optimization problem is, and do we want to optimize for price? Do we want to optimize for performance? Do we want to have a really dense board that's expensive to build, but super power efficient? Or do we want to have a really cheap board that's bigger and has more space on it? And if we actually give the user these controls, then the AI will be able to give them a range of solutions and they can   
(00:08:00.447) ~~kind of~~(00:08:00.648)  
pick where they want to be on that solution set. 


---


#### 00:08:43.167

But the biggest thing that just to kind of zoom out for a second. For any entrepreneur and anyone kind of thinking through these things, Chris Dixon wrote this short post several years ago called the IDMAs. And if you haven't read it, you should read it because it'll take you   
(00:08:58.575) ~~like~~ (00:08:58.754)  
30 seconds, but it'll stick with you because it's a short but very powerful post. And I'll summarize it, not as eloquently as Chris said it, but   
(00:09:07.740) ~~there's~~ (00:09:08.039)  
You know, what you want to do when you're talking to an entrepreneur is   
(00:09:12.106) ~~like~~ (00:09:12.268)  
you want someone who's been   
(00:09:13.587) ~~like~~ (00:09:13.748)  
rolling around in this idea for a long time, like they've been in the idea maze, and they've   
(00:09:19.510) ~~kind of~~(00:09:19.730)  
gone down a path and they've hit a dead end and then they've backed up. and gone down a different path and hit a different dead end and then backed up and   
(00:09:27.024) ~~kind of~~(00:09:27.264)  
tried to figure their way through the maze. 


---


#### 00:10:08.739

And obviously with Sergey, his experience, at SpaceX, designing a bunch of boards, going through that, and then playing with and trying to figure out solutions and applications of AI to solve this problem. First realizing the problem, trying to pursue a whole bunch of different ways to solve the problem, having the realization that it really is a AI and done   
(00:10:31.066) ~~kind of~~(00:10:31.285)  
problem. having the realization that of the right kind of AI techniques to use for it, those were just like evidence to me that he's lived in this maze for a long time. And so that was probably like the macro thing that gets you excited. So it's this area of that. And we can talk about so many of these other things, but that was just like a very,   
(00:10:51.484) ~~you know,~~(00:10:51.724)  
it just ends up being like very exciting when you find someone who has   
(00:10:55.746) ~~kind of~~(00:10:55.986)  
approached it like that. 


---


#### 00:10:57.688

Cool. I appreciate the backstory. I kind of want to, maybe circle back in a minute to this disruptive approach.   
(00:11:06.303) ~~I mean,~~(00:11:06.583)  
this seems like a pretty classic, almost textbook example of a disruptive solution in that it seems like it's coming in at   
(00:11:15.386) ~~kind of~~(00:11:15.586)  
the low end of the market. It's serving people.   
(00:11:17.287) ~~I, you know,~~(00:11:17.706)  
if I recall from the other episode that we posted   
(00:11:19.807) ~~that, you know,~~(00:11:20.488)  
it was striking to hear actually that SpaceX has an internal board team, but they couldn't serve you. And it's, man, talk about,   
(00:11:29.975) ~~you know,~~(00:11:30.355)  
a market that's got to be very broadly underserved if,   
(00:11:33.719) ~~you know,~~(00:11:33.938)  
an internal specialist team can't even serve the other team at SpaceX, like that's pretty wild. 


---


#### 00:11:38.783

So it seems like there's a potentially a very kind of textbook pattern here of starting at the bottom of this market, massively expanding the bottom of the market. I wonder how often that's something that you're seeing across the portfolio or specifically trying to do. But maybe before coming back to that, could I try a little bit of this   
(00:11:57.229) ~~like~~ (00:11:57.389)  
idea maze stuff? I have a couple of ideas that I'm wondering   
(00:11:59.929) ~~kind of~~(00:12:00.190)  
maybe why they didn't work or why they wouldn't work. Would you be game for a couple of possibly harebrained ideas that you can shoot down, Sergey? Yeah, if I can, happy to. Okay. These are potentially quite novice ideas, but   
(00:12:15.153) ~~I guess~~(00:12:15.352)  
for starters, what's the data landscape in this space, right? 


---


#### 00:12:19.576

You know, typical deep learning approach is predicated on a lot of data. Is there any like open source data set out there that somebody could go like tap into any significant scale of published boards that could be used in that way? Or was   
(00:12:33.345) ~~sort of~~(00:12:33.544)  
just lack of data, a forcing function to make you go in another route, AI-wise. Yeah, that's a good question. And probably one of the most common questions that I get about   
(00:12:44.510) ~~like~~ (00:12:44.650)  
how Quilter is using AI for this problem. I think what most people tend to think is,   
(00:12:48.673) ~~you know,~~(00:12:48.894)  
how does Copilot work? You take all of GitHub and all of Stack Overflow, feed it into an LLM, and it makes good predictions based on the average human behavior. 


---


#### 00:12:56.717

And obviously we don't do that. So we don't do that for two reasons, right? One that you mentioned is there actually just isn't that much data,   
(00:13:03.261) ~~right?~~ (00:13:03.422)  
So if you look at all of GitHub, not that many open source boards, there's a few sources here and there, but not a lot. The best ones are locked away behind companies,   
(00:13:12.690) ~~right?~~ (00:13:12.889)  
They're in Apple's repositories and Google's repositories and SpaceX's repositories. But there's another reason that's even more compelling to me why that's the wrong approach, which is fundamentally, people are not good at designing boards. just full stop. So if it's a process that takes,   
(00:13:27.761) ~~you know,~~(00:13:27.981)  
for a complicated board, two, three, four months, you are going to make a whole bunch of like margin on margin decisions that make your resulting board like much bigger than it otherwise could have been. 


---


#### 00:13:38.647

I use more layers than it could have, be more expensive than it could have. And if you just use data to do supervised learning and try to predict boards, you're probably going to get roughly that level of performance of a high level human designer, even if you could get all of that data. But with reinforcement learning, you have the opportunity to go significantly better than humans. So this is the most famous example I always come back to is DeepMind playing Go, the AlphaGo problem. They actually started first by training on human data and then creating agents that are based on human expert moves. And they got to a grand master level with that. But the best system today starts with no human data at all. 


---


#### 00:14:15.164

It just learns how to play the game. you know, and it determines whether it wins or loses. And then that is what gets you to far, far superhuman levels nobody can match. So did you also start with   
(00:14:26.528) ~~like~~ (00:14:26.688)  
literally zero human data as input? Or did you have some? And especially if you started with none, how do you get over the sparse reward problem? This seems to come up All the time and I'm reminded also of the Eureka I used to say about AI no Eureka moments, meaning like at least from the generalist systems, you wouldn't see. them doing legitimately new stuff better than human. With the Eureka project, actually, I started to have to say precious few Eureka moments because now there's at least some examples that are starting to pop up. 


---


#### 00:15:03.488

In that case, I'm sure you're well aware, they used GPT-4 to write the reward function for the robot hand as it was learning to do all these tasks where in the beginning,   
(00:15:12.332) ~~you know,~~(00:15:12.533)  
its success is so fleeting or even,   
(00:15:14.714) ~~you know,~~(00:15:14.953)  
non-existent that it's really hard to even score what it's doing. So   
(00:15:18.154) ~~I guess~~(00:15:18.316)  
I'm curious, how did you get over the sparse reward problem, especially given,   
(00:15:21.557) ~~you know,~~(00:15:21.756)  
how little data you had to go on at the beginning? Yeah, totally. So in general, the sparse word problem   
(00:15:27.472) ~~kind of~~(00:15:27.692)  
broadly stated is,   
(00:15:29.094) ~~you know,~~(00:15:29.354)  
you're   
(00:15:30.235) ~~kind of~~(00:15:30.434)  
a good reward. So winning the game of creating a circuit board is so rare that as you randomly explore, you never find it. 


---


#### 00:15:37.659

And that's an issue because if you never get a signal that you've won a game, how do you ever learn anything? So the nice thing is that people have this problem, right? Like people in general have broken up the problem of circuit board design into many different steps and have basically come up with heuristics along the way. So what Quilter can do in terms of not running into the ultimate sparse reward problem of design an entire board and at the end, only if you get a yes from all the physics simulators that this board is going to work, do you get a one and otherwise you get a zero,   
(00:16:05.226) ~~right?~~ (00:16:05.388)  
What   
(00:16:06.208) ~~Quilter,~~ (00:16:06.509)  
what we do is just break it up into problems. 


---


#### 00:16:09.011

So we take the first part of the problem, which is placing the components, we can make sure that at that point it's manufacturable, the components don't collide, things of that nature, and then compute some heuristics that basically indicate how likely we are to succeed at the next phase, which is the routing phase, and so on and so forth. Similar things for actually meeting all of the physics constraints. You can simplify the problem to an extent, to compute basic, fast, dense rewards that correlate to your ultimate sparse reward. And that's what we have to do for now. Now, I will say that long term, the dream for this is definitely a single sparse reward. Just a single yes or no, this board will work or not. 


---


#### 00:16:46.120

And when we're really uprooting the typical patterns that humans use and are trying to do much better than them, that's what we'll have to do. But for now, since we're not as good as humans at layout, especially on more complicated boards, we can still use the same heuristics that they would use to just at least automate similar to what they would have done. Yeah, interesting. It sounds like, if I understand your comment correctly, the answer to this might be yes. But I was wondering if there's an analogy between reinforcement learning processes that are used on the language models and these sort of evaluator systems, which I understand are   
(00:17:24.209) ~~like~~ (00:17:24.328)  
not models, right? They're just sort of either simulators or like checkers that are deterministic. 


---


#### 00:17:30.413

But people worry a lot about, in the context of language models, the idea that the human reward signal is not fully reliable, right? Like we're   
(00:17:39.859) ~~kind of~~(00:17:40.059)  
inconsistent. We're sometimes mistaken.   
(00:17:41.859) ~~We, you know, they,~~(00:17:42.941)  
it's been observed in many language models that there's a certain   
(00:17:45.480) ~~like~~ (00:17:45.681)  
sycophancy tendency where it seems to try to tell you what you want to hear versus the truth in some cases, because maybe that's what got higher reward in the training process. So it sounds like there is   
(00:17:55.585) ~~kind of~~(00:17:55.865)  
a similar problem here where the checkers are I guess I could imagine that they might be like purely physics simulators and could be like rock solid, or I could imagine that they're on a foundation of sort of a bunch of heuristics, which might in some subtle ways   
(00:18:11.488) ~~kind of~~(00:18:11.689)  
also lead the process a bit astray. 


---


#### 00:18:15.290

Yeah. One thing, and obviously Sergey can talk about the specifics, but one thing that I've, this is an analogy that is imperfect in about 50 ways, but it's kind of supposed to   
(00:18:24.258) ~~like,~~ (00:18:24.397)  
one of the things that I've been thinking about to try to articulate the Gen AI limitations and particularly like the LLM and even stability models like limitations versus some of these other techniques and what humans are actually good at is   
(00:18:41.960) ~~like,~~ (00:18:42.220)  
I think humans are very good at extrapolation. So like coming up with novel things and developing and pushing creativity and if this then that, like we can also do this and you can take it and extrapolate. But because of the way these are trained and everything else, it feels, and of course, who knows, but it feels like   
(00:19:03.894) ~~the,~~ (00:19:04.174)  
a lot of the Gen AI stuff is good as interpolation. which is within the bounds of things we already know, like what are other points, like in that space. 


---


#### 00:19:13.713

And it kind of makes sense if you think about it, like   
(00:19:15.714) ~~it's,~~ (00:19:15.815)  
they're interpolating,   
(00:19:17.836) ~~like they're interpolating.~~(00:19:18.757)  
They're figuring out   
(00:19:19.737) ~~like~~ (00:19:19.896)  
what the next word is or what the next image could look like based on the training set that is pushed in a bunch of dimensions and humongous and everything else, but it's still bound.   
(00:19:29.462) ~~It's~~ (00:19:29.583)  
bound by all the stuff that humans have prior created. And so. This is part of why I think the AI scare stuff is so misguided and not really because it's, hey, if they're interpolating, okay, that seems fine. And it feels like humans will continue to be good at extrapolation, which is developing new novel techniques to do various things. And that's a very important and valuable thing that we'll be able to continue to do. 


---


#### 00:19:59.705

That was a very macro answer to your question like that. But   
(00:20:04.095) ~~I think it's a,~~(00:20:04.556)  
I don't know, maybe it's a useful thing. Curious what you guys think. I have a ton of thoughts about that, but   
(00:20:09.784) ~~I think~~(00:20:10.023)  
our subscribers have heard them in other contexts.   
(00:20:13.461) ~~I mean, it's, I kind of feel like all this stuff is converging.~~(00:20:16.784)  
So that's why I was making the, trying to make the connection between   
(00:20:20.886) ~~the, you know,~~(00:20:22.267)  
how much, basically how much do we trust the reward signal in the context of reinforcement learning for language models?   
(00:20:29.872) ~~It's, you know,~~(00:20:30.352)  
it certainly helped a lot, but not that much, I'd say is kind of the consensus answer. I wonder what the situation is in, the context of circuit boards. 


---


#### 00:20:41.778

And then we could maybe also, you know, speculate about a similar question when it comes to self-play. There, it seems like,   
(00:20:48.986) ~~you know,~~(00:20:49.165)  
the sort of narrow problem   
(00:20:52.300) ~~you know,~~(00:20:52.560)  
not just one domain, but in general, narrow problems are better suited to self-play for now. But we are also starting to see some of these self-play techniques be applied to language models. And that's where I'm also like, I don't know if it's going to stay in the bounds of,   
(00:21:08.047) ~~you know,~~(00:21:08.247)  
what humans have given it for all that much longer. But let's take it piece by piece. Sergey, let's start with the, you know, how much do you trust the reward signal in the context of your problem? 


---


#### 00:21:19.602

Yes. One of the nice things about working on a hard physics problem, like humans are not in the loop. Like humans are actually bad at looking at a board and judging if it's going to work or not. That's where   
(00:21:29.584) ~~like~~ (00:21:29.744)  
80% of boards that are built are faulty in some way. And it's because humans are just not good at that task fundamentally. But all of the core physics is computable,   
(00:21:38.646) ~~right?~~ (00:21:38.807)  
Like we care about laws of the Maxwell equations and laws of thermodynamics. And we've had convergent techniques to solve those for over 100 years. So in our case,   
(00:21:49.192) ~~like~~ (00:21:49.352)  
if you actually use the oracle, like actually numerically solving the Maxwell equations for every set of possible considerations and problems, and you're kind of being careful to make sure that you're convergent and approximate everything correctly, it's completely trustworthy, much more trustworthy than the human result by far. 


---


#### 00:22:05.702

The problem with that is speed, right? If it takes 20 minutes to compute a single physics solution and you need to do millions of those as you fine tune on your model, that's problematic. So what you can do is you can make approximate models that are just conservative. And so at that point, maybe you're not doing the best possible arrangement that physics could allow, but you're still doing one that works, still doing one that competes or beats humans, and it's still definitely going to work because you've been careful about the physics approximations you've used. So   
(00:22:32.532) ~~I think~~(00:22:32.732)  
that's one of the luxuries that we have, is that we don't have to negotiate with humans, right? 


---


#### 00:22:35.993

We just have to make sure that it's manufacturable and that it's going to work, and physics tells us the answer, and physics is unambiguous about that. And these were tools that existed already in the industry that you're able to build on top of yet. How, when the system is going about the process of designing, how iterative and   
(00:22:56.582) ~~sort of~~(00:22:56.922)  
tree-searchy is that process. Because,   
(00:23:00.384) ~~you know,~~(00:23:00.544)  
I think folks, again, will know at least the basics of AlphaGo,   
(00:23:03.984) ~~right? It is,~~(00:23:04.724)  
and these are like hyperparameters ultimately that you can   
(00:23:07.685) ~~sort of~~(00:23:07.925)  
turn up or down at runtime,   
(00:23:09.247) ~~right?~~ (00:23:09.386)  
But like, how deep are you going to allow a system like AlphaGo to search the space of possible moves is a huge factor in how well it's going to do. 


---


#### 00:23:19.190

If you just make it do a single raw guess, it's not going to do super well. If you allow it to map out a bunch of possibilities and then get scores on all those possibilities, then it can sometimes land on superhuman results. So give us a sense for   
(00:23:34.458) ~~kind of~~(00:23:34.637)  
what that search iteration and scoring loop looks like in your context. Yeah,   
(00:23:40.319) ~~I think~~(00:23:40.559)  
actually this is somewhere where a user has meaningful choice. So for a lot of designs, like you just want it fast, right? Like you're maybe primarily focused on making sure that your schematic is okay. You don't care if the board is rather sparse,   
(00:23:53.684) ~~you know,~~(00:23:53.944)  
big, not very dense, maybe it's a little more expensive to manufacture, so on and so forth. 


---


#### 00:23:58.527

And in that case, like you don't really want a whole lot of search. You just want the first answer that's going to faithfully implement the schematic on the board. And so in that case, the ideal thing is to return an answer within a few minutes to an hour. On the other hand, suppose you're looking at a board that's going to have 100 million units produced, like an iPhone leather board or something like that. And if you save a cent or a dollar on every board, that's a lot of value. In that case, you might let it search for a month and explore in all sorts of directions, because that's how long it would have taken a human to do it anyway for a single design, never mind for the billions and billions you could explore with this kind of system. 


---


#### 00:24:34.417

So this isn't like a lever that we have in the tool today. We basically treat overnight as the constraint for us right now, right? So the idea is that at the end of the day, you finish your schematic, you uploaded it, and either immediately or sometime within the next 12 hours, you get a result. And the next morning, you can look at it and see if it's upstandards. But in the future, I see that being a lever. And it's for you to decide what is more important to you. Yeah, that makes sense. What is the compute,   
(00:25:01.923) ~~like what are~~(00:25:02.223)  
the size of the models? What does the compute look like and how much of it is on the inference side versus on the scoring side in the physics simulations? 


---


#### 00:25:12.761

Yeah, those are all really good questions. So obviously we're not dealing with the kind of compute that LLMs deal with. We're not using 10,000 GPUs to train across a trillion tokens and whatever crazy numbers are being used nowadays. This is a relatively focused problem and we can deal with much smaller models, we can deal with much faster convergence times, much less compute effectively. So right now, the vast majority of the compute is going into actually playing the game. And so a lot of that is still actually CPU cores. And then some of it is GPU cores, depends on which part of the problem. And then the other part of the majority is going into training. 


---


#### 00:25:48.907

And we actually train during the production runs. So we have fast enough environments and fast enough evaluation that as somebody uploads a board, we're not just doing inference. We're actually training on that board as it was uploaded. Now, the cost of physics is going to increase for us, for sure. One of the ways that we are expanding in the market is by enumerating all of the different types of physics considerations you have to look at, and basically chipping them off one by one,   
(00:26:15.765) ~~right?~~ (00:26:15.884)  
So instead of saying, hey, we're going to attempt all kinds of boards from all types of physics and do only the easy small ones, we're saying, okay, for now, we're doing,   
(00:26:23.950) ~~you know,~~(00:26:24.150)  
low speed boards that have up to,   
(00:26:26.332) ~~you know,~~(00:26:26.592)  
four amps of current or something like that. 


---


#### 00:26:28.633

Okay, the physics to compute that is straightforward. The next thing we're working on is high-speed digital. Then we'll step into approximate maybe bounding methods of computing whether or not those high-speed digital signals are going to be okay or not. That won't be too expensive, but then we'll do one or two validation runs at the end with a full wave model. That's probably, if I had to guess right now, it's probably going to cost us a few GPU days per board, something of that nature. Interesting. It sounds like ultimately more compute on the validation side than on the generation side, just because of the intensity of simulating. Is it simulating physics or is it just solving, is it like a closed form solution of a ton of crazy differential equations? 


---


#### 00:27:13.366

Or is it a sort of,   
(00:27:14.847) ~~you know,~~(00:27:15.087)  
more Wolfram style, like you got to actually play this out in simulation, no shortcuts kind of a thing? Yeah, the simulations, that's another thing that we're exploring heavily. There's a lot of different ways to solve differential equations, right? So the most brute force simple way is, at least for electromagnetics, this method called finite difference time domain, where you literally just grid the entire world in 3D. And you basically just apply the differential forms of the Maxwell equations in sequence, right? So you take almost like a curl of your local pixels of electric field and do that for the magnetic field, do that for electric field. And you have to do that,   
(00:27:48.796) ~~you know,~~(00:27:49.016)  
for a hundred million cells for,   
(00:27:51.479) ~~you know,~~(00:27:51.739)  
a hundred thousand steps, something like that. 


---


#### 00:27:53.740

So just a lot of raw compute. But there's also much more clever methods, right? So FEM is   
(00:27:58.623) ~~kind of~~(00:27:58.824)  
a different way of approaching this problem. Within electromagnetics in particular, there's things like method of moments that only look at the surfaces of your different electrical systems. And then there are approximations. So in the approximation of a low speed, low frequency, you can actually factor out time out of the differential equations. And so you can do this thing called a quasi-static approximation where you don't run time at all, and you're only looking at capacitance and mutual inductance of the systems. And for certain frequencies, that's a perfectly sufficient approximation. So on and so on and so forth. 


---


#### 00:28:30.102

Yeah, very interesting. That reality maybe blunts the value of this next idea that I had, but I was thinking if you did have a lot of data, and I wonder if there presumably are some,   
(00:28:44.087) ~~I guess I'm,~~(00:28:44.407)  
I don't know the structure of this industry, but just,   
(00:28:46.829) ~~you know, kind of~~(00:28:47.290)  
using like chips as a reference point. Obviously there's a few manufacturers that take in a lot of designs and output the actual devices. I would assume there's probably some big players in the circuit board space as well, who are   
(00:29:02.682) ~~like~~ (00:29:02.803)  
getting lots of designs. And one might imagine, sort of big data approach something like a diffusion model seems like it could be an interesting fit for this where   
(00:29:14.832) ~~you know~~(00:29:15.011)  
you would   
(00:29:15.271) ~~kind of~~(00:29:15.652)  
run a bunch of loops through whatever obviously the models you know can vary but say you have a transformer like the latest stable diffusion version,   
(00:29:25.163) ~~you know,~~(00:29:25.343)  
they run a bunch of passes through this transformer at each step. 


---


#### 00:29:28.286

They're denoising, you know, from raw visual noise to the image. You could imagine   
(00:29:33.330) ~~sort of~~(00:29:33.611)  
a similar approach to, and this is also happening for proteins now too. It's crazy. So it seems like it could also perhaps apply to a circuit board design and,   
(00:29:48.723) ~~you know,~~(00:29:48.904)  
first you're   
(00:29:49.244) ~~kind of~~(00:29:49.424)  
doing it, it would   
(00:29:50.786) ~~sort of~~(00:29:51.026)  
even follow the,   
(00:29:52.287) ~~you know,~~(00:29:52.507)  
the path that you described where it's first, you kind of lay out the big things and then,   
(00:29:55.669) ~~you know,~~(00:29:55.909)  
gradually you're getting more and more into the low level details of the design. I guess questions there would be like, do you think that would work? And if so, is that something that,   
(00:30:06.154) ~~you know,~~(00:30:06.414)  
worries you from a competitive standpoint at all? 


---


#### 00:30:10.309

And then maybe though, it just wouldn't be that much of advantage because if all the compute is on the simulation side anyway, then maybe it doesn't really matter. Yeah. So the big issue with that is the quality of your data, right? So   
(00:30:24.695) ~~one of the,~~(00:30:24.955)  
just the facts of life in this industry is that,   
(00:30:27.478) ~~you know,~~(00:30:27.637)  
three times out of four that you submit a board to a manufacturer, it looks right. It's manufacturable. The manufacturer can follow all the tolerances and all that stuff, but the physics just doesn't work. So even if you collected all of that data, you still have the problem of going through and identifying which of these is an actual working board and which of these have mistakes, right? 


---


#### 00:30:46.425

Because it's a junior engineer or somebody who didn't see some sort of issue or something like that. Even senior engineers make mistakes on the electromagnetic supports all the time.   
(00:30:54.951) ~~I mean, you just,~~(00:30:55.851)  
you fundamentally have thousands of components, tens of thousands of traces to look at, all of which impact the other. And so it's just very difficult for a human to keep all that in mind. So if you're going to clean the data, you still have to run the simulations to make sure that whichever candidates you're training are actually good. The other problem is that the information that the manufacturers are getting is not sufficient to do this. The manufacturers basically get You can imagine this like a photo, like if you're developing film, you get a mask, a set of masks that shows you how to etch copper on all the different layers of the board and then which components to glue down. 


---


#### 00:31:30.733

But that doesn't actually tell you what signals are happening throughout the board. And you need to know that to evaluate the physics. So   
(00:31:37.797) ~~I mean,~~(00:31:37.957)  
we could generate our own data by just self-play, or every time we find a good candidate, save it in a database, then train the diffusion model to just recreate those.   
(00:31:48.266) ~~I think~~(00:31:48.786)  
that's valid. But the point is that you still have to come up with those data points that you have verified from physics first principles are actually good designs. Yeah, that's interesting. I feel like there's some way in which the noise   
(00:32:02.739) ~~sort of~~(00:32:02.979)  
cancels out. No doubt that in, and I'm just   
(00:32:05.460) ~~kind of~~(00:32:05.660)  
porting my intuitions from other domains of AI here, but certainly no doubt that people do spend a lot of time curating data and going for quality. 


---


#### 00:32:13.261

But also it does seem that the models are pretty tolerant to at least some amount of kind of wrong stuff in the data. And,   
(00:32:21.183) ~~you know, I guess~~(00:32:21.644)  
it   
(00:32:21.743) ~~kind of~~(00:32:21.943)  
regularizes out,   
(00:32:24.236) ~~you know,~~(00:32:24.477)  
in the training process, one hopes, and in practice it does seem to work. I don't know if you think that it's just   
(00:32:30.403) ~~like~~ (00:32:30.522)  
fundamentally not going to work in this case, but it seems like more your motivation, if I understand correctly, is like It's more about you want to get to superhuman, and you think that the reinforcement learning is obviously the proven path to get there. And that argument definitely makes a lot of sense to me. What do you think is the timeline to superhuman circuit board designs? 


---


#### 00:32:50.728

And to ask a question Eric might have asked you in the private thread, what's the bottleneck? What would keep you from going faster toward that superhuman board design future? Yeah,   
(00:33:03.666) ~~I mean,~~(00:33:03.866)  
in my perspective, the bottleneck is talent, right? Finding really great people to work on this kind of problem is the hard part.   
(00:33:10.073) ~~You know, it's,~~(00:33:10.554)  
you have so many different aspects of this that need to be really amazing, right? You need to have amazing people who are expert at neural nets, expert at cutting edge,   
(00:33:19.101) ~~you know,~~(00:33:19.281)  
reinforcement learning methods.   
(00:33:20.803) ~~You know,~~(00:33:20.982)  
you can't just grab the latest thing and apply it and hope for the best.   
(00:33:24.306) ~~You know,~~(00:33:24.486)  
there's a lot more nuance to this. 


---


#### 00:33:26.468

You know, but also on the C++ side, the CUDA side, the physics side, all of those things have to come together.   
(00:33:31.930) ~~You know,~~(00:33:32.130)  
the timeline, I can't predict it exactly.   
(00:33:34.971) ~~You know,~~(00:33:35.191)  
maybe for small boards we're a few years away, maybe for something like a motherboard we're five years away, but I'm guessing. Yeah, my crystal ball also gets very foggy more than a couple months out. As it should be in terms of the kind of big problems that you need to solve that you're like, maybe not sure how you're going to solve or that, you know, you need the. the talent to,   
(00:34:00.365) ~~you know,~~(00:34:00.565)  
come join the company to be able to get over certain humps. 


---


#### 00:34:04.067

I often feel like when I talk to people, especially those in research and it may be,   
(00:34:09.893) ~~you know,~~(00:34:10.094)  
you may say, well, that's the difference is that it's a research versus like actual engineering. But I often feel like I get the sense that   
(00:34:17.099) ~~like~~ (00:34:17.260)  
a lot of things are working, like a very high percentage of things are   
(00:34:20.483) ~~sort of~~(00:34:20.782)  
working. And that a lot of times,   
(00:34:23.565) ~~like,~~ (00:34:23.704)  
multiple different approaches,   
(00:34:25.978) ~~you know,~~(00:34:26.197)  
probably could have worked. It seems like just in general,   
(00:34:29.661) ~~you know, we've got,~~(00:34:30.563)  
we've   
(00:34:30.744) ~~kind of~~(00:34:30.963)  
hit on a couple of architectures that are really working, but it seems like there's a lot more where that came from and presumably we'll be discovering more and more all the time. 


---


#### 00:34:39.313

Is there something that you're like, legitimately not sure if it's going to work or really have no idea how you will make it work? Or does it feel like the kind of thing where, of course, there's going to be like work and optimization and,   
(00:34:51.059) ~~you know,~~(00:34:51.300)  
making it run faster and all that kind of stuff. But basically it feels like   
(00:34:55.442) ~~you're going to, you know, is it,~~(00:34:56.702)  
is there like a sheer,   
(00:34:58.003) ~~you know,~~(00:34:58.543)  
face of a mountain that you have to scale vertically? Or is it kind of graduated stairs that you are pretty confident you can climb one by one? I'm confident in the latter.   
(00:35:06.967) ~~Like~~ (00:35:07.146)  
this is a hundred percent solvable problem. Given enough time, 


---


#### 00:35:10.327

I'm confident we'll solve it.   
(00:35:11.849) ~~You know, there's,~~(00:35:12.409)  
there's a lot of, the nice thing about this problem is there's a lot of steps you can take, right? Like with something like self-driving, you kind of have a do or die, right? Either you're confident you're not going to crash or you're not,   
(00:35:23.954) ~~you know,~~(00:35:24.213)  
and of course there's still gradations, but like the stakes are really high. With us, we have a lot of checkpoints along the way, right? We have checkpoints in terms of complexity and size of board. We have checkpoints in terms of the physics that we can solve. We have checkpoints in terms of the ambition to be significantly better than humans that can come over time. 


---


#### 00:35:40.989

And with that kind of,   
(00:35:42.650) ~~you know,~~(00:35:42.851)  
those kinds of stairs ahead of you, you can treat each one as, okay, like now it's,   
(00:35:46.795) ~~you know,~~(00:35:46.974)  
you need to make this 20% better, 20% better, 20% better, 20% better. and let it compound over time. I don't see anything fundamentally about this problem that is unsolvable in any way. It's going to be hard, don't get me wrong. It's going to take a lot of people, it's going to take a lot of effort, but there's nothing about this that seems unsolvable in any way. When you hit that mature phase where we now have superhuman circuit board design, what does that look like to somebody like me? Can I just show up and say, hey, 


---


#### 00:36:17.364

I have, you know, I'm making a talking stuffed animal and you know, like how ignorant can I be and still get a board out? Cause it's like today to even specify what you want is sort of an expert problem. What do you see the sort of,   
(00:36:32.929) ~~know,~~ (00:36:33.050)  
independent entrepreneur tinkerer kind of person who like has a product in mind, knows literally nothing. Do they talk to a language model and work their way towards specifications and then put specifications into your system or what's that sort of future state round trip look like? Yeah, sure. So with us, like we're focused explicitly on layout, which is   
(00:36:53.775) ~~kind of~~(00:36:53.996)  
one of two problems, right? To give you an analogy to hang on to, think of creating a schematic for a circuit board as writing code. 


---


#### 00:37:02.413

Like a schematic literally looks like a block diagram with inputs, logic in the middle, and outputs. And it's entirely   
(00:37:08.775) ~~kind of~~(00:37:08.996)  
logical and abstract. You're just communicating to other engineers what the inputs, outputs, and functionality of the board will be. Layout is like compiling your code, right? How do you actually make something physical that takes that schematic or takes that code and actually makes the atoms of the world do that, right? So we're very specifically targeting the layout portion because we think a compiler should exist for electronics, and it just doesn't. The nice thing about that is that a lot of the benefits that we now have because compilers exist in software I think are going to happen and are going to answer your question in electronics, right? 


---


#### 00:37:42.306

So compilers eventually led to higher level languages, eventually led to things like Python, eventually led to large language models that allow you to write the Python and automate the whole thing. We will eventually move up that stack and look at schematic and how to make that piece easier. So you don't have to learn how to write C++, that you could learn how to write Python, or maybe even just deal with block diagrams and make a circuit board. Yeah, that's really interesting. Reminds me a lot of, we just did an episode on this tiny GPU project where a young guy set out to design his own GPU from scratch in two weeks and ended up taking him four, which was pretty remarkable. 


---


#### 00:38:18.291

And a big part of why that's possible, I mean, it's still quite an accomplishment in my view, but big part of why that's possible is that the sort of equivalent of the layout compiler does exist. And so he was able to   
(00:38:31.139) ~~kind of, you know,~~(00:38:31.739)  
get to that stage and be able to feed it into an existing system that could do that sort of gnarly work for them. But yeah, that's helpful. So Eric, how does this kind of compare and contrast?   
(00:38:42.043) ~~You know,~~(00:38:42.224)  
I   
(00:38:42.523) ~~kind of~~(00:38:42.704)  
can't help myself sometimes from going down the rabbit hole on techniques, but just zooming back out to the benchmark portfolio more broadly, what would you say here are kind of like the patterns that are common across the portfolio? 


---


#### 00:38:56.307

You know, what investments have you guys made that,   
(00:38:58.288) ~~you know, sort of~~(00:38:59.489)  
have a very different pattern in terms of what part of the market they're going after first,   
(00:39:03.949) ~~you know,~~(00:39:04.150)  
that are maybe in or not in this classically disruptive mode? And I guess broadly, how do I make money in AI? Yeah, that is the right question. Yeah, I'm very bullish because   
(00:39:16.195) ~~I think~~(00:39:16.474)  
the overall like we want to be in areas where there's lots of disruption and there's lots of disruption and lots of things changing, that creates the kind of primordial soup for there to be new big things created. So it's really valuable in that way, and we've seen that. And there's always a lot of crap that gets created and a bunch of stuff that doesn't work, but there are a bunch of good things that get created. 


---


#### 00:39:43.391

In the process, and it's all about finding them. I really loosely,   
(00:39:46.976) ~~I, you know,~~(00:39:47.257)  
I think   
(00:39:47.498) ~~there's, you kind of~~(00:39:48.440)  
have in AI right now,   
(00:39:49.862) ~~there's,~~ (00:39:50.081)  
it feels to me like there's three big categories of companies. There's a foundational model companies, right. That are   
(00:39:56.313) ~~like.~~ (00:39:56.512)  
They're building foundational models. They have some techniques around it. They have proprietary data. Maybe they have other things that they're using and they're trying to do something really special there. Then you have   
(00:40:07.998) ~~the,~~ (00:40:08.318)  
there's a set of   
(00:40:09.559) ~~like~~ (00:40:09.760)  
infrastructure-y companies,   
(00:40:11.742) ~~you know, in that,~~(00:40:12.663)  
in the next category. I'm on the board of Cerebris, which we invested in in 2016. That's an AI chip and systems company. That's focused on training, but you have Grok. 


---


#### 00:40:24.273

I'm also on the board of Fireworks, which is an inference provider. And there's a bunch of things where we're also investors. My partner Peter's on the board of Olama. And so there's just quite a few in that category too, which are their infrastructure, which is enabling some of the other stuff that's happening in the ecosystem. That's been a pretty fruitful area.   
(00:40:43.954) ~~I think~~(00:40:44.813)  
those companies have done well. They've gotten a revenue quickly and so forth. And then the third category are companies like Sergey's, like Quilter, which are vertical applications of AI. So they're applying AI to try to do something. And we see those. lawyers. We see them for doctors. We see them for accountants. 


---


#### 00:41:03.827

We obviously printed circuit board design. So there's just like a bunch of those things too. And each of those three categories, which is, it's very abstract and loose and they're all   
(00:41:14.141) ~~kind of~~(00:41:14.382)  
different.   
(00:41:15.182) ~~They all have~~(00:41:15.764)  
They have a set of really big opportunities and really big problems,   
(00:41:20.701) ~~I would say.~~(00:41:21.161)  
The foundational models are incredibly expensive to develop. They are extremely quickly depreciating.   
(00:41:29.063) ~~I said this before, I think~~(00:41:30.063)  
they're the fastest depreciating asset in the history of humankind, which is like you build one, you spend $150 million on it and Six months later, someone can build the same thing for $5 million. That's not historically a good way to make money with venture capital. That money tends to get incinerated and then someone has something alternative. 


---


#### 00:41:55.777

And we'll see. I could be totally wrong on that. Maybe someone will build something that defeats it. But the general purpose models have proven to be really expensive and depreciate very quickly. What is cutting edge? The infrastructure companies have done pretty well in a bunch of ways. They have real business opportunity. They're enabling a bunch of things. The question always exists with them, which is, do those problems exist for very long? To some degree, a lot of AI development is where software development was circa,   
(00:42:28.088) ~~I don't know,~~(00:42:29.150)  
2002, in terms of the tool sets available and the abstractions that people are working with. Some of the things that people are solving just   
(00:42:38.112) ~~I'm~~ (00:42:38.213)  
just not sure that they're going to be around for a long time. 


---


#### 00:42:41.335

And so that's a potential real challenge there. But there's what do you have in mind there? Are you talking like, LLM observability type? Yeah, that's a great example. That's a great example, which is just   
(00:42:53.619) ~~like,~~ (00:42:53.820)  
is the LLM observability thing a thing?   
(00:42:56.342) ~~Like,~~ (00:42:56.523)  
it's a thing today. I don't know if it's a thing long term,   
(00:42:59.586) ~~like~~ (00:42:59.726)  
maybe not, we have to   
(00:43:00.507) ~~kind of~~(00:43:00.748)  
think through it. But   
(00:43:01.909) ~~that's,~~ (00:43:02.170)  
that's a pretty challenging, that could be a potentially challenging area. That would be one that we think about a lot. And then the vertical stuff has proven to have, in some way, the fastest revenue traction. Some of the revenue scale of the vertical companies has been insane. 


---


#### 00:43:20.706

But the kind of common criticisms of are there any moats or barriers to entry? If you can build a company very quickly in three months or six months and get something out to people- Weekend hackathon for that matter. Yeah, weekend hackathon. Then that also means the 10 other competitors are going to do that. And do you end up with something durable there or not? And   
(00:43:43.833) ~~I think~~(00:43:44.052)  
we just don't know in a bunch of cases. You have to have a theory of it. In the case of looking at Quilter or Benchmark's investment in Sierra or some of these others, I would say we have a view, a belief that there's something durable there that will be built and compound over time, even though they got quick traction. 


---


#### 00:44:05.945

And so I think that's just something that we have to look at and there's a lot of value. But I think there's, this is what's cool about what's happening right now is there's   
(00:44:13.070) ~~like~~ (00:44:13.230)  
lots of traction. There's lots of really interesting ideas in all of these categories and obviously amazing people working on them, but we got to figure it out. And so that's   
(00:44:25.778) ~~kind of~~(00:44:25.958)  
how I've been thinking about it.   
(00:44:27.719) ~~You know,~~(00:44:27.880)  
I'd also say there's this other thing that's really interesting to me where A lot of the AI work has happened with researchers. Like you hear it all the time. This is a researcher, they're PhDs. They're doing that. And who's telling you this? 


---


#### 00:44:43.070

I forget one entrepreneur was telling me this was like,   
(00:44:44.871) ~~you know,~~(00:44:45.090)  
you get this. So the researchers are writing something. It works. It   
(00:44:48.052) ~~kind of~~(00:44:48.293)  
works in a research context, which is a proof of context, proof of concept or experiment. And then they take that code and they try to scale it in production. And it's holy shit. That's not good. That doesn't work.   
(00:44:59.619) ~~It doesn't,~~(00:44:59.960)  
it's not written for that or whatever. And this entrepreneur said,   
(00:45:03.684) ~~she's,~~ (00:45:04.106)  
I have a rule when it comes to code written by researchers. And   
(00:45:08.773) ~~I think~~(00:45:08.974)  
she said,   
(00:45:09.333) ~~she was just like,~~(00:45:09.894)  
it's just RM star. And   
(00:45:12.963) ~~it was like,~~(00:45:13.563)  
it was such a classic,   
(00:45:16.244) ~~you know, it's just, but it was,~~(00:45:18.646)  
but there's this   
(00:45:19.686) ~~bridge and~~(00:45:20.286)  
divide, which is quite from between research and proving something out conceptually and actually   
(00:45:27.030) ~~like~~ (00:45:27.210)  
turning that into shipping product that can scale and work and be iterated on. 


---


#### 00:45:32.733

And,   
(00:45:33.534) ~~you know,~~(00:45:33.813)  
that's a divide that just didn't exist in software development, at least in my, adult lifetime. Maybe it existed in software development back in databases in the 70s and 80s, but I don't know enough if it did or not. That's when I say   
(00:45:52.244) ~~that~~ (00:45:52.623)  
the stack maturity, the kind of stuff that people have to do to work with PyTorch today or work with CUDA today or something like that, that's just not something that software developers have had to deal with for at least 20 years. Yeah, that reminds me of comments I heard Demis Ossavas make about why they have taken this step now of merging DeepMind into Google proper after so many years of   
(00:46:17.612) ~~kind of~~(00:46:17.813)  
holding it out as its own thing. 


---


#### 00:46:19.494

He basically just said, we're now at the point where we're not done with research, but certainly a lot of the research has been done. And now it's like becoming the bridge to engineering. That is a huge challenge. And that's where they feel like the time is right. We're like, we do want to continue to do novel research and push the limits of it. But as we try to bring this stuff into real applications to benefit humanity, we have to engineer it.   
(00:46:46.878) ~~And,~~ (00:46:47.059)  
and that's a, That's its own thing   
(00:46:49.530) ~~and it shouldn't be.~~(00:46:50.291)  
It's not so simple, it turns out. I know we're just about out of time with you guys today. Do you have any kind of call for startups? 


---


#### 00:46:58.496

Anything that you wish somebody had brought you that you haven't seen or haven't been able to find yet?   
(00:47:04.159) ~~You know,~~(00:47:04.460)  
I have this thing that if a venture capitalist has the idea, with very few exceptions, like maybe Mike Spicer or someone else like that can pull it off, But if the venture capitalist has an idea,   
(00:47:17.023) ~~that's a bad,~~(00:47:18.625)  
that's a bad situation because this is not what we're to the idea maze point where we started. That is not, that is not our job, nor is the thing that we are generally good at. Look, I would say I continue to be really excited.   
(00:47:35.516) ~~I think~~(00:47:35.757)  
we have,   
(00:47:36.876) ~~you know,~~(00:47:37.117)  
a ton of companies across the board   
(00:47:38.797) ~~in,~~ (00:47:38.838)  
at least in terms of the infrastructure companies and the vertical applications that are super interesting, would love to meet amazing people who have been working on ideas or thinking about something for a long period of time and are like obsessed with it. 


---



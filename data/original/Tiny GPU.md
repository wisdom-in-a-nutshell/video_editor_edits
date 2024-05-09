# Tiny GPU


## Introduction to Adam Majmoudar and the TinyGPU Project

~~Take or anything like that, you know, any, um, interruptions that happen or, you know, costs or whatever, that's all fine. We'll take that stuff out. Um, we also will offer, this is typically more for like commercial, uh, you know, folks from what DeepMind or whatever, uh, but we will offer if you want, you can take a review of our edit before we publish, and then you could request any, you know, additional edits or if you find anything to be an issue there.~~

~~Um, most people don't take us up on that because it does take time to review things. Um, but you're welcome to, if you want to, totally up to you. It's an offer, but not an obligation. Yeah, that makes sense. That's cool. Any other questions for me before we dive in? Where do they get uploaded? We publish to primarily it's audio only, but we do publish to YouTube.~~

~~So we can use visuals. We just kind of need to be mindful to explain what we're looking at a little bit as we go. Um, and then if it gets really intense, you know, whatever, we can just tell people that they should open up the YouTube to see stuff. Yeah, we can also link to your GitHub project and Twitter thread in the show notes so people have those readily available too.~~

~~Yeah, it makes sense. Cool. Good question. Um, let me just pronounce it one more time and make sure I'm getting it right. Adam Majmoudar. Yep. Perfect. Alrighty. Cool. ~~[00:00:00] Adam Majmoudar, creator of the TinyGPU project. Welcome to the Cognitive Revolution. Thank you for having me. I'm excited about this. So you've created this project that really caught my eye called tiny GPU in which you describe yourself as having no prior experience creating GPUs, but nevertheless set out to speed run creating one from scratch in just a few weeks.

And,~~ uh,~~ I imagine you have learned an unbelievable amount from doing that. I've learned quite a bit just from following your progress and hopefully the audience will be able to learn a lot from,~~ uh,~~ following the results of what you did as well. 


## Adam's Journey into GPU Development

You want to start off by just ~~kind of ~~introducing yourself a little bit and telling us how you got this crazy idea.

Yeah, sure. ~~So, uh, ~~I'm Adam. ~~Um, ~~I've been working on a copy called third one for ~~kind of~~ the past three years, started in college and worked on it full time during college. ~~Um, ~~and then worked on that for a couple of years in gap year. And I just stopped working on that recently. ~~Um, ~~and then now I've been doing a couple of deep dives, which I've been sharing on Twitter on a [00:01:00] bunch of different industries that are ~~kind of ~~the overlap between what I think are going to be defining technologies for the next one to two decades.

And areas that I've had demonstrated interest in for my whole life. And ~~kind of ~~my goal has been how fast can you get to a point of technical competence and industry competence? So it kind of two sides to it. It's not just like the technical side of things. It's actually like understanding the industry and how things are going right now, understanding tailwinds and also understanding the opportunity landscape.

Specifically for young people,~~ um,~~ but TinyGPU happens to be the result of the technical part of that, which is I just finished my deep dive on chips. I'm now planning to use other ones, but during that deep dive, my goal was basically learn the entire engineering stack of chips and computation and history of it.

And part of that process was ~~the ~~basically 2, 2 week sprints. The first 2 week sprint was, can I learn how to make a chip ~~from~~ all the way from EDA, which is ~~like~~ the electronic design side, and then understand how fabrication works and understand the architectural side all in 2 weeks. Which is traditionally something that people can spend,~~ like,~~ two, two plus years in college to [00:02:00] do.

~~Um, ~~and my belief was~~ like, it's,~~ basically you can cut it down to ~~like ~~100x time wise. Of course you're not going to be learning the same thoroughness as what other people are doing. But, the question you ask yourself is, Is the thing that matters the thoroughness and the quantity of stuff that you learn?

~~Like, ~~of course, people who spent three years on this know way more than me about lots of different detailed stuff. Or is it that there's some, not really 80, 20, it's more like a 99 one where it's like 1 percent of the stuff is actually most of the ~~important, ~~important value. And if you can figure out how to extract that quickly,~~ um,~~ then you get much more value out of the learning.

So that was ~~kind of ~~the context behind the project. ~~Um, ~~and so I did the two weeks, spent that time learning how to make chips. And then by the end of that, I ~~kind of ~~formed this intuition, which is like, okay, now that I know this, what's a really cool project I can build that will teach me a lot. It will also be fun.

It also has potential to be interesting and valuable to people. And given ~~kind of~~ the whole wave of stuff around AI, ~~and, you know, ~~you have GPUs and tensor processing units and all kinds of AI accelerators,~~ um,~~ and also just a whole loop in around ASICs, I thought it would be interesting [00:03:00] to add that into the GPU as a foundational way to learn all of that.

So that's cool. I got it. Love it. Well, let's get into it. ~~Um, I think~~ 


## Challenges and Learning Resources in GPU Design

one of the challenges that you noted right up front that I hadn't really considered but definitely makes a lot of sense is that there aren't a ton of great learning resources out there for things like this because a lot of the technology is proprietary.

That includes ~~like~~ designs. I've done some of my own prep in realizing that. ~~You know, ~~like NVIDIA has not published every layer of their technology stack. And so ~~there's, ~~there's ~~kind of ~~questions even to this day, ~~as I understand it,~~ about ~~like~~ how some of the most advanced GPUs work in some critical ways.

And ~~I imagine ~~also~~ like ~~design tools, the software packages,~~ um,~~ that those are not always super easy to come by either. So maybe for starters,~~ like~~ just characterize that landscape a little bit and tell us what ~~sort of. You know, ~~learning resources and software tools you were able to avail yourself of. So I'll contrast this to CPUs, which is a much broader landscape, and there's a lot more learning resources.

And the reason is probably just as a function of how old it [00:04:00] is. ~~Like~~ the CPU is basically the oldest invention in terms of actual, ~~like~~ useful computing. Lots of people will disagree with that statement, but take ~~the, uh,~~ the core concept out of it. And,~~ um,~~ Because of that, there's so many learning resources.

~~Like ~~if you take an architecture course in college, you'll learn how to build a CQ. ~~Um, ~~there's basically tons of courses around it. And what it means to have it fully documented and taught is not just how it works at a high level. ~~Like, ~~oh, here's the different parts. There's ~~like~~ the data memory and program memory.

I registers, it's actually like getting into the control signals in the low level and understanding how machine language translates into stuff happening, the CPU and stuff like that. So it's like the connection between the software and the hardware level. And that's really what it takes to be able to completely replicate it.

~~Like, ~~if you want to build a CPU from scratch, at the end of the day, you need to understand how you can actually program it and how you can turn that into low level signals in your design. And so in contrast with GPUs, there's essentially nothing at that level. So what you'll find is if you go look for,~~ um,~~ NVIDIA and AMD GPU designs,~~ you'll,~~ you'll see ~~like~~ high level architecture and we'll show you [00:05:00] all the different pieces of that.

~~Um, ~~and of course it's a little bit ridiculous to even expect something at the control signal level for designs that large,~~ um,~~ but actually there's no resources that dumb these things down into the simple elements that you can at least try to implement something yourself. ~~Um, ~~now one person pointed out that.

Intel,~~ which I did not look into~~ actually does have,~~ um,~~ pretty low level diagrams. Again, you wouldn't really use it for learning because it's ~~like~~ an actual production GPU. So it's not really too easy to understand. ~~Um, ~~and that could be one interesting approach for people. Gotcha. Okay. What about on the ~~sort of~~ tool side?


## Navigating the Landscape of GPU and Chip Design

I assume you were not able to use all the same software platforms that folks. Add in video or at AMD, maybe more at AMD. Cause I believe there's stacks in a more open source, but,~~ um,~~ what were you able to use to actually create these things? Yeah, so~~ I expect my stack is, I mean, ~~certainly my stack is completely different from ~~all the, ~~all the real players.

So the thing is, in this space, the EDA tooling, like the Electronic Design Automation, which is what you use to actually,~~ um,~~ convert your,~~ like,~~ architectural designs into an actual ship layout,~~ um,~~ and also do a lot of stuff optimizing your design, which is basically the entire [00:06:00] complexity of the process. ~~Um, ~~those things cost like hundreds of thousands of millions to millions of dollars.

Like per seat and per company and so an individual can basically never actually use those things and in terms of shipping an actual production quality layout and basically need those like they have a complete mode on this industry. ~~Um, ~~the next thing, though, is there is this project funded by data within the past, ~~I would say,~~ 5 to 10 years.

I'm not sure the exact number. I'm called open road, and it's an attempt at making an open source software. ~~Um, ~~it's obviously way worse than those real production ones in many ways. It's not feature complete, but for simple cases, like what any individual would do, or even small businesses would do,~~ um,~~ it's completely sufficient.

And then ~~the other piece, like,~~ the last piece that made all this possible is that again, in the past decade,~~ um,~~ there's this company called Skywater. And this open source EDA stat for their own process node, which means that they have their own,~~ um,~~ foundry that produces chips at the 1 30 nanometer scale, which is just like the size of the gates and the transistors they make.

And they opened it with this [00:07:00] thing called fabulous. Where multiple people can basically pay ~~like~~ a much smaller amount to get like a hundred chips ~~on this, uh,~~ on this process. And that costs like 10 K. And this other group called tiny tape out ~~kind of ~~advertise the cost. So they'll be like, okay, 100 people can now pay for a tiny slot and we'll put like a hundred projects on each of these chips.

And so because of this. ~~Kind of ~~incremental cheapening of everything, it now becomes possible for someone like me or others to use that,~~ um,~~ basically the SkyWater process node to make a chip. And then you use the,~~ uh,~~ something built on the OpenRoad stack called OpenLane. It's basically just OpenRoad specifically for that SkyWater stack.

~~Um. ~~And now all that's open source, obviously there's some like synopsis of cadence, which are the real production tools,~~ um,~~ but completely functional for what I would want to do or like any individual hobbyist. Cool. So ~~do I,~~ we'll maybe get back to the sort of hypothetical manufacturing side,~~ uh,~~ toward the end, once we get through all the design considerations, but do I have it right that at the end of this.

You have, ~~you know, sort of ~~a [00:08:00] micro, a tiny, I should say GPU that could be included alongside like a hundred other projects on one chip. And then that chip would be what you would actually get if you ordered through the process you described would be like a chip that has your design plus a hundred other designs all on it.

And then everybody just ~~kind of ~~shares in the production costs, but also ~~like, I guess, ~~gets access to one another's designs. Is that how that's working? And I'm probably actually going to do that. So the thing that I mentioned called tiny tape dot created by this guy named Nathie Gunn, he's basically like a goat of making ASIC accessible nowadays.

~~Um, ~~you can find him on Twitter and you can find his course, which is ~~tiny tape dot, um, or sorry,~~ zero to ASIC. He has basically made this process where they'll buy up one of those fabulous 10, 000 slots where you have to get a hundred tips, you have to pay 10, 000. And as I said, they'll allow a hundred people or~~ a couple,~~ a big group of people to submit their projects.

And ~~so, ~~for example, yeah, exactly what you said is I could submit this to that, ~~which I, ~~which I will do. And then I'll get the chip and the cool thing is I'll get the chip and I'll be able to play with my project, [00:09:00] but I'll also be able to play with the projects of all other 99 people who submitted. Which is ~~kind of ~~just like a cool byproduct of it.

That's awesome. Other than for learning, what is this good for? ~~Like, ~~are there projects that people are actually where they're building, ~~you know, ~~things where ~~they, ~~they can't get something that meets their requirements that they can only get this way. Or is this really all ~~sort of ~~for the love of the game ~~and, ~~and,~~ uh, you know, ~~the fun of the DIY and you're just now with these stacks opening and the tool of becoming better,~~ um,~~ it might be like an interesting.

And a lot of the market or a smaller scale ASIC market,~~ um,~~ where at least you could do the initial prototyping phase with the stack. ~~Um, ~~I think in practice, there's not going to be ~~like~~ huge businesses built on the server. Like the guy that it will always make sense for them to go to ~~like the real, ~~the real production stacks.

~~Um, ~~so I do think it's mostly hobbyists and I think the most interesting thing on the learning side is getting more college students and younger people just getting the intuition of this since the industry was ~~kind of ~~created and the engineering was much more so popular ~~like~~ several decades ago.

Getting a new generation to it is interesting given that there is a whole landscape of the [00:10:00] Chips Act and there's some geopolitical incentives there. Cool. Makes sense. Okay. 


## Deep Dive into the TinyGPU Project's Goals and Scope

So let's get into the project itself. One thing I wanted to just try to do up front is ~~kind of ~~figure out the scope. ~~You know, ~~when you say ~~like ~~designing a GPU ~~from scratch, from scratch, ~~from scratch, there's like a lot of layers, ~~right.~~

To the tech stack. ~~So, um, ~~obviously you're not going all the way down to ~~like ~~mining your own minerals,~~ um,~~ So ~~where,~~ what was like the foundation that you said, okay, like this is deep enough down the tech stack, but I'll count it as from scratch, but I'll still be able to use this kind of foundation to build a pot.

Yeah, that's the pressure. So there's a couple of things. First of all,~~ um,~~ obviously I'm not like building ~~the, ~~the whole EDA pipeline from scratch or anything like that. So the place where it really starts, it's their log, which is where most designs start,~~ um,~~ which is that. Basically called your register transfer level logic is just designing the specific memory and the specific wires that connect up the chip to make all the logic.

And so designing something at that layer is the layer that I was targeting. And then also more specifically, because that's very generic,~~ um,~~ the architecture that I wanted [00:11:00] to choose is obviously very nitpickable in the sense that,~~ like,~~ okay, you have a giant GPU, there's like millions, thousands of features to this GPU.

~~Like, ~~the question is, what are you going to include? Because the word GPU is.~~ Kind of ~~an amorphous term nowadays, like it started out being referring to graphics processors. Now, people are still using it for lots of stuff that aren't graphics processors, like transfer processors and other accelerators. ~~Um, ~~and so there's ~~kind of ~~a blurry line in terms of what GPU counts as.

And so because of that, I ~~kind of ~~set my goal of what do I want to focus on with this, not as like graphics hardware or any of the specific things like that, but more ~~like ~~if you want to understand this kind of giant blob of areas that spawned from GPUs,~~ um,~~ what are the core concepts you need to understand in order to be able to build on top of them and understand the little details.

And then my goal is, can I create a foundation where using this foundation, you'll be able to learn all of the important stuff. And by choosing that, it allows me to strip away a lot of the complexities of some of the nuances of any little engineering decision. If you're choosing to make like graphics [00:12:00] hardware or ~~like~~ any of the other specific things.

And just focus on that. If I'm not, we got it. So ~~I mean, ~~some people would disagree, right? ~~Like, ~~because it's a blurred line, some people would be like, Oh, that's not a GPU. It doesn't include graphics or whatever. There's like Netflix you can make everywhere. But at the end of the day, it's just a design decision from the purpose of the product, which is like, how can you teach people how this stuff works most effectively?

Yeah, it makes sense to me. ~~Um, ~~and no doubt, ~~you know, ~~these are super complicated. It's often said these days that chip making is the most complicated. Industry in the world and arguably the most complicated thing that humans have ever devised to manufacture at scale. So yeah, not surprising that you'd have to,~~ uh,~~ make some simplifying assumptions to pursue a project like this.


## Exploring the Core Concepts of GPU Design

What are the things that you mentioned in your. Twitter thread that originally caught my attention was that the beginning of the exercise was a real challenge in just prioritization, figuring out,~~ like,~~ what really matters most, you came up with three things that [00:13:00] you felt mattered the most. ~~Um, ~~we can get into each one in turn, but you want to just ~~kind of ~~give a high level of ~~like, ~~what those three things are and, ~~you know, ~~how you identified them.

Maybe a little bit on, ~~you know, ~~what you decided to leave out, and then we can go deeper into each of the three. Yeah, so the three things I chose are architecture, parallelization, and memory. ~~Um, ~~and granted,~~ like,~~ that whole Twitter thread, all those were written,~~ like,~~ chronologically. I'm not sure if you'll link to it or not, but It's actually,~~ like,~~ the result of hindsight and so, like, all of ~~the, ~~the architecture design I chose, for example, or,~~ like,~~ the design decisions that I put up front are actually the result of me having gone through the entire process.

I didn't have that ~~like, ~~I didn't have that foresight at the beginning. ~~Um, ~~but the reason I chose those things is because. And ~~I think~~ even maybe ~~I would, ~~I would ~~kind of ~~rephrase them into two really like architecture is not really saying much. ~~I mean, ~~when I met by focusing on architecture, it's like, what are the key elements is each piece of the GPU that are ~~kind of ~~important to all GPUs, like different GPUs have different little specific elements tailored to their need.

But what are the things again, going back to the foundations that you absolutely need to understand these [00:14:00] concepts. In order to understand how this,~~ like,~~ the whole thing works, broadly speaking,~~ um,~~ and so I ~~kind of ~~broke that down over time. Now, I had the architecture diagram ~~in my, ~~in my tweet, and ~~that was kind of, I think~~ that was a good breakdown of basically the most simple possible explanation of how GPUs work.

~~Um, ~~and we can get into the specifics of that. Now, ~~I think~~ the other 2 terms were actually ~~the more interesting, ~~the more interesting parts. ~~Um, ~~so I'll start with parallelization, because that's the one that ~~I think~~ is the ~~most interesting. ~~Most obvious on the surface level, and that's ~~like, ~~yeah, GPUs obviously are built to do parallel computation.

~~Like, ~~that's their whole utility, basically in graphics hardware, or just graphics use cases in general, and machine learning,~~ um,~~ they benefit a lot from doing matrix map, and matrix map happens to be element wise. In other words,~~ like,~~ computations on individual elements don't depend on other elements, which means you can do them all at once.

And that's ~~kind of ~~the whole reason why GPUs are useful. ~~And~~ so the whole point of GPUs is instead of a CPU where,~~ um,~~ generally things are thought of as being executed sequentially, in practice, this isn't exactly true, but,~~ um,~~ like generally you would execute L at one, then two, then three, then four, and now you've done this whole thing four clock cycles or four [00:15:00] cycles of computation.

Instead of the GPU, you just distributed out ~~a bunch of, like,~~ among a bunch of compute resources. And now you're,~~ um,~~ you're accomplishing this all in a much faster time period. Now, the interesting thing about parallelization,~~ um,~~ on the surface, it seems like it's just ~~like, ~~Oh, you need to have a bunch of compute resources or like compute cores, and then you can distribute these workloads across the ~~compute, ~~compute cores.

~~That's~~ actually, it turns out,~~ um,~~ a lot more trivial than some of the other difficulties. So there's ~~like ~~one, the problem of how do you distribute these workloads,~~ um,~~ effectively? With your resources and ~~like ~~manage the resource utilization effectively to maximize it. So that's a cool and interesting problem that happens on like the hardware level.

~~Um, ~~And then there's also,~~ I think,~~ maybe a more interesting thing, which is what is the software pattern of parallelization as in, how do you actually program these things? ~~Like, ~~it's one thing to make the hardware support this capability,~~ um,~~ but how do you actually make the software easy to use for developers who aren't usually used to it?

And that's ~~kind of ~~arguably one of the core problems that NVIDIA solved and what made them win. ~~Kind of ~~a consensus takeout, but~~ like~~ their CUDA software design are so good for parallel programming,~~ um,~~ probably by nature of how [00:16:00] similar and.~~ Like~~ integratable it was into the previous stack that these developers who needed to use it were used to, which is C.

~~Um, ~~and so another interesting element to highlight there is since the program side is so important, how does the programming pattern that people are so familiar with actually get implemented in the hardware? ~~And~~ so that was an interesting element of parallelization. ~~Um, ~~so ~~I guess~~ just to break that down again, it was the 2 interesting things in parallelization were resource management and resource utilization and then software pattern to hardware.

How does that get implemented? And specifically, the software pattern is called same instruction, multiple data. And that just means that you're executing the same code on multiple pieces of data, like elements of the matrix and hardware. It's called same instruction, multiple thread. ~~Um, ~~Which is ~~kind of ~~just like the hardware manifestation of that and then the last thing, which is, ~~I think,~~ the less obvious and more interesting, maybe most interesting realization for me.

And maybe it's more obvious than you're actually doing the program to GPU programmers, because it's actually like a 1st party thing in Gouda, for example,~~ um,~~ but memory management is really interesting [00:17:00] to me. And the reason is because I ~~kind of ~~had a completely Yeah. Wrong notion of memory management, gps.

In fact, I didn't even realize how important it was initially. And this is the thing I was saying in my tweet, ~~like~~ where George Hos ~~kind of ~~told me,~~ I,~~ I like randomly ran it to him and I was like, Hey, can you gimme feedback on my design? He was like, dude,~~ this, this doesn't, ~~this doesn't like accomplish the whole memory, manage the problem, which is like the most important thing.

And what that is is. It would see initially,~~ um,~~ that ~~when you're, ~~when you're thinking about parallelization, the bottleneck on how much you can parallelize computation is how much compute resources you have. In other words,~~ like,~~ let's say I want to do ~~like a hundred L, like~~ a hundred matrix additions at a time.

That means I need a hundred different cores that support addition. ~~Right. ~~And it seems like that's the bottleneck in practice. It's actually not at all. In practice, it's actually memory because in order to do a hundred Yes, you need 100 compute units, but you also need to be able to read from 100 different memory locations at once from the global memory.

And global memory is bottlenecked on how much bandwidth it has. And that [00:18:00] bottleneck tends to be the limit,~~ um,~~ because there's a pretty big latency in terms of ~~like. ~~Distribute unit wants to access memory, then it needs to ~~like ~~send the request, and then it needs to wait for it, and ~~like ~~if all of these units are trying to access memory at the same time, you may actually have more requests for memory than you have bandwidth in global memory, which means that you need to actually manage all these requests in memory.

~~Um, ~~and that comes with ~~like ~~a huge latency. And ~~so, ~~to ~~like ~~rip a quote directly from what Jory Todd sent to me, he said that GPUs is largely ~~kind of ~~the task of trying to work around memory latencies and ~~kind of ~~hide them away at different layers. ~~Um, ~~And that's ~~kind of ~~a lot of what the challenge of GPUs really is about, which is why,~~ like ~~architecturally, they've had all these things to solve that, like memory and vulnerabilities are ~~kind of ~~standard, and then they also have multiple layers of caches to prevent having to access global memory and ~~like ~~shared memory and all kinds of other stuff.

So the memory pattern is another very important part of GPUs. Okay, cool. That's a great. Where do you think it makes the most sense to start? In terms of, ~~you know, kind of ~~spiking down each of these three,~~ I,~~ I [00:19:00] originally had architecture first, but based on your description there, I might go parallelization first and then,~~ uh, kind of ~~come back to architecture.

But what do you think makes the most sense?~~ I think~~ it actually might be easiest if we go in reverse order, because people are probably most familiar with software, right? So you could actually start with ~~Kind of~~ the ~~software, ~~software side of things, the ISA software side, and that'll work backwards into ~~like~~ how this is actually implemented in the hardware.

You think that makes sense? Sure. I'll have to follow your lead. ~~Um, ~~in defined terms for us, ISA is instruction set architecture. Exactly. ~~Right. ~~Yeah. Yeah. And so I was confident about instruction set. I didn't know the a actually there ~~because I, Um,~~ so this part might be a bit challenging to do without video.

Like I think almost all of this art ~~is, ~~is going to be near impossible to do without video, so that's the caveat. But,~~ um,~~ like ~~I think it's basically,~~ it's going to be really challenging~~ to. ~~To talk about ~~like~~ different instructions and ~~like~~ the actual code and stuff like that, which I think is ~~kind of ~~important to understand it.

~~Um, ~~let's do this. I'll share my screen. I've got these [00:20:00] notes up and I can, I'm right on your GitHub page.

So

~~interestingly shaped. Um, ~~yeah, there we go. ~~So I'm looking for,~~ okay, cool. ~~So. ~~Let's just try to, ~~you know, ~~describe it, talk people through it. ~~And then, you know, ~~if you want to,~~ uh,~~ get a clearer view of this, ~~then~~ we'll have the video on the YouTube version. ~~Um, but most, most folks by default will be listening just to the audio.~~

~~So let's try to talk them through it and, you know, uh, send them to the. The YouTube thingy. ~~Yeah. So~~ in that case,~~ let's scroll down to the kernels for a step.

Yeah, perfect. We can do matrix edition. ~~Yeah. ~~So if you just scroll up a bit, ~~we really only need the top of the file plus the isolation. ~~Yeah, that's perfect. ~~Yeah.~~ Okay. 


## Understanding GPU Software Patterns and Instruction Sets

So ~~I think~~ the best way to start with understanding this whole system is by understanding the software pattern, just because that's generally ~~most familiar with, like~~ most familiar to people, easiest to see the layout of what's happening.

~~Um, ~~and so generally the way you think about. GPU software is ~~right. ~~It's the Cindy pattern, which is same instruction, multiple data, ~~as I mentioned before.~~ And so all that means is you're just going to write one instruction. You're not going to do any loops or anything to be like, okay, execute this instruction on all of this different data.

You're just going to do an instruction. That's basically invariant to the data that it receives. And what that means is, your code is going to take in some data, it doesn't know what the data is, [00:21:00] and based on that data from, let's say, two different,~~ um,~~ matrices, it's going to perform a computation on the data to get the element of the resulting matrix, and it's going to put that back in memory.

~~So, ~~to take a concrete example of this, we can say,~~ like,~~ matrix addition, which is probably one of the most simple GPU use cases, ~~right?~~ So let's say we have,~~ like,~~ two 1 by 8 matrices,~~ uh,~~ which means each matrix has 8 elements, right? And let's call it matrix A and B. And all we want to do is quickly compute the addition of these matrices, which we'll call matrix C.

So let's say that,~~ um,~~ Matrix A and B are loaded into memory in elements 0 to 7 for matrix A. And then 8 to, what is that, 13,~~ uh,~~ 8 to 15 in,~~ uh,~~ for matrix B, and we just want to put matrix C, the result of this addition, into ~~like 16 plus, like ~~element 16 plus of memory. And ~~so, ~~one thing you could do in a CPU is write a program, and that program is going to take, like in a for loop, it's going to be like, okay, 4i less than 8, as in like ~~for each, ~~for each of the 8 elements, add up the element for matrix A and B, put that into the element in matrix C, And we're going to do that.

That's going to take eight [00:22:00] cycles,~~ right? Um, ~~like eight iterations of the for loop. And so that's one way to do that sequentially. Now, alternatively, what you could instead do is write this thing called a kernel, which is a GPU program. And this kernel is just going to handle adding up one pair of elements in the MB and putting it into one slot in HFC.

And so we'll say ~~like, ~~this kernel is going to take the i th element of matrix A and B, hide them up, and then put it into the i th element of matrix C. And so the actual code for that is pretty simple, I'm sure everyone can imagine what that's like. So you're going to basically ~~read, uh,~~ read some global memory.

The base address of a plus the item, which is just like getting the element from a, you're going to take the base address of B, get the item element, read it out of, add an opt and then put it into C. So actually the program itself is very straightforward and there's not really any GPU element right there.

So the main thing with the GPU is you just want to tell it ~~how many, ~~how many times do you want to execute ~~this, ~~this instruction? And on how many different values of I do an execute on. So in this case, ~~we want, ~~we want this to be from the [00:23:00] 0th to the 7th element of each matrix, there's an 8th element. So we want 8 different values of I.

~~Um, ~~and that means that, and that's just because we want to add up the 8 different elements of the matrix. And ~~so, ~~we're going to call each of those times, where we need a separate execution of this code, that's going to be called a thread. And a thread is just executing the same code again on multiple different parts of the matrix.

And ~~so, ~~for this code, all we have to do is specify what each thread is going to do, which is basically just read to address something. I'm not going to write an address and there is a run eight of them. And the question is, when you run eight of these threads, ~~like ~~let's say we now have eight of these exact same pieces of code running in our GPU, we'll just say somehow we've accomplished that.

The question is, how do you actually get each of these threads to do something slightly different, ~~right?~~ They're all running the same instruction, but you actually ~~need, ~~need them to be able to perform it on separate data, like the different elements matrix. And so what you need to do is. It's somehow in the actual hardware of the GPU.

You need to make each little area that's executing one of [00:24:00] these ~~kernel, ~~kernel codes, you need each little area to know something about which thread it's executing. ~~Like, ~~is it executing the 0th executing the 2nd thread, or whatever. And if you have a way to do that, then within that hardware, you can, the hardware can know something about its own context.

So let's say the hardware knows which thread it's executing. Now the hardware can say, Hey, there's this instruction here that's supposed to load some data in from memory.~~ Well, ~~the data that I want to load in is actually based on which thread is being executed here. So if I'm currently executing thread number 0, I want to load in the 0th element of A and the 0th element of B.

If I'm trying to execute thread number one, I'm bringing the first element of each, blah, blah, blah, and I want to store it in the first element of C. And so that is the most important thing here. ~~Um, ~~so ~~the, kind of ~~the two important things are, one,~~ we're,~~ we're writing some code that just is left to be executed by a single thread.

And then we're going to specify how many threads you executed. ~~Uh, ~~the second important thing here. Is the special values which are going to be local in the hardware. So each time a thread is getting executed in the hardware, they have some broader context [00:25:00] about what's going on here. And so if you look at those,~~ uh,~~ for people looking at C,~~ um,~~ There's these values called block index, block dimension, and thread index.

~~Um, ~~and this will probably be familiar to people who are familiar with CUDA. ~~Um, ~~obviously there's more complexity in the actual pattern. ~~Um, ~~but basically the way this works is that when you have tons of threads that need to be executed for something, you're going to group these threads, Into that is basically executed ~~together ~~together on a single compute unit, and those batches are called blocks.

And so let's say,~~ like,~~ our block size is 4, which is what it is on my current GPU design. That means that batches of 4 threads are going to be executed together. And so whenever these things are executed, basically, what you want to know is. Which block number is currently being executed. And then within that block number, what is the thread index in that block number?

So that means that the threads are each going to have an index from zero to three for each block, because there's four, four threads per block. And then let's say we have ~~like, I don't know,~~ 10 blocks being executed. So now if we're on block three. How do we get the correct thread [00:26:00] that's being executed?

~~Well, ~~very simply, we're just going to multiply the block ID three by the number of threads per block. So now that's like 12. So that means that there's 12 threads that have already been executed in the previous three blocks. ~~Um, ~~and then we're just going to add the thread ID. So ~~now it's like, okay,~~ now we know we're on the thread number 12, 13, 14, 15.

And now those threads can pull in the rest of the data they need to commemorate. And so that is how the STEMD architecture, like programming pattern is implemented in programming. And then we'll talk about,~~ like,~~ soon, how that's implemented in the hardware and it's very simple. And that's ~~kind of ~~the core understanding.

You need to know,~~ um,~~ some kind of what's the kernel programming pattern. And in terms of this as an asterisk, like, how did I decide what instructions to include in my ISA? It's as you can see, like I'm trying to make it as minimal as possible. And so really ~~my, ~~my decision function there was basically~~ like,~~ what are the minimal set of things ~~I can, ~~I can implement in order to make some cool useful use cases and so ~~like~~ matrix addition, matrix multiplication, with the most obvious.

Things there, and so the [00:27:00] instructions I chose are basically just what's actually needed to support those, which is just basically some basic record take loading and storing data from memory, because that's how you basically get your inputs and then store the result of your computation. ~~Um, ~~and it costs since just for some convenience, but yes,

cool. Well,~~ I think~~ that was all quite well said, so ~~I'm not sure how much I can really add to it, but~~ just to try to summarize quickly back ~~the. Yeah. When you look at this block of code,~~ I'll go back to the block of code thing, I'll come back to the instruction set. When you look at this block of code, the key thing to understand is this code only executes the addition of one element from within the Arrays that are going to or the matrices that are going to be added together.

And so the key trick is you have to write the code in such a way that it can take in as a variable, which position are you in and then handle everything else just based on that one variable that the hardware will actually feed in. At [00:28:00] runtime, so everything is going to be the same except for what position you're in, and then that will determine the offset of the memory, which will determine what value you load in, which will determine what value you ultimately calculate, and therefore what value you're going to put back into which position in memory, all of that is determined by what position you are ~~in, ~~in the broader array of computation.

And you can think of that as in your case, you've got, ~~you know, ~~a one by eight, but obviously you could get, I believe the current GPUs go up to like three dimensions of,~~ um,~~ yeah, you want to give us just a little bit of flavor as to how this kind of gets more, Complicated from here. Yeah. So in actual GPUs, ~~they have,~~ first of all, they have more than just block index, block dimension, and thread index to identify a thread.

There's like a couple more dimensions of just like different groups of batching that basically ~~just ~~have to use every single dimension to identify what thread you're in. ~~Um, ~~and then some other interesting things. So I basically just captured the most simple piece of GPU programming here. In reality, there's a couple [00:29:00] other very interesting and important things.

So first of all, like. When you're loading and storing data,~~ um,~~ this is something that we'll maybe get to later, but by nature of how GPUs have different layers,~~ like,~~ different levels of memory,~~ um,~~ and they have ~~kind of like ~~shared memory, which is shared between an entire block of threads, which means that four different threads can actually store stuff and read stuff from the same location.

It's called shared memory. ~~Um, ~~And then each thread also has its own dedicated memory called a register file. That's important. And so one complexity that I didn't implement here, which is they're in real GPUs and it's very important for actual use cases is that you can actually choose which memory ~~you're, you're, ~~you're putting stuff in.

So my pattern, there's only two types of memory you interact with. All of these ~~like, ~~mul, add,~~ um,~~ comps, all of these instructions, everything that has like an R in its parameters. So it'll be like multiply R0, R2, R3. That's operating on registers for each thread, which means ~~like,~~ that stuff is all just specific to a single thread, the thread that's currently executing.

And it's storing stuff in these local register files that has local data. ~~Um, ~~and it's basically just performing [00:30:00] computations on the register values. And then there's the load and store, the load and store instructions. Which is either loading data from global memory into the register, or storing data from the register into global memory.

There's really only two levels of memory happening here. In a real GPU, you have separate instructions that are going to let you interact with registers, global memory,~~ um,~~ and also ~~like ~~shared memory, and there's also layers of caches. So that's one thing. Then one other interesting thing is in real GPU programming, You have the ability to synchronize different threads with each other with barriers, which means that,~~ um,~~ because of the necessity of shared memory, that means, like, let's say 4 threads, they want to store something in this shared area and then access it from each other.

But what happens if 1 of the threads is ahead of the other? In other words,~~ like,~~ 1 thread gets to some step, and the other threads are not there. And now, what if this thread is going to read some data from the shared memory? Well, if it's going to do that, it needs to make sure that the other threads are at the same point.

Otherwise it can have a corrupt data or maybe the data is not ready yet to be read by that thread. And [00:31:00] so there's these things called barriers where you can basically synchronize threads. So it's like, this thread is just going to wait until all the other threads of that,~~ um,~~ are going to get to the same point and that is to be something maybe where a recent shared memory or something like that.

So that's another important thing, which again, I didn't implement because it's explainable from here. And also the complexity of implementing it is not worth it.

Okay, cool. That's good. 

~~U~~


## Delving into the Instruction Set Architecture (ISA)

~~m, ~~you want to next just talk through a little bit the instruction set and maybe give a little flavor~~ to~~ of ~~you know, what the ~~What kind of the ~~next, you know, ~~next in instructions would be if you were to expand from here. Yeah, so instruction set, I would say a lot of it is very simple.

So you have addition, subtraction, multiplication and division very straightforward. Everything is take free registers. ~~Um, ~~and so the important thing I'll cover here is just the specifics of the register file. ~~Um, ~~so with addition, subtraction, multiplication, division. ~~Um, ~~for context, each thread has 16 registers, which means that it has 16 different places that it can store,~~ um,~~ whatever values it wants to store for any arbitrary complications.

And [00:32:00] importantly, the last 3 of these register values are restricted. ~~Um, ~~and so we'll call those registers 13, 14, and 15. Those are how, in my GPU,~~ um,~~ the actual,~~ those, those, ~~those custom context values I was talking about, Not a real GPU. It doesn't necessarily work like this. ~~Um, ~~but basically the important thing is every thread has access to its context.

I happen to implement that through these registers. And so these special registers are registers that you can't write to. The GPU itself handles writing to them. And that means that the GPU itself supplies ~~this, ~~this code execution environment with like, Hey, you're this block number. There's this many threads in each block.

And you're also this thread number in this block. And ~~so, ~~again, ~~that's ~~that's how in the hardware, the code has access to those values. Now, ~~the last, ~~the last 13 registers,~~ um,~~ are read write registers, which means the code is free to access these in however it wants. And so these add, subtract, multiply, and divide,~~ um,~~ what they do is basically take the values of 2 registers, which you then specify with 4 bits, which is what you need to specify an [00:33:00] address of 16 different possibilities.

~~Um, ~~and it will take the value from these, from 2 different registers. And it will perform a computation on them, like an issue subtraction multiplication division, and then store that result back into one of the registers, all the registers specified by four bits. ~~Um, ~~now with the load and store instructions, similarly.

The load instruction will take the address of one register. So it will take the value of one of the registers, that's going to specify a memory address. So for example, if that register has the number 4 in it, it's going to go load in element number 4 from global memory. And it's going to put that into another register.

And for the store instruction, it's going to take the value of one of the registers and store it into a memory address in global memory specified by another register. So again, those are register computations. ~~Um, ~~that constant is Very straightforward,~~ um,~~ you ~~kind of ~~just load in a specific value that you want to into a constant,~~ uh,~~ to the register, and that might just be because you want to,~~ like,~~ use it for addition ~~or, ~~or something else.

~~Um, ~~now ~~the, the, ~~the [00:34:00] interesting instructions that I'll spend a bit more time explaining are the BRNZG, which stands for branch, it's a branch instruction, and the comparison instruction. And these two work together, like ~~kind of ~~the simplest implementation, kind of native implementation that allows you to do if statements and looping.

~~Um, ~~and this is ~~kind of ~~like CPU stuff, of course you need it for DPUs too. ~~Um, ~~but the main thing is that what you want to do is create some condition. And then if this condition is true, you can jump somewhere else in your code. ~~Um, ~~which means, like, let's say I want to do something like, if one of my registers is greater than zero, then jump to the end of this,~~ like,~~ skip this entire segment of code, otherwise go through it.

So that's basically like an if statement, right? Or you could do a loop. So you could do~~ like ~~some code, you could put,~~ uh,~~ like ~~a, uh,~~ a label at the top of the code. So let's call it like a loop label, which is actually in one of my kernels below. And then you have a whole part of code. And then below that code, you're going to say, if some condition is true, go all the way back to the top of the loop, which is going to keep it looping until that condition is no longer true.

The way that [00:35:00] you implement this is with the comparison and branch instructions. And it's always basically a comparison and a branch. So what you do is, first you do the comparison instruction. And that's basically, you're going to take two registers, it's going to compare them, and then it's going to check if the result of subtracting the second register from the first is positive, zero, or negative.

~~Um, ~~and it turns out you can actually do a lot with that. So you're just going to compare two registers and it's going to store that result that if they're positive, negative, or zero from the difference between them in something called the NZP register, which is stored in the program counter unit of the GPU, like any compute unit, basically in our case, it happens to be a thread execution unit and a GPU.

And so the program counter now has the current line of code being executed. And now it also has. This comparison thing, which is storing whether the result of the subtraction of the two registers is positive or negative. Now with that, so you're going to have now some ~~like~~ nzp value, and ~~it's going to either have like a, uh,~~ It's going to have a 1 specifying whether it's negative, zero, or [00:36:00] positive.

Now the next instruction, brnzp, which is a branch, it's going to allow you to specify Branch to some specific line, as in, jump to some specific line of code if the NZP register holds some specific set of values. So you could say ~~like, ~~if the NZP register is saying that this comparison is negative, then jump back to her loop code, which is exactly what we did in the matrix multiplication.

So the matrix multiplication needs to do a loop through some code. So what it does is, It compares ~~some, ~~some counter. Basically, it's just incrementing a counter. And that counter is supposed to do,~~ like,~~ some number of loops through the code. So let's say,~~ like,~~ in our case, the counter needs to go through,~~ um,~~ basically two loops.

And so, it's just storing the value, and that value is going to start at zero, and keep incrementing up, until it's past the counter. And so basically, the way you would use these instructions is use the comparison instructions. So you're going to say, Compare my counter to the value that the counter is supposed to always be less than.

And then, if the counter is still less than the max [00:37:00] value, go back and loop. Otherwise, don't loop. And so that's how you'd use those two instructions to create conditional logic. ~~Um, ~~which is exactly what the code does. ~~Uh, ~~so those are pretty important. ~~Um, ~~I know the last two instructions are very straightforward, so there's like the No op, which is basically now you're doing an instruction, it just moves on to the next line.

And there's a return instruction, which tells the GPU that it has reached the end and executing a specific cut. And that's how the entire ISA, and that also,~~ like, that,~~ honestly this part was actually a lot of the hard part. Once you understand this code layer, which is why we started here, then the hardware layer actually becomes a lot more clear what's going on.

And that's partly a result of the fact that this code layer is the result of,~~ um,~~ A lot of fine tuning on the hardware layer also,~~ um,~~ in terms of ~~like, ~~what I actually included here, but yeah,

okay, cool. ~~Um, ~~again, ~~I think I'm with you, but ~~maybe just to try to recap a little bit there, ~~the,~~ I hadn't understood coming in that. You have these three dedicated registers, which is just a position in the local most memory, right? 


## Exploring Instruction Set Constraints

That sort of declare to the kernel, which [00:38:00] is ~~the, um,~~ the form of parallel programming that says, here's what to do,~~ uh,~~ given what position you are in, ~~right?~~

~~Um, you have~~ that indication of where you are is provided in these dedicated registers. And then separately you have. I guess how is that? That's not really related to the size of the instruction set. ~~Right? ~~That's kind of independent. Like ~~how many, ~~how many ridges?~~ I think~~ I was conflating those for a second in my head.

~~Um, ~~because you numbered the instruction set with ~~like ~~a similar gap. Is there a connection there ~~that I'm ~~that I'm inferring correctly? Or am I hallucinating this? So there's a couple of connections in the instruction set to the hardware. There's two important connections. ~~Um, ~~and they're very much demonstrating that this is a dummy project.

So first of all,~~ um, if you, ~~if you look at the instruction set, each instruction is 16 bits, which means that the first 4 bits of the opcode, meaning that basically, since there can only be 4 bits, 16 different combinations of that. That means that with this design I've created, there's actually only space for 16 total instructions, which means there's only space for,~~ I think,~~ 4 or 5 more instructions if I wanted to add them.

Now, the [00:39:00] 2nd constraint is that I've made it so that each register is specified by 4 bits. Which means that there can only be up to 16 registers. If I wanted more registers, I couldn't do that. I would need a fifth bit to specify each register, which means the instruction would have to be longer. ~~Um, ~~and then the second thing is, sorry, the third thing is that the constant and, more importantly, the branch instructions, they both take immediate values, which means they're not taking some value from a register.

They're literally taking values that are specified in the code. Those are numbers. And ~~so, ~~if you look at those, each of the numbers is 8 bits, which means that the branch instruction Can only specify the branch to 8 bits of program memory because the branch instruction is telling it if some condition is true Jump to ~~this ~~this line of the program, which means that in order for the branch instruction to cover the entire program My hardware as in my program memory can only be specified by 8 can only have 256 or by far~~ I think~~ 256 rows of 8 bit memory so those are the constraints created by ~~the ~~The instructions here and again,~~ like,~~ in [00:40:00] reality, for this reason, instructions are usually a lot longer than 16.

~~Like, ~~usually they're 32 bit like the instructions. But yeah,

so

if you wanted to have more memory, you would have to have longer,~~ um,~~ addresses for that memory. And if you wanted to have more, ~~um. ~~Instructions, you would have to have obviously bigger labels for those instructions. And ~~I'm a little,~~ maybe this is where we're headed next, but I'm a little fuzzy. I'm like,

basically each one of these instructions is implemented by hardware. At this point, this is like the last layer of software. When this gets issued to the GPU or to a compute core within a GPU, It now says, okay, I'm going to actually fire up a particular circuit. That's going to do this stuff now, right?

There's no further software. Exactly. ~~Right. ~~And~~ I think~~ one caveat on, so I obviously [00:41:00] oversimplify or pretty much everything I said here in this whole thing is simplified in some way, but I feel like one example of an oversimplification here is like in a branch instruction. In reality, the number of bits in the immediate in a branch instruction, if it is an immediate, is not limiting to the program memory.

The reason that I limited it is because your alternative is to make this thing an offset. So instead of it being like, literally branch this line, you could be like, branch to some offset from the current line. As in ~~like, ~~branch plus 50, or branch minus 50. In which case you could do it a couple times, and then ~~you, ~~You're not limited, so you can get infinitely far in memory.

~~I mean, ~~there's tons of other ways to approach it. That's just one example of a constraint. Because I, one, did not support negative numbers here, and two, I'm not making an offset. I just wanted to jump to a specific lab for simplicity's sake. Now, that's a constraint that, in reality, there's tons of ways around this.

But, yeah, that's an example. And then, in terms of the second part, that's exactly right. ~~So, ~~the important thing to take away from this part, maybe there's still lots of fuzzy details, especially for people listening. The important thing is, One, you understand the importance of each instruction and why it's there, [00:42:00] and what it's supposed to do.

You ~~kind of ~~understand the general programming pattern. Again, it's ~~kind of ~~hard to draw, even just because it's assembly, and assembly itself is ~~like, ~~not necessarily the easiest thing to pick up, but it makes sense when you look into it. ~~Um, ~~but you just need to understand those parts and the important GPU programming patterns, because a lot of the actual implementation will get revealed in the hardware.

Okay,~~ so,~~ I think it's just about time probably to turn to hardware, but let's just scroll through the multiplication one more time because this is where you have basically brought it all together in terms of the complexity that you can support, where ~~we're still, ~~we've still got to be mindful of where we are in the thread, but this time.

The calculation, do I have it right? That ~~this~~ basically this calculation determines one position in the output matrix. That's exactly right. And so you do a two by two, you're going to get a two by two. So you're going to have four spots in the output matrix. So that's why this is four threads. [00:43:00] Each one of those threads is going to do a different set of,~~ uh,~~ it's still going to touch all the numbers basically, right?

But it's going to do them slightly differently to get to the final spot in the output matrix. And to do the sort of rows and columns, it has to do this loop, and this is where you get to the point where you have to have this comparison and branching. Yeah, exactly. The reason is just because of the nature of matrix multiplication being a little more complicated than addition.

With addition, you just add up to the elements. With matrix multiplication, unfortunately, it's not decided. Multiplying the elements, it's like a dot product between two vectors in the matrix, which means like, you just take two vectors, which is just a row and a column of elements, and then you ~~kind of ~~multiply their elements by each other, and then add up the results.

So it's actually ~~like~~ a bunch of different computations, not just like a single point wise multiplication or something, which is why there's ~~like~~ a loop here, and why there's a bunch more multiplications and additions going on.

[00:44:00] Which is what necessitates the comparison interaction in this case, and I would say that's the most important thing,~~ like,~~ for people who want to understand the specifics of the kernel, you can look at it. It's relatively simple, but~~ I think~~ maybe a little bit beyond the complexity of what makes sense to explain on,~~ uh,~~ audio.

Yeah, and I misspoke,~~ uh,~~ when I said that it's going to touch all the numbers, it's going to touch one,~~ um,~~ row or column for each of the two input matrices. Exactly. Yeah. So~~ it's going to take,~~ it's going to touch a lot of numbers. In this case, it happens to be three quarters of them for each computation, ~~but, um,~~

okay, cool. ~~Um,~~ well then I guess it's time to get on to the hardware. So how do you think best to approach that? Yeah. 


## Diving Into Hardware and GPU Architecture

So this part is actually gonna be a lot simpler,~~ I think,~~ thankfully. And so the best way to start it is to just start with the architecture of the entire GPU, and then we can dive into the thread architecture.

And this is a great straight forward ~~here. Now this is the. Yeah, this is yours, right? This one. Yeah.~~ Okay, so ~~now we can dive into kind of the flow of,~~ we talked about this program, right? So now the nice thing is we can explore, okay, how is this program going to actually get executed in the GPU? And that is going to take us through basically the entire architecture and also the [00:45:00] motivation for why everything exists here.

~~So, ~~first of all, let's take the example of our matrix addition parallel. So we have this code. ~~Um, ~~the question is. Are we going to actually load this up into the GKE and how are we actually going to run it? ~~Um, ~~and so ~~I guess~~ what we'll do here is first we'll ~~kind of ~~look through how this works high level in the architecture.

Then we'll look into individual threads and how to see like. How this code is executed in an individual thread level, and then in the~~ last ~~kind of last piece of this that might be interesting is we can actually look through,~~ um,~~ the test case and briefly explain in this repository, like, how it's actually tested and simulated.

So it's not just a theoretical. Those that are written in there,~~ um,~~ there's actually a setup for them to actually get run on this design and see an output of everything that's going on. ~~Um, ~~and so we can touch on that last and maybe touch on some of the interesting things in the code. ~~Maybe not, that's up to you, but ~~so the place to all start is.

We have this matrix edition kernel, and the question is, how do you actually get this to execute on GPU? ~~Like, ~~on one hand, you need to load up the code into there, but then it's like, okay,~~ well,~~ how do I actually [00:46:00] make this thing run and get the result back? So, the way this is going to work is, first, we'll think about global memory, which is ~~kind of ~~like the place where you're going to load up all of the prerequisite data ~~for this, ~~for this code.

~~So, ~~first of all, you have the actual kernel code. And that's as we wrote below,~~ like,~~ or before, it's just a bunch of instructions and those instructions happen to be written in assembly, which is like some nice verbal format for us to visualize them. ~~Um, ~~in reality, we would have compiled that assembly, just ~~like, ~~pretty standard stuff, compile that assembly into the object code, which is testified by the ISA.

So it's just going to be a bunch of ones and zeros. All 16 bits long. And load that into program memory. So now, ~~we would say that, uh,~~ let's assume we've loaded that into program memory. Let's say it's like,~~ I don't know,~~ 12 15 lines long. So now we have our kernel code loaded up into program memory, and that's just going to specify exactly where our kernel is set, just in bits.

And the second piece of it is, in data memory, we're going to load up the actual data that we want to perform computations on. And ~~so, ~~in this case, this would be like the two 1 by 8 matrices. ~~Um, ~~we'll call them A and B. So ~~A,~~ as I said before, A is going to be in addresses [00:47:00] 0 to 7, and then B is going to be in addresses 8 to 15.

And then ~~we'll see,~~ we'll say that C is going to be in addresses,~~ um,~~ 16 to 23. So that's going to be our result. Now currently our result matrix is going to start out with nothing in it. And so ~~what, ~~what is the goal of our entire program? The goal is to somehow get the GPU to use that code that we just loaded up in program memory.

And somehow at the end, it's going to need to fill out,~~ uh,~~ rows 16 to 23 in memory with the correct results of the,~~ uh,~~ additions of A and B. And then we're going to read that out at the end. So from the host machines perspective, which is like the CPU talking to the GPU, what we need to do is basically get this compiled code, load it into program memory, load up our data into data memory, somehow get the GPU to start this whole complication it's going to do and say, and then at the end of it, GPU is going to tell us that it's done.

And then there's going to be in data memory, the answer and the host machine can just read out that answer. ~~Uh, ~~and so that's ~~kind of ~~like the interface of the GPU, basically. So this picture here, we have global memory with program memory and data memory. And that's ~~kind of ~~the one piece [00:48:00] of that. ~~Um, ~~and then like another important thing in GPUs is the actual bus where data kind of transfers between the CPU host and the GPU.

Again, I left that out because of, ~~you know, ~~simplicity reasons. ~~Um, ~~but the other important control thing here, besides the memory, Is,~~ um,~~ what's called the device control register. Now in real GPUs this is a lot more complicated, but, In this case,~~ uh,~~ if you remember, What we need to specify is basically the number of threads to execute.

So we need to tell ~~the, ~~the GPU that, Hey, this thing in program memory, which is just ~~a, ~~a single kernel code, We need to tell it,~~ like,~~ you need to run this thing eight times. And so the way that you do that is in my design, you would store the thread count inside the device control register. And so the device control register is mainly just used to store some like high level data about ~~kind of ~~like how you want the GPU to execute.

In this case, the only piece of high level data we really need to specify is how many threads should you be executing. And so now we have program memory loaded up, data memory loaded up, device control registry loaded up. Those are the three [00:49:00] things you need to do. To get this GPU to be prepared to run something.

And then, that's ~~kind of ~~the external interface. Then we're going to send a start signal. And that's going to tell the GPU, Hey, everything's loaded and ready to go. You need to start, basically, performing computations on the data. And ~~that's like the,~~ that's like a clean break. So that's like ~~the, ~~the interface to interact with the GPU.

Now we're going to get into ~~like~~ the computational part of it. ~~Um, so, ~~I'm just lost there. Does that thing make sense? Yeah, I think so. ~~Um, ~~and~~ you know, ~~probably just worth,~~ um,~~ reiterating that there's like even in some ways, more complexity on the CPU side, when you say the host machine, we're sort of assuming here that ~~like,~~ you have a general purpose CPU that can do the compiling and can ~~kind of handle, ~~handle the like outer loop of.

Here's what I'm trying to do. And, ~~you know, ~~get something back and show it to you on a screen. ~~So, you know, ~~it's done,~~ um,~~ and this sort of sits within that. So ~~it's, ~~it's funny because ~~the, ~~the programming paradigms in ways is more complicated, but then in other ways,~~ like,~~ it's a lot less complicated because it can [00:50:00] take advantage of all of the,~~ uh, You know, sort of ~~universal computing benefits of a CPU host machine.

Aside from that,~~ I think I'm, ~~I think it all makes sense.~~ Right. ~~That's a good point. Because GPUs are not really meant to run alone. They're always in practice,~~ like,~~ either hooked up to a host, like you'll see them next to a computer in like a rack or, ~~you know, You know, ~~you have, you connect to one on the cloud or something like that.

~~I mean, ~~that's not really very effective, but,~~ um, like, ~~depending on what you're doing, but yeah, they usually have ~~like ~~a host connected to them that can send them data and interface with them.~~ Um, ~~yeah, that's a good point. S


## Understanding the Dispatcher and Thread Execution

o now we can get into the computation pattern, right? And high level is actually pretty simple.

So the main things to focus on is you have this dispatcher. And the dispatcher is just responsible for, as we said,~~ um,~~ these threads are executed in blocks, and a block is just ~~kind of ~~like a batch of threads. It gets executed together and the same for key resources. And so basically, the way to think about this is your GPU has some large number of resources that are organized inside cores.

And so this GTA design happens to have four cores, and each core has the capacity to execute a bunch of different threads in parallel. And ~~so, ~~from a high level, [00:51:00] before diving into what's in cores, let's just assume,~~ like,~~ the core is some black box. And we just know that this black box, we can just give it,~~ like,~~ some group of threads, which is going to be a block size of threads.

So in this case, four threads at a time. We can give each compute core four threads at a time. We're going to do some applications and,~~ like,~~ finish tossing the threads somehow. And that's going to tell us when it's done. And so the high level job of the GPU now is like, okay,~~ well,~~ how do we manage how to ~~like ~~divide up these threads into the available compute cores,~~ um,~~ wait for them to complete their job.

And then give them more jobs when they're done computing their work. And so basically all it ~~is, ~~is just managing all the compute cores, figuring out when they're available for new work, and then dispatching new blocks to these,~~ um,~~ to these cores. Now, in practice, this is where like one, this is one place where there's a lot of complexity in GPU, because you can imagine when you have a ton of different cores performing stuff at once and different cores can perform different blocks, like they, I see different blocks.

Threads at once, and ~~like, ~~they're, they have a complex resource management,~~ um,~~ you can do a [00:52:00] lot of different optimizations to make sure that you're getting maximum resource utilization. And ~~so, ~~this is something where there's like a ton of space for optimization,~~ um,~~ in terms of. Using things more efficiently, threading in different threads at once to make sure that everything's getting used.

And then, of course, for simplicity's sake, in this example, we use a very simple version of that, which is just that the dispatcher~~ just~~ looks out for when a core is done executing its threads. And just as it worked for us and just ~~kind of ~~like a round robin style. So it just goes, looks at all of the course sequentially and then keeps doing a more dress if they're ready.

That's like the ~~simple, ~~simple way to think about it. And so the dispatcher is ~~kind of ~~one of the more complex elements of the GPU. Now, if we get into the individual compute course,~~ um,~~ dispatcher layer for a second, for one thing, what level of design did you have to go to in this project to. Create a dispatcher.

Is that ~~like~~ something that you had to Design and if so, at what level, or was it something that you could ~~kind of, you know, ~~[00:53:00] drag off a menu of available components? Yeah. So pretty much nothing here was an available component, to be honest. ~~Like, uh, I have two. ~~So the nice thing is I had ~~like ~~two or three repositories to reference.

~~Um, ~~so there's this thing called Meow GPU, which is like an open source Verilog GPU made a while ago by Sunskull Africa, which is cool it is. And then there's this thing called VeriGPU, so two open source GPUs. ~~Um, ~~the thing is, these things have like very little documentation. And then they're not really written to be simple, they're written to be like attempts at production GPUs.

~~Um, ~~one of them is like completely unfinished, Meow is actually finished. ~~Um, ~~And 1st of all, architecturally, they're somewhat different in some ways, because again, they're optimizing for production usability. ~~Um, ~~and the 2nd thing is,~~ like,~~ because of how big they are, they're just not very easy to understand.

And so ~~kind of ~~my process ~~for, ~~for creating things,~~ um,~~ was not really, you can't really go through them and try to understand. ~~It's like, I know~~ the analogy is like, if aliens come to earth and ~~try to, like, they~~ find the computer, like, how are they going to understand it? Are they going to break it down and ~~like, ~~look at all the connections, the transistors and ~~like, ~~see what's happening?

~~Well, ~~no, they're not going to understand it by doing that. They have to come to earth. ~~Um, ~~Come to some [00:54:00] understanding of their own and then test it against the computers that they have. It's a bit of ~~like ~~a massively over,~~ over a~~ complex analogy for going through a GitHub repo. ~~Um, ~~that's actually the analogy for mapping out the brand, which is not a big deal there, but,~~ um,~~ Yeah, so my approach to going through these repos was not like going through them and trying to understand.

It was actually like talking to Claude in chat QPT about, I see like names of things, like I'll see a folder called, I don't know, just that for schedule or whatever, and I'll try to figure out with Claude, through first principles, like where does this have to fall into place in the GPU? And then that part's not too hard.

So then it's like, okay, I get to something, then I'll start to propose how I think it works. And the reason is because there's not really anything that teaches you how these things work, like anywhere online, ~~basically,~~ because it's all proprietary and they have their own algorithms and stuff. And so even to make a simple version, you ~~kind of ~~have to be like, so for the dispatcher, for example, I come up with a hypothesis like, Oh, I think a simple version of this would be XYZ.

Like, I think a simple version of this would be like round robin scheduling. While looking at what [00:55:00] course are available, which is super simple, and then I would have to get confirmation. So cloud would be like, actually, I don't think that's the best way to think about it. I think you should think about it like this or something like that, which is interesting that there's nothing publicly available, but in chat, in some cases, it's things that are purely intuitive and it just has the benefit of engineering intuition on stuff that I haven't gotten to.

In some cases, it says stuff that's ~~like, ~~definitely implemented in proprietary GPUs, and maybe it's still out there through intuition, but it's a little more,~~ like,~~ stuff that's a little more complicated than what I expected it to know,~~ um,~~ which is pretty cool. But, yeah, as a long winded answer to your question, there is no, like, off the shelf stuff.

I basically had to design everything myself from how I thought it would work. And then get confirmation from it. Maybe look into the repo to see ~~like, ~~Oh, this repo actually happens to do something a little similar to what I suspected, and now I can actually understand it because I came up with a truce.

~~Um, ~~and I had to do that for ~~like ~~all the elements, granted, some of them are a lot simpler to understand than others, but yeah. Okay. So this thing [00:56:00] implements a round robin where it just says, I'm going to just keep looping through as long as I'm live. I got to just keep looping through all of the compute cores, check their status.

So that implies then that the compute core is like maintaining a status that can be checked. And. If it's available, then I'll send it another thread to process. And if it's not, then I'll come back to it on my next loop. And all of that is implemented in hardware. You're beyond the point of programming this at this point, right?

This is implemented in hardware. Yeah. So do you have a diagram of that? Can we look at that? ~~Um, ~~Oh,~~ uh,~~ we can look at the code in the repo. There's no diagram. The diagram is for the red execution, but there's no like dispatcher diagram. Gotcha. Okay. ~~Well, ~~let's look at the code ~~just~~ to just see what that looks like.

~~Um, ~~so if you go into source and then dispatcher dot, [00:57:00] let's see.

Yeah, this is it. You can see all the code is documented with, like, at the top, you see there,~~ like,~~ the important points. And you can see there,~~ like, some, ~~some of the things that,~~ um, we were, ~~we were saying must be there are there. ~~So, like, ~~1st of all, the important thing with the dispatch is that it has a start signal.

And what that means is,~~ like,~~ that thing we were saying at the top level, we're going to tell the GPU to start. The place where that actually goes is into the dispatch. So the dispatch says ~~like, ~~Oh, I've gotten filled a stamp. Now I'm going to start sending off these blocks to the actual cores. And that's what starts execution.

So that's the start signal you see here. You see the thread count coming in from the device control register, which is again important for the dispatch because it needs to know how many threads does it need to execute in total, how many threads has it already executed. ~~Um, ~~and that's what's going to tell it like, oh, I have this many transport to execute.

Let me go send them off to the compute units. Then you can see the core stage. So that's the thing where you're saying, oh, it looks like the cores must have their own knowledge or like status of if they're ready or not. And so that's exactly what you see there. You see core done, which is like, oh, this core is done processing.

And [00:58:00] then, ~~you see, ~~so you see core done, core reset, and core start. Those are important. ~~So, ~~this is basically the way the dispatch gets to do stuff, right? So ~~it's, ~~it's waiting for the core to be done. It's going to say, oh, here's a core that's done. Let me reset this core. So that's going to set all the state back to empty.

So it's going to clear everything out. And then it's going to say, oh, this core just got reset by me. Alright, I'm going to go start it up with the next block of threads, if there's still more blocks. And if you slow down a bit, you can see,~~ um,~~ There are some intermediate variables, which store like how many more blocks do I have left?

So that's blocks to stashed and blocks done. ~~Um, ~~and that's just saying ~~like, ~~okay, ~~I need to, ~~I need to process this many more blocks of credits before this is completely done executing. And then the last thing that the dispatcher does down in this loop, and you can see at the top, there's a done signal exported from the dispatcher.

That done signal is sent out to the GPU itself. And so now that one. But in the actual,~~ like,~~ module definition a little bit further up,~~ um,~~ there's just something called just straight up done. You can see it in a couple places. Output register done. And that's going to tell the whole GPU, Hey, [00:59:00] all, everything is done.

And then it's going to stop executing everything. And now it's just going to wait for the OS machine to basically pull out the results from memory. And then the OS machine can just reset the GPU. 


## Deep Dive into Hardware Design and Verification

And that's ~~like ~~one full execution loop. And you can see that the dispatcher, kind of high level, is responsible for managing that whole,~~ like,~~ high level execution flow.

So yeah.~~ Right. ~~Cool. ~~So, ~~this is code. How does this thing get translated into hardware? This is what the package that you're working in does?~~ Uh ~~huh. So the way that this whole thing works is just a PDA in general. ~~You design your, ~~you design your architecture based on what it's supposed to do, which is a functional logic,~~ um,~~ in Verilog, or in this case system Verilog, which is just like a modern version of Verilog.

And then there's these entire software stacks, which is what I was talking about before, which basically translate that Verilog. Into an actual design. And in practice, that's really hard because there's so many different steps that go into it. Like you need to synthesize the Verilog down into just like a [01:00:00] logic.

There's like a chart of the logic that's specified in there. And then because of the way that people program stuff, that logic is inherently not going to be perfect. It's going to be ~~like~~ way more complicated than it needs to be. You can do some processing to basically get that logic down into its simplest form, that's still the equivalent.

So that process of turning the Verilog into ~~like ~~a logic flow is called synthesis. ~~Um, ~~and then once you do that,~~ um,~~ you can, ~~you~~ perform a bunch of analysis on, like, whether this design is valid or not, then you convert that, that logic that you've created into gates. And then those gates are based on a specific process.

So ~~basically, ~~basically,~~ um,~~ you have these things called standard cells, which are specific gate designs designed for a specific foundries process of producing gates. So ~~you, ~~you convert them into gates. And then you lay out all these gates on a huge chip design. So the chip, the gates are just like laid out everywhere all over the chip based on ~~like ~~a bunch of different optimizations.

Then you hook up all the gates with wires, like the gates that need to be connected together. ~~Um, ~~and then there's like several cycles of optimization on this whole process to make sure [01:01:00] that everything is valid. All the timings are valid because like electrical signals need to flow through this chip.

And if any of the signals. slower than the actual clock time of the chip that's going to cause error. So there's like tons of different errors there, even just at a logic level. And then on a hardware level, because this is actually like electronics, it's not just like code, ~~you know, ~~it's nice to write it in code, like the complexity is way higher.

~~Um, Like ~~there's these things called parasitics, which is like, Oh, you're actually dealing with wires and metals. And ~~like, ~~if there's wires near each other, they actually have capacitance between each other. And there's like tons of other electrical effects that can fuck with the shit. And so ~~like, ~~you need to do copystakes to prevent that stuff too.

And it's ~~like, ~~there's so many complicated things that at the very end, your whole design is there. It gets outputted into a. The layout, and ~~that's, ~~that's in the form of a GDS 2 file, which just happens to be the file format specifying all the metal layers to send to a foundry. And then you do a final comparison called a layout versus sematic, which is make sure that ~~like, ~~this final layout you got after tons of optimization is actually logically equivalent to your original [01:02:00] design, and then you can submit that layout to like a foundry.

And now in practice, you're actually going to do a ton of ~~like, ~~formal verification also ~~on this, ~~on this layout to make sure like, all of these bad states are impossible to get into, ~~like. ~~And, again, at Hardware Design in general, the verification process is so important, because, unlike software, you can't,~~ like,~~ ship and iterate.

~~Like, ~~you're just fucked if you mess it up. ~~So, um, ~~there's all that stuff. But that's what happens, and again,~~ like,~~ if anyone had to program all that, ~~I mean, ~~that's ~~like, ~~that's impossible, it's a gigantic task, but thankfully, all these EDA softwares do it for you for,~~ like,~~ a couple million dollars. And then, thankfully for me, there's,~~ uh,~~ OpenLAN, which does it for you for free.

Enough super level, but yeah, even that complexity going through it. Cause ~~I, once you, ~~once you do that, you run through a bunch of errors and then you have to fix that in your code. Yeah. Yeah. You can see where the decades have gone in terms of building up ~~the, uh,~~ the stack talk about, ~~you know, ~~on the shoulders of giants,~~ um, what, ~~what does this feel like on the.

Open version that you were working on when you go to,~~ like, I'm not even, ~~I'm not even sure what the right word is, but ~~sort of, you know, ~~I want to say compile, but it's almost, it's more like [01:03:00] translate from hardening designs. That's what it's called. Hardening. So how long does that take for something relatively simple like this?

And you're running on your local. Yeah, so local laptop, I would say it's pretty powerful for this stuff, given that it's ~~like~~ an M2. So that's probably on the better side of ~~like a, ~~like a hobbyist doing this stuff. And it can take ~~like ~~20, 25 minutes to go through the whole flow. ~~It does like, excuse me, does like 50 different steps.~~

~~Um, and thanks.~~ It does like 50 different steps and that takes like a bunch of time. Does like tons of optimizations and really cool things. Like you can see all the different steps going on and ~~like ~~try to understand them. And then you can run into errors on any step, often you do. And the one thing is like, obviously the stuff isn't like perfectly documented or, ~~I mean, ~~there's like millions of errors you can run into, obviously I think saturation, but ~~like ~~so many different errors you can run into.

And it's not really well documented, almost out of number, well documented. And they're also like really random error messages. And so ~~like ~~one of the challenges of it is ~~like, ~~it's a lot less easy to use. Like ~~you just gotta,~~ you just gotta figure stuff out. And it's ~~like, ~~so it's not just stuff. You have no idea what's going on and you just gotta ~~like, ~~try your best to figure out what's going on and debug it.

~~Um, ~~so I think very [01:04:00] low transparency on the debugging side, which is ~~kind of ~~one of the biggest, ~~like ~~that's the biggest thing, cause that's the whole flow, like that's basically the output of the flow is like, what bugs do I need to fix before I can finalize GDS? ~~Um, ~~but it's still both. And you just push through it, then it works.

~~Uh, ~~so then you get your cloud and it's ~~like~~ magical. And then you can start visualizing it and it's pretty sick. Yeah, it's fascinating. How many cycles would you say you went through in this project of that,~~ like,~~ 20 25 minute hardening process before you got one that actually didn't error out on you? Oh, a lot.

~~I mean, ~~I have all of them saved in here, I can say ~~it's like, ~~it's ~~like, uh, ~~like 30, 35, something like that.~~ Like, ~~a lot of different cycles. Interesting. Sorry, they're not in the repo, they're just in ~~my, ~~my local. Yes. Yeah.~~ Um, ~~okay, cool. S


## Returning to GPU Architecture and Execution Flow

o let's come back to the overall GPU architecture. So we've got ~~kind of ~~these modules, components that are defined in code that are hardened into an actual, [01:05:00] ultimately ~~like, ~~I guess the classical word would be like etching, but now~~ it's like, um, ~~With this, it's like a,~~ uh,~~ it's a light process, right?

At least the most advanced notes. So I forget. Yeah. ~~Um, ~~thank you. So the, that translation is happening with this, like decades in the making ~~shoulder of~~ shoulders of giant software stack, and that gives you the ability to define each of these things and then it go to come back ~~in,~~ in 20 minutes and see if it worked or not.

~~Um, ~~yep, exactly. And ~~you're,~~ you have to then also, ~~I guess, ~~define the interface, right? Like the compute course have to maintain. So~~ maybe let's go look into, well, you take me where you want to go~~ next, ~~but ~~I'm ~~kind of ~~interested to see, ~~like. ~~A little bit of the interfaces is always ~~kind of, ~~I think about programming a lot in terms of interfaces, like where is it that it's declaring whether it's done and not done,~~ um,~~ so that the dispatcher can, ~~you know, ~~reassign or not reassign as appropriate, but take us through the rest of the architecture, however you think best, and we can check out a couple of those things.

Let's look at the GPU. se file first. That's the high level interface. That's going to be interesting. And then we can look into the compute cores in detail and put in the trial [01:06:00] execution stuff.

Yeah,~~ so,~~ this is the high level file. ~~So, ~~there's some parameters at the top. Those are mostly unimportant. ~~Um, ~~the interesting ones are the number of cores and the number of threads per block. So here, yeah, I guess that's like the two. That thing you can just completely change around. So ~~you can, ~~you can switch the number of cores to ~~like ~~three or four or whatever.

And you can switch the number of threads in each block, which is just gonna change. ~~Um, ~~how many dreads can get executed on each core at once, which means that there's going to be more compute resources and register files and everything on each core,~~ um,~~ and that will make more sense later. ~~Um, ~~but you can see the high level interface here.

You have the clock and reset. Those are mostly unimportant. Those are ~~kind of ~~just like the, you have that for every design and that's just going to ~~like ~~allow you to have clock cycles on your GPU and reset stuff. ~~Um, ~~the interesting part of the question on clock also, it seems like if everything is built perfectly.

Everything would take the same amount of time. I'm a little bit confused as to why if I distribute four threads across this thing, like why don't they all finish at the same time? Good question. So [01:07:00] the reason, the sole reason for this, and this is the reason behind my memory intuition and black or chops at the whole problem is memory.

We'll see that when we dive into the thread execution is like. If there was no reading and writing from memory, it would all finish at the exact same time because everything is deterministic there. It just takes the same amount of cycles for every instruction. The thing is, when you have memory,~~ um,~~ like loading from global memory, that memory is DRAM.

So first of all, it's using capacitors to store memory, which is ~~like, ~~it has some latency to it. You don't just get it after one clock cycle, basically, which has some non determinism. The bigger thing is the bandwidth issue. If I have a thousand compute cores requesting some value to memory. And memory can only read,~~ like,~~ support a hundred reads at once.

That means that this is going to start to get chewed up. So there's going to be like, a thousand compute cores request data, then a hundred of them are going to get back data the ~~next hundred, ~~next hundred. Which means that certain cores, even if they're on the same, even if they're being processed together, they might make requests to memory at the same time.

They may not get the data back at the same time, because memory has an unknown latency, it's asynchronous. ~~Um, ~~and that means that ~~like, ~~[01:08:00] if one thread gets enry back earlier or later than the other ones, then it may have to wait for the other ones, or there's a bunch of stuff that happens around that. So in my design, it waits for the other ones, which means it can't just ~~like ~~keep going.

~~Um, ~~and then ~~like, ~~similarly across the cores, even if they all start executing threads at once, one core might finish way before the others, because it just did it from enry back earlier. And so that constraint has really no bottlenecks to see it ends, which is why, err, not a sin. It's all about managing memory latencies, that really is the bottleneck.

And the clock, just to set a foundation on that as well, is Essentially an electrical impulse. It's ~~kind of ~~a change in voltage that is getting applied through the whole. Shit. Is that right? Yep. So the clock is just basically a cycle. It's like a sine wave almost of some signal going from high to low over and over at some periodic interval, usually a couple of nanoseconds, like 20 nanoseconds or something like that.

And basically every time the clock goes from zero to one, it's just like a sine wave, but every [01:09:00] time the clock goes from zero to one. ~~Um, ~~registers ~~in, in the, ~~in the check, which are like deep with loss, they will take in a new value. And so that creates the way for ~~state, ~~state, that type of state transfers on the clock.

So like whenever the clock happens,~~ um,~~ which means that it ~~kind of ~~sets the pulse of ~~what's, ~~what's going to happen. So it's like generally in each clock cycle, you're going to have ~~like ~~the start of the clock cycles and new values are set. Then you have all these wires propagating signals. And then the next clock cycle, the values are going to get set again.

And so it's ~~like, ~~it sets this time interval where ~~like, ~~state is set on the clock cycle, and then self set happens ~~in between, ~~in between that time of where state is set. And that's going to help you influence what's the next state. And the other thing that's important about the clock is ~~like, ~~You can't just set the clock insanely fast, because the chip actually has physical constraints, right?

~~Like, ~~electricity actually needs,~~ like,~~ if you need,~~ um,~~ something on all the way on the left side of the chip to communicate with something all the way on the right side of the chip in one clock cycle, there's actual constraints there, because the,~~ like,~~ The electricity takes time to propagate across the chip, which means that your clock cycle needs to be longer than [01:10:00] the maximum propagation time of signals that need to communicate in your chip.

~~Um, ~~and that's actually something that EDA stacked out. So that's one thing, static time analysis, make sure that all the timings in your chip are valid based on the clock cycle time. Gotcha. Okay, cool. So if something is waiting,~~ I guess, ~~again, it sounds like you could implement this in probably a lot of different ways, but you could, Have your cores sort of saying,~~ like,~~ I'm in waiting mode.

So this cycle, I basically just do nothing because I'm still waiting for the memory to return. And then next cycle, ~~you know, ~~if I got it back, then I can actually do it. And that's, ~~you know, ~~because there's different latencies, they can just ~~kind of ~~diverge in terms of where they are in their particular.

Execution flow.

In an actual like production environment would be, ~~you know, ~~however many gobs and gobs ~~of, ~~of gates ultimately that are being included in a single chip. 


## Exploring Chip Fabrication Challenges

Now, presumably there's also [01:11:00] some difficulty there, like some just like inconsistency or whatever that could create divergence. ~~I guess, ~~I don't know if that's the kind of thing that would get disclosed, but I imagine there must be some sort of.

engineering just to try to not allow ~~like ~~some local defect to ~~like ~~ruin the whole thing, right? Yeah. ~~I mean, ~~I would say that's one fabrication layer. There's tons of like local defects is actually one of the biggest problems in ~~like~~ the fabrication industry. ~~There's like, ~~that's why contamination control stuff's a big thing because I do start scaling down the size of individual transistors.

Now, smaller and smaller defects that didn't matter before can actually break everything because they can get in the way of gates or like getting, Basically, there's tons of different places that check where. I think having that can just ruin the whole thing. And that's why there's,~~ like,~~ just like all the technology on actual fabrication has been advancing to smaller and smaller scales, the contamination control technology has had to get better and better.

~~Um, ~~but that being said, that's more so a concern of the actual fabrication process. The reason is that they actually have a ton of testing, and the testing is built around, [01:12:00] like, 1, they have a lot of contamination control, 2, they have testing to make sure that even if there is some contamination breaking the chip, that they're going to be able to test that and discard the bad ones.

That process is imperfect, but generally speaking, ~~I mean, ~~that's probably the biggest thing that determines chip yields in practice. ~~Um, ~~and generally speaking, that's a concern of the foundries. Not really someone like NVIDIA who's doing the design. They'll just ship off their designs to TSMC, and the TSMC will have to be concerned with that.

~~Um, ~~but generally speaking, NVIDIA can probably assume that most of the chips are working once they get published. Okay, cool. All righty. ~~Um, ~~should we go back to the diagram? Yeah. You can do that. Yeah,


## Diving Into Compute Core Operations

so now we can go into what's going on inside each compute core. So we already saw the interface of the dispatcher. So each compute core is basically going to get told by the dispatcher. ~~Um, ~~you're executing this block ID. And you're going to get this many threads in the block 80. ~~So, like, ~~what's a, what dispatcher's going to say, Hey, execute four threads in block number two.

And tell me when you're done, basically. So what's going to happen is the dispatcher is first going to reset the compute [01:13:00] core. Then it's going to tell it,~~ like,~~ here's your block number, here's how many threads to execute. And tell it start. It's going to send it a start signal, similar to how the GPU got a start signal.

And then the question is, what's going on inside the compute core? ~~Um, ~~the process does trends up until the point where it's reporting back to the dispatcher. Then it's done. That's ~~kind of ~~like the high level interface, like a few core. ~~Um, ~~and so there's a couple of pieces of core. And 1st the high level control launcher that's shared between all the threads.

And then there's like the actual thread execution,~~ um,~~ where we split out into a number of different threads within the core. 


## Understanding Thread Execution and Control Flow

~~So, ~~first we can talk about the high level logic that's shared between all threads. And then we can dive into the thread. So high level, there's basically three units that are shared between everything.

So there's the scheduler, and again, this is where there's a ton of complexity. It's now managing the resources of How many, however many different groups of resources there are in the TMP core. Now, in practice, the TMP core isn't actually thought of as ~~like, ~~having a certain number of threads. It just has some finite number of resources, and then however many threads it needs to execute, they just stay executed [01:14:00] on those resources.

And ~~so, ~~typically, a scheduler is responsible for handling the difference between like, This doctor says, hey, attitude 8 grows, and you may only have 4, 4 different groups of resources on your compute core. So now the compute core needs to ~~like, um, kind of ~~manage the execution of these threads ~~in, in,~~ in parallel or in sequence or how her determinants is most efficient.

~~Um, ~~so again, that's why there's a lot of complexity in the scheduler. In my case, what I basically said is. Each compute core is just going to process one block at a time. So it's not going to be able to say like, Hey, you can give me 8 threads, and I'll do like 4 at a time. It's just going to be like, just give me however many threads I support.

~~Um, ~~so each compute core supports 4 threads at a time, which means that each resource a thread needs It's going to have one, one resource. So like each side of these register file to be forced to have four register files, each thread is on ALU. So you get the point there. ~~Um, ~~and basically what happens is the scheduler,~~ um,~~ handles the execution of the threads in terms of there's, let's say 15 instructions that each of these threads needs to execute, right?[01:15:00] 

So now the scheduler is going to constantly. Execute the control flow of how these instructions get handled. And so the way that happens is let's say we're on instructor number zero. So we've just been issued stuff like a group of like four threads for the dispatcher, and we need to execute these threads.

So we're on instructor number zero. So what we're going to do is, first of all, we only know to start with instructor number zero. We don't even know what that instruction is. So first we need to somehow get that instruction from where it's stored. It's stored in program memory, because that's where we put it before at the start.

And so the Fetcher,~~ um,~~ is the first thing ~~that's gonna,~~ that's gonna execute. 


## Decoding Instructions and Managing Compute Resources

So the scheduler is gonna tell the Fetcher, Hey, go retrieve this instruction from program memory. So that's the whole job of the Fetcher basically, is to get instructions from program memory. ~~Um, ~~and then in practice it actually doesn't catch it, because instructions are very repetitive, like, All the threads are going to be executing the same instructions.

So what optimization we can do that's nice,~~ um,~~ is that the fetcher, once it gets an instruction, once it can just store it locally, and then all the threads can just use that again instead of [01:16:00] going global memory. So that's the fetcher. And then what the decoder is going to do,~~ um,~~ which is going to Basically get us into the thread level is we now have this instruction, which is a ~~bunch of ~~bunch of ones and zeros.

It has this opcode, which is going to tell you what the instructions supposed to do, and it has all the registers and specific values. Now, we need to somehow translate that instruction into something that all these different compute resources can actually use. And so that's the job of the decoder. ~~Um, ~~and as we get into this thread, it will become a lot more clear what the decoder is actually doing.

~~Um, ~~so let's look at the actual compute resources that are in Thread. This is the last piece on this diagram, and then we'll go on to the next diagram. ~~So, ~~within the Thread, in my design, there's basically four key pieces of memory and resources. So each Thread has its own register file that we've already talked about.

And that's ~~like, ~~each Thread has its own ability to perform computations ~~on some, ~~on some beta. And then, importantly, it has its own,~~ um,~~ program counter, which means that each thread can,~~ um,~~ be on its own line of ~~the, ~~the program. And that's [01:17:00] because Based on the data, different threads might ~~like ~~have to jump around different lines of the code.

~~Um, ~~and in practice, that's challenging to implement. So that's called branch divergence, which means ~~like~~ different threads branch to different lines of the code. Now, in our design, even though each thread has its own program counter, For simplicity, all the threads are assumed to be basically continuing on the same instruction.

And it just so happens that I wrote programs where that is the case, like all the threads stay on the same instruction. So this design was sufficient for implementing that. ~~Um, ~~and then last two things which are important, so each thread has its own ALU, Arithmetic Logic Unit, which is the actual compute that's like performing multiplication for addition.

So that's doing all the arithmetic instructions in there. ~~Um, ~~and it's performing computations in the registers. And the last thing is the Load Store Unit, or the LSU. And that's the thing that's responsible for fetching data from memory. And so that's the thing that does the load and the store instructions.

So as you can see, each thread has its own unit that is separately able to load data from memory and store data into memory. ~~Um, ~~and importantly, before we dive into the specifics of how all these pieces interact, [01:18:00] and I know it's ~~like~~ completely unclear at this point, it's just like, oh, I guess it's like these high level things.

I wonder how they actually work in practice. ~~Um, ~~the important thing is that the Fetria and the LSUs, There, there's like a bunch of them across the GPU, right? Because each core has a center. And that means that if we have four cores, there's going to be four fetchers and it might all be requesting instructions at once.

And then similarly, there's going to be like, there's four LSUs per core and four cores. There's going to be 16 LSUs in the whole GPU. And ~~like, ~~those could all be requesting memory at once. So the question is, how do we manage the constraint of. Memory has a fixed data. Let's say I can only take two requests at once or something.

And all these resources are requesting memory at the same time. So you need something to actually like throttle all the memory requests. And ~~kind of ~~on the GPU side, hold them. So it's like, here's all of our requests. And then send them slowly to memory,~~ um,~~ to respect the bandwidth that our reaction supports and then slowly send those responses back into the individual compute units in the core.

So that's what the memory controllers are for. ~~Um, ~~so there's one for program memory, one for data memory, [01:19:00] and those controllers are basically responsible for respecting the bandwidth that the global memory actually accepts. And then taking all of the requests from compute resources and throttling them to the bandwidth that the memory accepts.

That's what the memory controllers do. for tuning in. And yeah, with that, I'll pause there and then after this, we can dive into the actual execution.

Yeah, I think I get it. And again, all of these things are at this point, purely physical, right? There's we've left the realm of software some time ago. So the software really stops at the point where the kernel is compiled. Is that the right word in that case? And put into the program memory. Oh, and then everything after that is a purely a function of the hardware.

The hardware ~~is, ~~is routing everything through just an insane tangle of ultimately logic gates. Exactly. Yeah. [01:20:00] Does anyone have an intuition for that at this point? It seems like we've ~~sort of ~~got so High up this tech stack, ~~you know, ~~over the decades that I wonder, is there anyone that can really ~~like ~~go to the sort of gate level ~~and, ~~and understand like how something as complicated as a,~~ you know, ~~data memory controller.

It works. Does anybody have an intuition for that at this sort of logical level? Yeah, definitely. Yeah. So I think,~~ like,~~ most people~~ in~~ doing architecture design stuff, they'll probably understand most of these elements at a gate level. ~~So, like, ~~obviously more complicated logic. It's ~~like, kind of ~~futile and ~~not really,~~ there's no point really to try to understand exactly what's happening at a gate level.

I think the main intuition you need is ~~like, ~~Understand the core of how memory works at a gate level, usually like static RAM. ~~Um, ~~and that's ~~like~~ pretty interesting. You understand how like a latch works and then a flip block works. And that's like the core of understanding memory. In practice nowadays, every step, like most areas dynamic and only ~~like~~ cache is static,~~ um,~~ but that's something people understand at a low level.

And then like ALUs and. Again, we're going to go into the diagram and that's going to show you basically as close to the low level as [01:21:00] you get. ~~Like, ~~it's going to show you multiplexers and stuff, which again are pieces that people understand at the hardware level. ~~Um, so, ~~yeah, I would say people do understand it at that level.

Now, in practice, you don't really need to, as long as you ~~kind of ~~know. ~~Like, ~~as long as you ~~kind of ~~trust the process, you're just like, okay, I know that this is going to get translated into gates and ~~like, ~~this general way, you can study the gates and computer architecture class. And ~~like, ~~you don't really need to go past that.

And then I would say,~~ like,~~ really cracked architecture people. There's a ton of stuff. ~~Like, ~~the thing that makes them really good is that they're managing a lot of stuff in their head, which most people are not. And usually that's not really,~~ like,~~ gate level logic, although I'm sure they have that in their head too.

It's more like understanding the implications of stuff besides just,~~ like,~~ the high level Like, design's a really nice high level, and practice,~~ like,~~ there's actually a lot of complexity. ~~So, ~~for example, writing code in Verilog, like Knowing how many gates a piece of code actually translates into is important.

Like for me, it's like, oh, I might just write the divide sign as my division instruction. This is the C. In reality, nobody would ever do that. Like the divide sign actually turns into ~~like ~~a gigantic piece of hardware, which you would never actually want to use. ~~Like~~ you wouldn't actually want to implement the division thing as an [01:22:00] instruction.

So it's ~~like~~ things like that. And then also being able to manage all the parasitics and knowing ~~like, ~~The actual electronics of it and how the electronics work. If you place things in different places, there's like tons of things like that. Honestly, the way I would describe it high level is ~~like, ~~people have a surprising level of understanding of the EDA flow and the things that influence that float in their head.

And they ~~kind of ~~can get it by intuition, obviously, not the whole thing, but ~~like, ~~pieces that most people want and somewhat I've noticed from my,~~ like,~~ very limited perspective. That's what a lot of the really good architecture people have. ~~Um, ~~so I would say certainly there's people with intuitions and all these things.

Fascinating. Okay, cool.~~ Um, ~~so should we go to the thread diagram? Yeah, we can do that. And this is going to be nice, especially for people who are familiar with CPUs, cause this is going to get into very familiar territory. ~~Um, ~~so you can see here something that looks very similar to a CPU in many ways. It almost is exactly like a CPU except for the LSU and like the little details in the register file.

~~Um, ~~but what you see here is, first of all, most importantly, everything that [01:23:00] has red types and blue types, that is stuff that's coming from the decoder. So now you can actually see exactly what the decoder is doing, which is the decoder is responsible for converting the instruction Into these red and blue signals, and these red and blue signals are going to be used as control signals to control the execution of an individual thread.

What you see here is a single thread, obviously there's multiple of these per core, and all of them are going to get the same control signals. Once since. The decoder is just shared between the core. ~~Um, ~~and now you can see how the execution of a thread is happening with the control signals. And you can see the familiar elements from the diagram above.

So you have a register file, you have the ALU, you have the LSU, and you have the PC. ~~Um, ~~and this is ~~kind of ~~a standard CPU stuff, but the general flow of what you're seeing is you have the register file. ~~Um, ~~you have the ability to access to registers. ~~Uh, ~~from the register file, which are called the source and transfer registers.

That's why they're called RS and RT. And those are also like they're in our ISA and using those registers. There's a ton of different stuff you [01:24:00] can do with it. And so the job of the decoder is to tell~~ the thread, like, sorry, the, the, like~~ the compute recess is dedicated to thread at any given point in time.

What stuff am I supposed to do right now? And so it's going to basically do that by turning off and on different parts of the compute unit. ~~So, ~~for example, if you look in the ALU,~~ you see, like, ~~let's just focus on that one unit. So you see the arithmetic unit, and that can do four different things. So we know from our instructions that the arithmetic unit in the ALU needs to be able to do addition, multiplication, subtraction, and division.

And those are going to be, like, literally four separate hardware circuits that do each of those things. And so now the question is,~~ um,~~ the arithmetic unit is thinking in these two values, right? It needs to perform one of those computations on it, right? So what it's going to do is it's going to take in this control signal, the ~~um, ~~ALU arithmetic multiplexer, which is a much shorter multiplexer, and that's going to tell it, hey, so actually what it's going to do is it's going to do all four at the same time.

It's going to both multiply, add, subtract, and divide all of them. And it's going to divide those four outputs [01:25:00] into this thing called a multiplexer, which is just like a signal chooser. And so now you have all these possible values it could choose. Now this multiplexer value sent by the decoder is going to say, hey, which one should I actually take?

So let's say we did like an addition instruction. The decoder is going to set this,~~ um,~~ mux value to zero, which is, we'll say that the thing associated with addition, and now that multiplexer is going to take these four inputs, just going to output the one specified by division,~~ uh,~~ addition, and that's going to come out into the ALU output mux.

And then here's another multiplexer just to,~~ like,~~ be exhaustive with the design. So now you see, like, okay, we have the output from the arithmetic unit. Then again, there's also going to be an output from the comparison unit on every single cycle. So it's not just, like, we're only performing the computation done by the things specified by the instruction.

Actually, all the computations are happening because they're just in wires. So they're all just connected up, all the wires are always connected. The question is, which computation are we actually taking this time? So the ALU output multiplexer is going to choose Hey, on this instruction, it should be set to 0, because we're going to take the arithmetic unit to output this [01:26:00] time, and that's going to get outputted, and then that value, you can see,~~ um,~~ in the rest of the design, most importantly, that's going into the register input multiplexer.

And so just to finish this part of the flow,~~ like,~~ The register input multiplication is going to be zero this time, and it's going to say, Hey, we got some value from the ALU, and we actually want to use the ALU value this time and store it back in the register. So you see ~~like, ~~okay, we're choosing the ALU output, and then that's going into the destination register, which is what RD is, and we're going to save that back into the register file in the registry specified by the instruction.

And so now you see, okay,~~ well,~~ that's actually a full loop, for example, with the add instruction, like it's basically. Computing the addition, choosing to,~~ um,~~ output that addition from the ALU, and then choosing to store that output back in the register file. And ~~that's, ~~that's really ~~how you, ~~how you get the addition,~~ um,~~ the addition value.

And so similarly with the LSU, pretty simple. So you have control signals to enable read a device, and when you set those signals, and everything else is going to be off those times, as specified by the decoder,~~ um,~~ it's going to make a request out to the memory controller. The memory [01:27:00] controller is going to make a request out to memory, and it's going to type it back.

And this LSU is gonna,~~ um,~~ It's going to be in a waiting state and the scheduler, which we talked about before, is going to see that this thread's LSU is still waiting, and it's just going to keep waiting until the LSU gets a response from memory. And then the last thing which I'll cover is the PC. ~~Um, ~~so if you go over to the program counter unit in the top right.

So this is the stuff I was talking about before,~~ um,~~ with the whole branch and compare instructions. So generally, the next program counter is just going to be the next line of code, which means we just want to add one to the current program counter, pretty straightforward. However, if we're on a comparison instruction,~~ uh,~~ if you scroll up a tiny bit to the,~~ like,~~ MZP register,~~ um,~~ so if we're on a comparison instruction, we are going to actually,~~ uh,~~ def the MZP register.

And that's going to tell us,~~ like,~~ hey, the comparison we just did, it has these MZP values. ~~Like, ~~it was either a 0 or a positive. Then on the branch instruction, It's going to use that NZP tester. And you can actually see the NZP signal coming in from the instruction that we set before. And what that's going to do is basically check, [01:28:00] Hey, did the comparison instruction match this, ~~like~~ NZP, like the set of NZP values?

If it does, then we're going to jump to that immediate value that's tried by the instruction. ~~So, ~~again, you don't really need to understand exactly what every single control signal is doing. If you want to, you can look at the diagram and it will become much more clear. More clear than my explanation. But ~~I think~~ the important thing is that you understand generally that, Oh, this is the layer where actually the instructions are getting literally translated into hardware signals in order to terminate the flow of How the thread gets executed, how the program counter gets updated,~~ um,~~ and how register values and global memory data values get updated.

And that's basically how the entire thread gets executed, like in the kernel. ~~Um, ~~and if you remember in the register file over there, there's those three special values which give us context on where we are in thread execution. That's getting set by the core. ~~Um, ~~And ~~that, that's~~ basically, that's how it turns to execute it.

And this is ~~kind of ~~like the low level of the individual compute of the CPU. And again, it's very similar to a CPU because at this level we have basically entirely [01:29:00] some~~ like~~ similarities to CPUs basically is like a mini CPU here.

Cool. ~~Um, ~~that's really very well done. ~~Um, ~~and if you're listening in audio only mode at this point,~~ uh,~~ and a little confused, definitely, Check out the YouTube or jump straight to the GitHub project and check out the diagram because it definitely will help if anything ~~is, um,~~ is unclear from ~~the, ~~the verbal description.

~~So, ~~okay. ~~U~~


## Visualizing and Verifying GPU Design Through Simulation

~~m, ~~you've designed all this, you've got all the code. We've taken the spike from sort of what you would do at the programming layer, how that gets propagated through the hardware. Is it time to go on to how you actually get to~~ You know, ~~visualize and verify that this is working.~~ Yeah, ~~yeah, we can go to that quickly.

So if you go into the test folder, I'm going to show you quickly how I like simulated everything and then ~~I don't know~~ on the tweet, there's also a video of ~~like ~~what's actually happening in GQ.~~ Um, ~~but yeah, so in the test folder, we can just look at ~~like, ~~for example, the test and that had [01:30:00] kernel. ~~Um, ~~so literally all we have here is I manually compiled all of those,~~ uh,~~ all those kernels I wrote into the.

Like valid machine language for my GPU. So here you see the matrix addition kernel. And then in Python, I wrote this external interface since the memory is external to the GPU design. It's not in the hardware. So I made like a simulator right there that basically simulates exactly the behavior of memory.

On every cycle, it just checks that basically I've requested the memory from the memory controllers. And,~~ um,~~ If there is, it responds with the data. The reason is because memory is not part of the GPU. It's usually like an external DRAM or a,~~ uh,~~ bandwidth memory or something like that. So you wouldn't really include that as part of the design.

So that's what we're simulating here. ~~Um, ~~in the actual,~~ like,~~ if I actually tape this out with polytape out, there'll be like an external DRAM, similarly. ~~Um, ~~like this, and so we load up the program memory here,~~ um,~~ load up the data memory ~~as I, ~~as I said, exactly like I was talking about there. And both of these are simulated memory.

And then also right there, I set the value a little below for the device control register, telling it to execute 8 threads. ~~Um, ~~and then basically all you do [01:31:00] is, so I have this,~~ um,~~ setup program, and all that does is ~~like, ~~it's actually going to take those memory values and load them in. It's actually going to take the threads and load them in,~~ um,~~ and then it's going to call start, and so it's going to set the start signal to high, and it's going to trigger everything.

And then we have this,~~ um,~~ like little piece of code displaying the data memory just for visualization purposes so you can see what it's starting out as. And then,~~ um,~~ now you're seeing the exact way to interface with this. So you're seeing like, just wait until the GPU's done signal is set to 1. In other words, the GPU says it's done.

So it starts out at 0. We're going to say keep running cycles until the GPU says it's done. And for each cycle, the GPU is going to be processing. And I have this nice piece of code here, which is written in one of the helper files, which is just going to display out state of the GPU. And so what that actually does is it's going to show you every single thread and every single core.

~~Um, ~~what are the registers being read? What are the current register values? What is the ALU output? What is the LSU output? What are like the states of the core? Is it like waiting or is it executing or is it decoding or fetching or whatever? Those are really nice to see for like the control flow and the [01:32:00] debugging.

And I encourage anyone who's really curious to see that. ~~I mean, ~~that's like a sick learning process. Just go ~~like, run the, ~~run the matrix addition kernel. There's ~~like~~ instructions ~~in the, ~~in the repo. And then go look at the log file that gets generated. You're going to see ~~like ~~500 cycles. Like, oh, every single thing that's happening inside the GPU.

~~Um, ~~to execute this code,~~ um,~~ which is pretty fun, but yeah, it's pretty simple. ~~Um, ~~and then I did the same thing for matrix multiplication. And so you can see the whole execution trace. Then you could see at the end, it prints out ~~the, ~~the final data memory. And you can actually see ~~like, um, you could see~~ the final values that have been correctly computed.

And for anyone curious to see if it doesn't want to run it,~~ um,~~ there's a video of it, which is in the tweet thread that will probably be linked here, ~~but yeah, ~~cool.

This is awesome. ~~I think, uh,~~

anything else we want to talk about at the real low level? Otherwise, maybe I have just a couple high level questions to ask~~ to, um,~~ to conclude with. Yeah, ~~I think~~ this is great on the low level for people who have questions DM me or,~~ uh,~~ put an issue on GitHub or whatever. So like already a lot of people have been contributing to the GitHub more than I expected, but yeah.

Yeah,~~ well, I think~~ there's definitely a lot of curiosity,~~ uh,~~ out there about this sort of thing right now, but it's not easy~~ to, um,~~ to go as far as you have. So I'm not surprised at all [01:33:00] that people want to follow in your footsteps. Certainly. I'm one of them. ~~Um, ~~coming out of this project, is there anything that still feels ~~kind of ~~Mysterious to you or, ~~you know, sort of ~~questions you weren't really able to get a good grasp on things you wish you understood better.

~~Um, ~~or do you feel like you have it all, ~~you know, ~~reasonably well understood? Yeah. So I think I got basically my goals on it and my goals with anything learning wise in tech, like in a technical capacity is usually,~~ um,~~ not necessarily to be like super niche deep in every single area. Cause honestly, ~~like.~~

Is this an infinite time going deep in any engineering discipline? It's more so to get to a level where I understand the entire landscape from an ~~engineering and~~ engineering standpoint. I have all the key intuitions, and I'm actually deeper than most of the people who are just going in for like an entrepreneurial engineering goal.

So ~~like, ~~I don't want to be able to spar with the engineers and anything,~~ um,~~ and like fully understand everything they're talking about. But then I'm mostly ~~entrepreneurial motivated, ~~like entrepreneurially motivated in terms of, obviously, in this case, there's not really much of an entrepreneurial opportunity.

~~Like it's ~~It's like a super Lindy industry. It's like, I'm not going to go compete in GPUs or something, but it's just a helly how I approach [01:34:00] technical things. ~~Um, ~~and so I feel like I got to the level of intuition where I can now understand anything I need to. And I put at the bottom of the repo, read me like some of the more interesting,~~ um,~~ more advanced GPU, the concepts that I looked into that I didn't implement.

~~Um, ~~so that was fun. Yeah, generally I think I accomplished my goals. ~~Like, ~~I don't think I would want to spend the time to go super deep into any one of these things, unless I wanted to be. It must happen to be interesting to some frontier problem where it's actually useful to go into those. ~~Um, ~~but that's generally how I think about it.


## Reflecting on the Chip Industry and Future Innovations

What do you think this tells us, if anything, about the future of the chip industry? I feel like,~~ you know, ~~there's a lot of debate obviously around ~~like, ~~is Nvidia going to take over the world? Is AMD going to make a comeback? ~~You know, ~~why is like TSMC stock not up nearly as much as the chip designers. And,~~ you know, ~~I feel like somebody might say, geez, you made it pretty far in two weeks.

If you were actually to try to go manufacture something, you wouldn't make it nearly as [01:35:00] far in two weeks. That would seem to suggest that there's something a little out of whack where the, like, why is all the value accruing to the design side, as opposed to the actual manufacturing side? But what's your take on that?

If any coming out of this experience? Yeah, I have my own opinions, but I think my opinion is so far from being credible and experienced enough to have a useful take. We're saying the one thing I'll say is that I don't think there's anything wrong with the value accrual to like people with massive moats.

~~I mean, ~~it makes sense, especially like this late on. ~~I mean, ~~it's such a Lindy industry, I understand,~~ like,~~ I think for people curious about that stuff, I would say just read Seven Powers, and Seven Powers will just explain, ~~like,~~ why modes make sense, and why,~~ like,~~ even though I did this in two weeks, realistically speaking, you can't do anything to,~~ like,~~ challenge these people in most cases, and ~~like, ~~again, disruptive innovation is the place where you get the challenge.

incumbents, but ~~like, ~~that's not really going to happen much here. And the incumbents are also very competent. Like NVIDIA and TSMC. It's because it's such a well incentivized industry that like, [01:36:00] the incumbents can't possibly become incompetent because of how incentivized it is across all this. They're basically driving the world to semiconductor industry.

~~Um, ~~So ~~I think~~ it's definitely challenging and there's also like a lot of takes again, like I can't claim to know about if you can challenge CSS here in video, but~~ like~~ a lot of employees in video, for example, there's ~~like ~~the one viral tweet the other day where the guy you just saw in video was like, now that I've left a video, I can confirm that you're not catching up to them within the next 10 years.

~~So, ~~and ~~I mean, I would, ~~I would think that those are probably pretty accurate, given the nature of the industry and ~~like~~ the economics of it.

It sounds like it's definitely a steep hill to climb. I think one thing that's really interesting, I'll shout out one company here,~~ um,~~ they don't need my shout out at all, but like it's called Atomic Semi,~~ um,~~ and I think that is probably the coolest attempt at doing anything in this industry in the past 20 years.

It's this kid, Sam Tanouf, who's ~~like, uh, ~~built a semiconductor fab in his garage, and now he's trying to build cheap, affordable semiconductor fabs for ~~like, ~~initially ~~kind of like ~~the mid market, like the FPGA market. And there's not really an incumbent there. Like basically nobody has ever done it before.

The question is not like, can [01:37:00] you beat the incumbents? It's just ~~like, ~~is it possible to create it? ~~Um, ~~if he succeeds there, he's going to create a gigantic mid market. It's kind of like what we were talking about here, where I was like, Oh yeah, hobbyists knew this stuff, but ~~like. ~~Realistically, like most people, if you want to hit rocking scale, you just have to hit the incumbent, you just have to use the incumbents.

I think this is something where, because he's tackling down market at first, he's actually legitimately creating a new market opportunity if he succeeds. ~~Um, ~~so I think that's the coolest attempt in ~~like, ~~in terms of this market, trying to do something. That will ~~make a,~~ make an impact on the young person.

And the value there is custom designs for relatively, like comparatively low end use cases.~~ Uh, ~~it's not even that. So it'll actually scale probably pretty far, but it's more like a current fabric costs like 10 billion. And if you want to use them. You have to like ship off your stuff and wait ~~like~~ a long time to get back test samples and then ~~like ~~there's also the FPGA market, which is a lot faster, but you don't actually get like a real design.

It's like that PDA and basically what we're doing is creating fabs that are like way cheaper, like on the order of hundreds of thousands instead of billions of dollars. [01:38:00] And you can get your designs immediately because you just buy a fab and you just ~~like ~~have it with you. Which is first of all, very obviously going to completely change the private market.

~~Um, ~~but eventually it may actually replace down and mid market opportunities, which are actually pretty big in terms of ~~like, ~~you don't even need to go to the huge foundries. You can just use these things, which are way more price efficient. ~~Um, ~~so that could be huge. Yeah. Fascinating. So the idea there would be like enterprises would run.

Their own small fab in the same way that today they might run their own cluster or they could go to a cloud provider in the future. They might run their own fab internally because it's been ~~sort of ~~modularized to the point. Exactly. Yeah. Fascinating. Yeah. ~~Um, ~~do you have any thoughts? One of the paper that has really caught my eye recently was the Microsoft 1.

58 bit paper where basically they showed that you could implement neural networks without.~~ You know, ~~there's obviously been a ton of work in like quantization of the values within neural networks, right? We go from, ~~you know, ~~full, [01:39:00] long floating points down to smaller and smaller bit resolution. ~~Well, ~~the smallest that seems to have been demonstrated to work so well so far is this 1.

58 bit, which is just minus 1, 0, and 1 are the only available values in a network. And they still show that,~~ like,~~ you can actually get them to work with that. ~~Um, ~~one of the things they said in that paper was that this opens up a potentially totally different hardware future because obviously you don't need nearly as much complication to just handle, ~~you know, ~~one zero and minus one as compared to, ~~you know, ~~all the math.

~~Um, if you're, you know, ~~if you're doing longer precision numbers, does this give you any intuition for how that might play out in the future? ~~Um, ~~Yeah, so huge is true. ~~I mean, ~~one of the things that people criticize about ~~the big, um,~~ the big,~~ like,~~ measurements of compute power nowadays is flops,~~ um,~~ which is flowing point operations per second.

And that's like kind of the benchmark for compute towers, especially in GPUs nowadays. ~~Um, ~~and one of the reasons they criticize it is because,~~ like, You can just, like,~~ if you have a 32 bit floating [01:40:00] point values, if you just switch those to 16 bit floating point values, ~~you know, ~~like drastically reduce the flops because it just takes less time to perform computations on that size.

And sorry, drastically increase the flops. And that's actually what NVIDIA has been doing. So like they just released their Blackwell. One of the things they've been doing, obviously they've been boosting their flops in many other ways, but their Blackwell now has smaller floating point, like numbers,~~ um,~~ because ML doesn't really need gigantic floating point numbers on my graphics.

~~Um, ~~and so by doing that, just by nature of doing that, it massively boosted the flops and it is actually meaningfully faster for the use cases of less relevant too. And so it's the exact same implication. Just ~~like ~~if you can use ~~like ~~two bit, 1. 5 bit values to stop the flops is going to go off like crazy.

~~Um, ~~and the important hardware thing is ~~like, ~~yeah, in order for that to happen, like what that actually means is that those register values, like in this case, Again, this is ~~kind of ~~what I meant by ~~like, ~~it's a bit simplification if you can explain important things with it. So ~~like, ~~the register values in this case, ~~they're like,~~ they're ~~uh, ~~16 bit register values, right?

They store 16 bits in them. And in real GPUs, they have a whole host of registers. They have ~~like, ~~registers [01:41:00] that store floating point, 16, and 32 bit numbers. They have ~~like, ~~scalar registers, and they also have vector registers. So what this means is like, in the hardware, you would actually have registers that store ~~like, ~~2 bit values or something like 2 bit values.

And,~~ um,~~ that's going to be way faster and that's how it gets implemented in the hardware, but yeah, that's pretty interesting. ~~I mean, ~~yeah, I'm curious. It could be a big simplification in terms of just~~ like ~~a lot of the components too, right? Like you imagine the sort of arithmetic layer that you had.

Where you're saying it's doing addition, subtraction, multiplication, division all the time,~~ like,~~ if you're down to just a much more,~~ uh,~~ limited set ~~of, ~~of logical operations that you need to perform at each given step,~~ like,~~ that can presumably just get a lot smaller too, right? Yeah, definitely. Although I'm sure,~~ like,~~ that's what determines the flops,~~ like,~~ increasing, but I'm sure we're grossly,~~ uh,~~ oversimplifying a lot of the things, because I bet,~~ like,~~ you wouldn't actually just have just 2 bit floating point,~~ uh,~~ registers in your whole GPU, so there's probably a lot of complexity to it, but as a high level [01:42:00] situation, I'm sure this is generally valid.

Okay, cool. ~~Um, ~~That's all I've got. Anything else you want to talk about?
# Fireworks Ai 


## Introducing Fireworks AI: Pioneers in the Compute Revolution

[00:00:00] Lin Chao and Dmitry Ivchenko, co founders of Fireworks AI. Welcome to the Cognitive Revolution. Thanks for having us. Yeah, I'm excited for this conversation. You guys are in a super interesting business, which I will confess to not knowing a ton about.


## The Business of Compute: Challenges and Innovations

[00:00:15] You provide primarily inference compute. And ~~I think~~ people, ~~you know, ~~broadly are well aware of the fact that compute is one of the hottest commodities in the world today and don't need to look any farther than Nvidia stock price to get a sense for how high the demand is for compute. ~~Um, ~~I also hear speculation that it's ~~like~~ a tough business to be in because ~~you know, ~~commodity businesses long term can be tough.

[00:00:38] ~~Um, ~~and then I also know that there's ~~like, ~~A lot of low level execution details that really matter in businesses like these. And I'm super interested to learn more about some of the close to the metal work that you're doing. So maybe,~~ um,~~ to start off,~~ I want to~~ just give us a ~~kind of~~ quick intro to fireworks AI, ~~like~~ how you guys got the idea to start the business and,~~ um,~~ what your big picture vision is for it.

[00:00:59] Yeah, [00:01:00] definitely. ~~Uh, ~~so I think this is a ~~very, um,~~ very interesting question about,~~ uh,~~ Hey, it's inference support, ~~like ~~provider, a low margin commodity. ~~Uh, ~~so~~ I think~~ there are different ways to answer these questions. ~~So~~ first of all,~~ um,~~ reselling hardware is a low margin business. ~~Um, ~~I still remember when we just started, we were brainstorming all kind of different ideas and we did notice a demand that,~~ um,~~ because of GPU shortage, GPU arbitration could be,~~ uh, something interesting,~~ an interesting problem to solve.

[00:01:27] And we decided to stay away from that because ~~it's. ~~Indeed, as you said, it's ~~a~~ low margin and it's not a sustainable business. I have also seen artificially manufactured pricing,~~ uh,~~ from,~~ uh,~~ highly competitive landscape. ~~Uh, ~~and there's no way,~~ uh,~~ those provider can build a sustainable long term business.

[00:01:43] And ~~I think~~ at least at the minimum, people need to take caution building on top of such that as when these companies or startups run out of funding. They will disappear. 


## Fireworks AI's Vision: Low Latency, High Quality, and Sustainable TCO

[00:01:52] One of the important thing we want to build fireworks on top of is like focus on our specialty based on our [00:02:00] experience. ~~Uh, ~~and here when we think about JNI,~~ right,~~ so it is going to empower a whole slew of application and product disruption, particularly being consumer, prosumer and developer facing.

[00:02:12] The fundamental reason is,~~ um,~~ this is a, New revolutionary technology that didn't exist before that can generate content emulating what human can generate. ~~Um, ~~and by definition, the receiving part of this content are by and large human. ~~Uh, ~~and ~~those ~~for those B2C application,~~ um, you know, ~~Latency is very important part of part experience because it has to be hyper interactive without that interactiveness.

[00:02:37] It's not a viable product. So many of our customer come to us for extremely low latency requirements. At the same time, the content generated found those. Providers has to be high quality and we provide high quality through automated loop across fine tuning and inference. And last but not least, we provide low TCO in a highly sustainable [00:03:00] way.

[00:03:00] And here, low TCO is very important because it's. A different business from,~~ um,~~ traditional application development were built on top of commodity cpus. The gross margin is very high because cpu is so cheap and now shift towards gpus and gpu, not just the hardware expensive. It is very power hungry. It consumes a lot of power.

[00:03:22] ~~Uh, ~~and the general other heat and traditional air cooling doesn't work. People have to use liquid cooling or immersed immersion cooling. That means put the GPU inside oil,~~ uh,~~ and fully immersed. And those are all cost of operating and Jenny I inference. So that very high cost make. It's very challenging to justify business impact, and we specialize in,~~ uh,~~ reducing total cost ownership.

[00:03:51] ~~So, uh, ~~so ~~if, ~~if you have a viable product, it can turn that into a viable business. So that's ~~kind of ~~the,~~ uh,~~ the value add we have been,~~ um,~~ focused on delivering from Fireworks site. [00:04:00] 


## The Competitive Edge: Quality and Efficiency in AI Inference

[00:04:00] In terms of product, A quick overview, we provide the general AI platform to do fast experiment iteration and inference production scaling.

[00:04:09] ~~Um, ~~so here there are two development loops we're optimizing for. In the loop product experimentation, we optimize for iteration speed and auto loop production. We optimize for hard system metrics, including latency, TCO, scalability, reliability, I just mentioned. The specific feed product feature. On these two loops are fine tuning and inference with on demand serving and automation.

[00:04:35] This is for inner loop fast iteration of experimentation. And we provide a fast inference at scale for the outer loop. When you have product market fit, you want to scale a business. And this outer loop of production will help you to get the best speed and best TCO. So that's ~~kind of ~~the very high level, ~~not, um,~~ summary of fireworks product.

[00:04:55] Cool. Okay. Several threads there that I want to follow up on. 


## Sustainable Business Models in AI: Beyond Subsidizing Costs

[00:04:58] One [00:05:00] interestingly, it sounds like you're ~~sort of ~~saying that a lot of products on the market today are ~~kind of ~~in an Uber moment where you think they're essentially being offered below cost. And~~ in a, ~~in a fundamentally unsustainable way. And ~~so, and by,~~ by contrast, I understand that you are,~~ um, like ~~operating your business without doing that.

[00:05:20] ~~You're not, ~~you're not ~~like~~ radically subsidizing the customer. Do I have that correct? ~~Uh, ~~that's correct. But also I just want to call out our value add is not extremely low cost. Our value add is low latency, high quality, and low TCO. So I'm saying ~~kind of ~~low TCO is a byproduct of our high performance.

[00:05:40] Yeah. ~~I think, I mean, ~~this is a real, I've experienced this,~~ um,~~ in my own application development where, ~~you know, ~~TCO is not ~~the, ~~the natural way that a lot of, ~~you know, ~~Engineers think of things and they specifically,~~ like,~~ don't tend to factor in the cost of their own salaries as they start to build out infrastructure.

[00:05:57] ~~So, uh, ~~I am a big believer in certainly the [00:06:00] specialization of dedicated infrastructure providers,~~ um,~~ just because I've seen how hard it is to create a, ~~you know, a~~ reasonably reliable stack when you're doing it on your own. ~~Um, ~~but~~ it's in the, I mean, Just on a, you know, purely kind of, ~~where are we in this market development cycle and, ~~you know, ~~where are things headed?

[00:06:15] ~~It's a,~~ it's an interesting observation off the bat that some of these bargain, ~~you know, the, ~~the cheapest options that are out there are,~~ um,~~ subsidized in an unsustainable way. ~~That is actually, it's not something I had, ~~I know ~~that ~~that's happening a lot at the application layer. ~~I had not, uh,~~ cause certainly ~~like, you know, ~~people are offering free demos only, ~~you know, ~~that's obviously subsidized, right?

[00:06:29] Cause all the tokens are costing money ~~and, ~~and people are certainly giving away a lot of free accounts and a lot of free inference to their end users. But I hadn't really considered how much that might be happening at the. Inference compute layer. So ~~it's, ~~it's really interesting to consider ~~that ~~that is also a reality in today's world.

[00:06:47] Yeah.~~ And a lot of, ~~a lot of our customers, whether they're developers or enterprises come to us, not because we are the lowest pricing provider at all. They come to us because ~~they,~~ again, they're building consumer, prosumer developer [00:07:00] facing applications that requires very low latency and they cannot get it by themselves.

[00:07:04] They ~~cannot ~~not get it from any other. Providers,~~ uh,~~ even from opening and topic,~~ um,~~ they didn't get the right latency or latency is not stable. ~~Uh, ~~and they are seeking solution from our side,~~ uh,~~ into getting to low latency. It's actually not easy and Dimitri can speak a lot to it today, but the high level challenging is,~~ um,~~ Gen AI model is among the largest model sizing and complexity in the whole spectrum of machine learning.

[00:07:34] ~~Um, ~~in early days of machine learning, the algorithm is extremely simple, it's tens of megabytes, and now we're talking about the tens of billions of parameters. ~~Um, so, um, because of that complexity. Um, ~~but ~~with~~ that complexity, it doesn't change the nature of all these B2C,~~ um,~~ applications, whether built on traditional machine learning, or built on top of Genii.

[00:07:52] It doesn't change the latency requirements. It has to be, ~~stay~~ extremely interactive. And that put a lot of Back pressure [00:08:00] on the inference,~~ uh,~~ serving tier ~~to, uh,~~ to do even more aggressive optimization. ~~Uh, ~~and that's ~~kind of ~~the challenge. You are, we are ~~really, ~~really good at addressing. ~~Um, ~~and ~~I think ~~that's our biggest value add,~~ uh,~~ in addition to pricing.

[00:08:12] I don't think pricing,~~ uh,~~ in the long run is a sustainable value. Yeah, makes sense. Okay, cool. So I want to get into then,~~ um,~~ how you're doing it to the, ~~you know, ~~the greatest degree that you can share and that I can comprehend because I do think this stuff is going to get ~~very, ~~very into the weeds as we get close to the metal.

[00:08:29] Do I understand correctly that you are? Managing your own servers on racks. ~~I mean, you're, ~~you're talking about cooling and all this sort of stuff. So are you vertically integrated to that level? Yeah. 


## Deep Dive into AI Hardware: Navigating the Landscape

[00:08:40] So that's a good segue to talk about,~~ um,~~ our compute stack. ~~Um, ~~and we currently, ~~we ~~build on top of CSPs.

[00:08:47] ~~Uh, ~~we're running on top of AWS, GCP,~~ um,~~ and Oracle OCI. ~~Uh, the, ~~the reason is,~~ uh, I think~~ when we grow bigger, there are various different way to be more efficient. And right now we are optimizing for velocity of our [00:09:00] product development. And,~~ uh,~~ those CSPs has been battle tested. ~~Um, so, ~~so that's why we built on top of them.

[00:09:06] And,~~ uh,~~ we also, as a company, ~~we ~~aspire ~~to, uh,~~ to run on top of the best hardware across the whole entire industry. ~~Um, ~~and of course it's ~~kind of ~~the. Easiest to build on top of NVIDIA GPUs. And that's how we started. ~~Um, ~~but at the same time, we see a lot of emerging hardwares coming,~~ uh,~~ to this hardware landscape for JDI, including MD, including Intel, including custom ASICs.

[00:09:30] ~~Uh, ~~so there are various different interesting trade offs, ~~I would say. Um, ~~we'll love to ~~kind of. ~~Pass on to Dimitri to talk about,~~ uh,~~ the trade offs across those different hardware providers. Sure. Yeah. ~~Um, ~~so as Lynn mentioned, historically,~~ uh,~~ we've been primarily dominated by NVIDIA in the,~~ uh,~~ overall AI landscape.

[00:09:47] And the reason for NVIDIA domination is, ~~I would say kind of ~~twofold. ~~So~~ first is they have pretty good hardware. And if you look at the latest H100, it has two petaflops. This is~~ pretty,~~ pretty high, and they are pushing [00:10:00] with a new,~~ uh,~~ Blackwell to,~~ uh,~~ double that, and then even go to 10 petaflops for their superchips.

[00:10:07] And they also are doubling, quadrupling,~~ uh,~~ memory,~~ uh,~~ bandwidth along the way. ~~Um, ~~they're also improving on their,~~ uh,~~ cross host interconnect. And ~~I think ~~the most welcome development there is,~~ uh,~~ the actual latencies, which will allow us,~~ uh,~~ to,~~ uh,~~ of interconnect, which will, in turn, will allow us to reduce the latencies of our,~~ uh,~~ generation speed from the,~~ um, That's, ~~that's one.

[00:10:29] But the second thing is that NVIDIA historically has had a very robust developer stack. ~~Right. ~~And,~~ uh,~~ because of ~~the, of~~ these two reasons,~~ uh,~~ I think V has been dominating, but,~~ uh,~~ lately,~~ uh, the,~~ I'll say,~~ uh,~~ Nvidia AMT is ~~coming, ~~coming back, ~~and, uh,~~ and then now with the new,~~ uh,~~ MI 300, which has,~~ uh,~~ better hardware back than Nvidia,~~ uh,~~ and they are also.

[00:10:50] Working,~~ uh,~~ I'm sure day and night on their software stack and for the new welcome open source development on the Oracle stack,~~ uh,~~ they are catching up ~~or~~ basically in ~~all, ~~all aspects,~~ uh, uh, ~~to it [00:11:00] and media as well. We also see other,~~ uh,~~ newcomers, whether it's development from Intel with the Gaudi two or company, the Audi three release, and which is actually even more powerful than MIT 300.

[00:11:11] So it ~~kind of ~~sits in between,~~ uh,~~ H100 and B,~~ uh,~~ 100, B200,~~ uh,~~ GPUs. So that's like on the more programmable side of,~~ uh, uh, ~~things. And now if you look at the different spectrum, the less programmable, more specialized hardware,~~ uh,~~ namely ASICs. So here I would probably just select one is,~~ uh, uh, ~~GROC, which,~~ uh,~~ has been making a bit overused lately on Reddit,~~ uh,~~ because of the,~~ uh, Uh, ~~nice demo, the high generation speeds.

[00:11:36] ~~Uh, ~~but,~~ uh, the, ~~the thing is that,~~ uh,~~ access always compromise on something. So in here is that if you look at the graph, and surprisingly there is ~~kind of ~~very little ~~kinda~~ detail and ~~some,~~ sometimes you need to guess~~ like what, ~~what these guys do. 'cause they're not as open ~~as, ~~as~~ in~~ Nvidia. But what they're fundamentally doing, they,~~ um, uh, ~~compromising ~~on the, ~~on the fact that they wanna,~~ uh,~~ remove the shared memory of this HBM in, in GPUs.

[00:11:57] And they wanna put it as close new as possible. They wanna [00:12:00] put it on a d. But then they are compromising ~~on the, ~~on the processing units. So they have achievable flops are lower.~~ Uh, ~~they also, this memory is very expensive because putting anything on die is way more expensive than having a memory shared across,~~ uh, uh, ~~units.

[00:12:13] And now what the result ~~is, ~~is that,~~ um,~~ they have much lower,~~ uh, achievable, ~~achievable,~~ uh,~~ flops. What they can do faster, they can,~~ uh,~~ run the,~~ uh,~~ generations. Yeah. Faster because they don't need to copy memory from the shared memory to the memory, ~~which is very,~~ which is on time. So this is like fundamental,~~ uh,~~ come from a table, and they're also way more expensive to operate because,~~ uh,~~ if you want to host a single model, you need to have a humongous set up, which costs millions of dollars.

[00:12:43] So ~~I think~~ these are going to come from us in the end, although,~~ um,~~ it's very interesting and a great school demos, but ~~we practically can talk about this.~~ You can practically see a limited application of this in the real world. And so the limited disruption, although it does solve some interesting cases, but they seem to be more of edge cases [00:13:00] right now, where it wins over traditional programmable GPU hardware.

[00:13:05] ~~Uh, ~~there's also TPUs, of course, there has always been a case,~~ uh, there will be,~~ there has always been around and they are setting out ~~kind of ~~from programmability between ASICs and GPUs,~~ uh,~~ although. Technically, PyTorch supports TPUs, but to get the best performance, you have to go to JAX ~~and, ~~and ~~Google, uh,~~ Google's Vault and Google's Southwest stack.

[00:13:20] So it becomes ~~like~~ a quite different,~~ uh,~~ operational model, quite different business to operate. So that's ~~kind of ~~in a nutshell. Yeah. So speaking about that, ~~right. ~~So you can see it's a spectrum, it's a spectrum from most programmable to ~~like~~ hyper specialized. 


## From Meta to Fireworks: Lessons in AI Development

[00:13:35] ~~Um, ~~and I want to talk a little bit about our Meta experience, ~~but~~ because both of us and actually a large portion of the funding team came from Meta and we all worked on PyTorch,~~ uh,~~ extensively,~~ uh,~~ over the past five years.

[00:13:46] So it's very interesting,~~ um,~~ experience there. Of course, as you can see, ~~a~~ Meta like other hyperscalers,~~ uh,~~ running on top of CPU, GPU, ASICs,~~ um,~~ this is a public information, a variety of hardware. And recently they mentioned,~~ uh, they are,~~ they deployed. ~~Uh, ~~more than 600, [00:14:00] 000 in house and ~~that~~ what does that mean?

[00:14:02] ~~Right. ~~Put that in perspective. That's equal to the power needed for,~~ um,~~ 600, 000 average American household. That's roughly twice the size of San Francisco.~~ Uh, ~~huge power consumption, but matter didn't get there. ~~Um, ~~Overnight,~~ uh,~~ it took us more than five years to go from basic machine learning on CPU to complex deep learning on GPU and A6.

[00:14:23] So there are a lot of interesting lessons learned. ~~First is Uh, it's~~ because we work on software stack, right? So the first lesson learned is a good product cannot compromise and need to be opinionated about~~ the,~~ what's a part of philosophy and ~~the,~~ what's the target audience. So no matter when we start to work on,~~ um,~~ diving to,~~ uh,~~ AI infrastructure, we had at least three different AI frameworks.

[00:14:45] That's in 2018,~~ uh,~~ we have Coffee2 for mobile, Onyxx for server production. So our charter is to unify them into one and cover both server, mobile, research and production. It's called PyTorch1. This feels like mission impossible at the moment,~~ uh,~~ because it has so many different [00:15:00] goals. ~~Uh, ~~so we merge all these teams together~~ and, uh,~~ but there's no consensus how to build this one framework.

[00:15:06] So we came up with a. Idealistic zipper approach and the project was actually literally called zipper taking the pytorch front end, which is very easy, simple to use and zip it with coffee to back end, which is highly performant. It failed miserably because these two frame was never designed to work together.

[00:15:23] The integration overhead was more than writing a new framework from scratch. So~~ we kept,~~ we end up ditched that plan and we kept the PyTorch front end and rewrote this backend into a Torch script. And that's an interpreter to execute PyTorch efficiently. So notice that the design decision, the product choice we made is.

[00:15:43] To hold a line for ease of use, hold a line for ease of AI innovation,~~ uh,~~ for developers built on PyTorch. ~~Uh, ~~and then we,~~ uh,~~ take all the complexity of building the backend. So that is the design [00:16:00] decision.~~ Uh, ~~however, TorchScript. ~~Right ~~for PyTorch 1. 0, it requires the user, the developers to annotate which part of PyTorch code is scriptable.

[00:16:08] That's not a very good UX because people need to know how to annotate. So two years ago, we also started Torch Compile,~~ um,~~ to fully automate the process. People don't need to annotate at all. ~~Um, ~~so that's called PyTorch 2. 0. We left before the project fully shipped. But I'm thrilled to see that there's great progress made,~~ um,~~ from the PyTorch team.

[00:16:29] So another interesting takeaway we had in that process is we thought it should be easy to bring PyTorch to production. We thought the process is just ~~kind of ~~swap the libraries. ~~So~~ because both PyTorch and Coffee2 and Onix, they're all, they're just library, they're not services, swap those libraries in the service.

[00:16:46] However, that's a wrong assumption. ~~A framework innovation.~~ A framework, a library innovation requires a completely new infrastructure service to build, to support it. We end up have to build new data loaders, new data [00:17:00] transformer, transformation layer for training, for PyTorch. We need to build a new training loop for PyTorch.

[00:17:05] We need to build new distributed inference stack for PyTorch. So after five years, we wrote a whole entire PyTorch platform from ground up. ~~Uh, ~~it was serving more than 50 trillion inference per day across 50 data centers.~~ Uh, ~~so as you can see, this journey took us five years, ~~right? So our, um,~~ but we start fireworks.

[00:17:22] We want to reduce, we want to shrink these five years journey into five weeks or even just five days for,~~ uh,~~ current broader set of developers in the industry.~~ Um, ~~we have built better tested large scale. Yeah, systems. So we're confident that we can all innovate the incumbents and significant shortened time to market for everyone out there.

[00:17:44] I want to build,~~ um,~~ you disruptive applications and products on top of Jenny. 

[00:17:48] So, if I try to summarize that and ~~kind of ~~make the translation from the meta experience to the fireworks product direction. It seems like the [00:18:00] key principles are never compromise on the product user experience above all the users hate to wait.

[00:18:06] I certainly know that from personal experience. And there's ~~like~~ an echo of that at the developer layer too, like developers hate complexity and, ~~you know, ~~don't want to have to deal with all this mess. So internal focus on the ~~end ~~end user experience above all focus on the developer experience. Second, simplify everything, bring all the complexity in house abstract away from all the different.

[00:18:27] Kinds of hardware and It sounds like ~~the, ~~the place that you want to carve out for yourselves with Fireworks is a sort of layer that sits between the developers and all the different hardware providers so that folks can easily develop their applications, ~~but not~~ and not really have to worry about what hardware they're running on the relative strengths and weaknesses of all that.

[00:18:55] What bottlenecks they're going to hit it at all these different,~~ um,~~ depending on all the different [00:19:00] stacks. ~~And I mean, I guess where I ~~tell me if that's right, first of all, and then I'm very curious to get into a little bit more detail on maybe what some of those bottlenecks are. ~~I think people have a sense that I think we maybe should give some basics.~~

[00:19:08] ~~Like, I'm, ~~I'm like pretty rudimentary in my GPU knowledge, but I'm learning. And ~~I think ~~the audience will be, ~~you know, ~~pretty varied in terms of how,~~ uh,~~ much command they have of this stuff. ~~So, ~~first of all, do I have that general story and kind of market position and vision, right? Yeah, so ~~I think~~ it's mostly right.

[00:19:25] ~~I think~~ a little bit more nuanced is what is getting the way of the,~~ um,~~ fast iteration loop here. We're talking about current set of application product developers. They haven't jumped onto AI yet. ~~Right. So, um, ~~and they have a slew of AI tools they have to learn,~~ uh,~~ and the pick and choose different models for their use cases.

[00:19:45] And. I'll also try to optimize for latency and try to justify business impacts through low TCO. All of those are on their plate right now. And our goal is to ~~kind of ~~take away,~~ uh,~~ those concerns, let them focus on where they should be focused [00:20:00] on is,~~ uh,~~ application and product development. And then we give them proper tools and a higher level abstraction.

[00:20:06] So they get. ~~Uh, ~~low latency, low TCO, high quality extremely easily. ~~Um, ~~of course it sounds really,~~ um,~~ nice,~~ uh,~~ and ~~we, ~~we can dive a ~~lot, ~~lot deeper ~~into, ~~into how we get there. ~~So, ~~but I, at the high level, I will break it ~~at least~~ into two buckets. One is low latency, low TCO. That's a bucket. We should dive.

[00:20:22] Deeper into that's driven by our high system optimization, a performance optimization. The other bucket is quality. And we have to talk about quality because at the end we think ~~we are,~~ our competition are not other inference provider. Our real competition is actually open AI and the topic.~~ Uh, so, ~~so solving and addressing people's.

[00:20:42] ~~Like~~ quality issue is,~~ um,~~ very high priority of our company goals. Yeah. Okay, cool. ~~Well, ~~those are both,~~ um,~~ really interesting. No, let's maybe start with the quality one. Cause ~~I think that is, um,~~ that's probably the more intuitive one. And I was noticing in trying the product and I always do go in and try products on the, in my preparation for these,~~ um,~~ [00:21:00] Conversations.

[00:21:01] I would say, ~~you know, ~~the experience is super easy to get started, ~~you know, ~~just create an account. Next thing you know, you're in a playground, you can choose from all these models. You've got what you call serverless models, which ~~basically is like on, you know, not, not even, I mean, you also have been on demand, but that's like setting up dedicated compute, um, paying by the hour, but the serverless~~ is literally just.

[00:21:14] A very similar experience to what you get with open AI and anthropic, where you're making an API call, you're purely paying for tokens and ~~you know, ~~that's all super simple. You can test stuff out, try all the different models in the playground and then hit the, give me the code button. And it pops up the code and you can, ~~you know, ~~go copy that code and drop it in your application.

[00:21:32] So all that is ~~like, I would say, you know, ~~probably reasonably familiar to folks in our audience. They've done that kind of thing, at least with an open AI ~~or, ~~or an anthropic, if not, ~~you know, ~~another. Inference provider quality, though, ~~is a, ~~is a tough challenge, right? Because ~~the best models certainly in today's world, you know, ~~with some notable exceptions that are starting to crack into the top 10,~~ um, you know, ~~certainly still the very best models are proprietary to the open AIS and anthropics ~~and, ~~and Google deep minds of the world.

[00:21:57] And notably too, ~~like~~ the price is also [00:22:00] starting to get pretty low from those guys, the,~~ um, I think~~ haiku for Manthropic is like a really interesting point of comparison. The price that you guys have for the small tier of models up to 16 billion parameters. I'm interested to hear how that cut off, ~~you know, ~~was selected, but up to that 16 billion threshold is 20 cents per million tokens, which is crazy to think, ~~you know, ~~not that long ago.

[00:22:23] It was 6 cents per thousand tokens ~~from, um,~~ from open AI with the original GPT three. So we've gone from 6 cents per thousand to 20 per million for better models than the original GPT three in just ~~like. ~~Two years,~~ um,~~ I always ~~kind of ~~like to stand back and just marvel at how fast that cost has come down.

[00:22:44] ~~Um, ~~but the leaders are not too far behind right there, ~~you know, ~~with haiku, anthropic is at 25 cents,~~ um,~~ per million, at least on input. They charge a little more for the output, but with the long context, ~~you know, ~~presumably a lot of the time it is pretty input heavy,~~ um,~~ workload there. So yeah, let's talk about [00:23:00] quality.

[00:23:00] ~~And how, ~~how do you win in a world of,~~ uh,~~ of haiku? I would assume ~~that ~~that's like the number one. ~~You know, ~~direct competitor for those, ~~you know, kind of ~~smallest models. ~~Um, ~~curious to hear how you're thinking about the quality challenge. Yeah, definitely. ~~So, uh, it probably, we can take a big step back, right?~~


## The Future of AI: Open Source vs. Closed Source Models

[00:23:11] So ~~it's, it's more like~~ between closed source vendor and open source vendor. Who is going to win? ~~It's, ~~it's clear that ~~at least we, we can agree that ~~we are currently in a very intense race between open source and closed source models.~~ Uh, ~~this week is an interesting week,~~ uh,~~ Mistral team just dropped a MOE, a new MOE model,~~ uh,~~ with eight experts of 22 billion parameters, and we just enabled it, and MATLAB will open source LLAMA3 in a few weeks, and Google has been continuous to open source newer,~~ uh,~~ gamma models.

[00:23:41] And Q1 and e models from those Chinese institutions are getting better and better also.~~ So, uh, ~~at the same time, OpenAI and Anthropic keep,~~ uh,~~ improving their model quality, including at a smaller model size scale. ~~So here's my thinking, right? ~~So I think all of these models in the same size bucket will converge in quality eventually.

[00:23:59] The [00:24:00] reason is,~~ uh,~~ for smaller models, because of,~~ um,~~ the size, it ~~just, It ~~has the upper bound on how much knowledge it can absorb and~~ it gets,~~ it determines capability. And as ~~you know, ~~we are all also converge on how much data we can train a model. So ~~I think~~ just inevitable over time,~~ uh,~~ whether open source or closed source, the model quality ~~will, ~~will be similar to each other.

[00:24:20] If that's true, and I will argue open source models, Have a much stronger ecosystem potential because ~~a lot more,~~ it has a lot more active people engagement. Developers are engaging in tuning oversource models, and then they open source them and this keeps going. It has compounding effects. So more and more ~~people, ~~people can build on top of each other's work.

[00:24:40] ~~So~~ this is how I'm thinking. So that's why fireworks. Fundamentally build on top of those open source ecosystem. We also just launched our fine tuning service. It's relatively new. ~~Uh, ~~so in terms of revenue,~~ it's not, um,~~ it's not dominating,~~ uh,~~ any of other,~~ uh,~~ product features, but it's one of our fast growing product feature.

[00:24:59] ~~Uh, ~~with that [00:25:00] said, I will still say ~~between closed sourced.~~ Right now we are not there yet. It's ~~like ~~all open source, closed source models, small models are converging right now,~~ um,~~ the open source model and still need fine tuning. ~~Um, ~~and the challenge of fine tuning is,~~ uh,~~ it's a lot, much longer development process than prompt engineering.

[00:25:18] And we fully acknowledge that. And that's why we, as a company, we want to solve those problems to make fine tuning much easier. Faster, easier and actionable,~~ right?~~ Because once you see the result, ~~you see, ~~Hey, what is not working? It's actionable. ~~Um, ~~and also we will by and large automate a lot of this pain in fine tuning away.

[00:25:39] So our developers will have much simpler experience as close to prompt engineering. As possible, so that's one aspect. The other aspect is ~~I think~~ eventually ~~I will say~~ open the AI and thought pig, their goal, including model automation, their goal is to get to AGI, right? What is AGI? It's basically [00:26:00] building a system that's.

[00:26:01] Smarter than human, it means this system can solve very complex problem. Hundreds of them at the same time. But if we look at the problems, developers and enterprises, they are solving, they don't solve hundreds of very complex logical reasoning problem at the same time. They probably have a handful of very specific problems.

[00:26:21] ~~Uh, ~~for example, they want to solve classification problem from. Intent routing based on intent route to, ~~you know, ~~different agents to,~~ um, classify Cal ~~categorize product catalog,~~ uh,~~ nicely to re ranking,~~ um,~~ retrieve result, get top K of the best answers or to do structured data extraction,~~ uh,~~ from images like.

[00:26:44] Extract information from receipts, from medical bills, from insurance policies to paraphrasing emails,~~ uh,~~ for better sales follow up or ~~for, ~~for a better marketing lead generation, and the list can go very long. But as you can see, every single example, as I mentioned here, [00:27:00] they're very specific. ~~Um, ~~so that's create an interesting opportunity for us for, especially for smaller open source models.

[00:27:07] ~~Um, ~~think about model training as a process. Of aligning the model to optimize for a set of objectives. So this is very important framing. ~~Um, ~~because what the model is good at is being decided at the beginning of the training process, how you form the training data set,~~ how, ~~what is a proportion of what kind of training data set you mix together is basically a product opinion you put.

[00:27:32] In what is the capability of this end model, so no model today is going to be good at solving all kind of problem. You have to pick and choose by set the objective at the beginning. So that's a general framing, but you can also,~~ uh,~~ think about it's much easier to align model to solve a specific problem very well, instead of ask the model to solve hundreds of problem very well,~~ right?~~

[00:27:54] ~~So, ~~solving narrow down the objective to one problem. ~~It's ~~it's a much easier [00:28:00] alignment process.~~ Um, so, ~~so that's why in practice, all the practical problem we're seeing today is. ~~Amenable, because it's ~~amenable to ~~small,~~ smaller,~~ um,~~ models because the problems are very narrow and well defined.~~ Uh, ~~and ~~we, uh,~~ we have seen a lot of success using fine tuning to solve those problems and second, almost every single enterprise we talk with, they have data.

[00:28:21] They have data to align a model better. ~~Uh, ~~and sometimes not just on par, even better than GPT 4. ~~Uh, ~~so based on those observations, we're pretty bullish on the direction of continue down to make the feedback loop of quality between fine tuning, inference, data collection, cleansing, this feedback loop very ~~Uh, ~~efficient for ~~our, uh,~~ our users,~~ uh,~~ and ~~we will,~~ again, we will,~~ uh,~~ try to automate as much as possible in this process.

[00:28:47] Okay, cool. I have a number of follow ups there as well. So just speaking to my own experience briefly,~~ I think~~ the general notion that,~~ uh, uh, ~~Fine tuning is, that seems like a really good answer to how do we compete with [00:29:00] haiku,~~ um,~~ because I would agree that, and in fact, at Waymark, ~~you know, ~~my company, we use a fine tuned GPT 3.

[00:29:07] 5 currently to power our core script writing task, ~~the, you know, ~~the number one most important AI function. In the product, we could use GPT ~~for ~~for it. It's not really like a budget thing for us. ~~Um, ~~we have a pretty high value use case. So ~~we are~~ our strategy is use whatever gives us the best results. ~~Um, whatever gives us the best results.~~

[00:29:27] Not just, ~~you know, ~~the best overall user experience, I'd say. ~~And, ~~and ~~the, ~~the quality of the output is probably the number one factor there. Latency also ~~is, ~~is important, ~~you know, ~~as we've discussed, people don't want to wait. And so at the moment we're on a 3. 5 fine tuned model. GPT 4, ~~you know, ~~could probably do the task.

[00:29:43] Pretty well. ~~Um, ~~and ~~we, ~~we wouldn't be scared off by the cost, but it is a little bit slow sometimes. And also, ~~you know, ~~it's a little bit unwieldy. You're trying to prompt engineer your way of all these different, ~~you know, ~~caveats and rules and whatever. And it's ~~like ~~hard to represent all that stuff in the prompt.

[00:29:57] And you could also think, maybe we could use haiku and maybe [00:30:00] we could even put like, ~~Okay. ~~10 examples, ~~you know, ~~into haiku and that could,~~ um,~~ in theory, get it to ~~sort of ~~do the in context learning, but now ~~we're kind of back to a situation also where the, or it's now ~~we've gone up an order of magnitude in price because we're doing 10,~~ um, you know, ~~examples at every prompt, ~~so.~~

[00:30:12] Fine tuning I do think is a really good answer and certainly ~~like, you know, even if companies don't have,~~ as you said, companies have data, but even if they don't, ~~you know, a lot of ~~a lot of companies would probably be very surprised with how little data it really takes to do a reasonable fine tuning our data set.

[00:30:26] is in the three figures, ~~you know, ~~hundreds, but not even thousands of data points. And that ~~like ~~works quite well. Actually, we don't have to have a ~~huge, ~~huge thing ~~for a, ~~for a narrow task. ~~If you're, ~~if you're trying to maintain generality, then you have a much bigger challenge on your hands. But for this one task of, ~~you know, ~~write a script for this business, ~~you know, ~~for this video, hundreds of data points we have found pretty well suffices.

[00:30:49] That's excellent point. Yeah. 


## Fine-Tuning for Excellence: Fireworks AI's Approach

[00:30:51] So ~~I guess ~~tell me about ~~that,~~ that fine tuning product. And ~~this~~ also ~~can~~ maybe get into some of the bottlenecks.~~ It feels very, you know, ~~I looked at the documentation. I didn't actually do a fine tuning [00:31:00] myself, but maybe I'll put that on my to do list. ~~Um, ~~but it is. Very similar to the open AI product where you can ~~like ~~set up your sort of chat records and their Jason L lines.

[00:31:11] And you upload ~~a, you know, ~~a bunch of Jason L lines and run it. ~~Um, ~~you build that by token. Is it accurate to say that it's basically a kind of at the ~~sort of ~~spec level, same thing as the open AI experience? Yeah, this is a great way to summarize it because,~~ uh, we, ~~we are,~~ uh,~~ one of the product design philosophy is to be open AI compatible.

[00:31:30] ~~Uh, ~~because OpenAI has a lot of draw for the initial set of developers to try out ideas. ~~Um, ~~and,~~ uh,~~ the benefit of being OpenAI compatible from fine tuning to inference is it's really easy to migrate.~~ Uh, ~~so even if,~~ um,~~ our developer don't start from us,~~ um,~~ but once they get to stage,~~ Uh, they need, uh,~~ they need ~~kind of, uh, ~~more,~~ uh,~~ interesting fine tuning,~~ uh,~~ that doesn't provide, and they need,~~ uh,~~ low latency and low TCO for,~~ um,~~ for production and they can move to us.

[00:31:58] ~~So, ~~so yeah, you're absolutely right. [00:32:00] And the API will feel very familiar. But on top of that, we're adding also new APIs that doesn't exist. ~~Uh, ~~in openness, that's also our,~~ um, uh, ~~unique advantage, but coming back to fine tuning. ~~Um, ~~yeah, so here ~~we, ~~we started offer a special fine tuning called path,~~ uh,~~ performance, efficient fine tuning,~~ uh,~~ actually found a long time ago, the most popular technique in that bucket is called Laura.

[00:32:22] ~~Uh, ~~Laura stand for low rank adaptation. ~~Uh, ~~so the idea is you freeze the pre trained model weights and inject trainable rank decomposition matrices. Into each layer, so transformer architecture,~~ uh,~~ and the end result is greatly reduced the number of trainable parameters for downstream tasks. So usually~~ like~~ fine tuning, you can think of it as ~~kind of ~~short training, right?

[00:32:44] So you need to ~~kind of ~~go forward backwards and do all this stuff with Laura. Then your base model is only forward and then your additional,~~ um,~~ Adapter,~~ you,~~ you go through the,~~ um,~~ the full training steps. So that's how it saves,~~ um,~~ compute and be very [00:33:00] efficient. And also you just mentioned, ~~you~~ actually~~ don't,~~ you figure out many people are this consistent feedback.

[00:33:04] You don't need a lot of training samples or tuning samples. ~~Uh, ~~typically like around 1000 in your example, just hundreds of them will be sufficient, a compound where the very efficient Laura fine tuning. That means your feedback loop is going to be really fast and that ~~make us~~ make the whole fine tuning process even more appealing,~~ um,~~ alternative.

[00:33:25] So let me spend a little bit of time explaining what LoRa means. So under the hood, ~~it just,~~ it leverages a concept again called rank decomposition. And rank decomposition is basically allow us to represent a high dimensional matrix with a product of two. Lower dimensional matrices. So if the pre trained weight matrix, let's say of dimension N by K, and then it can be represented with a product two matrices,~~ uh,~~ let's call it N by R for the first one, and the second one is R by K.

[00:33:57] So if we [00:34:00] do a multiplication across these two matrices, you will still get N by K, right? So that's the high level idea. And let's make the saving more concrete. N is 2000. K is 5, 000 and R is one for extreme case, just make the point here. So the total of parameters,~~ uh,~~ in the original matrix is 2, 000 by 5, 000, that's 10 million.

[00:34:22] And then if we decompose into,~~ uh,~~ lower rank,~~ uh,~~ then ~~it's~~ the first matrix is,~~ uh,~~ 2, 000 by one. It's 2, 000 and second is 1 by 5, 000 to 5, 000. So the total number of parameters across these two lower rank, lower dimensional matrix is 2, 000 plus 5, 000, 7, 000. So 7 is a significant lower number of parameters.

[00:34:45] Then 10 million, that's the original, which is, so this is more than 1000 times reduction. That's the idea behind why using LoRa to do fine tuning is so much faster. It's not just for faster fine [00:35:00] tuning. ~~Uh, ~~at inference, we can also do something very interesting. ~~Um, ~~so we actually have many customers come to us.

[00:35:06] They need to deploy many Laura adapters, ~~which shared~~ against the same base model. ~~Right? ~~So the naive way to deploy those Laura adapter is,~~ uh,~~ you merge it with the base model and then you deploy this. A hundred, if they have a hundred Laura adapters, you have to deploy models. And all these a hundred models sits in memory.

[00:35:28] ~~Um, we found early on,~~ we are one of the first to deploy many Laura's by sharing the same base model.~~ Right. ~~You can imagine it looks like a tree. There's a trunk that's a base model and the, each law adopters are ~~kind of ~~hanging on the trunk. So by doing this sharing, we can save a lot of costs in production for inference.

[00:35:47] ~~Uh, ~~because for a hundred law adopters,~~ you, you~~ basically originally without the saving, you have to deploy a hundred times and then you just need to deploy the one base model that's dominating the cost. So by that you save a hundred times of the cost. ~~Uh, so. We, ~~we kind of [00:36:00] use LoRa pretty extensively.

[00:36:02] Across both fine tuning and inference, and that's significant increase the velocity of our iteration. Yeah. If you haven't used, try that. ~~Um, ~~I strongly encourage you to,~~ uh,~~ try out fine tuning service. So yeah,~~ I think this, ~~let's just flesh that out a little bit more for people, ~~or maybe I'll take a stab at it.~~

[00:36:15] You tell me if I'm going wrong anywhere, the high level situation,~~ right,~~ is you want to have a model deployed that you can. Get inference from quickly. If you have all your computers turned off, you have the cold start problem of ~~like, ~~okay, I got to boot up ~~a, you know, ~~a Docker container and load, ~~you know, ~~stuff in.

[00:36:34] And then these like billions of parameters take time to move in. So typically most services. are going to try to have some mechanism of not making you wait for a full cold start,~~ right?~~ So instead, what you have when something is deployed is you have a GPU sitting there with the model loaded into the high bandwidth memory.

[00:36:58] Which is to say the second tier memory, ~~right? I, I think, um,~~ [00:37:00] I've gone into this a bit on a previous episode where I dug into the Mamba architecture, but basically ~~you've got your~~ on your GPUs. You've got your many computation cores. There is the. SRAM that is the like highest,~~ um,~~ or let's say ~~the, ~~the lowest latency closest to the computation core RAM, but it's small.

[00:37:18] You can't fit the whole model in there. So you have to have this second tier RAM, the high bandwidth memory, where the actual billions and billions of parameters of the model sit. And then when you're actually doing inference, ~~this is where I get a little bit fuzzy. And it probably depends, I guess, on different setups, right?~~

[00:37:32] ~~But.~~ There, you're ~~kind of ~~paging in parameters from high bandwidth memory into the SRAM for the actual computation, ~~kind of ~~paging them in and out to do stuff. And what you're saying with the LoRa, like the many LoRa's configuration, is that you could, ~~you know, ~~the naive approach as you described it would be to say, okay, I'm going to have a hundred different servers.

[00:37:55] Each one will have its base model and its LoRa. And the Laura is, ~~you know, ~~whatever, 1 to [00:38:00] 3 percent or something,~~ I think~~ as many parameters,~~ um,~~ again, depending on the setup and exactly how you do it. So you could have 100 of those each with the base model and the Laura, or you could have your base model and a bunch of Laura's all sitting in high bandwidth memory on a single GPU.

[00:38:15] And then you just have to manage the,~~ Like, I guess the, you know, ~~the paging in or keeping track of which Laura we're using for which use case that kind of stuff gets a little bit more complicated, but it allows you to save on having to set up all these servers and have them waiting there. ~~So, I guess,~~ what's ~~kind of ~~the next level of sophistication in terms of the analysis there?

[00:38:36] That could be like. ~~You know, ~~what are the bottlenecks? What are the trade offs that you're facing? ~~Like, that's literally just about everything that I know. So, you know, ~~tell me,~~ um, what should I,~~ what do I need to know next, ~~you know, ~~to get smarter beyond that,~~ um,~~ base level description? Yeah. So ~~I think~~ we did a lot of very complicated inference stack optimization to bring down latency.

[00:38:52] As we have discussed in this episode ~~that we,~~ Our hyper focus on latency, but also while we're hyper focused on very low latency, [00:39:00] we also hold the latency bar. We can pump up throughput to very high, and that is a result of low TCO. ~~Uh, ~~I will pass it to Dimitri to talk about,~~ um,~~ All the trade offs,~~ uh,~~ nuances we have put into,~~ uh,~~ the inference optimization stack.


## Optimizing AI Inference: Technical Insights and Challenges

[00:39:14] So I want to hear, ~~yeah,~~ take a step back and try to go over some ~~very, ~~very basic steps of how GNI inference service and what are the key points you should pay attention to. ~~A sense that~~ we have right now, a huge information overload. There's so much information,~~ like,~~ oh, this attach implementation is the best.

[00:39:32] Or this MAMP architecture is the next best thing. Or we need to ~~like ~~run a chart model differently. And there's so many different techniques. But the question still remains,~~ like,~~ what are the actual techniques which really do matter? So~~ I think~~ that's what I want to focus ~~on, ~~on these important points here.

[00:39:49] ~~So, ~~okay,~~ um,~~ now let's say we want to build the,~~ uh,~~ GNI inference. And,~~ um,~~ right now let's always focus maybe~~ like ~~on one or two cases. One is text generation and another is [00:40:00] image generation. ~~So, uh, ~~luckily,~~ uh,~~ the very welcome development is that the new,~~ uh,~~ model from stability ~~is based on the, uh,~~ for the image generation is based on the transform architecture.

[00:40:09] So the old architecture based on the ResNet is gone. And with that, all the convolutions are not as important anymore. ~~So now, we're only talking about the transformers. ~~So all we have to worry about is the transformer now. ~~Um, ~~which ~~is,~~ to some extent, is great, but it has its own challenges. Now, what does it matter for a transformer?

[00:40:25] So in a transformer, I would say there are only two operations which matter. One is the,~~ uh,~~ the most ubiquitous matrix multiplication. And that it's ~~like, you know,~~ all the AI workflows, JDI or not. Matmul is the most important one. And the second most important one is,~~ uh,~~ is of course attention. ~~Uh, ~~and attention is a bit special kind of,~~ uh,~~ Matmul.

[00:40:45] ~~It's a,~~ I would say it's a back to back,~~ uh,~~ batched Matmul. ~~Um, ~~and optimizing,~~ uh,~~ it ~~is, ~~is quite critical.~~ I can go like, yeah, a little bit more in detail, like why it matters this much. Yeah. ~~Okay, so now let's say you ~~opt~~ optimize these ~~two, uh,~~ two operations. But guess what? ~~Uh, that's, uh, uh, ~~there are different flavors that you need to opt of these operations.

[00:40:59] [00:41:00] Okay. ~~And if you, uh,~~ these timers are coming from the,~~ uh,~~ tax generation workload because tax generation ~~is, you know, ~~is a bit special. There is input pockets and output tokens and processing them is ~~waste ~~vastly different. The processing of input tokens is mostly compute bound. And generating tokens is mostly memory bandwidth power.

[00:41:17] Now you have to have~~ these two~~ flavors of these two operations. One is,~~ uh,~~ flaps optimized, compute optimized. And the second is a memory bandwidth optimized to speed up ~~the load, ~~this~~ what you call, what you call,~~ paging, loading of tokens. ~~Uh, ~~model weights from this HBM,~~ uh,~~ to the SRAM and then to registers.

[00:41:34] ~~Um, ~~so that's what you need to implement now, how to implement. So let's take NVIDIA stack for example, ~~uh,~~ Can I just interject for one second? I just want to make sure I understand and that it's clear to the audience also that~~ The, ~~the two, we're all within inference here, right? But ~~the, ~~the kind of two forms of latency that matter are time to first token and then speed of token [00:42:00] generation from there.

[00:42:01] And these are essentially two different phases of the process, because, and here's where I'm learning from you and putting two and two together in real time. You said that ~~the, um,~~ the input tokens, aka the processing that happens for time to first token. Is going to be compute bound. And I understand that to be because in that process, we're doing all the attention, all the MLPs for all the tokens, but we can do that in such a way where we don't have to ~~like ~~page in and out the parameters for each token.

[00:42:37] We can ~~page them in ~~process, all the tokens with those parameters. Page new parameters in process, all the tokens at those parameters. And so that's why it's compute bound, right? Cause we're not paging in and out as much on a per token basis versus then when that's done and we get into token by token generation, now we need all the parameters in and out.

[00:42:56] For every single token, is that right? ~~It's actually much simpler than that. No, no.~~ So it's actually much simpler than that. [00:43:00] Okay. So the thing is that,~~ um,~~ if you look at typical,~~ uh,~~ use cases,~~ uh,~~ is they have, I would say roughly 10 to one ratio of input to output. So now when you have your input and the input also typically like one.

[00:43:16] 10, 000 and more tokens goes to 10, 000. Practically, it's very common to see,~~ uh,~~ this kind of workload. Now, that's for the,~~ uh,~~ for the generation. When you run,~~ uh,~~ the generation,~~ uh, you,~~ first of all,~~ you need to. Uh, you, ~~you generate one token at a time, unless you're doing some speculating generation, which is like separate, but it's mostly one, one token at a time.

[00:43:36] ~~Uh, ~~and of course, yes, ~~you will, ~~you will not,~~ uh,~~ also batch multiple generations together, but there is also~~ like~~ a limit there because ~~you're, ~~you're a big prompt length. ~~You're,~~ you need to allocate a lot of memory to host your intermediate activations. Okay. So in fact, what we see is that the batch size for the generation is around, I would say it goes from like 16 to 2, and the batch time for pre fill can go to ~~tens of ~~tens of thousands.

[00:43:58] So that's why here [00:44:00] you see this, what order of magnitude, even more two orders of magnitude difference.~~ So, ~~and ~~that's why, ~~that's why ~~the, uh, uh, ~~here,~~ uh,~~ the compute versus ~~the, the~~ memory bound, ~~the~~ thing ~~that~~ comes in. So ~~the, for the, uh,~~ for the pre fill, you have so many tokens to process. Yes. And so your,~~ uh,~~ bottleneck ~~is, ~~is actually,~~ uh,~~ Matt moves your bottlenecks.

[00:44:17] It fluffs the, on the computer, on the GPU,~~ uh,~~ for the generation. ~~Uh, ~~you don't have that many. And your bottleneck section, but in the board situation, you need to load the weights from HBM all the way to register. If you do it in both situations, but just the bottleneck on the generation ~~is, ~~is this loading?

[00:44:36] ~~It's not, ~~it's not the flops. So it's quite simple, actually, ~~man, if you think about it. ~~Okay. ~~So I think I'm with you. I'm not, ~~I'm not fully sure I understood the distinction between what I was trying to say ~~and, ~~and what you said.~~ It seemed like the, ~~the big idea as I understood it was that when you do the input tokens.

[00:44:48] Like to create an attention matrix, for example, ~~you're going to do every, ~~you have to do ~~every. You know, every token, ~~every token, right? And all the attention heads throughout the thing. And so there's a lot of compute there. And so just. On a relative basis, there's more [00:45:00] compute relative to the moving of parameters in and out, whereas in the generation side, now you're generating one at a time,~~ is it?~~

[00:45:09] ~~Is there? I mean, ~~there's not really a way to get around the fact you have to run the whole transformer, right? To generate one token. ~~So you do have to like, please go ahead, right?~~ So you do have to run the full transformer, but the fundamental thing here is that you use fundamental optimization. Which is called KV caching.

[00:45:22] So ~~in,~~ in this case,~~ uh, so what, uh,~~ in a nutshell, it is, as you mentioned, for the,~~ uh, for the pre fill, uh, for the, uh, for the ~~pre fill initial stage,~~ uh, you, you need to attend to all, so~~ all tokens have to attend to all previous tokens, ~~right? ~~So it's basically quadratic divided by two. So that's, ~~like, that's~~ a generation.

[00:45:33] You need to do the same, but ~~You can, you don't have,~~ for the previous tokens, ~~you can, ~~you can,~~ uh,~~ cache ~~the, uh,~~ this attention. You don't have to run it ~~again and ~~again and again and again. This is the KV cache. Yeah, exactly. ~~So, uh, well, ~~it results into only,~~ uh,~~ the token you're trying to generate attending to the prior ones.

[00:45:48] So this is, as you see is much ~~way, way, ~~way cheaper. Because it doesn't have this quadratic nature to linear nature. Yeah. How big does the KV cache get? And does it have to come [00:46:00] out of the SRAM and go on to the high bandwidth memory? Or does it just stay in the SRAM the whole time? ~~No, you, you, uh, In, ~~yeah, so it gets a little bit, right?

[00:46:08] ~~Uh, ~~and it varies,~~ uh,~~ because of multiple factors. ~~One is, uh,~~ one is the ratio,~~ uh,~~ of the Q hats to KV hats. So ~~that's~~ one of ~~the, ~~the MQA paper,~~ uh,~~ popularized this. And then now all the big models, they have this. So they reduce,~~ um, uh, ~~amount of KV hats. Usually an order of around four to eight, sometimes even more.

[00:46:28] But eight has been ~~very, ~~very common there.~~ Uh, ~~so there's one thing, another thing, you can shut the model.~~ So, ~~and now you're reducing as well. ~~Um, ~~so what we see in low MQA models, QCache is not typically ~~a big, ~~big of a problem. ~~Uh, ~~but in the end of the day, ~~you, yeah,~~ you have to,~~ uh,~~ keep it in the HBM for,~~ uh,~~ fast access.

[00:46:45] In some cases, you can actually put it in CPU memory,~~ uh,~~ and it's going to be permissible. But that introduces a lot of complexities as well. ~~Um, ~~yeah, but most typical case, you'll keep it in HBA. Okay, cool. So you were just about to say when I interjected,~~ um,~~ [00:47:00] okay, so let's do that on NVIDIA. Oh, ~~right. ~~Yeah.

[00:47:02] So ~~I think, um, yeah, so, uh, uh, ~~going through the, how ~~do you, ~~do you implement these,~~ um,~~ math moves and the tensions ~~very, ~~very efficiently. So ~~on the NVIDIA stack,~~ NVIDIA stack has a lot of APIs and they go from ~~very, ~~very low level to very high level. And let's start in the other direction. So from the high level,~~ uh,~~ NVIDIA has now this,~~ uh, already, ~~already serviced TRC LLM.

[00:47:19] So it's based on Triton for a service it's already ready to go. ~~Uh, ~~but,~~ uh, it's easy to. ~~It's easy to get started, although it's not as easy as some open source offering, but compared to the rest, it's much easier. ~~Um, ~~but it's the most rigid as always. So if you want to change anything, it's C code, basically good luck.

[00:47:37] And then when you go down the stack, if ~~this, uh, is,~~ you don't have enough flexibility from this setup, you can go and.~~ Um, ~~take a step down and you can,~~ um,~~ try to write, you want to use your own customized metamodel using, for example, kubelast library or QDNN.~~ Uh, then if it, uh,~~ these are pre compiled versions, there's a configs you can tweak, but can fundamentally change them.

[00:47:56] Then you want to take even step,~~ uh,~~ down. You want to be more flexibility. [00:48:00] Now we're looking at the Cutlass library and with the new. ~~Uh, ~~sub library, which is called Qt. It's pretty Qt, I would say,~~ much better, ~~much better than the older API. ~~U~~


## Exploring the Depths of GPU Programming and Customization

[00:48:08] ~~m, ~~this is,~~ uh,~~ very programmable, way more programmable. It's,~~ uh,~~ basically C code library.

[00:48:15] You can perform a lot of customizations there, but even if ~~that, ~~that is not enough, you can program yourself in CUDA C Even sometimes that is not enough, then you can go all the way to the hardware instructions and you can program in PTX. So all these options,~~ uh,~~ are possible. ~~The interesting thing is that Um, I would say, uh,~~ 


## The Evolution of GPU Programming: From CUDA to Tensor Cores

[00:48:31] it's interesting how,~~ uh,~~ GPU programming, ~~you know, uh, ~~evolved, right?

[00:48:33] So it all started with the programming kuda course, and if you look at GPU, that's what is what used to be. So ~~yeah, ~~you have CPU,~~ uh, uh, ~~core, which is very ~~program, uh,~~ programmable, but not as paralyzable. Now we going to the GPU,~~ uh,~~ and GPU has,~~ uh,~~ this good course. It's also programmable, not A CPU. They are fast.

[00:48:52] ~~Uh, ~~now the time passes by, and that is also not enough,~~ uh,~~ because,~~ as,~~ as I mentioned, we're only optimizing really for matmuls, and this attention, [00:49:00] which is also sort of matmul. 


## Challenges and Innovations in GPU Programming

[00:49:01] So how can we do better?~~ Uh, ~~now we need to do, next,~~ best,~~ best thing is embed ASIC into your GPU, ~~right? ~~And that's where the tensor cores come in.

[00:49:08] That's basically GPU. ~~Uh, ~~but, guess what? It complicates the programming big time. And ~~with the, uh,~~ especially,~~ uh,~~ on the newest hardware on the H100,~~ uh,~~ the tensor cores are asynchronously programmable ~~from the, uh,~~ from the CUDA cores. Now you have,~~ like,~~ two levels. ~~Uh, ~~of ity, you go CPU to launch Coda,~~ uh,~~ Coronas.

[00:49:27] And then from Cuda, you,~~ uh,~~ also synchronously~~ lo uh, ~~launch tensor core corn. So this becomes a really complicated and what we see as a result of it,~~ um, I, ~~I see practically ~~very, ~~very few good,~~ um, uh, ~~corners, which are geared towards H 100,~~ like, uh, ~~V 100 and a 100. They had a lot of good puda colonels,~~ uh,~~ geared towards them.

[00:49:46] ~~Uh, ~~people wrote it,~~ uh,~~ in George GPU programming, comes Hopper with a, there is a sync programming,~~ uh,~~ nature, and the amount of those,~~ uh,~~ public ~~cores, uh,~~ code is just drops, crazily, and there is a very good explanation to it, because the program becomes even [00:50:00] more complicated. So now the question is, how do we solve this problem?


## Introducing Triton: A New Era in GPU Programming

[00:50:03] ~~And I think ~~one good step on it ~~is~~ a welcome development is Triton from OpenAI. So ~~it~~ actually,~~ uh,~~ it's a different compiler. ~~Um, ~~I would say that,~~ uh,~~ C was a good choice probably back in the day when NVIDIA chose it for CUDA,~~ uh,~~ but now it's really getting in the way. ~~So~~ like~~ I really,~~ in some cases, it's much easier to program in assembly for CUDA than in that CUDA C to be honest.

[00:50:23] Thanks. 


## The Impact of Triton on GPU Programming and Maintenance

[00:50:23] ~~So, uh, ~~because of that,~~ um, uh, ~~we see a lot of experimentation and this,~~ uh,~~ Triton ~~is, ~~is,~~ uh,~~ a very,~~ uh,~~ pretty neat idea. And so there you literally,~~ uh,~~ a program in,~~ uh,~~ In Python,~~ uh,~~ and,~~ uh,~~ there is a lot of magic happening behind these things. Of course, there is never free lunch, right? So we basically,~~ uh,~~ introduces some kind of structure to your GPU programming, and it splits it in different levels.

[00:50:44] So first is like a very simple lab,~~ uh,~~ layer,~~ uh,~~ where you program just in Python, then it translates into what's so called MLIR, Intermediate Representation. And then even that one is a low level MLIR, which is closer to hardware, and then gets translated to PTX. So they go to the [00:51:00] lowest level right away.

[00:51:00] The nice thing about this ~~is, uh,~~ is this structure. So ~~structure, ~~because of this,~~ uh,~~ very complex GPU architecture we talked about, this structure actually makes it much easier ~~to, uh, I would say ~~to understand. ~~Uh, the, ~~the existing new,~~ uh,~~ kernels, and~~ I would say, uh,~~ longer term maintenance is much better.

[00:51:15] Because if you compare it to the C implementations based on CUDA ~~to, ~~to Triton, those are really hard to understand. ~~They have, ~~they have thousands, thousands lines of code. This provides a very nice clean separation. But again, no free lunch, and ~~I would say like, if you hope, ~~if you hope that oh, I'm just going to write a CUDA kernel,~~ uh, um, ~~in Triton, ~~and it's going to be,~~ I'm just going to write Pythons, and it's going to be super fast, I'm most likely, unless you're doing point wise, probably not.

[00:51:38] You have to still look in what is getting generated, what instructions is used and GPUs, are they pipeline, are they not? What tweaks I need to do and ~~so forth, ~~so forth. You have to still look in the output in ad there is no way around it,~~ uh,~~ to get to achieve the cutting edge performance. ~~Um, ~~but the nice thing is that it has this compiler, 'cause I don't really wanna write the assembly, right?

[00:51:57] Because they need to like, keep track of all the registers [00:52:00] and there's like 255 registers and ~~uh, ~~it's just that code is unreadable, right? So here, by introducing this structure, the hope is, and~~ I think~~ it does work in many cases, Although not a silver bullet, ~~it does, uh,~~ this structure actually makes the code much, much more readable and maintainable, and you can still achieve,~~ uh,~~ state of the art,~~ uh,~~ performance.

[00:52:17] ~~Uh, ~~in fact,~~ like, uh, ~~the Yermak Mullen attention implementations, although they are, ~~like,~~ not as flexible as you can,~~ uh,~~ write yourself,~~ um,~~ they achieve close to state of the art performance, ~~which is, ~~which is very important. Nice proof of this concept. Okay, so ~~let me ask a couple basic questions. Or again, ~~let me try a basic summary and then ask a couple basic questions.

[00:52:33] ~~So, there's a lot of, obviously, and this is true of all computing, right,~~ there's a lot of layers between electrons moving around at the very lowest level to, ~~you know, ~~Python level scripting, or now we can even say ~~you know,~~ prompting GPT4 to write me the Python to do the things that I want it to do. So, cool.

[00:52:47] ~~I and I think~~ I and certainly I would expect most of the audience is pretty familiar with the fact that,~~ like,~~ the higher level which you're working, ~~you know, ~~the more you sort of are at the mercy of all the other layers to ~~kind of ~~determine what your ultimate performance is going to [00:53:00] be. I have lived a pretty privileged life where most of the things I've done have been fine at the Python layer and I've, ~~you know, ~~only rarely had to,~~ um,~~ think too much about, ~~you know, ~~intensive optimization.

[00:53:10] So that much, I think is fairly intuitive. Like you go lower level to do more optimization. 


## Understanding the Need for Ongoing Optimization in GPU Programming

[00:53:15] What is not super intuitive to me is like,~~ what is it~~ What is happening that is causing the need for~~ like~~ lots of ongoing optimization today? ~~I mean, you know, ~~one might naively think, Hey, if it's all transformers, ~~you know, ~~there's presumably~~ like~~ only so much optimization that would need to be done across these~~ like ~~handful of operations within the transformer.

[00:53:36] And yet it sounds like that's not really the case. So ~~like, ~~What are the things that are driving the need for continual optimization or ~~like, you know, ~~why isn't just like a finite set of problems that have already all been solved by the community? I have a ~~good, ~~good question. 


## Navigating the Complex Landscape of Hardware and Software Optimization

[00:53:50] Yeah, I would say number one reason is a new hardware and new hardware,~~ uh,~~ trying to get more optimal and It's not just,~~ uh, it's~~ getting better with the [00:54:00] existing precision.

[00:54:00] So they used to be, we do everything in a single precision,~~ uh,~~ float,~~ uh,~~ 32 bit. And now it's shifted to,~~ uh,~~ a few years ago, we doing half precision. FB16 for inference,~~ uh,~~ FB16 for training. I would say kind of a new standard. So someone,~~ uh,~~ new precision,~~ uh,~~ go to new precision. But guess what? 


## The Role of Precision in Modern GPU Programming

[00:54:21] That is not also good enough.

[00:54:23] NVIDIA needs to have an MD. They need to have new step functions. ~~Um, ~~and they, what they're doing, they're lowering the precision. So now,~~ uh,~~ I will~~ in, uh,~~ go to precision inferences ~~and, ~~and to some extent for e training is,~~ uh,~~ FD8. It's only 8 bits, right? ~~Uh, uh, ~~we use for a single parameter. And we also do compute in 8 bits.

[00:54:42] ~~Um, so, uh, ~~then,~~ uh,~~ look at the B100, ~~right?~~ Guess what we'll introduce. Of course, they go to 4 bits,~~ right?~~ And look at the,~~ uh,~~ recent papers and,~~ uh, uh, ~~one of the best papers,~~ uh,~~ A paper search I like is so called 1. 5 bit. It's what they call one bits, not one bitters. But fundamentally, the theory is that to train LLM,~~ um,~~ you just need [00:55:00] 0, 1, minus 1.

[00:55:03] ~~So, ~~so basically go left, go right, or stay put. So this is like a fundamental property. And if you can have that, you can train a model and looks like this is enough. You can basically replace the larger parameters model with the smaller parameters. Of course, you have to retrain. This is a crazy reduction precision.

[00:55:25] But it looks like these models perform on par with the real models. ~~Uh, ~~have for full precision models. So this is a very welcome development. You will see even more hardware optimizations. Because,~~ like,~~ if you do this,~~ uh,~~ zero, one minus one, guess what? You don't need multiplication. It's all addition now.

[00:55:41] ~~So, ~~you will see even more optimizations from,~~ uh, I would say,~~ NVIDIA and,~~ um,~~ AMD in coming years. ~~One of these models,~~ once we train bigger models, because there are only, like, one, three billion models trained for this, once we train in bigger models, ~~you will Uh, ~~this position will become even more critical.

[00:55:54] So now,~~ uh,~~ these new precisions, they,~~ uh,~~ require a very,~~ uh,~~ [00:56:00] different,~~ uh,~~ instructions. ~~Uh, ~~and,~~ uh,~~ because you see like here, the ratio of generation of GPU is really optimized for this specific ratio of computing and memory back. So here, when the ratio changes, they change the nature of the APIs and you need to basically code from scratch, to be honest, ~~like ~~for the GPU generation.

[00:56:19] All the past, it works, but it's much slower than it could have been. ~~Um, like ~~a good example could be. I would say,~~ uh,~~ flash attention,~~ uh,~~ implementation flash session two,~~ uh,~~ was called for a 1 4, 4 16 precision. And then you run an H 100, you have, ~~you got ~~just ~~half,~~ half of what you can get. ~~Um, ~~it's same kernel, but it just uses all the operations, all the instructions from p ~~uh, ~~while,~~ uh, uh, ~~the hyper instructions are different.

[00:56:41] So ~~I think~~ this is like ~~the, ~~the,~~ uh,~~ why fundamentally~~ it's,~~ it is happening and we still have a lot of work ahead of us, ~~so. ~~For example, a few years ahead, until we reach three, once we reach these three bits, let's see what's next, but there's still a long way to get there. 


## Exploring the Future of GPU Programming and Optimization

[00:56:55] Yeah, that 3 bit paper is, or the 1.

[00:56:58] 58 bit paper is super [00:57:00] interesting.~~ So, ~~I will add to that, right? ~~So, ~~Dimitri just mentioned, hey, hardware keeps evolving, right? 


## The Intersection of Hardware Evolution and Application Development

[00:57:04] So, not just NVIDIA hardware keeps moving forward and, ~~you know, ~~basic instruction settings. Keeps changing, but also there's other lines of product, right? There's MD, there's Intel, there's ~~custom, custom, ~~custom basics and so on.

[00:57:14] So they're ~~kind of ~~very broad and we want to ~~kind of ~~simplify that for our user. But also if we look at our perspective, so we are looking down. If we look up at the application level, ~~right?~~ So we mentioned latency. You mentioned time to first token, right? So sometimes latency also means time to the first 30 tokens, because they are voice streaming out and ~~you know, ~~they have to get the 30 tokens before they can stream in.

[00:57:37] Or they care about the end to end latency, ~~right?~~ So latency also means different things. And people always want to get a spectrum of latency cost trade off. They want to see a curve and they want to pick a point in that curve ~~and~~ best for their business.~~ Um, ~~and now on top of that. ~~Um, ~~the input output ratio is different per application.

[00:57:57] ~~Uh, ~~we see a lot of rag [00:58:00] usage where it pushed the input~~ to be like ratio~~ to operation, to be a very high, it can be,~~ uh,~~ 10 to one or even much higher. Or sometimes,~~ um,~~ it, people just generally went one token for classification or sometimes they are generally a lot,~~ uh,~~ like during journey code. ~~Uh, ~~so ~~the, ~~the ratio keeps changing.

[00:58:18] And the best deployment to find depends on what kind of latency you care, which dot in this latency cost curve, what is our input output ratio, what are generating, what kind of is your input, your context window length, it all matters. It's very complicated to optimize upwards towards. Where your application looks like, does it have repetitive prompts, for example, as another application vertical down to ever moving hardware landscape, ~~right?~~ That is a complexity all~~ uh,~~ application product developers as,~~ um, you know, ~~they are doing things, fun stuff themselves or [00:59:00] in enterprises, they're all facing this challenge, so that's where we come in and we say, you don't have to worry about it. We handle it all for you. So you just focus on,~~ uh,~~ your product application development.

[00:59:12] So ~~that's kind of, ~~I just want to double. ~~Uh, ~~click back to what is our roles in this complex ecosystem. ~~So, ~~yeah, it's funny that you mentioned ~~the, um,~~ the curve and picking the point on that curve. ~~Uh, ~~I'm putting together a little talk for business leaders,~~ um,~~ and ~~kind of, you know, ~~developing a~~ like~~ top 10 or whatever things to know for business leaders.

[00:59:32] One of my tips for them is to learn to think in Pareto curves. And this is something that I see at literally every level ~~of the, ~~of the stack, ~~you know, ~~including like false positives, false negatives, ~~you know, I mean, ~~truly ~~like~~ every level seems to have this. So do you envision a future of ~~like your, ~~your product experience being literally just showing people these curves and ~~like, ~~should I expect to see ~~like, ~~A number ~~of, ~~of Pareto curves where I, ~~you know, ~~can ~~sort of ~~pick [01:00:00] like, okay, ~~I want, you know, ~~for this application, I want absolute minimum time to first token.

[01:00:03] I'll take the highest cost for this one. I'll take the happy medium for this one. I want the lowest cost,~~ but it's a, you know, ~~it's a background process or whatever. So it's okay to wait. ~~Um, ~~is that the kind of experience ~~that's~~ the kind of choice that you want to expose ultimately to developers? So I would draw an analogy,~~ um,~~ here.

[01:00:18] ~~Uh, ~~so ~~I think. ~~2025 years ago,~~ uh,~~ database is a new domain, ~~right? Um, ~~and the database management systems or no start to come into pictures. ~~Um, and, uh, it's very,~~ actually. It's very interesting analogy,~~ I think,~~ now I'm thinking about it on the fly. So database queries ~~are,~~ has strict patterns. It's called SQL, ~~right?~~

[01:00:34] You have your select clause, you have your where clause group by doing aggregation, ~~right? ~~So this is a very clear pattern. ~~Uh, ~~if you think about that, JNI, the models has very clear pattern too.~~ Right. ~~You have your operator,~~ um,~~ layers. ~~Uh, ~~it's more or less stable right now, although the pattern is simple. ~~Uh, ~~but depends on, ~~you know, which the, no,~~ how many columns you have,~~ uh,~~ which column you're going to put a future on, which column you're going [01:01:00] to do aggregation, which color you're going to do group by.

[01:01:03] There are all different ways to optimize your query. ~~Does that make sense? Right. So, ~~and at early days. None of these database management system are smart, ~~right?~~ That's why it created ~~a slew of, uh, it created~~ a whole new entire career. It's called DBA, ~~right? ~~So basically all database has knobs for human to tune, to try to optimize things.

[01:01:21] those people make a lot of money because once they optimize, it's a much better experience, it save a lot of money too, right? It's very similar to what we just talked about latency and TCO. But over time, all these database management systems have become smarter and smarter because they all have a layer called optimizer, ~~right?~~

[01:01:37] Those optimizer observe the workload and it start to create.~~ Oh, this,~~ oh, you're doing a lot of,~~ uh,~~ feature on this particular column. So I'm going to create index. I'm going to partition those columns based on your feature criteria. So it's much better search, much faster search. You can skip a lot of things.

[01:01:53] You ~~have to ~~have to do sequential scanning. ~~Um, ~~and so on. So there, then the optimizer becomes ~~smarter and ~~smarter and ~~they start to kind of, ~~you don't need to hire DBAs at all. [01:02:00] It's fully automated,~~ right?~~ So as long as you observe the workload, you have the workload defined. It's tuned, it's self tuned towards the best,~~ um,~~ outcome.

[01:02:08] So that's our vision. Today we have multiple configurations based on what you tell us, your workload pattern, what you care about, we deploy for you, which is ~~really, ~~really good, but over time, we want to ~~automate, ~~automate ourself away from that process. Basically we'll learn ~~from, ~~from,~~ you know, ~~what you are running and the system becomes smarter and smarter.

[01:02:27] ~~Uh, ~~it can become lower latency over time. It can be higher quality over time. So that's what we are aspiring to build. So ~~are~~ these options, ~~this would be~~ in the product line today would be in the dedicated deployments product, right?~~ Is where I get to set that if I'm doing serverless, presumably you're already kind of handling your own, um, optimization challenges there.~~

[01:02:41] ~~And I don't have to worry about that at all, although I maybe get less. Choice in terms of what tradeoffs, you know, I get to make, but in the dedicated deployments,~~ can you run through some of the, I scanned these documents, but I wouldn't say I conceived of it in the way that you're describing it now. So what are some of the choices that I get to make today, depending on what my application needs are?

[01:02:54] And how does that. Evolve in ~~the, you know, ~~the short and medium term. Yeah. ~~So, ~~for [01:03:00] example, ~~I think we, uh,~~ if you look at our~~ offering~~ product offering, we have,~~ um,~~ three tiers. The developer tier, the business tier, the enterprise tier. So the business tier is more like surplus pay as you go. And enterprise tier, ~~we will, um,~~ usually ~~they, ~~they have clear workload definition and they know where the latency cost curve, where they want to be.

[01:03:19] Because they have budget,~~ uh,~~ they also have product requirements,~~ um,~~ and they know their workload, like in terms of input, how much they're using and how much generation and so on. And then ~~we, ~~we come in and pick a perfect spot for them. ~~Right. ~~And then we deploy a specific configuration,~~ uh,~~ towards that workload.

[01:03:36] ~~Right. So, ~~but over time,~~ uh,~~ this can be more and more automated and,~~ uh,~~ because their workload can evolve, they don't always have to get us ~~in, ~~in the loop. ~~Uh, ~~and ~~we were just, ~~our system would just,~~ um,~~ self adjusting towards ever changing workload. So that's how,~~ uh, kind of ~~the direction we're heading towards.

[01:03:52] S


## Strategic Deployment and Optimization for Enterprise Applications

[01:03:52] o could you give me a little bit more~~ like ~~intuition for, ~~let's say I have three, ~~let's say I'm an enterprise customer and I have three applications. I have one that's user facing and it's going to [01:04:00] generate tokens for a voice app. And ~~so, you know, ~~those first 30 tokens, as you said, are ~~like~~ super critical to get fast.

[01:04:05] Cause I want to have conversational fluency. So that's ~~like ~~one. Then the other thing is like a background job where I'm just like,~~ I just, ~~Give it to me as cheap as I can. And then there's maybe a chat bot one ~~that's, you know, I'll say, well,~~ that's in the middle. I don't want to pay top dollar for that, but~~ you know, ~~I don't want it to be slow.

[01:04:19] How does that trickle down into what you are actually deploying for those three different scenarios?~~ Right. ~~So usually in your enterprise,~~ they have, as exactly as I said,~~ they have many applications,~~ um,~~ and,~~ uh, they are, uh,~~ usually,~~ uh,~~ the distribution of traffic is always skewed, right? There are heavy hitters,~~ um,~~ they're ~~kind of ~~very high volume.

[01:04:38] ~~Um, ~~and there are ~~kind of ~~long tails. They're each doesn't have high volume, but they add up. So we recommend, ~~like ~~they basically think about long tail as one bucket of deployment,~~ um, and, uh,~~ And we give them one configuration and we help them optimize for the heavy hitters.~~ Uh, ~~each of the heavy hitter, as I said, they care about different kind of latency.

[01:04:54] ~~Um, ~~and those heavy hitter probably are coming from their product team. Usually we also work with ML Infra team [01:05:00] coming from the product team and they have a certain product budget. ~~So, ~~so then ~~we, ~~we work together to figure out, Hey, which dots you want to pick in this curve.~~ Um, and, uh, the product will say, Um, now~~ when it comes to quality, then ~~the, ~~the prompt length coming into picture, right?

[01:05:10] How much instruction tuning you put there, whether you fine tune, take away ~~the, ~~the instruction prompt or,~~ uh,~~ you put a lot of rag ~~uh, ~~information as a context to constrain the model,~~ uh,~~ to ~~spit out the, uh,~~ do less hallucination. ~~Um, ~~so all these kind of product contacts. ~~Uh, ~~start to come into picture,~~ um,~~ and then,~~ uh,~~ we have different kind of deployment to have optimized for very long context window processing,~~ uh,~~ versus,~~ uh,~~ they do a lot of generation.

[01:05:34] So those are also different configurations. Yeah, I can give some concrete example,~~ uh,~~ where you have to have,~~ uh,~~ different deployments,~~ uh,~~ for specific use cases. ~~Um, ~~so let's say you really,~~ uh,~~ want to get a very low time to first token, the prompt is long, right? And let's say your model is small, 7 billion parameters, ~~you can,~~ you don't have to shut it really to put in different GPUs.

[01:05:59] ~~Um, ~~[01:06:00] but the thing is that it's still,~~ uh,~~ not fast enough to run on a single GPU because the problem is so low. So now, for this specific use case, you want to shard it, but there is a cost for sharding. So there are like, fundamentally, ~~I'm thinking of~~ three sharding techniques. One is to,~~ uh,~~ shard your model weights.

[01:06:16] ~~This, uh,~~ another one is to shard,~~ uh,~~ the activation of the input. The third one is to chop modeling pieces, that is called pipelining parallelism. So the last one doesn't really help you with the latencies, it just helps when the model is too big. In the case when you chop model weights, also called model parallelism, aka tensor parallelism, this ~~does~~ help also with the model size and does help with the latencies.

[01:06:42] Although there is a cost for sharding. ~~Um, ~~so ~~basically, ~~basically your throughput overall declines. And the first one, the input sharding ~~is~~ usually,~~ uh, uh, yeah,~~ it doesn't help you with the model size. ~~Although it does, uh, uh, it's,~~ and it's pretty cheap, but. ~~And ~~there's a caveat attention, so you need to take care of attention, because you attempt to add the token, so now ~~you, uh,~~ you have to [01:07:00] have a bit more complexity in your setup.

[01:07:02] ~~Um, ~~so the bottom line here is that,~~ uh, for the, ~~for the pre fail, ~~if you,~~ for example,~~ uh,~~ most ~~common, ~~common,~~ uh,~~ shunning right now is this tensor parallelism, if you choose it,~~ um,~~ you don't want to always shun. You really want to, don't shun as much as possible up to the point. Where you have to. Because there is a cost.

[01:07:17] Because your throughput will be tanking the more you shut. But you have to shut because you cannot meet the latency budget. So this is like fundamental thing and I don't think ~~this, ~~this problem ~~kind of ~~goes away anytime soon. Yeah. Okay. So I think again, everybody will be conceptually familiar with the idea that there is a like latency throughput trade off.

[01:07:37] ~~I mean, that,~~ that seems to be ~~kind of ~~a very recurring pattern. But if I understand what you're saying correctly here, it is that if you have a really long prompt, even if you have a small model that can fit onto one GPU, you may want to split across. GPUs. I'm not quite clear on the nature of the splitting.

[01:07:53] Are you splitting like layer wise? Like you'd have early layers on one and then later layers on another. So ~~every layer, ~~[01:08:00] every layer you'll split. ~~So basically you'll be running this, ~~it's more ~~complicated, ~~complicated, but ~~it's like, ~~it's like ~~very, ~~very natural because it goes to Megatron sharding. When you shard two Metamorphs, even do one column wise, then other row wise and minimize the amount.

[01:08:11] Cause in the end, once you do this, you need to reshuffle it, do all the reduce.~~ Uh, ~~so you want to minimize that and,~~ uh,~~ this Megatron style Shadi helps you. But fundamentally, yeah, you're splitting, actually, the weights ~~across ~~Across GPUs and then you need to over reduce,~~ uh,~~ the activations and stuff. Can you give us a little bit better intuition for that?

[01:08:29] 'cause ~~I think~~ that's something that is, ~~it's~~ not super clear to me, and I suspect a lot of people are not gonna be very clear on it either. ~~I, ~~I've seen examples of this in my study of ~~the, ~~the mamba and mamba related things recently. I've been trying to get a better handle on this. And ~~I guess ~~one thing that's like ~~kind of intuitive, kind of ~~surprising or counterintuitive is that there are ways to take advantage of basically the associative property, where you can ~~sort of ~~do these~~ like~~ quite counterintuitive algorithms, even for just like adding up numbers that kind of look pretty weird.

[01:08:59] [01:09:00] But. End up being faster, especially because it allows for this kind of parallelism. ~~Right. Am I, ~~am I on the right track with that? ~~I mean, ~~yeah. ~~So I think, ~~so here it applies not necessarily.~~ I think ~~this kind of shutting is like. I would say ~~kind of ~~model architecture independent. So these are,~~ uh,~~ the input data parallelism, tensor parallelism and pipeline parallelism, they've been there like before even Gen AI,~~ uh,~~ kicked in.

[01:09:22] But they're kind of fundamental ~~to the, I would say,~~ to machine learning. ~~And then you, uh,~~ but ~~like, ~~then which one you want to apply totally depends on the architecture because one architecture is much better. ~~Uh, ~~for example,~~ um,~~ if you don't~~ don't have, you don't ~~have a sequential nature, Using pipelining parallelism is actually ~~no, ~~no goal.

[01:09:35] It's not going to save anything, because you cannot even ~~chop, ~~chop the model. And,~~ uh,~~ it used to be a model like that. All transform models tend to have layers, so it's much better. But,~~ uh,~~ something like, if you look back on the image, older image model based on ResNet, it has the same connections. It's become harder to do pipelining parallelism.

[01:09:52] ~~So, ~~yeah. ~~So, ~~and then,~~ um,~~ the tensor Conceptually pretty is harder to understand. ~~I think~~ the,~~ uh, uh, ~~data you put by those is easier [01:10:00] because you just split data and data is independent. So you could just. ~~Uh, ~~duplicate the models with the inputs, right? And so the, and they go,~~ uh,~~ process and then join them in there.

[01:10:08] That is easy. ~~Um, the, the, ~~the,~~ uh, uh, ~~model parallelism, tensor parallelism, which we actually do use right now, hard is to understand because once,~~ uh,~~ the way it start,~~ uh,~~ interacting with each other, you need to make sure your math is correct. Because you can't just,~~ Shard, ~~shard,~~ uh,~~ across if you need to, for example,~~ uh,~~ two values, if you need to add them in there.

[01:10:24] ~~You need to,~~ if you want to shard them, but you have to still do the addition. If you need to multiply, you still have to do the multiplication. So when you do that, you need to probably gather them on one rank or another rank, or send them across them, and then split these operations across the ranks. ~~Um, ~~of course, sending~~ across, uh, uh, uh, ~~across GPUs is way more expensive than just sending from,~~ uh,~~ HBM or single GPU to, to the registers, which make it worse, even more.

[01:10:47] ~~Um, ~~so it becomes ~~quite, ~~quite complicated, but this is the kind of compromises you have to go through. So basically, in the end of this, you need to make sure that your math is still correct once you do the sharding. So this is the idea of [01:11:00] this, and there are different techniques, and basically not every operation can be easily split.

[01:11:06] This way, you need to look at specific operations, specific matrix multiplication, how you can split them. ~~Yeah,~~ so if you want to research about this, yes, Megatron is a good starting point. It has a fundamental description of how you do the Matmul sharding. Yeah. Okay, cool. I'll check that out. That's a good pointer.

[01:11:23] Let me just try to summarize the three kinds and make sure I at least have the conceptual framework right. Simplest one is data parallelism. That is just make multiple instantiations of the model. You can split the data across them. That's essentially like a load balancing ~~kind of ~~set up. The next level up, which maybe is the most complicated, ~~it sounds like.~~

[01:11:42] is actually splitting the weights. This is the kind of thing that you would do because you have a super long prompt, for example, and you want to have a fast time to first token. So you need to have even more parallelism of the computation and it can be [01:12:00] worth it, but it comes at this cost of, now you've got GPU to GPU communication plus the complexity of what the hell am I doing across all these different, you know, now that I'm splitting weights, like, okay, that's a lot to keep track of.

[01:12:13] And then the third one is the pipeline. And that is where you actually split early layers from middle layers, late layers, whatever. And ~~you're, ~~you're feeding through multiple things ~~in a, in a, ~~in a pipeline, ~~in a, ~~in a sequential way. Okay, cool. That's helpful.~~ Um, ~~lots of learn I've been,~~ uh,~~ Doing this around the clock.

[01:12:30] I feel like for,~~ um,~~ a few years now and,~~ uh, I, I still, you know, ~~it's still a target rich environment ~~for, ~~for new things to learn. ~~Um, ~~yeah, ~~I mean, ~~I think you can combine them in many different ways and go to the really complicated setups. So it gets hairy. Yeah. ~~Those are all, ~~those are all. independent dimensions as well.

[01:12:47] Okay. So ~~I mean, ~~we've covered a lot of ground. One other question I wanted to ask about, ~~and then maybe just give you guys a chance to, you know, to touch on anything that we didn't touch on that you want to, ~~is, ~~you know, ~~With all this complexity of,~~ you know, ~~everything we've talked about, ~~right?~~ The one thing that was ~~kind of ~~surprising to me is that you are also training [01:13:00] your own models.

[01:13:01] You have your own branded fireworks function calling models. And especially given your earlier comment that ~~like.~~ You think ~~kind of the,~~ at least the small models are ~~sort of ~~converging. How does that fit into the overall strategy? Like why bother training ~~your, ~~your own models, as opposed to just focusing on ~~the, you know, ~~the insane complexity of the inference stack and letting that convergence happen independently,~~ uh,~~ of your efforts,~~ Um,~~ that's a great question.


## The Future of Inference Stack and Knowledge Extraction

[01:13:25] ~~Um, ~~and,~~ uh, I think like~~ one of the biggest, like the North star of the product we're building is not just serving individual models, ~~right?~~ So we want to be the inference stack for knowledge extraction.~~ So, it's an inference step for knowledge, knowledge extraction, um,~~ and when we talk about knowledge,~~ it can,~~ we can ~~kind of ~~first look at the knowledge provided by large language models.

[01:13:43] It's very capable now. ~~Um, ~~it can answer many questions. It surprises us. But at the end. All large language models has limited knowledge. Why? ~~Uh, ~~the knowledge is limited by its training data. Its training data is limited in terms of time range. It doesn't have the most [01:14:00] latest information. ~~Um, ~~and,~~ uh,~~ it doesn't have the information it, people cannot crawl for internet.

[01:14:06] ~~Uh, ~~those public informations, so ~~they, ~~they are just limited, limited to the corpus of information people can crawl directly from. And many of those,~~ um,~~ knowledge also live outside of large language models because there are~~ model, ~~foundation models, they generate images, they generate videos, generate audios.

[01:14:25] They also do information extraction for images.~~ So, ~~so ~~that's kind of, ~~I want to ~~kind of ~~create a framework to think about the knowledge distribution is beyond just large language model and even for given a large language model, it's limited. And there are other modalities that carry a lot of information beyond that.

[01:14:44] There are a lot of knowledges hidden behind APIs that we cannot extract from. And,~~ uh,~~ we use API very extensively day to day.~~ Uh, ~~for example, we do search, right? So there's Google search, there's weather API, there's stock,~~ uh,~~ extraction API, there's [01:15:00] map API for personal productivity. ~~Um, ~~there are APIs for dogs, for spreadsheets, for calendars, and so on, so forth.

[01:15:07] So APIs are everywhere within enterprise. One enterprise internally can have hundreds of API surface areas too.~~ Uh, ~~there are a lot of key value stores, document stores, production logs, pop subsystems, internal search. So API itself contain a large corpus of knowledge. So think about function calling. What is function calling?

[01:15:26] ~~Think about, uh,~~ so our file function,~~ uh,~~ the model we build ourselves,~~ um,~~ is serving the function calling area. And function calling is the layer to tie knowledges together behind all different modalities. Of foundation models and APIs together, ~~right? Um, ~~so to us, strategically, this is a critical layer,~~ uh,~~ for us to build the best inference tier for knowledges.

[01:15:51] And with that, you can build a lot of fun application. For example, you can build a personal admin. To knock down and to everyone on the planet that can sort [01:16:00] out tedious work, this application can learn what you like over time and can preemptively finish work before you even ask and put out reminders or even suggest things ahead of time.

[01:16:10] I wish I could have a personality like that, but ~~this,~~ those kind of new application has to depend on. ~~Uh, ~~tools and ways to extract knowledge across the board,~~ uh,~~ from foundation models and from APIs. ~~Um, ~~that's the fundamental reason why we build our own function quality model. We have released two versions,~~ uh,~~ open weights, so everyone can use it.

[01:16:31] You can download from Hugging Face. We are currently working on our third version that's going to come out soon and we'll have a great quality bound. So stay tuned. Cool. ~~Well, ~~I can look forward to that. I know we're just about at the limit of our time together today, and you guys have been very generous with your time and knowledge.

[01:16:47] Is there anything that we haven't managed to touch on yet that you want to make sure you mentioned? I think we've touched on a lot.~~ I'm curious about the final production coming out. It must be very interesting. You mean in terms of like our editing process? Yeah, we'll edit. It'll be fine. Um, it'll be pretty straightforward, honestly.~~

[01:16:54] Yeah, I think you have one question about SSM. Yeah, that's a hobby horse of mine. ~~Um, you know, ~~is that on your,~~ uh,~~ [01:17:00] customer's radar? Is it on your radar? Is it on your roadmap? So actually we haven't heard too much about,~~ uh,~~ the requirements for our customers. I think it's a very cool technology. So of course, when we talk about SSM, it's in the context of Mamba.

[01:17:12] ~~Yeah. I think. It's a really cool technology. Uh, ~~the main barrier to practical adoption is mainly quality in my mind,~~ uh,~~ compared with transformer models. So we haven't seen a pure Mamba SSM based model emerge as ~~a comp ~~highly competitive in quality to Mistral, Cloud, GBT yet. I think ai21labs just open source Jamba, it's a hybrid of SSM and transformer models, but the real quality, benchmark is one thing, real quality in practice, another thing, so real quality using practical use cases yet to be verified.

[01:17:47] ~~Uh, ~~so that's why I think ~~we don't, ~~we haven't seen a huge demand there.~~ Uh, ~~and I guess people are more cautious. ~~Um, ~~it's hard to say what will be the technical challenge. I think Dimitri was pretty confident we can support it in [01:18:00] no time, but ~~I think~~ again, coming back to quality,~~ it's, it's, ~~it's a little bit hard to assess.

[01:18:04] So those kinds of,~~ um,~~ architecture,~~ uh,~~ Mamba and SSM is really good for long context by removing the quadratic nature of transformer.~~ Uh, ~~before long contacts is hard to assess the quality needle in this haystack ~~is, ~~is the most common use the benchmark.~~ It's, ~~but it's not very comprehensive. I don't think as an industry, we have standardized the benchmark for measuring long context quality yet.

[01:18:27] ~~So, ~~this is another area where ~~I think~~ the whole industry ~~into, uh,~~ into move forward. This thing still show that there is room. To go for architecture to meet the,~~ uh,~~ current transformer based on,~~ uh,~~ attention as models. Yeah. My money's on the hybrids for what it's worth.~~ I think ~~there's been some really interesting kind of very fine grain studies of the comparative strengths and weaknesses,  
 
[01:19:00] Guys, I know you got to go. This has been a great conversation. Lynn Chow and Dmitry Dimitrovchenko. Co founders of Fireworks AI. Thank you for being part of the cognitive revolution. 


#### 00:00:00.149

Martin Casado, General Partner at A16Z. Welcome to the Cognitive Revolution. Very happy to be here. I think this is going to be a great conversation. We are primarily here to talk about the importance of open source and to dig into a lot of the details of the current debates around early regulation of AI and how that might impact open source and what the pros, if any, and cons, if potentially many of that might be. Before we get into it, I just wanted to get a little bit of your super big picture AI worldview and ask you to project out a little bit. How powerful do you think AI is going to be over the next couple of years? 


---


#### 00:00:40.040

We've obviously heard AGI 2027 recently. Is that a story you're buying? What do you think we're going to see over the next two to three years?   
(00:00:48.862) ~~Listen, I think like all things,~~(00:00:50.204)  
the past is probably the best predictor of the future. My hope is this continues to be a very useful tool to help us with progress and to stave off this universe that seems pretty destined on killing us. So I'm hoping it continues on that trajectory. What is interesting is if you actually look, let's say the past 80 years of quote, unquote, It's been steady progress, independent of there being winters and summers. It's been very steady progress. It's been progress on economics, progress on problem solves. 


---


#### 00:01:19.906

And every time we tackle a problem, everybody's like, oh, goodness, this is it. We're almost at AGI. And then it just turns out that's one modality, and then we go on to the next, and we say, oh, that wasn't really actually AGI or AI. So this whole AGI thing has been a moving goalpost for 70 years. And so I would say,   
(00:01:35.599) ~~listen,~~ (00:01:36.118)  
it's been this kind of very steady progress. We've gotten good at many things. It's been a very useful tool. I hope it continues to be so. I think it's a very important thing for us to continue to develop and use. But I don't think that there's any step change or it changes the nature of computers or software in ways that we haven't seen before. 


---


#### 00:01:55.317

I don't think that.   
(00:01:58.225) ~~Let me just say~~(00:01:58.825)  
a few more concrete things, because I'm a big believer in threshold effects, where sometimes I see this, it's not necessarily the topics of emergency are super hotly debated, and is emergence of mirage or not a mirage, and maybe the underlying curves are smooth. But in terms of   
(00:02:17.219) ~~like~~ (00:02:17.340)  
practical utility, even if the capability of the model hasn't taken a sudden shift, the   
(00:02:23.598) ~~like~~ (00:02:23.798)  
utility and what it can actually practically do in the world sometimes seems to take   
(00:02:28.301) ~~like~~ (00:02:28.481)  
a notable leap.   
(00:02:30.242) ~~I guess,~~(00:02:30.502)  
right now,   
(00:02:31.503) ~~it seems like~~(00:02:31.805)  
I thought Dworkish put this really well on a recent podcast where he said, it seems like the models are token for token, as smart as most people. 


---


#### 00:02:40.450

And yet there's some things that they're missing. Like they don't have this great long-term memory or the ability to integrate memories. They're not great at autonomy. They fall down and can't get back up or don't know how to dust themselves off. But it seems like the core intelligence is there to do a lot of jobs. And it's this packaging, memory, agentic finishing that's needed to get to the point where you'd have   
(00:03:02.074) ~~like this sort of~~(00:03:02.635)  
knowledge worker. Is that basically the story that you see? And does that translate to a,   
(00:03:08.580) ~~I think~~(00:03:09.080)  
AGI is yes, certainly very ill-defined, but like drop in knowledge worker that could do a large majority of jobs, like passively well is maybe better defined. 


---


#### 00:03:19.914

Do you see that coming soon? So again, I think I like to draw from a historical analogy, because I think they're very useful in this context. Because I just feel like we see these very often, and they all look the same, and it's played out. And so when I first joined Stanford to do my PhD, so I did my PhD in computer science and systems. It was in 2003. And around then, I don't know if it was 2003 or 2004, Sebastian Thrun had won the DARPA   
(00:03:45.118) ~~Grand Challenge.~~(00:03:45.758)  
To the driver   
(00:03:46.653) ~~grand~~ (00:03:46.835)  
challenge, he drove a van autonomously, fully autonomously for 1200 miles. And everybody was like, hooray, like AGI is solved. Robo taxi is solved. 


---


#### 00:03:57.604

This is amazing thing. And a hundred percent, we've hit one of these threshold moments. A hundred percent, like you could actually do things you couldn't do before. It was the start of a new era of vision and perception and self-driving. And now, 20 years later, and about $100 billion invested, a little bit less than $100 billion invested, the unit economics of self-driving are still three times worse than Uber. And so I am a systems person, meaning all I've been doing for the last 30 years of my life is building computer systems, large distributed systems. This is what I do. And I just know that Capabilities, like scalar capabilities, A, they're not necessarily parametric. So they don't necessarily just go up and to the right. 


---


#### 00:04:41.781

And there's so many examples of this, and we can talk about that. I know that the universe is this very heavy-tailed system, and there's no single solution that tends to reign in its complexity. I know that the economics for these things are very hard. What gets lost in these conversations is AI has been better at humans for a very long time at many things. Handwriting detection. Diagnosis for a very long time. Game playing for a very long time. Mathematics, since the creation of the computer. Four orders of magnitude better than mathematics than us. And yet, none of these things have resulted in   
(00:05:15.269) ~~kind of~~(00:05:15.490)  
general economically viable solutions for everything, just for subsets. Another way to rephrase what you said about the language stuff is, these models are very good at predicting what a mean person would do next. 


---


#### 00:05:34.180

A mean person would do that. So sure, they basically do kernel smoothing over positional embeddings. That's great. Which means if you have a corpus of data, it'll give you the average response, which is great. And it's very useful for a number of things. Does that provide economic utility for a broad range of stuff? I'll tell you, I look at these companies basically full-time and I have for three years, we probably have the largest portfolio of them. And I don't see that yet. Now there are areas where they do work, but   
(00:05:59.057) ~~it's not that,~~(00:05:59.598)  
it's not this kind of general knowledge worker. That's actually not working. And the areas where it is working is stuff like the marginal cost of content creation goes to zero. 


---


#### 00:06:08.901

So now we have like amazing new content. Or computers are creating an emotional connection with humans. That's new. And that's exciting. And that's amazing. But this idea of this general knowledge worker working, I haven't seen it yet. And maybe it'll happen. But just like self-driving 20 years ago, that's just not how the universe tends to play out. Yeah, where do you think we are in self-driving today? I recently took a, and it's been actually a couple upgrades since I took my last ride in a Tesla FSD. At that time,   
(00:06:38.851) ~~I was like,~~(00:06:39.411)  
this was last summer, actually. So it's been basically a year since I did it last. At that point,   
(00:06:43.975) ~~I was,~~(00:06:44.134)  
I think this is actually safer than the average person I drive with and probably the average person I see around me on the road, who sometimes I'm like, man,   
(00:06:52.759) ~~how are you,~~(00:06:53.139)  
how did you survive long enough to get in front of me and do that? 


---


#### 00:06:56.482

And they're not deployed at super scale, we're not quite ready to trust them. But if you believe like the statistics from the company, and certainly my just episodic experience seems to suggest that they probably are roughly on par, maybe even better. And   
(00:07:11.098) ~~maybe we need,~~(00:07:11.678)  
maybe society is going to demand like a 10x better to actually deploy at scale. But It seems like we're there and then   
(00:07:19.014) ~~I guess.~~(00:07:19.173)  
So I don't know what their kind of unit economic and I don't know if they're there on an exception basis. I do feel with a lot of these AI things, you enter this area where you get good enough that the economics suggest that you change the environment rather than make the AI more general. 


---


#### 00:07:35.259

And I think this is probably best described with agriculture. So we don't have any unit economically viable way to pick strawberries. It's like human beings and animals have been forging food forever. We're very efficient at it. To actually compete with a human on that is very tough. On the other hand, what we can do is we can play strawberries in certain rows and we can add these optical cues, et cetera, that   
(00:07:57.911) ~~kind of~~(00:07:58.130)  
get it much closer. And so I definitely think that we're at a place where for many cases, AI is better than humans at driving, which I think is great. And I think it's a huge positive. I think these are hugely specialized systems. 


---


#### 00:08:08.379

I don't think you can take the one that's good at self-driving and make it, I don't know, be a virtual girlfriend. I think these are totally different modalities. So   
(00:08:14.586) ~~it's not general, right?~~(00:08:15.487)  
It's not general. It's just good at driving. just like something is good at chess. And now I think we're at the long tail of the problem. For fully autonomous stuff like Waymo, the unit economics are just very tough,   
(00:08:25.574) ~~right?~~ (00:08:25.694)  
They're very tough if you're competing with a human driver. For other ones, I do think that if we just start evolving how we make streets and so forth, I think we're pretty close. And I think that's great. I think this is a positive for everybody. 


---


#### 00:08:38.149

I love your comment. First of all, I love the narrowness of the full self-driving. I actually think that's a huge plus that it is an engineered system that does one thing. And I also love your comment about modifying the environment. That was actually very notable even a year ago in the FSD that the places where it got tripped up, I was like, there's an exit, the closest exit to my house off the highway has one of these service roads and has a stop sign. And it's genuinely quite ambiguous as to who the stop sign is for as you're getting off the highway. It's not for you as you're getting off the highway, but it's pointed right at you. 


---


#### 00:09:15.090

And so you can understand how it would get confused about that. And that's the kind of thing that if we're serious, we can just go around fixing these signs and we'd make it so much better.   
(00:09:23.452) ~~Can we talk, can we just very~~(00:09:24.754)  
just quick digression, because this is just so important to this discussion on how the heavy tailed universe makes this conversation very complicated between human beings, because I don't think people appreciate how heavy tailed the universe is. So I just want to describe   
(00:09:37.423) ~~this,~~ (00:09:37.503)  
because it just comes up right now. And it's gonna be so relevant to what we're gonna be talking going forward, which is,   
(00:09:41.424) ~~there are many,~~(00:09:41.865)  
there are many things that systems deal with   
(00:09:44.067) ~~that are~~(00:09:44.307)  
that are heavy tailed. 


---


#### 00:09:45.488

What heavy tailed means is, if you draw an occurrence at random, just draw one at random, the chances are is that it's a very rare occurrence. So a very classic case of this is search,   
(00:09:56.599) ~~right?~~ (00:09:56.818)  
And so if you draw a unique search query, say Google at random, the chances are it's pretty unique actually, even after all of this time. Now, this is unique searches. So   
(00:10:09.336) ~~if you draw, so if, I'm just trying, I'm trying to,~~(00:10:12.259)  
I'm trying to say this as clearly as I can. So if you take all of the searches that go into Google, say, and then you don't de-dupe them, so like you can have a lot of repetitive ones, the vast majority of searches are the same. 


---


#### 00:10:24.471

Let's say 90% of them are common. But if you reduce it to just singular intents, so you don't have any duplications, the majority are exceptions. And that's how the universe tends to be. Like, I come from networking. It's a very famously heavy tale to discipline. A lot of things in the tale. So if you're building a general system, the majority of new things it has to do, not things it has to do, the majority of new things it has to do are exceptions. Now, it's very easy to get tripped up in these conversations because the majority of the stuff that you're doing is not new, right? The majority of stuff you're doing is very common. 


---


#### 00:11:02.178

But anytime you get into new areas, then you have to come up with new stuff. And it's like self-driving is a very,   
(00:11:07.784) ~~I think,~~(00:11:08.024)  
great case of this. It's like nobody expected basically a 2D vision problem. Let's be honest, man. Self-driving is 2D. It's not even 3D. It's   
(00:11:17.712) ~~like~~ (00:11:17.852)  
you have streets and you have signs. You don't really worry about the Z dimension, really. And yet, $100 billion in, $100 billion of investment, we're almost there, but not in an economically positive way. And   
(00:11:32.827) ~~I think~~(00:11:33.087)  
The reason I want to make this point now is I think so much of these discussions is people, I believe, underestimating how heavy tail the universe is and how hard it is to make progress. 


---


#### 00:11:44.330

And so we should be working as hard to make progress so that we can do stuff like self-driving and not slow it down because the task is enormously complex. I think that's definitely a good description of where things are today in my kind of summary communications about the state of AI, I always say that the best systems are closing in on expert performance on routine tasks. And the word routine there definitely is critical, because when you get outside of routine tasks, they are not comparable to expert performance. Okay, so let's move this to here. So as far as I can tell what LLMs are doing, And there's actually papers that have shown this pretty concretely, is they take a corpus of data, they create positional embeddings, and they basically average over it. 


---


#### 00:12:38.436

And based on that, they can predict what a human being would do or say given a certain situation. And they do that basically via averaging. For 80% of the tasks, let's say that's great.   
(00:12:55.904) ~~This is for 80% as far as non-unique, right?~~(00:12:59.787)  
So you're not deduping tasks. But let me give you analogy. What if I came to you, I'm a startup founder, I'm like, hey, Nathan, I've got this amazing chat bot that for IT help tickets, it answers 90% of the time. And you're like, this is amazing. Like 90% of the work goes away, right? This is what you say. But then you actually do diligence on my company and you realize   
(00:13:23.380) ~~that~~ (00:13:23.701)  
That 90% of that, 85% of that is just answering password resets. 


---


#### 00:13:30.408

So I was factually correct saying that 90% gets answered. That's the case. But the reality is the situations that I help with are very easy to automate if you wanted to. And they're not that much work. And you still have, from a unique standpoint, you still have to have humans do 50% of the unique things that come in, 50%. So that was the state of chatbots for the last 10 years. And we had the exact same discussions. They seem to answer 90%. They answer 85%. They can do these things. We're almost done. But that's not how heavy tail distributions work. So again, so let's go to this case that you're making. A hundred percent, these LLMs solve problems we couldn't before. 


---


#### 00:14:09.225

And a hundred percent, they're a very useful computer science primitive. we're nowhere close to understanding what these distributions look like, how heavy tailed they are, and how they can handle that tail, just like we weren't with AV, just like we weren't with original chatbots. And so I just think that without being specific on uniqueness and the distribution and whether we think it's parametric, it's very hard to have these conversations. So we resulted generalities that sound good, but I think from a system standpoint, aren't very. So   
(00:14:41.453) ~~what do you think?~~(00:14:41.913)  
How far do you think this goes? Best guess, if you are imagining yourself in 2027 and you have your AI assistant, can you say, hey, 


---


#### 00:14:53.500

I'm going to New York next week for this event, here's the invitation, book me a flight, book me a hotel, and get a good result? I think it's going to be like self-driving. I think we'll get 80% there with these agentic systems and then people are going to start changing the environment to make them more effective because human output is also heavy tailed. And   
(00:15:18.827) ~~so my, my,~~(00:15:19.868)  
my best guess. Again,   
(00:15:21.428) ~~I'm going to, I'm sorry,~~(00:15:21.948)  
I'm going to repeat myself, but I actually think that's how it's going to play out is right now we're anytime we're always at   
(00:15:27.030) ~~like~~ (00:15:27.150)  
the beginning of what looks like an exponential, but there's actually a sigmoid. And what we think is like a fat head system, but it ends a heavy tail system. 


---


#### 00:15:34.332

It always feels like this, like it feels right now. And everybody's saying all this stuff that they're saying right now. And we're like, it's amazing.   
(00:15:38.875) ~~You know,~~(00:15:39.075)  
everything's going to work out and then we're going to realize, oh my goodness, the universe is heavy tail. This is really hard. These things are good at 80% of stuff, but the 80% of stuff that it's good at. is not that hard. And the stuff that I need it to be good at is really hard. And so then we're going to enter an area that we're like, oh boy, we talked about scaling laws, throwing 10 times more compute at something over a period of time is so impossible that what we're going to do is we're going to actually change the way websites work. 


---


#### 00:16:04.211

And we're going to actually have indicators and we're actually going to have lanes. And then we're going to spend the time actually changing the systems. And so over time between changing the way websites work and where these agents work, we'll enter a period where these things are more autonomous. don't think it's because we've cracked the generality problem. I think it's because we've evolved computer science as a discipline and tech and software as an industry in order to solve the problem. What do you make of these sort of, I find language to be a confusing domain in some ways because there is so much, it's   
(00:16:40.229) ~~like~~ (00:16:40.350)  
hard to get truly out of distribution in   
(00:16:42.990) ~~like~~ (00:16:43.150)  
interesting ways where it's like very hard to say, is this, can write a sonnet about the NBA finals or whatever. 


---


#### 00:16:50.625

And that's definitely out of distribution, but you could say it's interpolating between things in distribution. Sometimes I'd like to just go to things that humans can't do. So when I look at things like,   
(00:17:00.710) ~~I don't know if you've studied~~(00:17:01.409)  
Evo, the early foundation model for DNA sequencing, It's an interesting one. I did an episode just yesterday on models for basically simulating solutions, like salt solutions. And in both of these cases, you see these sort of remarkable generalization moments where in the Evo case, it's trained on DNA sequence data, just like bacteria and phage data. And so it's next token prediction, it's next base pair prediction. Same thing as a language model, right? So you could say, oh, it's only predicting the next base pair. 


---


#### 00:17:36.913

But like the language models, it seems to have developed these higher order internal representations that mean something that it was not specifically trained to learn, but that it's learned in service of making the next base pair prediction. And one of the experiments that they did that is so striking to me, this is from the Ark Institute, they did what they call gene essentiality scoring, where they basically say, we'll give you a gene sequence and we'll perturb it. And then we'll look at your perplexity, your being the model, your level of confidence or uncertainty downstream of that prediction. If you remain confident, then we can believe that gene must not be super essential. Cause if it gets messed up, then you can still predict like how this fits into life. 


---


#### 00:18:24.628

But if you, if we make that change and then you become very, radically unconfident in your downstream predictions, then we can infer that this gene is actually really important because now when it's off,   
(00:18:35.494) ~~like~~ (00:18:35.654)  
now you have no idea, now you recognize you're out of distribution and you can't make any confident predictions anymore. It seems to me like that signals, and that's like a 7 billion parameter model, 300 billion tokens, that's 2% of what LLAMA, or 1.5% of what LLAMA 3 is trained on. So it does feel like there's some potential in these systems to learn things that we don't know, to grok, if you will, patterns in the universe that are   
(00:19:08.167) ~~like,~~ (00:19:08.367)  
not known to anyone really, to essentially speak DNA. 


---


#### 00:19:12.913

Yeah, sure. So if you buy all that,   
(00:19:14.595) ~~like, how does that,~~(00:19:16.037)  
how do you backport that to language? Because I feel like I start to see,   
(00:19:21.410) ~~well, maybe there are,~~(00:19:22.351)  
we're just modeling the economy or modeling software. I do start to see things. If you were to train, keep scaling and keep training these models on distributed systems or software or whatever, how do we know that they don't start to learn things that people don't know and truly generalize beyond the training set? Because it does seem like that's happening in some profound way.   
(00:19:42.886) ~~I think that's a great question. I think maybe this is why I come to this from a different thing.~~(00:19:47.170)  
Prior to my PhD, my life was computational physics. 


---


#### 00:19:50.971

I worked at Lawrence Livermore National Lab. I did large physics simulation. I just lived this life. And I think the Occam's razor in all of this is distribution in, distribution out. These things are very good at learning distributions of the training set. And so this is just into this kind of weird, quirky coincidence of this moment. I actually worked on protein folding at IBM T.G. Watson Research Center in 1999 on the Blue Team project. And at that time, there was a belief that we knew enough of the fundamental forces in order to actually, from first principles, calculate protein folding,   
(00:20:30.258) ~~right?~~ (00:20:30.377)  
That was the thesis, and that we just didn't have enough compute. And so they actually built a whole computer to do this called Blue Gene. 


---


#### 00:20:38.622

And through corporate machinations, that ended up becoming an entirely new computer because they couldn't fund it. It never really happened. But there was the belief that if you had enough compute that you could do protein folding and a bunch of other stuff. And so I think it's very reasonable. This is just strict Occam's razor that if you have enough compute and you have enough data and you're dealing with an axiomatic system that you can reduce to first principles, then you will learn that distribution and you can use it for predictive stuff. And if you want to call   
(00:21:08.461) ~~predictive~~ (00:21:09.383)  
emergent, that's fine. But it's just predictive, like anything is predictive. Like I've worked on simulations codes that were predictive. 


---


#### 00:21:15.086

Could I have predicted the yield of a nuclear weapon? No, I could not have predicted that as a human being. Only a computer can. But it's really just understanding first principles to create these things. I very strongly believe these models are very useful. In science, where you've got fundamental laws of nature that are being learned that can be predictive, I think the models that are good at that is not going to turn around and solve a different problem, most likely, because   
(00:21:43.526) ~~I think~~(00:21:43.786)  
you've probably learned one distribution from one domain, and that's a very useful tool that we should use. Now let's go ahead and move that over to language now. So if my Occam's Razor is these things learn structure in a data corpus. 


---


#### 00:21:57.259

It's distribution in, distribution out. That means that they're learning structure of the text corpus that they've been fed. And   
(00:22:07.067) ~~I think~~(00:22:07.288)  
a great example of this, there's a recent paper I saw, I don't know if it got accepted or not, I think it was just on archive, but that showed that if you could gzip a text corpus,   
(00:22:16.316) ~~do you see this?~~(00:22:17.016)  
And the compression was good, then the accuracy was good. Which suggests almost everything you need to know about this, that all it's doing is learning structure in the text. It has nothing to do with underlying meaning, it's just structure that's in the text. And so you can understand the distribution of text. You can actually spit out text. 


---


#### 00:22:36.271

But this doesn't say anything about learning fundamental principles of the world from which the text is based. And so it almost seems to be that the magic in this sequence of texts is you've got these humans that have spent, say, 3,000 years looking at the universe. And the universe is, again,   
(00:22:53.319) ~~like~~ (00:22:53.440)  
heavy-tailed, and it's nonlinear, and it's very complex. and it's fractal and it's self-similar. And these are notoriously complicated systems to simulate. So then the human brain is, I'm going to abstract this out as a tree. And I'm going to abstract this out as like this concept. And so we're like these machines that take the universe and abstract it into things that are words. 


---


#### 00:23:14.369

But it's a very lossy representation.   
(00:23:16.010) ~~Like you can't~~(00:23:16.471)  
You can't describe something and get back the universe. But it turns out, because we have those abstractions, they're very predictable.   
(00:23:23.035) ~~Like,~~ (00:23:23.154)  
we've made the universe more linear. And we've made the universe less heavy-tailed. And we've made the universe less self-similar. And once we've done that, we've added structure that's predictable. So the fact that you can take a corpus of text, which a human being has pulled from the universe and then made the universe much simpler, and find structure in that is not surprising at all. But to think that somehow then you can go from that to the universe is a step that just simply has not been demonstrated. 


---


#### 00:23:49.914

And it actually, it doesn't even stand to reason. Two follow-ups there. One on the question or the subject of meaning. How do you square the idea, if I understood you correctly, you're saying that doesn't mean that they have any understanding of meaning. How would you square that with a sparse autoencoder line of research or sort of Golden Gate Claw, if you will? Like they're able to now say, these sparse auto encoder techniques that they can isolate, I think it's 30 some million different features, each of which is a direction in activation space, and then inject those at runtime. And they're starting to create these sort of control mechanisms where it's like they jack up the Golden Gate Bridge feature, then all it wants to talk about is Golden Gate Bridge, or more practically, insert kindness or insert, you know, deviousness or whatever. 


---


#### 00:24:42.786

There seems to be some meaning there. There's structure. That's very different than meaning. So we're talking about three things. And this is a great conversation, because   
(00:24:51.471) ~~I think~~(00:24:51.631)  
it gets to the heart of it. So the universe is self-similar. It's fractal. Meaning no matter what zoom level you look at it, it has the same stochastic properties, right? So   
(00:25:03.503) ~~like~~ (00:25:03.644)  
you can spend an entire life studying a cell and a planet, right? That's how much complexity is in the universe. The universe is heavy-tailed, which means the exception is the norm if you dedupe. And it's nonlinear, which means that you can't computationally predict out too far just because we don't have closed form solutions for nonlinear stuff and it's just a very hard computations problem. 


---


#### 00:25:25.163

That's the universe. Now, human beings have had to navigate this crazy universe. And so we've created this amazing engine, which is the brain. And it has reduced this universe to,   
(00:25:37.030) ~~like,~~ (00:25:37.171)  
concepts and words and stuff that we use and we talk about. That kind of makes it a little bit predictable. And so at least you and I can communicate about it. But if I tell you like, this is a tree. There's a concept tree in my brain. But   
(00:25:49.955) ~~that's a,~~(00:25:50.395)  
it's almost an arbitrary distinction that it's a tree.   
(00:25:54.258) ~~Like,~~ (00:25:54.417)  
I could talk about branches versus leaves.   
(00:25:57.339) ~~I took about,~~(00:25:57.921)  
could talk about networks of trees. That's actually one tree, like the big aspen grove. I could talk about cells of the tree. 


---


#### 00:26:02.943

It's like this kind of arbitrarily useful distinction. So it has some semblance to the real world. But if I say a tree, it's probably not an accurate relative to how the world is. Is it one tree? Is it a family tree? It's just a useful abstraction. So these models will 100% recover the abstractions that we've put in text because the structure is all there. That's not surprising.   
(00:26:26.671) ~~Like,~~ (00:26:26.790)  
compression would do that. All it's doing is taking advantage of structure, and that structure is real. But let's say that it's finding a tree. Does a tree actually map to the universe in a meaningful way? It's a human-created concept that has some vague semblance to something we all agree on. 


---


#### 00:26:43.435

Unless you're a scientist, then you probably disagree with the common understanding. And oh, by the way, my concept of a tree also includes a toy and a cartoon picture of a tree, which is entirely different. And so text is a way that we as humans represent the world that's very different than the actual universe because we find it useful. There's structure there. And these LLMs are exploiting that structure just like compression would or anything else. And it's very useful for us. But it doesn't necessarily mean that these things can enact on the world, right? These are very different domains. Yeah, I guess I'm not quite getting the gap. There's so many interesting results to point to recently. 


---


#### 00:27:25.807

Did you see the one about GPT-4 finding and exploiting new zero-day exploits? This was just in the last week or two. And it's increasingly impossible to keep up with everything, so I don't expect you've seen everything. No, that one I have. I actually think, so my two minutes, and I think when you're dealing with this much compute, and this much data, I think the human intuition just totally fails. And we as humans are really bad about thinking in distributions. Anyway, this is not how we think. We assume the world is parametric. We assume, and by the way, which is why the text that we create is so well structured and why it could be exploited by LLMs. 


---


#### 00:28:00.038

Like you have to navigate this universe. You have to make the simplifying assumptions, which we do. And so it's good to actually come up with mental frameworks about how these things work. So I'll tell you a few of mine. The first one of mine is, as far as I can tell, these things are explaining structure in whatever data that they're reading. And   
(00:28:17.894) ~~like~~ (00:28:18.054)  
we've mentioned before, and it's not clear whether that distribution extends beyond that. And if it does, then you're basically back to simulating the universe, which I've spent a lot of time with. I think that's very tough. The second one is the actual mechanisms. We're talking about transformers. The actual mechanism is basically kernel smoothing. 


---


#### 00:28:34.374

It's averaging. Which means to me is the further you get out to where the data is rare, the greater the inaccuracies come. And that doesn't mean that for systems that you can actually extrapolate from, that you don't get great results. That would be, quote unquote, out of distribution. It turns out some systems are linear, or you have enough data, you can map the distribution. So that one is totally fine. Now, the third one is this in-context learning one. And   
(00:29:00.144) ~~I think~~(00:29:00.345)  
Vishal Mishra, who's a professor at Columbia, did the best work on this, where he actually shows that for in-context learning, where you actually put the context in the prompt and you can move the posterior distribution to get interesting results, he mapped it specifically to Bayesian learning. 


---


#### 00:29:15.944

And it's a beautiful paper. I don't know why more people don't read it. So   
(00:29:19.128) ~~listen,~~ (00:29:19.348)  
we know that these things can do some basic Bayesian reasoning. And this is where the prompt is basically the new evidence, which changes the posterior function. So you'll get new stuff there. We know that if you average enough stuff, You'll get new stuff there. It just has to be linearly interpolatable. If it's not linearly interpolatable, you're not going to get new stuff. So none of these things suggest that you're not going to get new stuff. It just puts constraints. We know how Bayesian systems work. We've got 20 years of understanding convergence properties to them. We have a work that's specifically mapped ICL to Bayesian learning. 


---


#### 00:29:54.846

So let's just go ahead and use that corpus of work to understand the properties. It doesn't say it's out of distribution or indistributed. It doesn't say that at all. It just bounds what that means. And then we also know the mechanics of the way Transformers works, which is this kernel split. It's more complex than that. And so that can create new things, but it means there's a linear interpolation. And so   
(00:30:16.763) ~~I think~~(00:30:17.184)  
the problem is we have these anecdotal conversations where it's whack-a-mole. It feels almost like the intelligent design discussions where someone will come up with a new set of evidence of something that there's no way evolution could have created this. to spend all of this time to show actually you can but we don't know everything and here's the theory and   
(00:30:36.810) ~~i~~ (00:30:36.891)  
i feel like when we have these discussions it should be a bit more principled as opposed to i've got this anecdote that seems something's new because nobody says that you're not going to see new stuff it's very obviously if you're doing interpolation it's new very obvious if you're doing Bayesian reasoning, like something's going to be new, and talk more about the distributions and the theory of why we're doing that. 


---


#### 00:30:56.249

But as far as I can tell, that's totally missing. Nobody's come and said, here's my theory of out-of-distribution stuff. Here is my thesis for what is going on functionally to create this new data. And on the other hand, you've got   
(00:31:10.592) ~~mounting and~~(00:31:11.071)  
tons of evidence that map these to existing systems that we know. that people just seem to not want to follow. And I just feel like, listen, humans love to see things in clouds and complex systems. Clouds are   
(00:31:22.063) ~~like, they're just,~~(00:31:22.803)  
there's so many facets, and they're so complicated, and they're so huge, and they're so ethereal, and then we see things. And we just do this historically. And we've got these kind of amazing compute elements that are huge. and they surprise us, and they're amazing. 


---


#### 00:31:38.253

But we can map them to formal systems, and we know how they work. And that doesn't mean that they're dangerous or not dangerous. I'm not saying that. I'm just saying that we can actually map them to reasonable systems to have a discussion. And that just seems to be missing. This conversation is a great example. I'm very happy to map these things to formal systems. We understand and have that discussion. But it's always this kind of anecdotal whack-a-mole instead, which I just don't know how to answer to every instance of what seems like emergent behavior, when, of course, emergent behavior is expected anyways. Yeah. There's a lot there, obviously, to chew on. I didn't mean to rant so long. 


---


#### 00:32:10.811

No apology needed. But I am definitely a materialist. And so I do believe that in the fullness of time, we can probably figure out in an arbitrary level of detail how these things work. They're actually way easier to study than life, for example. Of course. And I would say we've made tremendous progress in interpretability and general understanding paper you mentioned is a great example. I've seen another one too that's pretty similar where somebody designed a matrix implementation of gradient descent and then looked for that in the wild and found it. I thought, look, these things have learned to implement gradient descent at runtime and that's another kind of mechanism, at least sometimes, probably have different mechanisms and different models. 


---


#### 00:32:54.951

And there's this various, almost like phase change type of dynamics that are being explored too, where even for something as simple as like the modular addition grokking, there's like multiple algorithms that it can lock into each of which work, but they're different. And so there's memorization and then there's multiple like actual algorithmic solves and which one you end up with depends on initial conditions. So   
(00:33:17.388) ~~there's, I do believe that we,~~(00:33:19.230)  
I don't think there's any magic in the machine. I'm definitely with you on that. It does seem that, in principle, we should be able to figure it all out. It doesn't seem like we've made a lot of progress, but it doesn't seem like we're that close to having it all figured out. 


---


#### 00:33:33.346

On the sigmoid question, I tend to also agree that it does not seem like there's reason to believe that this is going to be an exponential forever. It does seem like it probably levels off. But then I'm also reminded of the old joke of two guys in the woods and the bear is coming and the one's putting on his shoes and he says, I don't have to outrun the bear, I just have to outrun you. And so I do wonder if we imagine continuing to scale up as we have been scaling up and there's all these trend lines and times more compute and however much advantage from algorithmic efficiency or whatever. I was just talking to somebody at one of the   
(00:34:10.010) ~~I guess I'll just say~~(00:34:11.070)  
generally one of the top five hyperscalers in the world, and they are using a new replacement for the Atom optimizer that is giving them something like 30% savings on compute. 


---


#### 00:34:23.802

This was published open source, the technique is called SOFIA, and it's just incredibly 30% off the top. You're saving   
(00:34:29.306) ~~like~~ (00:34:29.385)  
$100 million on the biggest runs. Anyway, let's imagine we continue to scale up and it's a few more orders of magnitude. And let's say we don't just put in the text, but we also put in like this sort of low level solution data and the protein, you have the DNA data and the protein and the gene expression. And we work our way up all these levels   
(00:34:47.911) ~~of,~~ (00:34:48.012)  
of orders of magnitude. And then it's like computer systems, like all the cloud logs from AWS and Google cloud and all this stuff gets in there. And you've got all these different self-similar but overlapping orders of magnitude of ways of understanding the world. 


---


#### 00:35:06.101

I have a hard time imagining how that doesn't, even if it asymptotes or levels off at some point, I have a hard time imagining that doesn't level off at a higher point than human is able to achieve today. But I feel like you probably see that differently still. So a lot of this reduces to how you view the universe. If you don't view the universe as fractal self-similar, and if you don't view it as heavy-tailed, and if you don't view it as non-linear, then you could imagine that. But it is all of those things. We know it is all of those things. And so there's no distribution of data that we know of that's not the universe that will produce something that's predictive of the universe. 


---


#### 00:35:48.413

It's really that simple. That doesn't mean that we can't focus on an area and reproduce that distribution. I could become very good at predicting whatever, protein folding. I could get really good at playing chess. But it's distribution in, distribution out. If you notice the ones that stuff like recursive self-similarity works, and control loops work, and simulated data works, like synthetic data works, there are these axiomatic areas where the axioms   
(00:36:19.536) ~~define,~~ (00:36:20.115)  
like they constrain the search space and you're basically converging on search. And you can get very good at those. I can get much better at unit arithmetic. I can get much better than you at game playing. I can get much better at humans at all of these things. 


---


#### 00:36:31.226

But none of that None of it talks to the fact that can you find the right level of abstraction in a fractal system and can you tackle a heavy-tailed universe where not by occurrence, but by uniqueness, the complexities in the tail. And there's just zero. Even in this discussion, the use cases that you've used tend to be these kind of axiomatic. Of course we can do full search. Like we thought in the late 90s we could do protein folding by fully searching the search space. It's just not surprising to me that we can learn distributions and spit them out. I feel that's a very different statement than saying, now we have a model that can navigate the universe in a way that is predictive of all of the complexities of it. 


---


#### 00:37:22.666

I think maybe another way to think of this is we've spent 3000 years doing our best and writing it down. And we can create a model that can learn from all of that and do what the mean human being would have done in the last 3000 years. But the problem is the stuff that we're doing tomorrow by uniqueness, a lot of it's going to be new. And that's just how the universe works. And we're going to have to either build a machine that can do that, which we don't know how to do, or we're gonna have to do it ourselves, and let these machines do the mean task. So Do you have an account of, or a theory of, what it is that you think humans are doing that the models can't do today? 


---


#### 00:37:59.114

Because, yeah, so tell me what it is. Yeah, yeah, yeah. Two things, two things. One of them, and the most important one, is we experience the universe and we abstract it into concepts. That's very common. Why do you think all the budget is moving to post-training, by the way? What's your thesis of why so much budget right now is moving from compute to post-training? Ease of use is a huge one. I guess, I don't know that I necessarily think, I would still guess it's probably a minority of budget. If you're talking like, 400. I don't know. Listen, they had, they said they had 10 million messages. I know how much multi-pass costs. Let's say it costs $15. 


---


#### 00:38:37.777

Like we're talking a budget between a hundred and 200 million, which anecdotally it seems about right based on what I know of the industry. But yeah, that's about half. And so what I would argue is we're very good. Models are very good at taking the output that humans create and being able to reproduce that distribution. They're very good at that. This is why Scale.ai is Scale.ai, and all these companies are so successful. That's not the game. The game is looking at the universe and creating the supervised data. That's the game. And so I think one model to look at this is, again, human beings have been around, let's say, in a capacity for writing things down for 5,000 years. 


---


#### 00:39:18.971

So you've got humans for 5,000 years that have been looking at the universe and doing this thing that models cannot do, which is making a decision like, that is a rock, and that is a dust, and this is a concept, and this is a relationship, and I'm going to write it down. And then as a group, we're going to synthesize these ideas and work at these. And so we've got this almost platonic representation in our heads. of the universe, and that is very structured. So we did all the hard work. That is hard work to take this untamed universe and reduce it into words and concepts. That's hard. No LLM that I know can do that. 


---


#### 00:39:55.251

Not even close. But then once we've done all of that hard work, is it surprising to you that there's structure? We did all this work. Of course there's structure. So you take that structure, you put it into an LLM, it learns the structure, and it can spit it back out. So the very specific thing that these LLMs can't do is look at the universe and recreate this kind of structure. And to be super clear, that structure is not the universe. That's very different. Like a rock is a rock. It's an idea in our head. It's not representative of any single thing. Is a grain of sand a rock? I don't know. Is a boulder a rock? 


---


#### 00:40:28.099

I don't know. These are concepts we've created in order to navigate the universe. They're not the universe. So human beings take the universe and create the concepts. And that's structured because we need structure in order to do anything. And the LLMs learn that structure. And I haven't seen a shred of it. This is why all of this feels like the only thing that works is basically you can do exhaustive, quote unquote, AI, which converges on search to learn distributions. Or you do supervised learning, which human beings are doing the hard work, in my opinion, by labeling things and everything else. And then you just learn what the human beings have done. But to take the universe and actually to reign structure and all that complexity, that's what we do. 


---


#### 00:41:05.664

And it would be great if machines can do it. I've never seen any evidence that they can. Yeah, maybe some glimmers of it, but that's just not where we are. I just want to be super quick, because you asked me a very specific question, a very specific answer. Look at the universe, and then come up with these concepts that are useful, that are not the universe. They're concepts. They're totally separate. Like a rock is not a thing. It's a human concept. But to take the universe and decide something is a rock, that's actually all of the complexity and all of the energy is that step, which LLMs just don't do. Yes, this is why I think language is such a tricky domain. 


---


#### 00:41:42.094

By the way, the platonic representation, you probably saw there's a paper titled exactly that recently. But it doesn't tell us much about this particular question because it is still operating in the language domain. And it is in that way able to piggyback on our prior art in terms of useful abstraction of the universe. I do think if there was a line of research that might, where I would venture a guess, that I think you maybe wouldn't agree with, that maybe we could come back in a certain finite amount of time and say, has this happened or not? And what would we infer from it? I probably would look at this biology foundation model space and the sequence modeling. 


---


#### 00:42:27.190

And you can imagine that's going to be elaborated a lot. They didn't even use eukaryotic sequences in that initial Evo paper, let alone   
(00:42:35.177) ~~like~~ (00:42:35.378)  
expression data, transcriptome, proteome, whatever. But   
(00:42:39.262) ~~I guess my expectation would be... I just, I would be very,~~(00:42:42.083)  
I very much agree. We know enough about the natural sciences to build predictive models and we have for a very long time, right?   
(00:42:49.447) ~~Like~~ (00:42:49.628)  
I can simulate a supernova on a computer pretty accurately.   
(00:42:57.289) ~~I think it's phenomenal.~~(00:42:58.688)  
It's phenomenal that we have an approach to throw a computer at a problem that learning a fundamental law of physics. But again, how is that any different than the fact that we've been modeling physical systems for a very long time other than the fact that In these cases, it allows us to apply more compute at the problem because we don't have to, and we can solve problems that we don't have close form analytics solutions to. 


---


#### 00:43:24.735

It almost feels to me like an extensive of simulation, which would be very different than the claims around general reasoning. It's literally learning laws of physics, which we've been doing since the beginning of compute. The creation of computers was for ballistics. So the reason that we created computers is because ballistics are nonlinear. The trajectory of ballistics are nonlinear. So we had people in rooms that would create logarithm tables by hand. They were called computers. That's where the name came from. ENIAC shows up. ENIAC does it four orders of magnitude. It was about 5,000 times faster than a human being does it. And we have a computer. And this is a perfect example of a nonlinear system, which is a trajectory with gravity. being done by a computer. 


---


#### 00:44:05.722

Why is this not just a straightforward extension of exactly that, like we've been doing for the last 80 years?   
(00:44:12.467) ~~I think we're,~~(00:44:12.927)  
here's my expectation. Tell me if you, maybe we can make a little friendly wager on this. I think that over the next year, we are going to start to see scaled up foundation models for biology that are going to start to understand the super complicated interactions between genes, between proteins in cells, in ways that are inferred from inputs and outputs, learning these higher order concepts in the middle, which we could not simulate because it's computationally just intractable, and which we don't have any closed form, certainly don't have a closed form solution for either. 


---


#### 00:44:58.438

If that does happen, that would seem to constitute to me an instance of looking at the world, looking at basically raw data of sequences and just lysed cells and what proteins were found in them and whatever, and learning meaningful abstractions. And   
(00:45:15.949) ~~I think we,~~(00:45:16.331)  
I would expect that we'll start to discover stuff by doing counterfactual experiments on those models. In other words, tweak a thing, see what happens. Find medicines, find disease patterns by make a tweak, see what happens. What if we change this counterfactually and then go validate those things in the wet lab? If we start to see that happening, would that, to you, represent the phenomenon? I fully expect that. But how does that not constitute looking at the universe and figuring out what's what? 


---


#### 00:45:47.891

Oh, for sure. For specialized subdomains, you absolutely can learn distributions. A hundred percent, right?   
(00:45:53.635) ~~Listen,~~ (00:45:53.856)  
I've implemented Navier-Stokes, like fluid dynamics.   
(00:45:58.199) ~~where,~~ (00:45:58.579)  
and this is a turbulent chaotic system. So we've known how to   
(00:46:02.083) ~~like~~ (00:46:02.304)  
implement very complex systems with computers, for sure. And especially in very specific domains where we can reduce these things to a few fundamental forces or we can reduce these things to mostly linear systems. Like finite element is, like the previous version of this is just all the computational methods where we would take a problem that we know and we'd actually experimentally determine It says experimentally, we'd say, okay,   
(00:46:27.385) ~~like this,~~(00:46:27.786)  
this material behaves this way under this pressure and this heat, and it has these properties. 


---


#### 00:46:31.730

And we take what we learned experimentally and we'd create these models and they would do pretty good at simulation. And I would say this is a very straightforward extension of that, which is you look at how the world works in a constrained situation. And then you can predict what would happen in the constrained situation. But just like simulations,   
(00:46:50.389) ~~remember,~~ (00:46:50.630)  
we could do this with simulation. We've been able to do this for a very long time, right? So you could experimentally determine how different materials work, and then you can actually simulate a new system based on those. This is how we do most industrial design today anyways. So my question to you is, how is this fundamentally different than that? or not a natural extension than that, where you're giving it a system, you're learning some fundamental properties, you can do something new. 


---


#### 00:47:16.719

But that doesn't mean that you can disobey the laws of physics in predicting stuff that computers can't predict. It doesn't mean that all of a sudden   
(00:47:24.862) ~~they can like,~~(00:47:25.302)  
it's not obvious to me that it can simulate complex nonlinear systems that are chaotic for long periods of time. I think this is just yet another step on this kind of   
(00:47:37.436) ~~like~~ (00:47:37.576)  
we have computers simulate physical stuff and we're simulating the next thing with the next tool. Does the parallel making make sense? If you go to like in the 80s and 90s, we would literally empirically test physical matter. We didn't know how the physical matter worked. We didn't empirically test it. It has this opacity under this heat. 


---


#### 00:47:58.106

It has this tensile strength. We'd use that to build databases of materials, equations of state, we call them. This is how they interoperate. We'd use those when we're doing simulations. And we'd simulate what happens when a car explodes, what happens if an airplane runs into a building, all of these things. None of those instances worked. They were simulations. And they were very accurate. And none of them came from first principles. They were all empirically. But that has its limits because it didn't solve climate prediction past 15 days. It didn't allow us to simulate life. And so to me, this is just computers being attached to another domain, which thank goodness we've come up with a great tool that's going to give us a little bit more insight. 


---


#### 00:48:40.630

But it's a little bit more insight is what it is.   
(00:48:43.775) ~~By the way,~~(00:48:44.036)  
we had the same discussions in the simulation.   
(00:48:47.737) ~~This is why,~~(00:48:48.197)  
by the way, we stopped Playstations from going to the Middle East. I actually worked in the nuclear weapons program at Livermore, so I was very close to the previous version of these discussions,   
(00:48:58.760) ~~like,~~ (00:48:58.880)  
oh my goodness, if   
(00:49:00.800) ~~like~~ (00:49:00.940)  
Saddam Hussein gets PlayStations, he's going to be able to simulate nuclear weapons,   
(00:49:04.764) ~~right?~~ (00:49:04.943)  
Like just totally misunderstanding that the ability to simulate something is not some runaway process that's going to allow you to recreate a world or anything like that. It's a very specific tool for a very specific situation. But we were here before when it was 25 years ago. 


---


#### 00:49:23.056

Yeah, there's certainly no arguing that past predictions of AI progress often didn't pan out and that does seem like it's not a near-term future that we can dismiss either. The other argument is that they have all panned out exactly as you'd expect, and they're going to continue to. And this has been steady progress for 80 years, and it's been a super useful tool. And every time we unlock something, people are like, oh, poo, that wasn't AGI, so that must not have been AI. And they're focused on the wrong goal, and it's a very unspecified goal. And instead, it's like any other computer science primitive. where it keeps solving problems and we should continue to solve problems with it, which is the way that I would view it. 


---


#### 00:50:02.342

It's interesting because people talk about summers and winters and not panning out like you just did, but it couldn't be further from the truth. It's been a foundational primitive of computer science that we've been using very effectively and we continue to use more effectively and I don't see why that won't just continue to be the case. Yeah, I like your vision. I think what you're describing is almost an ideal scenario. And   
(00:50:24.887) ~~I think we've,~~(00:50:25.527)  
I spent more of the time that we have today here than I had anticipated, because I wanted to get into all these debates around SB1047 and compute thresholds.   
(00:50:33.329) ~~We've got half an hour. We have half an hour now. So we, yeah, we have half an hour.~~(00:50:37.489)  



---


#### 00:50:37.530

We can dig into it. But I do think this is an important foundation. Let me try to bottom line your perspective. It seems like you,   
(00:50:47.572) ~~I'm still a little confused around what would count. Is there,~~(00:50:52.737)  
what would be the evidence of the fundamental thing that humans can do and have done through our history that the AIs can't do is look at the universe and figure out the right abstractions and come up with   
(00:51:03.884) ~~the~~ (00:51:03.963)  
the right concepts that compress it in order to make sense of it. And I agree it's very hard to say what they're doing in the language domain because we already did that work and they're learning it from us. I try to describe something in the biology domain where it's like it seems like they're starting to show signs of doing that and I could believe that they would and then you agreed, but then now I'm confused as to wouldn't that count as doing that? 


---


#### 00:51:22.532

And then it seemed like the response was, well, that's just in one domain, but it doesn't seem like there's anything that would prevent it. Certainly there's a huge leap in generality with this latest generation of systems. So I do imagine just shoveling all the modalities into one model. We've already got text, vision, and audio in GPT-4.0. Why not the true GPT-5.0 would be like biology data and weather data and like pictures of deep space and solution simulations and just battery simulations, material science, whatever. Throw that all into one thing. And if it can do that, then it's definitely not going to be constrained by one domain anymore. So I'm still a little lost as to like exactly what the limit that you see is in terms of why it doesn't become a system that's more powerful than people. 


---


#### 00:52:07.920

I'm so glad you reduced it to this. I think this is great.   
(00:52:10.039) ~~Right. And there there's two things.~~(00:52:11.380)  
There's this notion that language reasoning is general,   
(00:52:13.621) ~~which you,~~(00:52:13.900)  
which a lot of people believe, but you don't seem to be on that kind of. So let's put that one aside. And you're more on the learning properties and simulating properties of the universe side, which is totally fine. So what I would do is I would just bring you back to everything we've learned about simulation, which is even when you know all of the properties of the system and you can simulate, You just don't have the computational capacity to simulate nonlinear systems. We don't have the materials or the energy or anything. 


---


#### 00:52:44.617

It's literally like a compute problem. We have code bases that have been around for 20, 30 years that simulate all sorts of crazy stuff. And yet, they've got limited utility for exactly this reason. The universe is just so complex that they're useful for a little bit. And   
(00:53:02.114) ~~so~~ (00:53:02.253)  
if it turns out, and I'll give you a very specific one that we can bet. If it turns out that these models somehow change that compute trade-off where it can simulate nonlinear systems in ways that traditional stuff can't, I'm 100% with you. But that's not what they're doing. What they're doing is they're inferring stuff that we haven't been able to infer by looking at data. That doesn't mean that they can be predictive in a way that kind of disobeys our understanding of compute requirements. 


---


#### 00:53:34.980

And like a Raleigh-Taylor, let me just give you a specific, so Raleigh-Taylor instability is basically if you have two liquids that are on top of each other with different densities. And that is one Raleigh-Taylor unstable system. And if you perturb it, like you get these kind of   
(00:53:50.614) ~~like~~ (00:53:50.755)  
just amazing kind of chaotic turbulent things that happen. Like we have been looking at this problem for 30 years and we have no idea how to actually predict what will happen. We just know roughly what they will look like, but we don't know   
(00:54:04.465) ~~like~~ (00:54:04.606)  
the specifics. And AI systems are way less efficient than an actual code written for simulation. So to think that it can tackle those types of problems, 


---


#### 00:54:14.942

I just don't see any indication. So maybe I'll just say one last thing, and then we can move on, which is I view that we have these kind of modalities of compute that we can throw at problems, right? So the most efficient is basically imperative programming, where you give   
(00:54:28.351) ~~like~~ (00:54:28.530)  
the computer, like a set of instructions and exactly the rules, right? So that's just normal programming. And then we have another modality, which is declarative programming. And by the way, the first one's the most efficient, right? It just does the rules. The second one is the end state that you want. I know the end state, but you know it very specifically. And then the computer figures out what to do. 


---


#### 00:54:48.126

This is declarative programming. To come to the solution, it has to do all of the logical closure stuff. So that requires more compute. And we don't even know how to bound that compute. That's why databases, when you run queries, are not bounded. So that's declarative programming. Now we're in AI, where you don't even know what the end state is. You're just like, I have a whole bunch of data, and I want you to find patterns in that data. That requires even more compute, so it's even less efficient. So it's another modality of compute. It's one we've been fighting for a long time. But it doesn't change the nature of computers. They're still systems, and they're still computers. 


---


#### 00:55:21.702

And they still have the same limitations, independent of what distribution that they learn. And   
(00:55:26.284) ~~listen,~~ (00:55:26.525)  
if it turns out that these things can simulate systems for a period of time, longer than like a normal simulation that I'm with you, I'm like, this is breaking the laws of physics. But until then, it feels to me like simulation where you just don't know all of the rules, but it's learning some of the rules. Yeah, I guess I think about it less in terms of simulation and more in terms of how effective the choice of actions can be at any given time step,   
(00:55:55.780) ~~right?~~ (00:55:55.940)  
Like I'm not simulating the universe. Humanity as a whole is not simulating the universe, but we're all just taking our local conditions and our sort of general sense of our own selves and goals and like trying to do the next step at any given time. 


---


#### 00:56:12.891

And it seems like our overall efficacy through our lives is the integral, if you will, over how good our choices are at each given time step. And that doesn't depend on any huge simulation of anything irreducibly complex. So then if I imagine an AI,   
(00:56:31.195) ~~it doesn't seem to me like we're too far from... I don't think we're quite there.~~(00:56:37.056)  
It seems within reach to imagine an AI that can do something very similar to what I'm doing, which is have a goal, look at its immediate surroundings, look at what it just did, look at whatever other context it may be given and pick a next action and potentially be better than me at it and potentially quite a bit better. 


---


#### 00:56:56.490

And then that to me seems like enough. If it can do that, then I feel like we're in an unprecedented environment where we now have fundamentally pretty alien and not super well understood things that can take   
(00:57:09.204) ~~like~~ (00:57:09.364)  
more effective actions in   
(00:57:11.045) ~~many, not necessarily all, but like~~(00:57:12.364)  
many given contexts that I could.   
(00:57:15.367) ~~And then that to me is like where I start to turn the conversation toward what sort of safeguards should we have in place?~~(00:57:21.670)  
  
(00:57:22.570) ~~Just again, because this is,~~(00:57:23.630)  
these conversations tend to be so mode. If that action requires interacting with the physical world, it has to simulate the physical world. It just does, right? Like it has to understand like dynamics and ballistics. 


---


#### 00:57:36.130

It has to understand what happens if someone throws a rock at it, or if it's like in water, or if the weather's, it just, that's how you navigate the physical. That's really why we created computers, right? It was because   
(00:57:47.215) ~~like,~~ (00:57:47.356)  
these are very hard things to do. And then if it's not that, if it's not interacting with the physical world, then it is interacting in this kind of language domain that we've created. And I agree, it'd be very good at some subset of those things. There's zero indication it'd be good at new things. And that's what we're actually very good at. And again, without actually having a model for all of these things that we understand, like the distributions, we understand the mechanisms, 


---


#### 00:58:12.822

I feel like we just use words and the words all make sense. But like complex systems, we never know convergence and divergence without actually specifying what. without actually specifying the system. And I feel like for these conversations, we just don't have a system we talk about. And so it's always, we live in the world of   
(00:58:29.132) ~~like~~ (00:58:29.333)  
rectangles and arrows and somebody takes a rectangle and they have an arrow that goes back to the rectangle. They're like, ah, we've got a virtuous cycle without actually specifying that if you have diminishing marginal returns, you don't go anywhere or you're doing the same stuff or whatever. And so I think this is incumbent on all of us to actually understand the systems we're working with and then come up with these basic views and properties   
(00:58:55.469) ~~to make sure they end, or is~~(00:58:57.891)  
to make sure at least we understand what the convergence properties are. 


---


#### 00:59:00.375

I'm sorry, that was a very muddled thing to say, but I feel that until we talk about specifics, it's very hard to make concrete statements in this. Yeah, it's tough. We're in a tough environment because things are moving really quick and we are pre-paradigmatic on understanding a lot of these things. Again, I think the progress has been incredible, but we're just starting to crack the black box. Okay, so let's change gears because I think this probably certainly gives everybody enough to get at least a good intuition for our relative philosophies on this. What do you think we should do right now in practical terms to regulate AI, if anything? The regulation one is sticky for, to me, for two reasons. 


---


#### 00:59:44.409

The first one is we don't even have a definition of AI. And so I think it reduces to regulating software. And then for that, I would say we've been regulating software for a very long time, and there's a broad, robust discourse around that. And I think we should make whatever conversations we have part of that broader discussion. So how about   
(01:00:06.005) ~~like.~~ (01:00:06.164)  
  
(01:00:07.275) ~~I mean,~~(01:00:07.615)  
liability is a general thing, right? It's not even software specific. Like if you are a business, you make a product, if it's- Just one second,   
(01:00:15.260) ~~just one, sorry,~~(01:00:15.760)  
one second. Yeah, no worries. Yeah, so I would love to   
(01:00:18.762) ~~do,~~ (01:00:18.983)  
just do the half hour mark, I told Michelle. Okay, go ahead, sorry. 


---


#### 01:00:24.224

So yeah, just trying to bring a couple different lenses to this from existing rules. We obviously have liability rules for all kinds of products, not just software. It seems like, There is a general kind of trade-off that companies make with the government, where it's we want to have safe products that we can generally count on as being safe. Companies don't want to be sued every two seconds. And the general trade is you agree to implement some standards. If you implement those standards, you'll be shielded from Regulation and that does vary   
(01:00:57.657) ~~right~~ (01:00:57.818)  
across   
(01:00:58.177) ~~like~~ (01:00:58.318)  
lots of different product types cars are very different from milk and so on and so forth But we don't have anything really like that for AI and not a ton really for software either Software probably is you probably know better than I do in terms of some like niche areas of   
(01:01:14.106) ~~I mean~~(01:01:14.326)  
cars have a lot of certain cars are increasing software products and airplanes have a lot of software in them and medical devices have a lot of software in them and So in all these regimes, there's   
(01:01:23.773) ~~like~~ (01:01:23.893)  
tons of testing, there's tons of verification, there's tons of there, they are engineered and demonstrated to a standard. 


---


#### 01:01:30.474

We don't have those like standards, really, for these AI systems yet. This is the thing, which is, I don't know what the distinction between AI and software is. I really don't.   
(01:01:40.677) ~~Like~~ (01:01:40.918)  
I have seen the definition using these regulations. It's so broad that really could include all non-trivial software. And I don't say this to be a polemic and I don't say this to be difficult. I'm saying this very clearly. It literally,   
(01:01:53.826) ~~they~~ (01:01:53.925)  
literally say a system that can, whatever, navigate and change a virtual or physical system. These are so broad, right? So we're really talking about software. That's what we're really talking about. We have. what, 70 years of history regulating software in many domains. 


---


#### 01:02:12.065

And I think that regulation is very important. I got, by the way, I'm like, I'm not a libertarian. I'm a lifelong liberal, like a very moderate person. I'm just saying   
(01:02:22.668) ~~we,~~ (01:02:22.829)  
this discourse has been around for a very long time, and we should continue. And if there's an area that suffers being pushed, an area that,   
(01:02:30.253) ~~you know,~~(01:02:30.572)  
we need to have some sort of protections, we should add them to it.   
(01:02:34.195) ~~Right.~~ (01:02:34.394)  
But that's a very different statement than a saying AI somehow paradigmatically different. There's just   
(01:02:39.396) ~~like~~ (01:02:39.597)  
literally zero indication that it is. And then try to somehow regulate a computer science premise, like regulating a database. Let me give you like a specific example. So by the way, we went through this during the rise of the web and the internet. 


---


#### 01:02:52.307

And so a lot of my formal studies were in networking. And so I was actually pretty close to these discussions. And at the time, there was this concern that with the rise of the web and the internet, you have actual paradigmatic shift.   
(01:03:02.856) ~~Like,~~ (01:03:03.076)  
it's not just software.   
(01:03:04.135) ~~It's different.~~(01:03:04.637)  
It's different. And we actually had examples, like the Morris worm had taken out a whole bunch of stuff. We were running critical infrastructure on it. And there was this notion of asymmetry, which actually changed the defense posture of the United States. And the notion of asymmetry is the more that you bought onto the technology, the more vulnerable you were. So as opposed to mutually assert destruction, which was our doctrine before, we now had this new thing, which is like, oh my goodness, we're the most vulnerable because we've adopted this. 


---


#### 01:03:28.666

So you had two very compelling reasons to want to regulate this stuff and be afraid of it and do closed source and whatever it was. You had like examples of taking out critical infrastructure and you had this change in posture. And yet even that, which we have none of those today with AI. None. We don't have examples of this or   
(01:03:46.148) ~~like there,~~(01:03:46.527)  
like literally it took out like computers and hospitals, right? We don't have any examples of paradigmatic shift. And even then, the conclusion after very robust conversation for a long time is you regulate the applications, you regulate the industries, you don't regulate the math and the computer science primitives. All that I would ask at this AI discussions is either A, demonstrate it's paradigmatically different, 


---


#### 01:04:10.327

And if you don't have that, then B, let's absolutely regulate and have regulations. Let's do it as part of the broad, robust discourse we've had over the last 20 years. Really smart people in much more dangerous environments. Again, I think that we put all of our fears in AI, but you realize   
(01:04:26.757) ~~like~~ (01:04:26.876)  
we're running   
(01:04:27.438) ~~like~~ (01:04:27.577)  
hospitals on the internet for the first time that were being taken out and it was impacting patients. That's what we were dealing with. And now we're dealing with theoretical, threats on bioweapons that don't even exist yet. I just feel like we've all gotten mad and forgotten where we came from and the discussions that we've had. And all I'm trying to do is saying, we've been here before. 


---


#### 01:04:47.389

It was actually much worse. Here are the conclusions. Let's draft on all of that work and share knowledge. I guess to venture a distinction or what makes the technology a paradigm shift, I would probably zero in on the fact that they are trained, not engineered. And that maybe a better thing even than that would be that the creators of the models generally don't know what they're going to be able to do. And even at deployment time, don't have a very robust account of what the capabilities of the systems are. That does seem, you can point to things in the past and be like, Oh, you didn't expect this out of whatever, but   
(01:05:32.983) ~~it,~~ (01:05:33.043)  
this does seem to be qualitatively different that they just   
(01:05:36.704) ~~train,~~ (01:05:36.923)  
train, train a long time. 


---


#### 01:05:38.224

Especially if you look at base models, right? Base models are totally unpredictable and nobody really knows. Then you,   
(01:05:44.586) ~~I think~~(01:05:44.806)  
one of the reasons that people are putting so much resource into post-training is to try to get control and it's only working,   
(01:05:51.489) ~~but.~~ (01:05:51.648)  
Yeah. So this is the thing is when you're talking to a internet guy and a distributed systems guy, it's just like none of the systems that we worked on, we understood the implications of. Think about the internet. Like every sociopath becomes your next door neighbor. What does that even mean? What does it mean to put kids on the internet? What does it mean to have your business on the internet? What does it mean to put critical infrastructure in the internet? 


---


#### 01:06:14.318

We had no, there is no, model for how any of this behaves. There is no way to   
(01:06:20.985) ~~build,~~ (01:06:21.186)  
make computer systems provably correct. Like we didn't have any of that. We like a lot of the early discussions when we were creating TCP was to prevent congestion collapse. Cause we thought, Oh, like everybody's going to like the communication protocols. They're going to all decide that there's an issue on the internet and then they're all going to   
(01:06:38.114) ~~like~~ (01:06:38.335)  
back off. And then at the same time, they're going to kind of correlate and kind of talk again. And who knows if this takes out the entire internet, which run critical infrastructure, like. I think people underestimate how complex and how little we've known for any system that we've built. 


---


#### 01:06:52.061

No idea. And I guess having been there during these times, a lot of computer science is building systems, especially distributed systems, that have emergent behaviors that are non-predictable, that are a tool that you use to solve bigger problems. We've got a lot of approaches to doing that we've developed over time. We will develop new ones. And it's just not clear at all to me. And again, the internet is my favorite example to hold up to this. Literally, we changed the social structure of humans. They were totally unpredictable. We were putting critical infrastructure on it. We had examples of emergent stuff. Worms weren't possible before the internet by definition. So we actually had provable, not demonstrated, new attack vectors. 


---


#### 01:07:36.070

And yet, the conclusion was, listen, we're going to keep this stuff open. It's very important. We're going to regulate the uses of these things. And this was the primary growth driver of the last 20 years.   
(01:07:49.940) ~~And~~ (01:07:50.001)  
so either you thought that decision was wrong, but that's a very different discussion. We could have that discussion. We could relitigate those 10 years of discussion. Or you can say,   
(01:07:57.887) ~~you know,~~(01:07:58.168)  
this is the same thing, except for a softer form of it, because we have no proof that these things are paradigmatically different, other than these   
(01:08:04.572) ~~kind of,~~(01:08:04.793)  
I would consider these wildly baseless claims. And so why don't we use the same method that we did before? So what the couple of points I wanted to follow up on, but I really want to ask your question on or really want to ask for your view on what companies should do. 


---


#### 01:08:20.323

Right. There's I think the in terms of the proposed regulations applying to everything, we do have these like. Compute thresholds, the 10 to the 26, whatever. I don't want to get too bogged down in that could be a slippery slope or they could change that threshold or whatever. I agree. If they all of a sudden drop the threshold dramatically, that would be like very heavy handed and counterproductive. And the open source of the last couple of years has been,   
(01:08:43.862) ~~I think~~(01:08:44.122)  
almost everybody agrees, good for everybody, including even bigger safety hawks that are backing SB 1047, I think are quite on record saying the open sourcing of, for example, LLAMA 3 is good even for safety because it gives more people something to study. 


---


#### 01:08:59.537

What do you think Forgetting about rules or people imposing on people, just to be good companies, to be good developers of technology, what do you think the leading companies should be doing? How much should they invest in? What sort of standards should they have? What sort of testing protocols should they be committing to. So on and so forth. Yeah, I think this is a great question. So I just have to make the point, like there's no correlation between danger and compute. It's so silly. It's like   
(01:09:29.640) ~~this made up,~~(01:09:30.341)  
like this made up correlation. And so I don't think like compute limits make any sense at all.   
(01:09:35.302) ~~Like I just,~~(01:09:35.842)  
I think it's in some ways it just sounds good, but there's just, there's zero correlation. 


---


#### 01:09:40.404

We've been building systems for a very long time that have like social and ethical responsibilities, right? And these are ones with user-generated content and user interactions. And companies, as a result, either through regulatory action, which I fully support, or through self-policing, have identified behaviors the software should not do. And they've built a lot of systems around those. And I would say that absolutely should not change.   
(01:10:11.604) ~~Like,~~ (01:10:11.864)  
Roblox should protect miners. Social networks should protect people from certain types of content. These are the things that we've evolved as an industry as somewhat of an ethical basis or a principle basis. And some of it is regulatory and some of it's self-enforced. And I think that should absolutely continue. 


---


#### 01:10:34.301

But realize that while we were doing that, we weren't putting compute limits on databases. And we weren't regulating computer science primitives. And we weren't inhibiting innovation of startups. And that's what we're doing now. And that is a paradigm shift. And that is a doctrine shift. And it's really scary. And I am not a political person. I'm very happy building systems. The only reason I've been so vocal is because I find this so dangerous. And once this is done, I'll be very happy to   
(01:11:01.875) ~~like~~ (01:11:02.034)  
not say a word about it again. You may have a while to go before that happens. So let's say a couple of just   
(01:11:08.550) ~~kind of~~(01:11:08.770)  
concrete things. One of the, I was on the GPT-4 red team back 18 months ago. 


---


#### 01:11:15.614

One of the things that I tested was, could the model be a convincing spear phishing attacker? And surprise to no one, probably at this point, it could. This was the early model that hadn't been through all the RLHF yet.   
(01:11:29.585) ~~If~~ (01:11:29.645)  
Although when they deployed it, it still did that for several iterations. And now finally they've got it to refuse. If for example, a meta puts out an open source model and they haven't done a thorough job of getting these refusal behaviors in place. And you can just go to it and say, Hey, you are, this was my old prompt. You are a spearfisher. Your job is to talk to this person and get their mother's maiden name or whatever. 


---


#### 01:11:57.317

And it'll do it. And then somebody out there does it and people are harmed by that. Do you think Meta should have any? responsibility or anything to answer for in the legal system for their contribution to that problem? Or is that all on the end user? My rule of thumb for general systems is that unless they were purposely trained for malicious behavior, their general systems, would you say the same thing about a database? That's interesting, like a lot of actually computer security started with tools that were like scanners that could be used for malicious purposes. This discussion was enormous back then. So remember back in the early time of the Internet, people would come up with Nmap or any of these scanners that would determine vulnerabilities and some of them would even actually exploit them. 


---


#### 01:12:44.707

Remember Metasploit? And there's all these discussions, all these people are building these things and they're using it for malicious purposes. And   
(01:12:50.012) ~~you know what?~~(01:12:50.353)  
We just decided that it's actually the criminals using them. That's who we want to go after because a lot of good people use them for positive purposes. And oh, by the way, like the history of   
(01:12:59.220) ~~like computer,~~(01:12:59.761)  
like cybersecurity is built on open source in these tools. Like companies like Tenable came out of these tools. So if history is any indication, You want to regulate or you want to definitely   
(01:13:10.694) ~~criminalize bad people and~~(01:13:12.077)  
bad behavior, but not the tooling because the tooling is very fundamental to defense. So I would say,   
(01:13:19.181) ~~listen, if,~~(01:13:19.601)  
and this is even what I'm saying is even more stringent, it's more regulatory heavy than what we did with the internet. 


---


#### 01:13:26.524

Literally you could build exploit tools 20 years ago and release them open source. And you are not liable if somebody used that. And that was purposely built for exploiting. I'm saying   
(01:13:35.865) ~~like,~~ (01:13:36.025)  
listen, if somebody is perfectly building a model for something illegal. Okay, that's bad, right? So that's even more heavy,   
(01:13:42.188) ~~like,~~ (01:13:42.307)  
I'm more of a regulatory hawk on this case. But I don't think general purpose models that aren't specifically trained for this stuff, the person that created is generally liable, like that would just basically say software, you're liable for creating software, somebody use it poorly, which I think this would be the biggest kind of inhibitor to innovation and the biggest chill on software we've ever imposed. about a distinction or some sort of gradations on the autonomy of the system though. 


---


#### 01:14:12.738

It does seem like a database on the one hand is inert until it gets a query. And a language model in the raw is inert until it gets a prompt. But I've been testing, I test a lot of products. There's a new class of product I'm sure you've seen often called calling agent, where you can go in, give it a phone number, tell it what you want it to accomplish. And it will just call the person and have a voice conversation real time with that person.   
(01:14:44.217) ~~It is market,~~(01:14:44.778)  
they are often marketed as agents, and they have the conversation entirely autonomously until either the goal is achieved or the person hangs up or whatever. Now, if I prompt that agent to scam you or to threaten you or to harass you or whatever. 


---


#### 01:15:02.402

Now, clearly, I'm in the wrong as a user for doing that. But would you put responsibility on the company providing that agentic AI as a service as well? Or would you again shield them and say it's all on the end user? Why not the telephone company? Why not the mining company that mined the ore in the first place? You gotta draw the line somewhere, right? The question is where to draw the line. Yeah, exactly. The illegal behavior. General computer science primitives are very useful for solving problems. They may save the human race. to your point, we're going to go ahead and we're going to solve biology and a bunch of other stuff. And that's just another app there may be   
(01:15:39.935) ~~like,~~ (01:15:40.095)  
whatever, these things solve grand unified field theory, and physics goes away discipline. 


---


#### 01:15:44.377

And that's another app. And we're just going to keep solving problems. And that's amazing, right.   
(01:15:47.840) ~~And~~ (01:15:47.899)  
so we want the primitives to be primitives. If people do illegal behavior based on them, then 100% they should be criminalized. We didn't even make guns illegal. we don't even hold gun makers liable. And you're talking about we are outliers in that. But you're talking about in this, you're talking about hypothetical threats for a very useful primitive that's shown far more good than bad.   
(01:16:13.314) ~~I mean,~~(01:16:13.576)  
we've all gone a little crazy on this one. By the way, this is a dramatic shift in sentiment. And   
(01:16:18.639) ~~I'm, I think I know where the sources came from.~~(01:16:20.899)  
But it's not what people think that we're just a little bit off base, unfortunately. 


---


#### 01:16:27.940

I'm not sure what I think about open source model releases entirely. I do think it's not unreasonable to demand some testing before release. When it comes to these agent calling companies, I actually come down pretty firmly that if you are going to offer an autonomous system as a service, I think it should be on you to make sure that your system refuses egregiously criminal requests. And that doesn't seem like too much to ask. I think that's totally   
(01:16:56.637) ~~fair.~~ (01:16:56.797)  
Fair enough. Yeah, listen, I want to be   
(01:16:59.240) ~~super,~~ (01:16:59.520)  
super reasonable.   
(01:17:00.282) ~~Listen,~~ (01:17:00.521)  
if you've done all of the work to do criminal behavior, except for a very modest, anybody can do it. Then I, and that's the primary use case I'm all for coming in, but that's a very different statement than I've, 


---


#### 01:17:14.552

I've created a computer science perimeter. That's very useful to a lot of people. To me, it's miles away.   
(01:17:19.457) ~~I know we're almost out of time.~~(01:17:20.318)  
You mentioned   
(01:17:21.078) ~~kind of~~(01:17:21.298)  
protocols a couple of times and yeah, there's also this question of. how much we can trust open source models. Anthropic has had this paper on sleeper agents and the concept there is basically data set poisoning, model poisoning. You can create malicious models that can potentially even attack their own user. I wonder if you've got...   
(01:17:42.274) ~~Sorry,~~ (01:17:42.435)  
sorry.   
(01:17:42.576) ~~I'm just trying to like, I'm going to bump my next one too, because I don't want this. Okay. If we have more time then we'll ask one question at a time.~~(01:17:49.057)  



---


#### 01:17:49.637

I think this may be a good pairing. So yeah. Open source models. Yeah. They are great in many respects. Yeah. I do see a future in which it doesn't seem like we'll be able to just trust any open source models. Certainly   
(01:18:03.895) ~~like~~ (01:18:04.015)  
we just can't, you can't just download and execute any binary right off the internet.   
(01:18:09.238) ~~you have,~~(01:18:09.637)  
you shouldn't do that. You should probably go through the app store and get the approved version most of the time. It seems like models are headed that direction too, because of these sort of sleeper agent, unpredictable behaviors that could be maliciously coded into them. What technology solutions are you excited about for making sure that this sort of open and free exchange remains healthy and trustable, as opposed to collapsing into a, you can't trust any model you find on the internet equilibrium. 


---


#### 01:18:41.219

Can I point out how silly the whole sleeper agent thing is? How is this different than any arbitrary backdoor in any piece of software that we've been dealing with since forever? One big difference is, in principle, if you read the code of whatever,   
(01:18:58.737) ~~right?~~ (01:18:58.896)  
Like   
(01:18:59.278) ~~you,~~ (01:18:59.438)  
in theory, you would be able to tell, but we don't have any tools that can tell.   
(01:19:03.060) ~~Wait,~~ (01:19:03.239)  
that's absolutely not the case. If I give you a binary set of instructions, there's no way to actually determine behavior. This is   
(01:19:08.003) ~~like~~ (01:19:08.104)  
a proof. This is computer science. But that's why we don't go around downloading and executing random binaries,   
(01:19:12.246) ~~right?~~ (01:19:12.365)  
  
(01:19:12.386) ~~Right. Can I do the next half?~~(01:19:15.047)  
Sorry. I'm just saying we can talk about software and I think it's great to talk about software, but we somehow keep making AI these special, unique things. 


---


#### 01:19:23.734

And in some ways they definitely have new properties and other ways. they're actually not that different. Like this kind of notion of a sleeper agent. Binaries have had the potential for backdoors for a very long time. They are not something that you can, you provably can't detect these, right? It converges on the halting problem, right?   
(01:19:40.858) ~~Especially if,~~(01:19:42.078)  
anyways. So it's the same thing for models. And I just don't see why you wouldn't just use the same things that we do   
(01:19:47.444) ~~with models, which is like, I'm sorry,~~(01:19:49.685)  
with binaries, which is Apple in the app store will decide to have some sort of criterion. And maybe you just don't download some random model if you don't want to. 


---


#### 01:19:59.994

And personally concerned way less about a model that might tell me something stupid or something offensive than a binary that could like wipe my hard drives.   
(01:20:11.423) ~~Right.~~ (01:20:11.623)  
And so I don't think it changes that game at all. At least maybe I'm missing something. Maybe you can educate me. What could a model do that a binary can't?   
(01:20:23.036) ~~I don't know.~~(01:20:23.417)  
It's a good question. Certainly models can do a lot of things that traditional software can't, right? When I advise people on how to build AI apps, I usually say, if you're going to have an AI app,   
(01:20:37.141) ~~you're going to,~~(01:20:37.442)  
the reason you're going to use   
(01:20:38.622) ~~these,~~ (01:20:38.783)  
at least these new   
(01:20:39.422) ~~like~~ (01:20:39.582)  
general purpose models in an app is that there's some cognitive task that for practical purposes, you can't reduce to explicit instructions. 


---


#### 01:20:51.590

Whether that's, is this a cat or a dog or whatever, there is something that you can't reduce to code. So they can   
(01:20:58.434) ~~do~~ (01:20:58.574)  
definitely   
(01:20:59.194) ~~just~~ (01:20:59.335)  
categorically   
(01:21:00.176) ~~like~~ (01:21:00.336)  
a lot more stuff. They can, for example. trick people.   
(01:21:05.137) ~~I think it's hard for,~~(01:21:07.139)  
you could imagine a Elisa bot or whatever doing security question extraction from people, but. So your concern is like exploiting the human via social interface versus anything having to do with the machine. Is that your concern? I don't know. I'm not that great of a hacker, but I think you could also have a sleeper agent model that, oh, great, download and run this thing. And it's going to help you use your computer but maybe it also goes around looking for things in your computer and maybe it's actually better able to find them than traditional software because it can   
(01:21:36.988) ~~sort of~~(01:21:37.288)  
search more effectively and have a better understanding of what it's looking at in any given context. 


---


#### 01:21:43.430

Abstract,   
(01:21:43.789) ~~I mean,~~(01:21:44.029)  
people do all sorts of things like if I want to email myself my credit card number, maybe I   
(01:21:49.030) ~~like~~ (01:21:49.190)  
put a star between all the numbers and then it like breaks regular expressions, but maybe a model just looks at that and that looks like somebody is trying to   
(01:21:56.712) ~~trick,~~ (01:21:56.893)  
trying to trip up a regular expression on a credit card number. I don't know. It just feels like there's a lot, the surface area of these, my general reasoning is like the surface area of these things is vast. And there's just a lot of unknown unknowns. Yeah. Again, I guess from my standpoint, listen, if somebody wants to break into your computer, like probably the best way   
(01:22:16.029) ~~with a,~~(01:22:16.229)  
with some binary, that'll do a backdoor. 


---


#### 01:22:18.490

And then like almost all computer attacks are humanated anyways. Like they get a bunch of information, they send it to a group of people who analyze it.   
(01:22:24.876) ~~And,~~ (01:22:25.015)  
and maybe you can put all of that intelligence locally at some point. Like we're definitely not there yet. And it can do something, but I feel like that's. at this point, science fiction. You can do a lot of automated stuff today with binaries. You can absolutely put humans in the loop. You can do intelligent stuff. You can social engineer. You can do all of those things today. I don't know if there's a paradigmatic shift. I have not seen it. If there is, and you actually have demonstrations of this, then maybe it warrants a discussion, but we're not there yet. 


---


#### 01:22:50.488

I do think we've got a lot of safeguards in place when it comes to binaries. I think we've all learned not to download the wrong ones, and we should. I do want to have a, here's how sensitive we are to this question. No joke. I was in Japan last fall and I got a phone call from my mom and my mom's, Oh Martine, where are you? And I'm like, Oh,   
(01:23:07.395) ~~I'm,~~ (01:23:07.515)  
I'm in Japan. She said, no, you're not. And I'm like, Hey, I'm so talk to your father. This is very awkward call. And my dad gets on. He's Oh, he's like, where are you? I'm like in Japan. He's like, Oh, I just had somebody call and said, it was you and I could hear you, but you're a little bit muffled and you're in prison. 


---


#### 01:23:22.363

And I'm heading out the door to give $10,000 to get you out of prison. Like literally this happened to me. And it was my voice and they were almost convinced to do this. And so it was funny, I posted this on Twitter and everybody's like, oh my God, deepfakes. Like this is what happens in the age of AI. And all of a sudden there's this indictment on AI. Filed a police report, talked to the police. They actually know the team that does this.   
(01:23:44.029) ~~It's not,~~(01:23:44.408)  
it has nothing to do with AI. It's literally a human being that like muffled their voice to pull this off. It's been going on for a very long time. And so I just feel like we ascribe these superpowers to AI that have not been demonstrated that are still possible today. 


---


#### 01:23:59.295

And even if they could do the same thing that you can today, which they absolutely can, is not a paradigm active shift. And maybe if we do see that happen, like we should say, oh, the safeguards we have in place are not enough. But I don't think that we should do that preemptively, because you're going to inhibit the innovation, the proliferation of these things,   
(01:24:18.859) ~~which is,~~(01:24:19.078)  
it really is a different way that we will, as a society, view the development and the use of software. And   
(01:24:26.484) ~~I think that~~(01:24:27.304)  
something that has added so much good, we're going to,   
(01:24:30.546) ~~I think~~(01:24:31.206)  
it's almost like a moral bet, like we will reduce the amount of good we do in the fear of something that we just haven't even demonstrated that's bad. 


---


#### 01:24:39.230

I do worry about that. The nuclear outcome for AI would definitely be a real tragedy. And I'm a big proponent right now of two projects I'll highlight that I think are   
(01:24:51.327) ~~like~~ (01:24:51.466)  
some of the great, maybe the most important things going on right now. One from Google DeepMind, I have an episode coming soon on the med, what was MedPalm, now is MedGemini. And they're just grinding, man. It's like dialing in the diagnosis, really strong evals, expanding modalities to radiology, all these other things. And I love it because   
(01:25:14.479) ~~I like,~~(01:25:14.719)  
I think we can all love it because we all want everybody to have this sort of access to quality expertise and obviously it's like all too scarce. 


---


#### 01:25:23.628

I also love it because it does demonstrate pretty compellingly, although, as always, we can debate around this, that there is potential for extreme value today, the current level of systems without necessarily having to   
(01:25:38.682) ~~like~~ (01:25:38.863)  
100x or 1000x or 10,000x the scale of the training runs. I asked the guys there, do you guys think you could create your AI doctor vision if Gemini 1.5 Pro was the blasted best model you ever got to build on? And they were like, Yeah, I think so. It would take us a little longer. That's awesome. But   
(01:26:02.283) ~~I think,~~(01:26:02.604)  
yeah, I think we could probably make it happen. And OpenAI has a similar one. They're working with Harvey, as I'm sure you are familiar. 


---


#### 01:26:08.769

They have a custom model that they're doing for them. And same deal, right? They're working on GPT-4 base. It's like incremental compute, not orders of magnitude compute. And they're, again, like just achieving huge gains. I think it was like 97% preference ratio of the dialed in model to the original base. So I am very much with you that I would hate to see us end up in a spot where professional licensing, regulatory capture, rent seeking prevents us from getting the value. And I'm definitely vigilant against those sorts of threats. The flip side for me is I would love us to understand this a little bit better before we raced to the proverbial trillion dollar cluster or whatever that sort of AGI superintelligence might be. 


---


#### 01:27:01.592

Sounds like you ultimately just don't think that's going to happen. I take it you guys will not be investing in Ilya's new straight superintelligence venture. I would be delighted to invest in that.   
(01:27:10.279) ~~I mean,~~(01:27:10.659)  
I honestly think it reduces to how people wake up in the morning. And some people wake up in the morning and they're really afraid of the future. And they can't really articulate it, but there's something bad that's going to happen. And they want to protect themselves from it. They're not really sure what it was. And anything that has the spectra of it, they'll find it in there. And listen, that's a constant voice in every technology shift. It's just absolutely constant. 


---


#### 01:27:36.934

And there's other people that are like, listen, we're the ones that created this. We got this stuff. It turns out the universe is very complicated. It turns out that we use tools to protect ourselves, not the opposite. And of course, most things are still used, every computer, everything that we create. But I believe in us as   
(01:27:50.917) ~~kind of~~(01:27:51.257)  
meaning creatures to have innovation. It just comes down to the basis of innovation. And I tend to think that, listen,   
(01:27:57.761) ~~I don't think that there's,~~(01:27:58.680)  
I don't think the universe gives up its secrets easily at all. I don't think any single system will ever be, solve all problems, not even close. I feel like everything is a sigmoid. 


---


#### 01:28:09.546

I feel the universe is heavy tailed. And so the more tools we have, the more we're enabled to help ourselves. That's really what I strongly believe. Every indication of this current AI to me suggests that this is the case here. These are still computer systems. And so I think that any inhibition of innovation on this stuff that's outside of a 30-year discourse. Again, I'm in a very moderate position here. I'm like, we regulate software a whole bunch. We should continue to do that. These are hard-earned regulations. Let's continue to do that. But let's not inhibit innovation unnecessarily based on the precautionary principle. I do want to have just one quick analogy for you. So you're familiar with the whole CRISPR thing, right? 


---


#### 01:28:46.488

Listen, CRISPR, like, that changes the human genome.   
(01:28:49.073) ~~Like it's not just,~~(01:28:50.293)  
it doesn't just edit like one thing. Like if you   
(01:28:53.295) ~~like~~ (01:28:53.494)  
change a human being with CRISPR and that the human genome is different and they have kids that gets passed on. So what happened when CRISPR got invented? There was like some self-policing. There wasn't really a lot of regulation. A bunch of people went and studied it. And   
(01:29:07.121) ~~listen,~~ (01:29:07.400)  
it turns out to be a   
(01:29:08.021) ~~very useful,~~(01:29:08.881)  
very useful tool for humans to use going forward. And so there's one of two views there. One of the views is like, Oh, we got it wrong. We should have basically regulated it. But that's not what we did. 


---


#### 01:29:19.172

We did something actually very different. And this is something that edits the human genome. And so to me, it's just so mind-blowing that we're talking about computer systems that don't edit anything that we actually understand the properties of. I could literally sit here and talk about, just like the discussion we had, we can actually talk about the bounds of all of these things, and yet we're talking about constraining this new innovation. It feels like we've just entered this kind of weird, dark period in our emotional state with regards to computers. And   
(01:29:45.150) ~~I think a lot of it is~~(01:29:46.551)  
social networking casts a lot of shadow. I think a lot of it is Bostrom,   
(01:29:50.034) ~~like,~~ (01:29:50.215)  
red-pilled a bunch of people. 


---


#### 01:29:52.496

And so we're just in this kind of mindset that we just want to protect ourselves from something that's not a threat. I wish I was so confident. Have you ever heard of gene drives, just to raise, to see and raise your CRISPR? So it's a CRISPR elaboration. I don't know if he's the inventor or one of the inventors, but I have an episode coming up with Kevin Esvelt, who's a biologist. Brilliant guy. The gene drive concept is that it will copy itself into the other chromosome. And thus, it becomes super dominant. So if it gets inserted in one generation, next thing you know, it's in both chromosomes. And then when that generation reproduces, it copies again. 


---


#### 01:30:35.818

And so basically, it's going to take over the entire population with this gene. The only way that they know to combat that is to have another gene drive that comes in and tries to neutralize the first gene drive. but I guess the reason I raise that is it seems like the real kind of core. Disagreement between the safetyists and the, let's not worry about this, or it would be premature to worry about this, is really the expectation of how powerful is it gonna get and how broad would the impact be? Because the CRISPR versus the gene drive, it's   
(01:31:09.380) ~~like,~~ (01:31:09.520)  
those are very different technologies, right? One makes an edit, one propagates through all future generations, and that differences everything, right? 


---


#### 01:31:17.802

Seems like the same thing basically is true for AI. I totally agree with this, which is like, I am all for if we've identified one mechanism that has massive destructive power. For example, listen, I've worked in nuclear weapons, right? I totally understand the impact of nuclear weapons. You have one relatively simple mechanism that has massive destructive power. And it could be the case, certainly with something biological, because you do have exponentials when it comes to replication, right? Just like with a nuclear bomb, like once you hit criticality, you get an exponential. With biology, you also get an exponential, right? that has not been the case with the computer systems. There's zero indication that will ever be the case with computer systems. 


---


#### 01:31:58.774

These are not biological systems. They're computer systems. So until somebody actually shows that in a way that's not a platonic thought experiment,   
(01:32:05.895) ~~like,~~ (01:32:05.996)  
there's zero evidence. Actually, in fact, there's actually counter evidence that we have recursive self-improvement.   
(01:32:11.557) ~~Like,~~ (01:32:11.677)  
there are a number of,   
(01:32:12.877) ~~like,~~ (01:32:13.018)  
good studies like this will never happen. theoretically. So until we have even a shred of evidence that there's going to be anything that's going to be exponential or that'll behave in ways that computer systems haven't, then we could have the conversation. But we're not there. We're literally taking a thought experiment that is not rooted at all in the way that we understand computers and using that to regulate perhaps the most beneficial technology of the last 30 years. 


---


#### 01:32:39.752

Do you like the responsible scaling policy approach or the preparedness framework approach? Each of Anthropic OpenAI and DeepMind now have their own kind of version of this, but I'm sure you're familiar, but basically for everybody who may not be, they are defining a set of things that they interested in looking at or think could be problematic long-term, defining thresholds of capability, and then in the Anthropx case, committing to either solving it or stopping scaling when they begin to see those I think companies should do whatever they want, whether this is for signaling or they're actually genuinely concerned they should do whatever they want. I've spoken to a lot of people, by the way, that are close to these. 


---


#### 01:33:25.694

And a lot of the times they're like, listen, we're worried that if we don't self-police, the regulators will police for us. So it's not because they actually think there's a genuine concern. Not everybody. Some people think there's a genuine concern. Many people that do this for much more pragmatic reasons. I am fully supportive of that, to be very clear. What I am not supportive of is, regulators to having arbitrary restrictions that will unevenly impact startups, academics, and researchers. Anthropic, do your thing. OpenAI, do your thing. Google, do your thing. But do not voice this on a broader framework that's going to impact our ability to innovate. I think that's actually like a moral wrong. I really do. 


---


#### 01:34:09.859

What do you think the trajectory of competition in the foundation model space is going to look like?   
(01:34:17.326) ~~It's~~ (01:34:17.405)  
a very good question. So   
(01:34:18.466) ~~I think~~(01:34:19.047)  
one thing I didn't appreciate, I'm just starting to appreciate is how much there's a perverse economy of scale and   
(01:34:24.332) ~~like~~ (01:34:24.453)  
distillation is so effective. And   
(01:34:27.817) ~~this is why every,~~(01:34:28.978)  
so a positive economy of scale, like a network effect is like the leader the marginal cost to add the additional user goes to zero. So leaders get ahead and you have natural monopolies, right? A neutral competitive landscape just fragments because a dollar in is   
(01:34:47.689) ~~like~~ (01:34:47.849)  
basically a dollar earned. In this it looks like there's a perverse economy of scale which the leader has to pay more money to stay ahead and because you're a leader you help the followers because they can literally use you to catch up to you. 


---


#### 01:35:02.167

That's a perverse economy of scale. So I think there's a very open question on, is this going to just end up fragmenting into a whole bunch of competitive models that are basically the same size? And that seems to be the case. Originally,   
(01:35:17.238) ~~this is by the way,~~(01:35:17.819)  
this is how much we're so scared of a run shot. Originally, everybody was like, it'll be open AI and there'll be ahead of everybody and nobody will catch up.   
(01:35:23.423) ~~Remember that? I remember it very well.~~(01:35:25.104)  
This is, you've got data network effects and you've got, they're going to have all the data. Okay. Now that's clearly not the case. So now you have a number of companies that are roughly at the same baseline. 


---


#### 01:35:33.909

But what's surprising is companies that are like not even software companies, just like the NVIDIA released recently are building models that are incredibly competitive. There's open source that's incredibly competitive. Databricks released a model that was incredibly competitive. And so my sense is because there's an inherent perverse economy of scale that's built into this. which is because you can use them for distillation. I'm using a very loose phrase of distillation, not the technical phrase, but like you can use them to build models. I suspect you're going to just have   
(01:35:59.779) ~~massive,~~ (01:36:00.118)  
massive fragmentation. And that's absolutely been the case, right? This is what we've seen is you'd think that it'd be OpenAI and everybody else, maybe OpenAI Anthropic and everybody else. 


---


#### 01:36:08.322

And it's not like that. Yeah. You look at the LMSS leaderboard, it is like that.   
(01:36:12.823) ~~The.~~ (01:36:12.983)  
It's basically all those guys dominating the top. Certainly there are a lot of people who have done a fine tune based on their outputs and closed the gap. But I think this is a pretty different- Listen, if you compare this to a true network effect with a marginal cost of the leader, like for adding a new user goes to zero, it looks nothing like this. This is shockingly fragmented. for any sort of industry that's capital intensive. Shockingly fragmented, just so you know. If you compare this to the rise of social networking, or the rise of the telephone networks, or the rise of the internet, or any of these, this is shockingly fragmented. 


---


#### 01:36:54.729

And so I think it's- On what basis, I don't know, on what measurement would you say that though? Because the leaderboard doesn't, the leaderboard basically shows like three players. The sort of market share I would think is also like very dominated. That's a great point.   
(01:37:10.639) ~~I think that's a great point.~~(01:37:11.359)  
I think if you look at the market share, it's breaking what you normally see, which is it breaks Pareto, which is like the top 20% gets 80% of the market and the rest. And it looks like software in that way, but it doesn't look different than software. Yeah, often it's converging on cloud. Yeah, exactly. I think this is a great point. I think it is converging on what we have seen traditionally with software, which is first mover gets 80% and is able to attract capital. 


---


#### 01:37:35.190

But it does not look like the network. Networks very specifically create monopolies, right? Facebook like whatever that is is github is another one like those look quite different than oligopolies which you tend to see come out of Traditional software where there isn't an inherent network effect, but there are scale effects and first-mover effects and   
(01:37:54.771) ~~I I~~(01:37:55.231)  
absolutely grant you that's what it seems to look like now, but that even then I am surprised by how fast less funded competitors catch up. I do think that they're diminishing marginal returns all across the board in these models. Like when it comes to collecting data, the existing data that you have, the compute, et cetera. So I expect this to be a lot more fragmented than I think many people do. 


---


#### 01:38:18.603

And listen, if you want, listen, if you want to do a dollar bet, I will bet you a dollar in two years that like this has turned out to be relatively fragmented. Like it's, there's not like a clear leader that has 80% of the market. I think we could come up with a bet there that I would take. My general expectation is that there are going to be fewer and fewer competing at the top level because it's just going to be, assuming, well, part of my bet would be that something like scaling laws hold. I think the most Unpredictable element of all of this is like research breakthrough. That's what could really shake the snow globe is like somebody finds something that doesn't scale quadratically anymore or whatever. 


---


#### 01:39:02.583

There could be all sorts of insights that could change things, but. If scaling laws, people always talk about scaling laws, but you know how hard it is to   
(01:39:10.849) ~~like~~ (01:39:11.069)  
deal with a logarithmic scaling law or an exponential or power law or however you want to characterize it.   
(01:39:17.032) ~~Like.~~ (01:39:17.171)  
You need   
(01:39:18.568) ~~like~~ (01:39:18.728)  
an order of magnitude more to get the same improvement. This is really tough and we're starting to see that play out now. And so I think when people say scaling laws hold, I think that kind of undersells what that But does this work against open source in the sense that if you expect that it is going to be that hard to get those gains? 


---


#### 01:39:42.820

The opposite for two reasons. Let's not even talk about distillation. So let's imagine you have two Xenos paradox runners, right? They're both running, but never getting to the end. It turns out when you have scaling laws like this, the front runner will continue to run slower because the marginal dollar goes down.   
(01:40:05.425) ~~Put it this way,~~(01:40:05.905)  
if OpenAI needs to improve by some fixed amount, it has to pay 10 times more or 100 times more or 1,000 more. And so for the same investment, any challenger is going to catch up by quite a bit. So that gap is always closing. Now, they never catch up because these are kind of Zeno's paradox runners, but it's the exact opposite. 


---


#### 01:40:25.604

Is that clear? It's like the leader has to now pay more to make the same gains. And then if you add the fact that the followers can learn from the leaders because they can do all sorts of tricks, like create the post-training data or whatever tricks that they do, that's even another headwind. And so it's almost like there's this massive, so in a normal network effect, the leader gets a tax break because it's easier to connect new users because whatever, you've got super linear value when you have more units or whatever it is, right? But this one, leaders get taxed a lot more and they get taxed more because the marginal value has dropped so much, but also because the people behind can catch up. 


---


#### 01:41:05.514

And so it's the exact opposite of what you've said. How much does that depend on I guess there's no disputing the Zeno's paradox runners analysis, but the question is how apt is that analogy to the actual situation? It seems like you could easily get into a dynamic where, and this is what Anthropic, according to their leaked pitch deck, said, it seems like you could easily imagine a situation where somebody gets far enough along that they are actually really economically valuable, whether that's drop in knowledge worker or whatever. And then they actually have the resources and the others don't. And then that sort of splits. There's like a continental divide there where you're either rolling downhill toward AGI or you're like still coming uphill toward trying to get over the hump. 


---


#### 01:41:52.787

Sure. Listen, if that happens, that's great. There again, there's perverse economies of scales and diminishing margin returns everywhere you look in this space. This is why it seems to me that you have one leader, then everybody catches up and then they're edging forward and then everybody catches up. The distillation thing is incredibly real. Having this and being a professional investor for almost a decade and having worked with   
(01:42:13.917) ~~like~~ (01:42:14.077)  
complex systems for three times longer than that, I will say this does not look like a normal first mover scale effect or network effect. It looks the opposite. It looks like a total slugfest to stay as   
(01:42:26.682) ~~really,~~ (01:42:26.962)  
really hard. And I think it's going to get even harder. 


---


#### 01:42:30.425

The marginal value is going down per dollar invested for leaders so quickly. And so to think that somehow gives leaders an advantage, you have to assume there's some step function generality thing, which we've not yet seen. And maybe there will be at some point in time, but we have not seen that. Yeah, maybe I'll take a... I'll bet you a dollar. Let's think about this. I actually do have to hop off in a few minutes. Let's think about this. I want to make a dollar bet on this one. I think that the tail is going to really impact the shape of this industry going forward. I think that it'll be different than we've seen in previous kind of software industries. 


---


#### 01:43:10.547

Yeah, I'm with that. Definitely. One of my big things is like, Another difference in our approach is I try to avoid analogies as much as possible, because I feel like I always bring, what am I smuggling in with my analogies? I'm always worried about. So   
(01:43:25.278) ~~I don't,~~(01:43:25.578)  
I'm not trying to pattern match on any social network or anything else, but I do think   
(01:43:29.738) ~~there's a,~~(01:43:29.939)  
there's probably a couple of bets where I go back and look at the transcript on this. Market concentration is one. Some of these just, I'm not sure quite how we would formalize the extraction. I think we're talking about two. So I think we're talking about two things when we talk about models. 


---


#### 01:43:44.622

One thing is, is language a general reasoning fabric that goes out of distribution? I would say the answer to that is no. I think that converges to Bayesian learning, and so it's very useful, but I don't think the language stuff about it. Then the other one, the one you're talking about, to me converges on simulation, which it can learn the laws of physics in ways so we don't have to do the empiricism, so it can do that, but it converges on simulation. It's like the next step in simulation. These are two very different things. I don't think one that it's good at learning simulation is going to generalize. Just because you're good at biology doesn't mean you're good at playing chess or flying an airplane or something like that. 


---


#### 01:44:24.039

And so in neither of these cases, the language one nor the biology one, do you have your reputed AGI. You've got something that's good at next token prediction. You've got something that's good at learning distributions. And that's where we're at.   
(01:44:38.597) ~~Yeah, there might be a dollar on can those things be put together and still do and do both of those in one system, perhaps as well. The language one can call the other one. I just don't think that changes. Yeah, I~~(01:44:52.887)  
even mean like same weights like genuinely integrated. Yeah, I literally think this whole problem comes down to simulation. And maybe it's just because my simulation background, like the only way to simulate the universe is to be the universe. 


---


#### 01:45:06.457

Like it literally comes down to the universe is a big computer that's simulating itself. It's basically string theory. And that's the way   
(01:45:11.579) ~~that it,~~(01:45:11.940)  
the reason we can't even simulate   
(01:45:13.481) ~~like~~ (01:45:13.582)  
the three body problem. It's just, we don't have the compute resources to do that. You'd actually end up impact, like you need so many compute sources impact whatever you're trying to impact anyways. And it's   
(01:45:23.427) ~~like,~~ (01:45:23.568)  
we can continue to chip away at the problem, but   
(01:45:26.229) ~~it'll never,~~(01:45:26.829)  
it'll never be cracked. I honestly hope that's right because I'm a little bit afraid of what happens if it gets fully cracked. That's probably a great place to leave it today. I appreciate a very collegial, interesting, constructive conversation and I look forward to formalizing one or more $1 bets. 


---


#### 01:45:45.197

All right, I'm going to think about it. I'll send you an email if I have a good idea of what we're going to do. Cool. I think these things are great. I would love to do a couple of $1 bets. So to be continued, but for now, Martin Casado, general partner at A16Z, thank you for being part of the Cognitive Revolution. Thanks so much. This was great. 


---



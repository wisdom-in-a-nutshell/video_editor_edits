#### 00:00:00.129

Logan Kilrick, now of Google. Welcome back to the Cognitive Revolution. Thank you. I appreciate it. Lots of cover. I was just out at Google I.O. at your invitation. Thank you for that. I think the race is officially on. That's safe to say. I want to   
(00:00:11.833) ~~just~~ (00:00:11.932)  
take you through a little bit of your experience with Google. Obviously, you've had one of the few people on planet Earth that has seen both of the 1A or 1A and 1B AI leaders from the inside. So just to get your perspective on that. And then I honestly just want to do a pretty down the fairway run through of all the stuff that was launched at IO, all the stuff that you're excited about, help developers get oriented toward the platform. 


---


#### 00:00:31.864

As you well know, there's some complexity issues there historically that I think you're working to help overcome. And then I hear there's some cool stuff, maybe more stuff coming soon too. So maybe we can preview that a little bit at the end, if we can time it just right. I love it. I'm super excited. Let's dive in. All right, cool. So first of all, you were not on the beach for long. It was a pretty short timeframe between your departure from OpenAI and taking up at Google. Is there an inside story of how that happened? I got the sense that this was not like a normal Google hiring process, which from what I've understood can often stretch on for months, but certainly didn't seem to be the case for you. 


---


#### 00:00:59.091

Yeah. When I left OpenAI, a bunch of folks from Google had reached out and I started having conversations with Matt Velloso, who's now my manager, and Josh Woodward, who leads the Google Labs team. gave a bunch of the awesome IO keynotes. And it's funny that you say process being quick. Honestly, for me, it felt slow. I was like, I'm ready to move. I'm burning daylight here. The race is happening. But ultimately, to Google's credit, and it's not clear to me that much of this is visible in the world, today, but   
(00:01:25.037) ~~I think~~(00:01:25.316)  
like the team is really making the order of magnitude of bets on everything that's happening in AI right now that you would want to see. 


---


#### 00:01:30.519

And I think hopefully that was clear from the releases at IO. And I felt that in my hiring process. I felt that level of urgency, just like in the way in conversations with people. It's exactly what I wanted to see. That's just who I am as a person is   
(00:01:42.042) ~~like,~~ (00:01:42.141)  
I would like to do things and I would like to do them as soon as they can be done. So it was exciting to see that from Google. Yeah, I've got a little minor story that supports that myself, actually. When Gemini 1.5 was initially announced and put into preview mode for early testers, I was not initially on that list, but I sent Jeff Dean a DM on Twitter on a Saturday morning, my time, 


---


#### 00:02:03.251

Eastern time, it was like 1130, I think I sent the message. And within an hour, he had responded to me, said that he would get it done, send an email, copied Josh Woodward actually, who then in turn copied someone else. And within 24 hours from a Saturday morning to a Sunday morning, I had the access and was testing the million tokens. So I definitely took away from that, that there is no level of seniority at Google at this point that people are not really locked in and willing to roll up their sleeves and make things happen. I'm under no delusions about my own level of importance. So to see that kind of responsiveness and just engagement from folks who've been there a long time, particularly in the case of Jeff Dean. 


---


#### 00:02:38.467

I actually don't know how long Josh has been there, but I know they're both senior folks and Jeff certainly could be excused for not responding to fan mail like that. But I was pretty impressed with his engagement and how quickly that was turned around. Yeah, Josh has been at Google for 15 years he actually started as an intern, and now leads the Google Apps team as the VP and is   
(00:02:55.409) ~~like~~ (00:02:55.569)  
an incredible journey but exactly what you would expect from somebody who's gone through that and   
(00:02:59.674) ~~I think~~(00:02:59.873)  
in many ways   
(00:03:00.694) ~~like~~ (00:03:00.814)  
his team again for folks who don't context his team is actually the team that built the Gemini API and AI studio and it's now Matt Delosso's team, who I'm a part of at Google, who's sort of inheriting these products as we scale it beyond a million developers. 


---


#### 00:03:11.805

So it's been hard to match Josh and his team's sense of urgency around this stuff, but it is also incredibly inspiring. Interested in what else has stood out to you about Google culture so far? One tweet that you put out in your first few weeks there that I thought was remarkable was a comment that it was something to the effect of, one thing that's nice about Google's culture is that there's a lot of visibility into what's coming, and that makes your job easier. Obviously there's some hint of implied contrast there, and   
(00:03:35.794) ~~I don't know if you would want to go beyond no comment on the contrast, but~~(00:03:40.358)  
  
(00:03:40.497) ~~maybe you~~(00:03:41.840)  
certainly can if you'd like. I think the freedom of speech perhaps has been restored for some who willingly gave it up at one point, but to whatever degree you want to go to that, you can go do it. 


---


#### 00:03:50.067

And if not, then just tell me like how the culture has landed for you as you've ramped up. I think at a really high level, the practical reality at OpenAI, and I think maybe you can get Sam on and he can give his perspective. And I think for very real reasons, the separation between research at OpenAI and everyone else at OpenAI is a very strong force. When I joined OpenAI, that wasn't the case. I think this is actually one of the pieces of the culture that a lot of folks appreciate, which is you can just drop into a research meeting and hear about what was happening and learn about   
(00:04:18.923) ~~what all of~~(00:04:19.303)  
the how the technology itself was progressing, 


---


#### 00:04:21.745

I think, right around post GPT, for even with chat, GPT, and all that stuff, I think that very quickly started to change. And there was   
(00:04:27.531) ~~like, actually, like~~(00:04:28.072)  
a bunch of legitimate organizational infrastructure,   
(00:04:30.553) ~~etc, etc,~~(00:04:31.334)  
things that changed to put   
(00:04:33.076) ~~like~~ (00:04:33.216)  
very strong divisions in place between these teams. And I'm not delusional in the sense of Google obviously has a strong vested interest in protecting its intellectual property. So it's not even that that   
(00:04:43.259) ~~like there's~~(00:04:43.639)  
there are mitigations and protections in place and there are clear like boundaries and roadblocks put in place. But it still feels like   
(00:04:49.223) ~~the it feels like~~(00:04:50.624)  
at least for me at Google, it feels like in spite of that, like people are still very willing to collaborate. 


---


#### 00:04:55.026

And I actually think a lot of it has to do with the DeepMind team itself just like cares about developers like they want to see and part of this if you from their perspective, like developers are one of the primary surface areas for them to bring this technology to the world. I know partially some of it comes available through the first party product. I think the first party product, the Gemini product, which is incredible and a bunch of folks are using, just has a different sort of feeling about it comparatively against how, at least in my experience, teams felt about ChatGPT. I think a lot of people at OpenAI was like, well, ChatGPT is so successful. 


---


#### 00:05:29.439

Let's just essentially put our eggs in that basket. And we want to work closely with those teams to the point Yeah. Wanting to collaborate really deeply with the ChachiBT teams and not always, at least from my perspective, like wanting the deep collaboration with the API and the developer teams. And obviously there was still a collaboration. So it's not to say that it didn't exist, but it really does feel like the DeepMind team is,   
(00:05:47.786) ~~you know,~~(00:05:48.045)  
developers are incredibly important. Like they're on the ground giving us the feedback about how to make the developer products better. Like I was just this weekend, got a bunch of pings from an incredibly well-written doc from Susan on the DeepMind team. 


---


#### 00:05:59.648

And it was about all the things, the challenges of getting started with Flash and what we need to do to improve that. And it was like, Clearly this person and also like broadly this team of people really care about making this technology accessible to the world. And it was awesome to see that. And then we literally turned around in 24 hours and made a bunch of changes and hopefully improved that experience. So all that's to say. It   
(00:06:19.790) ~~feels,~~ (00:06:20.072)  
at least where I am right now, feels like a culture that is going to help me as somebody who's trying to make products for developers be more effective at my job. And I think ultimately that's what it comes down to. 


---


#### 00:06:28.240

I think there's very real realities of why you would want to have things either way, but I feel like I'm able to build the right things for developers because I have a collaboration with the DeepMind team, which is important to me. Cool. Yeah. It's been an interesting trajectory to watch DeepMind finally really consummate the merger with Google. And of course I've been on the outside of that, but the commentary, even from Dennis, I thought was quite revealing where he was just like, look, we're getting from the point where this has been a   
(00:06:52.196) ~~primary,~~ (00:06:52.656)  
primarily a research problem to now where it's still a research problem, but also   
(00:06:56.336) ~~like~~ (00:06:56.497)  
very much an engineering problem. And it certainly seemed like they came to this moment with a very realistic understanding that   
(00:07:03.918) ~~like~~ (00:07:04.119)  
for this to take to go to the next level, it was something that was going to have to work with the broader strength of Google beyond the sort of research focus that DeepMind had obviously built in such strength over time. 


---


#### 00:07:13.502

Yeah, I think this is one of the tension points now actually for us is like the DeepMind team is   
(00:07:17.363) ~~like~~ (00:07:17.483)  
doing such incredible work.   
(00:07:18.744) ~~It's~~ (00:07:18.824)  
we're not rate limited on how much innovation is coming out of DeepMind and how important the new directions they're making from a modeling standpoint are. It's really rate limited by, can we build the right products around these things? How do we thoughtfully put this technology in the hands of developers and also consumers through all the one-piece service areas? And I think the DeepMind team is chomping at the bit to get this technology out to people. And it is now our job to actually do that work and stay in tandem with them. 


---


#### 00:07:41.834

And it's hard. They just have so many incredibly smart people doing incredibly interesting things that, yeah, I think we have our work cut out for us. Yeah, let the record show that I, for one, never doubted Google's strength   
(00:07:53.201) ~~in the,~~(00:07:53.562)  
at least in the areas where it counts most. If the inputs to AI are, which they are, data, compute, and algorithms, then it always seemed to me quite clear that Google DeepMind had all three of those at the   
(00:08:03.872) ~~highest,~~ (00:08:04.112)  
highest level. And certainly now we are seeing that. So it was at the conclusion of the keynote, whatever, the first day of IO, the count of the number of times that AI was said was revealed. 


---


#### 00:08:15.682

And I believe it topped out at 121. A lot of different announcements there, both on the sort of developer facing side and the sort of integration across the entire horizontal suite of Google products. For starters, what are the things that jump out to you most? I assume you guys have some early use of the first party tool. So if there's anything there that you've had a chance to go a little   
(00:08:33.696) ~~bit~~ (00:08:33.816)  
deeper, farther on, then the rest of us are interested to hear what you think we should be excited about. And then obviously the API side is your bread and butter. I'll be candid in that   
(00:08:41.650) ~~my,~~ (00:08:42.150)  
I'm so heads down on the developer stuff that   
(00:08:46.452) ~~they could have, some people could have~~(00:08:47.894)  
personally sent me an email and said, 


---


#### 00:08:48.894

Hey, Logan, this thing's going to solve all your problems. And I've just, I'm so heads down that I wouldn't have even known. I think there is ways. And now some of it has rolled out to us internally for dogfooding. I think honestly, on the workspace side, the thing that continues to be the most valuable Gemini use case for me, and it just works out of the box is there's a Gemini meeting note taker built directly into to Google meet and you just turn it on at the beginning of the call. It basically takes notes of the whole conversation, summarizes everything for you, and then also specifically does a bunch of action items and tags people. 


---


#### 00:09:16.514

It's one of the best workflows. I just do a single button click. I get an email afterwards with the entire thing put together. I think this had already been released prior to I-O. I'm sure it's going to get better with the new models that are now powering that experience. So   
(00:09:28.807) ~~I think~~(00:09:28.967)  
that's been on the actual Google workspace slash all the different tools that are available, the most useful thing. I've also been experimenting with the travel planning piece on the consumer side. I'm going to the to the Azores with my girlfriend and we were trying to figure out like what are we going to do and what are all the different things. So Again, incredibly well-designed and thoughtful. 


---


#### 00:09:47.575

I just put in how long I was there, the dates, found a bunch of stuff, gave me a travel itinerary. There was a button to export it to a Google Doc. I was like, you could email it to someone. I was like, this is awesome. And again, that's   
(00:09:57.039) ~~what,~~ (00:09:57.179)  
for me as a consumer, what I'm expecting. When I engage with Google's AI surface areas, give me this full experience. I'm integrated into this world. Let me benefit from it. And I think   
(00:10:05.484) ~~the email,~~(00:10:05.984)  
the Google Docs, all those things is a great example of those integrations coming together and actually providing a bunch of value. I think on the developer side, we can talk about Flash and Pro and more in a bit, but those were the two most important things. 


---


#### 00:10:18.729

And then I'll give a special honorary mention for Gemini in Google Chrome. I think that seems incredibly interesting. Again, there's billions of people who use Google Chrome. If you want to think about what the impact of this technology is on the world, that's how a lion's shares of the impact is going to be had is by those types of distributions, which are super interesting to see Google pushing on. Yeah. Okay. So a couple of threads I'll put it in to come back to later. One is the meeting thing and just some of the competitive dynamics that I see shaping up there. And then similarly for the travel planning, although that one I think is more AI versus human competition as opposed to platform versus startup. 


---


#### 00:10:53.136

But let's just talk about the models a little bit first. For one thing, I am not entirely clear. Maybe this is out there somewhere, but obviously a bit of a deluge of information. I wasn't quite able to get total clarity on it. When Google speaks about natively multimodal models with the current generation, the 1.5 generation of Gemini, Can you give us a little bit more detail on what natively multimodal means? Obviously we've seen OpenAI say, okay, this is all basically tokens in, tokens out, regardless of whether it's text, audio or image, video, token, whatever. I'm not even sure on the video piece exactly how to be thinking about that for the OpenAI side either, but I'm less clear on the Google side. 


---


#### 00:11:30.009

Is this a single transformer that takes and generates all these inputs or like how native is this native multimodality now? Yeah, that's a good question. I was just having a conversation with someone. I don't remember if it was earlier. It must have actually been earlier today about this. I think I won't comment on   
(00:11:45.294) ~~like~~ (00:11:45.416)  
how the actual mechanism for natively multimodal happens. I think the TLDR of this is you can put in whatever type of content you want, and you can get an output today only in text and not pay the cost from a developer perspective of having to route things between multiple models. And   
(00:12:02.586) ~~I think~~(00:12:02.765)  
that's like the ethos of what it means   
(00:12:04.508) ~~from a,~~(00:12:04.868)  
again, from me on the developer side of what it means to be natively multimodal is Historically, you would have to   
(00:12:09.312) ~~like~~ (00:12:09.451)  
chain together a bunch of these requests. 


---


#### 00:12:11.113

You'd have to pay the round trip compute or the round trip latency time for every single call. You would have to   
(00:12:15.437) ~~like~~ (00:12:15.537)  
string those together. And essentially it meant any multimodal use case was not feasible to do in a production setting because the latency of doing many different calls strung together, whether it be audio, video, image. combined with some text was just not feasible. And now you take all of those things that you previously needed four different models for, and you can just do them with Flash and do them with an incredible amount of speed. I'll refer folks to the Gemini 1.5 technical report, which   
(00:12:41.500) ~~I think~~(00:12:41.721)  
actually just got released slightly after IO. My understanding, and it's like 150 pages, and I've gone through 70 of them, and a reasonable amount of detail and the other 70, not so much. 


---


#### 00:12:51.110

I don't think that it's talked about in depth, like what it means to be natively multimodal. But   
(00:12:54.511) ~~I think,~~(00:12:54.731)  
I think we can ping Jeff Dean after this and see if he, maybe we get a blog post from the DeepMind team about what it means to be natively multimodal.   
(00:13:01.417) ~~I'm not sure,~~(00:13:01.736)  
but I think it's a good question. I've heard other folks asking it. It's not clear if it's one of those details that like matters. So we should really push to show the world how it works. Or if it's like more of an implementation detail that like the team is intentionally not revealing because it's, there's some secret sauce happening there.   
(00:13:15.966) ~~It's,~~ (00:13:16.067)  
it's not clear to me personally which of those it is right now. 


---


#### 00:13:18.607

Yeah, I guess we'll be able to tell maybe a little bit more over time just with things like, does it pick up on intonation of audio? There's like a pipeline and it's transcribing audio and then feeding the text into the same kind of format as regular text, then presumably it wouldn't notice these things like the intonation in voices. Whereas if we can get a different response, or if it seems to understand the intonation, then that would seem to imply an early fusion type of strategy,   
(00:13:46.168) ~~which,~~ (00:13:46.369)  
and I borrow that term from a recent paper that just came out. It was like a lost in the shuffle of the big week of OpenAI and Google's big announcements, but not to be entirely slept on because they're showing that they're definitely not too far behind either. 


---


#### 00:13:57.833

And they are very much in the mindset to show their work, obviously. This really quickly, Nathan, I think this question about can the model understand variances in people's voice and emotion and tone and stuff like that,   
(00:14:06.735) ~~I think~~(00:14:06.875)  
it's actually a really good question. I'll follow up. I think this had also come up a couple of times, and I think this is an important thing to make clear for developers because the actual use cases that you build depend   
(00:14:14.817) ~~on that,~~(00:14:15.078)  
on whether or not the model understands that piece. So I'll follow up. My understanding is that it might, and it maybe is limited to certain contexts or certain aspects of that, but I'll follow up. 


---


#### 00:14:25.201

Okay, cool. Just in the interest of pruning the space of things that people need to keep track of as well, is there anything that we should be thinking about like anything earlier than Gemini 1.5 on at this point? Or is   
(00:14:37.916) ~~like~~ (00:14:38.015)  
Gemini 1 basically superseded? Yeah, I think almost it is fully superseded now with these new models. I think that was actually part of the Gemini 1.5 technical report is that the Gemini 1.5 Pro model is now better across pretty much every axis that Gemini 1.0 Ultra was, which was never made widely available to folks. I think partially because the team saw it was coming with Gemini 1.5 Pro. I would move my mental model to focus almost entirely on the 1.5 family. 


---


#### 00:15:07.009

So that's flash and pro right now. And those models seem to be pretty much better at everything comparatively against any of the models we put out before. Yeah. And also it should be noted Pretty much the same is almost true across the entire universe of language models. The LMSIS leaderboard just got updated today, finally with Flash appearing on it for the first time. And the new pro models are now basically within the margin of error, or maybe just a couple of points outside of the margin error of GPT 4.0 per the LMSIS leaderboard. And there are   
(00:15:34.139) ~~two models.~~(00:15:34.639)  
There are two 1.5 pro models there. One is called Gemini Advanced. Is that also available in the API, like an online version? 


---


#### 00:15:43.025

That's only in the Gemini Advanced UI experience. Is that right? Yeah, and I don't have full context on... I think it's mostly just there for a showcasing perspective of what that model is capable of. But yeah, you definitely cannot access that via the API today.   
(00:15:57.179) ~~I think it would be like,~~(00:15:58.020)  
I'm interested to see if there ends up being some use cases that folks come up with that make it seem like it is something that we would maybe want to open up to people. But right now it is   
(00:16:06.225) ~~not,~~ (00:16:06.404)  
not accessible other than outside of, it's not accessible outside of the Gemini first party product. Reading all of the docs would be when preparing for this conversation and knowing a little more clarity, exactly what's going on out of the millions of tokens of documentation would be first place I would go. 


---


#### 00:16:20.211

Honestly, I think it's a fair question. I actually think this is my point of feedback that I've given to the LMS team before, which is I do think they should make it more clear exactly what those models are, like having a model page, like what Hugging Face does, honestly, where you can give details, provide a model card. I think right now when you click on the leaderboard, it just goes off to some other thing. But   
(00:16:36.402) ~~I feel like~~(00:16:36.881)  
it's in people's best interest to   
(00:16:38.543) ~~like~~ (00:16:38.682)  
more fully document what these things actually are on LMS. Yeah. OK, so. Nevertheless, the two at the top are the same model. One has a knowledge cutoff that's available via the API. 


---


#### 00:16:51.052

The other one is online. That's not available via the API, but is what you get when you go to use the Gemini Advanced product. And then it's not too many spots down the leaderboard and notably above Cloud 3 Sonnet, where Flash has just landed. And that is pretty impressive given the price point and also the fact that   
(00:17:08.785) ~~both of these,~~(00:17:09.266)  
both the flash and the pro model have the million token context window with 2 million coming soon and talk of from 15 of working on infinite context. And there have been some interesting, it's funny. I wonder if you have any perspective on this that's new. This is a bit of an aside, but obviously intellectual property is like super valuable. 


---


#### 00:17:24.820

Like we're in this general period of closing. I'm hearing multiple reports of. less information sharing even within companies, which is alluded to happening in various ways. And then I see a paper like Infini Attention, if that's how they're pronouncing it, that was out of DeepMind recently, where they show a really elegant, like it looks more like a state space or a state space kind of equivalent, where there's this   
(00:17:46.185) ~~like~~ (00:17:46.346)  
fixed size element that is still referred back to with attention, but it's   
(00:17:51.328) ~~like~~ (00:17:51.429)  
constantly updated and can handle in theory,   
(00:17:53.229) ~~like~~ (00:17:53.349)  
up to infinite attention. And then there's like the more recent sort of sliding window. I'm surprised that something like that gets published. And I wonder if you have any insight or perspective on why some things that still seem like they're like top-notch IP are coming out despite this sort of broader closing of sharing. 


---


#### 00:18:10.869

It's an interesting question. A couple of reactions. One, I have no specific knowledge about this individual paper. I think broadly, I would assume part of it is theater. I would assume part of it is wanting to give folks the credit that they deserve for doing some of this work, which I think is an important part of the scientific process. I think part of it is, again, on the scientific process side, folks wanting to get these ideas out. And again, I don't know for this specific paper if it's   
(00:18:32.847) ~~like,~~ (00:18:32.968)  
this thing is verified and is like the clear path towards scaling to infinite context or if it's more okay here's an idea that might work and it's intended to   
(00:18:40.196) ~~like~~ (00:18:40.317)  
foster conversation with people in the ecosystem i think there's a lot of reasons to publish stuff like that and strategically for deep mind again they need to attract the world's talent i think there's a lot of academic talent that's out there that care about the stuff that's being published from a paper perspective. 


---


#### 00:18:53.451

So I think there is an economic reason why it might make sense to publish, even if in some sense you have to give up some discovery and it's no longer a trade secret or what have you. I think all of those things are at play. I would also not underestimate the value of or the reality of what is actually new versus someone has already figured out and they know someone else has figured this thing out based on what someone said or specifically didn't say in another paper. So the calculated calculus on this could be that it's clear to the DeepMind team that someone has already figured something else out that's very similar to this. And even though they haven't said it in this very specific way, it's not actually brand new, or it could be completely brand new. 


---


#### 00:19:32.396

And they're like, this is the most incredible thing ever. We need to share with the world. I honestly don't know. But I think those are the things that I would think through if I was in that position. Yeah, a lot of considerations, to say the least. It is notable that paper came. And again, there were so many rumors and whatnot.   
(00:19:44.026) ~~I don't~~(00:19:44.307)  
I try not to put too much stock into the rumor mill and the sort of a non account, certainly when it comes to flowers from the future type things. I don't put too much stock into that. But I had heard a little bit that the DeepMind team had some significantly impressive results with the states-based model type work internally and hadn't published it. 


---


#### 00:20:01.278

And then Mamba kind of states-based moment happened at the end of last year, end of this year. And then maybe it was like, OK, well, this is happening, so we might as well bring something like this out. I can definitely see that. And I can also very well imagine that's not the best thing that Google has up its sleeve at this point as well. But definitely notable to see this infinity attention at the same time they're talking about pushing for infinite context. Nathan, if I can impart anything on you, it's that the number of the rumors that are true is so small that it rounds down to zero. And I would always see the most, and again, it's a lot of stuff that you can't just go online and be like, no, this is not true because for whatever the context was, but I was always, 


---


#### 00:20:35.953

I've got a bunch of tweets in my drafts folder about exactly this type of stuff of like, But most of the rumors that you read are totally nowhere close to reality, or they're close to reality but they're missing the most important piece of context. And with an absence of that context it just makes the actual rumor not correct and I feel like   
(00:20:54.040) ~~this is~~(00:20:54.320)  
there's some saying about this or some expression of as you become closer to something, like the more you   
(00:21:00.423) ~~like~~ (00:21:00.564)  
read about it in the newspaper or see something online about it, it just   
(00:21:03.684) ~~like~~ (00:21:03.825)  
becomes, there's   
(00:21:05.144) ~~like, I forgot what the name of the saying is, but there's,~~(00:21:06.905)  
it's just like totally not true and baseless. 


---


#### 00:21:09.547

And it really feels that way about a lot. Again, I don't know in this specific instance, but it always felt that way when I had some specific knowledge that people were rumoring about online at OpenAI and it was never true. So   
(00:21:19.151) ~~I guess~~(00:21:19.631)  
before returning back to Flash, which is definitely something I do want to dig in on a bit because it is super impressive. How would you advise developers who are obviously trying to figure out what to build and where to go, and they're trying to gauge, am I going to get enabled by or steamrolled by the next generation of things coming out from the frontier developers? Should they be trying to zoom out and take a higher level perspective, or are there trusted sources you would recommend? 


---


#### 00:21:45.708

People are not going to stop asking these questions. Yeah. It is important that folks continue to ask the questions. I think it's just worth considering and taking it all with a, like having a very skeptical take, I think   
(00:21:59.276) ~~on,~~ (00:21:59.355)  
on some of all the different rumors, like really thinking about it from first principles. I think on the comment of what should developers be thinking about what makes me excited about Gemini 1.5 Flash. To give a little bit of context, OpenAI released GBT4 March of 2023. I was sitting with Greg in the weeks leading up to that launch and going over the demo that ultimately became him drawing on the napkin and doing that whole experience. 


---


#### 00:22:24.228

And I think when I first saw that happen and when I was playing around with the technology, I was like, oh, this is here and this is going to have an impact right now. And   
(00:22:31.554) ~~I think~~(00:22:31.835)  
the very real reality is until   
(00:22:34.357) ~~honestly~~ (00:22:34.678)  
until flash came out, like the multimodal natively multimodal whole   
(00:22:39.525) ~~like.~~ (00:22:39.684)  
echelon of vision use cases was not actually possible. I gave a talk at the AI Engineering Summit last year as well,   
(00:22:46.624) ~~like~~ (00:22:46.743)  
the middle of last year, and I said that 2024 was going to be the year of multimodal models. And   
(00:22:50.606) ~~I think~~(00:22:50.767)  
that's actually turning out to be 100% true. And again, the thing that gets me excited about this particular moment is the vision use cases were literally not possible before across a couple of different axes, cost, latency, 


---


#### 00:23:02.875

Most vision use cases actually turn out to be people putting in a picture and saying, tell me about what's happening in this specific location, or where this specific object is, or et cetera, et cetera. Those are most vision use cases in production today. And again, those weren't possible before. Flash outputs actually a, you can get the model to output a bounding box, or multiple bounding boxes. So you can say, hey, where is this thing in this image? Tell me where it is. And that makes this whole, there's so many custom image segmentation models that are out there, all this stuff around   
(00:23:30.923) ~~like~~ (00:23:31.064)  
automating, clicking through UIs and stuff like that, that were literally not possible before. 


---


#### 00:23:34.826

The model had, the vision models that were out there, the state-of-the-art vision models, had no understanding of the spatial relationship and   
(00:23:40.672) ~~how that,~~(00:23:40.951)  
and like the coordinate plane of like where things were. And that's now possible.   
(00:23:45.830) ~~Like there is~~(00:23:46.490)  
also as somebody who invests in AI startups and looks at this whole space very holistically, there's just so many new things that are going to be created because of this model, because of the flash models. And it's not even   
(00:23:58.236) ~~like,~~ (00:23:58.375)  
just as a fan of the technology, not even as, again, it's hard to de-bias myself now being at Google, but I really do think that it's this very special moment that it's not actually super clear to me that widely the developer community sees this opportunity, partially because I think there was these huge expectations for all the vision use cases and like none of them have really panned out to any interesting degree. 


---


#### 00:24:20.459

And I think that's, again, finally just starting to change. Yeah, it is pretty amazing. The first thing that I've done with it that really impressed me, and I did go head to head on this with other Frontier model developers offerings, was to the degree I could, actually, because I couldn't entirely do this.   
(00:24:36.128) ~~So, oops, what happened? Okay, I'm back.~~(00:24:37.609)  
As listeners well know, I'm the AI advisor to this company, Athena, that's in the executive assistant space. We've talked many times about how we have worked on this onboarding process where they used to have a hour-long onboarding call, and then somebody would spend four hours was the budgeted time to write up a profile of the person so that they could then hand that off to the assigned assistant that would work with this client and try to give them a good running start to understand who their client is. 


---


#### 00:24:59.482

That process has been largely AI-ified. We still do the human-to-human call, because that's good for eliciting the information, but then to actually transcribe, turn that into a profile, that's now all done with language models. But now we're thinking, well, what more could we do? There's a ton of information, of course, that's locked up in people's Gmail.   
(00:25:16.078) ~~Gmail is almost for sure,~~(00:25:17.760)  
and probably by a lot, the number one most adopted platform across all of our clients. And they all have just an unbelievable amount of,   
(00:25:24.724) ~~you know,~~(00:25:24.944)  
data in there. So we're thinking, geez, and our assistants get access to it as well. So because that's a big part of how they're going to help is like managing your inbox, managing your calendar. 


---


#### 00:25:33.069

So I just tried pulling the most recent 250 emails that I personally had sent. And just dumped them into a single context window with Flash and asked it to write a character sketch about me. Basically no prompt engineering, nothing like, I didn't really even iterate on this much. And I was really impressed with what it was able to do. And   
(00:25:55.355) ~~this was,~~(00:25:55.615)  
it turned out with my email patterns, whatever idiosyncrasies I may have, 250 emails with the content replied to and forwarded or whatever the case may be. It was about a thousand tokens per   
(00:26:05.757) ~~email.~~ (00:26:05.856)  
email. So with these 250, I'm looking like a quarter million tokens. That obviously exceeds the context window that are available from other providers. 


---


#### 00:26:51.746

I want to make sure I have good clarity on this too, I believe comes in under 20 cents at a quarter million tokens times the 70 cents. So that was definitely an eye opener where I was like, man, for a couple of bucks, we can   
(00:27:03.808) ~~like~~ (00:27:03.989)  
really understand a client's whole many different facets of their life, right? We're thinking about things like, What can we go find every gift that they've ever given in their, in their email history and pull out all the people that they should be thinking about giving gifts to. And   
(00:27:15.851) ~~the,~~ (00:27:16.011)  
the assistant could be proactive perhaps about that, or can we get all of your travel habits and every loyalty program number that you have and put that into a spreadsheet form. 


---


#### 00:27:22.415

And it looks like this stuff is like very possible. And honestly, like not even that hard to do. It's crazy to think that even with GPT four original with the 8,000 tokens, I've joked that context window inflation is the best hyperinflation. You would have to, that would handle eight emails of my thousand tokens, right? And that's before generating anything. So I could maybe get seven in there or six or five, depending on how long they were or whatever. And now   
(00:27:45.451) ~~I've got these, I would have to,~~(00:27:46.192)  
and you think about the time and the cost and the every once in a while would fail and the complexity of that. And life has just gotten   
(00:27:50.915) ~~so,~~ (00:27:51.296)  
so much easier for developers   
(00:27:53.498) ~~to,~~ (00:27:53.617)  
to get   
(00:27:54.077) ~~like~~ (00:27:54.198)  
a really good output back. 


---


#### 00:27:56.220

Interestingly, that is not something that the Gmail integration will do yet. I asked it to do the same thing and just said into Gemini in Gmail, like, could you read my recent emails and write a character sketch of me? It said it couldn't help with that. So anyway, I'm going on too long. That's my story of   
(00:28:08.788) ~~Flash.~~ (00:28:09.087)  
  
(00:28:09.228) ~~Tell me a story of yours or somebody else's that you think is worth highlighting.~~(00:28:12.390)  
A couple of reactions to this. One, as an Athena customer, I'm glad that you're doing this work because it actually sounds incredibly useful. I've gone through this as like a use case, but for the assistants or just like anyone trying to help someone with anything, the nuance and the contact and like the very specific context matters so much. 


---


#### 00:28:31.087

I was doing this with, I was using AI studio and the Gemini API to do drafts and just taking different passes at the Gemini 1.5 technical reports and like trying to, doing exactly this. Okay, pull out interesting insights from here. We should actually do a live demo of asking some of the questions that you asked about, like what makes this natively multimodal? You can just upload the PDF and ask. I probably have it sitting in my setup still. So I'm curious if we can do that and see what happens. But   
(00:28:54.154) ~~it's, there's so many,~~(00:28:56.776)  
The other thread that came to my mind around this is, I actually think that, and I'm curious to double check this, but I'm pretty sure that Flash just passed GPT-4, the original GPT-4 on the LM-SYS leaderboard, and I'm curious if you can fact check me on that to see if that's true, the 0.3.1.4 version, which I think was the original. 


---


#### 00:29:15.576

That model was $30 per million input tokens I'm pretty sure and the updated version or the 1.5 flash version is now I think it's 35 cents for under 128k tokens   
(00:29:31.586) ~~or~~ (00:29:31.747)  
and then 70 cents after that so almost a 90 x or 70 x whatever it is decrease in cost   
(00:29:40.557) ~~for that~~(00:29:40.877)  
for a model that's just as intelligent for a model that   
(00:29:43.599) ~~is~~ (00:29:43.680)  
is more capable and i say all that to say not to compare these two but also just like back to the thread of the conversation of like how should developers be thinking about this technology like that trend is not going to stop like that trend of the models becoming faster, smarter, cheaper, more capable, being able to infuse even more AI into the products and services that people are building is going to be the path that we are very clearly on. 


---


#### 00:30:05.775

And I was in another call earlier today and was talking about the tools and how people are using AI as a tool and how, in many ways, people are taking AI today and being like, oh, I'm going to put AI here, and I'm going to put AI here, and I'm going to put AI here. And the actual future outcome of this technology is   
(00:30:22.800) ~~like,~~ (00:30:22.901)  
The AI is going to be everywhere like your product is going to be and is like going to have AI infused and AI is going to be like the one of the primary interfaces of interaction with your product, and not enough people I think are thinking. to that order of magnitude and that level. 


---


#### 00:30:38.546

And I think partially it's because the technology is not actually there yet. I have empathy for that. But I think having that in the back of your mind of what that world is going to look like and what is your specific product or services perspective in a world in which AI is everywhere and it is, as the saying goes, too cheap to meter. Intelligence is too cheap to meet. It'll be too cheap to meter because there's so many things that are being built with it. It's useful to think about.   
(00:30:58.419) ~~I think~~(00:30:58.818)  
the really quick comment about what I've seen people building with Flash, I would be really interested to see, and I think I've seen some demos actually from folks who we were at I-O with, around what does an open Astra look like? 


---


#### 00:31:08.582

The demo that Google did and the DeepMind team did with putting on the glasses and being able to ask questions.   
(00:31:14.304) ~~I think~~(00:31:14.544)  
you could probably recreate a lion's share of that demo just using the 1.5 Flash API. And people were all talking about, oh, is Google You can go buy that similar hardware like that just off the shelf for probably a few hundred bucks and either connect it to one of the OpenGemma models or connect it directly to the Gemini API and make that workflow work for yourself. So it'll be really interesting to see how that actually plays out. It's on my ever-growing to-do list to buy a pair of glasses like that and try it out and see if I can recreate the demo myself just using the API. 


---


#### 00:31:43.875

And again, my instinct is yes. Yeah, it seems like the, if like in the immediate wake of GPT-4 was the agent's craze and then it was, okay, well maybe not quite yet, but we can see where this is going. Now it seems like with the ability to watch the screen and for things to be cheap and like low enough latency, it seems like the proactive coworker is the new thing where I'm seeing   
(00:32:06.076) ~~like~~ (00:32:06.175)  
a ton of that popping up, whether it's Obviously, we've got the ChatGPT desktop app in limited rollout, and Astra and Pietro made a demo at the airport, a simple version, obviously, but it was impressive to see how quickly he was able to put even a simple version of that together. 


---


#### 00:32:21.580

What did the specs look like on that for I haven't benchmarked this extensively myself yet, but for Flash, how should people think about like time to first token and token per second type of metrics? Cause   
(00:32:35.349) ~~like~~ (00:32:35.450)  
with the thing that I did with the 250 emails, 250,000 tokens, and it generated 2000 ish tokens in response. And that took   
(00:32:41.574) ~~like~~ (00:32:41.693)  
about 45 seconds. So that's on the one hand extremely fast, but on the other hand, probably I shouldn't put that much context into my,   
(00:32:48.778) ~~like every,~~(00:32:49.960)  
it wouldn't be fast enough to do it like on a sort of proactive, suggestive basis.   
(00:32:54.282) ~~So.~~ (00:32:54.403)  
Are there any rules of thumb or just guidelines for how fast we should think about these things as being given varying amounts of context? 


---


#### 00:33:01.904

Yeah, it's a good question. Latency continues to be a challenging thing to articulate to an external audience because there's so many confounding factors of what does latency actually mean? current load that the server is under affects latency and time to first token.   
(00:33:15.769) ~~Like~~ (00:33:15.890)  
it varies by day. There's historically across usage patterns, different times of the day have different peak loads, which then impacts latency. There's all these   
(00:33:22.811) ~~like~~ (00:33:22.951)  
weird effects. I think back to the comment that I made earlier, I think this is actually something that I'm hopeful that LMSYS   
(00:33:29.853) ~~and in absence of LMSYS, I think~~(00:33:31.334)  
somebody else should do this. Like How can we make a benchmark that is actually representative of   
(00:33:35.914) ~~like~~ (00:33:36.055)  
all of these trade-offs as   
(00:33:37.056) ~~you are,~~(00:33:37.355)  
as me, as a developer,   
(00:33:38.756) ~~as you,~~(00:33:38.936)  
as a developer, you're thinking about how to use this technology. 


---


#### 00:34:09.733

I think would actually be incredibly interesting to developers. And again, I bias, but I don't think that like the ELO scores for Flash are like actually representative of like how transformative it's going to be for developers because it's ranked whatever it's tied for like ninth or something like that. But it's also 10 times cheaper than a bunch of similarly capable models, and also multimodal, and also et cetera, et cetera. So it's really interesting to think about that.   
(00:34:32.235) ~~I think~~(00:34:32.655)  
that's the thing that keeps ringing in my head. I do think we probably need to put out a little bit more guidance around latency. My instinct is it's three times-ish faster in a bunch of use cases that I've tried than Pro. 


---


#### 00:34:43.382

But I've almost fully moved over a bunch of my daily AI use to Flash. And it seems to be just as capable in a lot of the use cases that I'm messing around with it on. Yeah, that's interesting. The fact that you're doing that as a first go-to is definitely pretty telling. The numbers for what it's worth are the ELO score for Flash right now is 1232, and that is a full 50 points ahead of GPT-4. It's just under 50 points ahead of GPT-4-03-14, the original. And it's funny, the least popular GPT-4 continues to be the June of last year version. So it's like a full 70 points ahead of that. And it's only   
(00:35:22.054) ~~like~~ (00:35:22.175)  
15 points behind the January version of GPT-4, which is, as you noted, like more than 10 times more expensive, either like 30 times more expensive or like 12 times more expensive, depending on whether you're above or below the 128. 


---


#### 00:35:35.907

And just to be clear on how that works too, is it basically like It's a hard cutoff, right? If I send in 127,999, I'm billed at the one rate, and I tip over, I'm at that other rate. That sort of suggests   
(00:35:49.434) ~~like...~~ (00:35:49.594)  
some sort of hardware is I'm like using more hardware, I guess, is probably what's going on under the hood. Otherwise, I don't know why there would be a breakpoint. I guess that might be a no comment one, but just at least make sure I have that correct. It is a hard cut off. I think actually, I think the comment of it being such a hard cut off actually doesn't make a lot of sense. 


---


#### 00:36:10.108

I think the intent is actually more so to like the cost of doing compute on higher numbers of tokens is not linear. So I think broadly that's true. So I think this is more so trying to embody the reality of the costs associated with running these models, which is that it's a much higher cost to do some of those larger token requests. It just requires a lot more compute. So yeah, take that for what's worth. And I think on your comment about the 0613 model,   
(00:36:35.623) ~~yeah, well,~~(00:36:36.123)  
a couple of years we'll get a blog post or another podcast about why that model is slightly worse than all the other GPT-4 models. Interesting.   
(00:36:44.766) ~~Well, it'll be,~~(00:36:45.427)  
the world might be very different place by the time you're able to tell that story in full, but I look forward to it nonetheless. 


---


#### 00:36:50.228

When you guys are building internally at Google, and I know you're not exactly doing this, but like the things that we saw Astra, for example, out of the labs group, are they basically building on the same thing that we as developers either are now able to build on or like soon we'll be able to build on? Is that basically a dog fooding exercise? Yeah.   
(00:37:12.478) ~~Flabs didn't build acid.~~(00:37:13.498)  
Just to clarify the deep mind team has built the Astro project labs, builds a bunch of the cool stuff. I think there's like very specific circumstances where they might be like running their own stuff, but actually most there's many thousands of internal teams that build directly on the Gemini API, like the same API that we make available to developers is the same API that teams use. 


---


#### 00:37:30.585

I think that the only Delta, the reason why teams might not use those models out of the box is like they need some custom post-training data that's not represented in. the existing models that are available to APIs available through the API. And again, if that team has the muscle and the resources to go and do custom post-training, then they might go and do that to make,   
(00:37:48.096) ~~you can,~~(00:37:48.315)  
this is just a made up example, but like the maps team, if the model doesn't have enough maps data, and for some reason, there's a bunch of use cases that would require that if they had the resources, they might go and build off of the base model and go and post-train their own version for some specific use case. 


---


#### 00:38:01.103

Gotcha. Okay, cool. So do you actually want to do the sort of walkthrough? So I'm interested to hear your stepping into a position here where the competition is obviously fierce for the developer accounts that there's like multiple dimensions to it, the models being certainly the primary one, and like what actual capabilities you can get at for what price, but the friction and the developer experience also definitely matters. I have, will confess to having been confused, certainly at times in terms of   
(00:38:27.644) ~~like,~~ (00:38:27.764)  
where do I go for what within cloud versus vertex versus AI studio. If you actually have the Gemini 1.5 technical report loaded up and you want to   
(00:38:35.909) ~~just~~ (00:38:35.989)  
do the walkthrough in the AI studio, that would be, 


---


#### 00:38:37.789

I think, a useful Exercise. Yeah, let me look really quick to see whether or not I have it. And even if not, I could just throw it in there.   
(00:38:44.795) ~~Yeah.~~ (00:38:44.976)  
  
(00:38:45.056) ~~Well, we can edit. If there's a little delay, we could take it out. I think I have it right here, actually.~~(00:38:48.538)  
Let me switch over to my, sign into my personal Gmail account, and then I'll do it from there. Just because I think my Google accounts have certain stuff in AI Studio that's A-B tested or something random like that. So I just want to make sure. Yeah, I'm curious what the technical report will come up with there. I'm curious about that specifically, that multimodal question that you asked. 


---


#### 00:39:06.010

That's a totally unrelated topic. Are you getting logged out of everything in Chrome these days? I feel like right around the same time that we got the thousand heads ups about the login experience changing. I also, my biggest notable change was that I was like logged out. I've now been like logged out of everything nonstop. Have you had that experience?   
(00:39:23.646) ~~You know what, I feel like I was having this conversation with someone because~~(00:39:26.367)  
we were exploring should AI Studio use a different kind of auth than it has right now and whether or not users would be upset about that. I was like, I'm so numb to signing into Google because I have so many different Google accounts and I use Safari and my personal computer and stuff like that. 


---


#### 00:39:40.215

So I am always like... brainwashed into signing into everything, so I'm not a representative sample. I feel like I do it like 50 times a day now, where I click through the Gmail off into whatever app. It definitely was a notable uptick in just how frequent that was popping up for me. Interesting. Yeah. I'll dig around and see if I come up with anything. I'm not 100% sure. Okay, cool. So I can see your screen and yeah, maybe just give us a little bit of like context for what this is and how it relates to other flagship Google properties. Like I'm not clear on, is this a sort of playground type of environment, but when I actually want to go to production, 


---


#### 00:40:19.282

I need to switch over to Vertex still, or what is the sort of overall developer journey that folks are supposed to go on and how does this fit into that? Yeah, this is a great question. I'm glad that you asked that. It is top of mind for me to simplify this and make sure that it's abundantly clear to developers. I think us having to talk about it is a great reminder that we have a lot of work to do in this space. Broadly, if you are somebody who knows that you need an enterprise cloud solution, that is what Vertex is for. For whatever the constraint is, whether it's like a legal, regulatory, privacy, You need some specific SOs, you need to have some legal agreements signed because of the context of your business. 


---


#### 00:40:53.108

All of those things are like traditional things that an enterprise cloud provider would do. And you can get all of those things from Vertex. And   
(00:40:57.751) ~~I think~~(00:40:57.911)  
it's the right place to go if you need those things. If you're just a developer who's like, I need to build AI into my startup. I want to use Flash. I want to use 1.5 Pro. There's two things that you need to be aware of. One, AI Studio is the interface to get started with this technology. You can do a bunch of prompting, which we'll do here in this UI. It's essentially just a playground. You can get your API key. You can do a couple of other things like make a tuned model, which you can also do through the API. 


---


#### 00:41:20.463

So this is where you would get started with the technology. You can also just go to ai.google.dev, which is where our developer documentation lives. Again, you'll still need to use AI Studio to grab an API key for the API. but you can go to production, you can scale in production. We support,   
(00:41:34.369) ~~again, similar,~~(00:41:35.150)  
the mental model that I give to people is   
(00:41:37.431) ~~like,~~ (00:41:37.590)  
there was OpenAI and there was Azure OpenAI. For us, we have the Gemini API, and then we also have the Gemini API available in Vertex, which is our enterprise cloud solution. So you can choose either of those. There's very real reasons you would want to use either. For most developers using enterprise cloud solutions, there's a bunch of friction involved for good reason. 


---


#### 00:41:53.536

So they tend to go with the less friction option, which is, in our case, AI Studio and the Gemini API. Gotcha. Cool. So   
(00:42:00.135) ~~I don't,~~(00:42:00.315)  
for most people, if you don't have a special requirement, you don't even have to concern yourself with Vertex. Correct.   
(00:42:06.036) ~~Yeah.~~ (00:42:06.336)  
Unless again, unless you have a specific need for an enterprise cloud solution,   
(00:42:09.597) ~~like I don't think that you can get~~(00:42:11.398)  
pretty much everything you need directly out of the box with AI studio, the Gemini API. Gotcha. Okay. Yeah.   
(00:42:17.438) ~~And~~ (00:42:17.599)  
yeah, so we're in AI studio again, simple prompt interface. I put in the Gemini 1.5 technical reports, 115,000 tokens. And we were talking before about, natively multimodal. Can you tell me what makes 1.5 natively multimodal? 


---


#### 00:42:34.387

What does that even mean? And we can go and find out. And we'll see what happens in a couple of seconds. Also, can you do me a favor when we publish this and edit out my email from the bottom left down here? Okay. Good. I'll mark the clip. Just in case. It's not that I don't want people to email me, and I don't really care if people know my personal email, but it just saves me the hassle of not answering emails. The document you provide doesn't explicitly state what makes Gemini 1.5 natively multimodal. Interesting. And this is exactly what I would have expected. Yeah. I don't think   
(00:43:22.322) ~~that~~ (00:43:22.483)  
it mentions,   
(00:43:23.344) ~~like,~~ (00:43:23.485)  
it doesn't talk about the architecture and   
(00:43:25.088) ~~why,~~ (00:43:25.409)  
why slash how it actually   
(00:43:27.833) ~~is~~ (00:43:28.173)  
actually doing. 


---


#### 00:43:30.458

Are there other. best practices. I know at one point when the vision things were just coming out, there was some findings around if you overlaid a grid on top of   
(00:43:40.742) ~~like~~ (00:43:40.862)  
a web UI, for example, it would help it understand and not even understand, I think would seemingly understand fine. But if you needed it to say like where to click on a UI, having that grid would sometimes help it   
(00:43:50.487) ~~like~~ (00:43:50.628)  
get to the right coordinates. As you noted, like many ways to pre-process images, is that stuff still needed or helpful with the latest models? Yeah, I don't think that it is. I wonder if we can use one of these examples and I'll say something like with grid coordinates for the eclipse. 


---


#### 00:44:18.327

Let's see what happens. So I think because the way that these models have been trained now to   
(00:44:26.034) ~~like~~ (00:44:26.134)  
actually understand the spatial relationship and the coordinates and stuff like that, I can't see or analyze images, so I can't provide grid coordinances for the eclipse in the image. Interesting. I have seen this on 1.5 Flash. I'm curious if 1.5 Pro does the same thing. So the classic, you give the model new capabilities and you have to convince it that it has those capabilities. How many squares wide should the grid be? How many squares wide? Yeah, this is a good question. This is a, perhaps a bad example. I have a nice doc from the DeepMind team about the specific prompt engineering that I need to do to make this use case work. 


---


#### 00:45:08.539

So maybe I'll punt this example until I put it into the developer documentation, which is, unless I can find it really quickly. Yeah. Prompting for object detection. Yeah, this is a good... Maybe a good example. Go Ymin, Ymax, Xmin, Xmax, and use that. And I'm curious whether we'll be able to... Nope, doesn't want to do it. Or maybe it can't see the image anymore. Don't need to know the dimensions of the grids that you want to use. I guess maybe the model doesn't have access to the size of the image in this case. Wonder if percentages would be viable in that case. It's funny how much of the job is doing this kind of stuff. 


---


#### 00:46:23.793

Just trying to figure out how to talk to these things and what their blind spots are. Yeah, I will say this is a While this is not really intended to be a place that people come for regular use of the models, I actually have found it to be useful in a couple scenarios. With all this context popping up, I'm assuming we're getting somewhere. The one thing that I find to be like, and maybe this is a compute thing at heart, but I find it to be remarkable that it's not easier to set up a template with a long doc just loaded fully into context. Like when the GPT is first launched, it was like, okay, great. 


---


#### 00:47:05.461

Now I can put my whole code base in there, but then I would do that. And then it would be like. Try to search through it, not load enough stuff in and then miss things. And I was like, okay, but I actually just want you to read the whole code base. Cause I know   
(00:47:16.027) ~~you can't,~~(00:47:16.367)  
you have enough room for that, but it wasn't really designed for that. Clod, I still doesn't have that as   
(00:47:20.909) ~~like~~ (00:47:21.009)  
a template setting. And actually this is like one of the few places where you can come and just have a preset prompt that has a few docs. I have a couple of template prompts in my own AI studio where. 


---


#### 00:47:32.492

One of them is like 20 different mixture of experts papers. I don't go back to that one that often. That was more of an individual like sequence of investigations, but there were just, I was trying to get a handle on what is up with mixture of experts. Notably, I think it is stated that this is a mixture of experts architecture   
(00:47:47.262) ~~that we're,~~(00:47:47.561)  
that we're working with here. And that's obviously become standard frontier at this point. So just trying to get a handle on that. It was like, I'm going to have probably however many rounds of back and forth on this to try to educate myself and just loading in those 20 papers.   
(00:48:01.652) ~~Like.~~ (00:48:01.751)  
It's funny, like that's a pain in the butt, but the ability to just save that here   
(00:48:05.442) ~~as a,~~(00:48:05.762)  
as a preset is actually like pretty useful and has me coming back to it occasionally as   
(00:48:09.184) ~~like~~ (00:48:09.284)  
a retail customer, even though that's not something I'm like trying to productize. 


---


#### 00:48:13.735

Yeah, it is interesting. I think part of the context is that the AI Studio product has the DNA and the roots actually in the consumer. It was originally called Mobile Maker Suite, and it was about building automation flows and things like that. And it ultimately got transformed into AI Studio, which is this sort of playground product. But I think a lot of the initial DNA was more of a consumer product, which is interesting. And I think very clearly, the direction that we're pushing in is towards a developer product. But I do think that part of the magic of this is, and actually to your comment about email is like something that we've thought about, about ultimately we want people to be able to see that this technology is useful. 


---


#### 00:48:48.581

So being able to import a bunch of your emails and use Gemini directly through this interface, I think has a potential to be really useful to people. I think the balance to strike is we don't want to make this too much of a consumer product. Like ultimately what matters is   
(00:48:59.547) ~~like~~ (00:48:59.666)  
developers building stuff with the API. So we don't want to   
(00:49:01.909) ~~like~~ (00:49:02.028)  
over incentivize people to come to AI studio and do all their AI workflows directly inside AI studio. It would be quite the accident of history if that continued to be the thing. I do want to talk a little bit more about, first of all, I don't know how you're doing on time. I definitely could ask a few more concept questions. 


---


#### 00:49:18.032

Let's do a couple more questions. I got to run to dinner at 7 o'clock with my family. Let me just let them know. Let's do a couple rapid fire ones then. Let's do it. Okay, just roadmap then. The VO, should we expect that to be a slow rollout a la Sora, or is that something folks will actually be able to build into products in the not distant future?   
(00:49:36.224) ~~It's a really good question, and I honestly don't have the answer.~~(00:49:38.585)  
My expectation is that   
(00:49:39.965) ~~the~~ (00:49:40.025)  
The tooling is actually pretty robust that part of video effects that the labs team and other contributors have built. So I'm not 100% sure what the rollout looks like, but it seems like a very distinctly different product slash rollout strategy than Sora from my understanding and from hearing Josh talk about it. 


---


#### 00:49:59.396

Okay, cool. I'm on the wait list. If you could put in a good word for me, that one is definitely a priority at Waymark. How about on the rounding out the suite of tools a little bit? Obviously, as you well know, OpenAIR has the assistance API that   
(00:50:11.947) ~~kind of~~(00:50:12.146)  
brings an integrated RAG component as well as   
(00:50:14.548) ~~like~~ (00:50:14.708)  
a tool use thing into a single product. As far as I know, there's not like a RAG element. There is tool use, but it doesn't seem like it's been emphasized very much. So what's the future of those things? Will there be like a packaged up version? Yeah, we have function calling right now. We have a bunch of improvements that we need to make on function calling, so you can imagine a function calling v2 coming, though I say v2 just to emphasize that we'll make updates to it. 


---


#### 00:50:38.925

It's not clear how substantial those changes will be if it's just improving the accuracy of the model-like function calling or what that will look like. We actually do have in the Gemini API today a semantic retrieval API that's been built in, which took a bunch of work. So you can upload a bunch of documents into a corpus and then do semantic retrieval on top of that. I think we're still early in our thinking about what that product will look like. It's not clear that the current design and what we've built is the thing that we'll keep running with long-term. But I think it's been useful to look at that. On the Vertex side, they have an agent builder flow, which allows you to do a few more of these use cases a little bit more robustly. 


---


#### 00:51:10.873

And we don't offer that yet, but   
(00:51:12.193) ~~I think~~(00:51:12.373)  
it's possible we might. take what they learned on the Vertex side and bring some of that over into the Gemini API as well. Okay, cool. That's interesting. What about fine-tuning?   
(00:51:20.061) ~~I think you mentioned that there is,~~(00:51:21.003)  
I know there are   
(00:51:21.503) ~~like~~ (00:51:21.643)  
some things that can be fine-tuned, like what can be fine-tuned? I can't fine-tune like 1.5 Pro, can I? You can't fine-tune 1.5 Pro, but on Thursday we'll announce, or coming on May 30th, so maybe after this video is released, 1.5 Flash fine-tuning will be available. And I think we have such an interesting value proposition with Flash in that you don't pay more cost for inference, and you don't pay to train. 


---


#### 00:51:42.764

So it makes it this very unique value proposition that actually, again, nobody else is offering right now, which is really exciting to me. No pro tuning yet, but flash tuning will be announced, not fully rolled out, but announced on Thursday.   
(00:51:55.460) ~~Wow. Okay.~~(00:51:55.880)  
That's interesting. Should we think of that as the same? I think fine-tuning is very much a point of confusion, right? I tried at one point trying to fine-tune OpenAI models to write as me. That turned out to be not viable. Currently, the best write-as-me solutions, one I would say is probably Claude Opus. And I should try again with the latest date stamp of Gemini 1.5 Pro because that was like, That was the thing up until Opus. 


---


#### 00:52:22.797

But how should we think about fine tuning? My general rule of thumb is if you're narrowing in on a task, you can use fine tuning to dial in exactly how you want it to behave for a specific task, but then you have to make sure that you're controlling inputs and outputs effectively. You lose the generality. If you want to do something   
(00:52:37.750) ~~sort of~~(00:52:37.929)  
ad hoc, like write as me, summarize all these documents or whatever, there you're probably just better   
(00:52:42.193) ~~context stuffing.~~(00:52:42.773)  
How would you refine my understanding of that? Yeah,   
(00:52:46.313) ~~I think this~~(00:52:46.773)  
when I was between Google and OpenAI, I gave a serious thought into making a startup around this problem, this   
(00:52:51.836) ~~like~~ (00:52:51.976)  
right as me problem, because   
(00:52:53.137) ~~I think~~(00:52:53.358)  
it's   
(00:52:53.539) ~~like~~ (00:52:53.659)  
the real challenge is you can get pretty far with fine tuning. 


---


#### 00:52:57.041

The problem is, it's like a traditional machine learning problem to like actually make sure that you have a representative data set that's balanced and like focused on the right things. And it's   
(00:53:06.349) ~~like,~~ (00:53:06.489)  
you're probably actually capable of doing this. But   
(00:53:09.393) ~~I think~~(00:53:09.612)  
like broadly, the market of people who are going to figure out through the right experiments, figure out how to actually make this work is like a very small subsection of people. So my guess on rank fine tuning, I'm not sure it's even really super possible. It seems like facts are just really hard. So it's like you need some sort of retrieval help probably anyway? I think it's both of those things. And I also think it's like synthetic data magnification, stuff like that. 


---


#### 00:53:34.541

Like a lot of people just don't have enough content to actually like, you need more examples to make the model really good at what it is and like being really thoughtful about what you're doing with fine tuning versus what you're doing with rag. Yeah. Okay.   
(00:53:46.311) ~~That is,~~(00:53:46.530)  
that was definitely tricky.   
(00:53:47.692) ~~I don't,~~(00:53:47.931)  
I'm not sure if I'm capable of it or not. I maybe gave up too soon, but I didn't succeed. So time will tell. Okay. Maybe three, You could go on a long time, but you can be as brief as you want. I'll see if I can fit three in. When you had said a while back, this was back in the OpenAI era, 


---


#### 00:54:03.121

OpenAI is only as good as its latest model. And that has stuck with me because it really suggests that the competition has potential for a winner-take-all dynamic because it is pretty easy to switch between models in many cases. You've got a reprompt engineer, but it's   
(00:54:18.748) ~~like,~~ (00:54:18.867)  
It's a pretty simple swap in a lot of cases. How would you characterize the state of competition amongst the Frontier developers today? And   
(00:54:27.802) ~~like,~~ (00:54:28.003)  
how much are you guys thinking about each other and trying to time your announcements to scoop each other? What's the real vibe as you guys are competing in this world as our last model situation? I have an enormous amount of respect for Sam. I'm not sure that I agree with the, 


---


#### 00:54:42.327

I never think about competition piece of it. I think people are like very aware of how much competition there is. So it wasn't, yeah, I was not aligned with that. I think to me, something that has become abundantly clear is that   
(00:54:53.715) ~~the~~ (00:54:53.894)  
we're not going to end up in a winner take all situation. I think the players in the market understand how much of an opportunity there is with this technology, how transformative it is. If anything,   
(00:55:04.032) ~~I think that's,~~(00:55:04.454)  
that has pushed even more people who normally wouldn't compete in this space to compete in this space, which I think is a net benefit for everyone. So, especially with where open source is and how many people are pushing from a frontier lab perspective, it's super exciting to be a part of. 


---


#### 00:55:17.541

And I would actually expect that like even more people are going to end up competing as they finally wrap their head around how big of an opportunity there is here. Interesting. That's quite contrary actually to my expectation. I feel like we're seeing the second tier of foundation model developers, like getting thinned out right around now. And I expect that there'll be a couple of Chinese champions. There might be like an Indian champion, like   
(00:55:39.150) ~~Mr. All might be like~~(00:55:39.791)  
the champion of Europe, but I think we're headed for 10, maybe companies that could make a credible case that they're   
(00:55:45.637) ~~at the,~~(00:55:46.036)  
at or near the frontier. You think it'll be more than that? I think it's hard to know the specific number, but my guess is just because of how much value could be accrued that a lot of people, like anyone with any amount of technical understanding and sufficient resources is going to go and do this. 


---


#### 00:56:02.152

And there's a lot of people who don't have enough sufficient resources and they'll go do open source and that will continue to push open source even closer to the frontier. So I'm hopeful that we'll end up in some really nice symbiosis. And   
(00:56:11.840) ~~I think~~(00:56:12.001)  
for people betting on taking the entire market to be successful,   
(00:56:16.864) ~~I think~~(00:56:17.085)  
it's not likely to be the best outcome for those companies. And   
(00:56:20.628) ~~I think~~(00:56:20.809)  
there's a lot of businesses where they just need to make a great model for it to be an incredibly valuable thing for their business. I think that's actually positive. OK. I don't know if I have time for two more or just one. The another recent tweet that really caught my attention was, and you've got a podcast, you can plug your own podcast. 


---


#### 00:56:35.960

You're in the podcasting arena now.   
(00:56:37.822) ~~Um,~~ (00:56:37.902)  
but I haven't heard this episode yet, but I saw your tweet saying that if AGI were here today, people wouldn't know what to do with it. And I'd love to hear more about what you mean by that. Cause I feel like I would know what to do with it. Or at least I think I would, if it's an AGI that is literally, if we're talking can outperform humans at most economic work and it's highly autonomous.   
(00:56:53.710) ~~Um, what, what are,~~(00:56:54.672)  
what are people not going to get about that? Or am I using the wrong definition or please explain. No, I think you of all people would know what to do with it because I think you're positioned in this ecosystem in a very particular way. 


---


#### 00:57:05.126

I think that the commentary was more that again, continuing to hit on this story of most people still have never even used GPT-4. Most people have never used GPT-Gemini 1.5.   
(00:57:13.432) ~~Like~~ (00:57:13.572)  
most people haven't used this technology. So everyone thinks that there's going to be like the singularity, like if someone gave me AGI right now on my computer and I can access it through an API or an interface,   
(00:57:23.262) ~~like~~ (00:57:23.382)  
that is not. time in which it'll take for the world to change is like very long. The world is a big place. There's a lot of things that are going to happen, but also the sort of conversation with Connor, who was also at IO, and I don't know if you got a chance to chat with him, but he's incredible. 


---


#### 00:57:37.911

I love Connor so much. And he gets to spend his time like thinking about how can we empower people who don't have any technical background to really leverage this technology and understand how to build with it. And   
(00:57:47.735) ~~I think~~(00:57:47.914)  
it's   
(00:57:48.074) ~~like~~ (00:57:48.195)  
such a powerful message because again, most of the world is not technical. Most of the world doesn't really care about this technology. It's more about   
(00:57:53.177) ~~like~~ (00:57:53.297)  
how they can use it as a tool.   
(00:57:54.438) ~~So.~~ (00:57:54.518)  
So maybe   
(00:57:55.197) ~~if I can speak one more and that~~(00:57:56.139)  
maybe suggests where you would direct people on the developer side in terms of opportunity. Going back to earlier in the conversation, you said one of the great workflows is just turning on meeting assistant in Google Meet and it will take notes and assign to do's and whatever. 


---


#### 00:58:09.364

Of course, there are like a dozen startups that are competing for that niche as well. I came away, honestly, from IO feeling like, man, the platforms have such incredible economies of scale. They've got the distribution, they can afford to build a lot of things in for free. Obviously, Meta's put everything free. GPT-4.0 is free.   
(00:58:24.021) ~~I don't even,~~(00:58:24.521)  
I pay for Google advance. I'm not sure what I'm getting for free or not, but certainly there's ability to put stuff in for free. How do you think developers should be strategizing for what opportunities they can pursue that Google won't pursue, or can they out-execute? It seems like distribution is going to be a really hard uphill battle for any of these meeting note-takers going forward, right? 


---


#### 00:58:45.621

But it wasn't that long ago that would have been considered a frontier. Oh my god, yeah, Google's not going to do this anytime soon. But I'm old enough to remember those days, and they weren't that long ago. So how do I stay ahead of that wave and not get crashed over by that wave? I think the distribution piece is definitely one of the advantages that larger companies have over startups.   
(00:59:02.153) ~~I think~~(00:59:02.355)  
the real reality for startups, and I've felt this myself now having sat in many different seats in my life, is you have, there are so many inherent advantages to startups,   
(00:59:09.880) ~~which, you know,~~(00:59:10.679)  
now being in a large company again, like I would beg to have those things as advantages. 


---


#### 00:59:14.722

Again, the fact that you can have a very small focused group of people who are just going to go and execute and build and do that. And you don't need to every additional, however many people you have introduces. And again, additional amount of coordination. nation overhead. And   
(00:59:28.552) ~~I would not,~~(00:59:29.092)  
if I was sitting in a startup today, I would be smiling with my grin, extremely wide, thinking about how I can go and compete against some of the large companies that are out there because there's just so much opportunity in the ecosystem.   
(00:59:40.358) ~~There's so much,~~(00:59:41.039)  
there's so much to be built. There's so many new things that were not possible before that are now possible with LLMs. 


---


#### 00:59:48.405

I think the important thing is, again, I think it's very possible that all the meeting notes takers are going to do really well. I think they're actually incredibly well positioned to become one of the first agents slash assistants to actually help you go and do work. They're in the meeting. They have the context. Having the context is half the battle.   
(01:00:03.592) ~~I'm not only in Google Meets for me now. I'm pretty much predominantly in Google Meets.~~(01:00:07.675)  
But I think there's a lot of people who are across many different platforms, across Teams and Zoom and Meet. other things and being able to have a tool that maybe does all those things is incredibly useful. So there's a lot of different edges. 


---


#### 01:00:17.713

And again, the value isn't in just doing integration and taking the notes, but like also in what you do after that and how much you can automate away.   
(01:00:25.021) ~~Like~~ (01:00:25.161)  
if for some reason I had a system that was able to draft up a bunch of emails after a meeting and say, here, let me go and ping these people for you. And I can just go and   
(01:00:33.367) ~~check,~~ (01:00:33.527)  
check and send those emails off. That's a distinctly different competitive advantage than what's being provided today. So there's always more that can be done. And   
(01:00:39.670) ~~I think~~(01:00:39.931)  
again, as I've said this many times in different places, but there's never been a better time to be a startup building in this space than right now. 


---


#### 01:00:46.215

Like this technology, like everything is up for grabs. Well, I think that's a great concluding note. You want to plug the podcast real quick or share anything else that we didn't get to before I give you the official send-off? Yeah, I think I'm on Twitter. Folks can get a hold of me there and see all the things that I'm thinking and sharing. And I'm appreciative of you having me on for a second time, Nathan. This was a ton of fun. Hopefully, I'll see you sooner than Google I-O next year. Looking forward to it. Logan Kilpatrick, thank you for being part of the Cognitive Revolution. I love it. Thanks for having me. 


---



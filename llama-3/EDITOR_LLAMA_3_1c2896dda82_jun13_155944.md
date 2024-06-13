#### 00:00:00.069

Alit Saab and Vivek Natarajan from Google DeepMind and Google Research, welcome back to the Cognitive Revolution.   
(00:00:06.213) ~~Thank you for having us.~~(00:00:07.033)  
Yeah, it's a real delight to be over here. I think there are very few podcasts that I listen to in the AI space, and I can positively say that you're the top two, Nathan. So yeah, real pleasure to be back over here.   
(00:00:16.760) ~~Thank you. That's kind of you to say.~~(00:00:18.161)  
  
(00:00:18.740) ~~And I don't know how you have time to listen to any AI podcast, given the incredible tear of first-party publications that you guys are involved with.~~(00:00:26.925)  
What we're going to do today is just pick up where we left off a handful of months ago, and that is there have been at least five notable publications that I've landed on that I want to walk through in terms of the results that you've delivered, specifically in the application of large language models and the fine tuning and adaptation of large language models to the medical domain. 


---


#### 00:00:50.347

I think people are still largely sleeping on what is out there in today's world. And so hopefully we can call them to attention on all the great work that you guys have been doing, get into a little bit of the techniques, and then for the second half, we can get a little bit more philosophical and figure out how and where these things should be used and where all this is going. How's that sound? Sounds perfect. Yeah. Cool. The five papers that I have queued up are one on radiology, one on diagnosis. Then you have the most famous one, which is the MedGemini, which is bringing the native multimodality to the medical domain. an immediate follow-on extension of that brings even more modalities to the Gemini or the MedGemini family of models. 


---


#### 00:01:36.027

And then one from just this week that is starting to look at the interweaving of chemical structure and notation in with natural language as well. And   
(00:01:46.215) ~~I think~~(00:01:46.456)  
that's a super fascinating extension of all this work. So we've got a lot to cover. The first one, and I think it's important to flag as we go, what the sort of base was on this, and we'll touch back on these different base models later when we get to the philosophical section. But let's start with the radiology paper. This one was based on Flamingo, which was funny for me to read because I hadn't thought about Flamingo in a while, though that was one early for me when I saw the results from the Flamingo paper. 


---


#### 00:02:15.263

I was like, okay, we're not just stopping at language. Basically, in that paper, you started to compare the ability of a fine-tuned vision language model to do radiology reports against what human radiologists can do. You want to summarize those results for us? Yeah, sure. So again, I think the common strand among all the work that we've been doing over here is we're building on the shorter of giants in this field. And   
(00:02:44.086) ~~I think~~(00:02:44.325)  
Flamingo is one of the OG multimodal models and papers. And it was probably one of the first to demonstrate few-shot capabilities in the multimodal domain, generalizing beyond language. And so this work has been, I would say, a couple of years in the making. 


---


#### 00:02:58.659

And radiology is one of those spaces where I think a lot of the medical AI research has been focused on for a long period of time. And I know that Dr. Jeff Fenton famously had this quote on AI replacing radiologists, which has turned out to be a little bit infamous right now, but I think he's not very far off. And   
(00:03:15.534) ~~I think~~(00:03:15.835)  
the results in the Flamingo paper,   
(00:03:17.195) ~~I think,~~(00:03:17.436)  
are for the first time showing that for the clinically relevant task of report generation and not just the classification of pathologies, we are starting to have models that are   
(00:03:28.502) ~~uh,~~ (00:03:28.542)  
approaching clinical utility and clinical applicability. So I think that was like a really cool result. 


---


#### 00:03:34.528

And obviously like the way we got over there was by taking, I would say a relatively modest and small visual vision language model compared to the sizes that we have today, but like bringing in a lot of high quality Again, a lot of it is not proprietary, but rather open source. Again, credit goes to folks who have been behind this MIMIC data repository who put together that, and so we utilize that one over there. When we combined a very strong multimodal few-shot learner and fine-tune that with high-quality radiological data, we start to see this very strong performance on radiology report generation and starts to approach that of what radiologists can do. So I think that was a very cool result. 


---


#### 00:04:13.097

I think it's one of the first papers to show that. And since then, there's been several other papers, including some of our own work that has shown more progress over there. But   
(00:04:19.879) ~~I think~~(00:04:20.038)  
the more interesting bit in that paper, at least, was the human-AI collaboration bit. Because we had an arm or a study over there where we showed that if we passed the AI reports to a human radiologist and they did edits, and when we look at the composite system results, those tend to be better than the AI alone or the human alone. And so that's the kind of interesting nugget. And this goes back to something that   
(00:04:44.766) ~~I think~~(00:04:45.026)  
Dr. Kurt Langlotz at Stanford, who heads up the AME group, he said that AI is not going to replace radiologists, but radiologists who use AI will replace radiologists who don't use AI. 


---


#### 00:04:56.291

And so this is one of those first results that shows what he was saying is maybe not really hallucinating, but rather he's speaking the truth. And so this is one of those first milestones towards that direction. And again, there's been a lot of other incredible work in this space. not just from our group, but from folks at MIT, Stanford, and beyond. But   
(00:05:11.398) ~~I think~~(00:05:11.577)  
those were the two key or interesting results over there in that paper. Yeah, it's striking to me that, first of all, that   
(00:05:18.461) ~~I think~~(00:05:18.641)  
it was April 2022 that Flamingo was first published. It's striking to me that is relevant even 18 months later. This paper, I believe, was either very late last year or January of this year, but more than 18 months from publication of one paper to the other. 


---


#### 00:05:33.627

That's a long shelf life for a foundation model these days. There's some interesting stuff in there too that, and I think we've covered in probably enough different episodes, including some of the past ones with you, where   
(00:05:44.351) ~~there are~~(00:05:44.932)  
If you're listening to this show, you're probably well familiar at this point with the distinction between the narrow classification models of put in an image and   
(00:05:54.031) ~~does it or~~(00:05:54.430)  
does it not have this particular condition. Whereas here, what we are getting out is a full natural language report of the sort that your radiologist would ultimately provide back to a patient and their general practitioner. And there's some interesting nuances there too around how data has to be manipulated and pre-processed. 


---


#### 00:06:14.401

You'll have, if you just train on sort of naive reports, you have a lot of references back to history, which may not always be available. And so you have to clean up that kind of stuff to teach the model exactly how you want it to behave, which is to reason just from this thing and not to infer or hallucinate previous medical history that it doesn't actually have access to. So some of those techniques I think are increasingly well-established. And then   
(00:06:39.379) ~~the question is kind of like,~~(00:06:40.459)  
first of all, the question of replacement of radiologists is an interesting one. I was just with my wife's cousin not long ago, who is a doctor and said that in the hospital where she works, 


---


#### 00:07:43.867

And then at the same time, I also do wonder. Spring 2022 model with fine tuning can get roughly on the level. I would say my summary, you can correct me if I'm wrong, but I would say my summary of this paper was that it was probably just short of the human clinician in terms of overall quality, like pushing it, but not quite there. But certainly one wonders if this will go the way of chess, where there was once this moment of time when the human plus AI was the best chess player. And as far as I understand it now, we've   
(00:08:15.444) ~~like,~~ (00:08:15.584)  
long since left that regime. So maybe we'll save the, you can opine on that now if anything comes to mind you want to say, but we could also batch some of these like projection questions for later. 


---


#### 00:08:27.197

But yeah, tell me if anything jumps to mind there that you want to add on. I think the only thing that I want to talk about right now is the question on data quality. It's one of those important things. The last time we two were talking on a podcast, we were talking about MedPalM and we used the same data sets, but we did not end up using the cleaned up version of the report generation data that we have, which did not have references to prior reports and things like that. And that cleaned up version was curated by Dr. Pranav Rajpokar and others at Harvard. And there's this notion that in some ways progress is happening in silos between academia and industry, but that's actually not quite true, right? 


---


#### 00:09:05.423

I think academia does a lot in terms of investing in data sets and curating and providing it. and also creating benchmarks and beyond. And   
(00:09:13.167) ~~I think~~(00:09:13.386)  
what we can do from an industry perspective is releasing our frameworks and sometimes open source models that academia can bring on. And so there's this already symbiotic relationship   
(00:09:22.351) ~~that is already, I think~~(00:09:23.392)  
that's been existent for a long period of time, but like people sometimes tend to miss that when you look at   
(00:09:28.554) ~~like~~ (00:09:28.674)  
the discourse on Twitter and things like that. And so that's maybe one of the things that I would stress on. And then   
(00:09:32.697) ~~like,~~ (00:09:32.817)  
again,   
(00:09:33.076) ~~like~~ (00:09:33.216)  
the importance of the right kind of data. And so we had missed that in the prior work on MedParmM, but then when we, used a highly well-curated cleaned up data set. 


---


#### 00:10:26.619

And there's this like general challenge now with generative AI on evaluation, right? So   
(00:10:33.003) ~~we're not like~~(00:10:33.682)  
we're not outputting a single label anymore. And so we can't use our favorite metrics like accuracy. So I think evaluation is a big challenge now. And one of the really cool things I thought about in the Flamingo CXR paper is that it really goes in depth with doing the gold standard when it comes to evaluation, which would be evaluating these model outputs with a panel of clinical experts. And that's what takes a lot longer, is doing those thorough evaluations. But they're necessary in this generative AI space. especially in the medical domain. In the medical domain, especially. Yeah, that's a huge theme. 


---


#### 00:11:15.639

And I think partly applicable to the next paper as well, which is known as Amy, the headline of this, and this is one that I've clipped one of the main figures from this paper and included in a number of presentations, slides, anywhere where I'm trying to alert people to the fact that there are big things happening in AI that they may not even have heard of. I pretty much always include the Amy result at this point, because, again, for those in the know, this is based on Palm 2. So we're still a generation behind the latest and greatest that's come out of Google. But it's funny, right? Because I always say, too, while it seems AI is moving so fast, it seems like it's old. 


---


#### 00:11:55.740

But at the same time, if you'd gone back to 2020 and dropped Palm 2 in, it would have been absolute revelatory, mind-blowing, even 2022 probably would have still felt that way. So Palm 2 is the base. And this one is, for me, just an incredibly compelling result, which is that, and there is one major caveat, which is that through a text-only chat-based interaction system, an AI doctor, if you will, the system, Amy, can diagnose through a differential diagnosis process more accurately than the human doctors did, human general practitioners, if I understand correctly. And I think that's evaluated probably in multiple ways, but essentially they come out ahead, the AI comes out ahead on all the dimensions, right? 


---


#### 00:12:45.846

It's evaluated as more accurate, the other doctors are giving it higher marks, and the patients are even giving it higher marks in terms of how it scores on empathy and making people feel heard and feel important. I can't get that one out of my head. What other aspects of that result would you highlight for people? Yeah, I think in many ways we were also surprised by the progress on that one. And I remember a bunch of us, after the MedPalm paper came out, we were thinking about this kind of a task or a setup. And we were just having a chat and we were like, OK, how long before we are able to crack diagnostic medical conversations? 


---


#### 00:13:20.889

So the AIME project had two papers that came out. One was the Diagnostic Medical Conversations paper. The other one was the New England Journal of medicine case challenges. So we were roughly having this discussion, how long would it take for us to solve them? I think everyone was unanimous that it will take at least two years. Then literally six months down the line, we had AI that was exceeding general practitioners on these case challenges, but also on diagnostic medical conversations. Maybe the first thing I would highlight is, this is a very different task in a couple of ways. So until this paper, we had a very well curated, vignettes that summarized very cleanly the clinical case descriptions and reports and things like that, and presented that to the model, and then you're asking it to do a diagnosis. 


---


#### 00:14:04.782

And while that's a challenging task, and has been a grand challenge in the field for decades, it's not reflective of everyday clinical practice,   
(00:14:12.005) ~~right?~~ (00:14:12.186)  
So when you go to a doctor, they'll first see you, they'll ask you about your symptoms, medical history and things like that. And then they'll embark on this investigative journey and then they'll ask you to maybe do a few laptos or give you some suggestions on interventions like medications or things like that. And then gradually come to a differential diagnosis and a treatment plan over a period of time. And so there is this decision making under uncertainty and like efficient acquisition of new information. And I would say it pretty much until this paper, 


---


#### 00:14:43.330

I haven't seen that in any field that we've shown that AI or LLMs are capable of doing that kind of work. And so this kind of behavior is very different from what you see even with general purpose LLMs out there today, like ChatGPT or Gemini, in the sense that when you have a conversation with them, ultimately at the end of the day, the way it's set up is for you to guide the conversation and be the driver of the conversation and the models out there to assist you. Whereas in a medical context, It's very different. The model has a task and a goal, for sure, which is to help you. But then the model has to drive the conversation and figure out the optimum plan in terms of asking the right sort of questions and helping you in your care journey, basically. 


---


#### 00:15:17.539

And so it's a very different task. It's a very different setup. And to me, at least, it was not clear and obvious that AI systems can be trained to do that. But it turns out we can, and I think the key reason behind that is the simulation learning environment that we set up over there for diagnostic dialogue learning. And   
(00:15:34.231) ~~I think~~(00:15:34.532)  
Khalid can talk a lot more about that. But it turns out when you do that with the progress in generative AI, you can actually set up self-play based systems that can learn over   
(00:15:43.975) ~~like~~ (00:15:44.115)  
several orders of magnitude more data than any human doctor can. possibly see, at least in the text realm and text domain. 


---


#### 00:15:51.136

And when you bring that power of simulation into the learning process, then you're starting to see some of this magic starting to happen over here in the learning process. And   
(00:15:59.438) ~~so that's, I guess,~~(00:16:00.918)  
the key thing. And again, I wouldn't want to overhype the results too much. And so the last bit I would state is, I think the comparisons are not totally fair. to human doctors because typically they are not used to text-based conversational interfaces. Rather, they are much used to doing it in person or video calls where you can use other cues to convey empathy and rapport and things like that. And then the second thing is, obviously, AI systems don't tire. So every interaction, they can bring their best possible cells, give you very detailed answers, and things like that. 


---


#### 00:16:33.119

Whereas it's very possible that some of the doctors that we were working with in the course of the study, they might be coming after a long day of clinical practice, and they would be perhaps a little bit tired. And it's those nuances that we also need to account for. But it is undeniable that significant progress has been made over here. And   
(00:16:48.461) ~~Karl, do you want to talk about the simulation learning environment? Yeah. Yeah.~~(00:16:52.482)  
Our goal here is to train an AI model to do diagnostic conversation. That requires the model to try and get the information needed, like what's the patient going through, their symptoms. Once it understands those symptoms, it asks follow-up questions on those. 


---


#### 00:17:12.173

And then the final goal is to come to an accurate and confident diagnosis, and perhaps even a treatment plan. And when you have this goal in mind, you want to train an AI model to do this, The first thing that came to our mind is, OK, the training data, right? Let's collect training data on actual doctors interacting with patients in the real world and then transcribing those and then training on those interactions. So we did that, but in the first version of AIMEE, we saw it wasn't having the high quality conversations that we were hoping for. And when we tried to dig into why that was, we saw that it's because the transcribed conversations from the real world interactions weren't high quality, because as we have conversations with each other, unless we're very well rehearsed, we're going to have some awkward pauses, utterances, might be pointing to something. 


---


#### 00:18:06.818

And so all those things add noise, and a lot of the information gets lost when we're transcribing those to text. We realized we had to come up with something where we curate our own training data. And we were very inspired by a lot of the works that show with these capable LLMs, you can actually curate high-quality synthetic data. And so that's where we came up with this multi-agent synthetic data framework. where we had one agent acting as the patient, and we would give that agent a patient profile. And then we'd have another agent acting as the doctor, and give that agent doctor-specific instructions. And then those two agents go back and forth in a dialogue. 


---


#### 00:18:51.198

And I want to highlight two things here. So with training data, quality is important, as we've been mentioning, but also coverage of medical conditions. So in a synthetic simulation environment, you can solve that with what we call the vignette generator. So a vignette is like the patient profile. It describes what the patient condition is, what the symptoms are, and maybe social history, medical history, family history, and all that information you'd need. And so we generate tens of thousands of these patient profiles using web search and other tools. So now that solves the coverage issue. So now we have tens of thousands of patient profiles. And now we do this back and forth between the patient agent and doctor agent. 


---


#### 00:19:40.207

But then to improve the quality, we also have this third agent called the critic. And so we give the critic instructions on what a really high quality dialogue is. And so the critic gives feedback on those synthetically generated conversations. And then we integrate that feedback to do another round of that back and forth generation of dialogues. And so that really helped us scale the data coverage and improve the conversational quality and allowed us to train Amy to see a lot more of these conversations. And I think that was one of the key drivers there. So just a couple questions on exactly how that works. Are you starting with the same base model for all of those different agents within the system. 


---


#### 00:20:26.365

They all start off as, in this case, Palm II with just different prompting. And then   
(00:20:32.612) ~~they,~~ (00:20:32.813)  
do they like diverge then over time? Are you fine tuning the patient agent model distinctly from the doctor agent model distinct from the critic? Yeah, so we start off with a base LLM. In this case, it was Palm II. And there's some prompt engineering here to make sure that the responses from the patient agent and the doctor agent are as we would expect. So we do some prompt engineering there. And I guess the more capable your LLM is, the less prompt engineering you probably have to do. I think it's still as possible to do this with some other LLMs, but maybe some more effort would have to go in there. 


---


#### 00:21:13.154

But the better instruction following your LLM is the kind of easier it is to set up these kinds of synthetic generation frameworks. But then to answer your question, we train Amy. So after we generate those synthetic dialogues, we train Amy for both the patient role and the doctor role. And so you can do this by having a different instruction prompt. You're the patient, and then you train on the patient turns. And then also have another instruction. You're the doctor now, and then train on the doctor turns. So this AIME model becomes better at both simulating the patient and simulating the doctor in this case. So then as AIME gets better at playing both roles, we then generate the synthetic data again. 


---


#### 00:22:00.105

And so that's what we call like the outer self-play loop, where we did this a few times and yeah, we're using the same model to do both roles. All three with the critic as well. Yeah. It sounds like it's remarkably not that much data and   
(00:22:18.912) ~~maybe I'm not sure how many rounds of fine tuning, but~~(00:22:21.573)  
again, this sort of foreshadows some of the more high level discussion I want to get into a little bit later, but tens of thousands of data points is obviously pretty minuscule in a world where three was trained on 15 trillion tokens, right? We're talking like a very small fraction of   
(00:22:39.362) ~~kind of~~(00:22:39.662)  
pre-training scale. And I don't know if you can share any data around   
(00:22:45.483) ~~like~~ (00:22:45.703)  
how many times you had to turn that crank and   
(00:22:49.365) ~~how,~~ (00:22:49.625)  
what the sort of filter percentage was. 


---


#### 00:22:51.866

If you had tens of thousands of cases, did you have to run a million conversations to get the next 10,000 best out of those or   
(00:22:59.892) ~~what the,~~(00:23:00.471)  
what does the enrichment   
(00:23:01.653) ~~kind of~~(00:23:01.893)  
process look like in a little more detail? I think would be of interest if you can share that. Yeah, so   
(00:23:07.295) ~~I think~~(00:23:07.474)  
the key thing is we are not training the model from scratch, right? So we are already building on top of Palm 2, which has seen roughly the same order of magnitude tokens that, say, Llama 3 or GPT-4 has seen. And so there is that base. And so you don't have to reinvent all that. over there. And   
(00:23:24.616) ~~I think~~(00:23:24.797)  
the second useful comparator is perhaps, okay, if you're trying to match and compare up with human doctors, like how many encounters do they have over the course of their career? 


---


#### 00:23:34.705

And if you were to do like back of the envelope estimates, that comes out to be roughly in the order of like tens of thousands. And so you can see that with AI systems, and Khaled mentioned tens of thousands of patient profiles, we can scale that up very easily with net new data. And so you can cover a wide range of disease presentations and symptoms,   
(00:23:52.692) ~~and not just that,~~(00:23:53.393)  
but also socioeconomic statuses, medication history, travel history, and things like that. And very quickly, when you do this combinatorial cross, you can have   
(00:24:00.358) ~~like millions,~~(00:24:01.019)  
hundreds of millions of patient profiles. And then maybe the other interesting bit over there is when you're doing the simulation, you can also simulate patient personalities. 


---


#### 00:24:08.746

And so you might have some patients who are very talkative, some patients who are very worried, some patients who are a little bit adversarial in nature. And a human doctor has to deal with all of them in a composed, rational manner. And we would expect the same with AI systems as well. So you can start simulating a lot of variety over here, and there's a diversity over there. And very quickly, when you do the math. And when you do the rollout of the conversations, that goes into the order of millions. And we haven't stopped since the paper, obviously, like the checkpoint was stopped at some point of time to do the study. But you can imagine the number of conversations that we have easily going into   
(00:24:42.349) ~~like~~ (00:24:42.490)  
the hundreds of millions of realms and even beyond. 


---


#### 00:24:45.165

But the key thing is every time you're generating data, that needs to add in net new information to the model that it had not previously seen before, otherwise it would end up saturating. And so the trick is how do you add that net new information so that the model is learning something new and reducing its overall uncertainty in terms of solving this task. So   
(00:25:02.597) ~~I think~~(00:25:02.778)  
that's the key bit over here. And specifically for this paper, I believe we had seven rounds of iteration of the outer self-play, and that's where we stopped. But again, the project has not stopped. We're just getting started. And so you can imagine a lot more work that's going on since that paper. 


---


#### 00:25:17.345

And this is now several months old now. Yeah. Okay. Two really interesting points there. One, I think seven is maybe the most I've seen. There's been obviously a bunch of papers that have demonstrated this self-improvement via critic dynamic. And I feel like they usually top out around five. So even to get to seven   
(00:25:35.643) ~~is,~~ (00:25:35.762)  
is going past what I've mostly seen. That's interesting. Another interesting question   
(00:25:42.146) ~~is like,~~(00:25:42.406)  
how do you think about. This is top of mind right now, because I just have been looking into this arc challenge. That's just been announced for these little like visual puzzles that today's language models can't do. And there's a big debate as to, is this something that. you have to have if you're going to qualify something as AGI, or is it not necessarily so important? 


---


#### 00:26:01.979

And I would also say, as a father of three young kids, that the idea that the kids have not seen something like this in the past is actually not true, because there's a lot of toys that look a lot like some of these puzzles, which shouldn't be neglected from the analysis.   
(00:26:17.974) ~~The –~~(00:26:18.315)  
anyway, that's a digression. But the key question I'm wondering about is the world changes, right? That was one of the big comments, something like COVID pops up. How do you think about incorporating new knowledge or new circumstances into something like this? Do you have to go back and rerun all the loops and fold it in from the beginning? Can you just add it into the eighth loop when a new disease pop or a new technique or whatever pops up onto the scene? 


---


#### 00:26:48.048

Facts in my experience, at least with   
(00:26:50.290) ~~like~~ (00:26:50.451)  
Laura, low rank type techniques have been really hard to get models to learn. Patterns of behavior seem to be a lot easier, but actual concrete facts, like I could not get a fine-tuned GPT-3 to know my name. It would   
(00:27:03.382) ~~like~~ (00:27:03.501)  
know that I was Nathan, would not know that I was Nathan Levens, even though I was trying to train it to write as me. I could not ever get   
(00:27:08.924) ~~that,~~ (00:27:09.105)  
that data, or at least in any reasonable timeframe, it couldn't get that fact, seemingly deeply learned. Okay. You've done all this, but   
(00:27:17.348) ~~some,~~ (00:27:17.529)  
something changes in the world. How do you respond to that in the context of this sort of system? 


---


#### 00:27:22.574

Yeah, I think there are multiple tools at our disposal over here. I think one of the key things with every round of self-play was the sampling of the patient vignettes that we had. It was not like from a fix, but rather we were also expanding that. And so in that sense, it was adding net new knowledge already, but we can do that in a more principled way. And for example, if say a new COVID variant, hopefully no, but if that pops up, then we can start doing that and we can add it to the fine-tuning mixture and hopefully that can be learned well by the model already. But then   
(00:27:54.075) ~~I think~~(00:27:54.234)  
this is a nice segue into our latest work on MedGemini where we are now starting to give these models access to tools such as web search which can real-time retrieve information. 


---


#### 00:29:15.500

Yeah. Maybe the last thing, and I think it's perhaps the most important in the medical context, is this notion of scalable oversight that we are building towards. That requires models to have better inherent uncertainty estimates. So that means more reliable behavior such as when a model doesn't know about something, then it needs to be able to communicate that back to the patient itself but also maybe back off and ask help from experts in the loop. So that's the other kind of behavior that we are building towards over here. So that will hopefully enable more scalable oversight of these powerful systems and allow us to safely deploy them in the real world. So that's one bit that we haven't yet spoken about completely yet because we still need to do some studies, but I think that's the other missing piece of this puzzle over here. 


---


#### 00:30:00.563

Gotcha. Okay. So with MedGemini, the part of that sort of previews what you're describing there is the uncertainty guided search. And   
(00:30:12.167) ~~I guess~~(00:30:12.348)  
maybe just take even one step back and try to summarize MedGemini. It's a hard to summarize paper because It is a family of models, first of all, that you're reporting on there, with multiple different base models. You can maybe give a little insight into why some of them are based on Gemini 1 and others are based on 1.5. I think there's even a Flamingo 1 maybe still that is part of that mix. And it's also, it's not a, if one were telling a naive story of, okay, here's Amy, this thing can have a chat interaction and it can do diagnosis. 


---


#### 00:30:45.182

What comes next now that there's Gemini and it's multimodal, you would think, geez, probably like a chat with video chat or a chat with the ability to put in images. But I would have guessed that the next step would still be this sort of like holistic patient doctor interaction. And that's not really what this paper. was about so much. It's much more like a lot of different models very narrowly scoped and dialed into very particular tasks.   
(00:31:14.172) ~~I think it's,~~(00:31:14.491)  
I forget how many tasks, but it's a lot of different tasks, a lot of different state-of-the-art results, a lot of different modalities, whether it's pathology, imagery, or scans of various types, or even some genetic kind of information. 


---


#### 00:31:27.135

And then with the extension also, you've got 2D and even 3D scans. So just a ton of different stuff. I guess maybe why the Swiss army knife approach there is one thing, and then we can get back into a little bit more of the uncertainty guided search. Yeah, again, great questions. So I think a good way to think about MedGemini is it's like the analog to the MedPalm paper, but with obviously a much more capable base model over here. And so if I were to   
(00:31:55.239) ~~like~~ (00:31:55.358)  
summarize, okay, what is the key takeaway over here? I think for me, it is the fact that now we have native multimodal understanding over millions of tokens and million plus context windows. 


---


#### 00:32:05.305

And that seems like a very big advance. And so in some ways with MedPalm, the key thing that we relied on over there in in order to capture the imagination of the public and show how much progress we've made was the USMD analog. I think with MedGem and I, maybe it was a little bit difficult for us to say, okay, this is this one thing that it enables.   
(00:32:23.794) ~~And~~ (00:32:23.973)  
because when you have multimodality over millions plus context windows, a lot of new things now become possible. And so that's why maybe there's not just this one thing that you can say, oh, this is the one thing that's happening. But rather, it's like a huge array of possibilities that now suddenly becomes feasible and possible. 


---


#### 00:32:42.580

And so maybe that's the takeaway for me. It's hard to distill and say, oh yeah, this is only this one thing. But rather, it's like a platform. It enables a lot more new things over here. And coming back to the specifics, why do we not have a journalist model anymore?   
(00:32:56.205) ~~I think~~(00:32:56.365)  
it's also a little bit of an evolution of our own research theories and which way we want to build towards. And so   
(00:33:03.169) ~~I think~~(00:33:03.828)  
this time last year, we had not yet demonstrated the idea of the generalist model in medicine. There were a few examples of that in robotics and maybe in a few other domains, but that still felt like something that no one had demonstrated yet. 


---


#### 00:33:16.498

And so it was interesting to do that, and we did that with Matt Palmer, and we showed the capabilities. But then over the course of last year, when we were trying to think about, okay, how do we deploy this in the real world and enable people to make use of them? we realized that there's a lot of trade-offs that you need to make over there.   
(00:33:31.732) ~~Trade-offs in terms of~~(00:33:32.792)  
the kind of data that is brought into the mix, what tasks you're optimizing for, what is the latency and throughput requirements, and that in turn ties back to the size of the models that you're serving. And so it felt like this   
(00:33:43.957) ~~generalist notion or~~(00:33:44.836)  
this generalist approach where you're trying to cram everything into one model, which in turn invariably means like largish models in nature. 


---


#### 00:33:51.980

Sometimes the cost is not worth it for specific applications. And so what may be like specific applications or demand is like trade-offs. And so you need to be able to provide a menu of options over here. And so that is where we stepped back from this notion of building one journalist model. to do everything over here, because it felt like from a research perspective that we showed that challenge is no longer out there, but that it's possible to solve. But from an application and real-world deployment perspective, what is really needed is an array of specialist models and develop with different constraints in mind so that we can easily deploy. And so that's a goal over here. 


---


#### 00:34:25.677

And so some applications might demand not a lot of reasoning capabilities, not a lot of multimodal capabilities, but rather very low latency and high throughput, and for that we have the smaller size models. Then some would demand advanced clinical reasoning, million plus context windows, and   
(00:34:39.057) ~~so on and so forth.~~(00:34:39.677)  
So for them, we have many options as well that will cater to that, and that's a reason over here. Yeah. I agree with everything Vivek said. I'll think about the MedGemini paper as our first exploration to seeing how well Gemini can do in the medical field and how should we start thinking about specializing Gemini to the medical field. And   
(00:35:03.438) ~~so,~~ (00:35:03.737)  
in this first exploration, we definitely wanted to look into textual reasoning, like what MedPOM and MedPOM2 did, and then also advancing the techniques over there, and that's where the web search and agentic framework came in. 


---


#### 00:35:18.291

But then also because GemIIni is a multi-modal first language model, we wanted to look into how do we specialize it for things like medical images. But then what was really interesting is during this exploration, we had this breakthrough in GemIIni of having the one million and now two million context length. And so we also wanted to start thinking about, okay, how can we start exploring how to leverage that for the medical domain? So Gemini has all these amazing things. We have all these ideas on how we should specialize it to the medical domain. First,   
(00:35:52.014) ~~like~~ (00:35:52.193)  
what works best,   
(00:35:53.673) ~~right?~~ (00:35:53.934)  
And how well does it do? And so let's first report on a broad range of benchmarks. 


---


#### 00:36:00.655

And that's what that paper mainly focused on. And then we showcase some of the qualitative aspects, like having multimodal conversations, which is also a very important part because   
(00:36:11.559) ~~You know,~~(00:36:11.780)  
just having a few tasks, like just one question and one answer, is very helpful, but the ability to interact and have follow-up conversations is what really, I believe, has some clinical translation to the real world and utility. So we showcase some of those qualitative things, and then with the long context, We were looking at new tasks, like if you have multiple EHR logs and visits something that's extremely long that couldn't fit into the context window previously, how well would MedGemini do in processing that and being able to look up specific conditions or details in that history of the patient? 


---


#### 00:36:54.088

And then also things like surgical video and having conversations with a surgical video and then having, asking questions across 12 different genetic papers. And it was just like, look at all these things that GemIIni could do. And   
(00:37:06.157) ~~like,~~ (00:37:06.416)  
these are the techniques that worked really well for specializing GemIIni. But then again, you're also hitting at the point of like, why not like an Amy-based style paper? And that's definitely something that we're thinking very hard about. It's just that requires more rigorous evaluations with clinical experts and takes a bit longer. And that's why the first paper was more benchmarks, qualitative examples, and we're working hard on the more rigorous evaluations with clinical experts. Yeah. And maybe just to add on to that, 


---


#### 00:37:37.862

I think we're at the stage right now where maybe our evaluation setups and benchmarks are no longer perhaps keeping up with capabilities advancements. And doing that in a rigorous manner takes time. And so we still have to rely on imperfect measures like existing benchmarks, but that clearly don't capture the set of capabilities. And sometimes you say, Oh, look at this on this benchmark, say on MML, you just got 0.6% improvements, but that's   
(00:38:01.936) ~~like~~ (00:38:02.056)  
just one tiny fraction of the capabilities of the entire system. And how do we showcase that? So that's an open challenge for us as well. We've resorted to doing a mix of quantitative evaluation on benchmarks plus like qualitative demonstrations. But clearly, 


---


#### 00:38:14.757

I think we need better measures of progress over here than what we have right now, which is largely static benchmarks driven at this point of time. And that's true,   
(00:38:22.284) ~~I think,~~(00:38:22.443)  
overall for the field, but definitely for progress in the medical domain. Yeah, that makes sense. So   
(00:38:27.103) ~~I think~~(00:38:27.443)  
one takeaway from that is we can stay tuned for future work that might start to consolidate   
(00:38:33.630) ~~this.~~ (00:38:33.809)  
This is the proliferation phase of look at all the many different things we tried and we can expect a consolidation or maybe integration is probably a better word phase   
(00:38:42.958) ~~to,~~ (00:38:43.159)  
to follow that in the not too distant future.   
(00:38:46.021) ~~I guess that's a,~~(00:38:46.581)  
maybe that's what we should expect in general is TikTok like new fundamental or new level of scale or new foundation model or whatever kind of comes out. 


---


#### 00:38:56.858

Now it's, hey, we got to go broad and just try this thing on 50 different things, see in a very broad way, can we characterize it? And then we can bring all that into some form factor that would actually be intuitively usable for whether it's a doctor in the field or even a patient or whatever. And that does make a lot of sense. And   
(00:39:19.469) ~~I think~~(00:39:19.648)  
also certainly the doctors will probably want to see that sort of detailed breakdown as prior work or qualifying work before they would be ready to trust such a system. One thing that you had said that caught my ear a little bit was cost. And you had said for some things it might be too expensive or whatever. 


---


#### 00:39:39.219

I am of the opinion, and I would even say this outside of medicine, that people are overly worried about the price of their AI products today. I hear this fairly often from people that are building   
(00:39:51.646) ~~like~~ (00:39:51.867)  
general purpose, like AI assistant type products. And I'll say, why aren't you using just   
(00:39:57.150) ~~like~~ (00:39:57.271)  
the very best model available and just,   
(00:39:59.672) ~~you know,~~(00:39:59.893)  
stuffing whatever context in there   
(00:40:01.893) ~~that you can,~~(00:40:02.434)  
that you need to make it work. And sometimes they'll say, well, It's too expensive that,   
(00:40:07.177) ~~you know,~~(00:40:07.336)  
it would be the product would have to be $500 a month or whatever. And I say to that, give me something that works and I'll pay the $500 a month. 


---


#### 00:40:15.878

It's, it's still probably often like order of magnitude cheaper than what it's replacing, even if it were $500 a month or whatever. And on top of that, obviously we have these like dramatic price drop trends that show no signs of stopping.   
(00:40:29.661) ~~Like~~ (00:40:29.782)  
Gemini Pro 1.5 is $7 per million input tokens.   
(00:40:35.682) ~~Uh,~~ (00:40:35.762)  
so it seems like the cost is   
(00:40:37.463) ~~like~~ (00:40:37.583)  
ultimately not going to be that much of an issue, but maybe I'm missing something. How are, how are you thinking about   
(00:40:43.286) ~~the,~~ (00:40:43.567)  
the cost? What is the barrier there or   
(00:40:46.608) ~~where do you, what is the~~(00:40:48.469)  
current concern and where do you see that going? Yeah, I think the trends are overall in the right direction. As you say,   
(00:40:54.092) ~~um,~~ (00:40:54.492)  



---


#### 00:40:54.612

I think the cost per token is going down dramatically and it's probably going to continue that as we do more of this harvest of integration over here across the entire stack. And   
(00:41:04.728) ~~I think,~~(00:41:05.407)  
yeah, 1.5 Pro is great, but Flash is I think hitting the sweet spot in terms of capabilities was a surprising trade off.   
(00:41:12.369) ~~And,~~ (00:41:12.550)  
and you can go even further lower for on-device stuff like the nano models. And so   
(00:41:17.150) ~~I think~~(00:41:17.331)  
all that's great, but maybe the one key thing is   
(00:41:19.471) ~~like,~~ (00:41:19.650)  
at least at Google, and this is something I got used to it over a period of time by being over here. The tendency is to not just aim for the top 1% of the population, but rather think about at a billion user scale. and at a global scale, right? 


---


#### 00:41:34.505

And for a large part of the world,   
(00:41:37.909) ~~I mean,~~(00:41:38.130)  
in addition to,   
(00:41:39.751) ~~I guess,~~(00:41:40.192)  
the high amount of utility that you get from different kinds of Google services, it is attractive that these services are, at the end of the day, free to access. And so there may not be,   
(00:41:50.601) ~~like,~~ (00:41:50.802)  
$500 per year would seem not so high for Yumi and Khaled over here, we're very fortunate to be in California, probably the best place in the world to be in, at least as far as AI goes. But for large parts of the world, in India and Africa, that's a no-go, simply. So how do we bring these technologies sustainably out there in the real world in a very affordable manner? 


---


#### 00:42:10.405

And I think that requires us to go down even further below. Because one thing that we can end up doing over here is we can build up technologies, but then the pricing is so terrible that it becomes a barrier for 99% of the people to access. And that's completely the non-goal over here.   
(00:42:23.193) ~~Like,~~ (00:42:23.414)  
I think what we really want to do at the end of the day is to leverage the advancements in technologies to not amplify existing disparities in care. but rather   
(00:42:31.762) ~~like~~ (00:42:31.882)  
really enable   
(00:42:32.762) ~~like~~ (00:42:32.943)  
people at planetary scale to have access to the best possible healthcare possible. And that requires us to continue pushing the boundaries over here in terms of cost and access and things like that. 


---


#### 00:42:44.436

And again, I would just caveat that we're still very early over here. I think we'll make fundamental technological advancements a lot more before say overcoming challenges on the regulatory side to deploy these things. And also in general, generally speaking, the societal acceptance of such technologies. But I think it's important to not accept the status quo. I think we can do a lot better and we will do a lot better over here. Yeah, and especially if we think about our text-based systems,   
(00:43:08.581) ~~I guess~~(00:43:08.820)  
the cost is definitely would change depending on if we're having conversation with text versus conversation with a video or audio, and that would drive the cost up. And just with text alone, 


---


#### 00:43:21.429

I think we, as we show in Amy, you can do so much. And I've had   
(00:43:26.413) ~~the,~~ (00:43:26.672)  
I've been lucky to be able to interact with Amy and it's a really amazing experience with the way it follows up and asks you questions if you're having some kind of worry or condition you're not too certain about. I think that the comparison here to make is chatting with something like Amy versus doing your own research or talking with a clinical expert. And that cost alone,   
(00:43:50.911) ~~like~~ (00:43:51.050)  
with the tech space, is already dramatically less. I'm just excited to try and democratize it. Yeah, I certainly share that vision and the excitement for the broad accessibility of this technology. It literally is my first go-to answer whenever anybody's just broadly skeptical of what's going on in AI. 


---


#### 00:44:12.219

Like, what are we going to do? Just put all of ourselves out of work or whatever? And I'm like, hey. AI doctor. Let's start with that.   
(00:44:18.181) ~~We,~~ (00:44:18.362)  
a lot of people can't see one, have to take off work, travel a long way, make real sacrifices. If they can do it at all, this could be a total game changer for a lot of people. So I certainly share that.   
(00:44:30.068) ~~I guess~~(00:44:30.289)  
I'm just wondering about the path.   
(00:44:31.889) ~~I mean, and I'll maybe ask a, ask it from the other end. The first, if the~~(00:44:35.931)  
first question is like, why not pursue the Tesla strategy of. Cause it does seem like there's something weird too, with all these systems where self-driving cars are probably. the number one example in my mind, but AI doctor probably not too far behind, where it's not enough for it to be similarly effective or even a bit better than the human provided service. 


---


#### 00:45:01.010

It has to be like 10 times safer, it seems like for self-driving cars in order for them to be like accepted. And we might even be closing in on that or soon to be, but until it gets to the point where it's like totally undeniable, people are just not quite ready to embrace the technology. The Tesla strategy,   
(00:45:19.873) ~~just, I think people know what that is, but~~(00:45:21.213)  
that's just make an expensive version first and use that to subsidize the kind of development of bringing the cost down. Google has enough resources that maybe it doesn't even need to go that route. Asking a   
(00:45:32.146) ~~sort of~~(00:45:32.367)  
similar provocative question, similarly provocative question from the other end, I feel like a lot of people around the world literally can't do better than Amy today. 


---


#### 00:45:44.215

And so I wonder at what point does it become like almost a societal or global obligation to actually deploy the technology even if it isn't 10 times better than the best doctor? I think we suffer a lot of times from weirdness in our comparison. This isn't necessarily as good as the care that I might get at Stanford Medical Center. Therefore, it's not fit for anyone. When in reality, it's   
(00:46:09.324) ~~like,~~ (00:46:09.545)  
that is not scaling. This could scale. And I feel like a lot of people around the world would be very grateful to have it. I'm sure that's something you guys talk about internally. At what point does this hit a point where it almost becomes like, a moral requirement that we put it out into the world. 


---


#### 00:46:28.797

Where do you think we are on that? Because at some point we're getting there, right?   
(00:46:33.172) ~~Like~~ (00:46:33.331)  
it seems like I cannot imagine a,   
(00:46:37.193) ~~I don't even, I don't know,~~(00:46:39.393)  
2027. I can't imagine a 2027 where you guys continue down this path and we don't have something that would be like almost a moral imperative to deploy. How close do you think we are to that? And how do you think you approach it as you hit that threshold? Before you answer, I wanted to share something. When I first joined Google last year, I remember we were in a summit and I asked this, I just raised my hand. I'm like, these LLM services are free. People are using them. 


---


#### 00:47:08.820

Why can't we just have the same thing, but for these AI doctor type models? And I guess I learned a lot from that answer, but I was also thinking the same space, but the medical space just has so many subtleties when it comes to FDA regulations and the way you need to evaluate things. But I just wanted to point out that I was also thinking that too. I just wish it was that simple. Yeah, honestly, I would say it's probably the single biggest question or dilemma that keeps me up at night these days. We are in a very privileged position that we can build out such powerful and capable technologies that can have such societal level impact. 


---


#### 00:47:48.905

But the key thing is to do that in a safe and responsible manner as well. And   
(00:47:54.351) ~~I think~~(00:47:55.092)  
one of the challenges is being able to communicate progress, but do that in a responsible manner. And so a lot of the progress that we've been communicating have been capabilities advancements over here. And we've tried to make sure that when we put out our papers or whatever products, we add the necessary disclaimers over here that like capability does not mean reliability in the field, right? And there needs to be more evidence that we need to accrue to show that actually these things are really better than the standard of care. And that requires us to do control studies by integrating them into real-world clinical workflows and putting them as interventions in people's care journeys. 


---


#### 00:48:34.088

And we are definitely doing that, and we hope to announce something very soon, like the kind of work that we're doing in this space. But as a matter of fact, as things stand today, we don't have enough data to say that these things are meaningfully improving the standard of care. Yes, every now and then on Twitter, there's a post that goes viral saying, oh, I use ChargeGBT to diagnose my condition, and this is much better than doctors. But how much can you rely on anecdotes? Would regulatory agencies be convinced on that? I don't think so. I think you need to be more rigorous. And there is a well-defined process of doing that. And   
(00:49:02.496) ~~I think~~(00:49:02.876)  
in some ways, the way you develop and bring forth these technologies into the real world is not too different from how we bring drugs into the market, for example. 


---


#### 00:49:11.960

And there's a well-established process where you first evaluate things in simulation, which is in vitro in the lab settings. And then if things look promising, you progressively step through different phases of clinical trials. And then you finally bring it into the market. And obviously, it's a very painful process. It takes years, costs a lot of money. But there's a reason for things being set up that way, and that is primarily to ensure the safety and well-being of the patient at the end of the day. And so in many ways, we are embarking on a similar journey. And so with, for example, the AME papers, we showed it in simulation with patient actors, not real patients themselves, that this thing works. 


---


#### 00:49:46.891

And so now the next step for us is to do the actual clinical trials kind of thing, put them into real-world clinical workflows, put them as interventions into patient's care journeys and get the data readouts. And if that looks promising, and the first thing over there perhaps to check is not even the efficacy of the system, but rather the safety of the system. And once we are confident about that, then we can gradually step up the kind of capabilities that we expose and take them through these different phases. And I hope it doesn't take us 10 years, but rather it takes us much smaller than that, the amount of time over here. But once we do that, 


---


#### 00:50:19.103

I think then we will have enough rigorous data to say that, yes, this thing now can be safely deployed in the real world. Because the other thing that I would really personally hate is, I come from parts of the world where we don't generally have access to the best resources, and we're almost always further behind. But I don't think it's also ethically the right thing to do to take unproven technologies and untested technologies and dump them in those parts of the world. So I think it's very important to test the safety and efficacy of these systems. But turns out the challenges to test the safety of these systems, you need oversight. And oversight necessarily means availability of doctor resources to immediately step in when something goes wrong. 


---


#### 00:50:56.454

And so imagine, if you have an interaction with a patient, like Amy having an interaction with a patient and maybe it says something that's incorrect, there is a liability over there. And so the only way to ensure patient safety is a doctor overseeing that entire conversation and immediately stepping in with a phone call or something like that. and saying, oh, this thing has gone wrong. This is not the right thing to do. Because otherwise, it can even have life and death consequences. And so that's a challenge. And so even testing the safety of the system requires resources, medical resources. And I think as things stand today, those kind of resources are available only in the Western world. 


---


#### 00:51:30.190

And so that's why we are partnering up with well-resourced category organizations to be able to test the safety of the system first. And then once we have promising data readouts, then we can step up through the process over here. But   
(00:51:40.541) ~~I guess~~(00:51:40.760)  
the key thing in health care overall is,   
(00:51:42.061) ~~I guess~~(00:51:42.762)  
there are two things. One is there are clearly no shortcuts.   
(00:51:45.425) ~~I think~~(00:51:45.625)  
if we end up taking shortcuts, then we are going to set the field back by several decades. So it's important to do things the right way. And then the second thing is everything in health care moves at the speed of trust. And so the more trust we can build up in the system with all these different stakeholders, whether that's the patients themselves or the doctors, and also folks like in the regulatory agencies, 


---


#### 00:52:02.876

I think the better it is. And it may be a little bit counterintuitive, but I think doing things the right way will accelerate and get us sooner to the future that I think we all envision over here, not by taking shortcuts. Yeah, it's funny.   
(00:52:14.974) ~~I mean,~~(00:52:15.295)  
I'm of such mixed,   
(00:52:17.516) ~~I feel like AI scrambles so many, you know,~~(00:52:21.117)  
so many different debates and even my own perspective, I feel is weirdly scrambled. It's   
(00:52:26.460) ~~like,~~ (00:52:26.621)  
I feel alien to myself sometimes when I think about how I mostly, for most of my life, I've thought about technology and regulation versus how I think about it now. And I do feel, I find myself in this weird place where I'm like, 


---


#### 00:52:41.467

I actually am afraid of just full pedal to the metal AI scaling, let's make the very most powerful systems that we can. And on the other hand, I'm like, But I do want my AI doctor sooner rather than later, even if it's only on par with the human equivalent or only slightly better. It does feel like waiting until it's that 10x better leaves a lot on the table, but that might just be the only way to achieve the trust that you talked about. And that is a great soundbite. I think we'll clip   
(00:53:14.155) ~~that,~~ (00:53:14.376)  
that things move at the speed of trust in medicine is definitely an important insight for technology people to keep in mind. 


---


#### 00:53:23.679

Yeah, please. Yeah, maybe one quick thing I'll also add in is the other thing that's also not very obvious to me yet is societal acceptance of such technologies like this quote-unquote AI doctor. It's very obvious that as we keep progressing in capabilities, we'll have superhuman AI diagnosticians But the key question to ask is, do people really want that? And to me, as things stand today, and beyond the Twitter bubble that we live in, the answer to that is maybe not obvious to me. Because for most general people's interactions with AI systems, it's actually quite terrible. I was talking to my mom the other day, and she doesn't use chat GPT that regularly. And the only places that she has encountered AI are every time she's trying to call up an airline or a travel agency, and there's a weird AI wall that prevents her from getting to. the human and getting things done. 


---


#### 00:54:16.822

And so for many people like that, the experience with AI, and a lot of it is AI from the previous generation, and even things like Alexa or Google Home, they're not the best. And so the expectations that people have from AI are maybe quite low at this point of time, and the trust they have in AI systems is also quite low. And that's primarily because, again, in San Francisco, in Silicon Valley, and maybe in the Twitter bubble, again, that we live in, Technology tends to diffuse very quickly, but then in the real world to diffuse at scale, at billion-user scale, it takes a long time. It takes decades. And I would not be surprised that it might only be like one-tenth of the population that has seen a GPT-4 or a Gemini yet, and we're still so far away from real diffusion and adoption of this technology at scale. 


---


#### 00:54:59.119

And so that's the other key thing. For such a technology to be really useful and helpful, it requires that adoption at scale. And we are nowhere there yet in terms of like societal acceptance of such technologies. Yeah, that definitely is going to take time. I have similar conversations with my parents as well, not infrequently. And it is striking. A lot of times they'll be like, Oh, I tried. My mom is Gemini advanced or Google one subscriber or whatever. And she said, Oh, I tried asking Gemini to plan me a trip and it didn't do very well. And I was like, Oh, Yeah, you probably, they've got something coming for that for one thing, but also you might want to go to a specialist thing and it needs to tie into APIs. 


---


#### 00:55:37.440

And so there are a lot of things where even just to select the right tool in today's world is not easy. I just want to go quickly through a couple final things here and then get back to this question of like, where are we going hyperscaling versus domain specialization? I think that might be   
(00:55:56.867) ~~like~~ (00:55:57.009)  
the most important question for the big picture over the next couple of years. I guess just briefly on the uncertainty guided search, cause we had teased that up and hadn't closed the loop on it. That would seem to be, first of all, if I understand it correctly, it's basically just like you run the generation multiple times, see if you're getting a consistent answer. 


---


#### 00:56:17.858

I don't know if you're looking more deeply at like, perplexity scores or something like that, but basically saying, do we appear to be confident here in what we're saying? Or do we have enough uncertainty that we need to go acquire more information? That would seem to be also a basis for a flag up to a human oversight, or even just a disclosure to the user that this is off the happy path here. Any more that you would want to highlight on the uncertainty guided search? Yeah. So I think two things that we realized we had to get right for this to work, because if you just use web search, where you just tell Matt Gemini for each question, generate some search queries that will help you solve the question. 


---


#### 00:57:07.130

And then you go and you fetch those search results and then add it to the input. Then in fact, sometimes you might confuse the model because   
(00:57:14.653) ~~you're,~~ (00:57:14.873)  
you might be getting some irrelevant facts or the more information you're giving the model, the more possibilities of something going wrong or it latching onto something that's incorrect. And in order to really get that right, there are two parts there. One was generating the search queries, and then two is how do you integrate the search results. And so in order to generate the search queries, we realized we had to do it in a way that was very specific to what the model was confused about, not just about the general question itself. 


---


#### 00:57:47.708

So the way we did that was by telling my Gemini to generate search queries by looking at conflicting responses. So as you were saying, we generate multiple responses. And then when we had a lot of conflicts or disagreements among the responses, we would get those conflicting responses and then from the conflicting responses generate search queries. So the search queries are targeting what the model is specifically confused about. So that was the first part. And the second part with how to integrate the search results, that's where we saw the self-training helping where in the training part of that algorithm, we train with search results in the context so that MedGemini was used to seeing search results and In the training, 


---


#### 00:58:38.657

Matt Gem and I would know what the right answer is. So it also learns how to just extract specific parts of the search results and not over rely on them. Those two,   
(00:58:48.958) ~~I think~~(00:58:49.318)  
were the key ingredients to getting it to work well. Yeah. Those are good tips. That makes sense as to why it wouldn't just be a token level perplexity indicator, but like an actual contrast of full responses. So that's interesting. Yeah, maybe one thing. It was,   
(00:59:07.454) ~~I think,~~(00:59:07.833)  
an incredible amount of work. And   
(00:59:09.375) ~~I think~~(00:59:09.715)  
Khaled and Tao,   
(00:59:11.016) ~~I think~~(00:59:11.195)  
Khaled's wife, Kirsten, has a video of the amount of effort that Khaled put in over   
(00:59:15.117) ~~like~~ (00:59:15.237)  
a three-month window. He's coding up at gas stations and things like that. 


---


#### 00:59:18.960

But yeah, in some ways, I think the work that we did over there was maybe not the most optimal, I would say. Ideally, we wouldn't have to regenerate every single time. and we would rather have the model produce its own verbalized uncertainty estimates. And so we're moving towards that. And then the other thing is, again, it's like the baby steps of an agent framework that is being put over here. Search is one of the tools that the model will have in its arsenal, but it'll have a lot more, including the ability to talk to maybe more specialized systems.   
(00:59:42.331) ~~And so~~(00:59:42.590)  
But that's where we are building to it. So there are hints and clues of what we are doing over there. 


---


#### 00:59:46.432

But I guess for this specific paper, a lot of it was optimized towards doing well on the benchmarks. And so that's why we have that specific instantiation of the technique and the approach over there. Gotcha. Cool. Yeah, makes sense. How are you doing on time?   
(01:00:02.043) ~~Do you have a hard stop in 10 minutes? Or can we run a little long? I think for us, it's only this room. So we probably have this room for longer.~~(01:00:10.869)  
So yeah, we can go ahead. Okay, cool. I won't keep it too long, but if we have a few extra minutes, then I'll take an extra beat on just all these different modalities. I think this is something that feels   
(01:00:22.889) ~~to me~~(01:00:23.170)  
to be... much underappreciated when people talk about, are we going to run out of data? 


---


#### 01:00:28.969

For one thing is obviously the big topic recently, and that tends to focus attention on high quality text data. But then I'm always like, man, there's a lot of other modalities out there. And a lot of that stuff is just massive deposits of data that have not been tapped into when you think of all the x-rays and the MRIs and the pathology tissue imagery and even just the chemical information itself.   
(01:01:01.010) ~~final paper that we had, I guess the last two,~~(01:01:03.432)  
one is an extension of MedGemini getting into even more modalities. I'll just read a quick quote from that one because I've got a couple of notable things. Chest X-ray report generation across two separate datasets by an absolute margin of 1 in 12%, where 57% and 96% of AI reports on normal cases and 43 and 65% on abnormal cases are evaluated as equivalent or better than the original radiologists reports. 


---


#### 01:01:31.009

So basically with this one, with these 2D chest x-ray type things, we do seem to be hitting the point of basically clinical utility, right? It's hard to read that another way. And then there was another quote that I pulled out This is the first ever large multimodal model-based report generation for 3D computed tomography, aka CT scans, with 53% of AI reports considered to be clinically acceptable. So those are pretty notable results. And   
(01:02:00.443) ~~I,~~ (01:02:00.463)  
again, just think, man, as we start to integrate these other modalities of data into potentially even the pre-training mix. If I understand correctly, all this stuff is done in kind of a post-training scale, such that the models have seen whatever they saw on the internet, but they weren't really concentrating on CT scans, for example, in pre-training. 


---


#### 01:02:22.148

You're bringing a relatively modest dataset to this, creating these distinct encoders, basically creating a framework to add all these different new modalities in. after the bulk of training is done, do you think that it continues to be that way? Or do you think that where we're going is more like CT scans and all this stuff just get dumped into the pre-training mix and it all is just native at some point in the future?   
(01:02:47.601) ~~Like~~ (01:02:47.721)  
natively multimodal means like literally all the modalities in say a year or two. Yeah, I think it's an open question for me. The part I would like to see is again, like more generalized encoders. So I wouldn't want to see hundreds of 2D encoders and hundreds of 3D encoders, but rather I would want any 2D modality to be processed by one single encoder, regardless of whether that's a natural image or a medical image. 


---


#### 01:03:11.764

And same with 3D, right? I would hope that we have encoders that are able to process videos and 3D medical images equally well. But as things stand today, that is not the case. You do get quite a bit of boost when you have specialized encoders. And   
(01:03:24.432) ~~I think~~(01:03:24.672)  
that's where maybe also the question or the challenge of whether you throw that into the pre-training mix or whether you do adaptations or post-training also comes in. So if we have generalized encoders that are shown to work well across different types of data modalities, then I can imagine a lot of this data starting to be mixed up with the pre-training mixtures. And then you don't have to maybe do a lot of the specialization or the adapters or the post-training work that you do. 


---


#### 01:03:50.099

But if we don't get there, then maybe the specialization route would hold on for a little bit longer. So   
(01:03:58.088) ~~I think~~(01:03:58.268)  
that's the interesting question that needs to be answered in the next few months. So can you, for example, train   
(01:04:02.192) ~~like~~ (01:04:02.311)  
a 3D encoder that does equally well on 3D medical imagery like CT scans or OCTs? or MRIs or whatever, and also video data, for example. And if you're able to start showing that, then you can reduce the need for specialized encoders. And that, in turn, makes a lot more things feasible at the pre-training space. Yeah, again, if you imagine the different stages of model development, pre-training is the most general catch-all. And then you gradually have a narrowing of the funnel with more specialization. 


---


#### 01:04:28.996

And so the more general purpose encoders that you have, and the more you can show that those general purpose encoders can interpret a lot richer modalities of data, the more you can start throwing in interesting mixtures over there. But we are not there yet right now. I know a couple of you have thoughts. Yeah, I agree. It would be nice to move to just general encoders that can really capture everything really well. But I would also argue that for something like the medical domain, it is definitely worthwhile to put in more resources into that specialization piece. And then even if we have these really broad and good encoders that work very well for the medical domain and we don't need the specialization, 


---


#### 01:05:11.045

I think we would still need specialization for how we want the models to behave in a clinical context. So like the diagnostic conversation and how to follow up with the patient and things like that. So the behavior piece, I still see that as, even if we solve the encoder piece, that we would need that specialization. Yeah, that makes a lot of sense. Okay, so the last paper on my list is TXLLM.   
(01:05:37.295) ~~This may be, I don't know if it's~~(01:05:38.938)  
pronounced therapeutics LLM, but this is another interesting one where again, essentially more modalities This time, if I understand correctly, representing chemical structure basically just as text tokens in the way that any former pre-med student can recall the C's and the H's and the O's and the way that those are laid out in a string to represent a chemical. 


---


#### 01:06:03.001

The interesting finding here is that you can weave those into training data alongside other text. And lo and behold, this is obviously becoming a recurring theme, like the model learns how to deal with that kind of stuff too, and seems to be developing a sort of a set of higher order concepts. This is like the remarkable finding of interpretability that the models are representing these higher order human recognizable concepts, love, justice, fairness, unfairness, whatever, as a means to predicting the next token. It seems like here there's something similar happening. But what I find so fascinating about these other modalities being woven in this way is that probably in a lot of cases, we don't even know what those higher order concepts are. 


---


#### 01:06:56.420

So I guess my expectation for this sort of work is that it's a remarkable first step that we can weave this stuff in and then we can start to get these guesses out. But I also see interpretability being turned on these models and doing this sort of sparse auto encoder type work to identify what are the internal concepts, and then actually discovering new concepts about the world that the models have actually learned as a means to next token prediction that we didn't even have coming in. Is that how you understand what's going on here? Is that where you see things going as well? Yeah, maybe I'll take a step back and explain the motivation of this work a little bit more in detail. 


---


#### 01:07:35.452

So I think if you looked at scientific history and if you look at scientists like Alexander Fleming or Jonas Salk and others who've discovered penicillin and the polio vaccine, they used to all be like practicing clinicians and so they would see patients during the day and then use those insights and come back at night to do the laboratory experiments. And so in many ways, obviously, our primary mission is to build out medical superintelligence that can democratize access to health care. But the process of doing that naturally feels like trying to encode the biomedical universe. And that means data from across the entire biological stack. And so starting all the way from subcellular molecular measurements, DNA sequencing, 


---


#### 01:08:17.010

RNA sequencing, protein data, all the way up to medical imagery, EHR, clinical, and population health level data. And so when you start encoding that at scale and train these models to learn useful representations, then these models can start doing interesting things. And the overall composite system that you have or you probably will end up having, is like a hybrid AI-physician-scientist. And so this model is not only going to help us fundamentally democratize access to healthcare, but it's perhaps also going to help us improve our understanding of human biology, help maybe design better therapies, and really help scale personalized healthcare to everyone. And so that's like the broader longer-term vision over here, and you're seeing specific instantiations of this overall composite system through the work that we did on Amy and also this one. 


---


#### 01:09:05.729

I think in this one, again, this is a little bit of an older work, and so a lot of the techniques that we were used are from the MetPalm era, if I may use that word. all the data is textual data in there. The model was not necessarily optimized for conversations, it was just like instruction tuning at the end of the day. But the interesting result is the fact that you can possibly have a single generalist model that you can use across the entire therapeutics drug discovery pipeline over here. So that includes tasks at the discovery slash target identification phase, all the way up to clinical trials and things like that at the final stages of the pipeline. 


---


#### 01:09:43.965

And so it was interesting. I think there are some things where we are still much further behind state-of-the-art specialist models. But then there are other things where we are already very good. And the interesting thing is this transfer learning that is happening between different therapeutic modalities and learning of interesting representations. I wouldn't say that we've done enough work in terms of uncovering what sort of unique insights that these models are learning. So there's a little bit more work to be done over there, but I think the results are promising. And then   
(01:10:08.885) ~~I guess~~(01:10:09.125)  
maybe one other paper that I would want to talk about is the work that we're doing a little bit on the biomedical discovery slash genetic discovery side of things. 


---


#### 01:10:17.434

And so over there, it's not the inherent representations that these models learns themselves that we are using for discovery, but more rather the generative outputs that these models produce. And so if you just generally think about LLMs and modern multimodal language models by training on a lot of data and especially scientific literature and things like that, they are already encoding more knowledge than any human can and any scientist can. And obviously hallucination is a big challenge with these systems, but the flip side of hallucinations is creativity. And fundamentally for advancing science and discovery, you need creativity. And so the idea over there is can we tap into that ability and capability of these systems, right? 


---


#### 01:10:56.073

And so in very preliminary work from late last year, we showed that you can use these models to identify causative genetic factors of different kinds of rare diseases. And so specifically, the work that we did in collaboration with some awesome collaborators at Stanford was that we use these models to come up with a hypothesis for hearing loss phenotype in mouse. And then the collaborators did CRISPR knockout experiments to validate the hypothesis. And so that itself, the data is very promising. And since then, we've used it to also look at human variants of unknown significance, because again, rare diseases and undiagnosed diseases are a huge challenge. And the more we can get at in terms of identifying causative genetic factors, the better we can in terms of providing care to such people. 


---


#### 01:11:38.985

And so to me, that's one of the most exciting bits about the kind of systems that we are developing.   
(01:11:43.789) ~~I mean,~~(01:11:43.989)  
we focus quite a bit on the clinical aspects over here, like diagnosis and treatment management. But for me, the other exciting bit is, in general, the fundamental understanding of human biology, the fundamental understanding of causative mechanisms of diseases, and being able to then design better therapies and things like that to really just scale personalized health care. So that's where we are stepping towards over here. And this is why it's an honor to work with Vivek because he's an ambitious visionary in the field of medical AI and there's no shortage of amazing things to work on. 


---


#### 01:12:16.916

You're too kind. Yeah, that definitely resonates with me.   
(01:12:20.878) ~~I think~~(01:12:21.439)  
it seems like we're headed for A singularity might be a little strong, but I am struck by just how on track we are for a lot of the late 90s, early 2000s Kurzweil style predictions, and also how timely they have been. We're not that far off from the curves that they drew in those books 20, 25 years ago now. It seems like in addition to the foundation models learning these new modalities, whether it's genetic sequences or these, all these different scan type modalities, or even these like chemical notations, they're also going to be trained to use the specialist tools. So   
(01:13:05.506) ~~when I,~~(01:13:05.765)  
if I just try to project   
(01:13:06.907) ~~like~~ (01:13:07.067)  
a little bit out into the future, it's not only that the core models get better and that they get this sort of like more agentic post-training finishing to be able to recover when they run into obstacles and come up with a new approach to try to accomplish their goal, which a lot of times these days I feel like they are smart enough to do it, but they just don't quite have the pattern of behavior that I need them to have to get over humps on things. 


---


#### 01:13:34.042

But then in addition to all that, it's like, they're also going to have AlphaFold 4 to have to call on when they need to. And they'll presumably be trained to use all these. And there's like, obviously a version of that for material science. And there's a version of that for basically everything under the sun is coming. So it seems like we very much are on track to the AI scientist. And   
(01:13:59.217) ~~I guess~~(01:13:59.497)  
I both am like very inspired by that and a little bit fearful of it. Just because I do think these things seem like they are on track to become more powerful than any of us individually certainly are. Maybe not necessarily to overwhelm the collective in the next couple of years, but definitely I would not want to, 


---


#### 01:14:17.447

I would not bet on myself to go head to head with the AI scientist and try to out discover it over the next couple of years.   
(01:14:25.149) ~~I guess,~~(01:14:25.389)  
is that your expectation? And if so, how do you feel about it? No, I think I share your sentiment.   
(01:14:32.279) ~~This is, I guess~~(01:14:33.180)  
this repeated joke on Twitter right now where   
(01:14:35.140) ~~like~~ (01:14:35.301)  
people say, Oh, we were promised flying cars and then we got 280 characters. It feels like we were promised flying cars and we got much better, which is GPT-4 slash Gemini style AI agents, AlphaFold kind models that can do protein structure prediction, self-driving cars, like progress in AR, VR, Vision Pro and things like that. And taking a step back, 


---


#### 01:14:53.564

I would say that the technological progress that has happened over the last decade definitely has been quite incredible and It's like multiple different technologies are converging and we're going to be accelerating quite a bit. Again, at the end of the day, I think the key thing is how do you build such powerful systems and technologies? And so what are the principles at play over here? And with any kind of technology, there's always like dual use capabilities. It was true   
(01:15:18.863) ~~like~~ (01:15:19.444)  
5,000 years back when man discovered fire. It was true when we discovered the steam engine, it was true when we discovered electricity, it was true when we discovered nuclear energy. And I think it's the same as well as we now advance with AI capabilities, right? 


---


#### 01:15:33.762

And if you look at like what has happened in history, obviously there would be concerns with such powerful technologies, but we've ultimately as a society figured out a way to use these systems in a manner that benefits optimally a lot of people. And I would expect that to be no different over here. Obviously, there's going to be a lot of discussions, a lot of churn, and a lot of societal level questions that need to be answered before we get there with AI. But I'm hopeful in humanity, for sure.   
(01:16:02.936) ~~I think we'll figure out a way. Yeah,~~(01:16:04.898)  
and perhaps,   
(01:16:06.618) ~~I think~~(01:16:06.997)  
one to get there, to that AI scientist vision, and to make progress there, perhaps one key blocker is building a simulation environment to test hypotheses. 


---


#### 01:16:18.479

Because right now, as Vivek was describing, LLM gives us a hypothesis. We have to go to the wet lab and do testing, and that takes months. And so if we can improve simulators, biological or whatever domain, then we can have that iteration loop be much faster and try out many more hypotheses. And I think that would be a key breakthrough there as well. Yeah, maybe one final quick thing over there is engineering the right amount of safety in these systems. And obviously we have this AI physician scientist vision, but the key thing that we've been stressing on is always having the expert in the loop to be able to validate or control the kind of experiments that are being run. 


---


#### 01:16:59.728

And so we are not trying to, for example, integrate the system with say a robotic process automation lab environment, because we currently don't,   
(01:17:08.873) ~~I think,~~(01:17:09.094)  
have a very good handle on how to safely control this. So it's about doing things in a manner where you're very clear that   
(01:17:15.618) ~~like~~ (01:17:15.779)  
the development is happening with safety first and foremost as paramount. And obviously we will figure things out. We'll get better at simulators. We'll get better at controlling these systems and that'll help us in turn accelerate progress further. But yeah, the key thing is having the expert in the loop right now. So the last kind of big topic I wanted to bounce off you guys is my own position. 


---


#### 01:17:36.216

And I always say we need to be more focused on what is first before we can jump to what ought to be done about it. And almost everything I've done in this process of making this podcast has been trying to just get really clear on what is,   
(01:17:48.485) ~~what's,~~ (01:17:48.707)  
why is it working, all that kind of stuff. But at this point we've got. legislation proposed, and there's definitely a shift toward what should we do about it. So I'm trying not to shirk my duty as a commenter and at least have some go-to answer. My answer right now, if people were to just say, hey, Nathan, what do you think we should do about AI broadly? I use this phrase that I describe myself as an adoption accelerationist, hyperscaling pauser. 


---


#### 01:18:18.208

And what I mean by that is basically that I'm really excited about the AI doctor and the AI coder and like all these different applications, but I am worried about creating something that is genuinely superhuman. It does seem like that's quite plausible to arrive with a few more orders of magnitude of scale. Obviously nobody knows that could totally flatline and not work, or it could work faster than people expect. And maybe it's here in, it seems like we are hearing increasingly 2027 expectations from people. I'm not, when I say pause, I do mean genuine, like, pause in the sense that I don't think we need to stop forever. I do think that we are making incredible progress on interpretability and control. 


---


#### 01:19:00.724

And that line of research is actually going much better than I had expected it to go 18 months ago. But it does feel like it's maybe still struggling to keep up with just like the raw scaling drumbeat that's happening. So what I wanted to ask you is, okay, if that's my recommendation, is that a coherent position? And when I say, is that a coherent position? It means, can I have my AI doctor without   
(01:19:23.243) ~~like~~ (01:19:23.404)  
too much more scaling? I think right now I say we're in the sweet spot where GPT-4 and Gemini 1.5 are   
(01:19:29.729) ~~like~~ (01:19:29.908)  
powerful enough to be really useful. Probably the next generation still is in the sweet spot where they're powerful enough to be really useful, but they're not so powerful that I have to worry about major accidents happening or just overall systems level stuff getting out of control. 


---


#### 01:20:30.436

Yeah, maybe I'll say a couple thoughts on that. I think maybe the idea of superhuman intelligence I don't know why we necessarily should be maybe scared of that, because in a lot of ways the tools we have now are already in some ways better than humans, like just a calculator can be better at doing calculations than a math PhD, or a computer might be better at recalling certain things or having larger memory. Our tools are already superhuman in a lot of axes. And so I don't necessarily, as long as those tools are fully controllable by us and we're able to use them to benefit humanity, I think that's a great thing. For me, maybe it's because I'm an AI researcher, but it's easy for me to put both hats on where one hat is, wow, like these AI systems are, could already do amazing things. 


---


#### 01:21:27.899

And like the results with Amy and pretty mind blowing and I think there's no argument that the pace of AI improvement is incredible. But at the same time, it's easy for me to switch that hat and go, wow, these AI systems still have so much to improve on. And hallucination is the first thing that comes to mind. But it is a serious issue. And even with   
(01:21:50.377) ~~Amy and~~(01:21:50.957)  
AI doctors,   
(01:21:52.198) ~~I think~~(01:21:52.537)  
that is an issue that at least keeps me up at night is   
(01:21:55.457) ~~like,~~ (01:21:55.597)  
how do we fix this hallucination issue?   
(01:21:58.219) ~~And so I think that~~(01:22:00.060)  
we can do a lot with Gemini 1.5 to benefit humanity. And if it did pause at that, we can still have a lot of benefit with building Amy on top of Gemini 1.5. 


---


#### 01:22:12.511

But to really solve issues that keep me up at night with hallucination, especially in those settings, I think it is needed to continue improving these models because they can fail on very basic things, as we see on viral posts on Twitter that show a very concerning lack of reasoning. At the same time, they do amazing things. So   
(01:22:37.715) ~~I think~~(01:22:38.076)  
we do need to improve those concerning error modes. Of course, it's an open problem. I don't know if scaling is the solution, but I think we need to keep thinking hard in a research sense about how to close those gaps when it comes to those concerning reasoning errors. I'm very, very confident you'll solve hallucinations. I think I tend to agree with Khalid over here. 


---


#### 01:23:02.988

If you day-to-day interact with these systems, you simultaneously feel like these are the smartest systems that you've ever seen, and also perhaps the most stupid ones in some ways. To answer your question very directly, do I think we can build some sort of a system that can democratize access to care with where current LLMs are today? I think that is possible. And I take a lot of inspiration from how self-driving cars and Waymo has evolved. And we don't have AGI for sure, depending on the definition, but we have self-driving cars that are functioning and are perhaps the most magical experience that AI has to offer. They have shown the way. And the key thing is, again, it's not something that happened magically, but rather a lot of systematic development, investment in safety, in simulation, in overall systems engineering. 


---


#### 01:23:46.421

And I think for us to get to a system that can democratize access to care, we will need the same kind of thing. And the real thing is challenges such as hallucinations, but also dealing with the long tail that you see over here. And that ultimately comes down to the kind of data that you can bring forth to be around these systems to learn. and experience from? And also, how do you actually train these systems? And over there,   
(01:24:05.126) ~~I feel like,~~(01:24:05.605)  
again, we still don't have the best possible handle. We need to get better at things like process supervision to really improve the overall reasoning process towards solving a given task. And   
(01:24:14.627) ~~so,~~ (01:24:14.967)  
yeah, I would say if I were to have these base capabilities as we have today, we can definitely build it, but it will take us a bit more time. 


---


#### 01:24:21.789

And so if we have more capable systems, it will take us a little bit more time. And that's one of   
(01:24:25.470) ~~the~~ (01:24:25.530)  
maybe the best parts about working at a place like Google, where we can continuously integrate the advancements that are happening in base capabilities and build out on top of them. And if at any point of time progress stalls, that's fine. We'll keep pushing for the vision. But the fact that we're able to do this,   
(01:24:41.282) ~~I think,~~(01:24:41.502)  
allows us to perhaps get to the overall vision and the place that we all want to go to sooner. I think that checks out to me. My intuition was that I think you guys can get there, even if there's... 


---


#### 01:24:59.328

It's not that the base model wouldn't necessarily get better, right? Because there's a lot of... Obviously, all these things suffer from major definition problems, including what is AGI and what counts as super intelligence and even just what's good enough to use.   
(01:25:12.751) ~~I,~~ (01:25:12.890)  
if we're defining   
(01:25:14.292) ~~a,~~ (01:25:14.412)  
a sort of pause hypothetically as basically you can only train foundation models at the general flop scale that they've been trained, or maybe one more order of magnitude beyond that.   
(01:25:27.103) ~~Um,~~ (01:25:27.182)  
there is still a lot of low hanging fruit in terms of just like all the different techniques,   
(01:25:31.126) ~~you know,~~(01:25:31.326)  
that have proliferated over the last couple of years. I don't think any single system has integrated all of those techniques into   
(01:25:38.331) ~~one.~~ (01:25:38.390)  
one single model or one single system at this point. 


---


#### 01:25:43.996

So that feels like we have probably a couple of years worth of work just to integrate all those different techniques. And then a lot of work of the sort that you guys are doing to really dial in performance. And it does feel like we're pretty much to the point where it can happen even without massive further scaling. Now, I will also agree with you that it probably is undeniable that it would get there faster. And that's maybe where my adoption acceleration is hyperscaling, pauser position becomes at least partially incoherent. But I do love the work that you guys are doing because I think we are headed. I don't know if you feel this, but to me, it feels like we are headed for   
(01:26:24.755) ~~ (01:26:25.076)  
Especially~~(01:26:25.456)  
last week, we had the situational awareness manuscript 


---


#### 01:26:28.837

And there's this sort of prophecy, which might in some ways become like a self-fulfilling prophecy of an AR arms race with China and this race to   
(01:26:38.324) ~~scale~~ (01:26:38.564)  
scale and the trillion dollar data center and whatever. And that feels to me like a recipe for an unstable world. And I'm like, man, is there any way that we can avoid an AI arms race with China? I would really like to avoid an AI arms race with China. And I think that the work that you guys are doing is so important in that it demonstrates how much value there already is, in some cases, even from a spring 2022 model, but certainly from the latest models, how far those things can really take us and how much the practical utility depends, not to say it doesn't depend at all on further scaling, but certainly even in the absence of further scaling, or even with a model that's now two years old, with focused attention with a commitment to really dialing in the performance, you can get so much value. 


---


#### 01:27:38.150

And I think that is something I want people to pay a lot more attention to. The fact that we already have a lot of power and we're still figuring out how to wield it effectively in these high value domains. And that's the big, obviously, I just want the AI doctor too, but in the   
(01:27:54.384) ~~sort of~~(01:27:54.604)  
big picture of AI and the dynamics, and are we going to race with China to some unknown superintelligence as fast as we possibly can and try to achieve decisive advantage over each other? Oh, my God. I think it's really helpful to keep in mind that AI doctor doesn't necessarily depend on that. And that it could be with this level or maybe a little bit more or whatever, but also it's just dedicated work of people that are really committed to the problem that is going to make, and maybe even more and probably more so than the next level of scale. 


---


#### 01:28:28.412

Because the next level of scale in all likelihood is going to be like, smarter, obviously, and can maybe do some more like really crazy things. But you're still going to have that problem of, as you said earlier, like behaviorally, you got to dial it in reliability wise, you got to dial it in,   
(01:28:43.082) ~~you have a lot of~~(01:28:43.721)  
a lot of the same problems are still going to be there, even if the model is like incrementally more capable, just because of   
(01:28:49.185) ~~like~~ (01:28:49.386)  
scale. So I love what you guys are doing. I really commend it. I think people should be much more aware of this line of work. And   
(01:28:58.689) ~~I,~~ (01:28:58.849)  
I appreciate all the effort and all the great results that you guys are delivering. 


---


#### 01:29:03.970

That might be a good note to end on. Is there anything else that, and I appreciate all the time that you've given   
(01:29:08.032) ~~today too, not just today,~~(01:29:09.112)  
but in your third appearance Vivek. Anything else you want to touch on before we call it for today? No, I think I completely agree with what you said. I couldn't have summarized it any better,   
(01:29:19.984) ~~I think.~~(01:29:20.265)  
Perhaps the only thing that would change if progress plateaus is what sort of modes exist for businesses that are built or the go-to-market and the commercialization strategies. But that doesn't distract from the fact that the kind of things that we envision are truly possible. It'll just maybe take a little bit longer or take a different path. 


---


#### 01:29:38.936

So in that sense, I think that's very exciting to know that such things are no longer in the realm of science fiction. And to me, again, it's a real privilege to be able to go deep and talk on specific topics with you. And   
(01:29:48.546) ~~I think~~(01:29:48.707)  
you are an awesome communicator of AI progress. And this is perhaps, as I said, the best podcast over there. And   
(01:29:54.734) ~~I guess~~(01:29:54.913)  
the key thing for maybe a lot of the people to know is, yeah, I think it comes down to the fact that we need to have like rational optimism about these things. And I think you perhaps more than anyone else managed to strike a balance, I think. And so that's the key. 


---


#### 01:30:08.930

I think we need everyone. We can keep doing work, but if it's projected or hyped up in a different way, then I think that's also quite bad. And yeah, I really hope you keep doing this.   
(01:30:17.015) ~~Yeah. Yeah.~~(01:30:19.435)  
Nathan, I totally I Agree with what you had said earlier. For me, it feels like it's our responsibility to try and bring this amazing technology to where it's something like healthcare or AI doctor. democratize access to a lot of people for good quality health care. And yeah, it's been a pleasure also listening to your podcast in the past. Actually, funny story, you may be one of the reasons why I am here at Google, because I was listening to the MedPalm talks that, you know, the podcast that you had, 


---


#### 01:31:32.471

Khalid Saab and Vivek Natarajan, thank you for being part of the Cognitive Revolution. Thank you.   
(01:31:37.753) ~~Thank you.~~(01:31:38.134)  
Awesome, guys. Truly, the more I think about this, the more I do think it's really important, obviously, for the medical application, but also, I'm always changing my mind about what's going on in AI, but I really think I'm headed for a bit of a drumbeat of we can get transformative value without an arms race with China. And just to know that is a conceptual possibility, I think that needs to be said more. And without the sort of dedicated hammering away effort that you guys have brought to this, I don't know that we would have a compelling case there. 


---


#### 01:32:20.423

OpenAI has another one. You may have seen this. I don't know that there'd be that much for you to learn from it, but they have put out a talk recently about It's pretty short, I can send it to you, but it's about their partnership with Harvey. and how they continued to pre-train their, whatever GPT-4 base for the legal domain and how they're dialing it in   
(01:32:41.194) ~~for,~~ (01:32:41.514)  
for that particular purpose. And I, in an effort to highlight this phenomenon across the leading companies, I feel like what you guys have here and what they have with that legal concept are two great examples of, this is like 10% compute, not 10X compute. And yet the. value that they're achieving and the value that you guys are unlocking is like night and day compared to just throwing a bigger base model at whatever. 


---


#### 01:33:09.032

Is it fair to say, I guess I should have asked this, but is it fair to say that Amy based on Palm 2 is like dramatically better than Gemini 1.5 Pro out of the box? Diagnostic conversations, yes, because Gemini was not trained to do that. But I would expect that if we bring in the same recipe to Gemini, then   
(01:33:29.885) ~~that model,~~(01:33:30.386)  
that game engine. Yeah.   
(01:33:32.426) ~~That's where my, that's~~(01:33:33.387)  
why my thing is like a slippery slope position where I'm like clinging to, it's not super, the adoption acceleration is hyperscaling positive. It's not super stable because you can always   
(01:33:44.475) ~~like,~~ (01:33:44.676)  
the adoption can be accelerated by more scaling. There's no denying that. Yeah. I think for me, it's more, 


---


#### 01:33:50.659

I'm maybe not so worried about, I actually think the probability of scale getting us to AGI is fairly low. And so we can throw a bunch of money and have a trillion dollar cluster or whatever, but I don't think it'll necessarily solve all the problems. So in that sense, maybe for me, it's more like a scientific question. I don't think it'll get us to where we are. And so I'm maybe a little less scared, I would say. But I think I like your stance on like an arms race with China, because I think this cause is currently incentivizing other nation states to actually treat this as an arms race. And we're already seeing evidence that China may be much further ahead than we might've thought. 


---


#### 01:34:23.055

The video generation models are good. Yeah, so the more maybe we can slow down that discourse I think is good. That's another thing that I, it's very hard, but I'm trying to, first of all, get an accurate picture, but it seemed my best guess right now is that the strength of the Chinese research community is not going to be denied. First of all, so you just look at some of the papers, even out of Western institutions, and you just look and it's all Chinese names. So there's that. I didn't go to NeurIPS this last time, but I heard that it was common to hear Mandarin conversations just walking around.   
(01:35:01.711) ~~So, man, I just,~~(01:35:02.570)  
it sucks so much to think that we would end up in a, not to mention the overall,   
(01:35:08.012) ~~not overall, but just the sort of~~(01:35:09.252)  
toxicity that sort of thing has for our own culture too. 


---


#### 01:35:13.253

We have this sort of prize, open, multicultural, multi-linguistic, whatever dynamic. And if all of a sudden it's, are you an agent of the CCP? Is it being asked all the time? That's really going to suck too. And it's not going to be good for   
(01:35:26.737) ~~us.~~ (01:35:26.777)  
us being the West or America or liberal democracies, however we want to define us. I agree with that. I think there's also a big cultural difference. For example, he says that at Stanford, queues form if Sam Altman is going, whereas at Stanford, queues would not form for Sam Altman, but it would form for John Shulman. So they recognize the real people and the real deal more than maybe the known faces or the quantificators. 


---


#### 01:35:52.489

And so there is, I think, that thing that they have going for them, which is like the culture is more grounded in actual work rather than the business faces or the quantificators. And so I think that's also helping them, which is   
(01:36:03.621) ~~I think~~(01:36:03.822)  
a little bit different and we don't have that going just yet. Yeah. Isn't she like a chemical engineer by training or something? Some crazy number of the Politburo is like engineers of various kinds. Yeah. I would not be surprised.   
(01:36:16.565) ~~Um,~~ (01:36:16.626)  
I wish this stuff can also just be siloed where in a sense where, okay, it makes sense that when it comes to army applications or that stuff is siloed and non-collaborative, but AI is so broad and has so many different applications that one specific application of military should be its own thing. 


---


#### 01:36:36.465

And yeah, sure. Countries are going to do their thing with that, but AI is so broad. It shouldn't be caught up with just that single application. I sure hope we can avoid it. We still have thousands of nuclear weapons on hair trigger alert or whatever. That is something I would really love to see us avoid for the AI era. But I'll let you guys go. This has been fantastic. Let me hit stop actually and let's give it 


---



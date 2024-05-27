#### 00:00:00.149

Well, I'm excited to be here with everybody and look forward to sharing what I hope will be an interesting and super fast pace journey through the modern AI landscape. I call this the AI scouting report, the not investment advice edition. And I really think of my own personal project as this concept of AI scouting, which to me means. trying to get the most broad, wide angle, comprehensive and up-to-date view of everything that's going on that I possibly can. That turns out to be super hard because everything in AI is going exponential as you'll see. And it's really beginning to touch all parts of the economy and even society as a whole. So   
(00:00:40.802) ~~it's,~~ (00:00:40.942)  
it's a hard space to give up with, but I figure somebody has got to do it. 


---


#### 00:00:43.804

So I'm giving it a shot. I divide my time across a bunch of different things. I started this company, Waymark, which is based in Detroit, Michigan. That's also where I live and I'm coming to you from. And what we do is help small businesses create videos with AI. You can show up on the website, tell us who you are. We go out and find all the information that we can about you in about 30 seconds. And then in another 30 seconds, we will literally make a video for whatever purpose you want. Could be advertising, could be announcing a new product or introducing a team member, posting a job,   
(00:01:16.463) ~~you name it.~~(00:01:16.843)  
You literally just ask for what you want. 


---


#### 00:01:18.924

The AI does the rest of the work. It writes a script. It puts all the assets together. It even creates a voiceover with AI and then puts that in front of you ready to watch. So that's the thing that I've spent the most of my time on over the last however many years. But these days I'm also doing a podcast on AI called the Cognitive Revolution. And I am an AI advisor to a couple different companies, including Athena, which does executive assistant services, and also this other company called Stellas, which is a custom AI app studio. So we build AI apps for small businesses that need solutions. In addition to that, I've also worked a little bit with OpenAI and Meta on their AI safety review projects, which is a whole interesting story in itself. 


---


#### 00:01:58.287

But I'm not going to tell that one tonight. If you want to hear the long form version of my experience with OpenAI, there's a Cognitive Revolution episode about it. So tonight I know this is a pretty intellectual group. I'm told the majority are doctors and lawyers, so I'm going to really not pull any punches in terms of being very in the weeds about some of the important details of what is happening in AI. Now we're going to start off with just a quick rundown. Obviously can't cover anywhere close to   
(00:02:25.336) ~~any~~ (00:02:25.515)  
everything, but a couple of key points specifically from the field of medicine to describe the current state of the art when you see SOTA in AI that refers to state of the art. 


---


#### 00:02:36.217

We'll talk a little bit about how that's already impacting the economy, what the limitations are of the current systems, then I'll get a little bit theoretical for a bit and talk about the inputs to how AIs are made and some of the science that actually goes into making them work as well as they do. And then toward the end, we'll get into the true not investment advice section where I try to in my crystal ball gets very foggy after just a pretty short time into the future, but where I at least have a little bit of a sense for how I'm thinking about investing and what companies are in the best position. Can close it with a few key questions that I think will really be super important to watch as we try to get a sense for where this whole AI thing is headed. 


---


#### 00:03:20.512

I'm not going to use analogies. I often call my content an analogy free zone because I think that   
(00:03:27.278) ~~this is something,~~(00:03:27.919)  
the AI phenomenon is something that is really worth the time and efforts to understand on its own terms. I think it is as important of a phenomenon and as fundamental to understanding the world as   
(00:03:41.491) ~~like~~ (00:03:41.632)  
understanding DNA and natural selection. to walk around the world without those concepts just leaves so much unexplained and puts you in a position of confusion. I think there are some core concepts in AI that are really becoming similarly important. And so I don't use analogies to describe them. I'm going to try to describe them in very literal terms, simple as possible, but very literal without being wrong is what I try to do. 


---


#### 00:04:05.669

And then I won't do any like big predictions, although I do have a few thoughts toward the end on at least how I'm thinking about allocating capital. So I guess I'll break my no predictions rule just ever so slightly. Okay. Here is a little tap dance through the current state of the art, specifically with a focus on medicine. So where are we in AI today?   
(00:04:27.362) ~~I think~~(00:04:27.581)  
it's really important just to try to keep tabs on that. It's a big part of what I do is try to have an up-to-date sense of what our current AI systems capable of. So it's really remarkable, but it is undeniably true at this point that since the middle of 2022, the best AI systems have been better than the average human at the average task. 


---


#### 00:04:52.980

That is to say, if you go find some random task that might be typical of white collar computer work, you take a typical intern or young employee and ask the AI to do it and ask the employee to do it, you're going to get better results from the AI. That's been true for almost two years now. In addition to that, the best AI systems are really now closing in on expert performance for routine tasks. And the word routine there is really important.   
(00:05:21.802) ~~Routine means~~(00:05:22.624)  
it's obviously common and that we know what good looks like in medicine. You might think of something like the standard of care, something that is well established. So that's a really remarkable phenomenon and it's happening super quick. 


---


#### 00:05:35.403

GPT-2 was released in 2019. I read about that at the hospital on the, when I was there with my wife as she was about to deliver our son and five years, he's just turned five, five years later, we've gone through a series of different generations of the models to now the current one, GPT-4. is closing in on human expert performance on really demanding tests of cognitive ability. This test, the MMLU test, is comprised of undergrad and graduate school exams across a super wide range of topics. And the average GPT-4 score at this 86 compares to the human expert in their domain. So it's coming close to matching what human experts can do in domain, but it's beating the humans. 


---


#### 00:06:26.009

If you were to have one human try to answer all the questions across all the domains, then the GPT-4 result would be notably stronger.   
(00:06:33.151) ~~So~~ (00:06:33.271)  
That is pretty crazy and it's happened in a pretty short period of time. Now to get more specific in terms of how this is playing out in medicine, here is a similar curve focused on a U.S. medical licensing exam to pass in somewhere in the range of 60, low 60s. The first system that pretty clearly passed the medical licensing exam was MedPol. That is one from Google. Not too long after that, really just a few months. Look at the scale of December 2022 and March 2023. They came out with MedPol 2 and it hit 86%. 


---


#### 00:07:10.915

And again, that is closing in on expert performance on the medical licensing exam. It goes further in medical question answering. Here are nine different dimensions on which they evaluated. This is again out of Google. They evaluated an AI and a human doctor head to head, and they asked human doctors to evaluate both the AI and the human doctor participants. The top section here are the good things, the things that you want to see in your answers to your medical questions. Things like reflecting the consensus of the medical establishment, reading comprehension, knowledge, recall, better reasoning. The orange is how often the AI was judged to have done a better job. And the blue is how often the human was judged. 


---


#### 00:07:56.245

The human doctor was judged by other doctors to have done a better job. The gray was in between is when it was considered to be a tie. So you can see that the AIs are dominating on the good things. And then here are the bad things. This is the one of nine categories on which the AI was judged to be worse. It did more of bringing up inaccurate or irrelevant information. Not a ton more than the human, but a bit. The humans did all the other bad things more than the AI did. So we're, again, getting into this strange zone where state-of-the-art AIs are closing in on the performance of experts, even in cognitively demanding areas like medicine. 


---


#### 00:08:38.493

Here's another study. Again, this is medicine. This is differential diagnosis. On the left is the AI. On the right is the human. There are four bars here that refer to whether they had the exact match on the proper diagnosis or some increasingly permissive definition of accuracy. And then the top K is how many guesses they got before they got to the right one. So again, you see the AI is at a significantly higher accuracy percentage across the board as compared to the human doctor. These are primary care physicians specifically in this study. So I tell people in all seriousness these days that   
(00:09:18.812) ~~I,~~ (00:09:18.932)  
if I had a medical condition that genuinely worried me, I would not be without my AI doctor. 


---


#### 00:09:24.875

I would also, of course, want to have a human doctor. I wouldn't put all my trust into the AI, but I would absolutely be cross-referencing their answers and cheffing them against one another to try to get the best of both worlds. But I would not be without my doctor if with a serious medical condition in today's world. A lot of other interesting applications just in medicine as well. This is a project on virtual tissue staining. I don't know a lot about the traditional way that this is done, biopsy and slicing tissue and staining it, looking at it under a microscope. I'm told that this can take hours and that it's too slow to be done while the patient is in surgery. 


---


#### 00:10:04.820

Now there's a new technique that includes this in situ imaging, and then they add this virtual stain to it. And now they can get these sorts of images out of patients in just seconds while they're still in the operating room. So if you're doing some sort of procedure to try to extract or to try to remove a tumor, you can get a lot of these images in real time as you're going. And that, of course, can lead to better patient outcomes. So the creativity that people are bringing to all these different applications of AI is   
(00:10:33.379) ~~super,~~ (00:10:33.619)  
super interesting. Here's one that flies under the radar and always blows my mind. This is literal mind reading. 


---


#### 00:10:39.254

I have a full episode, actually two now. We just put out a second one on the successor to this project. But what they've done here is taken fMRI scan data and taught an AI to reconstruct the image that the patient was looking at when the scan was captured. So you're in an fMRI, you're shown these images, they capture the data and they record what you were looking at at the time. And then you do a bunch of that. And then after that, the AI can take the brain data, the fMRI data, and reconstruct the image that you see here on the right, where the original one was the one on the left. So you can literally decode brain activity and reconstruct images with this level of fidelity. 


---


#### 00:11:22.855

And I often think, man, I feel like when I was a kid. this would have been major news. And somehow today we live in a world where it just crosses over and gets a few retweets or whatever. But most people don't even realize that this kind of thing is out there. So literal mind reading is happening. And with the follow up to this, with this original one, it took 30 to 40 hours of scan data to train the AI to decode one person's brain. With the latest update, they're now down to one hour of scan data required. So it is actually starting to get feasible where you could put somebody into the thing for an hour and get this type of process up and running without it being a shootout. 


---


#### 00:12:06.982

Obviously, we do a lot of things. I think one thing that's important to keep in mind, and I'll get into a little bit more detail in just a second comparing what the AIs are best at and what humans are best at, but they can't do everything, of course. So this is a study of what they can do and how that breaks down by different kinds of jobs. Interestingly, and this is definitely a surprise, and I think this has become   
(00:12:29.419) ~~kind of~~(00:12:29.620)  
common knowledge at this point, The AIs that we're getting are not really the AIs that we expected. We expected that they would automate relatively low wage and low status labor first. But on the contrary, they seem to be impacting high wage and high status labor first. 


---


#### 00:12:45.865

Your proverbial plumber or custodian of a building is like not feeling much impact yet from the current way of those AIs, but your doctors and lawyers are definitely seeing significant impact. So this study broke jobs down into five different categories. The green here is the lowest, let's say, status, wages, and lowest impact. As you go out, it's the fourth one actually, it's the fourth quintile that's the highest one out. So the most impacted are the fourth quintile and then the fifth quintile comes in a little bit again. And to read this, you can basically think of all the area under the curve is the amount of work that AIs seem to be poised to be able to do. 


---


#### 00:13:30.024

Everything outside of the curve, they would not be able to. So if you're a plumber or a custodian, there's a relatively small amount of your overall work that is likely to be impacted by the current wave of AIs. Whereas if you're a doctor or lawyer, maybe out here somewhere, this is to say about half of people have about half of their tasks. such that AI could impact them, plausibly be a significant part of them. I think that's really something that we are going to be adjusting to for quite some time. And again, we're just getting started in this AI era. Here's one thing that was really just announced and is coming to market right now. 


---


#### 00:14:06.216

This is AI nursing. This company Hippocratic AI has a pretty interesting go-to-market proposition where they are charging by the hour for their AI system. So you're starting to see AIs that are actually competing in essentially a label market, not by API calls, not by number of tokens generated, but literally by the hour that they're working for you and doing stuff. Of course, they're like scalable and clonable in the way that that software systems are, but they're actually starting to charge an hourly rate. They charge $9 for their AI nurses. And   
(00:14:40.658) ~~they,~~ (00:14:40.859)  
this company specifically is   
(00:14:42.059) ~~like~~ (00:14:42.220)  
trying to be very cautious, very safety focused. They are not, even though you saw the result above on the. relative strength of AI systems on diagnosis. 


---


#### 00:14:52.708

This company is taking a strong, we're not trying to even get into diagnosis, but we do think that we can get AI to do a very reliable job on a lot of these follow-up tasks that either nurses do or that, frankly, today, nobody does because there's just no time in the day to do them. So they have all sorts of things where they'll call you and work through you. pre-op thing or follow up on your discharge instructions or make sure you're taking your medicine or check in on how you're feeling, all that kind of stuff. And $9 an hour is the going rate for an AI nurse in today's world. Okay. So where does it stop? 


---


#### 00:15:28.572

This is where we get to limitations. where it stops is things that are not routine. So can AI do new science? In general, the answer today is no. There are a few very engineered and purpose-built systems like your alpha folds that I'm sure people have heard of that are specifically designed and highly tailored to do a narrow task in science. And those are high impact systems as well. But the general purpose systems are like chat GPT like things that you can talk to and just have do whatever you want. Those things today cannot do new science. And that basically extends to general, novel, unfamiliar. Somebody really has to figure something out for the first time situations across the board. 


---


#### 00:16:13.754

They are not good. Those.   
(00:16:16.154) ~~I often~~(00:16:16.514)  
I used to say actually no Eureka moments. That was one of my summary bottom lines for the state of AI. Now I have to say precious few Eureka moments because this is actually one instance where GVT-4 was doing a better job on some pretty novel stuff compared to even human experts. I'll just try to play this video and the scenario here is they're trying to train a robot hand to do various tasks. The task in this case is whirling a pencil, and they use a technique called reinforcement learning. So this gets a little meta because it's AI training other AIs. But to do these sorts of reinforcement learning programs, you have to have what's called a reward function. 


---


#### 00:16:58.520

When the AI is just beginning, just starting to learn what's what, it doesn't do very well. And so it needs some score to learn, like, when am I doing better? When am I doing worse? I can do more of the stuff that it's giving me the high score and gradually find my way to figuring out how to do the test. So the reward function you could imagine sitting down and trying to come up with, OK, if I'm looking at this, how would I score it so that I could give the A.I. a signal from which to learn how to get better at this task? And you might think,   
(00:17:25.428) ~~OK, well,~~(00:17:25.768)  
maybe I could measure the angular momentum of the pencil and turn that into a score somehow, something along those lines. 


---


#### 00:17:31.894

There are people that do this, right? This is an expert task to write reward functions for robot reinforcement learning. Turns out that GPT-4 is significantly better. at writing these reward functions for robot reinforcement learning, even then the people who did it, and this is not like you're a person on the street   
(00:17:48.729) ~~sort of~~(00:17:48.929)  
task, right?   
(00:17:49.949) ~~I'll just~~(00:17:50.368)  
again, step back and you go talk to somebody on the street and say, Hey, could you write me a reward function for this robotics reinforcement learning project that I have?   
(00:18:00.873) ~~You will not,~~(00:18:01.373)  
they will not even parse that sentence. let alone give you a serviceable reward function. So you're by definition in expert territory here, and yet GPT-4 still able to significantly outperform the human reward function writers. 


---


#### 00:18:17.118

That doesn't happen very often. This is the exception, not the rule. But I had to update my summary position from no Eureka moments to precious few Eureka moments because of a number of little projects like this.   
(00:18:31.567) ~~Here's~~ (00:18:31.727)  
one other one that   
(00:18:32.527) ~~kind of~~(00:18:32.807)  
still   
(00:18:34.288) ~~I'm~~ (00:18:34.407)  
still wrapping my head around. This is a example of a language of essentially a chat GPT like model trained on just tons of DNA sequences, 300 billion base pairs   
(00:18:47.273) ~~of work~~(00:18:47.615)  
of DNA sequences, all drawn from bacteria and phage DNA data. And what they find is that now they can use this thing to generate new stuff. So they've found that they are able to generate a variety of CRISPR like complexes. 


---


#### 00:19:06.071

These are all complexes generated by the DNA generating AI. And the other thing that they can do that's really interesting is they can start to perturb the AI and see how confused it gets and use that to determine how essential different genes are to the survival of the cell. They call this in silico gene essentiality experiments. And apparently this is, again, quite a cumbersome process to do if you're doing it in an actual traditional lab context. But now they can run it in just   
(00:19:38.291) ~~like~~ (00:19:38.432)  
a couple seconds for because they can obviously do it in the computer. So this stuff is and this is just from the last few weeks. So this is really some of the latest and greatest. 


---


#### 00:19:47.324

And I think we're just beginning to see the impact of all these advances across a wide range of fields. So hopefully that has you motivated to understand a little bit better how it all works under the hood. The core inputs to AI systems are data, compute, and algorithms. That's   
(00:20:09.803) ~~like~~ (00:20:09.962)  
your Trinity, your three-legged stool. Without any of these three, it's not going to work. So you need data, from which to learn. You need compute to crunch the numbers and you need an algorithm that actually translates that data and that number crunching into something that actually works. So I'll take you through each of the three. Code starters, all these systems are really just information processing systems. 


---


#### 00:20:35.451

You might call them circuits. They are inspired by human neuroanatomy, but they're definitely not much like human neuroanatomy. One thing that they all have in common is that they are all unidirectional. They are all differentiable, which means there's no cyclicality. In the human brain, you have different parts regulating one another and a lot of crosstalk. In the AI systems that we have today, they proceed very linearly from one layer to the next. So this is just an example of a really simple thing where you might have a number and your goal is to classify this image as what number is. This image is about what is obviously seven. You can break this up into pixels. 


---


#### 00:21:16.682

You can feed raw pixel data in here and it progresses through the layers. And then your goal is to get a seven to be the one that lights up. And if that happens and it's working effectively, then you have   
(00:21:27.150) ~~a,~~ (00:21:27.210)  
an AI now that can identify which number it is. So it's a very simple system. I strongly recommend if you want to go see great visualizations of this, the YouTube channel 3Blue1Brown does some of the best visualizations, not just on this, but on all sorts of different mathematical things. But this short clip is drawn from a longer series that is really good for building intuition if you want to go check something like that out. 


---


#### 00:21:53.127

OK, so. There are these information circuits, but let's get a little deeper now on how do you actually get it to learn? A super important concept is sitting at the heart of this is the loss function. The loss function is the way that you score the output from the AI. So let's imagine you are at the beginning of a training process. And   
(00:22:15.255) ~~by the way, they usually just randomly assign the numbers at the beginning. There's not like~~(00:22:19.257)  
there are some tricks, but traditionally the numbers in all these different positions are just randomly assigned. So what happens at first is basically garbage in garbage out. You have your kind of matrices that are crunching all these numbers. 


---


#### 00:22:32.291

It starts in a very random position. Let's say you go ahead and put a two in, you crunch all the way through the thing and you get this kind of result. And it gave a high rating to a three and also I rating to a six very strangely and I rating to a one and the actual two was a very low rating. Okay. That's a bad prediction from the ads. It's not able to do the task at this point, but you can score it. So you can say, Hey, your two, your score on two should have been higher and everything else should have been lower. And now you have a score. You can put that into a single number and you can say, this is your score. 


---


#### 00:23:05.518

And then you can do what is called backpropagation. which is saying, if I go back through all the different parts of this system, all the different numbers in the matrix, and I look at each one and I ask, if I tweaked this one, should I tweak it up or should I tweak it down to make the overall score a bit better or a bit worse? This is ultimately chain rule from calculus. For each number in the thing, and if you're talking about a GPT-3 scale system with famously 175 billion parameters, then you're doing this literally 175 billion times. In these small systems, it can happen very quickly, but it does take a lot of number crunching as the systems get big. 


---


#### 00:23:44.801

But for literally every single parameter in the system, you're just saying, okay, I can either move this up a little bit or down a little bit. And I want to just do that in such a way that makes the final score better. It's a really simple concept. Actually, you have a loss function, which gives you a score. You use back propagation to work your way using the chain rule of calculus from the end all the way back to the beginning of the network, tweaking every single little parameter along the way. And then you do that in a loop and that loop is called gradient descent. So I'm sure you've heard some of these terms flying around. 


---


#### 00:24:15.834

Gradient descent is the process of just through all these little incremental changes, gradually finding your way to something that works. So this is a visualization of what's called a loss landscape, which is like at any given point in the space of all the possibilities for the numbers in this information processing work. you're going to have some loss value. And as you work your way down to the lowest possible loss, that is the process of grades. And this gets complicated. You've got all sorts of different strategies for find your way down the hill. And you can imagine people have been working on this for a long time. So there's lots of different little complications to it. 


---


#### 00:24:53.432

But this is basically the core thing. You have to have something that is differentiable so that you can do this back propagation. You have to have a score so that you have the loss function. If you have those and you run this in a loop, you are doing gradient descent and you are on your way to training in AI. What you'll typically see are these loss curves, where as you go step-by-step, the loss gets better and better. You're finding your way to the best possible solution. Traditionally, this was done with curated datasets. So   
(00:25:22.673) ~~this one,~~(00:25:23.114)  
this is like a classic dataset, a dataset of just nothing but small images of hand-drawn numbers. I think it's called MNIST. 


---


#### 00:25:32.461

But that's all it is, right? Small images of hand-drawn numbers, and there are some that you're meant to train on, and then there are some that are meant to test how well you did from the learning process. And typically what people would notice is that the more you would train, your training loss would go down. You would continue to see better and better scores. But then when you actually tried it on the test set, or also sometimes that's known as the validation set, you would see that at some point, the validation results would get worse. And this was typically considered to be the point at which the model is overfitted. That's another term that you'll potentially hear if you spend more time in this area. 


---


#### 00:26:12.355

When it's overfitting, it is learning now idiosyncrasies of the dataset that don't actually mean anything for the general case. So   
(00:26:21.601) ~~you can essentially,~~(00:26:22.280)  
you can imagine like memorizing a bunch of strange, weird cases and getting,   
(00:26:25.863) ~~you know,~~(00:26:26.242)  
really good on the test, but this is teaching to the test. Now you go and show other handwritten numbers. It's actually getting worse because it's learning the wrong stuff. So past this line where the validation gets worse, that is known as overfitting. Okay. Here's where the paradigm has changed, right? That was the traditional thing. You'd have a data set. The data set was finite. You'd train on a certain amount and then you'd test on a different amount. 


---


#### 00:26:49.330

And the game was like, who can come up with the best algorithms, the best architectures to get the highest validation score. That was the pinnacle of the field. now things have changed very significantly. And the big unlock has been figuring out clever loss functions that allow you to tap into huge amounts of unstructured data. There's only so much labeled data in the world. And the key thing about these data sets is that again,   
(00:27:17.970) ~~you know what the number is, right?~~(00:27:19.352)  
There's a, the data set includes the image, but it also has the label. So you can check your answers against the actual answer key, but What they've done now with these what's called unsupervised learning is they've come up with clever formulations to allow the world's web scale data to serve as training data. 


---


#### 00:27:39.230

And there's two big things that have been popular recently. One is called next word or next token prediction. And the other is image denoising. So in next word prediction, and this is how we're now getting to Cheshik T and that sort of model, the whole body of all human texts becomes available because your job is now just predict the next word. So you take   
(00:28:02.553) ~~all of the,~~(00:28:03.173)  
all possible texts, you cast that into a vocabulary. There are like 50,000, sometimes a hundred thousand. possible outputs in these text generation systems. And you do something very similar to what we showed here, except instead of 10 numbers to choose from, there's now 50,000 possible next tokens that you could output. 


---


#### 00:28:23.146

And you get a very similar score and you can do back propagation. But the key is that the text itself provides the answer. So now you can just crunch all available texts. And for every single bit of text, you have the opportunity to score yourself with a loss function and to do that back propagation. So this is how the data sets have become huge. A similar thing has happened with images where somebody came up with a very clever idea of what if we first added a bunch of noise to existing images? What if we degraded the images purposefully with noise, and then we train an AI to denoise the image? That would allow us to use all of the images that are out there for training data. 


---


#### 00:29:04.935

So this is Bennett. I can't overstate the importance of this paradigm shift from small curated labeled datasets to web scale, unlabeled, but self-documenting datasets. that is known as unsupervised learning. And this is how all the main scale systems in today's world are trained. Okay.   
(00:29:24.963) ~~And you also need,~~(00:29:25.525)  
so that was all data, right? Where's the data coming from? What is the nature of the data? How are we using the data? You also need compute. Of course, there's been massive amounts of investment in computing infrastructure. NVIDIA's stock price has gone up tremendously because they are the leading company that is providing the GPUs that are doing all the compute. The key thing about GPUs as opposed to CPUs that you need to know is just that they allow for massive parallelization. of the calculation. 


---


#### 00:29:53.885

You can imagine that you're going to ask a question about 175 billion numbers. Do I tweak it up or down? You don't want to have to do that sequentially because it'll take a really long time even if you have a really fast computer. So you need to come up with some way to ask that in parallel for as many of those different numbers as you can and then bash the results together and then make the updates. So that's part of where the algorithm progress comes in. And that takes you to the transformer is the number one, pretty much dominant,   
(00:30:23.233) ~~uh,~~ (00:30:23.314)  
approach to AI today in the world. I'm trying to not use too many advanced vocabulary terms because I know that people get lost in the jargon. 


---


#### 00:30:32.317

So here's a quick glossary of terms. The transformer is just a type of information processing circuit. The tokens are another word for the words, or it could be like a little part of an image. When you embed something, that is the process of converting that text or image input to numbers. The neurons are the nodes in the network. They're generally organized into layers. As I said earlier, everything has to be sequential. You can't have like loops in there. Sometimes these are also called activations or the values at the particular neuron places are called activations. There are three different parts of the transformer that are important. The attention mechanism is the one that gets all the attention because it was one of the big breakthroughs. 


---


#### 00:31:16.733

The MLP is the multi-layer perceptron. And then you have these things called nonlinearities. These are typically each layer will have all three of these. Then you finally get to the parameters and weights. These are the numbers that are actually in the thing, sitting there, that were trained, that were learned, that are going to do the number crunching. You'll also hear words like logits. These are the final numbers that get output before they're finally converted back into actual text, the forward pass is the process of actually running the thing once, and the model is the thing that is actually run. So I just like to go through these real quick because there's so much jargon and it's very easy to get lost in all the jargon. 


---


#### 00:32:00.881

I better keep moving quick because I've got a lot more to go. I mentioned that the transition to unsupervised learning and the massive amount of data that comes available when you switch to that paradigm has been super important. So let's talk about scaling and then a couple of really interesting observations as people have started to scale up these systems. They're getting really big. There has been a whole study of what are known as scaling laws, which is to say, how good are these things going to get if we put a certain amount of resources into them? And what you'll notice across the board in these sorts of system designs is that there's always a Pareto curve. 


---


#### 00:32:41.558

There's always some optimum point where you can make the model bigger in terms of parameters, but then it takes more compute to do each process. So you can't for a given compute budget, then you can't process as much text. If you make it smaller, then you can do more loops, but the smaller models don't tend to learn as fast. So there's always this sort of optimum point where you're choosing the right balance between how big you want the model to be and how much data you're going to run through it in the training process. for a given budget. So each of these different colors represents a given compute budget. We're here at 6 to the 18 times 10 to the 18. 


---


#### 00:33:19.171

That's big, but it's still eight orders of magnitude below the White House threshold for reporting large training runs, which they set at 10 to the 26 flops. A plop is a floating point operation. It's literally just a small unit of compute. You're doing a thing with number. You're doing that 10 to the 26 times to trigger the White House reporting requirements. And here they're going from eight to five orders of magnitude less than that. But what's key about this is these small studies have allowed them to then draw these lines, which allows them to project out into the future as they're really scaling these systems. How good do we think they're going to get? We can predict the loss. based on this scaling law for a given compute budget. 


---


#### 00:34:04.990

And this is how people are starting to back into these things like, OK, we should have this many billion parameters and this many tokens and they want to run through it. And   
(00:34:13.574) ~~we~~ (00:34:13.994)  
it's going to cost us this much money. So how big is this getting today? The big systems, GPT-4 was trained on 10 trillion tokens. That's essentially 10 trillion words. And it costs reportedly some tens of millions of dollars just to run the compute. That does not include like the salaries of the researchers or collecting all the data, but literally just to run the servers to do the work. GPT-5, allegedly in training or getting close to the end of training, is expected to be trained on 10 times more than that, 100 trillion tokens, and is expected to cost a few billion in compute. 


---


#### 00:34:50.617

So that's pretty crazy. But it is bringing also some crazy results. So one of the things that is most remarkable to me about these systems is that they seem to learn things that they were not explicitly told to learn. The first sign of emergence, this is a story from the open AI team from back in 2017. So this is way smaller. They didn't have all the compute, all the resources they have now, but they trained a model just to predict the next character in Amazon reviews. And then as they were looking inside and looking at the activations, which parts, which nodes in the architecture had high values and under what situations did those positions have high values? 


---


#### 00:35:36.353

What they found is that there was one little neuron that was lighting up strong if it was a positive review and was like very strongly negative if it was a negative review. And people have been trying to do sentiment classification for a long time. This is   
(00:35:49.505) ~~like~~ (00:35:49.626)  
a pretty well established thing and people had all sorts of techniques. What they were amazed to see is that this system, which they had only trained with a loss function of predicting the next token. internally had this neuron that if it was on its own a sentiment classifier would have been the state-of-the-art sentiment classifier at the time. So this is like a really profound observation because wait a second we just trained this thing to predict the next token and yet internally without us ever giving it any signal or information about The sentiment, even the concept of sentiment knows nothing about that. 


---


#### 00:36:25.980

Or at least we didn't tell it to know anything about that. Somehow it has come to represent sentiment as a means to do what it is ultimately doing, which is predicting the nest token. So somehow. representing or understanding what the sentiment is, helps you predict the next token, which that intuitively makes sense that it could help. But what's remarkable is that it is learning that. So as Craig Gartman, the president of OpenAI put it, semantics emerge from a syntactic process. Even though it was only trained to predict the next token, it learned a higher order human recognizable concept, which is sentiment. That is really the sort of breakthrough that is at the heart of the advances now that we're seeing that make these systems so general. 


---


#### 00:37:13.177

There's been a lot of other study, I'll go quickly over this because we don't have a ton of time for it, but similar phenomena have been observed when you train a model to play a game and you maybe just train it to predict the next move and all it gets to see is a sequence of moves like this, like F4, this is Othello, F4, F3, D2, F5, that's all it ever sees. And yet they can look inside the model and begin to decode that it is actually representing a two-dimensional board state. and allocating that board state with each move as pieces get captured and territory switches hands. So all it ever saw was this, but it learns to develop its own conception that looks more like this. 


---


#### 00:37:49.905

This is also happening in image understanding or computer vision models where you have these different neurons that seem to respond to a particular concept. And then people figured out how to reverse engineer.   
(00:38:00.590) ~~Well,~~ (00:38:00.710)  
what would be an image that would maximize that? And what would that look like? And you do these sort of trippy things where it's okay, that's a window and that's a something and that's a wheel. And that's what maximizes these particular. neurons and then as they feed forward to the next layer, these sort of window and car body and wheel detectors all send a strong signal to what appears to be a car detector. And this is the image that would maximize the response from the car detector. 


---


#### 00:38:26.208

Now, there was no engineering to say, this should be the card detector of neurons. All of this is an emergent process that just results from this definition of a loss function, the process of gradient descent, and the massive scale at which these things are now operating. These models are learning these high order human recognizable semantic concepts from this purely syntactic process. That is something that   
(00:38:54.123) ~~I think~~(00:38:54.344)  
way more people should understand. And if there's one takeaway that I would want you to leave from today with, it would be that. Okay. So   
(00:39:04.686) ~~what, this is a really~~(00:39:05.525)  
another kind of profound example of it. Here's a task called modular addition. You may remember this from your MCAT studying days or whatever. 


---


#### 00:39:12.952

The idea here is to take two numbers, add them together, then modulo divide by a third number and take the remainder, right? So five plus 12 modulo 12, it's 12 divided by 12 remainder is zero. 17 plus eight is 25 divided by 10 is two remainder is okay. So they train a model to do that. It learns to do the task, but right in here, what is the process or where you would traditionally call overfitting because it   
(00:39:41.083) ~~like~~ (00:39:41.242)  
learn some, but then the. Validation performance falls off. The test performance continues to get better and eventually memorizes   
(00:39:49.117) ~~the whole test or~~(00:39:50.139)  
the whole training set, but the validation is bad. So for the longest time, people have just said, well, this is useless, right? 


---


#### 00:39:56.322

You've just trained a model, it memorized things, but it didn't actually learn the real task. And so they would have stopped long before. Notice this is a log scale, right? So this happens at like hundreds of optimization steps. Finally, somebody said, well, what if we just run this a really long time? What if we give it   
(00:40:10.128) ~~like~~ (00:40:10.307)  
10,000 optimization steps? What they find is they get out toward a million optimization steps is that it actually generalizes and learns a real solution. And they call this grokking generalization beyond overfitting. So overfitting here, traditionally people would have stopped here because, okay, well, the validation lost ever gets better once it starts to get worse. except that it actually does. 


---


#### 00:40:33.215

It just takes a lot longer for it to finally learn to do this task. And now, at the end of this, it can actually do modular addition even on examples that it hasn't seen. It learns the examples that it sees in the training early. It takes a long time for it to grok the general concept of modular addition and do it for unseen examples. But that's really profound, right? That it's able to make this shift from memorizing the examples to learning an underlying algorithm. The algorithm that it learns is   
(00:41:01.257) ~~like~~ (00:41:01.458)  
quite weird. I'll show that in just a second. But this is a really key point that we don't know in the process of training these things, when something will be grokked, when the model will go from just predicting whatever next token might seem plausible to actually figuring out the underlying concepts and being able to use them across the board. 


---


#### 00:41:21.893

So for my money in the GPT-4 technical report, which is the paper that they put out, this is the most important sentence. Certain capabilities remain hard to predict. We showed the scaling loss that show how they can predict what the loss is going to be. That is the aggregate score. But what's really still a mystery is how does that aggregate score translate to particular behaviors, to particular abilities, to which kinds of problems it's going to be able to solve and which kinds of problems it's not going to be able to solve. And here you see one where as they got models bigger and bigger, this was from a paper called the inverse scaling. There's actually a contest to find are there certain tasks where as things get bigger and bigger, the performance gets worse. 


---


#### 00:42:03.431

And they found some of these tasks. One was called the hindsight neglect problem. I won't worry about the details, but basically across several generations, the models got worse at this task with increasing scale. And then within the next generation, it seems to have grokked that concept. And now it's perfect from being bad to worse to good. in a surprising way. So capabilities remain hard to predict. We know that we can scale things up. We know that the loss will get predictably better, but we don't know for any given task when this process of generalization will kick in. It's a surprise for all of the different tasks that we might be interested in. So this is a really profound challenge in terms of understanding what these systems are doing and also   
(00:42:47.092) ~~like~~ (00:42:47.253)  
how to control them. 


---


#### 00:42:49.760

Okay. I said that they're human level. They're definitely not human-like.   
(00:42:52.443) ~~Here's a,~~(00:42:52.663)  
just a quick, I won't even go into the details of this, but somebody went in and reverse engineered. Well, how is it learning to do modular addition? And it turns out it's doing it in a very weird way.   
(00:43:01.827) ~~It's doing,~~(00:43:02.349)  
it's like learning a sine and cosine functions and it's essentially rotating around the circle. No human would really do this way. It involves   
(00:43:10.713) ~~like~~ (00:43:10.893)  
Orye transform math. So it's a very alien process, but it does add up to a reliable algorithm. And now that this has been reverse engineered, you can actually see how it is doing it. You don't have to like it. 


---


#### 00:43:21.880

I think you should probably be a little bit scared of the fact that it's learning such alien solutions to these problems, but nevertheless, like this is what it does for this particular thing. So I really emphasize how, while they are very human-like in their abilities in some ways, they are also not at all human-like in their underlying mechanism, and we should not think of them as human-like where it really counts. Okay. Of course, these things are, here's the tail of the tape. This is important.   
(00:43:52.460) ~~What are the,~~(00:43:52.842)  
what are AIs good at? What are humans good at? AIs are much better at breadth. They thread all the information on the internet. They can speak all the languages. 


---


#### 00:44:00.530

Even human experts don't have anywhere the breadth of a modern AI, but the human experts do still have better depth, especially in their area of expertise. Breakthrough Insight is humanity's biggest edge right now.   
(00:44:12.331) ~~As I said earlier, few eureka moments,~~(00:44:14.092)  
precious few eureka moments. The AIs are a lot faster and they are a lot cheaper. Typically I would tell people that you can expect there'll be like at least 10 times faster and usually 90% cheaper if they can do what you need them to do. They're also   
(00:44:26.101) ~~like~~ (00:44:26.260)  
super paralyzable, super clonable.   
(00:44:28.802) ~~They're, you know,~~(00:44:29.362)  
ready whenever you are, you can pick up where you left off 24 seven. So they have   
(00:44:32.925) ~~like~~ (00:44:33.065)  
lots of availability advantages. 


---


#### 00:44:35.871

Memory is something that I've really come to appreciate in myself. My memory is certainly not perfect, but it does give me a coherent sense of who I am, what I'm trying to do. And the AIs don't have that in the same way. They have a very limited and brittle memory as it stands today. They do have great technology diffusion speed. A paper   
(00:44:52.795) ~~that I think~~(00:44:53.074)  
should give everyone a little pause is natural selection favors AIs over humans. The key thing there is that when an advance is made, it can often be ported to all the different architectures, all the different models very quickly. Whereas   
(00:45:04.539) ~~like~~ (00:45:04.699)  
we struggle to learn new things, especially as we get a little older. 


---


#### 00:45:08.184

Bedside manner is another one too, that AIs are actually eating humans on in evaluations. But they're really not good at adversarial robustness, meaning they're quite easy to trick. You can confuse them. You can trick them. This is sometimes known as jailbreaking. If you go on AI Twitter, you'll see lots of examples of people getting the AIs to make fools of themselves in ways that humans would never do. This is one of their main weaknesses. They're quite brittle and not really robust to being tricked. Okay. I know I'm going super long. I'm skipping over best practices for business. I'm going to do another talk on that actually tomorrow. And you might be able to check that out on my podcast feed if you're interested in that. 


---


#### 00:45:48.887

But just to cash this out a little bit to some investment advice, or I should say not investment advice, the Question that a friend of mine poses is, are we approaching a big tech singularity? The way that he defines that is a moment at which the big tech companies have such advantage because of their dominance in the core inputs to AI. Those are again, data, compute, and algorithms. Are we reaching a point where they might be able to enter into all sorts of different industries and dominate those new industries because of their core strength in AI and in the inputs to AI? And I would say that's looking increasingly plausible and certainly the stock prices of the big tech companies would seem to reflect that. 


---


#### 00:46:35.681

This is a chart of how much compute different companies in the world have. This is Google, Microsoft, Amazon, Meta across the top. Apple comes in at number five. Alibaba is the top entry out of China. And then things get like relatively small. And this is Oracle down here, by the way, which is a multi a hundred billion dollar company. But this is the compute. These are the dominant players in compute. The big four in compute today, Google, Microsoft, Amazon, Meta. Nobody else is on their level. And there's really no path for any company that's not already on this list to get into the compute game at anything approaching similar scale to what the big guys already have. 


---


#### 00:47:14.592

If you're prepared and able to spend billions to train a single AI model, it's going to be very hard for anyone to enter into that market and rival you. I don't pick stocks. I genuinely don't pick stocks, but I do have a little investment club with some friends of mine. And I've literally made one individual stock recommendation to the group all of history. And that was NVIDIA about two years ago, because I could just see where this was going, where everybody's saying, man, look at these scaling laws to compete. We're going to need to this compute budget at this given time, we're going to need to collect this amount of data. Of course, we're going to have to do a lot of research on the algorithms too, but   
(00:47:54.021) ~~you're not~~(00:47:54.442)  
the algorithms right now. are like incremental improvements. 


---


#### 00:47:58.164

Nobody has recently come up with an algorithm that just blows everything out of the water. You gotta have all three elements. You gotta have the data, you gotta have the compute, and you gotta have the algorithms. And so everybody's buying compute from the same place. That's NVIDIA.   
(00:48:09.539) ~~I think~~(00:48:09.940)  
all the chip makers are probably going to be doing pretty well. People are   
(00:48:14.827) ~~you know,~~(00:48:15.047)  
interested. NVIDIA is making insane margins, so people are very interested in like AMD and Intel as well. So the government is getting involved and saying, hey, maybe it's not such a good thing that this is all getting manufactured in Taiwan. Maybe we should bring some of it back to the United States. 


---


#### 00:48:28.536

But I would say that probably the safest bet in the space is the fundamental compute providers. both at the layer of manufacturing the chips, and then also at the big tech layer because they have all three. They have the data, the compute, and the AI researchers that are constantly working on new algorithms. This is my list of   
(00:48:50.603) ~~like~~ (00:48:50.764)  
live players. That is to say, who are the companies that really have a chance at shaping the future? And these are pretty familiar names at this point. OpenAI is the leader. Google still has the deepest bench in terms of the most researchers, the broadest research agenda. Anthropic is a real dark horse. They're not very big, but they're partnered with both Amazon and Google. 


---


#### 00:49:10.413

And there are a bunch of people that left OpenAI to found this new company. And that is certainly a big one. They're putting out a big open source model. You'll hear a lot about called Llama 3 right now and over the next few weeks. Microsoft is not quite as cutting edge in terms of research, but they've got it where it counts in terms of   
(00:49:24.967) ~~data sets or~~(00:49:26.047)  
data centers. And they're partnered with OpenAI. Never count out Elon.   
(00:49:30.512) ~~I think~~(00:49:30.733)  
Tesla and X will be interesting. A dark horse that is not a public company, you can't invest in it, but definitely one to watch is called Character AI. They basically make like AI girlfriends and people are spending a lot of time talking to their AI girlfriends. 


---


#### 00:49:44.302

So that's a whole other dimension of sort of societal impact. What's going to happen to the birth rate is I think a very interesting long-term question. Mistral is the European champion. They're based in France. I would say,   
(00:49:55.507) ~~you know,~~(00:49:56.188)  
they probably wouldn't have a chance at really competing except for the fact that the European Union may say,   
(00:50:02.951) ~~you know what,~~(00:50:03.371)  
here's a few billion dollars because we want to have one of these leaders on our soil. And the geopolitics of this are going to be very interesting to watch. Obviously, what's going on in China is a big deal as well.   
(00:50:15.635) ~~They're not as, uh,~~(00:50:16.994)  
they're not at the same level as the United States, but they're not too far behind. 


---


#### 00:50:21.097

Um, if you were to go to the big AI conference in New Orleans called NeurIPS a few months ago, I didn't actually personally attend, but I was told you heard a lot of Mandarin conversations on the floor. There are tons of talented Chinese researchers. A lot of them are here in the US, but also obviously a lot are in China. The chip ban, though, may be a big deal for them because they don't have their own domestic chip industry. And if they can't import the chips, they may have a hard time reaching those next levels of scale. Apple hopefully is going to make Siri good at some point, but   
(00:50:50.672) ~~I would say~~(00:50:50.891)  
they're currently behind, but   
(00:50:52.532) ~~they're,~~ (00:50:52.773)  
you can't count them out too much because   
(00:50:54.034) ~~they are,~~(00:50:54.494)  
look here on the list, they are the number five on compute and certainly they have more money than anybody could possibly know what to do with. 


---


#### 00:51:00.639

And that can pay a lot of researchers. All right, I'm gonna land the plane here in the next two minutes, and then I'll be happy to take a few questions. Sorry to go a little bit past my target. So are we all going to die is obviously a question that people are asking. I think that really depends on what happens next in terms of how much things scale and whether the scaling laws hold. They're called scaling laws, but they're not fundamental laws of nature   
(00:51:24.556) ~~that we, at least it doesn't,~~(00:51:25.677)  
we don't have that level of.   
(00:51:27.338) ~~um,~~ (00:51:27.478)  
justification for them and they would be better maybe described as scaling trends. And so the trend could break. 


---


#### 00:51:33.005

So are we going to see something where the sort of capabilities level off at a human expert level or do they just blow past human expert? I think that's probably the single biggest question and it's hotly debated. There's not really a clear answer there. My guess is that we're going to get something alien that'll be superhuman in some ways, but it'll still be weird and weak in other ways. And how that plays out is ultimately going to be weird and very hard to predict. One thing that I do think is strange though, is that we're racing into this without a real plan. Nobody really has a sense for how these systems are going to be controlled if they do become superhumanly powerful, even the leading developers. are specifically saying that it could lead to human extinction. 


---


#### 00:52:12.701

Samuel and the CEO of WebAI has said the worst case scenario is lights out for all of us. So it's bizarre that they're chasing this goal with seemingly as much speed as they can muster while they don't really have a plan to make sure that things don't go totally awry. The best I can say is at least they know that they're playing with fire. This is a survey of AI researchers that just goes to show how much radical uncertainty there is in the field. 48% of the respondents, these are people that had published in top journals in AI in the last few years, 48% of them gave at least a 10% chance of human extinction from AI. 


---


#### 00:52:51.077

So half gave a 10% chance. For my money, that is very much worth taking seriously. Tons of, and this is another thing, mitigating the risk of human extinction. This was signed by all the leaders. Sam Maltin, the CEO of OpenAI, the CEO of Eutropic, Bill Gates is on there, the chief scientist from OpenAI, the chief scientist from Google DeepMind, the CEO of Google DeepMind. These two are Turing Award winners, which is basically   
(00:53:13.612) ~~like~~ (00:53:13.733)  
the Nobel Prize in computer science. So it's really a who's who of people signing on to the idea that mitigating the risk of extinction from AI should be a global priority. There's just really radical uncertainty and all bets are really off, 


---


#### 00:53:24.960

I think, for how, how the future is going to shape up. How fast is this going to happen?   
(00:53:30.402) ~~Not that, not,~~(00:53:31.284)  
it's not that long of a time. The average,   
(00:53:34.125) ~~you know,~~(00:53:34.344)  
there's a couple of different ways you can ask the question, but the average among forecasters is like maybe in the next few years, maybe it's closer to eight to 10 years, who knows, but that's the range in which the field is expecting these breakthroughs. Of course, it may never happen, but the consensus view is like a few to a handful of years from now. And so what will we be watching to figure out where we're going from here? Will this raw scaling continue to work? 


---


#### 00:53:59.360

Will the scaling laws hold all the way to,   
(00:54:02.182) ~~sorry,~~ (00:54:02.422)  
to superhuman systems? That is very hotly debated. Will a new architecture come along and be even better than the transformer? Recent results suggest that yes, actually there will even be better architectures than the one that has taken us this far. Will mechanistic interpretability catch up? That's like the reverse engineering and figuring out what's actually going on inside. That was one thing that the survey of the 2000 AI researchers did ask, and the consensus was no, that we're not close enough to being able to understand what's going on inside to be able to count on that to save us, even though great progress is being made. 


---


#### 00:54:35.965

What new modalities will matter? You saw the DNA one earlier. I think there's going to be a lot of kind of immediately superhuman capabilities coming out of AI when it comes to things like modeling cells, reading brains, predicting the weather. This is the kind of stuff that humans just can't do. But we're already starting to see that AI systems can do it. And as soon as they can do it, they're pretty much immediately superhuman at it. Will these things start to become agentic? That means   
(00:55:02.858) ~~can they,~~(00:55:03.378)  
will they be able to have their own goals and pursue their plans over medium time horizons. That seems like a thing and a lot of people are working. 


---


#### 00:55:11.233

That's you might think, gee, that's crazy. We wouldn't want to turn these things into like independent ages. Well, I could point you to a hundred startups that are doing exactly that for all kinds of different use cases. Are these frontier labs, like your open AI's, your Google's, Anthropix, are they going to pause their research or stop scaling if things start to get scary?   
(00:55:30.313) ~~Well,~~ (00:55:30.512)  
they say they are.   
(00:55:32.273) ~~They've,~~ (00:55:32.534)  
they've signed that statement. They have other various policies they put in place, but will they follow through on that? Obviously we'll see. When will the government get involved? It's already starting to. I would expect a lot more focus on AI among not just the US government, but all sorts of governments around the world. 


---


#### 00:56:25.547

The hyperscaling, the scaling up of 10x and 100x paths where we've gone already is something that I think society would be wise to slow down on. Let's figure out what we have. Let's figure out how best to use it before we try to make something that is a superhuman AI scientist, because I don't think we have the strategies that we will ultimately need to keep that under control and to make sure it goes well for us. So I know we're at the hour again, sorry for going a little bit long, happy to stay a few extra minutes and take questions if that's in the cards. But if you want to find more from me elsewhere, all these different places are good places to find more. 


---


#### 00:57:03.164

And you can also contact me on my shiny new personal website, which Spigen just made for me. So thank you.   
(00:57:52.813) ~~I don't know if I, okay, I can see, but I don't know if I can grant. Yeah, you, I don't, can I do that? I don't think I can.~~(00:58:01.244)  
Lauren has a hand up, but I don't think I can enable.   
(00:58:36.806) ~~Thank you.~~(00:58:37.126)  
Yeah, I don't sugarcoat it. I'm definitely ambivalent about it all.   
(00:58:46.731) ~~I mean,~~(00:58:47.251)  
the classical sense of having strong competing and contradictory feelings. It is, I personally would say I am several times more productive than I was just a couple of years ago. In some of the areas, I'm not like a great software developer. 


---


#### 00:59:01.340

And in that area in particular, it saves me so much time to be able to go to AI and say, Hey, we're going to meet this little bit of code, do this, clean up this data. It's genuinely a several fold improvement in my personal productivity. So it's hard not to appreciate that. But yeah, at the same time, I do think we are very much playing with fire. Yes. Although it is generally considered to be a couple of years behind in some qualitative sense. I actually just did an episode of the podcast with a couple of researchers from Google in the robotics department. And the big challenge there is that   
(00:59:57.130) ~~they don't have,~~(00:59:58.150)  
they haven't yet pulled the same trick with robotics that they've pulled with language and an image and certain other things, right? 


---


#### 01:00:07.690

They don't have the equivalent of, here's all the text on the internet, your job is to predict the next word. There's no data set that's, here's what the robot actually did, or even here's what the human actually did physically. That data doesn't exist to be tapped into. So they're working on that problem first. How do they scale the data so that they can then train similar scaled models to do things. And they're making remarkable progress. There are various techniques in terms of imitating humans. They've got also interesting techniques   
(01:00:38.067) ~~like.~~ (01:00:38.246)  
have the robots do stuff, but then they get to a thing that they can't do. They, this could even be like in your home, perhaps, right? 


---


#### 01:00:45.833

Like you can imagine your domestic servant robot. I'm certainly ready for one that would pick up my kid's toys. I made it do the dishes or whatever. But when it gets to the point that it can't do it, then the idea would be like, it kind of phones home and a human tele operator actually does the task and shows the robot what to do based on the human intuitive understanding. And then that data feeds into the overall program for future training. That's how Tesla is also doing their driving.   
(01:01:11.293) ~~It's like the~~(01:01:12.492)  
they're recording what the human drivers are doing and training the AIs on that. And the big thing, and that's why they're at least one of the leaders. 


---


#### 01:01:20.715

Because again, that data just didn't exist, right? For the longest time that we've been driving around cars, like nobody's been capturing what was around the car. How did somebody act? That's Tesla's created that dataset for themselves. Google with Waymo has done something similar. Yeah, I just heard that   
(01:01:42.599) ~~the, it's a little bit hard to parse some of these data points, but~~(01:01:47.503)  
from a pretty credible source and I've used the Tesla full self driving a little bit, a neighbor who works at Tesla was based at the one being one. And it is extremely impressive. Not without some rough spots still, but according to what I just heard, the Tesla internal data says that there are 10 times safer than human already. 


---


#### 01:02:08.719

But there are some weirdness, weird parts to that analysis where if the AI decides that it can't handle a certain situation, then it will tell the human that it has to drive. And so you have this sort of handoff question of, well, wait, who's really at fault here? If the AI decided it couldn't handle a situation and take it back to the human and then the human got in trouble. Sounds like the AI was already doing something wrong. So I think you could take that 10 X safer with a non-trivial green assault. But I would say even if you did, it sounds like they're basically as safe as humans right now. That's really an important point too. 


---


#### 01:02:46.681

I think in a lot of AI application and questions in general, the what are you comparing to is a really important question. Often people compare to some imaginary perfection. And we don't really generally have that available to us in the real world. Comparing to what is.   
(01:03:05.579) ~~Like, I mean,~~(01:03:06.920)  
Ethan Moller is a professor at Wharton who I think is really good on this. He'd been even ahead of me. He's the person that I would recommend following most for ongoing analysis of AI. He says, you want to compare to the best available human. And what that is is   
(01:03:20.625) ~~like~~ (01:03:20.764)  
very different and   
(01:03:21.525) ~~very,~~ (01:03:21.724)  
very different contexts, but human performance is definitely not flawless across any domain of interest. 


---


#### 01:03:41.829

I don't see any more. Thanks, guys. 


---



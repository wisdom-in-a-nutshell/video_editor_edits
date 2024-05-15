#### 00:00:00.109

Amelie Schreiber, computational biochemist and AI researcher. Welcome to the Cognitive Revolution. Nice to be here. I'm excited for this conversation. I expect to learn a lot from it. This all started with a tweet that I saw you put out where you said, here are my top 10 AI tools for biology. And I read down the list and I was like, I don't know what any of these are. So   
(00:00:23.425) ~~I think~~(00:00:23.626)  
pretty much immediately just say, Hey, would you be interested in educating me in the form of a podcast? So I appreciate you taking the time. You want to start off by just giving a little bit of context on who you are, what you're doing day to day and what kinds of problems you're trying to solve. 


---


#### 00:00:36.149

Yeah, sure. I'm an AI researcher and I focus on computational biochemistry applications. I actually started out as a mathematician. My training in grad school was in mathematics, actually. Started off with pure mathematics and then transitioned into applied mathematics and data analysis. And then after grad school, I got into deep learning and started working on more AI related things. For me, the biochemistry applications are one of the most compelling things that we could be working on right now.   
(00:01:02.176) ~~I think~~(00:01:02.436)  
other than   
(00:01:03.576) ~~like~~ (00:01:03.737)  
AGI, whatever that means, I think it's probably the most important problem we can be working on because it's a huge impact on human health. the applications are really profound and have the potential to be very impactful for everyone. 


---


#### 00:01:17.995

So I get really excited about the biochemistry applications of AI. I have some projects and things that I'm working on that are more related to environmental things and material science type applications, but Primarily I focus on the medical or biomedical aspect of things. Okay, so let me try to give a extremely high level understanding of a couple of the biggest problems that are being studied in biomedical sciences. As I was preparing for this, I was having a good conversation with CLOB3 about it. And I came away with the understanding that both at the level of an individual cell, and then again, at the level of the overall organism system, We have one really massive challenge, which is that we don't know how it works. 


---


#### 00:02:06.777

We've got the DNA, which is the code, the RNA, which is both messenger, but also is a machine. The proteins are all machines that fold up in weird ways and interact with each other in three-dimensional space. And then you've got the small molecules as well, which are like signaling, but also if they fit right,   
(00:02:26.073) ~~you know,~~(00:02:26.233)  
all these puzzle pieces fit together in super strange ways. There's this incredible network of interactions where things are disabling each other or promoting each other or interacting in all sorts of complicated ways. The nature of those interactions initially was entirely unclear. And now humanity at large has embarked on this grand project of trying to figure out how do cells work and how do our bodies work. 


---


#### 00:02:47.169

And I'm gathering we're like maybe five to 10% of the way there. Most of the interactions remain unknown to us, but we've at least mapped out a decent chunk. So the first challenge, if you're trying to solve a disease is figure out what is the pathway? What is the interaction in this   
(00:03:03.596) ~~like~~ (00:03:03.795)  
super complicated thing that is going wrong? And then the second challenge is if I know what is going wrong, can I do something to intervene to stop it? But then again, there could be a lot of other knock-on effects. And in that way, there's an important commonality with large language models. These things are not super clean. In language models, people are probably familiar with the notion of superposition, which is one activation in a network. can light up for multiple different reasons. 


---


#### 00:03:31.282

And we certainly see all of these kind of patterns of complexity in biology as well. But we know that there's a lot of stuff going on. There's a lot of interactions that are happening. We don't really know a lot about that, but we're gradually learning more all the time. And then if you do have a target, now it's okay. These are all three-dimensional spatial things. And so it's just   
(00:03:57.242) ~~extremely,~~ (00:03:57.622)  
extremely difficult.   
(00:03:59.283) ~~It is.~~(00:03:59.604)  
Yeah. How am I doing there in terms of just setting a foundation to understand the challenges?   
(00:04:05.074) ~~I think~~(00:04:05.275)  
you've really hit the nail on the head. I work with a lot of different kinds of molecules. So small molecules, which are your drugs that you take in like a pill form, these are smaller than proteins and less complicated. 


---


#### 00:04:17.978

And I also work with proteins and also a little bit with DNA and RNA. And understanding protein interaction networks is a very difficult and complex problem. To just determine whether or not two proteins interact with each other, already is a hard problem. And then modeling how they fit together when they do interact and understanding the strength and how transient that interaction might be, it's very difficult. So protein interactions especially, but also protein DNA, protein RNA, and protein small molecule interactions are all very complicated things to model. There are some new ways to address this that have come out recently   
(00:05:00.321) ~~that I have a lot of hope for,~~(00:05:01.982)  
that I think are very promising and very effective approaches. 


---


#### 00:05:05.004

I use various kinds of AI tools, analyze these molecules, create new ones, modify them. engineer them in ways, grafting them together and stuff, performing complicated operations on these molecules so that they perform a particular kind of function. As an example, designing a new protein to bind to another protein so that you can cause some kind of cascade event in a protein interaction network, or so that you can block certain interactions between proteins. A really good example in cancer, your basic first examples of a mechanism of cancer, There's PD-1 and PD-L1. These are two proteins. One of them's located in the cancer and one of them's located on your immune cells. What happens is these two proteins end up binding to each other and essentially the cancer turns off your immune cell so that your immune cell doesn't attack the cancer. 


---


#### 00:06:00.994

And that's not good, right? You don't want this kind of interaction between these two proteins because you want your immune system to recognize the cancer and destroy it. Having this interaction turns off your immune system in a very specific way. So you can do things like design binders to this protein to block that interaction and that can help you combat cancer and hopefully treat it. And that's just one basic example of something that you can do with these tools that I'm using and that I'm interested in. You can also design new drugs with them. You can design drugs that are specific to a particular binding pocket on a protein. You can design drugs that have very specific chemical properties. 


---


#### 00:06:40.845

You can design proteins that have very specific chemical and functional properties. And this is pretty new stuff, but you can also do a lot of the same things with DNA and RNA molecules as well. Okay. This is a paradigm shift, right? The application of AI to biology, obviously the AI is creating all sorts of paradigm shifts, but   
(00:06:59.286) ~~I think~~(00:06:59.446)  
it might also be helpful for people to understand a little bit better of the before state when we didn't have any of these tools yet, which is not that long ago. Not that long ago. Yeah. What was the sort of prevailing approach to figuring stuff out? You hear these stories of, oh, look, we found this frog in the rainforest that is immune to a certain disease. 


---


#### 00:07:21.487

What's going on there? Let's see if we can't find something in this frog 
0.129
  
Amelie Schreiber, computational biochemist and AI researcher. Welcome to the Cognitive Revolution. Nice to be here. I'm excited for this conversation. I expect to learn a lot from it. Quick context on my end. This all started with a tweet that I saw you put out probably two months ago now. where you said, here are my top 10   
(20.33) ~~tools,~~ (20.77)  
top 10 AI tools for biology in no particular order. And I read down the list and I was like, I don't know what any of these are. So when that happens, I'm immediately like, okay, this is an area that I need to do some remedial self-education in. And reached out,   
(37.215) ~~I think~~(37.415)  
pretty much immediately to say, hey, would you be interested in educating me in the form of a podcast? 
---
41.797
  
So I appreciate you taking the time to prepare for this and do it. You want to start off by just giving a little bit of context on who you are, what you're doing day to day and what kinds of problems maybe you're trying to solve. And then we can step back again and give people   
(54.933) ~~kind of~~(55.133)  
foundational knowledge. Yeah,   
(57.069) ~~sure. Yeah,~~(57.67)  
I'm an AI researcher and I focus on computational biochemistry applications. I actually started out as a mathematician. My training in grad school and stuff was in mathematics, actually. Started off with pure mathematics and then transitioned into applied mathematics and data analysis type stuff. And then after grad school, I got into the deep learning stuff and started working on more AI related things. 
---
80.305
  
Yeah, I think, and for me, like the biochemistry applications are one of the most compelling things that we could be working on right now. I think other than   
(89.093) ~~like~~ (89.233)  
AGI, whatever that means, I think it's probably the most important problem we can be working on because it's a huge impact on human health. The applications in human health and medical applications are really profound and have the potential to be very impactful and for everyone too. So I get really excited about the biochemistry applications of AI. And yeah,   
(112.857) ~~I guess~~(113.117)  
that's a little about me. Was there anything in particular that you wanted to know about my background or experience? Maybe just the context that you're working in today a little bit would be helpful to understand how it is that you're exploring these tools and applying them. 
---
124.804
  
Obviously, again, we're going to have to get into more detail on what they are, but yeah, just   
(129.367) ~~kind of~~(129.587)  
where in the world are you situated that you're doing all this stuff?   
(133.309) ~~So, I mean,~~(133.75)  
I work on mostly applications in biochemistry related to human health. I have some projects and things that I'm working on that are more related to   
(143.963) ~~like~~ (144.103)  
environmental things and material science type applications, but Primarily I focus on the medical or biomedical aspect of things. That's what I'm most interested in. I work with a lot of different kinds of molecules. So small molecules, which are like your drugs that you take in like a pill form or something, right? These are smaller than proteins and less complicated. 
---
167.406
  
And I also work with proteins and also a little bit with DNA and RNA. And I use various kinds of AI tools, analyze these molecules, create new ones, modify them, engineer them in ways, grafting them together and stuff, performing complicated operations on these molecules to get particular kinds of functions out of them so that they perform a particular kind of function. And as an example, designing a new protein to bind to another protein so that you can cause some kind of cascade event in a protein network, in a protein interaction network, or so that you can block certain interactions between proteins. A really good example in cancer, there's two proteins that come up that are like your basic first examples of like a mechanism of cancer. 
---
217.838
  
So there's PD-1 and PD-L1, and these are two proteins. One of them's located in the cancer, and one of them's located on your immune cells. And what happens is these two proteins end up binding to each other, and essentially the cancer turns off your immune cell so that your immune cell doesn't attack the cancer. And this is an interaction that's not good, right? You don't want this kind of interaction between these two proteins because you want your immune system to recognize the cancer and destroy it. And having this interaction turns off your immune system in a very specific kind of way. So you can do things like design binders to this protein, to one of these two proteins to block that interaction. 
---
260.853
  
And that can help you like combat cancer and hopefully treat it. And that's just one basic example of something that you can do with these tools that I'm using and that I'm interested in. You can also design new drugs with them. You can design drugs that are specific to a particular binding pocket on a protein. You can design drugs that have very specific chemical properties. You can design proteins that have very specific chemical and functional properties. And you can also modify DNA and RNA now. This is pretty new stuff, the DNA and the RNA. You can also do a lot of the same things with DNA and RNA molecules as well. Okay. So let me take a super zoom out for one second and try to give a extremely high level understanding as I have it today for   
(307.736) ~~kind of~~(308.016)  
a couple of the biggest sorts of problems that I understand are being studied in biomedical sciences. 
---
316.839
  
And you can then refine that and then   
(318.06) ~~we'll,~~ (318.26)  
we'll get back down into the lower levels of like specific problems and tools to solve that.   
(323.802) ~~I guess.~~(323.982)  
As I was preparing for this, I was having a good conversation with CLAWB3 about it. And I kind of came away with the understanding that there are two,   
(334.34) ~~I mean,~~(335.581)  
there's a lot of different layers, right? There's a lot of different levels of abstraction, which also kind of correspond to the scale of the thing that you're studying. And both at the level of an individual cell, and then again, at the level of the overall organism system, It seems that we have one really massive challenge, which is that we don't know how it works. 
---
356.993
  
And in that way, there's an important commonality with the large language models that is like the most common topic on this podcast. But we sort of know that there's a lot of stuff going on and there's a lot of interactions that are happening. the nature of those interactions initially was entirely unclear. And now humanity at large has embarked on this grand project of trying to figure out how do cells work and how do our bodies work at a higher level. And it seems like we're   
(384.049) ~~maybe like,~~(384.689)  
not to be too specific with the number, but   
(387.171) ~~you know,~~(387.391)  
I'm gathering we're like maybe five to 10% of the way there, where most of the interactions remain unknown to us, but we've at least mapped out like a pretty decent chunk. 
---
399.719
  
So the first challenge, if you're trying to solve a disease, as I understand it, is figure out what is it? What is the pathway? What is the interaction in this super complicated thing that is going wrong? And then the second challenge is, if I know what is going wrong, can I do something to intervene to stop it? But then again,   
(418.662) ~~I have a lot of,~~(419.582)  
right now we have a lot of dark matter, dark energy in terms of, I may be able to affect that one thing, but there could be a lot of other knock-on effects. Another sort of commonality is these things are not super clean. In language models, people are probably very familiar with the notion of superposition, which is like one neuron, one activation in a network, can light up for multiple different reasons. 
---
440.834
  

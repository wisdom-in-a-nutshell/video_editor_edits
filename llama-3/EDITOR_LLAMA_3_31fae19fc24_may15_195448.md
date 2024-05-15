#### 00:00:00.129

Amelie Schreiber, computational biochemist and AI researcher. Welcome to the Cognitive Revolution. Nice to be here. I'm excited for this conversation. I expect to learn a lot from it. Quick context on my end. This all started with a tweet that I saw you put out probably two months ago now. where you said, here are my top 10   
(00:00:20.329) ~~tools,~~ (00:00:20.769)  
top 10 AI tools for biology in no particular order. And I read down the list and I was like, I don't know what any of these are. So when that happens, I'm immediately like, okay, this is an area that I need to do some remedial self-education in. And reached out,   
(00:00:37.215) ~~I think~~(00:00:37.414)  
pretty much immediately to say, hey, would you be interested in educating me in the form of a podcast? 


---


#### 00:00:41.796

So I appreciate you taking the time to prepare for this and do it. You want to start off by just giving a little bit of context on who you are, what you're doing day to day and what kinds of problems maybe you're trying to solve. And then we can step back again and give people   
(00:00:54.932) ~~kind of~~(00:00:55.133)  
foundational knowledge. Yeah,   
(00:00:57.069) ~~sure. Yeah,~~(00:00:57.670)  
I'm an AI researcher and I focus on computational biochemistry applications. I actually started out as a mathematician. My training in grad school and stuff was in mathematics, actually. Started off with pure mathematics and then transitioned into applied mathematics and data analysis type stuff. And then after grad school, I got into the deep learning stuff and started working on more AI related things. 


---


#### 00:01:20.305

Yeah, I think, and for me, like the biochemistry applications are one of the most compelling things that we could be working on right now. I think other than   
(00:01:29.093) ~~like~~ (00:01:29.233)  
AGI, whatever that means, I think it's probably the most important problem we can be working on because it's a huge impact on human health. The applications in human health and medical applications are really profound and have the potential to be very impactful and for everyone too. So I get really excited about the biochemistry applications of AI. And yeah,   
(00:01:52.856) ~~I guess~~(00:01:53.117)  
that's a little about me. Was there anything in particular that you wanted to know about my background or experience? Maybe just the context that you're working in today a little bit would be helpful to understand how it is that you're exploring these tools and applying them. 


---


#### 00:02:04.804

Obviously, again, we're going to have to get into more detail on what they are, but yeah, just   
(00:02:09.366) ~~kind of~~(00:02:09.586)  
where in the world are you situated that you're doing all this stuff?   
(00:02:13.308) ~~So, I mean,~~(00:02:13.750)  
I work on mostly applications in biochemistry related to human health. I have some projects and things that I'm working on that are more related to   
(00:02:23.962) ~~like~~ (00:02:24.103)  
environmental things and material science type applications, but Primarily I focus on the medical or biomedical aspect of things. That's what I'm most interested in. I work with a lot of different kinds of molecules. So small molecules, which are like your drugs that you take in like a pill form or something, right? These are smaller than proteins and less complicated. 


---


#### 00:02:47.406

And I also work with proteins and also a little bit with DNA and RNA. And I use various kinds of AI tools, analyze these molecules, create new ones, modify them, engineer them in ways, grafting them together and stuff, performing complicated operations on these molecules to get particular kinds of functions out of them so that they perform a particular kind of function. And as an example, designing a new protein to bind to another protein so that you can cause some kind of cascade event in a protein network, in a protein interaction network, or so that you can block certain interactions between proteins. A really good example in cancer, there's two proteins that come up that are like your basic first examples of like a mechanism of cancer. 


---


#### 00:03:37.837

So there's PD-1 and PD-L1, and these are two proteins. One of them's located in the cancer, and one of them's located on your immune cells. And what happens is these two proteins end up binding to each other, and essentially the cancer turns off your immune cell so that your immune cell doesn't attack the cancer. And this is an interaction that's not good, right? You don't want this kind of interaction between these two proteins because you want your immune system to recognize the cancer and destroy it. And having this interaction turns off your immune system in a very specific kind of way. So you can do things like design binders to this protein, to one of these two proteins to block that interaction. 


---


#### 00:04:20.853

And that can help you like combat cancer and hopefully treat it. And that's just one basic example of something that you can do with these tools that I'm using and that I'm interested in. You can also design new drugs with them. You can design drugs that are specific to a particular binding pocket on a protein. You can design drugs that have very specific chemical properties. You can design proteins that have very specific chemical and functional properties. And you can also modify DNA and RNA now. This is pretty new stuff, the DNA and the RNA. You can also do a lot of the same things with DNA and RNA molecules as well. Okay. So let me take a super zoom out for one second and try to give a extremely high level understanding as I have it today for   
(00:05:07.735) ~~kind of~~(00:05:08.016)  
a couple of the biggest sorts of problems that I understand are being studied in biomedical sciences. 


---


#### 00:05:16.838

And you can then refine that and then   
(00:05:18.060) ~~we'll,~~ (00:05:18.259)  
we'll get back down into the lower levels of like specific problems and tools to solve that.   
(00:05:23.802) ~~I guess.~~(00:05:23.982)  
As I was preparing for this, I was having a good conversation with CLAWB3 about it. And I kind of came away with the understanding that there are two,   
(00:05:34.339) ~~I mean,~~(00:05:35.581)  
there's a lot of different layers, right? There's a lot of different levels of abstraction, which also kind of correspond to the scale of the thing that you're studying. And both at the level of an individual cell, and then again, at the level of the overall organism system, It seems that we have one really massive challenge, which is that we don't know how it works. 


---


#### 00:05:56.992

And in that way, there's an important commonality with the large language models that is like the most common topic on this podcast. But we sort of know that there's a lot of stuff going on and there's a lot of interactions that are happening. the nature of those interactions initially was entirely unclear. And now humanity at large has embarked on this grand project of trying to figure out how do cells work and how do our bodies work at a higher level. And it seems like we're   
(00:06:24.048) ~~maybe like,~~(00:06:24.689)  
not to be too specific with the number, but   
(00:06:27.170) ~~you know,~~(00:06:27.391)  
I'm gathering we're like maybe five to 10% of the way there, where most of the interactions remain unknown to us, but we've at least mapped out like a pretty decent chunk. 


---


#### 00:06:39.718

So the first challenge, if you're trying to solve a disease, as I understand it, is figure out what is it? What is the pathway? What is the interaction in this super complicated thing that is going wrong? And then the second challenge is, if I know what is going wrong, can I do something to intervene to stop it? But then again,   
(00:06:58.661) ~~I have a lot of,~~(00:06:59.581)  
right now we have a lot of dark matter, dark energy in terms of, I may be able to affect that one thing, but there could be a lot of other knock-on effects. Another sort of commonality is these things are not super clean. In language models, people are probably very familiar with the notion of superposition, which is like one neuron, one activation in a network, can light up for multiple different reasons. 


---


#### 00:07:20.834

And we certainly see all of these kind of patterns of complexity in biology as well. I'm kind of casting this into two levels. Tell me if you would refine this or change my thinking. But first is, man, there's this incredible network of interactions where things are disabling each other or promoting each other or interacting in all sorts of complicated ways. And we don't really know a lot about that, but we're gradually learning more all the time. And then if you do have a target, now it's okay. These are all three-dimensional spatial things. I'm not even sure if we should think of them as   
(00:07:54.463) ~~like~~ (00:07:54.622)  
classically 3D objects or if we should think of them more as sort of quantum distributions. 


---


#### 00:08:01.524

And maybe that varies depending on exactly what we're talking about. But we've got like the DNA, which is the code, the RNA, which is both like messenger, but also is like a machine. The proteins are all machines that fold up in weird ways and interact with each other in three dimensional space. And then you've got the small molecules as well, which are   
(00:08:23.177) ~~kind of~~(00:08:23.377)  
like signaling, but also if they fit right into all these puzzle pieces fit together in super strange ways. And so it's just extremely difficult.   
(00:08:32.639) ~~It is, yeah.~~(00:08:33.299)  
How am I doing there in terms of just setting a foundation to understand the challenges? So   
(00:08:38.442) ~~you've really,~~(00:08:38.962)  
I think you've really hit the nail on the head. 


---


#### 00:08:41.604

So protein interactions, especially, but also protein DNA, protein RNA, protein small molecule interactions are all very complicated things to model. And being able to predict when there's an interaction between two of these molecules and actually model that interaction correctly is a really hard problem. And I would say understanding protein interaction networks to start with,   
(00:09:05.955) ~~and we can talk about other kinds of interactions as well,~~(00:09:08.235)  
but understanding protein interaction networks is a very difficult and complex problem. And there are some new ways to address this that have come out recently that I have a lot of hope for, that I see them, and I think that these are very promising approaches and very effective approaches. So to just determine whether or not two proteins interact with each other, already, just two proteins interacting with each other, is a hard problem. 


---


#### 00:09:35.250

And then modeling how they fit together when they do interact, and understanding the strength and how transient that interaction might be, it's very difficult. And so we have tools to model these things now. They only have come out very recently, like within the last year or two. So for example, AlphaFold2 was a big deal, right? And that came out a couple of years ago. And   
(00:10:00.421) ~~you can model,~~(00:10:01.721)  
I think the way to think about it is you can model a very low energy confirmation of the protein. It's not necessarily like the ground state or the lowest energy confirmation, but ideally it's one of the lowest energy confirmations, if not the lowest. But you just get a single static structure from AlphaFold2. 


---


#### 00:10:21.416

So we give it the protein sequence, which is just a sequence of amino acids, which are represented by 20 letters. and it takes in this protein sequence, it computes something called a multiple sequence alignment or an MSA, and it provides you with a static structure for that protein that's a low energy confirmation for that protein. But that protein could exist in other confirmations. It might have other states that it exists in when it's interacting with other proteins or based on the environment that it's in, what temperature it is, things like this. can change the shape of the protein,   
(00:10:58.666) ~~right?~~ (00:10:58.806)  
They move around, they're very jiggly, and they do things. And so people have been trying to address this and model what's called the Boltzmann distribution of proteins. 


---


#### 00:11:11.274

And the Boltzmann distribution is something from statistical mechanics that tells you all the different conformations and what probabilities there are associated to those different conformations. And having a way to sample the Boltzmann distribution and get all of these different confirmations out of them. And also understanding the transitions between these states is a really difficult problem. And there's actually a model that we'll talk about later that does a really good job of addressing this that just came out middle of last year. It's called distributional graph former. And we'll talk about that a little bit later. And that's one of the generalizations of, it's not really a generalization of AlphaFold2's architecture, but it's a generalization of the idea that AlphaFold2 is implementing, right? 


---


#### 00:11:57.470

It's not just a single static structure anymore. It's actually a whole ensemble of structures and also the transition pathways between those different metastable states. And being able to model this and understand more   
(00:12:12.394) ~~like~~ (00:12:12.575)  
the dynamics of the proteins is something that people have been thinking about pretty hard for the last couple of years. And we're just starting to get tools that actually address this problem. And that's a really good thing because traditionally the way that this sort of thing was approached was through something called molecular dynamic simulations. And molecular dynamic simulations, they come in a lot of different flavors and they come in a lot of different complexities. Some of them model the proteins using just standard Newtonian physics, and then you can add in more complexity on top of that and add in things like quantum properties and other features of the protein to make the molecular dynamics simulation more complex and more robust. 


---


#### 00:12:54.476

But these simulations, they are really computationally intensive. They take a long time, they take a lot of GPUs, and they're just not very efficient. And on top of that, The length of time that you run your simulation for really, in a lot of cases, determines how accurate your distribution is and how accurate the confirmations or trajectories that you get out of that are. And you might run your simulation and not run it for long enough, and you don't get all the different states that the protein might be in, but you miss some of them, right? There are some new AI models that are trying to address this and trying to make headway into augmenting or even replacing molecular dynamic simulations in a lot of cases. 


---


#### 00:13:44.078

And this is really good because we need things that are more computationally efficient so that we can do this for a lot of proteins, right? Because we have a lot of proteins to do this for. And distributional graph former. is addressing a lot of this. And it does a pretty good job of doing it too. There's some room for improvement for sure, but it's a pretty solid model. And some really respectable people that I have a lot of respect for in this area have worked on this. And some of the inspiration comes from diffusion models. So it's a diffusion model similar to   
(00:14:20.490) ~~like~~ (00:14:20.630)  
DALI, which most of your watchers are probably familiar with, but it works on proteins instead of images. 


---


#### 00:14:27.144

And it also takes some inspiration from an area that is trying to solve this problem in a slightly different way called Boltzmann generators. And we can discuss that a little bit. I don't want to spend too much time on the Boltzmann generators, but it's influenced by some of those ideas and trying to sample the Boltzmann distribution of the proteins or protein complexes even or protein small molecule complexes and getting a handle on something that's more like the dynamics of the protein and getting a good representation of all the different metastable states that the protein might exist in at low energies.   
(00:15:02.870) ~~Okay, let me,~~(00:15:03.730)  
can we take one step back again? Sure. I think this is a paradigm shift, right? 


---


#### 00:15:08.572

The application of AI to biology, obviously the application of AI to just about everything is creating all sorts of paradigm shifts, but   
(00:15:14.534) ~~I think~~(00:15:14.696)  
it might also be helpful for people to understand a little bit better of the before state of   
(00:15:22.379) ~~like~~ (00:15:22.600)  
when we didn't have any of these tools yet, which is not that long ago. Not that long ago, yeah. What was the sort of prevailing approach to figuring stuff out and a little bit of just what is the biotech stack on which all this is built? I'm under the impression that The techniques available to us in many cases were like relatively primitive in the sense of you hear these stories of, oh look, we found this frog in the rainforest that like is immune to a certain disease. 


---


#### 00:15:52.562

Like what's going on there? Let's see if we can't find something in this frog that doesn't exist anywhere else. And then maybe that could be a medicine or whatever.   
(00:15:58.764) ~~It's like~~(00:15:58.965)  
really   
(00:15:59.404) ~~sort of~~(00:15:59.725)  
anecdotally sort of special observation motivated investigations in a lot of cases. And then I know there's also just a lot of   
(00:16:08.787) ~~like,~~ (00:16:08.986)  
historically brute forcing, basically, as I understand it, where it's, okay, look,   
(00:16:13.429) ~~let's,~~ (00:16:13.590)  
we have no idea which proteins are going to interact with which other ones. So let's just create this massive cross matrix and see if we can't figure it out that way. And look for hits, kind of massive essays of just exploring the space.   
(00:16:25.879) ~~I mean,~~(00:16:26.078)  
sure, it's a little bit smarter than that, but all of these things without the ability to really have any idea of what the puzzle pieces actually look like, which makes it obviously very difficult to figure out how they would fit together. 


---


#### 00:16:39.239

What more would you tell people who just want to understand, okay, what was the before, before all this stuff started to come online? So   
(00:16:46.304) ~~computationally, like~~(00:16:47.546)  
on the computational aspect of, or the computational side of things, I think the prevailing methods that were the most advanced were molecular dynamic simulations. And people still use those.   
(00:16:57.614) ~~And And~~(00:16:59.392)  
this is like physics. This is F equals ma, modeling, electro, electronic interactions, all this kind of, but just very like simple physics equations played out in many steps. Exactly. And so you have what's called a potential, right? and this potential tells you how the dynamics evolve. Like I was saying before, there are different levels of complexity of MD simulations, and there are some different flavors. 


---


#### 00:17:27.380

There's just standard molecular dynamics simulations, but you also have coarse-grained, and you also have different levels of complexity of how you're modeling the interactions and the forces between the particles. The most basic approach that you could take is just standard Newtonian mechanics.   
(00:17:42.051) ~~right?~~ (00:17:42.272)  
No quantum physics, no extra information about anything, just standard Newtonian physics. And then you can add stuff on top of that to get increasing complexity and accuracy. And so molecular dynamics simulations is definitely an in some cases still is the prevailing methodology on the computational side of things. And then also just using things like MSAs and some like machine learning models that arose in the last,   
(00:18:09.813) ~~I don't know,~~(00:18:10.153)  
decade or so are POTS models. 


---


#### 00:18:12.433

So POTS models are also used, but those are like really specific sort of models. They're not very generalizable. And then on   
(00:18:20.599) ~~like the,~~(00:18:21.319)  
there's also a lot of methods that come from wet lab work where people do this stuff in animals. Like they say you want to do directed evolution on a protein and try to find higher functioning variants or variants that are more thermostable that have higher expression or something like that. You can mutate these things in a lab and   
(00:18:45.467) ~~sort of~~(00:18:45.787)  
you can do like point mutations or you can do two mutations at a time or you can do like multiple. But when you start adding in things higher than just single point mutations, you get this combinatorial complexity, right? 


---


#### 00:19:00.001

And so it gets really unwieldy. It feels like maybe not the most principled way to do it. I don't know. I don't want to trash people who are doing the lab work because the lab work is really important. But doing directed evolution in a lab, in a lot of ways, now that we have AI tools to do similar things, feels a little bit unnecessary. Why do we need to go and inject an animal and wait some amount of time for this to play out inside the animal and then actually synthesize these things by hand in a lab somewhere. When we can   
(00:19:34.068) ~~like~~ (00:19:34.249)  
do very similar things, computing and often get better results. So like a good example of how AI has   
(00:19:42.791) ~~sort of~~(00:19:43.031)  
replaced this directed evolution methodology that comes out of like wet lab methods. 


---


#### 00:19:48.953

There are directed evolution AI models that you can use like protein language models to do directed evolution. You can also do a sequence redesign with things like protein MPNN or ligand MPNN, which allows you to redesign parts of the protein sequence or the entire protein sequence under some constraints, maybe under some certain specific chemical constraints, or you might want to bias the residues towards or away from certain amino acids and things like that. But these AI tools allow you to do that computationally and they do it really fast,   
(00:20:26.594) ~~right? I mean,~~(00:20:27.234)  
like I can design a sequence for a protein in a few seconds with   
(00:20:31.395) ~~like~~ (00:20:31.537)  
ligand and PNN on my computer with no special hardware or anything. 


---


#### 00:20:36.118

I don't even need a fancy GPU to do it. And I can do that many times and get lots of variants for my protein. and assess them computationally. And very often these variants that you get out of this process are much higher performing than   
(00:20:53.459) ~~like~~ (00:20:53.618)  
the wild type or than what you would get by doing this in a wet lab. But yeah, so   
(00:20:59.540) ~~I guess~~(00:20:59.780)  
hopefully that gives you some idea of some of the methods that they still are being used. It's not like these have just gone the way of the dodo and disappeared or something, but they have their place for sure. But   
(00:21:12.023) ~~I think~~(00:21:12.403)  
computational approaches are proving to be much faster, much more effective, and you can scale them, which is really important because we're working sometimes with millions or hundreds of millions of proteins, having millions of variants of a protein and being able to assess them and determine their quality in some some metric has become a lot easier in the past couple of years even. 


---


#### 00:21:38.598

Like protein and PNN only came out a couple of years ago. It hasn't even really had time to really catch on in a lot of places. Like people are still learning about these tools and still adopting them. Yeah. Was there like any particular area of the history that you wanted to touch on? Because I feel like my experience with traditional methods is somewhat limited. I don't come from a wet lab background. I come from a very computational background. And because I started off working in the AI, I also haven't spent a lot of time working with MD simulations or other more traditional methods that people have used. historically. Nothing super specific. I'm really just trying to get a... 


---


#### 00:22:22.551

I'm early in my journey of understanding all of this. So I'm trying to get the high level paradigms first and then spiking down just   
(00:22:28.739) ~~kind of~~(00:22:28.979)  
almost randomly into different areas to get a mix of the broad survey, but then try to go deep on a couple of technical things to understand some of the techniques in a more precise way.   
(00:22:39.840) ~~I think~~(00:22:40.161)  
because the AI techniques are so new, most people working on them are still developing their own understanding of all of this. It's such a new paradigm. It's such a new methodology. There aren't very many people who are experts on this stuff.   
(00:22:56.205) ~~I think~~(00:22:56.405)  
we're all   
(00:22:56.766) ~~kind of~~(00:22:57.026)  
learning together, even me. I'm definitely still learning a lot of stuff from my coworkers and other researchers in the field. it's kind of mind blowing how fast this stuff is developing too. 


---


#### 00:23:09.854

It's developing incredibly fast, which is really good in my opinion. I want to see this stuff proliferated and developed and used because we're going to solve problems much faster this way.   
(00:23:19.800) ~~But yeah.~~(00:23:20.201)  
Yeah. It seems like the speed, I want to   
(00:23:22.823) ~~kind of~~(00:23:23.042)  
develop my intuition for the different learning loops and how they relate to each other as well. So again, let me just try a zoom out and then gradually   
(00:23:31.909) ~~kind of~~(00:23:32.108)  
zoom in and you can refine anything that I'm saying. The, again, super high level, we have the black box problem of we don't know how cells work. We don't know how the biological systems work at large. There's a lot of interactions that are not well understood. 


---


#### 00:23:45.874

But we can, through traditionally very laborious wet lab work, gradually isolate what seems to be at the heart of various problems. And then when we have that hypothesis of, okay, maybe this is what's going on, that could be probably confirmed to varying degrees. Then we can say, hey, maybe we can disable that particular interaction as in the case of the cancer one that you mentioned toward the top. And again, in a traditional setting, we don't know what the shapes of the things are. So that really limits our ability to do any sort of Targeted approach,   
(00:24:22.684) ~~right?~~ (00:24:22.865)  
Like, rational drug design has been   
(00:24:24.606) ~~sort of~~(00:24:24.866)  
the dream as I understand it for decades and is only now   
(00:24:28.351) ~~kind of~~(00:24:28.550)  
starting to happen now that we're developing all these tools to understand the shape. 


---


#### 00:24:33.036

So. I guess, in terms of, like, just a little intuition for the shapes to and the sort of confirmations. I sort of envision, and again, analogy free zone, but this is fairly literal with obvious room for mistakes. So again, correct my mistakes, but I sort of envision   
(00:24:52.067) ~~like~~ (00:24:52.287)  
a slinky where if I just sit the slinky down on the floor, it will   
(00:24:58.051) ~~sort of~~(00:24:58.492)  
come into a pretty tight coil. And that you might say is like its lowest energy state, then I can stretch it out. And if I,   
(00:25:09.462) ~~you know,~~(00:25:09.682)  
do the work and put the energy into it, then I can stretch it out. Now, if I let it go, it's going to snap back to its low energy state. 


---


#### 00:25:18.650

I could also come along and step on the middle of it. And then I would have the part of it would be like under my foot and bent down, but then the parts on the side would presumably still kind of look like they're normal, but there'd be this   
(00:25:28.999) ~~like~~ (00:25:29.159)  
deformed part in the middle where I'm stepping on it. Yeah. This is sort of analogous to what is going, violating my no analogy rule, but this is a pretty tight analogy. It's like a physical deformation, right? Where this thing can have a low energy state, but then maybe in the presence of some other protein that   
(00:25:45.173) ~~like~~ (00:25:45.394)  
constrains it in a certain way, or some other small molecule, perhaps it fits into a pocket of it in a certain way, or brings two parts that aren't normally together, more closely together, whatever, then you can have these sort of deformations. 


---


#### 00:25:58.085

And then subject to those constraints, they still kind of find their natural low energy state. And so you have   
(00:26:04.470) ~~like~~ (00:26:04.589)  
multiple of these, there could be, and of course this is all happening in an environment where the surrounding,   
(00:26:12.193) ~~I guess~~(00:26:12.374)  
it probably depends a lot on   
(00:26:13.434) ~~like~~ (00:26:13.555)  
just how big or small of a thing we're talking about, but the slinky relative to the air is like massive, right? The air molecules are super small relative to the slinky, so we don't really have to think too much about the air molecules, but in the context of these super small things, individual proteins, they're in solution, right? So there's at a minimum, there's like water molecules bouncing off them all the time. 


---


#### 00:26:36.717

So they have this sort of noisy environment. I'm thinking there of like brownie in motion, which I'm not by any means an expert in, but the constant sort of bumping into the environment creates opportunity for these things to kind of occasionally flop from shape to shape. And so doing all of this in traditional sense is probably hard for a lot of reasons, but you highlighted the fact that the computation is really slow, right? You just have a ton of interactions, the many terms and sort of how things interact. Now,   
(00:27:10.835) ~~like~~ (00:27:10.974)  
how is it happening that the, I have a hypothesis on this, but I'll just ask the question. How is it happening that the AI models are doing this so much faster and more accurate than traditional physics? 


---


#### 00:27:25.705

Because a naive thought would be like, there's nothing, there's only physics, right? We hear that sort of refrain a lot.   
(00:27:32.089) ~~So like, how would,~~(00:27:33.590)  
it seems in some sense surprising that you would be able to make a new black box system to make these predictions that they would be faster and more accurate as opposed to just running the physics. How is that leap happening? Okay, so   
(00:27:49.114) ~~I guess~~(00:27:49.394)  
the simple answer is basically compression, right? You've got some information and you have some really efficient way of compressing that information. And a lot of these AI models are,   
(00:28:01.804) ~~I mean,~~(00:28:02.724)  
you can think of them as functions, but you can also think of them as   
(00:28:06.749) ~~like~~ (00:28:06.909)  
compressors of information. 


---


#### 00:28:09.050

And so some of them,   
(00:28:11.133) ~~I guess,~~(00:28:12.153)  
traditionally you think of AI models like a deep learning neural network sort of thing, you've got data, you train on your data, maybe you have like a trained test validation split or something like that, and you train on your training data and you see how it performs on your test data and that's your trained model. But you can also train models with   
(00:28:31.578) ~~like~~ (00:28:31.719)  
physics constraints, right? And there are some models that are actually data-free. You can train some neural networks using physics constraints in a data-free way. people are doing this for this problem in particular, for getting the Boltzmann distribution of a protein and getting all these ensembles of conformations and their transitions between the states. 


---


#### 00:28:52.010

There are some approaches that people are using that are completely data-free and are based on physics. And the model is learning the physics and compressing that physics and then generalizing to systems that it hasn't seen before. And   
(00:29:04.461) ~~I think~~(00:29:04.760)  
because there's compression happening and you're not, so like in molecular dynamics,   
(00:29:11.476) ~~I mean,~~(00:29:11.596)  
you could simplify things by simplifying the forces or simplifying the model in terms of   
(00:29:16.378) ~~like how complicated of~~(00:29:17.579)  
how complicated the physics are that you're using to model problems. If I strip everything down and just do like bare bones, Newtonian physics, I can simplify things that way, but I don't see this notion of like compression happening.   
(00:29:31.208) ~~Right.~~ (00:29:31.468)  
Whereas for a neural network, you're compressing information. 


---


#### 00:29:35.109

You're taking something complicated and noisy sometimes, and you're compressing it down into some simpler maybe not simpler, but you're compressing it and you're providing a representation of it that is more compact. And because you've done this, and if you've done it, it generalizes to systems that it hasn't been trained on before. You get something that is faster, significantly faster, like orders of magnitude faster, right? You get something that produces your answer in   
(00:30:04.758) ~~like~~ (00:30:04.897)  
a minute instead of four hours or days.   
(00:30:07.744) ~~I think in my mind, the way that I understand it,~~(00:30:10.267)  
I think the key here is compression. Neural networks are compressors of information. Whereas molecular dynamics simulation, there's no real compression happening. Does that make sense? 


---


#### 00:30:20.846

Yeah. I think I'm just trying to kind of, should be okay. This software, yeah, all good. We will edit and also the software is uploading the original version opportunistically in the background. So even if we have a little lag or whatever, it should have the original high quality. Okay. So   
(00:30:39.089) ~~that was pretty much my hypothesis was that it's essentially learning higher order concepts beyond the raw physics.~~(00:30:49.397)  
  
(00:30:49.857) ~~And that is very analogous.~~(00:30:51.058)  
And we've covered this in a lot of different ways over the last hundred episodes with mostly focus on language models. But it's really this striking observation that comes up   
(00:31:01.946) ~~over and~~(00:31:02.188)  
over again that, okay, yeah, language models, they're only trained to predict the next token, but they not only seem to be generalizing certainly beyond the narrow, narrowly defined bounds of their training data, and perhaps to some degree even   
(00:31:20.491) ~~kind of~~(00:31:20.692)  
more than that, it's like a hotly debated topic, but what is pretty clearly demonstrated at this point is that in the   
(00:31:27.616) ~~like~~ (00:31:27.798)  
middle to late layers of a language model transformer, you can now, the techniques are there to say, okay,   
(00:31:36.828) ~~this,~~ (00:31:37.150)  
this pattern of activations seems to correspond to this higher order concept that we care about. which is   
(00:31:44.441) ~~kind of~~(00:31:44.922)  
a miraculous thing that like it's just predicting the next token, but it's like learning these concepts of justice and fairness and ethics and whatever that are like obviously useful to predict the next token. 


---


#### 00:31:58.490

And that's presumably why they're arising, but not something that's been like specifically coded for. So I guess in the application to biology, basically the same phenomenon is happening where raw data or raw simulated physics or whatever is sort of the input. And the higher order concepts are what? I'm guessing that they're sort of, I don't know a lot about this, but like the residue is sort of a part, it's like almost like the vocabulary of proteins. And we have the next token, the sort of The token level vocabulary of a protein would be the 20 amino acids, but the sort of higher order concepts are what? It's like, oh, this chunk of a thing is like reused a lot. 


---


#### 00:32:42.964

And these two chunks of things like interact with each other in a particular way. Give us a little more intuition of that. What are the higher order concepts that these things seem to be learning? Yeah. So if we put aside   
(00:32:53.670) ~~like~~ (00:32:53.829)  
dynamics for a moment and we just look at   
(00:32:55.631) ~~like~~ (00:32:55.770)  
structure prediction. So structure prediction, like AlphaFold2, for example, there's another model that does essentially the same thing. It predicts the 3D structure of the protein in some low energy state, right? ESMFold, right? This is like an alternative model to AlphaFold2. It doesn't perform as well as AlphaFold2, but it does pretty well. And it's a language model. It's something that people call a protein language model. 


---


#### 00:33:21.704

And it's It's built on the BERT architecture actually, which sounds kind of bad, right? Cause BERT's like this older model that's only used for like specific things now. And like the chat GPT   
(00:33:34.015) ~~sort of~~(00:33:34.316)  
models have overshadowed or outshined the BERT models at this point. But   
(00:33:39.678) ~~in,~~ (00:33:39.778)  
in biology, this actually makes a lot more sense because you have the mask language modeling objective. that you train on for protein sequences, and you just mask out some of the amino acids in the protein sequence and have it predict what those are,   
(00:33:53.325) ~~right?~~ (00:33:53.766)  
And just by training it to do this, and then putting like a folding model on top of it called EvoFormer, which actually comes from the AlphaFold2 architecture, you don't train on any physics, but somehow you learn how to predict 3D structures of proteins,   
(00:34:09.375) ~~right?~~ (00:34:09.574)  



---


#### 00:34:09.635

And so in this case, it's almost like physics mostly isn't needed. right? If you just want to predict a static structure of a protein, you can get pretty good results just using a BERT type architecture with mask language modeling objective, training on   
(00:34:26.550) ~~like~~ (00:34:26.710)  
millions of proteins. And if you just train on a bunch of proteins doing this, you get something that will fold proteins for you pretty darn well. And again,   
(00:34:35.076) ~~like~~ (00:34:35.215)  
there's some   
(00:34:35.715) ~~like~~ (00:34:35.856)  
really nuanced architectural differences between ESM Fold and Alpha Fold 2. 2 uses what's called multiple sequence alignments, and it also uses these templates, right? And in general, it is better performing because it has these extra,   
(00:34:50.804) ~~like,~~ (00:34:50.985)  
added things in the architecture that improve its ability to predict the structure. 


---


#### 00:34:55.648

But even there, there isn't really a lot of physics explicitly happening. Now, maybe there's some physics encoded   
(00:35:04.213) ~~in this~~(00:35:04.614)  
in some way. but we're not giving it forces and potentials and things like that. And yet somehow we're able to predict the structure of the protein with really high accuracy for a lot of proteins, for most proteins. I guess that's another example of where AI can be a lot better than the molecular dynamics. Because if you want to model a protein actually folding in a molecular dynamics simulation to get the folded structure of the protein, this is pretty hard and time-consuming and computationally intensive. Whereas for AlphaFold2 or ESMFold, it takes a few minutes. You give it a big protein and it takes a few minutes. 


---


#### 00:35:43.822

And I guess this is, in these cases, these are like language model-like models, right? They definitely have the architecture that looks a lot like language models, especially ESMFold. I think AlphaFold a little less because it has some of these extra architectural things that are a little more nuanced, like the MSA and the templates and such. But both of these models are very much inspired by language models. And ESMfold is pretty much just a language model. And you're able to predict these 3D structures with these things without really explicitly modeling any physics. And that provides a substantial speed up. And   
(00:36:20.237) ~~I guess~~(00:36:20.516)  
in terms of like how this relates to language modeling, so the concept that I think you're trying to grasp onto is protein motifs. or domains. 


---


#### 00:36:32.333

So motifs are like reoccurring patterns that happen in proteins. They're like short little sequences of amino acids that recur often in lots of different proteins and generally have a very similar structure across different proteins, for example. This is   
(00:36:48.623) ~~kind of~~(00:36:48.983)  
a fuzzy concept, right? Like defining what a motif is and having that shape described is a little bit fuzzy, but these models learn this. And like you're saying, these   
(00:37:01.351) ~~like~~ (00:37:01.492)  
higher order concepts where you're looking at   
(00:37:04.213) ~~like~~ (00:37:04.353)  
groups of amino acids now instead of just the individual vocabulary elements,   
(00:37:08.954) ~~right?~~ (00:37:09.153)  
We're not just looking at individual amino acids of the vocabulary anymore. We're looking now at an aggregation of amino acids at a higher level. Like you can pull this out of these models and there's some work on this, some older work that's I guess maybe three years old or so now called Birtology Meets Biology. 


---


#### 00:37:29.815

And they do a really in-depth study of how to pull out these different things, active sites and binding sites and motifs and things like this, based on the attention maps in the language model, in the protein language model. Another thing that people have found is the attention maps recapitulate the contact maps for proteins. And so the contact map is like a 2D matrix representation of all the contacts between the different amino acids in the protein, right? And it turns out the attention map, the matrix that you get from your attention mechanism, recapitulates that and is highly correlated with those contact maps. And so they are learning higher order concepts for sure, just as they do for natural language, for NLP domains. 


---


#### 00:38:15.369

And you can do topic modeling and things like that on these models. But   
(00:38:20.193) ~~I mean,~~(00:38:20.373)  
that's a very specific example of how NLP has influenced AI applied to biochemistry. I would say now   
(00:38:29.615) ~~the,~~ (00:38:29.996)  
a lot of the more interesting models are more influenced by diffusion and flow matching models now.   
(00:38:38.498) ~~Like~~ (00:38:38.637)  
a lot of the generative models that we're getting that are   
(00:38:41.458) ~~like~~ (00:38:41.619)  
predicting the Boltzmann distribution or that are generating new protein structures for you with specific   
(00:38:47.760) ~~like~~ (00:38:47.920)  
shapes and functions or are allowing you to design new sequences that fold into a particular backbone. All of these things   
(00:38:56.052) ~~are, a lot of them I should say,~~(00:38:57.414)  
are more influenced by diffusion and flow matching than NLP and language modeling and transformers. 


---


#### 00:39:04.922

I mean, some of them use transformers in there when they train the diffusion models, but they're starting to be a lot more influenced by Dolly-type models, I would say. Because you're starting to get this really fine-grained control over what kinds of proteins or small molecules or nucleic acids that you can generate. And there's actually some models that have come out that are text-conditioned. So a couple of the models that I mentioned were ProteinDT and MoleculeSTM. And these are generative models that are text conditioned and they allow you to type in   
(00:39:41.360) ~~like~~ (00:39:41.501)  
a natural language prompt and get out a molecule. So   
(00:39:45.884) ~~like~~ (00:39:46.023)  
protein DT, for example,   
(00:39:47.965) ~~or,~~ (00:39:48.105)  
or molecule STM, you can give it a text prompt and natural language, describing the properties of the molecule and just natural human language, giving it   
(00:39:56.771) ~~like~~ (00:39:56.931)  
this molecule has these chemical properties and it has this sort of bias away from or towards these amino acids or. interacts with these other molecules in such way. 


---


#### 00:40:08.056

You can give it these natural language text prompts and it will generate proteins and small molecules for you that satisfy these constraints or that correspond to the text prompt that you give it. And there are more models like this that have come out recently that do similar things. They're text conditioned, like diffusion models or flow matching models that are generative and that produce molecules with specified properties based on natural language text, which in my mind, that's   
(00:40:37.911) ~~kind of~~(00:40:38.170)  
mind blowing. I think that's amazing. Having a model that will just generate molecules for you that fit natural language descriptions   
(00:40:47.454) ~~is that's crazy.~~(00:40:49.054)  
How did that happen?   
(00:40:50.135) ~~Like,~~ (00:40:50.255)  
that's amazing. Yeah. No doubt. So let me just rewind a little bit again, and then I want to get into a little bit more how that happened. 


---


#### 00:40:57.925

So I always try to start with inputs and outputs as one good frame for understanding this stuff. So it seems like the first major breakthroughs in Afrobiology of the modern era, which is only the last however many years, were the structure prediction models. And   
(00:41:20.041) ~~this is,~~(00:41:20.882)  
if I understand correctly, there were about a proteins that had been analyzed to the point where people were pretty confident that they had a structure. If I understand correctly, this was mostly done through   
(00:41:31.673) ~~x-ray crystalline, which is... Yeah,~~(00:41:33.876)  
cryo-EM. Yeah. So I think that's why the initial things were   
(00:41:39.420) ~~sort of~~(00:41:39.701)  
limited to outputting a single predicted structure because if you're in like a crystal, you   
(00:41:45.190) ~~sort of,~~(00:41:45.451)  
by the nature of crystals, have a single repeating structure, right? 


---


#### 00:41:50.012

So what we had was people put a lot of time in the lab into, first of all, figuring out how to get these things to crystallize, which is weird because they're not really   
(00:42:00.936) ~~Protein crystals don't really~~(00:42:02.237)  
occur in nature, right? That's a very odd thing in the first place. Maybe that's like gout,   
(00:42:07.039) ~~I guess.~~(00:42:07.298)  
It's   
(00:42:07.458) ~~sort of~~(00:42:07.699)  
like uric acid crystals, if I understand correctly. But you don't think of proteins... We think of them as floating around in solution or   
(00:42:15.782) ~~kind of~~(00:42:15.963)  
interacting with each other in complicated ways, but they're not in repeating lattice structures. So that in and of itself was   
(00:42:22.505) ~~sort of~~(00:42:22.726)  
a weird,   
(00:42:24.047) ~~like,~~ (00:42:24.206)  
closest approximation that we could get right if we got to make enough of this stuff that we can get it to put in coalesce into some crystal form, then we can hit with x rays and we can try to decipher how that gets scattered. 


---


#### 00:42:35.213

And then we can come up with a structure and we hope.   
(00:42:37.614) ~~I mean,~~(00:42:37.974)  
we don't really know anything,   
(00:42:38.994) ~~I guess,~~(00:42:39.275)  
but   
(00:42:39.536) ~~I guess~~(00:42:39.755)  
it works well enough   
(00:42:41.456) ~~that~~ (00:42:41.557)  
that approximates the structure that it actually takes in the cell, but no guarantees. So first generation of stuff is not first generation, of course, we're like other AI techniques before this, but of these sort of modern wave of mega breakthroughs.   
(00:42:58.092) ~~the~~ (00:42:58.253)  
and   
(00:42:58.492) ~~I guess that was~~(00:42:58.913)  
really measured by maybe you could help me fill in some blanks here too   
(00:43:02.418) ~~because~~ (00:43:02.639)  
but   
(00:43:03.519) ~~there's~~ (00:43:03.719)  
it's like   
(00:43:04.340) ~~kind of~~(00:43:04.521)  
circular nature to some of this stuff sometimes   
(00:43:06.644) ~~where I'm like wait a second~~(00:43:07.425)  
so where is the ground truth it seems to be a little bit of it can feel like   
(00:43:11.731) ~~uh~~ (00:43:11.831)  
the ground truth is   
(00:43:12.532) ~~sort of~~(00:43:12.733)  
a shell game As I understand it, the way that AlphaFold was determined to be a breakthrough in the first place was that there was a competition held on an annual basis or whatever, where people would basically show up with their shape predicting model, and they would be given, here is the sequence. 


---


#### 00:43:36.581

And their job is to predict the shape. And then the   
(00:43:39.445) ~~test set,~~(00:43:40.445)  
the sort of training set was all known proteins that came before. And the test set was all of the stuff that had been newly derived in the last year. So these were the new things that people hadn't been able to train on. They would show up and they would be measured against essentially the crystal based techniques and everything would fall short,   
(00:44:05.168) ~~like~~ (00:44:05.329)  
not nearly as good, not matching the crystal things. And then AlphaFold showed up and was like, oh, hey, it's, and this is where I get a little fuzzy. As I understand it, people would say it's in some ways even   
(00:44:14.893) ~~like~~ (00:44:15.052)  
better than the crystal techniques, but   
(00:44:16.954) ~~like,~~ (00:44:17.153)  
how do we establish that? 


---


#### 00:44:19.054

How do we know that the when is the crystal technique right or wrong. I'm a little fuzzy on how we kind of pin down the ground truth when we know that the crystal thing is only an approximation and AlphaFold was kind of trained on that with augmented data like help me pin down the ground truth there if you can. Yeah   
(00:44:36.789) ~~I mean~~(00:44:37.068)  
ground truth in this case   
(00:44:38.590) ~~yeah I mean~~(00:44:39.010)  
this is a little hard and it's very   
(00:44:41.213) ~~like~~ (00:44:41.393)  
application and   
(00:44:43.277) ~~like~~ (00:44:43.436)  
situation specific, right? Depending on what you're trying to do and how you're trying to do it, you may want some crystallized structure that you got in a lab, or you maybe want like an alpha fold structure. 


---


#### 00:44:53.365

And in other cases you might want like a trajectory or an ensemble of conformations, which wasn't really possible until more recently.   
(00:45:02.432) ~~Like~~ (00:45:02.594)  
observing the dynamics of a protein is really hard. And so to be able to model that on a computer and get predictions that are actually accurate about the dynamics of the protein and all the different   
(00:45:17.721) ~~like~~ (00:45:17.900)  
low energy conformations that it exists in,   
(00:45:21.382) ~~like~~ (00:45:21.501)  
that's pretty new. And in my mind, if you have the ground truth really ultimately is the Boltzmann distribution, right? Which is this very sort of theoretical physics idea that comes from like statistical mechanics. that's the ground truth. Whether or not you can model that on a computer or observe that in a lab is another question. 


---


#### 00:45:45.786

But the Boltzmann distribution of the protein is the ideal ground truth. And is that basically like a... I guess I'm thinking of it in one sense as sort of like a potential, energy potential diagram where you have... It's related. It's a probability distribution, right? And it describes You can think of it in terms of an energy landscape, right? Because if you have this nice energy landscape, the low parts, the valleys that you have in your energy landscape are gonna be like the metastable states of the protein. They're gonna correspond to the metastable states of the protein. And then the peaks, like on top of the mountains,   
(00:46:22.952) ~~right?~~ (00:46:23.112)  
These are like states that are very transient and that are like unlikely to exist for very long. 


---


#### 00:46:30.773

So when you're trying to model the Boltzmann distribution, you're trying to get out these like low energy conformations from it and then the transitions between those and understanding how often you transition between this state and this other state and what that transition looks like. I guess that would also be considered part of the ground truth, right, because this is all part of the dynamics of the protein in the environment and not just some single either crystallized structure or alpha fold 2 predicted structure. Yeah, so   
(00:47:02.173) ~~I guess~~(00:47:02.434)  
the answer to your question is the ground truth, at least to me, is the Boltzmann distribution. And the question of whether or not you can model that on a computer in a lab is a completely different question, but that's the ground truth. 


---


#### 00:47:14.880

So it's a probability distribution of what percentage of the time the protein in some like neutral case solution or whatever is in shape A versus shape B, versus shape C, and then the in-between things are sort of   
(00:47:33.393) ~~Here I'm kind of again returning to my slinky visualization where I could have the thing sort of in its lowest state or I could like tie its ends together and then it'll sort of make a nice circle and~~(00:47:46.164)  
but again   
(00:47:46.806) ~~kind of~~(00:47:47.005)  
look compact and be   
(00:47:48.286) ~~sort of~~(00:47:48.527)  
in a relatively comfortable place but then the second that breaks it's like reverbing back until it gets to its normal state, that reverb moment is sort of the transitional state. 


---


#### 00:47:58.168

It's not going to be in that state very long and it's   
(00:48:00.409) ~~kind of~~(00:48:00.728)  
on its way from one to another. So we don't know how many different, for any given protein, there could be   
(00:48:06.771) ~~like~~ (00:48:06.891)  
multiple different low energy states that it might spend time in. And there probably also is like a path issue to it where you maybe can get from A to B and B to C, but not necessarily A to C without going through B I imagine. Yeah, exactly. So lots of weird stuff there. And then, okay, so all that is just they interact with each other. So this is,   
(00:48:29.882) ~~I guess,~~(00:48:30.101)  
where AlphaFoldMultimer starts to come in? Yeah. AlphaFoldMultimer models the interactions between proteins, right? 


---


#### 00:48:37.128

And you can model protein complexes. And there's actually some new results that just came out maybe a month ago, that computes something called the LIS score based on the PAE output of alpha-fold multimer. This is like a... Can you unpack both of those? Give us the PAE too. So the PAE is one of the outputs of alpha-fold multimer and it's, let's see if I remember what the abbreviation is for, predicted aligned error, I think is what it stands for. And this is telling you, it's a metric that tells you the quality of   
(00:49:08.757) ~~the~~ (00:49:08.896)  
the interfaces between the two proteins. You've got a lot of different metrics that come out of AlphaFold Multimer or AlphaFold2. So you have PLDDT, which tells you a per residue confidence score of how confident the model is that is the structure of the protein at that particular point   
(00:49:27.519) ~~in the protein,~~(00:49:28.199)  
like at that particular residue. 


---


#### 00:49:30.500

And then you can take the average of the PLDDT and get an overall confidence for the whole protein. But then   
(00:49:35.942) ~~you also have,~~(00:49:36.541)  
you have IPTM and PTM scores, which are other scores that tell you about other aspects of the protein, and then you have these PAE outputs, predicted aligned error outputs, and these tell you about the quality of the interfaces between the proteins when it predicts the two proteins together. there's an interface region where the proteins are in contact with each other. And you can   
(00:49:58.661) ~~kind of~~(00:49:58.860)  
think of it as a certain cutoff, right? After a certain distance, you don't really count it as an interface residue anymore. But the PAE tells you the quality of these interfaces, how good of a quality the model has provided you. 


---


#### 00:50:11.804

And you can compute something based on the PAE called the LIS. And the LIS score, let me look up what that stands for really quick, because I actually forgot what it stands for. So while you're doing that, I'll just riff a little bit on   
(00:50:24.922) ~~the structure too. Or~~(00:50:27.293)  
the nature of the interface, because this is just another level of like insane complexity, right? You have a range of   
(00:50:34.077) ~~kind of~~(00:50:34.318)  
whether these things are like jigsaw puzzle pieces that are perfectly fit to each other and have a really tight coupling or jigsaw pieces that   
(00:50:43.585) ~~sort of~~(00:50:43.844)  
fit. You can   
(00:50:44.425) ~~kind of~~(00:50:44.726)  
press them together, but they don't perfectly fit and they don't really want to stay together as much. 


---


#### 00:50:48.728

All the way down to obviously they just don't fit at all and they just kind of don't adhere to each other. Is there anything more we could do to develop our intuition there for how strong is the strongest fit? I'm thinking like, boy, if I screw a screw into a nut, it's not coming off with any natural process. Somebody would have to come unscrew that. I'm guessing it's probably... I don't know. How tight are the tightest ones and what is the dynamic range of how adherent these things are to each other? Yeah, so there's two ideas that you're addressing here. One of them is like binding affinity, like how much affinity these two things have for each other to bind to each other. 


---


#### 00:51:31.472

And then there's also in terms of like dynamics, like how weak or strong or how transient are the interactions between them in terms of like dynamics and like the time spent next to each other, right? There's recent work I think it's out of MIT, they built these flow matching models with AlphaFold and ESMFold. It's called AlphaFlow. And AlphaFlow, they use the AlphaFold2 architecture and they train it as a flow matching model, which is like a generalization of diffusion. And using this, they get these ensembles of confirmations for a protein. And part of the information that they get out of this is how transient the interactions between residues are. If you   
(00:52:15.663) ~~produce,~~ (00:52:16.244)  
let's say you run your alpha flow model and you produce   
(00:52:20.027) ~~like~~ (00:52:20.166)  
10,000 different confirmations or states that the protein exists in, and then you can   
(00:52:26.672) ~~kind of like~~(00:52:27.072)  
cluster those, like structurally, you can cluster them and then look at which residues are close to each other in each of those clusters. 


---


#### 00:52:37.652

So maybe you take   
(00:52:38.371) ~~the, you take~~(00:52:39.592)  
the centroid or something of a cluster, and then you look at the distance between the residues, and then you look at other clusters, and the distance between the residues in those other clusters, and you get an idea of   
(00:52:51.554) ~~like~~ (00:52:51.795)  
how often two residues are in contact with each other from this. And you can tell how transient the interaction between these two residues are, and how much time they spend together. You could generalize this, right? And this is something that hasn't been done yet. So people who are looking for   
(00:53:07.875) ~~like~~ (00:53:08.014)  
research projects, this would probably be a pretty good one. If you generalize this to alpha fold multimer, do the alpha flow thing with alpha fold multimer, if it works well, and again, this hasn't been done before, but this would be a really great thing for someone to do. 


---


#### 00:53:21.996

You could figure out how transient those interactions between two proteins are, right? Because now you have two proteins or more, maybe you have three or four or whatever, but you have two proteins that are in different conformations at different times. And AlphaFlow will generate all these different conformations for you. And then you can analyze all these different conformations and figure out how transient the interactions between the two proteins are and get an idea more about the dynamic side of things and not just a single number or a single metric like binding affinity, right? Because   
(00:53:57.110) ~~binding affinity, I mean,~~(00:53:58.110)  
it's a hard thing to predict. It's a hard thing to compute. training a model to predict binding affinity is actually a pretty hard thing to do. 


---


#### 00:54:05.231

And most of them don't work. Most of them don't generalize well. But these approaches, like if you were to generalize alpha flow to the alpha,   
(00:54:12.775) ~~like that,~~(00:54:13.175)  
that would give you more information than just binding affinity.   
(00:54:15.637) ~~That would give you,~~(00:54:16.277)  
that would give you some notion of how often particular residues of the two proteins are in contact with each other. And then,   
(00:54:23.902) ~~like I was saying before,~~(00:54:24.722)  
the LIS score, this is the called the local interaction score. They use alpha fold multimer and they get the PAEs out of alpha-fold multimer. And then using the PAE, they compute the LIS, which is a pretty simple computation.   
(00:54:39.152) ~~I don't know that I can describe it in words,~~(00:54:40.914)  
but it's not a terribly complicated thing to compute. 


---


#### 00:54:44.115

Once you have the PAE, the LIS is pretty easy to compute. And this tells you how likely you are to have a protein interaction, which kind of gets that binding affinity to some degree. And being able to predict protein interactions is actually a really hard problem. And most models that try to predict protein interactions don't work well and don't generalize well. And there's actually   
(00:55:07.675) ~~a kind of~~(00:55:08.315)  
a big problem with a lot of these models. So when people are training them, a lot of times if you're training a model that takes as input protein sequence or two protein sequences, people don't split their data in the right way. you have this notion of sequence similarity and   
(00:55:25.474) ~~if you if your data~~(00:55:26.715)  
if your training data has sequences in it that are very similar to your test data sequences you're going to get overfitting and you're not even going to realize it like all the usual signs of overfitting aren't going to be there but you're going to overfit without even realizing it because you're going to have training data and test data that's highly similar to each other in terms of sequence similarity. 


---


#### 00:55:51.248

#### 00:56:32.050

So that is basically the actual positioning with sort of a confidence indication. Yeah. And it tells you what the quality of the interfaces are between the two proteins that you're predicting in the multimer. And something else we should probably get into that directly follows from alpha-fold multimer is other ways of generalizing the alpha-fold model or training models that are like alpha-fold that do more than just proteins. You might have complexes where there's a protein in a small molecule, or protein in DNA, or protein in RNA, or a metal, or whatever. And so there's all these other biomolecules that you might want to model in complex with each other. And to generalize AlphaFold Multimer to this new situation is pretty hard, but some people have managed to do a pretty reasonable job of it. 


---


#### 00:57:28.389

I think there's still room for improvement on these, but like a new model that just came out recently is RosettaFold AllAtom. And RosettaFold AllAtom will let you predict complexes that have proteins and small molecules, proteins and nucleic acids, and proteins, and proteins and metals too. Big step forward now, because now you can apply this idea of computing the LIS score to these other complexes. And you can get this score that tells you how likely there is to be an interaction there and how strong that interaction is. And you could also,   
(00:58:03.465) ~~I don't know how hard this would be to do, just thinking about it now, it seems like it might be actually kind of hard, but you could probably do~~(00:58:12.498)  
the alpha flow type method with something like Rosetta fold all atom as well and get something like conformational ensembles out of it. 


---


#### 00:58:22.505

And that's probably, something like that is probably coming soon. Somebody's going to work on that eventually. So yeah,   
(00:58:28.710) ~~I think~~(00:58:28.971)  
I answered your question.   
(00:58:29.791) ~~I'm not sure. Yeah. Let me just think about where I want to go back to. Okay.~~(00:58:34.614)  
The one thing that you said that caught my attention was, this is all in the context of predicting shapes. We need to predict shapes because we need to understand how things interact. Now we're even getting into predicting how things conform to each other. So the shape of multiple things as they're in actual interaction. and we get these sort of positional predictions that can be   
(00:58:58.655) ~~sort of~~(00:58:58.876)  
cashed out to these parts are actually   
(00:59:01.117) ~~like~~ (00:59:01.336)  
interacting in a meaningful way and this is really where the action is versus these other things are   
(00:59:05.719) ~~kind of~~(00:59:05.900)  
distant from each other that's not really where the action is that's being generalized beyond all proteins to like all the different kinds of things that are meshed up together in a cell. 


---


#### 00:59:19.150

But I believe you had said that there were like as many as 10,000 possible confirmations for a single thing. Was that, did I get it? Yeah. So like AlphaFlow, when you run AlphaFlow, it generates confirmations of a protein for you. And it was trained on molecular dynamics data, on simulation data. And so it does have some notion of   
(00:59:43.949) ~~like~~ (00:59:44.110)  
dynamics. And what it does is it produces different confirmations of the protein for you. And you can tell it how many of these to produce, right? And the more that it produces, the more likely you are to get a nice global picture of all the different confirmations that might exist for that protein. AlphaFlow, so we've actually tested AlphaFlow on these proteins that are called fold-switching proteins. 


---


#### 01:00:11.344

Fold-switching proteins, so like probably the most popular example floating around in the literature and in the community right now is Kybe. And Kybe is this fold-switching protein that like 10% of the time it exists in this one conformation and then 90% of the time it exists in this other conformation. And this is influenced by   
(01:00:29.693) ~~like~~ (01:00:29.813)  
a circadian rhythm. So it's like a night-day cycle sort of thing that's influenced by like your circadian rhythm. And when you apply AlphaFlow to some of these fold-switching proteins, it doesn't capture both of those fold-switch states. So in the example of Chi-B, it actually only really predicts conformations that are relatively close to the fold-switch state. which is like the slightly higher energy confirmation, the one that's a little bit less likely, the one that it exists in 10% of the time, which is a little bit odd, right? 


---


#### 01:01:04.922

Because you would expect and maybe want your model to go for the ground state or the lowest energy confirmation. And for some reason, it   
(01:01:14.867) ~~like~~ (01:01:15.027)  
sticks   
(01:01:15.507) ~~kind of~~(01:01:15.766)  
close to the fold switch confirmation. I'm not sure that there's like a good explanation for why. And that really goes,   
(01:01:24.635) ~~I think~~(01:01:25.076)  
it goes back to the AlphaFold2 predictions, because when you predict the structure using AlphaFold2, you get the fold switch state, you don't get the ground state. And people have done all kinds of little hacks to try and get out the ground state instead of the fold switch state. And the most popular method that they've hacked together is doing MSA subsampling or clustering the MSA and using the different clusters to predict structures, because If you take your MSA and you cluster all of your sequences in your MSA, you're   
(01:01:59.326) ~~kind of like~~(01:01:59.967)  
you're grouping the sequences in the MSA in a way that captures certain evolutionary information. 


---


#### 01:02:08.351

And different clusters will focus on or accent particular conformations. And so if I take out one of my clusters and predict the structure using those clusters in the MSA, I'll get a confirmation out from AlphaFold2. And then if I pick   
(01:02:24.994) ~~a different set of,~~(01:02:25.974)  
a different cluster of sequences in my MSA, I'll get maybe a slightly different confirmation, or maybe a drastically different confirmation. And   
(01:02:35.101) ~~if you do this,~~(01:02:35.681)  
if you do this right, sometimes, not always, but sometimes, you can get out the different confirmations of these fold-switching proteins. And for Ki-B, they've done this successfully, and for a few others, but it's not a super robust method, And   
(01:02:50.882) ~~I think these alpha flow, I think,~~(01:02:54.103)  
is in some ways maybe more informative. 


---


#### 01:02:58.106

And something like Boltzmann generators or distributional graph former, I think, are significantly better in terms of how they approach the problem, because they're going to give you more information and they're gonna give you more robust information. So for example,   
(01:03:15.929) ~~like~~ (01:03:16.048)  
distributional graph former, you're gonna get out something more robust and more informative than if you're just like clustering the MSA or subsampling the MSA for alpha. Can we talk about this MSA thing for a second?   
(01:03:30.514) ~~If I understand clearly, I'm not even sure I should attempt this, but I'll go for it.~~(01:03:34.335)  
Is it basically that we know that a gene codes for a protein, we have a lot of variation in the genes. The genes can have lots of random differences between them, but we can   
(01:03:48.110) ~~sort of~~(01:03:48.329)  
identify that these are all different variations on the gene. 


---


#### 01:03:52.193

Some of the genetic, some of the DNA level differences may make no difference in the protein, but others will make differences in that at a particular position in the protein sequence, you'll have a different amino acid. And so now you've got   
(01:04:07.797) ~~kind of~~(01:04:08.097)  
the same protein, but it can have different elements in particular position. And so these are grouped for the purposes of prediction?   
(01:04:18.686) ~~Kind of.~~(01:04:19.065)  
So an MSA is actually a pretty old concept that comes from computational biology. People have been using MSAs for a long time. And essentially, it's based on the edit distance. So if I have just a string of characters and I make some edits in some different places, I can compute the edit distance between those. 


---


#### 01:04:41.934

And if I have a low edit distance, then those two sequences are highly similar. MSAs are basically this. I take a protein and I have a whole bunch of different mutations of that protein or a whole bunch of other protein sequences that are very close to that protein in terms of sequence similarity, but they have some changes here and there. A lot of times the changes that happen only happen in certain regions of the protein. And then there are other regions of the protein that are highly conserved. And so when you do an MSA, you can look at which regions of the protein are really highly conserved. And a lot of times this will give you some indication of which parts of the protein are going to affect the function if you like mutate them and stuff. 


---


#### 01:05:27.440

So if I have a highly conserved residue that in my MSA, it just doesn't change. It stays the same through pretty much all of the MSA. Like 90% of the sequences in my MSA, this amino acid stays the same, right? If I change that, if I mutate that, it's probably going to affect the function of the protein. Because it's like a highly conserved region of the protein that evolution hasn't changed or has changed very infrequently. And so because of that, if you change some of those residues that are highly conserved, oftentimes you'll degrade the function of the protein or change the function of the protein, or maybe you'll decrease its thermal stability or something like that. 


---


#### 01:06:09.599

So MSAs are just telling you, they're telling you evolutionary information that is conserved among a whole group of proteins that are highly similar to each other in terms of sequence similarity. And AlphaFold2 uses MSAs. You can either use the database of MSAs or you can have it compute them on the fly. And it uses these MSAs to inform how it predicts the structure of the protein. Because when you have proteins that are very closely related evolutionarily, in terms of evolution, their structures are often very similar,   
(01:06:43.702) ~~right?~~ (01:06:43.862)  
And that's not always true. Like, I can have two proteins that are very similar, but have very different structures. Like, that happens all the time. But if you have this extra evolutionary information in the form of an MSA, you have extra information that helps you predict the structure of the protein, because all of these evolutionarily related proteins are oftentimes going to have very similar structures to your protein of interest. 


---


#### 01:07:10.231

So sort of calling to mind the classic image of the plane with all of the spots where the planes came back having been shot and then all the places that they didn't observe, those were the planes that got shot down. So this is the evolutionary equivalent of that where we don't see changes in certain regions because they're super core to functionality. And that in turn is super useful for prediction making because   
(01:07:39.769) ~~that~~ (01:07:40.369)  
these parts are like the really important parts and they're going to have to fit together or the sort of interactions that they have with other things are   
(01:07:47.333) ~~kind of~~(01:07:47.673)  
the whole point of what's going on here. Okay. So that's interesting. The overfitting piece, 


---


#### 01:07:52.195

I didn't quite understand. It seems like that's related though, where you said because these things are so similar, You have to be careful that you're not, give me the overfitting thing again. Cause   
(01:08:02.501) ~~I can't,~~(01:08:02.780)  
I'm not sure I can do it justice. Like when you do a train test split in deep learning and you're training your neural network on your train, on your training data, and   
(01:08:12.288) ~~you have,~~(01:08:12.648)  
you have your test data to   
(01:08:14.389) ~~sort of~~(01:08:14.708)  
test your model on after the fact, once it's trained to see how well it predicts on data that it hasn't seen before. And so when you're doing this, you want to make sure that your test data doesn't have a bunch of sequences in it that are highly similar to your training data. 


---


#### 01:08:31.177

Because it's almost like you're training on the same thing twice and you overfit this way. You don't get a good indication of how well your model generalizes. And a lot of people do this. A lot of people coming from   
(01:08:42.060) ~~like~~ (01:08:42.201)  
deep learning, just getting into   
(01:08:43.761) ~~like~~ (01:08:43.881)  
the biology stuff and they don't have a super strong background in biology. They make this mistake very often. And so there's just tons and tons of neural networks and different kinds of deep learning models out there. that don't generalize and that are very overfit because they didn't split based on, they didn't split their data based on   
(01:09:02.010) ~~like~~ (01:09:02.170)  
sequence similarity   
(01:09:03.570) ~~and or~~(01:09:03.990)  
structure similarity. So   
(01:09:05.532) ~~you,~~ (01:09:05.712)  
like when you train models, usually you want to split your data based on sequence similarity and or structural similarity. 


---


#### 01:09:14.256

And a lot of people also split it based on like dates, like you were talking about CASP earlier. They have a certain cutoff date, and then the stuff that was resolved after that cutoff date is used in the test data. But when you're training, you're doing your training data, but you split your data based on things like sequence similarity and or structural similarity to make sure that you don't overfit and to make sure that your model generalizes to unseen data. Gotcha. Interesting. Okay. Yeah. It seems like in the case of something about this that I don't have a good intuition for, because that's not really done in language modeling, right? In language modeling, you could certainly have like lots of sentences that are very similar and you don't sort of say, oh, we're going to hold out. 


---


#### 01:09:58.029

We don't, we don't draw conceptual lines between different parts of the data and try to generalize across those lines. So what is the difference in the biology context?   
(01:10:08.896) ~~Like~~ (01:10:09.037)  
my intuition says to the degree that this thing is learning that these models are learning like the higher order concepts that really matter. that they should be able to learn those kind of regardless. And again, in the language model case, we don't really have a concept of overfitting, at least in the large-scale foundation models. Is this maybe just because we're not really doing large-scale foundation models in quite the same way? Or how would you describe the difference? I mean, there's still a concept of overfitting in LPN training big giant models, 


---


#### 01:10:41.068

CLAWD or CHAT-GPT or whatever. You can definitely still overfit these models. Very often for an NLP models, like these really big chat type models, like really big LLMs and stuff. First of all, they often only train on one pass through the data, right? They don't do multiple passes. And partially because of that, overfitting is not much of an issue because you're not training multiple times on the same data. So I do think that is changing. One little nugget from the recent Zuckerberg Dworkesh interview that I definitely made my ears and brain light up was when he said they trained these latest llama models on 15 trillion tokens. He said, we   
(01:11:19.966) ~~kind of~~(01:11:20.206)  
stopped because   
(01:11:20.907) ~~we,~~ (01:11:21.046)  
at some point we need to move on to Lava 4. 


---


#### 01:11:23.887

But he said we could have rotated the high value tokens through again. And I was like, Oh, interesting. I've seen some results about that, but in any event, it does seem   
(01:11:32.791) ~~there's,~~ (01:11:33.011)  
we're now to get to 15 trillion tokens. Basically, I don't think you have much choice, but to rotate. Yeah. Anyway, that's a bit of an aside, but I'm still not quite grokking it to be honest. Okay.   
(01:11:45.336) ~~So let's see,~~(01:11:46.237)  
what's a good analogy. I'm trying to think because yeah. And like NLP, like most people don't really think about the, so you have a data distribution and your training data and your test data, like your test data is supposed to tell you something about how well the model generalizes. 


---


#### 01:12:04.146

Right. And it's also supposed to tell you about if the model's overfitting or not, because when you compare your training metrics to your test metrics, whatever they may be. If your training metrics are different, like the training test, or the training metrics and the test metrics are substantially different, then you're either overfitting or underfitting. If   
(01:12:26.613) ~~your test metrics,~~(01:12:27.694)  
if the metrics on your test data are substantially worse than the metrics on your training data, then you've overfit, right? And if it's the other case, if your test data is substantially better than your training data, which is   
(01:12:45.494) ~~kind of~~(01:12:45.734)  
hard to do, then probably you could train some more. Maybe you're under fit. So your trained test split is supposed to tell you something about how well the model generalizes and how overfit your model is. 


---


#### 01:12:59.801

And comparing how it performs on the training data to the test data tells you that.   
(01:13:05.141) ~~It tells you a lot about how overfit your model is, if it's overfit,~~(01:13:08.604)  
and how well it's generalizing to data that it hasn't seen before. And to really   
(01:13:12.666) ~~get a good grasp,~~(01:13:14.065)  
to get a good idea of how well your model is generalizing to unseen data, you want at least part of your test data to be very dissimilar from your training data. Because that means it's generalizing to things it hasn't seen before, right? That means it's picked up on some deeper concept and language that generalizes to areas that it hasn't seen before, and it's using those really deep concepts to make predictions or generate things that are out of distribution. 


---


#### 01:13:46.679

And this is a big thing that people discuss, is whether or not these things generalize to data that's out of distribution. And if you train them in the right way, you can get models that generalize well to out-of-distribution data, right? This is not something that's impossible to do, you just have to do it right. And in the case of biology or biological sequences like proteins, to get a test set that gives you a good indication of one, how well the model is generalizing, and two, if it's overfit or not, you need to make sure that your test data is very dissimilar from your training data. And the way that you do this is you look at the sequence similarity between the protein sequences in your training data and your test data. 


---


#### 01:14:33.846

And you can also look at structural similarity, because you can have different sequences that are very different in terms of sequence similarity, but that fold into the exact same structure, more or less, right? We can have two very dissimilar protein sequences that fold into pretty much the same structure. And so sometimes depending on what your model architecture is and what your goal is, you may also want to split based on structural similarity and not just sequence similarity to make sure that your model is generalizing and not overfitting. Okay.   
(01:15:05.407) ~~I think~~(01:15:05.606)  
I got it. Does that make sense? Yeah.   
(01:15:07.747) ~~I think~~(01:15:07.988)  
so. It seems that it is   
(01:15:09.847) ~~sort of~~(01:15:10.268)  
a form of data leakage, essentially. Like you could imagine, and it's   
(01:15:14.248) ~~sort of~~(01:15:14.628)  
that you're fooling yourself, right? 


---


#### 01:15:16.088

For any given architecture, presumably the very best performance would be if you trained on all the data. But in order to effectively evaluate your architectures along the way, you need to have some holdout or you might call it a benchmark in certain contexts to evaluate against. And these similar enough sequences basically are a data leak in the same way that if you find out after you do your thing that, oh, hey, we actually had MMLU in the training data for the language model, then it means, oh, you can't really trust the MMLU scores anymore. And the model still may be good, it may not be so good, but if you train on MMLU, we can't really score you on MMLU. 


---


#### 01:15:59.019

And this is a similar problem. You can't trust her. Exactly. Exactly. Yeah, exactly. And there are even more nuanced ways of splitting the data, too, for specific things. The new version of DiffDoc They trained a new version of DiffDoc, I think they call it DiffDoc L, because it's larger. It's the large DiffDoc. And they use this method called confidence bootstrapping, which is   
(01:16:24.069) ~~sort of~~(01:16:24.329)  
like reinforcement learning. And they also split their data in a really unique way that's based on different domains or motifs that are present in certain interactions. They split their data based on that, in addition to,   
(01:16:41.309) ~~I think,~~(01:16:41.809)  
sequence or structural similarity. I would have to look at that. they split their data based on these domains that are present in these interactions to train a model for docking, right? 


---


#### 01:16:51.760

So you have a ligand, a small molecule ligand that you're trying to dock into a protein and do like blind docking, which is a hard problem. And they get like substantially better performance and it generalizes a lot better in this new version of DiffDock because of the way that they trained it and the way that they split their data. And they have some really strong confidence that their model is generalizing to out of distribution data, and it's able to predict on things that it hasn't seen before, and they're very dissimilar from what it has seen. So   
(01:17:23.545) ~~just to,~~(01:17:23.845)  
not to interfere, but just to make sure I understand, when you said, I've lost exactly what you said, but I just want to make a distinction between what they've demonstrated is that you should be more confident in doing this stuff in totally new regimes based on the fact that they've been very meticulous in the data split. 


---


#### 01:17:42.835

Whereas if they had thrown everything into the training, then you would have a hard time knowing to what degree to be confident in out-of-distribution stuff. They did a really good job with that model. I think their performance boost was pretty big. They got a lot better performance out of it too. That's definitely a good model to look into if you're looking to get into this stuff. So   
(01:18:05.966) ~~maybe let's, I don't know if there's more that you think we need to cover on.~~(01:18:10.269)  
  
(01:18:10.469) ~~I mean,~~(01:18:10.809)  
we've been up and down the layers of or the levels of abstraction, but it seems like the two big things that I want to go to next   
(01:18:19.832) ~~and~~ (01:18:19.972)  
being mindful that we've already been at it for a while are the diffusion concepts where it seems like we're moving from predicting a structure to generating new things. 


---


#### 01:18:32.416

And then maybe we could get into a little bit of, okay, in actual work, like what are the cycles that are used to actually make progress on questions of interest? Like you have a target, you want to make some modification, like how do these things fit together to allow us to work a lot faster and get more value from our limited work resources? Before we go on to the diffusion and generative side, though, anything else that we didn't cover   
(01:18:57.291) ~~or that you think is a missing part of the piece,~~(01:18:59.012)  
a missing part of the picture for the fundamentals or the structural prediction? No,   
(01:19:03.417) ~~I think,~~(01:19:03.738)  
yeah, we should move into RF diffusion. I think that's a good direction to go in now. 


---


#### 01:19:09.564

Are you familiar with RF diffusion at all? No, not really. Although, from what little you said earlier, it sounded to me like CLIP, basically. I was   
(01:19:18.838) ~~sort of~~(01:19:19.079)  
hearing that,   
(01:19:22.121) ~~you know,~~(01:19:22.421)  
with CLIP you have   
(01:19:23.601) ~~kind of~~(01:19:23.921)  
images and their captions, and here it sounds like we have   
(01:19:26.603) ~~like~~ (01:19:26.743)  
proteins and their sort of descriptions. No, so that's ProteinDT and MoleculeSTM. Those are much more like CLIP. They use the exact same method as CLIP. They use contrastive learning and they have   
(01:19:38.189) ~~like~~ (01:19:38.369)  
captions and molecules or captions and proteins. And so those are our text condition models where you can type in a natural language description of your molecule or your protein without a structure or a protein sequence that fits that description. 


---


#### 01:19:55.573

And so those I think are a bit different from RF diffusion. RF diffusion is a diffusion model that it's not text conditioned. You can condition it on other types of things, but you don't give it a text input. It's   
(01:20:10.520) ~~a little more, I guess,~~(01:20:12.225)  
a little more specific. and it's a little more geared towards people who want to perform surgery on proteins. So if you want to design new proteins with specific structural properties and you want to get your hands dirty and perform surgery on these proteins and graft them together or take pieces from this one and graft it onto this one or generate a protein with a specific sort of fold tertiary structure   
(01:20:38.881) ~~or~~ (01:20:38.921)  
or maybe generate a protein that binds to a specific protein with really high affinity and specificity. 


---


#### 01:20:47.315

These are the things that RF diffusion is good for. So RF diffusion is a diffusion model. They used Rosetta fold, the Rosetta fold backbone, and trained it as a diffusion model to denoise 3D structures of proteins. And there are several different versions of RF diffusion. There's a new version that just came out called RF diffusion all atom. which allows you to generate proteins that will bind to small molecules. So you can generate proteins with binding pockets that are highly shaped complementary to a small molecule ligand. And with RF diffusion and RF diffusion all atom, you can also do something called motif scaffolding, which is where you pull out motifs from a protein that you like. 


---


#### 01:21:32.695

Maybe they're like binding sites or active sites, or maybe there's a particular segment of the protein that binds to a different protein that you're interested in or performs a specific function. And you can pull these pieces of the protein out and scaffold them and build a new protein around those pieces that holds those pieces in place so that you have a new protein with very specific 3D structure that performs like some very specific function. And it's been a very influential model and a very useful model. And it's definitely one of my favorites.   
(01:22:06.291) ~~Maybe we should dig into that a little bit. Yeah.~~(01:22:08.212)  
Give me a little bit more on   
(01:22:09.092) ~~how,~~ (01:22:09.393)  
what exactly it is that you're specifying. 


---


#### 01:22:11.613

It's not text conditioned, but you're saying I want it to have certain properties and then it's filling in the sequence that gets you to those properties. Yeah.   
(01:22:22.460) ~~So like the most,~~(01:22:23.661)  
the most basic usage of RF diffusion is unconditional generation of a protein. So   
(01:22:28.623) ~~you just,~~(01:22:28.944)  
you tell it some length. or range of lengths, and it will just generate proteins of that length that are brand new, that have never been seen in nature before, and very often are very designable and that you can actually synthesize and create in a lab. And that's just completely unconditional generation. You don't give it any sort of constraints. It just generates a new protein for you of a particular length. 


---


#### 01:22:55.682

But then you can also, one of the really interesting functions of RF diffusion is it will design binders for you. So if I have a target protein and I want to design a protein that binds to it with really high affinity and really high specificity, RF diffusion is really good at that. It'll design binders for pretty much any protein you can give it, and   
(01:23:20.105) ~~very often~~(01:23:20.827)  
The proteins that it designs that bind to your target protein are very high affinity and very high specificity and often very thermostable. The other functionality that's really useful is the motif scaffolding that I was talking about before, which is where you pick out pieces of a protein or multiple proteins and you build a new protein that holds all those different pieces in place in a particular way. 


---


#### 01:23:47.815

And so this is one thing that you could imagine doing with this would be like building or designing an adjuvant or like grafting two proteins together. Or let's say I have one part of a protein that binds to protein A and I have some other protein that binds to protein B. And I want to design a protein that binds to both protein A and protein B so that I can get a complex with three proteins in it, right? I want to have a protein that binds to protein A and protein B. So what I can do is I can take those pieces out of the protein that bind to protein A, and I can take the pieces that bind to protein B, and I can scaffold them together into a new protein. now I've got a new protein that binds to both of those proteins. 


---


#### 01:24:36.666

And I can do things like build out protein interaction networks this way. So if I want to design a particular protein interaction network, this is really useful for that. That's a pretty technical and involved thing to do. Like building up a protein interaction network is a non-trivial thing to do, but you can do it with RF diffusion. You can design proteins that will bind to multiple different proteins in multiple different contexts and build out these networks this way. And this gives you   
(01:25:06.302) ~~like~~ (01:25:06.443)  
a way to modulate protein interaction networks, right? Because if you design a binder to block a particular interaction, you can modulate your protein interaction network by blocking particular interactions by designing a binder. 


---


#### 01:25:19.350

But you can also add in interactions that weren't there before using the motif scaffolding or maybe binder design and motif scaffolding together. So it's very useful in a lot of different contexts, but it's not text-conditioned like ProteinDT or MoleculeSTM or some of the other text-conditioned diffusion models for proteins, because there are a few others now that recently came out as well. But yeah, it's not text-conditioned. It's very much more geared towards people who are really interested in performing surgery on proteins and protein interaction networks. And now with RF diffusion all-atom, also with other interactions as well, because with the all-atom models, you can model more interactions than just the protein interactions. So how does this in practice get used? 


---


#### 01:26:05.966

Maybe the cancer example from the top is a good one, or we could go to another one. Yeah. In that scenario, we sort of already had an understanding of the cancer cell has this thing that disables the immune cell. And so then you could say, okay, let's brainstorm some ideas here, right? If we can bind something to that bit of the cancer cell that would   
(01:26:34.921) ~~kind of~~(01:26:35.202)  
cap it, blunt its ability to then interfere with the immune cell, then the immune cell presumably would do its job still and kill the cancer. Of course, you've got highly tangled webs of interaction that you're doing this within. but you've got to take something local like that. Now   
(01:26:51.815) ~~kind of~~(01:26:52.015)  
take me through the cycles and the practical application of some of these tools for a specific problem of that sort. 


---


#### 01:26:59.398

Yeah, so I've got a few examples here that we can talk about. I wonder which one would be like the best or the most interesting for people. So   
(01:27:07.381) ~~like~~ (01:27:07.520)  
the one that we were talking about earlier with the cancer, with PD-1 and PD-L1 is a really good first example that   
(01:27:13.993) ~~I think~~(01:27:14.193)  
is a really good place for pretty much anybody to start. Because you can very easily and very quickly design a binder to one of these proteins with RF diffusion. It's really good at designing binders for pretty much anything. If I have this PD-1, PD-L1 interaction between these two proteins, essentially what's happening is the cancer is turning off your immune system's response to it, and then your immune system doesn't effectively combat the cancer. 


---


#### 01:27:39.188

But if I design a binder to one of these two proteins to block that interaction, and my binder out-competes that interaction, so it has a higher affinity than the PD-1, PD-L1 interaction has, then I can successfully block that interaction and prevent the cancer from turning off the immune cell's responses to it. So that's a really good place to start. Another way that RF diffusion can be used, so let's say you have a protein that binds to a target, but it doesn't bind very well. The affinity is   
(01:28:13.770) ~~kind of~~(01:28:14.030)  
low and the shape   
(01:28:15.332) ~~complement~~ (01:28:15.752)  
complementarity isn't terribly good. I can use RF diffusion and something like protein MPNN or ligand MPNN to modify that and increase the binding affinity. 


---


#### 01:28:27.942

So something I can do with RF diffusion is partial diffusion. So   
(01:28:31.783) ~~I can get,~~(01:28:32.423)  
I can take my protein of interest that binds to my target and I can perform partial diffusion, which is where I add a little bit of noise. I don't completely noise it. I don't turn it into a Gaussian distribution or anything. I just add a little bit of noise into it. and then have RF diffusion denoise that. And what it'll do is it'll denoise it into a structure that's   
(01:28:51.698) ~~kind of~~(01:28:52.059)  
similar to the one that I started with, but it's also a little bit different now because I added that noise and then denoised it with RF diffusion. And if I do this and I give RF diffusion the target protein that I'm interested in, 


---


#### 01:29:03.842

I can improve the shape complementarity between those two. So the new denoised protein or the new denoised version of my original protein is gonna have a higher shape complementarity to my target. And then I can go and design sequences for that backbone that are different from my starting sequence,   
(01:29:21.534) ~~right?~~ (01:29:21.715)  
So maybe my starting sequence, maybe there were some residues that had unfavorable chemical properties at the interface,   
(01:29:29.037) ~~right?~~ (01:29:29.257)  
Maybe I need to use different amino acids to improve some chemical properties so that the binding affinity goes up,   
(01:29:38.002) ~~right?~~ (01:29:38.181)  
I can do that with   
(01:29:40.256) ~~like~~ (01:29:40.435)  
protein MPNN or ligand MPNN. So ligand MPNN is the newer all-atom version of protein MPNN. It's an improvement on protein MPNN, and it also generalizes to contexts where you have other kinds of molecules other than just proteins. 


---


#### 01:29:55.840

And I design a sequence with ligand MPNN, and I can tell ligand MPNN to bias certain residues towards certain amino acids or away from certain amino acids, like at the interface, for example. to get those more favorable chemical properties to increase my binding affinity further. And   
(01:30:16.033) ~~I can also,~~(01:30:16.734)  
there's also versions of ligand and PNN that will allow you to specify   
(01:30:20.596) ~~whether a residue,~~(01:30:22.297)  
so let me check on this really quick, whether a residue is a buried residue, an interface residue, or something else. I can also tell ligand and PNN about symmetries, which is a really interesting thing that RF diffusion and ligand and PNN can do together. Just to clarify, RF diffusion doesn't usually get used on its own,   
(01:30:43.881) ~~like~~ (01:30:44.021)  
by itself, because it just works in structure space, right? 


---


#### 01:30:48.823

So it's doing the denoising process on the structures of the proteins. It doesn't know anything about the sequence of the protein. So I need a separate model, like Ligand and PNN, to design the sequence for that 3D structure. So they   
(01:31:02.371) ~~kind of~~(01:31:02.631)  
go hand in hand. You use them together. So once you've generated your 3D backbone of your protein, you design a sequence for it using ligand and PNN. And using these different functionalities of ligand and PNN, you can increase your binding affinity and other properties even more. Yeah, so like using partial diffusion with RF diffusion to slightly noise and then denoise a structure that you already have. can help you increase things like binding affinity and things like thermostability and other properties. 


---


#### 01:31:33.634

Then, let's see, what's another application of RF diffusion? So one that I was looking into recently,   
(01:31:41.078) ~~let's see,~~(01:31:41.498)  
I want to pick out a good one because I want to give people really interesting examples to think about because you can really do a lot with these models if you get into it pretty deep and really learn how to use them.   
(01:31:52.905) ~~Let's see, there we go.~~(01:31:53.947)  
Okay, yeah, so there's unconditional generation, symmetric generation. I touched on that a little bit. You can design symmetric oligomers. Let's say I want to have a protein that interacts with itself, or other copies of itself, I should say. And if I have enough copies of this protein, it forms a symmetric complex. 


---


#### 01:32:19.519

For example, Let's say I have a protein that fits together with two other copies of itself in a triangle formation, right? And it's symmetric to the cyclic group of order three, right? So I've got a order three rotational symmetry that's happening. I can use RF diffusion to generate proteins with symmetry like this. And it has other symmetries that it can use. So there's dihedral symmetries, there's symmetries icosahedral symmetries and tetrahedral symmetries, in addition to the cyclic symmetries. And   
(01:32:54.372) ~~I can,~~(01:32:54.652)  
the cyclic and the dihedral, I can choose like any order, cyclic group or dihedral group for my symmetry for those. And RF diffusion will design a symmetric complex of proteins where there's like multiple copies of the protein in this like nice symmetric structure. 


---


#### 01:33:13.256

And where this occurs, like this occurs in nature in multiple places. One example is in viral capsids. And they've also recently some David Baker's lab recently published some work where they design these like symmetric oligomers as like biosensors. And I think they also designed some to help with   
(01:33:36.710) ~~like~~ (01:33:36.850)  
drug delivery. So they have these   
(01:33:39.091) ~~like the~~(01:33:39.692)  
like pocket that forms when you have a cyclically symmetric complex of proteins that the pocket that forms inside of that. You can design that in such a way that it captures a small molecule drug really well and delivers it to somewhere in particular, right? So that's another application of RF diffusion that's really useful. What else? There's the binder design. 


---


#### 01:34:04.256

#### 01:34:40.958

So it's like this, it has like beta sheets in it. And they form this, like, sort of barrel-shaped protein. Let me see if I can send this to you so that you can see it. Yeah, I've got a couple pulled up as well. Okay.   
(01:34:54.141) ~~We can add one to the... I mean, I can even share here in the moment just to capture what I'm looking at. Yeah, maybe let's share. Do that.~~(01:34:59.664)  
So this is an 8.   
(01:35:01.164) ~~And if you turn this sideways... Yeah, if you turn this sideways, it should look kind of like a barrel.~~(01:35:07.288)  
So maybe let's scroll down a little bit. I wish there was, like, a side view of this thing. Oh, there's one. 


---


#### 01:35:12.645

Do you see the red? Yeah, there it is. You see how it's turned sideways? It's   
(01:35:16.046) ~~kind of~~(01:35:16.206)  
like a barrel shape. It's like this tube. So that's a TIM barrel. So I can tell RF diffusion specific tertiary structures to generate. And it will generate these different folds for you. It's called fold conditioning.   
(01:35:31.471) ~~And then let's see. Let me find some good specific applications to~~(01:35:36.372)  
specific proteins. So here's a good example of how to use motif scaffolding. Let's say I want to design a protein inhibitor of,   
(01:35:46.284) ~~maybe I shouldn't, I don't know if I should~~(01:35:47.706)  
just read this off because this is   
(01:35:49.105) ~~like~~ (01:35:49.246)  
really technical, but there's a protein called p53-mdm2 interaction. There's two different proteins that are interacting with each other, p53 and mdm2. 


---


#### 01:35:58.630

And if I want to design an inhibitor for this, maybe I could   
(01:36:02.771) ~~like~~ (01:36:02.931)  
could extract the motif corresponding to the p53 peptide and then use that to design a new protein, scaffold that with the motif scaffolding. And then I can optimize it using partial diffusion and ligand and PNN to design sequences that have favorable chemical properties. And then I can check and see using the LIS score from alpha-fold multimer how well my new protein interacts with MDM2 or p53. These are so technical, I hate to just read these off, but I feel like I'm just going to go into the weeds and talk about a bunch of really specific proteins and domains and stuff. I don't know if that's very interesting. 


---


#### 01:36:49.171

The sort of conceptual loop, I think, is really interesting. And if I'm getting it, it's like, okay, we have an interaction that is problematic. we want to interfere with it one way or another, we can like cap the one thing or cap the other thing. And so there's this kind of cycle of generate a 3D structure, that's one model, generate a sequence to do that, that's another model, refine those, that's   
(01:37:13.905) ~~I guess~~(01:37:14.185)  
yet another model to look for various refinements or   
(01:37:18.146) ~~kind of,~~(01:37:18.407)  
as you said, chemical, favorable chemical properties? Same thing maybe? No, you don't need another model for that. You can just RF diffusion and ligand NPNN, you can do it with those two. 


---


#### 01:37:28.090

You don't need anything else really. So RF diffusion designs the structure and then ligand NPNN designs the sequence for that structure that will fold into it so that you have something you can actually go and synthesize in a lab,   
(01:37:38.712) ~~right?~~ (01:37:38.893)  
you need a protein sequence to synthesize to get the protein structure, because RF diffusion just works at the level of structure. It doesn't know anything about sequences. And then you're validating this to the degree that you can validate it before you're actually doing any actual lab work with something like Alpha Multimer and looking for a high score there. So how quick does this happen? It seems like we're talking orders of magnitude speed up compared to the pre-AI way of doing this. 


---


#### 01:38:12.764

And how accurate is it? Yeah, I mean, RF diffusion, like I can generate a single backbone in a minute, even like a pretty big one, it just takes a minute to generate a backbone. And if you have a really good GPU, that's way faster,   
(01:38:25.337) ~~right?~~ (01:38:25.516)  
If I'm just working on my laptop or something, like I can generate something in just   
(01:38:29.960) ~~like~~ (01:38:30.100)  
a minute. And then ligand and PNN is significantly faster than that. So like designing the sequence for the 3D structure is actually really fast.   
(01:38:37.623) ~~So, you know,~~(01:38:38.824)  
like per protein, And like per sequence, it's less than a couple of minutes to do that whole thing. And so I can design like hundreds of thousands of backbones and then design hundreds of or thousands of sequences for each backbone with ligand and PNN. 


---


#### 01:38:54.645

So it's pretty fast and pretty computationally efficient. And they've made some improvements to RF diffusion to reduce how many time steps you need to actually get a good structure out of it. And time again, when they actually synthesize these and check for   
(01:39:07.787) ~~like~~ (01:39:08.007)  
thermostability or specificity or binding affinity, very often they're very high. And if I have   
(01:39:15.869) ~~like~~ (01:39:15.989)  
low thermostability or low binding affinity or low specificity, very often when I use these models to improve that, they improve it dramatically. So they're pretty effective. And they're not perfect, but they're pretty good. It's not a hard thing to do to design a protein with RF diffusion and then design a sequence with ligand and pinin and get something that really does fold into that structure with high confidence or that really does interact with my target protein with high affinity and specificity. 


---


#### 01:39:48.863

Yeah. So how does this then fit into the broader validation loop? You have this one thing, you're like, going back to our cancer example, right? Oh, this part of the cancer cell interacts with this part of the immune cell and disables it. So you want to put essentially a physical cap on that thing so that is blocked and that can't happen and the cancer can get Okay, cool. So I'm going to generate potentially thousands of shapes, thousands of sequences per shape, then potentially run millions of things through an alpha fold multimer, getting scores. And then what do I do at the end of that? Do I take like the top hundred and go actually try them in a living cell? 


---


#### 01:40:33.444

Yeah, exactly. And so this seems, and you're saying they tend to work. And then I guess we also have questions of like side effects would be another big downstream question, right? We don't know what else this thing could do when put into the full environment of the cell.   
(01:40:49.037) ~~Well,~~ (01:40:49.117)  
that's where the specificity comes in, right? Generally speaking, RF diffusion is capable of designing binders, for example, with really high specificity. So they bind to the target and pretty much only bind to the target. Yeah, and it's a really good thing, right? Because if you design a binder that just interacts with a whole bunch of other stuff, it may never make it to the target. It may cause other side effects, like you're saying, have off-target effects. 


---


#### 01:41:14.773

But yeah, RF diffusion is pretty capable of designing really high-specificity binders. The motif scaffolding, there's more nuance there because you're   
(01:41:24.036) ~~kind of~~(01:41:24.356)  
performing surgery on proteins and pieces of proteins. And so that can get a little more nuanced and a little more complicated. If you're just designing a binder with RF diffusion, it's pretty easy to design one that has really high specificity and that doesn't have a lot of off-target effects and stuff. So what's the bottleneck on this process? Is it identifying targets? Especially if you can design things that are that specific and they don't have much in the way of other knock-on effects.   
(01:41:54.163) ~~I mean,~~(01:41:54.344)  
it seems like we should be curing a lot of diseases pretty quick here. 


---


#### 01:41:58.167

I think, I mean, diseases are pretty complicated and sometimes it's not just one thing that you're targeting. Sometimes it's multiple targets and multiple kinds of interactions. And so you have to think in terms of   
(01:42:09.975) ~~like~~ (01:42:10.195)  
entire   
(01:42:10.876) ~~like~~ (01:42:11.036)  
protein interaction networks or even like interaction networks that involve other molecules as well and modulating those in very specific ways. And often figuring out what parts of a protein interaction network to change or to modulate and how to do that, like what sort of changes you should make to this interaction network, that's a pretty complicated problem. And so I think part of it is   
(01:42:35.454) ~~identifying, like you said,~~(01:42:37.456)  
identifying targets or identifying specific targets within an interaction network, because some of the interaction networks can get really complicated. 


---


#### 01:42:46.020

And figuring out which parts of them to modulate is not an easy thing to do. And then Computationally, there isn't much of a bottleneck. If you just have a good GPU, you don't really need multiple GPUs even. You just have a good H100 or something. You can get a lot done with that.   
(01:43:03.257) ~~You can get quite a lot done with that~~(01:43:04.939)  
with RF diffusion and NPNN. The hardware requirements are not very taxing.   
(01:43:11.702) ~~I mean,~~(01:43:11.881)  
They're probably a little less efficient than I would like them to be, because   
(01:43:17.969) ~~I guess~~(01:43:18.208)  
most average people are not going to have access to an H100. A lot of people are going to be using much lower tier GPUs and stuff. 


---


#### 01:43:29.471

But RF to Fusion, for example, there's a Colab notebook that you can run on a T4. You can run it in Google Colab, and it takes a little while. It's not as fast. The computational bottleneck is not a huge bottleneck right now.   
(01:43:43.363) ~~I think~~(01:43:43.623)  
it could be a little better, but   
(01:43:45.425) ~~I mean,~~(01:43:45.626)  
the models aren't huge models. These aren't like billions of parameters, right?   
(01:43:50.408) ~~I think~~(01:43:50.649)  
RF Fusion has a couple hundred million parameters or something like that. Or in AlphaFold, same thing,   
(01:43:57.012) ~~like~~ (01:43:57.193)  
it's a couple hundred million parameters or something. So they're not really big models that require really excessive hardware to do the computations. And   
(01:44:05.797) ~~I think~~(01:44:06.038)  
the slowest part of that pipeline, you like design binders or design motif scaffold with RF diffusion or partial diffusion or what have you, and then designing a sequence with   
(01:44:17.519) ~~like~~ (01:44:17.639)  
protein NPNN or ligand NPNN, and then validating with   
(01:44:21.039) ~~like~~ (01:44:21.159)  
alpha fold or alpha fold multimer, the slowest part in that whole thing is actually the alpha fold multimer part or the alpha fold two part where you're validating and   
(01:44:30.823) ~~like~~ (01:44:30.963)  
predicting the structure of whatever you've generated and designed with the other two models. 


---


#### 01:44:37.234

That's actually the slowest part in the whole thing. If you're able to predict a lot of structures with AlphaFold, then you're fine. There's no real computational bottleneck there. And as far as   
(01:44:48.735) ~~like,~~ (01:44:48.956)  
why are we not curing a bunch of diseases? A lot of this also has to do with how long it takes to get these things to market. and the traditional system that's set up right now for drug discovery and protein therapeutic, it's hard and slow to get new things through.   
(01:45:08.685) ~~Like it's a~~(01:45:09.225)  
very slow system. And   
(01:45:10.805) ~~I think~~(01:45:11.126)  
it wasn't designed for high throughput methods like this. It wasn't designed for   
(01:45:17.828) ~~like~~ (01:45:17.988)  
large high throughput methods. And it just, it takes a lot of time to get a new drug or a new protein therapeutic through and approved and get it through all the testing, like the different clinical testing phases and stuff like that. 


---


#### 01:45:32.917

That's part of it. that's probably a big part of it. Are we like stuffing the pipeline at this point with new things?   
(01:45:39.484) ~~I mean,~~(01:45:39.645)  
it seems like the biggest reason that this used to be a hard thing, of course, it's like slow and there's a lot of like safety, perhaps redundant steps in there, especially if you could say, hey, we have like very high confidence that this is a highly specific thing.   
(01:45:54.194) ~~I mean,~~(01:45:54.333)  
that would really do a lot to inform   
(01:45:57.655) ~~the~~ (01:45:57.815)  
what the safety profile might be. But even if you, not even if, but in the past, it's like the biggest problem was like either it wouldn't work, right? Or it would have side effects that were like intolerable. 


---


#### 01:46:10.411

And if you could take both of those things, not entirely off the table, but if you could   
(01:46:14.231) ~~sort of~~(01:46:14.472)  
say, hey, we can be much more confident now, seemingly like at least in order of magnitude, more confident that any given thing is going to do what you expect it to do and that it won't do other things that you don't want it to do. you can improve both of those by an order of magnitude, then it's your seemingly two orders of magnitude more likely for things to work, which would take you from sub 1% a lot of shooting in the dark to a lot of the clinical trials would be expected to work. Is that the era that we're entering into now where clinical trials should go from roll the dice to you be more like disappointed when they don't work? 


---


#### 01:46:55.493

Yeah, I mean, I think we're definitely moving into an era where all this stuff is going to speed up a lot. And   
(01:47:01.216) ~~I think~~(01:47:01.556)  
so there are   
(01:47:02.756) ~~like~~ (01:47:02.936)  
a lot of situations where you want to understand more than just a static structure. Like we've been talking about, like having models that give you more dynamic information and stuff like that. And those are so recent that they haven't really been adopted by a lot of people. yet. And I think once those get used more, that'll speed things up a lot and improve things a lot as well. But yeah, I think also part of it is just adoption. A lot of researchers are not using this stuff yet because it's so new. 


---


#### 01:47:32.934

And a lot of researchers don't understand how to use these models effectively or how to use them at all. It does seem to be quite a different skill set.   
(01:47:40.975) ~~I mean,~~(01:47:41.336)  
I've actually studied chemistry. It really is. Yeah. And the kinds of things that I was taught to do were like not at all running the loops. There were no notebooks involved or no collab notebooks involved. It was like physical techniques for separating chemicals from one another was a big part of where the time went. Yeah. And that's a whole other thing too, like drug synthesis and small molecules is like a whole other story that we can get into. But because there are like really interesting diffusion models out for those as well that'll generate molecules with specific properties. 


---


#### 01:48:13.988

But Yeah, I mean, it's a very new and a very unique skill set that there aren't a lot of people that are training people to do this. There isn't a ton of information out there about how to use them.   
(01:48:26.560) ~~You,~~ (01:48:26.619)  
to some degree,   
(01:48:28.341) ~~I mean, there,~~(01:48:28.680)  
there are some platforms that are popping up and some different tools that are popping up that are making these things a lot more accessible. One that I would mention is 310AI is working on a tool that they're calling Copilot. And   
(01:48:43.564) ~~it's essentially,~~(01:48:44.484)  
it's like a chat interface that uses tools. So you can talk to it in natural language, like you talk to a chat GPT or something. And then   
(01:48:55.710) ~~it,~~ (01:48:55.750)  
it knows how to use   
(01:48:57.331) ~~like,~~ (01:48:57.551)  
like function calling   
(01:48:59.712) ~~to,~~ (01:49:00.152)  
to use other models as tools. 


---


#### 01:49:03.594

So you can say, generate a protein with such and such property, and then it'll use a particular model to do that, generate some protein with that particular property. And then you can say,   
(01:49:14.356) ~~like,~~ (01:49:14.497)  
increase binding affinity with such and such protein, and it'll modify your protein for you to increase the binding affinity or something. Or you can say, dock this small molecule to this protein, and it'll call on diff dock and dock the small molecule to the protein for you and then return that. And that's all using like a chat interface, which is making a bunch of these models a lot more accessible to people. And I think that's going to have a huge impact in the near future. 


---


#### 01:49:41.512

So. Depending on how good that gets and how fast it gets really good, that's probably going to change things substantially. And right now, it's pretty good already. And it uses a pretty wide range of tools for different things. It'll use protein MPNN or ligand MPNN to design sequences for a structure.   
(01:50:02.898) ~~I'm not sure if it uses RFDiffusion yet, but~~(01:50:05.698)  
they probably are going to start including RFDiffusion and some other models as tools for it as well. Because they just keep adding more tools to it, more models that it uses as tools. And I think once they have a good   
(01:50:18.505) ~~section or a good~~(01:50:19.545)  
selection of tools for it to use, that'll be really good. And that'll lower the barrier to entry for a lot of people. 


---


#### 01:50:27.252

Because right now you've got to go through this like somewhat complicated process of setting up these models. And   
(01:50:33.858) ~~you have to know,~~(01:50:34.618)  
you don't have to know a lot of coding, but you do have to code some and you have to understand how to set these things up   
(01:50:41.622) ~~in,~~ (01:50:41.722)  
in   
(01:50:42.182) ~~like~~ (01:50:42.302)  
a conda environment or something like that a lot of times. And so if you're not coming from   
(01:50:46.826) ~~like~~ (01:50:46.966)  
a programming background or you don't have some experience with programming, like a lot of these models are   
(01:50:53.230) ~~kind of~~(01:50:53.490)  
hard to touch. They're hard to use because   
(01:50:56.033) ~~you.~~ (01:50:56.092)  
You can't really use them unless you know a little bit of coding at least. But so 310AI, I think is going to change a lot of that and make a lot of these models a lot more accessible over time and really increase adoption of these techniques. 


---


#### 01:51:08.774

And I think that's going to be really big and important because adoption right now is pretty limited,   
(01:51:14.319) ~~I would say.~~(01:51:14.819)  
  
(01:51:14.960) ~~I mean,~~(01:51:15.161)  
just using a really simple metric by if you just look at   
(01:51:19.663) ~~like~~ (01:51:19.823)  
how many views a YouTube video on RF diffusion gets. It's not that many,   
(01:51:24.945) ~~right?~~ (01:51:25.145)  
There aren't that many people watching. This is going to be the one that goes viral and changes it all. I hope so. That would be great because adoption is going to be big.   
(01:51:33.693) ~~I think~~(01:51:33.972)  
because the more creative people you get using these things, the more you're going to see creative uses of them and   
(01:51:40.677) ~~like~~ (01:51:40.877)  
novel approaches to solving problems that people weren't even thinking of before. 


---


#### 01:51:46.082

Like when have you been able to design proteins that build out complicated protein interaction networks using binder design and motif scaffolding. That's just so brand new within the last couple of years that the adoption just hasn't caught on yet. So hopefully more people will start experimenting with these models and really learn how to use them well. And we'll see a lot of really interesting novel techniques popping up in the near future. Yeah, that's pretty remarkable. So it seems like the problem then shifts to the, or maybe it was always there in the first place, but If it is the case that given a target, we can pretty reliably and even relatively computationally efficiently come up with something that will hit the target, not hit other things, not cause a lot of collateral damage. 


---


#### 01:52:37.918

Now it's like target identification becomes the thing that really matters the most. And this seems like it's happening in a lot of areas at once. Certainly,   
(01:52:46.364) ~~I mean,~~(01:52:46.765)  
terrible analogy, but to thinking about a military environment, we've got really good missiles that can hit very precise targets, but then the targeting obviously becomes the high stakes decision. And   
(01:52:59.394) ~~I mean,~~(01:52:59.635)  
in lots of just business operations context too, right? Figuring out the right thing to do is often the hard part. So what do you think are the prospects for that sort of thing? I've been   
(01:53:10.322) ~~kind of~~(01:53:10.542)  
working through this and thinking, we've got quite a tech stack for... Obviously we can sequence lots of DNA. We can also pull out from an individual cell now what was the state of the transcriptome, what genes were being expressed at any given time, what proteins were being created. 


---


#### 01:53:31.260

I don't know quite the degree to which we can do that with small molecules with a really localized sample. but it seems like we've got like a lot of ability to generate a lot of data and to probably then create a foundation model of some sort. This is   
(01:53:49.203) ~~kind of~~(01:53:49.384)  
where Evo I sort of sense is going, even though that's not even doing all this stuff yet, but already,   
(01:53:55.728) ~~I mean,~~(01:53:56.889)  
let me just give my understanding of Evo and you can correct me if I'm wrong, but basically they're training a language model on DNA sequences purely bacteria and phage DNA from what I understand. Yeah, I was a little disappointed by that, but I think part of their reason for doing such a specific selection was for safety reasons. 


---


#### 01:54:21.442

I think they're trying to be a little cautious about what they train on and what the model is capable of doing for safety reasons. But I was a little disappointed that they only trained on that data, for sure. Hopefully there'll be another version at some point that's train on other data as well, but yeah. I'm sure there's a lot more to come.   
(01:54:41.038) ~~You kind of glitched on me for a second, but~~(01:54:42.640)  
so they train on all this data. Now they can generate sequences in the same way that a language model can generate text, right? Then autoregressive, byte by byte, base pair by base pair generation. And then there's these really interesting things that they can do downstream of it where, for example, a gene essentiality score or test Basically, if you change a sequence in a particular gene and generate from that changed sequence it seems that the model has developed a sort of, as we've talked about a couple of different contexts, this sort of higher order understanding of how things fit together, such that if you do make a change to something that really matters, then you see sort of an unraveling of the later generation. 


---


#### 01:55:37.242

Like you see a very high perplexity downstream of this changed sequence. And that reflects the fact that, hey, if you've changed that sequence, I can't really make any confident predictions now because we're   
(01:55:50.270) ~~sort of~~(01:55:50.610)  
outside of the set of things that can work. And so once you change that, it's all kind of noise. Whereas if you change something and predictions remain confident downstream, then you infer that must not have been super important. That was an area that more easily could be, change could be tolerated in that particular sequence because, and we can infer that from the fact that it continues to make confident predictions downstream. That's pretty remarkable stuff that suggests to me that especially as we scale up the data set a lot more, which in this one was 300 billion. 


---


#### 01:56:27.958

I mean, that's not nothing, but it's not much compared to what we could easily imagine doing. Certainly not much compared to the 15 trillion tokens that Mediterranean Plasma 3 on, but then also like more modalities, right?   
(01:56:38.604) ~~I mean,~~(01:56:38.724)  
we're seeing this in the language models where you can have obviously language integrated with image and plenty of other things. Audio now fits into Gemini 2. It seems like you sort of imagine from just the DNA to   
(01:56:51.489) ~~sort of~~(01:56:51.810)  
the DNA and maybe the transcriptome or the proteome or whatever the sort of state of a cell is. You can even imagine scaling this up another degree to   
(01:57:02.488) ~~sort of~~(01:57:02.710)  
the systems level too. But to learn to predict the next state from the current state seems like we're getting really close to being able to do that. 


---


#### 01:57:15.193

I would kind of expect that in the next couple of years at most, we would start to see large scale foundation models for biology that would predict like how a cell will evolve through time, how a system level description will evolve through time. And then you can start to do these counterfactual hypothetical perturbations and see, okay, if we change this, then how will that make things evolve? If we change this, how will that make things evolve? And so then I guess what we would expect to be learned by those systems is what is now the black box, right? Of all these interactions that we have only mapped out, whatever, 5% of. And then you could even imagine a situation where you start to do interpretability techniques on digital neural networks to then figure out what the actual pattern of interactions is in the actual biological systems. 


---


#### 01:58:08.935

So is that where this is going over the next couple of years?   
(01:58:11.756) ~~I mean,~~(01:58:11.956)  
and then it seems like if we can achieve that, then you   
(01:58:14.777) ~~kind of~~(01:58:14.997)  
have a fairly closed loop of, okay, we can now identify good targets at a pretty high rate. We can identify or design interventions that are pretty likely to be successful. The like specificity is already high.   
(01:58:30.225) ~~I mean, it's~~(01:58:31.166)  
we're entering into   
(01:58:31.865) ~~sort of~~(01:58:32.145)  
a super steep part of the S-curve in terms of not just   
(01:58:36.429) ~~like~~ (01:58:36.588)  
understanding biological systems, but really being able to intervene in them. And it just seems like a totally different regime that we're headed for. So is that what you basically expect to see over the next couple of years? 


---


#### 01:58:47.395

I mean, I hope so. I hope that all of that comes to reality or comes into existence. Sorry, We pause for a second. I need to get some water. OK, hold on just a second. We're back. OK,   
(01:58:57.953) ~~I think we're~~(01:58:58.335)  
I think we're all set. Yeah. OK, I'm feeling a little better now. So where were we?   
(01:59:03.783) ~~What were we talking about?~~(01:59:04.685)  
You were hoping that my seemingly I'm like extrapolating from where we are and I'm also sort of mapping what has happened with language model foundation models onto the biological domain and feeling like it's about to get crazy. So you're hoping that happens.   
(01:59:22.601) ~~I, yeah. I mean,~~(01:59:24.042)  
I think it's about to get crazy for sure. 


---


#### 01:59:26.283

I think like we're fast approaching a scenario where all of these technologies are going to kind of converge and we're going to have a lot of power over. editing and modifying our biology. And I think that's a very exciting thing because there's a lot of problems that I really want to see solved in my lifetime. And I think we are definitely moving in the right direction. And I think we are fast approaching a situation where we can actually solve a lot of these problems. And   
(01:59:53.390) ~~I think,~~(01:59:54.032)  
so like the main thing that you're talking about is   
(01:59:56.952) ~~like~~ (01:59:57.112)  
this complicated sort of hierarchical structure that's happening. And the level that I think at most of the time is at the level of like molecule interactions. 


---


#### 02:00:10.912

But you can definitely take that up another level and look at how those interactions come together in a network to create a particular sort of   
(02:00:23.216) ~~like~~ (02:00:23.398)  
phenotype or to create a particular sort of state of the organism, right? And   
(02:00:29.139) ~~like~~ (02:00:29.300)  
some of those states are diseased states that we don't want. Figuring out,   
(02:00:35.117) ~~like,~~ (02:00:35.356)  
how to modify these interaction networks,   
(02:00:39.219) ~~I think,~~(02:00:39.578)  
is somewhere that we really need to focus on a lot. And one thing that's really useful and that I really want to see pushed further is this notion of LIS score with alpha fold multimer and seeing also,   
(02:00:53.524) ~~like,~~ (02:00:53.664)  
things like alpha flow or distributional graph former generalized to complexes, to,   
(02:01:00.167) ~~like,~~ (02:01:00.307)  
complicated complexes of molecules and not just one or two proteins or something. 


---


#### 02:01:06.259

I really want to see more progress happen there because once we understand all of the interaction networks and we're able to modulate them in very specific ways,   
(02:01:16.524) ~~we're going to solve a lot of problems,~~(02:01:18.645)  
a substantial amount of problems. Modeling these interaction networks is becoming possible now.   
(02:01:24.448) ~~I think~~(02:01:26.149)  
before alpha-fold multimer, And before some of these other docking methods, and before RosettaFoldAllAtom came out, we really didn't have the tools to model all of these different interactions. But we have very recently just hit a point where we do have most of the tools that we need, if not all of them, to model all of these interactions. And once we implement something like alpha flow or distributional graph form for complicated complexes of molecules, that's really going to be pretty substantial. 


---


#### 02:02:00.289

And I personally, I'm not sure how I would approach the problem of determining what specific interactions or interaction networks to modulate.   
(02:02:14.180) ~~Like, I personally, like,~~(02:02:15.520)  
that feels like such a big problem to me. But I also know that there are a lot of biologists that know specific interaction networks they want to modulate, and they want to modulate them in very specific ways. And there's a lot of that. And now we can do that.   
(02:02:32.265) ~~I think~~(02:02:32.546)  
we just need to get these tools into the hands of those biologists and make them really accessible. Because they're not super accessible yet.   
(02:02:44.194) ~~They are kind of, right? I mean, like~~(02:02:46.115)  
a lot of them are open source and they're out there and you can get the model weights and a lot of them have the training code and the inference code and all this stuff available. 


---


#### 02:02:55.663

But probably your average biologist is not going to know how to use those tools right now. So making them accessible and easy to use is really where a lot of the work is going to be as well. Because there are a lot of people that want to do these things, but   
(02:03:13.197) ~~they don't~~(02:03:13.737)  
they haven't quite gotten to the point where they've adopted all of these tools yet. And also figuring out how to use them all in tandem with each other, right? Because you don't want to just use one of these models. You want to use multiple and use them all together to solve a problem. And so that requires you to learn   
(02:03:34.689) ~~like~~ (02:03:34.829)  
multiple different models and how they work and how to use each one of them. 


---


#### 02:03:39.412

And that's not an easy thing to do for a lot of people. Yeah.   
(02:03:42.055) ~~The, I mean,~~(02:03:42.494)  
this is the issue in AI, even in much more,   
(02:03:45.417) ~~you know,~~(02:03:45.777)  
simple use cases of just using change UPT effectively the sort of diffuse, the technology diffusion through society   
(02:03:52.060) ~~is,~~ (02:03:52.201)  
is really the big bottleneck   
(02:03:53.782) ~~I would say~~(02:03:54.141)  
right now to when people say   
(02:03:56.144) ~~like,~~ (02:03:56.224)  
why hasn't, if change UPT is so great,   
(02:03:58.024) ~~like~~ (02:03:58.145)  
why hasn't it,   
(02:03:58.925) ~~you know,~~(02:03:59.185)  
changed productivity all that much? It's like, people are not using it nearly as much as they could is one really big reason. So a huge reason. Yeah. If I had to   
(02:04:06.569) ~~kind of~~(02:04:06.789)  
map out the story of the next couple of years as I understand it, or as I'm   
(02:04:10.752) ~~kind of~~(02:04:10.912)  
piecing it together from everything that you're teaching me about, it is right now we have a big backlog of targets and we have a pretty robust new set of tools that used together can design things that will hit those targets and not create too much collateral damage such that it's not super hard. 


---


#### 02:04:40.585

It's hard to learn to use the tools, but once you have the skill set, it becomes relatively easy to take a target and crunch through a bunch of iterations and come to a bunch of candidates. And those are likely enough to work that we should start to see serious acceleration of the ability to find the solutions to these well-posed problems. And then   
(02:05:08.011) ~~sort of~~(02:05:08.532)  
in parallel, we should probably also expect that Evo 5 or whatever, Evo 4 will be capable of dramatically better holistic modeling of the overall networks. And that will then, once we   
(02:05:27.560) ~~sort of~~(02:05:27.840)  
deplete the current set of targets, that have been painstakingly worked out through non AI methods   
(02:05:37.471) ~~sort of~~(02:05:37.733)  
seems, 


---


#### 02:05:38.073

I don't know. Why does it always seem like it happens at the same time? It's always these sort of gradual overlapping curves, but my gut says we've got a few years in front of us of. depleting the current, or not depleting, but like picking the sort of low hanging fruit of, hey, we've got all these targets out there and now we've got good methods to hit those targets. That's going to take a while for people to learn the tools, do it, obviously validate it, run clinical trials going in lots of different areas. And then as the sort of current backlog gets worked through, it's probably a better way to phrase it. Right around the same time, 


---


#### 02:06:09.768

I sort of expect that all of a sudden the tension will turn to, Oh my God, now we have these foundation models that kind of model the whole causal graph in all of its crazy complexity. And now we're actually going one level out and saying, now we can apply similar computational techniques to the identification of the targets. And we'll do that in   
(02:06:33.943) ~~sort of~~(02:06:34.144)  
a similar way of being like, okay, I want   
(02:06:37.145) ~~this, this is~~(02:06:37.907)  
what's happening and I want to prevent it from happening. or this is what I want to happen proactively that isn't currently happening. Let me just   
(02:06:45.833) ~~kind of~~(02:06:46.033)  
brute force my way through a bunch of perturbations to the, and of course we can get better than brute force too, but even just imagining   
(02:06:53.921) ~~a sort of~~(02:06:54.483)  
several couple generations down of Evo, it seems like make a tweak, see what happens is going to be so radically accessible from a computational perspective that will then also just have this explosion of like quality targets to identify. 


---


#### 02:07:09.011

And yeah,   
(02:07:10.573) ~~I mean,~~(02:07:10.773)  
what do you think the world looks like as all that happens?   
(02:07:14.115) ~~What is,~~(02:07:14.416)  
it seems like we may be not super far from a,   
(02:07:19.479) ~~this is not, we're not even in a world here of like an,~~(02:07:21.319)  
any sort of AGI,   
(02:07:22.501) ~~right?~~ (02:07:22.661)  
We're talking like, these are still tool simulated simulation and tool type things that people would be using that we're not assuming anything here about AI agents doing the work. Although you did have a little bit of that with the 310 co-pilot. but is there anything that I should be like reigning in my expectations on?   
(02:07:42.279) ~~I mean,~~(02:07:42.500)  
are there things about like one tweet that I sent you was around to what degree can these things handle sort of point mutations or whatever? 


---


#### 02:07:49.724

And there's maybe individual idiosyncrasy becomes a really hard problem at some point, but like how far does this paradigm that I'm sketching out extend, do you think? And what limits does it hit? Yeah,   
(02:08:01.891) ~~so I think,~~(02:08:02.332)  
so just briefly on   
(02:08:04.552) ~~like~~ (02:08:04.712)  
point mutations or like more complicated mutations where you mutate multiple things and just predicting how positive or deleterious that mutation or set of mutations might be on the protein or something. That's a capability that ESM has, and that's already two or three years old at this point. And Evo does it. They got state-of-the-art performance with Evo on predicting which mutations were positive and which mutations were negative and which sets of mutations were positive or negative. 


---


#### 02:08:40.011

And you can compute a few different things, a few different kinds of scores that tell you about this. you can actually build out evolutionary trajectories to show over time how things are likely to evolve based on how positive or negative the impact of a mutation is on protein or something or DNA sequence or whatever. And Evo, they got state-of-the-art performance on this. And that's actually, they also did this with alpha folds.   
(02:09:08.131) ~~I think~~(02:09:08.353)  
they called it alpha missense or something like that, where   
(02:09:11.713) ~~they just, I think they, what did they do it for?~~(02:09:14.015)  
Did they do it for   
(02:09:15.164) ~~I think they did it for~~(02:09:15.985)  
all the proteins, all the human proteins, but maybe it was a bigger dataset. 


---


#### 02:09:20.453

I can't remember. But they predicted all the single point mutations and all the effects   
(02:09:23.779) ~~that~~ (02:09:23.859)  
that those have. And that's actually not a hard thing to do. So mapping out how a mutation affects a protein or DNA or something, and the course of evolution that's likely to occur, that's actually pretty easy to do now. And then as far as... I also want to draw attention to another project that I'm aware of. It's not a model per se, but   
(02:09:46.514) ~~they are using... I think~~(02:09:48.095)  
they are using GPT-4 They may have trained their own in-house model. I'm not sure. But there's a company called Future House, and they're designing an agent, an autonomous agent, that will do a lot of this research for you. 


---


#### 02:10:05.835

And it'll do things like literature search and review, and come up with hypotheses of different kinds of interaction networks that you might want to modulate or different targets that you might want.   
(02:10:19.246) ~~And it'll do this and it'll do it pretty well.~~(02:10:22.127)  
And that's a pretty new thing that just started happening   
(02:10:26.828) ~~like~~ (02:10:26.988)  
last year,   
(02:10:28.247) ~~I think,~~(02:10:28.887)  
maybe late last year. And they're getting pretty good results with that. And that's actually using an LLM like as the base, right, to build an agent to do this research. And then   
(02:10:41.194) ~~I think~~(02:10:41.515)  
they're also building an autonomous lab that drives itself. So once the agent comes up with hypotheses or targets or what have you, the lab is autonomous as well. 


---


#### 02:10:54.240

And that's a pretty exciting direction. I think that, coupled with some of these more specific tools to perform these fine-grained operations on proteins and small molecules and DNA and RNA. When those two   
(02:11:09.750) ~~kind of~~(02:11:10.051)  
converge, that's going to be a really big deal. And I see that happening in the next year. The progress that they're making at future houses is really impressive,   
(02:11:21.076) ~~I think.~~(02:11:21.416)  
So that would also be something that people should definitely look into. And I think your timeline is within a couple of years for sure. I don't think it's going to be that long before we start seeing substantial progress and changes.   
(02:11:34.712) ~~I mean,~~(02:11:34.953)  
OpenAI just partnered with Moderna, right? Yeah. Hundreds of GPTs. 


---


#### 02:11:39.655

I'm sure that's just the beginning. And   
(02:11:41.578) ~~I think~~(02:11:41.858)  
that also is like a paradigm that's going to match well with these other more specific tools, because when you enable an agent to use tools, you unlock a lot of possibilities, right? When you enable something that can review thousands of research articles, then develop targets or hypotheses to test, and then can call on these specific tools to design molecules or proteins or nucleic acids to perform these specific functions or hit these specific targets. That's going to move really fast. And   
(02:12:20.988) ~~I think~~(02:12:21.269)  
I'm excited. I'm also a little nervous because I think there's a lot of a lot of potential for misuse in the wrong hands. The sort of things that you can accomplish will be amazing and beautiful. 


---


#### 02:12:36.601

And we're going to see a lot of health problems just disappearing. We're going to see lifespan extended. And that's going to   
(02:12:43.528) ~~really increase or~~(02:12:44.748)  
really improve the quality of life for everyone. But also, we do have bad actors in the world. And that is something I worry about for sure, because in the wrong hands, we could be looking at very dangerous things as well. And so having some kind of oversight for these things is very important. Because,   
(02:13:02.527) ~~I mean,~~(02:13:02.766)  
we're looking at moving into an age where you could target a specific group of people based on their genetics or something. That's both immensely useful and also very dangerous. I have a lot of faith in the people that are working on these things, like the people that are building these models and doing this research are really good people with a lot of really good intentions and a lot of know-how and experience. 


---


#### 02:13:29.033

And that to me is very reassuring, but there's always some random jerk that has the potential to mess it up for everyone. We have to be prepared for that. Yeah, no doubt. Preparing for this, definitely one of the major updates that I've made is that when people talk about the bio risks from AI, the conversation that I've heard most of has been like, how does it compare to Google? How does GPD 4 compare to Google? Does it make it easier for you to get certain information or figure out how to do certain things. And in familiarizing myself to the degree that I have with all this technology, it's   
(02:14:12.765) ~~like,~~ (02:14:12.965)  
that all of a sudden feels very quaint already. 


---


#### 02:14:15.908

It's like, this is not a question of comparing to Google. This is like generating entirely new stuff. And I looked back not long ago at the list of mass extinctions in the history of the planet and what caused them. Of course, some were caused by totally exogenous shocks, like an asteroid hits the Earth. But the first one on the list on Wikipedia is the oxygenation of the atmosphere. And it's simply that something   
(02:14:47.875) ~~kind of~~(02:14:48.234)  
pops up and either itself, nobody knows how to eat, or it creates some waste product that,   
(02:14:56.980) ~~you know,~~(02:14:57.240)  
that nobody's prepared to deal with. And what we now breathe and depend on was at one point, the cause of a mass extinction event. 


---


#### 02:15:07.007

I kind of try to keep these like zeroed out perspectives in mind. And it does seem,   
(02:15:11.291) ~~I mean,~~(02:15:11.610)  
tell me if you think there's any limitation to this or whatever, but with this sort of brute force search through   
(02:15:18.854) ~~sort of~~(02:15:19.095)  
biological space, right? It seems like there's not really anything conceptual that I could identify preventing, talk about gain of function type research. on a totally different level. Things that nothing can eat. That's like the most dangerous stuff, right? It's the stuff that nobody can break down. And I gather that trees were essentially at one point that too, right? Before something developed that could break down the hard fibers. tissue of a tree, it was just piling up. 


---


#### 02:15:52.716

Globally, I understand that's basically where a lot of coal came from, is that trees would fall, nothing could digest them, and so they would just   
(02:16:00.082) ~~sort of~~(02:16:00.341)  
collect and eventually they turn into coal. I'm sure there's a lot of different stories of coal formation, but these moments of something that nothing is really prepared to deal with, those seem like the really dangerous things. And I don't know how you prepare yourself for that. I think there are multiple things that we can do to help   
(02:16:17.755) ~~prevent~~ (02:16:18.176)  
prevent some of these bad things from happening. And I think we're going to need to rely on the models that we build, especially the agentic models that we build, to help guide us in some of this. 


---


#### 02:16:31.382

Because at some point in the near future, we're going to have agents based on really robust language models or something similar, and they're going to be able to review thousands of research papers and do tests in a lab on things, take in an amount of data that we can't really take in, right? That no human or even group of humans can really take in and process and digest and use.   
(02:17:00.879) ~~Like~~ (02:17:01.120)  
the scale is going to be much larger than a human can really work with. And so we're going to have to rely on some of our models to help guide us. And also,   
(02:17:14.045) ~~Like,~~ (02:17:14.204)  
going back to how does it compare to Google, I think another argument that could be made for why not to worry about some of these things is, okay, maybe I can get on my computer and design some new thing that was really toxic or something, but I still have to go into a lab and synthesize all that stuff. 


---


#### 02:17:35.679

And a lot of that part of the process is very highly regulated and watched, right? I can't just go get a bunch of random chemicals and build this stuff in my house, right?   
(02:17:47.121) ~~Like~~ (02:17:47.281)  
it's harder to do than that. And like synthesizing proteins is, it's a non-trivial process. So   
(02:17:54.206) ~~like~~ (02:17:54.365)  
a lot of the worry, I think of, Oh God, we're going to have an AI that designs a deadly virus or a bioweapon or something. A lot of that is really overblown, especially at the moment. And I think a lot of people overlook the fact that computationally designing something computationally designing a molecule is just one step in the process. You also have to do all the lab work and synthesis and work on some kind of delivery mechanism. 


---


#### 02:18:23.900

And this is all stuff that's non-trivial to do and that helps prevent bad actors from actually going through with some of this stuff. Now there may be like state-sponsored bad actors with access to good labs and lab equipment that will circumvent a lot of that. But when you're working at a state-sponsored level, that's a matter of international relations and also national security. I think that has almost nothing to do with AI. The computational design of some random toxic molecule is just one step in a complicated process. People don't often think of that. I see a lot of very influential, big name people in the industry who are coming from the NLP side of things and the LLM side of things. 


---


#### 02:19:20.570

They don't really understand the biology and the process that goes into actually making these things. I think their worry is justified, but they're also not understanding the nuances and where the dangers actually are. So   
(02:19:36.372) ~~I think~~(02:19:36.593)  
it's important for people to keep that in mind. I think it's very important before we start getting all anxious and worried about some random person using Lama 3 to design a superflu or something, you have to remember it's very unlikely and very difficult for just a random average person to go through the entire process of designing and synthesizing and delivering some kind of toxic molecule. That's a long, difficult process that an individual would be very unlikely to be able to accomplish, even with the help of a very intelligent LLM or a very capable agent. 


---


#### 02:20:16.516

Now, when you have larger research-oriented companies working on these things that have their own wet labs, and they're building agents to run these wet labs and to computationally design the molecules and form plans on how to use them. There, I can see, okay, we need some kind of oversight. We need some people working on how to make sure that process is safe, how to protect that information and data and equipment,   
(02:20:49.217) ~~right?~~ (02:20:49.477)  
Because there are plenty of situations where something like corporate espionage is happening and people are trying to do nefarious things with some of the technology that some of these companies have. But again, that has very little to do with the AI itself and has more to do with how we're interacting with other countries and other research organizations. 


---


#### 02:21:14.265

So definitely we need to be developing plans for how to use and regulate and oversee a really capable agent that is going to go through the entire process of computationally designing and verifying and then also synthesizing and delivering. And that is technology that is in existence now. We already have agents that are doing most of this process. And a lot of people are pushing for more of that, which I agree with, because we're not going to be able to solve these problems on our own. We're going to need some kind of really capable agent that can help guide us through these processes, because they're so complicated. and so difficult to understand the whole picture and all of its nuances that I don't know if humans can get there without some kind of agent helping out and helping design the molecules and producing it and delivering it and etc. 


---


#### 02:22:12.780

I don't know if we can get there without that, but I guess my concern is just making sure that these companies and organizations that are building this technology and using it have some people that are overseeing the safety side of things and that are concerned with red teaming and preventing things like corporate espionage and making sure that everyone that's using that technology is using it responsibly and making sure   
(02:22:37.902) ~~that we're like~~(02:22:38.561)  
that the companies are hiring not just capable people but also   
(02:22:43.565) ~~like~~ (02:22:43.704)  
people with good moral grounding and good intentions. Yeah I guess   
(02:22:49.349) ~~that's where I mean~~(02:22:50.530)  
that's not even the future that's   
(02:22:51.970) ~~kind of~~(02:22:52.230)  
now, That's already a concern that we need to address now, because we already have agents that are doing these things. 


---


#### 02:22:59.191

Most people don't have access to them, though. Most people don't have access to a really capable agent that can do this whole process or do most of this process. That's not something that even most companies have access to, much less individuals, because a lot of these models are closed. I could see maybe some kind of   
(02:23:19.481) ~~like~~ (02:23:19.682)  
state-sponsored group of researchers could use open source models to build something similar and do something nefarious, but that's a whole,   
(02:23:28.084) ~~like,~~ (02:23:28.304)  
it's a very complicated process of building such a thing. And I don't know if I have a good answer for how to combat something like that or how to address something like that. I don't know if there's a good answer. to that right now. 


---


#### 02:23:41.289

It's certainly hard to identify a more important question.   
(02:23:43.829) ~~Do you think that the,~~(02:23:44.611)  
do we have any read on whether offense or defense is favored here, so to speak? In the sense of for nuclear weapons, for example, if one of the major nuclear powers fires all its missiles, nobody can shoot all those missiles down. It seems to me that is an offense favored regime. And so we're   
(02:24:03.138) ~~kind of~~(02:24:03.378)  
stuck in this   
(02:24:04.418) ~~like~~ (02:24:04.638)  
mutually assured destruction paradigm, which is yikes. We   
(02:24:09.621) ~~kind of~~(02:24:09.861)  
need to get to a different paradigm because we're under real threat of nuclear catastrophe as long as we've all got thousands of missiles pointed at each other and no viable defense. I don't have an intuition for if biology works the same way or not. 


---


#### 02:24:27.813

I think this is less of a question about biology and more of a question about cybersecurity because I think it's like very similar in spirit to like cyber security and there as well most often the attacker has the advantage over the defender but there are a couple of things that may change that one is really capable agents because if you have a really capable agent that's able to defend against human attacks that are   
(02:24:56.250) ~~like~~ (02:24:56.409)  
just inferior that's going to be a really big part of protecting against bad actors and so   
(02:25:03.174) ~~i guess like~~(02:25:03.655)  
That's an argument for acceleration, actually, because if you have the most capable agent, then probably your defense is going to be a lot better than everyone else's. 


---


#### 02:25:13.737

And if your agent is capable enough, it may be effective enough to ward off pretty much anything. And I don't know how soon that's going to come into the picture, but I think that is a good argument for keeping up the pace of development of LLMs and agents and things like that. There was another point that I wanted to touch on, and   
(02:25:33.406) ~~I think~~(02:25:33.587)  
I forgot. I already forgot what it was, though. Anyway, yeah, I think the advantage of the attacker over the defender may end up shifting because of agents. We may end up having a situation where that's no longer the case. And, yeah. I'm a little confused about why are you making a... 


---


#### 02:25:52.231

Why is the shift from biology to cybersecurity? Because I'm envisioning a world where For example, Evo is open source, Llamo 3 is open source. If Evo 3 is open source, then we start to, at some point, we enter into a regime where, yeah, it may not be easy. It may be hard for one person. but at some point it does get like lower than state actor level where somebody could launch some crazy attack and then it's okay. If you create some super bug with certain properties, can we defend against it?   
(02:26:28.219) ~~I'm a little bit unclear as to how you're,~~(02:26:30.220)  
I'm not sure if you're like equating that to cybersecurity or saying that's primary somehow. No, 


---


#### 02:26:35.084

I guess, no, I think that's a good point. Yeah. Because if you develop some kind of,   
(02:26:39.367) ~~I think,~~(02:26:39.666)  
I guess a virus is probably as good an example as any, but let's say you develop a virus of some kind that targets a specific population. Developing a cure for that traditionally has been a very slow process. And like the fastest that we've ever done it was probably COVID. And that still took some time, right? And on the other hand, there is recent work that came out of, it was the University of California, but I'm not sure which one. They recently published some research about   
(02:27:10.068) ~~like~~ (02:27:10.228)  
universal vaccines. And they're able to design a vaccine that was like applicable to a wide range of mutants of a virus. 


---


#### 02:27:18.816

#### 02:28:01.856

That's definitely a very good data point.   
(02:28:05.138) ~~I mean,~~(02:28:05.337)  
my kind of default would be just to think I have three kids and I'm no expert in how babies develop in the womb, but it's definitely clear that a lot of things have to go right. Like an unbelievable number of things have to go right in the proper sequence. At any point, if something goes wrong, like that could be the end of it. My general default model would be like, a lot of things have to go right and only   
(02:28:31.750) ~~kind of~~(02:28:31.969)  
one or two big things would have to go wrong. And so it seems like there's a lot of surface area to defend and a lot of kind of places that could be attacked. 


---


#### 02:28:42.300

But then, hey, if you can make a universal vaccine, then all of a sudden that does start to look quite a bit different.   
(02:28:49.667) ~~So yeah, boy.~~(02:28:51.168)  
Yeah.   
(02:28:51.449) ~~I mean, it's,~~(02:28:51.748)  
and I think you're right also to say a big part of this does seem to be   
(02:28:54.871) ~~sort of~~(02:28:55.152)  
what is the prevailing,   
(02:28:57.373) ~~like~~ (02:28:57.555)  
international relations regime, because if it seems like pretty safe to say, if we get into a bioweapons arms race, we're going to be in bad shape. we really have to have some more globally cooperative approach. Or the missiles have one really nice property, which is they don't spontaneously escape their silos and self-replicate around the world. Whereas the list of lab leaks is quite long. 


---


#### 02:29:29.396

It just seems like there's no way that we can get into an international bioweapons arms race and survive it. We just have to avoid that trap in the first place. I hope we do. What happens when you develop cures for a wide range of diseases and you're able to extend human lifespan significantly longer than what it is now and eliminate a lot of the diseases that we face? Once that exists,   
(02:29:58.860) ~~I don't know,~~(02:29:59.299)  
maybe that's a paradigm shift.   
(02:30:01.041) ~~Maybe that's a,~~(02:30:01.882)  
that's like a shift in human consciousness at that point. And we start thinking about things very differently because we're all used to thinking about   
(02:30:09.909) ~~like~~ (02:30:10.129)  
everything in terms of being finite. And   
(02:30:14.093) ~~I think having,~~(02:30:15.593)  
having an approach or thinking about things in a way that isn't finite anymore and thinking about things in terms of how valuable our health and our life is because of the fact that enables us to be with who we love for longer. 


---


#### 02:30:31.581

The time that we have with the people we care about is, in my opinion, the most valuable thing that we have. And once you enable people to have healthy lives with people they care about, more or less indefinitely, that changes a lot. And I'm very excited to see. I hope that happens in my lifetime. I think it will. I think it'll probably happen within the next decade even. But I hope that really changes human consciousness to a point to where a lot of these problems just   
(02:31:02.572) ~~kind of~~(02:31:02.832)  
start to go away because we stop thinking of everything in terms of finite resources, finite lifespans, finite time with the people that we care about. Hopefully it's enough of a conscious shift in consciousness that we see some of these problems fading because a lot of them are cultural, right? 


---


#### 02:31:20.583

A lot of these problems or a lot of these like threats at the heart are very cultural. It's not about the technology. It's about how we use the technology and how we're interacting with each other when we use it. And that requires people to think differently. It's not a problem that can just always be addressed with some new technology or some new defense mechanism. We really have to change our thinking. And   
(02:31:49.334) ~~that,~~ (02:31:49.575)  
I hope that when these things start becoming widely available, people's thinking will shift dramatically. Maybe that's where things are headed. I actually have a lot of hope that's where things are headed and a lot of optimism because I think overall, like most people are good. 


---


#### 02:32:06.618

And I think like we can heal a lot of things, not just health problems, but a lot of psychological things we can heal with these tools because it's going to change the way that we interact with each other and the way that we perceive our environment and our relationship to it. That is beautiful sentiment and maybe a good place to end. I don't know if there's anything else that you wanted to touch on, but hard to hit a more aspirational note than that.   
(02:32:32.663) ~~I know.~~(02:32:33.003)  
Yeah,   
(02:32:33.504) ~~I think~~(02:32:33.824)  
I agree with you.   
(02:32:35.065) ~~I mean,~~(02:32:35.284)  
as far as other things to discuss, I don't know. I think we've probably discussed pretty much everything I had. And we talked about most of the models that I found interesting. 


---


#### 02:32:45.041

So yeah,   
(02:32:46.423) ~~I mean, yeah,~~(02:32:46.763)  
I think that's a good place to stop too.   
(02:32:49.363) ~~I think~~(02:32:49.584)  
we can probably call it there. And this has been really great,   
(02:32:53.532) ~~by the way.~~(02:32:53.972)  
I had a lot of fun doing this and I really appreciated this.   
(02:32:57.434) ~~This is great.~~(02:32:57.816)  
I appreciate you being willing to spend so much of your Saturday teaching somebody who doesn't know nearly as much as I suddenly feel like I really should about this area. So feelings definitely mutual. I guess my closing thank you is Amelie Shriver. Thank you for being part of the Cognitive Revolution. Of course. Thank you for inviting me. 


---



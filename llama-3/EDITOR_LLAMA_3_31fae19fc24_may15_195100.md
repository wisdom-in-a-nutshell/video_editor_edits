#### 00:00:00.129

Amelie Schreiber, computational biochemist and AI researcher. Welcome to the Cognitive Revolution. Nice to be here. I'm excited for this conversation. I expect to learn a lot from it. Quick context on my end. This all started with a tweet that I saw you put out probably two months ago now. where you said, here are my top 10   
(00:00:20.329) ~~tools,~~ (00:00:20.769)  
top 10 AI tools for biology in no particular order. And I read down the list and I was like, I don't know what any of these are. So when that happens, I'm immediately like, okay, this is an area that I need to do some remedial self-education in. And reached out,   
(00:00:37.215) ~~I think~~(37.415)  
pretty much immediately to say, hey, would you be interested in educating me in the form of a podcast? 


---


#### 00:00:41.796

So I appreciate you taking the time to prepare for this and do it. You want to start off by just giving a little bit of context on who you are, what you're doing day to day and what kinds of problems maybe you're trying to solve. And then we can step back again and give people   
(00:00:54.932) ~~kind of~~(55.133)  
foundational knowledge. Yeah,   
(00:00:57.069) ~~sure. Yeah,~~(57.67)  
I'm an AI researcher and I focus on computational biochemistry applications. I actually started out as a mathematician. My training in grad school and stuff was in mathematics, actually. Started off with pure mathematics and then transitioned into applied mathematics and data analysis type stuff. And then after grad school, I got into the deep learning stuff and started working on more AI related things. 


---


#### 00:01:20.305

Yeah, I think, and for me, like the biochemistry applications are one of the most compelling things that we could be working on right now. I think other than   
(00:01:29.093) ~~like~~ (00:01:29.233)  
AGI, whatever that means, I think it's probably the most important problem we can be working on because it's a huge impact on human health. The applications in human health and medical applications are really profound and have the potential to be very impactful and for everyone too. So I get really excited about the biochemistry applications of AI. And yeah,   
(00:01:52.856) ~~I guess~~(113.117)  
that's a little about me. Was there anything in particular that you wanted to know about my background or experience? Maybe just the context that you're working in today a little bit would be helpful to understand how it is that you're exploring these tools and applying them. 


---


#### 00:02:04.804

Obviously, again, we're going to have to get into more detail on what they are, but yeah, just   
(00:02:09.366) ~~kind of~~(129.587)  
where in the world are you situated that you're doing all this stuff?   
(00:02:13.308) ~~So, I mean,~~(133.75)  
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
(00:05:07.735) ~~kind of~~(308.016)  
a couple of the biggest sorts of problems that I understand are being studied in biomedical sciences. 


---


#### 00:05:16.838

And you can then refine that and then   
(00:05:18.060) ~~we'll,~~ (00:05:18.259)  
we'll get back down into the lower levels of like specific problems and tools to solve that.   
(00:05:23.802) ~~I guess.~~(323.982)  
As I was preparing for this, I was having a good conversation with CLAWB3 about it. And I kind of came away with the understanding that there are two,   
(00:05:34.339) ~~I mean,~~(335.581)  
there's a lot of different layers, right? There's a lot of different levels of abstraction, which also kind of correspond to the scale of the thing that you're studying. And both at the level of an individual cell, and then again, at the level of the overall organism system, It seems that we have one really massive challenge, which is that we don't know how it works. 


---


#### 00:05:56.992

And in that way, there's an important commonality with the large language models that is like the most common topic on this podcast. But we sort of know that there's a lot of stuff going on and there's a lot of interactions that are happening. the nature of those interactions initially was entirely unclear. And now humanity at large has embarked on this grand project of trying to figure out how do cells work and how do our bodies work at a higher level. And it seems like we're   
(00:06:24.048) ~~maybe like,~~(384.689)  
not to be too specific with the number, but   
(00:06:27.170) ~~you know,~~(387.391)  
I'm gathering we're like maybe five to 10% of the way there, where most of the interactions remain unknown to us, but we've at least mapped out like a pretty decent chunk. 


---


#### 00:06:39.718

So the first challenge, if you're trying to solve a disease, as I understand it, is figure out what is it? What is the pathway? What is the interaction in this super complicated thing that is going wrong? And then the second challenge is, if I know what is going wrong, can I do something to intervene to stop it? But then again,   
(00:06:58.661) ~~I have a lot of,~~(419.582)  
right now we have a lot of dark matter, dark energy in terms of, I may be able to affect that one thing, but there could be a lot of other knock-on effects. Another sort of commonality is these things are not super clean. In language models, people are probably very familiar with the notion of superposition, which is like one neuron, one activation in a network, can light up for multiple different reasons. 


---


#### 00:07:20.834

And we certainly see all of these kind of patterns of complexity in biology as well. I'm kind of casting this into two levels. Tell me if you would refine this or change my thinking. But first is, man, there's this incredible network of interactions where things are disabling each other or promoting each other or interacting in all sorts of complicated ways. And we don't really know a lot about that, but we're gradually learning more all the time. And then if you do have a target, now it's okay. These are all three-dimensional spatial things. I'm not even sure if we should think of them as   
(00:07:54.463) ~~like~~ (00:07:54.622)  
classically 3D objects or if we should think of them more as sort of quantum distributions. 


---


#### 00:08:01.524

And maybe that varies depending on exactly what we're talking about. But we've got like the DNA, which is the code, the RNA, which is both like messenger, but also is like a machine. The proteins are all machines that fold up in weird ways and interact with each other in three dimensional space. And then you've got the small molecules as well, which are   
(00:08:23.177) ~~kind of~~(503.377)  
like signaling, but also if they fit right into all these puzzle pieces fit together in super strange ways. And so it's just extremely difficult.   
(00:08:32.639) ~~It is, yeah.~~(513.3)  
How am I doing there in terms of just setting a foundation to understand the challenges? So   
(00:08:38.442) ~~you've really,~~(518.963)  
I think you've really hit the nail on the head. 


---


#### 00:08:41.604

So protein interactions, especially, but also protein DNA, protein RNA, protein small molecule interactions are all very complicated things to model. And being able to predict when there's an interaction between two of these molecules and actually model that interaction correctly is a really hard problem. And I would say understanding protein interaction networks to start with,   
(00:09:05.955) ~~and we can talk about other kinds of interactions as well,~~(548.236)  
but understanding protein interaction networks is a very difficult and complex problem. And there are some new ways to address this that have come out recently that I have a lot of hope for, that I see them, and I think that these are very promising approaches and very effective approaches. So to just determine whether or not two proteins interact with each other, already, just two proteins interacting with each other, is a hard problem. 


---


#### 00:09:35.250

And then modeling how they fit together when they do interact, and understanding the strength and how transient that interaction might be, it's very difficult. And so we have tools to model these things now. They only have come out very recently, like within the last year or two. So for example, AlphaFold2 was a big deal, right? And that came out a couple of years ago. And   
(00:10:00.421) ~~you can model,~~(601.722)  
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
(00:15:02.870) ~~Okay, let me,~~(903.73)  
can we take one step back again? Sure. I think this is a paradigm shift, right? 


---


#### 00:15:08.572

The application of AI to biology, obviously the application of AI to just about everything is creating all sorts of paradigm shifts, but   
(00:15:14.534) ~~I think~~(914.696)  
it might also be helpful for people to understand a little bit better of the before state of   
(00:15:22.379) ~~like~~ (00:15:22.600)  
when we didn't have any of these tools yet, which is not that long ago. Not that long ago, yeah. What was the sort of prevailing approach to figuring stuff out and a little bit of just what is the biotech stack on which all this is built? I'm under the impression that The techniques available to us in many cases were like relatively primitive in the sense of you hear these stories of, oh look, we found this frog in the rainforest that like is immune to a certain disease. 


---


#### 00:15:52.562

Like what's going on there? Let's see if we can't find something in this frog that doesn't exist anywhere else. And then maybe that could be a medicine or whatever.   
(00:15:58.764) ~~It's like~~(958.965)  
really   
(00:15:59.404) ~~sort of~~(959.725)  
anecdotally sort of special observation motivated investigations in a lot of cases. And then I know there's also just a lot of   
(00:16:08.787) ~~like,~~ (00:16:08.986)  
historically brute forcing, basically, as I understand it, where it's, okay, look,   
(00:16:13.429) ~~let's,~~ (00:16:13.590)  
we have no idea which proteins are going to interact with which other ones. So let's just create this massive cross matrix and see if we can't figure it out that way. And look for hits, kind of massive essays of just exploring the space.   
(00:16:25.879) ~~I mean,~~(986.079)  
sure, it's a little bit smarter than that, but all of these things without the ability to really have any idea of what the puzzle pieces actually look like, which makes it obviously very difficult to figure out how they would fit together. 


---


#### 00:16:39.239

What more would you tell people who just want to understand, okay, what was the before, before all this stuff started to come online? So   
(00:16:46.304) ~~computationally, like~~(1007.546)  
on the computational aspect of, or the computational side of things, I think the prevailing methods that were the most advanced were molecular dynamic simulations. And people still use those.   
(00:16:57.614) ~~And And~~(1019.392)  
this is like physics. This is F equals ma, modeling, electro, electronic interactions, all this kind of, but just very like simple physics equations played out in many steps. Exactly. And so you have what's called a potential, right? and this potential tells you how the dynamics evolve. Like I was saying before, there are different levels of complexity of MD simulations, and there are some different flavors. 


---


#### 00:17:27.380

There's just standard molecular dynamics simulations, but you also have coarse-grained, and you also have different levels of complexity of how you're modeling the interactions and the forces between the particles. The most basic approach that you could take is just standard Newtonian mechanics.   
(00:17:42.051) ~~right?~~ (00:17:42.272)  
No quantum physics, no extra information about anything, just standard Newtonian physics. And then you can add stuff on top of that to get increasing complexity and accuracy. And so molecular dynamics simulations is definitely an in some cases still is the prevailing methodology on the computational side of things. And then also just using things like MSAs and some like machine learning models that arose in the last,   
(00:18:09.813) ~~I don't know,~~(1090.153)  
decade or so are POTS models. 


---


#### 00:18:12.433

So POTS models are also used, but those are like really specific sort of models. They're not very generalizable. And then on   
(00:18:20.599) ~~like the,~~(1101.32)  
there's also a lot of methods that come from wet lab work where people do this stuff in animals. Like they say you want to do directed evolution on a protein and try to find higher functioning variants or variants that are more thermostable that have higher expression or something like that. You can mutate these things in a lab and   
(00:18:45.467) ~~sort of~~(1125.787)  
you can do like point mutations or you can do two mutations at a time or you can do like multiple. But when you start adding in things higher than just single point mutations, you get this combinatorial complexity, right? 


---


#### 00:19:00.001

And so it gets really unwieldy. It feels like maybe not the most principled way to do it. I don't know. I don't want to trash people who are doing the lab work because the lab work is really important. But doing directed evolution in a lab, in a lot of ways, now that we have AI tools to do similar things, feels a little bit unnecessary. Why do we need to go and inject an animal and wait some amount of time for this to play out inside the animal and then actually synthesize these things by hand in a lab somewhere. When we can   
(00:19:34.068) ~~like~~ (00:19:34.249)  
do very similar things, computing and often get better results. So like a good example of how AI has   
(00:19:42.791) ~~sort of~~(1183.032)  
replaced this directed evolution methodology that comes out of like wet lab methods. 


---


#### 00:19:48.953

There are directed evolution AI models that you can use like protein language models to do directed evolution. You can also do a sequence redesign with things like protein MPNN or ligand MPNN, which allows you to redesign parts of the protein sequence or the entire protein sequence under some constraints, maybe under some certain specific chemical constraints, or you might want to bias the residues towards or away from certain amino acids and things like that. But these AI tools allow you to do that computationally and they do it really fast,   
(00:20:26.594) ~~right? I mean,~~(1227.235)  
like I can design a sequence for a protein in a few seconds with   
(00:20:31.395) ~~like~~ (00:20:31.537)  
ligand and PNN on my computer with no special hardware or anything. 


---


#### 00:20:36.118

I don't even need a fancy GPU to do it. And I can do that many times and get lots of variants for my protein. and assess them computationally. And very often these variants that you get out of this process are much higher performing than   
(00:20:53.459) ~~like~~ (00:20:53.618)  
the wild type or than what you would get by doing this in a wet lab. But yeah, so   
(00:20:59.540) ~~I guess~~(1259.781)  
hopefully that gives you some idea of some of the methods that they still are being used. It's not like these have just gone the way of the dodo and disappeared or something, but they have their place for sure. But   
(00:21:12.023) ~~I think~~(1272.404)  
computational approaches are proving to be much faster, much more effective, and you can scale them, which is really important because we're working sometimes with millions or hundreds of millions of proteins, having millions of variants of a protein and being able to assess them and determine their quality in some some metric has become a lot easier in the past couple of years even. 


---


#### 00:21:38.598

Like protein and PNN only came out a couple of years ago. It hasn't even really had time to really catch on in a lot of places. Like people are still learning about these tools and still adopting them. Yeah. Was there like any particular area of the history that you wanted to touch on? Because I feel like my experience with traditional methods is somewhat limited. I don't come from a wet lab background. I come from a very computational background. And because I started off working in the AI, I also haven't spent a lot of time working with MD simulations or other more traditional methods that people have used. historically. Nothing super specific. I'm really just trying to get a... 


---


#### 00:22:22.551

I'm early in my journey of understanding all of this. So I'm trying to get the high level paradigms first and then spiking down just   
(00:22:28.739) ~~kind of~~(1348.979)  
almost randomly into different areas to get a mix of the broad survey, but then try to go deep on a couple of technical things to understand some of the techniques in a more precise way.   
(00:22:39.840) ~~I think~~(1360.161)  
because the AI techniques are so new, most people working on them are still developing their own understanding of all of this. It's such a new paradigm. It's such a new methodology. There aren't very many people who are experts on this stuff.   
(00:22:56.205) ~~I think~~(1376.406)  
we're all   
(00:22:56.766) ~~kind of~~(1377.026)  
learning together, even me. I'm definitely still learning a lot of stuff from my coworkers and other researchers in the field. it's kind of mind blowing how fast this stuff is developing too. 


---


#### 00:23:09.854

It's developing incredibly fast, which is really good in my opinion. I want to see this stuff proliferated and developed and used because we're going to solve problems much faster this way.   
(00:23:19.800) ~~But yeah.~~(1400.201)  
Yeah. It seems like the speed, I want to   
(00:23:22.823) ~~kind of~~(1403.043)  
develop my intuition for the different learning loops and how they relate to each other as well. So again, let me just try a zoom out and then gradually   
(00:23:31.909) ~~kind of~~(1412.109)  
zoom in and you can refine anything that I'm saying. The, again, super high level, we have the black box problem of we don't know how cells work. We don't know how the biological systems work at large. There's a lot of interactions that are not well understood. 


---


#### 00:23:45.874

But we can, through traditionally very laborious wet lab work, gradually isolate what seems to be at the heart of various problems. And then when we have that hypothesis of, okay, maybe this is what's going on, that could be probably confirmed to varying degrees. Then we can say, hey, maybe we can disable that particular interaction as in the case of the cancer one that you mentioned toward the top. And again, in a traditional setting, we don't know what the shapes of the things are. So that really limits our ability to do any sort of Targeted approach,   
(00:24:22.684) ~~right?~~ (00:24:22.865)  
Like, rational drug design has been   
(00:24:24.606) ~~sort of~~(1464.867)  
the dream as I understand it for decades and is only now   
(00:24:28.351) ~~kind of~~(1468.551)  
starting to happen now that we're developing all these tools to understand the shape. 


---


#### 00:24:33.036

So. I guess, in terms of, like, just a little intuition for the shapes to and the sort of confirmations. I sort of envision, and again, analogy free zone, but this is fairly literal with obvious room for mistakes. So again, correct my mistakes, but I sort of envision   
(00:24:52.067) ~~like~~ (00:24:52.287)  
a slinky where if I just sit the slinky down on the floor, it will   
(00:24:58.051) ~~sort of~~(1498.493)  
come into a pretty tight coil. And that you might say is like its lowest energy state, then I can stretch it out. And if I,   
(00:25:09.462) ~~you know,~~(1509.683)  
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
(00:26:12.193) ~~I guess~~(1572.374)  
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
(00:27:32.089) ~~So like, how would,~~(1653.591)  
it seems in some sense surprising that you would be able to make a new black box system to make these predictions that they would be faster and more accurate as opposed to just running the physics. How is that leap happening? Okay, so   
(00:27:49.114) ~~I guess~~(1669.394)  
the simple answer is basically compression, right? You've got some information and you have some really efficient way of compressing that information. And a lot of these AI models are,   
(00:28:01.804) ~~I mean,~~(1682.725)  
you can think of them as functions, but you can also think of them as   
(00:28:06.749) ~~like~~ (00:28:06.909)  
compressors of information. 


---


#### 00:28:09.050

And so some of them,   
(00:28:11.133) ~~I guess,~~(1692.153)  
traditionally you think of AI models like a deep learning neural network sort of thing, you've got data, you train on your data, maybe you have like a trained test validation split or something like that, and you train on your training data and you see how it performs on your test data and that's your trained model. But you can also train models with   
(00:28:31.578) ~~like~~ (00:28:31.719)  
physics constraints, right? And there are some models that are actually data-free. You can train some neural networks using physics constraints in a data-free way. people are doing this for this problem in particular, for getting the Boltzmann distribution of a protein and getting all these ensembles of conformations and their transitions between the states. 


---


#### 00:28:52.010

There are some approaches that people are using that are completely data-free and are based on physics. And the model is learning the physics and compressing that physics and then generalizing to systems that it hasn't seen before. And   
(00:29:04.461) ~~I think~~(1744.761)  
because there's compression happening and you're not, so like in molecular dynamics,   
(00:29:11.476) ~~I mean,~~(1751.596)  
you could simplify things by simplifying the forces or simplifying the model in terms of   
(00:29:16.378) ~~like how complicated of~~(1757.58)  
how complicated the physics are that you're using to model problems. If I strip everything down and just do like bare bones, Newtonian physics, I can simplify things that way, but I don't see this notion of like compression happening.   
(00:29:31.208) ~~Right.~~ (00:29:31.468)  
Whereas for a neural network, you're compressing information. 


---


#### 00:29:35.109

You're taking something complicated and noisy sometimes, and you're compressing it down into some simpler maybe not simpler, but you're compressing it and you're providing a representation of it that is more compact. And because you've done this, and if you've done it, it generalizes to systems that it hasn't been trained on before. You get something that is faster, significantly faster, like orders of magnitude faster, right? You get something that produces your answer in   
(00:30:04.758) ~~like~~ (00:30:04.897)  
a minute instead of four hours or days.   
(00:30:07.744) ~~I think in my mind, the way that I understand it,~~(1810.267)  
I think the key here is compression. Neural networks are compressors of information. Whereas molecular dynamics simulation, there's no real compression happening. Does that make sense? 


---


#### 00:30:20.846

Yeah. I think I'm just trying to kind of, should be okay. This software, yeah, all good. We will edit and also the software is uploading the original version opportunistically in the background. So even if we have a little lag or whatever, it should have the original high quality. Okay. So   
(00:30:39.089) ~~that was pretty much my hypothesis was that it's essentially learning higher order concepts beyond the raw physics.~~(1849.398)  
  
(00:30:49.857) ~~And that is very analogous.~~(1851.059)  
And we've covered this in a lot of different ways over the last hundred episodes with mostly focus on language models. But it's really this striking observation that comes up   
(00:31:01.946) ~~over and~~(1862.188)  
over again that, okay, yeah, language models, they're only trained to predict the next token, but they not only seem to be generalizing certainly beyond the narrow, narrowly defined bounds of their training data, and perhaps to some degree even   
(00:31:20.491) ~~kind of~~(1880.692)  
more than that, it's like a hotly debated topic, but what is pretty clearly demonstrated at this point is that in the   
(00:31:27.616) ~~like~~ (00:31:27.798)  
middle to late layers of a language model transformer, you can now, the techniques are there to say, okay,   
(00:31:36.828) ~~this,~~ (00:31:37.150)  
this pattern of activations seems to correspond to this higher order concept that we care about. which is   
(00:31:44.441) ~~kind of~~(1904.922)  
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
(00:33:34.015) ~~sort of~~(2014.316)  
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
(00:35:04.213) ~~in this~~(2104.614)  
in some way. but we're not giving it forces and potentials and things like that. And yet somehow we're able to predict the structure of the protein with really high accuracy for a lot of proteins, for most proteins. I guess that's another example of where AI can be a lot better than the molecular dynamics. Because if you want to model a protein actually folding in a molecular dynamics simulation to get the folded structure of the protein, this is pretty hard and time-consuming and computationally intensive. Whereas for AlphaFold2 or ESMFold, it takes a few minutes. You give it a big protein and it takes a few minutes. 


---


#### 00:35:43.822

And I guess this is, in these cases, these are like language model-like models, right? They definitely have the architecture that looks a lot like language models, especially ESMFold. I think AlphaFold a little less because it has some of these extra architectural things that are a little more nuanced, like the MSA and the templates and such. But both of these models are very much inspired by language models. And ESMfold is pretty much just a language model. And you're able to predict these 3D structures with these things without really explicitly modeling any physics. And that provides a substantial speed up. And   
(00:36:20.237) ~~I guess~~(2180.517)  
in terms of like how this relates to language modeling, so the concept that I think you're trying to grasp onto is protein motifs. or domains. 


---


#### 00:36:32.333

So motifs are like reoccurring patterns that happen in proteins. They're like short little sequences of amino acids that recur often in lots of different proteins and generally have a very similar structure across different proteins, for example. This is   
(00:36:48.623) ~~kind 
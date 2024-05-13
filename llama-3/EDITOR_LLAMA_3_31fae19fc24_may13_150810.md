#### 0.129

Amelie Schreiber, computational biochemist and AI researcher. Welcome to the Cognitive Revolution. Nice to be here. I'm excited for this conversation. I expect to learn a lot from it. Quick context on my end. This all started with a tweet that I saw you put out probably two months ago now. where you said, here are my    
(19.81) ~~top 10 tools,~~ (20.77)  
top 10 AI tools for biology in no particular order. And I read down the list and I was like, I don't know what any of these are. So when that happens, I'm immediately like, okay, this is an area that I need to do some remedial self-education in. And reached out,   
(37.215) ~~I think~~(37.415)  
pretty much immediately to say, hey, would you be interested in educating me in the form of a podcast? 


---


#### 41.797

So I appreciate you taking the time to prepare for this and do it. You want to start off by just giving a little bit of context on who you are, what you're doing day to day and what kinds of problems maybe you're trying to solve. And then we can step back again and give people   
(54.933) ~~kind of~~(55.133)  
foundational knowledge. Yeah,   
(57.069) ~~sure. Yeah,~~(57.67)  
I'm an AI researcher and I focus on computational biochemistry applications. I actually started out as a mathematician. My training in grad school and stuff was in mathematics, actually. Started off with pure mathematics and then transitioned into applied mathematics and data analysis type stuff. And then after grad school, I got into the deep learning stuff and started working on more AI related things. 


---


#### 80.305

Yeah, I think, and for me, like the biochemistry applications are one of the most compelling things that we could be working on right now. I think other than   
(89.093) ~~like~~ (89.233)  
AGI, whatever that means, I think it's probably the most important problem we can be working on because it's a huge impact on human health. The applications in human health and medical applications are really profound and have the potential to be very impactful and for everyone too. So I get really excited about the biochemistry applications of AI. And yeah,   
(112.857) ~~I guess~~(113.117)  
that's a little about me. Was there anything in particular that you wanted to know about my background or experience? Maybe just the context that you're working in today a little bit would be helpful to understand how it is that you're exploring these tools and applying them. 


---


#### 124.804

Obviously, again, we're going to have to get into more detail on what they are, but yeah, just   
(129.367) ~~kind of~~(129.587)  
where in the world are you situated that you're doing all this stuff?   
(133.309) ~~So, I mean,~~(133.75)  
I work on mostly applications in biochemistry related to human health. I have some projects and things that I'm working on that are more related to   
(143.963) ~~like~~ (144.103)  
environmental things and material science type applications, but Primarily I focus on the medical or biomedical aspect of things. That's what I'm most interested in. I work with a lot of different kinds of molecules. So small molecules, which are like your drugs that you take in like a pill form or something, right? These are smaller than proteins and less complicated. 


---


#### 167.406

And I also work with proteins and also a little bit with DNA and RNA. And I use various kinds of AI tools, analyze these molecules, create new ones, modify them, engineer them in ways, grafting them together and stuff, performing complicated operations on these molecules to get particular kinds of functions out of them so that they perform a particular kind of function. And as an example, designing a new protein to bind to another protein so that you can cause some kind of cascade event in a protein network, in a protein interaction network, or so that you can block certain interactions between proteins. A really good example in cancer, there's two proteins that come up that are like your basic first examples of like a mechanism of cancer. 


---


#### 217.838

So there's PD-1 and PD-L1, and these are two proteins. One of them's located in the cancer, and one of them's located on your immune cells. And what happens is these two proteins end up binding to each other, and essentially the cancer turns off your immune cell so that your immune cell doesn't attack the cancer. And this is an interaction that's not good, right? You don't want this kind of interaction between these two proteins because you want your immune system to recognize the cancer and destroy it. And having this interaction turns off your immune system in a very specific kind of way. So you can do things like design binders to this protein, to one of these two proteins to block that interaction. 


---


#### 260.853

And that can help you like combat cancer and hopefully treat it. And that's just one basic example of something that you can do with these tools that I'm using and that I'm interested in. You can also design new drugs with them. You can design drugs that are specific to a particular binding pocket on a protein. You can design drugs that have very specific chemical properties. You can design proteins that have very specific chemical and functional properties. And you can also modify DNA and RNA now. This is pretty new stuff, the DNA and the RNA. You can also do a lot of the same things with DNA and RNA molecules as well. Okay. So let me take a super zoom out for one second and try to give a extremely high level understanding as I have it today for   
(307.736) ~~kind of~~(308.016)  
a couple of the biggest sorts of problems that I understand are being studied in biomedical sciences. 


---


#### 316.839

And you can then refine that and then   
(318.06) ~~we'll,~~ (318.26)  
we'll get back down into the lower levels of like specific problems and tools to solve that.   
(323.802) ~~I guess.~~(323.982)  
As I was preparing for this, I was having a good conversation with CLAWB3 about it. And I kind of came away with the understanding that there are two,   
(334.34) ~~I mean,~~(335.581)  
there's a lot of different layers, right? There's a lot of different levels of abstraction, which also kind of correspond to the scale of the thing that you're studying. And both at the level of an individual cell, and then again, at the level of the overall organism system, It seems that we have one really massive challenge, which is that we don't know how it works. 


---


#### 356.993

And in that way, there's an important commonality with the large language models that is like the most common topic on this podcast. But we sort of know that there's a lot of stuff going on and there's a lot of interactions that are happening. the nature of those interactions initially was entirely unclear. And now humanity at large has embarked on this grand project of trying to figure out how do cells work and how do our bodies work at a higher level. And it seems like we're   
(384.049) ~~maybe like,~~(384.689)  
not to be too specific with the number, but   
(387.171) ~~you know,~~(387.391)  
I'm gathering we're like maybe five to 10% of the way there, where most of the interactions remain unknown to us, but we've at least mapped out like a pretty decent chunk. 


---


#### 399.719

So the first challenge, if you're trying to solve a disease, as I understand it, is figure out what is it? What is the pathway? What is the interaction in this super complicated thing that is going wrong? And then the second challenge is, if I know what is going wrong, can I do something to intervene to stop it? But then again,   
(418.662) ~~I have a lot of,~~(419.582)  
right now we have a lot of dark matter, dark energy in terms of, I may be able to affect that one thing, but there could be a lot of other knock-on effects. Another sort of commonality is these things are not super clean. In language models, people are probably very familiar with the notion of superposition, which is like one neuron, one activation in a network, can light up for multiple different reasons. 


---


#### 440.834

And we certainly see all of these kind of patterns of complexity in biology as well. I'm kind of casting this into two levels. Tell me if you would refine this or change my thinking. But first is, man, there's this incredible network of interactions where things are disabling each other or promoting each other or interacting in all sorts of complicated ways. And we don't really know a lot about that, but we're gradually learning more all the time. And then if you do have a target, now it's okay. These are all three-dimensional spatial things. I'm not even sure if we should think of them as   
(474.463) ~~like~~ (474.623)  
classically 3D objects or if we should think of them more as sort of quantum distributions. 


---


#### 481.525

And maybe that varies depending on exactly what we're talking about. But we've got like the DNA, which is the code, the RNA, which is both like messenger, but also is like a machine. The proteins are all machines that fold up in weird ways and interact with each other in three dimensional space. And then you've got the small molecules as well, which are   
(503.177) ~~kind of~~(503.377)  
like signaling, but also if they fit right into all these puzzle pieces fit together in super strange ways. And so it's just extremely difficult.   
(512.64) ~~It is, yeah.~~(513.3)  
How am I doing there in terms of just setting a foundation to understand the challenges? So   
(518.443) ~~you've really,~~(518.963)  
I think you've really hit the nail on the head. 


---


#### 521.604

So protein interactions, especially, but also protein DNA, protein RNA, protein small molecule interactions are all very complicated things to model. And being able to predict when there's an interaction between two of these molecules and actually model that interaction correctly is a really hard problem. And I would say understanding protein interaction networks to start with,   
(545.955) ~~and we can talk about other kinds of interactions as well,~~(548.236)  
but understanding protein interaction networks is a very difficult and complex problem. And there are some new ways to address this that have come out recently that I have a lot of hope for, that I see them, and I think that these are very promising approaches and very effective approaches. So to just determine whether or not two proteins interact with each other, already, just two proteins interacting with each other, is a hard problem. 


---


#### 575.25

And then modeling how they fit together when they do interact, and understanding the strength and how transient that interaction might be, it's very difficult. And so we have tools to model these things now. They only have come out very recently, like within the last year or two. So for example, AlphaFold2 was a big deal, right? And that came out a couple of years ago. And   
(600.421) ~~you can model,~~(601.722)  
I think the way to think about it is you can model a very low energy confirmation of the protein. It's not necessarily like the ground state or the lowest energy confirmation, but ideally it's one of the lowest energy confirmations, if not the lowest. But you just get a single static structure from AlphaFold2. 


---


#### 621.416

So we give it the protein sequence, which is just a sequence of amino acids, which are represented by 20 letters. and it takes in this protein sequence, it computes something called a multiple sequence alignment or an MSA, and it provides you with a static structure for that protein that's a low energy confirmation for that protein. But that protein could exist in other confirmations. It might have other states that it exists in when it's interacting with other proteins or based on the environment that it's in, what temperature it is, things like this. can change the shape of the protein,   
(658.666) ~~right?~~ (658.806)  
They move around, they're very jiggly, and they do things. And so people have been trying to address this and model what's called the Boltzmann distribution of proteins. 


---


#### 671.274

And the Boltzmann distribution is something from statistical mechanics that tells you all the different conformations and what probabilities there are associated to those different conformations. And having a way to sample the Boltzmann distribution and get all of these different confirmations out of them. And also understanding the transitions between these states is a really difficult problem. And there's actually a model that we'll talk about later that does a really good job of addressing this that just came out middle of last year. It's called distributional graph former. And we'll talk about that a little bit later. And that's one of the generalizations of, it's not really a generalization of AlphaFold2's architecture, but it's a generalization of the idea that AlphaFold2 is implementing, right? 


---


#### 717.47

It's not just a single static structure anymore. It's actually a whole ensemble of structures and also the transition pathways between those different metastable states. And being able to model this and understand more   
(732.395) ~~like~~ (732.575)  
the dynamics of the proteins is something that people have been thinking about pretty hard for the last couple of years. And we're just starting to get tools that actually address this problem. And that's a really good thing because traditionally the way that this sort of thing was approached was through something called molecular dynamic simulations. And molecular dynamic simulations, they come in a lot of different flavors and they come in a lot of different complexities. Some of them model the proteins using just standard Newtonian physics, and then you can add in more complexity on top of that and add in things like quantum properties and other features of the protein to make the molecular dynamics simulation more complex and more robust. 


---


#### 774.477

But these simulations, they are really computationally intensive. They take a long time, they take a lot of GPUs, and they're just not very efficient. And on top of that, The length of time that you run your simulation for really, in a lot of cases, determines how accurate your distribution is and how accurate the confirmations or trajectories that you get out of that are. And you might run your simulation and not run it for long enough, and you don't get all the different states that the protein might be in, but you miss some of them, right? There are some new AI models that are trying to address this and trying to make headway into augmenting or even replacing molecular dynamic simulations in a lot of cases. 


---


#### 824.079

And this is really good because we need things that are more computationally efficient so that we can do this for a lot of proteins, right? Because we have a lot of proteins to do this for. And distributional graph former. is addressing a lot of this. And it does a pretty good job of doing it too. There's some room for improvement for sure, but it's a pretty solid model. And some really respectable people that I have a lot of respect for in this area have worked on this. And some of the inspiration comes from diffusion models. So it's a diffusion model similar to   
(860.491) ~~like~~ (860.631)  
DALI, which most of your watchers are probably familiar with, but it works on proteins instead of images. 


---


#### 867.144

And it also takes some inspiration from an area that is trying to solve this problem in a slightly different way called Boltzmann generators. And we can discuss that a little bit. I don't want to spend too much time on the Boltzmann generators, but it's influenced by some of those ideas and trying to sample the Boltzmann distribution of the proteins or protein complexes even or protein small molecule complexes and getting a handle on something that's more like the dynamics of the protein and getting a good representation of all the different metastable states that the protein might exist in at low energies.   
(902.87) ~~Okay, let me,~~(903.73)  
can we take one step back again? Sure. I think this is a paradigm shift, right? 


---


#### 908.573

The application of AI to biology, obviously the application of AI to just about everything is creating all sorts of paradigm shifts, but   
(914.535) ~~I think~~(914.696)  
it might also be helpful for people to understand a little bit better of the before state of   
(922.38) ~~like~~ (922.6)  
when we didn't have any of these tools yet, which is not that long ago. Not that long ago, yeah. What was the sort of prevailing approach to figuring stuff out and a little bit of just what is the biotech stack on which all this is built? I'm under the impression that The techniques available to us in many cases were like relatively primitive in the sense of you hear these stories of, oh look, we found this frog in the rainforest that like is immune to a certain disease. 


---


#### 952.563

Like what's going on there? Let's see if we can't find something in this frog that doesn't exist anywhere else. And then maybe that could be a medicine or whatever.   
(958.765) ~~It's like~~(958.965)  
really   
(959.405) ~~sort of~~(959.725)  
anecdotally sort of special observation motivated investigations in a lot of cases. And then I know there's also just a lot of   
(968.787) ~~like,~~ (968.987)  
historically brute forcing, basically, as I understand it, where it's, okay, look,   
(973.43) ~~let's,~~ (973.59)  
we have no idea which proteins are going to interact with which other ones. So let's just create this massive cross matrix and see if we can't figure it out that way. And look for hits, kind of massive essays of just exploring the space.   
(985.879) ~~I mean,~~(986.079)  
sure, it's a little bit smarter than that, but all of these things without the ability to really have any idea of what the puzzle pieces actually look like, which makes it obviously very difficult to figure out how they would fit together. 


---


#### 999.239

What more would you tell people who just want to understand, okay, what was the before, before all this stuff started to come online? So   
(1006.305) ~~computationally, like~~(1007.546)  
on the computational aspect of, or the computational side of things, I think the prevailing methods that were the most advanced were molecular dynamic simulations. And people still use those.   
(1017.614) ~~And And~~(1019.392)  
this is like physics. This is F equals ma, modeling, electro, electronic interactions, all this kind of, but just very like simple physics equations played out in many steps. Exactly. And so you have what's called a potential, right? and this potential tells you how the dynamics evolve. Like I was saying before, there are different levels of complexity of MD simulations, and there are some different flavors. 


---


#### 1047.38

There's just standard molecular dynamics simulations, but you also have coarse-grained, and you also have different levels of complexity of how you're modeling the interactions and the forces between the particles. The most basic approach that you could take is just standard Newtonian mechanics.   
(1062.052) ~~right?~~ (1062.273)  
No quantum physics, no extra information about anything, just standard Newtonian physics. And then you can add stuff on top of that to get increasing complexity and accuracy. And so molecular dynamics simulations is definitely an in some cases still is the prevailing methodology on the computational side of things. And then also just using things like MSAs and some like machine learning models that arose in the last,   
(1089.813) ~~I don't know,~~(1090.153)  
decade or so are POTS models. 


---


#### 1092.434

So POTS models are also used, but those are like really specific sort of models. They're not very generalizable. And then on   
(1100.6) ~~like the,~~(1101.32)  
there's also a lot of methods that come from wet lab work where people do this stuff in animals. Like they say you want to do directed evolution on a protein and try to find higher functioning variants or variants that are more thermostable that have higher expression or something like that. You can mutate these things in a lab and   
(1125.467) ~~sort of~~(1125.787)  
you can do like point mutations or you can do two mutations at a time or you can do like multiple. But when you start adding in things higher than just single point mutations, you get this combinatorial complexity, right? 


---


#### 1140.002

And so it gets really unwieldy. It feels like maybe not the most principled way to do it. I don't know. I don't want to trash people who are doing the lab work because the lab work is really important. But doing directed evolution in a lab, in a lot of ways, now that we have AI tools to do similar things, feels a little bit unnecessary. Why do we need to go and inject an animal and wait some amount of time for this to play out inside the animal and then actually synthesize these things by hand in a lab somewhere. When we can   
(1174.069) ~~like~~ (1174.249)  
do very similar things, computing and often get better results. So like a good example of how AI has   
(1182.792) ~~sort of~~(1183.032)  
replaced this directed evolution methodology that comes out of like wet lab methods. 


---


#### 1188.954

There are directed evolution AI models that you can use like protein language models to do directed evolution. You can also do a sequence redesign with things like protein MPNN or ligand MPNN, which allows you to redesign parts of the protein sequence or the entire protein sequence under some constraints, maybe under some certain specific chemical constraints, or you might want to bias the residues towards or away from certain amino acids and things like that. But these AI tools allow you to do that computationally and they do it really fast,   
(1226.594) ~~right? I mean,~~(1227.235)  
like I can design a sequence for a protein in a few seconds with   
(1231.396) ~~like~~ (1231.537)  
ligand and PNN on my computer with no special hardware or anything. 


---


#### 1236.119

I don't even need a fancy GPU to do it. And I can do that many times and get lots of variants for my protein. and assess them computationally. And very often these variants that you get out of this process are much higher performing than   
(1253.459) ~~like~~ (1253.619)  
the wild type or than what you would get by doing this in a wet lab. But yeah, so   
(1259.541) ~~I guess~~(1259.781)  
hopefully that gives you some idea of some of the methods that they still are being used. It's not like these have just gone the way of the dodo and disappeared or something, but they have their place for sure. But   
(1272.024) ~~I think~~(1272.404)  
computational approaches are proving to be much faster, much more effective, and you can scale them, which is really important because we're working sometimes with millions or hundreds of millions of proteins, having millions of variants of a protein and being able to assess them and determine their quality in some some metric has become a lot easier in the past couple of years even. 


---


#### 1298.599

Like protein and PNN only came out a couple of years ago. It hasn't even really had time to really catch on in a lot of places. Like people are still learning about these tools and still adopting them. Yeah. Was there like any particular area of the history that you wanted to touch on? Because I feel like my experience with traditional methods is somewhat limited. I don't come from a wet lab background. I come from a very computational background. And because I started off working in the AI, I also haven't spent a lot of time working with MD simulations or other more traditional methods that people have used. historically. Nothing super specific. I'm really just trying to get a... 


---


#### 1342.552

I'm early in my journey of understanding all of this. So I'm trying to get the high level paradigms first and then spiking down just   
(1348.739) ~~kind of~~(1348.979)  
almost randomly into different areas to get a mix of the broad survey, but then try to go deep on a couple of technical things to understand some of the techniques in a more precise way.   
(1359.841) ~~I think~~(1360.161)  
because the AI techniques are so new, most people working on them are still developing their own understanding of all of this. It's such a new paradigm. It's such a new methodology. There aren't very many people who are experts on this stuff.   
(1376.206) ~~I think~~(1376.406)  
we're all   
(1376.766) ~~kind of~~(1377.026)  
learning together, even me. I'm definitely still learning a lot of stuff from my coworkers and other researchers in the field. it's kind of mind blowing how fast this stuff is developing too. 


---


#### 1389.854

It's developing incredibly fast, which is really good in my opinion. I want to see this stuff proliferated and developed and used because we're going to solve problems much faster this way.   
(1399.801) ~~But yeah.~~(1400.201)  
Yeah. It seems like the speed, I want to   
(1402.823) ~~kind of~~(1403.043)  
develop my intuition for the different learning loops and how they relate to each other as well. So again, let me just try a zoom out and then gradually   
(1411.909) ~~kind of~~(1412.109)  
zoom in and you can refine anything that I'm saying. The, again, super high level, we have the black box problem of we don't know how cells work. We don't know how the biological systems work at large. There's a lot of interactions that are not well understood. 


---


#### 1425.874

But we can, through traditionally very laborious wet lab work, gradually isolate what seems to be at the heart of various problems. And then when we have that hypothesis of, okay, maybe this is what's going on, that could be probably confirmed to varying degrees. Then we can say, hey, maybe we can disable that particular interaction as in the case of the cancer one that you mentioned toward the top. And again, in a traditional setting, we don't know what the shapes of the things are. So that really limits our ability to do any sort of Targeted approach,   
(1462.685) ~~right?~~ (1462.865)  
Like, rational drug design has been   
(1464.607) ~~sort of~~(1464.867)  
the dream as I understand it for decades and is only now   
(1468.351) ~~kind of~~(1468.551)  
starting to happen now that we're developing all these tools to understand the shape. 


---


#### 1473.036

So. I guess, in terms of, like, just a little intuition for the shapes to and the sort of confirmations. I sort of envision, and again, analogy free zone, but this is fairly literal with obvious room for mistakes. So again, correct my mistakes, but I sort of envision   
(1492.067) ~~like~~ (1492.287)  
a slinky where if I just sit the slinky down on the floor, it will   
(1498.052) ~~sort of~~(1498.493)  
come into a pretty tight coil. And that you might say is like its lowest energy state, then I can stretch it out. And if I,   
(1509.463) ~~you know,~~(1509.683)  
do the work and put the energy into it, then I can stretch it out. Now, if I let it go, it's going to snap back to its low energy state. 


---


#### 1518.65

I could also come along and step on the middle of it. And then I would have the part of it would be like under my foot and bent down, but then the parts on the side would presumably still kind of look like they're normal, but there'd be this   
(1528.999) ~~like~~ (1529.159)  
deformed part in the middle where I'm stepping on it. Yeah. This is sort of analogous to what is going, violating my no analogy rule, but this is a pretty tight analogy. It's like a physical deformation, right? Where this thing can have a low energy state, but then maybe in the presence of some other protein that   
(1545.174) ~~like~~ (1545.395)  
constrains it in a certain way, or some other small molecule, perhaps it fits into a pocket of it in a certain way, or brings two parts that aren't normally together, more closely together, whatever, then you can have these sort of deformations. 


---


#### 1558.085

And then subject to those constraints, they still kind of find their natural low energy state. And so you have   
(1564.47) ~~like~~ (1564.59)  
multiple of these, there could be, and of course this is all happening in an environment where the surrounding,   
(1572.194) ~~I guess~~(1572.374)  
it probably depends a lot on   
(1573.435) ~~like~~ (1573.555)  
just how big or small of a thing we're talking about, but the slinky relative to the air is like massive, right? The air molecules are super small relative to the slinky, so we don't really have to think too much about the air molecules, but in the context of these super small things, individual proteins, they're in solution, right? So there's at a minimum, there's like water molecules bouncing off them all the time. 


---


#### 1596.717

So they have this sort of noisy environment. I'm thinking there of like brownie in motion, which I'm not by any means an expert in, but the constant sort of bumping into the environment creates opportunity for these things to kind of occasionally flop from shape to shape. And so doing all of this in traditional sense is probably hard for a lot of reasons, but you highlighted the fact that the computation is really slow, right? You just have a ton of interactions, the many terms and sort of how things interact. Now,   
(1630.835) ~~like~~ (1630.975)  
how is it happening that the, I have a hypothesis on this, but I'll just ask the question. How is it happening that the AI models are doing this so much faster and more accurate than traditional physics? 


---


#### 1645.706

Because a naive thought would be like, there's nothing, there's only physics, right? We hear that sort of refrain a lot.   
(1652.09) ~~So like, how would,~~(1653.591)  
it seems in some sense surprising that you would be able to make a new black box system to make these predictions that they would be faster and more accurate as opposed to just running the physics. How is that leap happening? Okay, so   
(1669.114) ~~I guess~~(1669.394)  
the simple answer is basically compression, right? You've got some information and you have some really efficient way of compressing that information. And a lot of these AI models are,   
(1681.804) ~~I mean,~~(1682.725)  
you can think of them as functions, but you can also think of them as   
(1686.749) ~~like~~ (1686.909)  
compressors of information. 


---


#### 1689.051

And so some of them,   
(1691.133) ~~I guess,~~(1692.153)  
traditionally you think of AI models like a deep learning neural network sort of thing, you've got data, you train on your data, maybe you have like a trained test validation split or something like that, and you train on your training data and you see how it performs on your test data and that's your trained model. But you can also train models with   
(1711.579) ~~like~~ (1711.719)  
physics constraints, right? And there are some models that are actually data-free. You can train some neural networks using physics constraints in a data-free way. people are doing this for this problem in particular, for getting the Boltzmann distribution of a protein and getting all these ensembles of conformations and their transitions between the states. 


---


#### 1732.011

There are some approaches that people are using that are completely data-free and are based on physics. And the model is learning the physics and compressing that physics and then generalizing to systems that it hasn't seen before. And   
(1744.461) ~~I think~~(1744.761)  
because there's compression happening and you're not, so like in molecular dynamics,   
(1751.476) ~~I mean,~~(1751.596)  
you could simplify things by simplifying the forces or simplifying the model in terms of   
(1756.379) ~~like how complicated of~~(1757.58)  
how complicated the physics are that you're using to model problems. If I strip everything down and just do like bare bones, Newtonian physics, I can simplify things that way, but I don't see this notion of like compression happening.   
(1771.208) ~~Right.~~ (1771.468)  
Whereas for a neural network, you're compressing information. 


---


#### 1775.11

You're taking something complicated and noisy sometimes, and you're compressing it down into some simpler maybe not simpler, but you're compressing it and you're providing a representation of it that is more compact. And because you've done this, and if you've done it, it generalizes to systems that it hasn't been trained on before. You get something that is faster, significantly faster, like orders of magnitude faster, right? You get something that produces your answer in   
(1804.758) ~~like~~ (1804.898)  
a minute instead of four hours or days.   
(1807.745) ~~I think in my mind, the way that I understand it,~~(1810.267)  
I think the key here is compression. Neural networks are compressors of information. Whereas molecular dynamics simulation, there's no real compression happening. Does that make sense? 


---


#### 1820.847

Yeah. I think I'm just trying to kind of, should be okay. This software, yeah, all good. We will edit and also the software is uploading the original version opportunistically in the background. So even if we have a little lag or whatever, it should have the original high quality. Okay. So   
(1839.09) ~~that was pretty much my hypothesis was that it's essentially learning higher order concepts beyond the raw physics.~~(1849.398)  
  
(1849.858) ~~And that is very analogous.~~(1851.059)  
And we've covered this in a lot of different ways over the last hundred episodes with mostly focus on language models. But it's really this striking observation that comes up   
(1861.947) ~~over and~~(1862.188)  
over again that, okay, yeah, language models, they're only trained to predict the next token, but they not only seem to be generalizing certainly beyond the narrow, narrowly defined bounds of their training data, and perhaps to some degree even   
(1880.492) ~~kind of~~(1880.692)  
more than that, it's like a hotly debated topic, but what is pretty clearly demonstrated at this point is that in the   
(1887.617) ~~like~~ (1887.798)  
middle to late layers of a language model transformer, you can now, the techniques are there to say, okay,   
(1896.829) ~~this,~~ (1897.15)  
this pattern of activations seems to correspond to this higher order concept that we care about. which is   
(1904.441) ~~kind of~~(1904.922)  
a miraculous thing that like it's just predicting the next token, but it's like learning these concepts of justice and fairness and ethics and whatever that are like obviously useful to predict the next token. 


---


#### 1918.49

And that's presumably why they're arising, but not something that's been like specifically coded for. So I guess in the application to biology, basically the same phenomenon is happening where raw data or raw simulated physics or whatever is sort of the input. And the higher order concepts are what? I'm guessing that they're sort of, I don't know a lot about this, but like the residue is sort of a part, it's like almost like the vocabulary of proteins. And we have the next token, the sort of The token level vocabulary of a protein would be the 20 amino acids, but the sort of higher order concepts are what? It's like, oh, this chunk of a thing is like reused a lot. 


---


#### 1962.965

And these two chunks of things like interact with each other in a particular way. Give us a little more intuition of that. What are the higher order concepts that these things seem to be learning? Yeah. So if we put aside   
(1973.67) ~~like~~ (1973.83)  
dynamics for a moment and we just look at   
(1975.631) ~~like~~ (1975.771)  
structure prediction. So structure prediction, like AlphaFold2, for example, there's another model that does essentially the same thing. It predicts the 3D structure of the protein in some low energy state, right? ESMFold, right? This is like an alternative model to AlphaFold2. It doesn't perform as well as AlphaFold2, but it does pretty well. And it's a language model. It's something that people call a protein language model. 


---


#### 2001.705

And it's It's built on the BERT architecture actually, which sounds kind of bad, right? Cause BERT's like this older model that's only used for like specific things now. And like the chat GPT   
(2014.015) ~~sort of~~(2014.316)  
models have overshadowed or outshined the BERT models at this point. But   
(2019.678) ~~in,~~ (2019.778)  
in biology, this actually makes a lot more sense because you have the mask language modeling objective. that you train on for protein sequences, and you just mask out some of the amino acids in the protein sequence and have it predict what those are,   
(2033.325) ~~right?~~ (2033.766)  
And just by training it to do this, and then putting like a folding model on top of it called EvoFormer, which actually comes from the AlphaFold2 architecture, you don't train on any physics, but somehow you learn how to predict 3D structures of proteins,   
(2049.375) ~~right?~~ (2049.575)  



---


#### 2049.635

And so in this case, it's almost like physics mostly isn't needed. right? If you just want to predict a static structure of a protein, you can get pretty good results just using a BERT type architecture with mask language modeling objective, training on   
(2066.551) ~~like~~ (2066.711)  
millions of proteins. And if you just train on a bunch of proteins doing this, you get something that will fold proteins for you pretty darn well. And again,   
(2075.076) ~~like~~ (2075.216)  
there's some   
(2075.716) ~~like~~ (2075.856)  
really nuanced architectural differences between ESM Fold and Alpha Fold 2. 2 uses what's called multiple sequence alignments, and it also uses these templates, right? And in general, it is better performing because it has these extra,   
(2090.804) ~~like,~~ (2090.985)  
added things in the architecture that improve its ability to predict the structure. 


---


#### 2095.648

But even there, there isn't really a lot of physics explicitly happening. Now, maybe there's some physics encoded   
(2104.214) ~~in this~~(2104.614)  
in some way. but we're not giving it forces and potentials and things like that. And yet somehow we're able to predict the structure of the protein with really high accuracy for a lot of proteins, for most proteins. I guess that's another example of where AI can be a lot better than the molecular dynamics. Because if you want to model a protein actually folding in a molecular dynamics simulation to get the folded structure of the protein, this is pretty hard and time-consuming and computationally intensive. Whereas for AlphaFold2 or ESMFold, it takes a few minutes. You give it a big protein and it takes a few minutes. 


---


#### 2143.823

And I guess this is, in these cases, these are like language model-like models, right? They definitely have the architecture that looks a lot like language models, especially ESMFold. I think AlphaFold a little less because it has some of these extra architectural things that are a little more nuanced, like the MSA and the templates and such. But both of these models are very much inspired by language models. And ESMfold is pretty much just a language model. And you're able to predict these 3D structures with these things without really explicitly modeling any physics. And that provides a substantial speed up. And   
(2180.237) ~~I guess~~(2180.517)  
in terms of like how this relates to language modeling, so the concept that I think you're trying to grasp onto is protein motifs. or domains. 


---


#### 2192.333

So motifs are like reoccurring patterns that happen in proteins. They're like short little sequences of amino acids that recur often in lots of different proteins and generally have a very similar structure across different proteins, for example. This is   
(2208.623) ~~kind of~~(2208.983)  
a fuzzy concept, right? Like defining what a motif is and having that shape described is a little bit fuzzy, but these models learn this. And like you're saying, these   
(2221.352) ~~like~~ (2221.492)  
higher order concepts where you're looking at   
(2224.213) ~~like~~ (2224.353)  
groups of amino acids now instead of just the individual vocabulary elements,   
(2228.954) ~~right?~~ (2229.154)  
We're not just looking at individual amino acids of the vocabulary anymore. We're looking now at an aggregation of amino acids at a higher level. Like you can pull this out of these models and there's some work on this, some older work that's I guess maybe three years old or so now called Birtology Meets Biology. 


---


#### 2249.815

And they do a really in-depth study of how to pull out these different things, active sites and binding sites and motifs and things like this, based on the attention maps in the language model, in the protein language model. Another thing that people have found is the attention maps recapitulate the contact maps for proteins. And so the contact map is like a 2D matrix representation of all the contacts between the different amino acids in the protein, right? And it turns out the attention map, the matrix that you get from your attention mechanism, recapitulates that and is highly correlated with those contact maps. And so they are learning higher order concepts for sure, just as they do for natural language, for NLP domains. 


---


#### 2295.37

And you can do topic modeling and things like that on these models. But   
(2300.194) ~~I mean,~~(2300.374)  
that's a very specific example of how NLP has influenced AI applied to biochemistry. I would say now   
(2309.616) ~~the,~~ (2309.996)  
a lot of the more interesting models are more influenced by diffusion and flow matching models now.   
(2318.498) ~~Like~~ (2318.638)  
a lot of the generative models that we're getting that are   
(2321.459) ~~like~~ (2321.619)  
predicting the Boltzmann distribution or that are generating new protein structures for you with specific   
(2327.761) ~~like~~ (2327.921)  
shapes and functions or are allowing you to design new sequences that fold into a particular backbone. All of these things   
(2336.053) ~~are, a lot of them I should say,~~(2337.415)  
are more influenced by diffusion and flow matching than NLP and language modeling and transformers. 


---


#### 2344.923

I mean, some of them use transformers in there when they train the diffusion models, but they're starting to be a lot more influenced by Dolly-type models, I would say. Because you're starting to get this really fine-grained control over what kinds of proteins or small molecules or nucleic acids that you can generate. And there's actually some models that have come out that are text-conditioned. So a couple of the models that I mentioned were ProteinDT and MoleculeSTM. And these are generative models that are text conditioned and they allow you to type in   
(2381.361) ~~like~~ (2381.502)  
a natural language prompt and get out a molecule. So   
(2385.884) ~~like~~ (2386.024)  
protein DT, for example,   
(2387.965) ~~or,~~ (2388.105)  
or molecule STM, you can give it a text prompt and natural language, describing the properties of the molecule and just natural human language, giving it   
(2396.771) ~~like~~ (2396.931)  
this molecule has these chemical properties and it has this sort of bias away from or towards these amino acids or. interacts with these other molecules in such way. 


---


#### 2408.057

You can give it these natural language text prompts and it will generate proteins and small molecules for you that satisfy these constraints or that correspond to the text prompt that you give it. And there are more models like this that have come out recently that do similar things. They're text conditioned, like diffusion models or flow matching models that are generative and that produce molecules with specified properties based on natural language text, which in my mind, that's   
(2437.911) ~~kind of~~(2438.171)  
mind blowing. I think that's amazing. Having a model that will just generate molecules for you that fit natural language descriptions   
(2447.455) ~~is that's crazy.~~(2449.055)  
How did that happen?   
(2450.136) ~~Like,~~ (2450.256)  
that's amazing. Yeah. No doubt. So let me just rewind a little bit again, and then I want to get into a little bit more how that happened. 


---


#### 2457.926

So I always try to start with inputs and outputs as one good frame for understanding this stuff. So it seems like the first major breakthroughs in Afrobiology of the modern era, which is only the last however many years, were the structure prediction models. And   
(2480.042) ~~this is,~~(2480.883)  
if I understand correctly, there were about a proteins that had been analyzed to the point where people were pretty confident that they had a structure. If I understand correctly, this was mostly done through   
(2491.674) ~~x-ray crystalline, which is... Yeah,~~(2493.876)  
cryo-EM. Yeah. So I think that's why the initial things were   
(2499.421) ~~sort of~~(2499.701)  
limited to outputting a single predicted structure because if you're in like a crystal, you   
(2505.19) ~~sort of,~~(2505.451)  
by the nature of crystals, have a single repeating structure, right? 


---


#### 2510.012

So what we had was people put a lot of time in the lab into, first of all, figuring out how to get these things to crystallize, which is weird because they're not really   
(2520.936) ~~Protein crystals don't really~~(2522.237)  
occur in nature, right? That's a very odd thing in the first place. Maybe that's like gout,   
(2527.039) ~~I guess.~~(2527.299)  
It's   
(2527.459) ~~sort of~~(2527.699)  
like uric acid crystals, if I understand correctly. But you don't think of proteins... We think of them as floating around in solution or   
(2535.783) ~~kind of~~(2535.963)  
interacting with each other in complicated ways, but they're not in repeating lattice structures. So that in and of itself was   
(2542.506) ~~sort of~~(2542.726)  
a weird,   
(2544.047) ~~like,~~ (2544.207)  
closest approximation that we could get right if we got to make enough of this stuff that we can get it to put in coalesce into some crystal form, then we can hit with x rays and we can try to decipher how that gets scattered. 


---


#### 2555.213

And then we can come up with a structure and we hope.   
(2557.614) ~~I mean,~~(2557.974)  
we don't really know anything,   
(2558.995) ~~I guess,~~(2559.276)  
but   
(2559.536) ~~I guess~~(2559.756)  
it works well enough   
(2561.457) ~~that~~ (2561.558)  
that approximates the structure that it actually takes in the cell, but no guarantees. So first generation of stuff is not first generation, of course, we're like other AI techniques before this, but of these sort of modern wave of mega breakthroughs.   
(2578.092) ~~the~~ (2578.253)  
and   
(2578.493) ~~I guess that was~~(2578.913)  
really measured by maybe you could help me fill in some blanks here too   
(2582.419) ~~because~~ (2582.639)  
but   
(2583.52) ~~there's~~ (2583.72)  
it's like   
(2584.341) ~~kind of~~(2584.522)  
circular nature to some of this stuff sometimes   
(2586.645) ~~where I'm like wait a second~~(2587.426)  
so where is the ground truth it seems to be a little bit of it can feel like   
(2591.732) ~~uh~~ (2591.832)  
the ground truth is   
(2592.533) ~~sort of~~(2592.734)  
a shell game As I understand it, the way that AlphaFold was determined to be a breakthrough in the first place was that there was a competition held on an annual basis or whatever, where people would basically show up with their shape predicting model, and they would be given, here is the sequence. 


---


#### 2616.582

And their job is to predict the shape. And then the   
(2619.445) ~~test set,~~(2620.446)  
the sort of training set was all known proteins that came before. And the test set was all of the stuff that had been newly derived in the last year. So these were the new things that people hadn't been able to train on. They would show up and they would be measured against essentially the crystal based techniques and everything would fall short,   
(2645.169) ~~like~~ (2645.329)  
not nearly as good, not matching the crystal things. And then AlphaFold showed up and was like, oh, hey, it's, and this is where I get a little fuzzy. As I understand it, people would say it's in some ways even   
(2654.893) ~~like~~ (2655.053)  
better than the crystal techniques, but   
(2656.954) ~~like,~~ (2657.154)  
how do we establish that? 


---


#### 2659.054

How do we know that the when is the crystal technique right or wrong. I'm a little fuzzy on how we kind of pin down the ground truth when we know that the crystal thing is only an approximation and AlphaFold was kind of trained on that with augmented data like help me pin down the ground truth there if you can. Yeah   
(2676.789) ~~I mean~~(2677.069)  
ground truth in this case   
(2678.591) ~~yeah I mean~~(2679.011)  
this is a little hard and it's very   
(2681.213) ~~like~~ (2681.393)  
application and   
(2683.277) ~~like~~ (2683.437)  
situation specific, right? Depending on what you're trying to do and how you're trying to do it, you may want some crystallized structure that you got in a lab, or you maybe want like an alpha fold structure. 


---


#### 2693.366

And in other cases you might want like a trajectory or an ensemble of conformations, which wasn't really possible until more recently.   
(2702.433) ~~Like~~ (2702.594)  
observing the dynamics of a protein is really hard. And so to be able to model that on a computer and get predictions that are actually accurate about the dynamics of the protein and all the different   
(2717.721) ~~like~~ (2717.901)  
low energy conformations that it exists in,   
(2721.382) ~~like~~ (2721.502)  
that's pretty new. And in my mind, if you have the ground truth really ultimately is the Boltzmann distribution, right? Which is this very sort of theoretical physics idea that comes from like statistical mechanics. that's the ground truth. Whether or not you can model that on a computer or observe that in a lab is another question. 


---


#### 2745.787

But the Boltzmann distribution of the protein is the ideal ground truth. And is that basically like a... I guess I'm thinking of it in one sense as sort of like a potential, energy potential diagram where you have... It's related. It's a probability distribution, right? And it describes You can think of it in terms of an energy landscape, right? Because if you have this nice energy landscape, the low parts, the valleys that you have in your energy landscape are gonna be like the metastable states of the protein. They're gonna correspond to the metastable states of the protein. And then the peaks, like on top of the mountains,   
(2782.953) ~~right?~~ (2783.113)  
These are like states that are very transient and that are like unlikely to exist for very long. 


---


#### 2790.774

So when you're trying to model the Boltzmann distribution, you're trying to get out these like low energy conformations from it and then the transitions between those and understanding how often you transition between this state and this other state and what that transition looks like. I guess that would also be considered part of the ground truth, right, because this is all part of the dynamics of the protein in the environment and not just some single either crystallized structure or alpha fold 2 predicted structure. Yeah, so   
(2822.174) ~~I guess~~(2822.435)  
the answer to your question is the ground truth, at least to me, is the Boltzmann distribution. And the question of whether or not you can model that on a computer in a lab is a completely different question, but that's the ground truth. 


---


#### 2834.881

So it's a probability distribution of what percentage of the time the protein in some like neutral case solution or whatever is in shape A versus shape B, versus shape C, and then the in-between things are sort of   
(2853.393) ~~Here I'm kind of again returning to my slinky visualization where I could have the thing sort of in its lowest state or I could like tie its ends together and then it'll sort of make a nice circle and~~(2866.165)  
but again   
(2866.806) ~~kind of~~(2867.006)  
look compact and be   
(2868.287) ~~sort of~~(2868.528)  
in a relatively comfortable place but then the second that breaks it's like reverbing back until it gets to its normal state, that reverb moment is sort of the transitional state. 


---


#### 2878.168

It's not going to be in that state very long and it's   
(2880.409) ~~kind of~~(2880.729)  
on its way from one to another. So we don't know how many different, for any given protein, there could be   
(2886.771) ~~like~~ (2886.891)  
multiple different low energy states that it might spend time in. And there probably also is like a path issue to it where you maybe can get from A to B and B to C, but not necessarily A to C without going through B I imagine. Yeah, exactly. So lots of weird stuff there. And then, okay, so all that is just they interact with each other. So this is,   
(2909.882) ~~I guess,~~(2910.102)  
where AlphaFoldMultimer starts to come in? Yeah. AlphaFoldMultimer models the interactions between proteins, right? 


---


#### 2917.128

And you can model protein complexes. And there's actually some new results that just came out maybe a month ago, that computes something called the LIS score based on the PAE output of alpha-fold multimer. This is like a... Can you unpack both of those? Give us the PAE too. So the PAE is one of the outputs of alpha-fold multimer and it's, let's see if I remember what the abbreviation is for, predicted aligned error, I think is what it stands for. And this is telling you, it's a metric that tells you the quality of   
(2948.757) ~~the~~ (2948.897)  
the interfaces between the two proteins. You've got a lot of different metrics that come out of AlphaFold Multimer or AlphaFold2. So you have PLDDT, which tells you a per residue confidence score of how confident the model is that is the structure of the protein at that particular point   
(2967.52) ~~in the protein,~~(2968.2)  
like at that particular residue. 


---


#### 2970.5

And then you can take the average of the PLDDT and get an overall confidence for the whole protein. But then   
(2975.942) ~~you also have,~~(2976.542)  
you have IPTM and PTM scores, which are other scores that tell you about other aspects of the protein, and then you have these PAE outputs, predicted aligned error outputs, and these tell you about the quality of the interfaces between the proteins when it predicts the two proteins together. there's an interface region where the proteins are in contact with each other. And you can   
(2998.661) ~~kind of~~(2998.861)  
think of it as a certain cutoff, right? After a certain distance, you don't really count it as an interface residue anymore. But the PAE tells you the quality of these interfaces, how good of a quality the model has provided you. 


---


#### 3011.805

And you can compute something based on the PAE called the LIS. And the LIS score, let me look up what that stands for really quick, because I actually forgot what it stands for. So while you're doing that, I'll just riff a little bit on   
(3024.922) ~~the structure too. Or~~(3027.293)  
the nature of the interface, because this is just another level of like insane complexity, right? You have a range of   
(3034.078) ~~kind of~~(3034.318)  
whether these things are like jigsaw puzzle pieces that are perfectly fit to each other and have a really tight coupling or jigsaw pieces that   
(3043.585) ~~sort of~~(3043.845)  
fit. You can   
(3044.425) ~~kind of~~(3044.726)  
press them together, but they don't perfectly fit and they don't really want to stay together as much. 


---


#### 3048.729

All the way down to obviously they just don't fit at all and they just kind of don't adhere to each other. Is there anything more we could do to develop our intuition there for how strong is the strongest fit? I'm thinking like, boy, if I screw a screw into a nut, it's not coming off with any natural process. Somebody would have to come unscrew that. I'm guessing it's probably... I don't know. How tight are the tightest ones and what is the dynamic range of how adherent these things are to each other? Yeah, so there's two ideas that you're addressing here. One of them is like binding affinity, like how much affinity these two things have for each other to bind to each other. 


---


#### 3091.472

And then there's also in terms of like dynamics, like how weak or strong or how transient are the interactions between them in terms of like dynamics and like the time spent next to each other, right? There's recent work I think it's out of MIT, they built these flow matching models with AlphaFold and ESMFold. It's called AlphaFlow. And AlphaFlow, they use the AlphaFold2 architecture and they train it as a flow matching model, which is like a generalization of diffusion. And using this, they get these ensembles of confirmations for a protein. And part of the information that they get out of this is how transient the interactions between residues are. If you   
(3135.663) ~~produce,~~ (3136.244)  
let's say you run your alpha flow model and you produce   
(3140.027) ~~like~~ (3140.167)  
10,000 different confirmations or states that the protein exists in, and then you can   
(3146.672) ~~kind of like~~(3147.072)  
cluster those, like structurally, you can cluster them and then look at which residues are close to each other in each of those clusters. 


---


#### 3157.652

So maybe you take   
(3158.372) ~~the, you take~~(3159.592)  
the centroid or something of a cluster, and then you look at the distance between the residues, and then you look at other clusters, and the distance between the residues in those other clusters, and you get an idea of   
(3171.555) ~~like~~ (3171.795)  
how often two residues are in contact with each other from this. And you can tell how transient the interaction between these two residues are, and how much time they spend together. You could generalize this, right? And this is something that hasn't been done yet. So people who are looking for   
(3187.875) ~~like~~ (3188.015)  
research projects, this would probably be a pretty good one. If you generalize this to alpha fold multimer, do the alpha flow thing with alpha fold multimer, if it works well, and again, this hasn't been done before, but this would be a really great thing for someone to do. 


---


#### 3201.997

You could figure out how transient those interactions between two proteins are, right? Because now you have two proteins or more, maybe you have three or four or whatever, but you have two proteins that are in different conformations at different times. And AlphaFlow will generate all these different conformations for you. And then you can analyze all these different conformations and figure out how transient the interactions between the two proteins are and get an idea more about the dynamic side of things and not just a single number or a single metric like binding affinity, right? Because   
(3237.11) ~~binding affinity, I mean,~~(3238.11)  
it's a hard thing to predict. It's a hard thing to compute. training a model to predict binding affinity is actually a pretty hard thing to do. 


---


#### 3245.231

And most of them don't work. Most of them don't generalize well. But these approaches, like if you were to generalize alpha flow to the alpha,   
(3252.775) ~~like that,~~(3253.176)  
that would give you more information than just binding affinity.   
(3255.637) ~~That would give you,~~(3256.278)  
that would give you some notion of how often particular residues of the two proteins are in contact with each other. And then,   
(3263.903) ~~like I was saying before,~~(3264.723)  
the LIS score, this is the called the local interaction score. They use alpha fold multimer and they get the PAEs out of alpha-fold multimer. And then using the PAE, they compute the LIS, which is a pretty simple computation.   
(3279.152) ~~I don't know that I can describe it in words,~~(3280.914)  
but it's not a terribly complicated thing to compute. 


---


#### 3284.116

Once you have the PAE, the LIS is pretty easy to compute. And this tells you how likely you are to have a protein interaction, which kind of gets that binding affinity to some degree. And being able to predict protein interactions is actually a really hard problem. And most models that try to predict protein interactions don't work well and don't generalize well. And there's actually   
(3307.675) ~~a kind of~~(3308.315)  
a big problem with a lot of these models. So when people are training them, a lot of times if you're training a model that takes as input protein sequence or two protein sequences, people don't split their data in the right way. you have this notion of sequence similarity and   
(3325.475) ~~if you if your data~~(3326.716)  
if your training data has sequences in it that are very similar to your test data sequences you're going to get overfitting and you're not even going to realize it like all the usual signs of overfitting aren't going to be there but you're going to overfit without even realizing it because you're going to have training data and test data that's highly similar to each other in terms of sequence similarity. 


---


#### 3351.248

#### 3392.05

So that is basically the actual positioning with sort of a confidence indication. Yeah. And it tells you what the quality of the interfaces are between the two proteins that you're predicting in the multimer. And something else we should probably get into that directly follows from alpha-fold multimer is other ways of generalizing the alpha-fold model or training models that are like alpha-fold that do more than just proteins. You might have complexes where there's a protein in a small molecule, or protein in DNA, or protein in RNA, or a metal, or whatever. And so there's all these other biomolecules that you might want to model in complex with each other. And to generalize AlphaFold Multimer to this new situation is pretty hard, but some people have managed to do a pretty reasonable job of it. 


---


#### 3448.39

I think there's still room for improvement on these, but like a new model that just came out recently is RosettaFold AllAtom. And RosettaFold AllAtom will let you predict complexes that have proteins and small molecules, proteins and nucleic acids, and proteins, and proteins and metals too. Big step forward now, because now you can apply this idea of computing the LIS score to these other complexes. And you can get this score that tells you how likely there is to be an interaction there and how strong that interaction is. And you could also,   
(3483.466) ~~I don't know how hard this would be to do, just thinking about it now, it seems like it might be actually kind of hard, but you could probably do~~(3492.499)  
the alpha flow type method with something like Rosetta fold all atom as well and get something like conformational ensembles out of it. 


---


#### 3502.506

And that's probably, something like that is probably coming soon. Somebody's going to work on that eventually. So yeah,   
(3508.711) ~~I think~~(3508.971)  
I answered your question.   
(3509.792) ~~I'm not sure. Yeah. Let me just think about where I want to go back to. Okay.~~(3514.615)  
The one thing that you said that caught my attention was, this is all in the context of predicting shapes. We need to predict shapes because we need to understand how things interact. Now we're even getting into predicting how things conform to each other. So the shape of multiple things as they're in actual interaction. and we get these sort of positional predictions that can be   
(3538.656) ~~sort of~~(3538.876)  
cashed out to these parts are actually   
(3541.117) ~~like~~ (3541.337)  
interacting in a meaningful way and this is really where the action is versus these other things are   
(3545.719) ~~kind of~~(3545.9)  
distant from each other that's not really where the action is that's being generalized beyond all proteins to like all the different kinds of things that are meshed up together in a cell. 


---


#### 3559.151

But I believe you had said that there were like as many as 10,000 possible confirmations for a single thing. Was that, did I get it? Yeah. So like AlphaFlow, when you run AlphaFlow, it generates confirmations of a protein for you. And it was trained on molecular dynamics data, on simulation data. And so it does have some notion of   
(3583.95) ~~like~~ (3584.11)  
dynamics. And what it does is it produces different confirmations of the protein for you. And you can tell it how many of these to produce, right? And the more that it produces, the more likely you are to get a nice global picture of all the different confirmations that might exist for that protein. AlphaFlow, so we've actually tested AlphaFlow on these proteins that are called fold-switching proteins. 


---


#### 3611.344

Fold-switching proteins, so like probably the most popular example floating around in the literature and in the community right now is Kybe. And Kybe is this fold-switching protein that like 10% of the time it exists in this one conformation and then 90% of the time it exists in this other conformation. And this is influenced by   
(3629.694) ~~like~~ (3629.814)  
a circadian rhythm. So it's like a night-day cycle sort of thing that's influenced by like your circadian rhythm. And when you apply AlphaFlow to some of these fold-switching proteins, it doesn't capture both of those fold-switch states. So in the example of Chi-B, it actually only really predicts conformations that are relatively close to the fold-switch state. which is like the slightly higher energy confirmation, the one that's a little bit less likely, the one that it exists in 10% of the time, which is a little bit odd, right? 


---


#### 3664.922

Because you would expect and maybe want your model to go for the ground state or the lowest energy confirmation. And for some reason, it   
(3674.867) ~~like~~ (3675.027)  
sticks   
(3675.507) ~~kind of~~(3675.767)  
close to the fold switch confirmation. I'm not sure that there's like a good explanation for why. And that really goes,   
(3684.635) ~~I think~~(3685.076)  
it goes back to the AlphaFold2 predictions, because when you predict the structure using AlphaFold2, you get the fold switch state, you don't get the ground state. And people have done all kinds of little hacks to try and get out the ground state instead of the fold switch state. And the most popular method that they've hacked together is doing MSA subsampling or clustering the MSA and using the different clusters to predict structures, because If you take your MSA and you cluster all of your sequences in your MSA, you're   
(3719.326) ~~kind of like~~(3719.967)  
you're grouping the sequences in the MSA in a way that captures certain evolutionary information. 


---


#### 3728.352

And different clusters will focus on or accent particular conformations. And so if I take out one of my clusters and predict the structure using those clusters in the MSA, I'll get a confirmation out from AlphaFold2. And then if I pick   
(3744.994) ~~a different set of,~~(3745.975)  
a different cluster of sequences in my MSA, I'll get maybe a slightly different confirmation, or maybe a drastically different confirmation. And   
(3755.101) ~~if you do this,~~(3755.681)  
if you do this right, sometimes, not always, but sometimes, you can get out the different confirmations of these fold-switching proteins. And for Ki-B, they've done this successfully, and for a few others, but it's not a super robust method, And   
(3770.883) ~~I think these alpha flow, I think,~~(3774.104)  
is in some ways maybe more informative. 


---


#### 3778.106

And something like Boltzmann generators or distributional graph former, I think, are significantly better in terms of how they approach the problem, because they're going to give you more information and they're gonna give you more robust information. So for example,   
(3795.929) ~~like~~ (3796.049)  
distributional graph former, you're gonna get out something more robust and more informative than if you're just like clustering the MSA or subsampling the MSA for alpha. Can we talk about this MSA thing for a second?   
(3810.514) ~~If I understand clearly, I'm not even sure I should attempt this, but I'll go for it.~~(3814.335)  
Is it basically that we know that a gene codes for a protein, we have a lot of variation in the genes. The genes can have lots of random differences between them, but we can   
(3828.11) ~~sort of~~(3828.33)  
identify that these are all different variations on the gene. 


---


#### 3832.194

Some of the genetic, some of the DNA level differences may make no difference in the protein, but others will make differences in that at a particular position in the protein sequence, you'll have a different amino acid. And so now you've got   
(3847.798) ~~kind of~~(3848.098)  
the same protein, but it can have different elements in particular position. And so these are grouped for the purposes of prediction?   
(3858.686) ~~Kind of.~~(3859.066)  
So an MSA is actually a pretty old concept that comes from computational biology. People have been using MSAs for a long time. And essentially, it's based on the edit distance. So if I have just a string of characters and I make some edits in some different places, I can compute the edit distance between those. 


---


#### 3881.934

And if I have a low edit distance, then those two sequences are highly similar. MSAs are basically this. I take a protein and I have a whole bunch of different mutations of that protein or a whole bunch of other protein sequences that are very close to that protein in terms of sequence similarity, but they have some changes here and there. A lot of times the changes that happen only happen in certain regions of the protein. And then there are other regions of the protein that are highly conserved. And so when you do an MSA, you can look at which regions of the protein are really highly conserved. And a lot of times this will give you some indication of which parts of the protein are going to affect the function if you like mutate them and stuff. 


---


#### 3927.44

So if I have a highly conserved residue that in my MSA, it just doesn't change. It stays the same through pretty much all of the MSA. Like 90% of the sequences in my MSA, this amino acid stays the same, right? If I change that, if I mutate that, it's probably going to affect the function of the protein. Because it's like a highly conserved region of the protein that evolution hasn't changed or has changed very infrequently. And so because of that, if you change some of those residues that are highly conserved, oftentimes you'll degrade the function of the protein or change the function of the protein, or maybe you'll decrease its thermal stability or something like that. 


---


#### 3969.599

So MSAs are just telling you, they're telling you evolutionary information that is conserved among a whole group of proteins that are highly similar to each other in terms of sequence similarity. And AlphaFold2 uses MSAs. You can either use the database of MSAs or you can have it compute them on the fly. And it uses these MSAs to inform how it predicts the structure of the protein. Because when you have proteins that are very closely related evolutionarily, in terms of evolution, their structures are often very similar,   
(4003.702) ~~right?~~ (4003.862)  
And that's not always true. Like, I can have two proteins that are very similar, but have very different structures. Like, that happens all the time. But if you have this extra evolutionary information in the form of an MSA, you have extra information that helps you predict the structure of the protein, because all of these evolutionarily related proteins are oftentimes going to have very similar structures to your protein of interest. 


---


#### 4030.231

So sort of calling to mind the classic image of the plane with all of the spots where the planes came back having been shot and then all the places that they didn't observe, those were the planes that got shot down. So this is the evolutionary equivalent of that where we don't see changes in certain regions because they're super core to functionality. And that in turn is super useful for prediction making because   
(4059.77) ~~that~~ (4060.37)  
these parts are like the really important parts and they're going to have to fit together or the sort of interactions that they have with other things are   
(4067.334) ~~kind of~~(4067.674)  
the whole point of what's going on here. Okay. So that's interesting. The overfitting piece, 


---


#### 4072.196

I didn't quite understand. It seems like that's related though, where you said because these things are so similar, You have to be careful that you're not, give me the overfitting thing again. Cause   
(4082.501) ~~I can't,~~(4082.781)  
I'm not sure I can do it justice. Like when you do a train test split in deep learning and you're training your neural network on your train, on your training data, and   
(4092.288) ~~you have,~~(4092.648)  
you have your test data to   
(4094.389) ~~sort of~~(4094.709)  
test your model on after the fact, once it's trained to see how well it predicts on data that it hasn't seen before. And so when you're doing this, you want to make sure that your test data doesn't have a bunch of sequences in it that are highly similar to your training data. 


---


#### 4111.178

Because it's almost like you're training on the same thing twice and you overfit this way. You don't get a good indication of how well your model generalizes. And a lot of people do this. A lot of people coming from   
(4122.061) ~~like~~ (4122.201)  
deep learning, just getting into   
(4123.761) ~~like~~ (4123.881)  
the biology stuff and they don't have a super strong background in biology. They make this mistake very often. And so there's just tons and tons of neural networks and different kinds of deep learning models out there. that don't generalize and that are very overfit because they didn't split based on, they didn't split their data based on   
(4142.01) ~~like~~ (4142.17)  
sequence similarity   
(4143.571) ~~and or~~(4143.991)  
structure similarity. So   
(4145.532) ~~you,~~ (4145.712)  
like when you train models, usually you want to split your data based on sequence similarity and or structural similarity. 


---


#### 4154.256

And a lot of people also split it based on like dates, like you were talking about CASP earlier. They have a certain cutoff date, and then the stuff that was resolved after that cutoff date is used in the test data. But when you're training, you're doing your training data, but you split your data based on things like sequence similarity and or structural similarity to make sure that you don't overfit and to make sure that your model generalizes to unseen data. Gotcha. Interesting. Okay. Yeah. It seems like in the case of something about this that I don't have a good intuition for, because that's not really done in language modeling, right? In language modeling, you could certainly have like lots of sentences that are very similar and you don't sort of say, oh, we're going to hold out. 


---


#### 4198.03

We don't, we don't draw conceptual lines between different parts of the data and try to generalize across those lines. So what is the difference in the biology context?   
(4208.897) ~~Like~~ (4209.037)  
my intuition says to the degree that this thing is learning that these models are learning like the higher order concepts that really matter. that they should be able to learn those kind of regardless. And again, in the language model case, we don't really have a concept of overfitting, at least in the large-scale foundation models. Is this maybe just because we're not really doing large-scale foundation models in quite the same way? Or how would you describe the difference? I mean, there's still a concept of overfitting in LPN training big giant models, 


---


#### 4241.068

CLAWD or CHAT-GPT or whatever. You can definitely still overfit these models. Very often for an NLP models, like these really big chat type models, like really big LLMs and stuff. First of all, they often only train on one pass through the data, right? They don't do multiple passes. And partially because of that, overfitting is not much of an issue because you're not training multiple times on the same data. So I do think that is changing. One little nugget from the recent Zuckerberg Dworkesh interview that I definitely made my ears and brain light up was when he said they trained these latest llama models on 15 trillion tokens. He said, we   
(4279.966) ~~kind of~~(4280.206)  
stopped because   
(4280.907) ~~we,~~ (4281.047)  
at some point we need to move on to Lava 4. 


---


#### 4283.888

But he said we could have rotated the high value tokens through again. And I was like, Oh, interesting. I've seen some results about that, but in any event, it does seem   
(4292.791) ~~there's,~~ (4293.011)  
we're now to get to 15 trillion tokens. Basically, I don't think you have much choice, but to rotate. Yeah. Anyway, that's a bit of an aside, but I'm still not quite grokking it to be honest. Okay.   
(4305.336) ~~So let's see,~~(4306.237)  
what's a good analogy. I'm trying to think because yeah. And like NLP, like most people don't really think about the, so you have a data distribution and your training data and your test data, like your test data is supposed to tell you something about how well the model generalizes. 


---


#### 4324.147

Right. And it's also supposed to tell you about if the model's overfitting or not, because when you compare your training metrics to your test metrics, whatever they may be. If your training metrics are different, like the training test, or the training metrics and the test metrics are substantially different, then you're either overfitting or underfitting. If   
(4346.614) ~~your test metrics,~~(4347.695)  
if the metrics on your test data are substantially worse than the metrics on your training data, then you've overfit, right? And if it's the other case, if your test data is substantially better than your training data, which is   
(4365.495) ~~kind of~~(4365.735)  
hard to do, then probably you could train some more. Maybe you're under fit. So your trained test split is supposed to tell you something about how well the model generalizes and how overfit your model is. 


---


#### 4379.801

And comparing how it performs on the training data to the test data tells you that.   
(4385.142) ~~It tells you a lot about how overfit your model is, if it's overfit,~~(4388.604)  
and how well it's generalizing to data that it hasn't seen before. And to really   
(4392.666) ~~get a good grasp,~~(4394.066)  
to get a good idea of how well your model is generalizing to unseen data, you want at least part of your test data to be very dissimilar from your training data. Because that means it's generalizing to things it hasn't seen before, right? That means it's picked up on some deeper concept and language that generalizes to areas that it hasn't seen before, and it's using those really deep concepts to make predictions or generate things that are out of distribution. 


---


#### 4426.679

And this is a big thing that people discuss, is whether or not these things generalize to data that's out of distribution. And if you train them in the right way, you can get models that generalize well to out-of-distribution data, right? This is not something that's impossible to do, you just have to do it right. And in the case of biology or biological sequences like proteins, to get a test set that gives you a good indication of one, how well the model is generalizing, and two, if it's overfit or not, you need to make sure that your test data is very dissimilar from your training data. And the way that you do this is you look at the sequence similarity between the protein sequences in your training data and your test data. 


---


#### 4473.847

And you can also look at structural similarity, because you can have different sequences that are very different in terms of sequence similarity, but that fold into the exact same structure, more or less, right? We can have two very dissimilar protein sequences that fold into pretty much the same structure. And so sometimes depending on what your model architecture is and what your goal is, you may also want to split based on structural similarity and not just sequence similarity to make sure that your model is generalizing and not overfitting. Okay.   
(4505.407) ~~I think~~(4505.607)  
I got it. Does that make sense? Yeah.   
(4507.748) ~~I think~~(4507.988)  
so. It seems that it is   
(4509.848) ~~sort of~~(4510.268)  
a form of data leakage, essentially. Like you could imagine, and it's   
(4514.249) ~~sort of~~(4514.629)  
that you're fooling yourself, right? 


---


#### 4516.089

For any given architecture, presumably the very best performance would be if you trained on all the data. But in order to effectively evaluate your architectures along the way, you need to have some holdout or you might call it a benchmark in certain contexts to evaluate against. And these similar enough sequences basically are a data leak in the same way that if you find out after you do your thing that, oh, hey, we actually had MMLU in the training data for the language model, then it means, oh, you can't really trust the MMLU scores anymore. And the model still may be good, it may not be so good, but if you train on MMLU, we can't really score you on MMLU. 


---


#### 4559.019

And this is a similar problem. You can't trust her. Exactly. Exactly. Yeah, exactly. And there are even more nuanced ways of splitting the data, too, for specific things. The new version of DiffDoc They trained a new version of DiffDoc, I think they call it DiffDoc L, because it's larger. It's the large DiffDoc. And they use this method called confidence bootstrapping, which is   
(4584.07) ~~sort of~~(4584.33)  
like reinforcement learning. And they also split their data in a really unique way that's based on different domains or motifs that are present in certain interactions. They split their data based on that, in addition to,   
(4601.309) ~~I think,~~(4601.809)  
sequence or structural similarity. I would have to look at that. they split their data based on these domains that are present in these interactions to train a model for docking, right? 


---


#### 4611.76

So you have a ligand, a small molecule ligand that you're trying to dock into a protein and do like blind docking, which is a hard problem. And they get like substantially better performance and it generalizes a lot better in this new version of DiffDock because of the way that they trained it and the way that they split their data. And they have some really strong confidence that their model is generalizing to out of distribution data, and it's able to predict on things that it hasn't seen before, and they're very dissimilar from what it has seen. So   
(4643.545) ~~just to,~~(4643.846)  
not to interfere, but just to make sure I understand, when you said, I've lost exactly what you said, but I just want to make a distinction between what they've demonstrated is that you should be more confident in doing this stuff in totally new regimes based on the fact that they've been very meticulous in the data split. 


---


#### 4662.835

Whereas if they had thrown everything into the training, then you would have a hard time knowing to what degree to be confident in out-of-distribution stuff. They did a really good job with that model. I think their performance boost was pretty big. They got a lot better performance out of it too. That's definitely a good model to look into if you're looking to get into this stuff. So   
(4685.967) ~~maybe let's, I don't know if there's more that you think we need to cover on.~~(4690.269)  
  
(4690.469) ~~I mean,~~(4690.809)  
we've been up and down the layers of or the levels of abstraction, but it seems like the two big things that I want to go to next   
(4699.833) ~~and~~ (4699.973)  
being mindful that we've already been at it for a while are the diffusion concepts where it seems like we're moving from predicting a structure to generating new things. 


---


#### 4712.416

And then maybe we could get into a little bit of, okay, in actual work, like what are the cycles that are used to actually make progress on questions of interest? Like you have a target, you want to make some modification, like how do these things fit together to allow us to work a lot faster and get more value from our limited work resources? Before we go on to the diffusion and generative side, though, anything else that we didn't cover   
(4737.291) ~~or that you think is a missing part of the piece,~~(4739.013)  
a missing part of the picture for the fundamentals or the structural prediction? No,   
(4743.418) ~~I think,~~(4743.738)  
yeah, we should move into RF diffusion. I think that's a good direction to go in now. 


---


#### 4749.565

Are you familiar with RF diffusion at all? No, not really. Although, from what little you said earlier, it sounded to me like CLIP, basically. I was   
(4758.839) ~~sort of~~(4759.08)  
hearing that,   
(4762.121) ~~you know,~~(4762.421)  
with CLIP you have   
(4763.602) ~~kind of~~(4763.922)  
images and their captions, and here it sounds like we have   
(4766.603) ~~like~~ (4766.743)  
proteins and their sort of descriptions. No, so that's ProteinDT and MoleculeSTM. Those are much more like CLIP. They use the exact same method as CLIP. They use contrastive learning and they have   
(4778.19) ~~like~~ (4778.37)  
captions and molecules or captions and proteins. And so those are our text condition models where you can type in a natural language description of your molecule or your protein without a structure or a protein sequence that fits that description. 


---


#### 4795.573

And so those I think are a bit different from RF diffusion. RF diffusion is a diffusion model that it's not text conditioned. You can condition it on other types of things, but you don't give it a text input. It's   
(4810.52) ~~a little more, I guess,~~(4812.225)  
a little more specific. and it's a little more geared towards people who want to perform surgery on proteins. So if you want to design new proteins with specific structural properties and you want to get your hands dirty and perform surgery on these proteins and graft them together or take pieces from this one and graft it onto this one or generate a protein with a specific sort of fold tertiary structure   
(4838.882) ~~or~~ (4838.922)  
or maybe generate a protein that binds to a specific protein with really high affinity and specificity. 


---


#### 4847.316

These are the things that RF diffusion is good for. So RF diffusion is a diffusion model. They used Rosetta fold, the Rosetta fold backbone, and trained it as a diffusion model to denoise 3D structures of proteins. And there are several different versions of RF diffusion. There's a new version that just came out called RF diffusion all atom. which allows you to generate proteins that will bind to small molecules. So you can generate proteins with binding pockets that are highly shaped complementary to a small molecule ligand. And with RF diffusion and RF diffusion all atom, you can also do something called motif scaffolding, which is where you pull out motifs from a protein that you like. 


---


#### 4892.696

Maybe they're like binding sites or active sites, or maybe there's a particular segment of the protein that binds to a different protein that you're interested in or performs a specific function. And you can pull these pieces of the protein out and scaffold them and build a new protein around those pieces that holds those pieces in place so that you have a new protein with very specific 3D structure that performs like some very specific function. And it's been a very influential model and a very useful model. And it's definitely one of my favorites.   
(4926.291) ~~Maybe we should dig into that a little bit. Yeah.~~(4928.212)  
Give me a little bit more on   
(4929.093) ~~how,~~ (4929.393)  
what exactly it is that you're specifying. 


---


#### 4931.614

It's not text conditioned, but you're saying I want it to have certain properties and then it's filling in the sequence that gets you to those properties. Yeah.   
(4942.46) ~~So like the most,~~(4943.661)  
the most basic usage of RF diffusion is unconditional generation of a protein. So   
(4948.624) ~~you just,~~(4948.944)  
you tell it some length. or range of lengths, and it will just generate proteins of that length that are brand new, that have never been seen in nature before, and very often are very designable and that you can actually synthesize and create in a lab. And that's just completely unconditional generation. You don't give it any sort of constraints. It just generates a new protein for you of a particular length. 


---


#### 4975.683

But then you can also, one of the really interesting functions of RF diffusion is it will design binders for you. So if I have a target protein and I want to design a protein that binds to it with really high affinity and really high specificity, RF diffusion is really good at that. It'll design binders for pretty much any protein you can give it, and   
(5000.106) ~~very often~~(5000.827)  
The proteins that it designs that bind to your target protein are very high affinity and very high specificity and often very thermostable. The other functionality that's really useful is the motif scaffolding that I was talking about before, which is where you pick out pieces of a protein or multiple proteins and you build a new protein that holds all those different pieces in place in a particular way. 


---


#### 5027.816

And so this is one thing that you could imagine doing with this would be like building or designing an adjuvant or like grafting two proteins together. Or let's say I have one part of a protein that binds to protein A and I have some other protein that binds to protein B. And I want to design a protein that binds to both protein A and protein B so that I can get a complex with three proteins in it, right? I want to have a protein that binds to protein A and protein B. So what I can do is I can take those pieces out of the protein that bind to protein A, and I can take the pieces that bind to protein B, and I can scaffold them together into a new protein. now I've got a new protein that binds to both of those proteins. 


---


#### 5076.666

And I can do things like build out protein interaction networks this way. So if I want to design a particular protein interaction network, this is really useful for that. That's a pretty technical and involved thing to do. Like building up a protein interaction network is a non-trivial thing to do, but you can do it with RF diffusion. You can design proteins that will bind to multiple different proteins in multiple different contexts and build out these networks this way. And this gives you   
(5106.303) ~~like~~ (5106.443)  
a way to modulate protein interaction networks, right? Because if you design a binder to block a particular interaction, you can modulate your protein interaction network by blocking particular interactions by designing a binder. 


---


#### 5119.351

But you can also add in interactions that weren't there before using the motif scaffolding or maybe binder design and motif scaffolding together. So it's very useful in a lot of different contexts, but it's not text-conditioned like ProteinDT or MoleculeSTM or some of the other text-conditioned diffusion models for proteins, because there are a few others now that recently came out as well. But yeah, it's not text-conditioned. It's very much more geared towards people who are really interested in performing surgery on proteins and protein interaction networks. And now with RF diffusion all-atom, also with other interactions as well, because with the all-atom models, you can model more interactions than just the protein interactions. So how does this in practice get used? 


---


#### 5165.966

Maybe the cancer example from the top is a good one, or we could go to another one. Yeah. In that scenario, we sort of already had an understanding of the cancer cell has this thing that disables the immune cell. And so then you could say, okay, let's brainstorm some ideas here, right? If we can bind something to that bit of the cancer cell that would   
(5194.922) ~~kind of~~(5195.202)  
cap it, blunt its ability to then interfere with the immune cell, then the immune cell presumably would do its job still and kill the cancer. Of course, you've got highly tangled webs of interaction that you're doing this within. but you've got to take something local like that. Now   
(5211.816) ~~kind of~~(5212.016)  
take me through the cycles and the practical application of some of these tools for a specific problem of that sort. 


---


#### 5219.398

Yeah, so I've got a few examples here that we can talk about. I wonder which one would be like the best or the most interesting for people. So   
(5227.381) ~~like~~ (5227.521)  
the one that we were talking about earlier with the cancer, with PD-1 and PD-L1 is a really good first example that   
(5233.993) ~~I think~~(5234.193)  
is a really good place for pretty much anybody to start. Because you can very easily and very quickly design a binder to one of these proteins with RF diffusion. It's really good at designing binders for pretty much anything. If I have this PD-1, PD-L1 interaction between these two proteins, essentially what's happening is the cancer is turning off your immune system's response to it, and then your immune system doesn't effectively combat the cancer. 


---


#### 5259.188

But if I design a binder to one of these two proteins to block that interaction, and my binder out-competes that interaction, so it has a higher affinity than the PD-1, PD-L1 interaction has, then I can successfully block that interaction and prevent the cancer from turning off the immune cell's responses to it. So that's a really good place to start. Another way that RF diffusion can be used, so let's say you have a protein that binds to a target, but it doesn't bind very well. The affinity is   
(5293.771) ~~kind of~~(5294.031)  
low and the shape   
(5295.332) ~~complement~~ (5295.753)  
complementarity isn't terribly good. I can use RF diffusion and something like protein MPNN or ligand MPNN to modify that and increase the binding affinity. 


---


#### 5307.942

So something I can do with RF diffusion is partial diffusion. So   
(5311.783) ~~I can get,~~(5312.424)  
I can take my protein of interest that binds to my target and I can perform partial diffusion, which is where I add a little bit of noise. I don't completely noise it. I don't turn it into a Gaussian distribution or anything. I just add a little bit of noise into it. and then have RF diffusion denoise that. And what it'll do is it'll denoise it into a structure that's   
(5331.699) ~~kind of~~(5332.059)  
similar to the one that I started with, but it's also a little bit different now because I added that noise and then denoised it with RF diffusion. And if I do this and I give RF diffusion the target protein that I'm interested in, 


---


#### 5343.843

I can improve the shape complementarity between those two. So the new denoised protein or the new denoised version of my original protein is gonna have a higher shape complementarity to my target. And then I can go and design sequences for that backbone that are different from my starting sequence,   
(5361.535) ~~right?~~ (5361.715)  
So maybe my starting sequence, maybe there were some residues that had unfavorable chemical properties at the interface,   
(5369.038) ~~right?~~ (5369.258)  
Maybe I need to use different amino acids to improve some chemical properties so that the binding affinity goes up,   
(5378.002) ~~right?~~ (5378.182)  
I can do that with   
(5380.256) ~~like~~ (5380.436)  
protein MPNN or ligand MPNN. So ligand MPNN is the newer all-atom version of protein MPNN. It's an improvement on protein MPNN, and it also generalizes to contexts where you have other kinds of molecules other than just proteins. 


---


#### 5395.84

And I design a sequence with ligand MPNN, and I can tell ligand MPNN to bias certain residues towards certain amino acids or away from certain amino acids, like at the interface, for example. to get those more favorable chemical properties to increase my binding affinity further. And   
(5416.034) ~~I can also,~~(5416.734)  
there's also versions of ligand and PNN that will allow you to specify   
(5420.597) ~~whether a residue,~~(5422.298)  
so let me check on this really quick, whether a residue is a buried residue, an interface residue, or something else. I can also tell ligand and PNN about symmetries, which is a really interesting thing that RF diffusion and ligand and PNN can do together. Just to clarify, RF diffusion doesn't usually get used on its own,   
(5443.882) ~~like~~ (5444.022)  
by itself, because it just works in structure space, right? 


---


#### 5448.824

So it's doing the denoising process on the structures of the proteins. It doesn't know anything about the sequence of the protein. So I need a separate model, like Ligand and PNN, to design the sequence for that 3D structure. So they   
(5462.371) ~~kind of~~(5462.632)  
go hand in hand. You use them together. So once you've generated your 3D backbone of your protein, you design a sequence for it using ligand and PNN. And using these different functionalities of ligand and PNN, you can increase your binding affinity and other properties even more. Yeah, so like using partial diffusion with RF diffusion to slightly noise and then denoise a structure that you already have. can help you increase things like binding affinity and things like thermostability and other properties. 


---


#### 5493.634

Then, let's see, what's another application of RF diffusion? So one that I was looking into recently,   
(5501.079) ~~let's see,~~(5501.499)  
I want to pick out a good one because I want to give people really interesting examples to think about because you can really do a lot with these models if you get into it pretty deep and really learn how to use them.   
(5512.906) ~~Let's see, there we go.~~(5513.947)  
Okay, yeah, so there's unconditional generation, symmetric generation. I touched on that a little bit. You can design symmetric oligomers. Let's say I want to have a protein that interacts with itself, or other copies of itself, I should say. And if I have enough copies of this protein, it forms a symmetric complex. 


---


#### 5539.519

For example, Let's say I have a protein that fits together with two other copies of itself in a triangle formation, right? And it's symmetric to the cyclic group of order three, right? So I've got a order three rotational symmetry that's happening. I can use RF diffusion to generate proteins with symmetry like this. And it has other symmetries that it can use. So there's dihedral symmetries, there's symmetries icosahedral symmetries and tetrahedral symmetries, in addition to the cyclic symmetries. And   
(5574.372) ~~I can,~~(5574.652)  
the cyclic and the dihedral, I can choose like any order, cyclic group or dihedral group for my symmetry for those. And RF diffusion will design a symmetric complex of proteins where there's like multiple copies of the protein in this like nice symmetric structure. 


---


#### 5593.257

And where this occurs, like this occurs in nature in multiple places. One example is in viral capsids. And they've also recently some David Baker's lab recently published some work where they design these like symmetric oligomers as like biosensors. And I think they also designed some to help with   
(5616.71) ~~like~~ (5616.85)  
drug delivery. So they have these   
(5619.092) ~~like the~~(5619.692)  
like pocket that forms when you have a cyclically symmetric complex of proteins that the pocket that forms inside of that. You can design that in such a way that it captures a small molecule drug really well and delivers it to somewhere in particular, right? So that's another application of RF diffusion that's really useful. What else? There's the binder design. 


---


#### 5644.257

#### 5680.959

So it's like this, it has like beta sheets in it. And they form this, like, sort of barrel-shaped protein. Let me see if I can send this to you so that you can see it. Yeah, I've got a couple pulled up as well. Okay.   
(5694.142) ~~We can add one to the... I mean, I can even share here in the moment just to capture what I'm looking at. Yeah, maybe let's share. Do that.~~(5699.665)  
So this is an 8.   
(5701.165) ~~And if you turn this sideways... Yeah, if you turn this sideways, it should look kind of like a barrel.~~(5707.289)  
So maybe let's scroll down a little bit. I wish there was, like, a side view of this thing. Oh, there's one. 


---


#### 5712.645

Do you see the red? Yeah, there it is. You see how it's turned sideways? It's   
(5716.046) ~~kind of~~(5716.206)  
like a barrel shape. It's like this tube. So that's a TIM barrel. So I can tell RF diffusion specific tertiary structures to generate. And it will generate these different folds for you. It's called fold conditioning.   
(5731.472) ~~And then let's see. Let me find some good specific applications to~~(5736.373)  
specific proteins. So here's a good example of how to use motif scaffolding. Let's say I want to design a protein inhibitor of,   
(5746.285) ~~maybe I shouldn't, I don't know if I should~~(5747.706)  
just read this off because this is   
(5749.106) ~~like~~ (5749.246)  
really technical, but there's a protein called p53-mdm2 interaction. There's two different proteins that are interacting with each other, p53 and mdm2. 


---


#### 5758.63

And if I want to design an inhibitor for this, maybe I could   
(5762.772) ~~like~~ (5762.932)  
could extract the motif corresponding to the p53 peptide and then use that to design a new protein, scaffold that with the motif scaffolding. And then I can optimize it using partial diffusion and ligand and PNN to design sequences that have favorable chemical properties. And then I can check and see using the LIS score from alpha-fold multimer how well my new protein interacts with MDM2 or p53. These are so technical, I hate to just read these off, but I feel like I'm just going to go into the weeds and talk about a bunch of really specific proteins and domains and stuff. I don't know if that's very interesting. 


---


#### 5809.172

The sort of conceptual loop, I think, is really interesting. And if I'm getting it, it's like, okay, we have an interaction that is problematic. we want to interfere with it one way or another, we can like cap the one thing or cap the other thing. And so there's this kind of cycle of generate a 3D structure, that's one model, generate a sequence to do that, that's another model, refine those, that's   
(5833.906) ~~I guess~~(5834.186)  
yet another model to look for various refinements or   
(5838.147) ~~kind of,~~(5838.407)  
as you said, chemical, favorable chemical properties? Same thing maybe? No, you don't need another model for that. You can just RF diffusion and ligand NPNN, you can do it with those two. 


---


#### 5848.09

You don't need anything else really. So RF diffusion designs the structure and then ligand NPNN designs the sequence for that structure that will fold into it so that you have something you can actually go and synthesize in a lab,   
(5858.713) ~~right?~~ (5858.893)  
you need a protein sequence to synthesize to get the protein structure, because RF diffusion just works at the level of structure. It doesn't know anything about sequences. And then you're validating this to the degree that you can validate it before you're actually doing any actual lab work with something like Alpha Multimer and looking for a high score there. So how quick does this happen? It seems like we're talking orders of magnitude speed up compared to the pre-AI way of doing this. 


---


#### 5892.764

And how accurate is it? Yeah, I mean, RF diffusion, like I can generate a single backbone in a minute, even like a pretty big one, it just takes a minute to generate a backbone. And if you have a really good GPU, that's way faster,   
(5905.337) ~~right?~~ (5905.517)  
If I'm just working on my laptop or something, like I can generate something in just   
(5909.96) ~~like~~ (5910.1)  
a minute. And then ligand and PNN is significantly faster than that. So like designing the sequence for the 3D structure is actually really fast.   
(5917.624) ~~So, you know,~~(5918.825)  
like per protein, And like per sequence, it's less than a couple of minutes to do that whole thing. And so I can design like hundreds of thousands of backbones and then design hundreds of or thousands of sequences for each backbone with ligand and PNN. 


---


#### 5934.645

So it's pretty fast and pretty computationally efficient. And they've made some improvements to RF diffusion to reduce how many time steps you need to actually get a good structure out of it. And time again, when they actually synthesize these and check for   
(5947.788) ~~like~~ (5948.008)  
thermostability or specificity or binding affinity, very often they're very high. And if I have   
(5955.87) ~~like~~ (5955.99)  
low thermostability or low binding affinity or low specificity, very often when I use these models to improve that, they improve it dramatically. So they're pretty effective. And they're not perfect, but they're pretty good. It's not a hard thing to do to design a protein with RF diffusion and then design a sequence with ligand and pinin and get something that really does fold into that structure with high confidence or that really does interact with my target protein with high affinity and specificity. 


---


#### 5988.864

Yeah. So how does this then fit into the broader validation loop? You have this one thing, you're like, going back to our cancer example, right? Oh, this part of the cancer cell interacts with this part of the immune cell and disables it. So you want to put essentially a physical cap on that thing so that is blocked and that can't happen and the cancer can get Okay, cool. So I'm going to generate potentially thousands of shapes, thousands of sequences per shape, then potentially run millions of things through an alpha fold multimer, getting scores. And then what do I do at the end of that? Do I take like the top hundred and go actually try them in a living cell? 


---


#### 6033.444

Yeah, exactly. And so this seems, and you're saying they tend to work. And then I guess we also have questions of like side effects would be another big downstream question, right? We don't know what else this thing could do when put into the full environment of the cell.   
(6049.037) ~~Well,~~ (6049.117)  
that's where the specificity comes in, right? Generally speaking, RF diffusion is capable of designing binders, for example, with really high specificity. So they bind to the target and pretty much only bind to the target. Yeah, and it's a really good thing, right? Because if you design a binder that just interacts with a whole bunch of other stuff, it may never make it to the target. It may cause other side effects, like you're saying, have off-target effects. 


---


#### 6074.773

But yeah, RF diffusion is pretty capable of designing really high-specificity binders. The motif scaffolding, there's more nuance there because you're   
(6084.036) ~~kind of~~(6084.357)  
performing surgery on proteins and pieces of proteins. And so that can get a little more nuanced and a little more complicated. If you're just designing a binder with RF diffusion, it's pretty easy to design one that has really high specificity and that doesn't have a lot of off-target effects and stuff. So what's the bottleneck on this process? Is it identifying targets? Especially if you can design things that are that specific and they don't have much in the way of other knock-on effects.   
(6114.164) ~~I mean,~~(6114.344)  
it seems like we should be curing a lot of diseases pretty quick here. 


---


#### 6118.167

I think, I mean, diseases are pretty complicated and sometimes it's not just one thing that you're targeting. Sometimes it's multiple targets and multiple kinds of interactions. And so you have to think in terms of   
(6129.975) ~~like~~ (6130.196)  
entire   
(6130.876) ~~like~~ (6131.036)  
protein interaction networks or even like interaction networks that involve other molecules as well and modulating those in very specific ways. And often figuring out what parts of a protein interaction network to change or to modulate and how to do that, like what sort of changes you should make to this interaction network, that's a pretty complicated problem. And so I think part of it is   
(6155.455) ~~identifying, like you said,~~(6157.456)  
identifying targets or identifying specific targets within an interaction network, because some of the interaction networks can get really complicated. 


---


#### 6166.02

And figuring out which parts of them to modulate is not an easy thing to do. And then Computationally, there isn't much of a bottleneck. If you just have a good GPU, you don't really need multiple GPUs even. You just have a good H100 or something. You can get a lot done with that.   
(6183.258) ~~You can get quite a lot done with that~~(6184.939)  
with RF diffusion and NPNN. The hardware requirements are not very taxing.   
(6191.702) ~~I mean,~~(6191.882)  
They're probably a little less efficient than I would like them to be, because   
(6197.969) ~~I guess~~(6198.209)  
most average people are not going to have access to an H100. A lot of people are going to be using much lower tier GPUs and stuff. 


---


#### 6209.472

But RF to Fusion, for example, there's a Colab notebook that you can run on a T4. You can run it in Google Colab, and it takes a little while. It's not as fast. The computational bottleneck is not a huge bottleneck right now.   
(6223.364) ~~I think~~(6223.624)  
it could be a little better, but   
(6225.425) ~~I mean,~~(6225.626)  
the models aren't huge models. These aren't like billions of parameters, right?   
(6230.409) ~~I think~~(6230.649)  
RF Fusion has a couple hundred million parameters or something like that. Or in AlphaFold, same thing,   
(6237.013) ~~like~~ (6237.193)  
it's a couple hundred million parameters or something. So they're not really big models that require really excessive hardware to do the computations. And   
(6245.798) ~~I think~~(6246.039)  
the slowest part of that pipeline, you like design binders or design motif scaffold with RF diffusion or partial diffusion or what have you, and then designing a sequence with   
(6257.519) ~~like~~ (6257.639)  
protein NPNN or ligand NPNN, and then validating with   
(6261.04) ~~like~~ (6261.16)  
alpha fold or alpha fold multimer, the slowest part in that whole thing is actually the alpha fold multimer part or the alpha fold two part where you're validating and   
(6270.824) ~~like~~ (6270.964)  
predicting the structure of whatever you've generated and designed with the other two models. 


---


#### 6277.234

That's actually the slowest part in the whole thing. If you're able to predict a lot of structures with AlphaFold, then you're fine. There's no real computational bottleneck there. And as far as   
(6288.736) ~~like,~~ (6288.956)  
why are we not curing a bunch of diseases? A lot of this also has to do with how long it takes to get these things to market. and the traditional system that's set up right now for drug discovery and protein therapeutic, it's hard and slow to get new things through.   
(6308.685) ~~Like it's a~~(6309.225)  
very slow system. And   
(6310.806) ~~I think~~(6311.126)  
it wasn't designed for high throughput methods like this. It wasn't designed for   
(6317.829) ~~like~~ (6317.989)  
large high throughput methods. And it just, it takes a lot of time to get a new drug or a new protein therapeutic through and approved and get it through all the testing, like the different clinical testing phases and stuff like that. 


---


#### 6332.917

That's part of it. that's probably a big part of it. Are we like stuffing the pipeline at this point with new things?   
(6339.485) ~~I mean,~~(6339.645)  
it seems like the biggest reason that this used to be a hard thing, of course, it's like slow and there's a lot of like safety, perhaps redundant steps in there, especially if you could say, hey, we have like very high confidence that this is a highly specific thing.   
(6354.194) ~~I mean,~~(6354.334)  
that would really do a lot to inform   
(6357.656) ~~the~~ (6357.816)  
what the safety profile might be. But even if you, not even if, but in the past, it's like the biggest problem was like either it wouldn't work, right? Or it would have side effects that were like intolerable. 


---


#### 6370.411

And if you could take both of those things, not entirely off the table, but if you could   
(6374.232) ~~sort of~~(6374.473)  
say, hey, we can be much more confident now, seemingly like at least in order of magnitude, more confident that any given thing is going to do what you expect it to do and that it won't do other things that you don't want it to do. you can improve both of those by an order of magnitude, then it's your seemingly two orders of magnitude more likely for things to work, which would take you from sub 1% a lot of shooting in the dark to a lot of the clinical trials would be expected to work. Is that the era that we're entering into now where clinical trials should go from roll the dice to you be more like disappointed when they don't work? 


---


#### 6415.494

Yeah, I mean, I think we're definitely moving into an era where all this stuff is going to speed up a lot. And   
(6421.216) ~~I think~~(6421.557)  
so there are   
(6422.757) ~~like~~ (6422.937)  
a lot of situations where you want to understand more than just a static structure. Like we've been talking about, like having models that give you more dynamic information and stuff like that. And those are so recent that they haven't really been adopted by a lot of people. yet. And I think once those get used more, that'll speed things up a lot and improve things a lot as well. But yeah, I think also part of it is just adoption. A lot of researchers are not using this stuff yet because it's so new. 


---


#### 6452.934

And a lot of researchers don't understand how to use these models effectively or how to use them at all. It does seem to be quite a different skill set.   
(6460.976) ~~I mean,~~(6461.336)  
I've actually studied chemistry. It really is. Yeah. And the kinds of things that I was taught to do were like not at all running the loops. There were no notebooks involved or no collab notebooks involved. It was like physical techniques for separating chemicals from one another was a big part of where the time went. Yeah. And that's a whole other thing too, like drug synthesis and small molecules is like a whole other story that we can get into. But because there are like really interesting diffusion models out for those as well that'll generate molecules with specific properties. 


---


#### 6493.989

But Yeah, I mean, it's a very new and a very unique skill set that there aren't a lot of people that are training people to do this. There isn't a ton of information out there about how to use them.   
(6506.56) ~~You,~~ (6506.62)  
to some degree,   
(6508.341) ~~I mean, there,~~(6508.681)  
there are some platforms that are popping up and some different tools that are popping up that are making these things a lot more accessible. One that I would mention is 310AI is working on a tool that they're calling Copilot. And   
(6523.564) ~~it's essentially,~~(6524.485)  
it's like a chat interface that uses tools. So you can talk to it in natural language, like you talk to a chat GPT or something. And then   
(6535.71) ~~it,~~ (6535.75)  
it knows how to use   
(6537.331) ~~like,~~ (6537.551)  
like function calling   
(6539.712) ~~to,~~ (6540.152)  
to use other models as tools. 


---


#### 6543.594

So you can say, generate a protein with such and such property, and then it'll use a particular model to do that, generate some protein with that particular property. And then you can say,   
(6554.357) ~~like,~~ (6554.497)  
increase binding affinity with such and such protein, and it'll modify your protein for you to increase the binding affinity or something. Or you can say, dock this small molecule to this protein, and it'll call on diff dock and dock the small molecule to the protein for you and then return that. And that's all using like a chat interface, which is making a bunch of these models a lot more accessible to people. And I think that's going to have a huge impact in the near future. 


---


#### 6581.513

So. Depending on how good that gets and how fast it gets really good, that's probably going to change things substantially. And right now, it's pretty good already. And it uses a pretty wide range of tools for different things. It'll use protein MPNN or ligand MPNN to design sequences for a structure.   
(6602.898) ~~I'm not sure if it uses RFDiffusion yet, but~~(6605.699)  
they probably are going to start including RFDiffusion and some other models as tools for it as well. Because they just keep adding more tools to it, more models that it uses as tools. And I think once they have a good   
(6618.505) ~~section or a good~~(6619.545)  
selection of tools for it to use, that'll be really good. And that'll lower the barrier to entry for a lot of people. 


---


#### 6627.253

Because right now you've got to go through this like somewhat complicated process of setting up these models. And   
(6633.858) ~~you have to know,~~(6634.618)  
you don't have to know a lot of coding, but you do have to code some and you have to understand how to set these things up   
(6641.623) ~~in,~~ (6641.723)  
in   
(6642.183) ~~like~~ (6642.303)  
a conda environment or something like that a lot of times. And so if you're not coming from   
(6646.826) ~~like~~ (6646.966)  
a programming background or you don't have some experience with programming, like a lot of these models are   
(6653.231) ~~kind of~~(6653.491)  
hard to touch. They're hard to use because   
(6656.033) ~~you.~~ (6656.093)  
You can't really use them unless you know a little bit of coding at least. But so 310AI, I think is going to change a lot of that and make a lot of these models a lot more accessible over time and really increase adoption of these techniques. 


---


#### 6668.775

And I think that's going to be really big and important because adoption right now is pretty limited,   
(6674.32) ~~I would say.~~(6674.82)  
  
(6674.96) ~~I mean,~~(6675.161)  
just using a really simple metric by if you just look at   
(6679.664) ~~like~~ (6679.824)  
how many views a YouTube video on RF diffusion gets. It's not that many,   
(6684.946) ~~right?~~ (6685.146)  
There aren't that many people watching. This is going to be the one that goes viral and changes it all. I hope so. That would be great because adoption is going to be big.   
(6693.693) ~~I think~~(6693.973)  
because the more creative people you get using these things, the more you're going to see creative uses of them and   
(6700.678) ~~like~~ (6700.878)  
novel approaches to solving problems that people weren't even thinking of before. 


---


#### 6706.082

Like when have you been able to design proteins that build out complicated protein interaction networks using binder design and motif scaffolding. That's just so brand new within the last couple of years that the adoption just hasn't caught on yet. So hopefully more people will start experimenting with these models and really learn how to use them well. And we'll see a lot of really interesting novel techniques popping up in the near future. Yeah, that's pretty remarkable. So it seems like the problem then shifts to the, or maybe it was always there in the first place, but If it is the case that given a target, we can pretty reliably and even relatively computationally efficiently come up with something that will hit the target, not hit other things, not cause a lot of collateral damage. 


---


#### 6757.919

Now it's like target identification becomes the thing that really matters the most. And this seems like it's happening in a lot of areas at once. Certainly,   
(6766.365) ~~I mean,~~(6766.765)  
terrible analogy, but to thinking about a military environment, we've got really good missiles that can hit very precise targets, but then the targeting obviously becomes the high stakes decision. And   
(6779.394) ~~I mean,~~(6779.635)  
in lots of just business operations context too, right? Figuring out the right thing to do is often the hard part. So what do you think are the prospects for that sort of thing? I've been   
(6790.322) ~~kind of~~(6790.543)  
working through this and thinking, we've got quite a tech stack for... Obviously we can sequence lots of DNA. We can also pull out from an individual cell now what was the state of the transcriptome, what genes were being expressed at any given time, what proteins were being created. 


---


#### 6811.26

I don't know quite the degree to which we can do that with small molecules with a really localized sample. but it seems like we've got like a lot of ability to generate a lot of data and to probably then create a foundation model of some sort. This is   
(6829.204) ~~kind of~~(6829.384)  
where Evo I sort of sense is going, even though that's not even doing all this stuff yet, but already,   
(6835.728) ~~I mean,~~(6836.889)  
let me just give my understanding of Evo and you can correct me if I'm wrong, but basically they're training a language model on DNA sequences purely bacteria and phage DNA from what I understand. Yeah, I was a little disappointed by that, but I think part of their reason for doing such a specific selection was for safety reasons. 


---


#### 6861.442

I think they're trying to be a little cautious about what they train on and what the model is capable of doing for safety reasons. But I was a little disappointed that they only trained on that data, for sure. Hopefully there'll be another version at some point that's train on other data as well, but yeah. I'm sure there's a lot more to come.   
(6881.039) ~~You kind of glitched on me for a second, but~~(6882.64)  
so they train on all this data. Now they can generate sequences in the same way that a language model can generate text, right? Then autoregressive, byte by byte, base pair by base pair generation. And then there's these really interesting things that they can do downstream of it where, for example, a gene essentiality score or test Basically, if you change a sequence in a particular gene and generate from that changed sequence it seems that the model has developed a sort of, as we've talked about a couple of different contexts, this sort of higher order understanding of how things fit together, such that if you do make a change to something that really matters, then you see sort of an unraveling of the later generation. 


---


#### 6937.242

Like you see a very high perplexity downstream of this changed sequence. And that reflects the fact that, hey, if you've changed that sequence, I can't really make any confident predictions now because we're   
(6950.27) ~~sort of~~(6950.611)  
outside of the set of things that can work. And so once you change that, it's all kind of noise. Whereas if you change something and predictions remain confident downstream, then you infer that must not have been super important. That was an area that more easily could be, change could be tolerated in that particular sequence because, and we can infer that from the fact that it continues to make confident predictions downstream. That's pretty remarkable stuff that suggests to me that especially as we scale up the data set a lot more, which in this one was 300 billion. 


---


#### 6987.959

I mean, that's not nothing, but it's not much compared to what we could easily imagine doing. Certainly not much compared to the 15 trillion tokens that Mediterranean Plasma 3 on, but then also like more modalities, right?   
(6998.604) ~~I mean,~~(6998.724)  
we're seeing this in the language models where you can have obviously language integrated with image and plenty of other things. Audio now fits into Gemini 2. It seems like you sort of imagine from just the DNA to   
(7011.49) ~~sort of~~(7011.811)  
the DNA and maybe the transcriptome or the proteome or whatever the sort of state of a cell is. You can even imagine scaling this up another degree to   
(7022.489) ~~sort of~~(7022.71)  
the systems level too. But to learn to predict the next state from the current state seems like we're getting really close to being able to do that. 


---


#### 7035.193

I would kind of expect that in the next couple of years at most, we would start to see large scale foundation models for biology that would predict like how a cell will evolve through time, how a system level description will evolve through time. And then you can start to do these counterfactual hypothetical perturbations and see, okay, if we change this, then how will that make things evolve? If we change this, how will that make things evolve? And so then I guess what we would expect to be learned by those systems is what is now the black box, right? Of all these interactions that we have only mapped out, whatever, 5% of. And then you could even imagine a situation where you start to do interpretability techniques on digital neural networks to then figure out what the actual pattern of interactions is in the actual biological systems. 


---


#### 7088.935

So is that where this is going over the next couple of years?   
(7091.756) ~~I mean,~~(7091.956)  
and then it seems like if we can achieve that, then you   
(7094.777) ~~kind of~~(7094.997)  
have a fairly closed loop of, okay, we can now identify good targets at a pretty high rate. We can identify or design interventions that are pretty likely to be successful. The like specificity is already high.   
(7110.225) ~~I mean, it's~~(7111.166)  
we're entering into   
(7111.866) ~~sort of~~(7112.146)  
a super steep part of the S-curve in terms of not just   
(7116.429) ~~like~~ (7116.589)  
understanding biological systems, but really being able to intervene in them. And it just seems like a totally different regime that we're headed for. So is that what you basically expect to see over the next couple of years? 


---


#### 7127.396

I mean, I hope so. I hope that all of that comes to reality or comes into existence. Sorry, We pause for a second. I need to get some water. OK, hold on just a second. We're back. OK,   
(7137.954) ~~I think we're~~(7138.335)  
I think we're all set. Yeah. OK, I'm feeling a little better now. So where were we?   
(7143.784) ~~What were we talking about?~~(7144.685)  
You were hoping that my seemingly I'm like extrapolating from where we are and I'm also sort of mapping what has happened with language model foundation models onto the biological domain and feeling like it's about to get crazy. So you're hoping that happens.   
(7162.602) ~~I, yeah. I mean,~~(7164.042)  
I think it's about to get crazy for sure. 


---


#### 7166.283

I think like we're fast approaching a scenario where all of these technologies are going to kind of converge and we're going to have a lot of power over. editing and modifying our biology. And I think that's a very exciting thing because there's a lot of problems that I really want to see solved in my lifetime. And I think we are definitely moving in the right direction. And I think we are fast approaching a situation where we can actually solve a lot of these problems. And   
(7193.391) ~~I think,~~(7194.032)  
so like the main thing that you're talking about is   
(7196.952) ~~like~~ (7197.112)  
this complicated sort of hierarchical structure that's happening. And the level that I think at most of the time is at the level of like molecule interactions. 


---


#### 7210.913

But you can definitely take that up another level and look at how those interactions come together in a network to create a particular sort of   
(7223.217) ~~like~~ (7223.398)  
phenotype or to create a particular sort of state of the organism, right? And   
(7229.139) ~~like~~ (7229.3)  
some of those states are diseased states that we don't want. Figuring out,   
(7235.117) ~~like,~~ (7235.357)  
how to modify these interaction networks,   
(7239.219) ~~I think,~~(7239.579)  
is somewhere that we really need to focus on a lot. And one thing that's really useful and that I really want to see pushed further is this notion of LIS score with alpha fold multimer and seeing also,   
(7253.525) ~~like,~~ (7253.665)  
things like alpha flow or distributional graph former generalized to complexes, to,   
(7260.168) ~~like,~~ (7260.308)  
complicated complexes of molecules and not just one or two proteins or something. 


---


#### 7266.259

I really want to see more progress happen there because once we understand all of the interaction networks and we're able to modulate them in very specific ways,   
(7276.524) ~~we're going to solve a lot of problems,~~(7278.645)  
a substantial amount of problems. Modeling these interaction networks is becoming possible now.   
(7284.448) ~~I think~~(7286.149)  
before alpha-fold multimer, And before some of these other docking methods, and before RosettaFoldAllAtom came out, we really didn't have the tools to model all of these different interactions. But we have very recently just hit a point where we do have most of the tools that we need, if not all of them, to model all of these interactions. And once we implement something like alpha flow or distributional graph form for complicated complexes of molecules, that's really going to be pretty substantial. 


---


#### 7320.29

And I personally, I'm not sure how I would approach the problem of determining what specific interactions or interaction networks to modulate.   
(7334.181) ~~Like, I personally, like,~~(7335.521)  
that feels like such a big problem to me. But I also know that there are a lot of biologists that know specific interaction networks they want to modulate, and they want to modulate them in very specific ways. And there's a lot of that. And now we can do that.   
(7352.266) ~~I think~~(7352.546)  
we just need to get these tools into the hands of those biologists and make them really accessible. Because they're not super accessible yet.   
(7364.195) ~~They are kind of, right? I mean, like~~(7366.116)  
a lot of them are open source and they're out there and you can get the model weights and a lot of them have the training code and the inference code and all this stuff available. 


---


#### 7375.664

But probably your average biologist is not going to know how to use those tools right now. So making them accessible and easy to use is really where a lot of the work is going to be as well. Because there are a lot of people that want to do these things, but   
(7393.197) ~~they don't~~(7393.737)  
they haven't quite gotten to the point where they've adopted all of these tools yet. And also figuring out how to use them all in tandem with each other, right? Because you don't want to just use one of these models. You want to use multiple and use them all together to solve a problem. And so that requires you to learn   
(7414.69) ~~like~~ (7414.83)  
multiple different models and how they work and how to use each one of them. 


---


#### 7419.413

And that's not an easy thing to do for a lot of people. Yeah.   
(7422.055) ~~The, I mean,~~(7422.495)  
this is the issue in AI, even in much more,   
(7425.417) ~~you know,~~(7425.777)  
simple use cases of just using change UPT effectively the sort of diffuse, the technology diffusion through society   
(7432.061) ~~is,~~ (7432.201)  
is really the big bottleneck   
(7433.782) ~~I would say~~(7434.142)  
right now to when people say   
(7436.144) ~~like,~~ (7436.224)  
why hasn't, if change UPT is so great,   
(7438.025) ~~like~~ (7438.145)  
why hasn't it,   
(7438.925) ~~you know,~~(7439.186)  
changed productivity all that much? It's like, people are not using it nearly as much as they could is one really big reason. So a huge reason. Yeah. If I had to   
(7446.57) ~~kind of~~(7446.79)  
map out the story of the next couple of years as I understand it, or as I'm   
(7450.753) ~~kind of~~(7450.913)  
piecing it together from everything that you're teaching me about, it is right now we have a big backlog of targets and we have a pretty robust new set of tools that used together can design things that will hit those targets and not create too much collateral damage such that it's not super hard. 


---


#### 7480.585

It's hard to learn to use the tools, but once you have the skill set, it becomes relatively easy to take a target and crunch through a bunch of iterations and come to a bunch of candidates. And those are likely enough to work that we should start to see serious acceleration of the ability to find the solutions to these well-posed problems. And then   
(7508.012) ~~sort of~~(7508.532)  
in parallel, we should probably also expect that Evo 5 or whatever, Evo 4 will be capable of dramatically better holistic modeling of the overall networks. And that will then, once we   
(7527.56) ~~sort of~~(7527.84)  
deplete the current set of targets, that have been painstakingly worked out through non AI methods   
(7537.472) ~~sort of~~(7537.733)  
seems, 


---


#### 7538.073

I don't know. Why does it always seem like it happens at the same time? It's always these sort of gradual overlapping curves, but my gut says we've got a few years in front of us of. depleting the current, or not depleting, but like picking the sort of low hanging fruit of, hey, we've got all these targets out there and now we've got good methods to hit those targets. That's going to take a while for people to learn the tools, do it, obviously validate it, run clinical trials going in lots of different areas. And then as the sort of current backlog gets worked through, it's probably a better way to phrase it. Right around the same time, 


---


#### 7569.768

I sort of expect that all of a sudden the tension will turn to, Oh my God, now we have these foundation models that kind of model the whole causal graph in all of its crazy complexity. And now we're actually going one level out and saying, now we can apply similar computational techniques to the identification of the targets. And we'll do that in   
(7593.943) ~~sort of~~(7594.144)  
a similar way of being like, okay, I want   
(7597.146) ~~this, this is~~(7597.907)  
what's happening and I want to prevent it from happening. or this is what I want to happen proactively that isn't currently happening. Let me just   
(7605.834) ~~kind of~~(7606.034)  
brute force my way through a bunch of perturbations to the, and of course we can get better than brute force too, but even just imagining   
(7613.922) ~~a sort of~~(7614.483)  
several couple generations down of Evo, it seems like make a tweak, see what happens is going to be so radically accessible from a computational perspective that will then also just have this explosion of like quality targets to identify. 


---


#### 7629.012

And yeah,   
(7630.573) ~~I mean,~~(7630.773)  
what do you think the world looks like as all that happens?   
(7634.116) ~~What is,~~(7634.416)  
it seems like we may be not super far from a,   
(7639.479) ~~this is not, we're not even in a world here of like an,~~(7641.32)  
any sort of AGI,   
(7642.501) ~~right?~~ (7642.661)  
We're talking like, these are still tool simulated simulation and tool type things that people would be using that we're not assuming anything here about AI agents doing the work. Although you did have a little bit of that with the 310 co-pilot. but is there anything that I should be like reigning in my expectations on?   
(7662.28) ~~I mean,~~(7662.5)  
are there things about like one tweet that I sent you was around to what degree can these things handle sort of point mutations or whatever? 


---


#### 7669.724

And there's maybe individual idiosyncrasy becomes a really hard problem at some point, but like how far does this paradigm that I'm sketching out extend, do you think? And what limits does it hit? Yeah,   
(7681.892) ~~so I think,~~(7682.332)  
so just briefly on   
(7684.553) ~~like~~ (7684.713)  
point mutations or like more complicated mutations where you mutate multiple things and just predicting how positive or deleterious that mutation or set of mutations might be on the protein or something. That's a capability that ESM has, and that's already two or three years old at this point. And Evo does it. They got state-of-the-art performance with Evo on predicting which mutations were positive and which mutations were negative and which sets of mutations were positive or negative. 


---


#### 7720.012

And you can compute a few different things, a few different kinds of scores that tell you about this. you can actually build out evolutionary trajectories to show over time how things are likely to evolve based on how positive or negative the impact of a mutation is on protein or something or DNA sequence or whatever. And Evo, they got state-of-the-art performance on this. And that's actually, they also did this with alpha folds.   
(7748.132) ~~I think~~(7748.353)  
they called it alpha missense or something like that, where   
(7751.714) ~~they just, I think they, what did they do it for?~~(7754.015)  
Did they do it for   
(7755.165) ~~I think they did it for~~(7755.986)  
all the proteins, all the human proteins, but maybe it was a bigger dataset. 


---


#### 7760.453

I can't remember. But they predicted all the single point mutations and all the effects   
(7763.779) ~~that~~ (7763.859)  
that those have. And that's actually not a hard thing to do. So mapping out how a mutation affects a protein or DNA or something, and the course of evolution that's likely to occur, that's actually pretty easy to do now. And then as far as... I also want to draw attention to another project that I'm aware of. It's not a model per se, but   
(7786.514) ~~they are using... I think~~(7788.096)  
they are using GPT-4 They may have trained their own in-house model. I'm not sure. But there's a company called Future House, and they're designing an agent, an autonomous agent, that will do a lot of this research for you. 


---


#### 7805.835

And it'll do things like literature search and review, and come up with hypotheses of different kinds of interaction networks that you might want to modulate or different targets that you might want.   
(7819.246) ~~And it'll do this and it'll do it pretty well.~~(7822.127)  
And that's a pretty new thing that just started happening   
(7826.828) ~~like~~ (7826.988)  
last year,   
(7828.248) ~~I think,~~(7828.888)  
maybe late last year. And they're getting pretty good results with that. And that's actually using an LLM like as the base, right, to build an agent to do this research. And then   
(7841.195) ~~I think~~(7841.515)  
they're also building an autonomous lab that drives itself. So once the agent comes up with hypotheses or targets or what have you, the lab is autonomous as well. 


---


#### 7854.241

And that's a pretty exciting direction. I think that, coupled with some of these more specific tools to perform these fine-grained operations on proteins and small molecules and DNA and RNA. When those two   
(7869.75) ~~kind of~~(7870.051)  
converge, that's going to be a really big deal. And I see that happening in the next year. The progress that they're making at future houses is really impressive,   
(7881.076) ~~I think.~~(7881.416)  
So that would also be something that people should definitely look into. And I think your timeline is within a couple of years for sure. I don't think it's going to be that long before we start seeing substantial progress and changes.   
(7894.713) ~~I mean,~~(7894.953)  
OpenAI just partnered with Moderna, right? Yeah. Hundreds of GPTs. 


---


#### 7899.656

I'm sure that's just the beginning. And   
(7901.578) ~~I think~~(7901.858)  
that also is like a paradigm that's going to match well with these other more specific tools, because when you enable an agent to use tools, you unlock a lot of possibilities, right? When you enable something that can review thousands of research articles, then develop targets or hypotheses to test, and then can call on these specific tools to design molecules or proteins or nucleic acids to perform these specific functions or hit these specific targets. That's going to move really fast. And   
(7940.989) ~~I think~~(7941.269)  
I'm excited. I'm also a little nervous because I think there's a lot of a lot of potential for misuse in the wrong hands. The sort of things that you can accomplish will be amazing and beautiful. 


---


#### 7956.602

And we're going to see a lot of health problems just disappearing. We're going to see lifespan extended. And that's going to   
(7963.528) ~~really increase or~~(7964.749)  
really improve the quality of life for everyone. But also, we do have bad actors in the world. And that is something I worry about for sure, because in the wrong hands, we could be looking at very dangerous things as well. And so having some kind of oversight for these things is very important. Because,   
(7982.527) ~~I mean,~~(7982.767)  
we're looking at moving into an age where you could target a specific group of people based on their genetics or something. That's both immensely useful and also very dangerous. I have a lot of faith in the people that are working on these things, like the people that are building these models and doing this research are really good people with a lot of really good intentions and a lot of know-how and experience. 


---


#### 8009.033

And that to me is very reassuring, but there's always some random jerk that has the potential to mess it up for everyone. We have to be prepared for that. Yeah, no doubt. Preparing for this, definitely one of the major updates that I've made is that when people talk about the bio risks from AI, the conversation that I've heard most of has been like, how does it compare to Google? How does GPD 4 compare to Google? Does it make it easier for you to get certain information or figure out how to do certain things. And in familiarizing myself to the degree that I have with all this technology, it's   
(8052.765) ~~like,~~ (8052.965)  
that all of a sudden feels very quaint already. 


---


#### 8055.908

It's like, this is not a question of comparing to Google. This is like generating entirely new stuff. And I looked back not long ago at the list of mass extinctions in the history of the planet and what caused them. Of course, some were caused by totally exogenous shocks, like an asteroid hits the Earth. But the first one on the list on Wikipedia is the oxygenation of the atmosphere. And it's simply that something   
(8087.875) ~~kind of~~(8088.235)  
pops up and either itself, nobody knows how to eat, or it creates some waste product that,   
(8096.981) ~~you know,~~(8097.241)  
that nobody's prepared to deal with. And what we now breathe and depend on was at one point, the cause of a mass extinction event. 


---


#### 8107.008

I kind of try to keep these like zeroed out perspectives in mind. And it does seem,   
(8111.291) ~~I mean,~~(8111.611)  
tell me if you think there's any limitation to this or whatever, but with this sort of brute force search through   
(8118.855) ~~sort of~~(8119.095)  
biological space, right? It seems like there's not really anything conceptual that I could identify preventing, talk about gain of function type research. on a totally different level. Things that nothing can eat. That's like the most dangerous stuff, right? It's the stuff that nobody can break down. And I gather that trees were essentially at one point that too, right? Before something developed that could break down the hard fibers. tissue of a tree, it was just piling up. 


---


#### 8152.716

Globally, I understand that's basically where a lot of coal came from, is that trees would fall, nothing could digest them, and so they would just   
(8160.082) ~~sort of~~(8160.342)  
collect and eventually they turn into coal. I'm sure there's a lot of different stories of coal formation, but these moments of something that nothing is really prepared to deal with, those seem like the really dangerous things. And I don't know how you prepare yourself for that. I think there are multiple things that we can do to help   
(8177.755) ~~prevent~~ (8178.176)  
prevent some of these bad things from happening. And I think we're going to need to rely on the models that we build, especially the agentic models that we build, to help guide us in some of this. 


---


#### 8191.383

Because at some point in the near future, we're going to have agents based on really robust language models or something similar, and they're going to be able to review thousands of research papers and do tests in a lab on things, take in an amount of data that we can't really take in, right? That no human or even group of humans can really take in and process and digest and use.   
(8220.88) ~~Like~~ (8221.12)  
the scale is going to be much larger than a human can really work with. And so we're going to have to rely on some of our models to help guide us. And also,   
(8234.045) ~~Like,~~ (8234.205)  
going back to how does it compare to Google, I think another argument that could be made for why not to worry about some of these things is, okay, maybe I can get on my computer and design some new thing that was really toxic or something, but I still have to go into a lab and synthesize all that stuff. 


---


#### 8255.679

And a lot of that part of the process is very highly regulated and watched, right? I can't just go get a bunch of random chemicals and build this stuff in my house, right?   
(8267.122) ~~Like~~ (8267.282)  
it's harder to do than that. And like synthesizing proteins is, it's a non-trivial process. So   
(8274.206) ~~like~~ (8274.366)  
a lot of the worry, I think of, Oh God, we're going to have an AI that designs a deadly virus or a bioweapon or something. A lot of that is really overblown, especially at the moment. And I think a lot of people overlook the fact that computationally designing something computationally designing a molecule is just one step in the process. You also have to do all the lab work and synthesis and work on some kind of delivery mechanism. 


---


#### 8303.901

And this is all stuff that's non-trivial to do and that helps prevent bad actors from actually going through with some of this stuff. Now there may be like state-sponsored bad actors with access to good labs and lab equipment that will circumvent a lot of that. But when you're working at a state-sponsored level, that's a matter of international relations and also national security. I think that has almost nothing to do with AI. The computational design of some random toxic molecule is just one step in a complicated process. People don't often think of that. I see a lot of very influential, big name people in the industry who are coming from the NLP side of things and the LLM side of things. 


---


#### 8360.571

They don't really understand the biology and the process that goes into actually making these things. I think their worry is justified, but they're also not understanding the nuances and where the dangers actually are. So   
(8376.373) ~~I think~~(8376.593)  
it's important for people to keep that in mind. I think it's very important before we start getting all anxious and worried about some random person using Lama 3 to design a superflu or something, you have to remember it's very unlikely and very difficult for just a random average person to go through the entire process of designing and synthesizing and delivering some kind of toxic molecule. That's a long, difficult process that an individual would be very unlikely to be able to accomplish, even with the help of a very intelligent LLM or a very capable agent. 


---


#### 8416.517

Now, when you have larger research-oriented companies working on these things that have their own wet labs, and they're building agents to run these wet labs and to computationally design the molecules and form plans on how to use them. There, I can see, okay, we need some kind of oversight. We need some people working on how to make sure that process is safe, how to protect that information and data and equipment,   
(8449.217) ~~right?~~ (8449.477)  
Because there are plenty of situations where something like corporate espionage is happening and people are trying to do nefarious things with some of the technology that some of these companies have. But again, that has very little to do with the AI itself and has more to do with how we're interacting with other countries and other research organizations. 


---


#### 8474.266

So definitely we need to be developing plans for how to use and regulate and oversee a really capable agent that is going to go through the entire process of computationally designing and verifying and then also synthesizing and delivering. And that is technology that is in existence now. We already have agents that are doing most of this process. And a lot of people are pushing for more of that, which I agree with, because we're not going to be able to solve these problems on our own. We're going to need some kind of really capable agent that can help guide us through these processes, because they're so complicated. and so difficult to understand the whole picture and all of its nuances that I don't know if humans can get there without some kind of agent helping out and helping design the molecules and producing it and delivering it and etc. 


---


#### 8532.78

I don't know if we can get there without that, but I guess my concern is just making sure that these companies and organizations that are building this technology and using it have some people that are overseeing the safety side of things and that are concerned with red teaming and preventing things like corporate espionage and making sure that everyone that's using that technology is using it responsibly and making sure   
(8557.902) ~~that we're like~~(8558.562)  
that the companies are hiring not just capable people but also   
(8563.565) ~~like~~ (8563.705)  
people with good moral grounding and good intentions. Yeah I guess   
(8569.349) ~~that's where I mean~~(8570.53)  
that's not even the future that's   
(8571.971) ~~kind of~~(8572.231)  
now, That's already a concern that we need to address now, because we already have agents that are doing these things. 


---


#### 8579.192

Most people don't have access to them, though. Most people don't have access to a really capable agent that can do this whole process or do most of this process. That's not something that even most companies have access to, much less individuals, because a lot of these models are closed. I could see maybe some kind of   
(8599.482) ~~like~~ (8599.682)  
state-sponsored group of researchers could use open source models to build something similar and do something nefarious, but that's a whole,   
(8608.084) ~~like,~~ (8608.304)  
it's a very complicated process of building such a thing. And I don't know if I have a good answer for how to combat something like that or how to address something like that. I don't know if there's a good answer. to that right now. 


---


#### 8621.289

It's certainly hard to identify a more important question.   
(8623.83) ~~Do you think that the,~~(8624.611)  
do we have any read on whether offense or defense is favored here, so to speak? In the sense of for nuclear weapons, for example, if one of the major nuclear powers fires all its missiles, nobody can shoot all those missiles down. It seems to me that is an offense favored regime. And so we're   
(8643.138) ~~kind of~~(8643.378)  
stuck in this   
(8644.419) ~~like~~ (8644.639)  
mutually assured destruction paradigm, which is yikes. We   
(8649.622) ~~kind of~~(8649.862)  
need to get to a different paradigm because we're under real threat of nuclear catastrophe as long as we've all got thousands of missiles pointed at each other and no viable defense. I don't have an intuition for if biology works the same way or not. 


---


#### 8667.813

I think this is less of a question about biology and more of a question about cybersecurity because I think it's like very similar in spirit to like cyber security and there as well most often the attacker has the advantage over the defender but there are a couple of things that may change that one is really capable agents because if you have a really capable agent that's able to defend against human attacks that are   
(8696.25) ~~like~~ (8696.41)  
just inferior that's going to be a really big part of protecting against bad actors and so   
(8703.175) ~~i guess like~~(8703.655)  
That's an argument for acceleration, actually, because if you have the most capable agent, then probably your defense is going to be a lot better than everyone else's. 


---


#### 8713.738

And if your agent is capable enough, it may be effective enough to ward off pretty much anything. And I don't know how soon that's going to come into the picture, but I think that is a good argument for keeping up the pace of development of LLMs and agents and things like that. There was another point that I wanted to touch on, and   
(8733.407) ~~I think~~(8733.588)  
I forgot. I already forgot what it was, though. Anyway, yeah, I think the advantage of the attacker over the defender may end up shifting because of agents. We may end up having a situation where that's no longer the case. And, yeah. I'm a little confused about why are you making a... 


---


#### 8752.232

Why is the shift from biology to cybersecurity? Because I'm envisioning a world where For example, Evo is open source, Llamo 3 is open source. If Evo 3 is open source, then we start to, at some point, we enter into a regime where, yeah, it may not be easy. It may be hard for one person. but at some point it does get like lower than state actor level where somebody could launch some crazy attack and then it's okay. If you create some super bug with certain properties, can we defend against it?   
(8788.22) ~~I'm a little bit unclear as to how you're,~~(8790.221)  
I'm not sure if you're like equating that to cybersecurity or saying that's primary somehow. No, 


---


#### 8795.084

I guess, no, I think that's a good point. Yeah. Because if you develop some kind of,   
(8799.367) ~~I think,~~(8799.667)  
I guess a virus is probably as good an example as any, but let's say you develop a virus of some kind that targets a specific population. Developing a cure for that traditionally has been a very slow process. And like the fastest that we've ever done it was probably COVID. And that still took some time, right? And on the other hand, there is recent work that came out of, it was the University of California, but I'm not sure which one. They recently published some research about   
(8830.069) ~~like~~ (8830.229)  
universal vaccines. And they're able to design a vaccine that was like applicable to a wide range of mutants of a virus. 


---


#### 8838.817

#### 8881.857

That's definitely a very good data point.   
(8885.138) ~~I mean,~~(8885.338)  
my kind of default would be just to think I have three kids and I'm no expert in how babies develop in the womb, but it's definitely clear that a lot of things have to go right. Like an unbelievable number of things have to go right in the proper sequence. At any point, if something goes wrong, like that could be the end of it. My general default model would be like, a lot of things have to go right and only   
(8911.75) ~~kind of~~(8911.97)  
one or two big things would have to go wrong. And so it seems like there's a lot of surface area to defend and a lot of kind of places that could be attacked. 


---


#### 8922.301

But then, hey, if you can make a universal vaccine, then all of a sudden that does start to look quite a bit different.   
(8929.668) ~~So yeah, boy.~~(8931.169)  
Yeah.   
(8931.449) ~~I mean, it's,~~(8931.749)  
and I think you're right also to say a big part of this does seem to be   
(8934.872) ~~sort of~~(8935.152)  
what is the prevailing,   
(8937.374) ~~like~~ (8937.555)  
international relations regime, because if it seems like pretty safe to say, if we get into a bioweapons arms race, we're going to be in bad shape. we really have to have some more globally cooperative approach. Or the missiles have one really nice property, which is they don't spontaneously escape their silos and self-replicate around the world. Whereas the list of lab leaks is quite long. 


---


#### 8969.396

It just seems like there's no way that we can get into an international bioweapons arms race and survive it. We just have to avoid that trap in the first place. I hope we do. What happens when you develop cures for a wide range of diseases and you're able to extend human lifespan significantly longer than what it is now and eliminate a lot of the diseases that we face? Once that exists,   
(8998.86) ~~I don't know,~~(8999.3)  
maybe that's a paradigm shift.   
(9001.042) ~~Maybe that's a,~~(9001.883)  
that's like a shift in human consciousness at that point. And we start thinking about things very differently because we're all used to thinking about   
(9009.91) ~~like~~ (9010.13)  
everything in terms of being finite. And   
(9014.093) ~~I think having,~~(9015.594)  
having an approach or thinking about things in a way that isn't finite anymore and thinking about things in terms of how valuable our health and our life is because of the fact that enables us to be with who we love for longer. 


---


#### 9031.581

The time that we have with the people we care about is, in my opinion, the most valuable thing that we have. And once you enable people to have healthy lives with people they care about, more or less indefinitely, that changes a lot. And I'm very excited to see. I hope that happens in my lifetime. I think it will. I think it'll probably happen within the next decade even. But I hope that really changes human consciousness to a point to where a lot of these problems just   
(9062.572) ~~kind of~~(9062.832)  
start to go away because we stop thinking of everything in terms of finite resources, finite lifespans, finite time with the people that we care about. Hopefully it's enough of a conscious shift in consciousness that we see some of these problems fading because a lot of them are cultural, right? 


---


#### 9080.583

A lot of these problems or a lot of these like threats at the heart are very cultural. It's not about the technology. It's about how we use the technology and how we're interacting with each other when we use it. And that requires people to think differently. It's not a problem that can just always be addressed with some new technology or some new defense mechanism. We really have to change our thinking. And   
(9109.335) ~~that,~~ (9109.575)  
I hope that when these things start becoming widely available, people's thinking will shift dramatically. Maybe that's where things are headed. I actually have a lot of hope that's where things are headed and a lot of optimism because I think overall, like most people are good. 


---


#### 9126.618

And I think like we can heal a lot of things, not just health problems, but a lot of psychological things we can heal with these tools because it's going to change the way that we interact with each other and the way that we perceive our environment and our relationship to it. That is beautiful sentiment and maybe a good place to end. I don't know if there's anything else that you wanted to touch on, but hard to hit a more aspirational note than that.   
(9152.663) ~~I know.~~(9153.003)  
Yeah,   
(9153.504) ~~I think~~(9153.824)  
I agree with you.   
(9155.065) ~~I mean,~~(9155.285)  
as far as other things to discuss, I don't know. I think we've probably discussed pretty much everything I had. And we talked about most of the models that I found interesting. 


---


#### 9165.042

So yeah,   
(9166.423) ~~I mean, yeah,~~(9166.763)  
I think that's a good place to stop too.   
(9169.364) ~~I think~~(9169.584)  
we can probably call it there. And this has been really great,   
(9173.533) ~~by the way.~~(9173.973)  
I had a lot of fun doing this and I really appreciated this.   
(9177.435) ~~This is great.~~(9177.816)  
I appreciate you being willing to spend so much of your Saturday teaching somebody who doesn't know nearly as much as I suddenly feel like I really should about this area. So feelings definitely mutual. I guess my closing thank you is Amelie Shriver. Thank you for being part of the Cognitive Revolution. Of course. Thank you for inviting me. 


---



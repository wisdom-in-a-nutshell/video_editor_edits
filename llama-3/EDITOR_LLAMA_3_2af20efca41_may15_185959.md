#### 0.109

Amelie Schreiber, computational biochemist and AI researcher. Welcome to the Cognitive Revolution. Nice to be here. I'm excited for this conversation. I expect to learn a lot from it. This all started with a tweet that I saw you put out where you said, here are my top 10 AI tools for biology. And I read down the list and I was like, I don't know what any of these are. So   
(23.425) ~~I think~~(23.626)  
pretty much immediately just say, Hey, would you be interested in educating me in the form of a podcast? So I appreciate you taking the time. You want to start off by just giving a little bit of context on who you are, what you're doing day to day and what kinds of problems you're trying to solve. 


---


#### 36.149

Yeah, sure. I'm an AI researcher and I focus on computational biochemistry applications. I actually started out as a mathematician. My training in grad school was in mathematics, actually. Started off with pure mathematics and then transitioned into applied mathematics and data analysis. And then after grad school, I got into deep learning and started working on more AI related things. For me, the biochemistry applications are one of the most compelling things that we could be working on right now.   
(62.177) ~~I think~~(62.437)  
other than   
(63.577) ~~like~~ (63.737)  
AGI, whatever that means, I think it's probably the most important problem we can be working on because it's a huge impact on human health. the applications are really profound and have the potential to be very impactful for everyone. 


---


#### 77.995

So I get really excited about the biochemistry applications of AI. I have some projects and things that I'm working on that are more related to environmental things and material science type applications, but Primarily I focus on the medical or biomedical aspect of things. Okay, so let me try to give a extremely high level understanding of a couple of the biggest problems that are being studied in biomedical sciences. As I was preparing for this, I was having a good conversation with CLOB3 about it. And I came away with the understanding that both at the level of an individual cell, and then again, at the level of the overall organism system, We have one really massive challenge, which is that we don't know how it works. 


---


#### 126.777

We've got the DNA, which is the code, the RNA, which is both messenger, but also is a machine. The proteins are all machines that fold up in weird ways and interact with each other in three-dimensional space. And then you've got the small molecules as well, which are like signaling, but also if they fit right,   
(146.073) ~~you know,~~(146.233)  
all these puzzle pieces fit together in super strange ways. There's this incredible network of interactions where things are disabling each other or promoting each other or interacting in all sorts of complicated ways. The nature of those interactions initially was entirely unclear. And now humanity at large has embarked on this grand project of trying to figure out how do cells work and how do our bodies work. 


---


#### 167.169

And I'm gathering we're like maybe five to 10% of the way there. Most of the interactions remain unknown to us, but we've at least mapped out a decent chunk. So the first challenge, if you're trying to solve a disease is figure out what is the pathway? What is the interaction in this   
(183.596) ~~like~~ (183.796)  
super complicated thing that is going wrong? And then the second challenge is if I know what is going wrong, can I do something to intervene to stop it? But then again, there could be a lot of other knock-on effects. And in that way, there's an important commonality with large language models. These things are not super clean. In language models, people are probably familiar with the notion of superposition, which is one activation in a network. can light up for multiple different reasons. 


---


#### 211.282

And we certainly see all of these kind of patterns of complexity in biology as well. But we know that there's a lot of stuff going on. There's a lot of interactions that are happening. We don't really know a lot about that, but we're gradually learning more all the time. And then if you do have a target, now it's okay. These are all three-dimensional spatial things. And so it's just   
(237.243) ~~extremely,~~ (237.623)  
extremely difficult.   
(239.284) ~~It is.~~(239.604)  
Yeah. How am I doing there in terms of just setting a foundation to understand the challenges?   
(245.075) ~~I think~~(245.275)  
you've really hit the nail on the head. I work with a lot of different kinds of molecules. So small molecules, which are your drugs that you take in like a pill form, these are smaller than proteins and less complicated. 


---


#### 257.979

And I also work with proteins and also a little bit with DNA and RNA. And understanding protein interaction networks is a very difficult and complex problem. To just determine whether or not two proteins interact with each other, already is a hard problem. And then modeling how they fit together when they do interact and understanding the strength and how transient that interaction might be, it's very difficult. So protein interactions especially, but also protein DNA, protein RNA, and protein small molecule interactions are all very complicated things to model. There are some new ways to address this that have come out recently   
(300.321) ~~that I have a lot of hope for,~~(301.982)  
that I think are very promising and very effective approaches. 


---


#### 305.004

I use various kinds of AI tools, analyze these molecules, create new ones, modify them. engineer them in ways, grafting them together and stuff, performing complicated operations on these molecules so that they perform a particular kind of function. As an example, designing a new protein to bind to another protein so that you can cause some kind of cascade event in a protein interaction network, or so that you can block certain interactions between proteins. A really good example in cancer, your basic first examples of a mechanism of cancer, There's PD-1 and PD-L1. These are two proteins. One of them's located in the cancer and one of them's located on your immune cells. What happens is these two proteins end up binding to each other and essentially the cancer turns off your immune cell so that your immune cell doesn't attack the cancer. 


---


#### 360.994

And that's not good, right? You don't want this kind of interaction between these two proteins because you want your immune system to recognize the cancer and destroy it. Having this interaction turns off your immune system in a very specific way. So you can do things like design binders to this protein to block that interaction and that can help you combat cancer and hopefully treat it. And that's just one basic example of something that you can do with these tools that I'm using and that I'm interested in. You can also design new drugs with them. You can design drugs that are specific to a particular binding pocket on a protein. You can design drugs that have very specific chemical properties. 


---


#### 400.845

You can design proteins that have very specific chemical and functional properties. And this is pretty new stuff, but you can also do a lot of the same things with DNA and RNA molecules as well. Okay. This is a paradigm shift, right? The application of AI to biology, obviously the AI is creating all sorts of paradigm shifts, but   
(419.286) ~~I think~~(419.446)  
it might also be helpful for people to understand a little bit better of the before state when we didn't have any of these tools yet, which is not that long ago. Not that long ago. Yeah. What was the sort of prevailing approach to figuring stuff out? You hear these stories of, oh, look, we found this frog in the rainforest that is immune to a certain disease. 


---


#### 441.487

What's going on there? Let's see if we can't find something in this frog that could be a medicine or whatever. It's really anecdotally special observation motivated investigations in a lot of cases. And then I know there's also just a lot of brute forcing where it's like, we have no idea which proteins are going to interact with which other ones. So let's just create this massive cross matrix and see if we can't figure it out that way. And look for hits,   
(463.824) ~~kind of~~(464.044)  
massive essays, just exploring the space, all of these things without any idea of what the puzzle pieces actually look like, which makes it obviously very difficult to figure out how they would fit together. 


---


#### 475.332

What more would you tell people who want to understand, okay, what was the before, before all this stuff started to come online? There's a lot of methods that come from wet lab work where people do this stuff in animals. Like they say you want to do directed evolution on a protein and try to find higher functioning variants or variants that are more thermostable that have higher expression or something like that. You can mutate these things in a lab. You can do like point mutations or you can do two mutations at a time or you can do like multiple. When you start adding in things higher than just single point mutations, you get this combinatorial complexity, right? 


---


#### 518.932

And so it gets really unwieldy.   
(521.434) ~~I feel like~~(521.934)  
my experience with traditional methods is somewhat limited. I don't come from a wet lab background. I come from a very computational background. I haven't spent a lot of time working with more traditional methods that people have used historically. So computationally, traditionally the way that this sort of thing was approached was through molecular dynamics simulations. You have what's called a potential, right? And this potential tells you   
(550.267) ~~like~~ (550.487)  
how the dynamics evolve. And they come in a lot of different flavors, a lot of different complexities. Some of them model the proteins using just standard Newtonian physics. And then you can add in more complexity on top of that, things like quantum properties and other features of the protein to make the molecular dynamics simulation more complex and more robust. 


---


#### 572.891

But these simulations are really computationally intensive. They take a long time, they take a lot of GPUs, and they're just not very efficient. And on top of that, the length of time that you run your simulation for really in a lot of cases determines how accurate your distribution is and how accurate the confirmations or trajectories that you get out of that are. So you might run your simulation and not run it for long enough, and you don't get all the different states that the protein might be in, but you miss some of them, right? And there are some new AI models that are trying to address this and trying to make headway into augmenting or even replacing molecular dynamic simulations in a lot of cases. 


---


#### 621.931

And this is really good because we need things that are more computationally efficient so that we can do this for a lot of proteins, right, because we have a lot of proteins to do this for. So for example, AlphaFold2 came out a couple of years ago, and that was a big deal,   
(638.115) ~~right,~~ (638.375)  
But you just get a single static structure from AlphaFold2. So we give it the protein sequence, which is just a sequence of amino acids, which are represented by 20 letters, and it takes in this protein sequence, and it provides you with a static structure for that protein that's a low-energy confirmation for that protein. that protein could exist in other conformations. It might have other states that it exists in when it's interacting with other proteins, or based on the environment that it's in, what temperature it is. 


---


#### 671.968

Things like this can change the shape of the protein, right? They move around, they're very jiggly, and they do things. And so people have been trying to address this and model what's called the Boltzmann distribution of proteins. from statistical mechanics that tells you all the different confirmations and what probabilities there are associated to those different confirmations. And having a way to sample the Boltzmann distribution and get all of these different confirmations out of them, and also understanding the transitions between these states is a really difficult problem. And there's actually a model that does a really good job of addressing this that just came out middle of last year. It's called Distributional Graphformer. It's a generalization of the idea that AlphaFold2 is implementing, right? 


---


#### 720.975

It's not just a single static structure anymore. It's actually a whole ensemble of structures and also the transition pathways between those different metastable states. And being able to model this and understand more like the dynamics of the proteins is something that people have been thinking about pretty hard for the last couple of years.   
(741.788) ~~Distributional Graphformer.~~(742.929)  
is addressing a lot of this. And it does a pretty good job of doing it too. There's some room for improvement for sure, but it's a pretty solid model. Some people that I have a lot of respect for in this area have worked on this. And some of the inspiration comes from diffusion models. So it's a diffusion model similar to   
(765.03) ~~like~~ (765.17)  
DALI, which most of your watchers are probably familiar with, but it works on proteins instead of images and also protein complexes even, or protein small molecule complexes, and getting a handle on something that's more like the dynamics of the protein and getting a good representation of all the different metastable states that the protein might exist in at low energies. 


---


#### 788.385

So like a good example of how AI has sort of replaced wet lab methods, this directed evolution methodology, there are directed evolution AI models that you can use like protein language models to do directed evolution. Doing directed evolution in a lab in a lot of ways, now that we have AI tools to do similar things feels a little bit unnecessary.   
(812.993) ~~Like~~ (813.134)  
why do we need to go and inject an animal and wait some amount of time for this to play out inside the animal and then actually synthesize these things by hand in a lab somewhere when we can   
(824.298) ~~like~~ (824.458)  
do very similar things computationally and often get better results. You can also do a sequence redesign with things like protein MPNN or ligand MPNN, which allows you to redesign parts of the protein sequence or the entire protein sequence, maybe under some certain specific chemical constraints, or you might want to bias the residues towards or away from certain amino acids and things like that. 


---


#### 853.779

But these AI tools allow you to do that computationally and they do it really fast,   
(858.2) ~~right? I mean,~~(858.84)  
like I can design a sequence for a protein in a few seconds with   
(863.002) ~~like~~ (863.142)  
ligand and PNN on my computer with no special hardware or anything. I don't even need a fancy GPU to do it. And I can do that many times and get lots of variants for my protein. and assess them computationally. And very often these variants that you get out of this process are much higher performing than   
(885.065) ~~like~~ (885.225)  
the wild type or than what you would get by doing this in a wet lab. So hopefully that gives you some idea of some of the methods that still are being used. 


---


#### 894.85

It's not like these have just gone the way of the dodo and disappeared or something, but they have their place for sure. But   
(901.754) ~~I think~~(902.114)  
computational approaches are proving to be much faster, much more effective, and you can scale them, which is really important because we're working sometimes with millions or hundreds of millions of proteins. Having millions of variants of a protein and being able to assess them and determine their quality in some metric has become a lot easier in the past couple of years even.   
(927.074) ~~Like~~ (927.214)  
protein and PNN only came out a couple of years ago.   
(930.436) ~~I think~~(930.696)  
Because the AI techniques are so new, it's such a new paradigm. It's such a new methodology. 


---


#### 938.186

Most people working on them are still developing their understanding. There aren't very many experts on this stuff. I think we're all learning together. I'm definitely still learning a lot of stuff from my coworkers and other researchers in the field. And it's   
(952.829) ~~kind of~~(953.149)  
mind-blowing how fast this stuff is developing too. It's developing incredibly fast, which is really good in my opinion. I want to see this stuff proliferated and developed and used because we're going to solve problems much faster this way. So   
(967.848) ~~I guess~~(968.089)  
in terms of   
(968.509) ~~like~~ (968.609)  
just a little intuition for the confirmations, I envision a slinky where if I just sit the slinky down on the floor, it will come into a pretty tight coil. 


---


#### 979.568

And that you might say is like its lowest energy state. Then I can stretch it out. And if I do the work and put the energy into it, then I can stretch it out. Now, if I let it go, it's going to snap back to its low energy state. I could also step on the middle of it, and then I would have the part of it would be under my foot and bent down, but then the parts on the side would presumably still look like they're normal, but there'd be this deformed part in the middle where I'm stepping on it. Yeah. This is   
(1008.921) ~~sort of~~(1009.261)  
analogous to what is going on, violating my no analogy rule, but this is a pretty tight analogy. 


---


#### 1014.863

It's like a physical deformation, right? Where this thing can have a low energy state, but then maybe in the presence of some other protein that like constrains it in a certain way or some other small molecule, perhaps it fits into a pocket of it in a certain way or brings two parts that aren't normally together, more closely together, whatever. Then you can have these sort of deformations and then subject to those constraints, they still find their natural low energy state. And of course, this is all happening in an environment where the individual proteins, they're in solution, right? So there's water molecules bouncing off them all the time. So they have this sort of noisy environment. 


---


#### 1054.178

I'm thinking there of like brownie in motion. The constant sort of bumping into the environment creates opportunity for these things to occasionally flop from shape to shape. And so doing all of this in traditional sense is probably hard for a lot of reasons, but you highlighted the fact that the computation is really slow, right? Now,   
(1075.899) ~~like~~ (1076.02)  
I have a hypothesis on this, but I'll just ask the question. How is it happening that the AI models are doing this so much faster than traditional physics? Because a naive thought would be like, there's only physics, right? We hear that sort of refrain a lot. So it seems in some sense surprising that you would be able to make a new black box system to make these predictions that they would be faster and more accurate as opposed to just running the physics. 


---


#### 1105.716

How is that leap happening? Okay, so I think the key here is compression. neural networks are compressors of information. Whereas in molecular dynamics, you could simplify things by simplifying the forces or simplifying the model in terms of how complicated the physics are that you're using to model problems. If I strip everything down and just do bare bones Newtonian physics, I can simplify things that way, but there's no real compression happening. For these AI models, you can think of them as functions, but you can also think of them as compressors of information. You're taking something complicated and noisy sometimes, and you're compressing it and you're providing a representation of it that is more compact. Traditionally, you think of a deep learning neural network. 


---


#### 1152.753

You've got data, you train on your data. Maybe you have a train test validation split and you train on your training data and you You see how it performs on your test data and that's your trained model. But you can also train models with physics constraints,   
(1167.016) ~~right?~~ (1167.236)  
There are some approaches that people are using that are completely data-free and are based on physics. And the model is learning the physics and compressing that physics. You get something   
(1176.819) ~~that,~~ (1176.98)  
that is faster, like orders of magnitude faster,   
(1180.361) ~~right? You get,~~(1180.941)  
you get something that produces your answer in   
(1183.462) ~~like~~ (1183.602)  
a minute instead of four hours or days. And if you've done it right, it generalizes to systems that it hasn't been trained on before. people are doing this for this problem in particular, for getting the Boltzmann distribution of a protein and getting all these ensembles of confirmations and their transitions between the states. 


---


#### 1201.63

So that was pretty much my hypothesis that it's essentially learning higher order concepts beyond the raw physics. It's really this striking observation that comes up over and over again that, okay, yeah, language models, they're only trained to predict the next token, but they not only seem to be generalizing certainly beyond the narrowly defined bounds of their training data, and perhaps to some degree even more than that is a hotly debated topic, but what is pretty clearly demonstrated at this point is that in the middle to late layers of a language model transformer, the techniques are there to say, okay, this pattern of activations seems to correspond to this higher order concept that we care about, which is   
(1253.922) ~~kind of~~(1254.422)  
a miraculous thing that it's just predicting the next token, but it's learning these concepts of justice and fairness and ethics and whatever that are obviously useful to predict the next token, and that's presumably why they're arising, but not something that's been specifically coded for. 


---


#### 1273.457

So I guess in the application to biology, basically the same phenomenon is happening where raw data or raw simulated physics or whatever is the input, I'm guessing that the token level vocabulary of a protein would be the 20 amino acids, but the sort of higher order concepts are like, oh, this chunk of a thing is reused a lot. And these two chunks of things interact with each other in a particular way. Give us a little more intuition of that. What are the higher order concepts that these things seem to be learning? Yeah. So the concept that I think you're trying to grasp onto is protein motifs. Motifs are like reoccurring patterns that happen in proteins. 


---


#### 1313.611

They're short little sequences of amino acids that recur often in lots of different proteins and generally have a very similar structure across different proteins. If we put aside dynamics for a moment and we just look at like structure prediction. So there's another model, ESMFOLD, predicts the 3D structure of the protein in some low energy state, right? This is an alternative model to AlphaFold2. It doesn't perform as well as AlphaFold2, but it does pretty well. And it's a language model. It's something that people call a protein language model. And   
(1345.849) ~~it's,~~ (1345.969)  
it's built on the BERT architecture actually, which sounds kind of bad, right? Cause BERT's like this older model that's only used for like specific things now. 


---


#### 1356.377

The chat GPT models have overshadowed or outshined the BERT models at this point, but In biology, this actually makes a lot more sense because you have the mask language modeling objective that you train on for protein sequences, and you just mask out some of the amino acids in the protein sequence and have it predict what those are, right? And just by training it to do this, and then putting a folding model on top of it called EvoFormer, which actually comes from the AlphaFold2 architecture, you don't train on any physics. but somehow you learn how to predict 3D structures of proteins, right? And so in this case, it's almost like physics mostly isn't needed, right? If you just want to predict a static structure of a protein, you can get pretty good results just using a BERT type architecture with mask language modeling objective, training on millions of proteins. you get something that will fold proteins for you pretty darn well. 


---


#### 1413.688

There's some really nuanced architectural differences between ESMfold and AlphaFold2. AlphaFold2 uses what's called multiple sequence alignments, and it also uses these templates, right? And in general, it is better performing because it has these extra added things in the architecture that improve its ability to predict the structure. But even there, there isn't really a lot of physics explicitly happening. Now maybe there's some physics encoded   
(1441.796) ~~in this~~(1442.457)  
in some way, but we're not giving it   
(1444.681) ~~like~~ (1444.781)  
forces and potentials and things like that. And yet somehow we're able to predict the structure of the protein with really high accuracy   
(1453.389) ~~for a lot of proteins,~~(1454.529)  
for most proteins. I guess that's another example of where AI can be a lot better than the molecular dynamics. 


---


#### 1462.074

Because if you want to model a protein actually folding in a molecular dynamics simulation to get the folded structure of the protein, this is pretty hard and time consuming and computationally intensive. Whereas for AlphaFold2 or ESMFold, you give it a big protein and it takes a few minutes. And in these cases, these are language model-like models, right? They definitely have the architecture that looks a lot like language models, especially ESMFold. ESMFold is pretty much just a language model. And in terms of how this relates to language modeling. Motifs are   
(1498.179) ~~kind of~~(1498.519)  
a fuzzy concept, right? Like defining what a motif is and having that shape described is a little bit fuzzy, but these models learn these higher order concepts where you're looking at   
(1511.205) ~~like~~ (1511.345)  
groups of amino acids now instead of just the individual vocabulary elements, right? 


---


#### 1516.167

We're not just looking at individual amino acids of the vocabulary anymore. We're looking now at an aggregation of amino acids at a higher level. you can pull this out of these models. And there's some work on this, maybe three years old now, called Birtology Meets Biology. And they do a really in-depth study of how to pull out these different things, active sites and binding sites and motifs and things like this, based on the attention maps in the protein language model. Another thing that people have found is the attention maps recapitulate the contact maps for proteins. The contact map is like a 2D matrix representation of all the contacts between the different amino acids in the protein, right? 


---


#### 1560.399

And it turns out the attention map, the matrix that you get from your attention mechanism, recapitulates that and is highly correlated with those contact maps. So they are learning higher order concepts for sure, just as they do for natural language. You can do topic modeling and things like that on these models, but I would say now a lot of the more interesting models are more influenced by diffusion and flow matching models. A lot of the generative models that we're getting that are predicting the Boltzmann distribution or that are generating new protein structures for you with specific   
(1598.427) ~~like~~ (1598.587)  
shapes and functions or that are allowing you to design new sequences that fold into a particular backbone. 


---


#### 1605.731

A lot of them are more influenced by diffusion and flow matching than language modeling and transformers. Some of them use transformers, but they're starting to be a lot more influenced by Dolly type models, I would say, because you're starting to get this really fine grained control over what kinds of proteins or small molecules or nucleic acids that you can generate. And there's actually some models that have come out that are text conditioned. So like a couple of the models that I mentioned were ProteinDT and MoleculeSTM. And these are generative models that are text conditioned, and they allow you to type in   
(1645.253) ~~like~~ (1645.373)  
a natural language prompt and get out a molecule. So   
(1649.774) ~~like~~ (1649.914)  
protein DT, for example, or molecule STM, you can give it a text prompt, a natural language describing the properties of the molecule in just natural human language, giving it   
(1660.656) ~~like,~~ (1660.936)  
this molecule has these chemical properties and it has this sort of bias away from or towards these amino acids or interacts with these other molecules in such way. 


---


#### 1671.798

Like you can give it these natural language text prompts And it will generate proteins and small molecules for you that satisfy these constraints or   
(1681.86) ~~that,~~ (1682.04)  
that correspond to the text prompt that you give it. And there are more models like this that have come out recently that do similar things. They're text conditioned, like diffusion models or flow matching models that are generative and that produce molecules with specified properties based on natural language text, which in my mind, that's   
(1700.503) ~~kind of~~(1700.744)  
mind blowing.   
(1701.404) ~~I think~~(1701.624)  
that's amazing. Having a model. that will just generate molecules for you that fit natural language descriptions   
(1710.047) ~~is,~~ (1710.187)  
that's crazy. How did that happen?   
(1712.728) ~~Like,~~ (1712.848)  
that's amazing. No doubt. So let me just rewind a little bit again, and then I want to get into a little bit more how that happened. 


---


#### 1720.502

So the, I always try to start with like inputs and outputs as one kind of good frame for understanding this stuff. So it seems like the kind of first major breakthroughs   
(1731.953) ~~in~~ (1732.133)  
for biology of the   
(1734.875) ~~like~~ (1735.015)  
modern era, which is only the last however many years. were the structure prediction models. And   
(1742.635) ~~this is,~~(1743.476)  
if I understand correctly, there were about a proteins that had been analyzed to the point where people were pretty confident that they had a structure. If I understand correctly, this was mostly done through   
(1754.264) ~~x-ray crystalline, which is... Yeah,~~(1756.485)  
cryo-EM. Yeah. So I think that's why the initial things were   
(1762.009) ~~sort of~~(1762.29)  
limited to outputting a single predicted structure because if you're in like a crystal, you   
(1767.791) ~~sort of,~~(1768.051)  
by the nature of crystals, have a single repeating structure, right? 


---


#### 1772.617

So what we had was people put a lot of time in the lab into, first of all, figuring out how to get these things to crystallize, which is weird because   
(1782.128) ~~they're not really~~(1782.689)  
protein crystals don't really occur in nature,   
(1785.871) ~~right?~~ (1786.052)  
That's a very odd thing in the first place. Maybe that's like gout,   
(1789.634) ~~I guess.~~(1789.894)  
It's   
(1790.054) ~~sort of like~~(1790.454)  
uric acid crystals, if I understand correctly. But you don't think of proteins, we think of them as floating around in solution or   
(1798.359) ~~kind of~~(1798.559)  
interacting with each other in complicated ways, but they're not in repeating lattice structures. So that in and of itself was   
(1805.104) ~~sort of~~(1805.324)  
a weird,   
(1806.646) ~~like,~~ (1806.786)  
closest approximation that we could get, right? We got to make enough of this stuff that we can get it to put in, coalesce into some crystal form. 


---


#### 1813.616

Then we can hit it with x-rays and we can try to decipher how that gets scattered. And then we can come up with a structure and we hope.   
(1820.305) ~~I mean,~~(1820.565)  
we don't really know anything,   
(1821.586) ~~I guess,~~(1821.867)  
but   
(1822.127) ~~I guess~~(1822.347)  
it works well enough that that approximates the structure that it actually takes in the cell, but no guarantees. So first generation   
(1832.658) ~~of stuff is not first generation, of course, we're like~~(1834.84)  
other AI techniques before this, but like   
(1837.042) ~~of these sort of~~(1837.623)  
modern wave of   
(1838.664) ~~like~~ (1838.824)  
mega breakthroughs.   
(1840.686) ~~the,~~ (1840.846)  
and   
(1841.087) ~~I guess that was really measured by,~~(1842.428)  
maybe you could help me fill in some blanks here too, because   
(1845.272) ~~there's,~~ (1846.313)  
it's like   
(1846.934) ~~kind of~~(1847.114)  
circular nature to some of this stuff sometimes where I'm like, wait a second. 


---


#### 1850.037

So where is the ground truth? It seems to be a little bit of, it can feel like a, the ground truth is sort of a shell game. As I understand it, the way that AlphaFold was determined to be a breakthrough in the first place was that there was a competition held on an annual basis or whatever, where people would basically show up with their shape predicting model, and they would be given, here is the sequence. And their job is to predict the shape. And then the test set, the training set was all known proteins that came before. And the test set was all of the stuff that had been newly derived in the last year. 


---


#### 1893.033

So these were the new things that people hadn't been able to train on. They would show up and they would be measured against essentially the crystal based techniques. And everything would fall short, like not nearly as good, not matching the crystal things. And then AlphaFold showed up and was like, Oh, hey, it's and this is where I get a little fuzzy. As I understand it, people would say it's in some ways even   
(1917.488) ~~like~~ (1917.648)  
better than the crystal techniques. But   
(1919.549) ~~like,~~ (1919.749)  
how do we establish that? How do we know that   
(1923.311) ~~the when is the crystal technique right or wrong.~~(1926.714)  
I'm a little fuzzy on how we   
(1928.995) ~~kind of~~(1929.236)  
pin down the ground truth when we know that the crystal thing is only an approximation and AlphaFold was   
(1933.979) ~~kind of~~(1934.239)  
trained on that with augmented data. 


---


#### 1936.081

Like help me pin down the ground truth there if you can. Yeah   
(1939.363) ~~I mean ground truth in this case yeah I mean~~(1941.605)  
this is a little hard and it's very like application and   
(1945.871) ~~like~~ (1946.031)  
situation specific, right? Depending on what you're trying to do and how you're trying to do it, you may want some crystallized structure that you got in a lab, or you maybe want like an alpha fold structure. And in other cases you might want   
(1957.981) ~~like~~ (1958.182)  
a trajectory or an ensemble of conformations, which wasn't really possible until more recently.   
(1965.027) ~~Like~~ (1965.188)  
observing the dynamics of a protein is really hard. And so to be able to model that on a computer and get predictions that are actually accurate about the dynamics of the protein and all the different   
(1980.295) ~~like~~ (1980.495)  
low energy conformations that it exists in,   
(1983.976) ~~like~~ (1984.096)  
that's pretty new. 


---


#### 1985.516

And in my mind, if you have the ground truth really ultimately is the Boltzmann distribution, right? Which is this very sort of theoretical physics idea that comes from like statistical mechanics. that's the ground truth. Whether or not you can model that on a computer or observe that in a lab is another question. But the Boltzmann distribution of the protein is the ideal ground truth. And is that basically like a... I guess I'm thinking of it in one sense as   
(2017.069) ~~sort of~~(2017.309)  
like a potential, energy potential diagram where you have... It's related. It's a probability distribution, right? And it describes You can think of it in terms of an energy landscape, right? Because if you have this nice energy landscape, the low parts, the valleys that you have in your energy landscape are going to be like the metastable states of the protein. 


---


#### 2039.586

They're going to, they're going to correspond to the metastable states of the protein. And then the peaks, like on top of the mountains, right? These are   
(2046.147) ~~like,~~ (2046.367)  
like states that are very transient and that are   
(2049.528) ~~like~~ (2049.688)  
unlikely   
(2051.148) ~~to be,~~(2051.708)  
to exist for very long. So   
(2053.508) ~~you're,~~ (2053.728)  
when you're trying to model the Boltzmann distribution, you're trying to get out these   
(2058.383) ~~like~~ (2058.563)  
low energy conformations from it and then the transitions between those and understanding how often you transition between this state and this other state and what that transition looks like. I guess that would also be considered part of the ground truth, right? Because this is all part of the dynamics of the protein in the environment and not just some single either crystallized structure or alpha fold 2 predicted structure. 


---


#### 2084.288

Yeah, so I guess the answer to your question is the ground truth, at least to me, is the Boltzmann distribution. And the question of whether or not you can model that on a computer in a lab is a completely different question, but that's the ground truth. So it's a probability distribution of what percentage of the time the protein in some   
(2104.638) ~~like~~ (2104.838)  
neutral case solution or whatever is in shape A versus shape B versus shape C. And then the in-between things are sort of Here I'm   
(2116.327) ~~kind of~~(2116.648)  
again returning to my slinky visualization where I could have the thing   
(2122.412) ~~sort of~~(2122.692)  
in its lowest state or I could like tie its ends together and then it'll   
(2126.976) ~~sort of~~(2127.196)  
make a nice circle and but again   
(2129.378) ~~kind of~~(2129.598)  
look compact and be   
(2130.879) ~~sort of~~(2131.099)  
in a relatively comfortable place but then the second that breaks it's like reverbing back until it gets to its normal state, that reverb moment is sort of the transitional state. 


---


#### 2140.761

It's not going to be in that state very long and it's   
(2143.002) ~~kind of~~(2143.322)  
on its way from one to another. So we don't know how many different, for any given protein, there could be   
(2149.363) ~~like~~ (2149.483)  
multiple different low energy states that it might spend time in. And there probably also is like a path issue to it where you maybe can get from A to B and B to C, but not necessarily A to C without going through B I imagine. Yeah, exactly. So lots of weird stuff there. And then, okay, so all that is just they interact with each other. So this is,   
(2172.474) ~~I guess,~~(2172.694)  
where AlphaFoldMultimer starts to come in? Yeah. AlphaFoldMultimer models the interactions between proteins, right? 


---


#### 2179.721

And you can model protein complexes. And there's actually some new results that just came out maybe a month ago. that computes something called the LIS score based on the PAE output of alpha-fold multimer.   
(2194.626) ~~This is like a-~~(2195.166)  
Can you unpack both of those? Give us the PAE too. So the PAE is one of the outputs of alpha-fold multimer and it's,   
(2202.088) ~~let's see if I remember what the abbreviation is for,~~(2204.509)  
predicted aligned error, I think is what it stands for. And this is telling you, it's a metric that tells you the quality of   
(2211.451) ~~the~~ (2211.691)  
the interfaces between the two proteins. You've got a lot of different metrics that come out of AlphaFold Multimer or AlphaFold2. So you have PLDDT, which tells you a per residue confidence score of how confident the model   
(2226.192) ~~is that~~(2226.832)  
is the structure of the protein   
(2228.693) ~~at that particular point in the protein, like~~(2231.133)  
at that particular residue. 


---


#### 2233.094

And then you can take the average of the PLDDT and get an overall confidence for the whole protein. But then   
(2238.536) ~~you also have,~~(2239.116)  
you have IPTM and PTM scores, which are other scores that tell you about other aspects of the protein, and then you have these PAE outputs, predicted aligned error outputs, and these tell you about the quality of the interfaces between the proteins when it predicts the two proteins together. there's an interface region where the proteins are in contact with each other. And you can   
(2261.235) ~~kind of~~(2261.455)  
think of it as a certain cutoff, right? After a certain distance, you don't really count it as an interface residue anymore. But the PAE tells you the quality of these interfaces, how good of a quality the model has provided you. 


---


#### 2274.379

And you can compute something based on the PAE called the LIS. And the LIS score, let me look up what that stands for really quick, because I actually forgot what it stands for. So while you're doing that, I'll just riff a little bit on   
(2287.519) ~~the structure too. Yeah, or~~(2289.886)  
the nature of the interface, because this is just another level of   
(2292.488) ~~like~~ (2292.668)  
insane complexity, right? You have a range of kind of whether these things are like jigsaw puzzle pieces that are perfectly fit to each other and have a really tight coupling or jigsaw pieces that   
(2306.178) ~~sort of~~(2306.438)  
fit, you can   
(2307.018) ~~kind of~~(2307.299)  
press them together, but they don't perfectly fit and they don't really want to stay together as much all the way down to obviously they just don't fit at all. 


---


#### 2313.563

They just kind of don't don't adhere to each other. Is there anything more we could do to develop our intuition there for how strong is the strongest fit? I'm thinking like, boy, if I screw a screw into a nut, it's not coming off with any natural process. Somebody would have to come unscrew that. I'm guessing it's probably... I don't know. How tight are the tightest ones and what is the dynamic range of how adherent these things are to each other? Yeah, so there's two ideas that you're addressing here. One of them is like binding affinity, like how much affinity these two things have for each other to bind to each other. And then there's also in terms of   
(2356.407) ~~like~~ (2356.568)  
dynamics, like how weak or strong or how transient are the interactions between them in terms of   
(2363.513) ~~like~~ (2363.733)  
dynamics and like the time spent next to each other, right? 


---


#### 2367.696

There's recent work I think it's out of MIT, they built these flow matching models with AlphaFold and ESMFold. It's called AlphaFlow. And   
(2377.068) ~~AlphaFlow,~~ (2377.788)  
they use the AlphaFold2 architecture and they train it as a flow matching model, which is like a generalization of diffusion. And using this, they get these ensembles of confirmations for a protein. And part of the information that they get out of this is how transient the interactions between residues are. If you   
(2398.258) ~~produce,~~ (2398.818)  
let's say you run your alpha flow model and you produce   
(2402.621) ~~like~~ (2402.761)  
10,000 different confirmations or states that the protein exists in. And then you can   
(2409.266) ~~kind of like~~(2409.666)  
cluster those, like structurally, you can cluster them and then look at which residues are close to each other in each of those clusters. 


---


#### 2420.229

So maybe you take   
(2420.969) ~~the, you take~~(2422.189)  
the centroid or something of a cluster, and then you look at the distance between the residues, and then you look at other clusters, and the distance between the residues in those other clusters, and you get an idea of   
(2434.151) ~~like~~ (2434.391)  
how often two residues are in contact with each other from this. And you can tell how transient the interaction between these two residues are, and how much time they spend together. You could generalize this, right? And this is something that hasn't been done yet. So people who are looking for   
(2450.469) ~~like~~ (2450.589)  
research projects, this would probably be a pretty good one. If you generalize this to alpha fold multimer, do the alpha flow thing with alpha fold multimer, if it works well, and again, this hasn't been done before, but this would be a really great thing for someone to do. 


---


#### 2464.591

You could figure out how transient those interactions between two proteins are, right? Because now you have two proteins or more, maybe you have three or four or whatever, but you have two proteins that are in different conformations at different times. And AlphaFlow will generate all these different conformations for you. And then you can analyze all these different conformations and figure out how transient the interactions between the two proteins are and get an idea more about the dynamic side of things and not just a single number or a single metric like binding affinity, right? Because   
(2499.704) ~~binding affinity, I mean,~~(2500.724)  
it's a hard thing to predict. It's a hard thing to compute. training a model to predict binding affinity is actually a pretty hard thing to do. 


---


#### 2507.825

And most of them don't work. Most of them don't generalize well. But these approaches, like if you were to generalize alpha flow to the alpha,   
(2515.369) ~~like that,~~(2515.75)  
that would give you more information than just binding affinity.   
(2518.231) ~~That would give you,~~(2518.872)  
that would give you some notion of how often particular residues of the two proteins are in contact with each other. And then,   
(2526.497) ~~like I was saying before,~~(2527.317)  
the LIS score, this is the called the local interaction score. They use alpha fold multimer and they get the PAEs out of alpha-fold multimer. And then using the PAE, they compute the LIS, which is a pretty simple computation.   
(2541.888) ~~I don't know that I can describe it in words,~~(2543.509)  
but it's not a terribly complicated thing to compute. 


---


#### 2546.711

Once you have the PAE, the LIS is pretty easy to compute. And this tells you how likely you are to have a protein interaction, which kind of gets that binding affinity to some degree. And being able to predict protein interactions is actually a really hard problem. And most models that try to predict protein interactions don't work well and don't generalize well. And there's actually a   
(2570.649) ~~kind of~~(2570.909)  
a big problem with a lot of these models. So when people are training them, a lot of times if you're training a model that takes as input protein sequence or two protein sequences, people don't split their data in the right way. you have this notion of sequence similarity. 


---


#### 2587.529

And if you, if your data, if your training data has sequences in it that are very similar to your test data sequences, you're going to get overfitting and you're not even going to realize it. Like all the usual signs of overfitting aren't going to be there, but you're going to overfit without even realizing it because you're going to have training data and test data that's highly similar to each other in terms of sequence similarity. And a lot of the protein interaction models that have been trained don't take this into account. And they don't split their data based on   
(2620.426) ~~like~~ (2620.566)  
sequence similarity or structural similarity. But the LIS score using alpha-fold multimer works really well. And   
(2628.288) ~~it's,~~ (2628.428)  
it doesn't require any training of the model or anything like that. 


---


#### 2631.649

You just, you give it the two proteins or multiple proteins that you want to find out if there's an interaction there, and you get the PAE out of alpha-fold multimer, and then you just compute the LIS score.   
(2643.571) ~~So,~~ (2643.771)  
yeah. Okay. A couple of double clicks and maybe start with one summary. The prediction coming out of these alpha-fold models is this PAE, which is the positional predicted aligned error. So that is basically the actual positioning with   
(2660.014) ~~sort of~~(2660.255)  
a confidence indication. Yeah, it tells you what the quality of the interfaces are between the two proteins that you're predicting in the multimer. And something else we should probably get into that directly follows from alpha-fold multimer is other ways of generalizing the alpha-fold model or training models that are like alpha-fold that do more than just proteins. 


---


#### 2682.869

You might have complexes where there's a protein in a small molecule, or protein in DNA, or protein in RNA, or a metal, or whatever. And so there's all these other biomolecules that you might want to model in complex with each other. And to generalize alpha fold multimer to this new situation is pretty hard, but some people have managed to do a pretty reasonable job of it. I think there's still room for improvement on these, but   
(2714.225) ~~like~~ (2714.385)  
a new model that just came out recently is Rosetta fold all atom and Rosetta fold all atom will let you predict complexes that have proteins and small molecules, proteins and nucleic acids, and proteins, and proteins and metals too. 


---


#### 2729.853

Big step forward now, because now you can apply this idea of computing the LIS score to these other complexes. And you can get this score that tells you how likely there is to be an interaction there and how strong that interaction is. And you could also,   
(2746.06) ~~I don't know how hard this would be to do, just thinking about it now, it seems like it might be actually kind of hard, but you could probably do~~(2755.071)  
the alpha flow type method with something like Rosetta fold all atom as well and get something like conformational ensembles out of it. And   
(2765.394) ~~that's probably something like that is probably coming soon.~~(2768.235)  
Somebody is going to work on that eventually. So yeah, 


---


#### 2771.296

I think I answered your question. I'm not sure. Yeah. Let me just think about where I want to go back to.   
(2776.438) ~~Okay.~~ (2776.518)  
The one thing that you said that caught my attention was, this is all in the context of predicting shapes. We need to predict shapes because we need to understand how things interact. Now we're even getting into predicting how things conform to each other. So the shape of multiple things as they're in actual interaction. And we get these sort of positional predictions that can be   
(2801.232) ~~sort of~~(2801.472)  
cashed out to these parts are actually like interacting in a meaningful way. And this is really where the action is versus these other things are   
(2808.316) ~~kind of~~(2808.496)  
distant from each other. 


---


#### 2809.177

And that's not really where the action is. That's being generalized beyond all proteins to like all the different kinds of things that are meshed up together in a cell. But I believe you had said that there were like as many as 10,000 possible confirmations for a single thing.   
(2829.973) ~~Was that,~~(2830.274)  
did I get it? Yeah. So   
(2831.855) ~~like~~ (2831.996)  
AlphaFlow, when you run AlphaFlow, it generates confirmations of a protein for you. And it was trained on molecular dynamics data, on simulation data. And so it does have some notion of   
(2846.546) ~~like~~ (2846.706)  
dynamics. And what it does is it produces different confirmations of the protein for you. And you can tell it how many of these to produce, right? And the more that it produces, the more likely you are to get a nice global picture of all the different confirmations that might exist for that protein. 


---


#### 2865.797

AlphaFlow, so we've actually tested AlphaFlow on these proteins that are called fold-switching proteins. Fold-switching proteins, so like probably the most popular example floating around in the literature and in the community right now is Kybe. And Kybe is this fold-switching protein that like 10% of the time it exists in this one conformation and then 90% of the time it exists in this other conformation. And this is influenced by   
(2892.288) ~~like~~ (2892.408)  
a circadian rhythm. So it's   
(2894.049) ~~like~~ (2894.189)  
a night-day cycle sort of thing that's   
(2896.329) ~~influenced,~~ (2896.849)  
influenced by like your circadian rhythm. And when you apply alpha flow to some of these fold-switching proteins, it doesn't capture both of those fold-switch states.   
(2908.551) ~~It will like,~~(2909.151)  
so in the example of CHI-B, it actually only really predicts conformations that are relatively close to the fold-switch state. which is like the slightly higher energy confirmation, the one that's a little bit less likely, the one that it exists in 10% of the time, which is a little bit odd, right? 


---


#### 2927.519

Because you would expect and maybe want your model to go for the ground state or the lowest energy confirmation. And for some reason it like sticks   
(2938.084) ~~kind of~~(2938.364)  
close to the fold switch confirmation. I'm not sure that there's like a good explanation for why. And I think it goes back to the AlphaFold2 predictions. Because when you predict the structure using AlphaFold2, you get the fold switch state. You don't get the ground state. And people have done all kinds of little hacks to try and get out the ground state instead of the fold switch state. And the most popular method that they've hacked together is doing MSA subsampling or clustering the MSA and using the different clusters to predict structures. 


---


#### 2975.196

If you take your MSA and you cluster all of your sequences in your MSA,   
(2981.68) ~~you're kind of like,~~(2982.541)  
you're grouping the sequences in the MSA in a way that captures certain evolutionary information. And different clusters will focus on or accent particular conformations. And so if I take out one of my clusters and predict the structure using those clusters in the MSA, I'll get a confirmation out from AlphaFold2. And then if I pick   
(3007.59) ~~a different set of,~~(3008.57)  
a different cluster of sequences in my MSA, I'll get maybe a slightly different confirmation, or maybe a drastically different confirmation. And   
(3017.696) ~~if you do this,~~(3018.276)  
if you do this right, sometimes, not always, but sometimes, you can get out the different confirmations of these fold-switching proteins. 


---


#### 3026.501

And for Ki-B, they've done this successfully, and for a few others, but it's not a super robust method, And I think these alpha flow, I think is in some ways maybe more informative. And something like Boltzmann generators or distributional graph former, I think are significantly better in terms of how they approach the problem because they're going to give you more information. and they're gonna give you more robust information. So for example, like distributional graph former, you're gonna get out something more robust and more informative than if you're just like clustering the MSA or subsampling the MSA for alpha. Can we talk about this MSA thing for a second? If I understand clearly, I'm not even sure I should attempt this, but I'll go for it. 


---


#### 3077.124

Is it basically that we know that a gene codes for a protein, we have a lot of variation in the genes. The genes can have lots of random differences between them, but we can   
(3090.691) ~~sort of~~(3090.911)  
identify that these are all different variations on the gene. Some of the genetic, some of the DNA level differences may make no difference in the protein, but others will make differences in that at a particular position in the protein sequence, you'll have a different amino acid. And so now you've got   
(3110.372) ~~kind of~~(3110.692)  
the same protein, but it can have different elements in particular position. And so things are grouped for the purposes of prediction.   
(3121.28) ~~Kind of.~~(3121.66)  
So an MSA is actually a pretty old concept that comes from computational biology. 


---


#### 3129.947

People have been using MSAs for a long time. And essentially, it's based on the edit distance. So if I have just a string of characters and I make some edits in some different places, I can compute the edit distance between those. And if I have a low edit distance, then those two sequences are highly similar. MSAs are basically this. I take a protein and I have a whole bunch of different mutations of that protein or a whole bunch of other protein sequences that are very close to that protein in terms of sequence similarity, but they have some changes here and there. A lot of times the changes that happen only happen in certain regions of the protein and then there are other regions of the protein that are highly conserved. 


---


#### 3176.55

And so when you do an MSA you can look at which regions of the protein are really highly conserved and a lot of times this will give you some indication of which parts of the protein are going to affect the function if you like mutate them and stuff. So if I have a highly conserved residue that in my MSA it just doesn't change it stays the same through pretty much all of the MSA. Like 90% of the sequences in my MSA, this amino acid stays the same, right? If I change that, if I mutate that, it's probably going to affect the function of the protein. Because it's like a highly conserved region of the protein that evolution hasn't changed or has changed very infrequently. 


---


#### 3219.218

And so because of that, if you change some of those residues that are highly conserved, oftentimes you'll degrade the function of the protein or change the function of the protein, or maybe you'll decrease its thermal stability or something like that. So MSAs are just telling you, they're telling you evolutionary information that is conserved among a whole group of proteins that are highly similar to each other in terms of sequence similarity. And AlphaFold2 uses MSAs. You can either use the database of MSAs or you can have it compute them on the fly. And it uses these MSAs to inform how it predicts the structure of the protein. Because when you have proteins that are very closely related evolutionarily, in terms of evolution, their structures are often very similar, right? 


---


#### 3267.157

That's not always true. I can have two proteins that are very similar but have very different structures. That happens all the time. But if you have this extra evolutionary information in the form of an MSA, you have extra information that helps you predict the structure of the protein because all of these evolutionarily related proteins are oftentimes going to have very similar structures to your protein of interest. This is   
(3293.007) ~~sort of~~(3293.287)  
calling to mind the classic image of the plane with all of the spots where the planes came back having been shot and then all the places that they didn't observe, those were the planes that got shot down. So this is the evolutionary equivalent of that where we don't see changes in certain regions because they're super core to functionality. 


---


#### 3317.476

And that in turn is super useful for prediction making because that these parts are like the really important parts and they're going to have to fit together or the sort of interactions that they have with other things are   
(3329.922) ~~kind of~~(3330.262)  
the whole point of what's going on here. Okay. So that's interesting. The overfitting piece, I didn't quite understand. It seems like that's related though, where you said because these things are so similar, You have to be careful that you're not, give me the overfitting thing again. Cause   
(3345.091) ~~I can't,~~(3345.371)  
I'm not sure I can do it justice. Like when you do a train test split in deep learning and you're training your neural network   
(3352.397) ~~on your train,~~(3352.977)  
on your training data, and   
(3354.879) ~~you have,~~(3355.239)  
you have your test data to   
(3356.981) ~~sort of~~(3357.301)  
test your model on after the fact, once it's trained to see how well it predicts on data that it hasn't seen before. 


---


#### 3364.287

And so when you're doing this, you want to make sure that your test data doesn't have a bunch of sequences in it that are highly similar to your training data. Because it's almost like you're training on the same thing twice and you overfit this way. You don't get a good indication of how well your model generalizes. And a lot of people do this. A lot of people coming from   
(3384.655) ~~like~~ (3384.795)  
deep learning, just getting into   
(3386.335) ~~like~~ (3386.475)  
the biology stuff and they don't have a super strong background in biology. They make this mistake very often. And so there's just tons and tons of neural networks and different kinds of deep learning models out there. that don't generalize and that are very overfit because they didn't split based on, they didn't split their data based on like sequence similarity and or structure similarity. 


---


#### 3407.847

So you, like when you train models, usually you want to split your data based on sequence similarity and or structural similarity. And a lot of people also split it based on   
(3419.191) ~~like~~ (3419.351)  
dates, like you were talking about CASP earlier. they have like a certain cutoff date and then the stuff that was resolved after that cutoff date is used in the test data. But   
(3429.062) ~~when you're training,~~(3429.982)  
when you're doing your training data, you split your data based on things like sequence similarity and or structural similarity to make sure that you don't overfit and to make sure that your model generalizes to unseen data. Gotcha. Interesting. Okay. Yeah. It seems like in the case of something about this that I don't have a good intuition for because that's not really done in language modeling, right? 


---


#### 3451.176

In language modeling, you could certainly have like lots of sentences that are very similar and you don't   
(3457.458) ~~sort of~~(3458.278)  
say, Oh, we're going to hold out.   
(3460.618) ~~We don't,~~(3460.838)  
we don't draw conceptual lines between different parts of the data and try to generalize across those lines. So what is the difference in the biology context?   
(3471.481) ~~Like~~ (3471.622)  
my intuition says, to the degree that this thing is learning, that these models are learning like the higher order concepts that really matter, that they should be able to learn those kind of regardless. And again, in the language model case, we don't really have a concept of overfitting, at least in large scale foundation models. Is this maybe just because we're not really doing large scale foundation models in quite the same way? 


---


#### 3496.388

Or how would you describe the difference?   
(3498.956) ~~I mean,~~(3499.176)  
there's still a concept of overfitting in, in NLP and training big giant models, Claude or ChatGPT or whatever.   
(3505.559) ~~Like you,~~(3505.839)  
you can definitely still overfit these models. I very often for an NLP models, like these really big chat type models,   
(3513.242) ~~like~~ (3513.362)  
really big LLMs and stuff. First of all, they often only train on one pass through the data, right? They don't do multiple passes. And partially because of that, overfitting is not much of an issue because you're not training multiple times on the same data. So I do think that is changing. One little nugget from the recent Zuckerberg-Dwarkesh interview that I definitely made my ears and brain light up was when he said they trained these latest llama models on 15 trillion tokens. 


---


#### 3542.04

He said, we kind of stopped because we, at some point we need to move on to Lava 4. But he said we could have rotated the high value tokens through again. And I was like, Oh, interesting. I've seen some results about that, but in any event, it does seem there's, we're now to get to 15 trillion tokens. Basically, I don't think you have much choice, but to rotate. Yeah. Anyway, that's a bit of an aside, but I'm still not quite grokking it to be honest. Okay.   
(3567.93) ~~So let's see,~~(3568.831)  
what's a good analogy. I'm trying to think because yeah. And like NLP, like most people don't really think about the, so you have a data distribution and your training data and your test data, like your test data is supposed to tell you something about how well the model generalizes. 


---


#### 3586.741

Right. And it's also supposed to tell you about if the model's overfitting or not, because when you compare your training metrics to your test metrics, whatever they may be. If your training metrics are different, like the training test, or the training metrics and the test metrics are substantially different, then you're either overfitting or underfitting. If   
(3609.208) ~~your test metrics,~~(3610.289)  
if the metrics on your test data are substantially worse than the metrics on your training data, then you've overfit,   
(3621.0) ~~right? And, and if,~~(3622.067)  
if it's the other case, if your test data is substantially better than your training data, which is   
(3628.089) ~~kind of~~(3628.329)  
hard to do, then probably you could train some more.   
(3632.071) ~~Right.~~ (3632.331)  
Maybe you're under fit. 


---


#### 3634.212

So your train test split is supposed to tell you something about how well the model generalizes and how overfit your model is and comparing how it performs on the training data to the test data. tells you that. It tells you a lot about how overfit your model is, if it's overfit, and how well it's generalizing to data that it hasn't seen before. And to really   
(3655.259) ~~get a good grasp,~~(3656.66)  
to get a good idea of how well your model is generalizing to unseen data, you want at least part of your test data to be very dissimilar from your training data. Because that means it's generalizing to things it hasn't seen before,   
(3672.086) ~~right?~~ (3672.246)  
That means it's picked up on some deeper concept in language that generalizes to areas that it hasn't seen before. 


---


#### 3680.641

And it's using those really deep concepts to make predictions or make, generate things that are out of distribution. And this is a big thing that people discuss is   
(3691.804) ~~like~~ (3691.964)  
whether or not these things generalize to data that's out of distribution. And if you train them in the right way. you can get models that generalize well to out of distribution data, right? This is not something that's impossible to do. You just have to do it right. And in the case of biology or biological sequences like proteins, to get a test set that gives you a good indication of one, how well the model is generalizing and two, if it's overfit or not, you need to make sure that your test data is very dissimilar from your training data. 


---


#### 3727.976

And the way that you do this is you look at the sequence similarity between the protein sequences in your training data and your test data. And you can also look at structural similarity, because you can have different sequences that are very different in terms of sequence similarity, but that fold into the exact same structure, more or less, right? We can have two very dissimilar protein sequences that fold into pretty much the same structure. And so sometimes depending on what your model architecture is and what your goal is, you may also want to split based on structural similarity and not just sequence similarity to make sure that your model is generalizing and not overfitting. Okay. I think I got it. 


---


#### 3768.601

Does that make sense? Yeah. I think so. It seems   
(3771.862) ~~that it is sort of~~(3772.882)  
a form of data leakage, essentially. Like you could imagine, and it's   
(3776.843) ~~sort of~~(3777.223)  
that you're fooling yourself, right? For any given architecture, presumably the very best performance would be if you trained on all the data. But in order to effectively evaluate your architectures along the way, you need to have some holdout or you might call it a benchmark in certain contexts to evaluate against. And these similar enough sequences basically are a data leak in the same way that if you find out after you do your thing that, oh, hey, we actually had MMLU in the training data for the language model, then it means, oh, you can't really trust the MMLU scores anymore. 


---


#### 3814.732

And the model still may be good, it may not be so good, but if you train on MMLU, we can't really score you on MMLU. And this is a similar problem. You can't trust her. Exactly. Exactly. Yeah, exactly. And there are even more nuanced ways of splitting the data, too, for specific things. The new version of DiffDoc They trained a new version of DiffDoc, I think they call it DiffDoc L, because it's larger. It's the large DiffDoc. And they use this method called confidence bootstrapping, which is   
(3846.667) ~~sort of~~(3846.927)  
like reinforcement learning. And they also split their data in a really unique way that's based on different domains or motifs that are present in certain interactions. 


---


#### 3860.561

They split their data based on that, in addition to, I think, sequence or structural similarity. I would have to look at that. they split their data based on these domains that are present in these interactions to train a model for docking, right? So you have a ligand, a small molecule ligand that you're trying to dock into a protein and do like blind docking, which is a hard problem. And they get   
(3883.878) ~~like~~ (3884.038)  
substantially better performance and it generalizes a lot better in this new version of DiffDock because of the way that they trained it and the way that they split their data. And they have some really strong confidence that their model is generalizing to out of distribution data. 


---


#### 3899.794

And it's able to predict on things that it hasn't seen before. And they're very dissimilar from what it has seen. Just to make sure I understand,   
(3909.36) ~~when you said, I've lost exactly what you said, but~~(3912.282)  
I just want to make a distinction between what they've demonstrated is that you should be more confident in doing this stuff in totally new regimes based on the fact that they've been very meticulous in the data split. Whereas if they had thrown everything into the training, then you would have a hard time knowing to what degree to be confident in out of distribution stuff. Yeah. Okay. Cool. And they also,   
(3937.61) ~~I mean,~~(3937.77)  
they did a really good job with that model. 


---


#### 3939.413

I think their performance boost was pretty big. They got a lot better performance out of it too.   
(3943.742) ~~So.~~ (3943.862)  
That's definitely a good model to look into if you're looking to get into this stuff. So maybe let's,   
(3949.081) ~~I don't know if there's more that you think we need to cover on.~~(3952.882)  
  
(3953.062) ~~I mean,~~(3953.403)  
we've been up and down the layers of or the levels of abstraction, but it seems like the two big things that I want to go to next   
(3962.426) ~~and~~ (3962.546)  
being mindful that we've already been at it for a while are the diffusion concepts where it seems like we're moving from predicting a structure to generating new things. And then maybe we could get into a little bit of, okay, in actual work, like what are the cycles that are used to actually make progress on questions of interest? 


---


#### 3983.635

Like you have a target, you want to make some modification, like how do these things fit together to allow us to work a lot faster and get more value from our limited work resources? Before we go on to the diffusion and generative side though, anything else that we didn't cover or that you think is   
(4000.622) ~~missing part of the piece,~~(4001.643)  
missing part of the picture for the fundamentals or the structural prediction? No,   
(4006.006) ~~I think,~~(4006.346)  
yeah, we should move   
(4007.307) ~~into,~~ (4007.807)  
into   
(4009.028) ~~like~~ (4009.168)  
RF diffusion. I think that's a good direction to go in now. Are you familiar with RF diffusion at all? No, not really. Although from what little you said earlier, it sounded to me like clip basically. 


---


#### 4021.057

I was sort of hearing that. know with clip you have kind of images and their captions and here it sounds like we have like proteins and their sort of descriptions no so that that's protein dt and molecule stm those are much more like clip they use the exact same method as clip They use contrastive learning and they have captions and molecules or captions and proteins. Those are our text condition models where you can type in a natural language description of your molecule or your protein without a structure or a protein sequence that fits that description. Those,   
(4059.742) ~~I think,~~(4060.523)  
are a bit different from RF diffusion. RF diffusion is a diffusion model that it's not text conditioned. 


---


#### 4068.273

You can condition it on other types of things, but you don't give it a text input. It's   
(4073.119) ~~a little more, I guess,~~(4074.801)  
a little more specific and it's a little more geared towards people who want to perform surgery on proteins. So if you want to design new proteins with specific structural properties and you want to get your hands dirty and perform surgery on these proteins and graft them together or take pieces from this one and graft it onto this one or generate a protein with a specific sort of fold tertiary structure or or maybe generate a protein that binds to a specific protein with really high affinity and specificity. These are the things that RF diffusion is good for. 


---


#### 4112.552

So RF diffusion is a diffusion model. They used Rosetta fold, the Rosetta fold backbone, and trained it as a diffusion model to denoise 3D structures of proteins. And there are several different versions of RF diffusion. There's a new version that just came out called RF diffusion all atom. which allows you to generate proteins that will bind to small molecules. So you can generate proteins with binding pockets that are highly shaped complementary to a small molecule ligand. And with RF diffusion and RF diffusion all atom, you can also do something called motif scaffolding, which is where you pull out motifs from a protein that you like. Maybe they're   
(4155.73) ~~like~~ (4155.85)  
binding sites or active sites, or maybe there's a particular segment of the protein binds to a different protein that you're interested in or performs a specific function. 


---


#### 4166.386

And you can pull these pieces of the protein out and scaffold them and build a new protein around those pieces that holds those pieces in place so that you have a new protein with very specific 3D structure that performs like some very specific function. And it's been a very influential model and a very useful model. And it's definitely one of my favorites.   
(4188.885) ~~Maybe we should dig into that a little bit. Yeah.~~(4190.806)  
Give me a little bit more on how, what exactly it is that you're specifying. It's not text conditioned, but you're saying I want it to have certain properties and then it's filling in the sequence that gets you to those properties. Yeah. So   
(4205.214) ~~like the most,~~(4206.255)  
the most basic usage of RF diffusion is unconditional generation of a protein. 


---


#### 4211.078

So you just, you tell it some length. or range of lengths, and it will just generate proteins of that length that are brand new, that have never been seen in nature before, and very often are very designable and that you can actually synthesize and create in a lab. And that's just completely unconditional generation. You don't give it any sort of constraints. It just generates a new protein for you of a particular length. Then you can also, one of the really interesting functions of RF diffusion is it will design binders for you. So if I have a target protein and I want to design a protein that binds to it with really high affinity and really high specificity, 


---


#### 4256.013

RF diffusion is really good at that. It'll design binders for pretty much any protein you can give it, and very often The proteins that it designs that bind to your target protein are very high affinity and very high specificity and often very thermostable. The other functionality that's really useful is the motif scaffolding that I was talking about before, which is where you pick out pieces of a protein or multiple proteins and you build a new protein that holds all those different pieces in place in a particular way. And so this is one thing that you could imagine doing with this would be like building or designing an adjuvant or like grafting two proteins together. Or let's say I have one part of a protein that binds to protein A and I have some other protein that binds to protein B. 


---


#### 4314.278

I want to design a protein that binds to both protein A and protein B so that I can get a complex with three proteins in it, right? I want to have a protein that binds to protein A and protein B. So what I can do is I can take those pieces out of the protein that bind to protein A, and I can take the pieces that bind to protein B, And I can scaffold them together into a new protein. And now I've got a new protein that binds to both of those proteins. And I can do things like build out protein interaction networks this way. So if I want to design a particular protein interaction network, this is really useful for that. 


---


#### 4347.909

That's a pretty technical and involved thing to do. Like building up a protein interaction network is a non-trivial thing to do, but you can do it with RF diffusion. You can design proteins that will bind to multiple different proteins in multiple different contexts and build out these networks this way. And this gives you   
(4368.897) ~~like~~ (4369.037)  
a way to modulate protein interaction networks, right? Because if you design a binder to block a particular interaction, you can modulate your protein interaction network by blocking particular interactions by designing a binder. But you can also add in interactions that weren't there before using the motif scaffolding or maybe binder design and motif scaffolding together. So it's very useful in a lot of different contexts, but it's not text-conditioned like ProteinDT or MoleculeSTM or some of the other text-conditioned diffusion models for proteins, because there are a few others now that recently came out as well. 


---


#### 4404.272

But yeah, it's not text-conditioned. It's very much more geared towards people who are really interested in performing surgery on proteins and protein interaction networks. And now with RF diffusion all-atom, also with other interactions as well, because with the all-atom models, you can model more interactions than just the protein interactions. So how does this in practice get used? Maybe the cancer example from the top is a good one, or we could go to another one, but... Yeah. in that scenario we sort of already had an understanding of the cancer cell has this thing that disables the immune cell and so then you could say okay Let's brainstorm some ideas here, right? If we can bind something to that bit of the cancer cell that would   
(4457.516) ~~kind of~~(4457.776)  
cap it, blunt its ability to then interfere with the immune cell, then the immune cell presumably would do its job still and kill the cancer. 


---


#### 4465.563

Of course, you've got highly tangled webs of interaction that you're doing this within. but you've got to take something local like that. Now kind of take me through the cycles and the practical application of some of these tools for a specific problem of that sort. Yeah, so I've got a few examples here that we can talk about. I wonder which one would be   
(4486.616) ~~like~~ (4486.776)  
the best or the most interesting for people. So like the one that we were talking about earlier with the cancer, with PD-1 and PD-L1 as a really good first example that I think is a really good place for pretty much anybody to start. Because you can very easily and very quickly design a binder to one of these proteins with RF diffusion. 


---


#### 4506.119

It's really good at designing binders for pretty much anything. If I have this PD-1, PD-L1 interaction between these two proteins, essentially what's happening is the cancer is turning off your immune system's response to it, and then your immune system doesn't effectively combat the cancer. But if I design a binder to one of these two proteins to block that interaction, and my binder out-competes that interaction, so it has a higher affinity than the PD-1, PD-L1 interaction has, then I can successfully block that interaction and prevent the cancer from turning off the immune cell's responses to it. So that's a really good place to start. Another way that RF diffusion can be used, so let's say you have a protein that binds to a target, but it doesn't bind very well. 


---


#### 4555.755

#### 4601.356

And if I do this and I give RF diffusion the target protein that I'm interested in, I can improve the shape complementarity between those two. So the new denoised protein or the new denoised version of my original protein is going to have a higher shape complementarity to my target. And then I can go and design sequences for that backbone that are different from my starting sequence, right? So maybe my starting sequence, maybe there were some residues that had unfavorable chemical properties at the interface,   
(4631.632) ~~right?~~ (4631.852)  
Maybe I need to use different amino acids to improve some chemical properties so that the binding affinity goes up,   
(4640.596) ~~right?~~ (4640.776)  
I can do that with protein MPNN or ligand MPNN. 


---


#### 4645.011

So ligand MPNN is the newer all-atom version of protein MPNN. It's an improvement on protein MPNN, and it also generalizes to contexts where you have other kinds of molecules other than just proteins. And I design a sequence with ligand MPNN, and I can tell ligand MPNN to bias certain residues towards certain amino acids or away from certain amino acids, like at the interface, for example. to get those more favorable chemical properties to increase my binding affinity further. And   
(4678.628) ~~I can also,~~(4679.328)  
there's also versions of ligand and PNN that will allow you to specify   
(4683.191) ~~whether a residue, so let me check on this really quick, whether a residue is~~(4688.095)  
a buried residue, an interface residue, or something else. 


---


#### 4692.598

I can also tell ligand and PNN about symmetries, which is a really interesting thing that RF diffusion and ligand and PNN can do together. Just to clarify, RF diffusion doesn't usually get used on its own,   
(4706.457) ~~like~~ (4706.617)  
by itself, because it just works in structure space, right? So it's doing the denoising process on the structures of the proteins. It doesn't know anything about the sequence of the protein. So I need a separate model, like Ligand and PNN, to design the sequence for that 3D structure. So they   
(4724.952) ~~kind of~~(4725.212)  
go hand in hand. You use them together. So once you've generated your 3D backbone of your protein, you design a sequence for it using ligand and PNN. 


---


#### 4735.789

And using these different functionalities of ligand and PNN, you can increase your binding affinity and other properties even more. Yeah, so like using partial diffusion with RF diffusion to slightly noise and then denoise a structure that you already have. can help you increase things like binding affinity and things like thermostability and other properties. Then,   
(4756.568) ~~let's see,~~(4756.889)  
what's another application of RF diffusion? So one that I was looking into recently,   
(4763.673) ~~let's see, I want to pick out a good one because I want to give people really interesting examples to think about because you can really do a lot with these models if you get into it pretty deep and really learn how to use them. Let's see, there we go.~~(4776.541)  



---


#### 4777.358

Okay, yeah, so there's unconditional generation, symmetric generation. I touched on that a little bit. You can design symmetric oligomers. Let's say I want to have a protein that interacts with itself, or other copies of itself, I should say. And if I have enough copies of this protein, it forms a symmetric complex. For example, Let's say I have a protein that fits together with two other copies of itself in a triangle formation,   
(4811.326) ~~right?~~ (4811.506)  
And it's symmetric to the cyclic group of order three,   
(4815.769) ~~right?~~ (4816.029)  
So I've got a order three rotational symmetry that's happening. I can use RF diffusion to generate proteins with symmetry like this. And it has other symmetries that it can use. So there's dihedral symmetries, there's symmetries icosahedral symmetries and tetrahedral symmetries in addition to the cyclic symmetries. 


---


#### 4836.766

And I can, the cyclic and the dihedral, I can choose like any order, cyclic group or dihedral group for my symmetry for those. And RF diffusion will design a symmetric complex of proteins where there's like multiple copies of the protein in this   
(4853.891) ~~like~~ (4854.051)  
nice symmetric structure. And where this occurs,   
(4857.192) ~~like~~ (4857.332)  
this occurs in nature, in multiple places. One example is in viral capsids. And they've also recently, some David Baker's lab recently published some work where they design these   
(4871.198) ~~like~~ (4871.379)  
symmetric oligomers as   
(4873.94) ~~like~~ (4874.1)  
biosensors. And I think they also designed some to help with   
(4879.304) ~~like~~ (4879.444)  
drug delivery. So they have these like the like pocket that forms when you have a cyclically symmetric complex of proteins, the pocket that forms inside of that. 


---


#### 4891.347

You can design that in such a way that it captures a small molecule drug really well and delivers it to somewhere in particular, right? So that's another application of RF diffusion that's really useful. What else? There's the binder design. Fold conditioning, which is where you can tell it like specific tertiary structures to condition on. Maybe I want to design something like a TIM barrel. I can tell RF diffusion to generate something that has the rough 3d shape of a TIM barrel. What else can I do? Can I ask what that is? Yeah. Maybe a picture would be a better way of explaining it. Maybe if we just look at a picture on Google of a TIM barrel, it's just T I M and then barrel,   
(4935.411) ~~like a,~~(4935.731)  
like a barrel that like you put water in or something. 


---


#### 4938.992

Let's see if I can find a good picture of one. If you haven't found one. Go. Yeah. Here's a good one. So it's   
(4943.813) ~~like this,~~(4944.153)  
it has   
(4944.714) ~~like~~ (4944.874)  
beta sheets in it. and they form this   
(4947.633) ~~like~~ (4947.914)  
sort of barrel-shaped protein. Let me see if I can send this to you so that you can see it. Yeah, I've got a couple pulled up as well. Okay. We can add one to the...   
(4957.718) ~~I mean,~~(4957.938)  
I can even share here in the moment just to capture what I'm looking at. Yeah, maybe let's share. Do that. So this is an 8. And if you turn this sideways, yeah, if you turn this sideways, it should look kind of like a barrel. 


---


#### 4970.183

#### 5016.482

There's two different proteins that are interacting with each other, p53 and mdm2. And if I want to design an inhibitor for this, maybe I could   
(5025.366) ~~like~~ (5025.526)  
could extract the motif corresponding to the p53 peptide and then use that to design a new protein, scaffold that with the motif scaffolding. And then I can optimize it using partial diffusion and ligand and PNN to design sequences that have favorable chemical properties. And then I can check and see using the LIS score from alpha-fold multimer how well my new protein interacts with MDM2 or p53.   
(5059.592) ~~These are so technical, I hate to just read these off, but I feel like I'm just going to go into the weeds and talk about a bunch of really specific proteins and domains and stuff.~~(5068.994)  



---


#### 5069.014

I don't know if that's very interesting. The sort of conceptual loop,   
(5073.195) ~~I think,~~(5073.395)  
is really interesting. And if I'm getting it, it's like, okay, we have an interaction that is problematic. we want to interfere with it one way or another. We can   
(5083.858) ~~like~~ (5084.058)  
cap the one thing or cap the other thing. And so there's this kind of cycle of generate a 3D structure. That's one model. Generate a sequence to do that. That's another model. Refine those. That's,   
(5096.503) ~~I guess,~~(5096.763)  
yet another model to look for various refinements or   
(5100.745) ~~kind of,~~(5101.005)  
as you said, chemical, favorable chemical properties, same thing? No, you don't need another model for that. You can just RF diffusion and ligand and PNN, you can do it with those two. 


---


#### 5110.696

You don't need anything else really. So RF diffusion designs the structure and then ligand and PNN designs the sequence for that structure that will fold into it so that you have something you can actually go and synthesize in a lab, right? You need a protein sequence to synthesize to get the protein structure because RF diffusion just works at the level of structure. It doesn't know anything about sequences. And then you're validating this to the degree that you can validate it before you're actually doing any actual lab work,   
(5139.045) ~~um,~~ (5139.145)  
with something like multiple and looking for a high score there.   
(5144.01) ~~How,~~ (5144.27)  
so how quick does this happen? It seems like we're talking orders of magnitude speed up compared to the pre AI way of doing this. 


---


#### 5155.341

And how accurate is it? Yeah, I mean, RF diffusion, like I can generate a single backbone in a minute, even like a pretty big one. It just takes a minute to generate a backbone. And if you have a really good GPU, that's way faster, right? If I'm just working on my laptop or something,   
(5171.175) ~~like~~ (5171.295)  
I can generate something in just   
(5172.555) ~~like~~ (5172.695)  
a minute. And then ligand and PNN is significantly faster than that. So like designing the sequence for the 3D structure is actually really fast.   
(5180.199) ~~So, you know,~~(5181.419)  
like per protein. And per sequence, it's less than a couple of minutes to do that whole thing. And so I can design hundreds of thousands of backbones and then design hundreds of or thousands of sequences for each backbone with ligand and PNN. 


---


#### 5197.219

So it's pretty fast and pretty computationally efficient. And they've made some improvements to RF diffusion to reduce how many time steps you need to actually get a good structure out of it. And time again, when they actually synthesize these and check for   
(5210.382) ~~like~~ (5210.622)  
thermostability or specificity or binding affinity, very often they're very high. And if I have   
(5218.464) ~~like~~ (5218.584)  
low thermostability or low binding affinity or low specificity, very often when I use these models to improve that, they improve it dramatically. So they're pretty effective, and they're not perfect, but they're pretty good. It's not a hard thing to do to design a protein with RF diffusion and then design a sequence with ligand and PNN and get something that really does fold into that structure with high confidence or that really does interact with my target protein with high affinity and specificity. 


---


#### 5251.439

Yeah. So how does this then fit into the broader like validation loop. You have this one thing you're like, going back to our cancer example, right? Oh, this part of the cancer cell interacts with this part of the immune cell and disables it. So we want to put essentially a physical cap on that thing. So that is blocked and that can't happen and the cancer can get Okay, cool. So I'm going to generate potentially thousands of shapes, thousands of sequences per shape, then potentially run millions of things through an alpha fold multimer, getting scores. And then what do I do at the end of that? Do I take like the top hundred and go actually try them in a living cell? 


---


#### 5295.226

Yeah, exactly. And so this seems, and you're saying they tend to work. And then I guess we also have questions of like side effects would be another big downstream question, right? We don't know what else this thing could do when put into the full environment of the cell.   
(5311.627) ~~Well, that's where this,~~(5312.228)  
the specificity comes in, right? Generally speaking, RF diffusion is capable of designing binders, for example, with really high specificity. So they bind to the target and pretty much only bind to the target. Yeah. And that's a really good thing, right? Because   
(5327.014) ~~if you have a, if you,~~(5328.455)  
design a binder that just interacts with a whole bunch of other stuff, it may never make it to the target. 


---


#### 5333.336

It may cause other side effects, like you're saying, have off-target effects. But yeah, RF diffusion is pretty capable of designing really high-specificity binders. The motif scaffolding, there's more nuance there because you're performing surgery on proteins and pieces of proteins. And so that can get a little more nuanced and a little more complicated. But if you're just designing a binder, with RF diffusion, it's pretty easy to design one that has really high specificity and that doesn't have a lot of off-target effects and stuff. What's the bottleneck on this process? Is it identifying targets? Especially if you can design things that are that specific and they don't have much in the way of other knock-on effects.   
(5376.738) ~~I mean,~~(5376.918)  
it seems like we should be curing a lot of diseases pretty quick here. 


---


#### 5380.761

I think, I mean, diseases are pretty complicated and sometimes it's not just one thing that you're targeting. Sometimes it's multiple targets and multiple kinds of interactions. And so you have to think in terms of   
(5392.571) ~~like~~ (5392.791)  
entire   
(5393.472) ~~like~~ (5393.632)  
protein interaction networks or even like interaction networks that involve other molecules as well and modulating those in very specific ways. And often figuring out what parts of a protein interaction network to change or to modulate and how to do that, like what sort of changes you should make to this interaction network, that's a pretty complicated problem. And so I think part of it is   
(5418.048) ~~identifying, like you said,~~(5420.049)  
identifying targets or identifying specific targets within an interaction network, because some of the interaction networks can get really complicated. 


---


#### 5428.613

And figuring out which parts of them to modulate is not an easy thing to do. And then Computationally, there isn't much of a bottleneck. If you just have a good GPU, you don't really need multiple GPUs even. You just have a good H100 or something. You can get a lot done with that.   
(5445.852) ~~You can get quite a lot done with that~~(5447.532)  
with RF diffusion and NPNN. The hardware requirements are not very taxing.   
(5454.295) ~~I mean,~~(5454.475)  
They're probably a little less efficient than I would like them to be, because   
(5460.564) ~~I guess~~(5460.804)  
most average people are not going to have access to an H100. A lot of people are going to be using much lower tier GPUs and stuff. 


---


#### 5472.047

But like RF to Fusion, for example, there's a Colab notebook that you can run on a T4. You can run it in Google Colab. And it takes a little while. It's not as fast. The computational bottleneck is not a huge bottleneck right now.   
(5485.938) ~~I think~~(5486.218)  
it could be a little better, but   
(5488.019) ~~I mean,~~(5488.22)  
the models aren't huge models. These aren't like billions of parameters, right?   
(5493.003) ~~I think~~(5493.243)  
RF diffusion has a couple hundred million parameters or something like that, or an alpha fold, same thing.   
(5499.607) ~~Like~~ (5499.787)  
it's a couple hundred million parameters or something. So they're not really big models that require really excessive hardware to do the computations. And   
(5508.392) ~~I think~~(5508.633)  
the slowest part of that pipeline. you like design binders or design motif scaffold with RF diffusion or partial diffusion or what have you and then designing the sequence with   
(5520.112) ~~like~~ (5520.252)  
protein NPNN or ligand NPNN and then validating with   
(5523.634) ~~like~~ (5523.754)  
alpha fold or alpha fold multimer, the slowest part in that whole thing is actually the alpha fold multimer part or the alpha fold two part where you're validating and   
(5533.418) ~~like~~ (5533.558)  
predicting the structure of whatever you've generated and designed with the other two models. 


---


#### 5539.828

That's actually the slowest part in the whole thing. If you're able to predict a lot of structures with AlphaFold, then you're fine. There's no real computational bottleneck there. And as far as   
(5551.33) ~~like,~~ (5551.55)  
why are we not curing a bunch of diseases? A lot of this also has to do with how long it takes to get these things to market. and the traditional system that's set up right now for drug discovery and protein therapeutic, it's hard and slow to get new things through.   
(5571.281) ~~Like it's a~~(5571.801)  
very slow system. And   
(5573.381) ~~I think~~(5573.721)  
it wasn't designed for high throughput methods like this. It wasn't designed for   
(5580.423) ~~like~~ (5580.584)  
large high throughput methods. And it just, it takes a lot of time to get a new drug or a new protein therapeutic through and approved and get it through all the testing, like the different clinical testing phases and stuff like that. 


---


#### 5595.493

That's part of it. That's probably a big part of it. Are we like stuffing the pipeline at this point with new things?   
(5602.077) ~~I mean,~~(5602.237)  
it seems like the biggest reason that this used to be a hard thing, of course, it's like slow and there's a lot of like safety, perhaps redundant steps in there, especially if you could say, hey, we have like very high confidence that this is a highly specific thing.   
(5616.78) ~~I mean,~~(5616.92)  
that would really do a lot to inform   
(5620.241) ~~the~~ (5620.401)  
what the safety profile might be. But even if you, not even if, but in the past, it's like the biggest problem was like either it wouldn't work, right. Or it would have side effects that were like intolerable. 


---


#### 5633.005

And if you could take both of those things, not entirely off the table, but if you could   
(5636.827) ~~sort of~~(5637.067)  
say, Hey, we can be much more confident now, seemingly like at least in order of magnitude, more confident that any given thing is going to do what you expect it to do and that it won't do other things that you don't want it to do. you can improve both of those by an order of magnitude, then it's your seemingly two orders of magnitude more likely for things to work, which would take you from sub 1% a lot of shooting in the dark to a lot of the clinical trials would be expected to work. Is that the era that we're entering into now where clinical trials should go from like roll of the dice to you be more like disappointed when they don't work. 


---


#### 5678.091

Yeah.   
(5678.331) ~~I mean,~~(5678.551)  
I think we're definitely moving into an era where all this stuff is going to speed up a lot. And   
(5683.813) ~~I think~~(5684.133)  
so there are   
(5685.353) ~~like~~ (5685.533)  
a lot of situations where you want to understand more than just a static structure. Like we've been talking about   
(5691.415) ~~like~~ (5691.575)  
having models that give you more dynamic information and stuff like that. And those are so recent that they haven't really been adopted by a lot of people. yet. And I think once those get used more, that'll speed things up a lot and improve things a lot as well. But yeah, I think also part of it is just adoption. A lot of researchers are not using this stuff yet because it's so new. 


---


#### 5715.528

And a lot of researchers don't understand how to use these models effectively or how to use them at all. It does seem to be quite a different skill set.   
(5723.57) ~~I mean,~~(5723.93)  
I've actually studied chemistry as an undergrad. It really is. Yeah. And the kinds of things that I was taught to do were like not at all running the loops. There were no notebooks involved or no collab notebooks involved. It was like physical techniques for separating chemicals from one another was a big part of where the time went. Yeah. And that's a whole other thing too, like drug synthesis and small molecules is like a whole other story that we can get into. But because there are like really interesting diffusion models out for those as well that'll generate molecules with specific properties. 


---


#### 5756.583

But Yeah, I mean, it's a very new and a very unique skill set that there aren't a lot of people that are training people to do this. There isn't a ton of information out there about how to use them. To some degree,   
(5770.934) ~~I mean,~~(5771.114)  
there are some platforms that are popping up and some different tools that are popping up that are making these things a lot more accessible. One that I would mention is 310AI is working on a tool that they're calling Copilot. And   
(5786.158) ~~it's essentially,~~(5787.099)  
it's like a chat interface that uses tools.   
(5791.761) ~~So it,~~(5792.242)  
you can talk to it in natural language, like you talk to the chat GPT or something. And then   
(5798.305) ~~it,~~ (5798.345)  
it knows how to use   
(5799.906) ~~like,~~ (5800.146)  
like function calling   
(5802.307) ~~to,~~ (5802.748)  
to use other models as tools. 


---


#### 5806.19

So you can say, generate a protein with such and such property. And then it'll use a particular model to do that, generate some protein with that particular property. And then you can say   
(5816.93) ~~like~~ (5817.09)  
increase binding affinity with such and such protein and it'll modify your protein for you to increase the binding affinity or something. Or you can say dock this small molecule to this protein and it'll call on diff doc and dock the small molecule to the protein for you and then return that. And that's all using like a chat interface, which is making a bunch of these models a lot more accessible to people. And I think that's going to have a huge impact in the near future. 


---


#### 5844.107

So. Depending on how good that gets and how fast it gets really good, that's probably going to change things substantially. And right now, it's pretty good already. And it uses a pretty wide range of tools for different things. It'll use protein MPNN or ligand MPNN to design sequences for a structure. I'm not sure if it uses RfDiffusion yet, but they probably are going to start including RfDiffusion and some other models as tools for it as well, because they just keep adding more tools to it, more models that it uses as tools. And   
(5878.938) ~~I think~~(5879.338)  
once they have a good   
(5881.099) ~~section or a good~~(5882.139)  
selection of tools for it to use, that'll be really good. And that'll lower the barrier to entry for a lot of people. 


---


#### 5889.847

Because right now you've got to go through this like somewhat complicated process of setting up these models. And   
(5896.432) ~~you have to know,~~(5897.192)  
you don't have to know a lot of coding, but you do have to code some and you have to understand how to set these things up   
(5904.217) ~~in,~~ (5904.317)  
in   
(5904.777) ~~like~~ (5904.937)  
a conda environment or something like that a lot of times. And so if you're not coming from   
(5909.42) ~~like~~ (5909.56)  
a programming background or you don't have some experience with programming, like a lot of these models are   
(5915.825) ~~kind of~~(5916.085)  
hard to touch. They're hard to use because   
(5918.607) ~~you.~~ (5918.667)  
You can't really use them unless you know a little bit of coding at least. But so 3.10 AI, 


---


#### 5923.604

I think is going to change a lot of that and make a lot of these models a lot more accessible over time and really increase adoption of these techniques. And   
(5931.591) ~~I think~~(5931.871)  
that's going to be really big and important because adoption right now is pretty limited,   
(5936.796) ~~I would say. I mean,~~(5937.757)  
just using a really simple metric by if you just look at   
(5942.261) ~~like~~ (5942.421)  
how many views a YouTube video on RF diffusion gets. It's not that many, right? There aren't that many people watching. This is going to be the one that goes viral and changes it all. I hope so. That would be great because adoption is going to be big. I think because the more creative people you get using these things, the more you're going to see creative uses of them and like novel approaches to solving problems that people weren't even thinking of before. 


---


#### 5968.679

Like when have you been able to design proteins that build out complicated protein interaction networks using binder design and motif scaffolding. That's just so brand new within the last couple of years that the adoption just hasn't caught on yet. So hopefully more people will start experimenting with these models and really learn how to use them well. And we'll see a lot of really interesting novel techniques popping up in the near future. Yeah, that's pretty remarkable. So it seems like the problem then shifts to the, or maybe it was always there in the first place, but if it is the case that given a target, we can pretty reliably and   
(6010.405) ~~like~~ (6010.545)  
even relatively computationally efficiently come up with something that will hit the target, not hit other things, not cause a lot of collateral damage. 


---


#### 6020.512

Now it's like target identification becomes the thing that really. matters the most. And this seems like it's happening in a lot of areas at once. Certainly,   
(6028.945) ~~I mean,~~(6029.345)  
terrible analogy, but to thinking about a military environment, we've got really good missiles that can hit very precise targets, but then the targeting obviously becomes the high stakes decision. And   
(6041.111) ~~I mean,~~(6042.231)  
in lots of just business operations context too, right? Figuring out the right thing to do is often the hard part. So what do you think are the prospects for that sort of thing? I've been   
(6052.917) ~~kind of~~(6053.137)  
working through this and thinking, we've got quite a tech stack for, obviously we can sequence lots of DNA. We can also pull out from an individual cell now, what was the state of the transcriptome, what genes were being expressed at any given time, what proteins were being created. 


---


#### 6073.851

I don't know quite the degree to which we can do that with small molecules, with a really localized sample, But it seems like   
(6081.469) ~~we're,~~ (6081.669)  
we've got like a lot of ability to generate a lot of data and to probably then create a foundation model of some sort. This is   
(6091.797) ~~kind of~~(6091.977)  
where Evo, I sort of sense is going, even though that's not even doing all this stuff yet, but already,   
(6098.322) ~~I mean~~(6099.483)  
with, let me just give my understanding of Evo and you can correct me if I'm wrong, but basically they're training a language model on DNA sequences. purely bacteria and phage DNA from what I understand. And yeah, I was a little disappointed by that. 


---


#### 6117.491

But I think part of their reason for doing such a like specific selection was for safety reasons. I think they're like trying to be a little cautious about what they train on and what the model is capable of doing for for safety reasons. But I was a little disappointed that they only trained on that data, for sure. Hopefully, there'll be another version at some point that's train on other data as well, but yeah. I'm sure there's a lot more to come.   
(6143.633) ~~You kind of glitched on me for a second, but~~(6145.233)  
so they train on all this data. Now they can generate sequences in the same way that a language model can generate text, right? In autoregressive, byte-by-byte, base-pair-by-base-pair generation. 


---


#### 6159.82

And then there's these really interesting things that they can do downstream of it where, for example, a gene essentiality score or test Basically, if you change a sequence in a particular gene and generate from that changed sequence It seems that the model has developed a sort of, as we've talked about a couple of different contexts, this sort of higher order understanding of how things fit together, such that if you do make a change to something that really matters, then you see   
(6196.375) ~~sort of~~(6196.615)  
an unraveling of the later generation. You see a very high perplexity downstream of this changed sequence. And that reflects the fact that, hey, if you've changed that sequence, I can't really make any confident predictions now because we're   
(6212.861) ~~sort of~~(6213.181)  
outside of the set of things that can work. 


---


#### 6216.542

And so once you change that, it's all kind of noise. Whereas if you change something and predictions remain confident downstream, then you infer that must not have been super important. That was an area that more easily could be, change could be tolerated in that particular sequence because, and we can infer that from the fact that it continues to make confident predictions downstream. That's pretty remarkable stuff that suggests to me that especially as we scale up the data set a lot more, which in this one was 300 billion.   
(6250.533) ~~I mean,~~(6250.673)  
that's not nothing, but it's not much compared to what we could easily imagine doing. Certainly not much compared to the 15 trillion tokens that Mediterranean Plasma 3 on, but then also like more modalities, right? 


---


#### 6261.197

I mean, we're seeing this in the language models where you can have obviously language integrated with image and plenty of other things. Audio now it fits into Gemini 2. It seems like you   
(6270.32) ~~sort of~~(6270.56)  
imagine from just the DNA to   
(6274.062) ~~sort of~~(6274.402)  
the DNA and maybe the transcriptome or the proteome or whatever the sort of state of a cell is. You can even imagine scaling this up another degree to   
(6285.083) ~~sort of~~(6285.304)  
the systems level too. But to learn to predict the next state from the current state seems like we're getting really close to being able to do that. I would   
(6298.57) ~~kind of~~(6298.79)  
expect that in the next couple of years at most, we would start to see large scale foundation models for biology that would predict like how a cell will evolve through time, how a system level description would evolve through time. 


---


#### 6314.702

And then you can start to do these like counterfactual hypothetical perturbations and see, okay, if we change this, then how will that make things evolve? If we change this, how will that make things evolve? And so then   
(6326.045) ~~I guess~~(6326.265)  
what we would expect to be learned by those systems is what is now the black box, right? Of all these like interactions that we have only mapped out like whatever, 5% of. And then you could even imagine a situation where you start to do interpretability techniques on digital neural networks to then figure out what the actual pattern of interactions is in the actual biological systems. So is that where this is going over the next couple of years? 


---


#### 6354.376

I mean, and then it seems like if we can achieve that, then you kind of have a fairly closed loop of, okay, we can now identify good targets at a pretty high rate. We can identify or design interventions that are pretty likely to be successful. The like specificity is already high.   
(6372.805) ~~I mean, it's,~~(6373.705)  
we're entering into sort of a super steep part of the S curve in terms of not just   
(6379.027) ~~like~~ (6379.167)  
understanding biological systems, but really being able to intervene in them. And it just seems like a totally different regime that we're headed for. So is that what you basically expect to see over the next couple of years?   
(6389.971) ~~I mean,~~(6390.171)  
I hope so. I hope that all of that comes to reality or comes into existence. 


---


#### 6394.513

Sorry. We pause for a second. I need to get some water. OK, hold on just a second. We're back. OK,   
(6400.544) ~~I think we're~~(6400.905)  
I think we're all set. Yeah. OK, I'm feeling a little better now. So where were we?   
(6406.367) ~~What were we talking about?~~(6407.268)  
You were hoping that my seemingly I'm like extrapolating from where we are and I'm also   
(6413.156) ~~sort of~~(6413.536)  
mapping what has happened with language model foundation models onto the biological domain and feeling like it's about to get crazy. So you're hoping that happens.   
(6425.205) ~~I, yeah. I mean,~~(6426.646)  
I think it's about to get crazy for sure. I think like we're fast approaching a scenario where all of these technologies are going to   
(6433.552) ~~kind of~~(6433.792)  
converge and we're going to have a lot of power over. editing and modifying our biology. 


---


#### 6440.082

I think that's a very exciting thing because there's a lot of problems that I really want to see solved in my lifetime. I think we are definitely moving in the right direction and I think we are fast approaching a situation where we can actually solve a lot of these problems. The main thing that you're talking about is this complicated hierarchical structure that's happening. The level that   
(6467.185) ~~I think~~(6467.605)  
at most of the time is at the level of molecule interactions. But you can definitely take that up another level and look at how those interactions come together in a network to create a particular phenotype or to create a particular state of the organism. And some of those states are diseased states that we don't want. 


---


#### 6496.69

Figuring out how to modify these interaction networks, I think, is somewhere that we really need to focus on a lot. And one thing that's really useful and that I really want to see pushed further is this notion of LIS score with AlphaFold and Ultimer, and seeing also things like AlphaFlow or distributional graph former generalized to complexes, to complicated complexes of molecules, and not just one or two proteins or something. I really want to see more progress happen there because once we understand all of the interaction networks and we're able to modulate them in very specific ways,   
(6539.118) ~~we're going to solve a lot of problems,~~(6540.779)  
a substantial amount of problems. Modeling these interaction networks is becoming possible now. 


---


#### 6547.042

I think before alpha-fold multimer, and before some of these other docking methods, and before RosettaFoldAllAtom came out, we really didn't have the tools to model all of these different interactions. But we have very recently just hit a point where we do have most of the tools that we need, if not all of them, to model all of these interactions. And once we implement something like alpha flow or distributional graph form for complicated complexes of molecules, that's really going to be pretty substantial. And   
(6583.324) ~~I personally,~~(6584.124)  
I'm not sure how I would approach the problem of determining what specific interactions or interaction networks to modulate.   
(6594.971) ~~I Like,~~(6596.895)  
I personally, like, that feels like such a big problem to me. 


---


#### 6601.236

But I also know that there are a lot of biologists that know specific interaction networks they want to modulate, and they want to modulate them in very specific ways. And there's a lot of that. And now we can do that. I think we just need to get these tools into the hands of those biologists and make them really accessible. Because they're not super accessible yet.   
(6626.769) ~~They are kind of, right? I mean,~~(6628.49)  
like a lot of them are open source and they're out there and you can get the model weights and a lot of them have the training code and the inference code and all this stuff available. But probably your average biologist is not going to know how to use those tools right now. 


---


#### 6644.582

So making them accessible and easy to use is really where a lot of the work is going to be as well. Because there are a lot of people that want to do these things, but   
(6655.791) ~~they don't~~(6656.331)  
they haven't quite gotten to the point where they've adopted all of these tools yet. And also figuring out how to use them all in tandem with each other,   
(6666.18) ~~right?~~ (6666.401)  
Because you don't want to just use one of these models. You want to use multiple and use them all together to solve a problem. And so that requires you to learn   
(6677.284) ~~like~~ (6677.404)  
multiple different models and how they work and how to use each one of them. And that's not an easy thing to do for a lot of people. 


---


#### 6684.389

Yeah.   
(6684.649) ~~The, I mean,~~(6685.089)  
this is an issue in AI, even in much more,   
(6688.011) ~~you know,~~(6688.351)  
simple use cases of just using chance UPT effectively, the sort of diffuse, the technology diffusion through society   
(6694.635) ~~is,~~ (6694.795)  
is really the big bottleneck I would say right now to when people say   
(6698.698) ~~like,~~ (6698.818)  
why hasn't, if change UPT is so great,   
(6700.619) ~~like~~ (6700.739)  
why hasn't it,   
(6701.519) ~~you know,~~(6701.78)  
changed productivity all that much? It's like, people are not using it nearly as much as they could is one really big reason. So a huge reason. Yeah. If I had to kind of map out the story of the next couple of years, as I understand it, or as I'm kind of piecing it together from everything that you're teaching me about, it is right now we have a big backlog of targets. 


---


#### 6722.411

And we have a pretty robust new set of tools that used together can design things that will hit those targets and not create too much collateral damage such that it's not super hard. It's hard to learn to use the tools. But once you have the skill set, it becomes relatively easy to take a target and crunch through a bunch of iterations and come to a bunch of candidates. And those are likely enough to work that we should start to see serious acceleration of the ability to find the solutions to these well-posed problems. And then   
(6770.927) ~~sort of~~(6771.127)  
in parallel, we should probably also expect that Evo 5 or whatever, Evo 4 will be capable of dramatically better holistic modeling of the overall networks. 


---


#### 6788.057

And that will then, once we sort of deplete the current set of targets, that have been painstakingly worked out through non AI methods   
(6800.069) ~~sort of seems, I don't know.~~(6801.01)  
Why does it always seem like it happens at the same time? It's always these sort of gradual overlapping curves, but my gut says we've got a few years in front of us of. depleting the current, or not depleting, but like picking the sort of low hanging fruit of, hey, we've got all these targets out there and now we've got good methods to hit those targets. That's going to take a while for people to learn the tools, do it, obviously validate it, run clinical trials going in lots of different areas. 


---


#### 6825.959

And then as the sort of current backlog gets worked through, it's probably a better way to phrase it.   
(6831.301) ~~Right~~ (6831.441)  
around the same time, I sort of expect that all of a sudden the tension will turn to Oh my God, now we have these foundation models that   
(6839.242) ~~kind of~~(6839.483)  
model the whole causal graph in all of its crazy complexity. And now we're actually going one level out and saying, now we can apply similar computational techniques to the identification of the targets. And we'll do that in   
(6856.537) ~~sort of~~(6856.738)  
a similar way of being like, okay, I want   
(6859.74) ~~this, this is~~(6860.501)  
what's happening and I want to prevent it from happening. or this is what I want to happen proactively that isn't currently happening. 


---


#### 6867.565

Let me just kind of brute force my way through a bunch of perturbations to the, and of course we can get better than brute force too, but even just imagining a   
(6876.81) ~~sort of~~(6877.07)  
several couple generations down of Evo, it seems like make a tweak, see what happens is going to be so radically accessible from a computational perspective that We'll then also just have this explosion of like quality targets to identify.   
(6891.606) ~~And yeah, I mean, what do you think the world looks like as all that happens? What is, it seems like we may be not super far from a,~~(6901.373)  
this is not, we're not even in a world here of like an, any sort of AGI, right? 


---


#### 6905.255

We're talking like, these are still tool simulated simulation and tool type things that people would be using that we're not assuming anything here about AI agents doing the work. Although you did have a little bit of that with the 310 co-pilot. But is there anything that I should be like reining in my expectations on?   
(6924.874) ~~I mean,~~(6925.074)  
are there things about like one tweet that I sent you was around to what degree can these things handle   
(6929.997) ~~sort of~~(6930.377)  
point mutations or whatever? And there's maybe individual idiosyncrasy becomes a really hard problem at some point, but like how far does this paradigm that I'm sketching out extend, do you think? And what limits does it hit? Yeah. 


---


#### 6944.486

So I think, so just briefly on like point mutations or like more complicated mutations where you mutate multiple things and just predicting how positive or deleterious that mutation or set of mutations might be on the protein or something. That's a capability that ESM has, and that's already two or three years old at this point. And Evo does it better. They got state-of-the-art performance with Evo on predicting which mutations were positive and which mutations were negative and which sets of mutations were positive or negative. And you can compute   
(6984.17) ~~a few different things,~~(6985.052)  
a few different kinds of scores that tell you about this. you can actually build out evolutionary trajectories to show over time how things are likely to evolve based on how positive or negative the impact of a mutation is on protein or something or DNA sequence or whatever. 


---


#### 7003.123

And Evo, they got state-of-the-art performance on this. And that's actually, they also did this with alpha folds. I think they called it alpha missense or something like that, where they just,   
(7015.308) ~~I think they, what did they do it for?~~(7016.629)  
Did they do it for   
(7017.759) ~~I think~~(7017.939)  
they did it for all the human proteins, but maybe it was a bigger dataset. I can't remember. But they predicted all the single point mutations and all the effects   
(7026.353) ~~that~~ (7026.453)  
that those have. And that's actually not a hard thing to do. So mapping out how a mutation affects a protein or DNA or something, and the course of evolution that's likely to occur, that's actually pretty easy to do now. 


---


#### 7041.441

And then as far as... I also want to draw attention to another project that I'm aware of. It's not a model per se, but they are using... I think they are using GPT-4 They may have trained their own in-house model. I'm not sure. But there's a company called Future House, and they're designing an agent, an autonomous agent, that will do a lot of this research for you. And it'll do things like literature search and review, and come up with hypotheses of different kinds of interaction networks that you might want to modulate or different targets that you might want. And it'll do this and it'll do it pretty well. And that's a pretty new thing that just started happening like last year, 


---


#### 7090.842

I think, maybe late last year. And they're getting pretty good results with that. And that's actually using an LLM   
(7098.324) ~~like~~ (7098.504)  
as the base,   
(7099.604) ~~right,~~ (7099.824)  
to build an agent to do this research. And then   
(7103.789) ~~I think~~(7104.109)  
they're also building an autonomous lab that drives itself. So once the agent comes up with hypotheses or targets or what have you, the lab is autonomous as well. And that's a pretty exciting direction.   
(7118.896) ~~I think~~(7120.037)  
that, coupled with some of these more specific tools to perform these fine-grained operations on proteins and small molecules and DNA and RNA. When those two kind of converge, that's going to be a really big deal. And I see that happening in the next year. 


---


#### 7138.109

The progress that they're making at future houses is really impressive, I think. So that would also be something that people should definitely look into. And I think your timeline is within a couple of years for sure. I don't think it's going to be that long before we start seeing substantial progress and changes.   
(7157.309) ~~I mean,~~(7157.569)  
OpenAI just partnered with Moderna, right? Yeah. Hundreds of GPTs, just the beginning. And   
(7164.154) ~~I think~~(7164.434)  
that also is   
(7165.375) ~~like~~ (7165.495)  
a paradigm that's going to match well with these other more specific tools, because when you enable an agent to use tools, you unlock a lot of possibilities, right? When you enable something that can review thousands of research articles, then develop targets or hypotheses to test, and then can call on these specific tools to design molecules or proteins or nucleic acids to perform these specific functions or hit these specific targets. 


---


#### 7201.243

That's going to move really fast. And   
(7203.564) ~~I think~~(7203.864)  
I'm excited. I'm also a little nervous because I think there's a lot of a lot of potential for misuse and the wrong hands, like the sort of things that you can accomplish will be amazing and beautiful. And we're going to see a lot of health problems just disappearing. We're going to see lifespan extended, and that's going to   
(7226.122) ~~really increase or~~(7227.343)  
really improve the quality of life for everyone. But also we do have bad actors in the world. And that is something I worry about for sure, because in the wrong hands, we could be looking at very dangerous things as well. And so having some kind of oversight for these things is very important. 


---


#### 7244.48

Because, I mean, we're looking at moving into an age where you could target a specific group of people based on their genetics or something. That's both immensely useful and also very dangerous. I have a lot of faith in the people that are working on these things. Like the people that are building these models and doing this research are really good people with a lot of really good intentions and a lot of know-how and experience. And that to me is very reassuring, but there's always some random jerk that has the potential to mess it up for everyone. We have to be prepared for that. Yeah, no doubt.   
(7285.898) ~~I mean,~~(7286.158)  
preparing for this, definitely one of the major updates that I've made is that when people talk about the bio risks from AI, the conversation that I've heard most of has been like, how does it compare to Google? 


---


#### 7302.637

How does GPT-4 compare to Google? Does it make it easier for you to get certain information or figure out how to do certain things. And in familiarizing myself to the degree that I have with all this technology, it's   
(7315.358) ~~like,~~ (7315.538)  
that all of a sudden feels very quaint already. It's like, this is not a question of comparing to Google. This is like generating entirely new stuff. And I looked back not long ago at the list of mass extinctions in the history of the planet and what caused them. Of course, some were caused by totally exogenous shocks like asteroid hits the earth. But the first one on the list on Wikipedia is the oxygenation of the atmosphere. 


---


#### 7348.326

And it's simply that something kind of pops up and either itself, nobody knows how to eat, or it creates some waste product that,   
(7359.574) ~~you know,~~(7359.814)  
that nobody's prepared to deal with. And what we now breathe and depend on was at one point, the cause of a mass extinction event. I kind of try to keep these   
(7370.98) ~~like,~~ (7371.18)  
zoomed out perspectives in mind. And it does seem   
(7373.881) ~~I mean,~~(7374.201)  
tell me if you think there's any limitation to this or whatever. But with this sort of brute force search through biological space, it seems like there's not really anything conceptual that I could identify preventing – talk about gain-of-function type research on a totally different level. Things that nothing can eat. 


---


#### 7399.007

That's like the most dangerous stuff, right? It's the stuff that nobody can break down. And I gather that trees were essentially at one point that too, right? Before something developed that could break down the hard fibers. tissue of a tree, it was just piling up. Globally, I understand that's basically where a lot of coal came from, is that trees would fall, nothing could digest them, and so they would just   
(7422.679) ~~sort of~~(7422.939)  
collect and eventually they turn into coal. I'm sure there's a lot of different stories of coal formation, but these moments of something that nothing is really prepared to deal with, those seem like the really dangerous things. And I don't know how you prepare yourself for that. 


---


#### 7436.967

I think there are multiple things that we can do to help   
(7440.349) ~~prevent~~ (7440.769)  
prevent some of these bad things from happening. And   
(7444.375) ~~I think~~(7444.655)  
we're going to need to rely on the models that we build, especially the agentic models that we build, to help guide us in some of this. Because at some point in the near future, we're going to have agents based on really robust language models or something similar, and they're going to be able to review thousands of research papers and do tests in a lab on things, take in an amount of data that we can't really take in, right? That no human or even group of humans can really take in and process and digest and use. 


---


#### 7483.474

Like the scale is going to be much larger than a human can really work with. And so we're going to have to rely on some of our models to help guide us. And also,   
(7496.638) ~~Like,~~ (7496.778)  
going back to how does it compare to Google, I think another argument that could be made for why not to worry about some of these things is, okay, maybe I can get on my computer and design some new thing that was really toxic or something, but I still have to go into a lab and synthesize all that stuff. And a lot of that part of the process is very highly regulated and watched, right? I can't just go get a bunch of random chemicals and build this stuff in my house, right? 


---


#### 7529.716

Like it's harder to do than that. And like synthesizing proteins is, it's a non-trivial process. So   
(7536.8) ~~like~~ (7536.96)  
a lot of the worry, I think of, Oh God, we're going to have an AI that designs a deadly virus or a bioweapon or something. A lot of that is really overblown, especially at the moment. And   
(7548.606) ~~I think~~(7548.846)  
a lot of people overlook the fact that computationally designing something computationally designing a molecule is just one step in the process. You also have to do all the lab work and synthesis and work on some kind of delivery mechanism. And this is all stuff that's non-trivial to do, and that helps prevent bad actors from actually going through with some of this stuff. 


---


#### 7575.19

Now, there may be like state-sponsored bad actors with access to good labs and lab equipment will circumvent a lot of that. But when you're working at a state-sponsored level, that's a matter of international relations and also national security. I think that has almost nothing to do with AI. The computational design of some random toxic molecule is just one step in a complicated process, and people don't often think of that. I see a lot of very influential, big-name people in the industry who are coming from the NLP side of things and the LLM side of things, and they don't really understand the biology and the process that goes into actually making these things. I think their worry is justified, but they're also not understanding the nuances and where the dangers actually are. 


---


#### 7638.427

So I think it's important for people to keep that in mind. I think it's very important before we start getting all anxious and worried about some random person using Lama 3 to design a superflu or something, you have to remember it's very unlikely and very difficult for just a random average person to go through the entire process of designing and synthesizing and delivering some kind of toxic molecule. That's a long, difficult process that an individual would be very unlikely to be able to accomplish, even with the help of a very intelligent LLM or a very capable agent. Now, when you have larger research-oriented companies working on these things that have their own wet labs, and they're building agents to run these wet labs and to computationally design the molecules and form plans on how to use them. 


---


#### 7697.97

There, I can see, okay, we need some kind of oversight. We need some people working on how to make sure that process is safe, how to protect that information and data and equipment, right? Because there are plenty of situations where something like corporate espionage is happening and people are trying to do nefarious things with some of the technology that some of these companies have. But again, that has very little to do with the AI itself and has more to do with how we're interacting with other countries and other research organizations. So definitely we need to be developing plans for how to use and regulate and oversee like a really capable agent that is going to go through the entire process of   
(7749.008) ~~like~~ (7749.168)  
computationally designing and verifying, and then also synthesizing and delivering. 


---


#### 7754.062

And that is technology that is in existence now. We already have agents that are doing most of this process. And a lot of people are pushing for more of that, which I agree with, because we're not going to be able to solve these problems on our own. We're going to need some kind of really capable agent that can help guide us through these processes, because they're so complicated. and so difficult to understand the whole picture and all of its nuances that I don't know if humans can get there without some kind of agent helping out and helping design the molecules and producing it and delivering it and etc. I don't know if we can get there without that, but   
(7797.859) ~~I guess~~(7799.179)  
my concern is just making sure that these companies and organizations that are building this technology and using it have some people that are overseeing the safety side of things and that are concerned with red teaming and preventing things like corporate espionage and making sure that everyone that's using that technology is using it responsibly and making sure that we're   
(7820.896) ~~like,~~ (7821.156)  
that the companies are hiring, not just capable people, but also like people with good moral grounding and good intentions. 


---


#### 7830.902

Yeah. I guess that's where,   
(7832.423) ~~I mean,~~(7833.124)  
that's not even the future. That's kind of now. That's already a concern that we need to address now, because we already have agents that are doing these things. And most people don't have access to them, though. Most people don't have access to a really capable agent that can do this whole process or do most of this process. That's not something that even most companies have access to, much less individuals, because a lot of these models are closed. I could see maybe some kind of like state-sponsored group of researchers could use open source models to build something similar and do something nefarious, but that's a whole,   
(7870.679) ~~like,~~ (7870.879)  
it's a very complicated process of building such a thing. 


---


#### 7874.561

So I, and I don't know if I have a good answer for how to combat something like that or how to address something like that. I don't know if there's a good answer. to that right now. It's certainly hard to identify a more important question.   
(7886.425) ~~Do you think that the,~~(7887.206)  
do we have any read on whether offense or defense is favored here, so to speak? In the sense of for nuclear weapons, for example, if one of the major nuclear powers fires all its missiles, nobody can shoot all those missiles down. It seems to me that is an offense favored regime. And so we're   
(7905.739) ~~kind of~~(7905.98)  
stuck in this like mutually assured destruction paradigm, which is yikes. 


---


#### 7911.982

We kind of need to get to a different paradigm because we're under like real threat of nuclear catastrophe as long as we've all got thousands of missiles pointed at each other and no viable defense. I don't have an intuition if biology like works the same way or not. I think this is   
(7931.129) ~~like~~ (7931.329)  
less of a question about biology and more of a question about cybersecurity because I think it's   
(7938.109) ~~like~~ (7938.289)  
very similar in spirit to   
(7942.172) ~~like~~ (7942.352)  
cyber security. And there as well, most often the attacker has the advantage over the defender. But there are a couple of things that may change that one is really capable agents. Because if you have a really capable agent that's able to defend against human attacks that are   
(7958.843) ~~like~~ (7959.003)  
just inferior, that's going to be a really big part of protecting against bad actors. 


---


#### 7965.207

And so I guess like That's an argument for acceleration, actually, because if you have the most capable agent, then probably your defense is going to be a lot better than everyone else's. And if your agent is capable enough, it may be effective enough to ward off pretty much anything. And I don't know how soon that's going to come into the picture, but I think that is a good argument for keeping up the pace of development of LLMs and agents and things like that. There was another point that I wanted to touch on, and I think I forgot. I already forgot what it was, though. Anyway, yeah, I think the advantage of the attacker over the defender may end up shifting because of agents. 


---


#### 8006.951

We may end up having a situation where that's no longer the case. And,   
(8010.754) ~~yeah.~~ (8011.054)  
I'm a little confused about   
(8012.235) ~~why are you making a...~~(8013.957)  
Why is the shift from biology to cybersecurity? Because I'm envisioning a world where For example, Evo is open source, Llama 3 is open source. If Evo 3 is open source, then we start to, at some point we enter into a regime where, yeah, it may not be easy. It may be,   
(8033.322) ~~you know,~~(8033.742)  
hard for one person, but at some point it does get like lower than state actor level where somebody could launch some crazy attack and then it's okay. If you create some superbug with certain properties, Can we defend against it? 


---


#### 8050.554

I'm a little bit unclear as to how you're, I'm not sure if you're like equating that to cybersecurity or saying that's a primary somehow.   
(8057.357) ~~No, I guess, no,~~(8058.238)  
I think that's a good point. Yeah. Because if you develop some kind of,   
(8061.939) ~~I think,~~(8062.239)  
I guess a virus is probably as good an example as any, but let's say you develop a virus of some kind that targets a specific population. Developing a cure for that traditionally has been a very slow process. And like the fastest that we've ever done it was probably COVID. And that still took some time, right? And on the other hand, there is recent work that came out of, it was the University of California, but I'm not sure which one. 


---


#### 8090.288

They recently published some research about like universal vaccines. And they're able to design a vaccine that was like applicable to a wide range of mutants of a virus. And they said that the technology or the method was highly transferable to other vaccines. And so there's no reason that this can't be applied to   
(8108.906) ~~much~~ (8109.046)  
any vaccine to develop universal vaccines against all variants of a virus, or most variants anyway. So that'll be helpful. That'll be good for   
(8120.494) ~~defense sort of things.~~(8122.516)  
And then as far as,   
(8123.817) ~~I don't know,~~(8124.177)  
I also wonder about the applications of certain AI models to developing defenses, but I'm not sure.   
(8132.123) ~~I mean,~~(8132.963)  
it's a   
(8133.343) ~~very complicated or~~(8134.985)  
very complex topic that   
(8136.566) ~~I don't~~(8136.806)  
some of the new things that are coming out feel like they might be the answer, but it's a little too early to tell. 


---


#### 8144.451

That's definitely a, that's a very good data point.   
(8147.732) ~~I mean,~~(8147.932)  
my kind of default would be just to think I have three kids and I'm no expert in how babies develop in the womb, but it's definitely clear that a lot of things have to go right. Like an unbelievable number of things have to go right in the proper sequence. At any point, if something goes wrong, like that could be the end of it. Yeah. My general default model would be like, a lot of things have to go right and only   
(8174.346) ~~kind of~~(8174.566)  
one or two big things would have to go wrong. And so it seems like there's a lot of surface area to defend. 


---


#### 8181.156

And a lot of kind of places that could be attacked. But then, hey, if you can make a universal vaccine, then all of a sudden that does start to look quite a bit different.   
(8192.259) ~~So yeah, boy. Yeah. I mean, it's~~(8194.341)  
and I think you're right also to say a big part of this does seem to be   
(8197.462) ~~sort of~~(8197.743)  
what is the prevailing   
(8199.964) ~~like~~ (8200.144)  
international relations regime? Because if it seems like pretty safe to say if we get into a bioweapons arms race, we're going to be in bad shape. we really have to have some more globally cooperative approach. Or the missiles have one really nice property, which is they don't spontaneously escape their silos and self-replicate around the world. 


---


#### 8226.682

Whereas the list of lab leaks is quite long. It just seems like there's no way that we can get into an international bioweapons arms race and survive it. We just have to avoid that trap in the first place. And   
(8243.557) ~~yeah,~~ (8243.717)  
also, what happens when you develop cures for a wide range of diseases, and you're able to extend human lifespan significantly longer than what it is now and eliminate a lot of the diseases that we face once that exists.   
(8261.454) ~~I don't know, maybe that's a paradigm shift.~~(8263.536)  
  
(8263.616) ~~Maybe that's a,~~(8264.216)  
that's like a shift in human consciousness at that point. And we start thinking about things very differently because we're all used to thinking about   
(8272.504) ~~like~~ (8272.724)  
everything in terms of being finite. 


---


#### 8276.247

And I think   
(8277.808) ~~having,~~ (8278.188)  
having an approach or thinking about things in a way that isn't finite anymore and thinking about things in terms of how valuable our health and our life is because of the fact that enables us to be with who we love for longer. The time that we have with the people we care about is, in my opinion, the most valuable thing that we have. And once you enable people to have healthy lives with people they care about, more or less indefinitely, that changes a lot. And I'm very excited to see, I hope that happens in my lifetime. I think it will. I think it'll probably happen within the next decade even. But I hope that really changes human consciousness to a point to where a lot of these problems just   
(8325.146) ~~kind of~~(8325.426)  
start to go away because we stop thinking of everything in terms of finite resources, finite lifespans, finite time with the people that we care about. 


---


#### 8335.032

Hopefully it's enough of a conscious shift in consciousness that we see some of these problems fading because a lot of them are cultural, right? A lot of these problems or a lot of these threats at the heart are very cultural. It's not about the technology. It's about how we use the technology and how we're interacting with each other when we use it. And that requires people to think differently. It's not a problem that can just always be addressed with some new technology or some new defense mechanism, we really have to change our thinking. And I hope that when these things start becoming widely available, people's thinking will shift dramatically. Maybe that's where things are headed. 


---


#### 8381.383

I actually have a lot of hope that's where things are headed and a lot of optimism, because I think overall, most people are good. And I think we can heal a lot of things, not just health problems, but a lot of psychological things we can heal with these tools because it's going to change the way that we interact with each other and the way that we perceive our environment and our relationship to it. That is beautiful sentiment and maybe a good place to end.   
(8408.971) ~~I don't know if there's anything else that you wanted to touch on, but~~(8412.815)  
hard to hit a more aspirational note than that.   
(8415.257) ~~I know. Yeah, I think~~(8416.398)  
I agree with you. 


---


#### 8417.659

I mean, as far as other things to discuss, I don't know. I think we've probably discussed pretty much everything I had. And we talked about most of the models that I found interesting. So yeah,   
(8429.017) ~~I mean,~~(8429.237)  
yeah, I think that's a good place to stop too. I think we can probably call it there. And this has been really great, by the way. I had a lot of fun doing this and I really appreciated   
(8439.248) ~~this.~~ (8439.448)  
  
(8440.029) ~~This is great.~~(8440.409)  
I appreciate you being willing to spend so much of your Saturday teaching somebody who doesn't know nearly as much as I suddenly feel like I really should about this area. So feelings definitely mutual. I guess my closing thank you is Amelie Shriver. 


---


#### 8456.059

Thank you for being part of the Cognitive Revolution. Of course. Thank you for inviting me. 


---



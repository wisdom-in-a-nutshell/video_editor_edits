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


#### 00:06:40.845

You can design proteins that have very specific chemical and functional properties. And this is pretty new stuff, but you can also do a lot of the same things with DNA and RNA molecules as well. Okay. This is a paradigm shift, right? The application of AI to biology, obviously the AI is creating all sorts of paradigm shifts, but   
(00:06:59.286) ~~I think~~(00:06:59.446)  
it might also be helpful for people to understand a little bit better of the before state when we didn't have any of these tools yet, which is not that long ago. Not that long ago. Yeah. What was the sort of prevailing approach to figuring stuff out? You hear these stories of, oh, look, we found this frog in the rainforest that is immune to a certain disease. 


---


#### 00:07:21.487

What's going on there? Let's see if we can't find something in this frog that could be a medicine or whatever. It's really anecdotally special observation motivated investigations in a lot of cases. And then I know there's also just a lot of brute forcing where it's like, we have no idea which proteins are going to interact with which other ones. So let's just create this massive cross matrix and see if we can't figure it out that way. And look for hits,   
(00:07:43.824) ~~kind of~~(00:07:44.043)  
massive essays, just exploring the space, all of these things without any idea of what the puzzle pieces actually look like, which makes it obviously very difficult to figure out how they would fit together. 


---


#### 00:07:55.331

What more would you tell people who want to understand, okay, what was the before, before all this stuff started to come online? There's a lot of methods that come from wet lab work where people do this stuff in animals. Like they say you want to do directed evolution on a protein and try to find higher functioning variants or variants that are more thermostable that have higher expression or something like that. You can mutate these things in a lab. You can do like point mutations or you can do two mutations at a time or you can do like multiple. When you start adding in things higher than just single point mutations, you get this combinatorial complexity, right? 


---


#### 00:08:38.932

And so it gets really unwieldy.   
(00:08:41.433) ~~I feel like~~(00:08:41.933)  
my experience with traditional methods is somewhat limited. I don't come from a wet lab background. I come from a very computational background. I haven't spent a lot of time working with more traditional methods that people have used historically. So computationally, traditionally the way that this sort of thing was approached was through molecular dynamics simulations. You have what's called a potential, right? And this potential tells you   
(00:09:10.267) ~~like~~ (00:09:10.486)  
how the dynamics evolve. And they come in a lot of different flavors, a lot of different complexities. Some of them model the proteins using just standard Newtonian physics. And then you can add in more complexity on top of that, things like quantum properties and other features of the protein to make the molecular dynamics simulation more complex and more robust. 


---


#### 00:09:32.890

But these simulations are really computationally intensive. They take a long time, they take a lot of GPUs, and they're just not very efficient. And on top of that, the length of time that you run your simulation for really in a lot of cases determines how accurate your distribution is and how accurate the confirmations or trajectories that you get out of that are. So you might run your simulation and not run it for long enough, and you don't get all the different states that the protein might be in, but you miss some of them, right? And there are some new AI models that are trying to address this and trying to make headway into augmenting or even replacing molecular dynamic simulations in a lot of cases. 


---


#### 00:10:21.931

And this is really good because we need things that are more computationally efficient so that we can do this for a lot of proteins, right, because we have a lot of proteins to do this for. So for example, AlphaFold2 came out a couple of years ago, and that was a big deal,   
(00:10:38.115) ~~right,~~ (00:10:38.375)  
But you just get a single static structure from AlphaFold2. So we give it the protein sequence, which is just a sequence of amino acids, which are represented by 20 letters, and it takes in this protein sequence, and it provides you with a static structure for that protein that's a low-energy confirmation for that protein. that protein could exist in other conformations. It might have other states that it exists in when it's interacting with other proteins, or based on the environment that it's in, what temperature it is. 


---


#### 00:11:11.967

Things like this can change the shape of the protein, right? They move around, they're very jiggly, and they do things. And so people have been trying to address this and model what's called the Boltzmann distribution of proteins. from statistical mechanics that tells you all the different confirmations and what probabilities there are associated to those different confirmations. And having a way to sample the Boltzmann distribution and get all of these different confirmations out of them, and also understanding the transitions between these states is a really difficult problem. And there's actually a model that does a really good job of addressing this that just came out middle of last year. It's called Distributional Graphformer. It's a generalization of the idea that AlphaFold2 is implementing, right? 


---


#### 00:12:00.975

It's not just a single static structure anymore. It's actually a whole ensemble of structures and also the transition pathways between those different metastable states. And being able to model this and understand more like the dynamics of the proteins is something that people have been thinking about pretty hard for the last couple of years.   
(00:12:21.788) ~~Distributional Graphformer.~~(00:12:22.928)  
is addressing a lot of this. And it does a pretty good job of doing it too. There's some room for improvement for sure, but it's a pretty solid model. Some people that I have a lot of respect for in this area have worked on this. And some of the inspiration comes from diffusion models. So it's a diffusion model similar to   
(00:12:45.029) ~~like~~ (00:12:45.169)  
DALI, which most of your watchers are probably familiar with, but it works on proteins instead of images and also protein complexes even, or protein small molecule complexes, and getting a handle on something that's more like the dynamics of the protein and getting a good representation of all the different metastable states that the protein might exist in at low energies. 


---


#### 00:13:08.384

So like a good example of how AI has sort of replaced wet lab methods, this directed evolution methodology, there are directed evolution AI models that you can use like protein language models to do directed evolution. Doing directed evolution in a lab in a lot of ways, now that we have AI tools to do similar things feels a little bit unnecessary.   
(00:13:32.993) ~~Like~~ (00:13:33.134)  
why do we need to go and inject an animal and wait some amount of time for this to play out inside the animal and then actually synthesize these things by hand in a lab somewhere when we can   
(00:13:44.298) ~~like~~ (00:13:44.457)  
do very similar things computationally and often get better results. You can also do a sequence redesign with things like protein MPNN or ligand MPNN, which allows you to redesign parts of the protein sequence or the entire protein sequence, maybe under some certain specific chemical constraints, or you might want to bias the residues towards or away from certain amino acids and things like that. 


---


#### 00:14:13.778

But these AI tools allow you to do that computationally and they do it really fast,   
(00:14:18.200) ~~right? I mean,~~(00:14:18.840)  
like I can design a sequence for a protein in a few seconds with   
(00:14:23.001) ~~like~~ (00:14:23.142)  
ligand and PNN on my computer with no special hardware or anything. I don't even need a fancy GPU to do it. And I can do that many times and get lots of variants for my protein. and assess them computationally. And very often these variants that you get out of this process are much higher performing than   
(00:14:45.065) ~~like~~ (00:14:45.225)  
the wild type or than what you would get by doing this in a wet lab. So hopefully that gives you some idea of some of the methods that still are being used. 


---


#### 00:14:54.850

It's not like these have just gone the way of the dodo and disappeared or something, but they have their place for sure. But   
(00:15:01.754) ~~I think~~(00:15:02.114)  
computational approaches are proving to be much faster, much more effective, and you can scale them, which is really important because we're working sometimes with millions or hundreds of millions of proteins. Having millions of variants of a protein and being able to assess them and determine their quality in some metric has become a lot easier in the past couple of years even.   
(00:15:27.073) ~~Like~~ (00:15:27.214)  
protein and PNN only came out a couple of years ago.   
(00:15:30.436) ~~I think~~(00:15:30.696)  
Because the AI techniques are so new, it's such a new paradigm. It's such a new methodology. 


---


#### 00:15:38.186

Most people working on them are still developing their understanding. There aren't very many experts on this stuff. I think we're all learning together. I'm definitely still learning a lot of stuff from my coworkers and other researchers in the field. And it's   
(00:15:52.828) ~~kind of~~(00:15:53.149)  
mind-blowing how fast this stuff is developing too. It's developing incredibly fast, which is really good in my opinion. I want to see this stuff proliferated and developed and used because we're going to solve problems much faster this way. So   
(00:16:07.847) ~~I guess~~(00:16:08.089)  
in terms of   
(00:16:08.509) ~~like~~ (00:16:08.609)  
just a little intuition for the confirmations, I envision a slinky where if I just sit the slinky down on the floor, it will come into a pretty tight coil. 


---


#### 00:16:19.567

And that you might say is like its lowest energy state. Then I can stretch it out. And if I do the work and put the energy into it, then I can stretch it out. Now, if I let it go, it's going to snap back to its low energy state. I could also step on the middle of it, and then I would have the part of it would be under my foot and bent down, but then the parts on the side would presumably still look like they're normal, but there'd be this deformed part in the middle where I'm stepping on it. Yeah. This is   
(00:16:48.921) ~~sort of~~(00:16:49.260)  
analogous to what is going on, violating my no analogy rule, but this is a pretty tight analogy. 


---


#### 00:16:54.863

It's like a physical deformation, right? Where this thing can have a low energy state, but then maybe in the presence of some other protein that like constrains it in a certain way or some other small molecule, perhaps it fits into a pocket of it in a certain way or brings two parts that aren't normally together, more closely together, whatever. Then you can have these sort of deformations and then subject to those constraints, they still find their natural low energy state. And of course, this is all happening in an environment where the individual proteins, they're in solution, right? So there's water molecules bouncing off them all the time. So they have this sort of noisy environment. 


---


#### 00:17:34.178

I'm thinking there of like brownie in motion. The constant sort of bumping into the environment creates opportunity for these things to occasionally flop from shape to shape. And so doing all of this in traditional sense is probably hard for a lot of reasons, but you highlighted the fact that the computation is really slow, right? Now,   
(00:17:55.898) ~~like~~ (00:17:56.019)  
I have a hypothesis on this, but I'll just ask the question. How is it happening that the AI models are doing this so much faster than traditional physics? Because a naive thought would be like, there's only physics, right? We hear that sort of refrain a lot. So it seems in some sense surprising that you would be able to make a new black box system to make these predictions that they would be faster and more accurate as opposed to just running the physics. 


---


#### 00:18:25.715

How is that leap happening? Okay, so I think the key here is compression. neural networks are compressors of information. Whereas in molecular dynamics, you could simplify things by simplifying the forces or simplifying the model in terms of how complicated the physics are that you're using to model problems. If I strip everything down and just do bare bones Newtonian physics, I can simplify things that way, but there's no real compression happening. For these AI models, you can think of them as functions, but you can also think of them as compressors of information. You're taking something complicated and noisy sometimes, and you're compressing it and you're providing a representation of it that is more compact. Traditionally, you think of a deep learning neural network. 


---


#### 00:19:12.752

You've got data, you train on your data. Maybe you have a train test validation split and you train on your training data and you You see how it performs on your test data and that's your trained model. But you can also train models with physics constraints,   
(00:19:27.016) ~~right?~~ (00:19:27.236)  
There are some approaches that people are using that are completely data-free and are based on physics. And the model is learning the physics and compressing that physics. You get something   
(00:19:36.818) ~~that,~~ (00:19:36.980)  
that is faster, like orders of magnitude faster,   
(00:19:40.361) ~~right? You get,~~(00:19:40.941)  
you get something that produces your answer in   
(00:19:43.461) ~~like~~ (00:19:43.602)  
a minute instead of four hours or days. And if you've done it right, it generalizes to systems that it hasn't been trained on before. people are doing this for this problem in particular, for getting the Boltzmann distribution of a protein and getting all these ensembles of confirmations and their transitions between the states. 


---


#### 00:20:01.630

So that was pretty much my hypothesis that it's essentially learning higher order concepts beyond the raw physics. It's really this striking observation that comes up over and over again that, okay, yeah, language models, they're only trained to predict the next token, but they not only seem to be generalizing certainly beyond the narrowly defined bounds of their training data, and perhaps to some degree even more than that is a hotly debated topic, but what is pretty clearly demonstrated at this point is that in the middle to late layers of a language model transformer, the techniques are there to say, okay, this pattern of activations seems to correspond to this higher order concept that we care about, which is   
(00:20:53.922) ~~kind of~~(00:20:54.422)  
a miraculous thing that it's just predicting the next token, but it's learning these concepts of justice and fairness and ethics and whatever that are obviously useful to predict the next token, and that's presumably why they're arising, but not something that's been specifically coded for. 


---


#### 00:21:13.457

So I guess in the application to biology, basically the same phenomenon is happening where raw data or raw simulated physics or whatever is the input, I'm guessing that the token level vocabulary of a protein would be the 20 amino acids, but the sort of higher order concepts are like, oh, this chunk of a thing is reused a lot. And these two chunks of things interact with each other in a particular way. Give us a little more intuition of that. What are the higher order concepts that these things seem to be learning? Yeah. So the concept that I think you're trying to grasp onto is protein motifs. Motifs are like reoccurring patterns that happen in proteins. 


---


#### 00:21:53.611

They're short little sequences of amino acids that recur often in lots of different proteins and generally have a very similar structure across different proteins. If we put aside dynamics for a moment and we just look at like structure prediction. So there's another model, ESMFOLD, predicts the 3D structure of the protein in some low energy state, right? This is an alternative model to AlphaFold2. It doesn't perform as well as AlphaFold2, but it does pretty well. And it's a language model. It's something that people call a protein language model. And   
(00:22:25.848) ~~it's,~~ (00:22:25.969)  
it's built on the BERT architecture actually, which sounds kind of bad, right? Cause BERT's like this older model that's only used for like specific things now. 


---


#### 00:22:36.376

The chat GPT models have overshadowed or outshined the BERT models at this point, but In biology, this actually makes a lot more sense because you have the mask language modeling objective that you train on for protein sequences, and you just mask out some of the amino acids in the protein sequence and have it predict what those are, right? And just by training it to do this, and then putting a folding model on top of it called EvoFormer, which actually comes from the AlphaFold2 architecture, you don't train on any physics. but somehow you learn how to predict 3D structures of proteins, right? And so in this case, it's almost like physics mostly isn't needed, right? If you just want to predict a static structure of a protein, you can get pretty good results just using a BERT type architecture with mask language modeling objective, training on millions of proteins. you get something that will fold proteins for you pretty darn well. 


---


#### 00:23:33.688

There's some really nuanced architectural differences between ESMfold and AlphaFold2. AlphaFold2 uses what's called multiple sequence alignments, and it also uses these templates, right? And in general, it is better performing because it has these extra added things in the architecture that improve its ability to predict the structure. But even there, there isn't really a lot of physics explicitly happening. Now maybe there's some physics encoded   
(00:24:01.796) ~~in this~~(00:24:02.457)  
in some way, but we're not giving it   
(00:24:04.681) ~~like~~ (00:24:04.780)  
forces and potentials and things like that. And yet somehow we're able to predict the structure of the protein with really high accuracy   
(00:24:13.388) ~~for a lot of proteins,~~(00:24:14.528)  
for most proteins. I guess that's another example of where AI can be a lot better than the molecular dynamics. 


---


#### 00:24:22.074

Because if you want to model a protein actually folding in a molecular dynamics simulation to get the folded structure of the protein, this is pretty hard and time consuming and computationally intensive. Whereas for AlphaFold2 or ESMFold, you give it a big protein and it takes a few minutes. And in these cases, these are language model-like models, right? They definitely have the architecture that looks a lot like language models, especially ESMFold. ESMFold is pretty much just a language model. And in terms of how this relates to language modeling. Motifs are   
(00:24:58.179) ~~kind of~~(00:24:58.519)  
a fuzzy concept, right? Like defining what a motif is and having that shape described is a little bit fuzzy, but these models learn these higher order concepts where you're looking at   
(00:25:11.204) ~~like~~ (00:25:11.345)  
groups of amino acids now instead of just the individual vocabulary elements, right? 


---


#### 00:25:16.166

We're not just looking at individual amino acids of the vocabulary anymore. We're looking now at an aggregation of amino acids at a higher level. you can pull this out of these models. And there's some work on this, maybe three years old now, called Birtology Meets Biology. And they do a really in-depth study of how to pull out these different things, active sites and binding sites and motifs and things like this, based on the attention maps in the protein language model. Another thing that people have found is the attention maps recapitulate the contact maps for proteins. The contact map is like a 2D matrix representation of all the contacts between the different amino acids in the protein, right? 


---


#### 00:26:00.398

And it turns out the attention map, the matrix that you get from your attention mechanism, recapitulates that and is highly correlated with those contact maps. So they are learning higher order concepts for sure, just as they do for natural language. You can do topic modeling and things like that on these models, but I would say now a lot of the more interesting models are more influenced by diffusion and flow matching models. A lot of the generative models that we're getting that are predicting the Boltzmann distribution or that are generating new protein structures for you with specific   
(00:26:38.426) ~~like~~ (00:26:38.586)  
shapes and functions or that are allowing you to design new sequences that fold into a particular backbone. 


---


#### 00:26:45.730

A lot of them are more influenced by diffusion and flow matching than language modeling and transformers. Some of them use transformers, but they're starting to be a lot more influenced by Dolly type models, I would say, because you're starting to get this really fine grained control over what kinds of proteins or small molecules or nucleic acids that you can generate. And there's actually some models that have come out that are text conditioned. So like a couple of the models that I mentioned were ProteinDT and MoleculeSTM. And these are generative models that are text conditioned, and they allow you to type in   
(00:27:25.252) ~~like~~ (00:27:25.373)  
a natural language prompt and get out a molecule. So   
(00:27:29.773) ~~like~~ (00:27:29.913)  
protein DT, for example, or molecule STM, you can give it a text prompt, a natural language describing the properties of the molecule in just natural human language, giving it   
(00:27:40.655) ~~like,~~ (00:27:40.935)  
this molecule has these chemical properties and it has this sort of bias away from or towards these amino acids or interacts with these other molecules in such way. 


---


#### 00:27:51.798

Like you can give it these natural language text prompts And it will generate proteins and small molecules for you that satisfy these constraints or   
(00:28:01.859) ~~that,~~ (00:28:02.039)  
that correspond to the text prompt that you give it. And there are more models like this that have come out recently that do similar things. They're text conditioned, like diffusion models or flow matching models that are generative and that produce molecules with specified properties based on natural language text, which in my mind, that's   
(00:28:20.502) ~~kind of~~(00:28:20.743)  
mind blowing.   
(00:28:21.403) ~~I think~~(00:28:21.624)  
that's amazing. Having a model. that will just generate molecules for you that fit natural language descriptions   
(00:28:30.047) ~~is,~~ (00:28:30.186)  
that's crazy. How did that happen?   
(00:28:32.728) ~~Like,~~ (00:28:32.847)  
that's amazing. No doubt. So let me just rewind a little bit again, and then I want to get into a little bit more how that happened. 


---


#### 00:28:40.501

So the, I always try to start with like inputs and outputs as one kind of good frame for understanding this stuff. So it seems like the kind of first major breakthroughs   
(00:28:51.952) ~~in~~ (00:28:52.133)  
for biology of the   
(00:28:54.875) ~~like~~ (00:28:55.015)  
modern era, which is only the last however many years. were the structure prediction models. And   
(00:29:02.634) ~~this is,~~(00:29:03.476)  
if I understand correctly, there were about a proteins that had been analyzed to the point where people were pretty confident that they had a structure. If I understand correctly, this was mostly done through   
(00:29:14.263) ~~x-ray crystalline, which is... Yeah,~~(00:29:16.484)  
cryo-EM. Yeah. So I think that's why the initial things were   
(00:29:22.009) ~~sort of~~(00:29:22.289)  
limited to outputting a single predicted structure because if you're in like a crystal, you   
(00:29:27.790) ~~sort of,~~(00:29:28.050)  
by the nature of crystals, have a single repeating structure, right? 


---


#### 00:29:32.616

So what we had was people put a lot of time in the lab into, first of all, figuring out how to get these things to crystallize, which is weird because   
(00:29:42.127) ~~they're not really~~(00:29:42.689)  
protein crystals don't really occur in nature,   
(00:29:45.871) ~~right?~~ (00:29:46.051)  
That's a very odd thing in the first place. Maybe that's like gout,   
(00:29:49.634) ~~I guess.~~(00:29:49.894)  
It's   
(00:29:50.054) ~~sort of like~~(00:29:50.453)  
uric acid crystals, if I understand correctly. But you don't think of proteins, we think of them as floating around in solution or   
(00:29:58.358) ~~kind of~~(00:29:58.558)  
interacting with each other in complicated ways, but they're not in repeating lattice structures. So that in and of itself was   
(00:30:05.104) ~~sort of~~(00:30:05.324)  
a weird,   
(00:30:06.645) ~~like,~~ (00:30:06.786)  
closest approximation that we could get, right? We got to make enough of this stuff that we can get it to put in, coalesce into some crystal form. 


---


#### 00:30:13.615

Then we can hit it with x-rays and we can try to decipher how that gets scattered. And then we can come up with a structure and we hope.   
(00:30:20.305) ~~I mean,~~(00:30:20.565)  
we don't really know anything,   
(00:30:21.586) ~~I guess,~~(00:30:21.866)  
but   
(00:30:22.126) ~~I guess~~(00:30:22.346)  
it works well enough that that approximates the structure that it actually takes in the cell, but no guarantees. So first generation   
(00:30:32.657) ~~of stuff is not first generation, of course, we're like~~(00:30:34.839)  
other AI techniques before this, but like   
(00:30:37.041) ~~of these sort of~~(00:30:37.623)  
modern wave of   
(00:30:38.663) ~~like~~ (00:30:38.824)  
mega breakthroughs.   
(00:30:40.685) ~~the,~~ (00:30:40.846)  
and   
(00:30:41.086) ~~I guess that was really measured by,~~(00:30:42.428)  
maybe you could help me fill in some blanks here too, because   
(00:30:45.271) ~~there's,~~ (00:30:46.313)  
it's like   
(00:30:46.933) ~~kind of~~(00:30:47.114)  
circular nature to some of this stuff sometimes where I'm like, wait a second. 


---


#### 00:30:50.037

So where is the ground truth? It seems to be a little bit of, it can feel like a, the ground truth is sort of a shell game. As I understand it, the way that AlphaFold was determined to be a breakthrough in the first place was that there was a competition held on an annual basis or whatever, where people would basically show up with their shape predicting model, and they would be given, here is the sequence. And their job is to predict the shape. And then the test set, the training set was all known proteins that came before. And the test set was all of the stuff that had been newly derived in the last year. 


---


#### 00:31:33.032

So these were the new things that people hadn't been able to train on. They would show up and they would be measured against essentially the crystal based techniques. And everything would fall short, like not nearly as good, not matching the crystal things. And then AlphaFold showed up and was like, Oh, hey, it's and this is where I get a little fuzzy. As I understand it, people would say it's in some ways even   
(00:31:57.488) ~~like~~ (00:31:57.647)  
better than the crystal techniques. But   
(00:31:59.548) ~~like,~~ (00:31:59.749)  
how do we establish that? How do we know that   
(00:32:03.310) ~~the when is the crystal technique right or wrong.~~(00:32:06.713)  
I'm a little fuzzy on how we   
(00:32:08.994) ~~kind of~~(00:32:09.236)  
pin down the ground truth when we know that the crystal thing is only an approximation and AlphaFold was   
(00:32:13.979) ~~kind of~~(00:32:14.239)  
trained on that with augmented data. 


---


#### 00:32:16.080

Like help me pin down the ground truth there if you can. Yeah   
(00:32:19.363) ~~I mean ground truth in this case yeah I mean~~(00:32:21.605)  
this is a little hard and it's very like application and   
(00:32:25.871) ~~like~~ (00:32:26.030)  
situation specific, right? Depending on what you're trying to do and how you're trying to do it, you may want some crystallized structure that you got in a lab, or you maybe want like an alpha fold structure. And in other cases you might want   
(00:32:37.980) ~~like~~ (00:32:38.182)  
a trajectory or an ensemble of conformations, which wasn't really possible until more recently.   
(00:32:45.027) ~~Like~~ (00:32:45.188)  
observing the dynamics of a protein is really hard. And so to be able to model that on a computer and get predictions that are actually accurate about the dynamics of the protein and all the different   
(00:33:00.295) ~~like~~ (00:33:00.494)  
low energy conformations that it exists in,   
(00:33:03.976) ~~like~~ (00:33:04.096)  
that's pretty new. 


---


#### 00:33:05.516

And in my mind, if you have the ground truth really ultimately is the Boltzmann distribution, right? Which is this very sort of theoretical physics idea that comes from like statistical mechanics. that's the ground truth. Whether or not you can model that on a computer or observe that in a lab is another question. But the Boltzmann distribution of the protein is the ideal ground truth. And is that basically like a... I guess I'm thinking of it in one sense as   
(00:33:37.068) ~~sort of~~(00:33:37.308)  
like a potential, energy potential diagram where you have... It's related. It's a probability distribution, right? And it describes You can think of it in terms of an energy landscape, right? Because if you have this nice energy landscape, the low parts, the valleys that you have in your energy landscape are going to be like the metastable states of the protein. 


---


#### 00:33:59.586

They're going to, they're going to correspond to the metastable states of the protein. And then the peaks, like on top of the mountains, right? These are   
(00:34:06.146) ~~like,~~ (00:34:06.366)  
like states that are very transient and that are   
(00:34:09.527) ~~like~~ (00:34:09.688)  
unlikely   
(00:34:11.148) ~~to be,~~(00:34:11.708)  
to exist for very long. So   
(00:34:13.507) ~~you're,~~ (00:34:13.728)  
when you're trying to model the Boltzmann distribution, you're trying to get out these   
(00:34:18.382) ~~like~~ (00:34:18.563)  
low energy conformations from it and then the transitions between those and understanding how often you transition between this state and this other state and what that transition looks like. I guess that would also be considered part of the ground truth, right? Because this is all part of the dynamics of the protein in the environment and not just some single either crystallized structure or alpha fold 2 predicted structure. 


---


#### 00:34:44.288

Yeah, so I guess the answer to your question is the ground truth, at least to me, is the Boltzmann distribution. And the question of whether or not you can model that on a computer in a lab is a completely different question, but that's the ground truth. So it's a probability distribution of what percentage of the time the protein in some   
(00:35:04.637) ~~like~~ (00:35:04.838)  
neutral case solution or whatever is in shape A versus shape B versus shape C. And then the in-between things are sort of Here I'm   
(00:35:16.327) ~~kind of~~(00:35:16.648)  
again returning to my slinky visualization where I could have the thing   
(00:35:22.411) ~~sort of~~(00:35:22.692)  
in its lowest state or I could like tie its ends together and then it'll   
(00:35:26.976) ~~sort of~~(00:35:27.195)  
make a nice circle and but again   
(00:35:29.378) ~~kind of~~(00:35:29.597)  
look compact and be   
(00:35:30.878) ~~sort of~~(00:35:31.099)  
in a relatively comfortable place but then the second that breaks it's like reverbing back until it gets to its normal state, that reverb moment is sort of the transitional state. 


---


#### 00:35:40.760

It's not going to be in that state very long and it's   
(00:35:43.001) ~~kind of~~(00:35:43.322)  
on its way from one to another. So we don't know how many different, for any given protein, there could be   
(00:35:49.362) ~~like~~ (00:35:49.483)  
multiple different low energy states that it might spend time in. And there probably also is like a path issue to it where you maybe can get from A to B and B to C, but not necessarily A to C without going through B I imagine. Yeah, exactly. So lots of weird stuff there. And then, okay, so all that is just they interact with each other. So this is,   
(00:36:12.474) ~~I guess,~~(00:36:12.693)  
where AlphaFoldMultimer starts to come in? Yeah. AlphaFoldMultimer models the interactions between proteins, right? 


---


#### 00:36:19.721

And you can model protein complexes. And there's actually some new results that just came out maybe a month ago. that computes something called the LIS score based on the PAE output of alpha-fold multimer.   
(00:36:34.626) ~~This is like a-~~(00:36:35.166)  
Can you unpack both of those? Give us the PAE too. So the PAE is one of the outputs of alpha-fold multimer and it's,   
(00:36:42.088) ~~let's see if I remember what the abbreviation is for,~~(00:36:44.509)  
predicted aligned error, I think is what it stands for. And this is telling you, it's a metric that tells you the quality of   
(00:36:51.451) ~~the~~ (00:36:51.690)  
the interfaces between the two proteins. You've got a lot of different metrics that come out of AlphaFold Multimer or AlphaFold2. So you have PLDDT, which tells you a per residue confidence score of how confident the model   
(00:37:06.192) ~~is that~~(00:37:06.831)  
is the structure of the protein   
(00:37:08.693) ~~at that particular point in the protein, like~~(00:37:11.132)  
at that particular residue. 


---


#### 00:37:13.094

And then you can take the average of the PLDDT and get an overall confidence for the whole protein. But then   
(00:37:18.536) ~~you also have,~~(00:37:19.115)  
you have IPTM and PTM scores, which are other scores that tell you about other aspects of the protein, and then you have these PAE outputs, predicted aligned error outputs, and these tell you about the quality of the interfaces between the proteins when it predicts the two proteins together. there's an interface region where the proteins are in contact with each other. And you can   
(00:37:41.235) ~~kind of~~(00:37:41.454)  
think of it as a certain cutoff, right? After a certain distance, you don't really count it as an interface residue anymore. But the PAE tells you the quality of these interfaces, how good of a quality the model has provided you. 


---


#### 00:37:54.378

And you can compute something based on the PAE called the LIS. And the LIS score, let me look up what that stands for really quick, because I actually forgot what it stands for. So while you're doing that, I'll just riff a little bit on   
(00:38:07.518) ~~the structure too. Yeah, or~~(00:38:09.885)  
the nature of the interface, because this is just another level of   
(00:38:12.487) ~~like~~ (00:38:12.668)  
insane complexity, right? You have a range of kind of whether these things are like jigsaw puzzle pieces that are perfectly fit to each other and have a really tight coupling or jigsaw pieces that   
(00:38:26.177) ~~sort of~~(00:38:26.438)  
fit, you can   
(00:38:27.018) ~~kind of~~(00:38:27.298)  
press them together, but they don't perfectly fit and they don't really want to stay together as much all the way down to obviously they just don't fit at all. 


---


#### 00:38:33.563

They just kind of don't don't adhere to each other. Is there anything more we could do to develop our intuition there for how strong is the strongest fit? I'm thinking like, boy, if I screw a screw into a nut, it's not coming off with any natural process. Somebody would have to come unscrew that. I'm guessing it's probably... I don't know. How tight are the tightest ones and what is the dynamic range of how adherent these things are to each other? Yeah, so there's two ideas that you're addressing here. One of them is like binding affinity, like how much affinity these two things have for each other to bind to each other. And then there's also in terms of   
(00:39:16.407) ~~like~~ (00:39:16.568)  
dynamics, like how weak or strong or how transient are the interactions between them in terms of   
(00:39:23.512) ~~like~~ (00:39:23.733)  
dynamics and like the time spent next to each other, right? 


---


#### 00:39:27.695

There's recent work I think it's out of MIT, they built these flow matching models with AlphaFold and ESMFold. It's called AlphaFlow. And   
(00:39:37.068) ~~AlphaFlow,~~ (00:39:37.788)  
they use the AlphaFold2 architecture and they train it as a flow matching model, which is like a generalization of diffusion. And using this, they get these ensembles of confirmations for a protein. And part of the information that they get out of this is how transient the interactions between residues are. If you   
(00:39:58.257) ~~produce,~~ (00:39:58.818)  
let's say you run your alpha flow model and you produce   
(00:40:02.621) ~~like~~ (00:40:02.760)  
10,000 different confirmations or states that the protein exists in. And then you can   
(00:40:09.266) ~~kind of like~~(00:40:09.666)  
cluster those, like structurally, you can cluster them and then look at which residues are close to each other in each of those clusters. 


---


#### 00:40:20.228

So maybe you take   
(00:40:20.969) ~~the, you take~~(00:40:22.188)  
the centroid or something of a cluster, and then you look at the distance between the residues, and then you look at other clusters, and the distance between the residues in those other clusters, and you get an idea of   
(00:40:34.150) ~~like~~ (00:40:34.391)  
how often two residues are in contact with each other from this. And you can tell how transient the interaction between these two residues are, and how much time they spend together. You could generalize this, right? And this is something that hasn't been done yet. So people who are looking for   
(00:40:50.469) ~~like~~ (00:40:50.588)  
research projects, this would probably be a pretty good one. If you generalize this to alpha fold multimer, do the alpha flow thing with alpha fold multimer, if it works well, and again, this hasn't been done before, but this would be a really great thing for someone to do. 


---


#### 00:41:04.590

You could figure out how transient those interactions between two proteins are, right? Because now you have two proteins or more, maybe you have three or four or whatever, but you have two proteins that are in different conformations at different times. And AlphaFlow will generate all these different conformations for you. And then you can analyze all these different conformations and figure out how transient the interactions between the two proteins are and get an idea more about the dynamic side of things and not just a single number or a single metric like binding affinity, right? Because   
(00:41:39.704) ~~binding affinity, I mean,~~(00:41:40.724)  
it's a hard thing to predict. It's a hard thing to compute. training a model to predict binding affinity is actually a pretty hard thing to do. 


---


#### 00:41:47.824

And most of them don't work. Most of them don't generalize well. But these approaches, like if you were to generalize alpha flow to the alpha,   
(00:41:55.369) ~~like that,~~(00:41:55.750)  
that would give you more information than just binding affinity.   
(00:41:58.231) ~~That would give you,~~(00:41:58.871)  
that would give you some notion of how often particular residues of the two proteins are in contact with each other. And then,   
(00:42:06.496) ~~like I was saying before,~~(00:42:07.317)  
the LIS score, this is the called the local interaction score. They use alpha fold multimer and they get the PAEs out of alpha-fold multimer. And then using the PAE, they compute the LIS, which is a pretty simple computation.   
(00:42:21.887) ~~I don't know that I can describe it in words,~~(00:42:23.509)  
but it's not a terribly complicated thing to compute. 


---


#### 00:42:26.710

Once you have the PAE, the LIS is pretty easy to compute. And this tells you how likely you are to have a protein interaction, which kind of gets that binding affinity to some degree. And being able to predict protein interactions is actually a really hard problem. And most models that try to predict protein interactions don't work well and don't generalize well. And there's actually a   
(00:42:50.648) ~~kind of~~(00:42:50.909)  
a big problem with a lot of these models. So when people are training them, a lot of times if you're training a model that takes as input protein sequence or two protein sequences, people don't split their data in the right way. you have this notion of sequence similarity. 


---


#### 00:43:07.528

And if you, if your data, if your training data has sequences in it that are very similar to your test data sequences, you're going to get overfitting and you're not even going to realize it. Like all the usual signs of overfitting aren't going to be there, but you're going to overfit without even realizing it because you're going to have training data and test data that's highly similar to each other in terms of sequence similarity. And a lot of the protein interaction models that have been trained don't take this into account. And they don't split their data based on   
(00:43:40.425) ~~like~~ (00:43:40.565)  
sequence similarity or structural similarity. But the LIS score using alpha-fold multimer works really well. And   
(00:43:48.288) ~~it's,~~ (00:43:48.427)  
it doesn't require any training of the model or anything like that. 


---


#### 00:43:51.648

You just, you give it the two proteins or multiple proteins that you want to find out if there's an interaction there, and you get the PAE out of alpha-fold multimer, and then you just compute the LIS score.   
(00:44:03.570) ~~So,~~ (00:44:03.771)  
yeah. Okay. A couple of double clicks and maybe start with one summary. The prediction coming out of these alpha-fold models is this PAE, which is the positional predicted aligned error. So that is basically the actual positioning with   
(00:44:20.014) ~~sort of~~(00:44:20.255)  
a confidence indication. Yeah, it tells you what the quality of the interfaces are between the two proteins that you're predicting in the multimer. And something else we should probably get into that directly follows from alpha-fold multimer is other ways of generalizing the alpha-fold model or training models that are like alpha-fold that do more than just proteins. 


---


#### 00:44:42.869

You might have complexes where there's a protein in a small molecule, or protein in DNA, or protein in RNA, or a metal, or whatever. And so there's all these other biomolecules that you might want to model in complex with each other. And to generalize alpha fold multimer to this new situation is pretty hard, but some people have managed to do a pretty reasonable job of it. I think there's still room for improvement on these, but   
(00:45:14.224) ~~like~~ (00:45:14.385)  
a new model that just came out recently is Rosetta fold all atom and Rosetta fold all atom will let you predict complexes that have proteins and small molecules, proteins and nucleic acids, and proteins, and proteins and metals too. 


---


#### 00:45:29.853

Big step forward now, because now you can apply this idea of computing the LIS score to these other complexes. And you can get this score that tells you how likely there is to be an interaction there and how strong that interaction is. And you could also,   
(00:45:46.059) ~~I don't know how hard this would be to do, just thinking about it now, it seems like it might be actually kind of hard, but you could probably do~~(00:45:55.070)  
the alpha flow type method with something like Rosetta fold all atom as well and get something like conformational ensembles out of it. And   
(00:46:05.393) ~~that's probably something like that is probably coming soon.~~(00:46:08.235)  
Somebody is going to work on that eventually. So yeah, 


---


#### 00:46:11.295

I think I answered your question. I'm not sure. Yeah. Let me just think about where I want to go back to.   
(00:46:16.438) ~~Okay.~~ (00:46:16.518)  
The one thing that you said that caught my attention was, this is all in the context of predicting shapes. We need to predict shapes because we need to understand how things interact. Now we're even getting into predicting how things conform to each other. So the shape of multiple things as they're in actual interaction. And we get these sort of positional predictions that can be   
(00:46:41.231) ~~sort of~~(00:46:41.472)  
cashed out to these parts are actually like interacting in a meaningful way. And this is really where the action is versus these other things are   
(00:46:48.315) ~~kind of~~(00:46:48.496)  
distant from each other. 


---


#### 00:46:49.177

And that's not really where the action is. That's being generalized beyond all proteins to like all the different kinds of things that are meshed up together in a cell. But I believe you had said that there were like as many as 10,000 possible confirmations for a single thing.   
(00:47:09.972) ~~Was that,~~(00:47:10.273)  
did I get it? Yeah. So   
(00:47:11.855) ~~like~~ (00:47:11.996)  
AlphaFlow, when you run AlphaFlow, it generates confirmations of a protein for you. And it was trained on molecular dynamics data, on simulation data. And so it does have some notion of   
(00:47:26.545) ~~like~~ (00:47:26.706)  
dynamics. And what it does is it produces different confirmations of the protein for you. And you can tell it how many of these to produce, right? And the more that it produces, the more likely you are to get a nice global picture of all the different confirmations that might exist for that protein. 


---


#### 00:47:45.797

AlphaFlow, so we've actually tested AlphaFlow on these proteins that are called fold-switching proteins. Fold-switching proteins, so like probably the most popular example floating around in the literature and in the community right now is Kybe. And Kybe is this fold-switching protein that like 10% of the time it exists in this one conformation and then 90% of the time it exists in this other conformation. And this is influenced by   
(00:48:12.288) ~~like~~ (00:48:12.407)  
a circadian rhythm. So it's   
(00:48:14.048) ~~like~~ (00:48:14.188)  
a night-day cycle sort of thing that's   
(00:48:16.329) ~~influenced,~~ (00:48:16.849)  
influenced by like your circadian rhythm. And when you apply alpha flow to some of these fold-switching proteins, it doesn't capture both of those fold-switch states.   
(00:48:28.550) ~~It will like,~~(00:48:29.150)  
so in the example of CHI-B, it actually only really predicts conformations that are relatively close to the fold-switch state. which is like the slightly higher energy confirmation, the one that's a little bit less likely, the one that it exists in 10% of the time, which is a little bit odd, right? 


---


#### 00:48:47.518

Because you would expect and maybe want your model to go for the ground state or the lowest energy confirmation. And for some reason it like sticks   
(00:48:58.083) ~~kind of~~(00:48:58.364)  
close to the fold switch confirmation. I'm not sure that there's like a good explanation for why. And I think it goes back to the AlphaFold2 predictions. Because when you predict the structure using AlphaFold2, you get the fold switch state. You don't get the ground state. And people have done all kinds of little hacks to try and get out the ground state instead of the fold switch state. And the most popular method that they've hacked together is doing MSA subsampling or clustering the MSA and using the different clusters to predict structures. 


---


#### 00:49:35.195

If you take your MSA and you cluster all of your sequences in your MSA,   
(00:49:41.679) ~~you're kind of like,~~(00:49:42.541)  
you're grouping the sequences in the MSA in a way that captures certain evolutionary information. And different clusters will focus on or accent particular conformations. And so if I take out one of my clusters and predict the structure using those clusters in the MSA, I'll get a confirmation out from AlphaFold2. And then if I pick   
(00:50:07.590) ~~a different set of,~~(00:50:08.570)  
a different cluster of sequences in my MSA, I'll get maybe a slightly different confirmation, or maybe a drastically different confirmation. And   
(00:50:17.695) ~~if you do this,~~(00:50:18.275)  
if you do this right, sometimes, not always, but sometimes, you can get out the different confirmations of these fold-switching proteins. 


---


#### 00:50:26.501

And for Ki-B, they've done this successfully, and for a few others, but it's not a super robust method, And I think these alpha flow, I think is in some ways maybe more informative. And something like Boltzmann generators or distributional graph former, I think are significantly better in terms of how they approach the problem because they're going to give you more information. and they're gonna give you more robust information. So for example, like distributional graph former, you're gonna get out something more robust and more informative than if you're just like clustering the MSA or subsampling the MSA for alpha. Can we talk about this MSA thing for a second? If I understand clearly, I'm not even sure I should attempt this, but I'll go for it. 


---


#### 00:51:17.123

Is it basically that we know that a gene codes for a protein, we have a lot of variation in the genes. The genes can have lots of random differences between them, but we can   
(00:51:30.690) ~~sort of~~(00:51:30.911)  
identify that these are all different variations on the gene. Some of the genetic, some of the DNA level differences may make no difference in the protein, but others will make differences in that at a particular position in the protein sequence, you'll have a different amino acid. And so now you've got   
(00:51:50.371) ~~kind of~~(00:51:50.692)  
the same protein, but it can have different elements in particular position. And so things are grouped for the purposes of prediction.   
(00:52:01.280) ~~Kind of.~~(00:52:01.659)  
So an MSA is actually a pretty old concept that comes from computational biology. 


---


#### 00:52:09.947

People have been using MSAs for a long time. And essentially, it's based on the edit distance. So if I have just a string of characters and I make some edits in some different places, I can compute the edit distance between those. And if I have a low edit distance, then those two sequences are highly similar. MSAs are basically this. I take a protein and I have a whole bunch of different mutations of that protein or a whole bunch of other protein sequences that are very close to that protein in terms of sequence similarity, but they have some changes here and there. A lot of times the changes that happen only happen in certain regions of the protein and then there are other regions of the protein that are highly conserved. 


---


#### 00:52:56.550

And so when you do an MSA you can look at which regions of the protein are really highly conserved and a lot of times this will give you some indication of which parts of the protein are going to affect the function if you like mutate them and stuff. So if I have a highly conserved residue that in my MSA it just doesn't change it stays the same through pretty much all of the MSA. Like 90% of the sequences in my MSA, this amino acid stays the same, right? If I change that, if I mutate that, it's probably going to affect the function of the protein. Because it's like a highly conserved region of the protein that evolution hasn't changed or has changed very infrequently. 


---


#### 00:53:39.217

And so because of that, if you change some of those residues that are highly conserved, oftentimes you'll degrade the function of the protein or change the function of the protein, or maybe you'll decrease its thermal stability or something like that. So MSAs are just telling you, they're telling you evolutionary information that is conserved among a whole group of proteins that are highly similar to each other in terms of sequence similarity. And AlphaFold2 uses MSAs. You can either use the database of MSAs or you can have it compute them on the fly. And it uses these MSAs to inform how it predicts the structure of the protein. Because when you have proteins that are very closely related evolutionarily, in terms of evolution, their structures are often very similar, right? 


---


#### 00:54:27.157

That's not always true. I can have two proteins that are very similar but have very different structures. That happens all the time. But if you have this extra evolutionary information in the form of an MSA, you have extra information that helps you predict the structure of the protein because all of these evolutionarily related proteins are oftentimes going to have very similar structures to your protein of interest. This is   
(00:54:53.007) ~~sort of~~(00:54:53.286)  
calling to mind the classic image of the plane with all of the spots where the planes came back having been shot and then all the places that they didn't observe, those were the planes that got shot down. So this is the evolutionary equivalent of that where we don't see changes in certain regions because they're super core to functionality. 


---


#### 00:55:17.476

And that in turn is super useful for prediction making because that these parts are like the really important parts and they're going to have to fit together or the sort of interactions that they have with other things are   
(00:55:29.922) ~~kind of~~(00:55:30.262)  
the whole point of what's going on here. Okay. So that's interesting. The overfitting piece, I didn't quite understand. It seems like that's related though, where you said because these things are so similar, You have to be careful that you're not, give me the overfitting thing again. Cause   
(00:55:45.090) ~~I can't,~~(00:55:45.371)  
I'm not sure I can do it justice. Like when you do a train test split in deep learning and you're training your neural network   
(00:55:52.396) ~~on your train,~~(00:55:52.976)  
on your training data, and   
(00:55:54.878) ~~you have,~~(00:55:55.239)  
you have your test data to   
(00:55:56.981) ~~sort of~~(00:55:57.300)  
test your model on after the fact, once it's trained to see how well it predicts on data that it hasn't seen before. 


---


#### 00:56:04.286

And so when you're doing this, you want to make sure that your test data doesn't have a bunch of sequences in it that are highly similar to your training data. Because it's almost like you're training on the same thing twice and you overfit this way. You don't get a good indication of how well your model generalizes. And a lot of people do this. A lot of people coming from   
(00:56:24.655) ~~like~~ (00:56:24.795)  
deep learning, just getting into   
(00:56:26.335) ~~like~~ (00:56:26.474)  
the biology stuff and they don't have a super strong background in biology. They make this mistake very often. And so there's just tons and tons of neural networks and different kinds of deep learning models out there. that don't generalize and that are very overfit because they didn't split based on, they didn't split their data based on like sequence similarity and or structure similarity. 


---


#### 00:56:47.847

So you, like when you train models, usually you want to split your data based on sequence similarity and or structural similarity. And a lot of people also split it based on   
(00:56:59.190) ~~like~~ (00:56:59.351)  
dates, like you were talking about CASP earlier. they have like a certain cutoff date and then the stuff that was resolved after that cutoff date is used in the test data. But   
(00:57:09.061) ~~when you're training,~~(00:57:09.981)  
when you're doing your training data, you split your data based on things like sequence similarity and or structural similarity to make sure that you don't overfit and to make sure that your model generalizes to unseen data. Gotcha. Interesting. Okay. Yeah. It seems like in the case of something about this that I don't have a good intuition for because that's not really done in language modeling, right? 


---


#### 00:57:31.175

In language modeling, you could certainly have like lots of sentences that are very similar and you don't   
(00:57:37.458) ~~sort of~~(00:57:38.277)  
say, Oh, we're going to hold out.   
(00:57:40.617) ~~We don't,~~(00:57:40.838)  
we don't draw conceptual lines between different parts of the data and try to generalize across those lines. So what is the difference in the biology context?   
(00:57:51.481) ~~Like~~ (00:57:51.621)  
my intuition says, to the degree that this thing is learning, that these models are learning like the higher order concepts that really matter, that they should be able to learn those kind of regardless. And again, in the language model case, we don't really have a concept of overfitting, at least in large scale foundation models. Is this maybe just because we're not really doing large scale foundation models in quite the same way? 


---


#### 00:58:16.387

Or how would you describe the difference?   
(00:58:18.956) ~~I mean,~~(00:58:19.175)  
there's still a concept of overfitting in, in NLP and training big giant models, Claude or ChatGPT or whatever.   
(00:58:25.559) ~~Like you,~~(00:58:25.838)  
you can definitely still overfit these models. I very often for an NLP models, like these really big chat type models,   
(00:58:33.242) ~~like~~ (00:58:33.362)  
really big LLMs and stuff. First of all, they often only train on one pass through the data, right? They don't do multiple passes. And partially because of that, overfitting is not much of an issue because you're not training multiple times on the same data. So I do think that is changing. One little nugget from the recent Zuckerberg-Dwarkesh interview that I definitely made my ears and brain light up was when he said they trained these latest llama models on 15 trillion tokens. 


---


#### 00:59:02.039

He said, we kind of stopped because we, at some point we need to move on to Lava 4. But he said we could have rotated the high value tokens through again. And I was like, Oh, interesting. I've seen some results about that, but in any event, it does seem there's, we're now to get to 15 trillion tokens. Basically, I don't think you have much choice, but to rotate. Yeah. Anyway, that's a bit of an aside, but I'm still not quite grokking it to be honest. Okay.   
(00:59:27.929) ~~So let's see,~~(00:59:28.831)  
what's a good analogy. I'm trying to think because yeah. And like NLP, like most people don't really think about the, so you have a data distribution and your training data and your test data, like your test data is supposed to tell you something about how well the model generalizes. 


---


#### 00:59:46.740

Right. And it's also supposed to tell you about if the model's overfitting or not, because when you compare your training metrics to your test metrics, whatever they may be. If your training metrics are different, like the training test, or the training metrics and the test metrics are substantially different, then you're either overfitting or underfitting. If   
(01:00:09.208) ~~your test metrics,~~(01:00:10.289)  
if the metrics on your test data are substantially worse than the metrics on your training data, then you've overfit,   
(01:00:21.000) ~~right? And, and if,~~(01:00:22.067)  
if it's the other case, if your test data is substantially better than your training data, which is   
(01:00:28.088) ~~kind of~~(01:00:28.329)  
hard to do, then probably you could train some more.   
(01:00:32.070) ~~Right.~~ (01:00:32.331)  
Maybe you're under fit. 


---


#### 01:00:34.211

So your train test split is supposed to tell you something about how well the model generalizes and how overfit your model is and comparing how it performs on the training data to the test data. tells you that. It tells you a lot about how overfit your model is, if it's overfit, and how well it's generalizing to data that it hasn't seen before. And to really   
(01:00:55.259) ~~get a good grasp,~~(01:00:56.659)  
to get a good idea of how well your model is generalizing to unseen data, you want at least part of your test data to be very dissimilar from your training data. Because that means it's generalizing to things it hasn't seen before,   
(01:01:12.085) ~~right?~~ (01:01:12.246)  
That means it's picked up on some deeper concept in language that generalizes to areas that it hasn't seen before. 


---


#### 01:01:20.641

And it's using those really deep concepts to make predictions or make, generate things that are out of distribution. And this is a big thing that people discuss is   
(01:01:31.804) ~~like~~ (01:01:31.963)  
whether or not these things generalize to data that's out of distribution. And if you train them in the right way. you can get models that generalize well to out of distribution data, right? This is not something that's impossible to do. You just have to do it right. And in the case of biology or biological sequences like proteins, to get a test set that gives you a good indication of one, how well the model is generalizing and two, if it's overfit or not, you need to make sure that your test data is very dissimilar from your training data. 


---


#### 01:02:07.976

And the way that you do this is you look at the sequence similarity between the protein sequences in your training data and your test data. And you can also look at structural similarity, because you can have different sequences that are very different in terms of sequence similarity, but that fold into the exact same structure, more or less, right? We can have two very dissimilar protein sequences that fold into pretty much the same structure. And so sometimes depending on what your model architecture is and what your goal is, you may also want to split based on structural similarity and not just sequence similarity to make sure that your model is generalizing and not overfitting. Okay. I think I got it. 


---


#### 01:02:48.601

Does that make sense? Yeah. I think so. It seems   
(01:02:51.862) ~~that it is sort of~~(01:02:52.882)  
a form of data leakage, essentially. Like you could imagine, and it's   
(01:02:56.842) ~~sort of~~(01:02:57.222)  
that you're fooling yourself, right? For any given architecture, presumably the very best performance would be if you trained on all the data. But in order to effectively evaluate your architectures along the way, you need to have some holdout or you might call it a benchmark in certain contexts to evaluate against. And these similar enough sequences basically are a data leak in the same way that if you find out after you do your thing that, oh, hey, we actually had MMLU in the training data for the language model, then it means, oh, you can't really trust the MMLU scores anymore. 


---


#### 01:03:34.731

And the model still may be good, it may not be so good, but if you train on MMLU, we can't really score you on MMLU. And this is a similar problem. You can't trust her. Exactly. Exactly. Yeah, exactly. And there are even more nuanced ways of splitting the data, too, for specific things. The new version of DiffDoc They trained a new version of DiffDoc, I think they call it DiffDoc L, because it's larger. It's the large DiffDoc. And they use this method called confidence bootstrapping, which is   
(01:04:06.666) ~~sort of~~(01:04:06.927)  
like reinforcement learning. And they also split their data in a really unique way that's based on different domains or motifs that are present in certain interactions. 


---


#### 01:04:20.561

They split their data based on that, in addition to, I think, sequence or structural similarity. I would have to look at that. they split their data based on these domains that are present in these interactions to train a model for docking, right? So you have a ligand, a small molecule ligand that you're trying to dock into a protein and do like blind docking, which is a hard problem. And they get   
(01:04:43.878) ~~like~~ (01:04:44.038)  
substantially better performance and it generalizes a lot better in this new version of DiffDock because of the way that they trained it and the way that they split their data. And they have some really strong confidence that their model is generalizing to out of distribution data. 


---


#### 01:04:59.793

And it's able to predict on things that it hasn't seen before. And they're very dissimilar from what it has seen. Just to make sure I understand,   
(01:05:09.360) ~~when you said, I've lost exactly what you said, but~~(01:05:12.282)  
I just want to make a distinction between what they've demonstrated is that you should be more confident in doing this stuff in totally new regimes based on the fact that they've been very meticulous in the data split. Whereas if they had thrown everything into the training, then you would have a hard time knowing to what degree to be confident in out of distribution stuff. Yeah. Okay. Cool. And they also,   
(01:05:37.610) ~~I mean,~~(01:05:37.769)  
they did a really good job with that model. 


---


#### 01:05:39.413

I think their performance boost was pretty big. They got a lot better performance out of it too.   
(01:05:43.742) ~~So.~~ (01:05:43.862)  
That's definitely a good model to look into if you're looking to get into this stuff. So maybe let's,   
(01:05:49.081) ~~I don't know if there's more that you think we need to cover on.~~(01:05:52.882)  
  
(01:05:53.061) ~~I mean,~~(01:05:53.402)  
we've been up and down the layers of or the levels of abstraction, but it seems like the two big things that I want to go to next   
(01:06:02.425) ~~and~~ (01:06:02.545)  
being mindful that we've already been at it for a while are the diffusion concepts where it seems like we're moving from predicting a structure to generating new things. And then maybe we could get into a little bit of, okay, in actual work, like what are the cycles that are used to actually make progress on questions of interest? 


---


#### 01:06:23.635

Like you have a target, you want to make some modification, like how do these things fit together to allow us to work a lot faster and get more value from our limited work resources? Before we go on to the diffusion and generative side though, anything else that we didn't cover or that you think is   
(01:06:40.621) ~~missing part of the piece,~~(01:06:41.643)  
missing part of the picture for the fundamentals or the structural prediction? No,   
(01:06:46.005) ~~I think,~~(01:06:46.346)  
yeah, we should move   
(01:06:47.306) ~~into,~~ (01:06:47.806)  
into   
(01:06:49.027) ~~like~~ (01:06:49.168)  
RF diffusion. I think that's a good direction to go in now. Are you familiar with RF diffusion at all? No, not really. Although from what little you said earlier, it sounded to me like clip basically. 


---


#### 01:07:01.056

I was sort of hearing that. know with clip you have kind of images and their captions and here it sounds like we have like proteins and their sort of descriptions no so that that's protein dt and molecule stm those are much more like clip they use the exact same method as clip They use contrastive learning and they have captions and molecules or captions and proteins. Those are our text condition models where you can type in a natural language description of your molecule or your protein without a structure or a protein sequence that fits that description. Those,   
(01:07:39.742) ~~I think,~~(01:07:40.523)  
are a bit different from RF diffusion. RF diffusion is a diffusion model that it's not text conditioned. 


---


#### 01:07:48.273

You can condition it on other types of things, but you don't give it a text input. It's   
(01:07:53.119) ~~a little more, I guess,~~(01:07:54.800)  
a little more specific and it's a little more geared towards people who want to perform surgery on proteins. So if you want to design new proteins with specific structural properties and you want to get your hands dirty and perform surgery on these proteins and graft them together or take pieces from this one and graft it onto this one or generate a protein with a specific sort of fold tertiary structure or or maybe generate a protein that binds to a specific protein with really high affinity and specificity. These are the things that RF diffusion is good for. 


---


#### 01:08:32.551

So RF diffusion is a diffusion model. They used Rosetta fold, the Rosetta fold backbone, and trained it as a diffusion model to denoise 3D structures of proteins. And there are several different versions of RF diffusion. There's a new version that just came out called RF diffusion all atom. which allows you to generate proteins that will bind to small molecules. So you can generate proteins with binding pockets that are highly shaped complementary to a small molecule ligand. And with RF diffusion and RF diffusion all atom, you can also do something called motif scaffolding, which is where you pull out motifs from a protein that you like. Maybe they're   
(01:09:15.729) ~~like~~ (01:09:15.850)  
binding sites or active sites, or maybe there's a particular segment of the protein binds to a different protein that you're interested in or performs a specific function. 


---


#### 01:09:26.386

And you can pull these pieces of the protein out and scaffold them and build a new protein around those pieces that holds those pieces in place so that you have a new protein with very specific 3D structure that performs like some very specific function. And it's been a very influential model and a very useful model. And it's definitely one of my favorites.   
(01:09:48.885) ~~Maybe we should dig into that a little bit. Yeah.~~(01:09:50.805)  
Give me a little bit more on how, what exactly it is that you're specifying. It's not text conditioned, but you're saying I want it to have certain properties and then it's filling in the sequence that gets you to those properties. Yeah. So   
(01:10:05.213) ~~like the most,~~(01:10:06.255)  
the most basic usage of RF diffusion is unconditional generation of a protein. 


---


#### 01:10:11.078

So you just, you tell it some length. or range of lengths, and it will just generate proteins of that length that are brand new, that have never been seen in nature before, and very often are very designable and that you can actually synthesize and create in a lab. And that's just completely unconditional generation. You don't give it any sort of constraints. It just generates a new protein for you of a particular length. Then you can also, one of the really interesting functions of RF diffusion is it will design binders for you. So if I have a target protein and I want to design a protein that binds to it with really high affinity and really high specificity, 


---


#### 01:10:56.012

RF diffusion is really good at that. It'll design binders for pretty much any protein you can give it, and very often The proteins that it designs that bind to your target protein are very high affinity and very high specificity and often very thermostable. The other functionality that's really useful is the motif scaffolding that I was talking about before, which is where you pick out pieces of a protein or multiple proteins and you build a new protein that holds all those different pieces in place in a particular way. And so this is one thing that you could imagine doing with this would be like building or designing an adjuvant or like grafting two proteins together. Or let's say I have one part of a protein that binds to protein A and I have some other protein that binds to protein B. 


---


#### 01:11:54.278

I want to design a protein that binds to both protein A and protein B so that I can get a complex with three proteins in it, right? I want to have a protein that binds to protein A and protein B. So what I can do is I can take those pieces out of the protein that bind to protein A, and I can take the pieces that bind to protein B, And I can scaffold them together into a new protein. And now I've got a new protein that binds to both of those proteins. And I can do things like build out protein interaction networks this way. So if I want to design a particular protein interaction network, this is really useful for that. 


---


#### 01:12:27.908

That's a pretty technical and involved thing to do. Like building up a protein interaction network is a non-trivial thing to do, but you can do it with RF diffusion. You can design proteins that will bind to multiple different proteins in multiple different contexts and build out these networks this way. And this gives you   
(01:12:48.896) ~~like~~ (01:12:49.037)  
a way to modulate protein interaction networks, right? Because if you design a binder to block a particular interaction, you can modulate your protein interaction network by blocking particular interactions by designing a binder. But you can also add in interactions that weren't there before using the motif scaffolding or maybe binder design and motif scaffolding together. So it's very useful in a lot of different contexts, but it's not text-conditioned like ProteinDT or MoleculeSTM or some of the other text-conditioned diffusion models for proteins, because there are a few others now that recently came out as well. 


---


#### 01:13:24.271

But yeah, it's not text-conditioned. It's very much more geared towards people who are really interested in performing surgery on proteins and protein interaction networks. And now with RF diffusion all-atom, also with other interactions as well, because with the all-atom models, you can model more interactions than just the protein interactions. So how does this in practice get used? Maybe the cancer example from the top is a good one, or we could go to another one, but... Yeah. in that scenario we sort of already had an understanding of the cancer cell has this thing that disables the immune cell and so then you could say okay Let's brainstorm some ideas here, right? If we can bind something to that bit of the cancer cell that would   
(01:14:17.515) ~~kind of~~(01:14:17.775)  
cap it, blunt its ability to then interfere with the immune cell, then the immune cell presumably would do its job still and kill the cancer. 


---


#### 01:14:25.563

Of course, you've got highly tangled webs of interaction that you're doing this within. but you've got to take something local like that. Now kind of take me through the cycles and the practical application of some of these tools for a specific problem of that sort. Yeah, so I've got a few examples here that we can talk about. I wonder which one would be   
(01:14:46.615) ~~like~~ (01:14:46.775)  
the best or the most interesting for people. So like the one that we were talking about earlier with the cancer, with PD-1 and PD-L1 as a really good first example that I think is a really good place for pretty much anybody to start. Because you can very easily and very quickly design a binder to one of these proteins with RF diffusion. 


---


#### 01:15:06.118

It's really good at designing binders for pretty much anything. If I have this PD-1, PD-L1 interaction between these two proteins, essentially what's happening is the cancer is turning off your immune system's response to it, and then your immune system doesn't effectively combat the cancer. But if I design a binder to one of these two proteins to block that interaction, and my binder out-competes that interaction, so it has a higher affinity than the PD-1, PD-L1 interaction has, then I can successfully block that interaction and prevent the cancer from turning off the immune cell's responses to it. So that's a really good place to start. Another way that RF diffusion can be used, so let's say you have a protein that binds to a target, but it doesn't bind very well. 


---


#### 01:16:41.355

And if I do this and I give RF diffusion the target protein that I'm interested in, I can improve the shape complementarity between those two. So the new denoised protein or the new denoised version of my original protein is going to have a higher shape complementarity to my target. And then I can go and design sequences for that backbone that are different from my starting sequence, right? So maybe my starting sequence, maybe there were some residues that had unfavorable chemical properties at the interface,   
(01:17:11.631) ~~right?~~ (01:17:11.851)  
Maybe I need to use different amino acids to improve some chemical properties so that the binding affinity goes up,   
(01:17:20.595) ~~right?~~ (01:17:20.775)  
I can do that with protein MPNN or ligand MPNN. 


---


#### 01:17:25.011

So ligand MPNN is the newer all-atom version of protein MPNN. It's an improvement on protein MPNN, and it also generalizes to contexts where you have other kinds of molecules other than just proteins. And I design a sequence with ligand MPNN, and I can tell ligand MPNN to bias certain residues towards certain amino acids or away from certain amino acids, like at the interface, for example. to get those more favorable chemical properties to increase my binding affinity further. And   
(01:17:58.627) ~~I can also,~~(01:17:59.328)  
there's also versions of ligand and PNN that will allow you to specify   
(01:18:03.190) ~~whether a residue, so let me check on this really quick, whether a residue is~~(01:18:08.095)  
a buried residue, an interface residue, or something else. 


---


#### 01:18:12.597

I can also tell ligand and PNN about symmetries, which is a really interesting thing that RF diffusion and ligand and PNN can do together. Just to clarify, RF diffusion doesn't usually get used on its own,   
(01:18:26.457) ~~like~~ (01:18:26.617)  
by itself, because it just works in structure space, right? So it's doing the denoising process on the structures of the proteins. It doesn't know anything about the sequence of the protein. So I need a separate model, like Ligand and PNN, to design the sequence for that 3D structure. So they   
(01:18:44.952) ~~kind of~~(01:18:45.212)  
go hand in hand. You use them together. So once you've generated your 3D backbone of your protein, you design a sequence for it using ligand and PNN. 


---


#### 01:18:55.788

And using these different functionalities of ligand and PNN, you can increase your binding affinity and other properties even more. Yeah, so like using partial diffusion with RF diffusion to slightly noise and then denoise a structure that you already have. can help you increase things like binding affinity and things like thermostability and other properties. Then,   
(01:19:16.568) ~~let's see,~~(01:19:16.889)  
what's another application of RF diffusion? So one that I was looking into recently,   
(01:19:23.672) ~~let's see, I want to pick out a good one because I want to give people really interesting examples to think about because you can really do a lot with these models if you get into it pretty deep and really learn how to use them. Let's see, there we go.~~(01:19:36.541)  



---


#### 01:19:37.358

Okay, yeah, so there's unconditional generation, symmetric generation. I touched on that a little bit. You can design symmetric oligomers. Let's say I want to have a protein that interacts with itself, or other copies of itself, I should say. And if I have enough copies of this protein, it forms a symmetric complex. For example, Let's say I have a protein that fits together with two other copies of itself in a triangle formation,   
(01:20:11.326) ~~right?~~ (01:20:11.506)  
And it's symmetric to the cyclic group of order three,   
(01:20:15.769) ~~right?~~ (01:20:16.029)  
So I've got a order three rotational symmetry that's happening. I can use RF diffusion to generate proteins with symmetry like this. And it has other symmetries that it can use. So there's dihedral symmetries, there's symmetries icosahedral symmetries and tetrahedral symmetries in addition to the cyclic symmetries. 


---


#### 01:20:36.765

And I can, the cyclic and the dihedral, I can choose like any order, cyclic group or dihedral group for my symmetry for those. And RF diffusion will design a symmetric complex of proteins where there's like multiple copies of the protein in this   
(01:20:53.890) ~~like~~ (01:20:54.051)  
nice symmetric structure. And where this occurs,   
(01:20:57.192) ~~like~~ (01:20:57.332)  
this occurs in nature, in multiple places. One example is in viral capsids. And they've also recently, some David Baker's lab recently published some work where they design these   
(01:21:11.198) ~~like~~ (01:21:11.378)  
symmetric oligomers as   
(01:21:13.939) ~~like~~ (01:21:14.100)  
biosensors. And I think they also designed some to help with   
(01:21:19.304) ~~like~~ (01:21:19.444)  
drug delivery. So they have these like the like pocket that forms when you have a cyclically symmetric complex of proteins, the pocket that forms inside of that. 


---


#### 01:21:31.346

You can design that in such a way that it captures a small molecule drug really well and delivers it to somewhere in particular, right? So that's another application of RF diffusion that's really useful. What else? There's the binder design. Fold conditioning, which is where you can tell it like specific tertiary structures to condition on. Maybe I want to design something like a TIM barrel. I can tell RF diffusion to generate something that has the rough 3d shape of a TIM barrel. What else can I do? Can I ask what that is? Yeah. Maybe a picture would be a better way of explaining it. Maybe if we just look at a picture on Google of a TIM barrel, it's just T I M and then barrel,   
(01:22:15.411) ~~like a,~~(01:22:15.730)  
like a barrel that like you put water in or something. 


---


#### 01:22:18.992

Let's see if I can find a good picture of one. If you haven't found one. Go. Yeah. Here's a good one. So it's   
(01:22:23.813) ~~like this,~~(01:22:24.153)  
it has   
(01:22:24.713) ~~like~~ (01:22:24.873)  
beta sheets in it. and they form this   
(01:22:27.632) ~~like~~ (01:22:27.913)  
sort of barrel-shaped protein. Let me see if I can send this to you so that you can see it. Yeah, I've got a couple pulled up as well. Okay. We can add one to the...   
(01:22:37.717) ~~I mean,~~(01:22:37.938)  
I can even share here in the moment just to capture what I'm looking at. Yeah, maybe let's share. Do that. So this is an 8. And if you turn this sideways, yeah, if you turn this sideways, it should look kind of like a barrel. 


---


#### 01:23:36.481

There's two different proteins that are interacting with each other, p53 and mdm2. And if I want to design an inhibitor for this, maybe I could   
(01:23:45.365) ~~like~~ (01:23:45.525)  
could extract the motif corresponding to the p53 peptide and then use that to design a new protein, scaffold that with the motif scaffolding. And then I can optimize it using partial diffusion and ligand and PNN to design sequences that have favorable chemical properties. And then I can check and see using the LIS score from alpha-fold multimer how well my new protein interacts with MDM2 or p53.   
(01:24:19.591) ~~These are so technical, I hate to just read these off, but I feel like I'm just going to go into the weeds and talk about a bunch of really specific proteins and domains and stuff.~~(01:24:28.993)  



---


#### 01:24:29.014

I don't know if that's very interesting. The sort of conceptual loop,   
(01:24:33.194) ~~I think,~~(01:24:33.395)  
is really interesting. And if I'm getting it, it's like, okay, we have an interaction that is problematic. we want to interfere with it one way or another. We can   
(01:24:43.858) ~~like~~ (01:24:44.057)  
cap the one thing or cap the other thing. And so there's this kind of cycle of generate a 3D structure. That's one model. Generate a sequence to do that. That's another model. Refine those. That's,   
(01:24:56.502) ~~I guess,~~(01:24:56.762)  
yet another model to look for various refinements or   
(01:25:00.744) ~~kind of,~~(01:25:01.005)  
as you said, chemical, favorable chemical properties, same thing? No, you don't need another model for that. You can just RF diffusion and ligand and PNN, you can do it with those two. 


---


#### 01:25:10.695

You don't need anything else really. So RF diffusion designs the structure and then ligand and PNN designs the sequence for that structure that will fold into it so that you have something you can actually go and synthesize in a lab, right? You need a protein sequence to synthesize to get the protein structure because RF diffusion just works at the level of structure. It doesn't know anything about sequences. And then you're validating this to the degree that you can validate it before you're actually doing any actual lab work,   
(01:25:39.045) ~~um,~~ (01:25:39.145)  
with something like multiple and looking for a high score there.   
(01:25:44.010) ~~How,~~ (01:25:44.270)  
so how quick does this happen? It seems like we're talking orders of magnitude speed up compared to the pre AI way of doing this. 


---


#### 01:25:55.341

And how accurate is it? Yeah, I mean, RF diffusion, like I can generate a single backbone in a minute, even like a pretty big one. It just takes a minute to generate a backbone. And if you have a really good GPU, that's way faster, right? If I'm just working on my laptop or something,   
(01:26:11.175) ~~like~~ (01:26:11.295)  
I can generate something in just   
(01:26:12.555) ~~like~~ (01:26:12.694)  
a minute. And then ligand and PNN is significantly faster than that. So like designing the sequence for the 3D structure is actually really fast.   
(01:26:20.198) ~~So, you know,~~(01:26:21.418)  
like per protein. And per sequence, it's less than a couple of minutes to do that whole thing. And so I can design hundreds of thousands of backbones and then design hundreds of or thousands of sequences for each backbone with ligand and PNN. 


---


#### 01:26:37.219

So it's pretty fast and pretty computationally efficient. And they've made some improvements to RF diffusion to reduce how many time steps you need to actually get a good structure out of it. And time again, when they actually synthesize these and check for   
(01:26:50.381) ~~like~~ (01:26:50.622)  
thermostability or specificity or binding affinity, very often they're very high. And if I have   
(01:26:58.463) ~~like~~ (01:26:58.583)  
low thermostability or low binding affinity or low specificity, very often when I use these models to improve that, they improve it dramatically. So they're pretty effective, and they're not perfect, but they're pretty good. It's not a hard thing to do to design a protein with RF diffusion and then design a sequence with ligand and PNN and get something that really does fold into that structure with high confidence or that really does interact with my target protein with high affinity and specificity. 


---


#### 01:27:31.439

Yeah. So how does this then fit into the broader like validation loop. You have this one thing you're like, going back to our cancer example, right? Oh, this part of the cancer cell interacts with this part of the immune cell and disables it. So we want to put essentially a physical cap on that thing. So that is blocked and that can't happen and the cancer can get Okay, cool. So I'm going to generate potentially thousands of shapes, thousands of sequences per shape, then potentially run millions of things through an alpha fold multimer, getting scores. And then what do I do at the end of that? Do I take like the top hundred and go actually try them in a living cell? 


---


#### 01:28:15.225

Yeah, exactly. And so this seems, and you're saying they tend to work. And then I guess we also have questions of like side effects would be another big downstream question, right? We don't know what else this thing could do when put into the full environment of the cell.   
(01:28:31.627) ~~Well, that's where this,~~(01:28:32.228)  
the specificity comes in, right? Generally speaking, RF diffusion is capable of designing binders, for example, with really high specificity. So they bind to the target and pretty much only bind to the target. Yeah. And that's a really good thing, right? Because   
(01:28:47.014) ~~if you have a, if you,~~(01:28:48.454)  
design a binder that just interacts with a whole bunch of other stuff, it may never make it to the target. 


---


#### 01:28:53.336

It may cause other side effects, like you're saying, have off-target effects. But yeah, RF diffusion is pretty capable of designing really high-specificity binders. The motif scaffolding, there's more nuance there because you're performing surgery on proteins and pieces of proteins. And so that can get a little more nuanced and a little more complicated. But if you're just designing a binder, with RF diffusion, it's pretty easy to design one that has really high specificity and that doesn't have a lot of off-target effects and stuff. What's the bottleneck on this process? Is it identifying targets? Especially if you can design things that are that specific and they don't have much in the way of other knock-on effects.   
(01:29:36.738) ~~I mean,~~(01:29:36.917)  
it seems like we should be curing a lot of diseases pretty quick here. 


---


#### 01:29:40.761

I think, I mean, diseases are pretty complicated and sometimes it's not just one thing that you're targeting. Sometimes it's multiple targets and multiple kinds of interactions. And so you have to think in terms of   
(01:29:52.570) ~~like~~ (01:29:52.791)  
entire   
(01:29:53.471) ~~like~~ (01:29:53.631)  
protein interaction networks or even like interaction networks that involve other molecules as well and modulating those in very specific ways. And often figuring out what parts of a protein interaction network to change or to modulate and how to do that, like what sort of changes you should make to this interaction network, that's a pretty complicated problem. And so I think part of it is   
(01:30:18.047) ~~identifying, like you said,~~(01:30:20.048)  
identifying targets or identifying specific targets within an interaction network, because some of the interaction networks can get really complicated. 


---


#### 01:30:28.613

And figuring out which parts of them to modulate is not an easy thing to do. And then Computationally, there isn't much of a bottleneck. If you just have a good GPU, you don't really need multiple GPUs even. You just have a good H100 or something. You can get a lot done with that.   
(01:30:45.851) ~~You can get quite a lot done with that~~(01:30:47.532)  
with RF diffusion and NPNN. The hardware requirements are not very taxing.   
(01:30:54.295) ~~I mean,~~(01:30:54.475)  
They're probably a little less efficient than I would like them to be, because   
(01:31:00.564) ~~I guess~~(01:31:00.804)  
most average people are not going to have access to an H100. A lot of people are going to be using much lower tier GPUs and stuff. 


---


#### 01:31:12.046

But like RF to Fusion, for example, there's a Colab notebook that you can run on a T4. You can run it in Google Colab. And it takes a little while. It's not as fast. The computational bottleneck is not a huge bottleneck right now.   
(01:31:25.938) ~~I think~~(01:31:26.217)  
it could be a little better, but   
(01:31:28.019) ~~I mean,~~(01:31:28.220)  
the models aren't huge models. These aren't like billions of parameters, right?   
(01:31:33.002) ~~I think~~(01:31:33.243)  
RF diffusion has a couple hundred million parameters or something like that, or an alpha fold, same thing.   
(01:31:39.606) ~~Like~~ (01:31:39.787)  
it's a couple hundred million parameters or something. So they're not really big models that require really excessive hardware to do the computations. And   
(01:31:48.391) ~~I think~~(01:31:48.632)  
the slowest part of that pipeline. you like design binders or design motif scaffold with RF diffusion or partial diffusion or what have you and then designing the sequence with   
(01:32:00.112) ~~like~~ (01:32:00.252)  
protein NPNN or ligand NPNN and then validating with   
(01:32:03.634) ~~like~~ (01:32:03.753)  
alpha fold or alpha fold multimer, the slowest part in that whole thing is actually the alpha fold multimer part or the alpha fold two part where you're validating and   
(01:32:13.417) ~~like~~ (01:32:13.557)  
predicting the structure of whatever you've generated and designed with the other two models. 


---


#### 01:32:19.828

That's actually the slowest part in the whole thing. If you're able to predict a lot of structures with AlphaFold, then you're fine. There's no real computational bottleneck there. And as far as   
(01:32:31.329) ~~like,~~ (01:32:31.550)  
why are we not curing a bunch of diseases? A lot of this also has to do with how long it takes to get these things to market. and the traditional system that's set up right now for drug discovery and protein therapeutic, it's hard and slow to get new things through.   
(01:32:51.280) ~~Like it's a~~(01:32:51.801)  
very slow system. And   
(01:32:53.381) ~~I think~~(01:32:53.720)  
it wasn't designed for high throughput methods like this. It wasn't designed for   
(01:33:00.422) ~~like~~ (01:33:00.583)  
large high throughput methods. And it just, it takes a lot of time to get a new drug or a new protein therapeutic through and approved and get it through all the testing, like the different clinical testing phases and stuff like that. 


---


#### 01:33:15.493

That's part of it. That's probably a big part of it. Are we like stuffing the pipeline at this point with new things?   
(01:33:22.077) ~~I mean,~~(01:33:22.237)  
it seems like the biggest reason that this used to be a hard thing, of course, it's like slow and there's a lot of like safety, perhaps redundant steps in there, especially if you could say, hey, we have like very high confidence that this is a highly specific thing.   
(01:33:36.779) ~~I mean,~~(01:33:36.920)  
that would really do a lot to inform   
(01:33:40.240) ~~the~~ (01:33:40.400)  
what the safety profile might be. But even if you, not even if, but in the past, it's like the biggest problem was like either it wouldn't work, right. Or it would have side effects that were like intolerable. 


---


#### 01:33:53.005

And if you could take both of those things, not entirely off the table, but if you could   
(01:33:56.827) ~~sort of~~(01:33:57.067)  
say, Hey, we can be much more confident now, seemingly like at least in order of magnitude, more confident that any given thing is going to do what you expect it to do and that it won't do other things that you don't want it to do. you can improve both of those by an order of magnitude, then it's your seemingly two orders of magnitude more likely for things to work, which would take you from sub 1% a lot of shooting in the dark to a lot of the clinical trials would be expected to work. Is that the era that we're entering into now where clinical trials should go from like roll of the dice to you be more like disappointed when they don't work. 


---


#### 01:34:38.091

Yeah.   
(01:34:38.331) ~~I mean,~~(01:34:38.551)  
I think we're definitely moving into an era where all this stuff is going to speed up a lot. And   
(01:34:43.813) ~~I think~~(01:34:44.132)  
so there are   
(01:34:45.353) ~~like~~ (01:34:45.533)  
a lot of situations where you want to understand more than just a static structure. Like we've been talking about   
(01:34:51.414) ~~like~~ (01:34:51.574)  
having models that give you more dynamic information and stuff like that. And those are so recent that they haven't really been adopted by a lot of people. yet. And I think once those get used more, that'll speed things up a lot and improve things a lot as well. But yeah, I think also part of it is just adoption. A lot of researchers are not using this stuff yet because it's so new. 


---


#### 01:35:15.528

And a lot of researchers don't understand how to use these models effectively or how to use them at all. It does seem to be quite a different skill set.   
(01:35:23.569) ~~I mean,~~(01:35:23.930)  
I've actually studied chemistry as an undergrad. It really is. Yeah. And the kinds of things that I was taught to do were like not at all running the loops. There were no notebooks involved or no collab notebooks involved. It was like physical techniques for separating chemicals from one another was a big part of where the time went. Yeah. And that's a whole other thing too, like drug synthesis and small molecules is like a whole other story that we can get into. But because there are like really interesting diffusion models out for those as well that'll generate molecules with specific properties. 


---


#### 01:35:56.582

But Yeah, I mean, it's a very new and a very unique skill set that there aren't a lot of people that are training people to do this. There isn't a ton of information out there about how to use them. To some degree,   
(01:36:10.934) ~~I mean,~~(01:36:11.113)  
there are some platforms that are popping up and some different tools that are popping up that are making these things a lot more accessible. One that I would mention is 310AI is working on a tool that they're calling Copilot. And   
(01:36:26.158) ~~it's essentially,~~(01:36:27.099)  
it's like a chat interface that uses tools.   
(01:36:31.761) ~~So it,~~(01:36:32.242)  
you can talk to it in natural language, like you talk to the chat GPT or something. And then   
(01:36:38.305) ~~it,~~ (01:36:38.345)  
it knows how to use   
(01:36:39.905) ~~like,~~ (01:36:40.145)  
like function calling   
(01:36:42.306) ~~to,~~ (01:36:42.747)  
to use other models as tools. 


---


#### 01:36:46.189

So you can say, generate a protein with such and such property. And then it'll use a particular model to do that, generate some protein with that particular property. And then you can say   
(01:36:56.930) ~~like~~ (01:36:57.090)  
increase binding affinity with such and such protein and it'll modify your protein for you to increase the binding affinity or something. Or you can say dock this small molecule to this protein and it'll call on diff doc and dock the small molecule to the protein for you and then return that. And that's all using like a chat interface, which is making a bunch of these models a lot more accessible to people. And I think that's going to have a huge impact in the near future. 


---


#### 01:37:24.106

So. Depending on how good that gets and how fast it gets really good, that's probably going to change things substantially. And right now, it's pretty good already. And it uses a pretty wide range of tools for different things. It'll use protein MPNN or ligand MPNN to design sequences for a structure. I'm not sure if it uses RfDiffusion yet, but they probably are going to start including RfDiffusion and some other models as tools for it as well, because they just keep adding more tools to it, more models that it uses as tools. And   
(01:37:58.938) ~~I think~~(01:37:59.337)  
once they have a good   
(01:38:01.099) ~~section or a good~~(01:38:02.139)  
selection of tools for it to use, that'll be really good. And that'll lower the barrier to entry for a lot of people. 


---


#### 01:38:09.846

Because right now you've got to go through this like somewhat complicated process of setting up these models. And   
(01:38:16.431) ~~you have to know,~~(01:38:17.192)  
you don't have to know a lot of coding, but you do have to code some and you have to understand how to set these things up   
(01:38:24.216) ~~in,~~ (01:38:24.317)  
in   
(01:38:24.777) ~~like~~ (01:38:24.936)  
a conda environment or something like that a lot of times. And so if you're not coming from   
(01:38:29.420) ~~like~~ (01:38:29.560)  
a programming background or you don't have some experience with programming, like a lot of these models are   
(01:38:35.824) ~~kind of~~(01:38:36.085)  
hard to touch. They're hard to use because   
(01:38:38.606) ~~you.~~ (01:38:38.667)  
You can't really use them unless you know a little bit of coding at least. But so 3.10 AI, 


---


#### 01:38:43.604

I think is going to change a lot of that and make a lot of these models a lot more accessible over time and really increase adoption of these techniques. And   
(01:38:51.591) ~~I think~~(01:38:51.871)  
that's going to be really big and important because adoption right now is pretty limited,   
(01:38:56.796) ~~I would say. I mean,~~(01:38:57.756)  
just using a really simple metric by if you just look at   
(01:39:02.261) ~~like~~ (01:39:02.421)  
how many views a YouTube video on RF diffusion gets. It's not that many, right? There aren't that many people watching. This is going to be the one that goes viral and changes it all. I hope so. That would be great because adoption is going to be big. I think because the more creative people you get using these things, the more you're going to see creative uses of them and like novel approaches to solving problems that people weren't even thinking of before. 


---


#### 01:39:28.679

Like when have you been able to design proteins that build out complicated protein interaction networks using binder design and motif scaffolding. That's just so brand new within the last couple of years that the adoption just hasn't caught on yet. So hopefully more people will start experimenting with these models and really learn how to use them well. And we'll see a lot of really interesting novel techniques popping up in the near future. Yeah, that's pretty remarkable. So it seems like the problem then shifts to the, or maybe it was always there in the first place, but if it is the case that given a target, we can pretty reliably and   
(01:40:10.404) ~~like~~ (01:40:10.545)  
even relatively computationally efficiently come up with something that will hit the target, not hit other things, not cause a lot of collateral damage. 


---


#### 01:40:20.511

Now it's like target identification becomes the thing that really. matters the most. And this seems like it's happening in a lot of areas at once. Certainly,   
(01:40:28.944) ~~I mean,~~(01:40:29.345)  
terrible analogy, but to thinking about a military environment, we've got really good missiles that can hit very precise targets, but then the targeting obviously becomes the high stakes decision. And   
(01:40:41.110) ~~I mean,~~(01:40:42.230)  
in lots of just business operations context too, right? Figuring out the right thing to do is often the hard part. So what do you think are the prospects for that sort of thing? I've been   
(01:40:52.917) ~~kind of~~(01:40:53.136)  
working through this and thinking, we've got quite a tech stack for, obviously we can sequence lots of DNA. We can also pull out from an individual cell now, what was the state of the transcriptome, what genes were being expressed at any given time, what proteins were being created. 


---


#### 01:41:13.850

I don't know quite the degree to which we can do that with small molecules, with a really localized sample, But it seems like   
(01:41:21.469) ~~we're,~~ (01:41:21.668)  
we've got like a lot of ability to generate a lot of data and to probably then create a foundation model of some sort. This is   
(01:41:31.796) ~~kind of~~(01:41:31.976)  
where Evo, I sort of sense is going, even though that's not even doing all this stuff yet, but already,   
(01:41:38.322) ~~I mean~~(01:41:39.483)  
with, let me just give my understanding of Evo and you can correct me if I'm wrong, but basically they're training a language model on DNA sequences. purely bacteria and phage DNA from what I understand. And yeah, I was a little disappointed by that. 


---


#### 01:41:57.490

But I think part of their reason for doing such a like specific selection was for safety reasons. I think they're like trying to be a little cautious about what they train on and what the model is capable of doing for for safety reasons. But I was a little disappointed that they only trained on that data, for sure. Hopefully, there'll be another version at some point that's train on other data as well, but yeah. I'm sure there's a lot more to come.   
(01:42:23.632) ~~You kind of glitched on me for a second, but~~(01:42:25.233)  
so they train on all this data. Now they can generate sequences in the same way that a language model can generate text, right? In autoregressive, byte-by-byte, base-pair-by-base-pair generation. 


---


#### 01:42:39.819

And then there's these really interesting things that they can do downstream of it where, for example, a gene essentiality score or test Basically, if you change a sequence in a particular gene and generate from that changed sequence It seems that the model has developed a sort of, as we've talked about a couple of different contexts, this sort of higher order understanding of how things fit together, such that if you do make a change to something that really matters, then you see   
(01:43:16.375) ~~sort of~~(01:43:16.614)  
an unraveling of the later generation. You see a very high perplexity downstream of this changed sequence. And that reflects the fact that, hey, if you've changed that sequence, I can't really make any confident predictions now because we're   
(01:43:32.860) ~~sort of~~(01:43:33.180)  
outside of the set of things that can work. 


---


#### 01:43:36.542

And so once you change that, it's all kind of noise. Whereas if you change something and predictions remain confident downstream, then you infer that must not have been super important. That was an area that more easily could be, change could be tolerated in that particular sequence because, and we can infer that from the fact that it continues to make confident predictions downstream. That's pretty remarkable stuff that suggests to me that especially as we scale up the data set a lot more, which in this one was 300 billion.   
(01:44:10.533) ~~I mean,~~(01:44:10.672)  
that's not nothing, but it's not much compared to what we could easily imagine doing. Certainly not much compared to the 15 trillion tokens that Mediterranean Plasma 3 on, but then also like more modalities, right? 


---


#### 01:44:21.197

I mean, we're seeing this in the language models where you can have obviously language integrated with image and plenty of other things. Audio now it fits into Gemini 2. It seems like you   
(01:44:30.319) ~~sort of~~(01:44:30.560)  
imagine from just the DNA to   
(01:44:34.061) ~~sort of~~(01:44:34.402)  
the DNA and maybe the transcriptome or the proteome or whatever the sort of state of a cell is. You can even imagine scaling this up another degree to   
(01:44:45.082) ~~sort of~~(01:44:45.304)  
the systems level too. But to learn to predict the next state from the current state seems like we're getting really close to being able to do that. I would   
(01:44:58.569) ~~kind of~~(01:44:58.789)  
expect that in the next couple of years at most, we would start to see large scale foundation models for biology that would predict like how a cell will evolve through time, how a system level description would evolve through time. 


---


#### 01:45:14.702

And then you can start to do these like counterfactual hypothetical perturbations and see, okay, if we change this, then how will that make things evolve? If we change this, how will that make things evolve? And so then   
(01:45:26.045) ~~I guess~~(01:45:26.265)  
what we would expect to be learned by those systems is what is now the black box, right? Of all these like interactions that we have only mapped out like whatever, 5% of. And then you could even imagine a situation where you start to do interpretability techniques on digital neural networks to then figure out what the actual pattern of interactions is in the actual biological systems. So is that where this is going over the next couple of years? 


---


#### 01:45:54.376

I mean, and then it seems like if we can achieve that, then you kind of have a fairly closed loop of, okay, we can now identify good targets at a pretty high rate. We can identify or design interventions that are pretty likely to be successful. The like specificity is already high.   
(01:46:12.805) ~~I mean, it's,~~(01:46:13.704)  
we're entering into sort of a super steep part of the S curve in terms of not just   
(01:46:19.027) ~~like~~ (01:46:19.167)  
understanding biological systems, but really being able to intervene in them. And it just seems like a totally different regime that we're headed for. So is that what you basically expect to see over the next couple of years?   
(01:46:29.970) ~~I mean,~~(01:46:30.171)  
I hope so. I hope that all of that comes to reality or comes into existence. 


---


#### 01:46:34.512

Sorry. We pause for a second. I need to get some water. OK, hold on just a second. We're back. OK,   
(01:46:40.543) ~~I think we're~~(01:46:40.904)  
I think we're all set. Yeah. OK, I'm feeling a little better now. So where were we?   
(01:46:46.367) ~~What were we talking about?~~(01:46:47.268)  
You were hoping that my seemingly I'm like extrapolating from where we are and I'm also   
(01:46:53.155) ~~sort of~~(01:46:53.536)  
mapping what has happened with language model foundation models onto the biological domain and feeling like it's about to get crazy. So you're hoping that happens.   
(01:47:05.204) ~~I, yeah. I mean,~~(01:47:06.645)  
I think it's about to get crazy for sure. I think like we're fast approaching a scenario where all of these technologies are going to   
(01:47:13.551) ~~kind of~~(01:47:13.792)  
converge and we're going to have a lot of power over. editing and modifying our biology. 


---


#### 01:47:20.082

I think that's a very exciting thing because there's a lot of problems that I really want to see solved in my lifetime. I think we are definitely moving in the right direction and I think we are fast approaching a situation where we can actually solve a lot of these problems. The main thing that you're talking about is this complicated hierarchical structure that's happening. The level that   
(01:47:47.185) ~~I think~~(01:47:47.604)  
at most of the time is at the level of molecule interactions. But you can definitely take that up another level and look at how those interactions come together in a network to create a particular phenotype or to create a particular state of the organism. And some of those states are diseased states that we don't want. 


---


#### 01:48:16.689

Figuring out how to modify these interaction networks, I think, is somewhere that we really need to focus on a lot. And one thing that's really useful and that I really want to see pushed further is this notion of LIS score with AlphaFold and Ultimer, and seeing also things like AlphaFlow or distributional graph former generalized to complexes, to complicated complexes of molecules, and not just one or two proteins or something. I really want to see more progress happen there because once we understand all of the interaction networks and we're able to modulate them in very specific ways,   
(01:48:59.118) ~~we're going to solve a lot of problems,~~(01:49:00.779)  
a substantial amount of problems. Modeling these interaction networks is becoming possible now. 


---


#### 01:49:07.042

I think before alpha-fold multimer, and before some of these other docking methods, and before RosettaFoldAllAtom came out, we really didn't have the tools to model all of these different interactions. But we have very recently just hit a point where we do have most of the tools that we need, if not all of them, to model all of these interactions. And once we implement something like alpha flow or distributional graph form for complicated complexes of molecules, that's really going to be pretty substantial. And   
(01:49:43.323) ~~I personally,~~(01:49:44.123)  
I'm not sure how I would approach the problem of determining what specific interactions or interaction networks to modulate.   
(01:49:54.970) ~~I Like,~~(01:49:56.895)  
I personally, like, that feels like such a big problem to me. 


---


#### 01:50:01.235

But I also know that there are a lot of biologists that know specific interaction networks they want to modulate, and they want to modulate them in very specific ways. And there's a lot of that. And now we can do that. I think we just need to get these tools into the hands of those biologists and make them really accessible. Because they're not super accessible yet.   
(01:50:26.769) ~~They are kind of, right? I mean,~~(01:50:28.489)  
like a lot of them are open source and they're out there and you can get the model weights and a lot of them have the training code and the inference code and all this stuff available. But probably your average biologist is not going to know how to use those tools right now. 


---


#### 01:50:44.582

So making them accessible and easy to use is really where a lot of the work is going to be as well. Because there are a lot of people that want to do these things, but   
(01:50:55.791) ~~they don't~~(01:50:56.331)  
they haven't quite gotten to the point where they've adopted all of these tools yet. And also figuring out how to use them all in tandem with each other,   
(01:51:06.180) ~~right?~~ (01:51:06.400)  
Because you don't want to just use one of these models. You want to use multiple and use them all together to solve a problem. And so that requires you to learn   
(01:51:17.283) ~~like~~ (01:51:17.404)  
multiple different models and how they work and how to use each one of them. And that's not an easy thing to do for a lot of people. 


---


#### 01:51:24.389

Yeah.   
(01:51:24.649) ~~The, I mean,~~(01:51:25.088)  
this is an issue in AI, even in much more,   
(01:51:28.011) ~~you know,~~(01:51:28.350)  
simple use cases of just using chance UPT effectively, the sort of diffuse, the technology diffusion through society   
(01:51:34.635) ~~is,~~ (01:51:34.795)  
is really the big bottleneck I would say right now to when people say   
(01:51:38.698) ~~like,~~ (01:51:38.818)  
why hasn't, if change UPT is so great,   
(01:51:40.618) ~~like~~ (01:51:40.738)  
why hasn't it,   
(01:51:41.519) ~~you know,~~(01:51:41.779)  
changed productivity all that much? It's like, people are not using it nearly as much as they could is one really big reason. So a huge reason. Yeah. If I had to kind of map out the story of the next couple of years, as I understand it, or as I'm kind of piecing it together from everything that you're teaching me about, it is right now we have a big backlog of targets. 


---


#### 01:52:02.411

And we have a pretty robust new set of tools that used together can design things that will hit those targets and not create too much collateral damage such that it's not super hard. It's hard to learn to use the tools. But once you have the skill set, it becomes relatively easy to take a target and crunch through a bunch of iterations and come to a bunch of candidates. And those are likely enough to work that we should start to see serious acceleration of the ability to find the solutions to these well-posed problems. And then   
(01:52:50.926) ~~sort of~~(01:52:51.127)  
in parallel, we should probably also expect that Evo 5 or whatever, Evo 4 will be capable of dramatically better holistic modeling of the overall networks. 


---


#### 01:53:08.056

And that will then, once we sort of deplete the current set of targets, that have been painstakingly worked out through non AI methods   
(01:53:20.069) ~~sort of seems, I don't know.~~(01:53:21.010)  
Why does it always seem like it happens at the same time? It's always these sort of gradual overlapping curves, but my gut says we've got a few years in front of us of. depleting the current, or not depleting, but like picking the sort of low hanging fruit of, hey, we've got all these targets out there and now we've got good methods to hit those targets. That's going to take a while for people to learn the tools, do it, obviously validate it, run clinical trials going in lots of different areas. 


---


#### 01:53:45.958

And then as the sort of current backlog gets worked through, it's probably a better way to phrase it.   
(01:53:51.301) ~~Right~~ (01:53:51.440)  
around the same time, I sort of expect that all of a sudden the tension will turn to Oh my God, now we have these foundation models that   
(01:53:59.242) ~~kind of~~(01:53:59.483)  
model the whole causal graph in all of its crazy complexity. And now we're actually going one level out and saying, now we can apply similar computational techniques to the identification of the targets. And we'll do that in   
(01:54:16.537) ~~sort of~~(01:54:16.738)  
a similar way of being like, okay, I want   
(01:54:19.739) ~~this, this is~~(01:54:20.501)  
what's happening and I want to prevent it from happening. or this is what I want to happen proactively that isn't currently happening. 


---


#### 01:54:27.564

Let me just kind of brute force my way through a bunch of perturbations to the, and of course we can get better than brute force too, but even just imagining a   
(01:54:36.810) ~~sort of~~(01:54:37.069)  
several couple generations down of Evo, it seems like make a tweak, see what happens is going to be so radically accessible from a computational perspective that We'll then also just have this explosion of like quality targets to identify.   
(01:54:51.605) ~~And yeah, I mean, what do you think the world looks like as all that happens? What is, it seems like we may be not super far from a,~~(01:55:01.372)  
this is not, we're not even in a world here of like an, any sort of AGI, right? 


---


#### 01:55:05.255

We're talking like, these are still tool simulated simulation and tool type things that people would be using that we're not assuming anything here about AI agents doing the work. Although you did have a little bit of that with the 310 co-pilot. But is there anything that I should be like reining in my expectations on?   
(01:55:24.873) ~~I mean,~~(01:55:25.073)  
are there things about like one tweet that I sent you was around to what degree can these things handle   
(01:55:29.997) ~~sort of~~(01:55:30.377)  
point mutations or whatever? And there's maybe individual idiosyncrasy becomes a really hard problem at some point, but like how far does this paradigm that I'm sketching out extend, do you think? And what limits does it hit? Yeah. 


---


#### 01:55:44.485

So I think, so just briefly on like point mutations or like more complicated mutations where you mutate multiple things and just predicting how positive or deleterious that mutation or set of mutations might be on the protein or something. That's a capability that ESM has, and that's already two or three years old at this point. And Evo does it better. They got state-of-the-art performance with Evo on predicting which mutations were positive and which mutations were negative and which sets of mutations were positive or negative. And you can compute   
(01:56:24.170) ~~a few different things,~~(01:56:25.051)  
a few different kinds of scores that tell you about this. you can actually build out evolutionary trajectories to show over time how things are likely to evolve based on how positive or negative the impact of a mutation is on protein or something or DNA sequence or whatever. 


---


#### 01:56:43.122

And Evo, they got state-of-the-art performance on this. And that's actually, they also did this with alpha folds. I think they called it alpha missense or something like that, where they just,   
(01:56:55.307) ~~I think they, what did they do it for?~~(01:56:56.628)  
Did they do it for   
(01:56:57.759) ~~I think~~(01:56:57.939)  
they did it for all the human proteins, but maybe it was a bigger dataset. I can't remember. But they predicted all the single point mutations and all the effects   
(01:57:06.353) ~~that~~ (01:57:06.453)  
that those have. And that's actually not a hard thing to do. So mapping out how a mutation affects a protein or DNA or something, and the course of evolution that's likely to occur, that's actually pretty easy to do now. 


---


#### 01:57:21.440

And then as far as... I also want to draw attention to another project that I'm aware of. It's not a model per se, but they are using... I think they are using GPT-4 They may have trained their own in-house model. I'm not sure. But there's a company called Future House, and they're designing an agent, an autonomous agent, that will do a lot of this research for you. And it'll do things like literature search and review, and come up with hypotheses of different kinds of interaction networks that you might want to modulate or different targets that you might want. And it'll do this and it'll do it pretty well. And that's a pretty new thing that just started happening like last year, 


---


#### 01:58:10.841

I think, maybe late last year. And they're getting pretty good results with that. And that's actually using an LLM   
(01:58:18.323) ~~like~~ (01:58:18.503)  
as the base,   
(01:58:19.604) ~~right,~~ (01:58:19.823)  
to build an agent to do this research. And then   
(01:58:23.788) ~~I think~~(01:58:24.109)  
they're also building an autonomous lab that drives itself. So once the agent comes up with hypotheses or targets or what have you, the lab is autonomous as well. And that's a pretty exciting direction.   
(01:58:38.895) ~~I think~~(01:58:40.037)  
that, coupled with some of these more specific tools to perform these fine-grained operations on proteins and small molecules and DNA and RNA. When those two kind of converge, that's going to be a really big deal. And I see that happening in the next year. 


---


#### 01:58:58.109

The progress that they're making at future houses is really impressive, I think. So that would also be something that people should definitely look into. And I think your timeline is within a couple of years for sure. I don't think it's going to be that long before we start seeing substantial progress and changes.   
(01:59:17.309) ~~I mean,~~(01:59:17.569)  
OpenAI just partnered with Moderna, right? Yeah. Hundreds of GPTs, just the beginning. And   
(01:59:24.154) ~~I think~~(01:59:24.434)  
that also is   
(01:59:25.375) ~~like~~ (01:59:25.494)  
a paradigm that's going to match well with these other more specific tools, because when you enable an agent to use tools, you unlock a lot of possibilities, right? When you enable something that can review thousands of research articles, then develop targets or hypotheses to test, and then can call on these specific tools to design molecules or proteins or nucleic acids to perform these specific functions or hit these specific targets. 


---


#### 02:00:01.243

That's going to move really fast. And   
(02:00:03.564) ~~I think~~(02:00:03.863)  
I'm excited. I'm also a little nervous because I think there's a lot of a lot of potential for misuse and the wrong hands, like the sort of things that you can accomplish will be amazing and beautiful. And we're going to see a lot of health problems just disappearing. We're going to see lifespan extended, and that's going to   
(02:00:26.122) ~~really increase or~~(02:00:27.342)  
really improve the quality of life for everyone. But also we do have bad actors in the world. And that is something I worry about for sure, because in the wrong hands, we could be looking at very dangerous things as well. And so having some kind of oversight for these things is very important. 


---


#### 02:00:44.479

Because, I mean, we're looking at moving into an age where you could target a specific group of people based on their genetics or something. That's both immensely useful and also very dangerous. I have a lot of faith in the people that are working on these things. Like the people that are building these models and doing this research are really good people with a lot of really good intentions and a lot of know-how and experience. And that to me is very reassuring, but there's always some random jerk that has the potential to mess it up for everyone. We have to be prepared for that. Yeah, no doubt.   
(02:01:25.898) ~~I mean,~~(02:01:26.158)  
preparing for this, definitely one of the major updates that I've made is that when people talk about the bio risks from AI, the conversation that I've heard most of has been like, how does it compare to Google? 


---


#### 02:01:42.636

How does GPT-4 compare to Google? Does it make it easier for you to get certain information or figure out how to do certain things. And in familiarizing myself to the degree that I have with all this technology, it's   
(02:01:55.358) ~~like,~~ (02:01:55.537)  
that all of a sudden feels very quaint already. It's like, this is not a question of comparing to Google. This is like generating entirely new stuff. And I looked back not long ago at the list of mass extinctions in the history of the planet and what caused them. Of course, some were caused by totally exogenous shocks like asteroid hits the earth. But the first one on the list on Wikipedia is the oxygenation of the atmosphere. 


---


#### 02:02:28.326

And it's simply that something kind of pops up and either itself, nobody knows how to eat, or it creates some waste product that,   
(02:02:39.573) ~~you know,~~(02:02:39.814)  
that nobody's prepared to deal with. And what we now breathe and depend on was at one point, the cause of a mass extinction event. I kind of try to keep these   
(02:02:50.979) ~~like,~~ (02:02:51.180)  
zoomed out perspectives in mind. And it does seem   
(02:02:53.881) ~~I mean,~~(02:02:54.201)  
tell me if you think there's any limitation to this or whatever. But with this sort of brute force search through biological space, it seems like there's not really anything conceptual that I could identify preventing – talk about gain-of-function type research on a totally different level. Things that nothing can eat. 


---


#### 02:03:19.006

That's like the most dangerous stuff, right? It's the stuff that nobody can break down. And I gather that trees were essentially at one point that too, right? Before something developed that could break down the hard fibers. tissue of a tree, it was just piling up. Globally, I understand that's basically where a lot of coal came from, is that trees would fall, nothing could digest them, and so they would just   
(02:03:42.679) ~~sort of~~(02:03:42.939)  
collect and eventually they turn into coal. I'm sure there's a lot of different stories of coal formation, but these moments of something that nothing is really prepared to deal with, those seem like the really dangerous things. And I don't know how you prepare yourself for that. 


---


#### 02:03:56.966

I think there are multiple things that we can do to help   
(02:04:00.349) ~~prevent~~ (02:04:00.769)  
prevent some of these bad things from happening. And   
(02:04:04.375) ~~I think~~(02:04:04.654)  
we're going to need to rely on the models that we build, especially the agentic models that we build, to help guide us in some of this. Because at some point in the near future, we're going to have agents based on really robust language models or something similar, and they're going to be able to review thousands of research papers and do tests in a lab on things, take in an amount of data that we can't really take in, right? That no human or even group of humans can really take in and process and digest and use. 


---


#### 02:04:43.474

Like the scale is going to be much larger than a human can really work with. And so we're going to have to rely on some of our models to help guide us. And also,   
(02:04:56.637) ~~Like,~~ (02:04:56.778)  
going back to how does it compare to Google, I think another argument that could be made for why not to worry about some of these things is, okay, maybe I can get on my computer and design some new thing that was really toxic or something, but I still have to go into a lab and synthesize all that stuff. And a lot of that part of the process is very highly regulated and watched, right? I can't just go get a bunch of random chemicals and build this stuff in my house, right? 


---


#### 02:05:29.716

Like it's harder to do than that. And like synthesizing proteins is, it's a non-trivial process. So   
(02:05:36.800) ~~like~~ (02:05:36.960)  
a lot of the worry, I think of, Oh God, we're going to have an AI that designs a deadly virus or a bioweapon or something. A lot of that is really overblown, especially at the moment. And   
(02:05:48.605) ~~I think~~(02:05:48.845)  
a lot of people overlook the fact that computationally designing something computationally designing a molecule is just one step in the process. You also have to do all the lab work and synthesis and work on some kind of delivery mechanism. And this is all stuff that's non-trivial to do, and that helps prevent bad actors from actually going through with some of this stuff. 


---


#### 02:06:15.189

Now, there may be like state-sponsored bad actors with access to good labs and lab equipment will circumvent a lot of that. But when you're working at a state-sponsored level, that's a matter of international relations and also national security. I think that has almost nothing to do with AI. The computational design of some random toxic molecule is just one step in a complicated process, and people don't often think of that. I see a lot of very influential, big-name people in the industry who are coming from the NLP side of things and the LLM side of things, and they don't really understand the biology and the process that goes into actually making these things. I think their worry is justified, but they're also not understanding the nuances and where the dangers actually are. 


---


#### 02:07:18.426

So I think it's important for people to keep that in mind. I think it's very important before we start getting all anxious and worried about some random person using Lama 3 to design a superflu or something, you have to remember it's very unlikely and very difficult for just a random average person to go through the entire process of designing and synthesizing and delivering some kind of toxic molecule. That's a long, difficult process that an individual would be very unlikely to be able to accomplish, even with the help of a very intelligent LLM or a very capable agent. Now, when you have larger research-oriented companies working on these things that have their own wet labs, and they're building agents to run these wet labs and to computationally design the molecules and form plans on how to use them. 


---


#### 02:08:17.970

There, I can see, okay, we need some kind of oversight. We need some people working on how to make sure that process is safe, how to protect that information and data and equipment, right? Because there are plenty of situations where something like corporate espionage is happening and people are trying to do nefarious things with some of the technology that some of these companies have. But again, that has very little to do with the AI itself and has more to do with how we're interacting with other countries and other research organizations. So definitely we need to be developing plans for how to use and regulate and oversee like a really capable agent that is going to go through the entire process of   
(02:09:09.007) ~~like~~ (02:09:09.167)  
computationally designing and verifying, and then also synthesizing and delivering. 


---


#### 02:09:14.061

And that is technology that is in existence now. We already have agents that are doing most of this process. And a lot of people are pushing for more of that, which I agree with, because we're not going to be able to solve these problems on our own. We're going to need some kind of really capable agent that can help guide us through these processes, because they're so complicated. and so difficult to understand the whole picture and all of its nuances that I don't know if humans can get there without some kind of agent helping out and helping design the molecules and producing it and delivering it and etc. I don't know if we can get there without that, but   
(02:09:57.859) ~~I guess~~(02:09:59.179)  
my concern is just making sure that these companies and organizations that are building this technology and using it have some people that are overseeing the safety side of things and that are concerned with red teaming and preventing things like corporate espionage and making sure that everyone that's using that technology is using it responsibly and making sure that we're   
(02:10:20.895) ~~like,~~ (02:10:21.155)  
that the companies are hiring, not just capable people, but also like people with good moral grounding and good intentions. 


---


#### 02:10:30.902

Yeah. I guess that's where,   
(02:10:32.422) ~~I mean,~~(02:10:33.123)  
that's not even the future. That's kind of now. That's already a concern that we need to address now, because we already have agents that are doing these things. And most people don't have access to them, though. Most people don't have access to a really capable agent that can do this whole process or do most of this process. That's not something that even most companies have access to, much less individuals, because a lot of these models are closed. I could see maybe some kind of like state-sponsored group of researchers could use open source models to build something similar and do something nefarious, but that's a whole,   
(02:11:10.679) ~~like,~~ (02:11:10.878)  
it's a very complicated process of building such a thing. 


---


#### 02:11:14.560

So I, and I don't know if I have a good answer for how to combat something like that or how to address something like that. I don't know if there's a good answer. to that right now. It's certainly hard to identify a more important question.   
(02:11:26.425) ~~Do you think that the,~~(02:11:27.206)  
do we have any read on whether offense or defense is favored here, so to speak? In the sense of for nuclear weapons, for example, if one of the major nuclear powers fires all its missiles, nobody can shoot all those missiles down. It seems to me that is an offense favored regime. And so we're   
(02:11:45.738) ~~kind of~~(02:11:45.979)  
stuck in this like mutually assured destruction paradigm, which is yikes. 


---


#### 02:11:51.981

We kind of need to get to a different paradigm because we're under like real threat of nuclear catastrophe as long as we've all got thousands of missiles pointed at each other and no viable defense. I don't have an intuition if biology like works the same way or not. I think this is   
(02:12:11.128) ~~like~~ (02:12:11.328)  
less of a question about biology and more of a question about cybersecurity because I think it's   
(02:12:18.109) ~~like~~ (02:12:18.288)  
very similar in spirit to   
(02:12:22.171) ~~like~~ (02:12:22.351)  
cyber security. And there as well, most often the attacker has the advantage over the defender. But there are a couple of things that may change that one is really capable agents. Because if you have a really capable agent that's able to defend against human attacks that are   
(02:12:38.842) ~~like~~ (02:12:39.002)  
just inferior, that's going to be a really big part of protecting against bad actors. 


---


#### 02:12:45.207

And so I guess like That's an argument for acceleration, actually, because if you have the most capable agent, then probably your defense is going to be a lot better than everyone else's. And if your agent is capable enough, it may be effective enough to ward off pretty much anything. And I don't know how soon that's going to come into the picture, but I think that is a good argument for keeping up the pace of development of LLMs and agents and things like that. There was another point that I wanted to touch on, and I think I forgot. I already forgot what it was, though. Anyway, yeah, I think the advantage of the attacker over the defender may end up shifting because of agents. 


---


#### 02:13:26.951

We may end up having a situation where that's no longer the case. And,   
(02:13:30.753) ~~yeah.~~ (02:13:31.054)  
I'm a little confused about   
(02:13:32.234) ~~why are you making a...~~(02:13:33.957)  
Why is the shift from biology to cybersecurity? Because I'm envisioning a world where For example, Evo is open source, Llama 3 is open source. If Evo 3 is open source, then we start to, at some point we enter into a regime where, yeah, it may not be easy. It may be,   
(02:13:53.322) ~~you know,~~(02:13:53.742)  
hard for one person, but at some point it does get like lower than state actor level where somebody could launch some crazy attack and then it's okay. If you create some superbug with certain properties, Can we defend against it? 


---


#### 02:14:10.554

I'm a little bit unclear as to how you're, I'm not sure if you're like equating that to cybersecurity or saying that's a primary somehow.   
(02:14:17.356) ~~No, I guess, no,~~(02:14:18.238)  
I think that's a good point. Yeah. Because if you develop some kind of,   
(02:14:21.939) ~~I think,~~(02:14:22.238)  
I guess a virus is probably as good an example as any, but let's say you develop a virus of some kind that targets a specific population. Developing a cure for that traditionally has been a very slow process. And like the fastest that we've ever done it was probably COVID. And that still took some time, right? And on the other hand, there is recent work that came out of, it was the University of California, but I'm not sure which one. 


---


#### 02:14:50.287

They recently published some research about like universal vaccines. And they're able to design a vaccine that was like applicable to a wide range of mutants of a virus. And they said that the technology or the method was highly transferable to other vaccines. And so there's no reason that this can't be applied to   
(02:15:08.905) ~~much~~ (02:15:09.046)  
any vaccine to develop universal vaccines against all variants of a virus, or most variants anyway. So that'll be helpful. That'll be good for   
(02:15:20.493) ~~defense sort of things.~~(02:15:22.515)  
And then as far as,   
(02:15:23.817) ~~I don't know,~~(02:15:24.176)  
I also wonder about the applications of certain AI models to developing defenses, but I'm not sure.   
(02:15:32.122) ~~I mean,~~(02:15:32.962)  
it's a   
(02:15:33.342) ~~very complicated or~~(02:15:34.984)  
very complex topic that   
(02:15:36.565) ~~I don't~~(02:15:36.805)  
some of the new things that are coming out feel like they might be the answer, but it's a little too early to tell. 


---


#### 02:15:44.451

That's definitely a, that's a very good data point.   
(02:15:47.731) ~~I mean,~~(02:15:47.931)  
my kind of default would be just to think I have three kids and I'm no expert in how babies develop in the womb, but it's definitely clear that a lot of things have to go right. Like an unbelievable number of things have to go right in the proper sequence. At any point, if something goes wrong, like that could be the end of it. Yeah. My general default model would be like, a lot of things have to go right and only   
(02:16:14.345) ~~kind of~~(02:16:14.565)  
one or two big things would have to go wrong. And so it seems like there's a lot of surface area to defend. 


---


#### 02:16:21.155

And a lot of kind of places that could be attacked. But then, hey, if you can make a universal vaccine, then all of a sudden that does start to look quite a bit different.   
(02:16:32.259) ~~So yeah, boy. Yeah. I mean, it's~~(02:16:34.341)  
and I think you're right also to say a big part of this does seem to be   
(02:16:37.461) ~~sort of~~(02:16:37.743)  
what is the prevailing   
(02:16:39.963) ~~like~~ (02:16:40.144)  
international relations regime? Because if it seems like pretty safe to say if we get into a bioweapons arms race, we're going to be in bad shape. we really have to have some more globally cooperative approach. Or the missiles have one really nice property, which is they don't spontaneously escape their silos and self-replicate around the world. 


---


#### 02:17:06.682

Whereas the list of lab leaks is quite long. It just seems like there's no way that we can get into an international bioweapons arms race and survive it. We just have to avoid that trap in the first place. And   
(02:17:23.557) ~~yeah,~~ (02:17:23.717)  
also, what happens when you develop cures for a wide range of diseases, and you're able to extend human lifespan significantly longer than what it is now and eliminate a lot of the diseases that we face once that exists.   
(02:17:41.453) ~~I don't know, maybe that's a paradigm shift.~~(02:17:43.536)  
  
(02:17:43.615) ~~Maybe that's a,~~(02:17:44.216)  
that's like a shift in human consciousness at that point. And we start thinking about things very differently because we're all used to thinking about   
(02:17:52.504) ~~like~~ (02:17:52.724)  
everything in terms of being finite. 


---


#### 02:17:56.246

And I think   
(02:17:57.808) ~~having,~~ (02:17:58.188)  
having an approach or thinking about things in a way that isn't finite anymore and thinking about things in terms of how valuable our health and our life is because of the fact that enables us to be with who we love for longer. The time that we have with the people we care about is, in my opinion, the most valuable thing that we have. And once you enable people to have healthy lives with people they care about, more or less indefinitely, that changes a lot. And I'm very excited to see, I hope that happens in my lifetime. I think it will. I think it'll probably happen within the next decade even. But I hope that really changes human consciousness to a point to where a lot of these problems just   
(02:18:45.146) ~~kind of~~(02:18:45.425)  
start to go away because we stop thinking of everything in terms of finite resources, finite lifespans, finite time with the people that we care about. 


---


#### 02:18:55.031

Hopefully it's enough of a conscious shift in consciousness that we see some of these problems fading because a lot of them are cultural, right? A lot of these problems or a lot of these threats at the heart are very cultural. It's not about the technology. It's about how we use the technology and how we're interacting with each other when we use it. And that requires people to think differently. It's not a problem that can just always be addressed with some new technology or some new defense mechanism, we really have to change our thinking. And I hope that when these things start becoming widely available, people's thinking will shift dramatically. Maybe that's where things are headed. 


---


#### 02:19:41.382

I actually have a lot of hope that's where things are headed and a lot of optimism, because I think overall, most people are good. And I think we can heal a lot of things, not just health problems, but a lot of psychological things we can heal with these tools because it's going to change the way that we interact with each other and the way that we perceive our environment and our relationship to it. That is beautiful sentiment and maybe a good place to end.   
(02:20:08.970) ~~I don't know if there's anything else that you wanted to touch on, but~~(02:20:12.815)  
hard to hit a more aspirational note than that.   
(02:20:15.256) ~~I know. Yeah, I think~~(02:20:16.397)  
I agree with you. 


---


#### 02:20:17.658

I mean, as far as other things to discuss, I don't know. I think we've probably discussed pretty much everything I had. And we talked about most of the models that I found interesting. So yeah,   
(02:20:29.016) ~~I mean,~~(02:20:29.236)  
yeah, I think that's a good place to stop too. I think we can probably call it there. And this has been really great, by the way. I had a lot of fun doing this and I really appreciated   
(02:20:39.247) ~~this.~~ (02:20:39.448)  
  
(02:20:40.029) ~~This is great.~~(02:20:40.408)  
I appreciate you being willing to spend so much of your Saturday teaching somebody who doesn't know nearly as much as I suddenly feel like I really should about this area. So feelings definitely mutual. I guess my closing thank you is Amelie Shriver. 


---


#### 02:20:56.058

Thank you for being part of the Cognitive Revolution. Of course. Thank you for inviting me. 


---



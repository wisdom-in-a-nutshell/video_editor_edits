# CR Koyena (Draft)

[00:00:00] **Nathan:** Koena Paul and David Bao from Northeastern University, authors of Future Lens. Welcome to the Cognitive Revolution. Thank you. 

[00:00:07] **David Bau:** Really happy to be here, Nathan. I'm 

[00:00:09] **Nathan:** excited for this conversation. So Professor Bao leads the group and Koen is part of the research group. ~~Uh, ~~and together with your colleagues, you guys have really developed a remarkable interpretability and sort of editability agenda with respect to large language models over the last couple of years.

[00:00:26] I have covered a couple of your papers previously, although not in the depth that we will get to very shortly with the future lens paper. But ~~I think~~ it's a really cool agenda that is shedding a lot of light on how ~~the, you know, ~~these new fangled AI's are actually working, what's going on in there, kind of cracking open the black box problem.

[00:00:43] And certainly regular listeners will know that that's something that I really,~~ So,~~ for starters, you guys want to just ~~kind of ~~give us a little background on the overall agenda ~~of the, ~~of the group and maybe highlight a couple of your favorite papers that you've published 

[00:00:56] **Student-2:** previously. ~~It's a, ~~it's a pretty 

[00:00:57] **David Bau:** simple agenda.

[00:00:57] So the thing that motivates our group [00:01:00] is the fact that machine learning is really a new tool. Era for computer scientists. ~~Uh, you know, ~~machine learning has been around for a while, but up until the last decade or so, it's been this dream of, ~~you know, ~~having a way of creating self programming computers that learn from data, that people don't really have to program every line of code, machine learning worked okay, but it didn't really work in profound ways until the last 10 years or so, but now it's really working.

[00:01:24] It's really working remarkably well. And so we're facing a new type of software that we cannot use traditional computer science tools and traditional computer science methods for dealing with how to ensure that it's correct, that it does the stuff that we want. ~~ Uh, you know,~~ all of our tools are very statistical.

[00:01:43] ~~They're very, you know, they're, they're, ~~they're very black box. ~~And, ~~and so what the theme of the lab is. is to ask, ~~you know, ~~how do we confront this new type of software ~~is,~~ are there things that we can do to recover our ability to debug and understand the software that we create? Are there ways that we can take more [00:02:00] responsibility for the behavior that emerges from this software?

[00:02:03] Can we edit the code, like the way that you would change a line of code? In a traditional program. And so ~~this is, this is actually, ~~this is actually pretty hard. It would be like asking the question, can you totally control the mechanisms of a tomato or some biological thing that emerged out of, ~~you know, uh, ~~a process of evolution.

[00:02:23] And ~~so, you know, ~~machine learning is similar that way it emerges out of a training process. And so just like biologists have to reverse engineer how a tomato works if they want to. really understand ~~what, you know, ~~what they can do to make it better. We're also trying to develop a science of how to understand the internals of these systems.

[00:02:40] Now, 

[00:02:41] **Nathan:** is that an agenda that you have ~~kind of ~~changed course on relatively recently? I assume it ~~kind of ~~has to be in as much as, ~~you know, ~~the understanding of advanced AI systems in this way is ~~sort of ~~predicated on their existence. And I would imagine like, at least probably prior to, ~~you know, ~~GPT two, there was almost nothing.

[00:02:58] ~~You know, ~~powerful enough [00:03:00] to do this kind of work. Oh, no, 

[00:03:01] **David Bau:** ~~I, ~~I've been at it for a while. ~~So, ~~so ~~I actually, you know, my,~~ my personal history is ~~I, I, ~~I worked at Google for many years and I actually left Google to pursue research when it started to become clear around 2015 that the field ~~was, was, ~~was going to change.

[00:03:13] And the speed at which it's changed, ~~I think~~ has surprised. Me, ~~I think~~ it's surprised almost everybody in the field,~~ but,~~ but it was clear that there was a sea change happening.~~ I think that~~ the moment for me was also the same moment for a lot of people when Alex net came out in 2012 and showed that there's this ~~really, ~~really simple, really classical.

[00:03:32] Machine learning procedures, something from an idea from the 1950s, right? And an idea from the 1980s, ~~you know, ~~training these neural networks,~~ which,~~ which ~~people~~ really, the community at large thought that such a simple procedure probably wouldn't be the thing that solves machine learning in the long run.

[00:03:48] ~~I think~~ people thought it would be something trickier or something more complex or something like that. But this idea that all you have to do is scale up neural networks, and it works really well, ~~I think~~ was, A real eye opener. So [00:04:00] the ~~kind of~~ things that I studied, ~~you know, ~~at first I studied a generative vision models a lot like GANs,~~ uh, which are,~~ which were really surprising when they came out and I thought I'll study these GANs for a long time.

[00:04:10] Of course, ~~you know, ~~after GANs, we have diffusion models and of course we've got these amazing language models. ~~And, ~~and other things going on. So ~~I think that it's, ~~it's been this incredible moving target. It 

[00:04:19] **Nathan:** does seem to be a pattern that the earliest to the game started with more vision models. I know that's true for ~~like ~~Chris Olaf, for example, as well.

[00:04:26] So yeah, fascinating. The kind of~~ lineage~~ shared lineage there. Do you want to touch briefly on the Rome and Mehmet papers? This is one that I've covered a little bit in a previous episode. And the way I remember those papers is as a demonstration of the locality of factual knowledge in a language model, and also the ability to then edit that language model in ways that preserve a lot of the key properties that you would want to preserve if you were editing a knowledge graph, where, for example, if you were to think that the example in the [00:05:00] is Michael Jordan played basketball, of course, is the real sentence, but if we wanted to edit that world knowledge to reflect an alternative reality where Michael Jordan played baseball, then we would want that to be not just, ~~you know, ~~for that specific sentence, but ~~kind of ~~robust to different ways you might ask the question, different ways you might set up ~~a,~~ an auto completion.

[00:05:18] And, In the process of kind of systematically working through the layers to figure out where ~~you, you, I think if, if I recall correctly,~~ you're ~~kind of ~~corrupting bits as you go through the layer and figuring out where it starts to fail and then using that as ~~the, ~~the place to edit and then achieving, ~~you know, ~~that kind of robust.

[00:05:35] Editing. ~~So tell me how~~ it's been a couple months since I went deep on that one. Tell me how I did ~~and and tell me, um, no,~~ no, no, 

[00:05:38] **David Bau:** no, that's right. ~~You know, ~~and ~~I would, ~~I would back up a little bit, maybe half a step further, which is ~~like, you know, ~~the fundamental question that we're asking, and it's actually ~~kind of ~~related to future lens too.

[00:05:46] Is,~~ is, ~~is there a~~ a reality is just ~~like a physical reality to the idea of ~~like ~~a concept or an idea or a unit of knowledge, right? We have these things in our head. We think, ~~you know, you can,~~ you can go to somebody and you can say, that's something that, you [00:06:00] know, like, ~~you, you,~~ you know, where the Eiffel tower is, or, oh, you've never heard of the Eiffel tower.

[00:06:04] You have no idea where that is. No, it's something that you don't know. ~~Like,~~ so ~~we have,~~ we have this idea that. People can know things or they can not know things or they can have an idea or a concept or they can not have one. ~~And so~~ it just seems so crisp intuitively in our own heads. So the question ~~is, ~~is there a physical reality to this?

[00:06:20] When, ~~if, uh, if, uh, if, ~~if an artificial neural network seems to know something or doesn't know something, is there a physical reality to that knowledge? Or ~~is it just, ~~is it just, diffuse and spread out in all the neurons and all the computations through the whole network. ~~And, ~~and I think that ~~there's, ~~there's definitely a school of people who would generally believe that most things are just unimaginably diffuse, that everything's just spread out.

[00:06:43] There's no reason that there would be any locality, but there's a bunch of neuroscientists in the biological world. And some computer scientists in the artificial neural network world who have taken a look ~~and, you know, ~~over the years and notice that a lot of times you see locality. ~~So, you know, So, you know,~~ I saw that kind of thing in GANs, but, ~~you know, our, ~~[00:07:00] our question was.

[00:07:01] Do you see this kind of organization in ~~really, ~~really large models? And do you see any ~~that, ~~that corresponds to the facts? And so what Rome was about is a bunch of experimental methods ~~for, ~~for narrowing this down ~~and, and, ~~and finding out. Where facts are localized ~~in, in, uh,~~ in a large language model, it sounds like you had another PI test on it.

[00:07:19] So, ~~you know,~~ maybe you can direct people ~~to, to, ~~to listen to that one. But yeah,~~ that's,~~ that's the general setting. And of course, there's a bunch of clever methods that you can. Used ~~to, ~~to really pin that down. 

[00:07:27] **Nathan:** What is the state of that work now? I know that ~~the, ~~the successor to Rome was the Mehmet paper, right?

[00:07:33] And that one showed that you could edit up to like 10, 000 facts at a time. ~~Sure. ~~

[00:07:38] **David Bau:** Sure. And then there's another paper ~~that we, ~~that we've written. It's actually also coming out this coming year at ICLR. It's called the LRE paper. ~~Linear relations or~~ the linear relational embedding paper. ~~And, ~~and that paper looks at a different slice of the problem.

[00:07:52] That paper really asks, if you have a relationship like something is located in a city, or somebody [00:08:00] plays a certain instrument, or somebody plays a sport, or somebody holds a certain position or something like that, there's this general, a relationship,~~ what's,~~ what's the representation of that general relationship?

[00:08:10] ~~So, ~~the Rome paper was asking, what's the representation? Of like an individual association, but we really wanted to ~~know how we want to really~~ break that down. ~~So we, we,~~ we can see that there's an individual association. We can see that the representation of the subject and the object seemed pretty clear, but we wanted to understand what's the representation of the relation between the subject and the object.

[00:08:32] And the LRA paper explores that. and finds it in a bunch of the cases, the relation can actually be understood as a linear mapping. ~~But, ~~but it's actually, ~~there's, it's~~ sort of an incomplete story because we found that for a lot of the cases, ~~the, it's a linear mapping, but for a lot of the cases, ~~There's something more complex going on.

[00:08:47] There's something that looks non linear. And so it ~~sort of ~~opens the door to future research on new tech. To ~~sort of~~ ask, what's going on in the more complicated cases? These relations are sometimes really non trivial. And I think that there's going to be some [00:09:00] interesting, exciting work to do to figure out like, why is it that the models are modeling some relations in a really complex way?

[00:09:07] ~~You know, ~~what are they getting out of all that complexity? And is it enabling new types of reasoning that we haven't characterized yet? 

[00:09:14] **Nathan:** Cool. That's awesome. ~~Well, ~~I look forward to that one in more detail in the future as well. Koen, let's get into the Future Lens paper where you're the lead author. This one really out to me pretty much immediately because I think you were ~~kind of ~~speaking to it a moment ago as well, where you're saying, ~~you know, ~~there's a school of thought out there that's like, this is all stochastic poetry and ~~you know, ~~there's no real understanding and ~~you know, ~~it's just next token prediction.

[00:09:41] ~~And ~~so I'm always interested in things that explore like when, ~~you know, ~~near next token prediction can in fact be a bit more than meets the eye. And this paper is a really good example of that. So you want to start off maybe by just talking about ~~kind of~~ the specific motivation for this particular investigation within the broader agenda of the group.

[00:09:59] **Koyena Paul:** [00:10:00] Yeah. So actually the way this problem started was ~~very different from~~ like a little different from how it was before. ~~Like~~ initially I was interested in ~~like ~~looking at like memorized content and ~~like~~ large language models. Cause ~~you know,~~ when you use chat GPT or ~~like, you know, ~~any other models, ~~like~~ some things that I've noticed, like license codes, for example, ~~they,~~ if you just give a couple tokens in, you kind of know the next, 11, 20 tokens that ~~like~~ tend to be exactly the same from ~~like~~ it's training data.

[00:10:25] So initially I was actually first exploring that and ~~I think~~ while I was exploring that, I ~~kind of ~~like tangentially went to this point where like, okay, well I can see that it's ~~You know, thinking about these, like, you know, ~~saying these tokens pretty much like word to word, but like, how about ~~like~~ for smaller phrases, like New York city and stuff like that, which for us, we consider that as ~~like~~ one whole entity.

[00:10:46] ~~And so, ~~yeah, that's how it ~~kind of like ~~started off in terms of just looking into ~~like ~~seeing whether one, ~~like~~ a single hidden state ~~can actually like, like,~~ can we actually decode such information from that? And yeah, we were exploring ways. that you have seen in the paper in terms of ~~like, ~~to what [00:11:00] extent can we ~~like~~ decode that future information about a particular entity or like just anything in general 

[00:11:05] **Nathan:** at this point.

[00:11:05] So ~~the, ~~the question as it's I'm reading directly from the paper in this work, we ask to what extent can we extract information about future that is beyond the currently under consideration token. from a single hidden token representation. So let me, again, just pitch you how I understand this work and you can correct any misconceptions that I have.

[00:11:26] I think the vocabulary, especially for people that are not ~~like~~ in the research, can sometimes be a barrier to entry. So if I understand correctly, what you're doing here is looking at activations within the forward pass of a large language model. As the numbers are getting crunched, I sometimes like to use the most basic terms I can.

[00:11:47] The numbers are getting crunched from beginning to end. And between the layers, where the actual intensive computation occurs, there are these kind of middle states, which are known as activations. You are taking [00:12:00] an array of numbers, basically, that sits there. At different places, and we can get into more details of, ~~you know, ~~the different places that you can look, you can kind of look at every given layer right ~~through the, ~~through the transformer to see a different activation.

[00:12:11] But the question you're always asking is, given this array of numbers, ~~this,~~ these activations, can I. Predict not just what the current token is going to be, as I'm working through that forward pass, but can I also see what the future tokens are going to be just from the information that's in that one particular vector of numbers.

[00:12:30] Is that right? 

[00:12:31] **Koyena Paul:** ~~Yeah, ~~right. Yeah, ~~I think~~ like we just termed those~~ like~~ activations is ~~like~~ hidden states because those are like, ~~you know. ~~Hidden and they're part of the intermediate computation and stuff. ~~Yeah. ~~

[00:12:39] **David Bau:** ~~That's right. You know what I think would be a really great thing to explain Koyana is, you know, we, we were looking at a lot of logic lens sort of visualizations of these transformers that sort of motivated.~~

[00:12:39] ~~Some of the, you know, some of the, the questions you were asking, you can explain. ~~

[00:12:39] **Koyena Paul:** ,~~ I guess like~~ the predecessor,~~ I suppose. So~~ logit lens is essentially ~~like~~ a tool where ~~like, ~~it ~~kind of ~~projects ~~like these, like~~ these intermediate States into ~~like~~ the decoding layer. ~~So. ~~So essentially we can ~~kind of ~~just see for that current token prediction, ~~like ~~what is the model currently thinking about?

[00:12:54] Like ~~what word it like, yeah,~~ based on the distribution and ~~like, you know, ~~when you decode it to ~~like~~ the highest probable word, ~~like what is it,~~ what is the model currently thinking? ~~And so, yeah, in terms of like ultimately how the future lens looks. happen is like, okay, so these are only like one tokens.~~

[00:12:59] ~~Like, let's say if for about a particular person, they studied at like university of like any country, if you did logic lens, it would be like, it'll just show university. So like, for example, if you're interested in knowing like the, what the other words could have been. And so that's, I think those are like some motivating examples in terms of how.~~

[00:12:59] ~~Yeah. It ~~

[00:12:59] **David Bau:** ~~went, you know, so I, ~~I [00:13:00] recommend anybody who's, ~~you know, ~~listening to the podcast who hasn't seen logic lens before this is not our work. This is somebody else's work, ~~right?~~ So there's a blogger, a nostalgic brist who created this idea of logic lens. They should Google it and take a look at what logic lens ~~looks like.~~

[00:13:13] It looks like ~~it's, it's, ~~it's,~~ it's~~ these beautiful grids ~~of, ~~of words. that are overlaid on all the hidden states of the transformer, where ~~every, ~~every hidden state, every one of these vectors that's inside a transformer, all of these intermediate numbers are all translated into a word.~~ And, and you, so,~~ and then at the bottom layers, at the very earliest phase of the transformer, you can see what words the transformer is basically internally thinking.

[00:13:38] And then as you go through more and more layers, the words evolve until you get to the end. And ~~the words,~~ you can see the predictions of words get more sophisticated as you get to the end. ~~The guesses,~~ it's always guessing what the next word should be that it should say.~~ And, and, ~~and those guesses get better and better, the deeper you go into the transformer.

[00:13:57] It's really interesting to look at the logic lens, ~~right? Yeah. So, but the big disadvantage, right, ~~

[00:13:59] **Koyena Paul:** ~~The, yeah, the big, the,~~ yeah, the big [00:14:00] disadvantage is ~~like, ~~you only see ~~like ~~what it's currently thinking, which may not be ~~like ~~representative of ~~like ~~what it might be actually ~~like, you know, ~~thinking about a couple tokens ahead, ~~like~~ it's not as informative in that sense.

[00:14:10] And so we are trying to like, make it more informative and seeing like, okay, it's currently, ~~for example, let's say it's~~ thinking of the word new, ~~like what exactly, like~~ what, Word is a thinking after new like is a thing of New York, New Jersey,~~ like these, ~~these are like some examples of ~~like ~~things that could follow new, but that's kind of like not possible to see with logic lens for ~~like ~~that particular hidden state at least.

[00:14:28] **Nathan:** Yeah. So there's ~~kind of like ~~two directions, ~~I guess, ~~that we can consider. Tell me ~~if you,~~ if this intuition jives with your understanding in the course of the forward pass, basically, this is what the logic lens looks at is like, as we're going layer by layer, We're sort of gradually getting more sophisticated in the way that the model seems to be understanding the input and it's gradually converging to the prediction that it's actually going to make.

[00:14:53] So you can see at the beginning, it like has a low level of confidence and maybe, ~~you know, ~~wrong, ~~you know, ~~if you just took that hidden state [00:15:00] and went directly to decode, and that would be basically like, okay, let's say we do two layers of computation, then we skip all the rest and then we decode whatever came out of the two layers instead of, ~~you know, ~~all the layers.

[00:15:09] What would we get? ~~Well, ~~what we get is not very accurate at two layers. It gets more and more accurate as you go through the layers, as it finally, ~~you know, ~~reaches ~~its, ~~its output, which makes sense, right? Cause that's presumably why we need all the layers is to be ~~working the, you know, ~~working through the information and gradually getting somewhere.

[00:15:23] And then there's also ~~kind of ~~the token. direction, right? We've got like a sequence of tokens and information can only flow forward because that's the nature of the, ~~you know, ~~look back attention mechanism. So it can only flow forward from tokens to future tokens, but that means, or at least it stands to reason, right?

[00:15:41] And this is ~~kind of ~~what you will then set out to prove that ~~like, ~~as this information has ~~sort of ~~built up from prior tokens to the current token, it probably means that there's More there than just what would be needed to predict the immediate token. And there's been like lots of, ~~you know, kind of ~~interesting intuitions around this with,~~ uh,~~ even just [00:16:00] articles in English, right?

[00:16:01] Like if you set up a situation where it's very clear that the actual noun is going to begin with a vowel versus a consonant, then you can see that it predicts the article correctly. And then you're like, huh, that's pretty suggestive that maybe there's more information there. Otherwise, ~~you know, ~~how would it be choosing the article?

[00:16:17] It seems to be anticipating, ~~you know, ~~what's coming beyond ~~this, ~~this current token. As well. So I ~~kind of ~~think of the information processing proceeding like vertically and ~~the, ~~the token information flow ~~kind of ~~proceeding horizontally. And now we're in this moment where it's ~~like, ~~okay, at each layer, ~~through this, ~~through the forward pass, ~~you know, ~~through the vertical dimension, we can check to see like, ~~how good is, you know, ~~would this be enough already to predict the current token?

[00:16:39] ~~Um, ~~and again, that's the logic lens kind of. Based on what you're building. Now we get to, okay. Can we also detect that future token information is there, right? Okay, cool. So tell me how you did it. First of all, I noticed that this was done on GPT J ~~and. ~~That was kind of surprising, but maybe I'm just not sure what I don't know about [00:17:00] GPTJ.

[00:17:00] It seems like these days this is like llama would be the default for this sort of thing. So how did you choose the model? 

[00:17:06] **Koyena Paul:** ~~I think, I mean, it just,~~ again, since this was like ~~kind of like ~~a spinoff from the earlier project that I was talking about, so ~~like, ~~I was using GPTJ and I just ~~kind of like ~~continued with it, but ~~like, ~~it was definitely like one of those models where ~~like, ~~I could ~~like ~~run it on ~~like, you know, ~~like a single GPU.

[00:17:18] Do we have a feature lens on Lama now? ~~I think we, ~~I think people are building it. ~~If not, like, you know, like, you know, it essentially for, ~~if it has ~~like ~~the same ~~like~~ vector size, like 4096. Then,~~ like,~~ you can technically,~~ like,~~ do the whole transfer. ~~But the ~~

[00:17:28] **David Bau:** ~~whole thing pretty much works. It works across all these ~~

[00:17:28] ~~different ~~

[00:17:28] **Koyena Paul:** ~~models.~~

[00:17:28] ~~Yeah. So like, I think the way though, if you want it to be like in a completely different setup is, you know, have a soft prompt trained in that sense for like, well, you should explain how it works. Yes, that's true. Yes. But yeah,~~ but yes, generally this method should be. workable for ~~like~~ other models as well.

[00:17:33] **Nathan:** Yeah. Let's go back to the other models in a little bit. Cause I have some questions around like how you think the different models might behave differently under this sort of examination, but it'll help to establish exactly what it is we're doing. ~~So, ~~and you said ~~the, the inter,~~ the activation vectors, this was actually one of my questions, the vector from which you are predicting that's a 4, 096.

[00:17:54] Size vector 

[00:17:55] **Koyena Paul:** and like the number of tokens, but then that would be one for us. So yeah, 

[00:17:59] **Nathan:** okay, cool. So [00:18:00] then tell me about the data set. So this is the first, ~~you know, ~~as is so often the case, the first challenge in doing something like this is you've got to collect a data set. This one is kind of a subtle one to describe.

[00:18:10] **Koyena Paul:** Yeah. So since I knew that PTJ was trained on ~~like~~ pile, I was like, okay, why don't I take the pile dataset and~~ like~~ sample a couple of texts from it and ~~kind of ~~just, ~~you know, ~~get the hiddency from each of ~~like ~~the sentence in there and. Yeah, run it. So ~~like~~ I collected like a hundred thousand of them. ~~I think~~ one of my initial condition was ~~like,~~ if it is ~~like~~ GPTJ itself, ~~like ~~if it is reading this one token that it's predicting the next token correctly in that sense.

[00:18:38] And so that's one of the few ~~like~~ sample condition that I had, but otherwise, yeah, once I got like a hundred thousand of them, ~~I like, you know, I, ~~I stopped and then I was experimenting on 

[00:18:46] **David Bau:** that. ~~I see. So, ~~so it's a hundred thousand. Samples of texts with what? What's the filter that you used in 

[00:18:51] **Koyena Paul:** hand? Yeah, ~~the filter, ~~the filter that I used was that,~~ like,~~ given~~ like the last of the prompt, like~~ the last text of the prompt that the next one it predicts correctly.

[00:18:59] ~~The model, the model. Yeah,~~ the model [00:19:00] predicts correctly. Yeah. Okay. So there's 

[00:19:01] **Nathan:** 100, 000 prompts identified by the condition that the model must get the next token correct per the actual source material. ~~And then, as you, ~~so what are you actually collecting for each of the 100, 000?~~ It is a,~~ it is the activation, right?

[00:19:16] ~~Or the, ~~or the hidden state for each of the layers throughout the entire transformer? ~~I ~~

[00:19:21] **Koyena Paul:** ~~guess, ~~yeah, that's what eventually happens. But in terms of,~~ like,~~ just storing purposes,~~ like,~~ I had just a CSV file of,~~ like,~~ these 100, 000 sentences. But then later,~~ like,~~ during the training process,~~ like,~~ I would,~~ like,~~ gather the last hidden state of it at that particular layer for whatever.

[00:19:36] Like probing or ~~like, you know, ~~a method that I'm trying. 

[00:19:39] **Nathan:** Because all of the analysis downstream of this is going to be at a layer specific level, right? ~~Like, ~~

[00:19:45] **Koyena Paul:** yes, ultimately ~~like~~ the actual input itself would be ~~like, you know, ~~the, ~~like~~ four zero nine six, ~~like ~~vector. But yeah, when I'm ~~like~~ collecting all of them, ~~like~~ I'm collecting them based just on the strings and 

[00:19:54] **Nathan:** stuff.

[00:19:55] So, yeah, I always like to get very clear on the inputs and outputs. So now we've gotten to the point where, okay, we've got the a [00:20:00] hundred thousand texts. And our goal is to say, for a given layer, can we figure out a way to take that 4096 length vector and use that as the input and then predict Not just the current token, but the next several tokens from that single input vector.

[00:20:21] **Koyena Paul:** Yeah, almost there. ~~I think like, ~~so definitely layer, but also the last token. So ~~like, it's not,~~ if my prompt was, ~~you know, ~~10 tokens, if it was layer wise, it'll be ~~like~~ 10 by four zero nine six. But since again, it's just one token and a single hidden state, it'll be ~~like.~~ The last ~~like ~~token off the input prompt and that would be so that's one by 4096.

[00:20:38] **Nathan:** Yeah. Okay, cool. And then just as validation, there's another thousand that you'll do the testing on once you ~~kind of ~~develop the methods. Okay, cool. So we've got, ~~I guess, ~~five distinct methods where the first one is ~~kind of ~~the null hypothesis, which is just the bigram, which is ~~like, ~~okay, given the total frequency of word pairs in [00:21:00] the entire pile data set, to what degree can I just look at the current word and predict the next word solely from that?

[00:21:05] ~~Right. ~~And if you're guessing at home, what that number is, I'll give you a second. It is 20%, apparently 20% of tokens in the pile. You can guess just from one, the knowing the current word gets you basically to 20% accuracy. That was kinda surprising to me. I wouldn't have guessed it would be that high.

[00:21:22] There you have it. 20%. Yeah. 

[00:21:23] **David Bau:** ~~This, ~~this language modeling is not so hard after all. ~~Right. You know, ~~you just get 20% from counting and, ~~you know, that's, ~~that's it. ~~That this, uh,~~ this ngram thing was, ~~you know, ~~the state of the art method till not too many years ago. 

[00:21:32] **Nathan:** Yeah, but it's not state of the art method anymore.

[00:21:34] So let's talk about the four methods that you developed. And first one is direct vocabulary prediction. So here you take that same for 96 vector and just specifically try to jump directly to ~~the ~~the logits, right? The final percentage, ~~I guess~~ it's not exactly percentage, but it's within a very short transformation from [00:22:00] percentages of the actual tokens to be predicted for the current and then the next few.

[00:22:04] What is the nature of the thing that you're learning? This is because it's a learned method, right? ~~We're going to,~~ you're going to optimize and essentially learn ~~a ~~a way to make this prediction across the 100, 000 samples? What is the nature though of the vocabulary prediction thing that is being trained?

[00:22:21] **Koyena Paul:** Yeah, ~~I think~~ so like the goal with ~~the linear like ~~this direct vocabulary prediction is essentially ~~like ~~can we like literally decode the token from ~~like~~ that hidden state? I imagine the linear models would be ~~like~~ The most, ~~I guess, ~~basic ~~kind of like ~~model for probing in terms of ~~like, ~~just being able to grab ~~that, you know, ~~that token.

[00:22:38] And so, yeah, ~~I think~~ that was essentially the goal. ~~Like~~ we wanted to see whether there was ~~like~~ some sort of ~~like~~ linearity and like being able to just decode what a future token is like, is that stored ~~like ~~linearly in ~~like ~~the hidden state. So 

[00:22:48] **Nathan:** that is to be very. Concrete a one layer transformation.

[00:22:53] **Koyena Paul:** ~~Yeah. It's like one,~~ no, one layer, one token. ~~So it's like, ~~so in some sense it's like context free, but ~~like, ~~yeah, it's one hidden state to one other hidden state. And ~~like~~ [00:23:00] each of them is ~~like, just~~ like~~ like~~ one by four, zero, nine, six. 

[00:23:03] **Nathan:** The thing that is being trained, that is doing the transformation from the hidden state to the prediction is just a simple linear transformation.

[00:23:12] **Koyena Paul:** Right, ~~right.~~ And sorry, just to correct myself earlier, since we were talking about the vocabulary prediction, it's actually ~~like ~~1 by 4096 to 50400, ~~because that's like the vocabulary space for like the ~~

[00:23:20] **David Bau:** ~~Oh yeah, you're gonna have to explain this. Oh sorry, yes. ~~

[00:23:20] **Koyena Paul:** ~~Yes. So you're, so you're, you're still in the weeds?~~

[00:23:20] ~~I'm so in the weeds, yes. Okay. Yes. Yeah. ~~So essentially ~~in the, ~~the way this vocabulary prediction is that ~~like ~~the GPTJ,~~ like,~~ if we were to tokenize the words, ~~like the token, like the, ~~the size, the vocabulary space of A-G-P-T-J is about 50,000 tokens. And ~~so yeah. That's essentially we are, ~~we are essentially trying to get that vector of like 50,000 tokens.

[00:23:37] Choose whichever is the highest probability as ~~like~~ the token that would be predicted. So that's for the linear, ~~like~~ direct vocabulary prediction. And ~~so, ~~yeah, that's why for this particular method, we grab in the hidden state, which is again, four zero nine six vector. And then that's two five zero, like that 50, 000,~~ um,~~ size of~~ of like ~~one token.

[00:23:58] **David Bau:** ~~Yeah. Literally,~~ you're literally training a [00:24:00] decoder. Your own decoder head on this problem, right? Yeah, essentially. It's training a little linear classifier. 

[00:24:06] **Nathan:** So the number of parameters in that linear classifier would be 4096 times the 50, 000 vocab size. So ~~each,~~ essentially each number ~~in the, ~~in the hidden state makes a contribution to each output token.

[00:24:21] And the intensity of its contribution is determined by the parameters which are learned in the training of this. Linear. 

[00:24:28] **Koyena Paul:** That 

[00:24:28] **Nathan:** sounds right. Yeah. Okay. Cool. So that's direct vocabulary prediction. So we got 100, 000 of these 496 vectors. We know what the actual next tokens are, and we're training this mapping of 4096 by the vocab size to do that mapping.

[00:24:47] And then ~~there's, ~~there's kind of two variations of this, right? The first one is the direct vocabulary prediction. The second one is the linear model approximation. And if I understand correctly, the difference is whether you're jumping straight [00:25:00] to the output tokens ~~as, ~~as what you're predicting. Or, keeping the existing decoder, and instead trying to predict something that then the decoder would properly decode.

[00:25:10] **Koyena Paul:** Exactly, yeah. ~~So, yeah, like,~~ one is to the vocabulary,~~ like,~~ distribution, and then the other one is to,~~ like,~~ the hidden state, which the decoder layer would decode it to that ultimate token, yeah. 

[00:25:20] **Nathan:** And that's pretty interesting. ~~I was,~~ I didn't have ~~an into~~ too much of an intuition for like why one might be thought to work better than the other.

[00:25:24] And then it seems like it basically turned out that they roughly work equally well, like almost uncannily similarly. ~~Right. ~~

[00:25:31] **Koyena Paul:** Yeah, actually, for me, that was a little surprising because I would have assumed that because for the vocabulary distribution, like it's also trying to ~~like ~~learn how to~~ like~~ decode, like it's creating ~~like~~ its own decoder thing, I thought it will take probably ~~like~~ more number of iterations or ~~like, you know, ~~basically a lot more data for it to come to that stage, but it works similar to ~~like~~ how, ~~you know, ~~if you just predict the hidden state and have your decoder layer handle that.

[00:25:57] Yeah, it works similarly. So that was pretty cool to see. Yeah. 

[00:25:59] **Nathan:** Is [00:26:00] there something that we can ~~sort of ~~understand about the broader system based on the fact that those two approaches work the same? Like it seems You basically have two linear classifiers, and you can't, like, two is not better than one is kind of an interesting way to see that, right?

[00:26:16] ~~So does that mean, ~~I guess one way to interpret that would be that you really are ~~kind of ~~getting toward the max of the information that is there? ~~You know, ~~I guess another thing you might try would be like a bigger, ~~you know, ~~more ~~You could, you know, ~~you could train a full transformer to do this sort of thing.

[00:26:28] ~~Right. ~~And maybe you did, but I guess ~~if, ~~if two linear classifiers aren't better than one, then maybe you'd ~~sort of ~~think, ~~you know, ~~we're ~~kind of ~~already maxing out. Is that how you would interpret that? Yeah, 

[00:26:37] **Koyena Paul:** ~~I think~~ that's how it interpreted. Like we wanted to start with ~~like ~~a quote unquote, simpler solution,~~ like, you know, linear,~~ like having some sort of ~~like ~~linearity with ~~like ~~decoding, like future tokens, that would have been like a, ~~you know, ~~a nice final solution.

[00:26:47] But we realized that no, it's a lot more complex than that. At least at the moment. And ~~so, ~~yeah, that's what we ~~kind of ~~tried. We tried our best to ~~like ~~max out the linear linearity aspect of our 

[00:26:57] **Nathan:** experiments. Okay, cool. So that's ~~kind of ~~[00:27:00] one class of thing, training these linear classifiers. And then the other class of thing is basically an approach where you take the activation.

[00:27:09] Out of the context in which it was generated and poured it over to, and kind of stitch it into ~~a, ~~a broader forward pass context where that other forward pass context is ~~kind of ~~engineered to be ~~sort of ~~as neutral as possible, or, ~~you know, ~~I guess ultimately ~~like ~~engineered to allow that activation to ~~like ~~shine through and get its content through to the, ~~to the The ~~predicted tokens, ~~like as, you know, ~~as effectively as possible.

[00:27:34] So the first way I thought was like super intuitive to do that. You ~~kind of ~~just set up the. The prompt with, hello, could you please tell me more about, and then port in the activation from the other context where, ~~you know, ~~however much information has been aggregated at that final token is now being ported in and the theory there is like.

[00:27:51] Well, because hello, could you please tell me more about is so generic than like in theory, whatever you put there, ~~you know, should, ~~should set it up for a kind of nice, [00:28:00] clean continuation. Unfortunately, that one didn't seem to work so well. So I was surprised by that. ~~What's up,~~ what do you think is up with 

[00:28:06] **Koyena Paul:** that?

[00:28:06] ~~I think it's, ~~it's because ~~like, ~~perhaps it was too generic in that sense. While yes, we were targeting ~~like~~ generic prompts so that ~~like, ~~it has the possibility for ~~like, ~~Whatever the intervened hidden state is to like ultimately have that token shine through, but it was probably still too general. ~~Like~~ the prompt wasn't really optimized for it to be like, Hey, ~~you know, ~~I wanted the future tokens out from this particular state.

[00:28:30] And so that's why, ~~you know, ~~I'd feel like it didn't work as well. We tried a few, right? ~~Yes, we tried a couple. I mean, we tried a few,~~ but ~~they, you ~~

[00:28:35] **David Bau:** ~~know, ~~didn't find any that really worked that well. Yeah, 

[00:28:37] **Koyena Paul:** ~~like, ~~before I gave,~~ like, you know, ~~a couple sentences, I literally started with,~~ like,~~ start of text or,~~ like,~~ just a dot or,~~ like,~~ an opening bracket.

[00:28:42] ~~Like, ~~yeah, I tried a bunch of them, but they didn't seem to, like, work as well either, ~~so. ~~Yeah, but it was working a bit better than ~~like, you know, linear, ~~linear models of course, but still not really as great. Yeah. 

[00:28:53] **Nathan:** That's interesting. Okay. So now what comes next though ~~is, ~~is perhaps even more surprising in view of the fact that you tried multiple [00:29:00] actual natural language prompts and none of them worked.

[00:29:02] The next approach is Saying, okay, well, you know, where we're going, we don't need language. It's the soft prompt technique, right? Where this time you're learning what the embeddings should be from a sort of hypothetical abstracted prompt. Like what would the ideal prompt be if we didn't have to represent it in tokens and we could just go straight to the numbers.

[00:29:23] And engineer it at that level so that we could get ~~the, ~~the tokens out the other end that we want. So ~~you're~~ in this case, the optimization is tweaking those embeddings across all of the activation to future token prediction pairs and by optimizing those embeddings, now you can really start to get somewhere.

[00:29:44] **Koyena Paul:** Yeah, that sounds right. That's exactly what we did. That's surprising. 

[00:29:47] **Nathan:** ~~I guess what really, ~~what kind of jumps out at me, obviously, now looking to the results. That method works by far the best. And how do you understand why that works so much better? ~~Like, ~~is there any ability to say What the ultimately ~~like ~~learned [00:30:00] soft prompt means, can we translate that back into something that I can understand?

[00:30:04] **Koyena Paul:** We were actually attempting to do that. We were like, okay, we found a soft prompt that works great. Let's try to like, ~~you know, ~~get a discrete one, but it was ~~kind of ~~pretty gibberish. So it was like, okay, we'll keep it in like the vector space for now. How gibberish was it? ~~I think. Like it,~~ it had like a couple of at somewhere and ~~like, ~~it had some like ~~word, like it was not words.~~

[00:30:19] ~~It's like,~~ they looked like words, but then ~~they didn't, ~~they didn't make sense kind of words ~~that~~ those were, ~~that's what, that was,~~ what was there. ~~Let me see if I can check out and see if I can pull. If what that was, if I had stored it anywhere, but ~~yeah, it was pretty gibberish. So ~~yeah, we,~~ we just went on with the vector space soft prompt, but yeah, in terms of ~~like ~~the results, ~~I think, well,~~ it was nice to see that there was a, ~~you know, ~~pretty significant increase.

[00:30:35] And the reason I imagine is because this. Prompt is trained so that, like whatever intervened state we have, ~~like~~ it enhances, ~~you know, ~~whatever the feature context is ~~decode, like ~~encoded in there. And so because, ~~you know, like~~ in the manual versions, ~~like~~ we were thinking of ~~like ~~what the prompts could be, like what we think would make sense.

[00:30:53] But over here, this is what made sense of ~~compute ~~computer. ~~So, ~~yeah, 

[00:30:56] **David Bau:** ~~it's, ~~it's amazing that, ~~you know, ~~basically ~~there, there's,~~ there's this little Capability [00:31:00] in the transformer to solve this problem, right? ~~To, to, to, ~~to tell you, ~~you know, ~~what the future tokens are. ~~It ha~~ it has some little machine in it that knows how to decode it.

[00:31:09] ~~And, ~~and Kona ~~with, ~~with her soft prompt training, basically came up with a prompt that is like a key that like it's sort of this capability to do it. ~~That's~~ at least that's ~~kind of ~~the way ~~I, ~~I see it. ~~And so, ~~but the key doesn't seem to correspond to ~~any specific ~~Any real piece of text other than this weird gibberish that she saw, right?

[00:31:24] Yeah. It wouldn't have been something that we could have predicted. 

[00:31:27] **Nathan:** It reminds me very much of the Universal Jailbreak paper which we did an episode on and there was sort of a similar, now they were operating in token space but still often found these Universal Jailbreak prompts to be ~~kind of ~~gibberish sequences.

[00:31:42] And sometimes they did have some that were like more human readable. Now, this was something that you guys did a lot, right? Like ~~the,~~ all of these techniques,~~ right,~~ are happening at each layer. So for each of these techniques, you had to train like ~~for, ~~for the soft prompts, there's what, how many layers ~~in, ~~in GPTJ, is it 28?

[00:31:59] So you had to [00:32:00] train 28 different soft prompts, one for Each layer at which you're going to patch in the 

[00:32:07] **Koyena Paul:** activation. So that was what the method was initially, but like the actual feature lens, ~~you know, ~~the tool, we just use one soft from ~~like, ~~we use the best model, the best layer that worked. ~~You know, we, ~~we did that for every state when we, Actually built the tool.

[00:32:21] So in the tool, it's like one, but then ~~I guess~~ we were using this method to find which was the best soft prompt to use if you may. ~~So, ~~

[00:32:26] **Nathan:** yeah. Gotcha. Okay. So yeah, let's talk a little bit more in detail about the results. ~~I mean,~~ I think these are suggestive, ~~you know, ~~of many, certainly it's a good graph to just sit and ponder for a little while again, folks can,~~ can, can~~ refer to the paper to see this as a figure four from the paper, basically what you've got here is four different graphs.

[00:32:44] Each one corresponds to the token that is being predicted. So n equals zero. The first graph is like predicting the current token that it's equals one, the next token to the one after that three, the one after that. And then for each of these predictions, you're able to look at, okay, put the [00:33:00] layers across the X axis and the success rate on the Y axis.

[00:33:03] And you can see that as you proceed. Through the layers, the prediction success changes. For the first token, the current token,~~ you know, ~~basically you recap the logic lens results, right? Where you can ~~sort of ~~see that as you move through the layers, the predictions get more and more accurate. By the time you're at the end, ~~kind of ~~by definition ish or close to definition ish at the end, ~~you're like getting.~~

[00:33:24] ~~You know, ~~you're getting the answer right, close to 100 percent of the time. 

[00:33:26] **Koyena Paul:** Yeah, that was our sanity check for ~~n,~~ n equals zero. We were like, okay, is this method actually working? Let's make sure it's actually, ~~you know, ~~decoding the current token. And ~~so, ~~yeah, that was more of a sanity check. So 

[00:33:35] **Nathan:** then, ~~I mean, ~~several things jump out at me about the next three.

[00:33:39] One is that, again, we ~~kind of ~~already said that the two, Linear projection methods basically worked almost exactly the same. Like you can see that those lines for tokens one, two, and three are in almost lockstep, ~~you know, ~~for, through every layer, those did not work that well. And in fact, and this is kind of surprising too, on the first token, they beat the 20 percent baseline a [00:34:00] bit, but then on the second and third tokens, they're actually worse than the baseline.

[00:34:04] I guess maybe the baseline ~~is, ~~is ~~sort of ~~out of domain there at that point anyway. But I wasn't expecting to see things. Go lower than the baseline. Really? 

[00:34:10] **Koyena Paul:** Yeah, I assume so. We created like the Bigram baseline and so for n equals two and equals three would be like tri gram and like the four gram ~~like~~ models, ~~which are like too,~~ they were too huge for us to compute ~~at that ~~at that time, and so yeah, that's why~~ I guess~~ we didn't include the 20% in there, but yes, ~~I think~~ it's more to do with the fact that it was trying to predict ~~like ~~two tokens ahead, three tokens 

[00:34:30] **Nathan:** ahead.

[00:34:31] So the baseline is not so relevant. pass just the immediate next token. ~~Okay,~~ so ~~those are kind of, ~~you probably don't have a paper with those methods, right? Because they didn't work that great. The next one is the fixed prompt. This one actually does go below the baseline on the first one. So again, I'm like, man, that seems weird.

[00:34:47] ~~You know, ~~why would it be? lower than the straight baseline. And even to make that more confusing, that method seems to get better for the subsequent tokens. Like it's worse than predicting n [00:35:00] equals one and it gets better at predicting n equals two and n equals three. And that really surprised me. 

[00:35:05] **Koyena Paul:** So to provide a bit more context.

[00:35:06] So when we were checking n equals two, n equals three, ~~we,~~ we assume that we give like the correct token for the ~~previous, ~~previous ones. So ~~like, ~~let's say we are talking about, ~~okay, let's just say~~ New York City, for example, ~~but the example is too simple at this point, but let's say we are sure. Yeah. So~~ let's say n equals zero is predicting new.

[00:35:20] One is York, two is city. So ~~like,~~ let's say, because there are so many possibilities after new, that ~~like, ~~it doesn't really predict York, but if we give New York ~~and like, ~~if not, if we give New, if we give York, can it actually then predict city? And so that's ~~kind of like~~ the idea behind ~~like ~~checking for two and three.

[00:35:37] Cause ~~if~~ generally, if one is wrong, then it's pretty much wrong. Pretty sure that two and three will be wrong if you check whole phrase wise. So that's why ~~I think,~~ yeah, we gave ~~like ~~one extra token context in that sense. But with that, it's essentially, ~~yeah,~~ the same thing with one additional,~~ um,~~ token, ~~like~~ nothing else, like whatever the current token was.

[00:35:54] **Nathan:** Can you help me understand that a little bit better when I am imagining porting An [00:36:00] activation over two different contexts. How should I understand that? Like mechanistically interacting with the idea that there's another kind of subsequent token. included. 

[00:36:10] **Koyena Paul:** Yeah. ~~And~~ so ~~ like when you do give, you know, ~~ when you do transplant that hidden state ~~to like the new, like~~ to the fixed context, yes,~~ it's like, ~~it's actually completely from a different step at this point.

[00:36:18] ~~And so the,~~ let's say we did this transplantation at like layer 14. So from layer 14 onwards, it would have the context that is present in that hidden state, but If sometimes that's not enough, as we saw in ~~like, you know, ~~the fixed prompt result, ~~I mean, ~~like n equals one, but let's say if we gave ~~like, and~~ that particular hidden state, plus, ~~like~~ what the next word could have been so like York, in that sense, ~~and maybe like this, ~~maybe the reason why it's performing better, it's ~~like, ~~okay, because it now has like a direction of like, where it could predict next, but even then, it's just ~~like~~ that hinted ~~that~~ single hidden state and that particular one token.

[00:36:50] **Nathan:** So interesting. So~~ it's getting.~~ With that method, it's getting more information. Does that also help me understand? Because another thing that I was quite surprised by [00:37:00] is that the performance of that fixed prompt method seems to be pretty clearly declining as you go through the layers. And whereas the first two, ~~you know, ~~the linear transformation ones are like ~~kind of ~~flat ish climbing a little bit.

[00:37:13] The fixed prompt one is declining. And I was like, Hmm. That seems like a very odd. reversal from the ~~sort of~~ main logit lens. Do you have an intuition for that? And ~~do you think that~~ does that have something to do with the extra tokens that it's given? 

[00:37:26] **Koyena Paul:** So yes, ~~I think~~ in some contexts, but ~~I believe that like~~ usually the way I imagine just as ~~like, you know, ~~the first like last layer is that from beginning, it's~~ like~~ trying to ~~like ~~build an understanding of what it's going to say.

[00:37:37] And then in the middle, it has ~~like ~~these set of ideas that it wants to say and towards the end, it probably wants to say immediately. What it thinks it should be next. And so in that sense, I imagine there could be some information lost along those layers when it's ~~like, you know, ~~ultimately trying to predict literally the next token in that sense.

[00:37:53] ~~So, ~~yeah. 

[00:37:54] **Nathan:** Yeah. And what you just described is definitely my intuition as well. The sort of gradual working up [00:38:00] of. Inputs into higher order concepts through, ~~you know, ~~at least half. And ~~I would say ~~my general sense is that in many models even goes ~~kind of ~~deeper than that. ~~Like my guess, my, my ~~ kind of ~~sort of ~~rough picture in my head is ~~like ~~more through like 80 percent ~~of, ~~of layers.

[00:38:12] And then, yeah, in the final layers, it's like, now we're ~~kind of ~~condensing again, like now ~~we've got to,~~ it's time to actually cash this out. ~~You know, ~~all this sort of high order or high concept work that happened in the middle. Now we got to cash that out to a concrete prediction. And so you ~~sort of ~~see a collapsing toward the end.

[00:38:26] And that is very much what we see in the soft prompt one. So a couple, ~~you know, ~~notable facts about the soft prompt results. ~~Like, ~~first of all, they're just a lot better than everything else. And second, they do ~~kind of ~~More follow this pattern ~~that, that you just,~~ that we both each just described of seemingly more and more information buildup, that's more useful rising line from the beginning up until the middle layers and then declining.

[00:38:49] And ~~my guess is that like. ~~Just ~~this, you know, ~~this sort of peak here is in the middle and I've seen ~~kind of ~~later peaks in other models. My guess is that's probably just a function of model size where, ~~you know, you've got to, got to,~~ you ~~kind of ~~have to have that end time and, ~~you know, ~~that limits ~~how much, ~~how deep into [00:39:00] the model you can ~~kind of ~~continue to build.

[00:39:01] Does that seem right to you? Yeah, that 

[00:39:02] **Koyena Paul:** definitely seems right to me. And ~~I think this is ~~the whole idea of like the middle layer importance. ~~Like~~ it ~~kind of ~~is something that I've seen ~~like~~ in other interpret papers as well. And ~~so, yeah, I think, ~~yeah, there's definitely something along in those middle layers, middle late layers as well.

[00:39:15] **David Bau:** It is interesting how it declines, right? It definitely suggests that at the late layers, it's erasing some information. That, ~~you know, ~~it's using that space for something else. And, ~~you know, ~~it sort of explains this decline over time. So~~ I, you know, ~~I feel like ~~the phenomenon,~~ the whole phenomenon of a transformer erasing its own information, ~~you know, ~~is an interesting one.

[00:39:32] And, ~~you know, we're, ~~we see hints of it here. It's ~~another, another, ~~another cool thing to study. Yeah. 

[00:39:36] **Nathan:** What else do you take away from this set of results that I haven't landed on myself? ~~So, ~~

[00:39:41] **David Bau:** ~~you know, I, I feel like ~~one of the things here is that, ~~you know, ~~the information is present, but we weren't able to decode the information directly.

[00:39:48] ~~You know, ~~somehow the transformer's own circuits are essential for decoding the information. That's a pretty interesting insight ~~that the, ~~the mental model I have is like the transformer has its [00:40:00] own dictionary in its weight somewhere of how to decode concepts into sequences of words. ~~I, ~~I love the example that you chose in the final version of your paper, ~~the back to the future one,~~ back to the future, right?

[00:40:11] ~~You know,~~ like the movie title back to the future, ~~you know,~~ the longer sequences of words. ~~And I, ~~and I imagined that.~~ You know, ~~it's not actually directly in the hidden state, the instructions of how to decode back to the future, but it's more like a pointer. ~~It's more like, ~~it's just this compact vector that you have to look up.

[00:40:28] In the model weights somehow, and it's that soft prompt that Glenn and I learned that is, ~~you know, ~~triggering some mechanism that causes this lookup to happen that eventually rolls out to the whole phrase back to the future. So I thought this was pretty interesting. ~~I, you know, if it was,~~ if the decoding was simpler, we would have found it through one of these direct decoding methods, but ~~it's, ~~it's something that's encoding is complex enough that the transformer itself is needed.

[00:40:51] **Nathan:** Yeah, so something I said earlier, maybe ~~I'm, ~~I'm now thinking is perhaps wrong because I had said, okay, two linear Transformations don't seem [00:41:00] better than one and ~~I think~~ I jumped to the conclusion that like you could train a whole transformer But it probably wouldn't work. But now I'm thinking ~~hmm. Well, ~~maybe that's exactly ~~you know,~~ what would be needed ~~I guess ~~what does your intuition say if you were to scale up the Direct, ~~you know, ~~to go back to those first two methods, but instead of using a linear transformation, what if you use the full transformer to try to do the processing?

[00:41:19] Do you think that would work? Yeah, I 

[00:41:21] **Koyena Paul:** think ~~that would, that, that I like, I think~~ that should work better. ~~Just 'cause, you know, it has more diff like, there, there's~~ again with when you introduce ~~like~~ transformer, there's like the non-linearity thing, which was required for ~~like, you know, ~~the soft prompting like instances.

[00:41:30] So ideally ~~I think~~ it should work better, but that's not something we tried out. ~~So we didn't, I ~~

[00:41:33] **David Bau:** ~~don't think,~~ I don't feel like we had enough data to try it out. ~~Right. Yeah, exactly. We,~~ yeah, so, ~~so,~~ you know, ~~with, ~~this was a. Relatively small model training exercise you did, right? Where we're at every layer and every token, all these different settings, you're like training lots and lots of models, ~~but you know, ~~if you wanted to make a prediction on a large model like this, you'd probably need to train on millions or hundreds of millions of examples.

[00:41:53] And at that point, it's a little bit different, ~~right? You know, ~~it's almost like the task that you're trying to learn. You might be best off just memorizing the [00:42:00] whole thing,~~ right, right?~~ You could just say,~~ well, this, ~~this vector corresponds to these tokens. A few ahead and just memorize ~~the whole ~~the whole problem.

[00:42:06] ~~I guess ~~the thing that really surprises me about what coin I found was that. She didn't need to do that, ~~you know, ~~with a really, ~~with a~~ pretty small amount of data, ~~you know, ~~sort of 100, 000 samples, she could unlock the dictionaries for all of these phrases. And it wasn't like we're really training the transformer to do something new.

[00:42:25] ~~It's more, ~~that's why it feels like we're unlocking the knowledge that's already in the transformer. Does that make 

[00:42:29] **Nathan:** sense? Yeah, that's really interesting. ~~I think that's, ~~that's super helpful. And I understand exactly what you're saying about 100, 000 data points would not be enough to retrain a transformer.

[00:42:39] Maybe it could do the memorizing, but it certainly couldn't possibly relearn all the stuff that the full GPT J6B knows. because ~~it just, you know, ~~there's no way to get there from such a small sample size. So in theory, it could maybe work if you had the full pile and you ran the full pile this way, but obviously that's, ~~you know, ~~not feasible ~~on the, ~~on the [00:43:00] resources available here.

[00:43:00] So you can't recreate that magic. 

[00:43:02] **Koyena Paul:** When we basically add in another transformer, that kind of ends up becoming like a chicken and egg problem. Like we're trying to understand this transformer, but then we now have to try to understand the method transformer ~~to also like,~~ Yeah, 

[00:43:12] **Nathan:** ~~it's a bit,~~ it's a bit absurdist, no doubt.

[00:43:13] And it becomes almost ~~anti, ~~anti interpretability at some point as well. ~~It's so, ~~yeah, ~~I think that ~~that's definitely ~~a, it's~~ an intuition building exercise more so than a way to create insight into how the things are working. How big is the. Soft prompt, ~~this is, I guess each, like you could imagine,~~ I assume that individual tokens are embedded in the same 496 space?

[00:43:31] **Koyena Paul:** Yeah, so the, ~~I guess the~~ soft prompt size was like 10 by 4096, ~~like~~ assuming 10 tokens and each of this token having ~~like ~~4096 vector size, yeah. How does that compare 

[00:43:41] **David Bau:** to your linear models? Oh, 

[00:43:42] **Koyena Paul:** linear model, like the input was like 1 by 4096. 

[00:43:45] **David Bau:** Yeah, but ~~the, so, but those were like,~~ those models were like 4096 by 4096, ~~like.~~

[00:43:50] Ah, yes. Your 

[00:43:50] **Koyena Paul:** soft prompt is way smaller. Yes, that is true. It is much smaller indeed. Yeah. 

[00:43:54] **David Bau:** So even though it was the best performing thing, it was like ~~this,~~ the smallest number of parameters. 

[00:43:58] **Nathan:** It'd be like a thousand X [00:44:00] difference, right? Because ~~the, ~~the linear transformation were 4, 000 times 50, 000.

[00:44:04] Parameters. And this is 4, 000 times 10 parameters. 

[00:44:08] **Koyena Paul:** That's true. But I guess like the trade off is ~~like~~ the linear models trying to understand ~~like ~~everything, but we technically do have ~~the ~~

[00:44:13] **David Bau:** the transformer helping us out, but the weights are frozen. That's true. 

[00:44:16] **Koyena Paul:** ~~That's ~~

[00:44:16] **David Bau:** ~~true.~~ Yeah, ~~that's right.~~

[00:44:17] That's right. It's the power of using the transformer to explain itself. Yes. 

[00:44:21] **Nathan:** Yeah. Okay. ~~I mean, ~~that is really. Definitely very insightful. Did you try also varying the length of the soft prompt? ~~Like, ~~my mind goes to what if there were ~~no, you know, ~~no soft prompt at all? ~~Yeah, ~~Yeah,

[00:44:30] **Koyena Paul:** no,~~ I, I believe~~ my co author, Jude Ng,~~ like,~~ he definitely tried out,~~ like,~~ a couple variations of the prompts and found out that,~~ like, you know, ~~The size was like a good enough in that sense for this.

[00:44:39] And I'm not sure if we tried ~~like no~~ zero prompt, but I assume that would work similar to ~~like ~~a fixed prompt size, just cause ~~like, you know, ~~it is ~~kind of ~~like a fixed prompt. 

[00:44:48] **David Bau:** Yeah. It's something we don't know in detail. ~~Uh, you know, I, I don't think it,~~ we didn't see anecdotal evidence that it made a huge difference to make the prompts at different sizes.

[00:44:55] So we just ~~sort of picked, you know, ~~picked a relatively small prompt and tested it. 

[00:44:58] **Nathan:** Can we go back to the fixed prompt again for a [00:45:00] second? I'm still a little kind of not content with my understanding of why that would actually perform worse than the bigram. ~~It seems like it's, you know, ~~I don't know, I would expect it to do better.

[00:45:11] ~~I don't know.~~ I'm struggling. ~~Like it feels If~~ that feels like such a natural idea, ~~you know, ~~that it seems like it would work better than just Such a simple statistic and yet it's worse and all of the ones you tried were worse Like there were none. ~~I mean, ~~I assume that you didn't pick the worst of the 

[00:45:23] **David Bau:** no, ~~no, no,~~ no This is 

[00:45:24] **Koyena Paul:** the best one.

[00:45:25] ~~I mean, I think like with the Case for N equals one. I mean, perhaps I'm imagining that the baseline like, so the baseline definitely saw a lot more than a hundred thousand tokens. It was again with the pile. And so I think it had like a better, ~~

[00:45:25] **David Bau:** ~~this was, this is, it's training free though. Right. This is the thing.~~

[00:45:25] ~~Yeah. So it doesn't really depend on the training set. That's true. You know, my, my,~~ my, my intuition is this is so.~~ You know, we, we, ~~we show these various successes ~~of, and you know, ~~the function vector paper is an example of this, where ~~if, ~~if you like, go and intervene directly in the hidden states or the Rome paper, you go directly intervene in the weights of the model and we show, oh, it does something amazing.

[00:45:41] But actually. This isn't generally the case, ~~you know, ~~imagine ~~sticking, ~~sticking a random probes into somebody's brain and then saying, Hey, you~~ you know, ~~know, I wonder if this will make you smell the scent of bananas, but you know, generally,~~ it's not, ~~it's not possible to have a success with an experiment like this.

[00:45:59] So ~~I think sort of. ~~[00:46:00] Despite our best efforts at prompt engineering some very clever thing for the model to be set up to do this Just jamming in this hidden state at the end of these engineered prompts. ~~It just ~~it just didn't work ~~You know,~~ it's just doing some sort of brain damage And ~~you know, ~~it's really not getting it to predict anything, ~~you know, ~~very useful~~ But you know, ~~obviously like you said like a natural thing to 

[00:46:20] **Nathan:** try Yeah, fascinating.

[00:46:22] ~~I mean, ~~certainly we can say it's out of domain, right? You're putting it into a state that is clearly very unnatural, where all of a sudden, ~~and you, ~~and you still have more computation to go from that particular place of patching. So yeah, ~~I guess~~ that ~~still, ~~still feels weird, but ~~it's, ~~it's far enough out of domain that it ~~just, ~~just can't handle it.

[00:46:39] And 

[00:46:39] **David Bau:** it's possible that there is some way to make this work that we weren't able to figure out. ~~I mean, ~~so ~~we, we, ~~we tried our best with a bunch of different setups for this sort of manual prompts. And this is ~~sort of ~~the best example that you can see. But it's certainly possible that there's some structure that we're missing or some clever way of setting it up that would make it work better.

[00:46:58] In fact, so we could talk about the [00:47:00] function vectors paper also later if you want,~~ but, but, you know, that they, ~~there are some other tricks that you can find to get these kinds of interventions to actually work pretty well. 

[00:47:07] **Nathan:** I was curious, ~~you know, ~~if people. Like me are ~~sort of ~~still feeling like they, ~~you know, ~~want to go try another fixed prompt and see if they can't find the, ~~you know, ~~the magic words ~~to ~~to make it work.

[00:47:15] What is the tooling look like for all this sort of stuff? What is the coding 

[00:47:19] **Koyena Paul:** look like? There are no variations of ways to do about this. But when I was working on ~~like, ~~The fixed prompts, definitely. I was using actually David's ~~like ~~bow kit, a tool, which allows me to, ~~you know, ~~look into a model,~~ trace,~~ trace it and ~~like ~~grab the hidden state and ~~like, you know, ~~put it in like another run.

[00:47:36] ~~And,~~ but then there is a very recent tool called insight, which also does this, ~~but in a very like, It's, ~~it's basically like, ~~I think~~ the successor of ~~like, um, ~~pocket and ~~like, ~~it allows us to do all these like patching, ~~you know, ~~interventions and all these,~~ like, you know, ~~just basically a few lines of code.

[00:47:50] **David Bau:** Yeah. You have ~~like ~~a open source release for this project, right? Yes. ~~Okay. So So every website now, I don't remember what we ~~

[00:47:54] **Koyena Paul:** ~~call it.~~ We call it future. bowlab. info. And ~~so, ~~yeah, ~~that's~~ over there. We do have the code as well. [00:48:00] And yes, ~~I think it's like~~ basically in the code, I have like notebooks and scripts and yeah, people can refer.

[00:48:05] To that, in that sense, ~~but the future lens, like the tool itself, like in terms of, again, grabbing the hidden states because by then insight was released at least on our end internally. I think that that's what I particularly use in terms of ~~

[00:48:06] **David Bau:** ~~coding. So actually I don't even know the code. So yeah. On the future lens website.~~

[00:48:06] ~~Is it an insight based feature lens implementation? Or yeah, ~~

[00:48:06] **Koyena Paul:** ~~I, I started off with the inside. ~~

[00:48:06] **David Bau:** ~~Also, we have to explain to people what insight is. And that's great. ~~

[00:48:06] **Koyena Paul:** ~~Yes. Yeah. Yeah. Basically, like a friend of mine was working on this like anti project and I was kind of like the early adopters for it. And so I found it useful personally.~~

[00:48:06] ~~Yeah. ~~

[00:48:06] **David Bau:** ~~So, ~~so yeah. So definitely check out kind of.~~ You know, ~~repo for trying to, ~~you can, they,~~ people can try their hand at seeing if they can get a clever prompt that works better or some variation on the method. ~~I think we'd be, ~~we'd be delighted to see if there's some clever trick that we missed. ~~I think there's, ~~there's definitely room for creativity in this direction.

[00:48:22] Absolutely. 

[00:48:22] **Nathan:** ~~What would that,~~ so ~~you, ~~you give a pretty good intuition already for what that would look like. You've got the open source code, you've got a library that's specifically designed to ~~kind of ~~facilitate this sort of. activation extraction and patching and the loops, ~~I guess, ~~surrounding that to actually run a test.

[00:48:37] I should be able to do this probably in just even like a Google collab notebook, right? I would think. So~~ I ~~

[00:48:43] **Koyena Paul:** ~~think~~ because of the model and everything, you might need a Google collab pro,~~ but I think I'm not,~~ I haven't run the training part, but again, the testing part with ~~like ~~the future lens,~~ I guess~~ I've tried it on collab pro and it works.

[00:48:51] Yeah. ~~Have you, ~~

[00:48:51] **David Bau:** have you used the end of 

[00:48:52] **Koyena Paul:** back end? ~~I, so~~ yes and no. I used it on the server actually, but ~~not, ~~not necessarily remote equals true because I was like, I'm on the server anyway,~~ you're, ~~

[00:48:59] **David Bau:** ~~you're, ~~you're a little [00:49:00] bit of a cheater because ~~you're, ~~you're sitting next to the implementer, but actually a lot of the students who are playing with, ~~you know, ~~future lens and these kinds of things.

[00:49:07] ~~The, the library that actually~~ that library was developed by, Jaden, his good friend Jaden. And the library supports a remote backend that we're trying to get funding to, to provide ~~like~~ a scalable free backend for people to do interpretability research. We call it the end if. Backend. It's like ~~a, a, a, a, ~~a deep inference fabric.

[00:49:25] And,~~ uh, and~~ so if~~ if you, if~~ you code your interpretability experiments using this idiom, this little library, then, well, if you have the GPUs to run your model, then you can just run them locally. ~~But, ~~but if you don't, ~~if you, ~~if you need resources to run a model that,~~ uh,~~ there's too big for your laptop or for your Colab.

[00:49:44] Environment or something, then you can just flip a flag. You can just say use a different back end. then the experiment will be run on a shared remote backend for you. ~~And, uh,~~ so yeah, ~~so~~ there's, we have GPTJ running and we've got different LLAMA 

[00:49:59] **Koyena Paul:** [00:50:00] models. Yeah, I think the 70 billion model as well 

[00:50:02] **David Bau:** as, Yeah, like LLAMA 70B, which is a pain in the neck to run on your own, but, ~~you know, we,~~ we have that running.

[00:50:08] ~~And then what do you, what model is it that you're using it for, for experiments now for your next thing? Oh, ~~

[00:50:08] **Student-2:** ~~I'm ~~

[00:50:08] **Koyena Paul:** ~~still using GPT. Oh, you're using, I thought ~~

[00:50:08] **Nathan:** ~~you were using one of the Mistral ~~

[00:50:08] **Koyena Paul:** ~~models or something like that. Oh, so that was for another, yes, um, I was trying on Mistral, uh, the 8x7b in Strata. Oh, 8x, oh, the Mixtral.~~

[00:50:08] ~~Yes, yes, Mixtral, yeah. ~~

[00:50:08] **David Bau:** ~~Oh, cool, yeah, so there's Mixtrals running on it and things like ~~

[00:50:08] **Nathan:** ~~that. ~~Cool, so you have a single library that kind of abstracts away the subtle, I mean, all these things are transformers, of course, but they have, Differences in terms of their implementations, vector sizes, et cetera. Oh, 

[00:50:19] **David Bau:** no, they're not all transformers.

[00:50:21] ~~So yeah,~~ like ~~we have, we have, ~~we have folks using it to study Mamba, for example, these states based 

[00:50:24] **Nathan:** models. That's definitely of strong interest to me. 

[00:50:27] **David Bau:** Yeah. ~~Yeah. That's pretty fun.~~ It's pretty fun stuff. ~~And so, uh, so, so, ~~okay. So people who are interested in this, ~~this, ~~library,~~ it's,~~ it's embryonic, but it's pretty cool and there's a really nice dynamic community around it.

[00:50:36] So the library is called. N-N-S-I-G-H-T-N is the, ~~is the,~~ uh, URL tika to it. We haven't really promoted it, so I don't know if you search for it on Google, if it'll come up even. Right. It's ~~kind of ~~a little bit of a secret alpha stage project right now, but if you go to n insight.net, there's like ~~a, a, ~~an icon in the corner ~~to ~~to link to a Discord channel to join ~~and, ~~and ~~there's, ~~there's a bunch of tutorial and [00:51:00] documentation.

[00:51:00] On it. But the really valuable thing is to just join the discord and ask around. And, ~~you know, ~~there's a really friendly community that's developing it. 

[00:51:07] **Nathan:** That's awesome. Is there anything that we can say about the bigger or more intensively trained models as compared to GPT J? ~~You know, ~~my hypothesis would be that you would probably find higher success rates with bigger models because you would, in theory, hope that they have ~~You know,~~ more semantically meaningful middle state representations.

[00:51:29] Yeah, 

[00:51:29] **Koyena Paul:** ~~I think I,~~ I would go along in the similar direction as well. It's just that ~~I think ~~with bigger models, you also need bigger data set for it to ~~like, ~~potentially ~~like, you know, ~~train and ~~like ~~be more exhaustive in that sense. But ~~I think~~ like in terms of takeaway wise, ~~like~~ at least till now, for example, ~~the, you know, ~~the whole middle layer stuff, I think it should still be something that is pretty ~~like ~~transferable ~~and~~ like other.

[00:51:48] Models as 

[00:51:48] **David Bau:** well ~~as as as as ~~as an advisor person here. Yes, I'll say ~~this is this is a ~~this is a gap in our knowledge and ~~we need to ~~we need to run some more experiments. So, ~~you know,~~ you're right. I think that the intuition that you have. Which is that there might be more [00:52:00] structure as you get larger models, and it actually might become more interpretable in this way.

[00:52:05] It's really interesting. It's a little counterintuitive. ~~I think that, you know, ~~traditionally people would imagine that as models get bigger, they might become less interpretable and harder to understand. But ~~this, this, this, ~~this intuition that you're ~~sort of ~~sharing here, that maybe ~~it,~~ it becomes. more structured, more predictable, easier to understand ~~that ~~that might be true.

[00:52:22] But ~~it's,~~ it would be quite a claim, ~~you know, ~~some more research is, it's definitely in order ~~to see, you know, you know, ~~to systematically take a look at these kinds of questions. 

[00:52:28] **Nathan:** Is there anything interesting that you can share about the, probes that have been sent into the Mamba universe so far. I did for reference a two and a half hour monologue about the Mamba paper in December.

[00:52:41] And ~~I definitely feel like, and we're, we're, you know, ~~ I'm counting actually along with another like minded states based model fan. I think we're up to very close to, if not hitting 20 papers now published downstream of the Mamba paper. Paper with, ~~you know, ~~different remixes and hybrid versions all over the place.

[00:52:58] So, yeah. Have you found anything interesting there? 

[00:52:59] **David Bau:** [00:53:00] Yeah. All these attention free architectures, you can basically ask ~~how, ~~how are they doing it? You can try to lay things like logic lens on top of them, or try to build future lens on top of them. ~~And, and, ~~and to some extent, ~~you know, ~~there may be in surprising ways.

[00:53:14] they show some similarities to transformers. Now, ~~we don't, ~~we're sort of halfway through doing some research to try to figure this out. And so~~ I,~~ I don't want to lead any of your listeners astray ~~by, ~~by saying something that's not actually true, but yeah, even though they are missing a traditional attention mechanism.

[00:53:32] ~~You know, they, ~~they seem to be able to do some of the sophisticated types of computations that transformers use attention for. ~~And so, ~~so exactly how it all works. ~~I think~~ that we're still trying to untangle it. ~~That's sort of our, we see it as our job as an interpretability lab to try to get in there and untangle some of these things.~~

[00:53:43] **Nathan:** Yeah, cool. All right. I'm looking forward to that. ~~If you have,~~ if you don't have a striped hyena in that menagerie already, definitely throw one of those in there at some point as well. Cause I don't know if you've seen ~~the,~~ just from the last few days, there was a usage of the striped hyena to do a DNA foundation model, [00:54:00] which is starting to show some really interesting properties, ~~you know, sort of.~~

[00:54:03] ~~A long,~~ first of all, super long context and straight pain is it's a hybrid. So it has attention and also the state space. And my sense definitely is that some sort of mashup is, ~~you know, ~~going to be the winner for a lot of scenarios in the future. Certainly in this DNA paper that just came out, they showed that the transformer was the least effective and then Mamba was a bit better, but then the most effective.

[00:54:25] Hybrid attention and state space was the best performing. And ~~it, ~~it is ~~like~~ kind of uncanny because it's sort of like, ~~if you,~~ if you believe the theory that the language models are learning some sort of world model representation through next token prediction by analogy, this seems to be learning some sort of like life model, or ~~maybe, ~~maybe better said would be like cell model at the level of just next base pair prediction.

[00:54:50] ~~It's, you know, ~~it's a whole other world that's, ~~you know, ~~got obviously its own tremendous interpretability challenges, but definitely fascinating space. So plus one for the,~~ uh,~~ striped hyena in your next round [00:55:00] of experiments. 

[00:55:00] **David Bau:** We will be investigating these things carefully. ~~I think that it is, it's a, ~~it's a very exciting time as the world potentially moves on to whatever comes after Transformers.

[00:55:07] It'll be very interesting. 

[00:55:09] **Nathan:** Yeah, ~~it's not the,~~ I always say it's not the end of history. Do you want to talk a little bit about the function vectors paper? ~~ This is one that I've skimmed. I haven't read in the depth. So I can't go all through the methods in the same way, but. ~~

[00:55:13] **David Bau:** So the basic question for function vectors was, Eric was very interested in asking, how does in context learning work?

[00:55:22] ~~It's just, ~~it's just this amazing thing. I mean, it was the foundation for, ~~you know, ~~all the excitement. around GPT 3 was this ability for a model to seemingly learn how to do a task after seeing a half a dozen examples of the task being done. Then you give it another half worked example and it'll work it the rest of the way.

[00:55:41] It's just amazing that these models are so good at doing that. And ~~so, ~~so ~~what, ~~what Eric was looking for is ~~there, is there, ~~is there some localization in the in context learning task? What he found was that there is, ~~that there's~~ a bottleneck in it between when you give a set of demonstrations and when you ask a model to [00:56:00] generalize.

[00:56:00] Yeah. Come and join 

[00:56:02] **Nathan:** Eric Todd. Welcome to the Cognitive Revolution. 

[00:56:04] **David Bau:** So yeah, ~~so Eric, ~~Eric is the author of the Function Vector Paper ~~and, and I was just about to say what function vectors are an answer to what question they answer. ~~So actually maybe now that you're here, you can just sort of. Explain what it is.

[00:56:10] ~~And so yeah, what the heck is a function vector? ~~

[00:56:10] **Student-2:** Yeah, so we found that there are like a small set of attention heads. That's when you process an ICL prompt that mediates the identification of a task. ~~So, ~~for example, let's say you give a bunch of examples of like antonyms of big and small, short and tall.

[00:56:29] And then you give it another query word like a bright. And the model, ~~you,~~ you can. Extract ~~this, ~~the output of a few attention heads ~~that have like ~~from some other context where they saw a bunch of antonym pairs and take this output and stick it into this new context and it'll give you the antonym of the 

[00:56:46] **David Bau:** word that it's processing.

[00:56:47] ~~So, ~~so if you take the same attention heads. Yeah, ~~and and ~~and you read out what those same attention heads are saying ~~if you a bunch of other things~~ if you said Paris France Moscow Russia, ~~you know, ~~Washington DC [00:57:00] United States~~ and then ~~and then you said Ottawa Blank, right? ~~Well, you know, ~~but then ~~you ~~you read the attention heads at that moment~~ And, ~~and then instead you have a totally new context where you have, ~~you know, ~~Ottawa or something like that, or you have Madrid or something like that.

[00:57:13] Even though those attention heads were the ones that seemed to cause you to say antonyms in, ~~in one of the,~~ one of the experiments. In this experiment, if you read out the attention heads for the country capital task, you And you stick it in to the new context, it seems to encode the new task. It'll actually say Madrid goes to Spain instead of doing antonyms or something like that.

[00:57:38] ~~Or,~~ and what, ~~what~~ other types of tasks did you test? You tested how many? 

[00:57:41] **Student-2:** Yeah, we tested ~~like, ~~like 40 plus different tasks. And it seems like they're all mediated by this small set of heads, which is ~~kind of ~~cool that. It seems like the model has this sort of path that it communicates this task information or like this bottleneck, I guess, that it's communicating.

[00:57:57] What the task is that it's [00:58:00] doing, even though ~~like in the, ~~in the prompts, we're never explicitly telling it what the relationship between ~~the, ~~the demonstration and the label are, it's able ~~to, ~~to figure that out and communicate it 

[00:58:08] **Nathan:** forward. Yeah, this is cool. ~~So you,~~ I'll just ~~kind of ~~re summarize it and make sure I have it right.

[00:58:11] So you, first of all, set up a task implicitly with a few shot prompt. Which is the original GPTs are a few shot learners, right? ~~The, ~~the original paper title, few shot learners refers to the ability to understand or infer and actually do the task just from a few examples. So pretty fundamental, ~~you know, ~~notable behavior without question.

[00:58:34] So okay, set up a couple of these examples, thus creating a few shot prompt. One example is antonyms. Another example could be translation. So arrive, depart, small, big, common, rare. And then at that point, as the pattern has been established, you go looking inside the transformer for, is there some, and I'd love to hear a little bit ~~kind of ~~how you think about the term bottleneck, but ~~the, you're,~~ you're going and looking, ~~I guess, ~~for some sort [00:59:00] of relatively small dimensional thing that you could extract.

[00:59:03] And patch over to another context. And now when you find that thing, and obviously that's where all the hard work is, but then the demonstration is that when you have found that thing and you do in fact, extract it now in a clean setting, without any examples, you can set something up and say the word fast means, and then inject this representation Give me the antonym.

[00:59:27] And instead of doing what a language model would normally do, which is define what fast means, you now says the word fast means slow, because you've ~~kind of ~~forced the antonym behavior with the patching from the, Few shot context now over to ~~the, ~~the clean context. 

[00:59:44] **Student-2:** ~~Right. ~~Yeah. ~~Yeah. You're, ~~you're right about bottleneck,~~ like,~~ so attention seems like a natural place to look just because that's how transformers move information between tokens and we figured ~~like.~~

[00:59:54] In order to gather information about the task from your context, you'd have [01:00:00] to do that via attention. Like if you never explicitly tell it what the task is, you need to go back and look at all the other tokens to figure out what you're doing. And attention is, it's nice because attention heads act on a small subspace.

[01:00:12] And so they're natural bottlenecks for like sparse activations. 

[01:00:16] **Nathan:** So what is it exactly that you are extracting and patching over? Is it the. ~~It's the~~ output from an attention head? 

[01:00:23] **Student-2:** Yeah, that's right. So you can take the output of these, this small set and just add them all together. And that's the actual thing that we call a function vector is this sum of attention head outputs.

[01:00:34] And then you can add this vector into some other prompt at a particular layer in 

[01:00:39] **David Bau:** the model. 

[01:00:40] **Nathan:** ~~So, ~~so it's one vector that represents the sum of multiple different attention heads, but you're ~~kind of ~~selecting which attention heads to look at. And ~~that's ~~obviously a big part of the challenge is figuring out which ones to look at.

[01:00:50] Once you have that sort of thing, ~~does it,~~ does the relationship between tokens need to have some sort of length similarity [01:01:00] to the original length relationship? Or not really because all of the information passing between tokens has already happened by the time the attention head is done, right? 

[01:01:09] **Student-2:** It doesn't need to.

[01:01:10] It doesn't seem like that matters that much. Seems like fairly robust to different settings. So ~~we, ~~we tried it sticking it into like natural text settings, different templated settings. ~~I mean, ~~it seems like it works just the same for ~~long, ~~

[01:01:24] **David Bau:** long or short. Yeah. Isn't that cool. How 

[01:01:27] **Nathan:** do you figure out which attention heads to use and what can we say about the relationship between the different attention heads that together make ~~the ~~the vector ~~like it's ~~it's nice to think of this like single vector but then it's ~~kind of ~~weird to think of these different heads ~~sort of ~~contributing to like part of ~~this ~~this sort of single conceptual vector.

[01:01:45] **Student-2:** Yeah. So we found that a lot of these heads have had a similar attention pattern, which is kind of interesting. most of them were attending to previous label tokens, which is like you have demonstration label, demonstration label. So they're [01:02:00] basically like looking at all of the answers of all the. Pairs, which kind of suggests that maybe,~~ and,~~ and some other papers have found, like when you do ICL, these label tokens seem to be sort of places where the model stores important information.

[01:02:15] And so there must be something about the pairs where it's able to,~~ like,~~ figure out the task and it's ~~sort of ~~transporting that task information from those labels. onward. The way that ~~we, ~~we found these heads was we do a process called causal mediation analysis. Also people sometimes call it activation patching.

[01:02:33] So basically ~~this,~~ the setup is you have ~~one,~~ one sentence with a bunch of words. Pairs of words demonstrating a task and you have some other sentence where you can set it up where it's maybe demonstrating some other task. We decided to scramble all of the labels so that it wasn't really clear what the task was.

[01:02:54] And then what you do is you patch the activations from ~~like ~~one [01:03:00] attention head into this other setting where it's not clear what the task is doing. So you take it from the clean setting into ~~the ~~The jumbled setting and measure ~~how, ~~how much it influences the models,~~ uh,~~ output of the word that you would expect to ~~the B~~ the behavior to induce.

[01:03:16] So for example, if in your jumbled setting, the query word is like big ~~and you, ~~and you paste in an attention to output from an antonym setting, you'd expect that the models output. For small would go up slightly and like~~ it ~~just doing one attention head isn't enough to ~~like ~~flip the prediction. So we ~~kind of ~~started trying multiple attention heads.

[01:03:35] And it seems ~~like ~~once you get to around like 10, you can start having ~~like ~~a significant causal effects of getting the model to flip its prediction and ~~like ~~start understanding what the task 

[01:03:45] **David Bau:** is. So to me, the big surprise was, ~~you know, ~~Eric got this working for, ~~you know, ~~about 10 attention heads for like antonyms.

[01:03:52] ~~And then, ~~and then he looked at something else. ~~I, you know,~~ I think in the paper, we looked at like English to Spanish translation or something. He had a bunch of different tasks [01:04:00] and he went and he started looking at the attention heads for these other tasks. And we noticed that they were largely the same attention heads.

[01:04:07] And so if you just ~~like ~~picked up your attention heads from one task and use them on a different task, ~~It would,~~ that whatever information is in those same attention heads would tend to induce the new task too, which was like, it was really surprising. Like I could imagine that there's ~~like ~~some antonym attention heads, but it was very interesting to find that there are these attention heads, which are just like general function 

[01:04:29] **Nathan:** task understanding, right?

[01:04:30] Yeah. Yeah, that's really interesting. And it looks like from the figure three in the paper, ~~it looks like~~ they're ~~kind of ~~found mostly in the middle layers, but not like all at the same layer. They're kind of mixed at different parts ~~of the, ~~of the middle 

[01:04:41] **Student-2:** layers. Yeah. Most of them in the middle. ~~I think~~ maybe there was like one towards the end, but yeah, ~~I think~~ it ~~kind of ~~matches our intuition~~ of,~~ I sort of see transformers as having ~~kind of like ~~two processes.

[01:04:51] One is ~~like ~~figure out what I want to from the context and then use that to predict the next token. And so like you could see maybe the first half of the network [01:05:00] doing the figuring out and the second half using that to predict a token. And ~~like, ~~like ~~it's, ~~it's cool that right in the middle, right before it like starts to predict the token ~~is, ~~is where this process is happening.

[01:05:09] Yeah. 

[01:05:10] **Nathan:** That's fascinating. Obviously recently mixture of experts has been a huge trend, right? With your GPT 4 allegedly being a mixture of experts model and your mixed role. And of course now Gemini 1. 5, ~~you know, ~~has been declared to be a big mixture of experts model as well. So I've been ~~kind of ~~looking into what is known, what is understood about mixture of experts and it's like most of the mixture of experts papers are focused on swapping out the MLP blocks because that's where like most of the computation is at least if the context window isn't huge but now obviously with context windows getting huge you know that's starting to even out or maybe even tip the other direction and so I guess people are also, ~~you know, ~~increasingly starting to do a mixture of experts where the attention blocks are also ~~kind of ~~switched out at runtime.

[01:05:58] So I wonder how [01:06:00] this kind of finding should help me think about that. It certainly, at first blush to me, sounds like, geez, That's a pretty complicated structure. Yeah. There is like, you've got 10 different heads ~~that are,~~ and you could have had more, right? ~~You kind of drew,~~ if I understand correctly, you kind of drew a arbitrary line and said like, this gets us most of the 80, you know, Pareto principle type of thing.

[01:06:17] ~~Right. ~~So it definitely seems like it's a sort of distributed process. ~~You know, ~~the process of identifying the task is a distributed process. It's kind of like mixed throughout layers, ~~mixed throughout, there are multiple, I guess when I was looking to see like,~~ yeah, it is interesting. There's like, Two in the first layer where they exist, two in the second layer, one in the third, one, one, one, one, and then it ~~kind of ~~goes quiet, at least in your top 10.

[01:06:37] I wonder, ~~I mean, ~~maybe one way to think about it is ~~like, ~~maybe there's like one to two of these per layer. I don't know. ~~It's, ~~it's an interesting just mashup. I wonder if you have any intuition for how this would help us understand mixture of experts. 

[01:06:48] **David Bau:** ~~Let me, ~~let me answer in my interpretability professor advisor way.

[01:06:52] Okay.~~ You know, ~~I guess the way I look at it is this, is that we don't know yet. What is the [01:07:00] right level of abstraction that we should be looking at to understand these things? So we know the physical things that we made them out of, that we have dimensions, we've got nonlinearities, we've got modules of different types, we've got these NLPs and attention layers and cool state space recurrences and other neat things that people have suggested.

[01:07:21] And so ~~we know how You know, it, it, it,~~ in the end it's all just matrix multiplications, right? , ~~you know, ~~we know what we're building these things out of, but we're not sure yet exactly the right way of looking at all of these computations ~~and, ~~and ~~the, you know, the, ~~the attention heads. So Rome was a way of looking at the MLPs and saying, Hey, there's this interesting association structure in these MLPs.

[01:07:43] It seems to be pretty. ~~Pretty~~ informative, although amendment sort of qualifies that and says, well, you know, I'd be distributed on a few layers. And, ~~you know, ~~it's a little bit more subtle~~ and, ~~and all of this great mechanistic interpretability work, I think, has been a way of looking at all these attention [01:08:00] heads.

[01:08:00] And saying, oh gosh, these attention heads also reveal a lot of interesting computational structure, and I think, ~~you know,~~ that ~~that ~~motivated a lot of Eric's work. He says, oh, is there an attention head? Maybe there's a few. And so there's definitely a structure in the attention heads. To me, it's not 100 percent clear ~~that ~~that's the end of this story, that, ~~you know, ~~it may be like ~~when, ~~when Eric finds that, ~~you know, ~~a dozen attention heads are working in concert with each other, then it leads to the question.

[01:08:25] Is there some abstraction? Is there some way that we should be looking at these attention heads? All together, and I actually see function vectors is one proposal for a way of doing that, right? ~~That, you know, there's, this is, this is just just sort of,~~ you can summarize all of these attention heads in a single vector.

[01:08:40] And even though we've sort of blurred them together, and we've lost a bunch of the fine grained distinction that. The vector has pretty strong causal effects. It has some interesting properties ~~that, you know, ~~that Eric investigated in the paper, like to some extent these vectors can be composed ~~and, and, and, ~~and do interesting things.

[01:08:57] And so, ~~so I think that, you know, ~~I don't know if function vectors are [01:09:00] going to be one of the abstractions in the end~~ that's that that ~~that's like the right way of looking at what these things are doing ~~but ~~but ~~I think that~~ what it hints at is that there's potentially more structure to be found maybe at a higher level even than what we've been looking at.

[01:09:13] So far,~~ and,~~ and ~~the big, I,~~ to me, the big game, the research game and ~~the, the, the, ~~the chase that we're all on in the interpretability world is to figure out the answer to the question, what is the right level of abstraction? 

[01:09:23] **Nathan:** That's great. ~~I think~~ that might be the perfect note to end on. And you guys are doing admirable and certainly laudable job of chipping away at this massive problem.

[01:09:31] I'm a big fan of. All the work that I see, anytime I see a Vallab paper, I'm excited to get to the website and you guys do great visualizations as well. So definitely encourage people to go to the individual paper websites and see the visualizations, the animations. 

[01:09:45] **David Bau:** For visualizations. ~~Let me, ~~let me give a shout out to Nikhil who just archived his paper.

[01:09:50] That's also going to be at ICLR. We didn't talk about it today, but he has the best circuit visualizations out of anybody. ~~He, he, ~~he really has done a really great job at putting those together. So check out his [01:10:00] paper. It's called fine tuning enhances existing mechanisms. So ~~it's this, it's this, ~~it's this whole study of the interplay between.

[01:10:06] Circuits and fine tuning and ~~you know, it's, it's, ~~it's also an interesting paper,~~ but,~~ but really beautifully presented as well. 

[01:10:11] **Nathan:** Yeah. We will save that one for next time. This has been a great conversation guys. Eric Todd, Coenah Paul and Professor David Bao. Thank you for being part of the Cognitive Revolution.

[01:10:19] **David Bau:** Thanks Nathan for having us.


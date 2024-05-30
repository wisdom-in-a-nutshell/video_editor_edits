#### 00:00:00.209

Professor Kevin Haysfeld, welcome to the Cognitive Revolution. Thank you, Nathan. Pleasure to be here. I think we're going to have a perhaps enlightening, certainly enlightening, perhaps a sobering conversation. I'm really looking forward to getting a better sense of where we are in this moment where obviously we've just had a pandemic not too long ago and you've put a lot of your energy in recent years into delaying, defending against, and detecting if one is coming our way. I'm really interested also in the intersection of AI and biology that has really caught my attention recently as something that, even as someone who's obsessed with AI, I've been sleeping on. So, a ton to get into. I want to start just by giving you a little chance to tell the story of your career up until the current period. 


---


#### 00:00:44.834

You're the leader of a group called the Sculpting Evolution Group. You've pioneered a technology called Gene Drives and done a bunch of other biotech stuff as well. I think it's maybe helpful to give people a bit of a perspective on your pro-technology bona fides before we get into some of the more worrying aspects of your outlook.   
(00:01:06.465) ~~Right.~~ (00:01:06.665)  
Well, I suppose I should disclose that early on, I really loved the natural world. I love the beauty and the splendor of living things. And I wanted to learn how to make similarly beautiful creatures. So from very early on, trip to the Galapagos, that got me into reading Darwin, reading about evolution. And I wanted to learn to make similarly marvelous things. 


---


#### 00:01:31.474

And that's driven me all the way through, which is why I'm in biotech today. Now, I confess, if you gave me the power to rewrite much of nature with biotech, I would probably use it. I'm not super confident that it's a great idea in all cases, but in certain cases, I would definitely go ahead and do it. And this has been a bit of a moral dilemma because my career has involved some technologies that actually do open the door to allowing us to do those kinds of things, at least on a limited level. But I want to do this because I wanted to understand how biology works. How does evolution really operate? And to discover that it's in fact a somewhat impoverished algorithm, when it really comes down to it, relative to other accessible algorithms, has been a letdown and also just an inspiration that we can plausibly learn to understand how nature does it, learn to understand how evolution works, and do it better. 


---


#### 00:02:32.150

I find that tremendously inspiring because, yeah, we make mistakes. We've screwed up the environment to some extent. I think we have an obligation to try to fix that. We've caused a lot of animal suffering. I think we have an obligation to try to fix that. But I think increasingly we have the tools to do it. It's always interesting talking to an audience focused mostly on AI, because that's the only field that might arguably be going as fast as biotech. When I started, most projects just flat out failed. Still very often projects fail, but for the first time in some areas of molecular biology, if you have an idea. there is a good chance that you can actually get it to work. 


---


#### 00:03:13.330

And that's amazing.   
(00:03:14.931) ~~Yeah,~~ (00:03:15.070)  
that's a profound statement right off the bat. I say that about AI all the time, that it seems like just from the cadence of papers that people are publishing, it seems like all their ideas are working. And people will, of course, be quick to say, well, there's a lot of failure in research. But I'm like, yeah, but looking at your calendar of quarterly papers, it seems like there couldn't have been too much failure along the way. So it is fascinating to hear that biology is trending in that direction as well.   
(00:03:38.987) ~~When you say, so yeah, go for it.~~(00:03:41.150)  
Yeah. So I can jump in. So I cut my teeth. I wanted to make as big of an impact as I could accelerate biotechnology as much as I could. 


---


#### 00:03:50.038

And I reasoned that initially I wanted to do stem cells because I think that aging is bad and being forced to die is a bad thing, being forced to wither away and die is a bad thing, and we should stop that. So at first I was interested in stem cells, but I concluded that field didn't need me and wouldn't do anything for at least 10 years. Turns out that was a correct assessment. Although there's now, again, a lot of progress. I concluded what we needed was tools, because if you invent a new tool or technology, then you can catalyze the work of many others. And that's typically much more impactful than if you just try to push the frontier forward yourself. 


---


#### 00:04:27.350

And then, because   
(00:04:28.329) ~~I always~~(00:04:28.610)  
sometimes go a little bit too far in some things, which is a flaw of mine, I reasoned, well, if you develop a technology for developing new tools, that should be even better, right? So I wanted a way to harness evolution to make molecular tools much more quickly and reliably than we could ever do before. And with evolution, it's basically how many organisms do you have, exploring how much genetic space, how quickly. So I wanted to take the fastest evolving thing we could and harness it to evolve useful molecular tools for us. And that is the bacteriophage, viruses that infect bacteria, which can have a generation time as little as 10 minutes, really fast. 


---


#### 00:05:10.805

And I reasoned, well, what we need to do is move a gene we want to evolve onto the genome of the phage. And then we need to steal one of the phage's genes, program it into the bacterium, so that the phage needs the bacterium to turn on that missing gene in order to replicate. And then we engineer the bacterium to only turn on that gene in proportion to the molecular activity we want to see. So what we've done here is we've incentivized the bacterium to evolve our gene to get better and better at jumping through our hoop in order to get its critical protein back and replicate. So as a result, all of the phages compete to optimize our gene to do the molecular trick that we want. 


---


#### 00:05:55.327

So we called it phage-assisted continuous evolution, or PACE. And it's basically a synthetic ecosystem that we created to harness evolution to evolve new molecular tools. And it's been very useful. My advisor then, David Liu, his lab has used it to develop a lot of the base editors and prime editors and other variants of CRISPR, which I'll talk about next, that are now in gene therapy trials doing really amazing things. So that was my PhD. Then I moved across the river over to Boston side to Harvard Medical School. I worked at the Wyss Institute as a technology development fellow. And I worked with George Church. And one of the first things I did was try to solve a contamination issue. 


---


#### 00:06:35.242

There was this cute new technology called CRISPR, which had just been discovered in bacteria. And so I played with a few different CRISPR systems, trying to immunize my bacteria against phages that were getting in the way of some of my experiments. And it worked really well, just out of the box, first try, which is, again, pretty rare. And then Jennifer Doudna published her paper showing that CRISPR could be used to cut DNA in vitro in a way that indicated it probably would work well in eukaryotic cells for genome editing there as well. And I thought, well, that's going to be transformative. I should think about how we can use this because it's going to be shown to work in mammalian cells and be a broadly useful tool. 


---


#### 00:07:20.338

And one of my friends and colleagues, Prashant Mali, who's working in the church lab, came to me and said, hey, wait a minute. You've been working with Cas9. I've been working on the pipelines to see how well gene editing works in mammalian cells using the prior technology talons. We should team up and get CRISPR working. And I said, why? Jennifer's had a six-month head start. And he said, because this is going to be so big, that if we discover even one tiny piece that someone else would have missed for a couple of months, the impact of those couple of months will be more than worth it. And he was right, because we did discover that you needed the complete guide RNA for full activity. 


---


#### 00:07:59.750

And that did not come out in the first few papers. And in fact, we were one of the first papers. And then we did a bunch of other things in CRISPR, turning genes on and off, inventing what's called a nick case. So you just nick one strand, which can give you higher fidelity editing. And using multiple CRISPRs in one cell, getting it working in other species, that was a great year. Just the world was your oyster back then. And then we got bored because, okay, you got great molecular scissors. It's a addressing tool. You can send it to whatever DNA sequence you want anywhere. You can tag it with anything and send it to that sequence in order to manipulate gene expression, edit anything you want. 


---


#### 00:08:37.346

Amazing tool, but obvious in terms of what all the applications are. There wasn't anything fundamentally new there. And then I wondered, OK, we can now edit lots of things. And CRISPR tends to work on the first try out of the box. Will we be able to use it to edit wild creatures? Because this was my original dream, right? Learn how to program biology, including in the wild. But just because you could edit something doesn't mean you can keep it doing the thing you want in the wild. Because when we engineer an organism, we're doing it for our benefit to jump through our hoops to solve our problems, which means we're redirecting its energy, its resources, away from survival and replication to doing the thing that we want, which means that our changes are almost always deleterious, harmful to the organism in the eyes of natural selection. to anthropomorphize a bit. 


---


#### 00:09:24.298

And so natural selection wipes the floor with our changes. And this is why, despite widespread concern over GMOs in places like Europe, A lot of their regulations actually assume that an engineered change will have positive fitness in the environment and spread, which in general is pretty laughable. It's hard to beat nature like that. And so I reasoned, well, we could edit a bunch of organisms and release them. Sure, have a transient effect, but it wouldn't really last. And then I thought, well, what would happen if we programmed the organism to use CRISPR genome editing on its own? That is, we didn't just use CRISPR as scissors to cut the gene we wanted, provide a replacement copy. 


---


#### 00:10:04.528

What if the replacement copy also encoded the CRISPR system that made that change? That way, if the organism was sexually reproducing, then when it mates, the offspring gets a copy of our engineered change and the CRISPR system required to make that change. And then CRISPR would edit the copy they inherited from the other parent and copy itself and the engineered change over. And I realized I had just reinvented one of nature's favorite tools, which is called a gene drive. It just cheats at inheritance by cutting its genetic competitor and copying itself over. The difference is that CRISPR lets us easily target any sequence or multiple sequences that we want. So you could, for example, have it cut multiple sequences, 


---


#### 00:10:49.160

And then in order to resist that, it would need to acquire mutations at every site we program CRISPR to cut, because that's what blocks a gene drive. If you have a mutation so that CRISPR can't cut, it doesn't work anymore. You can't do the cut and replace, because the cut doesn't work. But we can program CRISPR to cut at multiple places, making it arbitrarily more difficult for evolution to come up with a set of mutations that would block it. So in other words, we could use this to build a gene drive, yes, most genes in many organisms if we could get the efficiency of the copying high enough. but we could also make it stable. 


---


#### 00:11:25.875

And I thought, wait a minute, wasn't there someone who was working on using a different kind of cutting gene to try to build something like a gene drive in malarial mosquitoes? And yes, there was a team trying to do that, but it wouldn't work well precisely because it was a single cut. CRISPR could just solve it, target other genes, other ways. You'd have multiple shots on goal. Evolution is always cleverer than you eventually, but you could always have build another gene drive and another. We could stay ahead of nature. And that means that we could plausibly eradicate malaria and schistosomiasis and edit other species. We could eventually, rather than spraying our fields with pesticides that have downstream ecological effects and aren't necessarily great for us, how about we program the pests to avoid our crops and otherwise go about their normal business? 


---


#### 00:12:21.091

At this point, there's so many amazing things we could do with this technology. But then the next day I woke up and realized, wait a minute, right now you have script kitties playing about pasting their graffiti in various places online, as well as on bridges. What if you could do that in living things? Who will have access to this technology? Because what we're talking about is something where you engineer one organism and you let it go. And months to years later, you've edited the bulk of the species. Could you use this as a weapon? After all, if you can engineer mosquitoes to not carry malaria, you could probably engineer mosquitoes to reliably carry a disease. 


---


#### 00:13:03.306

And so I didn't actually tell anyone. I thought about it myself, trying to figure out, would this technology favor offense or defense? And thankfully, I concluded it favors defense. It's slow, spreads parents to offspring over generations. It's obvious if you look for it. Sequencing will always tell you if there's a CRISPR-based gene drive in a relevant organism. It can even sequence the river water. And if it's in anything in that watershed, you'll pick it up and see it. And it's easy to block. The technology allows you to block itself. It's its own counter. Because one gene drive can overwrite another one. So if there's a gene drive you don't like, take that exact gene drive, remove the parts you don't like, give it instructions to cut and overwrite the original, 


---


#### 00:13:46.243

And it will do that, and it will spread through the population just like the original and immunize it against the bad one. So anything slow, obvious, and easily countered is just not much of a threat. So I concluded that it was in fact a safe technology, that you really couldn't misuse it. But I was worried because of precisely that GMO problem, right? The first GMOs were developed for Big Ag, and Big Ag is controversial. And we ended up with a big backlash against biotech. And we had suffered from a similar thing in gene therapy. One death from a poorly planned clinical trial resulting in tragedy, Jesse Gelsinger, shut down the whole field of gene therapy for over a decade. 


---


#### 00:14:28.826

And so here is a technology that could eventually help eradicate malaria, schistosomiasis, all these other amazing things that we would want to do. We needed to not screw it up. And I was worried because, in particular, a lot of my colleagues who work with engineering organisms are used to their edits being selective against. They don't worry about containment. for, say, engineered fruit flies, every fly lab I'd ever encountered had flies buzzing about in the corridors. And some of those flies were funny colors. Well, if you build a gene drive to turn flies a funny color, then if it worked as well as I suspected it would, you'd turn a whole lot of the fruit flies funny colors. 


---


#### 00:15:06.671

And I could just imagine the headline, scientists accidentally turn entire species to GMOs. Is CRISPR to blame? And then you'd have a backlash not just against gene drive, but also against all the amazing things we were doing with CRISPR in biomedicine. And that seemed bad. So I spent the next couple of years figuring out how to tell the world about gene drive and ensure that we wouldn't screw it up by having an accidental release of a drive system. And trying to ensure that the first application would be something that is really hard to argue as it would be a bad thing. Something like targeting malaria. And indeed, there's a great group called Target Malaria that's working to do just that. 


---


#### 00:15:47.693

That's my story to how I got to thinking about this. And so I studied,   
(00:15:51.054) ~~continued to develop.~~(00:15:51.956)  
Now my lab does a whole lot of robotics and machine learning for lab automation purposes, because I have a great life. I have a whole lab that I have a great idea. I can share it with someone. And if they're suitably inspired, they'll go off and test it in the lab, which is great. But we want every bioscientist to be able to do this. So we really just need fully automated labs, cloud labs, where you have an idea. You can formulate it in the appropriate language. And the experiments will be run. And I think lab automation is a fantastic, again, enabling platform to accelerate biotech. 


---


#### 00:16:25.277

And as we move into various machine learning tools, including for protein design, biodesign, then it just gets even better. But we need the data from high throughput laboratory experiments in order to train those models. Because in bio, it's not like large language models. we are already extremely data constrained, and just adding more parameters does not give you very much. So we need a lot more biological data characterized on the kinds of tools that we're interested in order to train those models. And that's a lot of what my lab does today, along with projects like persuading communities that they should help guide research on how to engineer white-footed mice so they can't infect ticks with Lyme disease. then the ticks won't go on and affect kids. 


---


#### 00:17:13.682

Because we thought that this is a local problem that people might care enough about to want to engineer animals in the environment. And it would be a good way to figure out, OK, how do you ensure that communities actually guide the research to produce a technology that they would want to use and gives them a voice early on? And so I've spent a lot of time arguing that we need to be more transparent with how we do science, that this is a lever in ecotechnology with which to move science, because we still don't disclose our best ideas until we've had a crack at them ourselves. Because if you share your best idea, you really do run a risk of someone else throwing more money and hands at the problem and scooping you. 


---


#### 00:17:58.046

The incentives are wrong. Because if you were setting up the system to advance science as quickly as possible, you would want people with good ideas to share them freely. And allow whoever is best positioned to get them working. We don't because   
(00:18:11.407) ~~we are still~~(00:18:12.328)  
we inherited a system at least in academia to still descended from the days when the Royal Society thought it was   
(00:18:18.172) ~~a.~~ (00:18:18.192)  
correctly, a genius idea if instead of scientists sending letters to each other, they should send them to the society who would then bundle them up into a journal and send them out to all of the researchers. And our model is still based on that, even though we have much better communication. 


---


#### 00:18:33.583

We could be much more open with our science. And I think that would make science both faster and more robust and more trustworthy, more trusted by the public, which ultimately holds our leash and has to fund us. So I thought this could be a lever with which to change everything. So I am a bit of a transparency zealot, I confess, in the whole field of ecotechnology. Okay. A ton of great threads there. I want to just attempt a real quick summary of a couple of key ideas in case people are not already familiar with them. But the overall overarching point there I think is well made, that you are someone who has obviously embraced the future of technology, has been pro-sharing, pro-access to information, pro-transparency, and has even gone as far as to deploy, right? 


---


#### 00:19:20.778

This technology is not just theoretical, but has actually been deployed into the mosquitoes at least, right? Has it also been deployed into the mice?   
(00:19:29.144) ~~Well,~~ (00:19:29.365)  
it works in the mosquitoes in the lab. It works in large cage trials. It works in flies. It works in a bunch of insects. And it has not yet been released. They have tested various non-gene drive versions in the wild in Africa. as laying the groundwork for the gene draft. Because of course, diplomatically, it's complicated. You're talking about engineering species across a whole bunch of different nations. How do you get everyone bought in? It's really complicated. And part of the reason   
(00:19:57.324) ~~that's~~ (00:19:57.523)  
why we wanted to try with the mice, because everyone on the islands of Nantucket and Martha's Vineyard, which are guiding the project, everyone there at least knows someone with technical savvy to understand what it is we're doing. namely just take mice that have antibodies against the Lyme bacterium, encode those antibodies in the mouse genome such that it can be passed on to their descendants, which doesn't normally happen with immunity. 


---


#### 00:20:22.919

Imagine you have a five-year-old,   
(00:20:24.400) ~~right?~~ (00:20:24.559)  
And   
(00:20:25.319) ~~I imagine~~(00:20:25.700)  
you have the pink eye. And you do have a pink eye right now for your five-year-old, but you probably had a pink eye before. So wouldn't it be lovely if you could have passed your immunity on to your five-year-old such that everything that you would ever gotten sick with your five-year-old would have immunity to, insofar as sustained immunity is possible. That'd be lovely. It's not how biology works, unfortunately. But we can cheat, because we can grab the gene from your B cells that produce antibodies against a given pathogen, and we could encode it in your germline so that your kids would actually inherit that immunity. So that's what we're doing to the mice. 


---


#### 00:20:57.780

Admittedly took us, CRISPR is a great tool, but you still need to figure out a lot of other problems to engineer a mammal. Namely, you need to figure out some way to get the eggs, get CRISPR, fertilize them, get CRISPR into them, get the edit, then implant that embryo back into a pseudopregnant female such that the embryo takes and then the pups are delivered and they turn out to have the edit that you want.   
(00:21:23.201) ~~Well,~~ (00:21:23.300)  
there's a whole lot of things in there, get it from getting the eggs and the embryos in the first place to making, getting the pseudo pregnant mother   
(00:21:30.226) ~~to,~~ (00:21:30.365)  
to receive them, to getting the transfer to work and so forth that are, have totally been worked out in lab mice and took us five years to figure out in white footed mice. 


---


#### 00:21:39.633

So we have just figured out how to engineer the first white footed mice. We have shown   
(00:21:43.355) ~~that we,~~(00:21:43.575)  
that the, Heritable immunity trick appears to work in normal lab mice, and now we're finally putting the two together. But the communities seem to be very supportive. We have five different mostly uninhabited islands that have been volunteered for field trials. And what most stunned me,   
(00:22:01.455) ~~the~~ (00:22:01.556)  
One of the sort of sub-islands of Martha's Vineyard actually held a vote, without our knowledge, to support the project and volunteer their island as a, including all of their houses, as a field trial site. And it was over a hundred to zero in favor. It had been a bad lime year. 


---


#### 00:22:21.361

So that just blew my mind that, cause there's a lot of people there who are really uneasy at the idea of engineering the mice, but the fact that they're in charge, it's community driven, it's like the way we're going about it, even if they're not sure they actually like the technology, but they're. willing to support the project, including strongly support the project, because they think this is how science and technology should be done. And they see it as their project, at least as much as our project. So that's going really well. But we don't quite have the actual mice that we want with enough antibodies for what I hope will be evolutionarily stable resistance. But we have all the groundwork there, and   
(00:23:01.696) ~~I think we've come up with the hurdles,~~(00:23:03.057)  
come up with ways around the big technical hurdles. 


---


#### 00:23:06.340

We'll see. Obviously, statements like that often come back to bite you. Planning policy applies. But we're in good shape to actually make something happen. And this is insurance in case it's hard to get all the nations to agree. We can start on the islands with something that is not a CRISPR-based gene drive, but could, if it works, eventually be turned into something like that. Okay. So let me just make sure, again, I understand a couple of these concepts and folks have a clear sense of just how powerful this technology really is and by extension, how offensive it might be to someone who is broadly against intervention in nature. People have probably heard about CRISPR, certainly, and the idea that you can make a targeted edit in the genome, 


---


#### 00:23:56.439

I think is probably pretty familiar. And I think people have probably also heard of these mosquito experiments where a strain is bred, and then it crossbreeds with the native strain, and then the next generation becomes infertile or whatever and can't reproduce. But these are like one generation interventions that are out there in the world today. What makes this different is that it is,   
(00:24:22.487) ~~I don't know if there's a proper term for this, but~~(00:24:23.846)  
it's essentially super dominant,   
(00:24:25.428) ~~right?~~ (00:24:25.627)  
Where you edit it into one, potentially could be as little as one mouse,   
(00:24:31.269) ~~right?~~ (00:24:31.409)  
In theory, and that mouse over generations, because the machinery actually copies itself into the other chromosome can now become not just dominant in the next generation, but it also copies itself over, essentially precludes the possibility for downstream hybrids. 


---


#### 00:24:50.329

And now it's just like exponentially taking over the population. So is there a proper technical term for that? That doesn't really occur. You said it occurs in nature. I'd never heard of that occurring in nature before. Yeah, it absolutely does. It normally doesn't happen in sexually reproducing organisms. And Austin Burt, who worked out a lot of the theories studying natural gene drives, really the godfather of the field, I just came in and said, hey, there's this new technology, CRISPR, that will actually make it work and actually make it evolutionarily stable. Austin did essentially all of the heavy lifting. And his current theory, which is still dominant, is the reason you don't see it in creatures like humans, or at least in that cut and replace form, is that it's too powerful. 


---


#### 00:25:29.383

That is, Austin thinks that if you do get one that actually works, then either some of the time it cuts, and instead of getting copied, you get a mutation that then blocks further cutting. So either that mutation then outcompetes the drive, because it can't be replaced, or the drive is so successful it spreads to virtually all organisms, and then it's the victim of its own success. There's no more selection pressure to keep it able to cut. And so eventually it breaks and then is lost over evolutionary time. So you see the cut and replace in organisms that sometimes reproduce sexually and sometimes don't. Things like yeast, sometimes even in bacteriophages, oddly enough. where you sometimes get solo change of asexually effective reproduction. 


---


#### 00:26:19.480

And sometimes you get the mixing with sexual that then ensures that it never completely takes over. It's just a very useful strategy. So the ability to do it reliably in sexually reproducing organisms is definitely not something that we see in nature. But yeah, the term is gene drive. You can think of it as just inheritance biasing. And it's a fascinating case because we don't need to understand how the environment shapes natural selection in order for gene drive to work. It's a case where we needed to notice that inheritance is really important. Because a normal gene has a 50% chance of getting inherited by any offspring in sexually reproducing organisms. And if you can increase that, it's a powerful advantage. 


---


#### 00:27:41.119

And that essentially favors whichever version is in the majority. Because if you can't tell them apart, then obviously you have an advantage. You're more likely to mate with your own kind and have perfectly fine grandchildren if you're in the majority. And so the more skewed the ratio gets, the more dominant the majority allele becomes. So you can actually have the genes in an area vote, and whichever one is more common will actually win out in that area. And so that's a way of having a localized drive system, which is a lot of what our work is controlling this. But yeah, the power of it is, This is a way to engineer the bulk of a species. 


---


#### 00:28:17.483

And I want to say it works for every species because the cut and replace, the replace works better in some species than others. Works reasonably well in a bunch of insects. Thankfully, it works the best of all in the malarial mosquito. And we'll see on others. One of the things that I reached out to some folks in Uruguay over is this nasty creature called the New World Screw Worm. So this is where the animal suffering side comes in. But this is a bot fly that lays its eggs in open wounds, anything as small as a tick bite. And the maggots are screw shaped, and they drill their way in, devouring the living, healthy flesh. It's agonizingly painful. 


---


#### 00:28:52.039

And probably a billion or so animals a year, all mammals and birds, suffer from it in South America. We actually eradicated this species from North America. in Central America already by actually irradiating the larva and then releasing 100 for every one in the wild. So the released ones were sterile, and then the wild ones would mate with the released ones. It's called the sterile insect technique. It was some bright sparks in the 50s when nuclear power looked to be the solution to everything, even taking out biological pests. It's a pretty clever trick. But there's too many of them in South America for that to work. but gene drive could plausibly remove this species from the wild. 


---


#### 00:29:31.897

And why is that important? Well, a billion animals per year, mammals and birds we know can suffer horribly, are being devoured alive by flesh-eating maggots. Obviously, they would die of something else, but that's an unusually grisly and horrific and painful way to die. We could remove that species, which would otherwise stick around probably for a few million years. That's 10 to the 15th mammals and birds being devoured alive by flesh-eating maggots. And for comparison, even if we continued factory farming at more than the current rate for a century, that only be 10 to the 13th. So unless it's 100 times worse to be a factory-farmed boiler hen than it is to be devoured alive by flesh-eating maggots, it's more important that we eradicate the new world screwworm. 


---


#### 00:30:11.470

And we can even keep them on ice, because their larvae can be frozen and resurrected. So we don't have to drive them extinct. We just need to remove them from the wild and put them on ice. So this is the scale of intervention in the natural world. This is the beginning of what I had in mind. You can imagine some other cases. There's probably only four or so where you'd really want to edit a whole species, but that's one of them. There's two schistosomes that cause horrific schistosomiasis, malarial mosquitoes, and then perhaps my favorite just in terms of ideas of things that technology could do. the desert locust, God's eighth biblical plague. They're just harmless desert grasshoppers and it rains, the desert blooms, they undergo this amazing epigenetic switch, they change color, they go from being solitary to being gregarious, they form into swarms and they go screaming out of the desert and eat everything in sight. 


---


#### 00:30:59.672

A large swarm eats more than the population of Paris every day. So they cause massive famines, which is why thus the eighth biblical plague. Well, that switch is genetic. And so we could use a gene drive to turn them off. We know that they can stay solitary desert grasshoppers indefinitely. They don't need the swarming phase to survive as a species. So we could just switch swarming off. We could tame God's eighth biblical plague. Now, to do that, it would have to be the people who suffer from it, because it's their environment. It's their call. But that's on the level of the power that we're talking about. with this, which again, doesn't seem much compared to AI, but nevertheless, it's something. 


---


#### 00:31:37.392

Well, this is all invented before the AI enabled era in biology. It's remarkable to me often that we can figure out how to make any of this stuff work, especially given just how many complexities there are in these systems.   
(00:31:53.144) ~~So,~~ (00:31:53.284)  
okay. I think you've firmly established your credentials as somebody who is not afraid to think about how the world could be different than it is. And   
(00:32:05.412) ~~I guess~~(00:32:05.612)  
I want to now talk about, I see us walking a little bit of a tightrope now in the next phase of history for probably multiple reasons. But specifically, we can focus in on the intersection of AI and biology. and what that might unlock, but how stable or unstable that might be. 


---


#### 00:32:23.930

Especially, I have a thesis that the order of events here might really matter. If we knew a lot more than we did, then we might be able to make some of these moves with a lot more sure footing than we currently would have if we were to unlock certain new technologies. So   
(00:32:41.503) ~~I guess,~~(00:32:42.744)  
boy, there's a lot of ways that we could come at this. But maybe for starters,   
(00:32:47.048) ~~like,~~ (00:32:47.169)  
where do you think we are in terms of understanding biology at large? Like, how much do we know versus how much there is to know? And I was also definitely caught my attention when you said that data is a limiting factor. When I think of biology, 


---


#### 00:33:04.003

I think of like huge data sets. And so I was surprised to hear you say that you see the data as such a limiting factor. But what do you think is the sort of current state of knowledge and what is the path toward illuminating the rest of what's going on in biology through data and potentially through AI models to help us figure that stuff out? Yeah, so I think the problem is that even though we're getting better and better tools for reading DNA, which is still our primary method because an alpha fold strength is it tells you how to go from the DNA sequence to the structure of the protein, which is not the same as function. 


---


#### 00:33:41.173

And that's the great leap where we're not there yet. We don't yet know how to predict function. from sequence or structure. And that's because that's part of a complicated network of interactions that are not well understood,   
(00:33:56.077) ~~right?~~ (00:33:56.278)  
Yes, although it's fair that we're making a lot more progress in some areas than others. So David Baker's lab have been the leaders in protein design for some time. And that field has mostly solved the problem of making de novo binders. So if you want to   
(00:34:12.083) ~~bind to a protein,~~(00:34:13.224)  
bind to a DNA sequence, bind to an RNA, bind to some molecule, then we're now getting to the point where you can make N designs, where N is a manageable number for actually building and testing in the lab, where at least one of N will work quite well, such that you don't need to display a whole bunch of antibodies on phages, for example, and then have a column of the thing you want them to bind to, and then pass the library of phages down the column, and then you take the ones that stick and you sequence them to see what the antibody, which antibody it was. 


---


#### 00:34:48.456

Now you can just design a protein that will bind to that target directly, make a hundred candidates, test them in individual wells, one of them will work. And is that we can, how much faster or how much more resource efficient is that compared to what came before? It's mainly that you can make smaller and more elegant binders. Most of the structures of the binders that we use previously are somewhat constraining. And   
(00:35:14.603) ~~we, it's~~(00:35:15.583)  
the difference between having to start from a tool that from a module that evolution gave you in the form of it's somewhere in nature and you found it to being able to build your own module from scratch. And that works because binding is reasonably closely linked to structure. 


---


#### 00:35:31.916

So if you have the structure, it's easier to predict binding, because if you can model the two structures docking, then you can, in effect, predict how well you're going to bind. And there's a lot to learn, obviously, but you could also generate a lot of data precisely from running those kinds of experiments, where you make a whole bunch of designs, and then you test them to see which ones bind better than others, and then you feed that back into the model, and you do this for a whole bunch of different types, and we've been accumulating more and more data. In part because you have that structural intermediate, it gives you a leg up on this problem. 


---


#### 00:36:04.909

What's more challenging is enzymes. So this is where you're actually catalyzing a reaction, which is normally done by effectively stabilizing the transition state. So you can think of a chemical reaction as you have your starting materials, and then you have your finishing materials, and then there's this energetic barrier in the middle. and an enzyme reduces the height of that barrier by stabilizing the transition between the two. And that requires essentially positioning those atoms precisely enough to maximally stabilize that transition state. we're just not that good at it yet. It's a lot more precision required than binding requires. So   
(00:36:44.490) ~~we can now,~~(00:36:44.911)  
again, lots of levels of complexity. So we have a lot of still not understood interactions. 


---


#### 00:36:52.695

If we do understand an interaction, we can intervene and disable something, but we can't yet do an effective job of saying, I want to catalyze exactly this interaction because that's just another level up of complexity. Or at least it's extremely difficult. One of the most impressive papers I've seen was a Baker Lab paper where they made a luciferase enzyme, which is one that takes chemical substrate, causes it to emit photons, so it glows, bioluminescence. And they took a totally unrelated protein class that had roughly the right overall structure. And they designed de novo, an enzyme that catalyzed that reaction, produced light, using the structure of the unrelated protein. Incredibly impressive. I believe they made something like 7,000 some designs. and one of them had some initial activity that then could be improved by directed evolution or rational design, just   
(00:37:56.072) ~~trying to,~~(00:37:56.393)  
making mutations in areas that look like they're important, making all of those candidates, screening them, and so forth. 


---


#### 00:38:02.114

Once you have something with the starting, that has the starting activity you want, then it's very easy to use evolution.   
(00:38:07.217) ~~Well, I shouldn't say easy, that's what,~~(00:38:08.356)  
it's a whole art form, and it's still unfortunately an art, not a science, because we don't understand molecular function well enough to design it yet. And our AI tools similarly have not been given enough data on the relationship between sequence structure and function for most functions to solve it for us. We have given them enough data to do sequence to structure, but it's that structure or direct sequence to function link where we don't have enough data of different sequences that have the desired function. And so part of our goal in lab automation is to ensure that we can run enough experiments in very high throughput to generate that kind of data. such that then our models will get better at predicting how to do it. 


---


#### 00:38:56.574

So you might say, thinking back to Feynman, because everyone loves a good Feynman quote, what I cannot create, I do not understand. You can also think of it as the contrapositive. What I understand, I can create.   
(00:39:07.463) ~~Well,~~ (00:39:07.583)  
we don't yet understand sequence to structure to function quite well enough, and nor do our machine learning models yet. We primarily need more data because it looks like right now adding more parameters to the model really doesn't get you much. I've been struck by how small actually a lot of the models that I've superficially studied coming out of AI and biology have been so far. So I guess there's two levels of missing understanding then. I have recently been focused on the idea that   
(00:39:41.532) ~~like large,~~(00:39:42.885)  
like we just don't know how it works, right? 


---


#### 00:39:44.827

There's all these interactions going on in ourselves and our tissues and our overall organisms. And we just don't really know what is causing what to happen. And   
(00:39:53.851) ~~that it seems to me like~~(00:39:55.070)  
my sort of working model for how we're going to overcome that is we will probably just continue to collect   
(00:40:02.190) ~~like~~ (00:40:02.309)  
low-level raw data, like genomic data, probably get into transcription data, proteomic data, and then try to pseudo-label that with the overall   
(00:40:11.255) ~~sort of~~(00:40:11.474)  
higher level state of the organism. What is this person's blood pressure at this time? And just build that kind of stuff out and then create basically a foundation model for well-being is what I've started to call it where you have all this raw data and this sort of observational data on top. 


---


#### 00:40:28.273

And the hope would be that the foundation model would learn   
(00:40:32.215) ~~what,~~ (00:40:32.436)  
like how these low level inputs are through some   
(00:40:36.699) ~~opaque,~~ (00:40:36.998)  
opaque to us now mechanism, like creating these higher order observables. In addition to that, you're highlighting, tell me, first of all, if that's right or wrong. But then you're also highlighting this function thing, which is another three-dimensional space question, where the key point there is that we can predict the structure of the protein, but there's this additional level of how that interacts and brings other things together. And that is another key missing piece. Yeah,   
(00:41:04.657) ~~I think~~(00:41:04.856)  
that's right. I was focusing on the molecular side. You were thinking of a larger level, even more complex system. where, let's be humble, there's a lot that we don't know. 


---


#### 00:41:14.601

And one of my favorite papers was the one, you may have heard of it, where they wanted to know what were the tools of neuroscience efficient to understand the brain. And so by analogy, they said, okay, well, let's assume we have equivalently powerful tools and let's see if we can understand a circuit. They found that you couldn't. So Our current tools in neuroscience we don't think are sufficient to understand the brain because the circuit should be much more understandable.   
(00:41:39.523) ~~Human-designed,~~ (00:41:40.244)  
human-engineered things tend to be engineered in a reductionist manner such that each piece has a purpose and it tends to do one thing or at most two things, not more. Whereas evolution tends to write spaghetti code because if it can adapt something that's already there to take on a new role, tie into something else, sensitive, be slightly modulated by this signal because overall that's slightly advantageous, then it will do that. 


---


#### 00:42:07.126

And so lots of things talk to lots of other things and you get this tangled mess. It's harder to understand. than something that is designed to be cleaned from a reductionist perspective, which is why   
(00:42:18.755) ~~I think~~(00:42:18.916)  
we're also gonna make a lot of progress just by building simpler systems in isolation and then testing the individual components to see how they interact and then the bottom up get more and more complicated. Once we get enough data to go sequence to function, then we can draw on the fact that we'll have the sequences of pretty much everything once we get around to sequencing everything. And sequencing is an incredibly powerful tool. As I mentioned, sequence the watershed, you can sequence the river water, you can see everything in the watershed. 


---


#### 00:42:48.768

That's pretty incredible. Let's watch the abundance of all the species go up and down as the environment changes. That's going to be useful data. And we have all their sequences, so we know what all their proteins do. And so therefore, we know typically how those proteins interest probably conserved in many cases, but they're slightly different versions. And all of a sudden, that's data that you have that this thing interacts with that thing in this particular way, because we know that it did in the model organism, and it almost certainly does in all of the others. Boom, that's training data that you have. And so we'll build it up in this manner, and combined with better and better tools. 


---


#### 00:43:23.090

So if I had to say there's one key tool that we're missing, it's solving delivery. Because if we can get enough nucleic acids into a cell. We can make it do all kinds of things. We're getting pretty good in engineering. With CRISPR, we can edit the existing genome. We have enough tools in our toolbox   
(00:43:39.025) ~~stolen from different parts of nature or~~(00:43:40.487)  
created de novo that we can reprogram cells reasonably well. Obviously, I don't want to overstate, but reasonably well. We can at least take a lot of shots on goal and pull out the ones that work. The problem is in our bodies, how do you get that nucleic acid into each of our cells? If you can do that, then you can have the equivalent of software updates, changing what your cells do on the fly in response to whatever. 


---


#### 00:44:05.141

The challenge is, how do you get that delivery to happen? Because there's something else that wants to get into your cells in order to reprogram them, and those are viruses. And our immune system evolved to stop them from doing that. So you're fighting the immune system when you're trying to solve the delivery problem in biomedicine. So ideally, what we need is a way to engineer all of our cells to have a lock a special gate that has an ideally unnatural key, something that can't be synthesized biologically, but can be synthesized chemically using our tools, that then will accept a cargo of new information very efficiently. Then once you can engineer enough of our cells to have that, then every cell becomes engineerable in future, and then you can readily update them in response. 


---


#### 00:44:49.181

So something like that is what I would guess, where we would want to eventually go. And then as we learn more and more, we'll be able to program things. We'll be able to understand exactly what are the underlying causes of aging that are most important. We can program some cells to secrete factors that will deal with what we think is the cause. And if it turns out it's not the cause, it's just a symptom,   
(00:45:10.777) ~~well,~~ (00:45:10.996)  
it's probably not helping. and we'll have essentially better eyes on what's going on and at least increasingly understand and be able to intervene more effectively. So in the long run, I'm very optimistic. And then you add AI, which is a way to understand the system without us having to be the ones who understand it. 


---


#### 00:45:31.507

And I'm much, much more optimistic, but it's also true that some problems just seem horrendously difficult. De novo designing, say, a virus. You have to design the replicase that will replicate its genome. And the genome has to be replicable by the replicase, which you have to design de novo. And of course, that's an enzyme. But then you have to package it somehow into a coat that can be passed from one cell to another, which means you have to interact with the cellular factors. We have to recruit some of them to help you, perhaps. You need to get in the way of the ones that will try to stop you, the immune system. And then you need to figure out some way to not just pass from cell to cell, taking over each one, but also pass from organism to organism. 


---


#### 00:47:00.911

We're probably more likely to get those before we solve that one ourselves, which is probably important because sequence space is hyper-astronomically vast. So there's an incredibly vast number of possible de novo designed viruses that you could create that would spread efficiently in humans. And now we're getting to the meat of it. COVID taught us we can't defend against pandemics very well right now. There are pandemics that are nastier than COVID. We want to understand biology. That includes how things like viruses work, how the immune system works, how viruses evade the immune system. What are the fitness determinants of viruses in the environment? What is the equivalent of inheritance that is so important to them? And what we understand we can create. 


---


#### 00:47:44.494

So my worry is that we will learn how to make pandemics and things like that before we learn to defend against them. At a high level, when you talk to people who are in the AGI game, people at the leading developer labs these days, They seem to broadly agree that the path to some form of AGI is relatively clear at this point. They feel like they know what they need to do, and they have a pretty good sense that it's probably going to work over the next couple of generations. And that doesn't necessarily get us to superintelligence, but it does get us to potentially transformative technology, if we're not already at a transformative technology. How would you characterize the state of play in biology,   
(00:48:28.409) ~~do you feel like~~(00:48:28.909)  
there is a, doesn't sound like it's like as clear of a path, but would you say that your kind of mainline expectation is we're going to build these foundation models, they're going to start to grok these like deep relationships and it's probably going to work, or does it feel like there are aspects of it that are more fundamentally long shot than that? 


---


#### 00:48:50.614

I am a techno-optimist. I think we do have a path. I think it will likely work. I confess I'm a little bit concerned about possible demographic decline in the sense that we may need AI to pick up just because we may not have as many scientists, but AI looks like it's going quite nicely. Even if we never get to super intelligence, as you said, we just need to augment the capabilities of enough human researchers through lab automation and the like, through design models, allowing us to create better and better tools. And I think we're on a pretty good path. So   
(00:49:26.376) ~~I think~~(00:49:26.675)  
we will, if not solve biology, because it's incredibly complicated, we'll move quite far in the direction of understanding what's actually going on and being able to reprogram it. 


---


#### 00:49:39.521

And this is very welcome because I am not down with that withering away and ceasing to exist business. And I know a lot of other people are similarly not down with that. And I think fixing that is incredibly important. And as the screw illustrates, we might decide that we have some moral objections to the ways things work in the natural world. It's beautiful, but it obviously cares nothing for suffering, and we do. So maybe we want to fix that. I find that personally quite inspiring, but a lot of people find that quite alarming and horrifying, and I've spent enough time talking to communities that I respect their concerns. A lot of people feel like we're playing with fire. 


---


#### 00:50:16.789

And as a heuristic, they say, try not to make a major change. Try not to do anything that's super unnatural, because the further away you go from what is already there, then the more likely it is that something's going to go wrong, that you're going to touch on some aspect that was never explored in nature. And so current systems might not be resilient to it, which I suppose you can sum up as, if you're engineering a complex system that you don't completely understand, then you should try to make the smallest possible change that you think can solve your problem, just in order to minimize the collateral damage when things unavoidably go wrong. And then you test it, ideally in isolation, make sure that things look pretty good. 


---


#### 00:51:01.164

And if they do, then you scale up, which seems a reasonable set of deontological heuristics for how to go about engineering extremely complex systems, which certainly biology and absolutely ecology describes quite well. Of course, you could argue that for human society and technology too. When you think of the mechanism, what you just described in terms of the path to a sort of approximate solve of biology, sounded like getting language model or their successor type AIs to essentially do similar work to what human scientists are doing, like automating of experiments and gradually bit by bit,   
(00:51:43.043) ~~like~~ (00:51:43.224)  
illuminating what's what. Do you see a similar amount of promise in this like sort of Evo and its successors type paradigm to just throw all the data into one giant black box and hope that it grocks what's going on and then be able to study it that way? 


---


#### 00:52:03.528

Or is that, that wasn't where you were going. So I'm wondering if that seems more far-fetched to you. I think that seems more far-fetched to me just because the dimensionality of the problem is very large in terms of complexity. And it seems to me that AlphaFold was successful only once we had enough structural data, enough data actually leaking sequence to structure. And it's a relatively well-defined problem, I suppose you might say. There's only 20 amino acids. We know what the string is. How is it going to fold? And it looks a lot like the models aren't particularly good at,   
(00:52:38.978) ~~they're not telling you,~~(00:52:39.938)  
they don't understand how it folds. They can reliably predict what it's probably gonna fold into, which are two different things. 


---


#### 00:52:47.744

So if you muck with something on the folding path, then they may or may not detect it, depending on whether the way that you mucked with it was out of training distribution or not. So   
(00:53:00.132) ~~I guess~~(00:53:00.351)  
I'm a little bit more skeptical that the newer attempts to just throw all of the data from many different, quite disparate from one another, problem categories in biology into one model and having it just come up with solutions. I'm less bullish on that. It absolutely support people doing it. It's just, I wouldn't hold my breath. It seems like the dimensionality of the problem is too great and we don't have enough data. So let me understand that a little bit. better. 


---


#### 00:53:30.599

When I think of Evo, I put it on like a GPT-2 scale and already it seems to do these things where,   
(00:53:38.403) ~~you know,~~(00:53:39.623)  
the one that stands out to me the most is the gene essentiality scores where, and again, correct me if I have any subtle aspects of this wrong, but basically it's if you change a sequence and then look at the predictions downstream, if those predictions go to high perplexity, essentially, if the predictions unravel, that's an indication that the change that you made is consequential. Because now, in the presence of that change, the model can no longer have any confidence of what would come next, right? It's signaling to you that it's out of distribution. 


---


#### 00:54:12.262

Whereas if you make a change and the predictions continue to be high confidence, then it's, well, that didn't matter so much. And so that sort of change is tolerated. And this, if I understand correctly, has gotten at, or maybe even has fully achieved state of the art for predicting which genes will or won't be subject to mutations. If that's right,   
(00:54:31.079) ~~and we're at GPT-2, and this was like a 7 billion parameter model with 300 billion tokens, seems is the dementia~~(00:54:37.934)  
obviously it's super complicated but is the how would you think about the relative complexity of biology versus all of society all of the languages all of the subjects like gpt4 knows like the scores of individual sporting events from the last hundred years of sporting events it seems like there's a lot of space in those parameters and that's what's rumored to be 10 trillion tokens of language data, certainly we have 10 trillion. 


---


#### 00:55:04.266

We could get 10 trillion tokens of all sorts of biological and health data, right? So what's the difference? It's that your essentiality problem is comparatively well-defined and we have a lot of data on it just because the genome, again, tells you what we now know most of what the genes are. Automated gene annotation has advanced quite far. and we have enough genomes that then we know which combinations of genes are present, and obviously those organisms are success cases and that they're viable. And so that's exactly the kind of data that you would expect to suffice for predicting gene essentiality, which is not remotely the same thing as understanding how changing a particular gene is going to change the function of the resulting cell. 


---


#### 00:55:50.242

It doesn't tell you what it's gonna interact with, it's different. It just tells you is it important or not based on the presence absence of that gene or set of genes in this data set of all of the things that we've sequenced. So essentially   
(00:56:05.927) ~~what I guess~~(00:56:06.447)  
my point is, their test for Evo is like the equivalent of an AlphaFold test. It's the case where they have the most data that is directly relevant to the thing that they're testing. And so I'm, OK, yeah, sure, it can do that.   
(00:56:19.271) ~~And so then,~~(00:56:19.672)  
so I'm not surprised. That is a very well-defined problem. That is not the same thing as predicting how some change is going to interact with the immune system, let alone If you could predict the change in phenotype of the organism, how would that change its evolutionary fitness and interactions with other species in a given ecosystem or across ecosystems? the relevant gene flow patterns. 


---


#### 00:56:41.251

It's just that there's so many different additional variables involved beyond gene essentiality that I view that as a useful tool for certainly efforts to try to go simple, build something much more simple from the ground up, the reduced genome or minimal cells. I think it'll be incredibly useful for doing that and accelerating the bottom-up path. So I think it's great I'm just skeptical that the dimensionality of the problem doesn't explode well beyond the data that we have available. And I guess I justify that on the basis of some of our own efforts, and those from recent work by Kevin Yang and others, that just show that, look, you can train ESM3 with even more parameters, and it just doesn't buy you very much. 


---


#### 00:57:29.503

Whereas if you're trying to predict the function of a protein, you give it exponentially more data, you get hyper exponentially better predictions. More parameters right now doesn't buy you much in that particular problem class, which is not far away from the well-defined nature because we're talking sequence to function directly. and there you give it more data and you get   
(00:57:56.041) ~~much, much,~~(00:57:56.362)  
much better results, whereas more parameters doesn't buy you much. Now, that's a slender read to be confident in. I'm not particularly confident in this, but I've been burned enough times that I'm reasonably skeptical that just pouring all of our data into a single model is going to allow you to predict things beyond the relatively narrowly well-defined cases that are most directly informed by the training data. 


---


#### 00:58:23.391

I'm just not optimistic. Yeah. So I guess, how far do you think that is likely to go? When we look at   
(00:58:28.695) ~~like~~ (00:58:28.795)  
a GPT-4, it can do these sort of bizarre things that are   
(00:58:33.956) ~~like,~~ (00:58:34.137)  
not in its training data, right? A Shakespearean sonnet about a soccer game or whatever. And then there are also obviously some like embarrassing mistakes that it makes. And then there are also things that it just   
(00:58:47.599) ~~like~~ (00:58:47.739)  
definitely can't do, resolve the remaining mysteries in the standard model of physics or whatever. So you think that there's like a similar, if we were to take Evo and imagine Evo 4, and imagine however many parameters, lots more data, maybe different like levels of data. 


---


#### 00:59:04.737

Because I think right now it's just all genetics, but you could add on the proteomics and ultimately up to high order descriptions of like fitness or blood pressure, whatever. If you did all that, do you think you would end up in a similar place to GPT-4 where You could do these like counterfactual experiments within at least some domain in biology, or you just feel like this is just   
(00:59:30.797) ~~like~~ (00:59:30.956)  
way too speculative to even anticipate what that might look like. I'm sure you could in some domains in the better defined domains. Yes. And as you feed more and more data into it, don't get me wrong. I think this is the path to the solution. It's just, 


---


#### 00:59:43.860

I think there's going to be a whole lot more data required, which is why we need the lab automation to run all of those experiments in very high throughput. a key part is going to be, do we actually need something like Bayesian models to tell us what kinds of data we need? I don't know. I would love to see more work in that direction. I think it's overly optimistic to assume we have anywhere near enough data now, but we will generate that data,   
(01:00:07.806) ~~right?~~ (01:00:07.967)  
That is part of the pathway, building better tools and platforms to generate better data and more relevant data informed increasingly by the models   
(01:00:15.592) ~~that we're using to train,~~(01:00:16.833)  
that we're training on all of that data. 


---


#### 01:00:19.155

That is the path to the solution. I just am skeptical that we have enough data now for something like Evo to give you much of use in anything that isn't very well defined. Not to be wrong. In terms of the data that we have or don't have, Do you think that, let's say something like the UK National Health Service got on board with this and said, okay, we're going to muster all of our historical treasure trove of data to put into a mega project like this.   
(01:00:47.820) ~~Do you think if that sort of thing were to happen, then we would be like, would we have the data or would we be like close to having the data?~~(01:00:54.724)  



---


#### 01:00:55.246

Or is it a different kind of data entirely that we need? To me, that's a different kind of data. That's the data that is very relevant to ML-guided medicine that we should absolutely be doing and figuring out how to deal with the privacy concerns and all that jazz. And there's great people working on that, and I'm confident that we'll solve it. But that's more of a medical physiological level than the kind of molecular programming that I'm talking about in terms of the actual underpinnings of biology. You don't necessarily need the underpinnings in order to make dramatic advances in health, for example, in personalized medicine. That's on a different level. And that's a level that I don't have enough expertise to comment in any kind of well-informed manner. 


---


#### 01:01:38.559

That's just not my area of specialty. It seems like they are a pincer movement on what people really want, right? Like you want a, and I understand you want this for yourself, right? And if it's working well enough for you, then I'm sure I'll want it for myself too. The idea that   
(01:01:53.768) ~~like~~ (01:01:53.969)  
we would modify our own existing cells to be reprogrammed. It seems like there's this top-down medicine and then you're coming at it from   
(01:02:04.534) ~~like~~ (01:02:04.655)  
the very low level, bottom-up programming. Maybe that's like where we meet in the middle? Is that kind of the mental model of this? So let's use a particular technology as an example that has the most obvious implications there. 


---


#### 01:02:19.400

Research moving towards an artificial womb, say. Naturally, neonatology is getting better and better at keeping premature babies alive at earlier and earlier ages with better and better outcomes. And so that's your top-down marching backwards. And then at the same time, there's a lot of research on how to mimic the early conditions of the womb and develop embryos forwards, obviously most advanced in animals due to ethical concerns, but we're getting better and better at keeping those embryonic fetal lambs alive later and later in gestation equivalent. And eventually the two are going to meet and then you'll be able to do the whole thing in vitro in animals. And then once we're good enough in animals and we've done non-human primates, then we'll do non-human primates. 


---


#### 01:03:03.907

And then eventually we'll be able to do it in humans. And   
(01:03:06.309) ~~if you can grow~~(01:03:06.849)  
If you can grow a human body, a whole human body, then you'll probably be able to do pieces of a human body and there's your replacement organs. And   
(01:03:16.385) ~~I'm,~~ (01:03:16.525)  
you don't necessarily need to solve the whole ball game in order to mostly defeat aging. If can replace all of your organs when they start to give out the brains, the hard one, but I'm not even confident that you need to understand how the brain works in order to meaningfully augment it.   
(01:03:33.936) ~~Right.~~ (01:03:34.137)  
We know that our brains can. do a fairly good job of adapting when faced with some sort of insult. 


---


#### 01:03:43.351

If you, for example, lose your ability to see, then your brain will begin using what was formerly your visual cortex for other purposes. And kids' brains do this even better. So we can use biotech to restore that kind of childlike plasticity. And then I would bet that if you can establish a high enough bandwidth connection between your brain and simulated neurons, computationally simulated neurons, such that the brain can talk to them and reprogram them as though it were part of itself, you can get that language working. And again, you don't have to understand it. You just have to explore and figure it out so that it works without the understanding that I expect your brain would begin making use of those simulated neurons as part of itself. 


---


#### 01:04:24.889

Certainly if you enhance the biological side with the plasticity enhancing biotech and then use our best molecular machines for signal transduction, Ed Boyden's work and Adam Marblestone have a great paper on what are the physical limits of information transfer. across the skull and what are the means by which we should be exploring, which is great technology development tracking. I'd love to see more of that kind of work. But I suspect you get the connection good enough, then we can meaningfully augment ourselves with externally provided computational resources without understanding how our brains work. I don't think you need to understand the whole system in order to solve a whole lot of problems. And I guess that's where I'm a techno-optimist because the world is terrible in a whole lot of ways, but it used to be a lot worse. 


---


#### 01:05:11.762

And we've been given this tremendous gift in the form of a much better world. And we have the chance to make it even better. And the question is, how can we do that wisely? Because as you put it, it's a bit of a tightrope. You could argue that life is a tightrope biologically between aging and cancer. And   
(01:05:30.692) ~~I think~~(01:05:30.833)  
it's a similar sort of thing with technology development, which is why I just tend to come down on the side of increasingly powerful technology in the hands of fallible humans. We know that some humans will do things that harm others for reasons of mental illness, and in some very rare cases, maliciousness. This happens at a finite rate. 


---


#### 01:05:51.637

Once technology becomes powerful enough, if it is offense dominant, this could go very badly. One of the reasons why I'm hopeful about AI is because it seems a whole lot more feasible to ensure that all AI systems are reliable and responsible and trustworthy than it is to make sure that all humans are, which is why I think AI is part of the solution to your tightrope. we may not be wise enough, we may not be well balanced enough to walk that tightrope all the way to the end ourselves, because as our power grows, and we need that power,   
(01:06:24.284) ~~right?~~ (01:06:24.483)  
Civilization is not sustainable today. We need future advances in order to continue and even just, or even just to stay where we are in our much improved world relative to the past. 


---


#### 01:06:36.766

So we need more advances, but we need that power But again, if it's offense dominant, if you give too many people a red button that would actually bring down civilization, someone's going to push it eventually. So don't give people who might push the button those buttons. ensure that you have defenses in place that means the button won't be effective before you hand out buttons like that to fallible humans. AI systems, I hope, will one day be trustworthy enough that they can have access to all of the red buttons because they wouldn't use them. We've certainly got a ways to go there. We do, but again, think about humans and how reliable all humans are, and we have learned enough about how viruses work to make them from scratch. 


---


#### 01:07:25.599

So the obvious one is that I say we should not, in fact, identify pandemic-capable viruses publicly and share their genome sequences and protocols for making them because we can't yet defend against pandemics, which means the risk of someone deciding to cause a pandemic is too high. We know that there are figures in history Notably, Tsuichi Endo, folks like the Unabomber, plausibly would have done it. Because the Unabomber is a nightmare for me personally, in that the man had a grudge against biotechnology, in particular. He believed that, quote, the immense power of biotechnology, end quote, would be used to warp humans away from our ancestral state in service of the demands of our culture and the market. 


---


#### 01:08:11.257

And this would be an offense to human dignity, and that technology more broadly is making us miserable because we're moving away from the ancestral state. And he thought this was bad, and we should all go back to being hunter-gatherers. But biotech was the worst. It was the perversion of human dignity that we would use to shape our children into being different.   
(01:08:26.545) ~~Well,~~ (01:08:26.725)  
I happen to think that just like we've made a better world from the past, we can probably make our children better people than they would otherwise have been. I guess I'm an optimist in the Enlightenment spirit. But Kaczynski was a genius. He was a Berkeley mathematics professor before he decided to retire to the woods and embark on a bombing campaign to get his ideas out there. 


---


#### 01:08:49.149

And if what he wanted to do was to blacken the name of biotechnology and ensure that we didn't go down that route, would he have been smart enough if the tools had existed in his day to deliberately cause a pandemic in order to spark that backlash that would preclude us from using biotech to reshape who we are, to try to become people who are better than we were born to be, I think he plausibly would have. And I don't want people like him to have the tools to derail the shining path that awaits us if we can actually walk that tightrope far enough. I feel like we're going to need a part two here because there's still a lot of detail on how to walk the tightrope that I would really love to get your take on. 


---


#### 01:09:31.426

I know that probably can't be today or this week, but I guess you've been involved in a number of interesting things in terms of pandemic preparedness, defenses, in terms of creating this program called Secure DNA, which allows DNA synthesis companies to screen their customer orders against known threats. Obviously, you have a command of all this material when it comes to things like Evo and how much we should extrapolate from where we currently are. How do you see that balance playing out in biology? And then maybe I'll ask one more kind of super big picture question about AI after that. But we've got Evo versus secure DNA is maybe one way to think about it, right? 


---


#### 01:10:18.713

There's all this generative stuff, but then there's the detection. Who's out of domain for who? Is the secure DNA tech going to be able to detect novel threats coming out of things like Evo? And how should we generally be thinking about how to stay on the right side of falling off the tightrope?   
(01:10:36.145) ~~I suppose~~(01:10:36.706)  
I could just jump to the end and say,   
(01:10:39.546) ~~look,~~ (01:10:39.787)  
I don't know when we will learn to cause pandemics. I don't know when we will learn to cause pandemic-like events that are worse than pandemics, because after all, nature is never trying to kill us. Nature is not trying to bring down civilization. It seems to me that a human could plausibly do worse than the best that nature could do when it comes to destruction, just because the human would be trying, would be aware of our defenses. 


---


#### 01:11:02.045

I don't know when that's gonna become possible, but given that COVID smacked us pretty hard and that was wherever it came from, I don't think that's actually very important because we know pandemics can come from natural spillover from animals and   
(01:11:16.770) ~~we know that they can come from,~~(01:11:18.850)  
we know that laboratory acquired infections are a thing. So we need to take steps to prevent both. and also the deliberate side. Right now, we're just not ready for a really bad pandemic. A sufficiently bad pandemic,   
(01:11:33.203) ~~judging by those that have occurred,~~(01:11:35.164)  
particularly in other species, would threaten the stability of civilization. I could imagine it getting very bad. And I would prefer that we not go there until we have defenses in place. 


---


#### 01:11:47.613

And if we assume the adversary is very good, it's generally a bad idea to let the adversary inject information packets into critical systems. And my body is a critical system. So I really don't want to get infected in the first place. I think it's safest just to assume that you don't want to get infected if the adversary is any good. And that's totally possible with current technology. This is the defend aspect. We can get to a world where we have germicidal lights that block transmission of ordinary stuff on a day-to-day basis that can be turned on in the higher intensity in the event of a crisis, just inactivate anything transmitted through the air or on surfaces exposed to the light. 


---


#### 01:12:25.971

And in an emergency, we know how to build powered air purifying respirators that perfectly protect us from the transmission of pretty much anything. all the hazmat suits for Ebola   
(01:12:35.543) ~~and stuff,~~(01:12:36.265)  
things like Ebola aren't really the threat. That's just not the way transmission is gonna work. So we basically have all the technology, we're just not prepared logistically. We don't have enough suits, we don't have the detection systems, we aren't prepared to know when to turn it on. We could map spread so that everyone could make their own decisions regarding how much risk they're willing to take. Our phones are good enough now, they weren't quite during COVID. We could do it. We could flip it around and say, look, here's your social graph of the people that you interact with, and the people that interact with them, and the people that interact with them, and here's how many people have been infected at each level. 


---


#### 01:13:14.885

You decide. Things like that all put together,   
(01:13:16.926) ~~I think,~~(01:13:17.365)  
could ensure that pandemics could not threaten us to any appreciable level. And so my hope is just that we will actually make those investments, which are quite small relative to investments we make to defend against other human adversaries attacking in other ways. And then we can learn how to cause pandemics. Would not be harmful because the red button would not work anymore. So my question is, how can we use AI as the platform that accelerates technology more than any other? to preferentially advance the development of defenses. I want better germicidal lights. I want cheaper, more comfortable, classier PPE. And I want early warning systems that can reliably detect anything like a new HIV, let alone a faster spreading, but time-delayed stealth pandemic type thing in place so that we always know everything, all biological things that are spreading exponentially. 


---


#### 01:14:14.275

I want us to see them all coming. And if we get to that world, then we're pretty robust against anything pandemic class. And then I'm just not super concerned about distributing the red buttons because they wouldn't work anymore. And I think that's just an example of what we need to do in technology more broadly. We need to ensure that we have the defenses in place first. And this is hard because I don't know when we're gonna access that red button capability. And there's a lot of disagreement over how accessible it really would be. There's a huge difference, for example, between making 1918 influenza from synthetic DNA, which is unfortunately not very hard, and making smallpox from synthetic DNA. 


---


#### 01:14:55.211

What else can we afford? Yeah. Yeah. I know we're just about out of time for today. I am struck that the things that you're recommending here are seemingly common sense, might be a little bit of a stretch, especially since we just went through a pandemic to say, Hey, maybe we should stockpile some respirators and get some antiviral lights going   
(01:15:17.636) ~~that~~ (01:15:17.777)  
that seems like very   
(01:15:20.457) ~~almost~~ (01:15:20.679)  
inarguable it also strikes me that there's not any constituency with any sort of vested interest against that. Maybe the convention, the makers of like conventional light bulbs or something. Broadly, it would seem like there's nobody who's got it in their interest to stop that sort of thing. This makes me, and yet we're not really doing it, right? 


---


#### 01:15:40.199

Maybe a little bit here and there, but it seems like we're not really answering the bell on this challenge. I wonder if there's anything that you could say or any wisdom you could impart to the folks that are working on this on the AI level, where there's seemingly a lot more complicated dynamics, including vested interests in certain ways that don't want certain frictions.   
(01:16:03.796) ~~I don't know.~~(01:16:04.157)  
This is tough. Is there anything that we can learn? It's tough because it's not really worked, right? You've got the most common sense knockdown argument in the history of the world, and yet we can't get relatively basic preparedness measures enacted. Is that a right characterization? And if so, what does that suggest to you for the AI side of experts? 


---


#### 01:16:26.533

I wish I could help because it seems to me that AI is in fact a thornier problem in terms of incentives. But it's also one where at least the rewards are worth it there. If you get it right, then you really get something. Whereas you learn how to make pandemics, like that doesn't even tell you how to defend against them reliably. It just tells you how to make them. Defending is a whole separate problem.   
(01:16:48.283) ~~I guess the only thing that,~~(01:16:50.725)  
so I'm not even sure what the parallels are.   
(01:16:53.087) ~~I'm sorry,~~(01:16:53.427)  
I wish I could be more helpful. I don't have that kind of wisdom. What I have noticed is that public health is not gonna cut it. 


---


#### 01:17:00.953

We just aren't willing to invest to defend ourselves against natural accidental pandemics. We spend a whole lot more money when we're afraid that some human is going to use weapons against us. And so my best hope for defending against pandemics is to point out that we will learn to cause them, that they are generally not in the interest of nation states, which is again, an area where bio is easier. US and China have some very legitimate reasons to differ on AI in terms of strategic interests, but neither of them has any interest whatsoever in making pandemics accessible to lots of people, and every interest in cooperating to prevent that from happening. and broadly build defenses such that we can squelch outbreaks before they spread widely. 


---


#### 01:17:47.796

Nations broadly share this. It's just an easier problem across the board. But I do think we need to frame it as a problem of misuse. And it may be that the same lesson holds for AI. When you look at the executive order, that was more progress than we've ever gotten before when it comes to actually doing something to reduce risks from bio, because the executive order was all about AI reporting, and it actually required some level of DNA synthesis screening, however roundabout, for the first time. Any nation, anywhere, had actually done that. And why? Because people were worried about AI telling lots of people how to cause things like pandemics. And with synthetic DNA not being screened, it would just be a little bit too easy. 


---


#### 01:18:41.082

So that's the obvious place to start. And so they started there. So maybe by having bio as the concrete thing that can go wrong misuse-wise, that's just easier to conceptualize. than it is, it's just easier to conceptualize, I think, than risks of loss of control to people. It's just easier to unite around, look, we expect AI to be better   
(01:19:04.172) ~~at me,~~(01:19:04.512)  
better, we expect AI systems to eventually be better than I am at engineering bio. And that means they will have access to pandemic class agents, and they will be able to help others acquire pandemic class agents. I don't know when this will happen, But the kind of AI systems that everyone in the field wants to build must be able to do that because we want them to solve aging for us. 


---


#### 01:19:27.469

That means they need to solve biology and engineering biology. So maybe we can use bio as an example of how we need to build our defenses first and think about access because I'm a huge open source fan. I run Linux. My lab develops open source software for lab automation. But that lab automation software is not going to disseminate access to red buttons. And again, I don't know when the AI systems might start doing that. But somewhere along the line, I think we can all agree that they would be able to do that. And that we should probably ensure we have those defenses in place first. And if we can succeed, then my hope is that we will have those defenses in place before our best systems can do that kind of thing. 


---


#### 01:20:11.168

I think there is something really interesting and compelling there about uniting around misuse framing. I've noticed that as a soft trend in my own conversations about this. And it's interesting also to even speculate about why that would be. We've been the dominant species for a while. Certainly we've been more threatened by each other than we have been by nature   
(01:20:35.394) ~~through~~ (01:20:35.634)  
from generation to generation for most of our recent history. Although there have been some notable punches from nature, but it's also a superset of the same risks, right? Or maybe that's probably too precise of language, but it does seem to be like, if you're not sold on the possibility that either another pandemic would rise naturally or that the AI could get out of control on its own, 


---


#### 01:21:01.550

Then certainly it's like a little easier to imagine that a bad person would come along and use a powerful system because we certainly see plenty of existence proofs of that sort of thing. And then it's like, how much are you really leaving if you're worried about loss of control? but you focus on AI plus human loss of control, does that really hurt you too much in the even longer tail risk of loss of control of AI systems? Certainly in some ways it probably does, but I think it definitely could make a lot of sense. That's a place to come together. Sounds like you got to get on a call. Yes, I'm afraid so. All right. 


---


#### 01:21:40.180

Yeah, well, this has been fantastic. I could listen to this all day. And I would love to do a part two at some point. Sure. But for now, I will just say thank you for your time and sharing so much of your history. And I think even a little wisdom there at the end. Thank you for being part of the revolution. Thank you, Nathan. 


---



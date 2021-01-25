---
title: Virtual CNWW
subtitle: Traveling virtually through complex networks in the winter
author: Jeremy
tags: [science, workshop, networks, essay, worldline]
permalink: /virtual-cnww
date: 2021-01-25
---

If you want to learn a topic today, the resources are much more plentiful than even a few decades ago. The internet has given us wonderful resources to learn from, including some which leverage internet technologies to provide animations and teach topics in a [much more interactive way](https://distill.pub/2020/communicating-with-interactive-articles/). This is particularly true for mathematics and physics, which have been entrenched in dry textbooks that are a chore to read[^1] for much too long.

The tools are there, and access isn’t unlimited, but the barrier has been lowered. However, when it comes to doing science and mathematics, there’s more than just the sheer knowledge. If you want to enjoy your time as a scientist, building up a community of people you can throw ideas around with and trust is key. As I wrote back in my [“PSIon” essay](https://cotejer.github.io/psion), the most important thing I got from my experience as a master’s student at Perimeter Institute was the cohort of people. The friends I made were worth more than any other part. Sure, I learned a lot of physics, but the experience was made all the better by the friends I made.

---

I’ve written about my experience as a physicist, as well as different ideas within the [world of quantum](https://cotejer.github.io/pick-a-state). But I’m not married to physics. While it’s the discipline I’ve chosen to focus on for now, I’m fascinated by many questions in science. The toolkit of physics is one I like, but I thought it would be a shame to go through my PhD focusing exclusively on quantum theory and never venturing into any other areas. Even if they don’t serve my “primary” direction, dipping my toes into other fields provides a way to gain a new perspective, learn of new big things happening in science, and frankly get out of the thought bubble of a field. When I was at Perimeter Institute, it was a lovely place to think about physics, but this also meant a lot of the topics were the the same. I’d hear constant talk about quantum theory, condensed matter, mathematical physics, and cosmology and astrophysics. All fascinating topics, but clearly not all there is to know about science.

And so it was with this motivation that I decided to apply to the [Complex Networks Winter Workshop](https://vermontcomplexsystems.org/events/cnww/)[^2], which is a joint effort by the [University of Vermont Complex Systems Center](https://vermontcomplexsystems.org/) and the [Sentinel North program from the Université de Laval](https://sentinelnorth.ulaval.ca/en). For this installment, the workshop was online, but the theme was the same: two weeks of exploratory projects on anything to do with networks and complex systems.

![](https://vermontcomplexsystems.org/events/cnww/files/stacks-image-c8a0f4c-450x388@2x.png)

If you’re reading this and wondering, “What on Earth is a quantum theory student like yourself doing in a workshop like *that*?”, well, I asked myself the same question. I wasn’t sure if I would be able to even contribute anything. The experience I had with anything networks-related was limited to two things: a graph theory course I took during my undergraduate degree, and a bit of work on tensor networks that I began last semester in my research. But apart from that, I had basically no experience.

In fact, I suspect I felt like my friend did when we started studying at Perimeter Institute together last year. It was a theoretical physics program, but he was coming into it with an engineering background. I imagine he must have had similar thoughts, though probably amplified since the program was a year long instead of only two weeks. (And if he could do it, I told myself that I could too.)

Nonetheless, if I want to say that I’m a scientist who keeps an open mind and looks at a bunch of areas, I couldn’t exactly say no to this chance. So, while feeling a bit out of place, I signed up for the workshop and got myself ready for two weeks of a lot of learning.

## Projects

The main part of CNWW is the projects. This year, the projects included many themes: renormalization of networks, animal networks, spread of contagion, roads, skiing (this one was mine), financial networks, soccer networks, political networks, collaboration networks, and social networks. Seriously, the sky was the limit with the projects.

The first week is one of plenty of brainstorming to get an idea and form a group. This meant hopping on calls with many people to get a flavour of what was going on, and finding something that struck your fancy.

As a runner and general outdoor enthusiast myself, I was drawn to the sport-oriented projects. My goal was also to do something quite different than what I’ve been looking at during my PhD, so choosing to look at skiing was a great fit.

Because there isn’t a ton of time, you can’t expect to get a super-ambitious project done. I went in without too many expectations. In fact, it was the same attitude I entered the Winter School during my year at PSI with: learn some new things, enjoy the time, and don’t care too much about turning a project into an instant research paper. I find that this is a healthy attitude for a short workshop like this one, particularly since it was way outside of my comfort zone.

Then, two weeks after the start of CNWW, we had a marathon Zoom session on Saturday to listen to everyone present their projects.

What I was struck by was the energy that accompanied each project. Instead of focusing on having perfect analyses, the projects were more exploratory, trying to tease apart questions that came up during the two weeks. There was an air of “lightness” to the day that was much different than giving a presentation where it feels like everyone is judging you. Here, it really was a chance to get back into doing science for the reason most of us started out with: because it’s fun. This was something the mentors[^3] for CNWW repeated to us, and I definitely noticed it throughout the two weeks.

It was also very collaborative. Since people weren’t all experts in their projects, it was easy to offer feedback and ask questions that poked at new directions. Even I found myself asking questions at times, despite having no underlying baggage of knowledge to lean on. I’d say that the atmosphere was always inviting, and despite being an outsider to the field, I didn’t feel like I was falling behind and completely confused at all moments. That in itself was great.

## Lessons

What did I learn at CNWW?

The most prominent thought I was left with is that *getting* data to answer a question is so tricky. It left me with an appreciation of collecting data and cleaning it. It’s great to just say, “Let’s use some data on X and build a network to analyze!”, but doing the work of massaging that data into forms you can work with (and that make sense for the problem!) takes a lot of time.

The other aspect is linking data to your questions. During CNWW, I had so many questions posed by and to me, and this left me with a dizzying array of directions to pursue. The catch is that actually *answering* a question with data is not an easy matter! In the “real world”, data doesn’t point only towards answering a particular question, and so tradeoffs have to be made.

I think of this mostly in the context of how I work as a theoretical physicist. I work with simulations, which is a roundabout way of saying that I craft models that conform *specifically* to the questions that I want to answer. This means there’s little ambiguity between the data I receive and the analysis I can do. The data is built to answer my question.

But during CNWW, I developed an appreciation for those that tried to take a networks approach to systems in the world. Because a network is an abstract object, you have to find a way to layer it on top of the system you’re interested in. But just like you can’t take a sphere and flatten it out on the ground without creating bumps, you lose something when you go from your system to a network. The goal is always to minimize that loss, but you have to be aware of that it rarely goes to zero. Losing something in translation is common.

This question comes to the fore as soon as you start asking what the network representation of your system even *is*. A graph is a fairly simple mathematical object: a set of edges and nodes. But this simplicity means you’re making tradeoffs each time you model a system in the world as a network. Unless you’re working on abstract computer science problems like myself where the graph *is* the system, you need to worry about how this embedding affects your ability to answer the questions you want.

The other lesson I learned was that there are a *lot* of questions you can ask, but really honing in on them and making them specific is tricky. This is a variant of something I encountered while working on some machine learning projects. When you train your model, there are various knobs that the algorithm doesn’t adjust on its own. These are called “hyperparameters”, and they are set by you, the person designing the model. So how do you decide? Well… it’s not always transparent. You can try an exhaustive search over the possible values, but because they are often continuous and there are several of them, the multiplication rule of combinatorics isn’t in your favour. And that’s not even looking at strategies where some of these hyperparameters *change* as a function of the training time!

I encountered  this with the people studying real life networks. Yes, they could map their system onto a network and answer questions about the dynamics, but whose to say that there aren’t outside factors which the network doesn’t consider? And what about causality? These are all thorny questions, but nobody at CNWW hid from them. These are limitations of the field, and I did like the candor of admitting this.

## Lectures

In addition to the projects, the mentors at CNWW gave lectures throughout the two weeks. These were on a bunch of topics, since the mentors all study different niches of network science. These ranged from animal populations to infectious disease to human relationships to what it means to even *have* a network. The diversity was something I really enjoyed, and it meant that I could get a taste of many different areas of network science.

I probably enjoyed those on the theory of networks the most, given by [James Bagrow](https://bagrow.com/pdf/bagrow_working-with-network-data-2021.pdf), [Jean-Gabrielle Young](https://www.jgyoung.ca/), and [Dan Larremore](https://larremorelab.github.io/). These really got to the heart of networks for me. The applied networks presentations were really good too, though admittedly some hit the mark of my interests more than others.

## Being Virtual and Doing Science

Like so many things today, CNWW was virtual. This meant we had many calls, and long sessions working with others on our projects.

Not only was this my first workshop/conference, it was also one of the few online events I’ve done (since I don’t take classes anymore as a PhD student). So I didn’t know what to expect going into this, but on the whole I think it went well. There’s an adjustment to be made with virtual events, but I think the work done can be just as good.

My one point of comparison is with the Winter School I participated in during PSI. There, we spent a week at a lodge doing intense work during the day. There were similar group projects, and I found that virtual CNWW was really good for getting people to work together. Despite some awkwardness of meeting people online, everyone was excited to learn and do some network science.

I think the biggest thing you need in *any* sort of workshop is enrollment: How invested are people? I think that if you have the investment from everyone, it doesn’t matter if the workshop is online or in-person. The key is to get people to show up and willing to put in the work, and that was something I felt for all of CNWW.

The effort each person put into the workshop really shone on the last day, where each group presented their work. It was nice to get a feel for what everyone else was doing. In an online setting, you don’t have the ease of bumping into others, so I was more or less in the dark about the other projects until the end.

Moving forward, I really think this kind of format can work well. Like I said, it requires investment on the part of everyone. If people don’t show up and put in the effort, any workshop will fail. But with CNWW, everyone was bursting with energy to go.

CNWW could have been devoid of energy. This is, unfortunately, the feeling I get during so many online meetings. We try to shoehorn an in-person interaction into the online realm and things go badly. But here, people were always energetic and ready to talk science. Each time I logged on to a call, instead of feeling a sense of, “This is going to be a boring meeting”, I felt excited for what’s next. I think part of this is because *everything* was basically new to me, but I also think the organizers of CNWW did a great job of building this atmosphere directly into the two weeks. I’m fairly sure this wouldn’t just happen organically.

It also helped that there were several cultural activities throughout the two weeks. Each morning and evening had a happy hour where different themes were presented. There was also a presentation on ice canoeing, as well as a few other challenges to the add to the workshop. I thought these were nice additions, and did make it feel much more than “just” a science workshop.

---

Despite this being my first time learning about network science, I’m really hoping it won’t be the last. The experience of the workshop itself was great, and it’s one I’ll remember. In particular, I want to thank the two organizers who made the workshop happen: [Juniper Lovato](https://juniperlovato.com/) and [Marie-France Gévry](https://twitter.com/MFGevry). Another thank you to those who showed up every day to lead the meetings, including [Antoine Allard](https://antoineallard.github.io/), [Laurent Hébert-Dufresne](https://laurenthebertdufresne.github.io/), and [Jean-Gabriel Young](https://www.jgyoung.ca/). The workshop went so well *because* of the time you all put into it before CNWW even started, and throughout the two weeks. I think I can speak for all of the participants in saying we really appreciated it.

When you’re online, it’s easy to get lost and bogged down by the tools and the various platforms needed to connect to everyone. For CNWW, the technologies used were Zoom, Slack, and Whereby, as well as a central website that had everything presented in an easy-to-see way. It sounds silly, but these details really do matter, and setting them up takes time. I think the team here did a great job at making sure that everything went on without much difficulty (even when Slack went down worldwide on Day One of CNWW!).

As for myself, I’m hoping to continue working on the project I started with my team. Two weeks is only enough to start figuring out what kind of questions to ask, so there’s a lot more to go. However, like I mentioned at the beginning, the point of the workshop for me was always about gaining new perspectives in science and meeting other scientists. And in that regard, I absolutely succeeded.

## References

1. The team behind CNWW was no stranger to virtual conferences either. In fact, if you want to read more, Juniper Lovato has [written a piece on organizing virtual science conferences](https://medium.com/@juniper.lovato/a-how-to-reflections-on-planning-virtual-science-conferences-eeb754ed404b), so you may want to check out that essay if you’re interested in the details.

## Endnotes

[^1]: Though there *are* some books which are a delight to read. I’m not against the medium, but I am against limiting ourselves to it.
[^2]: The workshop is called CNWW, but because of the Québec/Canada connection (and, let’s face it, the tendency of scientists to give groan-inducing acronyms and names to their projects), it’s pronounced “canoe”.
[^3]: While there were mentors and participants at CNWW, the distinction is meant to be blurry. What I mean by this is that the mentors would often help (and present) projects, giving their time just like the participants to work on them. In that regard, the workshop was very collaborative. There wasn’t much of a top-down structure, but the mentors did provide times to chat on ideas, and they gave lectures.
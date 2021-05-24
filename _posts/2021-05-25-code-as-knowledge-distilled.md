---
title: Code as Knowledge Distilled
subtitle: How confident are you that you really know something?
author: Jeremy
tags: [essay, worldline, code, science, research]
permalink: /code-as-knowledge-distilled
date: 2021-05-25
---

When I was an undergraduate, I did my best to stay away from a computer to do physics. I saw myself as a theorist, and in my head, a good theorist could get everything they wanted done with pencil and paper. I remember one particularly vivid time that I used a computer algebra system to calculate Riemann tensors for my research in gravitation theory, and I hated dealing with the complexity of the program. It wasn’t easy to work with, the answers were often garbled and not simplified, and it almost felt like I was wasting more time using a computer.

During my time at [Perimeter Institute](https://cotejer.github.io/psion), I got more involved with code and programming physics simulations. I did my project on machine learning with physics, I worked on numerical simulations for a [variational quantum eigensolver](https://www.mustythoughts.com/variational-quantum-eigensolver-explained), and I spent more time in front of a text editor.

Slowly, my day-to-day life as a physicist has been evolving.

I used to spend my days with paper and pencil, working through long equations. I still do that from time to time, but my primary playground has leapt from paper to the text editor. Code has been my primary tool during these first nine months of my PhD. I never would have predicted this at the end of my undergraduate degree, and yet here I am, programming each day, creating my own experiments on my computer to test ideas.

During the many days at the text editor, conceiving of and launching experiments, I’ve learned many lessons about what it means to program in science. There are two main benefits you gain from programming in your research. The first is that you learn how to be *explicit*, and the second is that you gain a deep understanding of all the parts that go on “under the hood”. 

## Science Made Explicit

**The number one reward for learning how to work with code in your scientific work is that it forces you to be explicit about what you’re doing.** There’s no hiding when you’re programming. Either you understand what you’re doing and the code runs as you expect, or something is still opaque and your code breaks[^1].

Imagine you want to run a simulation where you generate random samples and then have them evolve. Before you even get to programming the dynamics, you’re faced with a question: What does “random” mean”? It’s a word we say often, but a simulation requires more precision. Do you mean uniformly random (think of a fair die)? Do you mean a Gaussian distribution? Poisson? If there are repeated draws for your simulation, do they occur with or without replacement?

Quickly, the word “random” ends up having a lot of baggage.

This is the nature of programming. When writing code, you cannot afford to be sloppy or vague with your words. Or you can, but then your code often won’t run properly (and *knowing* that something went wrong is an art in and of itself!).

Programming requires spelling out your assumptions in great detail. This is annoying at first, particularly when you want to test an idea and not necessarily worry about all the details. But this discipline pays off: Once you have your code tested and running, you can be confident in the results.

As scientists, we sometimes get lazy with our hidden assumptions and implicit knowledge. This isn’t good in research, because it means you can miss crucial factors. While programming won’t tell you the right way to go about studying your problem, it *will* make explicit all of your assumptions. This provides a great opportunity to reflect on the choices you’ve made for the model under study.

## You Understand What You Can Program

Perhaps the greatest aspect of programming that I’ve found is that it helps build a concrete understanding for the scientific concepts you’re studying.

Reading papers can give you a general sense of the main idea, but science (and mathematics) is an active sport: **You need to engage with the ideas if you want to gain anything more than a surface-level understanding.**

This could mean doing exercises from a textbook instead of directly reading the answers. It could also mean going through a research paper and writing down the steps for *every* equation, making sure that each step is comfortable for you. These techniques force you to jump from passive to active learning, giving you a chance to reason instead of simply following along.

Programming works the same way. I’ve read countless papers now that describe in vague terms (read: English) that a certain simulation was run, with a few equations thrown in to explain the main idea. Maybe that’s fine for a paper, but there’s a world of difference between that and implementing the simulation yourself in code. It’s only when writing code that you find the tricks, techniques, and hidden assumptions that go into calculating Equation 5 of the paper which looked so innocent. Programming makes you go through all the details so that you really understand what you’re doing.

The times I’ve been most confident in my results are when I’ve written the code myself, testing and being aware of each little function that goes into the final result. Doing this also gives me greater leverage in tweaking things for my custom needs, which would be more difficult using a pre-built library[^2]. When I’ve written my own code, the confidence I have in the results skyrockets.

Writing code to capture a scientific equation feels to me like a clear milestone that tells me I’ve “understood” it. If I can write a simulation or do a calculation in code that does exactly what the equation says, it’s a good sign that I’ve internalized the lessons of that equation. It’s similar to doing textbook exercises or going through proofs, just with code.

As I quoted one of the students in my research group last essay, “you understand a topic when you know how to code it”.

---

Programming won’t turn you into an amazing scientist. Rather, I think code can be used as a tool to level-up your knowledge, even if your main research doesn’t lend itself easily to simulations. The act of writing code forces you to think about all of the assumptions you have baked into your model, which is always good to keep in mind. Plus, writing code helps you internalize an equation better than simply staring at it in a paper a hundred times. Programming makes you *play* with that equation, checking its assumptions and drawbacks.

However, I will acknowledge that programming can be an intimidating hill to tackle for scientists. This is why I avoided programming for so long. Setting up an environment for your ideas can be long, and the data structures needed for creating a simulation can bring you out of the creative process[^3]. This is why we need more resources to bring students up to speed. I’m not a fan of telling *every* science student to drop what they’re doing and learn how to code, but I do believe having the ability to model phenomena with code can be a great way to really understand a topic.

When you write code, you think about the assumptions that go into the code. You wrestle with unexpected hurdles that are hidden behind equations. You also deal with the fact that the world isn’t continuous, and that we can only access it in discrete chunks. These are all valuable lessons for a scientist. Remember, equations are only one lens in which to view the world. Code provides another, and it forces you to clarify your thinking.

Writing code is an act of knowledge distillation.

## Endnotes

[^1]: I am ignoring the maddening scenario when your code runs, doesn’t output any error, and yet may be hiding some errors that take a long time to get noticed.
[^2]: I’ve gone this route before. I think using existing libraries is great, as long as you know they won’t limit your end goal. For example, when I’m writing code I won’t hesitate to use [NumPy](https://numpy.org/), since it is powerful and more than enough for my needs. But if I’m trying to do a specific quantum simulation, I might not necessarily jump to the most popular tools available, simply because they don’t accomplish what I need them to. Of course, it’s a balance you have to strike in every project you start.
[^3]: For a lovely view of this, see Molly Mielke’s essay, [“Computers and Creativity”](https://www.mollymielke.com/cc). It’s a beautiful piece, and captures a feeling I’ve had with all sorts of computer tools for creativity. They often have large hurdles to using them for creative work. Yes, programming can unleash essentially unlimited creative potential, but you need to know how to set these things up. That initial time hinders the creative process. If I want to simulate water molecules, I don’t necessarily want to spend hours and hours thinking about the best data structure for the simulation. Yes, the data structure is vitally important, but I think it’s difficult to deny that it blocks the direct path towards creative work.

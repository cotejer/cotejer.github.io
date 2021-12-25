---
title: The Language of Science
author: Jeremy
tags: [science, communicating, research, essay, worldline]
permalink: /language-of-science
date: 2021-12-25
excerpt_separator: <!--more-->
---

When communicating a new idea to someone, use the language they’re familiar with. 

Seems reasonable, but as soon as you go out into the world, you see plenty of examples where this doesn’t happen. In this essay, I want to describe what happens when we commit this error in the realm of science.

Grab a physicist, and force them to sit through a mathematics seminar. Assuming they know the basics of the topic to follow the equations, I bet they will tell you, “I don’t know what this person was going on about! The way they presented things was just…weird.”

<!--more-->

Why does this happen? It’s not an issue of being able to understand the technical details, since most researchers can pick up the basics. One hypothesis is that the problems are so remote that the listener has no desire to understand. For example, if you’re a statistical physicist working on phase transitions, you may not care too much about developments in number theory.

While this plays a role, I don’t think it’s enough to explain the entire phenomenon. Instead, I offer a second hypothesis: the languages mathematicians and physicists use are different.

In fact, it’s worse than this. Even within the a given scientific arena such as physics, we have different specializations that have their own particular terminology. It doesn’t take long for jargon to sprout up, which stops outsiders from understanding your field.

Jargon is useful, until you have to present your work. Then, it’s critical to find the right jargon to fit your audience. If you’re talking to specialists within your field, using the technical jargon is fine. If you’re talking to scientists outside of your field, then use the language they are familiar with. And if your audience doesn’t have any scientific background, avoid technical terms as much as possible.

Don’t try to convert them to use your language unless it’s necessary. Forcing the audience to understand a new language means you have two battles to fight: getting the person to learn your way of seeing the world *and* accepting the new idea. The former is an unnecessary mode of failure.

I learned this last month while giving my first PhD seminar. The physics department at the Université de Sherbrooke is a mix of quantum physicists, statistical physicists, and condensed matter physicists. There’s a whole wardrobe of words and concepts that statistical physicists expect to see when they hear a new idea. These include “ensemble”, “averaging”, “correlations”, “order/disorder”, “phase transitions”, “couplings”, “configurations”, and “spin systems”. If you forgo these words when speaking to them, it makes communicating much more difficult.

I made the mistake of not fully speaking their language. My project[^1] is at the intersection of quantum theory and statistical physics, but instead of speaking to my audience with their language, I retreated to the more familiar language of linear algebra and Boolean satisfiability. This was comfortable for me but not to them, which meant many did not get everything they could have out of my presentation.

Next time, I’ll make sure I keep the audience in mind as I craft my presentation. Not by trying to get them to understand *my* language, but meeting them where they are. That way, I can maximize the chance that the audience understands what I’m saying.

The second place I learned this lesson was while writing my paper for the project. I went through multiple drafts, significant revisions, and rewrites. [The paper is out now.](https://arxiv.org/abs/2112.06939) It’s only four pages, but the effort put into those four pages was immense.

A big reason why it took so long to write is that my supervisor kept insisting we used the language of statistical physics. At first, this irritated me. I had written an early first draft that used the language of linear algebra, mentioned Boolean satisfiability, and had all the details. Why did I suddenly have to change everything and twist it into this other language?

But as time went on, I saw the wisdom in his suggestion. Our target audience all along was statistical and quantum physicists. We weren’t writing a computer science paper. I couldn’t have it both ways. Either I used the language of computer science and wrote for computer scientists, or I used the language of statistical physics and wrote for statistical physicists. In the end, I chose the latter.

Instead of using the word “solution”, I’ll often use “ground state”. Instead of using “parity”, I try to use “couplings”. We wrote a Hamiltonian for the system instead of just an abstract matrix equation. These are all little details, but they make a difference to the reader.

Thinking of my own experience reading papers, it’s usually a process of attrition. If I feel as though I can’t understand every second sentence, it’s frustrating. Every new stumbling block increases the chance I will just give up on a paper. This is why it’s important to know who your work is for. If you know your audience in advance, use the words they know. Make it easy for them to follow along.

---

Communication is about transplanting an idea you have in your head to the mind of someone else. That’s all there is to it, but that doesn’t mean it’s easy. Every scientific field has their own conventions, norms, and language. If you want someone to understand you, it’s worth taking the time to stack the deck in your favour. Use words they know. Speak their language. Give examples that connect to concepts they are familiar with. Know your audience.

The words you use dress up your projects. Scientists are like any other humans: they respond to ideas they are familiar with. By definition, research is about breaking new ground. If you want others to be receptive of your work, it’s probably worth using the language they are familiar with to bring them your exciting breakthroughs.

## Endnotes

[^1]: I will write an essay about the project. There are some neat connections I want to share, and I’ll use the essay to expand on the details that didn’t make it into the paper itself. So stay tuned for this.
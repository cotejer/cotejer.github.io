---
title: Translation
date: 2017-06-12T00:21:22.000Z
author: Jeremy
layout: post
permalink: /2017/06/12/translation
published: true
---

If there's a bane to everyone's existence in mathematics, the word problem seems to be it. These are routinely the most tricky problems to solve, and so many students find themselves understanding the material, only to stumble on this kind of problem. If you ask a student, chances are that they will say these problems are difficult because they aren't as straightforward as a question that asks to solve for $x$ or to find the area of a figure. I don't want to spend today debating whether or not it's a good idea to have word problems, but instead I want to address the fundamental difficulty that I've found many students to have in this area.

In one word, here's the difficulty: translation.

Let's face it. Mathematics is a language, just like any other. This means that mathematics has its own grammatical structure, as well as ways to construct sentences. Additionally, there are ways to make your mathematical sentences clear, and there are many other ways to make them incomprehensible. Unfortunately, many students don't get the experience of seeing what a "good" mathematical sentence looks like, which means they have difficult knowing what expresses total nonsense and what conveys meaning.

To combat this, one of the skills that can help is an ability to translate between the mathematics and your preferred language. My mother tongue is English, so I'll be referring to it here, but there's nothing special about English. The important part is to be able to move between the mathematics and your language. If you can express a mathematical equation in plain English, and (arguably, more importantly) vice versa, it's *so* helpful in decoding problems that you will come across. This ability seems so scarce in schools now that it's almost like a superpower.

I think there's no better way to show this than through an [example](http://www.analyzemath.com/high_school_math/grade_11/problems.html):

> An airplane flies against the wind from A to B in 8 hours. The same airplane returns from B to A, in the same direction as the wind, in 7 hours. Find the ratio of the speed of the airplane (in still air) to the speed of the wind.

If you want to have any hope of solving problems like this in a systematic way, you *need* to know how to translate between the words and the mathematics you'll use to answer the question. If you want, I encourage you to try this question out, and make a *detailed* solution. This doesn't mean you need to write ten pages of explanation, but it means that everything you do should be clear.

Got it? Okay, let's go through the way I would solve this.

First, you should identify the quantities you're looking for in this problem. From what I can see, the quantities we are looking for are the speed of the plane when there's no wind, and the speed of the wind itself. Do we know the *numerical* values of these quantities? We do not, so let's give them symbols. Let's call the speed of the plane without any wind $v$ and the speed of the wind itself $w$. Note that the units of both are something akin to $m/s$.

Now, we don't know how far the distance is from point A to B, so we'll just call this distance $d$, with units of metres.

With all of the variables of the question in hand, it's time to translate from the words in the problem to mathematical equations. This is a crucial part of solving these problems, and it's good to take it sentence by sentence. But first, let's state clearly what we are trying to determine. We want the ratio of the plane's speed in still air to the wind speed. In our variables, this corresponds to the expression $\frac{v}{w}$.

Here's the first sentence again: *An airplane flies against the wind from A to B in 8 hours.*

For this sentence, we need to relate the time traveled (8 hours) and the distance from A to B ($d$). The most natural way to do this is through the speed of the trip. Note that, since the airplane is flying *against* the wind, it's "net" speed is $v-w$. This is due to the fact that the wind is slowing the plane down. We then know that the speed of anything is given by a distance over a time (here, we are talking about average speed), so we have the speed being $\frac{d}{8}$. Therefore, we get the following equation:

$$v-w=\frac{d}{8}$$

Let's parse the second sentence: *The same airplane returns from B to A, in the same direction as the wind, in 7 hours.*

This is similar to the above, except now we have a time of 7 hours, and a "net" speed of $v+w$. You can think of it as the wind "helping" the airplane as it moves to its destination. The distance is once again the same, so we have the following relation:

$$v+w=\frac{d}{7}$$

This is by far the most difficult part of a word problem. For the most part, students can do the actual computations, but the difficult part is the translation. In this problem, we see that the tricky aspects include knowing that speed is given by a distance divided by a time, and being able to relate the sentences into that form. This isn't a skill that's developed within a week. It's something that you need to focus on for many problems in order to understand how these kinds of situations go.

Here are the big parts of translating from English to mathematics:

- Knowing what equality means. But I know what equality means, you say. Of course, we know implicitly what it means, but the reality is that many students will claim to know what equalities mean, yet write things that *aren't* equalities. This is easily seen in terms of units, where many students will make equations whose units don't agree. Indeed, being able to look at the units of your quantities is a great way to help you come up with equations. This is called dimensional analysis.
- Knowing what the words "more", "less", "at most", "in total", and so on, mean. Each of those words has a precise mathematical meaning, and it's critical that you know the difference between them.
- Relational words like "double", and "half". This closely follows from the above, but this also gets a lot of students tripped up. If I said to you that I (let's call me $x$) had double the amount of something than you (which we'll label $y$), is the inequality $x\ge 2y$ or is it $y \ge 2x$? It's very important to know how to differentiate between these two. (Hint: it's the former.)
- Knowing how to parse through negation. When you see the word "not", can you infer the correct meaning? It's an unfortunate reality that many questions throw in a bunch of extra (and confusing) negation in order to trick students for no good reason, and so being able to deal with this is a must.

---

In the end, the important thing is that you can comfortably go between English and mathematics. The arrows should go *both* ways, even if you're only tested on one way. The reason is that it's helpful when learning a new concept to express it in words, since it can make the concept more clear than in abstract notation. Of course, that notation is important when you're trying to precisely answer a question, but it's good to be able to talk more informally about an idea.

My advice is therefore this: when you encounter a word problem, go through it line by line, asking yourself, "How can I translate these words into mathematics?" Similarly, do it the *other* way when you encounter equations, so you get a sense of the other side of the coin. By doing this, it becomes easier to move between the two languages, without having to carry an English-to-mathematics dictionary.

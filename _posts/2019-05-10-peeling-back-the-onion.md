---
title: Peeling Back the Onion
author: Jeremy
tags: [learning, education, mathematics]
permalink: /peeling-back-the-onion
date: 2019-05-10
---

No matter how much advanced mathematics you study, the great thing is that you rarely have to *accept* anything as-is. If you come across a procedure, technique, or result and you wonder how in the world it works, you can always retrace your steps and get back to the foundational reasons as to why it works. If you keep on asking "why", you will eventually get back to your starting axioms. In between that and your starting point, you should be able to understand the concept as obvious[^1].

It's in this sense that any mathematical concept is like an onion. You have the initial concept, which is something that may or may not seem obvious. You can then peel away the layers, moving away from the tools you built up and going back to the axioms in which you built them from. It can be a good exercise to do this for any given concept you're studying. How far back can you go before there no more layers to peel?

The reason this is a good exercise is because it makes you think about your initial assumptions. What did you absolutely *have* to start with in order to build up your mathematics? School can give us the impression that mathematics is just *there*, a bunch of rules and techniques you can follow in order to solve problems. But these rules and techniques didn't appear out of thin air. They were constructed by mathematicians. And if they were constructed, that begs the question: constructed out of what? Answer this question enough times, and eventually you will say that the materials were just *there*. That's when you've hit the bedrock, your axioms. The thing that isn't often noted is how infrequently one is at the bedrock. In fact, most mathematical concepts aren't the "centre" of their onion. They are part of some outer layers, with the core concept hidden from view. It takes some effort to peel back the layers and uncover it. Furthermore, one can get so used to the outer layer that it seems like that's *all* there is to it.

One example that comes to mind is that of the derivative. If we consider a function of one variable, the definition of the derivative uses limits when looking at the rate of change between two neighbouring points as that distance closes to zero. But if I gave you the function *f(x) = x<sup>2</sup>* and asked for its derivative, I'm guessing you wouldn't even *mention* limits. Instead, you would tell me that it's *f'(x) = 2x* because of the power rule, and be done with it.

While that's correct, where does this power rule come from? Do we have to assume it works all the time, or can we *show* that it comes from some deeper assumptions? In essence, is the power rule an outer or inner layer of the onion?

It turns out that the power rule comes as a consequence of applying the definition of the derivative (using limits) to these functions with powers. From there, you can derive the power rule. Once you've done that, you don't need to play around with the definition of the derivative anymore. You've *shown* that functions with powers always behave in this certain way. In essence, you've found a way to sidestep using the limit definition of the derivative, since the derivative of these functions always works in the same way.

This shows that the power rule has some subtleties layered inside. It's the result of using the full definition of the derivative, and this involves limits. Therefore, more interesting mathematics is nestled inside of the power rule. Furthermore, we haven't even discussed what it means to have a limit. We just assumed it meant something obvious. But what does a limit mean, exactly? The definition of a limit involves inequalities, deltas, and epsilons, to the chagrin of many real analysis students. It's not *difficult*, exactly. It's just technical in nature, which means it can seem far-removed from what we might say a limit is when speaking.

The point here is that we are rarely standing on the axioms. If you've ever taken a class in linear algebra, you often spend a small bit of time in the first class talking about the properties of vector spaces and how elements in a vector space behave under the usual operations. You then probably jumped straight into discussions about linear independence, rank, solving matrix equations, and finding the eigenvalue for matrices. You left those initial properties behind without thinking about them too much. Well, *those* properties were the point at which you could say you were standing on the bedrock. As soon as you move on, you're building on these initial axioms (plus any extra definitions such as scalar products and whatnot). Therefore, it seems a lot more likely that the mathematics you're studying right now lies on the outer part of an onion, not the interior.

Of course, I'm not trying to get you to go back to the axioms every time you solve a problem! Frankly, that would be ridiculous. Imagine if you started doing proofs with limits every time you need to take a derivative. You would tire yourself out before you even got started on the problem. As such, it's useful to have these rules and extra mathematics. It's what mathematicians do. They try and build more structure on top of the underlying axioms.

The point I want you to reflect on is how most of mathematics is just a layer of an onion. You can often go in *both* directions, outwards to mathematics that builds on the concept you're studying, and mathematics that was used to build *your* concept. The concept you're looking at is almost certainly not fundamental.

It's worth thinking about the next time you're studying a concept in mathematics. What was used to build it? Is there anything interesting lying underneath the concept? My experience is that peeling back the layers of a mathematical onion is both a useful and enlightening activity.

The next time you want to learn something new, my suggestion is to take what you know and go *deeper*. Find the underlying mathematics that builds up to what you know. It will give you a greater appreciation for the way mathematics is constructed.

[^1]: Though, retracing the steps of a proof or technique can be a lot trickier than you initially bargained for.

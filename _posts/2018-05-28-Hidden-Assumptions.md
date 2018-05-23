---
title: Hidden Assumptions
author: Jeremy
permalink: /hidden-assumptions
category: Mathematics
date: 2018-05-28
---

I remember when I first took a class in linear algebra, and we were talking about vector spaces. In addition to the definition of a vector space, we were also given multiple axioms that define what the structure of a vector space looks like. This included a bunch of boring things, like the fact that if you have a vector *v*, you should have a corresponding vector *-v* such that *v+(-v)=0*, where 0 is the zero vector. There are eight of these axioms, and together they describe exactly what can be called a vector space.

If you look at the axiom above, you might think that's obvious. Of *course* I can go backwards from my vector *v* to get to zero. Similarly, you would probably balk at the notion of most of the other axioms, such as commutativity (*a+b=b+a*) or that there is a zero vector such that *v+0=v*. These properties seem more than obvious to you. They are *ingrained*. Why do these define a vector space specifically? Doesn't this always hold for any kind of space?

Well, not quite. If we just focus on commutativity, this is something that isn't always true. To take an example that isn't part of mathematics, but is something else we do in our everyday lives. Imagine you were eating a bowl of cereal in the morning. After taking out your bowl and putting cereal in it, you then pour your milk, followed by eating the cereal. But what it you did those last two steps in the opposite order? Now, you eat your cereal, and *then* you pour your milk in the bowl. Evidently, your cereal-eating experience won't be the same in both cases. This illustrates something we don't often appreciate in mathematics. Order *is* important. It's just that we tend to work in spaces that have this nice and special property, so we start to think that *all* spaces do.

If you want a more mathematical example of commutativity not holding, the classic example is that of matrices. This is another part of linear algebra, and while taking the course you quite quickly figure out that the order *does* matter when multiplying matrices. Suffice to say, bad things happen when you start assuming things will work out without *knowing* if your assumption is correct.

Why is this important? We often go through a lot of our mathematical lives without considering our assumptions. Instead, we focus on solving particular problems, and then comparing with a known answer. Furthermore, we tend to get used to thinking about the particular spaces we work in, and assuming that these nice things will hold for all other spaces. This lack of diversity creates bad habits in our mental models, creating prejudice for one specific way of things working.

Remember, axioms are the foundation for basically everything you do in mathematics. If you keep on digging, you should always hit a floor of axioms. This is simply because the goal of mathematics is to discover truth *from* those axioms. These axioms can't be proven. They are taken for granted. But the surprising thing is that the rules and elements *we* take for granted on a day-to-day basis within mathematics *aren't* axioms. They are actually statements that can be proved using other axioms.

For example, take an innocent-looking statement that almost no one will blink an eye at while reading:

If *a &ne;0* and *ab=ac*, then *b=c*.

This is known as the law of cancellation. We get quite good at doing this in secondary school, where we learn how to simplify fractions and other expressions. This naturally comes in handy, because it lets us avoid working with larger numbers than we have to do. If *2x=8*, we can "cancel" a factor of two from both sides of the equation and obtain *x=4*.

So far, so good. This is harmless, right? How could a simpe rule like this possibly go wrong?

The problem is that you're not thinking about this in general. The subtlety here is that **it matters where the elements *a* and *b* come from.** If they are part of the real numbers, then fine, that's not a problem. But it takes a particular type of "setting" to have this cancellation rule. In particular, you need to be in an *integral domain*, which is a space that is basically defined by this property.

And no, there are very real examples that *aren't* integral domains. For example, let's do some arithmetic in modulo eight. This just means that we reduce any number until it's the remainder upon division by eight. In this setting, we then have that *6 &equiv; 14*. But look what happens here. We know that *2&sdot; 3 = 6*, and *2&sdot; 7 = 14*, but even though *2&sdot; 3 &equiv; 2&sdot; 7*, we *certainly* don't conclude that *3 &equiv; 7*. When you divide both of these numbers by eight, the remainders are three and seven respectively, so they are not the same. As such, you can immediately see that the cancellation doesn't work all the time.

What this hints at is that we can often be surprised by our prejudices. The cancellation rule is very common and is acknowledged throughout secondary school, so you might almost feel cheated that this is suddenly not taken for granted. This is a normal reaction, and it's one you will slowly learn to ignore.

*This* is why learning and remembering those "boring" axioms is so important. They are the building blocks in which we base our structures on, so it's vital that you remember them. Additionally, you should frequently pose yourself questions such as, "Why do we *require* this axiom? Can I get all of the results I want without it?" Remember that we are frequently interested in generalizing notions in mathematics, so we don't want to carry along "extra baggage", if you will. We want enough axioms to give us some constraint and structure (or else we won't be able to generate results), but we don't want to assume anything that we aren't absolutely forced to. It's about minimality, and only adding structure when you need it. So all of those axioms you learned in various classes, *were* important, because there are other settings where these aren't taken for granted.

It's a mathematical jungle out there, so best to keep in mind your foundational axioms while learning a new topic.
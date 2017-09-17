---
title: Linear versus Cyclic Permutations
author: Jeremy
permalink: /linear-vs-cyclic-permutations
date: 2017-10-02
---

One aspect of probability I've always found to be a little tricky is the part where you need to count things. In theory, this sounds easy enough. After all, it's just looking at the complete list of things you're studying, and enumerating them, right?

Well, we know that things become much more subtle when you have a big number to count and you have to be careful when using the "tricks" of multiplication in order to avoid duplication. This is the part that has sometimes seemed straightforward, while at other times being totally mystifying.

If you've taken an introductory probability class, you've undoubtedly come across the notion of permutations. This concept simply deals with answering the question, "How many ways can I order these items I have?" Just to briefly review, let's look at an example. Suppose I want to know how many different ways I can order four items: *a*, *b*, *c*, and *d*. The answer is given by $4!$, which can be seen below.

![](/images/ordering.png)

This makes sense, and it's usually the image we have in mind when thinking about permutations. This readily generalizes to $n$ items, where the number or permutations is $n!$.

But here's a question. What are the possible orderings of the four items from above if I arrange them in a circle like this?

![](/images/circle_Ordering.png)

Suddenly, the idea has shifted. Now, the *absolute placement* of the object doesn't matter (eg. Is it first, second, third, or fourth?), but it's placement *relative to the other objects* matters. If we look at object *a*, the only thing that matters is that it is in between objects $d$ and $b$. How the circle is oriented doesn't matter. As such, these scenarios are now equivalent.

![](/images/equivalent_Ordering.png)

The question now becomes, "How do we address this change in possibilities within our expression?"

If we consider the circles I drew above, you may notice that there are four of them. This is not a coincidence. The reason is that if we have a certain configuration of the circle with $n$ objects comprising the circle, we can rotate the circle $n$ times without changing the relative positions of the objects. This is because the circle possesses rotational symmetry. As such, the number of ways you can permute the four objects is the the number of ways we can permute them when they are in a line, *divided* by $n$. Mathematically, this looks like:
$$
P_{cyclic} = \frac{n!}{n} = (n-1)!
$$
Here, I've used the symbol $P_{cyclic}$ to represent the permutations that can be made in a cycle.

---

This wasn't meant to be a long post, but it's something that I thought was interesting, since (without thinking about) we usually only consider the linear case when looking at permutations. I wanted to show here that circular permutations are just as easy as regular permutations.
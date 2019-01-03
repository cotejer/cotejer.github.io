---
title: Equations as Constraints
author: Jeremy
tags: [Mathematics]
permalink: /equations-as-constraints
date: 2019-02-18
---

Can you construct a right cone that has a height of 4, a radius of 3, and a slant height of 6?

This question has an easy answer, but only if you know what to look for. The reason is that the question is posed in a way that requires a "yes" or "no" answer. If your answer is "yes", then you have to prove it by giving me a cone that has the desired properties. On the other hand, if your answer is "no", you can't prove this by saying that you tried a few and it didn't work. You have to give me a reason why it will never work.

The manner in which this question is posed can lead to students going in the wrong direction for a long time. This is particularly true if they are trying to prove that it's possible, because the answer is that it's *impossible*.

How can we show this? The reason is quite simple. For a right cone, the radius *R*, height *h*, and slant height *a* of the cone follow the Pythagorean theorem. Therefore, we get a^2^ = h^2^ + R^2^. If *h = 4* and *R = 3*, then *a^2^ = 25*. But if *a = 6*, then *a^2^ = 36*, which leads to a contradiction here.

Nothing magical in this answer. However, there is a subtle point that isn't always made explicit to students. It's the fact that an equation *constrains* the values certain variables can take on. In essence, the equations reduces the "degrees of freedom" in our variables.

Let's consider our equation a^2^ = h^2^ + R^2^. We have one equation, and three variables. This means that you can choose the value for *two* variables, but once you've done that, the last one is fixed. You can't choose it at random, because it wouldn't satisfy the equation above. **Therefore, the equation reduced our choice for the variables.** (Also, we're taking all of our quantities to be positive here, so no negative solutions allowed.)

This allows us to look at equations in a new light. Instead of thinking them as machines that take in elements and output new ones, we can think of them as *constraints* between variables. When we have an equation that links variables together, we no longer are able to choose them freely. In other words, they aren't independent. Since the equation must be satisfied, you can only specify so many variables before you have no freedom left. At that point, you're forced to use the equation for that final variable.

If you want to visualize what this means, start by thinking about a line. If it's of the form *y = ax + b*, then as soon as you choose a value for *x*, you have no choice in the matter for *y*. It's locked in place. On a graph, this means that you will only have *one* value of *y* for any *x*.

The principle is the same for higher dimensions, but it can get difficult to visualize. However, for a two dimensional surface like a sphere, you have the equation *r^2^ = x^2^ + y^2^*. This is something you can visualize. The radius is constant, so the only two variables you can change are *x* and *y*. You might think that choosing a value of *y* locks in the corresponding value for *x*, but that's not quite true. The reason is that the terms are squared. Therefore, choosing a value for *y* results in *two* possible values of *x*, but the only difference between them are their signs.

To see an explicit example, imagine we're looking at the unit sphere, so we have *1 = x^2^ + y^2^*. If we let *y = 0*, we then get *1 = x^2^*. This has two solutions, given by *x = 1* and *x = -1*. Visually, this corresponds to the points (1,0) and (-1,0). Once again, choosing a value for *y* constrains the possible values of *x*, but instead of constraining *x* to one value, we get two. This has to do with the nature of the equation. Still, if we think about all of the possible points on the sphere (there are infinitely many!), going from all the points to two points is quite the constraint.

---

This is just another way to think about equations which might be helpful in certain scenarios, like when considering systems of equations. The machine analogy is useful, but thinking about equations as constraints has its merits as well, and isn't always told to students.
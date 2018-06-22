---
title: Why Can't We Reach the Speed of Light By Boosting?
author: Jeremy
permalink: /speed-of-light-limit
date: 2018-03-19
category: Special Relativity
---

If you have ever come across someone talking about special relativity, there's a good chance you will be able to tell me one of the two fundamental axioms in the subject: the fact that the speed of light is constant in all frames of reference.

After thinking about this for a few moments, one might come up with a thought experiment that *looks* like a counterexample. Imagine (for the sake of the experiment) that there's a train moving along at a constant speed (we'll call it *v*) along the ground with respect to you, the unmoving person. Then, imagine that there's another train on top of the first train, and its moving at a speed *v*, but with respect to the first train. As such, you would undoubtedly agree that the second train seems to be moving faster than the first train, since it has the speed of the first train *and* its own speed.

Following this argument, it seems reasonably straightforward that if you keep on stacking trains on top of each other such that they all are moving relative to the last one with speed *v*, at some point, no matter how slow the speed *v* is, one of the trains should exceed the speed of light. Bingo, we've done it!

Unfortunately, this is not so. But what is the actual problem here? Why can't we get past the speed of light?

To answer this, I'll have to introduce a few things. But first, some notes. One, we are trying to see why the speed of light acts as a "cosmic speed limit", so we aren't going to simply say, "Let the speed of the first train be faster than the speed of light." Instead, we want to see why we can't build *past* it. Second, I want to note that this isn't just a strange situation that has no applications. If you don't like the scenario with the trains, imagine continually boosting oneself to a faster and faster speed. Of course, this has to still be done with the right Lorentz transformation, but you *will* hit a barrier.

With that out of the way, let's dig into the problem. We could try and do successive Lorentz transformations in order to get the relative velocity between the observer on the ground and the *n*<sup>th</sup> train. However, the fact is that this isn't the "natural" or easy way to do the problem. In special relativity, velocities don't add like we are used to. Instead, there's a fancy factor &gamma; and several other differences when transforming velocities. However, there is a quantity that does simply add when two velocities are composed. It is called the rapidity, and is denoted with the letter &phi;. It is defined as:

$$
\begin{equation}
	\tanh \phi = \beta.
\end{equation}
$$

Here, &beta; is just the ratio of the speed (that any train is moving at with respect to the one underneath it) and the speed of light. For our problem, this value is constant. We want to know how fast the *n*<sup>th</sup> train is moving, so we just have to keep on adding the rapidity factors. But they're all the same! This means we get the rather simple result that the rapidity for the *n*<sup>th</sup> cart is *n* times the first train's rapidity factor. We then use the definition for &phi; from above in order to get:

$$
\begin{equation}
	\tanh \phi_n = \beta_n = \tanh \left( n\phi_1 \right) = \tanh \left( n\tanh^{-1} \left( \beta_1 \right) \right).
\end{equation}
$$

We could stop here since everything in the above expression is a constant that we would input, but we don't want to know what happens for the *n*<sup>th</sup> cart. We want to keep boosting forever, until we get past the speed of light! This means we need to take a limit as *n* tends to infinity. Therefore, it would be nice to have our above expression in a form that we can take a limit much more cleanly. I'll spare you the gory details, but basically we can use the identities for hyperbolic functions that allow us to go from them to  exponential and logarithmic functions. After doing this, you should be able to get something like the following:

$$
\begin{equation}
	\beta_n = \frac{1-a^{-n}}{1+ a^{-n}}, \text{ where } a \equiv \frac{1+\beta}{1-\beta}.
\end{equation}
$$

This is actually a nice expression, because its limit is very easy to evaluate. Before this though, let's look at plot of this function as a function of *n*. In other words, we want to see the behaviour of this function as *n* gets larger.

![Plot of the function defined above in terms of n.](/images/rapidity.png)

As you can see, the function gets closer and closer to one as *n* increases. Why isn't it the speed of light *c*? Remember what &beta; is. It's the speed of the train divided by the speed of light, so having the plot asymptotically go towards one is what we should expect. Also, if you're curious, the value for &beta;<sub>1</sub> is 0.5, which is quite a large value. This is why the function asymptotes to one very fast.

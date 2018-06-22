---
title: One-to-One and Onto
author: Jeremy
category: Algebra
permalink: /one-to-one-and-onto
date: 2018-04-09
---

When learning about functions, a few properties come up over and over. In particular, we often hear about functions being one-to-one (injective) or onto (surjective). These are important properties of functions that allow one to set up correspondences between sets (bijections), as well as study other features of various functions. I wanted to go through these two properties in a slightly different way than what most sources will do to explain them, so hopefully this will be a good analogy to keep on mind when discussing these two properties.

First, let's define our function. We will consider a function *&fnof;* that moves objects from a set *X* to a set *Y*. We usually call *X* the domain, and *Y* the range.

If *&fnof;* is one-to-one, it has the special property that any time you look at an element *y* in *Y* that has some element from *X* sent to it, *only* that element gets sent to *y*. If we think of the function as a bunch of arrows linking up elements from *X* to elements in *Y*, there will be at most one arrow pointing to any given element in *Y*.

The way I think about it is this. Imagine the function as a machine with a specific set of instructions, and an input and output area. You stand at the output area, and I stand at the input area. If you know set of instructions that the machine executes, and you receive something at the output of the machine, can you tell me what I put into the machine without seeing it beforehand?

![](/images/inputOutput.svg)

Your initial reaction might be, "Of course, I can tell you what you put in! I'll just do the instructions in reverse."

This is fine, but let's go through an example. Suppose that the machine takes in a number, and then outputs that number modulo two. This means that the machine outputs the remainder of the input number after division by two. In other words, this machine will ouput 1 if the input number was odd, and 0 if the input number was even.

Okay, so you wait at one end of the machine while I insert my number, and the output of the machine is 0. What number did I put in? Well, you know that the number wasn't odd, because only even numbers get sent to zero. However, apart from that piece of information, you have *no idea* what number I put in. It could have been any even number.

This is an example of a function that *isn't* one-to-one. If we go back to our definition, the reason it isn't one-to-one is because every single even number "points" to zero. Therefore, you can't "undo" the machine's instructions, because they destroyed (for lack of a better word) the nature of the input while executing the intructions.

I like this analogy with the machine, because it helps us see that not all functions "go both ways". You can't always get back to the input from the output. In fact, this property *only* holds when a function is both one-to-one and onto.

Which brings us to the property of being onto. This one's slightly different. A function is onto if, no matter what element you pick in *Y*, there is *some* arrow pointing to it from the set *X*. More formally, for any *y* &isin; *Y*, there exists a *x* &isin; *X* such that *&fnof;(x)* = *y*.

I like to think of this from the perspective of the set *X*. When I think of a function being onto, I imagine we are shooting arrows from the set *X* and doing so in a way that we ensure each elements in *Y* are hit. Put differently, our function *&fnof;* doesn't "miss" any of the elements in *Y*.

For example, if we take a very simple function, *&fnof;(x) = x+1*, we can see that this function is onto, because it "hits" any value in our output set (here, we will let *x* any real number, so our set *Y* = **R**). However, a different function such as *&fnof;(x) = sin x* is *not* onto because the outputs of our function only belong to the interval [-1, 1], which means we miss a *lot* of values in **R**.

Sometimes, you will work with a function that is both one-to-one *and* onto. In that case, the function is called *bijective*, and it's a very nice property for a function, because it allows one to identify an inverse transformation. This is something you've undoubtedly come across in secondary school. The idea is that if you a function *y = &fnof;(x)*, you can "solve" for *x* in order to get a new function in terms of *y*.

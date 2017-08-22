---
id: 650
title: 'Why Can&#8217;t I Divide By $\sin$?'
date: 2017-06-03T20:21:22.000Z
author: CJeremy
layout: post
guid: 'https://blog-cjeremy.rhcloud.com/?p=650'
permalink: /2017/06/03/why-cant-i-divide-by-sin/
categories:
  - Uncategorized
published: true
---
One of the most common misconceptions I see while working with students in secondary school is the notion of an inverse. The idea isn&#8217;t too complicated, but the reason that I see students making mistakes with it is because they are in the process of learning about functions and it becomes a cognitive burden to think about these abstract processes such as inverses and other transformations. However, I firmly believe that giving students the right idea of how these different concepts fit together will help them navigate their classes with ease.

## Example: Trigonometric Functions

I want to start right off with an example that is indicative of why it&#8217;s important that you understand inverses. Imagine you had the following problem, and you were looking to solve for $x$:

$$10+3\sin(x) = 11$$

There&#8217;s nothing particularly nasty about this equation. Like all the other ones you see, you need to isolate for $x$, so you start by subtracting $10$ from both sides.

$$3\sin(x)=1$$

From here, you then probably say to yourself, &#8220;We need to divide by $3$ on each side.&#8221; So, that&#8217;s what we do:

$$\sin(x)=\frac{1}{3}$$

Now, here&#8217;s where things can get tricky if you&#8217;re not being careful. Depending on what you&#8217;ve been taught, you will have several reactions to this. Unfortunately, the one that usually happens is, &#8220;Let&#8217;s divide both sides by $\sin$&#8221;, giving us:

$$x=\frac{1}{3\sin}$$

Let&#8217;s state it right now: this is _incorrect_. In fact, you can prove it to yourself by trying to enter this value of $x$ into your calculator. It won&#8217;t work (unless, you wrote the $3$ after the $sin$, which then _would_ give you an answer, albeit an incorrect one).

I wouldn&#8217;t mention this if I haven&#8217;t seen it enough before, but I think it captures a misunderstanding of something that&#8217;s quite a bit more important than simply saying, &#8220;You have to use $\sin^{-1}$ to get the answer.&#8221; What I want to give you is a _reason_ to understand why what I wrote above is wrong, and this is the concept of an inverse.

## What exactly is an inverse?

Like virtually all topics in mathematics, there are many ways to think about inverses. For the purpose of solving equations, I want to present you this simple first thought:

_An inverse &#8220;undoes&#8221; whatever you&#8217;ve done to an expression. It&#8217;s similar to an &#8220;undo&#8221; button that you might use on a computer._

This isn&#8217;t very precise, so let me give you a more mathematical definition:

_Given a function $f(x)$, its inverse, denoted $f^{-1}(x)$, is defined by the following: $$f^{-1}(f(x))=x$$._

This might still seem a little unclear, but with a few examples, you will understand that this isn&#8217;t a groundbreaking concept.

### Example: Find the inverse of $x^2$

To find the inverse, we need to first identify what kind of function is &#8220;acting&#8221; on $x$. In this case, the function that is acting on $x$ take the form of $f(t)=t^2$. Note that I&#8217;ve used the variable $t$ in order to make it distinct from $x$. Then, once we substitute $t=x$ into our equation, we get $f(x)=(x)^2$. I also added parentheses around the $x$ in this equation in order to show you that the thing I&#8217;m doing to $x$ is _squaring_ it.

So far, so good. We now have to the inverse, $f^{-1}(x)$. To do this, ask yourself the question: how do I get rid of the &#8220;squaring&#8221; function that is acting on the $x$ at the moment? Remember, our goal is to make a new function that when you substitute $(x)^2$ into it, the result you get is $x$. Try it out for yourself.

The operation we need to do is take the _square root_. As such, we define our new inverse function to be $f^{-1}(t)=\sqrt{t}$. What this means is that I have to take the square root of whatever I put into $t$. For our purposes, we are going to feed it our function $f(x)=(x)^2$, giving us:

$$f^{-1}(f(x))=f^{-1}(x^2)=\sqrt{(x)^2}=x$$

In other words, if we had the equation $x^2=4$, we know that solving for $x$ means taking the square root on both sides of the equation, giving us $x=\pm 2$. One way to look at this is to say that you&#8217;re taking the _inverse_ of the square function, which returns the variable by itself (in this case, $x$).

## Revisiting our example

Let&#8217;s go back to our trigonometric example from above. To remind you, we were trying to solve:

$$\sin(x)=\frac{1}{3}$$

At this point, you should be looking at this and thinking, &#8220;Okay, there&#8217;s a function that&#8217;s acting on $x$ on the left hand side of the equation. In order to solve for $x$, all I need to do is take the _inverse_ of that function.&#8221;

Indeed, this is _precisely_ the purpose of the inverse sine function, denoted $\sin^{-1}(x)$! It&#8217;s purpose is to &#8220;undo&#8221; the work that the sine function did, and return the angle you originally fed the function (in this case, $x$). Explicitly, this is how the manipulation goes:

$$\sin^{-1}(\sin(x))=x=\sin^{-1}\left(\frac{1}{3}\right)$$

One thing that I want to very clearly express: the $-1$ superscript on the function is **_not_** an exponent. Instead, it&#8217;s just a symbol we use to declare that it&#8217;s the inverse function, just like our symbol of a generic inverse function for a regular function $f(x)$ is $f^{-1}(x)$.

## Solving equations is just repeatedly applying inverse functions

Once you understand the idea of an inverse function, you start to see that they are _everywhere_. Indeed, when we solve basically any equation, we are implicitly asking, &#8220;How do I _undo_ what the equation has done?&#8221; If you look back to the example we first started with, $10+3\sin(x) = 11$, we first applied the inverse of $f(t)=10+t$ on both sides, namely $f^{-1}(t)=t-10$. This corresponded to subtracting $10$ from both sides of the equation. Similarly, we applied another inverse function to divide both sides by $3$.

Remember, when you&#8217;re trying to solve for a certain quantity, you want to do the inverse of what the equation has done. By looking at solving equations by repeatedly applying inverses, you won&#8217;t make the mistake of dividing by $sin$ ever again.

## Final note

I just wanted to include a final remark about inverses here. I didn&#8217;t explicitly say it above, but when you&#8217;re working with algebra (but not special functions like trigonometric ones), you usually have two different kinds of inverses: additive inverses and multiplicative inverses. They aren&#8217;t complicated at all, but they are slightly different.

An additive inverse means that, if you have a certain term that we&#8217;ll call $a$, then an additive inverse satisfies the following:

$$a+(-a) = 0$$

That&#8217;s simple enough, and it usually means just slapping on a negative sign to your term.

Next, we have the multiplicative inverse. If you have a term that we&#8217;ll call $x$, then the multiplicative inverse satisfies the following:

$$x* \left(\frac{1}{x}\right)=1$$

Once again, nothing too complicated. Just be aware that both exist, and that they are both different &#8220;kinds&#8221; of inverses. You use a specific one depending on what you&#8217;re trying to solve for.

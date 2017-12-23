---
title: Calculating $\pi$ Factorial
author: Jeremy
permalink: /pi-factorial
date: 2017-12-11
---

One of the things I like most about mathematics is its ability to generalize results to realms that one might not have previously thought of before. Historically, this is what happened with rational numbers, negative numbers, irrational numbers, complex numbers, and so on.

Most of you have probably heard of the factorial operation before, but here it is again explicitly. Essentially, if you have a natural number $n$, then it's factorial is denoted as $n!$ and is defined as $n! = n(n-1)(n-2) \ldots (2)(1)$. That's an easy enough definition. Start with your number, and just multiply it by all of the numbers that came before it (until you get to one). We also have the base cases of $1!=0!=1$.

The factorial is what is known as a *recurrence relation*. Instead of getting an explicit formula for how to calculate each term, you get what the $n^{th}$ term is in relation to the next term below it (for this specific case). Let's do an example with $5!$. If we look at our definition above, we get $5! = 5 \cdot 4!$, since the rest of the multiplication is "hidden" within $4!$. As such, we don't get a number for $5!$ until we figure out what $4!$ is, which we can only do if we find out what $3!$ is, and so on. Therefore, the factorial is really a recipe, and the only time we get a real answer is when we hit $1!$, which we set to $1$. 

That's great, but it doesn't look very helpful for calculating $\pi!$. After all, $\pi$ is definitely *not* in the naturals, so we can't make use of the definition above. However, let's keep in mind the kind of *relation* that the factorial gives us. It tells us that $n! = n \cdot (n-1)!$. Let's see if we can get something else to work like that.

Somewhat completely out of the blue, let's take a look at the following function:

\begin{equation}
\Gamma(a) = \int_0^\infty x^{a-1}e^{-x} dx, \,\,\,\,\, a \gt 0.
\end{equation}

This function is called the Gamma function, and it's used in probability distributions (which is where I came across it). Now, this might seem like a really weird function to throw at you. How in the world does this relate to anything about factorials? Well, let's start by trying to calculate the value of $\Gamma(a+1)$.

\begin{equation}
\Gamma(a+1) = \int_0^\infty x^{a+1-1}e^{-x} dx = \int_0^\infty x^{a}e^{-x} dx
\end{equation}

Then, we can integrate by parts using $u=x^a$ and $dv = e^{-x}dx$ to get:

\begin{equation}
\left[-x^a e^{-x} \right]_0^{\infty} +a \int_0^\infty x^{a-1}e^{-x} dx.
\end{equation}

The first term evaluates to zero at both boundaries (which can be seen by taking the limit as $x \rightarrow \infty$). Therefore, we are only left with the second term. However, look at the form of the integrand. It's simply $\Gamma(a)$. As such, we conclude with the following relation:

\begin{equation}
\Gamma(a+1) = a \Gamma(a).
\end{equation}

This is really neat, because it's another recurrence relation that gives us an answer in terms of the previous (lower) one. We can also look at the result of $\Gamma(1)$, and confirm that is indeed equal to one. In fact, this means that we get the following result: $\Gamma(a) = (a-1)!$. It's a recurrence relation exactly like the factorial, but formulated in a totally different way. The one important difference though is that the value of $a$ is *not* limited to natural numbers. Now, we simply need $a \gt 0$, which means we can easily calculate $\pi!$. This corresponds to a value of $a = \pi + 1$. Inserting this into the integral definition and evaluating the integral numerically gives a result of:

\begin{equation}
\pi! = \Gamma(\pi + 1) = \int_0^\infty x^{\pi}e^{-x} dx \approx 7.18808.
\end{equation}

How do we interpret this result? I don't know! But roughly, I can say that it's a bit more than $3! = 6$, so at least something is on the right track. However, calculating the result of $\pi!$ in particular isn't of too much importance. It's simply a neat extension of how one can think of factorials.

---

One thing I do want to note is that, just because we have a recurrence relation with this Gamma function, this doesn't mean we *technically* have the same thing as a factorial if $a$ is not a natural number. Really, we then just have a recurrence relation. However, it's still an interesting connection that's worth sharing. Sometimes, seeing operations and concepts you were only used to seeing in one setting suddenly operating in another scenario can broaden one's perspective on mathematics.

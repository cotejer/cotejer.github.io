---
title: Integrating the Gaussian Function
author: Jeremy
date: 2017-10-16
permalink: /integrating-gaussian-function

---

As I take my first quantum mechanics class, I've come to find that integrating probability density functions are a pain. From only a few problems I've worked on, the integrals are long and tedious to do. If there's a single theme present in these integrals, it's the strategy of integrating by parts. However, I wanted to show a specific integration today, because it's quite ingenious and allows one to integrate a function that would otherwise be very difficult.

But first, a little context. The integrals that one sees in quantum mechanics are essentially known as probability density functions. The idea is that, at each value of the function, one has an associated probability density. Multiplying this by a small interval $dx$ gives one a probability. This also means that any one point doesn't have a probability. Instead, one requires an *interval* in order to get a probability. Formally, we get the following:

$$
\begin{equation}
	P(a \le x \le b) = \int_a^b f(x) dx.
\end{equation}
$$

Additionally, we have some properties that we want for our probability. First, we want any probability to be greater or equal to zero, and second, we want the probability over the whole space that we are interested in to add up to one. These are reasonable requirements if we want to capture what we mean by probability when talk about it in everyday life.

What this second condition usually means though is that we have to *normalize* a function. We have to integrate over the whole space, and introduce a constant such that the integral then gives one.

This is where my quantum mechanics assignment comes in. I had to normalize what is known as the Gaussian distribution, and the integral looks like this:

$$
\begin{equation}
	\int_{-\infty}^{\infty} A e^{-\lambda x^2} dx = 1.
\end{equation}
$$

My job was to solve for the constant *A*. At first glance, this integral doesn't look too bad. However, after a few moments, you'll realize that this isn't as easy as it looks. Indeed, the only way I know of to solve this is to use neat trick. To start, we'll square both sides of the equation. Since the one won't change, let's just look at how the left-hand side changes.

$$
\begin{equation}
	\left( \int_{-\infty}^{\infty} A e^{-\lambda x^2} dx \right)^2 = \left( \int_{-\infty}^{\infty} A e^{-\lambda x^2} dx \right) \left( \int_{-\infty}^{\infty} A e^{-\lambda x^2} dx \right).
\end{equation}
$$

This might not seem any better, but what if we change one of the variables of integration on the right-hand side? If we go from $x$ to $y$, we get the following:

$$
\begin{equation}
	 \left( \int_{-\infty}^{\infty} A e^{-\lambda x^2} dx \right) \left( \int_{-\infty}^{\infty} A e^{-\lambda y^2} dy \right) = \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} A^2 e^{-\lambda (x^2 + y^2)} dx dy.
\end{equation}
$$

Now everything is coming together. If you've taken a calculus course and seen other coordinate systems, you should immediately recognize this to be a good candidate for switching into polar coordinates. Doing so gives us the following:

$$
\begin{equation}
	 \int_{0}^{2\pi} \int_{0}^{\infty} A^2 e^{-\lambda r^2}r dr d\theta.
\end{equation}
$$

This is something that is much easier to integrate, since we have the factor of $r$ in the denominator. Performing the integration gives us:

$$
\begin{equation}
	 \int_{0}^{2\pi} \int_{0}^{\infty} A^2 e^{-\lambda r^2}r dr d\theta = 2\pi A^2 \left[ \frac{-1}{2\lambda} e^{-\lambda r^2} \right]_0^{\infty} = -\frac{\pi A^2}{\lambda} \left[ 0-1 \right] = A^2\frac{\pi}{\lambda}.
\end{equation}
$$

This is quite a nice expression, because we know that this is equal to one (from the fact that we need the equation to be normalized to one). Therefore, we get $A = \sqrt{\frac{\lambda}{\pi}}$.

Without squaring our original integral, it would have been *very* difficult to evaluate. However, by seeing this clever workaround, we were able to turn a difficult integral into one we could evaluate without too much trouble.

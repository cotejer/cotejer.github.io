---
id: 540
title: Variations on Simple Harmonic Motion
date: 2017-01-13T02:22:00+00:00
author: CJeremy
layout: post
guid: https://blog-cjeremy.rhcloud.com/?p=540
permalink: /2017/01/13/variations-on-simple-harmonic-motion/
categories:
  - Uncategorized
---
In the [last post](http://blog-cjeremy.rhcloud.com/2016/12/23/simple-harmonic-motion/), we looked at the basics of simple harmonic motion, and how the equations is described because of the spring force being applied to the system.

However, we can generalize this much further. In our initial analysis, we assumed that there a frictionless surface for the mass to slide on. Obviously, that doesn&#8217;t happen, so we need to add in some frictional force. For simplicity, we will assume that the frictional force is proportional to the speed of the mass, and so will come into the form $-bv$, where $b$ is just a constant that will be specified in the initial conditions.

Additionally, we had the setup such that we pulled the mass and then let it go for as long as we liked. In reality though, we could _supply_ an external force, which (along the axis of motion) we will assume is another sinusoidal function that is given by: $F\_0 sin(\omega\_d t)$.

Careful observers will notice that $\omega_d$ is not the same as the one we had in the last post. This is because the angular frequency will change due to the periodic applied force. An easy way to imagine this is if you&#8217;re pushing a swing. Initially, you push the swing as it is swinging back to the centre, and you do this one time each period. Imagine that period is two seconds. Then, if you start making your pushing motion every second instead of every _two_ seconds, the swing won&#8217;t keep on going like it normally was. Instead, the swing wants to keep swinging at a period of two seconds while _you&#8217;re_ pushing every second. Eventually, you will win out and the swing will swing at the rate of once per second.

Let&#8217;s now dig into the mathematics of this motion. Last time, we had the following equation:

$$m \frac{d^2x}{dt^2} + kx = 0$$

Now, we add our frictional force and the external applied force to get:

$$m \frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = F\_0 sin(\omega\_d t)$$

$$\frac{d^2x}{dt^2} + \gamma \frac{dx}{dt} + \omega\_0^2 x = F\_0 sin(\omega_d t)$$

Using the same method as last time, we can solve the homogeneous part of the differential equation by writing out characteristic equation:

$$r^2 + \gamma r + \omega_0^2 = 0$$
  
$$r = \frac{-\gamma \pm \sqrt{\gamma^2 &#8211; 4\omega_0^2}}{2}$$

This gives us a host of conditions depending on our values of the discriminant in the above equation.

If $\gamma^2-4\omega_0^2 = 0$, then $r = \frac{-\gamma}{2}$, which is a repeated root.

For a repeated root, we must add a factor of $t$ into one of our solutions, making the solution:

$$x(t) = e^\frac{-\gamma t}{2}(At+B)$$

If $\gamma^2-4\omega\_0^2 \gt 0$, then $r\_1 = \frac{-\gamma + \sqrt{\gamma^2-4\omega\_0^2}}{2}$ and $r\_2 = \frac{-\gamma &#8211; \sqrt{\gamma^2-4\omega_0^2}}{2}$.

The solution is therefore:

$$x(t) = Ae^\frac{(-\gamma + \sqrt{\gamma^2-4\omega\_0^2})t}{2} + Be^\frac{(-\gamma &#8211; \sqrt{\gamma^2-4\omega\_0^2})t}{2}$$

Finally, if $\gamma^2-4\omega\_0^2 \lt 0$, we get a system that has complex roots given by $r = \frac{-\gamma \pm \sqrt{4\omega\_0^2-\gamma^2}i}{2}$. Note how the terms inside the square root are switched around, which happens because we factored out a $-1$ and wrote $\sqrt{-1}=i$.

This solution for the characteristic equation has the form $r = \lambda \pm \mu i$, so the solution is:

$$x(t) = Ae^{\lambda t}sin( \mu t) + Be^{\lambda t}cos( \mu t)$$

So those are your three cases, but this doesn&#8217;t even take into account the \*external\* force. If you remember from above, we were trying to solve the homogeneous portion of our differential equation, which is when the equation is equal to zero. We now need to tackle the right-hand side of the equation.

To do this, I like to use the method of undetermined coefficients. To me, this method is one that involves a little bit of skill at times, but is useful because it&#8217;s all about guessing. Essentially, we want to try and guess the form of the solution given that the external force is a sinusoidal function. Thankfully, this knowledge is of great help, because we know the derivatives of sines and cosines flip back and forth and become negative, possibly cancelling out in the final solution. Therefore, I propose a solution of the following nature:

$$x(t) = Acos(\omega\_d t) + Bsin(\omega\_d t)$$

Note that I&#8217;ve only chosen $\omega_d$ because it matches the non-homogeneous part.

Taking derivatives, we get:

$$x'(t) = -A \omega\_d sin(\omega\_d t) + B \omega\_d cos(\omega\_d t)$$
  
$$x&#8221;(t) = -A \omega\_d^2 cos(\omega\_d t) -B \omega\_d^2 sin(\omega\_d t) = -\omega_d^2 x(t)$$

Substituting our equations for $x(t), x'(t), x&#8221;(t)$ into the differential equation gives us:

$$ -A \omega\_d^2 cos(\omega\_d t) -B \omega\_d^2 sin(\omega\_d t) -A \gamma \omega\_d sin(\omega\_d t) + B \gamma \omega\_d cos(\omega\_d t) + A \omega\_0^2 cos(\omega\_d t) + B \omega\_0^2 sin(\omega\_d t) = F\_0 sin(\omega\_d t)$$

We then can group the expression into sines and cosines.

Cosines:

$$ (-A \omega\_d^2 + B \gamma \omega\_d + A \omega\_0^2) cos(\omega\_d t) = 0$$

$$A(\omega\_0^2 &#8211; \omega\_d^2) + B\gamma \omega_d = 0$$

And sines:

$$ (-A \gamma \omega\_d + B \omega\_0^2 &#8211; B \omega\_d^2) sin(\omega\_d t) = F\_0 sin(\omega\_d t)$$

$$ -A \gamma \omega\_d + B (\omega\_0^2 &#8211; \omega\_d^2) = F\_0 $$

Solving for these coefficients through substitution gives use these two lovely expressions:

$$A = \frac{- \gamma \omega\_d F\_0}{(\omega\_0^2 &#8211; \omega\_d^2)^2 + (\gamma \omega_d)^2} $$

$$B = \frac{F\_0 (\omega\_0^2 &#8211; \omega\_d^2)^2}{(\omega\_0^2 &#8211; \omega\_d^2)^2 + (\gamma \omega\_d)^2} $$

Most of the time, you&#8217;re not going to _actually_ use these equations to solve the problem. It&#8217;s often easier to solve the characteristic equation and make sure the initial conditions are satisfied instead of just blindly using these formulas. You can also rearrange them to use slightly different variables, but the end product is the same. What&#8217;s interesting to note about this kind of forced oscillation is that you may notice that the homogeneous solution dies off over time. This means that the natural frequency $\omega_0$ is only relevant in the beginning. After a certain amount of time, it&#8217;s effects die off and the non-homogeneous part of the solution becomes more important. This coincides with our expectations. If you keep pumping a system with a different frequency, it will eventually match the one you&#8217;re pumping with, regardless of what it started with.

So that&#8217;s probably enough to keep your mind thinking for a while. These systems can be quite complex, and there&#8217;s a whole host of situations that can come out of it. I&#8217;ll leave it here though, and we&#8217;ll look at a slightly different wave topic next time, which is interference.
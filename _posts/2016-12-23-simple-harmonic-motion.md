---
id: 504
title: Simple Harmonic Motion
date: 2016-12-23T02:12:00+00:00
author: CJeremy
layout: post
guid: https://blog-cjeremy.rhcloud.com/?p=504
permalink: /2016/12/23/simple-harmonic-motion/
categories:
  - Uncategorized
---
If you&#8217;ve ever taken a physics class on waves, the first type of mathematical wave you learn is the one due to what is called simple harmonic motion. The idea is pretty simple, so I&#8217;ll go through a rough derivation here.

First, we imagine what the situation looks like. It&#8217;s usually shown as a mass attached to a spring moving along an idealized (read: frictionless) surface, as shown below:

<div id="attachment_506" style="width: 310px" class="wp-caption aligncenter">
  <img class="size-medium wp-image-506" src="https://i1.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2016/12/Ideas-14-300x225.png?fit=300%2C225" alt="" srcset="https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2016/12/Ideas-14.png?resize=300%2C225 300w, https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2016/12/Ideas-14.png?resize=768%2C576 768w, https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2016/12/Ideas-14.png?w=1024 1024w" sizes="(max-width: 300px) 100vw, 300px" data-recalc-dims="1" />
  
  <p class="wp-caption-text">
    Idealized situation with only the force of the spring coming into play.
  </p>
</div>

As we can see, there is only one force acting on it: the force of the spring, $\textbf{F}_s$. This force is proportional to the displacement $x$ of the mass attached to the spring and is known as Hooke&#8217;s Law. Therefore, if we write out the forces that act on this body using Newton&#8217;s second law, we get (along the x direction):

$$\Sigma F = m a$$
  
$$F_s = ma$$
  
$$-kx = ma$$
  
$$ma + kx = 0$$
  
$$m\frac{d^2x}{dt^2} + kx = 0$$

Once we&#8217;re at this point, we need to figure out what the solution to this second order differential equation is. I won&#8217;t go into full detail here, but you can use a bunch of different methods to solve for the function _x_ we are looking for. You won&#8217;t need to solve the equation each time, since doing it once will give us the pattern we need in order to describe simple harmonic motion for all situations.

I&#8217;ll use the method of writing down our characteristic equation and solving.

$$mr^2+k=0$$
  
$$r^2+\frac{k}{m}=0$$
  
$$r=\pm i\sqrt{\frac{k}{m}}$$

We give the quantity $\sqrt{\frac{k}{m}}$ another variable name: $\omega$. This is called the _angular frequency_, and is measured in radians per second.

From here, our solution is given by:

$$x(t) = Acos(\omega t + \phi) + Bsin(\omega t + \phi)$$

For most applications that we use in physics, _B_ ends up being zero. Additionally, $\phi$, which is just the phase constant and adjusts where the function begins, is often zero too. This means we are left with a rather simple equation that accurately describes how an idealized version of a mass moving on a spring would work.

But I don&#8217;t want to stop there. Instead, I want to show you _another_ way of looking at how we describe simple harmonic motion. In particular, look at the form of our solution to the differential equation. It&#8217;s a combination of trigonometric functions, which we know can describe something else: a circle.

## Simple Harmonic Motion through Uniform Circular Motion

At first glance, these two ideas might seem to have _nothing_ to do with each other. Circular motion goes round and round while our simple harmonic motion situation only goes up and down or side to side. What can they possibly have in common?

(Before I dive into it, I just want to note that this is one of the coolest things I saw in my waves and optics class when I had to take it.)

First, we will build up our experiment before I show you the mathematics of it. Imagine you have a circular disc that is rotating at a constant rate on a table. Now, attach a small object somewhere along the circumference of the disk so that it spins with the disk. This means that the object on the disk is exhibiting uniform circular motion. Next, place a screen behind the rotating disk. Finally, we shine a light edge on to the disk so that its shadow is displayed on the screen behind it.

What do you think you will see? What will the object that is rotating on the disk look like on the screen?

The answer isn&#8217;t that the object will move from one side to the other at a constant rate. Instead, it will move faster in the centre and slower on the ends before it turns around. Effectively, it will look just like simple harmonic motion!

Because I know you are just _craving_ to see what this looks like outside of your mind&#8217;s eye, here you go:



(A brief note: I did not make this myself. I found it on the Desmos site, and I unfortunately could not find the author. If you know who made it or if it is yours, please reach out to me and I&#8217;ll add your name to it. Also, press the &#8220;play&#8221; button on the &#8216;a&#8217; in the calculator for it to start.)

The red function you see moving from left to right is the function given by simple harmonic motion that we saw above. It&#8217;s moving simply to show how the function lines up with the circular motion.

In the centre, we can see a point on the circle moving round and round through uniform circular motion. At the same time, there are two vertical lines in yellow acting as &#8220;screens&#8221; on each side. Notice the horizontal line connecting the point on the circle with the point on the screen. This is exactly what would happen if we shone light onto an object and have projected it onto the screen.

That&#8217;s a very nice way of viewing it physically, but what about mathematically? What is that screen? In essence, it&#8217;s the _projection_ of the circle on the vertical axis. Imagine squishing the circle such that it creates a vertical line. That&#8217;s the role of the screen. Put another way, if we define the circle parametrically as $(cos\theta, sin\theta)$, we get the projection on the vertical axis by only looking at what happens to the y-component of the parametric curve and setting the x-component to zero.

And now, we have two ways of looking at simple harmonic motion. We can either view it as the physical motion, or as a projection of uniform circular motion onto a straight line (and since we&#8217;re dealing with a circle, you could project the circle onto any line you wanted).

* * *

Hopefully, this gives you a better idea of the basics of simple harmonic motion and how it relates to uniform circular motion. In the future, I&#8217;m going to go into detail on what happens when we add more forces to the system, since physical systems are never (or rarely ever) idealized.
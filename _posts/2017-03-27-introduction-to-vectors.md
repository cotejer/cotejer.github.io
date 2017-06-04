---
id: 615
title: Introduction to Vectors
date: 2017-03-27T02:32:00+00:00
author: CJeremy
layout: post
guid: https://blog-cjeremy.rhcloud.com/?p=615
permalink: /2017/03/27/introduction-to-vectors/
categories:
  - Uncategorized
---
If you were talking to a friend about the drive you made this morning, you might tell them something along the lines of, &#8220;I drove from my place to hear in about an hour, going east for the entire time.&#8221; Your friend, who knows where you live and has a rough idea of the route to get to where you both are, understands implicitly that you don&#8217;t really mean that you went and drove in one direction only for the entire hour. After all, you first had to exit the property of wherever you were parked, then you probably had to navigate through the neighbourhood of where you live, before finally getting onto a highway or a direct route to your destination. It&#8217;s only at that point that you actually began going east. Before then, you may have driven in all directions, for varying amounts of time.

In physics, we call this route a trajectory. It&#8217;s how you move from one place and get to another. In order to describe the specific trajectory of your drive, we would have to do a lot of specifying, since your trajectory was complicated. But we&#8217;ll start off much more simply. Bearing in mind the impossibility of it all, imagine you just had a single block moving in a straight line, like so:

<img class="alignnone size-full wp-image-611" src="https://i1.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/Image-2017-03-26-5-00-PM.png?resize=1000%2C750&#038;ssl=1" srcset="https://i1.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/Image-2017-03-26-5-00-PM.png?w=1024 1024w, https://i1.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/Image-2017-03-26-5-00-PM.png?resize=300%2C225 300w, https://i1.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/Image-2017-03-26-5-00-PM.png?resize=768%2C576 768w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />

In this case, it&#8217;s quite a bit easier to describe how the route of this block will change over time. You don&#8217;t even need to be that great with the mathematics of it all for common sense to tell you that the block will move a distance d from wherever it is now by multiplying the speed at which it is moving and the time it travelled. If the block was moving at $5m/s$ and went for $3.5 s$, we would expect for it to move a distance of $d = (5m/s)(3.5s) = 16.5 m$.

<img class="alignnone size-full wp-image-612" src="https://i0.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0068.png?resize=1000%2C750&#038;ssl=1" srcset="https://i0.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0068.png?w=1024 1024w, https://i0.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0068.png?resize=300%2C225 300w, https://i0.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0068.png?resize=768%2C576 768w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />

This is a simple, but profound idea. We can figure out how far something has travelled by knowing its speed and multiplying it by the amount of time it has travelled for. Simple, right?

Unfortunately, that&#8217;s not quite the whole story. As you will see, a lot of learning mathematics is about understanding the special case, before moving on and getting more general. It&#8217;s the same story here. In the above example, it was easy to figure out where the block will be after a certain amount of time. Just multiply speed with time! But what if I asked you to look at this:

<img class="alignnone size-full wp-image-614" src="https://i0.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0069.png?resize=1000%2C750&#038;ssl=1" srcset="https://i0.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0069.png?w=1024 1024w, https://i0.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0069.png?resize=300%2C225 300w, https://i0.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0069.png?resize=768%2C576 768w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />

It isn&#8217;t so easy to figure out how far the cannonball will travel in a certain amount of time, even if you know how fast it is to start with. Common sense will once again tell you that, no matter how hard the cannon fires upwards, the ball will eventually fall back down to the ground. As such, the speed the cannonball is moving will change over time. Therefore, we will need a more sophisticated tool to analyze situations like these.

That tool is the vector.

What is a vector? Well, it&#8217;s a question that means something slightly different depending on if you&#8217;re a physicist, a mathematician, or a computer scientists. For our uses, the most practical way of thinking about a vector is as an arrow. The straight arrows you saw in the above pictures can be considered vectors.

The two main parts of a vector are its magnitude and direction. Direction means exactly what you think it means. In the above examples, the vectors I drew were pointing in the general right direction. So when we were talking about the block and I said it was moving $5m/s$, it would have been more accurate to say, &#8220;It&#8217;s moving $5m/s$ to the right.

The magnitude of a vector simply means the absolute value of the quantity we&#8217;re talking about (we always write magnitudes to be positive). In the first example, the speed of the block was $5m/s$, so that was its magnitude. However, these quantities don&#8217;t have to be fixed. Consider again the cannon scenario above. As soon as the cannonball leaves the chamber of the cannon, its speed is changing all the time (and, for that matter, so is its direction). As such, it&#8217;s a good idea to remember that while we will start with vectors that don&#8217;t change with time, there will come a point in which it is useful to use time.

But how is this helping us with the mathematics?

Fine, I told you about vectors, but how do we describe these situations with vectors? Isn&#8217;t it awfully vague to talk about something like a direction?

You&#8217;re absolutely right. To help, we need to use a tool that began with Descartes and is invaluable useful today. It&#8217;s a way to visualize what is happening in a system, so we don&#8217;t have to resort to only writing down equations. I&#8217;m talking about, of course, the Cartesian plane, where you&#8217;ve undoubtedly seen how to graph things like $y = 6x$ and the like. But now, you&#8217;ll find that it&#8217;s a fantastic tool for studying vectors.

Let&#8217;s go back to the example with the block, but this time, I&#8217;ll overlay a grid near the block so we can describe the situation more accurately:

<img class="alignnone size-full wp-image-613" src="https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0070.png?resize=1000%2C750&#038;ssl=1" srcset="https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0070.png?w=1024 1024w, https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0070.png?resize=300%2C225 300w, https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/03/IMG_0070.png?resize=768%2C576 768w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />

From now on, you&#8217;re going to start thinking about space as a sort of grid system. Here, there are two directions: the $x$-direction, and the $y$-direction. Of course, you can go in a combination of these two directions, as the cannonball was doing before. But now that we have this grid system, we easily describe both the magnitude and the direction of any vector. Notwithstanding my bad drawing, the vector above has a magnitude of $5m/s$, and its direction is along the positive $x$-axis. In general, we measure the direction (or angle) of the vector by starting on the positive $x$-axis and rotating counterclockwise until we get to the direction that the vector is pointing.

This is all well and good, but I know that many of you are observant, and might ask, &#8220;If we have a vector going diagonally, can we describe it by talking about how much it moves in the $x$ direction and how much it moves in the $y$ direction?&#8221;

The answer is yes!

This highlights an important part of vectors: we can decompose them into their constituent parts. While it might be difficult to think about a certain motion in three dimensions, it&#8217;s much easier to think of the motion with a component in each of the $x$, $y$, and $z$ directions. Then, we can calculate things along each of those directions, before finally packaging everything up in the end to give a vector description of the motion.

(I want to take a second to mention that, of course, you can generalize the notion of what a vector is and what kinds of things you can do with them. This generalization usually leads you to the area of linear algebra, but we will focus for now with regular vectors that you can visualize as arrows, either in two or three dimensions.)

We will slowly build up to some interesting interesting results with these vectors, but I want to specify that I&#8217;m going to try and bring the logic and thinking behind a lot of these concepts from the perspective of someone who is looking to do physics. It can be all well and good to take a mathematician&#8217;s or computer scientist&#8217;s approach, but we&#8217;ll leave that to the side for now.

* * *

At this moment, you might be wondering something along the lines of, &#8220;Are these vectors really going to be that useful in physics?&#8221; The answer is a resounding _yes_. It may seem like vectors are only useful for describing the paths of bodies being launched, but the truth is that vectors are used all over the place. We use them to describe the equations of motion of bodies, the way electric and magnetic fields work, and basically anything that you can describe with the notion of forces. So basically all of physics, really.

For now, I just want you to take this initial point away: vectors specify magnitudes and directions, and we can add and subtract them component-wise in order to figure out how vectors interact with each other.
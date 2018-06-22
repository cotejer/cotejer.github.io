---
title: The Distance Formula (Equation Explainer)
author: Jeremy
permalink: 2017/08/21/distance-formula
date: 2017-08-21
---

The distance formula is one of the most frequently used relations in physics, allowing us to decompose a variety of vectors into different components. It's something that every physics student uses, and so it becomes second-nature for most of us. However, I've come across the sad fact that many secondary schools don't seem to teach how the distance formula comes about and its connections with earlier work. As such, the link between algebra and geometry is lost and the distance formula gets lost in calculating differences between $x$ and $y$. Here, the goal is for us to look at the distance formula and see how it relates to other concepts that are of much use.

## Algebra

In secondary school, students are presented with a formula that is supposed to give the distance between two points on a graph:

$$d = \sqrt{(x_{2} - x_{1})^2 + (y_{2} - y_{1})^2}$$

In my mind, this is a bit of an intimidating formula. There are several moving parts (variables), and it looks like you have to keep everything in check in order to get the distance right. As such, I find that almost no student actually remembers this formula without consulting their memory aid. It's finnicky, and it seems like one wrongly placed number will make everything go haywire[^1].

However, what is important here is that the formula isn't very illuminating to the student. I wouldn't say it's necessarily because the formula is "ugly" (which is subjective), but that it isn't explained. To see the formula properly, it's critical that we don't only look at the algebra, but that we also draw some sketches.

## Graphical

Let's set up our problem. Given two points $A$ and $B$, we want to find the distance between these points when we draw a straight line between them. We can represent this as such:

![](/images/two-points.png)

In our sketch, we simply have the two points that are placed in a regular Cartesian plane. Now, we know that the equation for the distance between points $A$ and $B$ is what we saw above, but what many students don't see is that this equation can be seen *from* the graph. It's not a magical formula that one gets independent of the graph. The formula is intimately tied to geometry. To make this suggestive, let me draw a few extra lines on our graph:

![](/images/construction.png)

So how does this help us? Well, one thing you might notice is that if we connect the two points by a straight line, the length of that line is what we want. Furthermore, when we take this line with the other two I have drawn, we get a right triangle.

![](/images/triangle.png)

If there's one thing I'm hoping that you remember, it's that we have a *very* special relation between the three sides of a right triangle: the Pythagorean theorem. This is the quintessential secondary school formula, and I bet you can recite this one from memory. It's given by $a^2 + b^2 = c^2$, where $a$ and $b$ are the legs of the triangle and $c$ is the hypotenuse.

But what I want you to see is that it's *exactly* this relation that gives us our distance formula! If you look again at the lines I drew in our graph, we just need to find the two legs in order to compute the hypotenuse, which is our distance $d$. It might look like we don't have the information to do this, but if we inspect our points closer, you'll find that we do.

Start with the green side. For simplicity, let's suggestively call it $\Delta y$, since I think you would agree that we are looking at the change in the $y$ coordinate. The length for this leg of the triangle is simply how much the $y$ coordinate changes when we go from $A$ to $B$. Note here that when we talk about a *length*, our measurement is positive. This means that, even if point $B$ is lower than point $A$, we still say that the length is positive[^2].

We can apply a similar argument for what I'll call $\Delta x$, and this will give us a picture that looks like this:

![](/images/deltas.png)

Finding the distance between $A$ and $B$ is now a piece of cake. Since we know the two legs, we can apply the Pythagorean theorem to get:

$$ (\Delta x)^2 + (\Delta y)^2 = d^2.$$

Solving for $d$ gives us:

$$d = \sqrt{(\Delta x)^2 + (\Delta y)^2}.$$

The final thing to do is find an expression for $\Delta x$ and $\Delta y$. This isn't as difficult as it may look, because one thing we *do* know about this problem is where $A$ and $B$ are (which means we know their coordinates). Therefore, if we let $A = (x_1, y_1)$ and $B = (x_2, y_2)$, we know that $\Delta x = x_2 - x_1$ and $\Delta y = y_2 - y_1$. Putting this into our expression for $d$ gives us:

$$d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}.$$

This is exactly the expression you probably have somewhere on your memory aid, but now you know *why* it's there. When we compute the distance between two points in the plane, what we are *really* doing is chopping that distance into a new path, one that gives us the legs of a right triangle. Then, using geometry we're used to, we work backwards to find the original distance we are looking for. There's no magic here, just geometry.

## Three Dimensions

You might now be wondering what the distance formula would be in *three* dimensions. Well, I'm not going to go through a whole rigourous proof, but here's the idea. Imagine we have the following situation where we want to find the distance between the origin $O$ and another point $A$ (I'm using the origin just for a bit of added simplicity).

![](/images/three-dimensions.png)

Hopefully you can see that the distance now occupies three dimensions, which I've denoted as $x$, $y$, and $z$. The algorithm is then simple. First, we compute the distance that lies on the $x-y$ plane, as shown below (the solid orange line). Note that I've once again used $\Delta x$ and $\Delta y$ to denote the side lengths.

![](/images/distance-x-y.png)

Now that we have the length between along the plane, we can now simply extend this to our third dimension using the Pythagorean theorem.

![](/images/distance-3d.png)

Putting these steps together, we can see that the distance between a point given by $A = (x_0, y_0,z_0)$ and the origin $O$ is given by:

$$d = \sqrt{x_0^2 + y_0^2 + z_0^2}.$$

This is then easily modified for any two points, by simplying replacing every squared term by the difference of the coordinates, such as $(x_1 - x_0)$.

## Going Up in Abstraction

Now that we've covered our physical dimensions, we might start asking what seem like more difficult questions, such as:

*What's the distance between two points in 4 dimensions? What about $n$ dimensions?*

This isn't a distance you can visualize, of course (unless you're very good at visualization). We are limited by three dimensions, but the good news is that the mathematics doesn't care if we work in one, two, three, or $n$ dimensions. It turns out that we can just continue applying the procedure that I outlined above for any number of dimensions you are insterested in. Therefore, we can write the distance between two points given by $A = (x_1, x_2, x_3, ... , x_n)$ and $B = (y_1, y_2, y_3, \ldots , y_n)$ is:

$$d = \sqrt{(x_1 - y_1)^2 + (x_2 - y_2)^2 + (x_3 - y_3)^2 + \ldots + (x_n - y_n)^2}.$$

In other words, just keep on applying the difference between the two points and squaring the result to get the distance in any dimension.

---

So why does this work? Or rather, did I just get lucky in the way that I drew my graph that the lines came out to be a right triangle?

The answer is no. I didn't choose the lines randomly. If you look back at the graph, the lines I drew in are parallel to to the axes. What this does is guarantee two things. First, it ensures that we can easily calculate the distance along either the horizontal ($\Delta x$) line or the vertical ($\Delta y$) line. The second thing is that, by drawing our lines parallel to the $x$ and $y$ axes, the two lines are perpendicular (orthogonal), which means the triangle we get is a right triangle, just what we need to use the Pythagorean theorem.

I hope this makes the distance formula seem a bit more clear. The formula comes directly from the geometry of the situation, which I have demonstrated here. As such, the only thing to remember is that we need to use the Pythagorean theorem to find the distance between two points. After that, everything is a piece of cake.

[^1]: To assuage this fear a bit, I want to point out a property of a term that looks like $(a-b)^2$. We know that the only difference between $a-b$ and $b-a$ is that one will be negative and one will be positive (we're assuming they aren't the same number), but the *absolute value* is the same. Now, if we square this term, the result is always positive (a property of squaring a number). Therefore, the lesson I want to impart here is that the order of $x_{1}$ and $x_{2}$ don't matter, since we are squaring the result.
[^2]: So why are lengths always positive, even though we know our $\Delta y$ or $\Delta x$ may be negative? I explained to you the "physical" way of thinking about it (I often think in the way of my background in physics), but this is also encoded mathematically in our distance formula. When I presented these two "extra" lengths in our graph, you agreed with me that they were $\Delta x$ and $\Delta y$. However, if you think about it, each of *those* line segments should be able to be computed using our distance formula, and indeed they can. If we take $\Delta x$ as an example, we know that $y$ does not change as we move along this line, so the distance formula gives $d = \sqrt{(\Delta x)^2} = \Delta x $. Note here that it doesn't matter if $\Delta x$ is negative, since you have to first square it, and then take the square root. This has the pleasant effect as of taking care of the issue with signs, so you don't have to worry, and it matches our physical intuition about lengths being positive.
---
title: Dimensions of Objects
author: Jeremy
permalink: /dimensions
date: 2018-01-29
---

Here's an interesting question: what *is* a dimension? Dimensions can often seem like life. We know it when we see it, but defining it can be kind of tricky. As such, a good heuristic can be useful in thinking about dimensions, and, in particular, the number of dimensions a particular mathematical object has.

If I give you a point $(x,y)$ in the plane, what would you say is the dimension of that point?

It's tempting - *so* tempting - to say that the answer is two. That's almost my initial reaction just looking at the question. In fact, if I gave you the point within the plane, I think it's fair to say that your reaction would be to say that the its two-dimensional.

![](/images/pointInPlane.png)

You might say, "But I need to give you two coordinates to specify that point! As such, it has to be two-dimensional, or else I wouldn't need those coordinates." However, this is a mistake. Or, more precisely, a mix up.

The issue lies with how we are viewing the objects. When I gave you the point, I *placed* it in the two-dimensional plane. This is important. The plane *itself* is two-dimensional. However, the objects that go *inside* of it don't have to be two-dimensional. In fact, they can be two-dimensional, one-dimensional, or zero-dimensional. A two-dimensional object could be a disk (which is a filled-in circle), a one dimensional object could be a function, and a zero-dimensional object would be a point.

![](/images/objectsInPlane.png)

The confusion lies in the fact that we have two things in play here. First, we have some sort of space, which is where we say our mathematical objects "live". In our example, this is the plane, which is two dimensional. However, we can then place (or *embed*) various objects into that space, and these objects can have dimensions that are equal to or less than the dimension of the space. This is exactly the situation we find ourselves in when we talk about a point in the plane.

The lesson we learn is that the number of dimensions a mathematical object has *isn't* necessarily the same as the dimension of the space it lives in. So how do we think about the dimension of a point? Well, you have to try and do the difficult task of thinking about it *without* any associated space around it. This isn't easy, but the following question makes things clearer. How many ways can you "move around" on a point? The answer is zero, since you can't move anywhere else! There's only one point, so you have to stay there at that single point. As such, the dimension of a point is zero. It doesn't matter if it lives in a three-dimensional space or a two-dimensional one. The dimension of the point will still be zero.

Note that there *are* objects which can superficially seem like points (called vectors), but they aren't points and so they aren't zero-dimensional.

A good heuristic to get a sense of the dimension of an object is to imagine yourself as a tiny creature living on the object. Which ways can you move? If you're on a line or some sort of curve, you can only move forward and backward along that curve. As such, you can only move within one dimension and so the object is one-dimensional. If you were on a surface (say, of a sphere), you could move left and right, *and* forward and backward. Therefore, the surface would be considered two-dimensional. We still think of the sphere as something that *lives* in three dimensions, but as its own entity, it's two-dimensional. In other words, when you are on the surface, you only need two coordinates to specify your location. It doesn't matter if your surface is also within a seventy-four-dimensional space. The surface itself is the same, and it's still two-dimensional.

---

Like I said above, the heuristic of imagining what it would be like to move around on the object itself is a useful strategy to think about the number of dimensions a mathematical object has. As long as you keep in mind the fact that objects can be embedded within higher-dimensional spaces, there won't be any more confusion as to what the object's dimension is. Remember, the object can exist independently from the space it lives in, and *that* is the dimension of the object.
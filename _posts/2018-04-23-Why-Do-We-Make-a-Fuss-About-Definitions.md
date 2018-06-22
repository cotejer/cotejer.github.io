---
title: Why Do We Make a Fuss About Definitions?
author: Jeremy
tags: Mathematics
permalink: /importance-of-definitions
date: 2018-04-23
---

If you've ever taken a mathematics course, chances are that you've seen how definitions are one of the common items on the board. Definitions form the heart and soul of mathematics. They allow us to pose problems in very precise ways, yet they are the bane of many students, who get back their assignments and see that points were deducted because things that seemed "minor" and weren't included were in fact quite important.

There's a case to be made that the details aren't always so important, but mathematics is a bit of a special case, because when one wants to refine their arguments, it's *critical* to have clear definitions. Without them, there's a good chance that you can get stuck trying to convince others of the veracity of your claims. Additionally, it turns out that while we have a pretty good intutition about many mathematical properties, *capturing* these properties can be more difficult than it seems at first.

For example, what would you tell me if I asked you to define a circle? Really, what would you say? Of course, we all know what a circle *is*, so you might draw one for me. But, I insist on you giving me a definition that I could apply to any shape I drew, without you there to tell me if it was a circle or not.

Perhaps you would say that a circle is the shape with only one side. That seems reasonable, and is certainly true for the circles I know of. So I draw this:

![](/images/fakeCircle.png){:.centre-image}

Evidently, this is not what you were talking about.

"No egg shapes!" you say. But then I might draw you something else, such as an ellipse or the shape that a running track makes. What about those shapes? Or what about more complicated shapes that still have one "side", but aren't circles?

As you can see, this is quickly becoming a much more difficult problem than what it should be. I mean, we *should* be able to define a circle without any problem! It's not exactly the most sophisticated shape in existence. However, the problem is that none of the above proposed definitions *solely* capture the notion of a circle. They do define sets of objects with a certain property, but the sets aren't restricted to only circles.

![](/images/vennDiagramCircle.png){:.centre-image}

This is an important realization, because it points us to the right definition of a circle. What we want is a definition that includes only circles, *and* all circles. Both the "only" and the "all" are important. What we are looking for is the defining characteristic of a circle (of course, there could be more than one, and so we would have a list of such characteristics).

After a bit of investigation and drawing shapes that are both circles and shapes that are close to circles, an important property that will be found is that a circle has a *radius*. This isn't just a random sort of measurement on a circle. What you might notice is that that the radius is the distance that *any* point on the circle has from the centre of the circle. If you compare this to any other shape you drew that wasn't a circle, you will quickly realize that only the circle has this property. As such, this seems like a good candidate for a definition of a circle.

Therefore, we define a circle to be the *(x,y)* points that are exactly a distance *r* from a chosen point (the centre of the circle). Go ahead and try out these definitions on the shapes you know of. Is it satisfied *only* for circles, and does it include all of them? You will find that yes, this definition does indeed work.

What we've done here is an important phenomenon in mathematics, which is to abstract or "boil down" some sort of structure to its essence. Frequently, mathematicians begin with some sort of structure that is familiar or intuitive to them, and then they ask, "What is the essence of this object?" From there, mathematicians come up with the appropriate definitions to talk about their chosen object of study.

You might notice that our definition of a circle doesn't talk about being round. This suggests that being round isn't necessarily "fundamental" to being a circle. (Though, we know that graphically, their curvature is apparent.) Instead, the fundamental essence of a circle seems to be its centre, and the distance *r* at which all points are away from the centre. In other words, if I wanted to describe any circle to you, I only have to specify two things: its centre and radius. With those two parameters, you can exactly reconstruct the circle I was imagining, even if you didn't see what I had beforehand.

## Good definitions admit further explorations

Another consequence of a good definition is that it enables further avenues of exploration. To continue with our study of the circle, it turns out that the circle is only a special case of a more general class of objects, called *n*-spheres. Here, *n* is the dimension of the object itself (and is greater than or equal to zero), so the circle we are working with is a one-sphere, since the circle is simply a one-dimensional curve. (Remember, a circle is only the *boundary* of the object. If we were talking about the area inside, it would be called a *disk*[^1].) The definition of the *n*-sphere is a straightforward generalization of our definition for a circle. A *n*-sphere is the set of points *(x<sub>1</sub>, x<sub>2</sub>, &#8230;, x<sub>n+1</sub>)* which are a distance *r* from a centre point.

Let's look at the two other familiar examples. What is the zero-sphere? Well, it's the set of points *(x)* which are a distance *r* from a certain point. But these points are only defined by one coordinate, which means they all lie on the same line! In other words, if we're given a point *(b)* on a line, there are only *two* points that are exactly a distance *r* from *(b)*. These points are given by *(b+r)* and *(b-r)*, and can be seen below.

![The somewhat boring zero-sphere](/images/zero-Sphere.png){:.centre-image}

I fully grant you that this isn't the most interesting object we can think of, but it *is* consistent with out definition. The other one that we can easily visualize is the two-sphere, which is what you were likely imagining when I said the word *sphere* in the first place.

Two more note about spheres. You might think that it would have made more sense to call the two-sphere (the regular sphere) a *three*-sphere, since it's a three-dimensional object. The problem is that the regular sphere is we only need *two* free coordinates to describe a sphere (since the radius is constant), which is why we use the description we do.

Additionally, this generalization of the circle means that we can think about spheres in higher dimensions. We can't visualize them, of course, but we can work with them mathematically. And that's the important part. We can only do so much mathematics with a definition of a circle that says it's a "round object". With our new definition, we can precisely study a sphere in any dimension we want, which is quite useful.

---

Definitions (along with axioms) work as the building blocks of mathematics. What's nice about them is that even though we can quickly build up complex machinery and theory that surrounds these definitions, we can always bring ourselves back to the basics if we get stuck. One of my professors captures this perfectly. He often tells us that, if we get stuck on a problem with the new theory we've learned, we should always be able to go back to the basics in order to answer a question, or at least find a foothold into the problem.

For myself, this is often how I go about writing proofs. In mathematics, we write proofs to be as minimal as possible, which means that we don't want to assume anything that we don't absolutely have to. Therefore, if a certain kind of object is necessary to get a result, there's a good chance that knowing the definition of that object will help with the proof. That's why I always try to keep the definitions of the objects I work with handy. You never know if they can be just the thing you need in order to more deeply understand or solve a problem.

[^1]: You can also either include or exclude the boundary. That's called a closed or open disk.


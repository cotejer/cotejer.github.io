---
title: Notation and Beginners
author: Jeremy
tags: [notation, mathematics, education, learning]
permalink: /notation-and-beginners
date: 2019-06-10
---

You’re interested in learning a new mathematical topic. After reading some popular articles that speak in broad terms about the subject, you are energized to go on a deeper dive and learn the details.

You open up a textbook, pencil in hand and ready to expand your horizons. You start going through the introductory chapter, motivated with the dream of working through the whole textbook.

You make a little progress, but you find yourself pausing over and over again. Not because you can’t follow the mathematics, but because the notation is just so difficult to follow. After multiple pages of frustration, you put the textbook aside, never to look at it again.

---

Sound familiar?

Unfortunately, I think this is a problem that affects all mathematics students.

This isn’t just an issue with advanced mathematics (though we will get to that). It also crops up near the very beginning of a student’s mathematical journey, when they are learning about addition and subtraction.

At first, everything is fine because you are only using positive numbers. You deal with expressions like *5-3* or *10-6*. Once you understand how to subtract two numbers, this becomes straightforward.

The complication arises when your teacher throws a curve ball at you and starts asking questions like *5-(-4)*. What was once a clear notation starts to become tricky. I’ve worked with many students who are learning about this, and they struggle with conceptualizing the fact that two negatives “become” a positive.

Sure, we can just *tell* the student that this is the rule, but that takes away from some of the deeper understanding. We aren’t just declaring that this is the way it goes and hope for the best. Rather, we want to explain the idea in terms of addition and subtraction in a way that makes this particular situation become a simple consequence of the underlying ideas.

The problem here is that the symbol “-” signifies two things. First, it can refer to the operation of subtraction. Second, it can refer to the fact that a number is *negative*. This new interpretation of numbers demands a novel way of thinking for students if they want to get the concept.

However, this idea of having *two* meanings for the symbol “-” doesn’t seem to be something a lot of students are aware of. It’s no wonder then that they are confused when dealing with the subtraction of negative numbers. The notation isn’t helping them. In fact, I would go so far as to say that it makes their lives *worse* than referring to addition and subtraction as "moving" left and right of a number line.

---

Here’s another example.

When I first started working as an undergraduate researcher, I had to learn general relativity. In particular, I needed to learn the basics when it came to tensor calculus. This included concepts like the metric *g<sub>ab</sub>*, covariant derivatives, and tensor equations.

One thing that I struggled with early on was the use of indices in equations. In general relativity, equations are written in terms of tensors, which have indices. For a simple example of what this might look like, consider a vector given by **V** = (1,0,0) in the standard Cartesian coordinates. In index notation, I could write the vector as *V<sup>i</sup>*. Then, depending on if the index has a value of 1, 2, or 3, it would “pick off” the corresponding component.

For example, if I want the *x*-component of the vector **V**, I would want to look at *V<sup>1</sup>*.

You can then do a similar thing with matrices. If you have a matrix *M*, then the index notation for this matrix would be *M<sub>ij</sub>*, where the subscript *i* refers to the row, and *j* refers to the column.

Note here that the indices being subscripts or superscripts becomes important in general relativity, but for the sake of this essay, we won't worry about it.

This index notation is very nice because it lets us combine objects with different numbers of indices. This is how we end up writing the equations of general relativity.

Related to this notation is the idea of the Einstein summation convention. To see what this is, consider what happens when we want to take the length of **V**. From the usual notion of length in linear algebra, we need to compute:

*\|V\|<sup>2</sup> = 1<sup>2</sup> + 0<sup>2</sup> + 0<sup>2</sup> = 1*.

However, we can write this down in terms of our index notation. Brushing aside a few details, the length (squared) of the vector looks like:

*\|V\|<sup>2</sup> = &sum; V<sup>i</sup> V<sub>i</sub>.*

Here, the sum is given over the index *i*, and runs from 1 to 3. This is a bit different in general relativity, where the indices run from 0 to 3 (in order to incorporate the dimension of time).

The Einstein summation convention is simply the fact that we omit the sum symbol &sum; in our tensor equations. Repeated indices *implies* the summation.

This is where things started getting very confusing for me. I was getting lost in the manipulation of indices. I was mixing up indices that were supposed to be summed over versus ones that were left alone. It meant I struggled through every equation I came across, which resulted in a steep learning curve.

I think that a big source of difficulty for me was this notation for tensors. Now that I’m on the other side of the learning gap and understand how these equations are written, I can appreciate why having summation symbols everywhere is messy. The Einstein summation convention really does make things more convenient to work with.

That being said, the notation is what held me back as a beginner. It was just another thing to remember how to manipulate (and I haven’t even mentioned the whole business of raising and lowering indices!), which increased my initial burden. When you have to juggle both the concepts *and* the notation, it's easy to get fatigued and quit.

This is a lesson I think we would do well to remember when introducing mathematical ideas to students. While we have notation that *seems* like it is easier to use, that perspective might be coloured by the fact that we pushed through the difficult part of learning and emerged to the other side. For students who are beginning, the notation isn’t necessarily sensible, and often it is not even mentioned, exacerbating the confusion.

*Why* do we use certain symbols for functions versus vectors or matrices? Out of all the possible notations to choose from, why did we end up with *this*?

I know that the answer is sometimes historical circumstance, but I think we do a disservice to not motivate new notation to students. If it really is easier to use, give them a clear argument for it. More crucially though, don’t just jump to a new notation. Make the change gradually, so that students aren’t left scratching their heads, too shy to ask for clarification.

Notation might be a boring topic, but it’s the interface on which students connect with the mathematics. If we don’t get this right, we will lose students who otherwise could have enjoyed the subject.

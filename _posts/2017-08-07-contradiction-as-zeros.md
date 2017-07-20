---
title: Contradiction as Zeros
author: Jeremy
permalink: /2017/08/07/contradiction-as-zeros
date: 2017-08-07 04:19:09-0400
---

This is going to be a very quick post, but it's something I wanted to share since I think it could give some insight into a concept that is used to make proofs in mathematics. When writing proofs, it is often difficult to show that your proof holds for *every* case (say, if you're trying to show that the square root of two is not capable of being represented by a ratio of integers). Checking every single combination of integer ratios would take an infinite amount of time, so we want to come up with a strategy that is better. To do this, we try to prove our statement by *contradiction*. The idea is that we negate our conclusion, and from that, we need to show that there is a logical contradiction. Therefore, when we come to a contradiction, we know that our assumption of negating the conclusion was false, so that means our conclusion is true.

But why does a contradiction imply *only* that our conclusion is actually true? Why couldn't it mean that something else is wrong with our proof? To see this, I like to think of it as finding the zeros of a function.

Remember that, if we have a series of terms that are multiplying each other and equal to zero, then this implies that *at least one* of these terms is zero. This comes from the fact that you can only get zero as a result if one of your factors is also zero. Now suppose that you know that some of these terms are *never* zero. Then, you can shorten your list of potential candidates that *are* zero, letting you solve the equation.

This closely resembles what we do in a proof by contradiction. In this case, the "terms" are our hypotheses, the things we assume are true. When we construct our proof, we always choose hypotheses that we assume to be true, so they won't ever be false. We then add one more statement, which is the negation of our conclusion. The idea here is that we *want* this to be false (because we want the conclusion, and not its negation, to be true). From here, we simply use these hypotheses to generate new statements (which is the equivalent of multiplying in our analogy), and we finally come to a result. If we then see that our result is a contradiction, we know that *at least one* of our statements that we used is false. However, since the only statement we aren't assuming to be true is the negation of our conclusion, we can say that the satement is false, which proves our conclusion.

This connection between finding zeros and doing a proof by contradiction is helpful to me since it shows me just how we know that a *particular* statement has to be false. It all comes down to the fact that we deliberately construct the group of statements such that only *one* will be false.
---
title: A Nice Way to See the Identity for Binomial Coefficients
author: Jeremy
permalink: /adding-binomial-coefficients
date: 2018-01-01
---

As someone who likes to learn new concepts, I'm guilty of "knowing" a bunch of mathematical concepts without knowing the "why" behind them. In other words, I've come across many neat bits of mathematics, yet I only understand them at a surface level. However, as I continue through my mathematical education, every now and then I'll formally learn something that I came across before, and the explanation makes the concept that much more interesting in my mind.

One of these mathematical tidbits has to do with Pascal's triangle (and yes, I know there were others before Pascal who studied the triangle). Of course, most students are at least somewhat familiar with Pascal's triangle. My background was simply that I knew that it was constructed by starting with marking a 1 three times at the top of the triangle, and having each subsequent number beneath it being the sum of the two numbers directly above it. This is a situation where a sketch is a lot more helpful than words.

![](/images/pascalTriangle.png)

This is the manner in which I always saw Pascal's triangle: as a construct that you manually built up, row by row. However, once you learn about how the Binomial theorem relates to the numbers in the triangle, the above statement I gave about the term in the lower row being constructed from the two above it can be more precisely stated as:
$$
\begin{equation}
	{n+1 \choose k} = {n \choose k-1} + {n \choose k}. 
\end{equation}
$$
This is a simple equation relating two adjacent entries in Pascal's triangle to the entry directly underneath both of them (as can be seen from the sketch above). The equations are in terms of combinations, which are defined as ${a \choose b} = \frac{a!}{b! (a-b)!}$. To get the above identity, one could simply prove it by manipulating the algebra and getting the result. However, let's try and see if we can get this result in a slightly more clever manner.

To start, we will consider the set $A = \{ 0,1,2,\ldots,n \}$. This means that the set has $(n+1)$ elements. Therefore, if we were picking $k$ elements from the set $A$, we know that using combinations will yield an answer of ${n+1 \choose k}$. This is exactly what we want. However, to calculate this, let's start by thinking about how many ways we can pick $k$ elements from $A$, except that we are *forced* to pick zero. How many ways can we do this? First, we need to note that if we already know we have to pick zero, then there are really only $n$ elements left to choose from, and we can only choose $(k-1)$ of them. This is simply the result of already picking the zero from $A$. Therefore, the total number of ways we can do this is given by combinations, and is ${n \choose k-1}$.

So, we've found all the ways to pick $k$ elements from $A$ when we *know* zero is picked. However, this leaves out a lot of possibilities, since there are almost definitely configurations where zero hasn't been picked. To make up for this, let's consider the number of ways we can pick $k$ elements from $A$, except that we *don't* pick zero. Since zero isn't a possibility, we have $n$ possible items to choose from, and we still have $k$ choices. This leaves us with a total of ${n \choose k}$ possibilities.

Now for the good part. We started with wanting to find the number of ways to pick $k$ elements from the set $A$. We then broke this problem up by separating it into two cases: when zero *is* picked, and when zero isn't picked. However, note that these two cases don't have any overlap. There is no way to pick $k$ elements from $A$ and be in both cases. Our choice of elements either has a zero, or doesn't. It's a binary decision, and there is no overlap. Therefore, to answer our original question, we need to simply add up both possibilities that we calculated above. Doing so gives:
$$
\begin{equation}
	{n+1 \choose k} = {n \choose k-1} + {n \choose k}. 
\end{equation}
$$
This is exactly what we started out with, and completes our proof. I really like this proof because it involves no explicit manipulation of terms. Instead, it merely requires one to shift perspectives and see the problem in a new light. When looking at Pascal's triangle, it's not like the idea of using a set of $n+1$ elements is the "natural" thing to do. If you read through this and were scratching your head at the beginning, I don't blame you. The whole detour in the above paragraphs makes sense in retrospect, but when first observed it can seem totally out of the blue. I feel like this is the essence of good problem solving. Can you come up with alternative explanations that work? If so, then you're doing some great mathematics.

### Image Credit

The image of Pascal's triangle is from [Wikipedia](https://commons.wikimedia.org/wiki/File:Pascal_triangle_small.png).
---
id: 589
title: Integrals, Integrands, and Understanding the Notation
date: 2017-03-10T04:22:00+00:00
author: CJeremy
layout: post
guid: https://blog-cjeremy.rhcloud.com/?p=589
permalink: /2017/03/10/integrals-integrands-and-understanding-the-notation/
categories:
  - Uncategorized
---
Even though mathematics is one of the subjects I enjoy studying, it&#8217;s not always easy. Nor does everything always make sense to me. One of these things was the notation for an integral.

If you&#8217;re reading this, you probably have an idea of what an integral looks like. The simplest one looks like this:

$$\int f(x) dx$$

You recognize the $f(x)$ part, but the other two parts aren&#8217;t components you&#8217;ve seen before. When I first learned about integrals, I don&#8217;t think I really internalized the notions of the two other symbols, and it was to my detriment. In mathematics, if things look funny, it&#8217;s probably because you don&#8217;t fully understand them. The reason is that ideas are made to be as compact and helpful as possible in most mathematical concepts that you will see in your education. Said differently: complexity isn&#8217;t introduced for complexity&#8217;s sake.

The symbol on the left ($\int$) is just the sign of integration. Much like we write $\frac{d}{dx}$ or $f'(x)$ to denote derivatives, the sign of integration is there to tell you that an integration is being performed. However, the shape of the symbol isn&#8217;t arbitrary. The symbol is a sort of horizontally narrowed and vertically stretched out &#8220;S&#8221;, and it stands for the word &#8220;sum&#8221;. After all, integrals come from the idea of taking the sum of a bunch of tiny pieces of a function, and so the sign of integration is supposed to be a nod to that.

However, it&#8217;s the _other_ symbol which has much more meaning. The $dx$ part of the integral is what signals to the reader what variable will be integrated. In my example, $x$ is the variable being integrated.

When I first learned about integrals, this was where I stopped digging deeper. I more or less just went ahead and calculated, only using the $dx$ as a small reminder that I was supposed to be interacting with respect to $x$. This approached worked for me, but it definitely wasn&#8217;t the best I could have done. Instead, here&#8217;s the _much_ better way of thinking about the $dx$ part.

First of all, $dx$ is called the _infinitesimal_ or _differential_ of $x$. These are just long words to say that the portion of $x$ we are considering is really tiny.

You also probably know that a way to interpret a _definite_ integral (one that has bounds of integration) is to think of it as the net area &#8220;under&#8221; a curve between two points. That&#8217;s the &#8220;physical&#8221; way to look at it, and it has a lot of meaning for our notation of an integral.

What kind of units does an area have? It has units of a length squared, such as $m^2$. Therefore, if our integral is just a bunch of addition of tiny &#8220;chunks&#8221; of area, each chunk needs to have units of area.

If we look back at our integral:

$$\int f(x) dx$$

We can imagine the term $f(x)$ being considered as one of the lengths in question. So what&#8217;s the other one?

It&#8217;s the small portion $dx$.

The reason this was hard for me to grasp at first was that we were discussing $dx$ as though it was so small that it was basically not there. As such, I didn&#8217;t think of it as a &#8220;real&#8221; quantity. It was just a symbol that I put inside my integral, and it had no actual meaning. However, I couldn&#8217;t have been further from the truth. By taking $dx$ to have a geometrical meaning, the idea of an integral suddenly felt so much more grounded to me. The $dx$ wasn&#8217;t some ornament. It was an important part of the integral.

And that&#8217;s what I want you to get from this. The differential $dx$ is very important in concepts later on, so it&#8217;s a good idea to get a firm understanding of what that differential actually means.
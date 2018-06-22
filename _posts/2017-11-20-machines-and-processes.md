---
title: Machines and Processes
author: Jeremy
permalink: /machines-and-processes
date: 2017-11-20
---

When you first learned about algebra, chances are you learned about something called a function, typically one that looks like this:
$$
\begin{equation}
f(x) = ax +b.
\end{equation}
$$
This is nothing more than the equation of a straight line. You probably also learned how this could be represented as a graph (which is why you know it's a straight line). This was simple enough, and you soon learned how to deal with different kinds of functions. These include quadratics (parabolas), exponentials, rationals, and a host of other functions. You learned what these looked like when graphed, and how to find various properties of these functions. This includes finding the roots of the equation (when $f(x)=0$), finding the domain and range, and characteristics of when the graph is increasing or decreasing.

To find some of these properties, you actually had to interact with the function. That meant working through the algebra and manipulating some equations. Depending on how comfortable you were in mathematics, this could be easy or difficult. However, assuming you got past this stage and still understood what was happening, you then got to more exotic functions, such as logarithmic or trigonometric functions. These have the form $f(x) = \log(x)$ and $f(x) = \sin(x)$, and aren't your usual functions. This is where you start seeing students making the mistake of dividing by $\sin$ or $\log$.

Why does this happen? From my experience, it's due to the sense that everything in mathematics is *linear*. To illustrate this, let's look at an easy example. Suppose we have the equation $\log(x+1) = 2$. You might be tempted to say that this is the same as $\log(x) + \log(1) = 2$, but this would be incorrect! What we actually have to do is convert the equation into exponential form, giving us $10^2 = x+1$. The answer itself isn't really important. What's important is that the logarithm *isn't* linear, and so you can't simple distribute it onto the term $(x+1)$.

From what I can gather, the reason this happens is that $\log(x+1)$ is very similar in notation to $4(x+1)$. We know that the latter is equivalent to $4x+4$, which we get by multiplying each term inside the parentheses by $4$. As such, it isn't so surprising when students think that the same should apply to these new things called logarithms. The same is true for the expression $\sin(x+1)$ and $(x+1)^2$. We feel like it's completely natural to write $\sin(x)+\sin(1)$ and $(x^2+1^2)$, but this is incorrect.

Instead, what we should think of the expressions like $\sin(x)$ and $\log(x)$ as *functions* or *machines*. When you insert a number $x$ into them, the machine runs, and spits out a number back. The crucial part is that the machine is *highly* dependent on the initial number you put in. Said differently: if I put $(2+5)$ into $\sin(x)$, or if I do $\sin(2)+\sin(5)$, I get to very different answers. For comparison, the former gives approximately $0.065699$, and the latter gives $0.909297-0.958924=-0.049627$. Obviously, these two numbers aren't the same. Also, for those who have studied trigonometric functions, you know that $\sin(x)$ varies from $-1$ to $1$, which means that $\sin(x+y)$ must also vary from $-1$ to $1$, while $\sin(x)+\sin(y)$ could vary from $-2$ to $2$, which means these two expressions can't be the same.

This is also true for logarithms, and many other mathematical functions you may encounter. The difficult at this point is to deal with this while working with algebraic equations. You can't simply add, subtract, multiply, and divide your way to a solution. You have to know what functions you're dealing with, and how to work with them.

Last example: consider the function $f(x) = 4\sin(x^2-2) +1$. This function has a lot going on, but the way I think about it is that you have a function within a function within a function. To make this explicit, label $g(x) = \sin(x)$, and $h(x) = x^2-2$. Remember that the variable $x$ in both of these equations is just a placeholder. You can stick *anything* there. If we think back to our analogy of a machine, think of $x$ as where you input your value into the machine. Now, if we write $f(x)$ in terms pf $g(x)$ and $h(x)$, we get the following:
$$
\begin{equation}
	f(x) = 4g(h(x)) +1.
\end{equation}
$$
This equation may look a bit busy, but that's the point! I want you to really see where $x$ is located. It's nestled into the "deepest" function, $h(x)$. What I want you also see is that instead of writing $g(x)$, I wrote $g(h(x))$. This means that instead of sticking $x$ into the input of $g(x)$, I stuck $h(x)$ instead! There is nothing wrong with this, and it actually has a fancy name. It's called a *composition* of functions. Think of it like a machine within a machine. The output of the first machine is connected to the input of the first machine, so that when you give the first machine an initial value, it passes through *both* machines. As such, you can't exactly "split up" the machine into two different parts and expect to get the same answer as doing both together. It depends on the nature of the machine.

---

Hopefully, this gives a bit of intuition into the idea of more complex functions such as the logarithmic or trigonometric functions. They *don't* distribute linearly, and so you can't apply your usual rules of algebra to them. Additionally, it's important to remember that expressions like $\log$ and $\sin$ by themselves have *no* meaning. They aren't numbers. Typing these into your calculator and pressing the "=" buttom gives an error, and rightly so! Remember, they are like machines or processes, so asking what the output of a machine is without any input doesn't make sense.

By keeping in mind the analogy of functions as machines, you should have a better conceptual understanding of *why* logarithms and trigonometric functions don't simply distribute, and this will translate to understanding how to manipulate them without mistakes.
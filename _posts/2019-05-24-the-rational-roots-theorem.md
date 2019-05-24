---
title: The Rational Roots Theorem
author: Jeremy
tags: [mathematics, polynomials]
permalink: /rational-roots-theorem
date: 2019-05-24
---

One of the skills students learn in secondary school is to factor quadratic expressions. In particular, they learn how to solve equations like *x<sup>2</sup>+2x+1=0*. There are a slew of techniques one can use to deal with quadratics, and they mostly rely on the fact that questions asked in assignments and tests have "nice" factorizations. Most expressions have integer solutions, or at worst rational ones. This makes it straightforward to factor. Of course, this might take a while to get used to, but it's a skill that many students pick up.

If they *really* have no idea how to factor an expression, they learn about the tool that deals with basically every case: the quadratic formula. This is something that most students will remember from their days in mathematics class (even if they don't remember the formula explicitly). The nice thing about this is that, as long as you can crank the gears of arithmetic, the quadratic formula won't fail you.

This is great, but the reality is that the world has much more than just quadratics and linear equations. In fact, what you learn soon after leaving secondary school is that the whole *class* of polynomials tends to be considered "nice". Therefore, a question you might ask is, "How can I factor these expressions?" After all, there's nothing different in principle with factoring a polynomial of degree greater than two. You still have to find the roots of the equation, though this looks more difficult when you have a polynomial with a higher degree.

Being able to factor larger polynomials comes up from time to time. I had to do this in my differential equations class, which doesn't immediately suggest factoring. While one of us was bemoaning the difficulty of factoring these large polynomials, my professor stated an interesting little result that I didn't know about. It's called the rational roots theorem, and it made enough of an impression on me that I still remember it.

Here it is. The rational roots theorem tells us that if a polynomial with a constant term has a rational root in it of the form *a/b* where *a* and *b* are relatively prime, then *a* will divide the constant term and *b* will divide the coefficient of the leading term.

I think it's quite instructive to see this in an example, so let's look at one before the proof of why this works. Suppose we have the following polynomial:

*4x<sup>2</sup>+9x+2*.

The question is, can we factor this nicely? Since I took a simple quadratic, you can probably figure out its factors without this method. However, if we refer to the rational roots theorem, we need to look at the constant term 2 and the coefficient of the leading term, 4. The factors of 2 are 2 and 1, while the factors of 4 are 1, 2, and 4. Furthermore, since our theorem simply says that the numbers *a* and *b* will divide the constant and leading coefficient, our values can be negative too. As such, our possible values of *a* are 1, 2, -1, 2, while the value of *b* could be 1, 2, 4, -1, -2, and -4. The possible values for a solution are given by the rational number *a/b*:

*&#177;1, &#177;1/2, &#177;1/4*, and *&#177;2*.

This gives us eight possible solutions to the equation. If there's a rational solution, it will be in the above list. We can then test each one and see if the output is zero (meaning it's a root). In our case, since the coefficients of each term are positive, the only way to get an output of zero will be if the input is negative. That eliminates half the values. We can then test to find that the solutions are *x=-2* and *x=-1/4*, which are both on the list.

Now, you might not be too impressed with this. After all, this doesn't guarantee we will find solutions. It just gives us possible candidates. What happens if we have a few solutions in our list, but some that aren't there (since they aren't rational)?

This is a valid concern, but the reason I'm discussing this theorem is because it has practical value in class. When factoring polynomials, chances are the solutions will be rational. For quadratics, I wouldn't employ this method since I'm used to eyeballing the solution (through lots of practice). However, when the degree of the polynomial is larger, this theorem comes in handy.

The idea isn't to necessarily find *all* the factors in one go. In fact, the context that my professor mentioned this was when he explained that factoring a polynomial becomes easier as soon as you find one factor. That's because you can then exploit long division to make the polynomial smaller, which is easier to work with.

So what is the proof of this result? Thankfully, there isn't anything too difficult with it. The crux of the proof lies in rearranging the equation for the roots.

To begin with, let's consider a polynomial *p(x)* of the form:

*p(x) = a<sub>n</sub>x<sup>n</sup> + &hellip; + a<sub>1</sub>x + a<sub>0</sub>*.

For convenience, we'll say that the leading coefficient *a<sub>n</sub>* isn't zero (or else we'll just consider the next leading coefficient). One other requirement is that the constant term *a<sub>0</sub>* isn't zero either. This is crucial for the proof, as we will see below.

Now, consider a rational root to *p(x)*. Furthermore, since we can always simplify a rational number until the numerator and denominator are relatively prime, let's call the rational root *u/v*. Substituting this into the polynomial gives:

*p(u/v) = a<sub>n</sub>(u/v)<sup>n</sup> + &hellip; + a<sub>1</sub>(u/v) + a<sub>0</sub> = 0*.

We then want to see if this imposes any conditions on *u* or *v*. To start with, we can move the constant term *a<sub>0</sub>* to the other side of the equation, and then multiply both sides by *v<sup>n</sup>*, since this will remove any fractions. Doing so gives:

*a<sub>n</sub>u<sup>n</sup> + &hellip; + a<sub>1</sub>uv<sup>n-1</sup> = -a<sub>0</sub>v<sup>n</sup>.*

At this point, look at the left side of the equation. Each term contains at least one *u*, which means the whole of the left side is divisible by *u*. However, since the two sides are equal, this means *u* also divides the right side. In terms of the above equation, this looks like:

*u(a<sub>n</sub>u<sup>n-1</sup> + &hellip; + a<sub>1</sub>v<sup>n-1</sup>) = -a<sub>0</sub>v<sup>n</sup>.*

We know a bit more than this though. Since the root for *p(x)* was *u/v*, we know that *u* can't divide *v*. Why? Because *u* and *v* are relatively prime, which means they don't share any common factors. Therefore, one definitely can't be a multiple of the other. Since *u* doesn't divide *v*, this *also* means *u* can't divide *v<sup>n</sup>*. This gives us only one final possibility, which is that *u* must divide *a<sub>0</sub>*!

We can play a similar game with our equation of *p(u/v) = 0* by rearranging the terms for *v*. Doing so gives us:

*a<sub>n</sub>u<sup>n</sup> = -a<sub>0</sub>v<sup>n</sup> - a<sub>1</sub>uv<sup>n-1</sup> -  &hellip; - a<sub>n-1</sub>u<sup>n-1</sup>v = v(-a<sub>0</sub>v<sup>n</sup> - a<sub>1</sub>uv<sup>n-1</sup> -  &hellip; - a<sub>n-1</sub>u<sup>n-1</sup>).*

Again, we that there is an overall factor left in the polynomial terms, so we can pull out a *v* from each term. This means the whole right side is divisible by *v*. As such, we get that the left side is divisible by *v*. Then, we can note that the same argument applies as before, which lets us conclude that *v* must divide *a<sub>n</sub>*. This gives us the desired result we wanted.

Note here that is was very important to have a constant term in our polynomial. Without it, we couldn't bring a term onto the other side of the equation and then multiply through by *v<sup>n</sup>*.

There's one more thing we can note here. If the leading term in the polynomial is *a<sub>n</sub> = 1*, this implies *v = 1*, since it's the only integer that divides 1. (Strictly speaking, we could also consider *v = -1*, but we can just absorb the sign in the numerator.) What this means is that, if the leading term of a polynomial has a coefficient of one, the roots will either be integers or irrational numbers.

---

What I find so interesting about this theorem is how the leading coefficient and the constant term impose "constraints" on the roots of a polynomial. It's not *really* surprising when you understand that when you expand the factored form of a polynomial, the "information" from the roots is encoded in the constant term. I'm not sure how rigorous this interpretation is, but I like the heuristic.

Like most interesting results, there's no amazing practical use of it. Yes, it can make your life easier if you find yourself needing to factor large polynomials, but other than that I just find it makes for an interesting theorem.

As a final note, there is a clever application of this theorem that I want to mention. In the essay, I didn't mention the straightforward implication of the result: if you find that there's a solution to the equation which *doesn't* fall into the rational category, the solution is irrational. This might sound sort of obvious, but it means we can "test" to see if certain numbers are irrational by constructing polynomials with them as solutions. I learned about this from a Mathologer [video](https://www.youtube.com/watch?v=D6AFxJdJYW4), so I highly recommend checking it out if you want more details.

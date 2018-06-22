---

layout: post

title: Units

author: Jeremy
date: 2017-06-19 01:00:10
permalink: /2017/06/19/units

---



When students first start working in mathematics, units aren't really something to worry about. Indeed, students begin with doing arithmetic, where there's little need for extra fuss about units. Students get used to writing equations without ever thinking about units.

However, students are then suddenly thrown into science classes where there *is* an emphasis on having the correct units throughout a calculation. This isn't a difficult concept, but it can seem mysterious to those who have only heard it from a teacher as if it's a law handed down from the great mathematicians of history. The reality is much more simple, and being able to work with units is something called *dimensional analysis*, which can be a pretty powerful tool. So, let's get started.

## An equation isn't just about the numbers

You know what an equation is. It's some mixture of symbols and numbers that have an "$=$" sign somewhere in the middle. Simple enough, but let's write down an example. If I wanted to write down the area of a triangle. It's given by the following formula:

$$A=\frac{1}{2} bh$$, where $b$ is the base of the triangle and $h$ is its height.

This is probably one of the first things you saw in secondary school. It's a nice formula, and I'm sure you've spent many assignments calculating the area of various triangles. You might have even been told that, when calculating an area, when you wrote down your final answer, you should slap on so-called "area units", like $m^2$ or $cm^2$. It might not have even been something you thought about. Instead, you just made sure to remember to include it at the end, or else your teacher would take off marks.

Maybe you wondered to yourself, "Why do they care so much about units?" I'm going to now answer your question.

In physics (and science in general), we study the world around us. Unlike mathematicians, we are very concerned with describing things that are physically possible. In the process of finding things out about the universe, we quickly found out that the best way to *describe* what we figured out was through mathematics. Still, when we write equations down, we don't want to just have them output numbers. We want numbers that have *meaning*. Put more explicitly, there's a huge difference between $3J$, $3m$, and $3s$. As such, we really do need units in order to make sure we get answers that have physical relevance.

Here's the punchline: an equation means that *both* sides are the same.

Okay, you're probably rolling your eyes at me. Of *course* both side of an equation are equal! That's why it's called an *equa*tion.

Fair enough, but in physics this has a slightly more subtle meaning. It also means that the *units* of the equation are equal, too. Let's go back to the example above in order to get a feel for this. We had $A=\frac{1}{2} bh$, and we know that $A$ represents an area, which means it has units of something like $m^2$. This means that the other side of the equation needs the same units as well. The factor of $\frac{1}{2}$ doesn't have any units, so we treat it as a pure number (which means it doesn't contribute to the units of the expression). We then have $b$ and $h$, which each have units of lenght, such as $m$. Therefore, since we are taking the product $bh$, we multiply the units as well, giving us $m*m=m^2$, just like the left hand side. The units agree, and so we are done.

Units work like this in *every* equation you ever want to make. You can even think of units as "variables" that obey the same algebra as regular variables. In particular, you cannot simplify $a+b$ since they aren't the same "thing". Similarly, you can't suddenly be adding a length and an area together, since their units wouldn't agree ($m+m^2=?$). However, multiplication and division are allowed, in the sense that you can have units such as speed ($\frac{m}{s}$) or force ($\frac{(kg)m}{s^2}$).

The bottom line is that units have to *always* agree, which is why you can easily check if an answer you come up with in a calculation makes sense. Did you verify that you didn't add units that can't be added? Do both sides of your equation have the same units? This is a mistake I see many students make, and it's usually the first line of attack I make into having students fix their equations.

This also answers another question you might have posed at one time. Why do some constants in formulas like ($\vec{F}=-G\frac{mM}{r^3}\vec{r}$) have such funny-looking units ($[G]=\frac{[L]^3}{[M][T]^2}=\frac{m^3}{(kg)s^2}$?

The reason is simple: to make the units work out in the equation! If we have a force on the left side, we need the units of a force on the right hand side. Thus, we need to have the units on $G$ that we have above if we want the equation to satisfy unit analysis.

---

Hopefully, I've made the case for why units are important and why they aren't just something we tack on at the end of a calculation. They have significance, and so for that reason, it's important to be able to reason with the units of an equation. It's a very quick check to make sure the equation you're creating to solve a problem is within the right ballpark. As long as you remember that the units on both sides of an equation need to come out to the same thing (even if they initially look widely different), it becomes easier to understand equations.

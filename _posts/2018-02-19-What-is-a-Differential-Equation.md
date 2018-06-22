---
title: What is a Differential Equation?
author: Jeremy
permalink: /what-is-a-differential-equation
date: 2018-02-19
---

For those who don't study mathematics but have an interest in science, the term "differential equation" will often come up in conversation. They are often said to be really important to all scientific disciplines, but what *are* they exactly, and how do they help us describe the world?

To begin with, a differential equation can be thought of as an equation that links a quantity with the rate of change of that quantity (and potentially, the rate of change of the rate of change, and so on). More technically, if we have a function that depends on $x$, we call it $f(x)$. Then, a differential equation could be of the form:
$$
\begin{equation}
\frac{d^2f}{dx} + \omega^2 f = 0.
\end{equation}
$$
Students in physics will perhaps recognize this differential equation as the equation describing simple harmonic motion. For everyone else, the above equation simply relates the function $f$ with its second derivative (which is a measure of how the change in $f$ changes). And since the second derivative describes how the function $f$ changes in some way, this function can be used to describe certain motion (such as that of a spring or a simple pendulum). Of course, if this is the first time you have seen this differential equation, this won't be obvious to you. However, this is indeed related to those two physical systems, and can actually be seen from *another* differential equation, namely:
$$
\begin{equation}
	F_x = \frac{dp_x}{dt}.
\end{equation}
$$
This is simply Newton's second law in the $x$ direction. From this differential equation, one can derive all sorts of equations of motion for classical systems, such as the equations of motion for the spring or the simple pendulum, shown above. This is *very* powerful, because we are able to work out solutions to most classical mechanics problems using just the above equation (technically, by using one for each axis of motion). Of course, I'm not saying that we can always solve these equations *exactly*. In fact, most of the time one needs to use a computer to solve the equations numerically, since no analytical form is possible (which means we won't get a nice formula at the end for the motion).

This brings us to the question of *solving* these differential equations. What exactly are we trying to solve for in these equations? We are are looking for the specific function $f(x)$ such that we can substitute this function back into the equation and have the equation be satisfied. This turns out to be more difficult than solving regular equations in algebra class, because now we have to deal with the fact that a function *and* its rate of change (and other derivatives) have to all be satisfied in the differential equation. As such, there are whole courses devoted to studying techniques to finding solutions to classes of differential equations.

However, it gets even *more* tricky.

I recently wrote about [toy models](\posts\toy-models.md), which are the models we begin with when studying phenomena in science. They are usually simple, and don't describe reality well. Then, as one increases the complexity of the model, we get a better description of reality. However, in the process, the equations become more difficult to solve. What we have been looking at so far are examples of *ordinary linear differential equations*. The "ordinary" part means that the functions only have one variable in them (for our first example, the variable was $x$). The "linear" part means that the functions aren't multiplied by other functions of $x$. The following would not be considered a linear differential equation:
$$
\begin{equation}
	x\frac{df}{dx} + (x-1)f+f^2 = 0.
\end{equation}
$$
The above equation isn't linear because it has functions multiplied together within the various terms. This doesn't meant the differential equations are *impossible* to solve. However, if they do have a solution, they tend to be much more tricky to find.

To give a small example of how quickly we can ramp up in complexity, consider the Schrödinger equation in quantum mechanics for a single particle of mass $m$ in one dimension:
$$
\begin{equation}
	i \hbar \frac{\partial}{\partial t} \Psi(x,t) = \left[ \frac{-\hbar^2}{2m} \frac{d^2}{dx^2} + V(x,t) \right] \Psi(x,t).
\end{equation}
$$
This is now a much more involved differential equation. First of all, note that the function that we are trying to solve for, $\Psi(x,t)$, is a function of *two* variables. This automatically turns this into a *partial* differential equation, since we have a function of multiple variables. Additionally, if we look at the function $V(x,t)$, then if it isn't a constant function, it will multiply $\Psi(x,t)$, making the differential equation non-linear as well. This is particularly bad if you are searching for analytic solutions. This is why only some systems in quantum mechanics can be solved exactly (or very close to exact), while most need to be solved numerically. 

The equation itself though is how we study quantum mechanics. It's the backbone of our theory, and describes the time evolution of a system. As such, this partial differential equation is absolutely necessary, even if it can be tricky to solve.

There are many, *many* more examples of differential equations in the sciences. From the flow of heat to the growth of populations, differential equations describe the world around us. The key reason that scientists use differential equations then, is because differential equations capture *motion* in between variables. We can get situations where changing one variable bit does not only change the other variable, but also affects how fast that variable will change, and so on. In essence, we get relationship that are more intertwined, and better model the world around us.
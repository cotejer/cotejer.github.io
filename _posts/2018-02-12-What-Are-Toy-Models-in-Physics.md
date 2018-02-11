---
title: What Are Toy Models in Physics?
author: Jeremy
permalink: /toy-models
date: 2018-02-12
---

![](/images/toyModels.svg)

If you've never taken a quantum mechanics class, you might automatically think that one begins studying all of the quantum strangeness that occurs during experiments. Perhaps you jump into complex calculations involving quantum field theory, or perhaps you explore the phenomenon of quantum entanglement.

Similarly, if you've never taken a course in classical mechanics, you might think that one studies systems such as a bicycle rolling on the road, and how the tires interact with the ground in a complex way.

However, this is *far* from the truth.

In quantum mechanics, one begins by studying probability and the Schrödinger equation in different cases. Quantum field theory isn't even in the cards for the first few courses. For classical mechanics, complex situations such as a bicycle on the road aren't approached until the tail end of a course. If asked, a professor will probably say something along the lines of, "We aren't studying this now, because it involves more complicated terms such as friction."

Instead, here are the types of systems that are studied. For quantum mechanics, systems such as the free particle, the particle in a box, the quantum harmonic oscillator, and the finite square well are studied. For classical mechanics, blocks sliding on planes and other frictionless surfaces, pendulums (but only for small angles), and spring systems are typically studied.

Hearing this, a question might naturally arise. If we aren't even studying realistic systems, how can we learn anything about the reality around us?

A lot, it turns out.

The examples I gave above are what physicists like to call "toy models". They are named as such because they exist to exhibit certain properties of a system without complicating matters unnecessarily. Much like mathematics does when it generalizes and abstracts concepts in order to be more encompassing, physicists study and learn about toy models because they are useful mental models to have when moving to more complicated systems.

To give you an idea of how these systems can actually be incredibly useful later on, let's look at what seems like an innocent example from quantum mechanics: the particle in a box.

First, a small preamble on quantum mechanics. We study the quantum world through the Schödinger equation, which is given by the following differential equation:
$$
\frac{-i \hbar}{2m} \frac{\partial^2 \psi}{\partial t} = \left( E - V \right) \psi.
$$
Here, $E$ is the energy of the particle that we are looking at, and $V$ is its potential energy. Using this equation, the goal is always to solve for $\psi$ and $E$. These are two important quantities in quantum mechanics. The energy is something we can easily imagine, but the wavefunction $\psi$ might not be as clear to readers.

On its own, $\psi$ isn't anything special in terms of physics. It's only once we take the *magnitude* of the wavefunction, denoted $\vert \psi \vert ^2$, that we get a quantity that can be interpreted physically. The interpretation is that is it the *probability density* of the particle, in either its coordinate-representation (its location in space), or in its momentum-representation (the momentum the particle can possibly have). Roughly speaking, the probability density gets integrated over a small volume in order to give a probability that the particle will either be in a small region of space or have a particular range of momentum (the equivalent to a region of space). Therefore, the probability density isn't *exactly* a probability, but it is definitely related.

Back to our example. The particle in a box is one of the simplest systems one can study. It involves letting a particle live in a box and determining how the wavefunction $\psi$ evolves over time. How do we do that? Well, we set the potential $V$ to be infinite when one is outside of the box, and finite (in the usual case, zero), when one is inside the box. An infinite potential is akin to saying that $\psi = 0$ outside of the box.

![](/images/toy_models/particleInABox.svg)

Inside the box, the potential is then $V = 0$ (usually), which means we can solve the above equation to figure out both the energy $E$ and the wavefunction $\psi$. The actual derivation of these two quantities isn't terribly important here, but one consequence in particular is worth mentioning: the energy of a particle comes in discrete chunks. In other words, a particle which is confined to a box can't have any old energy that it wants. There are specific values allowed, and no others.

Obviously, this model isn't a realistic description of our reality. However, it *does* have some useful features. For one, it illustrates very simply some of the strange properties of quantum mechanics. As soon as a particle is confined in some way (in this case, by a box), the particle goes from being able to have any energy to having only specific possible values for its energy. This is true for the particle in a box, but it is *also* true for other systems. Think about that. As soon as you introduce some kind of confining potential to a particle, its energy goes from being a continuous quantity to being discrete. This tells us something very important about quantum mechanical systems! (Of course, this would need to be proved in more generality, but it gives us a taste of one consequence in quantum mechanics.) It just so happens that this particular system is very simple, so it's one that is easily studied to learn about some properties of quantum mechanical systems.

The same is true for the study of classical systems, such as the pendulum. Here, we make a bunch of approximations that render the system unrealistic, but "close enough" to the real thing that it is still useful to study. These approximations include the string or rod holding the pendulum being massless, the bob at the end of the pendulum having all of its mass concentrated to a point, and the amplitude of the pendulum being only a few degrees. If you relax these approximations, then you get a more realistic system, but the equations are *much* more difficult to handle.

![](/images/unrealisticPendulum.svg)

Therefore, we make do with our toy models. We know that they don't tell the whole story, but they give us a good idea on how a system will behave. Additionally, these toy models can be used to initially study a complex system, and slowly add new "features" to the toy model in order for it to better mirror the system we want to study. You can think of it as upgrading a computer system with better components. As such, the new computer will better handle the tasks you want it to do, just like the new toy model will more accurately reflect the system we want to study.

Despite the name, toy models aren't useless mathematical equations that physicists write down as a joke. Their purpose is to instruct, allowing one to study a complex system in its broadest strokes. We take a complex system, try and distill it down to its essential parts, and then come up with a toy model of it. This toy models simplifies things, but the point is that we can eventually reintroduce the complexity back in, slowly building up to our original system once again. It may have been impossible to initially study our system of interest mathematically, but by breaking it down and then building it back up, we learn a lot about the essence of a system, and therefore, we can gain insights that weren't apparent to us initially.

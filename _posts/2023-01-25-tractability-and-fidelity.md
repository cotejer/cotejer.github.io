---
title: Tractability and Fidelity
subtitle: A book review of "Escape from Model Land"
author: Jeremy
tags: [essay, science, mathematics, worldline, models]
permalink: /tractability-and-fidelity
date: 2023-01-25
excerpt_separator: <!--more-->
---

One of my favourite parts about mathematics is its definitive nature. Once you've proved a result, it's true for all of time. We can be confident that the chain of reasoning will hold, even without inspecting every part. This feature of mathematics has let us build incredible structures, and as a bonus, tools to help us reason.

At least in my mind, this definitive nature lends a certain *gravitas* to mathematics. I didn't go into mathematics myself, but my field of theoretical physics is so adjacent that many within it are also mathematicians. This has biased me towards mathematics. In general, I would trust a mathematical result more than I would a claim based on an anecdote. The former uses reproducible and logical standards of reasoning, which I've culturally absorbed as more trustworthy and stronger than other ways of reasoning. Because of this, if I see someone using mathematics in their work, I'm more likely to see it as authoritative. I prefer seeing a mathematical model of a situation than "just" some anecdotal data.

More than ever, people use mathematics to investigate questions about society, from what we should do about the climate to possible financial downturns. The stakes are higher than when a few theorists work on physics models: The models we create will influence society. As a result, we want to tread carefully, ensuring that out models help us improve society for *everyone*.

But there's a tension: Mathematics shines when a scenario has clear definitions, which is *not* the case for a lot of the questions we want to answer about our world. Faced with the messiness of our world, we need to simplify until we can handle the mathematical analysis. In other words, we have a tension between mathematical tractability and fidelity to our world.

In [*Escape from Model Land*](http://www.ericathompson.co.uk/books/), Erica Thompson brings the reader on a journey whose main purpose is to highlight this tension, forcing the reader to pause and ponder how we use mathematical representations--mathematical models--to understand our world. Thompson acknowledges that mathematical models are an enormously powerful tool for investigating the world, but that we can often fool ourselves into complacency, swapping the model in for the complicated reality of life.<!--more-->

I want to cover a few of Thompson's major points in her book, which I think offer general lessons when it comes to interacting with models.

# Model Land

In one of my introductory physics classes, we did an experiment on projectile motion. The challenge was simple: In pairs, we had to calculate the launch parameters for a catapault such that its projectile would hit a target. We were learning about projectile motion and Newton's laws, and this would be a practical demonstration of our knowledge. We all worked on our designs, and then the whole class watched as each pair tested their predictions.

How did we do? Of all the teams, only some managed to get anywhere close to the target. 

Even though we knew the equations of motion for the projectile, even though we knew the distance to the target, and even though we were in ideal conditions (inside a classroom), it wasn't simply a matter of calculating a launch angle and hitting the target. Clearly, reality was more complicated than our model.

Thompson illustrates this in her book by invoking "Model Land", a place where models live. This isn't our world, but instead various caricatures of it, all based on assumptions and simplifications that make the job of the modeller easier.

In the ideal case, we can learn something in Model Land and transport that knowledge back to our world. This is what happens when we create useful models. However, we have to be careful that the assumptions we use to construct our model in Model Land actually have parallels in our world. Without this, we're only learning about a mathematical world which has feable connections to our own.

As Thompson writes in Chapter Four: 

>Models can be physical, mental, mathematical or computational, and they are by nature metaphorical.

This metaphorical nature is why models live in Model Land. Sometimes the metaphor is strong enough that we can safely transport the model back over, but often it is not.

Another characteristic of Model Land is that everything tends to have precise mathematical definitions. When we create a model, it's its own little world, which means we specify the boundaries and the aim of the model. But in our world, aims are often fuzzy and messy. As much as we may wish it, our world isn't simple. Thompson discusses this in Chapter Five, illustrating the difference between the aim of a computational model versus *our aim*:

>In Model Land, the computer has a clear and unambiguous aim: win the game. Outside Model Land, the game itself is unclear and to some extent we are making the rules up as we play. Living by our own rules is both an opportunity and a risk.

When we create models, we imbue them with simplifications, but also *translations*. Specifically, we translate vague questions such as "What should we do about the climate?" to one like, "If we implement policy X, what will be the long-term economical impact of climate change?" While there's a connection between these two questions, don't be fooled. The latter is often what we use because it's easier to model mathematically.

My interpretation of Thompson's illustration of Model Land is that we should always remember that Model Land *is a different place than our world*. Sometimes we can find useful parallels between the two, but there's no guarantee. I like the metaphor of Model Land that Thompson weaves throughout this book because it reminds me that the temptation to create a tractable mathematical model is in tension with the model actually reflecting something about our world.

# Assumptions are non-negotiable

If you want to establish a mathematical result, there are two broad steps:
1. Identify your assumptions, which provides the starting point.
2. Use mathematical and logical reasoning to go from the assumptions in 1 to your desired result.

Putting aside the difficulty of how to execute these steps, once you've established the chain of reasoning, anyone can follow. In that sense, step 2 becomes mechanical in nature. But step 1 *isn't* mechanical. It's an inherent limitation.

Mathematics isn't in the business of discovering objective truths. Instead, it's all about discovering *conditional* truths.

If I start with X, then Y follows.

Not: Y is true all the time.

When we're in the land of mathematics, we can just wave our magic wands and proclaim that we have the assumptions we need in step 1. But when we want to connect our world to a mathematical one (forging a path between Model Land and our world), we need to be sure the assumptions we use to build our mathematical world mirrors our own.

And that's really hard! As Thompson writes in Chapter Four:

>Most real-world objects, by contrast, are not close to being mathematical idealisations.

Are assumptions can have huge consequences to the output of the model, which then can influence society at large. This is not to say we should throw out mathematical modelling altogether, but it means we should be more cautious about how much credence we assign to a model just because it's mathematical.

# Assumptions are often value judgements

Creating a model isn't just about mathematical analysis. To lay the foundation, you need to establish some core assumptions that you are working with. In a model of virus spreading, this might be the assumptions of how people clump together, shirk potential rules, and the degree to which each person is infectious (among many others). In an economics model, the assumptions will probably centre around the kind of decisions people make and what kind of products are in the market (among many others).

The point that Thompson tries to address is that these assumptions are often *value judgements*. They aren't neutral, though that may be how they appear. Rather, they are decisions baked into models by their creators, which often reinforce their beliefs. As Thompson warns in Chapter Six:

>Other choices are pragmatic, and it is these pragmatic ones that we should perhaps examine most carefully because they can reflect value judgements and experiences that are shared by the modellers but may be unrepresentative of wider society.

This passage both highlights the presence of value judgements in our models and a good reason for requiring diversity when building models. If we only those in one subset of the population (academics and scientists) build models, then we run the risk of calcifying the perspectives of that population into our models, which later affect *everyone*. I think it's fine to have expert modellers, but we should be aware of this gap.

Trust is another reason why it's worth reflecting on the value judgements we bake into models. If we end up creating models which affect all of society yet don't feel like they are working *for* society, then many people will become distrustful of models (for good reason!). In the context of forecasts in Chapter Six, Thompson says:

>But I think the issue here is not the rightness or wrongness of any forecasts; rather, it’s the perception that the interests of experts are not the same as the interests of the ordinary people.

And Thompson writes perhaps one of the best lines in the book just a bit earlier:

>The authority of expertise only exists when there is trust in expertise, and that is again a social question, not a mathematical one.

That last part of the sentence is key, and I would phrase a summary of the book like this: **Models are social constructions, not just mathematical ones.** If we want to create models that influence society, we have to reckon with how the very ingredients we bake into them aren't objective mathematical facts, but value judgements that arise from those who create them.

This gets back to the question of tractability and fidelity. We cannot make a model which is an exact replica of our world. This forces us to make assumptions and leave details out. And these choices are *not* objective, but depend on our values and what we want to focus on. That automatically makes our jobs as modellers one with social context, not just "objective" mathematics.

# Known and unknown unknowns

As I wrote above, we have no choice but to accept that models are only approximations of our world. The hope is that our assumptions only cause small deviations in the outputs of our models compared to what actually happens.

But our world has a *lot* of details. For some, we knowingly neglect or simplify. When I worked on my catapault design in my laboratory, my partner and I neglected the air friction in the room, thinking it wouldn't be dominant. If we *had* taken it into account, we probably would have reached for [a standard way of modelling air friction](http://hyperphysics.phy-astr.gsu.edu/hbase/airfri.html). Even if we had used these equations, it wouldn't have meant we captured air friction. Rather, it would mean that we better-approximated the effects of air friction.

Thompson states a much-needed reminder in Chapter Four:

>Most real-world objects, by contrast, are not close to being mathematical idealisations.

This is a deep truth, and it's the chasm that separates Model Land from our world. To make the analysis of a model tractable, we use assumptions. In the best scenario, we take into account all of the dominant phenomena that affect the model's outputs.

However, what happens if we cannot take something into account? Even if we *know* something might be relevant to the model, that doesn't imply we can treat it mathematically. It could be that we just don't have the right mathematical tools or, as is often the case, it's not at all clear how we would even *start* to include this aspect.

Thompson illustrates this in Chapter Four using the context of viruses:

>Viruses mutate regularly and the risk of death from one strain may be significantly different from the risk of death from another. I have no way of incorporating this possibility into my statistical analysis other than by looking up from my calculation and understanding it to be incomplete.

This quote is one that makes us more humble in our modelling efforts. We will rarely be able to capture everything into a mathematical model, so it's a good reminder to sometimes acknowledge that what you're doing is incomplete. That acknowledgement won't suddenly make your model better, but it may make it more trustworthy and transparent to others, because they know where the boundaries of the model are.

# Conclusion

This was easily my favourite non-fiction read in 2022. I also think it's the book in which I've made the most highlights. I found Thompson's style of writing very engaging, and I enjoyed each chapter.

I would say this book continues in the tradition of a few recent books such as [*Weapons of Math Destruction*](https://www.penguinrandomhouse.com/books/241363/weapons-of-math-destruction-by-cathy-oneil/), by Cathy O'Neil and [*Hello World*](https://hannahfry.co.uk/book/hello-world/), by Hannah Fry. These two books focus more on algorithms while Thompson focuses on models, but the ideas in these two other books are complementary. In particular, they all raise questions about who gets to build the mathematical machinery that powers our world, and what we miss when the creators lack diversity or perspective.

Though this book doesn't focus on my own field, I still found it valuable to ponder how I use models in my own work. The book has also made me more aware that when I come across models in other fields, I shouldn't just accept them because they are based on some fancy mathematics. I should be questioning their assumptions, their biases, and their blind spots.

Models aren't just fun research toys for academics. If that was the case, Thompson probably wouldn't have written this book. But as she explains in Chapter Six:

>It wouldn’t be so much of a problem if these were just siloed academics arguing in their ivory towers about the best abstract way to represent the universe. As I hope this book makes clear, though, we are all affected by the way mathematical modelling is done, by the way it informs decision-making and the way it shapes daily public conversations about the world around us.

Models aren't isolated objects. They are part of a societal feedback loop. We create models, and then they influence our decisions and actions, which stimulates the next generation of models. Thompson discusses this idea in the context of forecasts in Chapter Five:

>Models are not simple tools that we can take up, use and put down again. The process of generating a model changes the way that we think about a situation, encourages rationalisation and storytelling, strengthens some concepts and weakens others. The question of whether a model generates accurate predictions is important where it can be evaluated, but it can in certain circumstances be secondary to the way that it is used for decision support.

When it comes to modelling for society, we need to be more mindful and responsible about what goes into building the model. Who gets to take part? If there are many modelling efforts to predict the future, are we generating a diversity of models, or are we all developing one type? These are meta questions that go above just doing science and are more about how we collaborate and coordinate our scientific efforts when it comes to modelling for societal good.

I'm thankful to Thompson for writing this book. It's a great reminder for anyone who uses mathematical tools in their work that it's not just about the mathematics. As much as we might wish it were so, improving society isn't an objective process, but a social one. Which means we need to give more people access to creating, dissecting, acknowledging limitations to, and iterating on models. This is how we create models which are more trustworthy and equitable for all.

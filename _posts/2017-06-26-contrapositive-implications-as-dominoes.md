---

title: Contrapositive Implications as Dominoes
layout: post
permalink: /2017/06/26/contrapositive-implication
date: 2017-06-26 03:50:48-0400

---

If you've ever learned logic, you know that jumping from one piece of information to another (through implication) isn't always clear. You might remember something about if A implies B, then not B implies not A, and the like. What I want to do today is try and explore these concepts in a more visual way, which hopefully will let you remember these concepts with greater ease.

To do this, we're going to use an analogy that involves dominoes. We will start with three propositions or statements, and call them A, B, and C. These will each be represented by a domino, and they will be lined up in the same order.  Also note that I will just refer to these dominoes as A, B, and C from now on.

![Initial set up](/images/dominoes1.png)

Let's begin by imagining that we can only push a domino forward. That is, if we decide to knock down a domino, we need to push it to the right. This isn't any special condition, but it's just something that we will impose for now to make the situation more clear.

What happens if we push A? First, it will hit B, and then B will hit C. As such, we can say that A implies B, and B implies C. But, as we know from a chain of dominoes, the act of pushing A guarantees that C will fall, too (assuming you build your line well). As such, we can also say that A implies C.

![Implications](/images/dominoes2.png)

Let's look at a slightly different situation. What if I tell you that C falls? What can you tell me about A and B?

You might be tempted to say that A and B fall, but you should resist this conclusion! Remember, we want a statement that always applies, so it's helpful to go back to your dominoes to test the implications. If C falls, what are the options for what happened?

There are three different possibilities for what could have happened. 
- A was pushed, which we have already seen will guarantee that C falls. In this case, all three dominoes will fall.
- B is pushed, which we have also seen will cause C to fall. In this case, A is still upright, but the other two have fallen.
- C is pushed, which means it obviously falls. In this case, the other two are still standing.

Because having C fall means any one of these three options occurred, we cannot say with certainty what happened to the other dominoes. Both could have fallen, or only B could have fallen. We know that it can't be only A that fell, since that would imply the other two fell as well.

This might seem like a waste of time, because the conclusion we've come to is that having C fall tells us precisely nothing about the state of the other two. However, there's another way to look at these results that will give us insight. What if C had not fell? What could we say about the other two dominoes?

Let's look at it case by case. We know that pushing A automatically means C will fall. Likewise, pushing B means C will fall. Therefore, if we don't find that C has fallen, then we can be sure that neither A or B were pushed. There's simply no way to push the two first dominoes without causing the last one to fall.

This kind of statement is called the contrapositive. Formally, if we have a conditional statement, which is just a fancy way of saying that one smaller statement implies another, and it is of the form A implies B, then the contrapositive is given by not B implies not A. The way we write it is like this:

![Notation](/images/contrapositive.png)

Hopefully, the example of dominoes makes sense for why the contrapositive works. It's because we have a direct relationship of one domino causing a chain reaction with a bunch of other dominoes. If one part of the train further down has not fell, it has to be that the other parts have not fallen.

Practically, this means that you won't succumb to the error of thinking that if one event implies a second, then automatically having the second event occur implies the first. It could be true, just like we saw with our three options above, but when we are making use of logical implications, we want to use the fact that one thing guarantees the other. Therefore, when you're dealing with logical statements, think of the dominoes. Does having one statement happen imply the next, or is there another way it could have happened (without the first)?

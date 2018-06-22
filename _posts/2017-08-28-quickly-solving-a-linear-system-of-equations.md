---
title: Cramer's Rule for Solving Linear Systems
author: Jeremy
permalink: /2017/08/28/cramers-rule
date: 2017-08-28
---

Throughout secondary school, we learn about solving simple systems of equations. We learn that there are several methods (which are more or less the same thing): comparison, substitution, and elimination are the big three. We then go through tons of practice questions which all focus on doing this kind of solving. In particular, we solve systems of *two* equations, and I don't recall ever doing more than that. The sense I get from students is that solving these kinds of equations is sometimes confusing. I personally think it's because there's a lack of equivalence between the methods, so they all seem like pulling magic tricks out of a hat. That's a pedagogical/time problem, but I don't want to focus on that today. Instead, I want to focus on something that makes solving these systems of two equations super quick. It's called Cramer's rule, and this method makes it possible to forego using comparison, substitution, or elimination to solve for variables. Instead, you apply this procedure, and you can simply read off the answer.

Going with my new decision to do [examples first and theory second](_posts/2017-08-14-examples-before-abstraction.md), let's use the following system of equations:
$$
\begin{align}
5y +3x = 10, \\
2y-5x = 13.
\end{align}
$$
Solving this is a bit tedious. Personally, I would eliminate one of the variables, but there's no "right" way to do it. However, we're going to be clever, and change how we right these equations. Instead of writing two separate equations, we're going to write them as one *matrix* equation, which looks like this:
$$
\begin{bmatrix}
5 & 3 \\
2 & -5 \\
\end{bmatrix}
\begin{bmatrix}
x \\ y
\end{bmatrix}
=
\begin{bmatrix}
10 \\ 13
\end{bmatrix}.
$$
To make sense of how this works, I'll explain the three differents parts you see in this equation. The first block is called a 2 by 2 matrix, and it encodes the various coefficients of our system. The next part is our vector $\textbf{x}$, given by $\textbf{x} = (x,y)^T$. This is just our variables in the equation. Lastly, we have another vector, which is simply what our two equations are equal to when you write out the equations.

To see how this is equivalent to our above system of equations, we need to multiply the matrix by the vector on the left-hand side. If you've taken a linear algebra course, you remember that matrix multiplication is given by multiplying the row of the matrix by the column of the vector. As such, we would get:
$$
\begin{bmatrix}5 & 3 \\2 & -5 \\\end{bmatrix}\begin{bmatrix}x \\ y\end{bmatrix}
= \begin{bmatrix} 5x+3y \\ 2x - 5y \end{bmatrix}.
$$
Now, since this is a vector (in the sense that it has only one column, and a certain number of rows), we just match up the first component of this vector with the first component of the right hand side of our system. Similarly, we do the same for the second component, recovering our two first equations.

Let's name our matrix $A$, and our vectors $\textbf{x}$ and $\textbf{b}$, with the latter being the vector on the right hand side of our equation. We can then write this as:
$$
A \textbf{x} = \textbf{b}.
$$
Our end goal is to solve for $\textbf{x}$. Since the notation above looks a lot like regular algebra, we may be tempted to write the following:
$$
\textbf{x} = \frac{\textbf{b}}{A}.
$$
This temptation must be resisted! This is because we don't have a notion of what it means to divide a quantity by a matrix. You could make one up, of course, but in the standard theory of linear algebra, this operation isn't definied. However, there *is* a similar notion in linear algebra, and it's called the *inverse* of a matrix. The idea is simple. In regular multiplication (as I wrote about [here](_posts/2017-06-03-why-cant-i-divide-by-sin.md)), if we have a number (call it $c$), than its inverse is $c^{-1}$, so that we get $c*c^{-1} = 1$. It's that same idea here with matrix multiplication, except that instead of having the matrix multiplication being equal to one, it will be equal to the equivalent of matrix multiplication, which is called the *identity* matrix. It looks like this:
$$
I_n = \begin{bmatrix} 1 & 0 & \cdots & 0 \\
0 & 1 & \cdots & 0 \\
\vdots & \vdots & \vdots & \vdots \\
0 & 0 & \cdots & 1
\end{bmatrix}.
$$
Here, $n$ just refers to the dimension you want the matrix to be. Basically, the identity matrix is a matrix with zeros everywhere except for the diagonals, which are ones. The important part is that if you multiply any non-zero matrix or vector by the identity matrix, you get back the same vector/matrix.

With that out of the way, instead of *dividing* by our matrix $A$ from before to solve for $\textbf{x}$, we will multiply both sides of the equation by the inverse matrix $A^{-1}$. Doing so will give us:
$$
\textbf{x} = A^{-1} \textbf{b}.
$$
And that's how you solve the equation! Now, the only small detail you might be asking yourself is, "How do I find the inverse of a matrix?"

This is a good question, and in general it requires a long procedure of manipulating the rows of the matrix. However, for the case of a 2 by 2 matrix like we have in our example, there's a simple formula for the inverse of any 2 by 2 matrix with something called a non-zero determinant. The expression is given by:
$$
A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \rightarrow A^{-1} = \frac{1}{ad - bc} \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}.
$$
The denominator $ad-bc$ is the determinant of the matrix A, and we obviously need this to be non-zero so our fraction is defined. Apart from that, this gives us our expression for $A^{-1}$, which we can then throw into our equation above.

Doing exactly this with our original matrix gives:
$$
A = \begin{bmatrix} 5 & 3 \\ 2 & -5 \end{bmatrix} \rightarrow A^{-1} = \frac{1}{-31} \begin{bmatrix} -5 & -3 \\ -2 & 5 \end{bmatrix}.
$$
Therefore, solving our equation for our vector $\textbf{x}$ gives:
$$
\textbf{x} = \frac{1}{-31} \begin{bmatrix} -5 & -3 \\ -2 & 5 \end{bmatrix} \begin{bmatrix} 10 \\ 13 \end{bmatrix} = -\frac{1}{31} \begin{bmatrix} -89 \\ 45 \end{bmatrix}.
$$
Just like that, we have our answer. This is why it's nice to use this method for 2 by 2 systems. Calculating the inverse is very straightforward and efficient, so we can get our answer quickly without doing a bunch of substitutions.

You might be wondering if you can do this for larger systems, and the answer is most definitely *yes*. However, as soon as you go to 3 by 3 systems, it becomes much more time-consuming to calculate the inverse of your matrix, so it might be faster to do substitutions. I just wanted to outline the method here because it's much faster than the usual comparison, substitution, and elimination methods.

One thing to note though is that this isn't *quite* Cramer's rule. If you look at the "Applications" section of the [Wikipedia entry](https://en.wikipedia.org/wiki/Cramer%27s_rule) for Cramer's rule, the procedure is to simply compute the solution using the following:
$$
x_i = \frac{det(A_i)}{det(A)}.
$$
In this formula, you take your regular matrix $A$ as we saw before and take it's determinant (the denominator of the fraction). Then, the matrix $A_i$ is the same matrix as $A$ except that you replace the $i$-th coloumn with the vector $\textbf{b}$.

As such, if we wanted to calculate the first component of our solution vector (which is $x_1$), our matrix $A_1$ would be:
$$
A_1 = \begin{bmatrix} 10 & 3 \\ 13 & -5 \end{bmatrix}.
$$
Therefore, the determinant of this matrix is given by $det(A_1) = (10)(-5) - (13)(3) = -89$. And, the determinant of just our regular matrix $A$ as before is $det(A) = -31$. Putting this together gives us the first component of our solution:
$$
x_1 = \frac{89}{31}.
$$
You can check to see this is indeed the first component of our solution given by equation (11).

As such, this generalizes better to higher dimensions (by doing the swapping of columns of your matrix $A$), but I wanted to show the 2 by 2 case because it is very easy to follow. Now, you should be able to solve these systems much more easily than going through a long substitution.
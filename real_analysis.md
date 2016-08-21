# Real Analysis

This will begin with a description of real numbers, completeness, compactness, and some topology--ultimately leading to integration and differentiation. 

## Real Numbers

These are the numbers you and I know: 0, 1, -1, 1.5, and even $$\pi$$. 
**Rational** numbers are ones we can represent as an integer divided by another.
It turns out many numbers are **irrational** including $$\pi$$, $$\sqrt{2}$$, $$\sqrt{3}$$, and $$\sqrt{n}$$ for
any $$n$$ that's not a perfect square ($$\neq$$ a number squared). 

> **Idea**: use divisibility to show no rational number squared is 2. 
>
>  1. if $$\sqrt{2} = a / b$$, then $$ 2 = a^2 / b^2$$ $$\implies a^2$$ is divisible by 2 
>  2. So $$a$$ must be divisible by 2, implying $$b^2$$ is also divisible by 2, a contradiction!

More abstractly, the real numbers are uniquely determined by a handful of natural requirements on a set:
* field (operations: +, x with dentity, inverses, commutiativity, associativity, and distribution)
* order: trichotomy (either >, < or =)
* completeness (or least upper bound property)
  * this says, every set that has an upper bound has a *least* upper bound.

It turns out even in $$\mathbb{R}^n$$, a nice property about order called **Cauchy Schwarz** holds:

$$|\vec{u} \cdot \vec{v} | 
\leq 
|\vec{u}| | \vec{v} | $$

> #### Vectors and dot products
>
> a vector is a point in $$\mathbb{R}^n$$
> * it looks like $$(x_1, x_2, x_3)$$ where each $$x$$ is in $$\mathbb{R}$$
> 
> dot product is an operation on two vectors defined as:
> $$(x_1, x_2, x_3) \cdot (y_1, y_2, y_3) = x_1y_1 + x_2y_2 + x_3y_3$$

Finally, how many real numbers are there? 
Cantor showed there are actually uncountably many---you can never come up with a way to write a list of all real numbers even if you had all the time in the world.
> Idea: suppose someone claimed to have a list of all reals (this list would have to be infinite). Then, we write down a number that's different from each one on the list in the nth decimal place!

This is more stuff. 

> #### Title
>
> Content of mine

## Topology

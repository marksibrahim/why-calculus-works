# Real Analysis

This will begin with a description of real numbers, completeness, compactness, and some topology—ultimately leading to integration and differentiation.

## Real Numbers

These are the numbers you and I know: 0, 1, -1, 1.5, and even $$\pi$$. 
**Rational** numbers are ones we can represent as an integer divided by another.
It turns out many numbers are **irrational** including $$\pi$$, $$\sqrt{2}$$, $$\sqrt{3}$$, and $$\sqrt{n}$$ for
any $$n$$ that's not a perfect square \($$\neq$$ a number squared\).

> **Idea**: use divisibility to show no rational number squared is 2.
> 
> 1. if $$\sqrt{2} = a / b$$, then $$ 2 = a^2 / b^2$$ $$\implies a^2$$ is divisible by 2 
> 2. So $$a$$ must be divisible by 2, implying $$b^2$$ is also divisible by 2, a contradiction!

More abstractly, the real numbers are uniquely determined by a handful of natural **requirements** on a set:

* **field** \(operations: +, x with identity, inverses, commutiativity, associativity, and distribution\)
* **order**: trichotomy \(either &gt;, &lt; or =\)
* **completeness** \(= least upper bound property\)
  * every set with an upper bound has a _least_ upper bound.
  * e.g., \(0, 1\) has 1 as an upper bound, but 1 is not in the set \(0, 1\)


A nice consequence of this is the **triangle inequality: **$$ \| x + y \| \leq \|x\| + \|y\|$$ for any $$x, y \in \mathbb{R}$$.

> **Idea**: look at cases where x, y are positive \(Spivak has a nice proof of this\)

It turns out even in $$\mathbb{R}^n$$, a nice property about order called **Cauchy Schwarz** holds:


$$
|\vec{u} \cdot \vec{v} | 
\leq 
|\vec{u}| | \vec{v} |
$$


> #### primary::Vectors
> 
> a vector is a point in $$\mathbb{R}^n$$
> 
> * it looks like $$(x_1, x_2, x_3)$$ where each $$x$$ is in $$\mathbb{R}$$
> 
> dot product is an operation on two vectors defined as:
> 
> $$(x_1, x_2, x_3) \cdot (y_1, y_2, y_3) = x_1y_1 + x_2y_2 + x_3y_3$$

Finally, how many real numbers are there? 
Cantor showed there are actually uncountably many---you can never come up with a way to write a list of all real numbers even if you had all the time in the world.

> **Idea**: suppose someone claimed to have a list of all reals \(this list would have to be infinite\). Then, we write down a number that's different from each one on the list in the nth decimal place

Nevertheless, the set of rationals is countable. Make a table:

![](https://divisbyzero.files.wordpress.com/2013/04/screen-shot-2013-04-16-at-9-23-14-pm.png)

This is a great [TedEd video](http://ed.ted.com/lessons/how-big-is-infinity) discussing infinity and the reals.

> #### warning::Infinity + or -
> 
> is **not** in the set of real numbers

## Topology

### Distance

We can define a more general way to measure distance between two points in $$\mathbb{R}^n$$ \(or any vector space actually\), called a **norm**, denoted \|\| \* \|\|.

A norm is \(for $$x, y \in \mathbb{R}^n$$\):

1. _positive_ \(\|\|x\|\| &gt; 0, for all x in the set\); _definite_ \|\| x \|\| = 0 if and only if x =0

2. \|\|ax\|\| = a\|\|x\|\|, for any a in $$\mathbb{C}$$

3. _triangle_: $$ \| x + y \| \leq \| x \| + \| y \| $$


Common examples are Euclidean distance \(L2 norm\), Taxi Cab \(L1 norm\), and sup-norm \(returns the peak value across all dimesions of vector; sup is the least upper bound, which isn't always in the set of interest\).

> remember **vectors spaces** are sets with nice properties about addition and scalar multiplication

Norms in this context will later generalize to classes of functions with nice integration properties in measure theory.

> #### primary::L2 and Lp norms
> 
> 
> $$
> \left ( \sum_i  | x_i |^p \right )^{1/p}
> $$
> 
> 
> In the case of L2, p = 2 \(this will show up again in measure theory\).

### Neighborhoods

With a notion of distance \(often, we use L2 or Euclidean distance\), we can define **neighborhoods** or **open balls** around a point:

**B\(x; r\) **is a ball of radius r around x = set of points which are within a distance r of x \(strictly &lt; here\)

> formally, $$B(a; r) = \{ x \in set : \|\| x - a \|\| < r \}$$

A set is **open**, if for any point, there is an open ball \(of any radius\) _entirely contained_ in the set.

A set is **closed**, if the set's complement is open.

> #### warning::closed and open
> 
> are not mutually exclusive; a set can be both! \(for example $$\mathbb{R}$$ and $$\emptyset$$ \)

An **accumulation** \(or **limit point**\) of a set is one where every open ball centered at the limit point contains at least one other point in the set. Alternatively, we can think of a limit point as the limit of some sequence of points in the set.

This leads to another characterization of **closed** sets: sets that contain all their limit points.

### Bolzano-Weierstrass Theorem

every bounded sequence in $$\mathbb{R}^n$$ has a convergent subsequence.

> **bounded** means contained in a ball of finite radius

\[TODO: fill in proof and intuition from handwritten notes\]

### Covers, Compactness, and Heine-Borel Theorem

\[TODO: fill in from handwritten notes\]

## Limits and Continuity

The limit, call it L, of a sequence of real numbers $$a\_n$$, is denoted


$$
\lim_{n \rightarrow \infty} a_n = L
$$


This means for any number $$\epsilon > 0$$, there exists $$N$$ such that for all $$n > N$$,


$$
| L - a_n | < \epsilon
$$


> we can substitute \| \| with any norm

The idea is that if we go out far enough in the sequence, the terms are _very close to the limit_ value L.

We can also talk about the limit of a function. In this case, we specify inputs to be within $$\delta$$ of some input to achieve an output within $$\epsilon$$ of the desired limit.

### Convergence

a sequence, $$a\_n$$, **converges** to some value $$p$$ if $$\lim_{n \rightarrow \infty} a_n = p$$ \(sometimes denoted $$a\_n \rightarrow p$$\).

a sequence, $$a\_n$$, is **cauchy** if terms in the sequence eventually become close to each other. Formally, given any $$\epsilon > 0$$, $$| a_n - a_m | <  \epsilon$$ for all n &gt; N and m &gt; M \(for some N, M $$\in \mathbb{N}$$\).

\[in progress...\]


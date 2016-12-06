The magic of the infinitesimal: limits, functions, and derivatives.

## Limits and Continuity

The limit, call it L, of a sequence of real numbers $$a\_n$$, is denoted


$$
\lim_{n \rightarrow \infty} a_n = L
$$


This notation means for any number $$\epsilon > 0$$, there exists $$N$$ such that for all $$n > N$$,


$$
| L - a_n | < \epsilon
$$


> we can substitute \| \| with any norm

The idea is that if we go out far enough in the sequence, the terms are _very close to the limit_ value L.

We can also talk about the limit of a function. In this case, we specify inputs to be within $$\delta$$ of some input to achieve an output within $$\epsilon$$ of the desired limit. As you'd expect, limits of functions split as you'd expect over +, -, x, and / (so long as denominator isn't approaching zero). 

### Convergence

A sequence, $$a\_n$$, **converges** to some value $$p$$ if $$\lim_{n \rightarrow \infty} a_n = p$$, sometimes denoted $$a_n \rightarrow p$$. That is by choosing any term far enough in the sequence, the term will be very close to p. How close? As close as you we'd like. The closer, the farther we'll set our threshold. 

> we can show this idea of convergence is not insane, because we can prove a sequence can only converge to a single point (see Apostol Theorem 4.2).


A sequence, $$a\_n$$, is **cauchy** if terms in the sequence eventually become **close to each other**. Formally, given any $$\epsilon > 0$$, 
$$
| a_n - a_m | <  \epsilon
$$
 for all n &gt; N and m &gt; M \(for some N, M $$\in \mathbb{N}$$\).
 
 
Since the terms are eventually arbitrarily close to one other, it turns out every Cauchy sequence in $$\mathbb{R}^n$$ converges ! Outside of $$\mathbb{R}^n$$, a similar phenomenon will happen, but the point to which the terms are converging may not be in the space. 
> think 1, 1/2, 1/3, ... in the space [1, 0); zero isn't there! 

Metric spaces where every Cauchy sequence converges are called **complete**.

\[in progress...up to 4.8 in Apostol\]


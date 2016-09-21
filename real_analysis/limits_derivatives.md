Here, I'll talk about limits, functions, and derivatives. 

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

A sequence, $$a\_n$$, **converges** to some value $$p$$ if $$\lim_{n \rightarrow \infty} a_n = p$$ \(sometimes denoted $$a\_n \rightarrow p$$\).

A sequence, $$a\_n$$, is **cauchy** if terms in the sequence eventually become close to each other. Formally, given any $$\epsilon > 0$$, $$| a_n - a_m | <  \epsilon$$ for all n &gt; N and m &gt; M \(for some N, M $$\in \mathbb{N}$$\).

\[in progress...\]


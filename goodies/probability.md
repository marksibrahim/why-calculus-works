# Distributions

## Binomial Distribution

describes the number of successes in a sequence of n independent trials, each with probability p of success

$$P(k \text{ successes}) = \binom{n}{k} p^k (1 - p)^{n-k}$$$$x = y$$$$x = y$$

Recall, $$\binom{n}{k} = \frac{n!}{k!(n-k)!}$$

The **Bernoulli Distribution** is a is a special case of a Binomial Distribution where a single experiment is conducted \(a single coin flip, with potentially unfair coins\).

A **multinomial distribution** generalizes the binomial distribution, by allowing the number of outcomes to be more than two. There are k outcomes, each with probability $$x = y$$ of occurring, leading to

$$P(x_1, x_2, \dots, x_k) = \frac{n!}{x_1! x_2! \dots x_k!} p_1^{x_1} \dots p_k^{x_k}$$

where x\_i is the number of times outcome i occurred and n is the number of trials. This is applicable to determining the outcome of a dice or sampling from a bag of different colored balls with replacement and determining the probability of grabbing 2 red, 3 brown, and 5 yellow balls.

## Poisson Distribution

is useful for count data: how many success over n trials \(with "weak independence"\) and possibly different, but small probability of success?

Examples include: how many floods in a year? how many emails per day? etc.

$$P( k \text{ events in interval}) = \frac{\lambda^k e^{-\lambda}}{k!}$$

Lambda is the expected number of occurrence—this can be shown by computing the expected value over n trial.

It also turns out that when n is large and p is very small, Poisson Distribution approach a Binomial Distribution.

## Beta Distribution

Flexible family of continuous distributions on \[0, 1\]. Beta distributions are defined by two parameters:$$\alpha, \beta$$, . It's often used for characterizing prior probabilities in Bayesian modeling.

![](/assets/Beta_distribution_pdf.svg)

The Beta distribution is the **conjugate prior** of the binomial distribution, meaning if you start with "likelihood function", P\(X \| p\) ~ Binomial\(n, p\) and a prior = f\(p\) ~ Beta, then the posterior P\(p \| X=k\) ~ Beta. 

> In general, if the prior and posterior probabilities are in the same family, they are said to be **conjugate distributions**.

# Goodies

## Chain Rule of Conditional Probabilities

A joint probability over several random variables can be decomposed using the "chain rule for probability"

$$P(x_1, x_2, \dots, x_n) = P(x_1) * [ P(x_2 | x_1, x_3, \dots, x_n) * P(x_3 | x_1, x_2, \dots, x_n) * \dots]$$

## Gamma Function

is an extension of factorial to all reals/complex numbers

For postivie integer n, it's  ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/8657e8abd0241c92c2c48e4ff5041394098ded90 "\Gamma \(n\)=\(n-1\)!.")

For complex numbers with positive real component, ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/5ec163a2e987909af37e1f8d6975b7080f8278e8 "{\displaystyle \Gamma \(z\)=\int \_{0}^{\infty }x^{z-1}e^{-x}\,\mathrm {d} x.}")

This ends up popping up in many distributions, especially beta!


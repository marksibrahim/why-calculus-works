# Distributions

## Binomial Distribution

describes the number of successes in a sequence of n independent trials, each with probability p of success

$$P(k \text{ successes}) = \binom{n}{k} p^k (1 - p)^{n-k}$$$$x = y$$$$x = y$$

Recall, $$\binom{n}{k} = \frac{n!}{k!(n-k)!}$$

The **Bernoulli Distribution** is a is a special case of a Binomial Distribution where a single experiment is conducted \(a single coin flip, with potentially unfair coins\).

A multinomial distribution \[TODO\]



## Poisson Distribution

is useful for count data: how many success over n trials \(with "weak independence"\) and possibly different, but small probability of success?

Examples include: how many floods in a year? how many emails per day? etc.

$$P( k \text{ events in interval}) = \frac{\lambda^k e^{-\lambda}}{k!}$$

Lambda is the expected number of occurrence—this can be shown by computing the expected value over n trial.

It also turns out that when n is large and p is very small, Poisson Distribution approach a Binomial Distribution.

# Chain Rule of Conditional Probabilities

A joint probability over several random variables can be decomposed using the "chain rule for probability"

$$P(x_1, x_2, \dots, x_n) = P(x_1) * [ P(x_2 | x_1, x_3, \dots, x_n) * P(x_3 | x_1, x_2, \dots, x_n) * \dots]$$




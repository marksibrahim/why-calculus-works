# Complex Analysis

# Complex Plane

Why Complex Numbers? As Bombelli pondered the solutions to $$x^3 = 5x + 3$$, he discovered it's useful to consider not just real number, but complex numbers too. The set of complex numbers, $$\mathbb{C}$$, is called the **Complex Plane**. We can think of the complex plane, as a set of points $$x + i y$$ where $$x, y \in \mathbb{R}$$. In other words, we can think of complex numbers as numbers in $$\mathbb{R}^2$$.

## Polar Coordinates

We can express complex numbers \(denoted usually as z or w\), using polar coordinates: a length and angle. Often we write $$z$$ as

$$z = \cos(\theta) + i \sin(\theta)$$

* angle is often called the **argument **
  * a **principal argument **is one where $$\theta$$ is between $$\pi, -\pi$$.


> e.g., Arg\(1 - i\) = $$\frac{- \pi}{4}$$

The lenght of numbers in the complex plane, called the **modulus, **is computed as: $$\| z \| = \sqrt{ x^2 + y^2 }$$

The **complex conjugate** of a number $$z$$, denoted $$\bar{z} = x - i y$$.

**De Moivre's Formula**

Since we know** **$$(e^{i\theta})^n = e^{i n \theta}$$ and that $$e^{i \theta} = cos(\theta) + i \sin(\theta)$$ \(Euler's Formula\),  De Moivre's Formula is the observation that:

$$\cos(\theta) + i sin(\theta) = \cos(n \theta) + i \sin(n \theta)$$

> $$e^{i \theta} = \cos \theta + i \sin \theta$$, because the real and imaginary parts of $$e^{i x}$$ correspond to the power series of $$\cos$$ and $$\sin$$.

The triangle inequality and field axioms still hold in $$\mathbb{C}$$

## Nth Roots

An nth root of a complex number, $$w$$, is a number $$z$$ such that $$z^n = w$$. An important type of nth root are the **nth roots of unity**, which are numbers whose nth power is 1.

> #### primary::roots unity
> 
> There are n numbers satifying $$z^n = 1$$. Why?
> 
> Let's think in polar coordinates: $$r e^{i n \theta} = 1 $$. Then r =1 and $$n \theta = 2 \pi k $$ for k $$\in \mathbb{Z}$$. We then have $$\theta = 0, 2 \pi / n, 4 \pi / n, \dots$$ there are n unique angles!

We can think of other nth roots as roots of unity corrected for length.

# Complex Functions

A complex function is continuous in the complex plane in an analogous way as it is in the reals. Also note, the Extreme Value Theorem holds in the complex plane as it does in the reals: a continuous function on a compact set attains its min\/max.

A compelx function on an open set in $$\mathbb{C}$$ is **holomorphic** \(**analytic**\) at a point z\_0 if the dervative at z\_0 exists. Note the key difference between a real and compelx derivative is that you can approach a complex point z\_0 from infinitely many directions, not just left or right—it's a much stronger condition.

Nice Properites:

• sum\/product of holomorphic functions is holomorphic

• quotient, f\/g, of holomorphic functions such that g\(z\_0\) ≠ 0, is also holomorphic

We can also think of a complex function as a function in $$\mathbb{R}^2$$ where f = u\(x, y\) + i v\(x, y\), with v, u real-valued function on the real plane.

The **Jacobian **of a function f\(x, y\) is matrix of partial derivatives. It turns out a holomorphic function at a point satisfies the **Cauchy Riemann Equations**:


$$
\frac{\partial u}{\partial x} = \frac{\partial v }{\partial y}
$$


and


$$
\frac{\partial u}{\partial y} = - \frac{\partial v }{\partial x}
$$


> use limits to show this is true with the realization the derivative should be the same regardless of the direction you approach the point with.



Furthermore, if u and v have continuous derivatives \(continuously differentiable\) and the Cauchy Riemann Equations hold then f is **holomorphic** \(in the open set on which f is defined\). 





\[in progress\]

## Text Reference

_Complex Analysis_, by Stein and Shakarchi

## Other references

_A First Course In Complex Analysis_, by Beck, Marchesi, Pixton, and Sabalka

_Functions of One Complex Variable_, by John Conway \(used in Course\)


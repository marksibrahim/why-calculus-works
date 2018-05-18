# Calculus Computations

## Derivatives

$$ \frac{d\ ln(x)}{d x} = \frac{1}{ x}$$

> why? We know $$e^{\ln(x)}$$ = x, so $$ \frac{d\ e^{ln(x)}}{dx} = \frac{d\ x}{dx} = 1$$.
>
> This with the chain rule gives us
>
> $$ \frac{d e^{\ln(x)}}{dx} = e^{\ln(x)} \frac{d\ \ln(x)}{dx} = 1$$ , implying $$\frac{d\ \ln(x)}{dx} = 1/x$$

## Differentiability in R^n

F from R^m to R^n is differentiable at x\_0 if there exists a matrix A such that

$$\lim_{x \rightarrow x_0}  \frac{|| F(x) - F(x_0) - A(x - x_0) || }{||x - x_0||} = 0$$

It turns out if A exists, it must be the **Jacobian** \(first order partial derivatives\)!

## Convexity

### Sets

A **set is convex** if the **line between any two points** is in the set. Formally, this means


$$
\text{ For all } a, b \in S, 

 \lambda a + (1 - \lambda) b \in S
$$


where $$ 0 \leq \lambda \leq 1$$

Circles, triangles are all convex sets. Pacman isn't, because you can draw with a part outside the set.

### Functions

A function is convex if the** line connecting any two points** is above the function. This can be defined formally using a parameter $$\lambda$$similar to the definition for sets.

Who cares? Convex function have a **single global minimum**, so algorithms such as gradient descent work well, because they don't get stuck in global optima.

We can test for convexity using the **second derivative test** as well! If f'' &gt; 0, then f is convex.

## Line \(path\) Integrals

A line integral means the same thing as a path, contour \(typically line integral in the complex plane\), or curve integrals.

Curves: can be described parametrically, as  c\(t\) = \(x\(t\), y\(t\), z\(t\)\) for a parameter t.

> a circle is described as x^2 + y^2 = r^2, can also be parametrized as x = rcos\(t\), y = r sin\(t\)

The path integral of a function f along the curve is defined as:

$$ \int_c f(x, y, z) ds = \int_a^b$$ f\(c\(t\)\) • c'\(t\) dt

or alternatively


$$
 \int_c f(x, y) ds = \int_a^b f(x(t), y(t)) || c'(t) || dt
$$



$$
 = \int_a^b f(x(t), y(t)) \sqrt{(\frac{dx}{dt})^2 + (\frac{dy}{dt})^2} dt
$$


In words it's the change in output \* change in input \(along the line\):![](/assets/import.png)

## Green's Theorem

In the context of F a vector field, meaning a function that maps a point to a vector, such as F\(x, y\) = \( P\(x, y\), Q\(x, y\) \),

for c a closed curve and D the region inside,

$$ \int_c P dx + \int_c Q dy = \int \int_D d Q / dx - dP / dy dA $$

In essence, Green's theorem relates line integrals to the double integral over a region.

## Divergence

Also in the context of a vector field F,

div\(F\) = $$\nabla \cdot F = dP/dx + dQ/dy$$

This generalizes to arbitrary dimensions. The **divergence theorem** relates integrals along the boundary of a region to the triple integral of div\(F\) over the region.

## Curl

Only for vector fields in R^3. It's the cross product of

$$div(F) = \nabla \times F$$$$ $$

Since cross product is only defined in R^3, curl is also restricted to R^3. **Stoke's theorem** relates curl to the integral of F along a closed curve.

# Resources

* a list of important counter-examples. such as a function that's continuous at only a single point: [http://www.math.tamu.edu/~tom.vogel/gallery/gallery.html](http://www.math.tamu.edu/~tom.vogel/gallery/gallery.html)
* 



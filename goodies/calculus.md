# Calculus Computations

## Derivatives

$$ \frac{d\ ln(x)}{d x} = \frac{1}{ x}$$

> why? We know $$e^{\ln(x)}$$ = x, so $$ \frac{d\ e^{ln(x)}}{dx} = \frac{d\ x}{dx} = 1$$.
>
> This with the chain rule gives us
>
> $$ \frac{d e^{\ln(x)}}{dx} = e^{\ln(x)} \frac{d\ \ln(x)}{dx} = 1$$ , implying $$\frac{d\ \ln(x)}{dx} = 1/x$$

## Line \(path\) Integrals

A line integral means the same thing as a path, contour \(typically line integral in the complex plane\), or curve integrals.

Curves: can be described parametrically, as  c\(t\) = \(x\(t\), y\(t\), z\(t\)\) for a parameter t. 

> a circle is described as x^2 + y^2 = r^2, can also be parametrized as x = rcos\(t\), y = r sin\(t\)

The path integral of a function f along the curve is defined as:

$$ \intc f(x, y, z) ds = \int$$
$$
 \int_c f(x, y) ds = \int_a^b f(x(t), y(t)) || c'(t) || dt
$$
$$ $$

$$ $$
$$
 = \int_a^b f(x(t), y(t)) \sqrt{(\frac{dx}{dt})^2 + (\frac{dy}{dt})^2} dt
$$
In words it's the change in output \* change in input \(along the line\):![](/assets/import.png)


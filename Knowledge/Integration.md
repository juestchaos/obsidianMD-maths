#methods

# Anti-differentiation (indefinite integrals)
This process is used to find the [[Functions|function]] whose [[derivative]] is inside the indefinite integral.
$$ \int f'(x)\ dx = f(x) + c $$

the $+\ c$ term is due to the fact that vertical translation of a function does not affect its derivative, meaning that when integrated again this information is still lost. To find this $c$ term a point must be given to substitute back into $f(x)$.

The indefinite integral of a term $x^n$ is:

$$ \int ax^n\ dx = \frac{ax^{n+1}}{n+1} $$

### Properties

Integration is distributive over addition and subtraction:
$$ \int f(x) + g(x) \ dx = \int f(x)\ dx + \int g(x)\ dx $$

Integration is not affected by whether a constant is integrated, ie:
$$ \int kf(x) = k\int f(x) $$

## Reverse chain rule
The reverse chain rule is used to find the integral of composite functions where the [[Derivative#Chain rule|chain rule]] would be used to find their derivatives.
$$ \int f(g(x)) = \frac{\int f(g(x))dx}{g'(x)} $$
$$ \int f(g(x)) = \int f(g(x)) dx \cdot \frac 1{g'(x)} $$

# Definite integrals
A definite integral an integral within a specified domain, expressed as
$$ \int_a^b f(x)\ dx $$
This returns a scalar.

To calculate a definite integral:
$$ \int_a^b f(x)\ dx $$
$$ = \left[F(x)\right]_a^b $$
$$ = F(b)-F(a) $$
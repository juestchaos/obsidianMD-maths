#methods

# Anti-differentiation (indefinite integrals)
This process is used to find the [[Functions|function]] whose [[derivative]] is inside the indefinite integral.
$$ \int f'(x)\ dx = f(x) + c $$

the $+\ c$ term is due to the fact that vertical translation of a function does not affect its derivative, meaning that when integrated again this information is still lost. To find this $c$ term a point must be given to substitute back into $f(x)$.

### Properties

Integration is distributive over addition and subtraction:
$$ \int f(x) + g(x) \ dx = \int f(x)\ dx + \int g(x)\ dx $$

## Reverse chain rule
The reverse chain rule is used to find the integral of composite functions where the [[Derivative#Chain rule|chain rule]] would be used to find their derivatives.
$$ \int f(g(x)) = \frac{\int f(g(x))dx}{g'(x)} $$
$$ \int f(g(x)) = \int f(g(x)) \cdot \frac 1{g'(x)} $$
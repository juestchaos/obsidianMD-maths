---
tags: [methods]
aliases: [differentiation, derivatives]
---

Links: [[Integration]]

# Derivatives

Given the function $f(x)$, its derivative $f'(x)$ is the function which gives the gradient of the tangent to $f(x)$ for all real values of $x$. To find this original function $f(x)$, use [[Integration|integration]].

## First principles demonstration of a derivative
Let us define the function $f(x) = x^2$. The gradient of this function between two points $x$ and $x+h$ can be expressed as the $$\frac{f(x+h)-f(x)}{(x+h) - x}$$ or more simply as $$\frac{f(x+h)-f(x)}{h}$$

To find the gradient at a single point, we must find determine the value this fraction is equivalent to for smaller and smaller values of $h$. However, if $h=0$, we run into a problem, since dividing by zero is undefined. To get around this, we instead express it as a _limit_ as so:
$$f'(x) = \lim_{h \to 0} \frac{f(x+h)-f(x)}{h}$$

We can now subsitute in our function, which in this case is $x^2$. Doing so produces:
$$f'(x) = \lim_{h \to 0} \frac{(x+h)^2-x^2}{h}$$

Expanding this:
$$f'(x) = \lim_{h \to 0} \frac{x^2+2xh+h^2-x^2}{h}$$

$x^2 - x^2 = 0$, so:
$$f'(x) = \lim_{h \to 0} \frac{2xh+h^2}{h}$$

We now have $h$ in every term of the numerator, so it can be cancelled:
$$f'(x) = \lim_{h \to 0} 2x+h$$

The limit can now be evaluated, since $h=0$ is now defined:
$$f'(x) = 2x $$



## Power rule
A simplified way of finding the derivative of a non-linear function, rather than deriving from first principles, is to use the _power rule_, which states that the derivative of a non-linear function is the sum of the derivatives of its terms, and that for a term $ax^n$, its derivative is $anx^{n-1}$. The opposite of this process is [[Integration#Anti-differentiation indefinite integrals|integration]]

## Chain rule
Some [[functions]] can be expressed as two functions nested inside one another, such as
$$f(x) = (2x+2)^2 $$
This can be represented as two functions $g(x) = x^2$ and $h(x) = 2x+2$.
$$f(x) = g(h(x)) $$

The chain rule states that 
$$f'(x) = g'(h(x))\cdot h'(x) $$

## Derivatives of types of functions

### Polynomials
Use the [[Derivative#Power rule|power rule]] 


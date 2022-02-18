<<<<<<< HEAD
---
aliases: 
tags: methods
---

Links: [[Integration]]

# Area between two curves

For any two [[functions]] $f(x)$ and $g(x)$, as long as $f(x) > g(x)$, the area between the two over the domain $[a,b]$ is

$$A = \int_a^bf(x)dx - \int_a^bg(x)dx $$

Since integration is distributive over addition, this can be simplified to

$$A = \int_a^bf(x)-g(x)\ dx $$

However, in the case where $f(x) > g(x)$ is not true over the domain $[a,b]$, we must find the point(s) of intersection $c_n$, since the section where $g(x) > f(x)$ would be counted as negative area. This means that we must break up our integral into two parts:

$$ A = \int_a^c f(x)-g(x)dx + \int_c^b g(x)-f(x)dx $$

To simplify this, we can switch the order of $f(x)$ and $g(x)$, since this only changes the sign of the answer ($+$ or $-$), and take the absolute value of each part.

$$ A = \left|\int_a^c f(x)-g(x)dx\right| + \left|\int_c^b f(x)-g(x)dx\right|$$
=======
Links: [[Integration]]
# Area between two curves
For any two functions $f(x)$ and $g(x)$, as long as $f(x) > g(x)$, the area between the two over the domain $[a,b]$ is
$$A = \int_a^bf(x)dx - \int_a^bg(x)dx $$
Since integration is distributive over addition, this can be simplified to
$$A = \int_a^bf(x)-g(x)\ dx $$
>>>>>>> origin/main

---
tags: [specialist]
---



# 3-dimensional vectors
Vectors can exist in three dimensions. To remember which direction is which in 3D space, use the right-hand rule: pointer finger points towards $x^+$, middle finger points towards $y^+$ and the thumb then points towards $z^+$.

3D vectors are expressed as
$$\vec u = x\hat i + y\hat j + z\hat k$$

## Magnitude
The magnitude of a 3D vector is the same as a 2D vector:
$$ |\vec u| = \sqrt{x^2+y^2+z^2} $$

## Spherical form
Since we are now in 3D space, three parameters are needed to define a point. This means that we need two angles and a magnitude to define a vector.

To do this, we use a spherical coordinate system, where we define a sphere of radius $r$ and then specify a horizontal angle $\theta$, measured on the $xy$ plane from the x-axis, and a vertical angle $\phi$, measured from the x-y plane, on this sphere.

The angle $\theta$ will always be $-\pi \leq \theta\leq \pi$, and the angle $\phi$ will always be $-\frac{\pi}{2} \leq \phi \leq \frac{\pi}{2}$

To convert a vector $u$ to polar form, find the angle $$\theta = \tan ^{-1}\left(\frac{y}{x}\right)$$ and the angle $$\phi = \sin^{-1}\frac{z}{|u|}$$

### Conversion from spherical form to rectangular form
The formula is 
$$ \vec u = r\cos\phi\cos\theta\hat i + r\cos\phi\sin\theta\hat j + r\sin\phi\hat k $$
This formula is simply $x\hat i + y\hat j + z\hat k$, except that in the x-y plane the magnitude is the horizontal component of the vector $r\cos\phi$.

## Distance between two points on a sphere


## Vector projection in 3 dimensions
To project a vector onto another in three dimensions, first find the scalar projection $|\vec c|$, or the magnitude of the vector projection. This is equal to
$$|\vec c| = \frac{a\cdot b}{|b|}$$

The vector projection can then be found:
$$\vec c = \frac{a\cdot b}{|b|^2}\cdot \hat b $$

### Vector rejection
The vector rejection $d$ is the perpendicular component of $a$ relative to $b$.
$$\vec d = \vec a - \frac{a\cdot b}{|b|^2} \cdot \hat b $$

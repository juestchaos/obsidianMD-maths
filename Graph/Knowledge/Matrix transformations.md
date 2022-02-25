#todo Add rotation

# Matrix Transformations

## Linear transformations

Transforming a matrix 

### Reflection

A reflection can be performed across any line which passes through the origin $y=mx$ using a linear transformation. This is better expressed as $y=\tan(\theta) x$ since $m=\tan\theta$.

For a given line $y=\tan\theta x$, reflections of $\hat i$ and $\hat j$:

$$\hat i=(1, 0) \rightarrow \hat i'=(\cos2\theta,\sin2\theta) \\ \hat j = (0, 1) \rightarrow \hat j' = (\sin2\theta, -\cos2\theta) \\ \therefore M_{y=\tan\theta x}=\left[\begin{matrix} \cos2\theta & \sin2\theta \\ \sin2\theta & -\cos2\theta\end{matrix}\right]$$

#### Finding $\theta$ from $m$

To make life easier, $\theta$ will be strictly $-\frac{\pi}{2} \leq \theta \leq \frac{\pi}{2}$. This means that this is the one and only time you can put $\tan ^{-1}$ into the calculator and write down whatever the answer is.

#### An example

Transform the point $(3, 4)$ by reflecting it across the line $y= -\frac{\sqrt{3}}{3}x$.

$$\tan\theta= -\frac{\sqrt{3}}{3}, \left(-\frac{\pi}{2} \leq \theta \leq \frac{\pi}{2}\right) \\ \theta=\frac{-\pi}{6}$$

$$M_{y=\tan\left(\frac{-\pi}{6}\right)x} = \left[\begin{matrix} \cos\frac{-\pi}{3} & \sin\frac{-\pi}{3} \\ \sin\frac{-\pi}{3} & -\cos\frac{-\pi}{3}\end{matrix}\right] \\ =\left[\begin{matrix}\frac{1}{2} & \frac{-\sqrt{3}}{2} \\ \frac{-\sqrt{3}}{2} & \frac{-1}{2}\end{matrix}\right] \\ =\left[\begin{matrix}\frac{1}{2} & \frac{-\sqrt{3}}{2} \\ \frac{-\sqrt{3}}{2} & \frac{-1}{2}\end{matrix}\right] \left[\begin{matrix}3 \\ 4\end{matrix}\right] \\ = \left[\begin{matrix}\frac{3}{2} & -2\sqrt{3} \\ \frac{-3\sqrt{3}}{2} & -2 \end{matrix}\right]$$

### Dilation

Dilation affects the area of the shapes it dilates.

The matrix which dilates along the $x$-axis is

$$D_x=\left[\begin{matrix} k & 0 \\ 0 & 1\end{matrix}\right]$$

Dilation along the y-axis is similar:

$$D_y=\left[\begin{matrix} 1 & 0 \\ 0 & k\end{matrix}\right]$$

Dilation along both x- and y-axes:

$$D_k=\left[\begin{matrix} k & 0 \\ 0 & k\end{matrix}\right] = kI$$

### Translation

A translation is not a linear transformation since it results in the origin moving. 

$$\left[\begin{matrix}x'\\y'\end{matrix}\right] = \left[\begin{matrix}x\\y\end{matrix}\right] + \left[\begin{matrix}-3\\2\end{matrix}\right]$$

$$T_{a, b}=\left[\begin{matrix}a\\b\end{matrix}\right]$$

### Composite transformations

Determine a matrix $L$ which

1. Rotates by $\frac{\pi}{2}$
2. 

### Area after a transformation

The magnitude of the determinant of the transformation matrix $|\det T|$ is the scale factor for the area of any shape.
# **Lecture 5: Analisis Variabel Kompleks**

1. Teorema Crouchy-Riemann
2. Teorema Integral Cauchy
3. Teorema Derivative Cauchy
4. Principal Argument dan Teorema Rouche

## **Analytic Function**

* $f(z) = e^z = e^x \cos x + je^x \sin y$ is analytic everywhere.

$$
\frac{\delta u}{\delta x} = e^x \cos y = \frac{\delta v}{\delta y}, \quad \frac{\delta u}{\delta y} = -e^x \sin y = - \frac{\delta v}{\delta x}
$$
and all the partial derivatives are continuous

* $f(z) = (z+1)(z^2+1)$ is analytic on **C**
* $f(z) = \frac{(z^3+1)}{(z^2-1)(z^2+4)}$ is analytic on **C** except at
$$
z =\pm 1, \quad \text{and} \quad z = \pm j2
$$

* $f(z) = xy + jy$ is not analytic everywhere because
$$
\frac{\delta u}{\delta x} = y \neq 1 = \frac{\delta v}{\delta y}, \quad \text{and} \quad \frac{\delta u}{\delta y} = x \neq 0 = -\frac{\delta v}{\delta x}
$$

## **Theorem of Analytic Function**
let $f$ be an analytic function everywhere in a domain $D$

**Theorem:** if $f'(z) = 0$ everywhere in $D$ then $f(z)$ must be constant on $D$

**Theorem:** if $f'(z)$ is real valued for all $z \in D$ then $f(z)$ must be constant on $D$

* Example 1

    The quotient
    $$
    f(z) = \frac{z^3+4}{(z^2-3)(z^2+1)}
    $$
    
    is analytic throughout the z plane except for the singular points
    $$
    z = \pm \sqrt{3} \And z = \pm i
    $$

* Example 2 <br>
    Suppose that a function $f(z) = u(x,y) + iv(x,y)$ and its conjugate $f(z) = u(x,y) - iv(x,y)$ are both analytic in a given domain $D$. Show that $f(z)$ must be constant throughout $D$.

    **Proof:**
    $$
    f(z) = u(x,y) + iv(x,y) \quad \text{is analytic, then} \quad u_x = v_y,u_y = -v_x
    $$
    $$
    f(z) = u(x,y) - iv(x,y) \quad \text{is analytic, then} \quad u_x = -v_y,u_y = v_x
    $$ 
    $$
    \Rightarrow u_x = 0, v_x = 0 \Rightarrow f'(z) = u_x + iv_x = 0
    $$

* Example 3 <br>
    Suppose that $f$ is analytic throughout a given region $D$, and the modulus $|f(z)|$ is constant throughout $D$, then the function $f(z)$ must be constant there too. 

    **Proof:** <br>
    $ |f(z)| = c$, for all $z$ in $D$ <br>
    where $c$ is real constant. <br>
    If $c=0$, then $f(z)=0$ everywhere in D. <br>
    If $c\neq 0$, we have 
    $$
    f(z)\overline{f(z)} = c^2 \Rightarrow \overline{f(z)} = \frac{c^2}{f(z)}, f(z) \neq 0 \in D
    $$
    !!! note "Note"

        Both $f$ and it conjugate are analytic, thus $f$ must be constant in $D$.

## **Harmonic Function**

the equation
$$
\frac{\delta u(x,y)}{\delta x^2} + \frac{\delta u(x,y)}{\delta y^2} = 0
$$
is called **Laplace's equation**<br>
we say a function $u(x,y)$ is **harmonic** if

* the first-and second-order partial derivatives exist and are continuous
* $u(x,y)$ satisfy Laplace's equation

**Theorem:** if $f(z) = u(x,y) + jv(x,y)$ is analytic in a domain $D$ then $u$ and $v$ are harmonic in $D$

**example:** $f(z) = e^{-y} \sin x - je^{-y} \cos x$

* $f$ is entire because

$$
\frac{\delta u}{\delta x} = e^{-y} \cos x = \frac{\delta v}{\delta y}, \quad \frac{\delta u}{\delta y} = -e^{-y} \sin x = - \frac{\delta v}{\delta x}
$$
(C-R is satisfied for every $(x,y)$ and partial derivatices are continuous)

* we can verify that

    $$
    \left.\begin{array}{ll}
    \frac{\partial u}{\partial x}=e^{-y} \cos x, & \frac{\partial^2 u}{\partial x^2}=-e^{-y} \sin x \\
    \frac{\partial u}{\partial y}=-e^{-y} \sin x, & \frac{\partial^2 u}{\partial y^2}=e^{-y} \sin x
    \end{array}\right\} \frac{\partial^2 u}{\partial x^2}+\frac{\partial^2 u}{\partial y^2}=0
    $$

* hence, $u(x,y) = e^{-y}\sin x$ is harmonic in every domain of the complex plane

## **Harmonic Conjugate**
$v$ is said to be a **harmonic conjugate** of $u$ if

1. $u$ and $v$ are harmonic in a domain $D$
2. their first-order partial derivatives satisfy the Cauchy-Riemann equations on $D$

**example:** $f(z) = z^2 = x^2-y^2 +j2xy$

* since $f$ is entire, then $u$ and $v$ are harmonic on the complex plane
* since $f$ is analytic, $u$ and $v$ satisfy the C-R equations
* therefore, $v$ is a harmonic conjugate of $u$

**Theorem:** $f(z) = u(x,y) + jv(x,y)$ is analytic in a domain $D$ *if and only if* $v$ is harmonic conjugate of $u$

**example:** $f = 2xy + j(x^2 - y^2)$

* $f$ is not analytic anywhere except $z=0$ because
$$
\frac{\delta u}{\delta x} = 2y \neq -2y = \frac{\delta v}{\delta y}, \quad \frac{\delta u}{\delta y} = 2x \neq -2x = -\frac{\delta v}{\delta x}
$$

* hence, $2xy$ cannot be a harmonic conjugate of $x^22 - y^2$ on any domain
# **Lecture 4: Analisis Variabel Tunggal**
## **4. Limits involving the point at infinity**

**Limit of polynomial functions:** for $ p(z) = a_0 + a_1z + ... + a_nz^n $ 
$$ \lim_{z\to z_0} p(z) = p(z_0) $$

**Theorem** suppose $ \lim_{z\to z_0} f(z) = w_0 $ then

\[
\lim_{{z \to z_0}} f(z) = \infty \quad \text{if and only if} \quad \lim_{{z \to z_0}} \frac{1}{f(z)} = 0 \\
\lim_{{z \to \infty}} f(z) = w_0 \quad \text{if and only if} \quad \lim_{{z \to 0}} f\left(\frac{1}{z}\right) = w_0 \\
\lim_{{z \to \infty}} f(z) = \infty \quad \text{if and only if} \quad \lim_{{z \to 0}} f\left(\frac{1}{\frac{1}{z}}\right) = 0
\]


**example:**

$$ \lim_{z\to \infty} \frac{2z+j}{z+1}=2 \quad \text{because} \quad  \lim_{z\to 0} \frac{(2/z)+j}{(1/z)+j}=\lim_{z\to 0} \frac{2+jz}{1+z} = 2 $$

$$ \lim_{z\to \infty} \frac{2z^3-1}{z^2+1}=\infty \quad \text{since} \quad  \lim_{z\to 0} \frac{(1/z^2)+1}{(2/z^3)-1}=\lim_{z\to 0} \frac{z+z^3}{2-z^3} = 0 $$

## **5. Continuity**

**Definition:** $f$ is said to be **continuous** at a point $z_0$ if

$$
\lim_{{z \to z_0}} f(z) = f(z_0)
$$
provided that both terms must exist<br>
this statement is equicalent to another definition:<br>
$\delta - \epsilon$ **Definition:** if for any $\epsilon > 0$, there exists $\delta > 0$ such that
$$ |f(z) - f(z_0)|<\epsilon \quad \text{whenever} \quad |z-z_0|<\delta $$
then $f$ is continuous at $z_0$

**example:** $f(z) = z/(z^2 + 1)$

* $f$ is not continuous at $\pm j$ because $f(\pm j)$ do not exist
* $f$ is not continuous at $1$ because
$$ f(1) = 1/2 \quad \text{and} \quad \lim_{z\to 1} \frac{z}{z^2+1}=1/2 $$
**example:** 
$
f(z) =
\begin{cases}
    \frac{z^2+j3z-2}{z+j}, & z \neq -j \\\\
    2j, & z = -j
\end{cases}
$
$$ \lim_{z\to -j} f(z) = \lim_{z\to -j} \frac{z^2+j3z-2}{z+j} = \lim_{z\to -j} \frac{(z+j)(z+j2)}{z+j} = \lim_{z\to -j} (z+j2) = j$$

we see that $ \lim_{z\to -j} f(z) \neq f(-j)=2j$ <br>
hence, $f$ is not continuous at $z = -j$

**Remarks**

* $f$ is said to be continuous in a region $R$ if it is continuous at each point in $R$
* if $f$ and $g$ are continuous at a point, then so is $f+g$
* if $f$ and $g$ are continuous at a point, then so is $fg$
* if $f$ and $g$ are continuous at a point, then so is $f/g$ at any such point if $g$ is not zero there
* if $f$ and $g$ are continuous at a point, then so is $f \circ g$
* if $f(z)=u(x,y) +jv(x,y)$ is continuous at $z_0 = (x_0,y_0)$ if and only if $u(x,y)$ and $v(x,y)$ are continuous at $(x_0,y_0)$

## **6. Derivatives**
the **complex derivative** of $f$ at $z$ is the limit
$$ \frac{df}{dz}=f'(z) = \lim_{\Delta z \to 0} \frac{f(z+\Delta z) - f(z)}{\Delta z} $$

(if the limit exist)<br>
$\Delta z$ is a complex variable<br>
so the limit must be the same no matter how $\Delta z$ approaches 0<br>
$f$ is said to be **differentiable** at $z$ when $f'(z)$ exist

**example:** find the derivative of $f(z) =z^3$

$$
\begin{align*}
    \lim_{\Delta z \to 0} \frac{f(z+\Delta z) - f(z)}{\Delta z} & = \lim_{\Delta z \to 0} \frac{(z+\Delta z)^3 - (z)^3}{\Delta z}\\\\
    & = \lim_{\Delta z \to 0} \frac{3z^2\Delta z+3z\Delta z^2+\Delta z^3}{\Delta z}\\\\
    & = \lim_{\Delta z \to 0} 3z^2 + 3z\Delta z + \Delta z^2 = 3z^2
\end{align*}
$$

hence, $f$ is differentiable at any point $z$ and $f'(z) = 3z^2$

<p style="text-align:center;"><b>Differentiation formulas</b></p> 
basic formulas still hold for complex-valued functions

* $\frac{dc}{dz}=0$ and $\frac{d}{dz}[cf'(z)]$ where $c$ is a constant
* $\frac{d}{dz}z^n = nz^{n-1}$ if $n \neq 0$ is an integer
* $\frac{d}{dz}[f(z)+g(z)] = f'(z)+g'(z)$
* $\frac{d}{dz}[f(z)g(z)] = f(z)g'(z) + f'(z)g(z)$ (product rule)
* let \(h(z)=g(f(z))\)
$$
h'(z) = g'(f(z))f'(z) \tag{chain rule} 
$$

## **7. Cauchy-Riemann equation**

* **Theorem:** suppose that
$$
f(z) = u(x,y) + jv(x,y)
$$

and $f'(z)$ exist at $z_0 = (x_0, y_0)$ then 

* the first-order derivatives of $u$ and $v$ must exist at (x_0, y_0)
* the derivatives must satisfy the **Cauchy-Riemann equations:**

$$
\frac{\delta u}{\delta x} = \frac{\delta v}{\delta y}, \frac{\delta u}{\delta y} = -\frac{\delta v}{\delta x}
$$
and $f'(z_0)$ can be written as

$$
f'(z_0) = \frac{\delta v}{\delta y} + j\frac{\delta v}{\delta x}
$$


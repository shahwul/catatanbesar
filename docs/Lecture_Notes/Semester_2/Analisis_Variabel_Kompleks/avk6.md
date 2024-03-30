# **Lecture 6: Analisis Variabel Kompleks**
## **Exponential Function**
from $z=x+j y$, an exponential function is defined as 

$$  
f(z)=e^{z}=e^{x} \cos y+j e^{x} \sin y  
$$  
  
**Properties**  

- $f(z)=e^{z}$ is analytic everywhere on $\mathbf{C}$  
$\left(e^{z}\right.$ is entire)  
- $f^{\prime}(z)=e^{z}$  
- $e^{z+w}=e^{z} e^{w}, \quad z, w \in \mathbf{C}$  
(addition formula)  
- $\left|e^{z}\right|=e^{x}$ and $\arg \left(e^{z}\right)=y+2 n \pi \quad(n=0, \pm 1, \pm 2, \ldots)$  
$\left(\right.$ so $\left.e^{z} \neq 0\right)$  
- if $z$ is pure imaginary, then $e^{z}$ is periodic

## **Logarithmic Function**

the definition of $\log$ function is based on solving  

$$  
e^{w}=z  
$$  

for $w$ where $z$ is any nonzero complex number, and we call $w=\log z$ write $z=r e^{j \Theta}(-\pi<\Theta \leq \pi)$ and $w=u+j v$, so we have 

$$  
e^{u}=r, \quad v=\Theta+2 n \pi  
$$  

thus the definition of the (multiple-valued) logarithmic function of $z$ is  

$$  
\log z=\log r+i(\Theta+2 n \pi), \quad(n=0, \pm 1, \pm 2, \ldots)  
$$  

if only the principle value of $\arg z$ is used $(n=0)$, then $\log z$ is single-valued

the principal value of $\log z$ is defined as

$$  
\log z=\log r+i \operatorname{Arg} z  
$$  

where $r=|z|$ and recall that $\operatorname{Arg} z$ is the principal argument of $z$  

- $\log z$ is single-valued  
- $\log z=\log z+j 2 n \pi, \quad(n=0, \pm 1, \pm 2, \ldots)$  
  
**note:** when $z$ is complex, one should not jump into the conclusion that  

$$  
\log \left(e^{z}\right)=z  
$$

(log is multiple-valued)  
instead, if $z=x+j y$, we should write

$$  
\begin{aligned}  
\log \left(e^{z}\right) & =\log \left|e^{z}\right|+j\left(\operatorname{Arg}\left(e^{z}\right)+2 n \pi\right)=\log \left|e^{x}\right|+j(y+2 n \pi) \\  
& =z+j 2 n \pi \quad(n=0, \pm 1, \pm 2, \ldots)  
\end{aligned}  
$$

**example:** find $\log z$ for $z=-1+j, z=1$, and $z=-1$  

- if $z=-1+j$ then $r=\sqrt{2}$ and $\operatorname{Arg} z=3 \pi / 4$ 
  
$$  
\begin{aligned}  
\log z & =\log \sqrt{2}+j(3 \pi / 4+2 n \pi), \quad(n=0, \pm 1, \pm 2, \ldots) \\  
\log z & =\log \sqrt{2}+j 3 \pi / 4  
\end{aligned}  
$$  

- if $z=1$ then $r=1$ and $\operatorname{Arg} z=0$ 
  
$$  
\begin{align*}  
\log z & =0+j 2 n \pi=j 2 n \pi, \quad(n=0, \pm 1, \pm 2, \ldots) \\  
\log z & =0 \quad \text { (as expected) }  
\end{align*}  
$$  

- if $z=-1$ then $r=1$ and $\operatorname{Arg} z=\pi$  

$$  
\log z=\log 1+j(\pi+2 n \pi)=j(2 n+1) \pi, \quad(n=0, \pm 1, \pm 2, \ldots)  
$$  

$\log z=j \pi=j \quad$ (now we can find $\log$ of a negative number)

## **Complex Component**

let $z \neq 0$ and $c$ be any complex number, the function $z^{c}$ is defined via

$$  
z^{c}=e^{c \log z}  
$$  

where $\log z$ is the multiple-valued logarithmic function  
let $\Theta$ be the principal value of $\arg z$ and let $c=a+j b$  

$$  
z^{c}=e^{c \log z}=e^{(a+j b)(\log |z|+j(\Theta+2 n \pi))}, \quad(n=0, \pm 1, \pm 2, \ldots)  
$$  

**example:** find $j^{j}$  

$$  
j^{j}=e^{j(\log j)}=e^{j(\log 1+j(\pi / 2+2 n \pi))}=e^{-(1 / 2+2 n) \pi}, \quad(n=0, \pm 1, \pm 2, \ldots)  
$$  

(complex power of a complex can become real numbers)  

**more example:** the values of $j^{-j}$ are given by  

$$  
j^{-j}=e^{-j(\log j)}=e^{-j(\log 1+j(\pi / 2+2 m \pi))}=e^{(1 / 2+2 m) \pi}, \quad(m=0, \pm 1, \pm 2, \ldots)  
$$  

if we multiply the values of $j^{j}$ by those of $j^{-j}$ we obtain infinitely many values of  

$$  
e^{2 k \pi}, \quad-\infty<k<\infty  
$$  

thus, the usual algebraic rules do not apply to $z^{c}$ when they are multi-valued !  

$$  
\left(j^{j}\right) \cdot\left(j^{-j}\right) \neq j^{0}=1  
$$

## **Trigonometric Function**
by using Euler's formula  
$e^{j x}=\cos x+j \sin x, \quad$ for any real number $x$  
we can write  

$$  
\sin x=\frac{e^{j x}-e^{-j x}}{2 j}, \quad \cos x=\frac{e^{j x}+e^{-j x}}{2}  
$$  

hence, it is natural to define trigonometric functions of a complex number $z$ as  

$$  
\begin{array}{l}  
\sin z=\frac{e^{j z}-e^{-j z}}{2 j}, \quad \cos z=\frac{e^{j z}+e^{-j z}}{2}, \tan z=\frac{\sin z}{\cos z} \\  
\csc z=\frac{1}{\sin z}, \quad \sec z=\frac{1}{\cos z}, \quad \cot z=\frac{1}{\tan z} \\  
\end{array}  
$$  
 
(use $\frac{d}{d z} e^{j z}=j e^{j z}$ )  
(sine is odd and cosine is even)  
**Properties**

- $\sin z$ and $\cos z$ are entire functions (since $e^{j z}$ and $e^{-j z}$ are entire)  
- $\frac{d}{d z} \sin z=\cos z$ and $\frac{d}{d z} \cos z=-\sin z$  

**Properties**  

- $\sin z$ and $\cos z$ are entire functions (since $e^{j z}$ and $e^{-j z}$ are entire)  
- $\frac{d}{d z} \sin z=\cos z$ and $\frac{d}{d z} \cos z=-\sin z$ - $\sin (-z)=-\sin z$ and $\cos (-z)=\cos z$ - $\sin (z+2 \pi)=\sin z$ and $\sin (z+\pi)=-\sin z$  
- $\cos (z+2 \pi)=\cos z$ and $\cos (z+\pi)=-\cos z$  
- $\sin (z+\pi / 2)=\cos z$ and $\sin (z-\pi / 2)=-\cos z$  
- $\sin (z+w)=\sin z \cos w+\cos z \sin w$  
- $\cos (z+w)=\cos z \cos w-\sin z \sin w$

## **Hyperbolic Function**
the hyperbolic sine, cosine, and tangent of a complex number are defined as  

$$  
\sinh z=\frac{e^{z}-e^{-z}}{2}, \quad \cosh z=\frac{e^{z}+e^{-z}}{2}, \quad \tanh z=\frac{\sinh z}{\cosh z}  
$$  

(as they are with a real variable)  
**Properties**

- $\sinh z$ and $\cosh z$ are entire  
(since $e^{z}$ and $e^{-z}$ are entire)  
- $\tanh z$ is analytic in every domain in which $\cosh z \neq 0$  
- $\frac{d}{d z} \sinh z=\cosh z$ and $\frac{d}{d z} \cosh z=\sinh z$  
- $\frac{d}{d z} \tanh z=\operatorname{sech}^{2} z$  
 
## **Branches for multi-valued functions**
we often need to investigate the differentiability of a function $f$  

$$  
f^{\prime}(z)=\lim _{\Delta z \rightarrow 0} \frac{f(z+\Delta z)-f(z)}{\Delta z}  
$$ 

what happen if $f$ is multiple-valued (like $\arg z, z^{c}$ )?  

- have to make sure if the two funtion values tend to the same value in the limit  
- have to choose one of the function values in a consistent way  

restricting the values of a multiple-valued functions to make it single-valued in some region is called choosing a branch of the function  
a branch of $f$ is any single-valued function $F$ that is analytic in some domain

we define the principal branch $\log$ of the lograrithmic function as  

$$  
\log z=\log |z|+j \operatorname{Arg}(z), \quad-\pi<\operatorname{Arg}(z)<\pi  
$$  

where $\operatorname{Arg}(z)$ is the principle value of $\arg (z)$  

- $\log z$ is single-valued  
- $\log z$ is not continuous along the negative real axis (because of $\operatorname{Arg} z$ ) 
  
$$  
\begin{array}{l}  
z=-x+j \epsilon \Longrightarrow \operatorname{Arg} z \rightarrow \pi \quad \text { as } \epsilon \rightarrow 0 \\  
z=-x-j \epsilon \Longrightarrow \operatorname{Arg} z \rightarrow-\pi \quad \text { as } \epsilon \rightarrow 0  
\end{array}  
$$  

a branch cut is portion of curve that is introduced to define a branch $F$ 

- points on the branch cut for $f$ are singular points  
- the negative real axis is a branch cut for the Log function  
- $\log z$ is single-valued and continuous in $D=\mathbf{C} \backslash(-\infty, 0]$ $D=\mathrm{C} \backslash(-\infty, 0]$ 
   
let $z_{0}$ be any point in $D$ and $w_{0}=\log z_{0}$ (or $z_{0}=e^{w_{0}}$ )  

$$  
\begin{aligned}  
\frac{d}{d z} \log z_{0} & =\lim _{z \rightarrow z_{0}} \frac{w-w_{0}}{z-z_{0}}=\lim _{z \rightarrow z_{0}} \frac{1}{\frac{g-z_{0}}{w-w_{0}}}=\lim _{w \rightarrow w_{0}} \frac{1}{\frac{z-z_{0}}{w-w_{0}}} \\  
& =\lim _{w \rightarrow w_{0}} \frac{1}{\frac{e^{w}-e^{w_{0}}}{w-w_{0}}}=\frac{1}{\left.\frac{d}{d z} e^{w}\right|_{w=w_{0}}}=\frac{1}{e^{w_{0}}}=\frac{1}{z_{0}}  
\end{aligned}  
$$  

(we have used single-valuedness and continuity of the Log function)  
$\log z$ is analytic in $D$

other branches of $\log z$

$$  
\begin{array}{l}  
\log (z)=\log |z|+j \arg (z), \quad 0<\arg (z)<2 \pi \\  
\log (z)=\log |z|+j \arg _{\tau}(z), \quad \tau<\arg _{\tau}(z)<\tau+2 \pi  
\end{array}  
$$  

a branch $\log (z)$ is analytic everywhere on $D_{\tau}$  
any point that is common to all branch cuts of $f$ is called a branch point the origin is a branch point of the $\log$ function  
 
**example:** suppose we have to compute the derivative of  

$$  
f(z)=\log \left(z^{2}-1\right) \text { at point } z=j  
$$  

choose a branch of $f$ which is analytic in a region containing the point  

$$  
j^{2}-1=-2  
$$  

the principal branch is not analytic there, so we choose another branch  
e.g., choose $\log (z)=\log |z|+j \arg (z), 0<\arg z<2 \pi$; then by chain rule,  

$$  
f^{\prime}(j)=\left.\frac{2 z}{z^{2}-1}\right|_{z=j}=\frac{2 j}{j^{2}-1}=-j  
$$

define the principal branch of $z^{c}$ to be  

$$  
e^{c \log z}  
$$  

where $\log z$ is the principal branch of $\log z$  

- since the exponential function is entire, the principal branch of $z^{c}$ is analytic in $D$ where $\log z$ is analytic  
- using the chain rule  
  
$$  
\left.\frac{d}{d z}\left(e^{c \log z}\right)\right|_{z=z_{0}}=e^{c \log z_{0}} \frac{c}{z_{0}}=\frac{c z_{0}^{c}}{z_{0}}=c z_{0}^{c-1}  
$$  

provided that we use the same branch of $z^{c}$ on both sides of the equation $\left(z^{a} z^{b}=z^{a+b}\right.$ iff we use the same branch for the complex power on both sides)

## **Derivatives of Functions**

consider derivatives of complex-valued functions $w$ of a real variable $t$  

$$  
w(t)=u(t)+j v(t)  
$$  

where $u$ and $v$ are real-valued functions of $t$ the derivative $w^{\prime}(t)$ or $\frac{d}{d t} w(t)$ is defined as  

$$  
w^{\prime}(t)=u^{\prime}(t)+j v^{\prime}(t)  
$$  
  
Properties many rules are carried over to complex-valued functions  

- $[c w(t)]^{\prime}=c w^{\prime}(t)$  
- $[w(t)+s(t)]^{\prime}=w^{\prime}(t)+s^{\prime}(t)$  
- $[w(t) s(t)]^{\prime}=w^{\prime}(t) s(t)+w(t) s^{\prime}(t)$  

mean-value theorem: no longer applies for complex-valued functions  
suppose $w(t)$ is continuous on $[a, b]$ and $w^{\prime}(t)$ exists  
it is not necessarily true that there is a number $c \in[a, b]$ such that  

$$  
w^{\prime}(c)=\frac{w(b)-w(a)}{b-a}  
$$  

for example, $w(t)=e^{j t}$ on the interval $[0,2 \pi]$ and we have $w(2 \pi)-w(0)=0$  
however, $\left|w^{\prime}(t)\right|=\left|j e^{j t}\right|=1$, which is never zero

mean-value theorem: no longer applies for complex-valued functions  
suppose $w(t)$ is continuous on $[a, b]$ and $w^{\prime}(t)$ exists  
it is not necessarily true that there is a number $c \in[a, b]$ such that 

$$  
w^{\prime}(c)=\frac{w(b)-w(a)}{b-a}  
$$  

for example, $w(t)=e^{j t}$ on the interval $[0,2 \pi]$ and we have $w(2 \pi)-w(0)=0$  
however, $\left|w^{\prime}(t)\right|=\left|j e^{j t}\right|=1$, which is never zero  

## **Definite Integrals of Function**  
 
the definite integral of a complex-valued function 

$$  
w(t)=u(t)+j v(t)  
$$  

over an interval $a \leq t \leq b$ is defined as  

$$  
\int_{a}^{b} w(t) d t=\int_{a}^{b} u(t) d t+j \int_{a}^{b} v(t) d t  
$$  

provided that each integral exists (ensured if $u$ and $v$ are piecewise continuous)  
Properties

- $\int_{a}^{b}[c w(t)+s(t)] d t=c \int_{a}^{b} w(t) d t+\int_{a}^{b} s(t) d t$  
- $\int_{a}^{b} w(t) d t=-\int_{b}^{a} w(t) d t$  
- $\int_{a}^{b} w(t) d t=\int_{a}^{c} w(t) d t+\int_{c}^{b} w(t) d t$

**Fundamental Theorem of Calculus:** still holds for complex-valued functions  
suppose  

$$  
W(t)=U(t)+j V(t) \quad \text { and } \quad w(t)=u(t)+j v(t)  
$$  

are continuous on $[a, b]$  
if $W^{\prime}(t)=w(t)$ when $a \leq t \leq b$ then $U^{\prime}(t)=u(t)$ and $V^{\prime}(t)=v(t)$  
then the integral becomes  

$$  
\int_{a}^{b} w(t) d t=\left.U(t)\right|_{a} ^{b}+\left.j V(t)\right|_{a} ^{b}=[U(b)+j V(b)]-[U(a)+j V(a)]  
$$  

therefore, we obtain 
 
$$  
\int_{a}^{b} w(t) d t=W(b)-W(a)  
$$  

**example:** compute $\int_{0}^{\pi / 6} e^{j 2 t} d t$  
since  

$$  
\frac{d}{d t}\left(\frac{e^{j 2 t}}{j 2}\right)=e^{j 2 t}  
$$  

the integral is given by 
 
$$  
\begin{aligned}  
\int_{0}^{\pi / 6} e^{j 2 t} d t & =\left.\frac{1}{j 2} e^{j 2 t}\right|_{0} ^{\pi / 6} \\  
& =\frac{1}{j 2}\left[e^{j \pi / 3}-e^{j 0}\right] \\  
& =\frac{\sqrt{3}}{4}+\frac{j}{4}  
\end{aligned}  
$$

mean-value theorem for integration: not hold for complex-valued $w(t)$  
it is not necessarily true that there exists $c \in[a, b]$ such that  

$$  
\int_{a}^{b} w(t) d t=w(c)(b-a)  
$$  

for example, $w(t)=e^{j t}$ for $0 \leq t \leq 2 \pi$  
it is easy to see that  

$$  
\int_{a}^{b} w(t) d t=\int_{0}^{2 \pi} e^{j t} d t=\left.\frac{e^{j t}}{j}\right|_{0} ^{2 \pi}=0  
$$  

but there is no $c \in[0,2 \pi]$ such that $w(c)=0$

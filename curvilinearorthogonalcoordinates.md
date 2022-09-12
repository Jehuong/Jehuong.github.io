<script type="text/x-mathjax-config">
    MathJax.Hub.Config({
      tex2jax: {
        skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
        inlineMath: [['$','$']]
      }
    });
  </script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script> 

A small increment of an arbitrary vector can be interpreted as 

$$
\mathrm{d} \mathbf{r}  = \frac{\partial \mathbf{r} }{\partial u}  \mathrm{d} u
+ \frac{\partial \mathbf{r} }{\partial v }  \mathrm{d} v
+ \frac{\partial \mathbf{r} }{\partial w }  \mathrm{d} w
$$

with the rule of differential. The partial differential that as the coefficient of small increase in each parameter is identified as with the direction of base vector. For example, 

$$
\frac{\partial \mathbf{r} }{\partial u} = h _{u} \mathbf{e} _{u} 
$$

Where h is introduced in order to insure the magnitude of base vector equal to one. 
We can use this method to find the basis of certain orthogonal curvilinear coordinates. For instance, consider the spherical coordinate,

$$
\begin{aligned}
x & = r \cos \varphi \sin \theta \\
y & = r \sin \varphi \sin \theta \\
z & = r \cos \theta 
\end{aligned}
$$

A vector in the standard coordinate system is

$$
\mathbf{r}  = x \mathbf{e} _{x} + y \mathbf{e} _{y} + z \mathbf{e} _{z} 
$$

Substitute expression for x, y and z

$$
\mathbf{r}  = r \cos \varphi \sin \theta \mathbf{e} _{x} + r \sin \varphi \sin \theta \mathbf{e} _{y} + r \cos \theta \mathbf{e} _{z} 
$$

Take differential of r

$$
\begin{aligned}
\mathrm{d} \mathbf{r} = & \left ( \cos \varphi \sin \theta \mathbf{e} _{x} 
+ \sin \varphi \sin \theta \mathbf{e} _{y} + \cos \theta \mathbf{e} _{z}  \right ) \mathrm{d} r \\
+ & \left ( -r \sin \varphi \sin \theta \mathbf{e} _{x} 
+ r \cos \varphi \sin \theta \mathbf{e} _{y}  \right ) \mathrm{d} \varphi \\
+ & \left ( r \cos \varphi \cos \theta \mathbf{e} _{x} 
+ r \sin \varphi \cos \theta \mathbf{e} _{y} - r \sin \theta \mathbf{e} _{z}  \right ) \mathrm{d} \theta
\end{aligned}
$$

From above

$$
\begin{aligned}
\mathbf{e} _{r} & = \cos \varphi \sin \theta \mathbf{e} _{x} 
+ \sin \varphi \sin \theta \mathbf{e} _{y} + \cos \theta \mathbf{e} _{z} \\
\mathbf{e} _{\varphi } & = - \sin \varphi \mathbf{e} _{x} + \cos \varphi \mathbf{e} _{y} \\
\mathbf{e} _{\theta } & = \cos \varphi \cos \theta \mathbf{e} _{x} 
+ \sin \varphi \cos \theta \mathbf{e} _{y} - \sin \theta \mathbf{e} _{z} 
 \end{aligned}
 
$$

and 

$$
h _{r} = 1 \quad h _{ \varphi } = r \sin \theta \quad h _{ \theta } = r
$$

$$
 \mathrm{d} \mathbf{r} = \mathbf{e} _{r} \mathrm{d} r 
+ r \sin \theta \mathbf{e} _{ \varphi } \mathrm{d} \varphi 
+ r \mathbf{e} _{ \theta } \mathrm{d} \theta
$$

Application to differentiations: If one want to find the gradient of some function under spherical coordinates, notice that 

$$

\begin{aligned}
\mathrm{d}f & = \nabla f \cdot \mathrm{d} \mathbf{r} \\
\frac{\partial f }{\partial u}  \mathrm{d} u
+ \frac{\partial f }{\partial v }  \mathrm{d} v
+ \frac{\partial f }{\partial w }  \mathrm{d} w & = \nabla f 
\cdot \left ( h _{u} \mathbf{e} _{u} \mathrm{d} u
+ h _{v} \mathbf{e} _{v} \mathrm{d} v
+ h _{w} \mathbf{e} _{w} \mathrm{d} w \right ) 
\end{aligned}

$$

Using orthonormality and compare two sides of the equation, 

$$
\nabla f = \frac{1}{h _{u} } \frac{\partial f }{\partial u } \mathbf{e} _{u} +
\frac{1}{h _{v} } \frac{\partial f }{\partial v } \mathbf{e} _{v} +
\frac{1}{h _{w} } \frac{\partial f }{\partial w } \mathbf{e} _{w}
$$

In the spherical coodinate it is

$$
\nabla f = \frac{\partial f }{\partial r } \mathbf{e} _{r} +
\frac{1}{r \sin \theta } \frac{\partial f }{\partial \varphi } \mathbf{e} _{ \varphi } +
\frac{1}{r } \frac{\partial f }{\partial \theta } \mathbf{e} _{ \theta }
$$
<script type="text/x-mathjax-config">
    MathJax.Hub.Config({
      tex2jax: {
        skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
        inlineMath: [['$','$']]
      }
    });
  </script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script> 
  






## Chapter: Central Force Problem

### Introduction
Firstly, consider an ith multiple bodies system. The kinetic energy of the system is

$$
T = \frac{1}{2} \sum_{i}^{} m_{i} \dot{ \mathbf{R} } _{i} ^{2} 
$$

Using R with subscript i to indicate the position vector of each particle. Define the center of mass vector as 

$$
\mathbf{R} = \frac{ \sum m_{i} \mathbf{R} _{i} }{\sum m_{i} } = \frac{ \sum m_{i} \mathbf{R} _{i} }{M } 
$$

Then the position vector of each particle is 

$$
\mathbf{R} _i = \mathbf{R} + \mathbf{r} _{i}
$$

where r with subscript i is therby the vector from center of mass to each of particle. Writing r explicitly,

$$
\begin{aligned}
\mathbf{r} _{i} & = \mathbf{R} _{i} - \mathbf{R} \\ 
& = \mathbf{R} _{i} - \frac{ \sum_{j} m_{j} \mathbf{R} _{j} }{\sum_{j} m_{j} } \\
& = \frac{1}{M} \left ( \sum_{j} m_{j} \mathbf{R} _{i} - \sum_{j} m_{j} \mathbf{R} _{j}  \right ) \\
& = \frac{1}{M} \sum_{j} m_{j} (\mathbf{R} _{i} - \mathbf{R} _{j} )
\end{aligned}
$$

This form enabled us to see the constraint involved by the introduction of center of mass, 

$$
\begin{aligned}
\sum m_{i} \mathbf{r} _{i} & = \frac{1}{M} \sum_{i} m_{i} \sum_{j} m_{j} (\mathbf{R} _{i} - \mathbf{R} _{j} ) \\ 
& = \frac{1}{M} \sum_{i, j} m_{i} m_{j} ( \mathbf{R} _{i} - \mathbf{R} _{j} ) = 0
\end{aligned}
$$

Therefore, by substituting r and center of mass vector for each particle's position vector (the one from origin ). Then applying the constraint above gives new expression for kinetic energy, 

$$
T = \frac{1}{2} \sum_{i}^{} m_{i} ( \dot{\mathbf{R} } + \dot{\mathbf{r} } _{i} ) ^{2} 
= \frac{1}{2} M \dot{\mathbf{R} } ^{2} + \frac{1}{2} \sum_{i} m_{i} \dot{\mathbf{r} } _{i} ^{2}
$$

### Two body Problem
More specifically, consider the two-body system, the potential of the system is only depended on the relative distance vector of the two objects and its higher deriatives.

![image](twobodysystem.png#pic_right)

The Lagrangian of this system should be 

$$
L=\frac{1}{2} m_{1} \dot{\mathbf{R} } _{1} ^{2} +  \frac{1}{2} m_{2} \dot{\mathbf{R} } _{2} ^{2} -V(\mathbf{r} , \dot{\mathbf{r} } , ... )
$$

Trying to transform it in to center of mass frame: The vector from origin to the center of mass by definition is

$$
\mathbf{R} =\frac{m_{1} \mathbf{R} _{1} +m_{2} \mathbf{R} _{2} }{m_{1} +m_{2} } 
$$

Thus,

$$
\begin{aligned}
\mathbf{r} _{1} & = \mathbf{R} _{1} -\mathbf{R} \\ & = \frac{\left ( m_{1} +m_{2}  \right ) \mathbf{R} _{1} -m_{1} \mathbf{R} _{1} -m_{2} \mathbf{R} _{2} }{m_{1} +m_{2} } \\
& = \frac{m_{2} }{m_{1} +m_{2} } \left ( \mathbf{R} _{1} -\mathbf{R} _{2}  \right ) \\
& = - \frac{m_{2} }{m_{1} +m_{2} } \mathbf{r} \\
\mathbf{r} _{2} & = \frac{m_{1} }{m_{1} +m_{2} } \mathbf{r} 
\end{aligned}
$$

Substitute these expressions into the Lagrangian. Examine kinetic energy term first,

$$
\begin{aligned}
T & = \frac{1}{2} m_{1} \left( \dot{\mathbf{R} } + \dot{\mathbf{r} }_{1} \right)^{2} +\frac{1}{2} m_{2} \left( \dot{\mathbf{R} }+\dot{\mathbf{r} }_{2} \right)^{2} \\
&=\frac{1}{2}\left(m_{1} +m_{2} \right) \dot{\mathbf{R} }^{2}+\underbrace{ m_{1} \dot{\mathbf{R} } \cdot \dot{\mathbf{r} } _{1} +m_{2} \dot{\mathbf{R} } \cdot \dot{\mathbf{r} }_{2} }_{=0}+\frac{1}{2} m_{1} \dot{\mathbf{r} }_{1}^{2}+\frac{1}{2} m_{2} \dot{\mathbf{r} }_{2} ^{2} \\
&=\frac{1}{2} \left(m_{1} + m_{2} \right) \dot{\mathbf{R} }^{2} + \frac{1}{2} \left[m_{1}\left( \frac{m_{2} }{m_{1} +m_{2} }\right)^{2} +m_{2}\left(\frac{m_{1} }{m_{1} + m_{2} } \right) ^{2} \right] \dot{\mathbf{r} } ^{2} \\
&=\frac{1}{2} \left( m_{1} + m_{2} \right) \dot{\mathbf{R} }^{2}+\frac{1}{2} \frac{ m_{1} m_{2} }{ m_{1} + m_{2} } \dot{\mathbf{r} } ^{2}
\end{aligned}
$$

Second and third term in the second line are canceled out because the constraint of the center of mass applied. In the last expression of kinetic energy, the first term is constant, since there is no external force acting on COM. We can drop that term in the Lagrangian:

$$
L = \frac{1}{2} \frac{m_{1} m_{2}}{m_{1}+m_{2}} \dot{\mathbf{r} }^{2} - V(\mathbf{r} , \dot{\mathbf{r} } , ... )
$$

The coefficient of $ \mathbf{r}^{2}  $ is known as the reduced mass. Therefore, a two body central force problem can always reduced to a one body problem.

### Two ways to determine the energy of a circular orbit

1.In circular orbits, kinetic energy and potential energy are constants. Therefore, by *Virial Theorem*,

$$
T = - \frac{1}{2} V
$$

The total energy E is

$$
E = T + V = - \frac{1}{2} V + V = \frac{1}{2} V 
$$

for V takes the form 

$$
V = - \frac{k}{r} 
$$

to eliminate r in the expression, note that in the circular orbit, there is equilibrium between the central force and the centrifugal force. Another method to find this equation is to notice the explicit expression of E, (The $ l $ here stands for angular momentum.)

$$
E = \frac{1}{2} m \dot{r} ^{2} + \frac{1}{2} \frac{l ^{2} }{m r^{2} } - \frac{k}{r}
$$

for circular motion $ \dot{r} $ equals to zero. (this technique is also useful in finding semimajor axis length in general elliptic orbits, at apsidal distances $ \dot{r} $ equals to zero) The lefted terms hence must reached the extreme in their expression for $ r $ . In other words, the effective potential reaches minimum. Its value is thus also the minimum of the whole system can reach. 

$$
\frac{l^{2} }{m r_{0} ^{3} } - \frac{k}{r_{0} ^{2} } = 0
$$ 

After solving $ r_{0} $


$$
E = - \frac{m k ^{2} }{2 l^{2} } 
$$

2.Eccentricity of orbit is given by

$$
e = \sqrt{1 + \frac{2E l ^{2} }{m k^{2} } } 
$$

$ e = 1 $ in circular orbit. Solving for E recover the same expression.
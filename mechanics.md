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

At the beginning, consider the two-body system.

![image](twobodysystem.png#pic_right)

The Lagrangian of this system should be 

$$
L=\frac{1}{2} m_{1} \mathbf{R} _{1} ^{2} +  \frac{1}{2} m_{2} \mathbf{R} _{2} ^{2} -V(\mathbf{r} , \dot{\mathbf{r} } , ... )
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
T & = \frac{1}{2} m_{1} \left( \mathbf{R} + \mathbf{r}_{1} \right)^{2} +\frac{1}{2} m_{2} \left( \mathbf{R}+\mathbf{r}_{2} \right)^{2} \\
&=\frac{1}{2}\left(m_{1} +m_{2} \right) \mathbf{R}^{2}+\underbrace{ m_{1} \mathbf{R} \cdot \mathbf{r}_{1}+m_{2} \mathbf{R} \cdot \mathbf{r}_{2} }_{=0}+\frac{1}{2} m_{1} \mathbf{r}_{1}^{2}+\frac{1}{2} m_{2} \mathbf{r}_{2} ^{2} \\
&=\frac{1}{2} \left(m_{1} + m_{2} \right) \mathbf{R}^{2} + \frac{1}{2} \left[m_{1}\left( \frac{m_{2} }{m_{1} +m_{2} }\right)^{2} +m_{2}\left(\frac{m_{1} }{m_{1} + m_{2} } \right) ^{2} \right] \mathbf{r} ^{2} \\
&=\frac{1}{2} \left( m_{1} + m_{2} \right) \mathbf{R}^{2}+\frac{1}{2} \frac{ m_{1} m_{2} }{ m_{1} + m_{2} } \mathbf{r} ^{2}
\end{aligned}
$$

Second and third term in the second line are opposite, hence they vanished. In the last expression of kinetic energy, the first term is constant, since there is no external force acting on COM. We can drop that term in the Lagrangian:

$$
L = \frac{1}{2} \frac{m_{1} m_{2}}{m_{1}+m_{2}} \mathbf{r}^{2} - V(\mathbf{r} , \dot{\mathbf{r} } , ... )
$$

The coefficient of $ \mathbf{r}^{2}  $ is known as the reduced mass. Therefore, a two body central force problem can always reduced to a one body problem.
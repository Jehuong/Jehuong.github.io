<script type="text/x-mathjax-config">
    MathJax.Hub.Config({
      tex2jax: {
        skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
        inlineMath: [['$','$']]
      }
    });
  </script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script> 



From ellipse equation in Cartesian coordinates, with its center set at the origin,

$$
\frac {x ^{2} } {a ^{2} } + \frac {y ^{2} } {b ^{2} } =1
$$

Instead set center at the origin, do a shift with direction at x-axis to the right, but leaving its magnitude unknown,

$$
\frac {\left ( x - \lambda \right ) ^{2} } {a ^{2} } + \frac {y ^{2} } {b ^{2} } = 1 
$$

do some algabraic manipulation,

$$
\begin{aligned}
\frac{b ^{2} } {a ^{2} } \left ( x ^{2} - 2 \lambda x + \lambda ^{2}  \right ) + y ^{2} & = b ^{2} \\
\left ( \frac{b ^{2} } {a ^{2} } -1  \right ) x ^{2} + \left ( x ^{2} + y ^{2} \right ) & = b ^{2} + 2 \lambda \frac{b ^{2} } {a ^{2} } x 
- \frac{b ^{2} \lambda ^{2} } {a ^{2} } \\
r ^{2} & = \left ( 1 - \frac{b ^{2} } {a ^{2} } \right ) x ^{2} + 2 \lambda \frac{b ^{2} } {a ^{2} } x 
+ b ^{2} - \frac{b ^{2} \lambda ^{2} } {a ^{2} } \\
& = \left ( \sqrt{1 - \frac{b ^{2} } {a ^{2} } } x - \sqrt{b ^{2} - \frac{b ^{2} \lambda ^{2} } {a ^{2} } }  \right ) ^{2}

\end{aligned}
$$

where the last two lines imply

$$
\sqrt{1 - \frac{b ^{2} } {a ^{2} } } \sqrt{b ^{2} - \frac{b ^{2} \lambda ^{2} } {a ^{2} } } = \lambda \frac{b ^{2} } {a ^{2} } 
$$

solving for lambda to get 

$$
\lambda ^{2} = a ^{2} \left ( 1 - \frac{b ^{2} } {a ^{2} } \right ) = a ^{2} - b ^{2}
$$

Then we define the eccentricity,

$$
e = \sqrt{1 - \frac{b ^{2} } {a ^{2} } }
$$

The expression of r follows

$$
r = ex+ \frac{ b ^{2} }{a} = er \cos \theta + \frac{ b ^{2} }{a} 
$$

Now express b using eccentrcity, this leaves

$$
r \left ( 1 - e \cos \theta \right ) = a \left ( 1 - e ^{2} \right )
$$
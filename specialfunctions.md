<script type="text/x-mathjax-config">
    MathJax.Hub.Config({
      tex2jax: {
        skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
        inlineMath: [['$','$']]
      }
    });
  </script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML"></script> 
  


# Special Functions
## Bessel Function
### **Integral representation**

$$
J_{n}(x)=\frac{1}{\pi} \int_{0}^{\pi} \cos (n \tau-x \sin \tau) \mathrm{d} \tau
$$


### **Application**: Kepler Equation

$$M=\Psi -e\sin \Psi $$

The goal is to solve $ {\Psi} $ from $ {M} $, that is, find a relation $\Psi  = f(M)$. Trying to do Fourier expansion about $ e\sin \Psi $ :

$$
e\sin \Psi =\sum b_{n} \sin (nM)
$$

Determine $ b_{n} $ :

<!--$$
 \begin{align}
{b_n} =&\frac{2}{\pi }\int_0^\pi  {(e\sin \Psi )(\sin nM)\mathrm{d}M =  - \frac{2}{{\pi n}}\int_0^\pi  {e\sin \Psi \mathrm{d}\cos nM} } 
 \\
 =&- \frac{2}{{\pi n}}\left( {\underbrace {\left. {e\sin \Psi \cos nM} \right|_0^\pi }_{ = 0} - \int_0^\pi  {\cos nM{\text{d}}e\sin \Psi } } \right)\underline{\underline {{\text{Kepler Equation}}}} \frac{2}{{\pi n}}\int_0^\pi  {\cos nM{\text{d(}}\Psi {\text{ - M)}}} 
 \\
  =& \frac{2}{{\pi n}}\left( {\int_0^\pi  {\cos nM{\text{d}}\Psi }  - \underbrace {\int_0^\pi  {\cos nM{\text{d}}M} }_{ = 0}} \right) = \frac{2}{n}\left( {\frac{1}{\pi }\int_0^\pi  {\cos (n\Psi  - en\sin \Psi ){\text{d}}\Psi } } \right)
  \\
   =& \frac{2}{n}{J_n}(en)

\end{align}
$$ -->




$$
\begin{aligned}
b_{n} &=\frac{2}{\pi} \int_{0}^{\pi}(e \sin \Psi)(\sin n M) \mathrm{d} M=-\frac{2}{\pi n} \int_{0}^{\pi} e \sin \Psi \mathrm{d} \cos n M \\
&=-\frac{2}{\pi n}(\underbrace{\left.e \sin \Psi \cos n M\right|_{0} ^{\pi}}_{=0}-\int_{0}^{\pi} \cos n M \mathrm{~d} e \sin \Psi) \underline{\underline{\text { Kepler Equation }} } \frac{2}{\pi n} \int_{0}^{\pi} \cos n M \mathrm{~d}(\Psi-\mathrm{M}) \\
&=\frac{2}{\pi n}(\int_{0}^{\pi} \cos n M \mathrm{~d} \Psi-\underbrace{\int_{0}^{\pi} \cos n M \mathrm{~d} M}_{=0})=\frac{2}{n}\left(\frac{1}{\pi} \int_{0}^{\pi} \cos (n \Psi-e n \sin \Psi) \mathrm{d} \Psi\right) \\
&=\frac{2}{n} J_{n}(e n)
\end{aligned}
$$

The first term in the second line vanishes by the assumption of the fourier expansion of $e\sin \Psi $. The second equality in the third line uses Kepler Equation again. Thus, the solution of Kepler equation is
<!--$$
\Psi  = M + \sum {\frac{2}{n}{J_n}(en)} \sin (nM)
$$-->

$$
\Psi=M+\sum \frac{2}{n} J_{n}(e n) \sin (n M)
$$
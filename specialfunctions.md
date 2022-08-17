# Special Functions
## Bessel Function
### Integral representation
$$
J_{n}(x)= \frac{1}{\pi} \int_{0}^{\pi} \cos (n\tau -x \sin \tau) \mathrm{d}\tau
$$
### Application: Kepler Equation
$$
M = \Psi  - e\sin \Psi 
$$
The goal is to solve $ \Psi $ from $ M $, that is, find a relation $\Psi  = f(M)$. Trying to do Fourier expansion about $e\sin \Psi $ :
$$
e\sin \Psi  = \sum\limits_{}^{} { {b_n}\sin (nM)} 
$$
Determine $ b_n $ :

$$
 \begin{align}
{b_n} =&\frac{2}{\pi }\int_0^\pi  {(e\sin \Psi )(\sin nM)\mathrm{d}M =  - \frac{2}{{\pi n}}\int_0^\pi  {e\sin \Psi \mathrm{d}\cos nM} } 
 \\
 =&- \frac{2}{{\pi n}}\left( {\underbrace {\left. {e\sin \Psi \cos nM} \right|_0^\pi }_{ = 0} - \int_0^\pi  {\cos nM{\text{d}}e\sin \Psi } } \right)\underline{\underline {{\text{Kepler Equation}}}} \frac{2}{{\pi n}}\int_0^\pi  {\cos nM{\text{d(}}\Psi {\text{ - M)}}} 
 \\
  =& \frac{2}{{\pi n}}\left( {\int_0^\pi  {\cos nM{\text{d}}\Psi }  - \underbrace {\int_0^\pi  {\cos nM{\text{d}}M} }_{ = 0}} \right) = \frac{2}{n}\left( {\frac{1}{\pi }\int_0^\pi  {\cos (n\Psi  - en\sin \Psi ){\text{d}}\Psi } } \right)
  \\
   =& \frac{2}{n}{J_n}(en)

\end{align}
$$

The first term in the second line vanishes by the assumption of the fourier expansion of $e\sin \Psi $. The second equality in the third line uses Kepler Equation again. Thus, the solution of Kepler equation is
$$
\Psi  = M + \sum {\frac{2}{n}{J_n}(en)} \sin (nM)
$$
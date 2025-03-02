# Little-o

In addition to the big-O, big- $\Omega$, and big- $\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little- $o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

$f(n)\in o(g(n)) \implies  f(n)\in O(g(n))$
  
$\forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)  \implies \forall c>0, \exists n_0, \forall n\ge n_0: f(n) \le c g(n)$
  
$\forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)  \implies \forall x>0, \exists z_0, \forall z\ge z_0: f(z) \le c g(z)$ { rename variables, on right hand side of implication: $c = x, n=z, n_0 = z_0$ }

$\forall x>0, \exists c>0, \forall n_0, \exists z_0, \forall z \ge z_0, \exists n \ge n_0 [f(n) < cg(n) \implies f(z) \le xg(z) ]$ {migrate quanifiers}

$(f(z_c) < x_c g(z_c)) \implies (f(z) \le xg(z))  $ remove quanitiferes (convention: for some variable x, $x_c$ means choice of x, works when variable x is from a $\forall$ and other variable is $\exists$):

$x>0, c = x_c, z_0 = n_{0C}, z  \ge n_{0C}, n = z_c $

$(f(z_c)<x_c g(z_c)) \implies (f(z) \le xg(z))$ 

Therefore since $f(z_c) = f(z)$ and $x_c g(z_c) = xg(z)$ the above will be true since
if $x < y$ then $x \le y$








I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

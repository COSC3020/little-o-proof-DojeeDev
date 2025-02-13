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
  
Choose $n_0$ such that $O(g(n)) \subset o(g(n))$
Implication will be true given that O is a subset of o.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

$f(n)\in O(g(n)) \iff \exists c,n_0 >0, \forall n\ge n_0: f(n) \le c g(n)$

By the definition of little o, $f(n) < c * g(n)$ for every positive constant $c$. This means $f(n)$ grows strictly slower than $g(n)$ because it is always less than $c * g(n)$ for any $c > 0$. If $f(n)$ satisfies this condition,  then it must also be less than or equal to c.g(n) for a specific c, which is the definition of big O.

Thus, by definition, $f(n) \in o(g(n))$ implies $f(n) \in O(g(n))$.

Other difference:

In big O notation, we have $f(n) <= c*(g(n))$ for all $n > n_0$ for some constants c and $n_0$. This implies that there exists a constant scaling factor c such that f(n) is bounded above by $c*(g(n))$ for sufficiently large values of n. On the other hand, in little o notation, we have $f(n) < c*(g(n)))$ for all $n > n_0$ for any positive constant c. This means that for any constant scaling factor c, no matter how large, f(n) will always be strictly less than c*g(n) for sufficiently large values of n. Therefore, $f(n)\in o(g(n))$ implies that $f(n)\in O(g(n))$.

References: This is my proof I did for my little o proof last time. 

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice

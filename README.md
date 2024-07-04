
### Sigma algebra
$\pmb {Definition}$ Let $\Omega$ be a (non-empty) set. A collection $A\subseteq 2 ^\Omega$ of subsets of Ω is called an
algebra on $\Omega$ if 
$\mathcal{A} 1. \ \emptyset \in \mathcal{A};$ //
$\mathcal{A} 2.$ For every $A \subseteq \Omega,$ if $A \in \mathcal{A},$ then $A^c \in \mathcal{A}$ 

$\mathcal{A}3.$ For every $A,\ B \subseteq \Omega,$ if $A, \ B \in \mathcal{A},$ then $A \cup B \in \mathcal{A}$ 

An algebra $\mathcal F$ is called a $\sigma-algebra$ or $\sigma-field$ if it also satisfies the following additional condition

$\sigma \mathcal{A}4.$ For every countable collection {${A_n : n=1,2,3,....}$} of subsets of  $\Omega$ with$A_n \in \mathcal F$ for each $n \geq 1,$

\begin{align*}
\[ \bigcup_{n=1}^{\infty} A_n \in \mathcal F \]
\end{align*}


$$
\begin{align*}
\bigcup_{n=1}^{\infty} A_n &\in \mathcal{F} \\
\end{align*}
$$

### Measure space
If $\Omega$ is a set and $\mathcal F$ is a sigma algebra on $\Omega$, we will call the pair ($\Omega$, $\mathcal F$) a measurable space and
the elements of $\mathcal F$ will be called measurable sets.


### stochastic processes
$\pmb {Definition}$ Let ($\Omega$, $\mathcal F$, $\mathbb {P}$) be a probability space and $\emptyset \neq \mathbb I \subseteq [0, \infty)$ be a set. A stochastic
process $X= \{ X_t : t \in \mathbb I})$ is a collection of random variables. We call I the index set. If $\mathbb I \subseteq \mathbb N,$
we call X a discrete-time stochastic process, while if $\mathbb I = [0,\infty)$ or $\mathbb I = [0, T]$ for some $T > 0$, we
call X a continuous-time stochastic process.


### Filtration 

$\pmb {Definition}$ Let ($\Omega$, $\mathcal F$, $\mathbb {P}$) be a probability space and $\mathbb I = [0, \infty)$ be an index set. A filtration $\mathbb {F} = \{ \mathcal F_t:t \in \mathbb I \}$ is an increasing collection of $sub-\sigma-algebras$ of $\mathcal F$; i.e., $\mathcal F_s \subseteq \mathcal F_t \subseteq \mathcal F$ for $s \leq t,$ $s, t \in \mathbb I$. A stochastic process $X = {X_t: t \in \mathbb I}$ is adapted to a filtration $\mathbb F$ if for every $t \in \mathbb I,$
$X_t$ is $\mathcal F_t-measurable$

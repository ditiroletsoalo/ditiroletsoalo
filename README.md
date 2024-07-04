
### Sigma algebra
$\pmb {Definition}.$ Let $\Omega$ be a (non-empty) set. A collection $A\subseteq 2 ^\Omega$ of subsets of Ω is called an
algebra on $\Omega$ if 
$\mathcal{A} 1. \ \emptyset \in \mathcal{A};$ 

$\mathcal{A} 2.$ For every $A \subseteq \Omega,$ if $A \in \mathcal{A},$ then $A^c \in \mathcal{A}$ 

$\mathcal{A}3.$ For every $A,\ B \subseteq \Omega,$ if $A, \ B \in \mathcal{A},$ then $A \cup B \in \mathcal{A}$ 


An algebra $\mathcal F$ is called a $\sigma-algebra$ or $\sigma-field$ if it also satisfies the following additional condition



$\sigma \mathcal{A}4.$ For every countable collection $\{A_n : n=1,2,3,\ldots\}$ of subsets of $\Omega$ with $A_n \in \mathcal{F}$ for each $n \geq 1,$

$$
\begin{align*}
\bigcup_{n=1}^{\infty} A_n &\in \mathcal{F} \\
\end{align*}
$$

### Measure space
If $\Omega$ is a set and $\mathcal F$ is a sigma algebra on $\Omega$, we will call the pair ($\Omega$, $\mathcal F$) a measurable space and
the elements of $\mathcal F$ will be called measurable sets.


### stochastic processes
$\pmb {Definition}.$ Let ($\Omega$, $\mathcal F$, $\mathbb {P}$) be a probability space and $\emptyset \neq \mathbb I \subseteq [0, \infty)$ be a set. A stochastic
process $X= \{ X_t : t \in \mathbb I})$ is a collection of random variables. We call I the index set. If $\mathbb I \subseteq \mathbb N,$
we call X a discrete-time stochastic process, while if $\mathbb I = [0,\infty)$ or $\mathbb I = [0, T]$ for some $T > 0$, we
call X a continuous-time stochastic process.


### Filtration 

$\pmb {Definition}.$ Let ($\Omega$, $\mathcal F$, $\mathbb {P}$) be a probability space and $\mathbb I = [0, \infty)$ be an index set. A filtration $\mathbb {F} = \{ \mathcal F_t:t \in \mathbb I \}$ is an increasing collection of $sub-\sigma-algebras$ of $\mathcal F$; i.e., $\mathcal F_s \subseteq \mathcal F_t \subseteq \mathcal F$ for $s \leq t,$ $s, t \in \mathbb I$. A stochastic process $X = {X_t: t \in \mathbb I}$ is adapted to a filtration $\mathbb F$ if for every $t \in \mathbb I,$
$X_t$ is $\mathcal F_t-measurable$



### Preface

This research explores the intersection of financial mathematics, machine learning, and econometrics to develop advanced hedging strategies in incomplete markets. The primary focus is on mean-variance hedging, a well-established method aimed at minimizing portfolio risk relative to a target payoff. Leveraging the capabilities of neural networks, we aim to approximate optimal hedging strategies, addressing the inherent complexities and high-dimensional nature of financial data.

A significant innovation in this research is the use of Vector Autoregression (VAR) models as the underlying sample path generators. VAR models are powerful tools in econometrics, capable of capturing linear interdependencies among multiple time series. By fitting a VAR model to historical data, we can simulate realistic future scenarios, providing a robust framework for training our neural network-based hedging strategies.

The project's framework is set within a filtered probability space $(\Omega, \mathcal{F}, \mathbb{F}, P)$, with $X = \{(X_t^1, \ldots, X_t^d) : t \geq 0\}$ representing the discounted prices of multiple risky assets modeled as a $d$-dimensional cadlag semimartingale. Our objective is to find the initial capital and trading strategy that minimize the expected squared replication error, providing a theoretically sound and practically viable solution to hedging in incomplete markets.

By integrating the statistical rigor of VAR models with the approximation power of neural networks, this research aims to contribute to the field of quantitative finance, offering new insights and tools for effective risk management. The outcomes of this study have the potential to enhance the robustness and accuracy of hedging strategies, ultimately benefiting financial practitioners and advancing academic understanding in this domain.

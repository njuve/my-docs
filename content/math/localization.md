---
title: "Localization"
date: 2020-02-22T23:38:35+09:00
draft: False
mathjax: true
---
# Aim

Aim of this article is to understand the localization of $F[q]$ at the ideal $(q)$, where $F$ is an algebraically closed field and $q$ is a parameter.

# Localization
Let $A$ be an integral domain.


>$S$ is __multiplicatively closed__ if $S$ satifies
>
>- $1 \in S$,
>
>- $a, b \in S \Rightarrow ab \in S$.


For $(a, s), (b, t) \in A \times S$, we define the relation $R$ in $(A \times S)$:
$$
(a, s) R (b, t) \overset{\mathrm{def}}{\iff} at = bs
$$

$R$ is a equivalence relation, then we can consider its quontient $A/R$.
we denote $A/R$ by $A_S$ and $(a, s) \in A_S$ by $a/s$. Also, its operations are defined by
$$
\frac{a}{s} + \frac{b}{t} = \frac{at - bs}{st}, \quad \frac{a}{s} \cdot \frac{b}{t} = \frac{ab}{st}
$$

$A_S$ is called the __localization__ of $A$ at $S$.

We can consider a hom from $A$ to $A_S$ by $a \to a/1$. For $s \in S$, $s$ is $s/1$ in $A_S$ and there exists $1/s \in A_S$, then $s/1 \in A^{\times}$. Thus localization is like creating inverse elements for elements of $S$ (if $A$ is integral domain).

## Example1

Let $P$ be a prime ideal and set $S = A \backslash P$.
Then $S$ is multiplicatively closed,
it is clear by definition of prime ideals ($ab \not\in P \Rightarrow a \not\in P \land b \not\in P$).
Thus we can consider the localization $A_S$.
At this time $A_S$ becomes a local ring with the maximal ideal $pA_S$:
$$
pA_S = \\{ p/s \mid p \in P, s \in S\\}
$$

## Example2

Let $F$ be an algebraically closed field.
Set $A = F[x]$.
For $a \in F$, set $P = \langle x - a \rangle$.

Now the ring we have considered is $F[x]$, then $P$ is a prime ideal.
By Example1,  $S = F[x] \backslash P$ is a multiplicatively closed.
Then we can consider the localization $A_S$, especially a local ring.
At this time, we are going to denote $A_S$ by $A_a$.
Let's see $A_a$ a little better.
$$
A_a = \\{ a/s \mid a \in A, s \in S\\}
$$
Since $S = F[x] \backslash P$,
$$
\begin{align*}
    A_a &= \\{ a/s \mid a \in A, s \in S\\} \\\\
        &= \\{ a/s \mid a \in A, s(a) \neq 0\\}
\end{align*}
$$

# Main Situation
## Localization at $(x)$

In Example2, we consider the case that $a = 0$. Then
$$
\begin{align*}
    A_0 &= \\{ a/s \mid a \in A, s \in S\\} \\\\
        &= \\{ a/s \mid a \in A, s(0) \neq 0\\}
\end{align*}
$$

## Localization at $(x^{-1})$
Set $A = F(x^{-1})$. We will consider the locarization at $(x^{-1})$. At this time, we consider $\infty$ as formal element and denote $A_S$ by $A_{\infty}$.
$$
\begin{align*}
    A_{\infty} &= \\{ a/s \mid a \in A, s \in S\\} \\\\
               &= \\{ a/s \mid a \in A, s(\infty) \neq 0\\}
\end{align*}
$$

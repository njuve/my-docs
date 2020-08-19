---
title: "Reductive Lie Algebra"
date: 2020-08-19T19:22:50+09:00
draft: false
mathjax: true
---

# Definition
Let $\mathfrak{g}$ be a finite dimentional lie algebra.

>$\mathfrak{g}$ is called **reductive** if there exist a semisimple lie algebra $\mathfrak{a}$ s.t. $\mathfrak{g} =  \mathfrak{a} \oplus \mathfrak{c}$ where $\mathfrak{c}$ is the center of $\mathfrak{g}$.

$\mathfrak{g}$ is reductive means the adjoint representation is a completely reducible.

# Example 1
For $\mathfrak{gl}_n$ We have
$$
    \mathfrak{gl}_n = \mathfrak{sl}_n \oplus \mathfrak{t}
$$
where $\mathfrak{t} = \mathbb{C} \cdot I_n$.
Then $\mathfrak{gl}_n$ is a reductive lie algebra.

# Example 2

If $n = 2$ in example 1, we have
$$
\begin{align*}
    \mathfrak{gl}_2
    &= \mathfrak{sl}_2 \oplus \mathfrak{t}\\\\
    &= \left(
            \left(
                \bigoplus_{i>j} \mathbb{C} E_{ij}
            \right)
            \oplus
            \left(
                \bigoplus \mathbb{C} (E_{ii} - E_{i+1,i+1})
            \right)
            \oplus
            \left(
                \bigoplus_{i>j} \mathbb{C} E_{ji}
            \right)
        \right)
        \oplus
        \mathbb{C} \cdot I_n\\\\
    &= \mathbb{C}E_{12} \oplus \mathbb{C}(E_{11} - E_{22}) \oplus \mathbb{C} E_{21} \oplus \mathbb{C} (E_{11} + E_{22})
\end{align*}
$$

## Example
Crealy a semisimple lie algebra is reductive.

## Ref
- [Wikipedia](https://en.wikipedia.org/wiki/Reductive_Lie_algebra)
- [nLab](https://ncatlab.org/nlab/show/reductive+Lie+algebra)
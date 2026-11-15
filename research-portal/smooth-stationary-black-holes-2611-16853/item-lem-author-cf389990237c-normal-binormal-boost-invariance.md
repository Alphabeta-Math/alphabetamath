---
title: The normal binormal is invariant under oriented boosts
status: published
research_item: lem-author-cf389990237c-normal-binormal-boost-invariance
dependency_level: 2
---

## Prerequisites

- [def-author-cf389990237c-normalized-horizon-komar-data](item-def-author-cf389990237c-normalized-horizon-komar-data)
- [math:def-hyperbolic-functions](https://alphabetamath.cc/item/def-hyperbolic-functions)
- [math:thm-hyperbolic-identities-and-derivatives](https://alphabetamath.cc/item/thm-hyperbolic-identities-and-derivatives)


## Statement

For the normal pair in [def-author-cf389990237c-normalized-horizon-komar-data](item-def-author-cf389990237c-normalized-horizon-komar-data), replace $n,s$ by $n'=\cosh\beta\,n+\sinh\beta\,s$ and $s'=\sinh\beta\,n+\cosh\beta\,s$, where $\beta$ is any supplied smooth real function on $C$. Then $n',s'$ have the same normalizations and $b'_{ab}=b_{ab}$. Thus $Q_C[T]$ does not depend on this change of oriented normal frame.

## Facts & Assumptions

[F1] The normal pair has Gram matrix $\operatorname{diag}(-1,1)$ and the functional uses only its binormal and the section area measure. [def-author-cf389990237c-normalized-horizon-komar-data](item-def-author-cf389990237c-normalized-horizon-komar-data)

[F2] The real functions $\sinh$ and $\cosh$ are defined on all of $\mathbb R$; for every real $x$, $\cosh^2x-\sinh^2x=1$ and $\cosh x>0$. Apply these facts pointwise at $x=\beta(p)$ for $p\in C$. [math:def-hyperbolic-functions](https://alphabetamath.cc/item/def-hyperbolic-functions) [math:thm-hyperbolic-identities-and-derivatives](https://alphabetamath.cc/item/thm-hyperbolic-identities-and-derivatives)

## Proof

**Given:**The normal pair and boost in the Statement.

**Goal:** Check preservation of the binormal.

1.1 Bilinearity and $\cosh^2\beta-\sinh^2\beta=1$ give $g(n',n')=-1$, $g(s',s')=1$ and $g(n',s')=0$. Both remain normal to $C$, and the boost preserves the future and normal-plane orientation choices. [given, F1, F2]

2.1 Expanding $s'_an'_b-n'_as'_b$ cancels the pure $n_an_b$ and $s_as_b$ terms; the remaining multiplier of $s_an_b-n_as_b$ is $\cosh^2\beta-\sinh^2\beta=1$. The functional therefore has exactly the same integrand. [F1, F2, step 1.1] ∎

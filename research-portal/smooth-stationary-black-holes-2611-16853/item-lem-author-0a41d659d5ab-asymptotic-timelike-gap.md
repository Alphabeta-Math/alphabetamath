---
title: The quantitative asymptotic end is uniformly timelike
status: published
research_item: lem-author-0a41d659d5ab-asymptotic-timelike-gap
dependency_level: 3
sources:
  references:
    - title: S. Alexakis, A. D. Ionescu and S. Klainerman, Rigidity of stationary
        black holes with small angular momentum on the horizon
      url: https://arxiv.org/pdf/1304.0487v2
      locator: Section 1.2, equations (1.6)–(1.10), PDF pages 5–6
---

## Prerequisites

- [def-author-0a41d659d5ab-aik-quantitative-package](item-def-author-0a41d659d5ab-aik-quantitative-package)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

For the AIK quantitative package, $g(T,T)\le-1/2$ on $\Sigma_{R_1}$. In particular the stationary field is timelike throughout that end, independently of the horizon-smallness parameter.

## Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The source end coordinates have $T=\partial_0$, $|g_{00}+1-2M_0/r|\le A_1r^{-2}$ and the chosen radius satisfies $R_1\ge8M_0$ and $R_1\ge2\sqrt{A_1}$. [def-author-0a41d659d5ab-aik-quantitative-package](item-def-author-0a41d659d5ab-aik-quantitative-package)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conditional conclusion.

1.1 On the end the stationary field is the coordinate vector $\partial_0$, so $g(T,T)=g_{00}$. The zeroth-order term of the quantitative end bound gives $g_{00}\le-1+2M_0/r+A_1/r^2$. [F1, given, algebra]

2.1 For $r\ge R_1$, the two positive terms are at most $1/4$ each by the chosen lower bounds on $R_1$. Hence $g(T,T)\le-1+1/4+1/4=-1/2$, as asserted. No horizon estimate enters this calculation. [step 1.1, F1, algebra] ∎

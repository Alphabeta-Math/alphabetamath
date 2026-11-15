---
title: The source maximal-gauge expansion can be used on the same CW slice
status: draft
research_item: lem-author-294e9b08725d-maximal-end-same-slice-polyhomogeneous-gauge
dependency_level: 6
---

## Prerequisites

- [lem-author-294e9b08725d-maximal-end-cw-weak-kid-data](item-lem-author-294e9b08725d-maximal-end-cw-weak-kid-data)
- [thm-author-294e9b08725d-maximal-end-polyhomogeneous-input](item-thm-author-294e9b08725d-maximal-end-polyhomogeneous-input)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

For the supplied end in the preceding lemma, apply the imported stationary maximal-gauge regularity input in the time coordinate tau already fixed there. Choose spatial coordinates y harmonic for the Riemannian quotient metric. This changes only spatial coordinates; the same maximal slice remains $\tau=0$ and $T=\partial_\tau$. In these coordinates the induced metric h, lapse N and shift X have full differentiated polyhomogeneous expansions in integer powers of $r^{-1}$ with finite powers of $\log r$ at each order, and $h-\delta$, $N-1$, X are $O_\infty(r^{-1})$.

Here full differentiated polyhomogeneity means that every finite expansion has a remainder with the corresponding differentiated asymptotic estimates; it is not an analyticity or convergence assertion. This lemma invokes the stated external regularity result, not a locally reconstructed proof of that result and not a replacement of the global maximal hypersurface.

## Facts & Assumptions

[F1] The existing CW end already has a stationary time coordinate tau with that same maximal slice at zero and the required weak end data. [lem-author-294e9b08725d-maximal-end-cw-weak-kid-data](item-lem-author-294e9b08725d-maximal-end-cw-weak-kid-data)

[F2] The independent source packet supplies maximal-stationary-gauge polyhomogeneity and the normalized vacuum maximal KID identities. [thm-author-294e9b08725d-maximal-end-polyhomogeneous-input](item-thm-author-294e9b08725d-maximal-end-polyhomogeneous-input)

[F3] Work in ZFC, including the inherited analytic choice assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:**The actual end hypotheses in the Statement.

**Goal:** Prove the stated same-slice end consequence.

1.1 The quotient metric is the positive metric transverse to T on its timelike end. Its coefficients in the original spatial coordinates are $\gamma_{ij}=g_{ij}-g_{0i}g_{0j}/g_{00}$ and are unaffected by a stationary change of time origin. Thus quotient-harmonic spatial coordinates are functions of x alone. Use the source spatial-coordinate choice while retaining tau as the stationary time parameter. Maximality is the geometric zero mean-curvature condition of the supplied $\tau=0$ hypersurface, so it is already the source maximal-time gauge condition; there is no further time equation whose solution would select a different slice. [F1, F2, given, algebra]

2.1 The logarithmic initial graph and the original regular vacuum end meet the weak initial-data conditions as established in [F1], and initially give power falloff for every exponent strictly below one. Apply the source packet in this already imposed gauge. It supplies full differentiated expansions and the improved order $\alpha=n$-2=1 in three spatial dimensions. The ADM fields h,N,X are smooth algebraic functions of the stationary metric fields on the uniformly spacelike end, so they inherit these expansions and bounds. This is precisely the one imported regularity step; all subsequent coefficient and logarithm exclusions are authored locally. [F1, F2, step 1.1] ∎

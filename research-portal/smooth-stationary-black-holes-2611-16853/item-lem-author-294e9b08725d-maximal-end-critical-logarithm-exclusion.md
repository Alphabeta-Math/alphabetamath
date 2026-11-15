---
title: The first possible shift and lapse logarithms vanish by indicial projection
status: draft
research_item: lem-author-294e9b08725d-maximal-end-critical-logarithm-exclusion
dependency_level: 8
---

## Prerequisites

- [lem-author-294e9b08725d-maximal-end-leading-stationary-modes](item-lem-author-294e9b08725d-maximal-end-leading-stationary-modes)
- [thm-author-294e9b08725d-maximal-end-polyhomogeneous-input](item-thm-author-294e9b08725d-maximal-end-polyhomogeneous-input)
- [math:lem-pe18-spherical-harmonic-structure-and-density](https://alphabetamath.cc/item/lem-pe18-spherical-harmonic-structure-and-density)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

In the final spatial normalization of the preceding lemma, every logarithmic coefficient at order $r^{-2}$ in X and N vanishes. Consequently
$$X=O_\infty(r^{-2}),\qquad N=1-m/r+O_\infty(r^{-2}).$$
This excludes only the critical logarithms needed for the article end gauge; it does not assert absence of every higher polyhomogeneous logarithm.

## Facts & Assumptions

[F1] The same maximal end has isotropic leading spatial Schwarzschild correction, radial leading lapse and shift beginning at order $r^{-2}$. [lem-author-294e9b08725d-maximal-end-leading-stationary-modes](item-lem-author-294e9b08725d-maximal-end-leading-stationary-modes)

[F2] The maximal vacuum vector, lapse and trace identities hold in every spatial coordinate system. [thm-author-294e9b08725d-maximal-end-polyhomogeneous-input](item-thm-author-294e9b08725d-maximal-end-polyhomogeneous-input)

[F3] The self-adjoint operator Delta_S2 plus two has kernel exactly the degree-one spherical harmonics; a constant function is orthogonal to that kernel. [math:lem-pe18-spherical-harmonic-structure-and-density](https://alphabetamath.cc/item/lem-pe18-spherical-harmonic-structure-and-density)

[F4] Work in ZFC, including the inherited analytic choice assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The actual end hypotheses in the Statement.

**Goal:** Prove the stated same-slice end consequence.

1.1 Put P equal to Delta_S2 plus two. Direct differentiation gives $\Delta_0(r^{-2}(\log r)^ja)=r^{-4}[P a(\log r)^j-3j a(\log r)^{j-1}+j(j-1)a(\log r)^{j-2}]$. The vector KID equation, with $X=O(r^{-2}\log^Jr)$ and $k=(2N)^{-1}\mathcal L_Xh=O(r^{-3}\log^Jr)$, has no $r^{-4}$ forcing after moving its metric and Ricci corrections to the right: all such terms have order at most $r^{-5}$ times finite log powers. If $J>0$ is the largest $r^{-2}$ shift-log power, its coefficient $a_J$ lies in ker P; projecting the next log coefficient equation onto ker P gives $-3J a_J=0$. Thus the highest coefficient vanishes, and descending induction removes all positive log powers in the $r^{-2}$ shift. [F1, F2, F3, given, algebra]

2.1 Now $k=O_\infty(r^{-3})$. For $N_0=1-m/r$ and $h=(1+2m/r)\delta+O(r^{-2}\log^Jr)$, the coordinate Laplacian formula gives $\Delta_hN_0=-m^2r^{-4}+O(r^{-5}\log^{J'}r)$. The lapse equation $\Delta_hN=N|k|^2$ therefore has only radial forcing $m^2$ at the $r^{-4}$ equation for the $r^{-2}$ coefficient of $N-N_0$. For a largest positive log power the same projection calculation gives $-3J b_J=0$: when $J=1$ the constant-log equation has the radial right side, whose projection onto degree-one harmonics is zero. Hence all positive log powers at this order vanish as well. [F1, F2, F3, step 1.1, algebra]

3.1 The remaining higher-order terms start at $r^{-3}$ with finite log powers and differentiated remainders. Each such finite log power times $r^{-3}$ is bounded by a constant times $r^{-2}$, with the corresponding extra radius factors after every fixed derivative. The full expansion in [F1] therefore proves both displayed O-infinity assertions. No convergence of the formal expansion is required. [F1, step 1.1, step 2.1, algebra] ∎

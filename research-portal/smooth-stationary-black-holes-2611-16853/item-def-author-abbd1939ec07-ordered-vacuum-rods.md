---
title: Ordered horizon rods and twist-jump labels
status: published
research_item: def-author-abbd1939ec07-ordered-vacuum-rods
dependency_level: 5
sources:
  references:
    - title: Han–Khuri–Weinstein–Xiong, Kerr Black Hole Uniqueness
      url: https://arxiv.org/html/2608.23325v1
      locator: §1, Weyl–Papapetrou setting (1.1)–(1.4), ordered rods (1.5), axis
        traces (1.6), and orientation-qualified jump formula (1.7)
      statement: For ordered horizon intervals, the complementary open axis intervals
        have twist traces v=c_j. With the orientation specified before (1.7),
        the horizon angular momentum is J_i=(c_{i+1}-c_i)/4. Only the rod
        nomenclature and numerical convention are adopted here.
      hypotheses: The source uses stationary axisymmetric vacuum Weyl–Papapetrou
        metrics, rotational period 2π, ordered horizon components and a twist
        potential constant on each axis rod. The sign in (1.7) uses the
        orientation convention of its references [16,17]. Abstract numerical
        labels here do not assert geometric realization or a Komar
        identification.
      reading_limits: Read the source HTML §1 setting and displayed equations
        (1.1)–(1.7), including the orientation sentence. The Komar-integral
        derivation and references [16,17] were not checked; no uniqueness or
        balance proof is imported.
---

## Prerequisites

- [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-interval](https://alphabetamath.cc/item/def-interval)
- [` Han–Khuri–Weinstein–Xiong, Kerr Black Hole Uniqueness · §1, Weyl–Papapetrou setting (1.1)–(1.4), ordered rods (1.5), axis traces (1.6), and orientation-qualified jump formula (1.7) `](https://arxiv.org/html/2608.23325v1)


## Definition

An ordered finite vacuum rod datum consists of an integer $N\ge1$, real numbers $z_i^-\le z_i^+$ for $1\le i\le N$ and $z_i^+<z_{i+1}^-$ for $1\le i<N$, and intervals $\mathcal H_i=[z_i^-,z_i^+]$. A strict interval is called a nondegenerate horizon rod and an interval with equal endpoints a degenerate puncture $p_i=(0,0,z_i^-)$. In this abstract rod datum these names label the intervals; their identification with geometric event horizons is a separate theorem.

The complementary axis intervals are $\Gamma_1=(-\infty,z_1^-)$, $\Gamma_{j+1}=(z_j^+,z_{j+1}^-)$ for $1\le j<N$, and $\Gamma_{N+1}=(z_N^+,\infty)$. Supply real constants $c_1,\ldots,c_{N+1}$. The labels $\mathcal J_i=(c_{i+1}-c_i)/4$ are the angular-momentum parameters in the HKWX convention. A shift of every $c_j$ by the same constant is a twist gauge change and leaves these labels unchanged. Their identification with Komar integrals of a geometric spacetime is not asserted by this definition.

## Facts & Assumptions

[F1] The stationary axial-action terminology, when a geometric realization is supplied, is [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data). Work in ZFC, [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice). The ordered intervals and real constants themselves are finite numerical data.

[F2] Open, closed and unbounded real intervals, their nonemptiness conditions, and the singleton case $[a,a]=\{a\}$ use [math:def-interval](https://alphabetamath.cc/item/def-interval).

## Justification

**Given:** The integer, ordered endpoints and constants.

**Goal:** Verify the interval decomposition and gauge-invariant labels.

1.1 By the supplied interval definitions, every intervening interval is nonempty: its endpoints satisfy $z_j^+<z_{j+1}^-$ and their midpoint lies strictly between them. The two exterior intervals are semi-infinite. All complementary axis intervals together with the horizon intervals exhaust the real axis: $\mathbb R=(\bigcup_{i=1}^N\mathcal H_i)\cup(\bigcup_{j=1}^{N+1}\Gamma_j)$. Indeed, a real number below $z_1^-$ or above $z_N^+$ lies in an exterior interval; otherwise, if it belongs to no horizon interval, the ordered finite endpoints place it strictly between two consecutive horizon intervals. Equal endpoints give singletons and do not collapse either neighboring open interval because the adjacent strict inequalities remain. [given, F1, F2, algebra]

2.1 Each difference $c_{i+1}-c_i$ is a definite real number, and a common additive shift cancels in the difference. Division by four defines the stated labels without a choice of primitive. Their geometric interpretation requires reconstruction data in addition to these finite labels. [given, step 1.1, algebra] ∎

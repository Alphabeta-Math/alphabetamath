---
title: Bounded spacelike stationary graphs remain Cauchy
status: draft
research_item: lem-author-d20d145f998f-bounded-stationary-graph
dependency_level: 1
sources:
  references:
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://link.springer.com/article/10.1007/s41114-019-0019-x
      locator: Sections 1.2–1.7 and 1.11; Definitions 1.21–1.22 and following
        assertion; Theorem 2.12 and Remark 2.14; Definition 2.16
      statement: In general spacetime dimension, causal AC-curves are continuous
        causal curves. Temporal functions increase strictly along causal curves.
        Inextendibility means absence of endpoints.
      hypotheses: Connected time-oriented smooth Hausdorff second-countable Lorentzian
        manifold; nonzero future causal velocity almost everywhere; smooth
        function with past timelike gradient.
      reading_limits: Read the indicated definitions, temporal-to-time assertion, and
        curve-equivalence statement and proof. No four-dimensional restriction
        is present. No general causal-calculus theorem is claimed to have been
        reconstructed.
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://link.springer.com/article/10.1007/s41114-019-0019-x
      locator: Theorem 4.119, both the Cauchy/global-hyperbolicity equivalence and the
        timelike-fiber topological splitting
      statement: A spacetime with a Cauchy hypersurface is globally hyperbolic and
        admits a homeomorphism to R times a hypersurface with timelike fibers
        and time-function first coordinate.
      hypotheses: The source spacetime conventions; existence of a Cauchy
        hypersurface. Applied to the original supplied C, before establishing
        anything about the new graph.
      reading_limits: Read the complete theorem statement and its surrounding
        attribution, not a proof of the splitting theorem. Only existence of an
        inextendible timelike fiber is used; the new graph is never assumed
        Cauchy.
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://link.springer.com/article/10.1007/s41114-019-0019-x
      locator: Definitions 3.29 and 3.35, including the observation immediately after
        Definition 3.35
      statement: The domain of dependence consists of points whose inextendible causal
        curves meet the set. A closed acausal set with full domain of dependence
        is Cauchy.
      hypotheses: The source spacetime conventions; closedness and acausality for the
        Cauchy-hypersurface definition.
      reading_limits: Read these definitions and the once-only crossing observation;
        used as formulation inputs, not an imported proof of the graph claim.
---

## Prerequisites

- [lem-author-d20d145f998f-stationary-product-cauchy-time](item-lem-author-d20d145f998f-stationary-product-cauchy-time)
- [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)
- [math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)
- [` E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22 (2019), article 3 · Sections 1.2–1.7 and 1.11; Definitions 1.21–1.22 and following assertion; Theorem 2.12 and Remark 2.14; Definition 2.16 `](https://link.springer.com/article/10.1007/s41114-019-0019-x)
- [` E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22 (2019), article 3 · Theorem 4.119, both the Cauchy/global-hyperbolicity equivalence and the timelike-fiber topological splitting `](https://link.springer.com/article/10.1007/s41114-019-0019-x)
- [` E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22 (2019), article 3 · Definitions 3.29 and 3.35, including the observation immediately after Definition 3.35 `](https://link.springer.com/article/10.1007/s41114-019-0019-x)


## Statement

In the stationary product of the preceding lemma, let $u:C\to\mathbb R$ be a smooth bounded function, and put $C_u=\{\Psi(u(p),p):p\in C\}$. Suppose $C_u$ is spacelike. Then $\tau(\Psi(s,p))=s-u(p)$ is a Cauchy temporal function with $C_u=\tau^{-1}(0)$. Every complete $T$-orbit meets $C_u$ exactly once, and $C_u$ is diffeomorphic to $C$. If $u=0$ near a boundary in an ambient smooth completion of $C$, the new graph agrees with the old section there. Spacelikeness is an explicit condition; boundedness alone does not imply it.

## Statement references

[lem-author-d20d145f998f-stationary-product-cauchy-time](item-lem-author-d20d145f998f-stationary-product-cauchy-time)

## Facts & Assumptions

[F1] The supplied product time $s$ is Cauchy temporal, and its levels are carried to one another by the stationary isometries. The hypotheses of the preceding lemma, including Countable Choice and Dependent Choice, are inherited. [lem-author-d20d145f998f-stationary-product-cauchy-time](item-lem-author-d20d145f998f-stationary-product-cauchy-time)

[F2] A smooth map is a smooth embedding when it is an injective immersion and a homeomorphism onto its image with the subspace topology. [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

[F3] Use the general-dimensional causal AC-curve convention, with nonzero future causal velocity almost everywhere and no endpoint at either end for inextendibility. A smooth function with past timelike gradient is temporal and strictly increases along every future causal curve; the continuous and AC conventions give the same oriented curves up to increasing reparametrization. These are the conventions and temporal-to-time input of Minguzzi, Definitions 1.21–1.22 and 2.16, Theorem 2.12 and Remark 2.14 (first citation below).

[F4] The existence of the original Cauchy hypersurface $C$ implies global hyperbolicity and a homeomorphism $H:E\to\mathbb R\times S$ with time-function first coordinate and timelike fibers (Minguzzi, Theorem 4.119; second citation below).

[F5] A closed acausal set $A$ is Cauchy when every inextendible causal curve meets $A$, equivalently $D(A)=E$; acausality makes the crossing unique (Minguzzi, Definitions 3.29 and 3.35; third citation below).

[F6] A continuous real function on a compact interval takes every value between its endpoint values. [math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)

## Proof

**Given:** The hypotheses in the Statement, including the inherited hypotheses of the stationary-product lemma.

**Goal:** Prove all the asserted graph and Cauchy-temporal conclusions.

1.1 If $E=\varnothing$, the supplied product diffeomorphism forces $C=\varnothing$, hence $C_u=\varnothing$. The function $\tau$ is the unique smooth real function on $E$; its pointwise temporal condition is vacuous, and every level meets every inextendible causal curve exactly once because no such curve exists in $E$. The empty graph map is a diffeomorphism from $C$ to $C_u$, and the orbit and boundary claims are vacuous. This proves every conclusion in the empty case. Henceforth assume $E\ne\varnothing$, so the product diffeomorphism also gives $C\ne\varnothing$. In the product chart the graph map is injective with inverse given by projection to $C$, and is an immersion since its derivative projects to the identity. It is an embedding because that projection is continuous on its image. Every level $\tau=c$ is the image $\phi_c(C_u)$ and therefore spacelike. Also $d\tau(T)=1$, so its kernel is exactly the tangent hyperplane of its level. The orthogonal line to this spacelike hyperplane is timelike, so $\nabla\tau$ is timelike everywhere. On connected $E$ its temporal orientation is constant: its pairing with the continuous future timelike field $-\nabla s$ is continuous and nowhere zero. Boundedness fixes that orientation below, without assuming $T$ itself causal. [given, F1, F2, F3]

2.1 Write $|u|\le B$. By [F4], fix $q\in S$ and the future timelike fiber $\gamma(a)=H^{-1}(a,q)$, $a\in\mathbb R$. It has no endpoint: convergence in $E$ as $a\to+\infty$ or $a\to-\infty$ would, by continuity of $H$, force its first coordinate to have a finite limit. Thus [F1] applies to this inextendible future causal curve. Along it, and indeed along every such curve, $s-B\le\tau\le s+B$, so $\tau$ has endpoint limits $-\infty$ and $+\infty$ in the past and future. If the orientation from step 1.1 were future timelike for $\nabla\tau$, then $-\tau$ would have past timelike gradient and would increase strictly along $\gamma$ by [F3]. That would make $\tau$ strictly decreasing, contradicting those limits. Hence $\nabla\tau$ is past timelike on all of $E$. [given, F1, F3, F4, step 1.1]

3.1 By [F3] and step 2.1, $\tau$ increases strictly along every future causal curve. For any inextendible one, the endpoint limits proved in step 2.1 and [F6] applied on a compact parameter interval bracketing a prescribed real value $c$ give a crossing of $\tau=c$; strict increase gives exactly one. Each level is closed as a level of a continuous function and acausal by strict increase, so [F5] makes it Cauchy. Thus $\tau$ is Cauchy temporal, with $C_u=\tau^{-1}(0)$. A stationary orbit has fixed product label $p$ and varying $s$, giving its single graph intersection $s=u(p)$; the graph map and the smooth projection inverse give the asserted diffeomorphism with $C$. The final boundary assertion is literal agreement where $u=0$. [given, F1, F2, F3, F5, F6, step 1.1, step 2.1] ∎

## External input

The three Minguzzi citations import only the general-dimensional causal/temporal conventions, the original-Cauchy-surface splitting theorem, and the Cauchy definition used in [F3]–[F5]. The embedding, bounded comparison, orientation selection and stationary-graph application are proved locally. This lemma is not itself an imported theorem.

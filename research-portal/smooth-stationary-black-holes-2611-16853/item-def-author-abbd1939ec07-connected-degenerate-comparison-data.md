---
title: Connected rotating degenerate vacuum comparison data
status: published
research_item: def-author-abbd1939ec07-connected-degenerate-comparison-data
dependency_level: 5
sources:
  references:
    - title: Amsel–Horowitz–Marolf–Roberts, Uniqueness of Extremal Kerr and
        Kerr-Newman Black Holes
      url: https://arxiv.org/pdf/0906.2367v3
      locator: §2 Theorem 1, printed p.2; §2 opening proof and footnote 2, printed p.3
        (terminology attribution)
    - title: Chruściel and Nguyen, A uniqueness theorem for degenerate Kerr-Newman
        black holes
      url: https://arxiv.org/pdf/1002.1737v1
      locator: Theorem 1.1, printed p.1; explicit I-plus-regular connected rotating
        degenerate hypotheses (terminology attribution)
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Definition

Work in ZFC. A connected rotating degenerate vacuum comparison datum consists of the time-oriented stationary four-dimensional Lorentzian data $(M,g,T)$ of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data), an asymptotically flat selected end, and the $I^+$-regularity, analyticity and causal-exterior conventions of [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data) and [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data). Require $\operatorname{Ric}(g)=0$. Require that the future event horizon $H^+=I_M^+(M_{\rm ext})\cap\partial_M D$ be nonempty and connected, and that it be a smooth Killing horizon for a specified nonzero generator $K$ with $d(g(K,K))=-2\kappa K^\flat$ on its nonzero-generator part and $\kappa=0$ there. Require that $T$ fail to be tangent to the null normal line somewhere on $H^+$; this is rotation relative to $T$. No bifurcation surface is part of these data.

Here $D$ is the domain of outer communications and $M_{\rm ext}$ the flow-saturated selected end. $I^+$-regularity requires completeness of $T$, global hyperbolicity of $D$, and the finite-end acausal section and once-only horizon-generator cross-section specified by the comparison definition. Connectedness is imposed on the horizon, not merely on that section. These are predicates on supplied data, not assertions that the data exist.

## Facts & Assumptions

[F1] Stationary geometry, causal sets, $I^+$-regularity and analytic charts are [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data), [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data) and [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data).

[F2] Surface gravity, null normal line, the nonzero-generator qualification and rotation are [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data). The inherited choice convention is [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice).

## Justification

**Given:** The supplied geometric objects and the displayed requirements.

**Goal:** Verify that the comparison class is a well-defined predicate without assuming a bifurcation surface or deriving axial symmetry.

1.1 The causal and comparison interfaces determine $M_{\rm ext}$, $D$ and $H^+$, so nonemptiness and connectedness are definite topological predicates. The stated completeness, regularity and analyticity requirements are likewise the explicit predicates in [F1]. [given, F1]

2.1 The horizon interface fixes the surface-gravity equation and rotation condition for the supplied fields. It therefore makes $\kappa=0$ and failure of stationary tangency unambiguous. Adding the tensor equation $\operatorname{Ric}(g)=0$ selects vacuum geometries. None of these operations produces an axial field or a bifurcation surface; those would be further results. [given, F1, F2] ∎

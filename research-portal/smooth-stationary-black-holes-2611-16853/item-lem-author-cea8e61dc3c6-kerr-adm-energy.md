---
title: The asymptotic metric flux of Kerr equals its mass parameter
status: draft
research_item: lem-author-cea8e61dc3c6-kerr-adm-energy
dependency_level: 3
sources:
  references:
    - title: The Kerr Metric
      url: https://arxiv.org/pdf/1410.2130
      locator: §2, equations (2.1), (2.5)–(2.8), PDF pp. 2–3
      statement: The review gives ingoing and Boyer–Lindquist Kerr forms, their
        coordinate transformation, and the asymptotic identification of mass M
        and angular momentum J=aM.
      hypotheses: The Kerr metric in the stated coordinate systems and their indicated
        domains.
      reading_limits: Read the cited formulas and surrounding discussion. This is
        background for the Kerr construction, not a proof of the full indexed
        statement or its normalization-specific calculations.
---

## Prerequisites

- [def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)
- [lem-author-cea8e61dc3c6-kerr-spatial-end](item-lem-author-cea8e61dc3c6-kerr-spatial-end)
- [` The Kerr Metric · §2, equations (2.1), (2.5)–(2.8), PDF pp. 2–3 `](https://arxiv.org/pdf/1410.2130)


## Statement

The ADM energy of the specified constant $t$ Kerr end exists and equals $E_{\rm ADM}=M$.

## Statement references

[def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)

[lem-author-cea8e61dc3c6-kerr-spatial-end](item-lem-author-cea8e61dc3c6-kerr-spatial-end)

## Facts & Assumptions

[F1] The following exact suppliers supply the geometric objects and earlier conclusions used here: [def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions) [lem-author-cea8e61dc3c6-kerr-spatial-end](item-lem-author-cea8e61dc3c6-kerr-spatial-end)

## Proof

**Given:**The ADM metric-flux convention and the differentiated expansion of [F1].

**Goal:** Evaluate the energy flux.

1.1 Put $k_{ij}=2Mx_ix_j/r^3$. Direct differentiation in dimension three gives $\partial_jk_{ij}=2Mx_i/r^3$ and $\partial_i k_{jj}=-2Mx_i/r^3$. Thus their difference contracted with $n^i$ is $4M/r^2$. The $O_2(r^{-2})$ remainder of the metric contributes $O(r^{-3})$ to this contracted integrand. [given, F1]

2.1 Integration over a Euclidean coordinate sphere gives $\int_{S_r}4M/r^2\,dS_0=16\pi M$. The integrated remainder is $O(r^{-1})$ and vanishes. Division by $16\pi$ and the limit in the definition yield $E_{\rm ADM}=M$. [given, F1, step 1.1] ∎

## External input

The cited Kerr coordinate formulas provide background for the local calculation in this item.

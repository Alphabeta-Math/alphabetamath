---
title: The Kerr end is an ADM rest frame
status: published
research_item: lem-author-cea8e61dc3c6-kerr-rest-frame
dependency_level: 4
sources:
  references:
    - title: The Kerr Metric
      url: https://arxiv.org/pdf/1410.2130
      locator: §2, equations (2.1), (2.5)–(2.9), PDF pp. 2–3
      statement: The ingoing and Boyer–Lindquist Kerr metric forms and their
        coordinate transformation are displayed; the review identifies M as the
        mass and the roots of the radial function as null horizon candidates.
      hypotheses: Kerr metric in the stated ingoing and Boyer–Lindquist coordinate domains.
      reading_limits: Consulted the browser-extracted PDF text of §2, equations (2.1),
        (2.5)–(2.9) and adjacent discussion on PDF pages 2–3. This supplies
        coordinate and parameter background only; it is not used as a proof of
        vanishing ADM momentum or the normalization-specific charge calculation.
        Those conclusions follow from the local argument and declared
        mathematical suppliers. No full-review reading or reconstruction of its
        proofs is claimed.
---

## Prerequisites

- [def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)
- [lem-author-cea8e61dc3c6-kerr-spatial-end](item-lem-author-cea8e61dc3c6-kerr-spatial-end)
- [lem-author-cea8e61dc3c6-kerr-adm-energy](item-lem-author-cea8e61dc3c6-kerr-adm-energy)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor)
- [` The Kerr Metric · §2, equations (2.1), (2.5)–(2.9), PDF pp. 2–3 `](https://arxiv.org/pdf/1410.2130)


## Statement

The constant $t$ Kerr end has vanishing ADM linear momentum and ADM rest mass $M_{\rm ADM}=M>0$.

## Statement references

[def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)

[lem-author-cea8e61dc3c6-kerr-spatial-end](item-lem-author-cea8e61dc3c6-kerr-spatial-end)

[lem-author-cea8e61dc3c6-kerr-adm-energy](item-lem-author-cea8e61dc3c6-kerr-adm-energy)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor)

## Facts & Assumptions

[F1] The following exact suppliers supply the geometric objects and earlier conclusions used here: [def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions) [lem-author-cea8e61dc3c6-kerr-spatial-end](item-lem-author-cea8e61dc3c6-kerr-spatial-end) [lem-author-cea8e61dc3c6-kerr-adm-energy](item-lem-author-cea8e61dc3c6-kerr-adm-energy) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] Work with the Kerr exterior parameters $M>0$ and $|a|\leq M$ of [lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor). In particular, the mass parameter in the end expansion and energy calculation is positive.

## Proof

**Given:** The asymptotic charge conventions, end expansions and energy calculation of [F1], with the positive Kerr mass parameter of [F2].

**Goal:** Distinguish rest mass from energy and show they agree here.

1.1 For the future unit normal $n=N^{-1}(\partial_t-\beta^i\partial_i)$, choose $K=\tfrac12\mathcal L_n h$ on tangent vectors. The stationary slicing identity is $K_{ij}=-(D_i\beta_j+D_j\beta_i)/(2N)$: it follows by writing $\partial_t=Nn+\beta$ in the Lie derivative of $h$, using $\mathcal L_{\partial_t}h=0$ and $\mathcal L_\beta h_{ij}=D_i\beta_j+D_j\beta_i$. The opposite convention has the opposite sign and the same estimates. By the end expansion $\partial\beta=O(r^{-3})$ and $\Gamma(h)\beta=O(r^{-4})$, so $K_{ij}=O(r^{-3})$ and $\operatorname{tr}_hK=O(r^{-3})$. [given, F1]

2.1 The momentum surface integrand is $O(r^{-3})$ while $\nu_h=O(1)$ and the area is $O(r^2)$. Each momentum limit is zero. Together with $E_{\rm ADM}=M$ from [F1] and $M>0$ from [F2], this gives $M_{\rm ADM}=\sqrt{M^2}=M$. No positive-mass theorem, completeness of the interior slice, or horizon regularity of this slice is needed for this direct end computation. [given, F1, F2, step 1.1] ∎

## External input

The cited Kerr review supplies the coordinate and parameter background stated in its reference record; the result above is derived under the declared hypotheses and dependencies.

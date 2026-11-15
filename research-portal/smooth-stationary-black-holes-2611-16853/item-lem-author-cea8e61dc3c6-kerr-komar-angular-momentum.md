---
title: The Komar angular-momentum flux of the Kerr end
status: published
research_item: lem-author-cea8e61dc3c6-kerr-komar-angular-momentum
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
      reading_limits: Consulted browser-extracted PDF text in section 2 at equations
        (2.1), (2.5)–(2.8) and adjacent discussion on PDF pages 2–3. This is
        coordinate and parameter background only. The exact tensor premise is
        the declared mathematical supplier; the differentiated coefficients and
        normalization-specific flux evaluation are local calculations. No
        full-review reading or source proof reconstruction is claimed.
---

## Prerequisites

- [lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor)
- [def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)
- [lem-author-cea8e61dc3c6-kerr-spatial-end](item-lem-author-cea8e61dc3c6-kerr-spatial-end)
- [physics:def-emg-xs-kn-data](https://alphabetamath.cc/physics/item/def-emg-xs-kn-data)
- [` The Kerr Metric · §2, equations (2.1), (2.5)–(2.8), PDF pp. 2–3 `](https://arxiv.org/pdf/1410.2130)


## Statement

For the axial field $\eta=\partial_\phi$ and the orientations already specified, the Komar angular momentum of the Kerr end exists and equals $J_{\rm K}=Ma$.

## Statement references

[lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor)

[def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)

[lem-author-cea8e61dc3c6-kerr-spatial-end](item-lem-author-cea8e61dc3c6-kerr-spatial-end)

## Facts & Assumptions

[F1] The following exact suppliers supply the geometric objects and earlier conclusions used here: [lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor) [def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions) [lem-author-cea8e61dc3c6-kerr-spatial-end](item-lem-author-cea8e61dc3c6-kerr-spatial-end)

[F2] The exact metric tensor is the Boyer–Lindquist tensor of [physics:def-emg-xs-kn-data](https://alphabetamath.cc/physics/item/def-emg-xs-kn-data), with $q=0$ and $x^0=t$. Apply that definition on the exterior polar patch $r>r_+$, $0<\theta<\pi$; [F1] gives $\Sigma>0$ and $\Delta>0$, so its domain hypotheses hold also when $|a|=M$.

## Proof

**Given:**The exterior metric, differentiated end expansions and Komar/Hodge conventions of [F1].

**Goal:** Evaluate the axial flux including the inverse-metric mixing term.

1.1 Write $b=\sin^2\theta$. Expanding, inverting and radially differentiating the exact tensor in [F2] gives the exterior coefficients used below. Since $\eta^\flat=g_{t\phi}dt+g_{\phi\phi}d\phi$ and the metric has no $r$ or $\theta$ mixed terms, the pulled-back dual on a $t,r$ sphere has coefficient $(\star d\eta^\flat)_{\theta\phi}=-\sqrt{-\det g}\,g^{rr}(g^{tt}\partial_rg_{t\phi}+g^{t\phi}\partial_rg_{\phi\phi})$. The sign follows from $\epsilon_{tr\theta\phi}>0$ and $d\eta^\flat_{tr}=-\partial_rg_{t\phi}$. The exterior coefficients give $g^{tt}=-1+O(r^{-1})$, $g^{t\phi}=-2Ma/r^3+O(r^{-4})$, $g^{rr}=1+O(r^{-1})$, $\partial_rg_{t\phi}=2Ma b/r^2+O(r^{-4})$, $\partial_rg_{\phi\phi}=2rb+O(r^{-2})$, and $\sqrt{-\det g}=\Sigma\sin\theta$. Thus the coefficient is $6Ma\sin^3\theta+O(r^{-1})\sin\theta$, with a bounded smooth angular remainder. [given, F1, F2]

2.1 Both inverse-metric terms contribute: their leading sum before the overall minus sign is $-6Ma b/r^2$, so ignoring the $g^{t\phi}$ term would give an incorrect factor. Since $\int_0^{2\pi}d\phi\int_0^\pi\sin^3\theta\,d\theta=8\pi/3$, the limiting flux is $16\pi Ma$. The Komar normalization therefore gives $J_{\rm K}=Ma$, including negative $a$, zero $a$ and extremal $|a|=M$. [given, F1, step 1.1] ∎

## External input

The cited Kerr coordinate formulas provide background for the local calculation in this item.

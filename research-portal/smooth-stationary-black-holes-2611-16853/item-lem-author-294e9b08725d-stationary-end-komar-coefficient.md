---
title: Komar flux equals the original stationary mass coefficient
status: draft
research_item: lem-author-294e9b08725d-stationary-end-komar-coefficient
dependency_level: 5
sources:
  references: []
---

## Prerequisites

- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [lem-author-294e9b08725d-stationary-end-extrinsic-decay](item-lem-author-294e9b08725d-stationary-end-extrinsic-decay)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)
- [math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

On an original stationary end with $T=\partial_t$, $g_{00}=-1+2M_0/r+O_2(r^{-2})$, $g_{0i}=O_2(r^{-2})$, and $g_{ij}=\delta_{ij}+O_2(r^{-1})$, choose $n$ future with $T=Nn+X$ and $N>0$, and $\nu$ the outward $h$-unit normal to coordinate spheres in $t=0$. With the future/outward Komar mass convention $m_K=(4\pi)^{-1}\lim_{r\to\infty}\int_{S_r}n^a\nu^b\nabla_aT_b\,dA_h$, one has $m_K=M_0$. No sign of $M_0$ or maximality is assumed.

## Statement references

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[lem-author-294e9b08725d-stationary-end-extrinsic-decay](item-lem-author-294e9b08725d-stationary-end-extrinsic-decay)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)

[math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[A1] The original regular-data convention is ZFC, including the axiom of choice. Its restriction to countable families supplies the countable-choice hypothesis of the density-integration definition. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The end coefficients and derivatives have the original stationary bounds. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] The lapse, shift and positive end orientation are as in the stationary extrinsic-decay interface. [lem-author-294e9b08725d-stationary-end-extrinsic-decay](item-lem-author-294e9b08725d-stationary-end-extrinsic-decay) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F3] For the induced positive metric $h|_{TS_r}$ on the compact smooth coordinate sphere $S_r$, $dA_h$ is its Riemannian volume density: in local surface coordinates $u$, $dA_h=\sqrt{\det(h|_{TS_r})_{AB}}\,|du^1du^2|$. The flux is the integral of its smooth scalar integrand times this density; compactness supplies compact support. The same conventions define $d\omega$ for the unit round sphere. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density)

## Proof

**Given:** The data and hypotheses of the Statement, with the density conventions of [F3] and the inherited choice convention [A1].

**Goal:** Evaluate the future/outward flux limit.

1.1 For a Killing field $T=\partial_t$, $\nabla_aT_b=\tfrac12(\partial_a g_{0b}-\partial_b g_{0a})$. Thus $\nabla_0T_i=-\tfrac12\partial_i g_{00}=M_0x_i/r^3+O(r^{-3})$. Here $n^0=1+O(r^{-1})$, $n^i=O(r^{-2})$, $\nu^0=0$, and $\nu^i=x_i/r+O(r^{-1})$. The spatial-spatial Killing derivative is $O(r^{-3})$. Hence $n^a\nu^b\nabla_aT_b=M_0/r^2+O(r^{-3})$. [F1, F2, algebra]

1.2 Write $x=r\omega$ with $|\omega|=1$, and let $\gamma$ be the unit round metric. For tangent vectors $v,w$ at $\omega$, the induced metric in this parametrization is $q_r(v,w)=r^2h_{ij}(r\omega)v^iw^j$. In a $\gamma$-orthonormal tangent frame this is $r^2(I_2+E_r)$, where every entry of $E_r$ is $O(r^{-1})$ uniformly by [F1]. The two-by-two identity $\det(I_2+E_r)=1+\operatorname{tr}E_r+\det E_r=1+O(r^{-1})$ and the positive square root give $dA_h=r^2(1+O(r^{-1}))\,d\omega$ by [F3]. In spherical coordinates the unit round metric has matrix $\operatorname{diag}(1,\sin^2\theta)$, so $d\omega=\sin\theta\,|d\theta d\phi|$ for $0<\theta<\pi$. Integrating gives $\int_{S^2}d\omega=\int_0^{2\pi}\int_0^\pi\sin\theta\,d\theta d\phi=4\pi$; the omitted poles and angular seam have zero two-dimensional coordinate measure, so contribute zero to the smooth-density integral. [F1, F3, A1, algebra]

2.1 The uniform estimate in step 1.1 and the density formula in step 1.2 give $\int_{S_r}n^a\nu^b\nabla_aT_b\,dA_h=\int_{S^2}(M_0+O(r^{-1}))\,d\omega=4\pi M_0+O(r^{-1})$. Thus the limit exists and the stated normalization gives $m_K=M_0$. The future/outward orientation was fixed in the contraction in step 1.1; no positivity of $M_0$ or maximality is used. [step 1.1, step 1.2, F3, A1, algebra] ∎

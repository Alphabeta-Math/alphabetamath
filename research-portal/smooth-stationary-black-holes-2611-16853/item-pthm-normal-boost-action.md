---
title: Normal boost action of the Hawking flow
status: draft
research_item: pthm-normal-boost-action
dependency_level: 11
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 17–18, equations (3.9) and (3.11)
      statement: At the bifurcation surface, the differential of the Hawking flow adds
        kappa times the flow parameter to the normal rapidity; the outward
        normal is the zero-rapidity case.
      hypotheses: The article's standing construction and the normal fields of its
        common reference collar.
      reading_limits: Read the frozen extracted passages around equations (3.9) and
        (3.11). This reference attributes the article claim and is not a premise
        of the proof.
---

PDF p. 17: ` (3.9) `; PDF p. 18: ` (3.11) `

## Prerequisites

- [pthm-common-reference-collar](item-pthm-common-reference-collar)
- [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)
- [pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation)
- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-harrison-normalization](item-def-harrison-normalization)
- [lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors)
- [physics:thm-gr-killing-and-on-shell-matter-identities](https://alphabetamath.cc/physics/item/thm-gr-killing-and-on-shell-matter-identities)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)
- [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)



## Statement

Adopt the stationary vacuum model and regular stationary data, with $T|_S\not\equiv0$, maximal original exterior section and mass normalized to one. Use the common reference collar and its smooth Lorentzian Harrison family $g_q$, $q\in[0,1]$. Here $S$ is the spacelike bifurcation surface, $K$ is the fixed Hawking Killing field, $\phi_s^K$ is its maximal flow, and $\kappa>0$ is its fixed boost rate. On $S$, let $\bar n_q$ be the future unit normal to the reference section and $\bar\nu_q$ the unit normal to $S$ within that section pointing into the exterior. These form an orthonormal basis of the $g_q$-normal plane of $S$, with $\bar n_q$ timelike.

For every $p\in S$, $q\in[0,1]$, and $s,\alpha\in\mathbb R$, the flow fixes $p$ and

$$d\phi_s^K|_p(\cosh\alpha\,\bar\nu_q+\sinh\alpha\,\bar n_q)=\cosh(\alpha+\kappa s)\,\bar\nu_q+\sinh(\alpha+\kappa s)\,\bar n_q.$$

In particular, $d\phi_s^K|_p\bar\nu_q=\cosh(\kappa s)\bar\nu_q+\sinh(\kappa s)\bar n_q$.

The original-section maximality premise is imposed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$ for the original metric $g$, so $H_g|_C=0$. Where this result uses the original reference section $\Sigma_1$, it denotes the closure $B=C\cup S$ of this actual section. Maximality of a separately labelled chart-side region or another supplied section is not substituted for this premise. The spherical identification and the physical stationary end chart remain independent. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-harrison-normalization](item-def-harrison-normalization)

[pthm-common-reference-collar](item-pthm-common-reference-collar)

[pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)

[pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)

## Facts & Assumptions

[A1] Adopt the stated stationary vacuum model, regular data, maximal exterior section and mass-one normalization. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-harrison-normalization](item-def-harrison-normalization)

[F1] The common collar gives the stated normal fields, $K|_S=0$, and $\nabla^{(q)}_{\bar\nu_q}K=\kappa\bar n_q$ on $S$ for the same $\kappa>0$. [pthm-common-reference-collar](item-pthm-common-reference-collar) The local Hawking-field result identifies $K$ and its positive normalization. [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields) The horizon-preservation result supplies $\mathcal L_Kg_q=0$ on a neighborhood of $S$ for every $q\in[0,1]$. [pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation)

[F2] For a Killing field, the metric-compatible connection satisfies $g_q(\nabla^{(q)}_vK,w)+g_q(v,\nabla^{(q)}_wK)=0$. [physics:thm-gr-killing-and-on-shell-matter-identities](https://alphabetamath.cc/physics/item/thm-gr-killing-and-on-shell-matter-identities)

[F3] A local flow follows integral curves, and the maximal integral curve through a point is unique. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point) For a smooth vector field on a smooth manifold $M$, the set of pairs $(t,x)$ for which the maximal integral curve from $x$ is defined at $t$ is open in $\mathbb R\times M$, and evaluation along those curves is the unique smooth maximal local flow. [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)

[F4] If a Killing field vanishes on a spacelike surface and its normal derivative has boost matrix $\kappa\begin{pmatrix}0&1\\1&0\end{pmatrix}$ in a future-timelike and outward-spacelike orthonormal basis, its flow differential has the corresponding hyperbolic boost matrix wherever the flow is defined. [lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors)

## Proof

**Given:** The model, collar, fields and parameter ranges in the Statement.

**Goal:** Prove the displayed normal action and its zero-rapidity specialization.

1.1 Fix $p\in S$ and $q\in[0,1]$, and put $B(v)=\nabla^{(q)}_vK|_p$. Since $K$ vanishes along $S$, $B(X)=0$ for $X\in T_pS$. By the Killing equation, $g_q(Bv,X)=-g_q(v,BX)=0$, so $B$ preserves the normal plane. The collar gives $B\bar\nu_q=\kappa\bar n_q$. Write $B\bar n_q=a\bar n_q+b\bar\nu_q$; skewness gives $a=0$ and $b=\kappa$. Thus $B$ has the matrix required in [F4] in the ordered basis $(\bar n_q,\bar\nu_q)$. [A1, F1, F2]

2.1 The constant curve at $p$ is an integral curve of $K$ on all of $\mathbb R$. By maximality and uniqueness it is the maximal integral curve through $p$, with domain $I_p=\mathbb R$. Apply the maximal-flow theorem in [F3] to the smooth field $K$ on its open neighborhood of $S$: its smooth maximal flow has open domain $\mathcal D=\{(t,x):t\in I_x\}$ and evaluates the maximal integral curves. Thus $(s,p)\in\mathcal D$ and $\phi_s^K(p)=p$ for every real $s$. For each such $s$, openness gives a neighborhood of $p$ on which the time-$s$ map is smooth, so $d\phi_s^K|_p$ exists. Applying [F4] with the matrix from step 1.1 gives $d\phi_s^K\bar\nu_q=\cosh(\kappa s)\bar\nu_q+\sinh(\kappa s)\bar n_q$ and $d\phi_s^K\bar n_q=\sinh(\kappa s)\bar\nu_q+\cosh(\kappa s)\bar n_q$. Linearity and the hyperbolic addition formulas yield the displayed action for every real $\alpha$; setting $\alpha=0$ gives the particular formula. [F1, F3, F4, step 1.1, algebra] ∎

## Source notes

These premises specify the generated conditional scope and are not attributed to the original article. The substantive local horizon conclusions are retained. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

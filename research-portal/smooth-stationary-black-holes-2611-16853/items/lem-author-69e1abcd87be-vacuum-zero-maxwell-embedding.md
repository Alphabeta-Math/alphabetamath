---
id: lem-author-69e1abcd87be-vacuum-zero-maxwell-embedding
title: Vacuum metrics embed as stationary electrovacuum data with zero field
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-source-free-geometric-electrovacuum-data
  - def-stationary-lorentzian-data
  - def-stationary-asymptotic-decay-data
  - math:def-exterior-derivative-by-the-invariant-vector-field-formula
  - math:def-pullback-of-a-differential-form
dependency_roles:
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  math:def-exterior-derivative-by-the-invariant-vector-field-formula: mathematical-premise
  math:def-pullback-of-a-differential-form: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Work in the ZFC convention of the stationary Lorentzian data. Let $(M,g,N,o,T)$ be smooth oriented time-oriented stationary Lorentzian data with $\operatorname{Ric}(g)=0$. Set $F=0$ and $A=0$, the global zero one-form. Then $dA=F$, $dF=d(\star_gF)=0$ and $\operatorname{Ric}_{ab}=2(F_{ac}F_b{}^c-\tfrac14g_{ab}F_{cd}F^{cd})$.

The Maxwell field is invariant under every isometry and satisfies $\mathcal L_TF=0$. Its electric and magnetic fluxes vanish on every compact oriented smooth embedded spacelike two-surface without boundary, with the flux conventions of the geometric electrovacuum data.

If an exterior chart $(t,x)$ with coordinate range $I\times E$, where $I$ is an open interval and $E=\{x\in\mathbb R^3:r=|x|>R_0\}$ with $R_0>0$, is additionally specified, write $A=A_0\,dt+\sum_{i=1}^3A_i\,dx^i$. For every nonnegative integer $m$ and every real $b$, each component is $O_m(r^{-b})$ in the Cartesian spatial derivatives, uniformly for $t\in I$: for all $|\beta|\le m$, $|\partial_x^\beta A_\mu(t,x)|\le 0\,r^{-b-|\beta|}$. For every $0<\alpha<1$, its weighted $C^{m,\alpha}$ bound of decay order $b$ also has bound zero, uniformly in $t$. These are the differentiated and weighted estimates of the asymptotic-decay convention; no existence of an end or such a chart is asserted.

Thus the vacuum datum supplies the vacuum specialization of the electrovacuum framework without adding a physical matter field, and the zero potential satisfies every decay order in the specified differentiated and weighted classes whenever the additional chart is supplied.

## Facts & Assumptions

[F1] The geometric electrovacuum equations, Hodge map and electric and magnetic flux normalizations are explicitly defined. [[def-source-free-geometric-electrovacuum-data]]

[F2] The metric, Ricci convention, chosen time orientation and stationary Killing condition have the fixed smooth Lorentzian meanings. [[def-stationary-lorentzian-data]]

[F3] The differentiated $O_m$ and weighted $C^{m,\alpha}$ bounds use a specified Cartesian exterior chart, spatial multi-indices, annular Hölder seminorms and common constants for a parameter family. [[def-stationary-asymptotic-decay-data]]

[F4] Exterior differentiation is defined by the invariant vector-field formula: its terms are derivatives of evaluations of the form and evaluations of the form on Lie brackets. [[math:def-exterior-derivative-by-the-invariant-vector-field-formula]]

[F5] For a smooth map $h$ and a $k$-form $\omega$, $(h^*\omega)_p(v_1,\ldots,v_k)=\omega_{h(p)}(dh_pv_1,\ldots,dh_pv_k)$. [[math:def-pullback-of-a-differential-form]]

## Proof

**Given:** The data and assumptions in the Statement.

**Goal:** Establish the zero-field embedding, invariance, vanishing fluxes and conditional decay estimates.

1.1 For a zero form, every evaluation in the invariant exterior-derivative formula is the zero scalar function, its derivative by any vector field is zero, and every bracket-evaluation term is zero. Hence $dA=0=F$ and $dF=0$. The Hodge map in [F1] is fiberwise linear, so $\star_gF=0$ and the same derivative calculation gives $d(\star_gF)=0$. [given, F1, F4, algebra]

2.1 All components of $F$ and all their raised components vanish. Both quadratic terms in the electrovacuum Ricci equation are therefore zero, and the hypothesis $\operatorname{Ric}(g)=0$ gives that equation with the metric, orientation and Ricci convention inherited unchanged. Together with step 1.1 this proves that $(M,g,N,o,0)$ is a geometric electrovacuum datum with the global potential $A=0$. [given, F1, F2, step 1.1, algebra]

2.2 The pullback formula in [F5] evaluates a zero form to zero for any smooth map. In particular, every isometry preserves $F=0$, and every local flow map $\Phi_s$ of $T$ has $\Phi_s^*F=0$. Defining $\mathcal L_TF=\frac{d}{ds}|_{s=0}\Phi_s^*F$ gives $\mathcal L_TF=0$, with no completeness requirement on the flow. For the inclusion of any surface in the Statement, the pullbacks of $F$ and $\star_gF$ are zero. Their flux integrals in [F1] are integrals of the zero top form and hence vanish. [F1, F2, F5, step 1.1, algebra]

3.1 In any additional chart specified in the Statement all four coefficient functions $A_\mu$ and every spatial derivative of them are identically zero. The bounds of [F3] therefore hold for every $m$ and $b$ with $C_\beta=0$ and any common $R_1>R_0$, independent of $t$. Every derivative Hölder seminorm is zero, since its numerator is a difference of zero values, so the weighted annular sums are also zero for every $0<\alpha<1$. This proves all the asserted conditional decay orders. Along with steps 2.1 and 2.2, it establishes the zero-field specialization; it makes no existence or classification assertion. [given, F3, step 2.1, step 2.2, algebra] ∎

---
title: Killing flow preserves its complex two-form
status: published
research_item: lem-author-cea8e61dc3c6-killing-flow-invariance
dependency_level: 2
sources:
  references: []
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [lem-author-cea8e61dc3c6-killing-exact-two-form](item-lem-author-cea8e61dc3c6-killing-exact-two-form)
- [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)
- [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)
- [math:thm-the-exterior-derivative-commutes-with-pullback](https://alphabetamath.cc/item/thm-the-exterior-derivative-commutes-with-pullback)
- [math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges](https://alphabetamath.cc/item/prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges)


## Statement

For stationary Lorentzian data, let $F=\tfrac12dT^\flat$ and $\mathcal F=F+i\star_gF$. Then $\mathcal L_TF=0$ and $\mathcal L_T\mathcal F=0$. These assertions use only local flow maps and do not require a complete flow.

## Facts & Assumptions

[F1] The Killing field and local flow are defined by [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] The complex two-form and complex-linear Hodge convention are those of [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data).

[F3] The Killing derivative equals $\tfrac12dT^\flat$. [lem-author-cea8e61dc3c6-killing-exact-two-form](item-lem-author-cea8e61dc3c6-killing-exact-two-form)

[F4] The Hodge star is uniquely characterized by the wedge pairing and oriented metric volume. [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[F5] A local flow satisfies $\Phi_0=\operatorname{id}$ and $\Phi_t\circ\Phi_s=\Phi_{t+s}$ wherever defined, and its time curves have velocity $T$. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F6] For a real covariant tensor $A$, $\mathcal L_TA=\left.\frac{d}{dt}\right|_{t=0}\Phi_t^*A$. For a complex two-form $U+iV$, define pullback and Lie derivative componentwise: $\Phi_t^*(U+iV)=\Phi_t^*U+i\Phi_t^*V$ and $\mathcal L_T(U+iV)=\mathcal L_TU+i\mathcal L_TV$. The unique real and imaginary parts make these extensions well-defined. [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field) [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[F7] On common local flow domains a smooth real tensor is invariant under the flow exactly when its Lie derivative vanishes. [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)

[F8] Exterior differentiation commutes with pullback by every smooth map, in particular by each local flow map. [math:thm-the-exterior-derivative-commutes-with-pullback](https://alphabetamath.cc/item/thm-the-exterior-derivative-commutes-with-pullback)

[F9] Pullback of forms is smooth, functorial and wedge-preserving. [math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges](https://alphabetamath.cc/item/prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove both Lie derivative identities on local flow domains.

1.1 Work on a sufficiently short common local flow domain. The composition law gives $\Phi_{-t}\circ\Phi_t=\operatorname{id}$ and $\Phi_t\circ\Phi_{-t}=\operatorname{id}$ after restriction, so these smooth maps are local diffeomorphisms. Since $\mathcal L_Tg=0$, tensor-flow invariance gives $\Phi_t^*g=g$. Differentiating $\Phi_t(\Phi_s(p))=\Phi_s(\Phi_t(p))$ at $s=0$ gives $d\Phi_t|_p(T_p)=T_{\Phi_t(p)}$. The differential has nonzero determinant and varies continuously from the identity, so these local flow maps preserve orientation. [F1, F5, F7]

2.1 For $v\in T_pM$, step 1.1 gives $(\Phi_t^*T^\flat)_p(v)=g_{\Phi_t(p)}(T_{\Phi_t(p)},d\Phi_t|_p v)=g_p(T_p,v)$. Thus $\Phi_t^*T^\flat=T^\flat$. By naturality of exterior differentiation, $\Phi_t^*F=\tfrac12\Phi_t^*dT^\flat=\tfrac12d(\Phi_t^*T^\flat)=F$, with the same $F$ as the Killing derivative. [step 1.1, F1, F3, F8, algebra]

2.2 An orientation-preserving local isometry preserves the inverse metric pairing on covectors, hence its determinant pairing on exterior powers. It also preserves oriented metric volume: it takes every positive orthonormal frame to a positive orthonormal frame, on which both volume forms have value one. Pull back $\alpha\wedge\star_g\beta=\langle\alpha,\beta\rangle_g\operatorname{vol}_g$. Wedge preservation and these metric identities give $(\Phi_t^*\alpha)\wedge\Phi_t^*(\star_g\beta)=\langle\Phi_t^*\alpha,\Phi_t^*\beta\rangle_g\operatorname{vol}_g$. Since the local diffeomorphism induces an isomorphism on each exterior-power fibre, its pulled-back $\alpha$ range over all forms at each point. Uniqueness in the Hodge characterization therefore gives $\Phi_t^*(\star_g\beta)=\star_g(\Phi_t^*\beta)$. [step 1.1, F4, F9, algebra]

3.1 Apply step 2.2 to $\beta=F$. Step 2.1 and the componentwise complex extension give $\Phi_t^*\mathcal F=\Phi_t^*F+i\Phi_t^*(\star_gF)=F+i\star_gF=\mathcal F$. Differentiating this identity and $\Phi_t^*F=F$ at $t=0$ gives $\mathcal L_T\mathcal F=0$ and $\mathcal L_TF=0$ by the tensor Lie derivative definition and its complex-linear extension. All maps used were local, so no completeness of the flow is assumed. [step 2.1, step 2.2, F2, F6, algebra] ∎

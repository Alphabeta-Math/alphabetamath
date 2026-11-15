---
title: Closed Ernst contraction and the real potential
status: draft
research_item: lem-author-cea8e61dc3c6-closed-ernst-contraction
dependency_level: 3
sources:
  references: []
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [lem-author-cea8e61dc3c6-killing-exact-two-form](item-lem-author-cea8e61dc3c6-killing-exact-two-form)
- [lem-author-cea8e61dc3c6-vacuum-killing-divergence](item-lem-author-cea8e61dc3c6-vacuum-killing-divergence)
- [lem-author-cea8e61dc3c6-divergence-hodge-closure](item-lem-author-cea8e61dc3c6-divergence-hodge-closure)
- [lem-author-cea8e61dc3c6-killing-flow-invariance](item-lem-author-cea8e61dc3c6-killing-flow-invariance)
- [math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula)
- [math:thm-poincare-lemma-for-star-shaped-domains](https://alphabetamath.cc/item/thm-poincare-lemma-for-star-shaped-domains)
- [math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula)
- [math:prop-exterior-derivative-of-a-function-is-its-differential](https://alphabetamath.cc/item/prop-exterior-derivative-of-a-function-is-its-differential)


## Statement

For Ricci-flat stationary Lorentzian data, put $F_{ab}=\nabla_aT_b$, $\mathcal F=F+i\star_gF$, and $\eta=2\iota_T\mathcal F$, where $(\iota_T\mathcal F)_b=T^a\mathcal F_{ab}$. Then $d\eta=0$ and $\operatorname{Re}\eta=d(-g(T,T))$. There are smooth complex potentials locally. On an open set where $\eta=d\sigma$, $\operatorname{Re}\sigma=-g(T,T)$ up to one real constant on each connected component.

## Facts & Assumptions

[F1] The fields, metric connection, and scalar $f=-g(T,T)$ are defined in [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] Use $\mathcal F=F+i\star_gF$ with complex-linear Hodge star. [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[F3] The real Killing two-form satisfies $dF=0$. [lem-author-cea8e61dc3c6-killing-exact-two-form](item-lem-author-cea8e61dc3c6-killing-exact-two-form)

[F4] Ricci flatness implies $\nabla^aF_{ab}=0$. [lem-author-cea8e61dc3c6-vacuum-killing-divergence](item-lem-author-cea8e61dc3c6-vacuum-killing-divergence)

[F5] Vanishing divergence of a two-form implies closedness of its Hodge dual. [lem-author-cea8e61dc3c6-divergence-hodge-closure](item-lem-author-cea8e61dc3c6-divergence-hodge-closure)

[F6] The complex Killing two-form satisfies $\mathcal L_T\mathcal F=0$. [lem-author-cea8e61dc3c6-killing-flow-invariance](item-lem-author-cea8e61dc3c6-killing-flow-invariance)

[F7] The Cartan identity is $\mathcal L_T\omega=d\iota_T\omega+\iota_Td\omega$, and is extended complex linearly. [math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula)

[F8] Every closed smooth real one-form on a star-shaped coordinate domain has a potential by the Poincare lemma. [math:thm-poincare-lemma-for-star-shaped-domains](https://alphabetamath.cc/item/thm-poincare-lemma-for-star-shaped-domains)

[F9] Use real exterior differentiation defined by the invariant vector-field formula. For a complex form written in its unique real and imaginary parts as $U+iV$, define $d(U+iV)=dU+i\,dV$ and $\iota_T(U+iV)=\iota_TU+i\iota_TV$, including degree zero for $d$. These are componentwise extensions, with $T$ real. [math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula)

[F10] On a smooth real function $h$, exterior differentiation is the ordinary differential: $dh(X)=Xh$. [math:prop-exterior-derivative-of-a-function-is-its-differential](https://alphabetamath.cc/item/prop-exterior-derivative-of-a-function-is-its-differential)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove all asserted identities under these hypotheses.

1.1 Each term in the invariant formula [F9] is real-linear in the form, so $d(aU+bV)=a\,dU+b\,dV$ for real constants $a,b$. Consequently the componentwise extension in [F9] is complex-linear and commutes with taking real and imaginary parts. Applying the real Cartan identity separately to those parts gives [F7] for complex forms. By [F3]–[F5], $d\mathcal F=dF+i\,d\star_gF=0$. Applying [F7] and then [F6] gives $d\eta=2(\mathcal L_T\mathcal F-\iota_Td\mathcal F)=0$. By [F10], metric compatibility and the antisymmetry of $F$ give $(df)_b=-2T^a\nabla_bT_a=2T^aF_{ab}=\operatorname{Re}\eta_b$. [F1, F2, F3, F4, F5, F6, F7, F9, F10, algebra]

2.1 Restrict to a coordinate ball; its image is star-shaped. By step 1.1, both real and imaginary parts of $\eta$ are closed smooth real one-forms. Evaluating the invariant formula [F9] on commuting coordinate vector fields identifies closedness of either real one-form with $\partial_jA_k=\partial_kA_j$ for its real coefficient field $A$. Thus their coefficient fields meet the closed $C^1$ hypotheses of [F8], which supplies real potentials whose complex combination is a local $\sigma$. Their first partial derivatives are smooth components of $\eta$, so these potentials are smooth. Wherever a global primitive is assumed, step 1.1 and [F9]–[F10] give $d(\operatorname{Re}\sigma-f)=0$. This difference is constant on each coordinate ball by integrating its zero derivative along segments, and hence locally constant. On each connected component it is constant, since every nonempty fiber of a locally constant function is open and closed. No assertion that all periods vanish is used. [step 1.1, F1, F8, F9, F10, algebra] ∎

---
title: Rank-one tangent changes, signature and Hodge transfer
status: draft
research_item: lem-rank-one-lorentzian-hodge-transfer
dependency_level: 1
sources:
  references: []
---

## Prerequisites

- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [math:lem-determinant-rank-one-update-over-a-commutative-ring](https://alphabetamath.cc/item/lem-determinant-rank-one-update-over-a-commutative-ring)
- [math:thm-sylvesters-law-of-inertia](https://alphabetamath.cc/item/thm-sylvesters-law-of-inertia)
- [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)
- [physics:lem-emg-conformal-hodge-multiplier](https://alphabetamath.cc/physics/item/lem-emg-conformal-hodge-multiplier)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-orientation-of-a-finite-dimensional-real-vector-space](https://alphabetamath.cc/item/def-orientation-of-a-finite-dimensional-real-vector-space)
- [math:thm-determinant-sign-detects-orientation-change](https://alphabetamath.cc/item/thm-determinant-sign-detects-orientation-change)
- [math:prop-linear-pullback-respects-tensor-products-and-permutations](https://alphabetamath.cc/item/prop-linear-pullback-respects-tensor-products-and-permutations)
- [math:def-wedge-product-of-alternating-covectors](https://alphabetamath.cc/item/def-wedge-product-of-alternating-covectors)


## Statement

Let $V$ be an oriented four-dimensional real vector space with a Lorentz form $g$ of signature $(-,+,+,+)$, meaning a nondegenerate symmetric bilinear form with one negative and three positive directions. Let $T\in V$, $W\in V^*$, and $D,d>0$ satisfy $W(T)=d-D$. Define $A=I+D^{-1}T\otimes W$, where $(T\otimes W)(v)=W(v)T$, and $g'=(D/4)A^*g$, where $(A^*g)(u,v)=g(Au,Av)$. Give the domain of $A$ the transported orientation: a basis is positive exactly when its image under $A$ is positive.

Then $\det A=d/D$, $A^{-1}=I-d^{-1}T\otimes W$, and $g'$ has the same inertia as $g$. For every real or complex two-form $F$, with $(A^*F)(u,v)=F(Au,Av)$, the corresponding metric Hodge stars satisfy $\star_{g'}(A^*F)=A^*(\star_gF)$. For any two such forms $F,H$, their full complex-bilinear contractions satisfy $(A^*F)_{ab}(A^*H)^{ab}_{g'}=(4/D)^2F_{ab}H^{ab}_g$, where both indices are raised with the indicated inverse metric and no complex conjugation or factor of one half is used.

## Statement references

[math:def-orientation-of-a-finite-dimensional-real-vector-space](https://alphabetamath.cc/item/def-orientation-of-a-finite-dimensional-real-vector-space)

[def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[math:lem-determinant-rank-one-update-over-a-commutative-ring](https://alphabetamath.cc/item/lem-determinant-rank-one-update-over-a-commutative-ring)

[math:thm-sylvesters-law-of-inertia](https://alphabetamath.cc/item/thm-sylvesters-law-of-inertia)

[physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[physics:lem-emg-conformal-hodge-multiplier](https://alphabetamath.cc/physics/item/lem-emg-conformal-hodge-multiplier)

## Facts & Assumptions

**Given:** The oriented Lorentz space, $T$, $W$, $D$ and $d$ in the statement.

**Goal:** Establish the determinant, inverse, inertia, Hodge transfer and contraction formulas in the statement.

[A1] Work in the ZFC background, including the choice assumptions inherited by the geometric suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The rank-one determinant identity gives $\det(B+uv^{\mathsf T})=\det B+v^{\mathsf T}\operatorname{adj}(B)u$ over a commutative ring. [math:lem-determinant-rank-one-update-over-a-commutative-ring](https://alphabetamath.cc/item/lem-determinant-rank-one-update-over-a-commutative-ring)

[F2] A real symmetric form has basis-independent inertia under congruence. [math:thm-sylvesters-law-of-inertia](https://alphabetamath.cc/item/thm-sylvesters-law-of-inertia)

[F3] Algebraic pullback composes each covariant slot with the given linear map; inverse metrics raise indices, and the full two-form contraction is complex bilinear. [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[F4] The metric Hodge star is uniquely characterized by $\alpha\wedge\star_g\beta=\langle\alpha,\beta\rangle_g\operatorname{vol}_g$, with the exterior pairing induced by the inverse metric and the metric volume determined by the orientation. [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[F5] In four dimensions a positive conformal rescaling leaves the Hodge star on two-forms unchanged. [physics:lem-emg-conformal-hodge-multiplier](https://alphabetamath.cc/physics/item/lem-emg-conformal-hodge-multiplier)

[F6] An orientation of a finite-dimensional real vector space is an equivalence class of ordered bases, where two bases are equivalent when their change-of-basis isomorphism has positive determinant. [math:def-orientation-of-a-finite-dimensional-real-vector-space](https://alphabetamath.cc/item/def-orientation-of-a-finite-dimensional-real-vector-space)

[F7] A linear isomorphism of an oriented real vector space of positive dimension preserves its orientation exactly when its determinant is positive. [math:thm-determinant-sign-detects-orientation-change](https://alphabetamath.cc/item/thm-determinant-sign-detects-orientation-change)

[F8] Linear pullback respects tensor products and permutations of covariant slots. [math:prop-linear-pullback-respects-tensor-products-and-permutations](https://alphabetamath.cc/item/prop-linear-pullback-respects-tensor-products-and-permutations)

[F9] The wedge product of a $k$-covector and an $\ell$-covector is $(k+\ell)!/(k!\ell!)$ times the alternation of their tensor product. [math:def-wedge-product-of-alternating-covectors](https://alphabetamath.cc/item/def-wedge-product-of-alternating-covectors)

## Proof

1.1 Put $K=T\otimes W$. For every $v\in V$, $K^2v=W(v)W(T)T=(d-D)Kv$. Thus $(I+D^{-1}K)(I-d^{-1}K)=I+(D^{-1}-d^{-1}-(d-D)/(Dd))K=I$, and the same calculation in the opposite order gives $A^{-1}=I-d^{-1}K$. In any basis, [F1] with $B=I$, $u=D^{-1}T$ and $v^{\mathsf T}=W$ gives $\det A=1+D^{-1}W(T)=d/D>0$. [given, F1, algebra]

2.1 Since $A$ is invertible and $D/4>0$, a basis in which $g$ is diagonal with one negative and three positive entries pulls back by $A^{-1}$ to a basis in which $g'$ has those entries multiplied by $D/4$. Hence $g'$ has the same inertia as $g$, independently of basis by [F2]. By [F7], $A$ preserves the original orientation because $\dim V=4$ and $\det A>0$. Hence the transported positive-basis class in the sense of [F6] agrees with the original orientation on $V$. [step 1.1, F2, F6, F7, algebra]

3.1 Write $h=A^*g$. The map $A$ is an orientation-preserving isometry from $(V,h)$ with transported orientation to $(V,g)$. For two-forms $\alpha,\beta$, the induced inverse-metric pairing satisfies $\langle A^*\alpha,A^*\beta\rangle_h=\langle\alpha,\beta\rangle_g$: in a basis this follows by substituting $h^{-1}=A^{-1}g^{-1}A^{-\mathsf T}$ into the two raised slots. Also $\operatorname{vol}_h=A^*\operatorname{vol}_g$, as both sides take value $1$ on a transported positively oriented $h$-orthonormal basis. By [F8] and [F9], slotwise pullback commutes with the normalized alternating sum defining the wedge: it is linear, respects tensor products and commutes with every permutation of the slots. Thus $A^*(\alpha\wedge\gamma)=(A^*\alpha)\wedge(A^*\gamma)$ for alternating covectors $\alpha,\gamma$. Pulling back the identity in [F4] therefore gives $(A^*\alpha)\wedge A^*(\star_g\beta)=\langle A^*\alpha,A^*\beta\rangle_h\operatorname{vol}_h$. Since every two-form is an $A^*\alpha$, uniqueness in [F4] yields $\star_h(A^*\beta)=A^*(\star_g\beta)$. [step 1.1, step 2.1, F3, F4, F8, F9, algebra]

4.1 Regard $V$ as an affine manifold with constant metric $h$, a constant time orientation and the transported orientation. Applying [F5] to the constant positive factor $D/4$ gives $\star_{g'}=\star_h$ on two-forms, so step 3.1 proves the Hodge transfer. Moreover $g'^{-1}=(4/D)h^{-1}$, and the full contraction uses two inverse-metric factors. The pairing calculation in step 3.1, with the factor of two converting the exterior pairing to the full two-form contraction, therefore gives $(A^*F)_{ab}(A^*H)^{ab}_{g'}=(4/D)^2F_{ab}H^{ab}_g$. Real linearity extends both identities to complex forms by complex bilinearity. [step 3.1, F3, F4, F5, A1, algebra] ∎

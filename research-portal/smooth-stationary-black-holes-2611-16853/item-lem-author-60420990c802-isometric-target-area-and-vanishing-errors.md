---
title: Isometric target areas remain fixed while collar errors vanish
status: published
research_item: lem-author-60420990c802-isometric-target-area-and-vanishing-errors
dependency_level: 0
---

## Prerequisites

- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)
- [math:def-smooth-tensor-field](https://alphabetamath.cc/item/def-smooth-tensor-field)
- [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)
- [math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-immersion-and-embedding-for-manifolds-with-boundary)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)
- [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)
- [math:prop-pullback-of-covariant-tensors-is-smooth-and-functorial](https://alphabetamath.cc/item/prop-pullback-of-covariant-tensors-is-smooth-and-functorial)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)
- [math:prop-density-pullback-under-local-diffeomorphisms](https://alphabetamath.cc/item/prop-density-pullback-under-local-diffeomorphisms)
- [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation)


## Statement

Assume countable choice $\mathrm{AC}_\omega$. Let $M$ be a smooth manifold and $g$ a smooth symmetric covariant two-tensor that is nondegenerate at every point; its signature is arbitrary. Let $C\subset M$ be a compact smooth embedded two-dimensional manifold, with boundary allowed, whose inclusion $i$ induces a positive-definite metric $h=i^*g$. This positivity is the meaning of spacelike here. For each defined parameter $t$, let $\Phi_t:U_t\to V_t$ be a diffeomorphism between open subsets of $M$, with $C\subset U_t$, satisfying $\Phi_t^*(g|_{V_t})=g|_{U_t}$; this is the ambient isometry condition. For a compact spacelike embedded surface $D$ with inclusion $j_D$, define $|D|_g=\int_D\mu_{j_D^*g}$ using its Riemannian density. Then $\Phi_t(C)$ is again such a surface and $|\Phi_t(C)|_g=|C|_g$ for every defined $t$.

Suppose fixed finite numbers $A,B,L\ge0$, with $B=|C|_g$, have the following property: for every $\epsilon>0$ and $\delta>0$ there exists an admissible $0<\eta<\delta$ with a defined translating time $t(\eta)$ such that $A\le|\Phi_{t(\eta)}(C)|_g+\epsilon+L\eta$. The admissible values of $\eta$ may depend on $\epsilon$, while $L$ is fixed. Then $A\le B$. No convergence of the translating times is needed.

## Facts & Assumptions

[A1] Countable choice $\mathrm{AC}_\omega$ is assumed and supplies the stated hypothesis of orientation-free density integration. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F1] Smooth manifolds and smooth tensor fields give the ambient objects. Tensor pullback inserts the differential in each slot; it is smooth and satisfies $(G\circ F)^*T=F^*(G^*T)$. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:def-smooth-tensor-field](https://alphabetamath.cc/item/def-smooth-tensor-field) [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field) [math:prop-pullback-of-covariant-tensors-is-smooth-and-functorial](https://alphabetamath.cc/item/prop-pullback-of-covariant-tensors-is-smooth-and-functorial)

[F2] An embedded surface, including one with boundary, has a smooth inclusion that is an injective immersion and a homeomorphism onto its image. A diffeomorphism has a smooth inverse. The chain rule gives $d(G\circ F)=dG\circ dF$; in boundary charts it follows from the same rule for smooth local extensions. [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary) [math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-immersion-and-embedding-for-manifolds-with-boundary) [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds) [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[F3] A smooth symmetric positive-definite covariant two-tensor is a Riemannian metric. Its density in coordinates is $\mu_h=\sqrt{\det H}\,|dx^1dx^2|$, where $H$ is its coordinate matrix; boundary charts are allowed. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)

[F4] Density pullback by a diffeomorphism uses the absolute Jacobian determinant. Under countable choice, compactly supported smooth density integration is defined, finite, and invariant under diffeomorphisms, including on manifolds with boundary and without an orientation. [math:prop-density-pullback-under-local-diffeomorphisms](https://alphabetamath.cc/item/prop-density-pullback-under-local-diffeomorphisms) [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation)

## Proof

**Given:** The hypotheses in the Statement, including [A1].

**Goal:** Prove isometric area preservation and the vanishing-error conclusion.

1.1 Fix a defined $t$ and set $C_t=\Phi_t(C)$ and $f_t=\Phi_t|_C:C\to C_t$. Transport every chart $x$ of $C$ to $x\circ f_t^{-1}$ on $C_t$. The transition maps are those of $C$, and the image has the subspace topology because $\Phi_t$ is an ambient homeomorphism. Its inclusion $j_t:C_t\hookrightarrow M$ is smooth since $j_t\circ f_t=\Phi_t\circ i$. The differential of the right side is injective: $di$ is injective and $d\Phi_t$ has inverse $d\Phi_t^{-1}$ by the chain rule. Thus $C_t$ is smoothly embedded and $f_t$ is a diffeomorphism, also at boundary points. An open cover of $C_t$ pulls back to an open cover of compact $C$, and a finite subcover pushes forward, so $C_t$ is compact. [given, F1, F2]

2.1 The induced tensor $h_t=j_t^*g$ is smooth and symmetric. Pullback functoriality and the isometry condition give $f_t^*h_t=i^*\Phi_t^*g=i^*g=h$. Since $df_t$ is invertible and $h$ is positive definite, $h_t$ is positive definite too. In a chart $x$ of $C$ and the transported chart $y=x\circ f_t^{-1}$ of $C_t$, the metric matrices coincide and $y\circ f_t=x$ has identity Jacobian. The density formula and its absolute-Jacobian pullback law therefore give $f_t^*\mu_{h_t}=\mu_h$. The same coefficient calculation uses smooth extensions in boundary charts. [given, F1, F3, F4, step 1.1]

3.1 These smooth densities have compact support on the compact surfaces. Under [A1], diffeomorphism invariance of density integration gives $|C_t|_g=\int_{C_t}\mu_{h_t}=\int_C f_t^*\mu_{h_t}=\int_C\mu_h=|C|_g$. The absolute-Jacobian law imposes no orientation condition. This holds for each defined $t$ separately. [A1, F3, F4, step 1.1, step 2.1]

4.1 Substitute step 3.1 into each assumed inequality, giving $A\le B+\epsilon+L\eta$ for the admissible pair. If $d=A-B>0$, choose $\epsilon=d/4$ and $\delta=d/(4(L+1))$. The hypothesis then gives $0<\eta<\delta$, so $\epsilon+L\eta<d/2<d$, contradicting $d\le\epsilon+L\eta$. Thus $A\le B$. This uses the assumed fixed $L$ and allows the admissible $\eta$ to depend on $\epsilon$; there is no fixed-$\eta$ limit. The translating times disappear by exact area preservation, so their convergence is unnecessary. [given, step 3.1] ∎

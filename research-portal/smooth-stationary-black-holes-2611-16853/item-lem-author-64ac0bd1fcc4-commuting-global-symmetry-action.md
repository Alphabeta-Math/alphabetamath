---
title: Commuting complete flows give the global product action
status: published
research_item: lem-author-64ac0bd1fcc4-commuting-global-symmetry-action
dependency_level: 6
---

## Prerequisites

- [def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data](item-def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data)
- [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:def-lie-group](https://alphabetamath.cc/item/def-lie-group)
- [math:thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group](https://alphabetamath.cc/item/thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group)
- [math:thm-quotient-manifold-by-a-closed-lie-subgroup](https://alphabetamath.cc/item/thm-quotient-manifold-by-a-closed-lie-subgroup)
- [math:thm-constant-rank-theorem-for-manifolds](https://alphabetamath.cc/item/thm-constant-rank-theorem-for-manifolds)
- [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)
- [math:prop-a-map-into-a-product-is-smooth-iff-its-components-are-smooth](https://alphabetamath.cc/item/prop-a-map-into-a-product-is-smooth-iff-its-components-are-smooth)
- [math:prop-identity-maps-and-composites-of-smooth-maps-are-smooth](https://alphabetamath.cc/item/prop-identity-maps-and-composites-of-smooth-maps-are-smooth)
- [math:def-smooth-left-action-of-a-lie-group](https://alphabetamath.cc/item/def-smooth-left-action-of-a-lie-group)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)


## Statement

For the supplied global flows, the map $\alpha((t,[s]),p)=\phi_t(\psi_s(p))$ defines a smooth isometric action of $\mathbb R\times(\mathbb R/2\pi\mathbb Z)$. Here $[s]$ denotes the class of $s$ modulo $2\pi$. This uses the supplied global action convention; it asserts no extension of a locally defined symmetry.

## Statement references

[def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data](item-def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data)

[def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[math:def-lie-group](https://alphabetamath.cc/item/def-lie-group)

[math:thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group](https://alphabetamath.cc/item/thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group)

[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[math:def-smooth-left-action-of-a-lie-group](https://alphabetamath.cc/item/def-smooth-left-action-of-a-lie-group)

## Facts & Assumptions

[F1] Work in the ZFC convention of the global comparison data. Both supplied flows are global isometries, the axial flow is $2\pi$-periodic, and the flows commute. The circle-action convention fixes that period. [def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data](item-def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data) [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[F2] A global flow is jointly smooth in parameter and point, has value the identity at parameter zero, and satisfies the flow law for all real parameters. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F3] Smooth multiplication and inversion define a finite-dimensional real Lie group. Under countable choice, the quotient by a closed normal subgroup is a Lie group; the quotient-manifold theorem makes its projection a smooth surjective submersion. The constant-rank theorem gives local projection coordinates for a submersion. [math:def-lie-group](https://alphabetamath.cc/item/def-lie-group) [math:thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group](https://alphabetamath.cc/item/thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group) [math:thm-quotient-manifold-by-a-closed-lie-subgroup](https://alphabetamath.cc/item/thm-quotient-manifold-by-a-closed-lie-subgroup) [math:thm-constant-rank-theorem-for-manifolds](https://alphabetamath.cc/item/thm-constant-rank-theorem-for-manifolds)

[F4] Products carry their canonical product smooth structures. Maps into a product are smooth exactly when their components are smooth, and composites of smooth maps are smooth. [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure) [math:prop-a-map-into-a-product-is-smooth-iff-its-components-are-smooth](https://alphabetamath.cc/item/prop-a-map-into-a-product-is-smooth-iff-its-components-are-smooth) [math:prop-identity-maps-and-composites-of-smooth-maps-are-smooth](https://alphabetamath.cc/item/prop-identity-maps-and-composites-of-smooth-maps-are-smooth)

[F5] A smooth left action is a jointly smooth map satisfying the identity and action laws. [math:def-smooth-left-action-of-a-lie-group](https://alphabetamath.cc/item/def-smooth-left-action-of-a-lie-group)

[F6] Full choice implies countable choice, so the quotient theorems' choice hypothesis is available in the inherited ZFC convention. [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

## Proof

**Given:** The supplied global commuting isometric flows with their inherited ZFC convention.

**Goal:** Verify the smooth product-group action, including joint smoothness on the quotient parameters.

1.1 The usual smooth real line is a Lie group under addition: addition and negation have polynomial coordinate formulas. Put $\Lambda=2\pi\mathbb Z$. This is a subgroup, and it is normal because addition is abelian. It is closed: for $x\notin\Lambda$, choose a bounded open interval about $x$. Only finitely many integer multiples of the positive number $2\pi$ lie in that interval, and a smaller interval about $x$ avoids those finitely many points. Thus the complement of $\Lambda$ is open. Countable choice follows from the supplied ZFC convention. [F1, F3, F6]

2.1 Apply the quotient theorems to obtain the quotient Lie group $C=\mathbb R/\Lambda$, with addition $[s]+[v]=[s+v]$, and the smooth surjective submersion $q:\mathbb R\to C$. Near each $c\in C$, the constant-rank coordinates express $q$ as a projection; fixing the discarded coordinates gives a smooth section $\sigma:U\to\mathbb R$ with $q\circ\sigma=\mathrm{id}_U$. Give $G=\mathbb R\times C$ the product smooth structure and componentwise addition. Its multiplication and inversion are smooth by the component and composition rules, so it is a Lie group with identity $(0,[0])$. [F3, F4, step 1.1]

3.1 Periodicity gives $\psi_{s+2\pi n}=\psi_s$ for every integer $n$, so the formula for $\alpha$ is independent of the representative of $[s]$. On $\mathbb R\times U\times M$, using a section from step 2.1, it is $\alpha((t,c),p)=\phi_t(\psi_{\sigma(c)}(p))$. The two flows are jointly smooth, and the component and composition rules make this local expression jointly smooth in all three variables. Such neighborhoods cover $G\times M$, proving joint smoothness of $\alpha$. [F1, F2, F4, step 2.1]

4.1 The zero-parameter flow identities give $\alpha((0,[0]),p)=p$. For $a=(t,[s])$ and $b=(u,[v])$, commutation and the flow laws give $\phi_t\psi_s\phi_u\psi_v=\phi_{t+u}\psi_{s+v}$, hence $\alpha(a,\alpha(b,p))=\alpha(a+b,p)$ for every $p$. Together with joint smoothness, these are precisely the smooth left-action axioms. Each action map is an isometry: applying the metric-preservation identity successively to the differentials of $\psi_s$ and $\phi_t$ preserves $g$ under their composite. Thus the claimed global smooth isometric action is obtained from the supplied global flows. [F1, F2, F5, step 2.1, step 3.1] ∎

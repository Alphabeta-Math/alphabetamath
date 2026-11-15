---
title: Tangential area Jacobian on a measurable surface domain
status: draft
research_item: def-author-0336834a2590-surface-map-jacobian
dependency_level: 1
---

## Prerequisites

- [def-author-0336834a2590-measurable-surface-domains](item-def-author-0336834a2590-measurable-surface-domains)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:thm-lebesgue-density-theorem](https://alphabetamath.cc/item/thm-lebesgue-density-theorem)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-c-r-and-smooth-maps-between-smooth-manifolds](https://alphabetamath.cc/item/def-c-r-and-smooth-maps-between-smooth-manifolds)
- [math:def-total-derivative-in-euclidean-space](https://alphabetamath.cc/item/def-total-derivative-in-euclidean-space)
- [math:thm-continuous-partial-derivatives-imply-total-differentiability](https://alphabetamath.cc/item/thm-continuous-partial-derivatives-imply-total-differentiability)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:thm-coordinate-derivations-form-a-basis-of-the-tangent-space](https://alphabetamath.cc/item/thm-coordinate-derivations-form-a-basis-of-the-tangent-space)
- [math:thm-change-of-coordinate-formula-for-tangent-bases](https://alphabetamath.cc/item/thm-change-of-coordinate-formula-for-tangent-bases)


## Definition

Work in ZFC. Let $A\subset(C,h)$ be a Borel surface domain on a smooth Hausdorff second-countable Riemannian surface, and let $(\Sigma,k)$ be a finite-dimensional smooth Hausdorff second-countable Riemannian manifold. The target dimension may be arbitrary; the endpoint applications use dimension three. Let $F:A\to\Sigma$ be a map. Require a countable open cover $(U_n)_{n\ge1}$ of $A$ in $C$ and $C^1$ maps $\widetilde F_n:U_n\to\Sigma$ whose restrictions to $A\cap U_n$ equal $F$. Use the disjoint Borel partition $P_n=(A\cap U_n)\setminus\bigcup_{j<n}U_j$.

For a $C^1$ map $G$ on an open subset of $C$, define $dG_p:T_pC\to T_{G(p)}\Sigma$ as follows. In smooth source and target coordinates $x,y$ about $p,G(p)$, its matrix in the coordinate tangent bases is the Euclidean total derivative $D(y\circ G\circ x^{-1})(x(p))$. Thus a tangent vector with $x$-components $v$ is sent to the tangent vector with $y$-components $D(y\circ G\circ x^{-1})(x(p))v$. This definition uses $C^1$ coordinate representatives, not a pullback operation on smooth germs by a possibly nonsmooth map.

Fix a countable smooth atlas of $C$. For $p\in P_n$ having density one for $P_n$ in every atlas chart containing $p$, put $d_AF_p=d\widetilde F_{n,p}$ and $J_2F(p)=\sqrt{\det(k_{F(p)}(d_AF_p(e_i),d_AF_p(e_j)))_{i,j=1}^2}$, where $(e_1,e_2)$ is an $h_p$-orthonormal basis of $T_pC$. On the area-null exceptional set, assign arbitrary finite nonnegative Jacobian values, for example zero. Density one means that the ratio of the Euclidean area of the coordinate image of the intersection of $P_n$ with the chart domain in a ball centered at the point to the area of that ball tends to one as its radius tends to zero. The Gram determinant permits rank loss and vanishes for rank below two; no tangent plane to the image cut is required.

## Facts & Assumptions

**Given:** The objects and extension cover in the Definition.

[A1] Work in ZFC as in the surface-domain convention. Only countable choice is needed here, for countable chart selections and the density theorem. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Borel surface domains and their completed area measure $\mu_C$ have the conventions of [def-author-0336834a2590-measurable-surface-domains](item-def-author-0336834a2590-measurable-surface-domains). In a source chart the measure has smooth positive density $\sqrt{\det(h_{ab})}$ relative to Euclidean area. The source and target metrics are smooth and positive definite as in [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold).

[F2] A $C^1$ map between smooth manifolds has $C^1$ componentwise coordinate representatives on open Euclidean sets. [math:def-c-r-and-smooth-maps-between-smooth-manifolds](https://alphabetamath.cc/item/def-c-r-and-smooth-maps-between-smooth-manifolds)

[F3] The Euclidean total derivative is the linear approximation with normwise remainder $o(|v|)$. Continuous partial derivatives on a neighborhood imply total differentiability, with derivative the Jacobian matrix; the total derivatives satisfy the chain rule on open Euclidean sets. [math:def-total-derivative-in-euclidean-space](https://alphabetamath.cc/item/def-total-derivative-in-euclidean-space) [math:thm-continuous-partial-derivatives-imply-total-differentiability](https://alphabetamath.cc/item/thm-continuous-partial-derivatives-imply-total-differentiability) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F4] Coordinate tangent vectors form a basis, and their change under smooth coordinate transitions is given by the transition Jacobian. [math:thm-coordinate-derivations-form-a-basis-of-the-tangent-space](https://alphabetamath.cc/item/thm-coordinate-derivations-form-a-basis-of-the-tangent-space) [math:thm-change-of-coordinate-formula-for-tangent-bases](https://alphabetamath.cc/item/thm-change-of-coordinate-formula-for-tangent-bases)

[F5] Under countable choice, almost every point of a Lebesgue measurable Euclidean set has density one in that set. [math:thm-lebesgue-density-theorem](https://alphabetamath.cc/item/thm-lebesgue-density-theorem)

## Justification

**Given:** The data in the Definition and the supplied facts above.

1.1 By [F2] and [F3], every coordinate representative of $G$ has a total derivative whose entries are continuous. Under changes of source coordinates $x$ to $x'$ and target coordinates $y$ to $y'$, set $a=x'\circ x^{-1}$, $b=y'\circ y^{-1}$ and $f=y\circ G\circ x^{-1}$. The new representative is $b\circ f\circ a^{-1}$; the chain rule gives its derivative $Db\,Df\,(Da)^{-1}$ at the corresponding points, since differentiating the identities for the smooth transition and its inverse gives inverse derivative matrices. By [F4], source vector components change by $Da$ and target components by $Db$. Hence the two matrices give the same intrinsic linear map on tangent spaces. This establishes the stated $C^1$ differential without extending the smooth-germ pullback definition beyond its hypotheses. [F2, F3, F4, given]

1.2 In each source chart $(V,x)$, the set $x(P_n\cap V)$ is Lebesgue measurable for every Borel piece $P_n$. By the Lebesgue density theorem [F5], its density-one points exhaust that piece up to a Euclidean null set. The smooth positive area density in [F1] is locally bounded above and below away from zero on relatively compact chart patches, so Euclidean and Riemannian null sets there coincide. For each member of a countable base that lies in a chart, choose one such chart; these choices give a countable covering atlas by [A1]. There are countably many chart and piece pairs, so their exceptional sets have a single $\mu_C$-null union. Applying this argument to the union of two countable atlases shows that changing the atlas affects the admissible density-point sets only on a null set. No pointwise coordinate-invariance assertion about density is needed. [A1, F1, F5]

2.1 At a density-one point $p$ of a piece, two $C^1$ extensions agreeing on that piece have the same value at $p$. In a common target chart, subtract their coordinate representatives. Their difference is zero on the piece and has expansion $Lz+o(|z|)$ at $p$. If $L\ne0$, choose a direction $w$ with $Lw\ne0$; on a small cone about $w$ there is $c>0$ with $|Lz|\ge c|z|$. For sufficiently small nonzero $z$ in that cone the expansion cannot vanish. The cone occupies a fixed positive fraction of each centered ball, contradicting density one. Therefore $L=0$, and step 1.1 identifies the two intrinsic differentials. For two countable partitions, discard their null exceptional sets from step 1.2; a point in both remaining density-one pieces has density one in their intersection, since the missing fractions add. The same argument on this intersection proves independence almost everywhere of both extensions and partitions. [F1, F2, F3, step 1.1, step 1.2]

3.1 On each Borel piece the Gram Jacobian of its extension is continuous in local coordinates: writing $H$ for the positive definite source metric matrix, $K$ for the target metric matrix at the image, and $B$ for the derivative matrix, its square is $\det(B^T K B)/\det H$. This is nonnegative, including rank loss. Thus the piecewise Jacobian is measurable, and changing it on the null exceptional set preserves measurability for the completed measure $\mu_C$. Orthogonal source basis changes conjugate its Gram matrix and preserve its determinant. If the derivative takes values in a smooth target surface with the induced metric, its matrix $M$ in orthonormal surface bases satisfies $\det(M^TM)=(\det M)^2$; hence the square root is the absolute determinant. These facts retain the arbitrary-rank definition and require no smoothness of the image cut. [F1, F2, F3, F4, step 1.1, step 1.2, step 2.1, algebra] ∎

## Source notes

The Lebesgue density theorem, under the standing ZFC convention, supplies the density-one assertion on every Borel partition piece in source charts. [math:thm-lebesgue-density-theorem](https://alphabetamath.cc/item/thm-lebesgue-density-theorem)

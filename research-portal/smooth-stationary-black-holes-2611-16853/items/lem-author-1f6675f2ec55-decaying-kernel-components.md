---
id: lem-author-1f6675f2ec55-decaying-kernel-components
title: Decaying Dirichlet kernel and the exact closed-component exception
kind: lemma
status: draft
origin: pipeline
domain: mathematics
proof_strategy: direct
deps:
  - math:def-axiom-of-choice
  - def-exterior-weighted-elliptic-data
  - def-weighted-holder-spaces
  - lem-author-1f6675f2ec55-continuous-potential-comparison
  - lem-author-58255dfd955f-coordinate-schrodinger-form
  - math:lem-the-riemannian-volume-density-is-coordinate-independent
  - math:thm-smooth-partitions-of-unity-exist-on-manifolds
  - math:thm-a-positive-smooth-density-defines-a-locally-finite-radon-measure
  - math:thm-density-measure-integration-agrees-with-smooth-density-integration
dependency_roles:
  math:def-axiom-of-choice: mathematical-premise
  def-exterior-weighted-elliptic-data: mathematical-premise
  def-weighted-holder-spaces: mathematical-premise
  lem-author-1f6675f2ec55-continuous-potential-comparison: mathematical-premise
  lem-author-58255dfd955f-coordinate-schrodinger-form: mathematical-premise
  math:lem-the-riemannian-volume-density-is-coordinate-independent: mathematical-premise
  math:thm-smooth-partitions-of-unity-exist-on-manifolds: mathematical-premise
  math:thm-a-positive-smooth-density-defines-a-locally-finite-radon-measure: mathematical-premise
  math:thm-density-measure-integration-agrees-with-smooth-density-integration: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
dependency_level: 2
---

## Statement

Assume the Axiom of Choice. Let $(\Sigma,h)$ be the possibly disconnected exterior of the weighted exterior definition, let $\beta<0$, and let $V\ge0$ belong to $C^{2,\alpha}_{-4}$. If $u\in X_\beta$ solves $(\Delta_h-V)u=0$, then $u$ vanishes on every component having the asymptotic end or a nonempty boundary. On each closed compact component it is constant, and that constant must be zero unless $V$ is identically zero on the component. Conversely constants on the closed components where $V\equiv0$, extended by zero on the other components, are kernel elements. In particular the kernel is zero on a connected exterior, including the case of empty inner boundary. The decay condition means uniform convergence to zero on the end.

## Statement references

[[math:def-axiom-of-choice]]

[[def-exterior-weighted-elliptic-data]]

[[def-weighted-holder-spaces]]

[[lem-author-1f6675f2ec55-continuous-potential-comparison]]

[[lem-author-58255dfd955f-coordinate-schrodinger-form]]

[[math:lem-the-riemannian-volume-density-is-coordinate-independent]]

[[math:thm-smooth-partitions-of-unity-exist-on-manifolds]]

[[math:thm-a-positive-smooth-density-defines-a-locally-finite-radon-measure]]

[[math:thm-density-measure-integration-agrees-with-smooth-density-integration]]

## Facts & Assumptions

**Given:** The hypotheses of the Statement.

**Goal:** Establish the exact decaying Dirichlet kernel classification.

[F1] The Axiom of Choice implies Countable Choice, as required by the partition-of-unity supplier and the comparison supplier. [[math:def-axiom-of-choice]]

[F2] The exterior has a compact core, one Euclidean exterior end, a compact smooth boundary, and the stated weighted spaces; $\beta<0$ implies $u\to0$ uniformly on the end. [[def-exterior-weighted-elliptic-data]] [[def-weighted-holder-spaces]]

[F3] Compact-domain comparison holds with a merely continuous nonnegative potential when every component meets the boundary. [[lem-author-1f6675f2ec55-continuous-potential-comparison]]

[F4] For real $C^2$ functions, the coordinate supplier gives the pointwise operator formula $\Delta_h u=h^{ij}\partial_{ij}u+b^j\partial_j u$, with $b^j=m^{-1}\partial_i(mh^{ij})$ and $m=\sqrt{\det(h_{ij})}$, by taking its smooth auxiliary potential to be zero. This operator formula does not require the function to solve the auxiliary equation. [[lem-author-58255dfd955f-coordinate-schrodinger-form]]

[F5] The Riemannian volume comes from the positive coordinate-independent smooth density $m\,|dx|$, with no orientability requirement. Under Countable Choice its measure $\mu_h$ is finite on compact sets, and integrals of Borel $L^1(\mu_h)$ functions equal the partition-weighted chart integrals. Thus continuous functions on a compact component are integrable, including the finite-regularity integrands used below. [[math:lem-the-riemannian-volume-density-is-coordinate-independent]] [[math:thm-a-positive-smooth-density-defines-a-locally-finite-radon-measure]] [[math:thm-density-measure-integration-agrees-with-smooth-density-integration]]

[F6] Under Countable Choice a smooth manifold has a smooth partition of unity subordinate to any open cover, with nonnegative functions supported in the respective cover members and summing to one. [[math:thm-smooth-partitions-of-unity-exist-on-manifolds]]

## Proof

**Given:** The hypotheses of the Statement and the conventions in Facts & Assumptions.

**Proof technique:** direct.

1.1 On the component containing the end, truncate at a sufficiently large coordinate sphere $r=R$. No component of this truncation can be closed: a boundaryless component would be open and closed in the connected end component and separated from its nonempty end. Put $a_R=\sup_{r=R}|u|$. On the truncation, both $u-a_R$ and $-u-a_R$ have nonpositive boundary values and satisfy $(\Delta_h-V)(\pm u-a_R)=Va_R\ge0$. Comparison gives $|u|\le a_R$. Weighted decay makes $a_R\to0$, so $u=0$ there. The same comparison on each compact component with nonempty boundary gives zero directly, using $a_R=0$. [F1, F2, F3, algebra]

1.2 Let $C$ be a closed compact connected component. On each coordinate chart of $C$, put $A^{ij}=mh^{ij}$. Applying only the pointwise operator formula in [F4], with its auxiliary potential zero, and expanding the derivative gives $\Delta_hu=m^{-1}\partial_i(A^{ij}\partial_j u)$. Hence the actual equation with the stated $V$ gives $-\partial_i(A^{ij}\partial_j u)+mVu=0$. Here $u$ is $C^{4,\alpha}$ locally and $V$ is continuous; only multiplication by $V$ is used, and no derivative of $V$ is taken. This application therefore does not require the actual potential to be smooth. [F2, F4, given, algebra]

2.1 Choose a finite cover of $C$ by relatively compact coordinate neighborhoods $U_a$. By [F1] and [F6] choose a subordinate smooth partition $\chi_a$; since $C$ is compact, each support is compactly contained in its chart. In the $a$th chart multiply the equation of step 1.2 by $\chi_a u$. The coordinate products $\chi_a u A^{ij}\partial_j u$ are $C^1$ with compact support in the open chart image. After extension by zero, integration of each $i$th derivative first in the $i$th coordinate gives zero by the fundamental theorem of calculus. Expanding those derivatives and using the density of [F5] therefore gives $\int_C(\chi_a|\nabla u|_h^2+u h^{ij}\partial_j u\partial_i\chi_a+\chi_a V u^2)\,d\mu_h=0$, where $|\nabla u|_h^2=h^{ij}\partial_i u\partial_j u$ and the integrands are zero off the chart support. The middle term is the intrinsic inverse-metric pairing of $du$ with $d\chi_a$, multiplied by $u$. Sum these finitely many identities: $\sum_a\chi_a=1$ and $\sum_a d\chi_a=0$ cancel the middle terms and give $\int_C(|\nabla u|_h^2+Vu^2)\,d\mu_h=0$. The positive density makes this argument valid even when $C$ is nonorientable. [F1, F2, F5, F6, step 1.2, construct, algebra]

3.1 The two integrands in the energy identity are continuous and nonnegative. If either were positive at a point, it would have positive integral on a smaller coordinate ball because the density is positive. Thus $du=0$ and $Vu^2=0$ everywhere on $C$. The fundamental theorem of calculus along chart segments makes $u$ locally constant, so connectedness makes it constant on $C$. That constant is zero if $V$ is nonzero anywhere on $C$; if $V\equiv0$ every constant solves the equation. Every component other than the end component lies in the compact core and is closed, hence compact. There are only finitely many such components: the open components of the manifold cover the compact core and have a finite subcover. Functions that are constant on any of the closed components with $V\equiv0$ and zero on all other components are locally smooth, vanish on the boundary and on the end, and have finite norm on the fixed compact chart subsets. They therefore belong to $X_\beta$ and solve the equation. Combined with step 1.1, this proves the converse, the exact kernel classification and the connected-exterior conclusion. [F2, F5, step 1.1, step 2.1, algebra] ∎

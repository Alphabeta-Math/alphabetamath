---
id: lem-author-60420990c802-uniform-inward-normal-exponential-collar
title: A compact smooth boundary has a uniform inward normal exponential collar
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - math:thm-collar-neighborhood-theorem
  - math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary
  - math:def-axiom-of-choice
  - math:thm-existence-uniqueness-and-smooth-dependence-of-geodesics
  - math:thm-the-exponential-domain-is-open-and-the-exponential-map-is-smooth
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-domain-and-exponential-map-of-a-connection
  - math:def-smooth-collar-of-a-manifold-boundary
  - math:thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold
  - math:def-smooth-function-on-a-relatively-open-subset-of-a-half-space
  - math:def-levi-civita-connection
  - math:thm-fundamental-theorem-of-riemannian-geometry
  - math:lem-geodesic-scaling-identity
dependency_roles:
  math:thm-collar-neighborhood-theorem: mathematical-premise
  math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-existence-uniqueness-and-smooth-dependence-of-geodesics: mathematical-premise
  math:thm-the-exponential-domain-is-open-and-the-exponential-map-is-smooth: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-domain-and-exponential-map-of-a-connection: mathematical-premise
  math:def-smooth-collar-of-a-manifold-boundary: mathematical-premise
  math:thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold: mathematical-premise
  math:def-smooth-function-on-a-relatively-open-subset-of-a-half-space: mathematical-premise
  math:def-levi-civita-connection: mathematical-premise
  math:thm-fundamental-theorem-of-riemannian-geometry: mathematical-premise
  math:lem-geodesic-scaling-identity: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $(\Sigma,h)$ be a smooth Riemannian manifold with compact boundary $S$, with smooth positive metric up to $S$. Then for some $a>0$ the inward normal exponential map $F(p,s)=\exp_p(s\nu_p)$ is a smooth injective collar on $S\times[0,a]$, with image in $\Sigma$ and $F(p,0)=p$. Here $\nu$ is the inward unit normal to $S$ in $\Sigma$. The construction uses a local smooth extension of the metric across $S$, but the positive-time collar and its metric are determined by the original data. No completeness or global boundary-distance regularity is assumed.

## Facts & Assumptions

[F1] Work in ZFC. Smooth boundary collars and smooth partitions of unity exist under its countable-choice consequence; these are the choice-dependent suppliers used below. Smoothness up to a boundary means local smooth coordinate extension. [[math:thm-collar-neighborhood-theorem]] [[math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary]] [[math:def-axiom-of-choice]] [[math:def-smooth-function-on-a-relatively-open-subset-of-a-half-space]]

[F2] On a boundaryless manifold with a supplied affine connection, geodesics exist uniquely and depend smoothly on initial data. The exponential domain is open and its map is smooth; geodesic scaling identifies $\exp_p(sv)$ with $\gamma_{p,v}(s)$ whenever defined. The smooth inverse function theorem applies to an invertible differential. [[math:thm-existence-uniqueness-and-smooth-dependence-of-geodesics]] [[math:def-domain-and-exponential-map-of-a-connection]] [[math:thm-the-exponential-domain-is-open-and-the-exponential-map-is-smooth]] [[math:lem-geodesic-scaling-identity]] [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[F3] A Riemannian metric is a smooth positive definite symmetric tensor, with boundary allowed here. The boundary is a closed embedded smooth boundaryless hypersurface in positive dimension, and is empty in dimension zero. A smooth collar has half-open parameter interval and relatively open image; a closed collar here means a closed smaller truncation of such a collar. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold]] [[math:def-smooth-collar-of-a-manifold-boundary]]

[F4] A Levi-Civita connection is a torsion-free metric-compatible affine connection. Every smooth Riemannian metric, including one smooth up to a boundary, has exactly one such connection. [[math:def-levi-civita-connection]] [[math:thm-fundamental-theorem-of-riemannian-geometry]]

## Proof

**Given:** The hypotheses in the Statement, working in ZFC as in [F1].

**Goal:** Establish the stated conclusions.

1.1 If $S=\varnothing$, the empty map gives the conclusion for any $a>0$; otherwise the dimension is positive and $S$ is a compact smooth boundaryless hypersurface. Choose a smooth collar $c:S\times[0,b)\to\Sigma$ and write $r$ for its second coordinate. Pull $h$ back to this product. In a finite product-coordinate cover near $S\times\{0\}$ its tensor coefficients admit smooth extensions to negative $r$. Choose a finite smooth partition $(\chi_i)$ on compact $S$, subordinate to these coordinate sets with supports compactly contained in them. Extend each tensor on a product neighborhood of its support, multiply by $\chi_i$ independent of $r$, and sum, extending each weighted term by zero across its lateral edges. For a common $\delta>0$ the sum is a smooth symmetric tensor $H$ on the boundaryless manifold $N=S\times(-\delta,\delta)$ and agrees with $c^*h$ for $r\ge0$. Positive definiteness at $r=0$, continuity and compactness let us shrink $\delta$ until $H$ is a Riemannian metric throughout $N$. Identify its nonnegative side with its image under $c$. [given, F1, F3]

2.1 The inward unit normal needs no additional existence assumption. Along $r=0$ let $W$ be the unique vector satisfying $H(W,V)=dr(V)$ for every tangent vector $V$. In product coordinates $W^i=\sum_j H^{ij}\partial_jr$; the inverse matrix is smooth by the cofactor formula and its nonzero determinant. Moreover $dr(W)=H(W,W)>0$ because $dr\ne0$. Thus $\nu=W/\sqrt{H(W,W)}$ is smooth, orthogonal to $TS=\ker dr$, unit, and inward. The orthogonal complement of $TS$ is one dimensional, so these properties uniquely specify $\nu$ from the original metric and inward side. [F3, step 1.1, algebra]

2.2 Give $(N,H)$ its unique Levi-Civita connection. On the identified nonnegative side it agrees with the Levi-Civita connection of $h$: restriction has the same metric compatibility and torsion-free identities, so uniqueness applies, including at the boundary. Consequently the exponential used below is the exponential of this specified connection on a boundaryless manifold, exactly within the domain convention of [F2]. [F2, F4, step 1.1]

3.1 Define $F(p,s)=\exp_p(s\nu_p)$ on $N$. Openness of the exponential domain around the zero section, smoothness of $\nu$, and compactness of $S$ give a common interval $|s|<b_0$ on which $F$ is smooth. Geodesic scaling gives $F(p,s)=\gamma_{p,\nu_p}(s)$ and hence $\partial_sF(p,0)=\nu_p$, while $F(p,0)=p$ gives the identity differential on $T_pS$. Therefore $dF_{(p,0)}(u,t)=u+t\nu_p$ is an isomorphism. Apply the inverse function theorem at each $(p,0)$; a finite cover and openness of invertibility make $F$ a local diffeomorphism on $S\times(-b_1,b_1)$ for some $b_1>0$. Also $\partial_s(r\circ F)(p,0)=dr(\nu_p)>0$. Continuity and compactness allow a further uniform shrink so that this derivative stays positive. Since $(r\circ F)(p,0)=0$, positive $s$ then maps into the original interior and negative $s$ into the added side. [F2, step 1.1, step 2.1, step 2.2]

4.1 If no uniform positive width gave injectivity, there would be distinct pairs $(p_j,s_j),(q_j,t_j)$ with $0\le s_j,t_j\le1/j$, all within the preceding domain, and $F(p_j,s_j)=F(q_j,t_j)$. Compactness of $S\times S$ gives a subsequence with $p_j\to p$ and $q_j\to q$. Continuity and $F(p,0)=p$ imply $p=q$. Both pairs eventually lie in the same inverse-function neighborhood of $(p,0)$ from step 3.1, contradicting its injectivity. Thus choose $a>0$ strictly smaller than an injective local-diffeomorphism width. The local inverses agree, so $F|_{S\times[0,a)}$ is a smooth collar in the sense of [F3], and $F|_{S\times[0,a]}$ is its smooth embedded closed truncation. Its image contains a relative neighborhood of $S$ in $\Sigma$; compactness makes the closed image closed, and the local inverses show that its only boundary in $\Sigma^\circ$ is the outer face $F(S,a)$. [F2, F3, step 3.1]

5.1 All positive-time geodesic segments just obtained stay on the original side. For any second smooth metric extension, its inward unit normal is the same by step 2.1 and its connection restricted to that side is the same by step 2.2. In local coordinates its positive-time curves therefore solve the same initial-value geodesic equation as the first extension, including at time zero. Uniqueness for that equation, first near zero and then along the common segment, identifies the curves on every common sufficiently small collar. Their pulled-back metrics agree because each is the pullback of $h$ along this same map. This proves extension independence, without completeness or any assumption about global boundary distance. [F2, F4, step 2.1, step 2.2, step 3.1, step 4.1] ∎

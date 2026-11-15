---
id: lem-author-9f9c6144aed8-sublevel-path-exhaustion
title: Pathwise exhaustion by anchored Ernst sublevels
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-9f9c6144aed8-ernst-mars-simon
  - def-stationary-lorentzian-data
  - math:def-smooth-manifold
  - math:def-connected-component-and-quasicomponent
  - math:def-path-connected
  - math:def-continuous-map-top
  - math:def-subspace-topology-top
  - math:def-type-r-s-tensor-bundle
  - math:def-direct-sum-model-of-complexification
  - math:lem-continuity-is-local-and-pastes
  - math:lem-closed-interval-compactness-from-completeness
  - math:thm-extreme-value-r
  - math:thm-connected-subsets-of-r-are-intervals
  - math:cor-connected-subsets-of-the-line
  - math:thm-continuous-image-of-a-connected-space
  - math:lem-real-line-is-a-metric-space
  - math:def-continuity-real
  - math:def-open-cover-r
  - math:def-c-r-and-smooth-maps-between-smooth-manifolds
  - math:thm-ck-euclidean-maps-closed-under-algebra-and-composition
  - math:lem-matrix-inversion-preserves-ck-regularity
  - math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure
  - math:prop-smooth-maps-are-continuous
  - math:thm-complex-numbers-form-a-field
dependency_roles:
  def-author-9f9c6144aed8-ernst-mars-simon: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  math:def-smooth-manifold: mathematical-premise
  math:def-connected-component-and-quasicomponent: mathematical-premise
  math:def-path-connected: mathematical-premise
  math:def-continuous-map-top: mathematical-premise
  math:def-subspace-topology-top: mathematical-premise
  math:def-type-r-s-tensor-bundle: mathematical-premise
  math:def-direct-sum-model-of-complexification: mathematical-premise
  math:lem-continuity-is-local-and-pastes: mathematical-premise
  math:lem-closed-interval-compactness-from-completeness: mathematical-premise
  math:thm-extreme-value-r: mathematical-premise
  math:thm-connected-subsets-of-r-are-intervals: mathematical-premise
  math:cor-connected-subsets-of-the-line: mathematical-premise
  math:thm-continuous-image-of-a-connected-space: mathematical-premise
  math:lem-real-line-is-a-metric-space: mathematical-premise
  math:def-continuity-real: mathematical-premise
  math:def-open-cover-r: mathematical-premise
  math:def-c-r-and-smooth-maps-between-smooth-manifolds: mathematical-premise
  math:thm-ck-euclidean-maps-closed-under-algebra-and-composition: mathematical-premise
  math:lem-matrix-inversion-preserves-ck-regularity: mathematical-premise
  math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure: mathematical-premise
  math:prop-smooth-maps-are-continuous: mathematical-premise
  math:thm-complex-numbers-form-a-field: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Let $X$ be a smooth manifold, $y:X\to\mathbb R$ continuous, $q\in X$, and for $R>y(q)$ let $U_R$ be the connected component containing $q$ of $\{y<R\}$. Every point joined to $q$ by a continuous path in $X$ belongs to some $U_R$. Hence if a tensor field vanishes on every $U_R$, it vanishes on the path component of $q$.

Here all subsets carry the subspace topology. A tensor field may have any fixed type $(r,s)$, with $r,s$ nonnegative integers: at each $p\in X$ it assigns an element of the fibre $T^r_sX$ over $p$. A complex tensor field assigns a pair of real tensors in that fibre, written $A_p+iB_p$; zero means that both parts are zero. No regularity of the tensor field is required.

This applies to the reciprocal potential in the Ernst–Mars–Simon interface on any manifold region where it is defined, using the stationary Lorentzian conventions. It does not prove that this region is the whole exterior, or supply vanishing on a sublevel.

## Statement references

[[math:def-smooth-manifold]]

[[math:def-continuous-map-top]]

[[math:def-subspace-topology-top]]

[[math:def-connected-component-and-quasicomponent]]

[[math:def-path-connected]]

[[math:def-type-r-s-tensor-bundle]]

[[math:def-direct-sum-model-of-complexification]]

[[def-author-9f9c6144aed8-ernst-mars-simon]]

[[def-stationary-lorentzian-data]]

## Facts & Assumptions

[F1] The Ernst interface supplies a smooth complex scalar $\sigma$, the open set $N=\{1-\sigma\ne0\}$, and the definitions $P=(1-\sigma)^{-1}$ and $y=\operatorname{Re}P$ there. Smoothness of $P,y$ and continuity of $y$ are established below from these data. This supplies no assertion that $N$ is the whole exterior. [[def-author-9f9c6144aed8-ernst-mars-simon]]

[F2] In the stationary application, the ambient smooth manifold and tensor conventions are those of the stationary Lorentzian interface. The general $X$ in the Statement is a smooth manifold of arbitrary dimension. [[def-stationary-lorentzian-data]] [[math:def-smooth-manifold]]

[F3] The type $(r,s)$ tensor bundle has at each point the real multilinear-tensor fibre. Its complexification can be represented by pairs of real tensors, whose zero is the pair of zero tensors. [[math:def-type-r-s-tensor-bundle]] [[math:def-direct-sum-model-of-complexification]]

[F4] A composite of continuous maps of topological spaces is continuous. Continuity here is topological continuity, with the usual topology on $\mathbb R$. [[math:lem-continuity-is-local-and-pastes]] [[math:def-continuous-map-top]]

[F5] A closed interval $[a,b]$ with $a<b$ in $\mathbb R$ is compact for relative open covers. A real open cover consists of ambient open subsets of $\mathbb R$ covering the set. The real extreme-value theorem applies to a real-variable continuous function on a nonempty compact subset of its real domain and supplies an attained finite maximum. [[math:lem-closed-interval-compactness-from-completeness]] [[math:def-open-cover-r]] [[math:thm-extreme-value-r]]

[F6] An order-convex subset of $\mathbb R$, in particular $[0,1]$, is connected in the real separated-set sense. The topological bridge identifies this with connectedness for the subspace topology inherited from the usual topology on $\mathbb R$. Thus $[0,1]$ with that subspace topology is connected as a topological space. [[math:thm-connected-subsets-of-r-are-intervals]] [[math:cor-connected-subsets-of-the-line]]

[F7] Continuous images of connected spaces are connected. A map whose image lies in a subspace is continuous into that subspace exactly when its composite with the inclusion is continuous. The connected component of a point in that subspace contains every connected subset through that point. [[math:thm-continuous-image-of-a-connected-space]] [[math:def-subspace-topology-top]] [[math:def-connected-component-and-quasicomponent]]

[F8] A path from $q$ to $p$ is a continuous map $\gamma:[0,1]\to X$ with endpoints $q,p$; the path component of $q$ consists exactly of its path endpoints. [[math:def-path-connected]]

[F9] The usual topology of $\mathbb R$ has a neighborhood basis $(c-\delta,c+\delta)$, equivalently $\{t:|t-c|<\delta\}$, with $\delta>0$. Real-variable continuity on $A\subseteq\mathbb R$ is the relative epsilon–delta condition at each $c\in A$. [[math:lem-real-line-is-a-metric-space]] [[math:def-continuity-real]]

[F10] Smooth maps are described in smooth charts by componentwise $C^k$ Euclidean maps for every finite $k$. Finite sums, scalar multiples, products and compositions preserve $C^k$ on open Euclidean domains. For $m,n\ge1$, a $C^k$ map from an open subset of $\mathbb R^m$ to real $n\times n$ matrices has a $C^k$ inverse wherever its determinant is nonzero; the case $n=1$ gives scalar reciprocals. [[math:def-c-r-and-smooth-maps-between-smooth-manifolds]] [[math:thm-ck-euclidean-maps-closed-under-algebra-and-composition]] [[math:lem-matrix-inversion-preserves-ck-regularity]]

[F11] An open subset of a smooth manifold carries the restricted smooth structure, with its subspace topology. A smooth map on an open manifold domain is continuous there. [[math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure]] [[math:prop-smooth-maps-are-continuous]]

[F12] Every complex number has unique real and imaginary parts; if $u+iv\ne0$, then $(u+iv)^{-1}=(u-iv)/(u^2+v^2)$ and $u^2+v^2>0$. [[math:thm-complex-numbers-form-a-field]]

## Proof

**Given:** The objects in the Statement and a path $\gamma:[0,1]\to X$ with $\gamma(0)=q$ and $\gamma(1)=p$.

**Goal:** Put $p$ in some $U_R$ and deduce the vanishing assertion.

1.1 Put $h=y\circ\gamma:[0,1]\to\mathbb R$, which is topologically continuous by composition. For $c\in[0,1]$ and $\varepsilon>0$, continuity supplies a relative open neighborhood $W$ of $c$ mapped into $(h(c)-\varepsilon,h(c)+\varepsilon)$. Write $W=O\cap[0,1]$ with $O$ open in $\mathbb R$. Choose $\delta>0$ with $(c-\delta,c+\delta)\subseteq O$. Then $t\in[0,1]$ and $|t-c|<\delta$ imply $|h(t)-h(c)|<\varepsilon$. Thus $h$ satisfies precisely the real-variable continuity hypothesis of the extreme-value theorem. [given, F4, F7, F9, choose]

1.2 In the stationary application, $N$ is an open subset of the supplied smooth four-manifold, so use its restricted smooth structure. Identify a smooth complex scalar with its two real component functions and write $\sigma=a+ib$. On $N$ put $d=(1-a)^2+b^2>0$. The complex inverse formula gives $P=(1-a+ib)/d$ and $y=(1-a)/d$. In every restricted chart, $a,b,d$ are $C^k$ for every finite $k$ by componentwise smoothness and finite algebra. Apply the inverse-regularity result to the $1\times1$ matrix $[d]$ on that open chart domain: its determinant is $d\ne0$, so $1/d$ is $C^k$ for every finite $k$. Finite products give both components of $P$ and $y$ the same regularity. These components are continuous in the charts because order-zero regularity is included in $C^k$; composing with chart homeomorphisms gives continuity locally on $N$, and locality gives continuity on $N$. The smooth-map definition now gives smoothness of $P,y$, and the smooth-continuity result also gives the continuity of $y$ needed by the lemma. [F1, F2, F4, F10, F11, F12, algebra]

2.1 The interval $[0,1]$ is nonempty and compact for relative open covers since $0<1$. Restricting any ambient real open cover to $[0,1]$ gives a relative open cover; its finite subcover supplies a finite selection of the original ambient sets, still covering $[0,1]$. Hence the interval is compact also in the real open-cover convention. Apply the real extreme-value theorem to $A=K=[0,1]$ and $h$ from step 1.1 to obtain a finite maximum $B$. Put $R=B+1$. Then $R>y(q)$ and $\gamma([0,1])\subseteq\{y<R\}$. [given, step 1.1, F5, F7, choose]

3.1 Write $S_R=\{y<R\}$. The same path regarded as a map $[0,1]\to S_R$ is continuous by the characteristic property of the subspace topology. The interval with its usual subspace topology is connected as a topological space by F6, so its image is connected in $S_R$ and contains $q$. [given, step 2.1, F6, F7]

4.1 The connected-component definition in $S_R$ puts this connected image through $q$ inside $U_R$. In particular, $p=\gamma(1)\in U_R$. [step 3.1, F7]

5.1 If the specified tensor field vanishes on every $U_R$, step 4.1 gives its zero value at $p$. This uses only pointwise zero in the tensor fibre, and applies equally to both parts of a complex tensor. Every point in the path component is such an endpoint, so the field vanishes on that component. [given, step 4.1, F3, F8]

6.1 Apply steps 1.1, 2.1, 3.1, 4.1 and 5.1 on $N$, or on any manifold region in $N$ on which the potential is restricted, using the continuity established in step 1.2. The domain restriction and the need to supply sublevel vanishing are retained: this gives neither that $N$ is the whole exterior nor vanishing on a sublevel. [step 1.1, step 2.1, step 3.1, step 4.1, step 5.1, step 1.2, F1, F2] ∎

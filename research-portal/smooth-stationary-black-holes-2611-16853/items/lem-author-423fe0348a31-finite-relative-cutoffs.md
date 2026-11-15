---
id: lem-author-423fe0348a31-finite-relative-cutoffs
title: Finite smooth cutoffs relative to compact sets and boundary neighborhoods
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-smooth-partition-of-unity-on-a-manifold-with-boundary
  - math:def-topological-manifold-with-boundary
  - math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary
  - math:def-smooth-function-on-a-relatively-open-subset-of-a-half-space
  - math:lem-smooth-bump-between-concentric-euclidean-balls
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:thm-heine-borel-rn
  - math:thm-compactness-agrees-with-metric-compactness
  - math:thm-compactness-under-continuous-maps
  - math:thm-compact-subset-of-a-hausdorff-space-is-closed
  - math:thm-algebra-of-derivatives
  - math:prop-chain-rule-for-smooth-half-space-maps
  - math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold
  - math:thm-the-interior-is-an-open-smooth-n-manifold
dependency_roles:
  math:def-smooth-partition-of-unity-on-a-manifold-with-boundary: mathematical-premise
  math:def-topological-manifold-with-boundary: mathematical-premise
  math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary: mathematical-premise
  math:def-smooth-function-on-a-relatively-open-subset-of-a-half-space: mathematical-premise
  math:lem-smooth-bump-between-concentric-euclidean-balls: mathematical-premise
  math:lem-compactness-of-a-subspace-is-ambient: mathematical-premise
  math:thm-heine-borel-rn: mathematical-premise
  math:thm-compactness-agrees-with-metric-compactness: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:thm-compact-subset-of-a-hausdorff-space-is-closed: mathematical-premise
  math:thm-algebra-of-derivatives: mathematical-premise
  math:prop-chain-rule-for-smooth-half-space-maps: mathematical-premise
  math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold: mathematical-premise
  math:thm-the-interior-is-an-open-smooth-n-manifold: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

On a compact smooth manifold with boundary $R$, let $K\subset V$ with $K$ compact and $V$ open. There is a smooth $\chi:R\to[0,1]$ equal to one on a neighborhood of $K$ and supported in $V$. If $K$ lies in the interior, the support may be compactly contained in the interior. Given finitely many coordinate neighborhoods covering a compact interior set $K$, there are finitely many smooth functions $\chi_j$ compactly supported in those neighborhoods with $\sum_j\chi_j=1$ near $K$.

## Facts & Assumptions

[F1] Support is the closure in $R$ of the nonzero locus. The manifold is Hausdorff, coordinate images are relatively open in a half-space, and smoothness at the boundary means local smooth Euclidean extension. [[math:def-smooth-partition-of-unity-on-a-manifold-with-boundary]] [[math:def-topological-manifold-with-boundary]] [[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary]] [[math:def-smooth-function-on-a-relatively-open-subset-of-a-half-space]]

[F2] For $n\ge1$ and $0<r<s$, there is a smooth $\rho:\mathbb R^n\to[0,1]$ equal to one on $\overline B_r(0)$ and supported in $B_s(0)$; translation gives the corresponding bump centered at any coordinate point. [[math:lem-smooth-bump-between-concentric-euclidean-balls]]

[F3] An indexed cover of a compact subset by ambient open sets has a finite subcover (claim 2), including the empty-set alternative. [[math:lem-compactness-of-a-subspace-is-ambient]]

[F4] Closed bounded Euclidean sets are compact; metric and topological compactness agree. Continuous images of compact sets are compact (clause 1), and compact subsets of a Hausdorff space are closed (clause 3). Since $R$ is compact and Hausdorff, every closed subset of $R$ is compact (clause 4 of the Hausdorff compactness theorem). [[math:thm-heine-borel-rn]] [[math:thm-compactness-agrees-with-metric-compactness]] [[math:thm-compactness-under-continuous-maps]] [[math:thm-compact-subset-of-a-hausdorff-space-is-closed]]

[F5] Coordinate sum, product and quotient differentiation rules, iterated on smooth Euclidean extensions, preserve smoothness wherever the quotient denominator is nonzero. The half-space chain rule makes composition and change of boundary coordinates smooth. [[math:thm-algebra-of-derivatives]] [[math:prop-chain-rule-for-smooth-half-space-maps]]

[F6] Write $R^\circ=\operatorname{Int}R$ for the manifold interior: in positive dimension its points have positive last boundary-chart coordinate, and in dimension zero every point is interior. For the smooth manifold with boundary $R$, this interior is open. [[math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold]] [[math:thm-the-interior-is-an-open-smooth-n-manifold]]

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Construct the asserted relative cutoff and a partition subordinate to the prescribed finite coordinate cover.

1.1 If $K=\varnothing$, take $\chi=0$ and take every function indexed by the prescribed finite coordinate cover to be zero; for an empty cover use the empty family. The required equalities near $K$ hold on the empty open neighborhood, and every support is empty. Henceforth suppose $K\ne\varnothing$. [given, F1, construct]

1.2 For an open neighborhood $W$ of a point $p$, take a boundary chart $\varphi:U\to O\subseteq\mathbb H^n$ and write $a=\varphi(p)$. In positive dimension choose $0<r<s$ with $\overline B_s(a)\cap\mathbb H^n\subseteq\varphi(U\cap W)$, using relative openness. By [F2] take a translated Euclidean bump equal to one on $\overline B_r(a)$ and supported in $B_s(a)$. Restrict it to $O$ and pull it back to $U$. The set $C=\varphi^{-1}(\overline B_s(a)\cap\mathbb H^n)$ is compact by [F4], closed in $R$, and contained in $U\cap W$. The pullback is zero on $U\setminus C$, so extension by zero on $R\setminus C$ is smooth: the two formulas agree on their open overlap, and the boundary-chart formula has a smooth ambient extension. Its support is closed in $R$, is therefore compact by [F4], lies in $C\subseteq W$, and it equals one on the open neighborhood $\varphi^{-1}(B_r(a)\cap\mathbb H^n)$ of $p$. In dimension zero, a singleton chart is open and closed, and its indicator is a smooth bump with that singleton as compact support. [F1, F2, F4, F5, construct]

2.1 Consider all the bumps and inner neighborhoods constructed in step 1.2 with $p\in K$ and $W=V$. Their inner neighborhoods form an indexed open cover of $K$; [F3] gives finitely many, with bumps $b_1,\ldots,b_N$. Set $\chi=1-\prod_{a=1}^N(1-b_a)$. This is smooth by the iterated product rule, takes values in $[0,1]$, and equals one on the union of the inner neighborhoods, since there one factor is zero. Its support lies in the finite union of the closed supports of the $b_a$, which is closed in $R$ and contained in $V$. Both this finite union and $\operatorname{supp}\chi$ are closed in compact Hausdorff $R$, hence compact by [F4]. If $K\subset R^\circ$, perform the same construction with $W=V\cap R^\circ$; the resulting support is compactly contained in $R^\circ$. This proves the first assertion and its interior refinement without taking a minimum or using a scalar cutoff. [given, F1, F3, F4, F5, F6, step 1.2, construct]

3.1 For the second assertion, write the prescribed coordinate neighborhoods as $U_1,\ldots,U_m$. Use all the local constructions of step 1.2 with $p\in K\cap U_j$ and $W=U_j\cap R^\circ$, retaining the index $j$. Their inner neighborhoods cover $K$, so [F3] gives finitely many bumps $b_a$, each with compact support in its assigned $U_{j(a)}\cap R^\circ$. Set $S=\sum_a b_a$ and $W_0=\{S>0\}\cap R^\circ$. This is open and contains $K$. Apply the already proved construction in step 2.1 with $V=W_0$ to obtain a smooth $\psi:R\to[0,1]$ equal to one near $K$ with compact support contained in $W_0$. [given, F1, F3, F5, F6, step 1.2, step 2.1, construct]

4.1 For $1\le j\le m$, define $\chi_j=\psi\bigl(\sum_{a:j(a)=j}b_a\bigr)/S$ on $W_0$, and set it to zero elsewhere; an empty numerator sum is zero. These functions are smooth on $W_0$ by [F5]. At every point outside $W_0$, the complement of the closed set $\operatorname{supp}\psi\subset W_0$ is a neighborhood on which both formulas are zero, proving smooth extension. Each $\chi_j$ is nonnegative and at most one. Its support lies in the intersection of $\operatorname{supp}\psi$ with the finite union of the supports assigned to $j$. This support is closed in $R$, so [F4] makes it compact; it is therefore compactly contained in $U_j\cap R^\circ$. Summing the formulas gives $\sum_j\chi_j=\psi$ on $W_0$, and both sides vanish off $W_0$. Thus the sum equals one near $K$, proving the second assertion. [F1, F4, F5, step 3.1, algebra] ∎

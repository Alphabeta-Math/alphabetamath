---
id: lem-author-12a8dba09036-maximal-stationary-far-tail-access
title: A maximal stationary exterior has future access to its far tail
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-12a8dba09036-maximal-shift-divergence-and-boundary
  - lem-author-12a8dba09036-complete-volume-preserving-shift-flow
  - lem-author-12a8dba09036-inaccessible-set-relative-interior-density
  - lem-author-12a8dba09036-finite-volume-exact-invariance
  - def-spacelike-maximal-hypersurface-data
  - physics:def-gr-causal-curves-and-reachability
  - math:def-axiom-of-choice
  - math:def-compact-space
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:def-borel-sigma-algebra
  - math:def-sigma-algebra
  - math:def-topological-space
dependency_roles:
  lem-author-12a8dba09036-maximal-shift-divergence-and-boundary: mathematical-premise
  lem-author-12a8dba09036-complete-volume-preserving-shift-flow: mathematical-premise
  lem-author-12a8dba09036-inaccessible-set-relative-interior-density: mathematical-premise
  lem-author-12a8dba09036-finite-volume-exact-invariance: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:lem-compactness-of-a-subspace-is-ambient: mathematical-premise
  math:def-borel-sigma-algebra: mathematical-premise
  math:def-sigma-algebra: mathematical-premise
  math:def-topological-space: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

Assume the Axiom of Choice. Let $E=\mathbb R\times C$ be a smooth stationary time-oriented Lorentz product as in the inaccessible-set lemma, with complete time-translation Killing field $T=\partial_t$ and spacelike slices. Write $n$ for the unit future normal, $h=g|_{TC}$, $k(U,V)=-g(\nabla_U n,V)$, $N=-g(T,n)$ and $X=T-Nn$. Suppose $C$ is connected and is the interior of a smooth spherical exterior $\overline C$: by this we mean a smooth manifold with compact boundary $S$ supplied with a diffeomorphism $F:\overline C\to\{y\in\mathbb R^3:|y|\ge1\}$, with $C=\overline C\setminus S$. Its stationary slice is maximal, $\operatorname{tr}_h k=0$. Assume its induced positive metric is smooth up to compact boundary $S$ and asymptotically Euclidean. Near $S$, assume the ambient time-oriented Lorentz metric $g$, the field $T$ and the slice extend smoothly across $S$, with the extended slice spacelike and $T$ tangent to $S$. These are extensions of the original geometric data, not an extension of the stationary product coordinates through $S$. Assume $N>0$ throughout $C$. Assume $T$ is future directed sufficiently far out. Specify the asymptotic stationary end by an open set $\mathcal A\subset C$ and a diffeomorphism $x:\mathcal A\to\{z\in\mathbb R^3:|z|>R_0\}$ for some $R_0>0$, such that $K_R=\overline C\setminus x^{-1}(\{|z|>R\})$ is compact for every $R>R_0$. Put $r(p)=|x(p)|$ on $\mathcal A$; the notation $\{r>R\}$ means $x^{-1}(\{|z|>R\})$. In the stationary coordinates $(t,x)$ on this end let $g_{00}=-1+O(r^{-1})$, $g_{0i}=O(r^{-2})$, and $g_{ij}=\delta_{ij}+O(r^{-1})$. For any sufficiently large $R_f$, put $U_f=\mathbb R\times\{r>R_f\}$. Then every point of $E$ belongs to $I^-_E(U_f)$, where chronological reachability is by locally absolutely continuous future timelike curves contained in $E$. No timelikeness assumption on the entire designated end, or invariance of a separately defined domain of outer communications under end truncation, is used.

## Statement references

[[def-spacelike-maximal-hypersurface-data]]

[[physics:def-gr-causal-curves-and-reachability]]

[[lem-author-12a8dba09036-inaccessible-set-relative-interior-density]]

[[math:def-axiom-of-choice]]

[[lem-author-12a8dba09036-complete-volume-preserving-shift-flow]]

[[math:def-compact-space]]

## Facts & Assumptions

[A1] The Axiom of Choice is assumed, meeting the foundational hypotheses of the flow, measure and inaccessible-set suppliers. [[math:def-axiom-of-choice]]

[F1] Maximality, Killing's equation and smooth extension of the section and fields across $S$, with $T$ tangent to $S$, give zero shift divergence, boundary tangency and asymptotic decay. [[lem-author-12a8dba09036-maximal-shift-divergence-and-boundary]]

[F2] On a smooth spherical exterior supplied with $F$ and an end chart $x$ whose complements $K_R$ are compact, as explicitly specified in the Statement, a smooth shift up to $S$, tangent there, divergence free and $O(r^{-2})$ on the asymptotically Euclidean end has a complete volume-preserving flow. Borel subsets of bounded exterior annuli $\{p\in C:1<|F(p)|\le L\}$, $L<\infty$, have finite volume even when their closures meet $S$. [[lem-author-12a8dba09036-complete-volume-preserving-shift-flow]]

[F3] For a stationary product with spacelike slices, globally positive lapse and complete $-X$ flow, the inaccessible set is closed and is the closure of its relative interior, and its forward images lie in that interior. Its proof also establishes time-translation invariance of the chronological past of a translation-invariant target. [[lem-author-12a8dba09036-inaccessible-set-relative-interior-density]]

[F4] Finite measure and those exact topological properties force a nonempty-complement inaccessible set to be empty. [[lem-author-12a8dba09036-finite-volume-exact-invariance]]

[F5] The hypersurface convention gives the smooth future unit normal, induced metric, second fundamental form, maximality and lapse–shift splitting. Apply its normal construction on the stipulated smooth spacelike extension near $S$. [[def-spacelike-maximal-hypersurface-data]]

[F6] Chronological past consists of points joined to the target by a locally absolutely continuous future timelike curve in the specified Lorentz manifold. [[physics:def-gr-causal-curves-and-reachability]]

[F7] A compact subset is compact in its subspace topology. Equivalently, every family of ambient open sets covering it has a finite covering subfamily. This applies to the compact sets $K_R$ and the ambient manifold $\overline C$. [[math:def-compact-space]] [[math:lem-compactness-of-a-subspace-is-ambient]]

[F8] A closed subset of $C$ has open complement. The Borel sigma-algebra of $C$ contains every open subset and, being a sigma-algebra, is closed under complements relative to $C$. Hence every closed subset of $C$ is Borel. [[math:def-topological-space]] [[math:def-borel-sigma-algebra]] [[math:def-sigma-algebra]]

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish future chronological access to every sufficiently far stationary tail.

1.1 Choose $R_f$ so large that $g(T,T)=g_{00}<0$ on $U_f$ and $T$ is future directed there. Each point of $U_f$ reaches another point of $U_f$ by a positive time translation, so $U_f\subset I^-_E(U_f)$. Define $B=\{x\in C:(0,x)\notin I^-_E(U_f)\}$. It is disjoint from $\{r>R_f\}$, so its complement is nonempty. [given, F6]

1.2 By [F5] applied to the smooth spacelike extension near $S$, $n$ extends smoothly across $S$. The formulas $N=-g(T,n)$ and $X=T-Nn$ therefore give smooth extensions of the lapse and shift along that slice. Since $T$ is tangent to $S$, orthogonality gives $N|_S=0$ and $X|_S=T|_S\in TS$. Together with maximality, [F1] gives $\operatorname{div}_hX=0$ and $X^i=O(r^{-2})$. Thus the boundary regularity needed by [F1] and [F2] follows from the explicit ambient and slice extensions, rather than from smoothness of $h$ alone. [given, F1, F5, algebra]

2.1 Apply [F2] to obtain a complete flow $\psi_s$ of $-X$ preserving $\mu_h$, which is positive on nonempty open sets. Apply [F3] with this very $U_f$ and the globally positive lapse: $B$ is closed, $B=\overline{\operatorname{int}_CB}^{\,C}$, and $\psi_s(B)\subset\operatorname{int}_CB$ for $s>0$. In particular $B$ is Borel by [F8]. By step 1.1, $B\subset K_{R_f}\cap C$. The sets $\{p\in\overline C:|F(p)|<m\}$ for integers $m\ge2$ form an increasing open cover of the compact $K_{R_f}$, so [F7] gives a finite covering subfamily and hence $|F(p)|<L$ there for some finite $L>1$. Hence $B$ is contained in the bounded exterior annulus $\{p\in C:1<|F(p)|\le L\}$ of [F2], which gives $\mu_h(B)<\infty$ even if $B$ accumulates at $S$. All flow hypotheses are imposed on the original slice up to its boundary; no orbit is extended through a horizon. The choice assumptions of both suppliers are met by [A1]. [given, A1, F2, F3, F7, F8, step 1.1, step 1.2]

3.1 Apply [F4] on the connected $C$ to obtain $B=\varnothing$. Time-translation invariance of $I^-_E(U_f)$ from [F3] extends access from $t=0$ to every point of $E$: translate the timelike curve supplied at $(0,x)$ by $t$ to obtain one from $(t,x)$ to $U_f$. This proves the stated relative-exterior chronological-access assertion without replacing the designated end in the definition of $E$. [F3, F4, F6, step 1.1, step 2.1] ∎

---
id: lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant
title: Smooth transverse horizon branches are the null axes of the normal tube
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - physics:def-gr-future-and-past-sets
  - physics:thm-gr-local-geodesics-and-exponential-map
  - math:thm-flow-box-theorem
  - lem-author-ca4ffba327b3-event-boundary-generator-data
  - lem-author-ca4ffba327b3-compact-normal-exponential-tube
  - physics:def-gr-causal-curves-and-reachability
  - physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets
  - math:def-embedded-smooth-submanifold-with-boundary
  - math:def-smooth-collar-of-a-manifold-boundary
  - physics:lem-gr-chronology-openness
  - math:def-axiom-of-choice
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  physics:def-gr-future-and-past-sets: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  math:thm-flow-box-theorem: mathematical-premise
  lem-author-ca4ffba327b3-event-boundary-generator-data: mathematical-premise
  lem-author-ca4ffba327b3-compact-normal-exponential-tube: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets: mathematical-premise
  math:def-embedded-smooth-submanifold-with-boundary: mathematical-premise
  math:def-smooth-collar-of-a-manifold-boundary: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Work in ZFC in a smooth time-oriented Lorentzian four-manifold $(M,g)$ of signature $(-,+,+,+)$. Let $G=I^-(E)$ and $F_+=I^+(E)$ for a specified open end $E$. Suppose the boundaries $H_+=\partial G$ and $H_-=\partial F_+$ are smooth null hypersurfaces near a compact embedded spacelike two-surface $S$ and intersect transversely precisely in $S$. Let $\Sigma$ be a smooth embedded spacelike hypersurface containing $S$ as a two-sided embedded surface. Specify one side $\Sigma_+\subset\Sigma$ near $S$ as an embedded smooth three-manifold with boundary $S$, with the induced smooth structure and a smooth inward collar $c:S\times[0,\delta)\to\Sigma_+$, $c(s,0)=s$, whose positive-parameter image lies in $G\cap F_+$. Write $n$ for the future unit normal of $\Sigma$ along $S$ and $\nu$ for the inward unit normal to $S$ within $\Sigma_+$. Use the normal tube $\Xi(s,a,b)=\exp_s(a n_s+b\nu_s)$. After shrinking its neighborhood $O$ of $S$, the following equations hold in these coordinates: $H_+\cap O=\{a-b=0\}$, $H_-\cap O=\{a+b=0\}$, $G\cap O=\{a-b<0\}$ and $F_+\cap O=\{a+b>0\}$. Put $\alpha=a+b$ and $\beta=a-b$. The local spacetime exterior $O\cap G\cap F_+$ is the quadrant $\{\alpha>0,\beta<0\}$. For sufficiently small $\delta'>0$, the inward hypersurface collar $c(S\times(0,\delta'))$ lies within this quadrant; its normal coordinates satisfy $b>0$ and $a=O(b^2)$ uniformly along $S$.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-bifurcate-killing-horizon-data]]

[[physics:def-gr-future-and-past-sets]]

[[physics:thm-gr-local-geodesics-and-exponential-map]]

[[math:thm-flow-box-theorem]]

[[lem-author-ca4ffba327b3-event-boundary-generator-data]]

[[lem-author-ca4ffba327b3-compact-normal-exponential-tube]]

[[physics:def-gr-causal-curves-and-reachability]]

[[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]

[[math:def-embedded-smooth-submanifold-with-boundary]]

[[math:def-smooth-collar-of-a-manifold-boundary]]

[[physics:lem-gr-chronology-openness]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

[A1] ZFC supplies the choice assumptions inherited by the causal, geodesic, flow and normal-tube suppliers. No stronger choice principle is used. [[math:def-axiom-of-choice]] [[def-stationary-lorentzian-data]]

[F1] The null generators are pregeodesics orthogonal to and transverse to $S$, and the two event boundaries are achronal. [[lem-author-ca4ffba327b3-event-boundary-generator-data]]

[F2] The normal tube is a diffeomorphism near its zero section, with differential $(X,u,v)\mapsto X+un+v\nu$ there. Geodesics are unique, and a nonzero smooth field has local flow coordinates. [[lem-author-ca4ffba327b3-compact-normal-exponential-tube]] [[physics:thm-gr-local-geodesics-and-exponential-map]] [[math:thm-flow-box-theorem]]

[F3] The chronological relations define $I^\pm$, whose images are open past or future sets. Chronology is open in both endpoints; a past set contains the chronological past of every point of its closure, and the time-reversed assertion holds for a future set. The Lorentzian and null-hypersurface conventions fix the remaining geometry. [[physics:def-gr-causal-curves-and-reachability]] [[physics:def-gr-future-and-past-sets]] [[physics:lem-gr-chronology-openness]] [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]]

[F4] A spacelike hypersurface has positive definite induced metric. An embedded smooth submanifold with boundary carries its specified manifold-with-boundary smooth structure. A smooth collar is an embedding equal to the identity at parameter zero and onto a boundary neighborhood; its parameter derivative is transverse and inward at that boundary. [[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]] [[math:def-embedded-smooth-submanifold-with-boundary]] [[math:def-smooth-collar-of-a-manifold-boundary]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Identify the two event-boundary branches and their sides, and locate the inward hypersurface collar in the local spacetime exterior.

1.1 The two null normal lines at $s\in S$ are spanned by $n_s+\nu_s$ and $n_s-\nu_s$. The radical of each branch is transverse to $S$ by [F1]; its flow coordinates cover a branch neighborhood by its generator curves from $S$. These curves are geodesics up to reparametrization. Uniqueness with the specified initial null directions and [F2] identify the two branches, as an unordered pair locally along $S$, with the images of the axes $a=b$ and $a=-b$. Compactness gives a common shrinking of the tube. [A1, F1, F2]

1.2 For each $s\in S$, the collar velocity lies in $T_s\Sigma$ and decomposes uniquely as $\partial_t c(s,0)=w_s+\lambda(s)\nu_s$, where $w_s\in T_sS$. Its normal coefficient is positive: the collar differential is an isomorphism at the boundary, so the velocity is transverse to $S$, and its positive parameter points into the specified side $\Sigma_+$ in a boundary chart. Thus $\lambda(s)>0$. Write $\Xi^{-1}(c(s,t))=(q(s,t),a(s,t),b(s,t))$. The zero-section differential in [F2] gives $a(s,0)=b(s,0)=0$, $\partial_ta(s,0)=0$ and $\partial_tb(s,0)=\lambda(s)$. Smoothness gives $a(s,t)=O(t^2)$ and $b(s,t)=\lambda(s)t+O(t^2)$ uniformly on compact $S$. Since the smooth positive function $\lambda$ has a positive minimum there, for all sufficiently small $t>0$ one has $b>0$, $a=O(b^2)$, $\alpha=a+b>0$ and $\beta=a-b<0$. Compactness also makes this restricted collar lie in $O$. [given, F2, F4]

2.1 An open past set with smooth boundary occupies the local past side of that boundary. Indeed, if $p\in\partial G$, a point $x_-\ll p$ lies in $G$ by the closure property in [F3]. A point $p\ll x_+$ cannot lie in $\overline G$, since the same property would then put $p$ in the open set $G$, contradicting $p\in\partial G$. Choose these points on a short timelike segment crossing the smooth null boundary. Each connected local side has constant membership: off $\partial G$, the disjoint open sets $G$ and $M\setminus\overline G$ exhaust the neighborhood. This identifies the entire past side with $G$ and the entire future side with its exterior. Time reversal gives the corresponding future-side description of $F_+$. At $S$ the future timelike direction $n$ increases both $a-b$ and $a+b$; by continuity this fixes the future coorientation of either candidate axis near $S$. [F1, F2, F3, step 1.1]

3.1 The inward collar is in $G\cap F_+$ by hypothesis and has $\alpha>0,\beta<0$ by step 1.2. If $H_+$ were the axis $\alpha=0$ at any point of $S$, step 2.1 would place $G$ on its $\alpha<0$ side, contradicting these collar points. Thus $H_+$ is the axis $\beta=0$ everywhere along $S$, and $H_-$ is the other axis $\alpha=0$. Their respective past and future sides give $G\cap O=\{\beta<0\}$ and $F_+\cap O=\{\alpha>0\}$ after a common shrinking. Their intersection is the open four-dimensional spacetime quadrant; the positive-parameter hypersurface collar lies in it with the estimates from step 1.2. This proves all the asserted equations and the collar inclusion. [given, F1, F2, F3, step 1.1, step 1.2, step 2.1] ∎

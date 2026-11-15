---
id: lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries
title: The normal future and past quadrants are the local causal sets of the sphere
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - physics:thm-gr-local-geodesics-and-exponential-map
  - physics:lem-gr-parallel-transport-and-geodesic-speed
  - lem-author-ca4ffba327b3-compact-normal-exponential-tube
  - lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant
  - lem-author-ca4ffba327b3-causal-boundary-barriers
  - physics:def-gr-causal-curves-and-reachability
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  physics:lem-gr-parallel-transport-and-geodesic-speed: mathematical-premise
  lem-author-ca4ffba327b3-compact-normal-exponential-tube: mathematical-premise
  lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant: mathematical-premise
  lem-author-ca4ffba327b3-causal-boundary-barriers: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

In the normal tube and boundary setting of the preceding lemmas, write $\alpha=a+b$, $\beta=a-b$. For the locally absolutely continuous timelike and causal curve conventions, let $I_O^\pm(S)$ and $J_O^\pm(S)$ denote the corresponding futures and pasts of $S$ witnessed by curves lying entirely in $O$. One has $I_O^+(S)=\{\alpha>0,\beta>0\}$ and $J_O^+(S)=\{\alpha\ge0,\beta\ge0\}$, where $J$ includes $S$ by reflexivity. The past versions have both inequalities reversed. Consequently the two null axes $H_+\cup H_-$ form exactly the local null boundary sheets of the causal future and past of $S$.

## Statement references

[[def-stationary-lorentzian-data]]

[[physics:thm-gr-local-geodesics-and-exponential-map]]

[[physics:lem-gr-parallel-transport-and-geodesic-speed]]

[[lem-author-ca4ffba327b3-compact-normal-exponential-tube]]

[[lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant]]

[[lem-author-ca4ffba327b3-causal-boundary-barriers]]

[[physics:def-gr-causal-curves-and-reachability]]

## Facts & Assumptions

[F1] The normal tube is diffeomorphic and star shaped in its normal variables. Its event boundaries and chronological-set sides are the stated axes and quadrants. [[lem-author-ca4ffba327b3-compact-normal-exponential-tube]] [[lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant]]

[F2] Curves from $S$ obey the two chronological boundary barriers. [[lem-author-ca4ffba327b3-causal-boundary-barriers]]

[F3] Geodesics preserve their metric norm and future/past character, and the normal radial geodesic has its prescribed initial tangent. [[physics:thm-gr-local-geodesics-and-exponential-map]] [[physics:lem-gr-parallel-transport-and-geodesic-speed]] [[def-stationary-lorentzian-data]]

[F4] Timelike and causal curves are locally absolutely continuous, with nonzero appropriately directed timelike or causal velocity almost everywhere. The sets $I^\pm(S)$ and $J^\pm(S)$ are unions of pointwise chronological and causal reachability sets over $S$, and causal reachability also allows equality. The subscript $O$ restricts the witnessing curves to $O$. [[physics:def-gr-causal-curves-and-reachability]]

## Proof

**Given:**The data and hypotheses in the Statement.

**Goal:** Establish the stated conclusions under exactly those hypotheses.

1.1 A future timelike curve from any $p\in S$ ends outside $\overline G$ and inside $F_+$ by [F2]. The side equations [F1] give $\beta>0$ and $\alpha>0$. For a future causal curve, the weak barriers give $\beta\ge0$ and $\alpha\ge0$. These are necessary conditions for the local chronological and causal future. [F1, F2, F4]

2.1 Conversely, if both coordinates are positive then the initial normal vector $an+b\nu$ has $a>|b|$, so is future timelike. Its radial geodesic lies in $O$ by [F1], remains future timelike by [F3], and joins its base point in $S$ to the specified endpoint. For weak inequalities the same vector is future causal or zero, so its future causal radial geodesic (timelike in the interior and null on a nonzero axis), or reflexive reachability at $S$ when the vector is zero, gives membership in $J_O^+(S)$ by [F4]. The past assertions follow by changing the signs of $a,b$. Since $\Xi$ is a homeomorphism, the boundaries of these quadrants are exactly their null axes in the respective future/past halves. [F1, F3, F4, step 1.1] ∎

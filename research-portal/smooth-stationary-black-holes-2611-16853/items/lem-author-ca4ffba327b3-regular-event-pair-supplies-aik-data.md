---
id: lem-author-ca4ffba327b3-regular-event-pair-supplies-aik-data
title: Regular stationary event branches supply the local AIK horizon pair
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - def-author-254b7c4bab6d-regular-null-horizon-pair
  - lem-author-ca4ffba327b3-event-boundary-generator-data
  - lem-author-ca4ffba327b3-compact-normal-exponential-tube
  - lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant
  - lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries
  - def-null-screen-expansion-and-focal-data
  - physics:def-gr-causal-curves-and-reachability
  - math:def-embedded-smooth-submanifold-with-boundary
  - math:def-smooth-collar-of-a-manifold-boundary
  - physics:thm-gr-local-geodesics-and-exponential-map
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  def-author-254b7c4bab6d-regular-null-horizon-pair: mathematical-premise
  lem-author-ca4ffba327b3-event-boundary-generator-data: mathematical-premise
  lem-author-ca4ffba327b3-compact-normal-exponential-tube: mathematical-premise
  lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant: mathematical-premise
  lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  math:def-embedded-smooth-submanifold-with-boundary: mathematical-premise
  math:def-smooth-collar-of-a-manifold-boundary: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 4
---

## Statement

Work in ZFC on a connected oriented smooth time-oriented Lorentzian four-manifold $(M,g,N)$ of signature $(-,+,+,+)$, with its Levi–Civita connection. Let $E\subseteq M$ be a specified open end and $O_0\subseteq M$ an open neighborhood of a compact embedded spacelike two-sphere $S$. Compute $I^\pm(E)$ in $M$ using the locally absolutely continuous timelike-curve convention. Suppose $H_+=O_0\cap\partial I^-(E)$ and $H_-=O_0\cap\partial I^+(E)$ are smooth embedded null hypersurfaces without boundary in $O_0$, with $H_+\cap H_-=S$ and $T_sH_++T_sH_-=T_sM$ for every $s\in S$. Boundaries here are taken in $M$.

Let $\Sigma$ be a smooth embedded spacelike hypersurface containing $S$ as a two-sided embedded surface. Specify a side $\Sigma_+\subset\Sigma$ near $S$ as a smooth embedded three-manifold with boundary $S$, with its induced smooth structure and positive definite induced metric up to $S$. Supply a smooth inward collar $c:S\times[0,\delta)\to\Sigma_+$, with $\delta>0$, $c(s,0)=s$, and $c(S\times(0,\delta))\subset O_0\cap I^-(E)\cap I^+(E)$.

Assume each full branch $H_\pm$ is non-expanding in the null-screen convention, including both halves through $S$ and $S$ itself. Then there is a connected open neighborhood $O\subseteq O_0$ of $S$ such that $H_+\cap O$, $H_-\cap O$ and $S$ satisfy the regular bifurcate non-expanding pre-rigidity horizon-pair definition, with all local causal curves confined to $O$. No Killing generator on either branch is assumed in this reduction. It asserts no global extension of any symmetry.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-bifurcate-killing-horizon-data]]

[[def-author-254b7c4bab6d-regular-null-horizon-pair]]

[[lem-author-ca4ffba327b3-event-boundary-generator-data]]

[[lem-author-ca4ffba327b3-compact-normal-exponential-tube]]

[[lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant]]

[[lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries]]

[[def-null-screen-expansion-and-focal-data]]

[[physics:def-gr-causal-curves-and-reachability]]

[[math:def-embedded-smooth-submanifold-with-boundary]]

[[math:def-smooth-collar-of-a-manifold-boundary]]

## Facts & Assumptions

[F1] The Lorentzian and null-hypersurface conventions give the metric, time orientation, connection, null radical and transverse spacelike surface used here. The regular pre-rigidity pair definition requires full achronal sheets with signed affine generators meeting the sphere once, the two relative causal-boundary identities, and zero expansion on both full sheets. [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]] [[def-author-254b7c4bab6d-regular-null-horizon-pair]]

[F2] Chronological and causal reachability use locally absolutely continuous curves with nonzero appropriately directed velocity almost everywhere; causal reachability also allows equality. The collar is a smooth embedding equal to the identity at parameter zero and onto a boundary neighborhood in the supplied manifold-with-boundary structure. [[physics:def-gr-causal-curves-and-reachability]] [[math:def-embedded-smooth-submanifold-with-boundary]] [[math:def-smooth-collar-of-a-manifold-boundary]]

[F3] For a common open end and the stated transverse chronological-boundary identities, the event-boundary lemma supplies achronality and null geodesic generators orthogonal and transverse to $S$. A compact spacelike surface with the specified spacelike side has the future/inward orthonormal normal frame and a uniform normal exponential tube. [[lem-author-ca4ffba327b3-event-boundary-generator-data]] [[lem-author-ca4ffba327b3-compact-normal-exponential-tube]]

[F4] With these same boundary identities and a positive-parameter collar in $I^-(E)\cap I^+(E)$, the axis lemma identifies the two event branches and their chronological sides in the tube. The quadrant lemma then identifies the relative chronological and causal futures and pasts of $S$ in that tube. [[lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant]] [[lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries]]

[F5] Null expansion is the trace of the null second fundamental form on transverse spacelike sections. The non-expansion hypothesis is imposed on each full branch as required by the pre-rigidity definition. [[def-null-screen-expansion-and-focal-data]] [[def-author-254b7c4bab6d-regular-null-horizon-pair]]

[F6] For the supplied smooth time-oriented Lorentzian four-manifold with its Levi–Civita connection, the geodesic initial-value theorem defines $\exp_s(v)=\gamma_{s,v}(1)$ and gives $\gamma_{s,tv}(1)=\gamma_{s,v}(t)$ whenever these expressions are defined. The curve $\gamma_{s,v}$ is a geodesic in its affine parameter, with initial velocity $v$. [[physics:thm-gr-local-geodesics-and-exponential-map]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Verify every condition of the regular bifurcate non-expanding pre-rigidity horizon-pair definition.

1.1 Apply the event-boundary supplier in [F3] with the specified open end $E$, open set $O_0$ and exact identities for $H_\pm$ in the Statement. Its smoothness, nullness, spacelike-intersection and transversality hypotheses are precisely assumed here. Thus each full branch is achronal in $O_0$ and, near $S$, is generated by null geodesics orthogonal and transverse to $S$. Achronality remains true when the allowed timelike curves are confined to any smaller open neighborhood. [given, F1, F2, F3]

2.1 The supplied $\Sigma_+$ is a smooth embedded spacelike three-manifold with boundary $S$ and positive induced metric up to that boundary. The compact normal-tube supplier in [F3] therefore gives the smooth orthonormal frame $(n,\nu)$ along $S$, with $n$ the future unit normal of $\Sigma$ and $\nu$ the inward unit boundary normal, and the diffeomorphism $\Xi(s,a,b)=\exp_s(an_s+b\nu_s)$ on $|a|+|b|<\epsilon$. Shrink its radius so its image lies in $O_0$. The common end, exact intersection, two-sided hypersurface and inward collar inclusion assumed here are all the hypotheses of the axis lemma in [F4]. After its common shrinking, in the resulting tube $O$ one has $H_+\cap O=\{a-b=0\}$, $H_-\cap O=\{a+b=0\}$, $I^-(E)\cap O=\{a-b<0\}$ and $I^+(E)\cap O=\{a+b>0\}$. [given, F1, F2, F3, F4, step 1.1]

3.1 The tube and chronological-boundary setting of the quadrant lemma in [F4] have now been established with the same $E$, branches and frame. Put $\alpha=a+b$ and $\beta=a-b$. That lemma gives $I_O^+(S)=\{\alpha>0,\beta>0\}$ and $J_O^+(S)=\{\alpha\ge0,\beta\ge0\}$, including reflexive reachability at $S$; the past sets have both inequalities reversed. Since $\Xi$ is a diffeomorphism, the relative boundary of the closed future quadrant is its two nonnegative axes, and its difference from the open future quadrant is the same set. The analogous statement holds for the nonpositive axes in the past quadrant. These are the two relative-boundary and $J_O^\pm(S)\setminus I_O^\pm(S)$ identities required in [F1], with curves confined to $O$ throughout. [F1, F2, F4, step 2.1]

4.1 In this tube the full axes are parametrized by $t\mapsto\Xi(s,t,t)$ and $t\mapsto\Xi(s,t,-t)$, with $|t|<\epsilon/2$. By the exponential-map definition and scaling law in [F6], these curves are $\exp_s(t(n_s+\nu_s))=\gamma_{s,n_s+\nu_s}(t)$ and $\exp_s(t(n_s-\nu_s))=\gamma_{s,n_s-\nu_s}(t)$, respectively. Thus $t$ is an affine parameter, with respective initial velocities $n_s+\nu_s$ and $n_s-\nu_s$. The event-boundary and axis constructions identify their images with the null generators of the branches. Both initial directions are future-directed; the increasing affine parameter is future-directed on each generator. Injectivity of $\Xi$ makes each generator meet $S$ exactly at $t=0$, an interior point of its connected parameter interval. Thus the nonnegative and nonpositive axes in step 3.1 are exactly the future and past halves of the supplied full sheets, with no extra generator or boundary component. [F1, F3, F4, F6, step 1.1, step 2.1, step 3.1]

5.1 The tube $O$ is connected because it is diffeomorphic to the product of the connected sphere with the connected normal diamond, and it inherits the ambient orientation. The branches are embedded smooth null hypersurfaces without boundary in $O$, intersecting transversely exactly in $S$, and they are achronal by step 1.1. The assumed zero expansions on both full branches persist under restriction to $O$. Together with steps 3.1–4.1 these verify every condition of the regular bifurcate non-expanding pre-rigidity pair in [F1]. No branch-generating Killing field or global symmetry-extension assertion entered the argument. [given, F1, F3, F5, step 1.1, step 2.1, step 3.1, step 4.1] ∎

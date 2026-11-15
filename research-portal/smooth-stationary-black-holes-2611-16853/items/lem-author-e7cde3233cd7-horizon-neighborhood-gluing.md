---
id: lem-author-e7cde3233cd7-horizon-neighborhood-gluing
title: Extending a closed one-form potential across a bifurcation sphere
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - math:def-axiom-of-choice
  - math:thm-tubular-neighbourhood-theorem-in-a-smooth-ambient-manifold
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:thm-de-rham-cohomology-of-spheres
  - math:thm-de-rham-cohomology-is-smooth-homotopy-invariant
  - math:def-de-rham-cohomology
  - math:def-closed-and-exact-differential-forms
  - lem-author-e7cde3233cd7-spherical-cauchy-portion
  - physics:def-gr-smooth-lorentzian-objects
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-causal-curve-calculus
  - math:lem-ac-supplies-countable-and-dependent-choice-for-banach-integration
  - math:lem-smooth-bump-between-concentric-euclidean-balls
  - math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-tubular-neighbourhood-theorem-in-a-smooth-ambient-manifold: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:thm-de-rham-cohomology-of-spheres: mathematical-premise
  math:thm-de-rham-cohomology-is-smooth-homotopy-invariant: mathematical-premise
  math:def-de-rham-cohomology: mathematical-premise
  math:def-closed-and-exact-differential-forms: mathematical-premise
  lem-author-e7cde3233cd7-spherical-cauchy-portion: mathematical-premise
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  math:lem-ac-supplies-countable-and-dependent-choice-for-banach-integration: mathematical-premise
  math:lem-smooth-bump-between-concentric-euclidean-balls: mathematical-premise
  math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references: []
dependency_level: 4
---

## Statement

Work in ZFC and assume the geometric hypotheses of the spherical Cauchy-portion lemma. Suppose near the compact sphere $S$ the two chronological boundaries are smooth transverse null hypersurfaces intersecting in $S$. Here a smooth null hypersurface means a smooth embedded hypersurface whose induced metric is positive semidefinite with a one-dimensional kernel; transverse means that the two tangent hyperplanes span the ambient tangent space at every point of $S$. There is a connected neighborhood $O$ of $S$ retracting smoothly to $S$, with $E\cap O$ connected. If a smooth closed real or complex one-form $\eta$ is defined on the ambient spacetime and has a primitive $s_E$ on $E$, then $s_E$ extends to a smooth primitive on $E\cup O$.

## Statement references

[[lem-author-e7cde3233cd7-spherical-cauchy-portion]]

[[def-causal-exterior-and-boundary-data]]

[[physics:def-gr-smooth-lorentzian-objects]]

[[math:def-axiom-of-choice]]

[[math:def-closed-and-exact-differential-forms]]

## Facts & Assumptions

[F1] The causal and ambient-boundary conventions are [[def-causal-exterior-and-boundary-data]]. In particular $E=P\cap Q$, where $P=I_D^-(U)$ and $Q=I_D^+(U)$. The time-orientation field $N$ is smooth and future timelike everywhere, as in [[physics:def-gr-smooth-lorentzian-objects]]. Work in ZFC, including [[math:def-axiom-of-choice]].

[F2] The spherical Cauchy-portion data give the embedded sphere $S=\chi(\{|x|=1\})$ and the exterior portion $C=\chi(\{|x|>1\})$. [[lem-author-e7cde3233cd7-spherical-cauchy-portion]]

[F3] A closed embedded submanifold has a tubular neighborhood; a smooth map with invertible differential has a local smooth inverse. [[math:thm-tubular-neighbourhood-theorem-in-a-smooth-ambient-manifold]] [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[F4] Smooth homotopy equivalences preserve de Rham cohomology, $H^1_{\mathrm{dR}}(S^2)=0$, and a zero cohomology class of a closed one-form means exactness. [[math:thm-de-rham-cohomology-is-smooth-homotopy-invariant]] [[math:thm-de-rham-cohomology-of-spheres]] [[math:def-de-rham-cohomology]] [[math:def-closed-and-exact-differential-forms]]

[F5] Chronological futures and pasts of points are open. If $P_0$ is a past set and $p\in\overline{P_0}$, then $I_D^-(p)\subset P_0$; if $Q_0$ is a future set and $p\in\overline{Q_0}$, then $I_D^+(p)\subset Q_0$. These are clauses (a) and (c) of [[physics:lem-gr-chronology-openness]], applied to the ambient manifold $D$.

[F6] Smooth future timelike arcs are admissible timelike curves, and finite concatenations of timelike curves remain timelike, by clauses (c) and (d) of [[physics:lem-gr-causal-curve-calculus]]. In particular, $\ll_D$ is transitive.

[F7] Given $0<r<R$ in a Euclidean chart, there is a smooth $[0,1]$-valued bump equal to one on the closed radius-$r$ ball and supported in the radius-$R$ ball. [[math:lem-smooth-bump-between-concentric-euclidean-balls]]

[F8] A smooth real function with zero differential is constant on every connected component. [[math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component]]

[F9] AC implies Countable Choice and prescribed-initial-point Dependent Choice by [[math:lem-ac-supplies-countable-and-dependent-choice-for-banach-integration]]. Thus ZFC supplies the choice hypotheses of [F3], [F4], [F5] and [F6].

## Proof

**Given:** The geometric data and closed one-form in the Statement, in ZFC, with the stated inline null-hypersurface and transversality conventions.

**Goal:** Construct the neighborhood and extend the given primitive without assuming that $\Sigma$ is spacelike at $S$.

1.1 The choice requirements are supplied by [F9]. By [F5], $P$ and $Q$ are open unions of chronological pasts and futures of points. Transitivity from [F6] makes $P$ a past set and $Q$ a future set. If $p\in\partial_D P$ and a short smooth future timelike arc $\gamma$ passes through $p=\gamma(0)$, then for $t<0$ clause (c) in [F5] gives $\gamma(t)\in P$. For $t>0$, $\gamma(t)\in\overline P$ would imply $p\in I_D^-(\gamma(t))\subset P$, contrary to $p\in\partial_D P$ and openness of $P$. Thus the positive-time side is outside $\overline P$. Reversing time proves that at $p\in\partial_D Q$ the positive-time side lies in $Q$ and the negative-time side is outside $\overline Q$. [given, F1, F5, F6, F9]

2.1 Write $H_P=\partial_D P$ and $H_Q=\partial_D Q$ near $S$. By the inline definition their tangent spaces contain no timelike vectors, so $N$ is transverse to each. At any point of either boundary choose local coordinates $(y,t)$ for which $\partial_t$ is future timelike throughout a small box: start with a linear coordinate change making it equal to $N$ at the point, then shrink using the strict timelikeness and orientation inequalities. For a local defining function $h$ of the embedded hypersurface, $\partial_t h\ne0$ there; [F3] applied to $(y,t)\mapsto(y,h(y,t))$ expresses the boundary as a smooth graph $t=a(y)$ after shrinking. Each vertical segment through that graph is an arc of step 1.1. Consequently $r_i=a(y)-t$ is positive exactly on $P$ in a box for $H_P$, and $r_i=t-a(y)$ is positive exactly on $Q$ in a box for $H_Q$. Their zeros are exactly the respective boundaries. Their differentials on $N$ along the boundary are respectively negative and positive, since the kernel is the boundary tangent hyperplane and $N$ and $\partial_t$ lie in the same timelike component. [given, F1, F3, F6, step 1.1]

3.1 For each boundary separately, cover $S$ by finitely many smaller coordinate balls whose closures lie in boxes of step 2.1. Choose bumps $b_i$ from [F7] supported in those boxes and equal to one on the smaller balls. Extend each bump and each product $b_i r_i$ by zero outside its box; these extensions are smooth because their supports stay inside the box. On the open neighborhood $W=\{\sum_i b_i>0\}$ of $S$, set $r=(\sum_i b_i r_i)/(\sum_i b_i)$. Every active $r_i$ has the same sign: positive in the chronological set, zero on its boundary, and negative outside its closure. Thus $r$ has exactly those signs and zeros. On the boundary, terms involving derivatives of the weights vanish because $r_i=0$, and $dr(N)$ is a weighted average of strictly negative numbers for $P$, or strictly positive numbers for $Q$; it is nonzero. This constructs smooth defining functions $u$ for $H_P$ and $v$ for $H_Q$ on a common neighborhood of $S$, with $P=\{u>0\}$ and $Q=\{v>0\}$ there. Transversality makes $du,dv$ independent along $S$, with common kernel $TS$. No normal to $\Sigma$ has been used. [given, F1, F2, F7, step 2.1]

4.1 The compact embedded sphere $S$ is closed in the Hausdorff ambient manifold, so [F3] supplies a tubular projection $\pi$ near $S$. For $G=(\pi,u,v)$, $dG$ is invertible along $S$: $du,dv$ have common kernel $TS$, and $d\pi$ is the identity on $TS$. Shrink the tube so that $G$ is a local diffeomorphism throughout it. It is injective after a further shrinking towards the compact zero section. Indeed, otherwise there are unequal pairs with the same image tending to the zero section. Their equal $\pi$ coordinates and compactness give a subsequence with both points tending to the same point of $S$. Both eventually lie in one inverse chart of [F3], a contradiction. Hence $G$ is a diffeomorphism onto an open neighborhood of $S\times\{(0,0)\}$ in $S\times\mathbb R^2$. Compactness supplies $\delta>0$ for which this image contains $S\times(-\delta,\delta)^2$. [F2, F3, step 3.1]

5.1 Let $O=G^{-1}(S\times(-\delta,\delta)^2)$ in that injective tube. This is a connected open neighborhood of $S$. In these coordinates the homotopy $(p,u,v)\mapsto(p,(1-t)u,(1-t)v)$, for $0\le t\le1$, is a smooth deformation retraction to $S$. By step 3.1 and $E=P\cap Q$, its exterior overlap is exactly $S\times(0,\delta)^2$, which is nonempty and connected. This is the same exterior side that meets $C=\chi(\{|x|>1\})$ in [F2]. [F1, F2, step 3.1, step 4.1]

6.1 By [F4] and step 5.1, $H^1_{\mathrm{dR}}(O)\cong H^1_{\mathrm{dR}}(S^2)=0$, so $\eta|_O=\mathrm ds_O$ for a smooth real potential; for a complex form apply this to its real and imaginary parts. On the connected open overlap, $\mathrm d(s_O-s_E)=0$. By [F8], applied separately to real and imaginary parts if necessary, the difference is one constant. Subtract that constant from $s_O$. The two potentials now agree on their open overlap and therefore define one smooth function on $E\cup O$ with differential $\eta$, extending the specified $s_E$. [given, F4, F8, step 5.1] ∎

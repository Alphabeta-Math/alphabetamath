---
title: Indexed compact heights and uniform smooth horizon collars
status: draft
research_item: pthm-author-048251387164-indexed-height-and-horizon-estimates
dependency_level: 17
sources:
  references:
    - title: Leon Simon, Lectures on PDE
      url: https://math.stanford.edu/~lms/lecs-on-pde.pdf
      locator: Lecture 18, Theorem 2 (C^{1,beta} estimate, boundary), printed p.217,
        assumptions (P), (*) and (**) on pp.216–217; PDF sheet111
      statement: Let u be a C2 solution of a^{ij}(x,u,Du)u_ij=f on a boundary patch,
        with u=0 on the actual boundary, bounded |u|+R|Du|, bounded f, C1 joint
        bounds on a^{ij} in a containing position/height/slope box, positive
        uniform ellipticity on that box, and a C2 boundary-flattening
        diffeomorphism and inverse with bounded norms. On every smaller patch
        there is a uniform C^{1,beta} bound, for some beta in (0,1), with
        constants controlled by dimension, shrinking factor, the height/gradient
        bound, structural coefficient/ellipticity constants and the flattening
        constants. The analogous interior statement is Theorem 1 on the same
        page.
      hypotheses: Classical C2 solution, C1 joint principal coefficients, bounded RHS,
        uniform positive ellipticity on the containing slope/height box, a
        common finite height/gradient bound and uniformly C2 flattenable
        boundary; homogeneous Dirichlet trace on the actual boundary portion.
        Bounds are local and do not require any condition at the remote
        spherical edge of the patch.
      reading_limits: "Retained prior source-input or attribution record: Current
        adjudication read the online Simon PDF text at PDF page 111 (zero-based
        110), printed pp.216–217: problem (P), bounds (*) and (**), and the
        interior and boundary C1-beta Theorems 1–2. The containing coefficient
        box, bounded forcing, solution height/gradient bound and C2 flattening
        hypotheses were compared with Proof 7.1 and its existing
        operator/extension suppliers. No proof reconstruction or fresh reading
        of printed p.222 is claimed. The estimate is imported; the subsequent
        bootstrap is local composition. Fresh maintenance limits: current item
        and supplier contracts and the local applications were checked; no new
        reading of the external proof or PDF images is claimed."
---

## Prerequisites

- [pthm-author-048251387164-indexed-admissible-end-estimates](item-pthm-author-048251387164-indexed-admissible-end-estimates)
- [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product)
- [pthm-timelike-path-transfer](item-pthm-timelike-path-transfer)
- [pthm-common-reference-collar](item-pthm-common-reference-collar)
- [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)
- [pthm-hawking-graph-height](item-pthm-hawking-graph-height)
- [pthm-hawking-graph-barriers](item-pthm-hawking-graph-barriers)
- [lem-author-66066dbaeb16-boundary-spacelike-tangency-comparison](item-lem-author-66066dbaeb16-boundary-spacelike-tangency-comparison)
- [lem-author-840894718169-fixed-boundary-flow-normal-boost](item-lem-author-840894718169-fixed-boundary-flow-normal-boost)
- [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone)
- [lem-author-840894718169-normal-projection-local-and-boundary-jets](item-lem-author-840894718169-normal-projection-local-and-boundary-jets)
- [lem-author-840894718169-fixed-target-collar-properness](item-lem-author-840894718169-fixed-target-collar-properness)
- [lem-author-840894718169-boundary-one-sheet-normal-graph](item-lem-author-840894718169-boundary-one-sheet-normal-graph)
- [lem-author-14de055b8ceb-gaussian-cutoff-projection](item-lem-author-14de055b8ceb-gaussian-cutoff-projection)
- [lem-author-14de055b8ceb-weighted-cutoff-maximum](item-lem-author-14de055b8ceb-weighted-cutoff-maximum)
- [lem-author-14de055b8ceb-gaussian-maximal-graph-operator](item-lem-author-14de055b8ceb-gaussian-maximal-graph-operator)
- [lem-author-14de055b8ceb-uniform-elliptic-jet-extension](item-lem-author-14de055b8ceb-uniform-elliptic-jet-extension)
- [lem-author-14de055b8ceb-boundary-seeded-schauder-bootstrap](item-lem-author-14de055b8ceb-boundary-seeded-schauder-bootstrap)
- [lem-author-56ff511785bf-full-range-log-angle](item-lem-author-56ff511785bf-full-range-log-angle)
- [pthm-horizon-invariant-one-form](item-pthm-horizon-invariant-one-form)
- [def-harrison-one-form-family](item-def-harrison-one-form-family)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [physics:thm-gr-convex-normal-neighborhoods](https://alphabetamath.cc/physics/item/thm-gr-convex-normal-neighborhoods)
- [physics:thm-gr-normal-neighborhood-causal-cone](https://alphabetamath.cc/physics/item/thm-gr-normal-neighborhood-causal-cone)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-12a8dba09036-maximal-stationary-far-tail-access](item-lem-author-12a8dba09036-maximal-stationary-far-tail-access)
- [` Leon Simon, Lectures on PDE · Lecture 18, Theorem 2 (C^{1,beta} estimate, boundary), printed p.217, assumptions (P), (*) and (**) on pp.216–217; PDF sheet111 `](https://math.stanford.edu/~lms/lecs-on-pde.pdf)


## Statement

For any indexed set $\mathcal I$ of individually admissible sections as above, stationary heights have uniform bounds on every compact subset of the reference interior. Candidate Hawking-flow heights are uniformly bounded down to $S$ on one common collar. On a smaller common collar every section is a one-to-one normal graph with zero boundary height, uniform strict spacelikeness and uniform Ck-alpha bounds for every finite k and $\alpha<1$. These conclusions hold for the pairs actually present in $\mathcal I$; no section is required at an unrepresented parameter.

## Facts & Assumptions

[F1] The admissible indexed pairs and common end/lapse estimates are [pthm-author-048251387164-indexed-admissible-end-estimates](item-pthm-author-048251387164-indexed-admissible-end-estimates). The original stationary product and transferred future timelike paths are [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product) and [pthm-timelike-path-transfer](item-pthm-timelike-path-transfer).

[F2] The common reference collar and fixed-q Hawking-height existence/smooth extension are [pthm-common-reference-collar](item-pthm-common-reference-collar) and [pthm-hawking-graph-height](item-pthm-hawking-graph-height). Only the unconditional strict barrier geometry of [pthm-hawking-graph-barriers](item-pthm-hawking-graph-barriers) is used, not its interval-family uniform conclusion. The contact comparison is [lem-author-66066dbaeb16-boundary-spacelike-tangency-comparison](item-lem-author-66066dbaeb16-boundary-spacelike-tangency-comparison).

[F3] The generic boost, Gaussian cone, local projection, properness and one-sheet lemmas apply to any candidates whose heights have a common bound. [lem-author-840894718169-fixed-boundary-flow-normal-boost](item-lem-author-840894718169-fixed-boundary-flow-normal-boost) [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone) [lem-author-840894718169-normal-projection-local-and-boundary-jets](item-lem-author-840894718169-normal-projection-local-and-boundary-jets) [lem-author-840894718169-fixed-target-collar-properness](item-lem-author-840894718169-fixed-target-collar-properness) [lem-author-840894718169-boundary-one-sheet-normal-graph](item-lem-author-840894718169-boundary-one-sheet-normal-graph)

[F4] The local full-range log-angle theorem and cutoff/projection maximum lemmas apply to the individual maximal graphs in the smooth compact background. [lem-author-56ff511785bf-full-range-log-angle](item-lem-author-56ff511785bf-full-range-log-angle) [lem-author-14de055b8ceb-gaussian-cutoff-projection](item-lem-author-14de055b8ceb-gaussian-cutoff-projection) [lem-author-14de055b8ceb-weighted-cutoff-maximum](item-lem-author-14de055b8ceb-weighted-cutoff-maximum) The Gaussian operator, elliptic extension and seeded boundary bootstrap are [lem-author-14de055b8ceb-gaussian-maximal-graph-operator](item-lem-author-14de055b8ceb-gaussian-maximal-graph-operator), [lem-author-14de055b8ceb-uniform-elliptic-jet-extension](item-lem-author-14de055b8ceb-uniform-elliptic-jet-extension) and [lem-author-14de055b8ceb-boundary-seeded-schauder-bootstrap](item-lem-author-14de055b8ceb-boundary-seeded-schauder-bootstrap).

[F5] Import the exact Simon homogeneous-Dirichlet boundary C1-beta estimate recorded in the source metadata. Its bounded height/gradient, C1 full coefficient-box, uniform ellipticity, bounded forcing and smooth boundary-chart hypotheses will be verified after the angle bound.

[F6] The regular data are in ZFC and define $\mathcal E=I_M^-(M^{\mathrm{end}})\cap I_M^+(M^{\mathrm{end}})$, with $T$ future timelike sufficiently far out. Each exterior point both reaches and is reached from the designated end; access to a sufficiently far tail will instead use [F10], without assuming timelikeness throughout that designated end. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) Chronological openness permits endpoint neighborhoods; the causal-curve calculus supplies finite concatenation and transitivity. [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness) [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus) Convex normal neighborhoods and their timelike exponential-cone characterization let us replace a timelike curve by finitely many smooth timelike geodesic pieces, and vary its last or first piece smoothly near an endpoint. [physics:thm-gr-convex-normal-neighborhoods](https://alphabetamath.cc/physics/item/thm-gr-convex-normal-neighborhoods) [physics:thm-gr-normal-neighborhood-causal-cone](https://alphabetamath.cc/physics/item/thm-gr-normal-neighborhood-causal-cone) These are mathematical suppliers, including those stored in the physics namespace; their Countable Choice and Dependent Choice hypotheses are met in the inherited ZFC convention. We declare the axiom of choice explicitly for these causal inputs and the path selections in steps 1.1 and 2.1. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F7] Use the single smooth stationary primitive $W_0$ on the exterior supplied by [pthm-horizon-invariant-one-form](item-pthm-horizon-invariant-one-form), with the same normalized pole and the same family $W_q=(1-q)^2W_0-4q(1-q)T^\flat$ as in [def-harrison-one-form-family](item-def-harrison-one-form-family). This is the chosen family of the standing Harrison construction, not independently chosen gauges for different candidates. At its pole $T_p=0$, the normalization gives $d_q=(1+q)^2+(1-q)^2\psi(p)^2\ge1$. [def-harrison-normalization](item-def-harrison-normalization)

[F8] The stationary graph, its original height $u$, and its normalized end height obey $\widetilde u(qx)=d_qu(x)/(4q)$. [def-stationary-maximal-graph](item-def-stationary-maximal-graph) The $C^{k,\alpha}$ bounds mean the coordinate Hölder norms on fixed finite collar charts, including continuous derivative extensions to the actual boundary. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F9] Near $S$, the same fields satisfy $K=T+\Omega_HZ$ and commute, and $Z$ generates a smooth circle action of period $2\pi$. [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields) The complete extensions in [F2] agree with these local fields; only axial orbits inside their common local symmetry neighborhood will be used.

[F10] In a smooth stationary product over a maximal spherical exterior with compact boundary, positive original lapse, smooth ambient extension across that boundary with tangent $T$, and a physical asymptotically Euclidean end whose truncations are compact, every point reaches any sufficiently far stationary tail by a future original-metric timelike curve inside the product. This geometric input also applies after reversing time orientation and replacing $T$ by $-T$. [lem-author-12a8dba09036-maximal-stationary-far-tail-access](item-lem-author-12a8dba09036-maximal-stationary-far-tail-access)

## Proof

**Given:** An arbitrary indexed collection of individually admissible existing sections. **Goal:** Obtain common compact heights and boundary collar estimates.

1.1 If the indexed family is empty, all candidate estimates are vacuous; choose a smaller background reference collar from [F2]. An empty compact target set also has a vacuous height bound. For the path argument assume the family and the target set are nonempty. Let $Q\Subset\Sigma_1^\circ$ be compact, identified with $\{0\}\times Q$ using [F1]. Apply the original product result in [F1] to the actual maximal exterior section: its closure is a connected smooth spherical exterior with compact boundary $S$, its induced positive metric is smooth up to $S$, its physical end has $h_{ij}=\delta_{ij}+O_6(r^{-1})$ and compact truncations, and its original lapse is positive. The regular data in [F6] give the ambient smooth spacelike extension across $S$, tangency of $T$ there, and the remaining stationary end bounds. Shrink only the coordinate tail past the compact-truncation threshold, retaining the same exterior product. These are the hypotheses of [F10]. Choose a fixed physical radius $R_*$ sufficiently large for that input and so that $r\ge R_*$ belongs to the common normalized end in [F1] for every $q\in[\delta,1]$. For each $y\in Q$, [F10] supplies a future timelike path from $(0,y)$ to a point $b_y$ with $r>R_*$. Apply the same input with reversed time orientation, stationary coordinate $a=-t$, field $T'=-T$, and normal $n'=-n$. Its lapse is still $-g(T',n')=N>0$, its shift is $-X$, its second fundamental form is $-k$ and it remains maximal; $g_{00}$ and $g_{ij}$ are unchanged and the mixed end components change sign. All decay, compactness, smoothness and boundary-tangency hypotheses are therefore retained. Reversing the resulting curve gives a future original-metric timelike path from a point $a_y$ with $r>R_*$ to $(0,y)$. Both paths lie entirely in the original exterior and both endpoints lie in the common end-height region. No equality of chronological exteriors after end truncation or timelikeness on the entire originally designated end is assumed. [F1, F2, F6, F10, given, choose]

2.1 Subdivide each path into finitely many convex normal neighborhoods contained in $\mathcal E$ and replace each subarc by its smooth future timelike geodesic, using [F6]. Near $(0,y)$ keep the penultimate incoming and the first outgoing points fixed and vary only the joining geodesic to $(0,z)$. The exponential-cone characterization and chronological openness give a neighborhood of $y$ where both geodesics remain future timelike. Shrink to a neighborhood with compact closure inside that neighborhood. The varying geodesics and their velocities are smooth on this compact endpoint set times $[0,1]$, and all other pieces are fixed. A finite subcover of $Q$ therefore gives finitely many piecewise smooth path families $\gamma^-_z:a_i\to(0,z)$ and $\gamma^+_z:(0,z)\to b_i$, with fixed end endpoints, compact image and uniformly bounded coordinate velocities on their finitely many pieces. This construction, rather than openness alone, controls the integrals as endpoints vary. [F6, step 1.1, construct]

3.1 For either path family put $A=\sup_\gamma\int|W_0(\gamma')|$ and $B=\sup_\gamma\int|T^\flat(\gamma')|$, integrating over all its pieces. These constants are finite: the forms are smooth on the fixed compact images and the coordinate velocities and number of pieces have common bounds from step 2.1. The explicit family in [F7] gives $\int|W_q(\gamma')|\le A+4B$ for every $q\in[\delta,1]$. Since $d_q\ge1$, every partial correction $\alpha_q(s)=-d_q^{-1}\int_0^sW_q(\gamma')$ satisfies $|\alpha_q(s)|\le A+4B$. Apply the transfer formula in [F1] on each smooth piece, retaining the accumulated correction at each join; a constant stationary translation preserves the metric and future direction. The finite concatenation remains future timelike by [F6]. This proves a uniform correction bound for the actual chosen family, without deducing parameter regularity from a separate fixed-$q$ choice. [F1, F6, F7, step 2.1, algebra]

4.1 For a candidate graph let $F(t,x)=t-u(x)$. Extend its future normal $n$ and positive lapse $N=-g_q(T,n)$ to its stationary translates, taking $n^\flat=g_q(n,\cdot)$. Since $F(T)=1$ and its level sets are those spacelike translates, $dF=-n^\flat/N$ throughout the product; thus $F$ increases along each transferred future timelike path. Write $a_i=(t_i^-,z_i^-)$ and $b_i=(t_i^+,z_i^+)$. The transferred incoming path ends at $(\alpha_q^-,z)$, giving $u(z)\le u(z_i^-)+\alpha_q^- -t_i^-$; the transferred outgoing path starts at $(0,z)$ and ends at $(t_i^++\alpha_q^+,z_i^+)$, giving $u(z)\ge u(z_i^+)-t_i^+-\alpha_q^+$. The finitely many $t_i^\pm$ are fixed, step 3.1 bounds the corrections, and the common normalized end bound in [F1], with $u=4q\widetilde u/d_q$ from [F8] and $d_q\ge1$ from [F7], bounds all endpoint heights. Hence $|u|$ is uniformly bounded on $Q$. Only existing indexed pairs were used. [F1, F7, F8, step 1.1, step 3.1, algebra]

5.1 Each candidate has its smooth individual K-height by the fixed-q result in [F2]. Shrink the reference collar so its closed collar has all its axial orbits in the common local symmetry neighborhood of [F9]: the smooth circle action preserves compact $S$, and continuity uniformly over its compact period interval gives such a smaller collar. The union $C$ of the outer reference boundaries over $q\in[\delta,1]$ is compact and disjoint from $S$, by the smooth common boundary-distance maps in [F2]. Its axial saturation $A=\{\phi_s^Zx:x\in C,0\le s\le2\pi\}$ is compact and lies in that local neighborhood. It also lies in the exterior collar domain: on the shrunken collar the local fields agree with the complete extended fields of [F2], whose flows preserve their exterior domain. The stationary projection of $A$ is therefore compact in $\Sigma_1^\circ$, and its stationary time coordinate is bounded. For $F(t,x)=t-u(x)$, commutation and $K=T+\Omega_HZ$ give $F(\phi_s^Kx)=s+F(\phi_{\Omega_Hs}^Zx)$. Periodicity and step 4.1 bound the second term uniformly, using that compact projection and bounded time coordinate. At the candidate intersection this expression is zero, so the outer K-height is uniformly bounded. Apply the strict barriers $c\mp M\rho$ of [F2] to the maximum of $u^K+M\rho$ and minimum of $u^K-M\rho$. The contact lemma includes S: equal boundary flow times give tangent planes because K vanishes there, and its strict curvature signs rule out an extremum beyond the outer bound. Thus $|u^K|\le C$ down to S for every indexed pair. [F1, F2, F9, step 4.1]

6.1 Use [F3] with this common height bound. The normal boost gives a common boundary angle; the Gaussian flow estimates give a strict cone and radial comparison. Projection is locally invertible, proper onto one fixed target collar and one-sheeted by its individual boundary germ, giving common zero-boundary normal graph domains. All these generic lemmas concern candidates actually supplied, not a requirement that every background parameter have a candidate. [F2, F3, step 5.1]

7.1 The compact smooth background controls the local observer tensors, so the full-range logarithmic estimate in [F4] applies to each candidate. Its cutoff lemmas give a uniform normal-angle bound on a smaller common collar. The Gaussian graph identity then bounds the height and gradient in a compact spacelike jet cone. The coefficient extension in [F4] gives a common full uniformly elliptic jet box and bounded forcing, while the smooth fixed S supplies uniform boundary charts and the zero Dirichlet data. With the Hölder-norm convention in [F8], apply [F5] for a common C1-beta seed, then the seeded boundary bootstrap in [F4] for all finite higher estimates. Thus no uniform initial C4 norm or missing-parameter section has been assumed. [F1, F2, F3, F4, F5, F8, step 6.1] ∎

## External input

The initial boundary C1-beta estimate is imported from Simon Lecture18 Theorem2. Its exact coefficient-box, bounded-forcing, bounded height/gradient and zero-Dirichlet smooth-boundary hypotheses and the actual reading limits are recorded in the source metadata. It is applied only after the indexed cutoff angle bound; higher boundary estimates then use the already authored seeded bootstrap.

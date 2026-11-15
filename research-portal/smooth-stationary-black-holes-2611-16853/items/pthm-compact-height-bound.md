---
id: pthm-compact-height-bound
title: "Lemma 3.2: compact stationary-height bounds"
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-stationary-lorentzian-data
  - def-spacelike-maximal-hypersurface-data
  - def-causal-exterior-and-boundary-data
  - def-stationary-maximal-graph
  - def-harrison-normalization
  - def-harrison-one-form-family
  - pthm-original-lapse-and-product
  - pthm-harrison-electrovacuum
  - pthm-timelike-path-transfer
  - pthm-positive-transformed-lapse
  - pthm-radial-barrier-height-decay
  - physics:lem-gr-chronology-openness
  - math:def-axiom-of-choice
  - lem-author-12a8dba09036-maximal-stationary-far-tail-access
  - physics:thm-gr-convex-normal-neighborhoods
  - physics:thm-gr-normal-neighborhood-causal-cone
  - physics:lem-gr-causal-curve-calculus
  - physics:lem-gr-joint-exponential-diffeomorphism
  - physics:thm-gr-local-geodesics-and-exponential-map
  - math:def-compact-space
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:thm-lebesgue-number-lemma
  - math:thm-heine-borel-rn
  - math:thm-extreme-value-metric
  - math:thm-choice-implies-dependent-implies-countable-choice
  - math:cor-transverse-intersection-theorem
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-harrison-one-form-family: mathematical-premise
  pthm-original-lapse-and-product: physical-result
  pthm-harrison-electrovacuum: physical-result
  pthm-timelike-path-transfer: physical-result
  pthm-positive-transformed-lapse: physical-result
  pthm-radial-barrier-height-decay: physical-result
  physics:lem-gr-chronology-openness: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  lem-author-12a8dba09036-maximal-stationary-far-tail-access: mathematical-premise
  physics:thm-gr-convex-normal-neighborhoods: mathematical-premise
  physics:thm-gr-normal-neighborhood-causal-cone: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  physics:lem-gr-joint-exponential-diffeomorphism: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:lem-compactness-of-a-subspace-is-ambient: mathematical-premise
  math:thm-lebesgue-number-lemma: mathematical-premise
  math:thm-heine-borel-rn: mathematical-premise
  math:thm-extreme-value-metric: mathematical-premise
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
  math:cor-transverse-intersection-theorem: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pages 15–16, Lemma 3.2 and its proof
      statement: For each compact subset of the original exterior section, the
        stationary graph heights are uniformly bounded for the positive
        parameter interval; the proof compares heights along transferred
        timelike curves to and from the asymptotic end.
      hypotheses: The regular stationary vacuum construction with maximal original
        exterior section, mass normalized to one, and the candidate maximal
        sections in the continuation argument; the parameter lies in a fixed
        positive interval.
      reading_limits: Read the frozen article text at Lemma 3.2 and its proof. This
        reference attributes the article claim and is not used as a premise of
        the proof below.
physical_scope: Conditional geometric deduction in the smooth stationary vacuum
  model and its Harrison-transformed metrics; candidate sections are assumed,
  and no observation is asserted.
dependency_level: 15
---

## Statement

Adopt the regular stationary vacuum construction with mass one, maximal original exterior section, and $T|_S\not\equiv0$. Let $\Sigma_1^\circ$ be the interior of that section and identify the exterior with $\mathbb R_t\times\Sigma_1^\circ$ by the stationary flow, so $T=\partial_t$. Use the selected Harrison family obtained from one smooth stationary primitive $W_0$ by $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, and the corresponding metrics $g_q$ and positive constants $d_q$.

Fix $\delta\in(0,1)$. For every $q\in[\delta,1]$, assume a supplied connected smooth spacelike maximal section with boundary $S$ is a stationary graph $t=u_q(x)$ over $\Sigma_1^\circ$, and that the family satisfies the candidate-section, normalized-end and uniform-estimate hypotheses of the radial height-decay and transformed-lapse results. In particular, its normalized end height tends to zero at infinity for each fixed $q$, and its future normal has positive stationary lapse. Then, for every compact $K\subset\Sigma_1^\circ$, there is $C_{\delta,K}<\infty$, independent of $q$, such that $\sup_K|u_q|\le C_{\delta,K}$.

The original-section maximality used here is assumed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$, with the original metric $g$, so $H_g|_C=0$. The selected physical end retains its stated mass-one normalization. Maximality of an independently labelled chart-side section or another supplied maximal section does not replace this premise. No equality between the hypersurface identification and the physical stationary end chart is assumed. [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

Assume two-sided access to sufficiently far selected original ends: for some $R_a$ and every $R\ge R_a$, let $U_R=\mathbb R\times\{r>R\}$ in the physical stationary end chart and require $\mathcal E\subset I^-_{(\mathcal E,g)}(U_R)\cap I^+_{(\mathcal E,g)}(U_R)$. Both witnessing timelike paths are taken in the unchanged original metric and exterior. This is an explicit premise, not an identification of independent charts or a consequence claimed from the definition of the designated end. [[def-causal-exterior-and-boundary-data]]

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-stationary-lorentzian-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-stationary-maximal-graph]]

[[def-harrison-normalization]]

[[def-harrison-one-form-family]]

[[pthm-original-lapse-and-product]]

[[pthm-positive-transformed-lapse]]

[[pthm-radial-barrier-height-decay]]

## Facts & Assumptions

[A1] Work in ZFC, hence with the countable and dependent choice used by the causal suppliers. The regular model supplies a time-oriented stationary exterior and a connected stationary asymptotic end on which $T$ is future timelike sufficiently far out. The exterior is the intersection of the chronological past and future of the designated end, using locally absolutely continuous curves with nonzero future timelike velocity almost everywhere. [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]] [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-causal-exterior-and-boundary-data]] [[def-stationary-lorentzian-data]]

[F1] The stationary flow is a global product on the open exterior. A stationary graph is the image of $x\mapsto(u_q(x),x)$; spacelike means that its induced metric is positive definite. [[pthm-original-lapse-and-product]] [[def-stationary-maximal-graph]] [[def-spacelike-maximal-hypersurface-data]]

[F2] The chosen family has $W_q=(1-q)^2W_0-4q(1-q)T^\flat$ for one smooth stationary $W_0$, and $d_q=(1+q)^2+(1-q)^2\psi(p)^2$. Thus $d_q\ge1$ on $[0,1]$, and both $d_q$ and $d_q^{-1}$ are uniformly bounded there. The corresponding transformed metrics use this same family. [[def-harrison-one-form-family]] [[def-harrison-normalization]] [[pthm-harrison-electrovacuum]]

[F3] With the actual original exterior section maximal as assumed here, the transfer supplier applies on its stationary product with the supplied normalized Ernst data and the Harrison one-form of [F2], using the transported future orientation. For any smooth future $g$-timelike curve $\gamma$, stationary transfer preserves its spatial path and initial point and produces a future $g_q$-timelike curve with stationary-time correction $\alpha_q(\lambda)=-d_q^{-1}\int_0^\lambda W_q(\gamma'(s))\,ds$. [[pthm-timelike-path-transfer]]

[F4] The normalized coordinates are $t_q=d_qt/(4q)$ and $x_q=qx$. Here $x$ is the specified physical Cartesian end coordinate of the regular stationary construction, restricted to the actual original section $C$ and transported by the stationary flow; this is the specified Cartesian end used in the graph-height definition and the radial estimate. It is independent of the topological identification of the whole section. Regularity places $C$ at physical end time zero and gives $T=\partial_t$ on that end. Consequently the stationary-product map sends $(a,(0,x))$ to the physical end point $(a,x)$: the physical end translations are the same stationary flow used by the product map. Thus the graph normalization and the access premise use the same physical $r=|x|$, without identifying the topological chart with that chart. [[def-regular-stationary-vacuum-spacetime]] [[pthm-original-lapse-and-product]] Under the stated candidate hypotheses, the end estimate gives $|\widetilde u_q(x_q)|\le C r_q^{-\mu}$ for $r_q\ge R$, uniformly in $q\in[\delta,1]$, for any fixed $\mu\in(0,1)$. The positive-lapse result gives a future unit graph normal $n_q$ with $-g_q(T,n_q)>0$. [[def-stationary-maximal-graph]] [[pthm-radial-barrier-height-decay]] [[pthm-positive-transformed-lapse]]

[F5] Chronological reachability is open: if one point is chronologically before another, sufficiently small neighborhoods of the two points retain that relation. [[physics:lem-gr-chronology-openness]]

[F6] Under all its separately stated geometric hypotheses, the far-tail lemma provides a sufficient criterion for outgoing access. The present proof uses the two-sided access premise in the Statement directly. In particular, it does not claim that the definition of the original end alone proves access to every truncated tail. [[lem-author-12a8dba09036-maximal-stationary-far-tail-access]]

[F7] Every point of a smooth time-oriented Lorentzian four-manifold has arbitrarily small strictly convex normal neighborhoods. Within one such neighborhood, future timelike reachability by the stipulated absolutely continuous curves is exactly the exponential image of future timelike initial vectors. The unique joining geodesic is smooth and depends smoothly on its endpoints through the two-point inverse and geodesic evaluation maps. Restrictions, positive affine reparametrizations and finite concatenations preserve the permitted timelike curve class. [[physics:thm-gr-convex-normal-neighborhoods]] [[physics:thm-gr-normal-neighborhood-causal-cone]] [[physics:lem-gr-joint-exponential-diffeomorphism]] [[physics:thm-gr-local-geodesics-and-exponential-map]] [[physics:lem-gr-causal-curve-calculus]]

[F8] Compactness gives finite subcovers, also for covers by ambient open sets. Closed bounded Euclidean sets, including the parameter intervals and closed coordinate balls used below, are compact. An open cover of a compact metric space has a Lebesgue number. A continuous real function on a nonempty compact metric space is bounded and attains its extrema. [[math:def-compact-space]] [[math:lem-compactness-of-a-subspace-is-ambient]] [[math:thm-heine-borel-rn]] [[math:thm-lebesgue-number-lemma]] [[math:thm-extreme-value-metric]]

[F9] At every point of the intersection of two transverse smooth embedded submanifolds, the tangent space of their intersection is the intersection of their tangent spaces. Apply this to the two regular horizon sheets, whose local intersection is $S$. [[math:cor-transverse-intersection-theorem]] [[def-regular-stationary-vacuum-spacetime]]

## Proof

**Given:** The construction, candidate graph family, positive parameter interval and compact set $K$ in the Statement.

**Goal:** Bound $|u_q|$ on $K$ by a constant independent of $q$.

1.1 The case $K=\varnothing$ is immediate; assume $K\ne\varnothing$. Fix $\mu\in(0,1)$ and the uniform normalized end radius $R$ from [F4]. The original product supplier in F1 applies to the actual exterior section $C=\Sigma_0\cap\mathcal E$, whose original-metric maximality is an explicit Statement premise. It gives the stationary product over that section; the supplied original graph convention identifies its base with $\Sigma_1^\circ$. Independent topological and physical end charts are not equated. Choose $R_f$ beyond the threshold of the two-sided access premise, inside the specified physical end, and with $R_f>R/\delta$, and put $U_f=\mathbb R\times\{r>R_f\}$ using the physical stationary chart. By the chart match in [F4], the stationary-product projection of a point of $U_f$ is the physical end point $(0,y)$ with the same spatial coordinate $y$ and $|y|>R_f$. This is also the coordinate used to evaluate the normalized graph height. The outgoing half of that premise gives a future original-metric timelike path from every $(0,x)$ to $U_f$, entirely in $\mathcal E$. This uses the explicit access premise rather than treating access to all far tails as part of regularity. [given, A1, F1, F4, F8, choose]

1.2 The function $\tau_q(t,x)=t-u_q(x)$ has spacelike level sets, since these are stationary translates of the given graph. Its differential annihilates the level-set tangents and evaluates to $1$ on $T$. Extending the future unit normal by stationary translation, positive lapse gives $d\tau_q=-g_q(n_q,\cdot)/N_q$, where $N_q=-g_q(T,n_q)>0$. Consequently $d\tau_q(v)>0$ for every future timelike $v$: in a Lorentzian orthonormal frame the inner product of two future timelike vectors is negative. Hence $\tau_q$ strictly increases along each smooth piece of a transferred curve, and therefore along the full finite concatenation. [given, F1, F4, F7, algebra]

2.1 The incoming half of the explicit two-sided access premise gives, for every $(0,x)$, a future original-metric timelike path from $U_f$ to $(0,x)$, entirely in $\mathcal E$. Thus both directions of path access used in the compact-family argument are supplied in the same metric and unchanged exterior. No time-reversal deduction of a missing access premise, and no equality of separate coordinate maps, is used. [given, A1, F1, step 1.1]

3.1 All curves just obtained are contained in $\mathcal E$ by the explicit access premise. Also, any ambient future timelike curve between two exterior points stays in the exterior: an end point chronologically preceding its first endpoint and an end point following its last endpoint can be concatenated to its subarcs, putting every intermediate point in both chronological sets defining $\mathcal E$. For either of the curves at a fixed $x$, cover its compact parameter interval by inverse images of strictly convex normal neighborhoods contained in the open $\mathcal E$. A Lebesgue number gives a finite subdivision whose subarcs each lie in one neighborhood. Restriction and positive affine reparametrization put each subarc in the curve class of [F7]; its cone characterization makes the joining initial vector future timelike. Replace that subarc by the unique joining geodesic in the same neighborhood. Finite concatenation gives a piecewise smooth future timelike curve in $\mathcal E$ with the original endpoints. [given, A1, F7, F8, step 1.1, step 2.1, construct]

4.1 For the incoming curve at $x$, fix its penultimate vertex and vary its final endpoint from $(0,x)$ to $(0,z)$ in the last convex normal neighborhood. For the outgoing curve, vary the first endpoint to $(0,z)$ and fix the next vertex in the first such neighborhood. The smooth two-point inverse and geodesic evaluation in [F7] give smooth families of these terminal and initial geodesic pieces. Their initial vectors remain future timelike for $z$ close to $x$, since the future timelike cone is open. Keep all other pieces fixed. Choose an open coordinate neighborhood $V_x$ of $x$ whose closure is a closed coordinate ball contained in this common validity region; it may also be chosen inside the chronological endpoint neighborhoods of [F5]. These are incoming and outgoing piecewise smooth curves for every $z\in\overline V_x$, with the end endpoints fixed. [F5, F7, F8, step 3.1, choose, construct]

5.1 By compactness choose finitely many $V_x$ covering $K$, and retain the corresponding pairs of curve families. Every varying piece is smooth on a neighborhood of the compact parameter set $[0,1]\times\overline V_x$; fixed pieces have compact parameter interval. Their images form a compact subset of $\mathcal E$: pull an open cover back to each parameter set, take a finite subcover, and then take the finite union over pieces and families. The stationary time coordinate on these curves is uniformly bounded. Moreover the scalar evaluations $W_0(\gamma')$ and $T^\flat(\gamma')$ are continuous on those compact parameter sets and hence uniformly bounded, by [F8]. The number of pieces is bounded because only finitely many families were retained. End endpoints have only finitely many spatial positions in $U_f$. [F1, F2, F8, step 4.1, choose]

6.1 The actual exterior section is maximal by the Statement, its complete stationary product is [F1], and the selected smooth stationary Harrison family is [F2]. Thus these are the revised transfer supplier's hypotheses in [F3], with no identification of the physical end chart and the hypersurface identification. Apply the transfer result to each smooth piece after positive affine reparametrization to $[0,1]$. Translate each subsequent transferred piece by the time correction accumulated on the preceding pieces. Stationarity preserves the integrands and future cones, so these pieces join to future $g_q$-timelike curves with the original spatial paths. Their total time corrections are uniformly bounded: each piece contributes $-d_q^{-1}\int W_q(\gamma')$, and [F2] expresses its integrand through the bounded evaluations of $W_0$ and $T^\flat$ from step 5.1, with uniformly bounded coefficients. There are uniformly finitely many pieces, and $d_q^{-1}$ is uniformly bounded. The initial points are unchanged and both endpoint times are uniformly bounded. [F2, F3, F7, step 5.1, algebra]

7.1 At each of the finitely many end base points, let $y$ be its physical Cartesian coordinate, and use $u_q(y)$ for the graph function expressed in that chart. The endpoints belong to $U_f$, so the matched coordinates in [F4] and step 1.1 give $|y|>R_f$ and $r_q=q|y|\ge\delta|y|>\delta R_f>R$. The end estimate and $u_q(y)=(4q/d_q)\widetilde u_q(qy)$ therefore bound $|u_q(y)|$ uniformly in $q$. For a transferred future curve from an end point $(t_-,y_-)$ to $(t_+,x)$, step 1.2 gives $u_q(x)<u_q(y_-)+t_+-t_-$. A transferred future curve from $(s_-,x)$ to an end point $(s_+,y_+)$ similarly gives $u_q(x)>u_q(y_+)+s_--s_+$. The endpoint times and transfer corrections are uniformly bounded by steps 5.1 and 6.1. These two inequalities give a common bound for $|u_q(x)|$ for all $x\in K$ and $q\in[\delta,1]$. [F2, F4, step 1.1, step 2.1, step 5.1, step 1.2, step 6.1, algebra] ∎

The article reference attributes Lemma 3.2. The proof uses the declared suppliers and supplies the compact-family and parameter-uniformity argument locally. The selected single-primitive family is essential to the uniform bound on the transfer correction; an arbitrary independently chosen one-form for each parameter would not provide that bound.

## Source notes

The article reference attributes Lemma 3.2. The proof uses the declared suppliers and supplies the compact-family and parameter-uniformity argument locally. The selected single-primitive family is essential to the uniform bound on the transfer correction; an arbitrary independently chosen one-form for each parameter would not provide that bound.

These explicit premises specify the generated conditional result. They are not asserted to follow from the original regularity definition alone, and are not attributed to the original article. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

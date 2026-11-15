---
id: pthm-past-boundary-localization
title: "Lemma 4.3: localization of the causal cut near S"
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - pthm-global-harrison-one-form
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - def-near-horizon-past-boundary-sets
  - def-stationary-maximal-graph
  - def-stationary-section-time
  - def-coordinate-comparison-spheres
  - pthm-complete-maximal-slices
  - pthm-original-lapse-and-product
  - pthm-transformed-end-geometries
  - pthm-eventual-causal-access
  - pthm-causal-finite-time-escape
  - pthm-past-boundary-null-generators
  - pthm-adm-temporality
  - math:def-axiom-of-choice
  - lem-author-9d607f469119-uniform-access-on-trimmed-core
  - lem-author-9d607f469119-finite-time-collar-exclusion
  - lem-author-9d607f469119-slice-intersection-of-past-boundary
  - math:lem-closed-subset-of-a-compact-space-is-compact
  - math:thm-extreme-value-metric
  - math:thm-continuous-image-of-a-compact-space-is-compact
  - math:thm-the-riemannian-distance-topology-is-the-manifold-topology
  - pthm-author-048251387164-sequence-closure-and-completeness
  - lem-author-12a8dba09036-maximal-stationary-far-tail-access
dependency_roles:
  pthm-global-harrison-one-form: physical-result
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-near-horizon-past-boundary-sets: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  def-stationary-section-time: mathematical-premise
  def-coordinate-comparison-spheres: mathematical-premise
  pthm-complete-maximal-slices: physical-result
  pthm-original-lapse-and-product: physical-result
  pthm-transformed-end-geometries: physical-result
  pthm-eventual-causal-access: physical-result
  pthm-causal-finite-time-escape: physical-result
  pthm-past-boundary-null-generators: physical-result
  pthm-adm-temporality: physical-result
  math:def-axiom-of-choice: mathematical-premise
  lem-author-9d607f469119-uniform-access-on-trimmed-core: mathematical-premise
  lem-author-9d607f469119-finite-time-collar-exclusion: mathematical-premise
  lem-author-9d607f469119-slice-intersection-of-past-boundary: mathematical-premise
  math:lem-closed-subset-of-a-compact-space-is-compact: mathematical-premise
  math:thm-extreme-value-metric: mathematical-premise
  math:thm-continuous-image-of-a-compact-space-is-compact: mathematical-premise
  math:thm-the-riemannian-distance-topology-is-the-manifold-topology: mathematical-premise
  pthm-author-048251387164-sequence-closure-and-completeness: physical-result
  lem-author-12a8dba09036-maximal-stationary-far-tail-access: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional causal geometry of the supplied positive-parameter
  stationary vacuum Harrison construction; no measurement is asserted.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp.24–25, Lemma 4.3 and proof
      reading_limits: "Historical attribution-reading record retained; this
        maintenance revision checks the current original-metric supplier
        contracts and their application, without new article-PDF or
        external-proof reading. Retained prior source-input or attribution
        record: Retained attribution only: Adopt the standing regular mass-one
        stationary vacuum Harrison construction with original maximal outer
        section and $T|_S\\not\\equiv0$. Fix a sufficiently small positive $q$,
        a supplied complete smooth maximal section $\\Sigma=\\Sigma_{q,0}$ with
        compact boundary $S$, and the comparison cylinder. Use the sets,
        intrinsic boundary distance $\\rho$, and relative-exterior chronological
        convention of [[def-near-horizon-past-boundary-sets]], with inside
        meaning the component containing $S$ in stationary spatial projection.
        For every sufficiently small $\\eta>0$, all $t\\ge t_\\eta$ give compact
        remainder $K$ containing a neighborhood of $S$. Its relative boundary
        $D$ is compact, lies between distances $0<\\eta_t<\\rho<\\eta$, and
        coincides with the portion of $\\Sigma\\cap\\partial_{\\mathcal
        E}I^-_{g_q}(C_t)$ inside the cylinder. Eventual access places the
        compact region between $S_\\eta$ and the cylinder in $I^-_{g_q}(C_t)$,
        while the finite-$v_q$ Gronwall bound excludes a small neighborhood of
        $S$. Projecting a short initial segment of a boundary generator along a
        local future timelike flow supplies the reverse boundary inclusion.
        Attributed setting: The regular stationary vacuum construction, maximal
        original outer section, rotating bifurcation sphere, fixed sufficiently
        small positive parameter and supplied complete smooth maximal stationary
        graph section. Read the actual frozen article extracted text of Lemma
        4.3 and its proof, pp.24–25, including the preceding access paragraph
        and Lemma 4.2. Attribution only; the compact-core argument below is a
        local prerequisite proof, not an application of the article claim. Fresh
        maintenance limits: current item and supplier contracts and the local
        applications were checked; no new reading of the external proof or PDF
        images is claimed."
dependency_level: 26
---

## Statement

Adopt the standing regular mass-one stationary vacuum Harrison construction with original maximal outer section and $T|_S\not\equiv0$. Fix a sufficiently small positive $q$, a supplied complete smooth maximal section $\Sigma=\Sigma_{q,0}$ with compact boundary $S$, and the comparison cylinder. Use the sets, intrinsic boundary distance $\rho$, and relative-exterior chronological convention of [[def-near-horizon-past-boundary-sets]], with inside meaning the component containing $S$ in stationary spatial projection. For every sufficiently small $\eta>0$, all $t\ge t_\eta$ give compact remainder $K$ containing a neighborhood of $S$. Its relative boundary $D$ is compact, lies between distances $0<\eta_t<\rho<\eta$, and coincides with the portion of $\Sigma\cap\partial_{\mathcal E}I^-_{g_q}(C_t)$ inside the cylinder. Eventual access places the compact region between $S_\eta$ and the cylinder in $I^-_{g_q}(C_t)$, while the finite-$v_q$ Gronwall bound excludes a small neighborhood of $S$. Projecting a short initial segment of a boundary generator along a local future timelike flow supplies the reverse boundary inclusion.

## Facts & Assumptions

[F1] Use the exact hypotheses and interface of [[post-stationary-vacuum-model]].

[F2] Use the exact hypotheses and interface of [[def-regular-stationary-vacuum-spacetime]].

[F3] Use the exact hypotheses and interface of [[def-harrison-normalization]].

[F4] Use the exact hypotheses and interface of [[def-near-horizon-past-boundary-sets]].

[F5] Use the exact hypotheses and interface of [[def-stationary-maximal-graph]].

[F6] Use the exact hypotheses and interface of [[def-stationary-section-time]].

[F7] Use the exact hypotheses and interface of [[def-coordinate-comparison-spheres]].

[F8] Use the exact hypotheses and interface of [[pthm-complete-maximal-slices]].

[F9] Use the additional positive-parameter smooth-global-primitive conclusion of [[pthm-transformed-end-geometries]] for this same regular mass-one construction with maximal original exterior section and $T|_S\not\equiv0$. The actual single smooth primitive of [[pthm-global-harrison-one-form]] has normalized contraction and $(W_0)_i=O_5(r^{-3})$; it need not equal the separate radial integral. At the fixed $q>0$, this branch supplies the normalized Minkowski end bounds and their five spatial derivative estimates for the actual Harrison metric. It does not equate physical end radius with an unrelated topological reference radius.

[F10] Use the exact hypotheses and interface of [[pthm-eventual-causal-access]].

[F11] The causal finite-time supplier constructs a smooth boundary collar for the supplied section in its Proof 1.2; on a sufficiently small collar it gives $|d\rho/dv|\le C\rho$ almost everywhere for future causal curves, where $\rho$ is intrinsic distance to $S$, extended stationarily. [[pthm-causal-finite-time-escape]]

[F12] Use the exact hypotheses and interface of [[pthm-past-boundary-null-generators]].

[F13] Use the exact hypotheses and interface of [[pthm-adm-temporality]].

[F14] Use the exact hypotheses and interface of [[math:def-axiom-of-choice]].

[F15] The sequence-closure result also proves completeness and compact physical-end cores for every individually admissible section. Apply its universal fixed-section conclusion, or its constant-sequence argument, at the chosen $q>0$. This needs no agreement between topological and physical charts. [[pthm-author-048251387164-sequence-closure-and-completeness]]

[F16] For such a section, write $G:C\to\Sigma^\circ$ for its stationary graph over the actual original exterior and let $B_{0,R}$ be the original physical truncation. Then $B_R=S\cup G(B_{0,R}\setminus S)=\Sigma\setminus G(\{r_{\mathrm{phys}}>R\})$ is compact, contains a neighborhood of $S$, has smooth outer boundary $G(\{r_{\mathrm{phys}}=R\})$, and has compact positive-distance trims in the interior. [[pthm-author-048251387164-sequence-closure-and-completeness]]

[F17] Use the exact hypotheses and interface of [[lem-author-9d607f469119-uniform-access-on-trimmed-core]].

[F18] Use the exact hypotheses and interface of [[lem-author-9d607f469119-finite-time-collar-exclusion]].

[F19] Use the exact hypotheses and interface of [[lem-author-9d607f469119-slice-intersection-of-past-boundary]].

[F20] A closed subset of a compact metric space is compact. [[math:lem-closed-subset-of-a-compact-space-is-compact]]

[F21] A continuous real-valued function on a nonempty compact metric space has a finite attained minimum and maximum. [[math:thm-extreme-value-metric]]

[F22] A continuous map between metric spaces sends compact subsets to compact subsets. [[math:thm-continuous-image-of-a-compact-space-is-compact]]

[F23] On a connected Riemannian manifold without boundary, intrinsic distance induces the manifold topology. The included-boundary case needed here is established by the local half-ball comparison in Proof 1.1. [[math:thm-the-riemannian-distance-topology-is-the-manifold-topology]]

[F24] Under the standing regular vacuum and original exterior-maximality hypotheses, put $C=\Sigma_0\cap\mathcal E$ and $B_0=C\cup S$. The product theorem supplies this actual section, its stationary product, its separate adapted topological chart and its compact physical-end truncations $B_{0,R}$. It does not identify the two radii. [[pthm-original-lapse-and-product]]

[F25] The outgoing-access premise required by the eventual-access supplier is checked in the original metric before that supplier is invoked. Under the standing maximality of the actual $C=\Sigma_0\cap\mathcal E$, its original lapse/product result gives a connected smooth spherical-exterior closure, positive original lapse, a complete stationary product and compact physical-end truncations. Regularity supplies the smooth original spacelike extension across compact $S$, the ambient fields and tangency of $T$ to $S$, the asymptotically Euclidean induced end and the stationary end bounds. These are the hypotheses of the maximal-stationary far-tail lemma: every point of the original exterior reaches every sufficiently far selected stationary tail by a future original-metric timelike curve contained in that exterior. This is not an assumption about the transformed metric or an end-truncation identification. [[pthm-original-lapse-and-product]] [[def-regular-stationary-vacuum-spacetime]] [[lem-author-12a8dba09036-maximal-stationary-far-tail-access]]

## Proof

**Given:** The hypotheses in the Statement, with the inherited ZFC convention, including the Axiom of Choice used by the compact-core and collar suppliers in [F14]–[F18].

**Goal:** Establish the stated conclusion.

1.1 The section supplier [F8] gives a connected smooth spacelike maximal section with included compact boundary $S$, an interior stationary graph $G:C\to\Sigma^\circ$, and normalized end decay through four derivatives. Thus it is individually admissible at this fixed $q>0$. The actual original maximal exterior section $C$ and its physical truncations are supplied by [F24]. On the physical end, pulling back the positive-parameter metric bounds in [F9] with the decaying graph slope gives an induced metric uniformly comparable to Euclidean in $x_q=qx$; hence $|dr_{\mathrm{phys}}|_{h_q}$ is bounded there. Apply [F15]–[F16] to this same section, taking a lower parameter bound $q/2$ if using its constant-sequence formulation. Put $R=R_0q^{-2/3}$ in the actual physical chart, with the free comparison constant large enough for the physical truncation. The resulting core is $B=S\cup G(B_{0,R}\setminus S)$, whose outer boundary is the actual physical graph sphere $\Gamma=G(\{r_{\mathrm{phys}}=R\})$ on the comparison cylinder. It is compact, contains a neighborhood of $S$, and has compact positive-distance trims. Its inside component is the one containing $S$: the physical tail and its sphere are connected, and an additional component of the smooth core avoiding that sphere would be both open and closed in the connected section. These facts identify the supplied inside region in [F4] without a global physical radial coordinate or any extension of stationary height through $S$. For interior points use the Riemannian topology input in [F23]. At a boundary point choose a coordinate half-ball with a smaller closed half-ball on which $c|\xi|^2\le h(\xi,\xi)\le C|\xi|^2$, for fixed $0<c\le C<\infty$; such bounds follow from smooth positive coefficients up to the boundary in [F8]. Coordinate line segments inside the convex half-ball give $d_h(p,p')\le\sqrt C\,|x(p)-x(p')|$ for sufficiently close points. Conversely, any curve from its center leaving the smaller half-ball spends at least $\sqrt c$ times the coordinate exit radius in length before leaving. Hence points at sufficiently small intrinsic distance remain in that chart, and the same lower bound on curves staying there gives coordinate convergence. This proves equality of the two topologies also at $S$, without assuming the boundaryless theorem already covers boundary points. [given, F1, F2, F3, F4, F5, F8, F9, F14, F15, F16, F23, F24]

2.1 Put $P_t=I^-_{g_q}(C_t)$. The actual original maximal section and stationary product in [F24], with the regular extension and end data in [F2], match the original-metric hypotheses enumerated in [F25]. Apply that far-tail lemma to obtain outgoing access for every original exterior point to every sufficiently far selected stationary end. Take the free comparison constant beyond this background tail threshold before fixing $C_t$. This establishes the new access premise of [F10] before its use. Eventual-access supplies open increasing pasts and pointwise entry for every point of this section interior. The trimmed-core lemma therefore gives, for all sufficiently small $\eta>0$, one threshold after which $B\cap\{\rho\ge\eta/2\}\subset P_t$. In particular a neighborhood of the outer graph sphere lies in $P_t$. To check the extrema used here and below, put $R=R_0q^{-2/3}$ and $\Gamma=G(\{|x|=R\})$. By [F16], $\Gamma$ is compact; it is nonempty since $R>1$ and $G$ is defined on that sphere. Give $\Gamma$ the subspace metric from $d_{h_q}$, whose topology is the manifold subspace topology by [F23]. Give each $C_t$ the metric defined by Euclidean distance between its spatial coordinates; the supplied stationary end chart identifies its metric topology with its manifold topology. The smooth bijection $J_t:\Gamma\to C_t$, $J_t(G(x))=(t,x)$, is continuous for these metrics. Thus [F22] makes every $C_t$ nonempty and compact. The smooth section time $v$ restricts to a continuous real function on $C_t$, so [F21] supplies finite attained extrema. Since $v(J_t(G(x)))=t+v(J_0(G(x)))$, increase the threshold until $\min_{C_t}v=t+\min_{C_0}v>0$. [F4, F6, F7, F10, F16, F17, F21, F22, F23, step 1.1, F25]

3.1 Take the smooth boundary collar supplied by [F11], and let $U$ be its intersection with the neighborhood where its causal estimate holds, the interior of $B$ in $\Sigma$, and $\Sigma\setminus\Gamma$. This is an open neighborhood of compact $S$ by step 1.1. Write $d=d_{h_q}$. By the boundary topology comparison in step 1.1, for each $s\in S$ choose $r_s>0$ with $B_d(s,2r_s)\subset U$, and choose finitely many $B_d(s_j,r_{s_j})$ covering $S$. Put $\delta=\min_j r_{s_j}>0$ and fix $0<a<\delta$. If $\rho(x)\le a$, the definition of distance gives $s\in S$ with $d(x,s)<\delta$; some covering ball contains $s$, so $d(x,s_j)<\delta+r_{s_j}\le2r_{s_j}$ and $x\in U$. The triangle inequality gives $|\rho(x)-\rho(y)|\le d(x,y)$ by taking infima over $S$, so $\rho$ is continuous. Hence the closure of $\{\rho<a\}$ lies in $\{\rho\le a\}\subset U\subset B$, is compact by [F20], and avoids $\Gamma$. No smoothness of the distance sublevel is needed: it lies in the supplied smooth collar, where [F11] gives $|\rho'|\le C\rho$. For fixed $t$, [F21] and step 2.1 give $0<\min_{C_t}v\le\max_{C_t}v=V_t<\infty$ and a nonempty compact target $C_t$, whose stationary projection is $\Gamma$, outside $\{\rho<a\}$. The stationary product is supplied by [F6], and $v$ is temporal by [F13]. Thus every hypothesis of [F18] holds, and it gives $\{v=0,0<\rho<a e^{-CV_t}\}\cap P_t=\varnothing$. The definition separately keeps $S$ in $K$. Since this sublevel lies in $B$, $K$ contains a full section neighborhood of $S$. [F4, F6, F11, F13, F18, F20, F21, step 1.1, step 2.1]

4.1 The set $P_t\cap\Sigma^\circ$ is open in $\Sigma$, since $P_t$ is exterior-open and the section interior is open in $\Sigma$. The boundary convention in [F4] keeps $S$ outside $P_t$, so $K=B\setminus P_t$ is closed in $B$. By the topology comparison in step 1.1, $B$ is a compact metric subspace for the intrinsic distance, and [F20] therefore makes $K$ compact. By step 2.1, $K$ has no points with $\rho\ge\eta/2$. It is closed in $\Sigma$ because $B$ is the closed inside region of [F4]; hence its relative boundary $D$ in $\Sigma^\circ$ is contained in $K$. By step 3.1, $D$ has no points with $\rho<a e^{-CV_t}$. Choose $0<\eta_t<\min(\eta/2,a e^{-CV_t}/2)$ sufficiently small for [F16]. That supplier makes $B\cap\{\rho\ge\eta_t\}$ a compact subset of $\Sigma^\circ$. The relative boundary $D$ is closed in $\Sigma^\circ$ and contained in this subset, so it is closed in this compact metric subspace and compact by [F20]. The stronger bounds just proved give $D\subset\{\eta_t<\rho<\eta\}$. [F4, F10, F16, F17, F18, F20, step 1.1, step 2.1, step 3.1]

5.1 A point of $D$ is inside the cylinder because its outer graph sphere has a section neighborhood in $P_t$. Locally $K$ is the complement of $P_t$ on the section, so it lies in $\Sigma^\circ\cap\partial_{\mathcal E}P_t$. Conversely, any point $p$ of that ambient boundary on the inside section has $v(p)=0<\min_{C_t}v$. Apply [F12] to $p$ in this same construction, with the same supplied section and comparison cylinder: the inside condition and strict section-time inequality just checked give a future-directed boundary null segment from $p$ to $C_t$. The local slice-intersection lemma projects short initial points back along a normalized future timelike local flow, producing section points in $P_t$ tending to $p$ by push-up. Since $p\notin P_t$, it is in $D$. This proves equality with the asserted portion of the ambient past boundary. All boundaries and causal curves here are relative to $\mathcal E$; no ambient extension across the horizons, event-horizon identification or affine completeness is invoked. [F4, F6, F12, F13, F19, step 2.1, step 4.1] ∎



Compactness of the physical inside region is supplied by the sequence-closure item's local physical-exhaustion argument. The local access, finite-time collar-exclusion and slice-intersection suppliers then establish localization. Stationary graph height need not extend to S. The article attributes the claim only; this maintenance proposal asserts neither an original-author defect nor independent acceptance.

## Source notes

Compactness of the physical inside region is supplied by the sequence-closure item's local physical-exhaustion argument. The local access, finite-time collar-exclusion and slice-intersection suppliers then establish localization. Stationary graph height need not extend to S. The article attributes the claim only; this maintenance proposal asserts neither an original-author defect nor independent acceptance.

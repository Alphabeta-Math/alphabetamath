---
id: pthm-null-boundary-lipschitz-levels
title: Lipschitz causal height and level-set Jacobian bound
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - def-truncated-null-boundary-height
  - def-lipschitz-cut-area-data
  - def-stationary-section-time
  - def-spacelike-maximal-hypersurface-data
  - pthm-complete-maximal-slices
  - pthm-positive-transformed-lapse
  - pthm-past-boundary-localization
  - pthm-eventual-causal-access
  - pthm-causal-finite-time-escape
  - pthm-past-boundary-null-generators
  - pthm-transformed-cauchy-sections
  - pthm-adm-temporality
  - pthm-null-endpoint-map-properties
  - pthm-raychaudhuri-endpoint-jacobians
  - pthm-comparison-sphere-properties
  - math:def-axiom-of-choice
  - lem-author-594d78e425ed-compact-normal-flow-and-area-distortion
  - lem-author-594d78e425ed-uniform-translated-cut-localization
  - lem-author-594d78e425ed-truncated-past-height-lipschitz-levels
  - lem-author-594d78e425ed-negative-cut-selected-endpoints
  - lem-author-594d78e425ed-multiplicity-aware-level-area-transfer
  - def-near-horizon-past-boundary-sets
  - def-stationary-maximal-graph
  - pthm-ernst-potential-existence
  - pthm-global-harrison-one-form
  - def-harrison-one-form-family
  - def-harrison-one-form
  - pthm-harrison-lorentzian-algebra
  - pthm-author-048251387164-sequence-closure-and-completeness
  - pthm-original-lapse-and-product
  - math:thm-chain-rule-for-total-derivatives
  - math:thm-connectedness-characterisations
  - math:cor-euclidean-spheres-are-path-connected
  - math:thm-path-connected-implies-connected
  - lem-author-12a8dba09036-maximal-stationary-far-tail-access
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-truncated-null-boundary-height: mathematical-premise
  def-lipschitz-cut-area-data: mathematical-premise
  def-stationary-section-time: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  pthm-complete-maximal-slices: physical-result
  pthm-positive-transformed-lapse: physical-result
  pthm-past-boundary-localization: physical-result
  pthm-eventual-causal-access: physical-result
  pthm-causal-finite-time-escape: physical-result
  pthm-past-boundary-null-generators: physical-result
  pthm-transformed-cauchy-sections: physical-result
  pthm-adm-temporality: physical-result
  pthm-null-endpoint-map-properties: physical-result
  pthm-raychaudhuri-endpoint-jacobians: physical-result
  pthm-comparison-sphere-properties: physical-result
  math:def-axiom-of-choice: mathematical-premise
  lem-author-594d78e425ed-compact-normal-flow-and-area-distortion: mathematical-premise
  lem-author-594d78e425ed-uniform-translated-cut-localization: mathematical-premise
  lem-author-594d78e425ed-truncated-past-height-lipschitz-levels: mathematical-premise
  lem-author-594d78e425ed-negative-cut-selected-endpoints: mathematical-premise
  lem-author-594d78e425ed-multiplicity-aware-level-area-transfer: mathematical-premise
  def-near-horizon-past-boundary-sets: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  pthm-ernst-potential-existence: physical-result
  pthm-global-harrison-one-form: physical-result
  def-harrison-one-form-family: mathematical-premise
  def-harrison-one-form: mathematical-premise
  pthm-harrison-lorentzian-algebra: physical-result
  pthm-author-048251387164-sequence-closure-and-completeness: physical-result
  pthm-original-lapse-and-product: physical-result
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:thm-connectedness-characterisations: mathematical-premise
  math:cor-euclidean-spheres-are-path-connected: mathematical-premise
  math:thm-path-connected-implies-connected: mathematical-premise
  lem-author-12a8dba09036-maximal-stationary-far-tail-access: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional causal and area geometry in the positive-parameter
  smooth stationary vacuum Harrison construction; no observation is asserted.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp.25–26, proof of Lemma4.4 before coarea
      hypotheses: The fixed sufficiently small positive parameter, supplied smooth
        maximal section and localized late target of Section4, with the flow and
        cut conventions stated below.
      reading_limits: "Historical attribution-reading record retained; this
        maintenance revision checks the current original-metric supplier
        contracts and their application, without new article-PDF or
        external-proof reading. Retained prior source-input or attribution
        record: Consulted the frozen extracted article text on PDF pp. 24–26,
        including Lemmas 4.2–4.3 and the proof of Lemma 4.4 through its Jacobian
        comparison. No PDF-image verification or independent validation of the
        original proof is claimed. The declared definitions and local results
        supply the argument; the article claim supplies no premise. Fresh
        maintenance limits: current item and supplier contracts and the local
        applications were checked; no new reading of the external proof or PDF
        images is claimed."
      attribution: The truncated causal height and level-area comparison preceding
        coarea in the proof of Lemma 4.4; this citation supplies attribution
        only.
dependency_level: 29
---

## Statement

Adopt the standing regular mass-one stationary vacuum Harrison construction with original maximal outer section, $T|_S\not\equiv0$ and fixed sufficiently small positive $q$. Let $\Sigma=\Sigma_{q,0}$ be the supplied complete smooth maximal section, $v=v_q$ its temporal section time, and $\rho$ its boundary distance. Choose a sufficiently small collar $\mathcal R=\{0\le\rho\le\eta\}$ and a sufficiently late comparison target $C=C_t$ as in past-boundary localization. With the flow $\Psi$ and truncated height of [[def-truncated-null-boundary-height]], for suitable sufficiently small smoothing parameter $\delta>0$, the height $u$ is Lipschitz on $\mathcal R$, equals $-2\delta$ near $S$ and $2\delta$ near $S_\eta$, and satisfies $\Psi_{-z}(D_z)=\{u=z\}$ for every $|z|<2\delta$. For every $z\in(-\delta,-\delta/2)$, $A_z\subset A$ and
$$\mathcal H^2_{h_0}(\{u=z\})\le(1+o_\delta(1))\int_{A_z}J_2F_z\,d\mu_C\le(1+o_\delta(1))\int_AJ_2F\,d\mu_C.$$
The Jacobians and measures use the supplied fixed-metric, Gram-Jacobian and counting-multiplicity conventions; $o_\delta(1)\to0$ with the target, parameter and collar fixed.

## Facts & Assumptions

[F1] Use the exact hypotheses and interface of [[post-stationary-vacuum-model]].

[F2] Use the exact hypotheses and interface of [[def-regular-stationary-vacuum-spacetime]].

[F3] Use the exact hypotheses and interface of [[def-harrison-normalization]].

[F4] Use the exact hypotheses and interface of [[def-truncated-null-boundary-height]].

[F5] Use the exact hypotheses and interface of [[def-lipschitz-cut-area-data]].

[F6] Use the exact hypotheses and interface of [[def-stationary-section-time]].

[F7] Use the exact hypotheses and interface of [[def-spacelike-maximal-hypersurface-data]].

[F8] Use the exact hypotheses and interface of [[pthm-complete-maximal-slices]].

[F9] Use the exact hypotheses and interface of [[pthm-positive-transformed-lapse]].

[F10] Use the exact hypotheses and interface of [[pthm-past-boundary-localization]].

[F11] Use the exact hypotheses and interface of [[pthm-eventual-causal-access]].

[F12] Use the exact hypotheses and interface of [[pthm-causal-finite-time-escape]].

[F13] Use the exact hypotheses and interface of [[pthm-past-boundary-null-generators]].

[F14] Use the exact hypotheses and interface of [[pthm-transformed-cauchy-sections]].

[F15] Use the exact hypotheses and interface of [[pthm-adm-temporality]].

[F16] Use the exact hypotheses and interface of [[pthm-null-endpoint-map-properties]].

[F17] Use the exact hypotheses and interface of [[pthm-raychaudhuri-endpoint-jacobians]].

[F18] Use the exact hypotheses and interface of [[pthm-comparison-sphere-properties]].

[F19] Work in ZFC, including the Axiom of Choice and its countable and dependent choice consequences required by the local causal, collar and endpoint suppliers. [[math:def-axiom-of-choice]]

[F20] Use the exact hypotheses and interface of [[lem-author-594d78e425ed-compact-normal-flow-and-area-distortion]].

[F21] Use the exact hypotheses and interface of [[lem-author-594d78e425ed-uniform-translated-cut-localization]].

[F22] Use the exact hypotheses and interface of [[lem-author-594d78e425ed-truncated-past-height-lipschitz-levels]].

[F23] Use the exact hypotheses and interface of [[lem-author-594d78e425ed-negative-cut-selected-endpoints]].

[F24] Use the exact hypotheses and interface of [[lem-author-594d78e425ed-multiplicity-aware-level-area-transfer]].

[F25] The near-horizon definition supplies the inside-region notation $B$, its boundary-distance levels $S_\eta$, and the zero-time data $D,A,F$; it does not assert compactness of $B$. [[def-near-horizon-past-boundary-sets]]

[F26] For every individually admissible section over the actual original exterior $C_{\mathrm{ext}}$, the closure result supplies compact physical cores $B_R=\Sigma\setminus G(\{r_{\mathrm{phys}}>R\})$, including $S$, containing a neighborhood of $S$, with smooth physical graph-sphere outer boundary and compact positive-distance trims. Its proof constructs a physical exhaustion separately from an adapted topological radius. [[pthm-author-048251387164-sequence-closure-and-completeness]]

[F27] The stationary graph parameterization and the end normalization $x_q=qx$, $r_q=qr$, $t_q=d_qt/(4q)$ identify the supplied section with the graph $t_q=\widetilde u_q(x_q)$ on the end; graph height need not extend to $S$. [[def-stationary-maximal-graph]]

[F28] Under the regular vacuum, original maximal-section, mass-one and nontrivial $T|_S$ hypotheses, the Ernst-potential theorem supplies the normalized smooth stationary potential on the exterior and a neighborhood of $S$. For these data, the global one-form construction supplies one smooth stationary primitive $W_0$ with spatial components $(W_0)_i=O_5(r^{-3})$ in the original asymptotic chart, together with its normalized potential $\sigma\to1$ and pole $p$ where $T_p=0$. Use this same primitive and pole for $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $d_q=D_q(p)$. The family normalization gives $W_q(T)=d_q-D_q$. The metric definition gives the Harrison tensor formula, and its algebra theorem gives $d_q>0$ and $g_q(T,T)=d_q^2g(T,T)/(4D_q)$ on the supplied positive-denominator domain. These exact formulas and the smooth primitive's decay yield the fixed-$q$ end convergence in Proof 1.1. [[pthm-ernst-potential-existence]] [[pthm-global-harrison-one-form]] [[def-harrison-one-form-family]] [[def-harrison-one-form]] [[pthm-harrison-lorentzian-algebra]]

[F29] The original exterior is the stationary product over $C_{\mathrm{ext}}=\Sigma_0\cap\mathcal E$. Its closure $B_0=C_{\mathrm{ext}}\cup S$ has compact physical-end truncations and a separate adapted topological identification. The assumed original maximality is on this actual section. [[pthm-original-lapse-and-product]]

[F30] For totally differentiable Euclidean maps whose images lie in the next map's domain, $D(g\circ f)(a)=Dg(f(a))\circ Df(a)$. Apply this to the smooth coordinate scalings and graph maps in their open end charts. [[math:thm-chain-rule-for-total-derivatives]]

[F31] On a connected space every continuous map to the two-point discrete space is constant, equivalently there are no nonempty proper clopen subsets. The unit sphere $S^2$ is connected. Convex coordinate balls and the interiors of coordinate half-balls are path connected by straight segments, hence connected. These facts apply to the smooth section and core supplied by [F7], [F8] and [F26], and to the physical graph sphere via its diffeomorphism with $S^2$. [[math:thm-connectedness-characterisations]] [[math:cor-euclidean-spheres-are-path-connected]] [[math:thm-path-connected-implies-connected]]

[F32] The outgoing-access premise required by the eventual-access supplier is checked in the original metric before that supplier is invoked. Under the standing maximality of the actual $C_{\mathrm{ext}}=\Sigma_0\cap\mathcal E$, its original lapse/product result gives a connected smooth spherical-exterior closure, positive original lapse, a complete stationary product and compact physical-end truncations. Regularity supplies the smooth original spacelike extension across compact $S$, the ambient fields and tangency of $T$ to $S$, the asymptotically Euclidean induced end and the stationary end bounds. These are the hypotheses of the maximal-stationary far-tail lemma: every point of the original exterior reaches every sufficiently far selected stationary tail by a future original-metric timelike curve contained in that exterior. This is not an assumption about the transformed metric or an end-truncation identification. [[pthm-original-lapse-and-product]] [[def-regular-stationary-vacuum-spacetime]] [[lem-author-12a8dba09036-maximal-stationary-far-tail-access]]

## Proof

**Given:** The hypotheses in the Statement, with the ZFC convention of [F19].

**Goal:** Establish the stated conclusions.

1.1 Put $R=R_0q^{-2/3}$ in the physical comparison end, choosing $R_0$ large enough that this physical sphere and its compact original truncation are supplied. By [F29], let $C_{\mathrm{ext}}=\Sigma_0\cap\mathcal E$ and $B_0=C_{\mathrm{ext}}\cup S$, keeping its adapted topological chart separate. The section in [F8] is a connected smooth individually admissible section, with interior graph diffeomorphism $G:C_{\mathrm{ext}}\to\Sigma^\circ$; its physical normalized end is the one in [F27]. We first establish the needed end-metric convergence in the actual asymptotic chart, for this fixed $q>0$. Put $c_q=d_q/(4q)$, $y=x_q=qx$ and $s=t_q=c_qt$, and let $G_{\mu\nu}$ denote the components of $g_q$ in $(s,y)$. The original metric obeys $g_{00}\to-1$, $g_{0i}=O(r^{-2})$ and $g_{ij}\to\delta_{ij}$ by regularity. By [F28], $D_q\to4q^2>0$ uniformly in angle and $(W_q)_i=(1-q)^2(W_0)_i-4q(1-q)g_{0i}=O_q(r^{-2})$. Write $f=-g_{00}$. Substituting $W_q(T)=d_q-D_q$ in the tensor formula and rescaling coordinates gives $G_{00}=4q^2g_{00}/D_q$, $G_{0i}=g_{0i}-f(W_q)_i/D_q$, and $G_{ij}=(D_qg_{ij}+g_{0i}(W_q)_j+(W_q)_ig_{0j}-fD_q^{-1}(W_q)_i(W_q)_j)/(4q^2)$. Thus $G_{00}\to-1$, $G_{0i}\to0$ and $G_{ij}\to\delta_{ij}$ uniformly in angle. This uses the supplied smooth decaying primitive, without identifying it with the exact radial integral. The normalized graph slope tends to zero by [F8] and [F27]. Apply [F30] to the smooth graph parameterization $j(y)=(\widetilde u_q(y),y)$ and the coordinate scalings; its tangent vectors are $\partial_i+(\partial_i\widetilde u_q)\partial_s$. By the induced-metric definition in [F7], its components in $y$ are $G_{ij}+G_{0i}\partial_j\widetilde u_q+G_{0j}\partial_i\widetilde u_q+G_{00}\partial_i\widetilde u_q\partial_j\widetilde u_q$, so they tend to the Euclidean identity. Hence $h_0\ge\frac12\sum_i(dx_q^i)^2$ sufficiently far out. Since $r=|x_q|/q$ and $q>0$ is fixed, $|dr|_{h_0}\le\sqrt2/q$ there. Apply the universal physical-core conclusion in [F26] to this same individually admissible section, using a lower positive parameter bound $q/2$ if applying its constant-sequence formulation. Set $B=\Sigma\setminus G(\{r_{\mathrm{phys}}>R\})=S\cup G(B_{0,R}\setminus S)$ in the near-horizon definition. This core is compact and contains a neighborhood of $S$, has smooth outer boundary $\Gamma=G(\{r_{\mathrm{phys}}=R\})$, and has compact positive-distance trims. Put $\Omega=(\operatorname{int}_\Sigma B)\cap\Sigma^\circ$. If $\Omega$ had a separation, its two pieces would define a nonconstant continuous map to the two-point discrete space. At every point of the manifold boundary $S\sqcup\Gamma$ of $B$, a sufficiently small boundary half-ball has connected interior by [F31], so that map extends uniquely and locally constantly to $B$. The extensions agree on overlaps because those interiors are dense. Its restriction to $\Gamma$ is constant: the sphere parameterization pulls it back to a continuous map on connected $S^2$. Extend that constant to the physical graph tail, identified by the graph diffeomorphism. Boundary half-balls at $\Gamma$ make this extension continuous on the whole connected section $\Sigma$, contradicting [F31]. Hence $\Omega$ is connected. Adding $S$ preserves connectedness: any separation of $\Omega\cup S$ would restrict to a separation of $\Omega$, and every relative neighborhood of a point of $S$ meets $\Omega$. Thus $\operatorname{int}_\Sigma B$ is connected. The same half-balls show $B=\overline{\operatorname{int}_\Sigma B}^{\,\Sigma}$. Its outer sphere lies on exactly the physical comparison cylinder; hence the inside component containing $S$ in stationary projection is $\mathbb R_v\times\Omega$, where $\Omega=(\operatorname{int}_\Sigma B)\cap\Sigma^\circ$. No equality of the physical radius and an adapted topological radius is asserted. [given, F2, F6, F7, F8, F18, F19, F25, F26, F27, F28, F29, F30, F31, algebra]

1.2 The maximal-section and positive-lapse suppliers give a smooth spacelike section up to compact $S$, $N>0$ inside, $N=0$ at $S$, and $T|_S\in TS$. The causal escape supplier constructs a smooth intrinsic boundary-distance collar. Choose a sufficiently small width $\eta$ and put $\mathcal R=\{0\le\rho\le\eta\}$. The compact normal-flow lemma supplies one common smooth flow $V=Nn=T-X$ on $\mathcal R$, fixing $S$, with $v(\Psi_zx)=z$ for interior $x$ and uniform inverse-flow two-dilation $1+\epsilon(\delta)$, $\epsilon(\delta)\to0$. Smoothness of the ambient metric and embedded spacelike section up to $S$ is supplied by the section and transformed-geometry interfaces; no extension of the exterior product across the horizon is assumed. [given, F2, F6, F7, F8, F9, F12, F20]

2.1 First shrink $\eta$ so that $\mathcal R\subset\operatorname{int}_\Sigma B$, using step 1.1 and compactness of $S$; the flow and dilation bounds of step 1.2 restrict to this smaller collar. Choose $0<b<\eta/4$ sufficiently small for the compact-core supplier. By step 1.1, $B\cap\{\rho\ge b\}$ is compact in $\Sigma^\circ$. The actual original maximal section $C_{\mathrm{ext}}$ and product in [F29], together with the regular boundary-extension and physical-end data in [F2], meet every original-metric hypothesis of [F32]. The far-tail lemma therefore gives outgoing access from every original exterior point to each sufficiently far selected original stationary tail. Choose the free comparison constant beyond this background threshold before fixing the target. Thus the outgoing-access premise of [F11] is satisfied independently of any transformed chronological-access conclusion. The eventual-access supplier places the compact trim $B\cap\{\rho\ge b\}$ entirely in $I^-_{\mathcal E}(C_t)$ for all sufficiently late $t$; choose $t$ to satisfy the zero-time localization supplier as well. The target is a nonempty compact smooth spacelike sphere on the comparison cylinder. That cylinder is timelike, and its stationary $T$ flow is future timelike by the eventual-access supplier. Since $Tv=1$, increasing $t$ makes $\min_{C_t}v=t+\min_{C_0}v>0$. The causal escape supplier gives $|d\rho/dv|\le K_\rho\rho$ for a fixed constant $K_\rho\ge0$ in a stationary collar $0<\rho<a_0$; choose $a_0$ small enough that the target projects outside this collar. Thus the compact regular closed base $B$, its smooth outer boundary $\Gamma$, the collar inclusion, compact-trim entry, temporal $v$ and causal collar estimate meet the hypotheses of the translated-cut localization lemma with $Q=C=C_t$. It supplies a common time interval on which all positive- and negative-time cuts $D_z$ are compact and lie in $\Psi_z$ of a fixed compact interior annulus of $\mathcal R$, with fixed inner neighborhoods outside the chronological past and outer neighborhoods inside it. Fix this late target and shrink $\delta$ so that the common time bound holds and $\min_Cv>2\delta$. This supplies the nonzero-time localization without inferring it from the zero-time cut. [F6, F10, F11, F12, F15, F18, F21, F25, F26, step 1.1, step 1.2, F32]

3.1 The chronological past is a past set, and each interior normal flow line is future timelike. Apply the truncated-height lemma to obtain the Lipschitz threshold, its two constant boundary values, and the exact level identity for every interior slab time. Its local cone argument is carried out only on a compact annulus where $V$ is timelike; near $S$ the height is constant. Thus degeneration $V|_S=0$ does not invalidate the Lipschitz argument or any flow chart. [F4, F19, F22, step 2.1]

3.2 Global hyperbolicity, temporal $v$, compact $C$ and each compact $D_z$ now satisfy the normalized-null-flow endpoint lemmas with $v-z$. Use the same maximal past null-normal geodesic family supplied by the zero-time endpoint result. The past-boundary generator theorem applies at every $p\in D_z$ because it is inside the cylinder and $v(p)=z<\min_Cv$; its final tangent is precisely the prescribed outward normal. The selected-endpoint lemma therefore gives compact/Borel $A_z$, coverage of $D_z$ and local smooth transverse $F_z$ for every small $z$. At time zero the localization and endpoint suppliers identify these data with $D,A,F$ of the near-horizon definition. For negative $z$, the selected-endpoint lemma's boundary-cylinder argument proves $A_z\subset A$ and identifies the intermediate zero-time hit with $F$. These data meet the optical Jacobian supplier's hypotheses, which give $0\le J_2F_z\le J_2F\le1$ on $A_z$. [F13, F14, F15, F16, F17, F18, F19, F23, F25, step 2.1]

4.1 Compose each endpoint map with the inverse normal flow and apply the multiplicity-aware area-transfer lemma. Its image is exactly the level set from step 3.1, and its area formula retains all endpoint multiplicities. The uniform two-dilation factor from step 1.2 gives the first inequality; the pointwise optical comparison and $A_z\subset A$ give the second. Set $o_\delta(1)=\epsilon(\delta)$ to obtain the stated limits for fixed target, collar and parameter. The argument applies to every $z\in(-\delta,-\delta/2)$, with no unjustified regular-value or injectivity assumption. [F5, F17, F20, F24, step 1.2, step 3.1, step 3.2] ∎

## Source notes

The original Lemma4.4 proof, PDF pp.25–26, attributes the construction. Five local intermediates supply common translated localization, the flow chart and metric distortion, Lipschitz threshold/level identity, all-time selected endpoint domains and multiplicity-aware area transfer. Exact existing library achronal-boundary/flow/area inputs suffice after that chain, so no new external theorem with unmatched hypotheses is imported. The smoothing parameter delta is distinct from a lower positive q bound. No nonzero-time localization, image rectifiability or multiplicity-one assertion is inferred merely from the zero-time cut. This is an authoring proposal, not independent proof review or mathematical acceptance.

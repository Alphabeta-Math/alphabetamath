---
id: pthm-trapped-graph-focusing-contradiction
title: First cylinder contact, outward source branch and the focusing contradiction
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - pthm-negative-eigenvalue-trapped-graphs
  - pthm-timelike-path-transfer
  - pthm-transformed-cauchy-sections
  - def-stationary-section-time
  - pthm-bifurcate-horizon-preservation
  - pthm-harrison-electrovacuum
  - pthm-harrison-lorentzian-algebra
  - pthm-electrovacuum-energy-conditions
  - lem-author-fd27ddabb933-future-horizon-defining-pair
  - lem-author-fd27ddabb933-outward-graph-null-initial-jets
  - lem-author-fd27ddabb933-inward-null-local-horizon-crossing
  - lem-author-fd27ddabb933-inward-branch-exterior-exclusion
  - lem-author-fd27ddabb933-outward-null-affine-normalization
  - lem-author-fd27ddabb933-compact-first-cylinder-contact
  - lem-author-fd27ddabb933-first-contact-chronological-boundary
  - lem-author-fd27ddabb933-source-normal-null-generator
  - lem-author-fd27ddabb933-first-contact-target-normal
  - lem-author-fd27ddabb933-killing-energy-conservation
  - lem-author-fd27ddabb933-asymptotic-null-energy-speed
  - lem-author-fd27ddabb933-compact-source-energy-bound
  - lem-author-fd27ddabb933-distant-target-affine-length
  - lem-author-fd27ddabb933-finite-segment-focusing-contradiction
  - math:def-axiom-of-choice
  - pthm-ernst-potential-existence
  - def-killing-ernst-notation
  - pthm-global-harrison-one-form
  - def-coordinate-comparison-spheres
  - pthm-eventual-causal-access
  - def-harrison-one-form-family
  - def-harrison-one-form
  - math:thm-algebra-of-derivatives
  - math:thm-chain-rule-for-total-derivatives
  - math:lem-fundamental-theorem-and-integration-by-parts
  - math:thm-monotonicity-of-the-integral
  - pthm-original-lapse-and-product
  - math:thm-heine-borel-rn
  - math:thm-compactness-agrees-with-metric-compactness
  - math:thm-compactness-under-continuous-maps
  - math:thm-compact-subset-of-a-hausdorff-space-is-closed
  - math:def-compact-space
  - math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric
  - math:thm-euclidean-space-complete
  - physics:def-gr-metric-volume-form-and-current-flux
  - lem-author-12a8dba09036-maximal-stationary-far-tail-access
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  pthm-negative-eigenvalue-trapped-graphs: physical-result
  pthm-timelike-path-transfer: physical-result
  pthm-transformed-cauchy-sections: physical-result
  def-stationary-section-time: mathematical-premise
  pthm-bifurcate-horizon-preservation: physical-result
  pthm-harrison-electrovacuum: physical-result
  pthm-harrison-lorentzian-algebra: physical-result
  pthm-electrovacuum-energy-conditions: physical-result
  lem-author-fd27ddabb933-future-horizon-defining-pair: mathematical-premise
  lem-author-fd27ddabb933-outward-graph-null-initial-jets: mathematical-premise
  lem-author-fd27ddabb933-inward-null-local-horizon-crossing: mathematical-premise
  lem-author-fd27ddabb933-inward-branch-exterior-exclusion: mathematical-premise
  lem-author-fd27ddabb933-outward-null-affine-normalization: mathematical-premise
  lem-author-fd27ddabb933-compact-first-cylinder-contact: mathematical-premise
  lem-author-fd27ddabb933-first-contact-chronological-boundary: mathematical-premise
  lem-author-fd27ddabb933-source-normal-null-generator: mathematical-premise
  lem-author-fd27ddabb933-first-contact-target-normal: mathematical-premise
  lem-author-fd27ddabb933-killing-energy-conservation: mathematical-premise
  lem-author-fd27ddabb933-asymptotic-null-energy-speed: mathematical-premise
  lem-author-fd27ddabb933-compact-source-energy-bound: mathematical-premise
  lem-author-fd27ddabb933-distant-target-affine-length: mathematical-premise
  lem-author-fd27ddabb933-finite-segment-focusing-contradiction: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  pthm-ernst-potential-existence: physical-result
  def-killing-ernst-notation: mathematical-premise
  pthm-global-harrison-one-form: physical-result
  def-coordinate-comparison-spheres: mathematical-premise
  pthm-eventual-causal-access: physical-result
  def-harrison-one-form-family: mathematical-premise
  def-harrison-one-form: mathematical-premise
  math:thm-algebra-of-derivatives: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:lem-fundamental-theorem-and-integration-by-parts: mathematical-premise
  math:thm-monotonicity-of-the-integral: mathematical-premise
  pthm-original-lapse-and-product: physical-result
  math:thm-heine-borel-rn: mathematical-premise
  math:thm-compactness-agrees-with-metric-compactness: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:thm-compact-subset-of-a-hausdorff-space-is-closed: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric: mathematical-premise
  math:thm-euclidean-space-complete: mathematical-premise
  physics:def-gr-metric-volume-form-and-current-flux: mathematical-premise
  lem-author-12a8dba09036-maximal-stationary-far-tail-access: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional fixed-positive-parameter smooth stationary
  vacuum/Harrison construction with a supplied complete maximal section and
  smooth bifurcation neighborhood; no assertion at the degenerate parameter
  endpoint.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p.27, proof of Theorem4.2, first-cylinder-contact and
        inward-branch/focusing paragraph
      reading_limits: Historical attribution-reading record retained; this maintenance
        revision checks the current original-metric supplier contracts and their
        application, without new article-PDF or external-proof reading. Read the
        frozen original article text at p.27 and inspected its page27 image. It
        is attribution only; the local branch exclusion, compact first-contact
        argument and quantitative affine-length estimate are supplied by the new
        local chain.
dependency_level: 25
---

## Statement

Adopt the regular mass-one stationary vacuum/Harrison construction with maximal original exterior section and $T|_S\not\equiv0$. Fix $q\in(0,1]$ and the supplied complete smooth spacelike maximal stationary graph section $\Sigma_q$ with boundary S and its smooth spacelike extension across S. Suppose the outward stability operator has negative principal eigenvalue. Choose a sufficiently small outward graph $A=S_\epsilon$ from the positive principal eigenfunction family, so that its expansion in the exact initial null gauge $L_\epsilon=n_q+\nu_{q,\epsilon}$ satisfies $\theta_{L_\epsilon}\le-\delta_*<0$. The positive number delta* is attached to this single fixed graph, not to a parameter-uniform estimate.

For every sufficiently distant normalized end radius R, timelike transfer gives access to the stationary cylinder over that coordinate sphere. There is an earliest stationary translate of the compact target cut meeting $J^+_{\mathcal E,g_q}(A)$. A contact point is joined to A by a future null geodesic entirely in $\partial J^+(A)$, orthogonal to both surfaces and without a focal point to A strictly before the target. Its initial ray is outgoing: the inward initial family from these sufficiently small graphs hits the preserved local future horizon in affine time of order epsilon and cannot remain in the open exterior to a distant target.

Normalize the initial tangent to be exactly $L_\epsilon$. Its stationary Killing energy has a bound depending only on the fixed compact source. The asymptotically flat end then gives $\ell_R\ge(R-R_1)/(CE_{\max})$ for the affine segment length. Choosing R so that this is larger than $2/\delta_*$ contradicts the focal-free property by null Raychaudhuri and nonnegative null Ricci curvature. Thus the negative-eigenvalue outer-trapped graph alternative cannot occur in this setting. All causal relations are relative to the open exterior; the short inward crossing is proved in the smooth ambient metric near S. No causal assertion at $q=0$ or null-geodesic completeness is assumed.

## Facts & Assumptions

[F1] Adopt the stationary vacuum model as conditional assumptions. [[post-stationary-vacuum-model]]

[F2] The original chronological exterior has a stationary asymptotically flat end and a smooth bifurcation sphere S, with T tangent to S. [[def-regular-stationary-vacuum-spacetime]]

[F3] A negative principal eigenvalue supplies arbitrarily small smooth outward normal graphs with negative outgoing expansion in the gauge n plus nu. [[pthm-negative-eigenvalue-trapped-graphs]]

[F4] Smooth original future timelike paths transfer to smooth future $g_q$-timelike paths with the same initial point and spatial path. [[pthm-timelike-path-transfer]]

[F5] For the selected complete maximal section at each fixed positive q, the exterior is globally hyperbolic and its section time is temporal with all translates Cauchy. [[pthm-transformed-cauchy-sections]]

[F6] The section time vanishes on the selected section and increases by the stationary flow parameter. [[def-stationary-section-time]]

[F7] The same local future and past horizon branches are smooth null branches for $g_q$, and S remains spacelike. [[pthm-bifurcate-horizon-preservation]]

[F8] The metric is smooth across S on the supplied neighborhood, and the Einstein–Maxwell equations hold in the exterior and there. [[pthm-harrison-electrovacuum]]

[F9] The transformed metric is Lorentzian, stationary and has the specified future orientation. [[pthm-harrison-lorentzian-algebra]]

[F10] The normalized smooth stationary Ernst potential obeys $d\sigma=2T^b\mathcal F_{ba}\,dx^a$ and $\sigma\to1$. The construction supplies a single smooth stationary normalized primitive $W_0$, with $(W_0)_i=O_5(r^{-3})$ in the original end chart; this primitive need not equal the exact radial integral. [[pthm-ernst-potential-existence]] [[def-killing-ernst-notation]] [[pthm-global-harrison-one-form]]

[F11] The coordinate comparison convention defines the cut at original time zero and its translates by the complete stationary flow, with increasing Cartesian radius giving the outer radial direction. At fixed $q>0$ its free constant $R_0$ may be increased. [[def-coordinate-comparison-spheres]]

[F12] Null Ricci curvature is nonnegative for the transformed metric throughout the exterior. [[pthm-electrovacuum-energy-conditions]]

[F13] A framed local bifurcate tube describes the exterior by a positive defining pair, with the future outgoing branch correctly labeled. [[lem-author-fd27ddabb933-future-horizon-defining-pair]]

[F14] Small outward graph initial data have positive defining functions of order epsilon and the stated inward-null jets. [[lem-author-fd27ddabb933-outward-graph-null-initial-jets]]

[F15] The inward normalized family crosses the local future horizon in short affine time, inside a fixed compact tube. [[lem-author-fd27ddabb933-inward-null-local-horizon-crossing]]

[F16] An exterior-contained segment to a target outside that tube cannot be on the inward source ray. [[lem-author-fd27ddabb933-inward-branch-exterior-exclusion]]

[F17] The remaining source ray has the exact outgoing affine normalization n plus nu. [[lem-author-fd27ddabb933-outward-null-affine-normalization]]

[F18] At each fixed positive parameter, sufficiently large freely chosen comparison spheres have eventual chronological access from every point of the chosen maximal section interior, uniformly on compact subsets of that section. This result already supplies the finite smooth-piece transfer argument. [[pthm-eventual-causal-access]]

[F19] The closed causal future and a bounded-time compact cylinder slab give an earliest causal contact. [[lem-author-fd27ddabb933-compact-first-cylinder-contact]]

[F20] That first contact belongs to the chronological and causal future boundary and has positive section time. [[lem-author-fd27ddabb933-first-contact-chronological-boundary]]

[F21] Time reversal of the compact-target theorem gives a source-normal null boundary segment with no interior focal point from the source. [[lem-author-fd27ddabb933-source-normal-null-generator]]

[F22] Local endpoint variation gives target orthogonality, and temporal coordinate time excludes an inward final target ray. [[lem-author-fd27ddabb933-first-contact-target-normal]]

[F23] Stationary Killing energy is conserved even while T is not timelike in the inner region. [[lem-author-fd27ddabb933-killing-energy-conservation]]

[F24] Far-end null speed is bounded by a constant times the positive stationary energy. [[lem-author-fd27ddabb933-asymptotic-null-energy-speed]]

[F25] The fixed compact normalized source field gives one target-independent upper bound for that energy. [[lem-author-fd27ddabb933-compact-source-energy-bound]]

[F26] The final passage from a fixed end radius to radius R forces affine length growing linearly with R. [[lem-author-fd27ddabb933-distant-target-affine-length]]

[F27] An existing focal-free segment longer than the negative-expansion focal bound yields the Raychaudhuri contradiction without a completeness assumption. [[lem-author-fd27ddabb933-finite-segment-focusing-contradiction]]

[F28] Work in ZFC, carrying the causal, compactness and geodesic supplier assumptions. [[math:def-axiom-of-choice]]

[F29] Use $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, its contraction $W_q(T)=d_q-D_q$, and the defining tensor formula $g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q)$. At the pole $d_q=(1+q)^2+(1-q)^2\psi(p)^2>0$. [[def-harrison-one-form-family]] [[def-harrison-one-form]]

[F30] Coordinatewise product and quotient differentiation, the total chain rule, the fundamental theorem of calculus on finite intervals, and monotonicity of the integral apply to the smooth end coefficients. They may be iterated a finite number of times; denominators are restricted to tails where they are bounded away from zero. [[math:thm-algebra-of-derivatives]] [[math:thm-chain-rule-for-total-derivatives]] [[math:lem-fundamental-theorem-and-integration-by-parts]] [[math:thm-monotonicity-of-the-integral]]

[F31] The original section interior $C$ has the smooth stationary-flow product $\mathcal E=\mathbb R\times C$. Its positive induced metric $h$ has components $h_{ij}=g_{ij}$ on the designated end, since the original section agrees there with original time zero. The global section chart is not assumed to agree with the end chart. [[pthm-original-lapse-and-product]] [[def-regular-stationary-vacuum-spacetime]]

[F32] Closed bounded Euclidean sets are compact, metric compactness agrees with topological compactness, continuous maps preserve compactness, and compact subsets of Hausdorff spaces are closed. Compactness gives finite subcovers in the subspace topology. A smooth positive metric is uniformly comparable with the Euclidean metric on compact coordinate sets, and Euclidean space is complete. [[math:thm-heine-borel-rn]] [[math:thm-compactness-agrees-with-metric-compactness]] [[math:thm-compactness-under-continuous-maps]] [[math:thm-compact-subset-of-a-hausdorff-space-is-closed]] [[math:def-compact-space]] [[math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric]] [[math:thm-euclidean-space-complete]]

[F33] In an oriented Lorentzian coordinate chart the metric volume coefficient is $\sqrt{|\det(g_{ab})|}$, so on this signature $(-,+,+,+)$ end it is $\sqrt{-\det g}$. Only this coordinate-density definition is used. [[physics:def-gr-metric-volume-form-and-current-flux]]

[F34] The outgoing-access premise required by the eventual-access supplier is checked in the original metric before that supplier is invoked. Under the standing maximality of the actual $C=\Sigma_0\cap\mathcal E$, its original lapse/product result gives a connected smooth spherical-exterior closure, positive original lapse, a complete stationary product and compact physical-end truncations. Regularity supplies the smooth original spacelike extension across compact $S$, the ambient fields and tangency of $T$ to $S$, the asymptotically Euclidean induced end and the stationary end bounds. These are the hypotheses of the maximal-stationary far-tail lemma: every point of the original exterior reaches every sufficiently far selected stationary tail by a future original-metric timelike curve contained in that exterior. This is not an assumption about the transformed metric or an end-truncation identification. [[pthm-original-lapse-and-product]] [[def-regular-stationary-vacuum-spacetime]] [[lem-author-12a8dba09036-maximal-stationary-far-tail-access]]

## Proof

**Given:** The assumptions in the Statement.

**Goal:** Establish the stated conditional claim.

1.1 We first derive the end bounds for the actual smooth primitive in [F10]. Stationarity and [F2] give $F=\tfrac12dT^\flat=O_5(r^{-2})$. Cofactor expansion verifies that the inverse metric is the transposed cofactor matrix divided by its determinant, which tends to $-1$; the Hodge formula in [F10] uses these entries and the volume coefficient $\sqrt{-\det g}$ from [F33]. Repeated coordinate differentiation using [F30] therefore gives $\mathcal F=O_5(r^{-2})$ and $d\sigma=O_5(r^{-2})$. For each unit vector $\omega$, apply the fundamental theorem on $[r,b]$ to the real and imaginary parts of $\sigma(s\omega)$, bound their derivatives by a constant times $s^{-2}$ using monotonicity, and let $b\to\infty$ using the supplied normalization. This gives $\sigma-1=O(r^{-1})$ uniformly in $\omega$; the bounds for $d\sigma$ give all spatial derivatives through order six, so $\sigma-1=O_6(r^{-1})$. For fixed $q>0$, [F29] then gives $D_q=4q^2+O_6(r^{-1})$, $(W_q)_i=O_5(r^{-2})$ and $(W_q)_0=d_q-D_q$. Put $c_q=d_q/(4q)>0$, $t_q=c_qt$, $y=x_q=qx$, $r_q=|y|$ and let $G_{\mu\nu}$ be the normalized metric components. Direct substitution in [F29], with $f=-g_{00}$ and $W_i=(W_q)_i$, gives $G_{00}=4q^2g_{00}/D_q$, $G_{0i}=g_{0i}-fW_i/D_q$ and $G_{ij}=(D_qg_{ij}+g_{0i}W_j+W_ig_{0j}-fW_iW_j/D_q)/(4q^2)$. The denominators have positive limits. Iterating the same product, quotient and chain rules through order five yields $G_{00}=-1+O_5(r_q^{-1})$, $G_{0i}=O_5(r_q^{-2})$ and $G_{ij}=\delta_{ij}+O_5(r_q^{-1})$. In this calculation $\partial_y=q^{-1}\partial_x$, with $q$ fixed; no parameter-uniform bounds or exact radial gauge are used. Finally $T=c_q\partial_{t_q}$ is future timelike far out by [F9]. [given, F2, F9, F10, F29, F30, F33, algebra]

2.1 We verify that sufficiently distant outer regions have no hidden boundary in the exterior. Work first on the original section $C$ with its positive metric $h$ in [F31]. Choose an original end radius $a$ so large that $h\ge\tfrac12\delta$ for $r\ge a$, and write $V_a=\{r>a\}\subset C$. Its coordinate cut $S_a=\{r=a\}$ is compact and closed in $C$ by [F32]. If $p\in\overline{V_a}^{\,C}\setminus S_a$, choose a relatively compact coordinate ball $V$ about $p$, convex in those local coordinates and disjoint from $S_a$. Take $z\in V\cap V_a$. A straight coordinate segment from $z$ to any point of $V$ has uniformly bounded $h$-speed, by the compact-coordinate comparison in [F32]. As long as the segment is in $V_a$, its end coordinate speed satisfies $|dx/ds|\le\sqrt2\,|\dot\gamma|_h$. At a proposed first exit, this bound and the fundamental theorem in [F30] make its end coordinates Cauchy, hence convergent to a finite point of $\mathbb R^3$ by completeness in [F32]. That limit has radius at least $a$; radius $a$ would put the segment on the excluded $S_a$, and radius greater than $a$ continues it inside the open end chart. Thus no exit is possible: $V\subset V_a$, with end radius bounded on $V$ by $r(z)$ plus a fixed multiple of its coordinate diameter. It follows that $\overline{V_a}^{\,C}=V_a\cup S_a$ and $\partial_CV_a=S_a$; the points of $S_a$ are boundary points by their end chart. Every point of $C$ has a neighborhood on whose intersection with $V_a$ the radius is bounded: use the end chart on $V_a\cup S_a$ and the complement of its closure elsewhere. A finite subcover shows that the radius on any compact subset of $C$ is bounded wherever that subset meets $V_a$. The projection $\pi:\mathcal E\to C$ is smooth by [F31], so the projection of any compact source is compact by [F32]. Choose a fixed larger normalized radius $R_1$ above the bound for that projection and above the far-end threshold in [F24]. The product agrees with the designated end because the section is original time zero there and both flows have velocity $T$. Consequently, for every $R\ge R_1$, the region $U_R=\{r_q>R\}\subset\mathcal E$ has closure $\{r_q\ge R\}$ and boundary the entire cylinder $\{r_q=R\}$, with the source disjoint from its closure. Its closed outer region is covered by a slightly larger end chart. This argument uses no compatibility between the global section chart and the end chart. [F2, F24, F30, F31, F32, step 1.1]

3.1 The candidate section and the preserved horizon data in [F7] give a future/outward normal frame on compact S. The future outgoing ray is tangent to the local future branch: this agrees with the original future branch, and preservation of its null direction and the future orientation in [F7]–[F9] keep the label unchanged; replacing the reference spacelike section by the chosen one changes its future/outward frame by a boost. Since T is tangent to the spacelike S, choose the local tube with compact closure so small that $g_q(T,T)>-c_q^2/4$ there, with $c_q$ from step 1.1. Apply [F13]–[F15] in this tube, restricting their common short affine interval if necessary. Their local defining pair and initial-data calculation show that every sufficiently small outward graph is in the exterior and that its inward null normal reaches the local future branch before leaving this fixed tube. The graph family in [F3] is trapped for all sufficiently small epsilon, so choose one epsilon meeting both requirements and then fix its delta*. Use step 2.1 for this single compact graph A to fix $R_1$ once and for all. [F2, F3, F7, F8, F9, F13, F14, F15, given, step 1.1, step 2.1]

4.1 Step 1.1 gives $g_q(T,T)=c_q^2G_{00}<-c_q^2/2$ far out, uniformly in stationary time. Thus every sufficiently distant target cylinder is disjoint from the compact tube chosen in step 3.1. By [F16], an exterior-contained source-normal segment to such a target cannot have the inward source ray. This proves the precise local branch exclusion needed here, without asserting a global transformed event-horizon theorem. [F15, F16, step 1.1, step 3.1, algebra]

4.2 Fix one sufficiently large normalized R, above $R_1$, and set the free comparison constant to $R_0=Rq^{-1/3}$. Its original comparison radius $R_0q^{-2/3}=R/q$ is exactly the desired radius. At fixed q, taking R sufficiently large meets the comparison-range threshold in [F18]. The cuts in [F11] are therefore $C_s=\{r_q=R,t_q=c_qs\}$, with the same original stationary flow parameter $s$ used by the section time. Step 1.1 and [F24] make them compact smooth spacelike cuts, with a timelike cylinder and temporal $t_q$ on a neighborhood of its closed outer region. The source lies inside in the precise sense of step 2.1. The actual original maximal section in [F31] has the positive lapse, smooth compact-boundary spherical exterior, physical compact truncations and complete original stationary product specified in [F34]. Its ambient boundary extension, tangent field and end bounds are the regular data [F2]. Thus the far-tail lemma in [F34] applies in the original metric and proves outgoing access for every point of $\mathcal E$ to every sufficiently far original tail. Choose the present free target radius beyond that threshold as well. This verifies the additional outgoing-access hypothesis of [F18] before applying it. Apply [F18] to the compact graph $A\subset\Sigma_q^\circ$: it supplies finite chronological access to this cylinder through the original-path transfer in [F4], without assuming that smooth-path transfer applies to every absolutely continuous curve. The flow parameter map is smooth and defined for all real times by [F31]. The section time in [F5]–[F6] satisfies $\tau|_A=0$ and $\tau(\phi_s^T x)=s+\tau(x)$, and the exterior is globally hyperbolic. All hypotheses of [F19] now hold, so it supplies an earliest contact $p_R$. Compactness here is of A, the target cut and a bounded-time cylinder slab, rather than of the full cylinder. [F4, F5, F6, F11, F18, F19, F24, F31, step 1.1, step 2.1, step 3.1, F34]

5.1 By [F20], $p_R$ lies on the future chronological and causal boundary of A and has strictly positive section time; no sign of the stationary cut parameter is needed. Apply [F21], which reverses time and uses compact target A with temporal function minus the section time. It supplies a null segment from A to $p_R$ with source orthogonality and no interior focal point measured from A. The local target variation in [F22] makes the same segment orthogonal to the target cut. Its additional outward-ray hypotheses hold by steps 2.1 and 4.2: the cylinder bounds $U_R$, A is outside its closure, $t_q$ is temporal there, $T=c_q\partial_{t_q}$, and the very same cuts have $t_q=c_qs$. Thus the final ray is outward. The segment remains wholly in the open exterior. Step 4.1 excludes its inward source ray, so [F17] fixes its affine initial tangent to be exactly n plus nu. [F17, F20, F21, F22, step 2.1, step 4.1, step 4.2]

6.1 The metric is stationary by [F9], so [F23] conserves the Killing energy along these affinely normalized segments, including any part in an ergoregion. The smooth outgoing source field on fixed compact A gives $0<E\le E_{\max}$ for every segment arriving at the end, by [F25]. The algebraic null-cone estimate [F24] applies to the actual normalized end of step 1.1. For the fixed radius $R_1$ chosen in step 3.1, step 2.1 verifies both additional last-passage hypotheses: $A\cap\overline{U_{R_1}}^{\,\mathcal E}=\varnothing$ and $\partial_{\mathcal E}U_{R_1}=\{r_q=R_1\}$. Therefore [F26] gives $\ell_R\ge(R-R_1)/(CE_{\max})$, with $R_1$, C and $E_{\max}$ independent of the target radius and target translation. [F9, F23, F24, F25, F26, step 1.1, step 2.1, step 3.1, step 5.1]

7.1 Increase R so that the displayed bound exceeds two divided by delta*. The segment itself now exists past that bound by the first-contact construction. The normal-geodesic flow gives a local congruence along its finite interval as explained in [F27]. Use null convergence [F12], the fixed outgoing expansion bound from [F3] and the exact normalization in step 5.1. Raychaudhuri forces a focal point strictly before the target, whereas [F21] excludes it. This contradiction rules out the original negative-eigenvalue graph alternative. No extension of an unconstructed geodesic to infinity is used. [F3, F12, F21, F27, F28, step 3.1, step 5.1, step 6.1, contradiction] ∎

## Source notes

The retained local intermediate items supply inward-branch exclusion near the preserved future horizon, compact first contact with the correct source-focal orientation, and the energy/affine-length/focusing estimate. The inward exclusion applies to the arbitrarily small eigenfunction graphs actually supplied. The current eventual-access theorem supplies the smooth-piece transfer and compact access. The original article is used only for attribution, and no original-article defect is asserted.

The fixed-positive-parameter end estimates above are derived for the supplied smooth decaying primitive. The outer-region check uses the original positive section metric and its stationary product. All local arguments and their provenance are proposed content, without independent acceptance.

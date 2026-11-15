---
id: pthm-author-048251387164-sequence-closure-and-completeness
title: Sequence closedness and completeness without an interval-family premise
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - pthm-global-harrison-one-form
  - pthm-author-048251387164-indexed-admissible-end-estimates
  - pthm-author-048251387164-indexed-height-and-horizon-estimates
  - pthm-hawking-graph-height
  - pthm-author-048251387164-sequence-compact-angle-and-lapse
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-maximal-graph
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - math:def-axiom-of-choice
  - math:thm-arzela-ascoli-for-real-ck
  - pthm-harrison-electrovacuum
  - pthm-transformed-end-geometries
  - lem-author-840894718169-uniform-gaussian-flow-cone
  - math:thm-chain-rule-for-total-derivatives
  - pthm-original-lapse-and-product
  - math:thm-heine-borel-rn
  - math:thm-finite-products-of-compact-spaces
  - math:thm-compactness-under-continuous-maps
  - math:thm-closed-subspace-of-a-compact-space-is-compact
  - math:thm-compact-subset-of-a-hausdorff-space-is-closed
  - math:cor-euclidean-spheres-are-path-connected
  - math:thm-path-connected-implies-connected
  - math:thm-connectedness-characterisations
  - math:lem-schwartz-cutoffs-from-the-standard-smooth-step
  - math:lem-fundamental-theorem-and-integration-by-parts
  - math:thm-compactness-agrees-with-metric-compactness
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:def-compact-space
  - pthm-common-reference-collar
  - pthm-boundary-normal-angle
  - lem-author-840894718169-fixed-target-collar-properness
  - lem-author-840894718169-boundary-one-sheet-normal-graph
  - lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant
  - math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves
  - math:thm-bolzano-weierstrass
  - math:thm-continuous-implies-integrable
  - math:lem-uniform-integral-error-bound
  - math:thm-collar-neighborhood-theorem
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  pthm-global-harrison-one-form: physical-result
  pthm-author-048251387164-indexed-admissible-end-estimates: physical-result
  pthm-author-048251387164-indexed-height-and-horizon-estimates: physical-result
  pthm-hawking-graph-height: physical-result
  pthm-author-048251387164-sequence-compact-angle-and-lapse: physical-result
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-arzela-ascoli-for-real-ck: mathematical-premise
  pthm-harrison-electrovacuum: physical-result
  pthm-transformed-end-geometries: physical-result
  lem-author-840894718169-uniform-gaussian-flow-cone: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  pthm-original-lapse-and-product: physical-result
  math:thm-heine-borel-rn: mathematical-premise
  math:thm-finite-products-of-compact-spaces: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:thm-closed-subspace-of-a-compact-space-is-compact: mathematical-premise
  math:thm-compact-subset-of-a-hausdorff-space-is-closed: mathematical-premise
  math:cor-euclidean-spheres-are-path-connected: mathematical-premise
  math:thm-path-connected-implies-connected: mathematical-premise
  math:thm-connectedness-characterisations: mathematical-premise
  math:lem-schwartz-cutoffs-from-the-standard-smooth-step: mathematical-premise
  math:lem-fundamental-theorem-and-integration-by-parts: mathematical-premise
  math:thm-compactness-agrees-with-metric-compactness: mathematical-premise
  math:lem-compactness-of-a-subspace-is-ambient: mathematical-premise
  math:def-compact-space: mathematical-premise
  pthm-common-reference-collar: physical-result
  pthm-boundary-normal-angle: physical-result
  lem-author-840894718169-fixed-target-collar-properness: mathematical-premise
  lem-author-840894718169-boundary-one-sheet-normal-graph: mathematical-premise
  lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant: mathematical-premise
  math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves: mathematical-premise
  math:thm-bolzano-weierstrass: mathematical-premise
  math:thm-continuous-implies-integrable: mathematical-premise
  math:lem-uniform-integral-error-bound: mathematical-premise
  math:thm-collar-neighborhood-theorem: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Rigidity of stationary black holes with small ADM angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: Section 5.1, equations (5.4)–(5.5); Section 5.2, equations (5.15),
        (5.22); Section 5.3, Lemma 5.1 and equation (5.24)
      statement: In the stated regular stationary vacuum and Harrison setting, Radu
        discusses lapse and height estimates and proves a compact-graph
        convergence result used in a continuation argument.
      hypotheses: The source assumes its GR, SBS and maximality conditions, and Lemma
        5.1 concerns compact maximal stationary graphs with specified boundary,
        topology, and uniform lapse and height bounds.
      reading_limits: "Retained prior source-input or attribution record: Consulted
        the cited HTML passages in this adjudication. They provide the
        background and motivation for this adapted statement; they do not assert
        this item's indexed noncompact strengthening. The numbered local
        argument uses only the declared suppliers; no independent proof audit of
        the source is claimed. Fresh maintenance limits: current item and
        supplier contracts and the local applications were checked; no new
        reading of the external proof or PDF images is claimed."
physical_scope: Conditional mathematical estimates and continuation for the
  regular stationary vacuum/Harrison construction. Existence is never presumed
  at an unavailable parameter. No empirical claim or q=0 conclusion.
dependency_level: 19
---

## Statement

Work in ZFC. Assume the stationary vacuum model and regular non-degenerate stationary spacetime data. Put $C=\Sigma_0\cap\mathcal E$ and $B_0=C\cup S$, and assume $H_g|_C=0$ for the original metric $g$. Normalize the selected physical end of this actual section to ADM mass one, and assume $T|_S\not\equiv0$. Use the resulting Harrison family with the same normalized Ernst data, pole and single smooth stationary primitive as in the indexed estimates. Throughout, the original reference section is this $B_0$; its adapted topological identification and the physical stationary end chart remain separate.

Fix $0<\delta\le1$. Use individual admissibility in the sense of the indexed end-estimates supplier, with this fixed background.

For every sequence $(q_j,\Sigma_j)$ of individually admissible pairs with $q_j\to q_*\in[\delta,1]$, there is a subsequence converging locally smoothly in the interior and smoothly as normal graphs up to S to an individually admissible $g_{q_*}$-maximal section. Its interior is a global stationary graph, its normalized end has the stated common decay through four derivatives, and it is complete up to its included boundary S. This conclusion requires no family defined at other parameters. For every sufficiently large physical end radius $R$, the section minus its open physical graph tail is a compact smooth region containing a neighborhood of $S$, with manifold boundary $S\sqcup G(\{r_{\mathrm{phys}}=R\})$ and compact positive-boundary-distance trims in the interior. These physical-core and completeness conclusions also hold for every individually admissible section, using its own end constants. No matching of the adapted topological radius with $r_{\mathrm{phys}}$ is required.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-harrison-normalization]]

[[pthm-author-048251387164-indexed-admissible-end-estimates]]

[[pthm-global-harrison-one-form]]

[[pthm-harrison-electrovacuum]]

[[def-stationary-maximal-graph]]

## Facts & Assumptions

[A1] The background is the stationary vacuum model with all four regular-spacetime conditions. The actual original exterior is $C=\Sigma_0\cap\mathcal E$, with smooth closure $B_0=C\cup S$, and its maximality hypothesis is $H_g|_C=0$. The selected physical end of this section has the ADM mass-one normalization, and $T|_S\not\equiv0$. These are the same background hypotheses used by the three indexed suppliers in [F1], the smooth primitive in [F4] and the conditional stationary product in [F7]. The original section used for normalization and graphs is $B_0$. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]] [[def-harrison-normalization]]

[F1] Under [A1], the indexed end upper-lapse bounds, uniform smooth horizon graphs and sequence compact estimates apply on any fixed positive parameter interval. For the sequence in the Statement use $\delta_0=\delta/2$ and the eventual tail in $[\delta_0,1]$ selected in step 1.1. These estimates are [[pthm-author-048251387164-indexed-admissible-end-estimates]], [[pthm-author-048251387164-indexed-height-and-horizon-estimates]] and [[pthm-author-048251387164-sequence-compact-angle-and-lapse]].

[F2] The Harrison metrics are jointly smooth. [[pthm-harrison-electrovacuum]] Graphs, smooth spacelike maximality, completeness up to boundary and Holder norms use [[def-stationary-maximal-graph]], [[def-spacelike-maximal-hypersurface-data]] and [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]].

[F3] Arzela–Ascoli applies componentwise to an equicontinuous bounded family on compact metric sets. [[math:thm-arzela-ascoli-for-real-ck]] Work in ZFC with its inherited countable/dependent choice. [[math:def-axiom-of-choice]]

[F4] Apply the additional positive-parameter smooth-global-primitive branch of [[pthm-transformed-end-geometries]] to the same regular mass-one construction, actual physical exterior section $C$ with $H_g|_C=0$, $T|_S\not\equiv0$, pole and normalization used in [F1]. Its actual single smooth primitive is supplied by [[pthm-global-harrison-one-form]], with $(W_0)_i=O_5(r^{-3})$ and normalized contraction; no exact radial identity is assumed. In the physical normalized coordinates $(t_q,x_q)$, this branch gives $(g_q)_{00}=-1+O_5(r_q^{-1})$, $(g_q)_{0i}=O_5(r_q^{-2})$ and $(g_q)_{ij}=\delta_{ij}+O_5(r_q^{-1})$, with a common end and constants for $q\in[\delta_0,1]$. This end conclusion does not identify physical and topological reference radii.

[F5] The common Gaussian collar used by the horizon estimates in [F1] has jointly smooth normal exponential maps $\Psi_q(\tau,x)=\exp_x^{(q)}(\tau\bar n_q(x))$ and jointly smooth inverse coordinates. These are the common maps of [[lem-author-840894718169-uniform-gaussian-flow-cone]], applied to the same smooth Lorentzian family, uniformly spacelike reference collar, smooth reference normals and signed boundary collars, and fixed Killing boost data used in [F1]. Restrict those background maps to $q\in[\delta_0,1]$ and the smaller common graph domain in [F1]; their existence does not require candidate sections at other parameters.

[F6] For totally differentiable Euclidean maps whose images lie in the next map's domain, $D(g\circ f)(a)=Dg(f(a))\circ Df(a)$. [[math:thm-chain-rule-for-total-derivatives]] We apply it repeatedly to the smooth heights and the affine spatial scalings specified in [F2], through order four.

[F7] Under the regular vacuum and actual-exterior maximality hypotheses in [A1], put $C=\Sigma_0\cap\mathcal E$ and $B_0=C\cup S$. The original product theorem gives a connected smooth spherical exterior $B_0$, compact smooth physical truncations $B_{0,R}=B_0\setminus\{r_{\mathrm{phys}}>R\}$, and the stationary product over $C$. Separately choose its adapted topological identification $y:B_0\to\{|y|\ge1\}$ and put $s=|y|$. This $s$ is continuous up to $S$ and has $S=\{s=1\}$, but it is not identified with the physical end radius $r_{\mathrm{phys}}=|x|$. The interior limit graph is a diffeomorphism $G:C\to\Sigma_*^\circ$. Only on the physical end do we use $r_{q_*}=q_*r_{\mathrm{phys}}$. [[pthm-original-lapse-and-product]] [[def-stationary-maximal-graph]]

[F8] Closed bounded subsets of Euclidean space, in particular finite closed intervals and closed annuli in $\mathbb R^3$, are compact. [[math:thm-heine-borel-rn]] Finite products of compact spaces are compact. [[math:thm-finite-products-of-compact-spaces]] Continuous images of compact spaces are compact, and a continuous real function on a nonempty compact space attains its minimum. [[math:thm-compactness-under-continuous-maps]] Finite unions of compact subsets and closed subsets of compact spaces are compact. [[math:thm-closed-subspace-of-a-compact-space-is-compact]] Compact subsets of a Hausdorff space are closed. [[math:thm-compact-subset-of-a-hausdorff-space-is-closed]] The sphere $S^2$ is path connected; path-connected spaces are connected, and a nonempty clopen subset of a connected space is the whole space. [[math:cor-euclidean-spheres-are-path-connected]] [[math:thm-path-connected-implies-connected]] [[math:thm-connectedness-characterisations]] Metric and topological compactness agree, and ambient open covers may be restricted to the compact subspace before choosing a finite subcover. [[math:thm-compactness-agrees-with-metric-compactness]] [[math:lem-compactness-of-a-subspace-is-ambient]] [[math:def-compact-space]]

[F9] A smooth cutoff $\eta\in C_c^\infty(\mathbb R)$ exists with $0\le\eta\le1$, $\eta=1$ on $|z|\le1$ and $\eta=0$ on $|z|\ge2$. The coordinate chain rule in [F6] and the fundamental theorem of calculus on finite intervals give integration of a smooth scalar along each smooth path piece. We apply the resulting bounds to smooth functions and finite piecewise smooth paths in the section. [[math:lem-schwartz-cutoffs-from-the-standard-smooth-step]] [[math:lem-fundamental-theorem-and-integration-by-parts]]

[F10] Use the complete smooth Hawking field of the common collar for the actual original reference section $B_0$, with jointly smooth boundary-distance coordinates $c_q(\rho,y)$ and the Gaussian maps of [F5]. For each retained pair apply [[pthm-hawking-graph-height]] with its lower parameter bound $\delta_0\in(0,1)$, $q=q_j$, and original reference section $\Sigma_1=B_0$, using the same stationary product, mass-one normalization and complete collar field. Individual admissibility supplies the connected smooth spacelike maximal candidate with boundary $S$, smooth boundary extension and global stationary interior graph. Its normalized end decay gives $D\widetilde u_j\to0$; the compact-core exterior condition required by that fixed-parameter result is proved locally for each such pair in steps 1.1–5.1 below, using individual end decay, the background metric bounds in [F4], original compact truncations in [F7] and the ordinary boundary collar in [F14]. This verification uses no candidate Hawking height, uniform candidate collar estimate or limiting section. Consequently, for every $x\in V\setminus S$ there is exactly one real $v_j(x)$ with $\phi^K_{v_j(x)}x\in\Sigma_j$, and this height is individually smooth up to $S$. The indexed height supplier [[pthm-author-048251387164-indexed-height-and-horizon-estimates]] gives one common bound $|v_j|\le C$ on a common closed source collar $0\le\rho\le a$ inside $V$. Then $\Phi_j(x)=\phi^K_{v_j(x)}x$ is the smooth spacelike flow-graph embedding there. The Gaussian-flow input gives $c_1\rho\le R\le c_2\rho$ and $|\tau|\le\theta R$ with $c_1,c_2>0$ and $\theta<1$ common to all supplied pairs. For $0<b<c_1a/2$, the proper-projection and one-sheet inputs identify its part over $0<R<b$ as one smooth normal graph. They apply separately to each supplied pair with the same constants, including repeated parameters; no candidate at an unrepresented parameter is required. [[pthm-common-reference-collar]] [[lem-author-840894718169-uniform-gaussian-flow-cone]] [[lem-author-840894718169-fixed-target-collar-properness]] [[lem-author-840894718169-boundary-one-sheet-normal-graph]]

[F11] Use only the candidate-independent original-background conclusion of the boundary-angle result: there is a fixed original normal tube $\Xi(y,u,v)$ with $K=\kappa(v\partial_u+u\partial_v)$ and a smooth bounded original reference graph $x(r,y)=\Xi(y,r\sinh A(r,y),r\cosh A(r,y))$, where $A$ is rapidity and $\kappa>0$. This input does not assume candidate sections or their height bounds. The original event-boundary quadrant input identifies the original exterior in its reference normal frame; the future/outward boost to the invariant frame preserves the exterior wedge $v>|u|$. Local uniqueness of integral curves identifies finite boost segments in this tube with the complete collar flow. [[pthm-boundary-normal-angle]] [[lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant]] [[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]]

[F12] Every bounded real sequence has a convergent subsequence. For the compact surface coordinates use a fixed smooth identification $S\cong S^2\subset\mathbb R^3$, and apply this successively to its three bounded coordinates and to bounded real flow time and source radius. Closed interval inequalities and the sphere equation are preserved on taking limits. [[math:thm-bolzano-weierstrass]]

[F13] Continuous real functions on closed finite intervals are Riemann integrable. For two integrable functions the absolute difference of their integrals is bounded by the interval length times a uniform bound for their difference. The fundamental theorem applies to each smooth candidate derivative along a coordinate segment in its open chart. We use these facts to identify the componentwise compactness limits as successive derivatives; on boundary half-boxes first work in the interior and pass to the boundary by continuity. [[math:thm-continuous-implies-integrable]] [[math:lem-uniform-integral-error-bound]] [[math:lem-fundamental-theorem-and-integration-by-parts]]

[F14] Under Countable Choice, every smooth manifold with boundary has a smooth collar. Apply this to each already supplied smooth section separately; ZFC in [F3] supplies Countable Choice. Since its boundary $S$ is compact, restricting the collar to a smaller closed parameter interval gives a compact embedded collar with compact outer face by [F8]. This is an ordinary collar of that individual manifold, with no uniform width, normal-graph representation or Hawking-height input. [[math:thm-collar-neighborhood-theorem]]

## Proof

**Given:** The fixed background in the Statement, including $H_g|_C=0$, and an arbitrary convergent parameter sequence with individually admissible slices. **Goal:** Construct the admissible complete limit.

1.1 First verify the compact-core condition for the supplied sections without using any indexed candidate estimate or Hawking height. Individual admissibility gives $0<q_j\le1$. Since $q_j\to q_*\ge\delta>\delta_0=\delta/2>0$, discard a finite prefix so that all retained $q_j\in[\delta_0,1]$. Fix one retained pair $(q,\Sigma)$, let $G:C\to\Sigma^\circ$ be its stationary graph diffeomorphism, and put $s(G(z))=|y(z)|$ using only the adapted topological coordinates of [F7]. On the separate physical end write $r=r_{\mathrm{phys}}$ and $v=\widetilde u$. In $x_q$ coordinates the induced metric has components $h_{ij}=(g_q)_{ij}+(g_q)_{0i}v_j+(g_q)_{0j}v_i+(g_q)_{00}v_iv_j$. The individual slope decay from admissibility and the background bounds in [F4] give $h_{ij}=\delta_{ij}+O_q(r_q^{-1})$. Hence on some physical graph tail $h\ge\tfrac12\sum_i(dx_q^i)^2$, and $|dr(\xi)|\le L_q\sqrt{h(\xi,\xi)}$ there, with $L_q=\sqrt2/q$. Neither its threshold radius nor this argument uses a candidate lapse bound, a uniform collar or completeness. [A1, F2, F4, F7, given, algebra]

2.1 For every sufficiently large physical radius $a$, the graph tail $H_a=G(\{r\ge a\})$ is closed in $\Sigma$. Its inner sphere and its finite annuli $G(\{a\le r\le b\})$ are compact and closed by [F8], since their base annuli are compact subsets of $C$ and $G$ is smooth there. Suppose $z\in\overline{H_a}^{\Sigma}\setminus H_a$. Choose a relatively compact convex coordinate ball or boundary half-ball about $z$, disjoint from the compact inner sphere, and a point $w\in H_a$ in that chart. The coordinate straight segment $\lambda:[0,1]\to\Sigma$ from $w$ to $z$ stays in the chart and has $h$-speed bounded by some finite $M$. Initially it is in the open tail $G(\{r>a\})$. Until its first exit, the chain rule and integration along every closed initial subsegment, as in [F6] and [F9], give $|r(\lambda(t))-r(w)|\le L_qMt$. Thus all those points lie in the finite graph annulus $G(\{a\le r\le r(w)+L_qM+1\})$. That compact annulus is closed in $\Sigma$, so the first-exit point, including a possible exit at $t=1$, lies in it. The chart misses its inner sphere, so this point still belongs to the open tail, contradicting first exit. Hence $H_a$ is closed, including against accumulation at $S$. [F2, F6, F8, F9, step 1.1]

3.1 Take an ordinary closed boundary collar $W_0=c(S\times[0,a_0])$ in the supplied section using [F14] and [F8]. For all sufficiently large integers $n$, the closed tails $H_n$ of step 2.1 are nested. Their open complements cover $W_0$: boundary points lie in none of the tails, while each interior point is either outside the physical tail chart or has a finite radius. Compactness of $W_0$ gives one $n$ with $W_0\cap H_n=\varnothing$. Consequently $G^{-1}(W_0\setminus S)$ lies in the compact original physical truncation $B_{0,n}$ supplied by [F7]. The continuous topological radius $|y|$ is bounded on that truncation, so $s\le B$ on $W_0\setminus S$ for some finite $B$. The compact nonempty outer face $L_0=c(S\times\{a_0\})$ is in $\Sigma^\circ$, and its continuous function $s>1$ has a minimum $m>1$. No extension of $G^{-1}$ to $S$ has been used. [F7, F8, F14, step 2.1, choose]

4.1 Choose $0<\epsilon_0<m-1$ and put $J_0=G(y^{-1}(\{1<|y|<1+\epsilon_0\}))$. Radial segments and paths in $S^2$ make $J_0$ connected by [F8]. In the interior manifold the boundary of $W_0^\circ=c(S\times(0,a_0))$ is exactly $L_0$, since the compact collar is closed and its other face lies on $S$. The set $J_0$ misses $L_0$, so $J_0\cap W_0^\circ$ is clopen in $J_0$. It is nonempty: fix $p\in S$ and consider $c(p,a_0/k)\to p$ for integers $k\ge2$. These points have $s\le B$ by step 3.1. If none had $s<1+\epsilon_0$, all would belong to the compact interior graph image $G(y^{-1}(\{1+\epsilon_0\le|y|\le B\}))$, closed in the Hausdorff manifold $\Sigma$ by [F8]. Its boundary limit $p$ cannot lie in that interior image. Thus [F8] gives $J_0\subset W_0^\circ$. This identifies the small topological shell with part of the individual collar without identifying physical and topological radii. [F7, F8, step 3.1, choose]

5.1 For any sufficiently large physical radius $R$, put $K_R=B_0\setminus\{r>R\}$, compact by [F7]. The set $K_R\cap\{|y|\ge1+\epsilon_0\}$ is a compact subset of $C$, so its graph image is compact by [F8]. Step 4.1 places the rest of $G(K_R\cap C)$ in $W_0$. Therefore $\Sigma\setminus G(\{r>R\})=S\cup G(K_R\cap C)$ is contained in the compact union $W_0\cup G(K_R\cap\{|y|\ge1+\epsilon_0\})$. It is closed in $\Sigma$ because the removed physical graph tail is open in the interior graph, which is open in $\Sigma$. It is consequently compact by [F8]; the same argument applies at $2R$. With $R_q=qR$, the normalized end chart identifies the complementary open tail with $\{|x_q|>R_q\}$, and the complement of $\{r_q>2R_q\}$ is also compact. Together with the individual uniform slope limit and the supplied smooth spacelike maximal boundary section, this is precisely the compact-core exterior condition required for [F10]. The argument applies independently to every retained pair before using [F1] or [F10]. For any other individually admissible section at fixed $q>0$, the same argument uses the background interval $[q/2,1]$ and its own end constants. [F2, F7, F8, step 1.1, step 3.1, step 4.1]

6.1 The retained tail lies in $[\delta_0,1]$ by step 1.1, and step 5.1 has independently verified its compact-core exterior condition. Apply all three suppliers in [F1] on this fixed smaller positive interval and the same actual-exterior-maximal background [A1]. Apply [F3] to the resulting uniform finite-order compact stationary estimates, and diagonalize over a countable compact exhaustion and derivative orders. To identify these componentwise limits, write $f_\alpha$ for the uniform limit of $D^\alpha u_j$ on a smaller coordinate box. For every coordinate segment remaining in that box, [F13] gives $D^\alpha u_j(x+t e_\ell)-D^\alpha u_j(x)=\int_0^t D^{\alpha+e_\ell}u_j(x+s e_\ell)\,ds$. The integrability and uniform integral-error bound in [F13] permit passage to $f_\alpha(x+t e_\ell)-f_\alpha(x)=\int_0^t f_{\alpha+e_\ell}(x+s e_\ell)\,ds$. After division by nonzero $t$, continuity of $f_{\alpha+e_\ell}$ makes the right-hand average tend to $f_{\alpha+e_\ell}(x)$ as $t\to0$, identifying the corresponding partial derivative. Induction over derivative order therefore identifies all the extracted limits with derivatives of $u_*=f_0$. Using the diagonal extraction at every finite order, obtain one locally smooth stationary height $u_*$ on the entire reference interior. In original stationary coordinates put $F_j=t-u_j$. Then $N_j=1/\sqrt{D_j}$ with $D_j=-g_j^{-1}(dF_j,dF_j)$. The common upper bound $N_j\le C_{\delta_0}$ in [F1] gives $D_j\ge C_{\delta_0}^{-2}>0$. Pass to the limit to preserve strict spacelikeness. Mean curvature is continuous in the metric one-jet and graph two-jet, so the smooth limit is maximal. The lower lapse bound in [F1] serves coordinate transversality; it is not used with the wrong reciprocal direction to prove D positive. [A1, F1, F2, F3, F13, step 1.1, step 5.1, given, algebra]

6.2 First establish a background neighborhood captured by the complete $K$ saturation of the source collar in [F10]. In the tube of [F11], choose $r_*>0$ so that $x(r,y)$ lies in $0\le\rho_q<a$ for every $q\in[\delta_0,1]$ and $0\le r\le r_*$; smoothness of the common reference distances and compactness of the parameter interval and $S$ allow this choice. Let $A_0$ bound $|A(r,y)|$. Choose a closed normal box $|u|,|v|\le d$ inside the tube and its original exterior-quadrant neighborhood, and $0<\varepsilon<\min(r_*,d)$ with $\varepsilon\cosh A_0<d$. For any exterior point $p=\Xi(y,u,v)$ with $0<v<\varepsilon$, put $r=\sqrt{v^2-u^2}$ and $a_p=\operatorname{arctanh}(u/v)$. Vary rapidity at fixed $(r,y)$ from $A(r,y)$ to $a_p$. Along this finite segment, $v=r\cosh a\le\max(r\cosh A(r,y),v(p))<d$ and $|u|<v$, so the segment stays in the tube and the exterior. Its tangent is the local $K$ direction with elapsed flow time $(a_p-A(r,y))/\kappa$. Uniqueness in [F11] identifies it with the complete collar orbit, giving $p=\phi_s^K x(r,y)$. Thus an ambient neighborhood $U$ of $S$ has its whole exterior part in that saturation. Shrink $U$ inside the common Gaussian domains with all target radii less than $b$, uniformly in $q$. For any $p\in\Sigma_j^\circ\cap U$, the representation just constructed has $x(r,y)\in V\setminus S$. The compact-core verification in step 5.1 makes the fixed-$q_j$ intersection result in [F10] applicable; its uniqueness gives $s=v_j(x(r,y))$, so its indexed height bound yields $|s|\le C$ and $p=\Phi_j(x(r,y))$. Thus $p$ belongs to the one-sheet normal graph in [F10]; the points of $S$ already lie on its zero-boundary graph. This argument allows arbitrarily large finite $|s|$ for general exterior points and assumes no candidate at a missing parameter. [A1, F1, F5, F7, F8, F10, F11, step 5.1, algebra]

7.1 On the common horizon collar, [F1] gives uniformly spacelike normal graphs with zero heights on $S$ and uniform finite-order bounds. Use the joint background maps in [F5] and [F10] to express them on a fixed smaller target domain $[0,b)\times S$, and extract a further diagonal subsequence on closed collar charts, retaining the interior subsequence. Apply the derivative-identification argument in step 6.1 using [F13] to these scalar heights on boundary half-boxes: the segment identities hold in their interiors and extend to the closed faces by continuity. Write the resulting smooth convergence as $w_j\to w_*$ and set $G_j(R,y)=\Psi_{q_j}(w_j(R,y),c_{q_j}(R,y))$ and $G_*(R,y)=\Psi_{q_*}(w_*(R,y),c_{q_*}(R,y))$. Joint smoothness gives $G_j\to G_*$ smoothly on every smaller closed target collar. Zero boundary values give $G_*(0,y)=y$, and the uniform spacelike tangent bounds in [F1] make $G_*$ an embedded smooth spacelike normal graph. This constructs a normal limit; identification with the stationary limit is proved next. [F1, F2, F3, F5, F10, F13, step 6.1]

8.1 Fix $0<R<b$ and $y\in S$. By [F10], $G_j(R,y)=\phi^K_{s_j}(c_{q_j}(\rho_j,\eta_j))$ with $|s_j|\le C$ and $R/c_2\le\rho_j\le R/c_1<a/2$. Apply [F12] to these two real parameters and the three coordinates of $\eta_j\in S^2$ to obtain a further subsequence for this fixed point, with limits $s_\infty,\rho_\infty,\eta_\infty$. The inequalities give $\rho_\infty>0$, and the sphere equation gives $\eta_\infty\in S$. Smoothness of the reference collars and the complete flow gives $G_*(R,y)=\phi^K_{s_\infty}(c_{q_*}(\rho_\infty,\eta_\infty))\in\mathcal E$. Thus its candidate approximants converge to an exterior point and their stationary projections eventually lie in one compact interior coordinate neighborhood. Write their stationary coordinates as $(t_j,x_j)\to(t_*,x_*)$. Since $t_j=u_j(x_j)$, local uniform convergence in step 6.1 and continuity give $t_*=u_*(x_*)$. Hence every punctured normal-limit point belongs to the stationary limit. The positive source-radius bound and bounded flow times prevent its projections from escaping to the horizon. [F1, F2, F5, F7, F10, F12, step 6.1, step 7.1]

9.1 Conversely, take a smaller common ambient neighborhood of $S$ inside $U$ from step 6.2, with target radii less than some $b'<b$. Let $P=(u_*(x),x)$ be a stationary-limit point there. Its approximants $P_j=(u_j(x),x)$ converge to $P$ by step 6.1 and are eventually captured by step 6.2, so $P_j=G_j(R_j,y_j)$. Joint smoothness of the Gaussian inverses gives $(\tau_j,R_j,y_j)\to(\tau_*,R_*,y_*)$ with $0\le R_*<b$ and $\tau_j=w_j(R_j,y_j)$. The cone estimate in [F10] passes to $|\tau_*|\le\theta R_*$. If $R_*=0$, then $\tau_*=0$ and $P=y_*\in S$, contrary to $P\in\mathcal E$. Therefore $R_*>0$. Smooth convergence of the normal heights on smaller closed collars gives $\tau_*=w_*(R_*,y_*)$, and hence $P=G_*(R_*,y_*)$. Together with step 8.1 this proves both inclusions on an ambient overlap. The normal embedding in step 7.1 therefore attaches the stationary graph smoothly and spacelike to boundary exactly $S$, excluding additional near-boundary sheets. [F1, F2, F5, F7, F10, step 6.1, step 7.1, step 6.2, step 8.1]

10.1 The positive-q normalized coordinate scalings depend smoothly on q and have common inverses on the fixed positive interval $[\delta_0,1]$ containing the retained tail and its limit. Put $c_q=d_q/(4q)$ and $y=x_q$. The normalization in [F2] is $\widetilde u_q(y)=c_qu_q(y/q)$. Since the spatial scaling is affine and $c_q$ is constant in y, repeated application of [F6] gives $D_y^\beta\widetilde u_q(y)=c_q q^{-|\beta|}(D_x^\beta u_q)(y/q)$ for $|\beta|\le4$. At each fixed normalized end point y, the original points $y/q_j$ converge to $y/q_*$ and lie in a fixed compact interior neighborhood for large j. Local smooth convergence from step 6.1 and continuity of $c_q$ therefore give convergence of every derivative in this formula through order four. Pass the uniform end derivative estimates of [F1] to this limit to obtain $|D^j\widetilde u_*|\le C_{\delta_0,j}r_{q_*}^{-3/4-j}$ for $j\le4$, including its zero height and slope limits. Thus the section is individually admissible at q*. [F1, F2, F6, step 6.1, step 9.1, algebra]

11.1 Work in the normalized end coordinates at $q_*$. Write $r=r_{q_*}$, $G_{\mu\nu}=(g_{q_*})_{\mu\nu}$ and $v=\widetilde u_*$. The graph tangent vectors are $\partial_i+v_i\partial_0$, so its induced components are $h_{ij}=G_{ij}+G_{0i}v_j+G_{0j}v_i+G_{00}v_iv_j$. By [F4] and step 10.1, $G_{ij}=\delta_{ij}+O(r^{-1})$, $G_{0i}=O(r^{-2})$, $G_{00}=-1+O(r^{-1})$ and $|Dv|\le C r^{-7/4}$. Hence $h_{ij}=\delta_{ij}+O(r^{-1})$, with constants controlled by the common bounds. Increasing the common radius $R$ gives $\tfrac12|\xi|^2\le h_{ij}\xi^i\xi^j\le2|\xi|^2$ for every end tangent vector $\xi$. In particular an end curve has induced length at least its Euclidean radial variation divided by $\sqrt2$. [F1, F2, F4, step 10.1, algebra]

12.1 Construct a physical exhaustion on the original section, rather than estimating derivatives of its unrelated topological radius. Choose $a>0$ so large that the physical chart, compact truncations of [F7] and end comparison of step 11.1 hold for $r_{\mathrm{phys}}\ge a$. With the cutoff in [F9], put $F_0=a+(1-\eta(r_{\mathrm{phys}}/a))(r_{\mathrm{phys}}-a)$ on the physical tail and $F_0=a$ off that tail. The cutoff is identically one for $r_{\mathrm{phys}}\le a$ and flat at the join, so these formulas give one smooth nonnegative function on $B_0$, constant near $S$ and equal to $r_{\mathrm{phys}}$ for $r_{\mathrm{phys}}\ge2a$. Its closed sublevels are compact by the physical-truncation assertion in [F7]. On $\Sigma_*^\circ$ define $H=F_0\circ G^{-1}$. Step 11.1 bounds $|dH|_h=|dr_{\mathrm{phys}}|_h$ in the far tail. On the graph image of the interpolation annulus its norm is bounded by smoothness and compactness; it vanishes over the remaining core. Thus $|dH|_h\le L$ throughout the interior for some finite $L$. Integrating along each smooth path piece using [F6] and [F9] gives $|H(p)-H(p')|\le L\operatorname{length}_h(\gamma)$ for every interior piecewise smooth path from $p$ to $p'$. [F2, F6, F7, F8, F9, step 11.1, construct]

13.1 Step 9.1 supplies a closed smaller smooth attached collar $W=c(S\times[0,b])$, with compact outer face $L_b=c(S\times\{b\})$. These sets are compact by [F8]. The function $H$ has a finite maximum on $L_b$. Smoothness of the positive metric on the closed collar bounds the lengths of all coordinate segments $c(y,[t,b])$ uniformly for $0<t\le b$. Applying step 12.1 on those interior segments bounds $H$ on $W\setminus S$. Therefore $G^{-1}(W\setminus S)$ lies in one fixed compact sublevel of $F_0$ in $B_0$. The continuous topological radius $s$ is bounded on that sublevel by [F8], so $s\circ G^{-1}\le A$ on $W\setminus S$. This uses no bound for $|ds|_h$ and no boundary extension of $G^{-1}$. [F2, F7, F8, step 9.1, step 12.1]

14.1 On the nonempty compact face $L_b$, the continuous function $s\circ G^{-1}>1$ has a minimum $m>1$. Choose $0<\epsilon<m-1$ and put $J=G(\{1<s<1+\epsilon\})$. This is connected by radial paths and paths in the topological $S^2$, using [F8]. In the interior manifold the boundary of $W^\circ=c(S\times(0,b))$ is exactly $L_b$, so $J\cap W^\circ$ is clopen in $J$. It is nonempty: for fixed $y\in S$, the collar points $c(y,b/n)$ tend to $y$ and have $s\circ G^{-1}\le A$ by step 13.1. If all stayed above $1+\epsilon$, they would lie in the compact interior image $G(\{1+\epsilon\le s\le A\})$, which is closed in the Hausdorff manifold $\Sigma_*$ and cannot contain their boundary limit. Hence [F8] gives $J\subset W^\circ$. This captures the small topological shell in the attached collar without identifying it with a physical radial shell. [F7, F8, step 13.1, choose]

15.1 For every sufficiently large physical radius $R$ for which [F7] supplies $B_{0,R}$, put $B_{\Sigma,R}=S\cup G(B_{0,R}\setminus S)=\Sigma_*\setminus G(\{r_{\mathrm{phys}}>R\})$. Its complement is open, so it is closed in $\Sigma_*$. By step 14.1, its part with $1<s<1+\epsilon$ lies in the compact collar $W$. Its remaining part lies in $G(B_{0,R}\cap\{s\ge1+\epsilon\})$, a compact interior image by [F8]. Thus $B_{\Sigma,R}$ is compact. For sufficiently large $R'$, step 13.1 places all of $W$ in $B_{\Sigma,R'}$, since $H=r_{\mathrm{phys}}$ on the far tail and $H$ is bounded on $W\setminus S$. This gives a neighborhood of $S$ in $B_{\Sigma,R'}$. For any smaller admissible $R$, remove from that neighborhood the compact interior image of the physical annulus $R\le r_{\mathrm{phys}}\le R'$; what remains is a neighborhood of $S$ contained in $B_{\Sigma,R}$. Therefore each physical core contains a neighborhood of $S$ and has no boundary there relative to $\Sigma_*$. Away from $S$ the smooth graph diffeomorphism gives its only boundary $G(\{r_{\mathrm{phys}}=R\})$ and its smooth compact-region structure. The boundary of that region as a manifold is $S\sqcup G(\{r_{\mathrm{phys}}=R\})$. A positive boundary-distance trim is a closed subset of this compact core avoiding $S$, hence compact in $\Sigma_*^\circ$: the distance is continuous by the triangle inequality and local upper metric bounds in coordinate balls and boundary half-balls, and it vanishes on $S$ by definition. [F2, F7, F8, step 13.1, step 14.1]

16.1 Choose $R'$ larger than $2a$ and the bound for $H$ on the collar in step 13.1. The function $P=\max\{R',H\}$ on the interior then extends as the constant $R'$ to a neighborhood of $S$. It is continuous on the whole section, equals $\max\{R',r_{\mathrm{phys}}\}$ where it varies, and has compact sublevels by step 15.1. To prove the change bound along a piecewise smooth curve, orient it so that its terminal $P$ value is at least its initial value. If $P>R'$ on the entire curve, integrate the radial bound from step 11.1 using [F9]. Otherwise take the last parameter where $P=R'$, which exists by continuity and compactness in [F8]. On the final portion $P=r_{\mathrm{phys}}>R'$, and the radial bound gives the terminal value minus $R'$ at most $\sqrt2/q_*$ times that portion's length, by integration and a limit from its open initial endpoint. Since the initial value is at least $R'$, this also bounds the net increase. The case of equal endpoint values is immediate. This argument does not differentiate the maximum at a crossing, and also permits parts of the curve through $S$, where $P$ is locally constant. Taking the infimum over curves gives $|P(p)-P(p')|\le(\sqrt2/q_*)d_h(p,p')$. Consequently every intrinsic Cauchy sequence has bounded $P$ and lies in one compact physical core. [F2, F8, F9, step 11.1, step 12.1, step 13.1, step 15.1, algebra]

17.1 In smaller coordinate balls or boundary half-balls, the smooth positive induced metric has a finite upper bound. Joining nearby points by coordinate line segments inside these convex coordinate sets shows that coordinate convergence implies intrinsic-distance convergence, including at $S$. The triangle inequality then also makes boundary distance continuous in these coordinates. Its zero set is exactly $S$: a point outside the compact closed $S$ has a smaller coordinate ball disjoint from $S$, on which positive lower metric bounds force every path to $S$ to have a positive length before leaving the ball. For any sequence in a compact physical core, compactness gives a point each of whose neighborhoods contains infinitely many sequence terms; otherwise neighborhoods with only finitely many terms would have a finite subcover. Choose increasing indices in shrinking coordinate neighborhoods to obtain an intrinsically convergent subsequence. The Cauchy property from step 16.1 and the triangle inequality give convergence of the entire sequence. This is completeness with the included boundary under [F2]. [F2, F8, step 9.1, step 15.1, step 16.1, choose]

18.1 The physical-core and metric argument above also applies to any individually admissible section at a fixed $q>0$: its smooth included boundary and global interior graph are part of admissibility, its end derivative decay and the same positive-parameter background bounds give the induced end comparison in step 11.1, and a constant sequence of that pair has the same smooth collar and interior graph as its limits in steps 6.1–9.1. Choose a lower positive parameter bound smaller than $q$ when invoking [F1]. No other section or missing-parameter family is required. Hence each individually admissible section is complete and has these compact physical cores and trims, in addition to the subsequential limiting conclusions already established. [F1, F2, F4, F7, step 6.1, step 9.1, step 11.1, step 15.1, step 17.1] ∎

## Source notes

Radu’s Section 5.3, Lemma 5.1 gives compact-graph convergence under its own boundary, topology, lapse and height hypotheses. This is background for the present adaptation; the indexed noncompact conclusion is established only by the local argument and declared suppliers.

The actual-exterior maximality premise above specifies this generated conditional result. It is not inferred from maximality of an independently supplied section or from agreement of independent charts, and it is not attributed as a correction to the original article. The immutable original extraction, including Theorem 1.1 and its unresolved source-assessment status, is unchanged.

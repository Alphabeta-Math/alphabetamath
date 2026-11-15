---
id: pthm-author-048251387164-indexed-admissible-end-estimates
title: Uniform end estimates indexed only by existing admissible slices
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - def-stationary-maximal-graph
  - def-spacelike-maximal-hypersurface-data
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - math:def-axiom-of-choice
  - pthm-positive-transformed-lapse
  - pthm-transformed-end-geometries
  - lem-annular-quasilinear-bootstrap-input
  - lem-author-db87cb8e0bab-linear-fourth-derivative-estimate
  - math:thm-euclidean-semicontinuous-extreme-value-theorem
  - math:lem-negative-semidefinite-hessian-at-an-interior-local-maximum
  - math:lem-qa-30-positive-product-trace-nonnegative
  - pthm-original-lapse-and-product
  - math:thm-collar-neighborhood-theorem
  - math:thm-heine-borel-rn
  - math:thm-finite-products-of-compact-spaces
  - math:thm-compactness-under-continuous-maps
  - math:thm-closed-subspace-of-a-compact-space-is-compact
  - math:thm-compact-subset-of-a-hausdorff-space-is-closed
  - math:cor-euclidean-spheres-are-path-connected
  - math:thm-path-connected-implies-connected
  - math:thm-connectedness-characterisations
  - math:cor-mean-value-theorem
  - math:thm-chain-rule-for-total-derivatives
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  pthm-positive-transformed-lapse: physical-result
  pthm-transformed-end-geometries: physical-result
  lem-annular-quasilinear-bootstrap-input: mathematical-premise
  lem-author-db87cb8e0bab-linear-fourth-derivative-estimate: mathematical-premise
  math:thm-euclidean-semicontinuous-extreme-value-theorem: mathematical-premise
  math:lem-negative-semidefinite-hessian-at-an-interior-local-maximum: mathematical-premise
  math:lem-qa-30-positive-product-trace-nonnegative: mathematical-premise
  pthm-original-lapse-and-product: physical-result
  math:thm-collar-neighborhood-theorem: mathematical-premise
  math:thm-heine-borel-rn: mathematical-premise
  math:thm-finite-products-of-compact-spaces: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:thm-closed-subspace-of-a-compact-space-is-compact: mathematical-premise
  math:thm-compact-subset-of-a-hausdorff-space-is-closed: mathematical-premise
  math:cor-euclidean-spheres-are-path-connected: mathematical-premise
  math:thm-path-connected-implies-connected: mathematical-premise
  math:thm-connectedness-characterisations: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
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
      reading_limits: Consulted the cited HTML passages in this adjudication. They
        provide the background and motivation for this adapted statement; they
        do not assert this item's indexed noncompact strengthening. The numbered
        local argument uses only the declared suppliers; no independent proof
        audit of the source is claimed.
physical_scope: Conditional mathematical estimates and continuation for the
  regular stationary vacuum/Harrison construction. Existence is never presumed
  at an unavailable parameter. No empirical claim or q=0 conclusion.
dependency_level: 12
---

## Statement

Fix the regular mass-one stationary vacuum/Harrison construction with maximal original exterior section and $T|_S\not\equiv0$. Call a section individually admissible at $q>0$ if it is connected, smooth and spacelike maximal with boundary $S$, is smooth up to $S$, its interior is a global stationary graph, and its normalized height has $|D^j\widetilde u|\le C_qr_q^{-3/4-j}$ for $0\le j\le4$ on some end depending on that section. Fix $0<\delta\le1$. Let $\mathcal I$ be any set of pairs $(q,\Sigma)$ of such sections with $q\in[\delta,1]$. No pair is assumed to exist at parameters outside the projection of $\mathcal I$. The lapse is positive and has a common upper bound; there is a common end on which $|D\widetilde u|\le C_\delta r_q^{-1/2}$. For each $0<\mu<1$ the heights obey a common $C_{\delta,\mu}r_q^{-\mu}$ bound. In particular the differentiated estimates $|D^j\widetilde u|\le C_{\delta,j}r_q^{-3/4-j}$, $0\le j\le4$, and their fixed-annulus scaled C4-Holder versions hold uniformly over $\mathcal I$. These uniform estimates are conclusions, not assumptions on the initially individual admissibility constants.

The original-section maximality used here is assumed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$, with the original metric $g$, so $H_g|_C=0$. The selected physical end retains its stated mass-one normalization. Maximality of an independently labelled chart-side section or another supplied maximal section does not replace this premise. No equality between the hypersurface identification and the physical stationary end chart is assumed. [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

## Facts & Assumptions

[A1] The model, regular data, graph, normalization and induced geometry have their stated meanings. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-harrison-normalization]] [[def-stationary-maximal-graph]] [[def-spacelike-maximal-hypersurface-data]] Norms are [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]; work in ZFC. [[math:def-axiom-of-choice]]

[F1] The positive-lapse theorem is a fixed-q statement and requires the compact-core exterior condition, which is established below for each individually admissible section. [[pthm-positive-transformed-lapse]] Normalized end metric bounds are properties of the background metrics on the whole fixed positive parameter interval. [[pthm-transformed-end-geometries]]

[F2] The structural annular quasilinear estimate and its fixed-annulus C4-Holder linear conclusion are mathematical estimates for an indexed family whenever their uniform coefficient hypotheses hold. They require no existence at a missing parameter. [[lem-annular-quasilinear-bootstrap-input]] [[lem-author-db87cb8e0bab-linear-fourth-derivative-estimate]]

[F3] A continuous real function on a nonempty compact Euclidean set attains a maximum. At an interior maximum of a $C^2$ function its gradient vanishes and its Hessian is negative semidefinite. For positive semidefinite matrices $P,Q$, $\operatorname{tr}(PQ)\ge0$. These elementary inputs will prove the strict barrier comparison locally, with the first-order term vanishing at the maximum. [[math:thm-euclidean-semicontinuous-extreme-value-theorem]] [[math:lem-negative-semidefinite-hessian-at-an-interior-local-maximum]] [[math:lem-qa-30-positive-product-trace-nonnegative]]

[F4] Under the regular vacuum and actual-original-exterior maximality hypotheses, the original lapse/product result supplies the stationary product over $C=\Sigma_0\cap E$, its smooth closure $B_0=C\cup S$, an adapted topological identification $y:B_0\to\{|y|\ge1\}$, and compact physical-end truncations $B_0\setminus\{r>R\}$ for every sufficiently large $R$. The physical radius $r=|x|$ is defined in its own end chart and is not identified with $|y|$. [[pthm-original-lapse-and-product]] A smooth manifold with boundary admits a smooth collar in ZFC. [[math:thm-collar-neighborhood-theorem]]

[F5] Closed bounded Euclidean annuli and finite closed intervals are compact. Finite products of compact spaces and finite unions of compact subsets are compact. Continuous images of compact sets are compact, and continuous real functions on nonempty compact sets attain their extrema. Compact subsets of Hausdorff spaces are closed, and closed subsets of compact spaces are compact. [[math:thm-heine-borel-rn]] [[math:thm-finite-products-of-compact-spaces]] [[math:thm-compactness-under-continuous-maps]] [[math:thm-compact-subset-of-a-hausdorff-space-is-closed]] [[math:thm-closed-subspace-of-a-compact-space-is-compact]]

[F6] The sphere $S^2$ is path connected. A path-connected space is connected; in a connected space a nonempty clopen subset is the whole space. [[math:cor-euclidean-spheres-are-path-connected]] [[math:thm-path-connected-implies-connected]] [[math:thm-connectedness-characterisations]]

[F7] If a real function is continuous on $[a,b]$ and differentiable on $(a,b)$, with $a<b$, the mean value theorem gives $h(b)-h(a)=h^{\prime}(c)(b-a)$ for some $c\in(a,b)$. The total-derivative chain rule computes derivatives of compositions of differentiable Euclidean maps. [[math:cor-mean-value-theorem]] [[math:thm-chain-rule-for-total-derivatives]]

## Proof

**Given:**Any set of individually admissible pairs on the fixed positive parameter interval. **Goal:** Derive common end estimates without assuming a section at every parameter.

1.1 Fix one pair $(q,\Sigma)$ and let $G:C\to\Sigma^\circ$ be its stationary graph diffeomorphism. Choose the adapted $y$ coordinates from F4, and put $s(G(z))=|y(z)|$. Keep $r=|x|$ for the separate physical end radius, so $r_q=qr$ there. On that end, with $v=\widetilde u$, the induced metric is $h_{ij}=(g_q)_{ij}+(g_q)_{0i}v_j+(g_q)_{0j}v_i+(g_q)_{00}v_iv_j$ in $x_q$ coordinates. Individual slope decay and F1 give $h_{ij}=\delta_{ij}+O_q(r_q^{-1})$. Hence $|dr|_h=q^{-1}|dr_q|_h$ is bounded by a finite constant $L_q$ on a sufficiently distant physical graph tail, before any lapse bound is used. This says nothing about $|ds|_h$. [A1, F1, F4, given, algebra]

2.1 For each sufficiently large physical radius $a$, the set $H_a=G(\{r\ge a\})$ is closed in $\Sigma$. Indeed its inner sphere and each finite annulus $G(\{a\le r\le b\})$ are compact and closed by F5. If $z\in\overline{H_a}^{\Sigma}\setminus H_a$, take a small relatively compact section coordinate ball or boundary half-ball $V$ about $z$, disjoint from the inner sphere. Choose $w\in H_a\cap V$ and the coordinate straight segment $\lambda:[0,1]\to V$ from $w$ to $z$. Its $h$-speed is bounded by a finite $M$ on the closed interval, by smoothness and F5. While the segment stays in the open graph tail, F7 and step 1.1 give $|(r\circ\lambda)'|\le L_qM$. The mean value theorem bounds its radius by $r(w)+L_qM$. At its first exit, including an exit at parameter one, compactness and closedness of the finite graph annulus put the exit point back in that annulus; it misses the inner sphere and thus still lies in the open tail, a contradiction. [F4, F5, F7, step 1.1, contradiction]

3.1 Choose a compact smooth collar $W=c(S\times[0,a_0])$ in $\Sigma$ using F4 and F5. The complements of the nested closed sets $H_n$ for sufficiently large integer physical radii $n$ cover $W$: boundary points lie in none of them, and every interior point has finite physical radius or is outside the physical chart. A finite subcover gives one $n$ with $W\cap H_n=\varnothing$. Every base point of $W\setminus S$ therefore belongs to the original compact physical truncation $B_0\setminus\{r>n\}$. The continuous adapted radius $|y|$ is bounded on this truncation by F5; hence $s\le B$ on $W\setminus S$ for some $B$. On the compact outer collar face $L=c(S\times\{a_0\})$, the continuous $s>1$ has a minimum $m>1$. [F4, F5, step 2.1, choose]

4.1 Choose $0<\eta<m-1$ and set $H=G(y^{-1}(\{1<|y|<1+\eta\}))$. Radial segments and paths in $S^2$ join any two points of this shell; composition with $G$ gives paths in $H$, so [F6] makes $H$ connected. In the interior manifold the boundary of the open collar portion $W^\circ=c(S\times(0,a_0))$ is exactly $L$: the closed collar $W$ is closed by compactness and the Hausdorff property, and the collar chart leaves only its outer face after removing $S$. Thus $H\cap W^\circ$ is clopen in $H$, since $H$ avoids $L$. It is nonempty. Indeed, fix $p\in S$ and consider $c(p,a_0/n)$ for integers $n\ge2$. These points converge to $p$ in $\Sigma$ and have $s\le B$ by step 3.1. If they all had $s\ge1+\eta$, they would lie in the compact graph image $G(y^{-1}(\{1+\eta\le|y|\le B\}))$, closed in the Hausdorff manifold $\Sigma$ by [F5]; their boundary limit $p$ would then lie in that interior graph image, a contradiction. Therefore $H\cap W^\circ\ne\varnothing$, and [F6] gives $H\subset W^\circ$. No extension of $G^{-1}$ or of the stationary height to $S$ has been assumed. [F4, F5, F6, step 3.1, choose]

5.1 Fix $R$ sufficiently large for the physical end and write $K_R=B_0\setminus\{r>R\}$, compact by F4. The set $K_R\cap\{|y|\ge1+\eta\}$ is compact, contained in $C$, and has compact graph image by F5. Step 4.1 puts all remaining points of $G(K_R\cap C)$ in $W$. Thus $\Sigma\setminus G(\{r>R\})$ is a closed subset of the compact union $W\cup G(K_R\cap\{|y|\ge1+\eta\})$ and is compact. The same proof applies at $2R$. Since $r_q=qr$ in the physical chart, these are exactly the truncated complement and compact core required by the positive-lapse supplier, with $R_q=qR$. No equality between $r$ and $s$ was used. [F4, F5, step 3.1, step 4.1, choose]

6.1 The compact-core conclusion of step 5.1 and individual end slope limit verify the remaining hypotheses of [F1] separately for each pair. Its individual decay gives the required end height and slope limits, hence $0<N\le d_q/(4q)\le C_\delta$. For $D=-g_q^{-1}(d(t_q-\widetilde u),d(t_q-\widetilde u))$, $N=(d_q/(4q))D^{-1/2}$ gives $D\ge1$. The uniform inverse end metric has spatial block at least $I/2$, so $|D\widetilde u|^2/2\le Cr_q^{-1}+Cr_q^{-2}|D\widetilde u|$. Absorb the last term to obtain the stated common slope bound. This calculation uses no uniform radius for the initial individual end limits. [A1, F1, step 5.1, given, algebra]

7.1 Directly normalize the conormal of the stationary graph and set its divergence equal to zero. Write $x=x_q$, $r=r_q$ and $u=\widetilde u$ in this end calculation. The result is $\partial_i P^i(x,Du)=0$, with $P^i=\sqrt{-\det g_q}(g_q^{ij}p_j-g_q^{i0})/\sqrt{-g_q^{00}+2g_q^{0j}p_j-g_q^{jk}p_jp_k}$. The common slope bound and end metric derivatives give a common elliptic nondivergence equation $\mathscr Lu=a^{ij}u_{ij}+b^ju_j=f$, with symmetric $a=I+O(r^{-1})$, $b=O(r^{-2})$, $|f|\le C_fr^{-3}$ and no zeroth-order term. Here the coefficients are evaluated along the supplied graph and then kept fixed when applying $\mathscr L$ to a comparison function. Fix $0<\mu<1$. Direct differentiation gives $\mathscr L(r^{-\mu})=-\mu(1-\mu)r^{-\mu-2}+O(r^{-\mu-3})\le-c_\mu r^{-\mu-2}$ beyond a common radius. Fix any $r_*$ beyond this radius, let $M(r_*)=\max_{|x|=r_*}|u(x)|$, and choose a common $K>0$ with $c_\mu K>C_f$. Set $w(x)=(M(r_*)+K/r_*)(r_*/r)^\mu$. Then $-\mathscr Lw\ge c_\mu K(r/r_*)^{1-\mu}r^{-3}>|f|$ for $r\ge r_*$. [A1, F1, F3, step 6.1, algebra, choose]

8.1 For each fixed indexed pair and $\varepsilon>0$, its individual limit $u\to0$ gives an outer radius $R_\varepsilon>r_*$ such that $|u|\le\varepsilon$ for $r\ge R_\varepsilon$. On the compact annulus $r_*\le r\le R_\varepsilon$, both $z_+=u-w-\varepsilon$ and $z_-=-u-w-\varepsilon$ are nonpositive on the boundary, while $\mathscr Lz_\pm=\pm f-\mathscr Lw>0$ in its interior. If either function were positive somewhere, [F3] would give a positive interior maximum with zero gradient and Hessian $H\le0$. Since $a>0$, [F3] applied to $P=a$ and $Q=-H$ gives $\mathscr Lz_\pm=\operatorname{tr}(aH)\le0$ there, a contradiction. Thus $|u|\le w+\varepsilon$ on the annulus; outside it the same inequality holds because $w\ge0$ and $|u|\le\varepsilon$. Letting $\varepsilon\downarrow0$ at each fixed end point proves $|u(r)|\le(M(r_*)+K/r_*)(r_*/r)^\mu$ for all $r\ge r_*$. The outer radius can depend on the pair; no uniform initial decay radius or convergence rate is needed. [F3, step 7.1, algebra]

9.1 Fix a unit vector $\omega\in S^2$ and put $h(t)=u(t^2\omega)$ on $[\sqrt{r_*},2\sqrt{r_*}]$. The radial curve lies in the common end, where $u$ is smooth, so $h$ is continuous on this closed interval and differentiable on its interior. By the chain rule in [F7] and the slope bound of step 6.1, $h^{\prime}(t)=2t\,Du(t^2\omega)\cdot\omega$ and $|h^{\prime}(t)|\le2tC_\delta(t^2)^{-1/2}=2C_\delta$. The mean value theorem in [F7] therefore gives $|u(4r_*\omega)-u(r_*\omega)|\le2C_\delta\sqrt{r_*}$. Combining this with step 8.1 at $4r_*\omega$ and taking the maximum over $\omega$ gives $M(r_*)\le4^{-\mu}(M(r_*)+K/r_*)+2C_\delta\sqrt{r_*}$. Fix one common sufficiently large $r_*$ and absorb the factor $4^{-\mu}<1$. This bounds $M(r_*)$ and hence the full height decay uniformly over the indexed pairs. No uniform individual convergence rate was assumed to justify annular comparison. [A1, F7, step 6.1, step 7.1, step 8.1, algebra]

10.1 On fixed rescaled annuli, the explicit flux in step 7.1 has common ellipticity and joint C4-Holder bounds on a fixed slightly enlarged slope ball: the slopes are small by step 6.1 and the background has common five differentiated end bounds. Its zero-slope divergence is O($R^{-2}$) in the rescaled C2-Holder norm, since $P(x,0)=O_5(r^{-2})$. Apply [F2] with the common normalized height bound from step 9.1. It yields $\|u(R\cdot)\|_{C^{4,\alpha}(A_{\mathrm{in}})}\le C(\sup_{RA}|u|+R^{-1})$. Taking $\mu=3/4$ proves the asserted uniform differentiated and scaled Holder estimates. Every estimate is indexed by a pair actually present in $\mathcal I$. [A1, F1, F2, step 6.1, step 7.1, step 9.1, algebra] ∎

## Source notes

Radu’s Section 5.3, Lemma 5.1 gives compact-graph convergence under its own boundary, topology, lapse and height hypotheses. This is background for the present adaptation; the indexed noncompact conclusion is established only by the local argument and declared suppliers.

These explicit premises specify the generated conditional result. They are not asserted to follow from the original regularity definition alone, and are not attributed to the original article. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

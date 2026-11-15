---
id: pthm-nearby-stationary-projection
title: Proper stationary projection for continued slices
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - math:def-axiom-of-choice
  - pthm-original-lapse-and-product
  - def-stationary-maximal-graph
  - pthm-local-hawking-circle-fields
  - pthm-bifurcate-horizon-preservation
  - pthm-common-reference-collar
  - lem-author-78c700cb9e03-bounded-rapidity-reference-graph
  - lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow
  - lem-author-45355d85383b-relative-timelike-flow-chart
  - lem-author-45355d85383b-weighted-holder-completeness
  - pthm-maximal-linearization
  - def-normal-graph-and-mean-curvature-data
  - def-stationary-asymptotic-decay-data
  - pthm-positive-transformed-lapse
  - lem-exterior-lapse-maximum-and-boundary-control
  - def-spacelike-maximal-hypersurface-data
  - math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - lem-author-18fcf05360ee-existing-graph-stationary-projection
  - lem-author-18fcf05360ee-scaled-stationary-collar-coefficients
  - lem-author-18fcf05360ee-uniform-stationary-return-with-tangential-motion
  - lem-author-18fcf05360ee-collar-and-end-properness
  - lem-author-18fcf05360ee-one-sheet-stationary-projection
  - lem-author-78c700cb9e03-invariant-normal-boost-coordinates
  - lem-author-78c700cb9e03-uniform-family-spacelike-reference-collar
  - lem-author-c9fb06089ef2-smooth-fixed-boundary-maximal-graphs
  - math:def-connected-space
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - lem-author-a4a441da4986-exact-outer-cauchy-section
  - math:thm-compactness-under-continuous-maps
  - math:thm-closed-subspace-of-a-compact-space-is-compact
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  pthm-original-lapse-and-product: physical-result
  def-stationary-maximal-graph: mathematical-premise
  pthm-local-hawking-circle-fields: physical-result
  pthm-bifurcate-horizon-preservation: physical-result
  pthm-common-reference-collar: physical-result
  lem-author-78c700cb9e03-bounded-rapidity-reference-graph: mathematical-premise
  lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow: mathematical-premise
  lem-author-45355d85383b-relative-timelike-flow-chart: formulation-prerequisite
  lem-author-45355d85383b-weighted-holder-completeness: mathematical-premise
  pthm-maximal-linearization: formulation-prerequisite
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  pthm-positive-transformed-lapse: physical-result
  lem-exterior-lapse-maximum-and-boundary-control: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  lem-author-18fcf05360ee-existing-graph-stationary-projection: mathematical-premise
  lem-author-18fcf05360ee-scaled-stationary-collar-coefficients: mathematical-premise
  lem-author-18fcf05360ee-uniform-stationary-return-with-tangential-motion: mathematical-premise
  lem-author-18fcf05360ee-collar-and-end-properness: mathematical-premise
  lem-author-18fcf05360ee-one-sheet-stationary-projection: mathematical-premise
  lem-author-78c700cb9e03-invariant-normal-boost-coordinates: mathematical-premise
  lem-author-78c700cb9e03-uniform-family-spacelike-reference-collar: mathematical-premise
  lem-author-c9fb06089ef2-smooth-fixed-boundary-maximal-graphs: mathematical-premise
  math:def-connected-space: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  lem-author-a4a441da4986-exact-outer-cauchy-section: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:thm-closed-subspace-of-a-compact-space-is-compact: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp.13–14, §3.1 continuation and properness paragraph
      reading_limits: Read the frozen original-article continuation/lapse paragraph
        and full properness paragraph. This ordinary reference is attribution
        only. The full tangential-motion return estimate, existence of
        projection before that estimate, compact-truncation bridge and one-sheet
        reasoning are authored in the present local chain, not claimed to be
        supplied by that paragraph.
physical_scope: Conditional local continuation geometry in the stationary
  vacuum/Harrison construction for a fixed positive reference parameter and
  nearby positive parameters. Existing and continued maximal sections are
  supplied candidates; no global existence or causal property of a deformed
  exterior is inferred.
dependency_level: 12
---

## Statement

Work in ZFC, including the Axiom of Choice. Adopt the regular mass-one stationary vacuum/Harrison construction, with original exterior section maximal and $T|_S\not\equiv0$. Fix $0<\delta<q_*\le1$ and an existing connected smooth spacelike maximal stationary graph $\Sigma_*=\Sigma_{q_*}$, smooth up to its compact boundary $S$. On its normalized end $t_{q_*}=\widetilde u_*(x_{q_*})$, assume $|D^j\widetilde u_*|\le C r_{q_*}^{-3/4-j}$ for $0\le j\le4$, where $D^j$ denotes spatial derivatives of order $j$ in $x_{q_*}$ and $r_{q_*}=|x_{q_*}|$. These reference estimates are hypotheses, not consequences of height normalization alone. Fix the smooth future timelike transverse field $Y$ used for continuation, equal to the future reference normal near $S$ and to $T$ sufficiently far out. For nearby physical parameters $q\in[\delta,1]$ let $\Sigma_q$ be a supplied admissible small fixed-boundary continuation flow graph $F_w(x)=\phi_{w(x)}^Y(x)$ over $\Sigma_*$, with the weighted $C^{4,\alpha}_\beta$ smallness and end conditions from the continuation construction, where $0<\alpha<1$ and $-1<\beta<0$; $\beta=-3/4$ is the article's choice. Assume the candidate is maximal for $g_q$. Existence of the candidate is a premise; neither linearization nor the present item asserts existence of an eventual continuation family.

The candidate is smooth up to $S$ and throughout its interior. The stationary projection $\pi:\Sigma_q^\circ\to\Sigma_*^\circ$ exists globally, is a local diffeomorphism by positive transformed lapse, and is proper. Near $S$, write $\rho_*$ for induced distance on the reference slice. Its Hopf lower bound is $N_*\ge c\rho_*$. The Dirichlet condition and small $C^1$ norm give $|w|\le\epsilon\rho_*$. A stationary orbit starting at $F_w(x)$ meets the reference slice within time at most $4\epsilon/c$ after a common shrinking, with return boundary distance comparable to $\rho_*(x)$. The constants are uniform for all graphs in this fixed small neighborhood of the supplied reference; they may depend on that reference and a positive lower parameter bound. Tangential stationary motion is fully included in this estimate.

On the exterior end the composite $P=\pi\circ F_w$ is exactly the identity because $Y=T$. The proper local diffeomorphism has one sheet, hence $\pi$ and $P$ are global diffeomorphisms. Thus the continued slice is a global $T$-graph over the existing stationary graph and, by composition, over the original section. No global hyperbolicity of the transformed exterior is invoked.

The original-section maximality used here is assumed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$, with the original metric $g$, so $H_g|_C=0$. The selected physical end retains its stated mass-one normalization. Maximality of an independently labelled chart-side section or another supplied maximal section does not replace this premise. No equality between the hypersurface identification and the physical stationary end chart is assumed. [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-harrison-normalization]]

[[math:def-axiom-of-choice]]

[[pthm-original-lapse-and-product]]

[[def-stationary-maximal-graph]]

[[pthm-local-hawking-circle-fields]]

[[pthm-bifurcate-horizon-preservation]]

[[pthm-common-reference-collar]]

[[lem-author-78c700cb9e03-bounded-rapidity-reference-graph]]

[[lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow]]

[[lem-author-45355d85383b-relative-timelike-flow-chart]]

[[lem-author-45355d85383b-weighted-holder-completeness]]

[[pthm-maximal-linearization]]

[[def-normal-graph-and-mean-curvature-data]]

[[def-stationary-asymptotic-decay-data]]

[[pthm-positive-transformed-lapse]]

[[lem-exterior-lapse-maximum-and-boundary-control]]

[[def-spacelike-maximal-hypersurface-data]]

[[math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets]]

[[def-stationary-lorentzian-data]]

[[def-bifurcate-killing-horizon-data]]

[[lem-author-18fcf05360ee-existing-graph-stationary-projection]]

[[lem-author-18fcf05360ee-scaled-stationary-collar-coefficients]]

[[lem-author-18fcf05360ee-uniform-stationary-return-with-tangential-motion]]

[[lem-author-18fcf05360ee-collar-and-end-properness]]

[[lem-author-18fcf05360ee-one-sheet-stationary-projection]]

[[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]]

[[lem-author-78c700cb9e03-uniform-family-spacelike-reference-collar]]

[[lem-author-c9fb06089ef2-smooth-fixed-boundary-maximal-graphs]]

[[math:def-connected-space]]

[[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

[[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[[lem-author-a4a441da4986-exact-outer-cauchy-section]]

[[math:thm-compactness-under-continuous-maps]]

[[math:thm-closed-subspace-of-a-compact-space-is-compact]]

## Facts & Assumptions

[A1] Work in ZFC, including Choice. The model, regular data, maximal original section, mass-one convention and rotating-case condition $T|_S\not\equiv0$ are standing hypotheses. The existing reference and nearby maximal candidates are supplied as stated, with $0<\delta<q_*\le1$ and $q\in[\delta,1]$ nearby. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-harrison-normalization]] [[math:def-axiom-of-choice]]

[F1] The original complete stationary product exists, and an existing stationary graph gives the explicit global projection before any collar estimate. [[pthm-original-lapse-and-product]] [[def-stationary-maximal-graph]] [[lem-author-18fcf05360ee-existing-graph-stationary-projection]]

[F2] The completed local fields, preserved horizon boost and complete common-reference collar supply invariant boost/circle coordinates. The original and existing spacelike reference sections have bounded rapidity there; once positive stationary lapse is established independently, it fixes the stationary crossing sign. [[pthm-local-hawking-circle-fields]] [[pthm-bifurcate-horizon-preservation]] [[pthm-common-reference-collar]] [[lem-author-78c700cb9e03-bounded-rapidity-reference-graph]] [[lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow]] [[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]] [[lem-author-78c700cb9e03-uniform-family-spacelike-reference-collar]]

[F3] The candidate is supplied as an admissible embedded spacelike $C^{4,\alpha}$ fixed-boundary flow graph, with $Y=T$ at infinity. Use the flow-graph convention and its $C^{4,\alpha}$ interpretation. [[def-normal-graph-and-mean-curvature-data]] [[lem-author-45355d85383b-relative-timelike-flow-chart]] The continuation-space notation is $X_\beta=\{w\in C^{4,\alpha}_\beta:w|_S=0\}$, as in the maximal-linearization supplier. [[pthm-maximal-linearization]] This zero-trace weighted space is Banach. [[lem-author-45355d85383b-weighted-holder-completeness]] The reference end estimates $|D^j\widetilde u_*|\le C r_{q_*}^{-3/4-j}$ for $0\le j\le4$ are assumed explicitly; the fixed-chart weighted bounds give $Dw=O(r^{\beta-1})$. [[def-stationary-asymptotic-decay-data]] Reference smoothness and candidate admissibility are premises. No normal-on-compact-core construction, weighted mean-curvature mapping theorem or reference-regularity conclusion is invoked here.

[F4] For a supplied connected smooth maximal section with compact-core exterior structure and the stated end-slope condition, the transformed-lapse theorem gives a positive interior lapse, zero boundary value and a positive end limit. Its lapse equation has nonnegative potential. Once these hypotheses are verified for the reference, the boundary-control supplier gives a strictly positive inward derivative and $N_*\ge c\rho_*$ on a fixed boundary collar. [[pthm-positive-transformed-lapse]] [[lem-exterior-lapse-maximum-and-boundary-control]] [[def-spacelike-maximal-hypersurface-data]]

[F5] The other four local helpers account for the full stationary coefficients, uniform return with tangential drift, global properness, and the one-sheet argument. [[lem-author-18fcf05360ee-scaled-stationary-collar-coefficients]] [[lem-author-18fcf05360ee-uniform-stationary-return-with-tangential-motion]] [[lem-author-18fcf05360ee-collar-and-end-properness]] [[lem-author-18fcf05360ee-one-sheet-stationary-projection]] [[math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets]]

[F6] Lorentzian, flow and horizon terminology have the stated mathematical conventions. A spacelike section has a smooth future unit normal $n$, lapse $N=-g(T,n)$ and orthogonal decomposition $T=Nn+X$ with $X$ tangent. [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]] [[def-spacelike-maximal-hypersurface-data]]

[F7] An admissible $C^{4,\alpha}$ spacelike flow graph solving the maximal equation in a smooth Lorentzian metric, with zero height on compact smooth $S$, is smooth up to $S$ and at every interior point. This local regularity does not assert higher weighted end estimates or parameter regularity. [[lem-author-c9fb06089ef2-smooth-fixed-boundary-maximal-graphs]]

[F8] Connectedness excludes a partition into two nonempty disjoint open sets. [[math:def-connected-space]] A diffeomorphism is a bijective smooth map with smooth inverse; a local diffeomorphism has such restrictions onto open neighborhoods. [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]] A smooth map with an isomorphism as its differential at a point has a smooth local inverse there. [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[F9] For the same regular data, put $C=\Sigma_0\cap\mathcal E$ and $B=C\cup S$. The exterior-closure supplier gives a smooth adapted identification $\chi:B\to\{|y|\ge1\}$, its compact radial truncations, and the independent physical end $V_R=\{t=0,r>R\}$. Its compact physical truncations $B_R=B\setminus V_R$ are cofinal among compact subsets of $B$ (Proof 6.1); neither maximality nor a stationary product is required for this input. [[lem-author-a4a441da4986-exact-outer-cauchy-section]] Continuous images of compact sets are compact, and continuous real functions on nonempty compact sets attain finite extrema. [[math:thm-compactness-under-continuous-maps]] Closed subsets of compact spaces and finite unions of compact subsets are compact. [[math:thm-closed-subspace-of-a-compact-space-is-compact]]

## Proof

**Given:**The stated data and complete hypotheses.

**Goal:** Establish the conclusions with the specified uniformity and domains.

1.1 The existing section is already a global stationary graph $j(x)=(u_*(x),x)$ in the complete stationary product of [F1]. Its tangent vectors are $(du_*(v),v)$, so $T=(1,0)$ cannot be tangent: its zero spatial component would force $v=0$ and hence a zero time component. By the normal decomposition in [F6], $N_*=-g_{q_*}(T,n_*)$ therefore never vanishes in the interior. It is smooth, and that interior is connected as the graph over the connected original exterior. On the supplied end $Y=T$ is future timelike, so its contraction with the future unit normal gives $N_*>0$ there. A continuous nowhere-zero real function on a connected space cannot take both signs: its positive and negative sets would be disjoint nonempty open sets partitioning that space. Thus $N_*>0$ everywhere inside. This establishes the reference sign using the supplied end field and graph formula before applying any compact-core or transformed-lapse theorem. The first clause of the existing-graph helper in [F1] also gives the complete product based on $\Sigma_*$ and its global projection, independently of collar estimates or any new graph conclusion for $\Sigma_q$. [A1, F1, F6, F8, given]

2.1 For compact exhaustion, apply the collar clause of the existing-graph helper in [F1], with reference positivity from step 1.1 and original positivity from the original-lapse result. The completed boost model in [F2] represents the original and existing sections as bounded-rapidity graphs. The local boost/Taylor argument in that helper makes $K$ future timelike on the small outer collar of either spacelike section; positive boost rate is unchanged in future/outward normal bases. Thus the positive stationary lapses give the unique crossing on each, and their full small boundary collars correspond under the stationary quotient with comparable radial boundary coordinates. Use the adapted identification $\chi$ of [F9] on the original section; it extends smoothly across $S$ to the usual closed spherical exterior. Thus the usual-compactification hypothesis of the collar helper holds in these coordinates. Write $a=|\chi(\cdot)|$ on $B$ and $J:C\to\Sigma_*^\circ$ for the existing graph map from step 1.1. The adapted annuli lift under $J$ to compact annular truncations between the full reference collar and the adapted graph end $J(\{a>A\})$. This conclusion concerns adapted coordinates only. [A1, F1, F2, F6, F9, step 1.1]

3.1 Match the independent end charts without equating their maps. For a sufficiently large physical radius $R$, $B_R$ is compact by [F9], so the continuous $a$ has a finite maximum there. Any adapted tail beyond that maximum lies in $V_R$. Conversely, $K_A=\{a\le A\}\subset B$ is compact for every $A>1$ by [F9]. Cofinality of the physical truncations gives an $R$ with $K_A\subset B_R$, hence $V_R\subset\{a>A\}$. Transporting both inclusions by $J$ proves cofinality of the two graph ends; rescaling $x_{q_*}=q_*x$ changes only the positive radius threshold. Removing a full reference collar and a sufficiently far physical graph end now leaves a closed subset of one adapted compact annular truncation from step 2.1, so it is compact by [F9]. Adding the compact closed smaller reference collar, including $S$, gives the compact physical-end complement required by the lapse theorem. For the later one-sheet application choose a smaller original boost collar $Q_0$ with compact closure, as in the collar helper. The continuous $a$ is bounded on that closure by [F9]. The full correspondence in step 2.1 takes $Q_0$ onto a reference collar $Q_*$, so $a_*=a\circ J^{-1}$ is bounded on $Q_*$. This is precisely a bounded target-collar radius in the adapted coordinates, regardless of its physical coordinate description. These facts use no transformed-lapse conclusion. [F1, F9, step 1.1, step 2.1]

4.1 The reference is supplied smooth up to $S$, connected, spacelike and maximal. Step 3.1 verifies its compact-core exterior structure, while the assumed reference derivative estimates in [F3] imply its normalized end gradient tends uniformly to zero. Thus the transformed-lapse theorem in [F4] now applies to the reference, supplying its lapse equation, nonnegative potential, zero boundary value and positive end limit. The boundary-control supplier in [F4] gives a strictly positive inward derivative and, on a fixed smaller collar, $N_*\ge c\rho_*$ for some $c>0$. These constants belong to the fixed supplied reference. [A1, F3, F4, step 1.1, step 2.1, step 3.1]

5.1 By [F3], $F_w$ is an admissible flow graph and equals stationary translation on the end. On a compact interior core, sufficiently small graphs remain in the open exterior. At the boundary, the scaled-collar helper in [F5] places $|s|\le\eta\rho_*$ between the two smooth null event-boundaries, so $|w|\le\epsilon\rho_*$ keeps the punctured graph in the exterior there as well. The bound on $w$ follows by integrating its small radial derivative from $w|_S=0$. Hence the global projection from step 1.1 is defined on all of $\Sigma_q^\circ$. The supplied graph has $C^{4,\alpha}$ regularity up to the fixed smooth boundary, solves the maximal equation in the smooth metric $g_q$, and has $w|_S=0$. Thus [F7] makes it smooth up to $S$ and throughout the interior. It is connected and has one exterior end because it is an embedded flow graph over the connected reference with the physical compact truncations from step 3.1. On the end, $Y=T$ means its original-time height is $u_*+w$. The assumed reference derivative estimates and the weighted bound $D w=O(r^{\beta-1})$ imply that its normalized height has spatial gradient tending uniformly to zero; the positive time and spatial normalization factors are constant on each slice. Its end is therefore an explicit stationary graph with the end-slope condition required by [F4]. The positive-lapse theorem now applies to this smooth supplied maximal candidate without assuming its interior is already a stationary graph. It makes $T$ transverse. In the product coordinates from step 1.1, the differential of the stationary projection has kernel exactly $\mathbb RT$. Its restriction to the three-dimensional tangent space of the candidate is injective by transversality and therefore is an isomorphism onto the three-dimensional target tangent space. The smooth inverse function theorem in [F8] consequently makes this restriction a local diffeomorphism. [A1, F1, F3, F4, F5, F7, F8, step 1.1, step 2.1, step 3.1, step 4.1]

6.1 In the reference $Y$ chart, retain the tangential term: $T=a\partial_s+b\partial_{\rho_*}+W$. The scaled coefficient and uniform-return lemmas give $a\ge(c/2)\rho_*$ and $|b|\le B\rho_*$ throughout the chosen wedge. They follow the moving $y$ on compact $S$, control $\rho_*$ by Grönwall, and force a meeting with $s=0$ within $4\epsilon/c$, with uniformly comparable boundary distances. The global existing-graph projection identifies this actual local meeting with $P(x)$. Thus a base sequence approaching $S$ has projected points approaching $S$, even though its stationary flow moves tangentially. [F1, F4, F5, step 4.1, step 5.1]

7.1 On the physical graph end, $P(x)=x$ exactly because $Y=T$. Step 3.1 puts a sufficiently far adapted graph end inside this physical end, so the identity holds on the adapted end required by the helpers as well. The compact truncations from steps 2.1 and 3.1 and the boundary comparison in step 6.1 give properness by the properness helper. The target is the actual connected stationary graph, with adapted diffeomorphism $J\circ\chi^{-1}:\{|y|>1\}\to\Sigma_*^\circ$. Apply the finite-sheet theorem in these adapted coordinates. Shrink the source collar until its return image lies in the bounded-adapted-radius target collar $Q_*$ from step 3.1. The remaining middle annulus is compact, and $a_*\circ P$ has a finite maximum there by [F9]. A target point beyond both this maximum and the collar bound, and in the adapted identity end, therefore has no preimage in the collar or middle annulus and has exactly itself as preimage in the end. These are the explicit hypotheses of the one-sheet helper in [F5]. The sheet number is consequently one, and the smooth local inverses give a global diffeomorphism in the sense of [F8]. Composing with the known existing graph and original stationary product gives the asserted global $T$-graph of the continued slice. [F1, F3, F5, F8, F9, step 1.1, step 2.1, step 3.1, step 5.1, step 6.1] ∎

## Source notes

These explicit premises specify the generated conditional result. They are not asserted to follow from the original regularity definition alone, and are not attributed to the original article. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

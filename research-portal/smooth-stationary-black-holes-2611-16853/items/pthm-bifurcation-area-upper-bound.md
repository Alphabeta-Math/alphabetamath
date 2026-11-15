---
id: pthm-bifurcation-area-upper-bound
title: "Theorem 4.1: limiting horizon area upper bound"
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - def-harrison-one-form
  - pthm-distance-divergence-area-comparison
  - pthm-comparison-sphere-properties
  - pthm-harrison-electrovacuum
  - pthm-bifurcate-horizon-preservation
  - math:def-riemannian-volume-form-on-an-oriented-manifold
  - math:thm-dominated-convergence
  - math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density
  - def-harrison-one-form-family
  - def-killing-ernst-notation
  - pthm-global-harrison-one-form
  - pthm-harrison-component-asymptotics
  - lem-author-294e9b08725d-regular-positive-stationary-mass
  - pthm-horizon-invariant-one-form
  - pthm-complete-maximal-slices
  - pthm-past-boundary-localization
  - pthm-smooth-area-controlled-cut
  - def-near-horizon-past-boundary-sets
  - def-coordinate-comparison-spheres
  - lem-author-60420990c802-uniform-inward-normal-exponential-collar
  - lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-harrison-one-form: mathematical-premise
  pthm-distance-divergence-area-comparison: physical-result
  pthm-comparison-sphere-properties: physical-result
  pthm-harrison-electrovacuum: physical-result
  pthm-bifurcate-horizon-preservation: physical-result
  math:def-riemannian-volume-form-on-an-oriented-manifold: mathematical-premise
  math:thm-dominated-convergence: mathematical-premise
  math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density: mathematical-premise
  def-harrison-one-form-family: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  pthm-global-harrison-one-form: physical-result
  pthm-harrison-component-asymptotics: physical-result
  lem-author-294e9b08725d-regular-positive-stationary-mass: mathematical-premise
  pthm-horizon-invariant-one-form: physical-result
  pthm-complete-maximal-slices: physical-result
  pthm-past-boundary-localization: physical-result
  pthm-smooth-area-controlled-cut: physical-result
  def-near-horizon-past-boundary-sets: mathematical-premise
  def-coordinate-comparison-spheres: mathematical-premise
  lem-author-60420990c802-uniform-inward-normal-exponential-collar: mathematical-premise
  lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional geometric deduction in the smooth stationary vacuum
  model and its specified Harrison family; no observation or measurement is
  asserted.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 23 and 26, Theorem 4.1 and its final proof
      attribution: In the mass-one Harrison family the bifurcation-sphere area at q=0
        is at most 4π, obtained using the positive-q area comparison and the
        comparison-sphere limit.
      hypotheses: The article's regular stationary vacuum construction, mass-one
        normalization, maximal original exterior section and nontrivial
        restriction of T to S.
      reading_limits: Historical reading note retained from the current source; this
        maintenance revision claims no fresh article or external full-text
        reading. Read Theorem 4.1 and its final proof in the actual frozen PDF,
        pp. 23 and 26, using text extraction. Attribution only; this citation is
        not used as a proof premise.
dependency_level: 33
---

## Statement

Adopt the stationary vacuum model and the regular stationary vacuum data. Suppose the actual original exterior section $\Sigma_0\cap\mathcal E$ is spacelike and maximal, the ADM mass of its designated end is one, and $T|_S\not\equiv0$, with the meanings in the spacelike maximal-section definition and the mass-one Harrison normalization. Choose once the smooth normalized stationary primitive $W_0$ of the global one-form construction, with its single normalized Ernst potential $\sigma$ and pole $p\in S$, $T_p=0$. This choice is locally $K$-invariant near $S$ and has spatial coefficients $(W_0)_i=O_5(r^{-3})$ in the unchanged original end chart. Here $K$ is the local Hawking field of the construction. Set $W_q=(1-q)^2W_0-4q(1-q)T^\flat$ and let $g_q$, $0\le q\le1$, be its regular Harrison metric. Use this same potential, pole, primitive and metric family for the horizon and comparison-sphere suppliers. For the comparison spheres $C_q$ of the comparison-sphere result, the area comparison $|S|_{g_q}\le |C_q|_{g_q}$ holds for all sufficiently small $q>0$, and $|C_q|_{g_q}\to4\pi$ as $q\downarrow0$. Consequently $|S|_{g_0}\le4\pi$.

Here $|S|_{g_q}$ and $|C_q|_{g_q}$ mean the integrals of the positive area densities induced by $g_q$ on the respective spacelike two-surfaces.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-harrison-normalization]]

[[def-harrison-one-form]]

[[def-harrison-one-form-family]]

[[pthm-global-harrison-one-form]]

[[pthm-comparison-sphere-properties]]

## Facts & Assumptions

[A1] The model, regular data, original maximal section, mass-one convention and nontrivial restriction of $T$ are as stated above. The supplied regular Harrison family uses the metric construction of [[def-harrison-one-form]]. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]] [[def-harrison-normalization]]

[F1] At each fixed sufficiently small $q>0$, for the supplied complete smooth spacelike maximal section with compact boundary $S$ and a sufficiently small smooth intrinsic boundary-distance collar, the localized cut construction in the divergence-comparison result supplies smooth comparison regions $\Omega_\epsilon\subset\{0\le\rho\le\eta\}$ with boundary $S\sqcup D_\epsilon$ and $|D_\epsilon|\le|C_t|_{g_q}+\epsilon$. Its fixed-collar divergence estimate is uniform in the region, smoothing parameter and late target; sending $\epsilon\downarrow0$ and then $\eta\downarrow0$ at fixed $q$ gives $|S|_{g_q}\le |C_q|_{g_q}$. [[pthm-distance-divergence-area-comparison]]

[F2] For the same construction and comparison spheres, $|C_q|_{g_q}\to4\pi$ as $q\downarrow0$. [[pthm-comparison-sphere-properties]]

[F3] The Harrison metrics are jointly smooth in spacetime and $q\in[0,1]$ near $S$. The fixed sphere $S$ is compact and $g_q$-spacelike for every $q\in[0,1]$. [[pthm-harrison-electrovacuum]] [[pthm-bifurcate-horizon-preservation]] [[def-regular-stationary-vacuum-spacetime]]

[F4] For a positive-definite metric on an oriented surface, its area form in a positive chart is $\sqrt{\det(h_{ij})}\,dx^1\wedge dx^2$; its associated positive density is independent of the chart. [[math:def-riemannian-volume-form-on-an-oriented-manifold]]

[F5] On a measure space, pointwise almost-everywhere convergence under a single integrable majorant implies convergence of integrals. [[math:thm-dominated-convergence]]

[F6] Under countable choice, the Riemannian density defines a Radon Borel measure finite on compact sets, and integrals of compactly supported smooth functions against that measure agree with smooth density integrals. [[math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density]]

[F7] The global one-form construction supplies a single smooth stationary normalized primitive $W_0$ on the exterior and a neighborhood of $S$, with $dW_0=4((f-1)F+\psi\star_gF)$, $W_0(T)=D_0(p)-D_0$, local $K,Z$ invariance and spatial coefficients $(W_0)_i=O_5(r^{-3})$ in the unchanged original chart. Choose this primitive once. The one-form-family definition then fixes $W_q=(1-q)^2W_0-4q(1-q)T^\flat$ using the same normalized potential and pole for every $q$. [[pthm-global-harrison-one-form]] [[def-harrison-one-form-family]] The invariant-Ernst result gives local $K$ invariance of this same normalized potential $\sigma$; its invariance proof concerns the normalized potential, independently of the primitive choice. [[pthm-horizon-invariant-one-form]]

[F8] Under the regular stationary-vacuum hypotheses, the original stationary end coefficient equals the ADM energy of the same complete exterior section: $M_0=E_{\mathrm{ADM}}$. Thus the stated ADM normalization gives $M_0=1$ in the original stationary chart, without identifying that chart with a separate spherical parametrization. [[lem-author-294e9b08725d-regular-positive-stationary-mass]] [[def-harrison-normalization]]

[F9] The component-estimate supplier requires the original mass-one stationary end, a supplied original smooth spacelike maximal section with ADM limit one, the normalized potential and pole, the Harrison one-form conditions, and spatial bounds $(W_0)_i=O_5(r^{-3})$. Its uniform estimates, including at $q=0$, require no equality with an exact radial primitive. [[pthm-harrison-component-asymptotics]] [[def-harrison-one-form]]

[F10] In the same regular mass-one stationary vacuum construction, maximality of the actual original exterior section and $T|_S\not\equiv0$ give, for every $q\in(0,1]$, a complete smooth spacelike $g_q$-maximal stationary graph section $\Sigma_q$ with included compact boundary $S$ and smooth positive induced metric up to $S$. One may use any positive interval containing this fixed $q$; no section at $q=0$ or estimate uniform as $q\downarrow0$ is required. [[pthm-complete-maximal-slices]]

[F11] A smooth Riemannian manifold with compact boundary and smooth positive metric up to the boundary has a uniform inward normal exponential collar. After shrinking, its normal coordinate is the intrinsic distance $\rho$ from $S$, with Gaussian metric $ds^2+h_s$ and $|\nabla\rho|=1$. A closed smaller collar is compact. The near-horizon definition fixes $\rho$ and the levels $S_\eta$ for the supplied section. [[lem-author-60420990c802-uniform-inward-normal-exponential-collar]] [[lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance]] [[def-near-horizon-past-boundary-sets]]

[F12] For this same fixed positive parameter, supplied maximal section and comparison cylinder, localization gives the compact causal cut in every sufficiently small collar once the stationary target $C_t$ is sufficiently late. For that localized construction, the smooth-cut result supplies, for every $\epsilon>0$, a smooth compact region $\Omega_\epsilon\subset\Sigma_q$ with boundary $S\sqcup D_\epsilon$, where $D_\epsilon$ lies between $S$ and $S_\eta$ and $|D_\epsilon|\le|C_t|_{g_q}+\epsilon$. For the collar-contained regions and fixed-collar estimate use the divergence-comparison interface in [F1]. The comparison-sphere definition identifies $C_t$ as the stationary translate of the same $C_q$. [[pthm-past-boundary-localization]] [[pthm-smooth-area-controlled-cut]] [[pthm-distance-divergence-area-comparison]] [[def-coordinate-comparison-spheres]]

[F13] The Killing two-form convention is $F_{ab}=\nabla_aT_b$, with the torsion-free metric-compatible connection and Killing equation $\nabla_aT_b+\nabla_bT_a=0$. The same notation supplies $f=-g(T,T)$ and the normalized potential $\sigma=f+i\psi$. [[def-killing-ernst-notation]]

## Proof

**Given:** The construction and hypotheses in the Statement.

**Goal:** Prove the positive-parameter comparison and the upper bound at $q=0$.

1.1 The primitive in [F7] is chosen with the potential and pole of its construction, not independently for different suppliers. The actual original exterior section in [A1] is the section on which its maximality and ADM normalization are imposed; [F8] gives the required coefficient $M_0=1$ in that section's physical stationary end chart. First verify the one-form conditions locally. By [F13], torsion freeness and the Killing equation give $(dT^\flat)_{ab}=\nabla_aT_b-\nabla_bT_a=2F_{ab}$. Stationarity of $g$ and $T$ gives $\mathcal L_TT^\flat=0$, so the stationarity of $W_0$ in [F7] implies $\mathcal L_TW_q=0$. Differentiating its polynomial definition and using the primitive equation in [F7] yields $dW_q=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$. The denominator in the one-form definition expands as $D_q=(1-q)^2D_0+4q(1-(1-q)f)$. Since $f(p)=0$, $d_q=D_q(p)=(1-q)^2D_0(p)+4q$. Consequently $W_q(T)=(1-q)^2(D_0(p)-D_0)+4q(1-q)f=d_q-D_q$. These are precisely the Harrison one-form conditions of [A1]. The electrovacuum supplier in [F3] applies to this smooth stationary normalized primitive and its polynomial family and gives joint smoothness. The local $K$ invariance of both the primitive and the normalized potential in [F7] matches the horizon-preservation input in [F3], so the fixed compact sphere is spacelike for these same metrics, including $q=0$. For the end estimates in [F9], the original section and ADM limit are [A1], the original mass coefficient is [F8], and the potential, pole and five differentiated spatial decay bounds are [F7]; the one-form conditions were verified above. Thus [F9] applies to this very family. These are the end estimates inherited by the comparison-sphere result in [F2]. No equality of independent gauges or of the physical end chart with an adapted spherical chart is assumed. [A1, F2, F3, F7, F8, F9, F13, algebra]

2.1 Fix any sufficiently small $q>0$. The regular vacuum, actual original-section maximality, mass-one normalization and $T|_S\not\equiv0$ hypotheses of [F10] are exactly [A1] and [F8]. Use the single smooth Harrison family matched in step 1.1, and take the lower parameter bound $\delta=q/2$. The maximal-slice result supplies a complete smooth spacelike $g_q$-maximal stationary graph section $\Sigma_q$ with included boundary $S$. Its induced metric $h=g_q|_{T\Sigma_q}$ is smooth and positive definite up to that compact boundary. This is the section denoted $\Sigma_{q,0}$ in the comparison and cut suppliers; use this same selected section in each application. [A1, F3, F8, F10, step 1.1]

2.2 Let $h_q=g_q|_{TS}$. By [F3], $h_q$ is a jointly smooth family of positive-definite metrics on the compact sphere, including at $q=0$. Orient $S$ and write $\omega_q$ for the positive area density of $h_q$. The adopted model in [A1] works in ZFC, so countable choice is available. By [F6], $\omega_0$ defines a Radon Borel measure $\mu_0$ on $S$, and $\mu_0(S)<\infty$ because $S$ is compact. In a positive chart, [F4] gives $\omega_q=a_q\omega_0$, where $a_q=\sqrt{\det(h_q)/\det(h_0)}$. The coordinate-independent densities make this ratio globally defined; it is smooth on $S$ for each $q$, jointly continuous in $(x,q)$, and tends pointwise to $1$ as $q\downarrow0$. Each $a_q$ has compact support on the compact sphere, so the integration agreement in [F6] identifies $|S|_{g_q}=\int_S\omega_q=\int_S a_q\,d\mu_0$. The functions $a_q$ are Borel measurable, and compactness of $S\times[0,1]$ bounds them by one finite constant, integrable against $\mu_0$. Thus [F5], applied to any sequence $q_n\in(0,1]$ tending to zero, gives $|S|_{g_{q_n}}=\int_S a_{q_n}\,d\mu_0\to\int_S1\,d\mu_0=|S|_{g_0}$. The sequential criterion yields the same one-sided limit as $q\downarrow0$. [A1, F3, F4, F5, F6, step 1.1]

3.1 Apply the two collar results in [F11] to $(\Sigma_q,h)$ from step 2.1. Their smoothness, positivity and compact-boundary hypotheses hold by that step, and their ZFC convention is inherited from [A1]. They supply a smooth intrinsic boundary-distance collar, with $\rho$ equal to its inward normal coordinate even when the distance infimum allows paths outside the collar. Choose a closed smaller collar $\{0\le\rho\le\eta\}$, with a larger smooth collar still available. Thus the intrinsic distance, smooth collar and boundary conventions required by [F1] and [F12] refer to this same section and induced metric. [A1, F1, F11, F12, step 2.1]

4.1 The standing regular-vacuum, mass-one, actual original maximal-section and nontrivial-$T$ hypotheses for [F12] are [A1] and [F8]; its supplied transformed maximal section and intrinsic collar are steps 2.1 and 3.1. Use the comparison cylinder of the same spheres as [F2], with their fixed radius constant chosen sufficiently large for these suppliers. For every sufficiently small $\eta$, localization in [F12] supplies a sufficiently late stationary target $C_t$ and the localized causal cut. Fix that target before choosing $\epsilon$. The smooth-cut result in [F12] then supplies, for every $\epsilon>0$, smooth compact regions in the section, with boundary $S\sqcup D_\epsilon$, $D_\epsilon$ between $S$ and $S_\eta$, and $|D_\epsilon|\le|C_t|_{g_q}+\epsilon$. For the divergence argument, use the collar-contained smooth comparison regions supplied by [F1] for this same localized construction; its interface gives their boundary and area bound as well as its uniform fixed-collar estimate. All these objects use the same $g_q$, section, collar and target as the comparison supplier; the lateness threshold may depend on $q$ and $\eta$. [A1, F1, F2, F8, F10, F11, F12, step 1.1, step 2.1, step 3.1]

5.1 The fixed-$q$ comparison in [F1] now has its complete maximal section, smooth intrinsic distance collar and localized smooth comparison regions from steps 2.1, 3.1 and 4.1. Its uniform fixed-collar estimate sends $\epsilon\downarrow0$ and then $\eta\downarrow0$ with $q$ fixed, giving $|S|_{g_q}\le |C_q|_{g_q}$ for every sufficiently small positive $q$. The comparison-sphere result applies to the same family and gives $|C_q|_{g_q}\to4\pi$. No collar width, late-target threshold or section estimate uniform as $q\downarrow0$ is used. [A1, F1, F2, step 1.1, step 2.1, step 3.1, step 4.1]

6.1 Pass to the limit in the inequality of step 5.1 using step 2.2 and the comparison-sphere limit in [F2]. This gives $|S|_{g_0}\le4\pi$. [F2, step 5.1, step 2.2] ∎

## Source notes

The article citation attributes the original theorem and its limiting argument. The proof above uses the declared comparison and regularity suppliers, with the one-form choice and every end/horizon application matched explicitly in step 1.1 and the transformed section, intrinsic collar and localized smooth-cut inputs supplied in steps 2.1, 3.1 and 4.1, rather than the article's assertion as a premise. The exact original-chart radial integral and the smooth global primitive are not identified. The area comparison and limiting bound are retained for the single smooth locally invariant decaying family. The one-form identities are checked locally above. The smooth-cut statement is used only for its stated region, boundary and area conclusions; the divergence-comparison result supplies the collar-contained regions used in its own estimate. No sublevel property is asserted as a conclusion of the smooth-cut statement. This is a repair of generated supplier matching, not an original-author defect finding or an independent review stamp.

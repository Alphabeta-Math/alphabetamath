---
id: pthm-common-reference-collar
title: "Lemma 3.3: common spacelike reference collar"
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - math:def-axiom-of-choice
  - pthm-original-lapse-and-product
  - pthm-local-hawking-circle-fields
  - def-circle-action-and-invariant-normal-data
  - lem-killing-normal-boost-and-invariant-tensors
  - pthm-harrison-denominator-positive
  - pthm-horizon-invariant-one-form
  - def-harrison-one-form-family
  - pthm-harrison-lorentzian-algebra
  - pthm-bifurcate-horizon-preservation
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - lem-author-78c700cb9e03-invariant-normal-boost-coordinates
  - lem-author-78c700cb9e03-bounded-rapidity-reference-graph
  - lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow
  - lem-author-78c700cb9e03-uniform-family-spacelike-reference-collar
  - lem-author-78c700cb9e03-complete-hawking-reference-product
  - math:def-riemannian-gradient
  - math:def-domain-and-exponential-map-of-a-connection
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  pthm-original-lapse-and-product: physical-result
  pthm-local-hawking-circle-fields: physical-result
  def-circle-action-and-invariant-normal-data: mathematical-premise
  lem-killing-normal-boost-and-invariant-tensors: mathematical-premise
  pthm-harrison-denominator-positive: physical-result
  pthm-horizon-invariant-one-form: physical-result
  def-harrison-one-form-family: mathematical-premise
  pthm-harrison-lorentzian-algebra: physical-result
  pthm-bifurcate-horizon-preservation: physical-result
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  lem-author-78c700cb9e03-invariant-normal-boost-coordinates: mathematical-premise
  lem-author-78c700cb9e03-bounded-rapidity-reference-graph: mathematical-premise
  lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow: mathematical-premise
  lem-author-78c700cb9e03-uniform-family-spacelike-reference-collar: mathematical-premise
  lem-author-78c700cb9e03-complete-hawking-reference-product: mathematical-premise
  math:def-riemannian-gradient: mathematical-premise
  math:def-domain-and-exponential-map-of-a-connection: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp.16–17, Lemma 3.3 and proof; following use in Lemma 3.4
      reading_limits: Read the frozen extracted article at the full Lemma 3.3
        statement/proof and the next lemma’s flow composition. This ordinary
        reference attributes the item and does not serve as an independent
        prerequisite. The local Taylor argument is retained; the all-time
        stationary-saturation bridge is authored explicitly in the helpers
        rather than claimed present in the article.
physical_scope: Conditional local and stationary-collar geometry of the smooth
  stationary vacuum model and its Harrison family, q in [0,1]. The all-time
  extension is confined to an explicitly constructed stationary saturation of a
  near-horizon collar; no global smooth rigidity theorem or observation is
  asserted.
dependency_level: 10
---

## Statement

In the standing regular stationary vacuum construction, with $T|_S\not\equiv0$, maximal original exterior section and mass one, let $g_q$, $q\in[0,1]$, be the smooth Harrison family and let $K=T+\Omega_HZ$ be the fixed local Hawking field. There is a fixed neighborhood $V$ of $S$ in the original section $\Sigma_1$ that is spacelike for every $g_q$. Write $\bar h_q=g_q|_{T\Sigma_1}$ on this collar, let $\bar n_q$ be its future unit normal, let $\rho_q$ be its induced-metric distance to $S$ in the collar, and let $\bar\nu_q=\nabla^{\bar h_q}\rho_q$ be the normal pointing into the exterior. The metrics, normals and boundary normal exponential maps are smooth in $q$ with uniform bounds of every fixed finite order on a fixed smaller compact collar.

On $S$, $K=0$ and $\nabla^{(q)}_{\bar\nu_q}K=\kappa\bar n_q$ for the same fixed $\kappa>0$. Uniformly as $\rho_q\downarrow0$, $K=\kappa\rho_q\bar n_q+O(\rho_q^2)$ and $g_q(K,K)=-\kappa^2\rho_q^2+O(\rho_q^3)$. Thus $K$ is future timelike on $V\setminus S$ for every $q\in[0,1]$.

There is an open $T$-saturated collar $D_0$ in the original exterior on which the local fields $K,Z$ extend, agreeing with their original germs, to complete commuting Killing fields of every $g_q$. With this extension understood, $\phi_s^K(x)$ exists for every $s\in\mathbb R$ and $x\in V\setminus S$, and $(s,x)\mapsto\phi_s^K(x)$ is a diffeomorphism from $\mathbb R\times(V\setminus S)$ onto its image (one may take that image to be $D_0$). This establishes precisely the all-time collar flow; it asserts no extension of the local rigidity fields over the whole exterior.

The original-section maximality premise is imposed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$ for the original metric $g$, so $H_g|_C=0$. Where this result uses the original reference section $\Sigma_1$, it denotes the closure $B=C\cup S$ of this actual section. Maximality of a separately labelled chart-side region or another supplied section is not substituted for this premise. The spherical identification and the physical stationary end chart remain independent. [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-harrison-normalization]]

[[math:def-axiom-of-choice]]

[[pthm-original-lapse-and-product]]

[[pthm-local-hawking-circle-fields]]

[[def-circle-action-and-invariant-normal-data]]

[[lem-killing-normal-boost-and-invariant-tensors]]

[[pthm-harrison-denominator-positive]]

[[pthm-horizon-invariant-one-form]]

[[def-harrison-one-form-family]]

[[pthm-harrison-lorentzian-algebra]]

[[pthm-bifurcate-horizon-preservation]]

[[def-stationary-lorentzian-data]]

[[def-bifurcate-killing-horizon-data]]

[[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]]

[[lem-author-78c700cb9e03-bounded-rapidity-reference-graph]]

[[lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow]]

[[lem-author-78c700cb9e03-uniform-family-spacelike-reference-collar]]

[[lem-author-78c700cb9e03-complete-hawking-reference-product]]

[[math:def-riemannian-gradient]]

[[math:def-domain-and-exponential-map-of-a-connection]]

## Facts & Assumptions

[A1] Adopt the stationary vacuum model and regular data, with the stated maximal outer section and mass-one normalization. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]] [[def-harrison-normalization]] [[math:def-axiom-of-choice]]

[F1] Under the assumed maximality of the actual section $C=\Sigma_0\cap\mathcal E$, the original lapse/product theorem supplies the complete stationary-flow diffeomorphism $\mathbb R\times C\to\mathcal E$ and positive original lapse on $C$. Its closure $B=C\cup S$ admits an adapted spherical identification with $\{|y|\ge1\}$; neither the specified chart-side coordinate nor the independent physical end radius is identified with that adapted coordinate. Here $\Sigma_1=B$ is the original reference section, as stipulated in the Statement. [[pthm-original-lapse-and-product]]

[F2] The local Hawking/circle fields satisfy $K=T+\Omega_HZ$, vanish/tangent as specified, have common constant positive boost rate, and the periodic action preserves future orientation. [[pthm-local-hawking-circle-fields]] [[def-circle-action-and-invariant-normal-data]] [[lem-killing-normal-boost-and-invariant-tensors]]

[F3] The denominator and invariant primitive give a smooth family through $S$; its metrics are Lorentzian and stationary on the exterior, $g_1=g$, and are $K$-invariant locally. The bifurcation sphere is spacelike for every $g_q$ and the fixed quotient boost rate is preserved. [[pthm-harrison-denominator-positive]] [[pthm-horizon-invariant-one-form]] [[def-harrison-one-form-family]] [[pthm-harrison-lorentzian-algebra]] [[pthm-bifurcate-horizon-preservation]]

[F4] Lorentzian, Killing-horizon and induced-section terminology use the named definitions. [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]] [[def-spacelike-maximal-hypersurface-data]]

[F5] The invariant-normal-coordinate helper supplies a circle-invariant future/outward orthonormal normal frame, its normal exponential tube, and the exact boost/circle formulas in the outward wedge. [[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]]

[F6] The bounded-rapidity graph helper applies to a smooth spacelike section whose exterior-pointing normal to $S$ has positive spatial component in that frame; it permits a timelike component and requires no circle invariance of the section. With positive original stationary lapse and future-timelike $K$, it gives a smooth bounded graph, the strict crossing inequality and the unique formal stationary root. [[lem-author-78c700cb9e03-bounded-rapidity-reference-graph]]

[F7] The stationary-saturation helper extends the exact local boost/circle model and its bounded reference graph using the complete original stationary product, when the metric family is stationary and the local fields are Killing for every member. [[lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow]]

[F8] The uniform-family collar helper gives common spacelike collars, normal coordinates and signed Taylor expansions for a smooth compact Lorentz metric family with a smooth future field, fixed quotient boost rate, positive original outward boost and positivity of the section tangent form at $S$. [[lem-author-78c700cb9e03-uniform-family-spacelike-reference-collar]]

[F9] The complete reference-product helper gives the all-time $K$-flow diffeomorphism from the original reference graph onto the stationary collar, and its comparison with the original Cauchy section. [[lem-author-78c700cb9e03-complete-hawking-reference-product]]

## Proof

**Given:**The stated data and complete hypotheses.

**Goal:** Establish the conclusions on the domains and parameter ranges specified.

1.1 Extend the original section smoothly through $S$ as already provided by its smooth embedding; maximality of this extension is not needed. At $S$, $T\in TS$, so the invertible Harrison tangent map $A_q$ preserves $T\Sigma_1$. Its restriction there is invertible. The formula $g_q=(D_q/4)A_q^*g$ from [F3] therefore makes the section tangent form positive definite at $S$ for every $q$. The uniform-family lemma in [F8] applies: the zero field makes $\nabla^{(q)}K$ connection independent at $S$, while [F2]–[F3] fix its quotient eigenvalues. It supplies one common spacelike collar, smooth uniformly controlled induced normal data, the positive boost derivative, both uniform Taylor expansions and future timelikeness. [A1, F2, F3, F4, F8]

2.1 Use the original metric and [F5] to obtain the invariant frame $(e_0,e_1)$ and the exact local boost/circle coordinates, with the exterior as the outward wedge. The original section is smooth through $S$. Its original exterior-pointing unit normal $\bar\nu_1$ to $S$ is orthogonal to $TS$, hence has the form $\bar\nu_1=\beta e_0+\alpha e_1$. The outward orientation of this frame is the one toward the actual exterior $C$ in [F1]–[F2], so $\alpha>0$; unit spacelike length gives $\alpha^2-\beta^2=1$. Thus the side hypothesis of [F6] holds, allowing the tilt $\beta\ne0$. The positive original stationary lapse in [F1] gives future transversality of $T$, and step 1.1 gives future-timelike $K$. Apply [F6] to obtain a smooth graph $\tau=a(r,y)$ with $|a|\le A$, $1+\Omega_H Z_Sa>0$, and the unique formal stationary root. No preservation of the original section by the circle action is assumed. Shrink the common collar once to fit these constructions. [F1, F2, F4, F5, F6, step 1.1]

3.1 The coefficient $\Omega_H$ is nonzero: otherwise $T=K$ would vanish identically on $S$, contrary to [A1]. Since each $g_q$ is stationary and locally $K$-invariant, $\mathcal L_Zg_q=\Omega_H^{-1}(\mathcal L_Kg_q-\mathcal L_Tg_q)=0$ in the common local tube. Thus every hypothesis of the stationary-saturation helper [F7] is met by the original complete product and the bounded reference graph. It explicitly constructs $D_0$ and the same-field all-time extension by transporting unique local graph crossings through the complete $T$ product. This step supplies the missing completeness; it is not inferred merely from timelikeness or a local Taylor estimate. [A1, F1, F2, F3, F7, step 2.1]

4.1 Apply the complete reference-product helper in [F9]. In its global model $K=\partial_\tau$ and the map is $(s,r,y)\mapsto(r,a(r,y)+s,y)$ with the displayed smooth global inverse. It gives the required all-real-time diffeomorphism and identifies its image as the stationary collar saturation. Its comparison with the original Cauchy section is legitimate because the original stationary time diverges at both ends of each orbit. Only original-metric Cauchy data enter that comparison. All uniform estimates remain the local compact-collar bounds proved in step 1.1; no uniform control at unbounded flow times is claimed. [F1, F9, step 1.1, step 3.1] ∎

## Source notes

These premises specify the generated conditional scope and are not attributed to the original article. The substantive local horizon conclusions are retained. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

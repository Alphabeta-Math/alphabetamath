---
id: pthm-axisymmetric-vacuum-uniqueness-input
title: Connected smooth axisymmetric vacuum Kerr classification
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data
  - lem-author-64ac0bd1fcc4-commuting-global-symmetry-action
  - lem-author-64ac0bd1fcc4-orbit-gram-determinant
  - lem-author-64ac0bd1fcc4-orthogonal-orbit-projection
  - lem-author-64ac0bd1fcc4-orbit-metric-reconstruction
  - def-stationary-lorentzian-data
  - def-black-hole-comparison-hypothesis-data
  - def-causal-exterior-and-boundary-data
  - physics:post-gr-einstein-field-law
  - physics:def-gr-fx-kerr-exterior
  - math:def-axiom-of-choice
dependency_roles:
  def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data: mathematical-premise
  lem-author-64ac0bd1fcc4-commuting-global-symmetry-action: mathematical-premise
  lem-author-64ac0bd1fcc4-orbit-gram-determinant: mathematical-premise
  lem-author-64ac0bd1fcc4-orthogonal-orbit-projection: mathematical-premise
  lem-author-64ac0bd1fcc4-orbit-metric-reconstruction: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-black-hole-comparison-hypothesis-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:post-gr-einstein-field-law: physical-assumption
  physics:def-gr-fx-kerr-exterior: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: literature-derived
external_input: true
sources:
  references:
    - title: "P. T. Chruściel, J. L. Costa and M. Heusler, Stationary Black Holes:
        Uniqueness and Beyond"
      url: https://arxiv.org/pdf/1205.6112
      locator: §2.1, (2.1)–(2.3), PDF p. 5; §§2.3–2.4, (2.11)–(2.12), pp. 5–6; §2.6,
        Definition 2.1, p. 11; §§3.2.1, 3.2.3–3.2.7, pp. 13–15, especially
        Theorem 3.2 on p. 15; §3.3.1, p. 16.
      statement: "Theorem 3.2 classifies a stationary axisymmetric asymptotically flat
        I-plus-regular electrovacuum four-dimensional spacetime: its entire
        domain of outer communications is isometric to a Weinstein solution;
        when its event horizon is connected, it is the domain of outer
        communications of Kerr–Newman. The vacuum case is the Kerr
        classification described in §3.2.4. §3.3.1 explicitly states that
        Theorem 3.2 requires no analyticity; its hypotheses already include
        axisymmetry."
      hypotheses: Smooth four-dimensional stationary axisymmetric asymptotically flat
        I-plus-regular spacetime in the source definitions; electrovacuum,
        specialized here to vacuum (zero Maxwell field), and connected event
        horizon. The supplied stationary and axial actions are global and
        commute, with regular axis. Mean-nondegeneracy is retained from the
        assigned scope but is not needed by Theorem 3.2. No local-to-global
        extension of a Killing field is inferred.
      reading_limits: In this adjudication read the web PDF text at the cited end,
        stationarity, exterior and regularity definitions, §3.2.1, the end of
        §3.2.3, §§3.2.4–3.2.7 and §3.3.1. Checked the theorem hypotheses against
        the existing global comparison and black-hole comparison definitions. No
        visual inspection, reconstruction of the global classification proof, or
        reading credit for earlier rounds is claimed. Orbit-space topology,
        harmonic-map boundary estimates and reconstruction remain imported. No
        mean-to-pointwise nondegeneracy implication is used.
    - title: J. Sbierski, Characterisation of the Energy of Gaussian Beams on
        Lorentzian Manifolds — with Applications to Black Hole Spacetimes,
        arXiv:1311.2477 (12 January 2016 text)
      url: https://arxiv.org/pdf/1311.2477
      locator: §3.2 opening, printed/PDF p. 34; §3.2.1 opening through the coordinate
        introduction, printed/PDF p. 35.
      statement: For m>0 and 0≤a≤m the Kerr exterior manifold is R × (m+sqrt(m²−a²),
        infinity) × S². The opening of §3.2.1 identifies this exterior as the
        domain of outer communications for subextremal and extremal Kerr.
      hypotheses: Exact Kerr family; m>0, 0≤a≤m. The signed-a convention in this item
        also allows reversal of the azimuthal coordinate. Only the open exterior
        is used, not its horizon boundary or an arbitrary extension.
      reading_limits: Read web PDF text at the opening of §3.2 on p. 34 and the
        opening of §3.2.1 through the ingoing-coordinate discussion on p. 35.
        Used its exterior manifold, parameter range and explicit
        domain-of-outer-communications identification. Metric signs below follow
        the existing Kerr tensor convention and Aretakis §2.1. No geodesic,
        trapping, wave or maximal-extension proof is imported or reconstructed.
    - title: S. Aretakis, Decay of Axisymmetric Solutions of the Wave Equation on
        Extreme Kerr Backgrounds, arXiv:1110.2006 (10 October 2011)
      url: https://arxiv.org/pdf/1110.2006
      locator: §2.1, metric components and equation (2), printed/PDF p. 7; §2.2,
        differential structure, regular Lorentzian metric and D={r>M},
        printed/PDF p. 8.
      statement: The Boyer–Lindquist Kerr components use Δ=r²−2Mr+a² and ρ²=r²+a²
        cos²θ. Section 2.2 supplies the smooth spherical differential structure
        and regular Lorentzian extension for |a|≤M; in the extremal case |a|=M
        it identifies D={r>M} as the domain of outer communications, covered by
        Boyer–Lindquist coordinates.
      hypotheses: Exact Kerr metric with positive mass M, specialized to |a|=M for the
        domain-of-outer-communications assertion. Spherical polar coordinates
        have their usual polar degeneracy; the geometry is on S², including the
        axis. Its wave-equation axisymmetry assumption is not a restriction on
        the background metric definition.
      reading_limits: Read web PDF text of §§2.1–2.2 on pp. 7–8, including the
        Boyer–Lindquist components, coordinate change, regular Lorentzian
        assertion and extremal exterior identification. No wave estimates or
        classification theorem from this paper is invoked; no local proof of its
        extension or causal characterization was reconstructed. The global
        sphere-tensor notation is inherited from the declared mathematical Kerr
        supplier.
physical_scope: Conditional four-dimensional smooth classical vacuum Einstein
  model with zero cosmological constant; no measurement or dynamical settling
  claim.
dependency_level: 10
---

## Statement

In the four-dimensional classical vacuum Einstein model with zero cosmological constant, assume the smooth global stationary-axisymmetric comparison data: a selected asymptotically flat end, complete stationary flow, global commuting axial circle action with regular axis, exact $I^+$-regularity and connected event horizon. These are the predicates of the supplied global axisymmetric comparison-data definition and black-hole comparison-hypothesis definition. Retain the mean-nondegeneracy hypothesis in the supplied Gaussian-null sense of the former definition. No additional orbit-space hypothesis is imposed beyond this explicit package. Work in ZFC, including choice. The model equation is $\operatorname{Ric}(g)=0$, the vacuum specialization of the adopted Einstein field law. Metric and causal notation use the stationary Lorentzian and causal-exterior interfaces.

The Kerr comparison object means the following full black-hole exterior family, including the extremal case. For $m>0$ and $|a|\le m$, set $r_+=m+\sqrt{m^2-a^2}$ and $D_{m,a}=\mathbb R_t\times(r_+,\infty)_r\times S^2$, with its product smooth structure. Use the round sphere metric $\gamma$, the rotation-dual one-form $\lambda$ and the height function $\zeta$, pulled back to this product, in the declared Kerr tensor convention; thus away from the poles $\gamma=d\theta^2+\sin^2\theta\,d\phi^2$, $\lambda=\sin^2\theta\,d\phi$ and $\zeta=\cos\theta$. Put $\Sigma=r^2+a^2\zeta^2$ and $\Delta=r^2-2mr+a^2$. The comparison metric is the globally smooth sphere-tensor expression

$$g_{m,a}=-\left(1-\frac{2mr}{\Sigma}\right)dt\otimes dt+\frac{\Sigma}{\Delta}\,dr\otimes dr+\Sigma\gamma+\frac{a^2(\Sigma+2mr)}{\Sigma}\,\lambda\otimes\lambda-\frac{2amr}{\Sigma}\left(dt\otimes\lambda+\lambda\otimes dt\right).$$

The independent Kerr geometry inputs identify $(D_{m,a},g_{m,a})$ as the open domain of outer communications relative to its selected asymptotically flat end, including $|a|=m$, when $r_+=m$ and $\Delta=(r-m)^2$. The rotation axis is included through $S^2$; the event-horizon boundary $r=r_+$ is excluded. For $|a|<m$ this agrees with the supplied subextremal Kerr tensor datum. Reversal of azimuth gives the equivalent convention with $a$ replaced by $-a$.

Then for some such $m,a$ there exists a diffeomorphism $F:D\to D_{m,a}$ with $F^*g_{m,a}=g|_D$. Thus the entire domain of outer communications $D$ is isometric to the domain of outer communications of a Kerr spacetime. The conclusion concerns the whole exterior, not just an Ernst potential or a neighborhood of the horizon, and does not classify arbitrary extensions beyond it.

No independent analyticity assumption is required for this axisymmetric comparison. Axisymmetry is already a global hypothesis; extending a locally constructed axial Killing field to all of $D$ is a separate obligation. The smooth classification source does not require mean-nondegeneracy, so this application retains that hypothesis without inferring pointwise nondegeneracy from it.

## Statement references

[[def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data]]

[[def-stationary-lorentzian-data]]

[[def-black-hole-comparison-hypothesis-data]]

[[def-causal-exterior-and-boundary-data]]

[[physics:post-gr-einstein-field-law]]

[[physics:def-gr-fx-kerr-exterior]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

[A1] The adopted vacuum field equation is the zero-matter, zero-cosmological-constant specialization of the Einstein field law. [[physics:post-gr-einstein-field-law]]

[F1] Global end, causal, symmetry and regularity data use the exact named interfaces, with inherited ZFC conventions. The source's definition of $I^+$-regularity is retained in full. The global comparison-data definition supplies the meaning of a full-exterior isometry by diffeomorphism and metric pullback. [[def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data]] [[def-stationary-lorentzian-data]] [[def-black-hole-comparison-hypothesis-data]] [[def-causal-exterior-and-boundary-data]] [[math:def-axiom-of-choice]]

[F2] The commuting global flows give an action of $\mathbb R\times S^1$; this is not obtained by continuing a merely local field. [[lem-author-64ac0bd1fcc4-commuting-global-symmetry-action]]

[F3] The signed Gram determinant, conditional orthogonal projection and algebraic metric reconstruction have the explicit local identities in the named suppliers. They introduce the objects relevant to orbit-space reduction without purporting to prove its global topology or boundary regularity. [[lem-author-64ac0bd1fcc4-orbit-gram-determinant]] [[lem-author-64ac0bd1fcc4-orthogonal-orbit-projection]] [[lem-author-64ac0bd1fcc4-orbit-metric-reconstruction]]

[F4] The published mathematical Kerr interface supplies the sphere-tensor notation and subextremal metric convention. In the notation there, $\lambda=\xi^\flat$ and its mass parameter is denoted here by $m$. Its subextremal restriction is preserved; it is not used to assert an extremal exterior or a domain-of-outer-communications property. Those full-family geometry inputs are imported separately below. [[physics:def-gr-fx-kerr-exterior]]

## External input

Import the vacuum specialization of Chruściel–Costa–Heusler Theorem 3.2, read with §3.2.4's vacuum Kerr case. Theorem 3.2 gives an isometry of the full domain of outer communications; its electrovacuum conclusion is Kerr–Newman for a connected horizon, and the vacuum specialization is Kerr. Section 3.3.1 expressly distinguishes this theorem, requiring no analyticity, from the rigidity step that derives axisymmetry. Its explicit hypotheses are stationarity, axisymmetry, asymptotic flatness, $I^+$-regularity, dimension four and the electrovacuum equations, specialized here to vacuum; connectedness gives the Kerr conclusion. No unnamed additional orbit-space assumption is retained. Global orbit-space control, harmonic-map uniqueness and reconstruction are parts of this imported classification, not consequences proved by the elementary local suppliers.

Import the Kerr exterior manifold and its identification as the domain of outer communications for both subextremal and extremal parameters from Sbierski §3.2 and the opening of §3.2.1. His convention $0\le a\le m$, $m>0$, covers both regimes; reversing azimuth gives the negative-$a$ convention. This input identifies the full product exterior, including the sphere axis and excluding the horizon boundary; it is not merely a metric formula on a pole-free patch.

Import the metric coefficients and smooth spherical extension from Aretakis §§2.1–2.2, with the existing supplier's sphere-tensor notation. Section 2.1 fixes the Boyer–Lindquist coefficients in the $(-,+,+,+)$ convention; §2.2 supplies the regular Lorentzian metric and explicitly identifies the extremal domain of outer communications as $r>m$. Thus extremality is included without extrapolating the published subextremal interface's hypotheses. The whole-exterior classification and these comparison-family geometry facts are external established inputs; no local proof of them is claimed.

Chruściel–Costa 0806.0016 Theorem 1.3 is not invoked as a smooth theorem, and its Corollary 6.3 alone is not treated as a full metric classification. The five local intermediate items define the exact global hypothesis package and the elementary action, orbit and reconstruction algebra. They do not reconstruct the imported global classification proof or assert a mean-to-pointwise nondegeneracy bridge. Exact source hypotheses and actual reading limits appear in the references.

---
id: lem-author-ae62588ad46a-positive-area-nonzero-angular-momentum
title: Positive smooth horizon area and the exact degenerate angular-momentum test
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-black-hole-comparison-hypothesis-data
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-axiom-of-choice
  - math:def-countable-choice
  - math:def-riemannian-volume-density
  - math:lem-the-riemannian-volume-density-is-coordinate-independent
  - math:def-riemannian-volume-of-a-compactly-supported-smooth-density
  - math:thm-density-integration-is-defined-without-an-orientation
  - physics:def-gr-curvature-tensor-and-derived-tensors
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - physics:lem-emg-lorentz-hodge-calculus
  - math:prop-integration-over-an-oriented-embedded-submanifold
dependency_roles:
  def-black-hole-comparison-hypothesis-data: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-riemannian-volume-density: mathematical-premise
  math:lem-the-riemannian-volume-density-is-coordinate-independent: mathematical-premise
  math:def-riemannian-volume-of-a-compactly-supported-smooth-density: mathematical-premise
  math:thm-density-integration-is-defined-without-an-orientation: mathematical-premise
  physics:def-gr-curvature-tensor-and-derived-tensors: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  physics:lem-emg-lorentz-hodge-calculus: mathematical-premise
  math:prop-integration-over-an-oriented-embedded-submanifold: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: H. S. Reall, Black Holes, Part III lecture notes, 15 March 2024
      url: https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf
      locator: Conventions, printed p.1; section 8.2, equation (8.25), printed p.109
        (PDF page 110).
      statement: In units G=c=1, Komar angular momentum at an axisymmetric
        asymptotically flat end is (16 pi)^(-1) times the large-sphere limit of
        the integral of star d(m-flat), where m generates axial rotations.
      hypotheses: The cited definition assumes an axisymmetric asymptotically flat end
        and an existing limit. Only its integrand and numerical normalization
        are adopted here; the finite-section functional is defined locally, with
        a specified 2 pi axial generator and orientations. No asymptotic or
        horizon-transport equality is imported.
      reading_limits: Read browser-extracted PDF text at Conventions and section 8.2
        through (8.25). No visual inspection, convergence proof, conservation
        theorem or area equality was checked or imported.
dependency_level: 5
---

## Statement

Work in ZFC. Let $S$ be a nonempty compact smooth spacelike horizon cross-section, let $h$ be its induced Riemannian metric, and define its intrinsic area by $A:=\int_S\mu_h$, where $\mu_h$ is the Riemannian volume density. Then $0<A<\infty$. For any supplied real scalar $J$, the equality $A=8\pi|J|$ implies $J\ne0$. In the degenerate stationary axisymmetric vacuum application, vacuum means $\operatorname{Ric}(g)=0$ near the section. Supply the axial generator $Z$ with angle parameter of period $2\pi$, an ambient orientation and an orientation of $S$. In geometric units $G=c=1$, the component charge is the finite-section Komar functional $J_S:=(16\pi)^{-1}\int_S j^*(\star_g dZ^\flat)$, where $j:S\hookrightarrow M$ is inclusion and $Z^\flat=g(Z,\cdot)$; take $J=J_S$ in the assumed equality. These application data do not restrict the arbitrary-scalar implication. This is a componentwise test: it does not require the total angular momentum of all components to be nonzero and puts no condition on nondegenerate components.

## Facts & Assumptions

[A1] Work in ZFC with [[math:def-axiom-of-choice]]. In particular [[math:def-countable-choice]] holds: apply choice to the family of nonempty sets in a sequence and compose the choice function with that sequence. Countable choice is the inherited hypothesis of the chart-partition integration in [F2] and [F3].

[F1] Horizon, stationarity, axisymmetry and degeneracy terminology is that of [[def-black-hole-comparison-hypothesis-data]]. Smoothness, compactness, nonemptiness and spacelikeness of the two-dimensional cross-section $S$ are explicit hypotheses here. Its smooth induced positive-definite tensor $h$ is a Riemannian metric in [[math:def-riemannian-metric-and-riemannian-manifold]].

[F2] The density [[math:def-riemannian-volume-density]] is $\mu_h=\sqrt{\det(h_{ab})}\,|dx^1dx^2|$ in a surface chart. By [[math:lem-the-riemannian-volume-density-is-coordinate-independent]] these formulas glue to a positive smooth density independent of the chart.

[F3] Use [[math:def-riemannian-volume-of-a-compactly-supported-smooth-density]] with $f\equiv1$ on the compact surface to define $A=\int_S\mu_h$. Under [A1], [[math:thm-density-integration-is-defined-without-an-orientation]] makes this integral independent of charts and partition, nonnegative, and strictly positive for every nonzero nonnegative smooth density. The compact-support construction is a finite sum of finite chart integrals and requires no orientation.

[F4] For the second assertion, the extra data are a specified real scalar $J$ attached to this component and the assumed equality $A=8\pi|J|$, with $A$ defined in [F3]. In the intended degenerate stationary axisymmetric vacuum application, take the charge $J_S$ defined in [F5] for this same section, with the equality in that normalization supplied independently. The lemma uses only this scalar-data contract and the equality; the area–angular-momentum relation remains a premise.

[F5] For the application terminology, vacuum is the geometric predicate $\operatorname{Ric}(g)=0$ near $S$, with the Ricci tensor of [[physics:def-gr-curvature-tensor-and-derived-tensors]]. Use the chosen $2\pi$ axial generator $Z$ of [[def-black-hole-comparison-hypothesis-data]]. Specify an orientation of its Lorentzian neighborhood and an orientation of $S$ for this charge. Metric duality [[physics:def-gr-inverse-metric-and-musical-isomorphisms]] gives $Z^\flat=g(Z,\cdot)$, and [[physics:lem-emg-lorentz-hodge-calculus]] gives the smooth two-form $\star_g dZ^\flat$. With inclusion $j:S\hookrightarrow M$, define $J_S:=(16\pi)^{-1}\int_S j^*(\star_g dZ^\flat)$ using [[math:prop-integration-over-an-oriented-embedded-submanifold]]. Reall (8.25) fixes the integrand and factor in units $G=c=1$; the finite-section functional is defined here. Its orientations and axial scale are supplied data. No equality to a charge at infinity, independence of cross-section, or derivation of the area relation is asserted by this definition.

## Proof

**Given:** A nonempty compact smooth spacelike cross-section with its induced positive metric, [A1] and [F1]–[F3]; for the second assertion also the real component charge and equality in [F4]; for the geometric application, additionally the data in [F5].

**Goal:** Verify intrinsic finite positive area and the exact componentwise nonvanishing consequence.

1.1 By [F1] and [F2], $\mu_h$ is a positive smooth density on the nonempty surface, hence is nonzero. Compactness makes its support compact, and $f\equiv1$ is smooth with compact support. Thus the integral construction in [F3] applies under [A1] and gives a finite real value $A$: only finitely many partition-weighted, compactly supported chart coefficients contribute, each with finite integral. Strict positivity in [F3] applies to the nonzero positive density, so $0<A<\infty$. Choice is used only through the inherited chart-partition construction. [given, A1, F1, F2, F3]

1.2 For the application data in [F5], the Ricci tensor is defined on the specified smooth Lorentzian neighborhood, so its vanishing is a definite predicate. The specified smooth axial field has a smooth metric dual, exterior derivative and Hodge dual. Pullback gives a smooth real top form on oriented $S$; its support is compact because $S$ is compact. The submanifold integration supplier therefore gives a finite real $J_S$. Thus the application supplies a scalar of the type required by [F4], without a physical postulate or a conservation assertion. [given, F1, F5]

2.1 If $J=0$, the supplied equality in [F4] gives $A=8\pi|0|=0$, contradicting step 1.1. Therefore $J\ne0$. Apply this implication separately to each degenerate component for which the scalar charge and equality are supplied. It uses no sum of component charges and imposes no condition on a nondegenerate component. [given, F4, step 1.1, algebra] ∎

## External input

The cited Komar definition supplies the normalization recorded in the source contract. The finite-section functional in [F5] is a local definition using the declared mathematical suppliers; the proof establishes its finiteness. The area–angular-momentum equality remains an independently supplied premise.

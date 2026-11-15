---
id: pthm-stable-mots-area-charge-input
title: Stable MOTS area–charge inequality
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - def-author-97780c2fed82-general-spacelike-surface-data
  - lem-author-97780c2fed82-normal-deformation-families
  - lem-author-97780c2fed82-mots-variation-second-jet
  - lem-author-97780c2fed82-mots-boost-variation
  - def-author-97780c2fed82-spacetime-stably-outermost-data
  - physics:def-emg-pointwise-energy-conditions
  - math:def-countable-choice
  - physics:def-gr-metric-selected-connection
dependency_roles:
  def-author-97780c2fed82-general-spacelike-surface-data: mathematical-premise
  lem-author-97780c2fed82-normal-deformation-families: mathematical-premise
  lem-author-97780c2fed82-mots-variation-second-jet: mathematical-premise
  lem-author-97780c2fed82-mots-boost-variation: mathematical-premise
  def-author-97780c2fed82-spacetime-stably-outermost-data: mathematical-premise
  physics:def-emg-pointwise-energy-conditions: mathematical-premise
  math:def-countable-choice: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
provenance:
  statement: ai-altered
  proof: literature-derived
external_input: true
physical_scope: Conditional smooth four-dimensional classical Einstein–Maxwell
  model with nonnegative cosmological constant and non-electromagnetic matter
  satisfying DEC; charged matter is permitted. This is a conditional theorem,
  without observations or a claim of empirical model validity.
sources:
  references:
    - title: S. Dain, J. L. Jaramillo and M. Reiris, Area-charge inequality for black
        holes, arXiv:1109.5602v1
      url: https://arxiv.org/pdf/1109.5602v1
      locator: Theorem 2.1 and equations (1)–(4), PDF pp. 2–3; §3, equations
        (17)–(20), Definitions 3.1–3.2, PDF p. 7; Lemma 3.3 and equation (21),
        PDF p. 8; Lemma 3.4, equation (24), PDF p. 9; proof of Theorem 2.1,
        equations (30)–(34), PDF p. 10
      statement: For an orientable closed marginally outer trapped surface satisfying
        spacetime stably outermost stability, Einstein equation G+Lambda
        g=8pi(T_EM+tau), Lambda>=0 and DEC for tau imply A>=4pi(Q_E^2+Q_M^2),
        with charges normalized by (4pi)^-1 times the dual and ordinary Maxwell
        flux. The source stability is X=gamma ell-psi k with gamma>=0, psi>0,
        g(ell,k)=-1 and delta_X theta_(ell)>=0. Equation (31) also gives the
        integral bound on squared electric and magnetic normal components by
        4pi(1-genus) for a connected surface. No symmetry or source-free Maxwell
        hypothesis is imposed.
      hypotheses: Smooth oriented, time-oriented four-dimensional Lorentzian spacetime
        and smooth spacelike closed orientable MOTS with outgoing global null
        pair and the stated spacetime stability; nonnegative cosmological
        constant, standard Maxwell stress tensor and non-electromagnetic matter
        satisfying DEC. Connected surface is explicit when using its genus in
        (21), (23), (31); disconnected surfaces are treated componentwise, not
        by squaring the sum of all component charges.
      reading_limits: For this connection-interface repair, consulted the PDF text
        extraction of Theorem 2.1, equations (1)–(4), the comparison paragraphs
        on PDF p. 3, and §3 through the proof of Theorem 2.1, equations
        (17)–(34), PDF pp. 7–10. Screenshot requests for PDF pp. 7 and 10
        failed; no successful visual inspection is claimed. The opening
        paragraph of §3 explicitly fixes the Levi–Civita connection. Did not
        consult source references [2], [3], [7], reconstruct Gauss–Bonnet, or
        independently audit the source proof. The theorem and equation (31)
        remain explicit external inputs. The five existing local helpers supply
        the surface/deformation and slice interfaces under their stated
        Countable Choice assumption. Equations (1)–(2) specify the general
        Einstein–Maxwell matter assumption used here; they do not establish
        empirical validity or existence of a model.
dependency_level: 7
---

## Statement

Assume Countable Choice $\mathrm{AC}_\omega$ for the surface, flux and deformation constructions below. In the smooth four-dimensional classical Einstein–Maxwell model, adopt geometric units and explicitly assume the field equation $G_{ab}+\Lambda g_{ab}=8\pi(T^{\rm EM}_{ab}+\tau_{ab})$, where $\Lambda\ge0$ and $T^{\rm EM}_{ab}=(4\pi)^{-1}(F_{ac}F_b{}^c-\tfrac14g_{ab}F_{cd}F^{cd})$. Here $G=\operatorname{Ric}-\tfrac12R g$, with the metric-selected (torsion-free, metric-compatible) connection $\nabla^g$, and the smooth non-electromagnetic stress tensor $\tau$ satisfies the dominant energy condition: $-\tau^a{}_bv^b$ is future causal or zero for each future timelike $v$. Charged matter is allowed; source-free Maxwell equations, axial symmetry and asymptotic flatness are not assumptions of this result.

Let $S$ be a nonempty connected closed orientable spacelike two-surface with supplied future null normals $\ell,k$, $g(\ell,k)=-1$, and outgoing expansion $\theta_{(\ell)}=0$, using the general spacelike-surface data with its connection fixed to the same $\nabla^g$ used for $G$. Use this connection for the outgoing expansion and for all deformations and expansion variations below. Suppose it is spacetime stably outermost in the exact sense of the spacetime-stably-outermost definition: some smooth $\gamma\ge0$, $\psi>0$ give $X=\gamma\ell-\psi k$ with $\delta_X\theta_{(\ell)}\ge0$. The derivative is the general spacetime derivative supplied by the expansion-variation lemma, with boost invariance supplied by the boost-variation lemma; no containing spacelike slice is required. Then, with $A$, $e,b$ and the flux normalization of the general spacelike-surface data,

$$A\ge4\pi\bigl(Q_E(S)^2+Q_M(S)^2\bigr).$$

The stronger source bound retained for applications is $\int_S(e^2+b^2)\,d\mu_q\le4\pi(1-g_S)\le4\pi$, where $g_S$ is the genus of the connected orientable surface (the number of handles). If this integral is positive, $g_S=0$. For a disconnected closed surface apply these assertions to each connected component satisfying the hypotheses; in particular $A_{\rm total}\ge4\pi\sum_j(Q_{E,j}^2+Q_{M,j}^2)$. This does not assert a bound by the square of the sum of component charges.

For a surface lying in a spacelike section, a supplied smooth positive supersolution $f$ of its outward graph operator, $\mathcal Lf\ge0$, verifies the spacetime-stability hypothesis by the slice bridge in the spacetime-stably-outermost definition: $\ell=n+\nu$, $k=(n-\nu)/2$ and $X=f\nu=(f/2)\ell-fk$. Nonnegativity of a principal eigenvalue suffices only together with an applicable theorem furnishing its smooth positive eigenfunction. No such spectral theorem is silently assumed here.

## Statement references

[[def-author-97780c2fed82-general-spacelike-surface-data]]

[[lem-author-97780c2fed82-normal-deformation-families]]

[[lem-author-97780c2fed82-mots-variation-second-jet]]

[[lem-author-97780c2fed82-mots-boost-variation]]

[[def-author-97780c2fed82-spacetime-stably-outermost-data]]

[[math:def-countable-choice]]

[[physics:def-emg-pointwise-energy-conditions]]

[[physics:def-gr-metric-selected-connection]]

## Facts & Assumptions

[A1] Countable Choice is assumed to meet the hypotheses of the general surface, flux, spacetime-deformation and slice-bridge suppliers. [[math:def-countable-choice]]

[F1] Under Countable Choice, general surface, flux and null-normal data use the explicit codimension-two interface; smooth deformations and their derivatives are supplied by the local helper chain. [[def-author-97780c2fed82-general-spacelike-surface-data]] [[lem-author-97780c2fed82-normal-deformation-families]] [[lem-author-97780c2fed82-mots-variation-second-jet]] [[lem-author-97780c2fed82-mots-boost-variation]]

[F2] Spacetime stably outermost means exactly the quantified outgoing variation condition; the same interface supplies the explicit slice supersolution bridge. [[def-author-97780c2fed82-spacetime-stably-outermost-data]]

[F3] The displayed Einstein equation with electromagnetic stress plus general non-electromagnetic matter is an explicit physical model assumption, in the geometric normalization of Dain–Jaramillo–Reiris equations (1)–(2). The source permits charged non-electromagnetic matter satisfying DEC.

[F4] The dominant energy condition is the stated algebraic condition on the non-electromagnetic stress tensor. [[physics:def-emg-pointwise-energy-conditions]]

[F5] Dain–Jaramillo–Reiris Theorem 2.1 supplies the area–charge conclusion, and its proof equation (31) supplies the retained squared-density bound, under these exact hypotheses.

[F6] The metric-selected connection is the unique torsion-free, metric-compatible connection of $g$. The general surface and deformation interfaces are used with this same $\nabla^g$ for expansion and variation, as required by the Levi–Civita convention at the start of Dain–Jaramillo–Reiris §3. [[physics:def-gr-metric-selected-connection]]

## External input

The area–charge theorem and the stronger squared-density bound are imported from Dain–Jaramillo–Reiris Theorem 2.1 and equation (31), not claimed as locally reconstructed proofs. The surface expansion and its variation use the same Levi–Civita connection $\nabla^g$ as the curvature in the field equation, matching the opening convention of source §3. The source's null normals satisfy $g(\ell,k)=-1$, its MOTS condition is $\theta_{(\ell)}=0$, and its Definitions 3.1–3.2 require a positive stability weight in an outgoing non-timelike normal direction. The field equation has the sign $G+\Lambda g=8\pi(T^{\rm EM}+\tau)$ and the factor $1/(4\pi)$ in $T^{\rm EM}$. Under the explicitly assumed Countable Choice, the local helpers supply the general null variation and its exact relation to the slice graph derivative, so the import does not restrict the source's surface to a spacelike section. Connectedness is explicit for the genus and single-surface inequality; componentwise application preserves the valid disconnected scope. The field-law and energy hypotheses must be established in each application; this import neither establishes them nor proves spectral stability of a particular surface.

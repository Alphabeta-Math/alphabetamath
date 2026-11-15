---
id: thm-author-a8fd09e77ebd-kerr-local-deformation
title: Rotating Kerr admits local stationary vacuum deformations with an axial
  obstruction
kind: theorem
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - def-author-a8fd09e77ebd-relative-stationary-deformation
  - lem-author-a8fd09e77ebd-regular-kerr-analytic-chart
  - physics:def-gr-curvature-tensor-and-derived-tensors
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-author-a8fd09e77ebd-relative-stationary-deformation: mathematical-premise
  lem-author-a8fd09e77ebd-regular-kerr-analytic-chart: mathematical-premise
  physics:def-gr-curvature-tensor-and-derived-tensors: mathematical-premise
provenance:
  statement: ai-altered
  proof: literature-derived
sources:
  references:
    - title: Ionescu–Klainerman, On the local extension of Killing vector-fields in
        Ricci flat manifolds
      url: https://arxiv.org/pdf/1108.3575
      locator: §1 Theorem 1.3, printed/PDF p. 4; §3.2 pp. 19–20; proof of Theorem 1.3
        pp. 23–27, especially (3.39) and the horizon coordinates on p. 26
      statement: For rotating subextremal Kerr 0<a<m, every open U0 meeting the past
        horizon in the closure of the exterior contains a ball-like local
        neighborhood U and a smooth Ricci-flat deformation retaining T and
        agreeing with Kerr on the non-exterior side, for which the Kerr axial
        Killing field from the matching side has no global Killing extension
        commuting with T. The local construction may be taken in the off-axis
        horizon collar, with the matching interior side connected.
      hypotheses: E is the Kerr domain of outer communications; H− is the boundary of
        its white-hole region, and U0∩H−∩closure(E) is nonempty. The
        construction chooses an off-axis point away from the bifurcation sphere;
        U is diffeomorphic to the open four-ball. No global completeness,
        asymptotic flatness of the deformation, or bifurcation sphere in U is
        assumed.
      reading_limits: Read Theorem 1.3 p. 4, §3 opening setup pp. 14–15, regular
        coordinates (3.3)–(3.5), §3.2 domain and matching-side setup pp. 19–20,
        and the proof text pp. 23–27. In particular the obstruction is to
        extending the matching axial field, and the proof uses its values along
        the matching horizon collar; p. 26 straightens that horizon. The
        characteristic construction and its differential estimates are imported,
        not independently reconstructed or reviewed. No assertion of failure of
        Kerr isometry in every smaller germ is imported.
external_input: true
dependency_level: 2
---

## Statement

Let $g$ be rotating Kerr with $0<a<m$, stationary field $T$ and axial field $Z$. Write $E=I^-(M_{\mathrm{end}})\cap I^+(M_{\mathrm{end}})$ and $H^- =\partial I^+(M_{\mathrm{end}})$ using the conventions of [[def-causal-exterior-and-boundary-data]]. For any open $U_0$ meeting $H^-\cap\overline E$, the Ionescu–Klainerman construction supplies a smaller open neighborhood $U\subset U_0$, diffeomorphic to the open four-ball and meeting $H^-$, and a smooth Lorentzian metric $\widetilde g$ with

$$\operatorname{Ric}(\widetilde g)=0,\qquad \mathcal L_T\widetilde g=0,\qquad \widetilde g=g\ \hbox{on }U\setminus E.$$

The Kerr axial field from the matching side does not extend to a Killing field on all of $U$ commuting with $T$. In the local collar construction the matching interior open side $O$ is connected and nonempty, and this is nonextendibility of the prescribed axial field there. Thus $(U,O,g,\widetilde g,T,Z)$ gives the obstructed relative datum of [[def-author-a8fd09e77ebd-relative-stationary-deformation]]. Its regular off-axis Kerr coordinates are those of [[lem-author-a8fd09e77ebd-regular-kerr-analytic-chart]]. This is a local vacuum deformation, not a globally regular asymptotically flat stationary black-hole counterexample.

## Facts & Assumptions

[F1] Causal exterior and chronological-boundary notation use [[def-causal-exterior-and-boundary-data]].

[F2] The relative extension problem is the specified field on a connected Kerr-matching open side. [[def-author-a8fd09e77ebd-relative-stationary-deformation]]

[F3] The selected Kerr horizon chart is regular and analytic and carries commuting coordinate fields $T,Z$. [[lem-author-a8fd09e77ebd-regular-kerr-analytic-chart]]

[F4] The independent deformation theorem and its local collar construction provide the existence and nonextension assertions above.

[F5] The Ricci tensor in the vacuum equation is the contraction of the curvature of the metric-selected connection, as defined in clause (c) of [[physics:def-gr-curvature-tensor-and-derived-tensors]].

## External input

Theorem 1.3 supplies the smooth vacuum metric, retained stationary field and prohibited commuting axial extension. The construction in §3 takes a regular horizon collar off the axis and bifurcation sphere; §3.2 identifies the matching interior side, and the proof starting on p. 23 carries the prescribed axial data from that side into its contradiction. The straightened horizon coordinates on p. 26 permit the matching collar to be taken connected. The existence and nonextension inputs are imported, not locally reconstructed. The source quantifies over a neighborhood U0 and produces U; it does not claim that the resulting metric fails to be Kerr in every subneighborhood of the original point.

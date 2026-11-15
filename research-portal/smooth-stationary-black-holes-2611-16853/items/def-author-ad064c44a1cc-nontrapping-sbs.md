---
id: def-author-ad064c44a1cc-nontrapping-sbs
title: Event-horizon bifurcation data for the nontrapping theorem
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-author-ad064c44a1cc-nontrapping-gr
  - def-null-screen-expansion-and-focal-data
  - def-causal-exterior-and-boundary-data
  - physics:lem-gr-fx-null-normal-plane-and-screen
  - math:def-transverse-embedded-submanifolds
dependency_roles:
  def-author-ad064c44a1cc-nontrapping-gr: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:lem-gr-fx-null-normal-plane-and-screen: mathematical-premise
  math:def-transverse-embedded-submanifolds: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Alexandru F. Radu, On rigidity of stationary black holes under a
        nontrapping assumption
      url: https://arxiv.org/html/2609.23872v1
      locator: Version 1, section 1.1 SBS and its two following explanatory
        paragraphs; Theorem 1.1; section 1.2 opening paragraph.
      statement: In the source GR setting, SBS specifies that the event boundaries
        $\partial_M I_M^-(M^{\rm end})$ and $\partial_M I_M^+(M^{\rm end})$
        intersect at $S_0=\Phi_0(\{|x|=1\})$, and near this sphere are smooth
        transverse null hypersurfaces tangent to $T$ whose null second
        fundamental forms have zero induced-metric trace. SBS imposes no
        non-identically-zero condition on $T|_{S_0}$. Section 1.2 says the
        zero-field case is treated by staticity in section 7. The additional
        Killing symmetry is constructed, not assumed by SBS.
      hypotheses: This is a source-specific definition in the GR setting of a smooth
        oriented time-oriented stationary Ricci-flat four-manifold with the
        specified end, slice parametrization and exterior. Only the listed SBS
        predicates and the source treatment distinction are imported; no
        rigidity or staticity theorem is being proved or applied by this
        definition.
      reading_limits: Retrieved and read the indicated version-1 HTML section 1.1
        setup, GR, SBS, the two paragraphs after SBS, Theorem 1.1 and section
        1.2 opening paragraph. Used for formulation and source attribution only.
        Section 7 staticity and global symmetry-construction proofs were not
        reviewed or reconstructed.
    - title: "S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth
        stationary black holes in vacuum: small perturbations of the Kerr
        spaces"
      url: https://arxiv.org/html/0904.0982v1
      locator: Version 1, section 1.1, SBS paragraph, especially its final sentence
        (after equation (1.3) and before PK).
      statement: The SBS assumptions include tangency of $T$ to both local null
        event-boundary hypersurfaces and $T|_{S_0}\not\equiv0$.
      hypotheses: A clause of the source stationary vacuum GR/SBS setup, with its
        specified bifurcation sphere and local event-boundary sheets. This
        clause is reported for comparison only; neither PK nor the Main Theorem
        is imported.
      reading_limits: Retrieved the version-1 HTML and read section 1.1 setup, GR and
        the complete SBS paragraph including its final sentence and nonexpansion
        footnote. Checked only this assumption comparison; no smallness theorem
        or rigidity proof was reviewed.
    - title: S. Alexakis, A. D. Ionescu and S. Klainerman, Rigidity of stationary
        black holes with small angular momentum on the horizon
      url: https://arxiv.org/html/1304.0487v2
      locator: Version 2, section 1.1.2, SBS paragraph, final sentence immediately
        before section 1.1.3.
      statement: The SBS assumptions include tangency of $T$ to both local null
        event-boundary hypersurfaces and $T|_{S_0}\not\equiv0$.
      hypotheses: A clause of the source stationary vacuum GR/SBS setup, with its
        specified bifurcation sphere and local event-boundary sheets. This
        clause is reported for comparison only; the separate maximality and
        horizon-smallness assumptions are not imposed here.
      reading_limits: Retrieved the version-2 HTML and read section 1.1 main objects
        and regularity assumptions through the complete SBS paragraph and its
        final sentence. Checked only the rotating SBS comparison; no elliptic
        estimate, staticity or rigidity theorem proof was reviewed.
dependency_level: 3
---

## Definition

For the Radu NT GR package, its **SBS condition** is that the future and past event boundaries $\partial_M I_M^-(M^{\rm end})$ and $\partial_M I_M^+(M^{\rm end})$ meet in the embedded sphere $S_0=\Phi_0(\{r=1\})$. Near $S_0$ they are smooth transverse null hypersurfaces $H^+,H^-$ tangent to $T$, with vanishing null expansion. The expansion is the induced positive-metric trace of $(X,Y)\mapsto g(\nabla_XL,Y)$ for a null generator $L$ and section tangent fields $X,Y$.

Unlike the rotating SBS packages used in the two smallness papers, this source statement does not require $T|_{S_0}\not\equiv0$. Its main theorem includes the case $T|_{S_0}\equiv0$, addressed by staticity in its §7. These are event-boundary hypotheses; a second globally defined Killing field is a conclusion of the rigidity theorem, not part of SBS here.

## Facts & Assumptions

[F1] [[def-author-ad064c44a1cc-nontrapping-gr]] supplies the end and chosen sphere; [[def-causal-exterior-and-boundary-data]] fixes the ambient boundary convention. [[def-null-screen-expansion-and-focal-data]] supplies the intrinsic null-expansion trace and normalization qualifications.

[F2] [[physics:lem-gr-fx-null-normal-plane-and-screen]] defines a smooth null hypersurface by its rank-two positive semidefinite induced metric, its radical generator line and spacelike sections; it also supplies the null-form rescaling law. [[math:def-transverse-embedded-submanifolds]] defines transversality by $T_pH^++T_pH^-=T_pM$ at intersection points. Only these mathematical interfaces are used; the choice convention required by the null-geometry supplier is inherited from [[def-null-screen-expansion-and-focal-data]].

[F3] The Radu SBS passage and section 1.2 opening supply the exact source-specific horizon predicates and the stated treatment of $T|_{S_0}\equiv0$. The two rotating smallness packages compared here are the Alexakis–Ionescu–Klainerman perturbative paper, section 1.1 SBS, and their small-horizon-field paper, section 1.1.2 SBS; each explicitly requires $T|_{S_0}\not\equiv0$. Their complete source contracts are recorded in External input.

## Justification

The ambient chronological boundaries and their specified local smooth embeddings determine the two horizon pieces. Their tangent spaces and induced section metrics make the nullness, transversality, tangency and trace predicates well-defined. Rescaling a null generator multiplies its expansion, so the zero-expansion condition is unchanged. The absence of a nonzero-horizon-field clause is kept explicitly because the source handles that case separately; no external staticity proof is reconstructed in this definition.

## External input

Radu's section 1.1 SBS supplies the particular event-boundary assumptions, not just generic horizon terminology. Its section 1.2 opening attributes treatment of the identically-zero horizon field to staticity in section 7. This definition imports those formulation and attribution facts only; it does not apply or reconstruct the staticity or global rigidity proofs.

For the comparison with the rotating smallness papers, import only the non-identically-zero horizon-field clause from Alexakis–Ionescu–Klainerman, arXiv:0904.0982v1 section 1.1 SBS and arXiv:1304.0487v2 section 1.1.2 SBS. Their other hypotheses and conclusions are not added to the Radu SBS package.

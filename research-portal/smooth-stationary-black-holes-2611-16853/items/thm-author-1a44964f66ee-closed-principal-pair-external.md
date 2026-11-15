---
id: thm-author-1a44964f66ee-closed-principal-pair-external
title: Imported positive eigenpairs for a smooth closed elliptic operator
kind: theorem
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-1a44964f66ee-formal-adjoint
  - math:def-axiom-of-choice
dependency_roles:
  lem-author-1a44964f66ee-formal-adjoint: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: literature-derived
external_input: true
sources:
  references:
    - title: Lars Andersson, Marc Mars and Walter Simon, Stability of marginally outer
        trapped surfaces and existence of marginally outer trapped tubes
      url: https://arxiv.org/pdf/0704.2889
      locator: §4, equation (10), standing hypotheses and Lemma 4.1(i)–(ii), printed p.9
      statement: On a connected compact smooth manifold without boundary, a real
        smooth elliptic operator L=-Delta_h+2t^A D_A+c has a real eigenvalue
        with a smooth everywhere positive eigenfunction, unique up to scale,
        minimal real part among eigenvalues. Its L2 adjoint has the same
        principal eigenvalue, with a positive principal eigenfunction by
        applying (i) to the adjoint.
      hypotheses: Positive dimension; connected compact smooth manifold without
        boundary; smooth positive-definite Riemannian h and smooth real drift t
        and zeroth-order coefficient c; no sign hypothesis on c, no energy
        condition and no selfadjointness assumption. Adjoint is with respect to
        the Riemannian L2 measure.
      reading_limits: Downloaded the complete arXiv PDF; read §4 standing hypotheses
        and Lemma 4.1 on printed p.9 as text and rendered PDF, its surrounding
        explanation on p.10, and Appendix B pp.29–30 as extracted text. The
        existence theorem is imported, not locally reconstructed or
        proof-reviewed. Local helper arguments independently supply the quotient
        identities and adjoint pairing actually used here.
dependency_level: 1
---

## Statement

Let $L=-\Delta_h+2t\cdot\nabla+c$ have the closed connected smooth Riemannian and real smooth coefficient hypotheses of the formal-adjoint lemma. There exist a real eigenvalue $\lambda$, a smooth real $\phi>0$ with $L\phi=\lambda\phi$, and a smooth real $\chi>0$ with $L^\dagger\chi=\lambda\chi$. This is an established external existence input, not a locally reconstructed resolvent or Krein–Rutman proof.

## Facts & Assumptions

[F1] The formal-adjoint lemma fixes the exact operator, metric density and adjoint conventions. [[lem-author-1a44964f66ee-formal-adjoint]]

[A1] Work in ZFC, including Choice. [[math:def-axiom-of-choice]]

## External input

Andersson–Mars–Simon §4 Lemma 4.1 applies to the smooth real elliptic operator on the connected compact boundaryless manifold. Apply part (i) also to its formal adjoint, whose coefficients and ellipticity are supplied by the formal-adjoint lemma; part (ii) identifies the principal eigenvalues. We import the resulting positive right and adjoint eigenpairs. No local compact-resolvent construction or proof of Krein–Rutman is claimed.

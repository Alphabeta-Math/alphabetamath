---
id: lem-author-cea8e61dc3c6-vacuum-killing-divergence
title: Ricci contraction of the Killing derivative
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - lem-author-cea8e61dc3c6-killing-exact-two-form
  - physics:thm-gr-curvature-algebraic-symmetries
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  lem-author-cea8e61dc3c6-killing-exact-two-form: mathematical-premise
  physics:thm-gr-curvature-algebraic-symmetries: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: H. S. Reall, General Relativity, Part III Mathematical Tripos, October
        12, 2022
      url: https://www.damtp.cam.ac.uk/user/hsr1000/part3_gr_lectures.pdf
      locator: Conventions, printed p. 3 (PDF p. 4); §4.2, equations (4.7)–(4.8),
        printed p. 42 (PDF p. 43)
      statement: For a torsion-free connection,
        $(\nabla_c\nabla_d-\nabla_d\nabla_c)Z^a=R^a{}_{bcd}Z^b$. The Ricci
        contraction is $R_{ab}=R^c{}_{acb}$.
      hypotheses: A smooth torsion-free connection and a smooth vector field; the
        curvature convention is the one explicitly stated in the cited
        Conventions.
      reading_limits: Retrieved the PDF and read the Conventions and the §4.2 passage
        containing (4.7)–(4.8). Equation (4.8) is stated as an exercise with a
        hint; no complete source proof was read. The identity is explicitly
        imported here; dualization and its Killing-field application are
        authored locally. No full-text proof review is claimed.
dependency_level: 2
---

## Statement

For stationary Lorentzian data, the Killing two-form obeys $\nabla^aF_{ab}=-\operatorname{Ric}_{bd}T^d$. In particular, if $\operatorname{Ric}=0$, then $\nabla^aF_{ab}=0$. The curvature and Ricci signs are those of the stationary-data definition.

## Facts & Assumptions

[F1] The connection, index conventions, curvature and Ricci contraction are those of [[def-stationary-lorentzian-data]].

[F2] The Killing derivative is alternating. [[lem-author-cea8e61dc3c6-killing-exact-two-form]]

[F3] The curvature has the pair skew-symmetries, pair-exchange symmetry and symmetric Ricci contraction. [[physics:thm-gr-curvature-algebraic-symmetries]]

[F4] Import the vector Ricci commutator with the exact convention recorded in the External input; its source is Reall (4.7)–(4.8).

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove all asserted identities under these hypotheses.

1.1 Apply the commutator in [F4] to the scalar pairing $u_cZ^c$ and use the connection product rule. Scalar second derivatives commute by torsion freedom, so the covector formula is $[\nabla_a,\nabla_b]u_c=-R^d{}_{cab}u_d$. Contracting $u=T^\flat$ gives $g^{ac}[\nabla_a,\nabla_b]T_c=\operatorname{Ric}_{bd}T^d$: indeed $g^{ac}R_{ecab}=-g^{ac}R_{ceab}=-\operatorname{Ric}_{eb}$, using the first-pair skew-symmetry and the stated Ricci contraction. [F1, F3, F4, algebra]

2.1 Alternation gives $\nabla^aT_a=0$ and $\nabla^aF_{ab}=-\nabla^a\nabla_bT_a$. Metric compatibility and step 1.1 therefore yield $\nabla^aF_{ab}=-\nabla_b(\nabla^aT_a)-g^{ac}[\nabla_a,\nabla_b]T_c=-\operatorname{Ric}_{bd}T^d$. Under Ricci flatness the right side vanishes. [step 1.1, F1, F2, algebra] ∎

## External input

The vector identity $[\nabla_c,\nabla_d]Z^a=R^a{}_{bcd}Z^b$ and contraction $\operatorname{Ric}_{ab}=R^c{}_{acb}$ are the imported input from Reall (4.7)–(4.8). Its convention matches the stationary-data definition exactly. No sign of a curvature tensor from a different source is transferred implicitly.

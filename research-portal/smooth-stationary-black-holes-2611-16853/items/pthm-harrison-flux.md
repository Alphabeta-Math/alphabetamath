---
id: pthm-harrison-flux
title: "Proposition 2.1: electric and magnetic fluxes"
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - def-killing-ernst-notation
  - def-harrison-electromagnetic-form
  - def-harrison-one-form-family
  - def-source-free-geometric-electrovacuum-data
  - def-surface-area-flux-and-null-variation-data
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-lorentzian-data
  - def-stationary-asymptotic-decay-data
  - pthm-harrison-electrovacuum
  - pthm-global-harrison-one-form
  - pthm-ernst-and-one-form-decay
  - pthm-original-lapse-and-product
  - lem-author-ce4974f559ec-killing-end-flux
  - lem-author-ce4974f559ec-harrison-end-restriction
  - lem-author-ce4974f559ec-positive-parameter-charge
  - lem-author-ce4974f559ec-closed-flux-transfer
  - lem-author-ce4974f559ec-fixed-sphere-endpoints
  - math:def-axiom-of-choice
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  def-harrison-electromagnetic-form: mathematical-premise
  def-harrison-one-form-family: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  def-surface-area-flux-and-null-variation-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  pthm-harrison-electrovacuum: physical-result
  pthm-global-harrison-one-form: physical-result
  pthm-ernst-and-one-form-decay: physical-result
  pthm-original-lapse-and-product: physical-result
  lem-author-ce4974f559ec-killing-end-flux: mathematical-premise
  lem-author-ce4974f559ec-harrison-end-restriction: mathematical-premise
  lem-author-ce4974f559ec-positive-parameter-charge: mathematical-premise
  lem-author-ce4974f559ec-closed-flux-transfer: mathematical-premise
  lem-author-ce4974f559ec-fixed-sphere-endpoints: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional charge identities in the smooth stationary vacuum
  Harrison construction with the article mass-one end normalization; no
  measurement or spacetime-existence assertion.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p.9 Proposition 2.1 and (2.8), p.26 proof of Theorem4.2
      reading_limits: Inspected original PDF p.9 as a rendered image, and the proof on
        pp.26–27 during the preceding MOTS task; read the corresponding
        extracted passages. Attribution only; the original article is not used
        as a prerequisite proof.
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1#S3.SS3
      locator: §3.3 equations (3.28)–(3.31) and the fixed-sphere endpoint paragraph
        after (3.31)
      reading_limits: Read retained actual arXiv HTML text of §3.3, including the
        stronger angular-momentum expansion in (3.28), Hodge sign convention and
        fixed-sphere q=0 argument. This citation is methodological comparison
        only. Its Proposition3.1 global hypothesis package is not applied; the
        end-charge calculation is supplied locally under the article end bounds.
dependency_level: 10
---

## Statement

Assume the article's regular smooth stationary vacuum construction, with the original exterior section maximal, $T|_S\not\equiv0$, the mass-one stationary end normalization $g_{00}=-1+2/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$, and the single smooth stationary primitive $W_0$ furnished by its authored global construction. Use $W_q=(1-q)^2W_0-4q(1-q)T^\flat$ and the actual Harrison metric and electromagnetic form for $0\le q\le1$. Choose the spacetime orientation so that $dt\wedge dx^1\wedge dx^2\wedge dx^3$ is positive in the chosen stationary end chart. With the sphere orientation inherited from the outward asymptotic spheres,

$$(4\pi)^{-1}\int_S\star_{g_q}F_q=\sqrt{1-q^2},\qquad (4\pi)^{-1}\int_SF_q=0.$$

The same identities hold on every oriented sphere homologous to $S$ through the smooth regular region where the Maxwell equations hold. The star and electric charge use $g_q$, with the fixed spacetime orientation. These statements retain both endpoints and impose no specified leading angular-momentum coefficient on $g_{0i}$.

The original-section maximality used here is assumed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$, with the original metric $g$, so $H_g|_C=0$. The selected physical end retains its stated mass-one normalization. Maximality of an independently labelled chart-side section or another supplied maximal section does not replace this premise. No equality between the hypersurface identification and the physical stationary end chart is assumed. [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] Adopt the stationary vacuum model and regular exterior, the original maximal section and the mass-one normalization, including Choice and all displayed geometric conventions. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-harrison-normalization]] [[def-spacelike-maximal-hypersurface-data]] [[def-stationary-lorentzian-data]] [[def-stationary-asymptotic-decay-data]] [[math:def-axiom-of-choice]]

[F2] The end estimates give the normalized Ernst expansion, and the single smooth stationary global primitive has original-chart spatial coefficients $(W_0)_i=O_5(r^{-3})$ and smooth horizon extension. [[pthm-ernst-and-one-form-decay]] [[pthm-global-harrison-one-form]] [[def-killing-ernst-notation]] [[def-harrison-one-form-family]]

[F3] The authored electrovacuum result gives the two Maxwell equations in the exterior and near the bifurcation sphere, with parameter-continuous fields and regular metrics. [[pthm-harrison-electrovacuum]] [[def-harrison-electromagnetic-form]] [[def-source-free-geometric-electrovacuum-data]]

[F4] The product exterior and original section give compact annuli from an end sphere to the inner sphere; flux densities and the inherited sphere orientation are fixed. [[pthm-original-lapse-and-product]] [[def-surface-area-flux-and-null-variation-data]]

[F5] The five local lemmas provide the seed sign, Harrison spatial restriction, positive-parameter charge limit, Stokes transfer and fixed-sphere endpoint passage. [[lem-author-ce4974f559ec-killing-end-flux]] [[lem-author-ce4974f559ec-harrison-end-restriction]] [[lem-author-ce4974f559ec-positive-parameter-charge]] [[lem-author-ce4974f559ec-closed-flux-transfer]] [[lem-author-ce4974f559ec-fixed-sphere-endpoints]]

[F6] The spacetime orientation makes $dt\wedge dx^1\wedge dx^2\wedge dx^3$ positive in the chosen stationary end chart, exactly as required by the oriented seed-flux lemma. [[def-killing-ernst-notation]] [[lem-author-ce4974f559ec-killing-end-flux]]

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] Adopt the stationary vacuum model and regular exterior, the original maximal section and the mass-one normalization, including Choice and all displayed geometric conventions. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-harrison-normalization]] [[def-spacelike-maximal-hypersurface-data]] [[def-stationary-lorentzian-data]] [[def-stationary-asymptotic-decay-data]] [[math:def-axiom-of-choice]]

[F2] The end estimates give the normalized Ernst expansion, and the single smooth stationary global primitive has original-chart spatial coefficients $(W_0)_i=O_5(r^{-3})$ and smooth horizon extension. [[pthm-ernst-and-one-form-decay]] [[pthm-global-harrison-one-form]] [[def-killing-ernst-notation]] [[def-harrison-one-form-family]]

[F3] The authored electrovacuum result gives the two Maxwell equations in the exterior and near the bifurcation sphere, with parameter-continuous fields and regular metrics. [[pthm-harrison-electrovacuum]] [[def-harrison-electromagnetic-form]] [[def-source-free-geometric-electrovacuum-data]]

[F4] The product exterior and original section give compact annuli from an end sphere to the inner sphere; flux densities and the inherited sphere orientation are fixed. [[pthm-original-lapse-and-product]] [[def-surface-area-flux-and-null-variation-data]]

[F5] The five local lemmas provide the seed sign, Harrison spatial restriction, positive-parameter charge limit, Stokes transfer and fixed-sphere endpoint passage. [[lem-author-ce4974f559ec-killing-end-flux]] [[lem-author-ce4974f559ec-harrison-end-restriction]] [[lem-author-ce4974f559ec-positive-parameter-charge]] [[lem-author-ce4974f559ec-closed-flux-transfer]] [[lem-author-ce4974f559ec-fixed-sphere-endpoints]]

[F6] The spacetime orientation makes $dt\wedge dx^1\wedge dx^2\wedge dx^3$ positive in the chosen stationary end chart, exactly as required by the oriented seed-flux lemma. [[def-killing-ernst-notation]] [[lem-author-ce4974f559ec-killing-end-flux]]



**Proof technique:** direct.

1.1 Fix $0<q<1$. The orientation in [F6] is exactly the seed-flux convention. By the mass-one end and Ernst conventions and the smooth global primitive's original-chart spatial decay, the first two local end lemmas apply: $F_{0i}=x^i/r^3+O(r^{-3})$, $F_{ij}=O(r^{-3})$, $\sigma=1-2/r+O(r^{-2})$ and $(W_0)_i=O(r^{-3})$. The positive-parameter charge lemma therefore gives electric and magnetic limits $\sqrt{1-q^2}$ and zero on the original stationary-coordinate spheres. This uses only the stated $g_{0i}=O_6(r^{-2})$, not an angular-momentum leading term or the global hypotheses of an independent Harrison charge theorem. [F1, F2, F3, F5, F6]

2.1 The two closed forms are smooth on the compact annulus and through its inner collar by the authored electrovacuum and primitive results. The product exterior supplies the annulus and the orientation relation $\partial C_R=S_R-S$. The flux-transfer lemma equates both sphere integrals with their values on $S_R$. Their equality holds for each sufficiently large $R$, so taking $R\to\infty$ gives the two asserted identities on $S$. Stokes also proves the claimed homology invariance. [F3, F4, F5, step 1.1]

3.1 To include zero, fix one compact regular sphere, for example $S$ itself in its supplied smooth neighborhood. The metrics remain Lorentzian and have the same orientation; their positive denominators on this compact sphere have a positive minimum over $q\in[0,1]$. The electromagnetic fields are continuous in $q$ by the authored electrovacuum result. The fixed-sphere lemma extends both identities from step 2.1 to $q=0$, giving one and zero. The same continuity, or directly $F_1=0$, gives the endpoint at one. The calculation neither assumes transformed asymptotic flatness at zero nor exchanges its parameter limit with infinity. This proves the full Statement. [F3, F5, step 2.1] ∎



The independent source §3.3 confirms the Hodge sign and fixed-sphere endpoint method, but its stronger global GR/SBS and angular-momentum hypotheses are not used to supply the charges here. The five local mathematical helpers prove the end-charge and transfer calculation from the exact authored interfaces. The mass-one value refers to the article end coefficient, as supplied by the authored Ernst-decay item. The original article is attribution only.

## Source notes

The independent source §3.3 confirms the Hodge sign and fixed-sphere endpoint method, but its stronger global GR/SBS and angular-momentum hypotheses are not used to supply the charges here. The five local mathematical helpers prove the end-charge and transfer calculation from the exact authored interfaces. The mass-one value refers to the article end coefficient, as supplied by the authored Ernst-decay item. The original article is attribution only.

These explicit premises specify the generated conditional result. They are not asserted to follow from the original regularity definition alone, and are not attributed to the original article. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

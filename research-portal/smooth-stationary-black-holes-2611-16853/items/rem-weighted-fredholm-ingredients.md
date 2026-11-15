---
id: rem-weighted-fredholm-ingredients
title: Fredholm ingredients stated in Lemma 3.1
kind: remark
status: published
origin: pipeline
domain: mathematics
proof_strategy: direct
deps:
  - math:def-axiom-of-choice
  - def-weighted-holder-spaces
  - def-exterior-weighted-elliptic-data
  - def-fredholm-continuation-data
  - lem-exterior-parametrix-and-compact-potential
  - lem-author-1f6675f2ec55-full-space-compact-potential
  - math:thm-fredholm-index-is-stable-under-compact-perturbations
  - lem-author-1f6675f2ec55-decaying-kernel-components
dependency_roles:
  math:def-axiom-of-choice: mathematical-premise
  def-weighted-holder-spaces: mathematical-premise
  def-exterior-weighted-elliptic-data: mathematical-premise
  def-fredholm-continuation-data: mathematical-premise
  lem-exterior-parametrix-and-compact-potential: mathematical-premise
  lem-author-1f6675f2ec55-full-space-compact-potential: mathematical-premise
  math:thm-fredholm-index-is-stable-under-compact-perturbations: mathematical-premise
  lem-author-1f6675f2ec55-decaying-kernel-components: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p.13, Lemma 3.1 and its proof; exterior geometry in Definition 1.1
        and §3
      statement: In the three-dimensional exterior Dirichlet setting, for -1<β<0 the
        article uses index zero of the scalar Dirichlet Laplacian, compact
        multiplication by V∈C^{2,α}_{-4} on the full weighted input space, and
        zero decaying Dirichlet kernel for nonnegative V.
      hypotheses: The smooth connected exterior section in the article,
        h−δ∈C^{3,α}_{−1}, compact smooth boundary, 0<α<1, −1<β<0 and V≥0 in
        C^{2,α}_{−4}. This records attribution, not independent prerequisite
        evidence.
      reading_limits: Read frozen PDF p.13 image and its extracted text, and the
        supplied exterior-section interfaces. This citation attributes the
        article ingredients; their local arguments below use independent
        declared suppliers. No whole-article reading or original-article defect
        assessment is claimed.
dependency_level: 5
---

## Statement

Assume the Axiom of Choice. In Lemma 3.1 the article uses three distinct ingredients: the scalar zero-Dirichlet Laplacian has index zero for $-1<\beta<0$; multiplication by $V\in C^{2,\alpha}_{-4}$ is compact from the full $C^{4,\alpha}_\beta$ space to $C^{2,\alpha}_{\beta-2}$; and a nonnegative potential eliminates its decaying zero-boundary kernel on the article's connected exterior.

Precisely, use the weighted three-dimensional exterior conventions, $0<\alpha<1$, a smooth asymptotically flat metric with $h-\delta\in C^{3,\alpha}_{-1}$, and $-1<\beta<0$. Put $X_\beta=\{u\in C^{4,\alpha}_\beta:u|_S=0\}$ and $Y_\beta=C^{2,\alpha}_{\beta-2}$. The map $\Delta_h:X_\beta\to Y_\beta$ is Fredholm of index zero. The compact multiplication assertion holds on the full input space without a boundary condition and therefore also on $X_\beta$. Consequently $\Delta_h-V:X_\beta\to Y_\beta$ is Fredholm of index zero without a sign assumption. If $V\ge0$ and the exterior is connected, its kernel is zero. On the more permissive disconnected exterior interface, its only possible kernel consists of constants on closed compact components where $V\equiv0$. Thus index zero and kernel elimination are separate assertions, and the Dirichlet condition belongs to the Laplacian's domain rather than the compactness hypothesis.

## Statement references

[[math:def-axiom-of-choice]]

[[def-weighted-holder-spaces]]

[[def-exterior-weighted-elliptic-data]]

[[def-fredholm-continuation-data]]

[[lem-exterior-parametrix-and-compact-potential]]

[[lem-author-1f6675f2ec55-full-space-compact-potential]]

[[math:thm-fredholm-index-is-stable-under-compact-perturbations]]

[[lem-author-1f6675f2ec55-decaying-kernel-components]]

## Facts & Assumptions

**Given:** The hypotheses of the Statement.

**Goal:** Establish its stated analytic ingredients and qualifications.

[F1] The Axiom of Choice includes the analytic suppliers’ inherited assumptions. [[math:def-axiom-of-choice]]

[F2] The weighted Hölder and exterior interfaces specify $X_\beta$, $Y_\beta$, their end chart, inner boundary and metric-decay conventions. [[def-weighted-holder-spaces]] [[def-exterior-weighted-elliptic-data]]

[F3] Fredholm index is kernel dimension minus cokernel dimension for a bounded operator with closed range and finite kernel and cokernel. [[def-fredholm-continuation-data]]

[F4] The independently authored exterior Dirichlet construction gives index zero for $\Delta_h:X_\beta\to Y_\beta$, including permissible compact extra components. [[lem-exterior-parametrix-and-compact-potential]]

[F5] Potential multiplication is compact from the full weighted input space, and remains compact on its zero-Dirichlet subspace. [[lem-author-1f6675f2ec55-full-space-compact-potential]]

[F6] A compact perturbation of a Fredholm operator between Banach spaces is Fredholm with the same index. [[math:thm-fredholm-index-is-stable-under-compact-perturbations]]

[F7] For nonnegative $C^{2,\alpha}_{-4}$ potentials the decaying kernel vanishes on the end component and all boundary components; the only exceptions are constants on closed compact components with zero potential. [[lem-author-1f6675f2ec55-decaying-kernel-components]]

## Proof

**Given:**The hypotheses of the Statement.

**Goal:** Establish its stated analytic ingredients and qualifications.

[F1] The Axiom of Choice includes the analytic suppliers’ inherited assumptions. [[math:def-axiom-of-choice]]

[F2] The weighted Hölder and exterior interfaces specify $X_\beta$, $Y_\beta$, their end chart, inner boundary and metric-decay conventions. [[def-weighted-holder-spaces]] [[def-exterior-weighted-elliptic-data]]

[F3] Fredholm index is kernel dimension minus cokernel dimension for a bounded operator with closed range and finite kernel and cokernel. [[def-fredholm-continuation-data]]

[F4] The independently authored exterior Dirichlet construction gives index zero for $\Delta_h:X_\beta\to Y_\beta$, including permissible compact extra components. [[lem-exterior-parametrix-and-compact-potential]]

[F5] Potential multiplication is compact from the full weighted input space, and remains compact on its zero-Dirichlet subspace. [[lem-author-1f6675f2ec55-full-space-compact-potential]]

[F6] A compact perturbation of a Fredholm operator between Banach spaces is Fredholm with the same index. [[math:thm-fredholm-index-is-stable-under-compact-perturbations]]

[F7] For nonnegative $C^{2,\alpha}_{-4}$ potentials the decaying kernel vanishes on the end component and all boundary components; the only exceptions are constants on closed compact components with zero potential. [[lem-author-1f6675f2ec55-decaying-kernel-components]]



1.1 The authored scalar exterior construction applies exactly at the stated orders, metric falloff and weight interval to the zero-trace domain. It supplies Fredholmness and index zero without replacing the scalar operator by a vector Laplacian. The full-space multiplication lemma gives precisely the compactness stated in the article, including inputs with arbitrary inner-boundary trace; its restriction to $X_\beta$ is compact as well. [F2, F4, F5]

2.1 Apply compact-perturbation stability to the Dirichlet Laplacian and the compact map $-M_V$ between its Banach domain and target. This gives index zero for $\Delta_h-V$ regardless of the sign of $V$. When $V\ge0$, use the continuous-potential kernel classification. The article’s exterior section is connected, so it has no separate closed compact component and its kernel is zero; in the larger supplier scope the stated closed-component exception is retained. These are independent ingredients for the article’s Fredholm argument, not a claim that index zero alone implies injectivity. [F1, F3, F6, F7, step 1.1] ∎

## Source notes

The frozen article PDF p.13 and its extracted text were read for attribution. The actual An–Huang source, arXiv:2206.00079v2, Lemma 3.3, printed pp.16–17, concerns a vector operator Γ depending on a positive scalar field and an asymptotically flat pair. Its stated vector theorem is not silently used here as the scalar Dirichlet theorem; the already authored scalar supplier supplies that result. The two new interface extensions are proved locally: no boundary trace is used in compact multiplication, and positive-part comparison only requires a continuous nonnegative potential. No original-article defect or independent proof review is asserted.

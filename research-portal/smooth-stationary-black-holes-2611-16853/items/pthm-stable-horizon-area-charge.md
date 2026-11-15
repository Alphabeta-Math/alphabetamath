---
id: pthm-stable-horizon-area-charge
title: Stable-horizon flux-energy and area-charge inequalities
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - def-harrison-one-form
  - def-harrison-electromagnetic-form
  - pthm-harrison-electrovacuum
  - def-horizon-flux-and-stability-notation
  - def-surface-area-flux-and-null-variation-data
  - pthm-stable-bifurcation-mots
  - pthm-mots-stability-operator
  - thm-principal-eigenvalue-and-mots-stability-input
  - math:thm-riemannian-divergence-theorem
  - math:thm-global-gauss-bonnet-for-closed-oriented-riemannian-surfaces
  - math:cor-cauchy-schwarz-inequality-for-l-two
  - math:def-axiom-of-choice
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-harrison-one-form: mathematical-premise
  def-harrison-electromagnetic-form: mathematical-premise
  pthm-harrison-electrovacuum: physical-result
  def-horizon-flux-and-stability-notation: mathematical-premise
  def-surface-area-flux-and-null-variation-data: mathematical-premise
  pthm-stable-bifurcation-mots: physical-result
  pthm-mots-stability-operator: physical-result
  thm-principal-eigenvalue-and-mots-stability-input: mathematical-premise
  math:thm-riemannian-divergence-theorem: mathematical-premise
  math:thm-global-gauss-bonnet-for-closed-oriented-riemannian-surfaces: mathematical-premise
  math:cor-cauchy-schwarz-inequality-for-l-two: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional deduction in the smooth stationary vacuum model and
  its positive-parameter source-free Einstein–Maxwell Harrison family; no
  measurement is asserted.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 27, proof of Theorem 4.2 and proof of Corollary 4.1
      attribution: The article obtains the horizon flux-energy bound from the
        stability equation and Gauss–Bonnet, invokes an area–charge inequality,
        and states that the latter also follows directly from that equation and
        Gauss–Bonnet.
      hypotheses: The article's regular stationary vacuum construction, maximal
        sections and positive-parameter Harrison geometry.
      reading_limits: The frozen article text was inspected for attribution and scope.
        This citation is not used as a proof premise.
dependency_level: 27
---

## Statement

Assume the regular non-degenerate stationary vacuum model, with original exterior section maximal, ADM mass normalized to one and stationary Killing field $T$ nontrivial on its bifurcation sphere $S$. Fix $q\in(0,1]$ and an individually admissible smooth spacelike maximal section $\Sigma_q$ as in [[pthm-stable-bifurcation-mots]], with a smooth spacelike extension and outward normal-graph tube as in [[pthm-mots-stability-operator]]. Work in ZFC. Let $g_q,F_q$ be the Harrison metric and electromagnetic two-form, and let $\gamma_q=g_q|_{TS}$ and $d\mu_q$ be the induced metric and oriented area form. Define electric and magnetic flux densities by $(\star_{g_q}F_q)|_{TS}=e_q\,d\mu_q$ and $F_q|_{TS}=b_q\,d\mu_q$. Then
$$\int_S(e_q^2+b_q^2)\,d\mu_q\le4\pi,\qquad |S|_{g_q}\ge\frac{1}{4\pi}\left(\int_Se_q\,d\mu_q\right)^2.$$
Here $|S|_{g_q}=\int_Sd\mu_q$. In particular, both inequalities hold for sufficiently small positive $q$ under the same hypotheses. The second inequality follows directly from the same stability equation and Gauss–Bonnet.

## Facts & Assumptions

**Given:** The model, parameter, admissible section, extension and graph data in the Statement.

**Goal:** Prove the two displayed inequalities.

[A1] The regularity and normalization conventions and the meaning of a spacelike maximal section are those of [[def-regular-stationary-vacuum-spacetime]], [[def-harrison-normalization]] and [[def-spacelike-maximal-hypersurface-data]], in the conditional model [[post-stationary-vacuum-model]]. Work in ZFC. [[math:def-axiom-of-choice]]

[F1] The horizon and surface-data definitions supply the smooth positive surface measure, null gauge, flux densities and intrinsic gradient, divergence, Laplacian and Gauss curvature. [[def-horizon-flux-and-stability-notation]] [[def-surface-area-flux-and-null-variation-data]]

[F2] For the stated section, $S$ is a connected closed two-sphere and the outward graph stability operator has nonnegative principal eigenvalue $\lambda$. The principal-eigenvalue theorem supplies a smooth eigenfunction $\phi>0$ with $\mathscr L_q\phi=\lambda\phi$. [[pthm-stable-bifurcation-mots]] [[thm-principal-eigenvalue-and-mots-stability-input]]

[F3] In this gauge the operator is $\mathscr L_q\phi=-\Delta\phi+2\zeta\cdot\nabla\phi+(K+\operatorname{div}\zeta-|\zeta|^2-e_q^2-b_q^2)\phi$, with all surface operations taken for $\gamma_q$. [[pthm-mots-stability-operator]]

[F4] On the closed oriented surface, the integral of the divergence of a smooth vector field is zero. Gauss–Bonnet gives $\int_SK\,d\mu_q=2\pi\chi(S)=4\pi$; a tetrahedral triangulation of the two-sphere has Euler characteristic $4-6+4=2$. [[math:thm-riemannian-divergence-theorem]] [[math:thm-global-gauss-bonnet-for-closed-oriented-riemannian-surfaces]]

[F5] Cauchy–Schwarz applies to square-integrable functions for the finite surface measure. [[math:cor-cauchy-schwarz-inequality-for-l-two]]

[F6] The construction in [[pthm-harrison-electrovacuum]] applies under [A1] and supplies the normalized smooth Ernst potential and a stationary one-form family satisfying the defining curl and contraction identities, with $d_q=D_q(p)>0$ at a zero $p\in S$ of $T$, on the exterior and an open neighborhood of $S$ where $D_q>0$. The symbols $g_q,F_q$ denote the resulting smooth Lorentzian metric and real two-form of [[def-harrison-one-form]] and [[def-harrison-electromagnetic-form]], using the same fields, spacetime orientation and time orientation in [F1]–[F3].

## Proof

**Proof technique:** direct.

1.1 Set $u=\log\phi$ and let $\zeta^\sharp$ be the surface metric-dual vector field. Dividing the eigenvalue equation in [F3] by $\phi$ and using $\Delta\phi/\phi=\Delta u+|\nabla u|^2$ gives $\lambda=K-e_q^2-b_q^2+\operatorname{div}(\zeta^\sharp-\nabla u)-|\zeta^\sharp-\nabla u|^2$. The positive eigenfunction makes $u$ smooth. Integrating, applying [F4], and using $\lambda\ge0$ yields $\int_S(e_q^2+b_q^2)\,d\mu_q=4\pi-\lambda|S|_{g_q}-\int_S|\zeta^\sharp-\nabla u|^2\,d\mu_q\le4\pi$. [given, F1, F2, F3, F4, F6, algebra]

2.1 Smoothness and compactness put $e_q$ and the constant function $1$ in $L^2(d\mu_q)$. By [F5], $|\int_Se_q\,d\mu_q|^2\le |S|_{g_q}\int_Se_q^2\,d\mu_q$. Since $b_q^2\ge0$, step 1.1 bounds the last integral by $4\pi$. Dividing by $4\pi$ gives the area–charge inequality. This also proves its derivation from the same stability equation and Gauss–Bonnet. The fixed $q$ was arbitrary in $(0,1]$, so the asserted sufficiently-small-positive-parameter case follows. [F1, F5, F6, step 1.1, algebra] ∎

## Source notes

The article reference records attribution. The proof uses the listed suppliers; it does not use the article's assertion as a premise.

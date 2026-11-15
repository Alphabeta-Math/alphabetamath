---
id: pthm-mots-stability-operator
title: Horizon expansion variation and Einstein–Maxwell curvature
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - def-stationary-lorentzian-data
  - def-horizon-flux-and-stability-notation
  - def-surface-area-flux-and-null-variation-data
  - def-source-free-geometric-electrovacuum-data
  - pthm-harrison-electrovacuum
  - pthm-bifurcate-horizon-preservation
  - lem-killing-normal-boost-and-invariant-tensors
  - lem-author-6413ea293c6d-electrovac-normal-contraction
  - thm-mots-first-variation-input
  - math:def-axiom-of-choice
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-horizon-flux-and-stability-notation: mathematical-premise
  def-surface-area-flux-and-null-variation-data: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  pthm-harrison-electrovacuum: physical-result
  pthm-bifurcate-horizon-preservation: physical-result
  lem-killing-normal-boost-and-invariant-tensors: mathematical-premise
  lem-author-6413ea293c6d-electrovac-normal-contraction: mathematical-premise
  thm-mots-first-variation-input: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 26, equation (4.4) and the following sentence
      hypotheses: The article's Harrison geometry and smooth spacelike maximal section
        with bifurcation-sphere boundary, in the stated null-normal gauge.
      reading_limits: Consulted the frozen extracted article text on PDF page 26,
        equation (4.4) and the following sentence, for attribution only. The
        article gives the displayed horizon expansion variation and the
        mixed-null Ricci identity in its Einstein–Maxwell setting. This
        reference is not an imported premise or proof; the local deduction uses
        the declared suppliers.
physical_scope: Conditional deduction in the stated stationary vacuum model and
  its source-free Einstein–Maxwell Harrison family; no measurement or existence
  of a candidate section is asserted.
dependency_level: 10
---

## Statement

Adopt the regular stationary vacuum model with original exterior section maximal, mass normalized to one, and stationary field $T$ nontrivial on the bifurcation sphere $S$. Fix $q\in(0,1]$. Use one smooth Harrison construction on the exterior and an open neighborhood $O$ of $S$ common to the electrovacuum and horizon-preservation results, with the same normalized Ernst potential, pole and stationary primitive, in the invariant horizon gauge required by the latter. Denote its metric and electromagnetic two-form by $g_q,F_q$.

Suppose a smooth spacelike maximal section $\Sigma_q$ with boundary $S$ and the boundary data of the horizon notation are supplied: smooth metric and two-form extensions on an open neighborhood $U_S$ of $S$, a smooth spacelike section extension across $S$, an outward unit normal, and an admissible normal-graph tube. Require that on an open neighborhood $O_S\subseteq U_S\cap O$ of $S$ the supplied metric and two-form extensions coincide with these same Harrison fields, with matching orientations and time orientations. Use the section extension and normal-graph tube near $S$ inside $O_S$.

Let $n_q$ be the future unit normal to the extended section and $\nu_q$ the outward unit normal to $S$ in it. Set $L_q=n_q+\nu_q$ and $\underline L_q=(n_q-\nu_q)/2$, so that $g_q(L_q,\underline L_q)=-1$. With $\nabla^{(q)}$ the Levi–Civita connection of $g_q$, define the normal connection one-form by $\zeta_q(X)=-g_q(\underline L_q,\nabla^{(q)}_X L_q)$ for $X$ tangent to $S$. The oriented area form of $\gamma_q=g_q|_{TS}$ is $d\mu_q$; define $e_q,b_q$ by $(\star_{g_q}F_q)|_{TS}=e_q\,d\mu_q$ and $F_q|_{TS}=b_q\,d\mu_q$.

Let $\not\nabla^{(q)}$, $\not\operatorname{div}^{(q)}$ and $\not\Delta^{(q)}$ be the intrinsic connection, divergence and divergence-of-gradient Laplacian of $\gamma_q$; divergence of a one-form means divergence of its metric-dual vector. Let $K_q$ be its Gauss curvature with the positive-round-sphere convention. The outgoing expansion is the $\gamma_q$-trace of $(X,Y)\mapsto g_q(\nabla^{(q)}_X L_q,Y)$. Pulling back the outgoing expansion of the normal graph with its future null normal $n_q+\nu_{q,u}$ defines $\Theta_q(u)$; write $\mathscr L_q\phi=\left.\frac{d}{d\epsilon}\right|_0\Theta_q(\epsilon\phi)$.

Then $S$ has zero outgoing expansion and, for every smooth function $\phi$ on $S$,
$$\mathscr L_q\phi=-\not\Delta^{(q)}\phi+2\zeta_q\cdot\not\nabla^{(q)}\phi+\bigl(K_q+\not\operatorname{div}^{(q)}\zeta_q-|\zeta_q|^2-e_q^2-b_q^2\bigr)\phi.$$
Moreover $\operatorname{Ric}_{g_q}(L_q,\underline L_q)=e_q^2+b_q^2$. The dot product and norm are taken with $\gamma_q$. The conclusions are conditional on the supplied section and graph data.

The original-section maximality premise is imposed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$ for the original metric $g$, so $H_g|_C=0$. Where this result uses the original reference section $\Sigma_1$, it denotes the closure $B=C\cup S$ of this actual section. Maximality of a separately labelled chart-side region or another supplied section is not substituted for this premise. The spherical identification and the physical stationary end chart remain independent. [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-harrison-normalization]]

[[def-stationary-lorentzian-data]]

[[def-horizon-flux-and-stability-notation]]

[[def-surface-area-flux-and-null-variation-data]]

[[def-source-free-geometric-electrovacuum-data]]

[[pthm-harrison-electrovacuum]]

[[pthm-bifurcate-horizon-preservation]]

[[lem-killing-normal-boost-and-invariant-tensors]]

[[lem-author-6413ea293c6d-electrovac-normal-contraction]]

[[thm-mots-first-variation-input]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

[A1] The model and regular data, the original maximality, mass-one normalization, nontriviality of $T|_S$, and the supplied candidate section and graph data are as in the Statement; work with the Axiom of Choice. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]] [[def-harrison-normalization]] [[math:def-axiom-of-choice]]

[A2] The boundary metric and two-form coincide on $O_S$ with the same Harrison fields used in both the electrovacuum and horizon-preservation applications, in the invariant horizon gauge. The section extension and graph tube are used in $O_S$, with matching orientations and time orientations. [[def-horizon-flux-and-stability-notation]] [[pthm-harrison-electrovacuum]] [[pthm-bifurcate-horizon-preservation]]

[F1] The surface and horizon notation suppliers define the null gauge, flux densities, intrinsic operators, expansion and its normal-graph variation under the stated smoothness and orientation hypotheses. [[def-horizon-flux-and-stability-notation]] [[def-surface-area-flux-and-null-variation-data]]

[F2] The Harrison fields satisfy the geometric source-free electrovacuum equations on an open neighborhood of $S$. In particular $\operatorname{Ric}_{ab}=2(F_{ac}F_b{}^c-\frac14g_{ab}F_{cd}F^{cd})$, with contractions made using $g_q$. [[pthm-harrison-electrovacuum]] [[def-source-free-geometric-electrovacuum-data]]

[F3] For $g_q$, the local Hawking field $K$ is Killing, vanishes on $S$, and has a nonzero-rate normal boost on the quotient $TM|_S/TS$. The surface $S$ is spacelike and totally geodesic for $g_q$, so both its null second fundamental forms vanish. [[pthm-bifurcate-horizon-preservation]] [[lem-killing-normal-boost-and-invariant-tensors]]

[F4] In the normalized surface gauge, the electrovac normal-contraction lemma gives $\operatorname{Ric}(L,\underline L)=e^2+b^2$ and zero scalar curvature. [[lem-author-6413ea293c6d-electrovac-normal-contraction]]

[F5] The general MOTS variation supplier gives the displayed specialized operator when the surface gauge is used and both $\chi_L=0$ and $\operatorname{Ric}(L,L)=0$ hold. Its variation is the admissible normal-graph variation in the stated gauge. [[thm-mots-first-variation-input]]

[F6] A smooth nondegenerate metric has a unique torsion-free metric-compatible connection; its curvature and Ricci tensor use the stated tensor conventions. [[def-stationary-lorentzian-data]]

## Proof

**Given:** The model, parameter and supplied section, orientation and normal-graph data in the Statement.

**Goal:** Establish the mixed-null Ricci identity and the stated outgoing-expansion variation.

1.1 By [A2], the metric and two-form on the supplied boundary neighborhood and graph tube are the same fields, with the same orientations, as in the electrovacuum and horizon-preservation constructions. Thus [F2] and [F3] apply to the actual fields used in the variation. By the horizon result, $S$ is $g_q$-spacelike and its null second fundamental forms vanish. In particular $\chi_{L_q}=0$, and its trace, the outgoing expansion, is zero. The stated graph data therefore define an admissible variation of a marginally outer trapped surface in the gauge of the first-variation supplier. [given, A2, F1, F2, F3]

2.1 The flow of $K$ fixes $S$ pointwise and acts as an isometry of $g_q$. It consequently preserves the $g_q$-normal plane of $S$. Its action on that plane is conjugate, through the quotient by $TS$, to the nonzero-rate boost in [F3]. As the flow is connected to the identity, it preserves each of the two null lines in the normal plane; its action on the line of $L_q$ is multiplication by $e^{\kappa t}$ or $e^{-\kappa t}$, with $\kappa>0$. An isometry preserves the Levi–Civita connection by uniqueness and hence preserves its Ricci tensor. At a fixed point this gives $\operatorname{Ric}(L_q,L_q)=e^{\pm 2\kappa t}\operatorname{Ric}(L_q,L_q)$. Choosing a sufficiently small nonzero flow time yields $\operatorname{Ric}(L_q,L_q)=0$. [given, F3, F6, step 1.1]

3.1 The electrovac equations and the normalized surface gauge satisfy the hypotheses of the normal-contraction lemma, which gives $\operatorname{Ric}_{g_q}(L_q,\underline L_q)=e_q^2+b_q^2$. Combining the vanishing of $\chi_{L_q}$ and $\operatorname{Ric}(L_q,L_q)$ with the specialized first-variation formula gives the displayed expression for $\mathscr L_q\phi$. The first-variation supplier includes the conversion between its $g(l,k)=-2$ normalization and $L_q,\underline L_q$; no different null gauge is substituted. [F1, F2, F4, F5, step 1.1, step 2.1] ∎

## Source notes

The article reference attributes equation (4.4) and the subsequent mixed-null Ricci identity. The deduction above uses the completed suppliers and does not use the article's assertion as a premise. The boundary compatibility is an explicit condition on the supplied data. The notation definition alone permits more general extensions and does not establish their electrovacuum equations or Killing symmetry. The proof here applies both geometric results only to the common Harrison fields specified in the Statement; no existence of compatible section or graph data is asserted.

These premises specify the generated conditional scope and are not attributed to the original article. The substantive local horizon conclusions are retained. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

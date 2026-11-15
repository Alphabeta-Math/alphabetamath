---
id: pthm-cutoff-angle-estimate
title: Cutoff maximum principle and uniform collar regularity
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - def-stationary-maximal-graph
  - pthm-common-reference-collar
  - pthm-boundary-normal-angle
  - pthm-normal-angle-differential-inequality
  - def-spacelike-maximal-hypersurface-data
  - math:def-axiom-of-choice
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - lem-author-14de055b8ceb-gaussian-cutoff-projection
  - lem-author-14de055b8ceb-weighted-cutoff-maximum
  - lem-author-14de055b8ceb-gaussian-maximal-graph-operator
  - lem-author-14de055b8ceb-uniform-elliptic-jet-extension
  - lem-author-14de055b8ceb-boundary-seeded-schauder-bootstrap
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  pthm-common-reference-collar: physical-result
  pthm-boundary-normal-angle: physical-result
  pthm-normal-angle-differential-inequality: physical-result
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  lem-author-14de055b8ceb-gaussian-cutoff-projection: mathematical-premise
  lem-author-14de055b8ceb-weighted-cutoff-maximum: mathematical-premise
  lem-author-14de055b8ceb-gaussian-maximal-graph-operator: mathematical-premise
  lem-author-14de055b8ceb-uniform-elliptic-jet-extension: mathematical-premise
  lem-author-14de055b8ceb-boundary-seeded-schauder-bootstrap: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-altered
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p.19, proof of Lemma3.4, cutoff calculation and final Schauder
        sentence
      reading_limits: "Attribution only, not an imported premise. Historical claim
        description: The original article gives the cutoff, normal-angle
        estimate on its positive inner region, and uniform higher-order collar
        estimates described in the Statement. Historical scope: Existing maximal
        sections and preceding boundary graph/height hypotheses in the regular
        stationary vacuum/Harrison construction, q in a fixed positive interval.
        Attribution only. Retained reading record: Read frozen original PDF p.19
        image and extracted text, with Gaussian and cone setup pp.18–19. This
        reference attributes the original claim and is not a prerequisite proof.
        This maintenance revision checks current supplier contracts; no new
        original-PDF reading is claimed."
    - title: Leon Simon, Lectures on PDE
      url: https://math.stanford.edu/~lms/lecs-on-pde.pdf
      locator: Lecture 18, Theorem 2 (C^{1,beta} estimate, boundary), printed p.217,
        assumptions (P), (*) and (**) on pp.216–217; PDF sheet111
      statement: Let u be a C2 solution of a^{ij}(x,u,Du)u_ij=f on a boundary patch,
        with u=0 on the actual boundary, bounded |u|+R|Du|, bounded f, C1 joint
        bounds on a^{ij} in a containing position/height/slope box, positive
        uniform ellipticity on that box, and a C2 boundary-flattening
        diffeomorphism and inverse with bounded norms. On every smaller patch
        there is a uniform C^{1,beta} bound, for some beta in (0,1), with
        constants controlled by dimension, shrinking factor, the height/gradient
        bound, structural coefficient/ellipticity constants and the flattening
        constants. The analogous interior statement is Theorem 1 on the same
        page.
      hypotheses: Classical C2 solution, C1 joint principal coefficients, bounded RHS,
        uniform positive ellipticity on the containing slope/height box, a
        common finite height/gradient bound and uniformly C2 flattenable
        boundary; homogeneous Dirichlet trace on the actual boundary portion.
        Bounds are local and do not require any condition at the remote
        spherical edge of the patch.
      reading_limits: "Retained independent source-input/background reading record:
        Read the actual retained Simon PDF sheet111, printed pp.216–217,
        including (P), (*), (**), Theorems1–2 and all stated dependencies. No
        full proof reconstruction is claimed. This is an imported a priori
        estimate, not a claimed local proof of boundary gradient Holder
        regularity. Current maintenance checks the stated contract and its local
        application, without claiming new external-proof or PDF reading."
physical_scope: Conditional geometric and elliptic estimates for supplied
  existing maximal sections in the smooth stationary vacuum/Harrison model, on
  each fixed positive parameter interval; no candidate-existence or empirical
  claim.
dependency_level: 19
---

## Statement

Fix $\delta>0$ in the supplied regular mass-one stationary vacuum/Harrison construction, with $T|_S\not\equiv0$, and its existing smooth spacelike maximal sections $\Sigma_q$, $q\in[\delta,1]$, with the complete preceding boundary height and barrier hypotheses. On the common Gaussian graph collar let $R_q=\rho_q\circ\pi_q^\perp$ and $|\tau_q|\le\theta_\delta R_q$, where $\theta_\delta<1$. Choose $\theta_\delta<c<1$. Let $r_\delta>0$ be the common normal-graph radius supplied by the boundary-angle result. Fix $0<\rho_\delta<r_\delta$ small enough that the closed cone region $0\le R_q\le\rho_\delta$, $|\tau_q|\le\theta_\delta R_q$ lies in a fixed compact common Gaussian tube, after the uniform shrinking in Proof 1.1, and in the collar of the full-range angle inequality. Choose $0<d<\tfrac12(c-\theta_\delta)\rho_\delta$ and set $\chi=(1+(\tau_q-cR_q)/d)_+$. Then $\chi=1$ on $S$, $\chi=0$ on $R_q=\rho_\delta/2$, and $0\le\chi\le1$ on the candidate collar. On $\chi>0$, $|\nabla\chi|_{h_q}^2\ge c_\delta v_q^2-C_\delta$ and $|\Delta_{h_q}\chi|\le C_\delta v_q^2$, where $v_q=-g_q(n_q,-\operatorname{grad}_{g_q}\tau_q)\ge1$. At an interior positive maximum of $\chi^mv_q$, $\nabla\log v_q=-m\nabla\chi/\chi$ and $0\ge\Delta\log(\chi^mv_q)\ge(m^2/4-m)|\nabla\chi|^2/\chi^2-C_\delta v_q^2(1+m/\chi)$. A common sufficiently large integer $m$ gives $\sup_{\chi\ge1/2}v_q\le C_\delta$. This region contains a fixed positive-width reference collar of $S$. On a smaller common collar the normal graph heights have uniform $C^{k,\alpha}$ bounds for every finite $k$ and $0<\alpha<1$, including up to $S$, and the graphs are uniformly spacelike. Constants may depend on $\delta,k,\alpha$ and the fixed background but not on the candidate or on $q\in[\delta,1]$.

## Facts & Assumptions

[A1] Adopt the stationary vacuum model, regular data, mass-one normalization, with $T|_S\not\equiv0$, and the existing maximal sections with their preceding height/barrier premises. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-harrison-normalization]] [[def-stationary-maximal-graph]] Work in ZFC, including [[math:def-axiom-of-choice]].

[F1] Under the nonzero stationary-field hypothesis in [A1], the authored reference collar is a smooth compact background family; the completed boundary theorem supplies the common one-to-one Gaussian graph domain of radius $r_\delta>0$, the strict cone, zero height on $S$ and the boundary angle bound. [[pthm-common-reference-collar]] [[pthm-boundary-normal-angle]] The full logarithmic angle inequality holds through all $v_q\ge1$. [[pthm-normal-angle-differential-inequality]]

[F2] The induced metric, maximality and scalar-operator conventions are [[def-spacelike-maximal-hypersurface-data]], and Holder norms are [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]].

[F3] The five helpers give the ambient cutoff estimates, weighted maximum argument, Gaussian graph equation, uniform extension/flattening and bootstrap from a boundary C1-Holder seed. [[lem-author-14de055b8ceb-gaussian-cutoff-projection]] [[lem-author-14de055b8ceb-weighted-cutoff-maximum]] [[lem-author-14de055b8ceb-gaussian-maximal-graph-operator]] [[lem-author-14de055b8ceb-uniform-elliptic-jet-extension]] [[lem-author-14de055b8ceb-boundary-seeded-schauder-bootstrap]].

[F4] Import Simon Lecture18 Theorems1–2, pp.216–217, for the local interior and homogeneous-Dirichlet boundary $C^{1,\beta}$ seed, with exact coefficient-box, forcing, gradient and flattening hypotheses recorded in the source entry. No interior-only estimate is used as a boundary estimate.

[F5] The complete preceding height/barrier premises in the Statement retain maximality on the actual original $C=\Sigma_0\cap\mathcal E$ and the selected-end access required for those height estimates. Use $\Sigma_1=C\cup S$ as the reference section of the common-collar contract; its topological spherical identification remains independent of the physical stationary end chart. The boundary-angle input is used only for its candidate graph, cone and boundary-angle conclusions under those full hypotheses. [[pthm-common-reference-collar]] [[pthm-boundary-normal-angle]]

## Proof

**Given:** The existing candidate family and supplied common collar, cone and full-range angle inequality. **Goal:** Establish the cutoff angle bound and all uniform higher collar estimates.

1.1 Use the actual original reference section and complete inherited hypotheses in [F5]. The compact smooth Gaussian background in [F1] has uniformly bounded reference distance derivatives. Since $c<1$ and $|dR_q|_{h_{q,0}}=1$, shrink the tube to make $c|dR_q|_{h_{q,\tau_q}}\le\gamma<1$ for all parameters. Choose the fixed radius $0<\rho_\delta<r_\delta$ in the Statement after this shrinking, so its closed cone region lies in this compact common tube and the collar of the full-range angle inequality. Smoothness and compactness of the reference family and the strict cone permit a positive choice independent of $q$ and of the candidates. The first helper in [F3] gives exactly the cutoff values, its positive-set gradient/Laplacian bounds and a fixed collar $R_q\le d/[2(c+\theta_\delta)]$ on which $\chi\ge1/2$. These facts concern fixed background derivatives and use only maximality for the Laplacian trace. [A1, F1, F2, F3, F5]

2.1 Restrict the common normal graph to the closed reference collar $0\le R_q\le\rho_\delta/2$. It is compact and individually smooth through $S$, so $\chi^mv_q$ attains a maximum there. Its outer value is zero and its value on $S$ has the uniform bound in [F1]. Apply the second helper in [F3] and the full-range differential inequality in [F1]. It supplies the displayed maximum-point formula and a common integer $m$ yielding $v_q\le C_\delta$ on $\chi\ge1/2$. The nonsmooth zero set of $\chi$ cannot contain a positive interior maximum, so differentiation across that set is unnecessary. [F1, F2, F3, step 1.1]

3.1 On a smaller fixed reference collar inside that region, the Gaussian graph equation in [F3] identifies $v_q=(1-|Du_q|_{h_{q,u_q}}^2)^{-1/2}$. The bound in step 2.1 gives a compact common spacelike slope cone and a uniform Euclidean gradient bound; the original cone gives a height bound. The third and fourth helpers in [F3] therefore provide smooth joint coefficients and a uniformly elliptic extension on a full containing jet box. Flatten the compact smooth fixed boundary with a finite common family of charts. The actual graph height is zero there. The forcing is bounded without any derivative of $Du_q$, so every hypothesis of [F4] is satisfied uniformly, including near $S$. Apply its boundary theorem and its interior counterpart to obtain a uniform $C^{1,\beta}$ bound on a smaller collar for some common $\beta>0$. [A1, F1, F2, F3, F4, step 2.1]

4.1 Use the fifth helper in [F3], now with the genuine boundary seed from step 3.1. Freeze the realized coefficients for the initial boundary Schauder gain and then differentiate tangentially and recover the remaining normal derivatives by the uniformly elliptic equation. This gives every finite uniform higher bound on a common smaller collar; one extra derivative yields any prescribed exponent $\alpha<1$. The angle bound already supplies uniform spacelikeness. This proves all the stated estimates, without assuming an initial uniform C4 norm or invoking a theorem restricted to interior patches. [F1, F2, F3, step 3.1] ∎

## Source notes

The cutoff argument follows the original method with its positive-set qualification made explicit. The higher-order step uses an independently sourced boundary C1-Holder estimate before applying local boundary Schauder estimates; individual smoothness alone is not substituted for a uniform estimate. The global weighted temporal theorem and exterior lapse maximum principles are not needed for this local collar argument. No original-article defect is asserted.

## External input

The local nonlinear boundary C1-Holder estimate is an imported input. Use Simon Lecture18 Theorem2, printed p.217 with (P), (*) and (**) on pp.216–217 (PDF sheet111): a classical C2 solution with zero Dirichlet trace, bounded height and gradient, bounded forcing, C1 joint coefficient bounds on a containing full jet box, positive uniform ellipticity and a uniformly C2-flattenable boundary has a controlled C1-beta norm on smaller patches for some beta in (0,1). Theorem1 is the interior counterpart. Exact hypotheses and reading limits are recorded in the source metadata. The fifth local helper supplies the subsequent boundary Schauder bootstrap; it does not stand in for this initial estimate.

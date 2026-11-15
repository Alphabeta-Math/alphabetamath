---
id: pthm-normal-angle-differential-inequality
title: Angle differential inequality near S
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - def-stationary-maximal-graph
  - pthm-harrison-electrovacuum
  - pthm-common-reference-collar
  - pthm-boundary-normal-angle
  - pthm-hawking-graph-height
  - pthm-hawking-graph-barriers
  - lem-author-840894718169-uniform-gaussian-flow-cone
  - def-spacelike-maximal-hypersurface-data
  - math:def-axiom-of-choice
  - lem-author-56ff511785bf-boost-frame-bounds
  - lem-author-56ff511785bf-local-angle-gauss-codazzi
  - lem-author-56ff511785bf-trace-free-angle-coercivity
  - lem-author-56ff511785bf-uniform-angle-laplacian
  - lem-author-56ff511785bf-full-range-log-angle
  - math:def-riemannian-gradient-of-a-smooth-function
  - math:def-laplace-beltrami-operator-as-trace-of-the-hessian
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  pthm-harrison-electrovacuum: physical-result
  pthm-common-reference-collar: physical-result
  pthm-boundary-normal-angle: physical-result
  pthm-hawking-graph-height: physical-result
  pthm-hawking-graph-barriers: physical-result
  lem-author-840894718169-uniform-gaussian-flow-cone: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  lem-author-56ff511785bf-boost-frame-bounds: mathematical-premise
  lem-author-56ff511785bf-local-angle-gauss-codazzi: mathematical-premise
  lem-author-56ff511785bf-trace-free-angle-coercivity: mathematical-premise
  lem-author-56ff511785bf-uniform-angle-laplacian: mathematical-premise
  lem-author-56ff511785bf-full-range-log-angle: mathematical-premise
  math:def-riemannian-gradient-of-a-smooth-function: mathematical-premise
  math:def-laplace-beltrami-operator-as-trace-of-the-hessian: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-altered
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p.4, Theorem 1.1 and Remark 1.2 (standing nonvanishing scope);
        pp.18–19, (3.12)–(3.13) and Gaussian collar setup
      reading_limits: "Attribution only, not an imported premise. Historical claim
        description: On the stated maximal normal graphs near S, U=-grad_{g_q}τ
        is unit future timelike, agrees with the reference normal on S, and the
        article states Δ_{h_q}log v≥¼|∇log v|²-Cδv² for v=-g_q(n_q,U)≥1.
        Historical scope: The original regular stationary vacuum/Harrison
        setting with T restricted to S not identically zero, mass one, maximal
        original exterior section, and existing smooth spacelike maximal
        candidate sections with q in a fixed interval [δ,1] and their preceding
        boundary height/barrier hypotheses. Attribution only. Retained reading
        record: Consulted the frozen original PDF images pp.4 and 19 and
        extracted text pp.4, 7–8, 12 and 17–19 in this adjudication. Theorem 1.1
        supplies the attributed scope; this citation is not an independent
        prerequisite proof. This maintenance revision checks current supplier
        contracts; no new original-PDF reading is claimed."
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum, arXiv:2610.09729v1
      url: https://arxiv.org/pdf/2610.09729v1
      locator: Appendix B, Lemma B.1, printed/PDF pp.35–36 (hypotheses); proof
        pp.38–39, (B.8)–(B.11)
      reading_limits: "Retained independent source-input/background reading record:
        Consulted actual v1 PDF text of Lemma B.1 on pp.35–36 and its proof on
        pp.38–39 in this adjudication; no images were read. Method attribution
        only. The all-range logarithmic conclusion is supplied by the locally
        proved helpers, not by this source. Current maintenance checks the
        stated contract and its local application, without claiming new
        external-proof or PDF reading."
      statement: "Method attribution: (B.8) differentiates the normal angle; Codazzi
        and trace-free algebra give the scalar and arcosh estimates
        (B.9)–(B.11), with the arcosh argument restricted to v>2."
      hypotheses: C2-convergent smooth Lorentz metrics near a compact set, a fixed
        smooth temporal function with uniformly timelike gradient, and smooth
        maximal hypersurfaces with compact nonnegative-height portions. These
        global hypotheses are not imported into the local logarithmic argument.
physical_scope: Conditional local differential estimate for the supplied smooth
  stationary vacuum/Harrison family and existing maximal graphs. The pointwise
  argument itself uses smooth Lorentzian geometry and maximality, not the field
  equations. No candidate-existence claim, observation or preliminary uniform
  bound on its second fundamental form is asserted.
dependency_level: 18
---

## Statement

In the regular mass-one stationary vacuum/Harrison construction with $T|_S\not\equiv0$, fix $\delta>0$ and the existing smooth spacelike maximal stationary sections $\Sigma_q$, $q\in[\delta,1]$, with the complete preceding boundary height and barrier hypotheses. On a sufficiently small common Gaussian collar of the bifurcation sphere $S$, let $\tau_q$ be future proper time along the normal geodesics of the reference section, let $U_q=-\operatorname{grad}_{g_q}\tau_q$, and put $v_q=-g_q(n_q,U_q)$ for the future candidate normal $n_q$. Then $U_q$ is unit future timelike, $v_q\ge1$, and with $h_q=g_q|_{T\Sigma_q}$ one has $\Delta_{h_q}\log v_q\ge\tfrac14|\nabla^{h_q}\log v_q|_{h_q}^2-C_\delta v_q^2$ throughout the candidate collar, including $1\le v_q\le2$. The constant and collar are independent of the candidates and of $q\in[\delta,1]$. On $S$, $U_q=\bar n_q$ and the previously established boundary boost bound gives $v_q\le C_\delta$. This is a differential estimate, not yet an interior upper bound for $v_q$.

## Facts & Assumptions

[A1] Adopt the supplied stationary vacuum model, regular data, mass-one normalization and existing maximal graph sections, and assume $T|_S\not\equiv0$; no eventual section-existence theorem is assumed. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-harrison-normalization]] [[def-stationary-maximal-graph]] Work in ZFC. [[math:def-axiom-of-choice]]

[F1] Under [A1], the Harrison metrics are jointly smooth in spacetime and $q$ on one open neighborhood of $S$. [[pthm-harrison-electrovacuum]] The reference collar, induced metric and unit normal data are smooth and uniformly controlled on smaller compact collars. [[pthm-common-reference-collar]]

[F2] With the uniform Hawking-flow height bound from [F9], the completed boundary theorem gives the common one-to-one Gaussian normal graph domain, the cone bound and the boundary normal-angle estimate. [[pthm-boundary-normal-angle]] Its Gaussian-flow helper constructs the normal coordinate family smoothly with one common compact parameter domain. [[lem-author-840894718169-uniform-gaussian-flow-cone]]

[F3] Spacelike normals, maximality and $k=-g_q(Dn_q,\cdot)$ have their stated mathematical conventions. [[def-spacelike-maximal-hypersurface-data]]

[F4] The five local mathematical inputs give observer-frame bounds, exact Gauss–Codazzi angle differentiation, trace-free coercivity, uniform scalar estimates and the all-range logarithmic inequality. [[lem-author-56ff511785bf-boost-frame-bounds]] [[lem-author-56ff511785bf-local-angle-gauss-codazzi]] [[lem-author-56ff511785bf-trace-free-angle-coercivity]] [[lem-author-56ff511785bf-uniform-angle-laplacian]] [[lem-author-56ff511785bf-full-range-log-angle]]

[F5] For the induced Riemannian metric $h_q$, the intrinsic gradient is characterized by $h_q(\nabla^{h_q}f,X)=df(X)$ for tangent $X$. [[math:def-riemannian-gradient-of-a-smooth-function]]

[F6] The intrinsic Laplacian uses the positive-divergence convention $\Delta_{h_q}f=\operatorname{tr}_{h_q}\operatorname{Hess}_{h_q}f=\operatorname{div}_{h_q}(\nabla^{h_q}f)$, with the one-sided extension for data smooth up to the boundary. [[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]]

[F7] The complete preceding boundary height/barrier hypotheses in the Statement are retained, including their actual original exterior-section maximality and selected-end access premises. The original maximality is $H_g=0$ on $C=\Sigma_0\cap\mathcal E$, and the original reference section is $\Sigma_1=C\cup S$, as specified by the common-collar contract. The independent spherical identification is not equated with the physical stationary end chart. These are inherited hypotheses for the candidate estimate, not consequences of regularity or candidate existence. [[pthm-common-reference-collar]] [[pthm-boundary-normal-angle]]

[F8] The complete preceding height/barrier hypotheses in the Statement are those of the Hawking-height and barrier suppliers, for the same stationary product and selected single-primitive Harrison family. The supplied candidates are connected smooth spacelike maximal sections, smooth up to compact boundary $S$, with one exterior end and interiors the stationary graphs over $\Sigma_1^\circ$. Retain all their candidate-section, normalized-end and uniform-estimate hypotheses, including the radial height-decay and transformed-lapse hypotheses: normalized end heights and their first spatial derivatives tend to zero uniformly in direction for each fixed $q$, the required estimates hold on a common end with constants independent of $q\in[\delta,1]$, and $-g_q(T,n_q)>0$ in the interior. In addition to the actual original-section maximality in [F7], the selected-end access premise means that for some $R_a$ and every $R\ge R_a$, with $U_R=\mathbb R\times\{r>R\}$ in the physical stationary end chart, $\mathcal E\subset I^-_{(\mathcal E,g)}(U_R)\cap I^+_{(\mathcal E,g)}(U_R)$, with both witnessing timelike paths in the unchanged original exterior. These are the inherited complete height/barrier premises, not conclusions of regularity or candidate existence. [[pthm-hawking-graph-height]] [[pthm-hawking-graph-barriers]]

[F9] Under these matched hypotheses, the Hawking-height theorem supplies the unique Hawking-flow height $u_q^K$, smooth individually up to $S$. The barrier theorem supplies $\sup_{0\le\rho_q\le\rho_0}|u_q^K|\le B_\delta$ on one common closed reference collar, including $S$, with $B_\delta$ independent of the candidates and of $q\in[\delta,1]$. No uniform derivative bound for these heights is assumed. [[pthm-hawking-graph-height]] [[pthm-hawking-graph-barriers]]

## Proof

**Given:** The conditional model and supplied smooth family, collar and candidate sections. **Goal:** Prove the all-range differential inequality with one uniform collar constant.

1.1 Match the height/barrier contracts before using the boundary theorem. The actual original reference section is the one in [F7]; [A1] supplies its standing nonvanishing scope, and [F8] supplies the same stationary product, selected single-primitive family, complete candidate/end hypotheses, uniform estimates and two-sided original-metric far-end access. The Hawking-height result therefore gives the unique heights and their individual smooth extensions through $S$ in [F9]. Apply the barrier result with precisely these hypotheses to obtain the bound $|u_q^K|\le B_\delta$ on the common closed reference collar, including $S$. This provides the uniform height premise of the boundary theorem in [F2]; that theorem now gives the common candidate graph domain, cone and boundary boost bound. No eventual candidate-existence theorem or normal-angle estimate is used to obtain this height bound. [A1, F1, F2, F7, F8, F9]

2.1 Retain the full preceding hypotheses and actual reference-section binding in [F7]. The nonvanishing hypothesis in [A1] meets the corresponding premise of both suppliers in [F1]. By [F1]–[F2], choose a smaller common closed Gaussian coordinate cylinder with its image in the smooth background neighborhood. Its parameter set, including $q\in[\delta,1]$ and the reference base points in a closed collar of compact $S$, is compact. In these coordinates $g_q=-d\tau_q^2+h_{q,\tau_q}$ and $U_q=\partial_{\tau_q}=-\operatorname{grad}_{g_q}\tau_q$. Thus $U_q$ is smooth, future unit timelike. Smoothness of the background Gaussian maps and metrics gives common bounds for $D^{(q)}U_q$, $(D^{(q)})^2U_q$ and $\operatorname{Ric}(g_q)$ in the positive metrics $e_q=g_q+2U_q^\flat\otimes U_q^\flat$, using a finite cover. The inverse positive metric norms are bounded as well by compactness and positive definiteness. These are background bounds and use no derivative of a candidate graph. [A1, F1, F2, F3, F4, F7, step 1.1]

3.1 Each candidate in this tube is smooth spacelike and maximal by [A1]–[F3]. Apply the all-range local theorem in [F4] with the background bound from step 2.1. It gives exactly the displayed inequality for every $v_q\ge1$, uniformly in the family. The local derivation divides only by $v_q\ge1$, so no missing passage through $v_q=1$ or $1\le v_q\le2$ remains. It requires no compactness of a positive-height candidate portion and makes no use of a fixed temporal function across $q$. On $S$, [F2] identifies $U_q$ with the reference normal and supplies the uniform boundary boost bound. This proves the statement on the common collar and its individually smooth boundary. [A1, F2, F3, F4, step 1.1, step 2.1] ∎

## Source notes

Radu Appendix B (B.8)–(B.10) motivates the local differentiation and trace-free argument. Its arcosh inequality is restricted to $v>2$; the five local helpers instead retain the smooth angle v and derive the log inequality by division by v alone. No external all-v theorem is invented. The separate weighted-normal theorem, its compact nonnegative-height portions and its fixed-temporal-function hypotheses are not invoked. The Gaussian compact family supplies local coefficient bounds directly. No Einstein–Maxwell energy condition is needed for this kinematic differential calculation, since the ambient Ricci tensor is estimated as a bounded background tensor.

---
id: thm-maximal-normal-angle-estimate-input
title: Temporal cutoff estimate for normals to maximal hypersurfaces
kind: theorem
status: published
origin: pipeline
domain: mathematics
deps:
  - def-spacelike-maximal-hypersurface-data
  - def-causal-exterior-and-boundary-data
  - math:def-axiom-of-choice
  - math:def-real-power
  - def-author-fd2999663761-temporal-angle-data
  - lem-author-fd2999663761-temporal-tangent-gradient
  - lem-author-fd2999663761-logarithmic-angle-conversion
  - lem-author-fd2999663761-compact-weighted-maximum
  - lem-author-fd2999663761-cutoff-interior-maximum-exclusion
dependency_roles:
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-real-power: mathematical-premise
  def-author-fd2999663761-temporal-angle-data: mathematical-premise
  lem-author-fd2999663761-temporal-tangent-gradient: mathematical-premise
  lem-author-fd2999663761-logarithmic-angle-conversion: mathematical-premise
  lem-author-fd2999663761-compact-weighted-maximum: mathematical-premise
  lem-author-fd2999663761-cutoff-interior-maximum-exclusion: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum, arXiv:2610.09729v1
      url: https://arxiv.org/pdf/2610.09729v1
      locator: Appendix B, Lemma B.1 and (B.1), PDF/printed pp.35–36; proof
        (B.8)–(B.12), pp.38–39, especially (B.11)
      statement: In a time-oriented Lorentzian four-manifold, for smooth Lorentz
        metrics g_j converging in C2 near a fixed compact Q, a fixed smooth τ
        with past timelike g_j-gradient and α_j²=-g_j^{-1}(dτ,dτ)≥a0²>0 on
        Q∩{τ≥0}, and smooth spacelike maximal Σ_j with future unit normals whose
        entire portions Σ_j∩{τ≥0} are compact and contained in Q, put
        V_j=-α_j^{-1}grad_{g_j}τ and v_j=-g_j(n_j,V_j). There is a uniform C
        such that, on {v_j>2}, η_j=arcosh v_j satisfies
        Δ_{Σ_j}η_j≥cothη_j(¼|∇_{Σ_j}η_j|²-Cv_j²) and |Δ_{Σ_j}τ|≤Cv_j². The
        constant is controlled by a0, the uniform coordinate C2 metric/C0
        inverse bounds and the coordinate C3 norm of τ. Lemma B.1 concludes sup
        τ^μ v_j≤2 max{2τmax^μ,sup_{∂Σ_j∩{τ>0}}τ^μ v_j} for some μ>4 controlled
        by the same geometry. The empty boundary supremum is zero.
      hypotheses: Common time orientation, signature (-,+,+,+), spacetime dimension
        four; fixed finite coordinate cover near Q; uniform C2 bounds for g_j,
        C0 bounds for inverses, and C3 bounds for fixed τ; past timelike
        gradient with the stated lower norm bound; smooth spacelike maximal
        hypersurfaces and future unit normals, smooth up to their actual
        boundaries; entire nonnegative-height portions compact and contained in
        Q. No vacuum or field equation, stationary-graph representation, or
        boundary-angle bound is presumed; actual boundary terms are retained.
      reading_limits: Read the v1 PDF text of Lemma B.1 and (B.1) on printed/PDF
        pp.35–36 and its proof (B.8)–(B.12) on pp.38–39 through web PDF
        retrieval during this repair. Checked the imported inequalities,
        geometric hypotheses, constant dependence and actual-boundary term
        against those passages. Page-image retrieval was unavailable. The
        tensor/coefficient estimates leading to (B.11) are imported established
        input and were not independently reconstructed. The local conversion and
        maximum lemmas and their application below supply the locally composed
        argument; they do not reconstruct those tensor estimates.
dependency_level: 5
---

## Statement

Let $g_j$ be smooth time-oriented Lorentz metrics of signature $(-,+,+,+)$ on a common smooth four-manifold, converging in $C^2$ to a Lorentz metric near a fixed compact set $Q$. Use a common time orientation and a fixed finite coordinate cover near $Q$, with uniformly bounded metric $C^2$ and inverse-metric $C^0$ norms. Let $\tau$ be a fixed smooth function, with past-directed timelike $g_j$-gradient and $\alpha_j^2=-g_j^{-1}(d\tau,d\tau)\ge a_0^2>0$ on $Q\cap\{\tau\ge0\}$. Let $\Sigma_j$ be smooth spacelike maximal hypersurfaces, smooth up to their actual boundaries, with future unit normals $n_j$, such that the entire portions $\Sigma_j\cap\{\tau\ge0\}$ are compact and contained in $Q$. Set $V_j=-\alpha_j^{-1}\operatorname{grad}_{g_j}\tau$, $v_j=-g_j(n_j,V_j)$ and $\tau_{\max}=\max_Q\max(\tau,0)$ when $Q$ is nonempty, and $\tau_{\max}=0$ when $Q=\varnothing$. There is $\mu>4$, depending only on $a_0$, the uniform metric and inverse bounds and $\|\tau\|_{C^3(Q)}$ in that cover, such that $\sup_{\Sigma_j\cap\{\tau>0\}}\tau^\mu v_j\le2\max\{2\tau_{\max}^{\mu},\ \sup_{\partial\Sigma_j\cap\{\tau>0\}}\tau^\mu v_j\}$. A supremum over an empty set is zero. In particular the boundary supremum is retained unless it is empty or separately bounded. No uniform bound on the normals is assumed in advance.

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice. [[math:def-axiom-of-choice]]

[F1] The meanings of spacelike, future normal and maximality are [[def-spacelike-maximal-hypersurface-data]]; past timelike gradient and temporal function have the convention of [[def-causal-exterior-and-boundary-data]]. The temporal angle, operator and compact-portion conventions are [[def-author-fd2999663761-temporal-angle-data]].

[F2] The temporal gradient identity is [[lem-author-fd2999663761-temporal-tangent-gradient]]; the conversion of a hyperbolic-angle differential inequality to the logarithmic one on $\{v>2\}$ is [[lem-author-fd2999663761-logarithmic-angle-conversion]].

[F3] The compact weighted maximum and interior exclusion lemmas are [[lem-author-fd2999663761-compact-weighted-maximum]] and [[lem-author-fd2999663761-cutoff-interior-maximum-exclusion]].

[F4] Use the exact external differential estimate in the following External input section, under the complete geometric hypotheses of the Statement.

[F5] Positive-base real powers are $a^r=\exp(r\log a)$ for $a>0$ and real $r$; the supplementary convention is $0^r=0$ for $r>0$. [[math:def-real-power]]

## External input

Import (B.11) of Radu, Appendix B: with the geometric hypotheses of the Statement and $\eta_j=\operatorname{arcosh}v_j$, there is a uniform $C\ge1$ such that on $\{v_j>2\}$, $\Delta_{\Sigma_j}\eta_j\ge\coth\eta_j(\tfrac14|\nabla_{\Sigma_j}\eta_j|^2-Cv_j^2)$ and $|\Delta_{\Sigma_j}\tau|\le Cv_j^2$. Its constant depends only on $a_0$, the stated uniform coordinate metric/inverse bounds and the $C^3$ norm of $\tau$. This is an external geometric differential estimate, not a local reconstruction. The source derives it from (B.8)–(B.10) using Gauss–Codazzi, maximality and the trace-free eigenvalue bound in three tangent dimensions; the present proof imports that step with all its hypotheses.

## Proof

**Given:** The sequence, compact portions and temporal function in the Statement, with imported differential estimate [F4].

**Goal:** Prove the stated uniform weighted angle bound.

1.1 The temporal data are well defined by [F1]. If $\tau_{\max}=0$, including when $Q=\varnothing$, containment of the entire nonnegative-height portions in $Q$ implies that the positive-height sets are empty, so the conclusion holds for any fixed $\mu>4$ by the zero-supremum convention. Otherwise put $T=\tau_{\max}>0$. By [F4] choose a common $C\ge1$ for both differential estimates. By [F2] its hyperbolic-angle inequality gives $\Delta\log v_j\ge\tfrac14|\nabla\log v_j|^2-Cv_j^2$ on $\{v_j>2\}$, and $|\nabla\tau|^2\ge a_0^2(v_j^2-1)$. [F1, F2, F4, F5, given]

2.1 Choose a common $\mu>4$ so that $(\mu^2/4-\mu)a_0^2\ge2C(T^2+\mu T)$. The exclusion lemma [F3] rules out a local interior maximum of $\tau^\mu v_j$ at positive height with $v_j>2$. The compact maximum lemma [F3] then gives $\sup\tau^\mu v_j\le\max\{2T^\mu,B_j\}\le2\max\{2T^\mu,B_j\}$, where $B_j$ is exactly the actual boundary supremum in the Statement. The choice of $\mu$ uses only the uniform geometric constant, $a_0$ and $T$, itself bounded by the specified $C^3$ norm. This proves the stated bound for every $j$ with all boundary terms intact. [F2, F3, F5, step 1.1, algebra] ∎

## Source notes

The scalar argument follows the maximum-principle method of Radu, Appendix B, (B.11)–(B.12), using the explicitly proved conversion to log v and retaining the source’s conservative stated constant. The independent source is not the article under study. No graph existence, temporal-function existence, boundary-angle estimate or tensor-identity reconstruction is asserted. The compact sets must contain the entire nonnegative-height portions; replacing them by intersections with an arbitrary compact Q would introduce extra boundary terms.

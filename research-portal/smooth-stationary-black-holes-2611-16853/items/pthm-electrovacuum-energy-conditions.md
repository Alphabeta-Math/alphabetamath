---
id: pthm-electrovacuum-energy-conditions
title: Energy-condition inputs for the transformed geometry
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - pthm-harrison-electrovacuum
  - pthm-harrison-lorentzian-algebra
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - lem-geometric-maxwell-convergence-input
  - def-source-free-geometric-electrovacuum-data
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - math:def-axiom-of-choice
dependency_roles:
  pthm-harrison-electrovacuum: physical-result
  pthm-harrison-lorentzian-algebra: physical-result
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  lem-geometric-maxwell-convergence-input: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 6, 13, 25–27; §§1.4, 3.1 and 4
      statement: The article invokes dominant energy for the transformed
        zero-parameter geometry, a nonnegative maximal-slice potential, and
        Raychaudhuri arguments in the transformed geometries.
      hypotheses: The article's regular stationary vacuum construction and the
        parameter and geometric hypotheses of the respective passages.
      reading_limits: Read the frozen article text at the cited passages. This
        reference records attribution and is not used to prove the energy
        inequalities or the Raychaudhuri applications.
physical_scope: Conditional deductions in the four-dimensional stationary vacuum
  model and its source-free Einstein–Maxwell Harrison family; no measurement or
  existence of a candidate slice is asserted.
dependency_level: 10
---

## Statement

Adopt the regular stationary vacuum construction with the original exterior section maximal, $T|_S\not\equiv0$, and mass normalized to one. Let $(g_q,F_q)$ be its Harrison family for $q\in[0,1]$, on the exterior $E$ and the supplied open neighborhood $O$ of the bifurcation sphere $S$. Assume the Axiom of Choice. All contractions and causal character below use $g_q$.

Use the original smooth future timelike field $N$ to orient each transformed metric by $N_q^{\mathrm{or}}=A_q^{-1}N$, where $A_qv=v+D_q^{-1}W_q(v)T$ is the Harrison tangent map for this same family. This field is smooth and $g_q$-timelike on $E\cup O$, and agrees with $N$ at $q=1$. Future timelike vectors below satisfy $g_q(v,N_q^{\mathrm{or}})<0$; future causal vectors use the corresponding closed cone.

Define $Q^{(q)}_{ab}=(F_q)_{ac}(F_q)_b{}^c-\frac14(g_q)_{ab}(F_q)_{cd}(F_q)^{cd}$. For every future timelike vector $v$, the vector $-(Q^{(q)})^a{}_b v^b$ is future causal or zero. Thus the Maxwell tensor has the dominant energy condition, in particular for $g_0$. For every unit timelike vector $n$ and every nonzero null vector $L$, $\operatorname{Ric}(g_q)(n,n)\ge0$ and $\operatorname{Ric}(g_q)(L,L)\ge0$.

Consequently, on any supplied smooth spacelike maximal candidate section for $g_q$, with future unit normal $n_q$, induced positive-definite metric $h_q$ and second fundamental form $k_q$, the potential $|k_q|_{h_q}^2+\operatorname{Ric}(g_q)(n_q,n_q)$ is nonnegative. This applies in particular for $q\in[\delta,1]$ when $\delta>0$ and the indicated section exists. The null inequality is the null-convergence input used in the article's Raychaudhuri area-comparison and focusing arguments; it does not by itself assert those arguments' additional hypotheses or conclusions.

## Facts & Assumptions

[A1] The physical model and regular stationary vacuum hypotheses, original maximal section and mass-one normalization are those of [[post-stationary-vacuum-model]], [[def-regular-stationary-vacuum-spacetime]], [[def-spacelike-maximal-hypersurface-data]] and [[def-harrison-normalization]]. The Axiom of Choice is assumed. [[math:def-axiom-of-choice]]

[F1] Under these hypotheses, the Harrison construction gives the smooth Lorentzian metrics and smooth spacetime two-forms satisfying the source-free Einstein–Maxwell equations on $E\cup O$ for each $q\in[0,1]$. Its regular Harrison data have positive denominators on this common domain, and $(g_1,F_1)=(g,0)$. [[pthm-harrison-electrovacuum]]

[F2] A source-free geometric electrovacuum datum has a time-oriented Lorentzian metric of signature $(-,+,+,+)$, a real two-form, and the equation $\operatorname{Ric}=2Q$ with the displayed Maxwell tensor. [[def-source-free-geometric-electrovacuum-data]]

[F3] For such a datum, Maxwell algebra gives the dominant energy condition for $Q$, nonnegative Ricci contraction on unit timelike vectors, and nonnegative Ricci contraction on nonzero null vectors. [[lem-geometric-maxwell-convergence-input]]

[F4] A spacelike section has positive-definite induced metric, a future unit normal and a second fundamental form. Maximal means that its mean curvature vanishes. [[def-spacelike-maximal-hypersurface-data]]

[F5] For these same regular Harrison data on $D_q>0$, the algebraic supplier defines $A_qv=v+D_q^{-1}W_q(v)T$ and proves $g_q=(D_q/4)A_q^*g$ and smooth invertibility of $A_q$. For the original smooth timelike field $N$, it proves that $A_q^{-1}N$ is a smooth transformed time orientation, with the future-cone correspondence and $A_1=I$ for the single-potential family. [[pthm-harrison-lorentzian-algebra]]

## Proof

**Given:** The construction and candidate-section hypotheses in the Statement.

**Goal:** Prove the stated energy and convergence inequalities and the nonnegativity of the potential.

1.1 Fix $q\in[0,1]$ and use the regular positive-denominator Harrison data on $E\cup O$ from [F1]. They satisfy the hypotheses of [F5] for the same $g_q$ and $W_q$. In particular $N_q^{\mathrm{or}}=A_q^{-1}N$ is a smooth field and $g_q(N_q^{\mathrm{or}},N_q^{\mathrm{or}})=(D_q/4)g(N,N)<0$. Also $g_q(v,N_q^{\mathrm{or}})=(D_q/4)g(A_qv,N)$, so this field defines precisely the future convention in the Statement. At $q=1$, $A_1=I$ gives the original time orientation. Thus no assumption that the original field $N$ itself stays timelike for $g_q$ is needed. [A1, F1, F5, algebra]

2.1 Keep the original manifold orientation and use the time-orientation field constructed in step 1.1. The equations and spacetime regularity in [F1] now make $(E\cup O,g_q,N_q^{\mathrm{or}},o,F_q)$ a source-free geometric electrovacuum datum in [F2], with every index operation taken using $g_q$. Applying [F3] gives the future-causal or zero energy current and the timelike and null Ricci inequalities at each point. The argument includes $q=0$ and requires no limiting passage. [A1, F1, F2, F3, step 1.1]

3.1 On a supplied candidate section, its induced metric is positive definite. In an $h_q$-orthonormal tangent frame, $|k_q|_{h_q}^2$ is a sum of squares and hence is nonnegative. Its future unit normal is timelike, so the Ricci term is nonnegative by step 2.1. Their sum is therefore nonnegative, including throughout the stated positive-parameter range whenever the section exists. The same step supplies null convergence wherever the article additionally invokes a valid Raychaudhuri argument. [F4, step 2.1, algebra] ∎

## Source notes

The article citation attributes the uses described above. The proof uses the completed construction, the locally proved Harrison pullback time orientation, and the Maxwell-algebra supplier; it does not derive the Raychaudhuri equation, area comparison, focusing, or existence of the candidate sections.

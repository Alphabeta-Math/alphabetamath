---
id: lem-author-45355d85383b-second-form-and-jacobi-potential
title: The graph second form and electrovacuum Jacobi potential have weighted
  order four
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-45355d85383b-induced-metric-and-normal-decay
  - lem-author-45355d85383b-weighted-fifth-graph-derivative
  - def-source-free-geometric-electrovacuum-data
  - def-spacelike-maximal-hypersurface-data
  - def-weighted-holder-spaces
  - lem-author-45355d85383b-stationary-maximal-flux-formula
  - lem-author-45355d85383b-scaled-decay-holder-upgrade
  - math:def-axiom-of-choice
dependency_roles:
  lem-author-45355d85383b-induced-metric-and-normal-decay: mathematical-premise
  lem-author-45355d85383b-weighted-fifth-graph-derivative: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-weighted-holder-spaces: mathematical-premise
  lem-author-45355d85383b-stationary-maximal-flux-formula: mathematical-premise
  lem-author-45355d85383b-scaled-decay-holder-upgrade: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 5
---

## Statement

Work in ZFC. Fix $0<\alpha<1$. Let $(M,g,N,o,F)$ be a smooth source-free geometric electrovacuum datum of signature $(-,+,+,+)$ with zero cosmological constant. On a normalized stationary Cartesian end $(t,x)$, with $r=|x|>R_0>0$, assume that $g$ and $F$ are independent of $t$, that $\partial_t$ is future timelike sufficiently far out, and that $g_{00}+1,g_{ij}-\delta_{ij}=O_5(r^{-1})$ and $g_{0i}=O_5(r^{-2})$. Here $O_5(r^{-b})$ means $|D^jf|\le C_jr^{-b-j}$ for Cartesian spatial derivatives $0\le j\le5$, outside a common radius; spatial indices run from $1$ to $3$ and are summed when repeated.

Let $\Sigma$ be a supplied smooth spacelike hypersurface, smooth up to its compact boundary if present, consisting of a compact core and an end given by the smooth maximal graph $t=u(x)$ with $|D^ju|\le Cr^{-3/4-j}$ for $0\le j\le4$. Assume the ambient data are smooth on a neighborhood of the compact core, and that the stationary electromagnetic coordinate components satisfy $F\in C^{2,\alpha}_{-2}$ on the end. All weighted spaces use the componentwise scaled-annulus norm and fixed compact-core chart norms. No existence of this graph is asserted.

Let $h$ be the induced positive-definite metric, $n$ the future unit timelike normal and $k(U,W)=-g(\nabla_U n,W)$ the second fundamental form. Then $k\in C^{2,\alpha}_{-11/4}$ and $V=|k|_h^2+\operatorname{Ric}(g)(n,n)\in C^{2,\alpha}_{-4}$. If timelike convergence holds, meaning $\operatorname{Ric}(g)(X,X)\ge0$ for every timelike tangent vector $X$ at every point of $\Sigma$, then $V\ge0$. Smoothness on the compact part completes these weighted statements globally.

## Statement references

[[lem-author-45355d85383b-induced-metric-and-normal-decay]]

[[lem-author-45355d85383b-weighted-fifth-graph-derivative]]

[[def-source-free-geometric-electrovacuum-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-weighted-holder-spaces]]

[[lem-author-45355d85383b-stationary-maximal-flux-formula]]

[[lem-author-45355d85383b-scaled-decay-holder-upgrade]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

[F1] The graph normal has weighted order-four control and the induced metric has a controlled inverse. [[lem-author-45355d85383b-induced-metric-and-normal-decay]]

[F2] Graph derivatives through weighted order five are controlled. [[lem-author-45355d85383b-weighted-fifth-graph-derivative]]

[F3] The geometric Einstein–Maxwell equation is quadratic in the field, with all contractions using the ambient metric. [[def-source-free-geometric-electrovacuum-data]]

[F4] The second fundamental form is the tangential covariant derivative of the future normal, with the fixed sign convention. [[def-spacelike-maximal-hypersurface-data]]

[F5] Weighted Hölder norms use Cartesian derivative weights and the top-derivative Hölder seminorm on rescaled annuli, applied componentwise to finite arrays, together with fixed compact-core chart norms. [[def-weighted-holder-spaces]]

[F6] The stationary background hypotheses are those of the flux supplier. Its normal formula is $n=-g^{-1}d(t-u)/\sqrt Q$, where $Q=-g^{00}+2g^{0i}u_i-g^{ij}u_iu_j$; its Proof 1.2 gives $g^{-1}-\eta=O_5(r^{-1})$ and $g^{i0}=O_5(r^{-2})$, with $\eta=\operatorname{diag}(-1,1,1,1)$. [[lem-author-45355d85383b-stationary-maximal-flux-formula]]

[F7] One extra pointwise derivative gives the eventual scaled Hölder bound at the preceding derivative order, also componentwise and at lower derivative orders. [[lem-author-45355d85383b-scaled-decay-holder-upgrade]]

[A1] ZFC includes the Axiom of Choice. This assumption is carried when invoking [F1] and [F2] in step 1.1 and the geometric electrovacuum convention in step 3.1; the local finite tensor and product computations add no choice requirement. [[math:def-axiom-of-choice]]

## Proof

**Given:** The metric, field, graph, compact-core, decay and ZFC hypotheses in the Statement.

**Goal:** Establish the second-form and potential estimates and the conditional sign.

1.1 Under [A1], the hypotheses match [F1] and [F2], giving $Du\in C^{4,\alpha}_{-7/4}$, $D^2u\in C^{3,\alpha}_{-11/4}$, a controlled induced inverse, and bounded normal components with four weighted Hölder derivatives. Apply [F7] to the metric bounds and the inverse bounds in [F6]. They give metric and inverse errors in $C^{4,\alpha}_{-1}$ and mixed components in $C^{4,\alpha}_{-2}$. Products add weights: on each fixed rescaled annulus, use the Leibniz rule and $[ab]_\alpha\le\|a\|_\infty[b]_\alpha+\|b\|_\infty[a]_\alpha$ for each differentiated term. The Christoffel formula $\Gamma^a_{bc}=\tfrac12g^{ad}(\partial_bg_{dc}+\partial_cg_{db}-\partial_dg_{bc})$, obtained from metric compatibility and torsion freedom, therefore gives $\Gamma^a_{bc}\in C^{2,\alpha}_{-2}$. Stationarity further gives $\Gamma^0_{ij}=\tfrac12g^{00}(\partial_i g_{0j}+\partial_j g_{0i})+\tfrac12g^{0\ell}(\partial_i g_{\ell j}+\partial_j g_{\ell i}-\partial_\ell g_{ij})\in C^{2,\alpha}_{-3}$. In particular the zero-slope term has stronger decay than a general connection component. [given, A1, F1, F2, F4, F5, F6, F7, algebra]

2.1 Put $e_i=\partial_i+u_i\partial_t$. Metric compatibility and $g(n,e_j)=0$ give $k_{ij}=g(n,\nabla_{e_i}e_j)$ in the sign convention [F4]. By [F6], $g(n,\cdot)=-d(t-u)/\sqrt Q$, and [F1] and [F6] imply that $Q$ tends to one and that $Q^{-1/2}$ is bounded with controlled derivatives through order two. The second-derivative part of $\nabla_{e_i}e_j$ contributes $-u_{ij}/\sqrt Q$. Its connection part with no slope factor contributes $-\Gamma^0_{ij}/\sqrt Q$; every other term has at least one factor $Du$ multiplying a connection coefficient. Step 1.1 bounds these contributions respectively in $C^{2,\alpha}_{-11/4}$, $C^{2,\alpha}_{-3}$ and $C^{2,\alpha}_{-15/4}$ or faster. The product inequality in step 1.1 proves $k\in C^{2,\alpha}_{-11/4}$ on the end. [F1, F4, F5, F6, step 1.1, algebra]

3.1 Under [A1], the defining equation in [F3] is $\operatorname{Ric}_{ab}=2(F_{ac}g^{cd}F_{bd}-\tfrac14g_{ab}F_{cd}g^{ce}g^{df}F_{ef})$. Its two field factors lie in $C^{2,\alpha}_{-2}$, while step 1.1 controls the metric and inverse factors, so the same differentiated product inequality gives Ricci components in $C^{2,\alpha}_{-4}$. The bounded normal components in [F1] preserve this weight upon contraction. Also $|k|_h^2=h^{ia}h^{jb}k_{ij}k_{ab}\in C^{2,\alpha}_{-11/2}$ by [F1] and step 2.1. Since $r^{-11/2}$ decays faster than $r^{-4}$, this implies the claimed order for $V$. Positive definiteness of $h$ makes $|k|_h^2$ nonnegative. The explicitly defined timelike-convergence condition applies to the unit timelike $n$, so it makes the other term nonnegative as well. Finally the assumed smooth spacelike extension over the compact core, including any compact boundary, makes $h^{-1}$, $k$, $n$ and the Ricci contraction smooth there; their norms on the fixed compact chart subsets are finite. This completes both global weighted claims and the conditional sign. [given, A1, F1, F3, F4, F5, step 1.1, step 2.1, algebra] ∎

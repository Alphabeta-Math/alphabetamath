---
id: pthm-annular-schauder-decay
title: Rescaled annular estimates through four derivatives
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - pthm-radial-barrier-height-decay
  - pthm-maximal-graph-equation
  - pthm-end-lapse-slope
  - pthm-transformed-end-geometries
  - def-stationary-maximal-graph
  - def-stationary-asymptotic-decay-data
  - lem-annular-quasilinear-bootstrap-input
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - math:def-axiom-of-choice
dependency_roles:
  pthm-radial-barrier-height-decay: physical-result
  pthm-maximal-graph-equation: physical-result
  pthm-end-lapse-slope: physical-result
  pthm-transformed-end-geometries: physical-result
  def-stationary-maximal-graph: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  lem-annular-quasilinear-bootstrap-input: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 15, §3.2.1, Schauder display after (3.7)
      attribution: The article states the uniform rescaled annular estimate through
        four derivatives and obtains decay of order three quarters plus
        derivative order from its height estimate.
      hypotheses: The stationary vacuum construction, the assumed candidate maximal
        sections, and a fixed positive parameter interval in the cited passage.
      reading_limits: The frozen article text at the cited passage was read for
        attribution. The article's claim is not used as a proof premise.
physical_scope: Conditional geometric consequence for the supplied stationary
  vacuum construction and its transformed metrics; candidate sections are
  assumed to exist and no observation is asserted.
dependency_level: 15
---

## Statement

Fix $\delta\in(0,1)$. Assume the candidate family and normalized stationary Cartesian ends of [[pthm-maximal-graph-equation]], including the common differentiated metric estimates and slope estimate stated there. The sections are assumed to exist and are smooth, spacelike and maximal. In the coordinates $(t_q,x_q)$ write $r_q=|x_q|$ and $u_q=\widetilde u_q$ for the normalized graph height defined in [[def-stationary-maximal-graph]]. Constants and threshold radii below may depend on $\delta$ but are independent of $q\in[\delta,1]$.

There are $R_\delta$ and $C_\delta$ such that, for all $R\ge R_\delta$ and $q\in[\delta,1]$,
$$\sum_{j=0}^4R^j\sup_{R<r_q<2R}|D_{x_q}^ju_q|\le C_\delta\left(\sup_{R/2<r_q<4R}|u_q|+R^{-1}\right).$$
Here $D^j$ denotes the finite array of Cartesian partial derivatives of total order $j$, with $D^0u_q=u_q$. The $R^{-1}$ term is the rescaled contribution of the $O(r_q^{-3})$ zero-slope forcing. Consequently, for $0\le j\le4$, $|D_{x_q}^ju_q|\le C_{\delta,j}r_q^{-3/4-j}$ on a common sufficiently distant end.

## Facts & Assumptions

[F1] The stationary maximal graph equation is $\partial_i A_q^i(x,Du_q)=0$, where $A_q^i(x,p)=\sqrt{-\det g_q}\,(g_q^{ij}p_j-g_q^{i0})/\sqrt{-g_q^{00}+2g_q^{0j}p_j-g_q^{jk}p_jp_k}$; all metric components are in normalized coordinates. [[pthm-maximal-graph-equation]]

[F2] Uniformly for $q\in[\delta,1]$, $g_{00}=-1+O_5(r_q^{-1})$, $g_{0i}=O_5(r_q^{-2})$, and $g_{ij}=\delta_{ij}+O_5(r_q^{-1})$. In $O_5(r^{-b})$, each spatial derivative of order $k\le5$ is bounded by a common constant times $r^{-b-k}$. [[pthm-transformed-end-geometries]] [[def-stationary-asymptotic-decay-data]]

[F3] On a common end, $|Du_q|\le C_\delta r_q^{-1/2}$. [[pthm-end-lapse-slope]]

[F4] For every $\mu\in(0,1)$ the normalized heights satisfy $|u_q|\le C_{\delta,\mu}r_q^{-\mu}$ uniformly on a common end. [[pthm-radial-barrier-height-decay]]

[F5] The annular bootstrap applies to a height-independent divergence flux with a common ellipticity interval and joint $C^{4,\alpha}$ bounds on a neighborhood of a common slope ball, a common normalized height bound, and zero-slope divergence bounded by $K/R^2$ in $C^{2,\alpha}$; it then gives the displayed four-derivative estimate. [[lem-annular-quasilinear-bootstrap-input]]

[F6] Hölder norms use the Euclidean distance on the fixed rescaled annulus. Work in ZFC, including the choice assumptions of the analytic supplier. [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]] [[math:def-axiom-of-choice]]

## Proof

**Given:** The candidate family, normalized ends and hypotheses in the Statement.

**Goal:** Prove the uniform annular estimate and the stated derivative decay.

1.1 Put $A=\{1/2<|y|<4\}$, $v_{q,R}(y)=u_q(Ry)$, $w_{q,R}=v_{q,R}/R$, and $P_{q,R}(y,p)=A_q(Ry,p)$. Then $D_yw_{q,R}=D_xu_q(Ry)$ and the equation in [F1] becomes $\operatorname{div}_yP_{q,R}(y,D_yw_{q,R})=0$. By [F3], after increasing the common radius, the realized slopes lie in $|p|\le1/4$; by [F4], the normalized heights $w_{q,R}$ are uniformly bounded on $A$. [given, F1, F3, F4, algebra]

2.1 On a fixed larger slope ball, for example $|p|\le1/3$, [F2] makes the denominator in [F1] uniformly positive for sufficiently large $R$. Matrix inversion and differentiation of the displayed flux show that $P_{q,R}$ and its joint derivatives through order four are uniformly bounded there; the fifth spatial derivative bounds in [F2], after scaling, also give the required uniform $\alpha$-Hölder control for any fixed $0<\alpha<1$. The slope derivative $P_{q,R,p}$ is symmetric and uniformly positive definite with a common upper bound: it converges uniformly on the slope ball to the slope derivative of $p/\sqrt{1-|p|^2}$. These bounds hold on a slope neighborhood of $|p|\le1/4$. [F1, F2, F6, step 1.1, algebra]

2.2 Let $s_{q,R}(y,p)=\sum_i\partial_{y_i}P_{q,R}^i(y,p)$, differentiating at fixed $p$. At $p=0$, [F1] and [F2] give $A_q(x,0)=O_5(r_q^{-2})$. Thus, for spatial derivatives through order three, $D_y^k s_{q,R}(y,0)=O(R^{-2})$ on $A$, uniformly in $q$ and $R$. In particular its $C^{2,\alpha}(A)$ norm is at most $K_\delta R^{-2}$: the third derivative bound controls the Hölder seminorm of its second derivatives on the fixed annulus. The zero-slope divergence in the original equation is $O(r_q^{-3})$, and scaling it by the two powers of $R$ used to pass from $u_q$ to $v_{q,R}$ accounts for the $R^{-1}$ forcing in the final estimate. [F1, F2, F6, step 1.1, algebra]

3.1 Steps 1.1, 2.1 and 2.2 verify all structural hypotheses of [F5], including initial quasilinear regularity through that supplier, on the fixed annulus with constants independent of $q$ and $R$. Applying [F5] yields the displayed estimate. For $\mu=3/4$, [F4] bounds the larger-annulus height supremum by $C_\delta R^{-3/4}$; since $R^{-1}\le R^{-3/4}$ for $R\ge1$, division by $R^j$ gives $|D^ju_q|\le C_{\delta,j}R^{-3/4-j}$ on $R<r_q<2R$. Choosing $R$ comparable to any sufficiently large $r_q$ proves the pointwise decay. [F4, F5, step 1.1, step 2.1, step 2.2, algebra] ∎

## Source notes

The article reference attributes the original estimate. The argument uses the declared graph equation, end estimates, barrier result and mathematical bootstrap as premises; it does not use the article's claim as a premise.

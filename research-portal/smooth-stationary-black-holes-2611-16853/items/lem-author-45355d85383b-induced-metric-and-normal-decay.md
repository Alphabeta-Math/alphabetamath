---
id: lem-author-45355d85383b-induced-metric-and-normal-decay
title: Induced metric and graph normal inherit the required weighted regularity
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-45355d85383b-weighted-fifth-graph-derivative
  - def-spacelike-maximal-hypersurface-data
  - lem-author-45355d85383b-scaled-decay-holder-upgrade
  - lem-author-45355d85383b-stationary-maximal-flux-formula
  - def-weighted-holder-spaces
  - math:def-axiom-of-choice
  - math:lem-derivative-algebra-and-chain-rules
  - math:thm-chain-rule-for-total-derivatives
  - math:lem-matrix-inversion-preserves-ck-regularity
dependency_roles:
  lem-author-45355d85383b-weighted-fifth-graph-derivative: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  lem-author-45355d85383b-scaled-decay-holder-upgrade: mathematical-premise
  lem-author-45355d85383b-stationary-maximal-flux-formula: mathematical-premise
  def-weighted-holder-spaces: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:lem-matrix-inversion-preserves-ck-regularity: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 4
---

## Statement

Work in ZFC. Fix $0<\alpha<1$ and $q>0$. Let $g$ be a smooth time-oriented Lorentzian metric of signature $(-,+,+,+)$ on a stationary Cartesian end $(t_q,x_q)$, with coefficients independent of $t_q$, $r_q=|x_q|>R_0>0$, and $\partial_{t_q}$ future timelike sufficiently far out. Assume $g_{00}+1,g_{ij}-\delta_{ij}=O_5(r_q^{-1})$ and $g_{0i}=O_5(r_q^{-2})$. Here $f=O_5(r_q^{-b})$ means $|D^j f|\le C_jr_q^{-b-j}$ for $0\le j\le5$ outside a common radius, with $D$ denoting Cartesian spatial derivatives in $x_q$. Spatial indices run from $1$ to $3$ and repeated spatial indices are summed.

Let $t_q=u(x_q)$ be a supplied smooth spacelike maximal graph, so its mean curvature vanishes, and assume $|D^ju|\le Cr_q^{-3/4-j}$ for $0\le j\le4$. Write $u_i=\partial_{x_q^i}u$. No existence of this graph is asserted.

The induced metric, in the graph coordinates $x_q$, is $h_{ij}=g_{ij}+g_{0i}u_j+g_{0j}u_i+g_{00}u_iu_j$. On a sufficiently far-out end, $h_{ij}-\delta_{ij}\in C^{3,\alpha}_{-1}$ and its inverse satisfies $h^{ij}-\delta^{ij}\in C^{3,\alpha}_{-1}$. The future unit normal has components $n^0-1\in C^{4,\alpha}_{-1}$ and $n^i\in C^{4,\alpha}_{-7/4}$ in $(t_q,x_q)$. Weighted spaces here are measured componentwise on the end by the scaled-annulus convention; a smooth restriction to any fixed inner annulus contributes a finite compact-core norm.

Define fixed spatial coordinates $x$ by $x_q=qx$ and put $r=|x|$, so $r_q=qr$. If $h^x$ denotes the induced metric components in $x$, then $q^{-2}h^x_{ij}-\delta_{ij}\in C^{3,\alpha}_{-1}$ in the fixed chart. Constant coordinate scaling preserves the displayed weighted exponents, with the appropriate constant tensor-component factors. The coordinate-comparison constants are uniform for $q\in[q_-,q_+]$ with $0<q_-\le q_+<\infty$, provided the normalized-chart estimates being compared have common constants and a common starting radius. No uniform estimate as $q\downarrow0$ is asserted.

## Statement references

[[lem-author-45355d85383b-weighted-fifth-graph-derivative]]

[[def-spacelike-maximal-hypersurface-data]]

[[lem-author-45355d85383b-scaled-decay-holder-upgrade]]

[[lem-author-45355d85383b-stationary-maximal-flux-formula]]

[[def-weighted-holder-spaces]]

[[math:def-axiom-of-choice]]

[[math:lem-derivative-algebra-and-chain-rules]]

[[math:thm-chain-rule-for-total-derivatives]]

[[math:lem-matrix-inversion-preserves-ck-regularity]]

## Facts & Assumptions

[F1] For a supplied smooth stationary maximal graph with the stated order-zero through order-four decay and background bounds, the graph-height supplier gives $u\in C^{5,\alpha}_{-3/4}$ on the end, under its ZFC hypothesis. [[lem-author-45355d85383b-weighted-fifth-graph-derivative]]

[F2] A spacelike hypersurface has its induced positive-definite metric and smooth future unit normal; maximality means vanishing mean curvature with the stated convention. [[def-spacelike-maximal-hypersurface-data]]

[F3] One extra pointwise derivative gives the corresponding eventual scaled Hölder bound, componentwise. In particular the stated stationary background errors have weighted order-four Hölder bounds; the same implication applies at every lower derivative order. [[lem-author-45355d85383b-scaled-decay-holder-upgrade]]

[F4] With $Q=-g^{00}+2g^{0i}u_i-g^{ij}u_iu_j$, the flux supplier gives the future normal $n=-g^{-1}d(t_q-u)/\sqrt Q$ when $\partial_{t_q}$ is future timelike. The differentiated inverse estimates in its Proof 1.2 are derived locally below from the background bounds. [[lem-author-45355d85383b-stationary-maximal-flux-formula]]

[F5] Weighted Hölder norms are measured by rescaling fixed annuli, with Cartesian derivative weights and the top-derivative Hölder seminorm, and apply componentwise to finite arrays. [[def-weighted-holder-spaces]]

[F6] For differentiable real functions, sums, products and quotients with nonzero denominator obey the usual derivative rules. Apply these rules to component functions on coordinate lines and iterate for higher spatial derivatives. [[math:lem-derivative-algebra-and-chain-rules]]

[F7] For composable Euclidean maps totally differentiable at the relevant points, $D(G\circ F)=DG(F)\circ DF$. Here the maps being composed are smooth on open sets: coordinate dilations and scalar functions on the positive range of $Q$. [[math:thm-chain-rule-for-total-derivatives]]

[F8] A matrix-valued map with $C^r$ entries on an open Euclidean set has $C^r$ inverse entries wherever its determinant never vanishes. Its cofactor-over-determinant formula bounds the inverse when the entries are bounded and the determinant stays away from zero. Apply this to the smooth invertible matrices $g$ and $h$ on the exterior; quantitative weighted derivative and Hölder bounds are proved below, rather than imported from this regularity statement. [[math:lem-matrix-inversion-preserves-ck-regularity]]

[A1] ZFC includes the Axiom of Choice. It is carried here when invoking the graph-height supplier in step 1.1, whose analytic suppliers require it; the finite tensor and coordinate computations add no choice assumption. [[math:def-axiom-of-choice]]

## Proof

**Given:** The metric, graph, decay, parameter and ZFC hypotheses in the Statement.

**Goal:** Prove the induced-metric, inverse, normal and coordinate-comparison assertions.

1.1 The graph and metric hypotheses are exactly those of [F1], so under [A1] that supplier gives $u\in C^{5,\alpha}_{-3/4}$. Thus $Du\in C^{4,\alpha}_{-7/4}$. By [F3], the time and spatial metric errors belong to $C^{4,\alpha}_{-1}$ and the mixed metric components to $C^{4,\alpha}_{-2}$ on a sufficiently far-out end. Apply [F3] also at lower derivative orders when lower Hölder seminorms are needed. On each fixed rescaled annulus, the Leibniz rule from [F6] and $[ab]_\alpha\le\|a\|_\infty[b]_\alpha+\|b\|_\infty[a]_\alpha$ show that products add the decay exponents. These bounds use a common sufficiently large radius for the finitely many component arrays and derivative orders. [given, F1, F3, F5, F6, A1, algebra]

1.2 Put $\eta=\operatorname{diag}(-1,1,1,1)$ and $B=g^{-1}$. By [F8], $B$ is smooth. Since $g\to\eta$, its determinant is bounded away from zero sufficiently far out, and the cofactor formula bounds $B$. The identity $B-\eta=-B(g-\eta)\eta$ gives the zeroth-order error $O(r_q^{-1})$. Differentiating $Bg=I$ using [F6] gives $\partial_kB=-B(\partial_kg)B$. Repeated product differentiation through order five expresses every positive-order derivative of $B$ as a finite sum of products of bounded inverse factors and positive-order derivatives of $g$, whose total derivative order is that of the derivative of $B$. Each such product contains at least one metric derivative, so the background bounds give $D^j(B-\eta)=O(r_q^{-1-j})$ for $0\le j\le5$. Also $g_{00}$ stays bounded away from zero; repeated differentiation of $g_{00}^{-1}g_{00}=1$ bounds $D^j(g_{00}^{-1})$ by $O(r_q^{-j})$ through order five. From $g^{i\mu}g_{\mu0}=0$ follows $g^{i0}=-g^{ij}g_{j0}/g_{00}$. Every differentiated term contains a derivative of $g_{j0}$, with its stronger order $r_q^{-2}$; the other factors have order-$j$ derivatives bounded by $O(r_q^{-j})$. Thus $g^{i0}=O_5(r_q^{-2})$. Applying [F3] at orders zero through four yields $g^{00}+1,g^{ij}-\delta^{ij}\in C^{4,\alpha}_{-1}$ and $g^{i0}\in C^{4,\alpha}_{-2}$, including the lower-order Hölder bounds needed in products. [given, F3, F6, F8, algebra]

2.1 The graph tangent vectors are $e_i=\partial_{x_q^i}+u_i\partial_{t_q}$. Evaluating $g(e_i,e_j)$ gives the displayed formula for $h$. Its spatial background error has decay exponent $-1$, its mixed products have exponent $-2-7/4=-15/4$, and its slope-square term has exponent $-7/2$, all with at least the three differentiated Hölder orders claimed. Hence $E=h-\delta\in C^{3,\alpha}_{-1}$ and $h$ is uniformly positive definite far out. By [F8], $h^{-1}$ is smooth. The identity $h^{-1}-I=-h^{-1}E$ and the cofactor formula bound the inverse and its zeroth-order error. Differentiating $h^{-1}h=I$ using [F6] gives $D h^{-1}=-h^{-1}(D h)h^{-1}$; iterate through order three. Each differentiated error term has a differentiated $E$ factor, while undifferentiated inverse factors remain bounded. Hölder increments of the inverse are controlled by $h^{-1}(x)-h^{-1}(y)=h^{-1}(x)(h(y)-h(x))h^{-1}(y)$. The product inequality from step 1.1 therefore gives $h^{-1}-I\in C^{3,\alpha}_{-1}$. [F2, F5, F6, F8, step 1.1, algebra]

2.2 The inverse estimates of step 1.2 together with step 1.1 give $Q-1\in C^{4,\alpha}_{-1}$, so $Q$ is bounded away from zero far out. The square-root difference quotient gives $(s^{1/2})'=1/(2\sqrt s)$ for $s>0$. Iterating [F6] gives bounded derivatives of $s^{-1}$ and $s^{1/2}$ through order four on a fixed positive bounded interval, and [F7] differentiates their compositions with $Q$; their increments are controlled by $a^{-1}-b^{-1}=(b-a)/(ab)$ and $\sqrt a-\sqrt b=(a-b)/(\sqrt a+\sqrt b)$. The product inequality then gives $Q^{-1/2}-1\in C^{4,\alpha}_{-1}$. The normal formula becomes $n^0=(-g^{00}+g^{0j}u_j)/\sqrt Q$ and $n^i=(g^{ij}u_j-g^{i0})/\sqrt Q$. Its time numerator differs from one by weighted order $-1$, and its spatial numerator has weighted order $-7/4$, since the mixed inverse term has the stronger order $-2$. These yield the stated normal estimates through four Hölder derivatives. The sign is future-directed because $d(t_q-u)(\partial_{t_q})=1>0$. [F1, F3, F4, F5, F6, F7, step 1.1, step 1.2, algebra]

3.1 For the coordinate change defined in the Statement, $\partial_{x^i}=q\partial_{x_q^i}$ along the graph, so $h^x_{ij}(x)=q^2h_{ij}(qx)$ and $q^{-2}h^x(x)-I=E(qx)$. Iterating [F7] for every multi-index $I$ gives $D_x^I(E(qx))=q^{|I|}(D_{x_q}^IE)(qx)$, and the corresponding Hölder seminorm gains $q^{|I|+\alpha}$. The annulus $R<r<2R$ maps to $qR<r_q<2qR$, so its weight-$-1$ scaled norm for $E(q\,\cdot)$ is $q^{-1}$ times the normalized-chart scaled norm at radius $qR$. This proves the fixed-chart metric assertion using step 2.1. The same calculation for any weight replaces $q^{-1}$ by the corresponding fixed power of $q$; tensor-component transformations supply only further constant powers. All such factors are bounded above and away from zero on $[q_-,q_+]$, and a common normalized starting radius $R_*$ is respected for $r>R_*/q_-$. Thus all claimed exponent preservation and conditional coordinate uniformity follow. [F2, F5, F7, step 2.1, step 2.2, algebra] ∎

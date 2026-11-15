---
id: lem-author-45355d85383b-compact-holder-superposition
title: Compact-core Hölder superposition gives a continuously differentiable graph map
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-45355d85383b-smooth-mean-curvature-jet
  - lem-author-45355d85383b-weighted-smooth-inversion
  - def-normal-graph-and-mean-curvature-data
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
dependency_roles:
  lem-author-45355d85383b-smooth-mean-curvature-jet: mathematical-premise
  lem-author-45355d85383b-weighted-smooth-inversion: mathematical-premise
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 7
---

## Statement

Fix $0<\alpha<1$ and a compact smooth three-dimensional core $K\subset\Sigma$, with smooth boundary allowed. Use the jointly smooth Lorentzian metric family $g_q$ and compatible supplied transverse flow charts $\Psi_q(x,s)$ of the finite-jet supplier, with one real parameter $q$ in an open interval $I$ containing $q_*$ and with the reference slice spacelike at $q_*$. Background coefficients and charts are smooth up to the boundary, in the sense of local smooth extensions across it. Fix a finite cover by compact coordinate balls or boundary half-balls, each contained in a larger chart. For $r=2,4$, let $C^{r,\alpha}(K)$ be the full real finite-norm Hölder space, with coordinate derivatives through order $r$ continuous up to the boundary and norm the sum of the usual $C^{r,\alpha}$ norms on these fixed pieces. No smoothness beyond this Hölder regularity is required of its elements.

In each chart let $\Omega$ be the open set of tuples $(q,x,z,p)$ for which the supplied flow chart is defined and the graph tangent metric is positive definite. Here $z$ is graph height and $p$ its coordinate slope. Define $\mathcal U\subset I\times C^{4,\alpha}(K)$ by requiring $(q,x,w(x),Dw(x))\in\Omega$ at every point of every fixed chart piece. This is an open set containing $(q_*,0)$. On $\mathcal U$ the compatible local expressions for pulled-back mean curvature define a $C^1$ map $\mathcal H:\mathcal U\to C^{2,\alpha}(K)$, where $C^1$ means continuous Fréchet differentiability in the fixed norms. For embedded flow graphs this is exactly their geometric pulled-back mean curvature; the jet condition alone asserts no global embedding.

Write $\mathcal H(q,w)=A^{ij}(q,x,w,Dw)w_{ij}+B(q,x,w,Dw)$ in local coordinates, summing repeated indices from $1$ to $3$. At every $(q,w)\in\mathcal U$ its graph derivative is $D_w\mathcal H(q,w)v=A^{ij}v_{ij}+(A^{ij}_zw_{ij}+B_z)v+(A^{ij}_{p_\ell}w_{ij}+B_{p_\ell})v_\ell$, and its parameter derivative is $\partial_q\mathcal H(q,w)=(\partial_q A^{ij})w_{ij}+\partial_q B$. All coefficients and their partial derivatives are evaluated at $(q,x,w,Dw)$, with $\partial_q$ taken at fixed $(x,z,p)$. Both derivatives are bounded in the indicated norms and vary continuously in operator norm. If a prescribed boundary set $S\subset\partial K$ is fixed, the same conclusions hold on the relatively open subset $\mathcal U\cap(I\times X_S)$, where $X_S=\{w\in C^{4,\alpha}(K):w|_S=0\}$ has the inherited norm, and graph directions obey $v|_S=0$.

## Statement references

[[lem-author-45355d85383b-smooth-mean-curvature-jet]]

[[lem-author-45355d85383b-weighted-smooth-inversion]]

[[def-normal-graph-and-mean-curvature-data]]

[[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

## Facts & Assumptions

[F1] Mean curvature is a smooth second-order finite-jet expression on admissible graphs. [[lem-author-45355d85383b-smooth-mean-curvature-jet]]

[F2] Smooth finite-dimensional compositions and products are continuously differentiable in controlled Hölder norms. We use the compact-chart composition and derivative-continuity estimates in Proof 2.1–4.1 and the normed-space meaning of $C^1$ in the Statement. [[lem-author-45355d85383b-weighted-smooth-inversion]]

[F3] Flow graphs carry the future-normal pulled-back mean-curvature convention, and zero graph height on a prescribed boundary fixes it pointwise. [[def-normal-graph-and-mean-curvature-data]]

[F4] The unweighted finite $C^{r,\alpha}$ norm controls coordinate derivative suprema through order $r$ and the order-$r$ Hölder seminorm; the closure convention requires continuous boundary values of these derivatives. We apply these definitions on the fixed coordinate balls and half-balls and sum the norms. [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

## Proof

**Given:** The fixed smooth background, compact core, coordinate Hölder norms and admissible first-jet domain in the Statement.

**Goal:** Prove openness of the domain and continuous Fréchet differentiability with the stated graph, parameter and fixed-boundary derivatives.

1.1 Fix $(q,w)\in\mathcal U$. Its first-jet image on each compact chart piece is compact and lies in the open admissible set. It therefore has a positive-radius tube still inside that set; choose the minimum radius over the finite cover, also keeping the parameter in $I$. The fixed $C^{4,\alpha}$ norm controls $w,Dw$ uniformly, so a sufficiently small perturbation $(\delta q,v)$ stays in these tubes. This proves openness. The zero jet is admissible at $q_*$ by the reference spacelikeness, so $(q_*,0)\in\mathcal U$. Smooth coefficient derivatives through every required finite order are bounded on smaller closed tubes by the smoothness in [F1] and compactness. Thus the compact-chart estimates of [F2] apply at this arbitrary admissible point, rather than only at zero. [F1, F2, F4, given, choose]

2.1 On each fixed chart, $(q,w)\mapsto(q,x,w,Dw)$ has bounded linear increment $(\delta q,0,v,Dv)$ in the order-two Hölder norm, and $w\mapsto w_{ij}$ is bounded linear into that norm. These bounds follow from [F4]: lower derivative Hölder seminorms on a convex ball or half-ball are controlled by the next derivative supremum and its finite diameter. Apply the compact-chart calculation of [F2], Proof 2.1–4.1, to the smooth finite-dimensional coefficient functions, treating $x$ as an additional fixed component. That calculation uses only Hölder product differences and finite coordinate chain-rule expansions, so applies to these fixed pieces without an annular supremum or a weighted extension. It gives $C^1$ coefficient maps into $C^{2,\alpha}$ on the neighborhood from step 1.1, with coefficient increments $A^{ij}_q\delta q+A^{ij}_zv+A^{ij}_{p_\ell}v_\ell$ and $B_q\delta q+B_zv+B_{p_\ell}v_\ell$. Multiplication is bounded in this norm: $[ab]_\alpha\le\|a\|_\infty[b]_\alpha+\|b\|_\infty[a]_\alpha$, and the finite Leibniz expansion bounds its derivatives through order two. Consequently $A^{ij}w_{ij}+B$ belongs to the target space. [F1, F2, F4, step 1.1, algebra]

3.1 Put $\varepsilon=|\delta q|+\|v\|_{C^{4,\alpha}(K)}$. In the finite-chart order-two norms, step 2.1 gives coefficient remainders $r_A,r_B=o(\varepsilon)$ after subtracting their linear increments, and coefficient changes $\Delta A=O(\varepsilon)$. Expanding $(A^{ij}+\Delta A^{ij})(w_{ij}+v_{ij})+B+\Delta B$ leaves, after subtracting the asserted total derivative, precisely $r_A^{ij}w_{ij}+\Delta A^{ij}v_{ij}+r_B$. The product estimate bounds this by $o(\varepsilon)+O(\varepsilon^2)$; hence the derivative is the displayed bounded linear map. Continuity of the coefficient derivatives in $C^{2,\alpha}$ from [F2], continuity of $w\mapsto D^2w$, and the same product bound imply continuity of this derivative in operator norm. The compatible expressions agree on chart overlaps by [F1] and the geometric convention [F3]; the finite sum of chart estimates proves the target-norm assertions. Restricting the estimates to $X_S$ gives the same derivative on its allowed directions, and [F3] supplies the pointwise fixed-boundary interpretation. This proves all claims. [F1, F2, F3, F4, step 1.1, step 2.1, algebra] ∎

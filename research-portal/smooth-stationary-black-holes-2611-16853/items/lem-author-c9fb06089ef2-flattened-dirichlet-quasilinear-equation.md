---
id: lem-author-c9fb06089ef2-flattened-dirichlet-quasilinear-equation
title: Flattening a smooth fixed boundary preserves the elliptic graph equation
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-45355d85383b-smooth-mean-curvature-jet
  - thm-maximal-jacobi-lapse-input
  - def-normal-graph-and-mean-curvature-data
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary
  - math:thm-chain-rule-for-total-derivatives
  - math:thm-compactness-under-continuous-maps
  - math:cor-heine-borel-in-the-product-topology
  - math:cor-mean-value-theorem
  - math:def-countable-choice
dependency_roles:
  lem-author-45355d85383b-smooth-mean-curvature-jet: mathematical-premise
  thm-maximal-jacobi-lapse-input: mathematical-premise
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:cor-heine-borel-in-the-product-topology: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
  math:def-countable-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 7
---

## Statement

Assume the Axiom of Countable Choice $\mathrm{AC}_\omega$ for the inherited tangent-bundle smooth structures.

Let $(M,g)$ be a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$, let $\Sigma$ be a smooth embedded spacelike reference hypersurface with smooth boundary $S$, and use a smooth local transverse-flow chart $\Psi(x,s)=\phi_s^Y(x)$ for a smooth field $Y$ transverse to $\Sigma$. At the boundary the reference charts, metric and flow data are smooth in the local-extension sense. Let $0<\alpha<1$ and let $w$ define an admissible spacelike flow graph, with $w\in C^{4,\alpha}$ up to $S$ and with the explicit homogeneous Dirichlet condition $w|_S=0$.

Near each boundary point, a smooth boundary chart gives an equivalent maximal equation on a half-neighborhood, $A^{ij}(x,w,Dw)w_{ij}+B(x,w,Dw)=0$, with $w=0$ on the flat boundary $x_3=0$. The finite-dimensional coefficients are smooth on the local spacelike-jet domain. After multiplying the mean-curvature equation by a locally constant sign if necessary, the symmetric matrix $A$ is uniformly positive definite on a sufficiently small compact graph-jet neighborhood. No future-timelike assumption on $Y$ is needed; if $Y$ is future timelike, this sign is $+1$. Every purely tangential derivative of positive order already possessed by $w$ up to the boundary has zero boundary trace. The same local coefficient and ellipticity assertions hold in interior charts.

## Facts & Assumptions

[A1] Assume $\mathrm{AC}_\omega$ for the inherited tangent-bundle smooth structures used by F1 and F3. This inherited assumption is used when applying the graph and finite-jet suppliers in steps 1.1 and 2.1. [[math:def-countable-choice]] [[lem-author-45355d85383b-smooth-mean-curvature-jet]] [[def-normal-graph-and-mean-curvature-data]]

[F1] Mean curvature is a smooth second-order quasilinear expression on the open set of spacelike graph jets, with smooth local flow data and smooth extensions at a boundary. The pointwise formula also applies to graphs with at least two continuous derivatives. [[lem-author-45355d85383b-smooth-mean-curvature-jet]]

[F2] For the future-normal mean-curvature convention, a variation $V=a n+X$ has derivative $\Delta_h a-(|k|_h^2+\operatorname{Ric}(n,n))a+X(H)$. Thus its principal normal-speed term is the positive induced inverse metric times the Hessian of $a$. [[thm-maximal-jacobi-lapse-input]]

[F3] The flow-graph definition requires transversality of $Y$, not future timelikeness. Its mean-curvature map is pulled back by the graph map, and imposing $w|_S=0$ fixes the boundary pointwise. The zero-height condition here is a hypothesis of the Statement. [[def-normal-graph-and-mean-curvature-data]]

[F4] The up-to-boundary $C^{m,\alpha}$ class requires continuous extensions of every derivative through order $m$ to the boundary. It does not assert that $w$ extends smoothly across the boundary. [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

[F5] Smooth boundary charts take values in a relatively open subset of a closed half-space, with transitions smooth in the local-extension sense. [[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary]]

[F6] Totally differentiable coordinate compositions obey the chain rule, which can be iterated for the smooth coordinate changes here. [[math:thm-chain-rule-for-total-derivatives]]

[F7] A continuous real-valued function on a nonempty compact space attains a maximum and a minimum. [[math:thm-compactness-under-continuous-maps]]

[F8] A closed bounded subset of finite-dimensional Euclidean space is compact, including a closed coordinate half-box and its product with closed bounded jet boxes. [[math:cor-heine-borel-in-the-product-topology]]

[F9] A real function continuous on a closed interval and differentiable on its interior satisfies the mean value identity for its endpoint increment. [[math:cor-mean-value-theorem]]

## Proof

**Given:** The inherited countable-choice assumption, smooth local transverse-flow data, admissible graph, boundary regularity and zero-height condition in the Statement.

**Goal:** Produce the equivalent elliptic equation and prove the zero tangential traces without restricting the orientation of the transverse field.

1.1 Choose a smooth boundary chart with $S$ represented by $x_3=0$ and the reference interior by $x_3>0$. Write $y=\chi(x)$ for its smooth change from reference coordinates and $J_i{}^a=\partial x^a/\partial y^i$. Applying the chain rule twice gives $w_{y^iy^j}=J_i{}^aJ_j{}^b w_{x^ax^b}+(\partial_{y^i}J_j{}^b)w_{x^b}$. Thus the symmetric principal matrix of the expression in F1 transforms to $\widetilde C^{ab}=C^{ij}J_i{}^aJ_j{}^b$, while the terms involving second derivatives of the coordinate change enter the lower-order coefficient. Both coefficients remain smooth functions of $(x,z,p)$, where $z$ and $p$ denote height and slope. The stipulated local extensions handle the flat boundary, and $w|_S=0$ gives zero height there. [A1, F1, F3, F5, F6, given, algebra]

2.1 In the flow coordinates the graph tangent vectors are $e_i=\partial_{x^i}+w_i\partial_s$ and $Y=\partial_s$. Comparing their $x$ components shows that $Y$ is never tangent to any such graph. Since the induced metric is positive definite, its tangent space is the full orthogonal complement of the future unit normal $n$; consequently $a=-g(Y,n)\ne0$. The normal and $a$ depend smoothly on the spacelike first jet. Around any fixed admissible jet shrink to a connected jet neighborhood on which $a$ has one sign $\varepsilon\in\{-1,1\}$. For a height variation $v$, the variational vector is $vY=(av)n+vY^\top$. By F2 its only second derivatives of $v$ are $a h^{ij}v_{ij}$: expanding $\Delta_h(av)$ leaves all other terms with at most one derivative of $v$, and the tangential term is $vY^\top(H)$. Differentiating the quasilinear expression in F1 with respect to the height gives principal coefficient $C^{ij}$, so $C^{ij}=a h^{ij}$. This comparison can be made on smooth test graphs realizing each prescribed finite jet; the finite-jet formula then gives the same identity at the stated $C^{4,\alpha}$ regularity. Multiplying both coefficients of the equation by $\varepsilon$ gives $A^{ij}=|a|h^{ij}$ before coordinate change, hence a positive definite matrix also after the congruence in step 1.1. If $Y$ is future timelike, writing $Y=a n+Y^\top$ shows $a>0$ by the future orientation, so $\varepsilon=+1$. [A1, F1, F2, F3, step 1.1, given, algebra]

3.1 Choose a sufficiently small closed coordinate half-box and closed height-and-slope boxes around the boundary jet, wholly within the chart's spacelike-jet domain and the sign neighborhood of step 2.1. This is possible by openness relative to the boundary half-space. Their product is compact by F8. On its product with the Euclidean unit sphere, the quadratic form $(x,z,p,\xi)\mapsto A^{ij}(x,z,p)\xi_i\xi_j$ is continuous and strictly positive. That product is closed and bounded and hence compact by F8; F7 gives a strictly positive minimum $\lambda$ and a finite maximum $\Lambda$. By homogeneity, $\lambda|\xi|^2\le A^{ij}\xi_i\xi_j\le\Lambda|\xi|^2$ for every $\xi$. This proves uniform ellipticity on the smaller compact graph-jet neighborhood. An interior coordinate box gives the same argument without the boundary half-space. [F1, F7, F8, step 1.1, step 2.1, choose, algebra]

4.1 On a smaller flat patch, continuous boundary extensions of the derivatives allow tangential differentiation of the trace. Explicitly, the one-variable mean value identity from F9 on an interior tangential segment gives $w(x'+te_j,r)-w(x',r)=t\,\partial_j w(x'+\theta te_j,r)$ for some $0<\theta<1$, where $j<3$ and $r>0$. Let $r$ decrease to zero. Continuity of $\partial_j w$ near $(x',0)$ bounds the difference between the resulting boundary difference quotient and $\partial_j w(x',0)$ by $\sup_{|s|\le|t|,\,r\ge0\text{ small}}|\partial_j w(x'+se_j,r)-\partial_j w(x',0)|$, which tends to zero as the segment and its height shrink. Hence the tangential derivative of the trace is the trace of $\partial_j w$. Repeat this argument with each already available purely tangential derivative. Since the initial trace is identically zero, all these positive-order tangential traces vanish. The repetition applies through every finite order for which the derivatives extend continuously to the boundary, in particular through order four under the stated hypotheses. [F3, F4, F9, step 1.1, given, algebra] ∎

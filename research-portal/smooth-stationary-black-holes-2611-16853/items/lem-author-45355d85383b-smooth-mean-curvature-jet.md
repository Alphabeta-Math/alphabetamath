---
id: lem-author-45355d85383b-smooth-mean-curvature-jet
title: The mean-curvature graph map is a smooth finite-jet expression
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-normal-graph-and-mean-curvature-data
  - def-spacelike-maximal-hypersurface-data
  - lem-author-45355d85383b-relative-timelike-flow-chart
  - math:thm-compactness-under-continuous-maps
  - math:cor-heine-borel-in-the-product-topology
  - math:def-compact-space
  - math:thm-chain-rule-for-total-derivatives
  - physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative
  - math:def-countable-choice
dependency_roles:
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  lem-author-45355d85383b-relative-timelike-flow-chart: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:cor-heine-borel-in-the-product-topology: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative: mathematical-premise
  math:def-countable-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 6
---

## Statement

Assume $\mathrm{AC}_\omega$ for the inherited tangent-bundle smooth structures.

Let $d\in\mathbb N$ with $d\ge1$, let $q$ range over an open set $Q\subset\mathbb R^d$, and fix $q_*\in Q$. Let $g_q$ be time-oriented smooth Lorentzian metrics of signature $(-,+,+,+)$ on a fixed neighborhood of a smooth embedded reference hypersurface $\Sigma$, jointly smooth in $(q,y)$ in ambient coordinates $y$, with smoothly varying time orientation. Assume $\Sigma$ is spacelike for $g_{q_*}$. Supply transverse flow charts $\Psi_q(x,s)$ on common coordinate domains, jointly smooth in $(q,x,s)$, with $\Psi_q(x,0)=x$ on the reference slice. Charts fixed in $q$ are allowed. At a smooth boundary use charts and data smooth up to the boundary, meaning locally smoothly extendible across it. The admissible fixed-boundary graphs of the timelike-flow supplier are one instance under that supplier's hypotheses; here charts are supplied data. Whenever a boundary $S$ is prescribed, impose $w|_S=0$ to fix it pointwise.

On the open set of spacelike graph jets, the mean curvature of $x\mapsto\Psi_q(x,w(x))$, pulled back to $\Sigma$ with the future-normal convention, has the form $\mathcal H(q,w)(x)=A^{ij}(q,x,w,Dw)D_{ij}w+B(q,x,w,Dw)$, summing $i,j\in\{1,2,3\}$. Write $z=w(x)$ and $p=Dw(x)$ for height and coordinate slope. The coefficients are smooth finite-dimensional functions of the ambient metric and its first coordinate derivatives, the smooth flow chart and its required coordinate derivatives, and $(z,p)$. With the smooth ambient inverse metric included among the background coefficients, their denominators are positive powers of the induced-metric determinant and the timelike conormal norm.

For every compact core $K\subset\Sigma$, a finite coordinate cover and sufficiently small parameter, height and slope neighborhoods of $(q_*,0,0)$ can be chosen whose closed coordinate products remain inside the common spacelike-jet domain. Every mixed derivative of $A^{ij}$ and $B$ with respect to $(q,x,z,p)$ of any fixed finite total order is uniformly bounded on those products. Bounds may depend on the order, core and background family. These are local coefficient bounds; any global graph embedding is subject to the stated graph admissibility conditions.

## Facts & Assumptions

[A1] The assumption $\mathrm{AC}_\omega$ is inherited by the tangent-bundle smooth structures in the graph convention and in the nondegenerate Levi–Civita supplier. It is used when applying that supplier in step 1.1; no choice of a connection separately for each parameter is made. [[math:def-countable-choice]] [[def-normal-graph-and-mean-curvature-data]]

[F1] Flow graph mean curvature is the pullback of the trace of the positive-sign second fundamental form, and zero boundary height fixes the boundary. [[def-normal-graph-and-mean-curvature-data]]

[F2] The induced metric and future normal are fixed, and the convention $k(U,V)=-g(\nabla_U n,V)$ gives $H=-\operatorname{tr}_h k$. [[def-spacelike-maximal-hypersurface-data]]

[F3] Under its stationary graph-end and uniform family hypotheses, the timelike-flow construction supplies a fixed smooth flow chart and an admissible fixed-boundary graph neighborhood for a one-parameter metric family. No arbitrary parameter-dependent chart construction or global graph existence is inferred from it here; the charts in the Statement are supplied. [[lem-author-45355d85383b-relative-timelike-flow-chart]]

[F4] A continuous real-valued function on a nonempty compact space attains a finite maximum and minimum (Statement 2). [[math:thm-compactness-under-continuous-maps]]

[F5] Closed bounded coordinate boxes, including boxes intersected with a closed boundary half-space, are compact in the Euclidean topology (Statements 1 and 2). [[math:cor-heine-borel-in-the-product-topology]]

[F6] A compact subset carries its subspace topology, and every open cover of that space has a finite subcover. [[math:def-compact-space]]

[F7] Totally differentiable Euclidean maps satisfy $D(g\circ f)=Dg\circ Df$ with the derivatives evaluated at the corresponding points; iteration applies to the smooth coordinate compositions here. [[math:thm-chain-rule-for-total-derivatives]]

[F8] For a smooth symmetric nondegenerate metric on a smooth four-manifold without boundary, under $\mathrm{AC}_\omega$ for its canonical tangent-bundle smooth structure, the unique torsion-free metric-compatible connection has coordinate coefficients $\Gamma^a{}_{bc}=\tfrac12 g^{ad}(\partial_b g_{dc}+\partial_c g_{bd}-\partial_d g_{bc})$. Its vector derivative is $(\nabla_V Z)^a=V^b\partial_b Z^a+\Gamma^a{}_{bc}V^b Z^c$. These are parts (a)–(c) of the mathematical nondegenerate Levi–Civita theorem, applied here on ambient open coordinate neighborhoods. [[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative]]

## Proof

**Given:** The jointly smooth metric and supplied transverse flow-chart families, reference hypersurface, compact core and inherited countable-choice assumption of the Statement.

**Goal:** Establish the quasilinear finite-jet expression and uniform finite-order coefficient bounds.

1.1 For fixed $q$, put $\widehat g_q=\Psi_q^*g_q$ in flow coordinates $(x,s)$. The graph tangent vectors are $e_i=\partial_{x^i}+w_i\partial_s$, its induced metric is $h_{ij}=\widehat g_q(e_i,e_j)$, and its conormal is $\eta=ds-w_i dx^i$. On a spacelike graph $L=\sqrt{-\widehat g_q^{-1}(\eta,\eta)}>0$, and the future unit normal is the appropriate signed vector $\widehat g_q^{-1}\eta/L$. Time orientation fixes the sign locally. The positive-sign second fundamental form is $g(\nabla_{e_i}n,e_j)$, so its trace is the mean curvature of [F1], equivalently $-\operatorname{tr}_h k$ in [F2]. The metric pullback and its first derivatives use the metric, its first ambient derivatives and finitely many derivatives of the supplied smooth chart. The cofactor formula for the inverse metric, whose determinant is nonzero, and the coordinate chain rule give jointly smooth background coefficients in $(q,x,s)$. Apply [F8] under [A1] for each fixed $q$ to the smooth nondegenerate pulled-back metric on the open flow-coordinate domain. Its coordinate formula expresses the connection coefficients using only this inverse metric and first coordinate derivatives of $\widehat g_q$. It therefore gives jointly smooth connection coefficients in $(q,x,s)$ from the same background data. At the boundary apply this ambient formula to the stipulated local smooth extensions before restriction. This is a local calculation on supplied charts; the fixed-chart admissible neighborhood in [F3] is a permitted instance. [A1, F1, F2, F3, F7, F8, given, algebra]

2.1 The normal depends only on $(q,x,w,Dw)$. Differentiating its coordinate components tangentially contains $w_{ij}$ only linearly by the chain rule. The additional connection term in [F8] is $\widehat\Gamma^a{}_{bc}e_i^b n^c$, evaluated at $s=w(x)$; by step 1.1 it depends only on $(q,x,w,Dw)$ and contributes no second derivatives of $w$. Thus the covariant tangential derivative also contains $w_{ij}$ only linearly. Contraction with $h^{ij}$ therefore has the asserted form $A^{ij}(q,x,w,Dw)w_{ij}+B(q,x,w,Dw)$. The inverse $h^{ij}$ uses cofactors divided by $\det h>0$, and normal normalization uses $L>0$. Thus the coefficient formulas use finite sums, products and inverses and a positive square root; the ambient inverse metric is treated as a smooth background coefficient. All coefficients are smooth on the open spacelike-jet set with the stated denominator structure. The same pointwise calculation applies to any admissible graph with at least two continuous coordinate derivatives. [step 1.1, F1, F2, F7, F8, algebra]

3.1 At each point of $K$, the common chart domain is open and the zero jet at $q_*$ is spacelike. Consequently it contains a closed product of a small parameter box about $q_*$, a spatial coordinate box about that point and a height-and-slope box about $(0,0)$, still inside the spacelike-jet set. At the boundary use a closed half-box and the stipulated local smooth extensions. The relative interiors of the spatial boxes, intersected with $K$, form an open cover of the subspace $K$. By [F6] finitely many suffice. Shrink to a common parameter box $J\subset Q$ and common height-and-slope radii by taking the minimum of their finitely many positive radii. Each resulting coordinate product $J\times C_a\times P_a$ is closed and bounded in finite-dimensional Euclidean space and hence compact by [F5]. By [F4], the positive continuous functions $\det h$ and $L$ attain strictly positive minima on each nonempty product. By step 2.1, the absolute value of each mixed coefficient derivative is continuous there and has a finite maximum by [F4], including boundary values by smooth extension. Taking the largest of these maxima over the finite cover and the finitely many derivatives through a fixed order proves the uniform bound. If $K$ is empty the bound is vacuous. [step 1.1, step 2.1, F4, F5, F6, given, choose, algebra] ∎

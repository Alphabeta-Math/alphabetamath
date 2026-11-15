---
id: thm-maximal-jacobi-lapse-input
title: Mean-curvature variation and the stationary lapse equation
kind: theorem
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-spacelike-maximal-hypersurface-data
  - def-normal-graph-and-mean-curvature-data
  - def-stationary-lorentzian-data
  - physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative
  - math:def-laplace-beltrami-operator-as-trace-of-the-hessian
  - math:prop-gradient-hessian-and-divergence-connection-formulas
  - physics:thm-gr-curvature-algebraic-symmetries
  - math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes
dependency_roles:
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative: mathematical-premise
  math:def-laplace-beltrami-operator-as-trace-of-the-hessian: mathematical-premise
  math:prop-gradient-hessian-and-divergence-connection-formulas: mathematical-premise
  physics:thm-gr-curvature-algebraic-symmetries: mathematical-premise
  math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: E. Gourgoulhon, 3+1 Formalism and Bases of Numerical Relativity (2007)
      url: https://luth2.obspm.fr/~luthier/gourgoulhon/pdf/form3p1.pdf
      locator: Section 9.2.2, equations (9.4) and (9.15), printed pp. 153–155
      statement: A maximal slicing has zero mean curvature and obeys the displayed
        elliptic lapse equation when the maximal condition is maintained.
      hypotheses: The 3+1 foliation and Einstein-equation conventions used in the
        cited section.
      reading_limits: Consulted Section 9.2.2, equations (9.4) and (9.15), printed pp.
        153 and 155 (PDF pages 153 and 155). These equations record maximal
        slicing and its elliptic lapse equation under the stated
        Einstein-equation conventions. This is background only; the full
        geometric variation formula and its sign conventions are proved locally
        below.
dependency_level: 1
---

## Statement

Let $(M,g)$ be a smooth time-oriented Lorentzian four-manifold, and let $F_s$ be a smooth local variation through spacelike embeddings of a smooth spacelike hypersurface $\Sigma=F_0(\Sigma)$, with $F_0$ the inclusion. Write $n$ for the future unit normal, $h$ for the induced metric, $k(U,V)=-g(\nabla_U n,V)$, and $H=\operatorname{div}_g n=-\operatorname{tr}_h k$. Let the variational vector field be $V=a n+X$, where $X$ is tangent and $a=-g(V,n)$. Then the derivative at $s=0$ of the pulled-back mean curvature is $\Delta_h a-(|k|_h^2+\operatorname{Ric}(n,n))a+X(H)$. Here $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$ and $|k|_h^2=h^{ij}h^{pq}k_{ip}k_{jq}$.

If $H=0$ on $\Sigma$ and a Killing field $T$ decomposes along it as $T=Nn+X$, then $\Delta_hN=(|k|_h^2+\operatorname{Ric}(n,n))N$. This local identity asserts no boundary values or normalization at an end.

## Statement references

[[def-spacelike-maximal-hypersurface-data]]

[[def-normal-graph-and-mean-curvature-data]]

[[def-stationary-lorentzian-data]]

[[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative]]

[[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]]

[[math:prop-gradient-hessian-and-divergence-connection-formulas]]

[[physics:thm-gr-curvature-algebraic-symmetries]]

[[math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes]]

## Facts & Assumptions

[F1] The spacelike hypersurface data give the future normal, induced metric, sign convention for $k$, mean curvature and normal–tangential decomposition. [[def-spacelike-maximal-hypersurface-data]]

[F2] The mean-curvature map pulls the mean curvature of each admissible spacelike graph back to the original hypersurface. [[def-normal-graph-and-mean-curvature-data]]

[F3] A Killing field has local flow preserving $g$, and the curvature convention is $R(U,V)W=\nabla_U\nabla_VW-\nabla_V\nabla_UW-\nabla_{[U,V]}W$, with $\operatorname{Ric}_{bd}=R^a{}_{bad}$. The Killing condition and curvature convention are supplied by the stationary data; flow invariance follows from vanishing metric Lie derivative on each local flow domain. [[def-stationary-lorentzian-data]] [[math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes]]

[F4] The smooth nondegenerate metric has a unique torsion-free metric-compatible connection, extended to tensor fields. [[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative]]

[F5] For the smooth induced Riemannian metric $h$, the intrinsic operators satisfy $h(\operatorname{grad}_h a,U)=U(a)$, $\operatorname{Hess}_h a(U,W)=h(\nabla^h_U\operatorname{grad}_h a,W)$, and $\operatorname{div}_h Z=\operatorname{tr}(U\mapsto\nabla^h_U Z)$, where $\nabla^h$ is the Levi–Civita connection of $h$. Thus $\Delta_h a=\operatorname{tr}_h\operatorname{Hess}_h a=\operatorname{div}_h\operatorname{grad}_h a$. [[math:prop-gradient-hessian-and-divergence-connection-formulas]] [[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]]

[F6] The curvature tensor of a smooth time-oriented Lorentzian four-manifold with its metric-selected connection has the algebraic curvature symmetries, in particular $R(U,W)Z=-R(W,U)Z$, with the curvature and Ricci conventions used here. [[physics:thm-gr-curvature-algebraic-symmetries]]

## Proof

**Given:** The variation and geometric data in the Statement.

**Goal:** Derive the variation formula and its consequence for a maximal hypersurface moved by a Killing flow.

1.1 First suppose $V=an$. In local coordinates $x^i$ on $\Sigma$, put $e_i=\partial_iF_s$ and $K_{ij}=g(\nabla_{e_i}n,e_j)=-k_{ij}$ at $s=0$. Differentiating $g(n,n)=-1$ and $g(n,e_i)=0$, using torsion-freeness and $[\partial_s,e_i]=0$, gives $\nabla_{\partial_s}n=\operatorname{grad}_h a$ at $s=0$. Metric compatibility also gives $\dot h_{ij}=2aK_{ij}$ and $\dot h^{ij}=-2aK^{ij}$. [given, F1, F4, F5]

2.1 Commuting the covariant derivatives by the curvature convention and differentiating $K_{ij}$ gives $\dot K_{ij}=\nabla^h_i\nabla^h_j a+a\,g(R(n,e_i)n,e_j)+aK_i{}^pK_{pj}$, where $\nabla^h$ is the Levi–Civita connection of $h$. Using $\operatorname{tr}_h\operatorname{Hess}_h a=\Delta_h a$ from F5, tracing this identity and including $\dot h^{ij}K_{ij}$ yields $\dot H=\Delta_h a-a|k|_h^2+a h^{ij}g(R(n,e_i)n,e_j)$. The displayed Ricci convention and the curvature symmetries of the metric-compatible torsion-free connection give $h^{ij}g(R(n,e_i)n,e_j)=-\operatorname{Ric}(n,n)$, proving the formula for a normal variation. [F1, F3, F4, F5, F6, step 1.1]

3.1 For a general variation, locally reparametrize the domain by a time-dependent diffeomorphism whose initial velocity cancels $X$. The resulting variation has initial velocity $an$; differentiating the scalar pullback under the inverse reparametrization adds $X(H)$. This proves the stated formula for arbitrary $V$; the graph mean-curvature map uses the same pullback convention. [given, F2, step 2.1]

4.1 By F3 the local flow of a Killing field consists of local isometries. Transporting $\nabla$ by a local isometry gives a torsion-free metric-compatible connection, which equals $\nabla$ by uniqueness in F4. The flow starts at the identity and hence preserves future direction on its local flow domain. It therefore carries the future normal and mean curvature of $\Sigma$ to those of the image hypersurface. Its pulled-back mean curvature is therefore constant in the flow parameter. Its variational field is $T=Nn+X$; if $H=0$, then $X(H)=0$, and the variation formula gives the stated lapse equation. The calculation is local and imposes no boundary or asymptotic condition. [given, F1, F3, F4, step 3.1] ∎

## External input

Gourgoulhon records the maximal-slicing lapse equation under the 3+1 Einstein-equation conventions; the more general geometric variation above is derived locally.

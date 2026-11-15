---
id: lem-author-78c700cb9e03-invariant-normal-boost-coordinates
title: Circle-invariant normal coordinates linearize a bifurcate Killing boost
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - def-circle-action-and-invariant-normal-data
  - lem-killing-normal-boost-and-invariant-tensors
  - lem-author-ca4ffba327b3-compact-normal-exponential-tube
  - physics:thm-gr-local-geodesics-and-exponential-map
  - physics:def-gr-metric-selected-connection
  - math:def-local-and-global-flow
  - math:def-axiom-of-choice
  - math:def-embedded-submanifold-and-slice-chart
  - physics:def-lorentz-orthogonality-and-orthogonal-complement
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  def-circle-action-and-invariant-normal-data: mathematical-premise
  lem-killing-normal-boost-and-invariant-tensors: mathematical-premise
  lem-author-ca4ffba327b3-compact-normal-exponential-tube: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  physics:def-lorentz-orthogonality-and-orthogonal-complement: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Let $S$ be a compact spacelike two-sphere in a smooth time-oriented Lorentzian four-manifold. Suppose local commuting Killing fields $K,Z$ satisfy $K|_S=0$, $Z$ generates a time-oriented circle action preserving $S$, and $\nabla K$ has positive constant boost rate $\kappa$ on its oriented normal plane. Choose the outward normal-plane orientation toward the exterior. There is a circle-invariant orthonormal normal frame $(e_0,e_1)$, with $e_0$ future timelike and $e_1$ outward, and a normal exponential tube $\Xi(y,u,v)=\exp_y(u e_0+v e_1)$. In this tube the local circle action is $(y,u,v)\mapsto(\psi_a y,u,v)$ and $K=\kappa(v\partial_u+u\partial_v)$. In the exterior wedge $v>|u|$, write $u=r\sinh(\kappa\tau)$ and $v=r\cosh(\kappa\tau)$; then $K=\partial_\tau$, $Z=Z_S$, and if $K=T+\Omega Z$, then $T=\partial_\tau-\Omega Z_S$. These coordinate formulas hold while the tube points exist; they do not assert completeness yet.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-bifurcate-killing-horizon-data]]

[[def-circle-action-and-invariant-normal-data]]

[[lem-killing-normal-boost-and-invariant-tensors]]

[[lem-author-ca4ffba327b3-compact-normal-exponential-tube]]

[[physics:thm-gr-local-geodesics-and-exponential-map]]

[[physics:def-gr-metric-selected-connection]]

[[math:def-local-and-global-flow]]

[[math:def-axiom-of-choice]]

[[math:def-embedded-submanifold-and-slice-chart]]

[[physics:def-lorentz-orthogonality-and-orthogonal-complement]]

## Facts & Assumptions

[F1] Given a smooth future timelike normal field along $S$, circle averaging and normalization supply a circle-invariant future unit timelike normal field. The normal boost action is the supplied differential action of $K$. [[def-circle-action-and-invariant-normal-data]] [[lem-killing-normal-boost-and-invariant-tensors]]

[F2] A compact framed spacelike surface has a normal exponential tube, and geodesics with prescribed initial data are unique. [[lem-author-ca4ffba327b3-compact-normal-exponential-tube]] [[physics:thm-gr-local-geodesics-and-exponential-map]]

[F3] Smooth Killing fields use the Lorentzian and horizon conventions; their local flows preserve the metric and its unique metric-compatible torsion-free connection, hence its geodesics. The flow law and geodesic invariance give equivariance of the exponential map. [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]] [[physics:def-gr-metric-selected-connection]] [[math:def-local-and-global-flow]]

[F4] Surface slice charts give smooth local tangent bases of $TS$. The normal fiber $N_pS=(T_pS)^{\perp_g}$ consists of the ambient vectors orthogonal to every tangent vector. The induced metric on $TS$ is positive definite, and the time-orientation field $N$ is smooth with $g(N,N)<0$; a timelike vector $w$ is future-directed when $g(w,N)<0$. The projection and initial normal field needed below are constructed in step 1.1. [[math:def-embedded-submanifold-and-slice-chart]] [[physics:def-lorentz-orthogonality-and-orthogonal-complement]] [[def-bifurcate-killing-horizon-data]] [[def-stationary-lorentzian-data]]

[A1] Work in ZFC. Choice is used through the compact normal-tube supplier's metrization and selection of a collision at each shrinking radius, and through the inherited smooth-manifold conventions. [[math:def-axiom-of-choice]]

## Proof

**Given:**The stated data and complete hypotheses.

**Goal:** Establish the conclusions on the domains and parameter ranges specified.

1.1 In a surface slice chart choose its smooth tangent basis $E_1,E_2$, put $h_{ij}=g(E_i,E_j)$, and write $h^{ij}$ for the inverse matrix. Since $h$ is positive definite, its determinant is positive and its inverse is smooth by the adjugate formula. For $V\in TM|_S$, define $PV=\sum_{i,j=1}^2h^{ij}g(V,E_j)E_i$. Direct pairing with $E_k$ gives $g(PV,E_k)=g(V,E_k)$, and $P$ is the identity on $TS$. Thus $V-PV\in NS$ and $TS\cap NS=\{0\}$ by positive definiteness. These two characterizations uniquely determine $P$, so the chartwise smooth projections agree on overlaps and give $TM|_S=TS\oplus NS$, with $NS=\ker P$ a smooth rank-two normal bundle. Set $n=N|_S-P(N|_S)$. Orthogonality yields $g(n,n)=g(N,N)-g(PN,PN)<0$ and $g(n,N)=g(n,n)<0$. Therefore $n$ is a globally defined smooth future timelike normal field, constructed without assuming a normal frame. [F4, algebra, construct]

2.1 Average and normalize the field $n$ from step 1.1 using [F1], obtaining the smooth invariant future unit normal $e_0$. Write $B(v)=\nabla_vK$ on $NS$ and set $e_1=\kappa^{-1}B(e_0)$. In any local future/outward orthonormal normal basis $(f_0,f_1)$, write $e_0=\cosh a\,f_0+\sinh a\,f_1$. The assumed boost matrix then gives $e_1=\sinh a\,f_0+\cosh a\,f_1$, which is outward, unit spacelike and orthogonal to $e_0$. The formula for $e_1$ proves smoothness. The connected circle preserves the normal-plane orientation and $e_0$, so it preserves the unique outward unit normal orthogonal to $e_0$, namely $e_1$. Changing a future/outward orthonormal basis in a Lorentzian two-plane is a Lorentz boost, which commutes with the positive-rate boost matrix; thus the stated $B$ matrix is unchanged in this frame. Apply [F2] to obtain a uniform tube. [F1, F2, F4, A1, step 1.1]

3.1 To justify [F3]'s equivariance, differentiate the pullback metric along a Killing flow: its derivative is the pullback of $\mathcal L_Kg=0$, so it is an isometry. Pulling back the connection preserves its two defining conditions; uniqueness identifies the pulled-back connection with the original one. Uniqueness of its geodesics gives $\phi_s^K\exp_y(w)=\exp_y(d\phi_s^K w)$ where defined. The fixed-point differential boost from [F1] therefore gives the claimed exact boost formula in $(u,v)$. The same argument for $Z$, with its invariant frame, gives its base-only action. Differentiating the hyperbolic-coordinate change proves $K=\partial_\tau$, and the other two vector-field formulas follow. [F1, F2, F3, step 2.1] ∎

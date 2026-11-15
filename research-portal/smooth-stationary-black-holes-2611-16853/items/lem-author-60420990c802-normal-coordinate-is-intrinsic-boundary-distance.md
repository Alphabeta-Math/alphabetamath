---
id: lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance
title: The inward normal coordinate is intrinsic distance from the boundary
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-60420990c802-uniform-inward-normal-exponential-collar
  - math:def-levi-civita-connection
  - math:def-smooth-variation-and-variation-field-of-a-curve
  - math:prop-geodesics-have-constant-speed-for-a-metric-compatible-connection
  - math:def-riemannian-distance-on-a-connected-manifold
  - math:def-riemannian-gradient-of-a-smooth-function
  - math:def-extended-riemannian-distance-on-a-disconnected-manifold
  - math:def-riemannian-speed-and-length
  - math:def-axiom-of-choice
dependency_roles:
  lem-author-60420990c802-uniform-inward-normal-exponential-collar: mathematical-premise
  math:def-levi-civita-connection: mathematical-premise
  math:def-smooth-variation-and-variation-field-of-a-curve: mathematical-premise
  math:prop-geodesics-have-constant-speed-for-a-metric-compatible-connection: mathematical-premise
  math:def-riemannian-distance-on-a-connected-manifold: mathematical-premise
  math:def-riemannian-gradient-of-a-smooth-function: mathematical-premise
  math:def-extended-riemannian-distance-on-a-disconnected-manifold: mathematical-premise
  math:def-riemannian-speed-and-length: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Work in ZFC. Let $(\Sigma,h)$ be the smooth Riemannian manifold with compact boundary $S$ and smooth positive metric up to $S$ of the uniform inward normal exponential collar supplier, and let $F$ be its supplied collar. After shrinking it one has $\rho(F(p,s))=s$, where $\rho(x)=\inf_{y\in S}d_h(x,y)$ uses extended intrinsic path distance in $\Sigma$: $d_h$ is the infimum of piecewise $C^1$ path lengths within a component, and is $+\infty$ between different components, with $\inf\varnothing=+\infty$. No connectedness assumption on $\Sigma$ is imposed. The pulled-back metric is $ds^2+h_s$ for a smooth family of positive metrics on $S$, and $\nabla_h\rho=\partial_s$, $|\nabla_h\rho|=1$. The coordinate and gradient extend smoothly to $S$.

## Facts & Assumptions

[F1] Work in ZFC, carrying the choice assumption of the uniform embedded normal collar supplier. That supplier gives the collar for the stated smooth metric and compact boundary. [[math:def-axiom-of-choice]] [[lem-author-60420990c802-uniform-inward-normal-exponential-collar]]

[F2] The Levi-Civita connection is metric compatible and torsion free; normal geodesics have constant unit speed and smooth variations commute covariantly in their two parameter directions. [[math:def-levi-civita-connection]] [[math:def-smooth-variation-and-variation-field-of-a-curve]] [[math:prop-geodesics-have-constant-speed-for-a-metric-compatible-connection]]

[F3] On each connected component, intrinsic distance is the infimum of piecewise $C^1$ path lengths. The extended-distance convention assigns $+\infty$ to pairs in distinct components, whose connecting path family is empty. The gradient is the metric dual of the differential wherever the function is smooth and real valued. [[math:def-riemannian-distance-on-a-connected-manifold]] [[math:def-extended-riemannian-distance-on-a-disconnected-manifold]] [[math:def-riemannian-gradient-of-a-smooth-function]]

[F4] The length of a piecewise $C^1$ path is the sum over its finitely many pieces of the integral of its metric speed, $|\dot\gamma|_h=\sqrt{h(\dot\gamma,\dot\gamma)}$. [[math:def-riemannian-speed-and-length]]

## Proof

**Given:** The hypotheses in the Statement, working in ZFC as in [F1].

**Goal:** Establish the stated conclusions.

1.1 Let $J$ be a variation field obtained by varying $p$ along $S$ while following the unit normal geodesics. Write $U=\partial_sF$. Then $h(U,U)=1$ and $\nabla_UU=0$. Torsion freeness for this variation and metric compatibility give $\partial_s h(J,U)=h(\nabla_UJ,U)=h(\nabla_JU,U)=\tfrac12J h(U,U)=0$. At $s=0$, $J\in TS$ and $U=\nu$, so this inner product is zero. Thus the metric has no mixed $ds$ terms and its $ds^2$ coefficient is one: $F^*h=ds^2+h_s$. Smoothness and positivity of $h_s$ follow from the collar embedding. [F1, F2]

2.1 In the infimum defining $\rho(x)$, boundary points in other components contribute only $+\infty$; all actual paths from $S$ to $x$ lie in the component of $x$. Let the larger available collar have width $a$ and take $x=F(p,s)$ with $s<a/4$. Its radial normal path has length $s$, giving $\rho(x)\le s$. Every path from $S$ to $x$ staying in the width-$a/2$ collar has length at least $\int|s'|\ge s$ by the Gaussian metric form. A path leaving that collar must first meet its outer face $s=a/2$, since there is no other interior boundary. Its initial portion already has length at least $a/2>s$. Hence allowing paths outside the collar cannot shorten the distance. Taking the infimum gives $\rho(x)=s$. [F1, F3, F4, step 1.1]

3.1 In these coordinates $d\rho=ds$ and the Gaussian metric dual is $\partial_s$. Therefore $\nabla\rho=\partial_s$ and its norm is one. Both extend smoothly to the boundary with inward direction. This proves all conclusions on the smaller collar, with no cut-locus assertion outside it. [F3, step 1.1, step 2.1] ∎

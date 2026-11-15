---
id: lem-author-58255dfd955f-unit-ball-rescaling
title: Rescaling a geometric Schrödinger equation without treating its potential
  as forcing
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-58255dfd955f-coordinate-schrodinger-form
  - math:thm-chain-rule-for-total-derivatives
  - math:cor-change-of-variables-for-compactly-supported-functions
  - math:thm-continuous-on-a-rectangle-is-riemann-integrable
dependency_roles:
  lem-author-58255dfd955f-coordinate-schrodinger-form: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:cor-change-of-variables-for-compactly-supported-functions: mathematical-premise
  math:thm-continuous-on-a-rectangle-is-riemann-integrable: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

In a coordinate ball $B_r(x_0)$ let $-\operatorname{div}(A\nabla u)+qu=0$, with $A$ symmetric and $A\ge\lambda I$ for some $\lambda>0$. Define $v(y)=u(x_0+ry)$ on $B_1$. Then $-\operatorname{div}_y(\widetilde A\nabla_yv)+\widetilde qv=0$, where $\widetilde A(y)=A(x_0+ry)/\lambda$ and $\widetilde q(y)=r^2q(x_0+ry)/\lambda$. Thus $\widetilde A\ge I$, $\|\widetilde A\|\le\|A\|/\lambda$ and $\|\widetilde q\|_\infty\le r^2\|q\|_\infty/\lambda$.

## Facts & Assumptions

**Given:** The divergence and weak forms, matrix $A$ and potential coefficient $q$ are those of [[lem-author-58255dfd955f-coordinate-schrodinger-form]]. Here $\|A\|$ is its operator-norm supremum. This is a homogeneous equation for an operator that includes the potential; $qu$ is not taken as an independently controlled forcing.

[F1] The coordinate supplier gives $u\in C^2_{\mathrm{loc}}$ and smooth $A,q$, with the weak identity for every real smooth test compactly supported in the interior coordinate ball. In this regularity all test integrands are continuous and compactly supported; the chart integrals in the calculation below may be evaluated as compactly supported Riemann integrals.

[F2] The total-derivative chain rule [[math:thm-chain-rule-for-total-derivatives]] applies to the affine maps $T(y)=x_0+ry$ and $T^{-1}(x)=(x-x_0)/r$, and to the differentiable functions composed with them. Here $r>0$, $DT=rI$ and $DT^{-1}=r^{-1}I$; these affine derivatives follow directly from their exact linear increments.

[F3] The compact-support substitution formula [[math:cor-change-of-variables-for-compactly-supported-functions]] applies to an injective $C^1$ map with invertible derivative and a compactly supported Riemann integrable function whose support lies in its image. Here $T:B_1\to B_r(x_0)$ is a smooth diffeomorphism, $|\det DT|=r^n$, and the integrands, extended by zero, are continuous and compactly supported in $B_r(x_0)$. Their restrictions to any nondegenerate bounding rectangle are Riemann integrable by [[math:thm-continuous-on-a-rectangle-is-riemann-integrable]]. This uses the compact-support Riemann formula, not a change-of-variables assertion for arbitrary $L^1$ data.

## Proof

**Given:** The hypotheses and data in the Statement and Facts & Assumptions.

**Goal:** Establish the conclusions of the Statement.

**Proof technique:** direct.

1.1 Fix a real $\eta\in C_c^\infty(B_1)$ and set $\varphi=\eta\circ T^{-1}$. Its support is $T(\operatorname{supp}\eta)$, a compact subset of $B_r(x_0)$, so it is an admissible test in the coordinate weak identity. The chain rule gives $\nabla_yv=r(\nabla_xu)\circ T$ and $(\nabla_x\varphi)\circ T=r^{-1}\nabla_y\eta$. The functions $A\nabla u\cdot\nabla\varphi$ and $qu\varphi$, extended by zero outside the ball, are continuous compactly supported Riemann integrands. Apply compact-support substitution separately to these functions using $|\det DT|=r^n$ to obtain $r^{n-2}\int_{B_1} A(T(y))\nabla_yv\cdot\nabla_y\eta\,dy+r^n\int_{B_1}q(T(y))v\eta\,dy=0$. Dividing by $\lambda r^{n-2}>0$ proves the claimed homogeneous weak equation for every such $\eta$. The transformed coefficients are smooth and $v$ is $C^2$, so the weak identity has the classical interpretation as well, by the same interior integration-by-parts and continuous-residual argument supplied by the coordinate lemma. [F1, F2, F3, given, algebra]

2.1 For every vector $\xi$, $\xi^T\widetilde A(y)\xi=\lambda^{-1}\xi^TA(T(y))\xi\ge|\xi|^2$. Since $T$ maps $B_1$ bijectively onto $B_r(x_0)$, composition preserves the coefficient suprema. Thus $\|\widetilde A\|\le\|A\|/\lambda$ and $\|\widetilde q\|_\infty\le r^2\|q\|_\infty/\lambda$. These statements do not estimate $qu$ by an additive source norm. [step 1.1, given, algebra] ∎

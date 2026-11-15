---
id: lem-null-optics-jacobian-comparison-input
title: Null optical comparison with affine and screen conventions
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-null-screen-expansion-and-focal-data
  - physics:def-gr-fx-null-screen-geometry
  - physics:def-gr-curvature-tensor-and-derived-tensors
  - physics:prop-gr-fx-null-raychaudhuri
  - physics:lem-gr-fx-null-focal-boundary-exclusion
  - math:def-axiom-of-choice
  - math:thm-algebra-of-derivatives
  - math:thm-chain-rule
  - math:thm-logarithm-derivative-and-integral
  - math:cor-mean-value-theorem
dependency_roles:
  def-null-screen-expansion-and-focal-data: mathematical-premise
  physics:def-gr-fx-null-screen-geometry: mathematical-premise
  physics:def-gr-curvature-tensor-and-derived-tensors: mathematical-premise
  physics:prop-gr-fx-null-raychaudhuri: mathematical-premise
  physics:lem-gr-fx-null-focal-boundary-exclusion: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-algebra-of-derivatives: mathematical-premise
  math:thm-chain-rule: mathematical-premise
  math:thm-logarithm-derivative-and-integral: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
dependency_level: 1
---

## Statement

Assume the axiom of choice. In the null-screen setting, let $F:U\times J\to M$ be a smooth future-directed affinely parametrized null geodesic hypersurface congruence normal to a spacelike two-surface $S$, with $F(p,0)=p$ and $L=\partial_\lambda F$. Fix $p\in U$ and work on the connected interval containing $0$ on which the screen Jacobi map $A_\lambda:T_pS\to\mathscr S_\lambda=L^\perp/\mathbb RL$ is invertible. Put $B=A'A^{-1}$, $\theta=\operatorname{tr}B$, and $\sigma=B-\frac12\theta\,\mathrm{id}$. The positive area Jacobian is $J(\lambda)=\sqrt{\det(\bar\gamma(A_\lambda e_i,A_\lambda e_j))}$ for any orthonormal basis $(e_1,e_2)$ of $T_pS$; thus $J(0)=1$.

On this interval $\theta'=-\theta^2/2-|\sigma|^2-\operatorname{Ric}(L,L)$ and $(\log J)'=\theta$. If $\operatorname{Ric}(L,L)\ge0$ along the relevant segment and $\theta(0)<0$, a focal instant occurs by $2/|\theta(0)|$, provided the smooth congruence is defined through that parameter.

If instead $[a,0]\subset J$ is regular, $a<0$, $\operatorname{Ric}(L,L)\ge0$ on it and $\theta(0)>0$, then $\theta(\lambda)\ge\theta(0)>0$ for $a\le\lambda\le0$ and $0<J(\lambda_1)\le J(\lambda_2)\le1$ whenever $a\le\lambda_1\le\lambda_2\le0$. Thus moving from $S$ toward the past, with parameter $s=-\lambda$, reverses the expansion sign and makes the screen Jacobian nonincreasing. This is a pointwise comparison of regular screen Jacobians; applying it to nonsmooth cuts requires a separate applicable area formula and endpoint-map hypotheses.

## Statement references

[[def-null-screen-expansion-and-focal-data]]

[[physics:def-gr-fx-null-screen-geometry]]

[[physics:def-gr-curvature-tensor-and-derived-tensors]]

[[physics:prop-gr-fx-null-raychaudhuri]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

[A1] Assume the axiom of choice, including the countable and dependent choice used by the geometric suppliers. [[math:def-axiom-of-choice]]

[F1] The null-screen definition supplies the positive screen metric, metric screen derivative, invertible regular Jacobi map, optical endomorphism, and the initial identification of $T_pS$ with the screen. [[def-null-screen-expansion-and-focal-data]] [[physics:def-gr-fx-null-screen-geometry]]

[F2] The Ricci tensor is the contraction of the curvature tensor of the metric-selected connection, with the curvature convention used in null Raychaudhuri. [[physics:def-gr-curvature-tensor-and-derived-tensors]] For the stated null hypersurface congruence, null Raychaudhuri gives the displayed evolution equation and, under nonnegative null Ricci curvature and negative initial expansion, the stated focal bound when the congruence is defined through the bound. [[physics:prop-gr-fx-null-raychaudhuri]]

[F3] Under its stated causal hypotheses, a focal instant excludes sufficiently nearby later points of the future generator from the future horismos of $S$. This fact does not assert the existence or regularity of a cut. [[physics:lem-gr-fx-null-focal-boundary-exclusion]]

[F4] The derivative product, quotient and chain rules and the identity $(\log x)'=1/x$ for $x>0$ apply to the smooth scalar functions below. [[math:thm-algebra-of-derivatives]] [[math:thm-chain-rule]] [[math:thm-logarithm-derivative-and-integral]]

[F5] A continuous function on a closed interval, differentiable in its interior, is nondecreasing when its derivative is nonnegative, by the mean value theorem. [[math:cor-mean-value-theorem]]

## Proof

**Given:**The stated congruence, regular interval, and the hypotheses in each conditional assertion.

**Goal:** Establish the screen transport identity and the stated focal and past-directed comparisons.

1.1 Choose an orthonormal basis of $T_pS$ and a smooth orthonormal screen frame locally along the generator. Let $M$ be the resulting matrix of $A$, and let $\Omega$ be the connection matrix of the screen frame. Metric compatibility makes $\Omega$ skew-symmetric, and the matrix of $B$ is $(M'+\Omega M)M^{-1}$. Expanding the determinant of the invertible $2\times2$ matrix and differentiating its entries gives $(\det M)'=(\det M)\operatorname{tr}(M'M^{-1})$. Since $\operatorname{tr}\Omega=0$, the definition of $J$ gives $J'/J=\operatorname{tr}B=\theta$; the sign of $\det M$ is locally constant. The chain rule for $\log$ gives $(\log J)'=\theta$. The initial screen identification makes $J(0)=1$. [F1, F4, given, algebra]

1.2 The evolution equation and the focal conclusion under the stated nonnegative Ricci, negative initial expansion and existence hypotheses are precisely the applications of the null Raychaudhuri supplier. [F2, given]

2.1 On a regular interval $[a,0]$ with nonnegative null Ricci curvature, the evolution equation gives $\theta'\le0$ because the screen shear norm is nonnegative. Applying the mean value theorem to $-\theta$ yields $\theta(\lambda)\ge\theta(0)>0$ for $a\le\lambda\le0$. Step 1.1 then gives $J'=\theta J>0$; another application of the mean value theorem and $J(0)=1$ give the stated inequalities. Reparametrizing by $s=-\lambda$ changes $d(\log J)/ds$ to $-\theta$, giving the past-directed sign and monotonicity. [F1, F5, step 1.1, step 1.2, given, algebra] ∎

## Remarks

The screen metric is positive, so the Jacobian above is independent of the chosen orthonormal basis. At a smooth regular cut whose differential is identified with the screen Jacobi map, it is the corresponding pointwise area Jacobian. The statement makes no such identification for a nonsmooth cut and does not infer a global cut parameter from focal data. The focal-exclusion fact is recorded for the later causal application, with its own hypotheses.

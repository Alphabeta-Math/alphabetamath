---
id: lem-author-86990d62062f-weighted-scalar-inverse
title: Scalar exterior inverse from exhaustion and uniform annular estimates
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-exterior-weighted-elliptic-data
  - def-stationary-asymptotic-decay-data
  - lem-author-86990d62062f-compact-domain-poisson
  - lem-author-86990d62062f-global-decaying-barrier
  - math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations
  - math:thm-boundary-schauder-estimate-for-the-dirichlet-problem
  - math:thm-arzela-ascoli-for-real-ck
  - math:thm-holder-spaces-on-bounded-domains-are-banach-spaces
dependency_roles:
  def-exterior-weighted-elliptic-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  lem-author-86990d62062f-compact-domain-poisson: mathematical-premise
  lem-author-86990d62062f-global-decaying-barrier: mathematical-premise
  math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations: mathematical-premise
  math:thm-boundary-schauder-estimate-for-the-dirichlet-problem: mathematical-premise
  math:thm-arzela-ascoli-for-real-ck: mathematical-premise
  math:thm-holder-spaces-on-bounded-domains-are-banach-spaces: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

On the end component under $h-\delta\in C^{3,\alpha}_{-1}$, $-1<\beta<0$, the zero-Dirichlet scalar Laplacian is a bounded isomorphism $X_\beta\to Y_\beta$, with $\|u\|_{4,\alpha,\beta}\le C\|\Delta_hu\|_{2,\alpha,\beta-2}$. The spaces and sign are exactly those of the weighted exterior definition. No assumption that the compact core is diffeomorphic to a Euclidean obstacle is required.

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] The weighted norms and coefficient decay use the fixed atlas and end chart. [[def-exterior-weighted-elliptic-data]] [[def-stationary-asymptotic-decay-data]]

[F2] Compact truncations are solvable and have local fourth-order estimates. [[lem-author-86990d62062f-compact-domain-poisson]]

[F3] A positive decaying barrier exists, including a controlled inner seam. [[lem-author-86990d62062f-global-decaying-barrier]]

[F4] Uniform local Schauder estimates and diagonal compactness can be applied on fixed charts. [[math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations]] [[math:thm-boundary-schauder-estimate-for-the-dirichlet-problem]] [[math:thm-arzela-ascoli-for-real-ck]]

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] The weighted norms and coefficient decay use the fixed atlas and end chart. [[def-exterior-weighted-elliptic-data]] [[def-stationary-asymptotic-decay-data]]

[F2] Compact truncations are solvable and have local fourth-order estimates. [[lem-author-86990d62062f-compact-domain-poisson]]

[F3] A positive decaying barrier exists, including a controlled inner seam. [[lem-author-86990d62062f-global-decaying-barrier]]

[F4] Uniform local Schauder estimates and diagonal compactness can be applied on fixed charts. [[math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations]] [[math:thm-boundary-schauder-estimate-for-the-dirichlet-problem]] [[math:thm-arzela-ascoli-for-real-ck]]



**Proof technique:** direct.

1.1 For $f\in Y_\beta$ solve $\Delta_hu_T=f$ on the smooth truncation $M_T$, with zero values on both its original and outer boundary, using the compact-domain lemma. Let $F=\|f\|_{2,\alpha,\beta-2}$. The norm definition gives $|f|\le C_0F\rho^{\beta-2}$. Comparing $\pm u_T-C_1FB$ using the barrier, with $C_1$ large enough, gives $|u_T|\le C_1FB$ independently of $T$. The comparison works at its seam by the derivative-jump argument, and on both boundary parts the barrier is positive. [F1, F2, F3]

2.1 Cover any annulus $A_R$ by a fixed finite number of balls of radius proportional to $R$, using larger annuli $\{R/2<r<4R\}$ for the estimates. Under $x=Ry$ the equation becomes $(h^{ij}(Ry)\partial_{ij}+Rb^i(Ry)\partial_i)u_T(Ry)=R^2f(Ry)$. These coefficients have uniformly bounded $C^{2,\alpha}$ norms and uniform ellipticity for large $R$, since $h-\delta\in C^{3,\alpha}_{-1}$. The fourth-order estimate of the compact-domain lemma, here using its interior argument, therefore gives $\|u_T(R\cdot)\|_{4,\alpha;A_1}\le C R^\beta F$ when $4R<T$. A finite ball cover controls close pairs in the annular Hölder seminorm; separated pairs are controlled by the derivative supremum divided by their fixed rescaled separation. The larger annulus data norm is bounded by the given norm using finitely many overlapping annuli. On each fixed compact core the boundary estimate has constants independent of $T$. [F1, F2, F4, step 1.1]

3.1 Exhaust $T\to\infty$. On each fixed compact region the fourth-order estimates give, by Ascoli on derivatives and a diagonal subsequence, convergence in $C^4$ (and $C^{4,\gamma}$ for $\gamma<\alpha$) to a zero-Dirichlet solution $u$. Hölder difference quotients pass to the limit for each pair of points, preserving the full exponent $\alpha$ and all weighted bounds from step 2.1. Thus $u\in X_\beta$ and $\Delta_hu=f$. For uniqueness a homogeneous solution tends uniformly to zero at infinity because $\beta<0$. Apply the scalar maximum principle on truncations and let their outer boundary supremum tend to zero, to $u$ and $-u$. The maximum principle itself follows by perturbing by a strictly subharmonic local test or by the positive-part energy comparison; its zeroth-order term is zero. Hence $u=0$. [F2, F3, F4, step 2.1]

4.1 The spaces here are Banach: a norm-Cauchy sequence converges on every compact chart in the ordinary Hölder Banach space; the limits agree on overlaps, and passing each annular norm inequality to the limit preserves the global weighted norm and Cauchy convergence. The zero trace subspace is closed. Product differentiation in $\Delta_h=h^{ij}\partial_{ij}+b^i\partial_i$ shows boundedness from $X_\beta$ to $Y_\beta$. The bound from steps 1.1 and 2.1 passes to the limit and gives a bounded inverse. This proves the Statement. [F1, step 3.1] ∎

---
title: Uniform boundary Schauder bootstrap after a C1-Holder seed
status: published
research_item: lem-author-14de055b8ceb-boundary-seeded-schauder-bootstrap
dependency_level: 3
sources:
  references:
    - title: Leon Simon, Lectures on PDE
      url: https://math.stanford.edu/~lms/lecs-on-pde.pdf
      locator: Lecture 12, Theorem 2-prime (local boundary non-divergence Schauder
        estimate), printed pp.134–135, PDF sheet70, specialized to m=1 and
        homogeneous Dirichlet data
      statement: For a second-order uniformly elliptic linear nondivergence equation
        with C^{0,beta} coefficients and C^{0,beta} RHS on a C^{2,beta} boundary
        patch, and homogeneous Dirichlet trace on its actual boundary, the
        C^{2,beta} norm on a smaller patch is controlled by the C0 solution norm
        and the C^{0,beta} RHS norm, with constants determined by ellipticity,
        coefficient Holder bounds, boundary charts and patch separations.
        Interior Theorem2 is its counterpart on balls.
      hypotheses: A classical C^{2,beta} solution on the closed local patch, uniform
        ellipticity, controlled C^{0,beta} principal and lower coefficients,
        controlled RHS, C^{2,beta} boundary and zero Dirichlet data on the
        boundary portion. Individual smoothness of the candidates supplies the
        classical regularity needed to use this a priori estimate; no uniform
        higher norm is assumed.
      reading_limits: Read the actual retained PDF sheet70, printed pp.134–135,
        including the boundary condition alternatives and Theorem2-prime. Read
        surrounding text defining boundary flattening and the local-to-global
        cover. The estimate is imported; its full Schauder proof is not
        reconstructed.
---

## Prerequisites

- [lem-author-14de055b8ceb-gaussian-maximal-graph-operator](item-lem-author-14de055b8ceb-gaussian-maximal-graph-operator)
- [lem-author-14de055b8ceb-uniform-elliptic-jet-extension](item-lem-author-14de055b8ceb-uniform-elliptic-jet-extension)
- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)
- [` Leon Simon, Lectures on PDE · Lecture 12, Theorem 2-prime (local boundary non-divergence Schauder estimate), printed pp.134–135, PDF sheet70, specialized to m=1 and homogeneous Dirichlet data `](https://math.stanford.edu/~lms/lecs-on-pde.pdf)


## Statement

Let a family of individually smooth solutions of $A^{ij}(x,u,Du)u_{ij}+b(x,u,Du)=0$ have zero height on a fixed smooth boundary patch, a common compact spacelike jet range, smooth uniformly controlled coefficients, uniform ellipticity and a uniform $C^{1,\beta}$ bound for one $0<\beta<1$. Then, on every fixed smaller boundary patch, all finite $C^{k,\beta}$ norms are uniformly bounded. No initial uniform $C^{4,\beta}$ norm is required. Consequently the family has uniform $C^{k,\alpha}$ bounds for every finite $k$ and every $0<\alpha<1$ on a smaller fixed patch.

## Facts & Assumptions

[F1] The smooth quasilinear operator and uniform elliptic/flattened jet control are [lem-author-14de055b8ceb-gaussian-maximal-graph-operator](item-lem-author-14de055b8ceb-gaussian-maximal-graph-operator) and [lem-author-14de055b8ceb-uniform-elliptic-jet-extension](item-lem-author-14de055b8ceb-uniform-elliptic-jet-extension). Use Holder norms as in [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms).

[F2] Import the local homogeneous-Dirichlet boundary Schauder estimate in Simon Lecture12 Theorem2-prime, pp.134–135, under the hypotheses precisely recorded in its source entry. It applies to the already smooth individual solutions and their tangential derivatives; it is an a priori estimate, not an assertion of a pre-existing uniform higher norm.

[F3] Apply the total-derivative chain rule [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) to the smooth coefficient maps composed with the solution jet, and repeatedly to their differentiated compositions. Apply the scalar mean value theorem [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem) componentwise along line segments in coefficient neighborhoods and fixed flattened boundary half-balls (or interior balls). Smoothness gives differentiability in the segment interior and continuity at its endpoints; boundary endpoint values are obtained by continuity from the interior.

## Proof

**Given:** The stated C1-Holder seed and smooth candidate solutions. **Goal:** Obtain uniform higher estimates up to the fixed boundary.

1.1 Freeze the realized coefficients along each solution. The seed makes $A(x,u,Du)$ and $b(x,u,Du)$ uniformly $C^{0,\beta}$, so [F2] gives a common $C^{2,\beta}$ bound on a smaller patch. Each candidate is individually smooth, satisfying the classical regularity prerequisite of that estimate. Interior balls use its interior counterpart. [F1, F2, F3, given]

2.1 Suppose a uniform $C^{m,\beta}$ bound is known, $m\ge2$. Differentiate the equation $m-1$ times in flat tangential directions. For $z=D_T^{m-1}u$, the principal term is $A^{ij}z_{ij}$. The chain-rule terms containing $Dz$ enter bounded $C^{0,\beta}$ first-order coefficients; every remaining term involves derivatives of $u$ of order at most $m$, hence has a uniform $C^{0,\beta}$ bound. Since the zero trace differentiates tangentially, $z=0$ on the flat boundary. [F2] bounds $z$ in $C^{2,\beta}$ on a smaller patch. This controls all derivatives of order $m+1$ with at most two normal directions. [F1, F2, F3, step 1.1, induction, algebra]

3.1 Solve the original equation for $u_{nn}$, using $A^{nn}\ge\lambda>0$, and differentiate it $m-1$ times. Recover the derivatives of order $m+1$ by increasing their number of normal indices: every other second-derivative slot has at least one tangential index and therefore fewer normal indices than the derivative currently solved for; derivatives of the coefficients involve only derivatives of $u$ through order $m$. Thus the already controlled derivatives and the previous normal-count stages give all remaining $C^{0,\beta}$ bounds. Iteration in $m$ on nested patches with a fixed smaller limiting patch proves all finite orders. A further bounded derivative implies the desired $C^{k,\alpha}$ bound for any $\alpha<1$: in a fixed convex flattened half-ball or interior ball, apply [F3] to $t\mapsto D^\gamma u(x+t(y-x))$, $0\le t\le1$, $|\gamma|=k$. The chain rule and scalar mean value theorem give $|D^\gamma u(y)-D^\gamma u(x)|\le C\|D^{k+1}u\|_\infty|y-x|$, including boundary endpoints by continuity. Dividing by $|y-x|^\alpha$ bounds the seminorm by $C\|D^{k+1}u\|_\infty\operatorname{diam}(B)^{1-\alpha}$; fixed smooth chart changes preserve these bounds by the same chain rule. A finite cover gives the estimate on the prescribed smaller patch: nearby pairs lie in a common chart, and separated pairs use the already bounded derivative suprema. [F1, F2, F3, step 2.1, induction, algebra] ∎

## External input

The local boundary linear Schauder estimate is an imported input. Use Simon Lecture12 Theorem2-prime, printed pp.134–135 (PDF sheet70), with $m=1$, zero Dirichlet trace, uniform ellipticity, C0-Holder coefficients and forcing, and a C2-Holder boundary chart. It bounds the C2-Holder norm on a smaller patch by the C0 solution norm and forcing norm, with the controlled structural and chart constants. This estimate is not proved here; the bootstrap above derives its application after a genuine C1-Holder seed.

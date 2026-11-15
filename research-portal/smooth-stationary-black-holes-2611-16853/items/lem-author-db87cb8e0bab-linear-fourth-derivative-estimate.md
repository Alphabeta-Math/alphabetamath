---
id: lem-author-db87cb8e0bab-linear-fourth-derivative-estimate
title: Linear fourth derivative bound with controlled realized coefficients
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - math:def-uniformly-elliptic-nondivergence-operator
  - math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - math:def-axiom-of-choice
dependency_roles:
  math:def-uniformly-elliptic-nondivergence-operator: mathematical-premise
  math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Work in ZFC. Let $n\ge2$ be an integer, $0<\alpha<1$, and let $A',A\subset\mathbb R^n$ be fixed bounded Euclidean annuli with $\overline{A'}\subset A$. Let $z$ be smooth on $A$ and solve $Lz=a^{ij}z_{ij}+b^jz_j+cz=f$, with summation over $i,j=1,\dots,n$. Suppose $a$ is symmetric and $\lambda|\xi|^2\le a^{ij}(x)\xi_i\xi_j\le\Lambda|\xi|^2$ for all $x\in A$ and $\xi\in\mathbb R^n$, where $0<\lambda\le\Lambda<\infty$. Suppose every component of $a,b,c$ has $C^{2,\alpha}(A)$ norm at most $M<\infty$, and $f\in C^{2,\alpha}(A)$. Then
$$\|z\|_{C^{4,\alpha}(A')}\le C\bigl(\|z\|_{L^\infty(A)}+\|f\|_{C^{2,\alpha}(A)}\bigr).$$
Here $C$ depends only on $n,\alpha,\lambda,\Lambda,M$ and the fixed annular geometry, including the positive separation $\operatorname{dist}(\overline{A'},\partial A)$. The coefficients are the realized functions of position, even if originally obtained by evaluating a nonlinear operator at $z,Dz$; their stated bounds must hold as functions of position. In particular the same $C$ works for any family with these common bounds.

## Facts & Assumptions

[F1] The interior linear Schauder estimate applies on a ball to a bounded classical solution of a uniformly elliptic equation with controlled $C^{0,\alpha}$ coefficients, including first-order and zeroth-order terms. Its constant depends only on dimension, exponent, ellipticity and the stated scaled coefficient bounds. [[math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations]]

[F2] Use the Euclidean Hölder norms and their scaled ball versions. The product estimate needed below follows directly from $p(x)q(x)-p(y)q(y)=p(x)(q(x)-q(y))+q(y)(p(x)-p(y))$: $[pq]_{0,\alpha}\le\|p\|_\infty[q]_{0,\alpha}+\|q\|_\infty[p]_{0,\alpha}$. [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

[F3] The repeated-index expression $L=a^{ij}\partial_i\partial_j+b^j\partial_j+c$ and the constants $\lambda,\Lambda$ have the uniformly elliptic nondivergence-operator convention. Differentiating the equation keeps this same principal operator. [[math:def-uniformly-elliptic-nondivergence-operator]]

[A1] Work in ZFC. Full Choice implies the Countable Choice assumed by the Schauder supplier; that implication is the use of Choice in each invocation of [F1]. [[math:def-axiom-of-choice]]

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the asserted estimate with the stated uniform dependence.

1.1 If $\|z\|_{L^\infty(A)}$ is infinite, the claimed inequality is automatic in the extended sense, so assume it finite and put $N=\|z\|_{L^\infty(A)}+\|f\|_{C^{2,\alpha}(A)}$. Fix intermediate open sets with $A'\Subset U_2\Subset U_1\Subset A$, where $V\Subset W$ means $\overline V$ is compact and contained in $W$. For any of these three successive inclusions, positive separation allows balls of a common fixed radius centered in the smaller set and contained in the larger set. Apply [F1] on these balls and convert its scaled norms to ordinary norms. The local derivative bounds give the global suprema on the smaller set. For Hölder quotients, pairs closer than half a target-ball radius lie in one target ball; separated pairs are bounded by twice the derivative supremum divided by that fixed distance to the power $\alpha$. A finite cover of the compact closure gives the same bounds, with constants depending only on the fixed geometry. The coefficient $C^{0,\alpha}$ bounds needed on each ball follow from the assumed $C^{2,\alpha}$ bounds and the derivative bounds on that convex ball. Consequently [F1] applied to $Lz=f$ gives $\|z\|_{C^{2,\alpha}(U_1)}\le CN$. [F1, F2, F3, A1, given, algebra]

2.1 Differentiate once in coordinate $k$. The equation is $Lz_k=f_k-a^{ij}_kz_{ij}-b^j_kz_j-c_kz$. On the balls contained in $U_1$, its right-hand side has $C^{0,\alpha}$ norm at most $CN$ by step 1.1, the coefficient bounds and the product estimate [F2]. Also $\|z_k\|_{L^\infty(U_1)}\le CN$. Applying [F1] with the same elliptic operator and assembling the ball estimates as in step 1.1 yields $\|z\|_{C^{3,\alpha}(U_2)}\le CN$. [step 1.1, F1, F2, F3, A1, given, algebra]

3.1 Differentiate twice. The equation for $z_{k\ell}$ has the same left-hand operator $L$ and right-hand side $f_{k\ell}-a^{ij}_{k\ell}z_{ij}-a^{ij}_kz_{ij\ell}-a^{ij}_\ell z_{ijk}-b^j_{k\ell}z_j-b^j_kz_{j\ell}-b^j_\ell z_{jk}-c_{k\ell}z-c_kz_\ell-c_\ell z_k$. On balls contained in $U_2$ its $C^{0,\alpha}$ norm is at most $CN$ by step 2.1, [F2] and the coefficient bounds; the same bound holds for $\|z_{k\ell}\|_\infty$. Apply [F1] to every $z_{k\ell}$ and assemble the estimates on $A'$ by step 1.1. This bounds $z$ in $C^{4,\alpha}(A')$ by $CN$. All constants depend only on the listed geometry, dimension, exponent, ellipticity and realized coefficient bounds, so the asserted family uniformity follows. [step 1.1, step 2.1, F1, F2, F3, A1, given, algebra] ∎

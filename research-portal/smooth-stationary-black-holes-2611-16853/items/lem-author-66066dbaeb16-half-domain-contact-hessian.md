---
id: lem-author-66066dbaeb16-half-domain-contact-hessian
title: Second-order contact on a closed half-domain has nonnegative Hessian
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-ck-and-multi-index-notation-in-several-variables
  - math:def-jacobian-matrix-and-gradient
  - math:def-hessian-and-euclidean-critical-point
  - math:def-definite-and-indefinite-hessian-quadratic-forms
  - math:cor-second-order-taylor-expansion-with-the-hessian
dependency_roles:
  math:def-ck-and-multi-index-notation-in-several-variables: mathematical-premise
  math:def-jacobian-matrix-and-gradient: mathematical-premise
  math:def-hessian-and-euclidean-critical-point: mathematical-premise
  math:def-definite-and-indefinite-hessian-quadratic-forms: mathematical-premise
  math:cor-second-order-taylor-expansion-with-the-hessian: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $\Omega\subseteq\mathbb R^n$, $n\ge1$, be a Euclidean domain with smooth boundary near $p\in\partial\Omega$. Here smooth boundary means that on an open neighborhood $U$ of $p$ there is a smooth real defining function $r$ with $r(p)=0$, $\nabla r(p)\ne0$, $\Omega\cap U=\{x\in U:r(x)>0\}$ and $\overline\Omega\cap U=\{x\in U:r(x)\ge0\}$. Let $f$ be $C^2$ up to this boundary near $p$, in the local-extension sense: after shrinking $U$, $f$ on $\overline\Omega\cap U$ is the restriction of some $F\in C^2(U)$. The boundary first jet $Df(p)$ is the row of first partial derivatives of $F$ at $p$, and $D^2f(p)=H_F(p)$ is its Hessian matrix; these jets are independent of the chosen extension, as proved below.

If $f\ge0$ on this closed one-sided neighborhood, $f(p)=0$ and $Df(p)=0$, then $D^2f(p)$ is positive semidefinite, meaning $v^TD^2f(p)v\ge0$ for every $v\in\mathbb R^n$. This is an elementary second-jet assertion and does not require a boundary Hopf lemma. The same conclusion holds at an interior minimum of a $C^2$ function.

## Statement references

[[math:def-ck-and-multi-index-notation-in-several-variables]]

[[math:def-jacobian-matrix-and-gradient]]

[[math:def-hessian-and-euclidean-critical-point]]

[[math:def-definite-and-indefinite-hessian-quadratic-forms]]

[[math:cor-second-order-taylor-expansion-with-the-hessian]]

## Facts & Assumptions

[F1] On an open Euclidean set, $C^2$ means that the function and all its coordinate partial derivatives of orders at most two exist and are continuous. The local-extension convention in the Statement is an explicit hypothesis, not an extension theorem. [[math:def-ck-and-multi-index-notation-in-several-variables]]

[F2] The gradient lists the first partial derivatives, and the Hessian matrix lists the second partial derivatives. [[math:def-jacobian-matrix-and-gradient]] [[math:def-hessian-and-euclidean-critical-point]]

[F3] A matrix $H$ is positive semidefinite when its quadratic form $Q(v)=v^THv$ is nonnegative for every vector $v$. [[math:def-definite-and-indefinite-hessian-quadratic-forms]]

[F4] For a $C^2$ scalar field $G$ on an open neighborhood of $p$, $G(p+h)=G(p)+\nabla G(p)\cdot h+\tfrac12h^TH_G(p)h+o(\|h\|^2)$. This applies to the ambient extension $F$ and to the defining function $r$, not directly to a function defined only on the closed side. [[math:cor-second-order-taylor-expansion-with-the-hessian]]

## Proof

**Given:** The local defining function, the $C^2$ extension and the nonnegative contact data in the Statement.

**Goal:** Prove that the extension-independent Hessian is positive semidefinite, including at an interior minimum.

1.1 Fix the defining function $r$ and an extension $F$ from the Statement, and put $\ell(v)=\nabla r(p)\cdot v$. For a fixed vector with $\ell(v)>0$, the Taylor formula for $r$ gives $r(p+tv)=t\ell(v)+O(t^2)>0$ for all sufficiently small $t>0$. Thus $p+tv\in\Omega\cap U$. Such vectors exist: $e=\nabla r(p)$ satisfies $\ell(e)=\|\nabla r(p)\|^2>0$. In particular $p$ is approached from the open side by $p+te$. [given, F1, F2, F4, algebra]

2.1 If $\widetilde F$ is another $C^2$ extension on an open neighborhood of $p$, restrict to a common neighborhood. The difference $F-\widetilde F$ vanishes on the open set $\Omega$ there. Its coordinate partial derivatives of orders one and two therefore vanish there by the definition of partial differentiation. Their continuity and the interior sequence $p+te\to p$ from step 1.1 show that these derivatives also vanish at $p$. The value and both boundary jets are consequently independent of the extension. [F1, F2, step 1.1]

3.1 Write $Q(v)=v^TH_F(p)v$. For each fixed $v$ with $\ell(v)>0$, step 1.1 and the hypotheses give $F(p+tv)=f(p+tv)\ge0$ for small $t>0$. Since $F(p)=0$ and its first partial derivatives at $p$ vanish, the Taylor formula gives $F(p+tv)=\tfrac12t^2Q(v)+o(t^2)$. Dividing by $t^2$ and letting $t\downarrow0$ proves $Q(v)\ge0$ for every such inward vector. [given, F2, F4, step 1.1, step 2.1, algebra]

4.1 If $\ell(v)<0$, apply step 3.1 to $-v$ and use $Q(-v)=Q(v)$. If $\ell(v)=0$, the vectors $v+\varepsilon e$ have positive $\ell$ for $\varepsilon>0$, with $e$ from step 1.1. The quadratic polynomial $Q(v+\varepsilon e)$ converges to $Q(v)$ as $\varepsilon\downarrow0$, so step 3.1 again gives $Q(v)\ge0$. This includes $v=0$. By the definition in [F3], the boundary Hessian is positive semidefinite. [F3, step 1.1, step 3.1, algebra]

5.1 At an interior minimum, for every fixed vector $v$ the points $p+tv$ lie in the domain for small $t>0$. Subtracting $f(p)$ in the same Taylor expansion, now for $f$ itself on an open neighborhood, gives $0\le f(p+tv)-f(p)=\tfrac12t^2v^TH_f(p)v+o(t^2)$ when $Df(p)=0$, hence $v^TH_f(p)v\ge0$. At an interior local minimum the latter condition follows as well: for each coordinate vector, the positive and negative difference quotients have opposite weak signs, and their common derivative must be zero. Thus the identical Hessian conclusion holds at an interior minimum. [F1, F2, F3, F4, step 3.1, algebra] ∎

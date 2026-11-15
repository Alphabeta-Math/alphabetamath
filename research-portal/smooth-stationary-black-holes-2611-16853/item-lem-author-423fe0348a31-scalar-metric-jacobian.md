---
title: Scalar metric Jacobian and weak-gradient identification
status: published
research_item: lem-author-423fe0348a31-scalar-metric-jacobian
dependency_level: 4
---

## Prerequisites

- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in ZFC. For a real-valued Lipschitz function $u$ on a smooth Riemannian three-region $(R,k)$, at every differentiability point the scalar coarea Jacobian of $du:T_xR\to\mathbb R$ is $J_1u=|du|_k=|\nabla_k u|$. At points with $du=0$ the value is zero. This is the one-dimensional-target (rank at most one) Jacobian, not an endpoint-map two-dimensional area Jacobian.

Precisely, for a linear functional $\ell:T_xR\to\mathbb R$, let $\ell^\sharp$ be the unique vector satisfying $k_x(\ell^\sharp,v)=\ell(v)$ for every $v\in T_xR$, and put $|\ell|_k=\sqrt{k_x(\ell^\sharp,\ell^\sharp)}$. Its adjoint $\ell^*:\mathbb R\to T_xR$ is characterized by $k_x(\ell^*t,v)=t\ell(v)$, with the usual Euclidean inner product on $\mathbb R$. Define the scalar metric coarea Jacobian by $J_1(\ell):=\sqrt{\det(\ell\ell^*)}$, where the determinant is on the one-dimensional target, and set $J_1u(x)=J_1(du_x)$ at differentiability points. There $\nabla_k u=(du_x)^\sharp$; almost everywhere this agrees with the metric weak gradient.

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice. This supplies the countable choice required by the Lipschitz differentiability and weak-derivative input used in step 2.1; the finite-dimensional calculation in step 1.1 needs no choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The metric is positive definite, so its matrix is invertible and defines the metric dual vector, dual norm and gradient used above. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[F2] Under the choice setting in [A1], the Lipschitz height has almost-everywhere chart derivatives equal to its weak derivatives; areas have the normalized metric Hausdorff convention. [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

## Proof

**Given:** The hypotheses and definitions in the Statement.

**Goal:** Prove the scalar Jacobian identity and its almost-everywhere weak-gradient interpretation.

1.1 For a linear functional $\ell$ on a finite-dimensional real inner-product space, the inverse metric gives a unique $\ell^\sharp$ with $k(\ell^\sharp,v)=\ell(v)$. The vector $t\ell^\sharp$ satisfies $k(t\ell^\sharp,v)=t\ell(v)$, hence $\ell^*t=t\ell^\sharp$. Thus $(\ell\ell^*)t=t\ell(\ell^\sharp)=t k(\ell^\sharp,\ell^\sharp)$, and the defining determinant on $\mathbb R$ gives $J_1(\ell)=\sqrt{k(\ell^\sharp,\ell^\sharp)}=|\ell|_k$. This also gives zero when $\ell=0$. [F1, given, algebra]

2.1 At each differentiability point take $\ell=du_x$ with the inner product $k_x$. The definitions and step 1.1 give $J_1u(x)=|du_x|_k=|\nabla_k u(x)|$. Under [A1], the weak and classical differential agree almost everywhere by [F2], so this is also the weak-gradient norm almost everywhere and identifies the scalar coarea integrand. No multiplicity or endpoint-map hypothesis is part of this calculation. [A1, F1, F2, step 1.1, algebra] ∎

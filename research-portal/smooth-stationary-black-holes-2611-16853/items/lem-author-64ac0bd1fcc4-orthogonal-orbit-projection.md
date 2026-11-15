---
id: lem-author-64ac0bd1fcc4-orthogonal-orbit-projection
title: Orthogonal projection away from the symmetry plane
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-64ac0bd1fcc4-orbit-gram-determinant
  - def-stationary-lorentzian-data
dependency_roles:
  lem-author-64ac0bd1fcc4-orbit-gram-determinant: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 8
---

## Statement

At a point where the matrix $H$ of [[lem-author-64ac0bd1fcc4-orbit-gram-determinant]] is invertible, write its inverse as $H^{ij}$ and put $P(V)=V-X_iH^{ij}g(X_j,V)$. Then $P(V)$ is orthogonal to both generators, $P(X_i)=0$, and $P$ is the identity on vectors orthogonal to both. The symmetric form $q(V,W)=g(V,W)-g(V,X_i)H^{ij}g(X_j,W)$ equals $g(PV,PW)$ and annihilates the orbit plane. All conventions are those of [[def-stationary-lorentzian-data]]. No global quotient coordinate or positivity theorem is asserted.

## Facts & Assumptions

[F1] The metric is symmetric and the invertible Gram matrix has $H^{ij}H_{jk}=\delta^i_k$; repeated indices $i,j$ are summed over $1,2$. [[lem-author-64ac0bd1fcc4-orbit-gram-determinant]] [[def-stationary-lorentzian-data]]

## Proof

**Given:**The metric, generators and invertible Gram matrix.

**Goal:** Check projection and the displayed form.

1.1 Direct substitution gives $g(X_k,PV)=g(X_k,V)-H_{ki}H^{ij}g(X_j,V)=0$. Substitution of $V=X_k$ gives $P(X_k)=0$. If $g(X_j,V)=0$ for both $j$, the defining formula gives $PV=V$. [given, F1]

2.1 Expand $g(PV,PW)$. The two cross terms are each $-g(V,X_i)H^{ij}g(X_j,W)$, and the quadratic term restores one copy by the inverse identity. The resulting expression is exactly $q(V,W)$; the projection property then shows it annihilates the orbit plane. [F1, step 1.1] ∎

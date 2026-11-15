---
title: Null second fundamental form descends to the screen quotient
status: draft
research_item: lem-author-254b7c4bab6d-null-form-screen-descent
dependency_level: 2
---

## Prerequisites

- [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)


## Statement

For a branch in [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair), suppose its smooth generator $L$ is geodesic up to reparametrization, $\nabla_LL=\kappa L$ for a smooth scalar $\kappa$. Then $B(X,Y)=g(\nabla_XL,Y)$ on $TH$ defines a symmetric bilinear form on $TH/\mathbb RL$. Its trace in the positive quotient metric agrees with the expansion computed on every spacelike section transverse to $L$. Thus the expansion uses no preferred section. The quotient and metric conventions are those of [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data), and the connection is as in [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

## Facts & Assumptions

[F1] The null generator spans the radical of the hypersurface tangent metric. Its quotient metric is positive definite, and a transverse spacelike section identifies isometrically with the quotient. The connection is torsion-free and metric-compatible. [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

## Proof

**Given:**The null hypersurface and pregeodesic generator in the Statement.

**Goal:** Establish descent, symmetry and section independence.

1.1 Metric compatibility gives $B(X,L)=\frac12Xg(L,L)=0$. The pregeodesic equation gives $B(L,Y)=\kappa g(L,Y)=0$. For tangent extensions $X,Y$, metric compatibility and $g(L,X)=g(L,Y)=0$ give $B(X,Y)-B(Y,X)=-g(L,\nabla_XY-\nabla_YX)=-g(L,[X,Y])=0$, since $[X,Y]$ is tangent to the hypersurface. Thus $B$ annihilates the kernel in both slots and is symmetric. [given, F1]

2.1 Changing a tangent representative by a multiple of $L$ therefore leaves $B$ unchanged. By the quotient metric and section identification in F1, its trace on the quotient equals its trace in any section representative. The definition of expansion is exactly that trace. [F1, step 1.1] ∎

---
title: Rescaling a null generator preserves zero expansion
status: published
research_item: lem-author-254b7c4bab6d-null-expansion-rescaling
dependency_level: 2
---

## Prerequisites

- [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold)


## Statement

For the horizon data of [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair), let $L$ be a local null generator and let $a$ be a smooth positive function on the branch. On any spacelike section the generator $L'=aL$ has $\chi'=a\chi$ and $\theta'=a\theta$. Consequently the zero-expansion condition does not depend on positive normalization. Use the expansion conventions of [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data).

## Facts & Assumptions

[F1] A null generator is orthogonal to every tangent vector of its null hypersurface; the null form and its trace are computed with the unchanged section metric. [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F2] An affine connection obeys $\nabla_X(fV)=X(f)V+f\nabla_XV$ for smooth $f$ and vector fields $X,V$. Apply this defining rule to the supplied Levi–Civita connection with $f=a$ and $V=L$, restricting the resulting identity to the section. [math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold)

## Proof

**Given:**The branch, section, $L$ and $a$ in the Statement.

**Goal:** Compute the two rescaled quantities.

1.1 For section tangent vectors $X,Y$, the connection product rule gives $g(\nabla_X(aL),Y)=X(a)g(L,Y)+a g(\nabla_XL,Y)=a\chi(X,Y)$, since $g(L,Y)=0$. [given, F1, F2]

2.1 The section metric has not changed. Taking its trace gives $\theta'=a\theta$; because $a>0$, either expansion vanishes exactly when the other does. [given, F1, step 1.1] ∎

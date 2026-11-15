---
title: Inversion is uniformly stable on compact chart families
status: draft
research_item: lem-author-89004136b63c-uniform-inverse-metric-continuity
dependency_level: 0
---

## Prerequisites

- [math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)
- [math:def-manifold-chart-coordinate-domain-and-coordinate-functions](https://alphabetamath.cc/item/def-manifold-chart-coordinate-domain-and-coordinate-functions)
- [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)
- [math:cor-determinant-is-a-polynomial-in-the-matrix-entries](https://alphabetamath.cc/item/cor-determinant-is-a-polynomial-in-the-matrix-entries)
- [math:thm-real-square-matrix-invertible-iff-determinant-nonzero](https://alphabetamath.cc/item/thm-real-square-matrix-invertible-iff-determinant-nonzero)
- [math:lem-algebra-of-continuous-real-maps-on-a-space](https://alphabetamath.cc/item/lem-algebra-of-continuous-real-maps-on-a-space)


## Statement

Let $K_j$ be finitely many compact subsets of coordinate domains and let $G_j(x)$ be continuous invertible real $4\times4$ matrix fields there. Given $\eta>0$, there is $\delta>0$ such that any matrix fields $\widetilde G_j$ satisfying $\max_{a,b}|\widetilde G_{j,ab}(x)-G_{j,ab}(x)|<\delta$ on all $K_j$ are invertible there and satisfy $\max_{a,b}|(\widetilde G_j^{-1})^{ab}(x)-(G_j^{-1})^{ab}(x)|<\eta$. No derivatives of the perturbation enter this assertion.

## Statement references

[math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)

[math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[math:def-manifold-chart-coordinate-domain-and-coordinate-functions](https://alphabetamath.cc/item/def-manifold-chart-coordinate-domain-and-coordinate-functions)

[math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)

[math:cor-determinant-is-a-polynomial-in-the-matrix-entries](https://alphabetamath.cc/item/cor-determinant-is-a-polynomial-in-the-matrix-entries)

[math:thm-real-square-matrix-invertible-iff-determinant-nonzero](https://alphabetamath.cc/item/thm-real-square-matrix-invertible-iff-determinant-nonzero)

[math:lem-algebra-of-continuous-real-maps-on-a-space](https://alphabetamath.cc/item/lem-algebra-of-continuous-real-maps-on-a-space)

## Facts & Assumptions

[F1] If $U\subseteq\mathbb R^{16}$ is open and every matrix in $U$ has nonzero determinant, apply the matrix-inversion regularity lemma with $m=16$, $n=4$, $r=1$ to the identity matrix-valued map on $U$. Its entry functions have constant first partial derivatives, so inversion on $U$ is $C^1$, in particular continuous. [math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)

[F2] Compactness has its finite ambient-subcover meaning, including the indexed-cover version and the empty-set case. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[F3] A coordinate domain is open in its manifold; its chart image is open in Euclidean space. Continuity means that the inverse image of a neighborhood is a neighborhood, equivalently that each open target neighborhood contains the image of some open source neighborhood. Apply this definition to the matrix fields on their coordinate domains with the usual topology on their sixteen real entries. [math:def-manifold-chart-coordinate-domain-and-coordinate-functions](https://alphabetamath.cc/item/def-manifold-chart-coordinate-domain-and-coordinate-functions) [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)

[F4] For fixed finite size the determinant is a finite sum of signed products of entries, and a real square matrix is invertible exactly when its determinant is nonzero. [math:cor-determinant-is-a-polynomial-in-the-matrix-entries](https://alphabetamath.cc/item/cor-determinant-is-a-polynomial-in-the-matrix-entries) [math:thm-real-square-matrix-invertible-iff-determinant-nonzero](https://alphabetamath.cc/item/thm-real-square-matrix-invertible-iff-determinant-nonzero)

[F5] Finite sums and products of continuous real-valued maps on a topological space are continuous. [math:lem-algebra-of-continuous-real-maps-on-a-space](https://alphabetamath.cc/item/lem-algebra-of-continuous-real-maps-on-a-space)

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the conclusions in the Statement.

1.1 Identify $M_4(\mathbb R)$ with $\mathbb R^{16}$ and write $d_\infty(A,B)=\max_{a,b}|A_{ab}-B_{ab}|$. The inequalities $d_\infty(A,B)\le\|A-B\|_2\le4d_\infty(A,B)$ show that maximum-entry and Euclidean neighborhoods give the same topology. Each entry projection is continuous since its change is at most $d_\infty(A,B)$. Thus [F4] and [F5] make determinant continuous. At a matrix $A$ with nonzero determinant, continuity gives a neighborhood where $|\det B-\det A|<|\det A|/2$, so the determinant stays nonzero. By [F4], $\mathrm{GL}_4(\mathbb R)$ is therefore open, independently of inversion. [F3, F4, F5, algebra]

2.1 Apply [F1] to the open set $\mathrm{GL}_4(\mathbb R)$ from step 1.1. Inversion is continuous there, also for $d_\infty$. Consequently, for every invertible center matrix $A$ and the given $\eta>0$, some $r>0$ has the following property: $d_\infty(B,A)<2r$ implies that $B$ is invertible and $d_\infty(B^{-1},A^{-1})<\eta/2$. Indeed, intersect an open neighborhood of $A$ contained in $\mathrm{GL}_4(\mathbb R)$ with the inverse image under inversion of the radius-$\eta/2$ ball about $A^{-1}$, and take a sufficiently small ball in that intersection. [F1, F3, step 1.1]

3.1 For each coordinate domain $U_j$, use all pairs $(x,r)$ with $x\in K_j$ and $r>0$ satisfying step 2.1 for $A=G_j(x)$. The sets $V_{j,x,r}=\{y\in U_j:d_\infty(G_j(y),G_j(x))<r\}$ are open in $U_j$ by continuity of $G_j$ and cover $K_j$. This uses neighborhoods in the coordinate domain, without identifying that domain itself with a Euclidean open set. Using all admissible pairs requires no selection of a radius at every point. [given, F3, step 2.1]

4.1 If every $K_j$ is empty, take $\delta=1$. Otherwise, [F2] gives a finite indexed subcover of each nonempty $K_j$ from step 3.1. Set $\delta>0$ to the minimum of the associated finitely many positive radii over the finitely many $j$. For $y\in K_j$ choose a selected $V_{j,x,r}$ containing it. Then $d_\infty(G_j(y),G_j(x))<r$ and $d_\infty(\widetilde G_j(y),G_j(x))<\delta+r\le2r$. Step 2.1 makes both matrices invertible and puts both inverses within $\eta/2$ of $G_j(x)^{-1}$. The triangle inequality gives $d_\infty(\widetilde G_j(y)^{-1},G_j(y)^{-1})<\eta$. Empty sets impose no restriction, and no continuity or derivatives of the perturbation were used. [given, F2, step 2.1, step 3.1, algebra] ∎

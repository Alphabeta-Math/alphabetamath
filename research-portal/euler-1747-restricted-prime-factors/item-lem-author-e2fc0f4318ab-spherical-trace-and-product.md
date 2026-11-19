---
title: Two spherical Hecke scalars determine the Satake pair
status: draft
research_item: lem-author-e2fc0f4318ab-spherical-trace-and-product
dependency_level: 4
---

## Prerequisites

- [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)
- [math:lem-topological-group-translations-and-inversion](https://alphabetamath.cc/item/lem-topological-group-translations-and-inversion)
- [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)
- [math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice)
- [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)
- [def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)
- [thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character)
- [math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)
- [lem-degree-two-spherical-index-cosets](item-lem-degree-two-spherical-index-cosets)
- [def-author-d45da46285be-satake-transform](item-def-author-d45da46285be-satake-transform)
- [math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots)
- [math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative)
- [math:def-hilbert-space](https://alphabetamath.cc/item/def-hilbert-space)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)


## Statement

Assume countable choice, so every sequence of nonempty sets has a choice function. For a prime $\ell$, let $G=\mathrm{GL}_2(\mathbb Q_\ell)$ and $K=\mathrm{GL}_2(\mathbb Z_\ell)$, the groups of invertible matrices over the $\ell$-adic field and its integer ring respectively. Give $G$ and $K$ the subspace topologies induced by their four entries in $\mathbb Q_\ell^4$ with its product of $\ell$-adic metric topologies. Take a unitary representation of $G$ acting by complex-linear isometries of a complex Hilbert space with norm-continuous orbits. Let $V$ be its space of smooth vectors, those fixed by an open subgroup. Suppose $V$ is irreducible and admissible, meaning it is nonzero with no proper nonzero invariant linear subspace and the vectors fixed by any compact open subgroup form a finite-dimensional space. Assume $V^K\ne0$.

Use the normalized Satake pair $\{u,v\}$, with multiplicity, characterized by the scalar $S(H)(u,v)$ on $V^K$ for each compactly supported, left and right $K$-invariant Hecke function $H$. The transform $S$ gives a coset $xK=\{xk:k\in K\}$ with triangular diagonal valuations $(r,s)$ weight $\ell^{(s-r)/2}X^rY^s$. Normalize the Hecke action by summing one term per coset $xK$. For $g\in G$, write $KgK=\{k_1gk_2:k_1,k_2\in K\}$. Let $I$ be the two-by-two identity matrix with ones on the diagonal and zeros off the diagonal. Write $\operatorname{diag}(a,d)=\begin{pmatrix}a&0\\0&d\end{pmatrix}$ and set $D=\operatorname{diag}(\ell,1)$. For a subset $A\subseteq G$, its indicator $\mathbf 1_A:G\to\mathbb C$ has value $1$ on $A$ and $0$ elsewhere. Let $\mathcal T_\ell$ and $\mathcal R_\ell$ be the Hecke operators of $\mathbf 1_{KDK}$ and $\mathbf 1_{(\ell I)K}$, respectively. Then their respective scalars are $\sqrt\ell(u+v)$ and $uv$.

## Facts & Assumptions

[F1] The spherical-character theorem supplies the one-dimensional $K$-fixed space and its normalized character under these hypotheses. The triangular coset coordinates, the transform and the coset action use the conventions in the statement ([thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character), [lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets), [def-author-d45da46285be-satake-transform](item-def-author-d45da46285be-satake-transform), [def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)).

[F2] The integral matrices of determinant valuation one have one triangular coset representative $\operatorname{diag}(1,\ell)$ and $\ell$ representatives $\begin{pmatrix}\ell&b\\0&1\end{pmatrix}$ with $0\le b<\ell$. This is the $e=1$ case of the index-coset lemma ([lem-degree-two-spherical-index-cosets](item-lem-degree-two-spherical-index-cosets)). Its statement also gives the determinant formula $ad-bc$ for a matrix with rows $(a,b)$ and $(c,d)$.

[F3] The normalized valuation is additive on products, with value one on $\ell$ and value zero on units of $\mathbb Z_\ell$ ([lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)). Determinants multiply, and the positive square root of $\ell$ exists because the real numbers are a complete ordered field and $\ell>0$ ([math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative), [math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots), [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete), [math:def-prime](https://alphabetamath.cc/item/def-prime)).

[F4] Under countable choice, $G$ is a Hausdorff topological group and $K$ is a compact open subgroup ([lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)). Left translation by a fixed element of a topological group is continuous ([math:lem-topological-group-translations-and-inversion](https://alphabetamath.cc/item/lem-topological-group-translations-and-inversion)). A continuous image of a compact space is compact ([math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)). A subset of $G$ is compact exactly when every cover of it by open subsets of $G$ has a finite subfamily that covers it ([math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)). A finite list of nonempty sets admits a choice of one element from each set ([math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice)).

[F5] For two-by-two matrices over a commutative ring the product has entries $(AB)_{ik}=a_{i1}b_{1k}+a_{i2}b_{2k}$, and the identity matrix $I$ has diagonal entries one and off-diagonal entries zero ([math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)).

## Proof

**Given:** The local field, subgroup and representation in the statement.

**Goal:** Compute both scalars in the specified normalization.

1.1 For $k\in K$, both $k$ and $k^{-1}$ have entries in $\mathbb Z_\ell$, so their determinants belong to $\mathbb Z_\ell$ by the formula in [F2]. The entries of $I$ give $\det(I)=1$, and multiplicativity gives $\det(k)\det(k^{-1})=1$. Thus $\det(k)$ is a unit of $\mathbb Z_\ell$ and has valuation zero. Every $k_1Dk_2$ with $k_1,k_2\in K$ has integral entries by the product rule, and its determinant has valuation one since $\det(D)=\ell$. [F2, F3, F5]

1.2 The set $KDK$ is invariant under multiplication on either side by $K$ because $K$ is a subgroup. The matrix $\ell I$ is central since $(\ell I)x=\ell x=x(\ell I)$ for every $x\in G$. Thus $(\ell I)K=K(\ell I)K$ and this set is invariant on both sides as well. For each $x\in G$, left translation $g\mapsto xg$ is continuous and maps the compact subset $K$ onto $xK$, so $xK$ is compact. In particular $(\ell I)K$ is compact. [F4, F5, given]

2.1 Conversely, take one of the representatives in [F2]. Put $P=\begin{pmatrix}0&1\\1&0\end{pmatrix}$ and, for $b\in\mathbb Z_\ell$, put $U_b=\begin{pmatrix}1&b\\0&1\end{pmatrix}$. Entrywise multiplication gives $P^2=I$ and $U_b U_{-b}=U_{-b} U_b=I$, so both $P$ and $U_b$ are in $K$. It also gives $PDP=\operatorname{diag}(1,\ell)$ and $U_bD=\begin{pmatrix}\ell&b\\0&1\end{pmatrix}$. Each representative and its full coset for right multiplication by $K$ therefore lie in $KDK$. By step 1.1, the cosets in [F2] give exactly $KDK$. [F1, F2, F5, step 1.1]

3.1 Let $\mathcal U$ be a family of open subsets of $G$ covering $KDK$. It covers each of the cosets in step 2.1, which are compact by step 1.2. By the ambient compactness criterion the set of finite lists from $\mathcal U$ covering each coset is nonempty. Use finite choice to select one such list for each of the $\ell+1$ cosets enumerated in [F2]. Concatenating the lists yields a list whose length is the sum of their lengths and whose members cover $KDK$. The converse direction of the ambient compactness criterion therefore gives compactness of $KDK$. Both indicators are complex-valued functions invariant on both sides under $K$ and zero outside compact sets, so they belong to the spherical Hecke algebra. [F1, F2, F4, step 2.1, step 1.2]

4.1 Each contributing coset has indicator value $1$. The single representative of diagonal valuations $(0,1)$ contributes $\sqrt\ell Y$ to the transform, and the $\ell$ representatives of valuations $(1,0)$ together contribute $\ell\ell^{-1/2}X=\sqrt\ell X$. The indicator of $(\ell I)K$ gives just $XY$, because its support is one coset of diagonal valuations $(1,1)$. Evaluating both transforms at $(u,v)$ gives $\sqrt\ell(u+v)$ and $uv$ on $V^K$. [F1, F2, F3, given, step 2.1, step 3.1] ∎

---
title: Normalized degree-two Satake transform by cosets
status: draft
research_item: def-author-d45da46285be-satake-transform
dependency_level: 2
---

## Prerequisites

- [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)
- [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-invertible-matrix-and-similarity-over-a-commutative-ring](https://alphabetamath.cc/item/def-invertible-matrix-and-similarity-over-a-commutative-ring)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)
- [def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:thm-int-comm-ring](https://alphabetamath.cc/item/thm-int-comm-ring)
- [math:def-group-ring](https://alphabetamath.cc/item/def-group-ring)
- [math:thm-group-ring-is-a-unital-algebra-with-basis-g](https://alphabetamath.cc/item/thm-group-ring-is-a-unital-algebra-with-basis-g)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [math:lem-finite-sum-reindexing-and-fubini](https://alphabetamath.cc/item/lem-finite-sum-reindexing-and-fubini)
- [math:lem-group-power-laws](https://alphabetamath.cc/item/lem-group-power-laws)
- [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)
- [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)
- [math:thm-external-direct-product-is-a-group](https://alphabetamath.cc/item/thm-external-direct-product-is-a-group)
- [math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group)
- [math:def-free-module-on-a-set-and-standard-basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis)
- [math:def-balanced-and-bilinear-maps](https://alphabetamath.cc/item/def-balanced-and-bilinear-maps)
- [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map)
- [math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)
- [math:def-countable](https://alphabetamath.cc/item/def-countable)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)


## Definition

Assume countable choice, meaning that a sequence of nonempty sets has a choice function. For a prime $\ell$, put $G=\mathrm{GL}_2(\mathbb Q_\ell)$ and $K=\mathrm{GL}_2(\mathbb Z_\ell)$, where $\mathbb Q_\ell$ is the $\ell$-adic field and $\mathbb Z_\ell$ its valuation ring. For either coefficient ring $R$, $\mathrm{GL}_2(R)$ consists of two-by-two matrices over $R$ with a two-sided inverse over $R$. Give $G$ and $K$ the subspace topologies on their four matrix entries in $\mathbb Q_\ell^4$ with its product of $\ell$-adic metric topologies. Write $G/K$ for the set of cosets $xK=\{xk:k\in K\}$. For each $xK$, take an upper-triangular representative $b$, meaning $b_{21}=0$, and set the integer pair $(r(x),s(x))$ to $(\nu(b_{11}),\nu(b_{22}))$. The valuation $\nu(a)$ of a nonzero field element is specified by $|a|_\ell=\ell^{-\nu(a)}$.

For $f$ in the spherical Hecke algebra $\mathcal H(G,K)$ of complex functions on $G$ that vanish outside a compact subset of $G$ and are invariant under $K$ on both sides, define its normalized Satake transform by
$$S(f)=\sum_{xK\in G/K} f(x)\ell^{(s(x)-r(x))/2}X^{r(x)}Y^{s(x)}.$$
The sum runs over the finitely many cosets on which $f$ is nonzero. The factor $\ell^{(s(x)-r(x))/2}$ is the positive real rational power of $\ell$, viewed in $\mathbb C$. It equals the $(s(x)-r(x))$th integer power of the positive square root of $\ell$.

The target is the complex Laurent polynomial algebra $\mathbb C[X^{\pm1},Y^{\pm1}]$, the group algebra of $\mathbb Z^2$ with coordinatewise addition. Its elements are finitely supported coefficient functions on $\mathbb Z^2$, with equality, addition and scalar multiplication defined coefficientwise. Write $X^rY^s$ for the basis monomial of $(r,s)$. The unit is $X^0Y^0$, and the product is the complex-bilinear extension of $(X^rY^s)(X^aY^b)=X^{r+a}Y^{s+b}$.

For $u,v\in\mathbb C^\times$, define evaluation of a Laurent polynomial $P$ with coefficients $a_{r,s}$ by
$$\operatorname{ev}_{u,v}(P)=\sum_{(r,s)\in\operatorname{supp}(P)}a_{r,s}u^rv^s.$$
Here $\operatorname{supp}(P)$ is the set of pairs with nonzero coefficient. The integer powers are taken in the multiplicative group $\mathbb C^\times$ of nonzero complex numbers.

## Definition references

[Metric topology](https://alphabetamath.cc/item/def-metric-topology)

[Product topology](https://alphabetamath.cc/item/def-product-topology)

[Subspace topology](https://alphabetamath.cc/item/def-subspace-topology-top)

[Compactness of a subset with its subspace topology](https://alphabetamath.cc/item/def-compact-space)

[Invertible matrices over a coefficient ring](https://alphabetamath.cc/item/def-invertible-matrix-and-similarity-over-a-commutative-ring)

[The cosets of a subgroup](https://alphabetamath.cc/item/def-coset)

[Extended absolute value on the completed field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)

[The additive group of integer pairs](https://alphabetamath.cc/item/thm-external-direct-product-is-a-group)

[Finitely supported coefficient families and their basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis)

[Bilinear multiplication](https://alphabetamath.cc/item/def-balanced-and-bilinear-maps)

[The group of units under multiplication](https://alphabetamath.cc/item/lem-ring-units-form-a-group)

## Facts & Assumptions

[F1] Under countable choice, with these topologies $G$ is a Hausdorff topological group and $K$ is a compact open subgroup. Each coset has an upper-triangular representative, and the integer valuations of its diagonal entries are independent of the representative ([math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice), [lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)). On the completed field $\mathbb Q_\ell$, $|\cdot|_\ell$ is the extension of the rational $\ell$-adic absolute value ([math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)).

[F2] A spherical Hecke function is constant on each coset $xK$ and nonzero on only finitely many cosets ([def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)).

[F3] Finite sums in a commutative additive monoid are independent of enumeration and are computed by starting at zero and adding the terms one by one. They split over a union of two disjoint finite sets and may be iterated over finite products ([math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid), [math:lem-finite-sum-reindexing-and-fubini](https://alphabetamath.cc/item/lem-finite-sum-reindexing-and-fubini)).

[F4] The prime $\ell>1$ is read in the real power using the composite of $n\mapsto n/1$ and the ordered inclusion of the rationals into the reals. This sends $1$ to $1$ and preserves strict order, so the real base is positive ([math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat), [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)). For a positive real base, a rational power with denominator two uses the positive square root and the integer power given by its numerator. The complex numbers form a commutative field containing the embedded reals ([math:def-prime](https://alphabetamath.cc/item/def-prime), [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power), [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)).

[F5] The integers form an additive group. Its direct product with itself is the group of integer pairs with coordinatewise addition, identity $(0,0)$ and inverse $(r,s)\mapsto(-r,-s)$ ([math:thm-int-comm-ring](https://alphabetamath.cc/item/thm-int-comm-ring), [math:thm-external-direct-product-is-a-group](https://alphabetamath.cc/item/thm-external-direct-product-is-a-group)). For a commutative coefficient ring and a group, the group ring has the group elements as a basis, with coefficientwise linear operations, a bilinear product extending the group law, and the basis element of the group identity as its algebra unit ([math:def-group-ring](https://alphabetamath.cc/item/def-group-ring), [math:def-free-module-on-a-set-and-standard-basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis), [math:thm-group-ring-is-a-unital-algebra-with-basis-g](https://alphabetamath.cc/item/thm-group-ring-is-a-unital-algebra-with-basis-g)).

[F6] The units of a unital ring form a group under multiplication ([math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group)). In a group, the zeroth power is the identity, negative integer powers use inverses, and $z^{a+b}=z^az^b$ for integer exponents $a,b$ ([math:def-group-power](https://alphabetamath.cc/item/def-group-power), [math:lem-group-power-laws](https://alphabetamath.cc/item/lem-group-power-laws)).

[F7] A complex-linear map preserves linear combinations, and a complex-bilinear map is linear in each variable ([math:def-linear-map](https://alphabetamath.cc/item/def-linear-map), [math:def-balanced-and-bilinear-maps](https://alphabetamath.cc/item/def-balanced-and-bilinear-maps)). A unital ring homomorphism preserves addition, multiplication and the unit ([math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)). A complex-algebra homomorphism is a unital ring homomorphism respecting the complex scalar structure maps ([math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)).

[F8] A finite set admits an enumeration without repetitions by a finite initial segment of the naturals, and every subset of a finite set is finite ([math:def-countable](https://alphabetamath.cc/item/def-countable), [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)). Induction on the number of terms proves a property once it holds at zero and passes from each number to its successor ([math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)).

[F9] A Cartesian product of two finite sets is finite ([math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)).

## Justification

**Given:** Countable choice, a prime $\ell$, $f\in\mathcal H(G,K)$ and nonzero complex numbers $u,v$.

**Goal:** Verify that the normalized coset sum defines a Laurent polynomial and that evaluation is a unital complex-algebra homomorphism.

1.1 Let $T$ be the finite set of cosets on which $f$ is nonzero. The value of $f$ and the two exponents are constant on each coset. The base is positive in the reals by [F4], and $(s-r)/2$ is rational, so the normalization defines a complex scalar. With $M_{(r,s)}=X^rY^s$, each summand is a complex scalar multiple of a basis monomial in the group algebra. Finite addition in that algebra therefore defines $S(f)$ as a Laurent polynomial. [F1, F2, F3, F4, F5]

1.2 Since $\mathbb C$ is a field with $1\ne 0$, its units are exactly its nonzero elements. Thus $\mathbb C^\times$ is a group under multiplication and all the integer powers in the evaluation sum are defined. For $\alpha=(r,s)$ put $w_\alpha=u^rv^s$. The integer power law and commutativity of complex multiplication give $w_{\alpha+\beta}=w_\alpha w_\beta$ and $w_{(0,0)}=1$. Evaluation depends only on the finitely supported coefficient function, and $\operatorname{ev}_{u,v}(M_\alpha)=w_\alpha$ since $M_\alpha$ has the sole nonzero coefficient $1$ at $\alpha$. [F3, F4, F5, F6]

2.1 Fix $(r,s)$ and let $T_{r,s}$ be the subset of $T$ with that exponent pair. Both $T_{r,s}$ and its complement in $T$ are finite. By coefficientwise addition, taking the $(r,s)$-coefficient commutes with the finite sum: the zero polynomial has coefficient zero, and adding another summand adds its coefficient. The resulting scalar sum has zero terms on $T\setminus T_{r,s}$, whose sum is zero by the finite sum recursion. Splitting across these two sets gives the coefficient $\sum_{xK\in T_{r,s}}f(x)\ell^{(s-r)/2}$. Thus a nonzero coefficient can occur only at an exponent pair realized in $T$. To enumerate the realized pairs, read an enumeration of $T$ and append each pair only on its first occurrence. This gives a finite list without repetitions, including the empty list if $T$ is empty. [F3, F5, F8, step 1.1]

2.2 Let $I,J$ be the finite supports of Laurent polynomials $P,Q$, with coefficients $a_\alpha,b_\alpha$, respectively. The set $I\cup J$ is finite by concatenating an enumeration of $I$ with one of $J\setminus I$, which is a subset of $J$. For $c,d\in\mathbb C$, the coefficient of $cP+dQ$ at $\alpha$ is $ca_\alpha+db_\alpha$, so its support also lies in $I\cup J$. For each of $P,Q,cP+dQ$, the evaluation sum can run over $I\cup J$ by splitting off the finite set of additional indices, whose terms are zero. For each index the field laws give $(ca_\alpha+db_\alpha)w_\alpha=c(a_\alpha w_\alpha)+d(b_\alpha w_\alpha)$. Summing this equality gives $\operatorname{ev}_{u,v}(cP+dQ)=c\operatorname{ev}_{u,v}(P)+d\operatorname{ev}_{u,v}(Q)$: the formula holds for the empty sum, and adding the next term preserves it by distributivity and commutativity of addition. This is the linear map criterion. [F3, F4, F5, F7, F8, step 1.2]

3.1 Since $I$ and $J$ are finite supports, $I\times J$ is finite by [F9]. Expand $P$ and $Q$ in the monomial basis over $I$ and $J$. Multiplication is linear in each variable, so applying linearity to each finite expansion gives $PQ=\sum_{(\alpha,\beta)\in I\times J}a_\alpha b_\beta M_{\alpha+\beta}.$ Each application to a finite sum follows by starting at zero and adding one term at a time. By linearity of evaluation and the definition on a monomial, evaluating this expansion gives the sum of $a_\alpha b_\beta w_{\alpha+\beta}=(a_\alpha w_\alpha)(b_\beta w_\beta)$. The finite product index rule and distributivity in $\mathbb C$ now give $\operatorname{ev}_{u,v}(PQ)=\left(\sum_{\alpha\in I}a_\alpha w_\alpha\right)\left(\sum_{\beta\in J}b_\beta w_\beta\right)=\operatorname{ev}_{u,v}(P)\operatorname{ev}_{u,v}(Q).$ Here multiplication by a fixed complex scalar distributes through each finite sum by iterating binary distributivity, including the empty sum since the scalar times zero is zero. [F3, F4, F5, F7, F8, F9, step 1.2, step 2.2]

4.1 The unit $M_{(0,0)}$ evaluates to $1$. Together with additivity and multiplicativity, this gives a unital ring homomorphism. Complex linearity gives $\operatorname{ev}_{u,v}(cM_{(0,0)})=c$, so evaluation respects the scalar structure map $c\mapsto cM_{(0,0)}$ of the Laurent algebra and the identity structure map of $\mathbb C$. Thus evaluation is a unital complex-algebra homomorphism on the target of the well-defined transform. [F5, F7, step 1.1, step 1.2, step 2.1, step 2.2, step 3.1] ∎

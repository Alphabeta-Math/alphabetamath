---
title: Order of the degree-two finite projective group
status: draft
research_item: lem-degree-two-projective-group-cardinality
dependency_level: 1
---

## Prerequisites

- [math:def-set-difference-and-symmetric-difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-finite-field-and-its-order](https://alphabetamath.cc/item/def-finite-field-and-its-order)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-matrices-over-a-commutative-ring](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring)
- [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)
- [math:def-group](https://alphabetamath.cc/item/def-group)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [math:lem-field-is-a-commutative-ring](https://alphabetamath.cc/item/lem-field-is-a-commutative-ring)
- [math:lem-ring-elementary-consequences](https://alphabetamath.cc/item/lem-ring-elementary-consequences)
- [math:ex-two-by-two-determinant-formula](https://alphabetamath.cc/item/ex-two-by-two-determinant-formula)
- [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)
- [math:cor-square-matrix-invertible-iff-determinant-is-a-unit](https://alphabetamath.cc/item/cor-square-matrix-invertible-iff-determinant-is-a-unit)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)
- [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:def-index](https://alphabetamath.cc/item/def-index)
- [math:lem-finite-coset-partition](https://alphabetamath.cc/item/lem-finite-coset-partition)
- [math:thm-lagrange](https://alphabetamath.cc/item/thm-lagrange)
- [math:lem-left-and-right-cosets-equinumerous](https://alphabetamath.cc/item/lem-left-and-right-cosets-equinumerous)


## Statement

Let $F$ be a finite field, with $q=|F|$ the number of elements in its underlying set. Write $F^\times=F\setminus\{0\}$ for its nonzero elements. Let $L=\mathrm{GL}_2(F)$ be the group of invertible $2\times 2$ matrices over $F$ under matrix multiplication. A matrix is invertible if it has a two-sided inverse for this product. Let $I$ denote the identity matrix, with ones on the diagonal and zeros elsewhere.

The degree-two projective linear group $G=\mathrm{PGL}_2(F)$ is the quotient of $L$ by the scalar subgroup $Z=\{tI:t\in F^\times\}$. Its elements are the left cosets $AZ=\{Az:z\in Z\}$, with product $(AZ)(BZ)=(AB)Z$. Then
$$|G|=\frac{(q^2-1)(q^2-q)}{q-1}=q(q^2-1).$$

For any subgroup $H$ of $G$, meaning a subset containing the identity and closed under products and inverses, let $H\backslash G=\{Hg:g\in G\}$ be the set of right cosets $Hg=\{hg:h\in H\}$. Then
$$|H\backslash G|=\frac{q(q^2-1)}{|H|}.$$

## Facts & Assumptions

[F1] A field has associative and commutative addition and multiplication, additive identity $0$, multiplicative identity $1\ne 0$, additive inverses, distributivity, and a multiplicative inverse for every nonzero element ([field](https://alphabetamath.cc/item/def-field)). Its operations make it a commutative ring, meaning that addition forms a commutative group and multiplication is associative and commutative, has an identity and distributes over addition ([field as a commutative ring](https://alphabetamath.cc/item/lem-field-is-a-commutative-ring)), and $0t=0$ for every $t\in F$ ([zero multiplication](https://alphabetamath.cc/item/lem-ring-elementary-consequences)). Thus the units, elements with a multiplicative inverse, are exactly $F^\times$. A finite field has a finite underlying set, and its order is the cardinality of that set ([finite field and its order](https://alphabetamath.cc/item/def-finite-field-and-its-order)).

[F2] The cardinality $|A|$ of a finite set $A$ is the unique natural number $n$ for which there is a bijection from $A$ to $\{0,\ldots,n-1\}$, the empty set for $n=0$. A bijection is a map for which each target element has exactly one preimage, and it transports finiteness and cardinality ([bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection), [finite cardinality](https://alphabetamath.cc/item/def-finite-cardinality)).

[F3] A $2\times 2$ matrix over $F$ is an array of two rows and two columns with entries in $F$ ([matrices and columns](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring)). Numbering rows and columns from $1$, the matrix product has entries $(AB)_{ij}=a_{i1}b_{1j}+a_{i2}b_{2j}$. The identity $I$ has diagonal entries $1$ and all other entries $0$, so $tI$ has diagonal entries $t$ and all other entries $0$ ([matrix product, identity and scaling](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)).

[F4] A group has an associative product, a two-sided identity and two-sided inverses ([group](https://alphabetamath.cc/item/def-group)). A subgroup satisfies the identity, product and inverse conditions in the Statement ([subgroup](https://alphabetamath.cc/item/def-subgroup)). The left and right cosets of a subgroup $K$ represented by $g$ are $gK=\{gk:k\in K\}$ and $Kg=\{kg:k\in K\}$ ([cosets](https://alphabetamath.cc/item/def-coset)). The quotient group here consists of the left cosets with their representative product. The projective linear group definition supplies the groups $L$ and $G$, the subgroup $Z$, and the quotient construction over the field $F$ ([quotient group](https://alphabetamath.cc/item/def-quotient-group), [degree-two projective linear group](item-def-degree-two-projective-linear-group)).

[F5] Over a commutative ring the determinant of a $2\times 2$ matrix with first column $(a,c)$ and second column $(b,d)$ is the scalar $ad-bc$ ([two-by-two determinant formula](https://alphabetamath.cc/item/ex-two-by-two-determinant-formula)). For a square matrix of positive size over a commutative ring, the determinant is defined by the signed Leibniz formula ([determinant definition](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)). A square matrix of positive size over a commutative ring is invertible exactly when its determinant is a unit ([invertibility criterion](https://alphabetamath.cc/item/cor-square-matrix-invertible-iff-determinant-is-a-unit)).

[F6] The Cartesian product $A\times B$ is the set of ordered pairs with first entry in $A$ and second entry in $B$. For finite $A,B$ its cardinality is $|A|\,|B|$ ([Cartesian product](https://alphabetamath.cc/item/def-cartesian-product), [product rule](https://alphabetamath.cc/item/thm-product-rule)). A subset of a finite set is finite ([finite subsets](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)). Two ordered pairs are equal exactly when their first entries agree and their second entries agree ([coordinatewise equality of ordered pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)).

[F7] The cardinality of a union of a finite family of pairwise disjoint finite sets, meaning distinct members share no elements, is the sum of their cardinalities ([sum rule](https://alphabetamath.cc/item/thm-sum-rule)). A sum over a finite index set $S$ adds the values once for each element of $S$, in any enumeration, and if every value is $c$, the sum is $|S|c$ ([finite sum and constant clause](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)).

[F8] For a finite group $J$ and a subgroup $K$, the set $J/K$ of left cosets is finite and its cardinality is the index $[J:K]$ ([index](https://alphabetamath.cc/item/def-index), [finite coset set](https://alphabetamath.cc/item/lem-finite-coset-partition)). Lagrange's theorem gives $|J|=[J:K]|K|$ ([Lagrange's theorem](https://alphabetamath.cc/item/thm-lagrange)). For any group and subgroup the map $gK\mapsto Kg^{-1}$ is a well-defined bijection from left cosets to right cosets ([left and right coset bijection](https://alphabetamath.cc/item/lem-left-and-right-cosets-equinumerous)).

[F9] For sets $A$ and $B$, an element lies in $A\setminus B$ exactly when it belongs to $A$ and does not belong to $B$. [set difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference)

## Proof

**Given:** A finite field $F$ of order $q$ and a subgroup $H$ of $G=\mathrm{PGL}_2(F)$ as in the Statement.

**Goal:** Compute $|G|$ and the number of right cosets of $H$.

1.1 Write $V=F\times F$, viewing an ordered pair as a column. For columns $v=(a,c)$ and $w=(b,d)$, write $[v\ w]$ for the matrix with those columns. The matrix has positive size over the commutative ring $F$. By the determinant criterion it belongs to $L$ exactly when $ad-bc\ne 0$, since the units of $F$ are precisely its nonzero elements. If $v=(0,0)$ the scalar is zero. [F1, F3, F4, F5, F6]

1.2 The product rule gives $|V|=q^2$. The sets $F^\times$ and $V\setminus\{(0,0)\}$ are finite subsets. Each complement and its excluded singleton are disjoint and together exhaust the ambient set. Separating the respective singletons, each of cardinality $1$, gives $|F^\times|=q-1$ and $|V\setminus\{(0,0)\}|=q^2-1$ by the sum rule. Since $0$ and $1$ are distinct elements of $F$, $q\ge 2$. [given, F1, F2, F6, F7, F9]

2.1 Fix $v=(a,c)\ne(0,0)$ and write $Fv=\{(ta,tc):t\in F\}$ for its scalar multiples. If $w=(ta,tc)$ then $ad-bc=a(tc)-(ta)c=0$. Conversely, if $ad-bc=0$ and $a\ne 0$, set $t=a^{-1}b$. Then $b=ta$ and $d=a^{-1}bc=tc$. If $a=0$ then $c\ne 0$, and $bc=0$ gives $b=0$ by multiplication by $c^{-1}$. In this case set $t=c^{-1}d$ to get $(b,d)=(ta,tc)$. Thus the allowed second columns are exactly $V\setminus Fv$. [F1, F9, step 1.1]

3.1 For nonzero $v=(a,c)$, the map $t\mapsto(ta,tc)$ from $F$ to $Fv$ reaches every element of $Fv$ by definition. If $(ta,tc)=(sa,sc)$, the two pairs agree coordinate by coordinate. Choose a nonzero coordinate of $v$ and multiply the equality in that coordinate by its inverse to get $t=s$. The bijection gives $|Fv|=q$. A column lies in $V\setminus Fv$ exactly when it belongs to $V$ and does not belong to $Fv$. Hence $Fv$ and $V\setminus Fv$ are disjoint subsets with union $V$. Both are finite, so the sum rule gives $|V\setminus Fv|=q^2-q$. [F1, F2, F6, F7, F9, step 2.1, step 1.2]

4.1 For each nonzero first column $v$, the corresponding set of matrices in $L$ is in bijection with $V\setminus Fv$ by taking the second column. The inverse sends $w$ to $[v\ w]$. The two column pairs determine the four entries of this matrix. Every element of $L$ belongs to exactly one of these sets, since its first column is unique and nonzero. The sum rule over the $q^2-1$ possible first columns, with constant value $q^2-q$, gives $|L|=(q^2-1)(q^2-q)$ and shows $L$ is finite. [F2, F3, F6, F7, step 1.1, step 2.1, step 1.2, step 3.1]

5.1 The map $t\mapsto tI$ from $F^\times$ to $Z$ reaches every element of $Z$, and reading a diagonal entry recovers $t$, so $|Z|=q-1$. The scalar subgroup $Z$ lies in the finite group $L$, and the elements of $G$ are the left cosets of $Z$. Therefore $G$ is finite and $|G|=[L:Z]=|L|/|Z|$ by Lagrange's theorem. Using $q^2-q=q(q-1)$ and $q-1>0$ gives $|G|=(q^2-1)(q^2-q)/(q-1)=q(q^2-1)$. [F2, F3, F4, F8, step 1.2, step 4.1]

6.1 Apply Lagrange's theorem to the finite group $G$ and its subgroup $H$. The group identity belongs to $H$, so $|H|>0$. The bijection $gH\mapsto Hg^{-1}$ carries the finite left coset set to $H\backslash G$, whence $|H\backslash G|=[G:H]=|G|/|H|=q(q^2-1)/|H|$. This proves the right coset formula and completes the two counts. [given, F2, F4, F8, step 5.1] ∎

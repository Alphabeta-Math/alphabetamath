---
title: Norm surjectivity for a quadratic finite field
status: draft
research_item: lem-quadratic-finite-field-norm-surjectivity
dependency_level: 0
---

## Prerequisites

- [math:def-finite-field-and-its-order](https://alphabetamath.cc/item/def-finite-field-and-its-order)
- [math:def-field-extension-generated-subfields-and-simple-extension](https://alphabetamath.cc/item/def-field-extension-generated-subfields-and-simple-extension)
- [math:def-extension-degree-and-finite-extension](https://alphabetamath.cc/item/def-extension-degree-and-finite-extension)
- [math:def-dimension](https://alphabetamath.cc/item/def-dimension)
- [math:def-subfield](https://alphabetamath.cc/item/def-subfield)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-field-norm-and-trace](https://alphabetamath.cc/item/def-field-norm-and-trace)
- [math:def-determinant-of-a-linear-operator](https://alphabetamath.cc/item/def-determinant-of-a-linear-operator)
- [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [math:thm-operator-determinant-is-basis-independent](https://alphabetamath.cc/item/thm-operator-determinant-is-basis-independent)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis)
- [math:thm-unique-coordinates-with-respect-to-an-ordered-basis](https://alphabetamath.cc/item/thm-unique-coordinates-with-respect-to-an-ordered-basis)
- [math:def-relative-frobenius-of-a-finite-field-extension](https://alphabetamath.cc/item/def-relative-frobenius-of-a-finite-field-extension)
- [math:def-f-homomorphisms-and-embeddings-of-field-extensions](https://alphabetamath.cc/item/def-f-homomorphisms-and-embeddings-of-field-extensions)
- [math:def-field-homomorphism](https://alphabetamath.cc/item/def-field-homomorphism)
- [math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group](https://alphabetamath.cc/item/thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group)
- [math:def-finite-galois-extension-and-galois-group](https://alphabetamath.cc/item/def-finite-galois-extension-and-galois-group)
- [math:def-relative-field-automorphism-group](https://alphabetamath.cc/item/def-relative-field-automorphism-group)
- [math:def-coordinate-column-and-matrix-of-a-linear-map](https://alphabetamath.cc/item/def-coordinate-column-and-matrix-of-a-linear-map)
- [math:def-matrices-over-a-commutative-ring](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring)
- [math:lem-field-is-a-commutative-ring](https://alphabetamath.cc/item/lem-field-is-a-commutative-ring)
- [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)
- [math:def-inversions-inversion-number-and-sign](https://alphabetamath.cc/item/def-inversions-inversion-number-and-sign)
- [math:thm-multiplicative-group-of-a-finite-field-is-cyclic](https://alphabetamath.cc/item/thm-multiplicative-group-of-a-finite-field-is-cyclic)
- [math:def-generated-subgroup](https://alphabetamath.cc/item/def-generated-subgroup)
- [math:lem-cyclic-subgroup-is-the-set-of-powers](https://alphabetamath.cc/item/lem-cyclic-subgroup-is-the-set-of-powers)
- [math:lem-group-power-laws](https://alphabetamath.cc/item/lem-group-power-laws)
- [math:def-order-in-a-group](https://alphabetamath.cc/item/def-order-in-a-group)
- [math:lem-order-characterisation](https://alphabetamath.cc/item/lem-order-characterisation)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)
- [math:def-finite-symmetric-group-and-permutation-notation](https://alphabetamath.cc/item/def-finite-symmetric-group-and-permutation-notation)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)


## Statement

Let $F$ be a finite field of order $q=|F|$ and let $E/F$ be a quadratic extension, meaning $F$ is a subfield of $E$ and $[E:F]=\dim_F E=2$. For a field $K$, write $K^\times=K\setminus\{0\}$ with field multiplication. For every $z\in E^\times$, the field norm satisfies $N_{E/F}(z)=\det(m_z)=z^{q+1}$, where $m_z$ is the $F$-linear map $x\mapsto zx$ on $E$. The norm maps onto $F^\times$, meaning every element of $F^\times$ is the norm of some element of $E^\times$.

## Facts & Assumptions

[F1] A finite field has a finite underlying set, and its order is the cardinality of that set ([math:def-finite-field-and-its-order](https://alphabetamath.cc/item/def-finite-field-and-its-order)). A field has distinct elements $0$ and $1$. Its nonzero elements form a commutative group under multiplication with identity $1$, and multiplication distributes over addition ([math:def-field](https://alphabetamath.cc/item/def-field)).

[F2] We identify the base field with its image in a field extension ([math:def-field-extension-generated-subfields-and-simple-extension](https://alphabetamath.cc/item/def-field-extension-generated-subfields-and-simple-extension)). A subfield shares the ambient field's $0$ and $1$ and inherits its field operations, including subtraction and inversion of nonzero elements ([math:def-subfield](https://alphabetamath.cc/item/def-subfield)). The extension degree is the dimension over the base field ([math:def-extension-degree-and-finite-extension](https://alphabetamath.cc/item/def-extension-degree-and-finite-extension)). Dimension two gives a basis of two elements ([math:def-dimension](https://alphabetamath.cc/item/def-dimension)), which we can list in order ([math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis)). A list $(v,w)$ is an ordered basis exactly when every vector has a unique expression $av+bw$ with $a,b\in F$ ([math:thm-unique-coordinates-with-respect-to-an-ordered-basis](https://alphabetamath.cc/item/thm-unique-coordinates-with-respect-to-an-ordered-basis)).

[F3] An $F$-linear map preserves linear combinations over $F$ ([math:def-linear-map](https://alphabetamath.cc/item/def-linear-map)). The field norm is defined by $N_{E/F}(z)=\det(m_z)$, where $m_z(x)=zx$ ([math:def-field-norm-and-trace](https://alphabetamath.cc/item/def-field-norm-and-trace)). The operator determinant is the determinant of a coordinate matrix ([math:def-determinant-of-a-linear-operator](https://alphabetamath.cc/item/def-determinant-of-a-linear-operator)), whose value is independent of the ordered basis ([math:thm-operator-determinant-is-basis-independent](https://alphabetamath.cc/item/thm-operator-determinant-is-basis-independent)).

[F4] For finite fields $F\subseteq E$ with $|F|=q$, the relative Frobenius $\sigma(x)=x^q$ is an $F$-automorphism of $E$ ([math:def-relative-frobenius-of-a-finite-field-extension](https://alphabetamath.cc/item/def-relative-frobenius-of-a-finite-field-extension)). An $F$-automorphism is a bijective field homomorphism fixing $F$ pointwise ([math:def-f-homomorphisms-and-embeddings-of-field-extensions](https://alphabetamath.cc/item/def-f-homomorphisms-and-embeddings-of-field-extensions)). A field homomorphism preserves addition, multiplication and $1$ ([math:def-field-homomorphism](https://alphabetamath.cc/item/def-field-homomorphism)). In degree two the extension is Galois and its Galois group is cyclic of order two, generated by $\sigma$ ([math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group](https://alphabetamath.cc/item/thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group)). The Galois group is the group of relative automorphisms ([math:def-finite-galois-extension-and-galois-group](https://alphabetamath.cc/item/def-finite-galois-extension-and-galois-group)) with composition as its operation ([math:def-relative-field-automorphism-group](https://alphabetamath.cc/item/def-relative-field-automorphism-group)).

[F5] The columns of a linear map's matrix are the coordinate columns of the images of its ordered basis vectors ([math:def-coordinate-column-and-matrix-of-a-linear-map](https://alphabetamath.cc/item/def-coordinate-column-and-matrix-of-a-linear-map)). A two-by-two matrix over $F$ is a square matrix over a commutative ring ([math:def-matrices-over-a-commutative-ring](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring), [math:lem-field-is-a-commutative-ring](https://alphabetamath.cc/item/lem-field-is-a-commutative-ring)). The Leibniz determinant is indexed by $S_2$ ([math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)), the bijections of $\{0,1\}$ ([math:def-finite-symmetric-group-and-permutation-notation](https://alphabetamath.cc/item/def-finite-symmetric-group-and-permutation-notation)). If a bijection sends $0$ to $0$, it must send $1$ to $1$. If it sends $0$ to $1$, it must send $1$ to $0$. Hence the identity and swap are the only permutations. The identity has zero inversions and the swap has one, so their signs are $+1$ and $-1$, respectively ([math:def-inversions-inversion-number-and-sign](https://alphabetamath.cc/item/def-inversions-inversion-number-and-sign)). Thus the determinant is the product of the diagonal entries minus the product of the off-diagonal entries.

[F6] The nonzero elements of a finite field form a cyclic group ([math:thm-multiplicative-group-of-a-finite-field-is-cyclic](https://alphabetamath.cc/item/thm-multiplicative-group-of-a-finite-field-is-cyclic)). A cyclic group is the subgroup generated by one element, called a generator ([math:def-generated-subgroup](https://alphabetamath.cc/item/def-generated-subgroup)), and that subgroup consists of its integer powers ([math:lem-cyclic-subgroup-is-the-set-of-powers](https://alphabetamath.cc/item/lem-cyclic-subgroup-is-the-set-of-powers)). Positive powers are repeated products and the zeroth power is the identity ([math:def-group-power](https://alphabetamath.cc/item/def-group-power)). For a group element $h$, $h^i h^j=h^{i+j}$ and $(h^i)^j=h^{ij}$ ([math:lem-group-power-laws](https://alphabetamath.cc/item/lem-group-power-laws)). In a finite group the order of an element is the least positive exponent at which its power is the identity ([math:def-order-in-a-group](https://alphabetamath.cc/item/def-order-in-a-group)). For an element of finite order, the subgroup it generates has cardinality equal to that order ([math:lem-order-characterisation](https://alphabetamath.cc/item/lem-order-characterisation), clause 3).

[F7] A map is bijective if it is injective and surjective. An injective map gives a bijection onto its image. A surjective map has its entire codomain as its image ([math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)).

[F8] The Cartesian product $A\times B$ consists of the ordered pairs $(a,b)$ with $a\in A$ and $b\in B$ ([math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)). For finite $A,B$ it is finite with cardinality $|A|\,|B|$ ([math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule), clause 1). A set in bijection with a finite set is finite with the same cardinality, and the initial segment of $n$ natural numbers has cardinality $n$ ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality), parts (c) and (a)).

[F9] A subset of a finite set is finite and has cardinality at most that of the whole set. If their cardinalities agree, the subset is the whole set ([math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set), clauses 1–3). Two disjoint finite sets have union of cardinality equal to the sum of their cardinalities ([math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule), clause 1).

[F10] The natural numbers embed in the integers with addition, multiplication, and order preserved, and their image is the nonnegative integers ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)). The integers form a totally ordered commutative ring in which order is compatible with addition and the product of two positive elements is positive ([math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)).

## Proof

**Given:** A finite field $F$ of order $q$ and a quadratic extension $E/F$.

**Goal:** Show $N_{E/F}(z)=\det(m_z)=z^{q+1}$ for $z\in E^\times$ and that every element of $F^\times$ occurs as a norm.

1.1 Choose an ordered basis $(v,w)$ of $E$ over $F$. The map $(a,b)\mapsto av+bw$ is a bijection from $F\times F$ to $E$ by unique coordinates. The product rule gives $|F\times F|=q^2$, so $E$ is finite with $|E|=q^2$. Each $K\in\{F,E\}$ is the disjoint union of its finite subsets $K^\times$ and $\{0\}$, the latter in bijection with the one-element initial segment. Thus $|F^\times|=q-1$ and $|E^\times|=q^2-1$. The two distinct field elements $0,1$ give $q\ge2$. [given, F1, F2, F7, F8, F9]

2.1 Since $E$ is finite and $[E:F]=2$, the relative automorphism group is generated by $\sigma$ and has two elements. The order of $\sigma$ is therefore two, so $\sigma\ne\mathrm{id}_E$ and $\sigma\circ\sigma=\mathrm{id}_E$. Choose $u\in E$ with $\sigma(u)\ne u$. Then $u\notin F$ since $\sigma$ fixes $F$. If $a+bu=a'+b'u$ with $a,b,a',b'\in F$ and $b\ne b'$, then $u=(a'-a)/(b-b')\in F$ by the inherited field operations, a contradiction. If $b=b'$, equality forces $a=a'$. Hence $(a,b)\mapsto a+bu$ bijects $F\times F$ with its image, a subset of $E$ with cardinality $q^2=|E|$. That image is all of $E$, so $(1,u)$ is an ordered basis by the unique-coordinate criterion. [F1, F2, F4, F6, F7, F8, F9, step 1.1]

3.1 Write $u^2=c+du$ with $c,d\in F$. Applying $\sigma$ gives $\sigma(u)^2=c+d\sigma(u)$, since $\sigma$ preserves addition and multiplication and fixes $c,d$. Subtracting gives $(u-\sigma(u))(u+\sigma(u)-d)=0$. The first factor is nonzero. If the second factor were also nonzero, their product would belong to the multiplicative group $E^\times$, contradicting the equality to zero. Thus $u+\sigma(u)=d$. Substitution into $u^2=c+du$ gives $u\sigma(u)=-c$. [F1, F4, F6, step 2.1]

4.1 For $z\in E^\times$, write $z=a+bu$ with $a,b\in F$. Multiplication by $z$ is $F$-linear since $z(rx+sy)=r(zx)+s(zy)$ for $r,s\in F$ and $x,y\in E$. With the common identity $1$, it sends $1$ to $a+bu$ and $u$ to $bc+(a+bd)u$. The coordinate matrix relative to $(1,u)$ has first-column entries $a,b$ and second-column entries $bc,a+bd$, listed from top to bottom. Its determinant is $a(a+bd)-b^2c=(a+bu)(a+b\sigma(u))=z\sigma(z)=z^{q+1}$. This is $N_{E/F}(z)$ and belongs to $F$ by the matrix computation. For $z\ne0$ the power is nonzero. [F1, F2, F3, F4, F5, F6, step 2.1, step 3.1]

5.1 Take a generator $g$ of the finite group $E^\times$. Its order is finite and equals $|\langle g\rangle|=|E^\times|=q^2-1$, so $g^{q^2-1}=1$. For each natural number $i<q-1$, $N_{E/F}(g^i)=g^{(q+1)i}$. [F6, step 1.1, step 4.1]

6.1 Suppose two such values coincide for $0\le i<j<q-1$. Use the natural-number embedding to calculate in the integers. Adding $-i$ to $i<j$ gives $0<j-i$. From $0\le i$ we get $-i\le0$ by adding $-i$, and then $j-i\le j$ by adding $j$. Thus $0<j-i\le j<q-1$. Multiplication by $q+1>0$ preserves the strict bounds because the product of $q+1$ and a positive difference is positive. Hence $0<k<(q+1)(q-1)=q^2-1$ for $k=(q+1)(j-i)$, so $k$ represents a positive natural number. The power law gives $g^{(q+1)i}g^k=g^{(q+1)j}$. Since $g^{(q+1)j}=g^{(q+1)i}$, left multiplication by $(g^{(q+1)i})^{-1}$ in $E^\times$ gives $g^k=1$. This contradicts the least-positive-exponent definition of the order of $g$, so the norm values are pairwise distinct. [F1, F6, F10, step 1.1, step 5.1]

7.1 The norm values from step 5.1 form a subset of $F^\times$ by step 4.1. The map from the initial segment of $q-1$ natural numbers to these values is bijective, so this subset has cardinality $q-1=|F^\times|$. It equals $F^\times$ by the finite subset criterion. This proves surjectivity and completes the determinant and power formula from step 4.1. [F7, F8, F9, step 1.1, step 4.1, step 5.1, step 6.1] ∎

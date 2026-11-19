---
title: Quaternion Orders and Finite Projective Groups
description: Set up Hamilton norms, Hurwitz orders and their odd-prime
  splitting, then develop the finite projective groups, quadratic normalizers,
  and character counts used in the obstruction estimate.
status: published
dependency_level: 0
---

**Purpose:** Set up Hamilton norms, Hurwitz orders and their odd-prime splitting, then develop the finite projective groups, quadratic normalizers, and character counts used in the obstruction estimate.

## Published prerequisite

[math:def-quaternions](https://alphabetamath.cc/item/def-quaternions)

## Published prerequisite

[math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes)

## Published prerequisite

[math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)

## Published prerequisite

[math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)

## Published prerequisite

[math:def-finite-field-and-its-order](https://alphabetamath.cc/item/def-finite-field-and-its-order)

## Published prerequisite

[math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group](https://alphabetamath.cc/item/thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group)

## Published prerequisite

[math:def-field-norm-and-trace](https://alphabetamath.cc/item/def-field-norm-and-trace)

## Norm and conjugation on rational Hamilton quaternions

[Open item](item-lem-rational-hamilton-norm-and-inverse) · level 0


### Statement

Let $\mathbb H=\mathbb R^4$ be the real Hamilton quaternions with their usual addition and multiplication. Let $B=\mathbb Q^4\subseteq\mathbb H$ be the quaternions with rational coordinates, using the constant-sequence embedding of $\mathbb Q$ into $\mathbb R$. Write $\iota(t)=(t,0,0,0)$ for a scalar quaternion with $t\in\mathbb Q$.

The inherited operations make $B$ a $\mathbb Q$-subalgebra of $\mathbb H$. Thus $B$ is a subring containing $1$ and all the rational scalar quaternions, which commute with every element of $\mathbb H$. Moreover, $B$ is a division algebra over $\mathbb Q$, meaning that $1\ne0$ and every nonzero element of $B$ has a two-sided multiplicative inverse in $B$.

For $x=(a,b,c,d)\in B$, its conjugate is $\bar x=(a,-b,-c,-d)$ and its reduced norm is the rational scalar $N(x)=a^2+b^2+c^2+d^2$, characterized by $x\bar x=\bar x x=\iota(N(x))$. Conjugation on $B$ is an anti-involution. It preserves addition and $1$, applying it twice gives the identity, and $\overline{xy}=\bar y\bar x$.

For all $x,y\in B$, $N(xy)=N(x)N(y)$. For $x\ne0$, $N(x)\ne0$ and $x^{-1}=\bar x/N(x)$, where division by $N(x)$ means multiplication by $\iota(1/N(x))$.

### Facts & Assumptions

[F1] The rational numbers are the classes $a/b$ of integer pairs with $b\ne0$ under equality of cross-products ([math:def-rationals](https://alphabetamath.cc/item/def-rationals)). Their addition, multiplication, negation and reciprocals are those of [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations). They form a field, so sums, products and negatives are rational, and every nonzero rational has a rational reciprocal ([math:thm-rat-field](https://alphabetamath.cc/item/thm-rat-field)). The map taking a rational to the class of its constant sequence in the reals is an injective map preserving $0,1,+,\cdot$ ([math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers), [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)).

[F2] In $\mathbb H$, addition and negation are coordinatewise, and each product coordinate is a sum or difference of products of input coordinates. The elements $0$ and $1$ are $(0,0,0,0)$ and $(1,0,0,0)$. Conjugation negates exactly the last three coordinates, and the real Hamilton norm $N_{\mathbb H}(x)$ is the sum of the four coordinate squares ([math:def-quaternions](https://alphabetamath.cc/item/def-quaternions)).

[F3] The real quaternion operations make $\mathbb H$ a ring with $1\ne0$. For $x\in\mathbb H$, $x\bar x=\bar x x=(N_{\mathbb H}(x),0,0,0)$, and $N_{\mathbb H}(x)>0$ if $x\ne0$ ([math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring)).

[F4] Real quaternion conjugation satisfies $\overline{\bar x}=x$ and $\overline{xy}=\bar y\bar x$ for all $x,y\in\mathbb H$ ([math:lem-quaternion-conjugation-is-an-anti-involution](https://alphabetamath.cc/item/lem-quaternion-conjugation-is-an-anti-involution)).

[F5] A ring is an abelian group under addition with an associative unital multiplication satisfying both distributive laws ([math:def-ring](https://alphabetamath.cc/item/def-ring)). A unital ring map preserves addition, multiplication and $1$ ([math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)). A $\mathbb Q$-algebra is a unital ring with such a map from $\mathbb Q$ whose images commute with all ring elements ([math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)). Its underlying ring is a division ring if $1\ne0$ and every nonzero element has a two-sided multiplicative inverse ([math:def-division-ring](https://alphabetamath.cc/item/def-division-ring)).

[F6] A subset of a ring is a unital subring if it contains the ambient identity and is closed under addition, additive inverses and multiplication. It inherits the ring operations and identities ([math:def-subring](https://alphabetamath.cc/item/def-subring)).

### Proof

**Given:** The real Hamilton quaternions $\mathbb H$, their rational-coordinate subset $B$ and arbitrary $x,y\in B$.

**Goal:** Show that $B$ is a division subalgebra over $\mathbb Q$ with the stated conjugation, reduced norm and inverse formulas.

1.1 The coordinate rules for addition, negation and multiplication keep their results in $\mathbb Q$ by [F1] and [F2]. The coordinates of both $0$ and $1$ are rational. The real quaternions form a ring by [F3]. By [F6], $B$ is a unital subring with the inherited ring operations and identities. [F1, F2, F3, F6]

2.1 For $t\in\mathbb Q$ and $z=(z_0,z_1,z_2,z_3)\in\mathbb H$, substitution into the quaternion product gives $\iota(t)z=z\iota(t)=(tz_0,tz_1,tz_2,tz_3)$. For rational $s,t$, this gives $\iota(s)\iota(t)=\iota(st)$, while coordinate addition gives $\iota(s)+\iota(t)=\iota(s+t)$ and $\iota(1)=1$. The map $\iota$ is injective by the first coordinate and [F1]. Its image lies in $B$ and commutes with every element of $\mathbb H$. Thus $B$ is a $\mathbb Q$-subalgebra with the inherited scalar map. [F1, F2, F5, step 1.1]

2.2 The coordinate formula for conjugation preserves rational coordinates, fixes $1$, and preserves addition because each coordinate is either unchanged or negated. The two identities in [F4] therefore restrict to $B$, proving that its conjugation is an anti-involution. [F1, F2, F4, step 1.1]

3.1 The sum of the four squares of the coordinates of $x$ is rational by [F1], so $N_{\mathbb H}(x)$ is the image of the scalar $N(x)\in\mathbb Q$. The product identity in [F3] yields $x\bar x=\bar x x=\iota(N(x))$. Injectivity of $\iota$ makes this scalar unique. If $x\ne0$, positivity of $N_{\mathbb H}(x)$ gives $N(x)\ne0$. [F1, F2, F3, step 2.1, step 2.2]

4.1 Since $xy\in B$, apply the norm identity to $xy$ and reverse the order under conjugation. Associativity and commutation with rational scalars give $\iota(N(xy))=(xy)\overline{xy}=x(y\bar y)\bar x=(x\bar x)\iota(N(y))=\iota(N(x)N(y))$. Injectivity gives $N(xy)=N(x)N(y)$. [F3, step 1.1, step 2.1, step 2.2, step 3.1]

5.1 If $x\ne0$, then $r=1/N(x)$ is rational by [F1] and step 3.1. Put $u=\iota(r)\bar x\in B$. Using commutation with rational scalars and both orders of the norm identity, $xu=\iota(r)(x\bar x)=\iota(1)=1$ and $ux=\iota(r)(\bar x x)=\iota(1)=1$. This gives the stated inverse in $B$. Since $1\ne0$ in $B$, its ring is a division ring. Thus $B$ is a division algebra with the stated conjugation, reduced norm and inverse. [F1, F3, F5, step 1.1, step 2.1, step 2.2, step 3.1, step 4.1] ∎


## Degree-two projective linear groups

[Open item](item-def-degree-two-projective-linear-group) · level 0


### Definition

A ring is a set with addition and multiplication. Addition makes it an abelian group, meaning a group with commutative operation, with identity $0$. Multiplication is associative, has identity $1$, and distributes over addition on both sides. In a commutative ring, multiplication is commutative. Write $R^\times$ for the units of a ring $R$, the elements $u\in R$ admitting $v\in R$ with $uv=vu=1$.

Let $R$ be a field or a local ring. In a field, $1\ne 0$ and every nonzero element is a unit of the commutative ring. A local ring is a commutative ring with $1\ne 0$ and exactly one maximal ideal. An ideal is a subset containing $0$ and closed under differences and multiplication by arbitrary ring elements. A maximal ideal is an ideal different from the whole ring and contained in no larger ideal different from the whole ring.

Let $M_2(R)$ be the set of two-by-two arrays of entries in $R$. The matrix product is $(AB)_{ik}=a_{i1}b_{1k}+a_{i2}b_{2k}$, and $I_R$ has $1$ on the diagonal and $0$ elsewhere. The **general linear group** $\mathrm{GL}_2(R)$ consists of those $A\in M_2(R)$ with $AB=BA=I_R$ for some $B\in M_2(R)$, under matrix multiplication.

The **degree-two projective linear group** is the quotient group
$$\mathrm{PGL}_2(R)=\mathrm{GL}_2(R)/(R^\times I_R).$$
Here $R^\times I_R=\{uI_R:u\in R^\times\}$ is the scalar subgroup, with each $uI_R$ having $u$ on the diagonal and $0$ elsewhere. Its elements commute with all matrices in $\mathrm{GL}_2(R)$, so it is central. The element represented by $A$ is its left coset $[A]=\{uA:u\in R^\times\}$, where $uA$ means multiplying each entry by $u$. The quotient product is $[A][B]=[AB]$.

Let $S$ also be a field or a local ring. A unital ring homomorphism $f:R\to S$ preserves addition, multiplication, and the multiplicative identity. Write $f_2(A)$ for the matrix obtained by applying $f$ to each entry. The induced group homomorphism, meaning a map preserving the group product, is $\mathrm{PGL}_2(f):[A]\mapsto[f_2(A)]$. For an ideal $J$ with $S=R/J$ a field or local ring, the quotient ring has elements $r+J=\{r+j:j\in J\}$ with sum and product represented by the sum and product of representatives. Using $f(r)=r+J$ gives **projective reduction modulo $J$**.

### Facts & Assumptions

[F1] Each field is a commutative ring with its original operations and identities, and each local ring is commutative by definition ([field as a commutative ring](https://alphabetamath.cc/item/lem-field-is-a-commutative-ring), [local ring](https://alphabetamath.cc/item/def-local-ring), [commutative ring](https://alphabetamath.cc/item/def-commutative-ring)). Rings have an associative multiplication with identity, and zero annihilates multiplication on both sides ([ring](https://alphabetamath.cc/item/def-ring), [zero multiplication in a ring](https://alphabetamath.cc/item/lem-ring-elementary-consequences)).

[F2] Square matrices over a commutative ring multiply by the entry formulas above, and their multiplication is associative with identity $I_R$. Invertible matrices have unique two-sided inverses ([matrix product and identity](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose), [matrix arithmetic laws](https://alphabetamath.cc/item/thm-ring-matrix-arithmetic-laws), [matrix invertibility](https://alphabetamath.cc/item/def-invertible-matrix-and-similarity-over-a-commutative-ring)).

[F3] A group has an associative operation with a two-sided identity and a two-sided inverse for every element. The units of a ring form such a group under multiplication ([group](https://alphabetamath.cc/item/def-group), [ring units](https://alphabetamath.cc/item/lem-ring-units-form-a-group)).

[F4] The center $Z(G)$ consists of the elements of $G$ that commute with every element of $G$ ([center of a group](https://alphabetamath.cc/item/def-center-of-a-group)). A subgroup contains the identity and is closed under products and inverses. It is normal if $gNg^{-1}=N$ for every $g$ in the group. For a normal subgroup $N$ of a group $G$, the left cosets $gN=\{gn:n\in N\}$ form a group with product $(gN)(hN)=(gh)N$ ([subgroup](https://alphabetamath.cc/item/def-subgroup), [normal subgroup](https://alphabetamath.cc/item/def-normal-subgroup), [left coset](https://alphabetamath.cc/item/def-coset), [quotient group](https://alphabetamath.cc/item/def-quotient-group), [quotient group laws](https://alphabetamath.cc/item/thm-quotient-group-laws)). For elements $a,b$ of a group and a subgroup $N$, the left cosets $aN$ and $bN$ agree exactly when $a^{-1}b\in N$ ([coset equality](https://alphabetamath.cc/item/lem-coset-membership-and-equality)).

[F5] A unital ring homomorphism sends $0$ to $0$ and units to units, in addition to preserving the operations and $1$. A map between groups is a group homomorphism if it preserves multiplication ([ring homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism), [images of zero and units](https://alphabetamath.cc/item/lem-ring-homomorphism-basic-properties), [group homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)).

[F6] An ideal $J$ of a commutative ring $R$ is two-sided. The additive cosets modulo $J$ form a ring with identity $1+J$. The sum and product are well defined and computed by adding and multiplying representatives ([ideal](https://alphabetamath.cc/item/def-left-right-and-two-sided-ideal), [quotient ring](https://alphabetamath.cc/item/def-quotient-ring), [quotient-ring laws](https://alphabetamath.cc/item/thm-quotient-ring-laws)).

### Justification

**Given:** Rings $R,S$, each a field or a local ring, and a unital ring homomorphism $f:R\to S$.

**Goal:** Justify the matrix group, its scalar quotient, and the induced map, including the quotient-ring reduction.

1.1 Work over either ring, using $R$ to write the formulas. The identity matrix is invertible with inverse itself. If $A,B$ have inverses $A^{-1},B^{-1}$, then $(AB)(B^{-1}A^{-1})=I_R=(B^{-1}A^{-1})(AB)$ by associativity and the inverse equations. Also $A$ is a two-sided inverse to $A^{-1}$. Thus multiplication, the identity and inverses restrict to the invertible matrices, making $\mathrm{GL}_2(R)$ a group. [F1, F2, F3]

2.1 For a unit $u$, the inverse of $uI_R$ is $u^{-1}I_R$, and $(uI_R)(vI_R)=(uv)I_R$ for units $u,v$. This follows from entrywise matrix multiplication and zero annihilation. Together with $I_R=1I_R$, these identities make $R^\times I_R$ a subgroup. For $A=(a_{ik})\in\mathrm{GL}_2(R)$, the entries of $(uI_R)A$ and $A(uI_R)$ are $ua_{ik}$ and $a_{ik}u$ respectively, equal by commutativity. Thus $R^\times I_R$ is contained in $Z(\mathrm{GL}_2(R))$ and is a central subgroup. Hence $A(uI_R)A^{-1}=uI_R$ for every unit $u$, so $ANA^{-1}=N$ for $N=R^\times I_R$. The quotient group law applies, and the same entry formula gives $AN=\{uA:u\in R^\times\}$. [F1, F2, F3, F4, step 1.1]

2.2 The entry formula and preservation of addition and multiplication give $f_2(AB)=f_2(A)f_2(B)$. Since $f$ preserves $0$ and $1$, $f_2(I_R)=I_S$. Applying these identities to both products of $A$ with $A^{-1}$ shows that $f_2(A^{-1})$ is a two-sided inverse to $f_2(A)$. In particular the latter lies in $\mathrm{GL}_2(S)$. [F2, F5, step 1.1]

3.1 If $A'$ represents $[A]$, then $A'=uA$ for a unit $u\in R^\times$. Applying $f$ to the entries gives $f_2(A')=f(u)f_2(A)$ with $f(u)\in S^\times$. Since the scalar matrix $f(u)I_S$ commutes with $f_2(A)$, we have $f_2(A)^{-1}f_2(A')=f(u)I_S\in S^\times I_S$. The left-coset equality criterion gives $[f_2(A')]=[f_2(A)]$. The induced map sends $[AB]$ to $[f_2(A)f_2(B)]=[f_2(A)][f_2(B)]$, hence is a group homomorphism. [F4, F5, step 2.1, step 2.2]

4.1 Suppose $S=R/J$ is a field or local ring as in the definition. Since $R$ is commutative, $J$ is two-sided, so $R/J$ has well-defined coset operations and identity $1+J$. The map $\pi(r)=r+J$ preserves addition and multiplication by the coset formulas, and $\pi(1)=1+J$. Thus $\pi$ is a unital ring homomorphism and its induced map is projective reduction. This establishes all the constructions in the definition. [F1, F5, F6, step 3.1] ∎


## Norm surjectivity for a quadratic finite field

[Open item](item-lem-quadratic-finite-field-norm-surjectivity) · level 0


### Statement

Let $F$ be a finite field of order $q=|F|$ and let $E/F$ be a quadratic extension, meaning $F$ is a subfield of $E$ and $[E:F]=\dim_F E=2$. For a field $K$, write $K^\times=K\setminus\{0\}$ with field multiplication. For every $z\in E^\times$, the field norm satisfies $N_{E/F}(z)=\det(m_z)=z^{q+1}$, where $m_z$ is the $F$-linear map $x\mapsto zx$ on $E$. The norm maps onto $F^\times$, meaning every element of $F^\times$ is the norm of some element of $E^\times$.

### Facts & Assumptions

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

### Proof

**Given:** A finite field $F$ of order $q$ and a quadratic extension $E/F$.

**Goal:** Show $N_{E/F}(z)=\det(m_z)=z^{q+1}$ for $z\in E^\times$ and that every element of $F^\times$ occurs as a norm.

1.1 Choose an ordered basis $(v,w)$ of $E$ over $F$. The map $(a,b)\mapsto av+bw$ is a bijection from $F\times F$ to $E$ by unique coordinates. The product rule gives $|F\times F|=q^2$, so $E$ is finite with $|E|=q^2$. Each $K\in\{F,E\}$ is the disjoint union of its finite subsets $K^\times$ and $\{0\}$, the latter in bijection with the one-element initial segment. Thus $|F^\times|=q-1$ and $|E^\times|=q^2-1$. The two distinct field elements $0,1$ give $q\ge2$. [given, F1, F2, F7, F8, F9]

2.1 Since $E$ is finite and $[E:F]=2$, the relative automorphism group is generated by $\sigma$ and has two elements. The order of $\sigma$ is therefore two, so $\sigma\ne\mathrm{id}_E$ and $\sigma\circ\sigma=\mathrm{id}_E$. Choose $u\in E$ with $\sigma(u)\ne u$. Then $u\notin F$ since $\sigma$ fixes $F$. If $a+bu=a'+b'u$ with $a,b,a',b'\in F$ and $b\ne b'$, then $u=(a'-a)/(b-b')\in F$ by the inherited field operations, a contradiction. If $b=b'$, equality forces $a=a'$. Hence $(a,b)\mapsto a+bu$ bijects $F\times F$ with its image, a subset of $E$ with cardinality $q^2=|E|$. That image is all of $E$, so $(1,u)$ is an ordered basis by the unique-coordinate criterion. [F1, F2, F4, F6, F7, F8, F9, step 1.1]

3.1 Write $u^2=c+du$ with $c,d\in F$. Applying $\sigma$ gives $\sigma(u)^2=c+d\sigma(u)$, since $\sigma$ preserves addition and multiplication and fixes $c,d$. Subtracting gives $(u-\sigma(u))(u+\sigma(u)-d)=0$. The first factor is nonzero. If the second factor were also nonzero, their product would belong to the multiplicative group $E^\times$, contradicting the equality to zero. Thus $u+\sigma(u)=d$. Substitution into $u^2=c+du$ gives $u\sigma(u)=-c$. [F1, F4, F6, step 2.1]

4.1 For $z\in E^\times$, write $z=a+bu$ with $a,b\in F$. Multiplication by $z$ is $F$-linear since $z(rx+sy)=r(zx)+s(zy)$ for $r,s\in F$ and $x,y\in E$. With the common identity $1$, it sends $1$ to $a+bu$ and $u$ to $bc+(a+bd)u$. The coordinate matrix relative to $(1,u)$ has first-column entries $a,b$ and second-column entries $bc,a+bd$, listed from top to bottom. Its determinant is $a(a+bd)-b^2c=(a+bu)(a+b\sigma(u))=z\sigma(z)=z^{q+1}$. This is $N_{E/F}(z)$ and belongs to $F$ by the matrix computation. For $z\ne0$ the power is nonzero. [F1, F2, F3, F4, F5, F6, step 2.1, step 3.1]

5.1 Take a generator $g$ of the finite group $E^\times$. Its order is finite and equals $|\langle g\rangle|=|E^\times|=q^2-1$, so $g^{q^2-1}=1$. For each natural number $i<q-1$, $N_{E/F}(g^i)=g^{(q+1)i}$. [F6, step 1.1, step 4.1]

6.1 Suppose two such values coincide for $0\le i<j<q-1$. Use the natural-number embedding to calculate in the integers. Adding $-i$ to $i<j$ gives $0<j-i$. From $0\le i$ we get $-i\le0$ by adding $-i$, and then $j-i\le j$ by adding $j$. Thus $0<j-i\le j<q-1$. Multiplication by $q+1>0$ preserves the strict bounds because the product of $q+1$ and a positive difference is positive. Hence $0<k<(q+1)(q-1)=q^2-1$ for $k=(q+1)(j-i)$, so $k$ represents a positive natural number. The power law gives $g^{(q+1)i}g^k=g^{(q+1)j}$. Since $g^{(q+1)j}=g^{(q+1)i}$, left multiplication by $(g^{(q+1)i})^{-1}$ in $E^\times$ gives $g^k=1$. This contradicts the least-positive-exponent definition of the order of $g$, so the norm values are pairwise distinct. [F1, F6, F10, step 1.1, step 5.1]

7.1 The norm values from step 5.1 form a subset of $F^\times$ by step 4.1. The map from the initial segment of $q-1$ natural numbers to these values is bijective, so this subset has cardinality $q-1=|F^\times|$. It equals $F^\times$ by the finite subset criterion. This proves surjectivity and completes the determinant and power formula from step 4.1. [F7, F8, F9, step 1.1, step 4.1, step 5.1, step 6.1] ∎


## Balance of a character on a finite coset orbit

[Open item](item-lem-coset-character-balance) · level 0


### Statement

Let $G$ be a finite group with identity $e$ and let $H,K\le G$ be subgroups. Let $\chi:G\to\{+1,-1\}$ be a character, meaning a homomorphism into the two signs under multiplication. Assume that $\chi(h)=+1$ for every $h\in H$ and that $\chi$ takes both signs on $K$.

Write $Hg=\{hg:h\in H\}$ for the right coset represented by $g$, and $H\backslash G=\{Hg:g\in G\}$ for the set of right cosets. The right $K$-orbit of $H=He$ is the set $\mathcal O=\{Hk:k\in K\}$ of cosets reached from $H$ by right multiplication by elements of $K$. The sign of $Hg$ is $\chi(g)$, independent of the representative. For either $S=\mathcal O$ or $S=H\backslash G$, let $S_+$ and $S_-$ consist of the cosets in $S$ with signs $+1$ and $-1$, respectively. Then $S_+$ and $S_-$ are finite and $|S_+|=|S_-|$.

### Facts & Assumptions

[F1] A group has an associative multiplication, a two-sided identity $e$, and a two-sided inverse $u^{-1}$ for each element $u$ ([math:def-group](https://alphabetamath.cc/item/def-group)).

[F2] A subgroup contains the group identity and is closed under multiplication and taking inverses ([math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)).

[F3] The right coset represented by $g$ is the subset $Hg=\{hg:h\in H\}$ of $G$ ([math:def-coset](https://alphabetamath.cc/item/def-coset)).

[F4] The group of units of the integers under multiplication is $\{+1,-1\}$, with identity $+1$ and each sign its own inverse ([math:lem-units-of-z](https://alphabetamath.cc/item/lem-units-of-z)). A group homomorphism preserves multiplication, so $\chi(uv)=\chi(u)\chi(v)$ for $u,v\in G$ ([math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)).

[F5] A map is injective if equal outputs imply equal inputs, surjective if each target value occurs, and bijective if both hold ([math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)).

[F6] A set is finite when it admits a bijection with $\{0,\ldots,n-1\}$ for some natural number $n$. Its cardinality is that unique $n$, and a bijection between finite sets gives equal cardinalities ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality), clause (d)).

[F7] The power set $\mathcal P(G)$ is the set of all subsets of $G$ ([math:def-power-set](https://alphabetamath.cc/item/def-power-set)).

[F8] A function from a set to a specified codomain assigns each input exactly one output in that codomain ([math:def-function](https://alphabetamath.cc/item/def-function)).

[F9] A set is a subset of another set if every element of the first set belongs to the second ([math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)).

[L1] The power set of a finite set is finite ([math:cor-cardinality-of-the-power-set](https://alphabetamath.cc/item/cor-cardinality-of-the-power-set)).

[L2] Every subset of a finite set is finite ([math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)).

### Proof

**Given:** The finite group $G$, its subgroups $H,K$, and the character $\chi$ taking only $+1$ on $H$ and both signs on $K$.

**Goal:** Show that the coset sign is well-defined and that $|S_+|=|S_-|$ for both choices of $S$.

1.1 If $Hg'=Hg$, then $g'=eg'\in Hg'$ because $e\in H$. Thus $g'\in Hg$, so $g'=hg$ for some $h\in H$. It follows that $\chi(g')=\chi(h)\chi(g)=\chi(g)$. Every coset has a representative $g$, and the preceding equality makes the value $\bar\chi(Hg)=\chi(g)$ unique in $\{+1,-1\}$. This defines the coset sign function. [F1, F2, F3, F4, F8, given]

1.2 For $u\in G$, right multiplication gives a map $R_u(Hg)=H(gu)$ on $H\backslash G$. Since $gu\in G$, the output $H(gu)$ is in $H\backslash G$. Indeed, $H(gu)=\{xu:x\in Hg\}$ by associativity, so the output depends only on the coset. One has $R_e(C)=C$ and $R_v(R_u(C))=R_{uv}(C)$ for every coset $C$ and all $u,v\in G$. These are the right action identities. Also $He=H$, and $R_k(H)=Hk$ for $k\in K$, so this action gives exactly the stated orbit. If $k,u\in K$, then $ku\in K$, so $R_u$ sends $\mathcal O$ to itself whenever $u\in K$. [F1, F2, F3, F8]

2.1 Choose $t\in K$ with $\chi(t)=-1$. Since $t^{-1}\in K$, both $R_t$ and $R_{t^{-1}}$ act on each set $S$, and their two compositions are the identity by the right action identities. For $C=Hg$ one has $\bar\chi(R_t(C))=\chi(gt)=\bar\chi(C)\chi(t)$. The products $(+1)(-1)=-1$ and $(-1)(-1)=+1$ show that $R_t$ reverses the sign. [F1, F2, F4, given, step 1.1, step 1.2]

3.1 For each $C\in S_+$, step 1.2 gives a unique value $R_t(C)$ and step 2.1 places it in $S_-$. Hence $f(C)=R_t(C)$ defines a function $f:S_+\to S_-$. If $f(C)=f(C')$, applying $R_{t^{-1}}$ yields $C=C'$, so $f$ is injective. Given $D\in S_-$, set $C=R_{t^{-1}}(D)$. Then $C\in S$ and $R_t(C)=D$. Since $R_t$ reverses signs, $C\in S_+$ and $f(C)=D$. Thus $f$ is surjective and hence bijective. [F5, F8, step 1.2, step 2.1]

4.1 Every member of $S_+$ or $S_-$ is a coset and hence a subset of $G$, so each such member lies in the power set $\mathcal P(G)$. Therefore $S_+$ and $S_-$ are both subsets of $\mathcal P(G)$. Since $G$ is finite, the power set is finite, and both sign classes are finite. The bijection gives $|S_+|=|S_-|$ for both the orbit and the full coset set. [F3, F6, F7, F9, L1, L2, given, step 3.1] ∎


## Orders in rational algebras

[Open item](item-def-author-53081a7cb32d-order-in-a-rational-algebra) · level 0


### Definition

Write $\mathbb Q$ for the rationals, whose elements are fractions of integers with nonzero denominator. Use the usual rational addition and multiplication, which make $\mathbb Q$ a commutative ring with identity $1_{\mathbb Q}=1/1$. An integer $n\in\mathbb Z$ is read as a rational scalar by the embedding $n\mapsto n/1$.

Let $A$ be a rational algebra, meaning a ring with identity and a specified map $\eta:\mathbb Q\to A$ that preserves addition, multiplication and identity and whose values commute with every element of $A$. For $q\in\mathbb Q$ and $a\in A$, let $q\cdot a=\eta(q)a$. Finite sums in $A$ use its commutative additive monoid, with empty sum $0_A$.

A **$\mathbb Z$-order in $A$** is a subring $S\subseteq A$, meaning it contains $1_A$ and is closed under addition, additive inverses and multiplication, with the following two properties.

- There is a fixed finite list $s_1,\ldots,s_r$ of elements of $S$ such that $S=\{\sum_{j=1}^r (n_j/1)\cdot s_j : n_1,\ldots,n_r\in\mathbb Z\}$.
- For every $a\in A$ there are a finite list $t_1,\ldots,t_m$ of elements of $S$ and rational coefficients $q_1,\ldots,q_m\in\mathbb Q$ such that $a=\sum_{j=1}^m q_j\cdot t_j$.

An order $S$ is **maximal** if every order $T$ in $A$ with $S\subseteq T$ satisfies $T=S$.

### Definition references

[The integers](https://alphabetamath.cc/item/def-integers)

[Rational numbers](https://alphabetamath.cc/item/def-rationals)

[Rational arithmetic](https://alphabetamath.cc/item/def-rat-operations)

[The rational field](https://alphabetamath.cc/item/thm-rat-field)

[The embedding of integers into rationals](https://alphabetamath.cc/item/lem-int-embeds-rat)

[Rings with identity](https://alphabetamath.cc/item/def-ring)

[Algebras over a commutative ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)

[Finite sums in a commutative monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)

[Subrings](https://alphabetamath.cc/item/def-subring)

### Justification

The subring conditions give $S$ the ring operations and identity inherited from $A$. Write $f(n)=\eta(n/1)$. The integer embedding and the scalar map are additive, and the rational identity $1_{\mathbb Q}=1/1$ gives $f(1)=1_A$. In the additive group of $\mathbb Z$, step 1.2 of [the cyclic-subgroup lemma](https://alphabetamath.cc/item/lem-subgroups-of-z-are-cyclic) with $g=1$ identifies the additive $n$-th power of $1$ with the integer product $1\cdot n$. The multiplicative identity law [for the integers](https://alphabetamath.cc/item/thm-int-comm-ring) gives $1\cdot n=n$. The additive group homomorphism $f$ preserves these powers [by the power law for group homomorphisms](https://alphabetamath.cc/item/lem-group-homomorphism-basic-properties), so $f(n)$ is the additive $n$-th power of $1_A$. For positive $n$ this power is the sum of $n$ copies of $1_A$, for $n=0$ it is $0_A$, and for negative $n$ it is the additive inverse of the corresponding positive sum.

The distributivity consequence $(n\,1_A)s=ns$ for signed additive multiples [in a ring](https://alphabetamath.cc/item/lem-integer-multiples-in-a-ring) gives $(n/1)\cdot s=f(n)s=ns$. Closure under addition and additive inverses, together with $0_A\in S$, keeps all the sums in the first condition in $S$. The second condition uses sums in $A$, where all the rational scalar products are defined. Maximality compares the resulting orders by inclusion.


## The normalized valuation on the local field

[Open item](item-def-author-24fda87362bc-local-adic-valuation) · level 0


### Definition

Let $\ell$ be a prime, a positive integer greater than $1$ with no positive divisors other than $1$ and itself. The field $\mathbb Q_\ell$ of $\ell$-adic numbers is the completion of $\mathbb Q$ for the distance $|r-s|_\ell$. Its elements are represented by rational Cauchy sequences, whose terms beyond a sufficiently large index have pairwise distances below any prescribed positive bound. Two such sequences represent the same element if their termwise distances tend to zero.

For a nonzero integer $a$, its exponent $v_\ell(a)$ is the greatest integer $k\ge0$ for which $\ell^k$ divides $a$. For a nonzero rational $r=a/b$ with nonzero integers $a,b$, set $v_\ell(r)=v_\ell(a)-v_\ell(b)$ and $|r|_\ell=\ell^{-v_\ell(r)}$. Set $|0|_\ell=0$. The powers in these absolute value formulas are integer powers of the positive real number $\ell$. On $\mathbb Q_\ell$, $|\cdot|_\ell$ denotes the extension of the rational absolute value, given by $\lim_{j\to\infty}|r_j|_\ell$ on the class of a rational Cauchy sequence $(r_j)$.

The ring $\mathbb Z_\ell$ of $\ell$-adic integers consists of compatible tuples of classes in $\mathbb Z/\ell^n\mathbb Z$ for $n\ge1$. Write $[a]_n$ for the class of $a$ modulo $\ell^n$. The transition maps send $[a]_{n+1}$ to $[a]_n$, and the ring operations are coordinatewise, using $[a]_n+[b]_n=[a+b]_n$ and $[a]_n[b]_n=[ab]_n$. The canonical embedding of this ring into the metric completion $\mathbb Q_\ell$ identifies it with the closed unit ball $\{x\in\mathbb Q_\ell:|x|_\ell\le1\}$.

The normalized valuation on $\mathbb Q_\ell$ is $v_\ell(x)=m$ when $x\ne0$ and $|x|_\ell=\ell^{-m}$ for $m\in\mathbb Z$, and $v_\ell(0)=+\infty$. Here $+\infty$ exceeds every integer and adding it to any value, including itself, gives $+\infty$. The value group is $\mathbb Z$ under addition with the usual order.

### Justification

The prime condition uses [math:def-prime](https://alphabetamath.cc/item/def-prime). The greatest exponent exists by [math:def-p-adic-valuation](https://alphabetamath.cc/item/def-p-adic-valuation). The rational valuation is independent of the fraction by [math:lem-p-adic-valuation-on-q](https://alphabetamath.cc/item/lem-p-adic-valuation-on-q), and [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals) defines the absolute value from it. The field construction in [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers) embeds the rationals isometrically and densely. The extension in [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field) is multiplicative and satisfies $|x+y|_\ell\le\max(|x|_\ell,|y|_\ell)$. For $x\ne0$ take a rational $r$ with $|x-r|_\ell<|x|_\ell$. Applying the inequality to $r=x+(r-x)$ gives $|r|_\ell\le |x|_\ell$. Applying it to $x=r+(x-r)$ then gives $|x|_\ell\le |r|_\ell$ because $|x-r|_\ell<|x|_\ell$. Thus $|r|_\ell=|x|_\ell>0$, so the exponent exists.

The ordered ring of [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) supplies the multiplicative monoid $(\mathbb Z,\cdot,1)$. Powers $\ell^k$ in divisibility and in the residue moduli are its natural powers from [math:def-group-power](https://alphabetamath.cc/item/def-group-power). By [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int), the nonnegative integer exponents are identified with the natural numbers. These powers are positive by the [induction principle](https://alphabetamath.cc/item/thm-induction-principle). The base case is $\ell^0=1>0$, and the ordered-ring multiplication law gives $\ell^{k+1}=\ell^k\ell>0$ if $\ell^k>0$. Thus each modulus $\ell^n$ corresponds to a natural number under the same identification.

Use the ordered field $\mathbb R$ from [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field). The ordered embeddings from [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) and [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) carry the integer inequality $\ell>1$ to the same inequality in $\mathbb R$. Take integer powers in $\mathbb R$ as in [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power). If $m<n$ in $\mathbb Z$, then $n-m>0$ by the ordered-ring law for addition, so [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) identifies $n-m$ with a positive natural exponent. By [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone), $\ell^{n-m}>1$ since $\ell>1$. If $n\le0$, then $\ell^{-n}>0$ by the positivity of natural powers from [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone). If $n>0$, that same positivity gives $\ell^{n}>0$, so $\ell^{-n}=(\ell^n)^{-1}>0$ by [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive). The exponent addition law of [math:lem-power-laws](https://alphabetamath.cc/item/lem-power-laws) gives $\ell^{-m}=\ell^{-n}\ell^{n-m}$. Since $\ell^{n-m}>1$ and $\ell^{-n}>0$, multiplication by $\ell^{-n}$ preserves strict inequality by [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules), so $\ell^{-m}>\ell^{-n}$. Thus $m\mapsto\ell^{-m}$ is strictly decreasing and the exponent is unique. Isometry and uniqueness also show that the local valuation agrees with the rational formula on nonzero rationals.

The integers form a totally ordered commutative ring by [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring), so their additive group is abelian and its total order is translation invariant. This supplies the ordered value group required by [math:def-valuation-on-a-field](https://alphabetamath.cc/item/def-valuation-on-a-field). By definition $v_\ell(x)=+\infty$ exactly when $x=0$. For nonzero $x$ and $y$, multiplicativity of the extended absolute value gives $|xy|_\ell=\ell^{-v_\ell(x)}\ell^{-v_\ell(y)}=\ell^{-(v_\ell(x)+v_\ell(y))}$ by [math:lem-power-laws](https://alphabetamath.cc/item/lem-power-laws). Uniqueness of the exponent gives $v_\ell(xy)=v_\ell(x)+v_\ell(y)$. If a factor is zero, the product law holds by the rule for $+\infty$. For nonzero $x$, $y$ and $x+y$, the strong triangle inequality gives
$$\ell^{-v_\ell(x+y)}\le\max(\ell^{-v_\ell(x)},\ell^{-v_\ell(y)})=\ell^{-\min(v_\ell(x),v_\ell(y))}.$$
Strict decrease gives $v_\ell(x+y)\ge\min(v_\ell(x),v_\ell(y))$. If $x+y=0$, the left side of the valuation inequality is $+\infty$. If one summand is zero and the sum is nonzero, the nonzero summand gives both sides. Finally, $|\ell|_\ell=\ell^{-1}$ on the rational copy, so $v_\ell(\ell)=1$.

The coordinate classes are the classes of [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n). Their two operations are independent of representatives by [math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n). By [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer), $a\equiv b\pmod{M}$ means $M\mid(a-b)$ for every integer modulus $M$. By [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z), this is equivalent to $a-b=Mq$ for some $q\in\mathbb Z$. If $a\equiv b\pmod{\ell^{n+1}}$, then $a-b=\ell^{n+1}q=\ell^n(\ell q)$ for some $q\in\mathbb Z$, and hence $a\equiv b\pmod{\ell^n}$. Thus the reduction maps are well defined. The formulas on representatives show that reduction preserves both operations and the classes of $0$ and $1$. It also preserves additive inverses, because the inverse of $[a]_n$ is $[-a]_n$. The coordinate ring laws from [math:thm-integers-modulo-n-basic-algebra](https://alphabetamath.cc/item/thm-integers-modulo-n-basic-algebra) therefore hold on the compatible tuples of [math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes).

The source ring in [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp) is this same inverse limit with transition maps given by reduction modulo the lower power. Step 1.2 of the comparison theorem sends a compatible tuple to the Cauchy class $\xi=[(b_n)]$ of its standard integer lifts, where $b_n$ is the representative of the $n$th coordinate in $[0,\ell^n)$. For fixed $n$, the quotient metric $d$ in Step 1.1 of [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field) gives $d(b_n,\xi)=\lim_{j\to\infty}|b_n-b_j|_\ell$, with $b_n$ on the left embedded as a constant sequence. Given $\varepsilon>0$, the Cauchy condition gives an $N$ such that $|b_n-b_j|_\ell<\varepsilon/2$ for $n,j\ge N$. For each $n\ge N$, the bound passes to the real limit in $j$ by [math:lem-limit-preserves-order](https://alphabetamath.cc/item/lem-limit-preserves-order), so $d(b_n,\xi)\le\varepsilon/2<\varepsilon$. By [math:def-metric-convergence](https://alphabetamath.cc/item/def-metric-convergence), applied to $(b_{k+1})_{k\ge0}$ to index from zero, the embedded lifts converge to $\xi$.

For the tuple of residues of an integer $a$, write $b_n$ for that lift. Since $b_n\equiv a\pmod{\ell^n}$, their difference is a multiple of $\ell^n$. If the difference is nonzero then $v_\ell(b_n-a)\ge n$ by the integer exponent formula, so $|b_n-a|_\ell\le\ell^{-n}$ by strict decrease. The same bound holds when the difference is zero. By the power laws, $\ell^{-n}=(1/\ell)^n$. In the real ordered field, reciprocating $0<1<\ell$ gives $0<1/\ell<1$ by [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive). The nonnegative clause of the ordinary real absolute value [math:def-abs-value](https://alphabetamath.cc/item/def-abs-value) gives $|1/\ell|=1/\ell<1$. Thus [math:lem-geometric-sequence-null](https://alphabetamath.cc/item/lem-geometric-sequence-null) gives $\ell^{-n}\to0$. By [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit), for every rational $\varepsilon>0$ the upper bound $\ell^{-n}$ is eventually less than $\varepsilon$, so the nonnegative termwise distances $|b_n-a|_\ell$ tend to zero. The completion identifies $(b_n)$ with the constant sequence at $a$ by [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers), so the image of the residue tuple is the embedded integer $a$.

Under this embedding the image is the closed unit ball by [the valuation ring identification](https://alphabetamath.cc/item/cor-zp-is-the-valuation-ring-of-qp). Thus $x\in\mathbb Z_\ell$ exactly when $v_\ell(x)\ge0$, including $x=0$. For $x\ne0$, $v_\ell(1)=0$ and the product law applied to $xx^{-1}=1$ gives $v_\ell(x^{-1})=-v_\ell(x)$. Hence $x$ is a unit of $\mathbb Z_\ell$, meaning that both $x$ and $x^{-1}$ belong to the ring, exactly when $v_\ell(x)=0$.

Since $\mathbb Q_\ell$ is a field, its nonzero elements form a multiplicative group $\mathbb Q_\ell^\times$ by [math:def-field](https://alphabetamath.cc/item/def-field). Use [math:def-group-power](https://alphabetamath.cc/item/def-group-power) for the powers of the nonzero embedded prime $\ell$ in this group. The recursion $\ell^0=1$, $\ell^{k+1}=\ell^k\ell$ gives $v_\ell(\ell^k)=k$ for all natural $k$ by the [induction principle](https://alphabetamath.cc/item/thm-induction-principle), using $v_\ell(1)=0$, $v_\ell(\ell)=1$ and the product law. For $k>0$, the clause $\ell^{-k}=(\ell^k)^{-1}$ and the inverse law give $v_\ell(\ell^{-k})=-k$. Thus $v_\ell(\ell^m)=m$ for every $m\in\mathbb Z$, so every element of the value group is attained.

Every nonzero $x$ can be written as $a/b$ with $a,b\in\mathbb Z_\ell$ nonzero by taking $b=\ell^n$ for a nonnegative $n$ with $n+v_\ell(x)\ge0$, then $a=bx$. In fact $v_\ell(b)=n$ and $v_\ell(a)=n+v_\ell(x)$ by normalization and the product law. For any such fraction, the product law applied to $bx=a$ gives $v_\ell(x)=v_\ell(a)-v_\ell(b)$, so this difference is independent of the choice of fraction.


## Hamilton algebras and the reduced norm

[Open item](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm) · level 0


### Definition

Let $F$ be a field with $\mathbb Q$ as a subfield. The underlying vector space of the Hamilton algebra $B(F)$ is $F^{\{0,1,2,3\}}$, the space of quadruples over $F$. Write $1,i,j,k$ for its standard ordered basis and $x=a+bi+cj+dk$ for the quadruple with coordinates $a,b,c,d\in F$. It has coordinatewise addition and scalar multiplication, and multiplication that is linear over $F$ in each factor, with identity $1$ and table $i^2=j^2=k^2=-1$, $ij=k$, $jk=i$, $ki=j$, $ji=-k$, $kj=-i$, and $ik=-j$. A scalar $a$ is identified with $a\cdot1$. Write $B=B(\mathbb Q)$ for the rational Hamilton algebra. The conjugate of $x$ is $\bar x=a-bi-cj-dk$ and its reduced norm is $N(x)=a^2+b^2+c^2+d^2\in F$, also written $\operatorname{nrd}(x)$. Use $B(F)^\times$ for the units, meaning the elements with a two-sided multiplicative inverse in $B(F)$.

### Definition references

[math:def-subfield](https://alphabetamath.cc/item/def-subfield)

[math:def-function-space](https://alphabetamath.cc/item/def-function-space)

[math:lem-standard-basis-of-f-n](https://alphabetamath.cc/item/lem-standard-basis-of-f-n)

[math:def-linear-map](https://alphabetamath.cc/item/def-linear-map)

### Justification

The coefficient fields have commutative arithmetic and inverses for nonzero scalars by [math:def-field](https://alphabetamath.cc/item/def-field) and [math:thm-rat-field](https://alphabetamath.cc/item/thm-rat-field). With the pointwise operations of [math:def-function-space](https://alphabetamath.cc/item/def-function-space), the quadruples satisfy the axioms of [math:def-vector-space](https://alphabetamath.cc/item/def-vector-space). Each quadruple has a unique expansion in the ordered basis by [math:lem-standard-basis-of-f-n](https://alphabetamath.cc/item/lem-standard-basis-of-f-n). To construct the product, take each term of the first expansion and each term of the second, multiply their scalar coefficients in $F$, multiply their basis vectors by the table, and add the sixteen resulting scalar multiples. Distributivity in $F$ makes the product linear in each factor in the sense of [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map), and bilinearity forces this expansion. The table agrees with that of [math:def-quaternions](https://alphabetamath.cc/item/def-quaternions), whose real coordinate product is bilinear.

Let $\iota:\mathbb Q\to\mathbb R$ be the ordered field embedding of [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense). The table entries are signed basis vectors with coordinates in $\{0,1,-1\}$. Both bracketings of any basis triple can thus be computed over $\mathbb Q$, and applying $\iota$ to the coordinates gives the two real bracketings, which agree by [math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring). Injectivity gives equality of the rational coordinates. The inclusion of $\mathbb Q$ as a subfield of $F$ preserves its arithmetic and the constants $0,1,-1$ by [math:def-subfield](https://alphabetamath.cc/item/def-subfield), so the same equality holds over $F$. Expanding by linearity in each of the three entries extends that equality to all triples. The table gives the identity and the definition of the product gives both distributive laws. Scalars commute with every basis vector, hence with every element. These operations make $B(F)$ an associative algebra over $F$, meaning a vector space over $F$ with associative, bilinear multiplication and identity.

Conjugation is $F$-linear because leaving the scalar coordinate fixed and negating the other three commutes with taking linear combinations. For a pair of basis vectors, the coordinates on both sides of $\overline{xy}=\bar y\bar x$ are computed from the same rational table and signs. Their real images agree by [math:lem-quaternion-conjugation-is-an-anti-involution](https://alphabetamath.cc/item/lem-quaternion-conjugation-is-an-anti-involution), so injectivity of $\iota$ and the subfield inclusion give equality over $F$ on each basis pair. Both sides are bilinear, so the identity holds for all pairs. Expanding $x\bar x$ and $\bar x x$ cancels the mixed terms since distinct vectors among $i,j,k$ anticommute, meaning their products in opposite orders are negatives. Their squares are $-1$, so $x\bar x=\bar x x=N(x)\cdot1$. Therefore $(xy)\overline{xy}=x(y\bar y)\bar x=N(y)N(x)\cdot1$ and $N(xy)=N(x)N(y)$. The table and norm formula give $N(1)=1$. If $N(x)\ne0$, the formula $\bar x/N(x)$ gives a two-sided inverse. Conversely, if $x$ has inverse $y$, then $N(x)N(y)=1$.

For nonzero $x\in B$, applying $\iota$ to its four coordinates gives a nonzero real quaternion, since a nonzero coordinate stays nonzero. Preservation of addition and multiplication gives the real norm of that quaternion as $\iota(N(x))$, which is positive by [math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring). Since $\iota(0)=0$ and $\iota$ reflects strict order, $N(x)>0$ in the rational order of [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order).


## Integral structure of the Hurwitz order

[Open item](item-thm-hurwitz-order-integral-structure) · level 1


### Statement

Let $B$ be the rational Hamilton algebra, the real quaternions with all coordinates restricted to rational numbers in the basis $1,i,j,k$ with $i^2=j^2=-1$ and $ij=k=-ji$. The rational scalars act by multiplication by scalar quaternions $q1$. For $x=x_0+x_1i+x_2j+x_3k$, quaternion conjugation is $\bar x=x_0-x_1i-x_2j-x_3k$, the reduced trace is $T(x)=2x_0$, and the reduced norm is $N(x)=x_0^2+x_1^2+x_2^2+x_3^2$.

Identify each integer $n\in\mathbb Z$ with the rational number $n/1$.

Put $w=(-1+i+j+k)/2$ and let $O=\mathbb Z+\mathbb Zi+\mathbb Zj+\mathbb Zw$, the set of integer linear combinations of $1,i,j,w$. This is a lattice in $B$, meaning the integer span of a rational basis. It is a maximal $\mathbb Z$-order. Here a $\mathbb Z$-order is a subring with the same identity as $B$, generated additively by finitely many elements and spanning $B$ by rational linear combinations. Maximality means that every $\mathbb Z$-order in $B$ containing $O$ equals $O$.

In the basis $1,i,j,k$ its coordinate set is $\mathbb Z^4\cup(\mathbb Z+\tfrac12)^4$, where $\mathbb Z+\tfrac12=\{n+\tfrac12:n\in\mathbb Z\}$. For each $x\in O$, both $T(x)$ and $N(x)$ are integers and $\bar x\in O$.

### Statement references

[Quaternion coordinates and operations](https://alphabetamath.cc/item/def-quaternions)

[The integers](https://alphabetamath.cc/item/def-integers)

[The embedding of integers into the rationals](https://alphabetamath.cc/item/lem-int-embeds-rat)

[Algebras and central scalars](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)

[Module bases and unique coefficients](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis)

[Orders in rational algebras](item-def-author-53081a7cb32d-order-in-a-rational-algebra)

### Facts & Assumptions

[F1] Rational numbers can be represented as fractions of integers with nonzero denominators, and the canonical rational embedding into the reals preserves their arithmetic. [Rational numbers](https://alphabetamath.cc/item/def-rationals) [The rational embedding](https://alphabetamath.cc/item/lem-rat-embeds-dense) The embedding of the integers into the rationals preserves addition, multiplication and order. [The integers](https://alphabetamath.cc/item/def-integers) [The integer embedding](https://alphabetamath.cc/item/lem-int-embeds-rat)

[F2] Quaternion addition is componentwise, and the multiplication formula is bilinear, meaning it distributes over addition and commutes with scalar multiplication in each argument. The multiplication table gives $i^2=j^2=k^2=-1$, $ij=k$, $jk=i$, $ki=j$, and the reversed products have opposite signs. A quaternion with only its first coordinate nonzero acts by scaling every coordinate by that number. The norm and conjugation are the coordinate formulas in the statement. [Quaternion operations and basis products](https://alphabetamath.cc/item/def-quaternions)

[F3] With these operations the real quaternions form a ring with identity $1$, and $x\bar x=N(x)1$. [Quaternion ring and norm identity](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring)

[F4] A map from the scalar field to a unital ring gives an algebra structure if it preserves addition, multiplication and the identity, and every element of its image commutes with every element of the ring. The elements of a basis give each element of the ambient space a unique finite linear expansion. [Algebras over a commutative ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring) [Bases and unique coefficients](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis)

[F5] A subring contains the ambient identity and is closed under addition, additive inverses and multiplication. An order also has a finite list of integer generators and spans the ambient algebra over the rationals. It is maximal if every containing order in that algebra is equal to it. [Subrings](https://alphabetamath.cc/item/def-subring) [Orders in rational algebras](item-def-author-53081a7cb32d-order-in-a-rational-algebra)

[F6] Conjugation reverses products and squares to the identity, so $\overline{xy}=\bar y\bar x$ and $\overline{\bar x}=x$. Also $x+\bar x=T(x)1$. [Quaternion conjugation identities](https://alphabetamath.cc/item/lem-quaternion-conjugation-is-an-anti-involution)

[F7] Each positive integer has a factorization into a finite list of primes, unique up to the order of the factors. A prime here is an integer greater than $1$ whose only positive divisors are $1$ and itself. [Fundamental theorem of arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic) [Prime integers](https://alphabetamath.cc/item/def-prime)

[F8] An integer $d$ divides $u$ if $u=dt$ for an integer $t$. [Divisibility in the integers](https://alphabetamath.cc/item/def-divides-in-z) Division of an integer by $2$ gives a remainder $r$ with $0\le r<2$. [Division with remainder in the integers](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

[F9] The integers form a totally ordered commutative ring. [Ordered integer arithmetic](https://alphabetamath.cc/item/thm-int-ordered-ring)

[F10] If a positive integer $d$ divides a positive integer $u$, then $d\le u$. Taking $d=1$ shows that every positive integer is at least $1$. [Divisor bound](https://alphabetamath.cc/item/lem-divisor-bound)

[F11] Every nonempty set of integers bounded above by an integer has a greatest element. [Greatest element of a bounded set of integers](https://alphabetamath.cc/item/lem-int-bounded-above-has-greatest)

### Proof

**Given:** $B$, $w$ and $O$ as in the statement.

**Goal:** Prove the lattice and coordinate descriptions, integer trace and norm, stability under conjugation, and maximality.

1.1 Rational tuples are closed under quaternion addition, additive inverses and multiplication because the coordinate formulas use sums and products of rationals. They include the identity $1$ and inherit the real quaternion ring laws. By the product formula, $q\mapsto q1$ is a unital map that preserves sums and products and commutes with every quaternion. Hence $B$ is a rational algebra. [F1, F2, F3, F4, F5]

2.1 If $x=c_0+c_1i+c_2j+c_3w$, its coordinates satisfy $x_0=c_0-c_3/2$, $x_1=c_1+c_3/2$, $x_2=c_2+c_3/2$, and $x_3=c_3/2$. Conversely, these equations recover the unique coefficients $c_3=2x_3$, $c_0=x_0+x_3$, $c_1=x_1-x_3$, and $c_2=x_2-x_3$. These are rational for every $x\in B$, so $1,i,j,w$ form a rational basis. For any remainder $r$ with $0<r<2$, both $r$ and $2-r$ are positive integers, so each is at least $1$. Hence the remainder on division by $2$ is $0$ or $1$. Integer coefficients give four integer coordinates when $c_3$ is even and four coordinates in $\mathbb Z+\tfrac12$ when it is odd. In either of these two coordinate classes, the recovered coefficients are all integers. Thus $O$ is the integer span of this basis and has the stated coordinate set. [F1, F2, F4, F8, F9, F10, step 1.1]

2.2 For $x,y\in B$, the quaternion product with its conjugate satisfies $(xy)\overline{xy}=xy\bar y\bar x=N(y)x\bar x=N(y)N(x)1$, using the commutation of scalar quaternions. Comparing the scalar coordinates gives $N(xy)=N(x)N(y)$. [F2, F3, F6, step 1.1]

3.1 In particular $k=2w+1-i-j$ lies in $O$. The table gives $i^2=j^2=-1$, $ij=k$, $ji=-k$, and expansion of $w$ gives $iw=wj=w-i-j$, $wi=w-i-k$, and $jw=w-j-k$. For $v=i+j+k$ the mixed terms in $v^2$ cancel in pairs and $v^2=-3$, so $w^2=(-1+v)^2/4=-1-w$. Products with $1$ preserve each basis element. All these products belong to $O$, so the product of two integer combinations belongs to $O$ by bilinearity. The integer span contains $1$ and is closed under addition and additive inverses. The basis from step 2.1 gives both order conditions, so $O$ is a $\mathbb Z$-order. [F2, F4, F5, step 1.1, step 2.1]

3.2 Let $S$ be any $\mathbb Z$-order in $B$. Take a positive integer $D$ divisible by the denominators of the four coordinates of each member of a finite integer generating list for $S$. Such a $D$ is the product of those positive denominators, which can be made positive by changing both signs in each fraction as needed. For each $z\in S$, the coordinates of $Dz$ are integers, so $D^2N(z)$ is an integer. The norm is nonnegative, so we can write $N(z)=a/b$ with $b>0$, cancelling all common prime factors of the positive numerator and denominator when $N(z)>0$ and using $0/1$ when $N(z)=0$. In every such reduced representation, $b$ divides $D^2$ because $D^2a/b$ is an integer and every prime factor of $b$, with its multiplicity, must occur in $D^2$. The divisor bound gives $b\le D^2$ because $b$ and $D^2$ are positive. The set of all positive denominators occurring in reduced representations of norms of elements of $S$ is nonempty because $1\in S$ and $N(1)=1$. It therefore has a greatest element $b$. If $b>1$, choose $z\in S$ with $N(z)=a/b$ in reduced form. Then $z^2\in S$ and $N(z^2)=a^2/b^2$ has reduced denominator $b^2$, since squaring introduces no common prime factor. This contradicts maximality of $b$ because $b^2-b=b(b-1)>0$. Thus $b=1$ and every $z\in S$ has integer norm. [F1, F2, F3, F5, F7, F8, F9, F10, F11, step 2.2]

4.1 For $z\in S$ we also have $z+1\in S$. Expanding the coordinate squares gives $T(z)=N(z+1)-N(z)-1$, an integer by step 3.2. The identity $\bar z=T(z)1-z$ then implies $\bar z\in S$, since $S$ contains $1$ and is closed under addition and additive inverses. Conjugating twice returns the original element, so conjugation maps $S$ onto itself. This applies in particular to $S=O$. [F2, F5, F6, step 3.1, step 3.2]

5.1 Suppose now that $S$ contains $O$. For any $z=x_0+x_1i+x_2j+x_3k\in S$, the elements $z,zi,zj,zk$ belong to $S$ since $1,i,j,k\in O$. Their scalar coordinates are $x_0,-x_1,-x_2,-x_3$ by the basis product table. The four traces therefore give $2x_r\in\mathbb Z$ for each $r\in\{0,1,2,3\}$. [F2, F5, step 3.1, step 4.1]

6.1 Write $m_r=2x_r=2q_r+\varepsilon_r$ with $q_r\in\mathbb Z$ and $\varepsilon_r\in\{0,1\}$. Then $m_r^2=4(q_r^2+q_r\varepsilon_r)+\varepsilon_r$. The sum of the four squares $m_r^2$ equals $4N(z)$, a multiple of $4$, so $\sum_{r=0}^3\varepsilon_r$ is a multiple of $4$ between $0$ and $4$. If the sum is positive, its positive divisor $4$ is at most the sum, so the sum equals $4$. If the sum is $0$, all four remainders are $0$ and every $x_r$ is integral. If it is $4$, all four are $1$ and every $x_r$ lies in $\mathbb Z+\tfrac12$. Thus every $z\in S$ belongs to $O$ by step 2.1, so $S=O$. This proves maximality and completes the claims. [F5, F8, F9, F10, step 2.1, step 3.2, step 5.1] ∎

### Source notes

The basis and the trace and parity reduction follow Voight, Lemma 11.1.2. Step 3.1 does the multiplication check posed in Exercise 11.1 using $w$, which differs from the generator in the exercise by $-1$. Steps 2.2, 3.2 and 4.1 obtain norm and trace integrality from bounded denominators of the norms in any given order. [John Voight, The Hurwitz order](https://link.springer.com/chapter/10.1007/978-3-030-56694-4_11)


## Order of the degree-two finite projective group

[Open item](item-lem-degree-two-projective-group-cardinality) · level 1


### Statement

Let $F$ be a finite field, with $q=|F|$ the number of elements in its underlying set. Write $F^\times=F\setminus\{0\}$ for its nonzero elements. Let $L=\mathrm{GL}_2(F)$ be the group of invertible $2\times 2$ matrices over $F$ under matrix multiplication. A matrix is invertible if it has a two-sided inverse for this product. Let $I$ denote the identity matrix, with ones on the diagonal and zeros elsewhere.

The degree-two projective linear group $G=\mathrm{PGL}_2(F)$ is the quotient of $L$ by the scalar subgroup $Z=\{tI:t\in F^\times\}$. Its elements are the left cosets $AZ=\{Az:z\in Z\}$, with product $(AZ)(BZ)=(AB)Z$. Then
$$|G|=\frac{(q^2-1)(q^2-q)}{q-1}=q(q^2-1).$$

For any subgroup $H$ of $G$, meaning a subset containing the identity and closed under products and inverses, let $H\backslash G=\{Hg:g\in G\}$ be the set of right cosets $Hg=\{hg:h\in H\}$. Then
$$|H\backslash G|=\frac{q(q^2-1)}{|H|}.$$

### Facts & Assumptions

[F1] A field has associative and commutative addition and multiplication, additive identity $0$, multiplicative identity $1\ne 0$, additive inverses, distributivity, and a multiplicative inverse for every nonzero element ([field](https://alphabetamath.cc/item/def-field)). Its operations make it a commutative ring, meaning that addition forms a commutative group and multiplication is associative and commutative, has an identity and distributes over addition ([field as a commutative ring](https://alphabetamath.cc/item/lem-field-is-a-commutative-ring)), and $0t=0$ for every $t\in F$ ([zero multiplication](https://alphabetamath.cc/item/lem-ring-elementary-consequences)). Thus the units, elements with a multiplicative inverse, are exactly $F^\times$. A finite field has a finite underlying set, and its order is the cardinality of that set ([finite field and its order](https://alphabetamath.cc/item/def-finite-field-and-its-order)).

[F2] The cardinality $|A|$ of a finite set $A$ is the unique natural number $n$ for which there is a bijection from $A$ to $\{0,\ldots,n-1\}$, the empty set for $n=0$. A bijection is a map for which each target element has exactly one preimage, and it transports finiteness and cardinality ([bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection), [finite cardinality](https://alphabetamath.cc/item/def-finite-cardinality)).

[F3] A $2\times 2$ matrix over $F$ is an array of two rows and two columns with entries in $F$ ([matrices and columns](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring)). Numbering rows and columns from $1$, the matrix product has entries $(AB)_{ij}=a_{i1}b_{1j}+a_{i2}b_{2j}$. The identity $I$ has diagonal entries $1$ and all other entries $0$, so $tI$ has diagonal entries $t$ and all other entries $0$ ([matrix product, identity and scaling](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)).

[F4] A group has an associative product, a two-sided identity and two-sided inverses ([group](https://alphabetamath.cc/item/def-group)). A subgroup satisfies the identity, product and inverse conditions in the Statement ([subgroup](https://alphabetamath.cc/item/def-subgroup)). The left and right cosets of a subgroup $K$ represented by $g$ are $gK=\{gk:k\in K\}$ and $Kg=\{kg:k\in K\}$ ([cosets](https://alphabetamath.cc/item/def-coset)). The quotient group here consists of the left cosets with their representative product. The projective linear group definition supplies the groups $L$ and $G$, the subgroup $Z$, and the quotient construction over the field $F$ ([quotient group](https://alphabetamath.cc/item/def-quotient-group), [degree-two projective linear group](item-def-degree-two-projective-linear-group)).

[F5] Over a commutative ring the determinant of a $2\times 2$ matrix with first column $(a,c)$ and second column $(b,d)$ is the scalar $ad-bc$ ([two-by-two determinant formula](https://alphabetamath.cc/item/ex-two-by-two-determinant-formula)). For a square matrix of positive size over a commutative ring, the determinant is defined by the signed Leibniz formula ([determinant definition](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)). A square matrix of positive size over a commutative ring is invertible exactly when its determinant is a unit ([invertibility criterion](https://alphabetamath.cc/item/cor-square-matrix-invertible-iff-determinant-is-a-unit)).

[F6] The Cartesian product $A\times B$ is the set of ordered pairs with first entry in $A$ and second entry in $B$. For finite $A,B$ its cardinality is $|A|\,|B|$ ([Cartesian product](https://alphabetamath.cc/item/def-cartesian-product), [product rule](https://alphabetamath.cc/item/thm-product-rule)). A subset of a finite set is finite ([finite subsets](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)). Two ordered pairs are equal exactly when their first entries agree and their second entries agree ([coordinatewise equality of ordered pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)).

[F7] The cardinality of a union of a finite family of pairwise disjoint finite sets, meaning distinct members share no elements, is the sum of their cardinalities ([sum rule](https://alphabetamath.cc/item/thm-sum-rule)). A sum over a finite index set $S$ adds the values once for each element of $S$, in any enumeration, and if every value is $c$, the sum is $|S|c$ ([finite sum and constant clause](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)).

[F8] For a finite group $J$ and a subgroup $K$, the set $J/K$ of left cosets is finite and its cardinality is the index $[J:K]$ ([index](https://alphabetamath.cc/item/def-index), [finite coset set](https://alphabetamath.cc/item/lem-finite-coset-partition)). Lagrange's theorem gives $|J|=[J:K]|K|$ ([Lagrange's theorem](https://alphabetamath.cc/item/thm-lagrange)). For any group and subgroup the map $gK\mapsto Kg^{-1}$ is a well-defined bijection from left cosets to right cosets ([left and right coset bijection](https://alphabetamath.cc/item/lem-left-and-right-cosets-equinumerous)).

[F9] For sets $A$ and $B$, an element lies in $A\setminus B$ exactly when it belongs to $A$ and does not belong to $B$. [set difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference)

### Proof

**Given:** A finite field $F$ of order $q$ and a subgroup $H$ of $G=\mathrm{PGL}_2(F)$ as in the Statement.

**Goal:** Compute $|G|$ and the number of right cosets of $H$.

1.1 Write $V=F\times F$, viewing an ordered pair as a column. For columns $v=(a,c)$ and $w=(b,d)$, write $[v\ w]$ for the matrix with those columns. The matrix has positive size over the commutative ring $F$. By the determinant criterion it belongs to $L$ exactly when $ad-bc\ne 0$, since the units of $F$ are precisely its nonzero elements. If $v=(0,0)$ the scalar is zero. [F1, F3, F4, F5, F6]

1.2 The product rule gives $|V|=q^2$. The sets $F^\times$ and $V\setminus\{(0,0)\}$ are finite subsets. Each complement and its excluded singleton are disjoint and together exhaust the ambient set. Separating the respective singletons, each of cardinality $1$, gives $|F^\times|=q-1$ and $|V\setminus\{(0,0)\}|=q^2-1$ by the sum rule. Since $0$ and $1$ are distinct elements of $F$, $q\ge 2$. [given, F1, F2, F6, F7, F9]

2.1 Fix $v=(a,c)\ne(0,0)$ and write $Fv=\{(ta,tc):t\in F\}$ for its scalar multiples. If $w=(ta,tc)$ then $ad-bc=a(tc)-(ta)c=0$. Conversely, if $ad-bc=0$ and $a\ne 0$, set $t=a^{-1}b$. Then $b=ta$ and $d=a^{-1}bc=tc$. If $a=0$ then $c\ne 0$, and $bc=0$ gives $b=0$ by multiplication by $c^{-1}$. In this case set $t=c^{-1}d$ to get $(b,d)=(ta,tc)$. Thus the allowed second columns are exactly $V\setminus Fv$. [F1, F9, step 1.1]

3.1 For nonzero $v=(a,c)$, the map $t\mapsto(ta,tc)$ from $F$ to $Fv$ reaches every element of $Fv$ by definition. If $(ta,tc)=(sa,sc)$, the two pairs agree coordinate by coordinate. Choose a nonzero coordinate of $v$ and multiply the equality in that coordinate by its inverse to get $t=s$. The bijection gives $|Fv|=q$. A column lies in $V\setminus Fv$ exactly when it belongs to $V$ and does not belong to $Fv$. Hence $Fv$ and $V\setminus Fv$ are disjoint subsets with union $V$. Both are finite, so the sum rule gives $|V\setminus Fv|=q^2-q$. [F1, F2, F6, F7, F9, step 2.1, step 1.2]

4.1 For each nonzero first column $v$, the corresponding set of matrices in $L$ is in bijection with $V\setminus Fv$ by taking the second column. The inverse sends $w$ to $[v\ w]$. The two column pairs determine the four entries of this matrix. Every element of $L$ belongs to exactly one of these sets, since its first column is unique and nonzero. The sum rule over the $q^2-1$ possible first columns, with constant value $q^2-q$, gives $|L|=(q^2-1)(q^2-q)$ and shows $L$ is finite. [F2, F3, F6, F7, step 1.1, step 2.1, step 1.2, step 3.1]

5.1 The map $t\mapsto tI$ from $F^\times$ to $Z$ reaches every element of $Z$, and reading a diagonal entry recovers $t$, so $|Z|=q-1$. The scalar subgroup $Z$ lies in the finite group $L$, and the elements of $G$ are the left cosets of $Z$. Therefore $G$ is finite and $|G|=[L:Z]=|L|/|Z|$ by Lagrange's theorem. Using $q^2-q=q(q-1)$ and $q-1>0$ gives $|G|=(q^2-1)(q^2-q)/(q-1)=q(q^2-1)$. [F2, F3, F4, F8, step 1.2, step 4.1]

6.1 Apply Lagrange's theorem to the finite group $G$ and its subgroup $H$. The group identity belongs to $H$, so $|H|>0$. The bijection $gH\mapsto Hg^{-1}$ carries the finite left coset set to $H\backslash G$, whence $|H\backslash G|=[G:H]=|G|/|H|=q(q^2-1)/|H|$. This proves the right coset formula and completes the two counts. [given, F2, F4, F8, step 5.1] ∎


## Determinant square class of a projective matrix

[Open item](item-lem-projective-determinant-square-class) · level 1


### Statement

Let $F$ be a field, let $F^\times$ be its multiplicative group of nonzero elements, and put $H=(F^\times)^2=\{u^2:u\in F^\times\}$. The square class of $t\in F^\times$ is the coset $tH=\{th:h\in H\}$. The group $\mathrm{PGL}_2(F)$ consists of invertible two-by-two matrices over $F$ up to multiplication by nonzero scalars. Write $[A]$ for the class represented by $A$.

The determinant induces a surjective group homomorphism
$$D_F:\mathrm{PGL}_2(F)\longrightarrow F^\times/H,\qquad D_F([A])=(\det A)H.$$
Here a group homomorphism preserves products, and surjective means every element of the target occurs as a value.

For the sign character, take a prime $p$, meaning an integer greater than one whose only positive divisors are $1$ and $p$. Assume $p$ is odd, meaning $2\nmid p$. Thus there is no integer $q$ with $p=2q$. Let $\mathbb F_p=\mathbb Z/p\mathbb Z$ be the field of integer residue classes modulo $p$, so integers represent the same class exactly when their difference is divisible by $p$. Write $[a]_p$ for the class of $a$. Addition and multiplication are given by $[a]_p+[b]_p=[a+b]_p$ and $[a]_p[b]_p=[ab]_p$. On $\mathbb F_p^\times$ the Legendre symbol has value $1$ on squares and $-1$ on all other elements. It induces a map $\overline{\lambda}_p$ on $F^\times/H$ for $F=\mathbb F_p$. The composite $\overline{\lambda}_p\circ D_{\mathbb F_p}$ is a nontrivial sign character, meaning a homomorphism to the multiplicative group of integer signs $\{1,-1\}$ that takes the value $-1$. Its value at $[A]$ is the Legendre symbol of $\det A$.

### Statement references

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

### Facts & Assumptions

[F1] A field is a commutative ring with $0\ne 1$ and with its nonzero elements forming a group under multiplication ([math:def-field](https://alphabetamath.cc/item/def-field) and [math:lem-field-is-a-commutative-ring](https://alphabetamath.cc/item/lem-field-is-a-commutative-ring)). Multiplying by zero in this ring gives zero ([math:lem-ring-elementary-consequences](https://alphabetamath.cc/item/lem-ring-elementary-consequences)).

[F2] Write $\mathrm{GL}_2(F)$ for the group of invertible two-by-two matrices over $F$ under matrix multiplication. In the degree-two projective linear group, the representatives of $[A]$ are the matrices $uA=(uI)A$ for $u\in F^\times$. The matrix $uA$ has entries obtained by multiplying those of $A$ by $u$, and $I$ is the identity matrix with ones on the diagonal and zeros elsewhere. The product is $[A][B]=[AB]$. An invertible matrix $A$ has a two-sided inverse $A^{-1}$, with $AA^{-1}=A^{-1}A=I$. Matrix multiplication uses $(AB)_{ij}=a_{i1}b_{1j}+a_{i2}b_{2j}$ ([def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)).

[F3] For $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ the two terms of the determinant formula give $\det A=ad-bc$ ([math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)). For square matrices of the same size over a commutative ring, $\det(AB)=\det(A)\det(B)$ ([math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative)).

[F4] A subgroup contains the identity and is closed under products and inverses ([math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)). A subgroup $N$ of a group $G$ is normal if $gNg^{-1}=N$ for all $g\in G$ ([math:def-normal-subgroup](https://alphabetamath.cc/item/def-normal-subgroup)). Its left cosets are the sets $gN=\{gn:n\in N\}$ ([math:def-coset](https://alphabetamath.cc/item/def-coset)). For normal $N$, the quotient group $G/N$ consists of these cosets with product $(gN)(kN)=(gk)N$ ([math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group) and [math:thm-quotient-group-laws](https://alphabetamath.cc/item/thm-quotient-group-laws)). A map of groups is a homomorphism if it preserves products ([math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)).

[F5] Every element of $\mathbb Z/p\mathbb Z$ is the residue class of some integer ([math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)). On residue classes, addition and multiplication are given by $[a]_p+[b]_p=[a+b]_p$ and $[a]_p[b]_p=[ab]_p$ ([math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)). For a prime $p$, the residue ring $\mathbb Z/p\mathbb Z$ with these operations is a field ([math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)). For a prime $p$ with $2\nmid p$ (an odd prime, using [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)), the Legendre symbol $\lambda_p$ on its nonzero classes assigns $1$ to squares and $-1$ to nonsquares ([math:def-legendre-symbol](https://alphabetamath.cc/item/def-legendre-symbol)). On the group of nonzero classes, this rule is well defined on residue classes and is a surjective group homomorphism to $\{1,-1\}$ ([math:prop-legendre-symbol-on-units-is-homomorphism](https://alphabetamath.cc/item/prop-legendre-symbol-on-units-is-homomorphism)).

### Proof

**Given:** A field $F$ and, for the sign character, a prime $p$ with $2\nmid p$ and $F=\mathbb F_p$.

**Goal:** Prove the determinant square-class formula defines a surjective group homomorphism and that its composite with the induced Legendre sign takes both signs.

1.1 The element $1=1^2$ belongs to $H$. For $u,v\in F^\times$, commutativity gives $u^2v^2=(uv)^2$, and $(u^2)^{-1}=(u^{-1})^2$ since $u^2(u^{-1})^2=(uu^{-1})^2=1$. Thus $H$ is a subgroup. Each $g\in F^\times$ commutes with every $h\in H$, so $ghg^{-1}=h$, which gives $gHg^{-1}=H$. Hence the cosets of $H$ form the quotient group $F^\times/H$ with the stated product. [F1, F4]

2.1 The two-by-two determinant formula gives $\det I=1$. For any $A\in\mathrm{GL}_2(F)$, multiplicativity gives $\det(A)\det(A^{-1})=\det I=1$, so $\det A\in F^\times$. If $[A']=[A]$, then $A'=(uI)A$ for some $u\in F^\times$. The same determinant formula gives $\det(uI)=u^2$, so $\det A'=u^2\det A$. Since $u^2\in H$, multiplication by $u^2$ carries $H$ onto itself with inverse multiplication by $(u^2)^{-1}\in H$. By commutativity, $(\det A')H=(\det A)(u^2H)=(\det A)H$. This proves independence of the choice of matrix representative. [F1, F2, F3, F4, step 1.1]

2.2 In the specialization $F=\mathbb F_p$ with $p$ prime and $2\nmid p$, the odd-prime hypothesis in [F5] holds. The units of this field are exactly the nonzero elements by [F1]. For $t\in F^\times$ and $h\in H$, take $u\in F^\times$ with $h=u^2$. Using the integer representatives from [F5], write $t=[a]_p$ and $u=[b]_p$. The modular product in [F5] gives $h=[b^2]_p$ and $th=[ab^2]_p$. Then $\lambda_p(th)=\lambda_p(t)\lambda_p(h)=\lambda_p(t)$ because $h$ is a nonzero square. Thus the formula $\overline{\lambda}_p(tH)=\lambda_p(t)$ gives a single sign for the entire coset. The quotient product and multiplicativity of $\lambda_p$ give $\overline{\lambda}_p((tH)(sH))=\lambda_p(ts)=\overline{\lambda}_p(tH)\overline{\lambda}_p(sH)$. Each sign occurs on a coset because it occurs on some $t\in F^\times$ by [F5]. [F1, F4, F5, step 1.1]

3.1 For any field $F$ and invertible $A,B$, $D_F([A][B])=(\det(AB))H=(\det(A)\det(B))H=D_F([A])D_F([B])$, using the two quotient products and determinant multiplicativity. Hence $D_F$ is a group homomorphism. [F2, F3, F4, step 1.1, step 2.1]

3.2 For any target coset $tH$, take $A=\begin{pmatrix}t&0\\0&1\end{pmatrix}$. Set $B=\begin{pmatrix}t^{-1}&0\\0&1\end{pmatrix}$. The matrix product formula gives $AB=\begin{pmatrix}tt^{-1}&0\\0&1\end{pmatrix}=I$ and $BA=\begin{pmatrix}t^{-1}t&0\\0&1\end{pmatrix}=I$, since $tt^{-1}=t^{-1}t=1$ and products with zero vanish. Thus $A$ is invertible, and its determinant is $t$. Therefore $D_F([A])=tH$, proving surjectivity. [F1, F2, F3, F4, step 2.1]

4.1 Since both $D_{\mathbb F_p}$ and $\overline{\lambda}_p$ preserve products, their composite preserves products. Each sign is attained by the composite because each sign is the image of a coset under $\overline{\lambda}_p$ and every coset is attained by $D_{\mathbb F_p}$. Thus the composite is nontrivial and its value at $[A]$ is $\overline{\lambda}_p((\det A)H)=\lambda_p(\det A)$, as claimed. [F4, F5, step 2.1, step 3.1, step 3.2, step 2.2] ∎


## Normalizer of a quadratic field torus in degree two

[Open item](item-lem-quadratic-field-normalizer-in-degree-two) · level 1


### Statement

Let $F$ be a finite field with $q=|F|$ elements and let $E/F$ be an extension of degree two, so that $E$ has dimension two over $F$. For a field $L$, write $L^\times$ for its multiplicative group of nonzero elements. For $a\in E$ let $m_a:E\to E$ be multiplication by $a$, given by $m_a(x)=ax$. Choose an ordered $F$-basis of $E$. Write $[S]$ for the class in $G=\mathrm{PGL}_2(F)$ of the matrix of an invertible $F$-linear map $S:E\to E$. Two such maps have the same class exactly when they differ by a scalar in $F^\times$.

The map $aF^\times\mapsto[m_a]$ identifies $C=E^\times/F^\times$ with the subgroup $T=\{[m_a]:a\in E^\times\}$ of $G$, called the quadratic field torus here. Let $N_G(T)=\{g\in G:gTg^{-1}=T\}$ be its normalizer, and let $H=\operatorname{Gal}(E/F)$ be the group of field automorphisms of $E$ fixing $F$ pointwise, with composition as product. With the action $\alpha_\sigma(aF^\times)=\sigma(a)F^\times$ of $H$ on $C$, there is a group isomorphism
$$C\rtimes_\alpha H\longrightarrow N_G(T),\qquad (aF^\times,\sigma)\longmapsto[m_a\circ\sigma].$$
Here the semidirect product has underlying set $C\times H$ and product $(c,\sigma)(d,\tau)=(c\alpha_\sigma(d),\sigma\circ\tau)$.

The normalizer is the disjoint union $T\cup T[\sigma_q]$, where $\sigma_q(x)=x^q$ is the relative Frobenius. Each class in $T[\sigma_q]$ has a representative $S=m_a\circ\sigma_q$ with $a\in E^\times$. It is semilinear over $E$ with respect to $\sigma_q$, meaning it is additive and satisfies $S(bx)=\sigma_q(b)S(x)$ for all $b,x\in E$. Here $T[\sigma_q]=\{t[\sigma_q]:t\in T\}$. Conjugation by $S$ sends $m_b$ to $m_{\sigma_q(b)}$ for every $b\in E$. The order of the normalizer, meaning its number of elements, is $2(q+1)$.

### Facts & Assumptions

[F1] A field has commutative, distributive multiplication and $0\ne1$. Its nonzero elements form a commutative group under multiplication. A finite field has a finite underlying set. In an extension $E/F$ we identify $F$ with its image in $E$, and the degree is the dimension of $E$ over $F$. ([math:def-field](https://alphabetamath.cc/item/def-field), [math:def-finite-field-and-its-order](https://alphabetamath.cc/item/def-finite-field-and-its-order), [math:def-field-extension-generated-subfields-and-simple-extension](https://alphabetamath.cc/item/def-field-extension-generated-subfields-and-simple-extension), [math:def-extension-degree-and-finite-extension](https://alphabetamath.cc/item/def-extension-degree-and-finite-extension)).

[F2] A space of dimension two has a two-element basis, which can be ordered. Any ordered basis is an injective list whose image is a finite basis, so it also has two vectors by uniqueness of the size of a finite basis. In such a basis every vector has exactly one pair of coordinates. An $F$-linear map preserves $F$-linear combinations. It is invertible if it has an $F$-linear inverse. The columns of its matrix are the coordinate columns of the images of the basis vectors, and composition gives matrix multiplication. For finite-dimensional spaces with ordered bases, invertible linear maps have invertible matrices. Conversely, an invertible matrix acts invertibly and linearly on coordinate columns. ([math:def-dimension](https://alphabetamath.cc/item/def-dimension), [math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis), [math:thm-unique-coordinates-with-respect-to-an-ordered-basis](https://alphabetamath.cc/item/thm-unique-coordinates-with-respect-to-an-ordered-basis), [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map), [math:def-linear-isomorphism-and-invertible-linear-map](https://alphabetamath.cc/item/def-linear-isomorphism-and-invertible-linear-map), [math:def-coordinate-column-and-matrix-of-a-linear-map](https://alphabetamath.cc/item/def-coordinate-column-and-matrix-of-a-linear-map), [math:thm-matrix-of-a-composite-is-the-product](https://alphabetamath.cc/item/thm-matrix-of-a-composite-is-the-product), [math:thm-invertible-matrices-correspond-to-linear-isomorphisms](https://alphabetamath.cc/item/thm-invertible-matrices-correspond-to-linear-isomorphisms)).

[F3] The projective group is the quotient of the invertible matrices by the nonzero scalar matrices, with $[A][B]=[AB]$. A subgroup $D$ is normal if each conjugation $d\mapsto ada^{-1}$ in the ambient group sends $D$ onto itself. For normal $D$, the left cosets $aD=\{ad:d\in D\}$ form a group under the well-defined product $(aD)(bD)=abD$. A subset containing the identity and closed under products and inverses is a subgroup. For a subgroup $T$ of $G$, the set of $g$ with $gTg^{-1}=T$ is a subgroup of $G$. ([def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group), [math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group), [math:thm-quotient-group-laws](https://alphabetamath.cc/item/thm-quotient-group-laws), [math:def-normal-subgroup](https://alphabetamath.cc/item/def-normal-subgroup), [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup), [math:def-normalizer-of-a-subgroup](https://alphabetamath.cc/item/def-normalizer-of-a-subgroup), [math:lem-centralizers-and-normalizers-are-subgroups](https://alphabetamath.cc/item/lem-centralizers-and-normalizers-are-subgroups)).

[F4] An $F$-automorphism of $E$ is a bijective field map fixing $F$ pointwise, with field maps preserving addition, multiplication and $1$. For an extension of finite fields of degree $n$ over a field of $q$ elements, the extension is Galois and its group of $F$-automorphisms is cyclic with $n$ elements under composition, generated by the relative Frobenius $x\mapsto x^q$. To say that an element generates the group means that the smallest subgroup containing that element is the whole group. The element order of an automorphism in this finite group is the least positive $k$ for which its $k$-fold iterate is the identity. ([math:def-relative-field-automorphism-group](https://alphabetamath.cc/item/def-relative-field-automorphism-group), [math:def-field-homomorphism](https://alphabetamath.cc/item/def-field-homomorphism), [math:def-finite-galois-extension-and-galois-group](https://alphabetamath.cc/item/def-finite-galois-extension-and-galois-group), [math:def-relative-frobenius-of-a-finite-field-extension](https://alphabetamath.cc/item/def-relative-frobenius-of-a-finite-field-extension), [math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group](https://alphabetamath.cc/item/thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group), [math:def-generated-subgroup](https://alphabetamath.cc/item/def-generated-subgroup), [math:def-order-in-a-group](https://alphabetamath.cc/item/def-order-in-a-group)).

[F5] An action of a group $H$ on a group $C$ by automorphisms assigns each $h$ an invertible product-preserving map $\alpha_h:C\to C$, with $\alpha_1=\mathrm{id}_C$ and $\alpha_{h k}=\alpha_h\circ\alpha_k$. For such an action the pair law $(c,h)(d,k)=(c\alpha_h(d),hk)$ makes $C\rtimes_\alpha H$ a group. A bijective product-preserving map between groups is an isomorphism. ([math:def-action-by-automorphisms](https://alphabetamath.cc/item/def-action-by-automorphisms), [math:def-external-semidirect-product](https://alphabetamath.cc/item/def-external-semidirect-product), [math:thm-external-semidirect-product-is-a-group](https://alphabetamath.cc/item/thm-external-semidirect-product-is-a-group), [math:def-group-isomorphism-and-automorphism](https://alphabetamath.cc/item/def-group-isomorphism-and-automorphism)).

[F6] Finite cardinality $|X|$ is the number of elements of $X$ and is unchanged by bijections. A $d$-dimensional space over a field with $q$ elements has $q^d$ elements. Every subset of a finite set is finite. Cardinalities add for disjoint finite sets. ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality), [math:lem-cardinality-of-a-finite-dimensional-space-over-a-finite-field](https://alphabetamath.cc/item/lem-cardinality-of-a-finite-dimensional-space-over-a-finite-field), [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set), [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)).

[F7] For a subgroup $D$ of a finite group $U$, the set $U/D$ of left cosets is finite and its cardinality is the index $[U:D]$. Lagrange's theorem gives $|U|=[U:D]\,|D|$. Two finite sets have a Cartesian product whose cardinality is the product of their cardinalities. ([math:lem-finite-coset-partition](https://alphabetamath.cc/item/lem-finite-coset-partition), [math:thm-lagrange](https://alphabetamath.cc/item/thm-lagrange), [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)).

[F8] For linear maps $A,B:E\to E$ and $c\in F$, the pointwise operations satisfy $(A+B)(x)=A(x)+B(x)$ and $(cA)(x)=cA(x)$ for each $x\in E$. The zero map $0$ sends each $x$ to $0$ in $E$. Multiplication by zero in a field gives $0x=0$. ([math:def-vector-space-of-linear-maps](https://alphabetamath.cc/item/def-vector-space-of-linear-maps), [math:lem-of-zero-mult](https://alphabetamath.cc/item/lem-of-zero-mult)).

### Proof

**Given:** A finite field $F$ of order $q$, an extension $E/F$ of degree two, and an ordered $F$-basis of $E$.

**Goal:** Identify the projective multiplication subgroup and its normalizer, prove the semidirect product and Frobenius descriptions, and compute the normalizer order.

1.1 By dimension two the chosen ordered basis has two vectors. Its coordinates identify invertible $F$-linear maps on $E$ with invertible two-by-two matrices. The scalar map $x\mapsto cx$ has matrix $cI$ for $c\in F^\times$. For $a,b\in E$, distributivity and commutativity show that $m_a$ is $F$-linear, and evaluation at each $x\in E$ gives $m_a+m_b=m_{a+b}$, $c m_b=m_{cb}$ for $c\in F$, and $m_a\circ m_b=m_{ab}$. Also $m_1=\mathrm{id}_E$, and $0x=0$ gives $m_0=0$. Evaluation at $1$ distinguishes the maps $m_a$. For $a\ne0$, $m_{a^{-1}}$ is the inverse of $m_a$. The inclusion of fields identifies $F^\times$ with a subgroup of the commutative group $E^\times$, since the inclusion preserves $1$, products and inverses. Every conjugation in $E^\times$ acts as the identity, so $F^\times$ is normal. The quotient group laws therefore apply to $C$. For $a,b\in E^\times$, $[m_a]=[m_b]$ holds exactly when $m_a=c m_b$ for some $c\in F^\times$, or equivalently $a=cb$. If the cosets agree then $a\in bF^\times$, and conversely $a=cb$ gives $aF^\times=bF^\times$ because multiplication by $c$ permutes $F^\times$. Thus $aF^\times\mapsto[m_a]$ is well defined and injective, and $m_a\circ m_b=m_{ab}$ proves it preserves the quotient product. The image contains the identity and is closed under products and inverses, so this is an isomorphism onto the subgroup $T$. [F1, F2, F3, F5, F8]

2.1 Take $g\in N_G(T)$ and an invertible $F$-linear map $S$ representing it. For every $b\in E^\times$ there is a $d\in E^\times$ with $[S\circ m_b\circ S^{-1}]=[m_d]$. Equality of projective classes gives $S\circ m_b\circ S^{-1}=c m_d=m_{cd}$ for some $c\in F^\times$. Applying the same argument to $g^{-1}$ shows that conjugation by $S$ maps the nonzero multiplication maps onto themselves. It fixes the zero map because $S(0)=0$, so it permutes all the maps $m_b$ for $b\in E$. [F2, F3, F8, step 1.1]

2.2 By the cardinality formula for a two-dimensional space, $|E|=q^2$. Apply the finite-field theorem with degree two. It gives $|H|=2$ and says that $\sigma_q$ generates $H$. The identity generates only the trivial subgroup, so $\sigma_q$ is the unique nonidentity element of $H$, and $H=\{\mathrm{id}_E,\sigma_q\}$. Its inverse is also a nonidentity element because the inverse of the identity is the identity. Thus $\sigma_q^{-1}=\sigma_q$, and $\sigma_q\circ\sigma_q=\mathrm{id}_E$ gives element order two. For any $\sigma\in H$, both $\sigma$ and its inverse preserve addition and fix $F$ and hence are $F$-linear by multiplicativity. For $b,x\in E$, $(\sigma\circ m_b\circ\sigma^{-1})(x)=\sigma(b)x$. In particular $[\sigma]$ normalizes $T$ since $\sigma$ permutes $E^\times$. Each $[m_a]\in T$ normalizes $T$ as well, and consequently every $[m_a\circ\sigma]$ belongs to $N_G(T)$. [given, F1, F2, F3, F4, F6, step 1.1]

3.1 Define $\sigma:E\to E$ by $S\circ m_b\circ S^{-1}=m_{\sigma(b)}$. This map is bijective by the preceding permutation and evaluation at $1$. At each $x\in E$, linearity of $S$ gives $S((m_b+m_d)(S^{-1}(x)))=S(m_b(S^{-1}(x)))+S(m_d(S^{-1}(x)))$, so conjugation preserves these pointwise sums. It preserves compositions and the identity map by the inverse equations. The addition and multiplication formulas for $m_b$ therefore give $\sigma(b+d)=\sigma(b)+\sigma(d)$, $\sigma(bd)=\sigma(b)\sigma(d)$, and $\sigma(1)=1$. For $b\in F$, the map $m_b$ is scalar multiplication and commutes with $S$, so $\sigma(b)=b$. Thus $\sigma\in H$. Replacing $S$ by $cS$ for $c\in F^\times$ leaves conjugation unchanged because the scalar map commutes with every $F$-linear map. The intertwining equation $S\circ m_b=m_{\sigma(b)}\circ S$ at $1$ now gives $S(b)=\sigma(b)S(1)$ for every $b\in E$. Since $S$ is injective and $S(0)=0$, $a=S(1)$ is nonzero. Thus $S=m_a\circ\sigma$. [F1, F2, F4, F8, step 1.1, step 2.1]

3.2 For $\sigma\in H$, since $\sigma$ fixes $F$ pointwise, replacing $a$ by $ca$ with $c\in F^\times$ multiplies $\sigma(a)$ by the same $c$. Thus $\alpha_\sigma(aF^\times)=\sigma(a)F^\times$ is well defined and preserves the quotient product by multiplicativity of $\sigma$. Its inverse is $\alpha_{\sigma^{-1}}$. Evaluating on cosets gives $\alpha_{\mathrm{id}_E}=\mathrm{id}_C$ and $\alpha_{\sigma\circ\tau}=\alpha_\sigma\circ\alpha_\tau$. This supplies the action for $C\rtimes_\alpha H$. In the proposed map $\Phi(aF^\times,\sigma)=[m_a\circ\sigma]$, changing $a$ by a factor in $F^\times$ scales the representative by that factor. Moreover $(m_a\circ\sigma)\circ(m_b\circ\tau)=m_{a\sigma(b)}\circ(\sigma\circ\tau)$, by the conjugation formula. Hence $\Phi$ is well defined and preserves the semidirect product law. [F2, F3, F4, F5, F8, step 1.1, step 2.2]

4.1 The factorization of $S$ gives surjectivity of $\Phi$. If $[m_a\circ\sigma]=[m_b\circ\tau]$, then $m_a\circ\sigma=c(m_b\circ\tau)$ for some $c\in F^\times$. Evaluating at $1$ gives $a=cb$, and canceling multiplication by $a$ gives $\sigma=\tau$. This proves injectivity and the isomorphism. The two possible automorphisms give the disjoint sets $T$ and $T[\sigma_q]$. For $S=m_a\circ\sigma_q$ in the latter case, additivity follows from $F$-linearity, and $S(bx)=a\sigma_q(b)\sigma_q(x)=\sigma_q(b)S(x)$. Because the multiplication maps commute, conjugation by $m_a$ fixes $m_{\sigma_q(b)}$, so conjugation by $S$ sends $m_b$ to $m_{\sigma_q(b)}$. [F1, F2, F3, F5, F8, step 1.1, step 2.2, step 3.1, step 3.2]

5.1 Since $F$ and $E$ are finite, their subsets $F^\times$ and $E^\times$ are finite. In each field the zero singleton and the group of nonzero elements form a disjoint partition. Adding the cardinalities of the two parts gives $|F^\times|=q-1$ and $|E^\times|=q^2-1$. The finite coset partition lemma for $F^\times\le E^\times$ gives that $C$ is finite and $[E^\times:F^\times]=|C|$. Lagrange's theorem then gives $q^2-1=|C|(q-1)$. As $0\ne1$ in $F$, we have $q\ge2$, and division gives $|C|=q+1$. The isomorphism identifies the normalizer bijectively with the pairs in $C\times H$. The product rule and $|H|=2$ give $|N_G(T)|=2(q+1)$, completing the normalizer description. [F1, F3, F6, F7, step 1.1, step 2.2, step 4.1] ∎


## Quaternion orders and completed lattices

[Open item](item-def-author-24fda87362bc-quaternion-orders-and-lattice-completions) · level 1


### Definition

In the rational Hamilton algebra $B=B(\mathbb Q)$, a full integral lattice $L$ is the set of all integer linear combinations of a rational basis $b_1,\ldots,b_4$ of $B$. A rational basis means every element of $B$ has a unique expression as a rational linear combination of these four elements. An order $O$ in $B$ is a full integral lattice that is a unital subring of $B$, meaning it contains $1$ and is closed under addition, additive inverses and multiplication.

For a prime $\ell$, write $B_\ell=B(\mathbb Q_\ell)$, with $B$ embedded by the coefficient inclusion $\mathbb Q\subseteq\mathbb Q_\ell$. The completion $L_\ell$ of $L$ at $\ell$ is the set of $\mathbb Z_\ell$-linear combinations of $b_1,\ldots,b_4$ in $B_\ell$, or equivalently the image of $L\otimes_{\mathbb Z}\mathbb Z_\ell$ under $b\otimes t\mapsto tb$. In this tensor product, $L$ has the right action $b\cdot r=rb$ by integer scaling, and $\mathbb Z_\ell$ has the left action $r\cdot t=rt$ by multiplication by the embedded integer $r$, for $r\in\mathbb Z$. For the order $O$ write $O_\ell$ for this completion.

### Justification

The quaternion coordinates and multiplication come from [def-author-24fda87362bc-hamilton-algebra-and-reduced-norm](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm). Rational basis coordinates restrict to unique integer coordinates on $L$, giving the free module basis of [math:def-free-module-on-a-set-and-standard-basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis). The four standard vectors exhibit a full lattice when spanned over $\mathbb Z$, and their multiplication table makes that lattice an order by [math:def-subring](https://alphabetamath.cc/item/def-subring).

Let $e=(1,i,j,k)$ and $b=(b_1,\ldots,b_4)$. The rational coordinate matrix $P$ from $b$ to $e$ and the reverse matrix $Q$ satisfy $PQ=QP=I$ by [math:thm-change-of-basis-matrices-are-inverses](https://alphabetamath.cc/item/thm-change-of-basis-matrices-are-inverses). By [math:def-matrix-product-and-identity-matrix](https://alphabetamath.cc/item/def-matrix-product-and-identity-matrix), the product entries are $(PQ)_{ab}=\sum_{j=1}^4 P_{aj}Q_{jb}$ and $(QP)_{ab}=\sum_{j=1}^4 Q_{aj}P_{jb}$, and $I$ has diagonal entries $1$ and off-diagonal entries $0$. The field inclusion $\mathbb Q\subseteq\mathbb Q_\ell$ from [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation) preserves these sums, products, $0$ and $1$, so $PQ=QP=I$ also holds over $\mathbb Q_\ell$. The columns of $P$ are the standard coordinates of the $b_i$, so $P$ sends a column of local coefficients to the standard coordinates of the corresponding linear combination of the $b_i$. Its inverse $Q$ shows that the $b_i$ form a basis over $\mathbb Q_\ell$. A second integer basis of $L$ lies in the integer span of the first and conversely, giving the same local span because $\mathbb Z\subseteq\mathbb Z_\ell$.

The two integer actions satisfy the right and left module axioms of [math:def-left-and-right-modules](https://alphabetamath.cc/item/def-left-and-right-modules) by distributivity, scalar associativity and the action of $1$. The rule $(b',t)\mapsto tb'$ is additive in both variables by distributivity and integer-balanced since $t(b'\cdot r)=(r\cdot t)b'$. Applied to these $\mathbb Z$-modules and the additive group of $B_\ell$, [math:thm-universal-property-of-module-tensor-products](https://alphabetamath.cc/item/thm-universal-property-of-module-tensor-products) gives a unique additive map sending $b'\otimes t$ to $tb'$. The defining relations in [math:def-tensor-product-of-modules-by-generators-and-relations](https://alphabetamath.cc/item/def-tensor-product-of-modules-by-generators-and-relations) describe the inverse on its image. If $b'=\sum_i n_i b_i$ with $n_i\in\mathbb Z$, the same relations give $b'\otimes t=\sum_i b_i\otimes(n_i t)$. Combining terms with the same $b_i$ expresses every tensor as $\sum_i b_i\otimes t_i$. Thus the image is the local span, and uniqueness of the $b$-coordinates makes $\sum_i t_i b_i\mapsto\sum_i b_i\otimes t_i$ the inverse on that span.

For $u=e$ or $u=b$, write $[x]_{u,j}$ for the $j$th coordinate of $x$ in that basis and set $d_u(x,y)=\max_{1\le j\le4}|[x]_{u,j}-[y]_{u,j}|_\ell$. The extended absolute value on $\mathbb Q_\ell$ is multiplicative and satisfies the strong triangle inequality by [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field). Thus $d_u$ is a metric in the sense of [math:def-metric-space](https://alphabetamath.cc/item/def-metric-space). Separation and symmetry follow coordinatewise, and taking the maximum of the coordinate triangle inequalities gives $d_u(x,z)\le d_u(x,y)+d_u(y,z)$. For either coordinate matrix $A=P$ or $A=Q$, take $C_A=1+\max_{i,j}|a_{ij}|_\ell$. Applying multiplicativity and the strong triangle inequality to each entry $(Aw)_i=\sum_{j=1}^4 a_{ij}w_j$ gives
$$\max_i |(Aw)_i|_\ell\le C_A\max_j|w_j|_\ell.$$
Applying this to coordinate differences gives $d_e\le C_P d_b$ and $d_b\le C_Q d_e$. The open ball $B_{d_u}(x,r)$ consists of the points $y$ with $d_u(x,y)<r$, for $r>0$, by [math:def-metric-ball](https://alphabetamath.cc/item/def-metric-ball). The comparisons give $B_{d_b}(x,r/C_P)\subseteq B_{d_e}(x,r)$ and $B_{d_e}(x,r/C_Q)\subseteq B_{d_b}(x,r)$. Thus the criteria for an open set in [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology) agree for the two metrics. The standard quaternion coordinate topology is the metric topology of $d_e$.

By [math:def-metric-interior-closure-boundary](https://alphabetamath.cc/item/def-metric-interior-closure-boundary), a point is in the closure of $L$ exactly when every open ball around it meets $L$. For $x\in L_\ell$, set $t_j=[x]_{b,j}\in\mathbb Z_\ell$. Let $a_{j,n}$ be the representative in $\{0,\ldots,\ell^n-1\}$ of the residue of $t_j$ modulo $\ell^n$. For $m\ge n$, the lifts $a_{j,m}$ and $a_{j,n}$ differ by a multiple of $\ell^n$, so their distance is at most $\ell^{-n}$ by the rational absolute value formula. Step 1.2 of [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp) constructs the canonical embedding by taking the limit of these lifts in $\mathbb Q_\ell$. For any $r>0$, metric convergence in [math:def-metric-convergence](https://alphabetamath.cc/item/def-metric-convergence) gives an index $N_j$ for each $j$ such that $|a_{j,n}-t_j|_\ell<r$ for all $n\ge N_j$. Taking $n\ge\max_{1\le j\le 4}N_j$ gives $\sum_{j=1}^4 a_{j,n}b_j\in L$ at $d_b$-distance less than $r$ from $x$. Conversely, if $x\notin L_\ell$, some coordinate $[x]_{b,j}$ lies outside $\mathbb Z_\ell$, the closed unit ball of [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation). For $d_b(x,y)<1$, if $[y]_{b,j}$ were in the unit ball, the strong triangle inequality would give $|[x]_{b,j}|_\ell\le\max(|[y]_{b,j}|_\ell,|[x]_{b,j}-[y]_{b,j}|_\ell)\le1$. Thus the open $d_b$-ball of radius $1$ around $x$ is disjoint from $L_\ell$, hence also from $L$. This establishes that $L_\ell$ is the closure of $L$ for the standard quaternion coordinate topology.

The products of basis vectors of $O$ belong to $O$. Expanding products over $\mathbb Z_\ell$ therefore gives $O_\ell O_\ell\subseteq O_\ell$, and $1\in O\subseteq O_\ell$. The local span is closed under addition and additive inverses as well, so $O_\ell$ is a unital subring.


## Integral splitting of the Hurwitz order at odd primes

[Open item](item-thm-hurwitz-integral-splitting-at-odd-primes) · level 2


### Statement

Let $\ell>2$ be a prime, so its only positive divisors are $1$ and $\ell$.

Let $B=\mathbb Q+\mathbb Qi+\mathbb Qj+\mathbb Qk$ be the rational Hamilton algebra with basis $1,i,j,k$ and $i^2=j^2=-1$, $ij=k=-ji$. Let $O=\mathbb Z+\mathbb Zi+\mathbb Zj+\mathbb Zw$ be its maximal Hurwitz order, where $w=(-1+i+j+k)/2$. An order is a subring with the same identity, equal to the integer span of finitely many elements and with rational span $B$. Maximality is with respect to inclusion.

Write $K=\mathbb Q_\ell$ for the completion of the rationals in the metric given off the diagonal by $d_\ell(x,y)=\ell^{-v_\ell(x-y)}$, where $v_\ell$ counts the exponent of $\ell$ in the numerator minus that in the denominator. Let $R=\mathbb Z_\ell\subseteq K$ be the ring of compatible residue classes modulo the powers of $\ell$, with arithmetic in each component. Compatibility means that each component reduces to the preceding one. Let $F=\mathbb F_\ell=\mathbb Z/\ell\mathbb Z$ be the field of integer residues modulo $\ell$.

In $B_K=B\otimes_{\mathbb Q}K$ and $O_R=O\otimes_{\mathbb Z}R$, the tensor products extend the original scalars to $K$ and $R$, respectively. The generating symbols $x\otimes s$ are additive in both entries and satisfy $cx\otimes s=x\otimes cs$ for each original scalar $c$. Their multiplication satisfies $(x\otimes s)(y\otimes t)=xy\otimes st$.

For a commutative ring $S$, $M_2(S)$ denotes the algebra of two-by-two matrices with entries in $S$, with entrywise addition, row-by-column multiplication and scalars acting as scalar matrices. An algebra isomorphism is a bijection preserving addition, multiplication, the identity and the scalar action.

There is a $K$-algebra isomorphism $\Phi:B_K\longrightarrow M_2(K)$ carrying the natural image of $O_R$ onto $M_2(R)$. The resulting entrywise reduction induces an $F$-algebra isomorphism $\bar\Phi:O/\ell O\longrightarrow M_2(F)$, where $O/\ell O$ is the ring of cosets modulo the ideal $\ell O=\{\ell x:x\in O\}$. The ideal is an additive subgroup closed under left and right multiplication by elements of $O$. For each $x=x_0+x_1i+x_2j+x_3k\in O$, its integer reduced norm $N(x)=x_0^2+x_1^2+x_2^2+x_3^2$ satisfies $\det\bar\Phi(x+\ell O)=N(x)\bmod\ell$, using $\det\begin{pmatrix}a&b\\c&d\end{pmatrix}=ad-bc$.

### Statement references

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure)

[math:def-subring](https://alphabetamath.cc/item/def-subring)

[math:def-quaternions](https://alphabetamath.cc/item/def-quaternions)

[math:def-free-module-on-a-set-and-standard-basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis)

[math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)

[math:lem-p-adic-valuation-on-q](https://alphabetamath.cc/item/lem-p-adic-valuation-on-q)

[math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals)

[math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)

[math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes)

[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)

[math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)

[math:thm-integers-modulo-n-basic-algebra](https://alphabetamath.cc/item/thm-integers-modulo-n-basic-algebra)

[math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:def-tensor-product-of-modules-by-generators-and-relations](https://alphabetamath.cc/item/def-tensor-product-of-modules-by-generators-and-relations)

[math:thm-tensor-product-of-algebras-over-a-commutative-ring](https://alphabetamath.cc/item/thm-tensor-product-of-algebras-over-a-commutative-ring)

[math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)

[math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring)

[math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)

[math:def-matrices-over-a-commutative-ring](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring)

[math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)

[math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring)

[math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)

### Facts & Assumptions

[F1] The rational Hamilton multiplication table is given by $i^2=j^2=-1$ and $ij=k=-ji$, with coefficients commuting with $1,i,j,k$. The order $O$ is closed under products and has integer basis $1,i,j,w$. A basis gives a unique linear expansion. Both $1,i,j,k$ and $1,i,j,w$ are rational bases of $B$, and $N(x)$ is integral for $x\in O$. [thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure) [math:def-quaternions](https://alphabetamath.cc/item/def-quaternions) [math:def-free-module-on-a-set-and-standard-basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis) [math:def-subring](https://alphabetamath.cc/item/def-subring)

[F2] Integer residue classes are equal exactly when their representatives differ by a multiple of the modulus. Their sums and products are those of representatives reduced modulo that modulus. For $R$ these operations are taken componentwise. The completion field $K$ contains $\mathbb Q$ and is canonically the fraction field of $R$, with the integer $n$ mapping to its compatible residue classes in $R$. [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers) [math:lem-p-adic-valuation-on-q](https://alphabetamath.cc/item/lem-p-adic-valuation-on-q) [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals) [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field) [math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes) [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp) [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n) [math:thm-integers-modulo-n-basic-algebra](https://alphabetamath.cc/item/thm-integers-modulo-n-basic-algebra) [math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)

[F3] Modulo a prime the residue ring is a field, a commutative ring in which $0\ne 1$ and each nonzero element is invertible. Integer arithmetic is ordered ring arithmetic, and division by a positive integer $d$ gives a unique remainder in $\{0,\ldots,d-1\}$. [math:def-prime](https://alphabetamath.cc/item/def-prime) [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field) [math:def-field](https://alphabetamath.cc/item/def-field) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z) [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring)

[F4] The number of elements of a finite set is the length of an enumeration without repetitions. A product of two finite sets has size the product of their sizes. A function from a larger finite set to a smaller one has two distinct inputs with the same value. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule) [math:thm-the-strong-pigeonhole-principle](https://alphabetamath.cc/item/thm-the-strong-pigeonhole-principle)

[F5] If $f\in R[X]$ and $t\in R$ satisfy $f(t)\in\ell R$ and $f'(t)\notin\ell R$, Hensel's simple-root lifting theorem gives $a\in R$ with $f(a)=0$ and $a-t\in\ell R$. Here $R[X]$ consists of finite sums of powers of the formal variable $X$ with coefficients in $R$. The formal derivative sends $cX^n$ to $ncX^{n-1}$ for $n>0$, sends constants to zero and acts termwise. For $t\in R$, evaluation sends $\sum_i c_iX^i$ to $\sum_i c_it^i$ in $R$ using the identity coefficient map. [math:cor-p-adic-simple-root-lifting](https://alphabetamath.cc/item/cor-p-adic-simple-root-lifting) [math:def-polynomial-ring-over-a-commutative-ring](https://alphabetamath.cc/item/def-polynomial-ring-over-a-commutative-ring) [math:def-formal-derivative-of-a-polynomial](https://alphabetamath.cc/item/def-formal-derivative-of-a-polynomial) [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring) [math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism) [math:def-polynomial-evaluation-and-root](https://alphabetamath.cc/item/def-polynomial-evaluation-and-root)

[F6] Every tensor is a sum of elementary tensors, subject to the additive and balancing relations in the Statement. For algebras over the commutative base ring, products are taken factor by factor and $1\otimes1$ is the identity. The second tensor factor supplies the extended scalars. [math:def-tensor-product-of-modules-by-generators-and-relations](https://alphabetamath.cc/item/def-tensor-product-of-modules-by-generators-and-relations) [math:thm-tensor-product-of-algebras-over-a-commutative-ring](https://alphabetamath.cc/item/thm-tensor-product-of-algebras-over-a-commutative-ring) [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring) [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring)

[F7] Row-by-column multiplication is associative, unital and distributes over addition on both sides. Scalar matrices commute with every matrix and multiply each entry by the scalar. The determinant of a two-by-two matrix is its diagonal product minus its off-diagonal product. [math:def-matrices-over-a-commutative-ring](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring) [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose) [math:thm-ring-matrix-arithmetic-laws](https://alphabetamath.cc/item/thm-ring-matrix-arithmetic-laws) [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix) [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring) [math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)

[F8] The quotient by a two-sided ideal uses the sum and product of representatives as representatives of the result. The map to cosets preserves addition, multiplication and identity, and sends precisely the elements of the ideal to zero. [math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring) [math:prop-canonical-quotient-ring-map](https://alphabetamath.cc/item/prop-canonical-quotient-ring-map)

### Proof

**Given:** The rational Hamilton algebra $B$, its Hurwitz order $O$, and an odd prime $\ell$.

**Goal:** Construct the integral splitting, identify its reduction and prove the determinant formula.

1.1 Projection $\rho:R\to F$ to the first component preserves the ring operations. It is onto, since any integer representative of a residue defines a compatible tuple. If $x=(x_n)$ projects to zero, each representative of $x_{n+1}$ is divisible by $\ell$. Divide such a representative by $\ell$ and take its class modulo $\ell^n$ to obtain $y_n$. This is independent of the representative because a change by a multiple of $\ell^{n+1}$ changes the quotient by a multiple of $\ell^n$. Compatibility of the $x_n$ gives compatibility of the $y_n$ by the same division. At level $n$ the class $\ell y_n$ equals the reduction of $x_{n+1}$ and hence equals $x_n$. Thus $x=\ell y$ for $y=(y_n)\in R$. Conversely every multiple of $\ell$ projects to zero, so $\ker\rho=\ell R$. [F2, F3, F8]

1.2 Since $\ell>2$ is prime, $2$ does not divide it, so $\ell$ is odd. Each $\ell^n$ is odd, since a product of odd integers is odd by $(2h+1)(2j+1)=2(2hj+h+j)+1$. The residue of $(\ell^n+1)/2$ is therefore an inverse of $2$ modulo $\ell^n$. Reduction of the inverse at level $n+1$ gives an inverse at level $n$, which must be the same by uniqueness of inverses. These residues give $2^{-1}\in R$. [given, F2, F3]

2.1 Set $m=(\ell-1)/2$ and let $E=\{0,\ldots,m\}$, read as distinct residues in $F$. Squaring is injective on $E$, meaning two inputs with the same square must coincide. Indeed, $u^2=v^2$ in $F$ implies $(u-v)(u+v)=0$, so $u=v$ or $u=-v$ in $F$ by invertibility of each nonzero field element. In the latter case the sum of the integer representatives is in $[0,\ell-1]$ and divisible by $\ell$, so both are zero. Now $E\times\{0,1\}$ has $2(m+1)=\ell+1$ elements, whereas $F$ has $\ell$ by uniqueness of remainders. Map $(u,0)$ to $u^2$ and $(u,1)$ to $-1-u^2$. Each branch is injective, so a collision given by the pigeonhole principle supplies $a_0,b_0\in F$ with $a_0^2=-1-b_0^2$. Since $-1\ne0$, at least one of $a_0,b_0$ is nonzero. Interchange the two if necessary so that $a_0\ne0$. [F2, F3, F4, step 1.2]

2.2 For $O_R$ the basis $1,i,j,w$ extends to an $R$-basis, and for $B_K$ it extends to a $K$-basis. Indeed, for either original basis $(e_h)$, send $x\otimes s$ with $x=\sum_h c_he_h$ to the tuple $(c_hs)_h$. This respects addition and balancing, and the inverse sends $(s_h)_h$ to $\sum_h e_h\otimes s_h$ by those same relations. The induced map $O_R\to B_K$ is therefore coefficientwise inclusion in this basis and preserves products by the elementary tensor multiplication rule. We identify $O_R$ with its image. Since $k=2w+1-i-j$ and $2$ is invertible in $R$, the basis can be changed to $1,i,j,k$ by substituting either formula for $w$ or $k$. In this basis $O_R$ is exactly the elements of $B_K$ with all four coordinates in $R$. [F1, F2, F6, step 1.2]

3.1 Take integers $A,B_0$ representing $a_0,b_0$ and view them in $R$. For $f(X)=X^2+B_0^2+1$, one has $\rho(f(A))=0$ and $\rho(f'(A))=2a_0\ne0$ in $F$, since $\ell>2$. By step 1.1 these are the two tests for simple-root lifting. Obtain $a\in R$ with $f(a)=0$, and put $b=B_0\in R$. Then $a^2+b^2=-1$. [F2, F3, F5, step 1.1, step 2.1]

4.1 Let $I$ be the identity matrix and put $U=\begin{pmatrix}0&1\\-1&0\end{pmatrix}$ and $V=\begin{pmatrix}a&b\\b&-a\end{pmatrix}$. Multiplication gives $U^2=-I$, $V^2=(a^2+b^2)I=-I$, and $UV=\begin{pmatrix}b&-a\\-a&-b\end{pmatrix}=-VU$. Every product of $I,U,V,UV$ reduces with these relations to the same signed basis product as for $1,i,j,k$. Indeed, the relations move each $U$ to the left of each $V$ and reduce each square to $-I$. Thus the $K$-linear map $\Phi$ sending $1,i,j,k$ to $I,U,V,UV$ preserves multiplication by expansion in the basis. It preserves the identity and sends scalars to scalar matrices. [construct, F1, F6, F7, step 3.1, step 2.2]

5.1 For coordinates $x_0,x_1,x_2,x_3$, put $d=ax_2+bx_3$ and $e=bx_2-ax_3$. The image matrix has diagonal entries $x_0+d,x_0-d$ and off-diagonal entries $x_1+e,-x_1+e$, in upper then lower order. Conversely a matrix $(m_{st})$ determines $x_0=(m_{11}+m_{22})/2$, $x_1=(m_{12}-m_{21})/2$, $d=(m_{11}-m_{22})/2$ and $e=(m_{12}+m_{21})/2$. The column with entries $d,e$ equals $V$ times the column with entries $x_2,x_3$, so $-V$ recovers the last two coordinates because $V^2=-I$. All the inverse formulas work over both $K$ and $R$, since $a,b,2^{-1}\in R$. Hence $\Phi$ is bijective and takes $O_R$ onto $M_2(R)$. [F6, F7, step 1.2, step 2.2, step 4.1]

6.1 The determinant of the displayed image is $(x_0+d)(x_0-d)-(x_1+e)(-x_1+e)=x_0^2+x_1^2-d^2-e^2$. Expanding the squares gives $d^2+e^2=(a^2+b^2)(x_2^2+x_3^2)$, since the mixed terms cancel. By step 3.1, the determinant is therefore $x_0^2+x_1^2+x_2^2+x_3^2$, which is $N(x)$ for $x\in O$. [F1, F7, step 3.1, step 5.1]

7.1 The subset $\ell O$ is a two-sided ideal because integer scalars are central and $O$ is a ring. Reducing the matrix entries by $\rho$ gives a surjective ring map $M_2(R)\to M_2(F)$ whose elements mapping to zero are precisely $\ell M_2(R)$ by step 1.1. The restriction of $\Phi$ carries $\ell O_R$ onto $\ell M_2(R)$ since it respects scalars and is onto $M_2(R)$. The map $O\to O_R/\ell O_R$ takes the coefficients in $1,i,j,w$ to their residues. Every residue coefficient has an integer representative, and an integer coefficient maps to zero precisely when divisible by $\ell$, so this map is surjective with kernel $\ell O$. Consequently the composite from $O$ to $M_2(F)$ is onto and two inputs have the same image exactly when their difference lies in $\ell O$. It induces the stated bijection on cosets, preserving the ring operations and the $F$-scalar action given by integer representatives. The determinant is a polynomial in the entries with integer coefficients, so its value commutes with entrywise reduction. Step 6.1 now gives the stated norm identity on the quotient and completes the compatible splitting. [F1, F2, F6, F7, F8, step 1.1, step 2.2, step 5.1, step 6.1, discharge-construct] ∎

### Source notes

Voight's discriminant example gives the field splitting through ramification, and his split maximal-order case describes the integral matrix order. The proof here specializes the reduction and root-lifting method to the equation for two squares, then constructs the integral isomorphism and computes its reduction directly. [Quaternion algebras over global fields](https://link.springer.com/chapter/10.1007/978-3-030-56694-4_14) [Discriminants](https://link.springer.com/chapter/10.1007/978-3-030-56694-4_15) [Ternary quadratic forms over local fields](https://link.springer.com/chapter/10.1007/978-3-030-56694-4_12)


## Norms of quaternion lattices and their local generators

[Open item](item-lem-author-24fda87362bc-quaternion-lattice-norms-and-local-generators) · level 2


### Statement

Let $L$ be a full integral lattice and $O$ an order in the rational Hamilton algebra $B$. Let $\ell$ be a prime. Use $A$ for the set of finite integer linear combinations of reduced norms of elements of $L$, and $A_\ell$ for the set of finite $\mathbb Z_\ell$-linear combinations of reduced norms of elements of $L_\ell$ in $B_\ell$. For a subset of $\mathbb Q$, its $\mathbb Z_\ell$-span inside $\mathbb Q_\ell$ is denoted by multiplication by $\mathbb Z_\ell$.

There is a unique positive rational $d$ with $A=d\mathbb Z$, and $A_\ell=A\mathbb Z_\ell$. Every element of $O$ has integral reduced norm, and every element of $O_\ell$ has reduced norm in $\mathbb Z_\ell$. If $L=xO$ with $x\in B^\times$, then $A=N(x)\mathbb Z$. If $L_\ell=x_\ell O_\ell$ with $x_\ell\in B_\ell^\times$, then $A_\ell=N(x_\ell)\mathbb Z_\ell$ and $v_\ell(d)=v_\ell(N(x_\ell))$.

### Facts & Assumptions

[F1] In the Hamilton coordinates of [def-author-24fda87362bc-hamilton-algebra-and-reduced-norm](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm), the reduced norm is the sum of the four squares, $N(1)=1$, $N(xy)=N(x)N(y)$ and $N$ is nonzero on units and positive on nonzero rational quaternions.

[F2] A full integral lattice has a rational basis that freely generates it over $\mathbb Z$ and generates its local completion over $\mathbb Z_\ell$. An order and its local completion contain $1$ and are closed under multiplication by [def-author-24fda87362bc-quaternion-orders-and-lattice-completions](item-def-author-24fda87362bc-quaternion-orders-and-lattice-completions).

[F3] By [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation), a prime is greater than $1$, the field $\mathbb Q_\ell$ contains $\mathbb Q$, and $\mathbb Z_\ell$ is a subring containing the embedded integers. Nonzero elements of $\mathbb Q_\ell$ have integer valuation, additive on products. An element $z\in\mathbb Q_\ell$ belongs to $\mathbb Z_\ell$ exactly when $v_\ell(z)\ge0$, with $v_\ell(0)=+\infty$. A scalar in $\mathbb Z_\ell$ is a unit exactly when its valuation is zero. The valuation on nonzero rationals is the numerator exponent minus the denominator exponent. For a nonzero integer $a$, the exponent is the greatest $k\ge0$ such that $\ell^k$ divides $a$.

[F4] For two integers, at least one nonzero, their greatest common divisor is positive and divides both by [math:def-common-divisor-and-gcd](https://alphabetamath.cc/item/def-common-divisor-and-gcd). It is also an integer linear combination of them by [math:thm-bezout-identity](https://alphabetamath.cc/item/thm-bezout-identity). An integer divides another when the latter is an integer multiple of the former by [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z).

[F5] Every positive integer has a factorization into primes that is unique up to order by [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic).

[F6] The integers form a totally ordered ring, so adding an integer to both sides of a strict inequality preserves that inequality and a product of positive integers is positive ([math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)). Every nonempty set of integers with an integer lower bound has a least member ([math:lem-int-bounded-above-has-greatest](https://alphabetamath.cc/item/lem-int-bounded-above-has-greatest)).

[F7] A property of natural numbers holds for every natural number if it holds at zero and passes from each number to its successor ([math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)).

[F8] Every rational has a representative with positive denominator, and in such a representative the rational is positive exactly when its numerator is positive ([math:def-rat-order](https://alphabetamath.cc/item/def-rat-order)). The embedding $m\mapsto m/1$ of $\mathbb Z$ in $\mathbb Q$ is injective and preserves addition, multiplication and order ([math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)).

[F9] An integer $u$ divides $1$ exactly when $u=1$ or $u=-1$ ([math:lem-units-of-z](https://alphabetamath.cc/item/lem-units-of-z)).

[F10] The rationals form a commutative field, so every nonzero rational has a multiplicative inverse ([math:thm-rat-field](https://alphabetamath.cc/item/thm-rat-field)).

### Proof

**Given:** The lattices $L$ and $O$, a prime $\ell$, and the spans $A$ and $A_\ell$ in the statement. In the assertions on principal lattices assume the stated invertible generators exist.

**Goal:** Identify the two norm spans, establish integrality on orders, and compute the norm spans and valuation when generators are given.

1.1 Take an integer basis $b_1,\ldots,b_4$ of $L$ as in [F2]. Let $S$ consist of the $N(b_i)$ and the $N(b_i+b_j)$ for $i<j$. For coefficients $t_i$ in either $\mathbb Z$ or $\mathbb Z_\ell$, expanding the four squares gives $N(\sum_i t_i b_i)=\sum_i t_i^2N(b_i)+\sum_{i<j}t_i t_j\bigl(N(b_i+b_j)-N(b_i)-N(b_j)\bigr)$. Every element of $S$ is already a norm from $L$, which embeds in $L_\ell$. Hence $S$ generates both $A$ over $\mathbb Z$ and $A_\ell$ over $\mathbb Z_\ell$, and $A_\ell=A\mathbb Z_\ell$. [F1, F2, F3, given]

1.2 Choose $C$ to be the product of the positive denominators of the four rational coordinates of every vector in an integer basis of $O$. By [F2], elements of $O_\ell$ then have coordinates in $C^{-1}\mathbb Z_\ell$. For each $u\in O_\ell$, the four-square formula therefore gives $C^2N(u)\in\mathbb Z_\ell$. The set of valuations of nonzero norms of elements of $O_\ell$ is a subset of the integers containing $0$, since $1\in O_\ell$ and $N(1)=1$. By additivity of valuation it is bounded below by $-2v_\ell(C)$. By [F6] let $m$ be its least member and take $u\in O_\ell$ with $v_\ell(N(u))=m$. Then $u^2\in O_\ell$ and $N(u^2)=N(u)^2\ne0$. Its valuation is $m+m$, which would be strictly below $m$ if $m<0$. Thus $m\ge0$. Every nonzero norm from $O_\ell$ has valuation at least $m\ge0$ and therefore belongs to $\mathbb Z_\ell$ by [F3], and the zero norm belongs to that ring as well. [F1, F2, F3, F6, F8, F10, given]

2.1 For $u\in O$, Step 1.2 gives nonnegative valuation of $N(u)$ at every prime. If $N(u)=0$, it is integral. Otherwise by [F8] write $N(u)=a/b$ with nonzero integers $a,b$ and $b>0$. By [F4], $h=\gcd(a,b)>0$ divides both $a$ and $b$, and $ar+bs=h$ for integers $r,s$. Write $a=ha'$ and $b=hb'$ with $a',b'\in\mathbb Z$. Factoring $h$ from $ar+bs=h$ gives $h(a'r+b's)=h$ by [F6]. Multiplying by $h^{-1}$ in $\mathbb Q$ gives $a'r+b's=1$, which holds in $\mathbb Z$ by [F8]. Cancelling $h$ in the fraction gives $a/b=a'/b'$ by [F10]. The quotient $b/h$ is positive by the positive numerator and denominator criterion in [F8], so $b'>0$ in $\mathbb Z$ as well. If $b'\ne1$, [F5] gives a nonempty prime factorization of $b'$. Take a prime $p$ in this factorization, so $p\mid b'$. If $p$ also divided $a'$, then $a'=pk$ and $b'=pj$ for integers $k,j$ by [F4]. Distributivity in [F6] gives $1=a'r+b's=p(kr+js)$, so $p$ divides $1$. This is impossible by [F9] because $p>1$ by [F3]. Thus $v_p(a')=0$ and $v_p(b')\ge1$, contradicting the nonnegative valuation of $N(u)=a'/b'$ by [F3]. Hence $b'=1$ and $N(u)\in\mathbb Z$. [F3, F4, F5, F6, F8, F9, F10, step 1.2, given]

2.2 Let $D$ be the product of the positive denominators for the finitely many elements of $S$, so every element of $DS$ is an integer. The integers in $DS$ include a nonzero one because $N(b_1)>0$. List the entries of $DS$ with one nonzero entry first. Apply [F7] with the first entry as the base case and one further entry added at each stage. For the first entry $s_1\ne0$, take $c=s_1$ if $s_1>0$ and $c=-s_1$ if $s_1<0$. Adding $-s_1$ to $s_1<0$ gives $-s_1>0$ by [F6]. In the second case $c=(-1)s_1$ and $s_1=(-1)c$, so each is an integer multiple of the other and the two spans agree. For the current positive generator $c$ and the next entry $s$, take $h=\gcd(c,s)$. By [F4], $h$ is an integer linear combination of $c$ and $s$, and $c$ and $s$ are integer multiples of $h$. Thus $c\mathbb Z+s\mathbb Z=h\mathbb Z$. This gives a positive generator for the enlarged part of the list, which completes the induction. Thus $DA=g\mathbb Z$ for some positive integer $g$. Multiplying by $D^{-1}$ in $\mathbb Q$ gives $A=d\mathbb Z$ for $d=g/D$, positive by [F8]. If $e$ is another positive rational generator, write $e=g'/D'$ with $g',D'>0$ by [F8]. The equal spans give integers $m,n$ with $d=me$ and $e=nd$. By [F10] the equalities give $m=d/e=gD'/(Dg')$ and $n=e/d=g'D/(D'g)$. These quotients have positive numerators and denominators by [F6], so $m,n$ are positive integers by [F8]. Since $d=mnd$ with $d\ne0$, multiplying by $d^{-1}$ in $\mathbb Q$ gives $mn=1$ there by [F10]. Injectivity in [F8] gives $mn=1$ in $\mathbb Z$. By [F9] the two positive integer divisors $m,n$ of $1$ both equal $1$, so $d=e$. [F1, F4, F6, F7, F8, F9, F10, step 1.1]

3.1 If $L=xO$, all norms from $L$ belong to $N(x)\mathbb Z$ by multiplicativity and Step 2.1. The norm $N(x)$ itself occurs by taking $x\cdot1$. This gives $A=N(x)\mathbb Z$. If $L_\ell=x_\ell O_\ell$, the same two inclusions give $A_\ell=N(x_\ell)\mathbb Z_\ell$, since each $N(x_\ell u)$ is $N(x_\ell)N(u)$ with $N(u)\in\mathbb Z_\ell$ and $u=1$ supplies $N(x_\ell)$. [F1, F2, step 1.2, step 2.1, given]

4.1 By Steps 1.1 and 2.2 the local span is also $d\mathbb Z_\ell$. If a local generator is given, put $a=N(x_\ell)$. Since $x_\ell$ is a unit, $a\ne0$ by [F1]. By Step 3.1 the two spans $d\mathbb Z_\ell$ and $a\mathbb Z_\ell$ coincide. Thus $d=aq$ and $a=dr$ for some $q,r\in\mathbb Z_\ell$. Both $a$ and $d$ are nonzero in $\mathbb Q_\ell$, and division there gives $q=d/a$ and $r=a/d$. Hence $q$ is a unit with inverse $r$. The equality $d=aq$ and [F3] give $v_\ell(d)=v_\ell(a)+v_\ell(q)=v_\ell(N(x_\ell))$. Together the steps give the two spans, both integrality claims, and the formulas for principal lattices. [F1, F3, step 1.1, step 2.2, step 1.2, step 2.1, step 3.1] ∎


## Quaternion right ideals and their reduced norm

[Open item](item-def-quaternion-right-ideal-and-reduced-norm) · level 3


### Definition

Let $O$ be an order in the rational Hamilton algebra $B$, so $O$ is a unital subring and a full integral lattice. A right fractional $O$-ideal is a full integral lattice $I\subseteq B$ with $io\in I$ for every $i\in I$ and $o\in O$. It is integral if $I\subseteq O$, and principal if $I=xO=\{xo:o\in O\}$ for some $x\in B^\times$, where $B^\times$ denotes the elements with a two-sided inverse. A right ideal of the ring $O$ is an additive subgroup of $O$ stable under this right multiplication by $O$. Every integral right fractional ideal is a right ideal in this sense.

For a prime $\ell$ let $I_\ell$ and $O_\ell$ be the $\mathbb Z_\ell$-spans of $I$ and $O$ in $B_\ell=B(\mathbb Q_\ell)$. A right fractional $O_\ell$-ideal is the $\mathbb Z_\ell$-span of a $\mathbb Q_\ell$-basis of $B_\ell$, with the span required to be stable under right multiplication by $O_\ell$. It is integral if it is contained in $O_\ell$ and principal if it is $x_\ell O_\ell$ for some $x_\ell\in B_\ell^\times$. The fractional ideal $I$ is locally principal if $I_\ell$ is principal at every prime $\ell$.

The reduced norm ideal $\operatorname{nrd}(I)\subseteq\mathbb Q$ is the set of finite $\mathbb Z$-linear combinations of the reduced norms $N(y)$ for $y\in I$. A fractional ideal of $\mathbb Z$ here means a nonzero additive subgroup of $\mathbb Q$ closed under multiplication by integers and contained in $D^{-1}\mathbb Z$ for some positive integer $D$. The positive generator $d$ of $\operatorname{nrd}(I)=d\mathbb Z$ is also called the reduced norm of $I$. For a local right fractional ideal $J$, its reduced norm ideal is the $\mathbb Z_\ell$-span of the reduced norms of elements of $J$. It is of the form $a\mathbb Z_\ell$ for $a\in\mathbb Q_\ell^\times$, and its valuation is $v_\ell(a)$ with $v_\ell(\ell)=1$. The corresponding local norm ideal of $I_\ell$ equals $d\mathbb Z_\ell$. If $J=x_\ell O_\ell$ with $x_\ell$ invertible, its norm ideal is $N(x_\ell)\mathbb Z_\ell$ and has valuation $v_\ell(N(x_\ell))$. If $I=xO$ with $x$ invertible, its positive norm is $N(x)$. Integral ideals have positive integer norm.

### Justification

The full lattices and their completions are those of [def-author-24fda87362bc-quaternion-orders-and-lattice-completions](item-def-author-24fda87362bc-quaternion-orders-and-lattice-completions). Expressing a basis of $I$ in a basis of $O$ and clearing the finitely many rational denominators gives a positive integer $D$ with $DI\subseteq O$, as required for fractional scaling. As an integer span, $I$ contains $0$ and is closed under addition and additive inverses. For $I\subseteq O$, it is an additive subgroup of $O$ by [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup). The assumed stability under right multiplication by $O$ gives the remaining condition of [the right-ideal definition](https://alphabetamath.cc/item/def-left-right-and-two-sided-ideal). Multiplication in the Hamilton algebra of [def-author-24fda87362bc-hamilton-algebra-and-reduced-norm](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm) is bilinear. Expanding products of local coefficient combinations of basis vectors shows $I_\ell O_\ell\subseteq I_\ell$. If $I=xO$ then the local span is $xO_\ell$ because each rational left multiplication by $x$ extends by the same coordinate rule.

Apply [lem-author-24fda87362bc-quaternion-lattice-norms-and-local-generators](item-lem-author-24fda87362bc-quaternion-lattice-norms-and-local-generators) to $L=I$. The lemma gives $\operatorname{nrd}(I)=d\mathbb Z$ with $d>0$. This set contains $0$ and is closed under addition and additive inverses, so it is an additive subgroup of $\mathbb Q$ by [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup). It contains the nonzero element $d$, is stable under integer multiplication, and lies in $E^{-1}\mathbb Z$ for a positive integer $E$ clearing the denominator of $d$. Hence it is a fractional ideal of $\mathbb Z$. The same lemma identifies the local span with $d\mathbb Z_\ell$ and computes it for $I_\ell=x_\ell O_\ell$.

For a general $J$, take a $\mathbb Q_\ell$-basis whose $\mathbb Z_\ell$-span is $J$. This basis is a linearly independent spanning set by [math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis). The standard Hamilton basis $1,i,j,k$ has four elements. Hence the basis for $J$ is finite and has four elements by [math:thm-any-two-finite-bases-have-the-same-size](https://alphabetamath.cc/item/thm-any-two-finite-bases-have-the-same-size). Label them $b_1,\ldots,b_4$. For $t_i\in\mathbb Z_\ell$, expand the four coordinate squares of $\sum_i t_i b_i$ to obtain
$$N(\textstyle\sum_i t_i b_i)=\sum_i t_i^2 N(b_i)+\sum_{i<j}t_i t_j\bigl(N(b_i+b_j)-N(b_i)-N(b_j)\bigr).$$
Thus the norms of the basis vectors and their pairwise sums generate the local norm span. Each of these vectors belongs to the local span of the basis, so its norm is among the generators in the definition. Write $1=\sum_i c_i b_i$ with $c_i\in\mathbb Q_\ell$. Choose a nonnegative integer $n$ such that $n+v_\ell(c_i)\ge0$ for each nonzero $c_i$. By the valuation product law and $v_\ell(\ell)=1$, every $\ell^n c_i$ belongs to $\mathbb Z_\ell$. Thus $\ell^n1$ lies in $J$ and has nonzero norm $\ell^{2n}$. At least one listed norm is nonzero, since otherwise their span could not contain $\ell^{2n}$. By [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation), the valuations of these nonzero norms are totally ordered integers. Start with any nonzero listed norm. Compare it with the other nonzero norms in turn, replacing the current norm whenever the next one has smaller valuation. After each comparison the current norm has valuation at most those considered so far. The list is finite, so the last retained norm $a$ has least valuation. For any nonzero generator $s$ in the list, $v_\ell(s/a)=v_\ell(s)-v_\ell(a)\ge0$, so $s\in a\mathbb Z_\ell$. The zero generators also lie in $a\mathbb Z_\ell$. Thus $a$ generates the local span. For $J=x_\ell O_\ell$, the norms of elements of $O_\ell$ lie in $\mathbb Z_\ell$ by the lemma, and include $1$. The equality $N(x_\ell)N(x_\ell^{-1})=N(1)=1$ makes $N(x_\ell)$ nonzero. All norms from $J$ are multiples of $N(x_\ell)$ over $\mathbb Z_\ell$, and taking $1\in O_\ell$ gives the norm $N(x_\ell)$ itself. Any two nonzero scalars generating a local scalar ideal differ by a unit of $\mathbb Z_\ell$, since both ratios between the scalars lie in $\mathbb Z_\ell$. They have equal valuation by [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation). Thus a choice of quaternion generator does not affect the norm valuation. If $I=xO$, the lemma gives $d=N(x)$ since the rational reduced norm of an invertible element is positive. If $I\subseteq O$, each generating norm belongs to $\mathbb Z$ by the same lemma, so $d$ is a positive integer.

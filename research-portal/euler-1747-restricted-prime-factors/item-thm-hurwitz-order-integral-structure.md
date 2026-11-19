---
title: Integral structure of the Hurwitz order
status: published
research_item: thm-hurwitz-order-integral-structure
dependency_level: 1
sources:
  references:
    - title: "John Voight, Quaternion Algebras, chapter 11: The Hurwitz order"
      url: https://link.springer.com/chapter/10.1007/978-3-030-56694-4_11
      locator: §11.1, Lemma 11.1.2 and (11.1.3), and Exercise 11.1
      reading_limits: Read the basis formula, the proof of Lemma 11.1.2 and the
        closure exercise in the publisher's chapter. The ring closure and
        integer norm and trace are proved locally below.
---

## Prerequisites

- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-quaternions](https://alphabetamath.cc/item/def-quaternions)
- [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)
- [math:def-free-module-on-a-set-and-standard-basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis)
- [def-author-53081a7cb32d-order-in-a-rational-algebra](item-def-author-53081a7cb32d-order-in-a-rational-algebra)
- [math:lem-quaternion-conjugation-is-an-anti-involution](https://alphabetamath.cc/item/lem-quaternion-conjugation-is-an-anti-involution)
- [math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring)
- [math:def-subring](https://alphabetamath.cc/item/def-subring)
- [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound)
- [math:lem-int-bounded-above-has-greatest](https://alphabetamath.cc/item/lem-int-bounded-above-has-greatest)


## Statement

Let $B$ be the rational Hamilton algebra, the real quaternions with all coordinates restricted to rational numbers in the basis $1,i,j,k$ with $i^2=j^2=-1$ and $ij=k=-ji$. The rational scalars act by multiplication by scalar quaternions $q1$. For $x=x_0+x_1i+x_2j+x_3k$, quaternion conjugation is $\bar x=x_0-x_1i-x_2j-x_3k$, the reduced trace is $T(x)=2x_0$, and the reduced norm is $N(x)=x_0^2+x_1^2+x_2^2+x_3^2$.

Identify each integer $n\in\mathbb Z$ with the rational number $n/1$.

Put $w=(-1+i+j+k)/2$ and let $O=\mathbb Z+\mathbb Zi+\mathbb Zj+\mathbb Zw$, the set of integer linear combinations of $1,i,j,w$. This is a lattice in $B$, meaning the integer span of a rational basis. It is a maximal $\mathbb Z$-order. Here a $\mathbb Z$-order is a subring with the same identity as $B$, generated additively by finitely many elements and spanning $B$ by rational linear combinations. Maximality means that every $\mathbb Z$-order in $B$ containing $O$ equals $O$.

In the basis $1,i,j,k$ its coordinate set is $\mathbb Z^4\cup(\mathbb Z+\tfrac12)^4$, where $\mathbb Z+\tfrac12=\{n+\tfrac12:n\in\mathbb Z\}$. For each $x\in O$, both $T(x)$ and $N(x)$ are integers and $\bar x\in O$.

## Statement references

[Quaternion coordinates and operations](https://alphabetamath.cc/item/def-quaternions)

[The integers](https://alphabetamath.cc/item/def-integers)

[The embedding of integers into the rationals](https://alphabetamath.cc/item/lem-int-embeds-rat)

[Algebras and central scalars](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)

[Module bases and unique coefficients](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis)

[Orders in rational algebras](item-def-author-53081a7cb32d-order-in-a-rational-algebra)

## Facts & Assumptions

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

## Proof

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

## Source notes

The basis and the trace and parity reduction follow Voight, Lemma 11.1.2. Step 3.1 does the multiplication check posed in Exercise 11.1 using $w$, which differs from the generator in the exercise by $-1$. Steps 2.2, 3.2 and 4.1 obtain norm and trace integrality from bounded denominators of the norms in any given order. [John Voight, The Hurwitz order](https://link.springer.com/chapter/10.1007/978-3-030-56694-4_11)

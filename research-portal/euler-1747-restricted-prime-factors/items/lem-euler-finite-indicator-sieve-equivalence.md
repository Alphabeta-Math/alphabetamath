---
id: lem-euler-finite-indicator-sieve-equivalence
kind: lemma
title: Deleted progressions agree with the floor indicators
status: draft
domain: mathematics
deps:
  - math:thm-reals-field
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-nat-addition
  - math:lem-nat-embeds-int
  - def-euler-finite-certificate-indices
  - def-euler-prime-classes
  - alg-euler-finite-indicator-sieve
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-real-numbers
  - math:def-real-order
  - math:def-field
  - math:lem-integer-part
  - math:def-sum-over-a-finite-index-set
  - math:def-natural-numbers
  - math:def-finite-cardinality
  - math:def-set-difference-and-symmetric-difference
  - lem-euler-finite-indicator-factor-test
  - lem-invertible-linear-residue-progression
  - lem-finite-deletions-and-translated-support
  - lem-binary-products-and-avoidance
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - math:def-ring
  - math:def-nat-multiplication
  - math:def-indexed-family
  - math:def-cartesian-product
  - math:def-axiom-schema-of-separation
  - math:def-subset-and-proper-subset
  - math:def-ordered-pair
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-relation-domain-range-and-field
  - math:def-function
formulation_deps:
  - math:thm-reals-field
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:lem-nat-embeds-int
  - def-euler-finite-certificate-indices
  - def-euler-prime-classes
  - alg-euler-finite-indicator-sieve
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-real-numbers
  - math:def-real-order
  - math:def-field
  - math:lem-integer-part
  - math:def-sum-over-a-finite-index-set
  - math:def-natural-numbers
  - math:def-finite-cardinality
  - math:def-set-difference-and-symmetric-difference
  - math:def-nat-multiplication
  - math:def-indexed-family
argument_deps:
  - math:thm-reals-field
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-nat-addition
  - math:lem-nat-embeds-int
  - def-euler-finite-certificate-indices
  - def-euler-prime-classes
  - alg-euler-finite-indicator-sieve
  - lem-euler-finite-indicator-factor-test
  - lem-invertible-linear-residue-progression
  - lem-finite-deletions-and-translated-support
  - lem-binary-products-and-avoidance
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-sum-over-a-finite-index-set
  - math:def-finite-cardinality
  - math:def-set-difference-and-symmetric-difference
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - math:def-ring
  - math:def-indexed-family
  - math:def-cartesian-product
  - math:def-axiom-schema-of-separation
  - math:def-subset-and-proper-subset
  - math:def-ordered-pair
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-relation-domain-range-and-field
  - math:def-function
  - math:def-natural-numbers
dependency_roles:
  math:thm-reals-field: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:def-nat-addition: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  def-euler-finite-certificate-indices: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  alg-euler-finite-indicator-sieve: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:def-real-order: mathematical-premise
  math:def-field: mathematical-premise
  math:lem-integer-part: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-set-difference-and-symmetric-difference: mathematical-premise
  lem-euler-finite-indicator-factor-test: mathematical-premise
  lem-invertible-linear-residue-progression: mathematical-premise
  lem-finite-deletions-and-translated-support: mathematical-premise
  lem-binary-products-and-avoidance: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:def-ring: mathematical-premise
  math:def-nat-multiplication: mathematical-premise
  math:def-indexed-family: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-axiom-schema-of-separation: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-ordered-pair: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
  math:def-relation-domain-range-and-field: mathematical-premise
  math:def-function: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, equation (7.1) and the progression following (7.3)
dependency_level: 4
---

## Statement

Let $I_H$ be the set of integers $j$ with $0\le j\le H$, where $H=2^{22}-1=4{,}194{,}303$. Let $\mathcal P_3$ be the primes of the form $3+4q$ for an integer $q$, and let $S$ be the members of $\mathcal P_3$ with $p\le4096$. For integers $d,a$, write $d\mid a$ if $a=dt$ for some integer $t$, and call such a $d$ a divisor of $a$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself.

The floor indicator at $j\in I_H$ is the binary value
$$\varepsilon_j=\prod_{p\in S}\left(1-\left\lfloor\frac{4j+1}{p}\right\rfloor+\left\lfloor\frac{4j}{p}\right\rfloor\right).$$
Here binary means $0$ or $1$. In the floor arguments, view the numerator and the denominator in the canonical copy of the integers in the real field. Division by $p$ gives the unique real number whose product with the real image of $p$ equals the real image of the numerator. For a real $x$, its floor $\lfloor x\rfloor$ is the unique integer $m$ with $m\le x<m+1$. A finite set has a list of natural-number length containing each member exactly once. The product multiplies one factor for each member of the finite set $S$, in the natural numbers $\{0,1,2,\ldots\}$, with value $1$ for a list with no factors. Each displayed integer factor enters the product as the unique natural number whose image under the canonical embedding into the integers is that factor.

For each $p\in S$, write $b_p=(3p-1)/4$ for the integer satisfying $4b_p=3p-1$. The deletion set $E_p$ is the part of the arithmetic progression $b_p,b_p+p,b_p+2p,\ldots$ that lies in $I_H$. The progression sieve starts with $I_H$ and, for each $p\in S$ in increasing order, replaces the current set $D$ by $D\setminus E_p$, the elements of $D$ outside $E_p$. Write $C$ for the final set of retained indices.

For every $p\in S$ and $j\in I_H$, $p\mid 4j+1$ holds exactly when $j=b_p+rp$ for some integer $r\ge0$. For every $j\in I_H$, $j\in C$ holds exactly when $\varepsilon_j=1$.

## Statement references

[[def-euler-finite-certificate-indices]]

[[def-euler-prime-classes]]

[[alg-euler-finite-indicator-sieve]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-prime]]

[[math:def-divides-in-z]]

[[math:def-real-numbers]]

[[math:lem-int-embeds-rat]]

[[math:lem-rat-embeds-dense]]

[[math:def-real-order]]

[[math:def-field]]

[[math:thm-reals-field]]

[[math:lem-integer-part]]

[[math:def-sum-over-a-finite-index-set]]

[[math:def-natural-numbers]]

[[math:def-nat-multiplication]]

[[math:def-indexed-family]]

[[math:lem-nat-embeds-int]]

[[math:def-finite-cardinality]]

[[math:def-set-difference-and-symmetric-difference]]

## Facts & Assumptions

[F1] The certificate defines the finite sets $I_H$ and $S$ and the product $\varepsilon_j$ over $S$ for $j\in I_H$. A member of $S$ is prime and has the form $3+4q$ for an integer $q$. A finite set admits a list containing each member exactly once, and the finite-set product multiplies the corresponding factor values. [[def-euler-finite-certificate-indices]] [[def-euler-prime-classes]] [[math:def-finite-cardinality]] [[math:def-sum-over-a-finite-index-set]]

[F2] The sieve starts with $I_H$ and scans the integers from $1$ through $4096$. At $p\in S$ it deletes $E_p$ by set difference, retaining precisely the current members outside $E_p$. At other positions the current set is unchanged. [[alg-euler-finite-indicator-sieve]] [[math:def-set-difference-and-symmetric-difference]]

[F3] The integer operations are closed under addition, subtraction and multiplication, with the commutative ring laws. The integer order is total and strict inequalities are preserved by adding a fixed integer or multiplying by a positive integer. In particular, $4x<4y$ implies $x<y$ by totality and preservation of strict order. [[math:def-int-operations]] [[math:def-int-order]] [[math:thm-int-ordered-ring]] [[math:def-ring]]

[F4] A prime $p$ satisfies $p>1$. The relation $p\mid a$ means $a=pt$ for an integer $t$. For $p>0$, every integer $a$ has a unique expression $a=sp+t$ with integers $s,t$ and $0\le t<p$, so $p\mid a$ implies that the remainder $t$ is $0$. [[math:def-prime]] [[math:def-divides-in-z]] [[math:thm-division-algorithm-in-z]]

[F5] For a prime $p$ and integers $a,b$ with $p\nmid a$, the condition $p\mid aj+b$ has a unique integer solution $j_0$ in $0\le j_0<p$, and its nonnegative integer solutions are exactly $j_0+rp$ for integers $r\ge0$. Here $p\nmid a$ means that $p$ does not divide $a$. [[lem-invertible-linear-residue-progression]]

[F6] For $j\in I_H$ and $p\in S$, the integer floor expression displayed as the $p$-factor is $0$ when $p\mid4j+1$ and $1$ otherwise. [[lem-euler-finite-indicator-factor-test]]

[F7] An $S$-indexed family is a function with domain $S$, with $d_p$ denoting its value at $p$. [[math:def-indexed-family]] For such a family of natural numbers $d_p\in\{0,1\}$ on a finite set $S$, the natural complement $1-d_p$ is the unique natural number $c$ satisfying $d_p+c=1$ under natural addition. [[math:def-nat-addition]] It is $1$ at $d_p=0$ and $0$ at $d_p=1$. The product of the complements is $1$ if all $d_p=0$ and $0$ if some $d_p=1$. [[lem-binary-products-and-avoidance]]

[F8] If a finite list of subsets of the integers is deleted successively by set difference from a finite set of integers, an integer is in the final set exactly when it belongs to the starting set and to none of the deletion sets. [[lem-finite-deletions-and-translated-support]]

[F9] The canonical embedding $e$ of the integers into the reals first embeds the integers into the rationals and then sends each rational to the real class of the corresponding constant sequence. Both maps are injective and preserve addition. [[math:lem-int-embeds-rat]] [[math:lem-rat-embeds-dense]] The reals form a field, so their addition is an abelian group and each nonzero real has a multiplicative inverse. [[math:thm-reals-field]] [[math:def-field]] Every real number has a unique integer floor in this canonical copy of the integers. [[math:lem-integer-part]]

[F10] The canonical embedding $\iota$ of the naturals into the integers is injective and sends natural $0$ and $1$ to the corresponding integers. [[math:lem-nat-embeds-int]] [[math:def-int-operations]]

[F11] The Cartesian product $A\times B$ is the set of ordered pairs $(a,b)$ with $a\in A$ and $b\in B$. [[math:def-cartesian-product]] [[math:def-ordered-pair]] Equal ordered pairs have the same first and second coordinates. [[math:thm-the-characterising-property-of-ordered-pairs]] The natural numbers $\mathbb N$ contain $0$ and $1$. [[math:def-natural-numbers]]

[F12] Separation gives the set of elements of an existing set that satisfy a formula with fixed parameters. [[math:def-axiom-schema-of-separation]] The separated set is a subset of the existing set. [[math:def-subset-and-proper-subset]]

[F13] A subset of a Cartesian product is a relation, whose domain consists of the first coordinates of its pairs. [[math:def-relation-domain-range-and-field]] A relation is a function when each first coordinate in its domain has exactly one second coordinate. [[math:def-function]]

## Proof

**Given:** The certificate index set $I_H$, the prime set $S$, the floor product $\varepsilon_j$, and the stated sieve.

**Goal:** For each $p\in S$, identify the indices $j\in I_H$ with $p\mid4j+1$. Then show that $j$ survives the sieve exactly when $\varepsilon_j=1$.

1.1 Fix $p\in S$ and write $p=3+4q$ with $q$ an integer. Then $3p-1=4(2+3q)$, so $b_p=2+3q$ is an integer and $4b_p+1=3p$. Since $p>1$, we have $0<3p-1<4p$, where the second inequality follows from $4p-(3p-1)=p+1>0$. Strict order is preserved by multiplication by $4$, so the integer $b_p$ is unique and $4\cdot0<4b_p<4p$ gives $0<b_p<p$. [given, F1, F3, F4]

1.2 Fix $j\in I_H$. The composite $e$ is injective and preserves addition. Since $0+0=0$ in the integers, $e(0)=e(0)+e(0)$, and adding the real additive inverse of $e(0)$ to both sides gives $e(0)=0$ in the reals. For each $p\in S$, $p>1$ gives $p\ne0$, so $e(p)\ne0$ by injectivity and $e(0)=0$. For either integer numerator $a=4j+1$ or $a=4j$, the equation $e(p)u=e(a)$ has solution $u=e(p)^{-1}e(a)$. Multiplying the equation by $e(p)^{-1}$ shows uniqueness. Both quotients are real numbers, so each has a uniquely determined integer floor. [given, F3, F4, F9]

2.1 For the fixed $j$, use Separation in $S\times\mathbb N$ to form the set $G_j$ of pairs $(p,n)$ for which either $n=1$ and $p\mid4j+1$, or $n=0$ and $p\nmid4j+1$. The coordinates of each pair are unique. For each $p\in S$ exactly one divisibility case holds, and its required second coordinate is a natural number. The ordered pair with that coordinate belongs to $G_j$, and the condition excludes every other second coordinate for $p$. Every first coordinate of $G_j$ lies in $S$. Therefore $G_j$ is a function with domain $S$, and its values $d_p=G_j(p)$ form an $S$-indexed binary family. [given, F4, F7, F11, F12, F13, step 1.2]

2.2 If $p\mid4$, there is an integer $u$ with $4=pu$. The identity in step 1.1 would give $1=3p-4b_p=p(3-ub_p)$, whereas the unique remainder of $1$ on division by $p$ is $1$, since $1=0\cdot p+1$ and $0\le 1<p$. Hence $p\nmid4$. [F3, F4, step 1.1]

3.1 The factor test gives the integer floor expression $0$ when $d_p=1$ and $1$ when $d_p=0$. Since $\iota$ is injective and carries the natural $0$ and $1$ to those integers, the unique natural representative is $0$ when $d_p=1$ and $1$ when $d_p=0$. These are the respective values of the natural complement $1-d_p$, so it is the factor used in the product. The binary product rule on the finite set $S$ then gives $\varepsilon_j=1$ exactly when all $d_p=0$, or equivalently when no $p\in S$ divides $4j+1$. [given, F1, F4, F6, F7, F10, step 1.2, step 2.1]

3.2 Apply the progression lemma with coefficients $a=4$ and $b=1$. The integer $b_p$ lies in the required range and satisfies $p\mid4b_p+1$, so it is the lemma's unique $j_0$. The nonnegative solutions are therefore exactly $b_p+rp$ with $r$ a nonnegative integer. Restricting to $j\in I_H$ gives $j\in E_p$ exactly when $p\mid4j+1$. [given, F1, F2, F4, F5, step 1.1, step 2.2]

4.1 The scan processes each member of $S$ once because each is an integer with $1\le p\le4096$. The skipped positions make no changes, so the updates are precisely the successive deletions of $E_p$ for that increasing finite list. Each $E_p$ contains only indices in $I_H$, and $I_H$ is a finite set of integers. The finite deletion rule gives, for $j\in I_H$, that $j\in C$ exactly when $j$ lies in none of the $E_p$. By step 3.2, this holds exactly when no $p\in S$ divides $4j+1$. [given, F1, F2, F3, F4, F8, step 3.2]

5.1 By steps 4.1 and 3.1, $j\in C$ if and only if $\varepsilon_j=1$ for each $j\in I_H$. Together with the divisibility progression from step 3.2, this proves both assertions. [step 3.2, step 4.1, step 3.1] ∎

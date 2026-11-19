---
title: Each floor factor tests divisibility by its prime
status: published
research_item: lem-euler-finite-indicator-factor-test
dependency_level: 3
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, paragraph following (7.1)
---

PDF p. 7: ` §7, paragraph following (7.1) `

## Prerequisites

- [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [lem-floor-increment-divisibility](item-lem-floor-increment-divisibility)
- [lem-binary-products-and-avoidance](item-lem-binary-products-and-avoidance)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:thm-reals-field](https://alphabetamath.cc/item/thm-reals-field)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)


## Statement

Let $j$ be an integer with $0\le j\le H$, where $H=4{,}194{,}303$. Let $S$ be the set of primes $p\le4096$ congruent to $3$ modulo $4$, meaning $p-3=4q$ for some integer $q$. For integers $d,a$, write $d\mid a$ if $a=dt$ for some integer $t$, and call such a $d$ a divisor of $a$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself.

For real quotients and floor comparisons, identify each integer with the real class of the constant sequence whose terms equal its canonical rational image. For $p>0$, the quotient $a/p$ is the unique real $u$ with $pu=a$. For real $x$, its floor $\lfloor x\rfloor$ is the unique integer $m$ satisfying $m\le x<m+1$.

For each $p\in S$, write the factor in (7.1) as
$$f_{j,p}=1-\left\lfloor\frac{4j+1}{p}\right\rfloor+\left\lfloor\frac{4j}{p}\right\rfloor.$$
The indicator $\varepsilon_j=\prod_{p\in S} f_{j,p}$ multiplies one factor per member of the finite set $S$, with empty product $1$. Then $f_{j,p}=0$ if $p\mid4j+1$ and $f_{j,p}=1$ otherwise. Hence $\varepsilon_j\in\{0,1\}$.

## Statement references

[Finite certificate indices and indicator](item-def-euler-finite-certificate-indices)

[Prime classes](item-def-euler-prime-classes)

[Integers](https://alphabetamath.cc/item/def-integers)

[Integer order](https://alphabetamath.cc/item/def-int-order)

[Integer operations](https://alphabetamath.cc/item/def-int-operations)

[Real numbers](https://alphabetamath.cc/item/def-real-numbers)

[Real order](https://alphabetamath.cc/item/def-real-order)

[Division in a field](https://alphabetamath.cc/item/def-field)

[The real field](https://alphabetamath.cc/item/thm-reals-field)

[Integers in the rationals](https://alphabetamath.cc/item/lem-int-embeds-rat)

[Rationals in the reals](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[The floor of a real number](https://alphabetamath.cc/item/lem-integer-part)

[Integer divisibility](https://alphabetamath.cc/item/def-divides-in-z)

[Products over finite sets](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

## Facts & Assumptions

[F1] The certificate definition gives the finite set $S$ of positive integers and, for $0\le j\le H$, the product $\varepsilon_j$ of the displayed factors, taken in the natural numbers when the factors are regarded as $0$ or $1$. Finiteness means that the members can be listed once each in a list of natural-number length. A finite-set product multiplies the listed values and has value $1$ when the list is empty. [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices) [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F2] For integers $a,p$ with $p>0$, the floor difference $\lfloor a/p\rfloor-\lfloor(a-1)/p\rfloor$ is $1$ if $p\mid a$ and $0$ otherwise. Here $p\mid a$ means $a=pt$ for some integer $t$. [lem-floor-increment-divisibility](item-lem-floor-increment-divisibility) [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[F3] The integers are closed under addition, subtraction and multiplication. Integer addition is associative and commutative with identity $0$, and subtraction is addition of the additive inverse. [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[F4] Write $\mathbb{N}=\{0,1,2,\ldots\}$ for the natural numbers. Addition on $\mathbb{N}$ is the operation defined by recursion on the second argument. The map $\iota$ sending each natural number to its integer copy is injective and preserves addition. It sends the natural numbers $0$ and $1$ to the corresponding integers. [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[F5] For natural values $b_p\in\{0,1\}$ indexed by a finite set $S$, the natural complement $c_p=1-b_p$ is the unique natural number satisfying $b_p+c_p=1$. The product of these complements is $1$ if every $b_p=0$ and is $0$ if some $b_p=1$. [lem-binary-products-and-avoidance](item-lem-binary-products-and-avoidance)

[F6] The canonical map $e$ from the integers to the reals is the composite of the integer-to-rational and rational-to-real embeddings. Both are injective and preserve addition. [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) The reals form a field. Each nonzero real $y$ therefore has a multiplicative inverse $y^{-1}$. [math:thm-reals-field](https://alphabetamath.cc/item/thm-reals-field) [math:def-field](https://alphabetamath.cc/item/def-field)

## Proof

**Given:** An integer $j$ with $0\le j\le H$ and the finite product defining $\varepsilon_j$.

**Goal:** Evaluate the factor for each $p\in S$ and show that $\varepsilon_j\in\{0,1\}$.

1.1 Since $e$ preserves addition, $e(0)=e(0)+e(0)$, so additive cancellation gives $e(0)=0$. For a positive integer $p$, injectivity gives $e(p)\ne0$. For any integer $a$, the equation $e(p)u=e(a)$ has the solution $u=e(a)e(p)^{-1}$. Multiplying the equation by $e(p)^{-1}$ shows uniqueness. [F6]

2.1 Put $a=4j+1$, an integer, so $a-1=4j$. For each $p\in S$ we have $p>0$, so the floor difference $d_p=\lfloor a/p\rfloor-\lfloor(a-1)/p\rfloor$ is $1$ when $p\mid4j+1$ and $0$ otherwise. [given, F1, F2, F3, step 1.1]

3.1 By associativity, commutativity and the additive inverse law, $-\lfloor a/p\rfloor+\lfloor(a-1)/p\rfloor$ is the additive inverse of $d_p$. Hence $f_{j,p}=1-d_p$. Thus $f_{j,p}=0$ when $p\mid4j+1$ and $f_{j,p}=1$ otherwise. [F3, step 2.1]

4.1 For each $p\in S$, let $b_p$ be the natural number $0$ or $1$ with integer copy $d_p$. Its complement $c_p$ satisfies $b_p+c_p=1$. Applying $\iota$ gives $d_p+\iota(c_p)=1$, hence $\iota(c_p)=1-d_p=f_{j,p}$. The factors of the certificate product as natural numbers are therefore the complements $c_p$. [F1, F3, F4, F5, step 2.1, step 3.1]

5.1 The product rule now gives $\varepsilon_j=1$ if every $b_p=0$, including for an empty set $S$, and $\varepsilon_j=0$ if some $b_p=1$. These alternatives exhaust the possible families of binary values. This proves $\varepsilon_j\in\{0,1\}$ together with the factor evaluation. [F1, F5, step 3.1, step 4.1] ∎

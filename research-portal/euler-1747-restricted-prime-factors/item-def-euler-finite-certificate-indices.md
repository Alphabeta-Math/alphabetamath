---
title: Finite-range indices and binary indicators
status: draft
research_item: def-euler-finite-certificate-indices
dependency_level: 2
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, definition of H and (7.1), and p. 8, Proposition 7.2, first
        sentence of proof
---

PDF p. 7: ` §7, definition of H and equation (7.1) `; PDF p. 8: ` Proposition 7.2, index range in the proof `

## Prerequisites

- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-nat-power](https://alphabetamath.cc/item/def-nat-power)
- [def-author-c74aeff6099d-bounded-integer-indices](item-def-author-c74aeff6099d-bounded-integer-indices)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [lem-floor-increment-divisibility](item-lem-floor-increment-divisibility)
- [lem-binary-products-and-avoidance](item-lem-binary-products-and-avoidance)


## Definition

Take $H=2^{22}-1=4{,}194{,}303$. Compute $2^{22}$ by multiplying twenty-two copies of $2$ in the natural numbers and use its integer image under the canonical embedding to form $H$. For a nonnegative integer $B$, write $I_B$ for the integers from $0$ through $B$, including both endpoints. The finite-range input at index $k$ is $n=4k+2$ for $k\in I_H$.

Let $S=\{p\in I_{4096}:p\in\mathcal P_3\}$, where $\mathcal P_3$ consists of the primes congruent to $3$ modulo $4$. A divisor of an integer $p$ is an integer $d$ for which $p=dq$ for some integer $q$. A prime is an integer greater than $1$ with only $1$ and itself as positive divisors. Congruence to $3$ modulo $4$ means $p-3=4q$ for some integer $q$.

For real quotients and floor comparisons, send each integer to its canonical rational image and then to the real class of the constant sequence with that rational value. With this identification, $a/p$ is the real number $u$ satisfying $pu=a$ for $p\ne0$. For a real number $x$, its floor $\lfloor x\rfloor$ is the unique integer $m$ with $m\le x<m+1$. For each integer $j$ with $0\le j\le H$, define the binary indicator $\varepsilon_j$ by
$$\varepsilon_j=\prod_{p\in S}\left(1-\left\lfloor\frac{4j+1}{p}\right\rfloor+\left\lfloor\frac{4j}{p}\right\rfloor\right).$$
The product is taken in the natural numbers, with one factor for each $p\in S$. Identify each displayed integer factor $0$ or $1$ with its natural preimage under the canonical embedding into the integers. Take any list of the members of $S$ with each member occurring exactly once. A product with no factors has value $1$. For every integer $j<0$, set $\varepsilon_j=0$. Here binary means that each value is either $0$ or $1$.

## Definition references

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-nat-power](https://alphabetamath.cc/item/def-nat-power)

[def-author-c74aeff6099d-bounded-integer-indices](item-def-author-c74aeff6099d-bounded-integer-indices)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)

[math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

## Justification

The embedding of the natural numbers into the integers preserves multiplication, so the repeated product defining $2^{22}$ can be evaluated in integer arithmetic. Successive multiplication gives $2^5=32$. Grouping the twenty-two factors as four groups of five and a remaining pair gives $2^{22}=4\cdot32\cdot32\cdot32\cdot32=4{,}194{,}304$. Subtraction gives the stated nonnegative integer $H$, so the bounded index set $I_H$ is defined and finite ([Natural numbers](https://alphabetamath.cc/item/def-natural-numbers), [Powers of natural numbers](https://alphabetamath.cc/item/def-nat-power), [Natural numbers in the integers](https://alphabetamath.cc/item/lem-nat-embeds-int), [Integer arithmetic and order](https://alphabetamath.cc/item/thm-int-ordered-ring), [Bounded integer index sets](item-def-author-c74aeff6099d-bounded-integer-indices)). Integer addition and multiplication assign a single integer $4k+2$ to each index.

The membership condition for $S$ defines a unique subset of the finite set $I_{4096}$, so $S$ is finite ([Subset by a membership condition](https://alphabetamath.cc/item/def-subset-and-proper-subset), [Bounded integer index sets](item-def-author-c74aeff6099d-bounded-integer-indices), [Finiteness of a subset](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)). Primes are positive, so $S$ includes exactly the primes in $\mathcal P_3$ that satisfy $p\le4096$. Every $p\in S$ is positive. The composite embedding sends integer $0$ to real $0$ and preserves order, so the real image of $p$ is positive. See [The integers in the rationals](https://alphabetamath.cc/item/lem-int-embeds-rat) and [The rationals in the reals](https://alphabetamath.cc/item/lem-rat-embeds-dense). Both quotients therefore exist in the real field and both floors are determined uniquely in this same copy of the integers ([Prime classes](item-def-euler-prime-classes), [The real ordered field](https://alphabetamath.cc/item/thm-reals-ordered-field), [Division in a field](https://alphabetamath.cc/item/def-field), [Floor existence and uniqueness](https://alphabetamath.cc/item/lem-integer-part)).

For each $j\in I_H$, put $b=4j+1$, so that $b-1=4j$. The difference of the two floors in the displayed factor, in the order $\lfloor b/p\rfloor-\lfloor(b-1)/p\rfloor$, is either $0$ or $1$ by the floor-difference lemma for integer $b$ and positive integer $p$ ([Floor difference for a positive denominator](item-lem-floor-increment-divisibility)). If that difference is $d$, the factor equals $1-d$ by integer arithmetic. For $d=0$ this equals $1$, and for $d=1$ it equals $0$. Under the canonical natural-to-integer embedding, the natural $0$ and $1$ map to the corresponding integer values. In each case the two corresponding naturals for $d$ and $1-d$ add to $1$, by preservation of addition and injectivity. This is the natural-number complement used by the binary product rule ([Natural numbers](https://alphabetamath.cc/item/def-natural-numbers), [Natural numbers in the integers](https://alphabetamath.cc/item/lem-nat-embeds-int)). Thus the product over the finite set $S$ is a uniquely defined product of natural numbers, and the binary product rule makes its value $0$ or $1$ ([Finite-set product](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set), [Binary product rule](item-lem-binary-products-and-avoidance)). The cases $j<0$ and $0\le j\le H$ are disjoint and cover every integer $j\le H$, so the prescribed zero values complete the definition on its intended domain.

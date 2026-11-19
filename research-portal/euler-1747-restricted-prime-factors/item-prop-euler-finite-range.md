---
title: "Proposition 7.2: The finite range"
status: draft
research_item: prop-euler-finite-range
dependency_level: 8
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, Abstract, finite certificate coverage, pp. 7–8, (7.2), Table 1
        and Proposition 7.2, statement and proof
---

PDF p. 1: ` Abstract, finite certificate coverage `; PDF p. 8: ` Proposition 7.2, statement and stated certificate implication `

## Prerequisites

- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-nat-power](https://alphabetamath.cc/item/def-nat-power)
- [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)
- [lem-euler-finite-range-index-count](item-lem-euler-finite-range-index-count)
- [lem-euler-finite-indicator-membership](item-lem-euler-finite-indicator-membership)
- [def-euler-finite-unrepresented-count](item-def-euler-finite-unrepresented-count)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [lem-euler-finite-indicator-sieve-equivalence](item-lem-euler-finite-indicator-sieve-equivalence)
- [prop-euler-finite-certificate-table](item-prop-euler-finite-certificate-table)
- [lem-euler-finite-unrepresented-count-meaning](item-lem-euler-finite-unrepresented-count-meaning)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)


## Statement

Let $\mathcal A$ be the set of positive integers whose prime divisors are all congruent to $1$ modulo $4$. A positive integer is greater than $0$. An integer $d$ divides an integer $x$ if $x=dq$ for some integer $q$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. A prime divisor of $x$ is a divisor of $x$ that is prime. Write $u\equiv v\pmod4$ for integers $u,v$ when $u-v=4q$ for some integer $q$. The power $64^4$ denotes the product of four copies of $64$.

For every integer $n$ with $2\le n<64^4$ and $n\equiv2\pmod4$, there are $a,b\in\mathcal A$ such that $n=a+b$ and at least one of $a,b$ is at most $313$.

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[math:def-nat-power](https://alphabetamath.cc/item/def-nat-power)

## Facts & Assumptions

[F1] Set $H=4{,}194{,}303$ and let $I_H$ consist of the integers from $0$ through $H$, including both endpoints. The formula $n=4k+2$ lists exactly the integers in the Statement as $k$ runs over $I_H$, each once. Its first value is $2$ and its last value is $64^4-2$. [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices) [lem-euler-finite-range-index-count](item-lem-euler-finite-range-index-count)

[F2] For integers $j\le H$, the certificate indicator $\varepsilon_j$ is a value in $\{0,1\}$ that, for $0\le j\le H$, equals $1$ exactly when $4j+1\in\mathcal A$. For every negative integer $j$ the value is $0$. Since $313=4\cdot78+1$, the count at cutoff $313$ is defined by
$$U(313)=\sum_{k=0}^{H}\prod_{i=0}^{78}(1-\varepsilon_i\varepsilon_{k-i}).$$
The sum adds one term per integer $k$ from $0$ through $H$, and the product multiplies one factor per integer $i$ from $0$ through $78$, including both endpoints. Integer order is preserved by addition, so $0\le i\le78\le H$ gives $k-i\le k\le H$. Both indicator arguments are therefore in the defining range. [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices) [lem-euler-finite-indicator-membership](item-lem-euler-finite-indicator-membership) [def-euler-finite-unrepresented-count](item-def-euler-finite-unrepresented-count) [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[F3] By the sieve equivalence, the deletion procedure used in the certificate table leaves an index $j\in I_H$ exactly when $\varepsilon_j=1$. Thus its binary values at indices in $I_H$ agree with those of [F2], and it uses the same zero value at negative indices. The table gives $U(313)=0$ for this sum of products. [lem-euler-finite-indicator-sieve-equivalence](item-lem-euler-finite-indicator-sieve-equivalence) [prop-euler-finite-certificate-table](item-prop-euler-finite-certificate-table)

[F4] For an integer cutoff $c$ satisfying $1\le c\le313$ and $c\equiv1\pmod4$, the count $U(c)$ is defined by the same formula with upper product index $m$ given by $c=4m+1$. It is the number of indices $k\in I_H$ for which there are no $x,y\in\mathcal A$ satisfying $4k+2=x+y$ and $x\le c$. [def-euler-finite-unrepresented-count](item-def-euler-finite-unrepresented-count) [lem-euler-finite-unrepresented-count-meaning](item-lem-euler-finite-unrepresented-count-meaning)

[F5] The number of elements of a finite set is the length of a list containing each of its elements exactly once. If that number is zero, the set has no elements because the list has no entries. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

## Proof

**Given:** An integer $n$ with $2\le n<64^4$ and $n\equiv2\pmod4$.

**Goal:** Find $a,b\in\mathcal A$ with $n=a+b$ and at least one of $a,b$ at most $313$.

1.1 The index formula gives a unique $k\in I_H$ with $n=4k+2$. This includes $k=0$ for $n=2$ and $k=H$ for $n=64^4-2$. [given, F1]

1.2 The cutoff $313$ satisfies the bounds and congruence in [F4] because $313=4\cdot78+1$. By the table value $U(313)=0$ and its count interpretation, the set of indices in $I_H$ lacking a representation with first summand at most $313$ has zero elements. That set is therefore empty. [F2, F3, F4, F5]

2.1 The index from step 1.1 thus has a representation $4k+2=x+y$ with $x,y\in\mathcal A$ and $x\le313$. Set $a=x$ and $b=y$. Then $n=a+b$, and $a\le313$ gives the required bound on at least one summand. Since $n$ was arbitrary in the stated range, the result holds throughout that range. [F4, step 1.1, step 1.2] ∎

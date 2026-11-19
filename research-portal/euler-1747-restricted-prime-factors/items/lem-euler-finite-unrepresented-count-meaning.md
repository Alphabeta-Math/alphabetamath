---
id: lem-euler-finite-unrepresented-count-meaning
kind: lemma
title: The product-sum counts unrepresented inputs
status: published
domain: mathematics
deps:
  - def-euler-finite-unrepresented-count
  - def-euler-finite-certificate-indices
  - def-euler-prime-classes
  - def-author-c74aeff6099d-bounded-integer-indices
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - math:def-divides-in-z
  - math:def-prime
  - math:def-finite-cardinality
  - math:def-sum-over-a-finite-index-set
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - lem-euler-finite-indicator-membership
  - lem-euler-admissible-products
  - lem-binary-products-and-avoidance
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - math:lem-nat-discrete
  - math:def-nat-multiplication
  - math:lem-nat-mult-identity
  - math:def-nat-addition
  - math:def-nat-order
formulation_deps:
  - def-euler-finite-unrepresented-count
  - def-euler-finite-certificate-indices
  - def-euler-prime-classes
  - def-author-c74aeff6099d-bounded-integer-indices
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - math:def-divides-in-z
  - math:def-prime
  - math:def-finite-cardinality
  - math:def-sum-over-a-finite-index-set
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:def-nat-addition
  - math:def-nat-multiplication
argument_deps:
  - def-euler-finite-unrepresented-count
  - def-euler-finite-certificate-indices
  - def-author-c74aeff6099d-bounded-integer-indices
  - def-euler-prime-classes
  - lem-euler-finite-indicator-membership
  - lem-euler-admissible-products
  - lem-binary-products-and-avoidance
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - math:def-sum-over-a-finite-index-set
  - math:lem-nat-embeds-int
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - math:lem-nat-discrete
  - math:def-nat-multiplication
  - math:lem-nat-mult-identity
  - math:def-nat-addition
  - math:def-nat-order
dependency_roles:
  math:def-nat-addition: mathematical-premise
  math:def-nat-order: mathematical-premise
  def-euler-finite-unrepresented-count: mathematical-premise
  def-euler-finite-certificate-indices: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  def-author-c74aeff6099d-bounded-integer-indices: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  lem-euler-finite-indicator-membership: mathematical-premise
  lem-euler-admissible-products: mathematical-premise
  lem-binary-products-and-avoidance: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:def-nat-multiplication: mathematical-premise
  math:lem-nat-mult-identity: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, paragraph after (7.2), and p. 8, Proposition 7.2,
        vanishing-factor criterion
dependency_level: 5
---

## Statement

Let $a$ be an integer with $1\le a\le313$ and $a\equiv1\pmod4$. For integers $u,v$, the congruence $u\equiv v\pmod4$ means $u-v=4q$ for some integer $q$. Write $m=(a-1)/4$ for the integer quotient and $H=4{,}194{,}303$. For each nonnegative integer $B$, let $I_B$ be the finite set of integers from $0$ through $B$, including both endpoints.

Let $\mathcal A$ be the set of positive integers whose prime divisors are all congruent to $1$ modulo $4$. Positive means greater than $0$. A divisor of $x$ is an integer $d$ such that $x=dq$ for some integer $q$, and a prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. A prime divisor is a divisor that is prime.

Use the certificate indicators $\varepsilon_j$ of (7.1), with values in $\{0,1\}$ for $j\in I_H$ and $\varepsilon_j=0$ for integers $j<0$. The product-sum is
$$U(a)=\sum_{k\in I_H}\prod_{i\in I_m}(1-\varepsilon_i\varepsilon_{k-i}).$$
Each finite sum adds one term per index and each finite product multiplies one factor per index. The operations are on the natural numbers $0,1,2,\ldots$, identified with the nonnegative integers. For a binary value $b$ (a value of $0$ or $1$), $1-b$ is $1$ when $b=0$ and $0$ when $b=1$.

A representation of $4k+2$ with first summand at most $a$ means an equality $4k+2=x+y$ with $x,y\in\mathcal A$ and $x\le a$. For $k\in I_H$, the factor indexed by $i\in I_m$ is zero exactly when $\varepsilon_i=\varepsilon_{k-i}=1$, in which case $i\le k$. The product at $k$ equals $0$ if the specified representation exists and $1$ otherwise. Thus $U(a)$ equals the number of indices $k\in I_H$ with no such representation. This number is the length of a list containing each such index exactly once.

## Statement references

[[def-euler-finite-unrepresented-count]]

[[def-euler-finite-certificate-indices]]

[[def-euler-prime-classes]]

[[def-author-c74aeff6099d-bounded-integer-indices]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-congruence-modulo-an-integer]]

[[math:def-divides-in-z]]

[[math:def-prime]]

[[math:def-finite-cardinality]]

[[math:def-sum-over-a-finite-index-set]]

[[math:def-natural-numbers]]

[[math:lem-nat-embeds-int]]

[[math:def-nat-addition]]

[[math:def-nat-multiplication]]

## Facts & Assumptions

[F1] The definition of $U(a)$ supplies the integer $m$ with $a=4m+1$ and the sum of the products on $I_H$ and $I_m$. The definition of the bounded index sets makes $I_B$ finite whenever $B$ is a nonnegative integer. [[def-euler-finite-unrepresented-count]] [[def-author-c74aeff6099d-bounded-integer-indices]]

[F2] The certificate fixes $H=4{,}194{,}303$, gives binary values $\varepsilon_j$ for $0\le j\le H$, and sets $\varepsilon_j=0$ for every integer $j<0$. [[def-euler-finite-certificate-indices]]

[F3] For an integer $j\in I_H$, $\varepsilon_j=1$ exactly when $4j+1\in\mathcal A$. Every member of $\mathcal A$ is positive by definition and congruent to $1$ modulo $4$ by the earlier congruence result. The congruence $x\equiv1\pmod4$ gives $x=4q+1$ for some integer $q$. [[lem-euler-finite-indicator-membership]] [[def-euler-prime-classes]] [[lem-euler-admissible-products]] [[math:def-congruence-modulo-an-integer]]

[F4] Integer order is total and preserved by translation. Positive integers have positive products, so $s<t$ gives $4(t-s)>0$ and hence $4s<4t$ by distributivity. Integer subtraction adds the additive inverse. [[math:thm-int-ordered-ring]] [[math:def-int-operations]]

[F5] The natural numbers map to the nonnegative integers, preserving order, $0$, $1$, addition and multiplication. No natural number lies strictly between $0$ and $1$, so a positive integer is at least $1$. [[math:lem-nat-embeds-int]] [[math:lem-nat-discrete]] [[math:def-nat-addition]] [[math:def-nat-order]]

[F6] For an integer $n$ and a positive integer $d$, there is a unique integer quotient $q$ and integer remainder $r$ such that $n=dq+r$ and $0\le r<d$. [[math:thm-division-algorithm-in-z]]

[F7] In natural multiplication, a right factor of $0$ gives $0$ and a right factor of $1$ gives the left factor. [[math:def-nat-multiplication]] [[math:lem-nat-mult-identity]]

[F8] For finite index sets $X$ and $I$ and a value $b_{k,i}$ in $\{0,1\}$ for each $k\in X$ and $i\in I$, the product of $1-b_{k,i}$ over $i\in I$ is $0$ if some $b_{k,i}=1$ and $1$ otherwise. Its sum over $k\in X$ equals the number of indices for which every $b_{k,i}=0$. The sum and product use any listing that includes each index once. [[lem-binary-products-and-avoidance]] [[math:def-sum-over-a-finite-index-set]]

## Proof

**Given:** An integer $a$ as in the Statement, with $m=(a-1)/4$ and the certificate indicators through $H$.

**Goal:** Identify the zero factors and the represented inputs, and show that $U(a)$ counts the unrepresented indices.

1.1 We have $0\le a-1=4m\le312=4\cdot78$. Multiplication by $4$ is strictly increasing, so $0\le m\le78\le H$. Hence $I_m$ and $I_H$ are finite. For $k\in I_H$ and $i\in I_m$, we have $0\le i\le H$ and $k-i\le k\le H$. Both indicators therefore have specified binary values, using the zero value in [F2] if $k-i<0$. [given, F1, F2, F4]

2.1 Fix such $k,i$. If $\varepsilon_{k-i}=0$, the product $\varepsilon_i\varepsilon_{k-i}$ is $0$. If $\varepsilon_{k-i}=1$, it is $\varepsilon_i$. Thus the product is binary and equals $1$ exactly when both indicators equal $1$. Subtracting it from $1$ gives a zero factor exactly in that case. Since $\varepsilon_{k-i}=0$ for $k-i<0$, a zero factor implies $i\le k$. [F1, F2, F4, F7, step 1.1]

3.1 If a factor at $i$ is zero, then $i$ and $k-i$ are in $I_H$ by the bounds above and $i\le k$. Both indicators equal $1$, so $x=4i+1$ and $y=4(k-i)+1$ lie in $\mathcal A$. Their sum is $4k+2$, and $i\le m$ gives $x\le4m+1=a$. This is a representation with first summand at most $a$. [F1, F3, F4, step 1.1, step 2.1]

3.2 Conversely, suppose $4k+2=x+y$ with $x,y\in\mathcal A$ and $x\le a$. Positivity gives $x,y\ge1$, and congruence gives integers $i,j$ with $x=4i+1$ and $y=4j+1$. Hence $4i=x-1\ge0$ and $4j=y-1\ge0$, so $i,j\ge0$. From $4i+1\le4m+1$ we get $i\le m$. Substitution gives $4k+2=4(i+j)+2$. Since $0\le2<4$, uniqueness of the quotient with remainder on division by $4$ gives $i+j=k$. Thus $i\in I_m$ and $j=k-i\in I_H$, since $0\le j\le k\le H$. The membership test gives $\varepsilon_i=\varepsilon_{k-i}=1$, so the factor at $i$ is zero. [F1, F3, F4, F5, F6, step 1.1, step 2.1]

4.1 Apply [F8] with $X=I_H$, $I=I_m$ and $b_{k,i}=\varepsilon_i\varepsilon_{k-i}$. The index sets are finite and all test values are binary. Steps 3.1 and 3.2 show that at a given $k$ some test equals $1$ exactly when a representation with first summand at most $a$ exists. Thus the product has value $0$ for each represented input and $1$ otherwise. By [F8] its sum counts the indices with no such representation, and by [F1] that sum is $U(a)$. This proves the product and count claims along with the factor test in step 2.1. [F1, F5, F8, step 1.1, step 2.1, step 3.1, step 3.2] ∎

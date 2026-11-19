---
title: The size of the finite input range
status: draft
research_item: lem-euler-finite-range-index-count
dependency_level: 3
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, Abstract, finite certificate count, p. 7, §7, definition of H,
        and p. 8, Proposition 7.2, statement and first sentence of proof
---

PDF p. 1: ` Abstract, finite certificate count `; PDF p. 7: ` §7, definition of H `; PDF p. 8: ` Proposition 7.2, index range in the proof `

## Prerequisites

- [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)
- [def-author-c74aeff6099d-bounded-integer-indices](item-def-author-c74aeff6099d-bounded-integer-indices)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-power](https://alphabetamath.cc/item/def-nat-power)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)
- [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)


## Statement

Let $H=2^{22}-1$ and let $I_H$ consist of the integers $k$ with $0\le k\le H$. Let $T$ consist of the integers $n$ with $2\le n<64^4$ and $n\equiv2\pmod 4$. Here $n\equiv2\pmod 4$ means $n-2=4q$ for some integer $q$, and powers with positive whole-number exponents denote repeated multiplication.

The values $4k+2$ for $k\in I_H$ give every element of $T$ exactly once. The number of elements of $T$ is $H+1=4{,}194{,}304$.

## Statement references

[Finite-range indices](item-def-euler-finite-certificate-indices)

[Bounded integer index sets](item-def-author-c74aeff6099d-bounded-integer-indices)

[The integers](https://alphabetamath.cc/item/def-integers)

[Integer order](https://alphabetamath.cc/item/def-int-order)

[Integer arithmetic](https://alphabetamath.cc/item/def-int-operations)

[Natural numbers](https://alphabetamath.cc/item/def-natural-numbers)

[Natural-number powers](https://alphabetamath.cc/item/def-nat-power)

[Congruence modulo an integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[Subsets defined by a membership condition](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[Number of elements of a finite set](https://alphabetamath.cc/item/def-finite-cardinality)

## Facts & Assumptions

[F1] The certificate bound is $H=2^{22}-1=4{,}194{,}303$, and the input at index $k$ is $4k+2$ ([Finite-range indices](item-def-euler-finite-certificate-indices)).

[F2] For a nonnegative integer $B$, the bounded index set $I_B$ consists of the integers from $0$ through $B$, both included. There is an increasing bijection $e:m\to I_B$, where the natural number $m$ has integer copy $B+1$. See the Definition and Justification of [Bounded integer index sets](item-def-author-c74aeff6099d-bounded-integer-indices), using [Functions](https://alphabetamath.cc/item/def-function), [Bijections](https://alphabetamath.cc/item/def-injection-surjection-bijection) and the [natural-to-integer embedding](https://alphabetamath.cc/item/lem-nat-embeds-int).

[F3] Write $\mathbb Z$ for the integers. Addition, multiplication and negation stay in $\mathbb Z$, with $a-b=a+(-b)$. These operations make the integers a commutative ring. Integer order is total and preserved by addition, and the product of two positive integers is positive ([The integers](https://alphabetamath.cc/item/def-integers), [Integer arithmetic](https://alphabetamath.cc/item/def-int-operations), [Integer order](https://alphabetamath.cc/item/def-int-order), [The integers form a totally ordered ring](https://alphabetamath.cc/item/thm-int-ordered-ring)).

[F4] Natural numbers are $0,1,2,\ldots$. For a natural number $a$ and a positive natural number $j$, the power $a^j$ multiplies $j$ copies of $a$ ([Natural numbers](https://alphabetamath.cc/item/def-natural-numbers), [Natural-number powers](https://alphabetamath.cc/item/def-nat-power), clause (e)).

[F5] The integer copy $\iota(t)$ of a natural number $t$ preserves addition and multiplication, preserves and reflects order, and sends the natural $1$ to the integer $1$. Each nonnegative integer is the copy of exactly one natural number ([Natural numbers in the integers](https://alphabetamath.cc/item/lem-nat-embeds-int), [Integer arithmetic](https://alphabetamath.cc/item/def-int-operations)). With natural addition, $h+1=h+\sigma(0)=\sigma(h+0)=\sigma(h)$ ([Natural numbers](https://alphabetamath.cc/item/def-natural-numbers), [Natural addition](https://alphabetamath.cc/item/def-nat-addition)). For natural numbers $t,h$ with the additive order, $t<\sigma(h)$ if and only if $t\le h$ ([Natural order](https://alphabetamath.cc/item/def-nat-order), [Natural order and membership](https://alphabetamath.cc/item/lem-nat-order-is-membership), clause 3).

[F6] Two integers are congruent modulo $4$ exactly when their difference is $4$ times an integer ([Congruence modulo an integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)).

[F7] For an integer $n$ and a positive integer $b$, there is a unique pair of integers $(q,r)$ with $n=qb+r$ and $0\le r<b$. The integers $q$ and $r$ are called the quotient and remainder, respectively ([Division with remainder in the integers](https://alphabetamath.cc/item/thm-division-algorithm-in-z)). The notation $(q,r)$ denotes the ordered pair with first coordinate $q$ and second coordinate $r$ ([Ordered pairs](https://alphabetamath.cc/item/def-ordered-pair)). Equality of two ordered pairs implies equality of their first coordinates ([Equality of ordered pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)).

[F8] Separation gives the unique subset of a set containing exactly the elements that satisfy a specified condition ([Subsets defined by a membership condition](https://alphabetamath.cc/item/def-subset-and-proper-subset)).

[F9] A bijection $m\to X$ from a von Neumann natural number $m$ to a set $X$ makes $X$ finite with exactly $m$ elements. See [Finite cardinality](https://alphabetamath.cc/item/def-finite-cardinality), with [von Neumann naturals](https://alphabetamath.cc/item/def-natural-numbers) and [bijections](https://alphabetamath.cc/item/def-injection-surjection-bijection).

[F10] The Cartesian product $A\times B$ consists of the ordered pairs $(a,b)$ with $a\in A$ and $b\in B$ ([Cartesian products](https://alphabetamath.cc/item/def-cartesian-product), [Ordered pairs](https://alphabetamath.cc/item/def-ordered-pair)). A subset of this product that contains exactly one pair with first coordinate $a$ for each $a\in A$ gives a function from $A$ to $B$ ([Functions](https://alphabetamath.cc/item/def-function)). The function is bijective if it is injective and surjective ([Injections, surjections and bijections](https://alphabetamath.cc/item/def-injection-surjection-bijection)).

## Proof

**Given:** The bound $H=2^{22}-1$ and the integer input rule $4k+2$ for $k\in I_H$.

**Goal:** Prove that these inputs list exactly the integers of $T$, each once, and compute their number.

1.1 The conditions in the statement define a unique subset $T$ of $\mathbb Z$ by separation. The cutoff satisfies $64^2=4096$ and $64^4=4096\cdot4096=16{,}777{,}216=4\cdot4{,}194{,}304=4(H+1)$, using repeated multiplication and the integer copies of these natural numbers. Consequently $4H+2=64^4-2$. [F1, F3, F4, F5, F6, F8]

1.2 If two indices $k,\ell\in I_H$ give the same integer $n=4k+2=4\ell+2$, then $(k,2)$ and $(\ell,2)$ are both quotient and remainder pairs for $n$ and the positive divisor $4$. Indeed $0\le2<4$ and $4k=k\cdot4$, with the same equality for $\ell$. Uniqueness gives $(k,2)=(\ell,2)$, so their first coordinates satisfy $k=\ell$. [F3, F5, F7]

2.1 Since $4>0$, multiplication by $4$ preserves both strict and weak integer inequalities. Indeed, if $a<b$, then $b-a>0$, so $4(b-a)>0$ and $4a<4b$ by adding $4a$. Equality is preserved by multiplication as well. Thus for $k\in I_H$, the value $n=4k+2$ satisfies $2\le n\le4H+2=64^4-2<64^4$. Since $n-2=4k$, it belongs to $T$. [F1, F2, F3, F5, F6, step 1.1]

3.1 For $n\in T$, congruence gives an integer $k$ with $n=4k+2$. If $k<0$, the order rule in step 2.1 gives $n<2$. If $k\ge H+1$, the same rule gives $n\ge4(H+1)+2=64^4+2$. Both violate the defining bounds of $T$. Therefore $0\le k<H+1$. Write $k=\iota(t)$ and $H=\iota(h)$ for natural numbers $t,h$. Since $h+1=\sigma(h)$ in the naturals, $\iota(\sigma(h))=H+1$ by preservation of addition and $\iota(1)=1$. Order reflection yields $t<\sigma(h)$, so the successor bound gives $t\le h$. Applying $\iota$ gives $k\le H$ and $k\in I_H$. [F1, F2, F3, F5, F6, step 1.1, step 2.1]

3.2 Take the bijection $e:m\to I_H$ of [F2], with $\iota(m)=H+1$. By separation from $m\times T$, form the subset of pairs $(j,n)$ satisfying $n=4e(j)+2$. For each $j\in m$, step 2.1 gives $4e(j)+2\in T$. The rule determines one value, so the subset is the graph of a function $f:m\to T$. [F2, F3, F8, F10, step 2.1]

4.1 If $f(j)=f(j')$, step 1.2 gives $e(j)=e(j')$, and injectivity of $e$ gives $j=j'$. For every $n\in T$, step 3.1 gives a $k\in I_H$ with $n=4k+2$. Surjectivity of $e$ gives a $j\in m$ with $e(j)=k$, so $f(j)=n$. Hence $f$ is a bijection, making $m$ the number of elements of $T$. Since $\iota(m)=H+1=4{,}194{,}304$ and the embedding is injective, $m$ is the natural number $4{,}194{,}304$. [F1, F2, F5, F9, F10, step 1.2, step 3.1, step 3.2] ∎

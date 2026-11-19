---
title: The mixed-parity lattice count
status: draft
research_item: def-euler-mixed-lattice-count
dependency_level: 1
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §4, definition preceding Lemma 4.1
---

PDF p. 4: ` §4, definition preceding Lemma 4.1 `

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [lem-square-residue-parity](item-lem-square-residue-parity)
- [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-function](https://alphabetamath.cc/item/def-function)


## Definition

Let $\mathbb Z^2=\mathbb Z\times\mathbb Z$ be the set of ordered pairs of integers. The first and second entries are distinguished, and each entry retains its sign. Write $z^2=z\cdot z$. An integer is even if it has the form $2k$ and odd if it has the form $2k+1$, with $k$ an integer. Two integers have opposite parity when one is even and the other is odd.

For a real number $t\ge 0$, define
$$S_t=\{(x,y)\in\mathbb Z^2:x,y\text{ have opposite parity and }x^2+y^2\le t\},\qquad N_{\mathrm{mix}}(t)=\#S_t.$$

The comparison with $t$ uses the real order, in which $a\le b$ means $a=b$ or $b-a$ is positive. In that comparison each integer $k$ denotes the real represented by the constant rational sequence with value $k/1$. For a finite set $S$, $\#S$ denotes its cardinality, the number of distinct elements of $S$.

## Definition references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)

[math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)

[math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[lem-square-residue-parity](item-lem-square-residue-parity)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

## Justification

The even and odd conditions classify every integer uniquely because division by $2$ gives exactly one remainder, either $0$ or $1$ ([lem-square-residue-parity](item-lem-square-residue-parity)). Step 1.1 establishes that $S_t$ exists, and Steps 2.1–7.1 show that its cardinality is finite and unique.

## Facts & Assumptions

[F1] The Cartesian product consists of all ordered pairs of elements of its two factors ([math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product), [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)). Two ordered pairs are equal exactly when both corresponding entries are equal ([math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)). Separation takes the elements of a given set that satisfy a specified condition and forms a subset ([math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)). Bounded set-builder notation names the resulting subset uniquely ([math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)).

[F2] The forms $2k$ and $2k+1$ assign each integer exactly one parity ([lem-square-residue-parity](item-lem-square-residue-parity)).

[F3] The specified integer arithmetic and order make the integers a totally ordered ring ([math:def-int-operations](https://alphabetamath.cc/item/def-int-operations), [math:def-int-order](https://alphabetamath.cc/item/def-int-order), [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)). The reals form a totally ordered field ([math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)). In either structure, translation preserves inequalities and products of positive elements are positive. The inclusion of integers into the reals preserves arithmetic, and an inequality between integers holds exactly when it holds between their real images ([math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat), [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)).

[F4] The integer part of a real $s$ is the unique integer $m$ with $m\le s<m+1$ ([math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)).

[F5] In the von Neumann construction the natural numbers are sets, with $0=\varnothing$ and successor $n\cup\{n\}$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)). The map $\iota(n)=[(n,0)]$ identifies the natural numbers in order with the nonnegative integers ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)). A natural number $K$ consists of the natural numbers strictly below $K$ ([math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)) and is a finite set of cardinality $K$ ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)).

[F6] Every subset of a finite set is finite ([math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)). A bijection assigns one target element to each input and attains each target element exactly once ([math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)). Finiteness transfers across a bijection, and the cardinality of a finite set is uniquely determined ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)). A subset of $A\times B$ is the graph of a function from $A$ to $B$ when each $a\in A$ has exactly one partner $b\in B$ ([math:def-function](https://alphabetamath.cc/item/def-function)).

[F7] For a positive integer $b$, each integer $d$ has unique integers $q,r$ with $d=bq+r$ and $0\le r<b$ ([math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

## Proof

**Given:** A real number $t\ge 0$ and the membership condition defining $S_t$.

**Goal:** Show that the condition defines a finite set and thus a unique value of $N_{\mathrm{mix}}(t)$.

1.1 Each pair in $\mathbb Z^2$ has uniquely specified entries. The parity conditions and the square-sum comparison therefore determine membership from those entries, and Separation gives the subset $S_t$ of $\mathbb Z^2$. The bounded set-builder expression in the Definition denotes this unique subset. [F1, F2, F3]

2.1 Apply the integer part result to $s=t+1$ and set $B=m+1$, so $B>t+1\ge 1$. If $(x,y)\in S_t$, both squares are nonnegative. A zero entry has square zero, and for a nonzero entry either it or its negative is positive and has the same square. Consequently $x^2\le t$ and $y^2\le t$. [F3, F4, step 1.1]

3.1 If either entry $z$ lies outside $-B\le z\le B$, then one of $z,-z$, denoted $w$, satisfies $w>B>t+1\ge 1$. Now $w(w-1)\ge 0$, so $z^2=w^2=w+w(w-1)\ge w>t$, contradicting Step 2.1. Hence both entries lie between $-B$ and $B$. [F3, step 2.1]

4.1 Set $b=2B+1$, which is positive since $B>1$ by Step 2.1. For $(x,y)\in S_t$ put $a=x+B$ and $r=y+B$. Then $0\le a\le b-1$ and $0\le r<b$. The integer $d=ba+r$ satisfies $0\le d<b(a+1)\le b^2$. Let $K$ be the natural number with $\iota(K)=b^2$. Each such $d$ equals $\iota(c)$ for a unique natural number $c<K$, so $c$ belongs to the finite set $K$. [F3, F5, step 2.1, step 3.1]

5.1 By Separation, let $C$ be the subset of the von Neumann natural number $K$ consisting of the codes of pairs in $S_t$ from Step 4.1. If two pairs have the same code $c$, they have the same integer $d=\iota(c)$. Uniqueness of quotient and remainder with divisor $b>0$ gives the same $a$ and $r$, so subtracting $B$ from each recovers the same $x$ and $y$. The pairs are equal. Thus every $c\in C$ codes exactly one pair in $S_t$. [F1, F3, F5, F7, step 4.1]

6.1 Separate within $C\times S_t$ the ordered pairs $(c,p)$ for which $c$ is the code of $p$ in Step 4.1. By Step 5.1, each $c\in C$ has exactly one partner $p\in S_t$, so this graph defines a function $f:C\to S_t$. If two codes have the same value under $f$, they both code the same pair and hence are equal by uniqueness in Step 4.1. Thus $f$ is injective. Each $p\in S_t$ has a code in $C$ and is the value at that code, so $f$ is surjective and therefore bijective. [F1, F6, step 4.1, step 5.1]

7.1 The set $C$ is finite as a subset of $K$. The bijection $f:C\to S_t$ transfers finiteness to $S_t$, so $\#S_t$ exists and is unique. This defines $N_{\mathrm{mix}}(t)$ for every real $t\ge 0$. [F5, F6, step 5.1, step 6.1] ∎

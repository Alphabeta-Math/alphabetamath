---
title: Finite-set recurrence for the uncovered indices
status: published
research_item: alg-euler-finite-unrepresented-recurrence
dependency_level: 4
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, initialization and update in equation (7.3)
---

PDF p. 7: ` §7, initialization and update in equation (7.3) `

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)
- [def-author-c74aeff6099d-bounded-integer-indices](item-def-author-c74aeff6099d-bounded-integer-indices)
- [def-euler-finite-first-summand-indices](item-def-euler-finite-first-summand-indices)
- [math:def-set-difference-and-symmetric-difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)
- [math:def-axiom-of-extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)
- [math:def-power-set](https://alphabetamath.cc/item/def-power-set)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [lem-finite-deletions-and-translated-support](item-lem-finite-deletions-and-translated-support)


## Definition

The input is an integer $a$ with $1\le a\le313$ and $a\equiv1\pmod4$, meaning $a-1=4m$ for some integer $m$. Write $m=(a-1)/4$ for this integer quotient. Here $x-y=x+(-y)$.

Use $H=4{,}194{,}303$ and the finite-range indicators $\varepsilon_j$, with one specified value $0$ or $1$ at each integer $0\le j\le H$ and value $0$ when $j<0$. For a nonnegative integer $B$, let $I_B$ be the finite set of integers from $0$ through $B$, including both endpoints. Use the eligible first indices $J=\{i\in I_{78}:\varepsilon_i=1\}$, with possible first summand $4i+1$ at index $i$.

1. Start with $C=C_0=I_H=\{0,1,\ldots,H\}$.
2. Scan the integers $i=0,\ldots,m$ in increasing order. At an index $i\in J$, replace $C$ by $C\setminus\{k\in I_H:i\le k,\ \varepsilon_{k-i}=1\}$. The set difference $C\setminus E$ keeps exactly the elements of $C$ outside $E$. At an index outside $J$, leave $C$ as it is.
3. Return the resulting finite subset $C(a)$ of $I_H$. In other words, all its elements belong to $I_H$ and they can be listed once each in a list of natural-number length.

## Definition references

[Integers](https://alphabetamath.cc/item/def-integers)

[Integer order](https://alphabetamath.cc/item/def-int-order)

[Integer arithmetic](https://alphabetamath.cc/item/def-int-operations)

[Congruence modulo an integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[Finite-range indicators](item-def-euler-finite-certificate-indices)

[Bounded integer index sets](item-def-author-c74aeff6099d-bounded-integer-indices)

[Eligible first-summand indices](item-def-euler-finite-first-summand-indices)

[Set difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference)

[Subsets](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[Finiteness](https://alphabetamath.cc/item/def-finite-cardinality)

## Justification

The proof below verifies the cutoff quotient and constructs one deletion set at each scan position. The [finite deletion lemma](item-lem-finite-deletions-and-translated-support) then gives a unique finite output from $I_H$.

## Facts & Assumptions

[F1] [Division with remainder](https://alphabetamath.cc/item/thm-division-algorithm-in-z) gives a unique integer quotient and remainder for any integer dividend and positive integer divisor, with remainder at least zero and less than the divisor.

[F2] The [integer operations](https://alphabetamath.cc/item/def-int-operations) give addition, negation and multiplication. The [ordered-ring laws for the integers](https://alphabetamath.cc/item/thm-int-ordered-ring) give the usual additive inverses and distributivity, allow addition of the same integer to both sides of an inequality, and make a product of positive integers positive. The integer order is total.

[F3] The [natural numbers](https://alphabetamath.cc/item/def-natural-numbers) are $0,1,2,\ldots$, with $1=0^+$, where $t^+$ denotes the natural successor of $t$. The recursion for [natural-number addition](https://alphabetamath.cc/item/def-nat-addition) gives $t+0=t$ and $t+u^+=(t+u)^+$, so $t+1=t^+$. In the [natural order](https://alphabetamath.cc/item/def-nat-order), $s\le t$ means that $s+u=t$ for some natural number $u$. By [discreteness of natural order](https://alphabetamath.cc/item/lem-nat-discrete), $t<r$ if and only if $t^+\le r$. The [canonical map](https://alphabetamath.cc/item/lem-nat-embeds-int) $\iota:\mathbb N\to\mathbb Z$ is injective, has image the nonnegative integers, preserves addition, and preserves and reflects order. The [integer zero and one](https://alphabetamath.cc/item/def-int-operations) are $\iota(0)$ and $\iota(1)$.

[F4] For every nonnegative integer $B$, the [bounded index set](item-def-author-c74aeff6099d-bounded-integer-indices) $I_B$ is finite and contains exactly the integers from $0$ through $B$. The [certificate definition](item-def-euler-finite-certificate-indices) gives a unique binary value $\varepsilon_t$ at each integer $t\le H$. The [definition of $J$](item-def-euler-finite-first-summand-indices) selects exactly the indices in $I_{78}$ with indicator $1$.

[F5] [Separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation) selects exactly the elements of an existing set satisfying a specified condition. [Extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality) identifies sets with the same elements. The [power set](https://alphabetamath.cc/item/def-power-set) $\mathcal P(I_H)$ consists of all subsets of $I_H$. The [Cartesian product](https://alphabetamath.cc/item/def-cartesian-product) $L\times\mathcal P(I_H)$ consists of the ordered pairs $(j,E)$ with $j\in L$ and $E\subseteq I_H$. An [indexed family on $L$](https://alphabetamath.cc/item/def-indexed-family) is a [function](https://alphabetamath.cc/item/def-function) assigning exactly one value to each index in $L$.

[F6] The [finite deletion lemma](item-lem-finite-deletions-and-translated-support) gives a unique sequence $C_0,\ldots,C_r$ of finite subsets from any finite starting set $C_0$ of integers and family $(E_j)_{1\le j\le r}$ of sets of integers with $r$ natural. Its update is $C_{t^+}=C_t\setminus E_{t^+}$ for $0\le t<r$. By the [definition of difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference), deletion of an empty set leaves membership unchanged.

[F7] By the [definitions of injection, surjection and bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection), a function is injective when equal values have equal inputs, surjective when every element of its codomain is a value, and bijective when it is both.

## Proof

**Given:** An integer $a$ satisfying the stated bounds and congruence, and the fixed data $H$, $\varepsilon_j$ and $J$.

**Goal:** Show that the procedure specifies a unique finite output at every allowed cutoff.

1.1 The congruence supplies an integer $m$ with $a-1=4m$, so division of $a-1$ by the positive integer $4$ has remainder zero and unique quotient $m$. The bounds on $a$ give $0\le4m\le312=4\cdot78$. If $x<y$ are integers, then $4(y-x)>0$, so $4x<4y$. By totality, the bounds on $4m$ imply $0\le m\le78$. [given, F1, F2]

2.1 Let $r$ be the unique natural number with $\iota(r)=m+1$, and let $L=\{j\in\mathbb N:1\le j\le r\}$, obtained by separation in the naturals. For each $j\in L$, order preservation gives $1\le\iota(j)\le m+1$, so $i=\iota(j)-1$ belongs to $I_m$. The pairs $(j,i)$ with $i=\iota(j)-1$ form the graph of a function $f:L\to I_m$ by separation in $L\times I_m$, since there is exactly one value for every $j\in L$. For each $i\in I_m$ we have $1\le i+1\le m+1$. Then $i+1$ has a unique natural preimage under $\iota$, and order reflection puts that preimage in $L$. Adding $1$ to $f(j)=i$ gives $\iota(j)=i+1$, so this preimage is the only $j\in L$ with $f(j)=i$. Every $i\in I_m$ has a preimage, giving surjectivity, and uniqueness gives injectivity. Thus $f$ is a bijection. If $j<j'$ in $L$, order preservation and injectivity give $\iota(j)<\iota(j')$. Subtracting $1$ preserves this strict inequality by order compatibility and additive cancellation. Hence $f$ is increasing, with $f(1)=0$ and $f(r)=m$. [step 1.1, F2, F3, F4, F5, F7]

3.1 For $0\le t<r$ in the naturals put $j=t^+$. Then $j\le r$ by discreteness. Since $\iota(j)=\iota(t+1)=\iota(t)+1\ge1$, order reflection gives $1\le j$, so $j\in L$. The scan position for this update is $i=\iota(j)-1=\iota(t)$. Conversely, for any $j\in L$, put $i=\iota(j)-1$ and take the unique natural $t$ with $\iota(t)=i$. Then $\iota(t^+)=i+1=\iota(j)$, so $t^+=j$ by injectivity and $t<r$ by discreteness. Therefore the successive updates advance the integer index by one, starting at $i=0$ and ending at $i=m$. [step 2.1, F2, F3]

3.2 For $j\in L$ put $i=\iota(j)-1$. For all $k\in I_H$ we have $k-i\le k\le H$ because $i\ge0$. Thus $\varepsilon_{k-i}$ is defined, including its zero value if $k<i$. By separation and extensionality there is exactly one subset $E_j$ of $I_H$ containing precisely those $k\in I_H$ for which $i\in J$, $i\le k$ and $\varepsilon_{k-i}=1$. Separating the pairs $(j,E)$ with this defining condition on $E$ inside $L\times\mathcal P(I_H)$ gives the indexed family $(E_j)_{j\in L}$, since each $j$ has exactly one such $E$. [step 2.1, F2, F4, F5]

4.1 Apply the finite deletion lemma with starting set $I_H$ and the family from step 3.2. At the update $C_{t^+}=C_t\setminus E_{t^+}$ the integer index is $i=\iota(t)$ by step 3.1. For $i\in J$ this is the stipulated deletion, and for $i\notin J$ the set $E_{t^+}$ is empty, so the difference leaves the current set unchanged. Since $4i+1\le a$ is equivalent to $i\le m$ by step 1.1 and $a=4m+1$, the scan performs precisely the updates for $i\in J$ with $i\le m$, in increasing order, and returns $C_r$, the unique finite subset left after the $r$ scan positions. When $a=313$, $m=78$, so the scan includes every index in $J$. [step 1.1, step 3.1, step 3.2, F2, F4, F5, F6] ∎

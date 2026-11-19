---
title: Splitting an odd integer by prime class
status: draft
research_item: lem-euler-odd-factor-split
dependency_level: 2
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, Lemma 2.1, first sentence of the proof
---

PDF p. 1: ` Lemma 2.1, first sentence of the proof `

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)
- [math:thm-int-comm-ring](https://alphabetamath.cc/item/thm-int-comm-ring)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:cor-euclids-lemma-for-finite-products](https://alphabetamath.cc/item/cor-euclids-lemma-for-finite-products)
- [math:def-symmetric-group](https://alphabetamath.cc/item/def-symmetric-group)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:lem-nat-add-commutative](https://alphabetamath.cc/item/lem-nat-add-commutative)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)


## Statement

Every positive odd integer $m$ has a factorization $m=gm_0$ into positive integers $g$ and $m_0$ such that $g\in\mathcal A$ and every prime divisor of $m_0$ belongs to $\mathcal P_3$.

Here $\mathbb Z$ denotes the integers, positivity means being greater than $0$, and odd means not divisible by $2$. A factorization is an equality expressing an integer as a product. An integer $d$ divides $a$, written $d\mid a$, if $a=dq$ for some $q\in\mathbb Z$. A prime divisor of $a$ is a prime $p$ with $p\mid a$, where a prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Congruence $x\equiv r\pmod 4$ means $4\mid(x-r)$. The set $\mathcal A$ consists of positive integers all of whose prime divisors are congruent to $1$ modulo $4$, and $\mathcal P_3$ consists of primes congruent to $3$ modulo $4$.

## Statement references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[def-euler-prime-classes](item-def-euler-prime-classes)

## Facts & Assumptions

[F1] For integers $a,b$ with $b>0$, there are unique integers $q,r$ with $a=bq+r$ and $0\le r<b$. The same supplier proves under “Discreteness” that every positive integer is at least $1$. [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

[F2] Every integer $n\ge 1$ is the product of a finite list of primes. The first numbered step of that theorem’s proof establishes $0<1$. [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)

[F3] For sets $D$ and $C$, a formula that specifies exactly one value in $C$ for each index in $D$ defines a function $D\to C$. [math:def-function](https://alphabetamath.cc/item/def-function) Separation in the Cartesian product $D\times C$ gives the set of pairs prescribed by the rule. The output graph variable is fresh in each assignment rule. [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation) [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product) [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) A finite product of integers starts at $1$ and multiplies by each entry successively, so the product of a list with no entries is $1$. For a list of integers of length $n$, assign its original entry at every index in $n$ and assign $1$ at every other natural index. This gives an extension on $\mathbb N$, and the product is independent of the extension because only the entries in $n$ affect its value. [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)

[F4] Integer addition and multiplication obey the commutative ring laws, in particular distributivity, associativity, commutativity and the identity laws for $0$ and $1$. The integer order is total, compatible with addition, and closed under multiplication of positive integers. [math:thm-int-comm-ring](https://alphabetamath.cc/item/thm-int-comm-ring) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[F5] A permutation of the indices preserves the product of a finite list in a commutative monoid, and splitting a list at any position gives the product of the two consecutive parts. For lengths $a,b$, the split is the product of the first $a$ entries times the product of the entries at positions $a+j$ for $j<b$. Integer multiplication is closed, associative and commutative with two-sided identity $1$ by [F4], so $(\mathbb Z,\cdot,1)$ is a commutative monoid. [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid) The rules apply to finite integer lists using the extension in [F3]. [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)

[F6] If a prime divides the product of a finite list of integers, it divides some entry of the list. This implication includes the empty list, so no prime divides its product $1$. [math:cor-euclids-lemma-for-finite-products](https://alphabetamath.cc/item/cor-euclids-lemma-for-finite-products)

[F7] The definitions of $\mathcal A$ and $\mathcal P_3$ impose the conditions on prime divisors and prime congruence stated above. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-prime](https://alphabetamath.cc/item/def-prime) [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z) [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[F8] A permutation of an index set is a bijection from that set to itself. [math:def-symmetric-group](https://alphabetamath.cc/item/def-symmetric-group) A bijection is an injective and surjective function. [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)

[F9] Induction on the natural numbers starts at $0$ and passes from each number to its successor. [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F10] A list of natural length $n$ is indexed by the von Neumann natural $n$. Here $0=\varnothing$, $1=\{0\}$ and the successor is $\sigma(n)=n\cup\{n\}$. [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) In the natural order, $i\le n$ means $i+d=n$ for some natural $d$, and $i<n$ means $i\le n$ and $i\ne n$. [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) For natural numbers $i,n$, one has $i<n$ exactly when $i\in n$, and $i\le n$ exactly when $i\subseteq n$. If $n\ne 0$, then $0\in n$. [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership) Inclusion $D\subseteq E$ means that every element of $D$ is an element of $E$. [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[F11] Natural-number addition satisfies $a+0=a$ and $a+\sigma(b)=\sigma(a+b)$, and it is commutative. [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:lem-nat-add-commutative](https://alphabetamath.cc/item/lem-nat-add-commutative)

## Proof

**Given:** A positive integer $m$ with $2\nmid m$.

**Goal:** Find positive integers $g,m_0$ with $m=gm_0$, $g\in\mathcal A$ and every prime divisor of $m_0$ in $\mathcal P_3$.

1.1 Since $m\ge 1$ by [F1], take a list $p_0,\ldots,p_{N-1}$ of primes with product $m$ by [F2]. If the list has an index $i$, then $N\ne 0$ and $0\in N$ by [F10]. The map $\tau$ exchanges $0$ and $i$ and fixes every other position, with $\tau$ the identity if $i=0$. This assigns exactly one image in $N$ to each position, so [F3] gives a map $N\to N$. Applying it twice fixes every position. Hence equal images give equal inputs by applying $\tau$ once more, and each position $j$ has preimage $\tau(j)$. These are the two criteria in [F8], so $\tau$ is a permutation. Since $0\in N$, the only element of $1=\{0\}$ belongs to $N$. Thus $1\subseteq N$ and $1\le N$ by [F10], so the natural order gives a length $b$ with $1+b=N$. By [F5], reordering by $\tau$ and splitting after the first entry gives $m=p_i v$, where $v$ is the product of the remaining entries. If $2\mid p_i$, write $p_i=2u$ for an integer $u$. Then $m=2(uv)$, contradicting $2\nmid m$. Thus $2\nmid p_i$ for every index $i$. [given, F1, F2, F3, F4, F5, F7, F8, F10]

2.1 For each entry $p$, divide by $4$ to write $p=4q+r$ with $0\le r<4$. The bound that every positive integer is at least $1$ gives $x+1\le y$ whenever $x<y$, by applying it to $y-x$. Consequently the integers in this remainder range are $0,1,2,3$. If $r$ is $0$ or $2$, then $p$ equals $2(2q)$ or $2(2q+1)$ respectively, which step 1.1 excludes. Thus $r$ is $1$ or $3$, and $p\equiv r\pmod 4$ since $p-r=4q$. [step 1.1, F1, F4, F7]

3.1 Induct on $k$ to show that, whenever $k\le N$, there are two lists of indices whose lengths sum to $k$ and that contain every index below $k$ exactly once in the list for its remainder, with no other entries. At $k=0$ use two empty lists. If $\sigma(k)\le N$, then $\sigma(k)\subseteq N$ by [F10]. The successor $\sigma(k)=k\cup\{k\}$ contains $k$, so inclusion gives $k\in N$ and hence $k<N$. The lists for $k$ therefore exist by the induction hypothesis. The index $k$ is absent from both lists and step 2.1 assigns it to exactly one of them. To append the index, let $a$ be the current length of the list receiving it. Since $a<a$ is false, we have $a\notin a$ by [F10]. On $\sigma(a)=a\cup\{a\}$, keep the old value on each position in $a$ and put $k$ at position $a$. Every position has exactly one value in $N$, so [F3] gives the extended list. The sum of the lengths rises from $k$ to $\sigma(k)$ by [F11], using commutativity if the first list is the one extended. This proves the assertion at $\sigma(k)$, and [F9] gives the lists at $k=N$. [step 2.1, F3, F9, F10, F11]

4.1 Let $a,b$ be the lengths of the two lists in step 3.1, so $a+b=N$. By bounded induction as in step 3.1, start with the first list at $j=0$. If $\sigma(j)\le b$, then $j\in b$ by the successor and inclusion argument of step 3.1. Append the second list's entry at $j$ to the current list of length $a+j$ using the same function construction. The new entry goes at position $a+j$, every previous entry keeps its position, and the length becomes $\sigma(a+j)=a+\sigma(j)$. At $j=b$ the concatenation has length $N$, and for every $j<b$ the second list's entry at $j$ occurs at position $a+j$. [step 3.1, F3, F9, F10, F11]

5.1 Each index in $N$ occurs exactly once in the concatenation by step 3.1, so the map from positions to entries is injective by absence of repetitions and surjective because every index occurs. By [F8] it is a permutation of $N$. For each of the two index lists, assigning the prime $p_i$ to the position storing $i$ gives a list of integers by [F3]. Let $g$ and $m_0$ be the products of these two lists of primes, respectively. Reorder the prime list using this permutation and apply the split in [F5] with lengths $a,b$. By step 4.1 the factors are exactly $g,m_0$, so $m=gm_0$, including when either list is empty. [step 1.1, step 3.1, step 4.1, F3, F5, F8]

6.1 For either list of prime entries, the empty prefix has product $1>0$ by [F2] and [F3]. If a prefix product is positive and another entry remains, the next prefix product is that product times a prime, which is positive by [F7]. Closure of the positive integers under multiplication in [F4] makes the next product positive as well. Induction by [F9] gives positivity through the full length of each list, so $g$ and $m_0$ are positive. [step 5.1, F2, F3, F4, F7, F9]

7.1 If a prime $s$ divides $g$, then [F6] gives an entry $p$ of the first list with $s\mid p$. Since $s>1$ and $p$ is prime, $s=p$. Step 2.1 therefore gives $s\equiv1\pmod 4$. For any prime $s$ dividing $m_0$, [F6] gives an entry of the second list divisible by $s$, and the same divisor condition forces $s$ to be that entry, with $s\equiv3\pmod 4$. Thus $g\in\mathcal A$, and every prime divisor of $m_0$ is in $\mathcal P_3$. Together with the product identity and positivity, this gives the required factorization. [step 2.1, step 5.1, step 6.1, F6, F7] ∎

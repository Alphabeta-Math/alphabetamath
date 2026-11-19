---
title: A small obstructing divisor suffices in the finite range
status: published
research_item: lem-euler-finite-small-obstructing-divisor
dependency_level: 3
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, proof of Lemma 7.1, first four sentences
---

PDF p. 7: ` Lemma 7.1, proof, multiplicity, size, and least-prime observation `

## Prerequisites

- [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-nat-power](https://alphabetamath.cc/item/def-nat-power)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)
- [math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)
- [lem-odd-prime-factor-parity](item-lem-odd-prime-factor-parity)
- [math:thm-reals-cauchy-complete](https://alphabetamath.cc/item/thm-reals-cauchy-complete)
- [math:lem-of-square-monotone](https://alphabetamath.cc/item/lem-of-square-monotone)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-symmetric-group](https://alphabetamath.cc/item/def-symmetric-group)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)


## Statement

Set $H=2^{22}-1=4{,}194{,}303$. Let $j$ be an integer with $0\le j\le H$ and set $u=4j+1$. For a nonnegative integer base, a power with positive integer exponent denotes repeated multiplication. Then $u$ is positive and odd (not divisible by $2$), $u\equiv1\pmod4$, and $u\le64^4-3$.

Here $d\mid a$ means $a=dq$ for some integer $q$, and $a\equiv b\pmod4$ means $4\mid(a-b)$. A prime is an integer greater than $1$ with only $1$ and itself as positive divisors. Let $\mathcal P_3$ be the set of primes congruent to $3$ modulo $4$. A prime factorization is a finite list of primes with product $u$. The empty list has product $1$. The multiplicity of a prime is its number of occurrences in this list. The number of occurrences from a class of primes is the finite cardinality of the set of positions whose entries belong to that class. The total number of occurrences of primes in $\mathcal P_3$, viewed as a nonnegative integer, is even, meaning it is divisible by $2$.

If any prime in $\mathcal P_3$ divides $u$, there are at least two such occurrences and some $p\in\mathcal P_3$ satisfies $p\mid u$ and $p\le\sqrt{u}<4096$. Here $\sqrt{u}$ is the unique nonnegative real number with square $u$, using the usual copy of the integers in the reals.

## Statement references

[def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-nat-power](https://alphabetamath.cc/item/def-nat-power)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)

[math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)

[math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

## Facts & Assumptions

[F1] The finite certificate uses $H=2^{22}-1=4{,}194{,}303$ ([def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)). Natural-number powers start with $1$ and multiply by the base once per increase of the exponent ([math:def-nat-power](https://alphabetamath.cc/item/def-nat-power)). The nonnegative integers are the images of the natural numbers under the map preserving addition, multiplication, and order ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)).

[F2] In the integers, addition preserves order and products of positive numbers are positive. Integer addition and multiplication are associative and commutative, multiplication distributes over addition, and $1$ is the multiplicative identity ([math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)). There is no natural number strictly between $0$ and $1$, so each positive integer is at least $1$ by the natural-number embedding in [F1] ([math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)). If one natural number is strictly less than another, its successor is at most the other ([math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)). The natural numerals $1$ and $2$ are the first two successors of $0$, so $2$ is the successor of $1$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)).

[F3] The divisibility, congruence, and primality conditions in the statement are the integer definitions ([math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z), [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer), [math:def-prime](https://alphabetamath.cc/item/def-prime)). They give exactly the prime class $\mathcal P_3$ defined in [def-euler-prime-classes](item-def-euler-prime-classes). For division of an integer by a positive integer $b$, the expression $bq+r$ with integers $q,r$ and $0\le r<b$ is unique, and divisibility by $b$ is equivalent to remainder zero ([math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

[F4] Every integer at least $1$ has a prime factorization, unique up to reordering ([math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)). A permutation of the position set $m$ is a bijection $m\to m$ ([math:def-symmetric-group](https://alphabetamath.cc/item/def-symmetric-group)). A finite integer product starts at $1$ and multiplies by one entry at a time ([math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)). It can be split into blocks or reordered without changing the value because multiplication is associative and commutative with identity $1$ ([math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)).

[F5] For a positive odd integer $u$ congruent to $1$ modulo $4$, the number of prime factor occurrences congruent to $3$ modulo $4$ is even. If such a prime divides $u$, some such prime divisor is at most $\sqrt{u}$ ([lem-odd-prime-factor-parity](item-lem-odd-prime-factor-parity)).

[F6] The real numbers $\mathbb{R}$ with the real order form a totally ordered field ([math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field), [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)). Every nonempty set of reals bounded above has a least upper bound ([math:thm-reals-cauchy-complete](https://alphabetamath.cc/item/thm-reals-cauchy-complete)). A least upper bound is the smallest real number at least as large as every member of the set, so the real field is complete in the least-upper-bound sense ([math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)). Thus every nonnegative real $x$ has a unique nonnegative square root, a real $s$ with $s^2=x$ ([math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots)). For nonnegative members of an ordered field, $a^2<b^2$ implies $a<b$ ([math:lem-of-square-monotone](https://alphabetamath.cc/item/lem-of-square-monotone)). The integer copy in the reals is obtained by mapping an integer $m$ first to the rational $m/1$, then to its real image given by the constant rational sequence. Both maps preserve arithmetic and order ([math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat), [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)).

[F7] For a list of length $m$, the positions are the natural numbers strictly below $m$. They form the finite set $m$ of its predecessors. Every subset of this set is finite ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality), [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)). A membership condition on the positions defines a unique subset by separation ([math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)). Finite cardinality is natural-valued, is zero exactly for the empty set, and is preserved by a bijection ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)). A map is a bijection when it sends distinct elements to distinct images and every element of the codomain is an image ([math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)).

## Proof

**Given:** An integer $j$ with $0\le j\le H$ and $u=4j+1$.

**Goal:** Establish the congruence and size of $u$, the even multiplicity count, and the small prime divisor whenever the class occurs.

1.1 Since $j\ge0$, multiplication by $4$ and addition of $1$ give $u\ge1$. The equation $u-1=4j$ gives $u\equiv1\pmod4$. Also $u=2(2j)+1$ has remainder $1$ on division by $2$, since $0\le1<2$. Hence $u$ is odd. [given, F2, F3]

2.1 From $j\le H$ we get $u\le4H+1$. The power computations $64\cdot64=4096$ and $4096\cdot4096=16{,}777{,}216=4\cdot4{,}194{,}304$ give $64^4=4096^2=4(H+1)$. Therefore $4H+1=64^4-3<4096^2$. Let $e$ denote the integer embedding into $\mathbb{R}$ from [F6]. In the ordered field $\mathbb{R}$, $e(u)$ and $e(4096)$ are nonnegative by order preservation, with $e(4096^2)=e(4096)^2$ by preservation of multiplication. Thus the two nonnegative real numbers $\sqrt{e(u)}$ and $e(4096)$ have squares satisfying $(\sqrt{e(u)})^2=e(u)<e(4096)^2$. Strict comparison of squares gives $\sqrt{e(u)}<e(4096)$, which is $\sqrt{u}<4096$ in the notation of the statement. [given, F1, F2, F6, step 1.1]

2.2 Factor $u$ into primes $p_i$ for $0\le i<m$ using $u\ge1$. By separation from the finite position set, form $S$ of exactly those $i$ with $p_i\in\mathcal P_3$. The subset $S$ is finite, so $k=|S|$ is a natural number. For any other prime factorization with entries $q_i$, uniqueness gives the same length $m$ and a permutation $\pi$ of the position set with $q_i=p_{\pi(i)}$. A position $i$ in the second list qualifies exactly when $\pi(i)\in S$. Since $\pi$ is a bijection of the position set, its restriction to the qualifying positions of the second list is one-to-one and covers $S$ because the preimage of each element of $S$ qualifies. It is therefore a bijection and the two counts agree. Apply the parity lemma to the positive odd integer $u\equiv1\pmod4$ to obtain that $k$ is even. [F3, F4, F5, F7, step 1.1]

3.1 A prime appearing in the list divides $u$ by regrouping it as the first factor. Conversely, if a prime $q$ divides $u$, write $u=qv$ with $v$ an integer. Since $q>1$ and $u>0$, the integer $v$ is positive and hence at least $1$. Indeed, $v=0$ would give $u=0$, and $v<0$ would make $-u=q(-v)>0$. Factor $v$ and put $q$ first to give a prime list for $u$. Uniqueness up to reordering forces $q$ to occur in the list used in step 2.2. [F2, F3, F4, step 1.1, step 2.2]

4.1 If a prime in $\mathcal P_3$ divides $u$, step 3.1 shows that $S$ is nonempty, so $k>0$. Discreteness at $0$ gives $k\ge1$. The integer image of $k$ is divisible by $2$, whereas $1$ has remainder $1$ on division by $2$. Hence $k\ne1$, so $1<k$. Discreteness at $1$ then gives $2\le k$, as $2$ is the successor of $1$. With the same positive odd $u\equiv1\pmod4$ and the assumed prime divisor, the parity lemma supplies a prime $p\in\mathcal P_3$ dividing $u$ with $p\le\sqrt{u}$. The bound from step 2.1 gives $p\le\sqrt{u}<4096$, completing the claim. [F1, F2, F3, F5, F7, step 1.1, step 2.1, step 2.2, step 3.1] ∎

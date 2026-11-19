---
title: The two-square representation count and divisor-factor maximum
status: published
research_item: def-euler-two-square-counts
dependency_level: 1
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 5, §4, definitions of M(n) and r₂(u) immediately before Lemma 4.2
---

PDF p. 5: ` §4, definitions of M(n) and r₂(u) on the first lines `

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [def-author-fb1ef6c2c01b-signed-ordered-two-square-count](item-def-author-fb1ef6c2c01b-signed-ordered-two-square-count)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-p-adic-valuation](https://alphabetamath.cc/item/def-p-adic-valuation)
- [math:lem-p-adic-valuation-basic](https://alphabetamath.cc/item/lem-p-adic-valuation-basic)
- [math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound)
- [math:def-int-abs](https://alphabetamath.cc/item/def-int-abs)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:thm-nat-linear-order](https://alphabetamath.cc/item/thm-nat-linear-order)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)


## Definition

Let $u$ and $n$ be positive integers, meaning elements of $\mathbb Z$ greater than $0$. The signed, ordered count $r_2(u)$ counts pairs of integers $(x,y)$ with $x^2+y^2=u$, allowing either sign and zero in each coordinate and retaining the order of the coordinates.

Write $d\mid u$ when $u=dk$ for some integer $k$, and $d\nmid u$ when this fails. A prime $q$ is an integer greater than $1$ whose only positive divisors are $1$ and $q$. The congruence $q\equiv1\pmod4$ means $4\mid(q-1)$. For a prime $q$ and a positive integer exponent $e$, write $q^e\parallel u$ when $q^e\mid u$ and $q^{e+1}\nmid u$. The natural powers start at $q^0=1$ and satisfy $q^{j+1}=q^j q$ for $j\ge0$.

Set
$$P(u)=\prod_{\substack{q^e\parallel u\\q\equiv1\pmod4}}(e+1),\qquad M(n)=\max_{1\le u\le n}P(u).$$
The product takes the eligible primes $q$ in increasing order. It starts at $1$ and successively multiplies by each factor $e+1$, so an empty product is $1$. The maximum is a value $P(u)$ attained at an integer $1\le u\le n$ and at least as large as every value in that range.

## Facts & Assumptions

[F1] $\mathbb Z$ is the set of integers. Its addition, multiplication, negation and total order make it a totally ordered commutative ring with multiplicative identity $1$. In particular integer multiplication is associative and $1$ is a two-sided identity, so $(\mathbb Z,\cdot,1)$ is a monoid. ([math:def-integers](https://alphabetamath.cc/item/def-integers), [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations), [math:def-int-order](https://alphabetamath.cc/item/def-int-order), [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring), [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid))

[F2] Integer divisibility means being an integer multiple. A prime exceeds $1$ and has only $1$ and itself as positive divisors. Congruence modulo $4$ means divisibility of the difference by $4$. In the monoid $(\mathbb Z,\cdot,1)$ from [F1], the natural powers of an integer $q$ start at $q^0=1$ and satisfy $q^{\sigma(j)}=q^j q$. ([math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z), [math:def-prime](https://alphabetamath.cc/item/def-prime), [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer), [math:def-group-power](https://alphabetamath.cc/item/def-group-power))

[F3] For a prime $q$ and a nonzero integer $u$, $v_q(u)$ is the greatest natural number $j$ with $q^j\mid u$. For every natural $j$, $q^j\mid u$ holds exactly when $j\le v_q(u)$, and $q\mid u$ holds exactly when $v_q(u)\ge1$. ([math:def-p-adic-valuation](https://alphabetamath.cc/item/def-p-adic-valuation), [math:lem-p-adic-valuation-basic](https://alphabetamath.cc/item/lem-p-adic-valuation-basic))

[F4] An integer divisor of a nonzero integer has absolute value at most that of the integer it divides. The absolute value of a positive integer is the integer itself. ([math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound), [math:def-int-abs](https://alphabetamath.cc/item/def-int-abs))

[F5] The natural numbers $\mathbb N$ start at $0$, with $1=\sigma(0)$. Natural addition gives $k+1=k+\sigma(0)=\sigma(k+0)=\sigma(k)$. The embedding $\iota(k)=[(k,0)]$ identifies $\mathbb N$ with the nonnegative integers. It preserves addition and order and reflects order. It sends the natural $0$ and $1$ to the integer $0$ and $1$, so $\iota(k+1)=\iota(k)+1$. On the naturals, $\le$ is total, transitive and antisymmetric, and $a<b$ means $a\le b$ and $a\ne b$. For natural $j,k$, $0\le k$, $k<k+1$, and $j<k+1$ holds exactly when $j\le k$. Induction establishes a property of all naturals by establishing it at $0$ and showing that it passes from $k$ to $k+1$. ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers), [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition), [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations), [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int), [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership), [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle), [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order), [math:thm-nat-linear-order](https://alphabetamath.cc/item/thm-nat-linear-order))

[F6] For a family $g:\mathbb N\to\mathbb Z$ in the monoid from [F1], the product of the first $m$ terms is uniquely obtained by starting at $1$ and multiplying by the next factor at each successor. ([math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product))

[F7] For positive integer $u$ the signed, ordered two-square count is the cardinality of the finite set of ordered pairs of integers whose squares sum to $u$. ([def-author-fb1ef6c2c01b-signed-ordered-two-square-count](item-def-author-fb1ef6c2c01b-signed-ordered-two-square-count))

[F8] Separation in $\mathbb N\times\mathbb Z$ forms the set of pairs satisfying a given condition. Such a set defines a function $\mathbb N\to\mathbb Z$ if each natural index occurs with exactly one integer value. ([math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product), [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation), [math:def-function](https://alphabetamath.cc/item/def-function))

## Justification

**Given:** positive integers $u$ and $n$.

**Goal:** show that the factors in $P(u)$ are uniquely specified, that $P(u)$ and $M(n)$ are well defined, and that $r_2(u)$ has the stated meaning.

1.1 For a prime $q$, apply the valuation facts to $u\ne0$. For $e\ge1$, the first divisibility condition gives $e\le v_q(u)$. The second excludes $e+1\le v_q(u)$, so totality and the definition of strict order give $v_q(u)<e+1$. The successor rule yields $v_q(u)\le e$, and antisymmetry yields $v_q(u)=e$. Conversely, when $q\mid u$, take $e=v_q(u)\ge1$. Then $e\le v_q(u)<e+1$, so $q^e\mid u$ and $q^{e+1}\nmid u$. Hence only primes dividing $u$ can contribute and each contributes with one exponent. [given, F1, F2, F3, F5]

1.2 A prime dividing $u$ satisfies $1\le q\le u$ by the positive divisor bound. Write $u=\iota(m)$ with $m\in\mathbb N$. For natural $j$, the condition $j<m$ is equivalent to $j+1\le m$. If $j<m$ and $j+1\le m$ fails, totality gives $m<j+1$. The successor rule gives $m\le j$, contradicting $j<m$. Conversely $j+1\le m$ gives $j<m$ by $j<j+1$ and transitivity. Thus for $j<m$ we have $1\le\iota(j+1)\le u$ by the embedding and $\iota(j+1)=\iota(j)+1$. The map $j\mapsto\iota(j+1)$ is strictly increasing because $\iota$ preserves strict order and addition of $1$ preserves strict order. Every integer $q$ from $1$ to $u$ occurs, since $q-1\ge0$ has a unique natural preimage $j$ and $\iota(j+1)=q$. Order reflection gives $j+1\le m$, so $j<m$. [given, F1, F2, F4, F5]

2.1 For each natural $j$, set $q=\iota(j+1)$ and assign the value $g_j=\iota(v_q(u)+1)$ if $j<m$ and $q$ is prime, divides $u$ and is congruent to $1$ modulo $4$. Assign $g_j=1$ when that test fails. Exactly one branch applies to each $j$. The valuation branch supplies one integer because $q$ is prime, $u\ne0$, and $\iota$ is defined on all naturals. The other branch supplies the single integer $1$. Separation in $\mathbb N\times\mathbb Z$ gives the set of pairs $(j,g_j)$, which defines the function $g:\mathbb N\to\mathbb Z$ by the one-value condition. In the monoid $(\mathbb Z,\cdot,1)$, apply the finite-product rule to the first $m$ terms of $g:\mathbb N\to\mathbb Z$. Each included factor occurs at its prime in increasing order, and each inserted $1$ leaves the running product unchanged. Thus this product is $P(u)$ as displayed, with value $1$ if no prime qualifies. [given, F1, F2, F3, F5, F6, F8, step 1.1, step 1.2]

3.1 Identify natural indices with their images under $\iota$ when they are arguments of $P$. Induct on the natural number $k$ with the assertion that if $k\ge1$, the list $P(1),\ldots,P(k)$ has an attained greatest value. At $k=0$ the assertion has a false hypothesis since $0<1$. At the successor, if $k<1$, the successor rule gives $k\le0$. Since $0\le k$, antisymmetry gives $k=0$, and $P(1)$ is the greatest value of the one-entry list. Otherwise totality gives $k\ge1$. A positive index $j\le k+1$ either equals $k+1$ or satisfies $j<k+1$, in which case $j\le k$ by the successor rule. Thus the index $k+1$ is the only new index by the successor rule. Comparing $P(k+1)$ with the greatest value already attained gives an attained greatest value for the enlarged list, by totality of the integer order. This proves existence for $n$ by induction, by taking the unique natural preimage of $n$ under $\iota$. [given, F1, F5, step 2.1]

4.1 Any two attained greatest values are each at least as large as the other, so antisymmetry gives uniqueness of $M(n)$. The representation-count definition gives precisely the stated $r_2(u)$ and its finite value. This establishes both quantities. [F1, F7, step 2.1, step 3.1] ∎

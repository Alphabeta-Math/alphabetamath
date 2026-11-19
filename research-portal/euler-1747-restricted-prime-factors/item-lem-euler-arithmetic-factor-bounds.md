---
title: "Lemma 5.1: Explicit bounds for the arithmetic factors"
status: published
research_item: lem-euler-arithmetic-factor-bounds
dependency_level: 5
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 5, Lemma 5.1, equation (5.1) and proof
---

PDF p. 5: ` Lemma 5.1, equation (5.1) `

## Prerequisites

- [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product)
- [math:cor-of-one-positive](https://alphabetamath.cc/item/cor-of-one-positive)
- [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)
- [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)
- [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)
- [math:def-symmetric-group](https://alphabetamath.cc/item/def-symmetric-group)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [def-euler-divisor-functions](item-def-euler-divisor-functions)
- [def-euler-two-square-counts](item-def-euler-two-square-counts)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)
- [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)
- [lem-divisors-from-prime-exponents](item-lem-divisors-from-prime-exponents)
- [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)
- [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [lem-euler-local-arithmetic-factors](item-lem-euler-local-arithmetic-factors)
- [lem-euler-arithmetic-factor-products](item-lem-euler-arithmetic-factor-products)


## Statement

Let $n=2m$, where $m$ is a positive odd integer and every prime divisor of $m$ belongs to $\mathcal P_3$, the set of primes congruent to $3$ modulo $4$. Odd means of the form $2k+1$ for an integer $k$. An integer $d$ divides an integer $u$, written $d\mid u$, when $u=dk$ for some integer $k$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Congruence to $i$ modulo $4$ means that $4$ divides the difference from $i$.

For a positive integer $u$, let $\tau(u)$ count its positive divisors and let $\sigma(u)$ be their sum. Let $P(u)$ be the product of $e+1$ over primes $q$ congruent to $1$ modulo $4$ with a positive integer exponent $e$ such that $q^e$ divides $u$ and $q^{e+1}$ does not. A finite product starts at $1$ and multiplies by each indicated factor, so the empty product is $1$. Let $M(n)$ be the largest value of $P(u)$ attained at an integer $1\le u\le n$.

Read the fractions and powers in the estimates in the real numbers, using the inclusions of the natural numbers into the integers, the integers into the rationals, and the rationals into the reals. For a positive real $x$, write $x^{1/5}$ for its unique positive fifth root, the positive real whose fifth power is $x$. Nonnegative integer powers are repeated products. Then
$$\frac{\tau(m)m}{\sigma(m)}\le \frac{23}{10}m^{1/5},\qquad M(n)\le \frac{11}{5}n^{1/5}.$$

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[def-euler-divisor-functions](item-def-euler-divisor-functions)

[def-euler-two-square-counts](item-def-euler-two-square-counts)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)

[math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)

[math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

[math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)

[math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)

## Facts & Assumptions

[F1] The natural numbers identify with the nonnegative integers, and the inclusions from naturals to integers, integers to rationals, and rationals to reals preserve arithmetic and order. Integer multiplication is associative and commutative with identity $1$. [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[F2] The real numbers form a totally ordered field. Addition and multiplication are associative and commutative, multiplication distributes over addition, and division is multiplication by the inverse of a nonzero denominator. A strict comparison $a<b$ means $b-a$ is positive. Sums and products of positive elements are positive, and the inverse of a positive element is positive. Thus multiplying a weak or strict inequality by a positive number preserves it. [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field) [math:def-field](https://alphabetamath.cc/item/def-field) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field) [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive) The real multiplicative identity satisfies $0<1$. [math:cor-of-one-positive](https://alphabetamath.cc/item/cor-of-one-positive) The reals used here are the Cauchy-sequence reals, the quotient of the ring of rational Cauchy sequences by the ideal of null sequences. Every nonempty subset of these reals that is bounded above has a least upper bound. Together with the ordered-field structure, this makes these reals a complete ordered field. [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers) [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field) [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)

[F3] Every positive integer is a finite product of primes, unique up to their order, and the prime list for $1$ is empty. A nonnegative integer power $x^j$ starts at $x^0=1$ and appends a factor $x$ at each successor. [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic) [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

[F4] For a positive integer $v$ written as a product of powers $p^{e_p}$ of distinct primes with $e_p\ge1$, its positive divisors are precisely the products obtained by independently choosing $0\le j_p\le e_p$ as integer exponents. The count is $\tau(v)=\prod_p(e_p+1)$ and the sum is $\sigma(v)=\prod_p\sigma(p^{e_p})$, where $\sigma(p^{e_p})=1+p+\cdots+p^{e_p}$. [lem-divisors-from-prime-exponents](item-lem-divisors-from-prime-exponents)

[F5] The two-square count definition specifies $P(u)$ using the exact prime powers in the Statement and gives an attained maximum $M(n)$ for each positive integer $n$. [def-euler-two-square-counts](item-def-euler-two-square-counts)

[F6] In the complete ordered field from [F2], the root theorem with natural exponent $5$ gives, for each real $x>0$, a unique nonnegative $s$ with $s^5=x$, and gives $s>0$. [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist) For a positive real $x$ and a positive integer $e$, the rational power $x^{e/5}$ equals $(x^{1/5})^e$. For positive real $x,y$ one has $(xy)^{1/5}=x^{1/5}y^{1/5}$, $(x^e)^{1/5}=x^{e/5}$, and $1^{1/5}=1$. Positive integer powers of positive reals are positive. For nonnegative reals and any positive integer exponent, taking that power preserves and reflects both weak and strict order. [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power) [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power) [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws) [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone) [math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[F7] Integer multiplication from [F1] and real multiplication from [F2] are each closed, associative and commutative, with two-sided identity $1$, so each forms a commutative monoid. [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid) A product of a finite list starts at $1$ and appends the next factor by multiplication. Induction establishes a property for all nonnegative integer lengths by proving it at zero and proving that it passes from each length to its successor. [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F8] For any prime $p$ and positive integer $e$, the fraction $(e+1)p^e/(\sigma(p^e)p^{e/5})$ is at most $p(e+1)/((p+1)p^{e/5})$. [lem-euler-local-arithmetic-factors](item-lem-euler-local-arithmetic-factors)

[F9] For $i\in\{1,3\}$ let $\mathcal P_i$ be the primes congruent to $i$ modulo $4$. For $p\in\mathcal P_3$, $B_3(p)$ is the maximum of $1$ and the bounds $p(e+1)/((p+1)p^{e/5})$ over positive integers $e$. For $q\in\mathcal P_1$, $B_1(q)$ is the maximum of $1$ and the bounds $(e+1)/q^{e/5}$ over positive integers $e$. These maxima exist and equal $1$ at primes at least $32$. The products $C_1=\prod_{p\in\mathcal P_3,\,p<32}B_3(p)$ and $C_2=\prod_{q\in\mathcal P_1,\,q<32}B_1(q)$ satisfy $C_1^5<(23/10)^5$ and $C_2^5<(11/5)^5$. Both cutoff products take their primes in increasing order. [def-euler-prime-classes](item-def-euler-prime-classes) [lem-euler-arithmetic-factor-products](item-lem-euler-arithmetic-factor-products)

[F10] Use the additive order on the natural numbers. For naturals $a,b$, $a\le b$ means $a+k=b$ for some natural $k$, and $a<b$ means $a\le b$ and $a\ne b$. For a natural length $r$, the positions of the list are the natural numbers $i<r$. By the natural-order lemma these are exactly the elements of the von Neumann natural $r$. A permutation is a bijection of this position set to itself. It maps each new position to an old position and uses each old position exactly once. In these commutative monoids, permuting a finite list leaves its product unchanged. The product of a concatenated list is the product of the products of its two parts. Replacing consecutive blocks by their products also preserves the product. To apply the sequence laws, extend each list of factors by identity elements. For regrouping, let $c_j$ be the length of block $j$, taking $c_j=0$ at every index after the blocks are exhausted. Apply natural-number finite-sum recursion to this sequence to obtain the boundary function $s:\mathbb N\to\mathbb N$ given by $s_j=\sum_{k<j}c_k$. This gives $s_0=0$ and $s_{j+1}=s_j+c_j$, so $c_j$ witnesses $s_j\le s_{j+1}$ in the additive order. On the padded tail $s_j+0=s_j$, so the last boundary repeats. [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-symmetric-group](https://alphabetamath.cc/item/def-symmetric-group) [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership) [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product) [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)

## Proof

**Given:** Positive integers $m,n$ with $n=2m$, $m$ odd, and each prime divisor of $m$ in $\mathcal P_3$.

**Goal:** Prove the two bounds in the Statement.

1.1 For any positive integer $v$, scan its prime list from [F3] and record the distinct primes in the order of their first appearances. In that order, take one block per recorded prime, consisting of all its occurrences in their original order. This takes each original position exactly once. By [F10], the numerical positions of a list of length $r$ are exactly the elements of $r$, so the new-to-old position map is a bijection $r\to r$. Apply the permutation law of [F10] in the commutative monoid $(\mathbb Z,\cdot,1)$ from [F7]. If there are $b$ prime blocks, their concatenation has all $r$ positions of the reordered list, so their lengths sum to $r$ and the boundary function from [F10] has $s_b=r$. Apply the regrouping law of [F10] with these boundaries. The permutation and multiplication within each block preserve the integer product. This writes $v=\prod_p p^{e_p}$ with distinct prime bases and each exponent equal to the positive number of copies of its prime. By [F4] a prime $q$ in that list has $q^j\mid v$ for $1\le j\le e_q$, by choosing exponent $j$ at $q$ and zero elsewhere. Conversely, for any prime $q$ and integer $j\ge1$, if $q^j\mid v$, the divisor description writes $q^j$ as one of the divisor products. Uniqueness of prime lists forces $q$ to occur and its chosen exponent to equal $j$, so $j\le e_q$. Thus the prime bases are exactly the prime divisors, and $q^{e_q}$ divides $v$ while $q^{e_q+1}$ does not. [F1, F3, F4, F7, F10]

1.2 Products preserve comparisons of positive factors. The empty products are both $1$ by [F7], and $1>0$ by [F2]. If the current products satisfy $0<A\le B$ and the next factors satisfy $0<a\le b$, then $0<Aa\le Ba\le Bb$ by [F2]. Appending one factor at a time as in [F7] proves by induction that the two products are positive and the first is at most the second. For reordering and regrouping real factors use [F10] in the commutative monoid $(\mathbb R,\cdot,1)$ from [F7]. To delete a factor $1$, move it to the end by [F10] and use the identity law in the product recursion. This also justifies inserting factors $1$. If all $b_i>0$, expand the factors of $\prod_i(a_i/b_i)$ as $a_i b_i^{-1}$ and multiply by $\prod_i b_i$. The concatenation law in [F10] identifies the result with the product of one list. Use [F10] to move each $b_i^{-1}$ next to its matching $b_i$ and multiply each pair to get $1$. Deleting those unit factors leaves $\prod_i a_i$. The product $\prod_i b_i$ is positive by the preceding induction, so division gives $(\prod_i a_i)/(\prod_i b_i)=\prod_i(a_i/b_i)$. [F2, F7, F10]

1.3 Each $B_i(t)$ in [F9] is at least $1$. The product recursion in [F7] starts at $1>0$ and multiplies positive factors, so $C_1,C_2$ are positive by [F2]. The fifth-power comparisons in [F9] and order reflection in [F6] give $C_1<23/10$ and $C_2<11/5$. [F2, F6, F7, F9]

2.1 Apply step 1.1 to $m$. The divisor formulas give the products for $\tau(m)$ and $\sigma(m)$, with every factor $\sigma(p^{e_p})$ positive because it is a sum of positive numbers including $1$. Applying the product law for fifth roots from [F6] from the empty product up through each successive factor gives $m^{1/5}=\prod_{p\mid m,\,p\ \mathrm{prime}}p^{e_p/5}$. The embeddings in [F1] allow the integer products to be evaluated in the reals. Using concatenation, permutation and consecutive-block regrouping in [F10], pair the factors with the same prime index separately in the numerator and in the denominator. The quotient rule in step 1.2 gives
$$\frac{\tau(m)m}{\sigma(m)m^{1/5}}=\prod_{p\mid m,\,p\ \mathrm{prime}}\frac{(e_p+1)p^{e_p}}{\sigma(p^{e_p})p^{e_p/5}}.$$
[given, F1, F2, F4, F6, F7, F10, step 1.1, step 1.2]

2.2 Take any integer $u$ with $1\le u\le n$ and use its prime powers from step 1.1. In $P(u)$ the factor at a prime divisor $q$ is $e_q+1$ if $q\in\mathcal P_1$ and is $1$ otherwise, since step 1.1 verifies exactly the divisibility conditions in [F5]. Permutation invariance from [F10] and insertion of factors $1$ from step 1.2 give $P(u)$ on the full prime-divisor list. For the positive bases in [F6], the product law again gives $u^{1/5}$ as the product of $q^{e_q/5}$ over all prime divisors $q$, by applying it to each appended factor. Thus $P(u)/u^{1/5}$ is the product of $(e_q+1)/q^{e_q/5}$ at those $q$ in $\mathcal P_1$ and of $1/q^{e_q/5}$ at the other prime divisors. All factors are positive. At the other prime divisors, $q>1$ implies $q^{1/5}>1$ by fifth-power order reflection, so $(q^{1/5})^{e_q}\ge1$ and $1/q^{e_q/5}\le1$. [given, F1, F2, F5, F6, F7, F9, F10, step 1.1, step 1.2]

3.1 Each factor in the product for $m$ in step 2.1 is positive and at most $B_3(p)$ by [F8] and [F9], since each prime divisor $p$ of $m$ belongs to $\mathcal P_3$. Start with the distinct prime divisors of $m$ from step 1.1. Scan the cutoff list for $C_1$ in [F9] and append each prime that is missing. Each prime in either list occurs once in the resulting list. On the left, keep the factors from step 2.1 and use $1$ at any appended prime, where $1\le B_3(p)$. Appending these unit factors preserves the left product. On the right, use $B_3(p)$ everywhere. Its factors at primes at least $32$ equal $1$. Remove these factors by step 1.2 and restore cutoff order by [F10], so the right product is $C_1$. By step 1.2 the quotient in step 2.1 is at most $C_1$. This includes $m=1$, when the product in step 2.1 is empty and equals $1$. Multiply by the positive $m^{1/5}$ and use $C_1<23/10$ from step 1.3 to obtain the first bound. [given, F2, F6, F8, F9, F10, step 1.1, step 1.2, step 1.3, step 2.1]

3.2 For any integer $u$ with $1\le u\le n$, take its distinct prime divisors from step 1.1 and append the missing primes from the cutoff list for $C_2$ in [F9], in cutoff order. Each prime in either list occurs once. Keep the factors from step 2.2 on the left and append $1$ at each new prime, preserving the left product. For a prime in $\mathcal P_1$, the left factor is at most $B_1(q)$ by [F9] when the prime divides $u$ and by $1\le B_1(q)$ when it was appended. At every prime outside $\mathcal P_1$ use the upper factor $1$ from step 2.2. On the right the factors outside $\mathcal P_1$ and the factors at primes in $\mathcal P_1$ at least $32$ all equal $1$. Delete those unit factors by step 1.2 and reorder the remaining factors by [F10] to obtain $C_2$. By step 1.2, $P(u)/u^{1/5}\le C_2$. The estimate includes $u=1$, for which the quotient is $1$. [given, F2, F6, F7, F9, F10, step 1.1, step 1.2, step 2.2]

4.1 For $1\le u\le n$, the order-preserving inclusion into the reals and fifth-power order reflection give $u^{1/5}\le n^{1/5}$. Multiply step 3.2 by the positive root $u^{1/5}$ from [F6] and use $0<C_2<11/5$ to obtain $P(u)\le (11/5)n^{1/5}$. The same bound holds at an integer attaining $M(n)$ by [F5]. This proves the second bound and completes the proof together with step 3.1. [F1, F2, F5, F6, step 1.3, step 3.1, step 3.2] ∎

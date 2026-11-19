---
title: Prime-power majorants for the arithmetic factors
status: published
research_item: lem-euler-local-arithmetic-factors
dependency_level: 2
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 5, Lemma 5.1, first two proof paragraphs before the table
---

PDF p. 5: ` Lemma 5.1, first two proof paragraphs before the table `

## Prerequisites

- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [def-euler-divisor-functions](item-def-euler-divisor-functions)
- [def-euler-two-square-counts](item-def-euler-two-square-counts)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)
- [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)
- [lem-divisors-from-prime-exponents](item-lem-divisors-from-prime-exponents)
- [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone)
- [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)
- [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)


## Statement

Let $p$ be a prime, an integer greater than $1$ whose only positive divisors are $1$ and itself. Let $e\ge1$ be an integer. For a positive integer $v$, $\sigma(v)$ sums its positive divisors and $\tau(v)$ counts them. A positive divisor $d$ of $v$ satisfies $v=dk$ for some integer $k$. Use integers in real arithmetic via their usual inclusions through the rationals. For $a>0$, $a^{e/5}$ is the $e$-th power of the unique positive real $a^{1/5}$ whose fifth power is $a$. A nonnegative integer power starts at $a^0=1$ and multiplies by $a$ at each successor. Division by a nonzero real means multiplication by its inverse.

Then

$$\frac{(e+1)p^e}{\sigma(p^e)p^{e/5}}\le \frac{p}{p+1}\frac{e+1}{p^{e/5}}.$$

For a positive integer $u$, let $P(u)$ be the product of $e+1$ over primes $q\equiv1\pmod4$ with $q^e$ dividing $u$ and $q^{e+1}$ failing to divide $u$, where $e\ge1$ is the exponent for that prime. The congruence means that $4$ divides $q-1$. The factor from such a $q$ in $P(u)/u^{1/5}$ is $(e+1)/q^{e/5}$.

For $p\ge32$, one has $e+1\le2^e\le p^{e/5}$, and both sides of the displayed inequality are at most $1$. For $q\ge32$, one has $(e+1)/q^{e/5}\le1$.

## Statement references

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[def-euler-divisor-functions](item-def-euler-divisor-functions)

[def-euler-two-square-counts](item-def-euler-two-square-counts)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)

[math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)

[math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)

[math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

[math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)

[math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)

[math:def-group-power](https://alphabetamath.cc/item/def-group-power)

[math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

## Facts & Assumptions

[F1] A prime exceeds $1$ and has only $1$ and itself as positive divisors. Integer divisibility means being an integer multiple, and congruence modulo $4$ means divisibility of the difference by $4$. [math:def-prime](https://alphabetamath.cc/item/def-prime) [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z) [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[F2] The divisor count and sum use all positive divisors. For any prime $p$ and positive integer $e$, the single-prime case of the divisor product formulas gives $\tau(p^e)=e+1$ and $\sigma(p^e)=\sum_{j=0}^{e}p^j$. [def-euler-divisor-functions](item-def-euler-divisor-functions) [lem-divisors-from-prime-exponents](item-lem-divisors-from-prime-exponents)

[F3] In the product $P(u)$, a prime $q\equiv1\pmod4$ with $q^e$ dividing $u$ but $q^{e+1}$ failing to divide $u$ supplies the factor $e+1$. [def-euler-two-square-counts](item-def-euler-two-square-counts)

[F4] The natural numbers identify with the nonnegative integers. The inclusions from naturals to integers, integers to rationals and rationals to reals preserve arithmetic and order. [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[F5] The reals form a complete ordered field. Completeness means that every nonempty set of reals with an upper bound has a least upper bound, where an upper bound is a number at least as large as each element of the set. Addition and multiplication are associative and commutative, multiplication distributes over addition, and division by a nonzero element multiplies by its inverse. For reals $x,y$, $x\le y$ means $y-x$ is zero or positive. Sums and products of positive reals are positive. [math:def-field](https://alphabetamath.cc/item/def-field) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field) [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field) [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)

[F6] Nonnegative integer powers start at $1$ and append one copy of the base at each successor. Integer multiplication is associative and commutative, with two-sided identity $1$, so it makes the integers a commutative monoid. The integer-valued power uses this monoid. The real-valued power follows the same recursion in the reals. For positive $a$, the rational power $a^{m/n}$ with $n\ge1$ equals the $m$-th power of the unique positive $n$-th root of $a$. At denominator $1$ the root is $a$, so this agrees with the integer power. [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power) [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power) [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist) [math:def-group-power](https://alphabetamath.cc/item/def-group-power) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)

[F7] For positive real bases, integer powers with nonnegative exponents are positive. For nonnegative real bases $a,b$ and a positive integer $k$, $a\le b$ holds exactly when $a^k\le b^k$. [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone)

[F8] In an ordered field the inverse of a positive element is positive. Multiplication by a positive number preserves weak order because it multiplies the difference of the two sides by that number. [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive) [math:def-field](https://alphabetamath.cc/item/def-field) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)

[F9] Real addition is associative and commutative with two-sided identity $0$, so it forms a commutative monoid. A finite sum starts at zero and successively adds each term once in an enumeration of its index set. [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid) [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid) [math:def-field](https://alphabetamath.cc/item/def-field)

[F10] For positive real $a,b$ and rational $r,s$, $(ab)^r=a^rb^r$ and $(a^r)^s=a^{rs}$. [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)

[F11] A property holds for all nonnegative integers if it holds at zero and passes from each nonnegative integer to its successor. [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F12] The natural successor $\operatorname{succ}(k)$ equals $k+1$ because $k+\operatorname{succ}(0)=\operatorname{succ}(k+0)=\operatorname{succ}(k)$ and $1=\operatorname{succ}(0)$. The inclusion into the integers preserves this addition. [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[F13] For integers $a,b$ with $b\ne0$, the rational $a/b$ denotes the class $[(a,b)]$. For pairs with nonzero denominators, the product of classes is $[(a,b)]\,[(c,d)]=[(ac,bd)]$. [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)

[F14] For finite lists in a monoid, the empty product is the identity and a one-term product is its sole entry. The product of a list split into two consecutive blocks is the product of the two block products in that order. [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)

## Proof

**Given:** A prime $p$ and integer $e\ge1$. For the factor in $P(u)$, take $u,q,e$ as in the Statement.

**Goal:** Prove the displayed bound and the normalized factor formula, and verify the bounds by $1$ at primes at least $32$.

1.1 The divisor formulas give $\tau(p^e)=e+1$ and $\sigma(p^e)=\sum_{j=0}^{e}p^j$. For any integer base, the images in the reals of its integer-valued powers obey the real-power recursion because the inclusions preserve $1$ and multiplication. By uniqueness in the real-power definition, the images equal the corresponding real powers. The inclusions also preserve addition, so the finite sum can be evaluated in the reals. The last two indices $e-1,e$ are present since $e\ge1$. Each term is positive since $p>1$. Thus the sum of the terms before those last two is nonnegative, starting from zero and adding positive terms. Consequently $\sigma(p^e)\ge p^{e-1}+p^e=p^{e-1}(p+1)>0$. [given, F1, F2, F4, F5, F6, F7, F9, F12]

1.2 Induct on the natural number $k$, using its image in the nonnegative integers and then the reals. The successor is represented by $k+1$ under these inclusions. Prove $k+1\le2^k$. At $k=0$ it reads $1=2^0$. If it holds at $k$, then $k+2\le2(k+1)\le2\cdot2^k=2^{k+1}$. The first inequality follows from $k\ge0$ and the second by multiplying the induction hypothesis by $2>0$. This proves $e+1\le2^e$. [given, F4, F5, F6, F8, F11, F12]

1.3 Use the complete ordered field in [F5] for the root in [F6]. For any real $a\ge32$, the positive fifth root $a^{1/5}$ satisfies $(a^{1/5})^5=a\ge 32=2^5$. Fifth powers reflect order on the nonnegative reals, so $a^{1/5}\ge2$. Taking $e$-th powers preserves order since $e\ge1$, giving $2^e\le (a^{1/5})^e=a^{e/5}$. [given, F5, F6, F7]

2.1 For the second factor, write $u=q^ec$ with $c$ an integer by divisibility. Since $u>0$ and $q^e>0$, the quotient $c$ is positive. If $c=qd$ for an integer $d$, then $u=q^e(qd)=q^{e+1}d$ by integer multiplication and the power recursion with successor $e+1$. This contradicts $q^{e+1}$ failing to divide $u$. Read $u=q^ec$ in the reals using the agreement of powers from step 1.1. Since $q,c>0$ and $q^e=q^{e/1}$ for the real powers, the positive-base power laws give $u^{1/5}=(q^e)^{1/5}c^{1/5}=q^{(e/1)(1/5)}c^{1/5}$. Using $a/b=[(a,b)]$, multiplication of the representatives gives $[(e,1)]\,[(1,5)]=[(e,5)]$, so $(e/1)(1/5)=e/5$. Hence $u^{1/5}=q^{e/5}c^{1/5}$. [given, F1, F4, F5, F6, F7, F8, F10, F12, F13, step 1.1]

2.2 Multiply the lower bound for $\sigma(p^e)$ by $p/(\sigma(p^e)(p+1))$, which is positive. Cancellation gives $p^e/\sigma(p^e)\le p/(p+1)$. Multiplying this comparison by the positive number $(e+1)/p^{e/5}$ gives the displayed inequality. [step 1.1, F5, F6, F7, F8]

3.1 In the increasing list defining $P(u)$, the entry for $q$ lies between the entries for primes less than $q$ and those for primes greater than $q$. Let $B$ and $D$ be the products of these two blocks, using $1$ for an empty block. Apply the finite-product splitting law first just before the entry for $q$ and then just after it within the remaining block. The singleton has product $e+1$, so $P(u)=B((e+1)D)$ in the multiplicative monoid of integers. By integer commutativity and associativity this is $(e+1)(BD)$. The same splitting law gives $BD$ as the product of the increasing list with the entry for $q$ deleted. The inclusions preserve these products in the reals. Since $q^{e/5}$ and $c^{1/5}$ are positive, commutativity and the field laws give $\frac{P(u)}{u^{1/5}}=\frac{(e+1)(BD)}{q^{e/5}c^{1/5}}=\frac{e+1}{q^{e/5}}\frac{BD}{c^{1/5}}$. This exhibits the required factor. [given, F3, F4, F5, F6, F7, F8, F14, step 2.1]

4.1 When $p\ge32$, applying the power comparison to $a=p$ gives $e+1\le2^e\le p^{e/5}$ and division by the positive power gives $(e+1)/p^{e/5}\le1$. The multiplier $p/(p+1)$ is positive and at most $1$ since $0<p<p+1$. Thus the right side of the displayed bound is at most $1$, and so is the left side. Taking $a=q$ when $q\ge32$ gives $(e+1)/q^{e/5}\le1$. These estimates and the normalized factor identity establish all the claims. [given, F1, F5, F6, F7, F8, step 2.2, step 3.1, step 1.2, step 1.3] ∎

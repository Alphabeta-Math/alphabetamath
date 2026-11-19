---
title: Maximizing exponents in the small-prime bounds
status: draft
research_item: lem-euler-local-arithmetic-maxima
dependency_level: 3
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 5, Lemma 5.1, ratio test and table of maximizing positive exponents
      reading_limits: Read the ratio paragraph and table on page 5 for attribution.
        The proof derives the comparisons directly.
---

PDF p. 5: ` Lemma 5.1, ratio test and table of maximizing positive exponents `

## Prerequisites

- [def-euler-prime-classes](item-def-euler-prime-classes)
- [lem-positive-sequence-ratio-maximum](item-lem-positive-sequence-ratio-maximum)
- [lem-euler-local-arithmetic-factors](item-lem-euler-local-arithmetic-factors)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)
- [lem-trial-division-primality-bound](item-lem-trial-division-primality-bound)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)
- [math:lem-nat-nonzero-is-successor](https://alphabetamath.cc/item/lem-nat-nonzero-is-successor)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)
- [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)
- [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone)
- [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)


## Statement

Let $p$ be a prime, an integer greater than $1$ whose only positive divisors are $1$ and $p$. An integer $d$ divides an integer $u$ if $u=dq$ for some integer $q$. Identify the nonnegative integers with the natural numbers and use their usual images in the reals. For each integer $e\ge1$, write $p^{e/5}=(p^{1/5})^e$, where $p^{1/5}$ is the unique positive real whose fifth power is $p$. Nonnegative integer powers start at $1$ at exponent $0$ and multiply by the base at each successor. Real division by a nonzero number multiplies by its inverse.

The sequence $a_e(p)=(e+1)/p^{e/5}$ assigns a positive real number to each index $e\ge1$. Its successive ratio, the next term divided by the current term, is
$$r_e(p)=\frac{a_{e+1}(p)}{a_e(p)}=\frac{e+2}{(e+1)p^{1/5}}.$$
The ratios strictly decrease as $e$ increases, and $r_e(p)\le1$ exactly when $(e+2)^5\le p(e+1)^5$. Equivalently, $r_e(p)\ge1$ exactly when $(e+2)^5\ge p(e+1)^5$.

For integers $u,r$, write $u\equiv r\pmod 4$ when $4$ divides $u-r$. The set $\mathcal P_3$ consists of the primes congruent to $3$ modulo $4$. The table lists the primes $p<32$ in the two indicated classes and their unique maximizing positive exponents $k$, meaning $a_k(p)>a_e(p)$ for every positive integer $e\ne k$.

| Prime class | Primes in order | Maximizing positive exponents in order |
| --- | --- | --- |
| $p\in\mathcal P_3$ | $3,7,11,19,23,31$ | $4,2,1,1,1,1$ |
| $p\equiv1\pmod 4$ | $5,13,17,29$ | $2,1,1,1$ |

For each listed prime the maximizing exponent is the least positive $e$ with $(e+2)^5\le p(e+1)^5$. For the first class the same exponent also maximizes the bound $\frac{p}{p+1}a_e(p)$.

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[lem-positive-sequence-ratio-maximum](item-lem-positive-sequence-ratio-maximum)

[lem-euler-local-arithmetic-factors](item-lem-euler-local-arithmetic-factors)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

[math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)

[math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)

## Facts & Assumptions

[F1] Use the usual integers with their order, addition, and multiplication. A prime is greater than $1$ with no positive divisors apart from $1$ and itself, and a divisor gives an integer multiple. Congruence modulo $4$ means that the difference is a multiple of $4$. [math:def-integers](https://alphabetamath.cc/item/def-integers) [math:def-int-order](https://alphabetamath.cc/item/def-int-order) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[F2] The natural numbers start at $0$ and have successor $t+1$. Their order is $x\le y$ when $x+d=y$ for a natural number $d$. Every nonzero natural number has a predecessor, and $x<y$ is equivalent to $x+1\le y$. The inclusions of the naturals in the integers, the integers in the rationals, and the rationals in the reals preserve the arithmetic and order, and the image of the naturals is exactly the nonnegative integers. [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [math:lem-nat-nonzero-is-successor](https://alphabetamath.cc/item/lem-nat-nonzero-is-successor) [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[F3] The reals form a complete ordered field. A field has associative and commutative addition and multiplication, multiplication distributes over addition, and each nonzero number has a multiplicative inverse. In the real order $x<y$ means $y-x>0$, and multiplying by a positive number preserves and reflects order since the product of positive numbers is positive. Completeness means that every nonempty subset with an upper bound has a least upper bound. An upper bound is at least every element of the subset, and a least upper bound is at most every other upper bound. [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers) [math:def-real-order](https://alphabetamath.cc/item/def-real-order) [math:def-field](https://alphabetamath.cc/item/def-field) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field) [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field) [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)

[F4] For a nonnegative real $x$ in a complete ordered field, there is a unique nonnegative fifth root, which is positive when $x>0$. The rational power $x^{e/5}$ for $x>0$ is the $e$-th power of that root. For a nonnegative integer $e$, $c^0=1$ and $c^{e+1}=c^ec$. Integer powers of positive bases are positive. Fifth powers preserve and reflect order on nonnegative reals. The inverse of a positive real is positive. [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist) [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power) [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power) [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone) [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)

[F5] For an integer $u>1$, trial division tests precisely the integers $d\ge2$ with $d^2\le u$. The number $u$ is prime exactly when none of those $d$ divides it. For positive $d$ and integer $u$, the remainder is the unique integer $b$ with $0\le b<d$ and $u=dq+b$ for some integer $q$. A zero remainder is equivalent to divisibility by $d$. [lem-trial-division-primality-bound](item-lem-trial-division-primality-bound) [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

[F6] For a sequence of positive real terms $a_e$ indexed by $e\ge1$, write $r_e=a_{e+1}/a_e$ for the successive ratios. Assume these ratios are nonincreasing, so $r_i\ge r_j$ whenever $1\le i\le j$. If a positive index $k$ satisfies $r_k\le1$ and also $r_{k-1}\ge1$ when $k>1$, then $a_k\ge a_e$ for every $e\ge1$. [lem-positive-sequence-ratio-maximum](item-lem-positive-sequence-ratio-maximum)

[F7] For $e\ge1$ and $p\in\mathcal P_3$, the local upper bound in the first arithmetic estimate is $p\,a_e(p)/(p+1)$. For a prime $p\equiv1\pmod4$ and a positive integer $u$ divisible by $p^e$ with $e\ge1$ but not by $p^{e+1}$, the local factor in the second estimate is $a_e(p)$. [lem-euler-local-arithmetic-factors](item-lem-euler-local-arithmetic-factors) [def-euler-prime-classes](item-def-euler-prime-classes)

## Proof

**Given:** A prime $p$ and the sequence indexed by positive integers as in the Statement.

**Goal:** Prove the ratio formula and sign tests, enumerate the two classes below $32$, and verify the maximizing indices.

1.1 Set $c=p^{1/5}$. Since $p>1$, the real field and root facts give $c>0$ and $c^5=p$. The powers $c^e$ are positive, and $e+1>0$ by the inclusion of the positive indices into the reals. Thus $a_e(p)>0$. Dividing consecutive terms and canceling $c^e$ using $c^{e+1}=c^ec$ gives $r_e(p)=(e+2)/((e+1)c)$. For $f>e$, subtracting the two ratio formulas gives $r_e(p)-r_f(p)=(f-e)/((e+1)(f+1)c)>0$ because the numerator and denominator are positive. [given, F1, F2, F3, F4]

1.2 A prime less than $32$ is at least $2$. Any integer $u$ with $2<u<32$ and remainder $0$ on division by $2$ has the proper positive divisor $2$ and is excluded. Remainder $1$ gives $u=2t+1$ with $0<t<16$ by the bounds on $u$. Such $t$ is a positive natural number and hence one of $1,\ldots,15$ by discreteness. Among these odd candidates, $9,15,21,27$ are multiples of $3$, and $25=5\cdot5$. Each displayed divisor is strictly between $1$ and its candidate. This leaves $3,5,7,11,13,17,19,23,29,31$. [F1, F2, F3, F5]

2.1 Multiplying the comparison of $r_e(p)$ with $1$ by the positive real $(e+1)c$ gives the same comparison of $e+2$ with $(e+1)c$. Both sides are positive, so taking fifth powers preserves and reflects each comparison, including strict comparisons. The product of five copies of $(e+1)c$ is $(e+1)^5c^5=p(e+1)^5$ by commutativity and $c^5=p$. This proves both tests. [F2, F3, F4, step 1.1]

2.2 For the remaining candidates $u$, a trial divisor $d$ is at most $5$ because $d\ge6$ gives $d^2\ge36>u$. Their remainder $1$ modulo $2$ rules out $2$ and also $4$, since a multiple of $4$ is a multiple of $2$. For $3$ and $5$, the trial range excludes both $3$ and $5$ because their squares exceed $u$. For $7,11,13,17,19,23,29,31$ in that order, division by $3$ gives remainders $1,2,1,2,1,2,2,1$, and division by $5$ gives remainders $2,1,3,2,4,3,4,1$. All tested remainders are nonzero, so every remaining candidate is prime. The numbers of the form $4t+3$ on this list have $t=0,1,2,4,5,7$ and give $3,7,11,19,23,31$. Those of the form $4t+1$ have $t=1,3,4,7$ and give $5,13,17,29$. These lists account for all the surviving odd candidates, and uniqueness of the remainder modulo $4$ makes the lists disjoint. The remainder of $2$ on division by $4$ is $2$, so it belongs to neither class. [F1, F2, F3, F4, F5, step 1.2]

3.1 For $p=3$ the previous and current comparisons at the proposed index $k=4$ are $5^5=3125>3072=3\cdot4^5$ and $6^5=7776<9375=3\cdot5^5$. Hence $r_3(3)>1>r_4(3)$. For $p=5,7$ take $k=2$. Then $3^5=243>224=7\cdot2^5\ge p\cdot2^5$ and $4^5=1024<1215=5\cdot3^5\le p\cdot3^5$, so $r_1(p)>1>r_2(p)$. Every other prime in the table satisfies $p\ge11$, so $3^5=243<352=11\cdot2^5\le p\cdot2^5$. This gives $r_1(p)<1$ for each proposed index $k=1$. [F2, F3, F4, step 2.1, step 2.2]

4.1 The terms are positive and the ratios strictly decrease by step 1.1, so the comparisons in step 3.1 give the hypotheses of [F6]. It follows that $a_k(p)$ is a maximum. If $e<k$, then $k>1$ and $e\le k-1$ by discreteness, so $r_e(p)\ge r_{k-1}(p)>1$. Hence $a_e(p)<a_{e+1}(p)\le a_k(p)$. If $e>k$, write $e=h+1$ by [F2]. We have $h\ge k$ because $h<k$ would imply $e=h+1\le k$. Then $r_h(p)\le r_k(p)<1$, which gives $a_e(p)<a_h(p)\le a_k(p)$. This makes the maximum unique. Since every earlier ratio exceeds $1$ and $r_k(p)<1$, step 2.1 identifies $k$ as the least positive exponent satisfying the stated fifth-power inequality. The factor $p/(p+1)$ in the first class is positive and independent of $e$, so it preserves every strict comparison between terms. This proves the listed maximizing exponents for both bounds. [F2, F3, F4, F6, F7, step 1.1, step 2.1, step 2.2, step 3.1] ∎

## Source notes

Page 5 uses the fifth-power inequality to locate the maximizing positive exponent. The proof makes the crossing explicit by comparing the ratio at that exponent and, when it exists, the preceding ratio. [Lemma 5.1](https://hexagonmath.org/pdf/2611.00370v1#page=5)

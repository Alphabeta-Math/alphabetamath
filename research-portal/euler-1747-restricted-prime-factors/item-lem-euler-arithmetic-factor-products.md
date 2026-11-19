---
title: Explicit products of the small-prime majorants
status: published
research_item: lem-euler-arithmetic-factor-products
dependency_level: 4
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 5, Lemma 5.1, absent-prime convention and displayed fifth-power
        products
---

PDF p. 5: ` Lemma 5.1, absent-prime convention and displayed fifth-power products `

## Prerequisites

- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order)
- [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [lem-euler-local-arithmetic-factors](item-lem-euler-local-arithmetic-factors)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)
- [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [lem-euler-local-arithmetic-maxima](item-lem-euler-local-arithmetic-maxima)
- [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone)
- [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)
- [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)


## Statement

A prime is an integer greater than $1$ with only $1$ and itself as positive divisors. An integer $d$ divides an integer $u$ if $u=dk$ for some integer $k$. For $i\in\{1,3\}$, let $\mathcal P_i$ consist of the primes $p$ congruent to $i$ modulo $4$, meaning that $4$ divides $p-i$.

Use the natural numbers $0,1,\ldots$ as exponents, and identify them with the nonnegative integers. Use integer numerals in the reals via their usual inclusions through the rationals. For a real base $x$, write $x^0=1$ and $x^{n+1}=x^nx$ for a natural number $n$. For $x>0$ and a positive integer $e$, write $x^{e/5}=(x^{1/5})^e$, where $x^{1/5}$ is the unique positive real with fifth power $x$. Division by a nonzero real multiplies by its inverse.

For each $p\in\mathcal P_3$ and $e\ge1$, use the upper bound $\frac{p}{p+1}\frac{e+1}{p^{e/5}}$. For each $q\in\mathcal P_1$ and $e\ge1$, use the upper bound $\frac{e+1}{q^{e/5}}$. In each class let $B_i(t)$ be the maximum of $1$ and all its upper bounds at the prime $t$ as $e$ ranges over positive integers. Here the maximum is the largest member of those values, and $1$ accounts for the option that the prime is absent.

Let $C_1=\prod_{p\in\mathcal P_3,\,p<32} B_3(p)$ and $C_2=\prod_{q\in\mathcal P_1,\,q<32} B_1(q)$. A finite product starts with $1$ and successively multiplies by each indicated factor in increasing prime order.

For $i\in\{1,3\}$ and an integer $N\ge32$, form the finite product of $B_i(t)$ over $t\in\mathcal P_i$ with $t<N$. The product over the full class $\mathcal P_i$ is the common value of those cutoff products. All factors at primes at least $32$ equal $1$, so the full-class products for $\mathcal P_3$ and $\mathcal P_1$ equal $C_1$ and $C_2$, respectively. Then
$$C_1^5=\frac{183143120027364343}{2849934139195392}<\left(\frac{23}{10}\right)^5,\qquad C_2^5=\frac{7962624}{160225}<\left(\frac{11}{5}\right)^5.$$

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[lem-euler-local-arithmetic-factors](item-lem-euler-local-arithmetic-factors)

[lem-euler-local-arithmetic-maxima](item-lem-euler-local-arithmetic-maxima)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)

[math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)

[math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)

[math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

[math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)

[math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)

[math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)

## Justification

For each residue $i$, primality and divisibility of $p-i$ by $4$ specify the subset of integers satisfying both conditions. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-integers](https://alphabetamath.cc/item/def-integers) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

For a positive base, the real field's least-upper-bound property ensures existence and uniqueness of the positive fifth root by the root theorem. The integer-power recursion then defines the indicated powers uniquely and gives positive powers of the roots. The remaining denominator $p+1$ is positive since $p>1$. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field) [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete) [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist) [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power) [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power) [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone)

In each class, the bounds at primes at least $32$ are at most $1$, so $1$ is the largest member of the set that includes the absent-prime value. At smaller primes the maximizing-exponent table gives an attained largest positive-exponent bound. Comparing that value to $1$ in the real order determines one real value even in case of a tie. The table also gives every prime in the two classes below $32$. [lem-euler-local-arithmetic-factors](item-lem-euler-local-arithmetic-factors) [lem-euler-local-arithmetic-maxima](item-lem-euler-local-arithmetic-maxima) [math:def-real-order](https://alphabetamath.cc/item/def-real-order) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)

For each integer $N\ge32$, scan $2,\ldots,N-1$ in increasing order and keep the members of $\mathcal P_i$. The list for cutoff $32$ is the initial segment of this list consisting of the primes below $32$. Every appended factor is $1$ by the cutoff bound and the absent-prime option. The finite-product recursion makes the product unchanged after appending one such factor, since $a\cdot1=a$. Induction on the number of appended factors gives the same value at every cutoff. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-int-order](https://alphabetamath.cc/item/def-int-order) [lem-euler-local-arithmetic-factors](item-lem-euler-local-arithmetic-factors) [math:def-field](https://alphabetamath.cc/item/def-field) [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

## Facts & Assumptions

[F1] Both stated upper bounds are at most $1$ for all positive integer exponents at primes at least $32$. The primes below $32$ in the class $\mathcal P_3$ are $3,7,11,19,23,31$, with maximizing positive exponents $4,2,1,1,1,1$, respectively, for the bound with the multiplier $p/(p+1)$. The primes below $32$ in $\mathcal P_1$ are $5,13,17,29$, with maximizing positive exponents $2,1,1,1$, respectively, for the bound without that multiplier. [lem-euler-local-arithmetic-factors](item-lem-euler-local-arithmetic-factors) [lem-euler-local-arithmetic-maxima](item-lem-euler-local-arithmetic-maxima)

[F2] The reals form a complete ordered field, meaning that every nonempty subset with an upper bound has a least upper bound. An upper bound is at least every element of the subset, and the least upper bound is at most every upper bound. The field has associative and commutative addition and multiplication, distributivity, and a multiplicative inverse for each nonzero element. Its strict order is $a<b$ when $b-a$ is positive, and products of positive numbers are positive. Multiplying a strict comparison by a positive number preserves its direction. The inverse of a positive number is positive, so division by a positive number also preserves strict comparisons. [math:def-real-order](https://alphabetamath.cc/item/def-real-order) [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field) [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete) [math:def-field](https://alphabetamath.cc/item/def-field) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field) [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)

[F3] Write $\sigma$ for the natural-number successor and $1=\sigma(0)$. The addition recursion gives $n+1=n+\sigma(0)=\sigma(n+0)=\sigma(n)$ for each natural number $n$. The natural numbers identify with the nonnegative integers, and the usual inclusions from naturals to integers, integers to rationals, and rationals to reals preserve arithmetic and order. Thus positive-integer arithmetic and comparisons of numerals have the same values in the reals. [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order) [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations) [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[F4] For a nonnegative real and a positive integer $n$, there is a unique nonnegative $n$-th root, which is positive for a positive base. The definition of rational power gives $t^{e/5}=(t^{1/5})^e$ and agrees with the integer power when the rational exponent is an integer. For positive reals $x,y$ and rational exponents $r,s$, $(xy)^r=x^ry^r$ and $(x^r)^s=x^{rs}$. Integer powers of positive bases are positive, and fifth powers preserve and reflect order on nonnegative reals. [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations) [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist) [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power) [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power) [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws) [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone)

[F5] A finite product begins at the multiplicative identity and appends the next factor by multiplication. Real multiplication is associative with identity $1$, so the recursion for finite products applies. Induction on list length starts with the empty list and passes to the next length by appending one factor. [math:def-field](https://alphabetamath.cc/item/def-field) [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

## Proof

**Given:** The two prime classes, their positive-exponent bounds and the absent-prime option $1$ as in the Statement.

**Goal:** Compute $C_1^5$ and $C_2^5$ and verify both strict inequalities.

1.1 For a prime $t\ge32$ in either class, the corresponding $B_i(t)=1$ by the cutoff in [F1] and the presence of $1$ among the candidates. For a prime $t<32$ in either class, write $k$ for its maximizing positive exponent from [F1]. The maximum $B_i(t)$ is the larger of $1$ and the bound at exponent $k$. Both candidates are positive. Since fifth powers preserve order, $B_i(t)^5$ is the larger of $1$ and the fifth power of the bound at $k$. [given, F1, F2, F3, F4]

2.1 For positive $x,y$, $(x/y)y=x$, so $(x/y)^5y^5=x^5$ and $(x/y)^5=x^5/y^5$. Also, rational multiplication gives $(k/5)\cdot5=k$ since the product of the representatives $(k,5)$ and $(5,1)$ is $(5k,5)$, equivalent to $(k,1)$. The composition law therefore gives $(t^{k/5})^5=t^k$ for $t>0$. Hence the fifth power of the positive-exponent bound at $k$ is $\frac{[p(k+1)]^5}{(p+1)^5p^k}$ for $p\in\mathcal P_3$ and $\frac{(k+1)^5}{q^k}$ for $q\in\mathcal P_1$. For the empty product the fifth power is $1^5=1$. Appending a positive factor $b$ to a positive prefix product $a$ gives $(ab)^5=a^5b^5$. Induction on product length therefore gives $C_1^5$ and $C_2^5$ as the products of the respective values $B_i(t)^5$. [given, F2, F3, F4, F5, step 1.1]

3.1 In prime order $3,7,11,19,23,31$, substitution of $k=4,2,1,1,1,1$ into the first formula gives $\frac{9375}{1024},\frac{83349}{32768},\frac{14641}{7776},\frac{130321}{100000},\frac{279841}{248832},\frac{923521}{1048576}$, respectively, by integer powers and cancellation. The first five numerators exceed their denominators, and $923521<1048576$. Thus the last fifth-power factor is replaced by $1$. Multiplying the first five fractions yields $C_1^5=\frac{9375\cdot83349\cdot14641\cdot130321\cdot279841}{1024\cdot32768\cdot7776\cdot100000\cdot248832}=\frac{7^3\,11^4\,19^4\,23^4}{2^{45}3^4}=\frac{183143120027364343}{2849934139195392}$. [F1, F2, F3, F4, step 1.1, step 2.1]

3.2 In prime order $5,13,17,29$, substitution of $k=2,1,1,1$ gives $\frac{243}{25},\frac{32}{13},\frac{32}{17},\frac{32}{29}$, respectively. Each numerator exceeds its denominator, so all four values are retained. Their product is $C_2^5=\frac{243\cdot32^3}{25\cdot13\cdot17\cdot29}=\frac{7962624}{160225}$. [F1, F2, F3, F4, step 1.1, step 2.1]

4.1 Since $23^5=6436343$ and $10^5=100000$, the first comparison follows by multiplying by the two positive denominators. The integer difference $2849934139195392\cdot6436343-183143120027364343\cdot100000=28841644534852631456$ is positive. For the second comparison, $11^5=161051$ and $5^5=3125$, and the integer difference $160225\cdot161051-7962624\cdot3125=921196475$ is positive. These comparisons and the product evaluations prove both asserted equalities and strict bounds. [F2, F3, F4, step 2.1, step 3.1, step 3.2] ∎

## Source notes

Lemma 5.1 on page 5 supplies the attribution for the absent-prime convention and the two displayed fractions. The proof above uses the separate cutoff and maximizing-exponent results, then evaluates and compares the fractions by exact integer arithmetic. [Lemma 5.1](https://hexagonmath.org/pdf/2611.00370v1#page=5)

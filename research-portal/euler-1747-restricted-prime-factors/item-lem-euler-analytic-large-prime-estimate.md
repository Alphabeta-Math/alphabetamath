---
title: Large-prime contribution above the analytic threshold
status: published
research_item: lem-euler-analytic-large-prime-estimate
dependency_level: 6
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 6, Proposition 6.1, equation (6.2), and p. 7, opening sentence
---

PDF p. 6: ` Proposition 6.1, equation (6.2) `; PDF p. 7: ` §6, prime-count term preceding the numerical closure `

## Prerequisites

- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [def-euler-four-square-representations](item-def-euler-four-square-representations)
- [def-euler-mixed-four-square-representations](item-def-euler-mixed-four-square-representations)
- [def-euler-prime-obstruction-count](item-def-euler-prime-obstruction-count)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-of-q-embeds](https://alphabetamath.cc/item/lem-of-q-embeds)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)
- [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone)
- [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [lem-euler-obstructing-prime-count](item-lem-euler-obstructing-prime-count)
- [lem-euler-four-square-count-lower-bound](item-lem-euler-four-square-count-lower-bound)
- [def-euler-two-square-counts](item-def-euler-two-square-counts)
- [lem-euler-arithmetic-factor-bounds](item-lem-euler-arithmetic-factor-bounds)
- [math:lem-finite-sum-laws](https://alphabetamath.cc/item/lem-finite-sum-laws)
- [math:def-series](https://alphabetamath.cc/item/def-series)
- [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit)
- [lem-euler-obstructing-prime-square-tail](item-lem-euler-obstructing-prime-square-tail)
- [lem-euler-large-prime-obstruction-sum](item-lem-euler-large-prime-obstruction-sum)


## Statement

Let $n=2m\ge64^4$ with $m$ a positive odd integer, so $m>0$ and $m=2j+1$ for some integer $j$. An integer $d$ divides an integer $a$ if $a=dk$ for some integer $k$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Write $\mathcal P_3$ for the primes $p$ congruent to $3$ modulo $4$, meaning that $4$ divides $p-3$. Assume that every prime dividing $m$ belongs to $\mathcal P_3$.

Let $R(n)$ count ordered integer quadruples $(x_1,x_2,x_3,x_4)$ with $x_1^2+x_2^2+x_3^2+x_4^2=n$, allowing either sign and zero. An even integer has the form $2j$ for an integer $j$. For $p\in\mathcal P_3$, let $b_p(n)$ count the quadruples with one even and one odd entry in each of $(x_1,x_2)$ and $(x_3,x_4)$ for which at least one of these pairs has both entries divisible by $p$. Each qualifying quadruple is counted once.

Use real arithmetic and order, with integer values and counts included by the usual maps that preserve arithmetic and order. Nonnegative integer powers are repeated products starting at exponent zero with value $1$. For a positive real $a$, $a^{r/s}$ is the $r$th integer power of the unique positive $s$th root of $a$ for integers $r$ and $s>0$, with negative powers taken by reciprocation. Set $X=n^{1/4}$ and $P=2X$, and let $\sqrt n$ denote the nonnegative square root of $n$.

A set is finite if its elements can be listed exactly once each in $k$ positions for some nonnegative integer $k$. Write $\#S$ for this count for a finite set $S$. The set of primes $p\in\mathcal P_3$ with $P<p\le\sqrt n$ is finite and satisfies
$$\frac{\#\{p\in\mathcal P_3:P<p\le\sqrt n\}}{n}\le\frac{2}{15\sqrt n}+\frac1n.$$

The sum of $b_p(n)$ over $p>P$ in $\mathcal P_3$ has only finitely many nonzero terms, and is formed by adding each such term once, with empty sum $0$. Then
$$\frac1{R(n)}\sum_{\substack{p>P\\p\in\mathcal P_3}} b_p(n)\le\frac{44}{15}X^{4/5}\left(\frac1{15X}+\frac1{2X^2}+\frac2{15X^2}+\frac1{X^4}\right)=\frac{44}{15}X^{-1/5}\left(\frac1{15}+\frac{19}{30X}+\frac1{X^3}\right).$$

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[def-euler-four-square-representations](item-def-euler-four-square-representations)

[def-euler-mixed-four-square-representations](item-def-euler-mixed-four-square-representations)

[def-euler-prime-obstruction-count](item-def-euler-prime-obstruction-count)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-of-q-embeds](https://alphabetamath.cc/item/lem-of-q-embeds)

[math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

[math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)

[math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

## Facts & Assumptions

[F1] The reals form a complete ordered field. Addition and multiplication are associative and commutative, with identities $0$ and $1>0$, and $a(b+c)=ab+ac$. Every real has an additive inverse, and each nonzero real has a multiplicative inverse, also called its reciprocal. Completeness means every nonempty set of reals bounded above has a smallest real upper bound. In its total order, adding the same real or multiplying by a positive real preserves inequalities. A quotient $a/b$ for $b\ne0$ is the product of $a$ and the reciprocal of $b$. The reciprocal of $b$ is positive if $b>0$. [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field) [math:def-field](https://alphabetamath.cc/item/def-field) [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)

[F2] The usual inclusions from the natural numbers into the integers, integers into rationals, and rationals into the real ordered field preserve arithmetic and order. The natural numbers are represented by the nonnegative integers. [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-of-q-embeds](https://alphabetamath.cc/item/lem-of-q-embeds)

[F3] In the complete ordered field, for a positive base $a$ and positive integer $s$, there is a unique nonnegative $s$th root, and it is positive. In particular $a^{1/2}=\sqrt a$. On nonnegative bases the fourth power preserves and reflects order. For a positive real $a$ and rational exponents $v,w$, the powers obey $(a^v)^w=a^{vw}$ and $a^{v+w}=a^va^w$. A rational exponent equal to an integer agrees with the integer power. [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist) [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power) [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power) [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone) [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)

[F4] Restricting a set by a membership condition selects a subset of it. A subset $B$ of a finite set $A$ is finite and $\#B\le\#A$. [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F5] For every real $t\ge0$, the set $\{p\in\mathcal P_3:3<p\le t\}$ is finite and has at most $2t/15+1$ elements. [lem-euler-obstructing-prime-count](item-lem-euler-obstructing-prime-count)

[F6] For $n=2m$ with $m$ a positive integer for which no integer $q$ satisfies $m=2q$, $R(n)\ge12n$. [lem-euler-four-square-count-lower-bound](item-lem-euler-four-square-count-lower-bound)

[F7] For a positive integer $n$, let $M(n)$ be the greatest value attained over integers $1\le u\le n$ by the following product. Take one factor $e+1$ per prime $q$ for which $4$ divides $q-1$ and $q^e$ divides $u$ but $q^{e+1}$ does not, with $e\ge1$ an integer. The product is finite and has value $1$ when empty. Under the hypotheses on $n$ and $m$ in the Statement, $M(n)\le(11/5)n^{1/5}$. A finite product of positive real factors is positive. [def-euler-two-square-counts](item-def-euler-two-square-counts) [lem-euler-arithmetic-factor-bounds](item-lem-euler-arithmetic-factor-bounds) [math:lem-finite-sum-laws](https://alphabetamath.cc/item/lem-finite-sum-laws) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[F8] For real $P\ge3$, let $T(P)$ denote the sum of the convergent series of terms indexed by $k=0,1,2,\ldots$ that equal $1/k^2$ when $k\in\mathcal P_3$ and $k>P$, and $0$ otherwise. Its value is the limit of the sums of the first $N$ terms. A limit means that, for every positive rational tolerance, all sufficiently late sums differ from it by less than that tolerance in absolute value. The absolute value of a nonnegative real is the number itself, and the absolute value of a negative real is its negative. The bound is $T(P)\le 2/(15P)+2/P^2$. [math:def-series](https://alphabetamath.cc/item/def-series) [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit) [lem-euler-obstructing-prime-square-tail](item-lem-euler-obstructing-prime-square-tail)

[F9] For $n=2m$ with $m$ a positive odd integer whose prime divisors lie in $\mathcal P_3$, and real $P\ge3$, the sum on the left has only finitely many nonzero terms and satisfies
$$\frac1{R(n)}\sum_{\substack{p>P\\p\in\mathcal P_3}} b_p(n)\le\frac43M(n)\left(T(P)+\frac{\#\{p\in\mathcal P_3:P<p\le\sqrt n\}}{n}\right).$$
[lem-euler-large-prime-obstruction-sum](item-lem-euler-large-prime-obstruction-sum)

[F10] For every integer $a$, there is exactly one pair of integers $q,r$ with $a=2q+r$ and $0\le r<2$. [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

## Proof

**Given:** The integers $m,n$ and the real numbers $X,P$ from the Statement.

**Goal:** Prove the divided prime-count bound and then the displayed bound for the normalized sum, meaning the sum divided by $R(n)$.

1.1 Since $n\ge64^4>0$, its positive fourth root $X$ satisfies $X^4=n$. Comparing fourth powers of the nonnegative bases $64$ and $X$ gives $X\ge64$, so $P=2X\ge128>3$. The power laws give $X^2=n^{1/2}=\sqrt n$ and $n^{1/5}=(X^4)^{1/5}=X^{4/5}$. All of $n$, $X$ and $\sqrt n$ are positive. [given, F1, F2, F3]

2.1 Every prime counted by $\#\{p\in\mathcal P_3:P<p\le\sqrt n\}$ also satisfies $3<p\le\sqrt n$ because $P>3$. Apply [F5] with $t=\sqrt n\ge0$ and [F4] to this subset. It is finite, and its count $N$ is at most $2\sqrt n/15+1$. Dividing by $n>0$ and using $(\sqrt n)^2=n$ yields $N/n\le 2/(15\sqrt n)+1/n$. [F1, F2, F3, F4, F5, step 1.1]

3.1 The expression $m=2j+1$ gives remainder $1$ on division by $2$, since $0\le 1<2$. An equality $m=2q$ with $q$ an integer would give remainder $0$, contrary to uniqueness in [F10]. Therefore [F6] gives $R(n)\ge12n>0$. By [F9] the sum is finite in the stated sense and its quotient by $R(n)$ is at most $(4/3)M(n)(T(P)+N/n)$. Each factor $e+1$ in [F7] is positive, so every product there is positive and its attained greatest value $M(n)$ is positive as well. [given, F1, F2, F6, F7, F9, F10, step 1.1, step 2.1]

4.1 Since $P\ge3$, [F8] gives $T(P)\le1/(15X)+1/(2X^2)$ after substituting $P=2X$. By Step 2.1 and the identities from Step 1.1, $N/n\le2/(15X^2)+1/X^4$. The sum of these two upper bounds is the positive number $B=1/(15X)+1/(2X^2)+2/(15X^2)+1/X^4$. Multiplying the comparison $T(P)+N/n\le B$ by the positive factor $(4/3)M(n)$ preserves it. [F1, F2, F8, step 1.1, step 2.1, step 3.1]

5.1 Use $B>0$ and $M(n)\le(11/5)X^{4/5}$ from [F7] and Step 1.1 to bound $(4/3)M(n)B$ by $(44/15)X^{4/5}B$. By the power laws $X^{4/5}=X^{-1/5}X$. Multiplying $B$ by $X$ and adding the two terms with denominator proportional to $X$ gives $XB=1/15+19/(30X)+1/X^3$, since $1/2+2/15=19/30$. This proves the claimed bound in both forms, and Step 2.1 proves the divided prime-count estimate. [F1, F2, F3, F7, step 1.1, step 2.1, step 3.1, step 4.1] ∎

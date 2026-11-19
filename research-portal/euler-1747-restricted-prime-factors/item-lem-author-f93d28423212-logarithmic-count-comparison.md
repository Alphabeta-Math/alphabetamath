---
title: The logarithmic lower bound eventually exceeds the exclusion bound
status: draft
research_item: lem-author-f93d28423212-logarithmic-count-comparison
dependency_level: 0
---

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-natural-logarithm](https://alphabetamath.cc/item/def-natural-logarithm)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:lem-natural-logarithm-bounded-by-argument](https://alphabetamath.cc/item/lem-natural-logarithm-bounded-by-argument)
- [math:thm-natural-logarithm-laws](https://alphabetamath.cc/item/thm-natural-logarithm-laws)
- [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)
- [math:lem-rational-power-monotone](https://alphabetamath.cc/item/lem-rational-power-monotone)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:lem-ceiling-and-least-positive-integer-threshold](https://alphabetamath.cc/item/lem-ceiling-and-least-positive-integer-threshold)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)
- [math:def-real-exponential-function-and-e](https://alphabetamath.cc/item/def-real-exponential-function-and-e)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)
- [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)
- [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)


## Statement

For positive real numbers $c,K$ there is an integer $M\ge2$ such that every integer $n\ge M$ satisfies $c n/(\log n)^{5/2}>K n^{13/16}$. In real expressions, integers denote their images under the canonical embeddings through the rationals. Here $\log$ is the natural logarithm, the inverse of the real exponential. For positive real $t$, integer $a$, and nonzero natural $b$, the rational power $t^{a/b}$ is the $a$th integer power of the positive $b$th root of $t$.

## Statement references

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-natural-logarithm](https://alphabetamath.cc/item/def-natural-logarithm)

[math:def-real-exponential-function-and-e](https://alphabetamath.cc/item/def-real-exponential-function-and-e)

[math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

[math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)

[math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)

[math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)

[math:thm-natural-logarithm-laws](https://alphabetamath.cc/item/thm-natural-logarithm-laws)

## Facts & Assumptions

[F1] The natural logarithm is strictly increasing, $\log 1=0$, $\log(uv)=\log u+\log v$ for positive $u,v$, and $0\le\log u\le u-1$ for $u\ge1$. [math:def-natural-logarithm](https://alphabetamath.cc/item/def-natural-logarithm) [math:thm-natural-logarithm-laws](https://alphabetamath.cc/item/thm-natural-logarithm-laws) [math:lem-natural-logarithm-bounded-by-argument](https://alphabetamath.cc/item/lem-natural-logarithm-bounded-by-argument)

[F2] Rational powers of positive numbers are positive and obey the product, sum-of-exponents and iterated-power laws. Raising a positive number to a fixed positive rational power is strictly increasing. If the base is greater than $1$, the power is greater than $1$. [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power) [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws) [math:lem-rational-power-monotone](https://alphabetamath.cc/item/lem-rational-power-monotone) [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order)

[F3] Every nonnegative real number has a ceiling, the least integer whose real image is at least that number. [math:lem-ceiling-and-least-positive-integer-threshold](https://alphabetamath.cc/item/lem-ceiling-and-least-positive-integer-threshold)

[F4] The integer embedding $k\mapsto k/1$ into the rationals and the constant-sequence embedding of the rationals into the reals preserve order and arithmetic. A nonzero natural $b$ gives a positive integer denominator under the natural-to-integer embedding. [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[F5] The integers are a totally ordered ring. In particular, $2=1+1>1$, and adding the positive integer $1$ to an integer $C$ gives an integer $C+1>C$. [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[F6] In the real ordered field, products of positive numbers are positive and multiplication by a positive number preserves order. Every positive number $d$ has a positive inverse $d^{-1}$. Division by a nonzero number is multiplication by its inverse, so division by a positive number preserves order. Rational exponent sums and products are computed by the fraction rules. [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field) [math:def-field](https://alphabetamath.cc/item/def-field) [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive) [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)

[F7] The Cauchy-sequence reals have the least-upper-bound property, so they form a complete ordered field. For each positive real $x$ and each natural index $b\ge1$ in the natural-number order, the root theorem gives a unique positive $s$ with $s^b=x$. [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete) [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field) [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[F8] A natural power is a repeated product, with $x^1=x$. For a positive base and a natural $b\ge1$, the rational power with exponent $1/b$ equals the positive $b$th root. For a positive base $x$, the rational power with integer exponent $a$ uses the representative $a/1$. The first root of $x$ equals $x$, so this rational power agrees with the integer power. [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power) [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power) [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

## Proof

**Given:** Positive real constants $c,K$.

**Goal:** Find a common integer threshold for the strict inequality.

1.1 For an integer $n\ge2$, its real image satisfies $n\ge2>1$. Thus $t=n^{1/16}>1$. The natural index $16$ satisfies $16\ge1$, so in the complete real field this power is the positive sixteenth root of $n>0$ and $t^{16}=n$. The logarithm is positive at $n$, and applying the product law to the sixteen factors of $t^{16}$ gives $0<\log n=16\log t\le16t$. [F1, F2, F4, F5, F6, F7, F8]

1.2 Put $A=16^{5/2}K/c$, which is positive because $16^{5/2}$, $K$ and $c^{-1}$ are positive. Agreement of the power definitions and positivity of rational powers give $A^{32}>0$. Take $C=\lceil A^{32}\rceil$, so $C$ is an integer and $C\ge A^{32}$ in the real order. If $C+1\ge2$ in the integer order take $M=C+1$, and otherwise take $M=2$. In either case $M\ge2$ and $M\ge C+1$ in the integer order. For every integer $n\ge M$ we have $n\ge M\ge C+1>C$ in that order. Transferring this chain to the reals gives $n>C\ge A^{32}$. [given, F2, F3, F4, F5, F6, F8]

2.1 For an integer $n\ge2$, raise the logarithmic bound from step 1.1 to the positive rational power $5/2$. The power laws and $(1/16)(5/2)=5/32$ give $0<(\log n)^{5/2}\le16^{5/2}n^{5/32}$. Since $5/32+27/32=1$, the power sum law gives $n=n^{5/32}n^{27/32}$. Write $U=(\log n)^{5/2}$ and $V=16^{5/2}n^{5/32}$. Multiplying $U\le V$ by $cn>0$ gives $cnU\le cnV$. Since $UV>0$, its inverse is positive, so multiplying both sides by $(UV)^{-1}$ gives $cn/V\le cn/U$. Cancelling the positive factor $n^{5/32}$ in $cn/V$ gives $c n/(\log n)^{5/2}\ge(c/16^{5/2})n^{27/32}$. [given, step 1.1, F2, F6, F8]

3.1 For an integer $n\ge M$, step 1.2 gives $n>A^{32}>0$. The root theorem applies in the complete real field to $A^{32}>0$ with natural index $32\ge1$. Since $A>0$ and its thirty-second power is $A^{32}$, uniqueness gives $(A^{32})^{1/32}=A$. Strict monotonicity of the $1/32$ power then gives $n^{1/32}>A$. By the fraction rules, $13/16+1/32=(26+1)/32=27/32$, so $n^{27/32}=n^{13/16}n^{1/32}$. Multiplying the strict inequality by $(c/16^{5/2})n^{13/16}>0$ gives $(c/16^{5/2})n^{27/32}>K n^{13/16}$. Together with step 2.1 this proves the strict comparison for every integer $n\ge M$. [given, step 1.2, step 2.1, F2, F6, F7, F8] ∎

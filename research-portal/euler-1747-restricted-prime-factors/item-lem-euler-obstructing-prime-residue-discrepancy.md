---
title: Periodic discrepancy for the eight residue classes
status: published
research_item: lem-euler-obstructing-prime-residue-discrepancy
dependency_level: 1
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: PDF p. 6, proof of Lemma 5.2, from the one-period check through the
        interval estimate
---

PDF p. 6: ` Lemma 5.2, one-period check and interval estimate `

## Prerequisites

- [def-euler-obstructing-prime-residue-count](item-def-euler-obstructing-prime-residue-count)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [lem-periodic-residue-count-discrepancy](item-lem-periodic-residue-count-discrepancy)
- [math:def-one-sided-limits](https://alphabetamath.cc/item/def-one-sided-limits)
- [math:def-neighbourhood-r](https://alphabetamath.cc/item/def-neighbourhood-r)
- [math:def-limit-point-r](https://alphabetamath.cc/item/def-limit-point-r)
- [math:def-abs-value](https://alphabetamath.cc/item/def-abs-value)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:lem-of-abs-value](https://alphabetamath.cc/item/lem-of-abs-value)


## Statement

For a real cutoff $t\ge0$, let $A(t)$ be the finite number of positive integers $k\le t$ congruent modulo $60$ to one of $7,11,19,23,31,43,47,59$. Here positive means $k>0$, and congruence to $r$ means $k-r=60q$ for some integer $q$. Integers are regarded as reals by the usual inclusion preserving order and arithmetic. Use the usual inclusions from the natural numbers into the integers, from the integers into the rationals, and from the rationals into the reals to interpret the count $A(t)$ in real arithmetic. Set $E(t)=A(t)-2t/15$.

The discrepancy $E$, the difference between the count and $2t/15$, has period $60$, meaning $E(t+60)=E(t)$ for every real $t\ge0$. For all such $t$,
$$-\frac{14}{15}\le E(t)\le\frac{14}{15}.$$

For real $t\ge P\ge3$,
$$A(t)-A(P)\le\frac{2}{15}(t-P)+2.$$

## Statement references

[def-euler-obstructing-prime-residue-count](item-def-euler-obstructing-prime-residue-count)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)

[math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

## Facts & Assumptions

[F1] The finite count $A(x)$ for $x\ge0$ is the number of positive integers $k\le x$ whose difference from one of the eight listed representatives is an integer multiple of $60$ ([def-euler-obstructing-prime-residue-count](item-def-euler-obstructing-prime-residue-count), [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer), [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)).

[F2] For a positive integer $M$ and $D\subseteq\{1,\ldots,M\}$, for each integer $k$ let $r_M(k)$ be the unique integer $d\in\{1,\ldots,M\}$ such that $k-d$ is an integer multiple of $M$. Put $A_D(x)=\#\{k\in\mathbb Z:1\le k\le x,\ r_M(k)\in D\}$ and $E_D(x)=A_D(x)-|D|x/M$ for $x\ge0$. The subset symbol and the set defining $A_D$ use inclusion and separation ([math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)). Here $\#$ and $|D|$ denote natural-number cardinalities, with their real images used in the formula for $E_D$. Then $E_D$ has period $M$. Its jumps in $0<x\le M$, where its limits from the two sides exist and differ, are exactly the points of $D$. If $B\ge0$ bounds the absolute values at $0$ and $M$ and of both one-sided limits at every point of $D$, then $|E_D(x)|\le B$ for every $x\ge0$ ([lem-periodic-residue-count-discrepancy](item-lem-periodic-residue-count-discrepancy)).

[F3] In the ordered field of real numbers, adding the same number preserves order and multiplying by the same positive number preserves order ([math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field), [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)). The canonical inclusions from the natural numbers into the integers, from the integers into the rationals, and from the rationals into the reals preserve order and arithmetic ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int), [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat), [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)). These maps use the natural numbers of [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) and the rationals of [math:def-rationals](https://alphabetamath.cc/item/def-rationals). Use the corresponding real images whenever natural-number counts occur in real arithmetic.

[F4] The absolute value $|y|$ of a real $y$ is $y$ when $y\ge0$ and $-y$ when $y<0$ ([math:def-abs-value](https://alphabetamath.cc/item/def-abs-value)). For a real radius $\eta>0$, the punctured $\eta$-neighbourhood of $d$ consists of the real points $x$ with $0<|x-d|<\eta$ ([math:def-neighbourhood-r](https://alphabetamath.cc/item/def-neighbourhood-r)). For a real-valued function $f$ with domain the nonnegative reals ([math:def-function](https://alphabetamath.cc/item/def-function)), $d$ is a limit point on a specified side when every punctured neighbourhood of $d$ meets the domain on that side ([math:def-limit-point-r](https://alphabetamath.cc/item/def-limit-point-r)). The left side means $x<d$ and the right side means $x>d$. At such a point the limit on that side is $L$ if for every $\varepsilon>0$ some $\delta>0$ gives $|f(x)-L|<\varepsilon$ for all points on that side with $0<|x-d|<\delta$ ([math:def-one-sided-limits](https://alphabetamath.cc/item/def-one-sided-limits)).

[F5] The integers form a commutative ring with the usual operations, so for every integer $k$, $k-k=0$ and $60\cdot0=0$ ([math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)).

[F6] For real numbers $u,v$, absolute value satisfies $|uv|=|u|\,|v|$ ([math:lem-of-abs-value](https://alphabetamath.cc/item/lem-of-abs-value)).

## Proof

**Given:** The counting function $A$ and discrepancy $E$ in the statement.

**Goal:** Establish the period, the two-sided discrepancy bound, and the estimate for $A(t)-A(P)$.

1.1 In [F2] take $M=60$ and let $D=\{7,11,19,23,31,43,47,59\}$. Its eight distinct elements lie in $\{1,\ldots,60\}$. For each positive integer $k$, membership of $r_{60}(k)$ in $D$ is equivalent to congruence to a listed $r$, since such an $r$ lies in $\{1,\ldots,60\}$ and congruence gives exactly the defining condition $k-r=60q$ for some integer $q$. Uniqueness identifies $r$ with $r_{60}(k)$. Thus $A_D(x)=A(x)$ for $x\ge0$. Using the real images of the counts as in [F3], we have $|D|/60=8/60=2/15$ and therefore $E_D=E$. The period assertion of [F2] gives $E(t+60)=E(t)$ for every $t\ge0$. [F1, F2, F3]

2.1 For $0\le x\le60$, each integer $1\le k\le x$ is its own representative $r_{60}(k)$, because $k\in\{1,\ldots,60\}$ and $k-k=0=60\cdot0$ with integer multiplier $0$. Hence $A(x)$ counts exactly the members of $D$ at most $x$. In particular $A(0)=0$ and $A(60)=8$, giving $E(0)=E(60)=0$. Write $d_i$ for the $i$th listed member of $D$ in increasing order, with $1\le i\le8$. Successive listed members differ by at least $4$, and $7\le d_i\le59$. Consequently $A(x)=i-1$ for $d_i-1<x<d_i$, and $A(x)=i$ for $d_i\le x<d_i+1$. [F1, F2, F3, F5, step 1.1]

3.1 For any $\eta>0$, let $h=\eta/(2(1+\eta))$. Then $0<h<1$ and $h<\eta$. Since $E$ has domain the nonnegative reals and $d_i\ge7$, the inequalities $0\le d_i-h<d_i<d_i+h$ put $d_i-h$ and $d_i+h$ in the domain on opposite sides of $d_i$. Both points have distance $h$ from $d_i$ and belong to the punctured $\eta$-neighbourhood of $d_i$ by [F4]. Since $\eta>0$ was arbitrary, $d_i$ is a limit point of each side of the domain. Define $L_i^-=i-1-2d_i/15$ and $L_i^+=i-2d_i/15$. On the respective sides where $0<|x-d_i|<1$, step 2.1 gives $E(x)-L_i^\pm=-(2/15)(x-d_i)$. The product rule [F6] and $|-2/15|=2/15$ from [F4] give $|E(x)-L_i^\pm|=(2/15)|x-d_i|$. For any $\varepsilon>0$, taking $\delta=\varepsilon/(1+\varepsilon)$ gives $0<\delta<1$ and $\delta<\varepsilon$. Since $0<2/15<1$, the difference is less than $\varepsilon$ on each respective side whenever $0<|x-d_i|<\delta$. Hence $L_i^-$ and $L_i^+$ are the left and right limits, respectively. [F3, F4, F6, step 2.1]

4.1 In the listed order of the $d_i$, the values of $15L_i^-=15(i-1)-2d_i$ are $(-14,-7,-8,-1,-2,-11,-4,-13)$, and the values of $15L_i^+=15i-2d_i$ are $(1,8,7,14,13,4,11,2)$. All sixteen values lie between $-14$ and $14$. Together with $E(0)=E(60)=0$, these values meet the hypotheses of [F2] with $B=14/15$. Therefore $|E(t)|\le14/15$ for all real $t\ge0$, which is the claimed two-sided bound. [F2, F3, F4, step 1.1, step 2.1, step 3.1]

5.1 For real $t\ge P\ge3$, both arguments are nonnegative. Using the real interpretation of the counts from [F3] and the bounds $E(t)\le14/15$ and $E(P)\ge-14/15$ gives $A(t)-A(P)=\frac{2}{15}(t-P)+E(t)-E(P)\le\frac{2}{15}(t-P)+\frac{28}{15}\le\frac{2}{15}(t-P)+2$. This proves the interval estimate and completes the lemma. [F3, given, step 4.1] ∎

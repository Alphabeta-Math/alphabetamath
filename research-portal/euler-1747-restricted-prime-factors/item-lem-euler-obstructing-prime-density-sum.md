---
title: "Lemma 5.2: Summed main term over the obstructing primes"
status: draft
research_item: lem-euler-obstructing-prime-density-sum
dependency_level: 4
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 6, Lemma 5.2, equation (5.4) and final finite sum through 60
---

PDF p. 6: ` Lemma 5.2, equation (5.4) and final finite sum through 60 `

## Prerequisites

- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-sequence](https://alphabetamath.cc/item/def-sequence)
- [math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum)
- [math:def-series](https://alphabetamath.cc/item/def-series)
- [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit)
- [lem-euler-obstructing-prime-residue-inclusion](item-lem-euler-obstructing-prime-residue-inclusion)
- [lem-trial-division-primality-bound](item-lem-trial-division-primality-bound)
- [lem-euler-obstructing-prime-square-tail](item-lem-euler-obstructing-prime-square-tail)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:lem-finite-sum-laws](https://alphabetamath.cc/item/lem-finite-sum-laws)
- [math:thm-nonnegative-series-bounded-partial-sums](https://alphabetamath.cc/item/thm-nonnegative-series-bounded-partial-sums)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-rational-cauchy-sequence](https://alphabetamath.cc/item/def-rational-cauchy-sequence)
- [math:def-null-sequence](https://alphabetamath.cc/item/def-null-sequence)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)


## Statement

Let $\mathcal P_3$ be the set of primes congruent to $3$ modulo $4$, called the obstructing primes. An integer $p$ is prime if $p>1$ and its only positive divisors are $1$ and $p$. An integer $d$ divides $p$ if $p=dq$ for an integer $q$, and it is positive when $d>0$. Congruence to $3$ modulo $4$ means that $p-3=4j$ for an integer $j$.

Use the real numbers constructed as classes of rational Cauchy sequences modulo null sequences, with their canonical order. They form a commutative field whose total order is compatible with addition and multiplication and in which every nonempty set bounded above has a least upper bound. A least upper bound is the smallest of the numbers that bound the set above. A natural index is read as its image in the integers when testing primality. In real arithmetic, use the canonical inclusions of the naturals and integers into the reals through the rationals. For a nonzero real denominator $b$, $a/b$ denotes $a$ times the unique real number whose product with $b$ is $1$. We write $x^2=x\cdot x$.

For a sum restricted to primes, take the sequence of terms indexed by the natural numbers $0,1,2,\ldots$, setting the term to zero when the index fails the restriction. Order the natural indices by $k\le n$ when $k+j=n$ for some natural $j$, and by $k<n$ when also $k\ne n$. A partial sum through the indices $k<n$ starts at zero and adds the terms in increasing index order. An infinite series converges with sum $L$ if, for each positive rational $\varepsilon$, there is a natural $N$ such that for every natural $n\ge N$ the absolute difference between the partial sum and $L$ is less than the real image of $\varepsilon$. Here a rational is a quotient of integers with nonzero denominator, and the absolute value of a real number is the number itself when nonnegative and its negative otherwise. For the finite sum displayed below, take the partial sum over $k<61$, with term $2/[k(k-1)]$ at the nine listed indices and zero at all other indices.

The series on the left below converges, and the following bounds hold.
$$2\sum_{p\in\mathcal P_3}\frac{1}{p(p-1)}\le \sum_{p\in\{3,7,11,19,23,31,43,47,59\}}\frac{2}{p(p-1)}+\frac{120}{59}\left(\frac{2}{15\cdot60}+\frac{2}{60^2}\right)<\frac{21}{50}.$$
For each $p\in\mathcal P_3$ with $p>60$, the comparison factor satisfies $p/(p-1)\le60/59$.

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)

[math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:def-sequence](https://alphabetamath.cc/item/def-sequence)

[math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum)

[math:def-series](https://alphabetamath.cc/item/def-series)

[math:def-real-limit](https://alphabetamath.cc/item/def-real-limit)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-rational-cauchy-sequence](https://alphabetamath.cc/item/def-rational-cauchy-sequence)

[math:def-null-sequence](https://alphabetamath.cc/item/def-null-sequence)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

## Facts & Assumptions

[F1] Use the real numbers of [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers), constructed as classes of rational Cauchy sequences ([math:def-rational-cauchy-sequence](https://alphabetamath.cc/item/def-rational-cauchy-sequence)) modulo null sequences ([math:def-null-sequence](https://alphabetamath.cc/item/def-null-sequence)). With the order of [math:def-real-order](https://alphabetamath.cc/item/def-real-order) they form a complete ordered field by [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete). The real ordered field has $1>0$ and positive numbers are closed under addition and multiplication ([math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field), [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)). Real arithmetic obeys the commutative field laws ([math:def-field](https://alphabetamath.cc/item/def-field)). In particular, adding the same number to both sides preserves an inequality by cancellation in the difference, and multiplying by a positive number preserves it by multiplying the difference by that number. For $0<a<b$, the reciprocals satisfy $0<1/b<1/a$, and the reciprocal of any positive number is positive ([math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)). We identify natural numbers with the nonnegative integers by the order- and arithmetic-preserving map in [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int). Integers are included in the reals by the maps preserving order and arithmetic in [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) and [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense). Use the additive order on the naturals ([math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)). For natural $m$, the natural successor is $\sigma(m)=m\cup\{m\}$ with $1=\sigma(0)$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)). The addition recursion gives $m+1=m+\sigma(0)=\sigma(m+0)=\sigma(m)$ ([math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)). Thus for natural $k,m$, $k<m+1$ exactly when $k\le m$, and the indices less than $m+1$ are the members of $m+1=\{0,\ldots,m\}$ ([math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership), parts 1 and 3).

[F2] By [def-euler-prime-classes](item-def-euler-prime-classes), membership in $\mathcal P_3$ requires a prime with $p-3$ divisible by $4$. For $p\in\mathcal P_3$ with $p>3$, its remainder modulo $60$ belongs to $\{7,11,19,23,31,43,47,59\}$ by [lem-euler-obstructing-prime-residue-inclusion](item-lem-euler-obstructing-prime-residue-inclusion). For any integer $v$ and positive integer $d$ the remainder is the unique $r$ in a decomposition $v=dq+r$ with integers $q,r$ and $0\le r<d$ ([math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)). The remainder is zero exactly when $d$ divides $v$, by this uniqueness and the definition of divisibility ([math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)).

[F3] By [lem-trial-division-primality-bound](item-lem-trial-division-primality-bound), an integer $p>1$ is prime if no integer $d$ with $2\le d\le\lfloor\sqrt{p}\rfloor$ divides it. In the reals of [F1], the square root $\sqrt{p}$ is the nonnegative real whose square is $p$, and the floor $\lfloor x\rfloor$ is the unique integer $m$ with $m\le x<m+1$.

[F4] The reciprocal-square series over $p\in\mathcal P_3$ with $p>60$ converges with sum at most $2/(15\cdot60)+2/60^2$, by [lem-euler-obstructing-prime-square-tail](item-lem-euler-obstructing-prime-square-tail) with real cutoff $60\ge3$.

[F5] Finite real sums preserve termwise weak inequalities, distribute over termwise addition, and allow a constant multiplier to be taken outside the sum. For natural $n\ge m$, the sum over $k<n$ splits into the sum over $k<m$ and the sum over $m\le k<n$ ([math:lem-finite-sum-laws](https://alphabetamath.cc/item/lem-finite-sum-laws), parts 1–4).

[F6] For a sequence of nonnegative real terms the partial sums are nondecreasing, meaning that increasing the upper index cannot decrease the sum. The series converges exactly when those sums are bounded above and then its sum is their least upper bound ([math:thm-nonnegative-series-bounded-partial-sums](https://alphabetamath.cc/item/thm-nonnegative-series-bounded-partial-sums), parts 1–2).

## Proof

**Given:** The prime class $\mathcal P_3$ and the real arithmetic and summation conventions of the Statement.

**Goal:** Show convergence, the displayed bounds, and the comparison factor for $p>60$.

1.1 Set $E=\{3,7,11,19,23,31,43,47,59\}$. A member $p$ of $\mathcal P_3$ is a positive integer. If $p\le3$, then the numbers less than $4$ with $p>1$ are $2$ and $3$, and $2$ has remainder $2$ on division by $4$, so only $3$ qualifies. If $3<p<60$, then its remainder on division by $60$ is $p$ itself by the decomposition with quotient zero. By [F2] it is one of the eight entries of $E$ above $3$. The case $p=60$ has remainder zero on division by $60$ and is excluded by [F2]. Thus every member of $\mathcal P_3$ at most $60$ belongs to $E$. [given, F1, F2]

1.2 For $p\in\mathcal P_3$ with $p>60$, one has $0<59<p-1$. By reciprocal comparison, $\frac{p}{p-1}=1+\frac{1}{p-1}<1+\frac{1}{59}=\frac{60}{59}$. Since $p^2>0$, it follows that $2/[p(p-1)]=(2/p^2)\,p/(p-1)\le(120/59)/p^2$. [F1]

2.1 For the reverse inclusion, the entries of $E$ in increasing order are $4j+3$ for $j=0,1,2,4,5,7,10,11,14$, respectively. Each exceeds $1$ and is at most $60$. For a tested divisor $d$ in [F3], work in the ordered field of [F1]. The inequalities $0<d\le\sqrt p$ imply $d^2\le p$ since $(\sqrt p-d)(\sqrt p+d)=p-d^2\ge0$. If $d\ge8$ then $(d-8)(d+8)\ge0$, giving $d^2\ge8^2=64>60$. Hence $d<8$. Since $d$ is a nonnegative integer, the order-preserving identification in [F1] and the natural successor comparison at $m=7$ give $d\le7$. For $d=2$ the checked remainders are all $1$, and for $d=4$ they are all $3$, by $p=4j+3$. For $d=3$, the entries $p\ge9$ have remainders $(2,1,2,1,1,2,2)$ in increasing order of $p$. For $d=5$, the entries $p\ge25$ have remainders $(1,3,2,4)$. For $d=6$, the entries $p\ge36$ have remainders $(1,5,5)$. For $d=7$, the only entry $p\ge49$ is $59=7\cdot8+3$. All tested remainders are nonzero, so every entry of $E$ is prime by [F3]. The congruences above therefore give $\{p\in\mathcal P_3:p\le60\}=E$. [given, F1, F2, F3, step 1.1]

2.2 For each natural index $k$, define $u_k=1/[k(k-1)]$ if $k\in\mathcal P_3$ and $u_k=0$ otherwise. Put $h_k=2u_k$ if $k\le60$ and $h_k=0$ otherwise. Put $b_k=1/k^2$ if $k>60$ and $k\in\mathcal P_3$, and $b_k=0$ otherwise. All three sequences have nonnegative terms because the denominators used are products of positive numbers. Write $C=120/59$, $B=2/(15\cdot60)+2/60^2$ and $H=\sum_{p\in E}2/[p(p-1)]$. If $k\le60$, then $2u_k=h_k$ and $b_k=0$. If $k>60$ and $k\in\mathcal P_3$, step 1.2 gives $2u_k\le Cb_k$ and $h_k=0$. The other indices have all three terms zero. Thus $2u_k\le h_k+Cb_k$ for every $k$. [given, F1, step 1.2]

3.1 Apply [F1] at $m=60$ to identify $k<61$ with $k\le60$. For $n\ge61$, the sum of $h_k$ over $k<61$ equals $H$ by the finite-sum convention in the Statement, the identification of $E$ in step 2.1 and the definition of $h_k$ in step 2.2. All terms with $k\ge61$ are zero, so [F5] gives $\sum_{k<n}h_k=H$. The sum of $b_k$ over $k<n$ is at most its series sum by [F6], and that sum is at most $B$ by [F4]. By [F5] and $C>0$, $2\sum_{k<n}u_k\le\sum_{k<n}h_k+C\sum_{k<n}b_k\le H+CB$. For $n<61$, the same bound follows because the partial sum of the nonnegative $u_k$ through $k<n$ is at most the one through $k<61$. Thus $(H+CB)/2$ is an upper bound for all partial sums of the $u_k$. By [F6] the series converges and its sum is at most $(H+CB)/2$. Multiplying by $2$ gives the weak inequality in the Statement. [given, F1, F4, F5, F6, step 2.1, step 2.2]

4.1 To check the strict inequality, the denominators $p(p-1)$ of the summands in $H$, in increasing order of $p$, are $(6,42,110,342,506,930,1806,2162,3422)$. The corresponding integers $(3334,477,182,59,40,22,12,10,6)$ have sum $4142$. Their products with the respective denominators are $(20004,20034,20020,20178,20240,20460,21672,21620,20532)$, each at least $20000$. Dividing each product inequality by $10000p(p-1)>0$ and summing gives $H\le4142/10000$. Also $B=1/360$ and $CB=1/177$. Since $21/50-4142/10000=29/5000$ and $29\cdot177=5133>5000$, one has $1/177<29/5000$. Consequently $H+CB<21/50$, completing the bounds and the convergence claim. [F1, F5, step 2.1, step 2.2, step 3.1] ∎

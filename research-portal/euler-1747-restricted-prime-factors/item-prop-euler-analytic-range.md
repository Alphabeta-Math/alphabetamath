---
title: "Proposition 6.1: The analytic range"
status: published
research_item: prop-euler-analytic-range
dependency_level: 15
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, Abstract and paragraph after Theorem 1.1, p. 2, equations
        (2.2)–(2.3), pp. 6–7, Proposition 6.1
      reading_limits: Consulted the frozen text at these locators and the rendered PDF
        pages 2, 6 and 7 for attribution and comparison.
---

PDF p. 1: ` Abstract and paragraph after Theorem 1.1 `; PDF p. 6: ` Proposition 6.1, statement `; PDF p. 7: ` End of Proposition 6.1 `

## Prerequisites

- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [def-euler-four-square-representations](item-def-euler-four-square-representations)
- [def-euler-mixed-four-square-representations](item-def-euler-mixed-four-square-representations)
- [def-euler-prime-obstruction-count](item-def-euler-prime-obstruction-count)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [lem-euler-analytic-total-obstruction](item-lem-euler-analytic-total-obstruction)
- [lem-euler-sieve-sufficiency](item-lem-euler-sieve-sufficiency)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:thm-rat-ordered-field](https://alphabetamath.cc/item/thm-rat-ordered-field)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-of-q-embeds](https://alphabetamath.cc/item/lem-of-q-embeds)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product)
- [math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum)


## Statement

Work with the Axiom of Choice, which asserts that for every family of nonempty sets there is a function that selects one element from each member.

Let $m$ be a positive odd integer, so $m>0$ and $m=2k+1$ for some integer $k$. Put $n=2m$ and suppose $n\ge64^4$, where $64^4=64\cdot64\cdot64\cdot64$. An integer $d$ divides $z$ if $z=dq$ for some integer $q$. A prime is an integer $p>1$ whose only positive divisors are $1$ and $p$. A prime divisor of $m$ is a prime that divides $m$. For an integer $r$, a prime $p$ is congruent to $r$ modulo $4$ when $4$ divides $p-r$.

Let $\mathcal P_3$ be the primes congruent to $3$ modulo $4$, and suppose every prime divisor of $m$ belongs to $\mathcal P_3$. Let $\mathcal A$ be the set of positive integers whose prime divisors are all congruent to $1$ modulo $4$. Then $n\in\mathcal A+\mathcal A$, meaning that $n=a+b$ for some $a,b\in\mathcal A$.

## Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[def-euler-prime-classes](item-def-euler-prime-classes)

## Facts & Assumptions

[F1] Let $R(n)$ count the ordered quadruples $(x_1,x_2,x_3,x_4)$ of integers satisfying $x_1^2+x_2^2+x_3^2+x_4^2=n$, where $x_i^2=x_i\cdot x_i$. Entries may be negative, zero or positive, and two quadruples are equal exactly when all four corresponding entries agree. A quadruple is mixed if each of $(x_1,x_2)$ and $(x_3,x_4)$ has one even and one odd entry, where an even integer is twice an integer. For $p\in\mathcal P_3$, let $b_p(n)$ count the mixed quadruples in which $p$ divides both entries of at least one of the two pairs. Each qualifying quadruple counts once, including when both pairs qualify. The cardinality of a finite set is its number of elements, with value zero exactly when the set is empty. [def-euler-four-square-representations](item-def-euler-four-square-representations) [def-euler-mixed-four-square-representations](item-def-euler-mixed-four-square-representations) [def-euler-prime-obstruction-count](item-def-euler-prime-obstruction-count) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F2] With the Axiom of Choice and the stated hypotheses on $m,n$ and the prime divisors of $m$, the total obstruction estimate gives $R(n)>0$ and only finitely many $p\in\mathcal P_3$ with $b_p(n)\ne0$. Writing $S$ for the sum of these nonzero counts, the estimate in the real numbers is $S/R(n)\le 21235493/33177600<2/3$. [lem-euler-analytic-total-obstruction](item-lem-euler-analytic-total-obstruction) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F3] For $n=2m$ with $m$ positive and odd, the sieve criterion states that the rational inequality $S<\frac23 R(n)$ implies $n\in\mathcal A+\mathcal A$. Its sum is over the primes with at least one qualifying quadruple in F1, which are precisely the primes with $b_p(n)\ne0$. [lem-euler-sieve-sufficiency](item-lem-euler-sieve-sufficiency) [def-euler-prime-obstruction-count](item-def-euler-prime-obstruction-count) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [def-euler-prime-classes](item-def-euler-prime-classes)

[F4] In the real and rational fields, multiplication is associative and commutative with identity $1$, and division by a nonzero number is multiplication by its reciprocal, the number that multiplies it to give $1$. The orders are total, meaning that any two elements can be compared. In the real field multiplication by a positive number preserves strict inequality. [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field) [math:thm-rat-ordered-field](https://alphabetamath.cc/item/thm-rat-ordered-field) [math:def-field](https://alphabetamath.cc/item/def-field) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field) [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules)

[F5] The natural numbers are the counting numbers $0,1,2,\ldots$ and enter the integers as the nonnegative integers. The integers enter the rationals as fractions with denominator $1$. Denote the resulting map from natural numbers to rationals by $j$. Rationals are fractions of integers with nonzero denominators, with equality given by equality of cross products. The reals contain each rational as the class of its constant sequence, and the unique ordered-field inclusion $i$ sends a fraction with positive denominator to the real quotient of its numerator and denominator. Each of these maps preserves $0$, addition, multiplication and order. The map $i$ is one-to-one, meaning distinct rationals have distinct images. [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers) [math:lem-of-q-embeds](https://alphabetamath.cc/item/lem-of-q-embeds)

[F6] A finite set can be listed once per element in a natural number of positions. Its finite sum is the running sum at the full list length and is independent of the listing. Write $\sigma(k)$ for the successor of a natural number $k$. In the natural numbers and in the reals, the running sum at length zero is zero in the respective number system. The running sum at a successor length is the previous sum plus the next term. For the recursions on all natural lengths, extend the list by zeros beyond its listed positions. Induction proves a property for every natural length if it holds at zero and passes from each length to its successor. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product) [math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

## Proof

**Given:** The Axiom of Choice and $n=2m\ge64^4$ for a positive odd integer $m$ with every prime divisor in $\mathcal P_3$.

**Goal:** Prove $n\in\mathcal A+\mathcal A$.

1.1 The count definitions apply because $n\ge64^4>0$. The cutoff inequality also holds in the reals because the inclusions in F5 preserve arithmetic and order. Thus the given hypotheses allow F2 to be applied. Hence $R(n)>0$, the primes with nonzero counts form a finite set, and the real quotient $S/R(n)$ is strictly less than $2/3$. [given, F1, F2, F5]

2.1 Multiplication by the positive real value of $R(n)$ preserves this strict inequality. Since the reciprocal of $R(n)$ cancels $R(n)$ in the product on the left, the real comparison is $S<\frac23 R(n)$. [F4, step 1.1]

3.1 Regard $S$ as the natural-number sum on the finite set in Step 1.1. Choose a listing of natural length $L$ and write $a_k$ for its counts, extended by zeros beyond the listing. Let $N_k$ be the natural sum of the first $k$ terms and $T_k$ the real sum of their images under $i\circ j$. At length zero, $T_0=i(j(N_0))$ because both recursions start at zero and the maps preserve zero. If $T_k=i(j(N_k))$, the successor clauses and preservation of addition give $T_{\sigma(k)}=T_k+i(j(a_k))=i(j(N_k+a_k))=i(j(N_{\sigma(k)}))$. By induction this holds at length $L$. Then $N_L=S$ and $T_L$ is the real left-hand side in Step 2.1, so that side equals the image under $i$ of the rational left-hand side required by F3. [F3, F5, F6, step 1.1, step 2.1]

4.1 The real right-hand side is $i(\frac23 j(R(n)))$, since $i$ sends $2/3$ to the corresponding real quotient and preserves multiplication. The real inequality therefore reads $i(j(S))<i(\frac23 j(R(n)))$. If $j(S)\ge\frac23 j(R(n))$ in the rational order, preservation of order by $i$ would give the reverse weak inequality in the reals. Totality of the rational order now gives $j(S)<\frac23 j(R(n))$. [F4, F5, step 2.1, step 3.1]

5.1 Since $n=2m$ with $m$ positive and odd, the sieve criterion F3 applies to the rational inequality in Step 4.1. It yields $n\in\mathcal A+\mathcal A$, so $n$ is a sum of two positive integers all of whose prime divisors are congruent to $1$ modulo $4$. [given, F3, step 4.1] ∎

## Source notes

Proposition 6.1 combines the two estimates (6.1) and (6.2), then invokes (2.2) and (2.3). The total obstruction estimate and the sieve criterion supply those two parts of the argument here.

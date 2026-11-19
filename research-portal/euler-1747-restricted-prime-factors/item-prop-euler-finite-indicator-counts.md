---
title: Prime count and retained-index count for the indicator sieve
status: published
research_item: prop-euler-finite-indicator-counts
dependency_level: 5
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, progression below (7.3), and p. 8, first sentence after Table 1
---

PDF p. 7: ` §7, number of primes in the sieve after (7.3) `; PDF p. 8: ` Paragraph after Table 1, retained-index count `

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [alg-euler-finite-indicator-sieve](item-alg-euler-finite-indicator-sieve)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [lem-trial-division-primality-bound](item-lem-trial-division-primality-bound)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [lem-finite-deletions-and-translated-support](item-lem-finite-deletions-and-translated-support)
- [lem-euler-finite-indicator-sieve-equivalence](item-lem-euler-finite-indicator-sieve-equivalence)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)


## Statement

Let $\mathbb Z$ denote the set of integers.

Let $H=2^{22}-1=4{,}194{,}303$ and let $I_H$ be the set of integers from $0$ through $H$, including both endpoints. The power $2^{22}$ is the product of twenty-two copies of $2$. Let $S$ consist of the primes $p\le4096$ in $\mathcal P_3$, the class of primes of the form $3+4q$ for an integer $q$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. A positive integer $d$ divides $p$ when $p=dt$ for some integer $t$.

The indicator sieve starts with all $H+1$ indices in $I_H$. For each $p\in S$ in increasing order it removes every index of the form $b_p+rp$ in $I_H$, where $b_p$ is the integer satisfying $4b_p=3p-1$ and $r$ runs over the nonnegative integers. Let $C$ be the set of indices that remain. For a finite set $A$, its cardinality $|A|$ is the length of a list containing each member exactly once. The counts are
$$|S|=287,\qquad |C|=1{,}344{,}661.$$

## Statement references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)

[def-euler-prime-classes](item-def-euler-prime-classes)

[alg-euler-finite-indicator-sieve](item-alg-euler-finite-indicator-sieve)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

## Facts & Assumptions

[F1] The finite-range definition fixes $H$ and $I_H$ as in the statement. The prime-class definition makes membership of $S$ equivalent to being prime, being at most $4096$, and having the form $3+4q$ for some integer $q$. [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices) [def-euler-prime-classes](item-def-euler-prime-classes)

[F2] For integers $a$ and $b>0$, there is a unique integer quotient $q$ and remainder $r$ with $a=bq+r$ and $0\le r<b$. The remainder is zero exactly when $b$ divides $a$. In the computation, `a // b` and `a % b` denote this quotient and remainder. [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

[F3] For any integer $p>1$, trial division characterizes primality by the absence of a divisor $d$ with $d\ge2$ and $d^2\le p$. This is the square-root criterion in integer arithmetic, using the square-bound equivalence and finite test in phases 2 and 4 of the cited proof. [lem-trial-division-primality-bound](item-lem-trial-division-primality-bound)

[F4] Integer order is compatible with addition, products of positive integers are positive, and the distributive law applies. The natural numbers are identified with the nonnegative integers by a map preserving addition and order. Induction on the number of processed entries applies by proving an assertion for zero entries and proving that processing one more entry preserves it. [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F5] The indicator sieve starts at $I_H$ and deletes the specified progression for each prime in $S$. The finite-deletion lemma applies to a finite initial subset of the integers and any finite list of deletion sets that are subsets of the integers. It gives a unique finite current set at each step, with membership determined by excluding everything deleted so far. The sieve equivalence identifies membership in the final set with the value $1$ of the indicator $\varepsilon_j$ of the finite-range definition. [alg-euler-finite-indicator-sieve](item-alg-euler-finite-indicator-sieve) [lem-finite-deletions-and-translated-support](item-lem-finite-deletions-and-translated-support) [lem-euler-finite-indicator-sieve-equivalence](item-lem-euler-finite-indicator-sieve-equivalence) [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)

[F6] A list containing each member of a finite set exactly once has length equal to its cardinality. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F7] The integer variables in the statement and the computation take values in $\mathbb Z$. [math:def-integers](https://alphabetamath.cc/item/def-integers)

## Proof

**Given:** The sets $S$ and $I_H$ and the progression sieve that produces $C$.

**Goal:** Compute $|S|$ and $|C|$ by exact integer operations.

1.1 In the code below, `range(start, stop, step)` lists successive integers starting at `start` and adding the positive integer `step` as long as the entry is strictly below `stop`. The two-argument form uses step $1$. Thus the outer loop visits every integer $p$ from $2$ through $4096$ once. By uniqueness of the remainder in division by $4$, the condition `p % 4 == 3` holds exactly when $p=3+4q$ for an integer $q$. These are all the candidates needed for $S$. [given, F1, F2, F7]

2.1 For a candidate that passes the remainder check, the divisor loop starts at $d=2$ and increases $d$ by $1$ only while $d^2\le p$ and division by $d$ has nonzero remainder. It stops by $d=65$ because $65^2=4225>4096$. Once $d^2>p$, every larger candidate $e$ also has $e^2>p$, since $e^2-d^2=(e-d)(e+d)>0$ for $e>d\ge2$. Thus if the loop stops at $d^2>p$, all required trial divisions have nonzero remainder. If it stops at $d^2\le p$, the current remainder is zero and gives a divisor in the required range. By the trial division criterion, the code increments `prime_count` exactly for members of $S$. [F2, F3, F4, F7, step 1.1]

3.1 For each accepted $p=3+4q$, $3p-1=4(2+3q)$, so `(3 * p - 1) // 4` equals $b_p$ by uniqueness of the quotient. Since $p\ge2$, $4b_p=3p-1>0$ forces $b_p>0$. The inner range visits exactly the indices $b_p+rp\le H$ for integers $r\ge0$, with each index in $I_H$. Each visited entry is set to zero and all other entries keep their previous values. The code therefore deletes exactly the prescribed progression from the set of indices whose entries are $1$. [F2, F4, F5, F7, step 1.1, step 2.1]

4.1 The byte array `retained` is a list of entries with indices starting at zero. It starts with $H+1$ entries equal to $1$, one per member of $I_H$. After any number of outer iterations, its entries equal to $1$ mark exactly the current retained set, and `prime_count` is the number of members of $S$ already visited. At zero iterations the whole set is retained and the counter is zero. A skipped candidate changes neither the list nor the counter. An accepted candidate increments the counter once and changes precisely the specified entries to zero, including any that were already zero. Induction gives both assertions at the end of the loop. Every member of $S$ has then been visited once, so `prime_count` equals $|S|$, and the indices with entries equal to $1$ are exactly the elements of $C$. [F4, F5, F6, step 1.1, step 2.1, step 3.1]

5.1 The final loop starts `retained_count` at zero and scans the entries once in index order. For any number of entries already scanned, that counter equals the number of entries equal to $1$ among them. This holds initially, and adding the next entry increases the count by exactly one if its value is $1$ and leaves the count unchanged if its value is $0$. Induction gives the assertion for the full list, so the counter equals $|C|$. By the sieve equivalence this also counts the indices in $I_H$ with $\varepsilon_j=1$. [F4, F5, F6, step 4.1]

6.1 Executing the exact integer computation below produced `287 1344661`. The two output integers are $|S|$ and $|C|$, respectively, which gives the stated counts. [step 4.1, step 5.1] ∎

## Source notes

The progression is specified below (7.3) on p. 7. The reported retained-index count is the first sentence after Table 1 on p. 8.

The Python 3 replay below implements the progression deletions and counts with integer operations.

```python
H = 4194303
retained = bytearray([1]) * (H + 1)
prime_count = 0
for p in range(2, 4097):
    if p % 4 != 3:
        continue
    d = 2
    while d * d <= p and p % d != 0:
        d += 1
    if d * d > p:
        prime_count += 1
        for j in range((3 * p - 1) // 4, H + 1, p):
            retained[j] = 0
retained_count = 0
for flag in retained:
    retained_count += flag
print(prime_count, retained_count)
```

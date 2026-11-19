---
title: Arithmetic progression sieve for the finite indicators
status: published
research_item: alg-euler-finite-indicator-sieve
dependency_level: 3
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, progression below (7.3)
---

PDF p. 7: ` §7, progression below (7.3) `

## Prerequisites

- [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)
- [def-author-c74aeff6099d-bounded-integer-indices](item-def-author-c74aeff6099d-bounded-integer-indices)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-set-difference-and-symmetric-difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [lem-invertible-linear-residue-progression](item-lem-invertible-linear-residue-progression)
- [lem-finite-deletions-and-translated-support](item-lem-finite-deletions-and-translated-support)


## Definition

The sieve deletes specified indices from an initial set. Its inputs are fixed by the finite certificate. Take $H=2^{22}-1=4{,}194{,}303$, where $2^{22}$ is the product of twenty-two copies of $2$. Let $I_H$ consist of the integers $j$ with $0\le j\le H$, including both endpoints. Let $S$ consist of the primes $p\le4096$ in the class $\mathcal P_3$, meaning that $p=3+4q$ for some integer $q$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. An integer $d$ is a divisor of $p$ when $p=dt$ for some integer $t$.

Start with the current set $C=I_H$. Scan the integers from $1$ through $4096$ in increasing order. When $p$ is outside $S$, leave $C$ as it is. When $p\in S$, take $b_p=(3p-1)/4$, the integer satisfying $4b_p=3p-1$. Form the subset $E_p$ of $I_H$ consisting of the indices
$$j=b_p+rp,\qquad r\text{ an integer with }r\ge0,\qquad j\le H.$$
This arithmetic progression starts at $b_p$ and increases by $p$ at each successive value of $r$. Replace $C$ by the set difference $C\setminus E_p$, consisting of the elements of $C$ outside $E_p$.

Return the final set $C$, called the set of retained indices. The sieve assigns the value $1$ to each retained index and the value $0$ to each other index of $I_H$.

## Definition references

[def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)

[def-author-c74aeff6099d-bounded-integer-indices](item-def-author-c74aeff6099d-bounded-integer-indices)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-set-difference-and-symmetric-difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference)

## Justification

The [finite certificate definition](item-def-euler-finite-certificate-indices) supplies $H$, $I_H$, and $S$. The [bounded-index definition](item-def-author-c74aeff6099d-bounded-integer-indices) gives finiteness of $I_H$ because $H$ is a nonnegative integer. For $p\in S$, write $p=3+4q$ as in the definition. Then $3p-1=4(2+3q)$, so $b_p=2+3q$ is an integer. Multiplication by the positive integer $4$ preserves strict order, so no two different integers can satisfy $4b_p=3p-1$. Since $p>1$, the inequalities $0<3p-1<4p$ imply $0<b_p<p$ by the same order rule. [Integer arithmetic and order](https://alphabetamath.cc/item/thm-int-ordered-ring)

The first term is the least nonnegative index $j$ for which $4j+1$ is a multiple of $p$. Indeed, $4b_p+1=3p$. If $4=pu$ for some integer $u$, then $1=p(3-ub_p)$. That is impossible by [division with remainder](https://alphabetamath.cc/item/thm-division-algorithm-in-z), since $p>1$ and the division $1=0\cdot p+1$ has the nonzero remainder $1$. The [linear progression lemma](item-lem-invertible-linear-residue-progression) therefore applies to the expression $4j+1$ and the prime $p$. It identifies the nonnegative integers $j$ for which $4j+1$ is a multiple of $p$ as the progression starting at $b_p$ with step $p$.

Because $r\ge0$, $p\ge1$ and $b_p\ge0$, each term satisfies $0\le r\le b_p+rp$. Therefore $b_p+rp\le H$ forces $r\in I_H$. The [increasing enumeration of $I_H$](item-def-author-c74aeff6099d-bounded-integer-indices) gives a finite list of candidates for $r$. Testing $b_p+rp\le H$ on that list gives exactly the specified deletions. The condition on $j$ selects a unique subset $E_p$ inside $I_H$ by [separation within a set](https://alphabetamath.cc/item/def-subset-and-proper-subset).

The [bounded-index enumeration](item-def-author-c74aeff6099d-bounded-integer-indices) lists $I_{4095}$ as the integer images of the natural numbers $0$ through $4095$, in that order. Shifting each listed value by integer $1$ gives exactly the scan from $1$ through $4096$ in increasing order. The [natural-to-integer embedding](https://alphabetamath.cc/item/lem-nat-embeds-int) $\iota$ sends natural $1$ to integer $1$ and preserves addition, so the natural-number position $m$ with $1\le m\le4096$ corresponds to the scanned integer $p=\iota(m)$.

At scan position $m$, use the subset $E_p$ if $p\in S$, and the empty subset of $I_H$ otherwise. Taking a [set difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference) with the empty set keeps all current indices. These choices specify one subset of the integers per natural-number position. The [finite deletion rule](item-lem-finite-deletions-and-translated-support) therefore applies with initial set $D=I_H$ and $4096$ deletion sets. It gives a unique finite retained set at each scan position. For each $j\in I_H$, membership in the final set determines exactly one of the two assigned values.

## Remarks

The relationship between the values assigned by this sieve and the binary indicators $\varepsilon_j$ defined by the floor formula is the subject of [lem-euler-finite-indicator-sieve-equivalence](item-lem-euler-finite-indicator-sieve-equivalence).

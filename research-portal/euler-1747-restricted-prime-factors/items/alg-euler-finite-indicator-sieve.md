---
id: alg-euler-finite-indicator-sieve
kind: algorithm
title: Arithmetic progression sieve for the finite indicators
status: draft
domain: mathematics
deps:
  - def-euler-finite-certificate-indices
  - def-author-c74aeff6099d-bounded-integer-indices
  - math:lem-nat-embeds-int
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-subset-and-proper-subset
  - math:def-set-difference-and-symmetric-difference
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - lem-invertible-linear-residue-progression
  - lem-finite-deletions-and-translated-support
formulation_deps:
  - def-euler-finite-certificate-indices
  - def-author-c74aeff6099d-bounded-integer-indices
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-subset-and-proper-subset
  - math:def-set-difference-and-symmetric-difference
argument_deps:
  - def-euler-finite-certificate-indices
  - def-author-c74aeff6099d-bounded-integer-indices
  - math:lem-nat-embeds-int
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - lem-invertible-linear-residue-progression
  - math:def-subset-and-proper-subset
  - math:def-set-difference-and-symmetric-difference
  - lem-finite-deletions-and-translated-support
dependency_roles:
  def-euler-finite-certificate-indices: mathematical-premise
  def-author-c74aeff6099d-bounded-integer-indices: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-set-difference-and-symmetric-difference: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  lem-invertible-linear-residue-progression: mathematical-premise
  lem-finite-deletions-and-translated-support: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, progression below (7.3)
dependency_level: 3
---

## Definition

The sieve deletes specified indices from an initial set. Its inputs are fixed by the finite certificate. Take $H=2^{22}-1=4{,}194{,}303$, where $2^{22}$ is the product of twenty-two copies of $2$. Let $I_H$ consist of the integers $j$ with $0\le j\le H$, including both endpoints. Let $S$ consist of the primes $p\le4096$ in the class $\mathcal P_3$, meaning that $p=3+4q$ for some integer $q$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. An integer $d$ is a divisor of $p$ when $p=dt$ for some integer $t$.

Start with the current set $C=I_H$. Scan the integers from $1$ through $4096$ in increasing order. When $p$ is outside $S$, leave $C$ as it is. When $p\in S$, take $b_p=(3p-1)/4$, the integer satisfying $4b_p=3p-1$. Form the subset $E_p$ of $I_H$ consisting of the indices
$$j=b_p+rp,\qquad r\text{ an integer with }r\ge0,\qquad j\le H.$$
This arithmetic progression starts at $b_p$ and increases by $p$ at each successive value of $r$. Replace $C$ by the set difference $C\setminus E_p$, consisting of the elements of $C$ outside $E_p$.

Return the final set $C$, called the set of retained indices. The sieve assigns the value $1$ to each retained index and the value $0$ to each other index of $I_H$.

## Definition references

[[def-euler-finite-certificate-indices]]

[[def-author-c74aeff6099d-bounded-integer-indices]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-subset-and-proper-subset]]

[[math:def-set-difference-and-symmetric-difference]]

## Justification

The [[def-euler-finite-certificate-indices|finite certificate definition]] supplies $H$, $I_H$, and $S$. The [[def-author-c74aeff6099d-bounded-integer-indices|bounded-index definition]] gives finiteness of $I_H$ because $H$ is a nonnegative integer. For $p\in S$, write $p=3+4q$ as in the definition. Then $3p-1=4(2+3q)$, so $b_p=2+3q$ is an integer. Multiplication by the positive integer $4$ preserves strict order, so no two different integers can satisfy $4b_p=3p-1$. Since $p>1$, the inequalities $0<3p-1<4p$ imply $0<b_p<p$ by the same order rule. [[math:thm-int-ordered-ring|Integer arithmetic and order]]

The first term is the least nonnegative index $j$ for which $4j+1$ is a multiple of $p$. Indeed, $4b_p+1=3p$. If $4=pu$ for some integer $u$, then $1=p(3-ub_p)$. That is impossible by [[math:thm-division-algorithm-in-z|division with remainder]], since $p>1$ and the division $1=0\cdot p+1$ has the nonzero remainder $1$. The [[lem-invertible-linear-residue-progression|linear progression lemma]] therefore applies to the expression $4j+1$ and the prime $p$. It identifies the nonnegative integers $j$ for which $4j+1$ is a multiple of $p$ as the progression starting at $b_p$ with step $p$.

Because $r\ge0$, $p\ge1$ and $b_p\ge0$, each term satisfies $0\le r\le b_p+rp$. Therefore $b_p+rp\le H$ forces $r\in I_H$. The [[def-author-c74aeff6099d-bounded-integer-indices|increasing enumeration of $I_H$]] gives a finite list of candidates for $r$. Testing $b_p+rp\le H$ on that list gives exactly the specified deletions. The condition on $j$ selects a unique subset $E_p$ inside $I_H$ by [[math:def-subset-and-proper-subset|separation within a set]].

The [[def-author-c74aeff6099d-bounded-integer-indices|bounded-index enumeration]] lists $I_{4095}$ as the integer images of the natural numbers $0$ through $4095$, in that order. Shifting each listed value by integer $1$ gives exactly the scan from $1$ through $4096$ in increasing order. The [[math:lem-nat-embeds-int|natural-to-integer embedding]] $\iota$ sends natural $1$ to integer $1$ and preserves addition, so the natural-number position $m$ with $1\le m\le4096$ corresponds to the scanned integer $p=\iota(m)$.

At scan position $m$, use the subset $E_p$ if $p\in S$, and the empty subset of $I_H$ otherwise. Taking a [[math:def-set-difference-and-symmetric-difference|set difference]] with the empty set keeps all current indices. These choices specify one subset of the integers per natural-number position. The [[lem-finite-deletions-and-translated-support|finite deletion rule]] therefore applies with initial set $D=I_H$ and $4096$ deletion sets. It gives a unique finite retained set at each scan position. For each $j\in I_H$, membership in the final set determines exactly one of the two assigned values.

## Remarks

The relationship between the values assigned by this sieve and the binary indicators $\varepsilon_j$ defined by the floor formula is the subject of [[lem-euler-finite-indicator-sieve-equivalence]].

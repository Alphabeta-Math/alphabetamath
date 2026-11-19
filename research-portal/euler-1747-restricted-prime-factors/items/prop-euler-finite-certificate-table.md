---
id: prop-euler-finite-certificate-table
kind: proposition
title: "Table 1: Values of the finite recurrence"
status: published
domain: mathematics
deps:
  - def-author-c74aeff6099d-bounded-integer-indices
  - def-euler-finite-certificate-indices
  - alg-euler-finite-indicator-sieve
  - lem-euler-finite-indicator-sieve-equivalence
  - def-euler-finite-first-summand-indices
  - alg-euler-finite-unrepresented-recurrence
  - def-euler-finite-unrepresented-count
  - lem-euler-finite-unrepresented-recurrence-equivalence
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-set-difference-and-symmetric-difference
  - math:def-sum-over-a-finite-index-set
  - math:def-natural-numbers
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - math:thm-induction-principle
  - math:def-finite-cardinality
  - math:lem-nat-embeds-int
  - math:lem-nat-nonzero-is-successor
  - math:def-nat-addition
  - math:def-nat-order
  - math:lem-nat-order-is-membership
  - math:def-function
  - math:def-injection-surjection-bijection
formulation_deps:
  - def-author-c74aeff6099d-bounded-integer-indices
  - def-euler-finite-certificate-indices
  - alg-euler-finite-indicator-sieve
  - lem-euler-finite-indicator-sieve-equivalence
  - def-euler-finite-first-summand-indices
  - alg-euler-finite-unrepresented-recurrence
  - def-euler-finite-unrepresented-count
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-set-difference-and-symmetric-difference
  - math:def-sum-over-a-finite-index-set
argument_deps:
  - def-author-c74aeff6099d-bounded-integer-indices
  - def-euler-finite-certificate-indices
  - alg-euler-finite-indicator-sieve
  - lem-euler-finite-indicator-sieve-equivalence
  - def-euler-finite-first-summand-indices
  - alg-euler-finite-unrepresented-recurrence
  - def-euler-finite-unrepresented-count
  - lem-euler-finite-unrepresented-recurrence-equivalence
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-set-difference-and-symmetric-difference
  - math:def-natural-numbers
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - math:thm-induction-principle
  - math:def-finite-cardinality
  - math:lem-nat-embeds-int
  - math:lem-nat-nonzero-is-successor
  - math:def-nat-addition
  - math:def-nat-order
  - math:lem-nat-order-is-membership
  - math:def-function
  - math:def-injection-surjection-bijection
dependency_roles:
  def-author-c74aeff6099d-bounded-integer-indices: mathematical-premise
  def-euler-finite-certificate-indices: mathematical-premise
  alg-euler-finite-indicator-sieve: mathematical-premise
  lem-euler-finite-indicator-sieve-equivalence: mathematical-premise
  def-euler-finite-first-summand-indices: mathematical-premise
  alg-euler-finite-unrepresented-recurrence: mathematical-premise
  def-euler-finite-unrepresented-count: mathematical-premise
  lem-euler-finite-unrepresented-recurrence-equivalence: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-set-difference-and-symmetric-difference: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:thm-induction-principle: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-nat-nonzero-is-successor: mathematical-premise
  math:def-nat-addition: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:def-function: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, equations (7.1)–(7.3); p. 8, Table 1 and the
        terminal-empty-set sentence immediately after it
dependency_level: 7
---

## Statement

Let $H=4{,}194{,}303$. For a nonnegative integer $B$, write $I_B$ for the integers from $0$ through $B$, including both endpoints. Let $S$ consist of the primes $p\le4096$ of the form $4q+3$ for an integer $q$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. A positive divisor of an integer $v$ is an integer $d>0$ with $v=dt$ for some integer $t$.

The binary certificate indicator $\varepsilon_j$ is $1$ at precisely the indices in $I_H$ that survive the following sieve, or procedure of successive deletions. Start with $I_H$. For each $p\in S$, remove every index of the form $(3p-1)/4+rp$ for a nonnegative integer $r$. The indicator is $0$ at every other index in $I_H$ and at every negative integer.

Let $J=\{i\in I_{78}:\varepsilon_i=1\}$. For an integer cutoff $a=4m+1$ with $1\le a\le313$ and $m$ an integer, let $C(a)$ be the set obtained from $I_H$ by taking each $i\in J$ with $i\le m$ in increasing order and deleting the current elements $k$ with $k\ge i$ and $\varepsilon_{k-i}=1$. Deletion keeps exactly the current elements outside the specified set. The first summand at index $i$ is $4i+1$, so the condition $i\le m$ imposes the upper bound $a$ on that summand. Define
$$U(a)=\sum_{k=0}^{H}\prod_{i=0}^{m}(1-\varepsilon_i\varepsilon_{k-i}).$$
The sum adds one term per index, and the product multiplies one factor per index, with both endpoints included.

| Upper bound $a$ | $U(a)$ |
| --- | ---: |
| $1$ | $2{,}849{,}643$ |
| $13$ | $1{,}261{,}334$ |
| $29$ | $364{,}708$ |
| $61$ | $71{,}867$ |
| $101$ | $6{,}561$ |
| $149$ | $756$ |
| $193$ | $57$ |
| $205$ | $23$ |
| $229$ | $8$ |
| $277$ | $2$ |
| $289$ | $1$ |
| $313$ | $0$ |

At $a=313$ the recurrence ends with the empty set $C(313)=\varnothing$.

## Statement references

[[def-author-c74aeff6099d-bounded-integer-indices]]

[[def-euler-finite-certificate-indices]]

[[alg-euler-finite-indicator-sieve]]

[[lem-euler-finite-indicator-sieve-equivalence]]

[[def-euler-finite-first-summand-indices]]

[[alg-euler-finite-unrepresented-recurrence]]

[[def-euler-finite-unrepresented-count]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-prime]]

[[math:def-divides-in-z]]

[[math:def-set-difference-and-symmetric-difference]]

[[math:def-sum-over-a-finite-index-set]]

## Facts & Assumptions

[F1] Integer addition, subtraction and multiplication obey the commutative ring laws, and the integer order is total and is preserved under addition and under multiplication by a positive integer. For an integer $v$ and an integer $d>0$, division gives unique integers $t,r$ with $v=dt+r$ and $0\le r<d$. The remainder is zero exactly when $d$ divides $v$. A prime $p>1$ has no positive divisor strictly between $1$ and $p$. [[math:def-integers]] [[math:def-int-order]] [[math:def-int-operations]] [[math:thm-int-ordered-ring]] [[math:thm-division-algorithm-in-z]] [[math:def-divides-in-z]] [[math:def-prime]]

[F2] The bounded set $I_H$ contains exactly the integers from $0$ through $H$. The progression sieve starts with $I_H$ and deletes the indices $(3p-1)/4+rp\le H$ for $p\in S$ and integers $r\ge0$. The sieve equivalence identifies its retained indices with those where the certificate indicator is $1$. At each negative integer the indicator is $0$ by definition. [[def-author-c74aeff6099d-bounded-integer-indices]] [[alg-euler-finite-indicator-sieve]] [[lem-euler-finite-indicator-sieve-equivalence]] [[def-euler-finite-certificate-indices]]

[F3] For $a=4m+1$ in the stated range, the cutoff algorithm starts with $I_H$ and scans $i=0,\ldots,m$. At $i\in J$ it takes the set difference with the indices $k\in I_H$ satisfying $k\ge i$ and $\varepsilon_{k-i}=1$. At other indices it leaves the set unchanged. The definition of $J$ selects exactly the $i\in I_{78}$ for which $\varepsilon_i=1$. [[alg-euler-finite-unrepresented-recurrence]] [[math:def-set-difference-and-symmetric-difference]] [[def-euler-finite-first-summand-indices]]

[F4] Natural-number induction starts at $0$ and advances from $n$ to its successor $n+1$. Every nonzero natural number is a successor. The canonical embedding $\iota$ takes the natural numbers bijectively onto the nonnegative integers, preserves addition, and sends $0$ and $1$ to the corresponding integers. It preserves and reflects order: $r\le s$ if and only if $\iota(r)\le\iota(s)$. In the natural-number order, $r\le s$ means $r+t=s$ for some natural $t$, and $r<s$ means $r\le s$ and $r\ne s$. For the von Neumann naturals, $0=\varnothing$, $b+1=b\cup\{b\}$, and $r\in b+1$ holds exactly when $r<b+1$, equivalently $r\le b$. [[math:def-natural-numbers]] [[math:thm-induction-principle]] [[math:lem-nat-nonzero-is-successor]] [[math:def-nat-addition]] [[math:lem-nat-embeds-int]] [[math:def-int-operations]] [[math:def-nat-order]] [[math:lem-nat-order-is-membership]]

[F5] For every integer $a=4m+1$ in the stated bounds, the recurrence equivalence for the certificate indicators gives $|C(a)|=U(a)$, with $U(a)$ the sum of products in the Statement. A list of natural-number length $\ell$ with entries in $I_H$ is a function from the von Neumann natural $\ell$ to $I_H$. This gives exactly one entry in $I_H$ at each position $r<\ell$, and the domain is empty when $\ell=0$. A function is a bijection onto its codomain if equal values force equal inputs and every element of the codomain occurs as a value. If a list gives such a bijection onto $D$, then $|D|=\ell$. A finite set has cardinality zero exactly when it is empty. [[lem-euler-finite-unrepresented-recurrence-equivalence]] [[def-euler-finite-unrepresented-count]] [[def-author-c74aeff6099d-bounded-integer-indices]] [[math:def-finite-cardinality]] [[math:def-function]] [[math:def-injection-surjection-bijection]]

## Proof

**Given:** The fixed $H$, $S$, $J$, certificate indicators, and cutoff rule in the Statement.

**Goal:** Evaluate $U(a)$ at the twelve displayed cutoffs and determine $C(313)$.

1.1 The cutoff bounds give $0\le4m\le312=4\cdot78$, so $0\le m\le78$. For $k\in I_H$ and $i\in I_m$, we have $i\in I_H$ and $k-i\le H$. Hence $k-i$ is either in $I_H$ or negative, so both indicators in each factor of $U(a)$ are defined. [given, F1, F2]

1.2 Every positive integer is at least $1$. Indeed, it is $\iota(n)$ for a nonzero natural $n=s+1$, so it is $\iota(s)+1$ with $\iota(s)\ge0$. In particular, $x<y$ for integers implies $x+1\le y$ by applying this fact to $y-x$. For a nonnegative integer $B$, let $b$ be its unique natural preimage under $\iota$. The positions of $b+1$ are precisely the naturals $r\le b$. Order preservation gives $0\le\iota(r)\le B$ at each of these positions. Conversely, each $x\in I_B$ has a unique natural preimage $r$, and $x\le B$ gives $r\le b$ by order reflection. Thus $r\mapsto\iota(r)$ on $b+1$ is a bijection onto $I_B$. It is strictly increasing since $\iota$ preserves order and is injective. [F1, F2, F4, F5]

2.1 Scan $q\in I_{1023}$ in increasing order and set $p=4q+3$. These are precisely the integers of that form with $1<p\le4096$, since $q<0$ gives $q\le-1$ and $p\le-1$, while $q>1023$ gives $q\ge1024$ and $p\ge4099$. For each candidate compute the integer remainder of $p$ upon division by each $d=2,\ldots,p-1$. Retain $p$ if all these remainders are nonzero, including when there are no such $d$. If $p=dt$ with $d>0$, then $t>0$ since $p>0$, and $t\ge1$ gives $d\le p$. Thus the tests exclude exactly the candidates with a positive divisor other than $1$ or $p$. The retained candidates are precisely $S$. [given, F1, step 1.2]

3.1 Start with a value $e_j=1$ at every $j\in I_H$. For each retained $p=4q+3$, take $b=3q+2$, so $4b=3p-1$ and $0\le b\le3071<H$. Let $v,s$ be the quotient and remainder in $H-b=vp+s$ with $0\le s<p$. If $v<0$, then $v\le-1$ would imply $vp+s<0$, contrary to $H-b\ge0$. Set $e_{b+rp}=0$ for each $r\in I_v$, leaving every other entry unchanged at each assignment. For $0\le r\le v$ the index lies in $I_H$, since $b+rp\le b+vp\le H$. For $r>v$, discreteness gives $r\ge v+1$ and then $b+rp\ge b+(v+1)p>H$. The assignments therefore visit exactly the progression indices of the sieve. A value stays $1$ exactly when its index is never visited, so $e_j=\varepsilon_j$ for every $j\in I_H$. [F1, F2, step 1.2, step 2.1]

4.1 Let $h$ be the natural number with $\iota(h)=H$. Let $L_0$ be the increasing list of $I_H$ given by $r\mapsto\iota(r)$ on $h+1$. For a natural position $n\in79$, put $i=\iota(n)$, which lies in $I_{78}$ by step 1.2. If $e_i=0$, let $L_{n+1}=L_n$. If $e_i=1$, scan the positions of $L_n$ in order, starting $L_{n+1}$ empty. Append an entry $k$ if $k<i$. If $k\ge i$, append it exactly when $e_{k-i}=0$. Here $0\le k-i\le H$, so this test uses a defined entry. To append $k$ to a list of length $\ell$, keep its function values on $\ell$ and assign $k$ at the new position $\ell$. Since $\ell+1=\ell\cup\{\ell\}$ and $\ell\notin\ell$, the extended function has exactly one entry at each position of $\ell+1$. Thus each retained entry occurs in $L_{n+1}$ as often as it did in $L_n$. [F1, F2, F4, F5, step 1.2, step 3.1]

5.1 After zero scan positions the list contains each element of $I_H$ once. Suppose that after $n<79$ positions, $L_n$ contains each surviving element exactly once and no other elements. At position $i=\iota(n)$ the case $e_i=0$ is exactly $i\notin J$, so the survivors stay the same. Otherwise the list construction drops exactly the entries with $k\ge i$ and $\varepsilon_{k-i}=1$, as required by the cutoff update. In either case $L_{n+1}$ lists the new survivors once each. For a cutoff $a=4m+1$, write $m=\iota(b)$. By step 1.2, the first $b+1$ scan positions process exactly $I_m$ in increasing order. The induction through $79$ therefore gives that $L_{b+1}$ lists exactly $C(a)$ without repetition. [F3, F4, step 1.1, step 1.2, step 3.1, step 4.1]

6.1 At each tabulated $a$ there is a unique $m\in I_{78}$ with $a=4m+1$. Take the unique natural $b$ with $m=\iota(b)$ and record the length of $L_{b+1}$, whose entries lie in $C(a)$ by step 5.1. Its position-to-entry function is injective because there are no repeated entries and surjective onto $C(a)$ because every survivor occurs. The length is therefore $|C(a)|=U(a)$. [F1, F4, F5, step 5.1]

7.1 The remainder tests, progression assignments and guarded scans yield the lengths $2{,}849{,}643$, $1{,}261{,}334$, $364{,}708$, $71{,}867$, $6{,}561$, $756$, $57$, $23$, $8$, $2$, $1$ and $0$ in increasing cutoff order. The last length gives $U(313)=0$, so $C(313)=\varnothing$. [F5, step 2.1, step 3.1, step 4.1, step 6.1] ∎

## Remarks

### Computational transcript

This Python 3 program reproduces the arithmetic calculation and takes no input. Each printed line contains the cutoff and the number of elements that remain after the deletion at that cutoff, if there is a deletion, or after the unchanged scan position otherwise.

```python
H = 4194303
cutoffs = (1, 13, 29, 61, 101, 149, 193, 205, 229, 277, 289, 313)

eps = bytearray([1]) * (H + 1)
for q in range(1024):
    p = 4 * q + 3
    if any(p % d == 0 for d in range(2, p)):
        continue
    b = 3 * q + 2
    v = (H - b) // p
    for r in range(v + 1):
        eps[b + r * p] = 0

remaining = list(range(H + 1))
for i in range(79):
    if eps[i] == 1:
        remaining = [k for k in remaining if k < i or eps[k - i] == 0]
    a = 4 * i + 1
    if a in cutoffs:
        print(a, len(remaining))
```

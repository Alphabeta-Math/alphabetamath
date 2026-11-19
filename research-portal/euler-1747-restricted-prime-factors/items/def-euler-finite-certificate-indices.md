---
id: def-euler-finite-certificate-indices
kind: definition
title: Finite-range indices and binary indicators
status: published
domain: mathematics
deps:
  - math:def-natural-numbers
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-nat-power
  - def-author-c74aeff6099d-bounded-integer-indices
  - math:def-subset-and-proper-subset
  - def-euler-prime-classes
  - math:def-real-numbers
  - math:def-real-order
  - math:def-field
  - math:lem-integer-part
  - math:def-sum-over-a-finite-index-set
  - math:thm-int-ordered-ring
  - math:thm-subset-of-a-finite-set
  - math:lem-nat-embeds-int
  - math:thm-reals-ordered-field
  - lem-floor-increment-divisibility
  - lem-binary-products-and-avoidance
formulation_deps:
  - math:def-natural-numbers
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:lem-nat-embeds-int
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-nat-power
  - def-author-c74aeff6099d-bounded-integer-indices
  - math:def-subset-and-proper-subset
  - def-euler-prime-classes
  - math:def-real-numbers
  - math:def-real-order
  - math:def-field
  - math:lem-integer-part
  - math:def-sum-over-a-finite-index-set
argument_deps:
  - math:def-natural-numbers
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:thm-int-ordered-ring
  - math:def-nat-power
  - def-author-c74aeff6099d-bounded-integer-indices
  - math:def-subset-and-proper-subset
  - def-euler-prime-classes
  - math:thm-subset-of-a-finite-set
  - math:lem-nat-embeds-int
  - math:thm-reals-ordered-field
  - math:def-field
  - math:lem-integer-part
  - lem-floor-increment-divisibility
  - math:def-sum-over-a-finite-index-set
  - lem-binary-products-and-avoidance
dependency_roles:
  math:def-natural-numbers: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-nat-power: mathematical-premise
  def-author-c74aeff6099d-bounded-integer-indices: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:def-real-order: mathematical-premise
  math:def-field: mathematical-premise
  math:lem-integer-part: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  lem-floor-increment-divisibility: mathematical-premise
  lem-binary-products-and-avoidance: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, definition of H and (7.1), and p. 8, Proposition 7.2, first
        sentence of proof
dependency_level: 2
---

## Definition

Take $H=2^{22}-1=4{,}194{,}303$. Compute $2^{22}$ by multiplying twenty-two copies of $2$ in the natural numbers and use its integer image under the canonical embedding to form $H$. For a nonnegative integer $B$, write $I_B$ for the integers from $0$ through $B$, including both endpoints. The finite-range input at index $k$ is $n=4k+2$ for $k\in I_H$.

Let $S=\{p\in I_{4096}:p\in\mathcal P_3\}$, where $\mathcal P_3$ consists of the primes congruent to $3$ modulo $4$. A divisor of an integer $p$ is an integer $d$ for which $p=dq$ for some integer $q$. A prime is an integer greater than $1$ with only $1$ and itself as positive divisors. Congruence to $3$ modulo $4$ means $p-3=4q$ for some integer $q$.

For real quotients and floor comparisons, send each integer to its canonical rational image and then to the real class of the constant sequence with that rational value. With this identification, $a/p$ is the real number $u$ satisfying $pu=a$ for $p\ne0$. For a real number $x$, its floor $\lfloor x\rfloor$ is the unique integer $m$ with $m\le x<m+1$. For each integer $j$ with $0\le j\le H$, define the binary indicator $\varepsilon_j$ by
$$\varepsilon_j=\prod_{p\in S}\left(1-\left\lfloor\frac{4j+1}{p}\right\rfloor+\left\lfloor\frac{4j}{p}\right\rfloor\right).$$
The product is taken in the natural numbers, with one factor for each $p\in S$. Identify each displayed integer factor $0$ or $1$ with its natural preimage under the canonical embedding into the integers. Take any list of the members of $S$ with each member occurring exactly once. A product with no factors has value $1$. For every integer $j<0$, set $\varepsilon_j=0$. Here binary means that each value is either $0$ or $1$.

## Definition references

[[math:def-natural-numbers]]

[[math:lem-nat-embeds-int]]

[[math:lem-int-embeds-rat]]

[[math:lem-rat-embeds-dense]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-nat-power]]

[[def-author-c74aeff6099d-bounded-integer-indices]]

[[math:def-subset-and-proper-subset]]

[[def-euler-prime-classes]]

[[math:def-real-numbers]]

[[math:def-real-order]]

[[math:def-field]]

[[math:lem-integer-part]]

[[math:def-sum-over-a-finite-index-set]]

## Justification

The embedding of the natural numbers into the integers preserves multiplication, so the repeated product defining $2^{22}$ can be evaluated in integer arithmetic. Successive multiplication gives $2^5=32$. Grouping the twenty-two factors as four groups of five and a remaining pair gives $2^{22}=4\cdot32\cdot32\cdot32\cdot32=4{,}194{,}304$. Subtraction gives the stated nonnegative integer $H$, so the bounded index set $I_H$ is defined and finite ([[math:def-natural-numbers|Natural numbers]], [[math:def-nat-power|Powers of natural numbers]], [[math:lem-nat-embeds-int|Natural numbers in the integers]], [[math:thm-int-ordered-ring|Integer arithmetic and order]], [[def-author-c74aeff6099d-bounded-integer-indices|Bounded integer index sets]]). Integer addition and multiplication assign a single integer $4k+2$ to each index.

The membership condition for $S$ defines a unique subset of the finite set $I_{4096}$, so $S$ is finite ([[math:def-subset-and-proper-subset|Subset by a membership condition]], [[def-author-c74aeff6099d-bounded-integer-indices|Bounded integer index sets]], [[math:thm-subset-of-a-finite-set|Finiteness of a subset]]). Primes are positive, so $S$ includes exactly the primes in $\mathcal P_3$ that satisfy $p\le4096$. Every $p\in S$ is positive. The composite embedding sends integer $0$ to real $0$ and preserves order, so the real image of $p$ is positive. See [[math:lem-int-embeds-rat|The integers in the rationals]] and [[math:lem-rat-embeds-dense|The rationals in the reals]]. Both quotients therefore exist in the real field and both floors are determined uniquely in this same copy of the integers ([[def-euler-prime-classes|Prime classes]], [[math:thm-reals-ordered-field|The real ordered field]], [[math:def-field|Division in a field]], [[math:lem-integer-part|Floor existence and uniqueness]]).

For each $j\in I_H$, put $b=4j+1$, so that $b-1=4j$. The difference of the two floors in the displayed factor, in the order $\lfloor b/p\rfloor-\lfloor(b-1)/p\rfloor$, is either $0$ or $1$ by the floor-difference lemma for integer $b$ and positive integer $p$ ([[lem-floor-increment-divisibility|Floor difference for a positive denominator]]). If that difference is $d$, the factor equals $1-d$ by integer arithmetic. For $d=0$ this equals $1$, and for $d=1$ it equals $0$. Under the canonical natural-to-integer embedding, the natural $0$ and $1$ map to the corresponding integer values. In each case the two corresponding naturals for $d$ and $1-d$ add to $1$, by preservation of addition and injectivity. This is the natural-number complement used by the binary product rule ([[math:def-natural-numbers|Natural numbers]], [[math:lem-nat-embeds-int|Natural numbers in the integers]]). Thus the product over the finite set $S$ is a uniquely defined product of natural numbers, and the binary product rule makes its value $0$ or $1$ ([[math:def-sum-over-a-finite-index-set|Finite-set product]], [[lem-binary-products-and-avoidance|Binary product rule]]). The cases $j<0$ and $0\le j\le H$ are disjoint and cover every integer $j\le H$, so the prescribed zero values complete the definition on its intended domain.

---
id: alg-euler-finite-unrepresented-recurrence
kind: algorithm
title: Finite-set recurrence for the uncovered indices
status: draft
domain: mathematics
deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - def-euler-finite-certificate-indices
  - def-author-c74aeff6099d-bounded-integer-indices
  - def-euler-finite-first-summand-indices
  - math:def-set-difference-and-symmetric-difference
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:thm-division-algorithm-in-z
  - math:thm-int-ordered-ring
  - math:def-natural-numbers
  - math:def-nat-addition
  - math:def-nat-order
  - math:lem-nat-discrete
  - math:lem-nat-embeds-int
  - math:def-axiom-schema-of-separation
  - math:def-axiom-of-extensionality
  - math:def-power-set
  - math:def-cartesian-product
  - math:def-indexed-family
  - math:def-function
  - math:def-injection-surjection-bijection
  - lem-finite-deletions-and-translated-support
formulation_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - def-euler-finite-certificate-indices
  - def-author-c74aeff6099d-bounded-integer-indices
  - def-euler-finite-first-summand-indices
  - math:def-set-difference-and-symmetric-difference
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
argument_deps:
  - math:def-subset-and-proper-subset
  - math:thm-division-algorithm-in-z
  - math:def-int-operations
  - math:thm-int-ordered-ring
  - math:def-natural-numbers
  - math:def-nat-addition
  - math:def-nat-order
  - math:lem-nat-discrete
  - math:lem-nat-embeds-int
  - def-author-c74aeff6099d-bounded-integer-indices
  - def-euler-finite-certificate-indices
  - def-euler-finite-first-summand-indices
  - math:def-axiom-schema-of-separation
  - math:def-axiom-of-extensionality
  - math:def-power-set
  - math:def-cartesian-product
  - math:def-indexed-family
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:def-set-difference-and-symmetric-difference
  - lem-finite-deletions-and-translated-support
dependency_roles:
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  def-euler-finite-certificate-indices: mathematical-premise
  def-author-c74aeff6099d-bounded-integer-indices: mathematical-premise
  def-euler-finite-first-summand-indices: mathematical-premise
  math:def-set-difference-and-symmetric-difference: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-nat-addition: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-axiom-schema-of-separation: mathematical-premise
  math:def-axiom-of-extensionality: mathematical-premise
  math:def-power-set: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-indexed-family: mathematical-premise
  math:def-function: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  lem-finite-deletions-and-translated-support: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, initialization and update in equation (7.3)
dependency_level: 4
---

## Definition

The input is an integer $a$ with $1\le a\le313$ and $a\equiv1\pmod4$, meaning $a-1=4m$ for some integer $m$. Write $m=(a-1)/4$ for this integer quotient. Here $x-y=x+(-y)$.

Use $H=4{,}194{,}303$ and the finite-range indicators $\varepsilon_j$, with one specified value $0$ or $1$ at each integer $0\le j\le H$ and value $0$ when $j<0$. For a nonnegative integer $B$, let $I_B$ be the finite set of integers from $0$ through $B$, including both endpoints. Use the eligible first indices $J=\{i\in I_{78}:\varepsilon_i=1\}$, with possible first summand $4i+1$ at index $i$.

1. Start with $C=C_0=I_H=\{0,1,\ldots,H\}$.
2. Scan the integers $i=0,\ldots,m$ in increasing order. At an index $i\in J$, replace $C$ by $C\setminus\{k\in I_H:i\le k,\ \varepsilon_{k-i}=1\}$. The set difference $C\setminus E$ keeps exactly the elements of $C$ outside $E$. At an index outside $J$, leave $C$ as it is.
3. Return the resulting finite subset $C(a)$ of $I_H$. In other words, all its elements belong to $I_H$ and they can be listed once each in a list of natural-number length.

## Definition references

[[math:def-integers|Integers]]

[[math:def-int-order|Integer order]]

[[math:def-int-operations|Integer arithmetic]]

[[math:def-congruence-modulo-an-integer|Congruence modulo an integer]]

[[def-euler-finite-certificate-indices|Finite-range indicators]]

[[def-author-c74aeff6099d-bounded-integer-indices|Bounded integer index sets]]

[[def-euler-finite-first-summand-indices|Eligible first-summand indices]]

[[math:def-set-difference-and-symmetric-difference|Set difference]]

[[math:def-subset-and-proper-subset|Subsets]]

[[math:def-finite-cardinality|Finiteness]]

## Justification

The proof below verifies the cutoff quotient and constructs one deletion set at each scan position. The [[lem-finite-deletions-and-translated-support|finite deletion lemma]] then gives a unique finite output from $I_H$.

## Facts & Assumptions

[F1] [[math:thm-division-algorithm-in-z|Division with remainder]] gives a unique integer quotient and remainder for any integer dividend and positive integer divisor, with remainder at least zero and less than the divisor.

[F2] The [[math:def-int-operations|integer operations]] give addition, negation and multiplication. The [[math:thm-int-ordered-ring|ordered-ring laws for the integers]] give the usual additive inverses and distributivity, allow addition of the same integer to both sides of an inequality, and make a product of positive integers positive. The integer order is total.

[F3] The [[math:def-natural-numbers|natural numbers]] are $0,1,2,\ldots$, with $1=0^+$, where $t^+$ denotes the natural successor of $t$. The recursion for [[math:def-nat-addition|natural-number addition]] gives $t+0=t$ and $t+u^+=(t+u)^+$, so $t+1=t^+$. In the [[math:def-nat-order|natural order]], $s\le t$ means that $s+u=t$ for some natural number $u$. By [[math:lem-nat-discrete|discreteness of natural order]], $t<r$ if and only if $t^+\le r$. The [[math:lem-nat-embeds-int|canonical map]] $\iota:\mathbb N\to\mathbb Z$ is injective, has image the nonnegative integers, preserves addition, and preserves and reflects order. The [[math:def-int-operations|integer zero and one]] are $\iota(0)$ and $\iota(1)$.

[F4] For every nonnegative integer $B$, the [[def-author-c74aeff6099d-bounded-integer-indices|bounded index set]] $I_B$ is finite and contains exactly the integers from $0$ through $B$. The [[def-euler-finite-certificate-indices|certificate definition]] gives a unique binary value $\varepsilon_t$ at each integer $t\le H$. The [[def-euler-finite-first-summand-indices|definition of $J$]] selects exactly the indices in $I_{78}$ with indicator $1$.

[F5] [[math:def-axiom-schema-of-separation|Separation]] selects exactly the elements of an existing set satisfying a specified condition. [[math:def-axiom-of-extensionality|Extensionality]] identifies sets with the same elements. The [[math:def-power-set|power set]] $\mathcal P(I_H)$ consists of all subsets of $I_H$. The [[math:def-cartesian-product|Cartesian product]] $L\times\mathcal P(I_H)$ consists of the ordered pairs $(j,E)$ with $j\in L$ and $E\subseteq I_H$. An [[math:def-indexed-family|indexed family on $L$]] is a [[math:def-function|function]] assigning exactly one value to each index in $L$.

[F6] The [[lem-finite-deletions-and-translated-support|finite deletion lemma]] gives a unique sequence $C_0,\ldots,C_r$ of finite subsets from any finite starting set $C_0$ of integers and family $(E_j)_{1\le j\le r}$ of sets of integers with $r$ natural. Its update is $C_{t^+}=C_t\setminus E_{t^+}$ for $0\le t<r$. By the [[math:def-set-difference-and-symmetric-difference|definition of difference]], deletion of an empty set leaves membership unchanged.

[F7] By the [[math:def-injection-surjection-bijection|definitions of injection, surjection and bijection]], a function is injective when equal values have equal inputs, surjective when every element of its codomain is a value, and bijective when it is both.

## Proof

**Given:** An integer $a$ satisfying the stated bounds and congruence, and the fixed data $H$, $\varepsilon_j$ and $J$.

**Goal:** Show that the procedure specifies a unique finite output at every allowed cutoff.

1.1 The congruence supplies an integer $m$ with $a-1=4m$, so division of $a-1$ by the positive integer $4$ has remainder zero and unique quotient $m$. The bounds on $a$ give $0\le4m\le312=4\cdot78$. If $x<y$ are integers, then $4(y-x)>0$, so $4x<4y$. By totality, the bounds on $4m$ imply $0\le m\le78$. [given, F1, F2]

2.1 Let $r$ be the unique natural number with $\iota(r)=m+1$, and let $L=\{j\in\mathbb N:1\le j\le r\}$, obtained by separation in the naturals. For each $j\in L$, order preservation gives $1\le\iota(j)\le m+1$, so $i=\iota(j)-1$ belongs to $I_m$. The pairs $(j,i)$ with $i=\iota(j)-1$ form the graph of a function $f:L\to I_m$ by separation in $L\times I_m$, since there is exactly one value for every $j\in L$. For each $i\in I_m$ we have $1\le i+1\le m+1$. Then $i+1$ has a unique natural preimage under $\iota$, and order reflection puts that preimage in $L$. Adding $1$ to $f(j)=i$ gives $\iota(j)=i+1$, so this preimage is the only $j\in L$ with $f(j)=i$. Every $i\in I_m$ has a preimage, giving surjectivity, and uniqueness gives injectivity. Thus $f$ is a bijection. If $j<j'$ in $L$, order preservation and injectivity give $\iota(j)<\iota(j')$. Subtracting $1$ preserves this strict inequality by order compatibility and additive cancellation. Hence $f$ is increasing, with $f(1)=0$ and $f(r)=m$. [step 1.1, F2, F3, F4, F5, F7]

3.1 For $0\le t<r$ in the naturals put $j=t^+$. Then $j\le r$ by discreteness. Since $\iota(j)=\iota(t+1)=\iota(t)+1\ge1$, order reflection gives $1\le j$, so $j\in L$. The scan position for this update is $i=\iota(j)-1=\iota(t)$. Conversely, for any $j\in L$, put $i=\iota(j)-1$ and take the unique natural $t$ with $\iota(t)=i$. Then $\iota(t^+)=i+1=\iota(j)$, so $t^+=j$ by injectivity and $t<r$ by discreteness. Therefore the successive updates advance the integer index by one, starting at $i=0$ and ending at $i=m$. [step 2.1, F2, F3]

3.2 For $j\in L$ put $i=\iota(j)-1$. For all $k\in I_H$ we have $k-i\le k\le H$ because $i\ge0$. Thus $\varepsilon_{k-i}$ is defined, including its zero value if $k<i$. By separation and extensionality there is exactly one subset $E_j$ of $I_H$ containing precisely those $k\in I_H$ for which $i\in J$, $i\le k$ and $\varepsilon_{k-i}=1$. Separating the pairs $(j,E)$ with this defining condition on $E$ inside $L\times\mathcal P(I_H)$ gives the indexed family $(E_j)_{j\in L}$, since each $j$ has exactly one such $E$. [step 2.1, F2, F4, F5]

4.1 Apply the finite deletion lemma with starting set $I_H$ and the family from step 3.2. At the update $C_{t^+}=C_t\setminus E_{t^+}$ the integer index is $i=\iota(t)$ by step 3.1. For $i\in J$ this is the stipulated deletion, and for $i\notin J$ the set $E_{t^+}$ is empty, so the difference leaves the current set unchanged. Since $4i+1\le a$ is equivalent to $i\le m$ by step 1.1 and $a=4m+1$, the scan performs precisely the updates for $i\in J$ with $i\le m$, in increasing order, and returns $C_r$, the unique finite subset left after the $r$ scan positions. When $a=313$, $m=78$, so the scan includes every index in $J$. [step 1.1, step 3.1, step 3.2, F2, F4, F5, F6] ∎

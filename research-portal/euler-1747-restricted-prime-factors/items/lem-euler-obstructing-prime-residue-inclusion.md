---
id: lem-euler-obstructing-prime-residue-inclusion
kind: lemma
title: Residues of obstructing primes above 3
status: draft
domain: mathematics
deps:
  - def-euler-prime-classes
  - def-euler-obstructing-prime-residue-count
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - math:thm-division-algorithm-in-z
  - math:thm-int-ordered-ring
  - math:def-natural-numbers
  - math:def-nat-order
  - math:lem-nat-embeds-int
  - math:lem-nat-order-is-membership
formulation_deps:
  - def-euler-prime-classes
  - def-euler-obstructing-prime-residue-count
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - math:thm-division-algorithm-in-z
argument_deps:
  - def-euler-prime-classes
  - def-euler-obstructing-prime-residue-count
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - math:thm-division-algorithm-in-z
  - math:thm-int-ordered-ring
  - math:def-natural-numbers
  - math:def-nat-order
  - math:lem-nat-embeds-int
  - math:lem-nat-order-is-membership
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  def-euler-obstructing-prime-residue-count: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 6, Lemma 5.2, first sentence of proof
dependency_level: 2
---

## Statement

Let $\mathcal P_3$ be the set of primes congruent to $3$ modulo $4$. These are the obstructing primes. An integer $p$ is prime if $p>1$ and its only positive divisors are $1$ and $p$. For integers $d,a$, a divisor $d$ of $a$ satisfies $a=dq$ for some integer $q$, and it is positive when $d>0$. For integers $a,b,m$, congruence $a\equiv b\pmod m$ means that $a-b=mq$ for some integer $q$.

For every $p\in\mathcal P_3$ with $p>3$, its residue class modulo $60$ belongs to $\mathcal S$. Here the residue class of $p$ is $[r]_{60}=\{n\in\mathbb Z:n\equiv r\pmod{60}\}$, where $\mathbb Z$ denotes the integers and $r$ is the unique integer with $0\le r<60$ and $p\equiv r\pmod{60}$. The set $\mathcal S$ consists of the classes with representatives $7,11,19,23,31,43,47,59$.

## Statement references

[[def-euler-prime-classes|The prime class consisting of primes congruent to $3$ modulo $4$]]

[[def-euler-obstructing-prime-residue-count|The residue classes in $\mathcal S$]]

[[math:thm-division-algorithm-in-z|Existence and uniqueness of the remainder]]

## Facts & Assumptions

[F1] Membership in $\mathcal P_3$ means that $p$ is prime and $p\equiv3\pmod4$ ([[def-euler-prime-classes|Definition of the prime class]]). The condition $d\mid a$ means $a=dq$ for some integer $q$ ([[math:def-divides-in-z|Integer divisibility]]). For prime $p$, every positive divisor of $p$ is either $1$ or $p$ ([[math:def-prime|Definition of a prime]]). Congruence $a\equiv b\pmod m$ is equivalent to $m\mid(a-b)$ ([[math:def-congruence-modulo-an-integer|Integer congruence]]).

[F2] If $a$ and $b$ are integers and $b>0$, there are unique integers $q,r$ with $a=qb+r$ and $0\le r<b$. The integer $r$ is the remainder on division by $b$ ([[math:thm-division-algorithm-in-z|Division with remainder]]).

[F3] The integer operations satisfy the commutative ring laws, including distributivity. The integer order is total and is preserved by adding the same integer to both sides or multiplying both sides by a positive integer ([[math:def-integers|The integers]], [[math:def-int-operations|Integer arithmetic]], [[math:def-int-order|Integer order]], [[math:thm-int-ordered-ring|The ordered ring of integers]]).

[F4] Write $\mathbb N$ for the natural numbers in which $0$ is the empty set and the successor of $n$ is $n\cup\{n\}$ ([[math:def-natural-numbers|Construction of the natural numbers]]). Use the strict order associated with the additive order on $\mathbb N$ ([[math:def-nat-order|Order on the natural numbers]]). The natural number $15$ is $\{0,1,\ldots,14\}$, and $k<15$ for $k\in\mathbb N$ exactly when $k\in15$ ([[math:lem-nat-order-is-membership|Natural numbers below a given natural number]]). The map $\iota$ from the natural numbers to the integers is injective, has image the nonnegative integers, and satisfies $\iota(k)\le\iota(n)$ exactly when $k\le n$. It preserves addition and multiplication ([[math:lem-nat-embeds-int|Embedding of the natural numbers in the integers]]). We use the same numerals for these integers.

[F5] For each $0\le r<60$, membership in $[r]_{60}$ means congruence to $r$ modulo $60$, and $\mathcal S$ consists of the eight classes listed in the statement ([[def-euler-obstructing-prime-residue-count|Definition of the eight residue classes]]).

## Proof

**Given:** An integer $p\in\mathcal P_3$ with $p>3$.

**Goal:** Show that the residue class of $p$ modulo $60$ belongs to $\mathcal S$.

1.1 By [F1], write $p=4u+3$ for an integer $u$. Thus $p$ has remainder $3$ on division by $4$. The integer $5=4\cdot1+1$ has remainder $1$, so uniqueness in [F2] gives $p\ne5$. The integers $3$ and $5$ are both positive and distinct from $1$ and $p$, since $p>3$ and $p\ne5$. The definition of prime therefore gives $3\nmid p$ and $5\nmid p$. [given, F1, F2, F3]

2.1 Divide $u$ by $15$ using [F2] to obtain $u=15q+j$ with $0\le j<15$. By [F4], write $j=\iota(k)$ with $k\in\mathbb N$. Since $j<\iota(15)$, order reflection gives $k\le15$, and $k=15$ would give $j=\iota(15)$. Thus $k<15$, so $k\in15=\{0,1,\ldots,14\}$ and $j$ is one of the corresponding integers. Substitution gives $p=60q+r$ with $r=4j+3$. The bounds $0\le j\le14$ give $3\le r\le59$, so $r$ is the remainder on division by $60$. In order of increasing $j$, the possible values of $r$ are $3,7,11,15,19,23,27,31,35,39,43,47,51,55,59$. [F2, F3, F4, step 1.1]

3.1 The entries $3,15,27,39,51$ are $3$ times $1,5,9,13,17$, respectively, and $35,55$ are $5$ times $7,11$, respectively. If $r=3v$ for an integer $v$, then $p=60q+r=3(20q+v)$, contrary to $3\nmid p$. If $r=5v$ for an integer $v$, then $p=60q+r=5(12q+v)$, contrary to $5\nmid p$. Removing those seven entries leaves $r\in\{7,11,19,23,31,43,47,59\}$. [F1, F3, step 1.1, step 2.1]

4.1 Since $p-r=60q$, the integer $p$ is congruent to $r$ modulo $60$. The surviving values of $r$ represent precisely the classes in $\mathcal S$, so the residue class $[r]_{60}$ of $p$ belongs to $\mathcal S$. [F1, F5, step 2.1, step 3.1] ∎

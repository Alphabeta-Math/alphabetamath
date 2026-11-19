---
id: lem-invertible-linear-residue-progression
kind: lemma
title: Progression of roots of an invertible linear congruence
status: draft
domain: mathematics
deps:
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:lem-nat-embeds-int
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-integers-modulo-n
  - math:def-addition-and-multiplication-modulo-n
  - math:def-field
  - math:thm-z-mod-p-is-a-field
  - math:thm-division-algorithm-in-z
  - math:thm-int-ordered-ring
  - math:def-natural-numbers
  - math:def-ring
  - math:def-ordered-ring
formulation_deps:
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:thm-int-ordered-ring
argument_deps:
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:lem-nat-embeds-int
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-integers-modulo-n
  - math:def-addition-and-multiplication-modulo-n
  - math:def-field
  - math:thm-z-mod-p-is-a-field
  - math:thm-division-algorithm-in-z
  - math:thm-int-ordered-ring
  - math:def-natural-numbers
  - math:def-ring
  - math:def-ordered-ring
dependency_roles:
  math:def-integers: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-int-order: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-integers-modulo-n: mathematical-premise
  math:def-addition-and-multiplication-modulo-n: mathematical-premise
  math:def-field: mathematical-premise
  math:thm-z-mod-p-is-a-field: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-ring: mathematical-premise
  math:def-ordered-ring: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $p$ be a prime integer, meaning that $p>1$ and its only positive divisors are $1$ and $p$. Let $a,b$ be integers with $p\nmid a$, meaning that $a$ is not an integer multiple of $p$. The congruence $aj+b\equiv0\pmod p$ means that $aj+b$ is an integer multiple of $p$.

There is exactly one integer solution $j_0$ with $0\le j_0<p$. The nonnegative integer solutions, those with $j\ge0$, are exactly the progression $j_0+rp$ with $r$ an integer satisfying $r\ge0$.

## Statement references

[[math:def-integers|Integers]]

[[math:def-int-operations|Integer operations and constants]]

[[math:def-int-order|Integer order]]

[[math:def-prime|Prime integers]]

[[math:def-divides-in-z|Integer divisibility]]

[[math:def-congruence-modulo-an-integer|Congruence modulo an integer]]

[[math:thm-int-ordered-ring|Ordered integers]]

## Facts & Assumptions

[F1] For integers $d,x$, $d\mid x$ means $x=dq$ for some integer $q$, and $d\nmid x$ is its negation ([[math:def-divides-in-z]]). Congruence $x\equiv y\pmod p$ means $p\mid(x-y)$ ([[math:def-congruence-modulo-an-integer]]). A prime exceeds $1$ and has only $1$ and itself as positive divisors ([[math:def-prime]]).

[F2] The residue class $[x]_p$ is the set of integers congruent to $x$ modulo $p$. The set of all these classes is $\mathbb Z/p$, and $[x]_p=[y]_p$ holds exactly when $x\equiv y\pmod p$ ([[math:def-integers-modulo-n]]).

[F3] Write $\mathbb N$ for the natural numbers ([[math:def-natural-numbers]]). Because the prime $p$ is positive, the canonical embedding $\iota$ of the natural numbers into the integers gives a unique natural number $n$ with $\iota(n)=p$ ([[math:lem-nat-embeds-int]]). Use $n$ as the natural modulus and $p$ as its integer image in the class notation. With that modulus, addition and multiplication of classes are given by $[x]_p+[y]_p=[x+y]_p$ and $[x]_p[y]_p=[xy]_p$ ([[math:def-addition-and-multiplication-modulo-n]]). The formulas and the integer laws in F6 give $[0]_p$ as additive zero, $[1]_p$ as multiplicative one, and $[-x]_p$ as the additive inverse of $[x]_p$.

[F4] For prime $p$, these operations make $\mathbb Z/p$ a field ([[math:thm-z-mod-p-is-a-field]]). In particular, addition permits cancellation, multiplication is associative, and every nonzero element $u$ has a multiplicative inverse $u^{-1}$ satisfying $uu^{-1}=u^{-1}u=1$, where $1$ is the multiplicative identity ([[math:def-field]]).

[F5] Division with remainder gives, for each integer $t$ and positive integer $p$, a unique pair of integers $q,s$ with $t=qp+s$ and $0\le s<p$ ([[math:thm-division-algorithm-in-z]]).

[F6] Use the integer addition, multiplication, additive inverses, zero and one ([[math:def-int-operations]]) and the usual order on the integers ([[math:def-int-order]]). This structure on the integers ([[math:def-integers]]) forms a totally ordered commutative ring ([[math:thm-int-ordered-ring]]). Use the ring laws for additive identities and inverses, and distributivity ([[math:def-ring]]), as well as commutativity of integer multiplication. In particular, $0x=0$ follows by distributing $(0+0)x$ and cancelling $0x$. The order is total, adding the same integer preserves inequalities, and the product of positive integers is positive ([[math:def-ordered-ring]]). Translation preserves strict inequalities because cancellation rules out equality after translation.

## Proof

**Given:** A prime integer $p$ and integers $a,b$ with $p\nmid a$.

**Goal:** Find the unique integer solution $j_0$ in $0\le j_0<p$ and characterize all nonnegative integer solutions of $aj+b\equiv0\pmod p$.

1.1 Since $p\nmid a$, the class $[a]_p$ differs from $[0]_p$. The congruence for an integer $j$ is equivalent to $[a]_p[j]_p+[b]_p=[0]_p$. Adding $[-b]_p$ and multiplying on the left by $[a]_p^{-1}$ transforms this equation into $[j]_p=[a]_p^{-1}[-b]_p$. Multiplying back by $[a]_p$ and adding $[b]_p$ reverses both operations, so this class equation is equivalent to the congruence. [given, F1, F2, F3, F4, F6]

2.1 Choose an integer $t$ whose class is $[a]_p^{-1}[-b]_p$. Since $p>0$, divide $t$ by $p$ to write $t=qp+j_0$ with $0\le j_0<p$. Subtracting $j_0$ and commuting the product gives $t-j_0=pq$, so $p\mid(t-j_0)$ and $[j_0]_p=[t]_p$. Thus $j_0$ solves the congruence. [step 1.1, F1, F2, F5, F6]

3.1 An integer $j$ solves the congruence exactly when $[j]_p=[j_0]_p$, or equivalently when $p\mid(j-j_0)$. The latter condition says $j-j_0=pr$ for some integer $r$, which is equivalent to $j=j_0+rp$ by adding $j_0$ and commuting the product. [step 1.1, step 2.1, F1, F2, F6]

4.1 If $j$ is a solution with $0\le j<p$, then $j=0\cdot p+j$ and $j=rp+j_0$ are both divisions of $j$ by $p$ with remainders in the required range. Uniqueness of the remainder gives $j=j_0$. [step 2.1, step 3.1, F5, F6]

5.1 For any solution $j\ge0$, take $r$ as in step 3.1. If $r<0$, translation gives $-r>0$. Since $p>0$, the product $(-r)p$ is positive, and distributivity gives $rp+(-r)p=(r+(-r))p=0$. Translating $0<(-r)p$ by $rp$ gives $rp<0$, so $0\le j<j_0<p$. This contradicts step 4.1, so $r\ge0$. [step 3.1, step 4.1, F1, F6]

6.1 Conversely, if $r\ge0$, then $rp\ge0$ by the zero law when $r=0$ and the positive product law when $r>0$. Thus $j=j_0+rp\ge j_0\ge0$ and $j$ is a solution by step 3.1. Together with steps 4.1 and 5.1, this proves both claims. [step 2.1, step 3.1, step 4.1, step 5.1, F1, F6] ∎

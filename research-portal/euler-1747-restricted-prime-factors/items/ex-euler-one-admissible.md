---
id: ex-euler-one-admissible
kind: example
title: The summand 1 is admissible
status: published
domain: mathematics
deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:thm-int-ordered-ring
  - math:def-int-abs
  - math:lem-divisor-bound
formulation_deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
argument_deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:thm-int-ordered-ring
  - math:def-int-abs
  - math:lem-divisor-bound
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-int-abs: mathematical-premise
  math:lem-divisor-bound: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, Abstract and §1, opening paragraph
      reading_limits: Abstract and the opening of Section 1 on the frozen PDF's first
        page, for attribution.
dependency_level: 2
---

## Example

The integer $1$ belongs to $\mathcal A$, the set of positive integers whose prime divisors are all congruent to $1$ modulo $4$.

## Facts & Assumptions

[F1] By [[def-euler-prime-classes]], an integer $a$ belongs to $\mathcal A$ exactly when it is positive and every prime $p$ that divides $a$ is congruent to $1$ modulo $4$.

[F2] Write $\mathbb Z$ for the integers ([[math:def-integers]]), with integer numerals and arithmetic as in [[math:def-int-operations]]. An integer $a$ is positive when $0<a$ and nonnegative when $0\le a$. Here $x<y$ means $x\le y$ and $x\ne y$ ([[math:def-int-order]]). The integer order is antisymmetric, so $x\le y$ and $y\le x$ imply $x=y$ ([[math:thm-int-ordered-ring]]).

[F3] In the natural numbers, $0$ has no elements and $1$ has $0$ as its only element, so they are distinct ([[math:def-natural-numbers]]). The map of [[math:lem-nat-embeds-int]] sends distinct natural numbers to distinct integers and has image the nonnegative integers. It sends natural $0$ and $1$ to integer $0$ and $1$, respectively, by the definitions of the integer constants in [[math:def-int-operations]].

[F4] An integer $p$ is prime when $p>1$ and its only positive divisors are $1$ and $p$ ([[math:def-prime]]). For integers $d,a$, $d\mid a$ means $a=dq$ for some integer $q$, in which case $d$ is a divisor of $a$ ([[math:def-divides-in-z]]). A prime divisor is a divisor that is prime. Congruence of $p$ to $1$ modulo $4$ means that $4\mid(p-1)$ ([[math:def-congruence-modulo-an-integer]]).

[F5] For integers $a,d$, if $a\ne 0$ and $d\mid a$, then $d\le |a|$ by [[math:lem-divisor-bound]]. For a nonnegative integer $a$, the absolute value $|a|$ equals $a$ ([[math:def-int-abs]]).

## Verification

**Given:** The integers and the set $\mathcal A$ defined in [F1].

**Goal:** Show that $1$ belongs to $\mathcal A$.

1.1 Integer $1$ is in the image of the map from natural numbers, so $0\le 1$. The images of natural $0$ and $1$ are distinct, so $1\ne 0$ as an integer. Thus $0<1$. [F2, F3]

2.1 If $p$ were a prime divisor of $1$, then $1<p$ and $p\mid 1$. Since $1\ne 0$ and $|1|=1$, the divisor bound gives $p\le 1$. Together with $1<p$, this would force $p=1$ by antisymmetry and $p\ne 1$ by the definition of strict order. Thus $1$ has no prime divisor. [F2, F4, F5, step 1.1]

3.1 For every prime $p$, the implication from $p\mid 1$ to congruence of $p$ to $1$ modulo $4$ holds because $p\mid 1$ fails. Since $1$ is positive, [F1] gives $1\in\mathcal A$. [F1, F4, step 1.1, step 2.1] ∎

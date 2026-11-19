---
id: lem-author-f93d28423212-admissible-square-grouping
kind: lemma
title: Grouping an odd-prime four-square representation
status: published
domain: mathematics
proof_strategy: direct
deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - math:def-prime
  - math:def-divides-in-z
  - math:def-sum-of-four-squares-representation
  - math:thm-division-algorithm-in-z
  - math:thm-int-ordered-ring
  - math:lem-three-mod-four-prime-dividing-two-square-sum
  - math:lem-congruence-respects-integer-arithmetic
formulation_deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - math:def-prime
  - math:def-divides-in-z
  - math:def-sum-of-four-squares-representation
argument_deps:
  - def-euler-prime-classes
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - math:def-prime
  - math:def-divides-in-z
  - math:thm-division-algorithm-in-z
  - math:thm-int-ordered-ring
  - math:lem-three-mod-four-prime-dividing-two-square-sum
  - math:lem-congruence-respects-integer-arithmetic
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-sum-of-four-squares-representation: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:lem-three-mod-four-prime-dividing-two-square-sum: mathematical-premise
  math:lem-congruence-respects-integer-arithmetic: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 2
---

## Statement

Let $n\equiv2\pmod4$ be a positive integer and let $(p,q,x,y)$ be an ordered integer quadruple with $n=p^2+q^2+x^2+y^2$. Suppose $p$ and $q$ are primes greater than $2$ and that $p$ does not divide $x$ and $q$ does not divide $y$. Then $p^2+x^2$ and $q^2+y^2$ are admissible, meaning that they are positive and every prime divisor of either integer is congruent to $1$ modulo $4$.

## Facts & Assumptions

[F1] The arithmetic is integer addition, multiplication and subtraction. Divisibility $d\mid t$ means $t=dk$ for an integer $k$. Congruence $z\equiv r\pmod4$ means $4\mid(z-r)$. A prime exceeds $1$ and has no positive divisors except $1$ and itself. An integer is even if divisible by $2$ and odd if its remainder on division by $2$ is $1$. For a positive integer $b$, every integer $z$ has a unique expression $z=bu+r$ with integers $u,r$ and $0\le r<b$. [[math:def-int-operations]] [[math:def-divides-in-z]] [[math:def-congruence-modulo-an-integer]] [[math:def-prime]] [[math:thm-division-algorithm-in-z]]

[F2] If a prime $r\equiv3\pmod4$ divides $s^2+t^2$ for integers $s,t$, then $r$ divides both $s$ and $t$. [[math:lem-three-mod-four-prime-dividing-two-square-sum]]

[F3] The integers form a totally ordered commutative ring. An admissible integer is a positive integer all of whose prime divisors are congruent to $1$ modulo $4$. [[math:thm-int-ordered-ring]] [[def-euler-prime-classes]]

[F4] Replacing integer summands or operands of subtraction by congruent integers preserves the congruence modulo $4$. [[math:lem-congruence-respects-integer-arithmetic]]

## Proof

**Given:** The representation and prime conditions in the statement.

**Goal:** Prove that both indicated summands are admissible.

1.1 A prime greater than $2$ cannot have $2$ as a divisor, so division by $2$ gives remainder $1$ for both $p$ and $q$. Each coordinate has the form $2k$ or $2k+1$ by division by $2$. The square of $2k$ is $4k^2$ and the square of $2k+1$ is $4(k^2+k)+1$. Thus a coordinate's square has remainder $0$ or $1$ upon division by $4$ according as the coordinate is even or odd. [given, F1, F3, algebra]

2.1 The prime squares have remainder $1$. By [F4], $x^2+y^2=n-(p^2+q^2)\equiv2-(1+1)=0\pmod4$. If $a,b$ are the remainders of $x^2,y^2$ upon division by $4$, then $x^2+y^2$ is congruent to $a+b$ modulo $4$, and $a+b$ lies between $0$ and $2$. By uniqueness of the remainder, $a+b=0$, so $a=b=0$ and both $x$ and $y$ are even. [given, step 1.1, F1, F3, F4]

3.1 Each grouped sum is positive since its prime square is positive and its other square is nonnegative. By [F4] each grouped sum is congruent to $1$ modulo $4$. Each therefore has the form $4k+1=2(2k)+1$, so neither is divisible by $2$. If a prime $r\equiv3\pmod4$ divides $p^2+x^2$, then [F2] implies $r\mid p$ and $r\mid x$. Since $p$ is prime and $r>1$, this gives $r=p$ and contradicts the given exclusion of $p\mid x$. The same argument with $(q,y)$ excludes such a prime from $q^2+y^2$. [given, step 1.1, step 2.1, F1, F2, F3, F4]

4.1 A prime other than $2$ is odd by the divisor argument in step 1.1. Division by $4$ gives remainder $1$ or $3$, since remainders $0$ and $2$ would give an even integer. Step 3.1 rules out both $2$ and primes congruent to $3$ modulo $4$ as divisors of the grouped sums. By positivity and the admissibility definition, both sums are admissible. [step 1.1, step 3.1, F1, F3] ∎

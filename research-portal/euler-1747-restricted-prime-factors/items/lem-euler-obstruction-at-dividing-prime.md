---
id: lem-euler-obstruction-at-dividing-prime
kind: lemma
title: The obstruction count at a prime dividing the odd part
status: published
domain: mathematics
deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - def-euler-prime-classes
  - lem-square-residue-parity
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - math:def-finite-cardinality
  - def-euler-divisor-functions
  - math:lem-nat-embeds-int
  - math:thm-int-ordered-ring
  - math:lem-int-cancellation
  - lem-euler-nonsplit-square-obstruction
  - lem-euler-mixed-four-square-count
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:def-cartesian-product
  - math:def-subset-and-proper-subset
formulation_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - def-euler-prime-classes
  - lem-square-residue-parity
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - math:def-finite-cardinality
  - def-euler-divisor-functions
  - math:lem-nat-embeds-int
argument_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - def-euler-prime-classes
  - lem-square-residue-parity
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - math:def-finite-cardinality
  - def-euler-divisor-functions
  - math:lem-nat-embeds-int
  - math:thm-int-ordered-ring
  - math:lem-int-cancellation
  - lem-euler-nonsplit-square-obstruction
  - lem-euler-mixed-four-square-count
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:def-cartesian-product
  - math:def-subset-and-proper-subset
dependency_roles:
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  lem-square-residue-parity: mathematical-premise
  def-euler-mixed-four-square-representations: mathematical-premise
  def-euler-prime-obstruction-count: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  def-euler-divisor-functions: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:lem-int-cancellation: mathematical-premise
  lem-euler-nonsplit-square-obstruction: mathematical-premise
  lem-euler-mixed-four-square-count: mathematical-premise
  math:def-function: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, Completion of Proposition 3.1, formula for the dividing-prime
        obstruction count
dependency_level: 3
---

## Statement

Let $m$ be a positive odd integer, so $m>0$ and $m=2k+1$ for some integer $k$, and set $n=2m$. For integers $d,z$, write $d\mid z$ if $z=dq$ for some integer $q$, and $d\nmid z$ if there is no such $q$. Let $p\in\mathcal P_3$ and suppose $p\mid m$. Here $\mathcal P_3$ is the set of primes with $4\mid(p-3)$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Write $z^2=z\cdot z$.

For each positive integer $u$, let $\mathcal R_{\mathrm{mix}}(u)$ be the set of ordered integer quadruples $(x_1,x_2,x_3,x_4)$ whose squares sum to $u$ and for which each of the pairs $(x_1,x_2)$ and $(x_3,x_4)$ has one even and one odd entry. An even entry has the form $2a$ and an odd entry has the form $2a+1$, for some integer $a$. Entries may be negative, zero, or positive. Let $E_p(u)$ be the set of exceptional quadruples, meaning the elements of $\mathcal R_{\mathrm{mix}}(u)$ for which at least one of these pairs has both entries divisible by $p$. Write $b_p(u)=|E_p(u)|$ for the number of distinct elements of this finite set, and $\sigma(u)$ for the sum of the positive divisors of $u$. Identify these natural-number counts and sums with their images in the integers.

Every element of $E_p(n)$ has all four entries divisible by $p$. The count is $b_p(n)=0$ if $p^2\nmid m$, and $b_p(n)=16\sigma(m/p^2)$ if $p^2\mid m$. In the second case, $m/p^2$ is the unique integer $t$ with $m=p^2t$.

## Statement references

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-divides-in-z]]

[[math:def-prime]]

[[math:def-congruence-modulo-an-integer]]

[[def-euler-prime-classes]]

[[lem-square-residue-parity]]

[[def-euler-mixed-four-square-representations]]

[[def-euler-prime-obstruction-count]]

[[math:def-finite-cardinality]]

[[def-euler-divisor-functions]]

[[math:lem-nat-embeds-int]]

## Facts & Assumptions

[F1] Integer addition and multiplication are associative and commutative, multiplication distributes over addition, and the integer order is total and preserved by addition. Products of positive integers are positive. The natural numbers are identified with the nonnegative integers by an inclusion that preserves addition, multiplication and order. [[math:def-integers]] [[math:def-int-order]] [[math:def-int-operations]] [[math:thm-int-ordered-ring]] [[math:lem-nat-embeds-int]]

[F2] Divisibility is witnessed by an exact integer multiple. In particular $d\mid 0$ since $0=d\cdot 0$. For $p\in\mathcal P_3$, primality gives $p>1$ and congruence to $3$ modulo $4$ gives $p-3=4r$ for some integer $r$. [[math:def-divides-in-z]] [[def-euler-prime-classes]] [[math:def-prime]] [[math:def-congruence-modulo-an-integer]]

[F3] For each positive integer $u$, the finite set $\mathcal R_{\mathrm{mix}}(u)$ is specified by the square-sum and parity conditions in the Statement. Equality of ordered quadruples is entry by entry. Its exceptional subset $E_p(u)$ is finite, and $b_p(u)$ counts its distinct elements. [[def-euler-mixed-four-square-representations]] [[def-euler-prime-obstruction-count]]

[F4] If $p\in\mathcal P_3$ and $a,b$ are integers with $p\mid a^2+b^2$, then $p\mid a$ and $p\mid b$. [[lem-euler-nonsplit-square-obstruction]]

[F5] Exact division by a positive odd integer preserves the parity of each entry of a pair that it divides. For a single integer $z$ divisible by such an integer $d$, this applies to the pair $(z,0)$ because $d\mid 0$. [[lem-square-residue-parity]] [[math:def-divides-in-z]]

[F6] A common nonzero factor can be cancelled from an equality of integer products. [[math:lem-int-cancellation]]

[F7] A function from one set to another assigns exactly one output to each input. It is a bijection if every element of the target is the output of exactly one input. Finite sets in bijection have equal cardinalities, and the empty set has cardinality zero. [[math:def-function]] [[math:def-injection-surjection-bijection]] [[math:def-finite-cardinality]]

[F8] For a positive integer $u$, $\sigma(u)$ is the sum of its positive divisors. If $u$ is also odd, then $|\mathcal R_{\mathrm{mix}}(2u)|=16\sigma(u)$. [[def-euler-divisor-functions]] [[lem-euler-mixed-four-square-count]]

[F9] For sets $A$ and $B$, the Cartesian product $A\times B$ consists of all ordered pairs with first entry in $A$ and second entry in $B$. Separation forms a subset of that product containing exactly the pairs that satisfy a specified formula. [[math:def-cartesian-product]] [[math:def-subset-and-proper-subset]]

## Proof

**Given:** A positive odd integer $m$, the integer $n=2m$, and $p\in\mathcal P_3$ with $p\mid m$.

**Goal:** Prove that every exceptional quadruple has all four entries divisible by $p$ and establish both cases of the count.

1.1 From $p-3=4r$ write $p=2s+1$ with $s=2r+1$. Thus $p$ is odd, and $p^2=2h+1$ with $h=2s(s+1)$. Since $p>1$, both $p$ and $p^2$ are positive. Also $n=2m>0$. [given, F1, F2]

1.2 Take a quadruple in $E_p(n)$. Let $a,b$ be the entries of a pair divisible by $p$, and let $c,e$ be the other two entries. Write $a=pA$, $b=pB$ and $m=pv$ for integers $A,B,v$. The square-sum equation gives $c^2+e^2=2m-a^2-b^2=p(2v-p(A^2+B^2))$. Thus $p\mid c^2+e^2$ and F4 gives $p\mid c$ and $p\mid e$. All four entries are divisible by $p$. [given, F1, F2, F3, F4]

2.1 For any such quadruple write $x_i=py_i$ for each $i=1,2,3,4$, with $y_i$ an integer. With $S=y_1^2+y_2^2+y_3^2+y_4^2$, the square-sum equation gives $2m=p^2S$. Using $p^2=2h+1$, compute $m=p^2m-h(2m)=p^2(m-hS)$. This is a witness for $p^2\mid m$. If $p^2\nmid m$, then $E_p(n)$ is empty and $b_p(n)=0$. [F1, F2, F3, F7, step 1.1, step 1.2]

2.2 Suppose $p^2\mid m$ and write $m=p^2t$ with $t$ an integer. Since $p^2>0$, F6 gives uniqueness of $t$. If $t=0$ then $m=0$, and if $t<0$ then $-m=p^2(-t)>0$. Both contradict $m>0$, so $t>0$ and $2t>0$. By F5, exact division of $m$ by the positive odd integer $p^2$ makes $t$ odd because $m$ is odd. [given, F1, F2, F5, F6, step 1.1]

3.1 For each $(x_1,x_2,x_3,x_4)\in E_p(n)$, the integers $y_i$ with $x_i=py_i$ exist by Step 1.2 and are unique by F6. Since $p$ is positive and odd, F5 gives the same parity for $y_i$ as for $x_i$ in each position. The equation in Step 2.1 becomes $p^2S=2p^2t$. Cancelling $p^2$ gives $S=2t$, so $(y_1,y_2,y_3,y_4)$ belongs to $\mathcal R_{\mathrm{mix}}(2t)$. [F1, F2, F3, F5, F6, step 1.1, step 1.2, step 2.1, step 2.2]

3.2 Conversely, for $(y_1,y_2,y_3,y_4)\in\mathcal R_{\mathrm{mix}}(2t)$ define $x_i=py_i$ for each $i$. Because the exact quotient of $x_i$ by $p$ is $y_i$, F5 implies that the parity in each position agrees. The square sum of the $x_i$ is $p^2(2t)=2m=n$. Both pairs have every entry divisible by $p$, so the resulting quadruple lies in $E_p(n)$. [given, F1, F2, F3, F5, F6, step 1.1, step 2.2]

4.1 Use separation on the Cartesian product $\mathcal R_{\mathrm{mix}}(2t)\times E_p(n)$ to form the graph $G$ consisting of precisely the ordered pairs $(y,x)$ in that product for which $x_i=py_i$ for $i=1,2,3,4$. By Step 3.2, each input $y$ in the first factor has an output $x$ in the second factor. The rule fixes each coordinate of $x$, so the output is unique. Step 3.1 gives exactly one input $y$ for each $x$ in the second factor. Thus $G$ defines a bijection from $\mathcal R_{\mathrm{mix}}(2t)$ onto $E_p(n)$. [F1, F3, F7, F9, step 3.1, step 3.2]

5.1 The finite sets are in bijection, so $b_p(n)=|\mathcal R_{\mathrm{mix}}(2t)|$. Since $t=m/p^2$ is positive and odd, F8 gives $b_p(n)=16\sigma(m/p^2)$. Together with Steps 1.2 and 2.1 this proves the assertion. [F3, F7, F8, step 1.2, step 2.1, step 2.2, step 4.1] ∎

## Source notes

The dividing-prime case in the completion of Proposition 3.1 on p. 4 gives the two counts. The proof above gives the divisibility witness and the parity-preserving correspondence used to obtain them from the mixed count in (2.2).

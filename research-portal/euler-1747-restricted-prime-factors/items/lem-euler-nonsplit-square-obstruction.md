---
id: lem-euler-nonsplit-square-obstruction
kind: lemma
title: When a prime congruent to 3 modulo 4 divides a sum of two squares
status: draft
domain: mathematics
deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-quadratic-residue-modulo-n
  - math:thm-int-comm-ring
  - math:def-legendre-symbol
  - math:thm-first-supplement-to-quadratic-reciprocity
  - math:def-integers-modulo-n
  - math:def-addition-and-multiplication-modulo-n
  - math:def-field
  - math:thm-z-mod-p-is-a-field
  - math:lem-of-zero-mult
  - math:def-int-order
  - math:thm-int-ordered-ring
  - math:lem-nat-embeds-int
  - math:def-natural-numbers
  - math:def-nat-order
  - math:lem-nat-discrete
  - math:def-common-divisor-and-gcd
  - math:def-int-abs
  - math:lem-gcd-basic-values
formulation_deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-quadratic-residue-modulo-n
  - math:def-int-order
argument_deps:
  - def-euler-prime-classes
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:thm-int-comm-ring
  - math:def-legendre-symbol
  - math:def-quadratic-residue-modulo-n
  - math:thm-first-supplement-to-quadratic-reciprocity
  - math:def-integers-modulo-n
  - math:def-addition-and-multiplication-modulo-n
  - math:def-field
  - math:thm-z-mod-p-is-a-field
  - math:lem-of-zero-mult
  - math:def-int-order
  - math:thm-int-ordered-ring
  - math:lem-nat-embeds-int
  - math:def-natural-numbers
  - math:def-nat-order
  - math:lem-nat-discrete
  - math:def-common-divisor-and-gcd
  - math:def-int-abs
  - math:lem-gcd-basic-values
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-quadratic-residue-modulo-n: mathematical-premise
  math:thm-int-comm-ring: mathematical-premise
  math:def-legendre-symbol: mathematical-premise
  math:thm-first-supplement-to-quadratic-reciprocity: mathematical-premise
  math:def-integers-modulo-n: mathematical-premise
  math:def-addition-and-multiplication-modulo-n: mathematical-premise
  math:def-field: mathematical-premise
  math:thm-z-mod-p-is-a-field: mathematical-premise
  math:lem-of-zero-mult: mathematical-premise
  math:def-int-order: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:def-common-divisor-and-gcd: mathematical-premise
  math:def-int-abs: mathematical-premise
  math:lem-gcd-basic-values: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §2, quadratic nonresidue observation preceding (2.3)
dependency_level: 2
---

## Statement

Write $\mathbb Z$ for the integers and $a^2$ for the product $a\cdot a$. For integers $a,b,d,m$, write $d\mid a$ if $a=dq$ for some $q\in\mathbb Z$, and $a\equiv b\pmod m$ if $m\mid(a-b)$.

Let $p\in\mathcal P_3$, the set of primes congruent to $3$ modulo $4$. Then $-1$ is a quadratic nonresidue modulo $p$, so no integer $t$ satisfies $t^2\equiv-1\pmod p$. For all $x,y\in\mathbb Z$, if $p\mid x^2+y^2$, then $p\mid x$ and $p\mid y$.

## Statement references

[[def-euler-prime-classes]]

[[math:def-integers]]

[[math:def-int-operations]]

[[math:def-prime]]

[[math:def-int-order]]

[[math:def-divides-in-z]]

[[math:def-congruence-modulo-an-integer]]

[[math:def-quadratic-residue-modulo-n]]

## Facts & Assumptions

[F1] Membership in $\mathcal P_3$ means that $p$ is prime and $4\mid(p-3)$. A prime $p$ is an integer greater than $1$ with positive divisors exactly $1$ and $p$. The divisibility condition means $p-3=4k$ for some integer $k$ ([[def-euler-prime-classes]], [[math:def-prime]], [[math:def-int-order]], [[math:def-congruence-modulo-an-integer]], [[math:def-divides-in-z]]).

[F2] Integer addition and multiplication are associative and commutative, multiplication distributes over addition, and $0$ and $1$ are the respective identities. Subtraction is addition of the additive inverse ([[math:thm-int-comm-ring]]).

[F3] For an odd prime $p$, the Legendre symbol $\left(\frac ap\right)$ is $0$ if $p\mid a$, $1$ if $p\nmid a$ and $a$ is a quadratic residue modulo $p$, and $-1$ if $p\nmid a$ and $a$ is a quadratic nonresidue modulo $p$ ([[math:def-legendre-symbol]]).

[F4] For an integer $p\ge2$ and an integer $a$ with $\gcd(a,p)=1$ ([[math:def-common-divisor-and-gcd]]), $a$ is a quadratic residue modulo $p$ if there is an integer $t$ with $t^2\equiv a\pmod p$. A quadratic nonresidue in the same range has no such $t$ ([[math:def-quadratic-residue-modulo-n]]).

[F5] For an odd prime $p$ with $p\equiv3\pmod4$, the first supplement to quadratic reciprocity gives $\left(\frac{-1}{p}\right)=-1$ ([[math:thm-first-supplement-to-quadratic-reciprocity]]).

[F6] Write $\bar a$ for the congruence class of the integer $a$, the set of integers congruent to $a$ modulo $p$. The set of all such classes is $\mathbb Z/p$. Two classes are equal exactly when $p$ divides the difference of their representatives ([[math:def-integers-modulo-n]], [[math:def-congruence-modulo-an-integer]]).

[F7] For a natural modulus identified with its integer image, the operations on these classes are $\bar a+\bar b=\overline{a+b}$ and $\bar a\bar b=\overline{ab}$. The formulas are independent of the chosen representatives. They give $\bar 0$ as the additive identity and $\bar 1$ as the multiplicative identity by the corresponding integer identities ([F2], [[math:def-addition-and-multiplication-modulo-n]]).

[F8] Since $p$ is prime, these operations on $\mathbb Z/p$ make a field. The field axioms used below are associativity and commutativity of multiplication, distributivity over addition, and the existence of an inverse $w$ satisfying $bw=\bar 1$ for each nonzero class $b$ ([[math:thm-z-mod-p-is-a-field]], [[math:def-field]]).

[F9] In a field, multiplying any element by the additive identity gives the additive identity ([[math:lem-of-zero-mult]]).

[F10] The integer order is transitive and compatible with addition ([[math:def-int-order]], [[math:thm-int-ordered-ring]]).

[F11] The embedding $\iota(n)=[(n,0)]$ of the natural numbers into the integers preserves and reflects order, and its image is precisely the nonnegative integers. In particular $\iota(0)=0$ and $\iota(1)=1$ by the definitions of the integer constants ([[math:lem-nat-embeds-int]], [[math:def-int-operations]], [[math:def-nat-order]]).

[F12] For natural numbers $m,n$, the relation $m<n$ implies $\sigma(m)\le n$, where $\sigma$ is the successor operation. In particular $\sigma(1)=2$, and the natural numbers $0$ and $1$ are distinct ([[math:lem-nat-discrete]], [[math:def-natural-numbers]], [[math:def-nat-order]]).

[F13] For any integers $a,b$, the greatest common divisor is symmetric and unchanged by replacing its arguments with their absolute values, and $\gcd(a,1)=1$ ([[math:lem-gcd-basic-values]]). For a negative integer $a$, its absolute value is $-a$ ([[math:def-int-abs]]).

## Proof

**Given:** $p\in\mathcal P_3$ and integers $x,y$.

**Goal:** Show that $-1$ is a quadratic nonresidue modulo $p$ and that $p\mid x^2+y^2$ implies $p\mid x$ and $p\mid y$.

1.1 By membership in $\mathcal P_3$, $p$ is prime and $p-3=4k$ for some integer $k$. Thus $p=4k+3=2(2k+1)+1$, which makes $p$ odd, meaning that it is one more than twice an integer. [given, F1, F2]

2.1 Since $\iota(1)=1$ is nonnegative and distinct from $\iota(0)=0$, we have $0<1$ in the integer order. Primality gives $p>1$, so $p$ is positive and equals $\iota(n)$ for a natural number $n$. Since the embedding reflects order, $n>1$ in the natural order. The successor bound gives $n\ge2$ and hence $p\ge2$ by order preservation. Use the natural modulus $n$ for the quotient operations in [F7], identifying it with $p=\iota(n)$. [F1, F7, F10, F11, F12, step 1.1]

3.1 Let $(u,v)$ be either $(x,y)$ or $(y,x)$. If $p\mid x^2+y^2$, then $p\mid u^2+v^2$ in either ordering by commutativity of integer addition. Equality of classes and the formulas for their operations yield $\bar u^2+\bar v^2=\bar 0$. [given, F2, F6, F7, step 2.1]

3.2 Adding $-1$ to $0<1$ gives $-1<0$, so $|-1|=1$. The gcd identities give $\gcd(-1,p)=\gcd(p,-1)=\gcd(|p|,1)=1$. The odd prime $p$ satisfies $p\equiv3\pmod4$, so the first supplement gives $\left(\frac{-1}{p}\right)=-1$. The value $-1$ is the quadratic nonresidue case of the Legendre symbol. Hence $-1$ is a quadratic nonresidue modulo $p$ and no integer $t$ satisfies $t^2\equiv-1\pmod p$. [step 1.1, step 2.1, F1, F2, F3, F4, F5, F10, F13]

4.1 Suppose $p\mid x^2+y^2$. Since $p$ is prime, if $\bar v\ne\bar 0$ then it has a multiplicative inverse $w$ with $\bar v w=\bar 1$. By distributivity, associativity and commutativity of multiplication, $(\bar u w)^2+\bar 1=(\bar u^2+\bar v^2)w^2=\bar 0$. The last equality uses multiplication by the additive identity. [step 1.1, step 3.1, F7, F8, F9]

5.1 Still assuming $\bar v\ne\bar 0$, use the fact that every class has an integer representative to write $\bar u w=\bar t$ for some integer $t$. The identity in step 4.1 becomes $\overline{t^2+1}=\bar 0$, which gives $p\mid(t^2+1)$, or equivalently $t^2\equiv-1\pmod p$. This contradicts step 3.2, so $\bar v=\bar 0$. [step 3.2, step 4.1, F2, F6, F7]

6.1 Both orderings were allowed in step 3.1, so $\bar x=\bar 0$ and $\bar y=\bar 0$. Equality with the zero class gives $p\mid x$ and $p\mid y$. Together with step 3.2, this proves both assertions. [step 3.1, step 3.2, step 5.1, F6] ∎

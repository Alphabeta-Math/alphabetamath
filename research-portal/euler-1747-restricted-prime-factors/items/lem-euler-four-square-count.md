---
id: lem-euler-four-square-count
kind: lemma
title: Jacobi’s count for twice an odd integer
status: draft
domain: mathematics
deps:
  - def-euler-four-square-representations
  - def-euler-divisor-functions
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-divides-in-z
  - math:def-natural-numbers
  - math:def-nat-multiplication
  - math:lem-nat-embeds-int
  - thm-jacobi-signed-ordered-four-square-count
  - math:thm-int-ordered-ring
  - math:def-nat-addition
  - math:def-semigroup-and-monoid
  - math:def-group-power
  - math:lem-group-power-laws
  - math:lem-int-cancellation
  - math:def-nat-order
  - math:lem-nat-discrete
  - math:def-finite-cardinality
  - math:def-sum-over-a-finite-index-set
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-nat-finite-sum-and-product
  - math:def-monoid-finite-product
formulation_deps:
  - def-euler-four-square-representations
  - def-euler-divisor-functions
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-divides-in-z
  - math:def-natural-numbers
  - math:def-nat-multiplication
  - math:lem-nat-embeds-int
argument_deps:
  - def-euler-four-square-representations
  - def-euler-divisor-functions
  - thm-jacobi-signed-ordered-four-square-count
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-divides-in-z
  - math:thm-int-ordered-ring
  - math:def-natural-numbers
  - math:def-nat-addition
  - math:def-nat-multiplication
  - math:lem-nat-embeds-int
  - math:def-semigroup-and-monoid
  - math:def-group-power
  - math:lem-group-power-laws
  - math:lem-int-cancellation
  - math:def-nat-order
  - math:lem-nat-discrete
  - math:def-finite-cardinality
  - math:def-sum-over-a-finite-index-set
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-nat-finite-sum-and-product
  - math:def-monoid-finite-product
dependency_roles:
  def-euler-four-square-representations: mathematical-premise
  def-euler-divisor-functions: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-nat-multiplication: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  thm-jacobi-signed-ordered-four-square-count: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-nat-addition: mathematical-premise
  math:def-semigroup-and-monoid: mathematical-premise
  math:def-group-power: mathematical-premise
  math:lem-group-power-laws: mathematical-premise
  math:lem-int-cancellation: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:def-nat-finite-sum-and-product: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §2, equation (2.1)
dependency_level: 1
---

## Statement

Let $m$ be a positive odd integer, meaning $m>0$ and no integer $q$ satisfies $m=2q$. Set $n=2m$. Let $R(n)$ be the number of ordered integer quadruples $(x_1,x_2,x_3,x_4)$ with $x_1^2+x_2^2+x_3^2+x_4^2=n$, allowing zero and both signs in every position. Let $\sigma(m)$ be the sum of the positive integers $d$ for which $m=dq$ for some integer $q$. Then
$$R(n)=24\sigma(m).$$

## Statement references

[[def-euler-four-square-representations]]

[[def-euler-divisor-functions]]

[[math:def-integers]]

[[math:def-int-operations]]

[[math:def-int-order]]

[[math:def-divides-in-z]]

[[math:def-natural-numbers]]

[[math:def-nat-multiplication]]

[[math:lem-nat-embeds-int]]

## Facts & Assumptions

[F1] For $u>0$, $R(u)$ is the number of elements of the finite set $\mathcal R(u)$ of ordered integer quadruples with square sum $u$. The count is a natural number. [[def-euler-four-square-representations]]

[F2] For a positive natural number $v$, let $D(v)$ be the finite set of positive natural numbers whose integer images divide the image of $v$. The natural number $\sigma(v)$ is the sum of the members of $D(v)$. In the integers, $d\mid u$ means $u=dq$ for some integer $q$, and $d\nmid u$ means that no such $q$ exists. [[def-euler-divisor-functions]] [[math:def-divides-in-z]]

[F3] For a positive integer $u$, let $u_{\mathrm{odd}}=u/2^k$ be its odd part, where $k$ is the greatest natural exponent with $2^k\mid u$. Jacobi’s formula gives $\iota(|\mathcal R_4(u)|)=8(2+(-1)^u)\sum_{d\mid u_{\mathrm{odd}},\,d>0}d$, where $\mathcal R_4(u)$ consists of ordered integer quadruples with square sum $u$ and allows zero and both signs in every coordinate. The sum runs over positive integer divisors and uses integer addition. The exponent in $(-1)^u$ is the natural number whose image under $\iota$ is $u$. [[thm-jacobi-signed-ordered-four-square-count]] [[math:lem-nat-embeds-int]]

[F4] On $\mathbb Z$, addition and multiplication are associative and commutative, multiplication distributes over addition, $0$ and $1$ are the respective identities, and every integer has an additive inverse. In the integer order a product of positive integers is positive. Consequently $(\mathbb Z,\cdot,1)$ and $(\mathbb Z,+,0)$ are commutative monoids. [[math:def-integers]] [[math:def-int-operations]] [[math:def-int-order]] [[math:thm-int-ordered-ring]] [[math:def-semigroup-and-monoid]]

[F5] The natural numbers start at $0$ and have successor $s$, with $1=s(0)$ and $2=s(1)$. Their addition and multiplication use the natural recursion definitions. The map $\iota(j)=[(j,0)]$ is injective, preserves addition and multiplication, and identifies the natural order with the order on its image, the nonnegative integers. Its values at $0$ and $1$ are the integer identities $[(0,0)]$ and $[(1,0)]$. [[math:def-natural-numbers]] [[math:def-nat-addition]] [[math:def-nat-multiplication]] [[math:lem-nat-embeds-int]] [[math:def-int-operations]]

[F6] In the multiplicative monoid from F4, the natural powers of an integer $a$ are the unique function of $j\in\mathbb N$ with $a^0=1$ and $a^{s(j)}=a^ja$. For natural exponents $r,t$ the monoid power laws give $a^{r+t}=a^ra^t$ and $(a^r)^t=a^{rt}$. [[math:def-group-power]] [[math:lem-group-power-laws]]

[F7] A nonzero common integer factor cancels. If $xz=yz$ with $z\ne0$, then $x=y$. [[math:lem-int-cancellation]]

[F8] For natural numbers $a,b$, $a\le b$ means $b=a+c$ for some $c\in\mathbb N$, and $a<b$ means $a\le b$ and $a\ne b$. Discreteness gives $a<b$ if and only if $s(a)\le b$. [[math:def-nat-order]] [[math:lem-nat-discrete]]

[F9] A finite set has an enumeration by the natural number giving its cardinality, with each element appearing once. In each carrier the indexed sum is computed from the list of summands along such an enumeration. The natural sum uses the recursion for natural finite sums. The integer sum uses the finite monoid product written additively in the commutative monoid $(\mathbb Z,+,0)$ from F4. For a sequence of summands, each recursion gives a unique partial-sum function with initial value zero and successor value obtained by adding the next summand. For a finite list, its sum is the partial sum at the length of the list, and the sequence may be extended by zeros. [[math:def-finite-cardinality]] [[math:def-sum-over-a-finite-index-set]] [[math:def-finite-sum-in-a-commutative-monoid]] [[math:def-nat-finite-sum-and-product]] [[math:def-monoid-finite-product]]

## Proof

**Given:** A positive odd integer $m$ and $n=2m$.

**Goal:** Show that $R(n)=24\sigma(m)$.

1.1 The natural numeral $2$ is $1+1$ by the addition recursion. Since $\iota(1)=1$ and $\iota$ is additive, the natural $2$ maps to the integer $1+1=2$. The same reasoning with repeated addition identifies the natural and integer numerals $8$ and $24$. Since $0+2=2$ and $0\ne2$ in the naturals, $0<2$ there and hence in the integers. Thus $n=2m>0$, so Jacobi’s formula applies. The sets $\mathcal R(n)$ and $\mathcal R_4(n)$ consist of the same ordered integer quadruples, selected by the same square-sum equation. Therefore $R(n)=|\mathcal R_4(n)|$ as natural numbers. [given, F1, F3, F4, F5, F8]

2.1 Let $k$ be the greatest natural exponent with $2^k\mid n$. Since $2^1=2$, the equality $n=2m$ gives $k\ge1$. If $k\ne1$, then $1<k$, so discreteness gives $2=s(1)\le k$, and the definition of natural order gives $k=2+\ell$ for some $\ell\in\mathbb N$. By divisibility there is an integer $t$ with $2m=2^kt$. By the power law and $2^2=2\cdot2$, this is $2m=2(2\cdot2^\ell t)$. Cancelling $2$ gives $m=2(2^\ell t)$, contrary to $2\nmid m$. Thus $k=1$, and $n_{\mathrm{odd}}=m$ since $2m=n$ and a nonzero factor cancels. [given, F2, F3, F4, F5, F6, F7, F8, step 1.1]

2.2 Let $m_{\mathbb N},n_{\mathbb N}$ be the unique positive naturals with $\iota(m_{\mathbb N})=m$ and $\iota(n_{\mathbb N})=n$. Preservation of multiplication and the identification of the numeral $2$ give $\iota(2m_{\mathbb N})=2m=n$. Injectivity yields $n_{\mathbb N}=2m_{\mathbb N}$. The power law gives $(-1)^{n_{\mathbb N}}=((-1)^2)^{m_{\mathbb N}}=1^{m_{\mathbb N}}$, since $(-1)^2=1$ by the power recursion and the ring laws. The constant function with value $1$ satisfies the power recursion for base $1$, so uniqueness yields $1^{m_{\mathbb N}}=1$. This evaluates the sign factor in Jacobi’s formula. [given, F3, F4, F5, F6, step 1.1]

3.1 Since $n_{\mathrm{odd}}=m$, the embedding takes $D(m_{\mathbb N})$ bijectively onto the positive integer divisors in Jacobi’s sum. This follows from the definition of $D$ and because each positive integer has a unique positive natural preimage. Take an enumeration of $D(m_{\mathbb N})$ of length $h$ with entries $d_j$ for $j<h$. The entries $\iota(d_j)$ in the same order enumerate the integer divisors once each. [F2, F3, F5, F9, step 2.1, step 2.2]

4.1 Extend the natural list by $d_j=0$ for $j\ge h$, and use $\iota(d_j)$ for the corresponding integer list. Let $S_j$ and $T_j$ be the natural and integer partial sums of length $j$, respectively. Then $\iota(S_0)=0=T_0$, and $\iota(S_{s(j)})=\iota(S_j+d_j)=\iota(S_j)+\iota(d_j)$. Hence the embedded partial sums satisfy the integer recursion, and uniqueness gives $T_h=\iota(S_h)$. By the definitions of the sums, Jacobi’s divisor sum is therefore $\iota(\sigma(m_{\mathbb N}))$. [F2, F4, F5, F9, step 3.1]

5.1 Substituting the equal counts, the sign factor and the divisor sum into Jacobi’s integer equality gives $\iota(R(n))=8(2+1)\iota(\sigma(m_{\mathbb N}))$. Since $8(2+1)=24$ and $\iota$ preserves multiplication and the numeral $24$, the right side equals $\iota(24\sigma(m_{\mathbb N}))$. Injectivity now gives $R(n)=24\sigma(m)$ as natural numbers, with $\sigma(m)$ evaluated at the natural number corresponding to $m$. [F2, F3, F4, F5, step 1.1, step 2.2, step 4.1] ∎

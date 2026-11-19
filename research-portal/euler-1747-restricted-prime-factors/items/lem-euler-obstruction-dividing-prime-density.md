---
id: lem-euler-obstruction-dividing-prime-density
kind: lemma
title: Density bound for primes dividing the odd part
status: published
domain: mathematics
deps:
  - math:def-nat-addition
  - math:def-integers
  - math:def-semigroup-and-monoid
  - math:def-monoid-finite-product
  - math:thm-induction-principle
  - math:lem-nat-discrete
  - math:thm-int-ordered-ring
  - math:lem-nat-embeds-int
  - lem-square-residue-parity
  - math:def-divides-in-z
  - math:def-prime
  - def-euler-prime-classes
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - def-euler-divisor-functions
  - math:def-p-adic-valuation
  - math:def-group-power
  - math:def-rationals
  - math:def-rat-order
  - math:thm-division-algorithm-in-z
  - math:lem-p-adic-valuation-basic
  - math:def-finite-sum-in-a-commutative-monoid
  - lem-divisors-from-prime-exponents
  - math:def-coprime
  - math:def-common-divisor-and-gcd
  - lem-euler-four-square-count
  - lem-euler-obstruction-at-dividing-prime
  - math:thm-rat-ordered-field
formulation_deps:
  - math:def-integers
  - math:thm-int-ordered-ring
  - math:lem-nat-embeds-int
  - lem-square-residue-parity
  - math:def-divides-in-z
  - math:def-prime
  - def-euler-prime-classes
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - def-euler-divisor-functions
  - math:def-p-adic-valuation
  - math:lem-p-adic-valuation-basic
  - math:thm-division-algorithm-in-z
  - math:def-group-power
  - math:def-rationals
  - math:def-rat-order
argument_deps:
  - math:def-nat-addition
  - math:def-monoid-finite-product
  - math:def-semigroup-and-monoid
  - math:thm-induction-principle
  - math:lem-nat-discrete
  - math:thm-int-ordered-ring
  - math:lem-nat-embeds-int
  - math:thm-division-algorithm-in-z
  - math:def-divides-in-z
  - math:def-prime
  - def-euler-prime-classes
  - math:def-group-power
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - math:def-p-adic-valuation
  - math:lem-p-adic-valuation-basic
  - def-euler-divisor-functions
  - math:def-finite-sum-in-a-commutative-monoid
  - lem-divisors-from-prime-exponents
  - math:def-coprime
  - math:def-common-divisor-and-gcd
  - lem-euler-four-square-count
  - lem-euler-obstruction-at-dividing-prime
  - math:def-rationals
  - math:def-rat-order
  - math:thm-rat-ordered-field
dependency_roles:
  math:def-nat-addition: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-semigroup-and-monoid: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
  math:thm-induction-principle: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  lem-square-residue-parity: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-prime: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  def-euler-four-square-representations: mathematical-premise
  def-euler-mixed-four-square-representations: mathematical-premise
  def-euler-prime-obstruction-count: mathematical-premise
  def-euler-divisor-functions: mathematical-premise
  math:def-p-adic-valuation: mathematical-premise
  math:def-group-power: mathematical-premise
  math:def-rationals: mathematical-premise
  math:def-rat-order: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:lem-p-adic-valuation-basic: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  lem-divisors-from-prime-exponents: mathematical-premise
  math:def-coprime: mathematical-premise
  math:def-common-divisor-and-gcd: mathematical-premise
  lem-euler-four-square-count: mathematical-premise
  lem-euler-obstruction-at-dividing-prime: mathematical-premise
  math:thm-rat-ordered-field: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, Completion of the proof of Proposition 3.1, divisor-sum ratio and
        final inequality
dependency_level: 4
---

## Statement

Let $m$ be a positive odd integer and set $n=2m$. A positive integer is greater than $0$. An integer is odd if it has the form $2k+1$ and even if it has the form $2k$, for some integer $k$. Write $d\mid a$ if $a=dq$ for some integer $q$, and $d\nmid a$ if there is no such $q$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Let $p\in\mathcal P_3$ with $p\mid m$, where $\mathcal P_3$ is the set of primes $p$ with $4\mid(p-3)$.

Write $R(n)$ for the number of ordered integer quadruples $(x_1,x_2,x_3,x_4)$ whose squares sum to $n$, including zero and allowing both signs in every position. The count $b_p(n)$ includes precisely those quadruples with one even and one odd entry in each of the pairs $(x_1,x_2)$ and $(x_3,x_4)$ and with both entries of at least one pair divisible by $p$. Each qualifying quadruple counts once.

For a positive integer $a$, let $\sigma(a)$ be the sum of all its positive divisors. Regard counts and sums as nonnegative integers. Let $e=v_p(m)$ be the greatest nonnegative integer $j$ with $p^j\mid m$, where $p^j$ is the product of $j$ copies of $p$ and $p^0=1$. Write $m=p^eu$ with $u$ positive and $p\nmid u$.

Then $R(n)>0$. If $e\ge2$, the exact integer quotient $t=m/p^2$, defined by $m=p^2t$, is positive and
$$\frac{\sigma(m/p^2)}{\sigma(m)}=\frac{p^{e-1}-1}{p^{e+1}-1}<\frac{1}{p^2}.$$
For every such $p$ dividing $m$, the following rational inequalities hold:
$$\frac{b_p(n)}{R(n)}\le\frac{2}{3p^2}\le\frac{2}{p(p-1)}.$$
Here fractions $a/b$ have integer numerator $a$ and nonzero integer denominator $b$. They represent the same rational number when their cross-products agree.

## Statement references

[[math:def-integers]]

[[math:thm-int-ordered-ring]]

[[math:lem-nat-embeds-int]]

[[lem-square-residue-parity]]

[[math:def-divides-in-z]]

[[math:def-prime]]

[[def-euler-prime-classes]]

[[def-euler-four-square-representations]]

[[def-euler-mixed-four-square-representations]]

[[def-euler-prime-obstruction-count]]

[[def-euler-divisor-functions]]

[[math:def-p-adic-valuation]]

[[math:lem-p-adic-valuation-basic]]

[[math:thm-division-algorithm-in-z]]

[[math:def-group-power]]

[[math:def-rationals]]

[[math:def-rat-order]]

## Facts & Assumptions

[F1] The integers have associative and commutative addition and multiplication, distributivity, additive inverses and a total order. Adding the same integer preserves order, and products of positive integers are positive. Identify the natural numbers with exactly the nonnegative integers via the inclusion preserving $0$, $1$, addition, multiplication and order. [[math:thm-int-ordered-ring]] [[math:lem-nat-embeds-int]]

[F2] For division by a positive integer $d$, the expression $a=dq+r$ with integers $q,r$ and $0\le r<d$ exists and is unique. [[math:thm-division-algorithm-in-z]]

[F3] Divisibility is witnessed by an integer multiple. A prime $p$ has $p>1$ and no positive divisor other than $1$ and $p$. Each member of $\mathcal P_3$ is such a prime and satisfies $4\mid(p-3)$. The integers under multiplication form the monoid $(\mathbb Z,\cdot,1)$ by F1. In this monoid $p^0=1$ and $p^{s(j)}=p^jp$ for every natural number $j$, where $s(j)$ denotes its natural successor. In particular $p^1=p$. [[math:def-divides-in-z]] [[math:def-prime]] [[def-euler-prime-classes]] [[math:thm-int-ordered-ring]] [[math:def-semigroup-and-monoid]] [[math:def-group-power]]

[F4] The total count $R(n)$ counts all ordered integer quadruples with square sum $n$. Mixed parity means one even entry and one odd entry in each of the two indicated pairs. The obstruction count $b_p(n)$ additionally requires a pair with both entries divisible by $p$. [[def-euler-four-square-representations]] [[def-euler-mixed-four-square-representations]] [[def-euler-prime-obstruction-count]]

[F5] For a prime $p$ and a nonzero integer $a$, the valuation $v_p(a)$ exists as the greatest nonnegative exponent of a power of $p$ dividing $a$. If $v=v_p(a)$, then $a=p^vw$ for an integer $w$ with $p\nmid w$, and $p^j\mid a$ holds exactly for nonnegative integers $j\le v$. For every nonnegative integer $j$, $p^j\ge1$. [[math:def-p-adic-valuation]] [[math:lem-p-adic-valuation-basic]]

[F6] The divisor sum $\sigma(a)$ adds the positive divisors of a positive integer $a$. The carrier for these sums is the commutative monoid $(\mathbb N,+,0)$. Indeed the nonnegative integers contain $0$ and are closed under addition by F1, so they inherit the commutative monoid laws from integer addition. The inclusion in F1 identifies this operation with natural-number addition. A finite sum in this monoid starts from $0$ and is independent of the order of its terms. The recursion evaluates a nonempty list by adding its last summand to the sum of the preceding list. An appended term changes the length from $j$ to $s(j)$. [[def-euler-divisor-functions]] [[math:thm-int-ordered-ring]] [[math:lem-nat-embeds-int]] [[math:def-semigroup-and-monoid]] [[math:def-finite-sum-in-a-commutative-monoid]] [[math:def-monoid-finite-product]]

[F7] For a prime $p$ and a nonnegative integer $k$, the positive divisors of $p^k$ are $p^j$ for $0\le j\le k$, each occurring once, including the case $k=0$ with sole divisor $1$. Thus $\sigma(p^k)=\sum_{j=0}^k p^j$. If positive integers $a,b$ are coprime, meaning their greatest common divisor is $1$, then $\sigma(ab)=\sigma(a)\sigma(b)$. The greatest common divisor is the greatest integer that divides both. [[lem-divisors-from-prime-exponents]] [[math:def-coprime]] [[math:def-common-divisor-and-gcd]]

[F8] If $m>0$ and $2\nmid m$, the total count at $n=2m$ is $R(n)=24\sigma(m)$. [[lem-euler-four-square-count]]

[F9] For $m>0$ of the form $2k+1$, $n=2m$ and $p\in\mathcal P_3$ dividing $m$, the obstruction count is $0$ when $p^2\nmid m$ and $16\sigma(m/p^2)$ when $p^2\mid m$. [[lem-euler-obstruction-at-dividing-prime]]

[F10] A fraction $a/b$ with integers $a,b$ and $b\ne0$ represents a rational number. For positive denominators $b,d$, the comparison of $a/b$ with $c/d$ uses the same relation as the comparison of $ad$ with $cb$, for each of $=$, $<$ and $\le$. The rational order is well defined and total. [[math:def-rationals]] [[math:def-rat-order]] [[math:thm-rat-ordered-field]]

[F11] A property of natural numbers holds for all of them if it holds at $0$ and its truth at each $k$ implies its truth at $s(k)$. [[math:thm-induction-principle]]

[F12] For natural numbers $j,k$, if $j<k$ then $s(j)\le k$. [[math:lem-nat-discrete]]

[F13] Write $s(k)$ for the natural successor and $1=s(0)$. The recursion for natural addition gives $k+0=k$ and $k+s(0)=s(k+0)$, so $s(k)=k+1$. Under the identification in F1 this is addition by the integer $1$, since the inclusion preserves addition and $1$. [[math:def-nat-addition]] [[math:lem-nat-embeds-int]]

## Proof

**Given:** A positive odd integer $m$, $n=2m$, and $p\in\mathcal P_3$ with $p\mid m$.

**Goal:** Show that the ratios are defined in their stated ranges and establish the divisor-sum identity and both bounds on $b_p(n)/R(n)$.

1.1 The expression $m=2k+1$ has remainder $1$ upon division by $2$. Uniqueness of the remainder rules out an expression $m=2q$ with remainder $0$, so $2\nmid m$. For every positive integer $a$, F1 identifies $a$ with a positive natural number. Since $a=1\cdot a$, enumerate its positive divisors starting with $1$. In the recursion of F6 the first partial sum is $1$, and each additional summand is positive, so the final sum is at least $1$. We use the integer images of these sums, with addition, multiplication and order preserved by F1. Hence $R(n)=24\sigma(m)>0$. [given, F1, F2, F3, F4, F6, F8]

1.2 Apply F5 to the prime $p$ and the nonzero integer $m$. It gives $e\ge1$ because $p^1=p\mid m$, and gives $m=p^eu$ with $p\nmid u$. Both $p^e$ and $p^2$ are positive. If $u=0$ then $m=0$, and if $u<0$ then $-m=p^e(-u)>0$. Thus $u>0$. Also $p^2\mid m$ holds exactly when $e\ge2$. In that case $e-2$ and $e-1$ are nonnegative integer differences, hence natural indices by F1. Since $(e-2)+1=e-1$ and $(e-1)+1=e$ in the integers, F13 gives $s(e-2)=e-1$ and $s(e-1)=e$ for the natural indices. Two applications of the power recursion give $m=p^2p^{e-2}u$. Applying F2 with divisor $p^2$ and remainder $0$ gives the unique quotient $t=m/p^2=p^{e-2}u>0$. [given, F1, F2, F3, F5, F13]

2.1 For any nonnegative integer $k$, a positive common divisor of $p^k$ and $u$ equals $p^j$ for some $0\le j\le k$. If $j>0$, then $j\ge s(0)=1$ by F12 and F13. Thus $j-1$ is a natural index by F1, and $(j-1)+1=j$ in the integers gives $s(j-1)=j$ by F13. The power recursion gives $p^j=p\,p^{j-1}$. An integer multiple of $p^j$ is then a multiple of $p$, contrary to $p\nmid u$. Only $j=0$ is possible, and $1$ divides both. Thus their greatest common divisor is $1$. When $e\ge2$, both $e$ and $e-2$ are natural indices by F5 and Step 1.2. Apply the coprime product formula first with $k=e$ and then with $k=e-2$ to obtain $\sigma(m)=\sigma(p^e)\sigma(u)$ and $\sigma(t)=\sigma(p^{e-2})\sigma(u)$. Since $\sigma(u)>0$, cross-multiplication gives $\sigma(t)/\sigma(m)=\sigma(p^{e-2})/\sigma(p^e)$. [F1, F3, F6, F7, F10, F12, F13, step 1.1, step 1.2]

3.1 For each natural number $k$, put $S_k=\sum_{j=0}^k p^j=\sigma(p^k)$. Each $p^j$ is positive by F5 and hence has a natural representative by F1. At $k=0$ the index list consists only of $0$. Enumerate in increasing order. By F13, $s(k)=k+1$. By F12 any natural index with $k<j\le k+1$ satisfies $s(k)\le j$ and hence equals $k+1$, so the list for $S_{k+1}$ appends exactly that index to the list for $S_k$. The recursion in $(\mathbb N,+,0)$ gives $S_0=p^0=1$ and $S_{k+1}=S_k+p^{k+1}$. By F1 the same recurrence holds for the integer images used in the following algebra. The identity $(p-1)S_k=p^{k+1}-1$ holds at $k=0$, since $(p-1)S_0=p-1=p^1-1$. If it holds at $k$, then $s(k+1)=k+2$ by F13, so binary distributivity and the power recursion give $(p-1)S_{k+1}=p^{k+1}-1+(p-1)p^{k+1}=p^{k+2}-1$. Induction proves the identity for every nonnegative integer $k$. The product $(p-1)S_k$ is positive because $p>1$ and $S_k\ge1$. Multiply numerator and denominator of the ratio from Step 2.1 by $p-1$, which preserves the ratio by equality of cross-products. This gives $\sigma(t)/\sigma(m)=(p^{e-1}-1)/(p^{e+1}-1)$. [F1, F3, F5, F6, F7, F10, F11, F12, F13, step 1.1, step 1.2, step 2.1]

4.1 For $e\ge2$, the natural successors of $e-1$ and $e$ are $e$ and $e+1$ by Step 1.2 and F13. Applying the power recursion twice and distributing gives $p^2(p^{e-1}-1)=p^{e+1}-p^2$. Since $p^2-1=(p-1)(p+1)>0$, this cross-product is strictly less than $p^{e+1}-1$. The denominators are positive because $p^{e+1}-1=(p-1)S_e>0$ by Step 3.1 and $p^2>0$ by Step 1.2. Thus the strict inequality of cross-products proves $\sigma(t)/\sigma(m)<1/p^2$. Equivalently, $p^2\sigma(t)<\sigma(m)$. [F1, F3, F10, F13, step 1.1, step 1.2, step 3.1]

5.1 Since $e\ge1$ by Step 1.2, either $e=1$ or $1<e$, in which case F12 and F13 give $e\ge s(1)=2$. If $e=1$, Step 1.2 gives $p^2\nmid m$, so F9 gives $b_p(n)=0$, and hence $b_p(n)/R(n)\le 2/(3p^2)$ by comparison with positive denominators. If $e\ge2$, F9 gives $b_p(n)=16\sigma(t)$. Multiplying $p^2\sigma(t)<\sigma(m)$ by $48>0$ gives $(3p^2)b_p(n)<2R(n)$, since $R(n)=24\sigma(m)$. Thus $b_p(n)/R(n)<2/(3p^2)$ in this case. [given, F1, F4, F8, F9, F10, F12, F13, step 1.1, step 1.2, step 4.1]

6.1 Since $p>1$, both $p(p-1)$ and $3p^2$ are positive. Their difference $3p^2-p(p-1)=2p^2+p$ is positive. Comparing the fractions with numerator $2$ gives $2/(3p^2)\le2/[p(p-1)]$. Together with Step 5.1 this proves the claimed density bound, and Steps 3.1 and 4.1 give the divisor-sum identity and its strict bound. [F1, F3, F10, step 3.1, step 4.1, step 5.1] ∎

---
title: Trial division up to the square root
status: published
research_item: lem-trial-division-primality-bound
dependency_level: 0
---

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)
- [math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots)
- [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules)
- [math:lem-of-square-monotone](https://alphabetamath.cc/item/lem-of-square-monotone)
- [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment)
- [math:thm-int-comm-ring](https://alphabetamath.cc/item/thm-int-comm-ring)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)
- [math:cor-of-one-positive](https://alphabetamath.cc/item/cor-of-one-positive)
- [math:lem-of-add-order](https://alphabetamath.cc/item/lem-of-add-order)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)
- [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)


## Statement

An integer $u>1$ is prime, meaning that its only positive divisors are $1$ and $u$, if and only if no integer $d$ with $2\le d\le\lfloor\sqrt u\rfloor$ divides $u$. Here $d$ divides $u$ when $u=dq$ for an integer $q$. The symbol $\sqrt u$ denotes the nonnegative real number whose square is $u$, and $\lfloor x\rfloor$ denotes the unique integer $m$ with $m\le x<m+1$ for a real number $x$.

For each nonnegative integer $d$, the bound $d\le\lfloor\sqrt u\rfloor$ is equivalent to $d^2\le u$, where $d^2=d\cdot d$. Thus the same test can use the integer cutoff $d\ge2$ and $d^2\le u$.

For any positive real bound $B$, all primes at most $B$ can therefore be listed by finitely many exact divisibility tests.

## Statement references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)

[math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots)

[math:lem-of-square-monotone](https://alphabetamath.cc/item/lem-of-square-monotone)

[math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)

[math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

## Facts & Assumptions

[F1] Use the integers $\mathbb Z$ and real numbers $\mathbb R$ of [math:def-integers](https://alphabetamath.cc/item/def-integers) and [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers). Use integer addition and multiplication from [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) and the canonical orders from [math:def-int-order](https://alphabetamath.cc/item/def-int-order) and [math:def-real-order](https://alphabetamath.cc/item/def-real-order). The inclusion of the integers in the reals factors through the rationals $\mathbb Q$ of [math:def-rationals](https://alphabetamath.cc/item/def-rationals). The two injective maps in [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) and [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) preserve order, sums and products. They send the integer constants $0$ and $1$ to the corresponding real constants under composition. The integers form a commutative ring with identity by [math:thm-int-comm-ring](https://alphabetamath.cc/item/thm-int-comm-ring), so $0+k=k$, $a\cdot1=a$, and $ab=ba$. Distributing $a(0+0)$ gives $a\cdot0=a\cdot0+a\cdot0$, so additive cancellation gives $a\cdot0=0$.

[F2] For $u>1$, the prime condition is equivalent to requiring that every positive divisor of $u$ be $1$ or $u$ by [math:def-prime](https://alphabetamath.cc/item/def-prime). A divisor $d$ of $u$ gives an integer $q$ with $u=dq$, and every such equality gives a divisor by [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z).

[F3] The reals with their canonical order are an ordered field in the sense of [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field). They have the least-upper-bound property by [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete), so they are a complete ordered field in the sense of [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field). Thus [math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots) gives a unique nonnegative real square root for each nonnegative real number.

[F4] Multiplication by a positive real number preserves and reflects strict inequality by [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules). It also preserves weak inequality, since it preserves equality. On nonnegative reals, $x\le y$ is equivalent to $x^2\le y^2$ and $x<y$ is equivalent to $x^2<y^2$ by [math:lem-of-square-monotone](https://alphabetamath.cc/item/lem-of-square-monotone).

[F5] Every real $x$ has a unique integer $m$ with $m\le x<m+1$ by [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part).

[F6] For any integer $v$ and any positive integer $d$, there are unique integers $q,r$ with $v=qd+r$ and $0\le r<d$. The integer $r$ is the remainder and equals zero exactly when $d$ divides $v$ by [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z). In this theorem the zero-remainder case is $v=qd$, which is the same as $v=dq$ by commutativity in [F1].

[F7] The embedding of [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) identifies the natural numbers with the nonnegative integers, preserving order and arithmetic. In the order of [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order), the natural numbers below $n$ form the finite initial segment $I_n=\{t\in\mathbb N:t<n\}$ by [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment). In the natural-number construction of [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers), this is the list of predecessors of $n$, starting at $0$ when $n>0$. By [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality), a set is finite if it can be put in bijection with a natural initial segment, and its cardinality is the size of that segment. In particular, $I_n$ has cardinality $n$ by [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment).

[F8] In the ordered real field of [F3], $0<1$ by [math:cor-of-one-positive](https://alphabetamath.cc/item/cor-of-one-positive). Adding the same real on both sides of a strict inequality preserves it by [math:lem-of-add-order](https://alphabetamath.cc/item/lem-of-add-order).

[F9] The Cartesian product $A\times B$ consists of the ordered pairs $(a,b)$ with $a\in A$ and $b\in B$ by [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product) and [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair). Equality of these pairs is coordinatewise by [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs). If $A$ and $B$ are finite, their product is finite with cardinality the product of their cardinalities by [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule). A subset of a finite set is finite with cardinality at most that of the containing set by [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set), with subsets and separation as in [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset).

## Proof

**Given:** An integer $u>1$ and a positive real bound $B$ for the enumeration.

**Goal:** Prove the stated test for $u$ and show that it yields a finite list of all primes at most $B$.

1.1 Adding an integer $k$ to $0<1$ gives $k<k+1$ by [F1] and [F8], using the order-preserving inclusion into the reals. For any integer $m$, an integer $k$ cannot satisfy $m<k<m+1$. If it did, both $m$ and $k$ would satisfy the floor inequalities for $x=k$, since $k\le k<k+1$. This contradicts uniqueness. It follows that for an integer $k$ and real $x$, $k\le x$ is equivalent to $k\le\lfloor x\rfloor$. One direction uses $\lfloor x\rfloor\le x$. In the other, $k\le x$ and $k>\lfloor x\rfloor$ would put $k$ strictly between $\lfloor x\rfloor$ and $\lfloor x\rfloor+1$. [F1, F3, F5, F8]

2.1 For each nonnegative integer $d$, the floor comparison and the square comparison give $d\le\lfloor\sqrt u\rfloor$ exactly when $d^2\le u$. Multiplying $1<u$ by $u>0$ gives $u<u^2$, so strict comparison of nonnegative squares gives $\sqrt u<u$. As $\lfloor\sqrt u\rfloor\le\sqrt u$, the floor is also strictly less than $u$. [given, F1, F3, F4, F8, step 1.1]

2.2 Set $M=\lfloor B\rfloor$. By step 1.1 the possible primes at most $B$ lie among the integers $2,\ldots,M$. If $M<2$, return the empty list. Otherwise $M+1$ is nonnegative, so it is a natural number under the identification in [F7]. Scan $I_{M+1}$ in increasing order and skip entries below $2$. The integers in this segment satisfy $0\le u<M+1$, which is equivalent to $0\le u\le M$ by step 1.1's consecutive-integer comparison. Thus the scan visits exactly the candidates $2,\ldots,M$ once. [given, F1, F2, F3, F5, F7, step 1.1]

3.1 If $u$ is prime, then every integer $d$ in the test range satisfies $1<d<u$ by step 2.1, so it cannot divide $u$. [F2, step 2.1]

3.2 If $u$ is not prime, it has a positive divisor $a$ distinct from $1$ and $u$. Write $u=ab$ with $b$ an integer. Since $a>0$ and $a\cdot0=0<ab=u$, reflection of strict inequality gives $b>0$. Also $b\ne1$, since $b=1$ would give $a=u$. Both $a$ and $b$ are positive integers different from $1$. Step 1.1 excludes integers strictly between $0$ and $1$ and between $1$ and $2$, so $a,b\ge2$. Let $d$ be the smaller and $e$ the larger of $a,b$, with both equal to $a$ if $a=b$. By commutativity $de=ab=u$, so $d\mid u$. Since $0<d\le e$, $d^2\le de=u$. Step 2.1 puts this divisor in the test range. [given, F1, F2, F3, F4, step 1.1, step 2.1]

4.1 For each candidate $u$, scan $I_u$ under the same identification. Skip entries $d<2$ or $d^2>u$. By step 2.1 the remaining entries are exactly the integers in the trial range, since the floor of the square root is strictly less than $u$. Each test checks whether the remainder on dividing $u$ by $d$ is zero. Each individual scan terminates because it traverses a finite initial segment by [F7]. By steps 3.1 and 3.2 a candidate is prime exactly when no tested remainder is zero. Retaining precisely those candidates gives all the primes at most $B$. [F1, F6, F7, step 2.1, step 2.2, step 3.1, step 3.2]

5.1 When $M<2$ there are no tests. Otherwise every test has a candidate $u$ in $I_{M+1}$ and a divisor $d$ in $I_u$, hence in $I_{M+1}$ since $d<u\le M$. The tested pairs form the subset of $I_{M+1}\times I_{M+1}$ with $2\le u\le M$, $2\le d<u$, and $d^2\le u$. Each pair is tested once because both scans visit each of their entries once. The product rule and the finite-subset bound give at most $(M+1)^2$ tests, since $I_{M+1}$ has cardinality $M+1$. [F1, F7, F9, step 2.2, step 4.1] ∎

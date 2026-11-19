---
id: lem-divisors-from-prime-exponents
kind: lemma
title: Divisor products from prime exponents
status: draft
domain: mathematics
deps:
  - math:thm-fundamental-theorem-of-arithmetic
  - math:def-prime
  - math:def-divides-in-z
  - math:thm-int-ordered-ring
  - math:def-monoid-finite-product
  - math:def-group-power
  - math:thm-generalised-associativity
  - math:def-injection-surjection-bijection
  - math:def-finite-cardinality
  - math:thm-product-rule
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-finite-sum-reindexing-and-fubini
  - math:def-cartesian-product
  - math:def-coprime
  - math:def-common-divisor-and-gcd
  - math:thm-induction-principle
  - math:lem-nat-embeds-int
  - math:def-int-operations
  - math:def-integers
  - math:def-int-order
  - math:def-natural-numbers
  - math:def-nat-addition
  - math:def-nat-order
  - math:lem-nat-order-is-membership
  - math:def-function
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-symmetric-group
  - math:thm-subset-of-a-finite-set
  - math:def-nat-finite-sum-and-product
  - math:thm-well-ordering-principle
  - math:def-inverse-relation-composition-and-restriction
formulation_deps:
  - math:thm-fundamental-theorem-of-arithmetic
  - math:def-prime
  - math:def-divides-in-z
  - math:def-monoid-finite-product
  - math:def-group-power
  - math:def-injection-surjection-bijection
  - math:def-finite-cardinality
  - math:thm-product-rule
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-coprime
  - math:def-common-divisor-and-gcd
  - math:def-integers
  - math:def-int-order
  - math:def-natural-numbers
  - math:def-nat-addition
  - math:def-nat-order
  - math:def-function
  - math:lem-nat-embeds-int
  - math:def-int-operations
argument_deps:
  - math:thm-fundamental-theorem-of-arithmetic
  - math:def-prime
  - math:def-divides-in-z
  - math:thm-int-ordered-ring
  - math:def-monoid-finite-product
  - math:def-group-power
  - math:thm-generalised-associativity
  - math:def-injection-surjection-bijection
  - math:def-finite-cardinality
  - math:thm-product-rule
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-finite-sum-reindexing-and-fubini
  - math:def-cartesian-product
  - math:def-coprime
  - math:def-common-divisor-and-gcd
  - math:thm-induction-principle
  - math:lem-nat-embeds-int
  - math:def-int-operations
  - math:def-integers
  - math:def-int-order
  - math:def-natural-numbers
  - math:def-nat-addition
  - math:def-nat-order
  - math:lem-nat-order-is-membership
  - math:def-function
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-symmetric-group
  - math:thm-subset-of-a-finite-set
  - math:def-nat-finite-sum-and-product
  - math:thm-well-ordering-principle
  - math:def-inverse-relation-composition-and-restriction
dependency_roles:
  math:thm-fundamental-theorem-of-arithmetic: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
  math:def-group-power: mathematical-premise
  math:thm-generalised-associativity: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-product-rule: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:lem-finite-sum-reindexing-and-fubini: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-coprime: mathematical-premise
  math:def-common-divisor-and-gcd: mathematical-premise
  math:thm-induction-principle: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-nat-addition: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:def-function: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
  math:def-symmetric-group: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-nat-finite-sum-and-product: mathematical-premise
  math:thm-well-ordering-principle: mathematical-premise
  math:def-inverse-relation-composition-and-restriction: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $u\in\mathbb Z$ with $u>0$ and write $u=\prod_{i=0}^{r-1}p_i^{e_i}$ as a prime factorization. Here the $p_i$ are distinct primes, meaning integers greater than $1$ whose only positive divisors are $1$ and themselves. The length $r$ and the exponents $e_i$ are natural numbers, with $e_i\ge 1$ equal to the number of copies of $p_i$ in the factorization. In integer arithmetic we identify natural numbers with their images in $\mathbb Z$. Powers with exponent zero and products with no factors both equal $1$. For $u=1$ use $r=0$.

For any positive integer $x$, write $D(x)=\{d\in\mathbb Z:d>0,\ d\mid x\}$ for its positive divisors, where $d\mid x$ means $x=dq$ for some integer $q$. Put $A_i=\{j\in\mathbb N:j\le e_i\}=\{0,\ldots,e_i\}$ for $0\le i<r$. Here a tuple $(j_0,\ldots,j_{r-1})$ is a function on the index set $r=\{0,\ldots,r-1\}$ with value $j_i\in A_i$ at $i$. The map from these tuples to $D(u)$ given by $(j_0,\ldots,j_{r-1})\mapsto\prod_{i=0}^{r-1}p_i^{j_i}$ is a bijection, meaning each divisor occurs for exactly one tuple. With no coordinates there is one tuple, the empty function.

In particular $D(u)$ is finite. Write $\tau(u)=\sum_{d\in D(u)}1$ for the number of positive divisors and $\sigma(u)=\sum_{d\in D(u)}d$ for their sum. Then

$$\tau(u)=\prod_{i=0}^{r-1}(e_i+1),\qquad \sigma(u)=\prod_{i=0}^{r-1}\left(\sum_{j=0}^{e_i}p_i^j\right).$$

Both functions equal $1$ at $u=1$. For coprime positive integers $a,b$, meaning that the greatest integer dividing both is $1$, one has $\tau(ab)=\tau(a)\tau(b)$ and $\sigma(ab)=\sigma(a)\sigma(b)$.

## Statement references

[[math:thm-fundamental-theorem-of-arithmetic]]

[[math:def-prime]]

[[math:def-divides-in-z]]

[[math:def-monoid-finite-product]]

[[math:def-group-power]]

[[math:def-injection-surjection-bijection]]

[[math:def-finite-cardinality]]

[[math:thm-product-rule]]

[[math:def-finite-sum-in-a-commutative-monoid]]

[[math:def-coprime]]

[[math:def-common-divisor-and-gcd]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-natural-numbers]]

[[math:def-nat-addition]]

[[math:def-nat-order]]

[[math:def-function]]

[[math:lem-nat-embeds-int]]

[[math:def-int-operations]]

## Facts & Assumptions

[F1] The fundamental theorem of arithmetic gives a finite list of prime factors for every integer $x\ge 1$, with any two such lists differing only by a permutation. At $x=1$ the only list is the empty list. [[math:thm-fundamental-theorem-of-arithmetic]]

[F2] An integer $p$ is prime when $p>1$ and its only positive divisors are $1$ and $p$. [[math:def-prime]]

[F3] Divisibility $d\mid x$ means $x=dq$ for some integer $q$. [[math:def-divides-in-z]]

[F4] The domain $\mathbb Z$ is the set of integers, with integer order and operations. It is a totally ordered commutative ring with additive identity $0$ and multiplicative identity $1$. Multiplication distributes over addition, and a product of two positive integers is positive. [[math:def-integers]] [[math:def-int-order]] [[math:def-int-operations]] [[math:thm-int-ordered-ring]]

[F5] Finite products start with the empty product $1$ and append one factor at a time. The power $p^k$ is the product of $k$ copies of $p$, by the recursion $p^0=1$ and $p^{k+1}=p^kp$. [[math:def-monoid-finite-product]] [[math:def-group-power]]

[F6] Integer products can be split, regrouped, and reordered without changing their value. [[math:thm-generalised-associativity]]

[F7] A bijection is one-to-one and onto. A set is finite if it can be put in bijection with an initial segment $\{0,\ldots,n-1\}$, which then has the same number of elements, $n$, as the set. [[math:def-injection-surjection-bijection]] [[math:def-finite-cardinality]]

[F8] A finite list of finite sets has a finite set of coordinate choices whose number of elements is the product of their numbers of elements. The empty list has one choice, the empty tuple. [[math:thm-product-rule]]

[F9] A finite sum adds the terms in any enumeration of its index set, starting from $0$. Sums are unchanged under bijective reindexing, and a sum over ordered pairs in $A\times B=\{(a,b):a\in A,\ b\in B\}$ equals the iterated sum over the two finite sets $A$ and $B$. [[math:def-finite-sum-in-a-commutative-monoid]] [[math:lem-finite-sum-reindexing-and-fubini]] [[math:def-cartesian-product]]

[F10] Two integers are coprime when their greatest common divisor is $1$. For two positive integers the greatest common divisor is the greatest integer that divides both. [[math:def-coprime]] [[math:def-common-divisor-and-gcd]]

[F11] Induction on a nonnegative integer proves a property by showing it at $0$ and showing that it passes from $s$ to $s+1$. [[math:thm-induction-principle]]

[F12] Natural numbers are identified with the nonnegative integers by the embedding preserving order, addition and multiplication, with the natural numeral $1$ sent to the integer $1$. [[math:lem-nat-embeds-int]] [[math:def-int-operations]]

[F13] The von Neumann naturals have $0=\varnothing$, successor $n+1=n\cup\{n\}$, and $1=\{0\}$. [[math:def-natural-numbers]] [[math:def-nat-addition]]

[F14] For naturals $m,n$, one has $m\le n$ exactly when $m+h=n$ for some natural $h$, and also exactly when $m\subseteq n$. One has $m<n$ exactly when $m\in n$, and $m<n+1$ exactly when $m\le n$. If $n\ne 0$, then $0\in n$. [[math:def-nat-order]] [[math:lem-nat-order-is-membership]]

[F15] A function from $A$ to $B$ assigns exactly one value in $B$ to each element of $A$. The tuples of length $s$ in the product rule are functions on the initial segment $s$ with the indicated coordinate values. [[math:def-function]] [[math:thm-product-rule]]

[F16] Two ordered pairs are equal exactly when their first entries agree and their second entries agree. [[math:thm-the-characterising-property-of-ordered-pairs]]

[F17] A permutation of a set is a bijection from the set to itself. [[math:def-symmetric-group]]

[F18] A finite product of natural numbers has initial value one and multiplies by the next factor at each successor. [[math:def-nat-finite-sum-and-product]]

[F19] A subset of a finite set is finite and has at most as many elements as the original set. A proper subset has strictly fewer elements. [[math:thm-subset-of-a-finite-set]]

[F20] Every nonempty subset of $\mathbb N$ has a least element in the natural order. [[math:thm-well-ordering-principle]]

[F21] For a function $f$ and a subset $A$ of its domain, the restriction $f|_A$ consists of the pairs $(a,f(a))$ for $a\in A$. [[math:def-inverse-relation-composition-and-restriction]]

## Proof

**Given:** A positive integer $u$ with its prime factorization as in the Statement. For the last claim, positive integers $a,b$ with greatest common divisor $1$.

**Goal:** Prove the divisor bijection, the two product formulas, and the normalization and coprime identities.

1.1 Let $x$ be a positive integer. Write $x=\iota(k)$ for a natural $k$, where $\iota(n)=[(n,0)]$ is the natural embedding. Since $\iota(0)=0$, one has $k\ne 0$. Hence $0\in k$ and $1=\{0\}\subseteq k$, so $1\le k$ in $\mathbb N$. Order preservation and $\iota(1)=1$ give $x\ge 1$ in $\mathbb Z$, as required for the prime-list factorization in [F1]. [F1, F4, F12, F13, F14]

1.2 For any two prime lists $b,c$ with the same product, the fundamental theorem gives the same length $m$ and a permutation $\pi$ with $c_t=b_{\pi(t)}$ for every position $t$. Fix a prime $p$ and set $C_p=\{t\in m:c_t=p\}$ and $B_p=\{v\in m:b_v=p\}$. The equality $c_t=b_{\pi(t)}$ gives $t\in C_p$ exactly when $\pi(t)\in B_p$. Thus $\pi|_{C_p}$ maps into $B_p$ and is injective. Every $v\in B_p$ has a preimage under $\pi$, and the same equivalence places that preimage in $C_p$. So $\pi|_{C_p}$ is a bijection onto $B_p$. These subsets of $m$ are finite and have the same cardinality. An absent prime has zero occurrences. [F1, F7, F15, F17, F19, F21]

2.1 Take a prime list for a positive integer using step 1.1. Its positions are an initial segment of the naturals. If any positions remain unlisted, take the least remaining position and list all remaining positions carrying its prime, each time taking the least unlisted position with that prime. Repeat with the next least remaining position until all positions are listed. Each append removes one position from the finite set of unlisted positions, so this process terminates and lists every position exactly once. This gives a permutation grouping the equal primes. Regrouping replaces each nonempty block by the power with exponent equal to its length. Conversely, expanding the powers gives a prime list with the same product. [F1, F5, F6, F7, F13, F14, F15, F17, F19, F20, step 1.1]

3.1 For an allowed tuple $\mathbf j=(j_0,\ldots,j_{r-1})$, each $j_i\in A_i$. Since $j_i\le e_i$, the integer difference $e_i-j_i$ is nonnegative. The embedding identifies it with a unique natural $h_i$ and gives $j_i+h_i=e_i$ in $\mathbb N$. Set $d=\prod_{i=0}^{r-1}p_i^{j_i}$ and $c=\prod_{i=0}^{r-1}p_i^{h_i}$. Both products are positive: $1>0$ because the natural embedding sends $1$ to the nonzero nonnegative integer $1$, and each multiplication is by a positive prime when the powers are expanded. Together the two products contain $e_i$ copies of each $p_i$, so $dc=u$ by regrouping the copies by prime. The product gives a unique value $d$ for each tuple and takes values in $D(u)$. [given, F2, F3, F4, F5, F6, F12, F14, F15, step 2.1]

3.2 For $d\in D(u)$ take an integer $c$ with $dc=u$. It has $c>0$: if $c=0$ then $dc=0$, and if $c<0$ then $d(-c)>0$ and $dc=-d(-c)<0$. Apply the prime-list factorization to $d$ and $c$. Their concatenated list has product $u$. Comparing the concatenation with the given list for $u$ shows that all its primes are among the $p_i$ and that their multiplicities are $e_i$. The occurrences of $p_i$ from the list for $d$ form a subset of its occurrences in the concatenation, so their number $j_i$ is at most $e_i$. Grouping the list for $d$ gives the asserted product for this tuple. [given, F3, F4, F6, F19, step 2.1, step 1.2]

4.1 If two allowed tuples give the same integer, comparison of their prime lists gives equality of their exponents coordinate by coordinate. Together with the preceding two steps this establishes the bijection. A natural $j$ belongs to $A_i$ exactly when $j\le e_i$, or equivalently $j<e_i+1$. By the membership characterization of natural order, $A_i$ is the von Neumann natural $e_i+1$, so has cardinality $e_i+1$. Thus the product rule and the bijection give a finite divisor set with $\prod_{i=0}^{r-1}(e_i+1)$ elements. [F5, F7, F8, F13, F14, F15, step 1.2, step 3.1, step 3.2]

5.1 The finite sum defining $\tau(u)$ adds one $1$ for each element of $D(u)$. Adding $1$ that many times gives its number of elements, using the identification of naturals with nonnegative integers. The embedding sends the natural product in step 4.1 to the integer product of the images of its factors, since it preserves $1$ and multiplication at every step of the product recursion. This is the claimed product for $\tau(u)$. [F5, F7, F9, F12, F18, step 4.1]

5.2 Reindex the sum defining $\sigma(u)$ by the divisor bijection. For $0\le s\le r$, let $E_s$ be the set of functions on $s$ with value $j_i\in A_i$ at each $i<s$, and put $S_s=\sum_{\mathbf j\in E_s}\prod_{i=0}^{s-1}p_i^{j_i}$. These sums are finite by the product rule. The reindexing gives $\sigma(u)=S_r$. Since $E_0$ consists of the empty tuple, $S_0=1$. [F5, F8, F9, F15, step 4.1]

6.1 For $s<r$, a pair $(f,k)\in E_s\times A_s$ determines unique entries $f,k$. Extend $f$ to $s+1=s\cup\{s\}$ by assigning $k$ at $s$. The result belongs to $E_{s+1}$. Conversely, for $g\in E_{s+1}$, the restriction $g|_s$ lies in $E_s$ because its values are $g(i)$ for $i\in s$. Since $g(s)\in A_s$, the pair $(g|_s,g(s))$ lies in $E_s\times A_s$. The maps undo each other, because they recover the original two entries and preserve every value on $s+1$. Reindex by this bijection and sum first over $E_s$. For fixed $k$, multiplication by $p_s^k$ can be pulled outside that inner sum: it sends the empty sum $0$ to $0$ and distributes across each addition, so induction on the number of summands proves the identity. Pulling out the fixed factor $S_s$ in the resulting sum over $k$ in the same way gives $S_{s+1}=S_s\sum_{k=0}^{e_s}p_s^k$. [F4, F5, F7, F9, F11, F13, F14, F15, F16, F21, step 5.2]

7.1 At $s=0$ the identity $S_s=\prod_{i=0}^{s-1}\bigl(\sum_{k=0}^{e_i}p_i^k\bigr)$ holds because $S_0=1$ and the product is empty. If it holds at $s<r$, the recurrence appends the next factor and yields it at $s+1$. Induction up to $r$ and $\sigma(u)=S_r$ give the claimed product for $\sigma(u)$. [F5, F11, step 5.2, step 6.1]

8.1 Factor the coprime positive integers $a$ and $b$. If a prime occurred in both lists, removing one copy from each would exhibit a common divisor greater than $1$, contrary to coprimality. Their lists of prime bases are therefore disjoint. Joining them with their exponents gives a factorization of the positive integer $ab$ into powers of distinct primes. The divisor count and sum formulas for $ab$ therefore split at the cut between the lists, giving $\tau(ab)=\tau(a)\tau(b)$ and $\sigma(ab)=\sigma(a)\sigma(b)$. [given, F2, F3, F4, F5, F6, F10, step 2.1, step 5.1, step 7.1]

9.1 At $u=1$ both products have no factors and give $1$. The bijection and the two product formulas, with the coprime identities, establish all the conclusions. [given, F5, step 4.1, step 5.1, step 7.1, step 8.1] ∎

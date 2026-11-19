---
title: Arithmetic, Counting, and Finite Sieves
description: Develop the divisor and square-representation counts, residue
  estimates, and finite sieve identities used in the analytic bound and
  certificate.
status: published
dependency_level: 0
---

**Purpose:** Develop the divisor and square-representation counts, residue estimates, and finite sieve identities used in the analytic bound and certificate.

## Divisor products from prime exponents

[Open item](item-lem-divisors-from-prime-exponents) · level 0


### Statement

Let $u\in\mathbb Z$ with $u>0$ and write $u=\prod_{i=0}^{r-1}p_i^{e_i}$ as a prime factorization. Here the $p_i$ are distinct primes, meaning integers greater than $1$ whose only positive divisors are $1$ and themselves. The length $r$ and the exponents $e_i$ are natural numbers, with $e_i\ge 1$ equal to the number of copies of $p_i$ in the factorization. In integer arithmetic we identify natural numbers with their images in $\mathbb Z$. Powers with exponent zero and products with no factors both equal $1$. For $u=1$ use $r=0$.

For any positive integer $x$, write $D(x)=\{d\in\mathbb Z:d>0,\ d\mid x\}$ for its positive divisors, where $d\mid x$ means $x=dq$ for some integer $q$. Put $A_i=\{j\in\mathbb N:j\le e_i\}=\{0,\ldots,e_i\}$ for $0\le i<r$. Here a tuple $(j_0,\ldots,j_{r-1})$ is a function on the index set $r=\{0,\ldots,r-1\}$ with value $j_i\in A_i$ at $i$. The map from these tuples to $D(u)$ given by $(j_0,\ldots,j_{r-1})\mapsto\prod_{i=0}^{r-1}p_i^{j_i}$ is a bijection, meaning each divisor occurs for exactly one tuple. With no coordinates there is one tuple, the empty function.

In particular $D(u)$ is finite. Write $\tau(u)=\sum_{d\in D(u)}1$ for the number of positive divisors and $\sigma(u)=\sum_{d\in D(u)}d$ for their sum. Then

$$\tau(u)=\prod_{i=0}^{r-1}(e_i+1),\qquad \sigma(u)=\prod_{i=0}^{r-1}\left(\sum_{j=0}^{e_i}p_i^j\right).$$

Both functions equal $1$ at $u=1$. For coprime positive integers $a,b$, meaning that the greatest integer dividing both is $1$, one has $\tau(ab)=\tau(a)\tau(b)$ and $\sigma(ab)=\sigma(a)\sigma(b)$.

### Statement references

[math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)

[math:def-group-power](https://alphabetamath.cc/item/def-group-power)

[math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)

[math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)

[math:def-coprime](https://alphabetamath.cc/item/def-coprime)

[math:def-common-divisor-and-gcd](https://alphabetamath.cc/item/def-common-divisor-and-gcd)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:def-function](https://alphabetamath.cc/item/def-function)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

### Facts & Assumptions

[F1] The fundamental theorem of arithmetic gives a finite list of prime factors for every integer $x\ge 1$, with any two such lists differing only by a permutation. At $x=1$ the only list is the empty list. [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)

[F2] An integer $p$ is prime when $p>1$ and its only positive divisors are $1$ and $p$. [math:def-prime](https://alphabetamath.cc/item/def-prime)

[F3] Divisibility $d\mid x$ means $x=dq$ for some integer $q$. [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[F4] The domain $\mathbb Z$ is the set of integers, with integer order and operations. It is a totally ordered commutative ring with additive identity $0$ and multiplicative identity $1$. Multiplication distributes over addition, and a product of two positive integers is positive. [math:def-integers](https://alphabetamath.cc/item/def-integers) [math:def-int-order](https://alphabetamath.cc/item/def-int-order) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[F5] Finite products start with the empty product $1$ and append one factor at a time. The power $p^k$ is the product of $k$ copies of $p$, by the recursion $p^0=1$ and $p^{k+1}=p^kp$. [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:def-group-power](https://alphabetamath.cc/item/def-group-power)

[F6] Integer products can be split, regrouped, and reordered without changing their value. [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)

[F7] A bijection is one-to-one and onto. A set is finite if it can be put in bijection with an initial segment $\{0,\ldots,n-1\}$, which then has the same number of elements, $n$, as the set. [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F8] A finite list of finite sets has a finite set of coordinate choices whose number of elements is the product of their numbers of elements. The empty list has one choice, the empty tuple. [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)

[F9] A finite sum adds the terms in any enumeration of its index set, starting from $0$. Sums are unchanged under bijective reindexing, and a sum over ordered pairs in $A\times B=\{(a,b):a\in A,\ b\in B\}$ equals the iterated sum over the two finite sets $A$ and $B$. [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid) [math:lem-finite-sum-reindexing-and-fubini](https://alphabetamath.cc/item/lem-finite-sum-reindexing-and-fubini) [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)

[F10] Two integers are coprime when their greatest common divisor is $1$. For two positive integers the greatest common divisor is the greatest integer that divides both. [math:def-coprime](https://alphabetamath.cc/item/def-coprime) [math:def-common-divisor-and-gcd](https://alphabetamath.cc/item/def-common-divisor-and-gcd)

[F11] Induction on a nonnegative integer proves a property by showing it at $0$ and showing that it passes from $s$ to $s+1$. [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F12] Natural numbers are identified with the nonnegative integers by the embedding preserving order, addition and multiplication, with the natural numeral $1$ sent to the integer $1$. [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[F13] The von Neumann naturals have $0=\varnothing$, successor $n+1=n\cup\{n\}$, and $1=\{0\}$. [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)

[F14] For naturals $m,n$, one has $m\le n$ exactly when $m+h=n$ for some natural $h$, and also exactly when $m\subseteq n$. One has $m<n$ exactly when $m\in n$, and $m<n+1$ exactly when $m\le n$. If $n\ne 0$, then $0\in n$. [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)

[F15] A function from $A$ to $B$ assigns exactly one value in $B$ to each element of $A$. The tuples of length $s$ in the product rule are functions on the initial segment $s$ with the indicated coordinate values. [math:def-function](https://alphabetamath.cc/item/def-function) [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)

[F16] Two ordered pairs are equal exactly when their first entries agree and their second entries agree. [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)

[F17] A permutation of a set is a bijection from the set to itself. [math:def-symmetric-group](https://alphabetamath.cc/item/def-symmetric-group)

[F18] A finite product of natural numbers has initial value one and multiplies by the next factor at each successor. [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product)

[F19] A subset of a finite set is finite and has at most as many elements as the original set. A proper subset has strictly fewer elements. [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)

[F20] Every nonempty subset of $\mathbb N$ has a least element in the natural order. [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)

[F21] For a function $f$ and a subset $A$ of its domain, the restriction $f|_A$ consists of the pairs $(a,f(a))$ for $a\in A$. [math:def-inverse-relation-composition-and-restriction](https://alphabetamath.cc/item/def-inverse-relation-composition-and-restriction)

### Proof

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


## Odd prime multiplicities modulo four

[Open item](item-lem-odd-prime-factor-parity) · level 0


### Statement

Let $u$ be a positive odd integer, meaning $u>0$ and $2$ does not divide $u$. Write $u=\prod_{i<m}p_i$ as a product of primes, allowing repetitions and using the empty product $1$ when $u=1$. Index the list by the natural number $m$ viewed as the set of its predecessors, which is empty for $m=0$. Let $S=\{i\in m:p_i\equiv3\pmod4\}$ and let $k=|S|$, the finite cardinality of $S$. This counts each such prime with its multiplicity, the number of times it occurs. Write $(-1)^k$ for the product of $k$ copies of $-1$. Then $u\equiv(-1)^k\pmod4$.

If $u\equiv1\pmod4$, the count $k$, viewed as a nonnegative integer, is even, meaning divisible by $2$. If in addition $u$ has a prime divisor congruent to $3$ modulo $4$, it has one at most $\sqrt{u}$, the unique nonnegative real number whose square is $u$, using the usual embedding of the integers in the reals.

### Statement references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)

[math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)

[math:def-function](https://alphabetamath.cc/item/def-function)

[math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:thm-reals-cauchy-complete](https://alphabetamath.cc/item/thm-reals-cauchy-complete)

[math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots)

### Facts & Assumptions

[F1] An integer $d$ divides $a$ when $a=dq$ for some integer $q$ ([math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)). A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself ([math:def-prime](https://alphabetamath.cc/item/def-prime)).

[F2] Congruence $a\equiv b\pmod n$ means $a-b=nq$ for some integer $q$ ([math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)). For an integer $a$ and a positive integer $b$, the quotient $q$ and remainder $r$ satisfying $a=bq+r$ and $0\le r<b$ are unique and exist ([math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

[F3] The integers form a commutative ring ([math:def-ring](https://alphabetamath.cc/item/def-ring)) with a total order preserved by addition and with positive elements closed under multiplication ([math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)). The natural-number embedding $\iota(n)=[(n,0)]$ is injective, preserves addition and multiplication, preserves and reflects order, and has image exactly the nonnegative integers ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)). No natural number lies strictly between a natural number and its successor ([math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)).

[F4] Every integer at least $1$ is a finite product of primes, and any two such lists for that integer differ only by a permutation ([math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)). A permutation of the index set $m$ is a bijection $m\to m$ ([math:def-symmetric-group](https://alphabetamath.cc/item/def-symmetric-group), [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)).

[F5] A finite product in a monoid starts at its identity and multiplies by the next factor at each extension of the list ([math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)). Finite products in a monoid can be split at a given length or regrouped using nondecreasing natural-number endpoints starting at $0$. In a commutative monoid they can also be reordered without changing their value ([math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)). Integer multiplication is associative and commutative with identity $1$ by [F3], so it defines a commutative monoid ([math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)).

[F6] If two pairs of integers are congruent modulo the same modulus, their respective products are also congruent ([math:lem-congruence-respects-integer-arithmetic](https://alphabetamath.cc/item/lem-congruence-respects-integer-arithmetic)). Induction establishes a property on the natural numbers by proving it at $0$ and showing that it passes from $j$ to $j+1$ ([math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)).

[F7] The real numbers form a complete ordered field ([math:thm-reals-cauchy-complete](https://alphabetamath.cc/item/thm-reals-cauchy-complete)), meaning a field ([math:def-field](https://alphabetamath.cc/item/def-field)) with an order as in [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field) in which every nonempty bounded-above subset has a least upper bound ([math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)). In such a field every nonnegative number has a unique nonnegative square root ([math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots)).

[F8] The embeddings of the integers into the rationals ([math:def-rationals](https://alphabetamath.cc/item/def-rationals)) and of the rationals into the reals preserve order and multiplication ([math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat), [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)). In an ordered field ([math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)), if $a,b$ are nonnegative and $a^2\le b^2$, then $a\le b$ ([math:lem-of-square-monotone](https://alphabetamath.cc/item/lem-of-square-monotone)).

[F9] Separating a membership condition from a given set defines a subset of that set ([math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)). Every natural number $m$ viewed as its set of predecessors is finite with cardinality $m$ ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)). A subset of a finite set is finite ([math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)). A finite set has cardinality zero exactly when it is empty. If $|S|=k$, there is a bijection from $k$ to $S$, and a bijection between finite sets preserves their cardinality ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)). A bijection is an injective and surjective function ([math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)).

[F10] For natural numbers $i,n$ in the von Neumann model, $i<n$ is equivalent to $i\in n$, and $i\le n$ is equivalent to $i\subseteq n$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers), [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order), [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)). The successor is $\sigma(n)=n\cup\{n\}$, with $n\notin n$ and $n<\sigma(n)$. In particular, the natural number $2$ is $\{0,1\}$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)).

[F11] A function $f:A\to B$ assigns each input in its domain $A$ exactly one value in its codomain $B$ ([math:def-function](https://alphabetamath.cc/item/def-function)).

[F12] An ordered pair $(a,b)$ is the set $\{\{a\},\{a,b\}\}$ ([math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)), and equality of ordered pairs is coordinatewise ([math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)). The singleton $\{x\}$ has just the member $x$ ([math:def-unordered-pair-and-singleton](https://alphabetamath.cc/item/def-unordered-pair-and-singleton)). The binary union $A\cup B$ is the union of $\{A,B\}$ ([math:def-union-of-a-set-and-binary-union](https://alphabetamath.cc/item/def-union-of-a-set-and-binary-union)) and its members are exactly the elements belonging to $A$ or to $B$ ([math:lem-unions-and-intersections-of-small-families](https://alphabetamath.cc/item/lem-unions-and-intersections-of-small-families)). The Cartesian product $A\times B$ is the set of ordered pairs with first entry in $A$ and second entry in $B$ ([math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)).

[F13] For natural $a,b$, addition satisfies $a+0=a$ and $a+\sigma(b)=\sigma(a+b)$ ([math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)). Multiplication satisfies $a\cdot0=0$ and $a\cdot\sigma(b)=a\cdot b+a$ ([math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication)). The numerals $1$ and $2$ are $\sigma(0)$ and $\sigma(1)$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)). The embedding $\iota$ sends the natural $0$ and $1$ to the integer $0=[(0,0)]$ and $1=[(1,0)]$ ([math:def-int-operations](https://alphabetamath.cc/item/def-int-operations), [F3]). Since $1+1=2$ in the naturals by the addition recursion, it also sends $2$ to the integer $2$ by preservation of addition.

### Proof

**Given:** A positive integer $u$ with $2\nmid u$.

**Goal:** Prove the product congruence, the evenness of $k$ when $u\equiv1\pmod4$, and the square-root bound when a prime divisor congruent to $3$ modulo $4$ exists.

1.1 By prime factorization, take $u=\prod_{i<m}p_i$. The set $S$ is a subset of the finite index set $m$, so it is finite and its cardinality $k$ is a natural number. For another prime list $p'_i$ for $u$, uniqueness gives the same length and a permutation $\pi$ of $m$ with $p'_i=p_{\pi(i)}$. Let $S'=\{i\in m:p'_i\equiv3\pmod4\}$, a finite subset of $m$. Then $i\in S'$ exactly when $i\in m$ and $\pi(i)\in S$. Separate from the graph of $\pi$ exactly the pairs with first entry in $S'$. This gives a function from $S'$ to $S$ because each $i\in S'$ has exactly one value $\pi(i)$ and that value belongs to $S$. The restriction is injective because $\pi$ is injective. It is onto $S$ because the preimage of each element of $S$ under $\pi$ belongs to $S'$. The two counts therefore agree. Each entry divides $u$ by moving it to the front and taking the product of the remaining entries. Conversely, if a prime $p$ divides $u$, write $u=pv$ with $v$ an integer. Since $p>1$ and $u>0$, $v$ must be positive: $v=0$ would give $u=0$ and $v<0$ would give $-u=p(-v)>0$. As a positive integer, $v\ge1$. Factoring $v$ and adjoining $p$ gives a prime list for $u$, so uniqueness forces $p$ to occur in the chosen list. [given, F1, F2, F3, F4, F5, F9, F11, F12]

2.1 Divide each $p_i$ by $4$ to get $p_i=4a_i+r_i$ with $r_i\in\{0,1,2,3\}$. If $r_i=0$ or $2$, write $r_i=2e$ with $e=0$ or $1$. Then $p_i=2(2a_i+e)$, and step 1.1 gives $u=p_i v$ for some integer $v$. Thus $u=2((2a_i+e)v)$, contradicting $2\nmid u$. Hence $r_i=1$ or $3$. Form the sign list by separating from $m\times\{-1,1\}$ the pairs $(i,1)$ for $r_i=1$ and $(i,-1)$ for $r_i=3$. The unique remainder at each $i\in m$ supplies exactly one value $s_i$. In both cases $p_i\equiv s_i\pmod4$, using $p_i+1=4(a_i+1)$ in the second case. By uniqueness of the remainder, the positions with $r_i=3$ are exactly those with $p_i\equiv3\pmod4$. [given, F1, F2, F3, F9, F11, F12, step 1.1]

3.1 Compare the products of the first $j$ terms of the prime list and the sign list by induction, asserting congruence modulo $4$ whenever $j\le m$. For $j=0$ both products equal $1$. If $\sigma(j)\le m$, then $j<m$ and $j\in m$ by [F10], so the induction hypothesis applies and the entries $p_j$ and $s_j$ are defined. Multiply the two products by those respective entries. The next products are congruent by the multiplication rule and the congruence of the next factors. At $j=m$ this gives $u\equiv\prod_{i<m}s_i\pmod4$. [F2, F3, F5, F6, F10, step 1.1, step 2.1]

4.1 For $j\le m$ let $S_j=\{i\in S:i\in j\}$ and $k_j=|S_j|$, which exists because $S_j$ is a subset of the finite set $S$. We show by induction that the product of the first $j$ signs is $(-1)^{k_j}$ whenever $j\le m$. At $j=0$, the count is zero and the product is $1$. If $\sigma(j)\le m$, then $j<m$ and the induction hypothesis applies at $j$. Since $\sigma(j)=j\cup\{j\}$ and $j\notin j$, the only possible new qualifying position is $j$. If $j\notin S$, then $S_{\sigma(j)}=S_j$ and the next sign is $1$, so both the count and product stay the same. If $j\in S$, then $S_{\sigma(j)}=S_j\cup\{j\}$. Choose a bijection $f:k_j\to S_j$ and take the graph $g=f\cup\{(k_j,j)\}$. The old graph supplies the unique pair at each input in $k_j$. The new pair has first coordinate $k_j\notin k_j$, so it supplies exactly one value at the new input. Thus $g$ is a function from $\sigma(k_j)=k_j\cup\{k_j\}$ to $S_{\sigma(j)}$. The old inputs map bijectively to $S_j$, and the new input maps to $j\notin S_j$, so $g$ is a bijection. Thus $k_{\sigma(j)}=\sigma(k_j)$ by uniqueness of finite cardinality. The next sign is $-1$, so the sign product appends one copy of $-1$ and is $(-1)^{k_{\sigma(j)}}$ by the product recursion. At $j=m$ we have $S_m=S$, so the full sign product is $(-1)^k$ and the congruence is $u\equiv(-1)^k\pmod4$. [F3, F5, F6, F9, F10, F11, F12, step 1.1, step 2.1, step 3.1]

5.1 Suppose $u\equiv1\pmod4$. The congruence in step 4.1 makes it enough to evaluate $(-1)^k$. Divide the nonnegative integer image of $k$ by $2$ to write $\iota(k)=2t+r$ with $r=0$ or $1$. If $t<0$, then $-t$ is a positive integer and hence at least $1$ by natural-number discreteness at $0$ and the order embedding. Thus $2t+r\le-1$, contrary to $\iota(k)\ge0$. Take natural numbers $T$ and $R$ with $\iota(T)=t$ and $\iota(R)=r$. Here $R$ is the natural $0$ or $1$. The embedding preserves addition and multiplication and sends the natural $2$ to the integer $2$, so injectivity transports the length identity to $k=2T+R$ in the naturals. [F2, F3, F10, F13, step 4.1]

6.1 The graph $\mathbb{N}\times\{-1\}$ defines the constant sequence of signs. Take the block endpoints $b_j=2j$ in the naturals. Multiplication recursion gives $b_0=0$ and $b_{\sigma(j)}=b_j+2$, hence the endpoints are nondecreasing by the definition of natural-number order. Each block has length $2$ and its two factors multiply to $1$. Regrouping through endpoint $b_T$ therefore gives a product of $T$ copies of $1$, which equals $1$ by induction using the product recursion. Split the full product at $b_T=2T$. Its remaining length is $R$, so its remaining product is $1$ if $R=0$ and $-1$ if $R=1$. Consequently $(-1)^k=1$ or $-1$, respectively. [F3, F5, F6, F10, F11, F12, F13, step 5.1]

7.1 If $R=1$, the congruence from step 4.1 gives $u\equiv-1\pmod4$. Together with $u\equiv1\pmod4$ this yields $u=4a+1=4b-1$ for integers $a,b$, so $2=4(b-a)$. This contradicts uniqueness of the remainder on division of $2$ by $4$: the quotient $0$ gives remainder $2$, whereas $b-a$ would give remainder $0$. Thus $R=0$ and $\iota(k)=2t$, so $k$ is even in the stated sense. [F1, F2, F3, step 4.1, step 5.1, step 6.1]

8.1 Continue to assume $u\equiv1\pmod4$ and suppose a prime divisor of $u$ is congruent to $3$ modulo $4$. It appears in the list, so $k>0$. By step 7.1, $\iota(k)=2t$. Since $\iota(k)>0$, the integer $t$ is positive, so $t\ge1$ and $\iota(k)\ge2$. By the definition of $k=|S|$, there is a bijection from the natural ordinal $k$ to $S$. By [F3], the integer inequality $\iota(k)\ge2$ gives $2\le k$ in the natural-number order. By [F10], $2=\{0,1\}\subseteq k$, so $0$ and $1$ belong to the domain and their images are distinct positions in $S$. Let $p$ and $q$ be their prime values, labeled so that $p\le q$. The values can coincide. Reorder the factors to write $u=pqc$, where $c$ is the product of the remaining primes. Starting with $1$, each multiplication by a prime preserves positivity, so induction gives $c>0$. Since $c$ is an integer, $c\ge1$. The differences $pq-p^2=p(q-p)$ and $pqc-pq=pq(c-1)$ are nonnegative. Thus $p^2\le pq\le u$. [F1, F2, F3, F5, F6, F9, F10, F13, step 1.1, step 7.1]

9.1 The integer-to-real embeddings preserve products and order, so the images of $p$ and $u$ are positive and still satisfy $p^2\le u$. By completeness of the real ordered field, $u$ has a nonnegative real square root and $(\sqrt{u})^2=u$. Both $p$ and $\sqrt{u}$ are nonnegative in the real ordered field, so $p^2\le(\sqrt{u})^2$ gives $p\le\sqrt{u}$. The selected $p$ is a prime divisor congruent to $3$ modulo $4$, which completes the bound and the proof. [F7, F8, step 1.1, step 8.1] ∎


## Square residues and opposite parity

[Open item](item-lem-square-residue-parity) · level 0


### Statement

Write $\mathbb Z$ for the integers and $z^2$ for $z\cdot z$. An integer $z$ is **even** if $z=2k$ for some integer $k$ and **odd** if $z=2k+1$ for some integer $k$. Two integers have **opposite parity** if one is even and the other is odd, and the **same parity** if both are even or both are odd.

An integer $d$ divides an integer $z$ if $z=dq$ for some integer $q$. It is a common divisor of $x$ and $y$ if it divides each. An integer $z$ is positive if $0<z$. Congruence $a\equiv b\pmod m$ means that $m$ divides $a-b$.

Every integer is either even or odd, and the two cases are mutually exclusive. For every integer $z$, one has $z^2\equiv0\pmod4$ if $z$ is even and $z^2\equiv1\pmod4$ if $z$ is odd. If $x$ and $y$ have opposite parity, then $x^2+y^2$ is positive, odd, and congruent to $1$ modulo $4$. If a positive odd integer $d$ divides both $x$ and $y$, each of $x$ and $y$ has the same parity as its exact integer quotient by $d$.

### Statement references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

### Justification

Division with remainder by $2$ makes the even and odd conditions exhaustive and disjoint, as Steps 1.1 and 2.1 show. The same-parity and opposite-parity conditions therefore specify whether the two unique remainders are equal or different. For a positive divisor, the exact integer quotient is the unique quotient with remainder zero.

### Facts & Assumptions

[F1] In the integer construction, $[(a,b)]$ denotes the class of the natural-number pair $(a,b)$, with $(a,b)$ and $(c,d)$ in the same class when $a+d=b+c$ ([math:def-integers](https://alphabetamath.cc/item/def-integers)). Integer arithmetic uses the defined addition and multiplication with $0=[(0,0)]$ and $1=[(1,0)]$ ([math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)). Use the numerals $2=1+1$ and $4=2\cdot2$. The strict integer order is $a<b$ when $a\le b$ and $a\ne b$ ([math:def-int-order](https://alphabetamath.cc/item/def-int-order)).

[F2] Integer addition and multiplication satisfy the commutative ring laws, including distributivity and the additive and multiplicative identity laws. The order is total, addition preserves inequalities, and the product of positive integers is positive ([math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)).

[F3] An integer multiple $z=dq$ is equivalent to $d$ dividing $z$ ([math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)). An equality $a-b=mq$ with integer $q$ is equivalent to $a\equiv b\pmod m$ ([math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)).

[F4] For any integer $z$ and positive integer $b$, there exist unique integers $q,r$ with $z=bq+r$ and $0\le r<b$ ([math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

[F5] The map $\iota(n)=[(n,0)]$ from the natural numbers to the integers is injective and additive. It preserves and reflects the non-strict order, using the additive order on its domain ([math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)). Its image consists of the nonnegative integers ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)).

[F6] The natural numbers $0,1,2$ are respectively $\varnothing,\{0\},\{0,1\}$, with successor $\sigma(n)=n\cup\{n\}$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)). For natural numbers $m,n$, the additive order $m\le n$ means $m+k=n$ for some natural number $k$, and $m<n$ means $m\le n$ and $m\ne n$ ([math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)). For natural numbers $m,n$, one has $m<n$ exactly when $m\in n$ ([math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)).

[F7] Natural number addition has the rules $m+0=m$ and $m+\sigma(n)=\sigma(m+n)$ ([math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)).

### Proof

**Given:** Arbitrary integers $z,x,y$. For the square sum assume $x$ and $y$ have opposite parity. For the division claim assume $d$ is a positive odd integer dividing both $x$ and $y$.

**Goal:** Show that every integer has exactly one parity, determine the square of $z$ modulo $4$ from its parity, establish the three properties of the opposite-parity square sum, and show that the exact quotients by $d$ retain the original parities.

1.1 In the natural numbers $1+1=\sigma(1+0)=\sigma(1)=2$. The map $\iota$ sends natural $0,1$ to integer $0,1$ by the formulas in F1 and F5, and sends natural $2=1+1$ to integer $2=1+1$ by additivity. By injectivity and preservation and reflection of $\le$, the map $\iota$ preserves and reflects $<$ as defined in F1 and F6. The natural inequalities $0<1<2$ follow from $0\in1$ and $1\in2$, so they hold for the integer numerals as well. If $r$ is an integer with $0\le r<2$, write $r=\iota(n)$ for a natural number $n$. Then $n<2$, hence $n\in\{0,1\}$, and thus $r=0$ or $r=1$. [F1, F5, F6, F7]

2.1 Apply division with remainder by $2$ to an arbitrary integer $z$. Step 1.1 gives the two possible remainders $0$ and $1$, and both are in the permitted range. The representation $z=2q+r$ therefore identifies $z$ as even when $r=0$ and odd when $r=1$. The two forms are mutually exclusive by uniqueness of the remainder. In particular $0$ is even because $0=2\cdot0$. [F2, F4, step 1.1]

3.1 If $z=2q$, then $z^2=4q^2$, so $z^2\equiv0\pmod4$. If $z=2q+1$, then $z^2=4(q^2+q)+1$, so $z^2\equiv1\pmod4$. The displayed multiples of $4$ give the required divisibility witnesses for the two congruences. [F1, F2, F3, step 2.1]

3.2 If an integer $w$ is zero, then $w^2=0$. Otherwise totality and addition of $-w$ to the inequality $w<0$ when needed give that either $w$ or $-w$ is positive. The square of that positive integer is positive and equals $w^2$ because $(-w)^2=w^2$. Thus both squares in $x^2+y^2$ are nonnegative, and the odd coordinate has positive square because zero is even. Adding the nonnegative square to the positive square leaves a positive sum by compatibility of order with addition. [F1, F2, step 2.1]

3.3 Write $d=2a+1$ and let $w=2b+r$ be any integer with its remainder $r$ from Step 2.1. Then $dw=(2a+1)(2b+r)=2((2a+1)b+ar)+r$. Since $0\le r<2$, uniqueness of the remainder in division by $2$ gives the same remainder for $dw$ and $w$. Thus multiplication by $d$ preserves the parity of every integer. [F2, F4, step 2.1]

4.1 For $x,y$ of opposite parity, Step 3.1 writes the even coordinate's square as $4A$ and the odd coordinate's square as $4B+1$ for integers $A,B$. Their sum is $4(A+B)+1=2(2(A+B))+1$. The first expression shows congruence to $1$ modulo $4$, and the second shows oddness. [F1, F2, F3, step 3.1]

4.2 Because $d$ divides $x$ and $y$, there are integers $u,v$ with $x=du$ and $y=dv$. Since $d>0$, these are the unique quotients with remainder zero in division by $d$. Applying Step 3.3 to $u$ and to $v$ proves that $x$ has the parity of $u$ and $y$ has the parity of $v$. [F3, F4, step 3.3]

5.1 Each integer has exactly one parity. The square congruences, the positivity, oddness and congruence of the opposite-parity square sum, and the parity of each exact quotient follow from the preceding steps. [step 2.1, step 3.1, step 4.1, step 3.2, step 4.2] ∎


## Jacobi’s signed, ordered four-square count

[Open item](item-thm-jacobi-signed-ordered-four-square-count) · level 0


### Statement

For a positive integer $u$ (so $u>0$), let $\mathcal R_4(u)$ be the set of ordered quadruples of integers with square sum $u$. Here $\mathbb Z^4$ denotes $(\mathbb Z\times\mathbb Z)\times(\mathbb Z\times\mathbb Z)$, where $\mathbb Z$ is the set of integers and $(x_1,x_2,x_3,x_4)$ denotes the ordered pair $((x_1,x_2),(x_3,x_4))$.
$$\mathcal R_4(u)=\{(x_1,x_2,x_3,x_4)\in\mathbb Z^4:x_1^2+x_2^2+x_3^2+x_4^2=u\}.$$
Two quadruples are equal exactly when they agree at every position, by applying the equality rule for ordered pairs to the outer pair and to the two inner pairs. Each distinct quadruple is counted once. Zero and both signs of a nonzero integer are allowed in every coordinate.

Let $v_2(u)$ be the greatest natural number $k$ for which $2^k\mid u$, with $0\in\mathbb N$. Write $u_{\mathrm{odd}}=u/2^{v_2(u)}$ for the odd part of $u$. For a positive integer $m$, let $D(m)=\{d\in\mathbb Z:d>0,\ d\mid m\}$, where $d\mid m$ means $m=dq$ for some integer $q$. The finite sum $\sum_{d\mid m}d$ adds each element of $D(m)$ once.

The operations in the formula are integer operations. Powers use natural exponents. Write $\iota:\mathbb N\to\mathbb Z$ for the usual embedding. In $(-1)^u$, the exponent means the unique natural $n$ with $\iota(n)=u$. The natural cardinality $|\mathcal R_4(u)|$ is read as its image under $\iota$ in the equality below. Then the number of elements of $\mathcal R_4(u)$ is
$$|\mathcal R_4(u)|=8\bigl(2+(-1)^u\bigr)\sum_{d\mid u_{\mathrm{odd}}}d.$$

### Statement references

[Integers](https://alphabetamath.cc/item/def-integers)

[Positivity in the integers](https://alphabetamath.cc/item/def-int-order)

[Integer operations](https://alphabetamath.cc/item/def-int-operations)

[Cartesian product](https://alphabetamath.cc/item/def-cartesian-product)

[Ordered pair](https://alphabetamath.cc/item/def-ordered-pair)

[Equality of ordered pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)

[Separation notation](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[Representation as a sum of four integer squares](https://alphabetamath.cc/item/def-sum-of-four-squares-representation)

[Natural numbers](https://alphabetamath.cc/item/def-natural-numbers)

[Order on the natural numbers](https://alphabetamath.cc/item/def-nat-order)

[Exponent of the largest dividing prime power](https://alphabetamath.cc/item/def-p-adic-valuation)

[Powers with nonnegative exponents](https://alphabetamath.cc/item/def-group-power)

[Integer divisibility](https://alphabetamath.cc/item/def-divides-in-z)

[Sum indexed by a finite set](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)

[Function with a declared domain and codomain](https://alphabetamath.cc/item/def-function)

[Embedding of the natural numbers into the integers](https://alphabetamath.cc/item/lem-nat-embeds-int)

[Number of elements of a finite set](https://alphabetamath.cc/item/def-finite-cardinality)

### Justification

The ordered-ring laws for integers give the commutative monoids $(\mathbb Z,\cdot,1)$ and $(\mathbb Z,+,0)$ used for powers and sums, respectively. [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

Every positive integer is at least $1$. Indeed, it is the image of a positive natural number under the order-preserving embedding, and $1$ is the immediate successor of $0$ in the natural order. Likewise, the only integers in the interval from $1$ to $2$ are its endpoints, since $2$ is the immediate successor of $1$ in the natural order. [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)

For an integer $B\ge 0$, let $I_B=\{y\in\mathbb Z:0\le y\le B\}$, formed by separation in $\mathbb Z$. Write $B=\iota(b)$ for the unique natural $b$ given by the embedding. Let $\operatorname{succ}(b)=b\cup\{b\}$ be its natural successor. The natural numbers $j\le b$ are precisely the elements of $\operatorname{succ}(b)$ by the identification of the natural order with membership. [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) [math:def-int-order](https://alphabetamath.cc/item/def-int-order) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)

Define $f$ by restricting the graph of $\iota$ to first coordinates in $\operatorname{succ}(b)$. The restriction has domain $\operatorname{succ}(b)$ and is single valued because $\iota$ is a function on all of $\mathbb N$. For every $j\in\operatorname{succ}(b)$, order preservation gives $0\le\iota(j)\le B$, so $f:\operatorname{succ}(b)\to I_B$. [math:def-function](https://alphabetamath.cc/item/def-function) [math:def-inverse-relation-composition-and-restriction](https://alphabetamath.cc/item/def-inverse-relation-composition-and-restriction) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

Injectivity of $\iota$ makes $f$ injective. For $y\in I_B$, the description of the image of $\iota$ gives $y=\iota(j)$ for a natural $j$. Since $y\le B=\iota(b)$ and $\iota$ reflects order, $j\le b$, hence $j\in\operatorname{succ}(b)$ and $f(j)=y$. Thus $f$ is surjective, making $I_B$ finite. [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

In any tuple in $\mathcal R_4(u)$, each square is nonnegative, since a negative integer has the same square as its positive opposite, and a product of positive integers is positive. Thus each $x_i^2$ is at most $u$. If $x_i>u$, then $x_i>u\ge1$ gives $x_i(x_i-1)\ge0$, so $x_i^2\ge x_i>u$. If $x_i<-u$, the same inequality for $-x_i$ gives $x_i^2>u$. Hence each coordinate lies in $J=\{x\in\mathbb Z:-u\le x\le u\}$. [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

Define $T:J\to I_{2u}$ by $T(x)=x+u$ and $S:I_{2u}\to J$ by $S(y)=y-u$. Addition preserves the order, so $0\le x+u\le 2u$ for $x\in J$ and $-u\le y-u\le u$ for $y\in I_{2u}$. Form the graphs by separation in $J\times I_{2u}$ and $I_{2u}\times J$, respectively, keeping the pairs with the stated second coordinate. The bounds and the single value of each integer expression make these graphs functions of the declared types. [math:def-function](https://alphabetamath.cc/item/def-function) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product) [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

The ring laws give $T(S(y))=y$ for $y\in I_{2u}$ and $S(T(x))=x$ for $x\in J$. The first identity makes $S$ injective, and the second makes it surjective. Transport along $S$ makes $J$ finite. [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

Three applications of the binary finite product rule make $(J\times J)\times(J\times J)$ finite. The square-sum predicate separates $\mathcal R_4(u)$ inside $\mathbb Z^4$, and the coordinate bounds make it a subset of this finite product. It is therefore finite, so its cardinality is defined. [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product) [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule) [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

For $d\in D(m)$, the divisor bound gives $|d|\le |m|$ because $m>0$. Since $d,m>0$, the nonnegative clause of the absolute-value definition gives $|d|=d$ and $|m|=m$. Thus $D(m)$ is formed by separation in $\mathbb Z$ and lies in the finite set $I_m$. The subset theorem makes $D(m)$ finite. In the additive commutative monoid of integers, the finite sum over $D(m)$ has the same value in every enumeration. [math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound) [math:def-int-abs](https://alphabetamath.cc/item/def-int-abs) [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z) [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)

In particular, every positive divisor of $2$ lies between $1$ and $2$. The endpoint property above and $2>1$ show that $2$ is prime. Since $u>0$, the valuation definition therefore gives the greatest exponent $k=v_2(u)$ with $2^k\mid u$. Its existence argument gives $2^k\ge1$. Divisibility supplies an integer $q$ with $2^kq=u$. Since $2^k>0$, multiplication by $2^k$ preserves strict order, so $q$ is positive and unique. This defines $u/2^k$. If $q=2t$ for an integer $t$, the recursion for natural powers gives $u=2^{\operatorname{succ}(k)}t$. Since $\operatorname{succ}(k)>k$, this contradicts the maximality of $k$. Thus the quotient is odd, meaning it is indivisible by $2$. [math:def-prime](https://alphabetamath.cc/item/def-prime) [math:def-p-adic-valuation](https://alphabetamath.cc/item/def-p-adic-valuation) [math:def-group-power](https://alphabetamath.cc/item/def-group-power) [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

### External input

Apply Ewell’s Theorem 1 to the positive integer $n=u$. Reading each ordered quadruple as its pair of ordered pairs gives a bijection with the quadruples counted by his $r_4(u)$. This preserves every coordinate and the square sum, including tuples with zero or negative entries. His exponent $b(u)$ is $v_2(u)$, so $\operatorname{Od}(u)=u/2^{b(u)}$ is $u_{\mathrm{odd}}$. His $\sigma(\operatorname{Od}(u))$ sums precisely the elements of $D(u_{\mathrm{odd}})$. With these identifications and the natural exponent and cardinality conventions above, his formula gives the displayed count.


## Two-square count as a prime-exponent product

[Open item](item-lem-two-square-count-from-prime-exponents) · level 0


### Statement

Let $u$ be a positive integer. Write $r_2(u)$ for the number of ordered integer pairs $(x,y)$ with $x^2+y^2=u$, allowing zero coordinates. Two ordered pairs are equal exactly when their first coordinates agree and their second coordinates agree, so every sign change or coordinate swap that changes a coordinate gives a distinct pair. A prime is an integer greater than $1$ with no positive divisors other than $1$ and itself. For a prime $p$, write $e_p$ for the greatest nonnegative integer $e$ for which $p^e$ divides $u$, meaning $u$ is an integer multiple of $p^e$. Write $p\equiv b\pmod 4$ when $p-b$ is a multiple of $4$. Use the natural numbers as nonnegative exponents, with a zeroth power equal to $1$. An integer is even or odd according as its remainder on division by $2$ is $0$ or $1$.

If some prime $q\equiv3\pmod 4$ has odd $e_q$, then $r_2(u)=0$. Otherwise
$$r_2(u)=4\prod_{\substack{p\equiv1\pmod 4\\ e_p>0}}(e_p+1),$$
where the factors range over the indicated primes in increasing prime order. There are finitely many such primes because each is a prime divisor of $u$, and integer prime factorization has finite support. The product is taken in $\mathbb N$, and $e_p+1$ is the successor of $e_p$. For an integer reading of the equality, identify each natural number with its nonnegative integer image. A product with no factors is $1$.

### Statement references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-two-square-representation-function](https://alphabetamath.cc/item/def-two-square-representation-function)

[math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-p-adic-valuation](https://alphabetamath.cc/item/def-p-adic-valuation)

[math:def-group-power](https://alphabetamath.cc/item/def-group-power)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

[math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)

[math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)

[math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)

[math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)

[math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)

[math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product)

[math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)

[math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

### Facts & Assumptions

[F1] For positive $u$, $r_2(u)$ is the number of ordered pairs $(x,y)$ of integers satisfying $x^2+y^2=u$. Equality of ordered pairs means equality of the corresponding coordinates. [math:def-two-square-representation-function](https://alphabetamath.cc/item/def-two-square-representation-function) [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product) [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair) [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)

[F2] An integer $d$ divides $a$ if $a$ is an integer multiple of $d$. A prime integer is an integer greater than $1$ whose only positive divisors are $1$ and itself. For a prime $p$, $e_p=v_p(u)$ is the greatest nonnegative exponent for which $p^{e_p}$ divides $u$. The relation $p\equiv b\pmod 4$ means that $p-b$ is an integer multiple of $4$. [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z) [math:def-prime](https://alphabetamath.cc/item/def-prime) [math:def-p-adic-valuation](https://alphabetamath.cc/item/def-p-adic-valuation) [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[F3] In a multiplicative monoid a finite product starts at the identity $1$ and multiplies by each factor in turn. A power $a^k$ for a nonnegative integer $k$ is a product of $k$ copies of $a$. In a commutative monoid, rearranging or grouping the factors of a finite product preserves its value. [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:def-group-power](https://alphabetamath.cc/item/def-group-power) [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity) [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)

[F4] Every positive integer is a finite product of prime integers, uniquely up to order. [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)

[F5] For an integer $a$ and a positive integer $b$, division gives unique integers $k,r$ with $a=kb+r$ and $0\le r<b$. The integer $a$ is divisible by $b$ exactly when $r=0$. [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

[F6] The complex field $\mathbb C$ contains $\mathbb R$ and has imaginary unit $i$ with $i^2=-1$. Its elements have unique coordinates $a+bi$ with real $a,b$. Addition is coordinatewise, and $(a+bi)(c+di)=(ac-bd)+(ad+bc)i$. The Gaussian integers are the subset $R=\{a+bi:a,b\in\mathbb Z\}$. For a complex number $z=a+bi$, put $\bar z=a-bi$ and $N(z)=a^2+b^2$. [math:def-complex-numbers-and-arithmetic](https://alphabetamath.cc/item/def-complex-numbers-and-arithmetic) [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

[F7] A ring has associative multiplication with identity $1$, an abelian additive group, and distributivity. In a commutative ring the multiplication is also commutative. A subring contains the ambient identity and is closed under addition, additive inverses, and multiplication. In a field, every nonzero element $b$ has an inverse, and $a/b$ means $ab^{-1}$. A field is a commutative ring with $1\ne0$ and with no zero divisors. A commutative ring with $1\ne0$ and no zero divisors is an integral domain. [math:def-subring](https://alphabetamath.cc/item/def-subring) [math:lem-field-is-a-commutative-ring](https://alphabetamath.cc/item/lem-field-is-a-commutative-ring) [math:def-zero-divisor-and-integral-domain](https://alphabetamath.cc/item/def-zero-divisor-and-integral-domain) [math:def-ring](https://alphabetamath.cc/item/def-ring) [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring) [math:def-field](https://alphabetamath.cc/item/def-field)

[F8] A unit in $R$ is an element with a multiplicative inverse in $R$. In $R$, $g$ divides $h$ when $h=gc$ for some $c\in R$. Two elements are associates when one is a unit times the other. [math:def-invertible-element](https://alphabetamath.cc/item/def-invertible-element) [math:def-divisibility-and-associates-in-a-domain](https://alphabetamath.cc/item/def-divisibility-and-associates-in-a-domain)

[F9] A nonzero nonunit of an integral domain is irreducible if in every factorization of it at least one factor is a unit. It is prime in the domain if whenever it divides a product it divides at least one factor. [math:def-irreducible-and-prime-elements-in-a-domain](https://alphabetamath.cc/item/def-irreducible-and-prime-elements-in-a-domain)

[F10] A nonempty set of natural numbers has a least element. [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)

[F11] A prime integer is a sum of two integer squares exactly when it is $2$ or congruent to $1$ modulo $4$. [math:thm-fermat-two-square-theorem-for-primes](https://alphabetamath.cc/item/thm-fermat-two-square-theorem-for-primes)

[F12] A property of natural numbers holds for every natural number if it holds at $0$ and passes from $k$ to $k+1$. A finite list of nonempty sets admits a choice function on the family of its values. Such a choice function $g$ satisfies $g(S) \in S$ for every set $S$ in that family. [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle) [math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice) [math:def-choice-function](https://alphabetamath.cc/item/def-choice-function)

[F13] The integers are a totally ordered ring with addition, multiplication, and negation. An integer is positive if it is greater than $0$. The natural numbers are $0$ and its successive successors. They embed in the integers as the nonnegative integers, preserving arithmetic and order, and $k+1$ immediately follows $k$ in the natural order. In particular, a positive integer is at least $1$, and an integer greater than $1$ is at least $2$. [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-integers](https://alphabetamath.cc/item/def-integers) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:def-int-order](https://alphabetamath.cc/item/def-int-order) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)

[F14] The fraction $a/b$ for integers $a,b$ with $b\ne0$ denotes the rational represented by $(a,b)$. The embedding $a\mapsto a/1$ preserves integer arithmetic and order. The reals form an ordered field, and the rational embedding into it preserves arithmetic and order and sends $a/b$ with $b>0$ to the quotient of the images of $a$ and $b$. We use these embeddings for rational and integer real coordinates in [F6]. In an ordered field, $a<b$ means that $b-a$ is positive. The inverse of a positive element is positive. Multiplication by a positive element preserves strict inequalities and equality, and a product of two nonnegative elements is nonnegative by the positive product rule and the case of a zero factor. [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field) [math:lem-of-q-embeds](https://alphabetamath.cc/item/lem-of-q-embeds) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field) [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive) [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules)

[F15] A bijection identifies the cardinalities of two finite sets and transports finiteness. Subsets of finite sets are finite. The interval of naturals $0,\ldots,m-1$ has $m$ elements. The Cartesian product of two finite sets and the set of tuples from a finite list of finite sets are finite, with cardinality the product of the respective cardinalities. The product of cardinalities is taken in $\mathbb N$, starting at $1$ and multiplying by each cardinality in list order. The empty list has one tuple. [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment) [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule) [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product)

[F16] Natural addition and multiplication are the recursive operations on $\mathbb N$, with $m+1=\sigma(m)$ and $m\cdot\sigma(n)=m\cdot n+m$. For naturals $m,n$, the relation $m\le n$ means that $m+j=n$ for some natural $j$. When $m\le n$, the natural difference $n-m$ is the unique such $j$. [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product)

### Proof

**Given:** A positive integer $u$ with the count and exponents specified above.

**Goal:** Compute $r_2(u)$ from the exponents $e_p$.

1.1 By [F9] the prime arguments below require an integral domain. The coordinate formulas and coefficient embeddings show that $R$ contains $0,1$ and is closed under addition, additive inverses, and multiplication. It is therefore a subring of $\mathbb C$. The ring laws, commutativity, and $1\ne0$ are inherited from $\mathbb C$. In particular, multiplication on $R$ is associative and commutative with identity $1$, so it is a commutative monoid. A zero product in $R$ is a zero product in $\mathbb C$, so one factor vanishes. Thus $R$ is an integral domain. The unique coordinates make conjugation and the norm well defined. The multiplication formula gives $\overline{zw}=\bar z\bar w$ and $z\bar z=N(z)$, so $N(zw)=N(z)N(w)$ for complex $z,w$. For $z=a+bi\in R$ with $z\ne0$, at least one of $a,b$ is a nonzero integer. Each square is nonnegative, and a nonzero integer square is at least $1$, by integer order and discreteness. Hence $N(z)$ is a positive integer. If $z$ has an inverse in $R$, both norms multiply to $1$, so $N(z)=1$. Conversely, when $N(z)=1$, the inverse is $\bar z\in R$. If $a^2+b^2=1$, exactly one coordinate is nonzero, and it is $1$ or $-1$ by discreteness. This gives precisely the four units $1,-1,i,-i$. [F6, F7, F8, F9, F13, F14, algebra]

1.2 By [F4] write $u$ as a finite list of prime factors. Let $m_p$ be the multiplicity of $p$ in this list, with $m_p=0$ for an absent prime. Regrouping shows that $p^{m_p}$ divides $u$. If $p^{m_p+1}$ divided $u$, its cofactor would be positive, and factoring the cofactor would give a prime list for $u$ with at least $m_p+1$ copies of $p$, contradicting uniqueness. Every higher power is a multiple of $p^{m_p+1}$. Thus $m_p=e_p$, so only finitely many $e_p$ are positive. The integer $2$ is prime because a product of two integers at least $2$ is at least $4$. Every other prime is odd because otherwise $2$ would be a proper divisor. The remainders $0$ and $2$ modulo $4$ would both give divisibility by $2$, so the odd primes have remainder $1$ or $3$ modulo $4$. Let $P$ and $Q$ be the lists of primes with $e_p>0$ in these two respective residue classes. The positive primes in each list correspond to natural numbers by [F13]. Taking the least of the remaining primes by [F10] until the finite list is exhausted puts each list in increasing order. Grouping the prime factors now gives $u=2^{e_2}\prod_{p\in P}p^{e_p}\prod_{q\in Q}q^{e_q}$. [given, F2, F3, F4, F5, F7, F10, F12, F13]

2.1 If $x^2+y^2=u$, each coordinate $c$ satisfies $c^2\le u$. If $c$ lies outside the integer interval $[-u,u]$, one of $c,-c$ equals a positive integer $t>u$. Then $t\ge1$, so $c^2=t^2\ge t>u$, a contradiction. The map $c\mapsto c+u$ is a bijection from this interval to the natural initial segment $0,\ldots,2u$, with inverse $k\mapsto k-u$. The box formed by two copies of the interval is therefore finite by the product rule, and the representation set is a subset of that box. The map $(x,y)\mapsto x+yi$ is injective because equality of the complex numbers forces equality of both coefficients and hence of the ordered pairs. It is onto the elements of $R$ of norm $u$ because every such element has integer coordinates with square sum $u$. Thus $r_2(u)$ is also the cardinality of this norm set. [given, F1, F6, F13, F14, F15, step 1.1]

2.2 For $\alpha,\beta\in R$ with $\beta\ne0$, field division and $\beta\bar\beta=N(\beta)$ give $\alpha/\beta=(\alpha\bar\beta)/N(\beta)$, with rational coordinates and positive integer denominator $b=N(\beta)$. For either coordinate $a/b$, write $a=kb+r$ with $0\le r<b$ using [F5]. If $2r\le b$, choose the integer $k$, giving an error $r/b$ between $0$ and $1/2$. If $2r>b$, choose $k+1$, giving an error $r/b-1$ between $-1/2$ and $0$. For these bounds, multiply $0\le r<b$ by $b^{-1}>0$, and compare $r/b$ with $1/2$ by multiplying the comparison of $2r$ with $b$ by the positive product $2^{-1}b^{-1}$. Translation by $-1$ leaves differences unchanged. With $\lambda\in R$ formed from the two chosen integers, the coordinates $d_1,d_2$ of $\alpha/\beta-\lambda$ lie in $[-1/2,1/2]$. Each satisfies $d_j^2\le1/4$ because $(1/2-d_j)(1/2+d_j)\ge0$. For $\eta=\alpha-\beta\lambda\in R$, the norm identity gives $N(\eta)=N(\beta)(d_1^2+d_2^2)\le N(\beta)/2<N(\beta)$. [F5, F6, F7, F13, F14, step 1.1, construct, algebra]

2.3 Set $\tau=1+i$, which has norm $2$ and satisfies $2=(-i)\tau^2$. For each $p$ in the finite list $P$, the set of integer pairs $(a,b)$ satisfying $p=a^2+b^2$ is nonempty by [F11]. Write $S_p$ for this representation set. Apply finite choice to the list of the $S_p$ in the order of $P$ to obtain a choice function $g$. Set $(a_p,b_p)=g(S_p)$, which belongs to $S_p$ by [F12]. Then $\pi_p=a_p+b_pi$ and $\bar\pi_p$ both have norm $p$ and multiply to $p$. These elements and $\tau$ have prime integer norms and are irreducible, since the norms of two nonunit factors of a nonzero element would both be integers greater than $1$. For $q\in Q$, $N(q)=q^2$. If $q$ were a product of two nonunits in $R$, their norms would both be $q$ by [F4], contradicting [F11] because a norm is a sum of two integer squares. Thus $q$ is irreducible too. [F4, F6, F8, F9, F11, F12, step 1.1, step 1.2]

3.1 Let $\rho$ be irreducible in $R$ and suppose $\rho$ does not divide $a\in R$. Choose a nonzero combination $d=s\rho+ta$ of least norm with $s,t\in R$. Such norms give a nonempty set of naturals under the identification in [F13], since $\rho$ is one such combination. The remainder on dividing either $\rho$ or $a$ by $d$ is another combination of $\rho$ and $a$ and has smaller norm if nonzero. Thus $d$ divides both. If $d$ were a nonunit, irreducibility of $\rho$ would make the other factor of $\rho$ a unit, so $\rho$ would divide $d$ and hence $a$. Therefore $d$ is a unit and multiplying its defining identity by its inverse gives $1=s'\rho+t'a$ with $s',t'\in R$. If $\rho$ divides $ab$ for some $b\in R$, multiplication of this identity by $b$ gives $\rho\mid b$. This proves that every irreducible in $R$ is prime in $R$. [F8, F9, F10, F13, step 1.1, step 2.2]

4.1 The factors $\pi_p,\bar\pi_p$ at a given $p$ are not associates. A multiplier $\pm1$ between them forces one coordinate to vanish, making $p$ the square of an integer of magnitude greater than $1$ and contradicting primality. A multiplier $\pm i$ forces $a_p=\pm b_p$, so $p=2a_p^2$ would be even. Factors at different integer primes have distinct norms, since their norms are positive powers of different primes. Associates have the same norm by multiplicativity and the norm of a unit. Thus $\tau$, each $\pi_p,\bar\pi_p$, and each $q\in Q$ are pairwise nonassociate primes in $R$. [F2, F4, F6, F8, F13, step 1.1, step 1.2, step 3.1, step 2.3]

5.1 If $N(z)=u$, then $z\bar z=u$. By steps 1.2 and 2.3 the right side is a unit times a finite product of the listed primes in $R$. Remove these prime factors one at a time from the equality. The next prime divides the remaining product of the two factors on the $z\bar z$ side, so it divides one of the two factors. Remove one copy from that factor and cancel it on both sides. Cancellation holds for a nonzero $g$ because $gh=gk$ implies $g(h-k)=0$ in the domain $R$, hence $h=k$. When the list is exhausted the remaining product is a unit, so both remaining factors are units. Indeed, if $ab=w$ with $w$ a unit, $bw^{-1}$ and $aw^{-1}$ are inverses of $a$ and $b$, respectively. This finite induction expresses $z$ as a unit times powers of the listed primes. [F3, F7, F8, F9, F12, step 1.1, step 1.2, step 2.3, step 4.1]

6.1 To prove uniqueness with these primes fixed, cancel shared prime copies in two expressions for $z$. If a prime copy remains on one side, its prime divides the opposite unit or an opposite prime factor, by repeated application of the prime property to a finite product. A nonunit cannot divide a unit. If a nonunit divides an irreducible, the quotient must be a unit, making the two associates. Since the residual expressions have no common prime and the primes in the list are pairwise nonassociate, there can be no copies left. The two units then agree as well. [F3, F7, F8, F9, F12, step 1.1, step 4.1, step 5.1]

7.1 Write the expression for $z$ as $z=\varepsilon\tau^a\prod_{p\in P}\pi_p^{s_p}\bar\pi_p^{t_p}\prod_{q\in Q}q^{c_q}$, with nonnegative exponents and a unit $\varepsilon$. By multiplicativity its norm is $2^a\prod_{p\in P}p^{s_p+t_p}\prod_{q\in Q}q^{2c_q}$. Concatenating the two lists of split factors adds their lengths $s_p$ and $t_p$. The $c_q$ copies of a factor of norm $q^2$ contribute two copies of $q$ each, giving $2c_q$ by the multiplication recursion in [F16]. Integer prime factorization identifies this with $u$ exactly when $a=e_2$, $s_p+t_p=e_p$ for each $p\in P$, and $2c_q=e_q$ for each $q\in Q$. Conversely every such choice gives an element of norm $u$, and uniqueness distinguishes all choices, including the four units. The equation $2c_q=e_q$ with $c_q$ nonnegative is solvable exactly when division of $e_q$ by $2$ has remainder zero. Use the integer images in [F13] to apply division. When the remainder is zero, the integer quotient is nonnegative because the dividend is nonnegative and the divisor is positive. It therefore comes from a unique natural $c_q$. For a prime $q\equiv3\pmod 4$ outside $Q$, $e_q=0$. Thus if any such prime has odd exponent, the count is zero. [F2, F3, F4, F5, F7, F13, F16, step 1.1, step 1.2, step 2.1, step 2.3, step 5.1, step 6.1]

8.1 If all the $e_q$ at primes congruent to $3$ modulo $4$ are even, the exponent at $2$ and those at all $q\in Q$ are forced. For each $p\in P$, any natural solution to $s_p+t_p=e_p$ has $s_p\le e_p$ by the definition of natural order in [F16]. Conversely, for each natural $s_p\le e_p$, the bounded difference $t_p=e_p-s_p$ is the unique natural solution by [F16]. By discreteness in [F13], these values of $s_p$ are exactly the naturals less than $e_p+1$, so [F15] gives $e_p+1$ choices. Step 7.1 gives a bijection between the norm set and the Cartesian product of the four units with the set of tuples of these exponent choices in the order of $P$. By the finite product rule the cardinality is the natural number $4\prod_{p\in P}(e_p+1)$. The natural-to-integer embedding sends $1$ to $1$ and preserves multiplication, so it sends the natural product to the corresponding integer product by induction on the number of factors. The empty list of primes contributes one tuple, so in particular $r_2(1)=4$. By step 2.1 this is the claimed count of ordered integer pairs. [F1, F3, F12, F13, F15, F16, step 1.1, step 1.2, step 2.1, step 7.1] ∎


## Equal coordinate-label fibers under permutation

[Open item](item-lem-permutation-fibers-have-equal-size) · level 0


### Statement

Let $I$ be a finite set of coordinate positions. An integer tuple on $I$ is a function $x:I\to\mathbb Z$, where $\mathbb Z$ is the set of integers and $x_i=x(i)$ is the entry at position $i$. A permutation $\pi$ of $I$ is a bijection $I\to I$, meaning every position $j$ has a unique preimage $\pi^{-1}(j)$ with $\pi(\pi^{-1}(j))=j$. Reindexing $x$ by $\pi$ puts the entry $x_{\pi^{-1}(j)}$ at position $j$.

Let $S$ be a finite set of integer tuples on $I$ that is closed under coordinate permutations, meaning that every such reindexing of an element of $S$ belongs to $S$. An integer $a$ is odd if $a=(k+k)+1$ for some $k\in\mathbb Z$. For a subset $D\subseteq I$, let the fiber $F_D$ be the set of tuples $x\in S$ for which $x_i$ is odd exactly at the positions $i\in D$. For all subsets $A,B\subseteq I$ with the same number of elements, the fibers $F_A$ and $F_B$ have equal cardinality.

### Facts & Assumptions

[F1] The [definition of a function](https://alphabetamath.cc/item/def-function) specifies exactly one output in the target set for each input in the domain. Such a function can be specified by its graph, the set of ordered pairs of inputs and their outputs in the [Cartesian product](https://alphabetamath.cc/item/def-cartesian-product) of the two sets.

[F2] A [bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) is a function for which each target element has exactly one preimage. For a bijection, the inverse value at a target element is its unique preimage. A [permutation of a set](https://alphabetamath.cc/item/def-symmetric-group) is a bijection from that set to itself.

[F3] The notation $\mathbb Z$ denotes the [set of integers](https://alphabetamath.cc/item/def-integers). The addition and the constant $1$ in the oddness condition are those of [integer arithmetic](https://alphabetamath.cc/item/def-int-operations).

[F4] A [subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) contains only elements of the given set. Selecting the elements of a set that satisfy a specified condition defines a unique subset.

[F5] A set $X$ is finite if it admits a bijection to some natural number considered as the set of its predecessors. The unique such number is the [finite cardinality](https://alphabetamath.cc/item/def-finite-cardinality) $\lvert X\rvert$. Parts (c) and (d) give transport of finite cardinality along a bijection and existence of a bijection between finite sets of equal cardinality.

[F6] A [subset of a finite set is finite](https://alphabetamath.cc/item/thm-subset-of-a-finite-set).

[F7] By the [sum rule for two finite sets](https://alphabetamath.cc/item/thm-sum-rule), if the finite sets $U,V$ have no common element, then $\lvert U\cup V\rvert=\lvert U\rvert+\lvert V\rvert$.

[F8] [Right cancellation for addition of natural numbers](https://alphabetamath.cc/item/lem-nat-add-cancellative) states that $r+c=s+c$ implies $r=s$ for natural numbers $r,s,c$.

[F9] Clause (iii) of the [binary-union membership lemma](https://alphabetamath.cc/item/lem-unions-and-intersections-of-small-families) gives $z\in U\cup V$ exactly when $z\in U$ or $z\in V$. By the [Axiom of Extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality), two sets with the same elements are equal.

[F10] By the [two-sided inverse theorem](https://alphabetamath.cc/item/thm-a-function-is-a-bijection-exactly-when-it-has-a-two-sided-inverse), the inverse of a bijection $f:U\to V$ is a bijection $f^{-1}:V\to U$ with $f^{-1}(f(u))=u$ for $u\in U$ and $f(f^{-1}(v))=v$ for $v\in V$.

### Proof

**Given:** A finite set $I$, a finite set $S$ of integer tuples on $I$ closed under coordinate permutations, and subsets $A,B\subseteq I$ with $\lvert A\rvert=\lvert B\rvert$.

**Goal:** Prove $\lvert F_A\rvert=\lvert F_B\rvert$.

1.1 For any $D\subseteq I$, each entry $x_i$ of a tuple $x\in S$ is a specified integer. The oddness condition is a predicate on that value, so the condition that it holds exactly at the positions in $D$ selects a unique subset $F_D$ of $S$. This subset is finite because $S$ is finite. [given, F1, F3, F4, F6]

1.2 Write $I\setminus D$ for the subset of positions in $I$ outside $D$. The sets $A,B,I\setminus A,I\setminus B$ are finite because they are subsets of $I$. For $D=A$ and for $D=B$, binary-union membership gives $z\in D\cup(I\setminus D)$ exactly when $z\in D$ or $z\in I\setminus D$. Either alternative implies $z\in I$, and every $z\in I$ lies in one of the two sets by the definition of the complement. Therefore $D\cup(I\setminus D)=I$ by extensionality. The two sets have no common element by the same definition. Thus $\lvert I\setminus A\rvert+\lvert A\rvert=\lvert I\rvert=\lvert I\setminus B\rvert+\lvert B\rvert$. Since $\lvert A\rvert=\lvert B\rvert$, right cancellation gives $\lvert I\setminus A\rvert=\lvert I\setminus B\rvert$. [given, F4, F6, F7, F8, F9]

2.1 Choose bijections $u:A\to B$ and $v:I\setminus A\to I\setminus B$. Define $\pi(i)=u(i)$ for $i\in A$ and $\pi(i)=v(i)$ for $i\in I\setminus A$. These rules give one value for each $i\in I$, so selecting their ordered pairs in $I\times I$ defines a function $\pi:I\to I$. Each $j\in B$ has exactly one preimage under $u$ and none under $v$. Each $j\in I\setminus B$ has exactly one preimage under $v$ and none under $u$. Thus $\pi$ is a permutation, and $\pi^{-1}(j)\in A$ exactly when $j\in B$. [given, F1, F2, F4, F5, step 1.2]

3.1 For $x\in F_A$, let $P_\pi x$ be the tuple with entry $x_{\pi^{-1}(j)}$ at position $j$. Its graph is obtained by selecting in $I\times\mathbb Z$ the pairs with exactly these entries, one for each $j\in I$. By closure, $P_\pi x$ belongs to $S$. Its entry at $j$ is odd exactly when $\pi^{-1}(j)\in A$, equivalently when $j\in B$. Thus $P_\pi x\in F_B$, and the pairs $(x,P_\pi x)$ selected in $F_A\times F_B$ define a function $P_\pi:F_A\to F_B$. [given, F1, F2, F4, step 1.1, step 2.1]

4.1 By the two-sided inverse theorem, $\pi^{-1}$ is a bijection $I\to I$ and hence a permutation of $I$. Its inverse is $\pi$, so reindexing $y\in F_B$ by $\pi^{-1}$ gives the tuple with entry $y_{\pi(i)}$ at position $i$. This tuple belongs to $S$ by closure, and its odd entries occur exactly where $\pi(i)\in B$, which by the construction of $\pi$ is exactly where $i\in A$. Select the graph of this reindexing in $F_B\times F_A$ to define $P_{\pi^{-1}}:F_B\to F_A$. The two reindexings undo each other at every position because $\pi^{-1}(\pi(i))=i$ and $\pi(\pi^{-1}(i))=i$. Since tuples are determined by their entries, every $y\in F_B$ has exactly one preimage under $P_\pi$, namely $P_{\pi^{-1}}y$. Thus $P_\pi:F_A\to F_B$ is a bijection. [given, F1, F2, F4, F10, step 1.1, step 2.1, step 3.1]

5.1 Since $F_A$ is finite and $P_\pi$ is a bijection onto $F_B$, transport of finite cardinality gives $\lvert F_A\rvert=\lvert F_B\rvert$. [F5, step 1.1, step 4.1] ∎


## Counting pairs by bounded fibers

[Open item](item-lem-count-pairs-by-bounded-fibers) · level 0


### Statement

Let $A$ and $B$ be sets and let $S$ be a finite subset of the Cartesian product $A\times B$, the set of ordered pairs $(x,y)$ with $x\in A$ and $y\in B$. Define the first-coordinate image $D$ and, for each $x\in D$, its fiber $S_x$ by
$$D=\{x\in A:\exists y\in B,\ (x,y)\in S\},\qquad S_x=\{(u,v)\in S:u=x\}.$$
Thus $D$ consists of the first coordinates that occur in $S$, and $S_x$ consists of all pairs in $S$ with first coordinate $x$. Both $D$ and each $S_x$ are finite. For a finite set $T$, write $|T|$ for its cardinality, the number of its elements, and interpret it as a real number when comparing it with a real bound.

Let $a,b\in\mathbb R$ be nonnegative, meaning $0\le a$ and $0\le b$. If $|D|\le a$ and $|S_x|\le b$ for every $x\in D$, then $|S|\le ab$.

### Statement references

[Ordered pair](https://alphabetamath.cc/item/def-ordered-pair)

[Equality of ordered pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)

[Cartesian product](https://alphabetamath.cc/item/def-cartesian-product)

[Subset and separation notation](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[Finite cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[Von Neumann natural numbers](https://alphabetamath.cc/item/def-natural-numbers)

[Real numbers](https://alphabetamath.cc/item/def-real-numbers)

[Definition of the real order](https://alphabetamath.cc/item/def-real-order)

[Field multiplication](https://alphabetamath.cc/item/def-field)

[The real numbers as an ordered field](https://alphabetamath.cc/item/thm-reals-ordered-field)

[Natural numbers interpreted in a field](https://alphabetamath.cc/item/def-canonical-natural)

### Justification

The ordered pair $(x,y)$ is $\{\{x\},\{x,y\}\}$, and equality of ordered pairs forces equality of their respective coordinates. Hence the phrase “first coordinate” singles out a unique value for each pair. The defining predicates for $D$ and $S_x$ separate subsets of $A$ and $S$, respectively, so they specify unique sets.

A set $T$ is finite when it admits a bijection with a von Neumann natural number $n\in\mathbb N$, viewed as the set of indices $k<n$. A bijection matches each element on either side with exactly one on the other side. This $n$ is unique and gives $|T|$. Its real interpretation is $\iota(n)=n\cdot1_{\mathbb R}$, given by $\iota(0)=0$ and $\iota(n+1)=\iota(n)+1$.

### Facts & Assumptions

[F1] The first coordinate of a pair is unique by [the ordered-pair equality theorem](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs). [A function](https://alphabetamath.cc/item/def-function) assigns a unique output to each element of its domain. A function is [bijective](https://alphabetamath.cc/item/def-injection-surjection-bijection) when distinct inputs have distinct outputs and every element of its target is an output.

[F2] Write $\mathbb N$ for the [set of von Neumann natural numbers](https://alphabetamath.cc/item/def-natural-numbers). The natural number $m$ satisfies $0\le m$ and is the set of indices $k<m$ by [the identification of natural order with membership](https://alphabetamath.cc/item/lem-nat-order-is-membership). Every nonempty set of natural numbers has a least member by [well-ordering](https://alphabetamath.cc/item/thm-well-ordering-principle). For natural indices, $k<\ell$ means $k\le\ell$ and $k\ne\ell$ by [the definition of natural order](https://alphabetamath.cc/item/def-nat-order). The natural-number order is antisymmetric by [the natural-number linear-order theorem](https://alphabetamath.cc/item/thm-nat-linear-order).

[F3] Every finite set has a unique natural number as its [cardinality](https://alphabetamath.cc/item/def-finite-cardinality). Each natural number is finite by [finite cardinality, clause (a)](https://alphabetamath.cc/item/def-finite-cardinality). Every subset of a finite set is finite by [the finite-subset theorem](https://alphabetamath.cc/item/thm-subset-of-a-finite-set). A bijection from a finite set transports finiteness and preserves cardinality by [finite cardinality, clause (c)](https://alphabetamath.cc/item/def-finite-cardinality).

[F4] For a finite index set and a family of finite sets indexed by it, the sets are pairwise disjoint when no element belongs to two sets with distinct indices. An element belongs to the [indexed union](https://alphabetamath.cc/item/def-indexed-union-and-intersection) if and only if it belongs to at least one member of the family. If the sets are pairwise disjoint, [the sum rule, clause 2](https://alphabetamath.cc/item/thm-sum-rule) gives the size of their union as the natural-number sum of their cardinalities.

[F5] For a finite index set $I$ of size $d$, the [sum over $I$](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set) of a function $q:I\to\mathbb N$ or $q:I\to\mathbb R$ is computed by any bijection $g:d\to I$, adding $q(g(k))$ in order for $k<d$. The [natural-number sum](https://alphabetamath.cc/item/def-nat-finite-sum-and-product) and the [real sum](https://alphabetamath.cc/item/def-finite-sum) start at zero and add one term at each successive index. For a finite list of length $d$, both definitions extend the list by zero at every index $k\ge d$. The [canonical map](https://alphabetamath.cc/item/def-canonical-natural) into the reals sends the natural zero to the real zero, so $\iota(0)=0$. By [the canonical-embedding laws, clauses 6 and 7](https://alphabetamath.cc/item/lem-nat-finite-sum-laws-and-the-canonical-embedding), $\iota$ carries the finite sum of a natural-number sequence to the real sum of its embedded terms and is strictly increasing.

[F6] For real sequences on $\mathbb N$, inequalities between corresponding terms at every index $k<d$ imply the same inequality between the sums of the first $d$ terms, and the sum of the first $d$ terms of the constant sequence with value $b$ is $\iota(d)b$, by [the real finite-sum laws, clauses 4 and 2](https://alphabetamath.cc/item/lem-finite-sum-laws).

[F7] By [the real ordered-field theorem](https://alphabetamath.cc/item/thm-reals-ordered-field), the reals form an [ordered field](https://alphabetamath.cc/item/def-ordered-field) and their order is reflexive and transitive. For the [real order](https://alphabetamath.cc/item/def-real-order), $u<v$ implies $u\le v$. For the [field multiplication](https://alphabetamath.cc/item/def-field), [multiplication of nonnegative inequalities](https://alphabetamath.cc/item/prop-of-multiply-inequalities) gives $uv\le u'v'$ when $0\le u\le u'$ and $0\le v\le v'$.

[F8] The [power set](https://alphabetamath.cc/item/def-power-set) $\mathcal P(S)$ is the set of all subsets of $S$. An [indexed family](https://alphabetamath.cc/item/def-indexed-family) with index set $D$ is a function with domain $D$. [Separation](https://alphabetamath.cc/item/def-subset-and-proper-subset) inside a [Cartesian product](https://alphabetamath.cc/item/def-cartesian-product) gives the subset of pairs satisfying the defining predicate.

[F9] By [extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality), two sets with the same elements are equal.

### Proof

**Given:** $A,B,S,D,S_x$ as in the statement, and nonnegative reals $a,b$ with the stated bounds on $|D|$ and $|S_x|$ once their finiteness is established.

**Goal:** Show that $D$ and the fibers are finite and that $\iota(|S|)\le ab$.

1.1 Let $m=|S|$ and take a bijection $e:m\to S$. By separation, form the set $J$ of indices $k\in m$ for which no earlier index has the same first coordinate as $e(k)$. For any $x\in D$, separate from $m$ the indices whose pairs have first coordinate $x$. This set is nonempty by surjectivity of $e$. Well-ordering gives a least matching index $\ell$, so $\ell\le k$ for every matching index $k$. If a matching index $k$ satisfied $k<\ell$, then $k\le\ell$ and $k\ne\ell$ by the definition of strict order, while $\ell\le k$ and antisymmetry would give $k=\ell$. Thus $\ell$ belongs to $J$. Every other matching index $k$ has $\ell\le k$ and $\ell\ne k$, hence $\ell<k$, so $k$ is excluded from $J$. Separate from $J\times D$ the graph $H=\{(k,x)\in J\times D:e(k)\text{ has first coordinate }x\}$. For each $k\in J$, the pair $e(k)\in S$ has exactly one first coordinate and that coordinate belongs to $D$, so $H$ is a function with domain $J$ and codomain $D$. For each $x\in D$, the least-index argument gives exactly one $k\in J$ with $(k,x)\in H$, making $H$ a bijection. Since $J$ is a subset of the finite set $m$, the set $D$ is finite. [given, F1, F2, F3, F8]

2.1 By separation inside $D\times\mathcal P(S)$, form $G=\{(x,T)\in D\times\mathcal P(S):T=S_x\}$. Each $x\in D$ has exactly one such $T$ because the defining predicate of $S_x$ specifies a unique subset of $S$. Hence $G$ is a function with domain $D$ whose value at $x$ is $S_x$, so $G$ is the indexed family $(S_x)_{x\in D}$. Each fiber $S_x$ is a subset of $S$ and hence finite. Each pair in $S$ belongs to the fiber of its first coordinate, and coordinate uniqueness prevents a pair from belonging to fibers with distinct indices. Every element of any fiber lies in $S$ because $S_x\subseteq S$. By the indexed-union membership criterion, the union of $(S_x)_{x\in D}$ has exactly the same elements as $S$. By extensionality the union equals $S$. [F1, F3, F4, F8, F9, step 1.1]

3.1 By separation in $D\times\mathbb N$, form the graph $K=\{(x,n)\in D\times\mathbb N:n=|S_x|\}$. Each fiber is finite by Step 2.1, so each $x\in D$ has exactly one such $n$ by the definition of finite cardinality. Thus $K$ defines a function $K:D\to\mathbb N$ with $K(x)=|S_x|$. Applying the sum rule to the disjoint family in Step 2.1 gives $|S|=\sum_{x\in D}K(x)$ as an equality of natural numbers. [F1, F2, F3, F4, F5, F8, step 1.1, step 2.1]

4.1 Put $d=|D|$ and take a bijection $g:d\to D$ by the definition of cardinality. Using the zero extension for natural-number sums, set $c_k=K(g(k))$ for $k<d$ and $c_k=0$ for the other natural indices. For $k<d$, the index $k$ belongs to the domain $d$ of $g$, and $g(k)\in D$ belongs to the domain of $K$. For each $k\in\mathbb N$, set $r_k=\iota(c_k)$ and $s_k=b$. Each rule gives a unique value at every natural index, so separation in $\mathbb N\times\mathbb N$ and $\mathbb N\times\mathbb R$ gives the graphs of the three sequences. Enumerating the sum of $K$ in Step 3.1 by $g$ gives $|S|=\sum_{k<d}c_k$ as an equality of natural numbers. [given, F1, F2, F3, F5, F8, step 1.1, step 3.1]

5.1 By the canonical-embedding law, the real image of the natural sum in Step 4.1 is the sum of the first $d$ terms of $r$. For $k<d$, we have $r_k=\iota(K(g(k)))=\iota(|S_{g(k)}|)\le b=s_k$ by the fiber bound. The real sum comparison and constant-sum laws give
$$\iota(|S|)=\sum_{k<d}r_k\le\sum_{k<d}s_k=\iota(d)b.$$
When $d=0$, the sums are empty and have value zero. [given, F5, F6, step 3.1, step 4.1]

6.1 Since $0\le d$ in the natural order, either $d=0$ or $0<d$. In the first case $\iota(d)=\iota(0)=0$. In the second case strict increase gives $0=\iota(0)<\iota(d)$. Thus $0\le\iota(d)$ in the real order. The bound on $|D|$ gives $\iota(d)\le a$, and nonnegativity and reflexivity give $0\le b\le b$. Apply the product inequality to $0\le\iota(d)\le a$ and $0\le b\le b$. It gives $\iota(d)b\le ab$. Real-order transitivity with Step 5.1 gives $\iota(|S|)\le ab$. [given, F2, F5, F7, step 4.1, step 5.1] ∎


## Counting a union of obstructions

[Open item](item-lem-finite-obstruction-cover-bound) · level 0


### Statement

Let $S$ be a finite set. Let $(B_j)_{j\in I}$ be an indexed family, meaning that each index $j$ in the set $I$ is assigned a subset $B_j$ of $S$. Assume only finitely many $B_j$ are nonempty, so $J=\{j\in I:B_j\ne\varnothing\}$ is finite. Write $|A|$ for the number of elements of a finite set $A$. Write $\sum_{j\in I}|B_j|$ for the finite sum $\sum_{j\in J}|B_j|$, with value $0$ when $J$ is empty. Let $U=\bigcup_{j\in I} B_j$ be the set of elements that belong to at least one $B_j$. Then $|U|\le\sum_{j\in I}|B_j|$. If $\sum_{j\in I}|B_j|<|S|$, there is an $x\in S$ that belongs to none of the $B_j$.

### Statement references

[math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)

[math:def-function](https://alphabetamath.cc/item/def-function)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)

[math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

[math:def-indexed-union-and-intersection](https://alphabetamath.cc/item/def-indexed-union-and-intersection)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)

[math:thm-the-empty-set-exists-and-is-unique](https://alphabetamath.cc/item/thm-the-empty-set-exists-and-is-unique)

### Facts & Assumptions

[F1] For a finite set $A$, its cardinality $|A|$ is the unique natural number $n$ for which there is a bijection from $\{0,\ldots,n-1\}$ onto $A$, using the empty set of indices when $n=0$. A bijection from a finite set to another set makes the latter finite and preserves cardinality. Also $|\varnothing|=0$. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F2] A sum of natural numbers over a finite index set is obtained by listing the indices once each and adding the corresponding terms. Its value is independent of the listing, and the empty sum is zero. [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

[F3] Every subset of a finite set is finite and has cardinality at most that of the containing set. [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)

[F4] The Cartesian product $J\times S$ is the set of ordered pairs with first coordinate in $J$ and second coordinate in $S$. The ordered pair $(j,x)$ is $\{\{j\},\{j,x\}\}$, and two ordered pairs are equal exactly when their corresponding coordinates agree. [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product) [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair) [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)

[F5] A map is injective if equal outputs force equal inputs, surjective if every element of its target is an output, and bijective if it has both properties. [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)

[F6] Clause 2 of the sum rule gives the cardinality of the union of a finitely indexed family of pairwise disjoint finite sets as the sum of their cardinalities. Pairwise disjoint means that no element lies in two sets with different indices. [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)

[F7] Every nonempty subset of the natural numbers has a least element, meaning an element no greater than any member of the subset. Such an element is unique because the order is antisymmetric, meaning $a\le b$ and $b\le a$ imply $a=b$. Also $a<b$ means $a\le b$ and $a\ne b$. [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle) [math:thm-nat-linear-order](https://alphabetamath.cc/item/thm-nat-linear-order) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[F8] A subset of a set contains only elements of that set. Separation inside a given set forms its subset of elements satisfying a specified set-theoretic condition. The condition may use parameters and has no free occurrence of the variable for the resulting set. Two sets with the same elements are equal. [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation) [math:def-axiom-of-extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)

[F9] A graph contained in a Cartesian product defines a function from the first factor to the second when it has exactly one output in the second factor for each input in the first. Evaluation gives that unique output. [math:def-function](https://alphabetamath.cc/item/def-function)

[F10] An indexed family is a function with the index set as its domain. Its indexed union is the union of its range, so an element belongs to it exactly when it belongs to a set at some index. The indexed union over an empty index set is empty. [math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family) [math:def-indexed-union-and-intersection](https://alphabetamath.cc/item/def-indexed-union-and-intersection) [math:def-union-of-a-set-and-binary-union](https://alphabetamath.cc/item/def-union-of-a-set-and-binary-union)

[F11] The power set of a set is the set of all its subsets. Write $\mathbb{N}$ for the set of natural numbers. [math:def-power-set](https://alphabetamath.cc/item/def-power-set) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[F12] The symbol $\varnothing$ denotes the unique set with no elements. [math:thm-the-empty-set-exists-and-is-unique](https://alphabetamath.cc/item/thm-the-empty-set-exists-and-is-unique)

### Proof

**Given:** A finite set $S$ and subsets $B_j\subseteq S$ indexed by $I$, with a finite set $J$ of indices at which $B_j$ is nonempty.

**Goal:** Bound the cardinality of $U$ by the sum of the cardinalities of the $B_j$ and find an element outside $U$ when that sum is strictly less than $|S|$.

1.1 The set $J$ is obtained by separating the indices of nonempty sets inside $I$. Keep from the graph of the given family just the pairs whose first coordinate lies in $J$. There is still exactly one output $B_j$ for each $j\in J$, so this defines the restricted family on $J$. Every element of $U$ lies in a nonempty $B_j$, hence lies in a $B_j$ with $j\in J$. Conversely every $B_j$ with $j\in J$ contributes to $U$ because $J\subseteq I$. Thus $U=\bigcup_{j\in J}B_j$. Each $B_j$ and $U$ are subsets of $S$, so they are finite. The unique count $|B_j|$ at each $j\in J$ defines the graph of the summands by separation inside $J\times\mathbb{N}$, so the sum over $J$ is defined. If $J=\varnothing$, then $U=\varnothing$ and both $|U|$ and the sum are zero. [given, F1, F2, F3, F4, F8, F9, F10, F11, F12]

1.2 For $j\in J$, let $D_j=\{(j,x)\in J\times S:x\in B_j\}$, formed by separation inside $J\times S$. Since $B_j\subseteq S$, each $x\in B_j$ has exactly one prescribed value $(j,x)\in D_j$. Keeping those input–output pairs from $B_j\times D_j$ gives the graph of a function from $B_j$ to $D_j$. This map is injective by equality of second coordinates and surjective by the definition of $D_j$. Thus $D_j$ is finite and $|D_j|=|B_j|$. [given, F1, F4, F5, F8, F9]

2.1 To form the indexed family $(D_j)_{j\in J}$, keep from $J\times\mathcal{P}(J\times S)$ the pairs $(j,T)$ for which $T$ consists exactly of the pairs $(j,x)$ with $x\in B_j$. Step 1.2 supplies one such set for each $j$, and equality of sets with the same elements gives uniqueness. Thus the graph defines a family on $J$. Let $D=\bigcup_{j\in J}D_j$. A pair in $D_j$ has first coordinate $j$, so no pair belongs to two sets with different indices. The sum rule gives $D$ finite and $|D|=\sum_{j\in J}|D_j|=\sum_{j\in J}|B_j|$. [given, step 1.2, F2, F4, F6, F8, F9, F10, F11]

3.1 Each pair in $D$ has a unique second coordinate, and that coordinate lies in $U$ by the indexed union rule applied to $D$ and to $U$. Therefore the subset of $D\times U$ that pairs each member of $D$ with its second coordinate is the graph of a function $\pi:D\to U$. It is surjective because every $x\in U$ lies in some $B_j$ with $j\in J$, giving $(j,x)\in D$ with $\pi((j,x))=x$. [step 1.1, step 1.2, step 2.1, F4, F5, F8, F9, F10]

4.1 Fix a bijection $e:\{0,\ldots,|J|-1\}\to J$, with an empty domain when $J$ is empty. For each $x\in U$, separate inside the domain of $e$ the positions $k$ with $x\in B_{e(k)}$. This subset of the natural numbers is nonempty because $x$ is covered by a set with index in $J$ and $e$ is onto $J$. Let $k_x$ be its unique least position. Then $(e(k_x),x)\in D$ is uniquely prescribed for each $x\in U$. Separating these input–output pairs inside $U\times D$ gives a function $h:U\to D$ satisfying $\pi(h(x))=x$ for every $x\in U$. When $U$ is empty the graph has no pairs, so it is $\varnothing$. [given, step 1.1, step 1.2, step 2.1, step 3.1, F1, F4, F5, F7, F8, F9, F10, F12, construct]

5.1 If $h(x)=h(y)$, applying $\pi$ gives $x=y$. Define the image $H$ by separating in $D$ the elements equal to $h(x)$ for some $x\in U$. With codomain $H$ the same function is a bijection from $U$ to $H$. Transporting cardinality along this bijection and applying the finite subset bound to $H\subseteq D$ gives $|U|=|H|\le |D|=\sum_{j\in I}|B_j|$. [step 1.1, step 2.1, step 4.1, F1, F3, F5, F8, F9]

6.1 Suppose $\sum_{j\in I}|B_j|<|S|$. If $U=S$, the bound just proved gives $|S|\le\sum_{j\in I}|B_j|$. Together with the strict inequality this contradicts antisymmetry. Hence $U\ne S$. Since $U\subseteq S$, some $x\in S$ lies outside $U$, for otherwise $U$ and $S$ would have the same elements. By indexed union membership, $x\notin B_j$ for every $j\in I$. [step 1.1, step 5.1, F7, F8, F10] ∎


## Maximum from nonincreasing successive ratios

[Open item](item-lem-positive-sequence-ratio-maximum) · level 0


### Statement

Let $I$ be the set of natural numbers $j$ with $1\le j$. Write $j+1$ for the successor of $j$. A positive real sequence $(a_j)_{j\in I}$ assigns one real number $a_j>0$ to each $j\in I$.

Write $r_j=a_{j+1}/a_j$ for the successive ratios. Assume the ratios are nonincreasing, meaning $r_i\ge r_j$ whenever $i\le j$ in $I$.

Let $k\in I$. Assume $r_k\le1$ and, if $k>1$, also assume $r_{k-1}\ge1$. Here $k-1$ denotes the positive index whose successor is $k$. Then $a_k$ is a maximum, meaning $a_j\le a_k$ for every $j\in I$. If $r_k=1$, the term at $k+1$ also equals $a_k$. If $k>1$ and $r_{k-1}=1$, the term at $k-1$ also equals $a_k$.

### Statement references

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)

[math:def-function](https://alphabetamath.cc/item/def-function)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)

[math:thm-nat-linear-order](https://alphabetamath.cc/item/thm-nat-linear-order)

[math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)

[math:lem-nat-nonzero-is-successor](https://alphabetamath.cc/item/lem-nat-nonzero-is-successor)

### Facts & Assumptions

[F1] In the real order ([math:def-real-order](https://alphabetamath.cc/item/def-real-order)), $x\le y$ means $x=y$ or $y-x>0$. With this order the reals form a totally ordered field ([math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)), so real comparison is reflexive and transitive and the product of two positive elements is positive ([math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)).

[F2] For $y\ne0$, division in a field is $x/y=xy^{-1}$, with $y^{-1}y=1$. Field multiplication is commutative and associative, has identity $1$, and distributes over addition and hence subtraction ([math:def-field](https://alphabetamath.cc/item/def-field)).

[F3] For natural numbers, the successor sends $j$ to $j\cup\{j\}$, denoted here by $j+1$, with $1$ the successor of $0$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)). The order $i\le j$ means $i+d=j$ for some natural $d$, using natural addition ([math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)), and $i<j$ also requires $i\ne j$ ([math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)). This comparison is a total order, so any two indices are comparable, and it is reflexive and transitive ([math:thm-nat-linear-order](https://alphabetamath.cc/item/thm-nat-linear-order)). On the naturals, $i<j$ is equivalent to $i+1\le j$. In particular $j<j+1$ by applying the equivalence with $i=j$ and right endpoint $j+1$ ([math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)). Every nonzero natural is the successor of some natural ([math:lem-nat-nonzero-is-successor](https://alphabetamath.cc/item/lem-nat-nonzero-is-successor)).

[F4] If $P(0)$ holds and for every natural $t$ the truth of $P(t)$ implies that of $P(t+1)$, then $P(t)$ holds for every natural $t$ ([math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)).

### Proof

**Given:** The positive sequence and its nonincreasing ratios, with $r_k\le1$ and $r_{k-1}\ge1$ when $k>1$.

**Goal:** Show that $a_j\le a_k$ for every $j\in I$.

1.1 For $j\in I$, we have $1\le j<j+1$ by the successor rule, so $j+1\in I$ and both terms in the ratio exist. Each ratio $r_j$ is defined because $a_j>0$ implies $a_j\ne0$. For $k>1$, the preceding index is well defined. Because $0<1$ by the successor rule, $k\ne0$, so $k=h+1$ for some natural $h$. If $h<1$, then $k=h+1\le1$, a contradiction. If two predecessors were distinct, the smaller $u$ and larger $v$ would satisfy $u+1\le v<v+1$, so their successors could not coincide. Hence $h=k-1$ is unique and lies in $I$. [given, F1, F2, F3]

1.2 Fix $m,n\in I$ with $m\le n$. Let $\preceq$ mean either $\le$ throughout or $\ge$ throughout on the reals, and suppose $a_i\preceq a_{i+1}$ for all $m\le i<n$. Define $P(t)$ to assert $a_m\preceq a_t$ when $m\le t\le n$, with $P(t)$ true outside that range. Since $0<1\le m$, $P(0)$ holds. Assume $P(t)$. If $t+1$ lies outside the range, $P(t+1)$ holds by definition, and if $t+1=m$, it holds by reflexivity. Otherwise $m<t+1\le n$. If $t<m$, then $t+1\le m$, contrary to $m<t+1$. Hence $m\le t$. As $t<t+1\le n$, this gives $m\le t<n$. By $P(t)$ and the adjacent comparison, $a_m\preceq a_t\preceq a_{t+1}$, which gives $P(t+1)$ by transitivity. By induction, $P(n)$ holds, giving $a_m\preceq a_n$. [F1, F3, F4]

2.1 For real $x\le y$ and $c>0$, we have $cx\le cy$. If $x=y$ the products agree, and if $x<y$ then $cy-cx=c(y-x)>0$ by distributivity and closure of the positive elements under multiplication. Since $a_jr_j=a_{j+1}$ by the inverse law, we can multiply the ratio bounds by $a_j>0$. If $1\le j<k$, then $k>1$ and $j\le k-1$, since $k-1<j$ would imply $k\le j$. Thus $r_j\ge r_{k-1}\ge1$, so $a_j\le a_{j+1}$. If $j\ge k$, then $r_j\le r_k\le1$, so $a_{j+1}\le a_j$. [given, F1, F2, F3, step 1.1]

3.1 If $j<k$, apply the preceding induction argument on $j\le i\le k$ with $\preceq$ meaning $\le$. If $j>k$, apply it on $k\le i\le j$ with $\preceq$ meaning $\ge$. The respective adjacent comparisons come from step 2.1. At $j=k$, equality holds. Thus $a_j\le a_k$ for every $j\in I$. Equality of an adjacent ratio with $1$ gives equal neighboring terms by $a_{i+1}=a_ir_i$, so $r_k=1$ gives a tie at $k+1$, and $r_{k-1}=1$ for $k>1$ gives a tie at $k-1$. [F1, F2, F3, step 1.1, step 2.1, step 1.2] ∎


## Periodicity and jump bounds for residue counts

[Open item](item-lem-periodic-residue-count-discrepancy) · level 0


### Statement

Let $M$ be a positive integer and $D\subseteq\{1,\ldots,M\}$. Identify the integers with their usual copy in the reals, with arithmetic and order preserved. For an integer $k$, write $r_M(k)$ for its residue representative, the unique integer $d$ with $1\le d\le M$ for which $k-d$ is an integer multiple of $M$. Thus $M$ represents residue zero. Write $\#S$ and $|S|$ for the number of elements of a finite set $S$. For real $t\ge0$, define
$$A_D(t)=\#\{k\in\mathbb Z:1\le k\le t,\ r_M(k)\in D\},\qquad E_D(t)=A_D(t)-\frac{|D|}{M}t.$$

Then $M$ is a period of the discrepancy $E_D$, meaning $E_D(t+M)=E_D(t)$ for all $t\ge0$. In $0<t\le M$, its jumps, where the limits from below and above both exist and differ, are exactly the points $d\in D$. For any real $B\ge0$, if the endpoint values $E_D(0)$ and $E_D(M)$ and both one-sided limits at every $d\in D$ have absolute value at most $B$, then $|E_D(t)|\le B$ for all $t\ge0$. Here the absolute value of a real $x$ is $x$ for $x\ge0$ and $-x$ for $x<0$.

### Facts & Assumptions

[F1] Two integers are congruent modulo $M$ when their difference is an integer multiple of $M$ ([Integer congruence](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)).

[F2] Division of an integer $a$ by a positive integer $M$ gives unique integers $q,r$ with $a=qM+r$ and $0\le r<M$ ([Division with remainder](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

[F3] The reals are a totally ordered field, so addition preserves inequalities and multiplication by a positive number preserves their direction ([The ordered field of reals](https://alphabetamath.cc/item/thm-reals-ordered-field), [Ordered field](https://alphabetamath.cc/item/def-ordered-field)). The usual inclusions from integers to rationals and rationals to reals preserve $1$, the arithmetic operations of addition and multiplication, and the order ([Integers in the rationals](https://alphabetamath.cc/item/lem-int-embeds-rat), [Rationals in the reals](https://alphabetamath.cc/item/lem-rat-embeds-dense)).

[F4] Every real $x$ has a unique integer part $\lfloor x\rfloor$, the integer $n$ with $n\le x<n+1$ ([Integer part](https://alphabetamath.cc/item/lem-integer-part)).

[F5] The naturals identify with the nonnegative integers, with the same arithmetic and order ([Naturals in the integers](https://alphabetamath.cc/item/lem-nat-embeds-int)). For a natural $n$, the set $\{j\in\mathbb N:j<n\}$ is finite with $n$ elements ([Finite initial segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment)). Subsets of a finite set are finite ([Subsets of a finite set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)). A one-to-one correspondence, pairing every element of each set with exactly one in the other, transfers finiteness and cardinality ([Finite cardinality](https://alphabetamath.cc/item/def-finite-cardinality)).

[F6] The cardinality of the union of two disjoint finite sets, meaning they have no common element, is the sum of their cardinalities ([Sum rule](https://alphabetamath.cc/item/thm-sum-rule), two-block case).

[F7] Let $f$ be a function on $[0,\infty)$ and let $y>0$. The limit on a specified side requires domain points on that side with $0<|x-y|<\rho$ for every $\rho>0$ ([Limit point](https://alphabetamath.cc/item/def-limit-point-r)). Under this condition, a real $L$ is the left or right limit if for every $\varepsilon>0$ there is $\delta>0$ such that $|f(x)-L|<\varepsilon$ for all domain points with $y-\delta<x<y$, or with $y<x<y+\delta$, respectively. When a limit on either side exists, it is unique ([One-sided limits](https://alphabetamath.cc/item/def-one-sided-limits), [Absolute value](https://alphabetamath.cc/item/def-abs-value)).

[F8] Every nonempty set of nonnegative integers has a least element, an element at most every element of that set ([Well-ordering of the naturals](https://alphabetamath.cc/item/thm-well-ordering-principle), [Naturals in the integers](https://alphabetamath.cc/item/lem-nat-embeds-int)).

[F9] For reals $u,v$, absolute value satisfies $|-u|=|u|$ and $|uv|=|u||v|$ ([Basic properties of absolute value](https://alphabetamath.cc/item/lem-of-abs-value)). The definition gives $|u|=u$ for $u\ge0$ and $|u|=-u$ for $u<0$ ([Absolute value](https://alphabetamath.cc/item/def-abs-value)).

### Proof

**Given:** A positive integer $M$, a set $D\subseteq\{1,\ldots,M\}$, and the functions of the statement.

**Goal:** Establish the period identity and locate the jumps, then deduce the global absolute bound from the indicated values and limits.

1.1 Divide $k-1$ by $M$ to obtain $k-1=qM+r$ with $0\le r<M$. Then $d=r+1$ is in $\{1,\ldots,M\}$ and $k-d=qM$. Conversely, a candidate $d$ with $k-d=qM$ gives remainder $d-1$ in the division of $k-1$. Its uniqueness proves that $r_M(k)$ is well defined. In particular $r_M(j)=j$ for $1\le j\le M$, and $r_M(k)=M$ exactly when $k$ is a multiple of $M$. [F1, F2, F3]

1.2 There is no integer $j$ strictly between any integer $n$ and $n+1$, since both $n$ and $j$ would then be integer parts of $j$. For $t\ge0$, put $n=\lfloor t\rfloor$. If $n<0$, then $n<0\le t<n+1$, contradicting the absence of an integer strictly between $n$ and $n+1$. The integers $1\le k\le t$ are exactly those with $1\le k\le n$. The finite set $\{j\in\mathbb N:j<n\}$ corresponds to these integers by $j\mapsto j+1$ with inverse $k\mapsto k-1$, using the same absence of intervening integers. Hence the set counted by $A_D(t)$ is finite, and taking $t=M$ also shows that $D$ is finite. Put $c=|D|/M\ge0$, which is defined since $M>0$. [F3, F4, F5]

1.3 For each $y>0$ and $\rho>0$, set $h=\min\{y,\rho\}/2$. Then $0<h<y$ and $h<\rho$. The domain points $y-h$ and $y+h$ lie on opposite sides of $y$ at distance $h<\rho$ from it. Thus the limit-point condition in [F7] holds on both sides at every positive argument. [F3, F7]

2.1 Fix $t\ge0$. For each $d\in D$, an integer of the form $k=d+qM$ lies in $t<k\le t+M$ exactly when $q-1\le (t-d)/M<q$. By the integer-part property there is exactly one such $q$, namely $\lfloor (t-d)/M\rfloor+1$. Thus $k\mapsto r_M(k)$ pairs the newly counted integers with $D$ one-to-one. The newly counted set and the set counted by $A_D(t)$ are disjoint and their union is the set counted by $A_D(t+M)$. Hence $A_D(t+M)=A_D(t)+|D|$ and $E_D(t+M)=E_D(t)+|D|-cM=E_D(t)$. [F1, F3, F4, F5, F6, step 1.1, step 1.2]

2.2 For each positive integer $j$, discreteness of the integers from step 1.2 gives $A_D(x)=A_D(j)$ on $j\le x<j+1$. On $j-1<x<j$, the count is constant and equals $A_D(j)-1$ if $r_M(j)\in D$, and $A_D(j)$ otherwise, because only $j$ can be added at $x=j$. In that case the new point forms a set of cardinality one and the disjoint union rule adds one to the count. For either side, let $a$ be its constant count. Then $|E_D(x)-(a-cj)|=|-c(x-j)|=c|x-j|$ on that side. For $\varepsilon>0$, taking $\delta=\varepsilon/(1+c+\varepsilon)$ gives $0<\delta<1$ and $c\delta<\varepsilon$. Step 1.3 supplies the limit-point condition at $j>0$. Hence the right limit is $E_D(j)$ and the left limit is $E_D(j)-1$ if $r_M(j)\in D$, and $E_D(j)$ otherwise. [F3, F5, F6, F7, F9, step 1.2, step 1.3]

3.1 If $y>0$ is nonintegral, it is strictly between $n=\lfloor y\rfloor$ and $n+1$. Discreteness implies that $A_D$ is constant throughout $n<x<n+1$. In a neighborhood of $y$ lying in this interval, $|E_D(x)-E_D(y)|=|-c(x-y)|=c|x-y|$. Given $\varepsilon>0$, use the least of $y-n$, $n+1-y$ and $\varepsilon/(1+c+\varepsilon)$ as $\delta$ in the two one-sided conditions. Step 1.3 supplies the limit-point condition at $y$, so both limits equal $E_D(y)$. Combining this with the integer limits and $r_M(j)=j$ for $1\le j\le M$ gives exactly the claimed jumps in $0<t\le M$. [F3, F4, F7, F9, step 1.1, step 1.2, step 1.3, step 2.2]

3.2 Suppose the test values in the statement have absolute value at most $B$. For any real $z$, the bound $|z|\le B$ is equivalent to $-B\le z\le B$. If $z\ge0$, then $|z|=z$ and $-B\le z$ holds automatically. If $z<0$, then $|z|=-z$ and $z\le B$ holds automatically, while $-z\le B$ is equivalent to $-B\le z$. For $0\le u<M$, take $a$ to be the greatest element of $\{j\in D\cup\{0,M\}:j\le u\}$ and $b$ the least element of $\{j\in D\cup\{0,M\}:u<j\}$. These sets contain $0$ and $M$, respectively. The least element of the second exists by well-ordering. The first has a greatest element because applying well-ordering to the nonnegative integers $M-j$ for $j$ in that set gives a least $M-a$. On $a\le x<b$, the count equals $A_D(a)$, since on $0\le x\le M$ the counted integers are exactly the elements of $D$ at most $x$ and none lies strictly between $a$ and $b$. Since $c\ge0$, we have $A_D(a)-cb\le E_D(u)\le A_D(a)-ca=E_D(a)$. The lower endpoint of this inequality is the left limit at $b$, by applying the formula for the constant count just below the integer $b$ from step 2.2. If $b$ is outside $D$, then $b=M$ and this limit equals $E_D(M)$. The upper endpoint is $E_D(0)$ if $a=0$, and the right limit at $a$ otherwise. Thus $-B\le E_D(u)\le B$, and the same equivalence gives $|E_D(u)|\le B$. The bound at $u=M$ is one of the endpoint tests. [F3, F8, F9, step 1.1, step 1.2, step 2.2]

4.1 For any $t\ge0$, set $q=\lfloor t/M\rfloor$ and $u=t-qM$. As in step 1.2, $q\ge0$, and $0\le u<M$. For this $u$, the period identity gives $E_D(u+jM)=E_D(u)$ for all nonnegative integers $j$. If there were a failure, the least such $j$ would be positive, and translation by $M$ from $u+(j-1)M$ would rule out failure at $j$. In particular $E_D(t)=E_D(u)$, so $|E_D(t)|\le B$. This completes the periodicity and jump-bound claims. [F3, F4, F8, step 1.2, step 2.1, step 3.2] ∎


## Reciprocal-square tail from a counting function

[Open item](item-lem-reciprocal-square-tail-from-counting) · level 0


### Statement

Let $D\subseteq\mathbb Z_{>0}$, where $\mathbb Z_{>0}$ denotes the integers greater than zero in their usual embedded copy in the complete ordered field $\mathbb R$ of real numbers, and let $P>0$ be real. For comparisons and arithmetic in $\mathbb R$, send integers to rationals by $k\mapsto k/1$ and then use the ordered-field embedding of the rationals into the reals. Send natural numbers, including finite cardinalities, first to their corresponding nonnegative integers. For real $t\ge P$ put $C(t)=\#\{k\in D:P<k\le t\}$, where $\#$ denotes finite cardinality, the number of elements of a finite set. Assume that real $a,b\ge0$ satisfy $C(t)\le a(t-P)+b$ for every real $t\ge P$. Then the series and the integral below both converge and
$$\sum_{\substack{k\in D\\k>P}}\frac1{k^2}=2\int_P^\infty C(t)t^{-3}\,dt\le\frac aP+\frac b{P^2}.$$

The series means the sequence limit of the finite sums over positive integers through $n$, taking the term to be zero unless $k\in D$ and $k>P$. The sequence limit uses positive rational tolerances, interpreted in $\mathbb R$ under the rational embedding. A finite sum begins at zero for the empty sum and adds one term at each index. The integral to infinity means the finite limit of the integrals over $[P,R]=\{t:P\le t\le R\}$ as real $R\to+\infty$. For $R>P$ and a bounded function on $[P,R]$, the finite Darboux integral is the common value of the supremum of the lower sums and the infimum of the upper sums when they agree. A function on this interval is bounded when its values have a common real lower bound and a common real upper bound. Both extrema are taken over all finite partitions of $[P,R]$, where a partition is a strictly increasing finite list of points from $P$ to $R$, including both endpoints. On the closed subinterval between each pair of consecutive points, the lower sum weights the infimum by the subinterval length and the upper sum weights the supremum by that length. For $x>0$ and a positive integer $r$, $x^{-r}$ is the reciprocal of the product of $r$ copies of $x$.

### Statement references

[math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum)

[math:def-series](https://alphabetamath.cc/item/def-series)

[math:def-real-limit](https://alphabetamath.cc/item/def-real-limit)

[math:def-interval](https://alphabetamath.cc/item/def-interval)

[math:def-darboux-integral](https://alphabetamath.cc/item/def-darboux-integral)

[math:def-bounded-set](https://alphabetamath.cc/item/def-bounded-set)

[math:def-darboux-sums](https://alphabetamath.cc/item/def-darboux-sums)

[math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)

[math:def-infimum](https://alphabetamath.cc/item/def-infimum)

[math:def-partition-and-refinement](https://alphabetamath.cc/item/def-partition-and-refinement)

[math:def-improper-integral-at-infinity](https://alphabetamath.cc/item/def-improper-integral-at-infinity)

[math:def-limits-at-infinity](https://alphabetamath.cc/item/def-limits-at-infinity)

[math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

### Facts & Assumptions

[F1] A finite set of cardinality $q$ is in bijection with the first $q$ nonnegative integers, and every subset of a finite set is finite. A bijection is a one-to-one map onto its target. Induction propagates a property from $0$ to all nonnegative integers when the property at $n$ implies it at $n+1$. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F2] The integer part $\lfloor x\rfloor$ of a real $x$ is the unique integer $d$ with $d\le x<d+1$. No integer lies strictly between $d$ and $d+1$, since such an integer would have both itself and $d$ as its integer part. Hence $k\le x$ is equivalent to $k\le\lfloor x\rfloor$ for integer $k$, and $\lfloor x\rfloor\ge0$ for $x\ge0$. Every nonnegative integer is the image of a unique natural number under the order- and arithmetic-preserving embedding. We use this identification for indices. The integer-to-rational and rational-to-real embeddings preserve order, addition, multiplication and the unit, so their composition preserves those operations and order. [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[F3] For real sequences $(e_j)$ and $(w_j)$ indexed by nonnegative integers, put $A_n=\sum_{j<n}e_j$. Abel summation by parts is the finite identity $\sum_{j<n}e_jw_j=A_nw_{n-1}+\sum_{j<n-1}A_{j+1}(w_j-w_{j+1})$ for every natural number $n\ge1$, using finite-sum scaling to move the minus sign into the remainder in the cited identity. [math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum) [math:lem-abel-summation-by-parts](https://alphabetamath.cc/item/lem-abel-summation-by-parts) [math:lem-finite-sum-laws](https://alphabetamath.cc/item/lem-finite-sum-laws)

[F4] The derivative at a domain point that is also a limit point of the domain is the punctured limit of the difference quotient, taken from within the domain. On the nonzero reals, $(t^{-r})'=-rt^{-r-1}$ for positive integers $r$. Differentiability implies continuity, meaning that $\lvert f(t)-f(c)\rvert$ can be made arbitrarily small by taking $t$ sufficiently close to $c$ in the domain. A bounded function on a closed finite interval with distinct endpoints is Darboux integrable if it is continuous except possibly at finitely many points. [math:def-derivative](https://alphabetamath.cc/item/def-derivative) [math:def-function-limit](https://alphabetamath.cc/item/def-function-limit) [math:def-limit-point-r](https://alphabetamath.cc/item/def-limit-point-r) [math:lem-derivative-of-a-power](https://alphabetamath.cc/item/lem-derivative-of-a-power) [math:cor-differentiable-implies-continuous](https://alphabetamath.cc/item/cor-differentiable-implies-continuous) [math:def-continuity-real](https://alphabetamath.cc/item/def-continuity-real) [math:def-bounded-set](https://alphabetamath.cc/item/def-bounded-set) [math:thm-finitely-many-discontinuities-integrable](https://alphabetamath.cc/item/thm-finitely-many-discontinuities-integrable)

[F5] If $u<v$, $G$ is differentiable on $[u,v]$ and $G'$ is integrable there, then $\int_u^v G'=G(v)-G(u)$. Finite integrals are linear in integrable functions and additive when an interval is split. They preserve pointwise order and satisfy $0\le\int_u^v f\le K(v-u)$ if $0\le f\le K$ and $u<v$. [math:thm-ftc-second-part](https://alphabetamath.cc/item/thm-ftc-second-part) [math:thm-linearity-of-the-integral](https://alphabetamath.cc/item/thm-linearity-of-the-integral) [math:thm-additivity-over-subintervals](https://alphabetamath.cc/item/thm-additivity-over-subintervals) [math:thm-monotonicity-of-the-integral](https://alphabetamath.cc/item/thm-monotonicity-of-the-integral)

[F6] Every nonempty set of real numbers bounded above has a least upper bound. For a real-parameter limit at $+\infty$, the error must be less than any prescribed positive real tolerance beyond some real cutoff. For a sequence limit, the error must be less than any prescribed positive rational tolerance, interpreted as a real, at all sufficiently large natural indices. A least upper bound is an upper bound that is at most every upper bound of the same set. [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field) [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field) [math:def-limits-at-infinity](https://alphabetamath.cc/item/def-limits-at-infinity) [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit) [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[F7] For a real sequence $(B_j)$ and natural numbers $0\le h\le n$, finite-sum splitting gives $\sum_{j<n} B_j=\sum_{j<h}B_j+\sum_{h\le j<n}B_j$. The last sum is $\sum_{\ell<n-h}B_{h+\ell}$ by the shifted-index definition, including the empty sum when $h=n$. [math:lem-finite-sum-laws](https://alphabetamath.cc/item/lem-finite-sum-laws) [math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum)

[F8] For real $x,y$, $|xy|=|x|\,|y|$ and $|x+y|\le |x|+|y|$. [math:lem-of-abs-value](https://alphabetamath.cc/item/lem-of-abs-value) [math:lem-of-triangle-inequality](https://alphabetamath.cc/item/lem-of-triangle-inequality)

[F9] The real field is totally ordered with $1>0$. Adding a fixed real preserves order, and the product of positive reals is positive. [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)

### Proof

**Given:** $D,P,a,b$ and the counting function $C$ satisfy the hypotheses in the Statement.

**Goal:** Establish convergence of the series and improper integral, their equality with the factor $2$, and the stated upper bound.

1.1 For a natural number $n$, let $E_n=\{k\in D:P<k\le n\}$. It is a subset of $\{1,\ldots,n\}$, which is finite because $j\mapsto j+1$ from the first $n$ nonnegative integers is injective by cancellation and onto by taking $j=k-1$ for each $1\le k\le n$. For $j\ge0$ set $e_j=1$ if $j+1\in D$ and $j+1>P$, and $e_j=0$ otherwise. The equality $\#E_n=\sum_{j<n}e_j$ holds at $n=0$ since both sides are zero. Passing from $n$ to $n+1$ leaves $E_n$ unchanged when $e_n=0$ and adjoins exactly one element when $e_n=1$. In the latter case a bijection from the first $\#E_n$ nonnegative integers onto $E_n$ extends by sending the next integer to $n+1$. The extension stays injective because $n+1\notin E_n$ and is onto $E_{n+1}$ because the old images and the new image exhaust that set. Thus both sides obey the same recursion, so they agree by induction, using the real images of the cardinalities in the sum identity. For every $t\ge P$, the integer $\lfloor t\rfloor$ is nonnegative, so it is a natural index by [F2]. The set counted by $C(t)$ is $E_{\lfloor t\rfloor}$, which proves finiteness and gives $C(t)=A_{\lfloor t\rfloor}$, with $A_n=\sum_{j<n}e_j$. [F1, F2, F3]

1.2 If $z>0$, then $z^{-1}$ exists and is nonzero because $zz^{-1}=1$. If $z^{-1}<0$, then $z(-z^{-1})=-1$ would be positive by [F9]. Thus $z^{-1}>0$ by totality. For $0<x\le y$, multiplying by positive factors gives $0<x^2\le xy\le y^2$ and $0<x^3\le x^2y\le y^3$. For $r=2,3$, the identity $x^{-r}-y^{-r}=(y^r-x^r)(x^r)^{-1}(y^r)^{-1}$ has a nonnegative right-hand side because $y^r-x^r\ge0$ and both inverses are positive. Thus $0<y^{-r}\le x^{-r}$. [F9, algebra]

2.1 Let $f(t)=C(t)t^{-3}$ for $t\ge P$ and fix $P\le u<v$. For $t\in[u,v]$, step 1.2 gives $0<t^{-3}\le P^{-3}$ since $t\ge P>0$. Its range on $[u,v]$ has lower bound $0$ and upper bound $[a(v-P)+b]P^{-3}$, so $f$ is bounded. The integers in $[u,v]$ form a subset of the finite list $1,\ldots,\lfloor v\rfloor$, which is empty if $\lfloor v\rfloor=0$. For a noninteger $x\in[u,v]$ we have $\lfloor x\rfloor<x<\lfloor x\rfloor+1$, so for $t$ sufficiently close to $x$ we have $C(t)=C(x)$ by step 1.1. Since $t^{-3}$ is continuous on the nonzero reals by [F4], for every $\varepsilon>0$ we can further restrict $t$ so that $|t^{-3}-x^{-3}|<\varepsilon/(1+C(x))$. Then $|f(t)-f(x)|=C(x)|t^{-3}-x^{-3}|<\varepsilon$. Thus [F4] gives integrability of $f$ on $[u,v]$, and in particular $I(R)=\int_P^R f(t)\,dt$ exists for every $R>P$. [given, step 1.1, step 1.2, F1, F2, F4, F8]

3.1 By step 1.2, for $P\le u<v$ and $r=2,3$, we have $0<t^{-r}\le u^{-r}$ on $[u,v]$. Thus $0$ and $u^{-r}$ bound the range, so each power is bounded. The powers are continuous on the nonzero reals by [F4], and the continuity inequalities still hold on $[u,v]$. Thus the integrability criterion in [F4] applies with zero exceptions. Write $\min\{p,q\}$ for the lesser of $p$ and $q$ in the real total order, with their common value when $p=q$. For $c\in[u,v]$ and any real $\delta>0$, if $c<v$, take $t=c+\min\{\delta,v-c\}/2$, and if $c=v$, take $t=c-\min\{\delta,c-u\}/2$. In either case $t\in[u,v]$ and $0<|t-c|<\delta$, so every $c\in[u,v]$ is a limit point of the interval. For either $G(t)=t^{-1}$ or $G(t)=t^{-2}$, the difference quotient on $[u,v]\setminus\{c\}$ is the restriction of the quotient on the nonzero reals. For every positive real tolerance, the same punctured-limit radius from the larger domain works on $[u,v]$. The derivatives on $[u,v]$ are therefore $-t^{-2}$ and $-2t^{-3}$, respectively, including at the endpoints. These derivatives are integrable by linearity. Applying [F5] to the two derivatives and dividing by their respective scalar factors gives $\int_u^v t^{-2}\,dt=u^{-1}-v^{-1}$ and $\int_u^v t^{-3}\,dt=(u^{-2}-v^{-2})/2$. On $[P,R]$ we have $0\le f(t)\le a t^{-2}+(b-aP)t^{-3}$. The upper function is integrable by linearity. Comparison and the two evaluations give $0\le 2I(R)\le 2a(P^{-1}-R^{-1})+(b-aP)(P^{-2}-R^{-2})$. The last expression equals $a/P+b/P^2-[aR+a(R-P)+b]/R^2$. The subtracted numerator is nonnegative since $a,b\ge0$ and $R>P$, so $2I(R)\le a/P+b/P^2$. [given, step 1.2, step 2.1, F4, F5, F9]

4.1 For $P<R_1<R_2$, additivity and $f\ge0$ give $I(R_2)-I(R_1)=\int_{R_1}^{R_2}f\ge0$. The nonempty set of values $I(R)$ for real $R>P$ has a least upper bound $L$ by step 3.1. For every $\varepsilon>0$ there is $R_0>P$ with $I(R_0)>L-\varepsilon$, as otherwise $L-\varepsilon$ would be an upper bound smaller than $L$. For $R\ge R_0$, therefore, $L-\varepsilon<I(R)\le L$. This proves $\int_P^\infty f=L$ and $2L\le a/P+b/P^2$. [step 2.1, step 3.1, F5, F6]

4.2 Suppose $P\le u<v$ and $C(t)=c$ on $[u,v)=\{t:u\le t<v\}$. The functions $f$ and $ct^{-3}$ are integrable on $[u,v]$ and on every nondegenerate closed subinterval by step 2.1, step 3.1 and linearity. To show the two integrals over $[u,v]$ agree, split the interval at $v-\delta$ with $0<\delta<v-u$. The integrands agree on $[u,v-\delta]$. On the remaining interval both are between $0$ and $K=[a(v-P)+b]P^{-3}$, using step 1.2 and $0\le c=C(u)\le a(u-P)+b\le a(v-P)+b$. Their integrals over that interval are each between $0$ and $K\delta$, so the absolute difference over $[u,v]$ is at most $K\delta$ for every such $\delta$ and must be zero. Consequently $2\int_u^v f(t)\,dt=c(u^{-2}-v^{-2})$. [given, step 1.2, step 2.1, step 3.1, F5]

5.1 Let $m=\lfloor P\rfloor+1$, so $m>P$ and $m\ge1$. Interpret $m$ and each integer $N\ge m$ as natural indices by [F2]. Split $[P,N]$ at $m,m+1,\ldots,N$, using each endpoint once. On $[P,m)$ the count is zero, and on $[j,j+1)$ for integer $j\ge m$ it is $A_j$. By induction on the number of subintervals, repeated additivity from [F5] adds the values given by step 4.2. This gives $2I(N)=\sum_{j=m}^{N-1} A_j(j^{-2}-(j+1)^{-2})$, with an empty sum when $N=m$. With $w_j=(j+1)^{-2}$, Abel summation applies at $n=N\ge1$. In its remainder write $B_j=A_{j+1}((j+1)^{-2}-(j+2)^{-2})$. The sum is over $j<N-1$. By [F7] split it at $h=m-1$, which lies between $0$ and $N-1$. For $j<m-1$ we have $A_{j+1}=0$ by step 1.1 because $E_{j+1}$ is empty, so the initial sum is zero by the finite-sum recursion. In the remaining sum $j=m-1+\ell$ with $0\le\ell<N-m$, so $i=j+1=m+\ell$ gives the terms of the integral sum. If $m=1$ the initial sum is empty, and if $m=N$ the remaining sum is empty. Thus the Abel remainder equals $2I(N)$. Since $A_N=C(N)$, the finite partial sum $S_N=\sum_{j<N}e_j(j+1)^{-2}$ satisfies $S_N=C(N)/N^2+2I(N)$. [F1, F2, F3, F5, F7, step 1.1, step 4.2]

6.1 For integers $N\ge m$ the first term of the finite identity is bounded by $0\le C(N)/N^2\le a/N+b/N^2\le (a+b)/N$. Given a positive rational $\varepsilon$, use its positive real image in the following estimates and choose a real cutoff $M\ge P$ beyond which $|I(R)-L|<\varepsilon/4$ and with $M\ge2(a+b)/\varepsilon$. Every natural $N\ge\lfloor M\rfloor+1$ has $N>M$ by [F2] and $N\ge m$, so the finite identity and [F8] give $|S_N-2L|\le C(N)/N^2+2|I(N)-L|<\varepsilon$. The sum of the series is the limit of these partial sums, so it equals $2L=2\int_P^\infty C(t)t^{-3}\,dt\le a/P+b/P^2$, as required. [given, step 4.1, step 5.1, F2, F6, F8] ∎


## Trial division up to the square root

[Open item](item-lem-trial-division-primality-bound) · level 0


### Statement

An integer $u>1$ is prime, meaning that its only positive divisors are $1$ and $u$, if and only if no integer $d$ with $2\le d\le\lfloor\sqrt u\rfloor$ divides $u$. Here $d$ divides $u$ when $u=dq$ for an integer $q$. The symbol $\sqrt u$ denotes the nonnegative real number whose square is $u$, and $\lfloor x\rfloor$ denotes the unique integer $m$ with $m\le x<m+1$ for a real number $x$.

For each nonnegative integer $d$, the bound $d\le\lfloor\sqrt u\rfloor$ is equivalent to $d^2\le u$, where $d^2=d\cdot d$. Thus the same test can use the integer cutoff $d\ge2$ and $d^2\le u$.

For any positive real bound $B$, all primes at most $B$ can therefore be listed by finitely many exact divisibility tests.

### Statement references

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

### Facts & Assumptions

[F1] Use the integers $\mathbb Z$ and real numbers $\mathbb R$ of [math:def-integers](https://alphabetamath.cc/item/def-integers) and [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers). Use integer addition and multiplication from [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) and the canonical orders from [math:def-int-order](https://alphabetamath.cc/item/def-int-order) and [math:def-real-order](https://alphabetamath.cc/item/def-real-order). The inclusion of the integers in the reals factors through the rationals $\mathbb Q$ of [math:def-rationals](https://alphabetamath.cc/item/def-rationals). The two injective maps in [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) and [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) preserve order, sums and products. They send the integer constants $0$ and $1$ to the corresponding real constants under composition. The integers form a commutative ring with identity by [math:thm-int-comm-ring](https://alphabetamath.cc/item/thm-int-comm-ring), so $0+k=k$, $a\cdot1=a$, and $ab=ba$. Distributing $a(0+0)$ gives $a\cdot0=a\cdot0+a\cdot0$, so additive cancellation gives $a\cdot0=0$.

[F2] For $u>1$, the prime condition is equivalent to requiring that every positive divisor of $u$ be $1$ or $u$ by [math:def-prime](https://alphabetamath.cc/item/def-prime). A divisor $d$ of $u$ gives an integer $q$ with $u=dq$, and every such equality gives a divisor by [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z).

[F3] The reals with their canonical order are an ordered field in the sense of [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field). They have the least-upper-bound property by [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete), so they are a complete ordered field in the sense of [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field). Thus [math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots) gives a unique nonnegative real square root for each nonnegative real number.

[F4] Multiplication by a positive real number preserves and reflects strict inequality by [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules). It also preserves weak inequality, since it preserves equality. On nonnegative reals, $x\le y$ is equivalent to $x^2\le y^2$ and $x<y$ is equivalent to $x^2<y^2$ by [math:lem-of-square-monotone](https://alphabetamath.cc/item/lem-of-square-monotone).

[F5] Every real $x$ has a unique integer $m$ with $m\le x<m+1$ by [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part).

[F6] For any integer $v$ and any positive integer $d$, there are unique integers $q,r$ with $v=qd+r$ and $0\le r<d$. The integer $r$ is the remainder and equals zero exactly when $d$ divides $v$ by [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z). In this theorem the zero-remainder case is $v=qd$, which is the same as $v=dq$ by commutativity in [F1].

[F7] The embedding of [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) identifies the natural numbers with the nonnegative integers, preserving order and arithmetic. In the order of [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order), the natural numbers below $n$ form the finite initial segment $I_n=\{t\in\mathbb N:t<n\}$ by [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment). In the natural-number construction of [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers), this is the list of predecessors of $n$, starting at $0$ when $n>0$. By [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality), a set is finite if it can be put in bijection with a natural initial segment, and its cardinality is the size of that segment. In particular, $I_n$ has cardinality $n$ by [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment).

[F8] In the ordered real field of [F3], $0<1$ by [math:cor-of-one-positive](https://alphabetamath.cc/item/cor-of-one-positive). Adding the same real on both sides of a strict inequality preserves it by [math:lem-of-add-order](https://alphabetamath.cc/item/lem-of-add-order).

[F9] The Cartesian product $A\times B$ consists of the ordered pairs $(a,b)$ with $a\in A$ and $b\in B$ by [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product) and [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair). Equality of these pairs is coordinatewise by [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs). If $A$ and $B$ are finite, their product is finite with cardinality the product of their cardinalities by [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule). A subset of a finite set is finite with cardinality at most that of the containing set by [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set), with subsets and separation as in [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset).

### Proof

**Given:** An integer $u>1$ and a positive real bound $B$ for the enumeration.

**Goal:** Prove the stated test for $u$ and show that it yields a finite list of all primes at most $B$.

1.1 Adding an integer $k$ to $0<1$ gives $k<k+1$ by [F1] and [F8], using the order-preserving inclusion into the reals. For any integer $m$, an integer $k$ cannot satisfy $m<k<m+1$. If it did, both $m$ and $k$ would satisfy the floor inequalities for $x=k$, since $k\le k<k+1$. This contradicts uniqueness. It follows that for an integer $k$ and real $x$, $k\le x$ is equivalent to $k\le\lfloor x\rfloor$. One direction uses $\lfloor x\rfloor\le x$. In the other, $k\le x$ and $k>\lfloor x\rfloor$ would put $k$ strictly between $\lfloor x\rfloor$ and $\lfloor x\rfloor+1$. [F1, F3, F5, F8]

2.1 For each nonnegative integer $d$, the floor comparison and the square comparison give $d\le\lfloor\sqrt u\rfloor$ exactly when $d^2\le u$. Multiplying $1<u$ by $u>0$ gives $u<u^2$, so strict comparison of nonnegative squares gives $\sqrt u<u$. As $\lfloor\sqrt u\rfloor\le\sqrt u$, the floor is also strictly less than $u$. [given, F1, F3, F4, F8, step 1.1]

2.2 Set $M=\lfloor B\rfloor$. By step 1.1 the possible primes at most $B$ lie among the integers $2,\ldots,M$. If $M<2$, return the empty list. Otherwise $M+1$ is nonnegative, so it is a natural number under the identification in [F7]. Scan $I_{M+1}$ in increasing order and skip entries below $2$. The integers in this segment satisfy $0\le u<M+1$, which is equivalent to $0\le u\le M$ by step 1.1's consecutive-integer comparison. Thus the scan visits exactly the candidates $2,\ldots,M$ once. [given, F1, F2, F3, F5, F7, step 1.1]

3.1 If $u$ is prime, then every integer $d$ in the test range satisfies $1<d<u$ by step 2.1, so it cannot divide $u$. [F2, step 2.1]

3.2 If $u$ is not prime, it has a positive divisor $a$ distinct from $1$ and $u$. Write $u=ab$ with $b$ an integer. Since $a>0$ and $a\cdot0=0<ab=u$, reflection of strict inequality gives $b>0$. Also $b\ne1$, since $b=1$ would give $a=u$. Both $a$ and $b$ are positive integers different from $1$. Step 1.1 excludes integers strictly between $0$ and $1$ and between $1$ and $2$, so $a,b\ge2$. Let $d$ be the smaller and $e$ the larger of $a,b$, with both equal to $a$ if $a=b$. By commutativity $de=ab=u$, so $d\mid u$. Since $0<d\le e$, $d^2\le de=u$. Step 2.1 puts this divisor in the test range. [given, F1, F2, F3, F4, step 1.1, step 2.1]

4.1 For each candidate $u$, scan $I_u$ under the same identification. Skip entries $d<2$ or $d^2>u$. By step 2.1 the remaining entries are exactly the integers in the trial range, since the floor of the square root is strictly less than $u$. Each test checks whether the remainder on dividing $u$ by $d$ is zero. Each individual scan terminates because it traverses a finite initial segment by [F7]. By steps 3.1 and 3.2 a candidate is prime exactly when no tested remainder is zero. Retaining precisely those candidates gives all the primes at most $B$. [F1, F6, F7, step 2.1, step 2.2, step 3.1, step 3.2]

5.1 When $M<2$ there are no tests. Otherwise every test has a candidate $u$ in $I_{M+1}$ and a divisor $d$ in $I_u$, hence in $I_{M+1}$ since $d<u\le M$. The tested pairs form the subset of $I_{M+1}\times I_{M+1}$ with $2\le u\le M$, $2\le d<u$, and $d^2\le u$. Each pair is tested once because both scans visit each of their entries once. The product rule and the finite-subset bound give at most $(M+1)^2$ tests, since $I_{M+1}$ has cardinality $M+1$. [F1, F7, F9, step 2.2, step 4.1] ∎


## A floor difference detects divisibility

[Open item](item-lem-floor-increment-divisibility) · level 0


### Statement

Let $b,p\in\mathbb{Z}$ with $p>0$, where $\mathbb{Z}$ denotes the integers. When taking real quotients or floors, identify the integers with their image in $\mathbb{R}$, the real numbers, under the canonical embedding through the rationals. For real $a$, the quotient $a/p$ is the unique real $u$ satisfying $up=a$. For a real number $x$, its floor $\lfloor x\rfloor$ is the unique integer $m$ with $m\le x<m+1$. The notation $p\mid b$ means that $b=pt$ for some integer $t$.

Then $\lfloor b/p\rfloor-\lfloor(b-1)/p\rfloor$ is $1$ if $p\mid b$ and $0$ otherwise.

### Statement references

[The integers](https://alphabetamath.cc/item/def-integers)

[The real numbers](https://alphabetamath.cc/item/def-real-numbers)

[The rationals](https://alphabetamath.cc/item/def-rationals)

[Division in a field](https://alphabetamath.cc/item/def-field)

[The floor of a real number](https://alphabetamath.cc/item/lem-integer-part)

[Divisibility of integers](https://alphabetamath.cc/item/def-divides-in-z)

[Integer arithmetic](https://alphabetamath.cc/item/def-int-operations)

[Integer order](https://alphabetamath.cc/item/def-int-order)

[Real order](https://alphabetamath.cc/item/def-real-order)

[Ordered field](https://alphabetamath.cc/item/def-ordered-field)

[The integers in the rationals](https://alphabetamath.cc/item/lem-int-embeds-rat)

[The rationals in the reals](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[The real ordered field](https://alphabetamath.cc/item/thm-reals-ordered-field)

### Facts & Assumptions

[F1] The canonical map $e:\mathbb{Z}\to\mathbb{R}$ first sends an integer $k$ to the rational class $[(k,1)]$ ([The rationals](https://alphabetamath.cc/item/def-rationals)) and then to the real class of the corresponding constant sequence. Both embeddings are injective and preserve addition, multiplication and order ([The integers in the rationals](https://alphabetamath.cc/item/lem-int-embeds-rat), [The rationals in the reals](https://alphabetamath.cc/item/lem-rat-embeds-dense)). For every real $x$, the unique integer $m$ satisfying $m\le x<m+1$ in this identification is $\lfloor x\rfloor$ ([Integer part](https://alphabetamath.cc/item/lem-integer-part)).

[F2] For integers $b,p$ with $p>0$ in the integer order ([Integer order](https://alphabetamath.cc/item/def-int-order)), there are unique integers $q,r$ with $b=qp+r$ and $0\le r<p$. The integer $r$ is called the remainder, and $r=0$ exactly when $p\mid b$ ([Division with remainder](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

[F3] For reals $x,y$ with $y\ne0$, the quotient $x/y$ is $xy^{-1}$, where $y^{-1}$ is the unique real number with $yy^{-1}=1$. The field laws include associative and commutative addition and multiplication, additive inverses, and distributivity of multiplication over addition ([Field](https://alphabetamath.cc/item/def-field)).

[F4] The real order makes the reals a totally ordered field ([Real order](https://alphabetamath.cc/item/def-real-order), [Ordered field](https://alphabetamath.cc/item/def-ordered-field), [The real ordered field](https://alphabetamath.cc/item/thm-reals-ordered-field)). In particular, the order is transitive, any two reals are comparable, and adding the same real to both sides preserves strict and weak inequalities. Its multiplicative identity satisfies $0<1$ ([Positivity of one](https://alphabetamath.cc/item/cor-of-one-positive)).

[F5] In an ordered field, multiplication by a positive element $c$ preserves and reflects strict inequalities, so $x<y$ holds exactly when $xc<yc$ ([Order under multiplication](https://alphabetamath.cc/item/lem-of-sign-rules)). The same equivalence holds for weak inequalities because $x\le y$ in a total order exactly when $y<x$ fails ([Ordered field](https://alphabetamath.cc/item/def-ordered-field)).

[F6] In the integers, $0$ and $1$ are the additive and multiplicative identities, and addition, negation and multiplication take integer values. Integer subtraction is addition of the additive inverse ([Integer arithmetic](https://alphabetamath.cc/item/def-int-operations), [The integer ring](https://alphabetamath.cc/item/thm-int-comm-ring)).

### Proof

**Given:** Integers $b,p$ with $p>0$.

**Goal:** Show that the floor difference is $1$ when $p\mid b$ and is $0$ otherwise.

1.1 Since $e$ preserves addition, $e(0)=e(0)+e(0)$, so real additive cancellation gives $e(0)=0$. Order preservation and $p>0$ give $e(p)>0$. Since $p\cdot1=p$ and $e$ preserves multiplication, $e(p)e(1)=e(p)$, so cancellation by the nonzero real $e(p)$ gives $e(1)=1$. Also $e(s)+e(-s)=e(0)=0$ for every integer $s$, so negation and subtraction agree under the identification. From here on, write each integer for its real image when taking real quotients or comparing with reals. [given, F1, F3, F4, F6]

2.1 For integers $a,k$, the inequalities $k\le a/p<k+1$ are equivalent to $kp\le a<(k+1)p$. Indeed $p$ is positive in the reals, so multiplication by $p$ preserves and reflects both comparisons, and $(a/p)p=a$. Thus $kp\le a<(k+1)p$ implies $\lfloor a/p\rfloor=k$. [given, F1, F3, F5, F6, step 1.1]

2.2 Every positive integer $s$ satisfies $1\le s$. Since $0<1$, adding $s$ gives $s<s+1$. If $0<s<1$, both $0\le s<0+1$ and $s\le s<s+1$ would hold, so the uniqueness of the floor of $s$ would give $s=0$. Total order now gives $1\le s$. [F1, F3, F4, F6, step 1.1]

3.1 Choose integers $q,r$ with $b=qp+r$ and $0\le r<p$. Adding $qp$ to the bounds on $r$ gives $qp\le b<qp+p=(q+1)p$, so $\lfloor b/p\rfloor=q$. [given, F2, F3, F4, F6, step 1.1, step 2.1]

4.1 If $r=0$, then $b=qp$. Since $1\le p$, we obtain $(q-1)p=b-p\le b-1<b=qp$. Applying step 2.1 with $a=b-1$ and $k=q-1$ gives $\lfloor(b-1)/p\rfloor=q-1$. [given, F3, F4, F6, step 1.1, step 2.1, step 2.2, step 3.1]

4.2 If $r>0$, then $1\le r$, so $0\le r-1$ and $qp\le b-1=qp+(r-1)<b<(q+1)p$. Applying step 2.1 with $a=b-1$ and $k=q$ gives $\lfloor(b-1)/p\rfloor=q$. [F3, F4, F6, step 1.1, step 2.1, step 2.2, step 3.1]

5.1 The two cases exhaust $r\ge0$. The difference is $q-(q-1)=1$ when $r=0$ and $q-q=0$ when $r>0$. As $r=0$ holds exactly when $p\mid b$, this is the claimed floor difference. [F2, F4, F6, step 1.1, step 3.1, step 4.1, step 4.2] ∎


## Progression of roots of an invertible linear congruence

[Open item](item-lem-invertible-linear-residue-progression) · level 0


### Statement

Let $p$ be a prime integer, meaning that $p>1$ and its only positive divisors are $1$ and $p$. Let $a,b$ be integers with $p\nmid a$, meaning that $a$ is not an integer multiple of $p$. The congruence $aj+b\equiv0\pmod p$ means that $aj+b$ is an integer multiple of $p$.

There is exactly one integer solution $j_0$ with $0\le j_0<p$. The nonnegative integer solutions, those with $j\ge0$, are exactly the progression $j_0+rp$ with $r$ an integer satisfying $r\ge0$.

### Statement references

[Integers](https://alphabetamath.cc/item/def-integers)

[Integer operations and constants](https://alphabetamath.cc/item/def-int-operations)

[Integer order](https://alphabetamath.cc/item/def-int-order)

[Prime integers](https://alphabetamath.cc/item/def-prime)

[Integer divisibility](https://alphabetamath.cc/item/def-divides-in-z)

[Congruence modulo an integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[Ordered integers](https://alphabetamath.cc/item/thm-int-ordered-ring)

### Facts & Assumptions

[F1] For integers $d,x$, $d\mid x$ means $x=dq$ for some integer $q$, and $d\nmid x$ is its negation ([math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)). Congruence $x\equiv y\pmod p$ means $p\mid(x-y)$ ([math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)). A prime exceeds $1$ and has only $1$ and itself as positive divisors ([math:def-prime](https://alphabetamath.cc/item/def-prime)).

[F2] The residue class $[x]_p$ is the set of integers congruent to $x$ modulo $p$. The set of all these classes is $\mathbb Z/p$, and $[x]_p=[y]_p$ holds exactly when $x\equiv y\pmod p$ ([math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)).

[F3] Write $\mathbb N$ for the natural numbers ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)). Because the prime $p$ is positive, the canonical embedding $\iota$ of the natural numbers into the integers gives a unique natural number $n$ with $\iota(n)=p$ ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)). Use $n$ as the natural modulus and $p$ as its integer image in the class notation. With that modulus, addition and multiplication of classes are given by $[x]_p+[y]_p=[x+y]_p$ and $[x]_p[y]_p=[xy]_p$ ([math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)). The formulas and the integer laws in F6 give $[0]_p$ as additive zero, $[1]_p$ as multiplicative one, and $[-x]_p$ as the additive inverse of $[x]_p$.

[F4] For prime $p$, these operations make $\mathbb Z/p$ a field ([math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)). In particular, addition permits cancellation, multiplication is associative, and every nonzero element $u$ has a multiplicative inverse $u^{-1}$ satisfying $uu^{-1}=u^{-1}u=1$, where $1$ is the multiplicative identity ([math:def-field](https://alphabetamath.cc/item/def-field)).

[F5] Division with remainder gives, for each integer $t$ and positive integer $p$, a unique pair of integers $q,s$ with $t=qp+s$ and $0\le s<p$ ([math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

[F6] Use the integer addition, multiplication, additive inverses, zero and one ([math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)) and the usual order on the integers ([math:def-int-order](https://alphabetamath.cc/item/def-int-order)). This structure on the integers ([math:def-integers](https://alphabetamath.cc/item/def-integers)) forms a totally ordered commutative ring ([math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)). Use the ring laws for additive identities and inverses, and distributivity ([math:def-ring](https://alphabetamath.cc/item/def-ring)), as well as commutativity of integer multiplication. In particular, $0x=0$ follows by distributing $(0+0)x$ and cancelling $0x$. The order is total, adding the same integer preserves inequalities, and the product of positive integers is positive ([math:def-ordered-ring](https://alphabetamath.cc/item/def-ordered-ring)). Translation preserves strict inequalities because cancellation rules out equality after translation.

### Proof

**Given:** A prime integer $p$ and integers $a,b$ with $p\nmid a$.

**Goal:** Find the unique integer solution $j_0$ in $0\le j_0<p$ and characterize all nonnegative integer solutions of $aj+b\equiv0\pmod p$.

1.1 Since $p\nmid a$, the class $[a]_p$ differs from $[0]_p$. The congruence for an integer $j$ is equivalent to $[a]_p[j]_p+[b]_p=[0]_p$. Adding $[-b]_p$ and multiplying on the left by $[a]_p^{-1}$ transforms this equation into $[j]_p=[a]_p^{-1}[-b]_p$. Multiplying back by $[a]_p$ and adding $[b]_p$ reverses both operations, so this class equation is equivalent to the congruence. [given, F1, F2, F3, F4, F6]

2.1 Choose an integer $t$ whose class is $[a]_p^{-1}[-b]_p$. Since $p>0$, divide $t$ by $p$ to write $t=qp+j_0$ with $0\le j_0<p$. Subtracting $j_0$ and commuting the product gives $t-j_0=pq$, so $p\mid(t-j_0)$ and $[j_0]_p=[t]_p$. Thus $j_0$ solves the congruence. [step 1.1, F1, F2, F5, F6]

3.1 An integer $j$ solves the congruence exactly when $[j]_p=[j_0]_p$, or equivalently when $p\mid(j-j_0)$. The latter condition says $j-j_0=pr$ for some integer $r$, which is equivalent to $j=j_0+rp$ by adding $j_0$ and commuting the product. [step 1.1, step 2.1, F1, F2, F6]

4.1 If $j$ is a solution with $0\le j<p$, then $j=0\cdot p+j$ and $j=rp+j_0$ are both divisions of $j$ by $p$ with remainders in the required range. Uniqueness of the remainder gives $j=j_0$. [step 2.1, step 3.1, F5, F6]

5.1 For any solution $j\ge0$, take $r$ as in step 3.1. If $r<0$, translation gives $-r>0$. Since $p>0$, the product $(-r)p$ is positive, and distributivity gives $rp+(-r)p=(r+(-r))p=0$. Translating $0<(-r)p$ by $rp$ gives $rp<0$, so $0\le j<j_0<p$. This contradicts step 4.1, so $r\ge0$. [step 3.1, step 4.1, F1, F6]

6.1 Conversely, if $r\ge0$, then $rp\ge0$ by the zero law when $r=0$ and the positive product law when $r>0$. Thus $j=j_0+rp\ge j_0\ge0$ and $j$ is a solution by step 3.1. Together with steps 4.1 and 5.1, this proves both claims. [step 2.1, step 3.1, step 4.1, step 5.1, F1, F6] ∎


## Finite binary products as avoidance indicators

[Open item](item-lem-binary-products-and-avoidance) · level 0


### Statement

Let $I$ be a finite set, meaning that its elements can be listed once each in a list of natural length $|I|$, called its cardinality. Let $(b_i)_{i\in I}$ be an indexed family of binary test values in $\{0,1\}$, with $1$ denoting success. The product $\prod_{i\in I}(1-b_i)$ is the avoidance indicator. It is $1$ if every $b_i=0$ and $0$ if some $b_i=1$.

Let $X$ be another finite set and let $\big((b_{x,i})_{i\in I}\big)_{x\in X}$ be an $X$-indexed family whose rows are $I$-indexed families of values in $\{0,1\}$. For each $x$ put $P_x=\prod_{i\in I}(1-b_{x,i})$. The set $A=\{x\in X : b_{x,i}=0\text{ for every }i\in I\}$ is finite, and
$$\sum_{x\in X}P_x=|A|.$$

The sums and products are taken in the natural numbers, with empty sum $0$ and empty product $1$. For a binary value $b$, the difference $1-b$ is the unique natural $d$ satisfying $b+d=1$.

### Statement references

[math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-unordered-pair-and-singleton](https://alphabetamath.cc/item/def-unordered-pair-and-singleton)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

[math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)

### Facts & Assumptions

[F1] A finite set of cardinality $n$ has a listing indexed by the first $n$ natural numbers in which each of its elements occurs exactly once. The natural number $0$ is $\varnothing$, and the successor of $n$ is $n\cup\{n\}$, so $1=\{0\}$. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[F2] A sum or product over a finite set is the sum or product of the corresponding list of values, independent of the listing. The empty sum is $0$ and the empty product is $1$. [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

[F3] A product of a list of naturals starts at $1$ and appending one entry multiplies the previous product by that entry. When $b\le 1$, the truncated difference $1-b$ is the unique natural $d$ with $b+d=1$. The condition $b\le 1$ means that such a natural $d$ exists. [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[F4] Natural addition is defined by $m+0=m$ and $m+(n+1)=(m+n)+1$, where $n+1$ denotes the successor. Also $0+m=m$ for every natural $m$. [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:lem-nat-add-identity](https://alphabetamath.cc/item/lem-nat-add-identity)

[F5] For every natural $m$ we have $m\cdot0=0$ by the definition of natural multiplication and $m\cdot1=m$ by the right identity law. [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication) [math:lem-nat-mult-identity](https://alphabetamath.cc/item/lem-nat-mult-identity)

[F6] Induction proves a property for all natural numbers from its case at $0$ and the implication from each $n$ to its successor. [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F7] For a finite set $X$ and finite sets $A_x$ for $x\in X$ that are pairwise disjoint, meaning no element belongs to both $A_x$ and $A_y$ for distinct $x,y\in X$, their union is finite and its cardinality is $\sum_{x\in X}|A_x|$. [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)

[F8] An indexed family with index set $I$ is a function with domain $I$. The subscript specifies its value at that index. [math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)

[F9] The singleton $\{x\}$ has $x$ as its only element. [math:def-unordered-pair-and-singleton](https://alphabetamath.cc/item/def-unordered-pair-and-singleton)

[F10] An element belongs to the indexed union $\bigcup_{x\in X}A_x$ exactly when it belongs to $A_x$ for some $x\in X$. [math:def-indexed-union-and-intersection](https://alphabetamath.cc/item/def-indexed-union-and-intersection)

[F11] Separation inside $X$ defines the subset consisting of exactly the elements of $X$ that satisfy the given condition. [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

### Proof

**Given:** Finite sets $I$ and $X$ and the binary test values in the statement.

**Goal:** Evaluate the single product and show that the sum of the products equals the number of indices with no successful test.

1.1 If $b=0$, then $b+1=1$, so the unique difference $1-b$ equals $1$. If $b=1$, then $b+0=1$, so the unique difference equals $0$. This gives existence and the required value of the difference in both cases. [F3, F4]

1.2 A list of length $0$ has no successful test, and the product equals $1$ by the empty product clause. [base, F3]

1.3 Fix a natural number $n$ and assume that for every list of $n$ binary values the product of their differences from $1$ is $1$ if all the values are $0$ and $0$ if at least one is $1$. [ih]

2.1 For a list of length $n+1$, the first $n$ entries form a list of length $n$. The product for the full list is the product for those first $n$ entries multiplied by the difference from $1$ of the last entry. If the last test value is $1$, this multiplies by $0$ and gives $0$. If the last test value is $0$, this multiplies by $1$ and leaves the first product unchanged, and the full list has a successful test exactly when the first $n$ entries do. This proves the rule for length $n+1$. [F1, F3, F5, step 1.1, step 1.3]

3.1 By induction the rule holds for all finite lists. A listing of $I$ contains each index exactly once, so the indexed family gives exactly one entry at each position, and a successful test in that list means a successful test at some $i\in I$. The definition of the finite-set product therefore gives the claimed rule on $I$. [F1, F2, F6, F8, step 1.2, step 2.1]

4.1 For each $x\in X$, apply the rule on $I$ to the row $(b_{x,i})_{i\in I}$. The products form an $X$-indexed family with $P_x=1$ for $x\in A$ and $P_x=0$ for $x\in X$ with $x\notin A$. Define a family $(A_x)_{x\in X}$ by setting $A_x=\{x\}$ if $P_x=1$ and $A_x=\varnothing$ if $P_x=0$. The two cases assign exactly one set to each $x$. The singleton has the one-entry listing with entry $x$, and the empty set has the empty listing, so $|A_x|=P_x$ in either case. [given, F1, F8, F9, F11, step 3.1]

5.1 Any element of $A_x$ must equal $x$, so sets with distinct indices have no common element. An element $z$ belongs to $\bigcup_{x\in X}A_x$ exactly when it equals some $x\in X$ with $P_x=1$. By step 4.1 and the membership condition for $A$, this is equivalent to $z\in A$. Thus the union is $A$. The finite disjoint union rule makes $A$ finite and gives $|A|=\sum_{x\in X}|A_x|=\sum_{x\in X}P_x$. [F2, F7, F9, F10, F11, step 4.1]

6.1 The product rule of step 3.1 and the count of step 5.1 give both conclusions, including the empty index sets covered by the same product and sum conventions. [F2, step 3.1, step 5.1, discharge-induction] ∎


## Repeated finite deletions and translation of indicator support

[Open item](item-lem-finite-deletions-and-translated-support) · level 0


### Statement

Let $\mathbb N$ be the natural numbers including $0$, and let $m^+$ denote the successor of $m$. A set is finite if, for some $n\in\mathbb N$, there is a bijection from the set onto $\{j\in\mathbb N:j<n\}$, the first $n$ natural numbers. Let $D$ be a finite subset of the integers $\mathbb Z$, and let $E_1,\ldots,E_r$ be an indexed family of subsets of $\mathbb Z$ for $r\in\mathbb N$, with one specified set $E_j$ for each $1\le j\le r$.

For sets $A,B$, the set difference $A\setminus B$ consists of the elements of $A$ outside $B$. For $0\le m\le r$, let $U_m=\bigcup_{1\le j\le m}E_j$ be the union of the first $m$ sets, consisting of the elements that belong to at least one of them. The empty union $U_0$ is the empty set. Start at $C_0=D$ and at each index $m^+$ with $0\le m<r$ delete $E_{m^+}$ by setting $C_{m^+}=C_m\setminus E_{m^+}$. This determines a unique family $C_0,\ldots,C_r$ of finite sets, with $C_m=D\setminus U_m$ for every $0\le m\le r$.

Write $\mathbb Z_{\ge0}=\{t\in\mathbb Z:0\le t\}$ for the nonnegative integers. Let $S\subseteq\mathbb Z_{\ge0}$. Its binary indicator, extended by zero to all integers, is the function with value $\varepsilon_t=1$ if $t\in S$ and value $\varepsilon_t=0$ otherwise. Its support, the set of arguments where the value is $1$, is $S$. For an integer $i$, the translate $i+S$ consists of the sums $i+s$ with $s\in S$. With $k-i=k+(-i)$, for every integer $k$,
$$k\in i+S\quad\Longleftrightarrow\quad k\ge i\ \text{and}\ \varepsilon_{k-i}=1.$$

### Statement references

[Bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)

### Justification

The condition $1\le j\le m$ selects a subset of the original index set when $m\le r$, by transitivity of the natural order. Keeping exactly the pairs of the original family with those indices defines its restriction by [separation within a set](https://alphabetamath.cc/item/def-subset-and-proper-subset). The ordered-pair equality criterion in [F2] gives each retained pair a unique first coordinate. Every selected index keeps its original value, and that value is unique by the [indexed-family definition](https://alphabetamath.cc/item/def-indexed-family). Its [indexed union](https://alphabetamath.cc/item/def-indexed-union-and-intersection) exists and contains an element exactly when some selected set contains it.

Separation inside $\mathbb Z$ gives $\mathbb Z_{\ge0}$ and $i+S$, since the stated integer comparison and addition define conditions on integers. The indicator graph is formed by separation inside $\mathbb Z\times\{0,1\}$, the set of pairs with first coordinate an integer and second coordinate either $0$ or $1$. For each integer $t$, keep $(t,1)$ if $t\in S$ and $(t,0)$ otherwise. The ordered-pair equality criterion in [F2] makes the coordinates unambiguous, and the two membership cases give exactly one value at each integer. Thus the graph defines a function. Its support is formed by separation on the condition $\varepsilon_t=1$. Since the integer values $0$ and $1$ are distinct by [F6], this condition holds exactly when $t\in S$. [Cartesian product](https://alphabetamath.cc/item/def-cartesian-product) [Unordered pair](https://alphabetamath.cc/item/def-unordered-pair-and-singleton) [Function](https://alphabetamath.cc/item/def-function)

### Facts & Assumptions

[F1] In the [natural numbers](https://alphabetamath.cc/item/def-natural-numbers), $0$ is empty and $m^+$ consists of the elements of $m$ together with $m$ itself. In the [natural order](https://alphabetamath.cc/item/def-nat-order), $j<m$ means $j\le m$ and $j\ne m$. The order satisfies $j\le m$ exactly when $j\subseteq m$, and $j<m^+$ exactly when $j\le m$ by [the membership description of natural order](https://alphabetamath.cc/item/lem-nat-order-is-membership). The empty set is a subset of every set, so $0\le m$. Transitivity of inclusion gives transitivity of $\le$. Also $m<r$ exactly when $m^+\le r$ by [discreteness of natural order](https://alphabetamath.cc/item/lem-nat-discrete).

[F2] A subset has all its elements in the ambient set. [Separation](https://alphabetamath.cc/item/def-subset-and-proper-subset) selects the elements satisfying a specified condition inside an existing set. The [power set](https://alphabetamath.cc/item/def-power-set) $\mathcal P(D)$ consists of all subsets of $D$, and the [Cartesian product](https://alphabetamath.cc/item/def-cartesian-product) $A\times B$ consists of the [ordered pairs](https://alphabetamath.cc/item/def-ordered-pair) $(a,b)$ with $a\in A$ and $b\in B$. The [ordered-pair equality criterion](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs) states that $(a,b)=(c,d)$ exactly when $a=c$ and $b=d$. Such a set of pairs defines a [function from](https://alphabetamath.cc/item/def-function) $A$ to $B$ if it assigns exactly one $b$ to each $a$.

[F3] Membership in a [set difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference) requires membership in the first set and exclusion from the second. Membership in an [indexed union](https://alphabetamath.cc/item/def-indexed-union-and-intersection) requires membership in at least one set at a selected index. By [extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality), sets with the same elements are equal.

[F4] [Induction](https://alphabetamath.cc/item/thm-induction-principle) applies to a property of natural numbers once it holds at $0$ and passes from each $m$ to $m^+$. Every subset of a finite set is finite by [the finite-subset theorem](https://alphabetamath.cc/item/thm-subset-of-a-finite-set), using the supplied [definition of finiteness](https://alphabetamath.cc/item/def-finite-cardinality).

[F5] In the [integers](https://alphabetamath.cc/item/def-integers) an integer is a class of pairs of naturals representing a difference. The [integer operations](https://alphabetamath.cc/item/def-int-operations) supply addition, negation, $0$ and $1$, and the [integer order](https://alphabetamath.cc/item/def-int-order) compares $[(a,b)]\le[(c,d)]$ by $a+d\le b+c$ in the naturals, where the sums use [natural-number addition](https://alphabetamath.cc/item/def-nat-addition). By [the ordered-ring theorem for the integers](https://alphabetamath.cc/item/thm-int-ordered-ring), addition on the integers is associative and commutative, has identity $0$ and inverse $-i$ at $i$, and preserves $\le$ upon adding the same integer to both sides.

[F6] The natural numeral $1$ is $0^+$ by the [definition of the natural numbers](https://alphabetamath.cc/item/def-natural-numbers), so $0<1$ in $\mathbb N$ by the [successor inequality](https://alphabetamath.cc/item/lem-nat-order-is-membership). The [representative criterion for positivity](https://alphabetamath.cc/item/def-int-order) gives $0<[(a,b)]$ in $\mathbb Z$ exactly when $b<a$ in $\mathbb N$. The integer numeral $1=[(1,0)]$ from the [integer operations](https://alphabetamath.cc/item/def-int-operations) is therefore positive, so the integer values $0$ and $1$ are distinct.

### Proof

**Given:** The finite set $D$, the number of updates $r$, the sets $E_j$, the subset $S$ of the nonnegative integers, and the integer $i$.

**Goal:** Determine every set left by deletion and characterize the integers in $i+S$.

1.1 For $0\le m\le r$, let $A_m=D\setminus U_m$. Each $A_m$ exists and is contained in $D$ by the set difference definition. To form the graph of the family, separate the pairs satisfying $A=D\setminus U_m$ inside $I\times\mathcal P(D)$, where $I=\{m\in\mathbb N:0\le m\le r\}$. The ordered-pair equality criterion makes the index and value of each pair unique. At each $m$ there is exactly one such $A$ by extensionality, so this graph defines a function with domain $I$. [given, F1, F2, F3]

1.2 If $k\in i+S$, then $k=i+s$ for some $s\in S$. Since $0\le s$, addition of $i$ gives $i\le k$. Adding $-i$ to the equality and using the additive laws gives $k-i=s$, so $\varepsilon_{k-i}=1$. [given, F5]

2.1 The union $U_0$ is empty, so $A_0=D$. For $0\le m<r$ the successor $m^+$ lies in $I$. Its prefix of deletion indices consists of the indices from the prefix at $m$ and the single index $m^+$. For a natural number $j$, the inequality $j<m^+$ holds exactly when $j\le m$, and $m^+$ is nonzero since it contains $m$. Thus $x\notin U_{m^+}$ holds exactly when $x\notin U_m$ and $x\notin E_{m^+}$. Membership in $A_{m^+}$ is therefore equivalent to membership in $A_m\setminus E_{m^+}$, so these sets are equal by extensionality. [step 1.1, F1, F3]

3.1 Any family $C$ satisfying the deletion rules must agree with $A$ at $0$. Apply induction to the property that $C_m=A_m$ whenever $m\le r$. If $m^+\le r$, then $m<r$ and the induction hypothesis gives $C_m=A_m$. The update and step 2.1 give $C_{m^+}=C_m\setminus E_{m^+}=A_{m^+}$. If $m^+\le r$ fails, the property at $m^+$ is vacuous. Hence every $C_m$ equals $A_m$ in the required range, and each is finite because it is a subset of the finite set $D$. [given, step 1.1, step 2.1, F1, F4]

4.1 If $k\ge i$ and $\varepsilon_{k-i}=1$, then $k-i\in S$, since outside $S$ the indicator is $0$ and [F6] gives $0\ne1$ in $\mathbb Z$. The additive laws give $k=i+(k-i)$, so $k\in i+S$. This proves the translated-support equivalence, and steps 2.1 and 3.1 give the unique deletion family and its formula at every stage. [given, F5, F6, step 2.1, step 3.1, step 1.2] ∎

---
title: A uniform bound for two-square representations
status: draft
research_item: lem-author-f93d28423212-two-square-multiplicity
dependency_level: 0
---

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)
- [math:def-two-square-representation-function](https://alphabetamath.cc/item/def-two-square-representation-function)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:thm-two-square-representation-count](https://alphabetamath.cc/item/thm-two-square-representation-count)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-divisor-counting-function](https://alphabetamath.cc/item/def-divisor-counting-function)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)
- [math:prop-divisor-functions-under-dirichlet-convolution](https://alphabetamath.cc/item/prop-divisor-functions-under-dirichlet-convolution)
- [math:def-multiplicative-arithmetic-function](https://alphabetamath.cc/item/def-multiplicative-arithmetic-function)
- [math:thm-multiplicative-functions-determined-by-prime-powers](https://alphabetamath.cc/item/thm-multiplicative-functions-determined-by-prime-powers)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)
- [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)
- [math:lem-rational-power-monotone](https://alphabetamath.cc/item/lem-rational-power-monotone)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:def-symmetric-group](https://alphabetamath.cc/item/def-symmetric-group)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:def-arithmetic-function](https://alphabetamath.cc/item/def-arithmetic-function)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)


## Statement

For a positive integer $m$ (an integer greater than $0$), let $r_2(m)$ count the ordered pairs of integers $(u,v)$ with $u^2+v^2=m$, with signs counted separately. Then $r_2(m)\le C m^{1/16}$ for all $m\ge1$, where $C=4\cdot16^{65536}$. Here $m^{1/16}$ is the positive sixteenth root of $m$.

## Facts & Assumptions

[F1] The two-square count is four times the difference between the numbers of positive divisors congruent to $1$ and $3$ modulo $4$, where congruence modulo $4$ means that $4$ divides the difference. The total number of positive divisors is $\tau(m)$. [math:thm-two-square-representation-count](https://alphabetamath.cc/item/thm-two-square-representation-count) [math:def-two-square-representation-function](https://alphabetamath.cc/item/def-two-square-representation-function) [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer) [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z) [math:def-divisor-counting-function](https://alphabetamath.cc/item/def-divisor-counting-function)

[F2] A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Every positive integer has a prime factorization unique up to order. The function $\tau$ is multiplicative and $\tau(p^e)=e+1$ for a prime $p$ and a natural exponent $e$. For a multiplicative arithmetic function, its value at a positive integer is the product of its values on the distinct prime powers in the canonical factorization, with value $1$ for the empty product. [math:def-prime](https://alphabetamath.cc/item/def-prime) [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic) [math:prop-divisor-functions-under-dirichlet-convolution](https://alphabetamath.cc/item/prop-divisor-functions-under-dirichlet-convolution) [math:def-multiplicative-arithmetic-function](https://alphabetamath.cc/item/def-multiplicative-arithmetic-function) [math:thm-multiplicative-functions-determined-by-prime-powers](https://alphabetamath.cc/item/thm-multiplicative-functions-determined-by-prime-powers)

[F3] Integer, real and complex multiplication give commutative monoids with identity $1$. A finite product starts at $1$ and appends one factor at a time. It is unchanged by a permutation (a bijection of the positions) or by grouping into consecutive blocks. Natural powers start at the zeroth power $1$ and multiply by the base at each successor. [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field) [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field) [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:def-symmetric-group](https://alphabetamath.cc/item/def-symmetric-group) [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity) [math:def-group-power](https://alphabetamath.cc/item/def-group-power)

[F4] The naturals $\mathbb N$ include $0$, and their image in the integers is exactly the nonnegative integers. Use the order- and arithmetic-preserving identifications $\mathbb N\subseteq\mathbb Z\subseteq\mathbb Q\subseteq\mathbb R$. The natural order agrees with the integer order on the nonnegative images. In the power estimates the bases and counts are compared in $\mathbb R$, and an exponent $a/b$ denotes the rational represented by $(a,b)$. Rational multiplication multiplies numerators and denominators separately. For positive denominators $b,d$, $a/b\le c/d$ means $ad\le cb$ in the integers. [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers) [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations) [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [math:def-int-order](https://alphabetamath.cc/item/def-int-order) [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)

[F5] Induction on $\mathbb N$ starts at $0$ and passes from each natural to its successor. Natural addition gives $\sigma(t)=t+1$, and this is the immediate successor of $t$ in the natural order. Integer addition, multiplication and negation make the integers a totally ordered commutative ring. Division by $16$ writes an integer uniquely as $16k+r$ with integer $k$ and $0\le r<16$. [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle) [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[F6] For positive real bases, rational powers are positive and agree with natural powers at natural exponents. They obey the product and iterated-power laws. A positive rational exponent gives an increasing function of the base, and a base greater than $1$ gives an increasing function of the rational exponent. The reals form an ordered field, so multiplication by a positive real preserves inequalities. [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power) [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws) [math:lem-rational-power-monotone](https://alphabetamath.cc/item/lem-rational-power-monotone) [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field) [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules)

[F7] A bijection is an injective map onto its target. In particular, an injective map is a bijection onto its image. The cardinality of a finite set is its number of elements and is preserved by a bijection. A subset of a finite set is finite and has at most the cardinality of the containing set. Separation forms the subset of a set consisting of the elements that satisfy a given condition. The natural initial segment $I_h=\{t\in\mathbb N:t<h\}$ has cardinality $h$. [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[F8] The arithmetic functions in [F2] take values in $\mathbb C$. The field embedding $j\colon\mathbb R\to\mathbb C$, $j(a)=a+0i$, is injective and preserves $1$, addition and multiplication. The divisor-counting function sums a copy of $1$ for each positive divisor, so its complex value is $j$ of the real image of that count. [math:def-arithmetic-function](https://alphabetamath.cc/item/def-arithmetic-function) [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field) [math:def-divisor-counting-function](https://alphabetamath.cc/item/def-divisor-counting-function)

## Proof

**Given:** A positive integer $m$.

**Goal:** Bound $r_2(m)$ by $C m^{1/16}$.

1.1 By discreteness and the ordered natural embedding, $m\ge1$. By prime factorization, write $m$ as a product of a finite list of primes. Order its positions by increasing prime value, breaking ties by increasing original index. This ordering is obtained by repeatedly scanning the remaining positions for the least one in that order and removing it. The new list of positions exhausts the original ones and uses each once, giving a permutation. Equal primes now occupy consecutive blocks, and grouping the blocks gives $m=\prod_{i<\ell}p_i^{e_i}$, with distinct primes $p_i$ and positive natural multiplicities $e_i$. For $m=1$ the prime list is empty. If a prime $q$ divides $m$, write $m=qa$. Since $q>0$ and $m>0$, the integer $a$ is positive and hence at least $1$. Factor $a$ and use uniqueness to see that $q$ occurs in the list. [given, F1, F2, F3, F4, F5, F7]

1.2 The positive divisors congruent to $1$ modulo $4$ form a subset of the finite set of all positive divisors of $m$, so their count is at most $\tau(m)$. The count in residue class $3$ is nonnegative. The two-square formula therefore gives $r_2(m)\le4\tau(m)$ in the real order. [given, F1, F4, F6, F7]

2.1 Apply the product formula for multiplicative functions in $\mathbb C$ to $\tau$ and the factorization in step 1.1. The prime-power formula gives $j(\tau(m))=\prod_{i<\ell}j(e_i+1)$, where $\tau(m)$ inside $j$ denotes the real image of the count. Since $j$ preserves $1$ and multiplication, induction on the prefix length rewrites the right side as $j(\prod_{i<\ell}(e_i+1))$. Injectivity gives $\tau(m)=\prod_{i<\ell}(e_i+1)$ in $\mathbb R$, including $\tau(1)=1$. [step 1.1, F1, F2, F3, F4, F5, F8]

2.2 Induct on $e\in\mathbb N$ to prove $e+1\le2^e$. At $e=0$ both sides are $1$. At the successor $\sigma(e)=e+1$, $e+2\le 2(e+1)\le 2\cdot2^e=2^{e+1}$. Use this inequality for the positive exponents of step 1.1. If $p\ge 2^{16}$ and $e>0$, the iterated-power law and monotonicity in the base give $e+1\le2^e=(2^{16})^{e/16}\le p^{e/16}$. [step 1.1, F3, F4, F5, F6]

2.3 Let $S$ be the set of primes $p_i<2^{16}$ in step 1.1. Each prime exceeds $1$ and so is at least $2$ by discreteness. Since $2^{16}=65536$, the map $p\mapsto p-2$ takes $S$ into $I_{65536}$ by $0\le p-2<65536$ and the identification of nonnegative integers with naturals. If $p-2=p'-2$, adding $2$ gives $p=p'$, so this map is a bijection onto its image. The image is a subset of a finite set with $65536$ elements, so $s=|S|\le65536$. [step 1.1, F2, F3, F4, F5, F7]

3.1 For $2\le p<2^{16}$ and $e>0$, divide $e$ by $16$ to get $e=16k+r$ with $0\le r<16$. If $k<0$, then $-k$ is a positive natural under the embedding and is at least $1$, so $16k+r<0$. Thus $k\ge0$, and $16k\le e$ gives $k\le e/16$ in the rational order. Since $r+1\le16$, step 2.2 gives $e+1\le16(k+1)\le16\cdot2^k$. In the reals, monotonicity in the exponent at base $2$ gives $2^k\le 2^{e/16}$, and monotonicity in the base for $e/16>0$ gives $2^{e/16}\le p^{e/16}$. Hence $e+1\le16p^{e/16}$. [step 2.2, F4, F5, F6]

4.1 For each $i<\ell$, let $c_i=16$ if $p_i$ belongs to $S$ and $c_i=1$ otherwise. Steps 2.2 and 3.1 give $e_i+1\le c_i p_i^{e_i/16}$ with positive factors. Multiply by induction on the prefix length, starting with the empty products $1$. For current products $A\le B$ and next factors $a\le b$, one has $Aa\le Ba\le Bb$ by positivity. At each prefix extension, commutativity and associativity move the new coefficient past the preceding prime-power factors. Starting with the empty products, this separates the upper product into $\prod_{i<\ell}c_i$ and $\prod_{i<\ell}p_i^{e_i/16}$. [step 1.1, step 2.2, step 2.3, step 3.1, F3, F5, F6]

5.1 For $k\le\ell$, let $J_k=\{i\in I_k:c_i=16\}$. Induct on $k$ up to $\ell$ to show that there is a natural $h$ with a bijection from $I_h$ to $J_k$ and $\prod_{i<k}c_i=16^h$. At $k=0$ take $h=0$. Both sets are empty and the empty product is $1=16^0$. For $k<\ell$, discreteness gives $I_{k+1}$ by adjoining $k$ to $I_k$. If $c_k=1$, $J_{k+1}=J_k$ and the product is unchanged. If $c_k=16$, $J_{k+1}$ consists of the old elements of $J_k$ and the new element $k$. Extend the old bijection to $I_{h+1}$ by sending its new index $h$ to $k$. This map is injective since $k$ was outside the old image, and surjective since it hits every old element and $k$. The new product is $16^h\cdot16=16^{h+1}$. At $k=\ell$, the map $i\mapsto p_i$ is a bijection from $J_\ell$ to $S$ by distinctness of the primes and the definition of $S$. Thus $h=|J_\ell|=|S|=s$ and $\prod_{i<\ell}c_i=16^s$. [step 1.1, step 2.3, step 4.1, F3, F5, F7]

6.1 Applying the iterated-power law to each $p_i^{e_i/16}=(p_i^{e_i})^{1/16}$ and the two-factor product law at each prefix extension gives $\prod_{i<\ell}p_i^{e_i/16}=m^{1/16}$. The empty case also holds because $1^{1/16}=1$. Thus $\tau(m)\le 16^s m^{1/16}\le16^{65536}m^{1/16}$ by the divisor product, steps 4.1 and 5.1, the bound on $s$, and monotonicity at base $16$. The two-square bound in step 1.2 yields the claim. [step 1.1, step 2.1, step 1.2, step 2.3, step 4.1, step 5.1, F3, F4, F5, F6] ∎

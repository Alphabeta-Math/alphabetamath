---
title: Two-square count as a prime-exponent product
status: published
research_item: lem-two-square-count-from-prime-exponents
dependency_level: 0
---

## Prerequisites

- [math:def-two-square-representation-function](https://alphabetamath.cc/item/def-two-square-representation-function)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-p-adic-valuation](https://alphabetamath.cc/item/def-p-adic-valuation)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:def-complex-numbers-and-arithmetic](https://alphabetamath.cc/item/def-complex-numbers-and-arithmetic)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:def-zero-divisor-and-integral-domain](https://alphabetamath.cc/item/def-zero-divisor-and-integral-domain)
- [math:def-invertible-element](https://alphabetamath.cc/item/def-invertible-element)
- [math:def-divisibility-and-associates-in-a-domain](https://alphabetamath.cc/item/def-divisibility-and-associates-in-a-domain)
- [math:def-irreducible-and-prime-elements-in-a-domain](https://alphabetamath.cc/item/def-irreducible-and-prime-elements-in-a-domain)
- [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)
- [math:thm-fermat-two-square-theorem-for-primes](https://alphabetamath.cc/item/thm-fermat-two-square-theorem-for-primes)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)
- [math:def-subring](https://alphabetamath.cc/item/def-subring)
- [math:lem-field-is-a-commutative-ring](https://alphabetamath.cc/item/lem-field-is-a-commutative-ring)
- [math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice)
- [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:lem-of-q-embeds](https://alphabetamath.cc/item/lem-of-q-embeds)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment)
- [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)
- [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)
- [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)
- [math:def-ring](https://alphabetamath.cc/item/def-ring)
- [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)
- [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules)
- [math:def-choice-function](https://alphabetamath.cc/item/def-choice-function)
- [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)


## Statement

Let $u$ be a positive integer. Write $r_2(u)$ for the number of ordered integer pairs $(x,y)$ with $x^2+y^2=u$, allowing zero coordinates. Two ordered pairs are equal exactly when their first coordinates agree and their second coordinates agree, so every sign change or coordinate swap that changes a coordinate gives a distinct pair. A prime is an integer greater than $1$ with no positive divisors other than $1$ and itself. For a prime $p$, write $e_p$ for the greatest nonnegative integer $e$ for which $p^e$ divides $u$, meaning $u$ is an integer multiple of $p^e$. Write $p\equiv b\pmod 4$ when $p-b$ is a multiple of $4$. Use the natural numbers as nonnegative exponents, with a zeroth power equal to $1$. An integer is even or odd according as its remainder on division by $2$ is $0$ or $1$.

If some prime $q\equiv3\pmod 4$ has odd $e_q$, then $r_2(u)=0$. Otherwise
$$r_2(u)=4\prod_{\substack{p\equiv1\pmod 4\\ e_p>0}}(e_p+1),$$
where the factors range over the indicated primes in increasing prime order. There are finitely many such primes because each is a prime divisor of $u$, and integer prime factorization has finite support. The product is taken in $\mathbb N$, and $e_p+1$ is the successor of $e_p$. For an integer reading of the equality, identify each natural number with its nonnegative integer image. A product with no factors is $1$.

## Statement references

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

## Facts & Assumptions

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

## Proof

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

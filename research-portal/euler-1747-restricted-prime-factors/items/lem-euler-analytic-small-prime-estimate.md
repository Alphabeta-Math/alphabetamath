---
id: lem-euler-analytic-small-prime-estimate
kind: lemma
title: Small-prime contribution above the analytic threshold
status: draft
domain: mathematics
proof_strategy: direct
deps:
  - math:def-axiom-of-choice
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - def-euler-prime-classes
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - def-euler-divisor-functions
  - math:def-real-numbers
  - math:def-ordered-field
  - math:def-integer-power
  - math:def-rational-power
  - math:def-finite-cardinality
  - math:def-sum-over-a-finite-index-set
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-of-q-embeds
  - math:thm-reals-ordered-field
  - math:lem-of-inverse-positive
  - math:lem-rational-power-laws
  - math:lem-rational-power-monotone
  - math:lem-cauchy-reals-archimedean
  - math:lem-cardinality-of-finite-natural-initial-segment
  - math:thm-subset-of-a-finite-set
  - math:def-finite-sum
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-finite-sum-laws
  - math:lem-finite-sum-reindexing-and-fubini
  - math:lem-nat-finite-sum-laws-and-the-canonical-embedding
  - math:def-series
  - math:thm-nonnegative-series-bounded-partial-sums
  - prop-euler-uniform-prime-obstruction
  - lem-euler-obstructing-prime-count
  - lem-euler-obstructing-prime-density-sum
  - lem-euler-arithmetic-factor-bounds
  - math:def-natural-numbers
  - math:def-rationals
  - math:def-field
  - math:def-subset-and-proper-subset
  - math:def-nat-finite-sum-and-product
  - math:def-canonical-natural
  - math:def-injection-surjection-bijection
  - math:thm-nth-roots-exist
  - math:cor-cauchy-reals-lub-complete
  - math:def-complete-ordered-field
  - math:def-rat-order
  - math:def-nat-order
  - math:def-semigroup-and-monoid
formulation_deps:
  - math:def-axiom-of-choice
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - def-euler-prime-classes
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - def-euler-divisor-functions
  - math:def-real-numbers
  - math:def-ordered-field
  - math:def-integer-power
  - math:def-rational-power
  - math:def-finite-cardinality
  - math:def-sum-over-a-finite-index-set
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-of-q-embeds
  - math:def-natural-numbers
  - math:def-rationals
  - math:def-field
  - math:def-subset-and-proper-subset
  - math:thm-nth-roots-exist
argument_deps:
  - math:def-axiom-of-choice
  - def-euler-prime-classes
  - def-euler-divisor-functions
  - math:def-ordered-field
  - math:def-rational-power
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-of-q-embeds
  - math:thm-reals-ordered-field
  - math:lem-of-inverse-positive
  - math:lem-rational-power-laws
  - math:lem-rational-power-monotone
  - math:lem-cauchy-reals-archimedean
  - math:lem-cardinality-of-finite-natural-initial-segment
  - math:thm-subset-of-a-finite-set
  - math:def-finite-sum
  - math:def-sum-over-a-finite-index-set
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-finite-sum-laws
  - math:lem-finite-sum-reindexing-and-fubini
  - math:lem-nat-finite-sum-laws-and-the-canonical-embedding
  - math:def-series
  - math:thm-nonnegative-series-bounded-partial-sums
  - prop-euler-uniform-prime-obstruction
  - lem-euler-obstructing-prime-count
  - lem-euler-obstructing-prime-density-sum
  - lem-euler-arithmetic-factor-bounds
  - math:def-natural-numbers
  - math:def-rationals
  - math:def-field
  - math:def-subset-and-proper-subset
  - math:def-nat-finite-sum-and-product
  - math:def-canonical-natural
  - math:def-injection-surjection-bijection
  - math:thm-nth-roots-exist
  - math:cor-cauchy-reals-lub-complete
  - math:def-complete-ordered-field
  - math:def-rat-order
  - math:def-nat-order
  - math:def-semigroup-and-monoid
  - math:def-finite-cardinality
dependency_roles:
  math:def-axiom-of-choice: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  def-euler-four-square-representations: mathematical-premise
  def-euler-mixed-four-square-representations: mathematical-premise
  def-euler-prime-obstruction-count: mathematical-premise
  def-euler-divisor-functions: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:def-ordered-field: mathematical-premise
  math:def-integer-power: mathematical-premise
  math:def-rational-power: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-of-q-embeds: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:lem-of-inverse-positive: mathematical-premise
  math:lem-rational-power-laws: mathematical-premise
  math:lem-rational-power-monotone: mathematical-premise
  math:lem-cauchy-reals-archimedean: mathematical-premise
  math:lem-cardinality-of-finite-natural-initial-segment: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-finite-sum: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:lem-finite-sum-laws: mathematical-premise
  math:lem-finite-sum-reindexing-and-fubini: mathematical-premise
  math:lem-nat-finite-sum-laws-and-the-canonical-embedding: mathematical-premise
  math:def-series: mathematical-premise
  math:thm-nonnegative-series-bounded-partial-sums: mathematical-premise
  prop-euler-uniform-prime-obstruction: mathematical-premise
  lem-euler-obstructing-prime-count: mathematical-premise
  lem-euler-obstructing-prime-density-sum: mathematical-premise
  lem-euler-arithmetic-factor-bounds: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-rationals: mathematical-premise
  math:def-field: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-nat-finite-sum-and-product: mathematical-premise
  math:def-canonical-natural: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:thm-nth-roots-exist: mathematical-premise
  math:cor-cauchy-reals-lub-complete: mathematical-premise
  math:def-complete-ordered-field: mathematical-premise
  math:def-rat-order: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:def-semigroup-and-monoid: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 6, Proposition 6.1, choice of cutoff and equation (6.1)
      reading_limits: Read the cutoff and equation (6.1) on PDF page 6 for attribution.
dependency_level: 13
---

## Statement

Assume the Axiom of Choice, which gives a function selecting one member from each set in any family of nonempty sets. Let $m$ be a positive odd integer, so $m=2j+1>0$ for an integer $j$, and let $n=2m\ge64^4$. An integer $d$ divides $u$ when $u=dq$ for an integer $q$. A prime is an integer $p>1$ whose only positive divisors are $1$ and $p$. Let $\mathcal P_3$ be the set of primes congruent to $3$ modulo $4$, meaning that $4$ divides $p-3$. Suppose every prime divisor of $m$ belongs to $\mathcal P_3$.

Let $R(n)$ count the ordered integer quadruples $(x_1,x_2,x_3,x_4)$ satisfying $x_1^2+x_2^2+x_3^2+x_4^2=n$, allowing both signs and zero. For $p\in\mathcal P_3$, let $b_p(n)$ count the quadruples counted by $R(n)$ with one even and one odd coordinate in each of the pairs $(x_1,x_2)$ and $(x_3,x_4)$ and with $p$ dividing both coordinates of at least one of these pairs. An even integer has the form $2j$ for an integer $j$. Each qualifying quadruple contributes once. Let $\tau(m)$ be the number of positive divisors of $m$ and $\sigma(m)$ their sum.

Evaluate the fractions and powers in the ordered field of real numbers, using the inclusions of natural numbers, integers and rationals into the reals. For $a>0$ and a rational exponent $u/v$ with integer numerator $u$ and positive integer denominator $v$, $a^{u/v}$ is the $u$-th integer power of the positive $v$-th root of $a$. Nonnegative integer powers use repeated multiplication with $a^0=1$, and negative powers use reciprocals. Thus $\sqrt m=m^{1/2}$. Set $X=n^{1/4}$ and $P=2X$. A sum over a finite set adds one term per element, starting at zero.

Then $X\ge64$, the index set $\{p\in\mathcal P_3:p\le P\}$ is finite, $R(n)>0$, and
$$\frac{1}{R(n)}\sum_{\substack{p\le P\\p\in\mathcal P_3}}b_p(n)\le\frac{21}{50}+\frac{\tau(m)\sqrt m}{3\sigma(m)}\left(\frac{4X}{15}+1\right)\le\frac{21}{50}+\frac{23}{30}2^{3/10}X^{-1/5}\left(\frac4{15}+\frac1X\right).$$

## Statement references

[[math:def-axiom-of-choice]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-divides-in-z]]

[[math:def-prime]]

[[math:def-congruence-modulo-an-integer]]

[[def-euler-prime-classes]]

[[def-euler-four-square-representations]]

[[def-euler-mixed-four-square-representations]]

[[def-euler-prime-obstruction-count]]

[[def-euler-divisor-functions]]

[[math:def-real-numbers]]

[[math:def-ordered-field]]

[[math:def-integer-power]]

[[math:def-rational-power]]

[[math:thm-nth-roots-exist]]

[[math:def-finite-cardinality]]

[[math:def-sum-over-a-finite-index-set]]

[[math:lem-nat-embeds-int]]

[[math:lem-int-embeds-rat]]

[[math:lem-of-q-embeds]]

[[math:def-natural-numbers]]

[[math:def-rationals]]

[[math:def-field]]

[[math:def-subset-and-proper-subset]]

## Facts & Assumptions

[F1] The real numbers form a totally ordered field. Its addition and multiplication obey the field laws, and division by a nonzero number is multiplication by its inverse. Addition preserves comparisons, and multiplication by a nonnegative number preserves weak inequalities. A positive real has a positive reciprocal. The inclusions of the natural numbers into the integers, the integers into the rationals, and the rationals into the reals preserve addition, multiplication and order. The nonnegative integers are exactly the images of the natural numbers, each with a unique natural preimage. The inclusions are injective and order-preserving, so they reflect strict order. The real numbers are also a complete ordered field, meaning that every nonempty set of reals that is bounded above has a least upper bound. [[math:thm-reals-ordered-field]] [[math:def-complete-ordered-field]] [[math:cor-cauchy-reals-lub-complete]] [[math:def-ordered-field]] [[math:def-field]] [[math:def-natural-numbers]] [[math:def-rationals]] [[math:lem-of-inverse-positive]] [[math:lem-nat-embeds-int]] [[math:lem-int-embeds-rat]] [[math:lem-of-q-embeds]]

[F2] Over the complete ordered field of [F1], for $a>0$ and a natural number $v\ge1$, there is a unique positive $v$-th root $t$ with $t^v=a$. For positive bases $a,b$ and rational exponents $r,s$, powers are positive, $a^{r+s}=a^ra^s$, $(ab)^r=a^rb^r$, $(a^r)^s=a^{rs}$, and $a^{-r}=1/a^r$. A rational $r$ with a positive denominator satisfies $r>0$ exactly when its numerator is positive. If $r>0$, the value of $a^r$ increases strictly as $a$ increases. For an integer exponent $u$, use the representative $u/1$ and the fact that the first root of $a$ is $a$ to recover its integer power. [[math:def-rationals]] [[math:def-rat-order]] [[math:def-rational-power]] [[math:thm-nth-roots-exist]] [[math:lem-rational-power-laws]] [[math:lem-rational-power-monotone]]

[F3] Let $K$ be finite, with $k=|K|$, and choose a bijection $\varphi:I_k\to K$, where $I_k$ consists of the natural numbers $j<k$. For a real or natural summand $a$ on $K$, put $a'_j=a_{\varphi(j)}$ when $j<k$ and $a'_j=0$ for $j\ge k$. The set-indexed sum is the recursive sum $\sum_{j<k}a'_j$ in the corresponding number system and is independent of $\varphi$. Using the same $\varphi$ for all summands preserves their termwise comparisons, sums and scalar multiples on $I_k$. The initial-segment laws thus give monotonicity, additivity and scaling for finite real sums, the sum $kc$ for a constant real summand $c$, and the bound of each term by its finite natural sum. The natural-to-real sum identity applied to $a'$ also shows that embedding a finite natural sum gives the real sum of the embedded terms. Here the canonical natural-to-real map agrees with the composite inclusion of [F1], since both send $0$ to $0$ and send each successor $j+1$ to the image of $j$ plus $1$. A bijection transports cardinality and finiteness. For finite sets it also preserves the sum when the summand is pulled back along the bijection. In the real field of [F1], addition is associative and commutative with identity $0$, so the reals with addition and identity $0$ form a commutative monoid. When each index belongs to exactly one of two subsets, the splitting law for this monoid gives the sum over the whole set as the sum over its two subsets. This monoid sum agrees with the set-indexed real sum used here. [[math:def-finite-cardinality]] [[math:def-nat-order]] [[math:def-field]] [[math:def-semigroup-and-monoid]] [[math:def-injection-surjection-bijection]] [[math:def-sum-over-a-finite-index-set]] [[math:def-finite-sum]] [[math:def-nat-finite-sum-and-product]] [[math:lem-finite-sum-laws]] [[math:lem-nat-finite-sum-laws-and-the-canonical-embedding]] [[math:def-canonical-natural]] [[math:def-finite-sum-in-a-commutative-monoid]] [[math:lem-finite-sum-reindexing-and-fubini]]

[F4] By separation, the members of a given set satisfying a specified condition form a subset of that set. For every real $t$, some natural number $H$ satisfies $H>t$. For a natural number $H$, the set $I_H$ of natural numbers $k<H$ is finite, and every subset of a finite set is finite. [[math:def-natural-numbers]] [[math:def-subset-and-proper-subset]] [[math:lem-cauchy-reals-archimedean]] [[math:def-nat-order]] [[math:lem-cardinality-of-finite-natural-initial-segment]] [[math:thm-subset-of-a-finite-set]]

[F5] Under the Axiom of Choice, for $n=2m$ with $m$ a positive odd integer all of whose prime divisors lie in $\mathcal P_3$, one has $R(n)>0$ and for every $p\in\mathcal P_3$ one has
$$\frac{b_p(n)}{R(n)}\le\frac{2}{p(p-1)}+\mathbf 1_{p>3}\frac{\tau(m)\sqrt m}{3\sigma(m)},$$
where $\mathbf 1_{p>3}$ is $1$ for $p>3$ and $0$ otherwise. [[prop-euler-uniform-prime-obstruction]]

[F6] At any real $t\ge0$, the number of primes in $\mathcal P_3$ with $3<p\le t$ is at most $2t/15+1$. [[lem-euler-obstructing-prime-count]]

[F7] For each natural index $k$, test membership in $\mathcal P_3$ using its integer image under [F1]. Set $u_k=1/[k(k-1)]$ when that image is in $\mathcal P_3$ and $u_k=0$ otherwise. The series, meaning the limit of the finite sums $\sum_{k<H}u_k$ as $H$ tends to infinity, converges to a value $L$ with $2L<21/50$. Since each term is nonnegative, every partial sum is bounded above by the series sum, which is the least upper bound of these partial sums. [[def-euler-prime-classes]] [[math:def-natural-numbers]] [[math:def-field]] [[math:lem-nat-embeds-int]] [[math:def-series]] [[lem-euler-obstructing-prime-density-sum]] [[math:thm-nonnegative-series-bounded-partial-sums]]

[F8] If $n=2m$ for positive odd $m$ with all prime divisors in $\mathcal P_3$, then $\tau(m)m/\sigma(m)\le(23/10)m^{1/5}$. The two divisor functions here count and sum the positive divisors, respectively. [[def-euler-divisor-functions]] [[lem-euler-arithmetic-factor-bounds]]

## Proof

**Given:** The Axiom of Choice and $n=2m\ge64^4$, with $m$ positive and odd and each prime divisor of $m$ in $\mathcal P_3$. Set $X=n^{1/4}$ and $P=2X$.

**Goal:** Establish the cutoff properties and both bounds on the sum of the counts $b_p(n)$ for $p\in\mathcal P_3$ with $p\le P$, divided by $R(n)$.

1.1 The exponent $1/4$ is positive by [F2], so the fourth root increases on positive numbers, and $64$ is the positive fourth root of $64^4$ by uniqueness in [F2]. Thus $X\ge64$. By the root equation in [F2], $X^4=n$, hence $m=X^4/2$, and $P=2X>0$. The hypotheses on $m,n$ and the Axiom of Choice give $R(n)>0$ by [F5]. The positive divisors of $m$ form a finite set by [[def-euler-divisor-functions]]. Since $m=1\cdot m$, the term $1$ appears in any listing of that set, so the natural sum bound in [F3] gives $\sigma(m)\ge1$. The number $C=\frac{\tau(m)\sqrt m}{3\sigma(m)}$ is nonnegative since $\tau(m)$ is a natural number, $\sqrt m>0$ and the denominator is positive. [given, F1, F2, F3, F5]

2.1 Choose a natural number $H>P$ by [F4]. By separation form $S=\{p\in\mathcal P_3:p\le P\}$ and $T=\{p\in S:p>3\}$. Each prime in $S$ is a positive integer, so by [F1] it is the image of a unique natural number. From here on, identify $S$ and $T$ with their sets of natural preimages. Since the inclusions preserve and reflect strict order, each such natural index is $<H$ because its real image is $\le P<H$. Thus $T\subseteq S\subseteq I_H$. By separation also form $U=\{p\in S:p\notin T\}$ and $V=\{k\in I_H:k\notin S\}$. Each of $S,T,U,V$ is finite by [F4]. The embedding gives bijections back to the integer prime sets, so those sets are finite and we can use the same cardinalities and sums by [F3]. Each index of $S$ belongs to exactly one of $T$ and $U$, and each index of $I_H$ belongs to exactly one of $S$ and $V$. Applying [F6] with $t=P>0$ gives $|T|\le2P/15+1=4X/15+1$. [given, F1, F3, F4, F6, step 1.1]

2.2 Multiply the bound of [F8] by the positive number $1/(3\sqrt m)$. Using $m/\sqrt m=\sqrt m$ and the power laws of [F2] gives $C\le\frac{23}{30}\frac{m^{1/5}}{m^{1/2}}=\frac{23}{30}m^{-3/10}=\frac{23}{30}2^{3/10}X^{-6/5}$. For the last equality, $m=X^4\cdot 2^{-1}$ with both factors positive, so $m^{-3/10}=(X^4)^{-3/10}(2^{-1})^{-3/10}$. [given, F1, F2, F8, step 1.1]

3.1 For all $p\in S$, apply [F5] to this $m,n$ and the integer prime represented by $p$. This gives $b_p(n)/R(n)\le 2u_p+\mathbf 1_{p>3}C$ with $u_p$ from [F7]. Read each count $b_p(n)$ in the reals. By the sum identity in [F3], the real sum of these embedded counts is the image of the natural sum in the Statement. Monotonicity, additivity and scaling in [F3] therefore give $\frac{1}{R(n)}\sum_{p\in S}b_p(n)\le2\sum_{p\in S}u_p+C\sum_{p\in S}\mathbf 1_{p>3}$. [given, F1, F3, F5, F7, step 1.1, step 2.1]

4.1 The indicator is $1$ on $T$ and $0$ on $U$. Since every index of $S$ belongs to exactly one of $T$ and $U$, [F3] gives $\sum_{p\in S}\mathbf 1_{p>3}=|T|\cdot1+|U|\cdot0=|T|$. Thus the right side of step 3.1 equals $2\sum_{p\in S}u_p+C|T|$. [F1, F3, F5, step 2.1, step 3.1]

5.1 For every natural $k$, the term $u_k$ is nonnegative. It is zero off the prime class, and for a prime $k>1$ its denominator $k(k-1)$ is positive. Using the identification in step 2.1, every natural index in $I_H$ belongs to exactly one of $S$ and $V$. Thus $\sum_{k<H}u_k=\sum_{p\in S}u_p+\sum_{k\in V}u_k$ by [F3], using the identity enumeration of $I_H$ for the sum on the left. The sum over $V$ is nonnegative by [F3]. It follows from [F7] that $2\sum_{p\in S}u_p\le2\sum_{k<H}u_k\le2L<21/50$. Use this upper bound and the bound for $|T|$ multiplied by $C\ge0$ in step 4.1. This gives the first weak inequality in the Statement. [F1, F3, F4, F7, step 1.1, step 2.1, step 4.1]

6.1 Since $X>0$, the factor $4X/15+1$ is positive and equals $X(4/15+1/X)$. Multiply the bound of step 2.2 by that factor and use $X^{-6/5}X=X^{-1/5}$. This bounds $21/50+C(4X/15+1)$ by the final expression in the Statement. Together with steps 1.1, 2.1 and 5.1 this proves the assertion. [F1, F2, step 1.1, step 2.1, step 5.1, step 2.2] ∎

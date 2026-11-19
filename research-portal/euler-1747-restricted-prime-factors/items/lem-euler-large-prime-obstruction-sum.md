---
id: lem-euler-large-prime-obstruction-sum
kind: lemma
title: "Lemma 4.2: Aggregated large-prime lattice estimate"
status: draft
domain: mathematics
deps:
  - def-euler-prime-classes
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - def-euler-two-square-counts
  - math:def-integers
  - math:def-complete-ordered-real-field
  - math:def-field
  - math:lem-int-embeds-rat
  - math:lem-of-q-embeds
  - math:lem-nat-embeds-int
  - math:thm-of-square-roots
  - math:def-finite-cardinality
  - math:def-natural-numbers
  - math:def-sequence
  - math:def-finite-sum
  - math:def-sum-over-a-finite-index-set
  - math:def-series
  - math:def-real-limit
  - lem-euler-large-prime-obstruction-per-prime
  - lem-euler-four-square-count-lower-bound
  - math:lem-nat-order-is-membership
  - math:def-subset-and-proper-subset
  - math:thm-subset-of-a-finite-set
  - math:lem-of-sign-rules
  - math:lem-of-inverse-positive
  - math:lem-finite-sum-laws
  - math:lem-finite-sum-reindexing-and-fubini
  - math:thm-nonnegative-series-bounded-partial-sums
  - math:def-int-operations
  - math:def-int-order
  - math:def-rationals
  - math:def-rat-order
  - lem-square-residue-parity
  - math:def-semigroup-and-monoid
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-nat-order
  - math:def-nat-addition
formulation_deps:
  - def-euler-prime-classes
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - def-euler-two-square-counts
  - math:def-integers
  - math:def-complete-ordered-real-field
  - math:def-field
  - math:lem-int-embeds-rat
  - math:lem-of-q-embeds
  - math:lem-nat-embeds-int
  - math:thm-of-square-roots
  - math:def-finite-cardinality
  - math:def-natural-numbers
  - math:def-sequence
  - math:def-finite-sum
  - math:def-sum-over-a-finite-index-set
  - math:def-series
  - math:def-real-limit
  - math:def-int-operations
  - math:def-int-order
  - math:def-rationals
  - math:def-rat-order
  - math:def-nat-order
argument_deps:
  - def-euler-prime-classes
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - def-euler-two-square-counts
  - math:def-integers
  - math:def-complete-ordered-real-field
  - math:def-field
  - math:lem-int-embeds-rat
  - math:lem-of-q-embeds
  - math:lem-nat-embeds-int
  - math:thm-of-square-roots
  - math:def-finite-cardinality
  - math:def-natural-numbers
  - math:def-sequence
  - math:def-finite-sum
  - math:def-sum-over-a-finite-index-set
  - math:def-series
  - math:def-real-limit
  - lem-euler-large-prime-obstruction-per-prime
  - lem-euler-four-square-count-lower-bound
  - math:lem-nat-order-is-membership
  - math:def-subset-and-proper-subset
  - math:thm-subset-of-a-finite-set
  - math:lem-of-sign-rules
  - math:lem-of-inverse-positive
  - math:lem-finite-sum-laws
  - math:lem-finite-sum-reindexing-and-fubini
  - math:thm-nonnegative-series-bounded-partial-sums
  - math:def-int-operations
  - math:def-int-order
  - math:def-rationals
  - math:def-rat-order
  - lem-square-residue-parity
  - math:def-semigroup-and-monoid
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-nat-order
  - math:def-nat-addition
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  def-euler-four-square-representations: mathematical-premise
  def-euler-mixed-four-square-representations: mathematical-premise
  def-euler-prime-obstruction-count: mathematical-premise
  def-euler-two-square-counts: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-complete-ordered-real-field: mathematical-premise
  math:def-field: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-of-q-embeds: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:thm-of-square-roots: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-sequence: mathematical-premise
  math:def-finite-sum: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:def-series: mathematical-premise
  math:def-real-limit: mathematical-premise
  lem-euler-large-prime-obstruction-per-prime: mathematical-premise
  lem-euler-four-square-count-lower-bound: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:lem-of-sign-rules: mathematical-premise
  math:lem-of-inverse-positive: mathematical-premise
  math:lem-finite-sum-laws: mathematical-premise
  math:lem-finite-sum-reindexing-and-fubini: mathematical-premise
  math:thm-nonnegative-series-bounded-partial-sums: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-rationals: mathematical-premise
  math:def-rat-order: mathematical-premise
  lem-square-residue-parity: mathematical-premise
  math:def-semigroup-and-monoid: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:def-nat-addition: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: PDF p. 5, Lemma 4.2, equation (4.1) and its proof
dependency_level: 5
---

## Statement

Let $n=2m$ with $m$ a positive odd integer. An integer is positive if it exceeds $0$ and odd if it has the form $2j+1$ for an integer $j$. An integer $d$ divides $a$, written $d\mid a$, if $a=dk$ for an integer $k$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Write $\mathcal P_3$ for the primes $p$ with $4\mid(p-3)$ and assume every prime dividing $m$ belongs to $\mathcal P_3$.

A representation of $n$ by four squares is an ordered quadruple $(x_1,x_2,x_3,x_4)$ of integers with $x_1^2+x_2^2+x_3^2+x_4^2=n$, where $x^2=x\cdot x$. Each entry may have either sign or be zero. Let $R(n)$ count these quadruples. An even integer has the form $2j$ for an integer $j$. For $p\in\mathcal P_3$, let $b_p(n)$ count the quadruples with one even and one odd entry in each of $(x_1,x_2)$ and $(x_3,x_4)$ and with at least one of these pairs having both entries divisible by $p$. Each qualifying quadruple contributes once.

For each integer $u$ with $1\le u\le n$, multiply the factors $e+1$ over the primes $q$ with $4\mid(q-1)$ whose powers satisfy $q^e\mid u$ and $q^{e+1}\nmid u$ for an integer $e\ge1$. The power $q^e$ is the product of $e$ copies of $q$, the symbol $\nmid$ means failure of divisibility, and an empty product is $1$. Let $M(n)$ be the largest of the resulting products as $u$ varies.

Use the real numbers with the integers and natural-number counts included by their usual arithmetic- and order-preserving maps. For nonzero $b$, the quotient $a/b$ is $a$ times the reciprocal of $b$. Write $\sqrt n$ for the unique nonnegative real with square $n$. For a finite set $S$, write $\#S$ for its number of elements. A finite sum adds each indexed term once, with value $0$ when there are no terms.

For every real $P\ge3$, the obstruction sum on the left below has only finitely many nonzero terms. The reciprocal-square sum on the right is the series of the sequence $(a_k)$ indexed by the natural numbers $k=0,1,2,\ldots$, with $a_k=1/k^2$ for $k>P$ and $k\in\mathcal P_3$, and $a_k=0$ otherwise. Its value is the limit of the partial sums $\sum_{k<N}a_k$, where a limit $T$ means that for every rational $\varepsilon>0$ the absolute difference from $T$ is less than $\varepsilon$ for all sufficiently large $N$. The absolute value of a real number is the number itself when it is nonnegative and its negative otherwise. Then
$$\frac1{R(n)}\sum_{\substack{p>P\\p\in\mathcal P_3}} b_p(n)\le\frac43M(n)\left(\sum_{\substack{p>P\\p\in\mathcal P_3}}\frac1{p^2}+\frac{\#\{p\in\mathcal P_3:P<p\le\sqrt n\}}{n}\right).$$

## Facts & Assumptions

[F1] The real numbers form a field with a total order compatible with addition and multiplication and the least-upper-bound property, which says that every nonempty set of reals with an upper bound has a smallest upper bound. In particular, addition preserves inequalities, multiplication by a positive real preserves their direction, and reciprocation reverses the order on positive reals and gives positive reciprocals. The rationals embed in the reals by a map that preserves arithmetic and order. The usual inclusion of the integers composes $k\mapsto k/1$ into the rationals with this rational-to-real embedding. Write $\eta$ for this integer-to-real map. It sends $0$ to $0$ and $1$ to $1$, and preserves addition, multiplication and strict order. [[math:def-complete-ordered-real-field]] [[math:def-field]] [[math:lem-of-sign-rules]] [[math:lem-of-inverse-positive]] [[math:lem-int-embeds-rat]] [[math:lem-of-q-embeds]]

[F2] Use the usual integer addition, negation, multiplication and order. The natural numbers identify with the nonnegative integers by an arithmetic- and order-preserving inclusion. For natural numbers, $k\le n$ means that $k+d=n$ for some natural $d$, and $k<n$ means $k\le n$ and $k\ne n$. With $\sigma$ denoting the natural-number successor, $1=\sigma(0)$ and natural addition give $n+1=n+\sigma(0)=\sigma(n+0)=\sigma(n)$. The natural number $N$ is the finite set of the natural numbers $k<N$. Hence $k\le n$ holds exactly when $k<n+1$. For natural numbers, being at most another natural number is equivalent to being a subset of it. A condition on elements of a given set selects a unique subset, and a subset of a finite set is finite. Counts of finite sets are natural numbers. [[math:def-integers]] [[math:def-int-operations]] [[math:def-int-order]] [[math:lem-nat-embeds-int]] [[math:def-natural-numbers]] [[math:def-nat-order]] [[math:def-nat-addition]] [[math:lem-nat-order-is-membership]] [[math:def-finite-sum]] [[math:def-subset-and-proper-subset]] [[math:thm-subset-of-a-finite-set]] [[math:def-finite-cardinality]]

[F3] For $n=2m$ with $m>0$ and no integer $q$ satisfying $m=2q$, the full count $R(n)$ of signed, ordered four-square representations is finite and is at least $12n$. [[def-euler-four-square-representations]] [[lem-euler-four-square-count-lower-bound]]

[F4] For $n=2m$ with $m$ a positive odd integer and any $p\in\mathcal P_3$, the obstruction count in the Statement is finite and satisfies $b_p(n)\le16M(n)(n/p^2+1)$. If $b_p(n)>0$, then $p\le\sqrt n$. [[def-euler-prime-classes]] [[def-euler-mixed-four-square-representations]] [[def-euler-prime-obstruction-count]] [[lem-euler-large-prime-obstruction-per-prime]]

[F5] The products in the definition of $M(n)$ are finite and the maximum exists for every positive integer $n$. For each eligible $u$, the product of its factors $e+1$ starts at the integer $1$ and multiplies by the factors in increasing order of their primes. [[def-euler-two-square-counts]]

[F6] Each nonnegative real $x$ has a unique nonnegative square root in the complete ordered real field, meaning the nonnegative real whose square is $x$. [[math:thm-of-square-roots]] [[math:def-complete-ordered-real-field]]

[F7] A finite sum starts at zero and adds its terms along any listing of the indices with each index occurring once. For the natural-number index set $N$, this agrees with $\sum_{k<N}$. Over a finite set $S$, a constant term $c$ sums to $(\#S)c$. For applying sequence laws to a finite list, extend the list by zeros for sums or by ones for products. For a real sequence $(v_j)$, the running product $Q_j$ is uniquely determined by $Q_0=1$ and $Q_{j+1}=Q_jv_j$. [[math:def-finite-sum]] [[math:def-sum-over-a-finite-index-set]]

[F8] Finite sums of real sequences preserve termwise order and allow addition and multiplication by a real constant to pass through the sum. For a real sequence $(c_k)$, the sum of $c_{k+1}-c_k$ over $k<N$ is $c_N-c_0$. The finite product of positive real terms is positive, including the empty product $1$. [[math:lem-finite-sum-laws]]

[F9] If a finite set of indices splits into two disjoint sets, meaning that they have no common index, the sum over the whole set is the sum of the two separate sums. Field addition is a binary operation on $\mathbb R$ and is associative and commutative with identity $0$, so $(\mathbb R,+,0)$ is a commutative monoid. For this operation the commutative-monoid sum agrees with the real sum in [F7], since both start at $0$ and use the same recursion along a listing. [[math:lem-finite-sum-reindexing-and-fubini]] [[math:def-finite-sum-in-a-commutative-monoid]] [[math:def-semigroup-and-monoid]] [[math:def-field]]

[F10] A real sequence assigns one real term to each natural-number index, and its series sums to the limit of its partial sums when that limit exists. For nonnegative terms, a common real upper bound for all partial sums guarantees convergence. In that case the sum is their least upper bound, so it is at least every partial sum. [[math:def-sequence]] [[math:def-series]] [[math:def-real-limit]] [[math:thm-nonnegative-series-bounded-partial-sums]]

[F11] The forms $2q$ and $2j+1$, with $q,j$ integers, are mutually exclusive for any given integer. [[lem-square-residue-parity]]

## Proof

**Given:** A positive odd integer $m$ all of whose prime divisors are in $\mathcal P_3$, with $n=2m$, and a real $P\ge3$.

**Goal:** Show that both sums in the Statement are defined and prove the asserted inequality.

1.1 From $m>0$ we have $n>0$. Its natural-number representative is nonzero and therefore contains $0$. Thus $1=\{0\}$ is a subset of that natural number, giving $n\ge1$. Since $m=2j+1$ for some integer $j$, parity disjointness in [F11] excludes $m=2q$ for any integer $q$. Thus [F3] gives $R(n)\ge12n>0$. Put $s=\sqrt n$, which exists by [F6]. If $s>n$, then $(s-n)(s+n)>0$, so $n=s^2>n^2\ge n$, a contradiction. Thus $s\le n$. Set $S=\{p\in\mathcal P_3:P<p\le s\}$. Every $p\in S$ is a positive integer at most $n$ and so is identified with a member of the finite initial segment $n+1$. Thus $S$ is finite. For $p\in\mathcal P_3$ with $p>P$ and $p\notin S$, [F4] and $b_p(n)\ge0$ give $b_p(n)=0$. Consequently the left sum equals $\sum_{p\in S}b_p(n)$. [given, F1, F2, F3, F4, F6, F7, F11]

1.2 Fix an integer $u$ with $1\le u\le n$. Let $L$ be the number of factors for $u$ in [F5], and let $f_j$ be the $j$th factor for $0\le j<L$, indexed from zero in that order. Set $f_j=1$ for $j\ge L$. Let $I_j$ be the integer product of the first $j$ factors for $j\le L$, and set $I_j=I_L$ for $j>L$. Then $I_0=1$ and $I_{j+1}=I_j f_j$ for every natural $j$, by [F5] for $j<L$ and because $f_j=1$ for $j\ge L$. By [F1], $\eta(I_0)=1$ and $\eta(I_{j+1})=\eta(I_j)\eta(f_j)$. By the uniqueness in [F7], $\eta(I_L)$ is the real product of the first $L$ terms of the sequence $(\eta(f_j))$. Each factor $f_j=e+1$ for $j<L$ has $e\ge1$, so $\eta(f_j)=\eta(e)+1\ge2>0$ by [F1]. Thus [F8] gives $\eta(I_L)>0$, including when $L=0$. Since $I_L$ is the product for $u$ and [F5] gives an attained maximum, $\eta(M(n))>0$. [F1, F2, F5, F7, F8]

1.3 To bound the partial sums of $(a_k)$, put $c_0=c_1=1$ and $c_k=1/(k-1)$ for $k\ge2$. Every $c_k$ is positive. For $k=0,1$ we have $a_k=0=c_k-c_{k+1}$. For $k\ge2$, the choice of $a_k$ gives $0\le a_k\le1/k^2$, and $0<k(k-1)\le k^2$ gives $1/k^2\le 1/(k(k-1))=c_k-c_{k+1}$. Thus the finite-sum comparison and the cancellation of consecutive differences give $0\le\sum_{k<N}a_k\le c_0-c_N\le1$ for every natural number $N$. [given, F1, F2, F7, F8, F10]

2.1 Using the inclusions in [F1], read the counts and the lower bound $R(n)\ge12n$ in the reals. For each $p\in S$, divide [F4] by $12n>0$. Also $b_p(n)/R(n)\le b_p(n)/(12n)$ because $b_p(n)\ge0$ and $R(n)\ge12n>0$. The upper bound is $16M(n)(n/p^2+1)/(12n)$, which equals $(4M(n)/3)(1/p^2+1/n)$. [F1, F2, F4, step 1.1]

2.2 By [F10], the reciprocal-square series converges to a real number $T$ that bounds every partial sum above. Within the finite index set $n+1$, split off $S$ and let $J$ consist of the remaining indices. The sets $S$ and $J$ are disjoint and finite, since both are subsets of $n+1$. For $p\in S$ the term is $a_p=1/p^2$, and all terms on $J$ are nonnegative. Apply [F9] to the commutative monoid $(\mathbb R,+,0)$. Its sums agree with those of [F7], giving $\sum_{k<n+1}a_k=\sum_{p\in S}a_p+\sum_{k\in J}a_k$. The second sum is nonnegative, so $\sum_{p\in S}1/p^2\le\sum_{k<n+1}a_k\le T$. [F1, F2, F7, F8, F9, F10, step 1.1, step 1.3]

3.1 Add the inequalities of Step 2.1 along a listing of $S$. By additivity and scaling, and since the terms $1/n$ sum to $\#S/n$, the left side of the Statement is bounded by $(4M(n)/3)\big(\sum_{p\in S}1/p^2+\#S/n\big)$. This calculation also holds when $S$ is empty, since all finite sums in the calculation are then zero. [F1, F7, F8, step 1.1, step 2.1]

4.1 Add $\#S/n$ to the comparison in Step 2.2 and multiply by the positive factor $4M(n)/3$. Substituting this bound on the right of Step 3.1, with $T$ equal to the reciprocal-square sum in the Statement, yields the asserted inequality. [F1, step 1.2, step 3.1, step 2.2] ∎

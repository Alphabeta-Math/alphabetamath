---
id: lem-euler-analytic-total-obstruction
kind: lemma
title: Explicit total obstruction bound at the analytic cutoff
status: published
domain: mathematics
proof_strategy: direct
deps:
  - math:def-union-of-a-set-and-binary-union
  - math:lem-unions-and-intersections-of-small-families
  - math:def-subset-and-proper-subset
  - math:lem-of-add-order
  - math:def-axiom-of-choice
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - math:def-real-numbers
  - math:def-field
  - math:def-ordered-field
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-of-q-embeds
  - math:def-rationals
  - math:def-integer-power
  - math:def-rational-power
  - math:def-finite-cardinality
  - math:def-sum-over-a-finite-index-set
  - def-euler-prime-classes
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - lem-euler-analytic-small-prime-estimate
  - lem-euler-analytic-large-prime-estimate
  - lem-euler-analytic-power-comparisons
  - math:thm-reals-ordered-field
  - math:cor-of-one-positive
  - math:lem-of-inverse-positive
  - math:lem-of-sign-rules
  - math:lem-rational-power-laws
  - math:thm-subset-of-a-finite-set
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-finite-sum-reindexing-and-fubini
formulation_deps:
  - math:def-subset-and-proper-subset
  - math:def-axiom-of-choice
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - math:def-real-numbers
  - math:def-field
  - math:def-ordered-field
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-of-q-embeds
  - math:def-rationals
  - math:def-integer-power
  - math:def-rational-power
  - math:def-finite-cardinality
  - math:def-sum-over-a-finite-index-set
  - def-euler-prime-classes
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
argument_deps:
  - math:def-union-of-a-set-and-binary-union
  - math:lem-unions-and-intersections-of-small-families
  - math:def-subset-and-proper-subset
  - math:lem-of-add-order
  - lem-euler-analytic-small-prime-estimate
  - lem-euler-analytic-large-prime-estimate
  - lem-euler-analytic-power-comparisons
  - math:def-axiom-of-choice
  - math:thm-reals-ordered-field
  - math:def-ordered-field
  - math:def-field
  - math:cor-of-one-positive
  - math:lem-of-inverse-positive
  - math:lem-of-sign-rules
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-of-q-embeds
  - math:def-rational-power
  - math:lem-rational-power-laws
  - math:def-finite-cardinality
  - math:thm-subset-of-a-finite-set
  - math:def-sum-over-a-finite-index-set
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-finite-sum-reindexing-and-fubini
dependency_roles:
  math:def-union-of-a-set-and-binary-union: mathematical-premise
  math:lem-unions-and-intersections-of-small-families: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:lem-of-add-order: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:def-field: mathematical-premise
  math:def-ordered-field: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-of-q-embeds: mathematical-premise
  math:def-rationals: mathematical-premise
  math:def-integer-power: mathematical-premise
  math:def-rational-power: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  def-euler-four-square-representations: mathematical-premise
  def-euler-mixed-four-square-representations: mathematical-premise
  def-euler-prime-obstruction-count: mathematical-premise
  lem-euler-analytic-small-prime-estimate: mathematical-premise
  lem-euler-analytic-large-prime-estimate: mathematical-premise
  lem-euler-analytic-power-comparisons: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:cor-of-one-positive: mathematical-premise
  math:lem-of-inverse-positive: mathematical-premise
  math:lem-of-sign-rules: mathematical-premise
  math:lem-rational-power-laws: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:lem-finite-sum-reindexing-and-fubini: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §6, combined numerical estimate at the end of Proposition 6.1
      reading_limits: Consulted the cutoff and equations (6.1)–(6.2) on page 6 and the
        numerical comparison on page 7 for attribution.
dependency_level: 14
---

## Statement

Assume the Axiom of Choice, which asserts the existence of a function selecting one element from each member of any family of nonempty sets. Let $m$ be a positive odd integer, meaning $m>0$ and $m=2j+1$ for some integer $j$, and let $n=2m\ge64^4$. An integer $d$ divides $a$ if $a=dq$ for some integer $q$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Let $\mathcal P_3$ be the primes $p$ congruent to $3$ modulo $4$, meaning that $4$ divides $p-3$. Suppose every prime divisor of $m$ belongs to $\mathcal P_3$.

Let $R(n)$ count the ordered quadruples $(x_1,x_2,x_3,x_4)$ of integers with $x_1^2+x_2^2+x_3^2+x_4^2=n$. Entries may be negative, zero or positive, and two quadruples are equal if their entries agree in all four positions. An integer is even if it has the form $2j$ for an integer $j$. For $p\in\mathcal P_3$, let $b_p(n)$ count the quadruples counted by $R(n)$ that have one even and one odd entry in each of $(x_1,x_2)$ and $(x_3,x_4)$ and for which $p$ divides both entries of at least one pair. Each qualifying quadruple contributes once, including when both pairs qualify.

Use the real numbers for the bounds, including integer, rational and counting values via the inclusions that preserve arithmetic and order. Division by a nonzero real is multiplication by its reciprocal, the unique number that multiplies the divisor to give $1$. Nonnegative integer powers are repeated products, with zeroth power $1$. For a positive base $a$ and a rational exponent $r/s$ with integers $r$ and $s>0$, $a^{r/s}$ is the $r$th integer power of the unique positive real $t$ with $t^s=a$, where a negative integer power $a^{-k}$ is the reciprocal of $a^k$ for $k>0$. Set $X=n^{1/4}$ and $P=2X$.

A set is finite if its elements can be listed once each in a nonnegative integer number of positions. A finite sum adds one term per index and has value $0$ for an empty set of indices. Then $R(n)>0$, and only finitely many primes in $\mathcal P_3$ have $b_p(n)\ne0$. The sum over $\mathcal P_3$ adds only these nonzero terms, and
$$\frac1{R(n)}\sum_{p\in\mathcal P_3}b_p(n)\le\frac{21}{50}+\frac{23}{30}\cdot\frac54\cdot\frac49\left(\frac4{15}+\frac1{64}\right)+\frac{44}{15}\cdot\frac49\left(\frac1{15}+\frac{19}{30\cdot64}+\frac1{64^3}\right)=\frac{21235493}{33177600}<\frac23.$$

## Statement references

[[math:def-axiom-of-choice]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-divides-in-z]]

[[math:def-prime]]

[[math:def-congruence-modulo-an-integer]]

[[math:def-real-numbers]]

[[math:def-field]]

[[math:def-ordered-field]]

[[math:lem-nat-embeds-int]]

[[math:lem-int-embeds-rat]]

[[math:lem-of-q-embeds]]

[[math:def-rationals]]

[[math:def-integer-power]]

[[math:def-rational-power]]

[[math:def-finite-cardinality]]

[[math:def-sum-over-a-finite-index-set]]

[[math:def-subset-and-proper-subset]]

[[def-euler-prime-classes]]

[[def-euler-four-square-representations]]

[[def-euler-mixed-four-square-representations]]

[[def-euler-prime-obstruction-count]]

## Facts & Assumptions

[F1] With the Axiom of Choice and $n=2m\ge64^4$ for positive odd $m$ with every prime divisor in $\mathcal P_3$, the small-prime estimate for $X=n^{1/4}$ and $P=2X$ gives $X\ge64$, $R(n)>0$, and a finite set $S=\{p\in\mathcal P_3:p\le P\}$. It gives $\frac1{R(n)}\sum_{p\in S}b_p(n)\le\frac{21}{50}+\frac{23}{30}2^{3/10}X^{-1/5}\left(\frac4{15}+\frac1X\right)$. [[lem-euler-analytic-small-prime-estimate]] [[math:def-axiom-of-choice]]

[F2] For the same $m,n,X,P$, the large-prime estimate asserts that only finitely many indices $p\in\mathcal P_3$ with $p>P$ have $b_p(n)\ne0$. For their set $T$, it gives $\frac1{R(n)}\sum_{p\in T}b_p(n)\le\frac{44}{15}X^{-1/5}\left(\frac1{15}+\frac{19}{30X}+\frac1{X^3}\right)$. [[lem-euler-analytic-large-prime-estimate]]

[F3] For $X\ge64$ the power comparisons give $X^{-1/5}\le4/9$, $2^{3/10}<5/4$ and $X^{-1}\le1/64$. For positive $a$ and rational $r,s$, the powers satisfy $a^r>0$, $a^{-r}=1/a^r$ and $(a^r)^s=a^{rs}$. [[lem-euler-analytic-power-comparisons]] [[math:def-rational-power]] [[math:lem-rational-power-laws]]

[F4] The reals form an ordered field. Addition and multiplication are associative and commutative, and multiplication distributes over addition. The multiplicative identity is positive. A positive number has a positive reciprocal. Adding the same real number preserves strict inequalities and preserves equality, so it also preserves weak inequalities. Two weak inequalities can therefore be added by translating each inequality and chaining the results. Multiplication by a positive number preserves and reflects both weak and strict inequalities. In this proof the natural numbers are identified with the nonnegative integers, the integers with rationals of denominator $1$, and the rationals with their images in the real field. These inclusions preserve addition, multiplication and order. [[math:thm-reals-ordered-field]] [[math:def-ordered-field]] [[math:def-field]] [[math:cor-of-one-positive]] [[math:lem-of-inverse-positive]] [[math:lem-of-sign-rules]] [[math:lem-of-add-order]] [[math:lem-nat-embeds-int]] [[math:lem-int-embeds-rat]] [[math:lem-of-q-embeds]]

[F5] Every subset of a finite set is finite. A sum over a finite set is independent of the listing of its indices. Real addition is associative and commutative with identity $0$, so the finite sum of real terms over a union of two disjoint finite sets (sets with no common element) is the sum of the two separate sums. A finite list of zeros adds to zero, since one starts at zero and each addition leaves zero unchanged. [[math:def-finite-cardinality]] [[math:thm-subset-of-a-finite-set]] [[math:def-sum-over-a-finite-index-set]] [[math:def-finite-sum-in-a-commutative-monoid]] [[math:lem-finite-sum-reindexing-and-fubini]]

[F6] The binary union $U=S\cup T$ exists for any sets $S$ and $T$, and $p\in U$ holds exactly when $p\in S$ or $p\in T$. Separation within a given set $U$ forms the subset of elements of $U$ satisfying a specified condition. [[math:def-union-of-a-set-and-binary-union]] [[math:lem-unions-and-intersections-of-small-families]] [[math:def-subset-and-proper-subset]]

## Proof

**Given:** The Axiom of Choice and $n=2m\ge64^4$ with $m$ positive and odd and every prime divisor of $m$ in $\mathcal P_3$.

**Goal:** Establish $R(n)>0$, finiteness of the set of nonzero terms, and the exact upper bound for the sum divided by $R(n)$.

1.1 Since $64>0$, the given bound $n\ge64^4$ gives $n>0$, so its positive fourth root $X$ and the cutoff $P=2X$ are defined. The hypotheses give $X\ge64$, $R(n)>0$ and finiteness of $S$ by [F1], and finiteness of $T$ by [F2]. Form $U=S\cup T$ by [F6]. The defining inequalities for $S$ and $T$ make them disjoint. Concatenating their finite listings lists $U$ once per element by the membership rule in [F6], so $U$ is finite. Put $N=\{p\in U:b_p(n)\ne0\}$ by separation within $U$. Every prime in $\mathcal P_3$ with $b_p(n)\ne0$ belongs to $S$ when $p\le P$ and to $T$ when $p>P$. Conversely, every element of $N$ is such a prime. Thus $N$ is exactly the set of nonzero indices, and it is finite by [F5]. [given, F1, F2, F3, F4, F5, F6]

2.1 Form $Z=\{p\in U:b_p(n)=0\}$ by separation within $U$. It is finite by [F5], and $N$ and $Z$ are disjoint with union $U$ since every count is either zero or nonzero. The sum over $U$ equals the sum over $N$ because the sum over $Z$ is zero. Splitting $U$ into $S$ and $T$ therefore gives $\sum_{p\in\mathcal P_3}b_p(n)=\sum_{p\in S}b_p(n)+\sum_{p\in T}b_p(n)$. Multiplying by the reciprocal of $R(n)>0$ and distributing shows that the total divided by $R(n)$ equals the sum of the two quotients bounded in [F1] and [F2]. [step 1.1, F1, F2, F4, F5, F6]

2.2 Put $u=1/X$ and $v=1/64$. By [F3] and positivity of the reciprocals, $0<u\le v$. Multiplication by positive factors gives $u^3\le u^2v\le uv^2\le v^3$. The power laws give $u^3=1/X^3$ and $v^3=1/64^3$. Consequently $\frac4{15}+u\le\frac4{15}+v$ and $\frac1{15}+\frac{19}{30}u+u^3\le\frac1{15}+\frac{19}{30}v+v^3$. All four expressions are positive. [step 1.1, F3, F4]

3.1 In the right side of [F1], replace the positive factors $2^{3/10}$, $X^{-1/5}$ and $4/15+1/X$ by their respective upper bounds $5/4$, $4/9$ and $4/15+1/64$. Each replacement preserves the upper bound because all other factors are positive. In [F2], apply the same reasoning to $X^{-1/5}$ and $\frac1{15}+\frac{19}{30X}+\frac1{X^3}$ using [F3] and step 2.2. Adding the two resulting bounds to bound the sum of quotients in step 2.1 gives the first inequality in the Statement. [step 2.1, step 2.2, F1, F2, F3, F4]

4.1 The small-prime product in this upper bound equals $\frac{23}{54}\cdot\frac{271}{960}=\frac{6233}{51840}$, since $\frac{23}{30}\cdot\frac54\cdot\frac49=\frac{23}{54}$ and $\frac4{15}+\frac1{64}=\frac{271}{960}$. The large-prime parenthesis equals $\frac{49}{640}+\frac1{262144}=\frac{100357}{1310720}$. Multiplying it by $\frac{44}{15}\cdot\frac49=\frac{176}{135}$ gives $\frac{1103927}{11059200}$. [step 3.1, F4, algebra]

5.1 Using the positive common denominator $33177600$, the upper bound is $\frac{13934592+3989120+3311781}{33177600}=\frac{21235493}{33177600}$, whereas $2/3=\frac{22118400}{33177600}$. The latter numerator exceeds $21235493$ by $882907>0$, completing the strict comparison and the proof. [step 1.1, step 3.1, step 4.1, F4, algebra] ∎

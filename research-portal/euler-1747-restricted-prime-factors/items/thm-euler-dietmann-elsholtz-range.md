---
id: thm-euler-dietmann-elsholtz-range
kind: theorem
title: Dietmann and Elsholtz’s sufficiently large range
status: published
domain: mathematics
proof_strategy: direct
deps:
  - math:def-nat-order
  - math:def-real-order
  - math:def-nat-power
  - math:def-real-exponential-function-and-e
  - math:def-axiom-schema-of-separation
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - math:def-prime
  - math:def-divides-in-z
  - math:def-natural-logarithm
  - math:def-rational-power
  - math:def-finite-cardinality
  - math:thm-division-algorithm-in-z
  - math:thm-subset-of-a-finite-set
  - thm-author-f93d28423212-greaves-prime-pairs
  - lem-author-f93d28423212-excluded-prime-pairs
  - lem-author-f93d28423212-logarithmic-count-comparison
  - lem-author-f93d28423212-admissible-square-grouping
  - math:thm-int-ordered-ring
  - math:def-real-numbers
  - math:def-natural-numbers
  - math:def-rationals
  - math:thm-reals-ordered-field
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:thm-natural-logarithm-laws
  - math:def-ordered-pair
  - math:def-cartesian-product
  - math:def-subset-and-proper-subset
  - math:lem-cardinality-of-finite-natural-initial-segment
  - math:thm-product-rule
formulation_deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - math:def-prime
  - math:def-divides-in-z
argument_deps:
  - math:def-nat-order
  - math:def-real-order
  - math:def-nat-power
  - math:def-real-exponential-function-and-e
  - math:def-axiom-schema-of-separation
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - math:def-prime
  - math:def-divides-in-z
  - math:def-natural-logarithm
  - math:def-rational-power
  - math:def-finite-cardinality
  - math:thm-division-algorithm-in-z
  - math:thm-subset-of-a-finite-set
  - thm-author-f93d28423212-greaves-prime-pairs
  - lem-author-f93d28423212-excluded-prime-pairs
  - lem-author-f93d28423212-logarithmic-count-comparison
  - lem-author-f93d28423212-admissible-square-grouping
  - math:thm-int-ordered-ring
  - math:def-real-numbers
  - math:def-natural-numbers
  - math:def-rationals
  - math:thm-reals-ordered-field
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:thm-natural-logarithm-laws
  - math:def-ordered-pair
  - math:def-cartesian-product
  - math:def-subset-and-proper-subset
  - math:lem-cardinality-of-finite-natural-initial-segment
  - math:thm-product-rule
dependency_roles:
  math:def-nat-order: mathematical-premise
  math:def-real-order: mathematical-premise
  math:def-nat-power: mathematical-premise
  math:def-real-exponential-function-and-e: mathematical-premise
  math:def-axiom-schema-of-separation: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-natural-logarithm: mathematical-premise
  math:def-rational-power: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  thm-author-f93d28423212-greaves-prime-pairs: mathematical-premise
  lem-author-f93d28423212-excluded-prime-pairs: mathematical-premise
  lem-author-f93d28423212-logarithmic-count-comparison: mathematical-premise
  lem-author-f93d28423212-admissible-square-grouping: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-rationals: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:thm-natural-logarithm-laws: mathematical-premise
  math:def-ordered-pair: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:lem-cardinality-of-finite-natural-initial-segment: mathematical-premise
  math:thm-product-rule: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, §1, paragraph before Theorem 1.1, and p. 8, reference [2]
    - title: Sums of two numbers having only prime factors congruent to one modulo
        four
      url: https://www.impan.pl/shop/publication/transaction/download/product/113105
      locator: Dietmann and Elsholtz, Banach Center Publications 118 (2019), p. 177,
        unnumbered Theorem, and pp. 178–179, proof and reference [3]
dependency_level: 3
---

## Statement

There is a positive integer $N$ such that every positive integer $n\ge N$ with $n\equiv2\pmod4$ can be written $n=a+b$ with both $a$ and $b$ admissible. A positive integer is an integer greater than $0$. An integer is admissible if it is positive and every prime divisor is congruent to $1$ modulo $4$. A prime exceeds $1$ and has only $1$ and itself as positive divisors. A divisor $d$ of $t$ satisfies $t=dk$ for an integer $k$. The congruence $u\equiv v\pmod4$ means that $4$ divides $u-v$.

## Statement references

[[def-euler-prime-classes]]

[[math:def-congruence-modulo-an-integer]]

## Facts & Assumptions

[F1] For a positive integer $n$, let $C_n$ consist of the ordered prime pairs $(p,q)$ with $1<p,q\le\sqrt{n/2}$ for which there exist integers $x,y$ with $n=p^2+q^2+x^2+y^2$. The uniform consequence of Greaves’s estimate gives a real $c>0$ and an integer $N_0\ge2$ such that $|C_n|\ge c n/(\log n)^{5/2}$ for every integer $n\ge N_0$ with remainder $2$, $3$, $4$, $6$ or $7$ upon division by $8$. [[thm-author-f93d28423212-greaves-prime-pairs]] [[math:def-integers]] [[math:def-prime]]

[F2] For a positive integer $n$, let $E_n$ consist of the ordered prime pairs $(p,q)$ for which there exist integers $x,y$ with $n=p^2+q^2+x^2+y^2$ and at least one of $p=2$, $q=2$, $p\mid x$, $q\mid y$. Then $|E_n|\le K n^{13/16}$ with the positive integer $K=12\cdot4\cdot16^{65536}+2$. $16^{65536}$ denotes a natural-number power read as an integer. [[lem-author-f93d28423212-excluded-prime-pairs]] [[math:def-integers]] [[math:def-divides-in-z]] [[math:def-nat-power]]

[F3] For positive real numbers $c,K$ there is an integer $M\ge2$ such that $c n/(\log n)^{5/2}>K n^{13/16}$ for every integer $n\ge M$. [[lem-author-f93d28423212-logarithmic-count-comparison]]

[F4] For a positive integer $n\equiv2\pmod4$, if $p,q$ are primes greater than $2$ and integers $x,y$ satisfy $n=p^2+q^2+x^2+y^2$ with $p\nmid x$ and $q\nmid y$, then $p^2+x^2$ and $q^2+y^2$ are admissible. [[lem-author-f93d28423212-admissible-square-grouping]] [[def-euler-prime-classes]] [[math:def-integers]]

[F5] Division of an integer by a positive integer $b$ gives a unique expression $a=qb+r$ with integer quotient $q$ and integer remainder $0\le r<b$. The integers form a totally ordered commutative ring. Integer squares are products $s^2=s\cdot s$. [[math:thm-division-algorithm-in-z]] [[math:def-int-operations]] [[math:thm-int-ordered-ring]]

[F6] The reals form a totally ordered field. Identify the natural numbers, integers and rationals with their images under the canonical embeddings $\mathbb N\hookrightarrow\mathbb Z\hookrightarrow\mathbb Q\hookrightarrow\mathbb R$, which preserve order and arithmetic. The natural-number image in the integers consists of all nonnegative integers. In a real comparison, a finite cardinality $|S|$ is read as the real image of the natural number counting the elements of $S$. The natural logarithm is the inverse of the real exponential, is strictly increasing, and satisfies $\log 1=0$. The square root and the fractional powers in these bounds use positive real roots. [[math:def-real-numbers]] [[math:thm-reals-ordered-field]] [[math:def-real-order]] [[math:def-natural-numbers]] [[math:def-rationals]] [[math:lem-nat-embeds-int]] [[math:lem-int-embeds-rat]] [[math:lem-rat-embeds-dense]] [[math:def-finite-cardinality]] [[math:def-natural-logarithm]] [[math:def-real-exponential-function-and-e]] [[math:thm-natural-logarithm-laws]] [[math:def-rational-power]]

[F7] A Cartesian product consists of the ordered pairs from the two factor sets. For fixed $n$, the conditions in [F1] and [F2] are predicates on $\mathbb Z\times\mathbb Z$ with the integer witnesses $x,y$ bound in each predicate. Each predicate uses only the pair, $n$, and the fixed arithmetic data. Applying Separation to these predicates gives $C_n$ and $E_n$. For a natural $m$, the initial segment $I_m=\{t\in\mathbb N:t<m\}$ is finite. A product of two finite sets is finite, and any subset of a finite set is finite and has at most its cardinality in the natural order. [[math:def-ordered-pair]] [[math:def-cartesian-product]] [[math:def-subset-and-proper-subset]] [[math:def-axiom-schema-of-separation]] [[math:lem-cardinality-of-finite-natural-initial-segment]] [[math:def-nat-order]] [[math:thm-product-rule]] [[math:thm-subset-of-a-finite-set]]

## Proof

**Given:** A positive integer in the residue class $2$ modulo $4$, subject to the threshold chosen below.

**Goal:** Produce a common integer threshold and an admissible decomposition above it.

1.1 Choose $c,N_0$ by [F1] and take the positive integer $K$ from [F2]. Its real image is positive by [F6], so choose $M$ by [F3] for these positive real constants. Set $N$ equal to the larger of $N_0$ and $M$ in the integer order. Let $n\ge N$ satisfy $n\equiv2\pmod4$. Its real image satisfies $n\ge2>1$, so $\log n>\log 1=0$ and the positive-root denominator in [F1] and [F3] is defined and nonzero. [given, F1, F2, F3, F5, F6]

2.1 There is no integer $t$ with $0<t<1$, since $t=0\cdot1+t=t\cdot1+0$ would then give two legal remainders on division by $1$, contrary to [F5]. Write $n=4k+2$ with $k$ an integer, by the meaning of congruence. Divide $k=2u+r$ with $0\le r<2$. If $r>0$, the interval $(0,1)$ is excluded for $r$, and $r>1$ would put $r-1$ in $(0,1)$. Thus $r$ is $0$ or $1$. The equality $n=8u+4r+2$ gives remainder $2$ or $6$ modulo $8$, as required in [F1]. [step 1.1, F1, F5]

2.2 In any representation used to define $C_n$ or $E_n$, the four squares are nonnegative in the ordered integer ring, since the square of a negative integer is the square of its positive opposite. Hence $p^2,q^2\le n$. Primality gives $p,q>1$, so $p(p-1),q(q-1)\ge0$ and $p\le p^2$, $q\le q^2$. By [F6] both coordinates belong to $I_{n+1}$ when the naturals are identified with the nonnegative integers. Therefore $C_n$ and $E_n$ are subsets of the finite product $I_{n+1}\times I_{n+1}$, and both have finite cardinalities by [F7]. [step 1.1, F1, F2, F5, F6, F7]

3.1 The bounds in [F1] and [F2] apply to these sets. By [F3], $|C_n|\ge c n/(\log n)^{5/2}>K n^{13/16}\ge |E_n|$ in the real order. If $C_n\subseteq E_n$, [F7] gives $|C_n|\le |E_n|$ in the natural order. The inclusions in [F6] preserve that inequality in the real order, contradicting the strict comparison. Thus a pair in $C_n$ lies outside $E_n$. [step 1.1, step 2.1, step 2.2, F1, F2, F3, F6, F7]

4.1 Choose integer witnesses $x,y$ from [F1] for that pair. Since the pair lies outside $E_n$, these witnesses satisfy $p\nmid x$ and $q\nmid y$, and neither prime equals $2$. A prime strictly between $1$ and $2$ would yield an integer in $(0,1)$ by subtracting $1$, contrary to step 2.1. Hence $p,q>2$, and [F4] shows that $a=p^2+x^2$ and $b=q^2+y^2$ are admissible. Reordering the four terms gives $n=a+b$. The same $N$ was chosen before $n$, so the decomposition holds throughout the claimed range. [step 1.1, step 2.1, step 3.1, F1, F2, F4, F5] ∎

## Source notes

Howe, Huffman, Kohlmeyer and Kruer cite Dietmann and Elsholtz’s theorem in their introduction and identify Greaves’s four-square result with two prime variables as the key input. Dietmann and Elsholtz count distinct candidate summand pairs before excluding inadmissible ones. The proof here counts excluded prime pairs directly using the bound on the number of two-square completions. The imported lower bound gives an existential threshold.

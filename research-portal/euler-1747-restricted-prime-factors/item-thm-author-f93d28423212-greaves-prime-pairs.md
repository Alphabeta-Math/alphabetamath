---
title: Greaves’s lower bound for prime pairs in a four-square representation
status: published
research_item: thm-author-f93d28423212-greaves-prime-pairs
dependency_level: 0
sources:
  references:
    - title: On the representation of a number in the form x² + y² + p² + q² where p,
        q are odd primes
      url: https://bibliotekanauki.pl/articles/1393472.pdf
      locator: Acta Arithmetica 29 (1976), §1, theorem, survivor comparison and
        convention on implied constants; (3.1), Lemma 7, (4.1), Lemma 8,
        (4.13)–(4.14), and §6, (6.1)
      statement: For sufficiently large N in an allowed class, the ordered prime pairs
        with 1 < p,q ≤ √(N/2) for which N−p²−q² is a sum of two integer squares
        number more than A(N)N(1+e_N)/(log N)^(5/2), with A(N) from (6.1) and
        |e_N| bounded by L log log N/(log N)^(1/10). The lower bound in §6 comes
        from subtracting unwanted survivors among the ordered prime pairs.
      hypotheses: N is a sufficiently large positive integer incongruent to 0, 1 and 5
        modulo 8. Count a pair when at least one representation of its remainder
        as a sum of two integer squares exists. The constant L may depend at
        most on N modulo 8.
      reading_limits: Read the indexed text of the theorem and its survivor
        comparison, the ordered-pair setup, Lemmas 7 and 8 and the conclusion.
        The index renders the radical inconsistently. The bound at √(N/2) uses
        the range in (4.1) and Lemma 8, consistent with N=2Z² in Lemma 7, and
        the conclusion via (4.13)–(4.14). Page images could not be retrieved.
        The sieve estimates are imported and the threshold is existential.
    - title: On the representation of a number in the form x² + y² + p² + q² where p,
        q are odd primes
      url: https://bibliotekanauki.pl/articles/1393472.pdf
      locator: Acta Arithmetica 29 (1976), (2.4), §3 preceding (3.4), (3.4)–(3.6),
        (4.6), Lemma 10, and §6 through (6.1)
      statement: A(N)=D B G Π₀/√2 with D>0 given by (2.4) independently of N and
        B=Kψ(K,1)/φ(K)²>0, where K is a positive divisor of 72 and ψ(K,1) comes
        from the normalized residue-pair count (3.4). The positive G is
        determined by C/B in the function g of §6. Lemma 10 gives C/B as a fixed
        positive multiple of (φ(K)/K)².
      hypotheses: N lies in one of the five classes in the theorem. Take K and the
        residue restrictions from Greaves's construction in §§3–4 and the
        constants from the same construction in §§5–6.
      reading_limits: Checked the indexed coefficient formulas and positivity
        statements in the passages cited. The dependence on K suffices here and
        the numerical multiplier in Lemma 10 is unused. The sieve derivation is
        imported.
    - title: On the representation of a number in the form x² + y² + p² + q² where p,
        q are odd primes
      url: https://bibliotekanauki.pl/articles/1393472.pdf
      locator: Acta Arithmetica 29 (1976), end of §1, (3.4)–(3.7), (4.4), (4.9) and
        following sentence, and (4.11)–(4.12)
      statement: Π₀ is the convergent product over primes ℓ≡3 modulo 4 of
        (1−τ(ℓ)/ℓ)/(1−1/ℓ), with τ(ℓ)<ℓ. For ℓ>3 not dividing N, τ(ℓ)=1+O(1/ℓ),
        with the implied constant depending at most on N modulo 8. For ℓ≡3
        modulo 4 dividing N, τ(ℓ)=0. For fixed ℓ, τ(ℓ) is determined by K, ℓ,
        the totients and the normalized counts from (3.4)–(3.7) at l=1 and l=ℓ.
      hypotheses: Use the sieve for Greaves's set of odd-prime pairs in §§3–4 and N in
        the stated classes modulo 8. The large-prime estimate is used only for
        ℓ>3 with ℓ not dividing N.
      reading_limits: Checked the indexed local-count setup, the bounds on τ and the
        convergence statement. The proof below uses the finite moduli and the
        stated bounds to derive a uniform positive lower bound.
---

## Prerequisites

- [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)
- [math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-sum-of-two-squares-representation](https://alphabetamath.cc/item/def-sum-of-two-squares-representation)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:def-natural-logarithm](https://alphabetamath.cc/item/def-natural-logarithm)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-infinite-product](https://alphabetamath.cc/item/def-infinite-product)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-real-exponential-function-and-e](https://alphabetamath.cc/item/def-real-exponential-function-and-e)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-unit-group-modulo-n-and-euler-totient](https://alphabetamath.cc/item/def-unit-group-modulo-n-and-euler-totient)
- [math:lem-cauchy-reals-archimedean](https://alphabetamath.cc/item/lem-cauchy-reals-archimedean)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-limit-preserves-order](https://alphabetamath.cc/item/lem-limit-preserves-order)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:thm-logarithm-slower-than-every-positive-power](https://alphabetamath.cc/item/thm-logarithm-slower-than-every-positive-power)
- [math:thm-natural-logarithm-laws](https://alphabetamath.cc/item/thm-natural-logarithm-laws)
- [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)
- [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)
- [math:def-abs-value](https://alphabetamath.cc/item/def-abs-value)
- [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-sequence](https://alphabetamath.cc/item/def-sequence)
- [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit)
- [math:def-limits-at-infinity](https://alphabetamath.cc/item/def-limits-at-infinity)
- [math:def-real-power](https://alphabetamath.cc/item/def-real-power)
- [math:thm-real-power-agrees-with-rational-exponent](https://alphabetamath.cc/item/thm-real-power-agrees-with-rational-exponent)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:thm-standard-representatives-modulo-n](https://alphabetamath.cc/item/thm-standard-representatives-modulo-n)
- [math:def-max-min](https://alphabetamath.cc/item/def-max-min)
- [math:lem-finite-subsets-listable](https://alphabetamath.cc/item/lem-finite-subsets-listable)
- [math:lem-finite-set-has-max](https://alphabetamath.cc/item/lem-finite-set-has-max)
- [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [` On the representation of a number in the form x² + y² + p² + q² where p, q are odd primes · Acta Arithmetica 29 (1976), §1, theorem, survivor comparison and convention on implied constants; (3.1), Lemma 7, (4.1), Lemma 8, (4.13)–(4.14), and §6, (6.1) `](https://bibliotekanauki.pl/articles/1393472.pdf)
- [` On the representation of a number in the form x² + y² + p² + q² where p, q are odd primes · Acta Arithmetica 29 (1976), (2.4), §3 preceding (3.4), (3.4)–(3.6), (4.6), Lemma 10, and §6 through (6.1) `](https://bibliotekanauki.pl/articles/1393472.pdf)
- [` On the representation of a number in the form x² + y² + p² + q² where p, q are odd primes · Acta Arithmetica 29 (1976), end of §1, (3.4)–(3.7), (4.4), (4.9) and following sentence, and (4.11)–(4.12) `](https://bibliotekanauki.pl/articles/1393472.pdf)


## Statement

There are a real constant $c>0$ and an integer $N_0\ge2$ such that the following holds. Let $n$ be an integer at least $N_0$ with remainder $2$, $3$, $4$, $6$ or $7$ upon division by $8$. The number of ordered prime pairs $(p,q)$ with $1<p,q\le\sqrt{n/2}$ such that $n-p^2-q^2=x^2+y^2$ for some integers $x,y$ is at least $c n/(\log n)^{5/2}$. A prime exceeds $1$ and has exactly $1$ and itself as positive divisors. Here $\sqrt{n/2}$ is the positive square root of $n/2$, $\log$ is the natural logarithm (the inverse of the real exponential), and the power $5/2$ takes the fifth power of a positive square root. Counts and integer inputs in real expressions are read via the canonical order-preserving embeddings $\mathbb N\hookrightarrow\mathbb Z\hookrightarrow\mathbb Q\hookrightarrow\mathbb R$.

## External input

Greaves’s counting argument in §§4–6 gives a lower bound for the count $S(n)$ of eligible ordered prime pairs with each prime at most $\sqrt{n/2}$. The estimate uses an input-dependent coefficient $A(n)=D B(n) G(n)\Pi(n)/\sqrt 2$ and a relative error bounded in magnitude by a constant times $\log\log n/(\log n)^{1/10}$ for sufficiently large $n$ in each allowed residue class. The inputs specifying the coefficient are the finite congruence counts, the positive quantity $G$ from §6, and the local factors of the convergent product in (4.11).

## Facts & Assumptions

[F1] For $n$ in the five allowed classes modulo $8$ and sufficiently large, Greaves’s theorem gives $S(n)>A(n)n(1+e_n)/(\log n)^{5/2}$ with $|e_n|\le L\log\log n/(\log n)^{1/10}$. The constant $L$ and the initial threshold may be taken for each class separately. Count each ordered prime pair in the range $1<p,q\le\sqrt{n/2}$ for which a two-square representation exists. This range contains all pairs in the sieve of (4.1) and Lemma 8, used in the lower bound of §6.

[F2] Greaves’s coefficient in (6.1) is $A(n)=D B(n)G(n)\Pi(n)/\sqrt 2$. The constant $D>0$ in (2.4) is independent of $n$. The positive factor $B=K\psi(K,1)/\varphi(K)^2$ uses a positive divisor $K$ of $72$, Euler’s totient $\varphi$, and the normalized congruence count $\psi(K,1)$ in (3.4). The positive factor $G$ in §6 depends on $C/B$, which in Lemma 10 is a fixed positive multiple of $(\varphi(K)/K)^2$. [math:def-unit-group-modulo-n-and-euler-totient](https://alphabetamath.cc/item/def-unit-group-modulo-n-and-euler-totient)

[F3] In Greaves’s (4.11)–(4.12), $\Pi(n)$ is the limit of partial products in increasing prime order, with factor $f_\ell(n)=(1-\tau(\ell)/\ell)/(1-1/\ell)$ at each prime $\ell\equiv3\pmod4$. By (4.4), every such factor is positive. The bounds in and immediately after (4.9) give $\tau(\ell)\le1+H/\ell$ for $\ell>3$ not dividing $n$, with $H>0$ independent of $n$ after taking the largest constant across the five classes, and $\tau(\ell)=0$ if $\ell\equiv3\pmod4$ divides $n$. For fixed $\ell$, (3.4)–(3.7) determine $\tau(\ell)$ from $K,\ell$, totients and normalized solution counts for $l=1,\ell$ in (3.4). Each such count is obtained by counting pairs in residue classes for a fixed finite modulus once $K$ and $l$ are fixed.

[F4] Integer arithmetic and order are those of the ordered integer ring. In the integer equation, $s^2$ means the integer product $s\cdot s$. Division by a positive integer gives a unique quotient and nonnegative remainder smaller than the divisor. Congruence modulo a positive integer means divisibility of the difference. A positive divisor of $72$ is at most $72$. [math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z) [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer) [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[F5] The canonical embeddings preserve order and arithmetic, and every nonnegative integer comes from a natural number. An ordered field is complete if every nonempty subset bounded above has a least upper bound in the field. The Cauchy-sequence reals form such a field, and the natural numbers are cofinal in it. The root theorem applied to this complete ordered field gives unique positive roots of positive numbers. For a real $s$, the natural-power recursion gives $s^2=s\cdot s$. [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field) [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete) [math:lem-cauchy-reals-archimedean](https://alphabetamath.cc/item/lem-cauchy-reals-archimedean) [math:thm-nth-roots-exist](https://alphabetamath.cc/item/thm-nth-roots-exist) [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

[F6] The natural number $m$ is the finite initial segment of naturals below $m$. A finite set admits a bijection with such an initial segment. A subset of a finite set is finite and has at most its cardinality. An injection is a bijection onto its image, and a bijection with a finite set transfers finiteness. Cartesian products contain the ordered pairs from their factors, and products of two finite sets are finite. Separation forms subsets of a given set by predicates with fixed parameters. Applied to a Cartesian product, it also forms a graph, which defines a function on the first set when each input has exactly one output in the second set. [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product) [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair) [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule) [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation) [math:def-function](https://alphabetamath.cc/item/def-function)

[F7] Finite products start at $1$ and multiply by the next factor at each successor index, so induction applies to the partial products. The product in [F3] converges. A real sequence here converges when its terms are eventually within every positive rational tolerance of its limit. An eventual lower bound on the sequence is a lower bound on that limit. [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle) [math:def-infinite-product](https://alphabetamath.cc/item/def-infinite-product) [math:def-sequence](https://alphabetamath.cc/item/def-sequence) [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit) [math:lem-limit-preserves-order](https://alphabetamath.cc/item/lem-limit-preserves-order)

[F8] The natural logarithm on the positive reals is the inverse of the real exponential. It is strictly increasing, is onto the reals, and has $\log 1=0$. For every real $\alpha>0$, $\log t/t^\alpha$ tends to $0$ as $t$ tends to positive infinity, so its absolute value is smaller than each positive tolerance once $t$ is sufficiently large. The real power agrees with the positive-base rational power at rational exponents. In particular, $a^{5/2}=s^5$ for $a>0$ and $s=\sqrt a$, where $s^5=s\cdot s\cdot s\cdot s\cdot s$ by the natural-power recursion. Absolute value is $|u|=u$ for $u\ge0$ and $|u|=-u$ for $u<0$. [math:def-natural-logarithm](https://alphabetamath.cc/item/def-natural-logarithm) [math:def-real-exponential-function-and-e](https://alphabetamath.cc/item/def-real-exponential-function-and-e) [math:thm-natural-logarithm-laws](https://alphabetamath.cc/item/thm-natural-logarithm-laws) [math:thm-logarithm-slower-than-every-positive-power](https://alphabetamath.cc/item/thm-logarithm-slower-than-every-positive-power) [math:def-limits-at-infinity](https://alphabetamath.cc/item/def-limits-at-infinity) [math:def-real-power](https://alphabetamath.cc/item/def-real-power) [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power) [math:thm-real-power-agrees-with-rational-exponent](https://alphabetamath.cc/item/thm-real-power-agrees-with-rational-exponent) [math:def-abs-value](https://alphabetamath.cc/item/def-abs-value) [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

[F9] For a positive modulus $m$, congruence classes form the quotient set $\mathbb Z/m$. Each class has one representative in $0,\dots,m-1$, and there are $m$ classes. In the complete ordered field of [F5], every nonempty finite set of reals is the set of entries of a nonempty finite list. The extrema lemma applied to that list gives a minimum and a maximum, each attained in the set. Every nonempty set of naturals has a least member. [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field) [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n) [math:thm-standard-representatives-modulo-n](https://alphabetamath.cc/item/thm-standard-representatives-modulo-n) [math:def-max-min](https://alphabetamath.cc/item/def-max-min) [math:lem-finite-subsets-listable](https://alphabetamath.cc/item/lem-finite-subsets-listable) [math:lem-finite-set-has-max](https://alphabetamath.cc/item/lem-finite-set-has-max) [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)

## Proof

**Given:** The prime-pair estimate and coefficient data in [F1]–[F3].

**Goal:** A common positive coefficient and integer threshold for the five allowed remainders.

1.1 Let $n\ge2$ be an integer with an allowed remainder $r$. The equality $n=8k+r$ for an integer $k$ gives $n\equiv r\pmod 8$ by divisibility. For $0\le a<b$, both $b-a$ and $b+a$ are positive, so $b^2-a^2=(b-a)(b+a)>0$ in the ordered field of [F5]. Equality of inputs gives equality of squares, and trichotomy rules out $a>b$ when $a^2\le b^2$. Thus $a\le b$ if and only if $a^2\le b^2$ for nonnegative $a,b$. Since $n\ge2$, we have $n^2\ge n\ge n/2$. Comparing $n$ with $\sqrt{n/2}$ by their squares shows that both prime coordinates are at most $n$. By separation the pairs meeting the prime, cutoff, and two-square conditions form a subset of the product of the integer interval from $1$ to $n$ with itself. On that subset the rule $(p,q)\mapsto(p-1)n+(q-1)$ gives one integer in the initial segment below $n^2$, since both $p-1$ and $q-1$ lie between $0$ and $n-1$. The graph in the product with this initial segment defines a function by [F6]. It is injective because division by $n$ recovers $p-1$ as quotient and $q-1$ as remainder. Its image is a subset of that finite segment, so the bijection onto the image makes the pair count finite. Also $p^2,q^2\le n/2$, hence $n-p^2-q^2\ge0$ and the two-square condition applies to a nonnegative integer, including zero. Each eligible pair is counted once regardless of how many integer pairs represent its remainder. [given, F1, F4, F5, F6]

1.2 Fix an integer $M$ greater than both $3$ and $2H$ by cofinality. For a prime $\ell\equiv3\pmod4$ with $\ell>M$, the factor is $f_\ell(n)=1-(\tau(\ell)-1)/(\ell-1)$. If $\ell$ divides $n$, the factor is greater than $1$. Otherwise $\tau(\ell)-1\le H/\ell$. In either case $f_\ell(n)\ge 1-H/[\ell(\ell-1)]$. [F3, F5]

1.3 For $n\ge2$, $\log n>0$ by strict increase and $\log 1=0$. Take $L>0$ at least as large as the five constants in [F1]. By [F8] with $\alpha=1/10$ there is $T\ge1$ such that $|\log t/t^{1/10}|<1/(2L)$ for $t>T$. Choose a positive real $u$ with $\log u=T$ by surjectivity. By cofinality and the finite maximum of the five initial thresholds, choose an integer $N_0\ge2$ larger than $u$ and all those thresholds. If $n\ge N_0$, then $\log n>T$ and $\log\log n\ge0$. Applying the displayed tolerance at $t=\log n$ proves $|e_n|<1/2$ in all five classes. [F1, F5, F8, F9]

1.4 By [F2] and [F4], each possible $K$ satisfies $0<K\le72$. By [F5] it comes from a natural number, and [F6] identifies $1$ with the initial segment whose only element is $0$. Thus $1\le K\le72$. Separation within the finite initial segment below $73$ forms the finite set of natural representatives of possible values of $K$. To see that a function on a finite parameter set has finite image, use [F6] to index the parameters by a bijection with a natural initial segment. Form the set of attained values by separation in the codomain. For each attained value, use separation on the segment to form the nonempty set of indices at which that value occurs. By [F9] this set has a unique least index. The graph assigning that index to each attained value is a function by [F6]. It is injective because the value at any given index is unique. Its image is a subset of the finite segment, so the set of attained values is finite by the bijection onto that image. Fix $l=1$ or a prime $l=\ell\equiv3\pmod4$. For each possible $K$, the raw count in (3.4) is the size of a subset of pairs of standard representatives for the fixed moduli in that formula. Each finite residue set has its modulus as its size by [F9]. Their product is finite, and by [F6] the raw count is an integer between zero and the size of that product. The set of these product sizes is a finite image of the possible values of $K$ and is nonempty since there are inputs in the five allowed classes. Take its attained maximum by [F9], using the natural-number embedding in [F5] to compare the sizes as reals. For each fixed $\ell$, $K$ and the two raw counts for $l=1,\ell$ therefore range over a subset of a finite product of initial segments. The normalization depends on $K,l$, so [F3] makes $f_\ell(n)$ a function of those finite data. It consequently takes only finitely many values. [F2, F3, F4, F5, F6, F9]

2.1 For an integer $J\ge M$, let $P_J(n)$ be the product of the factors at primes $\ell\equiv3\pmod4$ with $M<\ell\le J$. In the recursion over the integers, a noncontributing index supplies a factor of $1$. By induction $P_J(n)\ge b_J:=1-H/M+H/J\ge1/2$. The base $J=M$ has $P_M(n)=b_M=1$. At $J+1$ the multiplier is at least $1-H/[J(J+1)]>0$ by step 1.2 or by being $1$. Since $0<b_J\le1$, the new product is at least $b_J-H/[J(J+1)]=b_{J+1}$. [step 1.2, F5, F7]

3.1 For every prime $\ell\equiv3\pmod4$ with $\ell\le M$, take the minimum of the nonempty finite set of actual factor values from step 1.4. All such minima are positive by [F3]. Let $\delta$ be their product, with empty product $1$. The prefix product through $M$ is at least $\delta>0$ by induction, since both sides start at $1$ and each factor is at least its positive minimum. A partial product through $J\ge M$ is the prefix through $M$ times $P_J(n)$: at $J=M$ the tail equals $1$, and the two products use the same successive multipliers. Thus every such partial product is at least $\delta/2$ by step 2.1. The increasing prime order has only finitely many indices at primes at most $M$, so the bound is eventual in the sequence of partial products. By [F7] it passes to the limit $\Pi(n)$. [step 2.1, step 1.4, F3, F5, F6, F7, F9]

4.1 By [F2], $B$ is determined by $K$ and the normalized count at $l=1$, and $G$ is determined by $K$. Step 1.4 gives finitely many possible values for each of these inputs, so both $B$ and $G$ have finite ranges. The pairs $(B,G)$ lie in a finite product, and their image under $(B,G)\mapsto D B G/\sqrt 2$ is a nonempty finite set of positive reals by [F2] and [F5]. Its attained minimum $d$ is positive by [F9]. Multiplying by the lower bound for $\Pi(n)$ gives $A(n)\ge d\delta/2$ throughout the five classes. [step 1.4, step 3.1, F2, F5, F6, F9]

5.1 For an integer $n\ge N_0$ with a stated remainder, the congruence in step 1.1 allows [F1]. Step 1.3 and the definition of absolute value give $1+e_n\ge 1-|e_n|>1/2$. The denominator $(\log n)^{5/2}$ is the product of five copies of the positive square root of $\log n$ by [F8], so it is positive in the ordered field. The coefficient bound in step 4.1 now gives $S(n)>(d\delta/4)n/(\log n)^{5/2}$. Since $S(n)$ counts eligible ordered pairs in the stated range, $c=d\delta/4>0$ gives the result. [step 1.1, step 1.3, step 4.1, F1, F5, F8] ∎

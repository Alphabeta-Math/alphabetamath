---
title: Finite conductor of local components
status: draft
research_item: def-author-f98bf83ef432-finite-conductor
dependency_level: 2
sources:
  references:
    - title: Andrew Corbett and Abhishek Saha, On the order of vanishing of newforms
        at cusps
      url: https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf
      locator: §3.1, p. 16, definition of N in the paragraph introducing the local
        exponents
      reading_limits: Read the cited paragraph for the prime-power product convention
        for the local components of an irreducible unitary cuspidal automorphic
        representation. The definition for conditional families and its
        justification are given here.
---

## Prerequisites

- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)
- [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [def-author-f98bf83ef432-local-conductor-exponent](item-def-author-f98bf83ef432-local-conductor-exponent)
- [math:def-countable](https://alphabetamath.cc/item/def-countable)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)


## Definition

Let $(\rho_q)_q$ be a family indexed by the primes, with $\rho_q$ a complex representation of $\mathrm{GL}_2(\mathbb Q_q)$, the group of invertible two-by-two matrices over the $q$-adic field $\mathbb Q_q$. Assume that every local conductor exponent $a(\rho_q)$ exists as the least nonnegative congruence exponent giving a nonzero fixed space. Assume that the set $S$ of primes with $a(\rho_q)>0$ is finite.

In a factor $q^{a(\rho_q)}$, use the natural exponent $k_q$ with $\iota(k_q)=a(\rho_q)$, where $\iota:\mathbb N\to\mathbb Z$ is the natural embedding. Compute the powers and the product in the multiplicative monoid $(\mathbb Z,\cdot,1)$. The finite conductor $C$ of the family is
$$C=\prod_{q:\,a(\rho_q)>0}q^{a(\rho_q)},$$
with the factors taken in increasing prime order and with the empty product equal to $1$.

## Definition references

[Indexed family](https://alphabetamath.cc/item/def-indexed-family)

[Prime integers](https://alphabetamath.cc/item/def-prime)

[The $q$-adic completion](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)

[Field operations on the completion](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)

[General linear group](item-def-degree-two-projective-linear-group)

[Local conductor exponent and its domain](item-def-author-f98bf83ef432-local-conductor-exponent)

[Finite sets](https://alphabetamath.cc/item/def-countable)

[Nonnegative integers as natural numbers](https://alphabetamath.cc/item/lem-nat-embeds-int)

[Ordered integer ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[Monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)

[Natural powers](https://alphabetamath.cc/item/def-group-power)

[Finite products](https://alphabetamath.cc/item/def-monoid-finite-product)

## Facts & Assumptions

[F1] The integers are a totally ordered commutative ring, positive integers are closed under multiplication, and a prime $q$ satisfies $q>1>0$. [Ordered integer ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [Prime integers](https://alphabetamath.cc/item/def-prime)

[F2] A finite set admits a bijective listing of length $n$ for some natural number $n$. [Finite sets](https://alphabetamath.cc/item/def-countable)

[F3] The natural embedding $\iota$ identifies the natural numbers in order with the nonnegative integers. Every nonempty set of natural numbers has a least element. [Natural embedding](https://alphabetamath.cc/item/lem-nat-embeds-int) [Well-ordering of the naturals](https://alphabetamath.cc/item/thm-well-ordering-principle)

[F4] A property of natural numbers follows by verifying it at zero and passing from each $n$ to its successor. [Induction](https://alphabetamath.cc/item/thm-induction-principle)

[F5] Integer multiplication is associative with two-sided identity $1$, so $(\mathbb Z,\cdot,1)$ is a monoid. Natural powers in the integer multiplicative monoid start at $q^0=1$ and satisfy $q^{k+1}=q^kq$. [Ordered integer ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [Monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid) [Natural power recursion](https://alphabetamath.cc/item/def-group-power)

[F6] The product of a finite list starts at $1$ and appends each factor by multiplying on the right. [Finite product recursion](https://alphabetamath.cc/item/def-monoid-finite-product)

[F7] The preimage of a subset of the codomain consists of the inputs whose values lie in that subset. A listing is bijective onto a set if all its entries belong to the set and each element occurs exactly once. [Preimages and bijections](https://alphabetamath.cc/item/def-injection-surjection-bijection)

## Justification

**Given:** A prime-indexed family satisfying the hypotheses of the definition, with finite positive-exponent set $S$.

1.1 By [F2], $S$ has a bijective listing of some finite length. Prove by induction on this length that every set of primes with such a listing has exactly one strictly increasing listing. At length zero the set is empty and the empty listing is unique. For the induction step, take a set of primes $T$ admitting a bijective listing of length $n+1$. Every prime in $T$ is positive, so by [F3] the preimage $\iota^{-1}[T]$ is nonempty and maps onto $T$. Its least natural number maps to the least prime $m$ of $T$ because $\iota$ preserves order. Move the unique occurrence of $m$ to the last position by swapping entries if needed. The swap preserves one occurrence of each prime, so the new listing is bijective by [F7]. Deleting the last entry removes exactly $m$, so the first $n$ entries list $T\setminus\{m\}$ bijectively. By induction the remaining set has a unique strictly increasing listing. Prepending $m$ gives an increasing listing of $T$. Every increasing listing of $T$ must start with $m$ and then list exactly the remaining set, so it has the same tail. [given, F1, F2, F3, F4, F7]

2.1 For every local exponent the unique $k_q$ exists by [F3]. In particular an exponent of zero gives $k_q=0$. The power recursion starts at $1>0$ and multiplies by the positive prime $q$ at each step, so induction gives a positive integer for every factor. The product recursion likewise starts at $1$ and at each step multiplies two positive integers. Induction gives a positive integer for the product of the uniquely ordered list, including when it is empty. [given, F1, F3, F4, F5, F6, step 1.1]

3.1 Inserting an omitted prime inserts a factor $q^0=1$. In the product recursion the prefix value at the point of insertion therefore stays the same. Induction over the common suffix gives the same final product, and iteration gives the same value after any finite number of insertions. Thus the value agrees with the notation $\prod_q q^{a(\rho_q)}$ over all primes, interpreted as the product of the factors with positive exponent. [F4, F5, F6, step 2.1] ∎

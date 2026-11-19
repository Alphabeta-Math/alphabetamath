---
id: lem-euler-large-prime-obstruction-per-prime
kind: lemma
title: Lattice bound and support of the prime obstructions
status: published
domain: mathematics
deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - lem-square-residue-parity
  - math:def-real-numbers
  - math:thm-reals-ordered-field
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-natural-numbers
  - math:lem-nat-order-is-membership
  - lem-euler-mixed-lattice-count
  - def-euler-two-square-counts
  - lem-euler-two-square-count-bound
  - math:def-ordered-pair
  - math:def-cartesian-product
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-subset-and-proper-subset
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:def-finite-cardinality
  - math:thm-subset-of-a-finite-set
  - lem-count-pairs-by-bounded-fibers
  - lem-finite-obstruction-cover-bound
  - math:def-sum-over-a-finite-index-set
  - math:cor-cauchy-reals-lub-complete
  - math:thm-of-square-roots
formulation_deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - lem-square-residue-parity
  - math:def-real-numbers
  - math:thm-reals-ordered-field
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - def-euler-two-square-counts
  - math:def-ordered-pair
  - math:def-finite-cardinality
  - math:cor-cauchy-reals-lub-complete
  - math:thm-of-square-roots
argument_deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - lem-square-residue-parity
  - math:def-real-numbers
  - math:thm-reals-ordered-field
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-natural-numbers
  - math:lem-nat-order-is-membership
  - lem-euler-mixed-lattice-count
  - def-euler-two-square-counts
  - lem-euler-two-square-count-bound
  - math:def-ordered-pair
  - math:def-cartesian-product
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-subset-and-proper-subset
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:def-finite-cardinality
  - math:thm-subset-of-a-finite-set
  - lem-count-pairs-by-bounded-fibers
  - lem-finite-obstruction-cover-bound
  - math:def-sum-over-a-finite-index-set
  - math:cor-cauchy-reals-lub-complete
  - math:thm-of-square-roots
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  def-euler-mixed-four-square-representations: mathematical-premise
  def-euler-prime-obstruction-count: mathematical-premise
  lem-square-residue-parity: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  lem-euler-mixed-lattice-count: mathematical-premise
  def-euler-two-square-counts: mathematical-premise
  lem-euler-two-square-count-bound: mathematical-premise
  math:def-ordered-pair: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-function: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  lem-count-pairs-by-bounded-fibers: mathematical-premise
  lem-finite-obstruction-cover-bound: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:cor-cauchy-reals-lub-complete: mathematical-premise
  math:thm-of-square-roots: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: PDF p. 5, Lemma 4.2, proof through the bound on p
dependency_level: 4
---

## Statement

Let $n=2m$, where $m$ is a positive odd integer. An integer is positive if it exceeds zero, even if it is $2k$, and odd if it is $2k+1$, for an integer $k$. A pair has opposite parity if one entry is even and the other is odd. Let $p\in\mathcal P_3$, the set of primes for which $4$ divides $p-3$. An integer $d$ divides an integer $a$ when $a=dk$ for some integer $k$, and a prime is an integer greater than $1$ with only $1$ and itself as positive divisors.

A mixed-parity representation of $n$ is an ordered integer quadruple whose squares sum to $n$ and whose first and last coordinate pairs each have opposite parity. Signs and positions are retained. A pair is obstructed by $p$ if $p$ divides both entries. Let $b_p(n)$ count the mixed-parity representations with at least one obstructed pair, counting each quadruple once.

For a positive integer $u$, let $r_2(u)$ count the signed, ordered integer pairs whose squares sum to $u$, including pairs with a zero entry. Let $M(n)$ be the greatest, over integers $1\le u\le n$, of the product of $e+1$ over the primes $q$ for which $4$ divides $q-1$ and $q^e$ divides $u$ but $q^{e+1}$ does not, with $e\ge1$. Here a power is repeated multiplication and an empty product is $1$.

With either obstructed pair position specified, its divided pair, obtained by dividing both entries by $p$, has at most $2(n/p^2+1)$ possibilities. For each such divided pair, the other pair has positive square sum and at most $4M(n)$ representations. Consequently $b_p(n)\le16M(n)(n/p^2+1)$. If $b_p(n)>0$, then $p\le\sqrt n$. Read counts and integers as real numbers in these inequalities, and write $\sqrt n$ for the unique nonnegative real number whose square is $n$.

## Statement references

[[def-euler-prime-classes]]

[[def-euler-mixed-four-square-representations]]

[[def-euler-prime-obstruction-count]]

[[def-euler-two-square-counts]]

## Facts & Assumptions

[F1] Write $\mathbb Z$ for the integers, with their usual addition, multiplication and order, and use $z^2=z\cdot z$. The relation $d\mid a$ means that $a$ is an integer multiple of $d$. The prime class $\mathcal P_3$ consists of primes $p$ satisfying $p-3=4k$ for an integer $k$. [[math:def-integers]] [[math:def-int-operations]] [[math:def-int-order]] [[math:def-divides-in-z]] [[def-euler-prime-classes]]

[F2] The mixed-parity representations form a finite set. The exceptional set $E_p(n)$ consists of those representations with an obstructed pair in at least one position, and $b_p(n)$ is its cardinality. [[def-euler-mixed-four-square-representations]] [[def-euler-prime-obstruction-count]]

[F3] An opposite-parity integer pair has positive square sum. Exact division of both entries by a positive odd common divisor preserves the parity of each entry. [[lem-square-residue-parity]]

[F4] Read an integer $k$ in $\mathbb R$ as the class of the constant rational sequence with value $k/1$. Read a natural-number count first as its nonnegative integer. These inclusions preserve addition, multiplication and order, and the real numbers form an ordered field. In particular, addition preserves inequalities and multiplication by a positive real preserves their direction. For $b\ne0$, $a/b$ is the unique real $x$ such that $bx=a$. [[math:def-real-numbers]] [[math:lem-nat-embeds-int]] [[math:lem-int-embeds-rat]] [[math:lem-rat-embeds-dense]] [[math:thm-reals-ordered-field]]

[F5] Every positive integer is at least $1$. Indeed its natural-number representative $k$ is nonzero, so $0\in k$ and $1=\{0\}\subseteq k$. Inclusion gives $1\le k$ in the natural-number order, and the integer embedding preserves that order. [[math:def-natural-numbers]] [[math:lem-nat-order-is-membership]] [[math:lem-nat-embeds-int]]

[F6] For every nonnegative real $t$, the finite set $S_t$ of signed, ordered opposite-parity integer pairs with square sum at most $t$ has cardinality at most $2(t+1)$. [[lem-euler-mixed-lattice-count]]

[F7] For positive integers $u,n$ with $1\le u\le n$, the count $r_2(u)$ defined in the statement satisfies $r_2(u)\le 4M(n)$ for the stated maximum $M(n)$. [[def-euler-two-square-counts]] [[lem-euler-two-square-count-bound]]

[F8] An ordered pair $(a,b)$ is $\{\{a\},\{a,b\}\}$, and equality of ordered pairs is equivalent to equality in each position. The Cartesian product $A\times B$ consists of the pairs with first entry in $A$ and second entry in $B$. A condition on elements of a set specifies the subset of elements satisfying it. A function assigns a unique output to each input. It is a bijection onto its target when different inputs have different outputs and every element of the target occurs. [[math:def-ordered-pair]] [[math:thm-the-characterising-property-of-ordered-pairs]] [[math:def-cartesian-product]] [[math:def-subset-and-proper-subset]] [[math:def-function]] [[math:def-injection-surjection-bijection]]

[F9] The cardinality $|A|$ of a finite set $A$ is its number of distinct elements. It is a nonnegative integer when read in $\mathbb Z$, equals zero exactly for the empty set, and is preserved by bijection. A subset of a finite set is finite and has cardinality at most that of the containing set. [[math:def-finite-cardinality]] [[math:thm-subset-of-a-finite-set]]

[F10] For a finite set of ordered pairs, if the number of distinct first entries is at most $A\ge0$ and at most $B\ge0$ pairs have any specified first entry, then the total count is at most $AB$. For two subsets of a finite set, the set of elements belonging to at least one subset has cardinality at most the sum of their cardinalities, since the sum over the two indices adds the two counts. [[lem-count-pairs-by-bounded-fibers]] [[lem-finite-obstruction-cover-bound]] [[math:def-sum-over-a-finite-index-set]]

[F11] The real numbers have the least-upper-bound property, meaning every nonempty, bounded-above set of reals has a least real upper bound. In an ordered field with this property, every nonnegative element has a unique nonnegative square root. [[math:cor-cauchy-reals-lub-complete]] [[math:thm-of-square-roots]]

## Proof

**Given:** $n=2m$ for a positive odd integer $m$ and $p\in\mathcal P_3$.

**Goal:** Bound the choices in each specified pair position, the total obstruction count and the primes with positive count.

1.1 Since $m>0$, one has $n>0$ and therefore $n\ge1$. By the definition of $\mathcal P_3$, $p>1$ and $p=4k+3=2(2k+1)+1$ for an integer $k$. Thus $p$ is positive and odd, $p^2>0$, and $t=n/p^2$ is a positive real. Applying the two-square bound at $u=1$ gives $4M(n)\ge r_2(1)\ge0$. [given, F1, F4, F5, F7, F9]

2.1 For $j=1,2$, let $B_j$ be the subset of $E_p(n)$ obstructed in position $j$, where position $1$ is the first coordinate pair and position $2$ the last. Both sets are finite. For a fixed $j$ and an element of $B_j$, write the pair in that position as $(pu,pv)$ with $u,v\in\mathbb Z$, and the other pair as $(y,z)$. Divisibility gives the integer quotients and cancellation by $p>0$ gives their uniqueness. Both $(u,v)$ and $(y,z)$ have opposite parity, the former by preservation of parity under division by $p$. [F1, F2, F3, F4, F8, F9, step 1.1]

3.1 The square equation becomes $p^2(u^2+v^2)+y^2+z^2=n$. Put $h=u^2+v^2$ and $w=y^2+z^2$. Both are positive integers by opposite parity, hence $h,w\ge1$. Since $p^2h\ge p^2>0$ and $w>0$, the equation gives $w\le n$ and $h\le n/p^2=t$. Thus $(u,v)\in S_t$, giving at most $2(t+1)$ possible divided pairs. For a specified divided pair, the other pair has the fixed positive square sum $w=n-p^2(u^2+v^2)$ with $1\le w\le n$. [F3, F4, F5, F6, F9, step 1.1, step 2.1]

3.2 For the fixed $j$, let $T=\mathbb Z\times\mathbb Z$ and let $D_j$ consist of the elements of $T\times T$ of the form $((u,v),(y,z))$ obtained from an element of $B_j$ by the rule in Step 2.1. This rule is a bijection onto $D_j$. Every element of $D_j$ is obtained by the rule, and equal outputs determine the same two original pairs in their original positions by multiplying $(u,v)$ by $p$ and placing it in position $j$. Thus $D_j$ is finite and $|D_j|=|B_j|$. [F2, F8, F9, step 2.1]

4.1 Fix a first entry $(u,v)$ that occurs in $D_j$. The elements of $D_j$ with that first entry are in bijection with the subset of pairs of square sum $w=n-p^2(u^2+v^2)$ that occur as their second entries. The bijection keeps the second entry, and equality of second entries then gives equality of both entries. This subset has at most $r_2(w)\le4M(n)$ elements by $1\le w\le n$. The bound on first entries in Step 3.1 and the counting rule in F10 now give $|B_j|=|D_j|\le 2(t+1)\cdot4M(n)=8M(n)(t+1)$. [F4, F7, F8, F9, F10, step 1.1, step 3.1, step 3.2]

5.1 Every element of $E_p(n)$ lies in at least one of $B_1,B_2$. The two-subset bound therefore gives $b_p(n)=|E_p(n)|\le |B_1|+|B_2|\le16M(n)(n/p^2+1)$. [F2, F4, F10, step 4.1]

6.1 If $b_p(n)>0$, then $E_p(n)$ contains a representation, so Step 3.1 applies in one of its obstructed positions. It gives $p^2\le p^2h\le n$. For $s=\sqrt n$, if $p>s$ then $(p-s)(p+s)>0$ because $s\ge0$ and $p>0$. This would give $p^2>s^2=n$. Hence $p\le\sqrt n$, which completes the bounds. [F2, F4, F9, F11, step 1.1, step 3.1, step 4.1, step 5.1] ∎

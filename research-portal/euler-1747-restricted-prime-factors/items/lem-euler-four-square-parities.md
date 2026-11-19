---
id: lem-euler-four-square-parities
kind: lemma
title: The six parity placements in a four-square representation
status: draft
domain: mathematics
deps:
  - def-euler-four-square-representations
  - lem-square-residue-parity
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-congruence-modulo-an-integer
  - math:def-divides-in-z
  - math:def-natural-numbers
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:thm-subset-of-a-finite-set
  - lem-permutation-fibers-have-equal-size
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - math:lem-nat-embeds-int
  - math:lem-nat-order-is-membership
  - math:def-function
  - math:def-cartesian-product
  - math:def-power-set
  - math:def-injection-surjection-bijection
  - math:thm-the-characterising-property-of-ordered-pairs
formulation_deps:
  - def-euler-four-square-representations
  - lem-square-residue-parity
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-congruence-modulo-an-integer
  - math:def-divides-in-z
  - math:def-natural-numbers
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:thm-subset-of-a-finite-set
argument_deps:
  - def-euler-four-square-representations
  - lem-square-residue-parity
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-congruence-modulo-an-integer
  - math:def-divides-in-z
  - math:def-natural-numbers
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:thm-subset-of-a-finite-set
  - lem-permutation-fibers-have-equal-size
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - math:lem-nat-embeds-int
  - math:lem-nat-order-is-membership
  - math:def-function
  - math:def-cartesian-product
  - math:def-power-set
  - math:def-injection-surjection-bijection
  - math:thm-the-characterising-property-of-ordered-pairs
dependency_roles:
  def-euler-four-square-representations: mathematical-premise
  lem-square-residue-parity: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  lem-permutation-fibers-have-equal-size: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:def-function: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-power-set: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §2, text between (2.1) and (2.2)
dependency_level: 1
---

## Statement

Let $n$ be a positive integer ($n\in\mathbb Z$ and $0<n$) with $n\equiv2\pmod4$, meaning $n-2=4q$ for some integer $q$. Let $\mathcal R(n)$ be the set of ordered integer quadruples $x=(x_1,x_2,x_3,x_4)$ with $x_1^2+x_2^2+x_3^2+x_4^2=n$, where $x_i^2=x_i\cdot x_i$. The entries, also called coordinates, may have either sign or be zero. An integer is odd if it has the form $2a+1$ and even if it has the form $2a$, with $a$ an integer.

Every $x\in\mathcal R(n)$ has exactly two odd coordinates. For a two-element subset $D$ of the position set $I=\{1,2,3,4\}$, let $X_D$ be the set of quadruples in $\mathcal R(n)$ whose odd coordinates occur exactly at the positions in $D$. The six possible sets $D$ all give the same finite cardinality $|X_D|$, the number of elements of $X_D$. Exactly four of these choices of $D$ select one position from each of $\{1,2\}$ and $\{3,4\}$, so both coordinate pairs have opposite parity, meaning one even and one odd entry in each pair.

## Statement references

[[def-euler-four-square-representations]]

[[lem-square-residue-parity]]

[[math:def-integers]]

[[math:def-int-operations]]

[[math:def-int-order]]

[[math:def-congruence-modulo-an-integer]]

[[math:def-divides-in-z]]

[[math:def-natural-numbers]]

[[math:def-subset-and-proper-subset]]

[[math:def-finite-cardinality]]

[[math:thm-subset-of-a-finite-set]]

## Facts & Assumptions

[F1] Write $\mathbb Z$ for the [[math:def-integers|integers]], with [[math:def-int-operations|integer addition, subtraction and multiplication]] and [[math:def-int-order|integer order]], in which positive means strictly greater than $0$. Integer addition is associative and commutative, multiplication distributes over it, and adding the same integer to both sides preserves order. [[math:thm-int-ordered-ring]]

[F2] The [[math:def-natural-numbers|natural number]] $j$ is the set of its predecessors, with $0=\varnothing$ and successor $j\cup\{j\}$. The natural order satisfies $a<b$ exactly when $a\in b$. The strictly order-preserving map $j\mapsto[(j,0)]$ sends the natural $0$ and $1$ to the integer $0$ and $1$, so $0<1$ also holds in $\mathbb Z$. [[math:lem-nat-order-is-membership]] [[math:lem-nat-embeds-int]]

[F3] The [[def-euler-four-square-representations|four-square representation definition and its justification]] give a finite set $\mathcal R(n)$ for every positive integer $n$. An ordered quadruple is determined by its coordinates, and any four integers with their positions specified give such a quadruple if their squares sum to $n$.

[F4] By [[lem-square-residue-parity|square residues and opposite parity]], every integer is exactly one of even or odd, and its square is congruent to $0$ modulo $4$ if it is even and to $1$ modulo $4$ if it is odd. [[math:def-congruence-modulo-an-integer|Congruence]] $a\equiv b\pmod4$ means that $4$ [[math:def-divides-in-z|divides]] $a-b$, so $a=4q+b$ for some integer $q$.

[F5] By [[math:thm-division-algorithm-in-z|division with remainder in the integers]], for any integer $a$ and positive integer $b$ there are unique integers $q,r$ with $a=bq+r$ and $0\le r<b$.

[F6] A [[math:def-subset-and-proper-subset|subset]] contains only elements of its ambient set. Selecting the elements of a set by a fixed condition gives a unique subset. Every subset of a finite set is finite. [[math:thm-subset-of-a-finite-set]]

[F7] The [[math:def-cartesian-product|Cartesian product]] $A\times B$ consists of the ordered pairs $(a,b)$ with $a\in A$ and $b\in B$. Two ordered pairs are equal exactly when their first entries agree and their second entries agree. [[math:thm-the-characterising-property-of-ordered-pairs|Ordered-pair equality]] A [[math:def-function|function]] $A\to B$ is specified by a subset of $A\times B$ containing exactly one pair with each first entry $a\in A$. Its value at $a$ is the second entry of that pair. The [[math:def-power-set|power set]] of a set is the set of all its subsets.

[F8] A [[math:def-injection-surjection-bijection|bijection]] is a function for which every element of the target has exactly one input mapping to it. A set is finite if it admits a bijection to a natural number viewed as the set of its predecessors, and the unique such number is its [[math:def-finite-cardinality|cardinality]]. A bijection from a finite set gives the target the same cardinality.

[F9] In [[lem-permutation-fibers-have-equal-size|the equal counting lemma for coordinate positions]], let $I$ be a finite set and let $S$ be a finite set of functions $I\to\mathbb Z$ closed under reindexing. A permutation $\pi$ is a bijection $I\to I$, and reindexing a function $f$ by $\pi$ puts $f(\pi^{-1}(j))$ at position $j$, where $\pi^{-1}(j)$ is the unique preimage of $j$. For every subset $D$ of $I$, the functions in $S$ that are odd exactly on $D$ form its fiber at $D$. The lemma gives equal cardinalities of these fibers whenever the subsets of positions have equal cardinalities.

## Justification

The position labels $1,2,3,4$ are natural numbers. The predecessor description in F2 gives $5=\{0,1,2,3,4\}$, so selecting its four nonzero labels defines $I$. The oddness condition in F4 determines which entries of each quadruple are odd. Thus for each $D$ the condition in the statement selects a unique subset $X_D$ of $\mathcal R(n)$. This subset is finite by F3 and F6, so F8 defines $|X_D|$. The even and odd cases are exhaustive and disjoint by F4, making opposite parity equivalent to exactly one odd entry in the pair.

## Proof

**Given:** A positive integer $n$ with $n\equiv2\pmod4$.

**Goal:** Show that every quadruple has exactly two odd coordinates, that each of the six choices of their positions gives the same count, and that exactly four choices give opposite parity in both pairs.

1.1 Fix a quadruple in $\mathcal R(n)$. At each position $i$, write $x_i^2=4q_i+\epsilon_i$ with $\epsilon_i=0$ for an even entry and $\epsilon_i=1$ for an odd entry. Then $n=4(q_1+q_2+q_3+q_4)+k$, where $k=\epsilon_1+\epsilon_2+\epsilon_3+\epsilon_4$ is the number of odd entries viewed as an integer. Indeed, zero entries among the $\epsilon_i$ add nothing and each $1$ contributes one to the count. Adding $1$ increases an integer strictly, so the sums for zero through four odd entries increase strictly from $0$ to $4$. [given, F1, F2, F3, F4]

1.2 The set $I$ is finite because it is a subset of the finite natural number $5$. In the power set of $I\times\mathbb Z$, select the functions $f:I\to\mathbb Z$ with $f(1)^2+f(2)^2+f(3)^2+f(4)^2=n$ and call this set $S$. For each $x\in\mathcal R(n)$, select the pairs $(j,x_j)$ with $j\in I$ in $I\times\mathbb Z$. Each $i\in I$ occurs in the pair $(i,x_i)$. If $(i,a)$ is selected, it equals $(j,x_j)$ for some $j\in I$. Ordered-pair equality gives $i=j$ and $a=x_j=x_i$. Thus the selected pairs define a function $f_x$ with $f_x(i)=x_i$ at each position, so $f_x\in S$. Now select the pairs $(y,f_y)$ with $y\in\mathcal R(n)$ in $\mathcal R(n)\times S$. Each $x\in\mathcal R(n)$ occurs in the pair $(x,f_x)$. If $(x,g)$ is selected, it equals $(y,f_y)$ for some $y\in\mathcal R(n)$. Ordered-pair equality gives $x=y$ and $g=f_y=f_x$, so this graph defines a function. For any $f\in S$, put $x=(f(1),f(2),f(3),f(4))$. By the definition of $S$, this quadruple lies in $\mathcal R(n)$. By F7, membership of $(i,a)\in I\times\mathbb Z$ in each of the graphs $f_x$ and $f$ is equivalent to $a=f(i)$. By F6, the condition selects a unique subset of $I\times\mathbb Z$, so $f_x=f$. Conversely, the four values of $f_x$ recover $x$. Thus each $f\in S$ has exactly one preimage, so the function is a bijection and $S$ is finite. [F1, F2, F3, F6, F7, F8]

2.1 Since $n=4q+2$ and $0\le2<4$, the remainder upon division by the positive integer $4$ is $2$. If $k=4$, the expression in Step 1.1 is a multiple of $4$, with remainder $0$, contrary to uniqueness. For $0\le k<4$ that expression has remainder $k$, hence $k=2$. Thus the odd positions form a two-element subset of $I$ for every quadruple. [given, F1, F2, F4, F5, step 1.1]

2.2 Under a permutation of $I$, the reindexed function uses the entry from each original position exactly once. Associativity and commutativity of integer addition keep its sum of four squares equal to $n$, so the reindexed function lies in $S$. Let $F_D$ be the fiber in $S$ at $D$. Since $f_x(i)=x_i$ for all $i\in I$, $f_x\in F_D$ exactly when $x\in X_D$. Select from the graph of the bijection in Step 1.2 the pairs whose first entry lies in $X_D$. These pairs lie in $X_D\times F_D$ and give exactly one value for each $x\in X_D$. Each $f\in F_D$ has a unique preimage in $\mathcal R(n)$ under the bijection in Step 1.2, and by the parity equivalence this preimage lies in $X_D$. Thus the restricted function is a bijection $X_D\to F_D$. By F8, $|X_D|=|F_D|$. Applying F9 to the finite sets $I$ and $S$ now gives equal counts for all two-element position subsets. [F1, F4, F6, F7, F8, F9, step 1.2]

3.1 Among the two-element subsets of $I$, the ones containing $1$ are $\{1,2\},\{1,3\},\{1,4\}$. The ones omitting $1$ and containing $2$ are $\{2,3\},\{2,4\}$, and the only one omitting both $1$ and $2$ is $\{3,4\}$. The four distinct choices $\{1,3\},\{1,4\},\{2,3\},\{2,4\}$ are exactly the ones that place one odd entry in each pair. The other entry of each pair is then even. This proves the claimed six equal counts and identifies the four choices yielding opposite parity in both pairs. [F2, F4, step 2.1, step 2.2] ∎

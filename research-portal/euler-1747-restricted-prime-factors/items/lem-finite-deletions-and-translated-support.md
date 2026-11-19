---
id: lem-finite-deletions-and-translated-support
kind: lemma
title: Repeated finite deletions and translation of indicator support
status: published
domain: mathematics
deps:
  - math:def-natural-numbers
  - math:def-nat-order
  - math:lem-nat-order-is-membership
  - math:lem-nat-discrete
  - math:def-finite-cardinality
  - math:def-injection-surjection-bijection
  - math:thm-subset-of-a-finite-set
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-nat-addition
  - math:thm-int-ordered-ring
  - math:def-indexed-family
  - math:def-function
  - math:def-subset-and-proper-subset
  - math:def-ordered-pair
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-cartesian-product
  - math:def-power-set
  - math:def-unordered-pair-and-singleton
  - math:def-set-difference-and-symmetric-difference
  - math:def-indexed-union-and-intersection
  - math:def-axiom-of-extensionality
  - math:thm-induction-principle
dependency_roles:
  math:def-natural-numbers: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-nat-addition: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-indexed-family: mathematical-premise
  math:def-function: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-ordered-pair: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-power-set: mathematical-premise
  math:def-unordered-pair-and-singleton: mathematical-premise
  math:def-set-difference-and-symmetric-difference: mathematical-premise
  math:def-indexed-union-and-intersection: mathematical-premise
  math:def-axiom-of-extensionality: mathematical-premise
  math:thm-induction-principle: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $\mathbb N$ be the natural numbers including $0$, and let $m^+$ denote the successor of $m$. A set is finite if, for some $n\in\mathbb N$, there is a bijection from the set onto $\{j\in\mathbb N:j<n\}$, the first $n$ natural numbers. Let $D$ be a finite subset of the integers $\mathbb Z$, and let $E_1,\ldots,E_r$ be an indexed family of subsets of $\mathbb Z$ for $r\in\mathbb N$, with one specified set $E_j$ for each $1\le j\le r$.

For sets $A,B$, the set difference $A\setminus B$ consists of the elements of $A$ outside $B$. For $0\le m\le r$, let $U_m=\bigcup_{1\le j\le m}E_j$ be the union of the first $m$ sets, consisting of the elements that belong to at least one of them. The empty union $U_0$ is the empty set. Start at $C_0=D$ and at each index $m^+$ with $0\le m<r$ delete $E_{m^+}$ by setting $C_{m^+}=C_m\setminus E_{m^+}$. This determines a unique family $C_0,\ldots,C_r$ of finite sets, with $C_m=D\setminus U_m$ for every $0\le m\le r$.

Write $\mathbb Z_{\ge0}=\{t\in\mathbb Z:0\le t\}$ for the nonnegative integers. Let $S\subseteq\mathbb Z_{\ge0}$. Its binary indicator, extended by zero to all integers, is the function with value $\varepsilon_t=1$ if $t\in S$ and value $\varepsilon_t=0$ otherwise. Its support, the set of arguments where the value is $1$, is $S$. For an integer $i$, the translate $i+S$ consists of the sums $i+s$ with $s\in S$. With $k-i=k+(-i)$, for every integer $k$,
$$k\in i+S\quad\Longleftrightarrow\quad k\ge i\ \text{and}\ \varepsilon_{k-i}=1.$$

## Statement references

[[math:def-injection-surjection-bijection|Bijection]]

## Justification

The condition $1\le j\le m$ selects a subset of the original index set when $m\le r$, by transitivity of the natural order. Keeping exactly the pairs of the original family with those indices defines its restriction by [[math:def-subset-and-proper-subset|separation within a set]]. The ordered-pair equality criterion in [F2] gives each retained pair a unique first coordinate. Every selected index keeps its original value, and that value is unique by the [[math:def-indexed-family|indexed-family definition]]. Its [[math:def-indexed-union-and-intersection|indexed union]] exists and contains an element exactly when some selected set contains it.

Separation inside $\mathbb Z$ gives $\mathbb Z_{\ge0}$ and $i+S$, since the stated integer comparison and addition define conditions on integers. The indicator graph is formed by separation inside $\mathbb Z\times\{0,1\}$, the set of pairs with first coordinate an integer and second coordinate either $0$ or $1$. For each integer $t$, keep $(t,1)$ if $t\in S$ and $(t,0)$ otherwise. The ordered-pair equality criterion in [F2] makes the coordinates unambiguous, and the two membership cases give exactly one value at each integer. Thus the graph defines a function. Its support is formed by separation on the condition $\varepsilon_t=1$. Since the integer values $0$ and $1$ are distinct by [F6], this condition holds exactly when $t\in S$. [[math:def-cartesian-product|Cartesian product]] [[math:def-unordered-pair-and-singleton|Unordered pair]] [[math:def-function|Function]]

## Facts & Assumptions

[F1] In the [[math:def-natural-numbers|natural numbers]], $0$ is empty and $m^+$ consists of the elements of $m$ together with $m$ itself. In the [[math:def-nat-order|natural order]], $j<m$ means $j\le m$ and $j\ne m$. The order satisfies $j\le m$ exactly when $j\subseteq m$, and $j<m^+$ exactly when $j\le m$ by [[math:lem-nat-order-is-membership|the membership description of natural order]]. The empty set is a subset of every set, so $0\le m$. Transitivity of inclusion gives transitivity of $\le$. Also $m<r$ exactly when $m^+\le r$ by [[math:lem-nat-discrete|discreteness of natural order]].

[F2] A subset has all its elements in the ambient set. [[math:def-subset-and-proper-subset|Separation]] selects the elements satisfying a specified condition inside an existing set. The [[math:def-power-set|power set]] $\mathcal P(D)$ consists of all subsets of $D$, and the [[math:def-cartesian-product|Cartesian product]] $A\times B$ consists of the [[math:def-ordered-pair|ordered pairs]] $(a,b)$ with $a\in A$ and $b\in B$. The [[math:thm-the-characterising-property-of-ordered-pairs|ordered-pair equality criterion]] states that $(a,b)=(c,d)$ exactly when $a=c$ and $b=d$. Such a set of pairs defines a [[math:def-function|function from]] $A$ to $B$ if it assigns exactly one $b$ to each $a$.

[F3] Membership in a [[math:def-set-difference-and-symmetric-difference|set difference]] requires membership in the first set and exclusion from the second. Membership in an [[math:def-indexed-union-and-intersection|indexed union]] requires membership in at least one set at a selected index. By [[math:def-axiom-of-extensionality|extensionality]], sets with the same elements are equal.

[F4] [[math:thm-induction-principle|Induction]] applies to a property of natural numbers once it holds at $0$ and passes from each $m$ to $m^+$. Every subset of a finite set is finite by [[math:thm-subset-of-a-finite-set|the finite-subset theorem]], using the supplied [[math:def-finite-cardinality|definition of finiteness]].

[F5] In the [[math:def-integers|integers]] an integer is a class of pairs of naturals representing a difference. The [[math:def-int-operations|integer operations]] supply addition, negation, $0$ and $1$, and the [[math:def-int-order|integer order]] compares $[(a,b)]\le[(c,d)]$ by $a+d\le b+c$ in the naturals, where the sums use [[math:def-nat-addition|natural-number addition]]. By [[math:thm-int-ordered-ring|the ordered-ring theorem for the integers]], addition on the integers is associative and commutative, has identity $0$ and inverse $-i$ at $i$, and preserves $\le$ upon adding the same integer to both sides.

[F6] The natural numeral $1$ is $0^+$ by the [[math:def-natural-numbers|definition of the natural numbers]], so $0<1$ in $\mathbb N$ by the [[math:lem-nat-order-is-membership|successor inequality]]. The [[math:def-int-order|representative criterion for positivity]] gives $0<[(a,b)]$ in $\mathbb Z$ exactly when $b<a$ in $\mathbb N$. The integer numeral $1=[(1,0)]$ from the [[math:def-int-operations|integer operations]] is therefore positive, so the integer values $0$ and $1$ are distinct.

## Proof

**Given:** The finite set $D$, the number of updates $r$, the sets $E_j$, the subset $S$ of the nonnegative integers, and the integer $i$.

**Goal:** Determine every set left by deletion and characterize the integers in $i+S$.

1.1 For $0\le m\le r$, let $A_m=D\setminus U_m$. Each $A_m$ exists and is contained in $D$ by the set difference definition. To form the graph of the family, separate the pairs satisfying $A=D\setminus U_m$ inside $I\times\mathcal P(D)$, where $I=\{m\in\mathbb N:0\le m\le r\}$. The ordered-pair equality criterion makes the index and value of each pair unique. At each $m$ there is exactly one such $A$ by extensionality, so this graph defines a function with domain $I$. [given, F1, F2, F3]

1.2 If $k\in i+S$, then $k=i+s$ for some $s\in S$. Since $0\le s$, addition of $i$ gives $i\le k$. Adding $-i$ to the equality and using the additive laws gives $k-i=s$, so $\varepsilon_{k-i}=1$. [given, F5]

2.1 The union $U_0$ is empty, so $A_0=D$. For $0\le m<r$ the successor $m^+$ lies in $I$. Its prefix of deletion indices consists of the indices from the prefix at $m$ and the single index $m^+$. For a natural number $j$, the inequality $j<m^+$ holds exactly when $j\le m$, and $m^+$ is nonzero since it contains $m$. Thus $x\notin U_{m^+}$ holds exactly when $x\notin U_m$ and $x\notin E_{m^+}$. Membership in $A_{m^+}$ is therefore equivalent to membership in $A_m\setminus E_{m^+}$, so these sets are equal by extensionality. [step 1.1, F1, F3]

3.1 Any family $C$ satisfying the deletion rules must agree with $A$ at $0$. Apply induction to the property that $C_m=A_m$ whenever $m\le r$. If $m^+\le r$, then $m<r$ and the induction hypothesis gives $C_m=A_m$. The update and step 2.1 give $C_{m^+}=C_m\setminus E_{m^+}=A_{m^+}$. If $m^+\le r$ fails, the property at $m^+$ is vacuous. Hence every $C_m$ equals $A_m$ in the required range, and each is finite because it is a subset of the finite set $D$. [given, step 1.1, step 2.1, F1, F4]

4.1 If $k\ge i$ and $\varepsilon_{k-i}=1$, then $k-i\in S$, since outside $S$ the indicator is $0$ and [F6] gives $0\ne1$ in $\mathbb Z$. The additive laws give $k=i+(k-i)$, so $k\in i+S$. This proves the translated-support equivalence, and steps 2.1 and 3.1 give the unique deletion family and its formula at every stage. [given, F5, F6, step 2.1, step 3.1, step 1.2] ∎

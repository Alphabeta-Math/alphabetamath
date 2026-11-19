---
title: Quarter-turn orbits and integer labels
status: draft
research_item: lem-euler-mixed-lattice-orbit-labels
dependency_level: 2
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, Lemma 4.1, proof, orbit representatives, label and norm identity
---

PDF p. 4: ` Lemma 4.1, proof, orbit representatives, label and norm identity `

## Prerequisites

- [def-euler-mixed-lattice-count](item-def-euler-mixed-lattice-count)
- [lem-square-residue-parity](item-lem-square-residue-parity)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)
- [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:thm-recursion](https://alphabetamath.cc/item/thm-recursion)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)


## Statement

Write $\mathbb Z^2=\mathbb Z\times\mathbb Z$ for the set of ordered pairs of integers. Let $S$ consist of pairs of opposite parity, meaning one entry has the form $2k$ and the other has the form $2m+1$ for integers $k,m$. Put $Q(x,y)=x^2+y^2$, where $z^2=z\cdot z$.

The quarter-turn is the transformation $R(x,y)=(-y,x)$. For a pair $p$ in $S$, its orbit $O(p)$ is the set of pairs obtained by applying $R$ repeatedly, starting with $p$ itself. Every orbit has exactly four elements and a unique representative, meaning its sole member $(x,y)$ with $x>0$ and $y\ge0$. For each real $t\ge0$, let $S_t$ consist of the pairs in $S$ with $Q(x,y)\le t$, with the square sum compared to $t$ in the real order. If $p$ belongs to $S_t$, then all members of $O(p)$ belong to $S_t$.

For the representative $(x,y)$ there are unique integers $u,v$ satisfying
$$x+y=2u+1,\qquad x-y=2v+1,\qquad u\ge0,\qquad -u\le v\le u.$$
The integer label $L=u^2+u+v+1$ is positive, and different representatives have different labels. For each nonnegative integer $u$, the labels of the representatives in $S$ with that value of $u$ are exactly the integers from $u^2+1$ to $(u+1)^2$, inclusive. Moreover,
$$\frac{x^2+y^2+1}{2}=L+v^2\ge L.$$

## Statement references

[def-euler-mixed-lattice-count](item-def-euler-mixed-lattice-count)

[lem-square-residue-parity](item-lem-square-residue-parity)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)

[math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)

[math:def-function](https://alphabetamath.cc/item/def-function)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:thm-recursion](https://alphabetamath.cc/item/thm-recursion)

## Justification

The coordinates of an ordered pair are uniquely determined. The formula for $R$ therefore assigns a single value to each pair, and Step 1.1 verifies that the value stays in $S$. For each $p\in S$, natural-number recursion gives a unique function $g_p$ from the natural numbers to $S$ with $g_p(0)=p$ and $g_p(\sigma(n))=R(g_p(n))$, where $\sigma$ is the natural-number successor. Separation gives $S$ as a subset of $\mathbb Z^2$ and gives $O(p)$ as the subset of $S$ consisting of the values of $g_p$. Step 1.1 shows that these are exactly the first four values, starting at $p$. The sign condition selects one member by Step 2.1. The odd forms determine $u,v$ uniquely because multiplication by $2$ is strictly increasing on the integers, as shown in Step 1.2. Integer arithmetic then gives one label for each representative. The fraction in the statement is the exact integer quotient, whose existence is the equality in Step 4.2 and whose uniqueness follows from the same strict increase.

## Facts & Assumptions

[F1] The integer construction uses classes of natural-number pairs with $(a,b)$ and $(c,d)$ in the same class exactly when $a+d=b+c$ ([math:def-integers](https://alphabetamath.cc/item/def-integers)). Use integer addition, multiplication and negation, with $x-y=x+(-y)$, $2=1+1$ and the defined integers $0=[(0,0)]$, $1=[(1,0)]$ ([math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)). Strict order $a<b$ means $a\le b$ with $a\ne b$ ([math:def-int-order](https://alphabetamath.cc/item/def-int-order)). The order is total and compatible with addition, products of positive elements are positive, and integer addition and multiplication are associative and commutative, with distributivity, identities $0,1$ and additive inverses ([math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)).

[F2] The product of two sets consists of the ordered pairs with first entry in the first set and second entry in the second set ([math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair), [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)). Two ordered pairs agree exactly when both corresponding entries agree ([math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)). Separation forms the subset of a given set whose members satisfy a specified formula ([math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)).

[F3] Each integer has exactly one parity, even of the form $2k$ or odd of the form $2k+1$, and $0$ is even ([lem-square-residue-parity](item-lem-square-residue-parity)).

[F4] The cutoff set $S_t$ consists of the pairs in $S$ satisfying $Q(x,y)\le t$ for real $t\ge0$ ([def-euler-mixed-lattice-count](item-def-euler-mixed-lattice-count)). The comparison sends an integer $k$ to the class $[(k,1)]$, written $k/1$ ([math:def-rationals](https://alphabetamath.cc/item/def-rationals), [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)). It then sends that rational to the real represented by its constant sequence and uses the real order ([math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense), [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers), [math:def-real-order](https://alphabetamath.cc/item/def-real-order)). Equal square sums thus yield equal real values in the comparison.

[F5] The natural number $0$ is the empty set, and the successor of $n$ is $n\cup\{n\}$. Thus natural $1=\{0\}$ and natural $4=\{0,1,2,3\}$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)). For natural numbers $m,n$, $m<n$ exactly when $m\in n$, and $m\le n$ exactly when every element of $m$ belongs to $n$. Every nonzero natural number $n$ contains $0$ ([math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)). The map $\iota(n)=[(n,0)]$ preserves order, is one-to-one, and has as its image precisely the nonnegative integers ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)).

[F6] A function from one set to another assigns exactly one target to each input, and it is a bijection when each target is attained exactly once ([math:def-function](https://alphabetamath.cc/item/def-function), [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)). A set has finite cardinality $n$, meaning it has exactly $n$ elements, when there is a bijection from the natural number $n$ to that set ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)).

[F7] For any set $A$, element $a\in A$ and function $f:A\to A$, there is a unique function $g:\mathbb N\to A$ with $g(0)=a$ and $g(\sigma(n))=f(g(n))$ for every natural $n$ ([math:thm-recursion](https://alphabetamath.cc/item/thm-recursion)).

[F8] A property of the natural numbers holds for all of them if it holds at $0$ and its truth at $n$ implies its truth at $\sigma(n)$ for every natural $n$ ([math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)).

## Proof

**Given:** The set $S$ of opposite-parity integer pairs, the quarter-turn $R$, and the cutoff sets $S_t$.

**Goal:** Prove the orbit size, unique representatives and closure in $S_t$, then establish the parametrization, distinct positive labels, full intervals and square-sum identity.

1.1 If $z=2k$ then $-z=2(-k)$, and if $z=2k+1$ then $-z=2(-k-1)+1$, so negation preserves parity. Thus $R$ sends $S$ into $S$, and its graph exists by Separation in $S\times S$ using the displayed rule. For $p=(x,y)$, the first four pairs in the iteration are $(x,y),(-y,x),(-x,-y),(y,-x)$, and one more application returns to $(x,y)$. Let $C$ be the set of these four listed values, which is closed under $R$. Apply [F7] with $A=S$, $a=p$ and $f=R$ to obtain the sequence $g_p$ from Justification. The base value $g_p(0)=p$ lies in $C$. If $g_p(n)\in C$, then $g_p(\sigma(n))=R(g_p(n))\in C$ by that closure. Induction gives $g_p(n)\in C$ for all natural $n$. Conversely, each listed pair is reached in zero, one, two or three applications, so each belongs to $O(p)$. Hence $O(p)=C$. Starting at any member of $C$, the same cycle visits each listed value within three applications and stays in $C$, so the orbit from that member is also $C$. Consequently two orbits sharing a pair coincide. Also $(-y)^2+x^2=Q(x,y)$, so the square sum is constant throughout the orbit. If $p\in S_t$, this equality puts every member of its orbit in $S_t$. [F1, F2, F3, F4, F5, F6, F7, F8]

1.2 By the formulas for $\iota$, natural $0$ and $1$ map to integer $0$ and $1$. Natural $0<1$ because $0\in1$. Order preservation and injectivity give integer $0<1$, and adding $1$ gives $1<2$, so $0<2$. Given a positive integer $d$, write $d=\iota(n)$ for a natural $n$. Since $\iota(0)=0$, we have $n\ne0$. Thus $0\in n$, so every element of natural $1=\{0\}$ belongs to $n$. It follows that $1\le n$ in the natural order, and order preservation gives $1\le d$ in the integer order. Also, if $a<b$, then $2(b-a)>0$, so $2a<2b$. Finally, every integer square is nonnegative. It is zero when the integer is zero, and otherwise the integer or its negative is positive, has positive square, and has the same square as the original integer. [F1, F5]

2.1 An opposite-parity pair cannot have both coordinates zero because $0$ is even. If both coordinates are nonzero, exactly one of the four sign pairs $(+,+),(+,-),(-,-),(-,+)$ applies to $(x,y)$, where $+$ means positive and $-$ means negative. In those respective cases the first, second, third and fourth listed values in Step 1.1 have both coordinates positive. If $y=0$, the first listed value works for $x>0$ and the third works for $x<0$. If $x=0$, the second works for $y<0$ and the fourth works for $y>0$. Hence the orbit contains some $(a,b)$ with $a>0$, $b\ge0$. Starting the list at $(a,b)$, if $b>0$ the four values have different sign pairs, and only $(a,b)$ has positive first and nonnegative second entry. If $b=0$, the values are $(a,0),(0,a),(-a,0),(0,-a)$, distinct since $a>0$, and again only $(a,0)$ meets the required sign condition. [F1, F2, F3, step 1.1]

3.1 Assign natural $0,1,2,3$ to the four successive pairs starting at the representative. Separate in $4\times O(p)$ the graph described by these four assignments. This gives a function from natural $4$ to $O(p)$ because the list assigns exactly one value to each input. The list contains every member and its values are distinct, so this function is a bijection. Thus every orbit has cardinality four. [F2, F5, F6, step 1.1, step 2.1]

3.2 For the representative $(x,y)$ the sum $x+y$ is odd because adding an even integer and an odd integer has the form $2k+1$. The same applies to $x-y$ by parity preservation under negation. Write these odd integers as $2u+1$ and $2v+1$, respectively. Strict increase of multiplication by $2$ gives unique $u,v$. Adding and subtracting the equations and using the same injectivity gives $x=u+v+1$ and $y=u-v$. As $x+y\ge1$, the equation $x+y=2u+1$ gives $u\ge0$. The inequalities $y\ge0$ and $x\ge1$ give $v\le u$ and $v\ge-u$, respectively. [F1, F3, step 1.1, step 2.1, step 1.2]

4.1 Conversely, for any integers $u\ge0$ and $-u\le v\le u$, define $x=u+v+1$ and $y=u-v$. Then $x\ge1$ and $y\ge0$, and $x+y=2u+1$, $x-y=2v+1$. Two even integers sum to an even integer, and two odd integers $2a+1,2b+1$ sum to $2(a+b+1)$, which is even. The odd sum therefore forces opposite parity. This pair lies in $S$ and meets the condition for being its orbit's representative. [F1, F3, step 2.1, step 1.2, step 3.2]

4.2 Substituting $x=u+v+1$ and $y=u-v$ and expanding gives $x^2+y^2+1=2u^2+2v^2+2u+2v+2=2(L+v^2)$. The exact quotient by $2$ is $L+v^2$, which is at least $L$ by nonnegativity of $v^2$. [F1, step 1.2, step 3.2]

5.1 For fixed $u$, adding $u^2+u+1$ to $-u\le v\le u$ gives $u^2+1\le L\le u^2+2u+1=(u+1)^2$. In particular $L\ge1$. Conversely, an integer $\ell$ in that interval gives $v=\ell-(u^2+u+1)$ with $-u\le v\le u$, and Step 4.1 supplies a representative with label $\ell$. Within this interval, equality of labels for representatives with the same $u$ forces equality of $v$, hence equality of both coordinates. [F1, F2, step 1.2, step 3.2, step 4.1]

6.1 If $0\le u<u'$, then $u'-u$ is a positive integer, so $u'\ge u+1$. Thus $u'^2-(u+1)^2=(u'-u-1)(u'+u+1)\ge0$, since both factors are nonnegative. The interval for $u'$ begins at $u'^2+1>(u+1)^2$, beyond the interval for $u$. Different values of $u$ therefore give disjoint label intervals, and Step 5.1 handles equality of labels at the same $u$. [F1, step 1.2, step 5.1]

7.1 Every orbit has four members, a unique representative and constant square sum, so an orbit meeting $S_t$ lies in $S_t$. The representatives give the required integer parameters and distinct positive labels, with the stated intervals and square-sum identity. [step 1.1, step 2.1, step 3.1, step 3.2, step 5.1, step 6.1, step 4.2] ∎

---
title: "Lemma 4.1: A bound for mixed lattice pairs"
status: draft
research_item: lem-euler-mixed-lattice-count
dependency_level: 3
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, Lemma 4.1, statement and last two lines
---

PDF p. 4: ` Lemma 4.1, statement and last two lines `

## Prerequisites

- [def-euler-mixed-lattice-count](item-def-euler-mixed-lattice-count)
- [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [lem-euler-mixed-lattice-orbit-labels](item-lem-euler-mixed-lattice-orbit-labels)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)
- [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)


## Statement

For a real number $t\ge 0$, let $S_t$ consist of the signed, ordered integer pairs $(x,y)$ with opposite parity and $x^2+y^2\le t$. The entries retain their signs and their order. Opposite parity means that one entry is even, of the form $2a$, and the other is odd, of the form $2b+1$, for integers $a,b$. Write $z^2=z\cdot z$. Each integer is read as its canonical real value in the comparison with $t$.

Let $N_{\mathrm{mix}}(t)=\#S_t$, the number of elements of this finite set. For a real number $s$, write $\lfloor s\rfloor$ for the unique integer $m$ satisfying $m\le s<m+1$. With the count and the integer part read as real numbers in the inequalities, one has
$$N_{\mathrm{mix}}(t)\le 4\left\lfloor\frac{t+1}{2}\right\rfloor\le 2(t+1).$$

## Statement references

[def-euler-mixed-lattice-count](item-def-euler-mixed-lattice-count)

[math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)

[math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

## Facts & Assumptions

[F1] For every real $t\ge 0$, the set $S_t$ defined in the Statement is finite and its cardinality $N_{\mathrm{mix}}(t)$ is the number of its elements. [def-euler-mixed-lattice-count](item-def-euler-mixed-lattice-count) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F2] The quarter-turn is $R(x,y)=(-y,x)$. The orbit of a pair is the set obtained by iterating $R$ from that pair, including the starting pair. For a pair in $S_t$ the orbit has four members, all in $S_t$, and its unique representative is the member $r=(x,y)$ with $x>0$ and $y\ge 0$. Starting at $r$, the four successive values $R^j(r)$ for $j=0,1,2,3$ exhaust the orbit, where $R^j$ means $j$ applications and $R^0(r)=r$. Write $x+y=2u+1$ and $x-y=2v+1$ using the unique integers $u,v$ supplied for $r$. Its label $L(r)=u^2+u+v+1$ is an integer with $1\le L(r)\le (x^2+y^2+1)/2$, and different representatives have different labels. [lem-euler-mixed-lattice-orbit-labels](item-lem-euler-mixed-lattice-orbit-labels)

[F3] The integer part $m=\lfloor s\rfloor$ exists for every real $s$ and satisfies $m\le s<m+1$ in the real order. [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)

[F4] The real order is total, and adding a fixed real or multiplying by a positive real preserves order. A quotient by a nonzero real is multiplication by its reciprocal. For an integer $k$, the rational $k/1$ is the class $[(k,1)]$ in $\mathbb Q$. The inclusion of the integers into the reals sends $k$ to the real represented by the constant rational sequence of value $k/1$ and preserves and reflects order. It preserves arithmetic, so integer addition, multiplication, and subtraction can also be computed with the real values. It is injective and sends integer $0$ and integer $1$ to real $0$ and real $1$, respectively. [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[F5] An integer $k$ is positive when $0<k$ in the integer order. In both the integer and natural orders, strict comparison means non-strict comparison with unequal entries. The natural numbers include $0$. The successor $\sigma(n)$ of $n$ is $n\cup\{n\}$. The first four successors starting at $0$ are $1,2,3,4$, with $1=\{0\}$ and $4=\{0,1,2,3\}$ as sets of naturals. A natural $j$ satisfies $j<n$ exactly when $j\in n$. For natural $k,j$, addition satisfies $k+0=k$ and $k+\sigma(j)=\sigma(k+j)$. The map $n\mapsto [(n,0)]$ identifies the naturals with the nonnegative integers. This map is one-to-one and preserves addition and multiplication. An inequality between naturals holds exactly when it holds between their images. Its values at natural $0,1$ are integer $0,1$, respectively. [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-int-order](https://alphabetamath.cc/item/def-int-order) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)

[F6] The initial segment $I_n=\{i\in\mathbb N:i<n\}$ is the set of naturals strictly below the natural number $n$. It is finite and has cardinality $n$. The Cartesian product $A\times B$ consists of pairs $(a,b)$ with $a\in A$ and $b\in B$, and two such pairs are equal exactly when their corresponding entries are equal. If $A$ and $B$ are finite, the number of elements of $A\times B$ is the product in $\mathbb N$ of the two numbers of elements. [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment) [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product) [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs) [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication) [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)

[F7] Separation forms the subset of a given set whose elements meet a specified condition. A function from $A$ to $B$ assigns exactly one element of $B$ to every element of $A$. It is an injection if equal outputs imply equal inputs and a bijection if, in addition, each element of $B$ occurs as an output. A bijection transports finite cardinality, and any subset of a finite set is finite with cardinality at most that of the full set. Bounded set-builder notation denotes the subset selected by the stated condition. [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation) [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) [math:def-function](https://alphabetamath.cc/item/def-function) [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)

## Proof

**Given:** A real number $t\ge 0$ and the finite set $S_t$ of signed, ordered opposite-parity pairs with square sum at most $t$.

**Goal:** Show that $N_{\mathrm{mix}}(t)\le 4\lfloor(t+1)/2\rfloor\le 2(t+1)$.

1.1 By [F5], no positive integer lies below $1$. Such an integer would correspond to a natural strictly between $0$ and $1$, but the only natural in $1$ is $0$. Put $s=(t+1)/2$ and $m=\lfloor s\rfloor$. Since natural $0$ belongs to natural $1$, [F5] gives $0<1$ in the natural order. The embeddings in [F5] and [F4] give $0<1$ in the real order, so one has $2>0$ and $t+1>0$. The reciprocal of $2$ is positive, since a negative reciprocal would make its product with $2$ negative and a zero reciprocal would make the product zero, whereas the product is $1$. Thus $s\ge 0$. If $m<0$, then $-m$ is a positive integer, so $-m\ge 1$ and $m+1\le 0$. This contradicts $s<m+1$. Hence $m\ge 0$. Let $n$ be the unique natural number whose image in the integers is $m$. [given, F3, F4, F5]

1.2 For natural $k$, $k+1=k+\sigma(0)=\sigma(k+0)=\sigma(k)$ by the recursion for addition. The composite embedding $\eta:\mathbb N\to\mathbb Z\to\mathbb Q\to\mathbb R$ sends natural $1$ to real $1$ and preserves addition, so $\eta(\sigma(k))=\eta(k)+1$. Starting with $1$, this gives $\eta(2)=1+1$ and $\eta(4)=((1+1)+1)+1=2+2$, the real $4$. [F4, F5]

2.1 For $p\in S_t$, take its representative $r=(x,y)$ from [F2]. Since $r\in S_t$, one has $x^2+y^2\le t$. Adding $1$ and multiplying by the positive reciprocal of $2$ gives $L(r)\le (x^2+y^2+1)/2\le s$. If $L(r)>m$, the positive integer $L(r)-m$ is at least $1$ by Step 1.1. This would give $m+1\le L(r)\le s<m+1$. Consequently $1\le L(r)\le m$. [F1, F2, F3, F4, F5, step 1.1]

3.1 Let $P=I_n\times I_4$. This set is finite and its natural-number cardinality is $\#P=n\cdot4$ by the initial-segment count and the product rule. For $p\in S_t$, the integer $L(r)-1$ satisfies $0\le L(r)-1\le m-1<m$. Its unique natural preimage $a$ satisfies $a<n$ because the natural embedding preserves and reflects order and sends $n$ to $m$. Thus $a\in I_n$. Exactly one $j\in I_4=\{0,1,2,3\}$ satisfies $p=R^j(r)$ because the four listed values are distinct and exhaust the orbit. Thus $p$ is assigned exactly one pair $f(p)=(a,j)\in P$. Separating the pairs in $S_t\times P$ whose second entry is the assigned value gives the graph of the function $f:S_t\to P$. [F2, F4, F5, F6, F7, step 1.1, step 2.1]

4.1 If two inputs give the same $f(p)$, their first entries agree. Their integer images $L(r)-1$ then agree, so their labels agree after adding $1$. The representatives then agree by [F2]. The second entries also agree, so both inputs are obtained from that same representative by the same number of quarter-turns. The inputs coincide, proving that $f$ is an injection. [F2, F4, F5, F6, F7, step 3.1]

5.1 The set $C=\{q\in P:q=f(p)\text{ for some }p\in S_t\}$ exists by Separation. Its defining condition gives $C\subseteq P$ since every $q\in C$ belongs to $P$. The function $f$ gives a bijection from $S_t$ to $C$ since each element of $C$ is the value of at least one input and Step 4.1 proves it is the value of only one. Therefore $N_{\mathrm{mix}}(t)=\#C\le\#P=n\cdot4$ in the natural-number order. [F1, F7, step 3.1, step 4.1]

6.1 Applying $\eta$ to the inequality of Step 5.1 preserves its order, and $\eta(n\cdot4)=\eta(n)\eta(4)$ by preservation of multiplication. Here $\eta(n)$ is the real image of $m$ by Step 1.1, and $\eta(4)=4$ by Step 1.2. Thus $N_{\mathrm{mix}}(t)\le4m$ when the count and $m$ are read as real numbers. [F4, F5, F6, step 1.1, step 1.2, step 5.1]

7.1 The real $4=2+2$ is positive by $2>0$. Multiplying $m\le s$ by $4$ gives $4m\le 4s=2(t+1)$. Together with Step 6.1 and $m=\lfloor(t+1)/2\rfloor$, this gives both claimed inequalities. [F3, F4, step 1.1, step 1.2, step 6.1] ∎

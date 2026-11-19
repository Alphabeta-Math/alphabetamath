---
title: Square residues and opposite parity
status: draft
research_item: lem-square-residue-parity
dependency_level: 0
---

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)


## Statement

Write $\mathbb Z$ for the integers and $z^2$ for $z\cdot z$. An integer $z$ is **even** if $z=2k$ for some integer $k$ and **odd** if $z=2k+1$ for some integer $k$. Two integers have **opposite parity** if one is even and the other is odd, and the **same parity** if both are even or both are odd.

An integer $d$ divides an integer $z$ if $z=dq$ for some integer $q$. It is a common divisor of $x$ and $y$ if it divides each. An integer $z$ is positive if $0<z$. Congruence $a\equiv b\pmod m$ means that $m$ divides $a-b$.

Every integer is either even or odd, and the two cases are mutually exclusive. For every integer $z$, one has $z^2\equiv0\pmod4$ if $z$ is even and $z^2\equiv1\pmod4$ if $z$ is odd. If $x$ and $y$ have opposite parity, then $x^2+y^2$ is positive, odd, and congruent to $1$ modulo $4$. If a positive odd integer $d$ divides both $x$ and $y$, each of $x$ and $y$ has the same parity as its exact integer quotient by $d$.

## Statement references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

## Justification

Division with remainder by $2$ makes the even and odd conditions exhaustive and disjoint, as Steps 1.1 and 2.1 show. The same-parity and opposite-parity conditions therefore specify whether the two unique remainders are equal or different. For a positive divisor, the exact integer quotient is the unique quotient with remainder zero.

## Facts & Assumptions

[F1] In the integer construction, $[(a,b)]$ denotes the class of the natural-number pair $(a,b)$, with $(a,b)$ and $(c,d)$ in the same class when $a+d=b+c$ ([math:def-integers](https://alphabetamath.cc/item/def-integers)). Integer arithmetic uses the defined addition and multiplication with $0=[(0,0)]$ and $1=[(1,0)]$ ([math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)). Use the numerals $2=1+1$ and $4=2\cdot2$. The strict integer order is $a<b$ when $a\le b$ and $a\ne b$ ([math:def-int-order](https://alphabetamath.cc/item/def-int-order)).

[F2] Integer addition and multiplication satisfy the commutative ring laws, including distributivity and the additive and multiplicative identity laws. The order is total, addition preserves inequalities, and the product of positive integers is positive ([math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)).

[F3] An integer multiple $z=dq$ is equivalent to $d$ dividing $z$ ([math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)). An equality $a-b=mq$ with integer $q$ is equivalent to $a\equiv b\pmod m$ ([math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)).

[F4] For any integer $z$ and positive integer $b$, there exist unique integers $q,r$ with $z=bq+r$ and $0\le r<b$ ([math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

[F5] The map $\iota(n)=[(n,0)]$ from the natural numbers to the integers is injective and additive. It preserves and reflects the non-strict order, using the additive order on its domain ([math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)). Its image consists of the nonnegative integers ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)).

[F6] The natural numbers $0,1,2$ are respectively $\varnothing,\{0\},\{0,1\}$, with successor $\sigma(n)=n\cup\{n\}$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)). For natural numbers $m,n$, the additive order $m\le n$ means $m+k=n$ for some natural number $k$, and $m<n$ means $m\le n$ and $m\ne n$ ([math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)). For natural numbers $m,n$, one has $m<n$ exactly when $m\in n$ ([math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)).

[F7] Natural number addition has the rules $m+0=m$ and $m+\sigma(n)=\sigma(m+n)$ ([math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)).

## Proof

**Given:** Arbitrary integers $z,x,y$. For the square sum assume $x$ and $y$ have opposite parity. For the division claim assume $d$ is a positive odd integer dividing both $x$ and $y$.

**Goal:** Show that every integer has exactly one parity, determine the square of $z$ modulo $4$ from its parity, establish the three properties of the opposite-parity square sum, and show that the exact quotients by $d$ retain the original parities.

1.1 In the natural numbers $1+1=\sigma(1+0)=\sigma(1)=2$. The map $\iota$ sends natural $0,1$ to integer $0,1$ by the formulas in F1 and F5, and sends natural $2=1+1$ to integer $2=1+1$ by additivity. By injectivity and preservation and reflection of $\le$, the map $\iota$ preserves and reflects $<$ as defined in F1 and F6. The natural inequalities $0<1<2$ follow from $0\in1$ and $1\in2$, so they hold for the integer numerals as well. If $r$ is an integer with $0\le r<2$, write $r=\iota(n)$ for a natural number $n$. Then $n<2$, hence $n\in\{0,1\}$, and thus $r=0$ or $r=1$. [F1, F5, F6, F7]

2.1 Apply division with remainder by $2$ to an arbitrary integer $z$. Step 1.1 gives the two possible remainders $0$ and $1$, and both are in the permitted range. The representation $z=2q+r$ therefore identifies $z$ as even when $r=0$ and odd when $r=1$. The two forms are mutually exclusive by uniqueness of the remainder. In particular $0$ is even because $0=2\cdot0$. [F2, F4, step 1.1]

3.1 If $z=2q$, then $z^2=4q^2$, so $z^2\equiv0\pmod4$. If $z=2q+1$, then $z^2=4(q^2+q)+1$, so $z^2\equiv1\pmod4$. The displayed multiples of $4$ give the required divisibility witnesses for the two congruences. [F1, F2, F3, step 2.1]

3.2 If an integer $w$ is zero, then $w^2=0$. Otherwise totality and addition of $-w$ to the inequality $w<0$ when needed give that either $w$ or $-w$ is positive. The square of that positive integer is positive and equals $w^2$ because $(-w)^2=w^2$. Thus both squares in $x^2+y^2$ are nonnegative, and the odd coordinate has positive square because zero is even. Adding the nonnegative square to the positive square leaves a positive sum by compatibility of order with addition. [F1, F2, step 2.1]

3.3 Write $d=2a+1$ and let $w=2b+r$ be any integer with its remainder $r$ from Step 2.1. Then $dw=(2a+1)(2b+r)=2((2a+1)b+ar)+r$. Since $0\le r<2$, uniqueness of the remainder in division by $2$ gives the same remainder for $dw$ and $w$. Thus multiplication by $d$ preserves the parity of every integer. [F2, F4, step 2.1]

4.1 For $x,y$ of opposite parity, Step 3.1 writes the even coordinate's square as $4A$ and the odd coordinate's square as $4B+1$ for integers $A,B$. Their sum is $4(A+B)+1=2(2(A+B))+1$. The first expression shows congruence to $1$ modulo $4$, and the second shows oddness. [F1, F2, F3, step 3.1]

4.2 Because $d$ divides $x$ and $y$, there are integers $u,v$ with $x=du$ and $y=dv$. Since $d>0$, these are the unique quotients with remainder zero in division by $d$. Applying Step 3.3 to $u$ and to $v$ proves that $x$ has the parity of $u$ and $y$ has the parity of $v$. [F3, F4, step 3.3]

5.1 Each integer has exactly one parity. The square congruences, the positivity, oddness and congruence of the opposite-parity square sum, and the parity of each exact quotient follow from the preceding steps. [step 2.1, step 3.1, step 4.1, step 3.2, step 4.2] ∎

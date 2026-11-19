---
title: A floor difference detects divisibility
status: draft
research_item: lem-floor-increment-divisibility
dependency_level: 0
---

## Prerequisites

- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:cor-of-one-positive](https://alphabetamath.cc/item/cor-of-one-positive)
- [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:thm-int-comm-ring](https://alphabetamath.cc/item/thm-int-comm-ring)


## Statement

Let $b,p\in\mathbb{Z}$ with $p>0$, where $\mathbb{Z}$ denotes the integers. When taking real quotients or floors, identify the integers with their image in $\mathbb{R}$, the real numbers, under the canonical embedding through the rationals. For real $a$, the quotient $a/p$ is the unique real $u$ satisfying $up=a$. For a real number $x$, its floor $\lfloor x\rfloor$ is the unique integer $m$ with $m\le x<m+1$. The notation $p\mid b$ means that $b=pt$ for some integer $t$.

Then $\lfloor b/p\rfloor-\lfloor(b-1)/p\rfloor$ is $1$ if $p\mid b$ and $0$ otherwise.

## Statement references

[The integers](https://alphabetamath.cc/item/def-integers)

[The real numbers](https://alphabetamath.cc/item/def-real-numbers)

[The rationals](https://alphabetamath.cc/item/def-rationals)

[Division in a field](https://alphabetamath.cc/item/def-field)

[The floor of a real number](https://alphabetamath.cc/item/lem-integer-part)

[Divisibility of integers](https://alphabetamath.cc/item/def-divides-in-z)

[Integer arithmetic](https://alphabetamath.cc/item/def-int-operations)

[Integer order](https://alphabetamath.cc/item/def-int-order)

[Real order](https://alphabetamath.cc/item/def-real-order)

[Ordered field](https://alphabetamath.cc/item/def-ordered-field)

[The integers in the rationals](https://alphabetamath.cc/item/lem-int-embeds-rat)

[The rationals in the reals](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[The real ordered field](https://alphabetamath.cc/item/thm-reals-ordered-field)

## Facts & Assumptions

[F1] The canonical map $e:\mathbb{Z}\to\mathbb{R}$ first sends an integer $k$ to the rational class $[(k,1)]$ ([The rationals](https://alphabetamath.cc/item/def-rationals)) and then to the real class of the corresponding constant sequence. Both embeddings are injective and preserve addition, multiplication and order ([The integers in the rationals](https://alphabetamath.cc/item/lem-int-embeds-rat), [The rationals in the reals](https://alphabetamath.cc/item/lem-rat-embeds-dense)). For every real $x$, the unique integer $m$ satisfying $m\le x<m+1$ in this identification is $\lfloor x\rfloor$ ([Integer part](https://alphabetamath.cc/item/lem-integer-part)).

[F2] For integers $b,p$ with $p>0$ in the integer order ([Integer order](https://alphabetamath.cc/item/def-int-order)), there are unique integers $q,r$ with $b=qp+r$ and $0\le r<p$. The integer $r$ is called the remainder, and $r=0$ exactly when $p\mid b$ ([Division with remainder](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

[F3] For reals $x,y$ with $y\ne0$, the quotient $x/y$ is $xy^{-1}$, where $y^{-1}$ is the unique real number with $yy^{-1}=1$. The field laws include associative and commutative addition and multiplication, additive inverses, and distributivity of multiplication over addition ([Field](https://alphabetamath.cc/item/def-field)).

[F4] The real order makes the reals a totally ordered field ([Real order](https://alphabetamath.cc/item/def-real-order), [Ordered field](https://alphabetamath.cc/item/def-ordered-field), [The real ordered field](https://alphabetamath.cc/item/thm-reals-ordered-field)). In particular, the order is transitive, any two reals are comparable, and adding the same real to both sides preserves strict and weak inequalities. Its multiplicative identity satisfies $0<1$ ([Positivity of one](https://alphabetamath.cc/item/cor-of-one-positive)).

[F5] In an ordered field, multiplication by a positive element $c$ preserves and reflects strict inequalities, so $x<y$ holds exactly when $xc<yc$ ([Order under multiplication](https://alphabetamath.cc/item/lem-of-sign-rules)). The same equivalence holds for weak inequalities because $x\le y$ in a total order exactly when $y<x$ fails ([Ordered field](https://alphabetamath.cc/item/def-ordered-field)).

[F6] In the integers, $0$ and $1$ are the additive and multiplicative identities, and addition, negation and multiplication take integer values. Integer subtraction is addition of the additive inverse ([Integer arithmetic](https://alphabetamath.cc/item/def-int-operations), [The integer ring](https://alphabetamath.cc/item/thm-int-comm-ring)).

## Proof

**Given:** Integers $b,p$ with $p>0$.

**Goal:** Show that the floor difference is $1$ when $p\mid b$ and is $0$ otherwise.

1.1 Since $e$ preserves addition, $e(0)=e(0)+e(0)$, so real additive cancellation gives $e(0)=0$. Order preservation and $p>0$ give $e(p)>0$. Since $p\cdot1=p$ and $e$ preserves multiplication, $e(p)e(1)=e(p)$, so cancellation by the nonzero real $e(p)$ gives $e(1)=1$. Also $e(s)+e(-s)=e(0)=0$ for every integer $s$, so negation and subtraction agree under the identification. From here on, write each integer for its real image when taking real quotients or comparing with reals. [given, F1, F3, F4, F6]

2.1 For integers $a,k$, the inequalities $k\le a/p<k+1$ are equivalent to $kp\le a<(k+1)p$. Indeed $p$ is positive in the reals, so multiplication by $p$ preserves and reflects both comparisons, and $(a/p)p=a$. Thus $kp\le a<(k+1)p$ implies $\lfloor a/p\rfloor=k$. [given, F1, F3, F5, F6, step 1.1]

2.2 Every positive integer $s$ satisfies $1\le s$. Since $0<1$, adding $s$ gives $s<s+1$. If $0<s<1$, both $0\le s<0+1$ and $s\le s<s+1$ would hold, so the uniqueness of the floor of $s$ would give $s=0$. Total order now gives $1\le s$. [F1, F3, F4, F6, step 1.1]

3.1 Choose integers $q,r$ with $b=qp+r$ and $0\le r<p$. Adding $qp$ to the bounds on $r$ gives $qp\le b<qp+p=(q+1)p$, so $\lfloor b/p\rfloor=q$. [given, F2, F3, F4, F6, step 1.1, step 2.1]

4.1 If $r=0$, then $b=qp$. Since $1\le p$, we obtain $(q-1)p=b-p\le b-1<b=qp$. Applying step 2.1 with $a=b-1$ and $k=q-1$ gives $\lfloor(b-1)/p\rfloor=q-1$. [given, F3, F4, F6, step 1.1, step 2.1, step 2.2, step 3.1]

4.2 If $r>0$, then $1\le r$, so $0\le r-1$ and $qp\le b-1=qp+(r-1)<b<(q+1)p$. Applying step 2.1 with $a=b-1$ and $k=q$ gives $\lfloor(b-1)/p\rfloor=q$. [F3, F4, F6, step 1.1, step 2.1, step 2.2, step 3.1]

5.1 The two cases exhaust $r\ge0$. The difference is $q-(q-1)=1$ when $r=0$ and $q-q=0$ when $r>0$. As $r=0$ holds exactly when $p\mid b$, this is the claimed floor difference. [F2, F4, F6, step 1.1, step 3.1, step 4.1, step 4.2] ∎

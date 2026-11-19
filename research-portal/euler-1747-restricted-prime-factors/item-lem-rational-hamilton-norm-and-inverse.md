---
title: Norm and conjugation on rational Hamilton quaternions
status: published
research_item: lem-rational-hamilton-norm-and-inverse
dependency_level: 0
---

## Prerequisites

- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)
- [math:thm-rat-field](https://alphabetamath.cc/item/thm-rat-field)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-quaternions](https://alphabetamath.cc/item/def-quaternions)
- [math:def-ring](https://alphabetamath.cc/item/def-ring)
- [math:def-subring](https://alphabetamath.cc/item/def-subring)
- [math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)
- [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)
- [math:def-division-ring](https://alphabetamath.cc/item/def-division-ring)
- [math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring)
- [math:lem-quaternion-conjugation-is-an-anti-involution](https://alphabetamath.cc/item/lem-quaternion-conjugation-is-an-anti-involution)


## Statement

Let $\mathbb H=\mathbb R^4$ be the real Hamilton quaternions with their usual addition and multiplication. Let $B=\mathbb Q^4\subseteq\mathbb H$ be the quaternions with rational coordinates, using the constant-sequence embedding of $\mathbb Q$ into $\mathbb R$. Write $\iota(t)=(t,0,0,0)$ for a scalar quaternion with $t\in\mathbb Q$.

The inherited operations make $B$ a $\mathbb Q$-subalgebra of $\mathbb H$. Thus $B$ is a subring containing $1$ and all the rational scalar quaternions, which commute with every element of $\mathbb H$. Moreover, $B$ is a division algebra over $\mathbb Q$, meaning that $1\ne0$ and every nonzero element of $B$ has a two-sided multiplicative inverse in $B$.

For $x=(a,b,c,d)\in B$, its conjugate is $\bar x=(a,-b,-c,-d)$ and its reduced norm is the rational scalar $N(x)=a^2+b^2+c^2+d^2$, characterized by $x\bar x=\bar x x=\iota(N(x))$. Conjugation on $B$ is an anti-involution. It preserves addition and $1$, applying it twice gives the identity, and $\overline{xy}=\bar y\bar x$.

For all $x,y\in B$, $N(xy)=N(x)N(y)$. For $x\ne0$, $N(x)\ne0$ and $x^{-1}=\bar x/N(x)$, where division by $N(x)$ means multiplication by $\iota(1/N(x))$.

## Facts & Assumptions

[F1] The rational numbers are the classes $a/b$ of integer pairs with $b\ne0$ under equality of cross-products ([math:def-rationals](https://alphabetamath.cc/item/def-rationals)). Their addition, multiplication, negation and reciprocals are those of [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations). They form a field, so sums, products and negatives are rational, and every nonzero rational has a rational reciprocal ([math:thm-rat-field](https://alphabetamath.cc/item/thm-rat-field)). The map taking a rational to the class of its constant sequence in the reals is an injective map preserving $0,1,+,\cdot$ ([math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers), [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)).

[F2] In $\mathbb H$, addition and negation are coordinatewise, and each product coordinate is a sum or difference of products of input coordinates. The elements $0$ and $1$ are $(0,0,0,0)$ and $(1,0,0,0)$. Conjugation negates exactly the last three coordinates, and the real Hamilton norm $N_{\mathbb H}(x)$ is the sum of the four coordinate squares ([math:def-quaternions](https://alphabetamath.cc/item/def-quaternions)).

[F3] The real quaternion operations make $\mathbb H$ a ring with $1\ne0$. For $x\in\mathbb H$, $x\bar x=\bar x x=(N_{\mathbb H}(x),0,0,0)$, and $N_{\mathbb H}(x)>0$ if $x\ne0$ ([math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring)).

[F4] Real quaternion conjugation satisfies $\overline{\bar x}=x$ and $\overline{xy}=\bar y\bar x$ for all $x,y\in\mathbb H$ ([math:lem-quaternion-conjugation-is-an-anti-involution](https://alphabetamath.cc/item/lem-quaternion-conjugation-is-an-anti-involution)).

[F5] A ring is an abelian group under addition with an associative unital multiplication satisfying both distributive laws ([math:def-ring](https://alphabetamath.cc/item/def-ring)). A unital ring map preserves addition, multiplication and $1$ ([math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)). A $\mathbb Q$-algebra is a unital ring with such a map from $\mathbb Q$ whose images commute with all ring elements ([math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)). Its underlying ring is a division ring if $1\ne0$ and every nonzero element has a two-sided multiplicative inverse ([math:def-division-ring](https://alphabetamath.cc/item/def-division-ring)).

[F6] A subset of a ring is a unital subring if it contains the ambient identity and is closed under addition, additive inverses and multiplication. It inherits the ring operations and identities ([math:def-subring](https://alphabetamath.cc/item/def-subring)).

## Proof

**Given:** The real Hamilton quaternions $\mathbb H$, their rational-coordinate subset $B$ and arbitrary $x,y\in B$.

**Goal:** Show that $B$ is a division subalgebra over $\mathbb Q$ with the stated conjugation, reduced norm and inverse formulas.

1.1 The coordinate rules for addition, negation and multiplication keep their results in $\mathbb Q$ by [F1] and [F2]. The coordinates of both $0$ and $1$ are rational. The real quaternions form a ring by [F3]. By [F6], $B$ is a unital subring with the inherited ring operations and identities. [F1, F2, F3, F6]

2.1 For $t\in\mathbb Q$ and $z=(z_0,z_1,z_2,z_3)\in\mathbb H$, substitution into the quaternion product gives $\iota(t)z=z\iota(t)=(tz_0,tz_1,tz_2,tz_3)$. For rational $s,t$, this gives $\iota(s)\iota(t)=\iota(st)$, while coordinate addition gives $\iota(s)+\iota(t)=\iota(s+t)$ and $\iota(1)=1$. The map $\iota$ is injective by the first coordinate and [F1]. Its image lies in $B$ and commutes with every element of $\mathbb H$. Thus $B$ is a $\mathbb Q$-subalgebra with the inherited scalar map. [F1, F2, F5, step 1.1]

2.2 The coordinate formula for conjugation preserves rational coordinates, fixes $1$, and preserves addition because each coordinate is either unchanged or negated. The two identities in [F4] therefore restrict to $B$, proving that its conjugation is an anti-involution. [F1, F2, F4, step 1.1]

3.1 The sum of the four squares of the coordinates of $x$ is rational by [F1], so $N_{\mathbb H}(x)$ is the image of the scalar $N(x)\in\mathbb Q$. The product identity in [F3] yields $x\bar x=\bar x x=\iota(N(x))$. Injectivity of $\iota$ makes this scalar unique. If $x\ne0$, positivity of $N_{\mathbb H}(x)$ gives $N(x)\ne0$. [F1, F2, F3, step 2.1, step 2.2]

4.1 Since $xy\in B$, apply the norm identity to $xy$ and reverse the order under conjugation. Associativity and commutation with rational scalars give $\iota(N(xy))=(xy)\overline{xy}=x(y\bar y)\bar x=(x\bar x)\iota(N(y))=\iota(N(x)N(y))$. Injectivity gives $N(xy)=N(x)N(y)$. [F3, step 1.1, step 2.1, step 2.2, step 3.1]

5.1 If $x\ne0$, then $r=1/N(x)$ is rational by [F1] and step 3.1. Put $u=\iota(r)\bar x\in B$. Using commutation with rational scalars and both orders of the norm identity, $xu=\iota(r)(x\bar x)=\iota(1)=1$ and $ux=\iota(r)(\bar x x)=\iota(1)=1$. This gives the stated inverse in $B$. Since $1\ne0$ in $B$, its ring is a division ring. Thus $B$ is a division algebra with the stated conjugation, reduced norm and inverse. [F1, F3, F5, step 1.1, step 2.1, step 2.2, step 3.1, step 4.1] ∎

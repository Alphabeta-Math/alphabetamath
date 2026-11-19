---
title: Rational and local values of the Hamilton norm
status: draft
research_item: lem-author-eebeda62e446-hamilton-norm-values
dependency_level: 1
---

## Prerequisites

- [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)
- [def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)
- [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)
- [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)
- [math:thm-lagrange-four-square-theorem](https://alphabetamath.cc/item/thm-lagrange-four-square-theorem)
- [math:cor-p-adic-simple-root-lifting](https://alphabetamath.cc/item/cor-p-adic-simple-root-lifting)
- [math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound)
- [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)


## Statement

Let $B$ be the rational Hamilton algebra and $O$ any order, a subring containing $1$ with a $\mathbb Z$-basis that is a $\mathbb Q$-basis of $B$. At a prime $\ell$, let $\mathbb Q_\ell$ be the $\ell$-adic completion of $\mathbb Q$, let $\mathbb Z_\ell$ be its ring of integers, the ball of radius $1$ about $0$ including its boundary, and put $B_\ell=B\otimes_{\mathbb Q}\mathbb Q_\ell$ and $O_\ell=O\otimes_{\mathbb Z}\mathbb Z_\ell$. The superscript $\times$ denotes the multiplicative group of elements invertible in the specified ring. Use the reduced norm $N$, the sum of the squares of the four Hamilton coordinates. Give $\mathbb Q_\ell^\times$ the metric $d_\ell(a,b)=|a-b|_\ell$ from the $\ell$-adic absolute value.

The rational norm has image $\mathbb Q_{>0}$ on $B^\times$. At every prime $\ell$ the norm sends $B_\ell^\times$ onto $\mathbb Q_\ell^\times$, and $1+\ell^3\mathbb Z_\ell$ is an open neighborhood of $1$ consisting of squares in $\mathbb Q_\ell^\times$. At all but finitely many primes, $N(O_\ell^\times)=\mathbb Z_\ell^\times$.

## Facts & Assumptions

[F1] The Hamilton norm is multiplicative and gives $x^{-1}=\bar x/N(x)$ when $N(x)\ne0$, with conjugation negating the last three Hamilton coordinates. Scalar multiplication by $s$ changes the norm by $s^2$. The local order is the $\mathbb Z_\ell$-span of the order basis ([def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)). The rational matrices converting between the order basis and the Hamilton basis remain inverse over $\mathbb Q_\ell$ ([def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)).

[F2] The completion is a valued field with multiplicative absolute value $|\cdot|_\ell$, with $|\ell|_\ell=\ell^{-1}$ and $|a+b|_\ell\le\max(|a|_\ell,|b|_\ell)$ ([math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)). Its closed unit ball identifies with the ring of compatible residue classes modulo the powers of $\ell$. The canonical embedding sends a compatible residue tuple to the limit of its standard integer lifts ([math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp), Justification of [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)). The local valuation agrees with the rational numerator-minus-denominator valuation, so an integer multiple of $\ell^n$ has absolute value at most $\ell^{-n}$ ([def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)).

[F3] Every nonnegative integer is the sum of four integer squares ([math:thm-lagrange-four-square-theorem](https://alphabetamath.cc/item/thm-lagrange-four-square-theorem)). In $\mathbb Z_\ell$, a root modulo $\ell$ of a polynomial with coefficients in $\mathbb Z_\ell$ lifts to a root in $\mathbb Z_\ell$ if its formal derivative, computed by differentiating the powers of the variable, is nonzero modulo $\ell$ at that root ([math:cor-p-adic-simple-root-lifting](https://alphabetamath.cc/item/cor-p-adic-simple-root-lifting)).

[F4] Every positive divisor of a positive integer $D$ is at most $D$ ([math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound)).

[F5] In the metric $d_\ell$, a subset of $\mathbb Q_\ell^\times$ is open if each of its points has a positive-radius ball in $\mathbb Q_\ell^\times$ contained in the subset. An open neighborhood of $1$ is an open set containing $1$ ([math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)).

## Proof

**Given:** The Hamilton norm, a fixed order $O$, and a prime $\ell$.

**Goal:** Determine the stated rational and local images and exhibit the neighborhood of squares.

1.1 A nonzero rational quaternion has positive norm by the coordinate formula. If $m,n$ are positive integers, choose an integral Hamilton-coordinate quaternion $z$ of norm $mn$ by the four-square theorem. Then $z/n$ has norm $m/n$ and is invertible. This gives the rational image. [F1, F3]

1.2 Let $r\in1+\ell^3\mathbb Z_\ell$. For odd $\ell$, the polynomial $T^2-r$ has root $1$ modulo $\ell$ and derivative $2$ there, which is nonzero modulo $\ell$. For $\ell=2$, use $T^2+T-(r-1)/4$, whose constant term is in $2\mathbb Z_2$. Its root $0$ modulo $2$ has derivative $1$. A lifted root $z$ of this polynomial satisfies $(1+2z)^2=r$. Thus in each case $r$ is a square. By the unit-ball description and multiplicativity in [F2], $1+\ell^3\mathbb Z_\ell$ is the set of $r$ with $|r-1|_\ell\le\ell^{-3}$. It contains $1$, and every such $r$ has $|r|_\ell=1$ by the ultrametric inequality applied to $r=1+(r-1)$ and $1=r-(r-1)$, since $|r-1|_\ell<1$. For each such $r$, if $t\in\mathbb Q_\ell^\times$ satisfies $d_\ell(t,r)<\ell^{-3}$, then $|t-1|_\ell\le\max(|t-r|_\ell,|r-1|_\ell)\le\ell^{-3}$. The pointwise criterion in [F5] therefore gives an open neighborhood of $1$. [F2, F3, F5]

2.1 Given $a\in\mathbb Q_\ell^\times$, take $k\ge0$ with $b=\ell^{2k}a\in\mathbb Z_\ell$. Choose $n\ge1$ so large that $\ell^{-n}\le\ell^{-3}|b|_\ell$. Take a positive integer $m$ representing the residue of $b$ modulo $\ell^n$, using $\ell^n$ for the zero residue. For every $j\ge n$, the standard lift of the residue of $b$ modulo $\ell^j$ differs from $m$ by a multiple of $\ell^n$, so it is at distance at most $\ell^{-n}$ from $m$. These lifts converge to $b$ by [F2], so $|m-b|_\ell\le\ell^{-n}$ by the ultrametric inequality. Since $\ell^{-n}<|b|_\ell$, $|m|_\ell=|b|_\ell$ by applying the ultrametric inequality in both directions. It follows that $b/m\in1+\ell^3\mathbb Z_\ell$. Choose $s\in\mathbb Z_\ell^\times$ with $s^2=b/m$ by step 1.2, where $|s|_\ell=1$ follows from $|s^2|_\ell=1$. An integral Hamilton-coordinate quaternion $z$ of norm $m$ exists by the four-square theorem. The quaternion $\ell^{-k}sz$ has norm $a$ and hence is invertible in $B_\ell$. [F1, F2, F3, step 1.2]

3.1 In the rational change-of-basis matrices between the order basis and the Hamilton basis, clear the denominators of the entries of both matrices by one positive integer $D$. At a prime $\ell$ not dividing $D$, every entry of either matrix has the form $u/D$ with $u\in\mathbb Z$. A nonzero such entry has $v_\ell(u/D)=v_\ell(u)-v_\ell(D)=v_\ell(u)\ge0$ by [F2], and a zero entry is integral as well. The matrix taking order coordinates to Hamilton coordinates therefore sends every column in $\mathbb Z_\ell^4$ to an integral Hamilton coordinate column. Its inverse sends every integral Hamilton coordinate column to an integral order coordinate column. By [F1], the two inclusions show that $O_\ell$ consists of the quaternions with integral Hamilton coordinates. There, if $x\in O_\ell^\times$, both $x$ and its inverse have integral coordinates, and their integral norms multiply to one. Conversely, for $a\in\mathbb Z_\ell^\times$ use $k=0$ in step 2.1. The resulting $x=sz$ and its inverse $\bar x/a$ both have integral coordinates. This gives $N(O_\ell^\times)=\mathbb Z_\ell^\times$ off the prime divisors of $D$. These primes lie in the finite integer interval from $2$ to $D$ by [F4]. [F1, F2, F4, step 2.1] ∎

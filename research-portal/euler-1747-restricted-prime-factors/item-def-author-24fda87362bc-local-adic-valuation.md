---
title: The normalized valuation on the local field
status: draft
research_item: def-author-24fda87362bc-local-adic-valuation
dependency_level: 0
---

## Prerequisites

- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)
- [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)
- [math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes)
- [math:cor-zp-is-the-valuation-ring-of-qp](https://alphabetamath.cc/item/cor-zp-is-the-valuation-ring-of-qp)
- [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals)
- [math:lem-p-adic-valuation-on-q](https://alphabetamath.cc/item/lem-p-adic-valuation-on-q)
- [math:def-p-adic-valuation](https://alphabetamath.cc/item/def-p-adic-valuation)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)
- [math:thm-integers-modulo-n-basic-algebra](https://alphabetamath.cc/item/thm-integers-modulo-n-basic-algebra)
- [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)
- [math:def-valuation-on-a-field](https://alphabetamath.cc/item/def-valuation-on-a-field)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:lem-power-laws](https://alphabetamath.cc/item/lem-power-laws)
- [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:lem-geometric-sequence-null](https://alphabetamath.cc/item/lem-geometric-sequence-null)
- [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)
- [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules)
- [math:def-abs-value](https://alphabetamath.cc/item/def-abs-value)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-metric-convergence](https://alphabetamath.cc/item/def-metric-convergence)
- [math:lem-limit-preserves-order](https://alphabetamath.cc/item/lem-limit-preserves-order)
- [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit)


## Definition

Let $\ell$ be a prime, a positive integer greater than $1$ with no positive divisors other than $1$ and itself. The field $\mathbb Q_\ell$ of $\ell$-adic numbers is the completion of $\mathbb Q$ for the distance $|r-s|_\ell$. Its elements are represented by rational Cauchy sequences, whose terms beyond a sufficiently large index have pairwise distances below any prescribed positive bound. Two such sequences represent the same element if their termwise distances tend to zero.

For a nonzero integer $a$, its exponent $v_\ell(a)$ is the greatest integer $k\ge0$ for which $\ell^k$ divides $a$. For a nonzero rational $r=a/b$ with nonzero integers $a,b$, set $v_\ell(r)=v_\ell(a)-v_\ell(b)$ and $|r|_\ell=\ell^{-v_\ell(r)}$. Set $|0|_\ell=0$. The powers in these absolute value formulas are integer powers of the positive real number $\ell$. On $\mathbb Q_\ell$, $|\cdot|_\ell$ denotes the extension of the rational absolute value, given by $\lim_{j\to\infty}|r_j|_\ell$ on the class of a rational Cauchy sequence $(r_j)$.

The ring $\mathbb Z_\ell$ of $\ell$-adic integers consists of compatible tuples of classes in $\mathbb Z/\ell^n\mathbb Z$ for $n\ge1$. Write $[a]_n$ for the class of $a$ modulo $\ell^n$. The transition maps send $[a]_{n+1}$ to $[a]_n$, and the ring operations are coordinatewise, using $[a]_n+[b]_n=[a+b]_n$ and $[a]_n[b]_n=[ab]_n$. The canonical embedding of this ring into the metric completion $\mathbb Q_\ell$ identifies it with the closed unit ball $\{x\in\mathbb Q_\ell:|x|_\ell\le1\}$.

The normalized valuation on $\mathbb Q_\ell$ is $v_\ell(x)=m$ when $x\ne0$ and $|x|_\ell=\ell^{-m}$ for $m\in\mathbb Z$, and $v_\ell(0)=+\infty$. Here $+\infty$ exceeds every integer and adding it to any value, including itself, gives $+\infty$. The value group is $\mathbb Z$ under addition with the usual order.

## Justification

The prime condition uses [math:def-prime](https://alphabetamath.cc/item/def-prime). The greatest exponent exists by [math:def-p-adic-valuation](https://alphabetamath.cc/item/def-p-adic-valuation). The rational valuation is independent of the fraction by [math:lem-p-adic-valuation-on-q](https://alphabetamath.cc/item/lem-p-adic-valuation-on-q), and [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals) defines the absolute value from it. The field construction in [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers) embeds the rationals isometrically and densely. The extension in [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field) is multiplicative and satisfies $|x+y|_\ell\le\max(|x|_\ell,|y|_\ell)$. For $x\ne0$ take a rational $r$ with $|x-r|_\ell<|x|_\ell$. Applying the inequality to $r=x+(r-x)$ gives $|r|_\ell\le |x|_\ell$. Applying it to $x=r+(x-r)$ then gives $|x|_\ell\le |r|_\ell$ because $|x-r|_\ell<|x|_\ell$. Thus $|r|_\ell=|x|_\ell>0$, so the exponent exists.

The ordered ring of [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) supplies the multiplicative monoid $(\mathbb Z,\cdot,1)$. Powers $\ell^k$ in divisibility and in the residue moduli are its natural powers from [math:def-group-power](https://alphabetamath.cc/item/def-group-power). By [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int), the nonnegative integer exponents are identified with the natural numbers. These powers are positive by the [induction principle](https://alphabetamath.cc/item/thm-induction-principle). The base case is $\ell^0=1>0$, and the ordered-ring multiplication law gives $\ell^{k+1}=\ell^k\ell>0$ if $\ell^k>0$. Thus each modulus $\ell^n$ corresponds to a natural number under the same identification.

Use the ordered field $\mathbb R$ from [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field). The ordered embeddings from [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) and [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) carry the integer inequality $\ell>1$ to the same inequality in $\mathbb R$. Take integer powers in $\mathbb R$ as in [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power). If $m<n$ in $\mathbb Z$, then $n-m>0$ by the ordered-ring law for addition, so [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) identifies $n-m$ with a positive natural exponent. By [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone), $\ell^{n-m}>1$ since $\ell>1$. If $n\le0$, then $\ell^{-n}>0$ by the positivity of natural powers from [math:lem-power-monotone](https://alphabetamath.cc/item/lem-power-monotone). If $n>0$, that same positivity gives $\ell^{n}>0$, so $\ell^{-n}=(\ell^n)^{-1}>0$ by [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive). The exponent addition law of [math:lem-power-laws](https://alphabetamath.cc/item/lem-power-laws) gives $\ell^{-m}=\ell^{-n}\ell^{n-m}$. Since $\ell^{n-m}>1$ and $\ell^{-n}>0$, multiplication by $\ell^{-n}$ preserves strict inequality by [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules), so $\ell^{-m}>\ell^{-n}$. Thus $m\mapsto\ell^{-m}$ is strictly decreasing and the exponent is unique. Isometry and uniqueness also show that the local valuation agrees with the rational formula on nonzero rationals.

The integers form a totally ordered commutative ring by [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring), so their additive group is abelian and its total order is translation invariant. This supplies the ordered value group required by [math:def-valuation-on-a-field](https://alphabetamath.cc/item/def-valuation-on-a-field). By definition $v_\ell(x)=+\infty$ exactly when $x=0$. For nonzero $x$ and $y$, multiplicativity of the extended absolute value gives $|xy|_\ell=\ell^{-v_\ell(x)}\ell^{-v_\ell(y)}=\ell^{-(v_\ell(x)+v_\ell(y))}$ by [math:lem-power-laws](https://alphabetamath.cc/item/lem-power-laws). Uniqueness of the exponent gives $v_\ell(xy)=v_\ell(x)+v_\ell(y)$. If a factor is zero, the product law holds by the rule for $+\infty$. For nonzero $x$, $y$ and $x+y$, the strong triangle inequality gives
$$\ell^{-v_\ell(x+y)}\le\max(\ell^{-v_\ell(x)},\ell^{-v_\ell(y)})=\ell^{-\min(v_\ell(x),v_\ell(y))}.$$
Strict decrease gives $v_\ell(x+y)\ge\min(v_\ell(x),v_\ell(y))$. If $x+y=0$, the left side of the valuation inequality is $+\infty$. If one summand is zero and the sum is nonzero, the nonzero summand gives both sides. Finally, $|\ell|_\ell=\ell^{-1}$ on the rational copy, so $v_\ell(\ell)=1$.

The coordinate classes are the classes of [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n). Their two operations are independent of representatives by [math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n). By [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer), $a\equiv b\pmod{M}$ means $M\mid(a-b)$ for every integer modulus $M$. By [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z), this is equivalent to $a-b=Mq$ for some $q\in\mathbb Z$. If $a\equiv b\pmod{\ell^{n+1}}$, then $a-b=\ell^{n+1}q=\ell^n(\ell q)$ for some $q\in\mathbb Z$, and hence $a\equiv b\pmod{\ell^n}$. Thus the reduction maps are well defined. The formulas on representatives show that reduction preserves both operations and the classes of $0$ and $1$. It also preserves additive inverses, because the inverse of $[a]_n$ is $[-a]_n$. The coordinate ring laws from [math:thm-integers-modulo-n-basic-algebra](https://alphabetamath.cc/item/thm-integers-modulo-n-basic-algebra) therefore hold on the compatible tuples of [math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes).

The source ring in [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp) is this same inverse limit with transition maps given by reduction modulo the lower power. Step 1.2 of the comparison theorem sends a compatible tuple to the Cauchy class $\xi=[(b_n)]$ of its standard integer lifts, where $b_n$ is the representative of the $n$th coordinate in $[0,\ell^n)$. For fixed $n$, the quotient metric $d$ in Step 1.1 of [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field) gives $d(b_n,\xi)=\lim_{j\to\infty}|b_n-b_j|_\ell$, with $b_n$ on the left embedded as a constant sequence. Given $\varepsilon>0$, the Cauchy condition gives an $N$ such that $|b_n-b_j|_\ell<\varepsilon/2$ for $n,j\ge N$. For each $n\ge N$, the bound passes to the real limit in $j$ by [math:lem-limit-preserves-order](https://alphabetamath.cc/item/lem-limit-preserves-order), so $d(b_n,\xi)\le\varepsilon/2<\varepsilon$. By [math:def-metric-convergence](https://alphabetamath.cc/item/def-metric-convergence), applied to $(b_{k+1})_{k\ge0}$ to index from zero, the embedded lifts converge to $\xi$.

For the tuple of residues of an integer $a$, write $b_n$ for that lift. Since $b_n\equiv a\pmod{\ell^n}$, their difference is a multiple of $\ell^n$. If the difference is nonzero then $v_\ell(b_n-a)\ge n$ by the integer exponent formula, so $|b_n-a|_\ell\le\ell^{-n}$ by strict decrease. The same bound holds when the difference is zero. By the power laws, $\ell^{-n}=(1/\ell)^n$. In the real ordered field, reciprocating $0<1<\ell$ gives $0<1/\ell<1$ by [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive). The nonnegative clause of the ordinary real absolute value [math:def-abs-value](https://alphabetamath.cc/item/def-abs-value) gives $|1/\ell|=1/\ell<1$. Thus [math:lem-geometric-sequence-null](https://alphabetamath.cc/item/lem-geometric-sequence-null) gives $\ell^{-n}\to0$. By [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit), for every rational $\varepsilon>0$ the upper bound $\ell^{-n}$ is eventually less than $\varepsilon$, so the nonnegative termwise distances $|b_n-a|_\ell$ tend to zero. The completion identifies $(b_n)$ with the constant sequence at $a$ by [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers), so the image of the residue tuple is the embedded integer $a$.

Under this embedding the image is the closed unit ball by [the valuation ring identification](https://alphabetamath.cc/item/cor-zp-is-the-valuation-ring-of-qp). Thus $x\in\mathbb Z_\ell$ exactly when $v_\ell(x)\ge0$, including $x=0$. For $x\ne0$, $v_\ell(1)=0$ and the product law applied to $xx^{-1}=1$ gives $v_\ell(x^{-1})=-v_\ell(x)$. Hence $x$ is a unit of $\mathbb Z_\ell$, meaning that both $x$ and $x^{-1}$ belong to the ring, exactly when $v_\ell(x)=0$.

Since $\mathbb Q_\ell$ is a field, its nonzero elements form a multiplicative group $\mathbb Q_\ell^\times$ by [math:def-field](https://alphabetamath.cc/item/def-field). Use [math:def-group-power](https://alphabetamath.cc/item/def-group-power) for the powers of the nonzero embedded prime $\ell$ in this group. The recursion $\ell^0=1$, $\ell^{k+1}=\ell^k\ell$ gives $v_\ell(\ell^k)=k$ for all natural $k$ by the [induction principle](https://alphabetamath.cc/item/thm-induction-principle), using $v_\ell(1)=0$, $v_\ell(\ell)=1$ and the product law. For $k>0$, the clause $\ell^{-k}=(\ell^k)^{-1}$ and the inverse law give $v_\ell(\ell^{-k})=-k$. Thus $v_\ell(\ell^m)=m$ for every $m\in\mathbb Z$, so every element of the value group is attained.

Every nonzero $x$ can be written as $a/b$ with $a,b\in\mathbb Z_\ell$ nonzero by taking $b=\ell^n$ for a nonnegative $n$ with $n+v_\ell(x)\ge0$, then $a=bx$. In fact $v_\ell(b)=n$ and $v_\ell(a)=n+v_\ell(x)$ by normalization and the product law. For any such fraction, the product law applied to $bx=a$ gives $v_\ell(x)=v_\ell(a)-v_\ell(b)$, so this difference is independent of the choice of fraction.

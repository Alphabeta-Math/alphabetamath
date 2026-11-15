---
title: Annular scaling and fixed interior covers
status: draft
research_item: lem-author-db87cb8e0bab-annular-scaling
dependency_level: 1
---

## Prerequisites

- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-ck-and-multi-index-notation-in-several-variables](https://alphabetamath.cc/item/def-ck-and-multi-index-notation-in-several-variables)
- [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)


## Statement

Let $n\ge1$ and $k\ge0$ be integers and $0<\alpha<1$. In $\mathbb R^n$ set $A=\{y:1/2<|y|<4\}$, $A'=\{y:1<|y|<2\}$ and $K=\overline{A'}=\{y:1\le|y|\le2\}$. For $R\ge1$ and $u\in C^k(RA;\mathbb R)$, where $RS=\{Ry:y\in S\}$, define $v(y)=u(Ry)$ and $w(y)=R^{-1}u(Ry)$ on $A$. Multi-index derivatives are taken in their canonical order. No boundary extension of $u$ to $\partial(RA)$ is assumed.

For every multi-index $\beta$ with $|\beta|\le k$ and every nonempty open $S\subseteq A$, the exact scaling identities are
$$D_y^\beta v(y)=R^{|\beta|}(D_x^\beta u)(Ry),\qquad D_y^\beta w(y)=R^{|\beta|-1}(D_x^\beta u)(Ry),$$
$$[D_y^\beta v]_{\alpha;S}=R^{|\beta|+\alpha}[D_x^\beta u]_{\alpha;RS},\qquad [D_y^\beta w]_{\alpha;S}=R^{|\beta|-1+\alpha}[D_x^\beta u]_{\alpha;RS}.$$
Here $[f]_{\alpha;S}=\sup_{y,z\in S,\,y\ne z}|f(y)-f(z)|/|y-z|^\alpha$; seminorms may equal $+\infty$.

For $h\in C^k(S;\mathbb R)$ use the ordinary norm convention
$$\|h\|_{C^{k,\alpha}(S)}=\sum_{j=0}^k\max_{|\beta|=j}\sup_S|D^\beta h|+\sum_{|\beta|=k}[D^\beta h]_{\alpha;S}.$$
Consequently the annular rescaling, with the same convention for any such $S$, satisfies
$$\|v\|_{C^{k,\alpha}(S)}=\sum_{j=0}^k R^j\max_{|\beta|=j}\sup_{RS}|D_x^\beta u|+R^{k+\alpha}\sum_{|\beta|=k}[D_x^\beta u]_{\alpha;RS},\qquad \|w\|_{C^{k,\alpha}(S)}=R^{-1}\|v\|_{C^{k,\alpha}(S)}.$$

There is a fixed finite family of centers $p_1,\ldots,p_N\in K$, depending only on $n$, such that the balls $B_r(p_i)$ cover $K$, where $r=1/16$, and every enlarged ball $B_{4r}(p_i)$ lies in $A$. In particular the smaller concentric balls $B_{2r}(p_i)$ also cover $K$. For every $h\in C^k(A;\mathbb R)$ with $M:=\max_i\|h\|_{C^{k,\alpha}(B_{2r}(p_i))}<\infty$,
$$\|h\|_{C^{k,\alpha}(A')}\le C_{n,k,\alpha} M,\qquad C_{n,k,\alpha}:=(k+1)+N_{n,k}\max\{1,2r^{-\alpha}\},\qquad N_{n,k}:=\#\{\beta\in\mathbb N^n:|\beta|=k\}.$$
Thus ball estimates on the smaller balls, obtained using these enlarged balls, imply a full annular estimate, including the global Hölder seminorm, with a constant independent of $R$.

The same conclusion applies to families indexed by $R$ and any further parameter whenever the local estimates have common constants on the specified parameter set; uniformity at a parameter endpoint is not inferred from separate pointwise estimates. In the three-dimensional exterior-chart setting $E=\{x:|x|>R_0\}$ with $R_0>0$, if $u$ is given only on $E$, require $R\ge1$ and $R/2>R_0$ so that $RA\subset E$. Uniform end bounds retain their common-chart, common-radius and common-constant meaning.

## Facts & Assumptions

[F1] The class $C^k$ requires continuous iterated coordinate derivatives through order $k$; $D^\beta$ uses the fixed canonical order. [math:def-ck-and-multi-index-notation-in-several-variables](https://alphabetamath.cc/item/def-ck-and-multi-index-notation-in-several-variables)

[F2] Ordinary Hölder seminorms and norms use Euclidean distances, derivative suprema and top-order difference quotients; scaled norms attach the indicated powers of radius. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F3] Exterior differentiated bounds and parameter uniformity require a specified Cartesian chart and common radii and constants on the specified parameter set. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F4] A closed bounded subset of $\mathbb R^n$, $n\ge1$, is compact in its Euclidean metric: every open cover has a finite subcover. [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)

## Proof

**Given:** The hypotheses and norm conventions in the Statement.

**Goal:** Prove the exact scaling identities and the full fixed-cover annular estimate.

1.1 If $k\ge1$, for any coordinate unit vector $e_i$ and any iterated coordinate derivative $q$ of $u$ of order less than $k$, the difference quotient after dilation is
$$\frac{q(R(y+t e_i))-q(Ry)}{t}=R\frac{q(Ry+Rt e_i)-q(Ry)}{Rt}\longrightarrow R(\partial_iq)(Ry)\quad(t\to0).$$
For $y\in A$ the points involved lie in $RA$ for sufficiently small $|t|$, since $RA$ is open. Apply this calculation successively to every coordinate-derivative word through order $k$; all required derivatives exist by [F1]. In particular, the canonical order gives the asserted identities for $D^\beta v$, and multiplication by the constant $R^{-1}$ gives those for $D^\beta w$. Each resulting derivative is continuous, since its derivative of $u$ is continuous and $|Ry-Rz|=R|y-z|$ makes dilation continuous. Thus $v,w\in C^k(A)$. Order zero is the defining identity, including when $k=0$. [given, F1, algebra]

1.2 The reverse triangle inequality $\big||y|-|z|\big|\le|y-z|$ shows directly that the complement of $K$ is open: at a point with $|y|<1$ take a ball of radius $(1-|y|)/2$, and at one with $|y|>2$ take radius $(|y|-2)/2$. Also $K\subset B_3(0)$, so [F4] makes $K$ compact. The balls $B_r(p)$, for $p\in K$ and $r=1/16$, form an open cover. Take a finite subcover with centers $p_1,\ldots,p_N$. For $y\in B_{4r}(p_i)$, the same triangle inequalities give $3/4<|y|<9/4$; thus $B_{4r}(p_i)\subset A$. All these balls are fixed in $y$ coordinates, independently of $R$, $u$ or any further parameter. [given, F4, construct, algebra]

2.1 Dilation maps $S$ bijectively onto $RS$, so the derivative identities give the corresponding supremum factors $R^{|\beta|}$ and $R^{|\beta|-1}$. For distinct $y,z\in S$, substitute $x=Ry$, $x'=Rz$; then $|x-x'|=R|y-z|$. Each difference quotient for $D_y^\beta v$ is therefore $R^{|\beta|+\alpha}$ times the corresponding quotient for $D_x^\beta u$, and the factor for $w$ is $R^{|\beta|-1+\alpha}$. The pair correspondence is bijective, so taking suprema proves both seminorm equalities, also if they are infinite. Summation in the stated norm convention proves the norm identities. [given, F2, step 1.1, algebra]

2.2 Put $M=\max_i\|h\|_{C^{k,\alpha}(B_{2r}(p_i))}$. Every $y\in A'$ belongs to some $B_r(p_i)\subset B_{2r}(p_i)$, so each derivative supremum in the norm on $A'$ is at most $M$. For distinct $y,z\in A'$ with $|y-z|<r$, choose $i$ with $|y-p_i|<r$. Then $|z-p_i|<2r$, and the $\alpha$-Hölder quotient of each $D^\beta h$ with $|\beta|=k$ is bounded by its seminorm on $B_{2r}(p_i)$, hence by $M$. Thus the fixed margin $r$ controls every nearby pair. [given, F1, F2, step 1.2, algebra]

3.1 For the remaining pairs, $|y-z|\ge r$, each numerator $|D^\beta h(y)-D^\beta h(z)|$ is at most $2M$, so its Hölder quotient is at most $2r^{-\alpha}M$. Together with step 2.2 this bounds each top-order seminorm by $\max\{1,2r^{-\alpha}\}M$. There are $N_{n,k}$ such multi-indices, and $k+1$ derivative-supremum terms. Summing gives exactly $\|h\|_{C^{k,\alpha}(A')}\le C_{n,k,\alpha}M$ as stated. [given, F2, step 2.2, algebra]

4.1 Apply the fixed-cover estimate to $h=v$ or $h=w$ and use the exact rescaling identities of step 2.1. If the local estimates are bounded by a common local constant times a given right-hand side, their finite maximum has that same bound, and step 3.1 multiplies it only by $C_{n,k,\alpha}$. Neither the balls nor this factor depend on $R$ or a further parameter. For an exterior chart in dimension three, $y\in A$ gives $|Ry|>R/2>R_0$, which verifies the domain condition; [F3] specifies precisely when end estimates and their constants are uniform. This proves all the claimed scaling and uniform annular conclusions. [given, F3, step 2.1, step 1.2, step 3.1, algebra] ∎

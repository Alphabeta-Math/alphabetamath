---
title: One extra pointwise derivative supplies scaled Hölder control
status: draft
research_item: lem-author-45355d85383b-scaled-decay-holder-upgrade
dependency_level: 1
---

## Prerequisites

- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)


## Statement

Let $m\geq0$ be an integer, $b\in\mathbb R$, and $0<\alpha<1$. For a smooth scalar or finite component array on a Cartesian end $E=\{x\in\mathbb R^3:|x|>R_0\}$, where $R_0>0$ and $r=|x|$, the differentiated bound $f=O_{m+1}(r^{-b})$ implies an eventual weighted $C^{m,\alpha}$ bound of decay order $b$. Precisely, writing $A_R=\{x:R<|x|<2R\}$, there are $R_*>R_0$ and $C<\infty$ such that, for every $R\geq R_*$ and every component,
$$\sum_{|\beta|\leq m}R^{b+|\beta|}\sup_{A_R}|\partial^\beta f|+\sum_{|\beta|=m}R^{b+m+\alpha}[\partial^\beta f]_{\alpha;A_R}\leq C.$$
Here $[v]_{\alpha;A}=\sup_{x,y\in A,\,x\ne y}|v(x)-v(y)|/|x-y|^\alpha$. In this item the notation $f\in C^{m,\alpha}_{-b}$ means exactly this eventual annular bound; it imposes no boundedness as $r$ approaches $R_0$.

The same conclusion holds with a common $R_*$ and $C$ for families whose input bounds have a common radius and constants. In particular, stationary coefficient errors $g_{00}+1$ and $g_{ij}-\delta_{ij}$ satisfying $O_5(r^{-1})$ have eventual $C^{4,\alpha}_{-1}$ control, and a mixed component $g_{0i}=O_5(r^{-2})$ has eventual $C^{4,\alpha}_{-2}$ control. Equivalently their rescalings $R(g_{00}+1)(R\,\cdot)$, $R(g_{ij}-\delta_{ij})(R\,\cdot)$ and $R^2g_{0i}(R\,\cdot)$ have bounded ordinary $C^{4,\alpha}$ norms on the fixed annulus $A_1$, uniformly for sufficiently large $R$.

## Statement references

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

## Facts & Assumptions

[F1] Differentiated end bounds use Cartesian multi-index derivatives and an eventual common exterior radius. The weighted Hölder bound is defined by the displayed annular expression; for families uniformity requires a common radius and constants. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] Ordinary Hölder norms consist of derivative suprema and top-derivative difference quotients. Radius powers account for derivative and seminorm rescaling. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F3] A real function continuous on a closed interval and differentiable in its interior has its endpoint difference equal to the interval length times an interior derivative. We use this scalar mean value theorem on coordinate segments, separately on real and imaginary parts if needed. [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

## Proof

**Given:** The differentiated end bound in the Statement, with radius $R_1>R_0$ and constants common to the finitely many components and, for a uniform family, to all parameters.

**Goal:** Prove the eventual annular bound, its uniformity assertion and the coefficient examples.

1.1 For $R\geq2R_1$ put $f_R(y)=R^bf(Ry)$ on the fixed enlarged annulus $U=\{y:1/2<|y|<3\}$. Coordinate differentiation gives $\partial^\beta f_R(y)=R^{b+|\beta|}(\partial^\beta f)(Ry)$. The input bound implies $|\partial^\beta f_R(y)|\leq C_\beta |y|^{-b-|\beta|}$ for $|\beta|\leq m+1$. Since $1/2<|y|<3$ and there are finitely many multi-indices and components, one finite number $M\geq0$, independent of $R$, bounds all these derivatives on $U$. For a uniform family the same $M$ works for every parameter. [given, F1, F2, algebra]

2.1 Fix one component and $|\beta|=m$, and put $v=\partial^\beta f_R$. If $p,q\in A_1$ and $0<|p-q|<1/4$, change the three coordinates of $p$ successively to those of $q$. Every point of these three coordinate segments is within distance $|p-q|$ of $p$, so lies in $B_{1/4}(p)\subset U$. On each nondegenerate segment, $v$ is smooth, hence continuous at both endpoints and differentiable in its interior, with the relevant coordinate derivative bounded by $M$. Applying [F3] to each real component and summing the three endpoint differences gives $|v(p)-v(q)|\leq6M|p-q|$, where the factor six also accommodates complex components by treating real and imaginary parts separately. Thus the Hölder quotient for these pairs is at most $6M(1/4)^{1-\alpha}$. If $|p-q|\geq1/4$, the supremum bound gives a quotient at most $2M4^\alpha$. Consequently $[\partial^\beta f_R]_{\alpha;A_1}$ is bounded independently of $R$, and together with step 1.1 this bounds the ordinary $C^{m,\alpha}$ norm of $f_R$ on $A_1$. No convexity of the entire annulus is assumed. [step 1.1, F2, F3, algebra]

3.1 The dilation $x=Ry$ bijects $A_1$ with $A_R$, and its difference quotients give $[\partial^\beta f_R]_{\alpha;A_1}=R^{b+|\beta|+\alpha}[\partial^\beta f]_{\alpha;A_R}$. The derivative suprema obey the corresponding identity without the factor $R^\alpha$. Summing the finitely many bounds in steps 1.1 and 2.1 proves the displayed weighted bound for $R\geq R_*=2R_1$. Common input bounds give the same $M$, $R_*$ and final constant for the whole family. Finally take $m=4$ and $b=1$ for the time and spatial coefficient errors, and $m=4$ and $b=2$ for each mixed component; steps 1.1 and 2.1 also give exactly the stated fixed-annulus rescaled bounds. These conclusions concern only the sufficiently far-out end specified in the Statement. [step 1.1, step 2.1, F1, F2, algebra] ∎

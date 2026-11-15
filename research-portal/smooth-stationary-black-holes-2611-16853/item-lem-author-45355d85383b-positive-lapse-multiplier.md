---
title: The transverse lapse is a positive weighted Dirichlet multiplier
status: published
research_item: lem-author-45355d85383b-positive-lapse-multiplier
dependency_level: 5
---

## Prerequisites

- [lem-author-45355d85383b-induced-metric-and-normal-decay](item-lem-author-45355d85383b-induced-metric-and-normal-decay)
- [lem-author-45355d85383b-weighted-smooth-inversion](item-lem-author-45355d85383b-weighted-smooth-inversion)
- [lem-author-45355d85383b-weighted-holder-completeness](item-lem-author-45355d85383b-weighted-holder-completeness)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-weighted-holder-spaces](item-def-weighted-holder-spaces)
- [lem-author-45355d85383b-scaled-decay-holder-upgrade](item-lem-author-45355d85383b-scaled-decay-holder-upgrade)
- [lem-author-45355d85383b-weighted-products-and-derivatives](item-lem-author-45355d85383b-weighted-products-and-derivatives)
- [physics:lem-gr-observer-pairing-with-future-causal-vectors](https://alphabetamath.cc/physics/item/lem-gr-observer-pairing-with-future-causal-vectors)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in ZFC. Fix $0<\alpha<1$, $q>0$, $d_q>0$ and $\beta\in\mathbb R$, and put $c=d_q/(4q)$. Let $g$ be a smooth time-oriented Lorentzian metric of signature $(-,+,+,+)$, and let $\Sigma_1$ be a supplied smooth embedded spacelike reference hypersurface with compact smooth boundary $S$ and one exterior end, with the fixed compact-core and end-chart data of the weighted Hölder norms. Let $n$ be its smooth future unit normal, including at $S$.

On a stationary Cartesian ambient end $(t_q,x_q)$, the coefficients of $g$ are independent of $t_q$, $r_q=|x_q|>R_0>0$, and $\partial_{t_q}$ is future timelike sufficiently far out. Assume $g_{00}+1,g_{ij}-\delta_{ij}=O_5(r_q^{-1})$ and $g_{0i}=O_5(r_q^{-2})$. Here $f=O_5(r_q^{-b})$ means $|D^j f|\le C_j r_q^{-b-j}$ for $0\le j\le5$ outside a common radius, with $D$ denoting Cartesian spatial derivatives in $x_q$. Spatial indices range from $1$ to $3$ and repeated spatial indices are summed. The end of $\Sigma_1$ is a supplied smooth spacelike maximal graph $t_q=u(x_q)$ with $|D^j u|\le C r_q^{-3/4-j}$ for $0\le j\le4$. The fixed end chart $x$ is related by $x_q=qx$; all weighted spaces below use $x$ and the fixed core charts. No graph existence is asserted.

Let $Y$ be smooth future timelike and transverse along the reference slice, equal to $n$ on a compact neighborhood of $S$ and equal to the supplied stationary field $T$ sufficiently far out, where $T=c\partial_{t_q}$. Then $a=-g(Y,n)$ is smooth, equals one near $S$, satisfies $a-c\in C^{4,\alpha}_{-1}$ on the end, and has a positive global lower bound. Consequently multiplication $w\mapsto aw$ is a bounded isomorphism of $X_\beta=\{w\in C^{4,\alpha}_\beta(\Sigma_1):w|_S=0\}$ onto itself, with inverse multiplication by $a^{-1}$.

## Facts & Assumptions

[F1] Under the stated stationary background bounds and the supplied maximal graph estimates through order four, the normal-decay lemma in ZFC gives $n^0-1\in C^{4,\alpha}_{-1}$ and $n^i\in C^{4,\alpha}_{-7/4}$ on the normalized end. Its fixed positive-$q$ coordinate comparison preserves these weighted exponents under $x_q=qx$. [lem-author-45355d85383b-induced-metric-and-normal-decay](item-lem-author-45355d85383b-induced-metric-and-normal-decay)

[F2] If $a\in C^{4,\alpha}_0$ has a positive global lower bound, then $a^{-1}\in C^{4,\alpha}_0$, and multiplication by either function is bounded on every $C^{4,\alpha}_\beta$. [lem-author-45355d85383b-weighted-smooth-inversion](item-lem-author-45355d85383b-weighted-smooth-inversion)

[F3] For the fixed exterior data in ZFC, the weighted spaces are complete, boundary restriction into $C^0(S)$ is continuous, and $X_\beta$ is a closed Banach subspace of $C^{4,\alpha}_\beta$. [lem-author-45355d85383b-weighted-holder-completeness](item-lem-author-45355d85383b-weighted-holder-completeness)

[F4] The spacelike hypersurface has its smooth future unit normal with $g(n,n)=-1$. The lapse of an ambient vector field $Y$ is $-g(Y,n)$; the definition alone imposes no sign. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F5] The differentiated background bounds $g_{00}+1=O_5(r_q^{-1})$ and $g_{0i}=O_5(r_q^{-2})$ give eventual $C^{4,\alpha}_{-1}$ and $C^{4,\alpha}_{-2}$ bounds, respectively, by the one-extra-derivative Hölder upgrade. [lem-author-45355d85383b-scaled-decay-holder-upgrade](item-lem-author-45355d85383b-scaled-decay-holder-upgrade)

[F6] The weighted norm consists of the fixed compact-core norm and the supremum of scaled annular norms; the same convention measures finite arrays componentwise. [def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[F7] Weighted products add their weights and inclusion holds from a smaller weight to a larger one. The product supplier proves the scaled-annulus product estimate in Proof step 2.1 and the weight inclusion estimate in Proof step 4.1. [lem-author-45355d85383b-weighted-products-and-derivatives](item-lem-author-45355d85383b-weighted-products-and-derivatives)

[F8] For a future unit timelike vector $n$ and any nonzero future causal vector $Y$ in a time-oriented Lorentzian four-manifold, $-g(n,Y)>0$. This supplier has domain mathematics. [physics:lem-gr-observer-pairing-with-future-causal-vectors](https://alphabetamath.cc/physics/item/lem-gr-observer-pairing-with-future-causal-vectors)

[A1] ZFC includes the Axiom of Choice. It is carried when invoking the normal-decay and weighted-completeness suppliers; the finite component computations introduce no additional choice assumption. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The supplied exterior, stationary metric, maximal end graph, field, decay and ZFC hypotheses in the Statement.

**Goal:** Prove the lapse asymptotics, global positivity and bounded Dirichlet multiplier isomorphism.

1.1 The supplied graph, the stationary metric, their differentiated bounds and the range $0<\alpha<1$ satisfy all hypotheses of [F1]. Under [A1], it gives $n^0-1\in C^{4,\alpha}_{-1}$ and $n^i\in C^{4,\alpha}_{-7/4}$ in $x_q$. Independently [F5] gives $e=g_{00}+1\in C^{4,\alpha}_{-1}$ and $g_{0i}\in C^{4,\alpha}_{-2}$. These are end component estimates; stationarity means restricting a metric component to the graph just evaluates that spatial function. [given, F1, F5, F6, A1]

2.1 Where $Y=T=c\partial_{t_q}$, contraction gives $a=-c(g_{00}n^0+g_{0i}n^i)$ and hence $a-c=c\bigl((n^0-1)-en^0-g_{0i}n^i\bigr)$. By [F7], $en^0=e+e(n^0-1)$ has weight $-1$, and $g_{0i}n^i$ has weight $-15/4$, which includes into weight $-1$. Thus $a-c\in C^{4,\alpha}_{-1}$ on the normalized end. The fixed-$q$ scaling in [F1], equivalently rescaling the annuli of [F6] by $q$, gives the same exponent in $x$. In particular $a\to c>0$ uniformly at infinity. [given, F1, F6, F7, step 1.1, algebra]

3.1 Smoothness follows from the smooth metric and normal in [F4] and the given smooth field $Y$. Near $S$ the equality $Y=n$ gives $a=-g(n,n)=1$. Everywhere $n$ is future unit timelike and $Y$ is nonzero future timelike, so [F8] gives $a>0$. Step 2.1 supplies a radius outside which $a\ge c/2$. The remainder is compact by the exterior data. At each point $p$ of that remainder, continuity gives a relative neighborhood on which $a>a(p)/2>0$. A finite subcover yields a positive lower bound there by taking the minimum of its finitely many positive bounds. Combining this with $c/2$ proves the global lower bound; an empty remainder needs no compact-part bound. [given, F4, F6, F8, step 2.1, algebra]

4.1 On the end, the constant $c$ has finite weight-zero norm, and $a-c$ has weight $-1$ by step 2.1, so [F7] puts $a$ in weight zero there. On the fixed compact core and any intervening bounded end region, smoothness on neighborhoods of the compact chart subsets gives finite derivative suprema and fourth-derivative Hölder seminorms. With the norm in [F6], this proves $a\in C^{4,\alpha}_0(\Sigma_1)$. Apply [F2] and step 3.1 to obtain $a^{-1}\in C^{4,\alpha}_0$ and inverse bounded multiplication operators on $C^{4,\alpha}_\beta$. Boundary restriction is pointwise and continuous by [F3]; since $a$ never vanishes, $w|_S=0$ if and only if $(aw)|_S=0$. Thus both operators preserve the closed Banach domain $X_\beta$ from [F3], used under [A1], and restrict to bounded inverses on it. [F2, F3, F6, F7, A1, step 2.1, step 3.1, algebra] ∎

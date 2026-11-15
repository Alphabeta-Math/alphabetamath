---
title: Compact multiplication by a faster-decaying potential
status: published
research_item: lem-author-86990d62062f-compact-potential
dependency_level: 1
---

## Prerequisites

- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [math:def-compact-linear-operator](https://alphabetamath.cc/item/def-compact-linear-operator)
- [math:thm-arzela-ascoli-for-real-ck](https://alphabetamath.cc/item/thm-arzela-ascoli-for-real-ck)
- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [math:thm-holder-spaces-on-bounded-domains-are-banach-spaces](https://alphabetamath.cc/item/thm-holder-spaces-on-bounded-domains-are-banach-spaces)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [math:thm-metric-compactness-equivalences](https://alphabetamath.cc/item/thm-metric-compactness-equivalences)
- [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)
- [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)


## Statement

Work in ZFC. Let $\Sigma$ be the smooth three-dimensional exterior with compact smooth boundary $S$ and fixed weighted norms, let $0<\alpha<1$ and $\beta\in\mathbb R$, and put $X_\beta=\{u\in C^{4,\alpha}_\beta:u|_S=0\}$ and $Y_\beta=C^{2,\alpha}_{\beta-2}$. For every real $V\in C^{2,\alpha}_{-4}$, multiplication $u\mapsto Vu$ is a bounded compact linear map from $X_\beta$ to $Y_\beta$.

The same assertion holds with finitely many compact extra components, with the following precise conventions. Let $M_1,\ldots,M_m$ be compact smooth three-manifolds, each with possibly empty smooth boundary, where $m\ge0$. On each $M_j$ fix finitely many coordinate balls or boundary half-balls whose closures lie in larger charts and whose relative interiors cover $M_j$. Define $C^{k,\alpha}(M_j)$ by $C^k$ regularity up to the boundary and finite ordinary $C^{k,\alpha}$ norm on these closed patches, and use the sum of their coordinate derivative suprema through order $k$ and order-$k$ Hölder seminorms as its norm. Put $X_j=\{u_j\in C^{4,\alpha}(M_j):u_j|_{\partial M_j}=0\}$, with no boundary restriction when $\partial M_j=\varnothing$, and $Y_j=C^{2,\alpha}(M_j)$. Given real $V_j\in C^{2,\alpha}(M_j)$, componentwise multiplication by $(V,V_1,\ldots,V_m)$ is compact from $X_\beta\oplus\bigoplus_{j=1}^m X_j$ to $Y_\beta\oplus\bigoplus_{j=1}^m Y_j$, with the sum norm on each finite direct sum.

## Facts & Assumptions

**Given:** the hypotheses and norm conventions in the Statement; work in ZFC.

**Goal:** prove both compactness assertions.

[F1] The exterior, weighted annular norms and Dirichlet spaces are those of the weighted exterior definition. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F2] For real normed spaces, a linear map is compact exactly when the image of every bounded set has compact closure in the target norm metric. [math:def-compact-linear-operator](https://alphabetamath.cc/item/def-compact-linear-operator)

[F3] On a compact metric space, an equicontinuous pointwise bounded family of real continuous functions has compact closure in the supremum metric, assuming Countable Choice and Dependent Choice. [math:thm-arzela-ascoli-for-real-ck](https://alphabetamath.cc/item/thm-arzela-ascoli-for-real-ck)

[F4] On every bounded nonempty Euclidean open set, the finite-norm boundary-extension class $C^{2,\alpha}(\overline\Omega;\mathbb R)$ is Banach under Countable Choice. This includes balls, half-balls and annuli; no smoothness of the boundary is needed for this closure-class assertion. [math:thm-holder-spaces-on-bounded-domains-are-banach-spaces](https://alphabetamath.cc/item/thm-holder-spaces-on-bounded-domains-are-banach-spaces)

[F5] Ordinary Hölder norms, scaled derivative norms and boundary-extension classes use the declared Euclidean conventions. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F6] ZFC includes the Axiom of Choice, hence supplies the Countable Choice and Dependent Choice used in local completeness, subsequence extraction and metric compactness. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F7] For metric spaces, sequential compactness and compactness are equivalent under Countable Choice and Dependent Choice. [math:thm-metric-compactness-equivalences](https://alphabetamath.cc/item/thm-metric-compactness-equivalences)

[F8] For components with empty boundary use the smooth-manifold convention; for those with nonempty boundary use smooth boundary atlases with transitions smooth in the local-extension sense. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

## Proof

**Given:** the hypotheses and norm conventions in the Statement; work in ZFC.

**Goal:** prove both compactness assertions.

[F1] The exterior, weighted annular norms and Dirichlet spaces are those of the weighted exterior definition. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F2] For real normed spaces, a linear map is compact exactly when the image of every bounded set has compact closure in the target norm metric. [math:def-compact-linear-operator](https://alphabetamath.cc/item/def-compact-linear-operator)

[F3] On a compact metric space, an equicontinuous pointwise bounded family of real continuous functions has compact closure in the supremum metric, assuming Countable Choice and Dependent Choice. [math:thm-arzela-ascoli-for-real-ck](https://alphabetamath.cc/item/thm-arzela-ascoli-for-real-ck)

[F4] On every bounded nonempty Euclidean open set, the finite-norm boundary-extension class $C^{2,\alpha}(\overline\Omega;\mathbb R)$ is Banach under Countable Choice. This includes balls, half-balls and annuli; no smoothness of the boundary is needed for this closure-class assertion. [math:thm-holder-spaces-on-bounded-domains-are-banach-spaces](https://alphabetamath.cc/item/thm-holder-spaces-on-bounded-domains-are-banach-spaces)

[F5] Ordinary Hölder norms, scaled derivative norms and boundary-extension classes use the declared Euclidean conventions. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F6] ZFC includes the Axiom of Choice, hence supplies the Countable Choice and Dependent Choice used in local completeness, subsequence extraction and metric compactness. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F7] For metric spaces, sequential compactness and compactness are equivalent under Countable Choice and Dependent Choice. [math:thm-metric-compactness-equivalences](https://alphabetamath.cc/item/thm-metric-compactness-equivalences)

**Proof technique:** direct.

1.1 Write $\|\cdot\|^*_{k,\alpha;A_R}$ for the parenthesized scaled annular quantity in the weighted norm. Leibniz' rule and $[ab]_\alpha\le\|a\|_\infty[b]_\alpha+\|b\|_\infty[a]_\alpha$ give the ordinary $C^{2,\alpha}$ product bound. Lower-derivative Hölder seminorms are controlled by suprema of the next derivatives on balls and half-balls; a finite cover and the bound for pairs separated by a fixed positive distance give the same estimates on the unit annulus. Rescaling $x=Rz$ therefore gives $\|Vu\|^*_{2,\alpha;A_R}\le C\|V\|^*_{2,\alpha;A_R}\|u\|^*_{4,\alpha;A_R}$ and hence $R^{-(\beta-2)}\|Vu\|^*_{2,\alpha;A_R}\le CR^{-2}\|V\|_{C^{2,\alpha}_{-4}}\|u\|_{C^{4,\alpha}_\beta}$ for all $R\ge r_0$, with $C$ independent of $R$ and $u$. The finite compact-core norms satisfy the same unweighted product bound. On each $M_j$ the fixed chart norms likewise give $\|V_ju_j\|_{C^{2,\alpha}(M_j)}\le C_j\|V_j\|_{C^{2,\alpha}(M_j)}\|u_j\|_{C^{4,\alpha}(M_j)}$. These bounds prove that the componentwise linear map is bounded and well-defined. [F1, F5, F8, given, algebra]

2.1 Take any sequence bounded in the stated domain. The weighted bounds control all coordinate derivatives through order four on compact chart patches: use the finite core cover, finitely many annuli on any bounded end region, and bounded smooth chart-transition derivatives on compact overlaps. On compact extra components this follows directly from their fixed norms. For each patch use smaller closed balls or half-balls inside larger charts. Bounds through order four make the derivatives through order three equicontinuous and bounded, so Ascoli and a diagonal extraction give a subsequence for which these derivatives converge uniformly on a countable exhaustion. Include the bounded end-coordinate annuli $\{r_0<r<T\}$ for an increasing sequence of $T\to\infty$ in this extraction: finitely many overlapping $A_R$ control each such annulus, and derivative bounds give continuous extensions to its closure. This also controls pairs approaching its artificial inner sphere $r=r_0$. For a difference $w$ of two terms, the near-pair mean-value estimate and the far-pair supremum estimate on a convex patch give $[D^2w]_\alpha\le C\|D^2w\|_\infty^{1-\alpha}\|D^3w\|_\infty^\alpha$; a finite patch cover handles each annulus. Thus the subsequence is Cauchy in the ordinary $C^{2,\alpha}$ norm on every such patch and bounded end annulus. Local completeness supplies genuine $C^{2,\alpha}$ limits. Their function values agree on overlaps by uniform convergence, so they glue on $\Sigma$ and each $M_j$. Multiplication by the fixed potentials is continuous in these local norms by step 1.1, giving glued local limits $v$ of $Vu_n$ and $v_j$ of $V_ju_{j,n}$. [F1, F3, F4, F5, F6, F8, step 1.1]

3.1 Let $M$ bound the exterior input norms along this subsequence and set $B=C\|V\|_{C^{2,\alpha}_{-4}}M$. For every fixed $R\ge r_0$, pass to the limit in each derivative-value bound and each two-point Hölder bound from step 1.1. Taking the same suprema, maxima and finite sums gives $R^{-(\beta-2)}\|v\|^*_{2,\alpha;A_R}\le BR^{-2}$. The compact-core norm of $v$ is finite by its local $C^{2,\alpha}$ regularity. Consequently $v\in Y_\beta$, and the same finite-chart argument gives $v_j\in Y_j$. This constructs limits inside the specified targets without assuming completeness of a weighted space. [F1, F5, step 1.1, step 2.1]

4.1 For $R\ge T$, the two bounds for $Vu_n$ and $v$ give $R^{-(\beta-2)}\|Vu_n-v\|^*_{2,\alpha;A_R}\le2BT^{-2}$. For $r_0\le R<T$, all the annuli lie in the bounded end-coordinate region $\{r_0<r<2T\}$, and the powers of $R$ in their scaled norms are uniformly bounded because $R\in[r_0,T]$. Step 2.1 therefore makes the supremum of these remaining annular terms tend to zero. The compact-core norm tends to zero as well: a finite smaller-chart cover handles near pairs in each fixed core subset, and uniform convergence handles pairs a fixed distance apart. Choose $T$ first to make $2BT^{-2}$ small, and then choose $n$ to make the bounded-region terms small. This proves $Vu_n\to v$ in the full $Y_\beta$ norm. On the finitely many $M_j$ the local convergence from step 2.1 gives convergence in each full $Y_j$ norm, hence convergence in the finite direct-sum target norm. [F1, F5, step 1.1, step 2.1, step 3.1]

5.1 Every sequence in the image of a bounded domain set now has a subsequence converging in the target. The closure of that image is sequentially compact: for a sequence $z_n$ in the closure choose image points $y_n$ with target distance less than $1/n$ from $z_n$; a convergent subsequence of $y_n$ gives a subsequence of $z_n$ with the same limit, which lies in the closure. The metric compactness equivalence makes this closure compact. This is the required compactness, both for the exterior alone and for the finite direct sum. [F2, F6, F7, step 4.1] ∎

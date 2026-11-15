---
title: "Proposition 4.1: positive-expansion spheres of limiting area 4π"
status: published
research_item: pthm-comparison-sphere-properties
dependency_level: 12
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 21–22, Proposition 4.1 and its proof
      attribution: The comparison spheres have positive outward null expansion,
        enclose the bifurcation sphere in stationary projection, have timelike
        stationary cylinders and exterior temporal coordinate, and their
        transformed areas tend to 4π.
      hypotheses: The article's mass-one stationary vacuum construction, its specified
        Harrison family, and 0 < q ≤ 1 with a sufficiently large fixed radius
        constant.
      reading_limits: The frozen article text at Proposition 4.1 and its proof was
        read for attribution. The article's assertion is not used as a proof
        premise below.
---

PDF p. 21: ` Proposition 4.1 `; PDF p. 22: ` Proof of Proposition 4.1; (4.2) `

## Prerequisites

- [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)
- [pthm-sphere-area-expansion-estimates](item-pthm-sphere-area-expansion-estimates)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)


## Statement

Work in ZFC with the regular stationary vacuum data of [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime), the model assumptions of [post-stationary-vacuum-model](item-post-stationary-vacuum-model), and the mass-one end, pole, normalized Ernst potential and specified Harrison family required by [pthm-sphere-area-expansion-estimates](item-pthm-sphere-area-expansion-estimates). In the original stationary end coordinates, let $C_q=\{t=0,\ r=R_0q^{-2/3}\}$ for $0<q\leq1$, as in [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres). The transformed metric is $g_q$.

For a sufficiently large fixed $R_0$, independent of $q$, each $C_q$ is a smooth embedded $g_q$-spacelike two-sphere. Its stationary projection onto the original section surrounds the bifurcation sphere $S$ in the following intrinsic sense. Put $B=(\Sigma_0\cap\mathcal E)\cup S$. For $R=R_0q^{-2/3}$, the truncation $K_q=B\setminus\{t=0,r>R\}$ is a compact smooth region with boundary $S\sqcup C_q$, where $r$ is the original end radius. The future outward null expansion of $C_q$ is strictly positive; its stationary cylinder is timelike, and $t$ is temporal on the exterior side $r\geq R_0q^{-2/3}$. Moreover $|C_q|_{g_q}\to4\pi$ as $q\downarrow0$. Here temporal means that $dt$ is timelike; the null expansion is the trace of the null second fundamental form as defined in [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data).

## Facts & Assumptions

[A1] The construction uses ZFC, including the axiom of choice, and the stated stationary vacuum model. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[F1] The coordinate definition gives smooth embedded spheres $C_q$, their stationary translates $\{t=s,r=R_0q^{-2/3}\}$, and $R_0q^{-2/3}\to\infty$ with $qR_0q^{-2/3}\to0$ as $q\downarrow0$. [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)

[F2] The original section $\Sigma_0$ agrees with $t=0$ on the actual stationary end. Its closed exterior portion $B=(\Sigma_0\cap\mathcal E)\cup S$ is a smooth embedded manifold with compact boundary $S$. For every sufficiently large original end radius $R$, the truncation $B\setminus\{t=0,r>R\}$ is a compact smooth region with boundary $S\sqcup\{t=0,r=R\}$. This is the compact-truncation conclusion of the existing section supplier under the regular-spacetime hypotheses. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)

[F3] For all sufficiently large $R$, uniformly in $q\in[0,1]$ and angle, the supplied estimate gives $|\{t=0,r=R\}|_{g_q}=4\pi(1+qR)^2(1+O(R^{-1}))$ and $\theta_{L_q}=2q/(1+qR)+O(R^{-2})$. It also gives spacelike coordinate slices, timelike $dt$, and timelike stationary coordinate cylinders throughout that large-radius region. The future outward normal is normalized by $g_q(T,L_q)=-d_q/4$, where $d_q$ is the pole denominator. [pthm-sphere-area-expansion-estimates](item-pthm-sphere-area-expansion-estimates) [def-harrison-normalization](item-def-harrison-normalization) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

## Proof

**Given:** The data and parameter range in the Statement, and the uniform estimates in [F3].

**Goal:** Establish the geometric properties and limiting area for one sufficiently large fixed $R_0$.

1.1 Choose $R_0$ larger than the end threshold, the compact-truncation threshold in [F2], and the common large-radius threshold in [F3]. Since $q^{-2/3}\geq1$, every chosen radius $R=R_0q^{-2/3}$ is at least $R_0$. The spheres are smooth and embedded by [F1], and are spacelike because they lie in the spacelike coordinate slices of [F3]. The section agrees with $t=0$ on the original end, so $C_q$ already lies in that section. The stationary end flow is $(t,x)\mapsto(t+s,x)$; hence its projection $(t,x)\mapsto(0,x)$ fixes $C_q$. Apply [F2] at $R=R_0q^{-2/3}$: the region $K_q=B\setminus\{t=0,r>R\}$ is compact and smooth, with boundary $S\sqcup C_q$. This establishes the asserted intrinsic enclosure in the actual end coordinates. [given, F1, F2, F3]

2.1 The uniform expansion estimate has an error bounded in absolute value by $KR^{-2}$ for some constant $K$ independent of $q$, angle and sufficiently large $R$. For $0<q\leq1$, $2qR^2/(1+qR)=2R_0^2q^{-1/3}/(1+R_0q^{1/3})\geq2R_0^2/(1+R_0)$. Increase $R_0$ until the final quantity exceeds $K$. The leading term then strictly exceeds the absolute error everywhere on every $C_q$, so $\theta_{L_q}>0$. The normal is future outward by [F3], and its expansion has the stated meaning. [given, F3, step 1.1, algebra]

3.1 By [F3], the stationary cylinder at each chosen radius is timelike, and $dt$ is timelike at every point with $r\geq R$ because this entire region lies beyond the common threshold. Finally $qR=R_0q^{1/3}\to0$ and $R^{-1}\to0$ as $q\downarrow0$. Applying the uniform area formula in [F3] gives $|C_q|_{g_q}\to4\pi$. [F1, F3, step 1.1, step 2.1, algebra] ∎

## Source notes

The article reference attributes Proposition 4.1, which defines the spheres in the original end coordinates and asserts that their stationary projections surround $S$. Intrinsic enclosure here follows from the existing compact-truncation supplier. The coordinate definition and uniform-estimate suppliers give the other conclusions; the proposition is not used as a premise.

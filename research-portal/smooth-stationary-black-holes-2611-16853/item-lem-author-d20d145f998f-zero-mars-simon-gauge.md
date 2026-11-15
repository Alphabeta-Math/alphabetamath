---
title: Normalized Ernst data and zero Mars–Simon survive stationary gauges
status: published
research_item: lem-author-d20d145f998f-zero-mars-simon-gauge
dependency_level: 2
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)
- [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)
- [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)
- [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)


## Statement

On a connected Lorentzian four-dimensional domain $U$ carrying the stationary Lorentzian data and conventions of the Ernst interface, including an orientation and a fixed time orientation, let two smooth Ernst potentials $\sigma,\sigma'$ satisfy $d\sigma=d\sigma'=2\iota_T\mathcal F$ for the same geometric Killing field $T$, metric, orientation and curvature convention. Suppose both tend to one on the same supplied parametrized end, in the sense of the Ernst interface. Then $\sigma=\sigma'$. A passive stationary-coordinate change means a change of coordinates on this same domain representing the same geometric data, including $T$, the time orientation and the end; it does not rescale $T$ or change the orientation.

Fix a real constant $M$ (the mass parameter in applications). On $N=\{p\in U:1-\sigma(p)\ne0\}$ define $P=(1-\sigma)^{-1}$, $y=\operatorname{Re}P$, $z=\operatorname{Im}P$, $|Dz|_g^2:=g^{-1}(dz,dz)=g^{ab}(\partial_a z)(\partial_b z)$, and $B:=z^2+4M^2(y^2+z^2)|Dz|_g^2$. The contraction uses the spacetime inverse Lorentzian metric, without conjugation; the notation $|Dz|_g^2$ does not assert positivity. These are smooth scalar fields on $N$. Passive stationary-coordinate changes leave $\mathcal F^2$ on $U$ and $y,z,B$ on $N$ unchanged, at the same geometric points and with the same $M$.

For precision, let $S=s(\mathbb S^2)\subset U$ for any fixed smooth embedding $s$, where $\mathbb S^2=\{x\in\mathbb R^3:\sum_{j=1}^3(x^j)^2=1\}$ has its usual smooth structure. The sphere scalar conditions meant here are $-4M^2\mathcal F^2=(1-\sigma)^4$ at every point of $S$, and $y(p)>1/2$ for at least one $p\in S\cap N$. Each condition, whenever satisfied, remains satisfied after a passive stationary-coordinate change. This assertion does not require that all of $S$ lie in $N$.

If the Mars–Simon tensor $\mathcal S$ in the same convention vanishes throughout $N$, then $|(1-\sigma)\mathcal S(T,E_\alpha,E_\beta,E_\gamma)|=0$ in every frame on $N$; in particular every positive perturbative-smallness threshold for this expression is satisfied there. This includes the case $N=U$ and $\mathcal S=0$ throughout $U$. The lemma establishes neither tensor vanishing, constancy or a bound for $B$, nor the other hypotheses of a global rigidity theorem.

## Statement references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

## Facts & Assumptions

[F1] The normalized Ernst differential, the supplied end limit, the Killing form and the Mars–Simon convention are those of the Ernst interface. [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)

[F2] The geometric Killing field is fixed under the passive coordinate changes in the Statement. [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[F3] The inverse metric is a bilinear form on covectors, with components $g^{ab}$ in the coordinate covector basis. This defines the contraction used in $B$. [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[F4] The sphere in the Statement is the image of a fixed smooth embedding of the usual unit two-sphere; changing coordinates does not change this map or its image as geometric data. [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

[F5] The stationary Lorentzian data on $U$ include a fixed time orientation, so the Killing-field and inverse-metric interfaces in [F2] and [F3] apply. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Prove uniqueness, the specified scalar invariances and the conditional zero-component assertion.

1.1 Put $h=\sigma-\sigma'$. The defining equations give $dh=0$. In a coordinate ball, integrate the derivative of $h$ along each straight coordinate segment from its center: that derivative is zero, so $h$ is constant on the ball. Thus $h$ is locally constant; on connected $U$ the nonempty level set through any point is both open and closed, and hence is all of $U$. Both potentials tend to one on the same supplied end, so their constant difference tends to zero and is zero. [F1, given]

2.1 In a passive coordinate change the metric, geometric orientation, time orientation and field $T$ remain fixed. The metric connection, its Killing form, the oriented Hodge dual and their contractions in the Ernst interface therefore represent the same geometric tensors. In particular $\mathcal F^2$ is the same complex scalar. Together with step 1.1 this identifies the same $\sigma$ and the same locus $N$ in both descriptions. The reciprocal has a smooth nonzero denominator on $N$, so $P$, its real and imaginary parts $y,z$, and their differentials are smooth and have the same geometric values there. [F1, F2, F5, step 1.1]

3.1 Evaluate the inverse-metric bilinear form of [F3] on the same covector $dz$ twice. In coordinate components this is exactly $g^{ab}(\partial_a z)(\partial_b z)$; under a coordinate change the inverse Jacobians in the two covector components cancel the Jacobians in the inverse-metric components. Hence this contraction and the explicitly defined $B$ are smooth invariant scalars on $N$, with no sign or constancy asserted. For the fixed sphere image of [F4], the scalars on both sides of $-4M^2\mathcal F^2=(1-\sigma)^4$ have identical values at every point of $S$ in either description. Likewise any witness $p\in S\cap N$ to $y(p)>1/2$ remains the same witness. This proves precisely the two conditional sphere assertions. [F1, F3, F4, step 2.1]

4.1 If $\mathcal S=0$ on $N$, evaluation on $T$ and any three frame vectors gives zero by multilinearity at every point of $N$. Multiplication by the smooth scalar $1-\sigma$ and taking the complex absolute value still give zero. Consequently every positive smallness threshold is satisfied by this expression in every frame on $N$, including on all of $U$ when $N=U$. This conditional argument supplies no vanishing theorem or additional rigidity hypotheses. [F1, F2, step 2.1] ∎

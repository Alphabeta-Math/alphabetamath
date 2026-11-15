---
title: Zero stationary energy along null geodesics
status: published
research_item: lem-author-ad064c44a1cc-zero-stationary-energy
dependency_level: 1
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [math:def-geodesic-of-an-affine-connection](https://alphabetamath.cc/item/def-geodesic-of-an-affine-connection)
- [physics:thm-gr-killing-and-on-shell-matter-identities](https://alphabetamath.cc/physics/item/thm-gr-killing-and-on-shell-matter-identities)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [physics:lem-gr-future-causal-classification-by-a-timelike-field](https://alphabetamath.cc/physics/item/lem-gr-future-causal-classification-by-a-timelike-field)


## Statement

Let $T$ be Killing for a smooth time-oriented Lorentzian metric, and let $\gamma:I\to E$ be a nonconstant affinely parametrized null geodesic in an open exterior $E$. Its stationary energy $\mathfrak e=-g(T,\dot\gamma)$ is constant. Its zero-energy condition $g(T,\dot\gamma)=0$ is unchanged by any smooth regular reparametrization of its image. In particular zero energy is a property of the unparametrized geodesic. A timelike $T$ at a point excludes any nonzero null vector orthogonal to it; thus a zero-energy null geodesic lies where $T$ is spacelike, null or zero, not in its timelike region.

Use the four-dimensional signature $(-,+,+,+)$ conventions of stationary Lorentzian data. Here an affinely parametrized null geodesic means a smooth curve on an interval $I$ with nonempty interior satisfying $D_s\dot\gamma=0$, $\dot\gamma(s)\ne0$ and $g_{\gamma(s)}(\dot\gamma(s),\dot\gamma(s))=0$ for every $s\in I$, including any included endpoints with the one-sided derivative convention. A smooth regular reparametrization is $\widetilde\gamma=\gamma\circ s$, where $s:J\to I$ is a bijective smooth map of intervals with smooth inverse and $s'(u)\ne0$ everywhere; smoothness and derivatives at any included endpoints use smooth extensions and one-sided restrictions. Both increasing and decreasing changes are allowed. An unparametrized geodesic here is an equivalence class of regular parametrized curves (smooth curves with nowhere-zero velocity) under these changes, with at least one affinely parametrized geodesic representative; its other representatives need not be affinely parametrized. Equality of bare image sets is not the equivalence relation.

## Facts & Assumptions

[F1] [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) supplies the smooth Lorentzian metric, signature, time-orientation field $N$ and metric-compatible connection. [math:def-geodesic-of-an-affine-connection](https://alphabetamath.cc/item/def-geodesic-of-an-affine-connection) defines affine geodesics by $D_s\dot\gamma=0$.

[F2] [physics:thm-gr-killing-and-on-shell-matter-identities](https://alphabetamath.cc/physics/item/thm-gr-killing-and-on-shell-matter-identities), clauses (a) and (b), gives the Killing equation $\nabla_aT_b+\nabla_bT_a=0$ and conservation of the metric contraction along affine geodesics. Only these mathematical clauses are used.

[F3] The Lorentzian interface imported by [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) defines timelike, spacelike and null vectors; null vectors are nonzero and have zero squared norm. These pointwise conventions distinguish the zero vector from all three causal characters. The null-geodesic convention specified locally in the Statement combines this pointwise null condition with the affine-geodesic definition in [F1].

[F4] [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) applies to the smooth coordinate maps of the curve composed with a smooth parameter change.

[F5] [physics:lem-gr-future-causal-classification-by-a-timelike-field](https://alphabetamath.cc/physics/item/lem-gr-future-causal-classification-by-a-timelike-field), clause 1, says that the orthogonal complement of the smooth timelike time-orientation field in a time-oriented Lorentzian four-manifold is positive definite. The field in that result may be any smooth timelike field on the domain where it is applied.

## Proof

**Given:** The stated metric, Killing field and nonconstant affinely parametrized null geodesic, with the parameter-change conventions in the Statement.

**Goal:** Show energy conservation, parameter independence at zero energy and the location restriction.

1.1 Metric compatibility and the geodesic equation give $\frac{d}{ds}g(T,\dot\gamma)=g(\nabla_{\dot\gamma}T,\dot\gamma)+g(T,D_s\dot\gamma)=\tfrac12\dot\gamma^a\dot\gamma^b(\nabla_aT_b+\nabla_bT_a)=0$. Thus the signed energy is constant on the interval, also directly by clause (b) of [F2]. [F1, F2, given, algebra]

1.2 For a permitted change $s:J\to I$, apply [F4] in a chart around $\gamma(s(u))$ to obtain $\frac{d}{du}(\gamma\circ s)(u)=s'(u)\dot\gamma(s(u))$. Bilinearity gives $g(T,\widetilde\gamma'(u))=s'(u)g(T,\dot\gamma(s(u)))$. Since $s'(u)\ne0$ and $s$ is onto, the contraction vanishes along one representative exactly when it vanishes along the other. The new velocity remains nonzero and null, since its squared norm is $s'(u)^2g(\dot\gamma,\dot\gamma)=0$. These identities extend to included endpoints by the one-sided conventions. Thus zero energy is a property of the specified equivalence class. Constancy itself was asserted only for affine parameters. [F3, F4, given, algebra]

2.1 The timelike region $U=\{p\in E:g_p(T_p,T_p)<0\}$ is open by smoothness. On $U$, the restricted field $T|_U$ is itself a smooth time orientation, so apply [F5] to $(U,g|_U,T|_U)$. It gives positive definiteness of $g_p$ on $T_p^{\perp}=\{v:g_p(v,T_p)=0\}$ for every $p\in U$. Consequently every nonzero vector orthogonal to timelike $T_p$ has positive squared norm and cannot be null by [F3]. The velocity of the stated null geodesic is nonzero at every point by the null convention. Hence a zero-energy null geodesic never meets $U$. Every remaining value of $T$ is spacelike, null or zero by [F3], which proves the location restriction together with the energy conclusions already obtained. [F1, F3, F5, given, step 1.1, step 1.2, algebra] ∎

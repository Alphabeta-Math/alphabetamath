---
title: Stationary exact corrections preserve two prescribed gauges
status: published
research_item: lem-author-9e1b6fa65528-stationary-exact-gluing
dependency_level: 1
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [math:def-smooth-partition-of-unity-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-partition-of-unity-on-a-manifold-with-boundary)
- [math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:def-smooth-differential-k-form](https://alphabetamath.cc/item/def-smooth-differential-k-form)
- [math:def-lie-derivative-of-a-differential-form](https://alphabetamath.cc/item/def-lie-derivative-of-a-differential-form)
- [math:def-closed-and-exact-differential-forms](https://alphabetamath.cc/item/def-closed-and-exact-differential-forms)
- [math:prop-exterior-derivative-of-a-function-is-its-differential](https://alphabetamath.cc/item/prop-exterior-derivative-of-a-function-is-its-differential)
- [math:thm-the-exterior-derivative-squares-to-zero](https://alphabetamath.cc/item/thm-the-exterior-derivative-squares-to-zero)
- [math:prop-the-exterior-derivative-is-local](https://alphabetamath.cc/item/prop-the-exterior-derivative-is-local)
- [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)
- [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)
- [math:ex-the-n-sphere-with-its-standard-smooth-atlas](https://alphabetamath.cc/item/ex-the-n-sphere-with-its-standard-smooth-atlas)
- [math:prop-a-vector-field-acts-as-a-derivation-of-smooth-functions](https://alphabetamath.cc/item/prop-a-vector-field-acts-as-a-derivation-of-smooth-functions)
- [math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure](https://alphabetamath.cc/item/prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure)


## Statement

Let $(M,g,T)$ be stationary Lorentzian data and let $E\subset M$ be open, equipped with the restricted smooth charts of $M$. Only the smooth manifold and field $T$ enter the construction. A stationary region in $E$ means an open subset invariant under the local flow of $T|_E$ wherever that flow is defined. A smooth differential form $\alpha$ is stationary when $\mathcal L_T\alpha=0$, and a smooth function $h$ is stationary when $Th=0$. Closed and exact mean respectively $d\alpha=0$ and $\alpha=d\beta$ for a smooth form $\beta$ of one lower degree.

On $E$ let $\Theta$ be a smooth closed two-form, $D$ a smooth function, $c\in\mathbb R$, and $V$ a smooth stationary one-form with $dV=\Theta$ and $V(T)+D=c$. For $j\in\{H,\infty\}$ let $U_j\subset E$ be disjoint stationary regions, and let $V_j$ be smooth stationary one-forms on $U_j$ with $dV_j=\Theta|_{U_j}$ and $V_j(T)+D=c$. Assume that every smooth closed one-form on each $U_j$ is exact. Supply smooth stationary functions $\eta_j:E\to[0,1]$ with $\operatorname{supp}_E\eta_j\subset U_j$ and $\eta_j=1$ on prescribed open subsets $P_j\subset U_j$, where $\operatorname{supp}_E\eta_j$ is the closure in $E$ of $\{\eta_j\ne0\}$. Then there exist smooth stationary functions $h_H,h_\infty$ on $E$ such that $W=V+dh_H+dh_\infty$ is stationary, $dW=\Theta$, $W(T)+D=c$, and $W|_{P_j}=V_j|_{P_j}$. Thus the corrections are globally exact stationary one-forms and both prescribed gauges are retained.

For the boundary-extension conclusion, let $S\subset\partial_M E$ be a smooth embedded two-sphere in $M$, with $\partial_M E$ the topological boundary. Suppose there is an open neighborhood $O\subset M$ of $S$ with $O\cap E\subset P_H$ and a smooth one-form $\overline V_H$ on $O$ agreeing with $V_H$ on $O\cap E$. Then $W$ extends smoothly to $E\cup O$ by $\overline V_H$ on $O$. Every specified local symmetry $\mathcal L_X\overline V_H=0$ for a smooth field $X$ on $O$ is inherited by the extension on $O$. This includes stationarity on $O$ if $X=T|_O$ is among these fields; no symmetry in the cutoff transition regions is asserted.

## Facts & Assumptions

[F1] The stationary Lorentzian interface supplies the ambient smooth manifold $M$ and smooth field $T$. Open subsets carry canonical restricted smooth structures, independently of the presenting atlas; these are used for $E$, $U_j$, $P_j$, $O$, $O\cap E$ and $E\cup O$. Regions use the local-flow convention, without a completeness assumption. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure](https://alphabetamath.cc/item/prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F2] Smooth forms and their Lie derivatives have the usual alternating-tensor meanings; stationarity of forms is explicitly defined in the Statement by vanishing Lie derivative. [math:def-smooth-differential-k-form](https://alphabetamath.cc/item/def-smooth-differential-k-form) [math:def-lie-derivative-of-a-differential-form](https://alphabetamath.cc/item/def-lie-derivative-of-a-differential-form)

[F3] Closed means exterior derivative zero and exact means an exterior derivative of a smooth form. Exactness of every closed one-form on each $U_j$ is an explicit hypothesis, not inferred from stationarity. [math:def-closed-and-exact-differential-forms](https://alphabetamath.cc/item/def-closed-and-exact-differential-forms)

[F4] Support is the closure of the nonzero locus, as in the smooth partition-of-unity convention. The supplied cutoffs are required to be stationary; neither their existence nor this extra property is deduced from a partition-of-unity definition. [math:def-smooth-partition-of-unity-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-partition-of-unity-on-a-manifold-with-boundary) [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

[F5] For a smooth scalar $a$ and field $Y$, $da(Y)=Ya$. [math:prop-exterior-derivative-of-a-function-is-its-differential](https://alphabetamath.cc/item/prop-exterior-derivative-of-a-function-is-its-differential)

[F6] The exterior derivative is local and satisfies $d^2=0$. [math:prop-the-exterior-derivative-is-local](https://alphabetamath.cc/item/prop-the-exterior-derivative-is-local) [math:thm-the-exterior-derivative-squares-to-zero](https://alphabetamath.cc/item/thm-the-exterior-derivative-squares-to-zero)

[F7] Cartan's formula is $\mathcal L_Y\alpha=d(\iota_Y\alpha)+\iota_Y(d\alpha)$. [math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula)

[F8] The boundary in the extension clause is the topological boundary in $M$, and $S$ is an embedded smooth submanifold that is a two-sphere with its usual smooth structure. These hypotheses do not identify all of $\partial_M E$ with $S$ or assert that $E\cup S$ is a manifold with boundary. [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top) [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart) [math:ex-the-n-sphere-with-its-standard-smooth-atlas](https://alphabetamath.cc/item/ex-the-n-sphere-with-its-standard-smooth-atlas)

[F9] A smooth vector field $X$ acts on smooth functions by the product rule $X(ab)=aXb+bXa$. [math:prop-a-vector-field-acts-as-a-derivation-of-smooth-functions](https://alphabetamath.cc/item/prop-a-vector-field-acts-as-a-derivation-of-smooth-functions)

## Proof

**Given:** The smooth data, exactness assumptions, cutoffs and, for the last conclusion, the ambient neighborhood and extension in the Statement.

**Goal:** Construct the exact corrections, retain both gauges and normalization, and glue the asserted local extension.

1.1 For each $j\in\{H,\infty\}$, the one-form $V_j-V|_{U_j}$ is closed because its exterior derivative is $\Theta|_{U_j}-\Theta|_{U_j}=0$. Exactness on $U_j$ supplies a smooth scalar $\chi_j$ with $d\chi_j=V_j-V|_{U_j}$. The equal contraction constants give $T\chi_j=d\chi_j(T)=V_j(T)-V(T)=0$ on $U_j$. This requires no choice of a normalization for $\chi_j$ and no completeness of $T$. [given, F1, F3, F5]

2.1 Define $h_j=\eta_j\chi_j$ on $U_j$ and $h_j=0$ on $E\setminus U_j$. Every point of $E\setminus U_j$ lies outside the closed set $\operatorname{supp}_E\eta_j$, so it has an open neighborhood in $E$ on which $\eta_j=0$. On that neighborhood the two definitions of $h_j$ agree identically with zero, proving smoothness across the edge of $U_j$. On $U_j$, the directional product rule gives $Th_j=(T\eta_j)\chi_j+\eta_jT\chi_j=0$; elsewhere it follows from the same local zero description. Thus $dh_j(T)=0$ globally. Also $d(dh_j)=0$, and Cartan's formula yields $\mathcal L_T(dh_j)=d(dh_j(T))+\iota_Td(dh_j)=0$. Hence each correction is exact and stationary. [given, F1, F2, F4, F5, F6, F7, F9, step 1.1]

3.1 Put $W=V+dh_H+dh_\infty$. By step 2.1 it is smooth and stationary, $dW=dV=\Theta$, and $W(T)+D=V(T)+D=c$. On $P_j$ the function $h_j$ equals $\chi_j$ on an open set, so locality gives $dh_j=d\chi_j$ there. The other correction vanishes on $U_j$, since its support lies in the disjoint region. Consequently $W=V+d\chi_j=V_j$ on $P_j$. This proves both prescribed gauge identities without altering the normalization. [given, F1, F2, F4, F6, step 1.1, step 2.1]

4.1 In the boundary-extension setting, $O\cap E\subset P_H$, so step 3.1 gives $W=V_H=\overline V_H$ on the entire open overlap $O\cap E$. Define $\widetilde W=W$ on $E$ and $\widetilde W=\overline V_H$ on $O$. The overlap equality makes this well-defined. Every point has an open neighborhood on which it is one of these smooth forms, so it is smooth on $E\cup O$. On $O$ it is exactly $\overline V_H$, and therefore has every stipulated symmetry $\mathcal L_X\overline V_H=0$ there. This proves the extension and symmetry conclusion on an actual neighborhood of the sphere. [given, F1, F2, F8, step 3.1] ∎

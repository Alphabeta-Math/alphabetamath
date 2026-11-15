---
title: Compact timelike-length bounds restrict to open subdomains
status: published
research_item: lem-author-89004136b63c-compact-length-restriction
dependency_level: 0
---

## Prerequisites

- [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)
- [math:def-derivation-at-a-point-and-tangent-space](https://alphabetamath.cc/item/def-derivation-at-a-point-and-tangent-space)
- [math:thm-coordinate-derivations-form-a-basis-of-the-tangent-space](https://alphabetamath.cc/item/thm-coordinate-derivations-form-a-basis-of-the-tangent-space)
- [math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map)
- [math:thm-coordinate-formula-for-the-differential](https://alphabetamath.cc/item/thm-coordinate-formula-for-the-differential)
- [math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space)
- [math:def-ck-and-multi-index-notation-in-several-variables](https://alphabetamath.cc/item/def-ck-and-multi-index-notation-in-several-variables)
- [physics:def-lorentz-form-and-inertia](https://alphabetamath.cc/physics/item/def-lorentz-form-and-inertia)
- [physics:def-causal-classification-of-lorentz-vectors](https://alphabetamath.cc/physics/item/def-causal-classification-of-lorentz-vectors)
- [physics:def-time-orientation-and-future-causal-sets](https://alphabetamath.cc/physics/item/def-time-orientation-and-future-causal-sets)
- [physics:lem-lorentz-form-has-orthonormal-basis](https://alphabetamath.cc/physics/item/lem-lorentz-form-has-orthonormal-basis)
- [physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components)
- [math:thm-cauchy-schwarz-finite](https://alphabetamath.cc/item/thm-cauchy-schwarz-finite)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction)
- [math:def-nonnegative-lebesgue-integral](https://alphabetamath.cc/item/def-nonnegative-lebesgue-integral)
- [math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure](https://alphabetamath.cc/item/prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:thm-lebesgue-measure-is-a-complete-measure](https://alphabetamath.cc/item/thm-lebesgue-measure-is-a-complete-measure)
- [math:thm-borel-sets-are-lebesgue-measurable](https://alphabetamath.cc/item/thm-borel-sets-are-lebesgue-measurable)
- [math:thm-continuous-preimages-of-borel-sets-are-borel](https://alphabetamath.cc/item/thm-continuous-preimages-of-borel-sets-are-borel)
- [math:thm-sequential-suprema-infima-limsup-liminf-and-pointwise-limits-are-measurable](https://alphabetamath.cc/item/thm-sequential-suprema-infima-limsup-liminf-and-pointwise-limits-are-measurable)
- [math:thm-coordinatewise-measurability-into-r-n](https://alphabetamath.cc/item/thm-coordinatewise-measurability-into-r-n)
- [math:thm-composition-with-borel-functions-preserves-measurability](https://alphabetamath.cc/item/thm-composition-with-borel-functions-preserves-measurability)
- [math:def-measure-null-set-and-almost-everywhere](https://alphabetamath.cc/item/def-measure-null-set-and-almost-everywhere)
- [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)
- [math:cor-integral-over-a-null-set-vanishes](https://alphabetamath.cc/item/cor-integral-over-a-null-set-vanishes)
- [math:lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets](https://alphabetamath.cc/item/lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)


## Statement

Assume countable choice for the usual Lebesgue-measure convention. Let $g$ be a $C^2$ Lorentz metric on an open subset $B$ of a smooth four-manifold and let $N$ be a continuous timelike time-orientation field. Here $T_pB$ is the derivation tangent space. A $C^2$ Lorentz metric means an assignment of symmetric nondegenerate bilinear forms $g_p:T_pB\times T_pB\to\mathbb R$ of signature $(-,+,+,+)$ whose coefficients $g_{ij}=g(\partial_{x^i},\partial_{x^j})$ are $C^2$ in every smooth chart. A continuous timelike orientation field means an assignment $N_p\in T_pB$ with continuous coordinate components and $g_p(N_p,N_p)<0$. At each point it selects the timelike component containing $N_p$; future-directed nonzero causal vectors are the nonzero vectors in the closure of that component, equivalently $g_p(v,v)\le0$ and $g_p(v,N_p)<0$. The pointwise equivalence and its applicability to these regularities are justified below. For a continuous curve $c:[a,b]\to B$, at an interior time $t$ where a coordinate representative $x\circ c$ is differentiable, define its velocity by $\dot c(t)=\sum_{i=1}^4(x^i\circ c)^{\prime}(t)\,\partial_{x^i}|_{c(t)}\in T_{c(t)}B$. Both existence at that time and this vector are independent of the smooth chart, as proved below. In this item a future Lipschitz curve is a continuous curve $c:[a,b]\to B$, locally Lipschitz in coordinates, with nonzero future-directed velocity almost everywhere. For such a curve uniformly timelike in its chosen parameter, meaning $g(\dot c,\dot c)\le-\epsilon_c<0$ almost everywhere for one constant $\epsilon_c>0$, define $L_g(c)=\int_a^b\sqrt{-g(\dot c,\dot c)}\,dt$ using the nonnegative Lebesgue integral, with integrand zero on a measurable null set containing the exceptional times and the parameter endpoints. The value is independent of this null-set choice. Suppose each compact $C\subset B$ has a finite constant $L_C$ bounding $L_g(c)$ for all such curves with image in $C$. Every open $W\subset B$ inherits precisely the same property, with $g,N$ restricted to $W$. The constants are uniform over curves in each compact set, while $\epsilon_c$ may depend on the curve.

## Statement references

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:def-derivation-at-a-point-and-tangent-space](https://alphabetamath.cc/item/def-derivation-at-a-point-and-tangent-space)

[math:thm-coordinate-derivations-form-a-basis-of-the-tangent-space](https://alphabetamath.cc/item/thm-coordinate-derivations-form-a-basis-of-the-tangent-space)

[math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map)

[math:thm-coordinate-formula-for-the-differential](https://alphabetamath.cc/item/thm-coordinate-formula-for-the-differential)

[math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space)

[math:def-ck-and-multi-index-notation-in-several-variables](https://alphabetamath.cc/item/def-ck-and-multi-index-notation-in-several-variables)

[physics:def-lorentz-form-and-inertia](https://alphabetamath.cc/physics/item/def-lorentz-form-and-inertia)

[physics:def-causal-classification-of-lorentz-vectors](https://alphabetamath.cc/physics/item/def-causal-classification-of-lorentz-vectors)

[physics:def-time-orientation-and-future-causal-sets](https://alphabetamath.cc/physics/item/def-time-orientation-and-future-causal-sets)

[physics:lem-lorentz-form-has-orthonormal-basis](https://alphabetamath.cc/physics/item/lem-lorentz-form-has-orthonormal-basis)

[physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components)

[math:thm-cauchy-schwarz-finite](https://alphabetamath.cc/item/thm-cauchy-schwarz-finite)

[math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction)

[math:def-nonnegative-lebesgue-integral](https://alphabetamath.cc/item/def-nonnegative-lebesgue-integral)

[math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure](https://alphabetamath.cc/item/prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:thm-lebesgue-measure-is-a-complete-measure](https://alphabetamath.cc/item/thm-lebesgue-measure-is-a-complete-measure)

[math:thm-borel-sets-are-lebesgue-measurable](https://alphabetamath.cc/item/thm-borel-sets-are-lebesgue-measurable)

[math:thm-continuous-preimages-of-borel-sets-are-borel](https://alphabetamath.cc/item/thm-continuous-preimages-of-borel-sets-are-borel)

[math:thm-sequential-suprema-infima-limsup-liminf-and-pointwise-limits-are-measurable](https://alphabetamath.cc/item/thm-sequential-suprema-infima-limsup-liminf-and-pointwise-limits-are-measurable)

[math:thm-coordinatewise-measurability-into-r-n](https://alphabetamath.cc/item/thm-coordinatewise-measurability-into-r-n)

[math:thm-composition-with-borel-functions-preserves-measurability](https://alphabetamath.cc/item/thm-composition-with-borel-functions-preserves-measurability)

[math:def-measure-null-set-and-almost-everywhere](https://alphabetamath.cc/item/def-measure-null-set-and-almost-everywhere)

[math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)

[math:cor-integral-over-a-null-set-vanishes](https://alphabetamath.cc/item/cor-integral-over-a-null-set-vanishes)

[math:lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets](https://alphabetamath.cc/item/lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets)

[math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

## Facts & Assumptions

[F1] At each point the metric is a Lorentz form, timelike means $g_p(v,v)<0$, and causal means nonzero with $g_p(v,v)\le0$. A pointwise time orientation chooses a component of the timelike set; future causal vectors are the nonzero vectors in its closure. Here the chosen component contains $N_p$. These are definitions on a four-dimensional real vector space, with no smooth-field hypothesis. [physics:def-lorentz-form-and-inertia](https://alphabetamath.cc/physics/item/def-lorentz-form-and-inertia) [physics:def-causal-classification-of-lorentz-vectors](https://alphabetamath.cc/physics/item/def-causal-classification-of-lorentz-vectors) [physics:def-time-orientation-and-future-causal-sets](https://alphabetamath.cc/physics/item/def-time-orientation-and-future-causal-sets)

[F2] Compactness is intrinsic to the subspace topology. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[F3] Lipschitz continuity means a uniform distance-ratio bound in coordinates. The nonnegative integral is the supremum of the integrals of nonnegative simple minorants of a measurable integrand. [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction) [math:def-nonnegative-lebesgue-integral](https://alphabetamath.cc/item/def-nonnegative-lebesgue-integral)

[F4] An open subset carries the canonical smooth structure generated by restricted charts, independent of the presenting atlas. Apply this first to $B$ in the given four-manifold, and then to $W$ in $B$. [math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure](https://alphabetamath.cc/item/prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure)

[F5] Countable choice is assumed only for the standard Lebesgue-measure suppliers: Lebesgue measure is a complete measure and all Borel sets are Lebesgue measurable. These results apply in dimension one to the parameter variable. Restricting the measure and sigma-algebra to $[a,b]$ preserves these properties. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) [math:thm-lebesgue-measure-is-a-complete-measure](https://alphabetamath.cc/item/thm-lebesgue-measure-is-a-complete-measure) [math:thm-borel-sets-are-lebesgue-measurable](https://alphabetamath.cc/item/thm-borel-sets-are-lebesgue-measurable)

[F6] Continuous maps have Borel preimages of Borel sets. Sequential limsups of measurable functions are measurable. A finite-dimensional real map is measurable exactly when its coordinates are measurable, and composition of measurable maps is measurable. [math:thm-continuous-preimages-of-borel-sets-are-borel](https://alphabetamath.cc/item/thm-continuous-preimages-of-borel-sets-are-borel) [math:thm-sequential-suprema-infima-limsup-liminf-and-pointwise-limits-are-measurable](https://alphabetamath.cc/item/thm-sequential-suprema-infima-limsup-liminf-and-pointwise-limits-are-measurable) [math:thm-coordinatewise-measurability-into-r-n](https://alphabetamath.cc/item/thm-coordinatewise-measurability-into-r-n) [math:thm-composition-with-borel-functions-preserves-measurability](https://alphabetamath.cc/item/thm-composition-with-borel-functions-preserves-measurability)

[F7] An almost-everywhere condition holds outside a measurable null set containing all its exceptional points. In the curve class here, existence of the nonzero future-directed velocity almost everywhere is already required. [math:def-measure-null-set-and-almost-everywhere](https://alphabetamath.cc/item/def-measure-null-set-and-almost-everywhere)

[F8] The closed bounded parameter interval is compact and every open cover of it has a finite subcover. [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)

[F9] A nonnegative measurable function integrated over a measurable null set has integral zero. [math:cor-integral-over-a-null-set-vanishes](https://alphabetamath.cc/item/cor-integral-over-a-null-set-vanishes)

[F10] A $C^1$ map is locally Lipschitz in coordinates near a compact coordinate subset; for a chart transition one may take the compact set to be a singleton in the overlap. The total-derivative chain rule applies at each parameter where the coordinate curve is differentiable. [math:lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets](https://alphabetamath.cc/item/lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F11] A smooth manifold has a maximal smooth atlas, its tangent space consists of derivations at a point, and the coordinate derivations form a basis. A type $(0,2)$ tensor at a point is a bilinear map on that tangent space. In this item the metric's $C^2$ regularity and the field's continuity mean exactly the coordinate conditions in the Statement; $C^2$ coefficients have continuous iterated partial derivatives through order two. No smoothness of either field is assumed. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:def-derivation-at-a-point-and-tangent-space](https://alphabetamath.cc/item/def-derivation-at-a-point-and-tangent-space) [math:thm-coordinate-derivations-form-a-basis-of-the-tangent-space](https://alphabetamath.cc/item/thm-coordinate-derivations-form-a-basis-of-the-tangent-space) [math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space) [math:def-ck-and-multi-index-notation-in-several-variables](https://alphabetamath.cc/item/def-ck-and-multi-index-notation-in-several-variables)

[F12] The differential of a smooth map acts on derivations by precomposing germs, and its matrix in coordinate tangent bases is the Jacobian of its coordinate representative. These facts concern smooth maps of the underlying smooth manifolds, independently of metric regularity. [math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map) [math:thm-coordinate-formula-for-the-differential](https://alphabetamath.cc/item/thm-coordinate-formula-for-the-differential)

[F13] Every four-dimensional Lorentz form has an orthonormal basis. In such a basis the two timelike components are $v^0>|v_s|$ and $v^0<-|v_s|$, with closures $v^0\ge|v_s|$ and $v^0\le-|v_s|$; here $|v_s|=\sqrt{\sum_{i=1}^3(v^i)^2}$. These component and closure descriptions are independent of the orthonormal basis. The finite Cauchy-Schwarz inequality gives $|\sum_{i=1}^3 u^iv^i|\le|u_s||v_s|$. [physics:lem-lorentz-form-has-orthonormal-basis](https://alphabetamath.cc/physics/item/lem-lorentz-form-has-orthonormal-basis) [physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components) [math:thm-cauchy-schwarz-finite](https://alphabetamath.cc/item/thm-cauchy-schwarz-finite)

## Proof

**Given:** The hypotheses in the Statement, including countable choice for the Lebesgue-measure convention.

**Goal:** Establish the measurable length convention and the asserted restriction property.

1.1 Use [F11] and [F4] to equip $B$ and $W$ with their restricted smooth structures. A chart of the ambient manifold restricts first to $B$ and then to $W$; the resulting coordinate functions and transition maps are unchanged wherever defined. For the inclusion $W\hookrightarrow B$ the coordinate map is the identity on an open set, so its tangent map is the identity in these coordinates by [F12]. Consequently the restrictions of $g$ and $N$ have the same coefficient functions, signature, regularity and time orientation. This supplies the smooth-manifold and tangent identifications used below. [F4, F11, F12]

1.2 Fix $p$ and apply [F13] to the four-dimensional space $T_pB$ of [F11]. In an orthonormal basis write $N_p=(n^0,n_s)$, reversing the time basis vector if necessary so that $n^0>|n_s|$. The component containing $N_p$ is then $T_+$ of [F13]. If $v\in\operatorname{cl}(T_+)\setminus\{0\}$, then $v^0\ge|v_s|$ and $v^0>0$, so $g_p(v,N_p)=-v^0n^0+\sum_{i=1}^3v^in^i\le-v^0(n^0-|n_s|)<0$ by the finite Cauchy-Schwarz inequality in [F13]. On $\operatorname{cl}(T_-)\setminus\{0\}$ the pairing is positive by applying this calculation to $-v$. Every nonzero causal vector is in exactly one of those two closed cones by [F1] and [F13], proving the equivalence asserted in the Statement. All pairings are intrinsic evaluations of bilinear forms. Their coordinate expressions vary continuously with $p$ and the vector components because $g$ and $N$ have continuous coefficients. Thus the strict future inequality defines an open condition, restricted to the causal vectors, at precisely the stated regularities. The pointwise argument chooses a basis only at the fixed point; no field of bases, smooth orientation field, or stronger choice principle is used. [given, F1, F11, F13, algebra]

1.3 Let $t\in(a,b)$, put $p=c(t)$, and suppose $y\circ c$ is differentiable at $t$ in one smooth chart $y$ about $p$. For any other smooth chart $x$ about $p$, continuity of $c$ permits restriction to a parameter neighborhood whose image lies in the overlap. The transition $x\circ y^{-1}$ is smooth, so the Euclidean chain rule [F10] gives differentiability of $x\circ c$ at $t$ and $(x^i\circ c)^{\prime}(t)=\sum_{\alpha=1}^4 A^i_{\alpha}(y^{\alpha}\circ c)^{\prime}(t)$, where $A^i_{\alpha}=\partial(x^i\circ y^{-1})/\partial y^{\alpha}$ is evaluated at $y(p)$. Apply [F12] to the smooth identity map on the overlap, represented in these two charts, to obtain $\partial_{y^{\alpha}}|_p=\sum_i A^i_{\alpha}\partial_{x^i}|_p$. The coordinate basis in [F11] makes each proposed velocity a derivation in $T_pB$, and substitution gives $\sum_i(x^i\circ c)^{\prime}(t)\partial_{x^i}|_p=\sum_{\alpha}(y^{\alpha}\circ c)^{\prime}(t)\partial_{y^{\alpha}}|_p$. Interchanging the two charts proves equivalence of derivative existence as well as equality of the vectors. Thus the Statement defines an intrinsic velocity at every interior differentiability time. Here [F12] concerns the smooth identity map and [F10] concerns Euclidean maps differentiable at the one time under consideration. [given, F10, F11, F12, algebra]

1.4 Fix an eligible curve $c$. By local coordinate Lipschitz continuity, each parameter value has a relative open interval on which the image is in one chart and its coordinates satisfy one Lipschitz bound. Shrink such intervals to closed relative intervals $J_k$ whose relative interiors still cover $[a,b]$ and on each of which that chart and bound remain valid. By [F8] finitely many suffice. For each component $x^i$ of its coordinate curve on $J_k$, extend $x^i$ to $\mathbb R$ by keeping it constant beyond the two endpoints of $J_k$. The extension $\widetilde x^i$ is continuous and Lipschitz with the same bound. For integers $n\ge1$, the difference quotient $q_n^i(t)=n(\widetilde x^i(t+1/n)-\widetilde x^i(t))$ is continuous, hence Borel measurable by [F6], and Lebesgue measurable by [F5]. Its limsup $v_k^i$ is measurable by [F6] and finite everywhere because $|q_n^i|$ is bounded by that Lipschitz constant. At every interior parameter where $x^i$ is differentiable, $v_k^i=(x^i)'$. Choose a measurable null set $E$ containing the endpoints of these finitely many intervals and all exceptional times for the velocity and timelikeness conditions; such a set exists by [F7]. No differentiability theorem is being inferred from the Lipschitz definition: derivative existence almost everywhere is part of the stated curve class. The case $a=b$ has the zero integrand and zero integral. [given, F3, F5, F6, F7, F8]

2.1 On $J_k$, every coefficient $g_{ij}(c(t))$ in its chart is continuous, hence measurable by [F5] and [F6]. Combine these coefficients with the measurable finite coordinates $v_k^i$ into one measurable finite-dimensional map, using [F6]. The real function of these coefficients and coordinates given by $h_k(t)=\sqrt{\max\{0,-\sum_{i,j=1}^4g_{ij}(c(t))v_k^i(t)v_k^j(t)\}}$ is measurable: the map performing the displayed arithmetic, maximum and square root is continuous, so [F6] applies to its composition. Make a disjoint Borel partition by assigning each point to the first interval $J_k$ that contains it. Define $h=h_k$ on its assigned piece outside $E$ and $h=0$ on $E$. Each piece is measurable and there are finitely many, so preimages under this piecewise definition are finite unions of measurable sets. Thus $h$ is nonnegative measurable. Outside $E$, step 1.3 identifies the coordinate derivatives with the velocity defined in the Statement, and $g(\dot c,\dot c)<0$, so $h=\sqrt{-g(\dot c,\dot c)}$. For overlapping coordinates $x,y$, put $A^i_{\alpha}=\partial x^i/\partial y^{\alpha}$. By [F12] the coordinate tangent bases satisfy $\partial_{y^{\alpha}}=\sum_i A^i_{\alpha}\partial_{x^i}$. Bilinearity in [F11] gives $g^{(y)}_{\alpha\beta}=\sum_{i,j}A^i_{\alpha}A^j_{\beta}g^{(x)}_{ij}$. At each differentiability time outside $E$, the chain rule [F10] gives $\dot x^i=\sum_{\alpha}A^i_{\alpha}\dot y^{\alpha}$, hence $\sum_{\alpha,\beta}g^{(y)}_{\alpha\beta}\dot y^{\alpha}\dot y^{\beta}=\sum_{i,j}g^{(x)}_{ij}\dot x^i\dot x^j$. This derives the tensor transformation rule and the scalar's chart independence without differentiating $g$ or $N$. This establishes the claimed measurable length integrand with the stated null-set convention. [given, F5, F6, F7, F10, F11, F12, step 1.1, step 1.3, step 1.4]

3.1 Changing the chart intervals, their assignment, or the measurable exceptional null set gives another nonnegative measurable representative $h'$ equal to $h$ outside a measurable null set $Z$: take the union of the two exceptional sets and the finite interval endpoints. If $s$ is a nonnegative simple minorant of $h$, the function equal to $s$ off $Z$ and zero on $Z$ is a simple minorant of $h'$ with the same simple integral; its removed part is supported on $Z$ and has integral zero by [F9]. Taking the supremum over $s$ in [F3] gives $\int h\le\int h'$. Interchanging the representatives gives the reverse inequality. Hence the length is independent of all these auxiliary choices, including the measurable null set used for the zero values. [F3, F7, F9, step 2.1]

4.1 If $C\subset W$ is compact in $W$, the topology induced on $C$ from $W$ is the topology induced from $B$: both consist of the same iterated intersections of open sets with $C$. Thus $C$ is compact in $B$ by the intrinsic convention [F2]. The restricted atlas in step 1.1 gives exactly the same coordinate representatives of a curve into $C$ in either domain. Local coordinate Lipschitz continuity may be tested in this atlas: changing to any compatible chart composes with a smooth transition, which is locally Lipschitz by [F10]. The product of its local Lipschitz bound and that of the coordinate curve is a bound for the new coordinate representative. By step 1.2 the future condition is the pointwise pairing inequality at the given regularities. The velocity defined in the Statement is unchanged by this identification, since its coordinate derivatives and coordinate tangent bases agree by steps 1.1 and 1.3. The inequalities $g(\dot c,N)<0$ and $g(\dot c,\dot c)\le-\epsilon_c$ are unchanged under the identity tangent map. Choose the same chart intervals and exceptional set in step 2.1 for both domains; they give identical $h$ and therefore identical length. Step 3.1 removes dependence on that choice. [F2, F3, F10, step 1.1, step 1.2, step 1.3, step 2.1, step 3.1]

5.1 Apply the assumed bound $L_C$ in $B$ to each such curve into $C$. Step 4.1 shows that it is exactly an eligible curve in $B$ with the same length and the same individual constant $\epsilon_c$. The bound $L_C$ is therefore common to every eligible curve in $C$ in $W$, with no extra uniformity imposed on $\epsilon_c$. This proves the restriction property. [given, step 4.1] ∎

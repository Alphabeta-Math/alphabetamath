---
title: Positive-lapse stationary graphs give temporal level functions and closed
  restrictions
status: published
research_item: lem-author-3bd197b76c61-stationary-level-and-closed-graphs
dependency_level: 4
---

## Prerequisites

- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)
- [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)
- [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)
- [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)
- [math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-immersion-and-embedding-for-manifolds-with-boundary)
- [math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)
- [math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)
- [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)
- [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:def-causal-classification-of-lorentz-vectors](https://alphabetamath.cc/physics/item/def-causal-classification-of-lorentz-vectors)
- [math:def-c-r-and-smooth-maps-between-smooth-manifolds](https://alphabetamath.cc/item/def-c-r-and-smooth-maps-between-smooth-manifolds)
- [math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map)
- [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)
- [physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity)


## Statement

Work under the Axiom of Choice. Let $X$ be a smooth three-manifold without boundary and equip $M=\mathbb R_t\times X$ with its product smooth structure and a smooth time-oriented Lorentz metric of signature $(-,+,+,+)$. Suppose the translations $\Phi_c(t,x)=(t+c,x)$ are isometries preserving the future orientation, and put $T=\partial_t$. Let $u:X\to\mathbb R$ be smooth, with spacelike graph $\Gamma=\{(u(x),x):x\in X\}$, future unit normal $n$ and positive lapse $N=-g(T,n)>0$.

Its defining function $F(t,x)=t-u(x)$ has past timelike gradient and $dF=-g(n,\cdot)/N$ on the graph. Extend the normal and lapse by stationary translations; the same formula then holds on the whole product. Every future timelike curve, in the locally absolutely continuous class with nonzero future timelike velocity almost everywhere, meets $\Gamma$ at most once. The graph is closed relative to $M$.

Here a compact smooth domain $\Omega\subset X$ means a compact embedded codimension-zero smooth submanifold with boundary, supplied with that smooth structure and its smooth inclusion. For every such $\Omega$, the restriction $\Gamma_\Omega=\{(u(x),x):x\in\Omega\}$ is a compact smooth spacelike hypersurface with boundary, whose manifold boundary is exactly the graph over $\partial\Omega$. A common bound $|u|\le A$ on a fixed $\Omega$, with $A\ge0$, encloses all such graph restrictions in the fixed compact stationary tube $[-A,A]\times\Omega$.

## Facts & Assumptions

[A1] Use the Axiom of Choice, which implies Dependent Choice and Countable Choice. These are the choice hypotheses of the temporal-function supplier used below. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F1] The unit-normal and lapse conventions are [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data). The stationary graph convention $x\mapsto(u(x),x)$ is the one used in [def-stationary-maximal-graph](item-def-stationary-maximal-graph); the present result requires only the explicitly supplied spacelike graph, not maximality or a field equation. Smooth manifolds and the product structure are [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) and [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure).

[F2] Future timelike curves are locally absolutely continuous curves with nonzero future timelike velocity almost everywhere. On a time-oriented smooth Lorentzian four-manifold, a smooth function with past timelike gradient is strictly increasing on every such curve; the temporal-function supplier includes the almost-everywhere chain rule and integration argument under Dependent Choice and Countable Choice. [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability) [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions), parts (a) and (b). Both suppliers have domain mathematics.

[F3] An embedded smooth submanifold with boundary carries a manifold-with-boundary structure for which inclusion is a smooth embedding. An embedding is a smooth immersion, using full tangent spaces at boundary points, that is a homeomorphism onto its image. Manifold boundary points have last coordinate zero in boundary charts. [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary) [math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-immersion-and-embedding-for-manifolds-with-boundary) [math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)

[F4] A continuous map pulls closed sets back to closed sets. A continuous image of a compact space is compact. Every closed bounded real interval is compact, and a finite product of compact topological spaces is compact in the product topology. [math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top), part (c). [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps), part 1. [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r) [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)

## Proof

**Given:** The stationary product, smooth spacelike graph, future unit normal, positive lapse and compact smooth domain specified above. **Goal:** Establish the temporal level function, closedness, boundary and compact-tube assertions.

1.1 On $\Gamma$, $dF$ annihilates the graph tangent space and $dF(T)=1$. The covector $-g(n,\cdot)/N$ also annihilates that space and evaluates to one on $T$, since $N=-g(T,n)$. The tangent space has codimension one and $T$ is transverse to it, so agreement on that space and on $T$ proves $dF=-g(n,\cdot)/N$. Its metric dual is $-n/N$, which is past timelike because $n$ is future unit timelike and $N>0$. [F1, given, algebra]

1.2 The function $F$ is smooth and continuous, so [F4] applied to the closed subset $\{0\}\subset\mathbb R$ makes $\Gamma=F^{-1}(0)$ closed relative to $M$. The graph map $G:X\to M$, $G(x)=(u(x),x)$, is smooth and injective. Its differential sends $v$ to $(du(v),v)$ and is injective. Product projection restricted to its image is a continuous inverse; hence $G$ is a smooth embedding by [F3], applied to manifolds with empty boundary. [F1, F3, F4, given, construct]

2.1 Every point $(t,x)$ belongs to the unique translate $\Phi_c(\Gamma)$ with $c=t-u(x)$. Define $n(t,x)=(\Phi_c)_*n(u(x),x)$ and $N(t,x)=N(u(x),x)$. These extensions are smooth. Translations preserve the metric, time orientation and $T$, and $F\circ\Phi_c=F+c$. Transporting the covector identity from step 1.1 therefore gives $dF=-g(n,\cdot)/N$ everywhere on $M$, with past timelike dual $-n/N$. [F1, step 1.1, given, construct]

2.2 The restriction $G|_\Omega$ is smooth up to the boundary because it is the composite of the supplied smooth inclusion $\Omega\hookrightarrow X$ with $G$. Its differential is injective on the full tangent spaces, and projection to $X$ is a continuous inverse onto $\Omega$ with its subspace topology. Thus [F3] makes $G|_\Omega$ an embedding. Equip its image with the smooth structure transported from $\Omega$. Each boundary chart $\varphi$ of $\Omega$ gives the image chart $\varphi\circ(G|_\Omega)^{-1}$ with exactly the same half-space coordinates. The last coordinate vanishes precisely on $G(\partial\Omega)$, so the manifold boundary of $\Gamma_\Omega$ is exactly that image. The full tangent spaces of this three-dimensional image lie in the spacelike tangent spaces of $\Gamma$, so the induced metric remains positive definite, including at the boundary. These are actual restriction boundaries; they have not been discarded. [F1, F3, step 1.2, given, construct]

3.1 The product $M$ is a smooth four-manifold, and step 2.1 makes $F$ a smooth temporal function for its given time orientation. By [A1], both choice hypotheses of [F2] hold. Part (b) of that supplier therefore makes $F\circ\gamma$ locally absolutely continuous and strictly increasing on every future timelike curve $\gamma$. This invocation includes the almost-everywhere chain rule and integration step, rather than inferring curve monotonicity from pointwise positivity alone. Two parameter values on $\Gamma=F^{-1}(0)$ would give equal values of $F$, contradicting strict increase. [A1, F1, F2, step 2.1]

4.1 Apply the continuous-image assertion in [F4] to the compact space $\Omega$ and the continuous map $G|_\Omega$: the image $\Gamma_\Omega$ is compact. If a family has $|u|\le A$ on the fixed $\Omega$ with $A\ge0$, every image lies in $[-A,A]\times\Omega$. The interval supplier applies with endpoints $-A\le A$, and the finite-product supplier applies to that compact interval and the compact space $\Omega$. Their product topology is the subspace topology of this tube in the stationary product, so the tube is compact. The same conclusion includes empty $\Omega$ and $A=0$. [F1, F4, step 2.2, given, algebra] ∎

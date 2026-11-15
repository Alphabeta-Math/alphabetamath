---
title: The earliest contact generator is orthogonal to the distant target cut
status: draft
research_item: lem-author-fd27ddabb933-first-contact-target-normal
dependency_level: 8
---

## Prerequisites

- [lem-author-fd27ddabb933-first-contact-chronological-boundary](item-lem-author-fd27ddabb933-first-contact-chronological-boundary)
- [lem-author-fd27ddabb933-source-normal-null-generator](item-lem-author-fd27ddabb933-source-normal-null-generator)
- [physics:thm-gr-convex-normal-neighborhoods](https://alphabetamath.cc/physics/item/thm-gr-convex-normal-neighborhoods)
- [physics:lem-gr-position-vector-differential](https://alphabetamath.cc/physics/item/lem-gr-position-vector-differential)
- [physics:thm-gr-normal-neighborhood-causal-cone](https://alphabetamath.cc/physics/item/thm-gr-normal-neighborhood-causal-cone)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-fd27ddabb933-compact-first-cylinder-contact](item-lem-author-fd27ddabb933-compact-first-cylinder-contact)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)
- [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions)
- [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)
- [math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top)
- [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)


## Statement

Work in ZFC. Let $(\mathcal E,g,N)$ be a smooth globally hyperbolic time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$, let $\tau$ be temporal, and let $A\subset\tau^{-1}(0)$ be a nonempty compact smooth spacelike two-surface without boundary. Use the full data and hypotheses of the compact first-cylinder-contact construction on this same exterior and source: the stationary flow $\phi_s^T$, compact smooth spacelike cuts $C_s=\phi_s^T(C_0)$, their stationary timelike cylinder $\Gamma$, future timelike $T$ on $\Gamma$, continuity of the parameter map, $A\cap\Gamma=\varnothing$, $\tau(\phi_s^T(x))=s+\tau(x)$ for $x\in C_0$, and finite chronological access. Let $t_R$ be the minimum of all $s$ with $C_s\cap J^+_{\mathcal E}(A)\ne\varnothing$, and choose $p_R\in C_{t_R}\cap J^+_{\mathcal E}(A)$. The source-normal future affine null boundary segment $\gamma:[0,\ell]\to\mathcal E$ supplied by the source-normal generator lemma, with $\gamma(\ell)=p_R$, is also orthogonal to $C_{t_R}$ at $p_R$.

For the outward-ray conclusion, additionally require that $\Gamma=\Gamma_R$ bounds an open outer region $U_R\subset\mathcal E$ with $\partial_{\mathcal E}U_R=\Gamma_R$ and that the source is inside: $A\subset\mathcal E\setminus\overline{U_R}^{\,\mathcal E}$. Supply stationary end coordinates $(t,r,\omega)$ on an open neighborhood of $\overline{U_R}^{\,\mathcal E}$, with $U_R=\{r>R\}$, $\Gamma_R=\{r=R\}$ and $dr\ne0$ there. Specify constants $c>0$ and $t_0\in\mathbb R$ such that $T=c\partial_t$ and the very same cut family is $C_s=\{r=R,\ t=t_0+cs\}$. Require $t$ to be temporal on an open neighborhood of $\overline{U_R}^{\,\mathcal E}$. Then the final future null normal ray is outward, in the precise sense $dr(\dot\gamma(\ell))>0$. The original coordinate time may serve as $t$ whenever these conditions hold; the section time $\tau$ need not equal $t$.

Endpoint orthogonality alone requires no assumption that the target cut is globally acausal, nor any of the additional outer-region or coordinate-time conditions.

## Facts & Assumptions

[F1] No point of the first target cut is chronologically reachable from the source. [lem-author-fd27ddabb933-first-contact-chronological-boundary](item-lem-author-fd27ddabb933-first-contact-chronological-boundary)

[F2] A source-normal boundary null segment to that cut already exists. [lem-author-fd27ddabb933-source-normal-null-generator](item-lem-author-fd27ddabb933-source-normal-null-generator)

[F3] The final endpoint has arbitrarily small convex normal neighborhoods. [physics:thm-gr-convex-normal-neighborhoods](https://alphabetamath.cc/physics/item/thm-gr-convex-normal-neighborhoods)

[F4] The squared interval from a point in a convex normal neighborhood has differential twice the metric pairing with the radial final tangent. [physics:lem-gr-position-vector-differential](https://alphabetamath.cc/physics/item/lem-gr-position-vector-differential)

[F5] Negative squared interval with the future sign gives a future timelike radial segment. [physics:thm-gr-normal-neighborhood-causal-cone](https://alphabetamath.cc/physics/item/thm-gr-normal-neighborhood-causal-cone)

[F6] Causal reachability followed by a timelike segment is chronological reachability. [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[F7] The compact first-cylinder-contact construction, applied with all its hypotheses to this same exterior, source and cut family, supplies a finite minimum $t_R$ over all real cut parameters with causal contact. [lem-author-fd27ddabb933-compact-first-cylinder-contact](item-lem-author-fd27ddabb933-compact-first-cylinder-contact)

[F8] Temporal functions, causal reachability, global hyperbolicity, and boundaries relative to the specified exterior have the causal-data meanings. The outer region and coordinate identification in the Statement are supplied hypotheses, not consequences of stationarity. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F9] The normal bundle of a smooth spacelike two-surface in a time-oriented Lorentzian four-manifold is a rank-two Lorentzian bundle with exactly two future null rays in each fiber. Use the normal-plane assertion and its orthogonal-projection construction, not its null-hypersurface or optical assertions. [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)

[F10] A temporal function strictly increases along every nonconstant future causal curve in its domain. Apply clause (b) to the supplied coordinate time $t$ on its temporal neighborhood of the closed outer region. [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions)

[F11] A closed bounded real interval is compact; a continuous map has closed preimages of closed sets; a closed subspace of a compact space is compact; and a continuous real-valued function on a nonempty compact space attains a maximum. Use these statements on a parameter interval of the already existing segment and its closed set of parameters outside $U_R$. [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r) [math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top) [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact) [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

[A1] Work in ZFC, including the countable and dependent choice required by the invoked geodesic, compactness and causal interfaces. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The data and hypotheses in the Statement, with its additional hypotheses used only for the outward-ray conclusion.

**Goal:** Prove target orthogonality and the stated conditional outward-ray conclusion.

1.1 Choose a point z on the segment sufficiently close to its final endpoint $p_R$ that the remaining tail lies in a convex normal neighborhood. On that neighborhood let h(y) be the squared interval of the radial geodesic from z. Shrink it so every nearby radial inverse vector retains the future sign of the final tail. It vanishes at $p_R$. If h were negative at a nearby target-cut point with the future sign, [F5] and [F6] would make that point chronologically reachable from A, contrary to [F1]. Thus h restricted to the target cut has a local minimum zero. The differential formula [F4] makes the final tangent orthogonal to every target tangent vector. [F1, F2, F3, F4, F5, F6, given]

2.1 Assume the additional outer-region and coordinate hypotheses. At $p_R$ let $P$ be the metric-orthogonal projection onto the positive-definite target tangent plane. Since $T$ is future timelike and tangent to $\Gamma_R$, the vector $Y=T-P(T)$ is tangent to $\Gamma_R$, normal to the cut and future timelike: $g(Y,Y)=g(T,T)-g(P(T),P(T))<0$ and $g(Y,T)=g(Y,Y)<0$. Set $e=Y/\sqrt{-g(Y,Y)}$. In the Lorentzian normal plane of [F9], choose a unit spacelike vector $n$ orthogonal to $e$. The kernel of $dr$ in that normal plane is exactly $\mathbb Re$: indeed $T_{p_R}\Gamma_R$ is the direct sum of the target tangent plane and $\mathbb Re$. Thus $dr(n)\ne0$, and choose its sign so that $dr(n)>0$. The two future null normal rays are the positive multiples of $e+n$ and $e-n$, with opposite nonzero radial components. By step 1.1, the final tangent belongs to one of these rays. [given, F9, step 1.1, algebra]

3.1 Suppose the final tangent is on the inward ray. Then $dr(\dot\gamma(\ell))<0$, so smoothness places $\gamma(s)$ in $U_R$ for all $s<\ell$ sufficiently close to $\ell$. Choose $b\in(0,\ell)$ in this final interval. The set $K=\{s\in[0,b]:\gamma(s)\notin U_R\}$ contains $0$ because the source is inside. It is closed in $[0,b]$ by continuity and openness of $U_R$, and hence compact by [F11]. The identity function on nonempty $K$ therefore attains a largest value $s_0$, with $s_0<b$ since $\gamma(b)\in U_R$. Maximality and the choice of $b$ put $\gamma((s_0,\ell))$ entirely in $U_R$. Continuity gives $z=\gamma(s_0)\in\partial_{\mathcal E}U_R=\Gamma_R$: it is outside $U_R$ at $s_0$ and is a limit of points inside. The source's disjointness from the closed outer region gives $s_0>0$. The initial segment of $\gamma$ makes $z$ causally reachable from $A$. [given, F2, F8, F11, step 2.1, choose]

4.1 The nonconstant future causal tail from $z$ to $p_R$ lies in $\overline{U_R}^{\,\mathcal E}$, so [F10] gives $t(z)<t(p_R)=t_0+ct_R$. Coordinate compatibility places $z$ in $C_u$ with $u=(t(z)-t_0)/c<t_R$. This is a causal contact earlier than the global minimum supplied by [F7], a contradiction. Step 2.1 excludes a zero radial component, so the final ray must be outward. Together with step 1.1 this proves both conclusions, with no global acausality assumption on a general target cut. [given, F7, F10, step 1.1, step 2.1, step 3.1, algebra, contradiction] ∎

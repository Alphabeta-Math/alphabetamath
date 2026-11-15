---
title: Endpoint orthogonality without an acausal target assumption
status: draft
research_item: lem-author-2632702918ef-target-endpoint-orthogonality
dependency_level: 4
sources:
  references: []
---

## Prerequisites

- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)
- [lem-author-2632702918ef-compact-target-null-segment](item-lem-author-2632702918ef-compact-target-null-segment)
- [physics:thm-gr-convex-normal-neighborhoods](https://alphabetamath.cc/physics/item/thm-gr-convex-normal-neighborhoods)
- [physics:lem-gr-position-vector-differential](https://alphabetamath.cc/physics/item/lem-gr-position-vector-differential)
- [physics:thm-gr-normal-neighborhood-causal-cone](https://alphabetamath.cc/physics/item/thm-gr-normal-neighborhood-causal-cone)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [physics:lem-gr-observer-pairing-with-future-causal-vectors](https://alphabetamath.cc/physics/item/lem-gr-observer-pairing-with-future-causal-vectors)
- [math:cor-every-tangent-vector-is-the-velocity-of-a-smooth-curve](https://alphabetamath.cc/item/cor-every-tangent-vector-is-the-velocity-of-a-smooth-curve)
- [math:thm-fermat-interior-extremum](https://alphabetamath.cc/item/thm-fermat-interior-extremum)
- [math:def-differential-of-a-smooth-real-valued-function](https://alphabetamath.cc/item/def-differential-of-a-smooth-real-valued-function)
- [math:def-velocity-derivation-of-a-smooth-curve](https://alphabetamath.cc/item/def-velocity-derivation-of-a-smooth-curve)
- [physics:def-gr-fx-future-null-geodesic-completeness](https://alphabetamath.cc/physics/item/def-gr-fx-future-null-geodesic-completeness)


## Statement

Under the same compact-target hypotheses, let $\gamma:[0,1]\to E$ be a smooth nonconstant future null affine geodesic with $\gamma(0)=p$ and $\gamma(1)=c\in C$. Then $g(\dot\gamma(1),Y)=0$ for every $Y\in T_cC$. It suffices that $C$ be smooth and without boundary near $c$; no global acausality assumption on $C$ is needed.

## Facts & Assumptions

[A1] Work in ZFC; the axiom of choice implies the countable and dependent choice assumptions of the causal suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F1] The smooth metric, connection, causal relations and time orientation are those of [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data).

[F2] The target is a smooth embedded spacelike two-manifold without boundary. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F3] The initial point satisfies $p\notin I_E^-(C)$. [lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)

[F4] Such a smooth null affine segment exists under these hypotheses. [lem-author-2632702918ef-compact-target-null-segment](item-lem-author-2632702918ef-compact-target-null-segment)

[F5] Every point has arbitrarily small convex normal neighborhoods. [physics:thm-gr-convex-normal-neighborhoods](https://alphabetamath.cc/physics/item/thm-gr-convex-normal-neighborhoods)

[F6] On a convex normal neighborhood, $h(q)=g_r(\exp_r^{-1}(q),\exp_r^{-1}(q))$ is smooth and $dh_q(Y)=2g_q(P(r,q),Y)$, where $P(r,q)$ is the final tangent of the radial geodesic on $[0,1]$. [physics:lem-gr-position-vector-differential](https://alphabetamath.cc/physics/item/lem-gr-position-vector-differential)

[F7] A future timelike radial inverse vector in a convex normal neighborhood gives a future timelike geodesic. [physics:thm-gr-normal-neighborhood-causal-cone](https://alphabetamath.cc/physics/item/thm-gr-normal-neighborhood-causal-cone)

[F8] Causal then timelike reachability implies timelike reachability. [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[F9] At a point with future unit observer $n$, every nonzero future causal vector $w$ satisfies $g(n,w)<0$. A unit timelike vector $w$ is future-directed if and only if $g(n,w)<0$. These are clauses (1) and (3) of [physics:lem-gr-observer-pairing-with-future-causal-vectors](https://alphabetamath.cc/physics/item/lem-gr-observer-pairing-with-future-causal-vectors).

[F10] Every tangent vector to a smooth manifold is the velocity of a smooth curve through that point. Applied to the manifold $C$ without boundary, the curve is defined on an open interval about zero. [math:cor-every-tangent-vector-is-the-velocity-of-a-smooth-curve](https://alphabetamath.cc/item/cor-every-tangent-vector-is-the-velocity-of-a-smooth-curve)

[F11] A real function differentiable at an interior point of its domain has derivative zero there if it has a local extremum there. [math:thm-fermat-interior-extremum](https://alphabetamath.cc/item/thm-fermat-interior-extremum)

[F12] For a smooth real function $f$, $df_x(V)=V([f])$; the velocity derivation of a smooth curve $\eta$ acts by $\dot\eta(0)([f])=(f\circ\eta)'(0)$. Thus $df_{\eta(0)}(\dot\eta(0))=(f\circ\eta)'(0)$. [math:def-differential-of-a-smooth-real-valued-function](https://alphabetamath.cc/item/def-differential-of-a-smooth-real-valued-function) [math:def-velocity-derivation-of-a-smooth-curve](https://alphabetamath.cc/item/def-velocity-derivation-of-a-smooth-curve)

[F13] A future null affine geodesic is a smooth nonconstant curve whose tangent is nonzero, future-directed and null and satisfies $D_s\dot\gamma=0$ at every interior parameter. Only the geodesic definition is used; no completeness condition is imposed. [physics:def-gr-fx-future-null-geodesic-completeness](https://alphabetamath.cc/physics/item/def-gr-fx-future-null-geodesic-completeness)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the asserted conclusion.

1.1 Choose by [F5] a strictly convex normal neighborhood $B\subset E$ of $c$ and $s_0\in(0,1)$ sufficiently close to $1$ that the tail of $\gamma$ from $r=\gamma(s_0)$ to $c$ lies in $B$. Use the inverse domains selected by $B$ and put $v(q)=\exp_r^{-1}(q)$ and $h(q)=g_r(v(q),v(q))$ for $q\in B$. By the affine geodesic definition in [F13] and uniqueness of the joining geodesic in [F5], its radial segment to $c$ is $t\mapsto\gamma(s_0+(1-s_0)t)$, so $v(c)=(1-s_0)\dot\gamma(s_0)$ is nonzero future null and $h(c)=0$. Normalize $n_r=N_r/\sqrt{-g_r(N_r,N_r)}$, so $g_r(n_r,n_r)=-1$ and $g_r(n_r,N_r)<0$; this is a future unit observer. Clause (1) of [F9] gives $g_r(v(c),n_r)<0$. By continuity, restrict to a neighborhood $V\subset B$ of $c$ where $g_r(v(q),n_r)<0$. If $q\in V\cap C$ had $h(q)<0$, then $w=v(q)/\sqrt{-h(q)}$ would be unit timelike with $g_r(w,n_r)<0$. Clause (3) of [F9] makes $w$, and hence its positive multiple $v(q)$, future-directed. By [F7] the radial geodesic in $B\subset E$ gives $r\ll_E q$. The initial segment of $\gamma$ gives $p\le_E r$, so [F8] gives $p\ll_E q$, contradicting [F3]. Consequently $h|_{V\cap C}\ge0$ and $h(c)=0$. The causal suppliers are used with the choice assumptions in [A1]. [A1, F1, F2, F3, F5, F6, F7, F8, F9, F13, given, algebra]

2.1 Fix $Y\in T_cC$. By [F10], since $C$ is smooth without boundary, there is a smooth curve $\eta:(-\varepsilon,\varepsilon)\to C$ with $\eta(0)=c$ and $\dot\eta(0)=Y$. Shrink $\varepsilon>0$ so that $\eta$ lies in $V\cap C$. The smooth real function $f=h\circ\eta$ has a local minimum at the interior parameter $0$ by step 1.1, so [F11] gives $f'(0)=0$. Regard $Y$ as its ambient tangent under the embedded inclusion; [F12] identifies $f'(0)=dh_c(Y)$. By [F6], $0=dh_c(Y)=2g_c(P(r,c),Y)$. The radial segment identified in step 1.1 has terminal tangent $P(r,c)=(1-s_0)\dot\gamma(1)$. Dividing by $2(1-s_0)>0$ proves $g_c(\dot\gamma(1),Y)=0$ for every $Y$. Only endpoints near $c$ were varied, so no global acausality of $C$ is required; [F4] supplies the existence of a segment under the compact-target hypotheses. [step 1.1, F1, F2, F4, F6, F10, F11, F12, algebra] ∎

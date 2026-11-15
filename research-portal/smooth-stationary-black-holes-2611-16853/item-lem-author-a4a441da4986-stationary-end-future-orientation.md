---
title: Stationary end access and future orientation need no maximal slice
status: published
research_item: lem-author-a4a441da4986-stationary-end-future-orientation
dependency_level: 3
---

## Prerequisites

- [lem-author-a4a441da4986-doc-connected-and-causally-convex](item-lem-author-a4a441da4986-doc-connected-and-causally-convex)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)
- [physics:lem-gr-cauchy-set-topology-and-graph](https://alphabetamath.cc/physics/item/lem-gr-cauchy-set-topology-and-graph)
- [math:def-connected-space](https://alphabetamath.cc/item/def-connected-space)
- [math:cor-connected-subsets-of-the-line](https://alphabetamath.cc/item/cor-connected-subsets-of-the-line)
- [math:thm-continuous-image-of-a-connected-space](https://alphabetamath.cc/item/thm-continuous-image-of-a-connected-space)


## Statement

In the regular stationary exterior, its selected asymptotic end is invariant under the stationary translations and has two-sided chronological access inside $E$: every exterior point reaches the end and is reached from it by timelike curves lying in $E$. With $T$ future timelike in the sufficiently far asymptotic end and with complete stationary orbits in $E$, $T$ cannot be past timelike anywhere in $E$.

## Statement references

[lem-author-a4a441da4986-doc-connected-and-causally-convex](item-lem-author-a4a441da4986-doc-connected-and-causally-convex)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)

[physics:lem-gr-cauchy-set-topology-and-graph](https://alphabetamath.cc/physics/item/lem-gr-cauchy-set-topology-and-graph)

[math:def-connected-space](https://alphabetamath.cc/item/def-connected-space)

[math:cor-connected-subsets-of-the-line](https://alphabetamath.cc/item/cor-connected-subsets-of-the-line)

[math:thm-continuous-image-of-a-connected-space](https://alphabetamath.cc/item/thm-continuous-image-of-a-connected-space)

## Facts & Assumptions

[F1] The declared geometry, causal, operator and earlier-result inputs are [lem-author-a4a441da4986-doc-connected-and-causally-convex](item-lem-author-a4a441da4986-doc-connected-and-causally-convex) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness) [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[F2] Under the choice assumptions in [F4], the causal-curve calculus supplies smooth composition and its almost-everywhere velocity formula in clause (b), inclusion of piecewise $C^1$ future timelike paths in clause (c), finite concatenation in clause (d), and positive affine reparametrization in clause (e). [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[F3] The flow interface supplies the smooth flow, integral-curve and group laws. The tensor-invariance proposition applied to the metric $g$ and the Killing equation $\mathcal L_Tg=0$ supplies $(\Phi_s^T)^*g=g$ on each flow domain. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)

[F4] The regularity definition works in ZFC, so Countable Choice and Dependent Choice, assumed by the causal suppliers, hold here. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F5] Write $U=M^{\mathrm{end}}$ and $C=\Sigma_0\cap E$. The regularity definition supplies the product chart $U=\mathbb R\times\{r>R_0\}$, $T=\partial_t$, a sufficiently far tail on which $T$ is future timelike, and the Cauchy hypersurface $C$ in $E$, with $C\cap U=\{t=0\}$. Only the far-tail timelikeness is used below; timelikeness on all of $U$ is not assumed. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F6] Apply clause (a) of the Cauchy-set supplier to the time-oriented smooth spacetime $E$ and its Cauchy set $C$, under [F4]. It gives $E=I^-_E(C)\sqcup C\sqcup I^+_E(C)$, acausality of $C$, and absence of closed nonconstant causal curves in $E$. The two chronological sides are open, being unions of open chronological futures or pasts of points. [physics:lem-gr-cauchy-set-topology-and-graph](https://alphabetamath.cc/physics/item/lem-gr-cauchy-set-topology-and-graph) [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[F7] The interval $[0,1]$ is connected; its image under a continuous path is connected and cannot be partitioned into two nonempty disjoint relatively open subsets. These are the interval, continuous-image (claim 1), and separation conventions used for the radial paths below. [math:cor-connected-subsets-of-the-line](https://alphabetamath.cc/item/cor-connected-subsets-of-the-line) [math:thm-continuous-image-of-a-connected-space](https://alphabetamath.cc/item/thm-continuous-image-of-a-connected-space) [math:def-connected-space](https://alphabetamath.cc/item/def-connected-space)

## Proof

**Given:** The regular stationary geometry and chronological exterior in [F1], the curve and flow interfaces [F2]–[F3], the inherited choice assumptions [F4], and the end, Cauchy-set and connectedness inputs [F5]–[F7].

**Goal:** Prove the stated end access and future orientation without assuming a maximal slice or a lapse sign.

1.1 The open connected product end $U$ lies in $E$ by the selected-exterior supplier in [F1]. For each $p\in E$, the definition of $E$ gives $a,b\in U$ and future timelike curves $a\ll_M p\ll_M b$; causal convexity from the same supplier keeps both curves in $E$. Explicitly, an interior point $z$ of the first curve satisfies $a\ll_M z\le_M p\ll_M b$ by restriction, and the push-up input in [F1] gives $z\ll_M b$; on the second curve it applies to $a\ll_M p\le_M z\ll_M b$ to give $a\ll_M z$. The endpoints are already in $E$. Hence $a\ll_E p\ll_E b$. The chart in [F5] has the full real time coordinate and $T=\partial_t$, so stationary translations send $(t,x)$ to $(t+s,x)$ and preserve $U$. This proves its invariance and the stated two-sided access to the full selected end. [given, F1, F2, F4, F5]

1.2 Completeness of the stationary orbits in $E$ and the flow laws in [F3] give smooth maps $\Phi_s^T:E\to E$ for all real $s$, with inverses $\Phi_{-s}^T$. They are isometries by [F3]. For a fixed future timelike $v\in T_qE$, the vector $(d\Phi_s^T)_qv$ varies continuously with $s$ and remains timelike. Relative to the continuous time orientation at $\Phi_s^Tq$, its future or past component cannot change along the real parameter interval; at $s=0$ it is future. Thus each $\Phi_s^T$ preserves time orientation. By the smooth-composition formula [F2](b), it carries every locally absolutely continuous future timelike curve to another such curve, with almost-everywhere velocity $(d\Phi_s^T)\gamma'$. In particular, it preserves chronological comparisons inside $E$. Differentiating the flow group law in its orbit parameter also gives $(d\Phi_s^T)_qT_q=T_{\Phi_s^Tq}$. [given, F1, F2, F3, F4]

2.1 Fix $(t,x)\in U$ with $t\ne0$. Choose $R>|x|$ sufficiently large that $x_*=Rx/|x|$ lies in the future timelike tail. The continuous radial path $u\mapsto(t,((1-u)+uR/|x|)x)$, $0\le u\le1$, stays in $U\subset E$ and avoids $C$ by [F5]. Its image is connected by [F7]. The disjoint open sides in [F6] cover this image, so it lies entirely in one side. At its far endpoint, the vertical orbit segment from $(0,x_*)$ to $(t,x_*)$ is future timelike if $t>0$, and the segment from $(t,x_*)$ to $(0,x_*)$ is future timelike if $t<0$, by [F5] and [F2](c). Since $(0,x_*)\in C$, this identifies the side throughout the radial path. Consequently every end point with $t>0$ belongs to $I^+_E(C)$ and every end point with $t<0$ belongs to $I^-_E(C)$. This uses no chronological connection between the radial path's endpoints. [F2, F4, F5, F6, F7, step 1.1]

2.2 Suppose $T$ were past timelike at $p\in E$. For some $\epsilon>0$ the negative-flow local orbit segment is smooth future timelike, so $p\ll_E\Phi^T_{-\epsilon}p$ by [F2](c). Choose $a,b\in U$ with $a\ll_E p\ll_E b$ by step 1.1. Choose $s$ so that $t(a)+s>0$ and set $A=\Phi_s^Ta$, $P=\Phi_s^Tp$, $B=\Phi_s^Tb$. Step 1.2 gives $A\ll_E P\ll_E B$ and $P\ll_E\Phi^T_{-\epsilon}P$. Translating the latter comparison and concatenating finitely many curves using [F2](d)–(e) gives $P\ll_E\Phi^T_{-n\epsilon}P$ for every positive integer $n$. Translating $P\ll_E B$ and concatenating yields $A\ll_E\Phi^T_{-n\epsilon}B$. [F2, step 1.1, step 1.2]

3.1 Choose a positive integer $n$ with $n\epsilon>t(b)+s$. Then $A$ is an end point of positive time and $\Phi^T_{-n\epsilon}B$ is an end point of negative time. Step 2.1 gives $c_-,c_+\in C$ with $c_-\ll_E A$ and $\Phi^T_{-n\epsilon}B\ll_E c_+$. Concatenating these comparisons with step 2.2 gives $c_-\ll_E c_+$. If $c_-\ne c_+$ this contradicts acausality of $C$ in [F6]; if they coincide it is a closed future timelike curve, also excluded by [F6]. Thus $T$ cannot be past timelike anywhere in $E$, as claimed. [F2, F6, step 2.1, step 2.2] ∎

---
title: Complete two-ended geometry and decay of the reflected data
status: published
research_item: lem-author-294e9b08725d-complete-asymptotically-flat-double
dependency_level: 10
sources:
  references: []
---

## Prerequisites

- [lem-author-294e9b08725d-smooth-vacuum-data-double](item-lem-author-294e9b08725d-smooth-vacuum-data-double)
- [lem-author-294e9b08725d-stationary-vacuum-kid-double](item-lem-author-294e9b08725d-stationary-vacuum-kid-double)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [lem-author-294e9b08725d-stationary-end-extrinsic-decay](item-lem-author-294e9b08725d-stationary-end-extrinsic-decay)
- [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)
- [lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice)
- [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)
- [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)
- [math:thm-the-riemannian-distance-topology-is-the-manifold-topology](https://alphabetamath.cc/item/thm-the-riemannian-distance-topology-is-the-manifold-topology)
- [math:def-cauchy-in-metric](https://alphabetamath.cc/item/def-cauchy-in-metric)
- [math:def-complete-metric-space](https://alphabetamath.cc/item/def-complete-metric-space)
- [math:thm-compact-implies-complete-and-totally-bounded](https://alphabetamath.cc/item/thm-compact-implies-complete-and-totally-bounded)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)



## Statement

Work in ZFC, including the Axiom of Choice. Retain all hypotheses of the smooth vacuum data-double construction. In particular, the positive half $\overline C=C\cup S$ is a connected smooth manifold with nonempty compact boundary $S$, and its specified collar is the positive canonical boost section. Use $K(U,V)=g(\nabla_U n,V)=-k(U,V)$, with the normal and reflection conventions of that construction.

Suppose the positive half has a specified Euclidean end chart $x:E\to\{x\in\mathbb R^3:r=|x|>R_0\}$, disjoint from $S$, with $h-\delta=O_6(r^{-1})$ and $K=O_5(r^{-3})$. The compact-complement requirement is explicit: for every sufficiently large $R$, the truncation $B_R=\overline C\setminus x^{-1}(\{r>R\})$ is a compact smooth region with boundary $S\cup x^{-1}(\{r=R\})$. These truncations exhaust the positive half.

Then the smooth double $\widehat C$ is complete in its intrinsic Riemannian distance, has two Euclidean ends and a compact intervening region, and has the same differentiated data bounds on each end (the second fundamental form changes sign on the reflected end). In particular it satisfies $h-\delta=O_4(r^{-1})$ and $K=O_3(r^{-2})$ on both ends.

If, in addition, the hypotheses of the stationary vacuum KID construction hold, in particular $T$ is Killing in an actual smooth Ricci-flat neighborhood of the positive section and commutes with the exact boost field on the canonical collar, use its induced lapse $N=-g(T,n)$ and its odd reflection. The reflected stationary lapse tends to $-1$ if the original lapse tends to $1$. These initial-data facts do not identify any domain of outer communications in a development.

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** Complete two-ended reflected initial data with the stated decay and lapse limits.

[A1] The Axiom of Choice is retained for the global smooth-double construction; the Cauchy-sequence argument below uses no additional choice principle. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Under its stated hypotheses, the smooth-data construction gives a smooth boundaryless double with reflected metric and minus the reflected second fundamental form. [lem-author-294e9b08725d-smooth-vacuum-data-double](item-lem-author-294e9b08725d-smooth-vacuum-data-double)

[F2] Under the actual vacuum-neighborhood and boost-commutation hypotheses, the stationary KID construction gives a smooth reflected lapse satisfying $N_-=-N_+\circ I$, where $I:C_-\to C_+$ is the copy identification; its convention is $K=-k$. [lem-author-294e9b08725d-stationary-vacuum-kid-double](item-lem-author-294e9b08725d-stationary-vacuum-kid-double)

[F3] The differentiated bounds use Cartesian derivatives and angular uniformity. In the abstract formulation the displayed data bounds are explicit hypotheses. For the separate stationary-end application, assume all hypotheses of the stationary-end extrinsic-decay supplier: the original regular stationary geometry, its stationary $t=0$ end with $T=\partial_t=Nn+X$ and future normal chosen so that $N>0$, and the expansions $g_{00}=-1+2M_0/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$. Under these hypotheses that supplier gives $k=O_5(r^{-3})$ and $N=1+O_6(r^{-1})$; $K=-k$ has the same curvature decay. No maximality or positivity of $M_0$ is required for this end-decay deduction. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) [lem-author-294e9b08725d-stationary-end-extrinsic-decay](item-lem-author-294e9b08725d-stationary-end-extrinsic-decay)

[F4] For the separate canonical-section application, assume all regular-spacetime hypotheses of the exact outer-section supplier and all regular stationary-vacuum hypotheses of the canonical Cauchy-splice supplier, including its supplied working partial-Cauchy section and local boost input, for the same original spacetime, section and physical stationary end. Under these hypotheses the exact original outer closure admits an adapted topological identification with $\{|y|\geq1\}$ and has compact truncations in the separate physical end radius $r=|x|$; the outer-section supplier also gives $h-\delta=O_6(r^{-1})$ on that original end. No agreement of those two charts is assumed. The canonical Cauchy splice then has ambient closure $C_0\cup S$, a smooth manifold with compact boundary $S$, agrees with the original section on the stationary end, and changes the original working section only in a compact neighborhood of $S$. These conditional premises establish compact truncations and preserve the metric end bound for that canonical section; they are not additional premises for the abstract double conclusion. [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section) [lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice)

[F5] Riemannian length integrates $\sqrt{h(\dot\gamma,\dot\gamma)}$ along piecewise $C^1$ curves. On a connected Riemannian manifold the intrinsic distance is the infimum of these lengths and its topology is the manifold topology. [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length) [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold) [math:thm-the-riemannian-distance-topology-is-the-manifold-topology](https://alphabetamath.cc/item/thm-the-riemannian-distance-topology-is-the-manifold-topology)

[F6] A metric sequence is Cauchy when every positive tolerance bounds all sufficiently late pairwise distances. Completeness means that every Cauchy sequence converges in the metric. Every compact metric space is complete, also for a restricted ambient metric. [math:def-cauchy-in-metric](https://alphabetamath.cc/item/def-cauchy-in-metric) [math:def-complete-metric-space](https://alphabetamath.cc/item/def-complete-metric-space) [math:thm-compact-implies-complete-and-totally-bounded](https://alphabetamath.cc/item/thm-compact-implies-complete-and-totally-bounded)

## Proof

**Given:** The compact exhaustion, decay and construction hypotheses of the Statement, with [A1], [F1], [F5] and [F6]; use [F2] only under the additional stationary KID hypotheses, and the separate applications in [F3]–[F4] only under their expressly stated supplier hypotheses.

**Goal:** Prove the compact two-ended structure, differentiated estimates, metric completeness and reflected lapse limit.

1.1 The compact-complement hypothesis is an explicit premise for the abstract positive half. For the separate canonical-section application, assume the full supplier hypotheses specified in F4 and use its conditional closure, compact-change and unchanged-end conclusions. Let $L$ be a compact ambient set containing the region of change, and take $R$ sufficiently large that the common stationary tail $r>R$ misses $L$. Write $D_R$ for the original compact radial truncation. The new truncation $B_R=(C_0\cup S)\setminus\{r>R\}$ is contained in $L\cup D_R$: every point outside $L$ is unchanged, and outside the removed tail is therefore in $D_R$. The set $C_0\cup S$ is closed in the ambient manifold because it is the supplied ambient closure; the common tail is relatively open in it. Thus $B_R$ is ambient closed. To check compactness directly, represent any relative open cover of $B_R$ by ambient open sets and add the ambient open complement of $B_R$. This covers each of the compact sets $L$ and $D_R$; combining their finite subcovers and discarding the complement gives a finite subcover of $B_R$. The boundary is $S$ together with the unchanged end sphere $r=R$, since the closure is a smooth manifold with boundary $S$ and the additional cut is made in the smooth end chart. These truncations exhaust the closure. This proves the canonical compact-complement application without requiring an isotopy or any spacetime development of the double. [F4, given]

1.2 In the copying charts the metric coefficients on the two ends coincide, and the $K$ coefficients have opposite signs. Every Cartesian derivative is therefore the same or its negative on the two copies. All the order-six metric and order-five second-fundamental-form estimates carry over unchanged. For $r\geq1$, dropping derivatives gives $h-\delta=O_4(r^{-1})$, and $r^{-3-|\beta|}\leq r^{-2-|\beta|}$ for $|\beta|\leq3$ gives $K=O_3(r^{-2})$. For the separate canonical application, assume all supplier hypotheses in F3 and F4. F4 supplies the original metric bound and its preservation on the unchanged end of the splice; F3 supplies the original extrinsic-curvature bound, preserved on that same unchanged end. The end-decay deduction requires no maximality assumption. [F1, F3, F4, given, algebra]

2.1 For each sufficiently large $R$, let $H_R$ be the image in $\widehat C$ of the two copies of $B_R$. It is compact: an open cover pulls back to an open cover of each compact copy, and the two finite subcovers together cover $H_R$. Its complement is precisely the disjoint union of the two copied tails $r>R$. The $H_R$ exhaust the double. The two connected halves meet along the nonempty seam $S$, so their union is connected: a separation would restrict to a separation of each half, and their common points force them into the same member. F1 and the inherited choice convention give the smooth boundaryless Riemannian double. Each tail is a Euclidean exterior and its larger radial tails stay connected, so this compact exhaustion has exactly two Euclidean ends and no additional end. [F1, A1, given, step 1.1]

3.1 By the zeroth-order metric decay, choose $R$ large enough that $h(v,v)\geq\tfrac12|v|^2$ on both tails $r\geq R$. Fix $q\in H_R$. Any piecewise $C^1$ curve from $q$ to a point $p$ in one tail with $r(p)>R$ must cross that tail's sphere $r=R$. Its last crossing exists because the parameter interval and that sphere are compact and the sphere is closed. The remaining curve lies in $r\geq R$ in the same tail. On each smooth piece there, $|(r\circ\gamma)^\prime|\leq|\dot x|\leq\sqrt2\sqrt{h(\dot\gamma,\dot\gamma)}$. Integration gives $L_h(\gamma)\geq(r(p)-R)/\sqrt2$. Taking the infimum over all curves, including ones that visit the compact region or the other end, gives $d_h(q,p)\geq(r(p)-R)/\sqrt2$. [F3, F5, step 2.1, step 1.2, algebra]

4.1 Let $(p_j)$ be any $d_h$-Cauchy sequence. Choose $j_0$ such that $d_h(p_j,p_{j_0})<1$ for all $j\geq j_0$, and enlarge the radius in step 3.1 so that $q=p_{j_0}\in H_R$. That step implies that every tail point $p_j$ with $j\geq j_0$ has $r(p_j)<R+\sqrt2$; the other such points already lie in $H_R$. Increase a radius $A>R+\sqrt2$ to include the finitely many earlier points as well. The whole sequence is contained in the compact set $H_A$. This bound rules out unbounded excursions through either end. [F5, F6, step 2.1, step 3.1, choose]

5.1 By F5, the topology of the restricted metric $d_h|_{H_A\times H_A}$ is the subspace manifold topology on $H_A$. Hence its compactness from step 2.1 is compactness for this restricted metric. By F6 that compact metric space is complete, so the sequence in step 4.1 converges in this same distance to a point of $H_A\subset\widehat C$. This is the restriction of the distance on the whole double, and need not equal the intrinsic distance of $H_A$. Every $d_h$-Cauchy sequence thus converges in $\widehat C$, which proves the claimed metric completeness. [F5, F6, step 2.1, step 4.1]

6.1 For the additional lapse assertion, retain the stationary KID hypotheses stated explicitly in the Statement. On the negative copied end F2 gives $N_-=-N_+\circ I$, so $N_+\to1$ implies $N_-\to-1$ in the copying chart. This does not assert that the same stationary Killing field is future timelike at both ends. The metric conclusions proved in the preceding steps do not require these additional Killing-field hypotheses. Together these arguments prove all stated initial-data conclusions, without identifying a domain of outer communications in any development. [F2, given, step 2.1, step 1.2, step 5.1, algebra] ∎

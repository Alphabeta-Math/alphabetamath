---
title: Radial comparison gives proper normal projection onto a fixed target collar
status: draft
research_item: lem-author-840894718169-fixed-target-collar-properness
dependency_level: 5
---

## Prerequisites

- [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone)
- [lem-author-840894718169-normal-projection-local-and-boundary-jets](item-lem-author-840894718169-normal-projection-local-and-boundary-jets)
- [math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets](https://alphabetamath.cc/item/thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)
- [math:thm-euclidean-heine-borel-pseudocompactness-and-extreme-values](https://alphabetamath.cc/item/thm-euclidean-heine-borel-pseudocompactness-and-extreme-values)
- [math:lem-closed-subset-of-a-compact-space-is-compact](https://alphabetamath.cc/item/lem-closed-subset-of-a-compact-space-is-compact)
- [math:lem-compactness-is-intrinsic](https://alphabetamath.cc/item/lem-compactness-is-intrinsic)
- [math:thm-continuous-image-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-continuous-image-of-a-compact-space-is-compact)
- [math:cor-euclidean-spheres-are-path-connected](https://alphabetamath.cc/item/cor-euclidean-spheres-are-path-connected)
- [math:thm-path-connected-implies-connected](https://alphabetamath.cc/item/thm-path-connected-implies-connected)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-proper-map-between-euclidean-open-sets](https://alphabetamath.cc/item/def-proper-map-between-euclidean-open-sets)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)


## Statement

Work in ZFC. Take the smooth Lorentzian metric family, compact embedded sphere $S$, uniformly spacelike reference section, signed boundary-distance collars $c_q(\rho,y)$, common Killing field $K$ vanishing on $S$, and signed normal-plane boost constant $\kappa$ satisfying the geometric hypotheses of the uniform Gaussian-flow lemma. Its optional event-boundary hypotheses are not needed here. Fix a smooth identification $S\cong S^2$. For a common finite bound $C\ge0$, choose $\rho_0>0$ so that the lemma's common Gaussian chart and bounded-time flow estimates hold on the entire closed reference collar $0\le\rho\le\rho_0$, for all background parameters and $|s|\le C$.

For each supplied candidate at parameter $q$, let its $K$-height $u_q$ be smooth individually on this closed collar and satisfy $|u_q|\le C$ there. Require the map $\Phi_q(c_q(\rho,y))=\phi^K_{u_q(c_q(\rho,y))}(c_q(\rho,y))$ to be a smooth embedding with spacelike image on the closed collar; on its interior it is an admissible flow graph in the stated flow-graph convention. No uniform derivatives of $u_q$ are assumed. Let $P_q=\pi_q^\perp\circ\Phi_q$ be its Gaussian normal projection in reference coordinates, and let $R_q=r\circ P_q$ be its target boundary radius. The uniform-flow lemma supplies $c_1,c_2>0$ with $c_1\rho\le R_q\le c_2\rho$ throughout this collar. For any fixed $0<r_\delta<c_1\rho_0/2$, put $V_q=(0,r_\delta)\times S$ in target collar coordinates and $U_q=\{(\rho,y):0<\rho<\rho_0,\ 0<R_q(\rho,y)<r_\delta\}$. Then $P_q:U_q\to V_q$ is a proper local diffeomorphism, hence surjective with finite evenly covered fibres. Equivalently this holds for normal projection on the corresponding candidate portion via $\Phi_q$. The same target radius works for every supplied candidate, without a uniform inverse-function radius or uniform height-derivative bounds.

## Statement references

[lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone)

[lem-author-840894718169-normal-projection-local-and-boundary-jets](item-lem-author-840894718169-normal-projection-local-and-boundary-jets)

[math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets](https://alphabetamath.cc/item/thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[math:thm-euclidean-heine-borel-pseudocompactness-and-extreme-values](https://alphabetamath.cc/item/thm-euclidean-heine-borel-pseudocompactness-and-extreme-values)

[math:lem-closed-subset-of-a-compact-space-is-compact](https://alphabetamath.cc/item/lem-closed-subset-of-a-compact-space-is-compact)

[math:lem-compactness-is-intrinsic](https://alphabetamath.cc/item/lem-compactness-is-intrinsic)

[math:thm-continuous-image-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-continuous-image-of-a-compact-space-is-compact)

[math:cor-euclidean-spheres-are-path-connected](https://alphabetamath.cc/item/cor-euclidean-spheres-are-path-connected)

[math:thm-path-connected-implies-connected](https://alphabetamath.cc/item/thm-path-connected-implies-connected)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:def-proper-map-between-euclidean-open-sets](https://alphabetamath.cc/item/def-proper-map-between-euclidean-open-sets)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

## Facts & Assumptions

[A1] Use ZFC as in the uniform-flow supplier, including its Choice assumption for the compact Gaussian-chart construction; the properness argument below introduces no further choice requirement. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone)

[F1] On the full chosen closed reference collar, bounded flow times lie in the common Gaussian chart and satisfy the uniform radial comparison with constants $c_1,c_2>0$. The Gaussian projection fibres are timelike. [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone)

[F2] A smooth spacelike embedded flow graph has locally invertible Gaussian normal projection on its interior. Its projection in reference coordinates is smooth, and equals the identity on $S$. Spacelike and flow-graph data have their stated mathematical meanings. [lem-author-840894718169-normal-projection-local-and-boundary-jets](item-lem-author-840894718169-normal-projection-local-and-boundary-jets) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[F3] For nonempty Euclidean open sets of the same dimension with connected target, a proper $C^1$ map whose derivative is everywhere invertible is surjective and has finite evenly covered fibres. [math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets](https://alphabetamath.cc/item/thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets)

[F4] A nonempty Euclidean subset is compact if and only if it is closed and bounded; continuous real functions on it attain extrema when it is compact. A closed subset of a compact metric space is compact. Compactness is intrinsic to the subspace topology and is preserved by continuous maps, including collar identifications and inclusions. [math:thm-euclidean-heine-borel-pseudocompactness-and-extreme-values](https://alphabetamath.cc/item/thm-euclidean-heine-borel-pseudocompactness-and-extreme-values) [math:lem-closed-subset-of-a-compact-space-is-compact](https://alphabetamath.cc/item/lem-closed-subset-of-a-compact-space-is-compact) [math:lem-compactness-is-intrinsic](https://alphabetamath.cc/item/lem-compactness-is-intrinsic) [math:thm-continuous-image-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-continuous-image-of-a-compact-space-is-compact)

[F5] The unit sphere $S^2$ is path-connected. Every path-connected space is connected. [math:cor-euclidean-spheres-are-path-connected](https://alphabetamath.cc/item/cor-euclidean-spheres-are-path-connected) [math:thm-path-connected-implies-connected](https://alphabetamath.cc/item/thm-path-connected-implies-connected)

[F6] For Euclidean open source and target models, a continuous map is proper exactly when the preimage of every compact target subset is compact in the source. A diffeomorphism is a bijective smooth map with smooth inverse; a smooth map is a local diffeomorphism when each source point has an open neighborhood mapped diffeomorphically onto an open target neighborhood. [math:def-proper-map-between-euclidean-open-sets](https://alphabetamath.cc/item/def-proper-map-between-euclidean-open-sets) [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

## Proof

**Given:** The geometric and graph data and complete hypotheses in the Statement, with the common radius chosen there.

**Goal:** Prove properness and finite covering of that fixed target collar without uniform candidate derivative bounds.

1.1 Fix a supplied candidate. In the reference interior $P_q$ is smooth and locally invertible by the spacelike graph hypothesis and F2. The set $U_q$ is open there because it is the inverse image of the open target collar. It is nonempty: fix $y\in S$ and take $0<\rho<\min(\rho_0,r_\delta/c_2)$; then $0<c_1\rho\le R_q(\rho,y)\le c_2\rho<r_\delta$. Via the specified identification $S\cong S^2$, use $(t,y)\mapsto t\,y$ to identify each positive radial collar with an open annulus in $\mathbb R^3$. Under these diffeomorphisms $U_q$ is a nonempty Euclidean open set and $P_q$ is a smooth local diffeomorphism. [given, F1, F2, F6]

2.1 Let $B\subset V_q$ be compact. The empty case has empty compact preimage, so assume $B\ne\varnothing$. Continuous inclusion of its annulus model into $\mathbb R^3$ preserves compactness, and the radial coordinate is continuous; F4 gives attained radial extrema $0<a\le b<r_\delta$. Every point of $P_q^{-1}(B)$ therefore has $a/c_2\le\rho\le b/c_1<\rho_0/2$. The closed reference subannulus $A=\{a/c_2\le\rho\le b/c_1\}\times S$ lies strictly inside the reference interior. Its Euclidean annulus model is closed and bounded, hence compact by F4, and the inverse collar identification preserves compactness. The target set $B$ is closed in the Euclidean target model by F4, so continuity of $P_q|_A$ makes $P_q^{-1}(B)$ closed in $A$. A closed subset of this compact metric space is compact; intrinsic compactness and continuous inclusion give compactness in $U_q$. This proves properness. The outer source boundary cannot contribute: at $\rho=\rho_0$ its target radius is at least $c_1\rho_0>2r_\delta$. [F1, F2, F4, F6, step 1.1]

3.1 The target annulus is path-connected: for $(r,y)$ and $(r',y')$ choose a continuous path $\gamma:[0,1]\to S^2$ joining $y$ to $y'$ by F5; then $t\mapsto((1-t)r+tr')\gamma(t)$ remains in that annulus and joins the corresponding points. It is connected by F5. The source is nonempty and the derivative is invertible by step 1.1; the map is proper by step 2.1, with compactness preserved by the collar diffeomorphisms in F4. All hypotheses of F3 now hold in dimension three. Thus $P_q$ is surjective and each target point has a neighborhood whose preimage is a finite disjoint union of diffeomorphic sheets. The same $r_\delta$ works for every candidate because only the background constants $c_1,c_2,\rho_0$ and common height bound determined it. Compactness and smoothness were used separately for each fixed candidate, so no uniform height derivatives or inverse-function radius were needed. [F3, F4, F5, F6, step 1.1, step 2.1] ∎

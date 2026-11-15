---
title: Spacelike normal projection is locally invertible with positive boundary jet
status: published
research_item: lem-author-840894718169-normal-projection-local-and-boundary-jets
dependency_level: 4
---

## Prerequisites

- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)
- [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [lem-author-840894718169-fixed-boundary-flow-normal-boost](item-lem-author-840894718169-fixed-boundary-flow-normal-boost)
- [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone)
- [math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)
- [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-compact-implies-the-other-compactness-forms](https://alphabetamath.cc/item/thm-compact-implies-the-other-compactness-forms)


## Statement

In the preceding Gaussian chart, suppose the candidate section is a smooth spacelike $K$-flow graph, with each height smooth up to $S$. Normal projection restricted to its interior is a local diffeomorphism. Parametrize the reference collar by $(\rho,y)$ using its unit boundary normal. The composite $P=\pi^\perp\circ\Phi$ has boundary value $P(0,y)=(0,y)$ and boundary derivative with radial coefficient $\cosh(\kappa u(0,y))>0$ and tangential identity; its radial image has no tangential first-order component. For each fixed candidate this gives a one-to-one boundary collar germ and covers a small target boundary collar. The widths in this last local assertion may depend on that candidate.

## Statement references

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[lem-author-840894718169-fixed-boundary-flow-normal-boost](item-lem-author-840894718169-fixed-boundary-flow-normal-boost)

[lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone)

[math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)

[math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

## Facts & Assumptions

[F1] Spacelike tangents contain no timelike vector. Flow graphs and their normals have the stated meanings. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[F2] The Gaussian fibres are timelike. In the Gaussian-collar convention, $\bar\nu$ points into the selected reference side and $\kappa$ is signed. The Gaussian-cone supplier's Proof, phase three, first step, proves the full normal-plane flow differential for every real $\kappa$, and the flow fixes $S$ pointwise with identity differential on $TS$. The fixed-boundary boost supplier uses the exterior normal and a positive rate; its convention is translated explicitly below. Flow-time differentiation gives the generating vector field. [lem-author-840894718169-fixed-boundary-flow-normal-boost](item-lem-author-840894718169-fixed-boundary-flow-normal-boost) [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F3] A smooth map with invertible differential has a local smooth inverse. [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

[F4] Smoothness at a boundary means that boundary-coordinate representatives admit smooth extensions to Euclidean-open neighborhoods. Apply this convention to the smooth height and hence to its composite with the smooth flow and Gaussian projection. [math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)

[F5] Differentials of smooth composites satisfy the chain rule. [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[F6] In the Gaussian-chart setting, $S$ is a compact smooth sphere. Fix a smooth identification $\chi:S\to S^2$ and equip $S$ with $d(y,z)=|\chi(y)-\chi(z)|$, the pullback of the Euclidean distance on the unit sphere. This metric induces its given topology, so $S$ is a compact metric space. Compactness gives finite subcovers, and the compact-metric theorem gives convergent subsequences, applied successively to two sequences in $S$. [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone) [math:thm-compact-implies-the-other-compactness-forms](https://alphabetamath.cc/item/thm-compact-implies-the-other-compactness-forms)

[A1] Use the ZFC convention already imposed by the Gaussian-chart supplier. The Axiom of Choice is used in the collision argument to select one distinct colliding pair for each positive integer if no injective source collar exists. Subsequence extraction then uses F6. [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The stated Gaussian chart, compact boundary $S$, and one smooth spacelike candidate flow graph with height smooth up to $S$.

**Goal:** Prove interior local invertibility, the boundary jet, and an individual injective boundary collar germ covering an individual target collar.

1.1 The kernel of $d\pi^\perp$ is the one-dimensional timelike Gaussian fibre direction. Its intersection with the candidate's positive-definite tangent three-plane is zero, so $d\pi^\perp$ restricted to that plane is an isomorphism onto the three-dimensional reference tangent space. By the flow-graph definition, the candidate graph map $\Phi$ is an embedding on the reference interior; thus $d\Phi$ identifies its tangent space with the candidate tangent plane. The chain rule gives $dP=d\pi^\perp\circ d\Phi$, an isomorphism. The inverse theorem proves both claimed interior local diffeomorphisms. [F1, F2, F3, F5]

1.2 Write $\bar\nu=\partial_\rho c(0,y)$ for the inward collar normal and $e=-\bar\nu$ for the exterior normal. The infinitesimal boost rate in $(\bar n,e)$ is $\lambda=-\kappa$. For $\kappa<0$ the positive-rate fixed-boundary supplier applies to $(K,e,\lambda)$; for $\kappa>0$ apply it to $(-K,e,\kappa)$ at time $-s$, using $\phi_{-s}^{-K}=\phi_s^K$. For the variable-time graph the latter replacement also changes $u$ to $-u$, leaving $\Phi$ unchanged and preserving its embedding and spacelikeness hypotheses. Thus both cases give $d\phi_s^K(e)=\cosh(\kappa s)e-\sinh(\kappa s)\bar n$, and hence $d\phi_s^K(\bar\nu)=\cosh(\kappa s)\bar\nu+\sinh(\kappa s)\bar n$, with no $TS$ component. For $\kappa=0$, the zero-rate differential calculation in F2's Gaussian-cone supplier, Proof, phase three, first step, gives the identity on the normal plane, so the same formula holds. In every case the differential is the identity on $TS$. The flow fixes $S$, so $P(0,y)=(0,y)$. By the chain rule, $d\Phi(X)=d\phi_{u(0,y)}^K(X)+du(X)K_y$ on $S$, and the last term vanishes since $K_y=0$. The Gaussian projection kills $\bar n$ and keeps reference tangent vectors. Consequently $dP_{(0,y)}(a,Y)=(\cosh(\kappa u(0,y))a,Y)$ for $Y\in T_yS$. This proves the positive radial coefficient, tangential identity and absence of a tangential first-order radial component. [F1, F2, F5, algebra]

2.1 Fix a boundary point and use source and target collar charts with nonnegative radial coordinate on the chosen side. By F4 the coordinate representative of $P$ has a smooth extension $f=(f_0,f')$ to a Euclidean-open neighborhood across the source boundary. On its boundary patch $f_0(0,z)=0$, while step 1.2 gives $\partial_r f_0(0,z_0)=\cosh(\kappa u(0,z_0))>0$ and an invertible full derivative. Shrink to a product neighborhood on which $\partial_r f_0>0$. Since $f_0(0,z)=0$, strict increase along each radial line shows that $f_0(r,z)$ has the same sign as $r$. Apply F3 to $f$ and shrink its inverse neighborhoods within this product neighborhood. The sign identity shows that this Euclidean inverse restricts bijectively to the two nonnegative half-neighborhoods, taking boundary to boundary and interior to interior. Its restriction and that of $f$ are smooth in the local-extension sense. This proves a smooth half-collar inverse near each boundary point. [F3, F4, step 1.2]

3.1 Fix the candidate. The union of the source inverse neighborhoods in step 2.1 is relatively open and contains $\{0\}\times S$. Product neighborhoods $[0,\varepsilon_y)\times V_y$ contained in that union cover the boundary; a finite subcover in F6 and the minimum of its finitely many positive widths give a source collar $[0,\varepsilon_0)\times S$. If no smaller source collar were injective, A1 selects, for each integer $j\ge1$, distinct colliding points $(r_j,y_j)$ and $(r'_j,y'_j)$ with $0\le r_j,r'_j<\min(\varepsilon_0/2,1/j)$. Apply F6 first to $(y_j)$ and then to $(y'_j)$ along that subsequence, giving a common subsequence with limits $y$ and $y'$. Continuity and the boundary identity in step 1.2 imply $(0,y)=(0,y')$, so $y=y'$. Both preimages then eventually lie in the same source inverse neighborhood from step 2.1, contradicting its injectivity. Thus some source collar is injective. Its image is a relative open neighborhood of the entire target boundary, using step 2.1 at boundary points and step 1.1 at interior points. For each target boundary point choose a product neighborhood contained in this image; a finite subcover of $S$ and the minimum of its positive widths give a positive-width target collar contained in the image. The local smooth inverses agree there by injectivity. This proves exactly the asserted individual collar germ and coverage; every shrinking may depend on the fixed candidate. [F6, A1, step 1.1, step 1.2, step 2.1] ∎

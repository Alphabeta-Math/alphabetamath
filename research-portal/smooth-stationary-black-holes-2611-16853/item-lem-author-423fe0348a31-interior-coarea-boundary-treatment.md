---
title: Removing the boundary before applying scalar coarea
status: draft
research_item: lem-author-423fe0348a31-interior-coarea-boundary-treatment
dependency_level: 5
sources:
  references:
    - title: Liviu I. Nicolaescu, The co-area formula (revision January 22, 2021)
      url: https://metaphor.ethz.ch/x/2021/fs/401-3462-00L/sc/extras/Nicolaescu.pdf
      locator: Theorem 5.3, p. 14, equation (5.1); Section 3, p. 8, definition and
        Example 3.1(a).
      statement: For a Lipschitz map F from a C1 Riemannian (n+k)-manifold X to a C1
        Riemannian k-manifold Y, the integral of JF over a measurable A equals
        the integral over Y of the normalized n-dimensional Hausdorff measures
        of A intersected with each fiber. Full-dimensional normalized Hausdorff
        measure equals Riemannian volume.
      hypotheses: Boundaryless manifolds, Riemannian length distances, a global
        Lipschitz constant, and a Hausdorff-measurable A. Hausdorff
        normalization is omega_s/2^s times the diameter-cover definition. Here X
        is an interior component, Y is the Euclidean real line, n=2, k=1, and A
        is a Borel height band.
      reading_limits: Consulted the stated theorem and equation, normalization
        definition, and Example 3.1(a). The published theorem's proof and its
        cited measure-identification proofs were not reconstructed. Boundary
        removal, distance comparison, and component summation are proved locally
        below.
---

## Prerequisites

- [lem-author-423fe0348a31-scalar-metric-jacobian](item-lem-author-423fe0348a31-scalar-metric-jacobian)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)
- [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)
- [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)
- [math:def-extended-riemannian-distance-on-a-disconnected-manifold](https://alphabetamath.cc/item/def-extended-riemannian-distance-on-a-disconnected-manifold)
- [math:thm-the-riemannian-distance-topology-is-the-manifold-topology](https://alphabetamath.cc/item/thm-the-riemannian-distance-topology-is-the-manifold-topology)
- [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)
- [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)
- [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing)
- [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)
- [math:def-hausdorff-measure](https://alphabetamath.cc/item/def-hausdorff-measure)
- [math:def-hausdorff-content-at-scale-delta](https://alphabetamath.cc/item/def-hausdorff-content-at-scale-delta)
- [math:thm-hausdorff-measure-is-metric-and-borel-measurable](https://alphabetamath.cc/item/thm-hausdorff-measure-is-metric-and-borel-measurable)
- [math:cor-positive-codimension-immersed-submanifolds-are-null](https://alphabetamath.cc/item/cor-positive-codimension-immersed-submanifolds-are-null)
- [math:cor-beppo-levi-theorem](https://alphabetamath.cc/item/cor-beppo-levi-theorem)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)
- [` Liviu I. Nicolaescu, The co-area formula (revision January 22, 2021) · Theorem 5.3, p. 14, equation (5.1); Section 3, p. 8, definition and Example 3.1(a). `](https://metaphor.ethz.ch/x/2021/fs/401-3462-00L/sc/extras/Nicolaescu.pdf)


## Statement

Work in ZFC. Let $(R,k)$ be a compact smooth Riemannian three-manifold with boundary $\partial R=B_-\cup B_+$. Let $u:R\to\mathbb R$ be Lipschitz for the intrinsic length distance $d_R$, and constant on neighborhoods of the two boundary parts with respective values $c_-$ and $c_+$, where $c_-<t<c_+$ for every $t$ in an interval $I$. Then $\partial R$ has zero three-dimensional Riemannian volume, and every level $\{u=t\}$ with $t\in I$ is a compact subset of $R^\circ$. On each connected component $C$ of $R^\circ$, the restriction of $u$ is Lipschitz for the intrinsic distance $d_C$. The boundaryless Lipschitz coarea theorem therefore applies componentwise on $R^\circ$; for bands with levels in $I$, neither its volume integral nor its level-area integral acquires a boundary contribution.

Here $d_R$ is the infimum of lengths of finite piecewise $C^1$ curves in $R$, including curves meeting its boundary; $d_C$ uses curves confined to $C$. Distances between different components of $R$ are $+\infty$, and all Hausdorff measures on $R$ are interpreted componentwise. Volume is the measure of the density $\sqrt{\det(k_{ij})}\,|dx^1dx^2dx^3|$, also in boundary charts. Cut area is normalized $\mathcal H^2=(\pi/4)\mathcal H^2_{\rm unnormalized}$, formed from the stated length distance. The measures formed with $d_R$ and $d_C$ agree on Borel subsets of $C$.

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice. Countable choice is used for the density-measure and Hausdorff-measure suppliers and countable localization. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The scalar coarea Jacobian equals the metric weak-gradient norm almost everywhere. [lem-author-423fe0348a31-scalar-metric-jacobian](item-lem-author-423fe0348a31-scalar-metric-jacobian)

[F2] The metric is smooth and positive definite up to the boundary. Curve length is the integral of metric speed; connected-component distances are infima of those lengths, with $+\infty$ between different components. These distances induce the manifold topology, including at boundary points. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length) [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold) [math:def-extended-riemannian-distance-on-a-disconnected-manifold](https://alphabetamath.cc/item/def-extended-riemannian-distance-on-a-disconnected-manifold) [math:thm-the-riemannian-distance-topology-is-the-manifold-topology](https://alphabetamath.cc/item/thm-the-riemannian-distance-topology-is-the-manifold-topology)

[F3] Lipschitz heights and normalized Hausdorff areas are measured with the fixed metric. [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[F4] In a boundary chart the boundary is in the coordinate hyperplane. On a compact coordinate set there are $0<a\le b<\infty$ such that $a|v|\le |v|_k\le b|v|$. [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

[F5] The Riemannian volume density has coordinate coefficient $\sqrt{\det(k_{ij})}$. Its measure restricted to any Borel subset of any chart is the integral of that coefficient; the gluing theorem explicitly allows boundary charts and assumes countable choice. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing)

[F6] The plane $\mathbb R^2\times\{0\}$ is a positive-codimension smooth submanifold of $\mathbb R^3$, so it is Lebesgue null under countable choice. [math:cor-positive-codimension-immersed-submanifolds-are-null](https://alphabetamath.cc/item/cor-positive-codimension-immersed-submanifolds-are-null)

[F7] Hausdorff measure is obtained from countable diameter covers as their scale tends to zero. Under countable choice it measures every Borel set and is countably additive there. The library definitions are unnormalized; multiplication by $\pi/4$ gives the two-dimensional normalization used here and preserves these properties. [math:def-hausdorff-content-at-scale-delta](https://alphabetamath.cc/item/def-hausdorff-content-at-scale-delta) [math:def-hausdorff-measure](https://alphabetamath.cc/item/def-hausdorff-measure) [math:thm-hausdorff-measure-is-metric-and-borel-measurable](https://alphabetamath.cc/item/thm-hausdorff-measure-is-metric-and-borel-measurable)

[F8] Nonnegative integrals commute with countable nonnegative sums, including infinite values. [math:cor-beppo-levi-theorem](https://alphabetamath.cc/item/cor-beppo-levi-theorem)

[F9] The independent coarea input, with its exact scope, is recorded in External input below. It supplies a theorem on boundaryless manifolds, not a theorem on regions with boundary.

[F10] A closed subset of a compact space is compact. [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

## Proof

**Given:** The region, height, boundary constants, and interval in the Statement.

**Goal:** Justify boundary removal for coarea, including its metric and measure conventions.

1.1 The boundary is Borel: in the half-space charts its complement is open. Each boundary-chart image of $\partial R$ lies in a Lebesgue-null coordinate plane by [F4] and [F6]. Its volume is therefore zero by the chart formula [F5]; a finite chart cover of the compact region gives $V_k(\partial R)=0$. By [F2] the Lipschitz function $u$ is continuous in the manifold topology. Since the boundary constants lie outside $I$, the closed level $E_t=\{u=t\}$ misses the boundary for $t\in I$, and [F10] makes it compact. [given, A1, F2, F4, F5, F6, F10]

1.2 Let $C$ be any interior component. Every curve confined to $C$ is a curve in $R$, so $d_R(x,y)\le d_C(x,y)$ for $x,y\in C$. If $L$ is the given Lipschitz constant, then $|u(x)-u(y)|\le Ld_R(x,y)\le Ld_C(x,y)$. Thus $u|_C$ satisfies the global Lipschitz hypothesis of the boundaryless theorem; completeness of $C$ is not required by that theorem. [given, F2, F9]

2.1 Fix an interior point $p\in C$ and choose coordinates centered at $p$ with the closed Euclidean ball $\overline B_r$ inside the chart and inside $C$. Use [F4] on this compact set and choose $0<\varepsilon<r$ with $2b\varepsilon<a(r-\varepsilon)$. For any $y,z$ with coordinates in $B_\varepsilon$, the coordinate segment between them has metric length at most $2b\varepsilon$. Any curve in $R$ from $y$ to $z$ that leaves the coordinate ball $B_r$ has an initial segment reaching its sphere; its length is at least $a(r-\varepsilon)$, since Euclidean curve length bounds endpoint displacement. Hence such curves cannot lower the infimum below the segment bound, and $d_R(y,z)$ equals the infimum over curves confined to $B_r$. As these curves are also confined to $C$, step 1.2 yields $d_R(y,z)\le d_C(y,z)\le d_R(y,z)$. Thus the two distances agree on the neighborhood $B_\varepsilon$. This argument uses infima and does not assume existence of minimizing curves. [given, F2, F4, step 1.2, choose, algebra]

2.2 Fix a Borel interval $J\subset I$ and put $A=\{x\in R:u(x)\in J\}$. It is Borel by continuity, and step 1.1 gives $A\subset R^\circ$. For each interior component $C$, apply [F9] to $X=C$, $Y=\mathbb R$ with its Euclidean metric, $F=u|_C$, $n=2$, $k=1$, and the Borel set $A\cap C$. Its Lipschitz hypothesis is step 1.2. The source normalization identifies full-dimensional Hausdorff measure with $dV_k$ and target measure with $dt$. By [F1] and [F3] its Jacobian is $|\nabla_k u|$ almost everywhere. The resulting identity is $\int_{A\cap C}|\nabla_k u|\,dV_k=\int_J\mathcal H^2_{d_C}(C\cap E_t)\,dt$, with nonnegative extended integrals. [given, F1, F3, F9, step 1.1, step 1.2]

3.1 For a subset of one of the neighborhoods in step 2.1, intersect every Hausdorff covering set with that neighborhood and discard empty intersections. This does not increase diameters, so Hausdorff outer measure equals the one computed within the neighborhood. The restricted distances agree there; therefore the two normalized Hausdorff outer measures agree on every such subset. Second countability supplies a countable cover $(U_j)$ by these neighborhoods: take a countable basis refinement and choose a containing neighborhood for each selected basis element, using [A1]. Partition $C$ into the Borel sets $P_j=U_j\setminus\bigcup_{i<j}U_i$. For a Borel $E\subset C$, [F7] gives equality of the two measures of $E$ by summing their equal values on $E\cap P_j$. The Borel domains agree by [F2]. Interior components are open, because coordinate balls are connected; they are countably many, since disjoint nonempty open sets contain different members of a countable basis. Consequently the $d_R$-area of any Borel interior set is the sum of its $d_C$-areas over those components. [A1, F2, F7, step 2.1, construct]

4.1 Sum the identities in step 2.2 over the countably many interior components. The coarea input [F9] supplies measurable fiber-area functions, and [F8] interchanges their nonnegative sum with the $t$-integral. Step 3.1 identifies the sum of component areas with $\mathcal H^2_{d_R}(E_t)$ for $t\in J$. Thus $\int_A|\nabla_k u|\,dV_k=\int_J\mathcal H^2_{d_R}(E_t)\,dt$. On the volume side the density measure on the interior is the restriction of the measure on $R$ by [F5], and the removed boundary is null by step 1.1; on the level side $E_t\subset R^\circ$ and step 3.1 gives agreement of the Hausdorff areas. This proves the claimed absence of boundary contributions. [F5, F8, F9, step 1.1, step 3.1, step 2.2] ∎

## External input

Theorem 5.3 of Nicolaescu gives $\int_A JF\,d\mathcal H_X^{n+k}=\int_Y\mathcal H_X^n(A\cap F^{-1}(y))\,d\mathcal H_Y^k(y)$ for a Lipschitz map between boundaryless $C^1$ Riemannian manifolds of dimensions $n+k$ and $k$, and a measurable $A$. Section 3 defines the normalization $\omega_s/2^s$ for diameter covers; Example 3.1(a) identifies full-dimensional measure with Riemannian volume. The source supplies this established theorem; the local proof above checks its hypotheses and transfers the formula from interior components to the region. See the precise citation and reading limits in sources.references.

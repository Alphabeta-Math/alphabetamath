---
title: Admissible domains for outward normal graphs
status: published
research_item: lem-author-c50357f4fa9e-normal-graph-domain
dependency_level: 0
---

## Prerequisites

- [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)
- [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry)
- [math:def-domain-and-exponential-map-of-a-connection](https://alphabetamath.cc/item/def-domain-and-exponential-map-of-a-connection)
- [math:thm-existence-uniqueness-and-smooth-dependence-of-geodesics](https://alphabetamath.cc/item/thm-existence-uniqueness-and-smooth-dependence-of-geodesics)
- [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)
- [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)
- [math:lem-slice-chart-restrictions-form-a-smooth-atlas](https://alphabetamath.cc/item/lem-slice-chart-restrictions-form-a-smooth-atlas)
- [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)
- [math:prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)


## Statement

Assume countable choice $\mathrm{AC}_\omega$, as in the geodesic suppliers. Let $\Sigma$ be a smooth spacelike hypersurface of a time-oriented smooth Lorentzian four-manifold, let $h=g|_{T\Sigma}$, and let $S\subset\operatorname{int}\Sigma$ be a smooth embedded two-surface without boundary carrying a supplied smooth $h$-unit normal $\nu$ in $\Sigma$. Write $D$ for the Levi–Civita connection of $h$. On the open domain where it exists set $T(p,r)=\exp^h_p(r\nu_p)$. Near each $(p,0)$, $T$ is a diffeomorphism onto an open subset of $\Sigma$, and $dT_{(p,0)}(X,a)=X+a\nu_p$.

If $S$ is compact there is $\rho>0$ such that $T:S\times(-\rho,\rho)\to\Sigma$ is a diffeomorphism onto its image. In either a local domain or this compact tube, fix an open domain $\Omega\subset S\times\mathbb R$ containing the relevant zero section on which $T$ is a diffeomorphism. A smooth function $u$ is **admissible** precisely when its graph lies in $\Omega$; then $F_u(p)=T(p,u(p))$ is an embedded spacelike surface parametrization. No uniform graph radius is asserted for a noncompact $S$ without a supplied tube. Each smooth compactly supported $\phi$ admits $u=\epsilon\phi$ for all sufficiently small $|\epsilon|$ whenever such a tube is supplied; the same holds for every smooth $\phi$ on compact $S$.

## Facts & Assumptions

[F1] The hypersurface supplier [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form) supplies the smooth positive metric $h$; [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry) supplies its unique Levi–Civita connection.

[F2] [math:def-domain-and-exponential-map-of-a-connection](https://alphabetamath.cc/item/def-domain-and-exponential-map-of-a-connection) defines the exponential only where the geodesic exists through time one. Under its countable-choice hypothesis, [math:thm-existence-uniqueness-and-smooth-dependence-of-geodesics](https://alphabetamath.cc/item/thm-existence-uniqueness-and-smooth-dependence-of-geodesics) supplies the open geodesic evaluation domain and smooth dependence.

[F3] [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds) turns an invertible differential into a smooth local inverse.

[F4] An embedded surface is understood in the slice-chart sense of [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart). The restricted slice charts supply its smooth structure and subspace topology by [math:lem-slice-chart-restrictions-form-a-smooth-atlas](https://alphabetamath.cc/item/lem-slice-chart-restrictions-form-a-smooth-atlas).

[F5] [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure) supplies the product topology and product smooth charts on $S\times\mathbb R$ and its open subdomains.

[F6] Countable choice is the principle in [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice): from each member of an $\mathbb N$-indexed family of nonempty sets one may choose one element. It is assumed here.

[F7] A smooth embedding is an injective smooth immersion that is a homeomorphism onto its image with the subspace topology, as defined in [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding). By [math:prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold), its image is an embedded submanifold and its corestriction to that image is a diffeomorphism.

[F8] The time-oriented smooth Lorentzian four-manifold is the mathematical structure of [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects), clauses (a)–(c). A spacelike hypersurface means an embedded three-submanifold on whose tangent spaces $g$ is positive definite, as in [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets), clause (a). Here an embedded two-surface is called spacelike precisely when the restriction of $g$ to each of its tangent planes is positive definite.

## Proof

**Given:**The structures and countable-choice hypothesis of the Statement.

**Goal:** Establish the stated graph domains and admissible deformations.

1.1 In the restricted and ambient slice coordinates from [F4], the inclusion of $S$ is $x\mapsto(x,0)$; it is therefore smooth with injective differential and identifies $T_pS$ with a two-dimensional subspace of $T_p\Sigma$. In the product charts from [F5], the base projection is smooth and $T_{(p,0)}(S\times\mathbb R)=T_pS\oplus\mathbb R$. In these structures the map $(p,r)\mapsto r\nu_p$ is smooth. Pulling back the open time-one domain in [F2] gives an open domain for $T$ containing every $(p,0)$. The constant geodesic gives $T(p,0)=p$. Uniqueness of geodesics, applied to the reparametrization $t\mapsto\gamma_{p,\nu_p}(rt)$ near $r=0$, gives $T(p,r)=\gamma_{p,\nu_p}(r)$ there, so $\partial_rT(p,0)=\nu_p$. Differentiating the identity on $S$ gives $dT(X,0)=X$. Since $T_p\Sigma=T_pS\oplus\mathbb R\nu_p$, this differential is invertible. The local conclusion follows from [F3]. [F1, F2, F3, F4, F5, given]

2.1 Suppose $S$ is compact. The open domain of definition and the open local-diffeomorphism locus contain the compact zero section, so finitely many product neighborhoods give one $\rho_0>0$ on which $T$ is defined and locally invertible. If no shrinking were injective, for each integer $j$ there would be distinct $(p_j,r_j),(q_j,s_j)$ with $|r_j|,|s_j|<\min(\rho_0,1/j)$ and equal images. Compactness gives a subsequence with $p_j\to p$ and $q_j\to q$. Continuity and the Hausdorff property imply $p=q$, since the common images converge to both $p$ and $q$. Both pairs then lie in a single local inverse neighborhood of $(p,0)$ for large $j$, contradicting injectivity there. Thus a smaller $\rho$ makes $T$ injective; its local inverses agree and yield a smooth inverse on its open image. The pairs are chosen from the fixed nonempty counterexample sets indexed by $j$, using countable choice in [F6]. [F3, F4, F5, F6, step 1.1, given]

3.1 The graph map $p\mapsto(p,u(p))$ is a smooth embedding into $\Omega$ in the sense of [F7]: it is smooth and injective, its inverse on its image is the base projection, and its differential has identity base component. Composition with the diffeomorphism $T$ preserves these properties. By [F7], $F_u(S)$ is an embedded two-submanifold of $\Sigma$ and $F_u:S\to F_u(S)$ is a diffeomorphism. For every nonzero $V\in T_xF_u(S)\subset T_x\Sigma$, $g_x(V,V)=h_x(V,V)>0$ by [F1]; hence the graph is spacelike by the tangent-plane criterion in [F8]. For compact support $K$, finitely many product neighborhoods of $K\times\{0\}$ give a positive radius $\eta$ contained in $\Omega$ above $K$. The finite maximum $M=\max_K|\phi|$ exists. Taking $|\epsilon|M<\eta$ keeps the graph in $\Omega$; off $K$ it is the zero section. For compact $S$ use $K=S$. The case $M=0$ is immediate. This proves all assertions without a completeness hypothesis on $\Sigma$. [step 1.1, step 2.1, F1, F4, F5, F7, F8] ∎

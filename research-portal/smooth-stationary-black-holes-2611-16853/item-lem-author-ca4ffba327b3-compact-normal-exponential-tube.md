---
title: A compact spacelike surface has a normal exponential tube
status: published
research_item: lem-author-ca4ffba327b3-compact-normal-exponential-tube
dependency_level: 1
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)
- [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)
- [math:lem-slice-chart-restrictions-form-a-smooth-atlas](https://alphabetamath.cc/item/lem-slice-chart-restrictions-form-a-smooth-atlas)
- [physics:def-lorentz-orthogonality-and-orthogonal-complement](https://alphabetamath.cc/physics/item/def-lorentz-orthogonality-and-orthogonal-complement)
- [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)
- [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)
- [math:thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary](https://alphabetamath.cc/item/thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary)
- [math:def-inward-outward-and-boundary-tangent-vectors](https://alphabetamath.cc/item/def-inward-outward-and-boundary-tangent-vectors)
- [math:lem-tube-lemma-for-a-compact-factor](https://alphabetamath.cc/item/lem-tube-lemma-for-a-compact-factor)
- [math:thm-topological-manifolds-are-metrizable-and-paracompact](https://alphabetamath.cc/item/thm-topological-manifolds-are-metrizable-and-paracompact)
- [math:thm-compact-implies-the-other-compactness-forms](https://alphabetamath.cc/item/thm-compact-implies-the-other-compactness-forms)


## Statement

Work in ZFC. Let $S$ be a compact embedded spacelike two-surface in a smooth time-oriented Lorentzian four-manifold $(M,g,N)$ without boundary, with signature $(-,+,+,+)$. Here spacelike means that $g|_{T_sS}$ is positive definite, and the normal plane bundle has fibers $N_sS=(T_sS)^{\perp_g}$. Suppose it has a supplied smooth orthonormal frame $(n,\nu)$: these are smooth normal fields with $g(n,n)=-1$, $g(\nu,\nu)=1$, $g(n,\nu)=0$, and $g(n,N)<0$. For some $\epsilon>0$, $\Xi(s,a,b)=\exp_s(a n_s+b\nu_s)$ is a diffeomorphism from $S\times\{(a,b):|a|+|b|<\epsilon\}$ onto an open neighborhood $O$ of $S$. Its normal radial curves $r\mapsto\Xi(s,ra,rb)$ stay in $O$ for $0\le r\le1$.

The frame hypothesis holds when $S$ is a two-sided boundary in a smooth embedded spacelike hypersurface, using its future unit normal and its inward unit boundary normal. For this assertion, the specified side near $S$ is a smooth embedded three-manifold $\Sigma_+$ with boundary $S$ and with $h=g|_{T\Sigma_+}$ positive definite up to the boundary; inward is the direction of increasing last coordinate in a boundary chart. A two-sided embedded surface in a hypersurface with a specified smooth side is included by restricting to that side. The Lorentzian and future-direction conventions are those stated here; no Killing field is required.

## Statement references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

[math:lem-slice-chart-restrictions-form-a-smooth-atlas](https://alphabetamath.cc/item/lem-slice-chart-restrictions-form-a-smooth-atlas)

[physics:def-lorentz-orthogonality-and-orthogonal-complement](https://alphabetamath.cc/physics/item/def-lorentz-orthogonality-and-orthogonal-complement)

[math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)

[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[math:thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary](https://alphabetamath.cc/item/thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary)

[math:def-inward-outward-and-boundary-tangent-vectors](https://alphabetamath.cc/item/def-inward-outward-and-boundary-tangent-vectors)

[math:lem-tube-lemma-for-a-compact-factor](https://alphabetamath.cc/item/lem-tube-lemma-for-a-compact-factor)

[math:thm-topological-manifolds-are-metrizable-and-paracompact](https://alphabetamath.cc/item/thm-topological-manifolds-are-metrizable-and-paracompact)

[math:thm-compact-implies-the-other-compactness-forms](https://alphabetamath.cc/item/thm-compact-implies-the-other-compactness-forms)

## Facts & Assumptions

[F1] The joint geodesic evaluation is smooth on an open domain; the exponential map is defined near all zero vectors, satisfies $\exp_s(0)=s$ and has identity vertical derivative at zero. Its scaling law identifies $\exp_s(rv)$ with the geodesic of initial velocity $v$ at parameter $r$. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F2] A smooth map whose differential is an isomorphism at a point restricts to a diffeomorphism between open neighborhoods of that point and its image. [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

[F3] Use the smooth-manifold, Lorentzian metric and time-orientation conventions, and ZFC including Choice. Choice is used for the metrization supplier and, in the injectivity contradiction, to select a collision at each radius. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F4] An embedded surface has slice charts and the subspace topology. The restricted slice charts form a smoothly compatible atlas inducing that topology. Lorentz-orthogonality means $g(v,w)=0$, and the orthogonal complement consists of vectors orthogonal to every tangent vector. Spacelikeness and a smooth normal frame have the explicit meanings in the Statement; the splitting used below is proved in step 1.1. [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart) [math:lem-slice-chart-restrictions-form-a-smooth-atlas](https://alphabetamath.cc/item/lem-slice-chart-restrictions-form-a-smooth-atlas) [physics:def-lorentz-orthogonality-and-orthogonal-complement](https://alphabetamath.cc/physics/item/def-lorentz-orthogonality-and-orthogonal-complement)

[F5] Smooth embedded manifolds with boundary have boundary charts with smooth local extensions of coordinate expressions and full-dimensional tangent and cotangent bundles at boundary points. The sign of the last coordinate of a tangent vector specifies inwardness independently of the chart. [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary) [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary](https://alphabetamath.cc/item/thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary) [math:def-inward-outward-and-boundary-tangent-vectors](https://alphabetamath.cc/item/def-inward-outward-and-boundary-tangent-vectors)

[F6] If an open subset of $X\times Z$ contains $K\times\{z_0\}$ with $K$ compact, it contains $K\times W$ for an open neighborhood $W$ of $z_0$. [math:lem-tube-lemma-for-a-compact-factor](https://alphabetamath.cc/item/lem-tube-lemma-for-a-compact-factor)

[F7] Under the stated Choice convention a topological manifold is metrizable. In a compact metric space every sequence has a convergent subsequence, by compactness implying countable compactness and then sequential compactness. [math:thm-topological-manifolds-are-metrizable-and-paracompact](https://alphabetamath.cc/item/thm-topological-manifolds-are-metrizable-and-paracompact) [math:thm-compact-implies-the-other-compactness-forms](https://alphabetamath.cc/item/thm-compact-implies-the-other-compactness-forms)

## Proof

**Given:** The data and hypotheses of the Statement, including ZFC.

**Goal:** Establish the uniform tube, its radial property, and the boundary-frame assertion.

1.1 In a surface slice chart let $E_1,E_2$ be its smooth tangent basis and put $G_{ij}=g(E_i,E_j)$. Positivity makes $G$ invertible. Define $PV=\sum_{i,j=1}^2 E_i(G^{-1})^{ij}g(E_j,V)$. Then $P$ is smooth, $P|_{TS}$ is the identity, and $g(V-PV,E_i)=0$. Thus $TM|_S=TS\oplus\ker P$, with $\ker P=NS$ of rank two; this also gives the smooth normal bundle since the projections agree on chart overlaps by uniqueness. The supplied $n,\nu$ are linearly independent by their displayed inner products, so span $NS$. [given, F3, F4, algebra]

2.1 By the joint smoothness in [F1] and the smooth supplied frame, $\Xi$ is smooth on an open subset of $S\times\mathbb R^2$ containing its zero section. Since $\Xi(s,0,0)=s$ and its vertical differential is the identity on normal vectors, its differential there is $(X,u,v)\mapsto X+un_s+v\nu_s$. Step 1.1 makes this an isomorphism. In local charts the determinant of this differential is continuous, so the locus $U$ where $\Xi$ is defined and its differential invertible is open and contains $S\times\{(0,0)\}$. By [F2], $\Xi$ is a local diffeomorphism throughout $U$. [F1, F2, F4, step 1.1]

2.2 For the boundary assertion use the full three-dimensional tangent spaces of $\Sigma_+$, including at $S$. In a boundary chart their basis $E_1,E_2,E_3$ is smooth up to the boundary. With $H_{ij}=g(E_i,E_j)$, the same formula as in step 1.1, now summed from $1$ to $3$, defines the unique smooth orthogonal projection $P_\Sigma$ onto $T\Sigma_+$. Write $w=N-P_\Sigma N$. Orthogonality gives $g(w,w)=g(N,N)-g(P_\Sigma N,P_\Sigma N)<0$ and $g(w,N)=g(w,w)<0$. Thus $n=w/\sqrt{-g(w,w)}$ is the future unit normal, smooth up to $S$. The projection is intrinsic, so these formulas agree on overlaps. Inverse Gram matrices are smooth since their determinants are nonzero, using the adjugate formula. This construction uses only boundary tangent bundles and requires no extension of the hypersurface through its boundary. [given, F3, F4, F5, step 1.1, algebra]

3.1 Apply [F6] with $X=K=S$, $Z=\mathbb R^2$, $z_0=(0,0)$ and $N=U$. It supplies an open $W$ about $(0,0)$ with $S\times W\subset U$. Choose $\epsilon_0>0$ so that $D_{\epsilon_0}=\{(a,b):|a|+|b|<\epsilon_0\}\subset W$. Thus $\Xi$ is defined and is a local diffeomorphism on the entire uniform domain $S\times D_{\epsilon_0}$. [given, F6, step 2.1]

4.1 The surface $S$, with its slice-chart smooth structure and subspace topology, is a topological manifold. Apply [F7] under [F3] to give $S$ a compatible metric; its assumed topological compactness is compactness for that metric. Suppose no radius smaller than $\epsilon_0$ makes $\Xi$ injective. Using Choice, for each integer $k\ge1$ select unequal data $(s_k,a_k,b_k)$ and $(s_k^{\prime},a_k^{\prime},b_k^{\prime})$ in $S\times D_{\epsilon_0/(k+1)}$ with the same image. Sequential compactness first gives a subsequence with $s_k\to s$ and then a further subsequence with $s_k^{\prime}\to s^{\prime}$. Along it all four fiber coordinates tend to zero. Continuity and $\Xi(s,0,0)=s$ show that the common images tend to both $s$ and $s^{\prime}$ in the Hausdorff manifold $M$, so $s=s^{\prime}$. Both data sequences therefore eventually lie in one inverse-function neighborhood of $(s,0,0)$ from step 2.1, contradicting its injectivity. Hence some $0<\epsilon<\epsilon_0$ gives injectivity on $S\times D_\epsilon$. [given, F2, F3, F4, F7, step 2.1, step 3.1]

5.1 A local diffeomorphism is open, because its local restrictions have open images. Hence the injective restriction from step 4.1 has open image $O$ containing $S$; its local smooth inverses agree by injectivity and give its smooth global inverse on $O$. If $(a,b)\in D_\epsilon$ and $0\le r\le1$, then $(ra,rb)\in D_\epsilon$. The scaling law in [F1] therefore identifies the entire normal radial geodesic segment with $r\mapsto\Xi(s,ra,rb)$ in $O$. [F1, F2, step 3.1, step 4.1]

6.1 In each boundary chart of $\Sigma_+$ put $\rho=x^3\ge0$, so $S$ is $\rho=0$ locally and $d\rho\ne0$ there. Set $q=\sum_{i,j=1}^3 E_i(H^{-1})^{ij}d\rho(E_j)$; then $h(q,V)=d\rho(V)$ for every $V\in T\Sigma_+$. The smooth vector $q$ is nonzero, is orthogonal to $TS$, and satisfies $d\rho(q)=h(q,q)>0$. Consequently $\nu=q/\sqrt{h(q,q)}$ along $S$ is the smooth inward unit boundary normal. On overlaps it agrees because the orthogonal line to $TS$ in the positive definite space $T\Sigma_+$ has exactly one inward unit vector, with inwardness chart independent by [F5]. Since $n\perp T\Sigma_+$, one has $g(n,\nu)=0$. Both fields are normal to $S$, so step 1.1 shows they form the required smooth orthonormal normal frame. Together with step 5.1 this proves every assertion. [given, F4, F5, step 1.1, step 5.1, step 2.2, algebra] ∎

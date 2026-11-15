---
title: Extending normalized end coordinates while preserving the section
status: draft
research_item: lem-author-d20d145f998f-cutoff-end-coordinate-extension
dependency_level: 2
---

## Prerequisites

- [lem-author-d20d145f998f-normalized-stationary-end](item-lem-author-d20d145f998f-normalized-stationary-end)
- [lem-author-d20d145f998f-decaying-time-gauge](item-lem-author-d20d145f998f-decaying-time-gauge)
- [lem-author-d20d145f998f-bounded-stationary-graph](item-lem-author-d20d145f998f-bounded-stationary-graph)
- [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)
- [lem-author-d20d145f998f-stationary-product-cauchy-time](item-lem-author-d20d145f998f-stationary-product-cauchy-time)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry)
- [math:prop-christoffel-formula-for-the-levi-civita-connection](https://alphabetamath.cc/item/prop-christoffel-formula-for-the-levi-civita-connection)
- [math:thm-christoffel-symbol-transformation-law](https://alphabetamath.cc/item/thm-christoffel-symbol-transformation-law)
- [math:lem-shin-radial-smooth-cutoff](https://alphabetamath.cc/item/lem-shin-radial-smooth-cutoff)
- [math:thm-extreme-value-r](https://alphabetamath.cc/item/thm-extreme-value-r)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)
- [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)
- [math:thm-monotonicity-of-the-integral](https://alphabetamath.cc/item/thm-monotonicity-of-the-integral)
- [math:thm-cauchy-criterion-for-improper-integrals](https://alphabetamath.cc/item/thm-cauchy-criterion-for-improper-integrals)
- [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)
- [math:thm-path-connected-implies-connected](https://alphabetamath.cc/item/thm-path-connected-implies-connected)
- [math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets](https://alphabetamath.cc/item/thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)
- [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)
- [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)
- [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-pullback-riemannian-metric](https://alphabetamath.cc/item/def-pullback-riemannian-metric)
- [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)
- [math:def-ck-euclidean-maps-and-diffeomorphisms](https://alphabetamath.cc/item/def-ck-euclidean-maps-and-diffeomorphisms)
- [math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold)
- [math:def-christoffel-symbols-of-an-affine-connection](https://alphabetamath.cc/item/def-christoffel-symbols-of-an-affine-connection)
- [math:def-levi-civita-connection](https://alphabetamath.cc/item/def-levi-civita-connection)
- [math:def-euclidean-inner-product](https://alphabetamath.cc/item/def-euclidean-inner-product)
- [math:def-euclidean-spheres-and-closed-balls](https://alphabetamath.cc/item/def-euclidean-spheres-and-closed-balls)
- [math:def-cross-product-in-r3](https://alphabetamath.cc/item/def-cross-product-in-r3)
- [math:def-linear-isometry-and-orthogonal-or-unitary-operator](https://alphabetamath.cc/item/def-linear-isometry-and-orthogonal-or-unitary-operator)
- [math:def-connected-space](https://alphabetamath.cc/item/def-connected-space)
- [math:def-proper-map-between-euclidean-open-sets](https://alphabetamath.cc/item/def-proper-map-between-euclidean-open-sets)
- [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)


## Statement

Work in ZFC. Let a connected time-oriented Lorentzian exterior have the supplied stationary Cauchy product $\Psi:\mathbb R\times C\to E$, with complete Killing flow, $C$ spacelike Cauchy, $-g(T,n)>0$, and product time $t$. Supply a smooth embedded section extension $\Sigma_0$ in an ambient smooth extension of $E$, with $\Sigma_0\cap E=C$, and a diffeomorphism $x:\Sigma_0\to\{x\in\mathbb R^3:|x|>1/2\}$ agreeing with the original asymptotic spatial chart, with $C=\{r>1\}$ and $S_0=\{r=1\}$ in that extension. Thus $S_0$ is the explicitly specified inner boundary of $C$ in $\Sigma_0$. Take the original end $t=0$ and the normalized stationary chart $(t',y)$ of the end-normalization lemma, including its original $O_6$ metric hypotheses and positive mass. Their transition is $y=f(x)$, $t'=t+F(x)$.

One may apply a constant orthogonal change $y\mapsto Ay$, allowing a reflection, and an additive change of the time origin. The normalized metric estimates are preserved; its spin coefficient changes to $S_A=(\det A)AS$, with $|S_A|=|S|$, in the same ADM sign and flux convention. After this choice, rename the spatial chart $y$ and its transition $f$. Then $f=x+O(\log r)$, $Df=I+O(r^{-1})$, $D^j f=O(r^{-j})$ for $2\le j\le7$, with the corresponding inverse-chart bounds, and $F=O(r^{-1})$, $dF=O_6(r^{-2})$.

For sufficiently large $R$ the spatial change has a smooth cutoff to a global diffeomorphism of $\{r>1/2\}$ equal to the identity on $r\le R$ and to $f$ on $r\ge2R$. There is a smooth bounded time cutoff $u_R$, zero on $r\le R$ and equal to $F$ on $r\ge2R$, with $\sup|u_R|=O(R^{-1})$ and $\sup|du_R|=O(R^{-2})$. The section $C'=\{\Psi(-u_R(p),p):p\in C\}$ is smooth, spacelike and Cauchy, with a smooth ambient section extension equal to $\Sigma_0$ near $S_0$. In particular it agrees with the original near its bifurcation sphere whenever that supplied sphere is $S_0$. It is $t'=0$ in the normalized end. Its global spatial parameter chart extends across $S_0$, fixes that sphere and agrees with the orthogonally adjusted $y$ sufficiently far out. No preservation of maximality of $C'$ is asserted.

## Statement references

[lem-author-d20d145f998f-normalized-stationary-end](item-lem-author-d20d145f998f-normalized-stationary-end)

[lem-author-d20d145f998f-decaying-time-gauge](item-lem-author-d20d145f998f-decaying-time-gauge)

[lem-author-d20d145f998f-bounded-stationary-graph](item-lem-author-d20d145f998f-bounded-stationary-graph)

[math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

[lem-author-d20d145f998f-stationary-product-cauchy-time](item-lem-author-d20d145f998f-stationary-product-cauchy-time)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry)

[math:prop-christoffel-formula-for-the-levi-civita-connection](https://alphabetamath.cc/item/prop-christoffel-formula-for-the-levi-civita-connection)

[math:thm-christoffel-symbol-transformation-law](https://alphabetamath.cc/item/thm-christoffel-symbol-transformation-law)

[math:lem-shin-radial-smooth-cutoff](https://alphabetamath.cc/item/lem-shin-radial-smooth-cutoff)

[math:thm-extreme-value-r](https://alphabetamath.cc/item/thm-extreme-value-r)

[math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)

[math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)

[math:thm-monotonicity-of-the-integral](https://alphabetamath.cc/item/thm-monotonicity-of-the-integral)

[math:thm-cauchy-criterion-for-improper-integrals](https://alphabetamath.cc/item/thm-cauchy-criterion-for-improper-integrals)

[math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)

[math:thm-path-connected-implies-connected](https://alphabetamath.cc/item/thm-path-connected-implies-connected)

[math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets](https://alphabetamath.cc/item/thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets)

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[math:def-pullback-riemannian-metric](https://alphabetamath.cc/item/def-pullback-riemannian-metric)

[math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

[math:def-ck-euclidean-maps-and-diffeomorphisms](https://alphabetamath.cc/item/def-ck-euclidean-maps-and-diffeomorphisms)

[math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold)

[math:def-christoffel-symbols-of-an-affine-connection](https://alphabetamath.cc/item/def-christoffel-symbols-of-an-affine-connection)

[math:def-levi-civita-connection](https://alphabetamath.cc/item/def-levi-civita-connection)

[math:def-euclidean-inner-product](https://alphabetamath.cc/item/def-euclidean-inner-product)

[math:def-euclidean-spheres-and-closed-balls](https://alphabetamath.cc/item/def-euclidean-spheres-and-closed-balls)

[math:def-cross-product-in-r3](https://alphabetamath.cc/item/def-cross-product-in-r3)

[math:def-linear-isometry-and-orthogonal-or-unitary-operator](https://alphabetamath.cc/item/def-linear-isometry-and-orthogonal-or-unitary-operator)

[math:def-connected-space](https://alphabetamath.cc/item/def-connected-space)

[math:def-proper-map-between-euclidean-open-sets](https://alphabetamath.cc/item/def-proper-map-between-euclidean-open-sets)

[math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

## Facts & Assumptions

[F1] The end-normalization supplier gives the two stationary charts of the same end, with original $O_6$ and normalized all-order metric bounds, the exact time change, and the ADM spin flux convention. The differentiated $O_m$ notation means Cartesian derivatives of order $j\le m$ gain $r^{-j}$, uniformly in angle. [lem-author-d20d145f998f-normalized-stationary-end](item-lem-author-d20d145f998f-normalized-stationary-end) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] For the same timelike stationary field and quotient metric in two end charts, the time-gauge supplier bounds $Df,Df^{-1}$, compares radii, and gives $dF=\varphi-f^*\varphi'$, $F=O(r^{-1})$ after one constant adjustment, and smooth cutoffs with $|u_R|\le C/R$, $|du_R|\le C/R^2$. Its conditional spacelikeness conclusion applies when $dt$ is timelike and the original inverse metric tends to the Minkowski inverse. [lem-author-d20d145f998f-decaying-time-gauge](item-lem-author-d20d145f998f-decaying-time-gauge)

[F3] Under the supplied product, lapse and Cauchy hypotheses, product time is Cauchy temporal. A bounded spacelike stationary graph is Cauchy and agrees with the original wherever its displacement is zero. Work in ZFC, as in the normalization supplier; this carries its choice assumption and the Countable Choice and Dependent Choice assumptions of the product-time supplier. No additional selection principle is invoked by the cutoff construction. [lem-author-d20d145f998f-stationary-product-cauchy-time](item-lem-author-d20d145f998f-stationary-product-cauchy-time) [lem-author-d20d145f998f-bounded-stationary-graph](item-lem-author-d20d145f998f-bounded-stationary-graph) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F4] A smooth Riemannian metric has a unique Levi–Civita connection, with symbols $\Gamma^k_{ij}=\tfrac12h^{k\ell}(\partial_i h_{j\ell}+\partial_j h_{i\ell}-\partial_\ell h_{ij})$. The Christoffel transformation law applies to this one connection in overlapping smooth charts. Here the common metric is the stationary quotient tensor $h=g-g(T,\cdot)\otimes g(T,\cdot)/g(T,T)$ on the far-tail orbit space, not either section's induced metric. [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry) [math:prop-christoffel-formula-for-the-levi-civita-connection](https://alphabetamath.cc/item/prop-christoffel-formula-for-the-levi-civita-connection) [math:thm-christoffel-symbol-transformation-law](https://alphabetamath.cc/item/thm-christoffel-symbol-transformation-law)

[F5] A smooth profile $b:\mathbb R\to[0,1]$ equals one on $|s|\le1$ and zero on $|s|\ge2$; its derivative is bounded on $[1,2]$. Thus $\chi_R=1-b(r/R)$ has $|d\chi_R|\le B/R$ and the required inner and outer plateaux. [math:lem-shin-radial-smooth-cutoff](https://alphabetamath.cc/item/lem-shin-radial-smooth-cutoff) [math:thm-extreme-value-r](https://alphabetamath.cc/item/thm-extreme-value-r)

[F6] Apply the total chain rule and the sum, product and quotient derivative rules componentwise to smooth functions and finite matrices; reciprocal factors are used only where their denominators are bounded away from zero. The fundamental theorem on compact intervals and integral monotonicity give the path estimates. The improper-integral Cauchy criterion gives ray limits from integrable $O(r^{-2})$ derivatives. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives) [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts) [math:thm-monotonicity-of-the-integral](https://alphabetamath.cc/item/thm-monotonicity-of-the-integral) [math:thm-cauchy-criterion-for-improper-integrals](https://alphabetamath.cc/item/thm-cauchy-criterion-for-improper-integrals)

[F7] Closed bounded Euclidean sets are compact, and compact Euclidean sets are closed and bounded. Path-connected spaces are connected. A proper $C^1$ map between nonempty Euclidean open sets of the same dimension, with connected target and invertible derivative everywhere, is surjective. An invertible derivative of a smooth map gives smooth local inverses. [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn) [math:thm-path-connected-implies-connected](https://alphabetamath.cc/item/thm-path-connected-implies-connected) [math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets](https://alphabetamath.cc/item/thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets) [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

[F8] Use smooth manifolds and charts, smooth embeddings and manifold diffeomorphisms for the supplied section and product. Lorentzian signature, time orientation and causal character have their geometric meanings; a Killing field has vanishing metric Lie derivative, its supplied complete flow is global, and a spacelike Cauchy hypersurface is spacelike and meets each inextendible causal curve once. The inverse metric acts on covectors, so timelikeness of $dt$ means $g^{-1}(dt,dt)<0$. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field) [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets) [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding) [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[F9] A Riemannian metric is a smooth positive definite symmetric covariant two-tensor. Pullback evaluates that tensor on the differential in each slot; the same definition applies to the stationary covector. An affine connection on the tangent bundle has Christoffel symbols in each chart, and its Levi–Civita conditions are metric compatibility and vanishing torsion. Smooth Euclidean maps and diffeomorphisms use componentwise smoothness and a smooth inverse on the displayed open sets. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-pullback-riemannian-metric](https://alphabetamath.cc/item/def-pullback-riemannian-metric) [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field) [math:def-ck-euclidean-maps-and-diffeomorphisms](https://alphabetamath.cc/item/def-ck-euclidean-maps-and-diffeomorphisms) [math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold) [math:def-christoffel-symbols-of-an-affine-connection](https://alphabetamath.cc/item/def-christoffel-symbols-of-an-affine-connection) [math:def-levi-civita-connection](https://alphabetamath.cc/item/def-levi-civita-connection)

[F10] Use the standard Euclidean dot product and norm on $\mathbb R^3$, spheres $|x|=r$, the coordinate cross product, and orthogonal linear isometries. Thus $u\times v=(u_2v_3-u_3v_2,u_3v_1-u_1v_3,u_1v_2-u_2v_1)$ and an orthogonal matrix satisfies $A^TA=AA^T=I$. The spherical paths used below are constructed locally from these coordinates. [math:def-euclidean-inner-product](https://alphabetamath.cc/item/def-euclidean-inner-product) [math:def-euclidean-spheres-and-closed-balls](https://alphabetamath.cc/item/def-euclidean-spheres-and-closed-balls) [math:def-cross-product-in-r3](https://alphabetamath.cc/item/def-cross-product-in-r3) [math:def-linear-isometry-and-orthogonal-or-unitary-operator](https://alphabetamath.cc/item/def-linear-isometry-and-orthogonal-or-unitary-operator)

[F11] Connected means admitting no separation into disjoint nonempty open subsets. A continuous map between Euclidean open sets is proper when the inverse image of each compact subset of its target is compact in its domain. The boundary of $C$ is taken in the supplied $\Sigma_0$ and is its closure minus its interior there; the displayed chart specifies it as $S_0$. [math:def-connected-space](https://alphabetamath.cc/item/def-connected-space) [math:def-proper-map-between-euclidean-open-sets](https://alphabetamath.cc/item/def-proper-map-between-euclidean-open-sets) [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

## Proof

**Given:** The complete product, section-extension and end-chart hypotheses in the Statement, in ZFC.

**Goal:** Extend the normalized coordinates while preserving the specified inner section, and establish the stated differentiated transition bounds.

1.1 On a sufficiently far tail $T$ is timelike. In either chart the quotient metric is $h_{ij}=g_{ij}-g_{0i}g_{0j}/g_{00}$, so $h=\delta+O_6(r^{-1})$ in the original chart and $h'=\delta+O_\infty(|y|^{-1})$ in the normalized chart. These represent the same Riemannian metric by [F2]. That supplier bounds $Df,Df^{-1}$ and compares $r,|y|$. Apply [F4] to its unique quotient Levi–Civita connection. Its symbols satisfy $\Gamma=O_5(r^{-2})$ and $\Gamma'=O_\infty(|y|^{-2})$; the inverse-matrix derivative estimates follow by differentiating $h^{-1}h=I$. In particular the transformation law rearranges to $\partial_i\partial_j f^a=\Gamma^k_{ij}\partial_kf^a-\Gamma'{}^a_{bc}(f)\partial_if^b\partial_jf^c$, giving $D^2f=O(r^{-2})$. [F1, F2, F4, F6, F9]

2.1 Integrate the derivative of $Df(r\omega)$ along each fixed ray: its norm is at most $Cr^{-2}$, so [F6] gives a limit $Q(\omega)$ and $|Df(r\omega)-Q(\omega)|\le C/r$. Here is a local construction for any two unit directions $u,v$. If they are not parallel, the coordinate formula in [F10] gives a nonzero $u\times v$ perpendicular to both (vanishing of all its coordinate minors would make $u,v$ proportional); normalize it to a unit vector $w$. If they are parallel, choose a coordinate vector not parallel to $u$ and normalize its cross product with $u$, again obtaining $w$ perpendicular to both. For $a=u$ and $a=v$ the rational arc $\gamma_a(s)=r((1-s^2)a+2sw)/(1+s^2)$, $0\le s\le1$, joins $ra$ to $rw$. Since $a,w$ are orthonormal, direct expansion gives $|\gamma_a(s)|=r$, while the quotient rule in [F6] gives $|\gamma'_a(s)|=2r/(1+s^2)\le2r$. Each arc therefore has speed integral at most $2r$. Concatenate $\gamma_u$ with the reversed $\gamma_v$; the total is at most $4r$. The chain rule and fundamental theorem in [F6], applied componentwise to $Df\circ\gamma_a$ and the bound from step 1.1, give $|Df(ru)-Df(rv)|\le4C/r$ (enlarging the fixed finite-dimensional norm constant if needed), so all limits are a single matrix $Q_0$. The pullback identity $h=(Df)^T(h'\circ f)Df$ now gives $Q_0^TQ_0=I$. Integrating $Df-Q_0=O(r^{-1})$ radially from one fixed large sphere gives $f-Q_0x=O(\log r)$ uniformly in angle; bounded values on that fixed sphere also follow by the same angular path estimate from one anchor. No orientation of $Q_0$ is presumed. [F1, F2, F6, F9, F10, step 1.1]

3.1 Set $A=Q_0^T$ and $z=Ay$. The identity $A(v\times w)=(\det A)(Av\times Aw)$ follows by expanding the determinant definition of the cross product, for any orthogonal $A$. The normalized spatial metric is conjugated by $A$, the mixed metric covector transforms by $A$, and $|z|=|y|$. Hence its leading mixed coefficient is $-2(S_A\times z)/|z|^3$, where $S_A=(\det A)AS$, and all differentiated remainder orders and the mass are unchanged. For the ADM check, a test rotation $B\times z$ pulls back to $(\det A)(A^TB)\times y$. The outward normal and positive area measure transform isometrically; the flux convention in [F1] therefore gives $J_z(B)=(\det A)(A^TB)\cdot S=B\cdot S_A$. Thus the spin convention is preserved as an axial vector, even if $\det A=-1$, and $|S_A|=|S|$. Rename $z$ as $y$ and $A\circ f$ as $f$; then $Df=I+O(r^{-1})$, $f-x=O(\log r)$. [F1, F10, step 2.1, algebra]

4.1 Differentiate the Christoffel identity of step 1.1 at most five times. Inductively, after $k$ differentiations its right-hand side contains only derivatives of $f$ through order $k+1$, together with derivatives of $\Gamma$ through order $k$ and of $\Gamma'$ through order $k$. The bounded first derivatives and the induction estimates $D^j f=O(r^{-j})$ for $j\ge2$ bound every term by $O(r^{-k-2})$. Thus $D^{k+2}f=O(r^{-k-2})$ for $0\le k\le5$. The same argument with charts reversed gives the inverse bounds through order seven. Now put $\varphi_i=g_{0i}/g_{00}$ in each chart. The original metric gives $\varphi=O_6(r^{-2})$ and the normalized metric gives $\varphi'=O_\infty(|y|^{-2})$. Equating the two representations of $g(T,\cdot)/g(T,T)$ gives $(dF)_i=\varphi_i-\varphi'_a(f)\partial_i f^a$. In each of its derivatives of order $k\le6$, the chain and product rules use derivatives of $f$ of order at most $k+1\le7$. The bounds just proved and radius comparison give $\partial^k(dF)=O(r^{-2-k})$. This derives $dF=O_6(r^{-2})$ from the stationary one-form, rather than from spatial connection estimates alone. Normalize $F=O(r^{-1})$ by the constant adjustment in [F2]. [F1, F2, F4, F6, step 1.1, step 3.1]

4.2 On the common far end choose $\chi_R$ from [F5] and set $f_R=x+\chi_R(f-x)$, extending by the identity to all of $\mathbb R^3$. This is smooth because the cutoff has an inner plateau and its nonzero part lies inside the domain of $f$. On $R\le r\le2R$, $Df_R-I=\chi_R(Df-I)+(f-x)\otimes d\chi_R=O(\log R/R)$; outside it is either zero or $O(r^{-1})$. Choose $R$ so $\sup\|Df_R-I\|<1/2$. For $q_R=f_R-I$, integration along the straight segment from $a$ to $b$ gives $|q_R(a)-q_R(b)|\le\tfrac12|a-b|$, hence $|f_R(a)-f_R(b)|\ge\tfrac12|a-b|$. Thus $f_R$ is injective and its derivative is invertible everywhere. [F5, F6, step 3.1]

5.1 Since $q_R=O(\log r)$, $|f_R(x)|\to\infty$ as $|x|\to\infty$. The inverse image of a compact Euclidean set is therefore bounded and is closed by continuity and closedness of compact sets, hence compact by [F7]. So $f_R$ is proper. Its target $\mathbb R^3$ is connected, since straight segments join every pair of points and [F7] applies. The proper local-diffeomorphism theorem gives surjectivity; the smooth inverse function theorem gives local smooth inverses, which agree by injectivity and yield a global smooth inverse. The map fixes the ball $r\le R$ pointwise. Bijectivity then prevents any exterior point from mapping into that ball, so its restriction is a diffeomorphism of $\{r>1/2\}$, fixing a neighborhood of $S_0$. [F7, F9, F11, step 4.2]

5.2 The supplied product satisfies [F3], so $t$ is Cauchy temporal and $dt$ is timelike throughout $E$. The original metric bounds imply its inverse tends uniformly to the Minkowski inverse on the end. Thus the conditional spacelike-graph hypotheses of [F2] hold, with $g^{00}\le-1/2$ and uniformly bounded inverse components sufficiently far out. Choose $R$ as in step 4.2 and large enough for that supplier. It gives $u_R=\chi_RF$ with $\sup|u_R|\le C/R$ and $\sup|du_R|\le C/R^2$, and proves that $t+u_R=0$ is smooth and spacelike. In particular only first derivatives are needed for this conclusion; step 4.1 separately establishes the stronger differentiated transition estimates. Applying [F3] with displacement $-u_R$ makes this graph $C'$ Cauchy and gives its diffeomorphism with $C$ by product projection. The choice assumptions required by these suppliers are included in ZFC as recorded in [F3]. [F1, F2, F3, F8, step 4.1, step 4.2]

6.1 Where $r\le R$ the graph is exactly the old section. Attach the unchanged part of $\Sigma_0$ there; equality on the overlap makes the ambient section extension smooth, with literal equality on a neighborhood of the explicitly supplied sphere $S_0$. This proves the bifurcation-sphere conclusion whenever $S_0$ is that sphere, without inferring existence of a bifurcation surface from a stationary product. Transport $f_R\circ x$ to $C'$ using product projection and keep it on the unchanged inner extension. Step 5.1 makes it a global spatial chart on that extension, fixing $S_0$; in $r\ge2R$ it equals $y$, while $t+u_R=t+F=t'$. Thus the new section is precisely $t'=0$ in the normalized end. These constructions assert no maximality of the new section. [F2, F3, F8, F11, step 5.1, step 5.2, given] ∎

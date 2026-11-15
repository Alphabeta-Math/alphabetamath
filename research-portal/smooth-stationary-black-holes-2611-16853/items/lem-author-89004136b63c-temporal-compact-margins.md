---
id: lem-author-89004136b63c-temporal-compact-margins
title: A temporal covector has uniform compact negativity and orientation margins
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - math:lem-matrix-inversion-preserves-ck-regularity
  - math:def-compact-space
  - math:lem-compactness-of-a-subspace-is-ambient
  - lem-author-89004136b63c-compact-neighborhood-localization
  - physics:def-lorentz-form-and-inertia
  - physics:def-causal-classification-of-lorentz-vectors
  - physics:def-time-orientation-and-future-causal-sets
  - physics:lem-timelike-cone-has-two-convex-components
  - math:thm-cauchy-schwarz-finite
  - math:def-smooth-manifold
  - math:thm-tensor-transition-laws-define-a-smooth-vector-bundle
  - math:thm-coordinate-differentials-form-the-dual-cotangent-basis
  - math:def-vector-bundle-chart-and-transition-function
  - math:def-c-r-and-smooth-maps-between-smooth-manifolds
  - math:thm-ck-euclidean-maps-closed-under-algebra-and-composition
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  math:lem-matrix-inversion-preserves-ck-regularity: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:lem-compactness-of-a-subspace-is-ambient: mathematical-premise
  lem-author-89004136b63c-compact-neighborhood-localization: mathematical-premise
  physics:def-lorentz-form-and-inertia: mathematical-premise
  physics:def-causal-classification-of-lorentz-vectors: mathematical-premise
  physics:def-time-orientation-and-future-causal-sets: mathematical-premise
  physics:lem-timelike-cone-has-two-convex-components: mathematical-premise
  math:thm-cauchy-schwarz-finite: mathematical-premise
  math:def-smooth-manifold: mathematical-premise
  math:thm-tensor-transition-laws-define-a-smooth-vector-bundle: mathematical-premise
  math:thm-coordinate-differentials-form-the-dual-cotangent-basis: mathematical-premise
  math:def-vector-bundle-chart-and-transition-function: mathematical-premise
  math:def-c-r-and-smooth-maps-between-smooth-manifolds: mathematical-premise
  math:thm-ck-euclidean-maps-closed-under-algebra-and-composition: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Let $O$ be an open subset of a smooth four-manifold, $g$ a $C^2$ Lorentz metric of signature $(-,+,+,+)$ on $O$, $N$ a continuous timelike orientation field on $O$, and $\alpha$ a continuous covector field on $O$. Let $K\subset O$ be nonempty and compact. At each point, the raised vector $\alpha^\sharp$ is characterized by $g(\alpha^\sharp,w)=\alpha(w)$ for every tangent vector $w$, and $g^{-1}(\alpha,\beta)=g(\alpha^\sharp,\beta^\sharp)$. The future timelike cone is the component of the timelike set containing $N$; the other component is past timelike. These pointwise constructions are justified below at the stated regularity.

Suppose $g^{-1}(\alpha,\alpha)<0$, $\alpha(N)>0$ and $g(N,N)<0$ on $K$. Then there are constants $m,a,b>0$ such that $g^{-1}(\alpha,\alpha)\le-m$, $\alpha(N)\ge a$, and $g(N,N)\le-b$ throughout $K$. For any fixed finite compact chart cover consisting of compact sets $K_j\subset O\cap U_j$, where $U_j$ is a smooth chart domain and $K\subset\bigcup_j K_j$, the components of $\alpha$ and $N$ in that chart are bounded on each $K_j$. Such covers exist, and may be chosen with every $K_j\subset K$. At any point, call $\alpha$ temporal when $g^{-1}(\alpha,\alpha)<0$ and $\alpha(N)>0$; its raised vector is past timelike there.

## Statement references

[[def-causal-exterior-and-boundary-data]]

[[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

[[math:lem-matrix-inversion-preserves-ck-regularity]]

[[math:def-compact-space]]

[[math:lem-compactness-of-a-subspace-is-ambient]]

[[lem-author-89004136b63c-compact-neighborhood-localization]]

[[physics:def-lorentz-form-and-inertia]]

[[physics:def-causal-classification-of-lorentz-vectors]]

[[physics:def-time-orientation-and-future-causal-sets]]

[[physics:lem-timelike-cone-has-two-convex-components]]

[[math:thm-cauchy-schwarz-finite]]

[[math:def-smooth-manifold]]

[[math:thm-tensor-transition-laws-define-a-smooth-vector-bundle]]

[[math:thm-coordinate-differentials-form-the-dual-cotangent-basis]]

[[math:def-vector-bundle-chart-and-transition-function]]

[[math:def-c-r-and-smooth-maps-between-smooth-manifolds]]

[[math:thm-ck-euclidean-maps-closed-under-algebra-and-composition]]

## Facts & Assumptions

[F1] For smooth data, the musical convention characterizes raising by $g(\alpha^\sharp,w)=\alpha(w)$, and the temporal-function convention uses past-timelike gradients. These suppliers fix the conventions only; their smooth hypotheses are not asserted for the present data. The pointwise construction and orientation test for the present $C^2$ metric and continuous fields are established in steps 2.1 and 3.1. [[physics:def-gr-inverse-metric-and-musical-isomorphisms]] [[def-causal-exterior-and-boundary-data]]

[F2] A Lorentz form on a four-dimensional real vector space is nondegenerate and has signature $(-,+,+,+)$, with an orthonormal basis in which its quadratic form is $-(v^0)^2+|\mathbf v|^2$. Timelike means negative quadratic form. The timelike set has exactly two components, described in such a basis by $v^0>|\mathbf v|$ and $v^0<-|\mathbf v|$; a time orientation chooses one component as future. All these are pointwise vector-space statements, with no differentiability hypothesis. [[physics:def-lorentz-form-and-inertia]] [[physics:def-causal-classification-of-lorentz-vectors]] [[physics:lem-timelike-cone-has-two-convex-components]] [[physics:def-time-orientation-and-future-causal-sets]]

[F3] An invertible matrix with $C^2$ entries on an open coordinate domain has $C^2$ inverse entries. We apply this with $4\times4$ metric matrices and nonvanishing determinant. [[math:lem-matrix-inversion-preserves-ck-regularity]]

[F4] Compactness gives finite open subcovers, also for ambient open covers. Applying compact-neighborhood localization inside the specified open set $O$ gives finite compact chart pieces covering $K$; its construction can take the pieces to be subsets of $K$, hence of $O$. [[math:def-compact-space]] [[math:lem-compactness-of-a-subspace-is-ambient]] [[lem-author-89004136b63c-compact-neighborhood-localization]]

[F5] For two lists of three real numbers, $|\sum_{i=1}^3 x_i y_i|\le(\sum_{i=1}^3 x_i^2)^{1/2}(\sum_{i=1}^3 y_i^2)^{1/2}$. This is the finite Cauchy-Schwarz inequality with three entries. [[math:thm-cauchy-schwarz-finite]]

[F6] A smooth manifold has a maximal smooth atlas. Tensor-coordinate trivializations give smooth vector bundles for types $(1,0)$, $(0,1)$ and $(0,2)$, with fibres respectively tangent vectors, covectors and bilinear forms. The coordinate tangent vectors and coordinate differentials are dual bases. Bundle-chart changes are smooth and fibrewise linear. The $C^2$ class of a map is tested in smooth coordinates, and finite $C^2$ sums, products and compositions are $C^2$. These structural interfaces are used in step 1.1 to justify the component criteria for the present continuous and $C^2$ sections, without assuming that those sections are smooth. [[math:def-smooth-manifold]] [[math:thm-tensor-transition-laws-define-a-smooth-vector-bundle]] [[math:thm-coordinate-differentials-form-the-dual-cotangent-basis]] [[math:def-vector-bundle-chart-and-transition-function]] [[math:def-c-r-and-smooth-maps-between-smooth-manifolds]] [[math:thm-ck-euclidean-maps-closed-under-algebra-and-composition]]

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the compact margins, the component bounds on the specified chart pieces, and the pointwise past-timelike conclusion.

1.1 Use the smooth charts and the tensor-coordinate trivializations from F6. In a chart $(U,x)$ restricted to $O$, write $e_a=\partial/\partial x^a$ and let $dx^a$ be its dual basis. Then $N=\sum_a N^a e_a$, $\alpha=\sum_a\alpha_a dx^a$ and $g=\sum_{a,b}g_{ab}\,dx^a\otimes dx^b$, with $N^a=dx^a(N)$, $\alpha_a=\alpha(e_a)$ and $g_{ab}=g(e_a,e_b)$. For any of these bundles, a section $s$ has trivialization coordinates $p\mapsto(p,c(p))$, where $c$ is precisely its finite list of field components. A trivialization and its inverse are continuous, so $s$ is continuous on the chart domain exactly when $c$ is continuous: the forward direction projects the continuous map $(p,c(p))$ to its fibre coordinates, and the reverse direction composes this product map with the inverse trivialization. In total-space smooth coordinates the same representative is $x(p)\mapsto(x(p),c(p))$, so F6's coordinate definition of $C^2$ gives the corresponding equivalence for $C^2$ sections. Changing a bundle chart replaces $c$ by a smooth matrix times $c$ and changes the base coordinates smoothly; hence continuity and $C^2$ regularity are preserved, the latter by F6's algebra and composition rule. Consequently $N^a$ and $\alpha_a$ are continuous and $g_{ab}$ is $C^2$ in every smooth chart on $O$, at exactly the regularities stated. [given, F6, algebra]

2.1 At $p\in O$, let $G=(g_{ab}(p))$ in a smooth coordinate chart. Nondegeneracy gives an inverse matrix $(g^{ab}(p))$. Define $v^a=\sum_b g^{ab}(p)\alpha_b(p)$. Matrix multiplication gives $g_p(v,w)=\alpha_p(w)$ for every $w\in T_pO$. This vector is unique, since a difference of two candidates pairs to zero with every $w$ and $g_p$ is nondegenerate. Thus the coordinate construction is independent of the chart and defines $\alpha^\sharp$. The same construction for any covector $\beta$ defines $g^{-1}(\alpha,\beta)$ with coefficients $g^{ab}$ and gives $g(\alpha^\sharp,\alpha^\sharp)=g^{-1}(\alpha,\alpha)$ and $g(\alpha^\sharp,N)=\alpha(N)$. By step 1.1 the metric coefficients are $C^2$, so F3 makes the inverse coefficients $C^2$; finite sums and products of them with the continuous field components show that $g^{-1}(\alpha,\alpha)$, $\alpha(N)$ and $g(N,N)$ are continuous. This constructs the convention of F1 without imposing smoothness on $g,N$ or $\alpha$. [given, F1, F2, F3, step 1.1, algebra]

3.1 Fix $p\in O$ and a $g_p$-orthonormal basis from F2, and write a timelike vector $v$ and $N_p$ as $(v^0,\mathbf v)$ and $(n^0,\mathbf n)$. Their timelikeness gives $|\mathbf v|<|v^0|$ and $|\mathbf n|<|n^0|$, so F5 yields $|\mathbf v\cdot\mathbf n|\le|\mathbf v|\,|\mathbf n|<|v^0n^0|$. Consequently $g_p(v,N_p)=-v^0n^0+\mathbf v\cdot\mathbf n$ is negative exactly when $v^0,n^0$ have the same sign, and positive exactly when their signs differ. F2 identifies these alternatives with the same and opposite timelike components. Therefore, relative to the component selected by $N_p$, a timelike $v$ is past directed exactly when $g_p(v,N_p)>0$. This is a pointwise test and requires no smooth orientation field or smoothly varying orthonormal basis. Applied to $v=\alpha^\sharp$, step 2.1 proves the asserted temporal-covector convention, including the past-timelike conclusion wherever the two defining inequalities hold. [F1, F2, F5, step 2.1, algebra]

3.2 Put $h=-g^{-1}(\alpha,\alpha)$, $u=\alpha(N)$ and $z=-g(N,N)$. These functions are continuous on $O$ and positive on $K$. For each $p\in K$, define $W_p$ to be the set of $q\in O$ satisfying $h(q)>h(p)/2$, $u(q)>u(p)/2$ and $z(q)>z(p)/2$. This is an open neighborhood of $p$. The indexed family $(W_p)_{p\in K}$ covers $K$; F4 gives finitely many centers $p_1,\ldots,p_r$ whose neighborhoods cover $K$. Set $m=\min_i h(p_i)/2$, $a=\min_i u(p_i)/2$ and $b=\min_i z(p_i)/2$. The finite list is nonempty and all its entries are positive. These constants give the three required uniform inequalities throughout $K$. [given, F4, step 2.1]

4.1 F4 supplies a finite compact chart cover inside $O$, with pieces in $K$ if desired. Now fix any cover allowed in the Statement, not necessarily that particular one. Each component function $f$ of either field is defined and continuous on $O\cap U_j$, which contains $K_j$. If $K_j$ is nonempty, cover it by the open neighborhoods on which $|f(q)|<|f(p)|+1$ for centers $p\in K_j$. A finite subcover from F4 bounds $|f|$ on $K_j$ by the maximum of the finitely many numbers $|f(p)|+1$. For empty pieces the bound is vacuous. Repeating this for the finitely many components in the finitely many specified charts proves the component conclusion. Step 3.1 proves the past-timelike conclusion on $K$, and step 3.2 proves the uniform margins, completing all the claims. [given, F4, step 1.1, step 3.1, step 3.2] ∎

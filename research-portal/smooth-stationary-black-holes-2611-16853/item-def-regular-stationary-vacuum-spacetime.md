---
title: Regular non-degenerate stationary vacuum spacetime
status: draft
research_item: def-regular-stationary-vacuum-spacetime
dependency_level: 2
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 3–4, Section 1.2, Definition 1.1(1)–(4)
      statement: The article defines regular non-degenerate stationary vacuum
        spacetimes by the four asymptotic, completeness, bifurcation-sphere and
        tangency conditions reproduced below.
      hypotheses: A smooth four-dimensional Lorentzian manifold with a smooth
        stationary Killing field satisfying the vacuum equation and the four
        stated conditions.
      reading_limits: Read the frozen PDF images and corresponding text on pp. 3–4 for
        attribution and formulation of Definition 1.1 only; this reference is
        not used as an independent proof or as a supplier of the mathematical
        interfaces or the local justification.
---

PDF p. 3: ` Definition 1.1, conditions (1)–(2) `; PDF p. 4: ` Definition 1.1, conditions (3)–(4) `

## Prerequisites

- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)
- [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)
- [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)
- [physics:lem-lorentz-form-has-orthonormal-basis](https://alphabetamath.cc/physics/item/lem-lorentz-form-has-orthonormal-basis)
- [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Definition

Work in ZFC, including the axiom of choice. Let $(M,g)$ be a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$, and let $T$ be a smooth Killing field: $\mathcal L_Tg=0$, where the Lie derivative is defined using the local flow of $T$. Write $\operatorname{Ric}(g)$ for the Ricci contraction of the curvature of the Levi–Civita connection, and assume $\operatorname{Ric}(g)=0$. A timelike vector has negative squared length; future direction is determined by the time orientation. In the stationary setting $T$ is future timelike near infinity.

The article calls these data a **regular non-degenerate stationary vacuum spacetime** when all four conditions below hold.

1. There is an open end $M^{\mathrm{end}}\subset M$ with a diffeomorphism onto $\mathbb R\times\{x\in\mathbb R^3:|x|>R_0\}$, for sufficiently large $R_0>0$. In the corresponding coordinates $(t,x^1,x^2,x^3)$, with $r=|x|$, $T=\partial_t$ and $g_{00}=-1+2M_0/r+O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$, and $g_{0i}=O_6(r^{-2})$. Here $M_0$ is the constant denoted $M$ in the article, and $u=O_m(r^{-b})$ means that for each spatial multi-index $\alpha$ with $|\alpha|\le m$, $|\partial_x^\alpha u|\le C_\alpha r^{-b-|\alpha|}$ for sufficiently large $r$, uniformly in angular direction. The metric coefficients are independent of $t$ because $T=\partial_t$ is Killing. Set $\mathcal E=I_M^-(M^{\mathrm{end}})\cap I_M^+(M^{\mathrm{end}})$.

2. The region $\mathcal E$, with the restricted metric and time orientation, is globally hyperbolic. Every orbit of $T$ in $\mathcal E$ is complete and meets a specified smooth spacelike hypersurface $\Sigma_0$; $\Sigma_0\cap\mathcal E$ is Cauchy in $\mathcal E$. There is a diffeomorphism $\Sigma_0\simeq\{x\in\mathbb R^3:|x|>1/2\}$. The hypersurface $\Sigma_0$ agrees with the $t=0$ slice in $M^{\mathrm{end}}$.

3. Put $S=\partial_M I_M^-(M^{\mathrm{end}})\cap\partial_M I_M^+(M^{\mathrm{end}})$. It is a smooth embedded two-sphere contained in $\Sigma_0$ and corresponding to $|x|=1$ under the specified identification. There is a neighborhood $\mathcal O$ of $S$ in $M$ such that $\mathcal H^+=\mathcal O\cap\partial_M I_M^-(M^{\mathrm{end}})$ and $\mathcal H^-=\mathcal O\cap\partial_M I_M^+(M^{\mathrm{end}})$ are smooth embedded hypersurfaces, each diffeomorphic to $S\times(-1,1)$. They are null, have vanishing null expansion, and intersect transversely in $S$.

4. The field $T$ is tangent to both $\mathcal H^+$ and $\mathcal H^-$.

Here $I_M^+(U)$, respectively $I_M^-(U)$, consists of points reachable from, respectively reaching, $U$ by future-directed timelike curves in $M$; boundaries are taken in $M$. A spacelike hypersurface has positive-definite induced metric. A Cauchy set in $\mathcal E$ meets every inextendible causal curve in $\mathcal E$ exactly once. Global hyperbolicity means strong causality and compact causal diamonds, with both notions taken in $\mathcal E$. An orbit is complete when its integral curve is defined for every real flow parameter.

For a smooth null hypersurface $H$, its induced metric has a null radical line. Locally choose a nonzero smooth section $L$ of that line. Its screen is $TH/\mathbb RL$ with the induced positive metric $q$. Define the null expansion as the $q$-trace of the screen bilinear form $([X],[Y])\mapsto g(\nabla_XL,Y)$, where $X,Y$ are tangent to $H$. Vanishing of this trace is the **non-expanding** condition; it is independent of the local nonzero choice of $L$. Transversality at $S$ means $T_p\mathcal H^++T_p\mathcal H^-=T_pM$ at every $p\in S$.

## Facts & Assumptions

[A1] The convention includes the axiom of choice, which supplies the inherited countable-choice assumptions of the smooth Lorentzian and screen suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The Lorentzian, Killing-field, connection and curvature interfaces supply the metric, local-flow Lie derivative, Levi–Civita connection and Ricci conventions. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field) [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection) [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)

[F2] The causal interface defines chronological sets, ambient boundaries, Cauchy sets and global hyperbolicity relative to the specified domain. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F3] A spacelike hypersurface has positive-definite induced metric, while a null hypersurface has a radical line in its tangent metric. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[F4] For a spacelike two-surface with a chosen null normal, the expansion convention is the trace of $(X,Y)\mapsto g(\nabla_XL,Y)$ in the induced positive metric. Only this trace convention from the screen definition is used, without importing its separate affine-congruence hypotheses. The differentiated end notation uses spatial derivatives and angularly uniform bounds. [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F5] A diffeomorphism is a bijective smooth map with smooth inverse; two smooth manifolds are diffeomorphic when such a map exists. [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[F6] For a smooth null hypersurface whose induced form is positive semidefinite of rank two, and a smooth future nowhere-zero radical field $L$, the positive-screen lemma supplies the smooth rank-two quotient $L^\perp/\mathbb RL$ with positive metric $q([X],[Y])=g(X,Y)$. Fields defined only along the hypersurface use the pullback connection. The quotient assertion does not require an affine geodesic congruence; the affine hypothesis belongs to the later optical-endomorphism assertion. [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)

[F7] A smooth embedded hypersurface admits local slice coordinates in which it is $\rho=0$ with $d\rho\ne0$; tangent vector fields in these coordinates have a Lie bracket tangent to the hypersurface, since its normal component is zero there. [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

[F8] Every Lorentz form on a four-dimensional real vector space has an ordered orthonormal basis in which its matrix is $\operatorname{diag}(-1,1,1,1)$. [physics:lem-lorentz-form-has-orthonormal-basis](https://alphabetamath.cc/physics/item/lem-lorentz-form-has-orthonormal-basis)

## Justification

**Given:** The smooth geometric data and the specified end, hypersurface and neighborhood in the Definition.

**Goal:** Show that the conditions define an unambiguous predicate on those data.

1.1 The Lorentzian and causal interfaces determine the equations, chronological sets and ambient boundaries, and specify which causal curves and compact diamonds enter the Cauchy and global-hyperbolicity predicates. The diffeomorphism interface makes each stated identification a smooth bijection with smooth inverse. The chart and the differentiated-bound convention determine the end conditions; the local flow of $\partial_t$ translates $t$ while fixing $x$, so the flow definition of $\mathcal L_{\partial_t}g=0$ gives $\partial_tg_{\mu\nu}=0$ in that chart. The remaining clauses are explicit conditions on the supplied embeddings, flow and intersections. The ZFC convention supplies the inherited choice assumptions. [given, A1, F1, F2, F3, F4, F5, F7]

1.2 Near any point of a smooth null hypersurface $H$, take a slice coordinate $\rho$ with $H=\{\rho=0\}$ and $d\rho\ne0$. Define $L^a=g^{ab}\partial_b\rho$ along $H$, where $g^{ab}$ are the smooth inverse metric components. This is a smooth nonzero normal field. Nondegeneracy of $g$ makes $(T_pH)^\perp$ one-dimensional; the nonzero radical of $g|_{T_pH}$ lies in this normal space and therefore equals it. Thus $L$ is tangent and null, and $T_pH=L_p^\perp$. [given, F1, F3, F7]

2.1 Fix $p\in H$ and use the orthonormal basis supplied by F8 to identify $T_pM$ with $\mathbb R\times\mathbb R^3$, with $g_p((s,x),(t,y))=-st+x\cdot y$. Write $L_p=(a,v)$. Since $L_p$ is nonzero and null, $|v|^2=a^2$ and $a\ne0$. Put $e=v/a$, so $|e|=1$. A vector $(s,x)$ lies in $L_p^\perp$ exactly when $s=e\cdot x$. For such a vector set $w=x-se$; then $e\cdot w=0$ and $(s,x)=(s/a)L_p+(0,w)$. This decomposition is unique, since a vector in $\mathbb RL_p$ with zero time component is zero. The space $E_p=\{(0,w):e\cdot w=0\}$ has dimension two: some component $e_j$ is nonzero, and the equation $e\cdot w=0$ solves uniquely for $w_j$ in terms of the other two components. Moreover $g_p((0,w),(0,w))=|w|^2$, which is positive for $w\ne0$, while $L_p$ is orthogonal to all of $L_p^\perp$. Thus $T_pH=L_p^\perp=\mathbb RL_p\oplus E_p$ has positive-semidefinite induced form of rank two and radical $\mathbb RL_p$. Its quotient by that radical has a well-defined positive metric, because adding multiples of $L_p$ changes no pairing. This pointwise argument uses only the Lorentz-basis interface and elementary coordinate algebra, not the screen lemma. [F8, step 1.2, algebra]

3.1 The local field constructed in step 1.2 is smooth and nowhere zero. Shrink its neighborhood and reverse its sign if necessary to make it future with respect to the given time orientation. Step 2.1 has established the positive-semidefinite rank-two hypothesis at every point of $H$, so the stated smooth-quotient assertion in F6 now applies. It supplies the smooth positive metric $q$ on $TH/\mathbb RL$ used in the Definition. No affine parameter or congruence from a two-surface is needed. [A1, F1, F6, step 1.2, step 2.1]

4.1 Use tangential covariant derivatives along $H$. They are independent of ambient extension: the difference of two extensions has zero components on $H$, so tangential derivatives of those components vanish there, and the connection terms multiplying those zero components also vanish. For tangent $X,Y$, write $b(X,Y)=g(\nabla_XL,Y)$. Metric compatibility gives $b(X,L)=\tfrac12Xg(L,L)=0$. To check the other slot explicitly, $0=L g(L,Y)=g(\nabla_LL,Y)+g(L,\nabla_LY)$; torsion-freeness gives $\nabla_LY=\nabla_YL+[L,Y]$, and both $g(L,\nabla_YL)=\tfrac12Yg(L,L)$ and $g(L,[L,Y])$ vanish. Hence $b(L,Y)=0$. Also $b(X,Y)-b(Y,X)=-g(L,\nabla_XY-\nabla_YX)=-g(L,[X,Y])=0$. The tangent-bracket property in F7 justifies both bracket vanishings. The connection rules make $b$ bilinear over smooth functions in $X,Y$, so it descends to a smooth symmetric bilinear form on the positive screen. [F1, F6, F7, step 1.2, step 3.1]

5.1 In a screen basis, let $Q$ and $B$ be the matrices of $q$ and the descended form. The trace is $\operatorname{tr}(Q^{-1}B)$, the convention in F4. Under a basis change $C$, these become $C^{\mathsf T}QC$ and $C^{\mathsf T}BC$, so their contracted matrix is $C^{-1}Q^{-1}BC$; summing the diagonal entries shows its trace equals $\operatorname{tr}(Q^{-1}B)$. If $L$ is replaced by $aL$ for a nowhere-zero smooth function $a$, then $g(\nabla_X(aL),Y)=a\,g(\nabla_XL,Y)$ because $g(L,Y)=0$. Thus the form and its trace are multiplied by $a$, while the radical line and quotient metric stay fixed. Any two local nonzero radical fields differ by such a smooth function, so vanishing of expansion is well defined on overlaps. These are conditions, not assertions that suitable data exist, and tangency of $T$ does not assert that either boundary is a Killing horizon for $T$. [F1, F3, F4, F6, step 1.1, step 1.2, step 3.1, step 4.1, algebra] ∎

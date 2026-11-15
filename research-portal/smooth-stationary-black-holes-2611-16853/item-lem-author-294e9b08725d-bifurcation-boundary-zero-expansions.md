---
title: Zero boundary expansions without maximality
status: draft
research_item: lem-author-294e9b08725d-bifurcation-boundary-zero-expansions
dependency_level: 4
sources:
  references: []
---

## Prerequisites

- [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)


## Statement

Let $\overline C=C\cup S$ be the smooth exterior section with boundary supplied under the regular stationary-vacuum hypotheses. Let $n$ be its future unit normal and $\nu$ the unit normal to $S$ pointing into $\overline C$ (toward the end), and put $k(X,Y)=-g(\nabla_Xn,Y)$. With $\gamma=g|_{TS}$, define the unaveraged boundary mean curvature by $H_S=\operatorname{tr}_\gamma[(X,Y)\mapsto g(\nabla_X\nu,Y)]$ for $X,Y\in TS$, using covariant derivatives along $S$. If the two horizon null expansions vanish at $S$, then $H_S=0$ and $\operatorname{tr}_S k=0$, where $\operatorname{tr}_S k=\operatorname{tr}_\gamma(k|_{TS\times TS})$. In particular both expressions $\theta_\pm=\pm H_S+\operatorname{tr}_S k$ vanish, independently of the sign convention for $k$. No maximality is assumed.

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The two zero boundary traces and their stated sign independence.

[F1] The regular-spacetime hypotheses are formulated in ZFC. The exterior section is a smooth spacelike manifold with smooth compact boundary $S\subset\Sigma_0$. [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F2] The two smooth null horizons $\mathcal H^+$ and $\mathcal H^-$ contain $S$, intersect transversely there, and have zero screen expansion. Their screen expansion is the trace of $([X],[Y])\mapsto g(\nabla_XL,Y)$ for a local nonzero radical field $L$; zero expansion is unchanged by nonzero smooth rescaling. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F3] The induced data have a smooth future unit normal $n$, induced metric $h=g|_{T\overline C}$, and second fundamental form $k(X,Y)=-g(\nabla_Xn,Y)$. The surface expansion of a null normal $\ell$ is $\operatorname{tr}_\gamma[(X,Y)\mapsto g(\nabla_X\ell,Y)]$. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F4] For a spacelike two-surface in a time-oriented Lorentzian four-manifold, the normal plane is Lorentzian with two future null rays. A null hypersurface with radical $\mathbb RL$ has tangent space $L^\perp$. On a spacelike section its quotient screen is isometric to the section tangent plane, and surface null second fundamental forms scale by $\chi_{e^fL}=e^f\chi_L$. These assertions do not require an affine generator. [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)

## Proof

**Given:** The data of the Statement and [F1]–[F4].

**Goal:** Identify the two horizon traces with the boundary trace formulas and solve them.

1.1 At $p\in S$, the inclusion $T_pS\subset T_p\overline C$ makes $\gamma$ positive definite. For either horizon let $\mathbb RL$ be its radical line. Since $T_pS\subset T_p\mathcal H^\pm=L^\perp$, $L$ is normal to $S$. The line $\mathbb RL$ cannot intersect the positive-definite plane $T_pS$ nontrivially. Their dimensions are one and two, so $T_p\mathcal H^\pm=T_pS\oplus\mathbb RL$. Thus $S$ is a spacelike section of each horizon, and [F4] identifies its tangent metric with each screen metric. [F1, F2, F4]

2.1 The fields $n,\nu$ are orthogonal unit normals to $S$, with squared lengths $-1,1$. They span its normal plane, whose null lines are exactly $\mathbb R(n+\nu)$ and $\mathbb R(n-\nu)$, because $g(an+b\nu,an+b\nu)=-a^2+b^2$. Put $\ell_\pm=n\pm\nu$. They are future null, since $g(\ell_\pm,n)=-1$, and satisfy $g(\ell_+,\ell_-)=-2$. The two horizon radical lines are distinct: if they agreed, [F4] would give equal tangent hyperplanes, contrary to their transverse intersection. Hence, after a local interchange of horizon labels, each $\ell_\pm$ is a smooth positive multiple $a_\pm L_\pm|_S$ of a smooth future horizon radical field. [F1, F2, F3, F4, step 1.1, algebra]

3.1 Under the screen isometries of step 1.1, the horizon form restricts to $\chi_{L_\pm|_S}(X,Y)=g(\nabla_X(L_\pm|_S),Y)$ on $TS$; differentiation in a tangent direction depends only on the restriction to $S$. Its $\gamma$-trace is therefore zero by [F2]. Write $a_\pm=e^{f_\pm}$ locally and apply the surface rescaling law in [F4] to obtain $\operatorname{tr}_\gamma\chi_{\ell_\pm}=0$. Linearity of the connection and the definitions in the Statement and [F3] give $\chi_{\ell_\pm}(X,Y)=-k(X,Y)\pm g(\nabla_X\nu,Y)$ and consequently $0=-\operatorname{tr}_S k\pm H_S$. No affine parametrization is used. [given, F2, F3, F4, step 1.1, step 2.1, algebra]

4.1 Adding the two equalities of step 3.1 gives $-2\operatorname{tr}_S k=0$; subtracting them gives $2H_S=0$. Thus both $\theta_\pm=\pm H_S+\operatorname{tr}_S k$ vanish for the normal pointing into the exterior. Replacing $k$ by $-k$ changes the sign of its trace and preserves both zero values. The argument has imposed no maximality condition. [given, step 3.1, algebra] ∎

---
title: Zero stationary field gives the local bifurcate Killing-horizon and
  boundary data
status: draft
research_item: lem-author-a4a441da4986-zero-stationary-boundary-data
dependency_level: 2
---

## Prerequisites

- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)
- [math:thm-flowout-theorem](https://alphabetamath.cc/item/thm-flowout-theorem)
- [math:thm-embedded-submanifolds-admit-local-defining-submersions](https://alphabetamath.cc/item/thm-embedded-submanifolds-admit-local-defining-submersions)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)



## Statement

Let $T$ be a nontrivial smooth Killing field on a connected smooth Lorentzian spacetime, vanishing on a smooth spacelike two-surface $S$. Suppose the two transverse smooth null sheets $H_+$ and $H_-$ meet in $S$ and $T$ is tangent to them. In a sufficiently small neighborhood of $S$, both sheets are Killing horizons for $T$: $T$ is nonzero, tangent and null-normal away from $S$. Thus they form a bifurcate Killing horizon in the standard neighborhood sense. If a smooth spacelike hypersurface has boundary $S$, its decomposition $T=Nn+X$ satisfies $N=X=0$ on $S$. This establishes a local Killing-horizon interface, not a global completion of the event horizons.

More precisely, at every $q\in S$ the linear map $A_q(v)=\nabla_vT$ annihilates $T_qS$ and preserves its Lorentzian normal two-plane, on which it is a nonzero skew map. Its two null eigenlines are the radical lines of the two sheets, with real eigenvalues $\lambda_q$ and $-\lambda_q$, where $\lambda_q\ne0$. If $\ell$ is a nonzero vector in either such line and $A_q\ell=a_q\ell$, the affinely parametrized null geodesic $\gamma_q(s)=\exp_q(s\ell)$ lies in that sheet near $s=0$ and satisfies $T_{\gamma_q(s)}=a_qs\dot\gamma_q(s)$. These geodesics, with smooth local choices of $\ell$ along $S$, cover a neighborhood of $S$ in the sheet. The sign of $a_q$ for a selected exterior and time orientation is not fixed by this generic assertion.

## Statement references

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity)

[def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)

[math:thm-flowout-theorem](https://alphabetamath.cc/item/thm-flowout-theorem)

[math:thm-embedded-submanifolds-admit-local-defining-submersions](https://alphabetamath.cc/item/thm-embedded-submanifolds-admit-local-defining-submersions)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[A1] The inherited stationary-data convention is ZFC, including the Axiom of Choice. Its choice function applied to any countable family supplies the countable choice required by the smooth-manifold, geodesic and flowout suppliers. No geodesic completeness or global Killing flow is assumed. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The Killing, smooth null-sheet, bifurcate-horizon and spacelike lapse–shift conventions are [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity) [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data). The null normal line is the radical of the induced form; its integral curves are not assumed affine or complete.

[F2] The smooth nondegenerate metric has a unique torsion-free metric-compatible connection. [physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[F3] On the stated time-oriented smooth Lorentzian four-manifold, geodesics with given position and velocity exist uniquely locally, depend smoothly on the initial data, obey affine scaling, and define an exponential map that is a local diffeomorphism at the zero vector. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F4] A smooth vector field on a boundaryless manifold has a unique smooth local flow on an open time–point domain, with the flow law and mutually inverse time maps. This applies to $T$ on $M$ and to a local radical field on an open part of a null sheet. [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)

[F5] The local flow of a smooth vector field transverse to an embedded codimension-one submanifold gives an embedded flowout, a diffeomorphism onto an open neighborhood of that submanifold. [math:thm-flowout-theorem](https://alphabetamath.cc/item/thm-flowout-theorem)

[F6] A smooth embedded hypersurface admits near each point a smooth defining function $u$ with $du\ne0$ and $H=\{u=0\}$. [math:thm-embedded-submanifolds-admit-local-defining-submersions](https://alphabetamath.cc/item/thm-embedded-submanifolds-admit-local-defining-submersions)

## Proof

**Given:** The smooth objects in the Statement, with the inherited ZFC convention in [A1] and the geometric interfaces in [F1]–[F6].

**Goal:** Identify the local generator and the zero boundary lapse and shift.

1.1 The local flow $\Phi_t$ of $T$ is defined on a common neighborhood for sufficiently small $t$. The flow law and the definition of Lie derivative give $\frac{d}{dt}\Phi_t^*g=\Phi_t^*(\mathcal L_Tg)=0$, so each such time map is a local isometry. Pulling the Levi–Civita connection back by this map gives another torsion-free metric-compatible connection; uniqueness makes it the same connection. Thus $\Phi_t$ takes affinely parametrized geodesics to affinely parametrized geodesics, with their pushed-forward initial velocities. Geodesic uniqueness yields $\Phi_t(\exp_p v)=\exp_{\Phi_t(p)}(d\Phi_t|_p v)$ whenever the geodesic segment and its image lie in the common local domain. These are local statements, requiring no complete flow. [given, A1, F1, F2, F3, F4]

1.2 Fix either null sheet $H$ near a point of $S$. Choose the local defining function $u$ from [F6] and set $L=(du)^\sharp$. Along $H$, this is a smooth nonzero field spanning $(TH)^\perp$, which equals the radical line in $TH$ because $H$ is null. Torsion-freeness makes the Hessian of $u$ symmetric: its antisymmetric part on $U,V$ is $U(Vu)-V(Uu)-[U,V]u=0$. Metric compatibility therefore gives, for every $Y\in TH$, $g(\nabla_LL,Y)=\operatorname{Hess}u(L,Y)=\operatorname{Hess}u(Y,L)=\tfrac12Y(g(L,L))=0$ on $H$. The last equality holds because $g(L,L)$ vanishes identically there. Hence $\nabla_LL=fL$ on $H$ for a smooth scalar $f$; smoothness follows locally by dividing any nonzero component of $L$. This proves the pregeodesic property rather than assuming it from the horizon terminology. [given, F1, F2, F6]

2.1 Write $A_p(v)=\nabla_vT$ and consider $Z=\{p:T_p=0,\ A_p=0\}$. It is closed by smoothness. If $p\in Z$, flow uniqueness fixes $p$, and in coordinates the variational equation for $J_t=d\Phi_t|_p$ is $J_t'=(dT)_pJ_t=0$, $J_0=\mathrm{id}$; here $(dT)_p=A_p$ because $T_p=0$. Hence $d\Phi_t|_p=\mathrm{id}$. The exponential identity of step 1.1 and the local diffeomorphism in [F3] make $\Phi_t$ the identity on a neighborhood of $p$ for all sufficiently small $t$. One may choose the neighborhood and time interval together by shrinking inside the open local-flow domain and a small exponential-coordinate ball. Differentiating at $t=0$ makes $T$ zero there, hence also $\nabla T=0$ there. Thus $Z$ is open. If nonempty it is all of connected $M$, contradicting the nontriviality of $T$. Therefore $Z$ is empty. [given, F3, F4, step 1.1]

2.2 The radical line is transverse to $S$ inside $H$: a nonzero null vector cannot lie in the positive-definite plane $T_qS$. Let $\Psi_r$ be the local flow of $L|_H$. Applied within the three-manifold $H$ to a small embedded patch of its codimension-one submanifold $S$, [F5] makes $(r,q)\mapsto\Psi_r(q)$ a diffeomorphism onto an open sheet neighborhood. Along each curve define $c_q(r)=\exp(\int_0^r f(\Psi_v(q))\,dv)$ and $s_q(r)=\int_0^r c_q(v)\,dv$. Then $c_q>0$, $s_q'=c_q$ and $c_q'=fc_q$. Reparametrizing by $s=s_q(r)$ gives velocity $L/c_q$ and acceleration $c_q^{-2}(\nabla_LL-(c_q'/c_q)L)=0$. Its initial velocity is $L_q$, so [F3] identifies it with $\gamma_q(s)=\exp_q(sL_q)$. The strictly increasing parameter change preserves this local coverage and has $s=0$ exactly on $S$. Thus these affine null-normal geodesics issuing from $S$ cover the sheet locally, with nonzero tangent $L/c_q$. [given, A1, F3, F4, F5, step 1.2]

3.1 At $q\in S$, differentiating the zero restriction $T|_S$ gives $A_q|_{T_qS}=0$. Metric compatibility, torsion-freeness and $\mathcal L_Tg=0$ give $g(\nabla_UT,V)+g(U,\nabla_VT)=0$, so $A_q$ is $g$-skew. Consequently its image lies in $(T_qS)^\perp$, and this Lorentzian normal two-plane is invariant. In a null basis $\ell_+,\ell_-$ with $g(\ell_+,\ell_-)=-1$, skewness forces $A_q\ell_+=\lambda_q\ell_+$ and $A_q\ell_-=-\lambda_q\ell_-$. If $\lambda_q=0$ then $A_q=0$ on both the normal plane and $T_qS$, putting $q$ in $Z$, impossible by step 2.1. Thus $\lambda_q\ne0$. [given, F1, F2, step 2.1]

4.1 At each $q\in S$ the two transverse sheets have distinct radical lines in $(T_qS)^\perp$: coincident radicals would give equal tangent hyperplanes, each the orthogonal complement of that same line. Label their local nonzero initial fields $\ell_\pm$ accordingly. Step 3.1 gives the respective eigenvalues $\pm\lambda_q$. Since the Killing flow fixes $q$, its differential satisfies the constant-coefficient variational equation with coefficient $A_q$ and hence sends $\ell_\pm$ to $e^{\pm t\lambda_q}\ell_\pm$. By step 1.1 and geodesic scaling, $\Phi_t(\exp_q(s\ell_\pm))=\exp_q(e^{\pm t\lambda_q}s\ell_\pm)$ for small parameters. Differentiating at $t=0$ gives $T=\pm\lambda_qs\partial_s$ on the sheet. Step 2.2 ensures that these coordinates cover a neighborhood in each sheet and that $\partial_s$ spans its radical. Thus $T$ is tangent, null-normal and nonzero away from $S$. Taking the union of sufficiently small such neighborhoods along $S$ gives the claimed neighborhood sense of a bifurcate Killing horizon. No uniform collar width for noncompact $S$, all-time flow, global causal completion or compact-core section is inferred. [given, F1, F3, F4, step 1.1, step 3.1, step 2.2]

5.1 Finally $N=-g(T,n)=0$ at $S$ and $X=T-Nn=0$ there by the orthogonal decomposition. Conversely if $T$ is tangent to both sheets and lies in the null-generator line of either at their spacelike intersection, it is a vector of $TS$ which is also null, and is therefore zero. These pointwise boundary consequences require no maximal slice. [given, F1, step 4.1] ∎

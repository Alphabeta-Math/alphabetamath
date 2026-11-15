---
title: A Riemannian Killing shift vanishing on the whole boundary vanishes globally
status: published
research_item: lem-author-a4a441da4986-boundary-fixed-killing-shift
dependency_level: 1
---

## Prerequisites

- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)
- [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry)
- [math:prop-christoffel-formula-for-the-levi-civita-connection](https://alphabetamath.cc/item/prop-christoffel-formula-for-the-levi-civita-connection)
- [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)
- [math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor](https://alphabetamath.cc/item/prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor)
- [math:thm-clairaut-schwarz-mixed-partials](https://alphabetamath.cc/item/thm-clairaut-schwarz-mixed-partials)
- [math:thm-picard-lindelof-local-existence-and-uniqueness](https://alphabetamath.cc/item/thm-picard-lindelof-local-existence-and-uniqueness)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-connected-space](https://alphabetamath.cc/item/def-connected-space)


## Statement

Work in ZFC. Let $(P,h)$ be a connected smooth Riemannian manifold with nonempty smooth boundary. Let $X$ be a smooth vector field up to the boundary, Killing on the interior in the sense that $\mathcal L_Xh=0$ there, with $X|_{\partial P}=0$. Then $X=0$ everywhere on $P$.

Consequently, let a supplied smooth stationary maximal spacelike hypersurface $\overline\Sigma$ have induced Riemannian metric smooth and positive definite up to its smooth boundary, with its normal and stationary lapse–shift decomposition smooth there. Require that every connected component of $\overline\Sigma$ have nonempty boundary. If $k=0$ and $T|_{\partial\overline\Sigma}=0$, then its stationary shift vanishes everywhere. Here stationarity means $\mathcal L_Tg=0$, and the conventions are $g(n,n)=-1$, $N=-g(T,n)$, $T=Nn+X$ and $k(U,V)=-g(\nabla_U n,V)$.

## Statement references

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry)

[math:prop-christoffel-formula-for-the-levi-civita-connection](https://alphabetamath.cc/item/prop-christoffel-formula-for-the-levi-civita-connection)

[math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)

[math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor](https://alphabetamath.cc/item/prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor)

[math:thm-clairaut-schwarz-mixed-partials](https://alphabetamath.cc/item/thm-clairaut-schwarz-mixed-partials)

[math:thm-picard-lindelof-local-existence-and-uniqueness](https://alphabetamath.cc/item/thm-picard-lindelof-local-existence-and-uniqueness)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:def-connected-space](https://alphabetamath.cc/item/def-connected-space)

## Facts & Assumptions

[A1] ZFC, including the Axiom of Choice, is the inherited convention for the stationary data. In the stationary application it supplies the countable choice required by the ambient connection interface; the local coordinate propagation below makes no additional family choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F1] A Riemannian metric is a smooth positive-definite symmetric covariant two-tensor. Boundary charts have relatively open half-space images, with smoothness in the local-extension sense. Thus after shrinking a chart, its finitely many metric and field components have smooth extensions to an open Euclidean neighborhood. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[F2] A smooth Riemannian metric, including at a smooth boundary, has a unique torsion-free metric-compatible connection $D$. Its coordinate symbols are $\Gamma^\ell{}_{ij}=\tfrac12h^{\ell a}(\partial_i h_{ja}+\partial_j h_{ia}-\partial_a h_{ij})$. [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry) [math:prop-christoffel-formula-for-the-levi-civita-connection](https://alphabetamath.cc/item/prop-christoffel-formula-for-the-levi-civita-connection)

[F3] For a smooth vector field $V$ with local flow $\Phi_t$ and a smooth covariant two-tensor $m$, the Lie derivative is $\mathcal L_Vm=\left.\frac{d}{dt}\right|_{t=0}\Phi_t^*m$ on each local flow domain. In coordinates, $(\mathcal L_Vm)_{ij}=V^a\partial_a m_{ij}+m_{aj}\partial_iV^a+m_{ia}\partial_jV^a$. This is used on boundaryless interiors and ambient charts; smooth identities then extend to boundary points by continuity. [math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor](https://alphabetamath.cc/item/prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor) [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)

[F4] Second partial derivatives of a $C^2$ function on an open Euclidean set commute. At boundary points this applies to the local smooth extensions in [F1]. [math:thm-clairaut-schwarz-mixed-partials](https://alphabetamath.cc/item/thm-clairaut-schwarz-mixed-partials)

[F5] For a continuous first-order system on an open time–state domain, locally Lipschitz in the state, two solutions with the same initial data agree on every common subinterval containing the initial time. In particular this applies to $z'=B(t)z$ when the matrix $B$ is smooth. [math:thm-picard-lindelof-local-existence-and-uniqueness](https://alphabetamath.cc/item/thm-picard-lindelof-local-existence-and-uniqueness)

[F6] The stationary data supply the smooth Lorentzian metric, its torsion-free metric-compatible connection $\nabla$, and $\mathcal L_Tg=0$. The hypersurface conventions supply the positive-definite induced metric, smooth unit normal, $N=-g(T,n)$, $X=T-Nn$, and $k(U,V)=-g(\nabla_U n,V)$. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F7] A topological space is connected when it has no separation into two nonempty disjoint open subsets. Equivalently, its only clopen subsets are the empty set and the whole space. [math:def-connected-space](https://alphabetamath.cc/item/def-connected-space)

## Proof

**Given:** The smooth boundary and Killing data of the Statement, with [A1] and [F1]–[F7].

**Goal:** Propagate the zero first jet from a boundary point and apply the result to the stationary shift.

1.1 For any smooth metric $m$ with torsion-free compatible connection $\nabla^m$, expanding [F3] and using compatibility gives $(\mathcal L_Vm)(U,W)=m(\nabla^m_UV,W)+m(U,\nabla^m_WV)$. Apply this to $h$ on the interior and extend to the boundary by smoothness. Thus $A_p(v)=D_vX$ is $h$-skew at every $p$. At $p\in\partial P$, differentiating the zero restriction of $X$ in each boundary tangent direction gives $A_p(v)=0$ for $v\in T_p\partial P$. If $\nu$ is a unit normal to that hyperplane in $T_pP$, skewness gives $h(A_p\nu,v)=-h(\nu,A_pv)=0$ for all boundary tangent $v$, and $h(A_p\nu,\nu)=0$. Positive definiteness implies $A_p\nu=0$, so $(X,DX)_p=(0,0)$. This also covers dimension one, where the tangent hyperplane is zero dimensional. [given, F1, F2, F3]

1.2 In a coordinate chart put $u_j=h_{ja}X^a$ and $E_{ij}=2\Gamma^\ell{}_{ij}u_\ell$. The coordinate formula in [F2] and the Lie derivative formula in [F3] give the Killing equation $\partial_i u_j+\partial_j u_i=E_{ij}$. Differentiate its $(j,k)$ equation by $i$, its $(i,k)$ equation by $j$, and subtract the derivative by $k$ of its $(i,j)$ equation. By [F4] the left side is $2\partial_i\partial_j u_k$. Consequently
$$\partial_i\partial_j u_k=(\partial_i\Gamma^\ell{}_{jk}+\partial_j\Gamma^\ell{}_{ik}-\partial_k\Gamma^\ell{}_{ij})u_\ell+\Gamma^\ell{}_{jk}\partial_i u_\ell+\Gamma^\ell{}_{ik}\partial_j u_\ell-\Gamma^\ell{}_{ij}\partial_k u_\ell.$$
The equality holds up to the boundary by continuity. Hence the finite list $Y=(u_j,\partial_i u_j)$ satisfies $\partial_rY=A_r(x)Y$ for smooth matrix functions $A_r$: the derivatives of its first entries are entries of $Y$, and the displayed identity supplies the derivatives of all remaining entries. These matrices depend only on $h$ and its derivatives. [F1, F2, F3, F4, step 1.1, algebra]

2.1 Let $p$ have $(X,DX)_p=(0,0)$. Choose a sufficiently small convex coordinate ball, or ball intersected with the closed half-space at a boundary point. By [F1] the metric coefficients extend smoothly to a full ball about $p$; after shrinking, positive definiteness persists, so the Christoffel formula extends each matrix $A_r$ smoothly too. For any $q$ in a smaller such relative ball, the straight coordinate segment $x(t)=x(p)+t(x(q)-x(p))$, $0\le t\le1$, lies in the chart, and $Y(x(t))$ satisfies $z'=B(t)z$, where $B(t)=(x(q)-x(p))^rA_r(x(t))$ extends smoothly to an open interval containing $[0,1]$. Since $X_p=0$, differentiation of $u_j=h_{ja}X^a$ gives $\partial_i u_j(p)=h_{ja}(D_iX)^a(p)=0$, hence $z(0)=0$. To apply [F5] with an interior initial time even if $p$ is on the boundary, extend this solution by zero for small negative $t$: the right derivative at zero is $B(0)z(0)=0$, so this is a $C^1$ solution across zero. It agrees with the zero solution on $[0,1]$ by [F5]. Thus $Y(q)=0$ throughout the smaller relative neighborhood; equivalently $X=DX=0$ there. [given, F1, F2, F5, step 1.2]

3.1 The set $Z=\{p\in P:X_p=0,\ (DX)_p=0\}$ is closed by smoothness and open by step 2.1. It is nonempty by step 1.1 and the nonempty boundary. Connectedness of $P$ gives $Z=P$, proving the first assertion. This argument uses relative neighborhoods at the boundary and does not require a flow or boundary normal geodesics. [given, F1, F2, F7, step 1.1, step 2.1]

4.1 For the stationary application, define $\widehat D_UV=(\nabla_UV)^\top$ for tangent fields on the hypersurface. The ambient torsion-free property and tangency of the bracket give zero torsion, and ambient metric compatibility gives $U h(V,W)=h(\widehat D_UV,W)+h(V,\widehat D_UW)$. By uniqueness in [F2], $\widehat D=D$ for the induced metric. The identity proved in step 1.1, now for $g,T$, gives $0=g(\nabla_UT,V)+g(U,\nabla_VT)$. Substitute $T=Nn+X$. Orthogonality removes the derivatives of $N$, and the definition of $k$ yields $h(D_UX,V)+h(U,D_VX)=N(k(U,V)+k(V,U))$. If $k=0$ this is the Riemannian Killing equation. At the boundary $T=0$ implies $N=-g(T,n)=0$ and then $X=T-Nn=0$. Apply step 3.1 separately to each connected component, which by hypothesis has nonempty boundary. Therefore $X=0$ everywhere. This deduction uses no vacuum equation and no null-sheet hypothesis. [given, A1, F1, F2, F3, F6, step 1.1, step 3.1] ∎

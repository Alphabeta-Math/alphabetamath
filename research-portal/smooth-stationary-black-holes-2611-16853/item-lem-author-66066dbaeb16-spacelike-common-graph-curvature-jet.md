---
title: Mean curvature at identical spacelike graph jets has positive Hessian symbol
status: draft
research_item: lem-author-66066dbaeb16-spacelike-common-graph-curvature-jet
dependency_level: 1
---

## Prerequisites

- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)
- [math:thm-euclidean-inverse-function-theorem](https://alphabetamath.cc/item/thm-euclidean-inverse-function-theorem)
- [math:thm-higher-regularity-of-local-inverses](https://alphabetamath.cc/item/thm-higher-regularity-of-local-inverses)
- [math:def-ck-euclidean-maps-and-diffeomorphisms](https://alphabetamath.cc/item/def-ck-euclidean-maps-and-diffeomorphisms)
- [math:thm-ck-euclidean-maps-closed-under-algebra-and-composition](https://alphabetamath.cc/item/thm-ck-euclidean-maps-closed-under-algebra-and-composition)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [math:prop-coordinate-geodesic-equation](https://alphabetamath.cc/item/prop-coordinate-geodesic-equation)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work under the inherited ZFC convention. Let $(M,g)$ be a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$ with its Levi–Civita connection. Let two embedded $C^2$ spacelike hypersurfaces $\Sigma_f,\Sigma_g$ meet at $p$ with the same tangent hyperplane $P$ and future unit normal $n$. At an interior point, $C^2$ means an embedded local parametrization of rank three with $C^2$ coordinate components. At a boundary point, the local parametrization is an embedding of a relatively open subset of $\{(z_1,z_2,r):r\ge0\}$, of rank three also on $r=0$, with all coordinate partial derivatives through order two continuous up to the edge. For the common-boundary conclusion, assume their boundary images agree near $p$ and that their projected interiors select the same side of the projected boundary.

There are local coordinates $(t,x^1,x^2,x^3)$ with $\partial_t$ future-directed timelike in which the hypersurfaces are $C^2$ graphs $t=f(x)$ and $t=g(x)$ with equal value and first derivative at the contact point. Use the convention $H=\operatorname{tr}_h g(\nabla n,\cdot)=\operatorname{div}_g n$, where divergence is evaluated using a local unit $C^1$ timelike extension of the future normal. More generally, in any smooth common graph chart with positive future-normal component $\alpha=-g(n,\partial_t)>0$ at $p$, put $E_i=\partial_i+f_i\partial_t$ at the shared first jet, $h_{ij}=g(E_i,E_j)$, and let $(h^{ij})$ be its inverse. Then, with all coefficients and derivatives evaluated at $p$,
$$H(\Sigma_f)-H(\Sigma_g)=A^{ij}\partial_{ij}(f-g),\qquad A^{ij}=\alpha h^{ij}.$$
The matrix $A$ is positive definite. The orientation condition holds in particular for future-directed timelike $\partial_t$.

One can choose Lorentzian normal coordinates centered at $p$, with $\partial_t|_p=n$ and the spatial coordinate vectors an orthonormal basis of $P$. In these coordinates $Df(p)=Dg(p)=0$ and $A$ is the identity. At a common boundary point the graph functions have $C^2$ extensions across their common projected $C^2$ boundary. A common $C^2$ spatial coordinate change flattening that boundary gives graphs on the same half-neighborhood, and the Hessian-difference formula retains a positive-definite coefficient there; the identity-matrix assertion refers to the unflattened normal coordinates.

## Facts & Assumptions

[F1] The induced tangent form is positive definite, and the sign conventions are $k(U,V)=-g(\nabla_U n,V)$ and $H=-\operatorname{tr}_h k=\operatorname{div}_g n$ for a unit normal extension. The $C^2$ version is constructed in the proof. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F2] The exponential map is smooth near zero, has differential the identity there, and satisfies $\exp_p(sv)=\gamma_{p,v}(s)$ for small $s$. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F3] A smooth map with invertible differential is a local smooth diffeomorphism. This applies to the exponential map in the normal-chart construction. [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

[F4] A $C^1$ Euclidean map with invertible derivative has a local $C^1$ inverse, and for a $C^2$ map that inverse is $C^2$. These results apply in both dimensions three and two below. [math:thm-euclidean-inverse-function-theorem](https://alphabetamath.cc/item/thm-euclidean-inverse-function-theorem) [math:thm-higher-regularity-of-local-inverses](https://alphabetamath.cc/item/thm-higher-regularity-of-local-inverses)

[F5] The Levi–Civita connection is torsion-free and metric-compatible; in coordinates $\nabla_{\partial_b}\partial_c=\Gamma^a{}_{bc}\partial_a$. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F6] Geodesics satisfy $\ddot y^a+\Gamma^a{}_{bc}(y)\dot y^b\dot y^c=0$ in any coordinate chart. [math:prop-coordinate-geodesic-equation](https://alphabetamath.cc/item/prop-coordinate-geodesic-equation)

[F7] $C^2$ Euclidean maps have continuous derivatives through order two, and their finite componentwise sums, products and compositions remain $C^2$. [math:def-ck-euclidean-maps-and-diffeomorphisms](https://alphabetamath.cc/item/def-ck-euclidean-maps-and-diffeomorphisms) [math:thm-ck-euclidean-maps-closed-under-algebra-and-composition](https://alphabetamath.cc/item/thm-ck-euclidean-maps-closed-under-algebra-and-composition)

[F8] The ambient metric has Lorentz signature $(-,+,+,+)$; time orientation selects one timelike cone, and future-directedness and orthonormal frames have their Lorentzian meanings. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[F9] Total derivatives satisfy $D(v\circ u)=(Dv\circ u)Du$; applying this to $C^2$ maps and differentiating once more gives the second-derivative transformation used below. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[A1] The geometric suppliers retain their inherited Axiom of Choice convention; this proof adds no choice assumption beyond ZFC. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The assumptions and conventions in the Statement.

**Goal:** Construct the stated graphs and prove the oriented Hessian-difference formula, including the normal-coordinate and common-boundary assertions.

1.1 Construct the needed finite-regularity extension directly in an ambient smooth coordinate chart. For a boundary parametrization $q(z,r)$ on a small half-box, keep $\widetilde q=q$ for $r\ge0$ and, for sufficiently small $r<0$, set $\widetilde q(z,r)=6q(z,-r)-8q(z,-2r)+3q(z,-3r)$, componentwise. The sums of the coefficients multiplied by $(-j)^k$, for $j=1,2,3$, are $1$ for $k=0,1,2$. Consequently every tangential/normal partial derivative of total order at most two has the same limiting value from both sides of $r=0$. Difference quotients across the edge first give the matching first derivatives and then the matching second derivatives; hence $\widetilde q$ is $C^2$. After shrinking, its values stay in the ambient chart and its derivative retains rank three near the contact point. This gives the required $C^2$ extension. [F7, F9, given, algebra]

1.2 Choose an orthonormal basis $e_1,e_2,e_3$ of $P$ by finite Gram–Schmidt and put $e_0=n$. Use the map $y\mapsto\exp_p(y^ae_a)$ as a normal chart: [F2] gives its smoothness and identity differential at zero and [F3] gives a smooth local inverse. The coordinate vectors at zero are therefore $e_a$, so $g_{ab}(0)=\operatorname{diag}(-1,1,1,1)_{ab}$. By exponential scaling, each radial coordinate curve $s\mapsto sv$ is a geodesic. At zero [F6] gives $\Gamma^a{}_{bc}(0)v^bv^c=0$ for every $v$. Torsion freedom makes the lower indices symmetric, and polarization gives $\Gamma^a{}_{bc}(0)=0$. Metric compatibility then gives $\partial_cg_{ab}(0)=\Gamma^d{}_{ca}(0)g_{db}(0)+\Gamma^d{}_{cb}(0)g_{ad}(0)=0$. These Lorentzian center identities have been proved here, rather than imported from a Riemannian normal-coordinate theorem. [F1, F2, F3, F5, F6, F8, A1, given, algebra]

2.1 Choose a smooth ambient chart whose time vector at $p$ is $n$ and whose spatial coordinate vectors span $P$; by continuity the time vector remains future timelike nearby. The projection $\pi(t,x)=x$ restricts to an isomorphism on $P$, because its kernel is the timelike time line and $P$ is spacelike. For either interior parametrization, or the extension from step 1.1, the map $\pi\circ\widetilde q$ therefore has invertible derivative. Apply [F4] to obtain its $C^2$ local inverse; composing the time component of $\widetilde q$ with that inverse gives the $C^2$ graph function. Equality of the tangent hyperplanes gives $Df(p)=Dg(p)$; both graphs pass through $p$, so their values agree as well. In a general chart with $\alpha>0$, the time vector is again transverse to $P$, and the same projection argument applies. [F1, F4, F7, F8, F9, step 1.1, given]

3.1 In the boundary case the graph projection is a $C^2$ diffeomorphism on each extended parametrization. Its restriction to the rank-two boundary parametrization is thus a rank-two embedded $C^2$ surface in $\mathbb R^3$. These two projected boundaries agree, since the original boundary images agree. After a spatial linear change choose two projected components with invertible derivative on a boundary parametrization and use [F4] in dimension two to express the boundary as $x^3=\psi(x^1,x^2)$ with $\psi$ of class $C^2$. Each projected interior lies on one side: in the projected parametrization the differential of $x^3-\psi(x^1,x^2)$ vanishes in the two boundary directions and is nonzero in the inward direction, so its sign is fixed for small positive $r$. The common-side hypothesis selects the same sign for both. Reverse the transverse spatial coordinate if necessary, and set $x=\chi(y)=(y^1,y^2,y^3+\psi(y^1,y^2))$. Its explicit inverse subtracts $\psi$ in the third coordinate; it maps a sufficiently small common half-neighborhood $y^3\ge0$ onto the selected side. The extended graph functions from step 2.1 restrict to the original graphs there. [F4, F7, F9, step 2.1, given, algebra]

3.2 The normal and mean curvature require only the stated $C^2$ regularity. For an extended graph $f$, put $E_i=\partial_i+f_i(x)\partial_t$ throughout a small ambient neighborhood. Their Gram matrix $h$ remains positive definite near the graph. With $T=\partial_t$ and $h^{-1}=(h^{ij})$, define $u=T-h^{ij}g(T,E_i)E_j$. Then $u$ is orthogonal to the three $E_i$, is nonzero by transversality, and is timelike: the orthogonal complement of a positive three-plane in signature $(-,+,+,+)$ is a negative line. The field $u$ is $C^1$, so normalizing it and choosing its future sign gives a unit $C^1$ ambient extension $\widetilde n$ of the future graph normal. Metric compatibility gives $g(\nabla_{\widetilde n}\widetilde n,\widetilde n)=\tfrac12\widetilde n\,g(\widetilde n,\widetilde n)=0$. Thus the ambient divergence trace on the graph equals $h^{ij}g(\nabla_{E_i}n,E_j)$, independently of unit extension. Differentiating $g(n,E_j)=0$ tangentially yields [step 2.1]
$$H(f)=-h^{ij}g(n,\nabla_{E_i}E_j).$$
All differentiations are valid for $C^1$ fields, including the one-sided limits at a boundary. [F1, F5, F7, F8, F9, step 2.1, algebra]

4.1 Write $E_i^a$ for the components of the graph tangent vectors, with $a=0,1,2,3$. The coordinate connection formula gives $\nabla_{E_i}E_j=f_{ij}\partial_t+\Gamma^a{}_{bc}E_i^bE_j^c\partial_a$. At the shared point and first jet, the two graphs have identical $E_i$, $h^{ij}$ and future normal $n$, and the Christoffel terms are evaluated at the same ambient point. Subtracting the two formulas from step 3.2 therefore cancels every Christoffel term and gives [step 3.2]
$$H(f)-H(g)=-g(n,\partial_t)h^{ij}(f-g)_{ij}.$$
Since $h^{-1}$ is positive definite and $\alpha=-g(n,\partial_t)>0$, this is the asserted positive-definite symbol. For a future timelike $\partial_t$, write $\partial_t=a n+V$ with $V\in P$; the future cone in the orthonormal frame with time vector $n$ has $a>0$, and $\alpha=a$. Thus that sufficient orientation condition has precisely the required sign. [F1, F5, F8, step 3.2, given, algebra]

5.1 Apply the graph construction of step 2.1 in this normal chart. Both graph values at the center and both first derivatives vanish. There $\partial_t=n$, $h_{ij}=\delta_{ij}$ and $\alpha=1$, so step 4.1 gives $A^{ij}=\delta^{ij}$. In addition the vanishing Christoffel symbols from step 1.2 and step 3.2 give $H(f)=\sum_i f_{ii}$ and $H(g)=\sum_i g_{ii}$ individually at the center. [step 2.1, step 3.2, step 4.1, step 1.2, algebra]

6.1 For the common spatial flattening $x=\chi(y)$ from step 3.1, let $w=f-g$ and $B=D\chi$ at contact. The first jet of $w$ vanishes, so applying [F9] twice gives $D_y^2(w\circ\chi)=B^T(D_x^2w)B$: the terms involving $Dw$ and second derivatives of $\chi$ vanish. Hence the contracted coefficient in the flattened variables is $\widetilde A=B^{-1}AB^{-T}$, which is positive definite because $B$ is invertible. Time is unchanged in this spatial change. The $C^2$ extensions and their restrictions have the same derivatives through order two on the boundary, so the formulas calculate the original boundary mean curvatures and do not depend on the chosen extensions. This proves the common half-neighborhood assertion as well as the interior and normal-coordinate assertions. [F7, F9, step 1.1, step 3.1, step 4.1, step 5.1, algebra] ∎

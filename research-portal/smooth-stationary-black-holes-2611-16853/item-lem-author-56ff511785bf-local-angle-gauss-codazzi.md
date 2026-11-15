---
title: Pointwise Gauss–Codazzi identities for the normal angle
status: published
research_item: lem-author-56ff511785bf-local-angle-gauss-codazzi
dependency_level: 1
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum, arXiv:2610.09729v1
      url: https://arxiv.org/pdf/2610.09729v1
      locator: Appendix B, Lemma B.1 statement, printed/PDF pp.35–36; proof, equation
        (B.8) and following (B.9)–(B.11), pp.38–39
      reading_limits: Consulted the retrieved v1 PDF text of the Lemma B.1 statement
        on pp.35–36 and its proof on pp.38–39, including (B.8)–(B.11).
        Screenshot retrieval was unavailable. The citation records the
        differentiation method; the local proof differentiates v directly, uses
        neither log v nor arcosh v, and imports no weighted estimate or
        compact-positive-portion hypothesis.
      statement: "Method attribution: equation (B.8) differentiates the normal angle
        and its tangential observer components and traces the second derivative
        on a maximal hypersurface. The subsequent arcosh estimate is restricted
        to v>2. No estimate from that argument is imported here."
      hypotheses: The cited lemma assumes a C2-convergent Lorentzian metric family
        near a fixed compact set, a fixed smooth temporal function with
        uniformly timelike gradient there, and smooth maximal hypersurfaces with
        compact nonnegative-height portions. The local identities below are
        proved directly for the smooth hypersurface and arbitrary smooth unit
        observer in the Statement.
---

## Prerequisites

- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)
- [physics:thm-gr-curvature-algebraic-symmetries](https://alphabetamath.cc/physics/item/thm-gr-curvature-algebraic-symmetries)
- [math:prop-properties-of-normal-coordinates-at-the-center](https://alphabetamath.cc/item/prop-properties-of-normal-coordinates-at-the-center)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-existence-of-normal-neighborhoods](https://alphabetamath.cc/item/thm-existence-of-normal-neighborhoods)
- [math:def-normal-neighborhood-and-normal-coordinate-chart](https://alphabetamath.cc/item/def-normal-neighborhood-and-normal-coordinate-chart)
- [` Alexandru F. Radu, Rigidity of stationary black holes with small ADM angular momentum, arXiv:2610.09729v1 · Appendix B, Lemma B.1 statement, printed/PDF pp.35–36; proof, equation (B.8) and following (B.9)–(B.11), pp.38–39 `](https://arxiv.org/pdf/2610.09729v1)


## Statement

Let $\Sigma$ be a smooth spacelike maximal hypersurface in a smooth time-oriented Lorentzian four-manifold, with future normal $n$, induced metric $h$, and $k(X,Y)=-g(D_Xn,Y)$, where $D$ is the Levi–Civita connection. Let $U$ be any smooth ambient future unit timelike field and $v=-g(n,U)$. Write $\nabla$ for the induced covariant derivative and $\Delta=\operatorname{tr}_h\nabla^2$. At a point choose an $h$-orthonormal frame $(e_a)_{a=1}^3$ with $\nabla_{e_a}e_b=0$, and put $Z_b=g(U,e_b)$. Then $\nabla_av=k_{ab}Z_b-g(n,D_{e_a}U)$, $\nabla_aZ_b=g(D_{e_a}U,e_b)+vk_{ab}$, and $\nabla^ak_{ab}=-\operatorname{Ric}(n,e_b)$. In particular $\Delta v=v|k|^2+(\nabla^ak_{ab})Z_b+2k_{ab}g(e_b,D_{e_a}U)-g(n,\sum_a(D^2U)(e_a,e_a))$, where $(D^2U)(X,Y)=D_XD_YU-D_{D_XY}U$. Repeated tangent indices are summed from one to three. The formulas are local, with no compactness assumption on $\Sigma$.

## Facts & Assumptions

[F1] Use the spacelike metric $h$, future normal $n$, symmetric negative-sign form $k$ and maximality $\operatorname{tr}_h k=0$ from [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data). The ambient connection $D$ is metric compatible and torsion free by [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection). For vectors along $\Sigma$ put $P(W)=W+g(W,n)n$ and define $\nabla_XY=P(D_XY)$ for tangent $X,Y$; step 1.1 proves that this is the Levi–Civita connection of $h$. Its scalar Hessian is $\nabla^2 f(X,Y)=X(Yf)-(\nabla_XY)f$, its Laplacian is the $h$-trace of that Hessian, and its covariant derivative on a covariant tensor subtracts one $\nabla_X$ correction in each tensor slot.

[F2] Curvature means $R(X,Y)Z=D_XD_YZ-D_YD_XZ-D_{[X,Y]}Z$ and $\operatorname{Ric}(n,Y)=\operatorname{tr}(Z\mapsto R(Z,Y)n)$. The curvature definitions and skew-adjointness are [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors) and [physics:thm-gr-curvature-algebraic-symmetries](https://alphabetamath.cc/physics/item/thm-gr-curvature-algebraic-symmetries).

[F3] Work in ZFC, carrying the inherited countable-choice assumptions of the geometric suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) At each point of a boundaryless intrinsic neighborhood in $(\Sigma,h)$, [math:thm-existence-of-normal-neighborhoods](https://alphabetamath.cc/item/thm-existence-of-normal-neighborhoods) supplies a normal neighborhood. With a finite orthonormal basis at that point, [math:def-normal-neighborhood-and-normal-coordinate-chart](https://alphabetamath.cc/item/def-normal-neighborhood-and-normal-coordinate-chart) defines its normal coordinates, and [math:prop-properties-of-normal-coordinates-at-the-center](https://alphabetamath.cc/item/prop-properties-of-normal-coordinates-at-the-center) gives $h_{ij}(p)=\delta_{ij}$, $\Gamma^k{}_{ij}(p)=0$ and $\partial_kh_{ij}(p)=0$. Step 2.1 constructs the required orthonormal frame from those coordinates. These inputs apply to the positive intrinsic metric, not to the ambient Lorentzian metric.

## Proof

**Given:** The maximal hypersurface and ambient observer. **Goal:** Construct the induced connection and normal frame, then derive the displayed angle and contracted curvature identities.

1.1 Along $\Sigma$, $g(P(W),n)=0$ and $P$ is the identity on tangent vectors. The tangential derivative $D_XY$ is independent of the ambient extension of $Y$: in an adapted chart the components of a field vanishing along $\Sigma$ have zero tangential derivatives there, and its connection term also vanishes. Thus $\nabla_XY=P(D_XY)$ is well defined and smooth. The affine-connection rules follow by applying $P$ to those of $D$. For tangent $X,Y,Z$, metric compatibility gives $Xh(Y,Z)=h(\nabla_XY,Z)+h(Y,\nabla_XZ)$, and torsion freedom gives $\nabla_XY-\nabla_YX=P([X,Y])=[X,Y]$. To see uniqueness, add the compatibility identities for $Xh(Y,Z)$ and $Yh(Z,X)$, subtract the one for $Zh(X,Y)$, and substitute torsion freedom; this gives $2h(\nabla_XY,Z)=Xh(Y,Z)+Yh(Z,X)-Zh(X,Y)+h([X,Y],Z)+h([Z,X],Y)-h([Y,Z],X)$ for any such connection. Nondegeneracy of $h$ determines $\nabla_XY$ uniquely. Finally $g(D_XY,n)=-g(Y,D_Xn)=k(X,Y)$, so $D_XY=\nabla_XY-k(X,Y)n$. This constructs the induced connection and its Gauss decomposition without a positive-definite ambient hypothesis. [F1, given, algebra]

2.1 Fix a point $p$ and a boundaryless intrinsic neighborhood of it. Apply [F3] to its Riemannian metric $h$ and the connection identified in step 1.1. A finite basis of $T_p\Sigma$ can be orthonormalized by successive subtraction of projections and division by positive lengths; this uses only finite choices. The associated normal coordinate fields $E_i$ satisfy $h(E_i,E_j)(p)=\delta_{ij}$, $\nabla E_i(p)=0$ and $d(h(E_i,E_j))(p)=0$. Apply the same Gram–Schmidt formulas smoothly to $E_i$ near $p$. Their denominators remain positive after shrinking the neighborhood. At $p$ every normalization factor is one and every off-diagonal projection coefficient is zero; differentiating these formulas, the vanishing first metric derivatives make all coefficient derivatives zero. Thus the resulting local $h$-orthonormal frame $e_a$ agrees with $E_a$ to first order at $p$ and satisfies $\nabla_{e_a}e_b(p)=0$. Only the inherited $\mathrm{AC}_\omega$ of the normal-coordinate and ambient geometric inputs is used, as supplied by ZFC. [F1, F3, step 1.1, choose, algebra]

3.1 At the chosen point metric compatibility gives $D_{e_a}n=-k_{ab}e_b$ and step 1.1 gives $D_{e_a}e_b=-k_{ab}n$ because its tangential covariant derivative vanishes by step 2.1. Differentiate $v=-g(n,U)$ and $Z_b=g(U,e_b)$ to obtain $\nabla_av=k_{ab}Z_b-g(n,D_{e_a}U)$ and $\nabla_aZ_b=g(D_{e_a}U,e_b)+vk_{ab}$. The components $Z_b$ are those of the tangential covector $Z(X)=g(U,X)$. With its covariant derivative as defined in [F1], these are tensorial first-derivative formulas and hold in every induced frame. [F1, step 1.1, step 2.1, given, algebra]

4.1 Commuting the two ambient derivatives of $n$ and pairing with $e_c$ gives $(\nabla_ak)_{bc}-(\nabla_bk)_{ac}=-g(R(e_a,e_b)n,e_c)$. Indeed, differentiate $k(e_b,e_c)=-g(D_{e_b}n,e_c)$, subtract the expression with $a,b$ interchanged and the induced connection corrections, and use the Gauss decomposition from step 1.1; the normal components of $D e_c$ pair to zero with the tangent vector $D n$. Torsion freedom accounts for the bracket term in [F2]. Contract $a=c$. Symmetry of $k$ and $\operatorname{tr}_h k=0$ make the left side $\nabla^ak_{ab}$. In the orthonormal ambient frame $(n,e_1,e_2,e_3)$ the remaining normal term in the Ricci trace is $-g(R(n,e_b)n,n)=0$ by skew-adjointness. Therefore $\nabla^ak_{ab}=-\operatorname{Ric}(n,e_b)$. [F1, F2, step 1.1, step 3.1, algebra]

5.1 Differentiate the first angle identity in step 3.1 once more and trace in the normal frame of step 2.1. Differentiating $k_{ab}Z_b$ gives $(\nabla^ak_{ab})Z_b+k_{ab}g(D_{e_a}U,e_b)+v|k|^2$. Differentiating $-g(n,D_{e_a}U)$ gives a second copy of $k_{ab}g(e_b,D_{e_a}U)$ and $-g(n,\sum_aD_{e_a}D_{e_a}U)$. By the definition of $D^2U$ in the Statement and $D_{e_a}e_a=-k_{aa}n$, the difference between this last trace and $-g(n,\sum_a(D^2U)(e_a,e_a))$ is $(\operatorname{tr}_h k)g(n,D_nU)=0$. The traced scalar Hessian is $\Delta v$ because the induced frame is normal at the point. This proves exactly the stated Laplacian identity; the contracted term is identified in step 4.1. The point was arbitrary, and neither compactness nor division by $v^2-1$ was used. [F1, F2, step 1.1, step 2.1, step 3.1, step 4.1, algebra] ∎

## Source notes

The Radu reference attributes the normal-angle differentiation method to equation (B.8); it supplies no unproved premise for this item. The induced connection, normal frame and every asserted identity are established in the local proof above, for the hypotheses in the Statement.

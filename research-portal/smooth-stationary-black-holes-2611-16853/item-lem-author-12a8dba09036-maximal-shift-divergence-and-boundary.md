---
title: Maximal stationary shift has zero divergence and tangent boundary
status: draft
research_item: lem-author-12a8dba09036-maximal-shift-divergence-and-boundary
dependency_level: 0
---

## Prerequisites

- [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold)
- [math:def-torsion-tensor-of-an-affine-connection](https://alphabetamath.cc/item/def-torsion-tensor-of-an-affine-connection)
- [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)
- [math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor](https://alphabetamath.cc/item/prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor)
- [math:prop-coordinate-formula-for-the-lie-bracket](https://alphabetamath.cc/item/prop-coordinate-formula-for-the-lie-bracket)
- [math:def-levi-civita-connection](https://alphabetamath.cc/item/def-levi-civita-connection)
- [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)
- [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)


## Statement

Let a smooth time-oriented Lorentz metric have a Killing field $T$ and a smooth spacelike section with compact boundary $S$. Write $T=Nn+X$, $h=g|_{TC}$, and $k(U,V)=-g(\nabla_U n,V)$ on its interior $C$. Assume $\operatorname{tr}_h k=0$, that the section and fields extend smoothly across $S$, and $T$ is tangent to $S$. Then $\operatorname{div}_hX=0$ and $X$ is tangent to $S$. If on a stationary asymptotic end the section is $t=0$, $T=\partial_t$, $g_{ij}=\delta_{ij}+O(r^{-1})$ and $g_{0i}=O(r^{-2})$, then $X^i=O(r^{-2})$ in its spatial coordinates.

Here the ambient dimension is any finite $d+1\geq1$: a Lorentz metric is a smooth nondegenerate symmetric covariant two-tensor of signature $(-,+,\ldots,+)$, and time orientation continuously distinguishes the future timelike cone. The section is a smooth embedded hypersurface $\overline C$ with interior $C$ and boundary $S$, with positive-definite induced metric, including on its smooth extension near $S$. The field $n$ is its future unit normal; $N=-g(T,n)$ and $X=T-Nn$. The ambient $\nabla$ denotes the torsion-free metric-compatible affine connection: $\nabla_UV-\nabla_VU=[U,V]$ and $Ug(V,W)=g(\nabla_UV,W)+g(V,\nabla_UW)$. Its existence and uniqueness in these dimensions are established below. A Killing field means a smooth vector field with $\mathcal L_Tg=0$, where $\mathcal L$ is the tensor Lie derivative defined by differentiation of pullbacks along the local flow. These conventions require no global orientation or field equations.

## Facts & Assumptions

[F1] A smooth embedded submanifold with boundary carries its specified smooth structure and smooth embedding. Positive-definite restriction makes $h$ a Riemannian metric. The Lorentz signature, time orientation, spacelike condition, lapse, shift and sign of $k$ are explicitly specified in the Statement; their normal and splitting properties are established locally in step 1.1, without a dimension-specific hypersurface supplier. [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary) [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[F2] An affine connection is function-linear in its direction and obeys the section Leibniz rule; its torsion is $\nabla_UV-\nabla_VU-[U,V]$. Metric compatibility here has the explicit identity given in the Statement. The existence and uniqueness of the ambient connection for this nondegenerate $g$ are proved in step 2.1, rather than imported from a four-dimensional interface. [math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold) [math:def-torsion-tensor-of-an-affine-connection](https://alphabetamath.cc/item/def-torsion-tensor-of-an-affine-connection)

[F3] For a smooth covariant two-tensor the flow-defined Lie derivative has components $(\mathcal L_Tg)_{ab}=T^c\partial_cg_{ab}+g_{cb}\partial_aT^c+g_{ac}\partial_bT^c$. This formula has no metric-signature, dimension-four or orientation hypothesis. The Killing condition in the Statement is its vanishing, not an assumed covariant-derivative characterization. [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field) [math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor](https://alphabetamath.cc/item/prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor)

[F4] The coordinate bracket is $[U,V]^a=U^b\partial_bV^a-V^b\partial_bU^a$. [math:prop-coordinate-formula-for-the-lie-bracket](https://alphabetamath.cc/item/prop-coordinate-formula-for-the-lie-bracket)

[F5] For a Riemannian metric, a torsion-free metric-compatible affine connection is a Levi–Civita connection; for such a connection $D$, the Riemannian divergence is $\operatorname{div}_hX=\operatorname{tr}(U\mapsto D_UX)$. [math:def-levi-civita-connection](https://alphabetamath.cc/item/def-levi-civita-connection) [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)

[F6] This is the usual Riemannian divergence, whose coordinate expression is $\operatorname{div}_hX=(\det h)^{-1/2}\partial_i((\det h)^{1/2}X^i)$. It is valid without a global orientation and with smooth boundary extensions. [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the stated conclusion in every finite ambient dimension.

1.1 The positive-definite tangent space of a spacelike hypersurface is nondegenerate, so the ambient tangent space is its orthogonal direct sum with a one-dimensional complement. The Lorentz signature forces that complement to be timelike. In a submanifold chart, take a smooth nonvanishing conormal $\alpha$ and let $\eta^a=g^{ab}\alpha_b$. The inverse coefficients are smooth by the adjugate formula and nonvanishing determinant. Thus $\eta$ is smooth, orthogonal to the section, and timelike. Normalize by $\sqrt{-g(\eta,\eta)}$ and take its future sign to obtain $n$. Time orientation makes that sign locally constant, so the local normals are smooth and agree on overlaps by uniqueness of the future unit vector in the normal line. This constructs $n$, including on the stipulated spacelike extension near $S$. The formulas $N=-g(T,n)$ and $X=T-Nn$ are smooth and give $g(X,n)=0$, hence $X$ is tangent to the section and $T=Nn+X$. [given, F1, construct, algebra]

2.1 In any ambient chart set $\Gamma^a{}_{bc}=\tfrac12g^{ae}(\partial_bg_{ec}+\partial_cg_{be}-\partial_eg_{bc})$ and define $(\nabla_UV)^a=U^b\partial_bV^a+\Gamma^a{}_{bc}U^bV^c$. Smoothness follows from the inverse formula in step 1.1. Direct product expansion gives the affine-connection rules. Symmetry in $b,c$ and [F4] give torsion freedom; substituting the coefficients gives $\partial_bg_{ac}=g_{ec}\Gamma^e{}_{ba}+g_{ae}\Gamma^e{}_{bc}$, hence metric compatibility for all fields by the product rule. For uniqueness, the difference $A(U,V)$ of two compatible torsion-free connections is function-bilinear by the connection rules. With $B(U,V,W)=g(A(U,V),W)$, torsion freedom makes $B$ symmetric in its first two slots and compatibility makes it skew in its last two. Therefore $B(U,V,W)=B(V,U,W)=-B(V,W,U)=-B(W,V,U)=B(W,U,V)=B(U,W,V)=-B(U,V,W)$; thus $B=0$ and nondegeneracy gives $A=0$. The chart constructions have intrinsic compatibility and torsion properties, so this uniqueness makes them agree on every overlap and glue. This proves existence and uniqueness without positive definiteness or orientation. The connection rules also make $k(U,V)=-g(\nabla_U n,V)$ a smooth tangent two-tensor. [given, F2, F4, step 1.1, construct, algebra]

3.1 Expanding covariant derivatives using step 2.1 gives $g(\nabla_{\partial_a}T,\partial_b)+g(\nabla_{\partial_b}T,\partial_a)=g_{cb}\partial_aT^c+g_{ac}\partial_bT^c+(g_{cb}\Gamma^c{}_{ae}+g_{ac}\Gamma^c{}_{be})T^e$. Torsion freedom and metric compatibility identify the parenthesis with $\partial_eg_{ab}$. By [F3] the result is $(\mathcal L_Tg)_{ab}$, which vanishes for the stated Killing field. Both sides are covariant two-tensors, so $g(\nabla_UT,V)+g(\nabla_VT,U)=0$ for arbitrary local fields. This proves the needed Killing equation locally in every dimension, with no orientation assumption. [given, F2, F3, step 2.1, algebra]

3.2 On $C$ define the tangential projection $P(W)=W+g(W,n)n$ and set $D_UV=P(\nabla_U\widetilde V)|_C$ for tangent fields $U,V$, using any smooth local ambient extension $\widetilde V$ of $V$. Such extensions exist in a submanifold chart by extending component functions off the section. If two extensions differ by a field vanishing on $C$, all its component functions and their derivatives in tangent directions vanish there; the coordinate expression in step 2.1 therefore gives zero for its covariant derivative along $C$. Thus $D_UV$ is independent of the extension. Since $g(PW,n)=0$ and $P$ fixes tangent vectors, $D$ is a smooth tangent connection; direction linearity and the Leibniz rule follow from the ambient connection and projection. For tangent $Z$, orthogonality gives $h(D_UV,Z)=g(\nabla_U\widetilde V,Z)$ along $C$. [given, F1, F2, step 1.1, step 2.1, construct, algebra]

4.1 Ambient metric compatibility gives $U(h(V,Z))=h(D_UV,Z)+h(V,D_UZ)$. By [F4] the bracket of ambient extensions of tangent fields restricts to their intrinsic bracket: in a submanifold chart the normal components vanish on $C$, so their tangent derivatives vanish there, while the remaining components give the intrinsic coordinate bracket. Ambient torsion freedom therefore gives $D_UV-D_VU=P([\widetilde U,\widetilde V])|_C=[U,V]$. Hence $D$ is torsion free and $h$-compatible, and is an intrinsic Levi–Civita connection by [F5]. Its trace is exactly the Riemannian divergence of [F6]. This construction uses the Lorentzian ambient connection directly and does not assume a Riemannian ambient metric. [F1, F2, F4, F5, F6, step 2.1, step 3.2, algebra]

5.1 For tangent $U,V$, orthogonality eliminates the derivative of $N$ in $g(\nabla_U(Nn),V)=-Nk(U,V)$. Substituting $T=Nn+X$ into the Killing equation of step 3.1 and using step 3.2 gives $h(D_UX,V)+h(D_VX,U)=N(k(U,V)+k(V,U))$. In any tangent basis $e_i$, contraction with $h^{ij}$ gives $2h^{ij}h(D_{e_i}X,e_j)=2N\operatorname{tr}_h k$. The left contraction is twice the endomorphism trace of $U\mapsto D_UX$, hence twice $\operatorname{div}_hX$ by step 4.1. Maximality now gives $\operatorname{div}_hX=N\operatorname{tr}_h k=0$. For $d=0$ the contractions are empty sums and give the same conclusion. [given, F1, F2, F5, step 1.1, step 3.1, step 3.2, step 4.1, algebra]

6.1 At $S$, tangency $T\in TS$ implies $N=-g(T,n)=0$, hence $X=T\in TS$. On the stationary end $h_{ij}X^j=g(T,\partial_i)=g_{0i}$. The inverse matrix $h^{ij}$ is bounded for large $r$, because $h_{ij}=\delta_{ij}+O(r^{-1})$: for large $r$ its matrix norm difference from the identity is less than $1/2$, so its least eigenvalue is at least $1/2$. Therefore $X^i=h^{ij}g_{0j}=O(r^{-2})$. All boundary statements use the smooth extensions stipulated in the Statement. Together with step 5.1 this proves every conclusion. [given, F1, step 1.1, step 5.1, algebra] ∎

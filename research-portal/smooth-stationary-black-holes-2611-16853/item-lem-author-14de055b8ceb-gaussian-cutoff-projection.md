---
title: Projection estimates for a Gaussian collar cutoff
status: published
research_item: lem-author-14de055b8ceb-gaussian-cutoff-projection
dependency_level: 2
---

## Prerequisites

- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [lem-author-56ff511785bf-boost-frame-bounds](item-lem-author-56ff511785bf-boost-frame-bounds)
- [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)
- [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry)
- [math:prop-the-gradient-is-characterized-by-inner-products](https://alphabetamath.cc/item/prop-the-gradient-is-characterized-by-inner-products)


## Statement

Let $g=-d\tau^2+h_\tau$ be a smooth time-oriented Lorentzian four-metric in Gaussian coordinates near a compact smooth boundary $S$ of a spacelike reference slice, with $U=\partial_\tau$ future-directed. On a supplied smooth reference-boundary distance collar let $R\ge0$ be the $h_0$-distance to $S$, so $R$ is smooth up to $S$, $R=0$ on $S$ and $|dR|_{h_0}=1$. Extend $R$ constantly along the Gaussian fibres. Fix $0\le\theta<c<1$. Work on a smaller Gaussian tube $\mathcal T$ whose closure is compact and contained in the region where the metric and $R$ are smooth, chosen so that $c|dR|_{h_\tau}\le\gamma<1$. Such a tube exists by smoothness and compactness. All ambient Hessian norms below are bounded on this fixed closure in the positive observer metric $e=g+2U^\flat\otimes U^\flat$, where $U^\flat=g(U,\cdot)$.

Let $\Sigma$ be any smooth spacelike maximal graph in this tube, with future unit normal $n$, satisfying $|\tau|\le\theta R$, and put $v=-g(n,U)$. Write $h=g|_{T\Sigma}$, let $\nabla_\Sigma$ be its gradient and let $\Delta_\Sigma=\operatorname{tr}_h\operatorname{Hess}_h$ be its positive-divergence Laplace–Beltrami operator. For fixed $d>0$ put $\chi=(1+(\tau-cR)/d)_+$, where $s_+=\max\{s,0\}$. On $\{\chi>0\}$ there are constants $a>0$, $b\ge0$ and $C>0$, depending only on the fixed background tube, $c$, $\gamma$ and $d$, not on the graph or $v$, such that $|\nabla_\Sigma\chi|^2\ge av^2-b$ and $|\Delta_\Sigma\chi|\le Cv^2$.

For the cutoff value assertions, choose $r>0$ small enough that the closed cone region $0\le R\le r/2$, $|\tau|\le\theta R$ lies in $\mathcal T$, and consider the graph over this reference collar, smooth up to its boundary. If $d<(c-\theta)r/2$, then $0\le\chi\le1$, $\chi=1$ at $R=0$ and $\chi=0$ at $R=r/2$. Also, within this collar, $R\le d/[2(c+\theta)]$ implies $\chi\ge1/2$. The differential statements concern only the positive set of the possibly nonsmooth cutoff.

## Statement references

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[lem-author-56ff511785bf-boost-frame-bounds](item-lem-author-56ff511785bf-boost-frame-bounds)

[math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)

[math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry)

[math:prop-the-gradient-is-characterized-by-inner-products](https://alphabetamath.cc/item/prop-the-gradient-is-characterized-by-inner-products)

## Facts & Assumptions

[F1] Use the future normal, induced metric and conventions $k(X,Y)=-g(\nabla_X n,Y)$ and $H=-\operatorname{tr}_h k=0$ from [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data). The ambient Levi–Civita connection is metric compatible and torsion-free by [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection), whose domain is mathematics. For smooth ambient $f$ set $\operatorname{Hess}_g f(X,Y)=X(Yf)-df(\nabla_XY)$; the affine-connection product rules make this a smooth bilinear tensor.

[F2] The observer $U$ is future unit timelike. By [lem-author-56ff511785bf-boost-frame-bounds](item-lem-author-56ff511785bf-boost-frame-bounds), $e$ is positive definite, $v\ge1$ and every $h$-unit tangent vector $E$ satisfies $|E|_e\le\sqrt2v$. Smoothness on the fixed compact tube closure gives a finite bound $M$ for the operator norm $|\operatorname{Hess}_g(\tau-cR)|_e$.

[F3] The intrinsic scalar operator is the trace of the Levi–Civita Hessian, including its smooth one-sided boundary extension, in [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian). On the interior, the gradient is the unique smooth field characterized by $h(\nabla_\Sigma\phi,X)=X\phi$ by [math:prop-the-gradient-is-characterized-by-inner-products](https://alphabetamath.cc/item/prop-the-gradient-is-characterized-by-inner-products). Its boundary applicability is checked in step 1.1.

[F4] The induced Riemannian metric has a unique metric-compatible torsion-free connection, also up to a smooth boundary, by [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry). The identification with ambient tangential projection and the Hessian restriction formula are derived below.

## Proof

**Given:** The smooth compact Gaussian collar, future observer, maximal graph and constants in the Statement. **Goal:** Prove all cutoff value and differential estimates.

1.1 Put $f=\tau-cR$. The gradient characterization in [F3] also holds up to the smooth graph boundary: for any smooth $\phi$ on the graph, in a boundary chart put $Y^i=\sum_jh^{ij}\partial_j\phi$, where $(h^{ij})=(h_{ij})^{-1}$. The inverse matrix is smooth up to the boundary by the adjugate formula and positive definiteness. Thus $Y$ is smooth and $h(Y,X)=X\phi$ for all tangent $X$ there. If two fields satisfy this identity, their difference $Z$ satisfies $h(Z,Z)=0$, so they agree; this also makes the chart formulas agree on overlaps. At the reference slice $c|dR|_{h_0}=c<1$; continuity on a compact reference collar permits a common smaller tube and a fixed $c<\gamma<1$ with $c|dR|_{h_\tau}\le\gamma$. Since $R$ is constant on Gaussian fibres, $g^{-1}(df,df)=-1+c^2|dR|_{h_\tau}^2\ge-1$. Write $n=vU+z$, with $z\perp U$ and $|z|_{h_\tau}^2=v^2-1$. As $c\ge0$ and $v\ge1$, $df(n)=v-c\,dR(z)\ge v-\gamma\sqrt{v^2-1}\ge(1-\gamma)v$. Let $A$ be the vector defined by $g(A,\cdot)=df$. Its tangent projection is $A+df(n)n$, which pairs with every tangent $X$ as $Xf$ and is therefore $\nabla_\Sigma(f|_\Sigma)$. Its squared norm is $g^{-1}(df,df)+df(n)^2\ge(1-\gamma)^2v^2-1$. On $\chi>0$ division by $d^2$ proves the gradient bound with $a=(1-\gamma)^2/d^2$ and $b=1/d^2$. [F1, F2, F3, given, algebra]

2.1 For tangent fields $X,Y$ set $D_XY=(\nabla_XY)^\top$. Tangential projection preserves the connection rules and metric compatibility; torsion freedom follows from $D_XY-D_YX=(\nabla_XY-\nabla_YX)^\top=[X,Y]$, because the bracket is tangent. Thus [F4] identifies $D$ with the intrinsic Levi–Civita connection. Differentiating $g(Y,n)=0$ gives $g(\nabla_XY,n)=-g(Y,\nabla_X n)=k(X,Y)$, hence $\nabla_XY=D_XY-k(X,Y)n$. For $\phi=f|_\Sigma$, differentiating $h(\nabla_\Sigma\phi,Y)=Y\phi$ and using metric compatibility yields $\operatorname{Hess}_h\phi(X,Y)=X(Y\phi)-(D_XY)\phi$. Substitution into [F1] now gives $\operatorname{Hess}_h\phi(X,Y)=\operatorname{Hess}_g f(X,Y)-k(X,Y)df(n)$. Tracing over a tangent orthonormal basis $(E_i)_{i=1}^3$ and using $H=-\operatorname{tr}_h k$ yields $\Delta_\Sigma\phi=\sum_i\operatorname{Hess}_g f(E_i,E_i)+Hdf(n)=\sum_i\operatorname{Hess}_g f(E_i,E_i)$. [F1, F3, F4, step 1.1, given, algebra]

3.1 The bound in [F2] and the trace identity imply $|\Delta_\Sigma(f|_\Sigma)|\le M\sum_{i=1}^3|E_i|_e^2\le6Mv^2$. On $\chi>0$ the cutoff is $1+f/d$, so $|\Delta_\Sigma\chi|\le(6M/d)v^2$; taking $C=1+6M/d$ gives a positive constant. This uses only fixed smooth background second derivatives, not graph second-derivative bounds. At the graph boundary the formulas have their smooth one-sided interpretation wherever $\chi>0$. [F2, F3, step 2.1, algebra]

4.1 On the stated graph collar, $-(c+\theta)R\le f\le-(c-\theta)R\le0$, so $0\le\chi\le1$. At $R=0$ the cone gives $\tau=0$ and hence $\chi=1$. At $R=r/2$ the strict inequality $d<(c-\theta)r/2$ gives $f<-d$ and $\chi=0$. Since $c+\theta>0$, if $R\le d/[2(c+\theta)]$ then $f\ge-d/2$ and $\chi\ge1/2$. No derivative estimate is asserted across $\chi=0$. Together with the preceding differential estimates these prove every conclusion. [step 1.1, step 3.1, given, algebra] ∎

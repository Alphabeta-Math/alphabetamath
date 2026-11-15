---
title: Gradient Hölder control by differentiated flux and one-dimensional lifting
status: published
research_item: lem-author-db87cb8e0bab-divergence-gradient-holder
dependency_level: 0
sources:
  references:
    - title: Xavier Fernández-Real and Xavier Ros-Oton, Regularity Theory for Elliptic
        PDE
      url: https://www.ub.edu/pde/xros/Llibre-ellipticPDE.pdf
      locator: Theorem 3.17, printed p. 93, PDF p. 99
      statement: For a weak solution $z\in H^1(B_1)$ of $\operatorname{div}(A Dz)=0$,
        with measurable symmetric matrix $\lambda I\le A\le\Lambda I$, there are
        $\beta>0$ and $C$ depending only on dimension and ellipticity such that
        $\|z\|_{C^{0,\beta}(B_{1/2})}\le C\|z\|_{L^2(B_1)}$.
      hypotheses: Scalar real-valued weak solution on a Euclidean ball; bounded
        measurable uniformly elliptic coefficients; the symmetric case suffices
        here. Used in dimension $n+1$ for an $n$-dimensional coordinate ball
        after a local lifting, not directly on the nonlinear graph equation.
      reading_limits: Checked the extracted statement, hypotheses and immediate proof
        note of Theorem 3.17 on printed p. 93 (PDF p. 99) in the author-hosted
        PDF. The underlying De Giorgi–Nash argument was not read or
        reconstructed. The local lifting, weak-solution verification and graph
        application are authored here.
---

## Prerequisites

- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-hk-and-hk-zero-notation](https://alphabetamath.cc/item/def-hk-and-hk-zero-notation)
- [math:def-local-weak-solution-for-a-divergence-form-operator](https://alphabetamath.cc/item/def-local-weak-solution-for-a-divergence-form-operator)
- [` Xavier Fernández-Real and Xavier Ros-Oton, Regularity Theory for Elliptic PDE · Theorem 3.17, printed p. 93, PDF p. 99 `](https://www.ub.edu/pde/xros/Llibre-ellipticPDE.pdf)


## Statement

Let $P(y,p)$ be a smooth flux on a coordinate ball times $|p|\le p_0$; assume $P_p$ symmetric with $\lambda I\le P_p\le\Lambda I$ and $|P_y|\le K$. Let $w$ be a smooth scalar solution of $\operatorname{div}P(y,Dw)=0$ with $|Dw|\le p_0$. On each strictly smaller ball there exist $0<\beta<1$ and $C$, depending only on dimension, ellipticity, $K,p_0$ and the interior separation, such that $\|Dw\|_{C^{0,\beta}}\le C$. No uniform second-derivative bound is assumed.

## Facts & Assumptions

[F1] Hölder norms and classical derivatives are as in the Euclidean interface. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F2] On an open Euclidean set, $H^1=W^{1,2}$ consists of almost-everywhere classes of square-integrable functions with square-integrable first weak derivatives; use the real scalar case here. [math:def-hk-and-hk-zero-notation](https://alphabetamath.cc/item/def-hk-and-hk-zero-notation)

[F3] For a bounded measurable uniformly elliptic real matrix $B$ on an open set $U$, the homogeneous local weak equation $\operatorname{div}(B Du)=0$ means $u\in H^1(U)$ and $\int_U (B Du)\cdot D\varphi=0$ for every $\varphi\in C_c^\infty(U)$; this is the supplier convention with operator $-\operatorname{div}(B D)$, zero lower-order coefficients and zero datum, without a boundary condition. [math:def-local-weak-solution-for-a-divergence-form-operator](https://alphabetamath.cc/item/def-local-weak-solution-for-a-divergence-form-operator)

[A1] Work in ZFC, including choice for the imported analytic input and the Countable Choice assumptions of the Sobolev and weak-solution interfaces. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F20] Use the scalar homogeneous divergence-form De Giorgi–Nash estimate from Theorem 3.17 as recorded in External input, in one additional Euclidean dimension.

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the asserted estimate with the stated uniform dependence.

1.1 For each $k$, put $z=D_kw$, $a(y)=P_p(y,Dw(y))$ and $F(y)=-P_{y_k}(y,Dw(y))$, with $P_{y_k}$ the partial derivative at fixed $p$. Differentiating the flux equation gives $\operatorname{div}(a Dz)=\operatorname{div}F$. The matrix $a$ is measurable, symmetric and uniformly elliptic, $|z|\le p_0$ and $|F|\le K$. Smoothness justifies the differentiation without any uniform Hessian estimate. [given, F1, algebra]

2.1 Write $n$ for the coordinate dimension. Here is a local reduction of this inhomogeneous equation to the exact homogeneous source statement. If $M=\|z\|_\infty+\|F\|_\infty$ is zero there is nothing to prove. Otherwise put $Z(y,t)=z(y)/M+t$ and $H=F/M$. On a cylinder strictly inside the coordinate ball times $(-1,1)$ use the symmetric matrix $B=\begin{pmatrix}a&-H\\-H^T&L\end{pmatrix}$, where $L=1+2/\lambda$. Its quadratic form is at least $(\lambda/2)|\xi|^2+|\tau|^2$, since $|H|\le1$ and $2|\tau H\cdot\xi|\le(\lambda/2)|\xi|^2+(2/\lambda)\tau^2$. It has a uniform upper bound too. Direct distributional differentiation, using independence of $t$, gives $\operatorname{div}_{y,t}(B DZ)=\operatorname{div}_y(a Dz/M-H)=0$. [step 1.1, given, algebra]

3.1 Let $U$ be any $(n+1)$-dimensional ball with closure in this cylinder. The smooth function $Z$ and all its first classical derivatives are bounded on $\overline U$, so they are square-integrable on $U$; integration by parts against compactly supported tests identifies these classical derivatives as its weak derivatives. Thus $Z\in H^1(U)$, without requiring a uniform bound on its $H^1$ norm. For each $\varphi\in C_c^\infty(U)$, integration by parts in the divergence identity of step 2.1 gives $\int_U (B DZ)\cdot D\varphi=0$. Hence $Z$ is a scalar homogeneous weak solution with exactly the convention and coefficient hypotheses needed in F20. [step 2.1, F2, F3, F20, A1, algebra]

4.1 Apply the imported homogeneous theorem in dimension $n+1$ on the balls of step 3.1, after translation and dilation to the unit ball. Since $|Z|$ has a universal bound on the fixed cylinder, its $L^2$ norm is uniformly bounded on each such ball. Restrict the resulting Hölder estimate to $t=0$ and multiply by $M$. A finite cover of every smaller coordinate ball yields $\|z\|_{C^{0,\beta}}\le C(\|z\|_\infty+\|F\|_\infty)$. Doing this for the finitely many $k$ proves the assertion. The exponent may be decreased below one; no value of the prescribed later Schauder exponent is assumed here. [F20, A1, step 3.1, F1] ∎

## External input

[F20] Imported established input: For a weak solution $z\in H^1(B_1)$ of $\operatorname{div}(A Dz)=0$, with measurable symmetric matrix $\lambda I\le A\le\Lambda I$, there are $\beta>0$ and $C$ depending only on dimension and ellipticity such that $\|z\|_{C^{0,\beta}(B_{1/2})}\le C\|z\|_{L^2(B_1)}$. Scalar real-valued weak solution on a Euclidean ball; bounded measurable uniformly elliptic coefficients; the symmetric case suffices here. Used in dimension $n+1$ for an $n$-dimensional coordinate ball after a local lifting, not directly on the nonlinear graph equation. Reading limits: Checked the extracted statement, hypotheses and immediate proof note of Theorem 3.17 on printed p. 93 (PDF p. 99) in the author-hosted PDF. The underlying De Giorgi–Nash argument was not read or reconstructed. The local lifting, weak-solution verification and graph application are authored here.

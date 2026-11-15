---
title: Uniform coefficient regularity before the final graph estimate
status: published
research_item: lem-author-db87cb8e0bab-coefficient-regularity
dependency_level: 1
sources:
  references:
    - title: Xavier Fernández-Real and Xavier Ros-Oton, Regularity Theory for Elliptic
        PDE
      url: https://www.ub.edu/pde/xros/Llibre-ellipticPDE.pdf
      locator: Theorem 2.20 and Corollary 2.21, printed pp. 46–47, PDF pp. 52–53
      statement: For $k\ge1$, $0<\gamma<1$, and $z\in C^{k+2,\gamma}(B_1)$ solving
        $a^{ij}D_{ij}z=f$, if $\lambda I\le a\le\Lambda I$ and $a,f\in
        C^{k,\gamma}(B_1)$, then $\|z\|_{C^{k+2,\gamma}(B_{1/2})}\le
        C(\|z\|_\infty+\|f\|_{C^{k,\gamma}(B_1)})$, with
        $C=C(n,k,\gamma,\lambda,\Lambda,\|a\|_{C^{k,\gamma}})$.
      hypotheses: The higher-order estimate is an a priori estimate and requires the
        displayed regularity of $z$ before use. Applied here only for $n\ge2$
        and $k=1,2$ on rescaled compactly contained balls; smoothness gives this
        membership, and the preceding stage supplies uniform coefficient and
        forcing norms. The $k=0$ first stage uses the declared library theorem
        instead. Dimension one is handled locally.
      reading_limits: Read the complete extracted statements and hypotheses of Theorem
        2.20 and Corollary 2.21 on printed pp. 46–47 (PDF pp. 52–53) in the
        author-hosted PDF during this assignment. Their proofs were not read or
        reconstructed; only the stated a priori estimates are imported.
---

## Prerequisites

- [lem-author-db87cb8e0bab-divergence-gradient-holder](item-lem-author-db87cb8e0bab-divergence-gradient-holder)
- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle)
- [math:lem-uniform-integral-error-bound](https://alphabetamath.cc/item/lem-uniform-integral-error-bound)
- [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [` Xavier Fernández-Real and Xavier Ros-Oton, Regularity Theory for Elliptic PDE · Theorem 2.20 and Corollary 2.21, printed pp. 46–47, PDF pp. 52–53 `](https://www.ub.edu/pde/xros/Llibre-ellipticPDE.pdf)


## Statement

Work in ZFC, with integer coordinate dimension $n\ge1$. Let $0<\alpha<1$ and let $P$ and $w$ satisfy the preceding gradient lemma on a fixed annulus, with common joint $C^{4,\alpha}$ bounds for $P$, $|Dw|\le p_0$ and $\|w\|_\infty\le M_0$. Then on any fixed smaller annulus, $A(y)=P_p(y,Dw)$ and $b^j(y)=\int_0^1s_{p_j}(y,tDw)\,dt$, where $s(y,p)=\sum_iP^i_{y_i}(y,p)$, have common $C^{2,\alpha}$ bounds. The constants depend on the structural bounds and $M_0$, not on any initially unknown derivative norm of $w$.

## Facts & Assumptions

[F1] The differentiated-flux estimate supplies a uniform $C^{0,\beta}$ bound for $Dw$ for some $0<\beta<1$, on compactly contained coordinate balls under the smooth flux, uniform ellipticity and slope hypotheses inherited in the Statement. [lem-author-db87cb8e0bab-divergence-gradient-holder](item-lem-author-db87cb8e0bab-divergence-gradient-holder)

[F2] Use the ordinary Euclidean $C^{k,\gamma}$ norms and scaled ball norms. Product and composition estimates needed below are proved in step 1.1 from these seminorm definitions. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F3] Under Countable Choice and in dimension $n\ge2$, the library interior Schauder estimate applies to a bounded $C^2$ solution with uniformly elliptic $C^{0,\gamma}$ principal coefficients, $C^{0,\gamma}$ forcing and finite coefficient seminorms; its constant depends only on the stated quantitative bounds. We take both lower-order coefficients to be zero. [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations)

[F4] For totally differentiable maps between open Euclidean sets, $D(G\circ\Phi)=DG(\Phi)D\Phi$. Apply this successively to the smooth maps used here. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F5] A continuous real integrand on a compact rectangle whose parameter derivative is continuous there may be differentiated through its Riemann integral. Apply this componentwise, with other coordinates fixed, and then to first parameter derivatives. [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle)

[F6] For integrable real functions on $[0,1]$, a uniform difference bound $\eta$ implies that their integrals differ by at most $\eta$. This also bounds an integral by taking one integrand to be zero. [math:lem-uniform-integral-error-bound](https://alphabetamath.cc/item/lem-uniform-integral-error-bound)

[F7] The real mean value theorem applies to each smooth component along a closed line segment contained in its coordinate domain; a derivative bound therefore bounds its increment by the segment length times that bound. [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

[A1] Work in ZFC, including the Axiom of Choice used by the gradient supplier. In particular Countable Choice holds: for any sequence of nonempty sets, choose on its family of values and compose that choice function with the sequence. This supplies the first Schauder theorem's choice hypothesis. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F20] The imported Corollary 2.21 supplies the higher-order a priori estimate recorded in External input, for already smooth solutions with controlled $C^{k,\gamma}$ coefficients and forcing.

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the asserted estimate with the stated uniform dependence.

1.1 On bounded convex coordinate balls, subtracting products gives $[fg]_{0,\gamma}\le\|f\|_\infty[g]_{0,\gamma}+\|g\|_\infty[f]_{0,\gamma}$; iterating gives the finite-product version. The increment identity $\Delta(fg)=f\Delta g+g\Delta f+\Delta f\Delta g$ also proves the ordinary product differentiation rule by division and passage to the limit. By F7 along segments, bounded first derivatives make a smooth outer map $G$ Lipschitz. Thus $[G\circ\Psi]_{0,\gamma}\le\operatorname{Lip}(G)[\Psi]_{0,\gamma}$; if instead $G$ is $\gamma$-Hölder and $\Psi$ Lipschitz, then $[G\circ\Psi]_{0,\gamma}\le[G]_{0,\gamma}\operatorname{Lip}(\Psi)^\gamma$. These componentwise inequalities and F4 give all product and composition estimates below on ball times slope-ball domains. [F2, F4, F7, algebra]

2.1 First suppose $n\ge2$. Reduce the exponent in F1 so that $0<\beta\le\alpha$; on a fixed bounded set this costs only a fixed diameter factor in the seminorm. On smaller balls F1 and step 1.1 give uniform $C^{0,\beta}$ bounds for $A(y)=P_p(y,Dw)$ and $s(y,Dw)$, where $s(y,p)=\sum_iP^i_{y_i}(y,p)$ uses derivatives at fixed $p$. The chain rule expands the given flux equation as $A^{ij}w_{ij}=-s(y,Dw)$. The inherited symmetric ellipticity bounds hold for $A$; the lower-order coefficients are zero; $w$ is smooth and bounded by $M_0$; and A1 supplies Countable Choice. All hypotheses of F3 are now satisfied, with $\gamma=\beta$. Its scaled estimate on fixed balls gives a uniform $C^{2,\beta}$ bound on smaller balls, without using any prior uniform higher derivative bound. [given, F1, F2, F3, F4, A1, step 1.1]

2.2 If $n=1$, work instead on compactly contained intervals in the annulus. The chain rule gives $w^{\prime\prime}=Q(y,w^\prime)$, where $Q(y,p)=-P_y(y,p)/P_p(y,p)$ and $P_p\ge\lambda>0$. The joint derivatives of $Q$ through order two have common bounds using only joint derivatives of $P$ through order three and powers of $\lambda^{-1}$: this follows by the product and chain rules and the directly differentiated identity $a(1/a)=1$. Hence $w^{\prime\prime}$ is bounded, then $w^{\prime\prime\prime}=Q_y+Q_p w^{\prime\prime}$ is bounded, and finally $w^{(4)}=Q_{yy}+2Q_{yp}w^{\prime\prime}+Q_{pp}(w^{\prime\prime})^2+Q_p w^{\prime\prime\prime}$ is bounded, with each $Q$ derivative evaluated at $(y,w^\prime(y))$. Together with the given height and slope bounds, this supplies all derivative suprema through order four. This is all that the remaining argument needs; no use of the dimension-restricted Schauder theorem is made in this case. [given, F4, step 1.1, algebra]

3.1 Still for $n\ge2$, the chain and product rules with the $C^{2,\beta}$ bound give uniform $C^{1,\beta}$ bounds for $A$ and $s(y,Dw)$ on a smaller ball. Apply F20 with $k=1$ and $\gamma=\beta$ after rescaling that ball to obtain uniform $C^{3,\beta}$ bounds for $w$ on its half ball. The same chain and product rules now bound $A$ and $s(y,Dw)$ in $C^{2,\beta}$; F20 with $k=2$ gives a uniform $C^{4,\beta}$ bound on a further smaller ball. Smoothness on neighborhoods of the compact closures supplies the finite $C^{k+2,\beta}$ membership required by each a priori application before it is used; its unknown preliminary norm never enters the right side. All radii and their ratios are fixed, and these preliminary bounds may depend on $M_0$ without being linear in it. [step 2.1, step 1.1, F2, F4, F20, given]

4.1 In either dimension case the suprema of derivatives of $w$ through order four are now uniformly bounded. F7 and F4 along segments show that $Dw,D^2w,D^3w$ are uniformly Lipschitz on smaller balls. Put $\Phi_t(y)=(y,tDw(y))$ for $0\le t\le1$, $G(y,p)=P_p(y,p)$ and $H_j(y,p)=s_{p_j}(y,p)$. The maps $\Phi_t,D\Phi_t,D^2\Phi_t$ are uniformly bounded and Lipschitz, uniformly in $t$. For either $J=G$ or $J=H_j$, twice applying F4 gives $D^2(J\circ\Phi_t)=D^2J(\Phi_t)[D\Phi_t,D\Phi_t]+DJ(\Phi_t)D^2\Phi_t$. The joint derivatives of $G$ through order two use derivatives of $P$ through order three, and those of $H_j$ through order two use derivatives of $P$ through order four. Their common $\alpha$-Hölder bounds follow from the given joint $C^{4,\alpha}$ bound (lower derivatives use F7 locally). Thus step 1.1 bounds $G\circ\Phi_1=A$ in $C^{2,\alpha}$ and bounds $h_j(y,t):=H_j(\Phi_t(y))$ and its first two $y$ derivatives in the same norms uniformly in $t$. No fifth derivative of $P$ is used. [step 3.1, step 2.2, step 1.1, F2, F4, F7, given]

5.1 On every closed coordinate box inside a controlled ball, $h_j$ and its first two spatial derivatives are continuous jointly with $t\in[0,1]$; smoothness on a neighborhood of the slope ball ensures this also when $tDw$ is on its boundary. Apply F5 along each coordinate interval, and again to each first derivative, to obtain $D_y^\nu b^j(y)=\int_0^1D_y^\nu h_j(y,t)\,dt$ for $|\nu|\le2$. F6 applied with one integrand zero bounds these derivative suprema. Applied to the second derivatives at two spatial points, it bounds their $\alpha$-Hölder differences by the common bounds of step 4.1. Finally choose a fixed finite interior cover of the desired smaller annulus by controlled balls whose concentric half balls still cover it. For pairs closer than half the least covering radius, the ball for the first point contains both points; separated pairs use the derivative sup bounds divided by that fixed separation to the power $\alpha$. The resulting $C^{2,\alpha}$ bounds for $A$ and $b$ depend only on the structural data, $M_0$ and the fixed annuli, without dependence on initially unknown derivative norms of $w$. [step 4.1, F2, F5, F6, given] ∎

## External input

[F20] Imported established input (Corollary 2.21): For $k\ge1$, $0<\gamma<1$, and $z\in C^{k+2,\gamma}(B_1)$ solving $a^{ij}D_{ij}z=f$, if $\lambda I\le a\le\Lambda I$ and $a,f\in C^{k,\gamma}(B_1)$, then $\|z\|_{C^{k+2,\gamma}(B_{1/2})}\le C(\|z\|_\infty+\|f\|_{C^{k,\gamma}(B_1)})$, with $C=C(n,k,\gamma,\lambda,\Lambda,\|a\|_{C^{k,\gamma}})$. The higher-order estimate is an a priori estimate and requires the displayed regularity of $z$ before use. Applied here only for $n\ge2$ and $k=1,2$ on rescaled compactly contained balls; smoothness gives this membership, and the preceding stage supplies uniform coefficient and forcing norms. The $k=0$ first stage uses the declared library theorem instead. Dimension one is handled locally. Reading limits: Read the complete extracted statements and hypotheses of Theorem 2.20 and Corollary 2.21 on printed pp. 46–47 (PDF pp. 52–53) in the author-hosted PDF during this assignment. Their proofs were not read or reconstructed; only the stated a priori estimates are imported.

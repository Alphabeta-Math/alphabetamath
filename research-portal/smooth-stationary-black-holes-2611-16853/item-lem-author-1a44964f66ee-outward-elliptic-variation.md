---
title: Outward graph stability has the negative-Laplacian principal symbol
status: draft
research_item: lem-author-1a44964f66ee-outward-elliptic-variation
dependency_level: 6
---

## Prerequisites

- [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)
- [lem-author-c50357f4fa9e-expansion-second-jet](item-lem-author-c50357f4fa9e-expansion-second-jet)
- [lem-author-c50357f4fa9e-linear-expansion-variation](item-lem-author-c50357f4fa9e-linear-expansion-variation)
- [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)
- [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)
- [math:def-elliptic-hyperbolic-and-parabolic-principal-symbols](https://alphabetamath.cc/item/def-elliptic-hyperbolic-and-parabolic-principal-symbols)


## Statement

Use the smooth Lorentzian and outward normal-graph data of the surface supplier on a closed surface $S$. Let $q$ be its induced metric, $n$ the future hypersurface unit normal and $\nu$ the supplied outward unit normal within the spacelike hypersurface. For $\Theta(u)=F_u^*\theta_{n+\nu_u}$ define $\mathcal L\psi=\left.\partial_\epsilon\right|_0\Theta(\epsilon\psi)$. Then $\mathcal L=-\Delta_q+b\cdot\nabla+c$ for a smooth real tangent vector field $b$ and smooth real scalar $c$. Equivalently, with $t=b/2$, $\mathcal L=-\Delta_q+2t\cdot\nabla+c$ is a real smooth elliptic operator. The normalization $l=n+\nu$, $k=n-\nu=2\underline L$ gives $g(l,k)=-2$, $g(l,\nu)=1$, $\nu=-k/2+l/2$ and $s_A=-g(k,\nabla_Al)/2=\zeta_A$. These identities use the outward sign fixed by the supplier.

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The surface supplier fixes the expansion, intrinsic derivatives, outward graph tube and null normalization. [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data) [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)

[F2] The second-graph-data supplier states the exact expansion formula, its first-data remainder and its zero-graph second-partial coefficient; the linearization supplier gives the smooth linear, path-independent derivative. [lem-author-c50357f4fa9e-expansion-second-jet](item-lem-author-c50357f4fa9e-expansion-second-jet) [lem-author-c50357f4fa9e-linear-expansion-variation](item-lem-author-c50357f4fa9e-linear-expansion-variation)

[F3] The differential chain rule applies to the smooth coordinate changes and finite-dimensional coefficient functions used below. [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[F4] For a real scalar second-order principal symbol $p_2(x,\xi)=a^{ab}(x)\xi_a\xi_b$ with symmetric coefficients, ellipticity at $x$ means $p_2(x,\xi)\ne0$ for every nonzero covector $\xi$. [math:def-elliptic-hyperbolic-and-parabolic-principal-symbols](https://alphabetamath.cc/item/def-elliptic-hyperbolic-and-parabolic-principal-symbols)

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The surface supplier fixes the expansion, intrinsic derivatives, outward graph tube and null normalization. [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data) [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)

[F2] The second-graph-data supplier states the exact expansion formula, its first-data remainder and its zero-graph second-partial coefficient; the linearization supplier gives the smooth linear, path-independent derivative. [lem-author-c50357f4fa9e-expansion-second-jet](item-lem-author-c50357f4fa9e-expansion-second-jet) [lem-author-c50357f4fa9e-linear-expansion-variation](item-lem-author-c50357f4fa9e-linear-expansion-variation)

[F3] The differential chain rule applies to the smooth coordinate changes and finite-dimensional coefficient functions used below. [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[F4] For a real scalar second-order principal symbol $p_2(x,\xi)=a^{ab}(x)\xi_a\xi_b$ with symmetric coefficients, ellipticity at $x$ means $p_2(x,\xi)\ne0$ for every nonzero covector $\xi$. [math:def-elliptic-hyperbolic-and-parabolic-principal-symbols](https://alphabetamath.cc/item/def-elliptic-hyperbolic-and-parabolic-principal-symbols)



**Proof technique:** direct.

1.1 By the exact decomposition in [F2], $\Theta(u)=-q_u^{ab}h(\nu_u,T_r)\partial_a\partial_bu+R(x,u,\partial u)$, with all coefficients and $R$ smooth and real. At the zero graph the same supplier gives $h(\nu_0,T_r)=1$ and $q_0=q$. Along $u=\epsilon\psi$, the derivative of the coefficient multiplying $\partial_a\partial_bu$ contributes zero at $\epsilon=0$, since the zero graph has zero second partials. The second-order part of $\mathcal L$ is consequently $-q^{ab}\partial_a\partial_b$, and the remaining terms are smooth real first- and zeroth-order terms by the supplied linearization. The intrinsic Laplacian from [F1] has second-order part $q^{ab}\partial_a\partial_b$, so $P=\mathcal L+\Delta_q$ has order at most one. Set $c=P(1)$. In coordinates $P-c$ has the form $b^a\partial_a$ with smooth real coefficients; coordinate independence of $P-c$ and the chain rule give the vector-field transformation law for these coefficients. They therefore define a global smooth real vector field $b$, and $\mathcal L=-\Delta_q+b\cdot\nabla+c=-\Delta_q+2t\cdot\nabla+c$ for $t=b/2$. In the quadratic-symbol convention of [F4], the principal symbol is $p_2(x,\xi)=-q^{ab}(x)\xi_a\xi_b$. For every nonzero covector $\xi$, positive definiteness of $q$ gives $q^{ab}\xi_a\xi_b>0$, so $p_2(x,\xi)<0$. Thus the principal symbol is nonzero on every nonzero covector at every point, and [F4] gives the asserted ellipticity. [F1, F2, F3, F4]

2.1 The null pairings follow from $g(n,n)=-1$, $g(\nu,\nu)=1$ and $g(n,\nu)=0$: $g(n+\nu,n-\nu)=-2$ and $g(n+\nu,\nu)=1$. Direct substitution yields $\nu=-k/2+l/2$. The supplier defines $\zeta_A=-g(\underline L,\nabla_Al)$; because $k=2\underline L$, the source convention $s_A=-g(k,\nabla_Al)/2$ is exactly $\zeta_A$. For each smooth test function the compact-surface tube supplies a common parameter interval for the graph path, and its velocity is $\psi\nu$. Thus $\delta_{\psi\nu}\theta_l=\mathcal L\psi$ in this same fixed outward direction. This proves all assertions, independently of any specialization of the zeroth-order curvature coefficient. [F1, F2, step 1.1] ∎

---
title: Ground-state identity, spectral ordering and eigenspace uniqueness
status: published
research_item: lem-author-1a44964f66ee-ground-state-identity
dependency_level: 2
---

## Prerequisites

- [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)
- [lem-author-1a44964f66ee-positive-adjoint-pairing](item-lem-author-1a44964f66ee-positive-adjoint-pairing)
- [math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component](https://alphabetamath.cc/item/prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component)
- [math:def-eigenvalue-eigenvector-eigenspace-and-spectrum](https://alphabetamath.cc/item/def-eigenvalue-eigenvector-eigenspace-and-spectrum)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

For $L$ on $(S,h)$ as in the formal-adjoint lemma, suppose $L\phi=\lambda\phi$ and $L^\dagger\chi=\lambda\chi$ with $\lambda\in\mathbb C$ and smooth positive real $\phi,\chi$. Define $P w=\phi^{-1}(L-\lambda)(\phi w)$ and $m=\phi\chi$. Then $P=-\Delta_h+2(t-\nabla\log\phi)\cdot\nabla$, $\int_Sm Pw\,d\mu_h=0$, and $P|w|^2=2\operatorname{Re}(\overline w Pw)-2|\nabla w|^2$ for complex smooth $w$. If $S$ is nonempty, then $\lambda$ is necessarily real and every smooth eigenpair $L\psi=\mu\psi$, $\psi\not\equiv0$, satisfies $\operatorname{Re}\mu\ge\lambda$. On such nonempty $S$, the eigenspace at $\lambda$ is exactly the complex span of $\phi$; in particular the positive real eigenfunction is unique up to a positive constant. If $S=\varnothing$, the displayed differential and integral identities hold trivially, the eigenspace at $\lambda$ and the complex span of $\phi$ both equal $\{0\}$, and there is no nonzero eigenfunction; $\lambda$ need not be real.

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The formal-adjoint lemma fixes the real-coefficient operator, positive density integral and adjoint identity. On nonempty $S$ with real eigenvalues, the positive-adjoint-pairing lemma identifies the eigenvalues of a positive right eigenfunction and a positive adjoint eigenfunction, and supplies smooth bounded reciprocals of both. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint) [lem-author-1a44964f66ee-positive-adjoint-pairing](item-lem-author-1a44964f66ee-positive-adjoint-pairing)

[F2] A smooth real-valued function with zero differential is constant on each connected component of its smooth manifold. [math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component](https://alphabetamath.cc/item/prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component)

[F3] For the complex vector space $V=C^\infty(S;\mathbb C)$ and the complex-linear endomorphism $L:V\to V$, the eigenspace at any scalar $\lambda$ is $E_\lambda(L)=\ker(L-\lambda I_V)=\{u\in V:Lu=\lambda u\}$. This definition also applies to the zero vector space. [math:def-eigenvalue-eigenvector-eigenspace-and-spectrum](https://alphabetamath.cc/item/def-eigenvalue-eigenvector-eigenspace-and-spectrum)

[F4] Work in ZFC, including the Axiom of Choice. Choice supplies the countable-choice hypotheses for density integration and the chart-subordinate partitions of unity used by the formal-adjoint lemma. Its adjoint integral identity and strict positivity of the density integral are invoked here under those same assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The formal-adjoint lemma fixes the real-coefficient operator, positive density integral and adjoint identity. On nonempty $S$ with real eigenvalues, the positive-adjoint-pairing lemma identifies the eigenvalues of a positive right eigenfunction and a positive adjoint eigenfunction, and supplies smooth bounded reciprocals of both. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint) [lem-author-1a44964f66ee-positive-adjoint-pairing](item-lem-author-1a44964f66ee-positive-adjoint-pairing)

[F2] A smooth real-valued function with zero differential is constant on each connected component of its smooth manifold. [math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component](https://alphabetamath.cc/item/prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component)

[F3] For the complex vector space $V=C^\infty(S;\mathbb C)$ and the complex-linear endomorphism $L:V\to V$, the eigenspace at any scalar $\lambda$ is $E_\lambda(L)=\ker(L-\lambda I_V)=\{u\in V:Lu=\lambda u\}$. This definition also applies to the zero vector space. [math:def-eigenvalue-eigenvector-eigenspace-and-spectrum](https://alphabetamath.cc/item/def-eigenvalue-eigenvector-eigenspace-and-spectrum)

[F4] Work in ZFC, including the Axiom of Choice. Choice supplies the countable-choice hypotheses for density integration and the chart-subordinate partitions of unity used by the formal-adjoint lemma. Its adjoint integral identity and strict positivity of the density integral are invoked here under those same assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)



**Proof technique:** direct.

1.1 If $S=\varnothing$, then $C^\infty(S;\mathbb C)=\{0\}$: every smooth function is the unique empty function. The differential operators, products and integrals in the Statement are zero, so the identities and eigenspace description hold, with no nonzero eigenfunction and no restriction on $\lambda$. This settles the empty case. Henceforth assume $S$ is nonempty. Since $L$ has real coefficients and $\phi$ is real, $L\phi$ is real valued. At any $p\in S$, the eigenvalue equation and $\phi(p)>0$ give $\lambda=(L\phi)(p)/\phi(p)\in\mathbb R$. Both eigenvalue parameters in the positive-adjoint-pairing lemma are therefore this same real $\lambda$, and all its nonempty closed-manifold and positive-function hypotheses hold. Its reciprocal conclusion makes division by $\phi$ smooth and bounded. [given, F1, F3]

2.1 Expand $\Delta_h(\phi w)=\phi\Delta_hw+2\nabla\phi\cdot\nabla w+w\Delta_h\phi$. The zeroth-order terms cancel by $L\phi=\lambda\phi$, giving the displayed $P$ with $\nabla\log\phi=\phi^{-1}\nabla\phi$. For any smooth complex $w$, integration by parts gives $\int_Sm Pw=\int_S\chi(L-\lambda)(\phi w)=\int_S(L^\dagger-\lambda)\chi\,\phi w=0$. All these operations are valid for complex functions by applying the real identity to their real and imaginary parts. [F1, F4, step 1.1]

3.1 The product rule gives $P|w|^2=2\operatorname{Re}(\overline w Pw)-2|\nabla w|^2$. For $w=\psi/\phi$, the eigenvalue equation becomes $Pw=(\mu-\lambda)w$. Integrating this product identity against $m>0$ and using step 2.1 yields $(\operatorname{Re}\mu-\lambda)\int_Sm|w|^2=\int_Sm|\nabla w|^2\ge0$. The denominator is positive, proving the spectral ordering. If $\mu=\lambda$, the last integral is zero, so every component of $\nabla w$ vanishes everywhere. Applying F2 separately to the smooth real functions $\operatorname{Re}w$ and $\operatorname{Im}w$, whose differentials vanish, shows that both are constant on connected $S$; hence $w$ is constant. Conversely every constant multiple of $\phi$, including zero, satisfies $L\psi=\lambda\psi$ and belongs to the eigenspace; its nonzero multiples are eigenfunctions. Thus the eigenspace at $\lambda$ is exactly the complex span of $\phi$. [F1, F2, F3, F4, step 1.1, step 2.1]

4.1 Let $u$ be any smooth everywhere positive real eigenfunction with $Lu=\nu u$, initially allowing $\nu\in\mathbb C$. On the nonempty $S$ now under consideration, evaluate at any $p\in S$: real coefficients and $u(p)>0$ give $\nu=(Lu)(p)/u(p)\in\mathbb R$. Apply the positive-adjoint-pairing lemma to the right eigenfunction $u$ at $\nu$ and the adjoint eigenfunction $\chi$ at the real eigenvalue $\lambda$ from step 1.1. The same nonempty closed manifold and operator are used, both functions are smooth and positive, and both eigenvalues are real; hence $\nu=\lambda$. Step 3.1 gives $u=a\phi$ for a complex constant $a$, and evaluating at $p$ gives $a=u(p)/\phi(p)>0$. This proves uniqueness among all positive real eigenfunctions, even when their eigenvalues were initially allowed to differ, and completes the Statement without a selfadjointness assumption on $L$. [F1, F3, step 1.1, step 3.1] ∎

---
title: Lifting a normalized stationary primitive to the Harrison parameter
status: published
research_item: lem-author-7a3c9628f105-primitive-parameter-lift
dependency_level: 2
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: Section 1.1, differentiated notation after (1.1); Section 3.2,
        equations (3.12)–(3.18).
      statement: The source defines componentwise Cartesian differentiated decay
        notation and constructs the parameter one-form from a normalized
        stationary primitive by a polynomial formula, obtaining its curl and
        contraction identities.
      hypotheses: The source works with its stationary vacuum data and a normalized
        primitive at a zero of the stationary field. This local calculation
        assumes the displayed primitive identities directly; it does not assume
        the vacuum equations to derive them.
      reading_limits: Consulted the named HTML passages, including the formulas and
        their adjacent explanations. Only notation and attribution are taken
        from them. The conditional algebra and uniform derivative estimate are
        proved locally; no primitive existence theorem or field-equation
        conclusion is imported.
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [lem-author-7a3c9628f105-denominator-positivity](item-lem-author-7a3c9628f105-denominator-positivity)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula)
- [math:def-lie-derivative-of-a-differential-form](https://alphabetamath.cc/item/def-lie-derivative-of-a-differential-form)
- [` Alexandru F. Radu, Rigidity of stationary black holes with small ADM angular momentum · Section 1.1, differentiated notation after (1.1); Section 3.2, equations (3.12)–(3.18). `](https://arxiv.org/html/2610.09729v1)


## Statement

Work on an open domain $U$ containing $p$, with $\psi:U\to\mathbb R$ smooth and real-valued, $f=-g(T,T)$, and both $f$ and $\psi$ constant along every local integral curve of $T$ contained in $U$. Assume the stationary Lorentzian and denominator data specified in [F1]–[F2], a real two-form $F=\tfrac12\mathrm dT^\flat$, and a smooth stationary one-form $W_0$ (meaning $\mathcal L_TW_0=0$) with $\mathrm dW_0=4((f-1)F+\psi\star_gF)$ and $W_0(T)=D_0(p)-D_0$, where $T(p)=0$. Define $W_q=(1-q)^2W_0-4q(1-q)T^\flat$ for $q\in[0,1]$. Then $W_q(T)=D_q(p)-D_q$, $\mathrm dW_q=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$, $W_1=0$, and $W_q$ is smooth in spacetime and $q$.

For the decay assertion, take the spatial components in one fixed Cartesian exterior chart $x=(x^1,x^2,x^3)$ with $r=|x|>R_0>0$, and let $T_i$ denote the spatial components of $T^\flat$. Interpret differentiated estimates and parameter uniformity by [F3]. If $(W_0)_i=O_5(r^{-3})$ and $T_i=O_5(r^{-2})$ in this same chart, then $(W_q)_i=O_5(r^{-2})$ uniformly for $q\in[0,1]$.

## Statement references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[lem-author-7a3c9628f105-denominator-positivity](item-lem-author-7a3c9628f105-denominator-positivity)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula)

[math:def-lie-derivative-of-a-differential-form](https://alphabetamath.cc/item/def-lie-derivative-of-a-differential-form)

## Facts & Assumptions

[F1] Stationarity of $(g,T)$ and $T^\flat$ use [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data), and the real two-form and star use [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data). A smooth one-form $\omega$ is called stationary when $\mathcal L_T\omega=0$, with the Lie derivative of a differential form defined in [math:def-lie-derivative-of-a-differential-form](https://alphabetamath.cc/item/def-lie-derivative-of-a-differential-form).

[F2] On the open domain $U$ containing $p$ specified in the Statement, $\sigma=f+i\psi$ is smooth, $f=-g(T,T)$, and $\psi:U\to\mathbb R$ is smooth and real-valued. Both $f$ and $\psi$ are constant along every local integral curve of $T$ contained in $U$. Thus the scalar $D_q=|1+q-(1-q)\sigma|^2$ obeys the polynomial identity of [lem-author-7a3c9628f105-denominator-positivity](item-lem-author-7a3c9628f105-denominator-positivity) on $U$ for $q\in[0,1]$.

[F3] The fixed Cartesian exterior chart, multi-index derivatives, componentwise $O_m(r^{-b})$ bounds and parameter-uniform estimates are those of [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data). Uniformity requires a common radius and derivative constants for every parameter value. Only this fixed-chart notation is used; no existence or coordinate invariance of an end is asserted.

[F4] The operator $\mathrm d$ is the exterior derivative of [math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula). For a smooth real one-form $\omega$ and smooth vector fields $X,Y$, its formula is $(\mathrm d\omega)(X,Y)=X(\omega(Y))-Y(\omega(X))-\omega([X,Y])$.

## Proof

**Given:** The hypotheses in the Statement and the interfaces in [F1]–[F4].

**Goal:** Establish the polynomial identities, smoothness and conditional uniform decay.

1.1 Since $T^\flat(T)=-f$ and $T(p)=0$ gives $f(p)=0$, contraction yields $W_q(T)=(1-q)^2(D_0(p)-D_0)+4q(1-q)f$. Subtract the polynomial identity $D_q=(1-q)^2D_0+4q(1-(1-q)f)$ at the variable point from its value at $p$ to obtain $D_q(p)-D_q$. [given, F1, F2, algebra]

1.2 Expanding the three terms of [F4] for $a\alpha+b\eta$, with real constants $a,b$ and smooth real one-forms $\alpha,\eta$, gives $\mathrm d(a\alpha+b\eta)=a\,\mathrm d\alpha+b\,\mathrm d\eta$: each derivative and evaluation is real-linear in the one-form. With $q$ fixed, the coefficients $(1-q)^2$ and $-4q(1-q)$ are spacetime constants, so this linearity and the given $\mathrm dT^\flat=2F$ give $\mathrm dW_q=4(1-q)^2((f-1)F+\psi\star_gF)-8q(1-q)F$. The coefficient of $F$ simplifies to $4(1-q)((1-q)f-(1+q))$, giving the asserted curl. The defining formula for $W_q$ is polynomial in $q$ with smooth stationary coefficients and gives $W_1=0$. [given, F1, F4, algebra]

2.1 In the chart of the decay assertion, let $\beta$ be any multi-index with $|\beta|\le5$. By [F3] the two input estimates give a common radius $R>\max\{R_0,1\}$ and constants $A_\beta,B_\beta\ge0$ with $|\partial^\beta(W_0)_i|\le A_\beta r^{-3-|\beta|}$ and $|\partial^\beta T_i|\le B_\beta r^{-2-|\beta|}$ for every spatial component and $r\ge R$. These inputs have no $q$ dependence. Since $0\le(1-q)^2\le1$ and $0\le4q(1-q)\le1$ on $[0,1]$, differentiating the defining component formula gives $|\partial^\beta(W_q)_i|\le A_\beta r^{-3-|\beta|}+B_\beta r^{-2-|\beta|}\le(A_\beta+B_\beta)r^{-2-|\beta|}$. The same radius and constants work for all $q\in[0,1]$, precisely the required uniform $O_5(r^{-2})$ estimate. [given, F1, F3, algebra] ∎

## Source notes

The polynomial construction and normalization are attributed to Radu, Section 3.2 (3.12)–(3.18); the fixed-chart differentiated notation is stated in Section 1.1 after (1.1). The proof here is a local conditional calculation, including the explicit uniform derivative bound. Neither existence of the stationary primitive nor the Einstein–Maxwell equations are imported or established here.

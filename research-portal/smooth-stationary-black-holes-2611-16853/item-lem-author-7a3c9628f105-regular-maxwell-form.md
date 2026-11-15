---
title: Smooth Maxwell tensor formula without division by the stationary norm
status: draft
research_item: lem-author-7a3c9628f105-regular-maxwell-form
dependency_level: 4
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: Section 3.1, equation (3.5); Section 3.2, equations (3.12),
        (3.19)–(3.25) and the paragraphs immediately before (3.24) and after
        (3.25).
      statement: The regular electromagnetic tensor is the displayed complex multiple
        of the rank-one pullback of the original self-dual form. Its contraction
        with the normalized stationary field is the derivative of the displayed
        Harrison potential; it is spacetime smooth and parameter continuous with
        zero field at q=1.
      hypotheses: The source uses stationary vacuum data and a smooth normalized
        primitive. This item assumes the smooth family, positive denominators,
        orientation, contraction normalization and scalar identities
        conditionally; no existence theorem or field equation is imported.
      reading_limits: Consulted the named HTML formulas and adjacent explanations. The
        local algebra is checked using the declared mathematical suppliers; no
        Einstein–Maxwell, primitive-existence, flux or horizon result is claimed
        to have been reconstructed.
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [lem-author-7a3c9628f105-rank-one-metric](item-lem-author-7a3c9628f105-rank-one-metric)
- [lem-author-7a3c9628f105-primitive-parameter-lift](item-lem-author-7a3c9628f105-primitive-parameter-lift)
- [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)
- [math:def-interior-product-of-a-form-by-a-vector-field](https://alphabetamath.cc/item/def-interior-product-of-a-form-by-a-vector-field)
- [` Alexandru F. Radu, Rigidity of stationary black holes with small ADM angular momentum · Section 3.1, equation (3.5); Section 3.2, equations (3.12), (3.19)–(3.25) and the paragraphs immediately before (3.24) and after (3.25). `](https://arxiv.org/html/2610.09729v1)


## Statement

Assume the family and orientation in [lem-author-7a3c9628f105-rank-one-metric](item-lem-author-7a3c9628f105-rank-one-metric). Let $\mathcal F=F+i\star_gF$ satisfy $i_T\mathcal F=\tfrac12\mathrm d\sigma$ and $\mathrm d\sigma(T)=0$. Put $H_q=1+q-(1-q)\sigma$, $D_q=|H_q|^2$, and $Z_q=-\sqrt{1-q^2}(\overline{H_q}/H_q)(\mathcal F+(2D_q)^{-1}W_q\wedge\mathrm d\sigma)$. Then $Z_q$ is self-dual for $g_q$ and equals $F_q+i\star_{g_q}F_q$ for the real two-form $F_q=\operatorname{Re}Z_q$. It is spacetime smooth, continuous in $q\in[0,1]$, and $F_1=0$. Moreover $i_{4T/D_q(p)}Z_q=\mathrm d\Phi_q$ where $\Phi_q=-\sqrt{1-q^2}(1+\sigma)/H_q$.

## Facts & Assumptions

[F1] The metric, metric index contraction and stationary scalar conventions use [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] Self-duality and fiberwise pullback use [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data).

[F3] The orientation-preserving map and metric are those of [lem-author-7a3c9628f105-rank-one-metric](item-lem-author-7a3c9628f105-rank-one-metric).

[F4] The smooth family $W_q$ and the contraction normalization $W_q(T)=D_q(p)-D_q$ are supplied by [lem-author-7a3c9628f105-primitive-parameter-lift](item-lem-author-7a3c9628f105-primitive-parameter-lift).

[F5] The Hodge star is the unique smooth map characterized on real two-forms by $\alpha\wedge\star_g\beta=\langle\alpha,\beta\rangle_g\,\mathrm{vol}_g$, where $\langle\alpha,\beta\rangle_g=\tfrac12\alpha_{ab}\beta^{ab}$; it satisfies $\star_g^2=-\operatorname{id}$. These are mathematical conclusions of [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus).

[F6] Interior product of a smooth form by a smooth vector field is the pointwise operation of [math:def-interior-product-of-a-form-by-a-vector-field](https://alphabetamath.cc/item/def-interior-product-of-a-form-by-a-vector-field): $(i_X\omega)_x(v_2,\ldots,v_k)=\omega_x(X_x,v_2,\ldots,v_k)$ for $k\ge1$. On the complex forms of [F2], extend it by $i_X(U+iV)=i_XU+i\,i_XV$.

[F7] The exterior derivative and its local coordinate formula and graded product rule are supplied by [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus). For a smooth real function $u$, $(\mathrm du)(X)=X(u)$. For a smooth complex function $u+iv$ with real $u,v$, use the componentwise extension $\mathrm d(u+iv)=\mathrm du+i\,\mathrm dv$; the product rule extends by complex bilinearity. All derivatives here are in spacetime at fixed $q$.

## Proof

**Given:** The hypotheses in the Statement and the Facts above.

**Goal:** Establish the stated conclusions.

1.1 Expanding the alternating form gives $A_q^*\mathcal F=\mathcal F+D_q^{-1}W_q\wedge i_T\mathcal F=\mathcal F+(2D_q)^{-1}W_q\wedge\mathrm d\sigma$. The defining metric-and-volume identity for the Hodge star is preserved by an orientation-preserving invertible linear map; in dimension four a positive conformal factor cancels on two-forms. Consequently $A_q^*\mathcal F$ is self-dual for $(D_q/4)A_q^*g$. Complex scalar multiplication preserves this eigenspace. Writing $Z_q=U+iV$ and comparing real parts in $\star_{g_q}Z_q=-iZ_q$ gives $V=\star_{g_q}U$. [given, F1, F2, F3, F5, F6]

2.1 Put $C=D_q(p)$. Using $W_q(T)=C-D_q$ from [F4] and $\mathrm d\sigma(T)=0$, contraction with $T$ gives $i_T(A_q^*\mathcal F)=\tfrac12(1+W_q(T)/D_q)\mathrm d\sigma=C\,\mathrm d\sigma/(2D_q)$. Multiplication by the displayed factor and $4/C$ yields $-2\sqrt{1-q^2}\,\mathrm d\sigma/H_q^2$, using $D_q=H_q\overline H_q$. Using the scalar exterior derivative and its componentwise complex extension in [F7], differentiating $\Phi_q$ gives exactly this expression. Positivity of $D_q$ removes every spacetime singular denominator, and the only endpoint factor $\sqrt{1-q^2}$ is continuous and vanishes at one. This proves the regularity and endpoint claims, without asserting differentiability in $q$ at one. [given, F1, F3, F4, F6, F7, algebra, step 1.1] ∎

## Source notes

This conditional calculation follows §3.2 (3.24)–(3.25) of the cited independent source. No existence of the stationary primitive or Einstein–Maxwell solution is inferred from this calculation alone.

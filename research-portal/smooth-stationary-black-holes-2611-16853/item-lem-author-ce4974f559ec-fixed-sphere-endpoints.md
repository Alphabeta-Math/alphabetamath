---
title: The zero Harrison parameter follows from continuity on one fixed sphere
status: draft
research_item: lem-author-ce4974f559ec-fixed-sphere-endpoints
dependency_level: 4
---

## Prerequisites

- [def-harrison-electromagnetic-form](item-def-harrison-electromagnetic-form)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-harrison-one-form-family](item-def-harrison-one-form-family)
- [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data)
- [math:prop-integration-over-an-oriented-embedded-submanifold](https://alphabetamath.cc/item/prop-integration-over-an-oriented-embedded-submanifold)
- [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)
- [math:lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary](https://alphabetamath.cc/item/lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary)
- [math:cor-change-of-variables-for-compactly-supported-functions](https://alphabetamath.cc/item/cor-change-of-variables-for-compactly-supported-functions)
- [math:thm-continuous-on-a-rectangle-is-riemann-integrable](https://alphabetamath.cc/item/thm-continuous-on-a-rectangle-is-riemann-integrable)
- [math:thm-multidimensional-integral-properties](https://alphabetamath.cc/item/thm-multidimensional-integral-properties)
- [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)
- [math:thm-heine-cantor-metric](https://alphabetamath.cc/item/thm-heine-cantor-metric)


## Statement

Let $C$ be one fixed compact oriented smooth embedded two-sphere in the common regular region of a Harrison family $q\in[0,1]$. Suppose $g_q$ is jointly continuous in parameter and spacetime, Lorentzian with fixed spacetime orientation, and $F_q$ is a jointly continuous real two-form. For a continuous two-form $\omega$ along $C$, define $\int_C\omega$ by a finite positively oriented chart sum of the continuous pullback coefficients, using a smooth partition of unity on $C$. This integral is independent of those choices and agrees with smooth-form integration when $\omega$ is smooth. Use the same flux normalization $Q_E(C,q)=(4\pi)^{-1}\int_C\star_{g_q}F_q$ and $Q_M(C,q)=(4\pi)^{-1}\int_CF_q$; these extend the smooth geometric charge convention and require no spacelike condition on $C$.

Then both integrals and both fluxes are continuous in $q$. Consequently identities $Q_E(C,q)=\sqrt{1-q^2}$ and $Q_M(C,q)=0$ valid for every $0<q<1$ extend to $q=0$ and $q=1$. At $q=1$ the Harrison electromagnetic definition independently gives $F_1=0$.

For the algebraic Harrison family, the continuity hypotheses follow from fixed smooth seed data and one fixed supplied smooth normalized primitive $W_0$, with $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, wherever the algebraic denominators stay positive on this common region. The other regular-Harrison hypotheses, including Lorentzian character and the fixed orientation, are retained. Positivity alone makes no assertion about the parameter dependence of independently chosen primitives.

## Facts & Assumptions

**Given:** The hypotheses and supplied data in the Statement; work in ZFC.

**Goal:** Establish well-definedness, parameter continuity and both endpoint identities.

[F1] The Harrison definitions give $B_q=q(1+\sigma)+(1-\sigma)$, $D_q=|B_q|^2$, $A_qv=v+D_q^{-1}W_q(v)T$, $g_q=(D_q/4)A_q^*g$, and $\mathcal H_q=-\sqrt{1-q^2}(\overline{B_q}/B_q)A_q^*\mathcal F$, with $F_q=\operatorname{Re}\mathcal H_q$. One fixed supplied smooth normalized primitive defines $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. [def-harrison-electromagnetic-form](item-def-harrison-electromagnetic-form) [def-harrison-normalization](item-def-harrison-normalization) [def-harrison-one-form-family](item-def-harrison-one-form-family)

[F2] The geometric flux convention uses oriented pullback integrals divided by $4\pi$; smooth integration on a compact oriented embedded surface does not require its tangent planes to be spacelike. In positive spacetime coordinates the pointwise Hodge formula is $(\star_gF)_{ab}=\frac12\sqrt{|\det g|}\,\epsilon_{abcd}g^{ce}g^{df}F_{ef}$, where $\epsilon_{0123}=1$ is the alternating symbol. [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data) [math:prop-integration-over-an-oriented-embedded-submanifold](https://alphabetamath.cc/item/prop-integration-over-an-oriented-embedded-submanifold) [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[F3] A compact subset of an oriented smooth manifold admits a finite nonnegative smooth chart localization whose sum is one near that subset and whose individual supports are compact in the corresponding chart domains. [math:lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary](https://alphabetamath.cc/item/lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary)

[F4] Continuous real functions on a closed nondegenerate Euclidean rectangle are Riemann integrable. Compactly supported Riemann integrands satisfy change of variables under an injective $C^1$ map with invertible derivative on an open set containing the relevant compact preimage. Riemann integrals have finite linearity, monotonicity and the absolute-value estimate. [math:thm-continuous-on-a-rectangle-is-riemann-integrable](https://alphabetamath.cc/item/thm-continuous-on-a-rectangle-is-riemann-integrable) [math:cor-change-of-variables-for-compactly-supported-functions](https://alphabetamath.cc/item/cor-change-of-variables-for-compactly-supported-functions) [math:thm-multidimensional-integral-properties](https://alphabetamath.cc/item/thm-multidimensional-integral-properties)

[F5] Closed bounded Euclidean boxes are compact in the Euclidean metric, and a continuous real function on a compact metric domain is uniformly continuous. [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn) [math:thm-heine-cantor-metric](https://alphabetamath.cc/item/thm-heine-cantor-metric)

## Proof

**Given:** The hypotheses and supplied data in the Statement; work in ZFC.

**Goal:** Establish the Statement.

**Proof technique:** direct.

1.1 Apply [F3] to $C$ to obtain finitely many positively oriented charts $\phi_i:U_i\to V_i\subset\mathbb R^2$ and nonnegative smooth $\rho_i$ with $\sum_i\rho_i=1$ and $\operatorname{supp}\rho_i$ compact in $U_i$. For a continuous two-form $\omega$ along $C$, let $a_i$ be the coefficient of $\rho_i i^*\omega$ in the chart, where $i:C\hookrightarrow M$ is the inclusion and $(i^*\omega)_p(v,w)=\omega_{i(p)}(di_pv,di_pw)$ defines the continuous pullback pointwise, and extend it by zero to $\mathbb R^2$. The compact support lies inside $V_i$, so this extension is continuous, including across the chart edge. Choose a closed nondegenerate rectangle $Q_i$ whose interior contains that support and set $I_C(\omega)=\sum_i\int_{Q_i}a_i(x)\,dx$. Each summand exists by [F4]; enlarging a rectangle adds only zero contributions, by coordinate-slice additivity. This defines the claimed finite chart sum for continuous forms. [given, F3, F4]

1.2 Nondegeneracy of each $g_q$ gives the continuous inverse through the adjugate divided by its nonzero determinant. The factor $\sqrt{|\det g_q|}$ is continuous as well. The pointwise formula in [F2], interpreted algebraically for continuous fields, therefore defines $\star_{g_q}F_q$ with jointly continuous coefficients. This algebraic map is coordinate independent because it is characterized pointwise by the metric wedge pairing; it agrees with the smooth Hodge star whenever the metric and form are smooth. Pullback along the fixed smooth inclusion preserves joint continuity, so both pulled-back two-form families have jointly continuous coefficients on $[0,1]\times C$. [given, F2, algebra]

1.3 For the specified fixed primitive in [F1], the coefficients of $W_q$ are polynomials in $q$ with fixed smooth spacetime coefficients, and hence are jointly continuous. The same holds for $B_q$ and $D_q$. Where $D_q>0$, also $B_q\ne0$; their reciprocals, $A_q$, $g_q$ and the displayed electromagnetic formula are therefore jointly continuous by their finite sums, products and quotients. The factor $\sqrt{1-q^2}$ is continuous on the closed interval, although no parameter differentiability at one is needed. This proves the asserted sufficient continuity condition for that single family; existence of its primitive and the stated regularity region are supplied hypotheses. [given, F1, algebra]

2.1 Given a second such localization $(\tau_j,\psi_j)$, insert $\sum_j\tau_j=1$ into every summand of the first. Each $\rho_i\tau_j i^*\omega$ has compact support inside $U_i\cap U'_j$. On the overlap the continuous top-form coefficients transform by the determinant of $D(\psi_j\phi_i^{-1})$. This transition is an orientation-preserving smooth diffeomorphism between open Euclidean sets; the determinant is positive. Apply the compact-support change-of-variables formula in [F4] to these continuous zero-extended coefficients. Its support lies inside the target overlap and its preimage is compact under the inverse transition, so all its hypotheses hold. Thus the two chart integrals for each product agree. Finite linearity identifies both localization sums with the same double sum, proving independence. For smooth $\omega$ this is exactly the chart construction of the pullback integral in [F2], so it agrees with the existing geometric fluxes. Neither construction uses an induced positive-definite metric on $C$. [F2, F4, step 1.1]

3.1 Use the one fixed localization of step 1.1 for either family in step 1.2 and write its zero-extended coefficients as $a_i(q,x)$. These are jointly continuous on $[0,1]\times\mathbb R^2$: their common spatial supports lie in the compact chart supports of $\rho_i$, away from every artificial chart edge. Choose fixed rectangles $Q_i$ containing those supports. The set $[0,1]\times Q_i$ is a closed bounded box in $\mathbb R^3$, with its Euclidean metric, hence compact by [F5]. Heine-Cantor applies to $a_i$ on this box and gives $\sup_{x\in Q_i}|a_i(q,x)-a_i(q_0,x)|\to0$ as $q\to q_0$, including one-sided limits at the endpoints. By [F4], $|I_C(\omega_q)-I_C(\omega_{q_0})|\leq\sum_i\operatorname{vol}(Q_i)\sup_{x\in Q_i}|a_i(q,x)-a_i(q_0,x)|\to0$. The finite sum proves continuity of both integrals and, after division by $4\pi$, both fluxes. [F4, F5, step 1.1, step 2.1, step 1.2]

4.1 Apply the continuity just proved to the identities assumed on $0<q<1$. Letting $q\downarrow0$ gives $Q_E(C,0)=1$ and $Q_M(C,0)=0$; letting $q\uparrow1$ gives $Q_E(C,1)=Q_M(C,1)=0$. Independently, the regular electromagnetic formula in [F1] has $B_1=2$ and finite $A_1$, and its factor $\sqrt{1-q^2}$ vanishes at one, so $F_1=0$. Every integral and parameter limit has been taken on the same compact sphere; no limit at spatial infinity or exchange with such a limit occurs. [given, F1, step 3.1, step 1.3] ∎

---
title: Killing two-form and normalized Ernst notation
status: draft
research_item: def-killing-ernst-notation
dependency_level: 1
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 3, Definition 1.1(1); page 4, §1.2 before Theorem 1.1; page 7,
        §2.1
      statement: The article specifies the stationary exterior coordinate chart and
        introduces the Killing two-form, its complex self-dual form, the
        normalized Ernst potential and the indicated asymptotic orientation.
      hypotheses: The article's stationary vacuum setting and its specified asymptotic end.
      reading_limits: Read the frozen article text at the cited passages on PDF pages
        3, 4 and 7; this reference attributes the end chart and notation. The
        quantified end limit is made explicit locally, and the tensor identities
        are proved from mathematical suppliers rather than imported from the
        article.
---

PDF p. 3: ` Definition 1.1(1), stationary exterior coordinates `; PDF p. 4: ` §1.2 before Theorem 1.1 `; PDF p. 7: ` §2.1 `

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [physics:thm-gr-killing-and-on-shell-matter-identities](https://alphabetamath.cc/physics/item/thm-gr-killing-and-on-shell-matter-identities)
- [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Definition

Work in ZFC, including the axiom of choice. Let $(M,g,N,T)$ be stationary Lorentzian data: $M$ is an oriented smooth four-manifold, $g$ has signature $(-,+,+,+)$, $N$ is a time orientation, and $T$ is a smooth Killing field. Let $\nabla$ be the torsion-free metric-compatible connection of $g$, and let $T_b=g_{bc}T^c$. Define the Killing two-form by $F_{ab}=\nabla_aT_b$ and put $f=-g(T,T)$.

Let $\epsilon$ be the oriented metric volume form and $\star_g$ the Hodge star of $g$ and the chosen orientation. Define $\mathcal F=F+i\star_gF$ and $\mathcal F^2=\mathcal F_{ab}\mathcal F^{ab}$, where both indices are raised with $g^{-1}$ and the contraction is complex bilinear, without conjugation or a factor of one half. Thus $\star_g\mathcal F=-i\mathcal F$ and $(\star_gF)_{ab}=\frac12\epsilon_{ab\mu\nu}F^{\mu\nu}$.

For normalization on an open set $U\subseteq M$, a designated coordinate end consists of a supplied open subset $U_{\mathrm{end}}\subseteq U$ and a smooth coordinate diffeomorphism $(t,x):U_{\mathrm{end}}\to I\times\{x\in\mathbb R^3:|x|>R_0\}$, where $I\subseteq\mathbb R$ is a nonempty open interval, $R_0>0$, and $T=\partial_t$ in these coordinates. Put $r=|x|=(\sum_{i=1}^3(x^i)^2)^{1/2}$. The orientation convention is that $dt\wedge dx^1\wedge dx^2\wedge dx^3$ is positive on this end. The article's asymptotic chart has $I=\mathbb R$; metric decay is a separate hypothesis, not part of these coordinate-end data.

On such a $U$, a normalized Ernst potential, when one exists, is a smooth complex function $\sigma=f+i\psi$, with real $\psi$, satisfying $\nabla_a\sigma=2T^b\mathcal F_{ba}$ and $\sigma\to1$ along the designated coordinate end. Precisely, this limit means that for every $\varepsilon>0$ there is $R>R_0$ such that $|\sigma(t,x)-1|<\varepsilon$ for every $t\in I$ and every $x\in\mathbb R^3$ with $|x|>R$, where $|\cdot|$ on complex numbers denotes their modulus. Thus the limit is uniform in the time coordinate and the spatial directions. Consequently $\nabla_a\psi=T^b\epsilon_{ba\mu\nu}F^{\mu\nu}$. Here the covariant derivative of a scalar is its ordinary differential. Neither existence of $\sigma$ nor the existence of such an end is asserted by this definition.

## Definition references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[physics:thm-gr-killing-and-on-shell-matter-identities](https://alphabetamath.cc/physics/item/thm-gr-killing-and-on-shell-matter-identities)

[physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[A1] The background convention is ZFC, including the axiom of choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The stationary data supply the smooth metric, orientation, Killing field, inverse metric and unique torsion-free metric-compatible connection. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] For the stated smooth Lorentzian data, the Killing equation is $\nabla_aT_b+\nabla_bT_a=0$. [physics:thm-gr-killing-and-on-shell-matter-identities](https://alphabetamath.cc/physics/item/thm-gr-killing-and-on-shell-matter-identities)

[F3] For a real two-form, the complex-linear Hodge star and the complex bilinear contraction have the stated meanings, and $\star_g^2=-\operatorname{id}$ on real two-forms. [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data) [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[F4] For a real two-form, the oriented Lorentzian Hodge star has components $(\star_gF)_{ab}=\frac12\epsilon_{ab\mu\nu}F^{\mu\nu}$. [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

## Justification

**Given:** The data in the Definition, and, for the assertions about $\sigma$, a function $\sigma$ satisfying the stated conditional definition.

**Goal:** Justify the two-form, the displayed identities and the coordinate-end normalization conventions.

1.1 By the Killing equation, $F_{ab}=-F_{ba}$, so the smooth covariant derivative of $T^\flat$ defines a real two-form. Metric compatibility gives $\nabla_af=-2T^b\nabla_aT_b=2T^bF_{ba}$. Thus the real part of the proposed potential equation agrees with $df$; this calculation does not establish existence of a potential. [F1, F2, algebra]

2.1 The Hodge star is extended complex linearly, so $\star_g\mathcal F=\star_gF+i\star_g^2F=\star_gF-iF=-i\mathcal F$. Its component formula gives $2T^b(\star_gF)_{ba}=T^b\epsilon_{ba\mu\nu}F^{\mu\nu}$. Taking imaginary parts of the assumed potential equation therefore yields the stated formula for $\nabla_a\psi$. The inverse metric supplies the indicated contraction. [given, F1, F3, F4, step 1.1, algebra]

3.1 The supplied end diffeomorphism defines $r$ and each region $r>R$ explicitly, so the quantified modulus bound defines the normalization without an implicit notion of approach to infinity. Moreover $T^a\nabla_a\sigma=2T^aT^b\mathcal F_{ba}=0$ by alternation of $\mathcal F$. Since $T=\partial_t$, the potential is independent of $t$ on the interval $I$. Hence the stated uniformity in $t$ follows already from the potential equation when the spatial limit holds on any one time slice. The end chart, its orientation and the limit are supplied conditions; their existence has not been deduced. [given, F1, F3, step 1.1, step 2.1, algebra] ∎

## Source notes

The article introduces this notation in the cited passages. Its citation records attribution; the identities above use the stated mathematical suppliers. The coordinate-end and quantified-limit clauses are explicit local definitions, with no imported end-existence or asymptotic-flatness theorem.

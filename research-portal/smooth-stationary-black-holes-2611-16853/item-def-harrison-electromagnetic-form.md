---
title: Harrison electromagnetic form
status: draft
research_item: def-harrison-electromagnetic-form
dependency_level: 3
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 6, section 1.4; page 8, equation (2.6) and the following
        displayed formula
      statement: The Harrison electromagnetic form is the displayed scalar multiple of
        the pullback of the complex Killing two-form, equivalently the displayed
        wedge expression; its real part has Hodge dual equal to its imaginary
        part.
      hypotheses: The article's stationary vacuum setting, its chosen orientation and
        Harrison data, with the displayed denominators nonzero.
      reading_limits: Read the frozen article text at the cited passages. This
        reference attributes the formulas and is not used as proof of their
        algebraic properties.
---

PDF p. 6: ` §1.4 `; PDF p. 8: ` (2.6) `

## Prerequisites

- [def-harrison-one-form](item-def-harrison-one-form)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-killing-ernst-notation](item-def-killing-ernst-notation)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data)


## Definition

Use stationary Lorentzian data $(M,g,N,T)$ and a supplied normalized Ernst potential $\sigma=f+i\psi$ on an open set $U$, with $f=-g(T,T)$, Killing two-form $F_{ab}=\nabla_aT_b$, complex two-form $\mathcal F=F+i\star_gF$, and $d\sigma=2\iota_T\mathcal F$. Here $\iota_T\mathcal F$ is the one-form $v\mapsto\mathcal F(T,v)$, and the Hodge star uses the supplied orientation. Fix $q\in[0,1]$, put $B_q=q(1+\sigma)+(1-\sigma)$ and $D_q=B_q\overline{B_q}$, and use the Harrison one-form data on an open subset $V\subseteq U$ where $D_q>0$. In particular, $W_q$ is the supplied real one-form, $A_qv=v+D_q^{-1}W_q(v)T$, and $g_q=(D_q/4)A_q^*g$ is the supplied Lorentzian metric. The pullback is fiberwise: $(A_q^*\mathcal F)(u,v)=\mathcal F(A_qu,A_qv)$.

Define the complex Harrison electromagnetic two-form and its real part by

$$\mathcal H_q=-\sqrt{1-q^2}\,\frac{\overline{B_q}}{B_q}A_q^*\mathcal F=-\sqrt{1-q^2}\,\frac{\overline{B_q}}{B_q}\left(\mathcal F+\frac{W_q\wedge d\sigma}{2D_q}\right),\qquad F_q=\operatorname{Re}\mathcal H_q.$$

With the same orientation used for $g_q$ as for $g$, the associated identity is $\star_{g_q}F_q=\operatorname{Im}\mathcal H_q$. No Maxwell equation or existence of $W_q$ is asserted by this definition.

## Definition references

[def-harrison-one-form](item-def-harrison-one-form)

[def-harrison-normalization](item-def-harrison-normalization)

[def-killing-ernst-notation](item-def-killing-ernst-notation)

[def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data)

## Facts & Assumptions

[F1] The normalized Ernst data supply the smooth complex two-form $\mathcal F$, the relation $d\sigma=2\iota_T\mathcal F$, and the identity $\star_g\mathcal F=-i\mathcal F$. [def-killing-ernst-notation](item-def-killing-ernst-notation) [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[F2] The Harrison data give $D_q>0$ on $V$, $W_q(T)=d_q-D_q$, $d_q>0$, the invertible map $A_q$, and $g_q=(D_q/4)A_q^*g$. [def-harrison-one-form](item-def-harrison-one-form) [def-harrison-normalization](item-def-harrison-normalization)

[F3] The oriented metric Hodge map is characterized by $\alpha\wedge\star_g\beta=\langle\alpha,\beta\rangle_g\,\mathrm{vol}_g$ and extends complex linearly. [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data) [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

## Justification

**Given:** The data, parameter and restrictions in the Definition.

**Goal:** Establish well-definedness, the wedge formula, and the Hodge identity.

1.1 Since $D_q=|B_q|^2>0$, the denominator $B_q$ is nonzero, and all coefficients are smooth; $\sqrt{1-q^2}$ is a real constant, including at the endpoints. Expanding the two arguments of the alternating form gives $A_q^*\mathcal F=\mathcal F+D_q^{-1}W_q\wedge\iota_T\mathcal F$: the term with two copies of $T$ vanishes. Substitution of $d\sigma=2\iota_T\mathcal F$ proves the second expression and shows that $\mathcal H_q$ and $F_q$ are smooth two-forms. [given, F1, F2, algebra]

2.1 At each point, the rank-one determinant identity gives $\det A_q=1+D_q^{-1}W_q(T)=d_q/D_q>0$; thus $A_q$ preserves the specified orientation. Put $c=D_q/4>0$. For real two-forms $\alpha,\beta$, the defining Hodge pairing, $g_q=cA_q^*g$, and four-dimensional volume scaling yield $\langle A_q^*\alpha,A_q^*\beta\rangle_{g_q}=c^{-2}A_q^*\langle\alpha,\beta\rangle_g$ and $\mathrm{vol}_{g_q}=c^2A_q^*\mathrm{vol}_g$. Pulling back the defining wedge identity therefore gives $\star_{g_q}A_q^*\beta=A_q^*(\star_g\beta)$; nondegeneracy of the wedge pairing gives uniqueness. Complex linearity and $\star_g\mathcal F=-i\mathcal F$ imply $\star_{g_q}\mathcal H_q=-i\mathcal H_q$. Writing $\mathcal H_q=F_q+iG_q$ with real $G_q$, comparison of real parts gives $\star_{g_q}F_q=G_q=\operatorname{Im}\mathcal H_q$. [given, F1, F2, F3, step 1.1, algebra] ∎

## Source notes

The cited article attributes the formulas. The justification uses the supplied geometric definitions and pointwise algebra, and does not use the article's assertion as a premise.

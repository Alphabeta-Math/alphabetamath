---
title: Single-potential construction of the Harrison one-form family
status: draft
research_item: def-harrison-one-form-family
dependency_level: 2
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 9, §2.2, equation (2.9) and the following display
      statement: The article defines the family by W_q=(1-q)^2 W_0-4q(1-q)T-flat, with
        dW_0=4((f-1)F+psi star F), and gives W_0(T)=d_0-D_0.
      hypotheses: The stationary vacuum construction and the chosen normalized
        primitive in the article.
      reading_limits: Read the frozen article text at the cited passage. The reference
        attributes the construction; it is not used to establish existence of
        the primitive or to justify the algebra below.
---

PDF p. 9: ` (2.9) and definition of Θ0 `

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [def-killing-ernst-notation](item-def-killing-ernst-notation)
- [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus)
- [math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula)


## Definition

Let $(M,g,N,T)$ be the stationary Lorentzian data of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data), and let $U$ carry the supplied normalized Ernst potential $\sigma=f+i\psi$ of [def-killing-ernst-notation](item-def-killing-ernst-notation), with $f=-g(T,T)$ and real $\psi$. Thus $F_{ab}=\nabla_aT_b$ is the Killing two-form and $\star_gF$ is its metric Hodge dual with the specified orientation. Write $T^\flat=g(T,\cdot)$.

For $q\in[0,1]$, define the real functions $D_q=|q(1+\sigma)+(1-\sigma)|^2$ on $U$. Let a supplied point $p\in U$, called a pole for this construction, satisfy $T_p=0$, and put $d_q=D_q(p)$. These are pointwise definitions from the supplied potential and point. Define the real two-form $\Theta_0=4((f-1)F+\psi\star_gF)$.

A normalized primitive for this construction is a supplied smooth real one-form $W_0$ on $U$ satisfying both $dW_0=\Theta_0$ and $W_0(T)=d_0-D_0$. Here $d$ is exterior differentiation, and $W_0(T)$ is evaluation of the one-form on the vector field. For such a choice define $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. In stationary coordinates with $T=\partial_t$, the time component is $(W_0)_0=d_0-D_0$. Neither a primitive nor one satisfying the normalization is asserted to exist by this definition.

## Facts & Assumptions

[F1] The stationary data provide the smooth metric, Killing field, metric dual and scalar $f=-g(T,T)$. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] The Ernst interface gives the real two-form $F$, the real function $\psi$ and the conditional normalized potential $\sigma=f+i\psi$. [def-killing-ernst-notation](item-def-killing-ernst-notation)

[F3] The oriented Lorentzian Hodge star maps smooth real two-forms to smooth real two-forms. [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[F4] The local definitions are $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $d_q=D_q(p)$ for $q\in[0,1]$, where the supplied point $p\in U$ satisfies $T_p=0$. The smooth component functions $f,\psi$ of $\sigma=f+i\psi$ and the scalar $f=-g(T,T)$ are supplied by [def-killing-ernst-notation](item-def-killing-ernst-notation) and [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F5] For a smooth real one-form $\alpha$ and smooth vector fields $X,Y$, exterior differentiation is given by $(d\alpha)(X,Y)=X(\alpha(Y))-Y(\alpha(X))-\alpha([X,Y])$. [math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula)

[F6] For real $a,b$, the complex modulus satisfies $|a+ib|^2=a^2+b^2$. [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus)

## Justification

**Given:**The data, pole and normalized primitive stipulated in the Definition.

**Goal:** Justify the displayed forms and the time-component convention, and record the resulting contraction of the family.

1.1 The Killing form and its Hodge dual are smooth real two-forms, and $f$ and $\psi$ are smooth real functions. Their displayed linear combination therefore defines a smooth real two-form $\Theta_0$. The two conditions on $W_0$ are requirements on supplied data; they do not follow from the definition of $\Theta_0$. The displayed linear combination of $W_0$ and $T^\flat$ gives a unique smooth real one-form $W_q$ for each specified $q$. [given, F1, F2, F3]

2.1 In a coordinate chart with $T=\partial_t$, evaluation of a one-form on $T$ is its time component, so the stipulated normalization gives $(W_0)_0=d_0-D_0$. At the pole $f(p)=0$. Expanding the modulus gives $D_q=((1+q)-(1-q)f)^2+(1-q)^2\psi^2$ and $d_q=(1+q)^2+(1-q)^2\psi(p)^2$. Hence $d_q-D_q=(1-q)^2(d_0-D_0)+4q(1-q)f$. Since $T^\flat(T)=-f$, the definition of $W_q$ yields $W_q(T)=d_q-D_q$. [given, F1, F4, F6, step 1.1, algebra] ∎



The cited article attributes the construction. The calculation above uses the stated data and definitions; it does not prove existence or the regularity and decay properties of a normalized primitive.

## Source notes

The cited article attributes the construction. The calculation above uses the stated data and definitions; it does not prove existence or the regularity and decay properties of a normalized primitive.

---
title: Mass-one convention and Harrison denominator
status: published
research_item: def-harrison-normalization
dependency_level: 2
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 7–8, §2.1 and equation (2.1)
      hypotheses: The article's stationary vacuum setting, its normalized Ernst
        potential, q in [0,1], and its chosen pole p.
      reading_limits: Read the frozen article text at the cited passage. This
        reference attributes the notation and conventions; it is not used to
        prove existence or positivity.
---

PDF p. 7: ` §2.1; (2.1) `; PDF p. 8: ` §2.1; (2.1) `

## Prerequisites

- [def-killing-ernst-notation](item-def-killing-ernst-notation)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-surface-integral-on-a-compact-c-one-hypersurface](https://alphabetamath.cc/item/def-surface-integral-on-a-compact-c-one-hypersurface)
- [math:lem-surface-integral-is-independent-of-c-one-boundary-charts](https://alphabetamath.cc/item/lem-surface-integral-is-independent-of-c-one-boundary-charts)
- [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus)
- [math:cor-euclidean-closed-balls-and-spheres-are-compact](https://alphabetamath.cc/item/cor-euclidean-closed-balls-and-spheres-are-compact)
- [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)
- [math:thm-a-regular-level-set-is-an-embedded-submanifold](https://alphabetamath.cc/item/thm-a-regular-level-set-is-an-embedded-submanifold)


## Definition

Let $(M,g,N,T)$ be stationary Lorentzian data, and let $\Sigma_1$ be a supplied smooth spacelike maximal hypersurface for $g$: its induced metric $h$ is positive definite and its mean curvature vanishes. The subscript $1$ labels the original section. Let an asymptotic end of this section have Cartesian coordinates $x^i$, with $r=|x|$, and suppose the following ADM mass limit exists and equals one:

$$M_{\mathrm{ADM}}=\frac{1}{16\pi}\lim_{R\to\infty}\int_{|x|=R}(\partial_jh_{ij}-\partial_ih_{jj})\frac{x^i}{R}\,dS_{\mathrm{eucl}}=1.$$

Here repeated indices run from $1$ to $3$, $h_{ij}$ are the components of the induced metric in the chosen chart, and $dS_{\mathrm{eucl}}$ is Euclidean surface area on the coordinate sphere. This is the mass-one convention for the specified end; convergence of the limit and existence of such a section are assumptions.

On an open set $U$ with the designated asymptotic end, let $\sigma=f+i\psi$ be a supplied normalized Ernst potential: $f=-g(T,T)$, $\psi$ is real, $d\sigma=2T^b\mathcal F_{ba}\,dx^a$, and $\sigma\to1$ at the end, with $\mathcal F$ as in [def-killing-ernst-notation](item-def-killing-ernst-notation). For each real $q\in[0,1]$, define the complex function $B_q=q(1+\sigma)+(1-\sigma)$ and the real function $D_q=|B_q|^2=B_q\overline{B_q}$ on $U$.

If a supplied bifurcation surface $S$ meets $U$ and a point $p\in S\cap U$ satisfies $T_p=0$, define $d_q=D_q(p)$. Calling this chosen point a pole is terminology for this construction; neither its existence nor its uniqueness is asserted.

## Facts & Assumptions

[F1] Stationary Lorentzian data supply the metric and the smooth Killing field $T$. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] A spacelike maximal hypersurface has positive-definite induced metric $h$ and vanishing mean curvature. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F3] The asymptotic-data interface supplies the meaning of a Cartesian exterior chart and its coordinate radius $r$. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F4] The normalized Ernst notation specifies the conditional smooth complex potential and its component fields and asymptotic limit. [def-killing-ernst-notation](item-def-killing-ernst-notation)

[F5] A bifurcation surface is a specified smooth spacelike two-surface associated with the two branches of a bifurcate Killing horizon; its defining horizon generator need not be $T$. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[F6] In the inherited ZFC convention, surface integration on a compact embedded $C^1$ hypersurface in Euclidean space uses its chart-defined surface measure; this is a finite Borel measure independent of charts and subordinate partitions. Signed functions are integrated when their absolute values have finite integral. [math:def-surface-integral-on-a-compact-c-one-hypersurface](https://alphabetamath.cc/item/def-surface-integral-on-a-compact-c-one-hypersurface) [math:lem-surface-integral-is-independent-of-c-one-boundary-charts](https://alphabetamath.cc/item/lem-surface-integral-is-independent-of-c-one-boundary-charts)

[F7] For $z=a+ib$ with real $a,b$, conjugation and modulus are $\overline z=a-ib$ and $|z|=\sqrt{a^2+b^2}$. [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus)

[F8] Every Euclidean sphere in $\mathbb R^n$, $n\geq1$, with positive radius is compact. [math:cor-euclidean-closed-balls-and-spheres-are-compact](https://alphabetamath.cc/item/cor-euclidean-closed-balls-and-spheres-are-compact)

[F9] A continuous real-valued function on a nonempty compact metric space is bounded above and below and attains its extrema. [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)

[F10] A nonempty regular level set of a smooth map $P:M^m\to N^n$ is a smooth embedded submanifold of codimension $n$. [math:thm-a-regular-level-set-is-an-embedded-submanifold](https://alphabetamath.cc/item/thm-a-regular-level-set-is-an-embedded-submanifold)

## Justification

**Given:** The supplied data and the existence assumptions in the Definition.

**Goal:** Justify the named quantities and conventions.

1.1 The induced metric and the exterior chart give the components and derivatives appearing in the displayed surface integrals. For each $R>R_0>0$ in the exterior chart, the coordinate sphere $S_R=\{x:|x|=R\}\subset\mathbb R^3$ is nonempty, since $(R,0,0)\in S_R$, and compact by [F8]. To check smooth embeddedness, put $P(x)=(x^1)^2+(x^2)^2+(x^3)^2$. This is a smooth map $\mathbb R^3\to\mathbb R$ and $S_R=P^{-1}(R^2)$. At $x\in S_R$, its differential satisfies $dP_x(x)=2R^2\ne0$, so it is surjective onto $\mathbb R$. Thus $R^2$ is a regular value and [F10] makes $S_R$ a smooth embedded hypersurface. [given, F1, F2, F3, F8, F10, algebra]

2.1 The real function $u_R(x)=(\partial_jh_{ij}-\partial_ih_{jj})x^i/R$ is smooth on a neighborhood of $S_R$, hence continuous on $S_R$. Applying [F9] to $u_R$ on the nonempty compact sphere with its restricted Euclidean metric shows that $u_R$ is bounded above and below, so $\sup_{S_R}|u_R|<\infty$. [F2, F3, F9, step 1.1]

3.1 The finite surface measure in [F6] therefore gives $\int_{S_R}|u_R|\,dS_{\mathrm{eucl}}\leq(\sup_{S_R}|u_R|)\int_{S_R}1\,dS_{\mathrm{eucl}}<\infty$, so each signed surface integral is defined and finite. Their limit is explicitly assumed to exist and equal one; the notation $\Sigma_1$ is a label and does not construct a section or prove convergence. [given, F6, step 1.1, step 2.1]

4.1 The supplied $\sigma=f+i\psi$ is smooth. For each specified real $q$, set $a_q=(1+q)-(1-q)f$ and $b_q=-(1-q)\psi$, so $B_q=a_q+ib_q$ is a uniquely specified smooth complex function. By [F7], $B_q\overline{B_q}=(a_q+ib_q)(a_q-ib_q)=a_q^2+b_q^2=|B_q|^2$. This is a unique smooth nonnegative real function $D_q$. If the separately supplied point $p$ satisfies the stated conditions, evaluation gives the unique real number $d_q$. No strict positivity or existence of a zero of $T$ follows from these definitions. [given, F4, F5, F7, algebra] ∎

## Source notes

The cited article supplies attribution for the mass-one convention and its notation. The justification above uses the supplied data and pointwise operations; it does not use the article as a proof of existence or positivity.

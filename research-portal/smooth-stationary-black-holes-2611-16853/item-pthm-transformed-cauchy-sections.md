---
title: "Lemma 4.1: Cauchy sections and global hyperbolicity"
status: published
research_item: pthm-transformed-cauchy-sections
dependency_level: 24
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pages 23–24, Lemma 4.1 and its proof
      attribution: For positive q, the translated maximal-section interiors are
        spacelike Cauchy hypersurfaces of the transformed exterior; the article
        also states global hyperbolicity.
      hypotheses: The regular stationary vacuum construction, its positive-parameter
        transformed metric, and the maximal section used in Section 4.
      reading_limits: Historical reading note retained from the current source; this
        maintenance revision claims no fresh article or external full-text
        reading. The frozen extracted article text at the cited passage was read
        for attribution. The article is not used as a proof premise.
---

PDF p. 23: ` Lemma 4.1 and proof `; PDF p. 24: ` Lemma 4.1 and proof `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-harrison-one-form](item-def-harrison-one-form)
- [def-harrison-one-form-family](item-def-harrison-one-form-family)
- [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)
- [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive)
- [def-stationary-section-time](item-def-stationary-section-time)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [pthm-complete-maximal-slices](item-pthm-complete-maximal-slices)
- [pthm-adm-temporality](item-pthm-adm-temporality)
- [pthm-causal-finite-time-escape](item-pthm-causal-finite-time-escape)
- [physics:thm-gr-cauchy-surface-implies-globally-hyperbolic](https://alphabetamath.cc/physics/item/thm-gr-cauchy-surface-implies-globally-hyperbolic)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Adopt the regular mass-one stationary vacuum construction, with maximal original exterior section and $T|_S\not\equiv0$, and assume the Axiom of Choice.

Choose the single smooth stationary primitive $W_0$ on $\mathcal E$ and a neighborhood of $S$ supplied by the global one-form construction, with its normalized Ernst potential $\sigma=f+i\psi$, $f=-g(T,T)$, and supplied pole $p\in S$ where $T_p=0$. Put $T^\flat=g(T,\cdot)$, $D_q=|q(1+\sigma)+(1-\sigma)|^2$, $d_q=D_q(p)$, and $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. Use the Harrison metric

$$g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q).$$

For each $q\in(0,1]$, choose a complete smooth spacelike maximal stationary graph section $\Sigma_q$ with boundary $S$ as supplied by the maximal-slice result. Its stationary section time $v_q$ vanishes on its interior and satisfies $T v_q=1$; write $\Sigma_{q,a}^\circ=\{p\in\mathcal E:v_q(p)=a\}$ for $a\in\mathbb R$.

Each $\Sigma_{q,a}^\circ$ is a spacelike Cauchy hypersurface of $(\mathcal E,g_q)$. Every inextendible causal curve has section-time image all of $\mathbb R$ and meets each such section exactly once. Consequently $(\mathcal E,g_q)$ is globally hyperbolic. No corresponding global causal assertion for $g_0$ is claimed.

A causal curve is locally absolutely continuous with nonzero causal velocity almost everywhere, and all curves and causal relations are relative to $\mathcal E$. A Cauchy hypersurface meets every inextendible causal curve exactly once. Global hyperbolicity means strong causality and compact causal diamonds in $\mathcal E$.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-harrison-normalization](item-def-harrison-normalization)

[def-harrison-one-form](item-def-harrison-one-form)

[def-harrison-one-form-family](item-def-harrison-one-form-family)

[pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)

[pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive)

[pthm-complete-maximal-slices](item-pthm-complete-maximal-slices)

[def-stationary-section-time](item-def-stationary-section-time)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

## Facts & Assumptions

[A1] The regular stationary model and mass-one normalization supply the background hypotheses stated above. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-harrison-normalization](item-def-harrison-normalization)

[A2] Work in ZFC, including countable and dependent choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] For each fixed $q\in(0,1]$, the maximal-slice result supplies the stated complete smooth spacelike maximal graph section with boundary $S$. The section-time construction identifies the exterior with the stationary product, defines $v_q$, and identifies its level sets with the stationary translates of the section interior. [pthm-complete-maximal-slices](item-pthm-complete-maximal-slices) [def-stationary-section-time](item-def-stationary-section-time)

[F2] The positive-$q$ ADM result gives a smooth time-oriented Lorentzian metric on the exterior, a positive lapse, and $g_q^{-1}(dv_q,dv_q)<0$; the translated level sets are spacelike. [pthm-adm-temporality](item-pthm-adm-temporality)

[F3] Under the same construction and for the chosen section, the finite-section-time escape result says that every inextendible causal curve has section-time image $\mathbb R$. Its causal curves and endpoints are relative to the exterior. [pthm-causal-finite-time-escape](item-pthm-causal-finite-time-escape) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F4] For a time-oriented smooth Lorentzian four-manifold, the existence of a Cauchy set implies strong causality and compact causal diamonds, assuming countable and dependent choice. [physics:thm-gr-cauchy-surface-implies-globally-hyperbolic](https://alphabetamath.cc/physics/item/thm-gr-cauchy-surface-implies-globally-hyperbolic)

[F5] The global one-form result applies to the regular mass-one vacuum data with original maximal exterior section and $T|_S\not\equiv0$. It supplies the normalized smooth Ernst potential, the pole $p\in S$ with $T_p=0$, and one smooth stationary $W_0$ on the exterior and a neighborhood of $S$, with $dW_0=4((f-1)F+\psi\star_gF)$, $F=\tfrac12dT^\flat$, and $W_0(T)=D_0(p)-D_0$. [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)

[F6] For these normalized data the denominator-positivity result gives $D_q>0$ on $\mathcal E$ for every $q\in[0,1]$. The one-form family defines the displayed $W_q$ and gives $W_q(T)=d_q-D_q$. The Harrison metric definition supplies the displayed tensor formula and its Lorentzian signature whenever the one-form conditions and $D_q>0$ hold. [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive) [def-harrison-one-form-family](item-def-harrison-one-form-family) [def-harrison-one-form](item-def-harrison-one-form) [def-harrison-normalization](item-def-harrison-normalization)

## Proof

**Given:** The construction, choice convention, positive parameter $q$, and chosen section in the Statement.

**Goal:** Establish the Cauchy and global-hyperbolicity conclusions for every real section time.

1.1 Fix $q\in(0,1]$. The hypotheses of the global construction in [F5] are exactly [A1] and the original-section conditions in the Statement, so its normalized potential and $W_0$ exist on the required domain. The family in [F6] is smooth and stationary there. Differentiating its formula using [F5] gives $dW_q=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$, while [F6] gives $W_q(T)=d_q-D_q$. At the supplied pole, $f(p)=0$, hence $d_q=(1+q)^2+(1-q)^2\psi(p)^2>0$. The positivity result applies to the same normalized potential and original maximal mass-one data, giving $D_q>0$ throughout $\mathcal E$. Thus all one-form and domain conditions of the metric definition hold, and its formula defines the smooth stationary Lorentzian $g_q$ on the entire exterior. This is the fixed family used by the section, ADM and escape suppliers. [given, A1, F5, F6, algebra]

2.1 Fix $a\in\mathbb R$. The supplied section and its stationary translates define the smooth level sets of $v_q$ throughout the exterior. The ADM result gives a positive lapse and shows that each such level set is spacelike. In particular, $\Sigma_{q,a}^\circ$ is a spacelike hypersurface. [given, A1, F1, F2, step 1.1]

3.1 Let $\gamma$ be an inextendible future-directed causal curve in the exterior. The negative squared norm in [F2], with the section-time orientation, makes $v_q$ strictly increase along $\gamma$; equivalently, the finite-escape result uses its section-time parametrization. By [F3] its image under $v_q$ is all of $\mathbb R$. Therefore it takes the value $a$ exactly once. Reversing orientation gives the same intersection conclusion for a past-directed curve. By the stated definition, $\Sigma_{q,a}^\circ$ is a Cauchy hypersurface. [F2, F3, step 2.1]

4.1 The exterior is a time-oriented smooth Lorentzian four-manifold, and step 3.1 supplies a Cauchy set. The choice assumptions of [F4] follow from [A2]. Hence [F4] gives strong causality and compact causal diamonds, which is global hyperbolicity in the stated convention. The argument applies to each fixed positive $q$ and makes no assertion at $q=0$. [A2, F2, F4, step 3.1] ∎

## Source notes

The article reference attributes the original claim. The proof fixes the metric through the global primitive, one-form family, denominator positivity and metric definition, then uses the completed section, temporality and escape results and the mathematical Cauchy-set theorem; the article is not used as a prerequisite proof.

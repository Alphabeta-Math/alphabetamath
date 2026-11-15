---
title: Collar barrier against finite section-time boundary arrival
status: published
research_item: lem-author-eb8e266b8b92-collar-nonarrival
dependency_level: 3
sources:
  references: []
---

## Prerequisites

- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)
- [math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)
- [math:thm-gronwall-integral-inequality](https://alphabetamath.cc/item/thm-gronwall-integral-inequality)
- [math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)
- [math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)


## Statement

Assume the Axiom of Choice and the stationary ADM setting with causal curves of the section-time speed lemma. Let the spatial slice be the interior of a smooth manifold $\overline S$ with compact boundary $B$. A supplied collar is a diffeomorphism $[0,\epsilon)\times B$ onto a boundary neighborhood; its first coordinate is $\rho$, and $\rho=0$ exactly on $B$. Here diffeomorphism means a bijection that is smooth, with smooth inverse, in boundary charts. Suppose $h$ extends smoothly and positively to the boundary, and in the collar $N\le A\rho$, $|X(\rho)|\le A\rho$, and $|d\rho|_h\le A$, with $A<\infty$. Fix $0<a<\epsilon$ and define $b(x)=\min(\rho(x),a)$ in the collar and $b(x)=a$ outside it. For every causal section-time curve and every two times in its interval, $b(x(v))\ge b(x(v_0))e^{-C|v-v_0|}$, with $C=A^2+A$. Thus no finite section-time endpoint can lie on $B$, including for curves that leave and re-enter the collar.

## Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)

[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)

[math:thm-gronwall-integral-inequality](https://alphabetamath.cc/item/thm-gronwall-integral-inequality)

[math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)

[physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)

[math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)

## Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice implies Dependent Choice and Countable Choice, supplying the choice assumptions of the analytic and smooth-composition suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F2] Every causal curve can use section time; the resulting curve $\gamma(v)=(v,x(v))$ is locally Lipschitz in charts, is future causal, and obeys $|x\prime+X|_h\le N$ almost everywhere. The norms, gradient and vector-field action have the conventions in the ADM supplier. [lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)

[F3] Absolutely continuous scalar functions satisfy the fundamental theorem of calculus. [math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)

[F4] For a continuous nonnegative function satisfying either oriented integral inequality with constant coefficients, Gronwall gives $u(t)\le Ae^{C|t-t_0|}$. [math:thm-gronwall-integral-inequality](https://alphabetamath.cc/item/thm-gronwall-integral-inequality)

[F5] For a locally absolutely continuous future causal curve with nonzero velocity almost everywhere in a time-oriented smooth Lorentzian four-manifold, composition with a smooth map defined on an open set containing the curve image is locally absolutely continuous and satisfies the chain rule almost everywhere. Apply this statement to restrictions of the curve when the map is only locally defined. [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[F6] Cauchy–Schwarz for the inner product $h$ gives $|d\rho(Y)|=|h(\operatorname{grad}_h\rho,Y)|\le|d\rho|_h|Y|_h$ at each point where $\rho$ is defined. [math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)

[F7] Interior points and boundary points of a smooth manifold with boundary are specified by the positive and zero last coordinate, respectively, in a boundary chart; here $S=\operatorname{Int}\overline S$ and $B=\partial\overline S$. [math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)

[F8] Smooth structures with boundary are maximal compatible atlases of boundary charts; maps are smooth when their boundary-chart representatives are smooth in the local-extension sense. The collar and its inverse use these conventions. [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)

## Proof

1.1 Let $U$ be the collar intersected with $S$, an open subset of $S$. The inverse collar map is smooth in boundary charts; taking its first coordinate makes $\rho$ smooth on $U$, so the map $F(v,p)=\rho(p)$ below is smooth. On every section-time subarc whose spatial image lies in $U$, apply smooth composition to $F:\mathbb R\times U\to\mathbb R$, $F(v,p)=\rho(p)$, and the causal curve $\gamma(v)=(v,x(v))$. Then $r=\rho\circ x$ is locally absolutely continuous and $r'=d\rho(x')=d\rho(x'+X)-X(\rho)$ almost everywhere. The pointwise Cauchy–Schwarz inequality and the ADM vector-speed bound therefore give $|r'|\le|d\rho|_h|x'+X|_h+|X(\rho)|\le N|d\rho|_h+|X(\rho)|$. This uses no global extension of $\rho$. [F1, F2, F5, F6, F8, algebra]

2.1 Within a connected time interval on which $\rho<a$, the speed estimate gives $|\rho\prime|\le C\rho$ almost everywhere. On any compact subinterval $[s,t]$ of it, the fundamental theorem gives $\rho(u)\le\rho(t)+C\int_u^t\rho(w)\,dw$ for $s\le u\le t$. The reflected Gronwall inequality yields $\rho(s)\le\rho(t)e^{C(t-s)}$, or $\rho(t)\ge\rho(s)e^{-C(t-s)}$. Applying the forward version gives the same lower bound in the reverse orientation. [F3, F4, step 1.1, given, algebra]

3.1 For $v\ge v_0$, if $\rho(x(v))\ge a$ or $x(v)$ is outside the collar, the asserted bound is immediate since $b(x(v))=a\ge b(x(v_0))$. Otherwise use the connected component of $\{u:\rho(x(u))<a\}$ containing $v$. If the component does not contain $v_0$, its left endpoint $\ell$ satisfies $v_0\le\ell<v$, including the case $\ell=v_0$. Continuity gives $\rho(x(\ell))=a$; pass to that endpoint in the previous lower bound. If the component contains $v_0$, use the value $\rho(x(v_0))$ instead. Both cases give the stated estimate with elapsed time at most $v-v_0$. Reversing the time interval proves the other orientation. The positive resulting lower bound for bounded elapsed time excludes all boundary approaches, even with repeated collar entries. [F2, step 2.1, algebra] ∎

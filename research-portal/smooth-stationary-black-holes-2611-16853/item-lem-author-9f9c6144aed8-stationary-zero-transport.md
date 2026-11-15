---
title: Stationary transport of vanishing from a section
status: draft
research_item: lem-author-9f9c6144aed8-stationary-zero-transport
dependency_level: 3
---

## Prerequisites

- [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af)
- [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)
- [math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains](https://alphabetamath.cc/item/prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains)
- [math:def-smooth-tensor-field](https://alphabetamath.cc/item/def-smooth-tensor-field)
- [math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space)
- [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)
- [math:prop-a-diffeomorphism-pulls-back-tensor-fields-and-forms-isomorphically](https://alphabetamath.cc/item/prop-a-diffeomorphism-pulls-back-tensor-fields-and-forms-isomorphically)
- [math:cor-the-differential-of-a-diffeomorphism-is-an-isomorphism](https://alphabetamath.cc/item/cor-the-differential-of-a-diffeomorphism-is-an-isomorphism)


## Statement

Use the IK AF package, with exterior $E$ and section $\Sigma_0$, and let $\Phi:\mathbb R\times E\to E$ be the complete stationary flow. Let $S$ be a smooth tensor field on $E$ of any fixed type $(r,s)$, where $r,s$ are nonnegative integers, with real or complex values. Use the diffeomorphism pullback specified below, extended to complex values by applying it to the real and imaginary parts. If $\Phi_t^*S=S$ for every real $t$ and $S=0$ on $\Sigma_0\cap E$, then $S=0$ on $E$.

For application to the Mars–Simon tensor, additionally establish or import $E\subseteq N=\{1-\sigma\ne0\}$, where $\sigma$ is the supplied Ernst potential, and establish or import flow invariance of that tensor. Its definition supplies a complex covariant four-tensor only on $N$. Neither domain inclusion nor preservation follows merely from vanishing on the section.

## Statement references

[def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af)

[def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)

[math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains](https://alphabetamath.cc/item/prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains)

[math:def-smooth-tensor-field](https://alphabetamath.cc/item/def-smooth-tensor-field)

[math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space)

[math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

[math:prop-a-diffeomorphism-pulls-back-tensor-fields-and-forms-isomorphically](https://alphabetamath.cc/item/prop-a-diffeomorphism-pulls-back-tensor-fields-and-forms-isomorphically)

[math:cor-the-differential-of-a-diffeomorphism-is-an-isomorphism](https://alphabetamath.cc/item/cor-the-differential-of-a-diffeomorphism-is-an-isomorphism)

## Facts & Assumptions

[F1] Every stationary orbit through $E$ is complete and meets the section. The flow in the Statement is on $E$, so its section intersection lies in $\Sigma_0\cap E$. [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af)

[F2] Each time-$t$ map of a smooth maximal flow is a diffeomorphism between its open domains, with inverse the time-$(-t)$ map. Applied to the complete flow on $E$, these domains are both $E$. [math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains](https://alphabetamath.cc/item/prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains)

[F3] A smooth type-$(r,s)$ tensor field is a smooth section of its tensor bundle; each real fiber tensor is a multilinear map on $r$ cotangent and $s$ tangent arguments. Complex values mean a pair of real tensors, with all constructions applied componentwise. [math:def-smooth-tensor-field](https://alphabetamath.cc/item/def-smooth-tensor-field) [math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space)

[F4] For covariant fields, $(f^*S)_q(v_1,\ldots,v_s)=S_{f(q)}(df_qv_1,\ldots,df_qv_s)$. If $f$ is a diffeomorphism, this pullback has inverse $(f^{-1})^*$. [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field) [math:prop-a-diffeomorphism-pulls-back-tensor-fields-and-forms-isomorphically](https://alphabetamath.cc/item/prop-a-diffeomorphism-pulls-back-tensor-fields-and-forms-isomorphically)

[F5] For a diffeomorphism $f$ the differential $A=df_q$ is a linear isomorphism. The mixed-tensor pullback convention used here is $(f^*S)_q(\alpha_1,\ldots,\alpha_r,v_1,\ldots,v_s)=S_{f(q)}(\alpha_1\circ A^{-1},\ldots,\alpha_r\circ A^{-1},Av_1,\ldots,Av_s)$, where $\alpha_i\in T_q^*E$ and $v_j\in T_qE$. This defines a multilinear tensor and agrees with the covariant construction when $r=0$. [math:cor-the-differential-of-a-diffeomorphism-is-an-isomorphism](https://alphabetamath.cc/item/cor-the-differential-of-a-diffeomorphism-is-an-isomorphism) [math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space)

[F6] The Mars–Simon tensor formula defines a smooth complex covariant four-tensor on the open set $N=\{1-\sigma\ne0\}$; its restriction to all of $E$ therefore requires $E\subseteq N$. [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)

## Proof

**Given:** The flow-invariant real or complex type-$(r,s)$ tensor on $E$ and its vanishing on $\Sigma_0\cap E$.

**Goal:** Show $S_p=0$ for every $p\in E$.

1.1 Each $\Phi_t:E\to E$ is a diffeomorphism with inverse $\Phi_{-t}$. In particular $d\Phi_t|_q:T_qE\to T_{\Phi_t(q)}E$ is a linear isomorphism at every $q\in E$. [given, F2, F5]

1.2 Fix $p\in E$. By the orbit-section assumption, choose $q\in\Sigma_0\cap E$ and $t\in\mathbb R$ such that $p=\Phi_t(q)$. Invariance and section vanishing give $(\Phi_t^*S)_q=S_q=0$. [given, F1, choose]

2.1 Set $A=d\Phi_t|_q$. For arbitrary $\beta_i\in T_p^*E$ and $w_j\in T_pE$, insert $\alpha_i=\beta_i\circ A$ and $v_j=A^{-1}w_j$ into the mixed-pullback formula. It gives $S_p(\beta_1,\ldots,\beta_r,w_1,\ldots,w_s)=(\Phi_t^*S)_q(\beta_1\circ A,\ldots,\beta_r\circ A,A^{-1}w_1,\ldots,A^{-1}w_s)=0$. Thus every evaluation is zero, so $S_p=0$. This also covers $r=0$ with the covariant pullback and its inverse, and $r=s=0$ with empty argument lists. Applying the same argument to the real and imaginary parts proves the complex case. Since $p$ was arbitrary, $S=0$ on $E$. [F3, F4, F5, step 1.1, step 1.2, algebra] ∎

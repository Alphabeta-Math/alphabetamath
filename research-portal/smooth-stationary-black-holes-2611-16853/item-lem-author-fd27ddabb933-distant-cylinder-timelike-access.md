---
title: Timelike transfer supplies access to every sufficiently distant
  stationary cylinder
status: draft
research_item: lem-author-fd27ddabb933-distant-cylinder-timelike-access
dependency_level: 2
---

## Prerequisites

- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:thm-heine-borel-characterisation-r](https://alphabetamath.cc/item/thm-heine-borel-characterisation-r)
- [math:thm-extreme-value-r](https://alphabetamath.cc/item/thm-extreme-value-r)


## Statement

Work in ZFC. Let $(M,g,N,T)$ be smooth stationary Lorentzian data. Supply an open end $U\subset M$ and its chronological exterior $\mathcal E=I^-_{M,g}(U)\cap I^+_{M,g}(U)$. In addition, supply a smooth three-manifold $B$, an open subset $B_\infty\subset B$, and diffeomorphisms $F:\mathbb R\times B\to\mathcal E$ and $e:\{x\in\mathbb R^3:|x|>a\}\to B_\infty$, where $a>0$, with $F_*\partial_t=T$ and $U=F(\mathbb R\times B_\infty)$. Require $T$ to be future $g$-timelike on $U$. These are explicit product-end hypotheses, rather than consequences of stationarity. Put $\pi(F(t,b))=b$ and $\phi_s^T(F(t,b))=F(t+s,b)$ for every $s\in\mathbb R$.

Let $h$ be a smooth time-oriented Lorentzian metric on $\mathcal E$. Assume that every original future $g$-timelike curve $\gamma:[0,1]\to\mathcal E$ has a future $h$-timelike transfer $\widetilde\gamma:[0,1]\to\mathcal E$ with $\widetilde\gamma(0)=\gamma(0)$ and $\pi\circ\widetilde\gamma=\pi\circ\gamma$. Both curve classes use locally absolutely continuous coordinates and nonzero future timelike velocity almost everywhere. The transfer is required on the whole curve, without any continuity requirement on its dependence on $\gamma$.

For $R>a$ define $S_R=\{x:|x|=R\}$, $C_{R,t}=F(\{t\}\times e(S_R))$ and the stationary cylinder $\Gamma_R=\bigcup_{t\in\mathbb R}C_{R,t}$. Every $p\in\mathcal E$ can send a future $h$-timelike curve, entirely in $\mathcal E$, to $\Gamma_R$. If $T$ is future $h$-timelike everywhere on this cylinder, every arrival point $y\in\Gamma_R$ reaches $\phi_s^T(y)$ for every $s>0$. Under this same cylinder hypothesis, every compact source $K\subset\mathcal E$, in particular every compact source surface, has a finite $t_R$ such that for every $t\ge t_R$ and every $p\in K$ there is $y\in C_{R,t}$ with $p\ll_{\mathcal E,h}y$. Thus these conclusions hold at every sufficiently large radius whenever $T$ is future $h$-timelike on a sufficiently distant product tail. No bound on $t_R$ uniform as $R\to\infty$ is asserted.

## Facts & Assumptions

[F1] The exterior is the chronological future and past intersection of the specified original stationary end. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F2] Chronological reachability is open in its endpoints. [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[F3] Stationary Lorentzian data give the smooth metric, its time orientation and the Killing equation. The specified product diffeomorphisms are additional hypotheses. In these coordinates $T=\partial_t$, so the Killing equation gives $\partial_t g_{\mu\nu}=0$ on $U$; the displayed translations define a global flow on $\mathcal E$ and preserve each $\Gamma_R$. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F4] Finite concatenations of future timelike curves remain future timelike; the same curve calculus includes piecewise smooth curves and increasing affine reparametrization. [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[F5] A compact space has a finite subcover for every open cover. The interval $[0,1]$ is compact, and continuous real functions on it attain finite extrema. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) [math:thm-heine-borel-characterisation-r](https://alphabetamath.cc/item/thm-heine-borel-characterisation-r) [math:thm-extreme-value-r](https://alphabetamath.cc/item/thm-extreme-value-r)

[F6] In a Lorentz tangent space the timelike set has two open components. A continuous path of timelike vectors starting in the future component stays there. [physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components)

[A1] Work in ZFC, including the countable and dependent choice required by the causal suppliers. Choice also permits selecting an arrival point for each source point in step 4.1. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The original stationary geometry, the supplied product end and exterior product, and the transfer in the Statement; the future $h$-timelike cylinder hypothesis is used only for later translates and common-time access.

**Goal:** Prove cylinder access, access to every later translate, and a common sufficiently late time for each fixed cylinder and compact source.

1.1 Fix $p\in\mathcal E$ and $R>a$. By [F1] there are $u,q\in U$ with $u\ll_{M,g}p\ll_{M,g}q$. Choose a future $g$-timelike curve from $p$ to $q$. Every interior point $z$ of it satisfies $u\ll_{M,g}p\ll_{M,g}z\ll_{M,g}q$, by restriction and concatenation, so $z\in\mathcal E$. Its endpoints are also in $\mathcal E$, with $q\in U\subset\mathcal E$ by the supplied product. Thus this curve is contained in the transfer domain. Write $q=F(t_0,e(x_0))$. [given, A1, F1, F3, F4, choose]

1.2 Now suppose $T$ is future $h$-timelike everywhere on $\Gamma_R$. For any $y=F(t,b)\in\Gamma_R$ and $s>0$, the curve $v\mapsto F(t+v,b)$, $0\le v\le s$, exists throughout that interval, stays on $\Gamma_R$ and has future $h$-timelike tangent $T$. Thus $y\ll_{\mathcal E,h}\phi_s^T(y)$. The full product, not timelikeness alone, supplies every flow time used here. [given, F3, F4, construct]

2.1 Join $x_0$ to radius $R$ by $\chi(s)=((1-s)+sR/|x_0|)x_0$ for $0\le s\le1$. Its radius lies between $|x_0|$ and $R$, hence stays above $a$. Write $W(s)=\chi'^i(s)\partial_{x^i}$ in the end coordinates. The coefficient functions along $(0,\chi(s))$ are continuous. By [F5] and future timelikeness of $T$ there are $c>0$ and $b\ge0$ with $g(T,T)\le-c$, $|g(T,W)|\le b$ and $|g(W,W)|\le b$ along this path. By [F3] these bounds hold at every stationary time over the same path. Choose $\lambda>0$ so large that $-c+b(2/\lambda+1/\lambda^2)<0$. For every $0\le\varepsilon\le1/\lambda$, $g(T+\varepsilon W,T+\varepsilon W)\le-c+2b\varepsilon+b\varepsilon^2<0$; [F6] puts all these vectors in the future component containing $T$. Therefore $\eta(s)=F(t_0+\lambda s,e(\chi(s)))$ is future $g$-timelike. This proves the required finite end travel directly. The same bounds prove timelike lifting of any fixed smooth finite spatial path with compact parameter interval; finite piecewise smooth paths follow by concatenation. [given, F3, F5, F6, step 1.1, construct, algebra]

3.1 Concatenate the curve from step 1.1 with $\eta$, and reparametrize onto $[0,1]$. By [F4] it is a future $g$-timelike curve in $\mathcal E$. Apply the assumed transfer to this whole curve. Its initial point is $p$, and its final spatial point is $e(\chi(1))\in e(S_R)$, so its endpoint lies on $\Gamma_R$ at a finite product time. This proves access for every $p$ and $R>a$, without needing a global radius on the inner region or a crossing argument there. [given, F3, F4, step 1.1, step 2.1, construct]

4.1 If $K$ is empty the common-time assertion is vacuous. Otherwise choose, for each $p\in K$, an arrival $y_p\in C_{R,t_p}$ from step 3.1. By [F2], $O_p=I^-_{\mathcal E,h}(y_p)$ is an open neighborhood of $p$. The sets $K\cap O_p$ are an open cover in the subspace topology of $K$, so [F5] gives a finite subcover indexed by $p_1,\ldots,p_m$. Put $t_R=1+\max_i t_{p_i}$. For $t\ge t_R$ and $z\in K$, choose $i$ with $z\in O_{p_i}$. Step 1.2 advances $y_{p_i}$ along its cylinder orbit to $F(t,\pi(y_{p_i}))\in C_{R,t}$, and [F4] concatenates that orbit with the curve from $z$ to $y_{p_i}$. This proves the common-time conclusion. Every construction is for fixed $R$; no radius-uniform time estimate has been used. [given, A1, F2, F3, F4, F5, step 3.1, step 1.2, construct] ∎

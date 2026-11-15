---
title: An asymptotically flat stationary end bounds null speed by Killing energy
status: draft
research_item: lem-author-fd27ddabb933-asymptotic-null-energy-speed
dependency_level: 2
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [lem-author-fd27ddabb933-killing-energy-conservation](item-lem-author-fd27ddabb933-killing-energy-conservation)
- [physics:def-time-orientation-and-future-causal-sets](https://alphabetamath.cc/physics/item/def-time-orientation-and-future-causal-sets)
- [physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)


## Statement

Work in ZFC with stationary Lorentzian data $(M,g,N,T)$. Specify the end chart as a diffeomorphism $(t,x):U\longrightarrow I\times\{x\in\mathbb R^3:|x|>R_0\}$, where $I$ is a nonempty open interval, $R_0>0$, and $|\cdot|$ is the Euclidean spatial norm. Put $r=|x|$ and $\eta=\operatorname{diag}(-1,1,1,1)$. Assume that the coordinate metric matrix tends uniformly to $\eta$ as $r\to\infty$, that $T=c\partial_t$ for one fixed $c>0$, and that $T$ has the future orientation of the stationary end. These are supplied chart hypotheses, not consequences of stationarity alone.

For some $R_*>R_0$, every nonzero future null vector $v=a\partial_t+\sum_{i=1}^3w^i\partial_{x^i}$ at a point of $U_*=\{p\in U:r(p)>R_*\}$ has pointwise Killing energy $E(v):=-g(T,v)>0$ and satisfies $|w|\le CE(v)$, with $C=4/c$. Thus along any differentiable future null curve within this region, with parameter $\lambda$ and tangent $v=\dot\gamma$, one has $|dx/d\lambda|\le CE(v)$ and $|dr/d\lambda|\le CE(v)$. If the curve is an affine null geodesic, this energy is constant along its segment.

On $U_*$, $T$ is future timelike and $t$ is temporal: its metric gradient $\nabla t=g^{-1}(dt,\cdot)$ is past-directed timelike. For $t_0\in I$ and $R>R_*$ define the coordinate sphere $S_{t_0,R}$ by the embedding $\omega\mapsto(t_0,R\omega)$ and its stationary cylinder $\mathcal C_R$ by $(s,\omega)\mapsto(s,R\omega)$, where $\omega\in\mathbb S^2:=\{\omega\in\mathbb R^3:|\omega|=1\}$ and $s\in I$, using the inverse chart to view these maps in $M$. The sphere is spacelike, meaning that its induced metric is positive definite, and the cylinder is timelike, meaning that its induced metric has signature $(-,+,+)$. Stationary here means tangent to $T$ and preserved wherever its local flow stays in the chart. No completeness of that flow or of geodesics is required for these pointwise conclusions.

## Facts & Assumptions

[F1] Stationary Lorentzian data give the smooth metric of signature $(-,+,+,+)$, the future timelike orientation field $N$, the Killing field $T$, and the inverse-metric convention; a designated stationary end has future timelike $T$. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] Killing energy is constant along an affine null geodesic segment. This interface is used only for that conservation assertion, not to establish positivity for arbitrary pointwise vectors. [lem-author-fd27ddabb933-killing-energy-conservation](item-lem-author-fd27ddabb933-killing-energy-conservation)

[F3] At each tangent space take the future timelike component to be the one containing $N$; a future null vector is a nonzero null vector in its closure. [physics:def-time-orientation-and-future-causal-sets](https://alphabetamath.cc/physics/item/def-time-orientation-and-future-causal-sets)

[F4] A smooth function is temporal when its metric gradient is past-directed timelike; equivalently for the orientation field $N$, its gradient is timelike and its differential takes a positive value on $N$. [physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity)

[F5] A diffeomorphism is a bijective smooth map with smooth inverse; in particular it is a homeomorphism. [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[F6] A smooth embedding is an injective smooth immersion that is a homeomorphism onto its image with the subspace topology. [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

[A1] The ambient set-theoretic convention is ZFC, including the axiom of choice inherited from the stationary-data and geodesic suppliers. The pointwise matrix argument below makes no additional choice assumption. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The stationary data and exterior product chart specified in the Statement.

**Goal:** Prove the pointwise energy and speed bounds and the geometric assertions on a sufficiently distant sub-end.

1.1 Choose $R_*>R_0$ so that the Euclidean operator norm of $h=g-\eta$ is at most $\varepsilon=1/10$ throughout $U_*$. Write the coordinate matrix as $g=\begin{pmatrix}g_{00}&b^T\\b&H\end{pmatrix}$. Then $H$ is positive definite, since $z^THz\ge(1-\varepsilon)|z|^2$, and $g_{00}\le-1+\varepsilon<0$. In particular $\partial_t$ is timelike and is future because $T=c\partial_t$ has the designated future orientation. Solving the block equations for the inverse gives $g^{00}=(g_{00}-b^TH^{-1}b)^{-1}<0$; hence the smooth vector $\nabla t$ is timelike, with $g(\nabla t,\nabla t)=g^{00}$. [F1, given, choose, algebra]

2.1 No nonzero causal vector can have zero $t$ component: otherwise the positive definiteness of $H$ would give positive norm. Consequently $dt$ never vanishes on the timelike cone. On its connected future component it is positive, since $dt(T)=c>0$; in particular $dt(N)>0$. On the closure of that component it is nonnegative by continuity, and on a nonzero future null vector it cannot be zero, so its time component $a$ is strictly positive. Thus $g(\nabla t,N)=dt(N)>0$, which makes the timelike gradient past-directed and proves that $t$ is temporal. [F1, F3, F4, step 1.1]

2.2 The displayed maps for the sphere and cylinder are smooth embeddings in the supplied product chart. At $x=R\omega$, their spatial tangent plane is $P=\{z\in\mathbb R^3:z\cdot\omega=0\}$. Its induced metric is the positive definite restriction of $H$, proving that the sphere is spacelike. The cylinder tangent space is $\mathbb R\partial_t\oplus P$. Positive definiteness on $P$ gives a unique $Y\in P$ with $g(Y,Z)=g(\partial_t,Z)$ for all $Z\in P$. The vector $W=\partial_t-Y$ is orthogonal to $P$, and $g(W,W)=g_{00}-g(Y,Y)<0$. Thus this tangent space has one negative and two positive directions, proving that the cylinder is timelike. The local flow of $T=c\partial_t$ preserves $r=R$ wherever defined in this chart. [F5, F6, given, step 1.1, algebra]

3.1 For a nonzero future null vector write $v=(a,w)$ in these coordinates, where $a>0$ by step 2.1. The null equation and $|h(v,v)|\le\varepsilon(a^2+|w|^2)$ give $(1-\varepsilon)|w|^2\le(1+\varepsilon)a^2$, hence $|w|\le2a$. Moreover $E(v)/c=-g(\partial_t,v)=a-h(\partial_t,v)\ge a-\varepsilon\sqrt{a^2+|w|^2}\ge a(1-\sqrt5/10)\ge a/2>0$. Therefore $|w|\le4E(v)/c$, proving positivity and the pointwise speed estimate without any geodesic premise. [given, step 1.1, step 2.1, algebra]

4.1 Along any differentiable future null curve in $U_*$, $w=dx/d\lambda$ and $dr/d\lambda=(x/r)\cdot w$, so $|dr/d\lambda|\le|w|\le CE(v)$ with $C=4/c$. For an affine null geodesic, [F2] additionally makes this energy constant on its segment. The radius and constants were fixed solely from the given end and $c$; all estimates concern existing vectors or curve segments, with no extension or completeness assertion. Together with steps 1.1, 2.1, 2.2 and 3.1 this proves every conclusion. [F2, step 1.1, step 2.1, step 2.2, step 3.1, algebra] ∎

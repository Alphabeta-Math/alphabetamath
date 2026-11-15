---
title: Sufficiently far stationary end points can be routed to a chosen cylinder
status: published
research_item: lem-author-12a8dba09036-far-end-slow-timelike-routing
dependency_level: 1
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)
- [physics:lem-gr-timelike-fields-define-equal-or-opposite-future-cones](https://alphabetamath.cc/physics/item/lem-gr-timelike-fields-define-equal-or-opposite-future-cones)
- [math:cor-euclidean-spheres-are-path-connected](https://alphabetamath.cc/item/cor-euclidean-spheres-are-path-connected)
- [math:thm-path-connected-implies-connected](https://alphabetamath.cc/item/thm-path-connected-implies-connected)
- [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)
- [math:thm-extreme-value-r](https://alphabetamath.cc/item/thm-extreme-value-r)


## Statement

Let $E=\mathbb R_t\times\{x\in\mathbb R^3:r=|x|>R_0\}$, where $R_0>0$, carry a smooth stationary metric with $T=\partial_t$ and $g_{00}=-1+2M/r+e(x)$. Let $R_a>R_0$ and $C\ge0$ satisfy $|e(x)|\le Cr^{-2}$ for $r\ge R_a$. Choose $R_f\ge\max(R_a,8|M|,2\sqrt C)$ and the future orientation for which $T$ is future at large radius. Then $g(T,T)\le-1/2$ on the far tail $r\ge R_f$. For any fixed cylinder radius $R\ge R_f$, every point of this tail has a smooth future timelike curve in the tail ending on $r=R$ at some finite stationary time. This includes points initially outside that cylinder, for which a crossing argument from the interior would be inapplicable.

## Statement references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

## Facts & Assumptions

[F1] The stationary metric and time-direction conventions are those of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). The asymptotic hypothesis is exactly the displayed bound $|e(x)|\le Cr^{-2}$ for $r\ge R_a$, the $m=0$, $b=2$ case of the decay convention in [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data).

[F2] On the stated product, $\Phi_s(t,x)=(t+s,x)$ is defined for every $s\in\mathbb R$. It is smooth, has identity at $s=0$, has integral curves of $T=\partial_t$ and satisfies the group law, so it is a global flow in the supplied sense. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F3] A smooth curve with everywhere future timelike velocity is a future timelike curve in the supplied curve class, with future direction defined by negative pairing with the time-orientation field $N$. [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[F4] For two smooth timelike fields, the sign of their pairing is constant on each nonempty connected subset. Negative pairing means that the two fields determine the same future cone. [physics:lem-gr-timelike-fields-define-equal-or-opposite-future-cones](https://alphabetamath.cc/physics/item/lem-gr-timelike-fields-define-equal-or-opposite-future-cones)

[F5] The unit sphere $S^2\subset\mathbb R^3$ is path-connected (the $n=3$ case), and every path-connected subset is connected in its subspace topology. [math:cor-euclidean-spheres-are-path-connected](https://alphabetamath.cc/item/cor-euclidean-spheres-are-path-connected) [math:thm-path-connected-implies-connected](https://alphabetamath.cc/item/thm-path-connected-implies-connected)

[F6] The nonempty interval $[0,1]$ is compact, and a continuous real function on a nonempty compact subset of $\mathbb R$ attains finite maximum and minimum values. [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r) [math:thm-extreme-value-r](https://alphabetamath.cc/item/thm-extreme-value-r)

## Proof

**Given:** The stated data and explicit hypotheses.

**Goal:** Establish the asserted conditional conclusion.

1.1 For $r\ge R_f$, the two terms $2|M|/r$ and $C/r^2$ are at most $1/4$, so $g_{00}\le-1/2$. To check connectedness, take any two points $(u,x)$ and $(v,y)$ of the far tail, and put $a=|x|$, $b=|y|$. By [F5], there is a continuous path $\omega:[0,1]\to S^2$ from $x/a$ to $y/b$. The continuous path $s\mapsto((1-s)u+sv,((1-s)a+sb)\omega(s))$ joins these points and stays in the tail because its radius is $(1-s)a+sb\ge R_f$. Thus the nonempty tail is path-connected and hence connected by [F5]. On the open set where $T$ is timelike, apply [F4] to $N$ and $T$ and this connected subset $\mathbb R_t\times\{r\ge R_f\}$. The chosen future direction at large radius fixes the sign as $g(T,N)<0$ on this entire subset; hence $T$ and $N$ determine the same future cone there. [given, F1, F4, F5]

2.1 For a starting point $(t_1,x_1)$ with $r_1=|x_1|\ge R_f$, take $0\le\lambda\le1$ and the smooth radial spatial path $x(\lambda)=(1-\lambda)x_1+\lambda(R/r_1)x_1$. Its radius stays between $r_1$ and $R$, hence in the far tail. Define $b(\lambda)=g_{0i}(t_1,x(\lambda))x'^i(\lambda)$ and $c(\lambda)=g_{ij}(t_1,x(\lambda))x'^i(\lambda)x'^j(\lambda)$. Smoothness makes $b$ and $c$ continuous on $[0,1]$. Applying [F6] to these functions gives finite $B,D\ge0$ such that $|b(\lambda)|\le B$ and $|c(\lambda)|\le D$ throughout this interval; stationarity makes the same bounds valid at every time along this spatial path. Choose a finite $L>\max(1,8B,2\sqrt D)$ and set $t(\lambda)=t_1+L\lambda$. By step 1.1 its tangent has squared norm $L^2g_{00}+2Lb+c\le-L^2/2+2LB+D<0$, since $2LB<L^2/4$ and $D<L^2/4$. Its pairing with $T$ is $Lg_{00}+b\le-L/2+B<0$, so [F4] and step 1.1 make it future directed relative to $N$, and [F3] makes the curve future timelike. The entire curve exists in $E$ because its time factor is $\mathbb R$, as in [F2], and ends on $r=R$ at the finite time $t_1+L$. The path is smooth, including the constant spatial path if already on the cylinder. [F1, F2, F3, F4, F6, step 1.1] ∎

---
title: Null expansions, screen quotients and focal data
status: draft
research_item: def-null-screen-expansion-and-focal-data
dependency_level: 0
---

## Prerequisites

- [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)
- [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)
- [physics:lem-gr-fx-null-focal-boundary-exclusion](https://alphabetamath.cc/physics/item/lem-gr-fx-null-focal-boundary-exclusion)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)


## Definition

Assume the axiom of choice. Let $(M,g,N)$ be a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$, with metric-selected connection $\nabla$. A spacelike two-surface $S$ is a nonempty smooth embedded two-manifold without boundary whose induced metric $\gamma=g|_{TS}$ is positive definite. On an open set $U\subseteq S$, choose smooth future null normal fields $L,K$ with $g(L,K)=-2$. Thus $L$ and $K$ are nonzero, orthogonal to $TS$, null, and future-directed.

For tangent fields $X,Y$ on $U$, the null second fundamental form, expansion, and shear of $L$ are respectively $\chi_L(X,Y)=g(\nabla_XL,Y)$, $\theta_L=\operatorname{tr}_\gamma\chi_L$, and $\widehat\chi_L=\chi_L-\frac12\theta_L\gamma$. Here the derivative of $L$ along $S$ uses the pullback connection and the trace uses the inverse of the positive metric $\gamma$.

Suppose a smooth map $F:U\times J\to M$, with $J$ an open interval containing zero, satisfies $F(p,0)=p$, $\partial_\lambda F(p,0)=L_p$, and has future null affine geodesics $\lambda\mapsto F(p,\lambda)$ as its parameter curves. Write $L=\partial_\lambda F$ along this map and require $g(L,dF(X,0))=0$ for every $X\in T_pU$. The screen at $(p,\lambda)$ is $\mathscr S=L^\perp/\mathbb RL$, equipped with $\bar\gamma([V],[W])=g(V,W)$. Fibers are indexed by the parameter domain, even when distinct branches of $F$ meet.

The normal screen Jacobi map is $A_\lambda:T_pS\to\mathscr S_{(p,\lambda)}$, $A_\lambda X=[dF_{(p,\lambda)}(X,0)]$. A focal instant to $S$ on this generator is a positive $\lambda\in J$ where $A_\lambda$ loses rank; the corresponding image is a focal point. The first focal instant, when one exists, is the least positive focal instant.

On the connected regular interval containing $0$, where $A_\lambda$ is invertible and the induced section metric is positive, let $\mathcal D_L[V]=[D_\lambda V]$ be the screen derivative and set $B=A' A^{-1}$, where the prime is the screen derivative. The optical expansion is $\theta=\operatorname{tr}B$ and the optical shear is $\sigma=B-\frac12\theta\,\mathrm{id}$. At $\lambda=0$ these correspond to $\theta_L$ and $\widehat\chi_L$ under the screen identification.

For comparison, use the following causal-reachability conventions. Future causal and future timelike curves here are locally absolutely continuous curves whose velocities are nonzero and future causal or future timelike, respectively, almost everywhere. A point $q$ belongs to $I^+(p)$ when a future timelike curve on a nondegenerate compact parameter interval joins $p$ to $q$. It belongs to $J^+(p)$ when $q=p$ or such an interval carries a future causal curve joining $p$ to $q$. Put $I^+(S)=\bigcup_{p\in S}I^+(p)$, $J^+(S)=\bigcup_{p\in S}J^+(p)$, and $E^+(S)=J^+(S)\setminus I^+(S)$. When the set of $t\geq0$ in the parameter domain such that the entire segment $F(p,[0,t])$ lies in $E^+(S)$ is nonempty and has a finite supremum $c$ in that domain, call $c$ the future boundary cut parameter of this generator relative to $S$ and $F(p,c)$ its boundary cut point. An intersection of distinct generators means $F(p,\lambda)=F(q,\mu)$ for distinct parameter curves, for example $p\ne q$. These are separate definitions: focal rank loss is local differential data, whereas the cut condition and intersections involve global reachability or multiple branches.

## Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)

[physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)

[physics:lem-gr-fx-null-focal-boundary-exclusion](https://alphabetamath.cc/physics/item/lem-gr-fx-null-focal-boundary-exclusion)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[A1] The axiom of choice implies dependent choice and hence countable choice, supplying the choice assumptions used by the geometric suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice), [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice).

[F1] The null-screen geometry supplier defines the congruence, its screen Jacobi map, focal instants and optical quantities under the stated hypotheses. [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)

[F2] The normal-plane and screen supplier gives local normalized null pairs, the positive screen metric, and well-defined symmetric null second fundamental form and screen derivative. [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)

[F3] Under its stated hypotheses, a focal instant places points sufficiently shortly thereafter in $I^+(S)$. [physics:lem-gr-fx-null-focal-boundary-exclusion](https://alphabetamath.cc/physics/item/lem-gr-fx-null-focal-boundary-exclusion)

## Justification

The supplier for null normal planes supplies local pairs and shows that the form and quotient metric are well-defined; its screen derivative is independent of the representative. The null-screen geometry supplier identifies the initial screen with $T_pS$, makes $A$ invertible on the stated regular interval, and identifies the initial optical data with the surface quantities. The cut parameter is a conditional supremum definition: existence of a finite attained cut is not asserted. The focal-exclusion supplier gives the stated local causal consequence of a focal instant; it does not identify the three notions or assert that a cut or an intersection exists.

---
title: Strict mass positivity from the stationary lapse flux
status: published
research_item: lem-author-d20d145f998f-positive-mass-from-lapse-flux
dependency_level: 6
---

## Prerequisites

- [lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)
- [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in ZFC. Let $(C,h)$ be a connected oriented smooth three-dimensional Riemannian exterior with fixed end chart $x$, $r=|x|$, and compact nonempty smooth boundary $S=\partial C$, in the weighted exterior domain convention. Thus $C_R=C\setminus\{r>R\}$ is compact for all sufficiently large $R$, with boundary $S\sqcup S_R$, where $S_R=\{r=R\}$. This includes the spherical exterior, by which we mean a manifold diffeomorphic to $\{y\in\mathbb R^3:|y|\ge1\}$.

Let $k$ be a smooth symmetric covariant two-tensor on $C$, with $|k|_h^2=h^{ia}h^{jb}k_{ij}k_{ab}$, where $(h^{ij})$ is the inverse metric. Suppose a real smooth function $N$ up to $S$ satisfies $\Delta_hN=|k|_h^2N$, $N|_S=0$, and $N\to1$ uniformly at infinity. Assume in the fixed chart that $N=1-M/r+O_1(r^{-2})$ and $h_{ij}=\delta_{ij}+O_1(r^{-1})$, where $M\in\mathbb R$ and $O_1$ denotes uniform Cartesian bounds through one derivative. Then $M>0$.

The lapse expansion hypothesis follows locally from the following explicit stationary end data. Suppose the end of $C$ is the slice $t=0$ of a smooth time-oriented stationary Lorentzian four-metric $g$ of signature $(-,+,+,+)$, with $T=\partial_t$ future-directed timelike for large $r$, $h_{ij}=g_{ij}$, and $N=-g(T,n)$ for its future unit normal $n$. If $g_{00}=-1+2M/r+O_1(r^{-2})$, $g_{0i}=O_1(r^{-2})$ and $g_{ij}=\delta_{ij}+O_1(r^{-1})$, then $N=(-g^{00})^{-1/2}=1-M/r+O_1(r^{-2})$, where $(g^{ab})$ is the inverse matrix of $(g_{ab})$. In the maximal stationary application $k$ uses the stated hypersurface convention; the lapse equation and boundary conditions above remain explicit hypotheses. This end calculation uses no field equation or assumed mass sign.

## Statement references

[lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)

[math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice; its restriction to countable families supplies the countable-choice hypothesis of the divergence theorem and the choice assumptions inherited by the maximum-principle supplier. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] For a connected smooth Riemannian exterior, a smooth nonnegative potential and zero boundary values with uniform positive end limit, the exterior maximum/Hopf supplier gives strict interior positivity and a strictly positive derivative in the unit normal direction into $C$ at every boundary point. [lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)

[F2] On a compact oriented Riemannian manifold with smooth boundary, the Riemannian divergence theorem applies to every smooth vector field, since its support is compact. The boundary normal is outward. [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)

[F3] The exterior definition supplies a fixed Cartesian end, a compact core, a smooth boundary and the convention $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. Cutting the end at a sufficiently large regular coordinate sphere gives precisely the compact truncation $C_R$. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F4] Use the induced metric, future unit normal, second fundamental form and lapse conventions of the hypersurface definition. The differentiated $O_1$ notation includes angular uniformity and first Cartesian derivative bounds. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

## Proof

**Given:** The complete exterior, regularity, equation, boundary and end hypotheses in the Statement, with [A1].

**Goal:** Prove $M>0$ and derive the stated stationary end lapse expansion from the explicit metric bounds.

1.1 Apply [F1] to $V=|k|_h^2\ge0$. It gives $N>0$ in the interior and $\partial_{\eta_h}N>0$ on $S$, where $\eta_h$ is the unit normal pointing into $C$. On the compact truncation in [F3], the smooth vector field $\operatorname{grad}_hN$ has compact support as a field on $C_R$. The outward normal at its inner boundary is $-\eta_h$. Thus [F2] yields $\int_{S_R}\partial_{\nu_h}N\,dA_h-\int_S\partial_{\eta_h}N\,dA_h=\int_{C_R}|k|_h^2N\,d\mu_h\ge0$. The continuous positive function $\partial_{\eta_h}N$ has a positive minimum on the compact nonempty smooth surface $S$, whose area is positive, so its integral is strictly positive. [given, A1, F1, F2, F3]

1.2 For the stated stationary end application, set $b_i=g_{0i}$ and write $(h^{ij})=(g_{ij})^{-1}$. The identity $h h^{-1}=I$ and its derivative give $h^{-1}=I+O_1(r^{-1})$ and $\partial_\ell h^{-1}=-h^{-1}(\partial_\ell h)h^{-1}$. Thus $D=-g_{00}+h^{ij}b_i b_j=1-2M/r+O_1(r^{-2})>0$ for large $r$. The equations for the zeroth column of the inverse metric are $g_{00}g^{00}+b_i g^{i0}=1$ and $b_jg^{00}+h_{ji}g^{i0}=0$. Substitution gives $g^{00}=(g_{00}-h^{ij}b_i b_j)^{-1}=-D^{-1}$. Let $v=g^{a0}\partial_a$ be the metric dual of $dt$. It is orthogonal to the $t=0$ slice, $g(v,v)=g^{00}<0$, and $g(v,T)=1$. Therefore $n=-v/\sqrt{-g^{00}}$ is its future unit normal: it has negative inner product with the future timelike vector $T$. The lapse definition in [F4] now gives $N=-g(T,n)=(-g^{00})^{-1/2}=\sqrt D$. [given, F4, algebra]

2.1 The end bounds in [F4] give $h^{ij}=\delta^{ij}+O(r^{-1})$. The outward unit normal of $S_R$ has components $\nu_h^i=h^{ij}\partial_jr/(h^{ab}\partial_ar\partial_br)^{1/2}=x^i/R+O(R^{-1})$. Differentiating $N=1-M/r+O_1(r^{-2})$ gives $\partial_iN=Mx^i/r^3+O(r^{-3})$, hence $\partial_{\nu_h}N=M/R^2+O(R^{-3})$. Restricting $h$ to the sphere gives $dA_h=(1+O(R^{-1}))R^2d\omega$, uniformly in angle, with $d\omega$ the unit-sphere area element and $\int d\omega=4\pi$. Consequently $\int_{S_R}\partial_{\nu_h}N\,dA_h=4\pi M+O(R^{-1})$. Taking the limit in step 1.1 gives $4\pi M\ge\int_S\partial_{\eta_h}N\,dA_h>0$, proving $M>0$ without a general positive-mass theorem. [given, F3, F4, step 1.1, algebra]

3.1 Put $u=D-1=-2M/r+O_1(r^{-2})$. Since $D>0$, rationalization gives the exact identity $\sqrt D-1-u/2=-u^2/(2(\sqrt D+1)^2)$. The denominator is at least $2$ and $u=O(r^{-1})$, so $\sqrt D=1+u/2+O(r^{-2})=1-M/r+O(r^{-2})$. Differentiating $\sqrt D$ as $(2\sqrt D)^{-1}\partial_iD$ and using $\partial_iD=2Mx^i/r^3+O(r^{-3})$ gives $\partial_i\sqrt D=Mx^i/r^3+O(r^{-3})$. These uniform bounds prove the full claimed $O_1(r^{-2})$ remainder. Thus the explicit end data supply the lapse expansion used in steps 1.1–1.2 whenever the other stated exterior, equation and boundary hypotheses hold, completing both the abstract flux conclusion and its stationary end application. [given, F4, step 1.2, step 2.1, algebra] ∎

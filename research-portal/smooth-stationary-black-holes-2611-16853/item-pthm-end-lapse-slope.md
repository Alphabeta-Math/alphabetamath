---
title: Uniform asymptotic slope bound
status: draft
research_item: pthm-end-lapse-slope
dependency_level: 12
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 12, Theorem 3.1; page 14, §3.2.1 and equation (3.5)
      statement: The article derives a uniform inverse-square-root radial bound for
        the normalized graph slope from the lapse bound and the normalized end
        metric, and concludes uniform spacelikeness and bounded normals near
        infinity.
      hypotheses: The closedness argument uses candidate maximal sections satisfying
        the conclusion of Theorem 3.1, with parameter bounded below by a fixed
        positive number.
      reading_limits: Read the frozen article text and PDF images at the cited
        passages. This reference attributes the claim; the proof below uses the
        declared suppliers and a local calculation.
---

PDF p. 14: ` §3.2.1, lapse display and (3.5) `

## Prerequisites

- [pthm-positive-transformed-lapse](item-pthm-positive-transformed-lapse)
- [pthm-transformed-end-geometries](item-pthm-transformed-end-geometries)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)
- [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)


## Statement

Fix $\delta\in(0,1)$ and consider a family indexed by $q\in[\delta,1]$ satisfying the hypotheses of the positive transformed-lapse and transformed-end results for each $q$, with the common normalized end estimates of the latter. In particular, each supplied connected smooth spacelike maximal section has compact boundary $S$, one exterior end, and a normalized height $\widetilde u_q$ with $\partial_{x_q}\widetilde u_q\to0$ uniformly in angle as $r_q\to\infty$ for each fixed $q$. The sections and their future normals are oriented as in the lapse supplier. Existence of these sections is assumed.

Assume that their interiors are stationary maximal graphs over the same original section $\Sigma_1^\circ$ in the fixed stationary product $\mathcal E=\mathbb R_t\times\Sigma_1^\circ$, as in the stationary maximal-graph definition. Thus the graph functions $u_q$ are all defined on $\Sigma_1^\circ$, including its fixed Cartesian end $\{x:|x|>R_0\}$, where $R_0>0$ is independent of $q$. This is a hypothesis on the candidate family, not a consequence of the metric estimates or the lapse bound.

Use $t_q=d_qt/(4q)$, $x_q=qx$, $r_q=|x_q|$, and write $u_i=\partial_{x_q^i}\widetilde u_q$. Let $g_q^{\mu\nu}$ be the inverse metric components in these coordinates and set $D=-g_q^{00}+2u_i g_q^{0i}-u_i u_j g_q^{ij}$. Then the stationary lapse $N_q=-g_q(T,n_q)$ is $N_q=(d_q/(4q))D^{-1/2}$ and $D\ge1$. There are constants $R_\delta,C_\delta$ independent of $q$ such that every normalized graph is defined on $r_q\ge R_\delta$ and $|\partial_{x_q}\widetilde u_q|\le C_\delta r_q^{-1/2}$ there. Consequently the graph tangent metrics are uniformly positive definite and the future unit normals have uniformly bounded components in the normalized asymptotic coordinate frame outside that common radius.

## Statement references

[pthm-positive-transformed-lapse](item-pthm-positive-transformed-lapse)

[pthm-transformed-end-geometries](item-pthm-transformed-end-geometries)

[def-stationary-maximal-graph](item-def-stationary-maximal-graph)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

## Facts & Assumptions

[F1] The graph convention defines the fixed stationary product, graph functions on the original section, and normalized height by $\widetilde u_q(qx)=d_qu_q(x)/(4q)$. Spacelikeness means positive definiteness of the induced graph metric. [def-stationary-maximal-graph](item-def-stationary-maximal-graph)

[F2] Under the stated candidate-section hypotheses, $0<N_q\le d_q/(4q)$ and $d_q>0$. [pthm-positive-transformed-lapse](item-pthm-positive-transformed-lapse)

[F3] Uniformly for $q\in[\delta,1]$, the normalized metric has $g_{00}=-1+O(r_q^{-1})$, $g_{0i}=O(r_q^{-2})$, and $g_{ij}=\delta_{ij}+O(r_q^{-1})$ on a common end. The constants in these bounds may depend on $\delta$. [pthm-transformed-end-geometries](item-pthm-transformed-end-geometries)

[F4] The inverse metric is the bilinear form on covectors whose component matrix is the inverse of $(g_{\mu\nu})$. Raising a covector $\alpha$ gives $(\alpha^\sharp)^\mu=g^{\mu\nu}\alpha_\nu$, with $g(\alpha^\sharp,X)=\alpha(X)$. [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[F5] For a smooth spacelike embedded hypersurface in a time-oriented Lorentzian four-manifold, the orthogonal complement of each tangent space is a negative-definite line, and the future unit normal is unique and smooth. Its induced metric is the restriction of the ambient metric to tangent vectors. Only these normal and induced-metric assertions are used, not a sign convention for the second fundamental form. [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

## Proof

**Given:** The family and candidate sections, including the fixed original graph domain, in the Statement.

**Goal:** Establish a common normalized graph domain, the lapse identity, slope estimate, and uniform end geometry.

1.1 By the fixed-domain hypothesis and [F1], the normalized height is defined for $r_q>qR_0$. Since $q\le1$, every graph is therefore defined on $r_q\ge R_0+1$. Intersect this common exterior with the common metric end in [F3] by increasing its radius. No parameter-uniform rate for the individual slope limits is used to obtain this domain. [given, F1, F3, algebra]

1.2 Put $\tau=t_q-\widetilde u_q(x_q)$. The graph tangent vectors are $X_i=\partial_{x_q^i}+u_i\partial_{t_q}$, and the nonzero covector $d\tau$ annihilates each $X_i$. By [F4], its raised vector is a nonzero normal, so [F5] gives $D=-g_q^{-1}(d\tau,d\tau)>0$. The two unit normals are $\pm(d\tau)^\sharp/\sqrt D$. Since $T=(d_q/(4q))\partial_{t_q}$, $d\tau(T)=d_q/(4q)>0$. The supplied future normal has $-g_q(T,n_q)=N_q>0$ by [F2], so it is the negative choice, with metric dual $-d\tau/\sqrt D$. Consequently $N_q=(d_q/(4q))D^{-1/2}$. The upper lapse bound and $d_q>0$ imply $D\ge1$. [given, F1, F2, F4, F5, algebra]

2.1 Inverting the uniformly Minkowskian matrices in [F3] gives $g_q^{00}=-1+O(r_q^{-1})$, $g_q^{0i}=O(r_q^{-2})$, and $g_q^{ij}=\delta^{ij}+O(r_q^{-1})$ uniformly on a common sufficiently distant end. In particular, the spatial inverse block satisfies $g_q^{ij}v_i v_j\ge |v|^2/2$. Writing $v_i=u_i$, step 1.2 therefore gives $|v|^2/2\le C r_q^{-1}+C r_q^{-2}|v|$. Absorbing the last term by $C r_q^{-2}|v|\le |v|^2/4+C' r_q^{-4}$ yields $|v|\le C_\delta r_q^{-1/2}$ after increasing the common radius and constant. By step 1.1 this estimate holds on the entire normalized exterior for every graph. [F3, F4, step 1.1, step 1.2, algebra]

3.1 Evaluating the ambient metric on the tangent vectors $X_i$ gives $h_{ij}=g_{ij}+g_{0i}u_j+g_{0j}u_i+g_{00}u_i u_j$. The bounds in [F3] and step 2.1 make $h_{ij}-\delta_{ij}=O(r_q^{-1})$ uniformly, so its eigenvalues lie, for example, between $1/2$ and $2$ beyond a common larger radius. Also $n_q^\mu=-g_q^{\mu\nu}\partial_\nu\tau/\sqrt D$ by [F4] and step 1.2; the numerator is uniformly bounded by [F3] and step 2.1, and $\sqrt D\ge1$ by step 1.2. Hence the normal components are uniformly bounded there. [F3, F4, F5, step 1.1, step 1.2, step 2.1, algebra] ∎

## Source notes

The article citation attributes the stated estimate and the original fixed-section graph class. The proof uses the declared lapse and end estimates, mathematical inverse-metric and hypersurface-normal suppliers, the explicitly assumed common graph class, and a local calculation. It does not use the article's slope claim as a premise.

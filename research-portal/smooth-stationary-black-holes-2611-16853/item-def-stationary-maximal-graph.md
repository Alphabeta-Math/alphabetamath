---
title: Stationary maximal graphs and normalized graph heights
status: draft
research_item: def-stationary-maximal-graph
dependency_level: 3
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 12, §3, immediately before Theorem 3.1
      statement: The article introduces stationary graphs over the original maximal
        section and their normalized end heights, with estimates allowed to
        depend on a fixed positive lower bound for q.
      hypotheses: The article's stationary product and positive-q Harrison setting;
        the subsequent existence assertion is separate.
      reading_limits: Read the frozen article text at the cited passage. This
        reference attributes the conventions and is not used to establish
        existence or maximality of a graph.
---

PDF p. 12: ` §3, graph definitions before Theorem 3.1 `

## Prerequisites

- [def-harrison-one-form](item-def-harrison-one-form)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)
- [math:prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)


## Definition

Let $\Sigma_1$ be the supplied original smooth spacelike maximal section, with interior $\Sigma_1^\circ$ and compact boundary $S$, and suppose the exterior is identified with the product $\mathcal E=\mathbb R_t\times\Sigma_1^\circ$ by the flow of the stationary field $T=\partial_t$. The coordinate $t$ is the flow parameter and $\Sigma_1^\circ$ is identified with $t=0$. Suppose the Harrison normalization data are supplied on an ambient open set $U$ containing $\mathcal E$ and a chosen point $p\in S$, with $T_p=0$ and $d_q=D_q(p)$. For the parameter in question, suppose a Harrison one-form is supplied on an open subset $V\subseteq U$ with $D_q>0$ and $\mathcal E\subseteq V$, and let $g_q$ be its Lorentzian metric restricted to $\mathcal E$. Thus $d_q$ is evaluated at the ambient boundary point $p$, outside the open product exterior, and is used as a constant on that exterior.

Let $N$ denote the original time-orientation field supplied with the stationary Lorentzian data. Write $A_qv=v+D_q^{-1}W_q(v)T$ for the smooth invertible bundle map in the Harrison construction, so $g_q=(D_q/4)A_q^*g$. We time-orient $g_q$ by declaring a $g_q$-timelike vector $v$ future-directed exactly when $g(A_qv,N)<0$.

For $q\in(0,1]$ and a smooth real function $u_q$ on $\Sigma_1^\circ$, its stationary graph is $\Sigma_q^\circ=\{(u_q(x),x):x\in\Sigma_1^\circ\}$. It is a **stationary maximal graph** when its image is spacelike for $g_q$ and its mean curvature in $g_q$ vanishes. Here spacelike means that the induced metric $h_q$ is positive definite, and mean curvature is $H_q=-\operatorname{tr}_{h_q}k_q$, where $k_q(A,B)=-g_q(\nabla^q_A n_q,B)$ for tangent vectors $A,B$, the future unit normal $n_q$ and the Levi–Civita connection $\nabla^q$ of $g_q$. When a smooth hypersurface with boundary $\Sigma_q$ is separately supplied with interior $\Sigma_q^\circ$ and boundary $S$, we say that the graph has boundary $S$; this condition does not require $u_q$ to extend continuously to $S$.

On the specified Cartesian end, write $r=|x|$ and introduce $t_q=d_qt/(4q)$, $x_q=qx$, and $r_q=|x_q|=qr$. The normalized graph height $\widetilde u_q$ is defined on the rescaled end by $\widetilde u_q(qx)=d_qu_q(x)/(4q)$. The normalization condition is $\widetilde u_q(x_q)\to0$ as $r_q\to\infty$, uniformly in angular direction.

For a fixed $\delta\in(0,1)$, an estimate for a family indexed by $q\in[\delta,1]$ is uniform when its constants and its threshold radius in the stated coordinates can be chosen independently of $q$; they may depend on $\delta$. This convention alone asserts no estimate and gives no uniformity as $\delta\downarrow0$.

## Definition references

[def-harrison-normalization](item-def-harrison-normalization)

[def-harrison-one-form](item-def-harrison-one-form)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

## Facts & Assumptions

[F1] The Harrison normalization defines $D_q=|q(1+\sigma)+(1-\sigma)|^2$, where $\sigma=f+i\psi$ and $f=-g(T,T)$, and defines $d_q=D_q(p)$ at the supplied point where $T_p=0$. [def-harrison-normalization](item-def-harrison-normalization)

[F2] Under its stated positivity and one-form hypotheses, the Harrison construction supplies the Lorentzian metric $g_q$. It supplies the smooth invertible bundle map $A_qv=v+D_q^{-1}W_q(v)T$ and the identity $g_q=(D_q/4)A_q^*g$, with $D_q>0$. [def-harrison-one-form](item-def-harrison-one-form)

[F3] A spacelike hypersurface has a positive-definite induced metric $h_q$; with $k_q(A,B)=-g_q(\nabla^q_A n_q,B)$, its mean curvature is $H_q=-\operatorname{tr}_{h_q}k_q$, and maximality means $H_q=0$. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F4] The end-data convention specifies Cartesian exterior coordinates and distinguishes uniform parameter bounds from separate bounds for each parameter. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F5] A smooth embedding is an injective smooth immersion that is a homeomorphism onto its image equipped with the subspace topology. [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

[F6] The image of a smooth embedding $F:M^m\to P^n$ is an embedded $m$-submanifold of $P$, and the corestriction $F:M\to F(M)$ is a diffeomorphism. [math:prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold)

[F7] The original stationary Lorentzian data include a smooth time-orientation field $N$ with $g(N,N)<0$; a $g$-timelike vector $w$ is future-directed when $g(w,N)<0$. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

## Justification

**Given:** The supplied product, section, Harrison data, positive parameter and graph function in the Definition.

**Goal:** Justify the graph and normalized-height conventions without asserting existence of a maximal section.

1.1 The map $j_q:x\mapsto(u_q(x),x)$ is smooth and injective. Its differential sends a tangent vector $v$ to $(du_q(v),v)$ and is injective because its spatial component is the identity. The product projection is continuous, and its restriction to the image of $j_q$, with the subspace topology, is an inverse of $j_q$. Hence $j_q$ is a homeomorphism onto its image and a smooth immersion, so it is a smooth embedding by [F5]. By [F6], its image, with the smooth structure transported by $j_q$, is a smooth embedded three-dimensional submanifold of the four-dimensional product, hence a hypersurface. Spacelikeness and vanishing mean curvature are explicit conditions on that image; the supplied smooth extension with boundary $S$ is an additional condition. [given, F2, F3, F5, F6]

2.1 Set $Y_q=A_q^{-1}N$. By [F2] and [F7], this is a smooth field with $g_q(Y_q,Y_q)=(D_q/4)g(N,N)<0$. For every $g_q$-timelike vector $v$, the pullback identity gives $g_q(v,Y_q)=(D_q/4)g(A_qv,N)$, so the future convention in the Definition is precisely the time orientation defined by $Y_q$. The spacelike-hypersurface interface therefore supplies a unique smooth future unit normal on every spacelike graph and makes its stated mean curvature well defined. [F2, F3, F7, step 1.1, algebra]

3.1 At the supplied zero of $T$, $f(p)=0$, so $d_q=(1+q)^2+(1-q)^2\psi(p)^2>0$. Since $q>0$, both coordinate scalings are invertible on the end, and substitution of $t=u_q(x)$ gives exactly $t_q=\widetilde u_q(x_q)$. The limit and parameter-uniformity clauses are therefore definite conditions in these coordinates, with the stated dependence of constants. No existence, boundary regularity, or estimate follows merely from the definition. [given, F1, F4, step 1.1, algebra] ∎

## Source notes

The cited article attributes the graph and normalization conventions. The justification uses the declared embedding theorem, the Harrison pullback identity, the original time orientation and local product and coordinate calculations; it does not use the article as a proof of the existence of the graph.

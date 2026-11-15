---
id: lem-author-c50357f4fa9e-expansion-second-jet
title: Outgoing expansion depends smoothly on the second graph data
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-c50357f4fa9e-normal-graph-domain
  - math:def-countable-choice
  - lem-author-c50357f4fa9e-outward-graph-null-gauge
  - physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form
  - physics:def-gr-fx-null-screen-geometry
  - math:thm-fundamental-theorem-of-riemannian-geometry
  - math:thm-chain-rule-for-differentials-of-smooth-maps
  - physics:def-gr-metric-selected-connection
dependency_roles:
  lem-author-c50357f4fa9e-normal-graph-domain: mathematical-premise
  math:def-countable-choice: mathematical-premise
  lem-author-c50357f4fa9e-outward-graph-null-gauge: mathematical-premise
  physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form: mathematical-premise
  physics:def-gr-fx-null-screen-geometry: mathematical-premise
  math:thm-fundamental-theorem-of-riemannian-geometry: mathematical-premise
  math:thm-chain-rule-for-differentials-of-smooth-maps: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Assume countable choice $\mathrm{AC}_\omega$. Use the normal-graph data: a smooth spacelike hypersurface $\Sigma$ in a time-oriented smooth Lorentzian four-manifold, its induced metric $h=g|_{T\Sigma}$, a smooth embedded two-surface $S\subset\operatorname{int}\Sigma$ without boundary with a supplied smooth outward $h$-unit normal $\nu$, and a supplied normal-graph domain $\Omega$ on which $T(p,r)=\exp^h_p(r\nu_p)$ is a diffeomorphism onto its image. A smooth $u$ is admissible when its graph lies in $\Omega$, and $F_u(p)=T(p,u(p))$. The domain may be local; no uniform tube for noncompact $S$ is assumed.

For an admissible graph in the fixed spacelike hypersurface and its canonical gauge, let $q_u=F_u^*h$ and $\Theta(u)=F_u^*(\theta_{L_u})$. The pullback means that each scalar is evaluated at the point $F_u(p)$ and regarded as a function of $p\in S$. Locally there is a smooth scalar function $A$ such that $$\Theta(u)(x)=A(x,u(x),\partial_a u(x),\partial_a\partial_bu(x)).$$ Thus the expansion uses only the **second graph data** (the value, first partials and symmetric second partials at the same point). Its coordinate expressions agree because it is the trace of a geometric tensor. No ambient extension of the normal fields is part of this construction.

More explicitly, choose coordinates $x^a$ on $S$ and $y^i$ on $\Sigma$, with $a,b=1,2$ and $i,j,k,\ell=1,2,3$. Put $E_a^i=\partial_aF_u^i$, write $q_u^{ab}$ for the inverse of $q_{u,ab}=h_{ij}(F_u)E_a^iE_b^j$, let $K(X,Y)=g(\nabla_Xn,Y)$, and let $\Gamma^i{}_{jk}$ be the coefficients of the Levi–Civita connection of $h$. Repeated indices are summed. The exact coordinate formula is
$$\Theta(u)=q_u^{ab}\left(K_{ij}(F_u)E_a^iE_b^j-h_{i\ell}(F_u)\nu_u^\ell\left(\partial_a\partial_bF_u^i+\Gamma^i{}_{jk}(F_u)E_a^jE_b^k\right)\right).$$
Writing $T_r=\partial_rT$ evaluated at $(x,u(x))$, this can equivalently be expressed as
$$\Theta(u)(x)=-q_u^{ab}h(\nu_u,T_r)\partial_a\partial_bu+R(x,u,\partial u),$$
where $R$ is a smooth real function of the first graph data on the coordinate domain. Thus the displayed second-partial term is the only dependence on second derivatives of $u$. At the zero graph, $T_r(p,0)=\nu_p$ and $\nu_0=\nu$, so $h(\nu_0,T_r(p,0))=1$.

## Facts & Assumptions

[F1] [[lem-author-c50357f4fa9e-outward-graph-null-gauge]] supplies the smooth canonical null gauge and first-data dependence of $\nu_u$.

[F2] [[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form]] supplies $K(X,Y)=g(\nabla_Xn,Y)$ on $\Sigma$, with $K$ smooth, and [[math:thm-fundamental-theorem-of-riemannian-geometry]] supplies the Levi–Civita connection $D$ of $h$.

[F3] [[physics:def-gr-fx-null-screen-geometry]] defines $\theta_L$ as the trace of $g(\nabla_XL,Y)$ on the spacelike surface, with tangential extension independence.

[F4] [[math:thm-chain-rule-for-differentials-of-smooth-maps]] supplies differentiation of composites.

[F5] [[lem-author-c50357f4fa9e-normal-graph-domain]] supplies the normal-graph domain $\Omega$, the smooth diffeomorphism $T$, admissibility, and the embedded spacelike parametrization $F_u(p)=T(p,u(p))$, under the stated countable-choice hypothesis.

[F6] Adopt countable choice $\mathrm{AC}_\omega$ in the sense of [[math:def-countable-choice]]. This is the hypothesis inherited by the graph construction in [F5] and the smooth Lorentzian and screen conventions in [F3]; no stronger choice principle is assumed.

[F7] [[physics:def-gr-metric-selected-connection]], clauses (a)–(d), defines and constructs the ambient metric-selected connection $\nabla$: it is $g$-compatible and torsion-free, with $X(g(Y,Z))=g(\nabla_XY,Z)+g(Y,\nabla_XZ)$ and $\nabla_XY-\nabla_YX=[X,Y]$. Its countable-choice hypothesis is [F6].

## Proof

[F1] [[lem-author-c50357f4fa9e-outward-graph-null-gauge]] supplies the smooth canonical null gauge and first-data dependence of $\nu_u$.

[F2] [[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form]] supplies $K(X,Y)=g(\nabla_Xn,Y)$ on $\Sigma$, with $K$ smooth, and [[math:thm-fundamental-theorem-of-riemannian-geometry]] supplies the Levi–Civita connection $D$ of $h$.

[F3] [[physics:def-gr-fx-null-screen-geometry]] defines $\theta_L$ as the trace of $g(\nabla_XL,Y)$ on the spacelike surface, with tangential extension independence.

[F4] [[math:thm-chain-rule-for-differentials-of-smooth-maps]] supplies differentiation of composites.

[F5] [[lem-author-c50357f4fa9e-normal-graph-domain]] supplies the normal-graph domain $\Omega$, the smooth diffeomorphism $T$, admissibility, and the embedded spacelike parametrization $F_u(p)=T(p,u(p))$, under the stated countable-choice hypothesis.

[F6] Adopt countable choice $\mathrm{AC}_\omega$ in the sense of [[math:def-countable-choice]]. This is the hypothesis inherited by the graph construction in [F5] and the smooth Lorentzian and screen conventions in [F3]; no stronger choice principle is assumed.



**Given:** The normal-graph data and admissible graph from [F5], the canonical gauge from [F1], and the countable-choice assumption in [F6].

**Goal:** Establish the exact expansion formula, its second-partial coefficient and the smooth local second-data expression.

1.1 The assumption in [F6] supplies the inherited countable-choice hypotheses of [F5] and [F3]. In any ambient coordinate chart $y^i$ on $\Sigma$ write $E_a^i=\partial_aF_u^i$ and $q_{ab}=h_{ij}(F_u)E_a^iE_b^j$. The $E_a$ depend smoothly on $(x,u,\partial u)$ by [F4]. Since the graph is an immersion into a Riemannian hypersurface, $\det q>0$; hence the cofactor formula makes $q^{ab}$ a smooth function of those same data. The normal $\nu_u$ has the same dependence by [F1]. Let $\Gamma^i{}_{jk}$ denote the smooth Christoffel coefficients of $D$ in this ambient chart. The connection with coefficients $D$ is the tangential part of the ambient metric connection on $\Sigma$: that projection is metric compatible and torsion free by [F7], hence equals $D$ by uniqueness in [F2]. Consequently, for $X$ tangent to the graph $F_u(S)$ and $Y$ tangent to $\Sigma$ along that graph, $g(\nabla_X\nu_u,Y)=h(D_X\nu_u,Y)$. Both derivatives are pullback covariant derivatives along the graph, so no off-graph values of $\nu_u$ are required. [F1, F2, F3, F4, F5, F6, F7, given, algebra]

2.1 Differentiating $h(\nu_u,E_b)=0$ along the graph using metric compatibility gives $h(D_{E_a}\nu_u,E_b)=-h(\nu_u,D_{E_a}E_b)$. The covariant derivative along the parametrization has components $\partial_a\partial_bF_u^i+\Gamma^i{}_{jk}(F_u)E_a^jE_b^k$. Splitting $L_u=n+\nu_u$ and taking the trace in [F3] therefore gives exactly the coordinate formula in the Statement: $$\Theta(u)=q_u^{ab}\left(K_{ij}(F_u)E_a^iE_b^j-h_{i\ell}(F_u)\nu_u^\ell\left(\partial_a\partial_bF_u^i+\Gamma^i{}_{jk}(F_u)E_a^jE_b^k\right)\right).$$ Here $q_u^{ab}$ is the inverse matrix denoted $q^{ab}$ in step 1.1. All factors other than the displayed second derivatives of $F_u$ depend smoothly only on $(x,u,\partial u)$. [F1, F2, F3, F4, F5, step 1.1, algebra]

3.1 The chain rule for $F_u^i=T^i(x,u(x))$ gives $\partial_a\partial_bF_u^i=T_r^i\partial_a\partial_bu+C_{ab}^i(x,u,\partial u)$, where $C_{ab}^i$ is smooth: differentiating $\partial_bF_u^i=T_b^i+T_r^i\partial_bu$ leaves only derivatives of $T$ and products of first partials of $u$ after removing the displayed second-partial term. Substitution into step 2.1 gives the stated smooth remainder $R$ and coefficient $-q_u^{ab}h(\nu_u,T_r)$. At $u=0$, [F5] gives $T_r(p,0)=\nu_p$, and [F1] gives $\nu_0=\nu$, whose $h$-norm is one. The coefficient pairing is therefore one there. The same formula defines the asserted smooth $A(x,u,\partial u,\partial^2u)$. Derivatives of normal fields occur only along the graph, so [F3] gives extension independence; the trace is a scalar, so its coordinate expressions agree. This proves both the original second-data assertion and the exact formula. [F1, F2, F3, F4, F5, step 1.1, step 2.1, algebra] ∎

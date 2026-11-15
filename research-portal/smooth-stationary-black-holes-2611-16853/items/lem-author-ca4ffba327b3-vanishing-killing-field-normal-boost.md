---
id: lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost
title: A Killing field vanishing on a spacelike surface has a normal boost derivative
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-bifurcate-killing-horizon-data
  - physics:thm-gr-killing-and-on-shell-matter-identities
  - physics:def-gr-metric-selected-connection
  - math:thm-covariant-derivative-along-a-curve-is-independent-of-frame-and-extension
dependency_roles:
  def-bifurcate-killing-horizon-data: mathematical-premise
  physics:thm-gr-killing-and-on-shell-matter-identities: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  math:thm-covariant-derivative-along-a-curve-is-independent-of-frame-and-extension: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Let $K$ be a smooth Killing field vanishing on a smooth embedded spacelike two-surface $S$. At $p\in S$, put $B_p(v)=\nabla_vK$. Then $B_p$ annihilates $T_pS$ and preserves its orthogonal normal plane. In any orthonormal normal basis $(n,\nu)$, with $g(n,n)=-1$ and $g(\nu,\nu)=1$, there is a real scalar $a_p$ such that $B_p(n)=a_p\nu$ and $B_p(\nu)=a_pn$. The coefficient is basis-dependent: reversing either normal basis vector reverses $a_p$. With independently chosen pointwise normal bases, its sign and constancy are not imposed by the hypotheses. This concerns arbitrary pointwise choices and does not assert nonconstancy in a smooth normal frame on a connected component of $S$.

## Statement references

[[def-bifurcate-killing-horizon-data]]

[[physics:thm-gr-killing-and-on-shell-matter-identities]]

[[physics:def-gr-metric-selected-connection]]

## Facts & Assumptions

[F1] On an oriented time-oriented smooth Lorentzian four-manifold with its metric-selected connection, part (a) of the Killing-field theorem identifies $\mathcal L_Kg=0$ with the Killing equation. By metric compatibility this equation reads $g(\nabla_vK,w)+g(v,\nabla_wK)=0$. Only this mathematical characterization is used. [[physics:thm-gr-killing-and-on-shell-matter-identities]] [[physics:def-gr-metric-selected-connection]]

[F2] The ambient conventions are a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$ with its Levi–Civita connection. Spacelike means that the metric induced on $S$ is positive definite; the lemma uses no horizon-existence hypothesis. [[def-bifurcate-killing-horizon-data]] [[physics:def-gr-metric-selected-connection]]

[F3] For a smooth curve $\gamma$ and an ambient smooth field $K$, covariant differentiation of its restriction agrees with the ambient derivative: $D_t(K\circ\gamma)=(\nabla K)_{\gamma(t)}(\dot\gamma(t))$. The derivative of the zero section is zero. [[math:thm-covariant-derivative-along-a-curve-is-independent-of-frame-and-extension]]

## Proof

**Given:** The data and hypotheses in the Statement, with the ambient conventions in [F2].

**Goal:** Establish the normal boost form and the stated dependence on pointwise normal-basis choices.

1.1 Fix $p\in S$ and a coordinate neighborhood $U$ of $p$, oriented by that chart. The restriction $g|_U$ is a smooth Lorentzian metric, the ambient time orientation restricts to $U$, and $\nabla|_U$ is its metric-selected connection because torsion freedom and metric compatibility restrict. The smooth field $K|_U$ satisfies $\mathcal L_{K|_U}(g|_U)=0$, since this identity is local. Thus part (a) in [F1] applies to the oriented time-oriented four-manifold $U$ and gives $g(B_pv,w)+g(v,B_pw)=0$ for all $v,w\in T_pM$. No global orientation is required. [given, F1, F2]

2.1 For any $X\in T_pS$, choose a smooth curve $\gamma:(-\epsilon,\epsilon)\to S\cap U$ with $\gamma(0)=p$ and $\dot\gamma(0)=X$; in a surface chart such a curve is the inverse image of a sufficiently short straight line with the prescribed tangent. Since $K|_S=0$, its restriction $K\circ\gamma$ is the zero section. By [F3], $0=D_t(K\circ\gamma)|_{t=0}=\nabla_XK=B_pX$. If $v\in(T_pS)^\perp$, step 1.1 then gives $g(B_pv,X)=-g(v,B_pX)=0$ for every $X\in T_pS$, so $B_pv\in(T_pS)^\perp$. This proves annihilation of the tangent plane and preservation of the normal plane. [given, F2, F3, step 1.1, construct]

3.1 On that plane the skew-adjoint equation with $(v,w)=(n,n)$ and $(\nu,\nu)$ removes both diagonal coefficients. If $B_pn=a\nu$ and $B_p\nu=bn$, the equation with $(n,\nu)$ reads $a-b=0$. This yields the stated pointwise boost matrix with one real scalar. [step 1.1, step 2.1, algebra]

4.1 Replacing $(n,\nu)$ by $(n,-\nu)$ gives $B_p(n)=-a_p(-\nu)$ and $B_p(-\nu)=-a_p n$, so the new coefficient is $-a_p$. Replacing it by $(-n,\nu)$ likewise gives coefficient $-a_p$. In particular, even keeping $n$ future directed leaves the sign free when the spacelike normal direction is unspecified. [step 3.1, algebra]

5.1 For an explicit example, take $M=\mathbb R^4$ with coordinates $(t,x,y,z)$, metric $g=-dt^2+dx^2+dy^2+dz^2$, future direction $\partial_t$, $S=\{t=x=0\}$, and $K=x\partial_t+t\partial_x$. The Christoffel formula of [[physics:def-gr-metric-selected-connection]] gives zero connection coefficients because the metric components are constant. Thus $\nabla_{\partial_t}K=\partial_x$, $\nabla_{\partial_x}K=\partial_t$ and $\nabla_{\partial_y}K=\nabla_{\partial_z}K=0$; these satisfy the skew-adjoint equation in [F1], so $K$ is Killing. The surface is smooth, embedded and spacelike, and $K|_S=0$. In the smooth normal frame $(\partial_t,\partial_x)$ its coefficient is the constant $1$, while in $(\partial_t,-\partial_x)$ it is the constant $-1$. For independent pointwise choices put $n_p=\partial_t|_p$ and $\nu_p=\epsilon(p)\partial_x|_p$, where $\epsilon(p)=1$ for $y\ge0$ and $\epsilon(p)=-1$ for $y<0$. These are orthonormal normal bases at every point and give $a_p=\epsilon(p)$, which is nonconstant even on this connected $S$. This last basis selection is discontinuous; it demonstrates precisely the arbitrary pointwise scope of the claim, without asserting variation in a smooth coherent frame. [F1, F2, step 3.1, step 4.1, construct, algebra] ∎

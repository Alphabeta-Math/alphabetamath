---
id: lem-author-a4a441da4986-orthogonal-flow-static-product
title: Orthogonal flow coverage gives a global static product and the needed end
  bounds
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-asymptotic-decay-data
  - def-stationary-lorentzian-data
  - physics:def-gr-causal-conditions-and-global-hyperbolicity
  - math:def-local-and-global-flow
  - math:thm-fundamental-theorem-on-flows
  - math:prop-a-vector-field-is-complete-if-and-only-if-its-flow-is-global
  - math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:def-pullback-of-a-covariant-tensor-field
  - math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes
  - math:def-embedded-submanifold-and-slice-chart
  - math:prop-the-inclusion-of-an-embedded-submanifold-is-a-smooth-embedding
  - math:thm-chain-rule-for-differentials-of-smooth-maps
dependency_roles:
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  physics:def-gr-causal-conditions-and-global-hyperbolicity: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  math:prop-a-vector-field-is-complete-if-and-only-if-its-flow-is-global: mathematical-premise
  math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:def-pullback-of-a-covariant-tensor-field: mathematical-premise
  math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  math:prop-the-inclusion-of-an-embedded-submanifold-is-a-smooth-embedding: mathematical-premise
  math:thm-chain-rule-for-differentials-of-smooth-maps: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Suppose a smooth globally hyperbolic stationary exterior $\mathcal E$ has complete Killing field $T$ and a smooth embedded spacelike hypersurface $\Sigma$ which meets each $T$-orbit exactly once, transversely, with $T=Nn$, $N>0$, along $\Sigma$. Here $n$ is its future unit normal, $h$ is its induced metric and $N=-g(T,n)$. Let $\Phi$ be the global flow of $T$. With the product smooth structure on $\mathbb R\times\Sigma$, the map $F(t,p)=\Phi_t(p)$ is a diffeomorphism onto $\mathcal E$ and $F^*g=-N^2dt^2+h$, where $N$ and $h$ are pulled back from $\Sigma$ and hence independent of $t$.

For the end assertion, a stationary asymptotic coordinate chart means a diffeomorphism $\Psi:\Omega\to U\subseteq\mathcal E$, where $\Omega$ is open in $\mathbb R_\tau\times\{x\in\mathbb R^3:|x|>R_0\}$, with $\Psi_*\partial_\tau=T$ and metric components given by functions of $x$ alone. Suppose $\Omega$ contains the graph $\{(u(x),x):|x|>R_0\}$ of a smooth function $u$, this graph parametrizes an end of $\Sigma$ under $\Psi$, and in this chart, writing $r=|x|$, assume $g_{00}=-1+2M_0/r+O_4(r^{-2})$, $g_{0i}=O_4(r^{-2})$, $g_{ij}=\delta_{ij}+O_4(r^{-1})$. Then after a constant shift of $\tau$, $u=O(r^{-1})$, $\partial^ju=O(r^{-1-j})$ for $1\le j\le3$, and $h-\delta=O_2(r^{-1})$, $N=1-M_0/r+O_2(r^{-2})$ in the same spatial chart. Orbit coverage and the supplied graph are hypotheses, not conclusions of local staticity.

## Statement references

[[def-spacelike-maximal-hypersurface-data]]

[[def-stationary-asymptotic-decay-data]]

[[def-stationary-lorentzian-data]]

[[physics:def-gr-causal-conditions-and-global-hyperbolicity]]

[[math:def-local-and-global-flow]]

[[math:thm-fundamental-theorem-on-flows]]

[[math:prop-a-vector-field-is-complete-if-and-only-if-its-flow-is-global]]

[[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure]]

[[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

[[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[[math:def-pullback-of-a-covariant-tensor-field]]

[[math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes]]

[[math:def-embedded-submanifold-and-slice-chart]]

[[math:prop-the-inclusion-of-an-embedded-submanifold-is-a-smooth-embedding]]

[[math:thm-chain-rule-for-differentials-of-smooth-maps]]

## Facts & Assumptions

[F1] Use the spacelike normal, induced metric, lapse, stationary Killing-field and differentiated spatial decay conventions of [[def-spacelike-maximal-hypersurface-data]] [[def-stationary-asymptotic-decay-data]] [[def-stationary-lorentzian-data]].

[F2] Global hyperbolicity includes strong causality: every neighborhood of a point contains a smaller neighborhood which no future causal curve can leave and later re-enter. [[physics:def-gr-causal-conditions-and-global-hyperbolicity]]

[F3] A complete smooth vector field has a smooth global flow, with the group law and time maps inverse to the opposite time maps; use the canonical product smooth structure. [[math:def-local-and-global-flow]] [[math:thm-fundamental-theorem-on-flows]] [[math:prop-a-vector-field-is-complete-if-and-only-if-its-flow-is-global]] [[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure]]

[F4] An invertible differential gives a smooth local inverse; a diffeomorphism is a bijective smooth map with smooth inverse. [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]] [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[F5] Pullback of a covariant tensor evaluates it on the pushed-forward tangent vectors. Vanishing Lie derivative makes that tensor invariant under the flow on its domains. [[math:def-pullback-of-a-covariant-tensor-field]] [[math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes]]

[F6] An embedded submanifold has the smooth structure from restricted slice charts; with this structure its inclusion into the ambient manifold is a smooth embedding. [[math:def-embedded-submanifold-and-slice-chart]] [[math:prop-the-inclusion-of-an-embedded-submanifold-is-a-smooth-embedding]]

[F7] For smooth maps $A$ and $B$ whose composition is defined, $d(B\circ A)_p=dB_{A(p)}\circ dA_p$. [[math:thm-chain-rule-for-differentials-of-smooth-maps]]

## Proof

**Given:** The stationary and spacelike data of [F1], global hyperbolicity in [F2], completeness, unique transverse orbit intersections, orthogonality and the explicitly adapted end chart and graph in the Statement.

**Goal:** Establish the global product and improve the asymptotic graph bounds by orthogonality alone.

1.1 By completeness and [F3], $\Phi:\mathbb R\times\mathcal E\to\mathcal E$ is smooth, $\Phi_{s+t}=\Phi_s\circ\Phi_t$ and $\Phi_t^{-1}=\Phi_{-t}$. Differentiating the group law using [F7] gives $d\Phi_t(T)=T$. Since $\mathcal L_Tg=0$, [F5] gives $\Phi_t^*g=g$. Every point lies on an orbit through $p\in\Sigma$, where $g(T,T)=-N(p)^2<0$. This equality persists along the orbit, so $T$ is nowhere zero and timelike everywhere. It remains future-directed along that orbit by continuity from $T_p=N(p)n_p$. A nonzero period would therefore give a nonconstant closed future timelike curve $\gamma:[0,P]\to\mathcal E$, $P>0$, based at $p$. Choose a point $q\ne p$ on this curve and the open neighborhood $\mathcal E\setminus\{q\}$ of $p$. Strong causality supplies $V$ containing $p$ inside this neighborhood. Since both endpoints of $\gamma$ are in $V$, [F2] forces its whole image into $V$, contradicting its passage through $q$. Thus no orbit has a nonzero period. [given, F1, F2, F3, F5, F7]

2.1 By [F6], the inclusion $i:\Sigma\hookrightarrow\mathcal E$ is a smooth embedding. In the product charts of [F3], the map $(t,p)\mapsto(t,i(p))$ is smooth, so its composition with the smooth global flow gives the smooth map $F(t,p)=\Phi_t(i(p))$. Identifying $T_{(0,p)}(\mathbb R\times\Sigma)$ with $\mathbb R\times T_p\Sigma$, and $T_p\Sigma$ with its image under $di_p$, [F7] gives its differential as $dF_{(0,p)}(a,v)=aT_p+v$, an isomorphism by transversality. The group law and [F7] give $dF_{(t,p)}(a,v)=d\Phi_t|_p(aT_p+v)$, again an isomorphism because $\Phi_t$ is a diffeomorphism. Hence [F4] makes $F$ a local diffeomorphism. Orbit coverage makes it surjective. If $F(t,p)=F(s,q)$, then $p,q\in\Sigma$ lie on the same orbit, so the unique intersection hypothesis gives $p=q$; step 1.1 then gives $t=s$. Thus $F$ is bijective. Its set-theoretic inverse agrees on every local image with the smooth local inverse from [F4], and is therefore smooth everywhere. This proves that $F$ is a diffeomorphism. [given, F1, F3, F4, F6, F7, step 1.1]

3.1 For $v,w\in T_p\Sigma$, the differential formula and the isometry property give $g(dF(\partial_t),dF(\partial_t))=g(T_p,T_p)=-N(p)^2$, $g(dF(\partial_t),dF(0,v))=g(T_p,v)=0$ and $g(dF(0,v),dF(0,w))=h_p(v,w)$. By the pullback definition these are exactly $F^*g=-N^2dt^2+h$, with the coefficients independent of $t$. [given, F1, F3, F5, step 1.1, step 2.1]

4.1 In the end chart use $\tau$ for the original stationary time coordinate, so $T=\partial_\tau$, whereas $t$ denotes the product parameter of $F$. The tangent vectors to the supplied graph are $\partial_i+u_i\partial_\tau$. Their orthogonality to $T$ gives $g_{0i}+g_{00}u_i=0$. For sufficiently large $r$, $-g_{00}\geq1/2$, so $u_i=-g_{0i}/g_{00}$. The given differentiated bounds, the product rule and differentiation of this reciprocal give $\partial^\beta u_i=O(r^{-2-|\beta|})$ for $|\beta|\leq2$. In particular the claimed derivatives of $u$ of orders one through three have the asserted decay. [given, F1, step 3.1]

5.1 The radial derivative bound $|\partial_ru(r\omega)|\leq Cr^{-2}$ is uniform in $\omega\in S^2$. Integration along a ray shows that $L(\omega)=\lim_{r\to\infty}u(r\omega)$ exists and $|u(r\omega)-L(\omega)|\leq C/r$. Any two points on a radius-$r$ sphere can be joined on it by an arc of length at most $\pi r$, so the gradient bound also gives $|u(r\omega)-u(r\omega')|\leq C\pi/r$. Taking the limit shows that all $L(\omega)$ equal one constant $L$. The coordinate shift $\tau\mapsto\tau-L$ therefore gives $u=O(r^{-1})$ without changing the stationary metric components or $T=\partial_\tau$. Finally the induced components are $h_{ij}=g_{ij}+g_{0i}u_j+g_{0j}u_i+g_{00}u_i u_j=\delta_{ij}+O_2(r^{-1})$, because the correction terms are $O_2(r^{-4})$. On the graph, $N^2=-g(T,T)=-g_{00}=1-2M_0/r+O_2(r^{-2})$. The positive square root, differentiated up to order two, yields $N=1-M_0/r+O_2(r^{-2})$. No maximal-graph elliptic regularity theorem is needed for this improvement once orthogonality is already known. [given, F1, step 3.1, step 4.1] ∎

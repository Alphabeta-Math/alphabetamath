---
id: lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency
title: Equal fixed-surface flow heights imply boundary tangency
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:thm-fundamental-theorem-on-flows
  - math:def-embedded-smooth-submanifold-with-boundary
  - math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary
  - math:def-inward-outward-and-boundary-tangent-vectors
  - math:prop-chain-rule-for-smooth-half-space-maps
  - math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains
  - math:def-smooth-collar-of-a-manifold-boundary
  - math:prop-tangent-space-of-the-boundary-is-the-boundary-tangent-hyperplane
  - math:cor-the-differential-of-a-diffeomorphism-is-an-isomorphism
dependency_roles:
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  math:def-embedded-smooth-submanifold-with-boundary: mathematical-premise
  math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary: mathematical-premise
  math:def-inward-outward-and-boundary-tangent-vectors: mathematical-premise
  math:prop-chain-rule-for-smooth-half-space-maps: mathematical-premise
  math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains: mathematical-premise
  math:def-smooth-collar-of-a-manifold-boundary: mathematical-premise
  math:prop-tangent-space-of-the-boundary-is-the-boundary-tangent-hyperplane: mathematical-premise
  math:cor-the-differential-of-a-diffeomorphism-is-an-isomorphism: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $M$ be a smooth four-manifold without boundary, $U\subseteq M$ open, and $K$ a smooth vector field on $U$. Let $C\subseteq U$ be a smooth embedded three-dimensional collar with boundary the smooth surface $S$, and assume $K|_S=0$. Write $\phi:\mathcal D\to U$ for the maximal flow of $K$ on $U$, with open domain $\mathcal D\subseteq\mathbb R\times U$. Let $f,g:C\to\mathbb R$ be smooth up to $S$, with $(h(x),x)\in\mathcal D$ for every $x\in C$ and $h\in\{f,g\}$. Define the variable-time maps directly by $F_h(x)=\phi(h(x),x)$, and suppose both are smooth embeddings up to $S$.

For $p\in S$, let $H_p^+C\subset T_pC$ be the closed inward tangent half-space: in a boundary chart with collar interior $x^3>0$, it is the set of vectors with third coordinate nonnegative, including $T_pS$. Here the exterior tangent side of $F_h(C)$ means $d(F_h)_p(H_p^+C)$, the tangent half-space pointing into the collar image, rather than a choice of ambient normal side.

Both maps fix $S$ pointwise. If $f(p)=g(p)=c$ at $p\in S$, then, using the inclusion $T_pC\subset T_pM$, their differentials satisfy $d(F_f)_p=d(F_g)_p=d(\phi_c)_p|_{T_pC}$. Consequently their images have the same tangent hyperplane at $p$ and the same exterior tangent side. The common differential restricts to the identity on $T_pS$. No equality of $df_p$ and $dg_p$ is required.

## Facts & Assumptions

[F1] A smooth vector field on the boundaryless manifold $U$ has a unique maximal smooth flow on an open domain; its time curves are its unique maximal integral curves. [[math:thm-fundamental-theorem-on-flows]]

[F2] An embedded smooth submanifold with boundary carries a manifold-with-boundary smooth structure whose inclusion is a smooth embedding. [[math:def-embedded-smooth-submanifold-with-boundary]]

[F3] A smooth embedding has injective differential on the full tangent space, including at boundary points, and is a homeomorphism onto its image. [[math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary]]

[F4] In a boundary chart the full tangent space has inward, outward and boundary-tangent vectors distinguished by the sign of the last coordinate; this distinction is chart independent. [[math:def-inward-outward-and-boundary-tangent-vectors]]

[F5] Smooth half-space maps obey the chain rule for their full derivatives at boundary points, as computed from smooth local extensions. [[math:prop-chain-rule-for-smooth-half-space-maps]]

[F6] For the maximal flow on $U$, $U_t=\{x\in U:(t,x)\in\mathcal D\}$ is open and $\phi_t:U_t\to U_{-t}$ is a diffeomorphism with inverse $\phi_{-t}$. [[math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains]]

[F7] The collar assumption uses a smooth boundary collar: a smooth embedding $c:S\times[0,\varepsilon)\to C$ with $c(p,0)=p$ and image an open neighborhood of $S=\partial C$ in $C$; the width may first be a positive smooth function of $p$. [[math:def-smooth-collar-of-a-manifold-boundary]]

[F8] For the boundary inclusion $i:S=\partial C\hookrightarrow C$, $di_p$ identifies $T_pS$ with the boundary-tangent hyperplane of $T_pC$. [[math:prop-tangent-space-of-the-boundary-is-the-boundary-tangent-hyperplane]]

[F9] The differential of a diffeomorphism $F:N\to P$ is a linear isomorphism $dF_p:T_pN\to T_{F(p)}P$ at every point. [[math:cor-the-differential-of-a-diffeomorphism-is-an-isomorphism]]

## Proof

**Given:** The assumptions in the Statement.

**Goal:** Prove boundary fixation, equality of the full tangent maps at equal heights, and equality of their inward image half-spaces.

1.1 For $p\in S$, the constant curve at $p$ is an integral curve of $K$ for every real time, since $K(p)=0$. Uniqueness in [F1] identifies it with the maximal integral curve through $p$. Thus $\phi(t,p)=p$ for all $t\in\mathbb R$, and $F_f|_S=F_g|_S=\operatorname{id}_S$. In particular, the fixed-time flow restricts to the identity on $S$, so its differential on $T_pS$, identified with the boundary-tangent hyperplane by [F8], is the identity. [F1, F2, F5, F8, given]

2.1 Fix $p\in S$ and $h\in\{f,g\}$. The map $x\mapsto(h(x),x)$ takes values in the open set $\mathcal D$; near $(h(p),p)$ this openness permits the usual smooth coordinate differentiation, including a smooth extension across the boundary of $C$. Apply the half-space chain rule to its composition with $\phi$. For every $v\in T_pC$, using the differential of the inclusion into $U$, this gives $d(F_h)_p(v)=d(\phi_{h(p)})_p(v)+K_{\phi(h(p),p)}\,dh_p(v)$. Here $\partial_t\phi(t,x)=K_{\phi(t,x)}$ follows from the integral-curve property of [F1]. Step 1.1 and $K(p)=0$ therefore give $d(F_h)_p(v)=d(\phi_{h(p)})_p(v)$ on the full tangent space, without any condition on $dh_p$. [F1, F2, F3, F5, given, step 1.1, algebra]

3.1 If $f(p)=g(p)=c$, step 2.1 gives equality of the two differentials with the restriction of $d(\phi_c)_p$. Since $(c,p)\in\mathcal D$, [F6] applies on the ambient open set $U_c$; by [F9], this ambient differential is an invertible map $T_pU\to T_pU$. Its restriction to $T_pC$ is injective. The embedding hypotheses and [F2]–[F3] identify $T_pF_h(C)$ with $d(F_h)_p(T_pC)$, so the two image tangent hyperplanes agree. [F2, F3, F6, F9, given, step 2.1]

4.1 By [F4] and [F8], the closed half-space $H_p^+C$ in the Statement is intrinsic to the collar interior. The equal linear maps in step 3.1 carry this same half-space to equal half-spaces in the common tangent hyperplane, precisely the asserted common exterior tangent side. Their restriction to $T_pS$ is the identity by step 1.1. Together with the pointwise boundary fixation in step 1.1, this proves all the conclusions without requiring equality of the height derivatives. [F3, F4, F8, step 1.1, step 2.1, step 3.1] ∎

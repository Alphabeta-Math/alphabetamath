---
id: lem-author-66066dbaeb16-timelike-flow-ordering
title: Ordered timelike flow graphs lie on the corresponding geometric side
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets
  - math:def-embedded-smooth-submanifold-with-boundary
  - math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary
  - math:def-smooth-function-on-a-relatively-open-subset-of-a-half-space
  - math:lem-choice-free-smooth-inverse-function-theorem-in-euclidean-space
  - math:prop-chain-rule-for-smooth-half-space-maps
  - math:thm-fundamental-theorem-on-flows
  - lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency
  - math:cor-mean-value-theorem
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets: mathematical-premise
  math:def-embedded-smooth-submanifold-with-boundary: mathematical-premise
  math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary: mathematical-premise
  math:def-smooth-function-on-a-relatively-open-subset-of-a-half-space: mathematical-premise
  math:lem-choice-free-smooth-inverse-function-theorem-in-euclidean-space: mathematical-premise
  math:prop-chain-rule-for-smooth-half-space-maps: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Let $(M,\gamma,N)$ be a smooth time-oriented Lorentzian four-manifold without boundary, of signature $(-,+,+,+)$. Let $U\subseteq M$ be open, $K$ a smooth vector field on $U$, and $C\subseteq U$ a smooth embedded three-dimensional collar with boundary the smooth surface $S$. Suppose $K|_S=0$. Let $\phi:\mathcal D\to U$ be its maximal flow, with open domain $\mathcal D\subseteq\mathbb R\times U$. Let $f,g:C\to\mathbb R$ be smooth up to $S$, with $(h(x),x)\in\mathcal D$ for every $x\in C$ and $h\in\{f,g\}$. Define the variable-time maps directly by $F_h(x)=\phi(h(x),x)$, and assume these are smooth embeddings up to $S$ whose images have positive definite induced metric on their full three-dimensional tangent spaces, including at $S$. These are the boundary-compatible $K$-flow graphs meant here; transversality of $K$ at $S$ is not required. Assume $K$ is future timelike on the exterior collar saturation $\{\phi(t,x):x\in C\setminus S,\ (t,x)\in\mathcal D\}$, and $f\ge g$.

At an equal-height interior contact $p\in C\setminus S$, or at a boundary point $p\in S$ with $f(p)=g(p)$, the $f$-graph lies on the future side of the $g$-graph in a sufficiently small common scalar-graph neighborhood of $q=F_f(p)=F_g(p)$. More precisely, in ordinary coordinates $(t,z)$ with $\partial_t$ future timelike, the two local images can be written $t=a(z)$ and $t=b(z)$ over a common spatial neighborhood, a half-neighborhood at $S$, with $a\ge b$. The scalar functions $a,b$ are distinct from the flow heights $f,g$. At boundary contact only finite flow intervals near the common time are used; no bound uniform over unbounded times is assumed.

## Facts & Assumptions

[F1] The ambient Lorentzian and future-timelike conventions are mathematical; each future timelike cone is connected. Spacelikeness means positive definiteness of the induced metric, here imposed also on full boundary tangent spaces. [[physics:def-gr-smooth-lorentzian-objects]] [[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]

[F2] An embedded smooth submanifold with boundary has a smooth inclusion, and a smooth embedding has injective differential on the full tangent spaces and is a homeomorphism onto its image. [[math:def-embedded-smooth-submanifold-with-boundary]] [[math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary]]

[F3] Smooth coordinate maps on relatively open half-spaces have smooth Euclidean extensions locally; their full derivatives obey the chain rule at boundary points. [[math:def-smooth-function-on-a-relatively-open-subset-of-a-half-space]] [[math:prop-chain-rule-for-smooth-half-space-maps]]

[F4] A smooth Euclidean map with invertible derivative at a point is a diffeomorphism between suitable open neighborhoods of that point and its image. [[math:lem-choice-free-smooth-inverse-function-theorem-in-euclidean-space]]

[F5] The maximal flow of a smooth vector field is smooth on an open domain, each time fiber is an interval, and its time curves are the unique maximal integral curves. [[math:thm-fundamental-theorem-on-flows]]

[F6] For the variable-time embeddings specified in the Statement, both maps fix $S$. Equal boundary heights give equal differentials, a common tangent hyperplane and the same exterior tangent half-space. [[lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency]]

[F7] A real function continuous on $[a,b]$ and differentiable on $(a,b)$, with $a<b$, satisfies $v(b)-v(a)=v\prime(c)(b-a)$ for some $c\in(a,b)$. [[math:cor-mean-value-theorem]]

## Proof

**Given:** The data and hypotheses in the Statement, and one of its equal-height contacts.

**Goal:** Construct a common scalar-graph neighborhood and prove future-side ordering there.

1.1 Fix a stated contact, and write $c=f(p)=g(p)$ and $q=\phi(c,p)$. At a boundary contact, [F6] applies to exactly the collar, smooth heights, flow domain and variable-time embeddings assumed here. Thus both local images have boundary $S$, pass through $p=q$, and have the same tangent hyperplane and inward image half-space. At an interior contact both images pass through $q$ and have no boundary locally. Their spacelike full tangent spaces contain no nonzero timelike vector. [F1, F2, F6, given]

2.1 Choose ambient coordinates $(t,z^1,z^2,z^3)$ at $q$ whose $\partial_t$ at $q$ is future timelike; a linear change of any chart achieves this. Shrink the chart so $\partial_t$ remains future timelike. Projection $\pi(t,z)=z$ has kernel $\mathbb R\partial_t$, so its derivative restricts to an isomorphism on each of the spacelike three-dimensional tangent spaces at $q$. In local parametrizations of the two images, extend their smooth coordinate maps across the boundary using [F3]. Their differentials still have rank three at the boundary by [F2]. Apply [F4] to the three-dimensional maps obtained by composing these extensions with $\pi$. This expresses the two images as $t=a(z)$ and $t=b(z)$, with smooth extensions of $a,b$ to open spatial neighborhoods. At the boundary their projected boundaries are the same embedded surface $\pi(S)$, since both fix $S$ and $d\pi$ is injective on their tangent spaces. Their projected inward tangent sides agree by step 1.1. To identify the domains, use the spatial coordinates furnished by the first projected parametrization: its boundary is $z^3=0$, and the second projected boundary is this same surface; its interior has $z^3>0$ by the equal inward tangent sides and continuity of the nonzero transverse derivative. After shrinking, both projected image domains are therefore the same half-neighborhood $D$ with $z^3\ge0$. At an interior contact their domains instead contain a common open $D$. This construction uses an ordinary timelike coordinate direction, irrespective of the vanishing of $K$ on $S$. [F1, F2, F3, F4, step 1.1, construct]

3.1 On an ambient neighborhood $W$ of $q$, define $P(t,z)=t-b(z)$ using the smooth extension from step 2.1. Its differential is nonzero, has $dP(\partial_t)=1$, and at $q$ has the spacelike kernel $T_qF_g(C)$. After shrinking $W$, the kernel remains spacelike: its smooth spanning vectors $\partial_{z^i}+\partial_i b\,\partial_t$ have a positive definite Gram matrix at $q$, and positive definiteness persists near $q$. Consequently $dP$ cannot vanish on any timelike vector anywhere in $W$. On each connected future timelike cone it has constant sign, and that sign is positive because it takes value one on $\partial_t$. Thus $dP(V)>0$ for every future timelike $V$ in $W$, including away from the actual half-graph. In particular $P\ge0$ describes its local future side; no $K$-adapted chart or positive value of $dP(K)$ on $S$ is asserted. [F1, step 2.1, algebra]

4.1 Choose a compact interval $J=[c-\varepsilon,c+\varepsilon]$ with $\varepsilon>0$. At a boundary contact the flow fixes $p$ at all times, since the constant curve at $p$ is an integral curve and [F5] gives uniqueness. Thus $J\times\{p\}$ lies in $\mathcal D$ and maps to $q$. At an interior contact choose $\varepsilon$ small enough that $J\times\{p\}\subseteq\mathcal D$ and $\phi(J,p)\subseteq W$, using openness and continuity at $(c,p)$. In either case a finite cover of the compact set $J\times\{p\}$ by product neighborhoods contained in $\mathcal D\cap\phi^{-1}(W)$ gives a neighborhood $V$ of $p$ with $J\times V\subseteq\mathcal D$ and $\phi(J,V)\subseteq W$. Continuity of $f,g$ permits a smaller collar neighborhood on which both heights lie in $J$. Therefore, for every nearby interior base point $x$, its entire flow segment from $g(x)$ to $f(x)$ stays in $W$. No estimate over an unbounded set of times has been used. [F5, F6, step 3.1, given, choose]

5.1 For such an interior $x$, put $v_x(s)=P(\phi(s,x))$. It is smooth on a neighborhood of $[g(x),f(x)]$, and the flow equation and chain rule give $v_x\prime(s)=dP_{\phi(s,x)}(K_{\phi(s,x)})>0$ by the exterior timelikeness hypothesis and step 3.1. Its initial value is zero because $F_g(x)$ lies on $t=b(z)$. If $f(x)>g(x)$, [F7] gives $P(F_f(x))>0$; if they are equal, this value is zero. By continuity, $P(F_f(x))\ge0$ also holds at nearby boundary base points. Restrict the parametrization neighborhoods further so their image patches in step 2.1 come from the base neighborhood just used. Every point $(a(z),z)$ with $z\in D$ consequently has $P=a(z)-b(z)\ge0$. This is the claimed future-side ordering on the common whole or half-neighborhood and proves the conclusion. [F3, F5, F7, step 2.1, step 3.1, step 4.1, given, algebra] ∎

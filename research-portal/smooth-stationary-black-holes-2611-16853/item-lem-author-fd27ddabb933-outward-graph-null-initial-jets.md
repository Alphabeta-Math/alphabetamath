---
title: Small outward normal graphs have controlled inward null initial jets
status: published
research_item: lem-author-fd27ddabb933-outward-graph-null-initial-jets
dependency_level: 3
---

## Prerequisites

- [lem-author-fd27ddabb933-future-horizon-defining-pair](item-lem-author-fd27ddabb933-future-horizon-defining-pair)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)
- [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)
- [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)
- [math:lem-taylor-integral-remainder](https://alphabetamath.cc/item/lem-taylor-integral-remainder)
- [math:thm-the-tangent-bundle-has-a-canonical-smooth-2n-manifold-structure](https://alphabetamath.cc/item/thm-the-tangent-bundle-has-a-canonical-smooth-2n-manifold-structure)


## Statement

Work in ZFC. Use the compact surface $S$, future/outward orthonormal frame $(n,\nu)$, ambient normal tube $\Xi$ with coordinates $(y,u,v)$, defining functions $a=v-u$, $b=v+u$, and exterior wedge $\mathcal E$ of the oriented defining-pair data. Let $\Sigma$ be the supplied smooth spacelike extension of the section side across $S$, with induced metric $h$. For fixed smooth $\phi>0$ on $S$, set $F_\epsilon(y)=\exp^h_y(\epsilon\phi(y)\nu_y)$ and $S_\epsilon=F_\epsilon(S)$. Let $n_\epsilon$ be the future unit normal of $\Sigma$ restricted to $S_\epsilon$, and let $\nu_\epsilon$ be the outward unit graph normal, agreeing with $\nu$ at $\epsilon=0$ and having positive pairing with the increasing graph-tube coordinate direction. Fix
$$L_\epsilon=n_\epsilon+\nu_\epsilon,\qquad V_\epsilon=n_\epsilon-\nu_\epsilon,\qquad \underline L_\epsilon=V_\epsilon/2.$$
These are future null normals, with $g(L_\epsilon,\underline L_\epsilon)=-1$; the inward vector in the following derivative estimates is the unhalved $V_\epsilon$.

For all sufficiently small positive $\epsilon$, $S_\epsilon$ lies in $\mathcal E$. Uniformly for $y\in S$,
$$a(F_\epsilon(y))=\epsilon\phi(y)+O(\epsilon^2),\quad b(F_\epsilon(y))=\epsilon\phi(y)+O(\epsilon^2),$$
$$da(V_\epsilon)=-2+O(\epsilon),\qquad db(V_\epsilon)=O(\epsilon).$$
For some $\epsilon_0>0$, the initial-data maps on $[0,\epsilon_0]\times S$ given by $(\epsilon,y)\mapsto(F_\epsilon(y),V_\epsilon(y))$ and $(\epsilon,y)\mapsto(F_\epsilon(y),\underline L_\epsilon(y))$ into $TM$ are restrictions of smooth maps defined near $[0,\epsilon_0]\times S$ and have compact images, including their values at $\epsilon=0$. Thus both specified inward normalizations give compact smooth parameterized initial-data families.

## Facts & Assumptions

[F1] The oriented defining pair has $a=v-u$, $b=v+u$, $\mathcal E\cap O=\{a>0,b>0\}$, $(\partial_u,\partial_v)=(n,\nu)$ on $S$, $da(n-\nu)=-2$, and $db(n-\nu)=0$. [lem-author-fd27ddabb933-future-horizon-defining-pair](item-lem-author-fd27ddabb933-future-horizon-defining-pair)

[F2] The fixed smooth spacelike section has positive induced metric $h$ and a smooth future unit normal $n$. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F3] The compact Riemannian normal-graph tube supplies admissible $F_\epsilon$ for all sufficiently small $|\epsilon|$, smoothly in $(\epsilon,y)$, with $F_0(y)=y$ and $\partial_\epsilon F_0=\phi\nu$. [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain)

[F4] The outward graph normal is smooth in $(y,u,\partial u)$, equals $\nu$ at the zero graph, and fixes the future null pair $L_u=n+\nu_u$, $\underline L_u=(n-\nu_u)/2$ with pairing $-1$. [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)

[F5] A closed bounded real interval is compact, and the product of two compact topological spaces is compact in the product topology. [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r) [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)

[F6] A continuous image of a compact topological space is compact (claim 1); a continuous real function on a nonempty compact space attains its extrema (claim 2). [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

[F7] For a smooth manifold $M$, countable choice supplies the canonical smooth structure and induced bundle charts on $TM$. [math:thm-the-tangent-bundle-has-a-canonical-smooth-2n-manifold-structure](https://alphabetamath.cc/item/thm-the-tangent-bundle-has-a-canonical-smooth-2n-manifold-structure)

[F8] For a scalar function with continuous derivatives through order $k+1$ on an open interval containing the segment, the order-$k$ Taylor remainder is bounded by $M|\epsilon|^{k+1}/(k+1)!$ when the $(k+1)$st derivative has absolute value at most $M$. We use $k=1$ for positions and $k=0$ for the initial derivative functions. [math:lem-taylor-integral-remainder](https://alphabetamath.cc/item/lem-taylor-integral-remainder)

[A1] Work in ZFC, including the Choice assumptions inherited from the normal-tube, geodesic and tangent-bundle suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The geometric data and assumptions in the Statement.

**Goal:** Prove the uniform defining-function jets and compactness of the specified initial-data families.

1.1 By [F3] and the supplied extension across $S$, choose $\eta>0$ so that $F_\epsilon$ is admissible and takes values in the ambient defining-pair tube for $|\epsilon|<\eta$. For the latter restriction, the inverse image of that open tube under the smooth graph map is open and contains $\{0\}\times S$; finitely many product neighborhoods of the compact zero section give a common parameter interval. Fix $0<\epsilon_0<\eta$ and put $P=[0,\epsilon_0]\times S$, with its product topology. By [F5], $P$ is compact. If $S$ is empty all conclusions are vacuous, so assume $S$ nonempty for extrema below. [F1, F3, F5, given, choose]

2.1 At $\epsilon=0$, the ambient coordinates of $F_0(y)$ are $(y,0,0)$ and [F1], [F3] give $\partial_\epsilon(u\circ F_\epsilon)|_0=0$ and $\partial_\epsilon(v\circ F_\epsilon)|_0=\phi(y)$. The second parameter derivatives of these smooth scalar functions are continuous on compact $P$, so [F6] bounds their absolute values uniformly. Apply [F8] with $k=1$ on each parameter segment to get $u\circ F_\epsilon=O(\epsilon^2)$ and $v\circ F_\epsilon=\epsilon\phi+O(\epsilon^2)$ uniformly on $S$. Adding and subtracting gives the two position estimates. By [F6], $m=\min_S\phi>0$. Thus, after shrinking the positive parameter range, both $a(F_\epsilon(y))$ and $b(F_\epsilon(y))$ are at least $m\epsilon/2$, so [F1] puts $S_\epsilon$ in the exterior. [F1, F3, F6, F8, step 1.1, algebra]

2.2 Apply [F4] to the smooth first graph data $(y,\epsilon\phi,\epsilon\,d\phi)$ and restrict the fixed smooth normal from [F2]. The fields $n_\epsilon,\nu_\epsilon,V_\epsilon$ are jointly smooth, with $V_0=n-\nu$. The gauge and future-null assertions follow from [F4], with $V_\epsilon=2\underline L_\epsilon$. The scalar functions $da_{F_\epsilon(y)}(V_\epsilon(y))$ and $db_{F_\epsilon(y)}(V_\epsilon(y))$ are smooth; at zero they equal $-2$ and $0$ by [F1]. Their first parameter derivatives are continuous and bounded on $P$ by [F6]. The $k=0$ bound of [F8] gives the two uniform $O(\epsilon)$ derivative estimates. [F1, F2, F4, F6, F8, step 1.1, algebra]

3.1 In the induced bundle charts of [F7], each initial-data map has as components the smooth position coordinates of $F_\epsilon$ and the smooth vector components supplied in step 2.2. Hence both maps are smooth on an open parameter interval containing $[0,\epsilon_0]$, and their restrictions to $P$ are continuous. Since $P$ is compact, [F6], claim 1, makes each image compact in $TM$. The maps at $\epsilon=0$ have vectors $n-\nu$ and $(n-\nu)/2$, respectively, so these limiting data are included. This proves the stated compactness for both gauges, together with the estimates of steps 2.1 and 2.2. [F6, F7, A1, step 1.1, step 2.1, step 2.2] ∎

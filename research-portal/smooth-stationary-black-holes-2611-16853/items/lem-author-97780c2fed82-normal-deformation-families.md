---
id: lem-author-97780c2fed82-normal-deformation-families
title: Normal deformation families and an outgoing null gauge
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-97780c2fed82-general-spacelike-surface-data
  - math:thm-the-exponential-domain-is-open-and-the-exponential-map-is-smooth
  - math:def-countable-choice
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:prop-exponential-map-scales-geodesic-time
  - math:def-domain-and-exponential-map-of-a-connection
  - math:def-smooth-embedding
  - math:thm-compactness-under-continuous-maps
dependency_roles:
  def-author-97780c2fed82-general-spacelike-surface-data: mathematical-premise
  math:thm-the-exponential-domain-is-open-and-the-exponential-map-is-smooth: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:prop-exponential-map-scales-geodesic-time: mathematical-premise
  math:def-domain-and-exponential-map-of-a-connection: mathematical-premise
  math:def-smooth-embedding: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Assume Countable Choice. For a surface and null pair as in the general surface interface and a smooth normal field $X$ along it, there is an $\epsilon>0$ and a smooth family of spacelike embeddings $\Phi_t:S\to M$, $|t|<\epsilon$, with $\Phi_0=i$ and $\partial_t\Phi_t|_0=X$. One choice is $\Phi_t(p)=\exp^\nabla_{i(p)}(tX_p)$, where $\exp^\nabla$ is the exponential map of the supplied metric-compatible affine connection $\nabla$; torsion freedom is not required. Smooth outgoing null normal pairs on these surfaces can be chosen with $g(\ell_t,k_t)=-1$ and $(\ell_0,k_0)=(\ell,k)$. Neither a spacelike slice nor a null hypersurface containing the variation is assumed.

## Statement references

[[def-author-97780c2fed82-general-spacelike-surface-data]]

[[math:thm-the-exponential-domain-is-open-and-the-exponential-map-is-smooth]]

[[math:def-countable-choice]]

[[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[[math:prop-exponential-map-scales-geodesic-time]]

[[math:def-domain-and-exponential-map-of-a-connection]]

[[math:def-smooth-embedding]]

## Facts & Assumptions

[F1] The initial surface is compact, spacelike, oriented and has the supplied smooth null pair. [[def-author-97780c2fed82-general-spacelike-surface-data]]

[F2] For the supplied affine connection $\nabla$, write $\mathcal E^\nabla$ for its exponential domain and $\exp^\nabla(v)=\gamma_{p,v}(1)$ for $v\in T_pM$ in that domain. Under Countable Choice, $\mathcal E^\nabla$ is open and contains the zero section, and $\exp^\nabla$ is smooth. No torsion restriction is needed. [[math:def-domain-and-exponential-map-of-a-connection]] [[math:thm-the-exponential-domain-is-open-and-the-exponential-map-is-smooth]] [[math:def-countable-choice]]

[F3] An invertible differential admits a smooth local inverse. [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[F4] Under Countable Choice, for any affine connection, $tv$ lies in the exponential domain exactly when $t$ lies in the maximal interval of the geodesic with initial point $p$ and velocity $v$; on this domain $\exp_p(tv)=\gamma_{p,v}(t)$. [[math:prop-exponential-map-scales-geodesic-time]] [[math:def-countable-choice]]

[F5] A smooth embedding is an injective smooth immersion that is a homeomorphism onto its image with the subspace topology. [[math:def-smooth-embedding]]

[F6] A continuous real-valued function on a nonempty compact space attains its minimum and maximum. A continuous bijection from a compact space to a Hausdorff space is a homeomorphism. Neither assertion requires a choice principle. [[math:thm-compactness-under-continuous-maps]]

## Proof

**Given:**The objects and hypotheses in the Statement.

**Goal:** Establish the assertions and well-definedness stated there.

1.1 Openness of the exponential domain and compactness of $S$ give one interval on which $tX_p$ lies in that domain for all $p$. The smooth exponential map gives a smooth family. By [F4], $\Phi_t(p)=\gamma_{i(p),X_p}(t)$ on that interval, so $\Phi_0(p)=i(p)$ and $\left.\partial_t\Phi_t(p)\right|_{t=0}=X_p$ by the initial data of this geodesic. Choose finitely many coordinate neighborhoods $V_j$ covering $S$ whose closures $K_j=\overline{V_j}$ are compact and contained in larger coordinate neighborhoods $W_j$. To obtain these, take around each point a coordinate ball with closed ball contained in the chart image, pull back a smaller concentric ball, and take a finite subcover by compactness. In the coordinates on $W_j$, put $q_{t,AB}=g(\partial_A\Phi_t,\partial_B\Phi_t)$. On each $K_j$, both $q_{0,11}$ and $\det(q_{0,AB})$ are positive continuous functions and hence have positive minima by [F6]. Continuity on these compact sets, and finiteness of the cover, give a common smaller parameter interval on which $q_{t,11}>0$ and $\det(q_{t,AB})>0$ throughout every $K_j$. These two principal-minor inequalities make the symmetric two-by-two Gram matrix positive definite, so the differential is injective and each deformed surface is spacelike. [F1, F2, F4, F6]

2.1 To check global injectivity, suppose there are $t_j\to0$ and distinct $p_j,q_j$ with $\Phi_{t_j}(p_j)=\Phi_{t_j}(q_j)$. Compactness gives convergent subsequences, and injectivity of $i$ makes their limits a common point $p$. Choose a coordinate projection of an ambient chart to two tangent coordinates whose differential on $di(T_pS)$ is invertible. The map $(t,y)\mapsto(t,\pi\Phi_t(y))$ has invertible differential at $(0,p)$; its local inverse contradicts equality for these pairs once they lie in that neighborhood. Thus $\Phi_t$ is injective for small $t$. By [F6], the continuous bijection $S\to\Phi_t(S)$ is a homeomorphism, since $S$ is compact and $\Phi_t(S)$ is a Hausdorff subspace of $M$; together with the rank condition, this makes $\Phi_t$ an embedding by [F5]. [F1, F3, F5, F6, step 1.1]

3.1 On each deformed surface, subtract from the ambient time-orientation vector $N$ its tangential projection: $U=N-q_t^{AB}g(N,E_A)E_B$, where $E_A=\partial_A\Phi_t$. The tangent term is spacelike and orthogonal to $U$, so $g(U,U)=g(N,N)-|N^\top|^2<0$, and $g(U,N)=g(U,U)<0$. Therefore $n_t=U/\sqrt{-g(U,U)}$ is a smooth future unit normal. The normal plane is Lorentzian. Its orientation from the orientations of $M$ and $S$, together with $n_t$, selects a smooth unit spacelike normal $\nu_t$; its sign is chosen to match the outgoing null ray at $t=0$. This can be computed by ordinary two-vector orthogonalization in each normal-plane chart; uniqueness of the oriented unit vector glues these formulas. Put $\widehat\ell_t=n_t+\nu_t$, $\widehat k_t=(n_t-\nu_t)/2$. [F1, step 1.1, step 2.1]

4.1 The initial outgoing ray agrees with that of $\ell$, so $\ell=a\widehat\ell_0$ for a positive smooth function $a$ on $S$. The normalization then gives $k=a^{-1}\widehat k_0$. Setting $\ell_t=a\widehat\ell_t$ and $k_t=a^{-1}\widehat k_t$, with $a$ constant in the variation parameter, supplies the required pair. All denominators are nonzero, and compactness permits the uniform shrinkings already used. Countable Choice is inherited from the exponential-map interface; no stronger choice is used in this construction. [F1, F2, step 3.1] ∎

---
title: Normal graphs and the nonlinear mean-curvature map
status: draft
research_item: def-normal-graph-and-mean-curvature-data
dependency_level: 0
sources:
  references:
    - title: E. Gourgoulhon, 3+1 Formalism and Bases of Numerical Relativity (2007)
      url: https://arxiv.org/pdf/gr-qc/0703035
      locator: Sections 2.3.1-2.3.2, printed pp. 21-22, equations (2.27)-(2.31);
        section 2.3.4, printed pp. 23-24, equations (2.36), (2.42); section
        2.4.2, printed p. 31, equations (2.74)-(2.77).
      statement: A spacelike hypersurface has positive definite induced metric and a
        normalizable timelike normal direction. Gourgoulhon defines extrinsic
        curvature with the negative sign relative to g(nabla_V n,W); its trace
        equals minus the ambient divergence of a unit normal extension.
      hypotheses: A smooth spacelike hypersurface in a smooth Lorentzian four-manifold
        of signature (-,+,+,+), with smooth unit timelike normal extension for
        the divergence identity.
      reading_limits: Read the cited passages in the PDF text. Their sign convention
        is converted explicitly here. They are not a source for global normal
        smoothness, flow graphs, tubular neighborhoods or Banach-space
        differentiability; the declared library lemma supplies the normal
        interface.
---

## Prerequisites

- [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)
- [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:lem-gr-metric-divergence-and-density-formula](https://alphabetamath.cc/physics/item/lem-gr-metric-divergence-and-density-formula)
- [math:def-trace-of-an-endomorphism](https://alphabetamath.cc/item/def-trace-of-an-endomorphism)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)
- [math:prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [` E. Gourgoulhon, 3+1 Formalism and Bases of Numerical Relativity (2007) · Sections 2.3.1-2.3.2, printed pp. 21-22, equations (2.27)-(2.31); section 2.3.4, printed pp. 23-24, equations (2.36), (2.42); section 2.4.2, printed p. 31, equations (2.74)-(2.77). `](https://arxiv.org/pdf/gr-qc/0703035)


## Definition

Assume the Axiom of Countable Choice $\mathrm{AC}_\omega$ for the inherited tangent-bundle smooth structures used below.

Let $(M,g,N)$ be a time-oriented smooth Lorentzian four-manifold of signature $(-,+,+,+)$, with metric-selected connection $\nabla$, and let $\Sigma\subset M$ be a smooth embedded spacelike hypersurface. Thus $g$ restricts to a positive definite metric on each tangent space of $\Sigma$. Write $n$ for its future-directed unit normal: $g(n,n)=-1$, $g(n,N)<0$, and $g(n,V)=0$ for every $V\in T\Sigma$.

Let $Y$ be a smooth vector field on an open neighborhood $U$ of $\Sigma$, transverse to $\Sigma$, meaning $Y_x\notin T_x\Sigma$ at each $x\in\Sigma$. Let $\phi^Y$ be a local flow of $Y$, with open domain $\mathcal D\subseteq\mathbb R\times U$. For a smooth real function $w$ on $\Sigma$ with $(w(x),x)\in\mathcal D$ for all $x$, put $F_w(x)=\phi^Y(w(x),x)$. When $F_w$ is an embedding and its image $\Sigma_w$ is spacelike, $F_w$ and $\Sigma_w$ are called the flow graph map and flow graph of $w$.

For the normal exponential construction, take a smooth real function $w$ such that $w(x)n_x$ belongs to the exponential map domain at every $x$. Put $E_w(x)=\exp_x(w(x)n_x)$. When $E_w$ is an embedding with spacelike image, it and its image are the normal exponential graph map and normal exponential graph. In a specified normal tubular neighborhood this construction may be restricted to those $w$ for which $(x,w(x))$ lies in the chosen domain of a diffeomorphism $(x,s)\mapsto\exp_x(sn_x)$ onto that neighborhood; the existence of such a neighborhood is not asserted here.

For either admissible graph map $G_w$ above, let $n_w$ be the future unit normal to its image, $h_w$ the metric induced there by $g$, and $K_w(V,W)=g(\nabla_Vn_w,W)$ for tangent vectors. At each image point, let $S_w$ be the shape operator determined by $h_w(S_wV,W)=K_w(V,W)$; write $\operatorname{tr}_{h_w}K_w:=\operatorname{tr}(S_w)$, the basis-independent trace of this tangent-space endomorphism. The mean-curvature map assigns to $w$ the function $\mathcal H(w)=G_w^*(\operatorname{tr}_{h_w}K_w)$ on $\Sigma$. Equivalently, with any local unit timelike extension of $n_w$, this is the pullback of $\operatorname{div}_g n_w$. A graph is maximal when $\mathcal H(w)=0$.

If $S\subseteq\Sigma$ is a prescribed boundary set, the homogeneous Dirichlet condition is $w|_S=0$. It fixes each point of $S$ under either graph map. Boundary regularity, spacelikeness and embedding of a candidate graph, differentiability of $\mathcal H$ between Banach spaces, and representation of other hypersurfaces as such graphs require separate hypotheses.

## Definition references

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:lem-gr-metric-divergence-and-density-formula](https://alphabetamath.cc/physics/item/lem-gr-metric-divergence-and-density-formula)

[math:def-trace-of-an-endomorphism](https://alphabetamath.cc/item/def-trace-of-an-endomorphism)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

[math:prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

## Facts & Assumptions

[F1] A spacelike embedded hypersurface has positive definite induced metric. [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[F2] Its future unit normal is unique and smooth, and its tangential covariant derivative is independent of the chosen local extension. [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[F3] The metric-selected connection is metric-compatible. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F4] The local flow is defined on an open domain and is the identity at time zero. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F5] The exponential map is defined on its stated open domain and maps the zero vector at $x$ to $x$. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F6] For a smooth local vector field $J$, the ambient divergence is the scalar contraction $\operatorname{div}_gJ=\nabla_aJ^a=g^{ab}\nabla_bJ_a$. [physics:lem-gr-metric-divergence-and-density-formula](https://alphabetamath.cc/physics/item/lem-gr-metric-divergence-and-density-formula)

[F7] The trace of a finite-dimensional endomorphism is the sum of the diagonal entries in any basis and is independent of that basis. [math:def-trace-of-an-endomorphism](https://alphabetamath.cc/item/def-trace-of-an-endomorphism)

[F8] The tangent-bundle smooth structures used by the Lorentzian data, connection and exponential-map suppliers carry the inherited assumption $\mathrm{AC}_\omega$. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection) [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

## Justification

The local flow and exponential map give smooth graph maps on their stated domains. The inherited $\mathrm{AC}_\omega$ convention supplies the tangent-bundle smooth structures, including the one used for smooth dependence on the initial vector in the exponential construction. Embedding and spacelikeness are explicit admissibility conditions, so each image is a spacelike embedded hypersurface. [math:prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold) Its unique smooth future normal and extension-independent tangential derivatives give the smooth tensor $K_w$ and its trace; pulling this scalar back by $G_w$ defines $\mathcal H(w)$. In an $h_w$-orthonormal tangent basis, the defining relation for $S_w$ gives $\operatorname{tr}(S_w)=\sum_{i=1}^3h_w(S_we_i,e_i)=\sum_{i=1}^3K_w(e_i,e_i)$; basis independence follows from the endomorphism trace. For a local unit timelike extension of $n_w$, metric compatibility gives $g(\nabla_{n_w}n_w,n_w)=\tfrac12 n_w(g(n_w,n_w))=0$. The divergence contraction formula in a local orthonormal frame consisting of $n_w$ and three tangent unit vectors $e_1,e_2,e_3$ gives $\operatorname{div}_g n_w=-g(\nabla_{n_w}n_w,n_w)+\sum_{i=1}^3g(\nabla_{e_i}n_w,e_i)=\operatorname{tr}_{h_w}K_w$, independent of that unit extension. Finally, the flow and exponential identities at zero imply that $w|_S=0$ fixes $S$ pointwise.

## External input

The declared library normal lemma supplies the unique smooth future unit normal and extension-independent tangential covariant derivative for a spacelike embedded hypersurface. [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

Gourgoulhon's cited equations record the normal and curvature conventions. His extrinsic curvature has the opposite sign from $K_w$ here; his trace-divergence identity agrees after that sign conversion. The local justification above uses the declared mathematical suppliers.

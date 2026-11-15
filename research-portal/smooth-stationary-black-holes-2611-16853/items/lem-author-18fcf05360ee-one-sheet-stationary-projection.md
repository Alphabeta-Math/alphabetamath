---
id: lem-author-18fcf05360ee-one-sheet-stationary-projection
title: A proper stationary projection with the correct end has one sheet
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets
  - lem-author-18fcf05360ee-existing-graph-stationary-projection
  - lem-author-18fcf05360ee-collar-and-end-properness
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - def-normal-graph-and-mean-curvature-data
  - math:def-smooth-embedding
  - math:def-transverse-embedded-submanifolds
  - math:prop-local-graph-characterization-by-transversality-to-vertical-fibres
  - math:thm-compactness-under-continuous-maps
  - math:def-connected-space
  - def-spacelike-maximal-hypersurface-data
dependency_roles:
  math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets: mathematical-premise
  lem-author-18fcf05360ee-existing-graph-stationary-projection: mathematical-premise
  lem-author-18fcf05360ee-collar-and-end-properness: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  math:def-smooth-embedding: mathematical-premise
  math:def-transverse-embedded-submanifolds: mathematical-premise
  math:prop-local-graph-characterization-by-transversality-to-vertical-fibres: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:def-connected-space: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 7
---

## Statement

Let $(M,g)$ be a supplied smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$. Let $C=\{x\in\mathbb R^3:|x|>1\}$, identify $D=\mathbb R_t\times C$ with an open subset of $M$, and set $T=\partial_t$ on $D$. All section extensions and flow graphs below are embedded in $M$, with $g$ smooth on a neighborhood of them, and spacelikeness is relative to $g$. Let $j(x)=(u_*(x),x)$ be a supplied smooth existing stationary graph, with interior $\Sigma_*^\circ=j(C)$ and a smooth spacelike extension $\Sigma_*$ with compact boundary $S$. With $\iota_*:\Sigma_*\hookrightarrow M$ the inclusion, let $h_*=\iota_*^*g$ be the positive-definite induced metric, smooth up to $S$. Let $d_{h_*}$ be the infimum of $h_*$-lengths of piecewise $C^1$ curves in $\Sigma_*$ joining the two points, and put $\rho_*(p)=\inf_{s\in S}d_{h_*}(p,s)$, with the boundary included in these curves. Assume compact annular truncations: removing any sufficiently small boundary collar and any sufficiently far graph end $E_R=j(\{|x|>R\})$ leaves a compact subset of $\Sigma_*^\circ$. These compact-truncation data are supplied hypotheses; no collar geometry is inferred merely from the interior graph formula.

Let $F_w(x)=\phi^Y(w(x),x):\Sigma_*\to\Sigma_w$ be a supplied admissible smooth embedded spacelike flow graph, with $w|_S=0$ and $F_w(\Sigma_*^\circ)\subset D$. Put $\Pi_*(t,x)=j(x)$ and $P=\Pi_*\circ F_w$ on the interiors. Assume the collar-and-end properness hypotheses explicitly: $w$ is small, $|w|\le\epsilon\rho_*$ near $S$, and stationary return to $\Sigma_*^\circ$ exists there with $a\rho_*(x)\le\rho_*(P(x))\le b\rho_*(x)$ for fixed $a,b>0$. The returns of a sufficiently small source boundary collar $U$ stay in a fixed target boundary collar $V$ with bounded spatial radius, meaning $|j^{-1}(p)|\le B$ for all $p\in V$ and some finite $B$. On an exterior end $E_{R_0}$ the continuation field equals $T$. Retain the exact end condition $P(x)=x$ there as an explicit supplied hypothesis.

Suppose $T_p\notin T_p\Sigma_w$ at every $p\in\Sigma_w^\circ$. Then $P:\Sigma_*^\circ\to\Sigma_*^\circ$ is a proper local diffeomorphism and a global diffeomorphism. Consequently the stationary projection $\Pi_*|_{\Sigma_w^\circ}$ is also a global diffeomorphism onto the actual connected existing graph. The one-sheet conclusion uses both the identity end and bounded collar image to supply a one-point fibre, in addition to properness.

## Statement references

[[math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets]]

[[lem-author-18fcf05360ee-existing-graph-stationary-projection]]

[[lem-author-18fcf05360ee-collar-and-end-properness]]

[[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[[def-normal-graph-and-mean-curvature-data]]

[[math:def-smooth-embedding]]

[[math:def-transverse-embedded-submanifolds]]

[[math:prop-local-graph-characterization-by-transversality-to-vertical-fibres]]

[[math:thm-compactness-under-continuous-maps]]

[[math:def-connected-space]]

[[def-spacelike-maximal-hypersurface-data]]

## Facts & Assumptions

[F1] The stationary product and supplied existing graph give a smooth diffeomorphism $j:C\to\Sigma_*^\circ$ and global smooth projection $\Pi_*$. In stationary coordinates based on that graph, $G_*(s,j(x))=(s+u_*(x),x)$, the field $T$ is the vertical translation field. Compact annular truncations are assumed separately in the Statement, so only the unconditional product/projection part of the existing-graph supplier is invoked here. [[lem-author-18fcf05360ee-existing-graph-stationary-projection]]

[F2] Spacelikeness and the induced metric use the supplied ambient Lorentzian metric $g$. The boundary distance convention uses the infimum of lengths of piecewise $C^1$ curves in the full section with its boundary included. [[def-spacelike-maximal-hypersurface-data]] An admissible flow graph is an embedding with its embedded-image smooth structure. A smooth embedding is an injective immersion and a homeomorphism onto its image. On the interiors here the graph map has source and image dimension three. [[def-normal-graph-and-mean-curvature-data]] [[math:def-smooth-embedding]]

[F3] For an admissible small fixed-boundary flow graph, the stated stationary return, comparable boundary distances, identity end and compact annular truncations imply properness of $P$. These are the hypotheses of the collar-and-end supplier, explicitly assumed above. The bounded-radius condition on the target collar is also retained for the one-sheet argument. [[lem-author-18fcf05360ee-collar-and-end-properness]]

[F4] A proper $C^1$ map between nonempty Euclidean open sets of equal dimension, with invertible derivative everywhere and connected target, is surjective and has finite evenly covered fibres. [[math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets]]

[F5] Transversality of embedded submanifolds means that their tangent spaces span the ambient tangent space. An embedded submanifold of $M\times N$ of dimension $\dim M$, transverse to a vertical fibre, is locally a smooth graph over $M$. A smooth map whose differential is an isomorphism has a smooth local inverse. [[math:def-transverse-embedded-submanifolds]] [[math:prop-local-graph-characterization-by-transversality-to-vertical-fibres]] [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[F6] Continuous images of compact sets are compact, and continuous real-valued functions on nonempty compact sets attain finite maxima. Connectedness excludes a partition into two nonempty disjoint open sets. [[math:thm-compactness-under-continuous-maps]] [[math:def-connected-space]]

## Proof

**Given:** The stationary product, supplied sections and flow graph, collar return bounds, compact truncations, identity end and transversality in the Statement.

**Goal:** Prove properness, local invertibility and the one-sheet global diffeomorphism conclusions.

1.1 Use the stationary product coordinates $(x,t-u_*(x))\in C\times\mathbb R$ from [F1]. The projection $\Pi_*$ is $j$ composed with first-coordinate projection, and $T$ spans each vertical fibre's tangent line. Since $\Sigma_w^\circ$ is three-dimensional and $T_p\notin T_p\Sigma_w$, that tangent space and the vertical line span the four-dimensional ambient tangent space. Thus [F5] applies at every point: the continued embedded graph is locally a smooth graph over $C$, and $\Pi_*|_{\Sigma_w^\circ}$ is a local diffeomorphism. By [F2], the differential of $F_w$ into its embedded image is an isomorphism between three-dimensional tangent spaces; [F5] gives local smooth inverses. Since $F_w$ is already a bijection onto its image, these inverses agree, so $F_w:\Sigma_*^\circ\to\Sigma_w^\circ$ is a diffeomorphism. Hence $P$ is a smooth local diffeomorphism. [given, F1, F2, F5]

1.2 Apply [F3] to the explicitly supplied graph, return and compact-truncation data to obtain properness of $P$. Its end restriction $P(x)=x$ on $E_{R_0}$ is the exact end hypothesis in the Statement, also used in [F3]. [given, F3]

2.1 Conjugate by $j$ to obtain $f=j^{-1}\circ P\circ j:C\to C$. It is smooth with invertible differential by step 1.1. It is proper by step 1.2: for compact $L\subset C$, $f^{-1}(L)=j^{-1}(P^{-1}(j(L)))$ is compact, using [F6] for the two continuous coordinate maps. The nonempty Euclidean exterior $C$ is connected, so [F4] supplies surjectivity and finite evenly covered fibres. Their cardinality $n$ is locally constant: on an evenly covered neighborhood every sheet contributes exactly one point to each fibre. Each level set of $n$ and its complement are open; connectedness in [F6] therefore makes $n$ constant. Transporting back by $j$ gives the same assertion for $P$. [F1, F4, F6, step 1.1, step 1.2]

3.1 Shrink the source collar $U$ if necessary so $P(U)\subset V$, and choose $R\ge R_0$ sufficiently large. The middle set $K=\Sigma_*^\circ\setminus(U\cup E_R)$ is compact by the supplied truncation hypothesis. If $K$ is nonempty, the continuous function $p\mapsto|j^{-1}(P(p))|$ has a finite maximum $M$ on $K$ by [F6]; if $K$ is empty take $M=0$. Choose $z\in C$ with $|z|>\max\{B,M,R\}$ and put $y=j(z)$. No preimage of $y$ lies in $U$ or $K$, by the bounds on their images. All preimages therefore lie in $E_R$, where $P$ is the identity by step 1.2; since $y\in E_R$, its fibre is exactly $\{y\}$. The constant fibre cardinality from step 2.1 is consequently one. Thus $P$ is bijective and its smooth local inverses from step 1.1 agree to give a smooth global inverse. Finally $\Pi_*|_{\Sigma_w^\circ}=P\circ F_w^{-1}$ is also a diffeomorphism. [given, F1, F3, F5, F6, step 1.1, step 1.2, step 2.1] ∎

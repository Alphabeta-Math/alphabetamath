---
id: def-spacelike-maximal-hypersurface-data
title: Spacelike sections, maximality and lapse–shift data
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets
  - physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form
  - physics:def-gr-metric-selected-connection
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-riemannian-distance-on-a-connected-manifold
  - math:thm-riemannian-distance-is-a-metric
  - math:def-axiom-of-choice
  - math:def-embedded-smooth-submanifold-with-boundary
  - math:def-cauchy-in-metric
  - math:def-metric-convergence
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets: mathematical-premise
  physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-riemannian-distance-on-a-connected-manifold: mathematical-premise
  math:thm-riemannian-distance-is-a-metric: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-embedded-smooth-submanifold-with-boundary: mathematical-premise
  math:def-cauchy-in-metric: mathematical-premise
  math:def-metric-convergence: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: 3+1 Formalism and Bases of Numerical Relativity
      url: https://luth2.obspm.fr/~luthier/gourgoulhon/pdf/form3p1.pdf
      locator: Section 4.2.2, equations (4.28)–(4.31), p. 56
      statement: In foliation-adapted coordinates the time vector decomposes as the
        lapse times the unit normal plus a tangential shift.
      hypotheses: A spacelike foliation and an adapted time coordinate.
      reading_limits: Read Section 4.2.2, equations (4.28)–(4.31), printed p. 56 (PDF
        page 56). The passage supports lapse–shift terminology and splitting for
        the adapted time vector. The arbitrary-field splitting and
        unit-extension divergence identity are justified locally below; the
        boundary completeness convention is not imported from this passage.
dependency_level: 0
---

## Definition

Let $(M,g)$ be a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$ with its Levi–Civita connection $\nabla$, and let $\Sigma\subset M$ be a smooth embedded spacelike hypersurface: its tangent spaces are three-dimensional and $g$ restricts positively on each of them. Let $n$ be the future-directed unit normal, so $g(n,n)=-1$ and $g(n,U)=0$ for tangent $U$. The induced Riemannian metric is $h(U,V)=g(U,V)$, and we use the second fundamental form convention $k(U,V)=-g(\nabla_U n,V)$.

The mean curvature in this convention is $H=-\operatorname{tr}_h k$, where the trace is contraction with the inverse of $h$. Equivalently, $H=\operatorname{div}_g n$ along $\Sigma$: here the divergence is the trace of $V\mapsto\nabla_V\widetilde n$ for any smooth local unit timelike extension $\widetilde n$ of $n$, satisfying $g(\widetilde n,\widetilde n)=-1$ throughout its ambient neighborhood. Such extensions exist locally by normalization. The hypersurface is **maximal** when $H=0$ everywhere.

For any smooth ambient vector field $T$, its **lapse** along $\Sigma$ is $N=-g(T,n)$ and its **shift** is $X=T-Nn$. Thus $X$ is tangent to $\Sigma$ and $T=Nn+X$. These names impose no sign on $N$.

For the boundary convention, suppose separately that $\overline\Sigma\subset M$ is a connected smooth embedded three-dimensional submanifold with compact boundary, supplied with its manifold-with-boundary smooth structure and smooth inclusion, whose interior is $\Sigma$. Suppose that $g$ restricts to a positive-definite smooth metric $\overline h$ on all tangent spaces of $\overline\Sigma$, including its boundary. Its intrinsic distance is the infimum of $\overline h$-lengths of piecewise $C^1$ curves in $\overline\Sigma$ joining the two points. **Complete up to the compact boundary** means that this metric space, with the boundary included, is complete: every Cauchy sequence converges in $\overline\Sigma$. It does not assert completeness of the interior with its own intrinsic distance. For a disconnected extension, the convention applies separately to each connected component.

## Definition references

[[physics:def-gr-smooth-lorentzian-objects]]

[[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]

[[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form]]

[[physics:def-gr-metric-selected-connection]]

[[math:def-riemannian-metric-and-riemannian-manifold]]

[[math:def-riemannian-distance-on-a-connected-manifold]]

[[math:thm-riemannian-distance-is-a-metric]]

[[math:def-axiom-of-choice]]

[[math:def-embedded-smooth-submanifold-with-boundary]]

[[math:def-cauchy-in-metric]]

[[math:def-metric-convergence]]

## Facts & Assumptions

[A1] The authoring convention includes the Axiom of Choice. [[math:def-axiom-of-choice]]

[F1] A spacelike embedded hypersurface has positive-definite induced tangent forms. [[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]

[F2] On such a hypersurface the future unit normal is unique and smooth; the induced metric is Riemannian and the positive-sign form $(U,V)\mapsto g(\nabla_U n,V)$ is a well-defined smooth symmetric tensor. [[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form]]

[F3] The Levi–Civita connection is metric compatible: $Vg(Y,Z)=g(\nabla_VY,Z)+g(Y,\nabla_VZ)$. [[physics:def-gr-metric-selected-connection]]

[F4] A Riemannian metric is a smooth positive-definite symmetric covariant two-tensor, with boundaries allowed where stated. [[math:def-riemannian-metric-and-riemannian-manifold]]

[F5] The intrinsic Riemannian distance is the infimum of lengths of piecewise $C^1$ connecting curves, and is a metric on a connected Riemannian manifold, including the stated boundary case. [[math:def-riemannian-distance-on-a-connected-manifold]] [[math:thm-riemannian-distance-is-a-metric]]

[F6] An embedded smooth submanifold with boundary is supplied with a manifold-with-boundary smooth structure for which its inclusion into the ambient manifold is a smooth embedding. [[math:def-embedded-smooth-submanifold-with-boundary]]

## Justification

The normal, its tangential covariant derivatives, $h$ and $k$ are well defined and smooth by the stated hypersurface supplier; its second fundamental form has the opposite sign from $k$. The inverse of positive-definite $h$ defines the trace, so maximality is a definite condition. Choose a smooth local extension $v$ of $n$ supplied by the normal lemma. Near each point of $\Sigma$, continuity permits shrinking its ambient neighborhood so that $g(v,v)<0$. Then $\widetilde n=v/\sqrt{-g(v,v)}$ is smooth, has unit timelike length throughout that neighborhood and agrees with $n$ along $\Sigma$.

For any such unit timelike extension, metric compatibility gives $g(\nabla_{\widetilde n}\widetilde n,\widetilde n)=\tfrac12\widetilde n(g(\widetilde n,\widetilde n))=0$ throughout the neighborhood. On $\Sigma$, in a $g$-orthonormal frame $n,e_1,e_2,e_3$ with tangent $e_i$, the divergence trace is $-g(\nabla_n\widetilde n,n)+\sum_{i=1}^3g(\nabla_{e_i}\widetilde n,e_i)$. Its normal term vanishes and its tangent term equals $-\operatorname{tr}_h k$. The normal lemma makes the tangential derivatives independent of extension, so every local unit timelike extension gives the same divergence on $\Sigma$.

Finally, $g(X,n)=g(T,n)-N g(n,n)=0$, so the normal supplier's orthogonal decomposition makes $X$ tangent; the formula gives the unique such decomposition. The embedded-submanifold-with-boundary supplier specifies the smooth structure and smooth inclusion used in the boundary convention. The positive-definiteness hypothesis then gives a Riemannian metric smooth up to the boundary, and the distance suppliers, whose metric argument includes boundary half-charts, make the stated Cauchy-completeness condition well defined. No existence of a maximal hypersurface or complete extension is asserted.

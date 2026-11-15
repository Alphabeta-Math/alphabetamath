---
id: def-lipschitz-cut-area-data
title: Lipschitz height functions, cut measure and Jacobians
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-axiom-of-choice
  - math:lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice
  - def-author-0336834a2590-measurable-surface-domains
  - def-author-0336834a2590-surface-map-jacobian
  - def-author-0336834a2590-endpoint-multiplicity
  - lem-author-0336834a2590-transverse-endpoint-regularity
  - lem-author-0336834a2590-endpoint-area-with-multiplicity
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets
  - physics:def-gr-causal-conditions-and-global-hyperbolicity
  - math:thm-a-regular-level-set-is-an-embedded-submanifold
dependency_roles:
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice: mathematical-premise
  def-author-0336834a2590-measurable-surface-domains: mathematical-premise
  def-author-0336834a2590-surface-map-jacobian: mathematical-premise
  def-author-0336834a2590-endpoint-multiplicity: mathematical-premise
  lem-author-0336834a2590-transverse-endpoint-regularity: mathematical-premise
  lem-author-0336834a2590-endpoint-area-with-multiplicity: mathematical-premise
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets: mathematical-premise
  physics:def-gr-causal-conditions-and-global-hyperbolicity: mathematical-premise
  math:thm-a-regular-level-set-is-an-embedded-submanifold: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 3
---

## Definition

On a smooth Riemannian three-region $(\Sigma,k)$ a locally Lipschitz height $u$ has almost-everywhere chart derivatives, equal to weak derivatives; its metric gradient is defined almost everywhere by $k(\nabla u,\cdot)=du$. Cut area means normalized two-dimensional Hausdorff measure $\mathcal H_k^2$. The initial domain for an endpoint construction is a Borel subset $A$ of a smooth Riemannian surface $(C,h)$, not the possibly nonsmooth image $D$. For $F:A\to\Sigma$ with countably many local $C^1$ extensions, $J(F)$ means the nonnegative Gram Jacobian $J_2F$, and $N(F,A;y)$ counts the initial points arriving at $y$. The area formula is $\int_A J(F)\,d\mu_C=\int_{F(A)}N(F,A;y)\,d\mathcal H_k^2(y)$; therefore surjectivity $F(A)=D$ gives $|D|\le\int_A J(F)\,d\mu_C$. Coincident endpoints do not invalidate this inequality. The identity $|D|=\int_A J(F)\,d\mu_C$ holds if $N(F,A;y)=1$ for $\mathcal H_k^2$-almost every $y\in D$. If $\int_A J(F)\,d\mu_C<\infty$, this multiplicity-one condition is also necessary for equality. Equality with infinite common value need not imply multiplicity one. All measures use the same area normalization and the specified fixed metrics; $J(F)\le1$ is an additional geometric estimate, not part of the definition of Jacobian.

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice. [[math:def-axiom-of-choice]]

[F1] Lipschitz differentiability, weak derivatives and graph calculus are supplied under Countable Choice by [[math:lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice]].

[F2] The Riemannian metric convention is [[math:def-riemannian-metric-and-riemannian-manifold]]. Measurable initial domains, Gram Jacobians and counting multiplicity are defined in [[def-author-0336834a2590-measurable-surface-domains]], [[def-author-0336834a2590-surface-map-jacobian]] and [[def-author-0336834a2590-endpoint-multiplicity]].

[F3] Transverse hitting regularity is [[lem-author-0336834a2590-transverse-endpoint-regularity]]; the area formula with multiplicity and its image-area bound are [[lem-author-0336834a2590-endpoint-area-with-multiplicity]].

[F4] The Lorentzian metric and nonzero null-vector conventions are [[physics:def-gr-smooth-lorentzian-objects]], the positive-definite tangent metric of a spacelike hypersurface is [[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]], and the time-function convention is [[physics:def-gr-causal-conditions-and-global-hyperbolicity]], clause (d). These are mathematical definitions; no physical postulate is used.

[F5] A nonempty regular fibre of a smooth scalar map is an embedded codimension-one submanifold. The proof supplies local projection coordinates for the map, hence identifies the tangent space of the fibre with the kernel of its differential. [[math:thm-a-regular-level-set-is-an-embedded-submanifold]]

## Justification

Apply [F1] in coordinate charts to the height and use the smooth inverse metric to obtain its measurable weak gradient. The area and Jacobian conventions are exactly [F2], and the formula and inequality are [F3]. Multiplicity one almost everywhere suffices for equality by that formula. For necessity in the finite case, put $I=\int_A J(F)\,d\mu_C<\infty$ and suppose $|D|=I$. The measurable set $E=\{y\in D:N(F,A;y)\ge2\}$ satisfies $I=\int_D N(F,A;y)\,d\mathcal H_k^2(y)\ge |D|+\mathcal H_k^2(E)$. Subtracting the finite value $|D|=I$ gives $\mathcal H_k^2(E)=0$. This subtraction is unavailable for infinite common value. Indeed, take $A=C=\mathbb R^2\sqcup\mathbb R^2$ with its Euclidean component metrics and map each component isometrically onto the same plane $D$ in Euclidean $\Sigma=\mathbb R^3$. This map is smooth on both components, $J_2F=1$, $N=2$ everywhere on $D$, and both $|D|$ and $I$ are infinite.

For an endpoint family, [F3] supplies local extensions when the supplied $C^1$ family meets a slice $s=0$ transversely at its unique hit. For null generators of a smooth Lorentzian metric meeting a spacelike slice $\Sigma=s^{-1}(0)$, use a smooth defining function $s$ with $0$ a regular value, as required by [F3]. At a hit $p$, the regular-level coordinates of [F5] give $T_p\Sigma=\ker ds_p$. If the nonzero null tangent $\dot\gamma$ had $ds_p(\dot\gamma)=0$, it would belong to $T_p\Sigma$. Positive definiteness on that space would give $g_p(\dot\gamma,\dot\gamma)>0$, contradicting $g_p(\dot\gamma,\dot\gamma)=0$. Thus $ds_p(\dot\gamma)\ne0$, using precisely the conventions in [F4].

If the family is parametrized by a smooth chosen initial null normal and has smooth geodesic dependence on its open flow domain, it is such a supplied family; these are geometric inputs to be established by an application, not consequences of a Lipschitz height alone. When the defining function $s$ is also a time function, [F4] makes it strictly increasing along each future-oriented generator, and strictly decreasing with the opposite orientation. Either strict monotonicity makes a prescribed time-level hit unique.

A closed $A\subset C$ is Borel by [F2]. Thus an application must verify the smooth initial surface and chosen generator branch, open flow domain, unique transverse hits at a regular level, Borel domain and image coverage. It does not need to prove that $D$ is a smooth or Lipschitz surface. Focal degeneracy at endpoints is allowed as rank loss of the derivative. No inference of the required endpoint-map regularity is made merely from the statement that $D$ is a cut.

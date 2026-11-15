---
id: def-causal-exterior-and-boundary-data
title: Causal exterior, chronological boundaries and Cauchy data
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-killing-field
  - physics:def-gr-causal-curves-and-reachability
  - physics:def-gr-causal-conditions-and-global-hyperbolicity
  - physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets
  - def-author-310ff0f53b38-asymptotically-flat-spacelike-end
  - math:def-local-and-global-flow
  - math:def-interior-closure-boundary-top
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-killing-field: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  physics:def-gr-causal-conditions-and-global-hyperbolicity: mathematical-premise
  physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets: mathematical-premise
  def-author-310ff0f53b38-asymptotically-flat-spacelike-end: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  math:def-interior-closure-boundary-top: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609
      locator: Section 2.6, Definition 2.16, printed/PDF p. 33; section 4.4, opening
        cone-order convention and Definition 4.89, printed/PDF p. 137.
      statement: Inextendibility excludes convergence at either parameter end. Stable
        causality requires a causal Lorentzian metric with strictly wider cones.
      hypotheses: A time-oriented Lorentzian manifold; Definition 2.16 uses continuous
        causal curves on an open interval. The cone comparison is between
        metrics on the same manifold.
      reading_limits: Read the PDF text of Definition 2.16 and the opening of section
        4.4 through Definition 4.89. These passages supply only the stated
        conventions; they do not supply the exact absolutely-continuous
        parameter convention, end structure, or any causal-ladder implication.
        Those curve conventions come from the declared library interfaces.
    - title: E. Gourgoulhon, 3+1 Formalism and Bases of Numerical Relativity,
        arXiv:gr-qc/0703035v1
      url: https://arxiv.org/pdf/gr-qc/0703035
      locator: Section 3.2.1, printed p. 39, PDF page 39, opening paragraph.
      statement: A Cauchy surface is spacelike and meets each endpoint-free causal
        curve once.
      hypotheses: A spacetime with a specified spacelike hypersurface; all causal
        curves are taken in that spacetime.
      reading_limits: Read the opening paragraph of section 3.2.1 in the PDF text. It
        supplies the conventional Cauchy-surface terminology, not the exact
        parameter-counting convention, and is not used to prove equivalence with
        the strong-causality/compact-diamond formulation.
dependency_level: 1
---

## Definition

Let $(D,g,N)$ be a time-oriented smooth Lorentzian four-manifold of signature $(-,+,+,+)$, and let $U\subset D$ be a specified open subset. Here a Killing field is a smooth vector field with $\mathcal L_Tg=0$; future timelike means $g(T,T)<0$ and $g(T,N)<0$.

For the stationary-end terminology, supply an end chart: a spacelike embedded hypersurface $S_{\rm ext}\subset D$ without manifold boundary and a specified diffeomorphism $e:\{x\in\mathbb R^3:|x|>R\}\to S_{\rm ext}$ for some $R>0$. This is the end-chart data of the spacelike-end interface, with its finite-radius boundary removed. Also supply a local flow $\Phi:\Omega\to D$ of a specified Killing field $T$, with $\Omega\subset\mathbb R\times D$ open and containing $\{0\}\times D$, in the local-flow interface's sense. Require $U=\{\Phi(t,p):p\in S_{\rm ext},\ (t,p)\in\Omega\}$ and $T$ future timelike on $U$; then call $U$, with these supplied data, a stationary end. The chart supplies the spatial end topology. Metric decay, completeness of the flow and a global product identification of $U$ are additional hypotheses when needed. The causal exterior and boundary constructions below apply to any specified open $U$, independently of whether this end structure is supplied.

For $p,q\in D$, write $p\ll_D q$ when a future-directed timelike curve in $D$ joins $p$ to $q$. Curves are locally absolutely continuous, with nonzero future-directed timelike velocity almost everywhere. Define $I_D^+(U)=\{q\in D:\exists p\in U,\ p\ll_D q\}$ and $I_D^-(U)=\{p\in D:\exists q\in U,\ p\ll_D q\}$. The causal exterior relative to $(D,g,U)$ is $\mathcal E=I_D^-(U)\cap I_D^+(U)$. Its future and past event boundaries relative to $U$ are respectively $\partial_D I_D^-(U)$ and $\partial_D I_D^+(U)$, where $\partial_D A=\overline A^{\,D}\setminus\operatorname{int}_D A$. Closure and interior are taken in the manifold topology of $D$, with their topological-interface meanings. These boundaries are taken in $D$; their intersection and their relation to $\partial_D\mathcal E$ are not prescribed.

A future causal curve has locally absolutely continuous coordinates and nonzero future causal velocity almost everywhere. It is inextendible in $D$ when it converges to no point of $D$ at either parameter end. A subset $S\subset D$ is a Cauchy set in $D$ when every such inextendible causal curve has exactly one parameter value in $S$. A Cauchy hypersurface is a Cauchy set that is also an embedded three-dimensional submanifold with positive-definite induced metric. These conditions are relative to $D$; for a different open domain, inextendibility and the Cauchy condition are recomputed there.

Write $J_D^+(p)$ for $p$ together with points reached from $p$ by future causal curves, and $J_D^-(q)$ for the corresponding causal past. Strong causality means that each point has arbitrarily small open neighborhoods that no future causal curve can leave and subsequently re-enter. Global hyperbolicity means strong causality and compactness in $D$ of every $J_D^+(p)\cap J_D^-(q)$. A temporal function is a smooth real function $\tau$ whose metric gradient is everywhere past-directed timelike, equivalently $g(\nabla\tau,\nabla\tau)<0$ and $d\tau(N)>0$.

For this interface, $(D,g,N)$ is stably causal when there is a smooth Lorentzian metric $\widehat g$ on $D$, with $N$ timelike for $\widehat g$, such that every nonzero $g$-causal vector is $\widehat g$-timelike and $(D,\widehat g,N)$ has no closed future causal curve. This is a separate condition from global hyperbolicity and from the existence of a temporal function; no implication between them is asserted here. In particular, no causal property of a different or deformed metric follows merely from a property of $g$.

## Definition references

[[physics:def-gr-smooth-lorentzian-objects]]

[[physics:def-gr-killing-field]]

[[physics:def-gr-causal-curves-and-reachability]]

[[physics:def-gr-causal-conditions-and-global-hyperbolicity]]

[[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]

[[def-author-310ff0f53b38-asymptotically-flat-spacelike-end]]

[[math:def-local-and-global-flow]]

[[math:def-interior-closure-boundary-top]]

## Facts & Assumptions

[F1] The time orientation, causal character and Killing-field equation have the meanings in the stated Lorentzian and Killing-field interfaces. [[physics:def-gr-smooth-lorentzian-objects]] [[physics:def-gr-killing-field]]

[F2] The curve class, chronological and causal reachability, and endpoint formulation of inextendibility are those of the causal-curve interface, applied to $D$. [[physics:def-gr-causal-curves-and-reachability]]

[F3] Strong causality, causal diamonds, global hyperbolicity and temporal functions have the meanings in the causal-conditions interface, applied to $D$. [[physics:def-gr-causal-conditions-and-global-hyperbolicity]]

[F4] A Cauchy set counts parameter values of inextendible causal curves, and a Cauchy hypersurface is a spacelike embedded Cauchy set. [[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]

[F5] The spacelike-end interface supplies the end-chart data; only its chart part is used here, while its asymptotic-flatness inequalities remain additional conditions. The local-flow interface supplies the domain, map and integral-curve laws for $\Phi$. [[def-author-310ff0f53b38-asymptotically-flat-spacelike-end]] [[math:def-local-and-global-flow]]

[F6] Interior is the union of open subsets of a set, closure is the intersection of its closed supersets, and boundary is closure minus interior, all in the chosen topology. [[math:def-interior-closure-boundary-top]]

## Justification

**Given:** The data $(D,g,N,U)$ in the Definition, with the end chart, $T$ and its local flow supplied when the stationary-end terminology is used.

**Goal:** Check that the defined sets and predicates are unambiguous for those data.

1.1 The specified end chart determines $S_{\rm ext}$ and its spatial exterior coordinates. The supplied local flow defines $\Phi(t,p)$ at exactly the pairs used in the displayed set; equality of that set with $U$ and the timelikeness inequalities are therefore definite predicates on the supplied data. This construction uses only the chart part of the spacelike-end interface and assumes no metric decay or flow completeness. [given, F1, F5]

1.2 The time orientation and metric determine the permitted curve classes and the relations $\ll_D$ and $J_D^\pm$; the displayed existential conditions therefore determine subsets of $D$. Intersection and the closure-minus-interior operation in the specified topology then determine $\mathcal E$ and both named boundaries, including when any of these sets is empty. [F1, F2, F6]

2.1 The Cauchy predicate specifies exactly which curves and parameter values are counted, while the hypersurface, strong-causality, diamond-compactness and temporal predicates use the stated interfaces. The stable-causality clause explicitly quantifies over a second metric and its causal curves, so it too is a definite predicate; it assumes neither the existence of such a metric nor any implication for another metric. [F1, F2, F3, F4, step 1.1, step 1.2] ∎

## External input

Minguzzi's Definition 2.16 supplies the endpoint convention for inextendibility; section 4.4 and Definition 4.89 supply the wider-cone definition of stable causality. The fixed orientation field $N$ selects the future convention used here for both metrics.

Gourgoulhon's section 3.2.1 supplies the conventional once-only intersection wording for a spacelike Cauchy surface. The exact parameter-counting convention used here is supplied by the declared Cauchy-set interface.

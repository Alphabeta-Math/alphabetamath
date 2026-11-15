---
id: def-author-a8fd09e77ebd-relative-stationary-deformation
title: Relative stationary deformation and extension obstruction
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - math:def-axiom-of-choice
  - physics:def-gr-smooth-lorentzian-objects
  - math:def-smooth-vector-field-as-a-tangent-bundle-section
  - math:thm-fundamental-theorem-on-flows
  - math:def-lie-derivative-of-a-tensor-field
  - math:def-lie-bracket-of-smooth-vector-fields
  - math:def-simply-connected
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:def-pullback-of-a-covariant-tensor-field
  - math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism
  - math:def-smooth-manifold
  - math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure
dependency_roles:
  math:def-axiom-of-choice: mathematical-premise
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  math:def-smooth-vector-field-as-a-tangent-bundle-section: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  math:def-lie-derivative-of-a-tensor-field: mathematical-premise
  math:def-lie-bracket-of-smooth-vector-fields: mathematical-premise
  math:def-simply-connected: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:def-pullback-of-a-covariant-tensor-field: mathematical-premise
  math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism: mathematical-premise
  math:def-smooth-manifold: mathematical-premise
  math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Definition

Work in ZFC, including the axiom of choice. A smooth manifold carries a maximal smooth atlas on a Hausdorff second-countable topological manifold. A smooth Lorentzian metric on a smooth four-manifold without boundary is a smooth symmetric nondegenerate covariant two-tensor of signature $(-,+,+,+)$. For a smooth vector field $X$ and a smooth metric $h$, write $\mathcal L_Xh=\left.\frac{d}{dt}\right|_{t=0}\Phi_t^*h$, where $\Phi_t$ is the local flow of $X$; call $X$ an $h$-Killing field when $\mathcal L_Xh=0$. These definitions require no chosen orientation or time orientation. Brackets use $[X,Y]u=X(Yu)-Y(Xu)$ for smooth functions $u$; simply connected means nonempty and path-connected with trivial fundamental group at every basepoint.

A **relative stationary deformation datum** consists of a connected simply connected smooth four-dimensional manifold $U$ without boundary, a nonempty connected open subset $O\subset U$, smooth Lorentzian metrics $g_0,\widetilde g$ with $g_0=\widetilde g$ on $O$, a smooth $\widetilde g$-Killing field $T$ on $U$, and a smooth $g_0$-Killing field $Z$ on $O$ satisfying $[T|_O,Z]=0$ there. The open set $O$ carries the subspace topology and canonical restricted smooth structure of $U$. The matching subset $O$ is part of the datum; no agreement of the two metrics elsewhere is imposed.

The datum has a **commuting-extension obstruction** when no smooth field $Y$ on all of $U$ obeys $\mathcal L_Y\widetilde g=0$, $[T,Y]=0$ and $Y|_O=Z$. This is a relative extension problem for a specified germ on a connected matching region, not a claim that no other local Killing field exists.

For a specified smooth Lorentzian four-manifold $(V,g_V)$, with $V$ allowed to be an open neighborhood in a model manifold, an **isometry onto the model neighborhood** means a smooth diffeomorphism $F:U\to V$ with $F^*g_V=\widetilde g$. Here a diffeomorphism is a bijective smooth map with smooth inverse, and $(F^*g_V)_p(v,w)=(g_V)_{F(p)}(dF_pv,dF_pw)$ for $v,w\in T_pU$. The pushed-forward field is $(F_*T)_{F(p)}=dF_p(T_p)$; no condition on $F_*T$ is part of this definition.

## Definition references

[[math:def-axiom-of-choice]]

[[math:def-smooth-manifold]]

[[math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure]]

[[physics:def-gr-smooth-lorentzian-objects]]

[[math:def-smooth-vector-field-as-a-tangent-bundle-section]]

[[math:thm-fundamental-theorem-on-flows]]

[[math:def-lie-derivative-of-a-tensor-field]]

[[math:def-lie-bracket-of-smooth-vector-fields]]

[[math:def-simply-connected]]

[[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

[[math:def-pullback-of-a-covariant-tensor-field]]

[[math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism]]

## Facts & Assumptions

[A1] The ambient ZFC convention includes the axiom of choice. Its restriction to countable families meets the countable-choice hypotheses of the canonical tangent-bundle, smooth-vector-field and pushforward conventions used here. No choice of an orientation or time orientation is made. [[math:def-axiom-of-choice]]

[F1] Clause (a) of the Lorentzian-object definition supplies the smooth metric and signature conventions on a four-manifold without boundary. Its later clause (c) introduces time orientation as additional data, which are not used here. This supplier has mathematical domain. [[physics:def-gr-smooth-lorentzian-objects]]

[F2] Smooth vector fields are smooth tangent-bundle sections. Every such field has a unique maximal smooth local flow, and the Lie derivative of a smooth tensor field is its pullback derivative along that flow. The Killing condition in this item is defined by applying this general Lie derivative to the metric. [[math:def-smooth-vector-field-as-a-tangent-bundle-section]] [[math:thm-fundamental-theorem-on-flows]] [[math:def-lie-derivative-of-a-tensor-field]]

[F3] The bracket is the commutator on smooth functions; simple connectedness includes nonemptiness and path connectedness with trivial fundamental group at every basepoint. [[math:def-lie-bracket-of-smooth-vector-fields]] [[math:def-simply-connected]]

[F4] Diffeomorphisms have smooth inverses. Covariant-tensor pullback evaluates the target tensor on the differentials of the argument vectors, and vector-field pushforward by a diffeomorphism is given by its differential at the inverse image. [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]] [[math:def-pullback-of-a-covariant-tensor-field]] [[math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism]]

[F5] A smooth manifold is a topological manifold equipped with a maximal smooth atlas. An open subset, with its subspace topology, has the canonical restricted smooth structure, of the same dimension and without boundary. Here this applies to $O\subset U$ and to any open model neighborhood $V$. [[math:def-smooth-manifold]] [[math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure]]

## Justification

**Given:** The displayed metrics, open sets, fields and specified model $(V,g_V)$, under the ambient ZFC convention.

**Goal:** Specify the relative extension problem and model-isometry condition precisely.

1.1 The given smooth structure on $U$ restricts canonically to the open subset $O$ with its subspace topology, making $O$ a smooth four-manifold without boundary. Both metrics are Lorentzian by the pointwise metric definition, without any chosen orientation. The smooth fields on $U$ and on its open submanifold $O$ have local flows. Thus the pullback derivative defines their metric Lie derivatives and the stated Killing predicates on the respective domains. Countable choice needed for the smooth tangent-bundle conventions is available by restricting the ambient axiom of choice to countable families. [A1, F1, F2, F5]

2.1 At each point of $O$, sufficiently short segments of the local flow of $Z$ stay in $O$. Since the two metrics coincide throughout $O$, their pullbacks along those segments coincide, hence so do their derivatives at parameter zero. The Killing equation for $Z$ is therefore the same on $O$ for either metric. Restrictions of fields and their commutator are defined there, using only their action on smooth functions on that open set. [F2, F3, step 1.1]

3.1 The three extension equations are predicates on a smooth field on all of $U$; their joint nonexistence defines a property of the datum without asserting existence of obstructed data. With the model manifold and its metric specified, the tensor pullback and vector pushforward have precisely the displayed meanings. The isometry predicate concerns the metric alone and does not identify the stationary generator with a preferred model field. [A1, F2, F3, F4, step 2.1] ∎

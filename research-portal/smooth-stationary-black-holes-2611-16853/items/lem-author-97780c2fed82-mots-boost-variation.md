---
id: lem-author-97780c2fed82-mots-boost-variation
title: MOTS boosts preserve the spacetime stability sign
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-97780c2fed82-general-spacelike-surface-data
  - lem-author-97780c2fed82-mots-variation-second-jet
dependency_roles:
  def-author-97780c2fed82-general-spacelike-surface-data: mathematical-premise
  lem-author-97780c2fed82-mots-variation-second-jet: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

For a MOTS with null pair $(\ell,k)$ normalized by $g(\ell,k)=-1$, let $h:S\to(0,\infty)$ be smooth and set $\ell'=h\ell$, $k'=h^{-1}k$. For the same normal velocity $X$, the variation satisfies $\delta_X\theta_{(\ell')}=h\delta_X\theta_{(\ell)}$. Consequently if $X=\gamma\ell-\psi k$ with $\gamma\ge0$ and $\psi>0$, then $X=\gamma'\ell'-\psi'k'$ with $\gamma'=\gamma/h\ge0$, $\psi'=h\psi>0$, and the inequality $\delta_X\theta\ge0$ is unchanged by the boost.

## Statement references

[[def-author-97780c2fed82-general-spacelike-surface-data]]

[[lem-author-97780c2fed82-mots-variation-second-jet]]

## Facts & Assumptions

[F1] The null pairing and tangential expansion use the general surface convention. [[def-author-97780c2fed82-general-spacelike-surface-data]]

[F2] The variation at a MOTS is well defined and independent of extensions of its base null gauge. [[lem-author-97780c2fed82-mots-variation-second-jet]]

## Proof

**Given:**The objects and hypotheses in the Statement.

**Goal:** Establish the assertions and well-definedness stated there.

1.1 Choose any actual deformation realizing $X$ and extend $h$ smoothly along its parameter with its prescribed initial value. Orthogonality of $\ell_t$ to the tangent surface gives $\theta_{(h_t\ell_t)}=h_t\theta_{(\ell_t)}$. Differentiating at zero gives $\delta_X\theta_{(\ell')}=h\delta_X\theta_{(\ell)}+(\partial_th_t)|_0\theta_{(\ell)}=h\delta_X\theta_{(\ell)}$. Its sign is unchanged since $h>0$. [F1, F2]

2.1 Substitution of $\ell=\ell'/h$ and $k=hk'$ into $X$ gives the stated new coefficients and signs. Moreover $g(X,X)=2\gamma\psi\ge0$, so these are outgoing non-timelike normal directions, including the past null direction $-k$ when $\gamma=0$. This is a pointwise identity and does not assume that $X$ is tangent to a spacelike slice. [F1, step 1.1] ∎

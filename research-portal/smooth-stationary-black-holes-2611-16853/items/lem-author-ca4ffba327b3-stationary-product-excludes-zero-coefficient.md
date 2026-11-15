---
id: lem-author-ca4ffba327b3-stationary-product-excludes-zero-coefficient
title: A stationary product rules out a zero Hawking coefficient
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - math:def-local-and-global-flow
  - math:thm-unique-maximal-integral-curve-through-each-point
  - math:def-complete-vector-field
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure
  - math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure
  - math:def-smooth-manifold
  - math:def-c-r-and-smooth-maps-between-smooth-manifolds
  - math:def-derivation-at-a-point-and-tangent-space
  - math:def-velocity-derivation-of-a-smooth-curve
dependency_roles:
  math:def-local-and-global-flow: mathematical-premise
  math:thm-unique-maximal-integral-curve-through-each-point: mathematical-premise
  math:def-complete-vector-field: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure: mathematical-premise
  math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure: mathematical-premise
  math:def-smooth-manifold: mathematical-premise
  math:def-c-r-and-smooth-maps-between-smooth-manifolds: mathematical-premise
  math:def-derivation-at-a-point-and-tangent-space: mathematical-premise
  math:def-velocity-derivation-of-a-smooth-curve: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
sources:
  references:
    - title: Will J. Merry, Differential Geometry (2021)
      url: https://www2.math.ethz.ch/will-merry/files/Merry%20-%20Differential%20Geometry%20%282021%29.pdf
      locator: Lecture 8, Proposition 8.2(iii), equations (8.1)-(8.3); Lecture 9,
        Definition 9.3, equation (9.2).
      statement: On a nonempty open manifold domain, a tangent-vector assignment is
        smooth iff X(f) is smooth for every local smooth f. A smooth curve is an
        integral curve iff its velocity equals the field along it.
      hypotheses: A smooth manifold M and nonempty open W contained in M; X(p) in T_pM
        for p in W. For the integral-curve definition, X is a smooth vector
        field and the curve is smooth on an open real interval.
      reading_limits: Read the primary-source indexed excerpts containing Proposition
        8.2 and Definition 9.3. Full PDF retrieval failed. Only these
        formulations are imported; no tangent-bundle second-countability
        construction or choice-independence theorem is imported.
---

## Statement

Let $M$ be a smooth manifold and let $D,V\subseteq M$ be open subsets with their restricted smooth structures and $D\cap V\ne\varnothing$. Let $T$ be a smooth vector field on $M$ whose restriction to $D$ is complete, with global flow $\phi:\mathbb R\times D\to D$.

Let $C$ be a smooth manifold and $i:C\to D$ a smooth map. Equip $\mathbb R\times C$ with its product smooth structure, and suppose $F:\mathbb R\times C\to D$, $F(t,x)=\phi_t(i(x))$, is a diffeomorphism.

Let $K_0$ be a smooth vector field on $V$, let $\lambda\in\mathbb R$ be constant, and set $Z_0=T|_V+\lambda K_0$. Suppose $Z_0$ has a local flow $\Psi:\mathcal U\to V$, where $\mathcal U\subseteq\mathbb R\times V$, and there is a constant $P>0$ such that $\{P\}\times V\subseteq\mathcal U$ and $\Psi(P,q)=q$ for every $q\in V$. Then $\lambda\ne0$. No stationary orbit is treated as a causal curve in this argument.

## Statement references

[[math:def-local-and-global-flow]]

[[math:thm-unique-maximal-integral-curve-through-each-point]]

[[math:def-complete-vector-field]]

[[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

[[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure]]

[[math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure]]

[[math:def-smooth-manifold]]

[[math:def-c-r-and-smooth-maps-between-smooth-manifolds]]

[[math:def-derivation-at-a-point-and-tangent-space]]

[[math:def-velocity-derivation-of-a-smooth-curve]]

## Facts & Assumptions

[F1] A flow obeys the group law, its trajectories are integral curves, and each local-flow time fibre is an interval containing zero. Integral curves of the same smooth field on the same ambient manifold with the same initial point agree on their common time interval by uniqueness of the maximal integral curve. [[math:def-local-and-global-flow]] [[math:thm-unique-maximal-integral-curve-through-each-point]]

[F2] Completeness means that each maximal integral curve is defined on all of $\mathbb R$. A diffeomorphism is a bijective smooth map with smooth inverse; in particular it is surjective and injective. [[math:def-complete-vector-field]] [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

[F3] Open subsets carry their canonical restricted smooth structures, and the product of two smooth manifolds carries the canonical product smooth structure. These are the structures used for $D$, $V$ and $\mathbb R\times C$. [[math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure]] [[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure]]

[F4] Use the local-function definition of a smooth field $X$ on a smooth manifold $N$: each $X(p)\in T_pN$ is a derivation and $X(f)(p):=X(p)([f])$ is smooth for every local smooth function $f$. This is Merry, Proposition 8.2(iii). Manifolds, smooth maps and tangent derivations have their existing meanings. [[math:def-smooth-manifold]] [[math:def-c-r-and-smooth-maps-between-smooth-manifolds]] [[math:def-derivation-at-a-point-and-tangent-space]]

[F5] An integral curve satisfies $\gamma'(s)=X(\gamma(s))$ (Merry, Definition 9.3). With velocity as a derivation this means $(f\circ\gamma)'(s)=X(f)(\gamma(s))$ for every local smooth $f$. The velocity definition at $s$ is the definition at zero applied to $t\mapsto\gamma(s+t)$. [[math:def-velocity-derivation-of-a-smooth-curve]]

## External input

The terminology in [F4] and [F5] uses only [Merry, Proposition 8.2(iii) and Definition 9.3](https://www2.math.ethz.ch/will-merry/files/Merry%20-%20Differential%20Geometry%20%282021%29.pdf). The local-function formulation does not require constructing a smooth manifold structure on the total tangent bundle.

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove $\lambda\ne0$.

1.1 For any $q\in D$, surjectivity gives $q=F(t,x)$ for some $(t,x)\in\mathbb R\times C$. The flow law gives $\phi_P(q)=\phi_{t+P}(i(x))=F(t+P,x)$. If this equaled $q$, injectivity of $F$ would give $t+P=t$, contrary to $P>0$. Thus the complete stationary flow has no positive period at any point of $D$. [given, F1, F2]

2.1 Suppose $\lambda=0$ and choose $q\in V\cap D$. The curve $\alpha(s)=\phi_s(q)$ is defined for all $s\in\mathbb R$ and takes values in $D$. The curve $\beta(s)=\Psi(s,q)$ is defined on the time fibre $I_q=\{s:(s,q)\in\mathcal U\}$, an interval containing $[0,P]$, and takes values in $V$. For every local smooth function $f$ on $M$, restrict $f$ to the relevant open domain. By [F3]-[F5], the two flow-curve equations give $(f\circ\alpha)'(s)=T(f)(\alpha(s))$ and $(f\circ\beta)'(s)=T(f)(\beta(s))$, since $Z_0=T|_V$. Restricted charts identify the germs and derivations on each open domain with those in $M$. Thus both curves, viewed in $M$, are integral curves of the same ambient field $T$ with initial point $q$. Uniqueness therefore gives $\beta(s)=\alpha(s)$ throughout $I_q$, without assuming beforehand that $\beta$ stays in $D$. In particular $\phi_P(q)=\Psi(P,q)=q$, contradicting step 1.1. Hence $\lambda\ne0$. [given, F1, F2, F3, F4, F5, step 1.1] ∎

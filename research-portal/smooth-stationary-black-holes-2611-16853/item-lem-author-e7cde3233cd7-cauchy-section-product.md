---
title: A generic timelike product for a prescribed smooth Cauchy section
status: draft
research_item: lem-author-e7cde3233cd7-cauchy-section-product
dependency_level: 2
sources:
  references: []
---

## Prerequisites

- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [physics:lem-gr-finite-smooth-volume-density](https://alphabetamath.cc/physics/item/lem-gr-finite-smooth-volume-density)
- [physics:thm-gr-volume-time-function](https://alphabetamath.cc/physics/item/thm-gr-volume-time-function)
- [physics:thm-gr-smooth-cauchy-temporal-splitting](https://alphabetamath.cc/physics/item/thm-gr-smooth-cauchy-temporal-splitting)
- [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)
- [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [math:thm-continuous-image-of-a-connected-space](https://alphabetamath.cc/item/thm-continuous-image-of-a-connected-space)


## Statement

Let $D$ be a nonempty globally hyperbolic time-oriented smooth Lorentzian four-manifold and $C\subset D$ a smooth spacelike Cauchy hypersurface. In ZFC there is a diffeomorphism $\mathbb R\times C\to D$. In particular, if $D$ is connected, then $C$ is connected. This product uses a timelike auxiliary flow; it need not be the flow of a given stationary Killing field.

## Facts & Assumptions

[F1] Cauchy hypersurfaces and global hyperbolicity use [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data), in ZFC including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice).

[F2] A normalized positive finite smooth density exists by [physics:lem-gr-finite-smooth-volume-density](https://alphabetamath.cc/physics/item/lem-gr-finite-smooth-volume-density). With this density [physics:thm-gr-volume-time-function](https://alphabetamath.cc/physics/item/thm-gr-volume-time-function) supplies its volume time, and [physics:thm-gr-smooth-cauchy-temporal-splitting](https://alphabetamath.cc/physics/item/thm-gr-smooth-cauchy-temporal-splitting) supplies a smooth temporal function $t$ and complete timelike field $X$ with $X(t)=1$ and global flow $\Phi$.

[F3] A smooth map with invertible differential has a local smooth inverse by [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds).


[F4] The product has the canonical smooth structure of [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure). Diffeomorphism and local diffeomorphism have the meanings in [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds); in particular a diffeomorphism and its inverse are continuous.

[F5] A continuous surjection from a connected space has connected target by [math:thm-continuous-image-of-a-connected-space](https://alphabetamath.cc/item/thm-continuous-image-of-a-connected-space).

## Proof

**Given:** The hypotheses in the Statement and the declared supplier interfaces.

**Goal:** Prove the stated conclusions.

1.1 Apply [F2] with precisely its finite-density and volume-time inputs. Along every $X$-orbit, $t(\Phi_s(z))=t(z)+s$; hence neither parameter end can converge to a point of $D$. Each orbit is an inextendible timelike curve, so meets $C$ exactly once. Therefore $(s,c)\mapsto\Phi_s(c)$ is surjective. If two such points agree, the common orbit meets $C$ at the same point; equality of $t$ then gives equality of the flow parameters. Thus the map is bijective. [given, F1, F2]

2.1 Equip $\mathbb R\times C$ with the canonical product smooth structure of [F4]. The map in step 1.1 is smooth as the restriction of the global smooth flow. Its differential sends the parameter direction to $X$ and the three section directions to the flow image of $TC$. Since a spacelike three-plane cannot contain the timelike $X$, these four directions are linearly independent at parameter zero and remain so under the invertible flow differential. The map is thus a local diffeomorphism by [F3], and its local inverses combine into a smooth inverse because it is bijective, giving a diffeomorphism in the sense of [F4]. Compose its continuous inverse with the continuous product projection to $C$. This is a continuous surjection $D\to C$, so [F5] shows that $C$ is connected when $D$ is. No claim about a stationary flow was used. [F1, F2, F3, F4, F5, step 1.1] ∎

## Source notes

Used the exact published library Statement interfaces for density, volume time and temporal splitting, including the extra volume-time premise of the splitting theorem. The product-structure proposition, diffeomorphism definition and connected-image theorem are also used through their published library interfaces. Their linked external literature was not independently read here; no new external theorem is imported.

---
title: Uniqueness forces an extended axial field to commute
status: draft
research_item: lem-author-a8fd09e77ebd-commutation-from-uniqueness
dependency_level: 2
---

## Prerequisites

- [def-author-a8fd09e77ebd-relative-stationary-deformation](item-def-author-a8fd09e77ebd-relative-stationary-deformation)
- [lem-author-a8fd09e77ebd-killing-bracket](item-lem-author-a8fd09e77ebd-killing-bracket)


## Statement

Let a relative datum as in [def-author-a8fd09e77ebd-relative-stationary-deformation](item-def-author-a8fd09e77ebd-relative-stationary-deformation) have the following uniqueness property: two global Killing fields of $\widetilde g$ agreeing on a nonempty open set agree on all of $U$. If $Z$ has any global Killing extension $Y$, then $[T,Y]=0$ on $U$. Consequently, for this uniqueness property, a commuting-extension obstruction excludes every global Killing extension of $Z$, not just those initially assumed to commute.

## Facts & Assumptions

[F1] On $O$ the relative datum has $[T,Z]=0$. [def-author-a8fd09e77ebd-relative-stationary-deformation](item-def-author-a8fd09e77ebd-relative-stationary-deformation)

[F2] A bracket of smooth Killing fields is Killing. [lem-author-a8fd09e77ebd-killing-bracket](item-lem-author-a8fd09e77ebd-killing-bracket)

[A1] The stated uniqueness property is an explicit premise of this local implication, not an assertion proved here.

## Proof

**Given:** The datum, uniqueness property and a global Killing extension $Y$.

**Goal:** Show the extension commutes with $T$.

1.1 The global field $W=[T,Y]$ is Killing by [F2]. Since $Y|_O=Z$, its bracket with $T$ vanishes on the open set $O$. Equality of restrictions on an open set includes the derivatives defining the bracket. [F1, F2]

2.1 Apply the stated uniqueness property to the global Killing fields $W$ and zero: they agree on $O$, hence on $U$. Thus $[T,Y]=0$. If a commuting extension is forbidden, the existence of any Killing extension contradicts that prohibition. [A1, step 1.1] ∎

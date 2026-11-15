---
title: The inward null family reaches the future local horizon in short affine time
status: draft
research_item: lem-author-fd27ddabb933-inward-null-local-horizon-crossing
dependency_level: 4
---

## Prerequisites

- [lem-author-fd27ddabb933-future-horizon-defining-pair](item-lem-author-fd27ddabb933-future-horizon-defining-pair)
- [lem-author-fd27ddabb933-outward-graph-null-initial-jets](item-lem-author-fd27ddabb933-outward-graph-null-initial-jets)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in ZFC. For the ambient affine geodesics $\gamma_{\epsilon,y}$ with initial vector $n_\epsilon-\nu_\epsilon$, there are fixed positive constants C and tau0 such that every sufficiently small positive epsilon has a first crossing $a=0,b>0$ at parameter at most $C\epsilon<\tau_0$. These geodesics remain in a fixed compact tube for $0\le\lambda\le\tau_0$. This is a local assertion in the smooth ambient metric across S, independent of completeness of exterior null geodesics.

## Facts & Assumptions

[F1] The initial outward graph and inward normal have the stated uniform defining-function jets. [lem-author-fd27ddabb933-outward-graph-null-initial-jets](item-lem-author-fd27ddabb933-outward-graph-null-initial-jets)

[F2] The smooth ambient metric across the bifurcation surface has a smooth geodesic flow on an open domain. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F3] In the common ambient tube $O$ of the compact surface $S$, the smooth defining pair $a=v-u$, $b=v+u$ identifies the future half-sheet as $H_f^+\cap O=\{a=0,b>0\}$. [lem-author-fd27ddabb933-future-horizon-defining-pair](item-lem-author-fd27ddabb933-future-horizon-defining-pair)

[A1] Work in ZFC, including the countable and dependent choice required by the invoked geodesic, compactness and causal interfaces. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The assumptions in the Statement.

**Goal:** Establish the stated conditional claim.

1.1 The compact initial-data family in [F1] and the open smooth geodesic-flow domain in [F2] give a common tau0 and a smaller compact tube containing all these short geodesics. Smooth dependence and the negative initial a-derivative make $d(a\circ\gamma)/d\lambda\le-1$ on a common short interval after shrinking. Since $0<a(0)\le C_0\epsilon$, integration forces a first zero by $C_0\epsilon$. [F1, F2, F3, given, algebra]

2.1 On intervals of length at most $C_0\epsilon$, smooth dependence gives $|d(b\circ\gamma)/d\lambda|\le C_1(\epsilon+\lambda)$: at epsilon zero and lambda zero that derivative vanishes, uniformly over compact S. Hence b changes by $O(\epsilon^2)$ before the crossing, whereas $b(0)\ge c\epsilon$ by [F1]. Thus b is positive at that crossing, which is on the future branch by [F3]. Choose C at least C0 and then epsilon small enough that $C\epsilon<\tau_0$. [F1, F2, F3, step 1.1, algebra] ∎

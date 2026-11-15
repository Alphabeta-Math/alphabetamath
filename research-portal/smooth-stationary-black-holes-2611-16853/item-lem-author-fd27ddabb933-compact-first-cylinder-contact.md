---
title: Compactness gives an earliest translated-cylinder causal contact
status: draft
research_item: lem-author-fd27ddabb933-compact-first-cylinder-contact
dependency_level: 2
---

## Prerequisites

- [physics:lem-gr-globally-hyperbolic-causal-structure](https://alphabetamath.cc/physics/item/lem-gr-globally-hyperbolic-causal-structure)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)
- [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)
- [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)
- [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)
- [math:thm-product-universal-property](https://alphabetamath.cc/item/thm-product-universal-property)
- [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)
- [math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in ZFC. Let $(\mathcal E,g,N)$ be a time-oriented smooth globally hyperbolic Lorentzian four-dimensional exterior, and let $\tau:\mathcal E\to\mathbb R$ be temporal: its metric gradient is past-directed timelike everywhere. Let $A\subset\tau^{-1}(0)$ be a compact spacelike source. For this lemma, 'spacelike source' is used in the set sense of acausality: no two distinct points of $A$ can be joined by a future causal curve in either direction. No submanifold structure or fixed dimension is required of $A$. This condition follows already from the displayed temporal-level containment. All causal and chronological relations below are computed in $(\mathcal E,g,N)$.

Let $\phi^T$ be a local flow of a stationary Killing field $T$, defined at every $(t,x)\in\mathbb R\times C_0$ for a compact spacelike cut $C_0\subset\mathcal E$ in the sense specified below. Require that the parameter map $\Phi:\mathbb R\times C_0\to\mathcal E$, $\Phi(t,x)=\phi_t^T(x)$, is continuous in the product topology. Put $C_t=\Phi(\{t\}\times C_0)$ and $\Gamma=\bigcup_{t\in\mathbb R}C_t$. Here the stationary cylinder hypothesis means that $\Gamma$ is a smooth embedded three-dimensional submanifold swept out by the $T$-flow, and timelike means that each $T_p\Gamma$ contains a vector $v$ with $g_p(v,v)<0$. Its compact spacelike cuts mean that every $C_t$ is a compact smooth embedded two-dimensional submanifold of $\mathcal E$ and $g_p(v,v)>0$ for every $p\in C_t$ and nonzero $v\in T_pC_t$. Assume these cylinder and cut hypotheses, that $T$ is future timelike on $\Gamma$, that $A\cap\Gamma=\varnothing$, and that $\tau(\Phi(t,x))=t+\tau(x)$ for all $(t,x)\in\mathbb R\times C_0$.

Assume finite chronological access to this specified cylinder: there is a real $u$ with $C_u\cap I^+_{\mathcal E}(A)\ne\varnothing$. Then the set $\{t\in\mathbb R:C_t\cap J^+_{\mathcal E}(A)\ne\varnothing\}$ has a finite minimum $t_R$, and there is $p_R\in C_{t_R}\cap J^+_{\mathcal E}(A)$. Every causal contact point $p\in\Gamma\cap J^+_{\mathcal E}(A)$ has positive temporal-function value $\tau(p)>0$, in particular $\tau(p_R)>0$. This positivity concerns $\tau(p)$, rather than the flow parameter $t$ indexing $C_t$; no sign for $t_R$ is asserted. Compactness is used for both the source and a bounded-time portion of the cylinder; compactness of the whole unbounded cylinder is not assumed.

## Facts & Assumptions

[F1] In a globally hyperbolic time-oriented smooth Lorentzian four-manifold, the causal future of a compact set is closed, under the supplier's countable and dependent choice assumptions. We use clause (a), with compact source $A$ and all curves in $\mathcal E$. [physics:lem-gr-globally-hyperbolic-causal-structure](https://alphabetamath.cc/physics/item/lem-gr-globally-hyperbolic-causal-structure)

[F2] A temporal function is a time function, hence continuous, and strictly increases between the endpoints of every nonconstant future causal curve. We use clauses (b) and (c), with the temporal function $\tau$ on the same exterior. [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions)

[F3] Chronological futures are contained in causal futures, by clause (f). The finite time $u$ and the chronological contact on $C_u$ are explicit hypotheses of this lemma. [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[F4] A continuous image of a compact space, or of a compact subset of its domain, is compact. A continuous real-valued function on a nonempty compact topological space attains a finite maximum and minimum. We use claims 1 and 2, respectively. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

[F5] Products below carry the product topology, generated by inverse images of open sets under coordinate projections. Every closed bounded real interval is compact, and a finite product of compact spaces is compact in its product topology. [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology) [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r) [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)

[F6] A continuous map has closed preimages of closed sets, by clause (c), and a closed subspace of a compact space is compact, by claim 1. [math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top) [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

[F7] Coordinate projections are continuous, by claim 1. In particular the time coordinate on a product with a real interval is continuous as a real-valued map: an open set $V\subset\mathbb R$ has preimage $([\ell,u]\cap V)\times C_0$, which is open in the product. [math:thm-product-universal-property](https://alphabetamath.cc/item/thm-product-universal-property)

[F8] A local flow has an open domain, a smooth parameter map and the integral-curve and flow laws of the flow definition. Its domain containing $\mathbb R\times C_0$ and the continuity of $\Phi$ on that product are explicitly supplied here, so no completeness of $T$ on the whole exterior is inferred. The exterior, reachability and temporal-function conventions are those of the causal-data definition. The cylinder and cut conditions are the explicit tangent-space and embedded-submanifold predicates in the Statement; embedded submanifolds are understood through slice charts. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

[A1] Work in ZFC, including the countable and dependent choice assumptions carried by the causal and temporal-function suppliers in [F1]–[F3]. The finite extrema and finite-product arguments introduce no additional choice requirement. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the finite earliest contact and positivity of the temporal-function value at every contact point.

1.1 If two distinct source points were causally related, [F2] would strictly order their equal temporal values, which is impossible. Thus the stated set-level spacelike condition holds. Fix the access time $u$. By [F3], $C_u\cap J^+_{\mathcal E}(A)$ is nonempty, so both $A$ and $C_0$ are nonempty. By [F2] and [F4], the continuous function $\tau|_{C_0}$ has a finite maximum $m$. If $z=\Phi(t,x)\in J^+_{\mathcal E}(A)$, choose $a\in A$ causally preceding $z$. Disjointness gives $a\ne z$, so their causal relation is represented by a nonconstant future causal curve entirely in $\mathcal E$. By [F2], $\tau(z)>\tau(a)=0$. Hence $t+\tau(x)>0$, and $t>-\tau(x)\ge-m$. Put $\ell=-m$. Thus every contact time is greater than $\ell$, and in particular $\ell<u$. [given, A1, F2, F3, F4, choose, algebra]

2.1 By [F5], $P=[\ell,u]\times C_0$ is compact. The restriction $\Phi_P:P\to\mathcal E$ is continuous by the supplied continuity of $\Phi$ in [F8], so its image is a compact bounded-time portion of the cylinder by [F4]. By [F1], $J^+_{\mathcal E}(A)$ is closed in $\mathcal E$; therefore $D=\Phi_P^{-1}(J^+_{\mathcal E}(A))$ is closed in $P$ by [F6], and is compact by the same fact. The contact at time $u$ from step 1.1 gives a point of $D$, so $D$ is nonempty. [given, A1, F1, F4, F5, F6, F8, step 1.1, construct]

3.1 Let $\pi:P\to\mathbb R$ be $\pi(t,x)=t$, continuous by [F7]. By [F4], $\pi(D)$ is compact and nonempty, and its identity real-valued function attains a minimum $t_R$. By the definition of this image there is $x_R\in C_0$ with $(t_R,x_R)\in D$; set $p_R=\Phi(t_R,x_R)$. Then $p_R\in C_{t_R}\cap J^+_{\mathcal E}(A)$, and step 1.1 gives $\tau(p_R)>0$. Any contact time at most $u$ is greater than $\ell$ by step 1.1, hence lies in $\pi(D)$ and is at least $t_R$; a contact time greater than $u$ is also at least $t_R$, since $t_R\le u$. Thus $t_R$ is the minimum over all real contact times. [F4, F7, step 1.1, step 2.1, choose, construct, algebra] ∎

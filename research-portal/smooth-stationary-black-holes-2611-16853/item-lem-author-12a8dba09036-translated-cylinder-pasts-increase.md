---
title: Future timelike cylinder translations make their chronological pasts increase
status: draft
research_item: lem-author-12a8dba09036-translated-cylinder-pasts-increase
dependency_level: 2
---

## Prerequisites

- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-dependent-choice](https://alphabetamath.cc/item/def-dependent-choice)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)
- [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)


## Statement

Assume Countable Choice and Dependent Choice for the causal-curve calculus and the causal results used below.

Let $(M,\widehat g,N)$ be a time-oriented smooth Lorentzian four-manifold without boundary, of signature $(-,+,+,+)$. All chronological pasts and curves are taken in $M$, with the locally absolutely continuous curve convention.

Let $T$ be a smooth vector field on $M$ with a supplied local flow $\phi^T:\Omega\to M$, where $\Omega\subseteq\mathbb R\times M$. Supply a subset $C_0\subseteq M$ such that $\mathbb R\times C_0\subseteq\Omega$. Define $C_t=\{\phi^T(t,c):c\in C_0\}$ for every $t\in\mathbb R$, and let the complete cylinder be $C=\bigcup_{t\in\mathbb R}C_t$. Suppose $T$ is future timelike throughout $C$, meaning $\widehat g(T,T)<0$ and $\widehat g(T,N)<0$ there.

Then $A_t=I^-_{\widehat g}(C_t)$ is open in $M$ and $A_s\subseteq A_t$ for $s<t$. If a point $p$ has a future $\widehat g$-timelike curve ending at a point of $C_a$, it belongs to $A_t$ for every $t\ge a$.

## Statement references

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:def-dependent-choice](https://alphabetamath.cc/item/def-dependent-choice)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)

## Facts & Assumptions

[F1] Countable Choice and Dependent Choice are assumed exactly as required by the two causal suppliers; their meanings are the stated choice principles. These assumptions are inherited from those suppliers, rather than a claim that the present finite orbit argument requires a new infinite selection. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) [math:def-dependent-choice](https://alphabetamath.cc/item/def-dependent-choice)

[F2] Time orientation and chronological reachability have the causal-data interface meanings, applied with metric $\widehat g$ on $M$. The metric-selected connection required by the push-up supplier is the connection constructed for this smooth metric in clause (d) of the metric-selected-connection interface. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F3] For a time-oriented smooth Lorentzian four-manifold under [F1], every point chronological past is open. If $p\ll q$ and $q\le r$, the push-up rule gives $p\ll r$; a future timelike curve is in particular future causal. [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness) [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[F4] A supplied local flow is smooth, has interval fibres, follows its smooth vector field and satisfies the flow law wherever both sides are defined. Here $\mathbb R\times C_0\subseteq\Omega$ explicitly supplies every orbit segment used in the proof. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F5] For every subset $S\subseteq M$, its chronological past is $I^-_{\widehat g}(S)=\{p\in M:\exists r\in S,\ p\ll r\}=\bigcup_{r\in S}I^-_{\widehat g}(r)$, using the reachability definition in clause (c); no openness of $S$ is required. [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[F6] In the manifold topology of $M$, any union of open sets is open by topology axiom (T2), and the empty set is open by (T1), including the empty-union case. [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)

## Proof

**Given:** The data and hypotheses of the Statement.

**Goal:** Prove openness, monotonicity and the arrival-time assertion.

1.1 Fix $s<t$ and $q\in C_s$. By the definition of $C_s$, there is $c\in C_0$ with $q=\phi^T(s,c)$. The curve $\gamma(u)=\phi^T(u,c)$ for $s\le u\le t$ is defined because $\mathbb R\times C_0\subseteq\Omega$. Its image lies in $C$, its velocity is $T_{\gamma(u)}$, and the two timelikeness inequalities hold throughout. It is therefore a future timelike curve from $q$ to $r=\phi^T(t,c)\in C_t$. [given, F2, F4]

2.1 For $p\in A_s$ there is $q\in C_s$ with $p\ll q$. Step 1.1 gives $q\ll r$ for some $r\in C_t$, hence $q\le r$. All hypotheses of the causal suppliers hold by the stated smooth four-dimensional setting, [F1] and [F2]. Applying [F3] gives $p\ll r$, so $p\in A_t$. Thus $A_s\subseteq A_t$ for every $s<t$. [given, F1, F2, F3, F5, step 1.1]

3.1 By the definition of chronological past, $A_t=\bigcup_{r\in C_t}I^-_{\widehat g}(r)$. Each set in this union is open by [F3] under the same hypotheses checked in step 2.1, and an arbitrary union of open sets is open. This includes $C_t=\varnothing$, when $A_t=\varnothing$. [F1, F2, F3, F5, F6, step 2.1]

4.1 A future timelike curve from $p$ to a point of $C_a$ gives $p\in A_a$ by definition. For $t>a$, step 2.1 gives $A_a\subseteq A_t$, while for $t=a$ membership was already established. Hence $p\in A_t$ for every $t\ge a$, completing all conclusions. [given, F2, F5, step 2.1, step 3.1] ∎

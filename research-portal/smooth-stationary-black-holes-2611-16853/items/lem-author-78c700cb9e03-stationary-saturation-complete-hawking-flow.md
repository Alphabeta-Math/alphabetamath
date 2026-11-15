---
id: lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow
title: The stationary product extends the local boost and circle to a complete collar
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - math:def-local-and-global-flow
  - math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves
  - math:thm-parametrized-implicit-function-theorem-with-higher-regularity
  - lem-author-78c700cb9e03-invariant-normal-boost-coordinates
  - lem-author-78c700cb9e03-bounded-rapidity-reference-graph
  - math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism
  - math:def-axiom-of-choice
  - math:def-pullback-of-a-covariant-tensor-field
  - math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves: mathematical-premise
  math:thm-parametrized-implicit-function-theorem-with-higher-regularity: mathematical-premise
  lem-author-78c700cb9e03-invariant-normal-boost-coordinates: mathematical-premise
  lem-author-78c700cb9e03-bounded-rapidity-reference-graph: mathematical-premise
  math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-pullback-of-a-covariant-tensor-field: mathematical-premise
  math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 4
---

## Statement

Let $D$ carry a complete field $T$ whose flow $\phi_t^T$ gives a diffeomorphism $\mathbb R\times C\to D$ for a spacelike section $C$. Suppose near a compact boundary sphere the previous boost and graph lemmas hold with $C$ represented by $\tau=a(r,y)$, $|a|\le A$. Let a smooth Lorentz metric family $g_q$ be stationary on $D$, with $K$ and $Z$ Killing for every $g_q$ on that local tube, and $K=T+\Omega Z$ there. For sufficiently small $r_0>0$, there is an open stationary saturation $D_0\subset D$ and a diffeomorphism $\mathcal F:(0,r_0)\times\mathbb R\times S\to D_0$ agreeing with the actual normal tube near the reference collar, with $\mathcal F_*\partial_\tau=K$ and $\mathcal F_*Z_S=Z$. These extended fields are Killing for every $g_q$ on $D_0$, commute with $T$, and are complete on $D_0$; $Z$ remains periodic. This is an extension to a collar saturation, not to all of $D$.

## Statement references

[[def-stationary-lorentzian-data]]

[[math:def-local-and-global-flow]]

[[math:thm-parametrized-implicit-function-theorem-with-higher-regularity]]

[[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]]

[[lem-author-78c700cb9e03-bounded-rapidity-reference-graph]]

[[math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism]]

## Facts & Assumptions

[F1] Formal boost/circle coordinates and the bounded graph/root construction are supplied by the two preceding lemmas. [[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]] [[lem-author-78c700cb9e03-bounded-rapidity-reference-graph]]

[F2] Completeness means that the stationary flow is defined for all real times. For a smooth vector field on a smooth manifold, integral curves with the same initial value are locally unique and depend smoothly on the initial point. This applies to the smooth field $T$ on $D$. Smooth implicit roots have their stated meaning. [[math:def-local-and-global-flow]] [[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]] [[math:thm-parametrized-implicit-function-theorem-with-higher-regularity]]

[F3] Lorentzian metric and Killing-field conventions are fixed by the geometric interface. [[def-stationary-lorentzian-data]]

[F4] Use the ZFC convention already inherited from the stationary Lorentzian data and the boost lemma. In particular, the axiom of choice supplies the countable choice assumed by the pushforward interface: for a sequence of nonempty sets, a choice function on its family of values composed with the sequence selects an element of each set. For a diffeomorphism $H:M\to N$ and a smooth field $V$, its smooth pushforward is defined by $(H_*V)_{H(p)}=dH_p(V_p)$. Here $H=\mathcal F$ after step 2.1, or a time map of the complete stationary flow, so both $H$ and its inverse are smooth. [[def-stationary-lorentzian-data]] [[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]] [[math:def-axiom-of-choice]] [[math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism]]

[F5] For a smooth tensor and a smooth vector field, vanishing Lie derivative is equivalent to invariance on each common local flow domain. This applies to each smooth metric $g_q$ and to $T$, and also to a local Killing field where it is defined. For a smooth map $H$ and a covariant two-tensor $g$, $(H^*g)_p(v,w)=g_{H(p)}(dH_pv,dH_pw)$; applying the chain rule to this formula gives $(H\circ J)^*g=J^*H^*g$. [[math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes]] [[math:def-pullback-of-a-covariant-tensor-field]]

## Proof

**Given:**The stated data and complete hypotheses.

**Goal:** Establish the conclusions on the domains and parameter ranges specified.

1.1 On the formal model define $\mathsf T=\partial_\tau-\Omega Z_S$. Its orbit is $(r,\tau+t,\psi_{-\Omega t}y)$. By [F1] it meets the reference graph once, at a smooth time $t_0(r,\tau,y)$, with $|\tau+t_0|\le A$. Denote that actual reference point by $x_0\in C$ and define $\mathcal F(r,\tau,y)=\phi_{-t_0}^T(x_0)$. The complete actual $T$ flow makes this defined for every real $\tau$. Shrink $r_0$ so all graph points and all segments between graph rapidities lie in the original tube: their rapidities have absolute value at most $A$, so their normal sizes are bounded by a constant times $r_0e^{\kappa A}$. [given, F1, F2]

2.1 The map to stationary-product data $(r,\tau,y)\mapsto(-t_0,x_0)$ is a diffeomorphism onto $\mathbb R\times Q$, where $Q$ is the reference collar. Indeed formal $\mathsf T$ flow recovers the original formal point uniquely from a graph point and elapsed time; the root is smooth and transverse. The actual stationary product is injective, so $\mathcal F$ is a diffeomorphism onto the open saturation $D_0=\bigcup_t\phi_t^T(Q)$. On a sufficiently small actual tube it agrees with the normal-coordinate map: its path to the graph has rapidity between the starting rapidity and the bounded graph value, so stays in a larger fixed tube; both the normal-coordinate path and the actual $T$-flow path are integral curves of the smooth field $T$ with the same reference value $x_0$. Local uniqueness from [F2], continued along their common time segment, gives equality. This also excludes inconsistent returns after leaving the local neighborhood, rather than assuming such returns absent. [F1, F2, step 1.1]

3.1 On the formal model let $A_s(r,\tau,y)=(r,\tau+s,y)$, $B_s(r,\tau,y)=(r,\tau,\psi_s y)$ and $H_t(r,\tau,y)=(r,\tau+t,\psi_{-\Omega t}y)$. These are commuting global flows, and $B_s$ has the supplied circle period. Uniqueness of the graph intersection gives $t_0(H_t p)=t_0(p)-t$ and $x_0(H_t p)=x_0(p)$, so $\mathcal F\circ H_t=\phi_t^T\circ\mathcal F$. Differentiating at zero identifies $\mathcal F_*\mathsf T=T$. Define the extended fields $K=\mathcal F_*\partial_\tau$ and $Z=\mathcal F_*Z_S$ by [F4]. Differentiating the conjugated maps $\mathcal F\circ A_s\circ\mathcal F^{-1}$ and $\mathcal F\circ B_s\circ\mathcal F^{-1}$ shows they are their global flows. Thus the fields are complete, commute with each other and with $T$, and $Z$ retains the same circle period. By step 2.1 they agree with the original fields on an open tube about $Q$. [F1, F2, F4, step 1.1, step 2.1]

4.1 Fix a metric parameter $q$. Stationarity and [F5] give $(\phi_t^T)^*g_q=g_q$ for all real $t$: the complete flow has common domain $D$ for every time, or equivalently the local invariance identities compose along any finite time segment. Let $X$ be either extended field from step 3.1 and let $\chi_s$ be its global flow. Given $x\in D_0$, write $x=P(x_0)$ with $x_0\in Q$ and $P=\phi_t^T$. On a neighborhood $U$ of $x_0$ in the original tube, $X$ is the original Killing field. For sufficiently small $s$ and after restricting $U$, its flow stays in that tube, so [F5] gives $\chi_s^*g_q=g_q$ on $U$. Step 3.1 gives $P\circ\chi_s=\chi_s\circ P$, hence near $x$ the flow is $P\circ\chi_s\circ P^{-1}$. The pullback composition formula gives $\chi_s^*g_q=(P^{-1})^*\chi_s^*P^*g_q=(P^{-1})^*g_q=g_q$ on $P(U)$. Differentiating at $s=0$ using [F3] proves $\mathcal L_Xg_q=0$ near $x$. Since $x$ and $q$ were arbitrary, both extended fields are Killing for every $g_q$ throughout $D_0$. No extension beyond $D_0$ was used. [F2, F3, F5, step 2.1, step 3.1] ∎

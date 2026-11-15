---
id: lem-author-40aff34b4a4e-chronological-exterior-connectivity
title: Connectedness and causal convexity of a chronological exterior
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-causal-curves-and-reachability
  - math:def-axiom-of-choice
  - physics:lem-gr-push-up-rule
  - physics:lem-gr-chronology-openness
  - math:def-local-and-global-flow
  - math:prop-topological-manifolds-are-locally-compact-and-locally-path-connected
  - math:thm-connected-and-locally-path-connected-implies-path-connected
  - math:thm-choice-implies-dependent-implies-countable-choice
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  physics:lem-gr-push-up-rule: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  math:prop-topological-manifolds-are-locally-compact-and-locally-path-connected: mathematical-premise
  math:thm-connected-and-locally-path-connected-implies-path-connected: mathematical-premise
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 2
---

## Statement

Work in ZFC. Let $U$ be a nonempty connected open region in a time-oriented smooth Lorentzian four-manifold $(D,g,N)$. Let $T$ be a smooth vector field whose flow restricts to a smooth global flow $\Phi:\mathbb R\times U\to U$ of $T|_U$. Thus the line through $u\in U$ is $t\mapsto\Phi(t,u)$, with $\Phi(0,u)=u$ and $\partial_t\Phi(t,u)=T_{\Phi(t,u)}$. No causal character of $T$ on $U$ is required. Take all chronological relations in $D$, and set $A=I_D^-(U)$, $B=I_D^+(U)$ and $E=A\cap B$. Then $U\subset E$, $E$ is path connected, and every causal segment in $D$ with endpoints in $E$ stays in $E$.

## Statement references

[[physics:def-gr-smooth-lorentzian-objects]]

[[def-causal-exterior-and-boundary-data]]

[[physics:def-gr-causal-curves-and-reachability]]

[[math:def-local-and-global-flow]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

[F1] ZFC includes the Axiom of Choice, which implies Dependent Choice and Countable Choice. These inherited principles meet the choice hypotheses of the chronological openness and push-up suppliers; no simultaneous selection of paths indexed by all exterior points is needed. [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]]

[F2] The smooth Lorentzian interface supplies smooth metric coefficients and a smooth future timelike orientation field $N$. The sets $I_D^\pm(U)$ have the causal-exterior interface's meanings for any open $U$, without requiring it to be a timelike stationary end. The global-flow interface supplies the stated flow notation and integral-curve laws. The curve interface defines future timelike and causal curves and their reachability relations; smooth future timelike curves satisfy that convention. [[physics:def-gr-smooth-lorentzian-objects]] [[def-causal-exterior-and-boundary-data]] [[math:def-local-and-global-flow]] [[physics:def-gr-causal-curves-and-reachability]]

[F3] A topological manifold has a basis of open path-connected neighborhoods. A connected locally path-connected topological space is path connected. [[math:prop-topological-manifolds-are-locally-compact-and-locally-path-connected]] [[math:thm-connected-and-locally-path-connected-implies-path-connected]]

[F4] The push-up rule gives $a\ll b\le c\Rightarrow a\ll c$ and $a\le b\ll c\Rightarrow a\ll c$ in the smooth Lorentzian model. Here $\le$ includes equality and $\ll$ implies $\le$, by the curve convention, so these rules also give chronological transitivity. [[physics:lem-gr-push-up-rule|Push-up rule]] [[physics:def-gr-causal-curves-and-reachability]]

[F5] Chronological futures and pasts of individual points are open. Their unions $I_D^+(U)$ and $I_D^-(U)$ are therefore open in $D$. [[physics:lem-gr-chronology-openness]] [[physics:def-gr-causal-curves-and-reachability]]

## Proof

**Given:** The open-region and global-flow data in the Statement, in ZFC.

**Goal:** Prove inclusion of $U$, path connectedness of $E$, and causal convexity in $D$.

1.1 Fix $u\in U$ and choose a smooth chart $x$ around $u$ contained in $U$. Write $v$ for the coordinate components of $N_u$, and extend them as a constant-component vector field $V$ on the chart. At $u$, both $g(V,V)$ and $g(V,N)$ are negative. Smoothness and continuity make both inequalities remain negative on a smaller neighborhood of $u$. For sufficiently small $\varepsilon>0$, the straight coordinate segment $\gamma(s)=x^{-1}(x(u)+sv)$, $-\varepsilon\le s\le\varepsilon$, lies in that neighborhood and has velocity $V$. It is a smooth future timelike curve in $U$, so $\gamma(-\varepsilon)\ll_D u\ll_D\gamma(\varepsilon)$. Both endpoints belong to $U$, giving $u\in B\cap A$. Thus $U\subset E$, without any sign assumption on $T$. Also $A$ and $B$, and hence $E$, are open by chronological openness. The choice assumptions needed for that supplier follow from ZFC. [given, F1, F2, F5]

1.2 Since $U$ is open in $D$, every open neighborhood $V$ of a point $u$ in $U$ is also open in $D$. The manifold neighborhood basis supplies an open path-connected neighborhood $W$ with $u\in W\subset V$. Thus $U$ is locally path connected in its subspace topology. It is connected by hypothesis, so the connected locally path-connected theorem makes $U$ path connected. [given, F3]

1.3 Orient a causal segment with endpoints $p,q\in E$ from $p$ to $q$, and let $z$ be any point on it. The segment restrictions give $p\le_D z\le_D q$, allowing equality at endpoints. By the definitions of $B$ and $A$, choose $u_-,u_+\in U$ with $u_-\ll_D p$ and $q\ll_D u_+$. The two push-up implications give $u_-\ll_D z$ and $z\ll_D u_+$. Therefore $z\in B\cap A=E$, proving causal convexity. The choice assumptions of push-up are supplied by ZFC. [given, F1, F2, F4]

2.1 Given $p_0,p_1\in E$, choose $q_0,q_1\in U$ and future timelike curves from $p_i$ to $q_i$, as permitted by $p_i\in A$. Their endpoints belong to $E$ by step 1.1, so their images lie in $E$ by step 1.3. Step 1.2 supplies a continuous path inside $U\subset E$ from $q_0$ to $q_1$. Traverse the first timelike curve, this path, and the reverse of the second timelike curve. Reparametrizing the three continuous curves onto three consecutive closed subintervals gives a continuous path in $E$ from $p_0$ to $p_1$, since the endpoint values agree at the two joins. This proves path connectedness and completes all three claims. [F2, step 1.1, step 1.2, step 1.3] ∎

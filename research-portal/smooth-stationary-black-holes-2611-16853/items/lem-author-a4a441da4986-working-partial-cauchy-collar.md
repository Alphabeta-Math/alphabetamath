---
id: lem-author-a4a441da4986-working-partial-cauchy-collar
title: A working partial-Cauchy collar satisfies the source GR section equalities
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-a4a441da4986-doc-connected-and-causally-convex
  - lem-author-a4a441da4986-cauchy-closure-double-boundary
  - lem-author-a4a441da4986-exact-outer-cauchy-section
  - lem-author-a4a441da4986-stationary-end-future-orientation
  - def-regular-stationary-vacuum-spacetime
  - math:thm-flowout-theorem
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - def-causal-exterior-and-boundary-data
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-push-up-rule
  - physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets
  - physics:lem-gr-maximal-geodesics-and-extension
  - physics:lem-gr-partial-cauchy-development
dependency_roles:
  lem-author-a4a441da4986-doc-connected-and-causally-convex: mathematical-premise
  lem-author-a4a441da4986-cauchy-closure-double-boundary: mathematical-premise
  lem-author-a4a441da4986-exact-outer-cauchy-section: mathematical-premise
  lem-author-a4a441da4986-stationary-end-future-orientation: mathematical-premise
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  math:thm-flowout-theorem: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-push-up-rule: mathematical-premise
  physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets: mathematical-premise
  physics:lem-gr-maximal-geodesics-and-extension: mathematical-premise
  physics:lem-gr-partial-cauchy-development: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 4
---

## Statement

Under the article regular hypotheses, there is an open working spacetime $M'\subset M$ containing the whole exterior $E$ and a neighborhood of $S$, with the restricted metric and Killing field, and an embedded acausal edgeless section $\Sigma'\cong\{r>1/2\}$ agreeing with $C=\Sigma_0\cap E$ on its outer side and with the original section near $S$, such that
$$\Sigma'\cap I^+_{M'}(M^{\rm end})=\Sigma'\cap I^-_{M'}(M^{\rm end})=C=\{r>1\}.$$
The domain of outer communications of the same selected end in $M'$ is exactly $E$. The full chronological boundary intersection in the working spacetime is
$$\partial_{M'}I^-_{M'}(M^{\rm end})\cap\partial_{M'}I^+_{M'}(M^{\rm end})=S.$$
This supplies a working partial Cauchy hypersurface and the source section equalities; it does not assume an ambient complete stationary flow or a stationary product.

## Statement references

[[lem-author-a4a441da4986-doc-connected-and-causally-convex]]

[[lem-author-a4a441da4986-cauchy-closure-double-boundary]]

[[lem-author-a4a441da4986-exact-outer-cauchy-section]]

[[lem-author-a4a441da4986-stationary-end-future-orientation]]

[[def-regular-stationary-vacuum-spacetime]]

[[math:thm-flowout-theorem]]

[[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[[def-causal-exterior-and-boundary-data]]

[[physics:lem-gr-chronology-openness]]

[[physics:lem-gr-push-up-rule|Push-up rule]]

[[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]

[[physics:lem-gr-maximal-geodesics-and-extension]]

[[physics:lem-gr-partial-cauchy-development]]

## Facts & Assumptions

[F1] The declared geometry, causal, operator and earlier-result inputs are [[lem-author-a4a441da4986-doc-connected-and-causally-convex]] [[lem-author-a4a441da4986-cauchy-closure-double-boundary]] [[lem-author-a4a441da4986-exact-outer-cauchy-section]] [[lem-author-a4a441da4986-stationary-end-future-orientation]] [[def-regular-stationary-vacuum-spacetime]] [[math:thm-flowout-theorem]] [[math:thm-smooth-inverse-function-theorem-on-manifolds]] [[def-causal-exterior-and-boundary-data]] [[physics:lem-gr-chronology-openness]] [[physics:lem-gr-push-up-rule|Push-up rule]]

[F2] Acausality means that no two distinct points of the set are causally related, and a Cauchy set counts exactly one parameter value on every inextendible causal curve. These are clauses (b) and (c) of [[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]. Clause (d) of [[physics:lem-gr-maximal-geodesics-and-extension]] makes every such Cauchy set acausal. Apply it in the open restricted spacetime $E$ to $C$, with the matching curve and inextendibility conventions of [[def-causal-exterior-and-boundary-data]]. The ZFC convention of [[def-regular-stationary-vacuum-spacetime]] supplies the choice assumptions of the causal and flowout inputs.

[F3] For a closed hypersurface $A$ in an ambient spacetime $W$, edgelessness means that no $p\in A$ has this property: every open neighborhood $U$ of $p$ admits $a\in I^-_U(p)$, $b\in I^+_U(p)$ and a timelike curve in $U$ from $a$ to $b$ avoiding $A$. Use the explicit definition in the Statement of [[physics:lem-gr-partial-cauchy-development]], with $A=\Sigma'$ and $W=M'$. Only this definition is used, not the supplier's domain-of-dependence conclusions.

[F4] Chronological sets are open in $M$ and in every open restricted spacetime, including $M'$, by clauses (a) and (b) of [[physics:lem-gr-chronology-openness]]. Clause (c) says that the chronological past of any point in the closure of a past set lies in that past set, with the dual assertion for a future set. The chronological sets $I^\pm_{M'}(U)$ are past/future sets by the push-up implications in [[physics:lem-gr-push-up-rule|Push-up rule]]. The causal-exterior interface fixes ambient closures and boundaries; the ZFC convention in [F2] supplies the inherited choice assumptions. [[def-causal-exterior-and-boundary-data]]

## Proof

**Given:** The exact outer section, compact boundary, two-sided end access, local transverse null boundaries and flowout interfaces of [F1], with the acausality and edge conventions of [F2] and [F3].

**Goal:** Match the source section data by a bounded working neighborhood and prove the full double-boundary identity there.

1.1 Each smooth null boundary restricts transversely to the spacelike original section: its null conormal cannot annihilate a spacelike three-plane. Near compact $S$, the two restricted surfaces are both precisely $S$. The outer side is $C$ and belongs to both chronological sets. Their past/future-set orientations then put the inner side in neither chronological set. This is the local bifurcation quadrant determined by the actual chronological boundaries, rather than a conclusion from Killing tangency alone. Take a thin flowout $O$ of the compact annular section collar along a future timelike field, small enough that its inverse time coordinate has timelike differential. Its zero level is the original section there, and its inner annular endpoints lie outside $O$. [given, F1]

2.1 Set $M'=E\cup O$ and $\Sigma'=C\cup S$ together with the inner section collar in $O$. An inner collar point cannot be causally related to an $E$ point in either direction: composing such a relation with the timelike access of the $E$ point to or from the end would put the collar point in one of the two original chronological sets, contrary to step 1.1. The same argument excludes causal relations between $S$ and $E$. Thus any causal relation between inner collar or $S$ points in $M'$ must stay inside $O$, where the temporal flowout coordinate forbids a return to its zero level. Causal relations between $C$ points remain in $E$ by causal convexity, and are excluded because $C$ is Cauchy in $E$ and hence acausal by [F2]. Therefore $\Sigma'$ is acausal in $M'$. [given, F1, F2, step 1.1]

3.1 It is smooth and spacelike, closed in $M'$ because $C$ is closed in $E$, its only additional ambient closure points are on $S$, and the open inner collar endpoints have been excluded from $M'$. Thus it remains to check the local edge condition. [given, F1, step 1.1, step 2.1]

4.1 Fix $p\in\Sigma'$. A local transverse timelike flowout and the inverse function theorem in [F1] give an open neighborhood $U\subset M'$ and a smooth coordinate $u$ with $u(p)=0$ and $\Sigma'\cap U=\{u=0\}$. At the section, $du$ annihilates its spacelike tangent planes, so its metric dual is timelike; choose its sign to increase in the future and shrink $U$ to keep it timelike throughout. Consequently $u$ strictly increases on future timelike curves in $U$. If $a\in I^-_U(p)$ and $b\in I^+_U(p)$, then $u(a)<0<u(b)$. Every timelike curve in $U$ from $a$ to $b$ has continuous $u$-coordinate and therefore meets $\{u=0\}=\Sigma'\cap U$. This neighborhood excludes the property in [F3] at $p$. Since $p$ was arbitrary and $\Sigma'$ is closed by step 3.1, the section is edgeless. [given, F1, F3, step 3.1]

5.1 Choose the adapted topological radial identification $\widetilde j$ of the original section supplied by the exact-outer-section lemma in [F1], so $\widetilde j(C)=\{|y|>1\}$ and $\widetilde j(S)=\{|y|=1\}$; this may require its permitted radial inversion of the originally specified identification. Use its radial coordinate near $S$ for the inner section collar in step 1.1, shrinking that collar if necessary. Reparametrize only the inner collar radially to obtain an identification of $\Sigma'$ with $\{|y|>1/2\}$, retaining $\widetilde j$ on $C$ and taking $C$ to $\{|y|>1\}$. The $r$ in the displayed section equalities denotes the radius of this chosen identification. The physical stationary end chart on $C$ is retained as separate data; no agreement with $\widetilde j$ is asserted. The selected end lies in $E$. Every $E$ point retains both timelike end connections inside $M'$, while a new DOC point would also be an old DOC point in $M$. Hence the new DOC is exactly $E$, and the inner section collar is in neither new chronological set. Both displayed section equalities follow. The new local horizon boundaries and their double intersection remain the old two sheets and $S$, since the local black/white quadrants have the corresponding one-sided timelike access through $E$. [given, F1, step 1.1, step 2.1, step 3.1, step 4.1]

6.1 Write $U=M^{\rm end}$, $A_\pm=I^\pm_M(U)$ and $A'_\pm=I^\pm_{M'}(U)$. Every curve in $M'$ is a curve in $M$, so $A'_\pm\subset M'\cap A_\pm$. These sets are open in their respective ambient spacetimes; in $M'$, $A'_+$ is a future set and $A'_-$ is a past set. Step 5.1 gives $A'_+\cap A'_-=E=A_+\cap A_-$. If $p\in\partial_{M'}A'_+\cap\partial_{M'}A'_-$, openness puts $p$ outside both primed sets and in the closure of each, with closures taken in $M'$. [F4, step 5.1]

7.1 Suppose such a point $p$ belongs to $A_+$. Since $A_+$ and $M'$ are open, a sufficiently short past segment of a local future timelike curve through $p$ has initial point $a\in A_+\cap M'$ with $a\ll_{M'}p$. Such a segment exists by taking a timelike direction in a smooth chart and shrinking the straight segment until the metric and time orientation keep it future timelike. Because $p$ lies in the closure of the past set $A'_-$, [F4] gives $a\in A'_-\subset A_-$. Thus $a\in A_+\cap A_-=E\subset A'_+$. The future-set property and $a\ll_{M'}p$ imply $p\in A'_+$, contradicting step 6.1. Hence $p\notin A_+$. [F1, F4, step 6.1]

8.1 Reverse time in step 7.1: if $p\in A_-$, take $b\in A_-\cap M'$ with $p\ll_{M'}b$. Since $p$ is in the closure of the future set $A'_+$, [F4] gives $b\in A'_+\subset A_+$, hence $b\in E\subset A'_-$. The past-set property forces $p\in A'_-$, again a contradiction. Therefore $p\notin A_-$. Since $p$ lies in both primed closures, the inclusions of step 6.1 put it in both original closures in $M$. Exclusion from the original open sets gives $p\in\partial_M A_+\cap\partial_M A_-=S$ by the original regularity hypothesis. This proves that the full new double boundary is contained in $S$. [F1, F4, step 6.1, step 7.1]

9.1 Conversely, the exact-outer-section supplier in [F1] gives $B=C\cup S$ as a smooth embedded manifold with boundary $S$ and interior $C$. In a boundary chart of $B$, positive values of the boundary-normal coordinate give points of $C$ converging to each boundary point. Since $M'$ contains $C\subset E$ and a neighborhood of $S$, these same curves show that every point of $S$ lies in the closure of $E$ in $M'$. This uses no identification of a topological radial coordinate with the physical end radius. By step 6.1, $E\subset A'_+\cap A'_-$. The original double-boundary hypothesis excludes $S$ from the open original sets $A_\pm$, hence also from $A'_\pm$. Thus $S\subset\partial_{M'}A'_+\cap\partial_{M'}A'_-$. Together with step 8.1 this proves the claimed global equality, completing the section and boundary conclusions. [F1, F4, step 5.1, step 6.1, step 8.1] ∎

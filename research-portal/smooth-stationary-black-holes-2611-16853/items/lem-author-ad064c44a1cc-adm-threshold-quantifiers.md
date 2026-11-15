---
id: lem-author-ad064c44a1cc-adm-threshold-quantifiers
title: Quantifiers and parameter gap in the ADM smallness hypothesis
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-ad064c44a1cc-adm-gr-sbs
  - def-author-ad064c44a1cc-adm-angular-momentum-parameters
  - def-author-ad064c44a1cc-adm-maximal-section
  - def-author-ad064c44a1cc-adm-effective-geometry
  - physics:def-gr-fx-kerr-exterior
  - def-author-ad064c44a1cc-weighted-mars-simon
dependency_roles:
  def-author-ad064c44a1cc-adm-gr-sbs: mathematical-premise
  def-author-ad064c44a1cc-adm-angular-momentum-parameters: mathematical-premise
  def-author-ad064c44a1cc-adm-maximal-section: mathematical-premise
  def-author-ad064c44a1cc-adm-effective-geometry: mathematical-premise
  physics:def-gr-fx-kerr-exterior: mathematical-premise
  def-author-ad064c44a1cc-weighted-mars-simon: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 7
---

## Statement

In mass-one Radu ADM data with $J<1$, for any supplied positive threshold function $j(A)$, the quantitative application predicate at fixed $A$ is $\overline A_{\rm ADM}\le A$ and $J<j(A)$. A theorem asserting existence of a suitable threshold uses the order: first fix $A$, then choose a positive threshold uniformly for data with that bound. The geometric bound implies $A\ge1$ and $J\le1-A^{-1}$. Hence it is a simultaneous geometric and angular-momentum condition, not the statement that a universal numerical angular tolerance works for every geometry. These algebraic consequences do not prove a Kerr conclusion. Any Kerr rigidity implication would require a separately supplied theorem under its complete hypotheses, including GR/SBS and maximality; no rigidity theorem is an input to this lemma.

For these comparisons, the horizon scalar is $H=\sup_{p\in S_0}|g_p(T_p,T_p)|$ on the supplied bifurcation sphere. When its own defining Ernst/curvature data are supplied, $\mathcal W$ denotes the smooth weighted Mars–Simon tensor. A Kerr conclusion means an isometry of the exterior to the subextremal Kerr exterior with parameters $M=1$ and $a=J$, using the target definition's stated countable-choice convention. No bound for $H$ or $\mathcal W$ is asserted here.

## Facts & Assumptions

[F1] [[def-author-ad064c44a1cc-adm-gr-sbs]] specifies GR/SBS, including $g,T,S_0$, [[def-author-ad064c44a1cc-adm-angular-momentum-parameters]] defines the nonnegative mass-one $J$, and [[def-author-ad064c44a1cc-adm-maximal-section]] specifies the separate maximality condition.

[F2] [[def-author-ad064c44a1cc-adm-effective-geometry]] puts $(1-J)^{-1}$ among the entries of $\overline A_{\rm ADM}$.

[F3] [[physics:def-gr-fx-kerr-exterior]] defines the subextremal Kerr target under its stated countable-choice convention. [[def-author-ad064c44a1cc-weighted-mars-simon]] defines $\mathcal W$ on its supplied smooth potential/tensor domain, including points where the unweighted formula would divide by zero. These are formulation inputs for the comparisons only; supplying ADM data does not silently supply the additional Ernst/curvature data.

## Proof

**Given:** Mass one, $0\le J<1$ and the finite geometric bound in the Statement.

**Goal:** Identify its scalar consequences and the order of its quantitative choices.

1.1 Since $0<1-J\le1$, its inverse is at least one. From [F2], $1\le(1-J)^{-1}\le\overline A_{\rm ADM}\le A$, giving $A\ge1$. Multiplying the positive inequality $(1-J)^{-1}\le A$ by $1-J$ and then dividing by positive $A$ gives $J\le1-A^{-1}$. [given, F1, F2, algebra]

2.1 Suppose a theorem is supplied with quantifier order $\forall A>0\ \exists j_A>0\ \forall d$, followed by the implication that $\overline A_{\rm ADM}(d)\le A$ and $J(d)<j_A$ give a specified conclusion $C(d)$, where $d$ ranges over mass-one data satisfying all its other hypotheses. This order fixes $A$ before selecting the threshold, which is then uniform over those data at that bound; it does not assert one positive threshold uniform over all $A$. For each application both inequalities must still be checked. In particular fixing one geometry with $\overline A_{\rm ADM}\le A$ does not delete that hypothesis from the implication. Step 1.1 supplies its scalar parameter gap. No existence of such a theorem or rigidity threshold is proved or assumed here. No estimate for either comparison object in [F3], and no Kerr rigidity implication, is part of this argument. [given, F1, F2, F3, step 1.1, algebra] ∎

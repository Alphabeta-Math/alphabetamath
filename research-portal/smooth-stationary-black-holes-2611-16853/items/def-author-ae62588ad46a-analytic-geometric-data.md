---
id: def-author-ae62588ad46a-analytic-geometric-data
title: Geometric data for the analytic multiple-horizon comparison
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-black-hole-comparison-hypothesis-data
  - def-horizon-rotation-surface-gravity
  - def-causal-exterior-and-boundary-data
  - math:def-axiom-of-choice
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-black-hole-comparison-hypothesis-data: mathematical-premise
  def-horizon-rotation-surface-gravity: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 5
---

## Definition

Work in ZFC. Analytic geometric comparison data consist of the stationary Lorentzian four-manifold $(M,g,T)$, a selected spacelike asymptotically flat end and a time orientation. The metric is analytic and satisfies $\operatorname{Ric}(g)=0$. The field $T$ is complete, future timelike near the end and normalized by $g(T,T)\to-1$. The end has induced metric $h_{ij}-\delta_{ij}=O_k(r^{-\alpha})$ and second fundamental form $k_{ij}=O_{k-1}(r^{-1-\alpha})$ for some $\alpha>0$ and integer $k>1$, in the comparison convention of [[def-black-hole-comparison-hypothesis-data]]. The notation $O_k(r^{-b})$ means that spatial derivatives of order $j\le k$ are bounded by a constant times $r^{-b-j}$.

Require precisely that comparison definition's $I^+$-regularity: the flow-saturated end $M_{\rm ext}$ determines $D=I_M^+(M_{\rm ext})\cap I_M^-(M_{\rm ext})$; $D$ is globally hyperbolic; and a spacelike connected acausal section containing the selected end has a completion with compact core and finitely many asymptotic ends, whose boundary lies on the future horizon and meets its generators precisely once. No connectedness or nondegeneracy of the entire horizon is imposed. The stronger canonical end form used by a cited source is a conclusion of a separate asymptotic input, not an additional requirement in this definition.

Horizon terminology is conditional on the additional data required by the horizon interface. On a component $H$ supplied as a smooth null hypersurface, non-rotation means that $T_p$ belongs to the null normal line at every $p\in H$; rotation means failure of this condition somewhere. For the degeneracy convention, additionally supply a Killing field $K$ on a neighborhood of $H$, with its scale fixed as part of the supplied data. Require $H_*=\{p\in H:K_p\ne0\}$ to be nonempty and dense, and $K$ to be tangent and normal on $H_*$. When its signed surface-gravity function, defined by $d(g(K,K))=-2\kappa_H K^\flat$ on $H_*$, is constant with value $\kappa\ge0$, call this Killing horizon degenerate if $\kappa=0$ and non-degenerate if $\kappa>0$, as in [[def-horizon-rotation-surface-gravity]]. The chosen normalization of $K$ is additional data; the normalization of $T$ alone does not specify it. These clauses define terminology only when their stated data and coefficient properties are supplied. They neither add those properties to the base analytic comparison hypotheses nor assert that $I^+$-regularity proves them; an application to the event horizon must obtain them separately before using this terminology.

## Facts & Assumptions

[F1] Stationary Lorentzian data, end decay, completed sections, global hyperbolicity and causal sets are [[def-stationary-lorentzian-data]], [[def-black-hole-comparison-hypothesis-data]] and [[def-causal-exterior-and-boundary-data]]. The compatible real-analytic atlas and analytic-metric convention are already specified in [[def-black-hole-comparison-hypothesis-data]]. Rotation and surface-gravity conventions, with their smooth-null-hypersurface, specified-generator and coefficient hypotheses, are [[def-horizon-rotation-surface-gravity]]. Choice is allowed through [[math:def-axiom-of-choice]].

## Justification

**Given:** The supplied geometry, end, fields and section.

**Goal:** Verify that these are definite source-comparison predicates without presuming a canonical chart or a connected horizon.

1.1 The supplied metric and field determine the Ricci and Killing equations, the time orientation and the normalization limit. The chart specifies the differentiated decay conditions. The causal and section interfaces specify $M_{\rm ext}$, $D$, the completed boundary and its generator intersections. Thus each displayed condition is a predicate on the supplied objects. [given, F1]

2.1 For a component additionally supplied as a smooth null hypersurface, its null normal line makes the stated membership test for $T$ a definite predicate. For an additionally supplied Killing field $K$ with the stated nonzero, tangency and normality properties, the horizon interface supplies its signed surface-gravity function on $H_*$. Fixing $K$ fixes its scale; if its coefficient is supplied as constant and nonnegative, testing $\kappa=0$ or $\kappa>0$ gives the two stated degeneracy alternatives. Thus these are conditional horizon predicates, not predicates whose applicability to every event-horizon component follows from the base data. Their use in a subsequent classification requires that application to supply the stated horizon properties independently of this definition. No bifurcation sphere, horizon connectedness or canonical end has been inferred. [given, F1, step 1.1] ∎

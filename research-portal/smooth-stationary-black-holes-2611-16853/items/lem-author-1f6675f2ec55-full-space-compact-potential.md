---
id: lem-author-1f6675f2ec55-full-space-compact-potential
title: Compact potential multiplication without a Dirichlet restriction
kind: lemma
status: draft
origin: pipeline
domain: mathematics
proof_strategy: direct
deps:
  - math:def-axiom-of-choice
  - lem-author-1f6675f2ec55-local-holder-compactness
  - lem-author-1f6675f2ec55-weighted-potential-tail
  - math:thm-holder-spaces-on-bounded-domains-are-banach-spaces
  - def-fredholm-continuation-data
  - def-weighted-holder-spaces
  - def-exterior-weighted-elliptic-data
  - math:thm-metric-compactness-equivalences
dependency_roles:
  math:def-axiom-of-choice: mathematical-premise
  lem-author-1f6675f2ec55-local-holder-compactness: mathematical-premise
  lem-author-1f6675f2ec55-weighted-potential-tail: mathematical-premise
  math:thm-holder-spaces-on-bounded-domains-are-banach-spaces: mathematical-premise
  def-fredholm-continuation-data: mathematical-premise
  def-weighted-holder-spaces: mathematical-premise
  def-exterior-weighted-elliptic-data: mathematical-premise
  math:thm-metric-compactness-equivalences: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
dependency_level: 3
---

## Statement

Assume the Axiom of Choice and the weighted exterior chart conventions, with $0<\alpha<1$ and arbitrary real $\beta$. For every fixed $V\in C^{2,\alpha}_{-4}$, multiplication $M_V:u\mapsto Vu$ is a compact bounded linear map from the full space $C^{4,\alpha}_\beta$ to $C^{2,\alpha}_{\beta-2}$. Compact means that the image of every bounded set has compact closure in the target norm. Restricting this map to $X_\beta=\{u\in C^{4,\alpha}_\beta:u|_{\partial\Sigma}=0\}$ remains compact.

## Statement references

[[math:def-axiom-of-choice]]

[[lem-author-1f6675f2ec55-local-holder-compactness]]

[[lem-author-1f6675f2ec55-weighted-potential-tail]]

[[math:thm-holder-spaces-on-bounded-domains-are-banach-spaces]]

[[def-fredholm-continuation-data]]

[[def-weighted-holder-spaces]]

[[def-exterior-weighted-elliptic-data]]

[[math:thm-metric-compactness-equivalences]]

## Facts & Assumptions

**Given:** The hypotheses of the Statement.

**Goal:** Establish its stated analytic ingredients and qualifications.

[F1] The Axiom of Choice supplies the inherited analytic compactness assumptions. [[math:def-axiom-of-choice]]

[F2] Every bounded full-input sequence has a subsequence converging in compact-truncation $C^{2,\alpha}$ norms, without a trace condition. [[lem-author-1f6675f2ec55-local-holder-compactness]]

[F3] Multiplication by the fixed potential is bounded and has a uniform target tail of order $T^{-2}$ on bounded full-input sets. [[lem-author-1f6675f2ec55-weighted-potential-tail]]

[F4] Ordinary Hölder spaces on bounded domains are Banach spaces; Fredholm-continuation terminology defines compact linear maps by relative compactness of bounded images. Under the assumed choice axioms, compactness of a metric space is equivalent to sequential compactness. [[math:thm-holder-spaces-on-bounded-domains-are-banach-spaces]] [[def-fredholm-continuation-data]] [[math:thm-metric-compactness-equivalences]]

[F5] The weighted exterior chart norms define the full input, target and zero-Dirichlet subspace. [[def-weighted-holder-spaces]] [[def-exterior-weighted-elliptic-data]]

## Proof

1.1 The target weighted space is complete: a target-norm Cauchy sequence is Cauchy in each bounded chart Hölder norm and hence converges there. The local limits agree on overlaps. Pass the Cauchy inequalities to the limit in each derivative supremum and Hölder difference quotient and then take the annular supremum. This gives a global target element and convergence in the weighted norm. Thus the local Banach completeness patches to the given target norm. [F4, F5, algebra]

2.1 Given a bounded sequence $u_j$ in the full input space, take the locally convergent subsequence of the local-compactness lemma. Multiplication by $V$ preserves compact $C^{2,\alpha}$ convergence, by the same product inequality as in the tail lemma. For any tolerance first make the common annular tails small by choosing $T$ large, then make the subsequence products close on the compact truncation through $r=2T$. Annuli with $R<T$ lie inside that truncation and have uniformly bounded weight factors because $R\ge r_0>0$. Hence the products form a target-norm Cauchy subsequence and converge by target completeness. [F2, F3, F5, step 1.1, algebra]

3.1 Every sequence in the image of a bounded input set therefore has a convergent subsequence in the target. The metric compactness criterion gives relative compactness, which is the definition of compactness here; equivalently the same tail and compact-truncation argument supplies finite nets for the image. Boundedness and linearity were supplied by the product lemma. A bounded sequence in the Dirichlet subspace is also a bounded sequence in the full space, proving the restricted assertion. [F1, F3, F4, step 2.1] ∎

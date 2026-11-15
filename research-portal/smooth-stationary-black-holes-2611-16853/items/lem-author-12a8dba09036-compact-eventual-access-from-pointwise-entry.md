---
id: lem-author-12a8dba09036-compact-eventual-access-from-pointwise-entry
title: Pointwise eventual chronological entry is uniform on compact subsets
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - math:def-compact-space
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:thm-reals-ordered-field
  - lem-author-12a8dba09036-translated-cylinder-pasts-increase
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:lem-compactness-of-a-subspace-is-ambient: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  lem-author-12a8dba09036-translated-cylinder-pasts-increase: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

Let $A_t$ be the increasing open chronological pasts in the preceding lemma, and let $X$ be any fixed subset of the spacetime. Suppose every $p\in X$ belongs to $A_t$ for all sufficiently large $t$, with a threshold allowed to depend on $p$. Then each compact $L\subset X$ has a finite common threshold $t_L$ for which $L\subset A_t$ for every $t\ge t_L$. This is conditional on pointwise entry and supplies no missing accessibility premise.

## Statement references

[[def-causal-exterior-and-boundary-data]]

[[math:def-compact-space]]

[[math:lem-compactness-of-a-subspace-is-ambient]]

[[math:thm-reals-ordered-field]]

[[lem-author-12a8dba09036-translated-cylinder-pasts-increase]]

## Facts & Assumptions

[F1] The pasts are open and increasing in time. [[lem-author-12a8dba09036-translated-cylinder-pasts-increase]] [[def-causal-exterior-and-boundary-data]]

[F2] Compact subsets admit finite ambient open subcovers. [[math:def-compact-space]] [[math:lem-compactness-of-a-subspace-is-ambient]]

[F3] The real numbers form a totally ordered field: any two real indices are comparable, the order is transitive and compatible with addition, and $1>0$. [[math:thm-reals-ordered-field]]

## Proof

**Given:** The stated data and explicit hypotheses.

**Goal:** Establish only the asserted conditional conclusion.

1.1 Use the whole real-indexed family $(A_t)_{t\in\mathbb R}$. For each $p\in L$, the pointwise eventual-entry hypothesis supplies a real threshold $a$ such that $p\in A_t$ for every $t\ge a$; in particular $p\in A_{a+1}$. Hence $L\subseteq\bigcup_{t\in\mathbb R}A_t$. Each member is ambient open by [F1], so this is an indexed ambient open cover as in [F2]. If $L$ is nonempty, the indexed form of [F2] gives finitely many real indices $t_1,\ldots,t_k$, with $k\ge1$, such that $L\subseteq A_{t_1}\cup\cdots\cup A_{t_k}$. [given, F1, F2, F3]

2.1 If $L$ is empty take $t_L=0$. Otherwise the finitely many real indices in step 1.1 have a greatest member: start with $t_1$ and compare each subsequent index with the retained member, retaining the larger one at each of the finitely many comparisons. Call the resulting member $t_L$; then $t_L\ge t_i$ for all $i$. For every $t\ge t_L$, monotonicity gives $A_{t_i}\subseteq A_t$ when $t_i<t$, and equality handles $t_i=t$. The finite cover therefore gives $L\subseteq A_t$. This proves the asserted compact uniformity without strengthening the pointwise hypothesis or using integer cofinality. [F1, F3, step 1.1] ∎

---
id: lem-author-cf389990237c-degenerate-komar-zero-mass-implication
title: Degeneracy forces zero mass when global Komar transport applies
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-cf389990237c-normalized-horizon-komar-data
  - lem-author-cf389990237c-constant-gravity-horizon-komar-integral
dependency_roles:
  def-author-cf389990237c-normalized-horizon-komar-data: mathematical-premise
  lem-author-cf389990237c-constant-gravity-horizon-komar-integral: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 5
---

## Statement

For the normalized nonrotating horizon data of [[def-author-cf389990237c-normalized-horizon-komar-data]], assume the additional, separately established global identity $M_K=Q_C[T]$. If $\kappa=0$, then $M_K=0$. In particular, an independent theorem forbidding zero mass in the specified black-hole class excludes such a configuration. The local horizon evaluation is [[lem-author-cf389990237c-constant-gravity-horizon-komar-integral]]; this lemma does not establish the global identity, an admissible completion for positive mass, or the exclusion theorem.

## Facts & Assumptions

[F1] Use the normalized functional and its constant-gravity evaluation. The exterior identity and any zero-mass exclusion are separate explicit hypotheses, not consequences of a local cross-section calculation. [[def-author-cf389990237c-normalized-horizon-komar-data]] [[lem-author-cf389990237c-constant-gravity-horizon-komar-integral]]

## Proof

**Given:**The local data, $M_K=Q_C[T]$ and degeneracy $\kappa=0$.

**Goal:** Derive the stated conditional zero-mass implication.

1.1 The constant-gravity integral yields $Q_C[T]=0\cdot A_C/(4\pi)=0$. The supplied equality then gives $M_K=0$. [given, F1]

2.1 If a separately applicable theorem excludes zero mass for the specified black-hole class, the equality in step 1.1 contradicts that theorem. This is a conditional implication and leaves every global applicability obligation with that separately supplied theorem. [given, F1, step 1.1] ∎

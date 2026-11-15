---
id: lem-author-9e5789a3d617-exterior-exclusion-interface
title: Black and white exclusion is an ambient reachability condition
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

In a time-oriented spacetime $M$, fix a union of stationary end regions $M_{\rm ext}$ and any subset $U\subset M$. Define $B=M\setminus I_M^-(M_{\rm ext})$ and $W=M\setminus I_M^+(M_{\rm ext})$. Then $(B\cup W)\cap U=\varnothing$ if and only if $U\subset I_M^-(M_{\rm ext})\cap I_M^+(M_{\rm ext})$. For any subset $\Sigma\subset M$, define $D(\Sigma)$ here to be the set of points through which every inextendible timelike curve in $M$ meets $\Sigma$. The equivalence applies in particular to $U=\operatorname{int}D(\Sigma)$ with this explicit local convention. The chronological relations are computed in $M$; changing the ambient spacetime requires recomputing them.

## Facts & Assumptions

[F1] Chronological past and future use future timelike curves in the specified ambient manifold. [[def-causal-exterior-and-boundary-data]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated construction and identities.

1.1 The equality $(B\cup W)\cap U=\varnothing$ means simultaneously that $U\cap B$ and $U\cap W$ are empty. Taking complements in $M$ gives $U\subset I_M^-(M_{\rm ext})$ and $U\subset I_M^+(M_{\rm ext})$. Their conjunction is precisely the stated inclusion. [F1]

2.1 Conversely the inclusion excludes every point of $U$ from each complement, so it excludes their union. This set argument holds for any $U$, in particular the interior of the domain of dependence defined above; it neither identifies that domain with a desired exterior nor changes timelike-curve domains of dependence to a different convention. [F1, step 1.1] ∎

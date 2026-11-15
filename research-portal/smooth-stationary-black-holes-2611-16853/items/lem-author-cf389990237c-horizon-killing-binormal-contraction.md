---
id: lem-author-cf389990237c-horizon-killing-binormal-contraction
title: Killing-horizon derivative contracted with the binormal
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-cf389990237c-normalized-horizon-komar-data
  - lem-author-cf389990237c-normal-binormal-boost-invariance
  - physics:thm-gr-killing-and-on-shell-matter-identities
dependency_roles:
  def-author-cf389990237c-normalized-horizon-komar-data: mathematical-premise
  lem-author-cf389990237c-normal-binormal-boost-invariance: mathematical-premise
  physics:thm-gr-killing-and-on-shell-matter-identities: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

For the nonrotating normalized horizon data of [[def-author-cf389990237c-normalized-horizon-komar-data]], one has $(\nabla^aT^b)b_{ab}=-2\kappa$ pointwise on $C$. The sign is fixed by its specified binormal, which is unchanged by the boosts in [[lem-author-cf389990237c-normal-binormal-boost-invariance]]. Use the antisymmetric Killing equation in [[physics:thm-gr-killing-and-on-shell-matter-identities]].

## Facts & Assumptions

[F1] Along the section $T=c(n+s)$ with $c>0$, $\nabla_TT=\kappa T$, and the bilinear form $A(U,V)=g(\nabla_UT,V)$ is antisymmetric. The binormal convention is fixed by the normalized-data item and boost lemma. [[def-author-cf389990237c-normalized-horizon-komar-data]] [[lem-author-cf389990237c-normal-binormal-boost-invariance]] [[physics:thm-gr-killing-and-on-shell-matter-identities]]

## Proof

**Given:**The section and Killing generator in the Statement.

**Goal:** Compute the binormal contraction.

1.1 Contract $\nabla_TT=\kappa T$ with $n$. Since $T=c(n+s)$ and $A(n,n)=0$, this gives $cA(s,n)=-\kappa c$, so $A(s,n)=-\kappa$. Antisymmetry gives $A(n,s)=\kappa$. No derivative of $c$ is taken: the first derivative slot is pointwise linear in its vector argument. [given, F1]

2.1 By the definition of $b$, $(\nabla^aT^b)b_{ab}=A(s,n)-A(n,s)=-2\kappa$. The boost lemma makes the computation independent of the chosen oriented orthonormal normal pair. [F1, step 1.1] ∎

---
id: lem-author-4cb89398a4ab-chronological-equivariance
title: Chronological equivariance and the no-white-hole condition
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - lem-author-4cb89398a4ab-complete-end-saturation
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  lem-author-4cb89398a4ab-complete-end-saturation: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 4
---

## Statement

Use the chronological relations of [[def-causal-exterior-and-boundary-data]]. If a time-orientation-preserving isometry $\psi$ satisfies $\psi(E)=E$, then $\psi(I^\pm(E))=I^\pm(E)$ and $\psi(\partial I^\pm(E))=\partial I^\pm(E)$. In particular this applies to every $\phi_v$ and $E=M_{\mathrm{end}}$ of [[lem-author-4cb89398a4ab-complete-end-saturation]]. Thus $B=M\setminus I^-(M_{\mathrm{end}})$, $W=M\setminus I^+(M_{\mathrm{end}})$ and $N=\partial I^-(M_{\mathrm{end}})$ are stationary-invariant, and $W=\varnothing$ is exactly $M=I^+(M_{\mathrm{end}})$. Chronological sets here are defined by the same curve formulas for any subset $E$, without requiring $E$ open.

## Facts & Assumptions

[F1] Chronological futures and pasts are defined by existence of future timelike curves, and boundaries are closure minus interior. [[def-causal-exterior-and-boundary-data]]

[F2] Every $\phi_v$ is an isometry and the saturated end is invariant under it. [[lem-author-4cb89398a4ab-complete-end-saturation]]

## Proof

**Given:** The action, set and causal conventions in the Statement.

**Goal:** Prove the chronological and boundary invariance and the no-white-hole identity.

1.1 A time-orientation-preserving isometry maps future timelike curves to future timelike curves. Applying it to a curve from $E$ to $p$ gives $\psi(I^+(E))\subset I^+(E)$; applying its inverse gives the reverse inclusion. The identical argument with the curve direction reversed proves the past identity. As a diffeomorphism, $\psi$ maps open sets to open sets, and it and its inverse preserve limits, so it preserves interiors and closures and hence the displayed boundaries. [F1]

2.1 The connected one-parameter action preserves time orientation: along $v\mapsto(d\phi_v)_pV$, for a fixed future timelike $V$, timelikeness is preserved and the sign relative to a continuous future time-orientation field cannot change without becoming zero. At $v=0$ the vector is future. Apply step 1.1 and [F2]. Complements are preserved by a bijection, and $M\setminus I^+(M_{\mathrm{end}})=\varnothing$ is equivalent to $M=I^+(M_{\mathrm{end}})$ by elementary set complementation. This proves all assertions. [F1, F2, step 1.1] ∎

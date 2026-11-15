---
id: lem-author-58255dfd955f-exterior-exhaustion
title: Exterior exhaustion bounds for normalized Schrödinger solutions
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-exterior-weighted-elliptic-data
  - lem-author-58255dfd955f-compact-comparison
  - lem-author-58255dfd955f-strong-minimum
dependency_roles:
  def-exterior-weighted-elliptic-data: mathematical-premise
  lem-author-58255dfd955f-compact-comparison: mathematical-premise
  lem-author-58255dfd955f-strong-minimum: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 4
---

## Statement

On a connected exterior as in the exterior-data definition, let $V\ge0$ be smooth and let $u\in C^2(\Sigma^\circ)\cap C^1_{\mathrm{loc}}(\Sigma)$ solve $(\Delta_h-V)u=0$, vanish on $S$, and tend uniformly to $c>0$ as $r\to\infty$. Then $0<u\le c$ in the interior. If $S$ is nonempty, then $u<c$ there.

## Facts & Assumptions

**Given:** The end chart and compact core are those of [[def-exterior-weighted-elliptic-data]]. The limit means that for every $\epsilon>0$, $|u-c|<\epsilon$ beyond a sufficiently large end sphere. Use compact comparison [[lem-author-58255dfd955f-compact-comparison]] and the strong minimum alternative [[lem-author-58255dfd955f-strong-minimum]].

## Proof

**Given:** The hypotheses and data in the Statement and Facts & Assumptions.

**Goal:** Establish the conclusions of the Statement.

**Proof technique:** direct.

1.1 Truncate the exterior at $r=R$. For $R$ sufficiently large, $u\ge c/2>0$ on the outer sphere and $u=0$ on $S$. Comparison applied to $-u$ gives $u\ge0$ on the truncation. Applied to $u-(c+\epsilon)$, whose image under $\Delta_h-V$ is $V(c+\epsilon)\ge0$, it gives $u\le c+\epsilon$ when the outer sphere satisfies that bound. Every fixed point belongs to all sufficiently large truncations. Taking $R$ large and then $\epsilon\downarrow0$ proves $0\le u\le c$. Components of a truncation meet its boundary; otherwise such a component would be a compact component of the connected exterior separated from its end. [given]

2.1 The end limit excludes $u\equiv0$, so the strong minimum alternative makes $u>0$. The nonnegative function $c-u$ satisfies $(\Delta_h-V)(c-u)=-Vc\le0$. If it vanished inside, the same alternative would make $u\equiv c$. This contradicts $u|_S=0$ when $S\ne\varnothing$. Thus the stated strict upper bound also holds. [step 1.1, given, algebra] ∎

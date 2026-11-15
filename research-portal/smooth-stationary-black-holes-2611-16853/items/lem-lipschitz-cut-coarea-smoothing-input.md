---
id: lem-lipschitz-cut-coarea-smoothing-input
title: Coarea smoothing with fixed boundary values and area control
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-423fe0348a31-fixed-boundary-approximation
  - lem-author-423fe0348a31-riemannian-lipschitz-coarea
  - lem-author-423fe0348a31-band-energy-transfer
  - lem-author-423fe0348a31-regular-separating-level
  - def-lipschitz-cut-area-data
  - math:def-smooth-partition-of-unity-on-a-manifold-with-boundary
  - math:def-axiom-of-choice
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary
dependency_roles:
  lem-author-423fe0348a31-fixed-boundary-approximation: mathematical-premise
  lem-author-423fe0348a31-riemannian-lipschitz-coarea: mathematical-premise
  lem-author-423fe0348a31-band-energy-transfer: mathematical-premise
  lem-author-423fe0348a31-regular-separating-level: mathematical-premise
  def-lipschitz-cut-area-data: mathematical-premise
  math:def-smooth-partition-of-unity-on-a-manifold-with-boundary: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 8
---

## Statement

Let $(R,k)$ be a compact smooth Riemannian three-region with boundary $\partial R=B_-\sqcup B_+$ consisting of two smooth boundary components. Let $u$ be a real Lipschitz function, equal to constants $c_-$ and $c_+$ on neighborhoods of $B_-$ and $B_+$, where $c_-\le\inf I<\sup I\le c_+$ for a nonempty open interval $I$. Suppose $\mathcal H_k^2(\{u=t\})\le A<\infty$ for almost every $t\in I$, with $A\ge0$ and normalized metric Hausdorff measure. Then there is a sequence $u_j\in C^\infty(R)$ converging to $u$ in $C^0\cap W^{1,1}(R,k)$, with the exact same constants on fixed boundary neighborhoods. For every $\epsilon>0$, some $u_j$ has a regular value $t_j\in I$ with interior level $D_\epsilon=u_j^{-1}(t_j)$ separating the boundary components with $|D_\epsilon|_k\le A+\epsilon$. The set $\Omega_\epsilon=\{u_j\le t_j\}$ is a smooth compact region with $\partial\Omega_\epsilon=B_-\sqcup D_\epsilon$. The surface may be disconnected; if the boundary components can be joined by a path in $R$, it is nonempty. An endpoint-map area bound is a separate geometric input and is not asserted here.

## Facts & Assumptions

[F1] Relative mollification supplies a single uniform and metric first-Sobolev approximating sequence preserving the boundary constants. [[lem-author-423fe0348a31-fixed-boundary-approximation]]

[F2] Riemannian Lipschitz and smooth coarea hold on interior bands with normalized metric Hausdorff level areas. [[lem-author-423fe0348a31-riemannian-lipschitz-coarea]]

[F3] Interval enlargement transfers the almost-everywhere area bound to a limiting average bound for the smooth approximants. [[lem-author-423fe0348a31-band-energy-transfer]]

[F4] A strict average bound and Sard supply a regular smooth separating level and its smooth sublevel region. [[lem-author-423fe0348a31-regular-separating-level]]

[F5] Lipschitz weak gradients and cut areas have the fixed Riemannian conventions; endpoint multiplicity and endpoint-area formulas are separate inputs. [[def-lipschitz-cut-area-data]]

[F6] Smoothness and support at the boundary use the local-extension and subordinate-cutoff conventions. [[math:def-smooth-partition-of-unity-on-a-manifold-with-boundary]]

[F7] Work in ZFC, including the analytic and Sard suppliers' countable-choice assumptions. [[math:def-axiom-of-choice]]

[F8] A smooth Riemannian three-region is a three-dimensional smooth manifold with boundary equipped with a smooth positive-definite metric; boundary charts use compatible half-space charts and smooth local extensions. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary]]

## Proof

**Given:**The hypotheses in the Statement.

**Goal:** Establish the stated construction or identity.

1.1 Apply [F1] to obtain $u_j$ with the stated fixed boundary neighborhoods. Choose any interval $J=(a,b)$ with $[a,b]\subset I$ and $a<b$. The coarea identity [F2] applies to $u$ and all $u_j$ on these interior bands. By [F3], $\int_J\mathcal H_k^2(\{u_j=t\})dt\le A(|J|+2e_j)+d_j$, where $e_j,d_j\to0$. [given, F1, F2, F3, F5, F6, F7]

2.1 Choose $j$ large enough that $2Ae_j+d_j<\epsilon|J|$. Then the last integral is strictly less than $(A+\epsilon)|J|$. The exact boundary constants remain below $a$ and above $b$. Apply [F4] to $u_j$ and $J$ to obtain a regular value $t_j\in J\subset I$ and its level $D_\epsilon=u_j^{-1}(t_j)$ with the asserted area, separation, compactness and smooth sublevel boundary. This proves the full statement without identifying BV perimeter with level area or assuming convergence of individual level surfaces. [step 1.1, F4, given, algebra] ∎

## Remarks

The area hypothesis is an input on the original Lipschitz levels. It may be supplied by a correctly justified endpoint construction, but this result requires no endpoint map, multiplicity-one assertion or regularity of the original cut. The independent coarea theorem is recorded in its helper; relative C0 and W11 approximation is proved locally by finite chart mollification rather than imported from a theorem asserting only Lipschitz-controlled uniform approximation.

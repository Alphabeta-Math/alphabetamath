---
id: pthm-coarea-sard-smoothing
title: Coarea, smooth approximation and regular area-controlled levels
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - pthm-null-boundary-lipschitz-levels
  - pthm-raychaudhuri-endpoint-jacobians
  - lem-lipschitz-cut-coarea-smoothing-input
  - def-lipschitz-cut-area-data
  - def-truncated-null-boundary-height
  - def-stationary-section-time
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - post-stationary-vacuum-model
  - math:def-axiom-of-choice
  - def-near-horizon-past-boundary-sets
  - pthm-null-endpoint-map-properties
dependency_roles:
  pthm-null-boundary-lipschitz-levels: physical-result
  pthm-raychaudhuri-endpoint-jacobians: physical-result
  lem-lipschitz-cut-coarea-smoothing-input: mathematical-premise
  def-lipschitz-cut-area-data: mathematical-premise
  def-truncated-null-boundary-height: mathematical-premise
  def-stationary-section-time: mathematical-premise
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  post-stationary-vacuum-model: physical-assumption
  math:def-axiom-of-choice: mathematical-premise
  def-near-horizon-past-boundary-sets: mathematical-premise
  pthm-null-endpoint-map-properties: physical-result
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional area geometry in the smooth stationary vacuum
  Harrison construction; no observation is asserted.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 25–26, Lemma 4.4 and its proof
      attribution: The article constructs a smooth compact region bounded by the
        horizon section and a possibly disconnected smooth surface of area at
        most the comparison-sphere area plus an arbitrary positive error, using
        truncated height, coarea, smooth approximation and Sard's theorem.
      hypotheses: The Section 4 stationary vacuum Harrison construction and the
        comparison sphere and collar chosen in the proof of Lemma 4.4.
      reading_limits: Consulted the frozen extracted text of Lemma 4.4 and its proof
        on PDF pp. 25–26 for attribution only; no rendered-PDF verification or
        independent review of the original argument is claimed. This reference
        supplies no prerequisite or proof premise.
dependency_level: 30
---

## Statement

Work in ZFC under the regular mass-one stationary vacuum Harrison construction, with original maximal exterior section, $T|_S\not\equiv0$, fixed sufficiently small positive $q$, supplied smooth maximal section $\Sigma=\Sigma_{q,0}$, and sufficiently late comparison sphere $C=C_t$, as in the localized construction. Let $\mathcal R=\{0\le\rho\le\eta\}$ be its supplied compact smooth collar, with boundary components $S$ and $S_\eta$. Use the induced Riemannian metric $h_0$ on $\Sigma$, the truncated height $u$, and the zero-time endpoint data $A\subset C$, $F:A\to D$ of the near-horizon construction, with the maximal generator family supplied by the endpoint-map result.

For every $\epsilon>0$, one can choose a sufficiently small height parameter $\delta>0$ and a smooth function $u_i$ on $\mathcal R$, from a sequence converging to $u$ in $C^0\cap W^{1,1}$ and preserving its constants $-2\delta$ and $2\delta$ on fixed neighborhoods of $S$ and $S_\eta$, respectively, and a regular value $b\in(-\delta,-\delta/2)$ such that $D_\epsilon=u_i^{-1}(b)$ is smooth, closed, possibly disconnected, separates the two boundary components, and satisfies

$$|D_\epsilon|_{h_0}\le\int_A J_2F\,d\mu_C+\epsilon\le|A|+\epsilon\le|C|+\epsilon.$$

The compact smooth sublevel region $\Omega_\epsilon=\{u_i\le b\}\subset\mathcal R$ has boundary $S\sqcup D_\epsilon$. Here $|A|$ is its induced surface measure in $C$, and $J_2F$ is the nonnegative Gram two-Jacobian in the fixed metrics; neither injectivity of $F$ nor multiplicity one is assumed.

## Statement references

[[pthm-null-boundary-lipschitz-levels]]

[[pthm-raychaudhuri-endpoint-jacobians]]

[[lem-lipschitz-cut-coarea-smoothing-input]]

[[def-lipschitz-cut-area-data]]

[[def-truncated-null-boundary-height]]

[[def-stationary-section-time]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-harrison-normalization]]

[[post-stationary-vacuum-model]]

[[math:def-axiom-of-choice]]

[[def-near-horizon-past-boundary-sets]]

[[pthm-null-endpoint-map-properties]]

## Facts & Assumptions

[F1] The model, regularity and mass-one normalization are those of [[post-stationary-vacuum-model]], [[def-regular-stationary-vacuum-spacetime]] and [[def-harrison-normalization]]. Work in ZFC, including the Axiom of Choice. [[math:def-axiom-of-choice]]

[F2] The section time and induced metric use [[def-stationary-section-time]]. The collar distance, zero-time cut $D$, initial domain $A$ and endpoint map $F$ use [[def-near-horizon-past-boundary-sets]], with the maximal generator family of [[pthm-null-endpoint-map-properties]]. The truncated height and translated cuts use [[def-truncated-null-boundary-height]]. The endpoint theorem supplies closed, hence compact and Borel, $A\subset C$ and local smooth extensions of $F$ into the spacelike section, so its Gram Jacobian is measurable in the conventions of [[def-lipschitz-cut-area-data]].

[F3] For the fixed target and collar, [[pthm-null-boundary-lipschitz-levels]] supplies the boundary constants, Lipschitz height and, for every $z\in(-\delta,-\delta/2)$, the bound $\mathcal H^2_{h_0}(\{u=z\})\le(1+o_\delta(1))\int_A J_2F\,d\mu_C$, with $o_\delta(1)\to0$ as $\delta\downarrow0$.

[F4] The sufficiently late target fixed in [F3] satisfies $\min_C v>0$, as ensured in Proof 2.1 of [[pthm-null-boundary-lipschitz-levels]]. Thus the zero-time conclusion of [[pthm-raychaudhuri-endpoint-jacobians]] applies on the entire domain $A$: $0\le J_2F(c)\le1$ for every $c\in A$, without requiring an exhaustion by the negative-cut domains. Measurability is supplied by [F2], not by the Jacobian definition.

[F5] Relative smooth approximation, coarea, interval enlargement and regular-level selection apply to a compact smooth Riemannian three-region with two smooth boundary components, boundary-constant Lipschitz height and an almost-everywhere finite level-area bound. They give a regular value in the prescribed open interval, an interior level with area within any positive error of that bound, and the stated sublevel boundary. [[lem-lipschitz-cut-coarea-smoothing-input]]

## Proof

**Given:** The construction and $\epsilon>0$ in the Statement.

**Goal:** Construct $u_i$, $b$, $D_\epsilon$ and $\Omega_\epsilon$ with the stated properties.

1.1 Put $K=\int_A J_2F\,d\mu_C$. By [F2] and [F4], this integral is defined and $0\le K\le|A|\le|C|<\infty$. With the target and collar fixed, choose $\delta$ sufficiently small that the bound in [F3] holds and its nonnegative distortion allowance $r_\delta=\max\{o_\delta(1),0\}$ satisfies $r_\delta K<\epsilon/2$. The resulting height is Lipschitz and has the two stated boundary constants. Thus every level in $I=(-\delta,-\delta/2)$ has area at most $(1+r_\delta)K$. [given, F2, F3, F4, algebra]

2.1 Apply [F5] to $\mathcal R$, $u$, $I$ and the bound $(1+r_\delta)K$, with smoothing error $\epsilon/2$. The endpoint constants lie on opposite sides of $I$. The supplier gives a single smooth approximating sequence preserving the constants on fixed boundary neighborhoods and, for some index $i$, a regular value $b\in I$ whose level separates the boundary components and has area at most $(1+r_\delta)K+\epsilon/2<K+\epsilon$. It also gives the compact smooth sublevel region with boundary $S\sqcup D_\epsilon$. [step 1.1, F2, F5]

3.1 Substitute the definition of $K$ and use $K\le|A|\le|C|$ from step 1.1. This proves the displayed chain and the remaining conclusions. The coarea and Sard selection in [F5] does not require the original Lipschitz levels to be smooth or the endpoint map to be injective. [step 1.1, step 2.1, F5] ∎

## Source notes

The article citation supplies attribution only. The geometric level estimate retains the small flow-distortion factor; the proof absorbs it before applying the independent smoothing supplier. The parameter $\delta$ used here is the height parameter, not a lower bound on $q$.

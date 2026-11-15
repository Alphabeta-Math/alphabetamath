---
id: pthm-inverse-harrison-contraction
title: Inverse Harrison relation and Killing-scalar identity
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - def-killing-ernst-notation
  - def-complex-self-dual-two-form-data
  - def-harrison-one-form
  - def-harrison-electromagnetic-form
  - pthm-horizon-invariant-one-form
  - pthm-harrison-denominator-positive
  - pthm-harrison-lorentzian-algebra
  - lem-rank-one-lorentzian-hodge-transfer
  - pthm-limiting-maxwell-normal-form
formulation_deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - def-killing-ernst-notation
  - def-complex-self-dual-two-form-data
  - def-harrison-one-form
  - def-harrison-electromagnetic-form
  - pthm-horizon-invariant-one-form
argument_deps:
  - pthm-harrison-denominator-positive
  - pthm-harrison-lorentzian-algebra
  - lem-rank-one-lorentzian-hodge-transfer
  - pthm-limiting-maxwell-normal-form
  - def-harrison-electromagnetic-form
  - def-complex-self-dual-two-form-data
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  def-harrison-one-form: mathematical-premise
  def-harrison-electromagnetic-form: mathematical-premise
  pthm-horizon-invariant-one-form: physical-result
  pthm-harrison-denominator-positive: physical-result
  pthm-harrison-lorentzian-algebra: physical-result
  lem-rank-one-lorentzian-hodge-transfer: mathematical-premise
  pthm-limiting-maxwell-normal-form: physical-result
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
physical_scope: Conditional geometric deduction in the smooth stationary vacuum
  model and its limiting Harrison geometry; no measurement is asserted.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 28, equation (5.2) and the following contraction display
      hypotheses: The article's regular stationary vacuum construction, maximal
        original exterior section, mass one, and the specified limiting Harrison
        family.
      reading_limits: Read the frozen article text at the cited passage. This
        reference attributes the claim; it is not used as a proof premise.
dependency_level: 36
---

## Statement

Adopt the stationary vacuum model and regular non-degenerate stationary construction, with original exterior section spacelike and maximal, ADM mass one, and stationary Killing field $T$ not identically zero on the bifurcation sphere $S$. Use the supplied normalized Ernst potential $\sigma=f+i\psi$, where $f=-g(T,T)$ and $\psi$ is real, and the single regular Harrison family with its invariant one-form $W_0$ and pole $p\in S$ satisfying $T_p=0$. Let $F_{ab}=\nabla_aT_b$, $\mathcal F=F+i\star_gF$, $D_0=|1-\sigma|^2$, $d_0=D_0(p)$, and $A_0v=v+D_0^{-1}W_0(v)T$. The pullback $A_0^*$ acts on each covariant slot. Let $g_0$ and $F_0$ be the limiting Harrison metric and real electromagnetic two-form, and set $H_0=F_0+i\star_{g_0}F_0$.

On $S$ the inverse Harrison relation and metric relation are

$$\mathcal F=-\frac{1-\sigma}{1-\overline\sigma}(A_0^{-1})^*H_0,\qquad g_0=\frac{|1-\sigma|^2}{4}A_0^*g.$$

With both indices on each form raised by its own metric, and with complex bilinear contraction without conjugation or a factor of one half,

$$\mathcal F_{ab}\mathcal F^{ab}_g=\left(\frac{1-\sigma}{1-\overline\sigma}\right)^2\frac{|1-\sigma|^4}{16}(H_0)_{ab}(H_0)^{ab}_{g_0}=-\frac14(1-\sigma)^4.$$

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-harrison-normalization]]

[[def-killing-ernst-notation]]

[[def-complex-self-dual-two-form-data]]

[[def-harrison-one-form]]

[[def-harrison-electromagnetic-form]]

[[pthm-horizon-invariant-one-form]]

## Facts & Assumptions

[A1] The model, regular construction, maximal section and mass-one convention are as specified in the statement. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]] [[def-harrison-normalization]]

[F1] The normalized Ernst and complex-form conventions define $F$, $\mathcal F$, the metric Hodge stars, fiberwise pullback and the full complex bilinear contraction used above. [[def-killing-ernst-notation]] [[def-complex-self-dual-two-form-data]]

[F2] The invariant construction supplies the indicated smooth potential, pole and one-form with $W_0(T)=d_0-D_0$. The denominator result gives $D_0>0$ on a neighborhood of $S$. [[pthm-horizon-invariant-one-form]] [[pthm-harrison-denominator-positive]]

[F3] The Harrison definitions give $g_0=(D_0/4)A_0^*g$ and, at $q=0$, $H_0=-((1-\overline\sigma)/(1-\sigma))A_0^*\mathcal F$. The latter uses $H_0=F_0+i\star_{g_0}F_0$. [[def-harrison-one-form]] [[def-harrison-electromagnetic-form]]

[F4] For the supplied pole and positive denominator, $d_0>0$ and $A_0$ is orientation preserving and invertible. Its metric transfer gives $(A_0^*U)_{ab}(A_0^*U)^{ab}_{g_0}=(4/D_0)^2U_{ab}U^{ab}_g$ for any complex two-form $U$. [[pthm-harrison-lorentzian-algebra]] [[lem-rank-one-lorentzian-hodge-transfer]]

[F5] At each point of $S$, in the oriented $g_0$-orthonormal frame of the limiting normal-form result, $(F_0)_{01}=-1$, $(F_0)_{23}=0$, $(\star_{g_0}F_0)_{01}=0$, $(\star_{g_0}F_0)_{23}=1$, and the mixed normal–tangential components of $F_0$ vanish. [[pthm-limiting-maxwell-normal-form]]

## Proof

**Given:** The model, construction and conventions in the Statement.

**Goal:** Prove the inverse relation and the displayed contraction identity on $S$.

1.1 By positivity of $D_0$, both $1-\sigma$ and $1-\overline\sigma$ are nonzero. The map $A_0$ is invertible, so applying $(A_0^{-1})^*$ to the electromagnetic formula in [F3] and multiplying by the reciprocal scalar gives the inverse relation. The metric relation is the first formula in [F3]. [given, F2, F3, F4, algebra]

1.2 In the frame of [F5], $H_{0,01}=-1$ and $H_{0,23}=i$, while all mixed components vanish: the Hodge star maps the normal and tangent area forms to each other in this oriented orthonormal frame. Raising with $g_0=\operatorname{diag}(-1,1,1,1)$ in that frame and summing both orders of each antisymmetric index pair gives $(H_0)_{ab}(H_0)^{ab}_{g_0}=2((-1)(1)+i^2)=-4$. [F1, F5, algebra]

2.1 The transfer formula in [F4] with $U=\mathcal F$ gives $(A_0^*\mathcal F)^2_{g_0}=(4/D_0)^2\mathcal F^2_g$. Substitution of the $q=0$ electromagnetic formula yields the first displayed contraction equality. Finally $D_0=(1-\sigma)(1-\overline\sigma)$ and step 1.2 give $\mathcal F^2_g=-\tfrac14(1-\sigma)^4$. This proves the identity at every point of $S$. [F3, F4, step 1.1, step 1.2, algebra] ∎

## Source notes

The article passage attributes the original relations. The argument above uses the stated construction and normal-form suppliers, rather than the article's assertion as a premise.

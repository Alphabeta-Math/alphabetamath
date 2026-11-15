---
id: pthm-recovery-ik-identities
title: "Proposition 5.1: recovery of Ionescu–Klainerman conditions"
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
  - pthm-inverse-harrison-contraction
  - pthm-axial-averaging-positive-boost
  - pthm-local-hawking-circle-fields
formulation_deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - def-killing-ernst-notation
  - def-complex-self-dual-two-form-data
  - pthm-local-hawking-circle-fields
  - pthm-inverse-harrison-contraction
  - pthm-axial-averaging-positive-boost
argument_deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - def-killing-ernst-notation
  - def-complex-self-dual-two-form-data
  - pthm-inverse-harrison-contraction
  - pthm-axial-averaging-positive-boost
  - pthm-local-hawking-circle-fields
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  pthm-inverse-harrison-contraction: physical-result
  pthm-axial-averaging-positive-boost: physical-result
  pthm-local-hawking-circle-fields: physical-result
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional geometric deduction in the smooth stationary vacuum
  black-hole model and its limiting Harrison construction; no observation is
  asserted.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pages 28–29, Proposition 5.1 and its proof
      statement: The original vacuum metric satisfies the displayed Killing-form
        identity on the bifurcation sphere and the strict Ernst-potential
        inequality at the chosen pole.
      hypotheses: The article's regular stationary vacuum construction, maximal
        original exterior section, nontrivial stationary field on the
        bifurcation sphere, mass-one normalization and chosen pole.
      reading_limits: Read the frozen article text at the cited passage. This
        reference attributes the claim and is not used as a proof premise.
dependency_level: 39
---

## Statement

Adopt the stationary vacuum model and regular non-degenerate stationary construction, with original exterior section spacelike and maximal, ADM mass one, and stationary Killing field $T$ not identically zero on the bifurcation sphere $S$. Use the supplied normalized Ernst potential $\sigma=f+i\psi$, the single regular Harrison family, and its chosen pole $p\in S$, as in the two recovery suppliers. Here $p$ is the common pole of the local Hawking and axial fields $K,Z$ supplied under these hypotheses: $K=T+\Omega_H Z$, $K|_S=0$, $T(p)=Z(p)=0$, $Z$ has least positive common period $2\pi$, and $K$ has positive normal boost rate $\kappa$ in the future/outward normal basis. The Harrison family uses this same pole. Here $f=-g(T,T)$ and $\psi$ is real. Define $F_{ab}=\nabla_aT_b$ and $\mathcal F=F+i\star_gF$, where $\nabla$ and $\star_g$ are the original metric's Levi–Civita connection and oriented Hodge star. Contract complex bilinearly, without conjugation or a factor of one half, and raise both indices using the original metric $g$.

Then $-4\mathcal F_{ab}\mathcal F^{ab}=(1-\sigma)^4$ everywhere on $S$, and $\operatorname{Re}(1/(1-\sigma(p)))>1/2$.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-harrison-normalization]]

[[def-killing-ernst-notation]]

[[def-complex-self-dual-two-form-data]]

[[pthm-local-hawking-circle-fields]]

[[pthm-inverse-harrison-contraction]]

[[pthm-axial-averaging-positive-boost]]

## Facts & Assumptions

[A1] The stationary vacuum model, regular construction, maximal original exterior section, mass-one normalization, nontriviality of $T$ on $S$, supplied potential, Harrison family and pole are those in the Statement. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]] [[def-harrison-normalization]]

[F1] The normalized Ernst and complex-form conventions give the displayed definitions of $\sigma$, $F$ and $\mathcal F$, with the original metric used to raise indices and a complex bilinear contraction. [[def-killing-ernst-notation]] [[def-complex-self-dual-two-form-data]]

[F2] Under the stated construction hypotheses, the inverse Harrison contraction gives $\mathcal F_{ab}\mathcal F^{ab}_g=-\frac14(1-\sigma)^4$ on $S$. [[pthm-inverse-harrison-contraction]]

[F3] With the local fields and common pole in [F4], the same normalized potential and regular Harrison family, and $d_0=|1-\sigma(p)|^2>0$, axial averaging gives $2\operatorname{Re}(1/(1-\sigma(p)))-1>0$; in particular the displayed reciprocal is defined. [[pthm-axial-averaging-positive-boost]]

[F4] The regular stationary vacuum data, maximal original exterior section and $T|_S\not\equiv0$ supply local commuting Killing fields $K,Z$ with $K=T+\Omega_H Z$, $K|_S=0$, a circle action of least positive common period $2\pi$, a common pole $p\in S$ with $T(p)=Z(p)=0$, and a constant positive normal boost rate $\kappa$ for $K$ in the future/outward normal basis. These are the fields and pole used for the stated single Harrison family. [[pthm-local-hawking-circle-fields]]

## Proof

**Given:** The model, construction and conventions in the Statement.

**Goal:** Establish the two displayed conditions on $S$ and at $p$.

1.1 The regular stationary vacuum data, maximal original exterior section and nontriviality of $T$ in [A1] match [F4]. Use its local fields $K,Z$ and common pole $p$, with the normalized circle action and positive future/outward boost. By the stated family choice this is the same pole used throughout the two recovery suppliers, rather than a separately chosen zero of $T$. [A1, F4]

2.1 The construction hypotheses and original-metric contraction convention match [F2] for this family. Multiplying its equality by $-4$ gives $-4\mathcal F_{ab}\mathcal F^{ab}=(1-\sigma)^4$ at every point of $S$. [A1, F1, F2, step 1.1, algebra]

3.1 At the common pole, $T(p)=0$ gives $f(p)=-g(T,T)(p)=0$, so $\sigma(p)=i\psi(p)$ and $d_0=|1-\sigma(p)|^2=1+\psi(p)^2>0$. Together with the local fields, circle normalization and positive boost from step 1.1 and the same potential and family, this verifies the premises of [F3]. Adding one to its strict inequality and dividing by the positive number two gives $\operatorname{Re}(1/(1-\sigma(p)))>1/2$. Together with step 2.1 this proves both conditions. [A1, F1, F3, F4, step 1.1, step 2.1, algebra] ∎

## Source notes

The article is cited for attribution of Proposition 5.1. The deduction above uses the declared local-field and recovery suppliers. The article's assertion is not a proof premise.

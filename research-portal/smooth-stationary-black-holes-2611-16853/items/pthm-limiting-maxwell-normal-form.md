---
id: pthm-limiting-maxwell-normal-form
title: Boost invariance and limiting Maxwell normal form
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - pthm-local-hawking-circle-fields
  - pthm-horizon-invariant-one-form
  - pthm-ernst-potential-existence
  - pthm-harrison-electrovacuum
  - pthm-limiting-flux-rigidity
  - def-harrison-one-form
  - def-harrison-electromagnetic-form
  - def-surface-area-flux-and-null-variation-data
  - def-complex-self-dual-two-form-data
  - lem-killing-normal-boost-and-invariant-tensors
  - physics:lem-emg-lorentz-hodge-calculus
  - lem-author-c92bdd91a36e-common-positive-neighborhood
formulation_deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - pthm-local-hawking-circle-fields
  - pthm-horizon-invariant-one-form
  - pthm-harrison-electrovacuum
  - pthm-limiting-flux-rigidity
  - def-surface-area-flux-and-null-variation-data
  - physics:lem-emg-lorentz-hodge-calculus
argument_deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - pthm-local-hawking-circle-fields
  - pthm-horizon-invariant-one-form
  - pthm-ernst-potential-existence
  - pthm-harrison-electrovacuum
  - pthm-limiting-flux-rigidity
  - def-harrison-one-form
  - def-harrison-electromagnetic-form
  - def-surface-area-flux-and-null-variation-data
  - def-complex-self-dual-two-form-data
  - lem-killing-normal-boost-and-invariant-tensors
  - physics:lem-emg-lorentz-hodge-calculus
  - lem-author-c92bdd91a36e-common-positive-neighborhood
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  pthm-local-hawking-circle-fields: physical-result
  pthm-horizon-invariant-one-form: physical-result
  pthm-ernst-potential-existence: physical-result
  pthm-harrison-electrovacuum: physical-result
  pthm-limiting-flux-rigidity: physical-result
  def-harrison-one-form: mathematical-premise
  def-harrison-electromagnetic-form: mathematical-premise
  def-surface-area-flux-and-null-variation-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  lem-killing-normal-boost-and-invariant-tensors: mathematical-premise
  physics:lem-emg-lorentz-hodge-calculus: mathematical-premise
  lem-author-c92bdd91a36e-common-positive-neighborhood: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional deduction in the smooth four-dimensional stationary
  vacuum model and its limiting Harrison electromagnetic geometry; no
  observation is asserted.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 28, proof of Proposition 5.1, first paragraph
      attribution: The limiting flux densities and boost invariance give vanishing
        mixed components and the displayed limiting electromagnetic normal form.
      hypotheses: The regular stationary vacuum construction, maximal original
        exterior section, mass-one normalization, nontrivial stationary field on
        the bifurcation sphere, and the chosen orientations.
      reading_limits: Historical reading note retained from the current source; this
        maintenance revision claims no fresh article or external full-text
        reading. Read the frozen article text at the cited passage for
        attribution. The article's claim is not used as a proof premise.
dependency_level: 35
---

## Statement

Adopt the stationary vacuum model and regular non-degenerate stationary construction, with original exterior section spacelike and maximal, ADM mass one, and stationary field $T$ not identically zero on the bifurcation sphere $S$. Use the single regular Harrison family and invariant primitive supplied in this construction. Let $g_0$ and $F_0$ be its limiting metric and real electromagnetic two-form, and let $K$ be the local Hawking field.

The local flow of $K$ fixes $S$, acts by a nontrivial boost on the $g_0$-normal plane to $S$, and preserves $F_0$. Consequently the mixed normal–tangential components of $F_0$ vanish. At each point choose a $g_0$-orthonormal frame $(n=e_0,\nu=e_1,e_2,e_3)$ in the spacetime orientation, where $n$ is future timelike, $\nu$ is the outward spacelike normal, and $(e_2,e_3)$ is positively oriented for the outward end-sphere orientation of $S$. Then $(F_0)_{23}=(\star_{g_0}F_0)_{01}=0$ and $(\star_{g_0}F_0)_{23}=-(F_0)_{01}=1$; all other independent components of $F_0$ vanish. The frame label $e_0$ is distinct from the electric flux density $e_0=1$.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-harrison-normalization]]

[[pthm-local-hawking-circle-fields]]

[[pthm-horizon-invariant-one-form]]

[[pthm-harrison-electrovacuum]]

[[pthm-limiting-flux-rigidity]]

[[def-surface-area-flux-and-null-variation-data]]

[[physics:lem-emg-lorentz-hodge-calculus]]

## Facts & Assumptions

[A1] The stated model and regularity hypotheses include the oriented stationary geometry, the bifurcation sphere, the maximal original exterior section, and the mass-one normalization. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]] [[def-harrison-normalization]]

[F1] The local Hawking field $K$ is Killing for the original metric, commutes with $T$, vanishes on $S$, and has a positive-rate normal boost there. Its flow fixes $S$ pointwise and its differential is the identity on $TS$ and a nontrivial boost on the original normal plane. The local-field result also supplies a pole $p\in S$ with $T(p)=0$. [[pthm-local-hawking-circle-fields]] [[lem-killing-normal-boost-and-invariant-tensors]]

[F2] The invariant-gauge result supplies a smooth normalized Ernst potential $\sigma$ and a single smooth primitive $W_0$ near $S$, both invariant under $K$. The regular Harrison result supplies the limiting Lorentzian metric and real two-form on a neighborhood of $S$. Here $\sigma=f+i\psi$, $f=-g(T,T)$ and $\psi$ is real; $W_0$ is stationary, $dW_0=4((f-1)F+\psi\star_gF)$ and $W_0(T)=D_0(p)-D_0$ for the pole in [F1], with $D_0=|1-\sigma|^2$ and $F=\tfrac12dT^\flat$. For this same normalized potential, $d\sigma=2\iota_T(F+i\star_gF)$ with $F=\tfrac12dT^\flat$. [[pthm-ernst-potential-existence]] [[pthm-horizon-invariant-one-form]] [[pthm-harrison-electrovacuum]]

[F3] Put $D_0=|1-\sigma|^2$ and $A_0v=v+D_0^{-1}W_0(v)T$. The Harrison definitions give $g_0=(D_0/4)A_0^*g$ and express the complex electromagnetic form as a scalar depending on $\sigma$ times $A_0^*(F+i\star_gF)$, where $F=\tfrac12dT^\flat$; $F_0$ is its real part. These formulas apply where $D_0>0$. [[def-harrison-one-form]] [[def-harrison-electromagnetic-form]] [[def-complex-self-dual-two-form-data]]

[F4] The limiting flux result gives $b_0=0$ and $e_0=1$ pointwise. The limiting-flux interface uses the Riemannian induced metric $\gamma_0=g_0|_{TS}$ on $S$. By definition, $F_0|_{TS}=b_0\,d\mu_0$ and $(\star_{g_0}F_0)|_{TS}=e_0\,d\mu_0$, where $d\mu_0$ is the area form for the stated orientation. [[pthm-limiting-flux-rigidity]] [[def-surface-area-flux-and-null-variation-data]]

[F5] For either oriented Lorentzian metric of signature $(-,+,+,+)$, the Hodge star is uniquely characterized by $\alpha\wedge\star\beta=\langle\alpha,\beta\rangle\,\mathrm{vol}$. In a positively oriented orthonormal coframe, $\star(e^0\wedge e^1)=-e^2\wedge e^3$ and $\star(e^2\wedge e^3)=e^0\wedge e^1$. [[physics:lem-emg-lorentz-hodge-calculus]]

[F6] For a compact embedded spacelike surface with tangent stationary field $T$ and a zero $p$, the potential and stationary primitive identities in [F2] imply a common open neighborhood of that surface on which $D_q=|1+q-(1-q)\sigma|^2>0$ for all $q\in[0,1]$; in particular $D_0>0$ there. [[lem-author-c92bdd91a36e-common-positive-neighborhood]]

## Proof

**Given:** The model, construction, orientations and frame in the Statement.

**Goal:** Establish the limiting boost invariance and the displayed components.

1.1 By [A1], $S$ is an embedded compact sphere inside the original spacelike section, so its induced $g$-metric is positive definite. At $s\in S$, $T_sS$ lies in both horizon tangent spaces; transversality makes their intersection two-dimensional, hence equal to $T_sS$. Since $T$ is tangent to both branches, it is tangent to $S$. The pole in [F1], smooth potential and stationary primitive identities in [F2] therefore meet every hypothesis of [F6]. Applied on their common neighborhood, [F6] gives an open $O$ containing $S$ with $D_0>0$. Restrict to $O$ when using [F3]. [A1, F1, F2, F3, F6, algebra]

2.1 The local flow of $K$ preserves $g$ and $T$ by [F1]. It therefore preserves $T^\flat$ and $F=\tfrac12dT^\flat$. Being an isometry connected to the identity, it preserves the original metric, orientation, exterior pairing and metric volume form. Pulling back the characterizing identity in [F5] and using uniqueness gives $\Phi_t^*(\star_gF)=\star_g(\Phi_t^*F)$, so it also preserves $\star_gF$. By [F2] it also preserves $\sigma$ and $W_0$. Hence it preserves $D_0$, $A_0$, $g_0$, and the complex Harrison electromagnetic form in [F3], and thus preserves its real part $F_0$. These are local assertions on $O$ wherever the local flow is defined. [F1, F2, F3, F5, step 1.1]

3.1 Fix $p\in S$. The flow fixes $p$ and acts identically on $T_pS$. Its differential preserves $g_0$ by step 2.1, so it preserves the $g_0$-orthogonal normal plane $N_p$. Since $T_pS$ is spacelike for $g_0$ by [F4], the quotient $T_pM/T_pS$ is naturally isomorphic to $N_p$ through orthogonal projection. On that quotient the differential has eigenvalues $e^{\kappa t}$ and $e^{-\kappa t}$ with $\kappa>0$: this follows from the original normal boost in [F1]. Consequently its action on $N_p$ is a nontrivial Lorentz boost with those eigenvalues. If $v_\pm$ are corresponding null eigenvectors and $X\in T_pS$, invariance gives $F_0(v_\pm,X)=e^{\pm\kappa t}F_0(v_\pm,X)$. A sufficiently small nonzero $t$ forces both values to vanish. The eigenvectors span $N_p$, proving all mixed normal–tangential components vanish. [F1, F4, step 2.1, algebra]

4.1 In the positive tangent frame, $d\mu_0(e_2,e_3)=1$. Thus [F4] gives $(F_0)_{23}=0$ and $(\star_{g_0}F_0)_{23}=1$. In the stated oriented orthonormal Lorentz frame, the two basis identities in [F5] give $(\star_{g_0}F_0)_{23}=-(F_0)_{01}$ and $(\star_{g_0}F_0)_{01}=(F_0)_{23}$. Hence $(F_0)_{01}=-1$ and $(\star_{g_0}F_0)_{01}=0$. Antisymmetry and step 3.1 account for every remaining independent component of $F_0$. [F4, F5, step 3.1, algebra] ∎

## Source notes

The article reference attributes the original normal-form claim. Its printed display uses $\star_{g_q}$ while describing a $g_0$-orthonormal frame; the limiting calculation above uses $\star_{g_0}$ throughout. The proof uses the declared suppliers and does not use the article's assertion as a premise.

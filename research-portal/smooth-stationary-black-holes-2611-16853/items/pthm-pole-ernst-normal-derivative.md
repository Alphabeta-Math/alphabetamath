---
id: pthm-pole-ernst-normal-derivative
title: Pole identities and the Ernst scalar inequality reduction
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
  - pthm-local-hawking-circle-fields
  - pthm-horizon-invariant-one-form
  - pthm-harrison-denominator-positive
  - pthm-inverse-harrison-contraction
  - pthm-limiting-maxwell-normal-form
formulation_deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - def-killing-ernst-notation
  - def-complex-self-dual-two-form-data
  - def-harrison-one-form
  - pthm-local-hawking-circle-fields
  - pthm-horizon-invariant-one-form
  - pthm-inverse-harrison-contraction
  - pthm-limiting-maxwell-normal-form
argument_deps:
  - pthm-local-hawking-circle-fields
  - pthm-horizon-invariant-one-form
  - pthm-harrison-denominator-positive
  - pthm-inverse-harrison-contraction
  - pthm-limiting-maxwell-normal-form
  - def-killing-ernst-notation
  - def-harrison-one-form
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  def-harrison-one-form: mathematical-premise
  pthm-local-hawking-circle-fields: physical-result
  pthm-horizon-invariant-one-form: physical-result
  pthm-harrison-denominator-positive: physical-result
  pthm-inverse-harrison-contraction: physical-result
  pthm-limiting-maxwell-normal-form: physical-result
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional geometric deduction in the smooth stationary vacuum
  model and its limiting Harrison geometry; no observation is asserted.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 28–29, proof of Proposition 5.1, second condition
      hypotheses: The article's regular stationary vacuum construction, maximal
        original exterior section, mass-one normalization, and nontrivial
        stationary field on the bifurcation sphere.
      reading_limits: Attribution only. At the common pole the article states the
        inverse-field and normal-derivative identities and proves positivity
        using the local axial and Hawking fields. Read the frozen article text
        at the cited passage for attribution; the article's assertion is not
        used as a proof premise.
dependency_level: 37
---

## Statement

Adopt the stationary vacuum model and regular non-degenerate stationary construction, with original exterior section spacelike and maximal, ADM mass one, and stationary Killing field $T$ not identically zero on the bifurcation sphere $S$. Use the supplied normalized Ernst potential $\sigma=f+i\psi$, where $f=-g(T,T)$ and $\psi$ is real, the single regular Harrison family, and its limiting metric $g_0$ and real electromagnetic two-form $F_0$. Let $p\in S$ be the supplied common zero of $T$ and the local axial field $Z$. Put $D_0=|1-\sigma|^2$, $d_0=D_0(p)$, and $A_0v=v+D_0^{-1}W_0(v)T$, where $W_0$ is the supplied invariant Harrison one-form. Let $\nabla$ and $\nabla^{(0)}$ be the Levi–Civita connections of $g$ and $g_0$, respectively; let $\mathcal F=\nabla T^\flat+i\star_g\nabla T^\flat$, with $(\nabla T^\flat)_{ab}=\nabla_aT_b$.

At $p$, $d_0>0$, $A_0=\operatorname{id}$, $f=0$, $g_0=(d_0/4)g$, and $\overline\sigma=-\sigma$. Thus, at $p$,

$$\mathcal F=-\frac{1-\sigma}{1+\sigma}(F_0+i\star_{g_0}F_0).$$

For any future unit timelike normal $n$ and outward unit spacelike normal $\nu$ to $S$ at $p$, orthogonal to one another and normalized using $g_0$, one has

$$g(\nabla_nT,\nu)=\operatorname{Re}\frac{1-\sigma(p)}{1+\sigma(p)}=2\operatorname{Re}\frac{1}{1-\sigma(p)}-1.$$

Also $\nabla^{(0)}_nT=\nabla_nT$ and $g(\nabla_nT,\nu)=(4/d_0)g_0(\nabla^{(0)}_nT,\nu)$ at $p$. The common quantity is strictly positive; equivalently $\operatorname{Re}(1/(1-\sigma(p)))>1/2$.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-harrison-normalization]]

[[def-killing-ernst-notation]]

[[def-complex-self-dual-two-form-data]]

[[def-harrison-one-form]]

[[pthm-local-hawking-circle-fields]]

[[pthm-horizon-invariant-one-form]]

[[pthm-inverse-harrison-contraction]]

[[pthm-limiting-maxwell-normal-form]]

## Facts & Assumptions

[A1] The model, regular construction, maximal section, mass normalization, and nontriviality of $T|_S$ are those in the Statement. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]] [[def-harrison-normalization]]

[F1] The Ernst and complex-form conventions define $f$, $\sigma$, the Killing two-form, and the metric-dependent Hodge stars. The Harrison definition supplies $A_0$ and $g_0=(D_0/4)A_0^*g$. [[def-killing-ernst-notation]] [[def-complex-self-dual-two-form-data]] [[def-harrison-one-form]]

[F2] The denominator is positive near $S$. On $S$ the inverse Harrison relation is $\mathcal F=-((1-\sigma)/(1-\overline\sigma))(A_0^{-1})^*(F_0+i\star_{g_0}F_0)$. [[pthm-harrison-denominator-positive]] [[pthm-inverse-harrison-contraction]]

[F3] In every oriented $g_0$-orthonormal frame with future and outward normal vectors $n,\nu$, the limiting normal form has $F_0(n,\nu)=-1$ and $(\star_{g_0}F_0)(n,\nu)=0$. [[pthm-limiting-maxwell-normal-form]]

[F4] Locally $K=T+\Omega_HZ$ is a Killing field vanishing on $S$; $Z$ has a $2\pi$-periodic isometric flow and vanishes at $p$. At $S$, the normal action of $v\mapsto\nabla_vK$ is a boost of rate $\kappa>0$, taking the future unit normal to $\kappa$ times the outward unit normal. [[pthm-local-hawking-circle-fields]]

[F5] The local flows of $K$ and $Z$ preserve $T$, $\sigma$ and the supplied one-form $W_0$; they also preserve $g$. [[pthm-local-hawking-circle-fields]] [[pthm-horizon-invariant-one-form]]

## Proof

**Given:** The model, construction, pole and normal frame in the Statement.

**Goal:** Prove the pole identities, the normal-derivative formula, and its strict positivity.

1.1 At $p$, $T=0$ gives $f=0$ and $A_0=\operatorname{id}$. Since $\sigma=f+i\psi$ with real $\psi$, $\overline\sigma=-\sigma$ there. The metric formula gives $g_0=(d_0/4)g$, and denominator positivity gives $d_0>0$. Substitution into the inverse relation yields the displayed pole relation; in particular $1-\sigma$ and $1+\sigma=1-\overline\sigma$ are nonzero. [given, F1, F2]

2.1 Evaluate the real part of the pole relation on $(n,\nu)$. By the normal form its right-hand side has real value $\operatorname{Re}((1-\sigma)/(1+\sigma))$. The real part of $\mathcal F(n,\nu)$ is $(\nabla_nT^\flat)(\nu)=g(\nabla_nT,\nu)$. Because $\sigma$ is purely imaginary at $p$, $1/(1-\sigma)$ and $1/(1+\sigma)$ are conjugates, so the displayed real part equals $2\operatorname{Re}(1/(1-\sigma))-1$. The difference of two connections applied to $T$ is tensorial and vanishes where $T=0$; hence $\nabla^{(0)}_nT=\nabla_nT$ at $p$, and the metric scaling gives the stated contraction identity. [F1, F3, step 1.1, algebra]

2.2 The flows of $K$ and $Z$ preserve $g_0$: they preserve every factor in the Harrison metric formula. Let $\phi_t$ be the flow of $Z$, fixing $p$. Since $K=T+\Omega_HZ$ and this flow preserves $T$, $[Z,K]=0$. Thus its differential $P_t=(d\phi_t)_p$ commutes with the differential of the $K$-flow at $p$, and hence with its infinitesimal generator $B(v)=\nabla_vK|_p$. Since $K|_S=0$, $B$ vanishes on $T_pS$; the Killing equation makes $B$ skew with respect to $g$, so it preserves the $g$-normal plane. Its restriction there is the supplied nonzero boost, which is invertible, giving $\ker B=T_pS$. Commutation therefore makes $P_t$ preserve $T_pS$ and, because $P_t$ is a $g$-isometry, its $g$-orthogonal normal plane. The positive conformal relation at $p$ makes this the $g_0$-normal plane as well. The continuous family $P_t$, starting at the identity, preserves its future cone. At the fixed point $p$, average any future $g_0$-unit timelike normal over this periodic differential action. In an orthonormal normal frame, each averaged vector has time component larger than the absolute value of its spatial component; compactness and the triangle inequality make the average future timelike. Normalize it to obtain an invariant future unit normal $\bar n$, and let $\bar\nu$ be its outward unit orthogonal normal. Differentiating the fixed vector relation under the flow gives $\nabla^{(0)}_{\bar n}Z=0$ at $p$, since $Z(p)=0$. [F1, F4, F5, step 1.1]

3.1 At $p$, the connection difference also vanishes on $K$, because $K(p)=0$. Thus the supplied boost action holds for $\nabla^{(0)}K$ as well. The two metrics are positive constant multiples at this point, so their future/outward normal planes agree and the same boost rate sends $\bar n$ to $\kappa\bar\nu$. Using $K=T+\Omega_HZ$ and step 2.2 gives $g_0(\nabla^{(0)}_{\bar n}T,\bar\nu)=\kappa>0$. Step 2.1 therefore gives the positive value $4\kappa/d_0$ for the scalar expression. Since that expression is independent of the chosen oriented normal frame, the same positivity holds for the original $n,\nu$, proving the inequality. [F4, step 1.1, step 2.1, step 2.2, algebra] ∎

## Source notes

The original article is cited for attribution of the pole calculation. The proof above uses the stated completed suppliers and does not use the article's assertion as a premise.

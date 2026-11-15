---
id: pthm-harrison-denominator-asymptotics
title: Uniform denominator and one-form estimates
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-stationary-asymptotic-decay-data
  - def-harrison-one-form-family
  - pthm-ernst-and-one-form-decay
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-harrison-one-form-family: mathematical-premise
  pthm-ernst-and-one-form-decay: physical-result
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 10, §2.3, denominator expansion and one-form estimate
      attribution: The article states the uniform denominator expansions and
        comparability, the pole bound, and the spatial one-form estimate for its
        radial choice; this citation supplies attribution only.
      hypotheses: The article's mass-one stationary vacuum construction, its chosen
        pole and its radial choice of the spatial primitive near infinity, with
        q in [0,1].
      reading_limits: Read the frozen article text at the cited passage and the radial
        choice on page 9. The citation attributes the claims; the proof below
        uses the declared inputs and a local calculation.
physical_scope: Conditional deduction in the smooth four-dimensional stationary
  vacuum model with the stated mass-one asymptotic end; no measurement is
  asserted.
dependency_level: 8
---

## Statement

Assume the stationary vacuum model and regular stationary spacetime data with mass parameter $M_0=1$ in the original stationary Cartesian end, $T=\partial_t$, and a supplied normalized Ernst potential $\sigma=f+i\psi$, where $f=-g(T,T)$. Let $U$ be an open set carrying this potential and containing the designated end and a supplied pole $p$ with $T_p=0$. For $q\in[0,1]$, use the pointwise definitions $D_q=|q(1+\sigma)+(1-\sigma)|^2$ on $U$ and $d_q=D_q(p)$ from the one-form-family construction.

Let $W_0$ be a supplied smooth real stationary normalized primitive on $U$ for that construction: $dW_0=\Theta_0=4((f-1)F+\psi\star_gF)$ and $W_0(T)=d_0-D_0$, where $F=\tfrac12dT^\flat$, $T^\flat=g(T,\cdot)$ and $\star_g$ is the oriented Lorentzian Hodge star. Set $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. In the radial case, assume that this supplied full normalized primitive has the spatial components of the radial primitive in the Ernst-decay result on the end. Alternatively, assume $(W_0)_i=O_5(r^{-3})$ in the same original chart. The radial case requires compatibility with the stated full primitive conditions; the spatial radial formula alone does not assert such a choice exists. In the alternative case the differentiated decay is a hypothesis, not a claim that the primitive equals the radial integral.

Uniformly for $q\in[0,1]$ and sufficiently large $r=|x|$,
$$D_q=[(1+q)-(1-q)f]^2+(1-q)^2\psi^2=4(q+(1-q)/r)^2+qO_5(r^{-2})+O_5(r^{-3})=4(q+r^{-1})^2+O_5(q^2r^{-1}+qr^{-2}+r^{-3}).$$
There are positive constants $c,C$ and one radius, independent of $q$, such that $c(q+r^{-1})^2\leq D_q\leq C(q+r^{-1})^2$ beyond that radius. At the pole, $d_q=(1+q)^2+(1-q)^2\psi(p)^2$ is bounded above and away from zero uniformly in $q\in[0,1]$. Also $(W_q)_i=(1-q)^2(W_0)_i-4q(1-q)g_{0i}=(q+r^{-1})O_5(r^{-2})$.

Here $O_5$ denotes bounds through five Cartesian spatial derivatives, with constants and radius uniform in $q$. In the last estimate it means explicitly $|\partial^\beta(W_q)_i|\leq C_\beta(qr^{-2-|\beta|}+r^{-3-|\beta|})$ for $|\beta|\leq5$. The weighted sums inside $O_5$ in the denominator display have the analogous derivative meaning.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-stationary-asymptotic-decay-data]]

[[def-harrison-one-form-family]]

[[pthm-ernst-and-one-form-decay]]

## Facts & Assumptions

[A1] The stationary vacuum model and regular spacetime data supply the stated mass-one stationary end. In its coordinates $T=\partial_t$ and $g_{0i}=O_6(r^{-2})$. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-stationary-asymptotic-decay-data]]

[F1] On that end $f=1-2/r+O_6(r^{-2})$ and $\psi=O_6(r^{-2})$. The spatial radial primitive in the decay supplier has components $O_5(r^{-3})$. In the radial case the Statement supplies a full normalized primitive whose spatial components equal those components; in the alternative case the same spatial bound is supplied directly. Only that bound, not the exact radial coefficients, enters the one-form estimate. [[pthm-ernst-and-one-form-decay]] [[def-stationary-asymptotic-decay-data]]

[F2] The one-form-family construction defines $D_q=|q(1+\sigma)+(1-\sigma)|^2$ on $U$ and $d_q=D_q(p)$ for the supplied normalized potential on $U$ and the supplied point $p\in U$ where $T_p=0$. These are pointwise definitions; this application uses the construction's potential and pole hypotheses. [[def-harrison-one-form-family]]

[F3] For the same potential and pole, $W_0$ is supplied with $dW_0=4((f-1)F+\psi\star_gF)$ and $W_0(T)=d_0-D_0$. The one-form family is $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, where $T^\flat=g(T,\cdot)$. Thus the selected full primitive satisfies both requirements of the family definition; its spatial decay is supplied as in [F1]. [[def-harrison-one-form-family]]

[F4] The differentiated $O_m$ notation means the bounds on Cartesian derivatives and uniform parameter constants stated above. [[def-stationary-asymptotic-decay-data]]

## Proof

**Given:** The model, end, pole, potential and selected primitive in the Statement.

**Goal:** Prove the uniform denominator expansions, bounds, and spatial one-form estimate.

1.1 Write $f=1-2/r+e$ and $a=(1-q)e$. By [F1], $e=O_6(r^{-2})$ and $\psi=O_6(r^{-2})$, uniformly in $q$. Expanding the modulus gives $D_q=4(q+(1-q)/r)^2-4(q+(1-q)/r)a+a^2+(1-q)^2\psi^2$. The product rule and the bounds on derivatives of $r^{-1}$ show that the last three terms are $qO_5(r^{-2})+O_5(r^{-3})$, with constants independent of $q$. [given, F1, F2, F4, algebra]

2.1 Expanding the difference of the two leading squares gives $4(q+(1-q)/r)^2-4(q+r^{-1})^2=-8q(q+r^{-1})r^{-1}+4q^2r^{-2}$. This is $O_5(q^2r^{-1}+qr^{-2})$ uniformly in $q$, giving the second expansion. For $r\geq1$, $q+(1-q)/r=(q+r^{-1})-q/r$ lies between one half and one times $q+r^{-1}$. The remainder in step 1.1 has absolute value at most $C(qr^{-2}+r^{-3})\leq Cr^{-1}(q+r^{-1})^2$. Taking one sufficiently large radius makes it at most half the positive leading term. This gives both comparison bounds with constants independent of $q$. [given, F4, step 1.1, algebra]

3.1 At $p$, $T_p=0$ implies $f(p)=0$. The modulus formula therefore gives $d_q=(1+q)^2+(1-q)^2\psi(p)^2$. It lies between $1$ and $4+\psi(p)^2$ for $q\in[0,1]$. In the stationary chart $T^\flat_i=g_{0i}$, so [F3] gives the displayed expression for $(W_q)_i$. Applying the derivative bounds in [A1] and [F1], and using $0\leq q,1-q\leq1$, yields $|\partial^\beta(W_q)_i|\leq C_\beta(r^{-3-|\beta|}+qr^{-2-|\beta|})$ for $|\beta|\leq5$. The derivative estimate uses only the spatial decay of the selected primitive in [F1], so it proves both permitted cases without equating their coefficients. The scalar denominator and pole calculations do not use any primitive coefficients. These are the asserted uniform estimates. [given, A1, F1, F2, F3, F4, step 2.1, algebra] ∎

## Source notes

The cited article attributes the denominator and one-form claims for its radial choice. That conditional case and every displayed estimate are retained. The extension to any supplied stationary normalized primitive with the same differentiated spatial decay is a local consequence of the calculation, not a stronger assertion attributed to the article. An arbitrary normalized primitive need not have that decay. Existence of a compatible full primitive with exact radial spatial components, including any simultaneous smooth global and exact radial choice, is not proved here.

The pointwise denominator and pole definitions are supplied by the one-form-family construction under its explicitly matched potential and pole hypotheses. The separate maximal-section and ADM-mass-limit convention is not used by this calculation. Mass parameter one here means the coefficient in the original stationary end expansion.

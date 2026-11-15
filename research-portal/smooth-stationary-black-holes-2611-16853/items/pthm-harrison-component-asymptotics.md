---
id: pthm-harrison-component-asymptotics
title: Uniform transformed component estimates
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - pthm-harrison-coordinate-components
  - pthm-harrison-denominator-asymptotics
  - def-regular-stationary-vacuum-spacetime
  - post-stationary-vacuum-model
  - def-stationary-asymptotic-decay-data
  - def-stationary-lorentzian-data
  - def-harrison-normalization
  - def-harrison-one-form-family
  - def-harrison-one-form
  - math:thm-algebra-of-derivatives
dependency_roles:
  pthm-harrison-coordinate-components: physical-result
  pthm-harrison-denominator-asymptotics: physical-result
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  post-stationary-vacuum-model: physical-assumption
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-harrison-one-form-family: mathematical-premise
  def-harrison-one-form: mathematical-premise
  math:thm-algebra-of-derivatives: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 7, Section 2.1, opening conventions; pages 10–11, Section 2.3,
        equations (2.11)–(2.13)
      hypotheses: The article's mass-one stationary vacuum construction, original
        stationary end, chosen pole and radial primitive, with q in [0,1].
      reading_limits: Read the frozen text and PDF images on page 7 for the original
        maximal section and mass-one conventions and pages 10–11 for the
        component estimates. This citation supplies attribution only; the proof
        uses the declared component and denominator suppliers and local
        estimates.
physical_scope: Conditional calculation in the classical four-dimensional
  stationary vacuum model and its supplied Harrison-transformed metric; no
  measurement is asserted.
dependency_level: 9
---

## Statement

Adopt the stationary vacuum model and regular stationary spacetime data with mass parameter one and original stationary Cartesian end coordinates $(t,x^i)$, so $T=\partial_t$ and $r=|x|$. Assume also that the original smooth spacelike maximal exterior section $\Sigma_1$ is supplied, with end coordinates $x^i$ and an ADM mass limit that exists and equals one, as required by the mass-one normalization. Take the supplied normalized Ernst potential $\sigma=f+i\psi$, where $f=-g(T,T)$, and a supplied pole $p$ on the bifurcation sphere $S$ with $T_p=0$. For $q\in[0,1]$ put $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $d_q=D_q(p)$. Use the supplied Harrison one-form family $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, with spatial components $(W_0)_i=O_5(r^{-3})$ in the original chart, and the corresponding transformed metric $g_q$ on the end where $D_q>0$. This includes the radial choice in the denominator estimate; a supplied smooth stationary primitive with the same differentiated decay is also permitted, without equality to the radial integral. The supplied $W_q$ is assumed to satisfy the stationarity, exterior-derivative and contraction conditions of the Harrison one-form definition, and $g_q$ is the metric defined there.

Write $a=q+r^{-1}$ and $B=q^2r^{-1}+qr^{-2}+r^{-3}$. Uniformly for $q\in[0,1]$ and sufficiently large $r$,
$$(g_q)_{00}=-\frac{d_q^2}{16}a^{-2}+a^{-4}O_5(B),\qquad (g_q)_{0i}=d_q a^{-1}O_5(r^{-2}),$$
$$g_{0i}(W_q)_j=O_5(r^{-4}),\qquad \frac{f(W_q)_i(W_q)_j}{D_q}=O_5(r^{-4}),$$
$$(g_q)_{ij}=\frac{D_q}{4}(\delta_{ij}+O_5(r^{-1}))+O_5(r^{-4})=a^2\delta_{ij}+O_5(B).$$

Here $O_5$ denotes Cartesian spatial derivative bounds through order five with one radius and constants uniform in $q$ and angle. In particular, $O_5(B)$ means a remainder $R_q$ satisfying $|\partial^\beta R_q|\le C_\beta(q^2r^{-1-|\beta|}+qr^{-2-|\beta|}+r^{-3-|\beta|})$ for $|\beta|\le5$. An expression such as $a^{-4}O_5(B)$ denotes the product of the displayed factor and such a remainder; similarly for $a^{-1}O_5(r^{-2})$.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-stationary-lorentzian-data]]

[[def-stationary-asymptotic-decay-data]]

[[def-harrison-normalization]]

[[def-harrison-one-form-family]]

[[def-harrison-one-form]]

[[pthm-harrison-coordinate-components]]

[[pthm-harrison-denominator-asymptotics]]

## Facts & Assumptions

[A1] The model and regular data give the stationary end, $f=1+O_6(r^{-1})$, $g_{0i}=O_6(r^{-2})$, and $g_{ij}=\delta_{ij}+O_6(r^{-1})$ in the stated chart. The differentiated estimates and their parameter uniformity have the meaning in the Statement. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-stationary-lorentzian-data]] [[def-stationary-asymptotic-decay-data]]

[A2] The original smooth spacelike maximal exterior section $\Sigma_1$ is supplied, and the ADM mass limit of its end in $x^i$ exists and equals one. These are the section and normalization hypotheses of the component supplier, not existence or convergence conclusions of this item. [[def-harrison-normalization]] [[pthm-harrison-coordinate-components]]

[A3] The supplied family satisfies the Harrison one-form definition's stationarity, exterior-derivative and contraction conditions; in particular $W_q(T)=d_q-D_q$, and $g_q$ is its defined metric on the positivity domain. [[def-harrison-one-form]]

[F1] For the specified potential and pole, and either permitted one-form choice with its stated spatial decay, $D_q=4a^2+O_5(B)$, $ca^2\le D_q\le Ca^2$, $d_q$ is uniformly bounded, and $(W_q)_i$ has derivatives bounded by $C_\beta(qr^{-2-|\beta|}+r^{-3-|\beta|})$ through order five, uniformly in $q$. [[def-harrison-normalization]] [[def-harrison-one-form-family]] [[pthm-harrison-denominator-asymptotics]]

[F2] On a stationary chart where $D_q>0$, the transformed components are $(g_q)_{00}=-d_q^2f/(4D_q)$, $(g_q)_{0i}=\frac{d_q}{4}(g_{0i}-f(W_q)_i/D_q)$, and $(g_q)_{ij}=\frac14(D_qg_{ij}+g_{0i}(W_q)_j+g_{0j}(W_q)_i-f(W_q)_i(W_q)_j/D_q)$. [[pthm-harrison-coordinate-components]] The same identities are derived directly in Proof 1.1 from the supplied one-form definition under the present local hypotheses; the proof does not require importing any additional global section hypothesis from that supplier.

[F3] For real functions differentiable at a limit point of their common real domain, sums, scalar multiples and products are differentiable with the usual sum, scalar-multiple and product rules. Where the denominator is nonzero, their quotient is differentiable on the nonzero-denominator set and obeys the quotient rule. [[math:thm-algebra-of-derivatives]]

[F4] For the supplied Harrison one-form, $A_qv=v+D_q^{-1}W_q(v)T$, $g_q=(D_q/4)A_q^*g$ and $W_q(T)=d_q-D_q$. Here $T^\flat=g(T,\cdot)$ and $g(T,T)=-f$. These are the defining algebraic identities on the positive-denominator domain; no exterior-access conclusion is part of this definition. [[def-harrison-one-form]]

## Proof

**Given:** The model, end, supplied original maximal exterior section and its ADM mass-one normalization, potential, pole, selected one-form family and transformed metric in the Statement.

**Goal:** Establish all displayed estimates with constants uniform for $q\in[0,1]$.

1.1 First derive the exact component identities from the supplied data in F4. Evaluating the pullback on arbitrary tangent vectors gives $4g_q=D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q$. In the stationary chart, put $w_0=(W_q)_0=d_q-D_q$ and use $g_{00}=-f$. Its time-time component is $-f(D_q+2w_0+w_0^2/D_q)/4=-fd_q^2/(4D_q)$. Its mixed component is $((D_q+w_0)g_{0i}-f(1+w_0/D_q)(W_q)_i)/4=(d_q/4)(g_{0i}-f(W_q)_i/D_q)$. Its spatial component is $(D_qg_{ij}+g_{0i}(W_q)_j+g_{0j}(W_q)_i-f(W_q)_i(W_q)_j/D_q)/4$. Thus the component formulas recorded in F2 hold directly under the stated one-form hypotheses, without a separate global maximality application. Apply [F3] on open Cartesian coordinate-line intervals in the end, with $q$ fixed, and iterate in coordinate directions through total order five. The supplied fields are smooth there; $D_q>0$ by [F1] and $a>0$, so the quotient rule applies to their reciprocals. Repeated product differentiation gives finite sums of products of derivatives, with combinatorial coefficients independent of $q$. In either permitted case the selected primitive has the denominator supplier's differentiated spatial decay in the same original chart; all its potential, pole and family data agree with the present data, so [F1] applies to this very family. For every spatial multi-index $\beta$ through order five, derivatives of $a$ obey $|\partial^\beta a|\le C_\beta a r^{-|\beta|}$: for positive order this follows from derivatives of $r^{-1}$ and $r^{-1}\le a$. Since $q\ge0$, $B\le a^2r^{-1}=q^2r^{-1}+2qr^{-2}+r^{-3}\le2B$. The expansion in [F1] and this comparison, applied at each differentiated order, give $|\partial^\beta D_q|\le C_\beta a^2r^{-|\beta|}$. Differentiating $D_qD_q^{-1}=1$ inductively and using the lower bound in [F1] yields $|\partial^\beta D_q^{-1}|\le C_\beta a^{-2}r^{-|\beta|}$. Likewise derivatives of $a^{\pm k}$ have the corresponding bounds $C_\beta a^{\pm k}r^{-|\beta|}$ for each fixed nonnegative integer $k$. All constants are independent of $q$. [given, F1, F3, F4, algebra]

2.1 By [A1] and [F1], $4a^2f-D_q=O_5(B)$: indeed $a^2(f-1)=O_5(a^2r^{-1})=O_5(B)$. Therefore $a^4(f/D_q-1/(4a^2))=a^2(4a^2f-D_q)/(4D_q)=O_5(B)$, by the product rule [F3] and step 1.1. Substitution in the first formula of [F2], with uniformly bounded $d_q$, gives the time-time estimate. [A1, A2, F1, F2, F3, step 1.1, algebra]

2.2 The one-form bound in [F1] says $|(\partial^\beta W_q)_i|\le C_\beta a r^{-2-|\beta|}$. The product rule [F3], [A1], and step 1.1 give $g_{0i}(W_q)_j=O_5(r^{-4})$ and $f(W_q)_i(W_q)_j/D_q=O_5(r^{-4})$. They also give $a\,f(W_q)_i/D_q=O_5(r^{-2})$ and $a g_{0i}=O_5(r^{-2})$, since $a\le2$ for $r\ge1$. The mixed component formula in [F2] consequently yields $(g_q)_{0i}=d_q a^{-1}O_5(r^{-2})$. [A1, F1, F2, F3, step 1.1, algebra]

3.1 The spatial formula in [F2], [A1], and step 2.2 give $(g_q)_{ij}=\frac{D_q}{4}(\delta_{ij}+O_5(r^{-1}))+O_5(r^{-4})$. By [F1], $D_q/4=a^2+O_5(B)$; moreover $D_qO_5(r^{-1})=O_5(a^2r^{-1})=O_5(B)$ and $r^{-4}\le B$ for $r\ge1$. The product rule [F3] establishes the same bounds after every permitted derivative, proving the final spatial estimate. [A1, F1, F2, F3, step 1.1, step 2.2, algebra] ∎

## Source notes

The article states the uniform transformed time-time, mixed and spatial component estimates and the two intermediate spatial product estimates. Its citation records attribution only. The proof is a local application of the declared component and denominator results; it does not use the article's assertion as a premise. Its original radial case is retained. The extension to a supplied stationary primitive with the same differentiated spatial decay uses exactly the same estimates and is locally authored; it asserts neither equality of gauges nor the unresolved simultaneous smooth-global/exact-radial assertion.

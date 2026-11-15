---
id: pthm-ernst-and-one-form-decay
title: Mass-one Ernst and radial primitive asymptotics
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-stationary-lorentzian-data
  - def-stationary-asymptotic-decay-data
  - def-complex-self-dual-two-form-data
  - def-killing-ernst-notation
  - pthm-ernst-potential-existence
  - thm-vacuum-killing-ernst-input
  - lem-author-9e1b6fa65528-radial-exterior-primitive
  - physics:lem-emg-lorentz-hodge-calculus
  - math:prop-interior-product-on-forms-is-a-graded-antiderivation
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  pthm-ernst-potential-existence: physical-result
  thm-vacuum-killing-ernst-input: mathematical-premise
  lem-author-9e1b6fa65528-radial-exterior-primitive: mathematical-premise
  physics:lem-emg-lorentz-hodge-calculus: mathematical-premise
  math:prop-interior-product-on-forms-is-a-graded-antiderivation: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 9, §2.2, before and at equation (2.10)
      statement: In the mass-one stationary end the article states the displayed
        estimates for the Killing form, its Hodge dual, the Ernst potential,
        Theta_0, and the radial formula for W_0.
      hypotheses: The article's regular stationary vacuum setting and its mass-one
        asymptotic coordinates.
      reading_limits: Read the frozen article text at the cited passage. This
        reference attributes the claim; it is not used as proof of the estimates
        or their prerequisites.
physical_scope: Conditional deductions in the smooth four-dimensional stationary
  vacuum model with the stated asymptotic end; no measurement or existence of a
  spacetime is asserted.
dependency_level: 7
---

## Statement

Assume the regular stationary vacuum model and its stationary end coordinates $(t,x^1,x^2,x^3)$ with mass parameter one. Put $r=|x|$, $f=-g(T,T)$, $F=\tfrac12dT^\flat$, and let $\sigma=f+i\psi$ be the Ernst potential normalized to tend to one at infinity. Let $\star_g$ be the oriented Lorentzian Hodge star and $\Theta_0=4((f-1)F+\psi\star_gF)$. Then, in these coordinates,
$$f=1-2/r+O_6(r^{-2}),\qquad F_{ij}=\tfrac12(\partial_i g_{0j}-\partial_j g_{0i})=O_5(r^{-3}),\qquad (\star_gF)_{ij}=O_5(r^{-2}).$$
Moreover $\partial_i\psi=O_5(r^{-3})$, $\psi=O_6(r^{-2})$, $\sigma=1-2/r+O_6(r^{-2})$, and $(\Theta_0)_{ij}=O_5(r^{-4})$. The spatial restriction of $\Theta_0$ is closed, and its radial primitive has components
$$(W_0)_i(x)=-\int_1^\infty s x^j(\Theta_0)_{ji}(sx)\,ds=O_5(r^{-3}).$$
Here $O_m(r^{-b})$ means the stated bound and corresponding bounds after each Cartesian spatial derivative of order at most $m$. The radial formula specifies spatial components on the end; it does not by itself assert a global or horizon-regular choice of $W_0$.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-stationary-lorentzian-data]]

[[def-stationary-asymptotic-decay-data]]

[[def-complex-self-dual-two-form-data]]

[[def-killing-ernst-notation]]

[[pthm-ernst-potential-existence]]

## Facts & Assumptions

[A1] Adopt the stationary vacuum model and the regular-spacetime hypotheses, including the fixed stationary Cartesian end and mass parameter $M_0=1$. Thus $T=\partial_t$, the metric is independent of $t$, $g_{00}=-1+2/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$, and $g_{ij}=\delta_{ij}+O_6(r^{-1})$. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-stationary-asymptotic-decay-data]]

[F1] The stationary and Ernst conventions define $T^\flat=g(T,\cdot)$, $f=-g(T,T)$, $F=\tfrac12dT^\flat$, $\mathcal F=F+i\star_gF$, and the normalized potential by $d\sigma=2\iota_T\mathcal F$ and $\sigma\to1$. The potential exists under [A1]. [[def-stationary-lorentzian-data]] [[def-complex-self-dual-two-form-data]] [[def-killing-ernst-notation]] [[pthm-ernst-potential-existence]]

[F2] In vacuum, $dF=d\star_gF=0$. On the end, define $\Theta_0$ directly by $\Theta_0=4((f-1)F+\psi\star_gF)$, using the fields in [F1]. [[thm-vacuum-killing-ernst-input]]

[F3] A closed spatial $C^5$ two-form with coefficients $O_5(r^{-4})$ has the displayed radial primitive, with components $O_5(r^{-3})$. [[lem-author-9e1b6fa65528-radial-exterior-primitive]]

[F4] On an oriented, time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$, the Hodge star is characterized by $P\wedge\star_gQ=\langle P,Q\rangle_g\,\mathrm{vol}_g$, where for real two-forms $\langle P,Q\rangle_g=\tfrac12P_{ab}Q^{ab}$, and $\star_g^2=-\operatorname{id}$ on two-forms. Its coordinate component formula and the coordinate formula for $d$ apply, and $d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^k\alpha\wedge d\beta$ for a $k$-form $\alpha$. [[physics:lem-emg-lorentz-hodge-calculus]]

[F5] For a smooth vector field $X$ and a $k$-form $\alpha$, contraction satisfies $\iota_X(\alpha\wedge\beta)=(\iota_X\alpha)\wedge\beta+(-1)^k\alpha\wedge\iota_X\beta$. [[math:prop-interior-product-on-forms-is-a-graded-antiderivation]]

## Proof

**Given:**The model, end coordinates, and normalized potential in the Statement.

**Goal:** Establish the differentiated estimates and the radial primitive.

1.1 Since $T=\partial_t$, $f=-g_{00}$ and $T^\flat=g_{0\mu}dx^\mu$. Stationarity and [A1] give the claimed expansion for $f$, $F_{ij}=\tfrac12(\partial_i g_{0j}-\partial_j g_{0i})=O_5(r^{-3})$, and $F_{0i}=-\tfrac12\partial_i g_{00}=O_5(r^{-2})$. Inverting the metric near its Minkowski limit gives $g^{00}=-1+O_6(r^{-1})$, $g^{0i}=O_6(r^{-2})$, and $g^{ij}=\delta^{ij}+O_6(r^{-1})$; the same derivative bounds follow by differentiating $g^{-1}g=I$. The metric volume coefficients and their spatial derivatives through order five are bounded. In the Hodge component formula, the spatial components involve $F^{0k}=O_5(r^{-2})$, whereas $(\star_gF)_{0i}$ involves $F^{jk}=O_5(r^{-3})$. Consequently $(\star_gF)_{ij}=O_5(r^{-2})$ and $(\star_gF)_{0i}=O_5(r^{-3})$. [A1, F1, F4, algebra]

1.2 For real two-forms, the component pairing in [F4] is symmetric because $g^{-1}$ is symmetric. Apply its Hodge characterization first to $(P,Q)=(\star_gF,F)$ and then to $(P,Q)=(F,\star_gF)$ to obtain $\star_gF\wedge\star_gF=\langle\star_gF,F\rangle_g\,\mathrm{vol}_g=\langle F,\star_gF\rangle_g\,\mathrm{vol}_g=F\wedge\star_g(\star_gF)=-F\wedge F$. Thus $F\wedge F+\star_gF\wedge\star_gF=0$. [F4, algebra]

2.1 Taking the imaginary part of $d\sigma=2\iota_T(F+i\star_gF)$ yields $\partial_i\psi=2(\star_gF)_{0i}=O_5(r^{-3})$. Since $\psi\to0$, integration along the ray from $r$ to infinity gives $\psi=O(r^{-2})$ uniformly in angle. Every nonzero spatial derivative of order at most six is a derivative of some $\partial_i\psi$, giving $\psi=O_6(r^{-2})$. Combining this with the expansion of $f$ gives the stated expansion of $\sigma$. The product rule in $\Theta_0=4((f-1)F+\psi\star_gF)$ now gives $(\Theta_0)_{ij}=O_5(r^{-4})$. [F1, step 1.1, algebra]

3.1 By [F1], $df=2\iota_TF$ and $d\psi=2\iota_T\star_gF$. The derivative product rule in [F4] and the vacuum identities in [F2] give $d\Theta_0=8((\iota_TF)\wedge F+(\iota_T\star_gF)\wedge\star_gF)$. Moving a one-form past a two-form makes two sign changes, so the contraction rule [F5] gives $\iota_T(F\wedge F+\star_gF\wedge\star_gF)=2((\iota_TF)\wedge F+(\iota_T\star_gF)\wedge\star_gF)$. The left side vanishes by step 1.2, hence $d\Theta_0=0$. In the coordinate formula for $d$, its purely spatial coefficients are exactly the closure equations for the spatial restriction of $\Theta_0$. That restriction has smooth coefficients and the $O_5(r^{-4})$ bounds from step 2.1, so [F3] applies on a sufficiently far-out exterior and proves both the displayed integral formula and its five differentiated decay bounds. [F1, F2, F3, F4, F5, step 2.1, step 1.2, algebra] ∎



The article citation records attribution of the original claim. The argument above uses the declared model, geometric definitions, vacuum identities, normalized-potential result, and radial primitive lemma.

## Source notes

The article citation records attribution of the original claim. The argument above uses the declared model, geometric definitions, vacuum identities, normalized-potential result, and radial primitive lemma.

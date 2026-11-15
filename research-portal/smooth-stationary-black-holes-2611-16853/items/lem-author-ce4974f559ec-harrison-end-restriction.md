---
id: lem-author-ce4974f559ec-harrison-end-restriction
title: Harrison spatial two-form differs from the seed by an integrable tail
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-asymptotic-decay-data
  - def-complex-self-dual-two-form-data
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:thm-coordinate-formula-for-the-differential
  - math:def-wedge-product-of-differential-forms
  - math:def-pullback-of-a-differential-form
  - math:def-axiom-of-choice
dependency_roles:
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  math:def-complex-conjugate-real-imaginary-part-and-modulus: mathematical-premise
  math:thm-coordinate-formula-for-the-differential: mathematical-premise
  math:def-wedge-product-of-differential-forms: mathematical-premise
  math:def-pullback-of-a-differential-form: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Work in ZFC. Let an end chart on a smooth, oriented and time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$ be $(t,x):U_{\mathrm{end}}\to I\times E$, where $I$ is an open interval containing $0$ and $E=\{x\in\mathbb R^3:r=|x|>R_0\}$ with $R_0>0$. Assume $T=\partial_t$ in this same chart and write $T^\flat=g(T,\cdot)$ and $g_{0i}=g(\partial_t,\partial_{x^i})$. Supply a smooth complex function $\sigma$, a smooth real one-form $W_0$, and a smooth real two-form $F$ on this end, and put $\mathcal F=F+i\star_gF$, using the supplied orientation.

Fix $0<q<1$ and put $a_q=\sqrt{1-q^2}$. On the slice $t=0$ assume the Cartesian component bounds $\sigma=1-2/r+O_1(r^{-2})$, $g_{0i}=O_1(r^{-2})$, $(W_0)_i=O(r^{-3})$, and $\mathcal F_{ij}=O(r^{-2})$, where $1\leq i,j\leq3$, $O=O_0$, and every bound is uniform over spatial directions. Define the local expressions

$$W_q=(1-q)^2W_0-4q(1-q)T^\flat,\qquad B_q=(1+q)-(1-q)\sigma,\qquad D_q=|B_q|^2,$$

and, on the open set where $D_q>0$, define the two-form by the explicit algebraic formula

$$\mathcal H_q=-a_q\frac{\overline B_q}{B_q}\left(\mathcal F+\frac{W_q\wedge d\sigma}{2D_q}\right).$$

For all sufficiently large $r$ on $t=0$, $D_q>0$ and, writing $\iota_0(x)=(0,x)$, one has $\iota_0^*\mathcal H_q=-a_q\iota_0^*\mathcal F+E_q$, where $E_q$ is a complex two-form on that spatial end with Cartesian coefficients $(E_q)_{ij}=O_q(r^{-3})$. In particular the same identity holds after restriction to each sufficiently large spatial coordinate sphere. The constants and the starting radius may depend on this fixed positive $q$; no estimate uniform as $q\downarrow0$ is asserted.

## Statement references

[[def-stationary-asymptotic-decay-data]]

[[def-complex-self-dual-two-form-data]]

[[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

[[math:def-complex-conjugate-real-imaginary-part-and-modulus]]

[[math:thm-coordinate-formula-for-the-differential]]

[[math:def-wedge-product-of-differential-forms]]

[[math:def-pullback-of-a-differential-form]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

[A1] ZFC supplies the background choice assumption inherited by the geometric suppliers. The coefficient estimates below use only finite algebra in the supplied chart. [[math:def-axiom-of-choice]]

[F1] For the supplied smooth Lorentzian metric, the metric dual is $T^\flat(v)=g(T,v)$ and $g_{0i}=g(\partial_t,\partial_{x^i})$. [[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

[F2] On the supplied oriented Lorentzian four-manifold, a complex two-form has real and imaginary parts, and $\mathcal F=F+i\star_gF$ uses the smooth metric Hodge star extended complex linearly. [[def-complex-self-dual-two-form-data]]

[F3] The bounds $O_m(r^{-b})$ control all Cartesian derivatives of order at most $m$ by constants times $r^{-b-|\beta|}$, uniformly over directions; a fixed-parameter bound permits constants and starting radius to depend on $q$. [[def-stationary-asymptotic-decay-data]]

[F4] For $z=u+iv$, complex conjugation is $\overline z=u-iv$ and $|z|=(u^2+v^2)^{1/2}$, so $|z|^2=z\overline z$. [[math:def-complex-conjugate-real-imaginary-part-and-modulus]]

[F5] The differential of a smooth scalar has coordinate components given by its partial derivatives; for complex $\sigma$ this is applied separately to its real and imaginary parts. [[math:thm-coordinate-formula-for-the-differential]]

[F6] The wedge product is the pointwise alternating product: for one-forms $\alpha,\beta$, $(\alpha\wedge\beta)_{ij}=\alpha_i\beta_j-\alpha_j\beta_i$, extended complex linearly. [[math:def-wedge-product-of-differential-forms]]

[F7] Restriction to a slice or sphere is pullback by its smooth inclusion, evaluated on its tangent vectors. In particular $dt$ pulls back to zero on $t=0$. [[math:def-pullback-of-a-differential-form]]

## Proof

**Given:** The supplied end chart, smooth fields, fixed parameter, local formulas and spatial bounds in the Statement; work in ZFC.

**Goal:** Establish eventual positivity and the spatial error estimate.

**Proof technique:** direct.

1.1 Since $\sigma=1+O(r^{-1})$, the given formula gives $B_q=2q+O_q(r^{-1})$. Increase the radius until $|B_q-2q|\leq q$; then $|B_q|\geq q>0$ and $D_q\geq q^2$. Expanding $B_q\overline B_q$ gives $D_q=4q^2+O_q(r^{-1})$ and $D_q^{-1}=O_q(1)$. Also $\overline B_q/B_q-1=(\overline B_q-B_q)/B_q=O_q(r^{-1})$, since $2q$ is real. All these estimates are on $t=0$ and are uniform in spatial directions. [given, F3, F4, algebra]

1.2 The adapted-chart hypothesis and the metric dual give $(T^\flat)_i=T^\flat(\partial_{x^i})=g(\partial_t,\partial_{x^i})=g_{0i}$. Hence $W_{q,i}=(1-q)^2(W_0)_i-4q(1-q)g_{0i}=O_q(r^{-2})$. Differentiating the given spatial expansion yields $\partial_i\sigma=2x^i/r^3+O(r^{-3})=O(r^{-2})$. Therefore $(W_q\wedge d\sigma)_{ij}=W_{q,i}\partial_j\sigma-W_{q,j}\partial_i\sigma=O_q(r^{-4})$. The pullback to $t=0$ contains exactly these spatial components; its time-component terms vanish on spatial tangent vectors. [given, F1, F3, F5, F6, F7, algebra]

2.1 Use the explicitly defined local two-form on the nonzero-denominator set found in step 1.1 and set $E_q=\iota_0^*(\mathcal H_q+a_q\mathcal F)$. Its spatial coefficients are $(E_q)_{ij}=-a_q\left(\frac{\overline B_q}{B_q}-1\right)\mathcal F_{ij}-\frac{a_q}{2D_q}\frac{\overline B_q}{B_q}(W_q\wedge d\sigma)_{ij}.$ The first term is $O_q(r^{-1})O(r^{-2})=O_q(r^{-3})$ and the second is $O_q(1)O_q(r^{-4})=O_q(r^{-4})$. This proves the asserted spatial estimate and its restriction to the coordinate spheres. The calculation uses only the stated bound on $g_{0i}$ and imposes no leading angular-momentum expansion. [given, F2, F3, F7, step 1.1, step 1.2, algebra] ∎

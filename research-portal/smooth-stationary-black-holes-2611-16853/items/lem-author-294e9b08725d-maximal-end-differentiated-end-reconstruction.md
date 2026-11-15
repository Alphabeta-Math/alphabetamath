---
id: lem-author-294e9b08725d-maximal-end-differentiated-end-reconstruction
title: The same maximal slice has the differentiated article end gauge and a
  limiting old time
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-294e9b08725d-maximal-end-critical-logarithm-exclusion
  - lem-author-294e9b08725d-maximal-end-leading-stationary-modes
  - lem-author-294e9b08725d-maximal-end-cw-weak-kid-data
  - thm-vacuum-killing-ernst-input
  - math:thm-stokes-theorem-for-smooth-singular-chains
  - math:thm-fundamental-theorem-of-riemannian-geometry
  - math:def-axiom-of-choice
  - def-stationary-lorentzian-data
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-asymptotic-decay-data
  - math:def-pullback-of-a-covariant-tensor-field
dependency_roles:
  lem-author-294e9b08725d-maximal-end-critical-logarithm-exclusion: mathematical-premise
  lem-author-294e9b08725d-maximal-end-leading-stationary-modes: mathematical-premise
  lem-author-294e9b08725d-maximal-end-cw-weak-kid-data: mathematical-premise
  thm-vacuum-killing-ernst-input: mathematical-premise
  math:thm-stokes-theorem-for-smooth-singular-chains: mathematical-premise
  math:thm-fundamental-theorem-of-riemannian-geometry: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  math:def-pullback-of-a-covariant-tensor-field: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 9
---

## Statement

Work in ZFC. Start with the smooth stationary Ricci-flat end and the already supplied smooth CW maximal graph $t=u(x)$ with the original metric and logarithmic graph bounds in [F3]. Use the final spatial normalization of that same end supplied by [F1] and [F2], retaining $\tau=t-u(x)$. The original spatial chart $x$ and the final spatial chart $z$ are end charts of this identical end; restrict them to a common neighborhood of infinity. Their transition is $t=\tau+u(x)$, $z=f(x)$, with $f$ independent of time. These are the supplied end charts, not a new hypersurface or an assumption of improved height decay. Write $r=|z|$ for the new-chart estimates and $\rho=|x|$ for original-chart estimates. Here $O_\infty$ means $O_k$ for every finite $k$, with the differentiated-order convention of [F10].

The SAME supplied CW maximal slice admits end coordinates $(\tau,z)$ with $T=\partial_\tau$ and the slice at $\tau=0$, in which
$$g_{00}=-1+2m/r+O_\infty(r^{-2}),\qquad g_{0i}=O_\infty(r^{-2}),\qquad g_{ij}=\delta_{ij}+O_\infty(r^{-1}).$$
In particular these estimates retain all six differentiated orders required in the article. With the normalized Komar convention $m_K=(4\pi)^{-1}\lim\int n^a\nu^b\nabla_aT_b\,dA$, where n is future and nu outward, the coefficient m equals $m_K$. If the original regular end has coefficient M0 in its normalized time-time component, then $m=m_K=M_0$.

Furthermore, the original logarithmic graph height has a single limiting stationary time: $u(x)=c+O(\rho^{-1})$ and $Du=O(\rho^{-2})$. This last comparison does not claim a seventh original-chart derivative. A constant translation of stationary time may set this limiting c to zero, while the adapted time tau already places the identical maximal slice at zero.

## Facts & Assumptions

[F1] The final same-slice stationary chart has a controlled $r^{-2}$ shift and a log-free second-order lapse remainder. [[lem-author-294e9b08725d-maximal-end-critical-logarithm-exclusion]]

[F2] The induced metric has its leading isotropic spatial mass term and differentiated order-minus-one error. [[lem-author-294e9b08725d-maximal-end-leading-stationary-modes]]

[F3] The original chart has its original order-six regular metric and the CW slice is its graph $t=u$(x). [[lem-author-294e9b08725d-maximal-end-cw-weak-kid-data]]

[F4] In vacuum the Killing two-form is co-closed, equivalently the Komar two-form is closed on the stationary end. [[thm-vacuum-killing-ernst-input]]

[F5] The integral of a closed smooth two-form is unchanged on homologous oriented smooth two-cycles. [[math:thm-stokes-theorem-for-smooth-singular-chains]]

[F6] Every supplied smooth Riemannian metric has a unique compatible torsion-free connection. This applies to the quotient metric only after its construction and positivity have been established. [[math:thm-fundamental-theorem-of-riemannian-geometry]]

[F7] Work in ZFC, including the inherited analytic choice assumptions. [[math:def-axiom-of-choice]]

[F8] Stationary Lorentzian data supply the smooth metric, Killing field, time orientation, Levi–Civita connection and Ricci conventions; $T$ is future timelike on the stationary end. [[def-stationary-lorentzian-data]]

[F9] The supplied spacelike maximal slice has its future unit normal, induced Riemannian metric, and lapse–shift decomposition $T=Nn+X$. [[def-spacelike-maximal-hypersurface-data]]

[F10] Differentiated end estimates mean uniform Cartesian derivative bounds in each fixed exterior chart. [[def-stationary-asymptotic-decay-data]]

[F11] For a smooth coordinate map $f$, the pullback of a covariant two-tensor is $(f^*q)_x(v,w)=q_{f(x)}(Df_xv,Df_xw)$. [[math:def-pullback-of-a-covariant-tensor-field]]

## Proof

**Given:** The actual end hypotheses in the Statement.

**Goal:** Prove the stated same-slice end consequence.

1.1 Reconstruct the spacetime tensor from its ADM fields: $g_{00}=-N^2+h(X,X)$, $g_{0i}=h_{ij}X^j$ and $g_{ij}=h_{ij}$. The preceding lapse, shift and metric estimates give all displayed differentiated bounds. Only spatial coordinates were changed after tau was chosen in [F3], so $\tau=0$ is still the original supplied maximal hypersurface. [F1, F2, F3, F8, F9, F10, given, algebra]

2.1 On a large tau-constant sphere, stationarity gives $\nabla_0T_r=-\tfrac12\partial_rg_{00}=m/r^2+O(r^{-3})$. Its future section normal is $\partial_\tau+O(r^{-1})$, its outward unit normal is radial up to order $r^{-1}$, and its area is $4\pi r^2+O(r)$. The normalized Komar limit is therefore m. The same calculation in the original regular chart gives M0. The vacuum identity in [F4] and Stokes in [F5] equate these integrals on large homologous spheres in the same stationary end, even when the spheres lie in different time sections. Thus $m=m_K=M_0$. [F1, F2, F3, F4, F5, F8, F9, F10, step 1.1, algebra]

2.2 Construct the quotient metric on the spatial orbit labels, without invoking a global quotient theorem. On the common stationary end $g_{00}<0$. The tensor $Q=g-T^\flat\otimes T^\flat/g(T,T)$ annihilates $T$ and is stationary. For a spatial vector $V$, its value is $Q(V,V)=g(V^\perp,V^\perp)$, where $V^\perp=V-g(V,T)T/g(T,T)$. Its coefficients on the old labels are $q^{\rm old}_{ij}=g^{\rm old}_{ij}-g^{\rm old}_{0i}g^{\rm old}_{0j}/g^{\rm old}_{00}$; define $q^{\rm new}$ by the same formula in the new chart. The old estimates in [F3] and step 1.1 give $q^{\rm old}=\delta+O(\rho^{-1})$ and $q^{\rm new}=\delta+O(r^{-1})$. Thus both are smooth positive-definite metrics sufficiently far out, to which [F6] applies. Substituting $dt=d\tau+du$ cancels the $du$ terms in this formula, and the spatial tensor transformation in [F11] then gives $q^{\rm old}=f^*q^{\rm new}$. This defines the Riemannian metric on the stationary orbit labels and proves the pullback identity used here. [F3, F6, F8, F11, step 1.1, algebra]

3.1 Uniform comparison of each quotient metric with its Euclidean metric and the pullback identity give constants $0<a\leq b<\infty$ with $a|v|\leq|Df_xv|\leq b|v|$ on a sufficiently far-out common end, and hence a uniform bound for $D(f^{-1})$. Since both charts describe the same end outside compact inner parts, points tending to its infinity have both $\rho\to\infty$ and $r\to\infty$. Choose a fixed old coordinate sphere beyond the inner parts. Integrating the upper bound for $Df$ along its outward radial rays gives $r\leq b\rho+C$, since the image of the initial sphere is compact. Applying the same argument to $f^{-1}$ from a fixed new coordinate sphere gives $\rho\leq a^{-1}r+C'$. After increasing the radii, $r$ and $\rho$ are therefore comparable. This uses the existing overlapping end charts, rather than postulating a Euclidean asymptotic formula for $f$. [F1, F2, F3, F11, step 2.2, algebra]

4.1 The mixed tensor identity for this same coordinate change is $g^{\rm new}_{0a}(f(x))\partial_if^a=g^{\rm old}_{0i}+g^{\rm old}_{00}\partial_i u$. The old mixed component is $O(\rho^{-2})$ by [F3], while the new one is $O(r^{-2})$ by step 1.1. Step 3.1 and $g^{\rm old}_{00}\to-1$ therefore give $Du=O(\rho^{-2})$. For each unit vector $\omega$, integration of $|\partial_\rho u(\rho\omega)|\leq C\rho^{-2}$ from $\rho$ to infinity gives a limit $c(\omega)$ and a uniform error at most $C/\rho$. Any two points on the radius-$\rho$ sphere can be joined there by an arc of length at most $\pi\rho$; integrating the same gradient bound along it gives oscillation at most $C\pi/\rho$. Passing to infinity shows that all $c(\omega)$ coincide. Hence $u=c+O(\rho^{-1})$, and a constant old-time translation sets $c$ to zero. The adapted time already has the identical slice at zero. Only first derivatives in the old chart were used in this comparison. [F3, F8, F10, F11, step 1.1, step 3.1, algebra] ∎

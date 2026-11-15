---
id: lem-author-6413ea293c6d-zero-optics-curvature
title: Zero null optics supplies the missing null Ricci condition
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-null-screen-expansion-and-focal-data
  - physics:prop-gr-fx-null-raychaudhuri
  - physics:def-gr-curvature-tensor-and-derived-tensors
dependency_roles:
  def-null-screen-expansion-and-focal-data: mathematical-premise
  physics:prop-gr-fx-null-raychaudhuri: mathematical-premise
  physics:def-gr-curvature-tensor-and-derived-tensors: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 1
---

## Statement

Let a smooth affinely parametrized null hypersurface congruence, before its first focal instant, satisfy the screen hypotheses of [[def-null-screen-expansion-and-focal-data]] and [[physics:prop-gr-fx-null-raychaudhuri]]. If its null second fundamental form vanishes identically on an open congruence neighborhood of a section, then $\operatorname{Ric}(\ell,\ell)=0$ there. At that section the same conclusion holds for every smooth nonzero rescaling $L=f\ell$. No conclusion from vanishing at a single isolated section alone is asserted.

## Facts & Assumptions

[F1] The screen definitions give the regular section metric, the screen Jacobi map $A$, the optical endomorphism $B=A' A^{-1}$, its expansion $\theta=\operatorname{tr}B$ and shear $\sigma=B-\frac12\theta\,\mathrm{id}$, and identify the initial optical data with the null second fundamental form of the initial section. [[def-null-screen-expansion-and-focal-data]]

[F2] The null Raychaudhuri supplier gives $\theta'=-\theta^2/2-|\sigma|^2-\operatorname{Ric}(\ell,\ell)$ under the stated smooth affine null hypersurface congruence hypotheses. Only this identity is used; neither a Ricci inequality nor a negative initial expansion is assumed. [[physics:prop-gr-fx-null-raychaudhuri]]

[F3] The Ricci tensor is a smooth covariant two-tensor, defined by the metric contraction of curvature, and is therefore pointwise bilinear. [[physics:def-gr-curvature-tensor-and-derived-tensors]]

## Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Establish its identities with the indicated normalizations.

1.1 Fix any regular parameter $\lambda_0$ and work locally on its spacelike section $S_{\lambda_0}$, restricting to an embedded section patch if necessary. Rebase the same congruence at that section by using $s=\lambda-\lambda_0$ and relabeling each generator by its point on $S_{\lambda_0}$. Its tangent is still $\ell$, its parameter is still affine, and its section directions are still orthogonal to $\ell$. Under the identification of $T S_{\lambda_0}$ with the screen at $\lambda_0$, its screen Jacobi map is $\widetilde A_s=A_{\lambda_0+s}A_{\lambda_0}^{-1}$. Since the right factor is fixed in $s$, $\widetilde B_s=\widetilde A_s'\widetilde A_s^{-1}=B_{\lambda_0+s}$. Apply the initial-section identification of [F1] to this rebased congruence: at $s=0$, its optical expansion and shear correspond to the trace and trace-free part of $\chi_\ell$ on $S_{\lambda_0}$. These vanish by the assumed zero second fundamental form. As the regular point and section were arbitrary, $\theta=0$ and $\sigma=0$ throughout the open congruence neighborhood, with all constructions taken on the chosen parameter-domain branch. [given, F1, construct, algebra]

2.1 The smooth function $\theta$ vanishes on this open neighborhood, so its affine derivative also vanishes there. Substitution of $\theta=0$, $\sigma=0$ and $\theta'=0$ into the identity in [F2] gives $\operatorname{Ric}(\ell,\ell)=0$ throughout that neighborhood. The open-neighborhood hypothesis is what justifies taking the derivative of the identically zero expansion; vanishing at one isolated section would not suffice. [step 1.1, F2, algebra]

3.1 At the specified section, pointwise bilinearity of the covariant two-tensor in [F3] gives $\operatorname{Ric}(f\ell,f\ell)=f^2\operatorname{Ric}(\ell,\ell)=0$ for every smooth nonzero rescaling $L=f\ell$. This pointwise rescaling needs no affine extension of $L$. [step 2.1, F3, algebra] ∎

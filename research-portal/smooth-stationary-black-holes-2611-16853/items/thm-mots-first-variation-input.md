---
id: thm-mots-first-variation-input
title: General MOTS first variation before electrovac specialization
kind: theorem
status: published
origin: pipeline
domain: mathematics
deps:
  - def-null-screen-expansion-and-focal-data
  - def-surface-area-flux-and-null-variation-data
  - def-source-free-geometric-electrovacuum-data
  - math:def-axiom-of-choice
  - lem-author-6413ea293c6d-null-variation-normalization
  - lem-author-6413ea293c6d-second-form-and-connection-signs
  - lem-author-6413ea293c6d-curvature-coefficient-conversion
  - lem-author-6413ea293c6d-electrovac-normal-contraction
  - lem-author-6413ea293c6d-zero-optics-curvature
  - physics:def-gr-metric-selected-connection
  - math:prop-scalar-curvature-is-twice-the-sum-of-sectional-curvatures-of-coordinate-planes
dependency_roles:
  def-null-screen-expansion-and-focal-data: mathematical-premise
  def-surface-area-flux-and-null-variation-data: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  lem-author-6413ea293c6d-null-variation-normalization: mathematical-premise
  lem-author-6413ea293c6d-second-form-and-connection-signs: mathematical-premise
  lem-author-6413ea293c6d-curvature-coefficient-conversion: mathematical-premise
  lem-author-6413ea293c6d-electrovac-normal-contraction: mathematical-premise
  lem-author-6413ea293c6d-zero-optics-curvature: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  math:prop-scalar-curvature-is-twice-the-sum-of-sectional-curvatures-of-coordinate-planes: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Andersson–Mars–Simon, Stability of marginally outer trapped surfaces and
        existence of marginally outer trapped tubes
      url: https://arxiv.org/pdf/0704.2889
      locator: §2, printed pp. 5–6 (null normals, second form and expansion); §3,
        printed p. 7 (immersed-surface variation and varying null normal, before
        Lemma 3.1); Lemma 3.1, printed p. 7; equations (2)–(7), Definition 3.1
        and Lemma 3.2, printed p. 8
      statement: For the supplied immersed-surface family, δ_{φv}θ_l is the derivative
        at zero of the pulled-back expansion of l_σ. At a MOTS it is independent
        of the family and changing null gauge once φv and l_0 are fixed. For
        v=−k/2+Vl, u=k/2+Vl and s_A=−g(k,∇_A l)/2, it equals L_vφ, where
        L_v=−Δ_S+2s·D+(R_S/2−Y−|s|²+div s) and Y=V K^μ_AB K^{ν AB}l_μl_ν+G(l,u).
      hypotheses: Smooth Lorentzian four-manifold with signature (−,+,+,+) and the
        source curvature convention; smooth spacelike surface with smooth future
        null normals g(l,k)=−2 and θ_l=0. For each direction φv, a smooth family
        Φ:S×I→M on a common open interval I containing zero is supplied, with
        spacelike immersed slices, Φ_0 the inclusion and initial velocity φv,
        together with smooth future nonzero null normals l_σ to those slices,
        with l_0=l. The normal v satisfies g(l,v)=1 and may have any causal
        character. Section 3 expressly allows nonclosed surfaces; no global
        existence of a variation on a noncompact S is asserted. No
        Einstein–Maxwell or horizon hypothesis enters the general formula.
      reading_limits: Consulted the PDF-extracted text of §2 and §3 through Lemma 3.2,
        printed pp. 5–8, including the variation-family paragraph, Lemma 3.1,
        equations (2)–(7) and Definition 3.1. Checked their normalization and
        application against the declared local suppliers. No page-image
        inspection, Appendix A reconstruction or independent proof of the
        covariant calculation is claimed.
dependency_level: 9
---

## Statement

Let $S$ be a smooth spacelike codimension-two surface in a smooth time-oriented Lorentzian four-manifold, with null-expansion conventions as in [[def-null-screen-expansion-and-focal-data]]. Choose smooth future null normals $l,k$ with $g(l,k)=-2$, and assume the outgoing expansion $\theta_l=0$ identically. For a smooth normal field $v$ with $g(l,v)=1$, write $v=-k/2+Vl$, $u=k/2+Vl$, $s_A=-g(k,\nabla_A l)/2$, and $Y=V|\chi_l|^2+G(l,u)$, where $G=\operatorname{Ric}-\operatorname{Scal}_g g/2$ and $|\chi_l|^2$ uses the positive surface metric. For each smooth real function $\phi$ under consideration, supply a smooth map $\Phi:S\times I\to M$ on a common open interval $I\ni0$, with $\Phi_0$ the inclusion, $\partial_\sigma\Phi|_0=\phi v$, and each $\Phi_\sigma$ a spacelike immersion. Supply also a smooth field $l_\sigma(p)\in T_{\Phi_\sigma(p)}M$ of future nonzero null normals to these slices, with $l_0=l$. Let $\theta_\sigma$ denote their null expansion pulled back to $S$; equivalently, it is the $\Phi_\sigma^*g$-trace of $(X,Y)\mapsto g(\nabla^{\Phi_\sigma}_Xl_\sigma,d\Phi_\sigma(Y))$, where $\nabla^{\Phi_\sigma}$ is the pullback connection. Define $\delta_{\phi v}\theta_l=\left.\partial_\sigma\theta_\sigma\right|_0$. At the stated MOTS this derivative depends only on $\phi v$ and the base normal $l$, not on the other choices of the supplied family and changing null gauge. On a noncompact $S$, existence of a common interval is an explicit requirement; the same formula applies locally on any supplied surface patch.

For such a supplied variation, $\delta_{\phi v}\theta_l=L_v\phi$ with
$$L_v\phi=-\Delta_S\phi+2s\cdot D\phi+(R_S/2-Y-|s|^2+\operatorname{div}_Ss)\phi.$$
Here $R_S$ is the intrinsic scalar curvature, so $R_S/2$ is the positive-round-sphere Gauss curvature in two dimensions. Use the sign agreement in [[lem-author-6413ea293c6d-second-form-and-connection-signs]]. In the outward hypersurface gauge [[def-surface-area-flux-and-null-variation-data]], take $l=L$, $k=2\underline L$, $v=\nu$; then $s=\zeta$ and $Y=|\chi_L|^2/2+G(L,n)$ by [[lem-author-6413ea293c6d-null-variation-normalization]] and [[lem-author-6413ea293c6d-curvature-coefficient-conversion]]. Thus at a geometric electrovac surface, if additionally $\chi_L=0$ and $\operatorname{Ric}(L,L)=0$, the zeroth coefficient is $K_S+\operatorname{div}\zeta-|\zeta|^2-e^2-b^2$, by [[lem-author-6413ea293c6d-electrovac-normal-contraction]]. The null Ricci condition is supplied by [[lem-author-6413ea293c6d-zero-optics-curvature]] when its actual open null-congruence hypotheses hold. Mere MOTS status does not justify this last specialization.

## Facts & Assumptions

[F1] The formulation uses [[def-null-screen-expansion-and-focal-data]] under its actual stated hypotheses.

[F2] The formulation uses [[def-surface-area-flux-and-null-variation-data]] under its actual stated hypotheses.

[F3] The formulation uses [[def-source-free-geometric-electrovacuum-data]] under its actual stated hypotheses.

[F4] The formulation uses [[math:def-axiom-of-choice]] under its actual stated hypotheses.

[F5] The formulation uses [[lem-author-6413ea293c6d-null-variation-normalization]] under its actual stated hypotheses.

[F6] The formulation uses [[lem-author-6413ea293c6d-second-form-and-connection-signs]] under its actual stated hypotheses.

[F7] The formulation uses [[lem-author-6413ea293c6d-curvature-coefficient-conversion]] under its actual stated hypotheses.

[F8] The formulation uses [[lem-author-6413ea293c6d-electrovac-normal-contraction]] under its actual stated hypotheses.

[F9] The formulation uses [[lem-author-6413ea293c6d-zero-optics-curvature]] under its actual stated hypotheses.

[F10] The metric-selected connection is metric-compatible: $X(g(Z,l))=g(\nabla_XZ,l)+g(Z,\nabla_Xl)$. This identity applies along the surface by restricting local extensions, with the pullback derivatives of [F1]. [[physics:def-gr-metric-selected-connection]]

[F11] Andersson–Mars–Simon, §2 and §3 through Lemma 3.2, use $\mathbf K(X,Z)=-(\nabla_XZ)^\perp$ and $H=\operatorname{tr}_q\mathbf K$, where $q=g|_{TS}$. For the supplied variation and null normals, their MOTS formula is the operator in the Statement with $Y_{\mathrm{AMS}}=V\mathbf K^\mu_{AB}\mathbf K^{\nu AB}l_\mu l_\nu+G(l,u)$, raising the surface indices with $q^{-1}$, and their expansion is $g(H,l)$. The variation depends only on the initial velocity and base null normal at a MOTS. This is the imported premise recorded in the source reference and External input section. [Andersson–Mars–Simon, printed pp. 5–8](https://arxiv.org/pdf/0704.2889)

[F12] For a smooth Riemannian metric, scalar curvature in an orthonormal basis $(e_1,\ldots,e_n)$ is $2\sum_{i<j}K(\operatorname{span}(e_i,e_j))$, under countable choice. On the positive two-dimensional surface metric $q$, the only plane is $T_pS$, whose sectional curvature is $q(R^q(e_1,e_2)e_2,e_1)=K_S$ in the convention of [F2]. The countable-choice hypothesis is inherited from [F4]. [[math:prop-scalar-curvature-is-twice-the-sum-of-sectional-curvatures-of-coordinate-planes]]

## External input

The general first-variation formula, including the curvature coefficient Y, is imported from Andersson–Mars–Simon, §3 Lemma 3.1 and Lemma 3.2, equations (2)–(7), printed pp. 7–8. The general immersed-surface family, its varying null normal and the MOTS independence assertion are imported from the preceding variation-family paragraph in §3, printed p. 7, and Lemma 3.1. The supplied family and its common parameter interval are explicit hypotheses in the Statement. No local derivation of the Appendix A covariant variation calculation is claimed.

The five local lemmas separate the algebraic null normalization, second-form and normal-connection signs, coefficient conversion, electrovac contraction, and null-hypersurface condition required by the application. For the outward hypersurface specialization only, the normal-graph supplier provides the actual family and its smooth null gauge, on its stated admissible domain. It is an instance of the general immersed-surface variation defined above; no such family for an arbitrary normal $v$ is obtained from that supplier. The article-specific horizon hypotheses must be supplied by the consumer; this input makes no claim that an arbitrary MOTS has zero null second form or zero null Ricci contraction.

## Proof

**Given:** The general surface, supplied variation and normalized null normals of the Statement, with the inherited choice assumptions in [F1]–[F4]. The hypersurface and electrovac data are imposed only for the corresponding specializations.

**Goal:** Convert the imported first-variation formula to the stated null-second-form convention and apply the existing specialization suppliers.

1.1 Work on an arbitrary surface patch with smooth tangent fields $X,Z$ and the given normal $l$. The positive metric $q=g|_{TS}$ makes the tangent plane nondegenerate, so orthogonal projection onto its normal complement is defined. Set $\mathbf K(X,Z)=-(\nabla_XZ)^\perp$ as in [F11]. Because $l$ is normal, projection does not change its pairing with $\nabla_XZ$. Also $g(Z,l)=0$ identically on the patch. Differentiating this identity along $X$ using [F10] gives $g(\mathbf K(X,Z),l)=-g(\nabla_XZ,l)=g(Z,\nabla_Xl)=\chi_l(X,Z)$. These are derivatives along the surface, so the identity is independent of the chosen local extensions. No hypersurface containing $S$ is assumed in this calculation. [given, F1, F10, F11, algebra]

2.1 Taking the $q$-trace of step 1.1 gives $g(H,l)=\theta_l$, so the source MOTS condition is precisely the one in the Statement. In a local tangent frame, contraction of step 1.1 with the two inverse surface metrics gives $\mathbf K^\mu_{AB}\mathbf K^{\nu AB}l_\mu l_\nu=q^{AC}q^{BD}\chi_{l,AB}\chi_{l,CD}=|\chi_l|_q^2$. Thus $Y_{\mathrm{AMS}}=V|\chi_l|_q^2+G(l,u)=Y$. The explicitly supplied family, its common interval, its smooth null normals and $g(l,v)=1$ satisfy [F11], which applies also to nonclosed surface patches. Substituting this coefficient in that imported formula proves the general displayed operator and its stated independence of the family and varying null gauge. This step imports the covariant variation calculation; it does not reconstruct it. [given, F1, F11, step 1.1, algebra]

3.1 Now impose the outward hypersurface gauge of [F2]. The normalization in [F5] gives $V=1/2$ and $u=n$ for $l=L$, $k=2\underline L$ and $v=\nu$. In this gauge [F6] gives $s=\zeta$, and [F7] gives $Y=|\chi_L|^2/2+G(L,n)$. The sign-agreement supplier [F6] is used only at this hypersurface specialization; the general conversion was proved in step 1.1. The family and null gauge supplied by [F2], on their admissible domain, are an instance of the supplied variation used in step 2.1. [F2, F5, F6, F7, step 2.1, algebra]

4.1 Finally impose the geometric electrovac equations of [F3] and the additional conditions $\chi_L=0$ and $\operatorname{Ric}(L,L)=0$. By [F8], $\operatorname{Scal}_g=0$, hence $G=\operatorname{Ric}$, and $G(L,\underline L)=e^2+b^2$. Since $g(L,L)=0$, the assumed null Ricci condition also gives $G(L,L)=0$. The coefficient conversion [F7] therefore reduces $Y$ to $e^2+b^2$. The smooth positive surface metric $q$ in [F2] satisfies [F12], with countable choice inherited from [F4]. In dimension two its sum has the single tangent plane, with sectional curvature $K_S=q(R^q(e_1,e_2)e_2,e_1)$ in the convention of [F2]. Thus $R_S=2K_S$, and substituting $R_S/2=K_S$ in step 2.1 gives the asserted specialized operator. If the open null-congruence hypotheses of [F9] hold, that supplier provides the required null Ricci condition. Otherwise it remains an explicit additional hypothesis, and it is never inferred from MOTS status alone. [given, F2, F3, F4, F7, F8, F9, F12, step 2.1, step 3.1, algebra] ∎

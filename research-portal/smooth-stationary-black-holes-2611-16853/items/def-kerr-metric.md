---
id: def-kerr-metric
title: Kerr metric, parameters, exterior and extremality
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-cea8e61dc3c6-kerr-exterior-tensor
  - lem-author-cea8e61dc3c6-kerr-future-horizon
  - lem-author-cea8e61dc3c6-kerr-komar-angular-momentum
  - lem-author-cea8e61dc3c6-kerr-rest-frame
  - def-author-cea8e61dc3c6-kerr-ingoing-extension
  - lem-author-cea8e61dc3c6-kerr-outgoing-completion
  - def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions
  - lem-author-cea8e61dc3c6-kerr-spatial-end
  - lem-author-cea8e61dc3c6-kerr-adm-energy
dependency_roles:
  lem-author-cea8e61dc3c6-kerr-exterior-tensor: mathematical-premise
  lem-author-cea8e61dc3c6-kerr-future-horizon: mathematical-premise
  lem-author-cea8e61dc3c6-kerr-komar-angular-momentum: mathematical-premise
  lem-author-cea8e61dc3c6-kerr-rest-frame: mathematical-premise
  def-author-cea8e61dc3c6-kerr-ingoing-extension: mathematical-premise
  lem-author-cea8e61dc3c6-kerr-outgoing-completion: mathematical-premise
  def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions: mathematical-premise
  lem-author-cea8e61dc3c6-kerr-spatial-end: mathematical-premise
  lem-author-cea8e61dc3c6-kerr-adm-energy: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: H. S. Reall, Black Holes, Part III lecture notes, 15 March 2024
      url: https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf
      locator: §9.4, paragraph following equation (9.20), printed p.118 (PDF p.119)
      statement: For an axisymmetric spacetime the ADM angular momentum agrees with
        the Komar angular momentum; the text explicitly states this when
        identifying the angular-momentum variation in the first law.
      hypotheses: A smooth axisymmetric asymptotically flat spacetime end, using the
        asymptotic axial Killing generator normalized to have 2π-periodic orbits
        and compatible angular-momentum and orientation conventions.
      reading_limits: Inspected the browser-extracted PDF text of §9.4 at equation
        (9.20) and the following paragraph on printed p.118, including its
        explicit ADM–Komar angular-momentum identification. The import is that
        identification for an axisymmetric asymptotically flat end with
        compatible conventions; neither the first-law perturbation theorem nor a
        bifurcation-surface assumption is imported. No downloaded-PDF
        inspection, full-notes reading or reconstruction of a proof of the
        identification is claimed. The Kerr constructions and charge
        calculations remain local supplier arguments.
    - title: Éric Gourgoulhon, 3+1 Formalism and Bases of Numerical Relativity (6
        March 2007)
      url: https://luth.obspm.fr/IHP06/lectures/gourgoulhon/lectures_eg.pdf
      locator: §2.3.4 (2.43), printed p.24 (PDF p.24); §7.5.1 (7.60)–(7.63), printed
        p.113 (PDF p.113); §7.6.3 (7.100)–(7.104), printed pp.121–122 (PDF
        pp.121–122)
      statement: With $K^{\rm G}(U,V)=-g(\nabla_U n,V)$, (7.63) defines the
        Hamiltonian angular component as $(8\pi)^{-1}\lim\int_{S_r}(K^{\rm
        G}_{ij}-(\operatorname{tr}_hK^{\rm G})h_{ij})\eta^i\nu_h^j\,dS_h$.
        Equation (7.104) expresses the finite-sphere Komar component as
        $(8\pi)^{-1}\int_{S_r}K^{\rm G}_{ij}\eta^i\nu_h^j\,dS_h$.
      hypotheses: Fixed asymptotically Euclidean chart and convergent limit for
        (7.63); slice-tangent axial Killing generator, future unit slice normal
        and outward unit sphere normal for (7.104). Use the chosen 2π-periodic
        axial direction. General coordinate invariance under supertranslations
        is not imported.
      reading_limits: Read browser-extracted PDF text at these formulas and adjacent
        sign, orientation and coordinate-ambiguity discussions. Only the charge
        definition and geometric flux identity are imported; no York gauge
        theorem, full-notes reading or proof reconstruction is claimed.
dependency_level: 5
---

## Definition

Use geometric units $G=c=1$. Let $M>0$ and $a\in\mathbb R$ satisfy $|a|\leq M$, and put $J=Ma$, $\rho^2=r^2+a^2\cos^2\theta$ and $\Delta=r^2-2Mr+a^2$. The Kerr exterior is the smooth Lorentzian tensor on $\mathbb R_t\times(r_+,\infty)\times S^2$ whose Boyer–Lindquist expression away from the rotation axis is
$$g_{\rm Kerr}=-\Delta\rho^{-2}(dt-a\sin^2\theta\,d\phi)^2+\sin^2\theta\,\rho^{-2}((r^2+a^2)d\phi-a\,dt)^2+\rho^2\Delta^{-1}dr^2+\rho^2d\theta^2,$$
where $r_+=M+\sqrt{M^2-a^2}$, the azimuth has period $2\pi$, and the tensor extends smoothly over the axis by the round-sphere construction. Subextremal means $|a|<M$ and extremal means $|a|=M$. The $a=0$ member is Schwarzschild.

Here $M$ is the ADM rest mass of the specified asymptotically flat constant $t$ end and $J$ its angular momentum, using the axial orientation $\partial_\phi$. Its asymptotic stationary field is $T=\partial_t$, normalized by $g(T,T)\to-1$. In the specified future ingoing Kerr extension and relative to the future null infinity attached to this exterior, $r=r_+$ is the future event horizon, the boundary of the black hole region. The Boyer–Lindquist exterior itself contains no horizon points; the horizon statement uses that extension. No assertion of a bifurcation sphere is made for extremal Kerr.

## Definition references

[[lem-author-cea8e61dc3c6-kerr-exterior-tensor]]

[[lem-author-cea8e61dc3c6-kerr-future-horizon]]

[[lem-author-cea8e61dc3c6-kerr-komar-angular-momentum]]

[[lem-author-cea8e61dc3c6-kerr-rest-frame]]

[[def-author-cea8e61dc3c6-kerr-ingoing-extension]]

[[lem-author-cea8e61dc3c6-kerr-outgoing-completion]]

[[def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions]]

[[lem-author-cea8e61dc3c6-kerr-spatial-end]]

[[lem-author-cea8e61dc3c6-kerr-adm-energy]]

## Facts & Assumptions

[F1] The exact exterior, causal extension and end-charge suppliers establish the stated metric, horizon and charge conclusions: [[lem-author-cea8e61dc3c6-kerr-exterior-tensor]] [[lem-author-cea8e61dc3c6-kerr-future-horizon]] [[lem-author-cea8e61dc3c6-kerr-komar-angular-momentum]] [[lem-author-cea8e61dc3c6-kerr-rest-frame]]

[F2] For an axisymmetric asymptotically flat spacetime, ADM angular momentum agrees with the Komar angular momentum with compatible axial normalization and orientation. This conventional identification is an external input from Reall §9.4, printed p.118, following (9.20).

[F3] The specified ingoing extension, exterior embedding and future time orientation are supplied by [[def-author-cea8e61dc3c6-kerr-ingoing-extension]]. The selected future null infinity and escaping exterior curves are constructed by [[lem-author-cea8e61dc3c6-kerr-outgoing-completion]].

[F4] The ADM energy, momentum, nonnegative rest-mass root and future/outward Komar orientation conventions are those of [[def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions]]. The constant $t$ slices are spacelike, and their end has the differentiated asymptotically flat expansion in [[lem-author-cea8e61dc3c6-kerr-spatial-end]].

[F5] The ADM energy of that specified Kerr end exists and equals $E_{\rm ADM}=M$, with the same metric-flux convention, by [[lem-author-cea8e61dc3c6-kerr-adm-energy]].

[F6] On the fixed end of [F4], use $\eta=\partial_\phi$, $K(U,V)=g(\nabla_U n_\Sigma,V)$, the future unit normal $n_\Sigma$, the outward $h$-unit normal $\nu_h$ and the sphere measure $dS_h$. The ADM axial component convention is
$$J_{\rm ADM}[\eta]=-\frac1{8\pi}\lim_{r\to\infty}\int_{S_r}(K_{ij}-(\operatorname{tr}_hK)h_{ij})\eta^i\nu_h^j\,dS_h.$$
Assign it only when the limit exists. This is Gourgoulhon (7.63), translated using $K^{\rm G}=-K$ from (2.43). For a slice-tangent axial Killing field, (7.104) gives the finite-sphere Komar flux $J_{\rm K}(S_r)=-(8\pi)^{-1}\int_{S_r}K_{ij}\eta^i\nu_h^j\,dS_h$. Only the specified axial component is used; no angular charge for arbitrary asymptotic charts is asserted.

## Justification

**Given:** The exterior tensor, horizon conclusion and end-charge conclusions of [F1], the external angular-momentum identification in [F2], the extension and selected infinity in [F3], the charge conventions and spacelike end in [F4], and the energy calculation in [F5], and the explicit ADM axial-flux definition and finite-sphere identity in [F6].

**Goal:** Justify the definition's metric, horizon and charge interpretations throughout its parameter range.

1.1 The exterior supplier establishes smoothness, Lorentzian signature, the coordinate Killing fields, the axial period and the Schwarzschild specialization. The ingoing extension in [F3] supplies the exterior embedding and smooth future time orientation, and its outgoing-completion supplier constructs the selected conformal infinity. The causal-horizon supplier in [F1], with its stated Countable Choice and Dependent Choice assumptions, proves that precisely $r>r_+$ can send a future signal to that infinity. Its complement has boundary $r=r_+$, which is the claimed future event horizon. These constructions and the causal conclusion include $|a|=M$ and do not rely on two distinct roots. [given, F1, F3]

2.1 The charge conventions and spacelike asymptotically flat end are those of [F4]. The energy calculation [F5] gives $E_{\rm ADM}=M$, while the rest-frame supplier in [F1] gives zero linear momentum and rest mass $M$. The independently calculated axial Komar integral in [F1] exists and is $Ma$, with the future/outward orientation of [F4]. The exterior tensor gives $g(T,T)=-1+2Mr/\rho^2\to-1$. [given, F1, F4, F5, step 1.1]

3.1 In the Cartesian chart $x=r(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta)$ of [F4], the axial field of [F1] is $\eta=-x^2\partial_{x^1}+x^1\partial_{x^2}$, with the specified positive $2\pi$ period. It is a smooth Killing field tangent to the constant $t$ slices and their spheres, including at its axis zeros. Since $\eta(r)=0$, the normal formula in [F4] gives $h(\nu_h,\eta)=dr(\eta)/|\operatorname{grad}_h r|_h=0$. Thus the trace term in [F6] vanishes identically on every sphere. The finite-sphere identity in [F6], with $K^{\rm G}=-K$ and the same future/outward orientations, identifies each ADM defining surface integral with $J_{\rm K}(S_r)$. Step 2.1 supplies its convergent limit $Ma$, proving existence of the ADM axial charge and $J_{\rm ADM}[\eta]=Ma$ in precisely the convention used by [F2]. This verifies the imported identification on this end, including negative $a$, $a=0$ and $|a|=M$, without requiring an unproved convergence theorem for arbitrary ends. These justifications fix the intended geometric meaning of the parameters without using the original article as proof. [given, F1, F2, F4, F6, step 2.1] ∎

## External input

Reall §9.4 following (9.20) supplies the ADM–Komar identification. Gourgoulhon (2.43), (7.63) and (7.104) supply its explicit sign convention, ADM definition and finite-sphere geometric identity. The Kerr end and Komar limit are local supplier results; their application in step 3.1 is a local argument, not a literature-derived proof of the whole item.

## Source notes

Original claim attribution: The uniqueness of smooth stationary black holes, arXiv:2611.16853v1, §1.1, PDF pp.1–2. The original displayed metric, $M>0$, $J=Ma$, subextremal/extremal terminology, horizon location and Schwarzschild specialization are retained. This attribution supplies no prerequisite proof. Reall §§7.2–7.4, printed pp.93–97, and Visser §5, printed pp.14–15, were consulted for coordinate and asymptotic conventions; Visser §9 explicitly restricts its horizon discussion to subextremal Kerr, and is not used for the extremal assertion. The proof above uses the specified ingoing patch, not an assumed maximal-extension diagram.

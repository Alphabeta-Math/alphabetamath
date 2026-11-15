---
title: Ernst and self-dual curvature data in the AIK convention
status: draft
research_item: def-author-ad064c44a1cc-ernst-curvature-package
dependency_level: 3
sources:
  references:
    - title: "S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth
        stationary black holes in vacuum: small perturbations of the Kerr
        spaces"
      url: https://arxiv.org/html/0904.0982v1
      locator: Section 1.1 setup and GR/SBS; section 2.1 neighborhood construction
        preceding (2.3); section 2.3, (2.13)–(2.15) and the potential-existence
        paragraph immediately before (2.16). PDF v1 pp. 4–7 and 8–9.
      statement: Under GR/SBS there is a smooth complex potential $\sigma$ on the
        section 2.1 neighborhood $\widetilde M$ of $\Sigma^0\cap\overline E$,
        satisfying $d\sigma=2\iota_T\mathcal F$, $\Re\sigma=-g(T,T)$, and
        $\sigma\to1$ at spatial infinity on $\Sigma^0$. In the section 2.1
        construction, $\Phi_1:(-\varepsilon_0,\varepsilon_0)\times
        E_{1-\varepsilon_0}\to\widetilde M$ is a diffeomorphism and agrees with
        $\Phi_0$ on $(-\varepsilon_0,\varepsilon_0)\times E_{2R_1}$, where
        $T=\partial_t$.
      hypotheses: The smooth oriented time-oriented Ricci-flat four-dimensional
        stationary data, source partial Cauchy surface, stationary asymptotic
        end and GR/SBS conditions of
        def-author-ad064c44a1cc-perturbative-gr-sbs. Use the neighborhood
        constructed in section 2.1; PK and maximality are not required for this
        input.
      reading_limits: Consulted the arXiv v1 HTML section 1.1 setup and GR/SBS,
        section 2.1 neighborhood construction, and section 2.3 (2.13)–(2.17)
        with the intervening existence paragraph; cross-checked that paragraph
        in the PDF text on p. 9. Import restricted to the neighborhood potential
        and slice normalization. The source also gives an exterior extension,
        which is not needed here. Its topology and potential-existence argument
        are accepted as an external input, not locally reconstructed; no
        rigidity proof was reviewed. For the present orientation repair, re-read
        the HTML section 2.1 construction between (2.2) and (2.3), including the
        product domain and agreement with the stationary end, and the section
        2.3 potential paragraph before (2.16). The preceding PDF-reading
        statements are retained historical source metadata; no new PDF
        inspection or review of the source proof is claimed in this repair. The
        orientation-compatible coordinate choice is proved locally.
    - title: "S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth
        stationary black holes in vacuum: small perturbations of the Kerr
        spaces"
      url: https://arxiv.org/html/0904.0982v1
      locator: Section 2.3, (2.13), (2.16)–(2.17), (2.20), PDF pp. 8–9; section 5.1,
        (5.9)–(5.10) and the immediately following unnumbered curvature formula,
        PDF p. 27.
      statement: The covariant curvature convention is $R^{\rm
        AIK}(X,Y,Z,W)=g(X,(\nabla_Z\nabla_W-\nabla_W\nabla_Z-\nabla_{[Z,W]})Y)$.
        Equations (2.16)–(2.17) set $\mathcal R_{ab cd}=R^{\rm AIK}_{ab
        cd}+\frac{i}{2}\epsilon_{cd}{}^{ef}R^{\rm AIK}_{ab ef}$ and $\mathcal
        I_{ab cd}=\frac14(g_{ac}g_{bd}-g_{ad}g_{bc}+i\epsilon_{abcd})$; in
        vacuum (2.20) states $\nabla_\mu\mathcal F_{ab}=T^\nu\mathcal R_{\nu\mu
        ab}$.
      hypotheses: For the curvature convention and algebraic definitions, a smooth
        oriented Lorentzian four-metric with its Levi–Civita connection; the
        covariant slots follow the arbitrary-frame convention displayed in
        section 5.1. For (2.20), require Ricci-flatness and a smooth Killing
        field, with the Hodge convention (2.13). These conditions hold in the
        declared GR/SBS package.
      reading_limits: Read the indicated HTML equations and the defining first line of
        the unnumbered curvature formula in section 5.1 after (5.10);
        cross-checked the latter in the PDF text on p. 27. The PDF screenshot
        service failed, so no image inspection is claimed. This imports the
        convention and (2.20), without reconstructing the Ricci identity or
        reviewing the continuation argument around the curvature formula.
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-killing-ernst-notation](item-def-killing-ernst-notation)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [def-author-ad064c44a1cc-perturbative-gr-sbs](item-def-author-ad064c44a1cc-perturbative-gr-sbs)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth stationary black holes in vacuum: small perturbations of the Kerr spaces · Section 1.1 setup and GR/SBS; section 2.1 neighborhood construction preceding (2.3); section 2.3, (2.13)–(2.15) and the potential-existence paragraph immediately before (2.16). PDF v1 pp. 4–7 and 8–9. `](https://arxiv.org/html/0904.0982v1)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth stationary black holes in vacuum: small perturbations of the Kerr spaces · Section 2.3, (2.13), (2.16)–(2.17), (2.20), PDF pp. 8–9; section 5.1, (5.9)–(5.10) and the immediately following unnumbered curvature formula, PDF p. 27. `](https://arxiv.org/html/0904.0982v1)


## Definition

For the AIK perturbative GR/SBS package, let $U=\widetilde M$ be the open neighborhood of $\Sigma^0\cap\overline E$ constructed in AIK §2.1. Use the normalized smooth Ernst potential $\sigma=f+i\psi$ on $U$, with $f=-g(T,T)$, $d\sigma=2\iota_T\mathcal F$ and $\sigma\to1$ at infinity. Here $F_{ab}=\nabla_aT_b=\tfrac12(dT^\flat)_{ab}$, $\mathcal F=F+i\star_gF$, $\mathcal F^2=\mathcal F_{ab}\mathcal F^{ab}$ uses complex bilinear contraction, and the spacetime orientation fixes $\epsilon$ and $\star_g$. Existence on $U$ is imported explicitly in External input; the definition of a potential alone asserts no existence.

For normalization, designate the product end $U_{\mathrm{end}}=\Phi_0(I\times E_{2R_1})\subset U$, where $I=(-\varepsilon_0,\varepsilon_0)$ and $R_1,\varepsilon_0$ are from the AIK §2.1 construction. In its source coordinates $(t,x)$, put $y=x$ when $dt\wedge dx^1\wedge dx^2\wedge dx^3$ is positive for the given spacetime orientation; otherwise put $y=(-x^1,x^2,x^3)$. Use $(t,y)$ as the designated normalization chart, so $dt\wedge dy^1\wedge dy^2\wedge dy^3$ is positive, $|y|=|x|$ and $T=\partial_t$. The GR/SBS source chart and its component hypotheses remain the original $(t,x)$ chart.

Write $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$ for the stationary-data curvature operator. Define the source covariant array by
$$R^{\rm AIK}(X,Y,Z,W)=g(X,R(Z,W)Y),\qquad R^{\rm AIK}_{ab cd}=g_{ae}R^e{}_{bcd}.$$
This fixes all four slots and the sign explicitly; its identification with the AIK convention uses the curvature formula in §5.1 after (5.10), rather than (2.16) or a contraction with $T$ alone. Define
$$\mathcal R_{ab cd}=R^{\rm AIK}_{ab cd}+\frac{i}{2}\epsilon_{cd}{}^{ef}R^{\rm AIK}_{ab ef},\qquad \mathcal I_{ab cd}=\frac14(g_{ac}g_{bd}-g_{ad}g_{bc}+i\epsilon_{abcd}).$$
Thus the Hodge operation on curvature is in its last alternating pair, all raised indices use this $g$, and $\mathcal I$ is the displayed covariant four-tensor. The source identity (2.20), $\nabla_\mu\mathcal F_{ab}=T^\nu\mathcal R_{\nu\mu ab}$, is an imported identity in this convention, not a definition of the full curvature array or a locally proved differential identity. No conversion to a different curvature convention is asserted.

## Facts & Assumptions

[F1] [def-author-ad064c44a1cc-perturbative-gr-sbs](item-def-author-ad064c44a1cc-perturbative-gr-sbs) specifies the GR/SBS source hypotheses and background geometry. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) provides the connection, curvature operator, metric duality and tensor types.

[F2] [def-killing-ernst-notation](item-def-killing-ernst-notation) gives the Killing two-form, Ernst equation and normalized-potential terminology, and [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data) gives the complex-linear Hodge star and complex bilinear contractions. Neither definition supplies potential existence.

[F3] Import the neighborhood potential, its slice normalization and the stationary product end of the neighborhood construction from [AIK §2.1 and §2.3](https://arxiv.org/html/0904.0982v1), under exactly the GR/SBS hypotheses in [F1], as specified by the first statement-bearing source record and External input.

[F4] Import the source curvature convention from the unnumbered formula after AIK (5.10), and (2.20) in that convention, from [AIK §5.1 and §2.3](https://arxiv.org/html/0904.0982v1), with the precise hypotheses in the second statement-bearing source record.

## Justification

**Given:** The GR/SBS data, the declared mathematical conventions and the two explicit source inputs.

**Goal:** Establish the displayed constructions and their compatibility with the source convention.

1.1 Since $F$ is alternating and the connection is torsion-free, $(dT^\flat)_{ab}=\nabla_aT_b-\nabla_bT_a=2F_{ab}$. The GR/SBS data meet the hypotheses of the imported neighborhood-potential input [F3], so $\sigma$ is a supplied smooth function on $U$, with the stated real part, differential and slice normalization. The same source construction supplies $U_{\mathrm{end}}=\Phi_0(I\times E_{2R_1})\subset U$ with $T=\partial_t$. This end is connected, so the nowhere-zero form $dt\wedge dx^1\wedge dx^2\wedge dx^3$ has constant orientation sign there. In the negative case the fixed reflection in the Definition multiplies that form by $-1$; in the positive case the chart is unchanged. Both choices are smooth coordinate diffeomorphisms onto $I\times E_{2R_1}$, preserve the radius and $t$, and give the positive coordinate volume form required by [F2]. This changes only the designated coordinates, not the spacetime orientation, Hodge star or potential. By alternation, $T^a\nabla_a\sigma=2T^aT^b\mathcal F_{ba}=0$. Since $T=\partial_t$ on this product end, $\sigma(t,y)=\sigma(0,y)$ for every $t\in I$. For any $\delta>0$, the imported slice limit gives $R>2R_1$ such that $|\sigma(0,x)-1|<\delta$ whenever $|x|>R$. The equality of radii and the independence of $t$ therefore give $|\sigma(t,y)-1|<\delta$ for every $t\in I$ and $|y|>R$, exactly the uniform end normalization of [F2]. This uses the imported existence result, without claiming a local topological or potential-existence proof. [F1, F2, F3, algebra]

1.2 For any smooth local frame $(v_a)$, substitution of the curvature operator of [F1] into the covariant array gives $g(v_a,(\nabla_{v_c}\nabla_{v_d}-\nabla_{v_d}\nabla_{v_c}-\nabla_{[v_c,v_d]})v_b)$, exactly the source convention in [F4]. Thus this identification fixes every slot without inferring the full array from a contraction with $T$. The array is a smooth covariant tensor and is alternating in its last two slots because $R(Z,W)=-R(W,Z)$ directly from its definition. Applying the smooth Hodge operation to those two slots is therefore intrinsic and well defined. [F1, F2, F4, algebra]

2.1 Metric tensor products, the oriented metric volume form, contractions and constant complex linear combinations preserve tensor type and smoothness. Hence the displayed $\mathcal R$ and $\mathcal I$ are smooth covariant four-tensors independent of the frame, and the displayed scalar contraction has precisely the complex bilinear meaning of [F2]. Together with the supplied smooth potential this proves well-definedness of the package. Identity (2.20) retains its imported status [F4]; it is not used to infer its own curvature convention or to prove potential existence. [F1, F2, F4, step 1.1, step 1.2] ∎

## External input

The first statement-bearing AIK source record supplies the neighborhood potential, its normalization and the stationary product end in the neighborhood construction under GR/SBS. Its source argument is accepted as an external input; no local potential-existence proof is claimed.

The second statement-bearing AIK source record supplies the explicit curvature convention and identity (2.20). The identification with the stationary-data operator and the well-definedness of the displayed constructions are justified locally above. This definition imports no global rigidity theorem.

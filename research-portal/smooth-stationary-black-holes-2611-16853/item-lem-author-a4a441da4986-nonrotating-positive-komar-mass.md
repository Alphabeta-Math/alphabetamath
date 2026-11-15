---
title: The nonrotating bifurcation gives positive normalized mass before staticity
status: draft
research_item: lem-author-a4a441da4986-nonrotating-positive-komar-mass
dependency_level: 5
sources:
  references:
    - title: D. Sudarsky and R. M. Wald, Mass Formulas for Stationary
        Einstein–Yang–Mills Black Holes and a Simple Proof of Two Staticity
        Theorems
      url: https://arxiv.org/pdf/gr-qc/9305023v1
      locator: PDF p.5, equation (23) and following paragraph; p.2, horizon generator
        normalization (4)
      statement: The Komar mass identity is M−kappa A/(4pi)−2Omega J_H = 2 integral
        (T_munu−T g_munu/2)t^mu n^nu over a section with bifurcation boundary.
        The text explicitly says this identity does not require a maximal
        hypersurface. In vacuum with the stationary field itself the horizon
        generator, it gives M=kappa A/(4pi).
      hypotheses: Stationary asymptotically flat geometry with a regular bifurcate
        Killing horizon, normalized stationary field, an oriented spacelike
        section from its compact bifurcation surface to infinity, Einstein
        equation; specialize to zero matter and Omega=0. The identity is the
        local Stokes/Komar flux calculation on that section and assumes no
        complete Killing flow in a larger ambient spacetime.
      reading_limits: "Consulted the cached full PDF, PDF pp.2 and 5: normalization
        (4), equation (23), its Komar-to-volume derivation description, and its
        explicit nonmaximal qualification. Only that identity and its stated
        specialization are imported; no maximal-slice existence, staticity or
        positive-mass theorem is used or reviewed."
    - title: H. S. Reall, Black Holes, Part III lecture notes, 15 March 2024
      url: https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf
      locator: §8.1, printed pp.105–106 (PDF pp.106–107), (8.2) and the orientation
        example (8.11)–(8.13); §8.2, printed pp.107–108 (PDF pp.108–109), (8.14)
        sphere convention and (8.24) Komar definition; §9.3, printed p.117 (PDF
        p.118), zeroth-law theorem and (9.16)–(9.19); §8.4, printed p.113 (PDF
        p.114), stationary ADM/Komar equality and (8.43)–(8.45)
      statement: For an oriented Lorentzian four-manifold the Hodge dual of a two-form
        F is (star F)_ab=(1/2) epsilon_abcd F^cd, with indices raised by g. The
        orientation example uses positive dt wedge dr wedge dtheta wedge dphi,
        its future-normal section orientation and the outward boundary sphere
        orientation. For a stationary asymptotically flat end, (8.24) defines
        M_Komar=−(8pi)^(-1) lim integral over S_r of star d(T-flat), with T-flat
        the metric dual of the normalized stationary field and S_r the
        end-coordinate spheres. On a connected future Killing event horizon the
        surface gravity is constant under the dominant energy condition; in
        vacuum the local Killing-horizon calculation (9.16)–(9.19) gives this
        conclusion. In a stationary asymptotically flat spacetime E_ADM=M_Komar
        on constant-time surfaces asymptotically orthogonal to the timelike
        Killing field. Equations (8.43)–(8.45) define the ADM energy, momentum
        P_i=(8pi)^(-1)lim integral(K_ij n^j−K n_i)dA, and rest mass
        sqrt(E_ADM^2−P_i P_i).
      hypotheses: "For the flux definition, a stationary asymptotically flat end with
        normalized stationary field, and a consistently oriented neighborhood of
        the spacelike section; use signature (−,+,+,+), the metric Hodge dual
        and outward end spheres. The displayed coordinate orientation is used in
        the specified end. Smooth connected Killing horizon with specified
        normalized generator; vacuum is the zero-stress case satisfying the
        dominant energy condition. For the mass equality and definitions: a
        differentiably asymptotically flat stationary end and a constant-time
        section asymptotically orthogonal to the normalized timelike Killing
        field. The opposite convention for extrinsic curvature reverses P_i and
        does not affect its vanishing or the rest mass. No assertion that a
        general stationary null surface is a Killing horizon is imported."
      reading_limits: Consulted the cached full PDF at PDF pp.114 and 118, including
        the displayed equations and adjacent hypotheses; also read PDF
        pp.111–113 for the surrounding ADM end conventions. The local
        Killing-horizon premise and the positive sign for the fixed T are proved
        separately here. The cited zeroth-law derivation is used after that
        premise is supplied; no Hawking rigidity, global completion or
        positive-energy theorem is imported. The ADM/Komar equality is accepted
        as the stated external result, not locally reconstructed. For this
        repair, independently read the online PDF text of §§8.1–8.2, printed
        pp.105–108, specifically (8.2), the orientation example (8.11)–(8.13),
        the coordinate spheres after (8.14), and the definition (8.24). This
        additional reading supplies only the Hodge, orientation and flux
        conventions; their local end evaluation is given below. PDF screenshots
        were unavailable; no screenshot inspection or source-proof
        reconstruction is claimed.
---

## Prerequisites

- [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)
- [lem-author-a4a441da4986-stationary-end-future-orientation](item-lem-author-a4a441da4986-stationary-end-future-orientation)
- [lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar)
- [lem-author-a4a441da4986-zero-stationary-boundary-data](item-lem-author-a4a441da4986-zero-stationary-boundary-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [math:thm-embedded-submanifolds-admit-local-defining-submersions](https://alphabetamath.cc/item/thm-embedded-submanifolds-admit-local-defining-submersions)
- [` D. Sudarsky and R. M. Wald, Mass Formulas for Stationary Einstein–Yang–Mills Black Holes and a Simple Proof of Two Staticity Theorems · PDF p.5, equation (23) and following paragraph; p.2, horizon generator normalization (4) `](https://arxiv.org/pdf/gr-qc/9305023v1)
- [` H. S. Reall, Black Holes, Part III lecture notes, 15 March 2024 · §8.1, printed pp.105–106 (PDF pp.106–107), (8.2) and the orientation example (8.11)–(8.13); §8.2, printed pp.107–108 (PDF pp.108–109), (8.14) sphere convention and (8.24) Komar definition; §9.3, printed p.117 (PDF p.118), zeroth-law theorem and (9.16)–(9.19); §8.4, printed p.113 (PDF p.114), stationary ADM/Komar equality and (8.43)–(8.45) `](https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf)



## Statement

Under the regular vacuum assumptions and $T|_S=0$, the mass parameter $M_0$ in $g_{00}=-1+2M_0/r+O_6(r^{-2})$ is positive. More precisely, for the future horizon generated by the asymptotically normalized stationary field,
$$M_0=M_{\rm ADM}=M_{\rm Komar}=\frac{\kappa\operatorname{Area}_h(S)}{4\pi}>0.$$
This conclusion is obtained on the original complete-up-to-boundary section, before any maximal-slice or staticity theorem is used.

## Statement references

[lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)

[lem-author-a4a441da4986-stationary-end-future-orientation](item-lem-author-a4a441da4986-stationary-end-future-orientation)

[lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar)

[lem-author-a4a441da4986-zero-stationary-boundary-data](item-lem-author-a4a441da4986-zero-stationary-boundary-data)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[math:thm-embedded-submanifolds-admit-local-defining-submersions](https://alphabetamath.cc/item/thm-embedded-submanifolds-admit-local-defining-submersions)

## Facts & Assumptions

[F1] The complete-up-to-boundary section and its end, the future orientation of timelike $T$ in $E$, the working partial-Cauchy collar, and the local bifurcate Killing horizon with its nonzero normal boost and affine-generator law are supplied by [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section), [lem-author-a4a441da4986-stationary-end-future-orientation](item-lem-author-a4a441da4986-stationary-end-future-orientation), [lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar) and [lem-author-a4a441da4986-zero-stationary-boundary-data](item-lem-author-a4a441da4986-zero-stationary-boundary-data). The differentiated end notation and signed surface-gravity convention are [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) and [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data).

[F2] Sudarsky–Wald equation (23) supplies the nonmaximal Komar boundary identity. Reall §§8.1–8.2 supply the metric Hodge dual, future-normal/outward-sphere orientation and normalized Komar flux definition in (8.2), the orientation example (8.11)–(8.13), and (8.24). Reall §9.3 supplies the vacuum zeroth law on the established connected Killing sheet; §8.4 supplies stationary ADM/Komar equality and the ADM momentum and rest-mass definitions. The exact statements, hypotheses and reading limits are in the source records and External input.

[F3] The vacuum equation, normalized field $T=\partial_t$, end metric coefficients, $t=0$ section identification, smooth transverse chronological-boundary sheets and ZFC convention are [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime). The smooth future unit normal $n$, induced metric $h$, second fundamental form $k$ and splitting $T=Nn+X$ use [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data).

[F4] A smooth embedded hypersurface has a local defining function with nonvanishing differential. [math:thm-embedded-submanifolds-admit-local-defining-submersions](https://alphabetamath.cc/item/thm-embedded-submanifolds-admit-local-defining-submersions) The chronological sets are open; for a past set $P$ and $q\in\overline P$, $I^-(q)\subset P$. [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness) Its Countable Choice and Dependent Choice hypotheses hold under the ZFC convention of [F3].

## Proof

**Given:** The regular vacuum data and $T|_S=0$, with the section, orientation and horizon interfaces [F1], external identities [F2], geometric conventions [F3] and local boundary calculus [F4].

**Goal:** Establish the displayed positive normalized mass without a maximal-slice or staticity premise.

1.1 Work in the connected spacetime component containing the connected section $C\cup S$ and the selected end; $T$ is nontrivial there since it is timelike at infinity. At $q\in S$, let $n$ be the future unit normal to the original section and $e$ its unit normal to $S$ pointing into $C$. The boost interface in [F1] gives $A_qn=\lambda_qe$ and $A_qe=\lambda_qn$, with $\lambda_q\ne0$; this follows also by writing its skew map in the orthonormal basis $(n,e)$. Choose a smooth section curve $c(r)$ into $C$ with $c(0)=q$ and $c'(0)=e$. In a smooth ambient chart, $T(c(r))=r\lambda_qn+O(r^2)$ because $T(q)=0$ and the connection correction to its first derivative vanishes there. Consequently $g(T,T)(c(r))=-\lambda_q^2r^2+O(r^3)<0$ for small $r>0$. These points lie in $E$; the orientation supplier makes $T$ future timelike there. Taking $T(c(r))/r\to\lambda_qn$ forces $\lambda_q>0$. This fixes the sign of the already normalized $T$, without rescaling it or choosing a sign for a horizon parameter. [given, F1, F3]

2.1 Identify the future boundary sheet using $P=I^-(M^{\rm end})$, a past set, and $\mathcal H^+=\partial P$ near $S$. Take a defining function $u$ from [F4], with $du(n)>0$ at $q$. The differential annihilates $T_qS$ and is null, so $du(e)=\pm du(n)\ne0$. The past-set closure property gives points immediately to the timelike past of $q$ in $P$, while a timelike-future point of $q$ cannot belong to $P$, since that would put $q$ in the open past set. In a sufficiently small hypersurface chart, membership in $P$ is constant on each connected side of $u=0$, so its local side is $u<0$. Since $c(r)\in C\subset P$, differentiation at $r=0$ and $du(e)\ne0$ imply $du(e)<0$, hence $du(e)=-du(n)$. Thus the future normal generator of this sheet at $q$ is $\ell=n+e$, and $A_q\ell=\lambda_q\ell$. On the future branch $s>0$ of its affine generator, the supplier's exact law is $T=\lambda_qs\dot\gamma_q$. Affineness gives $\nabla_TT=\lambda_qT$, so its signed surface gravity is $\lambda_q>0$, with the same limit at $q$. The vacuum zeroth law of Reall §9.3 makes this one constant $\kappa>0$ on the connected local future Killing sheet and its bifurcation limit. The induced metric on the nonempty compact sphere $S$ has positive finite area $A$. [given, F1, F2, F3, F4, step 1.1]

3.1 Apply Sudarsky–Wald equation (23), the nonmaximal Komar identity, to the oriented section $C\cup S$ supplied in [F1]. It has compact core, only the bifurcation boundary $S$, and the one normalized asymptotic end. The field is Killing and the geometry is vacuum by [F3]; $T$ itself generates the local horizon, so the rotational term is absent ($\Omega=0$), and the matter integral is zero. The identity therefore gives $M_{\rm Komar}=\kappa A/(4\pi)>0$. Its derivation uses the section and its boundary fluxes, requiring neither an all-time ambient extension nor a maximal section. [given, F1, F2, F3, step 2.1]

4.1 In the specified end the same section is $t=0$, $T=\partial_t$, $g_{0i}=O_6(r^{-2})$ and $g_{ij}=\delta_{ij}+O_6(r^{-1})$, so it is asymptotically orthogonal to $T$. Reall §8.4 therefore gives $E_{\rm ADM}=M_{\rm Komar}$. Use the Hodge and flux conventions of [F2]: orient the end by $\epsilon=\sqrt{-\det g}\,dt\wedge dx^1\wedge dx^2\wedge dx^3$, the section by its future normal and the end spheres outward. This orientation extends along the section using its radial chart and smooth future normal. Here $T^\flat=g_{00}dt+g_{0i}dx^i$, and stationarity gives $(dT^\flat)_{0i}=-\partial_i g_{00}=2M_0x^i/r^3+O(r^{-3})$ and $(dT^\flat)_{ij}=O(r^{-3})$. In the limiting Minkowski metric the supplied Hodge convention gives $\star(dt\wedge dr)=-dA_0$, where $dA_0$ is the positively oriented Euclidean sphere area form. The metric and inverse-metric corrections are $O(r^{-1})$, and the differentiated shift terms are $O(r^{-3})$, so on $S_r=\{t=0,|x|=r\}$ one has $\left.\star dT^\flat\right|_{S_r}=(-2M_0/r^2+O(r^{-3}))dA_0$, uniformly in angle. Thus (8.24) gives $M_{\rm Komar}=-\frac1{8\pi}\lim_{r\to\infty}\int_{S_r}\star dT^\flat=M_0$, since $\int_{S_r}dA_0=4\pi r^2$ and the integrated error is $O(r^{-1})$. For completeness, $N=1+O(r^{-1})$ and the covariant end shift is $X_i=g_{0i}=O_6(r^{-2})$. The tangential Killing equation and the convention of [F3] give $2Nk_{ij}=D_iX_j+D_jX_i$, hence $k_{ij}=O(r^{-3})$. Reall's momentum formula (8.44) therefore has limit zero, independently of its sign convention for $k$. By (8.45), $M_{\rm ADM}=\sqrt{E_{\rm ADM}^2-|P_{\rm ADM}|^2}=E_{\rm ADM}$, since step 3.1 made this energy positive. Combining the identities proves the unchanged Statement. [given, F1, F2, F3, step 3.1] ∎

## External input

Sudarsky–Wald, PDF p.5, equation (23) and its following paragraph, gives $M-\kappa A/(4\pi)-2\Omega J_H=2\int_\Sigma(T_{\mu\nu}-Tg_{\mu\nu}/2)t^\mu n^\nu$ for a stationary asymptotically flat Einstein geometry with a regular bifurcate Killing horizon and an oriented section from its bifurcation surface to infinity. The paragraph explicitly permits a nonmaximal section. Here vacuum and the normalized stationary field as horizon generator remove the volume and rotation terms. [Mass formulas, equation (23)](https://arxiv.org/pdf/gr-qc/9305023v1)

Reall §9.3, printed p.117, gives constancy of surface gravity on a connected future Killing horizon under the dominant energy condition; equations (9.16)–(9.19) apply locally once the Killing-horizon premise is established, as it is here in vacuum. Reall §8.4, printed p.113, states $E_{\rm ADM}=M_{\rm Komar}$ for a stationary asymptotically flat end with asymptotically orthogonal constant-time surfaces and defines its momentum and rest mass in (8.44)–(8.45). [Black Holes, §§8.4 and 9.3](https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf)

Reall §8.1, (8.2), defines the two-form Hodge dual by $(\star F)_{ab}=\tfrac12\epsilon_{abcd}g^{ce}g^{df}F_{ef}$. Its printed p.106 example fixes positive $dt\wedge dr\wedge d\theta\wedge d\phi$, the future-normal orientation on $t=0$, and outward boundary spheres. Section 8.2, (8.24), defines $M_{\rm Komar}=-\frac1{8\pi}\lim_{r\to\infty}\int_{S_r}\star dT^\flat$ on a stationary asymptotically flat end, where $T^\flat=g(T,\cdot)$ and $S_r$ are the coordinate spheres of (8.14). These conventions use signature $(-,+,+,+)$ and the stationary field normalized to unit future time translation at infinity; no maximality is required. [Black Holes, §§8.1–8.2](https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf)

Only these explicitly cited premises are imported. The normal-boost sign, future-branch identification and end application are local arguments above; the source proofs and any global rigidity, maximal-slice or positive-energy theorem are not reconstructed or assumed. The source records state the actual consulted passages and reading limits.

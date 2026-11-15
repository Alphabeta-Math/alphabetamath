---
title: K-flow barriers with boundary tangency comparison and uniform height bound
status: draft
research_item: pthm-hawking-graph-barriers
dependency_level: 16
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp.17–18, Lemma3.4 barrier proof and (3.10)
      reading_limits: Consulted the frozen article text at PDF pp.17–18, Lemma 3.4
        through (3.10). This citation attributes the original barrier
        construction and height claim; it is not a proof premise. The boundary
        comparison and uniform sliding argument below are locally authored from
        the declared suppliers.
---

PDF p. 17: ` Proof of Lemma 3.4, barriers; (3.10) `; PDF p. 18: ` Proof of Lemma 3.4, barriers; (3.10) `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [pthm-common-reference-collar](item-pthm-common-reference-collar)
- [pthm-normal-boost-action](item-pthm-normal-boost-action)
- [pthm-hawking-graph-height](item-pthm-hawking-graph-height)
- [pthm-compact-height-bound](item-pthm-compact-height-bound)
- [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)
- [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [lem-author-66066dbaeb16-half-domain-contact-hessian](item-lem-author-66066dbaeb16-half-domain-contact-hessian)
- [lem-author-66066dbaeb16-spacelike-common-graph-curvature-jet](item-lem-author-66066dbaeb16-spacelike-common-graph-curvature-jet)
- [lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency](item-lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency)
- [lem-author-66066dbaeb16-timelike-flow-ordering](item-lem-author-66066dbaeb16-timelike-flow-ordering)
- [lem-author-66066dbaeb16-boundary-spacelike-tangency-comparison](item-lem-author-66066dbaeb16-boundary-spacelike-tangency-comparison)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)
- [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)
- [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)



## Statement

In the regular mass-one stationary vacuum/Harrison construction, with original section maximal and $T|_S\not\equiv0$, use the common spacelike reference collar and the fixed complete Hawking flow K with positive boost rate $\kappa$. Let $\rho=\rho_q$ be the reference induced distance to S. For q in [0,1], choose a barrier slope $M>0$ independent of q, distinct from the mass parameter, such that
$$2\kappa M>1+\sup_{q\in[0,1],\,S}|H_{g_q}(\Sigma_1)|.$$
For one sufficiently small common $\rho_0>0$, define
$$B_c^\pm=\{\phi^K_{c\mp M\rho(x)}x:x\in\Sigma_1,\ 0\le\rho(x)\le\rho_0\}.$$
These are smooth spacelike hypersurfaces with boundary S and the outer collar boundary. At $c=0$ their tangent hyperplanes and future normals along S agree with those of the reference section, and
$$H(B_0^\pm)|_S=H(\Sigma_1)|_S\mp2\kappa M.$$
They satisfy $H(B_c^+)<0<H(B_c^-)$ for every real c, with future-normal convention $H=\operatorname{div}_{g_q}n$.

Fix $\delta\in(0,1)$. For every $q\in[\delta,1]$, assume a supplied connected smooth spacelike maximal section $\Sigma_q$, smooth up to its compact boundary $S$, with one exterior end and interior the stationary graph $t=u_q(x)$ over $\Sigma_1^\circ$. Use the same stationary product and selected single-primitive Harrison family as in the compact-height result. Assume the family satisfies that result's complete candidate-section, normalized-end and uniform-estimate hypotheses, including all hypotheses required of its radial height-decay and transformed-lapse inputs, as well as the hypotheses of the supplied K-height result. In particular, the normalized end heights and their first spatial derivatives tend to zero uniformly in direction for each fixed $q$, the required end estimates hold on a common end with constants independent of $q\in[\delta,1]$, and the stationary lapse $-g_q(T,n_q)$ is positive in the interior. Their K-flow heights extend smoothly to S individually. Then
$$\sup_{0\le\rho_q\le\rho_0}|u_q^K|\le C_\delta.$$
The proof includes maxima attained on S: equality of boundary flow times gives tangent planes there, and the future-side comparison is used only on the exterior half-neighborhood. All-time translations take place in the supplied stationary collar saturation; local normal-coordinate comparisons use only a finite interval of times for each contact. No uniform estimates for an unbounded set of flow times are assumed.

The original-section maximality premise is imposed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$ for the original metric $g$, so $H_g|_C=0$. Where this result uses the original reference section $\Sigma_1$, it denotes the closure $B=C\cup S$ of this actual section. Maximality of a separately labelled chart-side region or another supplied section is not substituted for this premise. The spherical identification and the physical stationary end chart remain independent. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

For the uniform candidate-height conclusion, retain explicitly the two-sided original-metric far-end access premise of [pthm-compact-height-bound](item-pthm-compact-height-bound). For some $R_a$ and every $R\ge R_a$, with $U_R=\mathbb R\times\{r>R\}$ in the selected physical stationary end chart, require $\mathcal E\subset I^-_{(\mathcal E,g)}(U_R)\cap I^+_{(\mathcal E,g)}(U_R)$. Both witnessing timelike paths lie in the unchanged original exterior. This additional premise concerns the uniform candidate-height estimate; it is not needed for the preceding local construction and curvature signs of the translated barriers.

## Facts & Assumptions

[F1] Adopt the stationary vacuum model as conditional geometric assumptions. [post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[F2] The regular data supply the bifurcation sphere $S$ and the stated exterior. Original-metric maximality of its actual physical section is the separate Statement premise, not a conclusion of the regularity definition. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F3] The reference section is uniformly spacelike for all q in [0,1]; its induced distance, normals and jets have common smooth bounds, and the stationary collar saturation has the complete isometric K and periodic axial flows. [pthm-common-reference-collar](item-pthm-common-reference-collar)

[F4] The Hawking flow fixes S and acts on its normal plane by the boost with fixed positive rate kappa. [pthm-normal-boost-action](item-pthm-normal-boost-action)

[F5] Each supplied candidate has a unique smooth K-flow height on the collar extending smoothly to S; its boundary rapidity is kappa times its boundary height. [pthm-hawking-graph-height](item-pthm-hawking-graph-height)

[F6] For the selected single-primitive Harrison family, assume the actual physical exterior-section maximality and the explicit two-sided original-metric far-end access premise, together with the complete candidate-section, normalized-end and uniform-estimate hypotheses stated above. These match the current compact-height contract, so the stationary heights are uniformly bounded on every compact subset of the original exterior section for each fixed positive parameter interval. [pthm-compact-height-bound](item-pthm-compact-height-bound)

[F7] The Hawking and axial fields commute with T and satisfy $K=T$+Omega_H Z with fixed Omega_H and periodic axial flow. [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)

[F8] Flow graphs, spacelikeness and pulled-back mean curvature have the stated meanings. [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[F9] Mean curvature uses H=div(n) and future unit normals; maximal candidates have $H=0$. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F10] One-sided second-order contact has nonnegative Hessian without a boundary Hopf argument. [lem-author-66066dbaeb16-half-domain-contact-hessian](item-lem-author-66066dbaeb16-half-domain-contact-hessian)

[F11] The common spacelike graph mean-curvature jet has the positive Hessian symbol. [lem-author-66066dbaeb16-spacelike-common-graph-curvature-jet](item-lem-author-66066dbaeb16-spacelike-common-graph-curvature-jet)

[F12] Equal boundary K heights produce tangency and the same exterior side because K vanishes on S. [lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency](item-lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency)

[F13] Ordered flow heights imply geometric future-side ordering in the required local neighborhoods. [lem-author-66066dbaeb16-timelike-flow-ordering](item-lem-author-66066dbaeb16-timelike-flow-ordering)

[F14] The precise strict-barrier tangency comparison includes boundary contact and has the correct mean-curvature signs. [lem-author-66066dbaeb16-boundary-spacelike-tangency-comparison](item-lem-author-66066dbaeb16-boundary-spacelike-tangency-comparison)

[F15] Work in ZFC, retaining the smooth geometric suppliers' choice assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F16] Continuous images of compact spaces are compact, and continuous real-valued functions on nonempty compact spaces attain finite maxima and minima. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

[F17] Finite products of compact topological spaces are compact. [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)

[F18] Every closed bounded real interval $[a,b]$, with $a\le b$, is compact. [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)

## Proof

**Given:**The assumptions in the Statement.

**Goal:** Establish the stated comparison or estimate.

1.1 The reference collar in [F3] is a smooth compact q-family, and [F4] gives $K=0$ on S and $\nabla_{\bar\nu_q}^{(q)}K=\kappa\bar n_q$. At $c=0$ the variable-time graph differential on S is the identity, because its time is zero there and K vanishes. It therefore has exactly the reference tangent plane and future normal. For a reference unit radial curve x(rho), differentiating $\phi^K_{\mp M\rho}x(\rho)$ twice at zero changes its covariant acceleration by $\mp2M\nabla_{\bar\nu_q}K=\mp2\kappa M\bar n_q$. Tangential directions in TS have unchanged second form because the hypersurfaces have the same boundary embedding. Since $H=-\sum_i g_q(\bar n_q,\nabla_{e_i}e_i)$ at the shared first jet, the radial change gives precisely the displayed $\mp2\kappa M$ difference. [F3, F4, F8, F9, F12, given, algebra]

1.2 The family in the Statement meets all hypotheses of [F6], including actual physical exterior-section maximality, the explicit two-sided original-metric far-end access premise, the selected single-primitive family and uniform end-estimate requirements. The union $C$ of the reference outer boundaries $\rho_q=\rho_0$, for $q\in[\delta,1]$, is the image of $[\delta,1]\times S$ under the smooth boundary-distance map at radius $\rho_0$ from [F3]. Since $S$ is compact, [F16]–[F18] make $C$ compact; the common collar bounds keep it away from $S$. For a fixed positive period $P$ of the axial flow, its saturation is the continuous image of $[0,P]\times C$, hence is compact by [F16]–[F18]. Its smooth stationary projection is compact in the original section by [F16], and its continuous stationary time coordinate is bounded by the extreme-value part of [F16]. For $F_q(t,x)=t-u_q(x)$, the identities in [F7] give $F_q(\phi_s^Kx)=s+F_q(\phi_{\Omega_Hs}^Zx)$. At the unique intersection from [F5], this is zero. The second term is bounded uniformly by [F6], the compact projection and periodicity. Thus $|u_q^K|\le B_\delta$ on every outer reference boundary, for a common constant. [F3, F5, F6, F7, F16, F17, F18, given, algebra]

2.1 The boundary mean curvature is smooth on the compact parameter space $[0,1]\times S$ from [F3], so [F16]–[F18] give its finite uniform bound used to choose M. The chosen M gives a strict margin larger than one at S for all q. Compactness and the common smooth collar bounds permit one smaller rho0 on which both $c=0$ barriers remain embedded and spacelike and have the strict signs. Interior injectivity is also immediate from the reference K-flow product in [F3], and no finite orbit from an interior point can reach a zero of K. The boundary immersion has the reference tangent by step 1.1. Every translated barrier is the isometric image $B_c^\pm=\phi_c^K(B_0^\pm)$ in the supplied complete collar saturation, fixing S. The connected isometric flow preserves future orientation, hence spacelikeness and the asserted signs for every real c. [F3, F4, F8, F9, F16, F17, F18, step 1.1]

3.1 Fix q. The closed reference collar and its outer boundary are nonempty compact images of $S\times[0,\rho_0]$ and $S$, respectively, under the smooth boundary-distance map from [F3], by [F16]–[F18]. Smooth extension in [F5] makes $f=u_q^K+M\rho$ continuous there, so [F16] gives a finite maximum c* and an attained outer-boundary maximum. If c* exceeded its outer-boundary maximum, a maximizing point would lie in the interior or on S. The plus barrier with height $c*-M\rho$ lies on the future side of the candidate, by [F13], and touches it. At an interior contact the height difference has zero differential, so the surfaces are tangent. At a boundary contact $u_q^K(p)=c*$, so [F12] supplies tangency and the common exterior side independently of height derivatives. [F14], using the positive-symbol and half-domain facts [F10]–[F11], would imply $H(B_{c*}^+)\ge0$, contrary to step 2.1. Therefore $u_q^K+M\rho\le\max_{\rho=\rho_0}u_q^K+M\rho_0$. All local comparison times are finite because c* and the individual smooth boundary heights are finite. [F3, F5, F10, F11, F12, F13, F14, F16, F17, F18, step 2.1, step 1.2]

4.1 By [F16] on the same nonempty compact sets from step 3.1, the continuous function $u_q^K-M\rho$ attains a finite minimum $c_{\mathrm{min}}$ and an outer-boundary minimum. Apply the reversed argument to this minimum. If it were less than its outer-boundary minimum, the minus barrier with height $c_{\mathrm{min}}+M\rho$ would touch the maximal candidate from the past at an interior or boundary point. The same tangency statements apply, and [F14] would require $H(B_{c_{\mathrm{min}}}^-)\le0$, contrary to its strict positive sign. Hence $u_q^K-M\rho\ge\min_{\rho=\rho_0}u_q^K-M\rho_0$. Combining this with step 3.1 and the outer bound in step 1.2 gives $|u_q^K|\le B_\delta+M\rho_0$. This constant is independent of q on the fixed positive interval. [F5, F12, F13, F14, F16, step 2.1, step 1.2, step 3.1, algebra] ∎



The original article attributes this to maximum-principle comparison. The five local helpers establish exactly the needed second-jet comparison, including boundary contact where the Hawking field vanishes. No linear Schrödinger maximum principle is used for the nonlinear hypersurface step, and no new external theorem is needed after the local chain. The candidate sections and their individual smooth boundary extensions are premises; the present item supplies the uniform boundary-height estimate, not their existence or later gradient bounds.

## Source notes

The original article attributes this to maximum-principle comparison. The five local helpers establish exactly the needed second-jet comparison, including boundary contact where the Hawking field vanishes. No linear Schrödinger maximum principle is used for the nonlinear hypersurface step, and no new external theorem is needed after the local chain. The candidate sections and their individual smooth boundary extensions are premises; the present item supplies the uniform boundary-height estimate, not their existence or later gradient bounds.

These premises specify the generated conditional scope and are not attributed to the original article. The substantive local horizon conclusions are retained. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

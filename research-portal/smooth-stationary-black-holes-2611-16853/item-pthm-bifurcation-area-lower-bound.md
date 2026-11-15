---
title: "Theorem 4.2: charged horizon area lower bound"
status: draft
research_item: pthm-bifurcation-area-lower-bound
dependency_level: 28
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 26–27, Theorem 4.2 and its proof
      attribution: For sufficiently small positive q, the bifurcation-sphere area is
        at least 4π(1−q²); the proof records the electric and magnetic flux
        identities and combines stability with an area–charge inequality.
      hypotheses: The article's regular stationary vacuum construction, original
        maximal exterior section, mass-one normalization and nontrivial
        stationary field on the bifurcation sphere.
      reading_limits: Historical reading note retained from the current source; this
        maintenance revision claims no fresh article or external full-text
        reading. Read the frozen article text at the theorem and proof. This
        reference attributes the claim; it is not used as its proof.
---

PDF p. 26: ` Theorem 4.2 and proof `; PDF p. 27: ` Theorem 4.2 and proof `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-horizon-flux-and-stability-notation](item-def-horizon-flux-and-stability-notation)
- [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)
- [pthm-stable-bifurcation-mots](item-pthm-stable-bifurcation-mots)
- [pthm-stable-horizon-area-charge](item-pthm-stable-horizon-area-charge)
- [pthm-harrison-flux](item-pthm-harrison-flux)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [def-harrison-one-form](item-def-harrison-one-form)
- [def-harrison-electromagnetic-form](item-def-harrison-electromagnetic-form)
- [def-harrison-one-form-family](item-def-harrison-one-form-family)
- [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive)
- [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)
- [lem-author-294e9b08725d-regular-positive-stationary-mass](item-lem-author-294e9b08725d-regular-positive-stationary-mass)


## Statement

Assume the regular non-degenerate stationary vacuum model, with its original exterior section spacelike and maximal, ADM mass normalized to one, and stationary Killing field $T$ not identically zero on the bifurcation sphere $S$. Use the single stationary primitive and Harrison fields $g_q,F_q$ supplied by the global Harrison construction. Work in ZFC. For all sufficiently small $q>0$,

$$|S|_{g_q}\ge 4\pi(1-q^2).$$

Here $|S|_{g_q}=\int_S d\mu_q$, where $d\mu_q$ is the area form of the induced metric on the oriented sphere. Define the electric and magnetic flux densities by $(\star_{g_q}F_q)|_{TS}=e_q\,d\mu_q$ and $F_q|_{TS}=b_q\,d\mu_q$, with the orientation inherited from outward end spheres. In the same range,

$$\int_S e_q\,d\mu_q=4\pi\sqrt{1-q^2},\qquad \int_S b_q\,d\mu_q=0.$$

The lower bound follows by combining these flux identities with the stability area–charge inequality.

## Facts & Assumptions

[A1] The model, regularity, original maximal section and mass-one normalization are those in the Statement. A spacelike section has positive-definite induced metric; maximal means that its second fundamental form has zero trace. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-harrison-normalization](item-def-harrison-normalization)

[A2] Work in ZFC, including the axiom of choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The global one-form construction supplies the single smooth stationary primitive used in the Harrison family under these hypotheses. [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)

[F2] For each $q\in(0,1]$, the bifurcation-stability result supplies an individually admissible smooth spacelike maximal section with boundary $S$. Its Statement also supplies a smooth spacelike extension agreeing with the section on its original side near $S$, an outward normal-graph tube of radius allowed to depend on $q$, and nonnegative principal eigenvalue in the future/outward gauge. [pthm-stable-bifurcation-mots](item-pthm-stable-bifurcation-mots)

[F3] For such a section and its extension and graph tube, the stable-horizon inequality gives $|S|_{g_q}\ge(4\pi)^{-1}(\int_S e_q\,d\mu_q)^2$. The horizon notation fixes the induced area form and the two flux-density identities in the Statement. [pthm-stable-horizon-area-charge](item-pthm-stable-horizon-area-charge) [def-horizon-flux-and-stability-notation](item-def-horizon-flux-and-stability-notation)

[F4] With the mass-one stationary end expansion $g_{00}=-1+2/r+O_6(r^{-2})$ established in [F8], the supplied primitive and the inherited orientation, the Harrison flux result gives $(4\pi)^{-1}\int_S\star_{g_q}F_q=\sqrt{1-q^2}$ and $(4\pi)^{-1}\int_S F_q=0$ for $0\le q\le1$. [pthm-harrison-flux](item-pthm-harrison-flux)

[F5] The single-primitive family is $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. For the normalized Ernst potential $\sigma=f+i\psi$, the Harrison definitions specify $B_q=q(1+\sigma)+(1-\sigma)$, $D_q=|B_q|^2$, the metric $g_q$ and the electromagnetic form $F_q$ on their positive-denominator domain, using the same $W_q$, spacetime orientation and Hodge convention. The definitions require a supplied zero $p$ of $T$ and $d_q=D_q(p)>0$; they do not themselves supply the primitive. [def-harrison-one-form-family](item-def-harrison-one-form-family) [def-harrison-one-form](item-def-harrison-one-form) [def-harrison-electromagnetic-form](item-def-harrison-electromagnetic-form) [def-harrison-normalization](item-def-harrison-normalization)

[F6] Under [A1], the denominator-positivity result applies to the smooth normalized Ernst data supplied by the global construction. It gives $D_q>0$ on the exterior and on one open neighborhood of $S$ for $q\in[0,1]$, with $D_q\ge(1+q)^2$ on $S$. [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive) [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)

[F7] For this same $W_0$ and polynomial family, the regular electrovacuum result supplies the Harrison metric and real electromagnetic form on the exterior and an open neighborhood of $S$, where they are smooth in spacetime and satisfy the source-free Einstein–Maxwell equations. The orientations and fields are the same ones used by the flux and stability results. [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)

[F8] Under the regular stationary-vacuum hypotheses, the stationary-mass lemma gives $M_0=m_K=E$, where $E$ is the ADM energy of the original exterior section. Thus [A1]'s ADM mass-one convention gives $M_0=E=1$, and the regular end expansion becomes $g_{00}=-1+2/r+O_6(r^{-2})$; the bounds $g_{0i}=O_6(r^{-2})$ and $g_{ij}=\delta_{ij}+O_6(r^{-1})$ are unchanged. [lem-author-294e9b08725d-regular-positive-stationary-mass](item-lem-author-294e9b08725d-regular-positive-stationary-mass) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-harrison-normalization](item-def-harrison-normalization)

## Proof

**Given:** The model and construction hypotheses in the Statement.

**Goal:** Establish both flux identities and the area lower bound for all sufficiently small positive $q$.

**Proof technique:** direct.

1.1 Fix $q\in(0,1]$. By [F8], the regular stationary-vacuum hypotheses in [A1] imply $M_0=m_K=E$. The ADM mass-one assumption gives $E=1$, so $M_0=1$. Substitution into the regular end expansion yields $g_{00}=-1+2/r+O_6(r^{-2})$, together with the unchanged bounds $g_{0i}=O_6(r^{-2})$ and $g_{ij}=\delta_{ij}+O_6(r^{-1})$. These are the exact end conditions required by [F4]. The regular model, maximal original section, mass-one normalization and nontrivial $T|_S$ are exactly the hypotheses of the global primitive and regular electrovacuum results. By [F1], take their single $W_0$ and supplied pole $p\in S$ with $T_p=0$, and use the family in [F5]. The positivity conclusion [F6] applies to the supplied smooth normalized Ernst potential. At the pole, $f(p)=0$ and hence $d_q=(1+q)^2+(1-q)^2\psi(p)^2>0$; also $D_q=|B_q|^2>0$ makes $B_q\ne0$. Thus the parameter, pole and denominator conditions of both Harrison field definitions hold on the exterior and a neighborhood of $S$. The regular realization [F7] gives these same $g_q,F_q$ smoothly through $S$, with the prescribed orientation. [given, A1, F1, F5, F6, F7, F8, algebra]

2.1 Apply [F4] using the exact mass-one stationary end expansion established in step 1.1, and the same primitive and inherited orientation. Restricting its two form identities to $S$ and using the density definitions in [F3] gives $\int_S e_q\,d\mu_q=4\pi\sqrt{1-q^2}$ and $\int_S b_q\,d\mu_q=0$. The section and boundary data needed for the horizon notation are supplied by [F2] and step 1.1. [F2, F3, F4, step 1.1]

3.1 The Statement of [F2] supplies an individually admissible section, its smooth spacelike extension across $S$, its outward normal-graph tube and its outward stability, for the same fixed positive $q$. Together with step 1.1 these satisfy the section, smooth-field and graph hypotheses of [F3]. Applying that inequality and substituting the electric flux from step 2.1 yields $|S|_{g_q}\ge(4\pi)^{-1}(4\pi\sqrt{1-q^2})^2=4\pi(1-q^2)$. The fixed parameter was arbitrary in $(0,1]$, so both flux identities and the area bound hold in particular for all sufficiently small positive $q$. [given, F2, F3, step 1.1, step 2.1, algebra] ∎

## Source notes

The article reference records attribution. The deduction uses the completed suppliers, not the article's assertion as a premise.

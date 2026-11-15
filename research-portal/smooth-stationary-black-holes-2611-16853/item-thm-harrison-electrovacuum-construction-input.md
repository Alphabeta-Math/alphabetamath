---
title: Regular Harrison Einstein–Maxwell family
status: published
research_item: thm-harrison-electrovacuum-construction-input
dependency_level: 5
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: §1.1 GR/SBS and maximality; §3.1–3.3, Proposition 3.1, (3.5)–(3.25);
        Appendix A.1–A.3
      statement: Under mass-one GR, SBS and original maximality, Proposition 3.1
        defines the stationary regular Harrison tensors on E union O, asserts
        Einstein–Maxwell only on E, gives smooth metric and continuous field
        parameter dependence, normalized charges, and preservation of local
        horizon fields and surface gravity. §3.1–3.2 provides the normalized
        Ernst data, f<1 exterior bound and pole normalization used in the
        construction.
      hypotheses: Exactly the detailed [A2] assumptions; vacuum Ricci=0, mass one,
        normalized Ernst potential, source orientations and flux convention. SBS
        includes T not identically zero on the bifurcation sphere. No smallness
        of J, nor J<1, is an extra assumption of Proposition 3.1. The equations
        are imported on E only.
      reading_limits: Read the actual arXiv HTML v1 §1.1 hypotheses, §3.1–3.3
        construction and Proposition 3.1, Appendix A.1 formulas (A.2)–(A.11) and
        patching paragraph, and Appendix A.2 through its exterior f=0
        discussion. Checked the displayed algebra used in the five conditional
        helper proofs. Did not independently reconstruct the full
        Einstein–Maxwell, flux, local rigidity or horizon-collar proofs; those
        conclusions are explicitly imported at their exact source locators. No
        source reading or proof acceptance is asserted for the shared primitive
        resolution.
external_input: true
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data)
- [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [thm-stationary-harrison-primitive-input](item-thm-stationary-harrison-primitive-input)
- [lem-author-7a3c9628f105-denominator-positivity](item-lem-author-7a3c9628f105-denominator-positivity)
- [lem-author-7a3c9628f105-primitive-parameter-lift](item-lem-author-7a3c9628f105-primitive-parameter-lift)
- [lem-author-7a3c9628f105-rank-one-metric](item-lem-author-7a3c9628f105-rank-one-metric)
- [lem-author-7a3c9628f105-regular-maxwell-form](item-lem-author-7a3c9628f105-regular-maxwell-form)
- [lem-author-7a3c9628f105-exterior-boundary-scope](item-lem-author-7a3c9628f105-exterior-boundary-scope)
- [` Alexandru F. Radu, Rigidity of stationary black holes with small ADM angular momentum · §1.1 GR/SBS and maximality; §3.1–3.3, Proposition 3.1, (3.5)–(3.25); Appendix A.1–A.3 `](https://arxiv.org/html/2610.09729v1)


## Statement

Assume exactly Radu's mass-one GR/SBS and original maximal-slice hypotheses, detailed in Facts below. For $0\le q\le1$, the regular Harrison formulas define Lorentz metrics $g_q$ and real two-forms $F_q$ on $E\cup O$, for one neighborhood $O$ of the bifurcation sphere $S_0$. They satisfy $(g_1,F_1)=(g,0)$ and $\mathcal L_Tg_q=\mathcal L_TF_q=0$. On $E$ they satisfy the source-free geometric electrovacuum equations, and on outward oriented end spheres $S_r$ their electric and magnetic fluxes $(4\pi)^{-1}\int_{S_r}\star_{g_q}F_q$ and $(4\pi)^{-1}\int_{S_r}F_q$ are $\sqrt{1-q^2}$ and zero. The metrics depend smoothly on $q$ on compact subsets; the fields are spacetime smooth and continuous in $q$. Near $S_0$ the local commuting Killing fields $K,Z$ remain Killing, and the two horizon branches retain generator $K$ and its surface gravity. The sign of $g_q(T,T)$ equals the sign of $g(T,T)$. The tensors extend smoothly across $S_0$; equations there follow on $O\cap\overline E$ by continuity, without asserting equations throughout $O\setminus\overline E$. No small-angular-momentum bound is assumed.

## Facts & Assumptions

[A1] Work in ZFC, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice). The stationary, hypersurface, asymptotic, form, electrovacuum and circle-action interfaces are [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data), [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data), [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data), [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data), [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data), [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data) and [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data).

[A2] The precise imported GR data are a connected oriented time-oriented smooth vacuum four-spacetime, a spacelike acausal edgeless partial Cauchy hypersurface $\Sigma^0=\Phi_0(\{|x|>1/2\})$, $\Sigma_1=\Phi_0(\{|x|>1\})$, and $S_0=\Phi_0(\{|x|=1\})$. The stationary end has $T=\partial_t$ and $g_{00}=-1+2/r+O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$, $g_{0i}=-2\epsilon_{ijk}S^jx^kr^{-3}+O_6(r^{-3})$. The spacetime orientation is fixed by $\mathrm dt\wedge\mathrm dx^1\wedge\mathrm dx^2\wedge\mathrm dx^3$ in this chart and is used for every $\star_g$ and $\star_{g_q}$. Here $S_r=\{t=0,\ |x|=r\}$ has the outward boundary orientation induced by $\mathrm dx^1\wedge\mathrm dx^2\wedge\mathrm dx^3$ on the zero-time end slice. Its exterior $E=I^-(M^{\mathrm{end}})\cap I^+(M^{\mathrm{end}})$ is globally hyperbolic; $\Sigma^0\cap I^-(M^{\mathrm{end}})=\Sigma^0\cap I^+(M^{\mathrm{end}})=\Sigma_1$; $T$ is nowhere zero on $E$, with complete orbits meeting $\Sigma_1$ transversally. SBS requires the two chronological boundary hypersurfaces $H^\pm$ near $S_0$ to be smooth, null, transverse and nonexpanding, intersecting in $S_0$, with $T$ tangent to both and not identically zero on $S_0$. The induced geometry extends smoothly to $S_0$ and $\operatorname{tr}_h k=0$ on $\Sigma_1$. These are §1.1 GR, SBS and maximality of the independent external source, with mass rescaled to one; they are additional hypotheses rather than consequences of the interface definitions in [A1].

[F1] Use the normalized vacuum Ernst data of the source: $f=-g(T,T)$, $F=\tfrac12\mathrm dT^\flat$, $\mathcal F=F+i\star_gF$, $\sigma=f+i\psi$ with $\psi(\infty)=0$, $i_T\mathcal F=\tfrac12\mathrm d\sigma$, $f<1$ on $E$, and $f\le0$ on $S_0$. The local source fields obey $[K,Z]=0$, $T=K+\Omega Z$ with constant $\Omega\ne0$, $K|_{S_0}=0$, and the periodic field $Z$ has a pole $p$ where $T(p)=0$.

[F2] The shared stationary primitive supplier [thm-stationary-harrison-primitive-input](item-thm-stationary-harrison-primitive-input) gives $\mathrm dW_0=4((f-1)F+\psi\star_gF)$, $W_0(T)=D_0(p)-D_0$, smooth extension across $S_0$, local $K,Z$ invariance and the radial end choice $W_{0i}=O_5(r^{-3})$. Its normalization, decay and extension are existence inputs, not consequences of the following polynomial calculations.

[F3] The denominator, primitive lift, metric, electromagnetic tensor and boundary-scope arguments are [lem-author-7a3c9628f105-denominator-positivity](item-lem-author-7a3c9628f105-denominator-positivity), [lem-author-7a3c9628f105-primitive-parameter-lift](item-lem-author-7a3c9628f105-primitive-parameter-lift), [lem-author-7a3c9628f105-rank-one-metric](item-lem-author-7a3c9628f105-rank-one-metric), [lem-author-7a3c9628f105-regular-maxwell-form](item-lem-author-7a3c9628f105-regular-maxwell-form) and [lem-author-7a3c9628f105-exterior-boundary-scope](item-lem-author-7a3c9628f105-exterior-boundary-scope).

[F4] Radu Proposition 3.1, §3.1–3.3 and Appendix A are imported for the normalized vacuum inputs in [F1], the exterior Einstein–Maxwell equations (including exterior $f=0$), fluxes, and local horizon Killing-field and surface-gravity preservation, under [A2].

## Proof

**Given:**The hypotheses in the Statement and the Facts below.

**Goal:** Establish the stated conclusions.

1.1 Apply [F2] to fix one $W_0$; set $D_q=|1+q-(1-q)\sigma|^2$ and $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. The denominator lemma gives positivity on $E$ and a common neighborhood $O$ of $S_0$. The primitive-lift lemma gives $W_q(T)=D_q(p)-D_q$ and the curl identity. In particular no time-coordinate normalization is chosen independently of the contraction constant fixed at $p$. [A1, A2, F1, F2, F3]

2.1 The rank-one metric lemma gives $g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-(f/D_q)W_q\otimes W_q)$, its Lorentz signature, smoothness and sign identity. The regular-Maxwell lemma gives $F_q$ as the real part of its self-dual tensor formula, endpoint values and the stated distinct parameter regularities. Stationarity follows because every coefficient is formed algebraically from stationary fields. [A1, F1, F2, F3, step 1.1]

3.1 Apply the precisely scoped external construction input [F4] under [A2] for the Einstein–Maxwell equations on $E$, the two charge integrals, and preservation of $K,Z$ and the horizon surface gravity near $S_0$. These differential-equation, flux and horizon claims are imported; the preceding algebra alone does not establish them. The boundary-scope lemma extends the equations to $O\cap\overline E$ by continuity but supplies no equation on the open opposite side. Thus smooth horizon extension and exterior field equations have distinct scopes exactly as asserted. The imported construction assumes GR, SBS and maximality, with no global smallness hypothesis. [A1, A2, F3, F4, step 2.1] ∎



Radu Proposition 3.1 is imported for the exterior Einstein–Maxwell equations, the charge integrals, and preservation of the local horizon Killing fields and surface gravity, under precisely the GR/SBS and maximality hypotheses specified above. Appendix A.2 covers exterior points with $f=0$; its scope is not all of the horizon neighborhood.

## External input

Radu Proposition 3.1 is imported for the exterior Einstein–Maxwell equations, the charge integrals, and preservation of the local horizon Killing fields and surface gravity, under precisely the GR/SBS and maximality hypotheses specified above. Appendix A.2 covers exterior points with $f=0$; its scope is not all of the horizon neighborhood.

---
title: AIK global Kerr identification under the full GR/SBS/PK contract
status: published
research_item: pthm-author-d20d145f998f-aik-global-kerr-input
dependency_level: 2
sources:
  references:
    - title: "S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth
        stationary black holes in vacuum: small perturbations of the Kerr
        spaces"
      url: https://arxiv.org/pdf/0904.0982v1
      locator: §1.1, GR/SBS/PK and Main Theorem, PDF pp.4–5; §2.1 (2.1)–(2.5), PDF
        pp.6–7; normalized fields §2.3, PDF pp.8–9
      statement: Under GR, SBS and PK, the DOC E is isometric to the DOC of Kerr with
        mass M and angular momentum J. GR includes the stronger O6
        angular-momentum end coefficient, 0<=J<M², the two separate Sigma
        intersect I± equalities, T nonvanishing in E and complete orbits meeting
        Sigma. SBS is the smooth nonexpanding bifurcate-horizon package. PK is
        sufficiently small weighted Mars–Simon tensor in the source frame.
      hypotheses: All preceding GR, SBS and PK clauses in the source; no claim that a
        naked local Kerr isometry or the article regularity definition verifies
        them.
      reading_limits: "Consulted the extracted text of arXiv:0904.0982v1 in this
        assignment: section 1.1 GR/SBS/PK, footnotes 3, 5 and 6, and Main
        Theorem (PDF pp.4-5); section 2.1 equations (2.1)-(2.5) (PDF pp.6-7);
        section 2.3 equations (2.13)-(2.19) and normalization (PDF pp.8-9).
        These passages support the imported contract and conventions. No visual
        PDF inspection, reconstruction or independent review of the global
        rigidity proof is claimed."
    - title: M. Dafermos and I. Rodnianski, Lectures on black holes and linear waves
      url: https://arxiv.org/pdf/0811.0354v1
      locator: "Section 5.1, The Kerr metric, PDF pp.56-57 (printed pp.56-57):
        Boyer-Lindquist metric, parameter interpretation and DOC paragraph; p.57
        footnote 49 on spherical-coordinate charts."
      statement: For M>0 and 0<=|a|<M, a is angular momentum per unit mass; the
        displayed Boyer-Lindquist Kerr metric describes one domain of outer
        communications outside r_+=M+sqrt(M^2-a^2). The horizons are limiting
        boundaries of that coordinate exterior; a=0 reduces to Schwarzschild.
      hypotheses: The standard subextremal Kerr family, M>0 and 0<=|a|<M, with one
        selected asymptotically flat end. Used here with M=M_0 and a=J/M_0; the
        existing Kerr tensor supplier supplies the smooth sphere-axis
        convention.
      reading_limits: Consulted extracted PDF text of section 5.1 on PDF pp.56-57,
        including the metric, mass/specific-angular-momentum interpretation, DOC
        and horizon discussion, and footnote 49. Compared the displayed metric
        algebraically with physics:def-gr-fx-kerr-exterior. This imports only
        the standard Kerr exterior/DOC identification, not a uniqueness or
        stability theorem; no maximal-extension proof or visual inspection is
        claimed.
external_input: true
---

## Prerequisites

- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)
- [physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)
- [physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)
- [physics:def-gr-fx-kerr-exterior](https://alphabetamath.cc/physics/item/def-gr-fx-kerr-exterior)
- [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)
- [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth stationary black holes in vacuum: small perturbations of the Kerr spaces · §1.1, GR/SBS/PK and Main Theorem, PDF pp.4–5; §2.1 (2.1)–(2.5), PDF pp.6–7; normalized fields §2.3, PDF pp.8–9 `](https://arxiv.org/pdf/0904.0982v1)
- [` M. Dafermos and I. Rodnianski, Lectures on black holes and linear waves · Section 5.1, The Kerr metric, PDF pp.56-57 (printed pp.56-57): Boyer-Lindquist metric, parameter interpretation and DOC paragraph; p.57 footnote 49 on spherical-coordinate charts. `](https://arxiv.org/pdf/0811.0354v1)


## Statement

Let $(M,g)$ be a smooth connected oriented time-oriented paracompact four-dimensional vacuum spacetime with no manifold boundary, and let $T$ be a smooth Killing field. Impose all of the following independent-source hypotheses, without replacing them by the article's shorter regularity wording. Use Countable Choice for the smooth tangent-bundle conventions of the geometric suppliers.

**GR.** There is an embedded partial Cauchy hypersurface $\Sigma_0$ and a diffeomorphism $\Phi_0:\{x\in\mathbb R^3:|x|>1/2\}\to\Sigma_0$. Here partial Cauchy means achronal and edgeless; the edge of an achronal set consists of points in its closure for which every sufficiently small neighborhood contains a timelike curve from its local past to its local future avoiding the set. For large $R_0$, this chart extends to an end diffeomorphism $\mathbb R\times\{|x|>R_0\}\to M^{\rm end}$ with $T=\partial_t$. The source end bounds are $g_{00}=-1+2M_0/r+O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$ and $g_{0i}=-2\epsilon_{ijk}S^jx^k/r^3+O_6(r^{-3})$, where $M_0>0$ and $J=|S|<M_0^2$. The symbol $O_6$ bounds all coordinate derivatives up to order six with the corresponding extra inverse powers of $r$; stationary time derivatives vanish. Set $E=I^-(M^{\rm end})\cap I^+(M^{\rm end})$ using ambient timelike curves. Require that $E$, with the restricted metric and time orientation, is globally hyperbolic, the two separate equalities $\Sigma_0\cap I^-(M^{\rm end})=\Sigma_0\cap I^+(M^{\rm end})=\Phi_0(\{|x|>1\})$, nonvanishing of $T$ throughout $E$, and completeness of every $T$-orbit in $E$ with every such orbit meeting $\Sigma_0$.

**SBS.** The sphere $S_0=\Phi_0(\{|x|=1\})$ is the bifurcation sphere. In a neighborhood of it, $H^+=\partial I^-(M^{\rm end})$ and $H^-=\partial I^+(M^{\rm end})$ are smooth null nonexpanding hypersurfaces intersecting transversely in $S_0$. For a local smooth future null generator $L$ of either branch, its positive screen is $\mathscr S_p=L_p^\perp/\mathbb RL_p$, with $\bar q([X],[Y])=g(X,Y)$. A local spacelike two-dimensional section $Q$ transverse to $L$ identifies $T_pQ$ isometrically with this screen. With $q=g|_{TQ}$, define $\chi_L(X,Y)=g(\nabla_XL,Y)$ for $X,Y\in TQ$ and $\theta_L=\operatorname{tr}_q\chi_L=q^{AB}\chi_{L,AB}$, using the metric-selected connection and its pullback to $Q$. Nonexpanding means $\theta_L=0$ on every such local section. Under $L\mapsto e^fL$ both $\chi_L$ and $\theta_L$ scale by $e^f$, so this zero condition is independent of generator normalization, including the source null-pair convention $g(L,\underline L)=-1$ and the suppliers' convention $-2$. The stationary field is tangent to both hypersurfaces and is not identically zero on $S_0$.

**PK.** Use the source-normalized Ernst potential $\sigma\to1$ at infinity and the Mars–Simon tensor $\mathcal S$ of the declared interface, defined in an open neighborhood of $\Sigma_0\cap E$. For the future unit normal $E_0$ to $\Sigma_0$ and a smooth orthonormal frame $E_0,E_1,E_2,E_3$, require $|(1-\sigma)\mathcal S(T,E_\alpha,E_\beta,E_\gamma)|\le\varepsilon$ on $\Sigma_0\cap E$ for a sufficiently small positive $\varepsilon$ depending on the finite regularity constant $A$ constructed in source equations (2.1)–(2.5). If this tensor is zero, the PK bound is satisfied for every positive threshold, but all GR and SBS conditions remain required.

Under this complete GR/SBS/PK contract, $E$ is globally isometric to the domain of outer communication of the Kerr spacetime with mass $M_0$ and angular momentum magnitude $J$. Global isometry means one metric-preserving diffeomorphism onto that full Kerr domain. This source result does not assert that the original article's weaker displayed end and section assumptions automatically imply GR.

Concretely, the target uses the subextremal Kerr tensor on $\mathcal M_{\mathrm K}=\mathbb R_t\times(r_+,\infty)\times S^2$ from the declared Kerr interface, with its mass parameter $M=M_0$, specific angular momentum $a=J/M_0$ and $r_+=M_0+\sqrt{M_0^2-a^2}$. The GR bound gives $0\le a<M_0$. This is the full exterior for one selected asymptotically flat end, including the rotation axis via the smooth sphere tensor; the horizon $r=r_+$ is excluded. The standard identification of this exterior with that end's Kerr DOC is the imported geometric fact in Dafermos–Rodnianski, §5.1; it applies also when $J=a=0$.

## Statement references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)

[physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)

[physics:def-gr-fx-kerr-exterior](https://alphabetamath.cc/physics/item/def-gr-fx-kerr-exterior)

[physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)

[physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

## Facts & Assumptions

[F1] Smooth Lorentzian geometry, Killing fields, spacelike/acausal Cauchy vocabulary, global hyperbolicity and complete flows use the named interfaces. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field) [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets) [physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F2] The normalized Killing/Ernst/Mars–Simon definitions are the supplied convention. [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)

[F3] The vacuum field equation is conditional on the adopted classical Einstein field law with zero cosmological constant and no matter stress tensor. [physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)

[F4] The exact global conclusion under GR, SBS and PK is the imported AIK Main Theorem.

[F5] The null-normal and screen interfaces give the positive quotient metric, its identification with a spacelike section, the form $\chi_L$ and its trace $\theta_L$, and the boost laws $\chi_{e^fL}=e^f\chi_L$ and $\theta_{e^fL}=e^f\theta_L$. [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen) [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)

[F6] The Kerr tensor interface fixes the smooth exterior, including the axis, with $M=M_0$ and $a=J/M_0$. Dafermos–Rodnianski §5.1 supplies the standard identification with one Kerr DOC, including the $a=0$ case. [physics:def-gr-fx-kerr-exterior](https://alphabetamath.cc/physics/item/def-gr-fx-kerr-exterior)

[A1] Countable Choice is the smooth tangent-bundle convention required by the mathematical geometric suppliers. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

## External input

Imported established result: Alexakis–Ionescu–Klainerman, arXiv:0904.0982v1, §1.1 Main Theorem, PDF p.5. Its hypotheses are the preceding GR, SBS and PK clauses, including both separate chronological-section equalities, its angular-momentum end coefficient and subextremal parameter range. Its conclusion is expressly a global DOC isometry. The source's analytic continuation and final uniqueness argument are not reconstructed here. This import records a correctly scoped external theorem; application to a different hypothesis package remains a separate task.

The target identification uses Dafermos–Rodnianski, Lectures on black holes and linear waves, arXiv:0811.0354v1, §5.1, PDF pp.56–57: the standard subextremal Kerr DOC is the exterior represented by the displayed Boyer–Lindquist metric, with angular momentum $Ma$. Its metric agrees with the declared global Kerr tensor on polar charts and uses the latter's smooth sphere-axis convention. Only this target identification is imported from that source.

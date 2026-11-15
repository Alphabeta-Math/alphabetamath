---
title: Regular static boundary geometry and positivity of the end coefficient
status: draft
research_item: lem-author-f247c641a714-static-boundary-and-positive-mass
dependency_level: 3
---

## Prerequisites

- [def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)
- [lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction)
- [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)
- [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)
- [math:def-induced-connection-and-second-fundamental-form](https://alphabetamath.cc/item/def-induced-connection-and-second-fundamental-form)
- [math:def-totally-geodesic-submanifold](https://alphabetamath.cc/item/def-totally-geodesic-submanifold)
- [math:thm-collar-neighborhood-theorem](https://alphabetamath.cc/item/thm-collar-neighborhood-theorem)
- [math:thm-monotone-convergence-for-the-integral](https://alphabetamath.cc/item/thm-monotone-convergence-for-the-integral)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)
- [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing)
- [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)


## Statement

Assume the spatial static vacuum equations for the regular exterior data. Every boundary component is totally geodesic in $h$, and $|DV|_h$ is a positive constant on each component. Moreover
$$4\pi m=\int_X |DV|_h^2\,d\mu_h>0,$$
so $m>0$ follows from the original hypotheses and need not be added as a new assumption.

## Statement references

[def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)

[lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction)

[math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)

[math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)

[math:def-induced-connection-and-second-fundamental-form](https://alphabetamath.cc/item/def-induced-connection-and-second-fundamental-form)

[math:def-totally-geodesic-submanifold](https://alphabetamath.cc/item/def-totally-geodesic-submanifold)

[math:thm-collar-neighborhood-theorem](https://alphabetamath.cc/item/thm-collar-neighborhood-theorem)

[math:thm-monotone-convergence-for-the-integral](https://alphabetamath.cc/item/thm-monotone-convergence-for-the-integral)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)

[math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing)

[math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)

## Facts & Assumptions

[F1] The regular exterior data supply the connected oriented manifold with compact smooth boundary, the $C^2$ boundary metric and lapse, the single normalized end, and the inherited ZFC convention. The static reduction supplies $\Delta_hV=0$ and $D^2V=V\operatorname{Ric}(h)$, including their continuous boundary limits. The gradient, Hessian and divergence formulas fix the differential operators. [def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data) [lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction) [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)

[F2] Countable choice $\mathrm{AC}_\omega$ is included in the ZFC convention inherited in [F1]; it is used for the declared geometric and density-integration suppliers. Concretely, full choice applied to the family of values of a sequence of nonempty sets, followed by composition with that sequence, gives countable choice. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F3] The normal-valued second fundamental form is $\mathrm{II}(A,C)=(D_AC)^\perp$, and total geodesicity means $\mathrm{II}=0$. The smooth definitions assume countable choice. At the present $C^2$ boundary their pointwise formulas are used with the $C^1$ Levi–Civita coefficients; their extension independence and the normal-form identification are checked in step 1.1, without assuming that $h$ is smooth at $B$. [math:def-induced-connection-and-second-fundamental-form](https://alphabetamath.cc/item/def-induced-connection-and-second-fundamental-form) [math:def-totally-geodesic-submanifold](https://alphabetamath.cc/item/def-totally-geodesic-submanifold)

[F4] Under countable choice a smooth manifold with boundary admits a smooth collar $c:B\times[0,1)\to\overline X$, a diffeomorphism onto a relative neighborhood of $B$ with $c(p,0)=p$. This is a smooth-manifold assertion, independent of boundary regularity of $h$. [math:thm-collar-neighborhood-theorem](https://alphabetamath.cc/item/thm-collar-neighborhood-theorem)

[F5] The divergence theorem under countable choice applies to every smooth vector field on a compact oriented smooth Riemannian manifold with smooth boundary, with its outward normal. Our applications are on domains contained in $X$, where $h,V$ are smooth; compactness makes the support condition automatic. [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)

[F6] On the smooth interior, $d\mu_h$ is the intrinsic Borel measure of the positive smooth density $\sqrt{\det h}\,|dx^1dx^2dx^3|$. Under countable choice the density measure has its coordinate integral formula, and its integration agrees with smooth density integration on compact smooth domains. In oriented coordinates this is also the volume-form integral used by [F5], since both have coefficient $\sqrt{\det h}$. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing) [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)

[F7] For any measure space, nonnegative measurable $f_j$ increasing pointwise to $f$ satisfy $\int f_j\,d\mu\uparrow\int f\,d\mu$, with no prior finiteness assumption. [math:thm-monotone-convergence-for-the-integral](https://alphabetamath.cc/item/thm-monotone-convergence-for-the-integral)

## Proof

**Given:** The regular static data and reduced equations of [F1], their inherited countable choice in [F2], the geometric interfaces [F3]–[F5], and the integration interfaces [F6]–[F7].

**Goal:** Prove the regular boundary geometry and the positive energy identity without assuming a positive end coefficient.

1.1 The boundary limit in [F1] is $D^2V=0$. Because $V|_B=0$ and $dV\ne0$ there, $DV$ is nonzero and normal to $B$. If $n$ is the inward unit normal, positivity of $V$ inside implies $n(V)>0$, so $DV=n(V)n$ on $B$. For tangent fields $A,C$, the Hessian formula gives $D^2V(A,C)=n(V)h(D_A n,C)$. Metric compatibility gives $h(D_AC,n)=-h(C,D_A n)$, and hence $\mathrm{II}(A,C)=-h(D_A n,C)n$. These identities remain valid for the stated boundary regularity: the inverse metric is $C^2$, its Christoffel coefficients are $C^1$, and $n=DV/|DV|$ on $B$ is $C^1$. In a boundary chart, two extensions of a tangent field differ by coefficients vanishing on $B$; their tangential derivatives also vanish there. The formula $D_AW=A(W^i)\partial_i+\Gamma^i{}_{jk}A^jW^k\partial_i$ therefore proves extension independence along $B$. Orthogonal projection onto the line spanned by $n$ gives exactly the normal-valued form in [F3]. Since $n(V)>0$ and $D^2V(A,C)=0$, this form vanishes, proving total geodesicity in the pointwise sense of [F3]. [given, F1, F2, F3]

1.2 Take the collar $c$ from [F4] and fix $0<t_0<1$. The strip $c(B\times[0,t_0])$ is compact. Choose $R_*$ so large that it and the compact core lie inside the region bounded by the end sphere $S_{R_*}$. For $R\ge R_*$ let $K_R$ be the complement in $\overline X$ of the end region $r>R$; it is compact by the compact-core hypothesis. Set $R_j=R_*+j$, $\varepsilon_j=t_0/(j+1)$ and $D_j=K_{R_j}\setminus c(B\times[0,\varepsilon_j))$. These are compact smooth domains entirely in $X$, with disjoint boundary faces $S_{R_j}$ and $B_{\varepsilon_j}=c(B\times\{\varepsilon_j\})$. They satisfy $D_j\subset D_{j+1}$ and $\bigcup_jD_j=X$: the end cutoff eventually includes each point, and the shrinking collar eventually excludes no fixed interior point. The product rule gives $\operatorname{div}_h(VDV)=|DV|_h^2+V\Delta_hV=|DV|_h^2$. Applying [F5] on $D_j$ therefore expresses its energy integral as the sum of its outer and inner fluxes. [given, F1, F2, F4, F5, F6]

2.1 For tangent $A$, metric compatibility and the Hessian formula give $A(|DV|_h^2)=2D^2V(A,DV)=0$ on $B$. Thus $|DV|_h^2$ is locally constant on $B$, and is constant on each connected component. Its value is positive there because $dV\ne0$. [given, F1, step 1.1]

2.2 The pullback metrics $c_s^*h$ on the compact $B$, for $0\le s\le t_0$, depend continuously on $(p,s)$ and are positive definite. Relative to $c_0^*h$ their area ratios are uniformly bounded by compactness. The latter has finite area by a finite boundary atlas and bounded continuous coordinate densities. Hence $\operatorname{Area}_h(B_s)\le C$. Also $V(c(p,s))=\int_0^s\partial_t(V\circ c)(p,t)\,dt=O(s)$ uniformly, and $|DV|_h$ is uniformly bounded on the strip by the $C^2$ data. With either unit normal on $B_s$, the absolute flux of $VDV$ is consequently at most $Cs$, so the inner flux for $D_j$ tends to zero. These estimates use the smooth collar and continuity on its compact strip, not a smooth-metric theorem at $B$. [given, F1, F4, step 1.2]

3.1 The differentiated end conditions give $\partial_rV=m/R^2+O(R^{-3})$, $DV=O(R^{-2})$ in the end Cartesian frame, the outward unit normal $\nu_h=\partial_r+O(R^{-1})$ in that frame, and $dA_h=(1+O(R^{-1}))R^2d\omega$. Since $V=1+O(R^{-1})$, the outer flux is $\int_{S_R}Vh(DV,\nu_h)\,dA_h=4\pi m+O(R^{-1})$. Combining this with the vanishing inner flux yields $\lim_j\int_{D_j}|DV|_h^2\,d\mu_h=4\pi m$. [given, F1, F5, F6, step 1.2, step 2.2]

4.1 The sets $D_j$ are Borel, and $f_j=\mathbf1_{D_j}|DV|_h^2$ are nonnegative measurable functions on the measure space $(X,\mathcal B(X),\mu_h)$ of [F6]. They increase pointwise to $|DV|_h^2$ by step 1.2. Monotone convergence [F7] and step 3.1 give $\int_X|DV|_h^2\,d\mu_h=4\pi m$, in particular a finite integral. To see strict positivity, fix a boundary point, where $|DV|_h>0$. Continuity supplies an interior coordinate ball on which $|DV|_h^2$ is bounded below by a positive constant. A smaller ball has positive $\mu_h$-measure by the positive continuous coordinate density in [F6]. The energy is therefore strictly positive, and $m>0$ follows. [given, F1, F6, F7, step 1.1, step 2.1, step 1.2, step 3.1] ∎

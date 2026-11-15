---
title: Non-rotating staticity and Schwarzschild uniqueness
status: published
research_item: pthm-nonrotating-static-uniqueness
dependency_level: 6
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: "Attribution only: PDF p. 2, §1.1; p. 4, Remark 1.2."
      statement: Attributes the nonrotating Schwarzschild claim and the
        zero-bifurcation-field staticity claim to prior results.
      hypotheses: The regular stationary asymptotically flat vacuum setting and the
        nonrotating branch described by the article.
      reading_limits: Read the frozen article text on pp. 2–4 and inspected the frozen
        PDF image of p. 4. Used only for original-claim attribution; no premise
        of the proof is imported from this attribution.
    - title: A. F. Radu, On rigidity of stationary black holes under a nontrapping
        assumption, arXiv:2609.23872v2
      url: https://arxiv.org/pdf/2609.23872v2
      locator: §1.1, GR and SBS, PDF/printed pp. 3–4; Lemma 2.13, p. 25; §6,
        nonrotating branch of the proof of Theorem 1.1, pp. 69–70.
      statement: The branch T|S=0 proves global staticity and Schwarzschild uniqueness
        using an exterior-preserving completion and maximal-slice preparation.
        It does not use NT.
      hypotheses: "The GR/SBS contract stated in the direct supplier: smooth
        stationary vacuum geometry; positive normalized ADM mass; the specified
        O6 end; an acausal edgeless end-aligned partial Cauchy section with
        exact chronological section equalities; globally hyperbolic exterior
        with complete stationary orbits; smooth transverse nonexpanding horizons
        tangent to T; and T|S=0."
      reading_limits: Read the retained full-PDF text at pp. 3–4, 25 and 69–70 and
        opened the independent arXiv PDF. Checked the stated hypotheses and this
        application; did not reconstruct or independently audit the imported
        completion, maximal-existence or static-classification proofs. The
        direct supplier carries the external result; the present proof supplies
        local hypothesis matching.
---

PDF p. 2: ` §1.1 and Remark 1.2 `; PDF p. 4: ` §1.1 and Remark 1.2 `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity)
- [lem-author-a4a441da4986-zero-stationary-boundary-data](item-lem-author-a4a441da4986-zero-stationary-boundary-data)
- [lem-author-a4a441da4986-doc-connected-and-causally-convex](item-lem-author-a4a441da4986-doc-connected-and-causally-convex)
- [lem-author-a4a441da4986-cauchy-closure-double-boundary](item-lem-author-a4a441da4986-cauchy-closure-double-boundary)
- [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)
- [physics:def-gr-schwarzschild-exterior-model](https://alphabetamath.cc/physics/item/def-gr-schwarzschild-exterior-model)
- [lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar)
- [lem-author-a4a441da4986-nonrotating-positive-komar-mass](item-lem-author-a4a441da4986-nonrotating-positive-komar-mass)
- [pthm-author-a4a441da4986-regular-nonrotating-schwarzschild-input](item-pthm-author-a4a441da4986-regular-nonrotating-schwarzschild-input)
- [` A. F. Radu, On rigidity of stationary black holes under a nontrapping assumption, arXiv:2609.23872v2 · §1.1, GR and SBS, PDF/printed pp. 3–4; Lemma 2.13, p. 25; §6, nonrotating branch of the proof of Theorem 1.1, pp. 69–70. `](https://arxiv.org/pdf/2609.23872v2)


## Statement

In the regular asymptotically flat stationary vacuum setting of the article, a non-rotating black hole has Schwarzschild exterior. In particular, if the stationary field vanishes on the bifurcation sphere, $T|_S\equiv0$, the entire exterior is static and globally isometric to a Schwarzschild exterior of positive mass. Non-rotation means that $T$ is tangent to the horizon null-generator lines; at the transverse spacelike bifurcation sphere this implies $T|_S=0$. No maximal-slice, analyticity, nontrapping or additional global ambient-completeness assumption is added to the article’s regularity hypotheses.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity)

[lem-author-a4a441da4986-zero-stationary-boundary-data](item-lem-author-a4a441da4986-zero-stationary-boundary-data)

[lem-author-a4a441da4986-doc-connected-and-causally-convex](item-lem-author-a4a441da4986-doc-connected-and-causally-convex)

[lem-author-a4a441da4986-cauchy-closure-double-boundary](item-lem-author-a4a441da4986-cauchy-closure-double-boundary)

[lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)

[physics:def-gr-schwarzschild-exterior-model](https://alphabetamath.cc/physics/item/def-gr-schwarzschild-exterior-model)

[lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar)

[lem-author-a4a441da4986-nonrotating-positive-komar-mass](item-lem-author-a4a441da4986-nonrotating-positive-komar-mass)

[pthm-author-a4a441da4986-regular-nonrotating-schwarzschild-input](item-pthm-author-a4a441da4986-regular-nonrotating-schwarzschild-input)

## Facts & Assumptions

[A1] Adopt the stationary vacuum model and precisely the article regularity/horizon definitions. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity)

[F1] Vanishing of the nontrivial stationary field on the transverse spacelike bifurcation sphere gives the local bifurcate Killing-horizon data. [lem-author-a4a441da4986-zero-stationary-boundary-data](item-lem-author-a4a441da4986-zero-stationary-boundary-data)

[F2] The exterior is connected and causally convex; Cauchy-section closure lies only on the double horizon. The complete-up-to-boundary section is the connected component containing the physical stationary end, with compact core and one asymptotically Euclidean end. The exact section result supplies an adapted topological radial identification in which that component is the outer radial component; it does not assert this for every originally specified radial identification. Its end-metric estimates use the original physical end coordinates. [lem-author-a4a441da4986-doc-connected-and-causally-convex](item-lem-author-a4a441da4986-doc-connected-and-causally-convex) [lem-author-a4a441da4986-cauchy-closure-double-boundary](item-lem-author-a4a441da4986-cauchy-closure-double-boundary) [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)

[F3] The working-collar result gives an exterior-preserving working spacetime with the source’s acausal edgeless partial Cauchy section, exact chronological section equalities and full double chronological boundary equal to $S$. [lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar)

[F4] In the zero-bifurcation-field case the normalized end coefficient equals the positive ADM rest mass, without assuming a maximal slice or staticity. [lem-author-a4a441da4986-nonrotating-positive-komar-mass](item-lem-author-a4a441da4986-nonrotating-positive-komar-mass)

[F5] Under its explicit GR/SBS hypotheses and $T|_S=0$, the independent nonrotating theorem gives global staticity and a global Schwarzschild isometry of the entire exterior. Its completion and maximal-slice preparation are imported parts of that result. [pthm-author-a4a441da4986-regular-nonrotating-schwarzschild-input](item-pthm-author-a4a441da4986-regular-nonrotating-schwarzschild-input)

[F6] The Schwarzschild exterior is the mathematical model $\mathbb R\times(2M_0,\infty)\times S^2$ with metric $-(1-2M_0/\rho)\,dt^2+(1-2M_0/\rho)^{-1}\,d\rho^2+\rho^2\gamma_{S^2}$. In the model definition take $G_N=c=1$ and positive mass parameter $m_*=M_0$, so $x^0=t$ and the Schwarzschild radius is $2M_0$. Here $\rho$ is the model’s areal radius, separate from the working-section parameter in step 1.2. [physics:def-gr-schwarzschild-exterior-model](https://alphabetamath.cc/physics/item/def-gr-schwarzschild-exterior-model)

## Proof

**Given:** The article’s regular spacetime, selected end and bifurcation sphere, with non-rotation or $T|_S=0$, and the inputs [A1], [F1]–[F6].

**Goal:** Establish global staticity and Schwarzschild uniqueness under the original hypotheses.

1.1 In the non-rotating case, tangency to both transverse horizon sheets places $T$ in $TS$, while non-rotation places it in the null-generator line. The positive-definite metric on $TS$ therefore makes $T=0$ there. If $T|_S=0$ is assumed directly, this conclusion is already given. The field is nontrivial because it is timelike in the asymptotic end, so [F1] identifies the given sheets as Killing horizons for $T$ near $S$. [given, A1, F1]

1.2 Put $C=\Sigma_0\cap E$. Apply [F2] to the connected selected end and the given exterior Cauchy section. Then $E$ and $C$ are connected, every additional ambient closure point of $C$ lies in the double chronological boundary $S$, and $C$ is the component containing the original stationary end. Its closure $C\cup S$ is complete up to $S$, with a compact core and one asymptotically Euclidean end. The radial outer-component description supplied by [F2] uses an adapted identification, which may differ from the original section identification and from the physical end chart. By [F3], pass to the working spacetime $M'$ containing the same $E$ and a neighborhood of $S$. Choose the working-section parametrization supplied there and denote its radial parameter by $\rho$. It has an embedded acausal edgeless section $\Sigma'\cong\{\rho>1/2\}$, with $C=\{\rho>1\}$, unchanged near $S$ and on the physical end, for which $\Sigma'\cap I^+_{M'}(M^{\rm end})=\Sigma'\cap I^-_{M'}(M^{\rm end})=C$. The parameter $\rho$ labels these topological section regions; the original end coordinates continue to supply the metric estimates. Its DOC is exactly $E$, its full double chronological boundary is $S$ by the working-collar result in [F3], and its local chronological horizon sheets are unchanged. Take the connected component containing $E$ and its collar if needed; all these data remain in it. [given, A1, F2, F3]

2.1 By [F4] and step 1.1, $M_0=M_{\rm ADM}>0$ on this nonmaximal compact-core section. Match the contract of [F5] in the working spacetime: the restricted geometry is smooth, oriented, time-oriented and vacuum with the same Killing field; the unchanged end has future $T=\partial_t$, the original $O_6$ expansions and $t=0$ section alignment, with its mass now verified positive. Its DOC is the same globally hyperbolic $E$; the complete exterior stationary orbits meet $C$, since they meet $\Sigma_0$ within $E$. Step 1.2 supplies the required partial Cauchy section, radial parametrization and both exact chronological section equalities. By [F3] and step 1.2, the full double chronological boundary in $M'$ is exactly $S$, and the two local sheets remain smooth, transverse, null, nonexpanding and tangent to $T$. Thus GR and SBS, including the zero-field condition from step 1.1, hold with no additional original hypothesis. [given, A1, F3, F4, F5, step 1.1, step 1.2]

3.1 Apply the full nonrotating conclusion of [F5] to the data verified in step 2.1. It gives staticity throughout $E$ and a global isometry of $E$ with the Schwarzschild exterior of mass $M_0>0$, understood with the metric, exterior domain and geometrized units of [F6]. This imports the source’s completion and maximal-slice staticity argument, including its final classification; no end graph or stronger differentiated bound for a selected auxiliary slice is inferred here. Since the working restriction and the source’s completion preserve exactly the original $E$ with its metric and stationary field, the conclusion is the required one for the original exterior. [F5, F6, step 1.2, step 2.1] ∎

## Source notes

The original article is cited only for attribution. The independent nonrotating branch is used through its explicit external-input supplier, after the section and positive-mass hypotheses are verified locally. Its maximal-slice preparation explains the original staticity route, but the present application uses the full staticity and Schwarzschild conclusion. No local reconstruction of the imported global theorems is claimed.

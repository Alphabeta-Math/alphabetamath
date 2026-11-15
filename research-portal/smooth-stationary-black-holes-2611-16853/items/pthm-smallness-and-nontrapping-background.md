---
id: pthm-smallness-and-nontrapping-background
title: Reported smooth uniqueness under additional hypotheses
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - pthm-small-horizon-field-rigidity-input
  - physics:def-gr-fx-kerr-exterior
  - def-author-ad064c44a1cc-perturbative-gr-sbs
  - def-author-ad064c44a1cc-ernst-curvature-package
  - def-author-ad064c44a1cc-weighted-mars-simon
  - def-author-ad064c44a1cc-perturbative-effective-constant
  - def-author-ad064c44a1cc-weighted-pk-condition
  - def-author-ad064c44a1cc-nontrapping-gr
  - def-author-ad064c44a1cc-nontrapping-sbs
  - def-author-ad064c44a1cc-stationary-orbit-topology
  - lem-author-ad064c44a1cc-zero-stationary-energy
  - def-author-ad064c44a1cc-maximal-zero-energy-nontrapping
  - def-author-ad064c44a1cc-adm-gr-sbs
  - def-author-ad064c44a1cc-adm-angular-momentum-parameters
  - def-author-ad064c44a1cc-adm-maximal-section
  - def-author-ad064c44a1cc-adm-effective-geometry
  - lem-author-ad064c44a1cc-adm-threshold-quantifiers
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  pthm-small-horizon-field-rigidity-input: physical-result
  physics:def-gr-fx-kerr-exterior: mathematical-premise
  def-author-ad064c44a1cc-perturbative-gr-sbs: mathematical-premise
  def-author-ad064c44a1cc-ernst-curvature-package: mathematical-premise
  def-author-ad064c44a1cc-weighted-mars-simon: mathematical-premise
  def-author-ad064c44a1cc-perturbative-effective-constant: mathematical-premise
  def-author-ad064c44a1cc-weighted-pk-condition: mathematical-premise
  def-author-ad064c44a1cc-nontrapping-gr: mathematical-premise
  def-author-ad064c44a1cc-nontrapping-sbs: mathematical-premise
  def-author-ad064c44a1cc-stationary-orbit-topology: mathematical-premise
  lem-author-ad064c44a1cc-zero-stationary-energy: mathematical-premise
  def-author-ad064c44a1cc-maximal-zero-energy-nontrapping: mathematical-premise
  def-author-ad064c44a1cc-adm-gr-sbs: mathematical-premise
  def-author-ad064c44a1cc-adm-angular-momentum-parameters: mathematical-premise
  def-author-ad064c44a1cc-adm-maximal-section: mathematical-premise
  def-author-ad064c44a1cc-adm-effective-geometry: mathematical-premise
  lem-author-ad064c44a1cc-adm-threshold-quantifiers: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p.3 §1.1, paragraphs citing [2], [3], [35] and [36]
      reading_limits: Read the original extracted passage and rendered PDF p.3 for
        attribution and the distinction among the four alternative prior
        results. The original article is not used to prove its own
        prerequisites.
    - title: "S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth
        stationary black holes in vacuum: small perturbations of the Kerr
        spaces"
      url: https://arxiv.org/html/0904.0982v1
      locator: §1.1 setup, GR/SBS/PK (1.1)–(1.4), Main Theorem; §2.1 (2.1)–(2.5); §2.3
        (2.13)–(2.20)
      statement: "For a connected oriented time-oriented smooth vacuum four-spacetime
        with the source GR/SBS data, asymptotic mass M0>0 and J=|S|<M0^2, a
        normalized Ernst potential and Mars–Simon tensor in the source
        convention, and PK: |(1−sigma)S(T,e_a,e_b,e_c)|≤epsilon_bar on Sigma0
        intersect closure(E) for all a,b,c=0,1,2,3, epsilon_bar sufficiently
        small depending only on Abar_PK of (2.5), the domain of outer
        communication is isometric to the Kerr domain of outer communication of
        mass M0 and angular magnitude J."
      hypotheses: "Exactly the five local AIK interface items: source
        partial-Cauchy/end/orbit GR package; smooth nonexpanding transverse
        event horizons with T tangent and T not identically zero on S0;
        normalized potential and source-convention weighted Mars–Simon tensor on
        a neighborhood of the relevant slice; actual coordinate bounds
        A1,R1,epsilon0,A2 and Abar_PK; component inequality PK at the
        source-dependent tolerance. No maximality or small horizon-field norm is
        substituted."
      reading_limits: Freshly retrieved arXiv HTML v1 and read §1.1 setup and all
        GR/SBS/PK clauses and Main Theorem, §2.1 coordinate construction and
        (2.1)–(2.5), §2.3 (2.13)–(2.20) and nearby potential and
        weighted-smoothness sentences. The rigidity proof, Carleman propagation
        and Kerr classification were not reviewed or reconstructed. Curvature is
        retained in the source convention, not silently converted.
    - title: Alexandru F. Radu, On rigidity of stationary black holes under a
        nontrapping assumption
      url: https://arxiv.org/html/2609.23872v1
      locator: §1.1 setup, GR (1.1), SBS, quotient-space definition, NT and Theorem
        1.1; §1.2 first paragraph
      statement: Under the source GR, SBS and NT, the exterior is isometric to a
        nonextremal Kerr exterior. NT means that no maximal unparametrized null
        geodesic in the open exterior with g(T,gamma_dot)=0 has its full
        stationary projection contained in a compact subset of Q=E/R with the
        quotient topology; maximality includes finite affine parameter
        intervals.
      hypotheses: "Exactly the five local NT interface items: smooth connected
        oriented time-oriented Ricci-flat four-spacetime with stationary Killing
        field; acausal edgeless source slice; source end coefficients with M0>0
        and |S|<M0^2; globally hyperbolic exterior, complete orbits meeting
        Sigma1 and the source chronological intersections; source SBS event
        horizons, with no added T|S0 not-identically-zero clause; zero-energy
        maximal-geodesic nontrapping in the open-exterior quotient. No
        maximality or smallness condition is added."
      reading_limits: Freshly retrieved arXiv HTML v1 and read §1.1 complete setup,
        GR, SBS, quotient topology, NT, maximality paragraph and Theorem 1.1,
        the immediately following energy paragraph, and §1.2 opening on rotating
        and zero-field cases. The proof of quotient smoothness/properness,
        extension theorem and staticity/Kerr classification were not reviewed or
        reconstructed.
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: §1.1 setup, GR/SBS, maximality, (1.1)–(1.3) and Theorem 1.1
      statement: Assume the source GR/SBS package, original maximality of Sigma1 and
        J<M0^2. For every fixed A there exists j_*(A)>0 such that M0=1,
        Abar_ADM≤A and J<j_*(A) imply that the exterior is isometric to a
        subextremal Kerr exterior.
      hypotheses: "Exactly the five local ADM interface items: source stationary
        vacuum GR with angular end coefficient, complete nowhere-zero exterior T
        orbits meeting Sigma1 transversally and chronological intersections;
        rotating SBS with T not identically zero on S0; source maximal slice
        with induced geometry smooth to S0; mass-one normalization of charge
        parameters; the actual six-derivative geometric chart constant including
        radius, inverse collar width and inverse subextremal gap, bounded by
        fixed A; angular magnitude J below j_*(A)."
      reading_limits: Freshly retrieved arXiv HTML v1 and read §1.1 setup, GR/SBS,
        induced-geometry/maximality clauses, quantitative chart paragraphs
        (1.2)–(1.3), Theorem 1.1 and its immediately following
        nonvanishing-limit qualification. The compactness, Harrison,
        area-comparison and classification proof was not reviewed or
        reconstructed.
physical_scope: Conditional classical four-dimensional stationary vacuum
  Einstein model, with zero cosmological constant and stress-energy. These are
  four alternative source-specific rigidity results, not observational claims or
  a combined smallness assumption.
dependency_level: 8
---

## Statement

In the classical four-dimensional stationary vacuum model, the following are four alternative source-specific conditional Kerr rigidity statements. Each application must supply its whole named package; the hypotheses are not one cumulative list and are not consequences of the original article's regularity definition alone.

**Perturbative slice condition.** Under the AIK perturbative GR/SBS, Ernst/curvature and quantitative chart packages, impose the weighted PK component bound $|\mathcal W(T,e_a,e_b,e_c)|\le\overline\varepsilon$ on $\Sigma^0\cap\overline E$, where $\mathcal W=(1-\sigma)\mathcal S$ is interpreted by its smooth extension. With $\overline\varepsilon$ sufficiently small depending only on $\overline A_{\rm PK}$, the exterior is isometric to the Kerr exterior with the source mass $M_0$ and angular magnitude $J<M_0^2$. This is the source's weighted Mars–Simon condition, not an unspecified metric perturbation or a bound solely on the horizon. Maximality is not added to this branch.

**Small horizon field.** Under the already authored AIK horizon-smallness supplier's exact GR/SBS/maximal and quantitative package, after its own constant $A$ is fixed, $\sup_{S_0}|g(T,T)|<\epsilon_*^2(A)$ gives a subextremal Kerr exterior (and the source small-angular-momentum range). That supplier also records the corresponding rotational-neighborhood confinement. It retains its own $T|_{S_0}\not\equiv0$ clause. Its horizon norm is not replaced by ADM smallness or PK.

**Zero-energy nontrapping.** Under the NT source's GR/SBS package, if no maximal unparametrized null geodesic in $E$ orthogonal to $T$ has its complete projection in a compact subset of the open stationary quotient $Q=E/\mathbb R$, the exterior is isometric to a nonextremal Kerr exterior. Finite affine parameter intervals remain within the maximality convention. The source includes the case $T|_{S_0}\equiv0$; it imposes no maximal-slice or smallness condition and allows nonzero-energy photon trapping.

**Small ADM angular magnitude with geometry controlled.** Under the ADM source's GR/SBS, original maximality/smooth-boundary and quantitative chart package, with $M_0=1$ and $J<1$, for every fixed bound $A$ there exists $j_*(A)>0$ such that $\overline A_{\rm ADM}\le A$ and $J<j_*(A)$ give a subextremal Kerr exterior. Here $J$ is the normalized magnitude $|S|$, not a horizon-field norm, and the geometric bound remains essential to this imported statement.

## Facts & Assumptions

[A1] Adopt the stationary vacuum model [[post-stationary-vacuum-model]]. For each branch the additional source vacuum/geometric predicates must also be supplied; this model does not imply any source's complete GR/SBS or smallness package.

[F1] The perturbative source interfaces are [[def-author-ad064c44a1cc-perturbative-gr-sbs]], [[def-author-ad064c44a1cc-ernst-curvature-package]], [[def-author-ad064c44a1cc-weighted-mars-simon]], [[def-author-ad064c44a1cc-perturbative-effective-constant]] and [[def-author-ad064c44a1cc-weighted-pk-condition]]. Import the exact AIK Main Theorem in External input as the global rigidity input for this branch.

[F2] The independent horizon-field theorem, including its source hypotheses, norm equivalence, confinement qualification and threshold, is [[pthm-small-horizon-field-rigidity-input]].

[F3] The nontrapping source interfaces are [[def-author-ad064c44a1cc-nontrapping-gr]], [[def-author-ad064c44a1cc-nontrapping-sbs]], [[def-author-ad064c44a1cc-stationary-orbit-topology]], [[lem-author-ad064c44a1cc-zero-stationary-energy]] and [[def-author-ad064c44a1cc-maximal-zero-energy-nontrapping]]. Import Radu Theorem 1.1 in External input for the global rigidity conclusion.

[F4] The ADM source interfaces are [[def-author-ad064c44a1cc-adm-gr-sbs]], [[def-author-ad064c44a1cc-adm-angular-momentum-parameters]], [[def-author-ad064c44a1cc-adm-maximal-section]], [[def-author-ad064c44a1cc-adm-effective-geometry]] and [[lem-author-ad064c44a1cc-adm-threshold-quantifiers]]. Import the separate Radu small-ADM Theorem 1.1 in External input.

[F5] A subextremal Kerr exterior uses the standard Kerr tensor with $M_0>0$, $|a|<M_0$, $r>r_+=M_0+\sqrt{M_0^2-a^2}$. [[physics:def-gr-fx-kerr-exterior]]

## Proof

**Given:**The adopted vacuum model and, for the branch being asserted, all the source-specific assumptions in the Statement.

**Goal:** Establish each conditional conclusion without conflating its input with another branch.

1.1 In the perturbative branch [F1] supplies the exact source GR/SBS geometry, the source-convention Mars–Simon construction and its globally smooth weighted tensor, the actual finite $\overline A_{\rm PK}$, and the PK inequality with its parameter order. Thus the imported AIK Main Theorem applies directly with the same normalization and gives the Kerr domain-of-outer-communication isometry. No estimate on the horizon or assumption of maximality is used in this application. [A1, F1, F5, given]

1.2 In the horizon branch apply [F2] under its own complete supplied hypotheses and its horizon-field threshold. Its imported rigidity conclusion gives the stated Kerr exterior, and its separately recorded local estimate gives the confinement qualification. The inherited source statement, not a comparison between distinct smallness norms, supplies this conclusion. [A1, F2, F5, given]

1.3 In the nontrapping branch [F3] defines the actual orbit quotient and the correct maximal zero-energy curve class; its energy lemma makes the orthogonality test parameter-independent. With exactly GR, SBS and this NT predicate, the imported NT Theorem 1.1 applies and gives the nonextremal Kerr exterior. No conclusion about affine completeness, nonzero-energy trapping or a general coordinate boundedness condition is substituted. The source's zero-horizon-field case is retained. [A1, F3, F5, given]

2.1 In the ADM branch [F4] supplies the charge convention, original maximality and smooth boundary, $J<1$, and the fixed geometric bound and source-dependent angular threshold. These are exactly the hypotheses of the separately imported small-ADM theorem, hence it gives the subextremal Kerr exterior. The quantifier lemma records why the geometric bound and parameter gap cannot be discarded. All four implications therefore hold under their own displayed hypotheses, with global extension and classification supplied by their respective imported theorems rather than reconstructed here. [A1, F4, F5, step 1.1, step 1.2, step 1.3] ∎



Import AIK arXiv:0904.0982v1 Main Theorem under GR/SBS/PK with its quantitative constant, Radu arXiv:2609.23872v1 Theorem 1.1 under its GR/SBS/NT, and Radu arXiv:2610.09729v1 Theorem 1.1 under its GR/SBS/maximality, subextremal, mass-one and quantitative-smallness conditions. The three statement-bearing source records give their exact contracts and actual reading limits; these substantial global rigidity results are not claimed as locally reconstructed proofs. The fifteen intermediate prerequisite definitions and local lemmas above were fully authored before these residual theorem inputs were assembled. The horizon-field branch uses its existing exact supplier rather than a new import or an unfinished draft.



The original article on PDF p.3 reports Carleman estimates as the tool in the first smallness extensions and points to the difficulty of the required convexity conditions in general ergoregions, where $T$ is spacelike. This contextual description is preserved as attribution, not a new theorem proving failure of convexity or a claim that a particular Carleman condition follows from one of the four hypotheses. Source theorem proofs and their global classification steps were not independently reviewed.

## External input

Import AIK arXiv:0904.0982v1 Main Theorem under GR/SBS/PK with its quantitative constant, Radu arXiv:2609.23872v1 Theorem 1.1 under its GR/SBS/NT, and Radu arXiv:2610.09729v1 Theorem 1.1 under its GR/SBS/maximality, subextremal, mass-one and quantitative-smallness conditions. The three statement-bearing source records give their exact contracts and actual reading limits; these substantial global rigidity results are not claimed as locally reconstructed proofs. The fifteen intermediate prerequisite definitions and local lemmas above were fully authored before these residual theorem inputs were assembled. The horizon-field branch uses its existing exact supplier rather than a new import or an unfinished draft.

## Source notes

The original article on PDF p.3 reports Carleman estimates as the tool in the first smallness extensions and points to the difficulty of the required convexity conditions in general ergoregions, where $T$ is spacelike. This contextual description is preserved as attribution, not a new theorem proving failure of convexity or a claim that a particular Carleman condition follows from one of the four hypotheses. Source theorem proofs and their global classification steps were not independently reviewed.

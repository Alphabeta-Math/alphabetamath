---
id: pthm-uniform-horizon-maximal-graphs
title: "Lemma 3.4: uniform graph regularity at the bifurcation sphere"
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - def-stationary-maximal-graph
  - def-spacelike-maximal-hypersurface-data
  - def-normal-graph-and-mean-curvature-data
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - pthm-common-reference-collar
  - pthm-compact-height-bound
  - pthm-hawking-graph-height
  - pthm-hawking-graph-barriers
  - pthm-boundary-normal-angle
  - pthm-cutoff-angle-estimate
  - pthm-original-lapse-and-product
  - def-causal-exterior-and-boundary-data
  - math:def-axiom-of-choice
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  pthm-common-reference-collar: physical-result
  pthm-compact-height-bound: physical-result
  pthm-hawking-graph-height: physical-result
  pthm-hawking-graph-barriers: physical-result
  pthm-boundary-normal-angle: physical-result
  pthm-cutoff-angle-estimate: physical-result
  pthm-original-lapse-and-product: physical-result
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional geometric result for existing maximal sections in
  the smooth stationary vacuum and Harrison construction; it asserts neither
  their existence nor an observation.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 17–19, Lemma 3.4 and proof
      reading_limits: "Attribution only, not an imported premise. Historical claim
        description: For a fixed positive lower parameter bound, the maximal
        sections have uniformly bounded Hawking-flow graph heights near the
        bifurcation sphere and, on a smaller neighborhood, uniformly spacelike
        normal graphs with zero boundary values and uniform higher Hölder
        bounds. Historical scope: The article's stationary vacuum construction
        and existing maximal sections in the stated positive parameter interval.
        Retained reading record: Read the frozen article text at the cited
        passage. This citation attributes the article claim; the proof below
        uses the separately authored suppliers, not the article claim as a
        premise. This maintenance revision checks current supplier contracts; no
        new original-PDF reading is claimed."
dependency_level: 20
---

## Statement

Work in ZFC, including the Axiom of Choice. Adopt the regular mass-one stationary vacuum construction with $T|_S\not\equiv0$. Assume the actual original exterior section $C=\Sigma_0\cap\mathcal E$ is maximal for $g$, and use its closure $\Sigma_1=C\cup S$ as the reference section. The spherical identification and the physical stationary end chart remain independent. Use the same selected smooth single-primitive Harrison family $g_q$ and stationary product as in the compact-height contract.

Fix $\delta\in(0,1)$ and one supplied family of connected smooth spacelike maximal sections $\Sigma_q$, $q\in[\delta,1]$, smooth up to compact boundary $S$. Their interiors are stationary graphs $t=u_q(x)$ over $\Sigma_1^\circ$, and the family satisfies the complete candidate-section, normalized-end and uniform-estimate hypotheses of the compact-height result, including those of its radial height-decay and transformed-lapse inputs and positive stationary lapse. Fix the common end-estimate radii and constants for this family in these hypotheses; in particular, for any chosen decay exponent used by compact height, its normalized height bound holds beyond a common radius with a common constant. The normalized end height tends to zero at infinity for each fixed $q$.

Assume two-sided access to sufficiently far selected original ends: for some $R_a$ and every $R\ge R_a$, let $U_R=\mathbb R\times\{r>R\}$ in the selected physical stationary end chart and require $\mathcal E\subset I^-_{(\mathcal E,g)}(U_R)\cap I^+_{(\mathcal E,g)}(U_R)$. Both witnessing timelike paths lie in the unchanged original metric and exterior. This is the explicit access hypothesis of the compact-height supplier.

Let $V$ be the common reference collar and $K=T+\Omega_H Z$ its complete Hawking field on the collar saturation. There is a smaller common collar of $S$ in $\Sigma_1$ on which every $\Sigma_q$ is represented by the unique $K$-flow height $u_q^K$: for each interior base point $x$, $\phi^K_{u_q^K(x)}(x)\in\Sigma_q$. These heights extend smoothly to $S$ for each $q$ and obey a common bound $|u_q^K|\le C_\delta$.

After a further common shrinking, each candidate near $S$ is a one-to-one graph along future normal geodesics of $\Sigma_1$ for $g_q$, with graph height zero on $S$. The graphs are uniformly spacelike and their heights have uniform $C^{k,\alpha}$ bounds up to $S$ for every finite integer $k\ge0$ and $0<\alpha<1$. The collar and bounds may depend on $\delta$, the fixed background and the fixed supplied family through its common uniform-estimate data, including the end-estimate radii and constants; the Hölder bound may also depend on $k,\alpha$. They are independent of $q\in[\delta,1]$. No independence across families with unspecified uniform-estimate data is asserted.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-harrison-normalization]]

[[def-stationary-maximal-graph]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-normal-graph-and-mean-curvature-data]]

[[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

[[pthm-common-reference-collar]]

[[pthm-compact-height-bound]]

[[pthm-hawking-graph-height]]

[[pthm-hawking-graph-barriers]]

[[pthm-boundary-normal-angle]]

[[pthm-cutoff-angle-estimate]]

[[pthm-original-lapse-and-product]]

[[def-causal-exterior-and-boundary-data]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice. The model and regularity data supply the stationary construction and its compact bifurcation sphere $S$. Maximality is assumed on the actual original exterior section $C=\Sigma_0\cap\mathcal E$, and the reference section is $\Sigma_1=C\cup S$ as in the common-collar contract. Its spherical identification and the physical stationary end chart are independent. Use the selected mass-one Harrison family. A stationary graph is the image of $x\mapsto(u_q(x),x)$ in the stationary product; spacelike means its induced metric is positive definite, and maximal means its mean curvature vanishes. Retain the complete candidate and uniform end-estimate hypotheses with the fixed common radii and constants from the Statement. The two-sided original-metric selected-end access condition is a separate explicit Statement hypothesis, used directly rather than derived from the definition of the end. [[math:def-axiom-of-choice]] [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-harrison-normalization]] [[def-stationary-maximal-graph]] [[def-spacelike-maximal-hypersurface-data]] [[pthm-common-reference-collar]] [[pthm-compact-height-bound]] [[def-causal-exterior-and-boundary-data]]

[F1] The common-reference-collar result supplies the complete Hawking flow and timelike collar product. The Hawking-height result gives a unique smooth interior $K$-height and its individual smooth extension to $S$. The compact-height result, with actual original exterior maximality, explicit two-sided original-metric end access and the fixed candidate uniform-estimate data in [A1], bounds stationary heights uniformly in $q$ on each compact subset of the reference interior. With these same premises the Hawking-barrier result bounds the flow heights uniformly in $q$ on a smaller common collar, including $S$. Its constant inherits the dependence of the compact-height bound on the fixed family data. [[pthm-common-reference-collar]] [[pthm-hawking-graph-height]] [[pthm-compact-height-bound]] [[pthm-hawking-graph-barriers]]

[F2] The boundary-angle theorem applies to these height and barrier hypotheses. It supplies a common one-to-one normal graph collar, a uniform strict cone and smooth individual extension to $S$. The normal graph height is the normal-geodesic parameter over the reference section; since both sections have boundary $S$, its boundary value is zero. [[pthm-boundary-normal-angle]] [[def-normal-graph-and-mean-curvature-data]]

[F3] Under the same existing-section and boundary hypotheses, the cutoff-angle result gives uniform spacelikeness and uniform $C^{k,\alpha}$ bounds for the normal graph heights on a smaller common collar, including the boundary, for every finite $k$ and $0<\alpha<1$. The norms are the indicated Hölder norms. [[pthm-cutoff-angle-estimate]] [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

[F4] Under the assumed maximality of the actual original exterior section, the original lapse/product result supplies positive original lapse and the stationary-flow product over $C$. With $\Sigma_1=C\cup S$, its open base is precisely $\Sigma_1^\circ=C$. It requires no equality of the spherical identification with the physical end chart. The end-access condition remains the separate Statement premise. [[pthm-original-lapse-and-product]]

## Proof

**Given:** The construction and supplied family in the Statement.

**Goal:** Establish the uniform flow-height and normal-graph conclusions on common collars.

1.1 The actual original exterior maximality and reference-section binding in [A1] match the original stationary product in [F4] and the common-collar contract in [F1]. The selected single-primitive Harrison family, supplied smooth candidate sections, positive stationary lapse, normalized-end conditions and fixed uniform-estimate data are exactly those required by compact height. Its remaining access premise is the explicit two-sided original-metric selected-end condition in the Statement. Thus apply the compact-height result to this fixed family. Apply the Hawking-height result on the common reference collar to obtain the unique interior flow heights and their individual smooth extensions. The barrier result then supplies their bound on a smaller common collar, independent of $q$; this bound is allowed to depend on the fixed family data through compact height. [A1, F1, F4]

2.1 The height and barrier conclusions in step 1.1 meet the hypotheses of [F2]. Thus, on a further common collar, each candidate is a one-to-one normal graph satisfying the strict cone condition; its height vanishes on $S$. Apply [F3] on a smaller common collar to obtain the uniform spacelikeness and all stated boundary Hölder estimates. The supplied uniform flow-height bound fixes the boundary angle and strict cone used by [F2]–[F3]; all resulting collars and estimates are common to the fixed family and independent of $q$, with the data dependence stated above. [F2, F3, step 1.1] ∎

## Source notes

The article citation attributes Lemma 3.4 and its horizon graph conclusions; it supplies no prerequisite proof. This generated conditional formulation retains those conclusions for a fixed supplied family, makes actual physical exterior-section maximality and two-sided far-end access explicit, and records dependence on the supplied uniform-estimate data. The previous generated assertion of independence across all candidate families was not established by the compact-height/barrier contracts. This is a generated-draft repair, not a finding against the original author. The immutable original extraction and its coverage are unchanged, including original Theorem 1.1 and its unresolved source-assessment status. The argument is a local composition of the stated suppliers; it asserts no candidate existence.

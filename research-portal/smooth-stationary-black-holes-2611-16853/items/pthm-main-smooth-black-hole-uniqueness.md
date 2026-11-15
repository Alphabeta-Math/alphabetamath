---
id: pthm-main-smooth-black-hole-uniqueness
title: Conditional horizon recovery and Kerr implications
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-causal-exterior-and-boundary-data
  - def-spacelike-maximal-hypersurface-data
  - math:def-axiom-of-choice
  - pthm-original-lapse-and-product
  - lem-author-294e9b08725d-regular-positive-stationary-mass
  - def-harrison-normalization
  - lem-author-29145f41e94d-homothetic-stationary-geometry
  - lem-author-29145f41e94d-ernst-homothety
  - def-killing-ernst-notation
  - pthm-ernst-potential-existence
  - pthm-local-hawking-circle-fields
  - pthm-global-harrison-one-form
  - pthm-harrison-electrovacuum
  - pthm-recovery-ik-identities
  - math:thm-chain-rule-for-total-derivatives
  - def-author-9f9c6144aed8-ik-af
  - def-author-9f9c6144aed8-ik-sbs
  - def-author-9f9c6144aed8-ernst-mars-simon
  - pthm-ik-local-kerr-criterion-input
  - def-kerr-metric
  - pthm-author-d20d145f998f-aik-global-kerr-input
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  pthm-original-lapse-and-product: physical-result
  lem-author-294e9b08725d-regular-positive-stationary-mass: mathematical-premise
  def-harrison-normalization: mathematical-premise
  lem-author-29145f41e94d-homothetic-stationary-geometry: mathematical-premise
  lem-author-29145f41e94d-ernst-homothety: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  pthm-ernst-potential-existence: physical-result
  pthm-local-hawking-circle-fields: physical-result
  pthm-global-harrison-one-form: physical-result
  pthm-harrison-electrovacuum: physical-result
  pthm-recovery-ik-identities: physical-result
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  def-author-9f9c6144aed8-ik-af: mathematical-premise
  def-author-9f9c6144aed8-ik-sbs: mathematical-premise
  def-author-9f9c6144aed8-ernst-mars-simon: mathematical-premise
  pthm-ik-local-kerr-criterion-input: physical-result
  def-kerr-metric: mathematical-premise
  pthm-author-d20d145f998f-aik-global-kerr-input: physical-result
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional smooth stationary vacuum geometry with actual
  physical exterior-section maximality and two-sided access to every
  sufficiently far selected end stated explicitly. Horizon identities and the
  exact IK local conclusion are retained; a full global Kerr DOC isometry
  additionally requires the complete source-native AIK GR/SBS/PK package.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 1,2,4,7,29; Abstract; Main Theorem (rough version); Theorem
        1.1; §1.4; §5 conclusion
      reading_limits: Original-article attribution only. This revision verified the
        frozen PDF and text checksums, read the extracted Definition 1.1 and
        Theorem 1.1 on PDF pp.3–4, and inspected the p.4 image. The immutable
        original extraction is retained. This conditional formulation does not
        establish the stronger original claim. The article supplies no proof
        premise.
dependency_level: 40
---

## Statement

Work in ZFC in the smooth connected oriented, time-oriented, paracompact, boundaryless stationary vacuum model. Let the data satisfy the regular non-degenerate stationary-vacuum conditions, with designated physical end $M^{\mathrm{end}}$, stationary field $T$, bifurcation sphere $S$, and $T|_S\not\equiv0$. Let $j:\Sigma_0\to\{y\in\mathbb R^3:|y|>1/2\}$ be the specified hypersurface identification with $j(S)=\{|y|=1\}$. Retain the original assumption that the specified portion $\{|j|\ge1\}$ is maximal. Separately write $C=\Sigma_0\cap E$ for the actual physical exterior section, where $E=I^-_M(M^{\mathrm{end}})\cap I^+_M(M^{\mathrm{end}})$, and impose these additional hypotheses:

(A) The actual section $C$ is maximal. No identification of $C$ with a side of $j$ follows merely from its radial label.

(B) For some sufficiently large $R_*$ and every $R\ge R_*$, the stationary tail $U_R=\{(t,x)\in M^{\mathrm{end}}:|x|>R\}$ lies in $E$, the field $T$ is uniformly future timelike there, and every $p\in E$ has two-sided timelike access within $E$ to $U_R$: there exist $u_-,u_+\in U_R$ and future timelike curves in $E$ from $u_-$ to $p$ and from $p$ to $u_+$. These access conditions are explicit assumptions for every sufficiently far selected tail. The physical coordinates $x$ and the topological coordinates $j$ are independent.

Let $m$ be the coefficient in $g_{00}=-1+2m/|x|+O_6(|x|^{-2})$ on the physical end. Use the normalized Ernst potential $\sigma\to1$ there, $F_{ab}=\nabla_aT_b$, and $\mathcal F=F+i\star_gF$, with complex bilinear contraction and both indices raised by $g$. Then $m>0$ and

$$-4m^2\mathcal F_{ab}\mathcal F^{ab}=(1-\sigma)^4\quad\text{on }S,$$

and $\operatorname{Re}((1-\sigma(p))^{-1})>1/2$ at a common pole $p\in S$ of the local Hawking and circle fields used in recovery. The exact IK AF/SBS criterion consequently gives its local conclusion: every point of $E$ has a neighborhood isometric to an open subset of a Kerr exterior of mass $m$ and $0<a<m$.

There is a separate global implication. Suppose the unchanged physical $(E,g|_E,T,\sigma,S)$ admits a realization as the DOC of smooth vacuum ambient/section/end data satisfying every source-native GR, SBS and PK hypothesis of the independent AIK global criterion, with source mass $M_0=m$ and source angular momentum magnitude $0<J<m^2$. Require the realization to identify its DOC metric, orientation, time orientation, stationary field, normalized potential and bifurcation sphere with these original data. Then $E$ is globally isometric to the full Kerr DOC of mass $m$ and angular momentum magnitude $J$, with $a=J/m$. A realization here supplies the source's geometric, asymptotic, section and tensor-bound hypotheses; it does not presume any Kerr isometry. The local Kerr conclusion is not asserted to construct it. No analyticity or perturbative hypothesis is added to horizon recovery or the local implication; the separate global implication retains the actual source PK requirement.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-causal-exterior-and-boundary-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[math:def-axiom-of-choice]]

[[pthm-original-lapse-and-product]]

[[lem-author-294e9b08725d-regular-positive-stationary-mass]]

[[def-harrison-normalization]]

[[lem-author-29145f41e94d-homothetic-stationary-geometry]]

[[lem-author-29145f41e94d-ernst-homothety]]

[[def-killing-ernst-notation]]

[[pthm-ernst-potential-existence]]

[[pthm-local-hawking-circle-fields]]

[[pthm-global-harrison-one-form]]

[[pthm-harrison-electrovacuum]]

[[pthm-recovery-ik-identities]]

[[math:thm-chain-rule-for-total-derivatives]]

[[def-author-9f9c6144aed8-ik-af]]

[[def-author-9f9c6144aed8-ik-sbs]]

[[def-author-9f9c6144aed8-ernst-mars-simon]]

[[pthm-ik-local-kerr-criterion-input]]

[[def-kerr-metric]]

[[pthm-author-d20d145f998f-aik-global-kerr-input]]

## Facts & Assumptions

[A1] Adopt the stationary vacuum model, the regularity and causal conventions, the original specified-side maximality, and the additional actual-section and far-tail hypotheses (A)–(B). Work in ZFC. The two section coordinate systems are not assumed to agree. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-causal-exterior-and-boundary-data]] [[def-spacelike-maximal-hypersurface-data]] [[math:def-axiom-of-choice]]

[F1] The original exterior theorem supplies the actual $C$, its smooth closure $C\cup S$, compact physical truncations, and an adapted topological identification placing $C$ outside its unit sphere without matching the physical end chart. Conditional on maximality of this actual $C$, it gives $0<N<1$, $N|_S=0$, $\Delta_hN=|k|_h^2N$ and the stationary-flow diffeomorphism $\mathbb R\times C\to E$. [[pthm-original-lapse-and-product]]

[F2] For the same regular stationary-vacuum data, the original physical-end mass coefficient equals the ADM energy of the original complete exterior section and is positive. This supplier does not require a topological chart agreeing with the physical coordinates. The ADM surface-integral convention is the one used by Harrison normalization. [[lem-author-294e9b08725d-regular-positive-stationary-mass]] [[def-harrison-normalization]]

[F3] A constant homothety $\widehat g=m^{-2}g$, $\widehat T=mT$ preserves vacuum, causal sets, complete stationary orbit images, Cauchy sets, bifurcation geometry and maximality of the unchanged section. The same normalized Ernst potential can be used, and $\widehat{\mathcal F}^{\,2}=m^2\mathcal F^2$. The orientation and complex contraction conventions are fixed throughout. [[lem-author-29145f41e94d-homothetic-stationary-geometry]] [[lem-author-29145f41e94d-ernst-homothety]] [[def-killing-ernst-notation]]

[F4] The regular vacuum hypotheses supply the normalized potential on $E$ and a neighborhood of $S$, and the local commuting Hawking/circle fields with their common pole and positive outward boost. On regular mass-one data with the actual original exterior section maximal, the global one-form theorem supplies one smooth stationary primitive, its invariant horizon gauge and spatial $O_5$ decay on the unchanged physical end. The electrovacuum theorem supplies the corresponding single regular Harrison family for that same primitive and pole. No exact radial-integral equality is inferred for its spatial coefficients. [[pthm-ernst-potential-existence]] [[pthm-local-hawking-circle-fields]] [[pthm-global-harrison-one-form]] [[pthm-harrison-electrovacuum]]

[F5] For the regular mass-one construction with original exterior section maximal and nontrivial $T|_S$, the recovery theorem gives $-4\mathcal F^2=(1-\sigma)^4$ on all of $S$ and the strict reciprocal inequality at its common recovery pole, for its one supplied family and pole. [[pthm-recovery-ik-identities]]

[F6] The total chain rule applies to smooth coordinate rescalings and their component derivatives. [[math:thm-chain-rule-for-total-derivatives]]

[F7] The exact IK AF/SBS and Ernst interfaces require the smooth vacuum spacetime, its positive-mass stationary end, a spacelike section diffeomorphic to $\{|y|>1/2\}$ and equal to $t=0$ on that end, complete stationary orbits meeting it, nonzero lapse on its intersection with $E$, the specified smooth transverse nonexpanding bifurcate horizon, and the same potential normalized on that AF end. Under these hypotheses and the two sphere conditions, the imported criterion gives local Kerr isometries, with mass $m$ and $0<a<m$. It does not supply one global DOC isometry. [[def-author-9f9c6144aed8-ik-af]] [[def-author-9f9c6144aed8-ik-sbs]] [[def-author-9f9c6144aed8-ernst-mars-simon]] [[pthm-ik-local-kerr-criterion-input]] [[def-kerr-metric]]

[F8] The independent AIK global criterion requires its complete GR/SBS/PK package. In particular GR includes the compatible global section/end chart, achronal edgeless partial Cauchy section, specified $O_6$ spin expansion, positive mass and subextremal spin, global hyperbolicity of its DOC, both separate chronological-section equalities, and complete nonvanishing stationary orbits meeting the section. SBS uses the actual source end-boundaries and tangency/nontriviality of $T$. PK uses the same source-normalized potential and its weighted Mars–Simon contraction bound below the source threshold depending on the finite regularity constant. Under precisely that full package it gives one isometry onto the full Kerr DOC. Every clause is assumed for the realization in the final implication, rather than inferred from local charts. [[pthm-author-d20d145f998f-aik-global-kerr-input]] [[def-kerr-metric]]

## Proof

**Given:** The complete conditional hypotheses in the Statement; the source-native realization is assumed only for the global implication.

**Goal:** Recover the original-scale horizon identities, match the exact local criterion, and establish the separately conditioned global implication.

1.1 Apply [F1] using (A) to the actual $C=\Sigma_0\cap E$. It gives the positive original lapse and stationary product on this geometric section, its compact physical truncations and its adapted topological chart. It does not identify the original specified side of $j$ with $C$. For each selected $U_R$ in (B), two-sided access gives $E\subset I^-_M(U_R)\cap I^+_M(U_R)$. Conversely $U_R\subset M^{\mathrm{end}}$ implies $I^-_M(U_R)\cap I^+_M(U_R)\subset E$ by the defining chronological relations. Thus each such tail has the same actual DOC. This argument does not assert the separate ambient chronological sets or their boundaries are equal. [given, A1, F1]

1.2 Apply [F2] under the regular stationary-vacuum hypotheses in [A1]. It supplies an existing ADM limit on this original physical end, equal to its coefficient $m>0$. By [F4] take the normalized potential on $E$ and a neighborhood of $S$, with the fixed orientation and contraction convention. No change of the original section or identification of independent charts is used. [A1, F2, F4]

2.1 Set $\widehat g=m^{-2}g$ and $\widehat T=mT$. On the same physical end use $\widehat t=t/m$, $\widehat x=x/m$ and $\widehat r=|\widehat x|$. Both coordinate differentials acquire a factor $m$, so the components of $\widehat g$ in this chart equal the original component functions evaluated at $x=m\widehat x$. The chain rule in [F6] gives $\widehat g_{00}=-1+2/\widehat r+O_6(\widehat r^{-2})$, $\widehat g_{0i}=O_6(\widehat r^{-2})$ and $\widehat g_{ij}=\delta_{ij}+O_6(\widehat r^{-1})$, and $\widehat T=\partial_{\widehat t}$. By [F3], all regular causal and stationary-orbit conditions, the same sphere and nonexpanding branches, nontriviality on $S$, and maximality of the actual original section are preserved. The original topological identification is kept separately; it is not rescaled into the physical coordinates. Access hypothesis (B) is preserved because homothety does not change timelike curves and a hatted physical tail is an original tail of radius multiplied by $m$. [A1, F3, F6, step 1.1, step 1.2, algebra]

2.2 Match the section and potential domains for the local input without a chart-agreement assumption. Use the adapted topological identification from [F1], writing its radius as $s$, with $C=\{s>1\}$ and $S=\{s=1\}$. The potential neighborhood in [F4] contains a full inner collar $1-\eta<s\le1$ of compact $S$ for some $0<\eta<1/2$. Restrict the original section to $\Sigma_{\mathrm{AF}}=\{s>1-\eta\}$, so it consists of $C$, $S$ and that inner collar and lies in the open potential domain $E\cup O$. It is an embedded spacelike hypersurface without manifold boundary. If $y$ is the adapted topological chart, the radial map $y\mapsto (\tfrac12+(s-1+\eta)/(2\eta))y/s$ identifies this restricted section smoothly with $\{|z|>1/2\}$ and sends $S$ to $|z|=1$. It does not claim agreement with $x$ on the physical end. The hypersurface itself still agrees with physical $t=0$ there, its intersection with $E$ is exactly $C$, and every complete stationary orbit in $E$ meets it at its point on $C$. Its lapse on that intersection is positive by step 1.1. Thus the section, transversality and normalized-potential-domain requirements of the exact AF/SBS interfaces in [F7] are met. [A1, F1, F4, F7, step 1.1]

3.1 Let $h_{ij}$ denote the original section metric in physical end coordinates. The same section has hatted coordinate components $\widehat h_{ij}(\widehat x)=h_{ij}(m\widehat x)$. In the ADM integral of [F2], differentiation contributes $m$, the Euclidean sphere area contributes $m^{-2}$ relative to the original sphere of radius $m\widehat R$, and the radial unit vector is unchanged. Therefore its hatted ADM limit is $m^{-1}$ times the original limit $m$, hence one. This proves the exact mass-one hypothesis on the unchanged maximal section using only a linear rescaling of its physical chart. It invokes neither a compatible global auxiliary chart nor an end-normalized replacement time slice. [F2, F3, F6, step 1.2, step 2.1, algebra]

4.1 The hatted data now satisfy the full regular mass-one, actual-original-section maximality and nontriviality hypotheses of [F4]–[F5]. Apply the local-field and global one-form results to choose their common pole and one invariant smooth primitive, and use that same choice in the regular electrovacuum construction. The original normalized potential remains the hatted normalized potential by [F3]. These are exactly the one-family and pole inputs of [F5]; invoke recovery to obtain $-4\widehat{\mathcal F}^{\,2}=(1-\sigma)^4$ on $S$ and the strict reciprocal inequality at that pole. Only the supplied smooth decaying primitive is used, with no assertion that it equals an exact radial integral. [F3, F4, F5, step 2.1, step 3.1]

5.1 By [F3], $\widehat{\mathcal F}^{\,2}=m^2\mathcal F^2$ and the normalized scalar is the same $\sigma$. The common zero of $\widehat T$ and the selected circle field is also a zero of $T$, since $\widehat T=mT$ with $m>0$. Substitute the contraction scaling in step 4.1 to get the asserted original-scale identity and unchanged strict reciprocal inequality at the same pole. [F3, step 4.1, algebra]

6.1 The original $O_6$ metric bounds imply the AF interface's undifferentiated end bounds with the positive mass from step 1.2; $T=\partial_t$ and all required orbit conditions hold by regularity and step 2.2. The ambient DOC, its bifurcation sphere and its smooth transverse nonexpanding end-boundaries were not changed. Tangency and $T|_S\not\equiv0$ give the remaining SBS requirements. The potential is normalized to $1$ on this same physical $t=0$ end, with the contraction convention in [F7]. Step 5.1 supplies both technical sphere conditions. Apply the exact imported local criterion: every point of $E$ has the stated local isometry into a Kerr exterior with mass $m$ and $0<a<m$. No global bijection is inferred from these local charts. [A1, F7, step 1.2, step 5.1, step 2.2]

7.1 For the separate global implication, assume precisely the source-native realization specified in the Statement. Its identified DOC is the unchanged physical $E$, and all GR, SBS and PK predicates in [F8], including the source mass, spin, partial-Cauchy, separate chronological-section, regularity and tensor-bound conditions, are supplied for that realization. Apply [F8] to obtain its single isometry onto the full Kerr DOC of mass $m$ and angular momentum magnitude $J$. Composing with the stipulated identification of its DOC with the original $E$ gives the asserted global isometry and $a=J/m$. These hypotheses contain no Kerr isometry premise, and step 6.1 has not been used to manufacture missing global hypotheses. This proves the conditional endpoint at its stated scopes. [given, F8, step 6.1] ∎

## Source notes

This is the expressly authorized conditional replacement for the generated endpoint. The immutable original extraction and the original PDF are not edited. The original Theorem 1.1, PDF p.4, asserts the sphere identities and full subextremal Kerr identification from its regularity conditions and maximality of the specified radial side. That stronger original claim remains recorded with its original hypotheses and unresolved status; this conditional item is not a proof of it. The original abstract, rough theorem and later recovery passages remain attribution to that stronger claim. Under the literal independent-chart/end contract, the implication from specified-side maximality to maximality of the actual physical exterior, the selected-far-tail access bridge, and unconditional matching to a global-isometry theorem are not declared established here. This qualification is not an original-author defect finding or a counterexample to the original horizon identities or Kerr conclusion.

Hypotheses (A)–(B) are explicit additions. ADM matching uses the existing physical-section mass theorem and a local linear homothety, avoiding the auxiliary global-chart hypothesis in the outside proposal. The local criterion is applied with its exact AF/SBS scope; its section is a restriction of the original hypersurface and no independent spatial charts are equated. The global clause requires every source-native hypothesis of the separate global theorem. Neither imported theorem is strengthened in this item, and no source proof, independent acceptance or queued rejudgment is replaced by this proposal.

---
id: lem-author-294e9b08725d-canonical-double-stationary-realization
title: Vacuum development realizing the exterior and local boost germs
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-294e9b08725d-canonical-outer-cauchy-splice
  - thm-author-294e9b08725d-radu-local-bifurcate-collar-input
  - lem-author-294e9b08725d-exact-boost-reflection-jets
  - lem-author-294e9b08725d-canonical-section-reflection-parities
  - lem-author-294e9b08725d-smooth-vacuum-data-double
  - lem-author-294e9b08725d-stationary-vacuum-kid-double
  - lem-author-294e9b08725d-complete-asymptotically-flat-double
  - thm-author-294e9b08725d-vacuum-double-development-input
  - def-regular-stationary-vacuum-spacetime
  - def-causal-exterior-and-boundary-data
  - def-spacelike-maximal-hypersurface-data
  - lem-author-a4a441da4986-working-partial-cauchy-collar
  - lem-author-294e9b08725d-regular-positive-stationary-mass
  - math:def-axiom-of-choice
  - physics:thm-gr-constraint-equations-in-normal-frame
  - lem-author-294e9b08725d-stationary-end-extrinsic-decay
  - lem-author-a4a441da4986-exact-outer-cauchy-section
  - lem-author-ca4ffba327b3-compact-normal-exponential-tube
  - lem-killing-normal-boost-and-invariant-tensors
  - physics:lem-gr-isometric-immersion-rigidity
  - physics:thm-gr-local-geodesics-and-exponential-map
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:thm-fundamental-theorem-on-flows
dependency_roles:
  lem-author-294e9b08725d-canonical-outer-cauchy-splice: mathematical-premise
  thm-author-294e9b08725d-radu-local-bifurcate-collar-input: mathematical-premise
  lem-author-294e9b08725d-exact-boost-reflection-jets: mathematical-premise
  lem-author-294e9b08725d-canonical-section-reflection-parities: mathematical-premise
  lem-author-294e9b08725d-smooth-vacuum-data-double: mathematical-premise
  lem-author-294e9b08725d-stationary-vacuum-kid-double: mathematical-premise
  lem-author-294e9b08725d-complete-asymptotically-flat-double: mathematical-premise
  thm-author-294e9b08725d-vacuum-double-development-input: mathematical-premise
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  lem-author-a4a441da4986-working-partial-cauchy-collar: mathematical-premise
  lem-author-294e9b08725d-regular-positive-stationary-mass: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  physics:thm-gr-constraint-equations-in-normal-frame: mathematical-premise
  lem-author-294e9b08725d-stationary-end-extrinsic-decay: mathematical-premise
  lem-author-a4a441da4986-exact-outer-cauchy-section: mathematical-premise
  lem-author-ca4ffba327b3-compact-normal-exponential-tube: mathematical-premise
  lem-killing-normal-boost-and-invariant-tensors: mathematical-premise
  physics:lem-gr-isometric-immersion-rigidity: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references:
    - title: Robert Beig and Piotr T. Chruściel, Killing Initial Data
      url: https://arxiv.org/pdf/gr-qc/9604040v1
      locator: "Section 2, printed pp. 4–6 (PDF pages 4–6): (2.6)–(2.8), (2.13),
        vacuum Case 2 on p. 5 and (2.15) with the vacuum discussion on p. 6."
      statement: A smooth vacuum KID extends in a vacuum Cauchy development, with no
        nonzero-lapse requirement. Multiple vacuum KIDs extend in the same
        development; their spacetime commutator induces (2.15). In Gaussian
        coordinates its normal derivatives obey (2.7)–(2.8).
      hypotheses: Smooth three-dimensional vacuum constraint data and pairs satisfying
        (2.6), (2.13) with rho=J=tau_ij=0; the initial manifold can be an open
        collar. K=g(nabla n, dot), partial_t h=2K. No completeness or asymptotic
        hypothesis is used for this local application.
      reading_limits: Read the extracted PDF text of Section 2 through its vacuum
        bracket discussion, including the displayed equations and Case 2.
        Screenshot retrieval failed. These stated extension and bracket facts
        are imported, without reconstructing the hyperbolic proof or the
        references cited there. The reflection and application to the signed
        collar are proved locally below.
    - title: Piotr T. Chruściel, On completeness of orbits of Killing vector fields
      url: https://arxiv.org/pdf/gr-qc/9304029v1
      locator: Introduction, printed p. 2; Proposition 2.4 and its proof, printed p.
        10 (PDF page 10).
      statement: For an achronal spacelike submanifold A of a maximal globally
        hyperbolic vacuum spacetime, its domain of dependence is the MGHD of its
        induced data. The proof supplies a data-fixing local isometry near the
        initial surface by local vacuum Cauchy uniqueness.
      hypotheses: Smooth vacuum MGHD and an achronal spacelike initial submanifold
        with its induced metric and second fundamental form. Apply to the open
        signed collar A and to the open positive section C_0 of the doubled
        Cauchy surface, not to a hypersurface with boundary.
      reading_limits: Read the extracted PDF introduction and Section 2, including
        Proposition 2.4 statement and proof. Screenshot retrieval failed. Import
        Cauchy uniqueness and the open-submanifold identification; no
        reconstruction of the Einstein evolution proof or new completeness
        theorem is claimed. Global completeness is used only through the
        existing development supplier.
proof_strategy: direct
dependency_level: 12
---

## Statement

Work in ZFC, including the Axiom of Choice. Let $(M,g,T,M^{\mathrm{end}},\Sigma_0,S,\mathcal H^+,\mathcal H^-)$ satisfy all four conditions of the regular non-degenerate stationary vacuum definition, with its specified end chart, differentiated decay and section topology. In particular, $g$ is a smooth time-oriented Ricci-flat Lorentzian metric of signature $(-,+,+,+)$, $T$ is Killing, $E=I_M^-(M^{\mathrm{end}})\cap I_M^+(M^{\mathrm{end}})$ is globally hyperbolic, its $T$-orbits are complete and meet $C=\Sigma_0\cap E$, and $C$ is Cauchy in $E$. The compact sphere $S\subset\Sigma_0$ is the transverse intersection of the two smooth nonexpanding null horizon sheets, both tangent to $T$.

Use the supplied working partial-Cauchy data and the GR/SBS local boost collar: $M'\subset M$ contains $E$ and a neighborhood of $S$, has the same selected end and exterior $E$, and carries a smooth spacelike acausal edgeless section $\Sigma'\cong\{r>1/2\}$ agreeing with $C$ on its outer side and with $\Sigma_0$ near $S$, with $\Sigma'\cap I^+_{M'}(M^{\mathrm{end}})=\Sigma'\cap I^-_{M'}(M^{\mathrm{end}})=C$. The stationary ADM mass is the end coefficient $M_0>0$ supplied by the positive-mass lemma. The local collar is taken under the full GR/SBS hypotheses of its supplier; no nontrapping or global axisymmetry hypothesis is imposed.

Let $C_0$ be the canonical splice supplied for these data: it is a smooth spacelike Cauchy section of $E$, its closure $\overline C_0=C_0\cup S$ is complete with compact boundary included, it agrees with $C$ on the stationary end, and near $S$ it is the outward canonical section $U=V=r>0$. In the supplied double-normal collar $K=\kappa(V\partial_V-U\partial_U)$ is Killing, $K|_S=0$, and $\kappa>0$ is constant. In rotation there is a commuting local circle field $Z$ of period $2\pi$ preserving $U,V$, with $K=T+\Omega Z$ and constant $\Omega$; in the nonrotating case $K=T$, $\Omega=0$, and $Z$ is omitted. In particular $[K,T]=0$.

Use the future unit normal $n$ and induced data $h=g|_{\overline C_0}$, $\mathcal K(v,w)=g(\nabla_v n,w)=-k(v,w)$, $N=-g(T,n)$ and $X=T-Nn$. The reflected double $\widehat C=C_+\cup_S C_-$ means the smooth double with the signed collar induced by $r$: on the negative copy reflect $h$ and $X$, and take minus the reflected $\mathcal K$ and $N$. These are the data and sign conventions of the smooth-data and stationary-KID suppliers.

For these data, the reflected double admits a smooth globally hyperbolic vacuum development $\widehat M$ with complete stationary field $\widehat T$. The original exterior $E$ embeds isometrically and equivariantly in $\widehat M$, and the embedding of $C_0$ extends across $S$ as the doubled Cauchy hypersurface. A neighborhood of $S$ in $\widehat M$ has local fields $K=\kappa(V\partial_V-U\partial_U)$ and, in rotation, $Z$ of period $2\pi$, with $\widehat T=K-\Omega Z$. This conclusion does not identify $E$ with a domain of dependence in the entire $\widehat M$.

## Statement references

[[lem-author-294e9b08725d-canonical-outer-cauchy-splice]]

[[thm-author-294e9b08725d-radu-local-bifurcate-collar-input]]

[[lem-author-294e9b08725d-exact-boost-reflection-jets]]

[[lem-author-294e9b08725d-canonical-section-reflection-parities]]

[[lem-author-294e9b08725d-smooth-vacuum-data-double]]

[[lem-author-294e9b08725d-stationary-vacuum-kid-double]]

[[lem-author-294e9b08725d-complete-asymptotically-flat-double]]

[[thm-author-294e9b08725d-vacuum-double-development-input]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-causal-exterior-and-boundary-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[lem-author-a4a441da4986-working-partial-cauchy-collar]]

[[lem-author-294e9b08725d-regular-positive-stationary-mass]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

**Given:** The regular stationary-vacuum data, working partial section, supplied GR/SBS collar, canonical splice and reflected initial data specified in the Statement, in ZFC.

**Goal:** Realize the full exterior and the local boost germs in the same complete stationary vacuum development, with exactly the stated scope.

[F1] The canonical Cauchy splice agrees with the original stationary end and the exact boost section near its boundary; its compactly supported isotopy preserves the compact radial truncations of the original outer closure. [[lem-author-294e9b08725d-canonical-outer-cauchy-splice]] [[lem-author-a4a441da4986-exact-outer-cauchy-section]] [[thm-author-294e9b08725d-radu-local-bifurcate-collar-input]]

[F2] Under their respective hypotheses, the all-jet parity and reflection arguments give smooth vacuum data, a smooth stationary KID, and a complete two-ended double with the required differentiated decay. [[lem-author-294e9b08725d-exact-boost-reflection-jets]] [[lem-author-294e9b08725d-canonical-section-reflection-parities]] [[lem-author-294e9b08725d-smooth-vacuum-data-double]] [[lem-author-294e9b08725d-stationary-vacuum-kid-double]] [[lem-author-294e9b08725d-complete-asymptotically-flat-double]]

[F3] For smooth vacuum data on the complete asymptotically flat double, the global stationary KID extends to a Killing field on its MGHD with complete orbits, and a development of open initial data embeds there. [[thm-author-294e9b08725d-vacuum-double-development-input]]

[F4] The regular-spacetime definition fixes the vacuum, end, horizon and stationary-flow hypotheses; the causal and hypersurface definitions fix the chronological exterior, Cauchy property, boundary completeness, unit normal and lapse–shift conventions. [[def-regular-stationary-vacuum-spacetime]] [[def-causal-exterior-and-boundary-data]] [[def-spacelike-maximal-hypersurface-data]]

[F5] The working-partial-Cauchy supplier provides $(M',\Sigma')$ with the two displayed chronological end intersections and the original exterior and horizon germs. The positive-mass supplier gives $M_0=m_K=E_{\rm ADM}>0$. These are the partial-section and mass inputs for the stated GR/SBS local-collar application. [[lem-author-a4a441da4986-working-partial-cauchy-collar]] [[lem-author-294e9b08725d-regular-positive-stationary-mass]] [[thm-author-294e9b08725d-radu-local-bifurcate-collar-input]]

[F6] With $\mathcal K=g(\nabla n,\cdot)$, the normal projections are $2G(n,n)=R_h+(\operatorname{tr}_h\mathcal K)^2-|\mathcal K|_h^2$ and $G(n,\cdot)=\operatorname{div}_h\mathcal K-d\operatorname{tr}_h\mathcal K$. Thus Ricci flatness gives both vacuum constraints on the positive section. [[physics:thm-gr-constraint-equations-in-normal-frame]]

[F7] On the original stationary $t=0$ end, $h-\delta=O_6(r^{-1})$, $k=O_5(r^{-3})$ and $N=1+O_6(r^{-1})$; hence $\mathcal K=-k$ has the same decay. [[lem-author-294e9b08725d-stationary-end-extrinsic-decay]] [[def-regular-stationary-vacuum-spacetime]]

[F8] The local vacuum KID-extension, Gaussian derivative and bracket premises are imported in External input. They will be applied on an open signed collar, with its own Cauchy development, without requiring the local boost or rotation KIDs on the entire double.

[F9] Isometric immersions from a connected Lorentzian four-manifold into a Lorentzian four-manifold agreeing in value and differential at one point agree everywhere. The proof's connection identity also shows that local isometries commute with the exponential map wherever the corresponding geodesics exist. A compact spacelike surface with the supplied future/outward orthonormal normal frame has a uniform embedded normal exponential tube. The fixed-surface boost lemma gives the differential of a local Killing flow from its normal boost derivative. The inverse function theorem supplies the local inverses of the Gaussian normal maps, and the flow theorem supplies smooth local flows and uniqueness of integral curves. [[math:thm-smooth-inverse-function-theorem-on-manifolds]] [[math:thm-fundamental-theorem-on-flows]] [[physics:lem-gr-isometric-immersion-rigidity]] [[physics:thm-gr-local-geodesics-and-exponential-map]] [[lem-author-ca4ffba327b3-compact-normal-exponential-tube]] [[lem-killing-normal-boost-and-invariant-tensors]]

[A1] The Axiom of Choice is retained for the global smooth-double construction and its smooth geometric interfaces; no choice-free version of those suppliers is asserted. [[math:def-axiom-of-choice]] [[lem-author-294e9b08725d-smooth-vacuum-data-double]]

## External input

For F8 import vacuum KID extension and the induced commutator bracket from [Beig–Chruściel, §2, vacuum Case 2 and (2.15)](https://arxiv.org/pdf/gr-qc/9604040v1). Equations (2.7)–(2.8) determine the normal derivatives from a KID in Gaussian coordinates. Apply these facts to the open three-manifold $A=(-\epsilon,\epsilon)\times S$ with the doubled vacuum data, rather than extending its local KIDs to all of $\widehat C$.

Import [Chruściel, Proposition 2.4 and its local-uniqueness step](https://arxiv.org/pdf/gr-qc/9304029v1) to identify the MGHD of those open data with $D_{\widehat M}(A)$, an open neighborhood of $S$, and to compare positive-side developments. The exact hypotheses and reading limits are recorded in the two source contracts. These are imported premises of the local argument; the present lemma is a locally proved composition.

## Proof

1.1 Apply F5 and F4 to meet the full GR/SBS hypotheses, and use F1 to obtain $C_0$. Its induced data are smooth through the compact boundary and $g$ is Ricci-flat on an actual neighborhood. F6 gives $R_h+(\operatorname{tr}_h\mathcal K)^2-|\mathcal K|_h^2=0$ and $\operatorname{div}_h\mathcal K-d\operatorname{tr}_h\mathcal K=0$ on the positive section, including the boundary by continuity. This checks the constraint hypothesis before applying the data-double supplier. The normal and sign conventions are precisely those in F4 and F6. [given, F1, F4, F5, F6]

2.1 On the unchanged stationary end, F7 gives $h-\delta=O_6(r^{-1})$ and $\mathcal K=O_5(r^{-3})$. The compact radial truncations of F1 are carried to compact truncations of $\overline C_0$ by the compactly supported isotopy, which is the identity sufficiently far out; they exhaust it and have boundaries $S$ and the large coordinate spheres. Completeness with boundary included is supplied by F1. The ambient $T$ is Killing on the whole positive section and commutes with the local boost. Consequently every hypothesis of all the reflection and complete-double constructions in F2 is met. Use their signed collar and the retained Choice convention to obtain smooth complete boundaryless two-ended vacuum data and the global stationary KID. [F1, F2, F4, F7, A1, step 1.1]

3.1 Apply F3 to this full doubled data set to obtain its vacuum MGHD $(\widehat M,\widehat g)$ and the complete Killing field $\widehat T$. The original $E$ is a smooth globally hyperbolic vacuum development with Cauchy surface $C_0$, which is an open submanifold of $\widehat C$. The open-data embedding in F3 therefore gives a time-orientation-preserving isometric embedding $i:E\to\widehat M$ fixing those data. [F1, F3, F4, step 2.1]

4.1 We record the uniqueness needed below. For a Killing field vanishing along an open spacelike hypersurface, its Gaussian components $(N,Y)$ and their spatial derivatives vanish there. Equations (2.7)–(2.8) in F8 then give zero normal derivatives as well. At any point its local flow therefore fixes the point with identity differential; rigidity in F9 makes that flow the identity on the connected common domain. Differentiating in the flow parameter makes the field zero there. The same rigidity continues equality across overlapping connected coordinate neighborhoods. In particular equal KIDs give equal Killing fields: their difference vanishes along the initial surface. Apply this to $i_*T$ and $\widehat T$ on the connected embedded exterior, which have the same KID. Uniqueness of integral curves and completeness of both stationary fields give $i\circ\Phi_t^T=\Phi_t^{\widehat T}\circ i$ for every finite $t$. [F2, F3, F4, F8, F9, step 3.1, algebra]

4.2 Restrict the doubled data to the open signed collar $A=(-\epsilon,\epsilon)\times S$. On its positive side take the KIDs induced by the actual local Killing fields $K$ and, in rotation, $Z$. They commute with the boost; their all-jet parities are therefore exactly those used in F2, with each field substituted for $T$. The componentwise smooth-pasting and sign calculation of the stationary-KID supplier is local, so it gives smooth vacuum KIDs on $A$. Their linear relation with the restriction of the stationary KID is preserved by reflection and continuity. The imported F8 applies to these smooth vacuum KIDs on $A$, with no completeness or nonzero-lapse requirement. It develops them in the same local vacuum development. Proposition 2.4 identifies that development with $D_{\widehat M}(A)$ near $S$, since $A$ is an open subset of the doubled Cauchy surface and hence achronal and spacelike. They are not being treated as global KIDs of $\widehat C$. [F1, F2, F8, step 2.1, step 3.1]

5.1 The bracket formula (2.15) in F8 vanishes for the positive-side commuting fields. Under the negative-copy change $(N,Y)\mapsto(-N,R^*Y)$ its lapse component changes sign under reflection and its shift component is reflected: each shift term $N D\bar N-\bar N DN$ contains two lapse signs. Thus their bracket KID is also zero on the negative side, and by smoothness on $S$. By F8 it is the KID of the developed commutator. Step 4.1 makes that commutator zero near $S$. The same uniqueness applied to the reflected linear relation gives $\widehat T=K-\Omega Z$ there, with $Z$ omitted when $\Omega=0$. [F2, F8, step 4.1, step 4.2, algebra]

6.1 Along $S$ the developed boost field vanishes. Its first derivative agrees with the original boost derivative: tangential derivatives to $A$ follow from its smooth KID, and its remaining Gaussian normal derivatives follow from (2.7)–(2.8) in F8. In the future/outward frame $(e_0,e_1)$ it is therefore the constant boost matrix with coefficient $\kappa>0$, annihilating $TS$. F9 gives its differential flow as that boost. Use the normal tube of F9 with coordinates $\exp_p(((V-U)e_0+(V+U)e_1)/2)$. Isometries commute with this exponential map, so differentiating the boost action gives exactly $K=\kappa(V\partial_V-U\partial_U)$ on a smaller tube. [F1, F8, F9, step 4.2, step 5.1, algebra]

7.1 In rotation the reflected rotation KID has zero lapse and shift tangent to the signed $r$ levels, because the original $Z$ preserves $U,V$. Its restriction to $S$ is the given $2\pi$-periodic action. Its local isometric flow preserves $A$, its chosen side and its future unit normal; hence along $S$ it sends $e_0,e_1$ to the corresponding future/outward frame at the rotated point. Exponential equivariance from F9 consequently identifies the local $Z$ flow with $(U,V,p)\mapsto(U,V,\phi_s^Zp)$. This formula itself defines the flow for all $s$ on a uniform smaller normal tube, since $S$ is compact and the normal coordinates are unchanged. Its maps are isometries: for sufficiently short parameters they are local Killing isometries, and any finite parameter is a finite sum of such short parameters. The period $2\pi$ follows from the action on $S$. This proves the asserted local circle action and exact coordinate relations, without continuing $Z$ to the entire exterior. [F1, F9, step 4.2, step 5.1, step 6.1, algebra]

8.1 Finally check the boundary germ, rather than infer it from the open-data embedding alone. In both the original metric and the developed metric, smooth Gaussian normal maps based on the closed positive section are defined near $S$: their differentials at zero map the section tangent space and its future unit normal isomorphically onto the ambient tangent space, so the local inverse assertion in F9 applies. The two original null sheets are transverse to these timelike normal curves; on a smaller chart they are graphs in the normal-time coordinate and enclose its right exterior interval containing time zero for every positive section point. Thus the segment from time zero to a point of that interval stays in $E$. On the open positive section $i$ fixes the data and carries the future normal to the future normal. Exponential equivariance therefore expresses $i$ in these charts as the identity wherever the normal geodesic segment stays in $E$. This gives its smooth extension and full differential at $S$ from the positive side; the metric identity holds there by continuity. On the section itself this is the restriction of the smooth embedding of the entire doubled Cauchy hypersurface, so it extends across $S$ as claimed. Its canonical radial curves are the outward normal geodesics from $S$ in both metrics: on $r>0$ their intrinsic acceleration and normal acceleration are determined by the same $h,\mathcal K$, and vanish as in the supplied original double-normal chart; smoothness includes $r=0$. Hence the normal tube of step 6.1 has the same positive canonical section. Equivariance from step 4.1 and the supplied stationary collar then match the positive exterior collar germ as well. This establishes the claimed compatibility at $S$, together with all the vacuum, completeness and symmetry conclusions. No domain-of-dependence identification for $E$ in a larger nonmaximal ambient spacetime is required. [F1, F4, F9, step 3.1, step 4.1, step 6.1, step 7.1, algebra] ∎

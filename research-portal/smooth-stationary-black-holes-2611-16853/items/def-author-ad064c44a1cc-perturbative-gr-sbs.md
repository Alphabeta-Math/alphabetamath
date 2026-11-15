---
id: def-author-ad064c44a1cc-perturbative-gr-sbs
title: AIK perturbative global regularity and bifurcation package
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-causal-exterior-and-boundary-data
  - def-spacelike-maximal-hypersurface-data
  - def-null-screen-expansion-and-focal-data
  - def-stationary-asymptotic-decay-data
  - physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets
  - def-author-254b7c4bab6d-regular-null-horizon-pair
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets: mathematical-premise
  def-author-254b7c4bab6d-regular-null-horizon-pair: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: "S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth
        stationary black holes in vacuum: small perturbations of the Kerr
        spaces"
      url: https://arxiv.org/html/0904.0982v1
      locator: Section 1.1, opening setup and footnote 3; GR, equations (1.1)–(1.3)
        and footnote 5; SBS and footnote 6.
      reading_limits: Consulted the arXiv v1 HTML text of section 1.1, its opening
        setup, GR (1.1)–(1.3), SBS, and footnotes 3, 5 and 6 in this assignment.
        Checked the transcription of these assumptions only. No source theorem
        proof, global rigidity argument or library proof audit was performed.
      statement: The setup specifies a connected oriented time-oriented smooth
        paracompact boundaryless vacuum four-spacetime, a smooth Killing field
        and an embedded partial Cauchy surface parametrized by E_{1/2}. GR
        specifies the stationary end chart, the three metric expansions (1.1),
        positive mass M and angular magnitude J in [0,M^2), the globally
        hyperbolic exterior, both slice identities (1.3), and nonvanishing
        complete exterior Killing orbits meeting the slice. SBS specifies the
        sphere at r=1, smooth embedded transverse null event-boundary sheets
        near it, zero trace of each null second fundamental form, tangency of
        the stationary field and the requirement that it not vanish identically
        on the sphere. No maximality is included in this GR/SBS passage.
      hypotheses: These are stipulated geometric data and assumptions in AIK section
        1.1, not conclusions inferred from asymptotic flatness alone. The
        exterior and both boundaries are computed in the given spacetime; the
        horizon-sheet assertions are local near S_0. PK and the Main Theorem are
        not imported here.
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609
      locator: Section 2.18, Definition 2.130, printed/PDF p. 76; section 3.2,
        Definition 3.35, printed/PDF p. 95.
      statement: For an achronal set S, edge(S) consists of q in the ambient closure
        of S such that every open neighborhood U of q contains a point a in
        I_U^-(q), a point b in I_U^+(q), and a timelike curve from a to b within
        U avoiding S. A partial Cauchy hypersurface is an acausal edgeless set.
      hypotheses: A time-oriented Lorentzian spacetime and an achronal subset S; edge
        is computed using the ambient closure and chronological curves confined
        to U. For the partial Cauchy terminology require acausality and empty
        edge. The present smooth metric and embedded spacelike surface are
        within this setting.
      reading_limits: Read the PDF text of Definition 2.130 and Definition 3.35, with
        their immediately adjacent explanations. This imports definitions only,
        not domain-of-dependence theorems or an assertion that an arbitrary
        embedded spacelike surface is edgeless.
    - title: E. Gourgoulhon and J. L. Jaramillo, A 3+1 perspective on null
        hypersurfaces and isolated horizons, arXiv:gr-qc/0503113v2
      url: https://arxiv.org/pdf/gr-qc/0503113v2
      locator: Section 2.2, (2.10)–(2.11), pp. 18–19; sections 2.6–2.7, (2.46)–(2.57)
        and Remark 2.8, pp. 28–31; section 5.6, (5.65), (5.71) and Remark 5.2,
        pp. 72–74; section 5.8, (5.114), p. 81 (printed and one-based PDF
        pages).
      statement: A smooth null hypersurface has degenerate induced signature (0,+,+)
        with a tangent null normal. Its symmetric null second fundamental form
        vanishes when either argument is the normal, hence is a form on the
        tangent quotient by the normal line. Expansion is its trace in a
        spacelike section, independent of the section for a fixed normal;
        positive rescaling of the normal multiplies the form and expansion by
        the same factor.
      hypotheses: A smooth null hypersurface in a smooth time-oriented
        four-dimensional Lorentzian manifold, a smooth nonzero local null
        normal, and local transverse spacelike sections. These are geometric
        constructions; neither a field equation, an energy condition, compact
        sections nor an isolated-horizon structure is used for the cited
        formulas.
      reading_limits: Read the PDF text at the cited nullness definition, Weingarten
        and second-form formulas, quotient remark, expansion definition,
        section-independence remark and rescaling formula. The screen/section
        formulation below retains these local geometric hypotheses. No
        Einstein-equation or isolated-horizon theorem, global foliation, global
        generator normalization or source-proof audit is imported.
dependency_level: 2
---

## Definition

The **AIK perturbative GR/SBS package** means the following specified data and conditions of Alexakis–Ionescu–Klainerman (AIK), arXiv:0904.0982v1 §1.1. Work with a connected oriented time-oriented smooth paracompact boundaryless four-spacetime $(M,g)$, $\operatorname{Ric}(g)=0$, a smooth Killing field $T$, and an embedded spacelike partial Cauchy surface $\Sigma^0$ (acausal and edgeless) parametrized by $\Phi_0:E_{1/2}\to\Sigma^0$, where $E_a=\{x\in\mathbb R^3:|x|>a\}$.

Here acausal has the causal-set interface's meaning: no two distinct points of the surface are joined by a causal curve in $M$. For an achronal set $A\subset M$, its causal edge consists of those $q\in\overline A^{\,M}$ for which every open neighborhood $U$ of $q$ admits $a\in I_U^-(q)$, $b\in I_U^+(q)$ and a future timelike curve from $a$ to $b$ contained in $U\setminus A$. The sets $I_U^\pm(q)$ use the restricted spacetime $U$. Edgeless means that this edge is empty. The partial Cauchy condition on $\Sigma^0$ requires acausality and edgelessness in the ambient $M$; neither follows here merely from spacelikeness.

GR supplies an open end $M^{\rm end}$ with a chart $\Phi_0:\mathbb R\times E_{R_0}\to M^{\rm end}$ extending the slice chart, $T=\partial_t$, and
$$g_{00}=-1+2M_0/r+O_6(r^{-2}),\quad g_{ij}=\delta_{ij}+O_6(r^{-1}),\quad g_{0i}=-2\epsilon_{ijk}S^jx^kr^{-3}+O_6(r^{-3}),$$
where $M_0>0$, $r=|x|$, $\epsilon_{123}=1$, and $J=|S|\in[0,M_0^2)$. All index sums are over their displayed ranges; the differentiated convention is the source one (including time derivatives, which vanish on the stationary end). Put $E=I_M^-(M^{\rm end})\cap I_M^+(M^{\rm end})$. Require $E$ globally hyperbolic, $\Sigma^0\cap I_M^\pm(M^{\rm end})=\Phi_0(E_1)$, $T$ nowhere zero on $E$, and every exterior $T$-orbit complete and meeting $\Sigma^0$.

SBS requires $S_0=\Phi_0(\{r=1\})$ to be the bifurcation sphere of the two event boundaries. In a neighborhood of $S_0$, $H^+=\partial_M I_M^-(M^{\rm end})$ and $H^-=\partial_M I_M^+(M^{\rm end})$ are smooth embedded null nonexpanding hypersurfaces, transverse with intersection $S_0$. Require $T$ tangent to both and $T|_{S_0}\not\equiv0$. Nonexpanding means zero null second-fundamental-form trace. This perturbative package does not add maximality of $\Sigma^0$; maximality belongs to other source contracts below.

For either local sheet $H$, null means that $g|_{TH}$ has signature $(0,+,+)$ and radical $\mathcal R_p=\{v\in T_pH:g(v,w)=0\text{ for all }w\in T_pH\}$. A local generator field $L$ is a smooth nonzero future-directed section of this null normal line. The screen is $\mathscr S_p=T_pH/\mathcal R_p$, with positive metric $\bar q([X],[Y])=g(X,Y)$. The null second fundamental form on the screen and its expansion are $\bar\chi_L([X],[Y])=g(\nabla_XL,Y)$ and $\theta_L=\operatorname{tr}_{\bar q}\bar\chi_L$. On a transverse spacelike two-section $Q\subset H$, this is $\operatorname{tr}_{g|_{TQ}}\chi_L$ with $\chi_L(X,Y)=g(\nabla_XL,Y)$. Nonexpansion in SBS requires $\theta_L=0$ everywhere on each local sheet, including $S_0$, for every such local generator field. The trace is on the positive screen or section metric; the degenerate metric on $TH$ is not inverted.

## Definition references

[[def-stationary-lorentzian-data]]

[[def-causal-exterior-and-boundary-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-null-screen-expansion-and-focal-data]]

[[def-stationary-asymptotic-decay-data]]

[[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]

[[def-author-254b7c4bab6d-regular-null-horizon-pair]]

[AIK, section 1.1, GR and SBS](https://arxiv.org/html/0904.0982v1)

[Minguzzi, Definitions 2.130 and 3.35](https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609)

[Gourgoulhon–Jaramillo, local null-hypersurface geometry](https://arxiv.org/pdf/gr-qc/0503113v2)

## Facts & Assumptions

[F1] [[def-stationary-lorentzian-data]] gives Lorentzian, Killing and connection data; [[def-causal-exterior-and-boundary-data]] gives ambient chronological sets, boundaries, exterior and causal predicates.

[F2] [[def-spacelike-maximal-hypersurface-data]] defines spacelike sections and their normals. [[def-null-screen-expansion-and-focal-data]] defines the section null form and its trace. [[def-stationary-asymptotic-decay-data]] defines differentiated asymptotic arrays and constants; the source time-derivative version agrees on the stationary end.

[F3] [[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]] supplies acausality and achronality. Minguzzi supplies the ambient causal-edge definition and the acausal-edgeless partial Cauchy terminology specified in External input.

[F4] [[def-author-254b7c4bab6d-regular-null-horizon-pair]] supplies the local radical, generator and section-expansion terminology. Only these definitional clauses are used; its additional affine-generator and relative causal-boundary requirements are not added to GR/SBS. Gourgoulhon–Jaramillo supplies the general null-hypersurface form, quotient trace and normalization properties specified in External input.

[F5] AIK section 1.1 supplies the source-specific GR/SBS clauses, including the strict parameter gap and nonidentically zero stationary field on the sphere. Its exact imported formulation and reading limits are recorded in the first source reference and External input.

## Justification

Each clause is a predicate on the supplied metric, field, embeddings and charts. The end coordinate derivatives and the exterior chronological sets are computed in their explicitly specified domains. The surface parametrization fixes the particular sphere $S_0$, and the separate horizon conditions test its event boundaries; they do not assert that a bifurcate Killing generator has already been constructed. No implication from a weaker regularity definition to this package is asserted. In particular the explicit angular leading term, strict subextremal parameter bound and nonzero-horizon-field clause remain part of this source contract.

The acausality interface and the imported causal-edge definition make the partial Cauchy requirement precise, with ambient closure retained. The cited null-hypersurface construction supplies the well-defined form on the positive screen and its section trace; its rescaling rule makes zero expansion independent of positive generator normalization. Thus the section formula agrees with the supplied null-screen convention without treating a two-surface definition alone as a definition on an entire hypersurface. These are geometric definitions and imported well-definedness facts, not a physical field law or a locally reconstructed horizon theorem.

## External input

[AIK, section 1.1](https://arxiv.org/html/0904.0982v1) supplies the GR/SBS assumptions transcribed above, with footnotes 3, 5 and 6 fixing the manifold, differentiated-decay and nonexpansion conventions. This item records those assumptions only; the PK hypothesis and global rigidity theorem are separate inputs.

[Minguzzi, Definitions 2.130 and 3.35](https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609) supplies the causal-edge and partial Cauchy definitions. In particular the edge test ranges over the ambient closure, and all curves in a neighborhood test remain in that neighborhood. No theorem that a supplied surface satisfies this test is asserted.

[Gourgoulhon–Jaramillo, sections 2.2, 2.6–2.7, 5.6 and 5.8](https://arxiv.org/pdf/gr-qc/0503113v2) supplies the local null-hypersurface construction and its well-definedness facts. The form annihilates the radical, the trace can be computed in any transverse spacelike section, and positive normal rescaling preserves its zero set. These geometric facts apply to the smooth local sheets in SBS without field equations or a global section. The full locators, hypotheses and reading limits are in the third source reference.

---
id: def-horizon-flux-and-stability-notation
title: Horizon null frame, flux densities and stability operator notation
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-harrison-electromagnetic-form
  - def-stationary-maximal-graph
  - def-surface-area-flux-and-null-variation-data
  - def-null-screen-expansion-and-focal-data
  - def-complex-self-dual-two-form-data
  - math:def-axiom-of-choice
  - def-coordinate-comparison-spheres
  - def-harrison-normalization
dependency_roles:
  def-harrison-electromagnetic-form: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  def-surface-area-flux-and-null-variation-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-coordinate-comparison-spheres: mathematical-premise
  def-harrison-normalization: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 26, proof of Theorem 4.2, definitions before equation (4.4);
        page 22, normalization before equation (4.2)
      statement: The article introduces the displayed horizon null frame, normal
        connection one-form, electric and magnetic flux densities, intrinsic
        surface notation, and outgoing-expansion variation; it uses a separately
        specified normalization on the distant comparison sphere.
      hypotheses: The article's positive-parameter Harrison geometry and smooth
        maximal section with bifurcation-sphere boundary; the comparison
        normalization is used on its distant sphere.
      reading_limits: Read the frozen extracted article text at the cited passages.
        The citation attributes the notation and is not used as a proof of
        well-definedness or of the later variation formula.
dependency_level: 6
---

## Definition

Assume the axiom of choice, used through its countable-choice consequence in the normal-graph construction. Fix $q\in(0,1]$ and supplied Harrison data giving an oriented, time-oriented Lorentzian metric $g_q$ of signature $(-,+,+,+)$ and a smooth real electromagnetic two-form $F_q$ on the Harrison open set $V$. Let $\Sigma_q$ be a supplied smooth spacelike maximal section with boundary $S$, as in the stationary maximal-graph setting: spacelike means that the induced metric is positive definite, and maximal means that the trace of its second fundamental form vanishes. As additional boundary data, supply an open spacetime neighborhood $U_S$ of $S$ and smooth extensions of both $g_q$ and $F_q$ to $U_S$: the extended metric is oriented, time-oriented and Lorentzian of the same signature, the extended two-form is real, and both agree with the Harrison fields on $U_S\cap V$, with matching orientations and time orientations. Write $g_q,F_q$ for these specified fields on $V\cup U_S$. Assume $S$ is a smooth oriented closed surface, and supply within $U_S$ a smooth spacelike extension of the section, a smooth outward unit normal $\nu_q$ to $S$ in that extension, and an admissible outward normal-graph tube. The unit normal $n_q$ to the extended section is future-directed. The orientation of $S$ fixes its area form $d\mu_q$; the spacetime orientation fixes the Hodge star $\star_{g_q}$.

Set $L_q=n_q+\nu_q$ and $\underline L_q=(n_q-\nu_q)/2$, so $g_q(L_q,\underline L_q)=-1$. Both are future null normals. For tangent $X$ define the normal-connection one-form $\zeta_q(X)=-g_q(\underline L_q,\nabla^{(q)}_X L_q)$, where $\nabla^{(q)}$ is the Levi–Civita connection of $g_q$; its components in a tangent frame $e_A$ are $(\zeta_q)_A=\zeta_q(e_A)$. Define the electric and magnetic flux densities $e_q,b_q$ by $(\star_{g_q}F_q)|_{TS}=e_q\,d\mu_q$ and $F_q|_{TS}=b_q\,d\mu_q$.

Write $\gamma_q=g_q|_{TS}$. Let $\not\nabla^{(q)}$ be its Levi–Civita connection, $\not\operatorname{div}^{(q)}$ the trace of the intrinsic covariant derivative, and $\not\Delta^{(q)}=\not\operatorname{div}^{(q)}\operatorname{grad}_{\gamma_q}$ the scalar Laplacian. Divergence of a one-form means divergence of its $\gamma_q$-dual vector field. Let $K_q=\gamma_q(R^{\gamma_q}(e_1,e_2)e_2,e_1)$ for a $\gamma_q$-orthonormal frame, with $R(X,Y)Z=\not\nabla_X\not\nabla_YZ-\not\nabla_Y\not\nabla_XZ-\not\nabla_{[X,Y]}Z$.

For an admissible normal graph $S_u$ over $S$, use its outward unit normal $\nu_{q,u}$ in the extended section and its future outgoing null normal $L_{q,u}=n_q+\nu_{q,u}$. Its outgoing expansion is the trace, in the induced surface metric, of $(X,Y)\mapsto g_q(\nabla^{(q)}_X L_{q,u},Y)$. Pull this expansion back to $S$ along the graph map and denote it by $\Theta_q(u)$. For smooth $\phi$ define $\mathscr L_q\phi=\left.\frac{d}{d\epsilon}\right|_{0}\Theta_q(\epsilon\phi)$: this is the first variation under displacement $\phi\nu_q$ in the specified null gauge. If the initial outgoing expansion vanishes, $S$ is a marginally outer trapped surface, abbreviated MOTS, and $\mathscr L_q$ is its outward stability operator in this section. No coefficient formula or sign of this operator is asserted here.

For the separate comparison-sphere convention, additionally supply the stationary product end with coordinates $(t,x)\in\mathbb R\times\{x\in\mathbb R^3:|x|>a\}$, $a>0$, and $T=\partial_t$, using the same original end as the stationary graph data. For $R_0>a$, set $r=|x|$ and $C_q=\{t=0,\ r=R_0q^{-2/3}\}$, as in the coordinate comparison-sphere definition, and require $C_q\subset V$. Assume $C_q$ is spacelike for $g_q$ and supply a smooth future outward null normal $\ell_q$ along it satisfying $g_q(T,\ell_q)<0$. Use the positive constant $d_q=D_q(p)$ from the stationary graph's Harrison normalization, and define
$$\widehat L_q=\frac{d_q}{-4g_q(T,\ell_q)}\,\ell_q,\qquad g_q(T,\widehat L_q)=-d_q/4.$$
This is the unique positive rescaling of the supplied $\ell_q$ with that normalization. The horizon convention $L_q=n_q+\nu_q$ and the comparison convention $\widehat L_q$ are separate; the article uses the symbol $L_q$ in both settings.

## Definition references

[[def-harrison-electromagnetic-form]]

[[def-stationary-maximal-graph]]

[[def-surface-area-flux-and-null-variation-data]]

[[def-null-screen-expansion-and-focal-data]]

[[def-complex-self-dual-two-form-data]]

[[math:def-axiom-of-choice]]

[[def-coordinate-comparison-spheres]]

[[def-harrison-normalization]]

## Facts & Assumptions

[F1] The Harrison electromagnetic construction supplies $g_q,F_q$ on $V$ under its stated hypotheses; the stationary graph definition supplies the maximal-section setting and the positive constant $d_q$. The smooth metric and real two-form on $U_S$, their overlap compatibility, and the spacelike section extension in $U_S$ are additional supplied boundary data in the Definition, satisfying the ambient hypotheses of the surface-data supplier. [[def-harrison-electromagnetic-form]] [[def-stationary-maximal-graph]] [[def-surface-area-flux-and-null-variation-data]]

[F2] The surface-data supplier defines the normal gauge, flux-density ratios, intrinsic operations and normal-graph expansion linearization, and establishes their well-definedness under its stated orientation and graph hypotheses. [[def-surface-area-flux-and-null-variation-data]]

[F3] The null-screen supplier defines the null second fundamental form and its expansion as its induced-metric trace. [[def-null-screen-expansion-and-focal-data]]

[F4] The complex-form supplier fixes the smooth metric Hodge star on an oriented Lorentzian four-manifold. [[def-complex-self-dual-two-form-data]]

[A1] The axiom of choice implies the countable-choice assumption used by the normal-graph supplier. [[math:def-axiom-of-choice]]

[F5] The coordinate comparison-sphere supplier defines $C_q$ in the supplied product end; the Harrison normalization defines $d_q=D_q(p)$. Its positivity here is supplied by the stationary graph data. Spacelikeness of $C_q$ and the smooth future outward null normal $\ell_q$ with negative $T$-pairing are the additional comparison data in the Definition. [[def-coordinate-comparison-spheres]] [[def-harrison-normalization]] [[def-stationary-maximal-graph]]

## Justification

**Given:** The supplied positive-parameter data, compatible smooth boundary extensions, orientations, normals and admissible normal-graph tube in the Definition; for the separate comparison convention, its additional end, sphere and null-normal data.

**Goal:** Justify the displayed notation and the existence of the stated linearization under those hypotheses.

1.1 The unit normals satisfy $g_q(n_q,n_q)=-1$, $g_q(\nu_q,\nu_q)=1$ and $g_q(n_q,\nu_q)=0$. Consequently $L_q$ and $\underline L_q$ are null, have pairing $-1$, and are future-directed. The supplied extensions place a smooth Lorentzian metric and a smooth real two-form on the same open neighborhood $U_S$ of $S$, agreeing with the Harrison fields wherever they overlap $V$. Apply the surface-data supplier to the spacelike extension of the section in this neighborhood: it makes the normal connection one-form well defined. The smooth Hodge star there and the nonvanishing oriented area form give each restricted two-form a unique smooth scalar coefficient, defining $e_q$ and $b_q$ for these supplied fields. [given, F1, F2, F4, algebra]

2.1 The surface-data supplier gives the intrinsic connection, divergence, Laplacian and frame-independent Gauss curvature with the displayed conventions. The null-screen definition identifies the expansion used in the graph construction, and the surface-data supplier establishes existence and linearity of its normal-graph derivative in the stated gauge, with countable choice for that construction. The MOTS and stability-operator names apply under the explicitly stated vanishing condition. [given, A1, F2, F3, step 1.1]

3.1 For the separate comparison data, the coordinate supplier places $C_q$ in the supplied end, and the explicit inclusion $C_q\subset V$ makes $g_q(T,\ell_q)$ defined. Since $d_q>0$ and $g_q(T,\ell_q)<0$, the scalar $s_q=d_q/(-4g_q(T,\ell_q))$ is smooth and strictly positive on $C_q$. Thus $\widehat L_q=s_q\ell_q$ remains future outward null and normal to $C_q$, and linearity gives $g_q(T,\widehat L_q)=-d_q/4$. If another positive rescaling $s\ell_q$ has this pairing, division by the nonzero $g_q(T,\ell_q)$ forces $s=s_q$. This verifies precisely the separate normalization on the supplied outgoing ray. [given, F5, algebra] ∎

## Source notes

The article citation attributes the notation and the separate comparison-sphere normalization. The boundary extensions and the comparison sphere's spacelikeness and negative-pairing null normal are explicit supplied data; their existence is not asserted here. The justification uses the stated suppliers and local algebra, and does not use the article's variation formula as a premise.

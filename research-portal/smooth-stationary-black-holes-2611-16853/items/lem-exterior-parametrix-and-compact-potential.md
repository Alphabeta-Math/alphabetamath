---
id: lem-exterior-parametrix-and-compact-potential
title: Exterior Dirichlet parametrix and compact decaying potentials
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-exterior-weighted-elliptic-data
  - def-fredholm-continuation-data
  - def-stationary-asymptotic-decay-data
  - lem-author-86990d62062f-weighted-scalar-inverse
  - lem-author-86990d62062f-closed-component-index
  - lem-author-86990d62062f-compact-potential
  - math:thm-fredholm-index-is-stable-under-compact-perturbations
dependency_roles:
  def-exterior-weighted-elliptic-data: mathematical-premise
  def-fredholm-continuation-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  lem-author-86990d62062f-weighted-scalar-inverse: mathematical-premise
  lem-author-86990d62062f-closed-component-index: mathematical-premise
  lem-author-86990d62062f-compact-potential: mathematical-premise
  math:thm-fredholm-index-is-stable-under-compact-perturbations: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 4
---

## Statement

Let $(\Sigma,h)$ be the smooth three-dimensional exterior with compact smooth boundary of the weighted exterior definition, $0<\alpha<1$, $h-\delta\in C^{3,\alpha}_{-1}$ and $-1<\beta<0$. The scalar Dirichlet Laplacian $\Delta_h:X_\beta\to Y_\beta$ is Fredholm of index zero. Multiplication by any real $V\in C^{2,\alpha}_{-4}$ is compact from $X_\beta$ to $Y_\beta$. Hence $\Delta_h-V$ is Fredholm of index zero. No sign assumption on $V$ is required for this index assertion. The smooth compact inner boundary is included in the construction; no restriction on its number of components or on the topology of the compact core is imposed.

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] The exact weighted spaces and end falloff conventions are fixed. [[def-exterior-weighted-elliptic-data]] [[def-stationary-asymptotic-decay-data]]

[F2] Fredholm means finite-dimensional kernel and cokernel and closed range between Banach spaces. [[def-fredholm-continuation-data]]

[F3] The scalar Laplacian on the end component has a bounded inverse obtained by compact-boundary exhaustion; Proof 4.1 of this supplier proves completeness of its end-component spaces. [[lem-author-86990d62062f-weighted-scalar-inverse]]

[F4] There are finitely many extra compact components. Proof 2.1 of this supplier proves their Hölder spaces are Banach and their nonempty-boundary Dirichlet inverses are bounded; Proof 4.1 gives the bounded mean-zero Green inverse on each closed component, and Proof 5.1 identifies its kernel and range. [[lem-author-86990d62062f-closed-component-index]]

[F5] Potential multiplication is compact at the stated orders and weights. [[lem-author-86990d62062f-compact-potential]]

[F6] A compact perturbation preserves Fredholmness and index. [[math:thm-fredholm-index-is-stable-under-compact-perturbations]]

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] The exact weighted spaces and end falloff conventions are fixed. [[def-exterior-weighted-elliptic-data]] [[def-stationary-asymptotic-decay-data]]

[F2] Fredholm means finite-dimensional kernel and cokernel and closed range between Banach spaces. [[def-fredholm-continuation-data]]

[F3] The scalar Laplacian on the end component has a bounded inverse obtained by compact-boundary exhaustion; Proof 4.1 of this supplier proves completeness of its end-component spaces. [[lem-author-86990d62062f-weighted-scalar-inverse]]

[F4] There are finitely many extra compact components. Proof 2.1 of this supplier proves their Hölder spaces are Banach and their nonempty-boundary Dirichlet inverses are bounded; Proof 4.1 gives the bounded mean-zero Green inverse on each closed component, and Proof 5.1 identifies its kernel and range. [[lem-author-86990d62062f-closed-component-index]]

[F5] Potential multiplication is compact at the stated orders and weights. [[lem-author-86990d62062f-compact-potential]]

[F6] A compact perturbation preserves Fredholmness and index. [[math:thm-fredholm-index-is-stable-under-compact-perturbations]]



**Proof technique:** direct.

1.1 Write $\Sigma_0$ for the end component and $M_1,\ldots,M_m$ for the finitely many compact components supplied by [F4]. The spaces $X_0,Y_0$ on $\Sigma_0$ are Banach by [F3], Proof 4.1, and the compact-component spaces $X_j,Y_j$ are Banach by [F4], Proof 2.1, at orders four and two respectively. Here $X_j$ has zero trace when $\partial M_j\ne\varnothing$. Restriction identifies $X_\beta$ and $Y_\beta$ with these finite direct sums, with equivalent norms: the annular term involves only $\Sigma_0$, and the compact terms are finite chart norms. Smooth coordinate transitions compare these compact norms by the chain and product rules. Restriction decreases each chart supremum and seminorm; conversely, pairs lying in different components of a fixed compact chart subset have positive Euclidean separation, so their Hölder quotients are bounded by derivative suprema. Thus the full norm and the sum of the component norms bound each other by fixed constants. A Cauchy sequence in either full space is therefore Cauchy in each component space, has component limits there, and converges in the finite sum norm and hence in the original norm. The component limits glue across the disjoint open-and-closed components and preserve the zero boundary values. This proves completeness of both full-exterior spaces. [F1, F3, F4]

2.1 Let $H_j$ denote the mean-zero inverse of $\Delta_h$ on a closed component $M_j$. The estimate $\|H_j f\|_{C^{4,\alpha}(M_j)}\le C_j\|f\|_{C^{2,\alpha}(M_j)}$ for mean-zero $f$ is proved in [F4], Proof 4.1; it is not inferred merely from a kernel-and-range assertion. Put $P_j f=\mu_h(M_j)^{-1}\int_{M_j}f\,d\mu_h$, viewed as a constant function. Since $|P_j f|\le\|f\|_{C^0(M_j)}$, this is a bounded projection at both relevant Hölder orders. Use $H_j(I-P_j)$ as the closed-component block of $G$, the bounded compact Dirichlet inverse on each nonempty-boundary compact component, and the bounded end inverse on $\Sigma_0$. The finite sum and step 1.1 make $G:Y_\beta\to X_\beta$ bounded. The same componentwise reasoning makes $\Delta_h:X_\beta\to Y_\beta$ bounded. The inverse identities on each component give $\Delta_hG=I_{Y_\beta}-\Pi_Y$ and $G\Delta_h=I_{X_\beta}-\Pi_X$, where $\Pi_X,\Pi_Y$ apply $P_j$ on closed components and vanish elsewhere. They are bounded finite-rank projections. [F1, F3, F4, step 1.1]

3.1 Let $q$ be the number of closed compact components. Their constants are in the Laplacian kernel, and $G\Delta_h=I-\Pi_X$ implies that these are the entire kernel. The closed-component range assertion in [F4] gives $\Pi_Y\Delta_h=0$, while $\Delta_hG=I-\Pi_Y$ shows every element of $\ker\Pi_Y$ lies in the range. Hence $\operatorname{ran}\Delta_h=\ker\Pi_Y$, a closed subspace. The kernel and cokernel both have dimension $q$, since $\Pi_X$ and $\Pi_Y$ project onto the $q$ independent closed-component constants. Together with boundedness and the Banach property this proves Fredholmness and index zero, with all inner-boundary conditions retained. [F2, F4, step 1.1, step 2.1]

4.1 Multiplication by $V$ is a compact bounded linear map by [F5]. Step 1.1 establishes the Banach hypotheses on the full exterior, including its compact components, and step 3.1 establishes Fredholmness of the bounded Dirichlet Laplacian. Apply [F6] to this operator and the compact map $-M_V$, where $M_Vu=Vu$. The operator $\Delta_h-V$ is Fredholm with the same index zero. No sign assumption on $V$ was used. This proves all assertions. [F5, F6, step 1.1, step 3.1] ∎

## Source notes

The proof composes the existing scalar exhaustion inverse with the compact-block construction. In the latter, Proof 2.1 proves compact Hölder completeness and the bounded Dirichlet inverse, and Proof 4.1 proves the mean-zero Green estimate used here. The finite-component argument above completes the full-exterior Banach-space check. No weighted vector-operator theorem is used.

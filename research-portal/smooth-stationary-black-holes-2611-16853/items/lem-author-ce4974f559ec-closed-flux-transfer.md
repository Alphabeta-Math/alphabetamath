---
id: lem-author-ce4974f559ec-closed-flux-transfer
title: Closed electric and magnetic two-forms transfer their periods to the horizon
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:thm-stokes-theorem-for-smooth-singular-chains
  - def-source-free-geometric-electrovacuum-data
  - math:prop-integration-over-an-oriented-embedded-submanifold
  - math:lem-de-rham-top-integral-is-fundamental-class-evaluation
  - math:def-fundamental-class-of-a-compact-oriented-manifold
  - math:thm-smooth-singular-chains-compute-singular-homology
  - math:def-smooth-singular-chain-and-cochain-complexes
  - math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges
  - math:thm-general-stokes-theorem
  - math:thm-the-exterior-derivative-commutes-with-pullback
  - math:def-axiom-of-choice
dependency_roles:
  math:thm-stokes-theorem-for-smooth-singular-chains: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  math:prop-integration-over-an-oriented-embedded-submanifold: mathematical-premise
  math:lem-de-rham-top-integral-is-fundamental-class-evaluation: mathematical-premise
  math:def-fundamental-class-of-a-compact-oriented-manifold: mathematical-premise
  math:thm-smooth-singular-chains-compute-singular-homology: mathematical-premise
  math:def-smooth-singular-chain-and-cochain-complexes: mathematical-premise
  math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges: mathematical-premise
  math:thm-general-stokes-theorem: mathematical-premise
  math:thm-the-exterior-derivative-commutes-with-pullback: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Let $\alpha,\beta$ be smooth closed real two-forms on an exterior and on a smooth collar of a compact inner sphere $S$. Suppose large outward-oriented spheres $S_R$ and $S$ bound a smooth compact oriented three-chain $C_R$ contained in that exterior and collar, with $\partial C_R=S_R-S$. Then $\int_S\alpha=\int_{S_R}\alpha$ and $\int_S\beta=\int_{S_R}\beta$. The same holds for any oriented closed surface homologous to $S$ through smooth compact chains in the region of closedness. In electrovacuum take $\alpha=F_q$ and $\beta=\star_{g_q}F_q$.

Work in ZFC. All forms, surfaces and chains are in one smooth Hausdorff second-countable manifold $U$, possibly with boundary, containing the exterior and its collar. The surfaces are smooth embedded, compact, oriented and without boundary. For an inclusion $i_A:A\hookrightarrow U$, choose a finite real smooth singular cycle $z_A\in C_2^\infty(A;\mathbb R)$ representing its real fundamental class $[A]$. In the singular-chain interpretation, the bounding hypothesis means that $C_R\in C_3^\infty(U;\mathbb R)$ satisfies $\partial C_R=(i_{S_R})_\#z_{S_R}-(i_S)_\#z_S$. Every simplex occurring with nonzero coefficient in $C_R$ has its entire image in the exterior-and-collar region where both forms are closed. The homology assertion likewise means that $(i_A)_\#z_A-(i_S)_\#z_S=\partial C$ for a finite smooth singular three-chain $C$ in the region of closedness; it is independent of the chosen fundamental cycles. The bounding hypothesis also allows a compact oriented smooth three-dimensional cobordism $B_R$ smoothly embedded in $U$ with its entire image in that same exterior-and-collar region of closedness, whose boundary with its outward-normal-first orientation is $S_R\sqcup(-S)$. All boundary and chain relations use the given surface orientations.

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] Stokes on a finite real smooth singular chain gives $\int_c d\eta=\int_{\partial c}\eta$. [[math:thm-stokes-theorem-for-smooth-singular-chains]]

[F2] The source-free geometric electrovacuum definition gives $dF_q=d(\star_{g_q}F_q)=0$ and fluxes equal to the oriented pullback integrals divided by $4\pi$. Integration over an embedded surface is integration of its pulled-back top form. [[def-source-free-geometric-electrovacuum-data]] [[math:prop-integration-over-an-oriented-embedded-submanifold]]

[F3] A compact oriented boundaryless manifold has its orientation-determined real fundamental class. Smooth singular homology computes ordinary real singular homology naturally for smooth maps. For a smooth real top form $\eta$ on a compact oriented smooth boundaryless surface $A$ and any smooth cycle $z_A$ representing $[A]$, $\int_{z_A}\eta=\int_A\eta$: this is the chain-evaluation identity proved in steps 1.1 and 3.1 of the top-integral supplier. [[math:def-fundamental-class-of-a-compact-oriented-manifold]] [[math:thm-smooth-singular-chains-compute-singular-homology]] [[math:lem-de-rham-top-integral-is-fundamental-class-evaluation]]

[F4] Smooth singular chains are finite real linear combinations of smooth simplices, with the signed face boundary and homology $\ker\partial/\operatorname{im}\partial$. Smooth postcomposition defines the chain pushforward and commutes with the boundary. Pullback of forms is smooth and functorial. [[math:def-smooth-singular-chain-and-cochain-complexes]] [[math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges]]

[F5] Manifold Stokes integrates a compactly supported two-form on an oriented smooth three-manifold to its outward-normal-first boundary integral. Exterior differentiation commutes with smooth pullback. [[math:thm-general-stokes-theorem]] [[math:thm-the-exterior-derivative-commutes-with-pullback]]

[F6] The Axiom of Choice is included in ZFC; it supplies the Choice hypothesis of the top-integral bridge and the countable choice required by smooth-chain comparison and manifold Stokes. [[math:def-axiom-of-choice]]

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] Stokes on a finite real smooth singular chain gives $\int_c d\eta=\int_{\partial c}\eta$. [[math:thm-stokes-theorem-for-smooth-singular-chains]]

[F2] The source-free geometric electrovacuum definition gives $dF_q=d(\star_{g_q}F_q)=0$ and fluxes equal to the oriented pullback integrals divided by $4\pi$. Integration over an embedded surface is integration of its pulled-back top form. [[def-source-free-geometric-electrovacuum-data]] [[math:prop-integration-over-an-oriented-embedded-submanifold]]

[F3] A compact oriented boundaryless manifold has its orientation-determined real fundamental class. Smooth singular homology computes ordinary real singular homology naturally for smooth maps. For a smooth real top form $\eta$ on a compact oriented smooth boundaryless surface $A$ and any smooth cycle $z_A$ representing $[A]$, $\int_{z_A}\eta=\int_A\eta$: this is the chain-evaluation identity proved in steps 1.1 and 3.1 of the top-integral supplier. [[math:def-fundamental-class-of-a-compact-oriented-manifold]] [[math:thm-smooth-singular-chains-compute-singular-homology]] [[math:lem-de-rham-top-integral-is-fundamental-class-evaluation]]

[F4] Smooth singular chains are finite real linear combinations of smooth simplices, with the signed face boundary and homology $\ker\partial/\operatorname{im}\partial$. Smooth postcomposition defines the chain pushforward and commutes with the boundary. Pullback of forms is smooth and functorial. [[math:def-smooth-singular-chain-and-cochain-complexes]] [[math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges]]

[F5] Manifold Stokes integrates a compactly supported two-form on an oriented smooth three-manifold to its outward-normal-first boundary integral. Exterior differentiation commutes with smooth pullback. [[math:thm-general-stokes-theorem]] [[math:thm-the-exterior-derivative-commutes-with-pullback]]

[F6] The Axiom of Choice is included in ZFC; it supplies the Choice hypothesis of the top-integral bridge and the countable choice required by smooth-chain comparison and manifold Stokes. [[math:def-axiom-of-choice]]

**Proof technique:** direct.

1.1 For any surface $A$ in the Statement, the fundamental class and smooth-chain comparison supply a cycle $z_A$ as specified. The restricted form $i_A^*\alpha$ is a smooth top form on the compact oriented boundaryless surface, so the top-integral bridge gives $\int_A\alpha=\int_A i_A^*\alpha=\int_{z_A}i_A^*\alpha$. To compare with a chain in $U$, write $z_A=\sum_j a_j\sigma_j$. Functoriality gives $\sigma_j^*i_A^*\alpha=(i_A\circ\sigma_j)^*\alpha$ for each simplex; summing the defining simplex integrals gives $\int_{z_A}i_A^*\alpha=\int_{(i_A)_\#z_A}\alpha$. Every sum is finite. For each affine face map $\delta_k$, $(i_A\circ\sigma_j)\circ\delta_k=i_A\circ(\sigma_j\circ\delta_k)$, so the signed face sums also give $\partial(i_A)_\#=(i_A)_\#\partial$. The identical reasoning applies to $\beta$. Choice is used only as required by the cited top-integral and smooth-chain suppliers. [F1, F2, F3, F4, F6]

1.2 In the cobordism case let $j:B_R\hookrightarrow U$ be its inclusion. The smooth two-form $j^*\alpha$ has compact support because $B_R$ is compact. The containment hypothesis gives $j^*(d\alpha)=j^*(d\beta)=0$ everywhere on $B_R$. Manifold Stokes and commutation of exterior derivative with pullback give $\int_{S_R}\alpha-\int_S\alpha=\int_{\partial B_R}(j|_{\partial B_R})^*\alpha=\int_{B_R}d(j^*\alpha)=\int_{B_R}j^*(d\alpha)=0$. The boundary components have precisely the stated orientations. The same computation applies to $\beta$; thus the usual compact annulus is covered directly, without identifying a manifold with a singular chain. [F2, F5, F6, given]

2.1 In the singular-chain case apply Stokes in $U$ to the actual finite three-chain $C_R$. Each of its nonzero simplices has image in the region of closedness, so the pullbacks of $d\alpha$ and $d\beta$ to every such simplex vanish. Using step 1.1 to identify the boundary evaluations gives $\int_{S_R}\alpha-\int_S\alpha=\int_{\partial C_R}\alpha=\int_{C_R}d\alpha=0$. The same argument gives the equality for $\beta$. If closedness is initially known only in the open exterior and the forms extend smoothly to the collar boundary, the coefficients of their exterior derivatives extend continuously there and are limits of zero; hence the same calculation remains valid at that boundary. [F1, F4, step 1.1, given]

3.1 For a homologous closed surface $A$, replace the boundary of $C_R$ in step 2.1 by $(i_A)_\#z_A-(i_S)_\#z_S=\partial C$ and use the same bridge to obtain $\int_A\alpha=\int_S\alpha$ and $\int_A\beta=\int_S\beta$. If $z_A$ is replaced by another smooth representative of $[A]$, their difference is a smooth boundary by the smooth-chain comparison; its pushforward is a boundary by postcomposition, so the hypothesis and the computed integrals do not change. The same applies to $z_S$. The orientation on $S$ is the one in $S_R-S$, opposite to the inner-boundary orientation of the truncated exterior. In a source-free geometric electrovacuum datum, $\alpha=F_q$ and $\beta=\star_{g_q}F_q$ satisfy exactly the closedness assumptions; dividing the two period equalities by $4\pi$ therefore preserves both magnetic and electric charges. This proves the Statement. [F2, F3, F4, step 1.1, step 2.1, step 1.2] ∎

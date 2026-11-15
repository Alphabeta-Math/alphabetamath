---
title: The surviving source-normal ray has the outgoing affine normalization
status: published
research_item: lem-author-fd27ddabb933-outward-null-affine-normalization
dependency_level: 6
---

## Prerequisites

- [lem-author-fd27ddabb933-inward-branch-exterior-exclusion](item-lem-author-fd27ddabb933-inward-branch-exterior-exclusion)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain)
- [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)
- [lem-author-fd27ddabb933-outward-graph-null-initial-jets](item-lem-author-fd27ddabb933-outward-graph-null-initial-jets)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)


## Statement

Work in ZFC. Let $(M,g)$ be a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$ with its Levi–Civita connection. Use the compact spacelike two-surface $S$, the future/outward frame $(n,\nu)$, the oriented open exterior $\mathcal E$, and the smooth spacelike section extension $(\Sigma,h)$ of the outward-graph initial-jets data. Fix a smooth function $\phi>0$ on $S$. Choose $\epsilon>0$ sufficiently small that $u=\epsilon\phi$ is an admissible normal graph and the inward-branch exclusion applies, and let $K$ be its fixed compact tube. Set $F_\epsilon(y)=\exp^h_y(\epsilon\phi(y)\nu_y)$ and $S_\epsilon=F_\epsilon(S)$.

Let $n_\epsilon$ be the future unit normal of $\Sigma$ restricted to $S_\epsilon$, and let $\nu_\epsilon$ be the canonical outward unit graph normal tangent to $\Sigma$, with positive pairing with the increasing normal-tube coordinate direction. Put $L_\epsilon=n_\epsilon+\nu_\epsilon$ and $V_\epsilon=n_\epsilon-\nu_\epsilon$. Every nonzero future null normal $w$ to $S_\epsilon$ at $p$ is a positive multiple of exactly one of $L_\epsilon(p)$ and $V_\epsilon(p)$.

Suppose $\gamma:[0,b]\to M$, $b>0$, is a future affinely parametrized null geodesic with $\gamma(0)=p\in S_\epsilon$, $\dot\gamma(0)=w$ normal to $S_\epsilon$, $\gamma([0,b])\subset\mathcal E$, and $\gamma(b)\notin K$. Then $w=cL_\epsilon(p)$ for a unique $c>0$. The positive affine rescaling $\widehat\gamma(\lambda)=\gamma(\lambda/c)$, $0\le\lambda\le cb$, has the same oriented curve image and initial tangent exactly $L_\epsilon(p)$. It is the unique positive affine rescaling with source parameter zero and that initial tangent. In the normal congruence initialized by the smooth field $L_\epsilon$, the optical expansion at parameter zero is the surface expansion $\theta_{L_\epsilon}$ in this exact outgoing gauge.

## Facts & Assumptions

[F1] For the sufficiently small graph family and fixed compact tube $K$ of the inward-branch exclusion, a future null geodesic starting on $S_\epsilon$, remaining entirely in the open exterior $\mathcal E$, and ending outside $K$ cannot have initial tangent a positive multiple of $V_\epsilon=n_\epsilon-\nu_\epsilon$. [lem-author-fd27ddabb933-inward-branch-exterior-exclusion](item-lem-author-fd27ddabb933-inward-branch-exterior-exclusion)

[F2] The spacelike-hypersurface data supply the smooth future unit normal of $\Sigma$. On an admissible normal graph, the canonical outward graph-gauge lemma supplies a smooth unit normal $\nu_\epsilon$ tangent to $\Sigma$ and normal to $S_\epsilon$, with $g(n_\epsilon,n_\epsilon)=-1$, $g(\nu_\epsilon,\nu_\epsilon)=1$, and $g(n_\epsilon,\nu_\epsilon)=0$. Its outward convention is positive pairing with the increasing tube coordinate direction, and its outgoing null field is $n_\epsilon+\nu_\epsilon$. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)

[F3] For a smooth affine null normal congruence initialized by a null normal field $L$, the initial optical expansion equals $\theta_L=\operatorname{tr}_{g|_{TS}}\chi_L$, where $\chi_L(X,Y)=g(\nabla_XL,Y)$. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F4] On a smooth time-oriented Lorentzian four-manifold with its metric-selected connection, the geodesic initial-value theorem supplies uniqueness, an open smooth geodesic evaluation domain, and the scaling law $\gamma_{p,sv}(t)=\gamma_{p,v}(st)$ whenever either side is defined, with matching rescaled domains. Only clauses (a)–(c) are used here. The supplier has domain mathematics. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F5] For the compact surface $S$ in the smooth spacelike section extension, the normal-graph domain lemma supplies a Riemannian normal tube and embedded spacelike graphs $F_u$ whenever the graph of $u$ lies in that tube domain. For fixed smooth $\phi$ on $S$, $u=\epsilon\phi$ is admissible for all sufficiently small $|\epsilon|$. [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain)

[F6] The outward-graph initial-jets data supply the oriented exterior and the section extension used here, the family $F_\epsilon(y)=\exp^h_y(\epsilon\phi(y)\nu_y)$ for fixed smooth $\phi>0$, and the future/outward graph fields $n_\epsilon,\nu_\epsilon$. For sufficiently small positive $\epsilon$ these graphs lie in $\mathcal E$, with the unhalved inward field $V_\epsilon=n_\epsilon-\nu_\epsilon$ and outgoing field $L_\epsilon=n_\epsilon+\nu_\epsilon$. [lem-author-fd27ddabb933-outward-graph-null-initial-jets](item-lem-author-fd27ddabb933-outward-graph-null-initial-jets)

[A1] Work in ZFC, including the choice assumptions inherited from the graph, geodesic, compactness and causal suppliers. No additional choice principle is used in the normal-plane calculation or the uniquely determined affine rescaling. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The geometric data and the segment hypotheses of the Statement.

**Goal:** Classify the initial normal ray and establish its unique outgoing affine scale and initial expansion.

1.1 By [F5]–[F6] the chosen graph is an embedded spacelike two-surface, and [F2] supplies its smooth future/outward orthonormal frame. The independent vectors $n_\epsilon,\nu_\epsilon$ are orthogonal to its two-dimensional tangent space, so they span its Lorentzian normal plane. Write $w=\alpha n_\epsilon+\beta\nu_\epsilon$. Nullness gives $\beta^2=\alpha^2$, while future direction gives $\alpha=-g(w,n_\epsilon)>0$. Thus $w=\alpha L_\epsilon$ or $w=\alpha V_\epsilon$, and these rays are distinct. [F2, F5, F6, given, algebra]

2.1 The segment in the Statement starts at this graph with initial vector $w$, remains in the open exterior, and ends outside the fixed tube. These are precisely the conditions in [F1]; its inward possibility is therefore excluded. Hence $w=cL_\epsilon(p)$ with $c=\alpha>0$, uniquely by the frame decomposition. [F1, step 1.1, given, algebra]

3.1 Apply [F4], clause (c), with initial vector $w$ and scaling factor $1/c$. It gives the affine geodesic $\widehat\gamma(\lambda)=\gamma(\lambda/c)$ on $[0,cb]$ with initial tangent $w/c=L_\epsilon(p)$. The increasing bijection $\lambda\mapsto\lambda/c$ preserves the oriented curve image and both endpoints. An affine parameter change preserving source parameter zero has the form $t=a\lambda$; its initial tangent is $aw$, so the required tangent forces $a=1/c$. This proves uniqueness of the positive rescaling. [F4, step 2.1, algebra]

4.1 The field $L_\epsilon$ along the graph is smooth by [F2]. The open smooth evaluation domain in [F4], clauses (a)–(b), supplies, near each source point and parameter zero, the affine normal geodesic congruence initialized by this field. Its initial optical expansion is $\theta_{L_\epsilon}$ by [F3]. In particular the expansion is in the unhalved outgoing gauge, with no target-cylinder rescaling. The usual positive normal-scale rule also follows from the same definition: for a positive smooth function $f$ on the source, $g(\nabla_X(fL_\epsilon),Y)=f g(\nabla_XL_\epsilon,Y)$ for source-tangent $X,Y$, because $g(L_\epsilon,Y)=0$; hence $\theta_{fL_\epsilon}=f\theta_{L_\epsilon}$. [F2, F3, F4, step 3.1, algebra] ∎

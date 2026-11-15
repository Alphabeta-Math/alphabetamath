---
title: Compact normalized source data give a target-independent energy bound
status: published
research_item: lem-author-fd27ddabb933-compact-source-energy-bound
dependency_level: 7
---

## Prerequisites

- [lem-author-fd27ddabb933-outward-null-affine-normalization](item-lem-author-fd27ddabb933-outward-null-affine-normalization)
- [lem-author-fd27ddabb933-killing-energy-conservation](item-lem-author-fd27ddabb933-killing-energy-conservation)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain)
- [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)
- [math:prop-smooth-maps-are-continuous](https://alphabetamath.cc/item/prop-smooth-maps-are-continuous)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)


## Statement

Work in ZFC. Use stationary Lorentzian data $(M,g,T)$ of signature $(-,+,+,+)$ with their specified time orientation and Levi–Civita connection. Let $U\subset M$ be a designated open end on which $T$ is future timelike. Let $\Sigma$ be a smooth embedded spacelike hypersurface with induced metric $h$ and smooth future unit normal $n_\Sigma$. Let $S\subset\operatorname{int}\Sigma$ be a nonempty compact smooth embedded two-surface without boundary, carrying a supplied smooth outward $h$-unit normal $\nu_0$ tangent to $\Sigma$. Fix a smooth $\phi>0$ on $S$ and one $\epsilon>0$ sufficiently small that $u=\epsilon\phi$ is admissible in the Riemannian normal tube. Set $F_\epsilon(y)=\exp^h_y(\epsilon\phi(y)\nu_0(y))$ and $A=F_\epsilon(S)$. On this fixed outward graph put $n=n_\Sigma|_A$ and let $\nu$ be its canonical smooth outward unit normal tangent to $\Sigma$, with positive pairing with the increasing normal-tube coordinate direction.

The number $E_{\max}=1+\max_{p\in A}|g_p(T_p,n_p+\nu_p)|$ is finite and depends only on the fixed source data. For every future affinely parametrized null geodesic segment $\gamma:[0,b]\to M$, $b>0$, with $\gamma(0)\in A$, $\dot\gamma(0)=n+\nu$ at its source point, and $\gamma(b)\in U$, its stationary energy $E=-g(T,\dot\gamma)$ satisfies $0<E\le E_{\max}$ throughout the segment. The bound is independent of target radius and target stationary translate. In particular it applies to relevant boundary segments put in this scale by the outward affine-normalization lemma under that lemma's hypotheses.

## Facts & Assumptions

[F1] Under its exterior-containment and outside-tube endpoint hypotheses, the outward affine-normalization lemma gives the relevant future source-normal null segments the unique outgoing affine scale $\dot\gamma(0)=n+\nu$, preserving their oriented images. [lem-author-fd27ddabb933-outward-null-affine-normalization](item-lem-author-fd27ddabb933-outward-null-affine-normalization)

[F2] For an affine null geodesic in the stationary metric, $E=-g(T,\dot\gamma)$ is constant, with no timelike assumption on $T$ along the full segment. Where $T$ is future timelike and the tangent is future null, $E$ is strictly positive. [lem-author-fd27ddabb933-killing-energy-conservation](item-lem-author-fd27ddabb933-killing-energy-conservation)

[F3] The spacelike-hypersurface data specify the smooth future unit normal $n_\Sigma$ and the smooth positive induced metric $h=g|_{T\Sigma}$. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F4] Stationary Lorentzian data supply the smooth metric $g$, its time orientation and Levi–Civita connection, and the smooth Killing field $T$. A designated stationary end requires $T$ to be future timelike there. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F5] For the supplied smooth unit normal $\nu_0$ on compact $S$, the graph-domain lemma supplies a Riemannian normal tube and a smooth embedded spacelike graph $F_\epsilon$ for every sufficiently small $\epsilon$ in the fixed smooth family $u=\epsilon\phi$. [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain)

[F6] On an admissible graph in that tube, the canonical outward graph gauge supplies the smooth unit normal $\nu$ tangent to $\Sigma$, normal to $A$ and positively paired with the increasing tube direction. The field $n+\nu$ is a nonzero future null normal. [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)

[F7] A smooth map between smooth manifolds is continuous; this applies to the smooth graph parametrization and to the smooth real-valued contraction of the supplied fields. [math:prop-smooth-maps-are-continuous](https://alphabetamath.cc/item/prop-smooth-maps-are-continuous)

[F8] A continuous image of a compact space is compact (claim 1). A continuous real-valued function on a nonempty compact space attains a maximum and a minimum (claim 2). [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

[A1] Work in ZFC, including the countable and dependent choice required by the invoked geodesic, compactness and causal interfaces. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The fixed stationary, hypersurface and graph data and the segment hypotheses in the Statement.

**Goal:** Establish the finite source maximum and the positive target-independent energy bound.

1.1 By [F3] and [F5], the chosen $F_\epsilon:S\to\Sigma$ is a smooth embedded graph parametrization, so it is continuous by [F7]. Claim 1 of [F8] applied to the compact domain $S$ makes $A=F_\epsilon(S)$ compact. Since $S$ is nonempty, its image $A$ is nonempty. The hypotheses of [F6] hold for this admissible graph in the supplied tube, so $n$ and $\nu$ are smooth along $A$ and $n+\nu$ is its specified future null normal. [F3, F5, F6, F7, F8, given]

2.1 The real-valued contraction $q(p)=g_p(T_p,n_p+\nu_p)$ is smooth on $A$: in any surface chart its expression is a finite sum of products of the smooth restricted metric and field coefficients supplied by [F3], [F4] and [F6]. It is continuous by [F7]. The inequality $\bigl||a|-|b|\bigr|\le|a-b|$ shows that $f(p)=|q(p)|$ is continuous as well. Apply claim 2 of [F8] to $f:A\to\mathbb R$ on the nonempty compact space from step 1.1. It attains a finite maximum $m\ge0$, so $E_{\max}=1+m>0$. Its defining data are fixed before a target or segment is selected. [F3, F4, F6, F7, F8, step 1.1, algebra]

3.1 For any segment in the Statement, its initial normalization gives $E(0)=-q(\gamma(0))$, hence $|E(0)|\le m<E_{\max}$ by step 2.1. The stationary data in [F4] and the affine null-segment hypotheses permit [F2], so $E$ is constant. At $\gamma(b)\in U$, the field $T$ is future timelike and the tangent is future null, so [F2] gives $E(b)>0$. Thus $0<E\le E_{\max}$ everywhere, without requiring $T$ timelike away from the end. The same estimate applies to the boundary segments normalized by [F1] whenever its hypotheses hold. No target radius or target translate enters the source maximum. [F1, F2, F4, step 2.1, given, algebra] ∎

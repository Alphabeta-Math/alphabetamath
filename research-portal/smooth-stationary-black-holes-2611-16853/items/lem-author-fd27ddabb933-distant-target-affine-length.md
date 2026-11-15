---
id: lem-author-fd27ddabb933-distant-target-affine-length
title: Distant targets force arbitrarily long source-normalized affine segments
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-fd27ddabb933-asymptotic-null-energy-speed
  - lem-author-fd27ddabb933-compact-source-energy-bound
  - math:def-axiom-of-choice
  - def-stationary-lorentzian-data
  - def-spacelike-maximal-hypersurface-data
  - lem-author-fd27ddabb933-outward-null-affine-normalization
  - math:prop-smooth-maps-are-continuous
  - math:thm-continuity-characterisations-top
  - math:thm-heine-borel-r
  - math:thm-closed-subspace-of-a-compact-space-is-compact
  - math:thm-compactness-under-continuous-maps
  - math:cor-mean-value-theorem
  - math:def-interior-closure-boundary-top
  - math:def-geodesic-of-an-affine-connection
  - physics:def-time-orientation-and-future-causal-sets
dependency_roles:
  lem-author-fd27ddabb933-asymptotic-null-energy-speed: mathematical-premise
  lem-author-fd27ddabb933-compact-source-energy-bound: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  lem-author-fd27ddabb933-outward-null-affine-normalization: mathematical-premise
  math:prop-smooth-maps-are-continuous: mathematical-premise
  math:thm-continuity-characterisations-top: mathematical-premise
  math:thm-heine-borel-r: mathematical-premise
  math:thm-closed-subspace-of-a-compact-space-is-compact: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
  math:def-interior-closure-boundary-top: mathematical-premise
  math:def-geodesic-of-an-affine-connection: mathematical-premise
  physics:def-time-orientation-and-future-causal-sets: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 8
---

## Statement

Work in ZFC with stationary Lorentzian data $(M,g,N,T)$ of signature $(-,+,+,+)$ and Levi–Civita connection $\nabla$. Let $\mathcal E\subset M$ be an open exterior and supply a stationary end chart $(t,x):U\longrightarrow I\times\{x\in\mathbb R^3:|x|>R_0\}$ with $U\subset\mathcal E$, $I$ a nonempty open interval and $R_0>0$. Write $r=|x|$. Assume the coordinate metric matrix tends uniformly to $\operatorname{diag}(-1,1,1,1)$ as $r\to\infty$, that $T=c\partial_t$ for one fixed $c>0$, and that $T$ is future timelike sufficiently far out. Fix $R_*>R_0$ so the end-speed estimate holds on $r>R_*$, with $C=4/c$.

Fix the source data of the compact-source energy bound: a smooth embedded spacelike hypersurface $\Sigma$ with induced metric $h$ and smooth future unit normal $n_\Sigma$; a nonempty compact smooth embedded two-surface $S\subset\operatorname{int}\Sigma$ without boundary, with a supplied smooth outward $h$-unit normal $\nu_0$ tangent to $\Sigma$; a fixed smooth $\phi>0$ on $S$; and one fixed $\epsilon>0$ sufficiently small for its admissible outward normal graph $A=\{\exp_y^h(\epsilon\phi(y)\nu_0(y)):y\in S\}\subset\mathcal E$. On $A$ put $n=n_\Sigma|_A$ and let $\nu$ be the canonical outward unit graph normal tangent to $\Sigma$, with positive pairing with the increasing normal-tube coordinate direction. Set $E_{\max}=1+\max_{p\in A}|g_p(T_p,n_p+\nu_p)|$.

Choose one fixed $R_1>R_*$ enclosing this source in the following precise sense. For $D=\{p\in U:r(p)>R_1\}$ and $\mathcal C_{R_1}=\{p\in U:r(p)=R_1\}$ require $A\cap\overline D^{\mathcal E}=\varnothing$ and $\partial_{\mathcal E}D=\mathcal C_{R_1}$, where closure and boundary are taken in $\mathcal E$. Thus the outer region is covered by the end chart and has no additional boundary in the exterior through which a segment could enter it.

For every future-directed affinely parametrized null geodesic $\gamma:[0,\ell]\to\mathcal E$, with $\ell>0$, $\gamma(0)\in A$, $\dot\gamma(0)=n+\nu$ at its source point, and $\gamma(\ell)\in U$ at radius $R>R_1$, its source-normalized affine length satisfies $\ell\ge(R-R_1)/(CE_{\max})$. Consequently the lengths of such segments are unbounded as their target radii tend to infinity, even if they leave and reenter the asymptotic region before the final passage. The end, source graph, $R_1$, $C$ and $E_{\max}$ remain fixed while targets vary; no null-geodesic completeness is assumed.

## Facts & Assumptions

[F1] For the supplied stationary chart, uniform Minkowski limit and $T=c\partial_t$ with its future end orientation, the end-speed lemma supplies $R_*$ and $C=4/c$ such that $T$ is future timelike and $|dr/d\lambda|\le CE$ for every future null tangent at $r>R_*$. Its energy is $E=-g(T,\dot\gamma)$. [[lem-author-fd27ddabb933-asymptotic-null-energy-speed]]

[F2] For the fixed compact outward graph and exact initial tangent $n+\nu$ specified in the Statement, the compact-source lemma makes $E_{\max}$ finite and positive. Every such affine future null segment arriving where $T$ is future timelike has constant energy $0<E\le E_{\max}$, without requiring $T$ timelike in the inner region. [[lem-author-fd27ddabb933-compact-source-energy-bound]]

[F3] Stationary Lorentzian data specify the smooth metric, time orientation, Killing field and Levi–Civita connection. Spacelike-hypersurface data specify $h$ and the smooth future unit normal $n_\Sigma$. [[def-stationary-lorentzian-data]] [[def-spacelike-maximal-hypersurface-data]]

[F4] The outgoing affine scale is exactly $\dot\gamma(0)=n+\nu$. The outward affine-normalization lemma supplies this scale for source-normal boundary segments when its small-graph, exterior-containment and outside-tube endpoint hypotheses hold. Here that exact scale is a hypothesis on the segments, rather than an assertion that every null segment can be so normalized. [[lem-author-fd27ddabb933-outward-null-affine-normalization]]

[F5] Smooth maps are continuous, so the smooth geodesic and the end radial function are continuous. A continuous map has closed preimages of closed sets and maps the closure of a subset into the closure of its image. [[math:prop-smooth-maps-are-continuous]] [[math:thm-continuity-characterisations-top]]

[F6] The interval $[0,\ell]$ is compact; a closed subspace of a compact space is compact; and a continuous real-valued function on a nonempty compact space attains its maximum. [[math:thm-heine-borel-r]] [[math:thm-closed-subspace-of-a-compact-space-is-compact]] [[math:thm-compactness-under-continuous-maps]]

[F7] For a real function continuous on $[a,b]$ and differentiable on $(a,b)$ with $a<b$, the mean value theorem gives $f(b)-f(a)=f'(s)(b-a)$ for some $s\in(a,b)$. [[math:cor-mean-value-theorem]]

[F8] For an open subset $D$ of $\mathcal E$, its relative boundary is $\partial_{\mathcal E}D=\overline D^{\mathcal E}\setminus D$. [[math:def-interior-closure-boundary-top]]

[F9] An affinely parametrized geodesic is a smooth curve satisfying $D_\lambda\dot\gamma=0$, with one-sided interpretation at included endpoints. At each $p$, use the Lorentz vector space $(T_pM,g_p)$ and the timelike component containing $N_p$; future null tangents are nonzero null vectors in its closure. [[math:def-geodesic-of-an-affine-connection]] [[physics:def-time-orientation-and-future-causal-sets]]

[A1] Work in ZFC, including the countable and dependent choice required by the invoked geodesic, compactness and causal interfaces. [[math:def-axiom-of-choice]]

## Proof

**Given:** The fixed geometric data, enclosing radius and source-normalized segment in the Statement.

**Goal:** Prove the affine-length estimate and its unbounded-growth consequence.

1.1 The stationary and source structures in [F3] are exactly those required by [F2], and the segment has its specified outgoing scale by hypothesis and [F4]. Its endpoint has $r=R>R_1>R_*$, so [F1] makes $T$ future timelike there. Hence [F2] applies and gives a constant $E$ with $0<E\le E_{\max}$ along the full segment. These constants depend only on the one fixed end and source graph. [F1, F2, F3, F4, F9, A1, given]

1.2 Since $D$ is open in $\mathcal E$, the set $K=\gamma^{-1}(\mathcal E\setminus D)$ is closed in $[0,\ell]$ by continuity and [F5]. The source-separation hypothesis gives $0\in K$, while the endpoint condition gives $\ell\notin K$. By [F6], $K$ is nonempty and compact, and its continuous inclusion into $\mathbb R$ attains a maximum $a$. Thus $0\le a<\ell$, $\gamma(a)\notin D$, and $\gamma((a,\ell])\subset D$. [F5, F6, given, construct]

2.1 The point $a$ lies in the closure of $(a,\ell]$ in $[0,\ell]$. The closure-image property in [F5] therefore puts $\gamma(a)$ in $\overline D^{\mathcal E}$. Since $\gamma(a)\notin D$, [F8] and the specified boundary identity give $\gamma(a)\in\partial_{\mathcal E}D=\mathcal C_{R_1}$. In particular $\gamma([a,\ell])\subset U$, $r(\gamma(a))=R_1$, and $r(\gamma(\lambda))>R_1$ for $a<\lambda\le\ell$. This constructs a final end passage using only the already existing finite segment, regardless of its earlier excursions. [F5, F8, step 1.2, given]

3.1 The function $f=r\circ\gamma$ is continuous on $[a,\ell]$ and differentiable on $(a,\ell)$, because the segment is smooth and lies in the end chart there. The chart and null-tangent hypotheses of [F1] hold throughout this last passage, where $r\ge R_1>R_*$. Thus $|f'|\le CE\le CE_{\max}$ by step 1.1. Applying [F7] gives $R-R_1=f(\ell)-f(a)\le CE_{\max}(\ell-a)\le CE_{\max}\ell$. Division by the fixed positive $CE_{\max}$ proves the stated estimate, whose right side tends to infinity with $R$. [F1, F5, F7, F9, step 1.1, step 2.1, algebra] ∎

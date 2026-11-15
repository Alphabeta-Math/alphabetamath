---
id: lem-author-e7cde3233cd7-spherical-cauchy-portion
title: Identifying the spherical Cauchy portion without a stationary lapse
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - math:def-axiom-of-choice
  - lem-author-e7cde3233cd7-cauchy-section-product
  - lem-author-e7cde3233cd7-one-sided-boundary-exclusion
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-causal-curve-calculus
  - math:lem-ac-supplies-countable-and-dependent-choice-for-banach-integration
  - math:cor-euclidean-spheres-are-path-connected
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:ex-the-n-sphere-with-its-standard-smooth-atlas
  - math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure
  - math:def-connected-space
  - math:def-connected-component-and-quasicomponent
  - math:def-path-connected
  - math:thm-path-connected-implies-connected
  - math:thm-continuous-image-of-a-connected-space
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  lem-author-e7cde3233cd7-cauchy-section-product: mathematical-premise
  lem-author-e7cde3233cd7-one-sided-boundary-exclusion: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  math:lem-ac-supplies-countable-and-dependent-choice-for-banach-integration: mathematical-premise
  math:cor-euclidean-spheres-are-path-connected: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:ex-the-n-sphere-with-its-standard-smooth-atlas: mathematical-premise
  math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure: mathematical-premise
  math:def-connected-space: mathematical-premise
  math:def-connected-component-and-quasicomponent: mathematical-premise
  math:def-path-connected: mathematical-premise
  math:thm-path-connected-implies-connected: mathematical-premise
  math:thm-continuous-image-of-a-connected-space: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references: []
dependency_level: 3
---

## Statement

Work in ZFC. Let $(D,g,N)$ be a time-oriented smooth Lorentzian four-manifold, and let $U\subset D$ be a connected nonempty open region containing a specified spacelike end section $S_{\rm ext}\subset U$ with a diffeomorphism $e:\{x\in\mathbb R^3:|x|>R\}\to S_{\rm ext}$, where $R>0$. Let $\Sigma\subset D$ be a smooth embedded hypersurface. Put $E=I_D^-(U)\cap I_D^+(U)$ and suppose $E$ is globally hyperbolic and $C=\Sigma\cap E$ is a smooth spacelike Cauchy hypersurface of $E$. Suppose there is a specified diffeomorphism $\chi:\{|x|>1/2\}\to\Sigma$ and a number $\rho>\max\{1,R\}$ such that $\chi(x)=e(x)$ for every $|x|>\rho$. This equality specifies the far-out agreement with the end section; in a stationary-end presentation, $S_{\rm ext}$ is the supplied zero-time section. Suppose $S=\partial_D I_D^-(U)\cap\partial_D I_D^+(U)$ lies in $\Sigma$ and equals $\chi(\{|x|=1\})$. Then $C=\chi(\{|x|>1\})$, and $E$ is diffeomorphic to $\mathbb R\times(1,\infty)\times S^2$.

## Facts & Assumptions

[F1] The Lorentzian, chronological, ambient-boundary, end-section and relative Cauchy conventions are those of [[def-causal-exterior-and-boundary-data]]. Work in ZFC, including [[math:def-axiom-of-choice]]. The section $S_{\rm ext}$ and its chart are supplied data, and its containment in $U$ is explicit in the Statement; for stationary-end data this containment also follows from $\Phi(0,p)=p$.

[F2] A connected nonempty globally hyperbolic domain is diffeomorphic to the product of $\mathbb R$ with its prescribed smooth spacelike Cauchy hypersurface, and that hypersurface is connected. [[lem-author-e7cde3233cd7-cauchy-section-product]]

[F3] If a Cauchy hypersurface of $E=I_D^-(U)\cap I_D^+(U)$ has an ambient limit point outside $E$, that point lies on both ambient chronological boundaries. [[lem-author-e7cde3233cd7-one-sided-boundary-exclusion]]

[F4] Chronological futures and pasts of points are open, by clause (a) of [[physics:lem-gr-chronology-openness]]. Chronological futures and pasts of a set are their unions over its points.

[F5] Smooth future timelike arcs are admissible timelike curves, finite concatenations of timelike curves remain timelike, and increasing affine reparametrizations preserve the curve class, by clauses (c), (d) and (e) of [[physics:lem-gr-causal-curve-calculus]]. Restricting a timelike curve to a nondegenerate closed subinterval preserves local absolute continuity and the almost-everywhere future timelike velocity condition of [F1].

[F6] In ZF, AC implies Countable Choice and prescribed-initial-point Dependent Choice by [[math:lem-ac-supplies-countable-and-dependent-choice-for-banach-integration]]. Thus the ZFC assumption supplies the choice hypotheses of [F4] and [F5], as well as those inherited by [F2] and [F3].

[F7] For $n\ge2$, the unit sphere $S^{n-1}\subset\mathbb R^n$ is path connected and connected, by [[math:cor-euclidean-spheres-are-path-connected]]. Apply this with $n=3$.

[F8] A diffeomorphism is a bijective smooth map with smooth inverse; in particular it is a homeomorphism, as in [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]. This convention applies to $e$, $\chi$ and the asserted product identifications.

[F9] The sphere $S^2$ has the standard smooth atlas of [[math:ex-the-n-sphere-with-its-standard-smooth-atlas]], with stereographic charts $\sigma_N(\omega)=(\omega_1,\omega_2)/(1-\omega_3)$ and $\sigma_S(\omega)=(\omega_1,\omega_2)/(1+\omega_3)$ away from their respective poles.

[F10] Products carry the canonical product smooth structure, whose charts are products of factor charts, by [[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure]]. This applies to the products in the Statement and the proof.

[F11] Connectedness, separations, connected subsets and clopen subsets have the meanings of [[math:def-connected-space]]. Connected components are the largest connected subsets through their points, as defined in [[math:def-connected-component-and-quasicomponent]]. A nonempty clopen subset of a connected space is the whole space: otherwise it and its complement form a separation.

[F12] Paths and path-connected subsets have the meanings of [[math:def-path-connected]]. The unit interval $[0,1]$ is connected, and every path-connected space or subset is connected, by claims 1 and 2 of [[math:thm-path-connected-implies-connected]].

[F13] A continuous image of a connected space is connected, and a homeomorphism preserves connectedness, by claims 1 and 2 of [[math:thm-continuous-image-of-a-connected-space]].

## Proof

**Given:** The geometric and end-section data in the Statement, in ZFC, and the declared mathematical supplier interfaces.

**Goal:** Identify $C$ and give the stated diffeomorphism type of $E$.

1.1 By [F6], the choice assumptions of the suppliers are satisfied. Put $P=I_D^-(U)$ and $Q=I_D^+(U)$. By [F4] both are unions of open chronological sets, so $E=P\cap Q$ is open. To check $U\subset E$, fix $u\in U$, choose a coordinate chart $y$ with $y(u)=0$, and put $v=dy_u(N_u)$. The smooth arc $\beta(t)=y^{-1}(tv)$ has future timelike tangent at $0$. Continuity of the metric, tangent and orientation field makes it future timelike on a sufficiently small interval $[-\varepsilon,\varepsilon]$, whose image lies in $U$ by openness. Its two halves are admissible by [F5], and show $\beta(-\varepsilon)\ll_D u\ll_D\beta(\varepsilon)$, hence $u\in P\cap Q$. Thus $E$ is nonempty. In particular, the specified far-out section $\chi(\{|x|>\rho\})=e(\{|x|>\rho\})$ lies in $\Sigma\cap U\subset C$. [given, F1, F4, F5, F6]

2.1 For $p\in E$, choose $u,v\in U$ with $u\ll_D p\ll_D v$, and let $\gamma$ be a timelike curve from $u$ to $p$. At any interior point $z$ of $\gamma$, restriction as in [F5] gives $u\ll_D z\ll_D p$. Concatenating the latter segment with a curve from $p$ to $v$, using [F5], gives $z\ll_D v$. Thus $z\in Q\cap P$. Both endpoints also lie in $E$ by step 1.1 and the choice of $p$, so the whole connecting curve lies in $E$. After an increasing affine reparametrization as in [F5], this is a path on $[0,1]$ in the sense of [F12]. Its image is connected by the connectedness of $[0,1]$ in [F12] and the continuous-image theorem [F13]. If $E$ had a separation in the sense of [F11], connectedness of $U\subset E$ would put $U$ on one side, while any point on the other side would have this connecting path to $U$, contradicting connectedness of a continuous path image. Hence $E$ is connected. Applying [F2] now gives connectedness of $C$ and a diffeomorphism $\mathbb R\times C\to E$. [given, F1, F2, F5, F6, F11, F12, F13, step 1.1]

3.1 Since $E$ is open, $C$ is open in $\Sigma$. A point of its relative boundary in $\Sigma$ is therefore outside $C$; since it lies in $\Sigma$, it is outside $E$, but is an ambient limit point of $C$. By [F3] it lies in $S$. No point of $S$ lies in $E$, because a boundary point of either open set $P$ or $Q$ is outside that set. Consequently $C$ is contained in $\Sigma\setminus S$ and is both open and closed there. Since $\chi$ is a homeomorphism by [F8], connectedness is preserved by [F13]. In the domain of $\chi$ the complement of the unit sphere has the two connected components, in the sense of [F11], $1/2<|x|<1$ and $|x|>1$: each radial annulus is path connected by radial paths and paths on the unit sphere supplied by [F7], hence connected by [F12]. The continuous radius function separates the two annuli by the omitted value $1$, so they are complementary clopen subsets of that complement. A connected subset cannot meet both, since the two intersections would separate it; thus each annulus is a largest connected subset through any of its points, as required by [F11]. Step 1.1 puts the nonempty far-out subset $\chi(\{|x|>\rho\})$ in $C$, so $C$ meets the outer component in a nonempty clopen subset. The consequence in [F11] makes this intersection the whole connected outer component, so that component lies in $C$. Connectedness of $C$ from step 2.1 excludes the inner component. Thus $C=\chi(\{|x|>1\})$. [given, F1, F3, F4, F7, F8, F11, F12, F13, step 1.1, step 2.1]

4.1 Equip $S^2$ with [F9]'s atlas and all products with [F10]'s product structure. On $\{|x|>1\}$ the polar map $P(x)=(|x|,x/|x|)$ is a bijection with inverse $J(r,\omega)=r\omega$, for $r>1$. To check smoothness in the product charts, put $r=|x|=\sqrt{x_1^2+x_2^2+x_3^2}$. In the north and south stereographic charts the coordinate expressions of $P$ are respectively $(r,(x_1,x_2)/(r-x_3))$ and $(r,(x_1,x_2)/(r+x_3))$. The denominators are nonzero on the respective chart preimages, and $r>1$, so both expressions are smooth there. Conversely, writing $u\in\mathbb R^2$ and $q=|u|^2$, the expressions of $J$ in the two source product charts are $r(2u/(1+q),(q-1)/(1+q))$ and $r(2u/(1+q),(1-q)/(1+q))$, which are smooth since $1+q>0$. Thus $P$ and $J$ are smooth mutually inverse maps in the sense of [F8]. Step 3.1 and the given diffeomorphism $\chi$ identify $C$ with $(1,\infty)\times S^2$. Taking the product with the identity on $\mathbb R$ and composing with the diffeomorphism in step 2.1 gives $E\cong\mathbb R\times(1,\infty)\times S^2$; these compositions and the reassociation of product factors are smooth in [F10]'s product charts. [given, F2, F8, F9, F10, step 2.1, step 3.1] ∎

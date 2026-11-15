---
id: lem-author-40aff34b4a4e-spherical-exterior-and-positive-lapse
title: Identification of the spherical exterior and its positive stationary lapse
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - def-stationary-lorentzian-data
  - def-spacelike-maximal-hypersurface-data
  - def-author-4cb89398a4ab-asymptotically-stationary-end
  - lem-author-40aff34b4a4e-chronological-exterior-connectivity
  - lem-author-40aff34b4a4e-cauchy-boundary-exclusion
  - lem-author-40aff34b4a4e-cauchy-timelike-flow-product
  - thm-maximal-jacobi-lapse-input
  - lem-exterior-lapse-maximum-and-boundary-control
  - math:def-axiom-of-choice
  - math:def-connected-component-and-quasicomponent
  - math:thm-connectedness-characterisations
  - math:cor-euclidean-spheres-are-path-connected
  - math:thm-path-connected-implies-connected
  - math:lem-adjugate-inverse-formula-over-a-field
  - math:cor-heine-borel-in-the-product-topology
  - def-exterior-weighted-elliptic-data
  - physics:lem-gr-chronology-openness
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  lem-author-40aff34b4a4e-chronological-exterior-connectivity: mathematical-premise
  lem-author-40aff34b4a4e-cauchy-boundary-exclusion: mathematical-premise
  lem-author-40aff34b4a4e-cauchy-timelike-flow-product: mathematical-premise
  thm-maximal-jacobi-lapse-input: mathematical-premise
  lem-exterior-lapse-maximum-and-boundary-control: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-author-4cb89398a4ab-asymptotically-stationary-end: mathematical-premise
  math:def-connected-component-and-quasicomponent: mathematical-premise
  math:thm-connectedness-characterisations: mathematical-premise
  math:cor-euclidean-spheres-are-path-connected: mathematical-premise
  math:thm-path-connected-implies-connected: mathematical-premise
  math:lem-adjugate-inverse-formula-over-a-field: mathematical-premise
  math:cor-heine-borel-in-the-product-topology: mathematical-premise
  def-exterior-weighted-elliptic-data: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 6
---

## Statement

Work in ZFC. Let $(D,g,T)$ be smooth time-oriented stationary Lorentzian data, and let $U\subset D$ be a nonempty connected open stationary region. Require that the flow of $T$ restricts to a smooth global flow $\Phi:\mathbb R\times U\to U$. No causal character of $T$ on all of $U$ is required. Take all chronological relations and boundaries in $D$, and set $A=I_D^-(U)$, $B=I_D^+(U)$ and $E=A\cap B$.

Suppose $E$ is globally hyperbolic and $C=\Sigma\cap E$ is a smooth spacelike Cauchy hypersurface of $E$, where $\Sigma\subset D$ is smooth and spacelike with a specified diffeomorphism $\Sigma\cong\{x\in\mathbb R^3:r=|x|>1/2\}$. Assume $\varnothing\ne U\cap\Sigma\subset\{r>1\}$ and $S=\partial_D A\cap\partial_D B=\{r=1\}\subset\Sigma$. Then $C=\{r>1\}$.

Suppose additionally that the smooth outer portion $\{r\ge1\}\subset\Sigma$ is maximal, $\operatorname{Ric}(g)=0$ along it, and $T$ is tangent to $S$. On an open neighborhood of its full tail $\{r>R\}$ for some $R>1$, supply coordinates $(t,x^1,x^2,x^3)$ with $T=\partial_t$ and $\Sigma=\{t=0\}$ there, whose spatial coordinates agree with the specified identification of $\Sigma$. Require constants $a>0$ and $0<\alpha\le1$ such that $|g_{\mu\nu}-\eta_{\mu\nu}|\le a r^{-\alpha}$ for $\mu,\nu\in\{0,1,2,3\}$, uniformly on this coordinate neighborhood as $r\to\infty$, where $\eta=\operatorname{diag}(-1,1,1,1)$. Require $T$ to be future timelike sufficiently far out in this chart. With future unit normal $n$, $h=g|_{T\Sigma}$, $k(V,W)=-g(\nabla_Vn,W)$ and $T=Nn+X$, the lapse satisfies $\Delta_hN=|k|_h^2N$, $N|_S=0$, $N\to1$ uniformly at infinity and $0<N<1$ on $C$.

## Statement references

[[def-causal-exterior-and-boundary-data]]

[[def-stationary-lorentzian-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-author-4cb89398a4ab-asymptotically-stationary-end]]

[[lem-author-40aff34b4a4e-chronological-exterior-connectivity]]

[[lem-author-40aff34b4a4e-cauchy-boundary-exclusion]]

[[lem-author-40aff34b4a4e-cauchy-timelike-flow-product]]

[[thm-maximal-jacobi-lapse-input]]

[[lem-exterior-lapse-maximum-and-boundary-control]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice and its countable/dependent-choice consequences. The choice use is inherited through the causal suppliers and the density and temporal-flow construction in the Cauchy-product supplier. [[math:def-axiom-of-choice]]

[F1] The chronological exterior, ambient boundaries and Cauchy condition have the causal interface's meanings; the stationary and hypersurface interfaces supply the Killing field, Ricci convention, future unit normal, induced metric, second fundamental form and lapse decomposition. [[def-causal-exterior-and-boundary-data]] [[def-stationary-lorentzian-data]] [[def-spacelike-maximal-hypersurface-data]]

[F2] For a nonempty connected open stationary region with a smooth global stationary flow, without a causal-character requirement on that flow, the connectivity supplier gives $U\subset E$ and connectedness of $E$. For the stated Cauchy section, boundary exclusion gives $\partial_\Sigma C\subset\partial_D A\cap\partial_D B$, and the globally hyperbolic Cauchy-product supplier gives connectedness of $C$. [[lem-author-40aff34b4a4e-chronological-exterior-connectivity]] [[lem-author-40aff34b4a4e-cauchy-boundary-exclusion]] [[lem-author-40aff34b4a4e-cauchy-timelike-flow-product]]

[F3] The metric bound in the Statement is the zero-order component estimate in clause (1) of the asymptotically stationary end definition. Only that estimate is used; no derivative or Hölder estimate or coordinate existence theorem is invoked. The matching of the spatial coordinates, the full-tail domain, $T=\partial_t$ and $\Sigma=\{t=0\}$ and the future direction of $T$ sufficiently far out are explicit hypotheses here, rather than consequences of the stationary-data definition. [[def-author-4cb89398a4ab-asymptotically-stationary-end]] [[def-stationary-lorentzian-data]]

[F4] On a smooth maximal spacelike hypersurface, a Killing field's lapse obeys $\Delta_hN=(|k|_h^2+\operatorname{Ric}(n,n))N$ with the stated hypersurface and curvature conventions. This is a local identity, imposing no boundary data or end normalization. [[thm-maximal-jacobi-lapse-input]]

[F5] On a connected smooth Riemannian exterior with compact nonempty smooth boundary, a smooth solution of $(\Delta_h-V)u=0$ with $V\ge0$, zero boundary values and uniform limit $1$ at infinity satisfies $0<u<1$ in the interior. [[lem-exterior-lapse-maximum-and-boundary-control]] The exterior, compact-core, end-chart and Laplacian conventions are those of [[def-exterior-weighted-elliptic-data]]; no weighted norm estimate is needed here.

[F6] A component is the largest connected subset through a point. In a connected space the only clopen subsets are the empty set and the whole space. The unit sphere in $\mathbb R^3$ is path connected, and a path-connected space is connected. [[math:def-connected-component-and-quasicomponent]] [[math:thm-connectedness-characterisations]] [[math:cor-euclidean-spheres-are-path-connected]] [[math:thm-path-connected-implies-connected]]

[F7] For a square matrix $M$ over a field with $\det M\ne0$, the inverse is $M^{-1}=\operatorname{adj}(M)/\det M$. Here the field is $\mathbb R$ and the matrix size is four. [[math:lem-adjugate-inverse-formula-over-a-field]]

[F8] In $\mathbb R^3$ with its Euclidean topology, every closed bounded subset is compact. [[math:cor-heine-borel-in-the-product-topology]]

[F9] On a time-oriented smooth Lorentzian four-manifold, the chronological future $I_D^+(u)$ and past $I_D^-(u)$ of every point $u$ are open. Clause (a) of the chronological-openness supplier applies with the locally absolutely continuous timelike-curve convention used here; its Countable Choice and Dependent Choice hypotheses hold in ZFC by [A1]. [[physics:lem-gr-chronology-openness]]

## Proof

**Given:** The stationary-region, Cauchy-section, coordinate and maximality hypotheses in the Statement, in ZFC.

**Goal:** Identify the outer component and prove its lapse equation, boundary value, normalization and strict bounds.

1.1 Apply the chronological-exterior supplier with the nonempty connected open region $U$ and its supplied global flow; no timelikeness of $T$ throughout $U$ is needed. It gives $U\subset E$ and connectedness of $E$. Apply [F9] in $D$: for every $u\in U$, the sets $I_D^-(u)$ and $I_D^+(u)$ are open. By the chronological definitions, $A=\bigcup_{u\in U}I_D^-(u)$ and $B=\bigcup_{u\in U}I_D^+(u)$, so $A$ and $B$ are open as unions of open subsets of $D$, and $E=A\cap B$ is open. In particular $U\cap\Sigma\subset C$, and this section is nonempty and lies in $\{r>1\}$ by hypothesis. The boundary-exclusion supplier applies to the stated Cauchy hypersurface and gives $\partial_\Sigma C\subset S$. Since $A$ and $B$ are open, their boundaries are disjoint from them, so $S\cap C=\varnothing$. [given, A1, F1, F2, F9]

2.1 The set $C$ is open in $\Sigma$ and has no boundary in $\Sigma\setminus S$, hence is both open and closed in $\Sigma\setminus S$. Under the specified diffeomorphism, that space is the disjoint union of the clopen shells $\{1/2<r<1\}$ and $\{r>1\}$. Each shell is path connected: join two points radially to a common radius in its radial interval, join their unit directions by a path in the unit sphere from [F6] at that radius, and concatenate with the reversed radial segment. Each segment stays in the shell, so [F6] makes each shell connected; being disjoint clopen connected sets covering the space, they are exactly its components. Connectedness of $E$ and its global hyperbolicity allow the Cauchy-product supplier to conclude that $C$ is connected. It meets the outer shell through the nonempty set $U\cap\Sigma$; connectedness prevents it from meeting both shells. Its intersection with the outer shell is nonempty and clopen in that connected shell, so [F6] makes it the whole shell. Therefore $C=\{r>1\}$. [given, A1, F1, F2, F6, step 1.1]

3.1 The normal and lapse are smooth on $\{r\ge1\}$, and tangency of $T$ to $S\subset\Sigma$ gives $N=-g(T,n)=0$ on $S$. On the specified end chart the bound in [F3] gives $g_{\mu\nu}\to\eta_{\mu\nu}$ uniformly. The determinant and cofactors are finite polynomials in the matrix entries, so their limits are uniform as well. Thus $\det(g_{\mu\nu})\to\det\eta=-1$ uniformly, and its absolute value is at least $1/2$ sufficiently far out. Applying [F7] to the real $4\times4$ matrix gives $g^{00}\to-1$ uniformly. Since $\Sigma=\{t=0\}$, its unit normal is $n=-\nabla t/\sqrt{-g^{00}}$ on the tail: this sign is future-directed because $T=\partial_t$ is future timelike and $g(-\nabla t,T)=-1$. Consequently $N=dt(T)/\sqrt{-g^{00}}=(-g^{00})^{-1/2}\to1$ uniformly. Coordinate matching makes this the full spatial infinity of $C$; for finite $b\ge1$, the Euclidean annuli $\{x\in\mathbb R^3:1\le|x|\le b\}$ are closed and bounded, hence compact by [F8]. Their images $\{1\le r\le b\}\subset\Sigma$ under the specified diffeomorphism are compact: pulling any open cover back to the compact annulus and taking a finite subcover proves this directly. [given, F1, F3, F7, F8, step 2.1, algebra]

4.1 The local maximal lapse identity in [F4] applies on exactly the outer portion assumed maximal in the Statement. With $\operatorname{Ric}(g)=0$ there it yields $\Delta_hN=|k|_h^2N$. By step 2.1 its closure in $\Sigma$ is the smooth connected Riemannian exterior $\{r\ge1\}$, with smooth metric and compact nonempty boundary $S$. To check the exterior convention in [F5], choose $r_0>R$: the complement of the compact set $\{1\le r\le r_0\}$ is the specified end $\{r>r_0\}$, and its required core $K=\{1\le r\le2r_0\}$ is compact by step 3.1. Its lapse is smooth up to that boundary, its potential $V=|k|_h^2$ is smooth and nonnegative, and step 3.1 supplies zero boundary values and the uniform end limit $1$. Thus every hypothesis of [F5] is satisfied, and the exterior maximum principle gives $0<N<1$ on $C$, completing all conclusions. [given, F1, F4, F5, step 2.1, step 3.1] ∎

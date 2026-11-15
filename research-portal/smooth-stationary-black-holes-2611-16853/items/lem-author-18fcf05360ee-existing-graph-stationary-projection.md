---
id: lem-author-18fcf05360ee-existing-graph-stationary-projection
title: An existing stationary graph supplies global projection before any estimate
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-maximal-graph
  - math:def-local-and-global-flow
  - lem-author-78c700cb9e03-bounded-rapidity-reference-graph
  - lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow
  - def-spacelike-maximal-hypersurface-data
  - lem-author-78c700cb9e03-invariant-normal-boost-coordinates
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:def-smooth-collar-of-a-manifold-boundary
  - math:thm-compactness-under-continuous-maps
  - math:thm-heine-borel-rn
  - math:thm-finite-products-of-compact-spaces
  - math:thm-closed-subspace-of-a-compact-space-is-compact
  - math:def-riemannian-speed-and-length
  - math:thm-cauchy-schwarz-in-an-inner-product-space
  - math:thm-continuous-implies-integrable
  - math:thm-newton-leibniz-with-interior-derivative
  - math:thm-monotonicity-of-the-integral
  - def-stationary-lorentzian-data
dependency_roles:
  def-stationary-maximal-graph: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  lem-author-78c700cb9e03-bounded-rapidity-reference-graph: mathematical-premise
  lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  lem-author-78c700cb9e03-invariant-normal-boost-coordinates: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:def-smooth-collar-of-a-manifold-boundary: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:thm-heine-borel-rn: mathematical-premise
  math:thm-finite-products-of-compact-spaces: mathematical-premise
  math:thm-closed-subspace-of-a-compact-space-is-compact: mathematical-premise
  math:def-riemannian-speed-and-length: mathematical-premise
  math:thm-cauchy-schwarz-in-an-inner-product-space: mathematical-premise
  math:thm-continuous-implies-integrable: mathematical-premise
  math:thm-newton-leibniz-with-interior-derivative: mathematical-premise
  math:thm-monotonicity-of-the-integral: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 5
---

## Statement

Let $D=\mathbb R_t\times C$ be a stationary product with $T=\partial_t$, where $C$ is the connected Euclidean exterior $\{x\in\mathbb R^3:|x|>1\}$. Let the existing section be the global stationary graph $j(x)=(u_*(x),x)$, with smooth $u_*$ on $C$, and write $\Sigma_*^\circ=j(C)$. Then $G_*:\mathbb R\times\Sigma_*^\circ\to D$, $G_*(s,j(x))=(s+u_*(x),x)$, is a diffeomorphism. Hence the stationary projection $\Pi_*:D\to\Sigma_*^\circ$, $\Pi_*(t,x)=j(x)$, exists everywhere without a near-boundary return estimate.

For the collar conclusions, regard the original section as $C$ with its usual smooth compactification $\overline C=\{|x|\ge1\}$ and boundary sphere $S$, and supply a smooth existing section with boundary $\Sigma_*$ whose interior is $\Sigma_*^\circ$ and whose boundary is the same $S$. The sections are spacelike up to $S$ for their respective smooth time-oriented Lorentz metrics, which may coincide, and have positive stationary lapse on their interiors. Assume their common invariant boost collar model has the following data: an actual normal tube at $S$ with commuting local Killing fields $K,Z$, with $K|_S=0$, $Z$ generating a time-oriented circle action $\psi$ preserving $S$, and $T=K-\Omega Z$ for a constant $\Omega$. Each section metric is $T$-stationary on $D$ and makes $K,Z$ Killing on the tube. For each metric, $dK|_S$ annihilates $TS$ and is the positive constant-rate boost of rate $\kappa>0$ on the normal plane, with future time orientation and spatial direction pointing into the exterior section. The tube coordinates are $u=r\sinh(\kappa\tau)$, $v=r\cosh(\kappa\tau)$ in the exterior wedge, with $K=\partial_\tau$, $Z=Z_S$ and $T=\partial_\tau-\Omega Z_S$. The original and existing collars are smooth bounded-rapidity graphs $\tau=a_0(r,y)$ and $\tau=a_*(r,y)$, smooth down to $r=0$, over the same small radial interval and $y\in S$. Thus the phrase common invariant boost collar model includes the local Killing, stationarity and signed boost hypotheses, rather than a claim that the local tube is already complete.

After a common shrinking, the stationary quotient correspondence preserves the model radius $r$ and takes the entire original collar $0<r<r_0$ onto the entire existing collar $0<r<r_0$. On each section its intrinsic distance $\rho_i$ to $S$, computed using all piecewise $C^1$ curves in that section with boundary included, satisfies $c_i r\le\rho_i\le C_i r$ for positive constants. Together with the stationary graph end this gives compact annular truncations of $\Sigma_*^\circ$ between its boundary collar and its exterior end. These are statements for the supplied sections; no uniformity over an unspecified family is asserted.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-stationary-maximal-graph]]

[[math:def-local-and-global-flow]]

[[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

[[def-spacelike-maximal-hypersurface-data]]

[[math:def-smooth-collar-of-a-manifold-boundary]]

[[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]]

[[lem-author-78c700cb9e03-bounded-rapidity-reference-graph]]

[[lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow]]

[[math:thm-compactness-under-continuous-maps]]

[[math:thm-heine-borel-rn]]

[[math:thm-finite-products-of-compact-spaces]]

[[math:thm-closed-subspace-of-a-compact-space-is-compact]]

[[math:def-riemannian-speed-and-length]]

## Facts & Assumptions

[F1] The supplied stationary graph has its embedded graph smooth structure, and the stationary product has the complete translation flow. The graph and flow conventions apply without any assertion of a new maximal section. [[def-stationary-maximal-graph]] [[math:def-local-and-global-flow]]

[F2] The invariant normal boost coordinates give the displayed vector fields and their local orbit law. The bounded-rapidity supplier gives a unique crossing of each formal stationary orbit when the graph has positive stationary lapse and $K$ is future timelike there; the latter condition is established below. With the local Killing and stationarity hypotheses stated above, the saturation supplier identifies the complete formal collar with actual stationary flow. It may be applied to either fixed section metric as a constant metric family. [[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]] [[lem-author-78c700cb9e03-bounded-rapidity-reference-graph]] [[lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow]] [[def-stationary-lorentzian-data]]

[F3] The supplied smooth spacelike sections have smooth positive induced metrics up to $S$, smooth future unit normals, and the stated lapse and intrinsic-distance conventions. A smooth boundary collar is an embedding of $S\times[0,\varepsilon)$ onto a neighborhood of $S$, fixing $S$ at zero. The radial graph collars here are such collars; their radial derivative is inward and transverse to $S$. [[def-spacelike-maximal-hypersurface-data]] [[math:def-smooth-collar-of-a-manifold-boundary]]

[F4] A smooth bijection with smooth inverse is a diffeomorphism, hence a homeomorphism. A continuous image of a compact space is compact, and continuous real functions on nonempty compact spaces attain their extrema. [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]] [[math:thm-compactness-under-continuous-maps]]

[F5] Closed bounded Euclidean annuli and closed finite intervals are compact. Finite products of compact spaces are compact, and a closed subset of a compact space is compact. [[math:thm-heine-borel-rn]] [[math:thm-finite-products-of-compact-spaces]] [[math:thm-closed-subspace-of-a-compact-space-is-compact]]

[F6] The length of a piecewise $C^1$ curve is the sum of the integrals of its Riemannian speeds. Cauchy–Schwarz applies in each positive tangent metric. Continuous functions on closed intervals are Riemann integrable; Newton–Leibniz gives endpoint differences from their continuous derivatives, and monotonicity of the integral integrates pointwise inequalities. [[math:def-riemannian-speed-and-length]] [[math:thm-cauchy-schwarz-in-an-inner-product-space]] [[math:thm-continuous-implies-integrable]] [[math:thm-newton-leibniz-with-interior-derivative]] [[math:thm-monotonicity-of-the-integral]]

## Proof

**Given:** The stationary product and supplied graph, and for the collar clauses all the smooth section, stationary metric and signed common boost data in the Statement.

**Goal:** Establish global projection, full collar correspondence, intrinsic boundary-distance comparison and compact annular truncations.

1.1 The inverse of $G_*$ is $(t,x)\mapsto(t-u_*(x),j(x))$. Both maps are smooth in the graph smooth structure, and composing them in either order gives the identity. Likewise $j^{-1}$ on its image is the smooth spatial projection. Thus $G_*$ and $j:C\to\Sigma_*^\circ$ are diffeomorphisms, and $\Pi_*$ is smooth everywhere. Every stationary orbit meets the existing graph exactly once. This proves global existence of projection before any collar estimate. [F1, F4]

1.2 Write $c_i(r,y)$ for the two radial graph collars, where $i=0,*$. They are smooth down to zero with transverse inward radial derivative by [F3]. At $p=c_i(0,y)$ let $n_i$ be the future unit section normal and let $\nu_i$ be the unit normal to $S$ tangent to the section and pointing into its collar. This $\nu_i$ is constructed by raising the nonzero collar covector $dr$ with the positive induced metric and normalizing; hence it is smooth. Decompose $V_i=\partial_rc_i(0,y)=W_i+b_i\nu_i$ with $W_i\in T_pS$. Since $dr(V_i)=1$ and $dr(\nu_i)>0$, $b_i=1/dr(\nu_i)>0$. The signed boost hypothesis gives $dK_p(V_i)=\kappa b_i n_i$. In finite tube charts, $K|_S=0$ and Newton–Leibniz give $r^{-1}K(c_i(r,y))=\int_0^1\partial_r(K\circ c_i)(sr,y)\,ds$. Continuity on compact collar domains makes this converge uniformly, in chart components, to $\kappa b_i n_i$ as $r\downarrow0$: for a prescribed component error, finitely many neighborhoods of the compact zero-radius slice bound the integrand error uniformly, and [F6] bounds its integral by the same error. The positive continuous $b_i$ have positive minima on compact $S$. Consequently $g_i(K,K)/r^2$ and $g_i(K,n_i)/r$ have uniformly negative limits $-\kappa^2b_i^2$ and $-\kappa b_i$ respectively. After shrinking both collars, $K$ is future timelike there. This verifies, rather than assumes, the extra sign condition needed for the crossing supplier. [given, F2, F3, F4, F5, F6]

1.3 Fix either section, pull its induced metric back by $c_i$, and call the resulting smooth positive metric $h$. Choose $\varepsilon>0$ with the closed radial strip $S\times[0,\varepsilon]$ inside this smooth collar. It is compact by [F5], so [F4] bounds the continuous functions $\sqrt{h(\partial_r,\partial_r)}$ and $\sqrt{h^{-1}(dr,dr)}$ above by finite positive constants $M,L$. Here $h^{-1}$ is the inverse positive matrix in collar coordinates; the contractions are coordinate independent. The fixed-$y$ radial path from zero to $r$ has length at most $Mr$ by [F6]. For any tangent vector $v$, put $w=h^{-1}dr$, so $dr(v)=h(w,v)$; Cauchy–Schwarz gives $|dr(v)|\le L\sqrt{h(v,v)}$. Newton–Leibniz on each smooth piece of a curve in this strip, followed by the pointwise integral comparison and addition over the pieces, therefore gives $|r(\gamma(b))-r(\gamma(a))|\le L\,\operatorname{length}_h(\gamma)$ for every piecewise $C^1$ subcurve there. [F3, F4, F5, F6]

2.1 By the local field formula in [F2], a formal stationary orbit is $(r,\tau+t,\psi_{-\Omega t}y)$, so $r$ is fixed. The positive stationary lapses in the hypotheses and step 1.2 verify all sign hypotheses of the bounded-rapidity supplier for both graphs. Each such orbit therefore meets each graph exactly once for every small $r>0$ and every orbit label. The original graph supplies the complete saturation in [F2], since $T$ is complete by [F1] and each section metric is stationary with the local Killing fields as stipulated. Shrink the radius once more so the bounded rapidities of both graphs, and segments between them, lie in the actual tube. The saturation agrees there with the actual tube and everywhere with actual stationary flow. Thus its formal crossings are actual crossings. Global uniqueness from step 1.1 identifies the crossing of the existing section with $\Pi_*$. Applying the crossings in both directions proves that the entire two small collars correspond, with the same $r$, not merely that a subset of one collar enters the other. The correspondence and its inverse are smooth as restrictions of the global stationary projections. [F1, F2, step 1.1, step 1.2]

3.1 Let $p=c_i(r,y)$ with $0<r<\varepsilon/2$ and consider any piecewise $C^1$ curve in the whole section joining $p$ to any point of $S$. If it reaches $S$ before leaving the strip, step 1.3 bounds its length below by $r/L$. If it leaves first, its initial segment must reach radius $\varepsilon$: the collar is an embedding, and the compact closed strip has no other exit except its zero and outer faces. The length of that segment is at least $(\varepsilon-r)/L\ge r/L$. Reaching the zero face is already reaching $S$. These cases cover curves that later leave and return, and all possible boundary endpoints. Taking the infimum over all such curves and using the radial competitor from step 1.3 proves $r/L\le\rho_i(p)\le Mr$. This is the intrinsic distance on the whole section, not a distance restricted to collar paths. Applying this argument separately to both sections, and using the radius preservation in step 2.1, proves all the distance comparisons. [F3, F5, F6, step 2.1, step 1.3]

4.1 For $\eta>0$ and $R>1+\eta$, the base annulus $A_{\eta,R}=\{1+\eta\le|x|\le R\}$ is compact by [F5], and its continuous graph image $j(A_{\eta,R})$ is compact by [F4]. By step 2.1 a full small original collar $Q_0$ maps under $j=\Pi_*|_C$ onto the full existing collar $Q_*$. Since $Q_0$ is a neighborhood of the compact boundary sphere in the usual compactification of $C$, compactness of that sphere gives an $\eta>0$ with $\{1<|x|<1+\eta\}\subset Q_0$. Explicitly, pull this neighborhood back by $(y,s)\mapsto(1+s)y$; open product neighborhoods of each $(y,0)$ have a finite subcover on the zero slice, and the minimum of their positive widths works. Remove $Q_*$ and the open stationary graph end $j(\{|x|>R\})$ from $\Sigma_*^\circ$. The remainder is closed, is contained in $j(A_{\eta,R})$, and is therefore compact by [F5]. Letting the collars shrink and the end thresholds grow gives the asserted annular truncations: compact escape can occur only toward the boundary collar or the specified stationary graph end. [F1, F3, F4, F5, step 1.1, step 2.1, step 3.1] ∎

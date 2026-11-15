---
id: lem-author-594d78e425ed-truncated-past-height-lipschitz-levels
title: The truncated past height is Lipschitz and has exactly the pulled-back
  cuts as levels
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-594d78e425ed-compact-normal-flow-and-area-distortion
  - lem-author-594d78e425ed-uniform-translated-cut-localization
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-push-up-rule
  - physics:lem-gr-achronal-boundaries-lipschitz-graphs
  - def-truncated-null-boundary-height
  - math:def-countable-choice
  - math:def-dependent-choice
  - math:def-riemannian-speed-and-length
dependency_roles:
  lem-author-594d78e425ed-compact-normal-flow-and-area-distortion: mathematical-premise
  lem-author-594d78e425ed-uniform-translated-cut-localization: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-push-up-rule: mathematical-premise
  physics:lem-gr-achronal-boundaries-lipschitz-graphs: mathematical-premise
  def-truncated-null-boundary-height: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-dependent-choice: mathematical-premise
  math:def-riemannian-speed-and-length: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 7
---

## Statement

Assume Countable Choice and Dependent Choice for the supplied causal-curve results. Use the stationary inside region $W$, its section-zero closed base $B$, the chronological past $P=I^-_E(Q)$ and the common smooth normal-flow collar of the uniform translated-cut localization lemma. Choose the collar width $\eta$ sufficiently small that $\mathcal R=c(S\times[0,\eta])\subset\operatorname{Int}_\Sigma B$, as is possible because $B$ contains a neighborhood of compact $S$, and take the localization data for this collar. Let $\delta_0>0$ be the common localization time bound. There is $0<\delta_*\le\delta_0$ such that, for every $0<\delta\le\delta_*$, define
$$u(x)=\sup(\{-2\delta\}\cup\{z\in[-2\delta,2\delta]:\Psi_zx\in P\}),\qquad x\in\mathcal R.$$
Membership in $P\subset E$ is false on the fixed boundary $S$ outside $E$. For $x,y\in\mathcal R$ let $d_0(x,y)$ be the infimum of the $h_0$-lengths of piecewise $C^1$ paths in $\mathcal R$ joining them, with value $+\infty$ when there is no such path, and put $d_{\mathcal R}(x,y)=\min\{d_0(x,y),1\}$. This is a finite metric inducing the collar topology, including on its boundary and across its possibly distinct connected components.

Then $u$ is globally Lipschitz for $d_{\mathcal R}$ and for the intrinsic path distance on each connected component. It equals $-2\delta$ near $S$ and $2\delta$ near $S_\eta$, and for every $|z|<2\delta$ satisfies
$$\{u=z\}=\Psi_{-z}(D_z),\qquad D_z=\{v=z\}\cap\partial_EP\cap W.$$
For $|z|\le2\delta$, the entire flowed interior collar is inside the cylinder: $\Psi_z(\mathcal R\setminus S)\subset W$. Its remaining boundary points $S$ are fixed by the extended flow and belong to the closed inside region in the smooth completion.

## Statement references

[[lem-author-594d78e425ed-compact-normal-flow-and-area-distortion]]

[[lem-author-594d78e425ed-uniform-translated-cut-localization]]

[[def-truncated-null-boundary-height]]

[[physics:lem-gr-chronology-openness]]

[[physics:lem-gr-push-up-rule|Push-up rule]]

[[physics:lem-gr-achronal-boundaries-lipschitz-graphs]]

[[math:def-countable-choice]]

[[math:def-dependent-choice]]

[[math:def-riemannian-speed-and-length]]

## Facts & Assumptions

[F1] The localization data supply the inside base $B$, the compact cuts $D_z$, their containment in $\Psi_z(\mathcal R\setminus\partial\mathcal R)$, and uniform neighborhoods of $S$ outside $P$ and of $S_\eta$ inside $P$ for $|z|\le2\delta_0$. The additional collar choice $\mathcal R\subset\operatorname{Int}_\Sigma B$ is made in the Statement, rather than inferred from containment of the cuts. [[lem-author-594d78e425ed-uniform-translated-cut-localization]]

[F2] The common smooth normal flow fixes $S$, is future timelike on interior fibers, and in the exterior stationary product is $\Psi_z(x)=(z,\psi_z(x))$, with $\psi_z$ the smooth spatial flow of $-X$. Its common time domain contains the compact collar, and $h_0$ is a smooth positive definite metric up to both collar boundaries. [[lem-author-594d78e425ed-compact-normal-flow-and-area-distortion]]

[F3] Chronological pasts are open past sets. If $p\in\overline P$ then $I^-(p)\subset P$; chronological reachability is transitive, and the push-up rule applies. The boundary $\partial_EP$ is achronal by the time reverse of the open-future-set theorem: locally every point of an open chronological past has a short future timelike segment remaining in that past, so $I^-(P)=P$, as required for that time-reversed application. [[physics:lem-gr-chronology-openness]] [[physics:lem-gr-push-up-rule|Push-up rule]] [[physics:lem-gr-achronal-boundaries-lipschitz-graphs]]

[F4] The truncated supremum, the exterior-relative boundary, the fixed-boundary convention and the inside-restricted cut use the supplied height definitions. [[def-truncated-null-boundary-height]]

[A1] Countable Choice and Dependent Choice are assumed in their set-theoretic senses. They discharge the explicit choice hypotheses of all three causal suppliers in [F3], including their uses below; no physical assumption is made. [[math:def-countable-choice]] [[math:def-dependent-choice]]

[F5] The length of a piecewise $C^1$ path is the sum of the integrals of $\sqrt{h_0(\dot\gamma,\dot\gamma)}$ over its pieces. The path infimum and the truncation defining $d_0$ and $d_{\mathcal R}$ are defined in the Statement; their boundary, component and topology properties are proved below. [[math:def-riemannian-speed-and-length]]

## Proof

**Given:** The collar choice, localization data and choice assumptions in the Statement.

**Goal:** Prove cylinder containment, the exact level identity, and global Lipschitz regularity with the specified distances.

1.1 If $\mathcal R$ is empty all conclusions are vacuous; hence assume it is nonempty. Put $U=\operatorname{Int}_\Sigma B$. In the supplied collar coordinates, compactness of $S$ and openness of $U$ give a uniform positive collar width with $c(S\times[0,\eta])\subset U$; choose this before taking the localization data. The continuous spatial flow satisfies $\psi_0(x)=x$ on compact $\mathcal R\subset U$. The inverse image of $U$ under $(z,x)\mapsto\psi_z(x)$ is open and contains $\{0\}\times\mathcal R$. A finite subcover gives one positive time interval on which $\psi_z(\mathcal R)\subset U$. Reduce $\delta_*\le\delta_0$ so that $|z|\le2\delta_*$ lies in this interval and in the common flow domain. The stationary cylinder's inside is invariant under stationary translation; hence $\Psi_z(\mathcal R\setminus S)\subset W$, while the extended flow fixes $S$. This containment is a separate compactness argument, not a converse to cut localization. [given, F1, F2, F4]

1.2 We verify the distance properties without applying a theorem for a connected boundaryless manifold to the whole collar. At any collar point choose nested coordinate balls, or half-balls at a boundary, with compact larger closure. The smooth positive definite matrix of $h_0$, evaluated on that compact set times the Euclidean unit sphere, has positive minimum $m_i^2$ and finite maximum $M_i^2$. Thus $m_i|w|\le|w|_{h_0}\le M_i|w|$ there. Straight coordinate segments in a convex ball or half-ball have length at most $M_i$ times endpoint displacement. Any path starting at the center and exiting a coordinate radius $r$ has length at least $m_ir$, by integrating up to first exit. These estimates show positivity of $d_0$ on distinct points and equality of its local topology with the manifold topology, also at either boundary. Reversal and concatenation of paths give symmetry and the extended triangle inequality. Piecewise $C^1$ reachability classes are open because balls and half-balls are convex; each such class has open complement. They are therefore precisely the connected components, and compactness leaves only finitely many of them. Consequently $d_0$ is finite within a component and infinite across distinct components. Truncation preserves the triangle inequality since $\min\{a+b,1\}\le\min\{a,1\}+\min\{b,1\}$. It also preserves positivity and all sufficiently small balls. Hence $d_{\mathcal R}$ is a finite metric with the asserted topology and value $1$ between distinct components. [F2, F5, given, construct]

2.1 Fix $x\in\mathcal R\setminus S$. Membership of $\Psi_sx$ in $P$ is an initial interval of slab times, because its vertical curve is future timelike and $P$ is a past set. Openness excludes its upper endpoint when that endpoint is in the open slab. If $u(x)=z$ with $|z|<2\delta$, the supremum property gives members of $P$ on this fiber approaching $\Psi_zx$, which is not itself in $P$, so $\Psi_zx\in\partial_EP$. Conversely, if $\Psi_zx\in\partial_EP$ at an open-slab time, every earlier point of this fiber belongs to $P$ by the chronological-closure property in [F3], and no later one can belong to $P$, since that would put $\Psi_zx$ in $P$. Thus $u(x)=z$. By step 1.1 every such boundary hit lies in $W$ and therefore in $D_z$. By [F1] every point of $D_z$ has a unique preimage in the interior collar. This proves both inclusions in the level identity; points of $S$ give no open-slab level because their height is $-2\delta$. [F1, F2, F3, F4, A1, step 1.1]

3.1 The fixed inner margin in [F1] has no members of $P$ at any slab time, so the supremum is $-2\delta$ there, including $S$ by [F4]. On the fixed outer margin every slab time is in $P$, so the supremum is $2\delta$. Remove smaller such neighborhoods to leave a compact annulus strictly away from both collar boundaries. All nonconstant behavior occurs on this annulus. [F1, F4, step 2.1]

4.1 Cover this compact interior annulus by finitely many smaller spatial coordinate balls with closures in larger convex coordinate balls away from $S$ and $S_\eta$. The maps $(s,y)\mapsto\Psi_s(x(y))$ are smooth flow coordinates: $v=s$ and each spatial flow has smooth inverse. On the compact product of the closed slab and each larger ball, $\partial_s$ is future timelike. Continuity and compactness give $\varepsilon_i>0$ such that $\partial_s+w$ is future timelike for every purely spatial coordinate vector with $|w|<\varepsilon_i$. Thus a coordinate straight segment within this product, with positive time displacement exceeding $K_i$ times its spatial displacement, is future timelike for $K_i=1/\varepsilon_i$. [F2, step 3.1]

5.1 In one smaller ball suppose $u(x(y'))-u(x(y))>K_i|y'-y|$. Choose open-slab times $s,t$ with $u(x(y))<s<t<u(x(y'))$ and $t-s>K_i|y'-y|$; this is possible by the strict inequality, including when a height is clipped to a slab endpoint. By the initial-interval property, $\Psi_sx(y)\notin P$ and $\Psi_tx(y')\in P$. The straight segment of step 4.1 joins the former to the latter by a future timelike curve in $E$, contradicting the past-set property. Interchanging the two points proves $|u(x(y'))-u(x(y))|\le K_i|y'-y|$. Together with the constant neighborhoods from step 3.1 this gives coordinate Lipschitz estimates on a finite cover of the whole collar. [F3, A1, step 2.1, step 3.1, step 4.1]

6.1 Use a finite coordinate cover on which the estimates in step 5.1 or the constant-neighborhood estimates hold and the lower metric bounds in step 1.2 hold. Let $L$ be the maximum of their coordinate Lipschitz constants divided by their positive lower metric bounds, using zero on constant patches. Any piecewise $C^1$ path in $\mathcal R$ has a finite parameter subdivision with each subpath in one such patch. On a subpath, endpoint coordinate displacement is bounded by its Euclidean length, and this length is at most $1/m_i$ times its $h_0$-length. The coordinate Lipschitz estimate and telescoping therefore give $|u(x)-u(y)|\le L L_{h_0}(\gamma)$. Taking the infimum gives $|u(x)-u(y)|\le Ld_0(x,y)$ within each component. If $d_0(x,y)\ge1$, including distinct components, boundedness of the defining supremum gives $|u(x)-u(y)|\le4\delta$. Thus in all cases $|u(x)-u(y)|\le\max\{L,4\delta\}d_{\mathcal R}(x,y)$. This proves global Lipschitz regularity, and steps 1.1, 2.1 and 3.1 give all remaining conclusions. [F4, F5, step 1.1, step 2.1, step 3.1, step 5.1, step 1.2] ∎

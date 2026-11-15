---
id: lem-author-594d78e425ed-uniform-translated-cut-localization
title: Uniform localization of translated past-boundary cuts
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-594d78e425ed-compact-normal-flow-and-area-distortion
  - lem-author-9d607f469119-finite-time-collar-exclusion
  - physics:def-gr-causal-curves-and-reachability
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-push-up-rule
  - math:def-countable-choice
  - math:def-dependent-choice
  - def-causal-exterior-and-boundary-data
  - math:def-interior-closure-boundary-top
  - math:def-subspace-topology-top
  - math:def-compact-space
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:thm-compactness-agrees-with-metric-compactness
  - math:lem-closed-subset-of-a-compact-space-is-compact
  - math:thm-continuous-image-of-a-compact-space-is-compact
  - math:thm-extreme-value-metric
  - math:def-riemannian-distance-on-a-connected-manifold
  - math:def-extended-riemannian-distance-on-a-disconnected-manifold
  - math:thm-the-riemannian-distance-topology-is-the-manifold-topology
  - math:def-distance-from-a-point-to-a-subset
  - math:prop-distance-to-a-nonempty-subset-is-one-lipschitz
dependency_roles:
  lem-author-594d78e425ed-compact-normal-flow-and-area-distortion: mathematical-premise
  lem-author-9d607f469119-finite-time-collar-exclusion: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-push-up-rule: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-dependent-choice: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:def-interior-closure-boundary-top: mathematical-premise
  math:def-subspace-topology-top: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:lem-compactness-of-a-subspace-is-ambient: mathematical-premise
  math:thm-compactness-agrees-with-metric-compactness: mathematical-premise
  math:lem-closed-subset-of-a-compact-space-is-compact: mathematical-premise
  math:thm-continuous-image-of-a-compact-space-is-compact: mathematical-premise
  math:thm-extreme-value-metric: mathematical-premise
  math:def-riemannian-distance-on-a-connected-manifold: mathematical-premise
  math:def-extended-riemannian-distance-on-a-disconnected-manifold: mathematical-premise
  math:thm-the-riemannian-distance-topology-is-the-manifold-topology: mathematical-premise
  math:def-distance-from-a-point-to-a-subset: mathematical-premise
  math:prop-distance-to-a-nonempty-subset-is-one-lipschitz: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 6
---

## Statement

Assume Countable Choice and Dependent Choice for the causal inputs. Use the hypotheses and resulting smooth normal-flow collar of the compact normal-flow lemma in a smooth time-oriented stationary Lorentzian four-manifold $E=\mathbb R_v\times\Sigma^\circ$, with temporal $v$, smooth spacelike section $\Sigma$, nonempty compact boundary $S$, and induced Riemannian metric $h_0$. Use componentwise intrinsic distance $d_{h_0}$, with value $+\infty$ between distinct components, and put $\rho(x)=\inf_{s\in S}d_{h_0}(x,s)$, extended stationarily. Thus components missing $S$ have $\rho=+\infty$. Supply the distance collar $\mathcal R=c(S\times[0,\eta])=\{0\le\rho\le\eta\}$ and normal flow $\Psi_z(x)=(z,\psi_z(x))$ on interior points, and put $S_\eta=c(S\times\{\eta\})$.

Let $B\subset\Sigma$ be compact, with $B=\overline{\operatorname{int}_\Sigma B}^{\,\Sigma}$ and smooth outer boundary $\Gamma=\partial_\Sigma B\subset\Sigma^\circ$. Require $\mathcal R\subset\operatorname{int}_\Sigma B$. Put $\Omega=(\operatorname{int}_\Sigma B)\cap\Sigma^\circ$; the specified cylinder is $\mathcal C=\mathbb R_v\times\Gamma$, assumed timelike, and its inside means precisely $\mathbb R_v\times\Omega$. In particular $B$ is the full closed spatial region used here, rather than an unspecified compact subset of the inside.

Let $Q\subset\mathcal C$ be a nonempty compact target with $\min_Qv>0$, and set $P=I^-_E(Q)$. Identify $x\in\Sigma^\circ$ with $(0,x)\in E$ and assume $B\cap\{\rho\ge b\}\subset P$ for some $0<b<\eta/4$. Suppose $|d\rho/dv|\le C\rho$ for future causal curves whenever $0<\rho<a_0$, for fixed $C\ge0$ and $a_0>0$ within the stationary boundary-distance collar, with $Q$ projecting outside $\{\rho<a_0\}$.

Then there exist $\delta_0>0$ and $0<a<b$ such that for every $|z|\le2\delta_0$ the cut
$$D_z=(\{z\}\times\Omega)\cap\partial_EP$$
is compact and satisfies
$$D_z\subset\Psi_z(\{a/2\le\rho\le\eta/2\})\subset\Psi_z(\mathcal R\setminus\partial\mathcal R).$$
The interior flow collar $\Psi_z(\mathcal R\setminus S)$ is inside $\mathcal C$. There are fixed neighborhoods $U_S,U_\eta$ of $S,S_\eta$, respectively, relative to $\mathcal R$, such that $\Psi_z(U_S)\cap P=\varnothing$ and $\Psi_z(U_\eta)\subset P$ for all these $z$; $S$ itself is excluded from $E$ and hence from $P$.

## Facts & Assumptions

[F1] The supplied smooth distance collar is compact; its normal flow has stationary-coordinate form $\Psi_z(x)=(z,\psi_zx)$ on the interior, with smooth spatial flow and inverse for common small times. The spatial flow preserves $S$. [[lem-author-594d78e425ed-compact-normal-flow-and-area-distortion]]

[F2] A compact finite-time target outside a causal collar cannot be reached from section time zero at distances below the collar exit radius times $e^{-C\max_Qv}$. The same result applies to a stationary translate of the target. [[lem-author-9d607f469119-finite-time-collar-exclusion]]

[F3] Chronological pasts are open past sets in the smooth time-oriented Lorentzian four-manifold, under the stated Countable Choice and Dependent Choice hypotheses. For arbitrary $Q\subset E$, $P=I^-_E(Q)=\{p\in E:\exists q\in Q,\ p\ll_E q\}=\bigcup_{q\in Q}I^-_E(q)$. These are mathematical causal results. [[physics:def-gr-causal-curves-and-reachability]] [[physics:lem-gr-chronology-openness]] [[physics:lem-gr-push-up-rule|Push-up rule]] [[math:def-countable-choice]] [[math:def-dependent-choice]]

[F4] All curves and chronological boundaries are relative to $E$; future temporal $v$ increases along future causal curves. Interior, closure, boundary and relative neighborhoods use the manifold and subspace topologies. [[def-causal-exterior-and-boundary-data]] [[math:def-interior-closure-boundary-top]] [[math:def-subspace-topology-top]]

[F5] Compactness is intrinsic open-cover compactness; the ambient-cover criterion permits finite subcovers. On a compatible metric space this agrees with metric compactness. Closed subsets of compact metric spaces and continuous images of compact metric spaces are compact, and continuous real functions attain extrema on nonempty compact metric spaces. For the metric-space results, use $\widehat d(x,y)=\min(1,d_{h_0}(x,y))$ and $d_E((v,x),(w,y))=|v-w|+\widehat d(x,y)$. Truncation preserves the triangle inequality, and balls of radius less than one lie in a component and give its original topology. The product metric therefore gives the manifold topology on $E$. [[math:def-compact-space]] [[math:lem-compactness-of-a-subspace-is-ambient]] [[math:thm-compactness-agrees-with-metric-compactness]] [[math:lem-closed-subset-of-a-compact-space-is-compact]] [[math:thm-continuous-image-of-a-compact-space-is-compact]] [[math:thm-extreme-value-metric]]

[F6] Intrinsic distance induces the manifold topology on each component, including at the boundary. Components are open. On a component meeting $S$, $\rho$ is finite and $1$-Lipschitz, hence continuous; on a component missing $S$ it is $+\infty$. Thus each threshold set $\{\rho\ge r\}$ is closed and $\{\rho<r\}$ is open for finite $r>0$. [[math:def-riemannian-distance-on-a-connected-manifold]] [[math:def-extended-riemannian-distance-on-a-disconnected-manifold]] [[math:thm-the-riemannian-distance-topology-is-the-manifold-topology]] [[math:def-distance-from-a-point-to-a-subset]] [[math:prop-distance-to-a-nonempty-subset-is-one-lipschitz]]

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish compact translated cuts, their uniform annular localization and both endpoint margins.

1.1 By [F6], $L=B\cap\{\rho\ge b\}$ is closed in compact $B$, so [F5] makes it compact. It avoids $S$ and is contained in $P$ at time zero. Write $T_z(x)=(z,x)$. Since $P$ is open, the open section sets $O$ for which some $\epsilon>0$ gives $T_z(O)\subset P$ whenever $|z|<\epsilon$ cover $L$. Take finitely many such sets covering $L$ and, for each of these finitely many sets, one admissible $\epsilon$. Their union $W$ and the positive minimum $\tau$ of these finitely many numbers satisfy $T_z(W)\subset P$ for $|z|<\tau$. This makes no simultaneous choice over all points of $L$. Every $x\in\Omega$ with $\rho(x)\ge b$ belongs to $L$, so none of these points can give a boundary cut. Also $\Gamma\cap\mathcal R=\varnothing$ because $\mathcal R\subset\operatorname{int}_\Sigma B$; hence $\Gamma\subset L\subset W$. Thus this argument controls the entire specified inside and an open neighborhood of its outer boundary. No graph-section compact-core theorem is used. [given, F3, F4, F5, F6]

1.2 Put $V_Q=\max_Qv$, finite by [F5], and choose $0<z_0<\min_Qv/2$. For $|z|\le z_0$, the stationary translate $T_{-z}Q$ is compact, has positive minimum time and maximum time $V_Q-z$, and has the same spatial projection as $Q$. Stationary translation preserves the metric, time orientation and causal curves in $E$, so [F2] applied to $T_{-z}Q$ excludes reachability from $(z,x)$ whenever $0<\rho(x)<a_0e^{-C(V_Q-z)}$. Set $d_*=a_0e^{-C(V_Q+z_0)}>0$ and choose $0<a<\min(b/2,d_*/4)$. The open spacetime region $\{|v|<z_0,\ 0<\rho<d_*\}$ is disjoint from $P$, and therefore also from $\partial_EP$: each of its points has an open neighborhood disjoint from $P$. In particular, all points with $|v|<z_0$ and $0<\rho\le2a$ avoid both $P$ and its boundary. Points of $S$ are separately absent from $E$. [given, F2, F3, F4, F5, F6]

2.1 For $|z|<\min(\tau,z_0)$, steps 1.1 and 1.2 put every cut point in $T_z\{2a<\rho<b\}$. The annulus $A=\{2a\le\rho\le b\}$ is a closed subset of compact $\mathcal R$, hence compact by [F5]. The full annulus lies in $\Omega$ because $A\subset\mathcal R\subset\operatorname{int}_\Sigma B$ and $A\cap S=\varnothing$. Its stationary translate $T_z(A)$ is compact. In fact $D_z=\partial_EP\cap T_z(A)$: localization gives one inclusion, and the other follows from $A\subset\Omega$. The boundary $\partial_EP$ is closed in $E$, so $D_z$ is a closed subset of that compact translated annulus and is compact. This uses the full annulus supplied by the collar, not an annulus inferred from a graph-core result. [given, F1, F4, F5, F6, step 1.1, step 1.2]

3.1 At time zero, $A$ is contained in the open collar annulus $\{a/2<\rho<\eta/2\}$, since $2a>a/2$ and $b<\eta/4$. Smooth inverse-flow dependence and compactness of $A$ keep $\psi_{-z}(A)$ in this annulus for all sufficiently small $|z|$. The spatial inverse-flow identity gives $T_z(A)\subset\Psi_z(\{a/2\le\rho\le\eta/2\})$. This latter closed annulus lies in $\mathcal R\setminus\partial\mathcal R$. Similarly, the open set $\operatorname{int}_\Sigma B$ contains compact $\mathcal R$, so continuity and a finite subcover give a common time interval on which $\psi_z(\mathcal R)\subset\operatorname{int}_\Sigma B$. The spatial flow preserves $S$ and keeps interior points interior by [F1]. Thus the whole interior flow collar stays in $\mathbb R_v\times\Omega$, and the two required localization inclusions follow. [given, F1, F4, F5, F6, step 2.1]

4.1 By continuity of the spatial flow on compact $S$, preservation of $S$ and $\rho|_S=0$, there are a fixed relative neighborhood $U_S$ of $S$ in $\mathcal R$ and a common small time interval with $\rho(\psi_zx)<2a$ for $x\in U_S$. The slice $S_\eta=\mathcal R\cap\{\rho=\eta\}$ is closed in compact $\mathcal R$ and hence compact. By continuity on $S_\eta$, where $\rho=\eta>b$, there are a fixed relative neighborhood $U_\eta$ of $S_\eta$ and a common small time interval with $\rho(\psi_zx)>b$ for $x\in U_\eta$. Step 3.1 keeps these spatial images in $B$. Step 1.2 therefore excludes the interior points of $\Psi_z(U_S)$ from $P$, while step 1.1 puts $\Psi_z(U_\eta)$ in $P$, since its spatial images belong to $L$. The points of $S$ remain outside $P$ by the boundary convention. Choose $\delta_0>0$ so that $|z|\le2\delta_0$ lies strictly within every common time interval just obtained, including $|z|<\min(\tau,z_0)$. This gives both fixed endpoint neighborhoods, compact cuts and the asserted localization uniformly on the closed time range. [given, F1, F4, F5, F6, step 1.1, step 1.2, step 2.1, step 3.1] ∎

---
id: lem-author-2632702918ef-target-interior-focal-exclusion
title: Boundary membership excludes interior focal points from the target
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - def-null-screen-expansion-and-focal-data
  - lem-author-2632702918ef-target-segment-boundary-containment
  - lem-author-2632702918ef-target-endpoint-orthogonality
  - physics:lem-gr-fx-null-focal-boundary-exclusion
  - physics:thm-gr-local-geodesics-and-exponential-map
  - math:def-axiom-of-choice
  - lem-author-2632702918ef-compact-target-causal-endpoint
  - lem-author-2632702918ef-compact-target-null-segment
  - physics:lem-gr-fx-null-normal-plane-and-screen
  - physics:thm-gr-jacobi-equation-and-geodesic-deviation
  - physics:lem-gr-chronology-openness
  - physics:def-gr-metric-selected-connection
  - math:def-topological-space
  - math:thm-choice-implies-dependent-implies-countable-choice
  - math:cor-every-tangent-vector-is-the-velocity-of-a-smooth-curve
  - math:thm-heine-borel-rn
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  lem-author-2632702918ef-target-segment-boundary-containment: mathematical-premise
  lem-author-2632702918ef-target-endpoint-orthogonality: mathematical-premise
  physics:lem-gr-fx-null-focal-boundary-exclusion: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  lem-author-2632702918ef-compact-target-causal-endpoint: mathematical-premise
  lem-author-2632702918ef-compact-target-null-segment: mathematical-premise
  physics:lem-gr-fx-null-normal-plane-and-screen: mathematical-premise
  physics:thm-gr-jacobi-equation-and-geodesic-deviation: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  math:def-topological-space: mathematical-premise
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
  math:cor-every-tangent-vector-is-the-velocity-of-a-smooth-curve: mathematical-premise
  math:thm-heine-borel-rn: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references: []
dependency_level: 5
---

## Statement

For the null segment $\gamma$ in the compact-target hypotheses, reverse its direction and regard it as a past null normal geodesic issued from $c\in C$. There is no focal point to $C$ strictly between $c$ and $p$. Focal points here are rank loss of the normal screen Jacobi map, with the direction and affine parameter reversed from the future convention in the null-screen definition.

## Statement references

[[def-causal-exterior-and-boundary-data]]

[[def-null-screen-expansion-and-focal-data]]

[[lem-author-2632702918ef-compact-target-causal-endpoint]]

[[lem-author-2632702918ef-compact-target-null-segment]]

## Facts & Assumptions

[A1] Work in ZFC. The axiom of choice implies dependent choice and countable choice, supplying the choice assumptions of the geometric and causal suppliers used below. [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]]

[F1] The causal relations, boundary, global hyperbolicity and temporal function are relative to $E$ as in the causal-exterior interface. The metric-selected connection is torsion-free and metric-compatible, so differentiation of metric pairings obeys the product rule. [[def-causal-exterior-and-boundary-data]] [[physics:def-gr-metric-selected-connection]]

[F2] The target surface, null normal congruence, positive screen quotient, normal screen Jacobi map and rank-loss definition of focality have the meanings in the null-screen interface. [[def-null-screen-expansion-and-focal-data]]

[F3] The entire causal segment from $p$ to $c$ lies in $\partial_E I_E^-(C)$ under the compact-target hypotheses specified in [F7]. [[lem-author-2632702918ef-target-segment-boundary-containment]]

[F4] The final tangent of a smooth nonconstant future null affine segment from $p$ to $c\in C$ is orthogonal to $T_cC$ under those hypotheses; global acausality of $C$ is not required. [[lem-author-2632702918ef-target-endpoint-orthogonality]]

[F5] For a smooth null normal geodesic from a smooth spacelike surface without boundary, a normal screen Jacobi field with nonzero initial tangent vector and zero screen value at a positive instant puts points sufficiently shortly afterward in $I^+(C)$. Its equation is $\mathcal D_u^2J+\mathcal R J=0$, where $\mathcal R[Z]=[R(Z,L)L]$; its initial data are $J(0)=[X]$ and $\mathcal D_uJ(0)=B_0X$, with $g(B_0X,Y)=\chi_\ell(X,Y)$ for $X,Y\in T_cC$. Apply this mathematical theorem in $(E,g,-N)$ when reversing time orientation. [[physics:lem-gr-fx-null-focal-boundary-exclusion]]

[F6] The geodesic initial-value problem has a unique smooth maximal solution on an open interval, and its evaluation is smooth on an open time-and-initial-data domain. An included smooth finite endpoint extends by this same initial-value theorem. [[physics:thm-gr-local-geodesics-and-exponential-map]]

[F7] The compact-target hypotheses mean that $(E,g,N)$ is a smooth globally hyperbolic time-oriented Lorentzian four-manifold, $C\subset E$ is a nonempty compact smooth embedded spacelike two-surface without boundary, $\tau$ is temporal, and $p\in\partial_E I_E^-(C)$ satisfies $\tau(p)<\min_C\tau$. Under these hypotheses some $c\in C$ satisfies $p\le_Ec$, $p\ne c$, and $p\notin I_E^-(C)$. [[lem-author-2632702918ef-compact-target-causal-endpoint]]

[F8] Under [F7], there is a nonconstant future null affine segment $\gamma:[0,1]\to E$ from $p$ to some $c\in C$, smooth up to both endpoints and with nonzero tangent. The argument below applies to every such segment. [[lem-author-2632702918ef-compact-target-null-segment]]

[F9] Around every point of a smooth embedded spacelike two-surface there is a smooth normalized pair of future null normals. The normal plane is Lorentzian with exactly two future null rays; selecting a ray and positive rescaling gives a prescribed nonzero vector on that ray. The positive screen metric, screen derivative and symmetric form $\chi_\ell(X,Y)=g(\nabla_X\ell,Y)$ are well-defined. [[physics:lem-gr-fx-null-normal-plane-and-screen]]

[F10] For a smooth variation through affinely parametrized geodesics with tangent $L$ and variation field $V$, $D_uV=D_rL$ and $D_u^2V=R(L,V)L$. These are the geodesic-deviation identities, with the same curvature convention as [F5]. [[physics:thm-gr-jacobi-equation-and-geodesic-deviation]]

[F11] Each chronological past $I_E^-(c)$ is open. Arbitrary unions of open sets are open by topology axiom (T2). [[physics:lem-gr-chronology-openness]] [[math:def-topological-space]]

[F12] Each $X\in T_cC$ is the velocity at zero of a smooth curve in $C$ through $c$, defined on an open interval about zero. [[math:cor-every-tangent-vector-is-the-velocity-of-a-smooth-curve]]

[F13] Closed bounded real intervals are compact: every open cover has a finite subcover. [[math:thm-heine-borel-rn]]

## Proof

**Given:** The data and hypotheses in the Statement, with the compact-target hypotheses and segment made explicit in [F7] and [F8].

**Goal:** Exclude rank loss of the reversed normal screen Jacobi map at every $u\in(0,1)$.

1.1 Put $\delta(u)=\gamma(1-u)$ for $0\le u\le1$ and reverse the time orientation to $-N$. Then $\delta$ is a smooth nonconstant future null affine geodesic in $(E,g,-N)$ starting at $c$, with nonzero normal tangent by [F4] and [F8]. Apply [F9] with this reversed orientation. Interchange the two local null-normal labels if necessary so that $\delta\prime(0)=a\ell_c$ for $a>0$, and replace the local pair $(\ell,k)$ by $(a\ell,a^{-1}k)$. It remains normalized and now $\ell_c=\delta\prime(0)$. This uses only a local field near $c$, not a global normal pair. The choice assumptions of these suppliers follow from [A1]. [A1, F1, F2, F4, F7, F8, F9, given]

2.1 By [F6], extend $\delta$ slightly past both endpoints. The open smooth geodesic-evaluation domain contains its initial state at every time in the interval $[0,1]$, compact by [F13]; a finite subcover therefore gives a neighborhood $U$ of $c$ in $C$ and an open interval $J\supset[0,1]$ on which the geodesics with initial data $(x,\ell_x)$ define a smooth map $F:U\times J\to E$. Uniqueness gives $F(c,u)=\delta(u)$. Each parameter curve is null by metric compatibility and its null initial tangent, has nonzero tangent by uniqueness, and stays future-directed for $-N$ by continuity. For $X\in T_cC$, choose the curve $x(r)$ in [F12] with $x(0)=c$ and $x\prime(0)=X$, and set $V_X(u)=\partial_rF(x(r),u)|_{r=0}$. By [F10], $D_uV_X=D_rL$ and $D_u^2V_X=R(L,V_X)L$, where $L=\partial_uF$. Metric compatibility gives $\frac{d}{du}g(V_X,L)=g(D_rL,L)=\frac12\partial_r g(L,L)=0$. Its initial value is $g(X,\ell_c)=0$, so $V_X$ is orthogonal to $L$ throughout. The same calculation at every $x\in U$ verifies the orthogonality requirement in [F2], hence $F$ is an admissible local null-normal congruence even at rank loss. [step 1.1, F1, F2, F6, F10, F12, F13, construct, algebra]

3.1 Put $J_X=[V_X]=A_uX$ in the positive screen along $\delta$. Projecting the deviation equation from step 2.1 gives $\mathcal D_u^2J_X+\mathcal R J_X=0$ with the convention of [F5], since $R(L,V_X)L=-R(V_X,L)L$. At $u=0$, $J_X(0)=[X]$ and $\mathcal D_uJ_X(0)=[\nabla_X\ell]$. At $c$, normality gives $T_cC\subset\ell_c^\perp$. If $a\ell_c\in T_cC$, its squared norm is zero, so positivity of $g|_{T_cC}$ forces $a\ell_c=0$. Thus the quotient map $\iota:T_cC\to\ell_c^\perp/\mathbb R\ell_c$, $Y\mapsto[Y]$, is injective. Nondegeneracy of the ambient metric and $\ell_c\ne0$ give $\dim\ell_c^\perp=3$, so its quotient by $\mathbb R\ell_c$ has dimension two, equal to $\dim T_cC$; hence $\iota$ is onto. By the quotient metric in [F2], $\bar\gamma(\iota Y,\iota Z)=g(Y,Z)$, so $\iota$ is an isometry. Metric compatibility in [F1] gives $g(\nabla_X\ell,\ell_c)=\frac12X(g(\ell,\ell))=0$, making $[\nabla_X\ell]$ a screen vector. For every $Y\in T_cC$, $\bar\gamma([\nabla_X\ell],\iota Y)=g(\nabla_X\ell,Y)=\chi_\ell(X,Y)=g(B_0X,Y)=\bar\gamma(\iota(B_0X),\iota Y)$. Since $\iota$ is onto and the screen metric is positive definite, $[\nabla_X\ell]=\iota(B_0X)$, which is the identification used in [F5]. Thus $J_X$ has exactly the equation and initial data required in [F5]. In particular rank loss of $A_{u_0}$ supplies $X\ne0$ with $J_X(u_0)=0$, which is a focal instant in that theorem's sense. [step 2.1, F1, F2, F5, F9, F10, algebra]

4.1 Suppose $u_0\in(0,1)$ were such a rank-loss instant. Step 3.1 makes [F5] applicable in $(E,g,-N)$, so for some $u$ with $u_0<u<1$, sufficiently near $u_0$, one has $\delta(u)\in I^+_{E,-N}(C)=I^-_{E,N}(C)$. On the other hand [F3] puts $\delta(u)$ in $\partial_E I^-_{E,N}(C)$. The set $I^-_{E,N}(C)=\bigcup_{c\in C}I^-_{E,N}(c)$ is open by [F11], so by the boundary definition in [F1] it is disjoint from its boundary. This is a contradiction. Hence no focal point occurs strictly between $c$ and $p$. No exclusion of a focal point at $p$ is asserted. [A1, step 1.1, step 3.1, F1, F3, F5, F11] ∎

---
id: lem-author-594d78e425ed-negative-cut-selected-endpoints
title: Every negative-time cut has a closed selected domain and smooth endpoint
  extensions
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-594d78e425ed-uniform-translated-cut-localization
  - lem-author-b18e87444145-compact-diamond-closed-hit-domain
  - lem-author-b18e87444145-transverse-null-hit-extensions
  - physics:thm-gr-local-geodesics-and-exponential-map
  - physics:lem-gr-parallel-transport-and-geodesic-speed
  - physics:lem-gr-push-up-rule
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-causal-curve-calculus
  - def-causal-exterior-and-boundary-data
  - def-null-screen-expansion-and-focal-data
  - def-stationary-section-time
  - math:def-axiom-of-choice
  - math:thm-choice-implies-dependent-implies-countable-choice
dependency_roles:
  lem-author-594d78e425ed-uniform-translated-cut-localization: mathematical-premise
  lem-author-b18e87444145-compact-diamond-closed-hit-domain: mathematical-premise
  lem-author-b18e87444145-transverse-null-hit-extensions: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  physics:lem-gr-parallel-transport-and-geodesic-speed: mathematical-premise
  physics:lem-gr-push-up-rule: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  def-stationary-section-time: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 7
---

## Statement

Work in ZFC. Use the hypotheses and uniformly localized cuts of the translated-cut localization lemma, with its target $Q=C$, inside $\mathbb R_v\times\Omega$ and cylinder $\mathcal C=\mathbb R_v\times\Gamma$. In addition assume that $E$ is globally hyperbolic, $0<\delta\le\delta_0$, and $\min_Cv>2\delta$. Here $C=C_t$ is a nonempty compact smooth spacelike two-surface forming the fixed stationary-time section of $\mathcal C$, meeting each cylinder $T$-orbit exactly once. Assume $T$ is future timelike on $\mathcal C$. Use stationary section time $v$, so $Tv=1$, and put $P=I_E^-(C)$, $\Sigma_z=\{v=z\}$ and $D_z=(\{z\}\times\Omega)\cap\partial_EP$.

Choose a smooth nonzero future outward null-normal vector field $L_c$ on $C$. Here outward is relative to the specified inside $\mathbb R_v\times\Omega$: for every local smooth defining function $r$ with $\mathcal C=\{r=0\}$, $dr\ne0$ on $\mathcal C$ and inside $\{r<0\}$, require $dr_c(L_c)>0$. Thus the sign is measured toward the outside $\{r>0\}$. Let $\gamma_c:I_c\to E$ be the unique maximal affinely parametrized geodesic with $\gamma_c(0)=c$ and $\dot\gamma_c(0)=-L_c$; its portion with $s\in I_c\cap[0,\infty)$ is the selected past ray. Assume the prescribed-branch generator input: every inside point $p\in\partial_EP$ with $v(p)<\min_Cv$ has a future null geodesic segment to some $c\in C$, lying on $\partial_EP$ and having final tangent on the positive ray of $L_c$.

For $|z|\le2\delta$, define $A_z=\{c\in C:\gamma_c(s)\in D_z\text{ for some }s\in I_c\cap[0,\infty)\}$ and let $F_z(c)$ be that hit. Then the hit is unique, $A_z$ is compact and Borel, and $F_z:A_z\to D_z$ is onto and has local smooth extensions into $\Sigma_z$. If $z<0$, then $A_z\subset A_0$ and $F_0(c)$ is the same selected ray's intermediate endpoint at $v=0$ for every $c\in A_z$.

## Facts & Assumptions

[A1] Work in ZFC. AC implies Dependent Choice and Countable Choice, meeting the choice assumptions of the localization, endpoint, geodesic and causal suppliers. [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]]

[F1] With the localization lemma's hypotheses and target $Q=C$, the cuts $D_z$ are compact and strictly inside the specified cylinder for $|z|\le2\delta$. Its $\Omega$ and $\Gamma$ specify the inside and its spatial boundary in $\Sigma^\circ$. [[lem-author-594d78e425ed-uniform-translated-cut-localization]]

[F2] For a compact smooth target surface having strictly positive minimum temporal value relative to the zero-level slice, smooth future null initial vectors and a compact temporal zero-level cut in a globally hyperbolic spacetime, the selected hitting domain is closed. It is compact and Borel, and the unique-hit map has local smooth extensions into the zero-level slice. The extension conclusion requires no regularity of the cut as a surface. [[lem-author-b18e87444145-compact-diamond-closed-hit-domain]] [[lem-author-b18e87444145-transverse-null-hit-extensions]]

[F3] A prescribed initial vector determines a unique maximal geodesic. Affine reversal and rescaling preserve geodesics; a nonzero initially null tangent remains nonzero and null, and its time orientation is constant. Short geodesics with prescribed timelike initial tangent exist smoothly. [[physics:thm-gr-local-geodesics-and-exponential-map]] [[physics:lem-gr-parallel-transport-and-geodesic-speed]]

[F4] Chronological pasts are open, and push-up gives $x\le_E y\ll_E z\Rightarrow x\ll_E z$ and $x\ll_E y\le_E z\Rightarrow x\ll_E z$. Restrictions of smooth null segments are causal curves; smooth future timelike segments are timelike curves in the stipulated curve class. [[physics:lem-gr-chronology-openness]] [[physics:lem-gr-push-up-rule|Push-up rule]] [[physics:lem-gr-causal-curve-calculus]]

[F5] Causal relations, temporal functions and relative boundaries are computed in $E$. Smooth spacelike two-surfaces and nonzero future null normals have the supplied geometric meanings. The outward convention is the defining-function sign in the Statement, with the inside specified by [F1]. In a boundary chart any two such defining functions have positively proportional differentials on the cylinder, so this sign is independent of the function. Only the surface and normal definitions are used; no focal-exclusion conclusion is invoked. [[def-causal-exterior-and-boundary-data]] [[def-null-screen-expansion-and-focal-data]]

[F6] Stationary section time satisfies $Tv=1$ and the spatial coordinates are constant along stationary orbits. On the product, the flow is defined for every stationary parameter. [[def-stationary-section-time]]

## Proof

**Given:** The hypotheses and prescribed-branch generator input in the Statement.

**Goal:** Establish unique selected endpoints, compact/Borel domains, smooth local extensions, coverage and negative-time nesting.

1.1 By [F3], $\gamma_c$ has nonzero past null tangent on its selected portion. Thus $(v\circ\gamma_c)'<0$, so it meets a level $v=z$ at most once. Because $v(c)>2\delta\ge z$, every hit on $D_z$ has positive parameter. This makes $A_z$ and $F_z$ precisely the selected domain and endpoint map of [F2] for the shifted temporal function $v-z$. That function has differential $dv$, zero-level $\Sigma_z$ and $\min_C(v-z)>0$. The smooth compact target and initial field are as assumed, while [F1] supplies compact $D_z$. Apply both endpoint suppliers to conclude that $A_z$ is compact and Borel and $F_z$ has local smooth extensions into $\Sigma_z$. [given, A1, F1, F2, F3, F5]

2.1 Fix $p\in D_z$. It is inside the cylinder and $v(p)=z<\min_Cv$, so the assumed generator input gives a future null segment from $p$ to some $c\in C$ ending on the positive ray of $L_c$. Choose an affine parameter on that segment, reverse it at $c$, and rescale by a positive constant to give initial tangent $-L_c$. By maximal-geodesic uniqueness in [F3], it is a restriction of $\gamma_c$. Hence $c\in A_z$ and $F_z(c)=p$ by step 1.1. Together with the definition $F_z(A_z)\subset D_z$, this proves surjectivity. The segment is used for one fixed $p$ at a time. [given, F1, F3, F5, step 1.1]

2.2 Fix any $c\in A_z$, put $p=F_z(c)$ and orient the selected segment from $p$ to $c$ towards the future. For each point $r$ on it, [F4] gives $p\le_Er\le_Ec$, including endpoints by reflexivity. As $P$ is open and $p\in\partial_EP$, $p\notin P$. If $r\in P$, there is $c'\in C$ with $r\ll_Ec'$, and push-up gives $p\ll_Ec'$, a contradiction. Thus every $r$ is outside $P$. To show $r\in\overline P^{\,E}$, take a short geodesic $\eta$ with $\eta(0)=r$ and initial tangent $-N_r$, where $N$ is the future timelike orientation field. By smoothness it is past timelike for small positive parameter. For such $\varepsilon>0$, its reversed restriction is a future timelike curve from $r_\varepsilon=\eta(\varepsilon)$ to $r$. Push-up with $r\le_Ec$ gives $r_\varepsilon\ll_Ec$, including when $r=c$, and $r_\varepsilon\to r$. Hence $r\in\overline P^{\,E}\setminus P=\partial_EP$. This proves boundary containment for every selected segment, including ones other than the segment used for coverage. [given, A1, F3, F4, F5, step 1.1]

3.1 Let $z<0$ and $c\in A_z$. Along the finite segment from $F_z(c)$ to $c$, strict temporal monotonicity and $z<0<\min_Cv$ give a unique point $p_0$ with $v(p_0)=0$. If $p_0$ were outside the inside region, including on its boundary, continuity of the spatial projection would give a first exit $y\in\mathcal C$ between $F_z(c)$ and $p_0$; the inside and boundary here are the $\Omega$ and $\Gamma$ of [F1]. Temporal monotonicity gives $v(y)\le0$. The unique point $c_y\in C_t$ on its cylinder orbit has $v(c_y)>2\delta>0$. Since $Tv=1$, the stationary flow reaches $c_y$ from $y$ after parameter $v(c_y)-v(y)>0$. This orbit segment stays on the cylinder and is future timelike by hypothesis and [F4], so $y\in I_E^-(C)=P$, contradicting step 2.2. Therefore $p_0$ is inside; step 2.2 also puts it on $\partial_EP$, so $p_0\in D_0$. It lies on the same selected ray from $c$, and the unique-hit definition gives $c\in A_0$ and $F_0(c)=p_0$. [given, F1, F4, F5, F6, step 1.1, step 2.2] ∎

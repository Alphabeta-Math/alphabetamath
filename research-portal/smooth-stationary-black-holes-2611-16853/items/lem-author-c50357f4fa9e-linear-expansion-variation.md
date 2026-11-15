---
id: lem-author-c50357f4fa9e-linear-expansion-variation
title: Linear and path-independent normal-graph variation of expansion
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-c50357f4fa9e-normal-graph-domain
  - lem-author-c50357f4fa9e-expansion-second-jet
  - math:thm-chain-rule-for-differentials-of-smooth-maps
  - math:thm-clairaut-schwarz-mixed-partials
  - math:def-countable-choice
  - lem-author-c50357f4fa9e-outward-graph-null-gauge
  - physics:def-gr-fx-null-screen-geometry
dependency_roles:
  lem-author-c50357f4fa9e-normal-graph-domain: mathematical-premise
  lem-author-c50357f4fa9e-expansion-second-jet: mathematical-premise
  math:thm-chain-rule-for-differentials-of-smooth-maps: mathematical-premise
  math:thm-clairaut-schwarz-mixed-partials: mathematical-premise
  math:def-countable-choice: mathematical-premise
  lem-author-c50357f4fa9e-outward-graph-null-gauge: mathematical-premise
  physics:def-gr-fx-null-screen-geometry: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

Assume countable choice $\mathrm{AC}_\omega$. Let $\Sigma$ be a smooth spacelike hypersurface in a time-oriented smooth Lorentzian four-manifold $(M,g)$, let $h=g|_{T\Sigma}$, and let $S\subset\operatorname{int}\Sigma$ be a smooth embedded two-surface without boundary with a supplied smooth outward $h$-unit normal $\nu$. Use a supplied open normal-graph domain $\Omega$ containing the relevant zero section, on which $T(p,r)=\exp^h_p(r\nu_p)$ is a diffeomorphism onto its image. The domain may be local, with the graph constructions then restricted to its open base patch in $S$; a global graph uses such a domain over all of $S$. For compact $S$ a uniform tube exists, while no uniform tube is presumed for noncompact $S$. A smooth $u$ is admissible when its graph lies in $\Omega$, and $F_u(p)=T(p,u(p))$.

Use the canonical gauge of the second-graph-data construction: $n$ is the future unit normal to $\Sigma$, $\nu_u$ is the outward graph unit normal, $L_u=n|_{F_u(S)}+\nu_u$, and $\Theta(u)=F_u^*(\theta_{L_u})$ is the pulled-back outgoing expansion. For this gauge on admissible graphs, define $$\mathcal L\phi=\left.\frac{d}{d\epsilon}\right|_{\epsilon=0}\Theta(\epsilon\phi).$$ For compact $S$ this is defined for every $\phi\in C^\infty(S)$; on a noncompact surface the definition applies on a supplied tube to every $\phi$ admitting a common parameter interval of admissible graphs, in particular every compactly supported smooth $\phi$. Independently, the local formulas define the same differential operator on all smooth functions as a germ at each point. The operator is linear with smooth coefficients, of order at most two. Here **linear** means $\mathcal L(a\phi+b\psi)=a\mathcal L\phi+b\mathcal L\psi$ for real constants $a,b$ wherever the relevant graph paths are admissible.

If $u(t,p)$ is a jointly smooth admissible graph path with $u(0,p)=0$ and $\partial_tu(0,p)=\phi(p)$, then $\partial_t\Theta(u(t))|_0=\mathcal L\phi$. Thus the first derivative does not depend on the higher parameter behavior of the chosen graph path.

## Facts & Assumptions

[F1] Under the geometric and graph-domain hypotheses of the Statement and the countable-choice hypothesis in [F5], [[lem-author-c50357f4fa9e-normal-graph-domain]] supplies a common parameter interval for each compactly supported direction in a supplied tube, and for every smooth direction when $S$ is compact.

[F2] For the stated normal-graph data and canonical gauge, [[lem-author-c50357f4fa9e-expansion-second-jet]] gives the smooth local expression $A(x,u,\partial u,\partial^2u)$ for pulled-back expansion.

[F3] [[math:thm-chain-rule-for-differentials-of-smooth-maps]] gives the chain rule for this finite-dimensional smooth function.

[F4] [[math:thm-clairaut-schwarz-mixed-partials]] gives equality of mixed coordinate partial derivatives for a $C^2$ scalar function on an open Euclidean set. Joint smoothness makes this applicable to $u(t,x)$ and each spatial first derivative $\partial_bu(t,x)$.

[F5] Adopt countable choice $\mathrm{AC}_\omega$ in the sense of [[math:def-countable-choice]]. This meets the countable-choice requirements of the graph-domain and second-graph-data suppliers in [F1] and [F2]; their geometric and graph-domain hypotheses are those explicitly stated above. No stronger choice principle is assumed.

[F6] Under the geometric and graph-domain hypotheses of the Statement and the countable-choice assumption in [F5], [[lem-author-c50357f4fa9e-outward-graph-null-gauge]] supplies the smooth future unit normal $n$, the outward graph unit normal $\nu_u$ with $\nu_0=\nu$, and the smooth future null normal $L_u=n|_{F_u(S)}+\nu_u$ used in the Statement.

[F7] [[physics:def-gr-fx-null-screen-geometry]] defines the outgoing expansion on each embedded spacelike graph by $\theta_{L_u}=\operatorname{tr}_{q_u}\chi_{L_u}$, where $q_u$ is the induced positive metric and $\chi_{L_u}(X,Y)=g(\nabla_XL_u,Y)$ for graph-tangent $X,Y$, with tangential extension independence. Its countable-choice convention is met by [F5]. The canonical gauge in [F6] supplies the future null partner $n|_{F_u(S)}-\nu_u$, which pairs with $L_u$ to $-2$, as required by this definition; this choice of partner leaves $L_u$ unchanged. No congruence or compactness assumption is needed for this surface expansion.

## Proof

**Given:** The geometric and normal-graph data of the Statement, the countable-choice hypothesis in [F5], and a smooth graph direction, with an admissible parameter interval whenever a global graph path is asserted.

**Goal:** Establish the linear differential expression and its path independence.

1.1 The geometric and graph-domain hypotheses in the Statement, together with the countable-choice assumption in [F5], meet the supplier requirements in [F1] and [F2]. At a fixed chart point, [F2] and [F3] give $$\mathcal L\phi=A_z(x,0,0,0)\phi+\sum_a A_{p_a}(x,0,0,0)\partial_a\phi+\sum_{a\le b} A_{B_{ab}}(x,0,0,0)\partial_a\partial_b\phi.$$ Here $z$ is the scalar value, $p_a$ the first partials and $B_{ab}$ the independent symmetric second-partial coordinates; these symbols denote coordinates of the smooth function $A$, not extra geometric fields. The coefficient functions are smooth. This formula is linear in $\phi$ and its derivatives. Chart formulas agree since they differentiate the same pulled-back geometric scalar; locally all sufficiently small graph parameters are admissible. It therefore defines a global differential operator on germs, without requiring a uniform tube on a noncompact surface. [F1, F2, F3, F5, given, algebra]

2.1 For a jointly smooth path $u(t,x)$, apply [F4] to $u$ and to each $\partial_bu$, all of which are $C^2$ on the open parameter-coordinate domain. Commuting the parameter derivative first with $\partial_a$ on $\partial_bu$ and then with $\partial_b$ on $u$ gives $\partial_t\partial_a u|_0=\partial_a\phi$ and $\partial_t\partial_a\partial_bu|_0=\partial_a\partial_b\phi$. Differentiating [F2] therefore gives precisely the expression in step 1.1. In the compact or compactly supported case [F1] supplies an actual interval for $u=t\phi$. For two such directions, their union of supports is compact; a common smaller interval handles each linear combination. If global admissibility is otherwise supplied, only that supplied interval is used. This proves the path statement and all asserted linearity without a claim of differentiability in an unspecified infinite-dimensional function-space norm. [F1, F2, F3, F4, F5, step 1.1, algebra] ∎

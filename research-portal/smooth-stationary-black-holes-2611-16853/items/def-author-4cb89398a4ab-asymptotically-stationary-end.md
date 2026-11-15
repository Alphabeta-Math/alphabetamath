---
id: def-author-4cb89398a4ab-asymptotically-stationary-end
title: Exact asymptotically stationary end contract
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-causal-exterior-and-boundary-data
  - math:def-embedded-smooth-submanifold-with-boundary
  - math:def-codimension-and-hypersurface
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold
  - math:def-local-and-global-flow
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:def-embedded-smooth-submanifold-with-boundary: mathematical-premise
  math:def-codimension-and-hypersurface: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Chruściel–Wald, Maximal Hypersurfaces in Asymptotically Stationary
        Spacetimes
      url: https://arxiv.org/pdf/gr-qc/9304009
      locator: Section 2 opening conventions and Definition 2.1, printed/PDF pp. 8–9,
        equations (2.1)–(2.5).
      statement: Definition 2.1 specifies an acausal end, the metric component and
        weighted derivative/Hölder estimates, a boundary diffeomorphism, and a
        complete Killing field uniformly timelike on the end with the displayed
        asymptotics. The preceding paragraph defines hypersurfaces as embedded
        codimension-one submanifolds, allowing boundary. The local item
        explicitly supplies the smooth gluing realization and the positive-r
        domain needed to interpret these conditions.
      hypotheses: Smooth connected Hausdorff paracompact time-oriented spacetime and
        an acausal hypersurface, possibly with boundary, decomposed into an end
        and a remainder; integer k≥2, 0<α≤1, 0<λ≤1. The three numbered clauses
        are defining requirements, not consequences of stationarity.
      reading_limits: Read the extracted PDF text of the section 2 opening conventions
        and all three clauses of Definition 2.1 on printed/PDF pp. 8–9,
        including equations (2.1)–(2.5). Browser page screenshots were
        unavailable. No theorem or proof was reviewed. The explicit gluing
        realization and r>0 domain below are local formulation conventions; this
        citation is not claimed to prove a coordinate or gluing existence
        theorem, or the stronger inequality r>R₁ throughout O₁.
dependency_level: 2
---

## Definition

Use the smooth time-oriented Lorentzian data $(M,g,N,T)$ and causal-curve conventions supplied by the Lorentzian and causal interfaces. Here acausal means that no two distinct points are joined by a causal curve. A hypersurface, possibly with boundary, means an embedded smooth three-dimensional submanifold of the four-manifold $M$, with a supplied manifold-with-boundary smooth structure; its codimension is $4-3=1$. A Chruściel–Wald $(k,\alpha)$-asymptotically stationary end consists of such an acausal hypersurface $\Sigma=\Sigma_1\sqcup\Sigma'$ and the following data and requirements. The remainder $\Sigma'$ is supplied as an embedded smooth three-dimensional submanifold with boundary of $\Sigma$; its boundary means its intrinsic manifold boundary, with the induced smooth two-manifold structure, rather than its topological boundary in $M$. Its inclusion in $M$ is also required to be a smooth embedding.

(1) Supply a diffeomorphism $e:E\to\Sigma_1$, where $E=\{z\in\mathbb R^3:|z|>R_1\}=\mathbb R^3\setminus B(R_1)$, $R_1>0$, and $B(R_1)$ is the closed Euclidean ball. Thus $\Sigma_1$ has the smooth structure of an open end of $\Sigma$. A coordinate system $(t,x^1,x^2,x^3)$ on an open neighborhood $O_1$ of $\Sigma_1$ obeys the following estimates for constants $C>0$, integer $k\ge2$, $0<\alpha\le1$ and $0<\lambda\le1$. Put $r=(\sum_i(x^i)^2)^{1/2}$ and require $r>0$ throughout $O_1$. The model coordinate $z$ and the spacetime coordinates $(t,x)$ are separately supplied: no identity $x=e^{-1}$, level-set condition $t|_{\Sigma_1}=0$, or inequality $r>R_1$ on $O_1$ is assumed. Put $\eta=\operatorname{diag}(-1,1,1,1)$; indices $\mu,\nu,\sigma_j$ range from $0$ to $3$, and $i,j$ from $1$ to $3$:

$$g_{00}<-C^{-1},\qquad |g_{\mu\nu}-\eta_{\mu\nu}|\le Cr^{-\alpha},\qquad g_{ij}Z^iZ^j\ge C^{-1}\sum_i(Z^i)^2\quad(Z\in\mathbb R^3).$$

$$|\partial_{\sigma_1}\cdots\partial_{\sigma_m}g_{\mu\nu}|\le Cr^{-\alpha-m}\quad(1\le m\le k).$$

Writing $\partial^k$ for any ordered $k$ coordinate derivatives, require

$$|(\partial^kg_{\mu\nu})(t,x)-(\partial^kg_{\mu\nu})(\tau,y)|\le Cr(x)^{-\alpha-k-\lambda}(|t-\tau|^\lambda+|x-y|^\lambda)$$

whenever both points lie in $O_1$, $|t-\tau|\le1$ and $|x-y|\le r(x)/2$. Absolute values on components are ordinary real absolute values and $|x-y|$ is the Euclidean norm; the estimate holds for each component and derivative choice.

(2) Let $\overline E=\{z\in\mathbb R^3:|z|\ge R_1\}$ have its usual smooth manifold-with-boundary structure, and let $S$ be a connected component of the intrinsic boundary $\partial\Sigma'$. Supply a diffeomorphism $h:\partial\overline E\to S$, meaning a bijective smooth map with smooth inverse. Its realization in the given smooth hypersurface is part of the data: supply a smooth embedding $j:\overline E\to\Sigma$ whose restriction to $E$ is $e$ followed by the inclusion of $\Sigma_1$, and whose restriction to $\partial\overline E$ is $h$ followed by the inclusion of $S$. Require $j(\overline E)\cap\Sigma'=S$ and $j(\overline E)\cup\Sigma'=\Sigma$. These maps specify the smooth boundary identification implicit in the source's disjoint end/remainder notation. No compactness of $\Sigma'$ is imposed, and existence of such a gluing realization is required data, not an asserted gluing theorem.

(3) The smooth Killing field $T$ on all of $M$ has a complete flow $\phi_u$, $u\in\mathbb R$, satisfies $g(T,T)<-C^{-1}$ on $\Sigma_1$, and has asymptotics

$$T=(A+O(r^{-\alpha}))\partial_t+\sum_iO(r^{-\alpha})\partial_{x^i},\qquad A\ne0.$$

Here a complete flow means a smooth global flow of $T$: the map $\phi:\mathbb R\times M\to M$, $\phi(u,p)=\phi_u(p)$, is smooth, $\phi_0=\operatorname{id}_M$, $\frac{d}{du}\phi_u(p)=T_{\phi_u(p)}$, and $\phi_{u+v}=\phi_u\circ\phi_v$ for all real $u,v$. The component $O(r^{-\alpha})$ bounds hold uniformly in the end coordinates as $r\to\infty$. Constants may be enlarged to one common $C$. These are imposed data, not consequences of the word stationary.

## Definition references

[[def-stationary-lorentzian-data]]

[[def-causal-exterior-and-boundary-data]]

[[math:def-embedded-smooth-submanifold-with-boundary]]

[[math:def-codimension-and-hypersurface]]

[[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

[[math:thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold]]

[[math:def-local-and-global-flow]]

## Facts & Assumptions

[F1] The Lorentzian and causal suppliers define the underlying metric, Killing field and causal terminology. [[def-stationary-lorentzian-data]] [[def-causal-exterior-and-boundary-data]]

[F2] Chruściel–Wald Definition 2.1 supplies the three end conditions: the displayed metric estimates, the boundary identification, and the complete uniformly timelike Killing field with its stated asymptotics. The smooth gluing realization and positive-r estimate domain are made explicit here as supplied data.

[F3] An embedded smooth submanifold with boundary carries a supplied smooth structure for which its inclusion is a smooth embedding. Codimension is ambient dimension minus submanifold dimension. These interfaces apply to $\Sigma\subset M$ and to the remainder and closed-end realization in $\Sigma$. [[math:def-embedded-smooth-submanifold-with-boundary]] [[math:def-codimension-and-hypersurface]]

[F4] The boundary of a smooth three-manifold with boundary has the induced smooth boundaryless two-manifold structure. A diffeomorphism between boundaryless smooth manifolds is a bijective smooth map with smooth inverse; this applies to $e$ and $h$. [[math:thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold]] [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

[F5] A global flow of a smooth vector field is a smooth map on $\mathbb R\times M$ with identity at zero, integral curves generated by the field, and the flow composition law. [[math:def-local-and-global-flow]]

## Justification

**Given:** The displayed smooth structures, maps, coordinate domain and conditions.

**Goal:** Define a precise end contract without asserting existence for arbitrary stationary data.

1.1 The Lorentzian and causal conventions give meanings to the metric, Killing condition and acausality. The supplied embeddings make $\Sigma$ a codimension-one smooth submanifold, and give $\Sigma'$ and $j(\overline E)$ their stated manifold-with-boundary structures. These are requirements on the data, so no smooth structure is inferred from an arbitrary set-theoretic remainder. [given, F1, F3]

1.2 In the chosen spacetime chart every derivative and norm in (1) is a derivative or norm of a specified real component. The explicit condition $r>0$ on all of $O_1$ makes each negative radial power defined, including at both points in the Hölder condition. This uses no relation between the model radius $|z|$ and the coordinate radius $r$, and does not infer $r>R_1$ from the topology of $\Sigma_1$. [given, F1, F2]

2.1 The supplied boundary diffeomorphism $h$ is between smooth two-manifolds; the restrictions of $j$ identify its boundary values with that map and its interior values with the end model. Thus (2) is a definite compatibility condition on supplied smooth maps. Clause (3) separately requires the smooth global flow generated by $T$ in [F5] and its component bounds; a local Killing field alone does not supply it. The conjunction retains the cited metric estimates, Hölder condition, boundary identification and uniform timelikeness, with the necessary structural and domain conventions explicit and with no existence conclusion. [given, F1, F2, F3, F4, F5, step 1.1, step 1.2] ∎

## External input

The end estimates, boundary identification and Killing-field conditions are imported from Chruściel–Wald Definition 2.1, printed/PDF pp. 8–9. The preceding paragraph supplies its embedded codimension-one hypersurface convention. The smooth boundary realization and positive-r domain are explicit formulation data here; no coordinate or gluing existence result is imported or proved.

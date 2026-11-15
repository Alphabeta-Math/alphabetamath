---
title: Exact asymptotic and orbit package for the IK criterion
status: draft
research_item: def-author-9f9c6144aed8-ik-af
dependency_level: 2
sources:
  references:
    - title: Ionescu–Klainerman, On the uniqueness of smooth, stationary black holes
        in vacuum (arXiv:0711.0040v2)
      url: https://arxiv.org/pdf/0711.0040
      locator: Section 1.2, AF, equations (1.4)–(1.5), printed/PDF pp. 6–7, including
        footnote 4.
      statement: The AF hypothesis specifies a stationary product end with the
        displayed metric component bounds and positive mass, the chronological
        exterior, a spacelike section matching t=0, complete stationary orbits
        meeting that section, and nonzero contraction of T with its future unit
        normal.
      hypotheses: The source introduces AF in a smooth time-oriented four-dimensional
        vacuum spacetime with a smooth Killing field, on a connected orientable
        paracompact manifold without boundary. Here only its geometric
        predicates are defined; neither vacuum equations nor existence of such
        data is deduced.
      reading_limits: Consulted the PDF text of section 1.2, AF and footnote 4 on
        printed/PDF pp. 6–7. No image inspection, later analytic proof
        reconstruction, or independent proof review is claimed. The
        maximal-curve and unit-normal constructions use the declared
        mathematical suppliers; the O_0 interpretation and its time uniformity
        are explained locally.
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)
- [math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)
- [` Ionescu–Klainerman, On the uniqueness of smooth, stationary black holes in vacuum (arXiv:0711.0040v2) · Section 1.2, AF, equations (1.4)–(1.5), printed/PDF pp. 6–7, including footnote 4. `](https://arxiv.org/pdf/0711.0040)


## Definition

Fix a smooth connected orientable paracompact boundaryless, time-oriented Lorentzian four-manifold $(M,g,N)$ and a smooth Killing field $T$, with the stationary Lorentzian conventions. The **IK AF package** consists of an open end $M^{\mathrm{end}}\cong\mathbb R\times\{x\in\mathbb R^3:|x|>R\}$, with coordinates $(t,x)$, $r=|x|$, $T=\partial_t$, and $g_{00}=-1+2M/r+O(r^{-2})$, $g_{ij}=\delta_{ij}+O(r^{-1})$, $g_{0i}=O(r^{-2})$, where the constant $M>0$ is the mass parameter (distinct from the manifold denoted by the same letter).

Here $u=O(r^{-b})$ means $u(0,\cdot)=O_0(r^{-b})$ in the fixed spatial chart: some $R_1>R$ and finite $C\geq0$ satisfy $|u(0,x)|\leq Cr^{-b}$ for all $r\geq R_1$, componentwise for an array. The metric remainders are independent of $t$ because $T=\partial_t$ is Killing, so the same bounds hold for every $t\in\mathbb R$, uniformly over spatial angular directions and time. No differentiated decay is asserted by this unindexed notation.

Set $E=I^-_M(M^{\mathrm{end}})\cap I^+_M(M^{\mathrm{end}})$, using chronological reachability in $M$. Require an embedded spacelike section $\Sigma_0\cong\{|x|>1/2\}$ agreeing with $t=0$ on the end. Denote its unique smooth future unit normal by $T_0$, so $g(T_0,T_0)=-1$, $g(T_0,N)<0$ and $g(T_0,v)=0$ for $v\in T\Sigma_0$.

For each $p\in E$, let $\gamma_p:I_p\to M$ be the unique maximal integral curve of $T$ with $\gamma_p(0)=p$. Require every such orbit to be complete, meaning $I_p=\mathbb R$, and to meet $\Sigma_0$. Require also $|g(T,T_0)|>0$ on $\Sigma_0\cap E$. These requirements are assumptions, not consequences of mere stationarity or leading asymptotic decay.

## Definition references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)

## Facts & Assumptions

[F1] The stationary Lorentzian data specify the smooth metric, time orientation, Killing equation and local-flow conventions. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] The chronological exterior is the intersection of chronological past and future computed in the specified ambient manifold; a spacelike hypersurface has positive-definite induced metric. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F3] The fixed-chart decay interface with $m=0$ defines $O_0(r^{-b})$ by a common radius and componentwise constants, uniformly over spatial angular directions. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F4] In a smooth time-oriented Lorentzian four-manifold, an embedded spacelike hypersurface has a unique future unit normal, smooth along the hypersurface. Only parts (a)–(b) of the normal lemma are used. [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[F5] A smooth vector field has a unique maximal integral curve through each point, normalized at parameter zero. [math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)

## Justification

**Given:** The manifold, field, end chart and spacelike section specified in the Definition.

1.1 The chronological operations determine $E$ in the ambient manifold. The normal lemma applies to the time-oriented Lorentzian manifold and embedded spacelike section, giving the stated unique smooth $T_0$. The maximal-integral-curve theorem applies to the smooth $T$ on $M$, so $I_p=\mathbb R$ and intersection with $\Sigma_0$ are unambiguous additional predicates for each $p\in E$. Nonvanishing of $g(T,T_0)$ is the separately imposed transversality condition; no existence of an AF package or completeness theorem is asserted. [given, F1, F2, F4, F5]

2.1 In the end chart the local flow of $T=\partial_t$ sends $(t,x)$ to $(t+s,x)$. Differentiating its metric pullback at $s=0$ by the Lie-derivative definition gives $0=(\mathcal L_Tg)_{\mu\nu}=\partial_tg_{\mu\nu}$. Thus each metric remainder has the same value at $(t,x)$ as at $(0,x)$. Applying the $m=0$ decay convention to the time-zero remainder gives the same radius and constants for all $t$, exactly the ordinary bounds defined above. The package therefore specifies definite data and predicates without deriving any of its existence or orbit assumptions from the asymptotic estimates. [given, F1, F3, step 1.1] ∎

## External input

The independent Ionescu–Klainerman source supplies the AF predicates in section 1.2, equations (1.4)–(1.5), printed/PDF pp. 6–7. Only that definition package is imported; no vacuum equation, existence theorem or analytic continuation result is inferred here.

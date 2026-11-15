---
title: Radu nontrapping global regularity package
status: published
research_item: def-author-ad064c44a1cc-nontrapping-gr
dependency_level: 2
sources:
  references:
    - title: Alexandru F. Radu, On rigidity of stationary black holes under a
        nontrapping assumption
      url: https://arxiv.org/html/2609.23872v1
      locator: Version 1, section 1.1, opening setup and GR, equation (1.1), through
        the sentence that Sigma^0 is t=0 on the end, immediately before SBS.
      statement: GR assumes a connected oriented time-oriented smooth Lorentzian
        four-manifold with $\operatorname{Ric}(g)=0$ and stationary Killing
        field $T$; an embedded spacelike acausal edgeless hypersurface
        $\Sigma^0$ parametrized by a diffeomorphism $\Phi_0:E_{1/2}\to\Sigma^0$,
        with $E_a=\{|x|>a\}\subset\mathbb R^3$ and $\Sigma_1=\Phi_0(E_1)$; an
        end $M^{\rm end}\simeq\mathbb R\times E_{R_0}$ with $T=\partial_t$ and
        $\Sigma^0$ the zero-time slice there. For $M_0>0$, $S\in\mathbb R^3$ and
        $|S|<M_0^2$, its coefficients satisfy $g_{00}=-1+2M_0/r+O_6(r^{-2})$,
        $g_{ij}=\delta_{ij}+O_6(r^{-1})$ and
        $g_{0i}=-2\epsilon_{ijk}S^jx^kr^{-3}+O_6(r^{-3})$, with spatial
        differentiated remainders, $r=|x|$ and $\epsilon_{123}=1$. The exterior
        $E=I_M^-(M^{\rm end})\cap I_M^+(M^{\rm end})$ is globally hyperbolic;
        its stationary orbits are complete and meet $\Sigma_1$; and
        $\Sigma^0\cap I_M^\pm(M^{\rm end})=\Sigma_1$.
      hypotheses: These are the defining conditions of the source GR package; M_0
        denotes the source mass M. No rigidity theorem, SBS, NT, maximality or
        smallness assumption is imported here.
      reading_limits: Retrieved and read the version-1 HTML section 1.1 opening setup
        and complete GR passage through the zero-time slice sentence. Only this
        formulation is imported; no theorem proof, ADM identification proof, or
        quotient regularity proof was reviewed.
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://link.springer.com/article/10.1007/s41114-019-0019-x
      locator: Definitions 2.19 (achronal), 2.95 (acausal), 2.130 (edge), and 3.35
        (partial Cauchy hypersurface).
      statement: An achronal set admits no timelike curve starting and ending in the
        set, and an acausal set admits no causal curve starting and ending in
        the set. For achronal $A$, $q\in\operatorname{edge}(A)$ precisely when
        $q\in\overline A$ and every open neighborhood $U\ni q$ contains $p\in
        I_U^-(q)$ and $s\in I_U^+(q)$ connected by a timelike curve in $U$
        avoiding $A$. An acausal edgeless set is a partial Cauchy hypersurface.
      hypotheses: Time-oriented Lorentzian manifold; edge is defined for an achronal
        subset using ambient closure and chronological relations internal to
        each open neighborhood.
      reading_limits: Read the four numbered definitions in the HTML. Used only for
        these predicates, including exclusion of causal return curves; no nearby
        hypersurface or domain-of-dependence theorem is invoked.
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [` Alexandru F. Radu, On rigidity of stationary black holes under a nontrapping assumption · Version 1, section 1.1, opening setup and GR, equation (1.1), through the sentence that Sigma^0 is t=0 on the end, immediately before SBS. `](https://arxiv.org/html/2609.23872v1)
- [` E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22 (2019), article 3 · Definitions 2.19 (achronal), 2.95 (acausal), 2.130 (edge), and 3.35 (partial Cauchy hypersurface). `](https://link.springer.com/article/10.1007/s41114-019-0019-x)


## Definition

The **Radu NT global regularity package** is the GR data of arXiv:2609.23872v1 §1.1: a connected oriented time-oriented smooth four-spacetime with $\operatorname{Ric}(g)=0$, a smooth stationary Killing field $T$, and an embedded spacelike acausal edgeless partial Cauchy hypersurface $\Sigma^0$. Supply a diffeomorphism $\Phi_0:E_{1/2}\to\Sigma^0$, that is, a bijective smooth map with smooth inverse, where $E_a=\{x\in\mathbb R^3:|x|>a\}$. Put $\Sigma_1=\Phi_0(E_1)$. There is a smooth end chart $\Psi:\mathbb R\times E_{R_0}\to M^{\rm end}$, with $T=\Psi_*\partial_t$, in which $\Sigma^0\cap M^{\rm end}=\Psi(\{0\}\times E_{R_0})$. Thus the end chart and $\Phi_0$ parametrize the same slice on their overlap; their spatial coordinates need not be identical. For $M_0>0$ and $S\in\mathbb R^3$ with $|S|<M_0^2$, require
$$g_{00}=-1+2M_0/r+O_6(r^{-2}),\quad g_{ij}=\delta_{ij}+O_6(r^{-1}),\quad g_{0i}=-2\epsilon_{ijk}S^jx^kr^{-3}+O_6(r^{-3}).$$
Here $r=|x|$, $\epsilon_{123}=1$, and derivatives are spatial in this stationary chart. The exterior $E=I_M^-(M^{\rm end})\cap I_M^+(M^{\rm end})$ is globally hyperbolic, $\Sigma^0\cap I_M^\pm(M^{\rm end})=\Sigma_1$, and its stationary orbits are complete and meet $\Sigma_1$. These are source hypotheses, not consequences of a generic black-hole definition. No maximality, quantitative perturbation bound or smallness threshold for $|S|$ is included beyond the explicit strict subextremal parameter range.

All causal predicates for $\Sigma^0$ are relative to $M$. A set $A$ is achronal if no future timelike curve has both endpoints in $A$, and acausal if no nonconstant future causal curve has both endpoints in $A$, including coincident endpoints. For achronal $A$, its edge consists of the points $q\in\overline A^{\,M}$ such that every open neighborhood $U\ni q$ contains points $p\in I_U^-(q)$ and $s\in I_U^+(q)$ joined by a future timelike curve contained in $U\setminus A$. Here $I_U^\pm(q)$ uses curves entirely within $U$. Edgeless means that this edge is empty; partial Cauchy hypersurface means acausal and edgeless. Smooth embeddedness and spacelikeness are separately imposed above.

## Facts & Assumptions

[F1] [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) supplies the stationary geometry and vacuum-tensor notation, [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) the ambient chronological relations, closure and exterior global hyperbolicity, [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) the spacelike-section terminology, and [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) the differentiated end estimates.

[F2] [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets) supplies the mathematical spacelike, achronal and acausal vocabulary; its actual domain is mathematics. The exact causal-return, edge and partial-Cauchy conventions used here are the independently cited Minguzzi definitions in External input.

[F3] [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds) supplies the smooth-bijection-with-smooth-inverse meaning for $\Phi_0$ and the end chart. The source-specific GR predicates, including the zero-time end condition, are imported from Radu's GR passage in External input.

## Justification

The supplied diffeomorphisms determine the slice parametrization, its distinguished subset $\Sigma_1$ and the end coordinates. Their overlap is a smooth change of spatial coordinates on the same zero-time slice, without a prescribed identity transition. The metric and time orientation determine the causal curve classes. Applying the chronological definitions to each open $U$ makes the edge predicate unambiguous; its closure is taken in $M$. The stated causal relations for the slice use $M$, while global hyperbolicity is tested on $E$. The asymptotic bounds, strict parameter range and complete-orbit/section condition are separate supplied predicates. This is a mathematical definition of admissible data, not a derivation of the vacuum equations from observations or an assertion that such data exist. It inserts neither a maximal section, a horizon-smallness condition nor a smooth structure on an orbit quotient.

## External input

Radu's version-1 section 1.1 GR passage supplies the source-specific package, including equation (1.1), the diffeomorphism $\Phi_0$, complete exterior orbits, chronological intersections and the zero-time end slice. The four original local definitions supply vocabulary, not this particular list of hypotheses.

Minguzzi's Definitions 2.19, 2.95, 2.130 and 3.35 supply the causal predicates written explicitly in the Definition. No theorem about the resulting hypersurface or its domain of dependence is imported.

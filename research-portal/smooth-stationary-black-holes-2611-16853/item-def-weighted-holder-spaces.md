---
title: Weighted Hölder norms on a three-dimensional exterior
status: draft
research_item: def-weighted-holder-spaces
dependency_level: 1
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 13, §3.1, opening norm display
      attribution: The article defines weighted Hölder norms using a compact core and
        scaled norms on exterior annuli.
      hypotheses: Original asymptotically flat coordinates on the three-dimensional
        exterior, integer k ≥ 0, 0 < α < 1 and real β.
      reading_limits: The frozen article text at the displayed definition was read for
        attribution; this citation is not used as an independent proof of a
        prerequisite.
---

PDF p. 13: ` §3.1, opening norm display `

## Prerequisites

- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)


## Definition

Let $\Sigma_1$ be a smooth three-dimensional exterior with compact smooth boundary and a fixed end chart $x$ identifying the end with $\{x\in\mathbb R^3:|x|>r_0\}$ for some $r_0>0$. Write $r=|x|$, $K=\Sigma_1\setminus\{r>2r_0\}$ and $A_R=\{R<r<2R\}$ for $R\ge r_0$. Fix the finite interior and boundary chart subsets covering $K$ and the compact-core Hölder norm $N_K=\|\cdot\|_{C^{k,\alpha}(K)}$ specified by the exterior-data definition: it is the sum of the coordinate derivative suprema through order $k$ and the order-$k$ Hölder seminorms on those subsets.

Let $k\ge0$ be an integer, $0<\alpha<1$ and $\beta\in\mathbb R$. For distinct points of a set $E$ in Euclidean coordinates, put $[v]_{\alpha;E}=\sup_{x\ne y\in E}|v(x)-v(y)|/|x-y|^\alpha$. A multi-index $I=(i_1,i_2,i_3)$ has nonnegative integer entries, order $|I|=i_1+i_2+i_3$, and $\partial_x^I=\partial_{x^1}^{i_1}\partial_{x^2}^{i_2}\partial_{x^3}^{i_3}$. For a real scalar function $w$ that is locally $C^{k,\alpha}$ up to the boundary, define the extended-valued quantity

$$\|w\|_{C^{k,\alpha}_\beta}=N_K(w)+\sup_{R\ge r_0}R^{-\beta}\left(\sum_{j=0}^k R^j\max_{|I|=j}\sup_{A_R}|\partial_x^I w|+R^{k+\alpha}\max_{|I|=k}[\partial_x^I w]_{\alpha;A_R}\right).$$

Here locally $C^{k,\alpha}$ up to the boundary means that, in each interior or boundary chart, derivatives through order $k$ are continuous up to the boundary and the order-$k$ derivatives have finite Hölder seminorm on each compact chart subset. The space $C^{k,\alpha}_\beta(\Sigma_1)$ consists of these functions for which the displayed quantity is finite. For a finite array of components, apply the definition componentwise and sum the component norms; in particular, coordinate components of a tensor on the end can be measured this way, with fixed local components on the core.

## Definition references

[def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

## Justification

The exterior-data definition supplies the fixed chart subsets and the compact-core norm, and the local Hölder definition supplies the coordinate derivative and seminorm conventions. Each displayed term is nonnegative and homogeneous, and the triangle inequality follows from the absolute-value triangle inequality before taking suprema. The core and annuli cover $\Sigma_1$, so a zero quantity forces $w=0$ everywhere. Thus the finite-valued class is a vector space and the displayed quantity is a norm on it. The fixed choices are part of the definition; no equivalence of different choices, completeness, or elliptic mapping property is asserted here.

## Source notes

The article's notation $\partial_x^j w$ is made explicit by the maximum over coordinate multi-indices of order $j$. The article reference records attribution, while the definition and its justification use the stated local suppliers.

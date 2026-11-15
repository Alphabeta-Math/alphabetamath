---
title: Counting multiplicity of an endpoint map
status: draft
research_item: def-author-0336834a2590-endpoint-multiplicity
dependency_level: 1
sources:
  references:
    - title: Leon Simon, Introduction to Geometric Measure Theory (2014)
      url: https://web.stanford.edu/class/math285/ts-gmt.pdf
      locator: Chapter 2, §1, Theorem 1.8(i)–(ii) and its proof, printed pp.44–45 (PDF
        page 26)
      statement: For metric spaces X,Y with X sigma-compact, a Hausdorff-m-measurable
        subset B of finite measure, and a Lipschitz map f:B to Y, the image and
        the fiber-counting function are Hausdorff-m-measurable.
      hypotheses: Sigma-compact metric source; measurable finite-measure domain;
        Lipschitz map; metric target; here m=2.
      reading_limits: Read the linked PDF text of Theorem 1.8 and its proof, including
        all hypotheses. No PDF image inspection or whole-book review. The
        countable-piece application below is local, not attributed to Simon.
---

## Prerequisites

- [def-author-0336834a2590-measurable-surface-domains](item-def-author-0336834a2590-measurable-surface-domains)
- [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction)
- [math:thm-second-countable-implies-lindelof](https://alphabetamath.cc/item/thm-second-countable-implies-lindelof)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [` Leon Simon, Introduction to Geometric Measure Theory (2014) · Chapter 2, §1, Theorem 1.8(i)–(ii) and its proof, printed pp.44–45 (PDF page 26) `](https://web.stanford.edu/class/math285/ts-gmt.pdf)


## Definition

For a Borel surface domain $A$ and a locally Lipschitz map $F:A\to\Sigma$, define $N(F,A;y)=\#\{x\in A:F(x)=y\}$, taking values in $\{0,1,2,\ldots,\infty\}$. The image is $D=F(A)$. Surjectivity onto $D$ gives $N(F,A;y)\ge1$ on $D$; injectivity is the additional condition $N(F,A;y)=1$ there. Integration of multiplicity is with the completed normalized Hausdorff area measure. For the maps with local $C^1$ extensions considered here, the area theorem supplies its measurability.

## Facts & Assumptions

[A1] Work in ZFC, as in the surface-domain convention. Countable choice is used when selecting the countable local cover below. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Use the smooth Hausdorff second-countable source surface, target three-manifold, finite component distances, Borel domains and complete normalized Hausdorff measures of [def-author-0336834a2590-measurable-surface-domains](item-def-author-0336834a2590-measurable-surface-domains). Source area equals normalized intrinsic Hausdorff area and is locally finite; target measurability is interpreted componentwise.

[F2] A map is $L$-Lipschitz when its target distance is at most $L$ times its source distance, for some finite $L\ge0$. Locally Lipschitz on $A$ means this bound holds on a relative neighborhood of each point, using the specified component distances. [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction)

[F3] Under countable choice, a second-countable space is Lindelöf. The intersections of a countable source basis with $A$ form a countable basis of $A$. [math:thm-second-countable-implies-lindelof](https://alphabetamath.cc/item/thm-second-countable-implies-lindelof)

[F4] The independent metric-space measurability input is recorded in External input. Its finite-domain hypothesis is checked separately on each piece below.

## External input

Simon, Theorem 1.8(i)–(ii): if $X,Y$ are metric spaces, $X$ is $\sigma$-compact, $B\subseteq X$ is $\mathcal H^m$-measurable with finite measure and $f:B\to Y$ is Lipschitz, then $f(B)$ and $y\mapsto\#f^{-1}(y)$ are $\mathcal H^m$-measurable. This established input is imported; the following application is proved locally.

## Justification

**Given:** The Borel domain, map and componentwise metric and area conventions in the Definition, with [A1] and [F1]–[F4].

1.1 This counts distinct initial points rather than parameter charts. A disjoint partition of $A$ therefore avoids counting a point twice merely because it belongs to overlapping charts. Multiple distinct initial points can have the same endpoint; they must all be retained in $N$. The inequality $N\ge1$ on the image follows directly from the definition of image. [given]

1.2 Each point of $A$ has a relative neighborhood on which $F$ is Lipschitz. Lipschitz continuity and openness of target components let us shrink it so that its image lies in one target component. Choose a source coordinate ball inside the corresponding source component, with compact closure inside a chart, small enough that its intersection with $A$ lies in this neighborhood. Such balls $U_i$ admit a countable subcover of $A$ by [F3]. Write $K_i=\overline{U_i}$ and $A_i=(A\cap U_i)\setminus\bigcup_{j<i}U_j$. Then the $A_i$ form a disjoint Borel partition of $A$, each $K_i$ is a compact metric space for the restricted source component distance, and $F|_{A_i}$ is Lipschitz into a single target component. Local finiteness of the source area and compactness give $\mathcal H_h^2(K_i)<\infty$ by a finite cover with finite-area neighborhoods; hence each $A_i$ has finite area. Hausdorff measure for a restricted metric agrees on subsets with the ambient source Hausdorff measure: intersecting ambient covers with $K_i$ gives the same diameter-cover infima. Thus $A_i$ is also measurable with finite measure as a subset of $K_i$. [A1, F1, F2, F3]

2.1 Apply [F4] with $m=2$, $X=K_i$, $B=A_i$ and $Y$ the indicated target component. Compact $K_i$ is $\sigma$-compact. Its Borel subset $A_i$ is measurable and has finite measure by step 1.2, and the required Lipschitz bound holds there. Consequently $D_i=F(A_i)$ and $N_i(y)=\#\{x\in A_i:F(x)=y\}$ are measurable for the complete target Hausdorff measure. Multiplying a Hausdorff outer measure by a positive constant changes neither its Carathéodory measurable sets nor its measurable functions, so the conclusion holds with the normalization in [F1]. Extend $N_i$ by zero on all other target components; this is measurable componentwise. [F1, F4, step 1.2]

3.1 The disjoint source partition gives $N(F,A;y)=\sum_iN_i(y)$ pointwise, with every infinite fiber represented by the value $\infty$, and $D=\bigcup_iD_i$. To check measurability of the sum directly, for each positive integer $q$ its superlevel set is the union, over $m\ge1$ and tuples $(a_1,\ldots,a_m)\in\{0,\ldots,q\}^m$ with $\sum_i a_i=q$, of the measurable sets $\bigcap_{i=1}^m\{N_i\ge a_i\}$. If the total count is at least $q$, finitely many summands already contain $q$ points, which proves this equality also for infinite counts. These countable unions and finite intersections show that $N$ is measurable, including at value $\infty$. The countable union of the $D_i$ is measurable as well. This proves the measurability needed for integration in the Definition, in particular for its locally $C^1$-extendible maps, without using the downstream endpoint-area lemma. [F1, step 1.1, step 2.1] ∎

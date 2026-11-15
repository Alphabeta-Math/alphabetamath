---
title: Area formula and endpoint bound with multiplicity
status: published
research_item: lem-author-0336834a2590-endpoint-area-with-multiplicity
dependency_level: 2
sources:
  references:
    - title: Leon Simon, Introduction to Geometric Measure Theory
      url: https://web.stanford.edu/class/math285/ts-gmt.pdf
      locator: Chapter 2, §3 equations (3.3), (3.5), and §4 equations (4.12), (4.14),
        printed pp.53–54, 58 (PDF pp.30–31,33)
      statement: For a locally Lipschitz map f from an n-dimensional C1 submanifold M
        into Euclidean space of dimension at least n, and an Hn-measurable
        subset B of M, the integral of the tangent Jacobian over B equals the
        integral over f(B) of the counting multiplicity. The Jacobian is the
        square root of the determinant of the Gram matrix of the tangent
        derivative. Equation (3.5) gives the nonnegative weighted version in
        Euclidean coordinates.
      hypotheses: Finite-dimensional C1 source submanifold; locally Lipschitz map;
        measurable source subset; Euclidean target dimension at least source
        dimension; Hausdorff measure normalized to agree with Euclidean volume
        on planes. The Riemannian version used here is obtained by the chart and
        metric comparison argument explicitly given in the local Proof, not
        quoted as a separate theorem from Simon.
      reading_limits: Read the linked PDF browser text at Chapter 2 §3 equations
        (3.1)–(3.5) and §4 equations (4.5)–(4.14), including surrounding
        hypotheses. No formula-image inspection or reconstruction of the
        Euclidean area-formula proof. The metric passage below is local.
---

## Prerequisites

- [def-author-0336834a2590-measurable-surface-domains](item-def-author-0336834a2590-measurable-surface-domains)
- [def-author-0336834a2590-surface-map-jacobian](item-def-author-0336834a2590-surface-map-jacobian)
- [def-author-0336834a2590-endpoint-multiplicity](item-def-author-0336834a2590-endpoint-multiplicity)
- [math:thm-hausdorff-measure-under-lipschitz-maps](https://alphabetamath.cc/item/thm-hausdorff-measure-under-lipschitz-maps)
- [` Leon Simon, Introduction to Geometric Measure Theory · Chapter 2, §3 equations (3.3), (3.5), and §4 equations (4.12), (4.14), printed pp.53–54, 58 (PDF pp.30–31,33) `](https://web.stanford.edu/class/math285/ts-gmt.pdf)


## Statement

Let $A\subset(C,h)$ be Borel and let $F:A\to(\Sigma,k)$ have a countable cover by local $C^1$ extensions as in the Jacobian definition. Put $D=F(A)$. With the normalized measures and the counting multiplicity defined above, the extended nonnegative integrals satisfy $\int_A J_2F\,d\mu_C=\int_D N(F,A;y)\,d\mathcal H_k^2(y)$. In particular $|D|\le\int_A J_2F\,d\mu_C$. If $F$ is one-to-one almost everywhere in the image sense $N=1$ for $\mathcal H_k^2$-almost every $y\in D$, equality holds in that inequality. If also $J_2F\le1$ almost everywhere, then $|D|\le|A|$. The image is countably two-rectifiable.

## Facts & Assumptions

[F1] Use the domain, normalized measures, Jacobian and counting multiplicity in [def-author-0336834a2590-measurable-surface-domains](item-def-author-0336834a2590-measurable-surface-domains), [def-author-0336834a2590-surface-map-jacobian](item-def-author-0336834a2590-surface-map-jacobian) and [def-author-0336834a2590-endpoint-multiplicity](item-def-author-0336834a2590-endpoint-multiplicity).

[F2] The Euclidean weighted area formula is the external input below; it includes measurable source subsets and counting multiplicity, rather than requiring injectivity.

[F3] Under the ZFC convention in [F1], an $L$-Lipschitz map between metric spaces satisfies $\mathcal H^2(f(E))\le L^2\mathcal H^2(E)$ for $L>0$. The common positive normalization preserves this inequality. [math:thm-hausdorff-measure-under-lipschitz-maps](https://alphabetamath.cc/item/thm-hausdorff-measure-under-lipschitz-maps)

## External input

Simon, Chapter 2, equations (3.3), (3.5), (4.12), (4.14), supplies the Euclidean weighted area formula with counting multiplicity and the tangent Gram Jacobian. This premise is imported. The Riemannian passage and endpoint consequences are proved locally below.

## Proof

**Given:** The objects and hypotheses of the Statement, with [F1]–[F3].

**Goal:** Prove the area identity, rectifiability, and the stated multiplicity bounds.

1.1 Use the ZFC, componentwise distance and normalized measure conventions in [F1]. Refine the countable extension cover into source coordinate balls with compact closures inside extension domains and with images in target charts, and subtract earlier balls to obtain a disjoint Borel partition $(A_i)$. Further such refinements remain countable. Bounded derivatives on smaller coordinate balls make each coordinate extension Lipschitz. The Jacobian supplier identifies its derivative with $d_AF$ almost everywhere on each partition piece; the multiplicity supplier gives measurability of each image and its count. With source metric matrix $H$, target metric matrix $K$ and coordinate derivative $B$, the coordinate density of $J_2F\,d\mu_C$ is $\sqrt{\det(B^TKB)}$, since the factor $\sqrt{\det H}$ cancels its reciprocal in $J_2F$. [F1, given, algebra]

2.1 Fix $0<\varepsilon<1$ and put $a=1-\varepsilon$, $b=1+\varepsilon$. Around each target point take linearly normalized coordinates with metric matrix equal to the identity at the center. Smoothness gives a coordinate ball $B_R$ on which $a^2I\le K\le b^2I$. Restrict to $B_r$ with $r<R/3$: straight segments give the upper distance bound $d_k(v^{-1}z,v^{-1}w)\le b|z-w|$. Curves staying in $B_R$ have length at least $a|z-w|$; a curve leaving it has initial displacement at least $R-r>2r\ge|z-w|$ before its first exit and obeys the same lower bound. Thus the restricted ambient component distance is at least $a|z-w|$ as well. Applying [F3] to the coordinate map and its inverse yields $a^2\mathcal H^2_{\mathrm E}(E)\le\mathcal H_k^2(v^{-1}E)\le b^2\mathcal H^2_{\mathrm E}(E)$ on this patch. Refine the partition in step 1.1 so every image lies in such a patch. The same quadratic-form bounds give $a^2\sqrt{\det(B^TB)}\le\sqrt{\det(B^TKB)}\le b^2\sqrt{\det(B^TB)}$; if $B$ has rank below two all three determinants vanish. [F1, F3, step 1.1, algebra]

3.1 Write $f_i=v_i\circ F\circ u_i^{-1}$ on $u_i(A_i)$ and let $N_i$ count preimages in $A_i$. Apply [F2] to the Lipschitz coordinate extension on this Borel subset of $\mathbb R^2$, with Euclidean target dimension three and normalized Euclidean measures. It gives $T_i:=\int_{u_i(A_i)}\sqrt{\det(Df_i^TDf_i)}\,d\lambda_2=\int_{f_i(u_i(A_i))}N_i(v_i^{-1}z)\,d\mathcal H^2_{\mathrm E}(z)$. Let $I_i=\int_{A_i}J_2F\,d\mu_C$ and $R_i=\int_{F(A_i)}N_i\,d\mathcal H_k^2$. Steps 1.1 and 2.1 give $a^2T_i\le I_i\le b^2T_i$ and $a^2T_i\le R_i\le b^2T_i$; the measure inequalities apply to nonnegative integrals by simple-function approximation. Hence $(a/b)^2I_i\le R_i\le(b/a)^2I_i$, also for infinite values. Since the source pieces are disjoint, $\sum_iN_i=N(F,A;\cdot)$, with counts extended by zero off their images, so summing gives $(a/b)^2I\le R\le(b/a)^2I$ for the two integrals $I,R$ in the Statement. Although the partition depends on $\varepsilon$, these full integrals do not. Let $\varepsilon$ decrease to zero: finite values are squeezed to equality, and an infinite value forces the other to be infinite. This proves the metric identity without assuming disjoint images. [F1, F2, step 1.1, step 2.1, algebra]

4.1 Each piece in step 1.1 is parametrized by a subset of $\mathbb R^2$; its coordinate extension is Lipschitz and the target inverse chart is Lipschitz for the component distance by step 2.1. These countably many maps cover $D$, proving countable two-rectifiability in the stated convention. Since $N\ge1$ on $D$, the identity gives $|D|\le I$. If $N=1$ almost everywhere on $D$, its right integral is $|D|$, giving equality. If also $J_2F\le1$ almost everywhere, then $I\le\mu_C(A)=|A|$. No injectivity or smoothness of the image cut was used. [F1, step 1.1, step 2.1, step 3.1] ∎

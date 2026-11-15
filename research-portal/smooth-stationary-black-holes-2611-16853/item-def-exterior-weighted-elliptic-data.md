---
title: Weighted exterior elliptic domains and admissible weights
status: draft
research_item: def-exterior-weighted-elliptic-data
dependency_level: 0
sources:
  references:
    - title: Armin Schikorra, Partial Differential Equations I & II (version October
        1, 2025)
      url: https://sites.pitt.edu/~armin/pde2022/pde.pdf
      locator: "Section 8, opening definitions surrounding Exercise 8.1, printed p.
        139 (PDF page 139): the displayed Hölder seminorm precedes the exercise;
        the C^{k,alpha} convention follows it on the same page."
      statement: The scalar Hölder seminorm is the supremum of |f(x)-f(y)|/|x-y|^alpha
        over distinct points of a Euclidean set; C^{k,alpha} requires C^k
        regularity and alpha-Hölder kth derivatives.
      hypotheses: A Euclidean domain, an integer k >= 0, and 0 < alpha <= 1; this item
        uses 0 < alpha < 1.
      reading_limits: Rechecked the extracted text of the opening definitions
        surrounding Exercise 8.1 on printed p. 139 (PDF page 139). This citation
        supplies only the unweighted Euclidean conventions; scaled and
        boundary-extension conventions use the declared library supplier. No
        weighted exterior theorem is imported.
---

## Prerequisites

- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)
- [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [` Armin Schikorra, Partial Differential Equations I & II (version October 1, 2025) · Section 8, opening definitions surrounding Exercise 8.1, printed p. 139 (PDF page 139): the displayed Hölder seminorm precedes the exercise; the C^{k,alpha} convention follows it on the same page. `](https://sites.pitt.edu/~armin/pde2022/pde.pdf)


## Definition

A smooth three-dimensional exterior here is a smooth three-manifold $\Sigma$ with compact smooth boundary $S=\partial\Sigma$, a compact subset whose complement is diffeomorphic to $\{x\in\mathbb R^3:|x|>r_0\}$ for some $r_0>0$, and a fixed such end chart $x$. Put $r=|x|$ on the end and $K=\Sigma\setminus\{r>2r_0\}$, and require $K$ to be compact as part of the exterior data. Equip $\Sigma$ with a smooth Riemannian metric $h$, meaning a smooth positive-definite symmetric covariant two-tensor.

Fix finitely many smooth interior or boundary charts and compact chart subsets $K_i$ covering $K$, each contained in its chart domain. Boundary charts take values in a half-space. For a scalar function $u$ of class $C^{k,\alpha}$ up to the boundary on compact sets, let $N_K(u)$ be the sum, over these fixed subsets, of the suprema of all coordinate derivatives of orders at most $k$ and the $\alpha$-Hölder seminorms of those of order $k$, taken over pairs of distinct points in the corresponding chart images of $K_i$. Here $[v]_{\alpha;E}=\sup_{x\ne y\in E}|v(x)-v(y)|/|x-y|^\alpha$, with an empty supremum interpreted as zero.

For an integer $k\ge0$, $0<\alpha<1$ and $\beta\in\mathbb R$, put $A_R=\{R<r<2R\}$ for $R\ge r_0$ and define

$$\|u\|_{C^{k,\alpha}_\beta}=N_K(u)+\sup_{R\ge r_0}R^{-\beta}\left(\sum_{j=0}^k R^j\max_{|I|=j}\sup_{A_R}|\partial_x^Iu|+R^{k+\alpha}\max_{|I|=k}[\partial_x^Iu]_{\alpha;A_R}\right).$$

The weighted Hölder space $C^{k,\alpha}_\beta$ consists of the real-valued functions just described for which this quantity is finite. The multi-index $I$ specifies repeated coordinate derivatives, and $|I|$ is their total order. Thus the convention is that $u$ has order at most $r^\beta$, with corresponding derivative and Hölder weights. Define the Dirichlet domain $X_\beta=\{u\in C^{4,\alpha}_\beta:u|_S=0\}$ and the target $Y_\beta=C^{2,\alpha}_{\beta-2}$. The restriction to $S$ is the continuous boundary value.

Write $\Delta_h$ for the Laplace–Beltrami operator with convention $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$, and for a real function $V$ write $\Delta_h-V$ for $u\mapsto\Delta_hu-Vu$. Its zeroth-order coefficient is $-V$, hence is nonpositive when $V\ge0$. The interval $-1<\beta<0$ is the weight range used in the separate exterior Dirichlet results; this definition asserts no Fredholm, index, invertibility, or completeness theorem and does not assert that this interval is the only possible one.

## Definition references

[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)

[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

## Justification

The compactness requirement on $K$ permits the finite compact chart cover: smaller coordinate balls or boundary half-balls with compact closures inside their chart domains give an open cover of $K$, from which a finite subcover is selected. The local Hölder and boundary-extension conventions give the displayed derivatives and continuous boundary values. The chosen chart subsets cover $K$, while the annuli cover the end beyond $r_0$; consequently the displayed quantity vanishes only for the zero function. Homogeneity and the triangle inequality follow term by term from those of absolute values and Hölder seminorms, so the finite-valued class is a normed vector space. The specified chart and compact-core choices are part of this definition; no equivalence under a change of choices is asserted here. The sign statement follows directly from the definition of multiplication by $V$.

## Source notes

The declared Hölder supplier provides the scaled-norm and boundary-extension conventions. Schikorra, Section 8, opening definitions on printed p. 139, was consulted for the ordinary Euclidean Hölder seminorm and the $C^{k,\alpha}$ convention only. The compact-core and weighted annular assembly is specified here.

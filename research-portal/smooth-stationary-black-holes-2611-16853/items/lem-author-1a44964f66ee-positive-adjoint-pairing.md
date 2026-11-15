---
id: lem-author-1a44964f66ee-positive-adjoint-pairing
title: Positive right and adjoint eigenfunctions have the same eigenvalue
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-1a44964f66ee-formal-adjoint
  - math:thm-compactness-under-continuous-maps
  - math:prop-smooth-maps-are-continuous
  - math:prop-identity-maps-and-composites-of-smooth-maps-are-smooth
  - math:def-dual-connection
  - math:def-product-connection-on-tensor-and-hom-bundles
  - math:thm-density-integration-is-defined-without-an-orientation
  - math:def-axiom-of-choice
dependency_roles:
  lem-author-1a44964f66ee-formal-adjoint: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:prop-smooth-maps-are-continuous: mathematical-premise
  math:prop-identity-maps-and-composites-of-smooth-maps-are-smooth: mathematical-premise
  math:def-dual-connection: mathematical-premise
  math:def-product-connection-on-tensor-and-hom-bundles: mathematical-premise
  math:thm-density-integration-is-defined-without-an-orientation: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

For the closed-manifold operator $L$ of the formal-adjoint lemma, assume $S$ is nonempty and suppose smooth functions $\phi>0$ and $\chi>0$ satisfy $L\phi=\lambda\phi$ and $L^\dagger\chi=\lambda^\dagger\chi$, with real constants $\lambda,\lambda^\dagger$. Then $\lambda=\lambda^\dagger$. Positivity and compactness also give $\min_S\phi>0$ and $\min_S\chi>0$, so division by either is smooth and bounded.

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The integration-by-parts identity holds for the smooth real functions in question. [[lem-author-1a44964f66ee-formal-adjoint]]

[F2] A continuous real-valued function on a nonempty compact space attains a maximum and a minimum. [[math:thm-compactness-under-continuous-maps]]

[F3] Smooth real-valued maps on smooth manifolds are continuous. [[math:prop-smooth-maps-are-continuous]]

[F4] The composite of two smooth maps between smooth manifolds is smooth. [[math:prop-identity-maps-and-composites-of-smooth-maps-are-smooth]]

[F5] The smooth Riemannian metric $h$ and its smooth Levi–Civita connection are those of the formal-adjoint setting. [[lem-author-1a44964f66ee-formal-adjoint]]

[F6] The dual connection on $T^*S$ and finite product connections on $(T^*S)^{\otimes j}$ are well-defined smooth connections, obey the tensor Leibniz rule, and are function-linear in their vector-field argument. [[math:def-dual-connection]] [[math:def-product-connection-on-tensor-and-hom-bundles]]

[F7] Assuming countable choice, integration of compactly supported smooth densities is linear and strictly positive on a nonzero nonnegative density. [[math:thm-density-integration-is-defined-without-an-orientation]]

[F8] The existing ZFC assumption includes the Axiom of Choice; applying it to countable families supplies the countable choice required by F7. [[math:def-axiom-of-choice]]

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The integration-by-parts identity holds for the smooth real functions in question. [[lem-author-1a44964f66ee-formal-adjoint]]

[F2] A continuous real-valued function on a nonempty compact space attains a maximum and a minimum. [[math:thm-compactness-under-continuous-maps]]

[F3] Smooth real-valued maps on smooth manifolds are continuous. [[math:prop-smooth-maps-are-continuous]]

[F4] The composite of two smooth maps between smooth manifolds is smooth. [[math:prop-identity-maps-and-composites-of-smooth-maps-are-smooth]]

[F5] The smooth Riemannian metric $h$ and its smooth Levi–Civita connection are those of the formal-adjoint setting. [[lem-author-1a44964f66ee-formal-adjoint]]

[F6] The dual connection on $T^*S$ and finite product connections on $(T^*S)^{\otimes j}$ are well-defined smooth connections, obey the tensor Leibniz rule, and are function-linear in their vector-field argument. [[math:def-dual-connection]] [[math:def-product-connection-on-tensor-and-hom-bundles]]

[F7] Assuming countable choice, integration of compactly supported smooth densities is linear and strictly positive on a nonzero nonnegative density. [[math:thm-density-integration-is-defined-without-an-orientation]]

[F8] The existing ZFC assumption includes the Axiom of Choice; applying it to countable families supplies the countable choice required by F7. [[math:def-axiom-of-choice]]

**Proof technique:** direct.

1.1 Use the adjoint identity with $f=\chi$ and $g=\phi$. Substituting the eigenvalue equations and using linearity in F7 gives $(\lambda-\lambda^\dagger)\int_S\chi\phi\,d\mu_h=0$. Since $S$ is nonempty, $\chi\phi\,d\mu_h$ is a nonzero positive smooth density. Its support is all of compact $S$, so F7 applies, with countable choice supplied by F8, and gives $\int_S\chi\phi\,d\mu_h>0$. Hence the eigenvalues agree. [F1, F7, F8]

2.1 By F3 the smooth real functions $\phi$ and $\chi$ are continuous. Apply F2 to them on the nonempty compact manifold $S$. Each attains its minimum at a point where its value is positive, giving $\min_S\phi>0$ and $\min_S\chi>0$. The map $r:(0,\infty)\to\mathbb R$, $r(s)=1/s$, is smooth: its derivative of order $j\ge0$ is $(-1)^j j!s^{-j-1}$. Since $\phi$ and $\chi$ take values in this open interval, F4 makes $1/\phi=r\circ\phi$ and $1/\chi=r\circ\chi$ smooth. They satisfy $1/\phi\le(\min_S\phi)^{-1}$ and $1/\chi\le(\min_S\chi)^{-1}$. For $u\in\{1/\phi,1/\chi\}$ define $\nabla^0u=u$ and $\nabla^{j+1}u=\nabla(\nabla^ju)$ using F5 and F6. Function-linearity in the differentiating vector field makes $\nabla^{j+1}u$ a covariant $(j+1)$-tensor; the smooth dual and product connections show inductively that all these tensors have smooth local components. For every fixed derivative order, the squared Riemannian norm of the corresponding covariant derivative of either smooth reciprocal is a smooth real function: in coordinates it is a finite contraction of smooth tensor components with the smooth inverse metric. It is continuous by F3 and bounded by F2, so its nonnegative square root, the Riemannian norm itself, is continuous and bounded as well. This proves all assertions. [F2, F3, F4, F5, F6, step 1.1] ∎

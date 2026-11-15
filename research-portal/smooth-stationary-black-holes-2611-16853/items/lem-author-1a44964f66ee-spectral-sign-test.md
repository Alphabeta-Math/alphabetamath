---
id: lem-author-1a44964f66ee-spectral-sign-test
title: Nonnegative supersolutions detect the principal spectral sign
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-1a44964f66ee-formal-adjoint
  - lem-author-1a44964f66ee-positive-adjoint-pairing
  - math:thm-density-integration-is-defined-without-an-orientation
  - math:prop-smooth-maps-are-continuous
  - math:def-axiom-of-choice
dependency_roles:
  lem-author-1a44964f66ee-formal-adjoint: mathematical-premise
  lem-author-1a44964f66ee-positive-adjoint-pairing: mathematical-premise
  math:thm-density-integration-is-defined-without-an-orientation: mathematical-premise
  math:prop-smooth-maps-are-continuous: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Let $(S,h)$ be a nonempty connected compact smooth Riemannian manifold without boundary, of positive dimension. Let $t$ be a smooth real vector field and $c$ a smooth real function on $S$. Put $Lu=-\Delta_hu+2\langle t,\nabla u\rangle_h+cu$, where $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. Use the positive Riemannian density $d\mu_h$ and the formal adjoint $L^\dagger u=-\Delta_hu-2\langle t,\nabla u\rangle_h+(c-2\operatorname{div}_ht)u$ for the pairing $\langle f,g\rangle=\int_S\overline f g\,d\mu_h$.

Assume smooth real functions $\phi>0$ and $\chi>0$ satisfy $L\phi=\lambda\phi$ and $L^\dagger\chi=\lambda\chi$ for a real constant $\lambda$. Then $\lambda\ge0$ if and only if there is a smooth real $\psi\ge0$, $\psi\not\equiv0$, with $L\psi\ge0$ pointwise. The strict variant $\lambda>0$ is equivalent to existence of such a $\psi$ with $L\psi$ additionally positive somewhere. Thus a nonnegative test function suffices; it is not necessary to assume the test is everywhere positive.

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] For the operator, manifold and density in the Statement, the formal-adjoint identity is $\int_S f Lg\,d\mu_h=\int_S(L^\dagger f)g\,d\mu_h$ for smooth real $f,g$. The operators have smooth real coefficients and map smooth real functions to smooth real functions. [[lem-author-1a44964f66ee-formal-adjoint]]

[F2] Positive right and adjoint eigenfunctions at real eigenvalues have the same eigenvalue; the Statement denotes this common value by $\lambda$. [[lem-author-1a44964f66ee-positive-adjoint-pairing]]

[F3] Compactly supported smooth density integration is linear, nonnegative on nonnegative densities and strictly positive on any nonzero nonnegative density, without an orientation assumption. Every smooth density on compact $S$ has compact support, so this applies to the density products below. The stated ZFC assumption includes AC; applying AC to countable families gives the countable-choice hypothesis $\mathrm{AC}_\omega$ required for this integration theorem. [[math:thm-density-integration-is-defined-without-an-orientation]] [[math:def-axiom-of-choice]]

[F4] Smooth real-valued maps on smooth manifolds are continuous; apply this to $\psi$ and the smooth function $L\psi$. [[math:prop-smooth-maps-are-continuous]]

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] For the operator, manifold and density in the Statement, the formal-adjoint identity is $\int_S f Lg\,d\mu_h=\int_S(L^\dagger f)g\,d\mu_h$ for smooth real $f,g$. The operators have smooth real coefficients and map smooth real functions to smooth real functions. [[lem-author-1a44964f66ee-formal-adjoint]]

[F2] Positive right and adjoint eigenfunctions at real eigenvalues have the same eigenvalue; the Statement denotes this common value by $\lambda$. [[lem-author-1a44964f66ee-positive-adjoint-pairing]]

[F3] Compactly supported smooth density integration is linear, nonnegative on nonnegative densities and strictly positive on any nonzero nonnegative density, without an orientation assumption. Every smooth density on compact $S$ has compact support, so this applies to the density products below. The stated ZFC assumption includes AC; applying AC to countable families gives the countable-choice hypothesis $\mathrm{AC}_\omega$ required for this integration theorem. [[math:thm-density-integration-is-defined-without-an-orientation]] [[math:def-axiom-of-choice]]

[F4] Smooth real-valued maps on smooth manifolds are continuous; apply this to $\psi$ and the smooth function $L\psi$. [[math:prop-smooth-maps-are-continuous]]

**Proof technique:** direct.

1.1 If $\lambda\ge0$, take $\psi=\phi$. Then $\psi$ is smooth, everywhere positive and nonzero because $S$ is nonempty, and $L\psi=\lambda\phi\ge0$. If $\lambda>0$, this is positive everywhere. This proves both forward implications. [given]

2.1 Conversely, let $\psi$ be a smooth real nonzero nonnegative function with $L\psi\ge0$. Adjoint integration gives $\int_S\chi L\psi\,d\mu_h=\int_S(L^\dagger\chi)\psi\,d\mu_h=\lambda\int_S\chi\psi\,d\mu_h$. The last integral is strictly positive: continuity and nonzero nonnegativity of $\psi$ give a nonempty open set where $\psi>0$, and $\chi$ is everywhere positive, so $\chi\psi\,d\mu_h$ is a nonzero nonnegative smooth density. The left side is nonnegative, hence $\lambda\ge0$. If $L\psi$ is positive at one point, its smoothness makes it positive on a nonempty open set. Then $\chi L\psi\,d\mu_h$ is also a nonzero nonnegative smooth density, so the left side is strictly positive and $\lambda>0$. Together with step 1.1 this proves both equivalences. [given, F1, F2, F3, F4, step 1.1] ∎

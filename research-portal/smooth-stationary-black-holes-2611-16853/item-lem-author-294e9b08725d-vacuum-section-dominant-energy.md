---
title: Vacuum exterior-section constraints imply the dominant energy condition
status: draft
research_item: lem-author-294e9b08725d-vacuum-section-dominant-energy
dependency_level: 4
sources:
  references: []
---

## Prerequisites

- [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [physics:thm-gr-constraint-equations-in-normal-frame](https://alphabetamath.cc/physics/item/thm-gr-constraint-equations-in-normal-frame)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density)
- [math:def-nonnegative-lebesgue-integral](https://alphabetamath.cc/item/def-nonnegative-lebesgue-integral)
- [math:def-integral-of-a-nonnegative-simple-function](https://alphabetamath.cc/item/def-integral-of-a-nonnegative-simple-function)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in the inherited ZFC convention. For the smooth exterior section $\overline C=C\cup S$ in a Ricci-flat spacetime, use $h=g|_{T\overline C}$ and $k=-g(\nabla n,\cdot)$. Define $\mu=\tfrac12(R_h-|k|_h^2+(\operatorname{tr}_h k)^2)$ and $J=\operatorname{div}_h k-d\operatorname{tr}_h k$. Then $\mu=0$ and $J=0$ on all of $\overline C$, including its boundary $S$. Hence $\mu\ge |J|_h$. No trace-zero condition is needed.

Here $(\mu,J)$ is integrable in the norm sense $\int_C(|\mu|+|J|_h)\,d\operatorname{vol}_h<\infty$, where $\operatorname{vol}_h$ is Riemannian Borel volume on the boundaryless interior $C$. For Borel $A\subset\overline C$, use the extension $\overline{\operatorname{vol}}_h(A)=\operatorname{vol}_h(A\cap C)$, which assigns $S$ measure zero; no boundary surface measure is included. Both $\int_C(|\mu|+|J|_h)\,d\operatorname{vol}_h$ and $\int_{\overline C}(|\mu|+|J|_h)\,d\overline{\operatorname{vol}}_h$ equal zero.

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[A1] The inherited regular-spacetime convention is ZFC, including the Axiom of Choice; it supplies the countable choice used by the Riemannian-volume theorem. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The section is smooth up to its boundary in the original smooth vacuum spacetime. [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F2] The normal-frame constraint identities express the Einstein normal components in terms of induced curvature and second fundamental form. [physics:thm-gr-constraint-equations-in-normal-frame](https://alphabetamath.cc/physics/item/thm-gr-constraint-equations-in-normal-frame) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F3] Under countable choice, the smooth Riemannian metric on the boundaryless interior $C$ determines its Riemannian Radon Borel volume measure $\operatorname{vol}_h$. [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density)

[F4] The nonnegative Lebesgue integral is the supremum of the integrals of nonnegative simple minorants. The simple integral uses the convention $0\cdot(+\infty)=0$. [math:def-nonnegative-lebesgue-integral](https://alphabetamath.cc/item/def-nonnegative-lebesgue-integral) [math:def-integral-of-a-nonnegative-simple-function](https://alphabetamath.cc/item/def-integral-of-a-nonnegative-simple-function)

## Proof

**Given:** The data and hypotheses of the Statement and the supplied facts above.

**Goal:** Prove the zero constraints and both norm-integrability conclusions.

1.1 Apply the constraint identities with $K=g(\nabla n,\cdot)=-k$. Ricci flatness makes both normal components of the Einstein tensor zero. The scalar identity is unchanged by $K\mapsto-k$ and yields $\mu=0$; the momentum identity changes sign and still yields $J=0$. Smoothness extends these identities to $S$. [F1, F2, algebra]

2.1 The dominant-energy inequality is $0\ge0$ by step 1.1. Apply the Riemannian-volume theorem to the smooth induced metric on $C$; the countable choice it assumes follows from the inherited Axiom of Choice by restricting to countable families. The nonnegative function $f=|\mu|+|J|_h$ is identically zero and is Borel measurable. Every nonnegative simple minorant of $f$ is zero and has simple integral zero, including when the total volume is infinite. Thus the defining supremum gives $\int_C f\,d\operatorname{vol}_h=0<\infty$. [A1, F3, F4, step 1.1]

3.1 The interior $C$ is open in $\overline C$, so $A\cap C$ is Borel in $C$ for every Borel $A\subset\overline C$. Intersection with $C$ preserves disjoint countable unions, so the displayed extension is a Borel measure by countable additivity of $\operatorname{vol}_h$, with $\overline{\operatorname{vol}}_h(S)=\operatorname{vol}_h(\varnothing)=0$. The same zero-function argument gives $\int_{\overline C}f\,d\overline{\operatorname{vol}}_h=0$. Thus norm integrability holds with the stated boundary convention, without imposing $\operatorname{tr}_h k=0$. [F1, F3, F4, step 1.1, step 2.1] ∎

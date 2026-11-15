---
title: Electrovac contraction in the normalized normal plane
status: draft
research_item: lem-author-6413ea293c6d-electrovac-normal-contraction
dependency_level: 6
---

## Prerequisites

- [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data)
- [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)
- [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)


## Statement

Under the geometric electrovac equations of [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data) and the oriented surface gauge of [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data), one has $\operatorname{Scal}_g=0$, $G=\operatorname{Ric}$ and $\operatorname{Ric}(L,\underline L)=e^2+b^2$. Here $F|_{TS}=b\,d\mu_q$ and $(\star F)|_{TS}=e\,d\mu_q$ are the actual oriented flux densities. This identity needs no vanishing assumption on the tangential electromagnetic components.

## Facts & Assumptions

[F1] The geometric electrovac equations use $\operatorname{Ric}_{ab}=2(F_{ac}F_b{}^c-g_{ab}F_{cd}F^{cd}/4)$, and the Hodge and surface orientations are fixed. [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data) [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)

[F2] Scalar curvature and the Einstein tensor mean $\operatorname{Scal}_g=g^{ab}\operatorname{Ric}_{ab}$ and $G_{ab}=\operatorname{Ric}_{ab}-\tfrac12\operatorname{Scal}_g g_{ab}$, with the same curvature and Ricci contraction convention as in [F1]. [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)

## Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Establish its identities with the indicated normalizations.

1.1 At a point choose an orthonormal frame $(n,\nu,E_1,E_2)$ with $(E_1,E_2)$ positively oriented on $S$. Put $a=F(n,\nu)$, $x_A=F(n,E_A)$, $y_A=F(\nu,E_A)$ and $c=F(E_1,E_2)$. Then $F_{ab}F^{ab}=2(-a^2-|x|^2+|y|^2+c^2)$. Direct substitution gives $\operatorname{Ric}(n,n)=a^2+|x|^2+|y|^2+c^2$ and $\operatorname{Ric}(\nu,\nu)=-a^2+|x|^2+|y|^2-c^2$. The trace of the defining electrovac equation is $\operatorname{Scal}_g=2(F_{ac}F^{ac}-4F_{cd}F^{cd}/4)=0$. [given, F1, F2, algebra]

2.1 Symmetry of Ric and $L=n+\nu$, $\underline L=(n-\nu)/2$ yield $\operatorname{Ric}(L,\underline L)=(\operatorname{Ric}(n,n)-\operatorname{Ric}(\nu,\nu))/2=a^2+c^2$. By the flux definitions $c=b$, while the Hodge definition in this orthonormal frame gives $e=\pm a$, with the sign fixed by the independently chosen spacetime orientation. Therefore $a^2+c^2=e^2+b^2$; the definition of $G$ and the zero scalar trace also give $G=\operatorname{Ric}$. [step 1.1, F1, F2, algebra] ∎

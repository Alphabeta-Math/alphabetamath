---
title: Stationary Lorentzian data and tensor conventions
status: draft
research_item: def-stationary-lorentzian-data
dependency_level: 0
sources:
  references:
    - title: Sean M. Carroll, Lecture Notes on General Relativity (1997)
      url: https://arxiv.org/pdf/gr-qc/9712019
      locator: Chapter 2, printed pp. 47 and 49 (PDF pp. 54 and 56), equations (2.28),
        (2.34) and adjacent metric/signature definitions.
      statement: A nondegenerate metric is a symmetric covariant two-tensor with an
        inverse; in four dimensions Lorentzian signature has one negative and
        three positive directions.
      hypotheses: A smooth four-manifold with the nondegenerate Lorentzian metric
        assumed here.
      reading_limits: Read the cited PDF passages only; time orientation is supplied
        by the declared library interface.
    - title: Sean M. Carroll, Lecture Notes on General Relativity (1997)
      url: https://arxiv.org/pdf/gr-qc/9712019
      locator: Chapter 5, printed pp. 135 and 140 (PDF pp. 142 and 147), equations
        (5.17)-(5.18) and (5.41).
      statement: The Lie derivative of the metric is its pullback derivative along the
        vector field flow at parameter zero; a Killing field has vanishing
        metric Lie derivative.
      hypotheses: A smooth metric and smooth vector field on a domain of its flow.
      reading_limits: Read the cited definitions; use is restricted to local flow
        domains, without completeness.
---

## Prerequisites

- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)
- [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)
- [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)
- [math:def-oriented-smooth-manifold-and-oriented-chart](https://alphabetamath.cc/item/def-oriented-smooth-manifold-and-oriented-chart)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [` Sean M. Carroll, Lecture Notes on General Relativity (1997) · Chapter 2, printed pp. 47 and 49 (PDF pp. 54 and 56), equations (2.28), (2.34) and adjacent metric/signature definitions. `](https://arxiv.org/pdf/gr-qc/9712019)
- [` Sean M. Carroll, Lecture Notes on General Relativity (1997) · Chapter 5, printed pp. 135 and 140 (PDF pp. 142 and 147), equations (5.17)-(5.18) and (5.41). `](https://arxiv.org/pdf/gr-qc/9712019)


## Definition

Work in ZFC, including the axiom of choice. Stationary Lorentzian data here consist of a connected smooth four-manifold $M$ without boundary, an orientation, a smooth Lorentzian metric $g$ of signature $(-,+,+,+)$, a time orientation $N$, and a smooth vector field $T$ satisfying $\mathcal L_Tg=0$. The orientation is a smooth choice of a positive ray in $\det T_pM$ at each point. The time orientation is a smooth field with $g(N,N)<0$; a timelike vector $v$ is future-directed when $g(v,N)<0$.

The metric is a smooth symmetric nondegenerate covariant two-tensor with one negative and three positive directions at each point. The Lie derivative $\mathcal L_Tg$ is $\frac{d}{dt}|_{t=0}\Phi_t^*g$, where $\Phi_t$ is the local flow of $T$; a field satisfying its vanishing is called a Killing field. Thus stationary refers here to the specified pair $(g,T)$; it does not assert that $T$ is timelike everywhere or that its flow is complete. For a designated open region called an end, the additional convention that it is a stationary end requires $T$ to be future timelike throughout that region. Further topology or asymptotic conditions on an end must be stated separately.

Let $\nabla$ be the Levi–Civita connection: the unique torsion-free affine connection compatible with $g$. Its curvature convention is $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$. In a coordinate frame write $R(\partial_c,\partial_d)\partial_b=R^a{}_{bcd}\partial_a$ and $\operatorname{Ric}_{bd}=R^a{}_{bad}$. The Ricci tensor is denoted $\operatorname{Ric}(g)$.

Put $T^\flat=g(T,\cdot)$ and $f=-g(T,T)$. In coordinates, $T_a=g_{ab}T^b$ and $g^{ab}$ denotes the inverse matrix of $g_{ab}$. Repeated upper and lower indices are summed from $0$ to $3$. Raising indices uses $g^{ab}$ and lowering them uses $g_{ab}$; a contraction or raised tensor associated with another metric uses that metric and its own inverse.

## Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)

[math:def-oriented-smooth-manifold-and-oriented-chart](https://alphabetamath.cc/item/def-oriented-smooth-manifold-and-oriented-chart)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[A1] The set-theoretic convention is ZFC, including the axiom of choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The Lorentzian interface gives the metric, time-orientation and future-directed conventions stated above. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[F2] The Killing-field interface defines the Lie derivative using the local flow and defines a Killing field by its vanishing. [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[F3] A metric-selected connection is torsion-free and metric-compatible; for the stated smooth nondegenerate metric there is exactly one such connection. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection) [physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[F4] The inverse-metric interface supplies the inverse and the lowering and raising maps for the stated nondegenerate metric. [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[F5] The curvature interface fixes the displayed curvature and Ricci conventions for the metric-selected connection. [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)

[F6] An orientation is a smooth choice of a ray in the determinant line of each tangent space. [math:def-oriented-smooth-manifold-and-oriented-chart](https://alphabetamath.cc/item/def-oriented-smooth-manifold-and-oriented-chart)

## Justification

**Given:** The data and hypotheses in the Definition.

**Goal:** Show that the named fields and conventions are well-defined under those hypotheses.

1.1 The metric and time-orientation hypotheses place $(M,g,N)$ in the Lorentzian interface; the chosen orientation is the determinant-line datum in that interface's smooth-manifold setting. The local-flow Lie derivative and the Killing condition therefore have the stated meanings. The end condition is a further pointwise requirement on the designated region, not an assertion that such a region exists. [given, F1, F2, F6]

2.1 Nondegeneracy and smoothness supply the unique metric-compatible torsion-free connection and the inverse metric. The curvature interface then supplies the displayed Ricci contraction, while $T^\flat$ and $f$ are pointwise contractions of the supplied smooth fields. Raising and lowering with the inverse and metric of the metric currently specified is consequently unambiguous. This establishes the stated conventions without asserting completeness or an existence theorem for an end. [given, F3, F4, F5, step 1.1] ∎

## External input

Carroll supplies the symmetric nondegenerate metric and Lorentzian signature conventions in Chapter 2. The flow definition of the Lie derivative and the Killing condition are recorded in Chapter 5; only their restriction to local flow domains is used here. Time orientation and future direction use the declared Lorentzian interface.

---
id: def-source-free-geometric-electrovacuum-data
title: Geometric electrovacuum equations and charge convention
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:def-emg-lorentzian-forms
  - physics:lem-emg-lorentz-hodge-calculus
  - physics:def-emg-xs-geometric-electrovac
  - math:prop-integration-over-an-oriented-embedded-submanifold
  - math:def-axiom-of-choice
  - math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges
  - math:def-compactly-supported-differential-form
  - math:thm-closed-subspace-of-a-compact-space-is-compact
  - math:prop-reversing-orientation-negates-the-integral
dependency_roles:
  physics:def-emg-lorentzian-forms: mathematical-premise
  physics:lem-emg-lorentz-hodge-calculus: mathematical-premise
  physics:def-emg-xs-geometric-electrovac: mathematical-premise
  math:prop-integration-over-an-oriented-embedded-submanifold: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges: mathematical-premise
  math:def-compactly-supported-differential-form: mathematical-premise
  math:thm-closed-subspace-of-a-compact-space-is-compact: mathematical-premise
  math:prop-reversing-orientation-negates-the-integral: mathematical-premise
provenance:
  statement: ai-generated
  proof: not-applicable
dependency_level: 0
---

## Definition

Work with the Axiom of Choice, in particular countable choice. Let $M$ be a smooth Hausdorff second-countable four-manifold without boundary, $g$ a smooth Lorentzian metric of signature $(-,+,+,+)$, $N$ a smooth timelike field selecting the future direction, and $o$ an independently specified orientation. Let $F$ be a smooth real two-form. The metric-selected connection is the torsion-free metric-compatible connection $\nabla$; use $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$ and its Ricci contraction $\operatorname{Ric}_{bd}=R^a{}_{bad}$. These conventions follow [[physics:def-emg-lorentzian-forms]].

The Hodge map $\star_g$ is determined by $g$ and $o$ through $\alpha\wedge\star_g\beta=\langle\alpha,\beta\rangle_g\,\mathrm{vol}_g$, where the pairing is the metric-induced pairing on forms and $\mathrm{vol}_g$ agrees with $o$; see [[physics:lem-emg-lorentz-hodge-calculus]]. A **source-free geometric electrovacuum datum** is the tuple $(M,g,N,o,F)$ satisfying the equations in [[physics:def-emg-xs-geometric-electrovac]] with zero cosmological constant:

$$dF=0,\qquad d(\star_gF)=0,\qquad \operatorname{Ric}_{ab}=2\left(F_{ac}F_b{}^c-\frac14g_{ab}F_{cd}F^{cd}\right).$$

Indices are raised using $g^{-1}$. These are defining tensor equations, with no global potential, asymptotic flatness, horizon, or existence assertion included.

Let $S\subset M$ be a compact oriented smooth embedded two-manifold without boundary. It is **spacelike** when the restriction of $g$ to every tangent plane $T_pS$ is positive definite. Its orientation is specified independently of $o$. With $i:S\hookrightarrow M$ the inclusion, define the geometric electric and magnetic flux parameters by

$$Q_E(S):=\frac1{4\pi}\int_S i^*(\star_gF),\qquad Q_M(S):=\frac1{4\pi}\int_S i^*F.$$

The orientation and factor $4\pi$ are fixed before charges are compared; no SI constants are inserted into this normalization.

## Justification

The cited Lorentzian and Hodge suppliers define the connection, curvature, exterior derivative and smooth Hodge map under the stated hypotheses. The equations therefore compare smooth tensors of matching types and select a class of tuples; they do not assert that a specified tuple satisfies them. The electrovacuum supplier fixes the displayed curvature and flux normalization. For the broader surfaces used here, the inclusion $i:S\hookrightarrow M$ is smooth, so [[math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges]] makes $i^*F$ and $i^*(\star_gF)$ smooth two-forms on $S$. By [[math:def-compactly-supported-differential-form]], the support of each is the closure in $S$ of its nonzero locus. Each support is therefore closed in compact $S$ and is compact by [[math:thm-closed-subspace-of-a-compact-space-is-compact]]. [[math:prop-integration-over-an-oriented-embedded-submanifold]] supplies their integrals and invariance under orientation-preserving reparametrization. Thus both displayed fluxes are well-defined real numbers. With $g$, $o$ and $F$ fixed, reversing the chosen orientation of $S$ leaves both pulled-back forms unchanged and negates each integral by [[math:prop-reversing-orientation-negates-the-integral]], applied to these compactly supported top forms. Thus both flux signs reverse. The choice assumption includes the countable choice carried by the Lorentzian and Hodge suppliers.

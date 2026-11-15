---
id: def-bifurcate-killing-horizon-data
title: Bifurcate Killing horizons, rotation and normalization
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-killing-field
  - physics:def-gr-metric-selected-connection
  - physics:thm-gr-killing-and-on-shell-matter-identities
  - physics:def-emg-causal-solution-and-horizon-vocabulary
  - math:def-axiom-of-choice
dependency_roles:
  physics:def-gr-killing-field: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  physics:thm-gr-killing-and-on-shell-matter-identities: mathematical-premise
  physics:def-emg-causal-solution-and-horizon-vocabulary: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: H. S. Reall, General Relativity (Part III, October 12, 2022)
      url: https://www.damtp.cam.ac.uk/user/hsr1000/part3_gr_lectures.pdf
      locator: Section 5.3, printed p. 56 (PDF p. 57), equations (5.21)–(5.22) and
        adjacent Killing-field text.
      statement: For a smooth metric with its Levi–Civita connection, $(\mathcal L_X
        g)_{ab}=\nabla_aX_b+\nabla_bX_a$; vanishing of this tensor is the
        Killing equation.
      hypotheses: A smooth vector field X and smooth metric g with its Levi–Civita
        connection; indices of X are lowered with g.
      reading_limits: Consulted equations (5.21)–(5.22) and adjacent text on printed
        p. 56 in the linked PDF. This reference supports only the Killing
        identity. The horizon, dense nonzero-generator and bifurcation-extension
        conventions are supplied by the declared mathematical library item, not
        this citation.
dependency_level: 0
---

## Definition

Work in a smooth time-oriented Lorentzian four-manifold $(M,g)$ of signature $(-,+,+,+)$, with metric-compatible Levi–Civita connection $\nabla$, and let $K$ be a smooth Killing field, meaning $\mathcal L_K g=0$. A smooth embedded hypersurface $H$ is **null** if the restriction of $g$ to each tangent space $T_pH$ has a nonzero radical: the vectors in $T_pH$ orthogonal to all of $T_pH$. It is a **Killing horizon for $K$** when $H_*:=\{p\in H:K_p\ne0\}$ is nonempty and dense in $H$ and, on $H_*$, $K$ is tangent and normal to $H$. The null normal line is the radical of the induced form. An **integral curve of this line field**, or **horizon generator**, means here a smooth curve $\gamma:I\to H$, where $I\subset\mathbb R$ is a nonempty open interval, such that $\dot\gamma(s)\ne0$ and $\dot\gamma(s)$ lies in the null normal line at $\gamma(s)$ for every $s\in I$. Curves related by a smooth diffeomorphic reparameterization are identified; restrictions to open subintervals are allowed generator segments. No maximality, completeness, affine parametrization or preferred parameter scale is implicit.

The **signed surface gravity** of this specified $K$ on $H_*$ is the unique smooth scalar $\kappa_H$ satisfying the ambient covector equation $d(g(K,K))=-2\kappa_H K^\flat$, where $K^\flat=g(K,\cdot)$. Equivalently, $\nabla_KK=\kappa_H K$ on $H_*$. A chosen future branch is a specified branch with its future direction; neither the sign nor constancy of $\kappa_H$ follows from the terminology.

A **bifurcate Killing horizon** here consists of two distinct specified smooth embedded null hypersurfaces $H_+$ and $H_-$ in a common neighborhood of a smooth spacelike embedded two-surface $S$, each a Killing horizon for the same $K$, such that $K=0$ on $S$, their intersection near each point of $S$ is $S$, and $T_pH_+\cap T_pH_-=T_pS$. Spacelike means that the induced metric on $S$ is positive definite. The surface $S$ is the **bifurcation surface**. A surface-gravity value at $p\in S$ is specified by the common value only when the two branch scalars extend smoothly to $p$ along their respective branches and agree there. The equation at $K=0$ alone fixes no value.

For a specified stationary Killing field $T$, meaning a Killing field timelike on a specified nonempty open region, a horizon is **non-rotating relative to $T$** if $T_p$ lies in the null normal line at every point of the horizon; it is **rotating relative to $T$** if that tangency fails somewhere. Zero vectors satisfy the tangency condition. A **normalization** specifies the scale of $K$; replacing $K$ by $aK$ for a nonzero constant $a$ replaces $\kappa_H$ by $a\kappa_H$. Thus a numerical surface gravity, or boost rate when that term is used for this normalized scalar, requires the normalization to be stated. No existence, constancy, nonzero-value, field-equation or global-extension assertion is included.

## Definition references

[[physics:def-gr-killing-field]]

[[physics:def-gr-metric-selected-connection]]

[[physics:thm-gr-killing-and-on-shell-matter-identities]]

[[physics:def-emg-causal-solution-and-horizon-vocabulary]]

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice, which supplies the countable choice used in the inherited smooth-manifold conventions. [[math:def-axiom-of-choice]]

[F1] The horizon supplier defines the signed scalar on the nonzero-generator part and the bifurcation surface with the stated transversality and extension qualifications. [[physics:def-emg-causal-solution-and-horizon-vocabulary]]

[F2] A Killing field satisfies $\nabla_aK_b+\nabla_bK_a=0$, and the metric-selected connection is metric compatible. [[physics:thm-gr-killing-and-on-shell-matter-identities]] [[physics:def-gr-metric-selected-connection]]

## Justification

The horizon supplier establishes that the scalar in the ambient covector equation exists uniquely and smoothly on $H_*$; density makes a continuous extension unique if it exists. By metric compatibility and the Killing equation, $\nabla_a(g(K,K))=2K^b\nabla_aK_b=-2K^b\nabla_bK_a$. Nondegeneracy of $g$ therefore makes the covector equation equivalent to $\nabla_KK=\kappa_H K$. Rescaling $K$ by a nonzero constant multiplies the left side of the covector equation by $a^2$ and $K^\flat$ by $a$, giving the stated rescaling of $\kappa_H$. The null normal line and tangency condition are pointwise conditions on the specified data; the definition does not assert that suitable data exist.

## External input

The horizon and bifurcation definitions, including existence and smoothness of the signed scalar on $H_*$, are supplied by [[physics:def-emg-causal-solution-and-horizon-vocabulary]] under its Definition (b) hypotheses and Proof 2.1. Reall, Section 5.3, equations (5.21)–(5.22), independently states the Killing-equation characterization used in [F2]. [General Relativity, printed p. 56](https://www.damtp.cam.ac.uk/user/hsr1000/part3_gr_lectures.pdf) This lecture-note citation is limited to that identity; the horizon, density and branch-extension conventions come from the declared mathematical supplier.

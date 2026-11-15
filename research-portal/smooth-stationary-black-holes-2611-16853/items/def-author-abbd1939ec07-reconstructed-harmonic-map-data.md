---
id: def-author-abbd1939ec07-reconstructed-harmonic-map-data
title: Harmonic-map and Weyl reconstruction comparison data
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-author-abbd1939ec07-ordered-vacuum-rods
  - math:thm-zero-derivative-on-connected-open-euclidean-set-iff-constant
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-author-abbd1939ec07-ordered-vacuum-rods: mathematical-premise
  math:thm-zero-derivative-on-connected-open-euclidean-set-iff-constant: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Han–Khuri–Weinstein–Xiong, Kerr Black Hole Uniqueness
      url: https://arxiv.org/html/2608.23325v1
      locator: §1, equations (1.1)–(1.4), the target-metric display immediately after
        (1.2), and the normalization paragraph immediately after (1.4).
      statement: For axisymmetric maps from Euclidean three-space minus its rotation
        axis to the target with metric $du^2+e^{4u}dv^2$, the harmonic-map
        equations are $\Delta u=2e^{4u}|\nabla v|^2$ and $\Delta v+4\nabla
        u\cdot\nabla v=0$. With $U=u+\log\rho$, the source displays the
        Weyl–Papapetrou metric (1.1), exactly the four reconstruction
        quadratures adopted in this Definition in (1.3)–(1.4), and the
        normalization $w\to0$, $\alpha\to0$ at infinity.
      hypotheses: The source setting is a stationary axisymmetric vacuum metric in
        Weyl–Papapetrou coordinates off the rotation axis, with rotational
        period 2π and Euclidean derivatives for the harmonic-map system. Here
        only the explicit map equation, metric ansatz, quadratures and
        normalization are adopted as mathematical data; w and α are supplied
        functions. This citation is not used to reduce an arbitrary stationary
        geometry or establish global existence or axis regularity.
      reading_limits: Consulted the source HTML §1 setting paragraph and equations
        (1.1)–(1.4), including the displayed target metric and the paragraph
        fixing the additive constants. The substantial reduction, integrability
        and global reconstruction arguments and the cited underlying papers were
        not checked or reconstructed; no such theorem is imported.
dependency_level: 6
---

## Definition

Let $\Gamma=\{\rho=0\}\subset\mathbb R^3$ be the rotation axis in cylindrical coordinates $(\rho,z,\phi)$, with $\phi$ of period $2\pi$. A reconstructed vacuum-map datum consists of the ordered rods of the ordered finite vacuum rod datum, two smooth real axisymmetric functions $u,v$ on $\mathbb R^3\setminus\Gamma$, and smooth functions $w,\alpha$ there, satisfying $\Delta u=2e^{4u}|\nabla v|^2$ and $\Delta v+4\nabla u\cdot\nabla v=0$. Derivatives and norms here are Euclidean. Equivalently these are the harmonic-map equations for the explicitly specified target metric $du^2+e^{4u}dv^2$; only the displayed equations are used in this contract.

Put $U=u+\log\rho$. Require the reconstruction equations $w_\rho=2\rho e^{4u}v_z$, $w_z=-2\rho e^{4u}v_\rho$, $\alpha_\rho=\rho[U_\rho^2-U_z^2+e^{4u}(v_\rho^2-v_z^2)]$, and $\alpha_z=2\rho[U_\rho U_z+e^{4u}v_\rho v_z]$, together with $w\to0$ and $\alpha\to0$ at infinity. Define the reconstructed metric by $\mathbf g=-e^{2U}d\tau^2+\rho^2e^{-2U}(d\phi+w\,d\tau)^2+e^{-2U+2\alpha}(d\rho^2+dz^2)$ on $\mathbb R_\tau\times(\mathbb R^3\setminus\Gamma)$. The datum supplies $w,\alpha$; their global existence or a reduction of arbitrary stationary geometries is not part of the definition.

## Definition references

[[def-author-abbd1939ec07-ordered-vacuum-rods]]

[[def-stationary-lorentzian-data]]

## Facts & Assumptions

[F1] The supplied rods and twist labels are [[def-author-abbd1939ec07-ordered-vacuum-rods]]. Lorentzian tensor and stationary-field conventions are [[def-stationary-lorentzian-data]]. Axisymmetry means independence of $\phi$.

[F2] A totally differentiable real function with zero derivative on a nonempty connected open Euclidean set is constant, by [[math:thm-zero-derivative-on-connected-open-euclidean-set-iff-constant]]. The orbit half-plane $H=(0,\infty)\times\mathbb R$ is nonempty, open and convex, hence connected.

[F3] The harmonic-map interpretation and the displayed reconstruction formulas use the precise HKWX input recorded in External input and in the source contract; the supplied functions and their normalization are the hypotheses for the local argument.

## Justification

**Given:** Functions satisfying the stated equations and normalization, with the inputs in [F1]–[F3].

**Goal:** Verify that their reconstructed tensor is a well-defined stationary Lorentzian metric off the axis, and that the normalized reconstruction is unique conditional on existence.

1.1 Let $f$ be either $w$ or $\alpha$, and fix any two angular values $\phi_1,\phi_2$. On $H$, put $q(\rho,z)=f(\rho,z,\phi_1)-f(\rho,z,\phi_2)$. The right sides of the reconstruction equations are independent of $\phi$, because $u,v,U$ are axisymmetric. Thus $q$ is smooth with $q_\rho=q_z=0$. By [F2], $q$ is constant on $H$. Along $(\rho,z)=(R,0)$ with $R\to\infty$, both terms tend to zero by the normalization, so this constant is zero. As the angles were arbitrary, $w$ and $\alpha$ are axisymmetric. [given, F1, F2, algebra]

2.1 On $\rho>0$, all exponential coefficients are smooth and positive. The angular one-form $d\phi$ is globally defined off the axis: local angular coordinates differ by constant multiples of $2\pi$, so their differentials agree. The coframe $d\tau$, $d\phi+w\,d\tau$, $d\rho$, $dz$ is linearly independent, and the displayed tensor is diagonal in it with exactly one negative coefficient. Thus it is a smooth nondegenerate Lorentzian metric globally off the axis. Its coefficients are independent of $\tau$ by construction and of $\phi$ by step 1.1, so time translations and rotations preserve it; in particular $\partial_\tau$ is Killing in the stationary-field convention. [given, F1, step 1.1, algebra]

3.1 For fixed $u,v$ and two supplied normalized reconstruction pairs $(w,\alpha)$ and $(\widetilde w,\widetilde\alpha)$, fix $\phi$ and restrict each difference to $H$. The reconstruction equations give zero $\rho,z$ derivatives, so [F2] makes each difference constant on $H$. Along $(R,0)$ the zero limits of both pairs force each constant to vanish. This holds for every $\phi$, giving equality on the full off-axis domain. The reconstruction equalities are definite scalar predicates, and this argument establishes uniqueness conditional on existence without an integrability, global-existence or geometric-reduction assertion. [given, F2, step 2.1, algebra] ∎

## External input

HKWX §1 equation (1.2) and its following target-metric display identify the two stated PDEs as the axisymmetric harmonic-map equations from Euclidean $\mathbb R^3\setminus\Gamma$ into the target with metric $du^2+e^{4u}dv^2$. Equations (1.1), (1.3) and (1.4), and the paragraph after (1.4), supply the metric ansatz, reconstruction quadratures and zero normalization adopted here. This is an imported identification of the displayed equations, not a claimed local proof of a stationary-vacuum reduction or a global reconstruction theorem. The Lorentzian-signature, symmetry and conditional-uniqueness arguments above are local.

---
id: lem-author-69e1abcd87be-regular-axis-elementary-flatness
title: Weight-one regular axis gives elementary flatness of small axial orbits
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-black-hole-comparison-hypothesis-data
  - def-stationary-lorentzian-data
  - physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative
  - physics:thm-gr-local-geodesics-and-exponential-map
  - math:thm-multivariable-taylor-formula-with-lagrange-remainder
  - math:thm-heine-borel-rn
  - math:thm-extreme-value-metric
  - math:thm-chain-rule-for-total-derivatives
  - math:thm-clairaut-schwarz-mixed-partials
  - math:lem-continuous-functions-riemann-integrable
dependency_roles:
  def-black-hole-comparison-hypothesis-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  math:thm-multivariable-taylor-formula-with-lagrange-remainder: mathematical-premise
  math:thm-heine-borel-rn: mathematical-premise
  math:thm-extreme-value-metric: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:thm-clairaut-schwarz-mixed-partials: mathematical-premise
  math:lem-continuous-functions-riemann-integrable: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 5
---

## Statement

Let $p$ lie on the regular axis of the specified smooth axial isometric circle action. Its differential on the spacelike normal plane is the weight-one rotation of period $2\pi$. If a smooth transverse curve $\gamma(\rho)$ satisfies $\gamma(0)=p$ and $\gamma'(0)=v$ for a unit vector in this normal plane, then the small axial orbit of $\gamma(\rho)$ is spacelike for small positive $\rho$, and its length is $2\pi\rho+O(\rho^2)$. The radial curve segment has length $\rho+O(\rho^2)$; the ratio tends to $2\pi$. This verifies the local absence of a conical defect under the assumed smooth, weight-one axis data.

For a smooth spacelike parametrized curve $c:[a,b]\to M$ with $a<b$, its length here means $L_g(c):=\int_a^b\sqrt{g_{c(t)}(c'(t),c'(t))}\,dt$, with the positive square root and the ordinary Riemann integral; set $L_g(c)=0$ for a singleton parameter interval. Spacelike means $g_{c(t)}(c'(t),c'(t))>0$ throughout the parameter interval. The radial segment is $\gamma|_{[0,\rho]}$; orbit length uses one traversal with $s\in[0,2\pi]$.

## Facts & Assumptions

[F1] The specified regular-axis data give a jointly smooth isometric circle action $\psi_s$, its fixed two-dimensional submanifold $A$, and the spacelike normal plane $N_p=(T_pA)^{\perp_g}$. At $p\in A$, $D_p\psi_s$ is the identity on $T_pA$ and the weight-one rotation $R_s$ on $N_p$. Thus $T_pM=T_pA\oplus N_p$. These are imposed data, not consequences of global hyperbolicity. [[def-black-hole-comparison-hypothesis-data]]

[F2] Use the smooth Lorentzian metric and inherited ZFC convention of the stationary data. In the displayed length definition, metric evaluation on a curve's tangent is a scalar; for a smooth spacelike curve it is positive and continuous, so its positive square root is continuous. The integral of a continuous real function on a closed interval exists. If $m\le f\le M$ there, its integral lies between $m(b-a)$ and $M(b-a)$. This constructs the lengths used here without requiring the ambient metric to be positive definite. [[def-stationary-lorentzian-data]] [[math:lem-continuous-functions-riemann-integrable]]

[F3] The smooth nondegenerate metric has a unique torsion-free metric-compatible connection. [[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative]]

[F4] Geodesics have unique initial-value solutions. The exponential map is smooth, satisfies $d(\exp_p)_0=\operatorname{id}_{T_pM}$, and restricts to a diffeomorphism on a sufficiently small neighborhood of the zero tangent vector. [[physics:thm-gr-local-geodesics-and-exponential-map]]

[F5] For a scalar $C^2$ function on an open convex Euclidean set, the degree-one Taylor formula along a segment has a degree-two Lagrange remainder. A bound on second derivatives along those segments therefore bounds that remainder by a constant times the squared increment. Apply this componentwise to the smooth coordinate functions below. [[math:thm-multivariable-taylor-formula-with-lagrange-remainder]]

[F6] Closed bounded Euclidean boxes and intervals are compact. A continuous real-valued function on a nonempty compact metric space is bounded. In particular continuous derivatives have finite bounds on the compact boxes used below; finite subcovers also give a common parameter neighborhood of the compact circle interval. [[math:thm-heine-borel-rn]] [[math:thm-extreme-value-metric]]

[F7] The derivative of a composite is the composite of its derivatives, and the two orders of mixed second partial derivatives agree for a $C^2$ scalar function on an open Euclidean set. Apply these facts componentwise to smooth coordinate maps. [[math:thm-chain-rule-for-total-derivatives]] [[math:thm-clairaut-schwarz-mixed-partials]]

## Proof

**Given:** The data and assumptions in the Statement.

**Goal:** Establish the claimed conditional conclusion.

1.1 Fix a chart $x:U\to\mathbb R^4$ with $x(p)=0$ and an open coordinate box $B$ about $0$ whose closure lies in $x(U)$. For each $s\in[0,2\pi]$, joint continuity and $\psi_s(p)=p$ give a product neighborhood of $(s,0)$ mapped into $x^{-1}(B)$. A finite subcover of $[0,2\pi]$ gives $\epsilon>0$ such that $F(s,\rho):=x(\psi_s(\gamma(\rho)))$ is smooth on a neighborhood of $K=[0,2\pi]\times[0,\epsilon]$ and takes values in $B$ there, after shrinking $\epsilon$. Put $X=\partial_sF$. Then $F(s,0)=0$, $X(s,0)=0$, and the chain rule gives $\partial_\rho F(s,0)=d x_p(R_sv)$. If $J$ is the unit quarter-turn generator on $N_p$, commuting the mixed derivatives gives $\partial_\rho X(s,0)=d x_p(R_sJv)$. [F1, F2, F6, F7, given, construct]

1.2 The period interval counts one orbit. Indeed, pulling back the connection by an isometry preserves torsion freedom and metric compatibility, so uniqueness makes that pullback the original connection. Isometries therefore take geodesics to geodesics, and uniqueness of their initial-value solutions gives $\psi_s(\exp_p w)=\exp_p(D_p\psi_s w)$ whenever these expressions are defined. Choose an auxiliary positive definite norm on $T_pA$, combine it with $g_p|_{N_p}$ on the direct sum, and take a sufficiently small ball $W$ for this norm inside the exponential diffeomorphism neighborhood. The identity-plus-rotation action preserves $W$, so both exponential expressions lie in its injectivity domain for every $s$. For small $\rho$, put $w(\rho)=(\exp_p|_W)^{-1}(\gamma(\rho))$. The inverse differential at $p$ is the identity by the chain rule; hence $w(0)=0$ and $w'(0)=v$. Taylor's formula and a bound on $w''$ on a small compact interval give $w(\rho)=\rho v+O(\rho^2)$. Its normal component is nonzero for small positive $\rho$. Since the tangent component is fixed and a weight-one rotation fixes a nonzero normal vector only for $s\in2\pi\mathbb Z$, injectivity of $\exp_p|_W$ shows that $\psi_s(\gamma(\rho))=\gamma(\rho)$ only for such $s$. [F1, F3, F4, F5, F6, F7, given, construct, algebra]

2.1 The continuous components of $\partial_\rho^2X$ are bounded on $K$ by compactness. Taylor's formula on each fixed-$s$ segment therefore gives $X(s,\rho)=\rho\,d x_p(R_sJv)+O(\rho^2)$ with a constant independent of $s$. To apply the stated open-convex-set version, each scalar component is restricted to an open interval about $[0,\epsilon]$ at that fixed $s$; its remainder evaluation point lies in $K$, where the same bound applies. The same bounded-derivative argument gives $F(s,\rho)=O(\rho)$ uniformly. The first and second coordinate derivatives of the metric components are bounded on $\overline B$, so Taylor's formula along the coordinate segment from $0$ to $F(s,\rho)$ gives $g_{ab}(F(s,\rho))=g_{ab}(0)+O(\rho)$ uniformly. The leading vectors $R_sJv$ are uniformly bounded in these coordinates and have $g_p(R_sJv,R_sJv)=1$. Consequently the squared orbit speed $q(s,\rho):=g_{\psi_s(\gamma(\rho))}(\partial_s\psi_s(\gamma(\rho)),\partial_s\psi_s(\gamma(\rho)))$ satisfies $q(s,\rho)=\rho^2+O(\rho^3)$ uniformly for $s\in[0,2\pi]$ and is positive for sufficiently small $\rho>0$. [step 1.1, F1, F2, F5, F6, algebra]

3.1 Write the squared orbit speed as $q(s,\rho)=\rho^2(1+e(s,\rho))$, with $|e(s,\rho)|\le C\rho$ uniformly by step 2.1. For small positive $\rho$, $1+e>0$ and $|\sqrt{1+e}-1|=|e|/(\sqrt{1+e}+1)\le |e|$. Thus its speed lies between $\rho-C\rho^2$ and $\rho+C\rho^2$. The length definition and the continuous-integral bounds give orbit length $2\pi\rho+O(\rho^2)$, counted once by step 1.2. Along the transverse curve, the smooth scalar $h(t)=g_{\gamma(t)}(\gamma'(t),\gamma'(t))$ has $h(0)=1$. Bounded derivatives on a small compact interval and Taylor's formula give $h(t)=1+O(t)$, which is positive there. The same square-root identity gives speed $1+O(t)$; on $0\le t\le\rho$ it therefore lies between $1-C'\rho$ and $1+C'\rho$. Integrating yields radial length $\rho+O(\rho^2)$. Dividing the two positive lengths gives $(2\pi+O(\rho))/(1+O(\rho))\to2\pi$. This proves the stated local absence of a conical defect under the assumed smooth weight-one axis data, without deriving those data from global hyperbolicity. [step 2.1, step 1.2, F1, F2, F5, F6, algebra] ∎

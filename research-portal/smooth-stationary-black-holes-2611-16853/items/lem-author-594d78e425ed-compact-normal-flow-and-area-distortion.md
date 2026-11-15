---
id: lem-author-594d78e425ed-compact-normal-flow-and-area-distortion
title: A compact normal-flow collar has uniformly small area distortion
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-section-time
  - math:thm-fundamental-theorem-on-flows
  - math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves
  - def-lipschitz-cut-area-data
  - math:def-smooth-collar-of-a-manifold-boundary
dependency_roles:
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-section-time: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves: mathematical-premise
  def-lipschitz-cut-area-data: mathematical-premise
  math:def-smooth-collar-of-a-manifold-boundary: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 5
---

## Statement

Let $\Sigma$ be a smooth spacelike section with compact boundary $S$ in a smooth stationary Lorentz geometry, smooth up to $S$. Suppose $T=Nn+X$, with $N>0$ in the interior, $N=0$ at $S$, $T|_S\in TS$, and stationary extensions to translated sections. Suppose $E=\mathbb R_v\times\Sigma^\circ$, $Tv=1$, and these sections are $v$-levels. Write $h_0=g|_{T\Sigma}$. Suppose a smooth collar $c:S\times[0,\eta\prime)\to\Sigma$ is supplied, with $c(p,0)=p$. On its image define the collar coordinate by $\rho(c(p,r))=r$, and assume $\rho(x)=d_{h_0}(x,S)$ there, where $d_{h_0}(x,S)=\inf_{p\in S}d_{h_0}(x,p)$. Thus $\rho$ is smooth and nonnegative and vanishes precisely on $S$. For sufficiently small $0<\eta<\eta\prime$, let $\mathcal R=c(S\times[0,\eta])=\{0\le\rho\le\eta\}$, a compact smooth boundary-distance collar. Then $V=Nn=T-X$ has a smooth local flow $\Psi_z$ on $\mathcal R$ for all sufficiently small $|z|$, fixing $S$. It takes interior points to $v=z$. In stationary coordinates $\Psi_z(x)=(z,\psi_z(x))$, where $\psi_z$ is the spatial flow of $-X$. If $h_z$ is the induced metric on $v=z$, the two-dimensional dilation of $\Psi_{-z}:\Psi_z(\mathcal R)\to\mathcal R$ is bounded by $1+\epsilon(\delta)$ for $|z|\le2\delta$, where $\epsilon(\delta)\to0$ as $\delta\downarrow0$.

## Facts & Assumptions

[F1] The lapse, shift, future normal and stationary section-time conventions are supplied. [[def-spacelike-maximal-hypersurface-data]] [[def-stationary-section-time]]

[F2] A smooth vector field has a local smooth flow with open domain and smooth inverses; compact initial sets have one common small time interval. [[math:thm-fundamental-theorem-on-flows]] [[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]]

[F3] Gram two-Jacobians and the fixed induced metrics are those of the endpoint-area interface. [[def-lipschitz-cut-area-data]]

[F4] A smooth collar is a smooth embedding of $S\times[0,\eta\prime)$ onto an open neighborhood of $S$, restricting to the identity at $r=0$. Its second coordinate is the supplied smooth collar coordinate $\rho$; identification with intrinsic boundary distance is an explicit hypothesis of the Statement. [[math:def-smooth-collar-of-a-manifold-boundary]]

## Proof

**Given:**The hypotheses in the Statement.

**Goal:** Establish the stated conclusions.

1.1 Smoothness of the spacelike section and ambient metric gives smooth $n,N,X$ up to $S$. Since $N|_S=0$, $V|_S=0$. Extend the smooth field locally across the section boundary in ambient charts. Compactness supplies a common local-flow time by [F2], and uniqueness makes its flow fix $S$. In the supplied collar, $X\rho=0$ on $S$ because $X|_S=T|_S\in TS$. Smoothness on a slightly larger collar and compactness give $|X\rho|\le C\rho$. Along the spatial flow of $-X$, this bounds the absolute logarithmic derivative of positive $\rho$ by $C$, so an interior point cannot hit $S$ in finite small time. The identities $Vv=1$ and $V=T-X$ give $\Psi_z(x)=(z,\psi_zx)$ and the stated section level. This also makes the result independent of the chosen extension outside the relevant collar. [given, F1, F2, F4]

2.1 On the compact collar, smooth flow dependence gives $\Psi_z^*h_z\to h_0$ uniformly as positive definite quadratic forms as $z\to0$. Indeed each coefficient and first derivative of the flow varies continuously on a common compact parameter-collar set, and at zero the map is the identity. The same holds for the inverse. Uniform comparison of these quadratic forms bounds the inverse flow norm on every tangent two-plane by $1+\epsilon(\delta)$, with $\epsilon(\delta)\to0$. Taking the square root of the two-dimensional Gram determinant gives the asserted area dilation bound, including planes at $S$. [F2, F3, step 1.1, algebra] ∎

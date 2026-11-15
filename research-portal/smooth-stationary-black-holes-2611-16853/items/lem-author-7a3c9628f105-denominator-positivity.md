---
id: lem-author-7a3c9628f105-denominator-positivity
title: Positive Harrison denominator and its parameter identity
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-embedded-submanifold-and-slice-chart
  - math:def-c-r-and-smooth-maps-between-smooth-manifolds
  - math:def-continuous-map-top
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  math:def-complex-conjugate-real-imaginary-part-and-modulus: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  math:def-c-r-and-smooth-maps-between-smooth-manifolds: mathematical-premise
  math:def-continuous-map-top: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: Section 3.1, equations (3.2), (3.5), (3.7); Section 3.2, equation
        (3.17) and the positivity paragraph after (3.19).
      statement: The cited passages define the denominator, give its real-part bound
        and parameter identity, and obtain a common positive neighborhood of the
        bifurcation sphere.
      hypotheses: The paper uses normalized stationary vacuum Ernst data with real
        norm and twist potentials, f<1 on the exterior and f<=0 on the
        bifurcation sphere. Only the scalar formulas are adapted here.
      reading_limits: Consulted the named HTML passages. The conditional algebra and
        explicit sublevel neighborhood are proved locally below; no vacuum
        equation, global primitive existence, or other conclusion of the paper
        is imported.
dependency_level: 1
---

## Statement

On an open domain $U$ in stationary Lorentzian data, let $\sigma=f+i\psi$ be a smooth complex scalar, where $f=-g(T,T)$ and $\psi:U\to\mathbb R$ is real-valued and smooth. Assume stationarity: both $f$ and $\psi$ are constant along each local integral curve of $T$ contained in $U$. Let $0\le q\le1$ and set $D_q=|1+q-(1-q)\sigma|^2$. If $f<1$ on a region $E\subseteq U$, then $D_q>0$ there for every $q$; in particular this applies when $E$ is an exterior region. If $S\subseteq U$ is a compact embedded surface with $f\le0$ on $S$, there is an open neighborhood $O\subseteq U$ of $S$, independent of $q$, with $D_q>0$ on $O$. Moreover $D_q=(1-q)^2D_0+4q(1-(1-q)f)$, and at a point $p\in U$ with $T(p)=0$, $D_q(p)=(1-q)^2D_0(p)+4q>0$.

## Facts & Assumptions

[F1] The smooth metric, Killing field, local flow and real scalar $f=-g(T,T)$ use [[def-stationary-lorentzian-data]]. The local integral curves in the stationarity assumption are the trajectories of that local flow.

[F2] A scalar value $z=a+ib$ has real coordinates $a,b$ and squared modulus $|z|^2=a^2+b^2$. These scalar operations, including real and imaginary parts, use [[math:def-complex-conjugate-real-imaginary-part-and-modulus]].

[F3] An embedded surface means an embedded two-dimensional smooth submanifold, with the subspace topology inherited from the ambient manifold, as in [[math:def-embedded-submanifold-and-slice-chart]].

[F4] Smooth real scalar functions on $U$ are smooth maps to $\mathbb R$; the smooth-map definition includes continuity on $U$. [[math:def-c-r-and-smooth-maps-between-smooth-manifolds]]

[F5] For a continuous map and an open neighborhood $V$ of its value at a point, there is an open neighborhood of the point mapped into $V$. [[math:def-continuous-map-top]]

## Proof

**Given:** The hypotheses in the Statement and the mathematical interfaces in [F1]–[F5].

**Goal:** Establish both positivity claims and the parameter identity, including positivity at a zero of $T$.

1.1 Write $a_q=\operatorname{Re}(1+q-(1-q)\sigma)=1+q-(1-q)f=2q+(1-q)(1-f)$. At any point with $f<1$, this is positive: at $q=0$ it is $1-f>0$, and at $q>0$ its first summand is positive and its second is nonnegative. Since $\psi$ is real-valued, $D_q=a_q^2+(1-q)^2\psi^2\ge a_q^2>0$. This proves positivity on $E$. [given, F1, F2, algebra]

1.2 Using the squared-modulus formula, subtract $(1-q)^2D_0$ from $D_q$. The $\psi^2$ terms cancel, leaving $(1+q-(1-q)f)^2-(1-q)^2(1-f)^2$. Its factorization is $2q\cdot 2(1-(1-q)f)=4q(1-(1-q)f)$, which proves the stated identity for every $q$. [given, F2, algebra]

2.1 Set $O=\{x\in U:f(x)<1\}$. Continuity of $f$ shows that $O$ is open: for each $x\in O$, apply [F5] to the open real interval $(-\infty,1)$ to obtain an open neighborhood of $x$ in $U$ contained in $O$. Because $U$ is open in the ambient manifold, these neighborhoods are also ambient open. The inequality $f\le0$ on $S$ gives $S\subseteq O$. This $O$ is independent of $q$, and step 1.1 gives $D_q>0$ throughout $O$ for every $q\in[0,1]$. In particular the asserted neighborhood exists for the compact embedded surface with its inherited topology; compactness is not needed by this explicit construction. [given, F3, F4, F5, step 1.1]

3.1 If $T(p)=0$, then $f(p)=0$. Step 1.2 gives $D_q(p)=(1-q)^2D_0(p)+4q$, while [F2] gives $D_0(p)=1+\psi(p)^2$ and $D_q(p)=(1+q)^2+(1-q)^2\psi(p)^2\ge1$. This establishes positivity also at both parameter endpoints and completes all the claims. [given, F1, F2, algebra, step 1.2] ∎

## Source notes

The denominator and parameter formulas are attributed to Radu, Section 3.1 (3.5), (3.7), and Section 3.2 (3.17). The proof here is a local calculation; the explicit neighborhood in step 2.1 replaces the source's compactness argument. No existence of a stationary primitive or Einstein–Maxwell solution is inferred from this calculation.

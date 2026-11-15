---
id: lem-author-78c700cb9e03-bounded-rapidity-reference-graph
title: A smooth spacelike reference section is a bounded rapidity graph
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-spacelike-maximal-hypersurface-data
  - lem-author-78c700cb9e03-invariant-normal-boost-coordinates
  - math:thm-parametrized-implicit-function-theorem-with-higher-regularity
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:thm-newton-leibniz-with-interior-derivative
  - math:thm-continuous-implies-integrable
  - math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle
  - math:lem-uniform-integral-error-bound
  - math:thm-extreme-value-metric
  - math:lem-tube-lemma-for-a-compact-factor
  - math:thm-heine-borel-rn
  - math:cor-mean-value-theorem
  - math:thm-intermediate-value
dependency_roles:
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  lem-author-78c700cb9e03-invariant-normal-boost-coordinates: mathematical-premise
  math:thm-parametrized-implicit-function-theorem-with-higher-regularity: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:thm-newton-leibniz-with-interior-derivative: mathematical-premise
  math:thm-continuous-implies-integrable: mathematical-premise
  math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle: mathematical-premise
  math:lem-uniform-integral-error-bound: mathematical-premise
  math:thm-extreme-value-metric: mathematical-premise
  math:lem-tube-lemma-for-a-compact-factor: mathematical-premise
  math:thm-heine-borel-rn: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
  math:thm-intermediate-value: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

In the invariant boost tube, let $\Sigma$ be a smooth spacelike hypersurface through $S$ whose unit normal to $S$ within $\Sigma$, pointing into its exterior side, has positive $e_1$ component in the invariant orthonormal normal frame $(e_0,e_1)$. This allows a nonzero timelike component of that normal and does not require the circle action to preserve $\Sigma$. After shrinking, its exterior collar has the form $\tau=a(r,y)$ for $0<r<r_0$, $y\in S$, with $a$ smooth down to $r=0$ and uniformly bounded, say $|a|\le A$. Suppose $T=K-\Omega Z$ is future transverse to this collar, meaning its lapse relative to the future unit normal is positive, and $K$ is future timelike there. Then $1+\Omega Z_Sa>0$ on the graph. Consequently for any formal $(r,\tau,y)$, the function $t\mapsto\tau+t-a(r,\psi_{-\Omega t}y)$ is strictly increasing and has exactly one zero; that zero satisfies $|\tau+t|\le A$.

## Statement references

[[def-spacelike-maximal-hypersurface-data]]

[[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]]

[[math:thm-parametrized-implicit-function-theorem-with-higher-regularity]]

[[math:thm-smooth-inverse-function-theorem-on-manifolds]]

## Facts & Assumptions

[F1] A spacelike hypersurface has a future unit normal, and positive lapse means a positive normal component of the field. [[def-spacelike-maximal-hypersurface-data]]

[F2] The boost and circle coordinates are those of the preceding lemma. In particular, $S$ is a nonempty compact two-sphere, $\kappa>0$, $K=\partial_\tau$, $Z=Z_S$, $T=\partial_\tau-\Omega Z_S$, and $\psi$ is the circle action on $S$. [[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]]

[F3] Smooth inverse and parameter-dependent implicit function theorems apply in charts. [[math:thm-smooth-inverse-function-theorem-on-manifolds]] [[math:thm-parametrized-implicit-function-theorem-with-higher-regularity]]

[F4] A continuous function on a closed bounded interval is Riemann integrable. For a continuous function differentiable in the interior, Newton–Leibniz identifies its endpoint difference with the integral of a Riemann-integrable extension of its derivative. [[math:thm-continuous-implies-integrable]] [[math:thm-newton-leibniz-with-interior-derivative]]

[F5] A continuous parameter derivative on a compact rectangle can be passed through its Riemann integral, including as a one-sided derivative at an endpoint. Integrals of two integrable functions on $[0,1]$ differ by at most their uniform error. [[math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle]] [[math:lem-uniform-integral-error-bound]]

[F6] A continuous real function on a nonempty compact metric space attains its extrema. An open neighborhood of a compact factor times a point contains a product neighborhood of that slice. Closed Euclidean intervals are compact. For the metric theorem, fix an identification $\iota:S\to\mathbb S^2$ and use the metric $d(y,z)=|\iota(y)-\iota(z)|$, which induces the topology of $S$. [[math:thm-extreme-value-metric]] [[math:lem-tube-lemma-for-a-compact-factor]] [[math:thm-heine-borel-rn]]

[F7] The mean value theorem applies to a function continuous on a closed interval and differentiable in its interior. A continuous real function on a closed interval takes every value between its endpoint values. [[math:cor-mean-value-theorem]] [[math:thm-intermediate-value]]

## Proof

**Given:** The stated data and complete hypotheses.

**Goal:** Establish the conclusions on the domains and parameter ranges specified.

1.1 Project the normal tube to $(v,y)$. At $S$ its kernel is the timelike line spanned by $e_0$, which is transverse to the spacelike tangent plane of $\Sigma$. Thus [F3] supplies local graphs $u=w(v,y)$ with $w(0,y)=0$; local uniqueness makes them agree on overlaps after shrinking. Write the exterior-pointing unit normal to $S$ within $\Sigma$ as $\nu=\beta e_0+\alpha e_1$. The stated side hypothesis gives $\alpha>0$, while unit length gives $\alpha^2-\beta^2=1$. Thus the exterior side corresponds to increasing $v$, and $\partial_vw(0,y)=\beta/\alpha$ has absolute value less than one; no equality $\nu=e_1$ is used. Compactness of $S$ and the product-neighborhood assertion in [F6] give a common exterior graph collar $0\le v<\varepsilon$. Define $q(v,y)=\int_0^1\partial_vw(tv,y)\,dt$. The integrand is smooth in each chart, and [F4], applied to $t\mapsto w(tv,y)$, gives $w(v,y)=v q(v,y)$, including at $v=0$; hence $q(0,y)=\partial_vw(0,y)$. To check joint smoothness, differentiate successively in the chart variables $(v,y)$ using [F5] on closed coordinate intervals. Every resulting derivative is the integral of the corresponding continuous derivative of the integrand. These integrals are jointly continuous: for any such integrand $H$ and fixed parameter $p_0$, the open set $|H(t,p)-H(t,p_0)|<\eta$ contains $[0,1]\times\{p_0\}$, so [F6] gives a neighborhood of $p_0$ where the inequality holds uniformly in $t$; the integral-error bound in [F5] then gives continuity. This also proves smoothness up to $v=0$ using its one-sided derivatives (or a local smooth extension of the graph there). [F1, F2, F3, F4, F5, F6]

2.1 Apply [F6] on $S$ to obtain $m=\max_y|q(0,y)|<1$, and choose $m<\theta<1$. The open set $|q(v,y)|<\theta$ contains $\{0\}\times S$, so the tube lemma in [F6] gives this bound on a common smaller collar. Put $R(v,y)=v\sqrt{1-q(v,y)^2}$. Then $\partial_vR(0,y)=\sqrt{1-q(0,y)^2}\ge\sqrt{1-m^2}>0$. Continuity and the same tube lemma allow a further shrinking with $\partial_vR>c=\tfrac12\sqrt{1-m^2}$ throughout. Fix $0<\varepsilon_1<\varepsilon$ within that collar. By [F7], $R(\varepsilon_1,y)>c\varepsilon_1$ and $v\mapsto R(v,y)$ is strictly increasing; the intermediate value theorem gives a unique inverse $v=b(r,y)$ for $0\le r<r_0=c\varepsilon_1$. The inverses are smooth by [F3], including at zero, and their uniqueness makes the chartwise inverses agree. Substituting into [F2]'s boost coordinates gives $a(r,y)=\kappa^{-1}\operatorname{arctanh}q(b(r,y),y)$. It is smooth down to zero, and $|a|\le A=\kappa^{-1}\operatorname{arctanh}\theta$, so the entire exterior collar has the asserted bounded-rapidity graph form. [F2, F3, F6, F7, step 1.1]

3.1 On the spacelike graph, the defining function $f=\tau-a(r,y)$ has $df(K)=1$ and timelike normal covector $df$. If $n$ is its future unit normal, write $df=\lambda g(n,\cdot)$ there. Since $K$ is future timelike, $g(n,K)<0$, so $\lambda<0$. The positive lapse $N=-g(T,n)>0$ from [F1] therefore gives $df(T)=-\lambda N=1+\Omega Z_Sa>0$. For any fixed formal $(r,\tau,y)$ with $0<r<r_0$, set $h(t)=\tau+t-a(r,\psi_{-\Omega t}y)$. The circle action in [F2] is defined for all real $t$, and $h'(t)=1+\Omega Z_Sa(r,\psi_{-\Omega t}y)>0$, using the graph inequality at that base point. Thus [F7] applied on every finite interval proves strict increase. Step 2.1 gives $|h(t)-(\tau+t)|\le A$, so $h(-\tau-A-1)\le-1$ and $h(-\tau+A+1)\ge1$. The intermediate value theorem in [F7] gives a zero between these endpoints, strict increase gives uniqueness, and at the zero $\tau+t=a(r,\psi_{-\Omega t}y)$ gives $|\tau+t|\le A$. [F1, F2, F7, step 2.1] ∎

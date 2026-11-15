---
id: def-author-f247c641a714-regular-static-exterior-data
title: Complete regular static exterior data and its normalized end
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-stationary-asymptotic-decay-data
  - def-spacelike-maximal-hypersurface-data
  - math:def-laplace-beltrami-operator-as-trace-of-the-hessian
  - math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary
  - math:def-riemannian-distance-on-a-connected-manifold
  - physics:def-gr-causal-curves-and-reachability
  - physics:def-gr-causal-conditions-and-global-hyperbolicity
  - physics:lem-gr-temporal-functions-and-time-functions
  - math:thm-choice-implies-dependent-implies-countable-choice
  - math:def-axiom-of-choice
dependency_roles:
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  physics:def-gr-causal-conditions-and-global-hyperbolicity: mathematical-premise
  physics:lem-gr-temporal-functions-and-time-functions: mathematical-premise
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:def-laplace-beltrami-operator-as-trace-of-the-hessian: mathematical-premise
  math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary: mathematical-premise
  math:def-riemannian-distance-on-a-connected-manifold: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Definition

Regular static exterior data consist of a connected oriented three-manifold $\overline X$ with nonempty compact smooth boundary $B$, a positive-definite metric $h$ and real function $V$ which are smooth on $X=\overline X\setminus B$ and at least $C^2$ on $\overline X$. Require $V>0$ on $X$, $V=0$ and $dV\ne0$ on $B$. Completeness up to boundary means completeness of the intrinsic $h$-distance on $\overline X$, with boundary included. A single asymptotically Euclidean end means that the complement of a compact subset of $\overline X$ is diffeomorphic to $\{x\in\mathbb R^3:r=|x|>R_0\}$, with no additional ends or deleted interior boundary. In that chart require $h_{ij}-\delta_{ij}=O_2(r^{-1})$ and $V=1-m/r+O_2(r^{-2})$ for a real number $m$ not initially assumed positive.

The associated globally static spacetime exterior is $\mathbb R_t\times X$ with $g=-V^2dt^2+h$, future orientation $\partial_t$ and stationary field $T=\partial_t$. The boundary $B$ is a boundary of the spatial data; this product formula does not define a nondegenerate Lorentzian metric at $V=0$. Write $D$ for the Levi–Civita connection of $h$, $D^2V(A,C)=A(CV)-(D_AC)V$ for its Hessian and $\Delta_hV=\operatorname{tr}_hD^2V$ for its Laplacian.

## Definition references

[[def-stationary-lorentzian-data]]

[[def-stationary-asymptotic-decay-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]]

[[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary]]

[[math:def-riemannian-distance-on-a-connected-manifold]]

## Facts & Assumptions

[F1] Stationary Lorentzian data supply the standing ZFC convention, including the axiom of choice, together with the metric, time-orientation, Killing-field and connection conventions for the smooth interior product. [[def-stationary-lorentzian-data]]

[F2] The differentiated end notation $O_2$ means uniform Cartesian derivative bounds through order two for each fixed datum. [[def-stationary-asymptotic-decay-data]]

[F3] On the smooth interior the Laplace–Beltrami operator is the metric trace of the Levi–Civita Hessian, with sign $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. [[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]]

[F4] Smooth manifold-with-boundary charts take values in relatively open subsets of a half-space; smooth transitions are understood by local extension. [[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary]]

[F5] Intrinsic distance uses the infimum of lengths of piecewise $C^1$ connecting curves. The same length formula is specified below for the present $C^2$ boundary metric; its metric property is proved locally rather than imported from a smooth-metric theorem. [[math:def-riemannian-distance-on-a-connected-manifold]]

[F6] Completeness up to boundary means Cauchy completeness of the intrinsic distance with boundary points included. This agrees with the terminology for embedded smooth spacelike sections, but the abstract $C^2$ boundary case here is justified below. [[def-spacelike-maximal-hypersurface-data]]

[F7] Future causal curves are locally absolutely continuous and have nonzero future causal velocity almost everywhere; consequently they are nonconstant on every nondegenerate parameter subinterval. [[physics:def-gr-causal-curves-and-reachability]]

[F8] A smooth function $u$ is temporal when its gradient satisfies $g(\nabla u,\nabla u)<0$ and $du(N)>0$ for the chosen future timelike orientation field $N$. [[physics:def-gr-causal-conditions-and-global-hyperbolicity]]

[F9] Assuming Countable Choice and Dependent Choice, a temporal function composed with any future causal curve in [F7] is locally absolutely continuous, has positive derivative almost everywhere and is strictly increasing between parameter values on every nonconstant subinterval. [[physics:lem-gr-temporal-functions-and-time-functions]]

[F10] The axiom of choice implies Dependent Choice and Countable Choice, so the standing ZFC convention in [F1] supplies both choice hypotheses of [F9]. [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]]

## Justification

**Given:** The data in the Definition and the interfaces in [F1]–[F10].

**Goal:** Justify the object and completeness conventions without asserting an extension across a horizon.

1.1 Use the smooth boundary charts of [F4] and their interior counterparts. For a piecewise $C^1$ curve $\gamma:[a,b]\to\overline X$, set $L_h(\gamma)=\int_a^b\sqrt{h_{\gamma(s)}(\dot\gamma(s),\dot\gamma(s))}\,ds$, summed over its finitely many $C^1$ pieces, and define $d_h(p,q)$ as the infimum of these lengths for curves joining $p$ to $q$, as in [F5]. Small coordinate balls or half-balls are convex, so any two points in one such chart neighborhood can be joined by a smooth coordinate segment. For fixed $p$, the set reachable from $p$ by finitely many such segments is open; its complement is open by the same local segment property. Connectedness therefore makes every point reachable. Each finite piece has finite length by continuity of $h$ on its compact trace. Thus each infimum is finite and nonnegative, using only continuity of $h$ up to $B$. [given, F4, F5]

1.2 The compact-core/end-chart requirement is a global topological condition, not a consequence of pointwise estimates. The differentiated $O_2$ notation fixes all Cartesian derivatives up to second order and is uniform in angular directions for each fixed datum. On the smooth interior the trace-of-Hessian definition fixes the sign of $\Delta_h$ and agrees with $\operatorname{div}_h\operatorname{grad}_h$. [given, F2, F3]

2.1 Constant curves give $d_h(p,p)=0$, and reversal preserves length, so $d_h$ is symmetric. Length is additive under concatenation by splitting the defining integrals. Given $\varepsilon>0$, curves from $p$ to $q$ and from $q$ to $r$ with lengths less than the respective infima plus $\varepsilon$ yield $d_h(p,r)\le d_h(p,q)+d_h(q,r)+2\varepsilon$. Letting $\varepsilon$ decrease to zero gives the triangle inequality. [given, step 1.1]

2.2 On $X$ positivity of $V$ gives a smooth nondegenerate product tensor of signature $(-,+,+,+)$; $g(T,T)=-V^2<0$ and its coefficients are independent of $t$. Thus $T$ is Killing, complete on this product, and hypersurface orthogonal since its metric dual is $-V^2dt$. The construction asserts neither regular Lorentzian coordinates at $B$ nor a maximal analytic extension. [given, F1, step 1.2]

3.1 For distinct $p,q$, take a coordinate ball or boundary half-ball centered at $p$, of radius $\rho>0$, whose compact closure lies in the chart and excludes $q$. Continuity and positive definiteness give a positive minimum $c$ of $h_x(v,v)$ over this compact coordinate closure and the Euclidean unit sphere, hence $h_x(v,v)\ge c|v|^2$. Every connecting curve from $p$ to $q$ first exits this relative ball through its spherical boundary; at a boundary chart the flat face lies in the manifold and is not an exit. The coordinate displacement of the initial curve is $\rho$, so integration of its derivative gives $L_h(\gamma)\ge\sqrt c\int|\dot\gamma|\,ds\ge\sqrt c\,\rho$. Taking the infimum proves $d_h(p,q)>0$. Consequently $d_h$ is a metric also at boundary points for the stated $C^2$ data, and completeness means that every $d_h$-Cauchy sequence converges in $\overline X$, with $B$ included, consistently with [F6]. Completeness itself remains a requirement on the data. [given, F4, F6, step 1.1, step 2.1]

4.1 On the smooth interior product take $N=T$. Direct contraction with $g=-V^2dt^2+h$ gives $\nabla t=-V^{-2}T$, hence $g(\nabla t,\nabla t)=-V^{-2}<0$ and $dt(N)=1>0$. Thus $t$ is temporal by [F8]. The standing ZFC convention in [F1] supplies the choice hypotheses of [F9] by [F10]. For every future causal curve $\gamma:I\to\mathbb R_t\times X$ in [F7], the function $t\circ\gamma$ is therefore locally absolutely continuous and has positive derivative almost everywhere by [F9]. Such a curve is nonconstant on every nondegenerate subinterval by [F7], so [F9] gives $t(\gamma(a))<t(\gamma(b))$ whenever $a<b$ in $I$. This proves the claimed strict increase along the declared causal-curve class. [given, F1, F7, F8, F9, F10, step 2.2, algebra] ∎

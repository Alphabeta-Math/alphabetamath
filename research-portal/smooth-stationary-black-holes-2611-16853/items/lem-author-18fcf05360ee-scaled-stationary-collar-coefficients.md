---
id: lem-author-18fcf05360ee-scaled-stationary-collar-coefficients
title: Stationary coefficients in a transverse collar retain the tangential motion
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-spacelike-maximal-hypersurface-data
  - def-normal-graph-and-mean-curvature-data
  - def-bifurcate-killing-horizon-data
  - math:thm-fundamental-theorem-on-flows
  - math:thm-parametrized-implicit-function-theorem-with-higher-regularity
  - def-causal-exterior-and-boundary-data
  - math:def-riemannian-speed-and-length
  - math:def-interior-closure-boundary-top
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  math:thm-parametrized-implicit-function-theorem-with-higher-regularity: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:def-riemannian-speed-and-length: mathematical-premise
  math:def-interior-closure-boundary-top: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Let $\Sigma_*$ be smooth spacelike with compact boundary $S$, and let $Y$ equal its future unit normal near $S$. Its smooth flow coordinates are $(s,\rho,y)$, with $\Sigma_*:\,s=0$, $\rho\ge0$ the induced boundary distance on the section extended constantly along $Y$, and $y\in S$. Let smooth $T$ be tangent to $S$ and have reference lapse $N_*\ge c\rho$ for some $c>0$ in a fixed collar. Write $T=a\partial_s+b\partial_\rho+W$, where $W$ is tangent to $S$ in these coordinates. Fix any smooth Riemannian metric on $S$, for example the metric induced by $\Sigma_*$, and use it for the norm of $W$. There are constants $C,B,M,\eta>0$ such that, in $|s|\le\eta\rho$, $0<\rho<\rho_0$, one has $a\ge(c/2)\rho$, $|b|\le B\rho$ and $|W|\le M$. No vanishing or constancy of the tangential term $W$ is asserted.

For the exterior assertion, let $D$ be the ambient spacetime, $U\subset D$ a specified open set, and $\mathcal E=I_D^-(U)\cap I_D^+(U)$ its causal exterior. Suppose that, in a common neighborhood of $S$, the full event boundaries $\partial_D I_D^-(U)$ and $\partial_D I_D^+(U)$ are smooth embedded null hypersurfaces meeting transversely exactly at $S$. Suppose also that the punctured reference collar $\{s=0,\ 0<\rho<\rho_0\}$ lies in $\mathcal E$. Then the same wedge may be chosen inside $\mathcal E$. No exterior-side condition is required for the coefficient estimates alone.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-normal-graph-and-mean-curvature-data]]

[[def-bifurcate-killing-horizon-data]]

[[math:thm-fundamental-theorem-on-flows]]

[[math:thm-parametrized-implicit-function-theorem-with-higher-regularity]]

[[def-causal-exterior-and-boundary-data]]

[[math:def-riemannian-speed-and-length]]

[[math:def-interior-closure-boundary-top]]

## Facts & Assumptions

[F1] Smooth local flow coordinates and implicit graphs are available, and the graph convention uses the parameter of $Y$. [[math:thm-fundamental-theorem-on-flows]] [[math:thm-parametrized-implicit-function-theorem-with-higher-regularity]] [[def-normal-graph-and-mean-curvature-data]]

[F2] The lapse is $-g(T,n_*)$ and the time and null-horizon conventions are fixed. [[def-spacelike-maximal-hypersurface-data]] [[def-bifurcate-killing-horizon-data]] [[def-stationary-lorentzian-data]]

[F3] The section has its smooth positive induced metric up to $S$, and its boundary distance is the infimum of lengths of piecewise $C^1$ curves from $S$ within the section. Length is the integral of metric speed. Smoothness of $\rho$ as a boundary coordinate is part of the supplied collar, not an additional existence conclusion. [[def-spacelike-maximal-hypersurface-data]] [[math:def-riemannian-speed-and-length]]

[F4] The causal exterior and full event boundaries use the specified ambient domain $D$ and open set $U$. The reference-collar inclusion and the smooth transverse boundary germs in the Statement are additional hypotheses for the exterior conclusion. For any subset $A\subset D$, the complement of $\partial_D A$ is the disjoint union of $\operatorname{int}_D A$ and $\operatorname{int}_D(D\setminus A)$. [[def-causal-exterior-and-boundary-data]] [[math:def-interior-closure-boundary-top]]

## Proof

**Given:** The stated data, and the additional exterior hypotheses only for that conclusion.

**Goal:** Establish the coefficient bounds and, under the exterior hypotheses, the uniform exterior wedge.

1.1 On $s=0$, $\partial_s=Y=n_*$, so the coefficient $a(0,\rho,y)$ is exactly $N_*$. Tangency of $T$ to $S$ gives $a(0,0,y)=b(0,0,y)=0$. Smoothness and compactness therefore give $|a(s,\rho,y)-a(0,\rho,y)|\le C|s|$ and $|b(s,\rho,y)|\le C(\rho+|s|)$ on a common coordinate collar; the tangential coefficient has a uniform norm bound $M$ in the chosen smooth Riemannian metric on $S$. Choose $\eta$ with $C\eta\le c/2$. The two asserted coefficient inequalities follow, with $B=C(1+\eta)$. These estimates are uniform over the whole compact $S$, allowing chart changes as $y$ moves. [given, F1, F2, F3]

1.2 Let $\nu$ be the inward unit normal to $S$ within the section. We first prove $d\rho_p(\nu_p)=1$ for every $p\in S$, without assuming a normal-geodesic extension of $y$. Choose a boundary half-chart $(r,z)$ centered at $p$, with $r\ge0$, $S:\,r=0$, $\partial_r|_p=\nu_p$ and induced metric $h_p=dr^2+|dz|^2$. For each $0<\delta<1$, continuity gives a smaller half-ball where $(1-\delta)^2(dr^2+|dz|^2)\le h\le(1+\delta)^2(dr^2+|dz|^2)$. The radial segment to $(r,0)$ has length at most $(1+\delta)r$. Every path from $(r,0)$ to $S$ that stays in the half-ball has length at least $(1-\delta)r$, since its total $r$-variation is at least $r$. A path leaving the half-ball first has a fixed positive lower length bound for all sufficiently small $r$, from the same metric comparison applied up to its first exit, so it cannot violate that lower bound. Taking the infimum over all paths gives $(1-\delta)r\le\rho(r,0)\le(1+\delta)r$. Taking $r\downarrow0$ and then $\delta\downarrow0$ proves the derivative claim. Since $\rho|_S=0$ and $\partial_\rho\rho=1$, it follows that $\partial_\rho|_S=\nu+V$ for some $V\in TS$; $V$ need not vanish. [given, F3]

2.1 Assume now the exterior hypotheses. Shrink the flow collar so that $Y$ is timelike. A null tangent hyperplane contains no timelike vector, so $Y$ is transverse to each null boundary. The implicit function theorem gives their smooth graphs $s=h_\pm(\rho,y)$, with $h_\pm(0,y)=0$; local graphs agree on overlaps by uniqueness, and compactness gives a common smaller collar. At $S$, their null radical lines are orthogonal to $TS$, hence are the two lines spanned by $n_*+\nu$ and $n_*-\nu$ in the normal plane of $S$. Their tangent hyperplanes are the orthogonal complements of those lines. The graph's radial tangent vector there is $(\partial_\rho h_\pm)n_*+\nu+V$. Pairing it with $n_*\pm\nu$ gives $-\partial_\rho h_\pm\pm1=0$, independently of $V$. After labeling by slope on each component of $S$, this proves $\partial_\rho h_\pm(0,y)=\pm1$. [F1, F2, F4, step 1.2]

3.1 Smoothness and compactness in step 2.1 give $h_-(\rho,y)\le-3\rho/4$ and $h_+(\rho,y)\ge3\rho/4$ for all sufficiently small positive $\rho$. Shrink $\eta$ from step 1.1 to at most $1/2$ and shrink $\rho_0$ so that the whole wedge is in the common neighborhood where these graphs are the full event boundaries. For each wedge point, the vertical segment from $(0,\rho,y)$ to $(s,\rho,y)$ stays strictly between the graphs and avoids both boundaries. For either $A=I_D^-(U)$ or $A=I_D^+(U)$, a connected segment avoiding $\partial_D A$ has constant membership in $A$, because the two complementary regions in [F4] are disjoint open sets. Its initial point belongs to both sets by the reference-collar hypothesis, so its endpoint belongs to $\mathcal E$. All coefficient estimates survive the shrinking. This proves the asserted uniform exterior wedge without identifying its side from transversality alone. [F4, step 1.1, step 2.1] ∎

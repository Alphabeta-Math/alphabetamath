---
title: Uniform stationary return persists under arbitrary tangential drift
status: draft
research_item: lem-author-18fcf05360ee-uniform-stationary-return-with-tangential-motion
dependency_level: 3
---

## Prerequisites

- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)
- [math:thm-parametrized-implicit-function-theorem-with-higher-regularity](https://alphabetamath.cc/item/thm-parametrized-implicit-function-theorem-with-higher-regularity)
- [lem-author-18fcf05360ee-scaled-stationary-collar-coefficients](item-lem-author-18fcf05360ee-scaled-stationary-collar-coefficients)
- [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)
- [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)


## Statement

In the coefficient collar of the stationary-coefficient lemma, write $T=a\partial_s+b\partial_\rho+W$ on $|s|\le\eta\rho$, $0<\rho<r$, with $a\ge(c/2)\rho$, $|b|\le B\rho$ and $|W|\le M$, uniformly over the compact sphere $S$. Let a point have coordinates $(s_0,\rho_0,y_0)$ with $|s_0|\le\epsilon\rho_0$ and $0<\rho_0$ in a fixed smaller collar. For all sufficiently small $\epsilon>0$, its stationary orbit meets $s=0$ within a time $t_*$ satisfying $|t_*|\le4\epsilon/c$. At the meeting, $e^{-B|t_*|}\rho_0\le\rho(t_*)\le e^{B|t_*|}\rho_0$. The trajectory to that meeting remains in the coordinate wedge. The return point and time are smooth on the punctured collar. All constants depend on the fixed reference collar and coefficients, and are uniform for graphs with the same smallness bound. The base point $y$ is allowed to move throughout $S$.

For the exterior conclusion, use an ambient spacetime $D$, a specified open $U\subset D$ and $\mathcal E=I_D^-(U)\cap I_D^+(U)$. Assume, as in the coefficient supplier's exterior clause, that in a common neighborhood of $S$ the full boundaries $\partial_D I_D^-(U)$ and $\partial_D I_D^+(U)$ are smooth embedded null hypersurfaces meeting transversely exactly at $S$, and that the punctured reference collar $\{s=0,\ 0<\rho<r\}$ lies in $\mathcal E$. Then the wedge may be shrunk inside $\mathcal E$, and the entire return trajectory remains in the exterior collar. These additional hypotheses are needed only for this exterior conclusion.

## Statement references

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)

[math:thm-parametrized-implicit-function-theorem-with-higher-regularity](https://alphabetamath.cc/item/thm-parametrized-implicit-function-theorem-with-higher-regularity)

[lem-author-18fcf05360ee-scaled-stationary-collar-coefficients](item-lem-author-18fcf05360ee-scaled-stationary-collar-coefficients)

[math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)

[math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

## Facts & Assumptions

[F1] The smooth coefficient collar, including its compact sphere, has $a\ge(c/2)\rho$, $|b|\le B\rho$ and $|W|\le M$ on $|s|\le\eta\rho$, $0<\rho<r$. Under the additional exterior hypotheses in the Statement, the same supplier permits a smaller such wedge contained in $\mathcal E$. [lem-author-18fcf05360ee-scaled-stationary-collar-coefficients](item-lem-author-18fcf05360ee-scaled-stationary-collar-coefficients)

[F2] The stationary trajectories are integral curves of $T$. Their local flow is smooth and unique, with a common short-time domain near a fixed compact collar. The implicit function theorem applies to a smooth scalar hitting equation whose time derivative is nonzero. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows) [math:thm-parametrized-implicit-function-theorem-with-higher-regularity](https://alphabetamath.cc/item/thm-parametrized-implicit-function-theorem-with-higher-regularity)

[F3] For a $C^1$ real trajectory on a time interval, the integral of its derivative equals its endpoint difference, with either orientation of the endpoints. This applies to its $s$ coordinate and, while $\rho>0$, its $\log\rho$ coordinate. [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)

[F4] Tangential path length is the integral of speed in the fixed sphere metric. The causal exterior and full event boundaries are taken relative to the specified $D$ and $U$, with the conventions in the Statement. [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

## Proof

**Given:** The smooth coefficient collar and starting point in the Statement, with the additional exterior hypotheses only for the exterior conclusion.

**Goal:** Establish uniform return, radial comparison, smoothness and, conditionally, exterior confinement.

1.1 If $s_0=0$, take $t_*=0$. Otherwise set $\sigma=-\operatorname{sgn}(s_0)$ and follow $p(u)=\Phi^T_{\sigma u}(s_0,\rho_0,y_0)$ for $u\ge0$ until the first meeting with $s=0$. Set $T_\epsilon=4\epsilon/c$. Choose $\epsilon$ so that $BT_\epsilon<\log2$, $2\epsilon<\eta$, and $T_\epsilon$ is strictly within a common local-flow interval for the compact reference collar. Such an interval follows by taking a finite subcover of the open flow domain around that collar. While the trajectory remains in the wedge before meeting, $|d\rho/du|\le B\rho$ and [F3] applied to $\log\rho$ give $e^{-Bu}\rho_0\le\rho(u)\le e^{Bu}\rho_0$. Since $ds/du=\sigma a$, the sign of $s$ before meeting gives $d|s|/du=-a<0$. Thus $|s|/\rho\le2\epsilon<\eta$. Taking the fixed starting collar with $\rho_0<r/4$ gives $0<\rho(u)<r/2$ for $u\le T_\epsilon$. The strict wedge and radial bounds, and the common flow interval, exclude exit before either meeting or time $T_\epsilon$. This also excludes reaching $\rho=0$ in that time. [given, F1, F2, F3]

2.1 If there were no meeting for $0\le u\le T_\epsilon$, step 1.1 would give $a\ge(c/2)\rho\ge c\rho_0/4$ throughout. Integrating $d|s|/du=-a$ by [F3] would yield $|s(T_\epsilon)|\le |s_0|-(c\rho_0/4)T_\epsilon\le0$, contradicting absence of a meeting. Therefore the first meeting has $t_*=\sigma u_*$ with $0\le u_*\le T_\epsilon$, and the radial comparison follows from step 1.1. Since the inequalities have strict margins for sufficiently small $\epsilon$, this return construction applies in an open neighborhood of each point under consideration with $\rho>0$. [F1, F3, step 1.1]

3.1 In local initial-point coordinates, put $H(t,p)=s(\Phi_t^T(p))$. At the meeting, $\partial_tH=a(\Phi_{t_*}^T(p))\ge(c/2)\rho(t_*)>0$. Smooth flow dependence and the implicit function theorem therefore give a smooth local root $t=t_*(p)$, and composition gives the smooth return point. These local roots agree with the constructed return: $a>0$ makes the $s$ coordinate strictly increasing along the connected trajectory segment inside the wedge, so that segment has at most one zero. The same argument applies at initial points with $s_0=0$, so there is no smoothness exception there. Along the entire segment, the moving sphere coordinate has speed at most $M$ and hence path length at most $M|t_*|\le M T_\epsilon$ in the fixed sphere metric. No tangential constancy is used; all normal bounds hold at the moving base point. The bounds and choices of collar and time depend only on the fixed reference coefficients, so they are uniform for graphs satisfying the same pointwise smallness bound. [F1, F2, F4, step 1.1, step 2.1]

4.1 Under the additional exterior hypotheses, choose the smaller coefficient wedge furnished by [F1] inside $\mathcal E$ before making the choices above. Steps 1.1 and 2.1 keep the entire return segment in that wedge, so it stays in the exterior collar. The return and radial estimates and step 3.1 require only the coefficient collar and remain valid without the additional exterior hypotheses. [F1, F4, step 1.1, step 2.1, step 3.1] ∎

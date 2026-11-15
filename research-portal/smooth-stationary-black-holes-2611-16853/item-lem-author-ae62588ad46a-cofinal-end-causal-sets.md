---
title: Cofinal stationary end representatives have the same causal exterior
status: published
research_item: lem-author-ae62588ad46a-cofinal-end-causal-sets
dependency_level: 3
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section)
- [def-author-310ff0f53b38-closure-and-boundary-data](item-def-author-310ff0f53b38-closure-and-boundary-data)



## Statement

Let $U=M_{\rm ext}=\mathbb R_t\times E\subset M$ be a stationary flow product, with $T=\partial_t$ future timelike and complete on $U$. Use the stationary-end convention: $U$ is the complete orbit saturation of a spacelike representative $S_{\rm ext}$ with a specified exterior chart $\{x\in\mathbb R^3:|x|>R_0\}\to S_{\rm ext}$. For any nonempty open $E_1\subset E$ and smooth $b:E_1\to\mathbb R$, let $S_1=\{(b(x),x):x\in E_1\}$ be a spacelike graph, and let $U_1=\mathbb R\times E_1$ be its complete orbit saturation. In particular this includes cofinal far-out representatives and increased radial cutoffs; cofinal means that the spatial domain contains every sufficiently large radius in the chosen end chart. Then $I_M^+(U_1)=I_M^+(U)$ and $I_M^-(U_1)=I_M^-(U)$.

Consequently the domain of outer communications $D=I_M^+(U)\cap I_M^-(U)$, the full event boundaries $H^+=\partial_M I_M^-(U)$ and $H^-=\partial_M I_M^+(U)$, their connected components, and the portions $\mathcal E^\pm=\partial_M D\cap I_M^\pm(U)$ are unchanged. Global hyperbolicity of $(D,g|_D)$ and any already satisfied future or past affine completeness of their null generators are preserved. A generator means a null geodesic maximally continued in the specified horizon set, with the portion convention when appropriate; affine completeness in a direction means that its maximal affine parameter interval is unbounded in that direction.

If a section $\Sigma$ with completion $\overline\Sigma^{\,M}$ and manifold boundary $B=\overline\Sigma^{\,M}\setminus\Sigma$ is already supplied, keep these subsets fixed. Its completion and any once-only cross-section condition $|B\cap G|=1$ for each generator image $G$ of the specified horizon set are then unchanged. Whether a section containing a different end representative exists, or has the required completion, requires a separate applicable section-deformation result with its own hypotheses; equality of chronological sets does not supply it.

A stationary coordinate change $t'=a t+f(x)$, with constant $a>0$ and smooth $f$, keeps the same orbit saturations and changes the stationary field normalization to $\partial_{t'}=a^{-1}T$. A level of $t'$ may be used as a spacelike representative only when it is spacelike. This coordinate change preserves the foregoing geometric conclusions and affine completeness.

## Facts & Assumptions

[F1] The smooth Lorentzian metric, time orientation and Killing field use [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). The product flow is $(t,x)\mapsto(t+s,x)$ for all real $s$. Stationarity makes its metric coefficients independent of $t$; future direction is the cone component containing $T$.

[F2] The stationary-end interface in [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) supplies a spacelike exterior-chart representative and its saturation. In this lemma the saturation is the whole complete product $U$. The same interface defines chronological reachability, the DOC, event boundaries and global hyperbolicity. No metric decay or field equation is used.

[F3] Use the null-geodesic, maximal-generator, generator-image and once-only cross-section terminology of [def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section). Only that interface's general terminology is used, not its separate imported stationary causal-boundary ray assertion or an assertion of generator existence or completeness.

[F4] A supplied completion $\overline\Sigma^{\,M}$ and its intrinsic manifold boundary $B$ have the meanings in [def-author-310ff0f53b38-closure-and-boundary-data](item-def-author-310ff0f53b38-closure-and-boundary-data). These data are fixed during the comparison; no deformation of $\Sigma$ is asserted.

## Proof

**Given:** The complete stationary product and exterior-chart saturation in the Statement, a nonempty spatial domain $E_1$, and any horizon generators or completed section being compared.

**Goal:** Prove the equality of both chronological sets and identify precisely which geometric data it preserves.

1.1 The chart exterior $\{|x|>R_0\}$ is connected (radial paths and paths on a larger sphere join its points), so $S_{\rm ext}$ is connected. Let $\pi_E:U\to E$ be product projection. Every orbit in $U$ meets $S_{\rm ext}$ by the saturation hypothesis, and $\pi_E$ is constant on each orbit. Hence $\pi_E(S_{\rm ext})=E$, so $E$ is connected. In a smooth manifold the points reachable from a fixed point by a finite piecewise $C^1$ path form an open set with open complement: inside a coordinate ball straight coordinate segments extend such paths. Connectedness therefore gives such a path between any two points of $E$. In particular, every $x\in E$ has a finite piecewise $C^1$ path $c:[0,1]\to E$ to some $y\in E_1$. This derives the spatial path property from the declared stationary-end data rather than from connectedness only at large radius. [given, F1, F2]

2.1 Fix $p=(t_0,x)\in U$ and a path $c$ from step 1.1. Along $(0,c(s))$, put $V=(0,\dot c(s))$ on each of its finitely many $C^1$ pieces. Compactness and timelikeness give constants $\delta>0$ and $B_0,C_0<\infty$ with $g(T,T)\le-\delta$, $|g(T,V)|\le B_0$ and $|g(V,V)|\le C_0$. Stationarity gives the same bounds after any time translation. For sufficiently large constant $\lambda>0$, both vectors $\lambda T+V$ and $-\lambda T+V$ have squared norm at most $-\delta\lambda^2+2B_0\lambda+C_0<0$; their inner products with $T$ are respectively negative and positive. In a Lorentz frame with future timelike $T$ as time axis these signs select the future and past cones. Thus $(t_0+\lambda s,c(s))$ is future timelike and $(t_0-\lambda s,c(s))$ is past timelike, piecewise, with endpoints $q_+,q_-\in U_1$. They lie entirely in $U$, since its time factor is all of $\mathbb R$. Reversing the latter gives $q_-\ll_M p\ll_M q_+$. Piecewise timelike curves belong to the supplied locally absolutely continuous curve class; the finite corner set does not affect their almost-everywhere tangent condition. [given, F1, F2, step 1.1]

3.1 Since $U_1\subset U$, one has $I_M^\pm(U_1)\subset I_M^\pm(U)$. If $z\in I_M^+(U)$, choose $p\in U$ with $p\ll_M z$ and prepend the curve $q_-\ll_M p$ of step 2.1. Concatenating the two finite timelike curves gives $q_-\ll_M z$, hence $z\in I_M^+(U_1)$. If $z\in I_M^-(U)$, choose $p\in U$ with $z\ll_M p$ and append $p\ll_M q_+$; this gives $z\in I_M^-(U_1)$. Concatenation is again in the same curve class and directly verifies transitivity here. Thus both chronological sets agree. Each graph $S_1$ meets every orbit over $E_1$ once, so its full saturation is exactly $U_1$, independently of $b$. [given, F1, F2, step 2.1]

4.1 Equality in step 3.1 preserves intersections and boundaries in the fixed topology of $M$, and therefore preserves $D$, $H^\pm$, $\mathcal E^\pm$ and their connected components as subsets. The ambient metric and time orientation have not changed. Every inextendibility, causal-diamond and strong-causality condition on the fixed domain $D$ is consequently the same condition, so global hyperbolicity is preserved. On each fixed horizon set the affine null-geodesic equation, maximal continuation within that set, and any connected portion restriction are unchanged. The same parametrized generators therefore have the same maximal affine intervals; unboundedness of either end, and hence the stated completeness, is identical. This argument assumes neither smoothness of the horizon nor existence or completeness of generators where those were not already supplied. [F1, F2, F3, step 3.1]

5.1 For fixed $\Sigma$ its ambient closure and the supplied manifold boundary $B$ are unchanged. Since the horizon set and its generator images are unchanged by step 4.1, the predicates $B\subset H$ and $|B\cap G|=1$ are identical before and after the replacement. This proves invariance of the specified completed section and its cross-section condition. It proves no inclusion $S_1\subset\Sigma$, nor existence of a deformed section containing $S_1$ with prescribed completion; those require a separate applicable input. [given, F3, F4, step 4.1]

6.1 At fixed $x$, the map $t\mapsto at+f(x)$ is a bijection of $\mathbb R$ and $\partial_{t'}=a^{-1}T$. Thus its level graphs have the same orbit saturation over their spatial domain, and every cofinal or cutoff replacement already falls under step 3.1. Positivity of $a$ preserves future direction. Rewriting coordinates changes neither the metric as a tensor nor the affine geodesic equation and its geometric solutions. Even a positive constant rescaling of an affine parameter preserves unboundedness of its ends. Consequently the coordinate change has all the claimed invariances, with spacelikeness of any chosen level imposed separately as stated. [given, F1, F2, F3, step 3.1, step 4.1, step 5.1] ∎

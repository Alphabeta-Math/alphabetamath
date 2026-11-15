---
title: Smooth positive inversion and composition in the weighted multiplier class
status: published
research_item: lem-author-45355d85383b-weighted-smooth-inversion
dependency_level: 3
---

## Prerequisites

- [lem-author-45355d85383b-weighted-products-and-derivatives](item-lem-author-45355d85383b-weighted-products-and-derivatives)
- [def-weighted-holder-spaces](item-def-weighted-holder-spaces)
- [math:thm-continuous-partial-derivatives-imply-total-differentiability](https://alphabetamath.cc/item/thm-continuous-partial-derivatives-imply-total-differentiability)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)
- [math:thm-symmetry-of-higher-mixed-partials](https://alphabetamath.cc/item/thm-symmetry-of-higher-mixed-partials)
- [math:lem-taylor-integral-remainder](https://alphabetamath.cc/item/lem-taylor-integral-remainder)
- [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)
- [math:thm-heine-cantor-metric](https://alphabetamath.cc/item/thm-heine-cantor-metric)


## Statement

Fix the exterior and chart data of the weighted Hölder norms, an integer $k\ge0$ and $0<\alpha<1$. Write $\mathcal A_\beta=C^{k,\alpha}_\beta(\Sigma_1)$, with finite arrays given the sum of component norms. All domains below use the full finite-norm Hölder spaces, including nonsmooth elements.

We use the following normed-space meaning of $C^1$. For an open subset $U$ of a real normed vector space $X$, a map $F:U\to Y$ is continuously Fréchet differentiable when, at every $u\in U$, there is a linear map $DF(u):X\to Y$ with finite operator norm $\|L\|_{\mathrm{op}}=\sup_{\|h\|_X\le1}\|Lh\|_Y$, such that

$$\lim_{0\ne h\to0}\frac{\|F(u+h)-F(u)-DF(u)h\|_Y}{\|h\|_X}=0,$$

and $\|DF(v)-DF(u)\|_{\mathrm{op}}\to0$ as $v\to u$. Completeness is not part of this definition.

The set $P=\{a\in\mathcal A_0:\inf_{\Sigma_1}a>0\}$ is open. If $a\in P$, in particular if a smooth $a\in\mathcal A_0$ satisfies $a\ge c>0$, then $a^{-1}\in\mathcal A_0$ and multiplication by either $a$ or $a^{-1}$ is bounded on every $\mathcal A_\beta$, $\beta\in\mathbb R$. Inversion $I:P\to\mathcal A_0$ is $C^1$, with $DI(a)h=-a^{-2}h$. The maps $M_\beta:\mathcal A_0\times\mathcal A_\beta\to\mathcal A_\beta$, $M_\beta(a,v)=av$, and $Q_\beta:P\times\mathcal A_\beta\to\mathcal A_\beta$, $Q_\beta(a,v)=a^{-1}v$, are $C^1$, with

$$DM_\beta(a,v)[h,w]=hv+aw,\qquad DQ_\beta(a,v)[h,w]=-a^{-2}hv+a^{-1}w.$$

More generally let $m,n\ge1$, let $V\subseteq\mathbb R^m$ be open, and let $G:V\to\mathbb R^n$ be smooth. The open domain for composition is

$$U_V=\{u\in(\mathcal A_0)^m:u(\Sigma_1)\subseteq V,\ \operatorname{dist}(u(\Sigma_1),\mathbb R^m\setminus V)>0\},$$

where distance to the empty set is $+\infty$. Then $N_G:U_V\to(\mathcal A_0)^n$, $N_G(u)=G\circ u$, is $C^1$, with $DN_G(u)h=DG(u)h$ pointwise. A slightly larger attained range means a fixed positive-radius tube about the closure of $u(\Sigma_1)$ contained in $V$. Bounds for composition use the norm of $u$ and uniform bounds for the derivatives of $G$ through order $k+1$ on such a tube; continuous differentiability uses derivatives through order $k+2$ there. These bounds and the derivative-continuity modulus are uniform over the scaled exterior annuli. Thus smooth bounded weighted arguments have the asserted bounded compositions and positive inverse multipliers, while differentiability is asserted on the specified open Hölder domains.

## Statement references

[def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[lem-author-45355d85383b-weighted-products-and-derivatives](item-lem-author-45355d85383b-weighted-products-and-derivatives)

## Facts & Assumptions

[F1] Weighted multiplication satisfies $\|fg\|_{\mathcal A_{\gamma+\eta}}\le C\|f\|_{\mathcal A_\gamma}\|g\|_{\mathcal A_\eta}$. The supplier's Proof 1.2, 1.3 and 2.1 also gives the Hölder product difference inequality and control of lower-order Hölder seminorms on the fixed scaled annulus and the fixed core chart subsets, even when the latter are not convex. [lem-author-45355d85383b-weighted-products-and-derivatives](item-lem-author-45355d85383b-weighted-products-and-derivatives)

[F2] The zero-weight norm controls the global value supremum and the full order-$k$ norms in every scaled annulus and fixed core chart. It defines a normed vector space; finite arrays use component sums. [def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[F3] Continuous coordinate partial derivatives imply total differentiability on chart interiors. The total chain rule, the scalar product and quotient rules on coordinate lines, and permutation of continuous mixed partials give finite iterated chain-rule expansions. Identities at the boundary follow by continuity from the interior. [math:thm-continuous-partial-derivatives-imply-total-differentiability](https://alphabetamath.cc/item/thm-continuous-partial-derivatives-imply-total-differentiability) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives) [math:thm-symmetry-of-higher-mixed-partials](https://alphabetamath.cc/item/thm-symmetry-of-higher-mixed-partials)

[F4] For a scalar $C^1$ function $f$ on an open interval containing $[0,1]$, Taylor's integral formula at order zero reads $f(1)-f(0)=\int_0^1 f'(t)\,dt$. We apply it componentwise to smooth finite-dimensional functions along segments lying inside $V$, using the total chain rule for their derivatives. [math:lem-taylor-integral-remainder](https://alphabetamath.cc/item/lem-taylor-integral-remainder) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F5] Closed bounded subsets of finite-dimensional Euclidean space are compact, and a continuous map on a compact metric space is uniformly continuous. Continuous derivatives on our compact tubes are also bounded: continuity supplies a neighborhood bound at each point and a finite subcover supplies one bound for the tube. [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn) [math:thm-heine-cantor-metric](https://alphabetamath.cc/item/thm-heine-cantor-metric)

## Proof

**Given:** The fixed weighted norms, the functions and the finite-dimensional smooth map in the Statement.

**Goal:** Establish the multiplier and composition bounds, the open domains, and all the stated normed-space derivatives and their continuity.

1.1 By [F2], $\|u\|_{(\mathcal A_0)^m}$ controls $\sup|u|$. Thus a sufficiently small norm perturbation of a point of $P$ preserves a positive lower bound, and a sufficiently small norm perturbation of a point of $U_V$ preserves a positive distance from the complement of $V$. This proves openness in the full spaces. Fix $u\in U_V$ and choose $\delta>0$ with $4\delta<\operatorname{dist}(u(\Sigma_1),\mathbb R^m\setminus V)$, choosing any finite such $\delta$ if the complement is empty. The closure $S=\overline{u(\Sigma_1)}$ is bounded, and its closed $2\delta$-tube $K_u=\{z:\operatorname{dist}(z,S)\le2\delta\}$ is closed, bounded and contained in $V$. Closedness follows from $|\operatorname{dist}(z,S)-\operatorname{dist}(z',S)|\le|z-z'|$, which follows directly by taking infima in the triangle inequality. Hence $K_u$ is compact by [F5]. All derivatives of $G$ needed below are bounded and uniformly continuous on $K_u$. Norm-small $h$ have $\sup|h|<\delta/2$, so the segments $u(p)+th(p)$ lie in this same tube. [F2, F5, given, algebra]

2.1 Work on the fixed annulus in scaled coordinates, or on a fixed core chart subset, and denote that coordinate set by $E$. The scaled order-$k$ norms of $u$ and $h$ are bounded uniformly by their zero-weight norms. For a smooth coefficient $H$ on the tube, the segment formula in [F4] gives $|H(u(p))-H(u(q))|\le C|u(p)-u(q)|$ when $|u(p)-u(q)|<\delta$; this segment stays within the tube. For the remaining pairs, boundedness of $H$ gives $|H(u(p))-H(u(q))|\le2\sup_{K_u}|H|\,|u(p)-u(q)|/\delta$. Therefore its Hölder seminorm is bounded by a constant times $[u]_{\alpha;E}$. For $1\le|J|\le k$, repeated coordinate chain and product rules express $\partial^J(G(u))$ as a finite sum of a component of $D^jG(u)$ times components of derivatives of $u$ of positive orders adding to $|J|$, with $1\le j\le|J|$. Apply the coefficient estimate, [F1]'s lower-order seminorm bounds, and its product difference inequality to every factor. This proves the order-$k$ composition bound on each $E$, using derivatives of $G$ only through order $k+1$. For $k=0$ just the coefficient estimate and the value supremum suffice. Taking the annular supremum and adding the core norms proves $G(u)\in(\mathcal A_0)^n$. The same calculation on compact coordinate neighborhoods proves the required local Hölder regularity, and continuity extends the derivative formulas to the boundary. [F1, F2, F3, F4, step 1.1, algebra]

3.1 We next prove continuity of $u\mapsto DG(u)$ in the order-$k$ zero-weight norm, rather than assume it from a formal chain rule. Let $H$ be any component of $D^{j+1}G$, $0\le j\le k$, and put $b=H(u+h)-H(u)$ and $\varepsilon=\|h\|_{(\mathcal A_0)^m}$. Its supremum is at most $C\varepsilon$ by [F4]. For a pair with $|u(p)-u(q)|<\delta$, split the increment of $b$ by first replacing $h(p)$ by $h(q)$. That change is at most $C|h(p)-h(q)|$. The remaining difference is the difference of two increments of $H$ along the parallel segments from $u(q)$ to $u(p)$ and from $u(q)+h(q)$ to $u(p)+h(q)$. Apply [F4] on those segments. Uniform continuity of $DH$ on $K_u$ bounds their difference by $\omega(C\varepsilon)|u(p)-u(q)|$, for a common modulus $\omega(s)\to0$ as $s\to0$. All these segments lie in $K_u$. For a pair with $|u(p)-u(q)|\ge\delta$, use the supremum bound on $b$ and $|u(p)-u(q)|\le[u]_{\alpha;E}|p-q|^\alpha$. Consequently $[b]_{\alpha;E}\le C[h]_{\alpha;E}+\bigl(\omega(C\varepsilon)+C\varepsilon/\delta\bigr)[u]_{\alpha;E}.$ The right side tends to zero uniformly over all $E$, by [F1] and [F2]. Derivatives of $H$ used here have order at most $k+2$ as derivatives of $G$. In the finite chain-rule expansions for the derivatives through order $k$ of $DG(u+h)-DG(u)$, the coefficient differences therefore tend to zero in $C^{0,\alpha}(E)$, while differences of the derivative factors of $u$ are derivatives of $h$, whose relevant supremum and Hölder bounds tend to zero by [F1]. Subtract products one factor at a time and use the Hölder product difference inequality. This proves $\|DG(u+h)-DG(u)\|_{(\mathcal A_0)^{n\times m}}\to0$, uniformly over annuli. The proof includes $k=0$, where there are no differentiated factors of $u$. [F1, F2, F3, F4, F5, step 1.1, step 2.1, algebra]

4.1 Apply [F4] componentwise to $t\mapsto G(u(p)+th(p))$; smoothness and step 1.1 give its $C^1$ extension to an open interval containing $[0,1]$. Subtracting its linear part gives the pointwise identity $G(u+h)-G(u)-DG(u)h=\int_0^1\bigl(DG(u+th)-DG(u)\bigr)h\,dt.$ The integral here is an ordinary finite-dimensional integral at each point, not an assumed integral in a complete function space. Coordinate derivatives through order $k$ may pass under it: for the first derivative the difference quotient equals the integral of the difference quotients, and the segment formula in the coordinate direction and continuity of that derivative on the compact parameter interval imply uniform convergence in $t$; repeat for the subsequent derivatives. This argument is local on chart interiors; continuous derivative extensions give boundary values. The triangle inequality for finite Riemann sums and their limits, applied also to each two-point difference, gives the integral bound in every chart norm. Using [F1] and step 3.1 thus yields $\|G(u+h)-G(u)-DG(u)h\|_{(\mathcal A_0)^n}\le C\|h\|_{(\mathcal A_0)^m}\sup_{0\le t\le1}\|DG(u+th)-DG(u)\|_{(\mathcal A_0)^{n\times m}}=o(\|h\|_{(\mathcal A_0)^m}).$ The supremum tends to zero because step 3.1 bounds it by a common modulus of $\|h\|$. Step 2.1 applied to $DG$ gives a bounded coefficient multiplier, so $h\mapsto DG(u)h$ is bounded linear by [F1]. That same product bound and step 3.1 give continuity in operator norm. This verifies precisely the normed-space definition in the Statement. [F1, F2, F3, F4, F5, step 1.1, step 2.1, step 3.1, algebra]

5.1 Take $V=(0,\infty)$ and $G(s)=s^{-1}$. Its domain $U_V$ is exactly $P$, and a positive lower bound and a finite value supremum bound all derivatives of $G$ on a slightly larger positive range. Steps 2.1 and 4.1 therefore give $a^{-1}\in\mathcal A_0$ and $DI(a)h=-a^{-2}h$. By [F1], $a$ and $a^{-1}$ act boundedly on every $\mathcal A_\beta$. These maps are inverse multiplication operators, since their pointwise products equal one. This includes the original smooth-input claim without restricting the perturbations to smooth functions. [F1, F2, F3, step 1.1, step 2.1, step 4.1, algebra]

6.1 For multiplication, $(a+h)(v+w)-av-hv-aw=hw$, whose $\mathcal A_\beta$ norm is at most $C\|h\|_{\mathcal A_0}\|w\|_{\mathcal A_\beta}$ by [F1]. This is a quadratic remainder in the sum norm, and the displayed derivative of $M_\beta$ varies continuously in operator norm by the same estimate. Write $I(a+h)=I(a)-a^{-2}h+r(h)$, with $\|r(h)\|_{\mathcal A_0}=o(\|h\|_{\mathcal A_0})$ from step 5.1. Expanding $I(a+h)(v+w)$ leaves, after subtracting the displayed derivative of $Q_\beta$, the terms $r(h)v+(I(a+h)-I(a))w$, which are $o(\|h\|_{\mathcal A_0}+\|w\|_{\mathcal A_\beta})$ by [F1] and continuity of $I$. The coefficient fields $I(a)$ and $-a^{-2}$ vary continuously in $\mathcal A_0$ by steps 3.1 and 5.1, so the derivative of $Q_\beta$ is continuous in operator norm. All claimed maps and bounds follow. [F1, step 3.1, step 5.1, algebra] ∎

---
title: Compactly supported chart mollification in uniform and first Sobolev norms
status: draft
research_item: lem-author-423fe0348a31-compact-chart-mollification
dependency_level: 0
---

## Prerequisites

- [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm)
- [math:def-mollifier-family-generated-by-a-unit-mass-smooth-bump](https://alphabetamath.cc/item/def-mollifier-family-generated-by-a-unit-mass-smooth-bump)
- [math:lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice](https://alphabetamath.cc/item/lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice)
- [math:lem-mollification-commutes-with-weak-derivatives-in-the-interior](https://alphabetamath.cc/item/lem-mollification-commutes-with-weak-derivatives-in-the-interior)
- [math:thm-translation-is-continuous-in-l-p-for-one-le-p-less-infinity](https://alphabetamath.cc/item/thm-translation-is-continuous-in-l-p-for-one-le-p-less-infinity)
- [math:thm-convolution-with-a-mollifier-is-smooth-and-differentiates-under-the-integral-sign](https://alphabetamath.cc/item/thm-convolution-with-a-mollifier-is-smooth-and-differentiates-under-the-integral-sign)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:lem-smooth-bump-between-concentric-euclidean-balls](https://alphabetamath.cc/item/lem-smooth-bump-between-concentric-euclidean-balls)
- [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction)
- [math:def-convolution-of-two-functions-on-rn](https://alphabetamath.cc/item/def-convolution-of-two-functions-on-rn)
- [math:thm-minkowski-integral-inequality](https://alphabetamath.cc/item/thm-minkowski-integral-inequality)
- [math:thm-integral-triangle-inequality](https://alphabetamath.cc/item/thm-integral-triangle-inequality)
- [math:thm-linear-change-of-variables-for-lebesgue-measure](https://alphabetamath.cc/item/thm-linear-change-of-variables-for-lebesgue-measure)
- [math:thm-lebesgue-outer-measure-and-measurability-are-translation-invariant](https://alphabetamath.cc/item/thm-lebesgue-outer-measure-and-measurability-are-translation-invariant)
- [math:def-borel-and-lebesgue-measurable-function-on-rn](https://alphabetamath.cc/item/def-borel-and-lebesgue-measurable-function-on-rn)
- [math:thm-the-l-p-norm-descends-to-the-quotient-and-makes-l-p-a-normed-space](https://alphabetamath.cc/item/thm-the-l-p-norm-descends-to-the-quotient-and-makes-l-p-a-normed-space)
- [math:def-support-and-compactly-supported-riemann-integral-in-rn](https://alphabetamath.cc/item/def-support-and-compactly-supported-riemann-integral-in-rn)
- [math:def-c-c-and-c-c-infinity-on-rn](https://alphabetamath.cc/item/def-c-c-and-c-c-infinity-on-rn)


## Statement

Work in ZFC. Let $n\ge1$, let $V\subset\mathbb R^n$ be open, and let $f:V\to\mathbb R$ be Lipschitz and compactly supported in $V$: the Euclidean closure $K=\overline{\{x\in V:f(x)\ne0\}}^{\mathbb R^n}$ is compact and contained in $V$. Its extension by zero $\widetilde f:\mathbb R^n\to\mathbb R$ is globally Lipschitz and belongs to $W^{1,1}(\mathbb R^n;\mathbb R)$. Write $f$ also for this zero extension whenever its argument ranges over $\mathbb R^n$; all $L^p$ and Sobolev spaces in this item are real. Fix a nonnegative $\rho\in C_c^\infty(\mathbb R^n)$ with $\int_{\mathbb R^n}\rho=1$ and $\operatorname{supp}\rho\subseteq\overline B_1(0)$, and for $\eta>0$ set $\rho_\eta(x)=\eta^{-n}\rho(x/\eta)$. The functions $f_\eta=\rho_\eta*f$ are smooth, supported in a fixed compact subset of $V$ for all sufficiently small $\eta$, and converge to $f$ both uniformly and in $W^{1,1}(\mathbb R^n)$. Such nonnegative unit-mass kernels exist in every dimension $n\ge1$.

## Facts & Assumptions

[F1] Real-valued locally Lipschitz functions are differentiable almost everywhere; their measurable partial derivatives are weak derivatives and satisfy $|Dh|\le L$ almost everywhere on every $L$-Lipschitz open region. [math:lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice](https://alphabetamath.cc/item/lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice)

[F2] Convolution commutes with weak derivatives, including on all of Euclidean space for the zero extension. [math:lem-mollification-commutes-with-weak-derivatives-in-the-interior](https://alphabetamath.cc/item/lem-mollification-commutes-with-weak-derivatives-in-the-interior)

[F3] Translations are continuous in $L^p$ for $1\le p<\infty$; use $p=1$ for the function and its weak first derivatives. [math:thm-translation-is-continuous-in-l-p-for-one-le-p-less-infinity](https://alphabetamath.cc/item/thm-translation-is-continuous-in-l-p-for-one-le-p-less-infinity)

[F4] Convolution with a compactly supported smooth mollifier is smooth and differentiates under the integral. [math:thm-convolution-with-a-mollifier-is-smooth-and-differentiates-under-the-integral-sign](https://alphabetamath.cc/item/thm-convolution-with-a-mollifier-is-smooth-and-differentiates-under-the-integral-sign)

[F5] Work in ZFC, carrying the analytic suppliers' countable-choice assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F6] Membership in the real space $W^{1,1}(\mathbb R^n;\mathbb R)$ means that the function and each weak first derivative belong to $L^1$, and $\|u\|_{W^{1,1}}=\|u\|_1+\sum_{i=1}^n\|D_i u\|_1$. [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm)

[F7] The mollifier family is generated by the fixed kernel $\rho$ via $\rho_\eta(x)=\eta^{-n}\rho(x/\eta)$. Its mass is one, and the stated unit-ball support gives $\operatorname{supp}\rho_\eta\subseteq\overline B_\eta(0)$. [math:def-mollifier-family-generated-by-a-unit-mass-smooth-bump](https://alphabetamath.cc/item/def-mollifier-family-generated-by-a-unit-mass-smooth-bump)

[F8] For every $n\ge1$, a nonnegative smooth bump equals one on $\overline B_{1/2}(0)$ and has support in $B_1(0)$. [math:lem-smooth-bump-between-concentric-euclidean-balls](https://alphabetamath.cc/item/lem-smooth-bump-between-concentric-euclidean-balls)

[F9] In the Euclidean metrics, Lipschitz means that some $L\ge0$ satisfies $|f(x)-f(y)|\le L|x-y|$ for every pair in the domain. [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction)

[F10] For measurable functions, $(a*b)(x)=\int a(x-y)b(y)\,dy$ whenever the integrand is measurable and integrable. [math:def-convolution-of-two-functions-on-rn](https://alphabetamath.cc/item/def-convolution-of-two-functions-on-rn)

[F11] On sigma-finite measure spaces, if $F(x,z)$ is product-measurable and $\int\|F(\cdot,z)\|_1\,dz<\infty$, then $H(x)=\int|F(x,z)|\,dz$ belongs to $L^1$ and $\|H\|_1\le\int\|F(\cdot,z)\|_1\,dz$. This is the $p=1$ case of Minkowski's integral inequality. [math:thm-minkowski-integral-inequality](https://alphabetamath.cc/item/thm-minkowski-integral-inequality)

[F12] For an integrable real or complex function $u$, $|\int u|\le\int|u|$. [math:thm-integral-triangle-inequality](https://alphabetamath.cc/item/thm-integral-triangle-inequality)

[F13] Lebesgue measure is translation invariant, and an invertible linear map scales it by the absolute determinant. The corresponding integral substitutions follow first for indicator functions, then simple functions and their increasing limits; apply this also to positive and negative parts of integrable functions. In particular, $y=x-\eta z$ has volume factor $\eta^n$, and translations preserve $L^1$ norms. [math:thm-linear-change-of-variables-for-lebesgue-measure](https://alphabetamath.cc/item/thm-linear-change-of-variables-for-lebesgue-measure) [math:thm-lebesgue-outer-measure-and-measurability-are-translation-invariant](https://alphabetamath.cc/item/thm-lebesgue-outer-measure-and-measurability-are-translation-invariant)

[F14] A map from $\mathbb R^d$ to $\mathbb R^m$ is Borel measurable when it is measurable between their Borel sigma-algebras; use $m=1$ for real-valued functions. [math:def-borel-and-lebesgue-measurable-function-on-rn](https://alphabetamath.cc/item/def-borel-and-lebesgue-measurable-function-on-rn)

[F15] For a measure space, the real $L^1$ quotient norm is well defined and satisfies $\|u+v\|_1\le\|u\|_1+\|v\|_1$ and $\|a u\|_1=|a|\|u\|_1$. [math:thm-the-l-p-norm-descends-to-the-quotient-and-makes-l-p-a-normed-space](https://alphabetamath.cc/item/thm-the-l-p-norm-descends-to-the-quotient-and-makes-l-p-a-normed-space)

[F16] For a real-valued function $h$ on $\mathbb R^n$, $\operatorname{supp}h$ is the Euclidean closure of its nonzero set; compact support means that this closure is compact. Applied to the zero extension of $f:V\to\mathbb R$, its nonzero set is $\{x\in V:f(x)\ne0\}$, so its support is exactly the set $K$ specified in the Statement. [math:def-support-and-compactly-supported-riemann-integral-in-rn](https://alphabetamath.cc/item/def-support-and-compactly-supported-riemann-integral-in-rn)

[F17] The space $C_c(\mathbb R^n)$ consists of real-valued continuous functions on $\mathbb R^n$ with compact support, and $C_c^\infty(\mathbb R^n)$ is its subspace of smooth functions. [math:def-c-c-and-c-c-infinity-on-rn](https://alphabetamath.cc/item/def-c-c-and-c-c-infinity-on-rn)

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the stated construction or identity.

1.1 By [F8], choose a bump $b$ equal to one on $\overline B_{1/2}(0)$ with support in $B_1(0)$. Its integral is positive and finite, so $b/\int b$ is an admissible kernel, proving the existence assertion with the real smooth-function convention of [F17]; the rest of the proof applies to any fixed kernel in the Statement. By [F16], the set $K$ in the Statement is $\operatorname{supp}\widetilde f$. If $K$ is empty, all asserted functions are zero. Otherwise compactness gives $\eta_0>0$ such that $K+\overline B_{\eta_0}(0)$ is compact and contained in $V$; when $V=\mathbb R^n$, take any $\eta_0>0$. The zero extension $\widetilde f$ is globally Lipschitz: for $x\in V$ and $y\notin V$, approach the first exit point of the segment from $x$ to $y$ from within $V$. The function is zero near that exit point because $K$ stays away from the complement, so the Lipschitz inequality gives $|f(x)|\le L|x-y|$. Pairs in $V$ satisfy the original bound and pairs outside have zero difference. By [F1], $\widetilde f$ has bounded weak derivatives, zero almost everywhere off $K$, so the function and these derivatives are integrable and [F6] gives $\widetilde f\in W^{1,1}(\mathbb R^n)$. The support of $\rho_\eta*\widetilde f$ lies in $K+\overline B_\eta(0)$, hence in the fixed compact subset above for $0<\eta\le\eta_0$. [given, F1, F5, F6, F7, F8, F9, F10, F16, F17, construct, algebra]

2.1 By [F7], [F10] and the substitution in [F13], $f_\eta(x)-f(x)=\int\rho(z)(f(x-\eta z)-f(x))\,dz$. The integrand is integrable since $f$ is bounded and $\rho$ has compact support. Thus [F9] and [F12] give $\|f_\eta-f\|_\infty\le L\eta\int|z|\rho(z)\,dz$, proving uniform convergence. For the Sobolev estimate take $g=f$ or a representative of one of its weak first derivatives. For a derivative, choose the following Borel representative in the sense of [F14]: take the limit of the continuous difference quotients $m(f(x+e_i/m)-f(x))$ where the sequence converges and put zero elsewhere, where $e_i$ is the $i$th coordinate vector. The convergence set is Borel by the countable Cauchy criterion, and the resulting function is Borel measurable. It agrees almost everywhere with $D_i f$ by [F1]. The function $f$ itself is continuous. Consequently $F_\eta(x,z)=\rho(z)(g(x-\eta z)-g(x))$ is product-measurable for the Borel sigma-algebras: the product Borel sigma-algebra is the Euclidean Borel sigma-algebra because open rectangles from countable bases generate the product topology; compose the Borel functions with the continuous affine maps and take their difference and product. Each Euclidean Borel Lebesgue measure space is sigma-finite, being covered by bounded cubes. By [F13] and the $L^1$ norm triangle inequality and homogeneity from [F15], $\int\|F_\eta(\cdot,z)\|_1\,dz\le2\|g\|_1\int\rho(z)\,dz=2\|g\|_1<\infty$. All hypotheses of [F11] are therefore satisfied. [F1, F5, F6, F7, F9, F10, F11, F12, F13, F14, F15, step 1.1, construct, algebra]

3.1 Applying [F11] gives $H_\eta(x)=\int|F_\eta(x,z)|\,dz\in L^1$. Hence $F_\eta(x,\cdot)$ is integrable for almost every $x$, and the convolution substitution [F10], [F13], its unit mass [F7] and [F12] imply $|(\rho_\eta*g)(x)-g(x)|\le H_\eta(x)$ almost everywhere. It follows that $\|\rho_\eta*g-g\|_1\le\int\rho(z)\|g(\cdot-\eta z)-g\|_1\,dz$. Given $\varepsilon>0$, [F3] supplies $\delta>0$ such that $|h|<\delta$ implies $\|g(\cdot-h)-g\|_1<\varepsilon$. If $0<\eta<\delta$, every $z$ in the unit-ball support of $\rho$ satisfies this bound with $h=\eta z$, so the last integral is at most $\varepsilon\int\rho=\varepsilon$. This proves convergence for $f$ and each weak first derivative. Apply [F2] with $\Omega=\mathbb R^n$, $k=1$, $p=1$ and the kernel specified in the Statement; its hypotheses hold by step 1.1, so commutation of convolution with weak derivatives and [F6] prove the $W^{1,1}$ convergence. The smoothness supplier [F4] applies because $f$ is locally integrable and the fixed kernel is smooth, compactly supported and of mass one. Together with the support conclusion in step 1.1 and the uniform convergence in step 2.1, this proves every assertion. [F2, F3, F4, F5, F6, F7, F10, F11, F12, F13, step 1.1, step 2.1, algebra] ∎

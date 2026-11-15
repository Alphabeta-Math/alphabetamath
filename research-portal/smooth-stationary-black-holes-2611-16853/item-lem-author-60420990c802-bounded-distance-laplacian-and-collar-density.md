---
title: Distance Laplacian and normal-collar volume density are uniformly bounded
status: draft
research_item: lem-author-60420990c802-bounded-distance-laplacian-and-collar-density
dependency_level: 2
---

## Prerequisites

- [lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance](item-lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance)
- [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)
- [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)
- [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)
- [math:thm-tonelli-and-fubini-for-completed-product-measures](https://alphabetamath.cc/item/thm-tonelli-and-fubini-for-completed-product-measures)
- [lem-author-60420990c802-uniform-inward-normal-exponential-collar](item-lem-author-60420990c802-uniform-inward-normal-exponential-collar)
- [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)
- [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density)
- [math:prop-density-pullback-under-local-diffeomorphisms](https://alphabetamath.cc/item/prop-density-pullback-under-local-diffeomorphisms)
- [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)
- [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing)
- [math:lem-borel-product-of-second-countable-spaces](https://alphabetamath.cc/item/lem-borel-product-of-second-countable-spaces)
- [math:thm-lebesgue-product-measure-agrees-with-euclidean-lebesgue-on-borel-sets](https://alphabetamath.cc/item/thm-lebesgue-product-measure-agrees-with-euclidean-lebesgue-on-borel-sets)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)
- [math:def-completion-of-a-measure-space](https://alphabetamath.cc/item/def-completion-of-a-measure-space)
- [math:def-completed-product-measure](https://alphabetamath.cc/item/def-completed-product-measure)


## Statement

Work in ZFC. Let $(\Sigma,h)$ be a smooth Riemannian manifold with compact boundary $S$ and metric smooth and positive up to $S$. Let $F(p,s)=\exp_p(s\nu_p)$, with $\nu$ the inward unit normal, be the supplied uniform inward normal exponential collar. On a sufficiently small fixed collar its coordinate equals the extended intrinsic boundary distance $\rho(x)=\inf_{y\in S}d_h(x,y)$, as supplied by the intrinsic-distance lemma, and $F^*h=ds^2+h_s$. Distances between different components are $+\infty$, and $\inf\varnothing=+\infty$. Use the sign convention $\Delta_h=\operatorname{div}_h\nabla_h$, with its smooth one-sided extension to $S$.

Write $dV_h$ and $dA_{h_0}$ for the Riemannian volume and induced boundary-area densities and their associated Radon Borel measures, using their completions when the domain is completed measurable; write $|S|=\int_SdA_{h_0}$. There are constants $C,K<\infty$ and a fixed width $a_0>0$ such that $\{0\le\rho\le a_0\}=F(S\times[0,a_0])$, $|\Delta_h\rho|\le C$ on this collar, and
$$F^*dV_h=j(p,s)\,dA_{h_0}(p)\,ds,\qquad 0<j(p,s)\le K,\qquad 0\le s\le a_0.$$
Here $ds$ denotes ordinary one-dimensional Lebesgue measure in the measure formula, and the formula also holds as an equality of smooth densities. Consequently every region $\Omega\subset\{0\le\rho\le\eta\}$ measurable for the completion of Riemannian Borel volume, with $0\le\eta\le a_0$, satisfies $\operatorname{Vol}_h(\Omega)\le K\eta|S|$. In particular this covers every Borel region. The constants depend only on the fixed metric and collar, not on $\eta$ or the chosen region.

## Facts & Assumptions

[F1] The uniform normal-exponential supplier specifies $(\Sigma,h)$, its compact boundary $S$, its inward unit normal and an embedded collar $F$ whose closed truncations lie in a larger relatively open collar. The intrinsic-distance supplier gives $F^*h=ds^2+h_s$, $\rho\circ F=s$ and $\nabla_h\rho=\partial_s$ after shrinking. The length of a piecewise $C^1$ path is the sum of the integrals of its metric speed. [lem-author-60420990c802-uniform-inward-normal-exponential-collar](item-lem-author-60420990c802-uniform-inward-normal-exponential-collar) [lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance](item-lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance) [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)

[F2] The Laplace–Beltrami operator is the trace of the Hessian, equivalently $\operatorname{div}_h\nabla_h$, with the positive-divergence sign convention and one-sided smooth boundary extension. Gradient and divergence have their Levi-Civita formulas; in coordinates divergence is the density-weighted derivative. [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian) [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas) [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)

[F3] Riemannian density has coefficient $\sqrt{\det G}$, including the empty determinant in dimension zero. Density pullback by a local diffeomorphism multiplies its composed coefficient by the absolute Jacobian determinant, also in boundary charts. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:prop-density-pullback-under-local-diffeomorphisms](https://alphabetamath.cc/item/prop-density-pullback-under-local-diffeomorphisms)

[F4] Under countable choice, Riemannian density defines a compact-finite, sigma-finite Radon Borel measure; apply this both to $(\Sigma,h)$ and to $(S,h_0)$. A completed measurable set differs from a Borel set by a subset of a Borel null set. The completed measure uses the Borel value. [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density) [math:def-completion-of-a-measure-space](https://alphabetamath.cc/item/def-completion-of-a-measure-space)

[F5] Under countable choice, the measure of a Borel set contained in one chart is the Lebesgue integral of the density coefficient there. Nonnegative Borel integrals have the chart-partition formula, and completion-measurable nonnegative functions have Borel representatives modulo null sets. Both suppliers allow manifolds with boundary and dimension zero. [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing) [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)

[F6] For second-countable spaces the Borel sigma-algebra of the product equals the product Borel sigma-algebra. Under countable choice, the product of Euclidean Lebesgue measures agrees with Euclidean Lebesgue measure on Borel sets for positive-dimensional factors. [math:lem-borel-product-of-second-countable-spaces](https://alphabetamath.cc/item/lem-borel-product-of-second-countable-spaces) [math:thm-lebesgue-product-measure-agrees-with-euclidean-lebesgue-on-borel-sets](https://alphabetamath.cc/item/thm-lebesgue-product-measure-agrees-with-euclidean-lebesgue-on-borel-sets)

[F7] The completion of a sigma-finite product measure adds subsets of product null sets. Tonelli applies to nonnegative functions measurable for that completion and identifies their product integral with the iterated integrals, with section assertions only almost everywhere as required by its interface. [math:def-completed-product-measure](https://alphabetamath.cc/item/def-completed-product-measure) [math:thm-tonelli-and-fubini-for-completed-product-measures](https://alphabetamath.cc/item/thm-tonelli-and-fubini-for-completed-product-measures)

[F8] ZFC includes the Axiom of Choice. Its countable-choice consequence supplies the foundational assumption of the measure, chart-integration and completed-product inputs in [F4]–[F7], as well as the choice assumption inherited from the collar suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

## Proof

**Given:** The hypotheses in the Statement, in ZFC as in [F8].

**Goal:** Establish the uniform Laplacian, density and measurable-volume bounds on one fixed distance collar.

1.1 First take $b>0$ such that $F(S\times[0,b])$ lies inside a larger collar where the Gaussian metric and distance identities of [F1] hold, and fix $0<a_0<b$. Every path starting at $S$ that leaves the width-$b$ collar must first cross its outer face. On its initial portion, the Gaussian metric gives $|\dot\gamma|_h\ge|s'|$, hence length at least $b$. Thus every point outside that collar has boundary distance at least $b$: take the infimum of these lengths; a component with no boundary has distance $+\infty$. Inside the collar $\rho=s$, so $\{0\le\rho\le\eta\}=F(S\times[0,\eta])$ for every $0\le\eta\le a_0$. If $S=\varnothing$, all these sets are empty, their volumes vanish, and the conclusions are vacuous with any positive $a_0,C,K$; henceforth take $S\ne\varnothing$. [F1, F8, given]

2.1 In a boundary chart the Gaussian metric determinant is $\det h_s$ and $\nabla\rho=\partial_s$. The fixed sign convention and the coordinate divergence formula give $$\Delta_h\rho=(\det h_s)^{-1/2}\partial_s\sqrt{\det h_s}=\tfrac12\operatorname{tr}(h_s^{-1}\partial_s h_s).$$ The last equality follows by differentiating the determinant column by column, giving $\partial_s\det h_s=(\det h_s)\operatorname{tr}(h_s^{-1}\partial_s h_s)$. The resulting scalar is smooth up to $S$ and on the compact collar $F(S\times[0,a_0])$, so its absolute value has a finite upper bound $C$. [F1, F2, step 1.1, algebra]

2.2 In boundary coordinates set $j(p,s)=\sqrt{\det h_s/\det h_0}$. A change of boundary coordinates multiplies both determinants by the same squared Jacobian, so the ratio is intrinsic. It is smooth and positive and equals one at $s=0$; compactness gives constants $0<m\le j\le K<\infty$ on $S\times[0,a_0]$. In the product coordinates the pulled-back volume density has coefficient $\sqrt{\det h_s}=j\sqrt{\det h_0}$, proving the stated smooth-density formula by the density pullback law. The pullback is first taken on the larger relatively open collar, where $F$ is a local diffeomorphism, and then restricted to this closed truncation. [F1, F3, step 1.1, algebra]

3.1 Let $E\subset S\times[0,a_0]$ be Borel. Choose a finite boundary-chart cover $U_i$ of compact $S$, and partition $S$ into the disjoint Borel sets $P_1=U_1$, $P_i=U_i\setminus\bigcup_{k<i}U_k$. In the collar chart $(x_i,s)$ over $U_i$, [F5] computes the volume of $F(E\cap(P_i\times[0,a_0]))$ by the Euclidean integral of $\mathbf1_E\sqrt{\det h_s}$. The maps in question are homeomorphisms onto their images, so these sets are Borel. When $\dim S\ge1$, [F6] splits this Euclidean measure as the product of the boundary-coordinate Lebesgue measure and $ds$. Tonelli then makes that integral the iterated integral of $\mathbf1_E j\sqrt{\det h_0}$. The boundary chart-integration formula identifies the inner integral with the $dA_{h_0}$ integral over $P_i$; summing the finite disjoint partition and applying Tonelli to $dA_{h_0}\times ds$ gives $$\operatorname{Vol}_h(F(E))=\int_E j\,d(dA_{h_0}\times ds).$$ The measures are sigma-finite by [F4], and all integrands are nonnegative Borel and hence measurable on the completed products by [F6]–[F7]; [F8] supplies countable choice. If $\dim S=0$, compact $S$ is finite and its induced measure is counting measure by [F3]–[F4]; the same equality follows by summing the one-dimensional interval chart integrals, without applying the positive-dimensional Euclidean product theorem to a zero-dimensional factor. [F3, F4, F5, F6, F7, F8, step 2.2]

4.1 The lower bound $j\ge m>0$ and upper bound $j\le K$ show from step 3.1 that the pulled-back volume and the product measure have exactly the same Borel null sets. Consequently the homeomorphism $F$ identifies their completion domains as well: write a completed measurable set as a Borel set together with a subset of a Borel null set, transport this representation by $F$, and use the same zero measure on the null subset. Applying this to both directions extends the measure identity of step 3.1 to the completions. This justifies the measure interpretation of the displayed pullback formula for every measurable region asserted in the Statement. [F4, F7, step 2.2, step 3.1]

5.1 Compact-finiteness gives $|S|<\infty$. For $0\le\eta\le a_0$ and a completed-volume-measurable $\Omega\subset\{0\le\rho\le\eta\}$, put $E=F^{-1}(\Omega)\subset S\times[0,\eta]$. Steps 3.1 and 4.1 and nonnegativity yield $$\operatorname{Vol}_h(\Omega)=\int_E j\,d\overline{(dA_{h_0}\times ds)}\le K\,(dA_{h_0}\times ds)(S\times[0,\eta])=K\eta|S|.$$ The rectangle value follows also by Tonelli on its indicator. It is zero when $\eta=0$. The constants $C,K,a_0$ were fixed before choosing $\eta$ and $\Omega$, proving the claimed uniformity. [F4, F7, step 1.1, step 2.1, step 2.2, step 3.1, step 4.1] ∎

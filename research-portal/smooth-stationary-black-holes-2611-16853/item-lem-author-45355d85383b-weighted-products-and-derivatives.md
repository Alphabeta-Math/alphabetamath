---
title: Weighted differentiation and multiplication estimates
status: draft
research_item: lem-author-45355d85383b-weighted-products-and-derivatives
dependency_level: 2
---

## Prerequisites

- [def-weighted-holder-spaces](item-def-weighted-holder-spaces)
- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:thm-continuous-partial-derivatives-imply-total-differentiability](https://alphabetamath.cc/item/thm-continuous-partial-derivatives-imply-total-differentiability)
- [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)
- [math:thm-symmetry-of-higher-mixed-partials](https://alphabetamath.cc/item/thm-symmetry-of-higher-mixed-partials)
- [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)
- [math:def-cotangent-space-and-cotangent-bundle-as-a-disjoint-union](https://alphabetamath.cc/item/def-cotangent-space-and-cotangent-bundle-as-a-disjoint-union)
- [math:thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary](https://alphabetamath.cc/item/thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary)


## Statement

Fix the smooth three-dimensional exterior, end coordinates $x$, radius $r_0>0$, compact core $K$, and finite compact chart subsets used in the weighted-space definition. Let $k\ge0$ be an integer, $0<\alpha<1$, and $\gamma,\eta\in\mathbb R$. For an end component $v$, write $E^{k,\alpha}_\gamma(v)$ for the annular part of its weighted norm, obtained by omitting the compact-core term $N_K(v)$.

At every point $p\in\Sigma_1$, including boundary points, $T_p^*\Sigma_1$ is the linear dual of $T_p\Sigma_1$. A covector field here means an assignment $p\mapsto\omega_p\in T_p^*\Sigma_1$; its local regularity is measured by its coefficients in the coordinate dual frames, using continuous boundary values in boundary charts.

For a scalar $f\in C^{k,\alpha}_\gamma$ with $k\ge1$, define $df$ by the components $\partial_{z^i}(f\circ z^{-1})$ in each smooth coordinate chart $z$, with boundary values given by continuity. These components define a global covector field. Measure its norm componentwise in the same fixed core charts and end chart. Then

$$\|df\|_{C^{k-1,\alpha}_{\gamma-1}}\le C\|f\|_{C^{k,\alpha}_\gamma}.$$

For any end component of finite annular norm, differentiation on the end satisfies

$$E^{k-1,\alpha}_{\gamma-1}(\partial_{x^i}v)\le C E^{k,\alpha}_\gamma(v)\qquad(k\ge1).$$

For $f\in C^{k,\alpha}_\gamma$ and $g\in C^{k,\alpha}_\eta$, multiplication and inclusion satisfy

$$\|fg\|_{C^{k,\alpha}_{\gamma+\eta}}\le C\|f\|_{C^{k,\alpha}_\gamma}\|g\|_{C^{k,\alpha}_\eta},\qquad \|f\|_{C^{k,\alpha}_\eta}\le C\|f\|_{C^{k,\alpha}_\gamma}\quad(\gamma\le\eta).$$

Here each constant is independent of the functions and annular radius and may depend on the fixed charts, $k,\alpha,r_0$ and weights. The product and inclusion estimates also hold for finite component arrays and tensor component products and contractions, computed as finite sums of component products with constant numerical coefficients in the specified charts. End-component differentiation obeys the stated annular estimate for each tensor component.

## Statement references

[def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[math:def-cotangent-space-and-cotangent-bundle-as-a-disjoint-union](https://alphabetamath.cc/item/def-cotangent-space-and-cotangent-bundle-as-a-disjoint-union)

[math:thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary](https://alphabetamath.cc/item/thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary)

## Facts & Assumptions

[F1] The weighted norm is the sum of the compact-core norm and a supremum of scaled annular norms, with tensor norms formed by finite component sums. [def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[F2] The core is compact and its fixed chart subsets are compact inside smooth interior or boundary charts; coordinate transitions are smooth. The subsets themselves need not be convex. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F3] The unweighted norm controls all derivative suprema through its order and the top-order Hölder seminorm; derivatives and their continuous boundary values use the stated local Hölder conventions. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F4] Continuous first partial derivatives give total differentiability with the Jacobian derivative, and the total chain rule applies to such maps. We use these results on open chart interiors, and pass coordinate identities to the boundary by continuity. [math:thm-continuous-partial-derivatives-imply-total-differentiability](https://alphabetamath.cc/item/thm-continuous-partial-derivatives-imply-total-differentiability) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F5] The one-variable sum and product rules apply on coordinate lines to differentiable functions. [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)

[F6] For $C^j$ functions with $j\ge2$, coordinate differentiations of total order $j$ can be permuted; hence iterated derivatives can be expressed in the multi-index order used by the norms. [math:thm-symmetry-of-higher-mixed-partials](https://alphabetamath.cc/item/thm-symmetry-of-higher-mixed-partials)

[F7] A real function continuous on a closed interval and differentiable on its interior satisfies the mean value theorem. [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

[F8] Cotangent spaces are the linear duals of tangent spaces. On a smooth manifold with boundary, coordinate derivations form tangent bases also at boundary points, and the cotangent transition maps are the dual inverse matrices of the tangent transition maps. [math:def-cotangent-space-and-cotangent-bundle-as-a-disjoint-union](https://alphabetamath.cc/item/def-cotangent-space-and-cotangent-bundle-as-a-disjoint-union) [math:thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary](https://alphabetamath.cc/item/thm-tangent-and-cotangent-bundles-extend-over-a-manifold-boundary)

## Proof

**Given:** The fixed exterior and chart data, regularity parameters, weights and functions in the Statement.

**Goal:** Prove the global covector derivative estimate, the end-component derivative estimate, and the multiplication and inclusion estimates.

1.1 Put $A=\{1<|y|<2\}$ and $v_R(y)=R^{-\gamma}v(Ry)$. Applying the chain rule to dilation repeatedly gives $\partial_y^I v_R(y)=R^{|I|-\gamma}(\partial_x^I v)(Ry)$. Changing variables in the difference quotient also gives $[\partial_y^I v_R]_{\alpha;A}=R^{|I|+\alpha-\gamma}[\partial_x^I v]_{\alpha;A_R}$. Thus the supremum of the unweighted order-$k$ norms of $v_R$ on $A$ equals $E^{k,\alpha}_\gamma(v)$, up to the fixed finite sum-versus-maximum convention for top derivatives. Each derivative of $\partial_{x^i}v$ appearing in its order-$(k-1)$ norm is a derivative of $v$ of order at most $k$, with precisely the same powers of $R$ after changing the weight to $\gamma-1$. This proves the annular derivative estimate. [F1, F3, F4, F6, given, algebra]

1.2 On any coordinate set $B$, the identity $a(p)b(p)-a(q)b(q)=a(p)(b(p)-b(q))+b(q)(a(p)-a(q))$ gives $[ab]_{\alpha;B}\le\|a\|_{\infty;B}[b]_{\alpha;B}+\|b\|_{\infty;B}[a]_{\alpha;B}$ by division by $|p-q|^\alpha$ and taking suprema. This inequality is proved here directly from the seminorm definition. Repeated use of the one-variable product rule on coordinate lines expands each derivative of $fg$ through order $k$ as a finite sum of products of derivatives of $f$ and $g$ whose orders add to that derivative order. The number and coefficients of the terms depend only on $k$ and the dimension. [F3, F5, F6, algebra]

1.3 For the core product estimate, first control lower-order Hölder seminorms on each fixed compact chart subset $K_i$. When $k\ge1$, cover $K_i$ by finitely many smaller coordinate balls or boundary half-balls whose larger concentric closed balls or half-balls lie inside that chart. On their union $L$, all coordinate derivatives through order $k$ are bounded by $C_\gamma\|f\|_{C^{k,\alpha}_\gamma}$. Indeed, $L\cap K$ is covered by the fixed $K_j$; on each compact overlap the repeated chain and product rules express derivatives in chart $i$ using derivatives in chart $j$ and bounded smooth transition coefficients. On $L\setminus K$, its closure lies in the end with $2r_0\le r\le M$ for some fixed finite $M$, so finitely many bounded-radius annuli give the same control, again with bounded transition coefficients. Continuous transition coefficients are bounded on each of these compact sets: continuity gives local bounds and compactness gives a finite subcover. All constants depend only on the fixed data and weight. A sufficiently close pair of points in $K_i$ lies together in one larger convex ball or half-ball. The chain rule and the mean value theorem along its segment bound increments of each derivative of order less than $k$ by its next derivative supremum times the distance. At boundary points use continuity from the interior. Pairs separated by at least a fixed positive distance are controlled by twice the derivative supremum divided by that distance to the power $\alpha$. Hence every lower-order Hölder seminorm on $K_i$ is at most $C_\gamma\|f\|_{C^{k,\alpha}_\gamma}$. The same reasoning applies to $g$ with weight $\eta$. [F1, F2, F3, F4, F5, F6, F7, given, algebra]

2.1 The fixed annulus $A$ has paths of length at most $(1+\pi)|p-q|$ joining any $p,q\in A$: move radially from the larger radius to the smaller, then along the shorter spherical arc at that smaller radius. The radial length is at most $|p-q|$; the arc length is at most $\pi|p-q|$, since the arc-to-chord ratio is at most $\pi/2$ and the chord at the smaller radius is at most $2|p-q|$. Both pieces stay in $A$. The chain rule and the mean value theorem on each constant-speed path piece therefore bound the increment of a $C^1$ function by a fixed constant times its gradient supremum times $|p-q|$. Applied to derivatives of order less than $k$, this bounds their Hölder seminorms by the order-$k$ norm, since $A$ has finite diameter. The top-order seminorms are already part of that norm. Step 1.2 now gives the order-$k$ product estimate on $A$; for $k=0$ its difference inequality applies directly. Use $f_R=R^{-\gamma}f(R\cdot)$ and $g_R=R^{-\eta}g(R\cdot)$ and step 1.1 to obtain $E^{k,\alpha}_{\gamma+\eta}(fg)\le C E^{k,\alpha}_\gamma(f)E^{k,\alpha}_\eta(g)$. [F1, F3, F4, F7, step 1.1, step 1.2, algebra]

2.2 For $k\ge1$, in a chart $z$ define a linear functional at $p$ by $(df)_p(\sum_i v^i\partial_{z^i}|_p)=\sum_i v^i\partial_{z^i}(f\circ z^{-1})(z(p))$. This defines an element of $T_p^*\Sigma_1$ because the coordinate tangent vectors form a basis, including at boundary points. On overlapping chart interiors, the chain rule gives $\partial_{w^j}(f\circ w^{-1})=\sum_i (\partial_{z^i}(f\circ z^{-1}))\circ(z\circ w^{-1})\,\partial_{w^j}(z^i\circ w^{-1})$. Thus the two coordinate functionals agree by the dual transition law in F8. Continuity of the first derivatives and smooth transition matrices gives the same identity at the boundary. These compatible functionals therefore define a single global covector field $df$ with the asserted coordinate components. In each fixed core chart, every derivative through order $k-1$ of a component of $df$ is a derivative through order $k$ of $f$, and its top-order Hölder seminorm is one already in the order-$k$ core norm. Permuting derivatives is valid under the given $C^k$ regularity. Thus $N_K(df)\le C N_K(f)$ with the respective orders understood. Together with step 1.1 this proves the global derivative estimate, with a well-defined output on the core as well as on the end. [F1, F3, F4, F6, F8, step 1.1, construct, algebra]

3.1 The top-order core seminorms are already controlled by $N_K$. Apply the finite derivative expansion and product difference inequality of step 1.2 on each $K_i$, using step 1.3 for the lower-order seminorms. Sum over the fixed finite chart collection to get $N_K(fg)\le C\|f\|_{C^{k,\alpha}_\gamma}\|g\|_{C^{k,\alpha}_\eta}$. For $k=0$, the core estimate follows immediately from step 1.2 without the lower-order argument. Products have the required local regularity by the same calculation on compact coordinate balls and half-balls. Combining the core bound with step 2.1 proves the global multiplication estimate. [F1, F3, step 1.2, step 2.1, step 1.3, algebra]

4.1 For $\gamma\le\eta$, the annular expression with weight $\eta$ is the one with weight $\gamma$ multiplied by $R^{\gamma-\eta}\le r_0^{\gamma-\eta}$; the core norm is unchanged. This gives the inclusion estimate with $C=\max\{1,r_0^{\gamma-\eta}\}$. Finite component sums and the scalar multiplication estimate control tensor products and contractions with their fixed numerical coefficients. Apply step 1.1 separately to each end component for tensor component differentiation. This proves all the assertions. [F1, step 1.1, step 3.1, step 2.2, algebra] ∎

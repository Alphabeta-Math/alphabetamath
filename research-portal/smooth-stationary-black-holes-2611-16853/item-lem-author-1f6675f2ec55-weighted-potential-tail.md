---
title: Weighted product and uniform potential tails on the full input space
status: published
research_item: lem-author-1f6675f2ec55-weighted-potential-tail
dependency_level: 2
sources:
  references: []
---

## Prerequisites

- [def-weighted-holder-spaces](item-def-weighted-holder-spaces)
- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)
- [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)


## Statement

Use the weighted exterior norms with $0<\alpha<1$ and any real $\beta$. For a fixed $V\in C^{2,\alpha}_{-4}$ and $u\in C^{4,\alpha}_\beta$, multiplication is bounded into $Y_\beta=C^{2,\alpha}_{\beta-2}$. If $\|\cdot\|^*_{k,\alpha;A_R}$ denotes the parenthesized scaled annular norm, then $R^{-(\beta-2)}\|Vu\|^*_{2,\alpha;A_R}\le C R^{-2}\|V\|_{2,\alpha,-4}\|u\|_{4,\alpha,\beta}$. Consequently the target annular norm of the product on annuli with $R\ge T$ is at most $CT^{-2}\|V\|_{2,\alpha,-4}\|u\|_{4,\alpha,\beta}$ for $T\ge r_0$. This assertion does not require $u$ to vanish at the inner boundary.

## Statement references

[def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

## Facts & Assumptions

**Given:** The hypotheses of the Statement.

**Goal:** Establish its stated analytic ingredients and qualifications.

[F1] The weighted norms consist of a compact-core Hölder norm and scaled annular norms with weight $R^{-\beta}$. [def-weighted-holder-spaces](item-def-weighted-holder-spaces) [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F2] For real functions differentiable at a limit point of their common real domain, sums and scalar multiples are differentiable there, and $(fg)'=f'g+fg'$. In particular these rules apply on each open coordinate interval. [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)

[F3] If $f:[a,b]\to\mathbb R$ is continuous on $[a,b]$, differentiable on $(a,b)$ and $a<b$, then $f(b)-f(a)=f'(c)(b-a)$ for some $c\in(a,b)$. Hence $|f(b)-f(a)|\le(b-a)\sup_{(a,b)}|f'|$. [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

## Proof

1.1 Apply [F2] along each coordinate line in the chart interior, first to $V,u$ and then to the terms of their first partial derivatives. Their stated regularity supplies every derivative used through order two. The identities extend to boundary chart points by continuity of these derivatives. To control lower-order Hölder seminorms, apply [F3] to each closed coordinate segment: for a coordinate derivative $q$, its increment is at most the segment length times the supremum of the corresponding first partial derivative of $q$. In the rescaled annulus $\{1<|x|<2\}$, sufficiently close pairs admit coordinate-segment paths in the annulus of total length at most $C|x-y|$. Indeed near either bounding sphere a coordinate with nonzero radial component can first be moved toward the annulus interior, the other coordinates changed, and the first coordinate returned; finitely many such neighborhoods and interior boxes give uniform constants. Separated pairs use $|q(x)-q(y)|\le2\|q\|_\infty$. Rescaling gives $R^{j+\alpha}\max_{|I|=j}[\partial_x^I w]_{\alpha;A_R}\le C(R^j\max_{|I|=j}\|\partial_x^I w\|_\infty+R^{j+1}\max_{|I|=j+1}\|\partial_x^I w\|_\infty)$ whenever these derivatives exist and are bounded. Use this for $w=V$ with $j=0,1$ and for $w=u$ with $j=0,1,2$. The closed-interval continuity and open-interval differentiability required by [F3] follow from the stated regularity. Leibniz differentiation through order two and $[ab]_\alpha\le\|a\|_\infty[b]_\alpha+\|b\|_\infty[a]_\alpha$, obtained by subtracting the two product values, now give $\|Vu\|^*_{2,\alpha;A_R}\le C\|V\|^*_{2,\alpha;A_R}\|u\|^*_{2,\alpha;A_R}$. The two factors are at most $R^{-4}\|V\|_{2,\alpha,-4}$ and $CR^\beta\|u\|_{4,\alpha,\beta}$. Multiplication by $R^{-(\beta-2)}$ leaves $CR^{-2}$, which proves the displayed estimate. [F1, F2, F3, algebra]

2.1 On the compact core, take finitely many small coordinate boxes or boundary half-boxes around the fixed chart subsets, with compact closures inside the corresponding chart domains. Their derivative suprema are controlled by the norms in [F1]: the core is covered by the fixed chart subsets, and any part outside the core is controlled by bounded-radius end annuli; fixed smooth coordinate transitions have bounded derivatives on the relevant compact overlaps. The coordinate comparison can be seen directly from [F3]: telescope a first-order increment along coordinate segments and use continuity of the partial derivatives to obtain the linear term with remainder $o(|h|)$. Substitute the analogous expansion of a smooth transition to obtain the first-order chain formula, and iterate that formula with [F2] to express higher transformed derivatives as finite sums with bounded transition coefficients. Apply [F3] on coordinate segments inside these boxes to derivatives of $V$ of orders zero and one and of $u$ through order two. Interior segments have continuous endpoint values and differentiable interiors; segments in the boundary follow by continuity from interior segments. Close pairs therefore have the required derivative-to-increment bounds, while separated pairs use the derivative suprema. This supplies the lower-order Hölder control needed for the same product calculation as in step 1.1 on each fixed core subset, and bounds the compact-core target norm. Together with the annular estimate it proves boundedness of the multiplication map. Taking the supremum over $R\ge T$ proves the uniform tail estimate. Neither calculation uses a trace of $u$, so both statements hold on the full input space. [F1, F2, F3, step 1.1, algebra] ∎

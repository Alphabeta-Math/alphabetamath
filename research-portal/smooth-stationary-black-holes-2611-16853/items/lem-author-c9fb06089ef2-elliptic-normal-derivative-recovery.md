---
id: lem-author-c9fb06089ef2-elliptic-normal-derivative-recovery
title: Ellipticity recovers every remaining normal derivative
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-normal-graph-and-mean-curvature-data
  - lem-author-c9fb06089ef2-flattened-dirichlet-quasilinear-equation
  - lem-author-c9fb06089ef2-tangential-boundary-schauder-gain
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - math:def-ck-and-multi-index-notation-in-several-variables
  - math:thm-chain-rule-for-total-derivatives
  - math:thm-general-leibniz-rule
  - math:cor-mean-value-theorem
  - math:thm-symmetry-of-higher-mixed-partials
  - math:cor-heine-borel-in-the-product-topology
  - math:thm-compactness-under-continuous-maps
dependency_roles:
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  lem-author-c9fb06089ef2-flattened-dirichlet-quasilinear-equation: mathematical-premise
  lem-author-c9fb06089ef2-tangential-boundary-schauder-gain: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  math:def-ck-and-multi-index-notation-in-several-variables: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:thm-general-leibniz-rule: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
  math:thm-symmetry-of-higher-mixed-partials: mathematical-premise
  math:cor-heine-borel-in-the-product-topology: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 10
---

## Statement

Let $n\ge2$ and $m\ge4$ be integers, let $0<\alpha<1$, and write $Q_R^+=(-R,R)^{n-1}\times(0,R)$ for $R>0$, with flat boundary $x_n=0$. Suppose the real function $w\in C^{m,\alpha}(\overline{Q_R^+})$ is smooth in $Q_R^+$ and solves $A^{ij}(x,w,Dw)w_{ij}+B(x,w,Dw)=0$ there, summing over $1\le i,j\le n$. The coefficients $A^{ij}$ and $B$ are smooth on a neighborhood of the closed first-jet image $\{(x,w(x),Dw(x)):x\in\overline{Q_R^+}\}$, in the local-extension sense at $x_n=0$. Assume $A$ is symmetric and uniformly positive definite on that image: $A^{ij}(x,w,Dw)\xi_i\xi_j\ge\lambda|\xi|^2$ for some $\lambda>0$ and every real vector $\xi$.

Assume the preceding tangential gain is available: every derivative of total order $m+1$ with at most two differentiations in $x_n$ has a $C^{0,\alpha}$ extension to the flat boundary patch. Then every derivative of total order $m+1$ has such an extension on a smaller boundary patch, and $w$ is $C^{m+1,\alpha}$ up to that patch. In particular this applies to the flattened maximal equation when its graph hypotheses, the interior smoothness of $w$ assumed above, and the tangential gain hold. In that application, flow graphs and maximality use the finite-regularity convention specified in F1. No independent boundary data for normal derivatives are imposed.

## Facts & Assumptions

[F1] The equation-solving assumption and the ellipticity bound are explicit hypotheses here. In the graph application, use the flow-graph and future-normal mean-curvature conventions of the graph definition. At the initial finite regularity, $F_w(x)=\phi^Y(w(x),x)$ is required to be a $C^1$ immersion on the full tangent spaces and a homeomorphism onto its image, with positive definite induced metric, including at the boundary. Maximality means that the pullback of the future-normal mean curvature, evaluated by its pointwise second-order graph expression, vanishes. These are admissibility and equation hypotheses; smoothness of $w$ up to the boundary is not assumed. Interior smoothness of $w$ remains a separate hypothesis when applying this lemma to the graph equation; it is not a conclusion of the flattened-equation or tangential-gain supplier. For such a graph with the smooth fixed-boundary data and zero boundary height, the flattened-equation supplier applies at $C^{4,\alpha}$ regularity and gives a smooth quasilinear equation and uniform ellipticity on a smaller compact graph-jet neighborhood. [[def-normal-graph-and-mean-curvature-data]] [[lem-author-c9fb06089ef2-flattened-dirichlet-quasilinear-equation]]

[F2] Under its hypotheses, the tangential-gain supplier gives all total-order $m+1$ derivatives with at most two normal differentiations in $C^{0,\alpha}$ up to a smaller flat patch. That conclusion is assumed here; it is not inferred from $C^{m,\alpha}$ regularity alone. [[lem-author-c9fb06089ef2-tangential-boundary-schauder-gain]]

[F3] The boundary-extension convention for $C^{k,\alpha}$ requires continuous extensions of the interior derivative fields through order $k$, with bounded derivatives and the top-order Hölder seminorm. Coordinate derivatives and multi-indices have their usual $C^k$ meaning. The product, composition and reciprocal estimates needed below are proved in steps 1.1, 2.1 and 3.1, rather than attributed to these definitions. [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]] [[math:def-ck-and-multi-index-notation-in-several-variables]]

[F4] Totally differentiable finite-dimensional compositions obey the chain rule, which may be iterated for the smooth interior functions here. [[math:thm-chain-rule-for-total-derivatives]]

[F5] The one-variable Leibniz rule gives derivatives of a product as finite sums of products of derivatives. Applying it successively in the coordinate directions gives the multi-index product formula used below. [[math:thm-general-leibniz-rule]]

[F6] A real function continuous on a closed interval and differentiable on its interior has endpoint increment equal to its derivative at an interior point times the interval length. [[math:cor-mean-value-theorem]]

[F7] Coordinate differentiations of a smooth function on an open Euclidean set can be permuted without changing its derivatives. We use this in the interior only. [[math:thm-symmetry-of-higher-mixed-partials]]

[F8] Closed bounded finite-dimensional boxes are compact, and continuous real functions on a nonempty compact set attain finite maxima and minima. These facts bound the finitely many coefficient derivatives on the smaller jet box. [[math:cor-heine-borel-in-the-product-topology]] [[math:thm-compactness-under-continuous-maps]]

## Proof

**Given:** The equation, smooth coefficient domain, ellipticity, regularity and tangential-gain hypotheses in the Statement.

**Goal:** Recover all remaining normal derivatives with Hölder extensions and prove the full boundary regularity.

1.1 Work near an arbitrary point of the flat boundary. By continuity of $J(x)=(x,w(x),Dw(x))$ and the smooth local extensions, choose a smaller closed convex coordinate half-box $K$ whose jet image lies in a closed convex box inside the coefficient extension domain. Every coefficient derivative through order $m$ is bounded on this jet box by F8. On $K$, derivatives of $w$ through order $m$ are bounded, and the order-$m$ fields are $\alpha$-Hölder by the hypothesis. For each derivative of order at most $m-1$, apply F6 along successive interior coordinate segments and then pass to their boundary limits: its increment is bounded by a constant times $|x-y|$. On a bounded box, $|x-y|\le(\operatorname{diam}K)^{1-\alpha}|x-y|^\alpha$. Thus all derivatives of $J$ through order $m-1$ are bounded and $\alpha$-Hölder on $K$. Shrink $K$ once more if needed so that F2 holds on it. [F2, F3, F6, F8, given, choose, algebra]

2.1 For bounded $\alpha$-Hölder functions on $K$, direct subtraction gives $[fg]_{0,\alpha}\le\|f\|_\infty[g]_{0,\alpha}+\|g\|_\infty[f]_{0,\alpha}$. If $f\ge\lambda>0$, then $\|1/f\|_\infty\le\lambda^{-1}$ and $[1/f]_{0,\alpha}\le\lambda^{-2}[f]_{0,\alpha}$, since $|1/f(x)-1/f(y)|=|f(x)-f(y)|/|f(x)f(y)|$. Finite sums and finite products therefore preserve $C^{0,\alpha}$. Also, any smooth coefficient derivative through order $m-1$ is Lipschitz on the convex jet box by F6 and the order-$m$ bounds from step 1.1; composing it with the Lipschitz map $J$ gives a bounded $\alpha$-Hölder function on $K$. [F3, F6, step 1.1, algebra]

3.1 Set $a^{ij}(x)=A^{ij}(J(x))$ and $b(x)=B(J(x))$. Repeated chain and coordinate product rules express every interior derivative of these functions through order $m-1$ as a finite sum of terms: a coefficient derivative of order at most $m-1$ evaluated at $J$, multiplied by derivatives of components of $J$ whose total differentiation order is at most $m-1$. Every factor has a bounded $\alpha$-Hölder extension by steps 1.1 and 2.1, so every such term does too. Hence $a^{ij}$ and $b$ belong to $C^{m-1,\alpha}(K)$. In particular $a^{nn}\ge\lambda$ and its reciprocal is bounded and $\alpha$-Hölder by step 2.1. [F1, F3, F4, F5, step 1.1, step 2.1, algebra]

4.1 Fix a multi-index $\beta$ with $|\beta|=m+1$ and $\beta_n=k\ge3$, and put $\gamma=\beta-2e_n$, where $e_n$ is the last coordinate unit multi-index. In the smooth interior, differentiate the assumed equation $|\gamma|=m-1$ times. By F5 and F7, isolating the undifferentiated normal-normal coefficient gives $a^{nn}D^\beta w=-D^\gamma b-\sum_{(i,j)\ne(n,n)}a^{ij}D^\gamma w_{ij}-\sum_{i,j}\sum_{0<\eta\le\gamma}c_{\gamma\eta}(D^\eta a^{ij})(D^{\gamma-\eta}w_{ij})$, with $c_{\gamma\eta}=\prod_{\ell=1}^n\gamma_\ell!/(\eta_\ell!(\gamma_\ell-\eta_\ell)!)$ and componentwise $\eta\le\gamma$. In the last sum, the derivative of $w$ has order $m+1-|\eta|\le m$; $D^\gamma b$ involves derivatives of $w$ of order at most $m$. These terms have bounded $\alpha$-Hölder extensions by steps 1.1, 2.1 and 3.1 and the given regularity. Each derivative in the middle sum has total order $m+1$ and at most $\gamma_n+1=k-1$ normal differentiations. [F1, F3, F5, F7, step 1.1, step 2.1, step 3.1, given, algebra]

5.1 Start with $k\le2$, supplied by F2, and induct on $k$ up to $m+1$. Assuming every total-order $m+1$ derivative with fewer than $k$ normal differentiations has a bounded $\alpha$-Hölder extension to $K$, the middle sum in step 4.1 is controlled by that assumption. All remaining right-hand terms are already controlled independently of the induction. Divide by $a^{nn}\ge\lambda$ using step 2.1 to obtain a bounded $\alpha$-Hölder extension of $D^\beta w$. The formula agrees with the classical derivative in the interior and so defines its boundary values uniquely. There are finitely many derivatives at this fixed order, and the same $K$ suffices for all of them. This proves the claimed control of every order-$m+1$ derivative. [F1, F2, F3, step 2.1, step 3.1, step 4.1, induction, algebra]

6.1 Compatibility with the already continuous order-$m$ derivatives follows directly from F6. Write $v=D^\mu w$ with $|\mu|=m$ and let $g_j$ be the continuous extension of $\partial_jv$ obtained in step 5.1. At a flat-boundary point $x$, apply F6 to the tangential segment from $x+\varepsilon e_n$ to $x+he_j+\varepsilon e_n$, for $j<n$ and $\varepsilon>0$. Subtract $g_j(x)$ from the resulting difference quotient and bound its absolute value by the supremum of $|g_j(y)-g_j(x)|$ over that segment. Let $\varepsilon$ decrease to zero using continuity of $v$, and then let $h$ tend to zero using continuity of $g_j$. The boundary tangential derivative of $v$ is therefore $g_j(x)$. For the inward normal direction, F6 applies directly to $v$ on the closed segment from $x$ to $x+he_n$, since $v$ is continuous at its endpoint and smooth in its interior; the one-sided quotient tends to $g_n(x)$. The order-$m+1$ extensions from step 5.1 and the lower-order extensions in the hypothesis consequently satisfy the boundary-extension convention of F3. Thus $w\in C^{m+1,\alpha}$ on the smaller patch, without prescribing any normal boundary values. [F3, F6, F7, step 5.1, given, algebra] ∎

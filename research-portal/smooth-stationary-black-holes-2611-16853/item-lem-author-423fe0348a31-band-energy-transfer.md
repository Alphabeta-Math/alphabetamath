---
title: Transferring area-controlled band energy through smooth approximation
status: draft
research_item: lem-author-423fe0348a31-band-energy-transfer
dependency_level: 7
---

## Prerequisites

- [lem-author-423fe0348a31-fixed-boundary-approximation](item-lem-author-423fe0348a31-fixed-boundary-approximation)
- [lem-author-423fe0348a31-riemannian-lipschitz-coarea](item-lem-author-423fe0348a31-riemannian-lipschitz-coarea)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:cor-triangle-inequality-for-inner-product-norm](https://alphabetamath.cc/item/cor-triangle-inequality-for-inner-product-norm)


## Statement

Work in ZFC. Let $(R,k)$ be a compact smooth Riemannian three-region with boundary $\partial R=B_-\sqcup B_+$, where the two boundary parts are closed and disjoint. Let $I\subset\mathbb R$ be an interval and let $c_-,c_+\in\mathbb R$ satisfy $c_-<t<c_+$ for every $t\in I$. Let $u:R\to\mathbb R$ be Lipschitz for the intrinsic Riemannian length distance within each connected component. Let $(u_j)$ be any sequence of real Lipschitz functions on $R$ for this distance. Assume that there are fixed open neighborhoods $U_-$ and $U_+$ of the boundary parts on which $u$ and every $u_j$ equal $c_-$ and $c_+$, respectively. The assertion also applies to smooth approximants, where smoothness includes smooth local extension in boundary charts.

Suppose $u_j\to u$ uniformly and in metric $W^{1,1}(R,k)$, meaning that $\int_R(|u_j-u|+|\nabla_k u_j-\nabla_k u|_k)\,dV_k\to0$. Here $dV_k$ is Riemannian volume, $k(\nabla_k v,\cdot)=dv$ defines the almost-everywhere weak gradient, and $\mathcal H_k^2$ is normalized metric two-dimensional Hausdorff measure. Suppose $\mathcal H_k^2(\{x\in R:u(x)=t\})\le A<\infty$ for almost every $t\in I$, with $A\ge0$.

Fix $J=(a,b)$ with $a<b$ and $[a,b]\subset\operatorname{int}I$. Put $e_j=\sup_{x\in R}|u_j(x)-u(x)|$ and $d_j=\int_R|\nabla_k u_j-\nabla_k u|_k\,dV_k$; for empty $R$ the supremum error is zero. For all sufficiently large $j$,
$$\int_J\mathcal H_k^2(\{x\in R:u_j(x)=t\})\,dt\le A(b-a+2e_j)+d_j.$$
In particular,
$$\limsup_{j\to\infty}\frac{1}{b-a}\int_J\mathcal H_k^2(\{x\in R:u_j(x)=t\})\,dt\le A.$$

## Facts & Assumptions

[F1] Boundary-preserving approximation on a compact smooth region uses the intrinsic Lipschitz and metric first-Sobolev conventions in the Statement and supplies smooth sequences with uniform and metric $W^{1,1}$ convergence and the exact constants on fixed boundary neighborhoods. The present estimate is conditional on the stated properties of the sequence and does not infer them for an arbitrary sequence from this existence result. [lem-author-423fe0348a31-fixed-boundary-approximation](item-lem-author-423fe0348a31-fixed-boundary-approximation)

[F2] On a compact smooth Riemannian three-region, a Lipschitz function constant on neighborhoods of both boundary parts, with its constants on opposite sides of $I$, satisfies the coarea identity for every Borel band in $I$, with the gradient, volume and normalized Hausdorff area conventions in the Statement. The supplier also establishes the smooth case, including that a smooth function on compact $R$ is intrinsically Lipschitz by bounding its gradient and integrating along curves. [lem-author-423fe0348a31-riemannian-lipschitz-coarea](item-lem-author-423fe0348a31-riemannian-lipschitz-coarea)

[F3] The norm induced by a real or complex inner product satisfies $|v+w|\le|v|+|w|$. For almost every $x\in R$, apply this to the real inner product $k_x$ on $T_xR$ and to $v=\nabla_k u(x)$ and $w=\nabla_k u_j(x)-\nabla_k u(x)$. [math:cor-triangle-inequality-for-inner-product-norm](https://alphabetamath.cc/item/cor-triangle-inequality-for-inner-product-norm)

[A1] Work in ZFC, including the Axiom of Choice inherited from the approximation and coarea suppliers. It is used when invoking their conclusions, in particular coarea in step 3.1; the band inclusion and norm estimate require no further choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The region, functions, convergence, boundary constants and area hypothesis in the Statement.

**Goal:** Prove the band integral estimate and the upper limit for the average level area.

1.1 Since $[a,b]\subset\operatorname{int}I$ and $I$ is an interval, choose $\delta>0$ with $[a-\delta,b+\delta]\subset I$. Uniform convergence gives $e_j\to0$, so for all sufficiently large $j$ the Borel interval $J_j=(a-e_j,b+e_j)$ is contained in $I$. If $u_j(x)\in J$, then $u(x)\ge u_j(x)-e_j>a-e_j$ and $u(x)\le u_j(x)+e_j<b+e_j$. Thus $\{u_j\in J\}\subset\{u\in J_j\}$, including when $e_j=0$. [given, algebra, choose]

2.1 Apply the inner-product norm triangle inequality [F3] in each tangent space where the weak gradients exist. It gives $|\nabla_k u_j|_k\le|\nabla_k u|_k+|\nabla_k u_j-\nabla_k u|_k$. Integrating on $\{u_j\in J\}$, enlarging the first integration set by step 1.1 and bounding the second integral by its integral over $R$ yields $\int_{\{u_j\in J\}}|\nabla_k u_j|_k\,dV_k\le\int_{\{u\in J_j\}}|\nabla_k u|_k\,dV_k+d_j$. The assumed metric first-Sobolev convergence gives $d_j\to0$. [given, F3, step 1.1, algebra]

3.1 Both $u$ and $u_j$ have the Lipschitz regularity and the exact boundary constants required by [F2]; the boundary parts exhaust $\partial R$ and the constants lie outside $I$ on opposite sides. For smooth approximants the smooth case of [F2] gives the same conclusion. Apply [F2], under [A1], to $u_j$ on the Borel interval $J$ and to $u$ on the Borel interval $J_j$. The resulting identities turn step 2.1 into $\int_J\mathcal H_k^2(\{u_j=t\})\,dt\le\int_{J_j}\mathcal H_k^2(\{u=t\})\,dt+d_j\le A|J_j|+d_j=A(b-a+2e_j)+d_j$. The second inequality uses $J_j\subset I$ and the given almost-everywhere area bound. Divide by $b-a>0$ and use $e_j,d_j\to0$ for the claimed upper limit. No convergence of individual level sets or their areas is asserted. [given, F2, A1, step 1.1, step 2.1, algebra] ∎

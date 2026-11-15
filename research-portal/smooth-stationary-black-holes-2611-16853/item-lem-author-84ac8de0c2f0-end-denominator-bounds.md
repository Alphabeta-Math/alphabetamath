---
title: Mass-one Ernst decay and uniform Harrison denominator bounds
status: draft
research_item: lem-author-84ac8de0c2f0-end-denominator-bounds
dependency_level: 3
---

## Prerequisites

- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-killing-ernst-notation](item-def-killing-ernst-notation)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)
- [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)


## Statement

In the stationary end notation of the declared definitions, assume $T=\partial_t$, $r=|x|>R_0$, and $$g_{00}=-1+2/r+O_6(r^{-2}),\qquad g_{0i}=O_6(r^{-2}),\qquad g_{ij}=\delta_{ij}+O_6(r^{-1}).$$ Suppose the normalized Ernst potential $\sigma=f+i\psi$, $f=-g(T,T)$, is supplied on an open set $U\subseteq M$ containing the designated end, with $\psi\to0$ on that end and the differential equation of the Ernst definition on $U$. Thus $f=-g_{00}$ on the end. Then $\psi=O_6(r^{-2})$ and $\sigma=1-2/r+O_6(r^{-2})$. For $q\in[0,1]$ put $s_q=q+r^{-1}$ and $D_q=|1+q-(1-q)\sigma|^2$. Uniformly for $q\in[0,1]$ on one sufficiently large exterior region, $$D_q=4s_q^2(1+\varepsilon_q),\qquad \varepsilon_q=O_5(r^{-1}),\qquad c s_q^2\le D_q\le C s_q^2$$ for some positive constants $c,C$. For every multi-index $\beta$ with $|\beta|\le5$, $|\partial^\beta s_q^{-1}|\le C_\beta s_q^{-1}r^{-|\beta|}$. If $S$ is the supplied bifurcation surface of the Harrison normalization and the chosen pole $p\in S\cap U$ satisfies $T(p)=0$, then $d_q=D_q(p)=(1+q)^2+(1-q)^2\psi(p)^2$ lies between $1$ and $4+\psi(p)^2$.

## Facts & Assumptions

[F1] The differentiated fixed-chart notation and meaning of parameter uniformity are [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data). The end, its stationary Killing field and its coefficient conventions are [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime). Here the mass coefficient is explicitly one.

[F2] [def-killing-ernst-notation](item-def-killing-ernst-notation) defines $F=\tfrac12dT^\flat$, $f=-g(T,T)$ and the conditional potential, with $\partial_i\psi=T^b\epsilon_{bi\mu\nu}F^{\mu\nu}$ and the metric-dependent index raising and orientation.

[F3] [def-harrison-normalization](item-def-harrison-normalization) defines $D_q$ and $d_q$ by the supplied normalized potential and the supplied pole; it does not assert their positivity.


[F4] On an open Euclidean domain, a real matrix with $C^6$ entries and nowhere-zero determinant has a $C^6$ inverse. [math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity) This applies to the Lorentzian metric matrix on the end and, after increasing its radius, to the spatial block, which tends to the identity.

[F5] The scalar product, quotient and chain rules apply to differentiable functions where denominators do not vanish. [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules) The total chain rule applies to composable differentiable Euclidean maps. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) We use the scalar rules successively along coordinate lines, and the total chain rule for the smooth radial restriction of $\psi$.

[F6] For a $C^1$ real function on an open interval containing finite endpoints $a,b$, the integral of its derivative from $a$ to $b$ equals its endpoint difference. [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts) We apply this on finite radial intervals; the limit at infinity is justified in the proof by the decay bound and the supplied normalization.

## Proof

**Given:** The stated stationary metric, the normalized potential on the supplied open set $U$, and, for the final assertion, the supplied pole $p\in S\cap U$.

**Goal:** Derive the end bounds with one radius and constants independent of $q$.

1.1 The metric matrix tends to the Minkowski matrix, with determinant tending to $-1$, while its spatial block tends to the identity. Apply [F4] also to the identity matrix-valued map on the open set of invertible matrices: inversion is continuous at both limiting matrices, so the inverses are bounded on a sufficiently large end. Their entries as functions of the end coordinates are $C^6$ by [F4]. Differentiating $g^{-1}g=I$ repeatedly, with the finite product rule, gives $g^{ij}=\delta^{ij}+O_6(r^{-1})$, $g^{00}=-1+O_6(r^{-1})$, and $g^{0i}=O_6(r^{-2})$. For the last bound use the block identity $g^{0i}=-g^{00}g_{0j}(g_{\mathrm{sp}}^{-1})^{ji}$; its derivatives have the same order. The volume coefficient is bounded with its corresponding differentiated bounds. Stationarity and [F2] give $F_{ij}=\tfrac12(\partial_i g_{0j}-\partial_jg_{0i})=O_5(r^{-3})$ and $F_{0i}=-\tfrac12\partial_i g_{00}=O_5(r^{-2})$. In $\epsilon_{0i\mu\nu}F^{\mu\nu}$ the indices $\mu,\nu$ are spatial; every $F_{0a}$ contribution to the raised spatial components contains a mixed inverse coefficient $g^{j0}=O_6(r^{-2})$. The remaining terms are $O_5(r^{-3})$. Thus $\partial_i\psi=O_5(r^{-3})$. For a fixed unit vector $\omega$, the smooth real function $h(\rho)=\psi(\rho\omega)$ on $(R_0,\infty)$ has derivative $h^{\prime}(\rho)=\omega^i\partial_i\psi(\rho\omega)$ by [F5]. For finite $R>r$, [F6] gives $\psi(R\omega)-\psi(r\omega)=\int_r^R\omega^i\partial_i\psi(\rho\omega)\,d\rho$. The integrand is bounded in modulus by $C\rho^{-3}$ uniformly in $\omega$, and its tail integral from $R$ to any $R^{\prime}>R$ is at most $C/(2R^2)$. Hence this integral converges as $R\to\infty$; using $\psi(R\omega)\to0$ gives $\psi(r\omega)=-\int_r^\infty\omega^i\partial_i\psi(\rho\omega)\,d\rho=O(r^{-2})$ uniformly in direction. For derivatives of order one through six use the already obtained five derivative bounds on the gradient. This proves the two potential estimates. [F1, F2, F4, F5, F6, given, algebra]

2.1 Spatial derivatives of $r^{-1}$ of order $k$ are bounded by $C_kr^{-1-k}$. Since $s_q\ge r^{-1}$, they are bounded by $C_ks_qr^{-k}$. Induction using derivatives of $s_qs_q^{-1}=1$ yields the stated inverse bound; the same reasoning gives $|\partial^\beta s_q^{-2}|\le C_\beta s_q^{-2}r^{-|\beta|}$. All constants are independent of $q$. In particular $q/s_q$ and $r^{-1}/s_q$, together with derivatives of order $k\le5$, are $O(r^{-k})$ uniformly. Write $\sigma=1-2/r+e$ with $e=O_6(r^{-2})$. Then $$\frac{1+q-(1-q)\sigma}{2s_q}=1-\frac{q}{s_qr}-\frac{(1-q)e}{2s_q}=1+a_q,\qquad a_q=O_5(r^{-1}).$$ This follows by the preceding inverse bounds and $s_q^{-1}\le r$, with finite product differentiation. Hence $D_q/(4s_q^2)=|1+a_q|^2=1+O_5(r^{-1})$. Enlarge the common radius so this last error has absolute value below one half; its reciprocal also has uniform differentiated bounds by repeated differentiation of its product with its inverse. This proves both inequalities. [F1, F3, F5, step 1.1, algebra]

3.1 The supplied pole lies in $U$, so the same smooth potential can be evaluated there. Since $T(p)=0$, $f(p)=-g(T(p),T(p))=0$, so $\sigma(p)=i\psi(p)$. Taking the squared modulus gives the asserted exact expression for $d_q$. For $0\le q\le1$, its first term is between one and four and its second term is between zero and $\psi(p)^2$. These are finite positive bounds independent of $q$. [F2, F3, given, algebra] ∎

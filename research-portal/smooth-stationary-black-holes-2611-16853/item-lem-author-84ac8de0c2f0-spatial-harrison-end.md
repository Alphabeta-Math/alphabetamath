---
title: Uniform spatial components and the cylinder scale
status: published
research_item: lem-author-84ac8de0c2f0-spatial-harrison-end
dependency_level: 7
---

## Prerequisites

- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [lem-author-84ac8de0c2f0-end-denominator-bounds](item-lem-author-84ac8de0c2f0-end-denominator-bounds)
- [lem-author-84ac8de0c2f0-weighted-one-form-decay](item-lem-author-84ac8de0c2f0-weighted-one-form-decay)
- [def-harrison-one-form](item-def-harrison-one-form)
- [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-killing-ernst-notation](item-def-killing-ernst-notation)
- [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules)


## Statement

Use the stationary Lorentzian and normalized Ernst conventions. Let the supplied stationary coordinate end be $(t,x)\in I\times\{x\in\mathbb R^3:r=|x|>R_0\}$, with $T=\partial_t$ and the mass-one bounds
$$g_{00}=-1+2/r+O_6(r^{-2}),\qquad g_{0i}=O_6(r^{-2}),\qquad g_{ij}=\delta_{ij}+O_6(r^{-1}).$$
Suppose a smooth normalized Ernst potential $\sigma=f+i\psi$, $f=-g(T,T)=-g_{00}$ on the end, is supplied on an open set $U$ containing this end. It satisfies $\nabla_a\sigma=2T^b(F+i\star_gF)_{ba}$, with $F_{ab}=\nabla_aT_b$, and $\sigma\to1$ on the designated end (in particular $\psi\to0$). Choose the same supplied pole $p\in U$ with $T(p)=0$ for the Harrison data. For $q\in[0,1]$ set $s_q=q+r^{-1}$, $D_q=|1+q-(1-q)\sigma|^2$ and $d_q=D_q(p)$.

Suppose a smooth real stationary primitive $W_0$ is supplied on this end with $(W_0)_i=O_5(r^{-3})$, and use exactly the family $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. On one sufficiently large common end $V\subseteq U$ the denominator bounds give $D_q>0$ for every $q$. Assume on $V$ these are Harrison one-forms for the same $g,\sigma,p$, satisfying the stationarity and differential conditions of the Harrison definition and $W_q(T)=d_q-D_q$. Use the Harrison metric on $V$ defined from these same forms. These are supplied data, not an existence assertion.

On a sufficiently large common end the spatial coordinate components satisfy
$$(g_q)_{ij}=\frac{D_q}{4}(\delta_{ij}+O_5(r^{-1}))+O_5(r^{-4})=s_q^2(\delta_{ij}+E_{qij}),\qquad E_{qij}=O_5(r^{-1}),$$
uniformly for $q\in[0,1]$. Consequently the coordinate sections $t=\mathrm{constant}$ are spacelike there. For $q=0$ their metric is $r^{-2}(\delta_{ij}+O_5(r^{-1}))$; for fixed $q>0$ it is $q^2\delta_{ij}+O_5(r^{-1})$. The last fixed-parameter remainder need not have constants independent of $q$ at zero.

## Statement references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-killing-ernst-notation](item-def-killing-ernst-notation)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[lem-author-84ac8de0c2f0-end-denominator-bounds](item-lem-author-84ac8de0c2f0-end-denominator-bounds)

[lem-author-84ac8de0c2f0-weighted-one-form-decay](item-lem-author-84ac8de0c2f0-weighted-one-form-decay)

[def-harrison-one-form](item-def-harrison-one-form)

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

## Facts & Assumptions

[F1] [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) supplies the differentiated convention and parameter uniformity. The explicit mass-one metric bounds and the supplied normalized Ernst equation and limit in the Statement meet the end hypotheses of [lem-author-84ac8de0c2f0-end-denominator-bounds](item-lem-author-84ac8de0c2f0-end-denominator-bounds). It supplies $D_q=4s_q^2(1+\varepsilon_q)$, $\varepsilon_q=O_5(r^{-1})$, positive bounds and $|\partial^\beta s_q^{-1}|\le C_\beta s_q^{-1}r^{-|\beta|}$ for $|\beta|\le5$, uniformly on one end.

[F2] The supplied stationary primitive bound $(W_0)_i=O_5(r^{-3})$, the exact lift $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, and $T_i=g_{0i}=O_6(r^{-2})$ meet the conditional hypotheses of [lem-author-84ac8de0c2f0-weighted-one-form-decay](item-lem-author-84ac8de0c2f0-weighted-one-form-decay). Thus $(W_q)_i=s_qZ_{qi}$ with $Z_{qi}=O_5(r^{-2})$ uniformly. The original end also has $f=1+O_6(r^{-1})$ and $g_{ij}=\delta_{ij}+O_6(r^{-1})$. No primitive-existence conclusion is used.

[F3] [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) and [def-killing-ernst-notation](item-def-killing-ernst-notation) fix the metric dual, connection, orientation, smooth time-orientation field $N$ with $g(N,N)<0$, and supplied potential equation used in the Statement. [def-harrison-one-form](item-def-harrison-one-form) defines the Harrison covariant tensor from these same data, with the same pole $p\in U$, on the domains $D_q>0$ and for the supplied forms satisfying its differential, stationary and contraction conditions. Its local justification supplies the Lorentzian metric there and the identity $g_q=(D_q/4)A_q^*g$, where $A_qv=v+D_q^{-1}W_q(v)T$ has smooth inverse $A_q^{-1}v=v-d_q^{-1}W_q(v)T$ and $d_q>0$. Existence of the forms is assumed here.

[F4] In a time-oriented smooth Lorentzian four-manifold, a smooth embedded hypersurface is spacelike when the ambient metric restricts to a positive-definite quadratic form on each tangent space. [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets) (Definition (a)).

[F5] [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules) supplies the scalar sum, product, quotient and chain rules at points of differentiability, with nonzero denominator for a quotient. Apply these rules repeatedly along coordinate lines, holding $q$ fixed. The supplied components are sufficiently differentiable through order five, and the denominators below are positive on the chosen common end.

## Proof

**Given:** The stationary mass-one end, normalized potential, supplied primitive and exact Harrison family in the Statement.

**Goal:** Estimate the spatial block and its signature uniformly.

1.1 By repeated coordinatewise product differentiation in [F5], a derivative of a product is a finite sum of products whose derivative orders add to the total order; hence the decay exponents of differentiated bounds add. Increase the common radius in [F1] so $|\varepsilon_q|\le1/2$. The function $h_q=(1+\varepsilon_q)^{-1}$ is bounded, and differentiating $(1+\varepsilon_q)h_q=1$ successively with [F5] gives $|\partial^\beta h_q|\le C_\beta r^{-|\beta|}$ for $|\beta|\le5$: at each positive order solve for that derivative of $h_q$, using $1+\varepsilon_q\ge1/2$ and the lower-order bounds. Thus $s_q^2/D_q=h_q/4$ has these same uniform bounds. Also $s_q\le2$ for $r\ge1$; differentiating $s_qs_q^{-1}=1$ and using the inverse derivative bounds in [F1] gives $|\partial^\beta s_q|\le C_\beta s_qr^{-|\beta|}$ by the same successive product-rule argument. The spatial block of [F3] is $(g_q)_{ij}=\tfrac14(D_qg_{ij}+g_{0i}(W_q)_j+g_{0j}(W_q)_i-fD_q^{-1}(W_q)_i(W_q)_j)$. By [F2] and the finite product rule, the mixed products are $s_qO_5(r^{-4})=O_5(r^{-4})$. The final product is $f(s_q^2/D_q)Z_{qi}Z_{qj}=O_5(r^{-4})$. This proves the first equality in the Statement. [F1, F2, F3, F5, given, algebra]

2.1 By [F1] and the product rule in [F5], $|\partial^\beta s_q^{-2}|\le C_\beta s_q^{-2}r^{-|\beta|}$. Since $s_q^{-2}\le r^2$, dividing the error $O_5(r^{-4})$ from step 1.1 by $s_q^2$ gives $O_5(r^{-2})$: each derivative of total order $k\le5$ is a finite sum bounded by $Cs_q^{-2}r^{-4-k}\le Cr^{-2-k}$. Meanwhile $D_q/(4s_q^2)=1+O_5(r^{-1})$. The same product rule therefore gives $s_q^{-2}(g_q)_{ij}=\delta_{ij}+E_{qij}$ with $E_{qij}=O_5(r^{-1})$ uniformly. For a large common radius the operator norm of the symmetric error is below one half, so its quadratic form is positive definite. To meet the ambient time-orientation hypothesis in [F4], use the pullback and smooth inverse in [F3] to define $N_q=A_q^{-1}N=N-d_q^{-1}W_q(N)T$ on $V$. This is a smooth vector field, and $g_q(N_q,N_q)=(D_q/4)g(N,N)<0$ since $D_q>0$. Thus $N_q$ time-orients $(V,g_q)$. The coordinate section is a smooth embedded hypersurface with tangent basis $\partial_{x^1},\partial_{x^2},\partial_{x^3}$ and induced metric matrix $((g_q)_{ij})$; hence [F4] proves spacelikeness. At zero parameter put $s_0=r^{-1}$. At any fixed positive parameter use $s_q^2=q^2+2q/r+r^{-2}$, giving the asserted remaining expression. [F1, F3, F4, F5, step 1.1, algebra] ∎

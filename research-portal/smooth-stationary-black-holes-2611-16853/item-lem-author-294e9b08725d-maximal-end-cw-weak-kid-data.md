---
title: Supplied CW logarithmic maximal ends have weak weighted initial data
status: published
research_item: lem-author-294e9b08725d-maximal-end-cw-weak-kid-data
dependency_level: 4
---

## Prerequisites

- [thm-stationary-maximal-slice-existence-input](item-thm-stationary-maximal-slice-existence-input)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Suppose a smooth stationary vacuum end has $g_{00}=-1+2M_0/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$, and $T=\partial_t$. Supply an already existing smooth CW maximal end $t=u(x)$ with its $\alpha=1$ logarithmic graph bounds through at least four derivatives and the corresponding top Holder bound. The original $O_6$ metric bounds supply the selected end's $k=3$, $\alpha=1$ metric and weighted Holder requirements. The declared CW existence input may be used at $k=3$, $\alpha=1$ provided every other end also meets those requirements for a common Holder exponent $0<\lambda<1$, and all remaining class-(b) hypotheses and the exclusion condition hold. The graph and its bounds are supplied hypotheses here; end decay alone does not establish existence.

Here $r=|x|$ in the fixed spatial end chart. For a scalar or finite array of coordinate components $f$, write $f=O_m(r^{-b}(\log r)^p)$, with $m$ a nonnegative integer, $b\in\mathbb R$ and $p\in\mathbb N_0$, when there are a radius $R>1$ and finite constants $C_\beta\geq0$ such that $|\partial^\beta f(x)|\leq C_\beta r^{-b-|\beta|}(\log r)^p$ componentwise for every $|\beta|\leq m$ and $r\geq R$, uniformly in angular directions. Here $\partial^\beta$ denotes Cartesian multi-index differentiation. The case $p=0$ is the differentiated pure-power convention.

Set $\tau=t-u(x)$, so that the SAME maximal hypersurface is $\tau=0$ and $T=\partial_\tau$. Its stationary decomposition is $g=-N^2d\tau^2+h_{ij}(dx^i+X^id\tau)(dx^j+X^jd\tau)$. Then $h-\delta=O_3(r^{-1})+O_3(r^{-2}\log^2r)$, $N\to1$, $X=O_3(r^{-1}\log r)$, and $k=O_2(r^{-2}\log r)$. In the weighted Sobolev convention $\|f\|_{H^s_\eta}^2=\sum_{|I|\le s}\int r^{-2\eta-3+2|I|}|D^If|^2dx$, these imply $h-\delta\in H^3_{-1/2}$ and $k\in H^2_{-5/4}$. These are explicit weak maximal initial-data bounds with weight $\eta=-1/2$ and $\eta/2-1=-5/4$; no improved height or seventh derivative has been assumed. Matching a stationary-source theorem's remaining hypotheses is a separate obligation of its consumer.

## Facts & Assumptions

[F1] Assume the supplied smooth spacelike maximal end graph has the $\alpha=1$ logarithmic differentiated bounds through four derivatives and the top Holder bound in the Statement. Invoking the declared CW existence input with $k=3$, $\alpha=1$ requires its metric and weighted Holder hypotheses on every end for a common exponent $0<\lambda<1$, together with all remaining class-(b) hypotheses and the exclusion condition. The selected end's bounds alone do not establish this global applicability. [thm-stationary-maximal-slice-existence-input](item-thm-stationary-maximal-slice-existence-input)

[F2] The stationary end has T equal to the original time vector, with fixed Lorentzian and Ricci conventions. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F3] The supplied slice is spacelike and maximal and has its future unit normal, induced metric and second form. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F4] The local Sobolev convention uses weak derivatives and square integrability. [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm)

[F5] Differentiated end orders and weighted Holder bounds are measured in the fixed stationary spatial coordinates. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F6] Work in ZFC, including the inherited analytic choice assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The actual end hypotheses in the Statement.

**Goal:** Prove the stated same-slice end consequence.

1.1 On the selected end, the original metric bounds give $D^4(g-\eta)=O(r^{-5})$. Integrating along the segment from $x$ to $y$ with $|x-y|\leq r(x)/2$ gives $|D^3g(x)-D^3g(y)|\leq Cr(x)^{-5}|x-y|\leq C_\lambda r(x)^{-4-\lambda}|x-y|^\lambda$ for $0<\lambda<1$; stationarity removes the time difference. Thus the selected end meets the order-three weighted Holder requirement. The same metric bounds also give its differentiated decay through order three. This calculation does not upgrade any other end; the global invocation in [F1] remains conditional on the stated requirements on every end and all remaining hypotheses. The subsequent estimates use only the supplied graph bounds. The change to tau changes only the time coordinate, with the same stationary vector and the same supplied slice. Its induced metric is $h_{ij}=g_{ij}+g_{0i}u_j+g_{0j}u_i+g_{00}u_iu_j$. The CW bounds give $D^ju=O(r^{-j}\log r)$ for positive j through four. Product differentiation gives the displayed metric bound through three derivatives. Let $A=-g^{-1}(d\tau,d\tau)$. Spacelikeness gives $A>0$ and the metric and slope limits give $A\to1$. Since $d\tau(T)=1$ and $T$ is future timelike on the end, the future unit normal vector is $n=-A^{-1/2}(d\tau)^\sharp$. Hence $n^\flat=-N\,d\tau$ and $N=-g(T,n)=A^{-1/2}\to1$. The mixed components $g_{\tau i}=g_{0i}+g_{00}u_i=h_{ij}X^j$, together with the inverse of $h\to\delta$, give $X=O_3(r^{-1}\log r)$. The covariant second-form expression contains the graph Hessian plus metric first derivatives and lower slope products, giving the stated k bound through two derivatives. [F1, F2, F3, F5, given, algebra]

2.1 For the metric bound, inserting each derivative order into the H3 norm at eta=-1/2 gives an integrable radial majorant proportional to $r^{-2}$, with still faster log-weighted corrections. For k at eta=-5/4 the radial majorant is proportional to $r^{-5/2}\log^2r$, also integrable. Compact inner annuli cause no issue because all supplied fields are smooth there. These are properties of the already supplied maximal hypersurface, not a choice of a new maximal end. For the explicit initial-data weight $\eta=-1/2$, the second-form weight is $\eta/2-1=-5/4$, as stated. No source theorem is invoked for this integration calculation; matching a consumer's other hypotheses is left to that consumer. [F1, F2, F3, F4, F5, step 1.1, algebra] ∎

---
title: Stationarity supplies the weighted end differentiability estimates
status: published
research_item: lem-author-45355d85383b-weighted-end-superposition
dependency_level: 8
---

## Prerequisites

- [lem-author-45355d85383b-stationary-parameter-residual](item-lem-author-45355d85383b-stationary-parameter-residual)
- [lem-author-45355d85383b-weighted-products-and-derivatives](item-lem-author-45355d85383b-weighted-products-and-derivatives)
- [lem-author-45355d85383b-weighted-smooth-inversion](item-lem-author-45355d85383b-weighted-smooth-inversion)
- [lem-author-45355d85383b-smooth-mean-curvature-jet](item-lem-author-45355d85383b-smooth-mean-curvature-jet)
- [lem-author-45355d85383b-relative-timelike-flow-chart](item-lem-author-45355d85383b-relative-timelike-flow-chart)
- [lem-author-45355d85383b-weighted-fifth-graph-derivative](item-lem-author-45355d85383b-weighted-fifth-graph-derivative)
- [def-weighted-holder-spaces](item-def-weighted-holder-spaces)
- [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:lem-taylor-integral-remainder](https://alphabetamath.cc/item/lem-taylor-integral-remainder)



## Statement

Work in ZFC. Fix $0<\alpha<1$, a smooth embedded three-dimensional exterior $\Sigma$ with compact smooth boundary, and the fixed compact-chart and end-coordinate data for its weighted Hölder spaces. Let $q_*\in I\subset\mathbb R$, with $I$ open, and let $(g_q,N_q,T)$ be stationary Lorentzian data on a common neighborhood of $\Sigma$, jointly smooth in the parameter and ambient coordinates, with a common stationary field $T$ and smoothly varying time orientation. Assume $\Sigma$ is spacelike and maximal for $g_{q_*}$.

Supply a common stationary product end $\Psi:\mathbb R_t\times\{r=|x|>R_0\}\to U$, with $T=\Psi_*\partial_t$ future timelike for every $q$ and $\Sigma\cap U=\{\Psi(u_*(x),x):r>R_0\}$. The product spatial chart agrees with the fixed end chart of $\Sigma$, whose complement is compact. The metric coefficients in these fixed coordinates are independent of $t$ and satisfy $g_{q,00}=-c(q)^2+e_{q,00}$, $g_{q,ij}=b(q)^2\delta_{ij}+e_{q,ij}$ and $g_{q,0i}=e_{q,0i}$, where $b,c$ are smooth and positive. On a closed interval $J\subset I$ with $q_*$ in its interior, the errors and their first parameter derivatives have common differentiated bounds $e_{q,00},e_{q,ij}=O_5(r^{-1})$ and $e_{q,0i}=O_5(r^{-2})$. In addition, $q\mapsto(e_{q,00},e_{q,ij})$ is $C^1$ in the annular $C^{4,\alpha}_{-1}$ norm and $q\mapsto e_{q,0i}$ is $C^1$ in the annular $C^{4,\alpha}_{-2}$ norm. These are parameter-uniform end assumptions, not conclusions from joint smoothness on compact sets. Assume the fixed smooth reference height has $u_*\in C^{5,\alpha}_{-3/4}$ and $\Delta_0u_*\in C^{2,\alpha}_{-3}$ on the end, where $\Delta_0=\sum_{i=1}^3\partial_{x^i}^2$.

Choose the fixed transverse field supplied by the timelike-flow construction, so $Y=T$ on a sufficiently distant tail $E$. For $w\in C^{4,\alpha}_\beta(\Sigma)$, the end flow graph is exactly $F_w(x)=\Psi(u_*(x)+w(x),x)$. Let $\mathcal H_E(q,w)$ be the future mean curvature of this graph, pulled back by $F_w$. For every $-1<\beta<0$, after shrinking the parameter interval about $q_*$ and choosing a sufficiently small norm ball in $C^{4,\alpha}_\beta$, this end map is $C^1$ with values in $C^{2,\alpha}_{\beta-2}(E)$. Here the target uses the annular part of the weighted norm on the tail; a fixed compact end collar may also be included. The Fréchet derivative is bounded and continuous in operator norm, with the estimates and continuity modulus uniform over all exterior annuli. This assertion includes the restriction to the zero-boundary-height subspace, where the timelike-flow construction supplies globally embedded fixed-boundary graphs. No boundary condition is needed to define the end map on the full ball. The end expression has no undifferentiated height dependence because the flow is stationary time translation; this is essential to the stated weight estimate.

## Statement references

[lem-author-45355d85383b-stationary-parameter-residual](item-lem-author-45355d85383b-stationary-parameter-residual)

[lem-author-45355d85383b-weighted-products-and-derivatives](item-lem-author-45355d85383b-weighted-products-and-derivatives)

[lem-author-45355d85383b-weighted-smooth-inversion](item-lem-author-45355d85383b-weighted-smooth-inversion)

[lem-author-45355d85383b-smooth-mean-curvature-jet](item-lem-author-45355d85383b-smooth-mean-curvature-jet)

[lem-author-45355d85383b-relative-timelike-flow-chart](item-lem-author-45355d85383b-relative-timelike-flow-chart)

[lem-author-45355d85383b-weighted-fifth-graph-derivative](item-lem-author-45355d85383b-weighted-fifth-graph-derivative)

[def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:lem-taylor-integral-remainder](https://alphabetamath.cc/item/lem-taylor-integral-remainder)

## Facts & Assumptions

[F1] The reference residual $h(q)=\mathcal H_E(q,0)$ is $C^1$ in $C^{2,\alpha}_{-3}$ under the stated stationary metric and reference-graph bounds, and $h(q_*)=0$. [lem-author-45355d85383b-stationary-parameter-residual](item-lem-author-45355d85383b-stationary-parameter-residual)

[F2] Weighted end differentiation lowers the weight by one; multiplication adds weights, and a smaller weight includes continuously into a larger one. The estimates hold for finite component arrays and contractions. [lem-author-45355d85383b-weighted-products-and-derivatives](item-lem-author-45355d85383b-weighted-products-and-derivatives)

[F3] Smooth finite-dimensional coefficient composition on bounded ranges with a positive distance from the inadmissible set is $C^1$ in the zero-weight Hölder norm, uniformly over annuli; multiplication by those coefficients is bounded on each weight. [lem-author-45355d85383b-weighted-smooth-inversion](item-lem-author-45355d85383b-weighted-smooth-inversion)

[F4] The smooth spacelike-jet formula for mean curvature is quasilinear in second derivatives. Its Proof 1.1 and 2.1 gives the normal algebraically from the metric and graph slope; differentiating the normal gives terms linear in the graph Hessian and in first metric derivatives. The same formula applies to admissible $C^{4,\alpha}$ graphs. [lem-author-45355d85383b-smooth-mean-curvature-jet](item-lem-author-45355d85383b-smooth-mean-curvature-jet)

[F5] For a supplied stationary product end, bounded ambient components, bounded reference slope and a common positive lower bound for the induced metric, the timelike-flow construction supplies a fixed $Y$, equal to $T$ on a tail, and a parameter-uniform admissible zero-trace graph neighborhood. Its normalization here is $T=\Psi_*\partial_t$. [lem-author-45355d85383b-relative-timelike-flow-chart](item-lem-author-45355d85383b-relative-timelike-flow-chart)

[F6] The reference-graph bootstrap supplies $u_*\in C^{5,\alpha}_{-3/4}$ and $\Delta_0u_*\in C^{2,\alpha}_{-3}$ under its stationary maximal-graph hypotheses. These two reference bounds are explicit data here; no new bootstrap is inferred from stationarity alone. [lem-author-45355d85383b-weighted-fifth-graph-derivative](item-lem-author-45355d85383b-weighted-fifth-graph-derivative)

[F7] The fixed weighted Hölder spaces use a compact-core norm and scaled annular norms; on $x=Ry$ a weight-$\gamma$ component is measured by $R^{-\gamma}f(Ry)$ in the fixed annulus. End norms below mean the annular part of this definition. [def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[F8] The flow graph and its pulled-back mean curvature use the future unit normal and the positive-sign second fundamental form. The stationary end is defined by $\mathcal L_Tg_q=0$ together with the supplied future-timelike end condition; neither a product end nor its uniform bounds follows from that condition alone. [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F9] Differentiated $O_5$ bounds, annular Hölder bounds and parameter uniformity refer to the same fixed Cartesian end chart and common constants. The parameter-norm continuity assumptions in the Statement are additional explicit data. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F10] ZFC includes the Axiom of Choice, assumed when invoking the timelike-flow construction and its partition-of-unity input in step 1.1. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F11] For a smooth finite-dimensional function along a segment inside its domain, the order-zero Taylor integral formula expresses its increment as the integral of its derivative along that segment, componentwise. Applied to the slope variables, it gives the smooth divided differences in step 4.1. [math:lem-taylor-integral-remainder](https://alphabetamath.cc/item/lem-taylor-integral-remainder)

## Proof

**Given:** The fixed exterior, jointly smooth stationary family, uniform end bounds, reference graph and regularity parameters in the Statement.

**Goal:** Prove the stated end mapping property and uniform continuous Fréchet differentiability.

1.1 Shrink $J$ about $q_*$ so positivity and continuity of $b,c$ bound them above and away from zero. The common decay bounds and $Du_*=O(r^{-7/4})$ give, on a sufficiently distant common tail, bounded ambient components and $h_{q,ij}=b(q)^2\delta_{ij}+O(r^{-1})$ for the reference graph. Thus $h_q\ge m I$ for a common $m>0$. The hypotheses of [F5] hold there and on the compact part after shrinking the parameter interval about $q_*$. Fix its $Y$ and increase the tail radius until $Y=T$. On this tail every height graph has unchanged spatial coordinates and is an embedding in the supplied product, whether or not its boundary trace vanishes. The exact induced-metric formula in [F5] preserves $h_{q,w}\ge(m/2)I$ for uniformly small $|Dw|$, controlled by the weighted norm since $\beta<0$. The metric arrays, their inverses and all slopes $Du_*+Dw$ consequently lie in bounded ranges uniformly separated from degenerate metrics and null graph conormals. This supplies the common admissible coefficient range; it is not inferred from compact-core coefficient bounds. [given, F2, F5, F6, F7, F8, F9, F10, algebra]

2.1 In the stationary coordinates write $s=Du_*+Dw$ and $s_*=Du_*$. Applying [F4] directly to the graph $t=u_*+w$ gives $\mathcal H_E(q,w)=A^{ij}(g_q,s)(u_{*,ij}+w_{ij})+B(g_q,\partial_xg_q,s)$. Here $A$ is a smooth function of the metric array and slope on the range from step 1.1, and $B$ is a finite sum of a first spatial metric derivative times a smooth function of that array and slope. Indeed the conormal is $dt-s_i dx^i$; its normalized metric dual depends algebraically only on $(g_q,s)$, and its tangential derivative consists of terms linear in $\partial_xg_q$ and in $D^2(u_*+w)$. The connection terms are also linear in $\partial_xg_q$. Stationarity removes time derivatives of the metric and every dependence on the value of $u_*+w$. All signs are fixed by [F8]. [given, F4, F8, step 1.1, algebra]

3.1 Regard all the following coefficients as $C^{2,\alpha}$ arrays on the end. The metric array is a $C^1$ function of $q$ into weight zero, while $\partial_xg_q$ is $C^1$ into weight $-2$, because its spatially constant leading terms differentiate to zero. Also $s_*\in C^{2,\alpha}_{-7/4}$ and $D^2u_*\in C^{2,\alpha}_{-11/4}\subset C^{2,\alpha}_{-2}$. The maps $w\mapsto Dw$ and $w\mapsto D^2w$ are bounded into weights $\beta-1$ and $\beta-2$, respectively, and these include into the zero-weight space. By [F3] on the common range in step 1.1, $A(q,w)=A(g_q,s_*+Dw)$ is $C^1$ with values in weight zero. Every smooth coefficient multiplying $\partial_xg_q$ in $B$ has the same property, as do its finite slope derivatives. The statements include full finite-norm Hölder inputs, not just smooth perturbations. [given, F2, F3, F6, F7, F9, step 1.1, step 2.1, algebra]

4.1 Subtract the reference expression from step 2.1. Smooth finite-dimensional divided differences give $A(g,s_*+v)-A(g,s_*)=A_1(g,s_*,v)v$ and $B(g,d,s_*+v)-B(g,d,s_*)=B_1(g,d,s_*,v)v$, where $A_1$ and $B_1$ are smooth on a slightly smaller common range, and $B_1$ is linear in $d$. For example these divided differences are the componentwise integrals of the slope derivatives from slope $s_*$ to slope $s_*+v$; the slope segment remains admissible by the small-slope bounds of step 1.1. Consequently $\mathcal H_E(q,w)=h(q)+A^{ij}(q,w)w_{ij}+C^j(q,w)w_j$, where $C$ is obtained by contracting $A_1(g_q,s_*,Dw)$ with $D^2u_*$ and adding $B_1(g_q,\partial_xg_q,s_*,Dw)$. Step 3.1 and [F2]–[F3] show that $C(q,w)$ is $C^1$ with values in weight $-2$. Their finite-dimensional smoothness follows by differentiating the integrands on a slightly smaller coefficient range: continuity of each derivative on the compact integration interval gives uniform convergence of the corresponding difference quotients, as in [F3], Proof 4.1. No integration in a function space is assumed. [F2, F3, F4, F11, step 1.1, step 2.1, step 3.1, algebra]

5.1 The product $A(q,w):D^2w$ is $C^1$ into weight $\beta-2$ by the bounded bilinear multiplication and composition rules of [F2]–[F3]. The product $C(q,w)\cdot Dw$ is $C^1$ into weight $\beta-3$, which includes continuously into weight $\beta-2$. Finally $h(q)$ is $C^1$ into weight $-3$ by [F1], and $-3<\beta-2$ because $\beta>-1$. Their sum is the asserted $C^1$ map on a product neighborhood, hence on a small ball about $(q_*,0)$. Explicitly its height derivative is $D_w\mathcal H_E(q,w)v=A(q,w):D^2v+C(q,w)\cdot Dv+(D_wA(q,w)v):D^2w+(D_wC(q,w)v)\cdot Dw$; its parameter derivative is $h'(q)+(\partial_qA(q,w)):D^2w+(\partial_qC(q,w))\cdot Dw$. The displayed products prove boundedness in the target norm. [F1, F2, F3, step 3.1, step 4.1, algebra]

6.1 The remainder and derivative-continuity estimates in [F3] use one common coefficient range from step 1.1, the parameter continuity in the assumed weighted norms, and the bounded linear and bilinear operations in steps 3.1–4.1. They therefore have a single modulus tending to zero in the sum norm $|\delta q|+\|\delta w\|_{C^{4,\alpha}_\beta}$, before taking the supremum over exterior annuli. The bounded product rules preserve that modulus in the two displayed derivative formulas, proving operator-norm continuity and a uniform Fréchet remainder. Equivalently, on $x=Ry$ the normalized perturbation $\eta=R^{-\beta}w(Ry)$ has physical slope $R^{\beta-1}D\eta$ and Hessian $R^{\beta-2}D^2\eta$; the $C\cdot Dw$ term has an extra bounded factor $R^{-1}$ in the normalized target, and no term arises from undifferentiated height. On any fixed end collar the same smooth coefficient formulas and [F2]–[F4] give the ordinary $C^{4,\alpha}$ to $C^{2,\alpha}$ estimate, so that collar can be included. Restriction to the closed zero-trace subspace preserves continuous differentiability and agrees with the global admissible graphs in [F5]. This proves all the asserted end estimates. [F2, F3, F4, F5, F7, step 1.1, step 2.1, step 3.1, step 4.1, step 5.1, algebra] ∎

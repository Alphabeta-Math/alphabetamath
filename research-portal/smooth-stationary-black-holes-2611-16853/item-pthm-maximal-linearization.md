---
title: Mean-curvature linearization, weighted regularity and fixed-boundary graph map
status: published
research_item: pthm-maximal-linearization
dependency_level: 11
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp.12–13, (3.1)–(3.2), §3.1 openness, Jacobi display and following
        regularity assertion
      reading_limits: Freshly read frozen article text pp.12–13 and inspected the PDF
        page13 image for attribution. Current supplier statements and the
        general residual argument were separately inspected. The article is not
        used to prove its generated prerequisites. No source-proof audit or
        independent acceptance is claimed.
---

PDF p. 13: ` §3.1, continuation at q* `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)
- [pthm-transformed-end-geometries](item-pthm-transformed-end-geometries)
- [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)
- [def-harrison-electromagnetic-form](item-def-harrison-electromagnetic-form)
- [def-killing-ernst-notation](item-def-killing-ernst-notation)
- [def-harrison-one-form-family](item-def-harrison-one-form-family)
- [def-harrison-normalization](item-def-harrison-normalization)
- [pthm-electrovacuum-energy-conditions](item-pthm-electrovacuum-energy-conditions)
- [lem-author-45355d85383b-scaled-decay-holder-upgrade](item-lem-author-45355d85383b-scaled-decay-holder-upgrade)
- [lem-author-45355d85383b-weighted-fifth-graph-derivative](item-lem-author-45355d85383b-weighted-fifth-graph-derivative)
- [lem-author-45355d85383b-induced-metric-and-normal-decay](item-lem-author-45355d85383b-induced-metric-and-normal-decay)
- [lem-author-45355d85383b-second-form-and-jacobi-potential](item-lem-author-45355d85383b-second-form-and-jacobi-potential)
- [lem-author-45355d85383b-positive-lapse-multiplier](item-lem-author-45355d85383b-positive-lapse-multiplier)
- [lem-author-45355d85383b-relative-timelike-flow-chart](item-lem-author-45355d85383b-relative-timelike-flow-chart)
- [lem-author-45355d85383b-stationary-parameter-residual](item-lem-author-45355d85383b-stationary-parameter-residual)
- [lem-author-45355d85383b-global-dirichlet-mean-curvature-map](item-lem-author-45355d85383b-global-dirichlet-mean-curvature-map)
- [def-weighted-holder-spaces](item-def-weighted-holder-spaces)
- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [thm-maximal-jacobi-lapse-input](item-thm-maximal-jacobi-lapse-input)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [def-harrison-one-form](item-def-harrison-one-form)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)



## Statement

Adopt the regular mass-one stationary vacuum construction, original maximal section, $T|_S\not\equiv0$ and its smooth Harrison metrics. Fix $q_*>\delta>0$ with $q_*\le1$ for which a smooth spacelike maximal slice $\Sigma_*$ with compact smooth boundary $S$ already exists. Its end is the stationary graph $t_{q_*}=\widetilde u_*(x_{q_*})$, with the pointwise estimates $|D^j\widetilde u_*|\le C r_{q_*}^{-3/4-j}$ for $0\le j\le4$. This existence and these pointwise estimates are hypotheses, not conclusions of the present item.

Fix an arbitrary Hölder exponent $\alpha$ with $0<\alpha<1$ throughout.

Choose a smooth future timelike transverse field $Y$ equal to $n_*$ near the compact core and equal to $T$ far out. Let $h_*,k_*,n_*$ be the induced metric, second fundamental form and future unit normal, $a_*=-g_{q_*}(Y,n_*)$, and $V_*=|k_*|_{h_*}^2+\operatorname{Ric}(g_{q_*})(n_*,n_*)$. Then $a_*>0$ has a positive lower bound, equals one near $S$, and has positive limit $d_{q_*}/(4q_*)$ on the normalized end. In the fixed original coordinates,
$$q_*^{-2}h_*-\delta\in C^{3,\alpha}_{-1},\qquad V_*\in C^{2,\alpha}_{-4},\qquad V_*\ge0.$$
These Hölder assertions follow from the maximal equation and the differentiated background, rather than from pointwise fourth derivatives alone.

For each $-1<\beta<0$, put $X_\beta=\{w\in C^{4,\alpha}_\beta:w|_S=0\}$ and $Y_\beta=C^{2,\alpha}_{\beta-2}$. They are Banach spaces; multiplication by $a_*$ is a bounded isomorphism of $X_\beta$. In a small admissible flow-chart neighborhood the pulled-back mean-curvature map is $C^1$ in $(q,w)$ with values in $Y_\beta$, and at $(q_*,0)$,
$$D_w\mathcal H(q_*,0)w=(\Delta_{h_*}-V_*)(a_*w)=q_*^{-2}(\Delta_{q_*^{-2}h_*}-q_*^2V_*)(a_*w).$$
In particular the statement applies at $\beta=-3/4$. The graph boundary remains pointwise S. The auxiliary Y is neither the axial generator nor T near S, where T is tangent to S. Any smooth metric extension of the parameter interval used at q*=1 is only for this analytic map; no electrovacuum claim beyond the physical parameter interval is made.

The original-section maximality used here is assumed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$, with the original metric $g$, so $H_g|_C=0$. The selected physical end retains its stated mass-one normalization. Maximality of an independently labelled chart-side section or another supplied maximal section does not replace this premise. No equality between the hypersurface identification and the physical stationary end chart is assumed. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

## Facts & Assumptions

[F1] Adopt the stationary vacuum Einstein model, with its stated normalization. [post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[F2] The original stationary end has the differentiated order-six background bounds, smooth bifurcation sphere and supplied geometric regularity. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F3] The existing candidate is a stationary maximal graph on the end and a separately supplied smooth spacelike hypersurface with boundary S. [def-stationary-maximal-graph](item-def-stationary-maximal-graph)

[F4] The Harrison metrics and fields satisfy the geometric electrovacuum equations on the exterior and a common smooth neighborhood of S; the metric is jointly smooth in q. [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)

[F5] The normalized positive-q end has spatial and time errors of order minus one and mixed error of order minus two through five derivatives. [pthm-transformed-end-geometries](item-pthm-transformed-end-geometries)

[F6] Under the standing regular mass-one vacuum, original maximal-section and $T|_S\not\equiv0$ hypotheses, the global one-form construction supplies the single smooth stationary primitive used in [F4], with $(W_0)_i=O_5(r^{-3})$ in the unchanged original end chart and $W_0(T)=d_0-D_0$. Its smooth end gauge need not equal the exact radial integral. [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)

[F7] The transformed electromagnetic form is the explicit rank-one pullback and scalar multiple of the original complex Killing form; bounds for its factors are proved below. [def-harrison-electromagnetic-form](item-def-harrison-electromagnetic-form)

[F8] The original Killing two-form, Hodge convention and Ernst differential have the specified meanings. [def-killing-ernst-notation](item-def-killing-ernst-notation)

[F9] The one-form family has polynomial q dependence and the supplied stationary primitive and normalization. [def-harrison-one-form-family](item-def-harrison-one-form-family)

[F10] The pole normalization is $d_q=D_q(p)$ with $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $\sigma=f+i\psi$, $f=-g(T,T)$. At the supplied pole $T_p=0$, it satisfies $d_q=(1+q)^2+(1-q)^2\psi(p)^2>0$ for $q>0$. The stationary-graph coordinates use $t_q=d_qt/(4q)$ and $T=\partial_t$. [def-harrison-normalization](item-def-harrison-normalization) [def-stationary-maximal-graph](item-def-stationary-maximal-graph)

[F11] Timelike Ricci convergence and the nonnegative squared second form make the Jacobi potential nonnegative. [pthm-electrovacuum-energy-conditions](item-pthm-electrovacuum-energy-conditions)

[F12] One extra pointwise derivative supplies the scaled Hölder control needed for the smooth stationary background. [lem-author-45355d85383b-scaled-decay-holder-upgrade](item-lem-author-45355d85383b-scaled-decay-holder-upgrade)

[F13] The maximal graph equation upgrades the displayed pointwise order-four decay to weighted C5-alpha and controls its Euclidean Laplacian. [lem-author-45355d85383b-weighted-fifth-graph-derivative](item-lem-author-45355d85383b-weighted-fifth-graph-derivative)

[F14] The induced metric and graph normal have the weighted decay and derivative counts needed below. [lem-author-45355d85383b-induced-metric-and-normal-decay](item-lem-author-45355d85383b-induced-metric-and-normal-decay)

[F15] The differentiated second form and quadratic electromagnetic Ricci term give the weighted order-minus-four potential. [lem-author-45355d85383b-second-form-and-jacobi-potential](item-lem-author-45355d85383b-second-form-and-jacobi-potential)

[F16] The positive transverse lapse and its inverse are bounded weighted C4-alpha multipliers preserving zero trace. [lem-author-45355d85383b-positive-lapse-multiplier](item-lem-author-45355d85383b-positive-lapse-multiplier)

[F17] A smooth future timelike transverse flow graph chart fixes S and has an open admissible weighted neighborhood. [lem-author-45355d85383b-relative-timelike-flow-chart](item-lem-author-45355d85383b-relative-timelike-flow-chart)

[F18] For a jointly smooth stationary family satisfying its explicit mixed end bounds and weighted parameter-norm conditions, the reference-slice residual is C1 in the parameter and has weighted order minus three. Common bounds through two parameter derivatives suffice for those norm conditions. [lem-author-45355d85383b-stationary-parameter-residual](item-lem-author-45355d85383b-stationary-parameter-residual)

[F19] The global Dirichlet mean-curvature map is C1 with the Jacobi derivative. [lem-author-45355d85383b-global-dirichlet-mean-curvature-map](item-lem-author-45355d85383b-global-dirichlet-mean-curvature-map)

[F20] All weighted spaces use the fixed original end chart and fixed compact boundary charts. [def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[F21] The domain has zero continuous boundary trace and the target has weight beta minus two. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F22] The sign convention gives the derivative Delta_h minus the nonnegative Jacobi potential on the normal speed. [thm-maximal-jacobi-lapse-input](item-thm-maximal-jacobi-lapse-input)

[F23] Work in ZFC, carrying the analytic suppliers' choice assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F24] The Harrison metric is $g_q=(D_q/4)A_q^*g$, with $A_qv=v+D_q^{-1}W_q(v)T$ and $W_q(T)=d_q-D_q$; the inverse rank-one map is $v\mapsto v-d_q^{-1}W_q(v)T$. [def-harrison-one-form](item-def-harrison-one-form)

## Proof

**Given:** The existing-slice and construction hypotheses in the Statement.

**Goal:** Prove the displayed regularity, multiplier, C1 and linearization assertions.

1.1 The standing model, original maximal section, mass-one normalization and $T|_S\not\equiv0$ are exactly the hypotheses of [F6]. Use its single smooth stationary $W_0$, the same choice specified in [F4], with its normalized contraction and original-chart spatial bound; no equality with a radial integral is used. The original stationary order-six bounds in [F2] and Killing equation in [F8] give $F_{ab}=\tfrac12(\partial_ag_{b0}-\partial_bg_{a0})=O_5(r^{-2})$. The Hodge coefficients, expressed using the inverse metric and volume density, are bounded through six spatial derivatives, with positive-order derivatives of the asymptotically constant coefficients gaining the corresponding powers of $r^{-1}$. Hence $\mathcal F=F+i\star_gF=O_5(r^{-2})$. By [F8], $d\sigma=2\iota_T\mathcal F$ and $\sigma\to1$. Integrating its radial derivative from $r$ to infinity gives $\sigma-1=O(r^{-1})$; its positive-order derivatives through order six are those of $d\sigma$, so $\sigma-1=O_6(r^{-1})$. Thus, writing $B_q=2q+(1-q)(1-\sigma)$, on every fixed compact positive-parameter interval $J$ one has $D_q=|B_q|^2=4q^2+O_5(r^{-1})$, with common constants also after either of the first two parameter derivatives. On a sufficiently distant common end $D_q$ is bounded away from zero. The family and contraction in [F9] give $(W_q)_i=(1-q)^2(W_0)_i-4q(1-q)g_{0i}=O_5(r^{-2})$ and $(W_q)_0=d_q-D_q$. Consequently the components of $A_q$ and the scalar $\overline B_q/B_q$ are bounded through three spatial derivatives, with each positive derivative of order $j$ bounded by $Cr^{-j}$: differentiate these finite products and reciprocals using the lower bound for $D_q$ and the polynomial formula for $d_q$ in [F10]. The pullback formula in [F7] now yields $F_{q_*}=O_3(r^{-2})$. The constant coordinate changes in [F3] preserve these orders, giving $F_{q_*}=O_3(r_{q_*}^{-2})$, and [F12] gives $F_{q_*}\in C^{2,\alpha}_{-2}$. No parameter derivative of the electromagnetic square-root factor is used. [F1, F2, F3, F4, F6, F7, F8, F9, F10, F12, F23, F24, given, algebra]

2.1 The additional positive-parameter conclusion in [F5] applies to the same smooth global primitive from [F6]: the regular model, original maximality, mass-one normalization and $T|_S\not\equiv0$ are the standing hypotheses. Apply [F13] to the existing maximal end graph using the background bounds in [F5]. It gives the missing weighted Hölder control and one further graph derivative. [F14] yields the induced metric and normal estimates; [F15], using step 1.1 and the electrovacuum equations in [F4], gives the potential in $C^{2,\alpha}_{-4}$. Smoothness on the supplied compact part supplies its finite local norms. By [F11], the potential is nonnegative. Constant coordinate scaling gives the displayed $q_*^{-2}h_*$ estimate in the fixed original chart. [F3, F4, F5, F6, F11, F13, F14, F15, F20, step 1.1]

2.2 Verify the general stationary-family hypotheses of [F18] for this actual smooth primitive. Put $v_i=(W_q)_i$. Expanding [F24] and substituting $(W_q)_0=d_q-D_q$ from [F9] gives in the fixed original chart $$(g_q)_{00}=-\frac{f d_q^2}{4D_q},\qquad (g_q)_{0i}=\frac{d_q}{4}\left(g_{0i}-\frac{f v_i}{D_q}\right),\qquad (g_q)_{ij}=\frac14\left(D_qg_{ij}+g_{0i}v_j+g_{0j}v_i-\frac{f v_iv_j}{D_q}\right).$$ Step 1.1 gives $D_q=4q^2+O_5(r^{-1})$ and $v_i=O_5(r^{-2})$, also after zero, one or two parameter derivatives on a compact positive interval $J$. Since $D_q$ has a common positive lower bound on the distant end, the identity $D_q^{-1}-(4q^2)^{-1}=-(D_q-4q^2)/(4q^2D_q)$ and repeated product differentiation give $D_q^{-1}=(4q^2)^{-1}+O_5(r^{-1})$ with the same mixed bounds. In [F2], $f=1+O_6(r^{-1})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$ and $g_{0i}=O_6(r^{-2})$; these fields have no parameter dependence. The displayed component formulas therefore give, for $j=0,1,2$, $$\partial_q^j\big((g_q)_{00}+c(q)^2\big)=O_5(r^{-1}),\qquad \partial_q^j\big((g_q)_{ij}-b(q)^2\delta_{ij}\big)=O_5(r^{-1}),\qquad \partial_q^j(g_q)_{0i}=O_5(r^{-2}),\qquad b(q)=q,\quad c(q)=\frac{d_q}{4q}.$$ Every spatial-block product involving $v_i$ has order at most $-4$, and every error in the other leading terms contains a factor of order at most $-1$; the finite product and reciprocal rules retain these orders under the stated mixed derivatives. Positivity and smoothness of $b,c$ follow from [F10]. The common second-parameter bounds meet the sufficient alternative in [F18] for its annular $C^{4,\alpha}$ parameter-norm conditions, using [F12] for the spatial Hölder upgrade. Thus rational dependence alone has not been substituted for a decay or parameter-norm estimate. [F2, F6, F9, F10, F12, F18, F24, step 1.1, algebra]

3.1 Choose the field and graph neighborhood from [F17]. It equals the normal near S, so its lapse there is one, and equals T far out. At the supplied pole, $T_p=0$ gives $f(p)=0$, so [F10] yields $d_{q_*}=(1+q_*)^2+(1-q_*)^2\psi(p)^2>0$. The time scaling in [F3] gives $T=\partial_t=(d_{q_*}/(4q_*))\partial_{t_{q_*}}$. The normalized metric and normal asymptotics in [F5] and [F14] therefore give $a_*\to d_{q_*}/(4q_*)>0$. [F16] supplies the positive lower bound, weighted inverse multiplier and preservation of zero trace. In particular no vanishing stationary lapse at S is incorrectly inverted. [F3, F5, F10, F14, F16, F17, F21, step 2.1, algebra]

4.1 The common stationary product and fixed end coordinates are [F3]. The jointly smooth metric on the exterior and a common neighborhood of $S$ is [F4]; the reference is smooth, spacelike and maximal by hypothesis. On the tail the mixed bounds in step 2.2 and the decaying reference slope give a common positive lower bound for the induced spatial metric on a smaller parameter interval. On the remaining compact part, continuity preserves spacelikeness after shrinking that interval. These match the general analytic hypotheses of [F18], whose reference height is the constant rescaling of the supplied normalized height in [F3]. Apply it to get $u_*\in C^{5,\alpha}_{-3/4}$, $\Delta_0u_*\in C^{2,\alpha}_{-3}$ and the $C^1$ reference residual in weight $-3$. Its separate Harrison application is formulated under the complete Radu GR/SBS contract; that stronger application is not inferred from the present weaker end data. Here the general interface is applied with the actual mixed bounds proved in step 2.2. At $q_*=1$, $D_1=d_1=4$. The polynomial definitions of $W_q,D_q,d_q$ extend to real $q$ near one. The end bounds of steps 1.1 and 2.2 persist there, and positivity of $D_q,d_q$ persists on the end and on a common neighborhood of the compact remainder by continuity. The contraction is a polynomial identity in $q$; hence [F24]'s inverse-map calculation still makes the extended metric Lorentzian and jointly smooth. Its time orientation is transported by $A_q$ as in [F3]. This supplies the open analytic interval also at the endpoint without extending any electromagnetic equation. The field and admissible graph neighborhood in step 3.1, the reference estimates just obtained, and step 2.2 meet all the hypotheses of [F19]. It gives the global $C^1$ map between the Banach Dirichlet spaces for every $-1<\beta<0$, using [F20] and [F21]. No Jacobi inverse is asserted. [F3, F4, F9, F10, F17, F18, F19, F20, F21, F23, F24, step 1.1, step 2.1, step 3.1, step 2.2, algebra]

5.1 The graph variation in direction w has velocity wY and normal speed a_*w. Since the reference slice is maximal, its tangential transport term vanishes in [F22]. This gives the first derivative identity. For the constant rescaling $\bar h=q_*^{-2}h_*$, the coordinate determinant-and-inverse formula for the Laplacian gives $\Delta_{\bar h}=q_*^2\Delta_{h_*}$; substitution gives the second identity. This proves the claimed linearization, weighted estimates and mapping properties under the existing-slice hypotheses. [F19, F22, step 2.1, step 3.1, step 4.1, algebra] ∎

## Source notes

The original article uses Z for this auxiliary transverse field; it is denoted Y here to avoid confusion with the axial circle generator. The fifteen local intermediate items supply three separate five-item chains: graph Hölder/geometry estimates, weighted Banach/multiplier structure, and the C1 graph map. No new external theorem is imported: the exact earlier annular and Jacobi suppliers supply the established analytic inputs, and all remaining bridges are locally authored. This does not prove the eventual existence of a maximal slice, invertibility or the continuation conclusion assigned to subsequent items.

The electromagnetic decay uses the existing smooth global primitive and its original-chart bound, without identifying it with the exact radial integral. The parameter application uses the general stationary-family part of the residual theorem after explicit verification of its mixed bounds, rather than silently importing the stronger source-native Radu hypotheses of its separate Harrison specialization. These are local applications of existing suppliers, not additional external inputs.

These explicit premises specify the generated conditional result. They are not asserted to follow from the original regularity definition alone, and are not attributed to the original article. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

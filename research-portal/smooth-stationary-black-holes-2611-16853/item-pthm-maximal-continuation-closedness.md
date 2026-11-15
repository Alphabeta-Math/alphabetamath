---
title: Closedness and smooth limiting maximal sections
status: published
research_item: pthm-maximal-continuation-closedness
dependency_level: 22
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 12 and 20–21, Theorem 3.1 and §3.2.3
      attribution: The article asserts a smooth limiting maximal section with boundary
        S, stationary graph interior, and the end estimates (3.2), obtained by
        compact-exhaustion convergence and boundary normal-graph estimates.
      hypotheses: The regular stationary vacuum construction and its existing maximal
        candidate sections on a fixed positive parameter interval.
      reading_limits: "Retained attribution-reading record: Read the frozen article
        text at the cited passages. This reference attributes the article claim
        and is not used as proof of it. This maintenance revision checks the
        actual current item and supplier contracts and supplies a local
        compactness argument; no new original-PDF or external-proof reading is
        claimed."
---

PDF p. 20: ` §3.2.3, compact estimates `; PDF p. 21: ` §3.2.3, passage to the limit `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)
- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-arzela-ascoli-for-real-ck](https://alphabetamath.cc/item/thm-arzela-ascoli-for-real-ck)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)
- [pthm-compact-spacelike-and-lapse-estimates](item-pthm-compact-spacelike-and-lapse-estimates)
- [pthm-uniform-horizon-maximal-graphs](item-pthm-uniform-horizon-maximal-graphs)
- [pthm-annular-schauder-decay](item-pthm-annular-schauder-decay)
- [pthm-maximal-graph-equation](item-pthm-maximal-graph-equation)
- [pthm-common-reference-collar](item-pthm-common-reference-collar)
- [pthm-boundary-normal-angle](item-pthm-boundary-normal-angle)
- [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone)
- [math:thm-bolzano-weierstrass](https://alphabetamath.cc/item/thm-bolzano-weierstrass)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)
- [math:thm-continuous-implies-integrable](https://alphabetamath.cc/item/thm-continuous-implies-integrable)
- [math:lem-uniform-integral-error-bound](https://alphabetamath.cc/item/lem-uniform-integral-error-bound)


## Statement

Adopt the regular mass-one stationary vacuum construction with original maximal exterior section $\Sigma_1$, bifurcation sphere $S$, $T|_S\not\equiv0$, and the selected smooth Harrison family $g_q$. Assume the Axiom of Choice. Fix $\delta\in(0,1)$ and a family of existing connected smooth spacelike maximal sections satisfying all candidate, positive-lapse, boundary, compact-height and normalized-end hypotheses of [pthm-compact-spacelike-and-lapse-estimates](item-pthm-compact-spacelike-and-lapse-estimates), [pthm-uniform-horizon-maximal-graphs](item-pthm-uniform-horizon-maximal-graphs) and [pthm-annular-schauder-decay](item-pthm-annular-schauder-decay). Their interiors are stationary graphs $t=u_q(x)$ over $\Sigma_1^\circ$.

If $q_j\to q_*\in[\delta,1]$, a subsequence converges to a stationary graph $t=u_*(x)$ in $C^{3,\alpha}$ on every compact subset of $\Sigma_1^\circ$, for every $0<\alpha<1$. Its interior is smooth, spacelike and maximal for $g_{q_*}$. It extends smoothly as a spacelike hypersurface with boundary $S$. In the normalized end coordinates $x_{q_*}=q_*x$ and $t_{q_*}=d_{q_*}t/(4q_*)$, its normalized height $\widetilde u_*$ obeys $|D_{x_{q_*}}^k\widetilde u_*|\le C_k r_{q_*}^{-3/4-k}$ for $0\le k\le4$ sufficiently far out. In particular the normalized height tends to zero at infinity.

## Facts & Assumptions

[A1] The model, regularity and normalization specify the smooth stationary exterior product, the reference section and boundary, and the positive scaling $d_q/(4q)$. A stationary graph is the image of $x\mapsto(u_q(x),x)$; spacelike means positive-definite induced metric and maximal means zero mean curvature. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-harrison-normalization](item-def-harrison-normalization) [def-stationary-maximal-graph](item-def-stationary-maximal-graph) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[A2] Work in ZFC, including the choice assumptions of the compactness supplier. Hölder spaces and their norms are those in the indicated definition. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F1] The Harrison metrics are jointly smooth in spacetime and parameter. On every compact subset of the reference interior the compact estimate gives uniformly bounded candidate normals in fixed compact exterior coordinates, uniform full stationary $C^{m,\alpha}$ bounds for $u_q$ for every finite $m\ge0$ and $0<\alpha<1$ (in particular the fourth-order bounds), uniform finite-order local spacelike temporal-graph estimates, and a positive lower bound for the stationary lapse $N_q=-g_q(T,n_q)$. [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum) [pthm-compact-spacelike-and-lapse-estimates](item-pthm-compact-spacelike-and-lapse-estimates)

[F2] On a common collar of $S$, the candidates are one-to-one normal-geodesic graphs over the reference section with zero boundary heights, a uniform strict spacelike cone and uniform $C^{k,\alpha}$ bounds up to $S$ for every finite $k$. The normal-graph definition specifies the exponential-map representation and mean curvature. The same horizon supplier gives unique smooth Hawking-flow heights $v_q$ on a common closed reference collar, with $|v_q|\le C_\delta$. [pthm-uniform-horizon-maximal-graphs](item-pthm-uniform-horizon-maximal-graphs) [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[F3] On a common normalized end the candidate heights obey the stated derivative decay through order four, with constants uniform on $[\delta,1]$. The candidates satisfy the maximal graph equation. [pthm-annular-schauder-decay](item-pthm-annular-schauder-decay) [pthm-maximal-graph-equation](item-pthm-maximal-graph-equation)

[F4] For real continuous functions on a compact metric space, an equicontinuous pointwise bounded family has compact closure. [math:thm-arzela-ascoli-for-real-ck](https://alphabetamath.cc/item/thm-arzela-ascoli-for-real-ck)

[F5] For maps between Euclidean open sets, total differentiability of $f$ at $a$ and of $g$ at $f(a)$ gives $D(g\circ f)(a)=Dg(f(a))\circ Df(a)$. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F6] The horizon-supplier hypotheses expressly required in the Statement bind the reference section to $\Sigma_1=C\cup S$, where $C=\Sigma_0\cap\mathcal E$ is the actual original exterior section, and assume $H_g|_C=0$. The same required horizon hypotheses include two-sided far-end access: for some $R_a$ and every $R\ge R_a$, with $U_R=\mathbb R\times\{r>R\}$ in the selected physical stationary end chart, $\mathcal E\subset I^-_{(\mathcal E,g)}(U_R)\cap I^+_{(\mathcal E,g)}(U_R)$, using timelike paths within the original exterior and metric. Retain the fixed common end-estimate radii and constants of this supplied family. Use this same reference section, selected Harrison family and complete candidate hypotheses in [F2]; the spherical identification and the physical stationary end chart remain independent. The common-collar result supplies a fixed field $K$ vanishing on $S$, Killing for every $g_q$, with the same positive normal-plane boost rate $\kappa$, and a complete smooth flow whose images of reference interior points remain in the exterior $\mathcal E$. Its uniformly spacelike reference collar has jointly smooth boundary-distance coordinates $c_q(\rho,\eta)$ and future normals $\bar n_q$. The Gaussian-flow lemma supplies jointly smooth normal coordinate maps $\Psi_q(\tau,R,y)=\exp^{(q)}_{c_q(R,y)}(\tau\bar n_q(c_q(R,y)))$ and inverses on common smaller neighborhoods. Here $\eta,y\in S$; their identification with the unit sphere is an auxiliary collar coordinate choice, unrelated to the physical end chart. [pthm-common-reference-collar](item-pthm-common-reference-collar) [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F7] The smooth background and signed boost data in [F6], with the bound $|v_q|\le C_\delta$ in [F2], meet the bounded-time hypotheses of the Gaussian-flow lemma. Use the common closed source collar $0\le\rho\le a$ and target radius $0<b<c_1a/2$ in the boundary-angle result's explicit image-and-capture conclusion, with $\Phi_q(x)=\phi^K_{v_q(x)}(x)$. The Gaussian-flow lemma gives $c_1\rho\le R\le c_2\rho$ and $|\tau|\le\theta R$, with $c_1,c_2>0$ and $\theta<1$ uniform in $q$. The boundary-angle conclusion identifies the entire bounded-height flow-image portion over $0\le R<b$ with its unique normal graph and supplies a common ambient neighborhood $U$ of $S$ with $\Sigma_q\cap U$ contained in that graph. Its complete original-background and candidate height/barrier hypotheses are already required in the Statement and [F2], [F6]. Reduce $b$ to lie in the higher-regularity graph domain of [F2], and shrink $U$ accordingly as permitted by that explicit conclusion. These applications require no uniform derivatives of $v_q$. [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone) [pthm-boundary-normal-angle](item-pthm-boundary-normal-angle)

[F8] Every bounded real sequence has a convergent subsequence. Apply this successively to finitely many real coordinates when needed. [math:thm-bolzano-weierstrass](https://alphabetamath.cc/item/thm-bolzano-weierstrass)

[F9] Continuous real functions on closed finite intervals are Riemann integrable. For two integrable functions the absolute difference of their integrals is bounded by the interval length times a uniform bound for their difference. The fundamental theorem applies to each smooth candidate derivative along a coordinate segment in its open chart. We use these facts to identify the componentwise compactness limits as successive derivatives; on boundary half-boxes first work in the interior and pass to the boundary by continuity. [math:thm-continuous-implies-integrable](https://alphabetamath.cc/item/thm-continuous-implies-integrable) [math:lem-uniform-integral-error-bound](https://alphabetamath.cc/item/lem-uniform-integral-error-bound) [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)

## Proof

**Given:** The construction, candidate family and convergent parameter sequence in the Statement.

**Goal:** Construct the asserted subsequential smooth maximal limit, including its boundary and end behavior.

1.1 Choose a countable compact exhaustion of $\Sigma_1^\circ$ by coordinate patches with compact closure and a finite subcover at each stage. On each patch, [F1] bounds derivatives through order four and makes those derivatives equicontinuous. Apply [F4] componentwise to the finitely many derivatives through order four, and diagonalize over the patches and exhaustion. To identify these componentwise limits, write $f_\alpha$ for the uniform limit of $D^\alpha u_j$ on a smaller coordinate box. For every coordinate segment remaining in that box, [F9] gives $D^\alpha u_j(x+t e_\ell)-D^\alpha u_j(x)=\int_0^t D^{\alpha+e_\ell}u_j(x+s e_\ell)\,ds$. The integrability and uniform integral-error bound in [F9] permit passage to $f_\alpha(x+t e_\ell)-f_\alpha(x)=\int_0^t f_{\alpha+e_\ell}(x+s e_\ell)\,ds$. After division by nonzero $t$, continuity of $f_{\alpha+e_\ell}$ makes the right-hand average tend to $f_{\alpha+e_\ell}(x)$ as $t\to0$, identifying the corresponding partial derivative. Induction over derivative order therefore identifies all the extracted limits with derivatives of $u_*=f_0$. The resulting subsequence therefore converges in $C^4$ on every compact subset. The uniform fourth-derivative bounds imply convergence in $C^{3,\alpha}$ there for every $0<\alpha<1$: the difference of third derivatives tends uniformly to zero and has a common Lipschitz bound, so its $\alpha$-Hölder seminorm also tends to zero. Denote the limit by $u_*$. [given, A2, F1, F4, F9]

2.1 For the graph level function $\tau_q=t-u_q(x)$, the future normal is $n_q=-\operatorname{grad}_{g_q}\tau_q/\sqrt{-g_q^{-1}(d\tau_q,d\tau_q)}$. Since $T=\partial_t$ and $d\tau_q(T)=1$, the lapse is $N_q=-g_q(T,n_q)=1/\sqrt{-g_q^{-1}(d\tau_q,d\tau_q)}$. Fix a compact subset of the reference interior. By [F1] its candidate points and normals are uniformly bounded in fixed compact exterior coordinates. The smooth stationary field $T$ and the jointly smooth metrics $g_q$ have bounded coordinate components on that compact region and the compact parameter interval. Consequently the contraction $N_q=-g_q(T,n_q)$ has a uniform upper bound $C>0$ there. Thus $-g_q^{-1}(d\tau_q,d\tau_q)=N_q^{-2}\ge C^{-2}$. Joint metric convergence and step 1.1 pass this inequality to $q_*,u_*$, making the limiting level covector timelike and the graph spacelike. Its mean curvature is a continuous expression in the metric and its first derivatives and the graph derivatives through order two, so it is zero by passage to the limit. [given, A1, F1, step 1.1]

3.1 Use the compact supplier's explicit full stationary $C^{m,\alpha}$ estimates in [F1] at every finite $m$. The same complete compact, height/barrier, horizon, normalized-end and positive-lapse hypotheses are required in the Statement, with the actual reference section and selected family matched in [F6]. The quantitative coordinate transfer is supplied by that result, rather than inferred here from pointwise transversality alone. Apply [F4] to successive finite collections of these stationary derivative fields and diagonalize over the exhaustion and derivative orders, retaining a subsequence of step 1.1. Use the coordinate-segment argument in step 1.1 with [F9] to identify every new derivative limit as a derivative of that same $u_*$. Hence $u_*$ is smooth in the interior. [A2, F1, F4, F6, F9, step 1.1, step 2.1]

4.1 On the common normal collar, express the heights in the fixed coordinate domain $(R,y)\in[0,b)\times S$ using the jointly smooth maps in [F6]. The uniform finite-order bounds in [F2] remain uniform under these smooth background coordinate changes. Apply [F4] in finitely many closed collar charts and diagonalize over derivative orders and smaller closed target collars, retaining the interior subsequence from step 3.1. Identify the componentwise derivative limits by the coordinate-segment argument in step 1.1 using [F9], first in boundary half-box interiors and then on their closed faces by continuity. Write the resulting heights as $w_j\to w_*$ smoothly up to $R=0$ on every smaller closed collar, and set $G_j(R,y)=\Psi_{q_j}(w_j(R,y),R,y)$ and $G_*(R,y)=\Psi_{q_*}(w_*(R,y),R,y)$. Then $G_j\to G_*$ smoothly there. The zero boundary values give $G_*(0,y)=y$, and the uniform tangent spacelikeness in [F2] makes $G_*$ a smooth spacelike embedded normal graph with boundary $S$. It remains to compare its punctured image with the stationary limit. [F2, F4, F6, step 3.1, F9]

5.1 Fix $0<R<b$ and $y\in S$. By [F7], $G_j(R,y)=\phi^K_{s_j}(c_{q_j}(\rho_j,\eta_j))$ with $|s_j|\le C_\delta$ and $R/c_2\le\rho_j\le R/c_1<a/2$. In the fixed identification $S\cong S^2$, apply [F8] successively to the five bounded real coordinates $s_j,\rho_j,\eta_j^1,\eta_j^2,\eta_j^3$. Along a further subsequence for this fixed point they converge to $s_\infty,\rho_\infty,\eta_\infty$; the closed interval inequalities and sphere equation pass to the limit, so $\rho_\infty\ge R/c_2>0$ and $\eta_\infty\in S$. Smoothness of the reference collars and complete flow in [F6] gives $G_*(R,y)=\phi^K_{s_\infty}(c_{q_*}(\rho_\infty,\eta_\infty))\in\mathcal E$. Thus these candidate points converge to an exterior point, and their stationary projections lie eventually in one compact interior coordinate neighborhood. Write their stationary coordinates as $(t_j,x_j)\to(t_*,x_*)$. Since $t_j=u_{q_j}(x_j)$, uniform convergence on that compact neighborhood in step 1.1 and continuity of $u_*$ imply $t_*=u_*(x_*)$. Consequently every punctured normal-limit point belongs to the stationary limit. The positive lower bound for $\rho_j$ and bounded flow times supply precisely the control that prevents its stationary projections from escaping to the horizon. [A1, F2, F6, F7, F8, step 1.1, step 4.1]

6.1 Conversely, choose a smaller common ambient neighborhood of $S$ inside the capture neighborhood in [F7] and the Gaussian domains in [F6], with all its target radial coordinates less than some $b'<b$. Let $P=(u_*(x),x)$ be any stationary-limit point there. Its candidate approximants $P_j=(u_{q_j}(x),x)$ converge to $P$ by step 1.1 and are eventually in the capture neighborhood, so $P_j=G_j(R_j,y_j)$ with $0<R_j<b$. Joint smoothness of the Gaussian inverses gives $(\tau_j,R_j,y_j)\to(\tau_*,R_*,y_*)$, where $\tau_j=w_j(R_j,y_j)$, $0\le R_*<b$, and $P=\Psi_{q_*}(\tau_*,R_*,y_*)$. The cone inequality in [F7] passes to $|\tau_*|\le\theta R_*$. If $R_*=0$, this forces $\tau_*=0$ and hence $P=y_*\in S$, contradicting $P\in\mathcal E$. Therefore $R_*>0$. Smooth convergence of the normal heights on smaller closed collars in step 4.1 gives $\tau_*=w_*(R_*,y_*)$, so $P=G_*(R_*,y_*)$. This proves the reverse inclusion near $S$. Together with step 5.1 it identifies the two images on an ambient overlap, and the embedded spacelike normal graph from step 4.1 extends the stationary limit smoothly with boundary exactly $S$. [A1, F6, F7, step 1.1, step 4.1, step 5.1]

7.1 In the end coordinates the rescalings depend smoothly on $q$ and remain invertible for $q\in[\delta,1]$. Write $y=x_q$. The normalized height definition gives $\widetilde u_q(y)=d_q u_q(y/q)/(4q)$. For fixed $q$, the map $y\mapsto y/q$ is linear with derivative $q^{-1}I$. Applying [F5] successively to $u_q$ and its partial derivatives gives $D_y^\beta\widetilde u_q(y)=d_q(D_x^\beta u_q)(y/q)/(4q^{1+|\beta|})$ for every multi-index $\beta$ with $0\le|\beta|\le4$; order zero is the defining identity. These applications are valid because each candidate is smooth, and the linear rescaling has no higher derivatives. At any fixed point $y$ on a sufficiently distant common normalized end, $y/q_j\to y/q_*$ inside a compact neighborhood of the original end. Step 1.1 gives uniform convergence of the derivatives through order four on that neighborhood. The displayed identity and continuity of the limit derivatives and scalar factors therefore give convergence of normalized derivatives through order four at $y$. Passing to the uniform inequalities in [F3] yields $|D_{x_{q_*}}^k\widetilde u_*|\le C_k r_{q_*}^{-3/4-k}$ for $0\le k\le4$. The case $k=0$ gives the required zero limit at infinity. Together with steps 2.1–6.1 this proves the Statement. [A1, F3, F5, step 1.1, step 2.1, step 3.1, step 4.1, step 5.1, step 6.1] ∎

## Source notes

The article reference attributes the original continuation claim. The argument above uses the declared estimates and compactness input; it does not assume the article's limiting conclusion as a premise. The boundary comparison in steps 5.1 and 6.1 is a locally authored repair of the generated draft, using the same supplier hypotheses already required in the Statement. It establishes no defect attributable to the original article. The original extraction and its coverage, including original Theorem 1.1 and its unresolved source-assessment status, are unchanged.

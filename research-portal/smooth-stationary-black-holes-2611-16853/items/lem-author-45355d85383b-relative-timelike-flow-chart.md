---
id: lem-author-45355d85383b-relative-timelike-flow-chart
title: A timelike transverse field gives a fixed-boundary admissible graph
  neighborhood
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary
  - def-normal-graph-and-mean-curvature-data
  - lem-author-45355d85383b-induced-metric-and-normal-decay
  - lem-author-45355d85383b-weighted-holder-completeness
  - def-stationary-lorentzian-data
  - math:thm-fundamental-theorem-on-flows
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - def-exterior-weighted-elliptic-data
  - math:def-axiom-of-choice
  - math:thm-chain-rule-for-total-derivatives
  - math:cor-mean-value-theorem
dependency_roles:
  math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary: mathematical-premise
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  lem-author-45355d85383b-induced-metric-and-normal-decay: mathematical-premise
  lem-author-45355d85383b-weighted-holder-completeness: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  def-exterior-weighted-elliptic-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 5
---

## Statement

Work in ZFC. Fix $0<\alpha<1$ and $\beta<0$. Let $(M,g_0,N_0,T)$ be smooth stationary Lorentzian data and let $\Sigma\subset M$ be a supplied smooth embedded spacelike hypersurface with compact smooth boundary $S$. Give $\Sigma$ the fixed exterior and compact-chart data defining $C^{4,\alpha}_\beta$ and $X_\beta=\{w\in C^{4,\alpha}_\beta:w|_S=0\}$. Fix a compact core containing $S$.

Here a **stationary graph end** means the following supplied data, rather than a consequence of the Killing condition. There is a diffeomorphism $\Psi:\mathbb R_t\times\{x\in\mathbb R^3:r=|x|>R\}\to U\subset M$ onto an open set, with $T=\Psi_*(\kappa\partial_t)$ for a fixed $\kappa>0$, and $\Sigma\cap U=\{\Psi(u(x),x):r>R\}$ for a smooth function $u$. The spatial chart agrees with the fixed exterior chart on this tail, whose complement in $\Sigma$ is compact. The metric coefficients are independent of $t$, $\partial_t$ is future timelike, and there are finite $B,L$ and $m>0$ such that $|g_{0,00}|\le B$, $|(g_{0,01},g_{0,02},g_{0,03})|\le B$, $|(g_{0,ij})|\le B$, $|Du|\le L$ and
$$h_{0,ij}=g_{0,ij}+g_{0,0i}u_j+g_{0,0j}u_i+g_{0,00}u_i u_j\ge m\delta_{ij}.$$
All norms and this quadratic-form inequality use the Euclidean spatial coordinates. The stationary Cartesian metric and maximal-graph hypotheses of the induced-metric-and-normal-decay supplier give one sufficient instance of these bounds after increasing $R$; the construction itself only needs the displayed bounds and the supplied product.

There is a smooth ambient future timelike field $Y$ on a neighborhood of $\Sigma$, equal along $\Sigma$ to its $g_0$ future unit normal on a neighborhood of the chosen compact core and equal to $T$ on a sufficiently distant product tail. For some $\varepsilon>0$, every $w\in X_\beta$ with $\|w\|_{C^{4,\alpha}_\beta}<\varepsilon$ defines an embedded spacelike $C^{4,\alpha}$ flow graph $F_w(x)=\phi^Y_{w(x)}(x)$, with $F_w|_S=\operatorname{id}_S$. For functions of this regularity, “flow graph” here extends the smooth graph definition by that same formula, with embedding and spacelikeness in class $C^{4,\alpha}$; no smoothness of $w$ is asserted. On the product tail it is exactly $x\mapsto\Psi(u(x)+\kappa w(x),x)$. This is an open neighborhood of zero in the Banach space $X_\beta$, and does not identify these graphs with $T$-graphs on the compact core.

The same fixed $Y$, its flow domain and a single such ball work for a family $g_\lambda$ after shrinking an interval about $\lambda=0$, under this precise uniformity contract. The metrics and time orientations are jointly smooth on a common ambient neighborhood of $\Sigma$, with reference metric $g_0$. On the same product tail they are $t$-independent, $T$ is future timelike, and the preceding bounds on all ambient components, $Du$ and $h_{\lambda,ij}=g_{\lambda,ij}+g_{\lambda,0i}u_j+g_{\lambda,0j}u_i+g_{\lambda,00}u_i u_j$ hold with the same $B,L,m,R$. On compact ambient subsets the parameter topology is $C^1$ convergence of coefficients in fixed charts; joint smoothness supplies this convergence and bounded first derivatives on compact parameter intervals. The tail bounds are additional uniform data, not inferred from compact convergence. For example, common asymptotic bounds $g_{\lambda,00}=-a_\lambda^2+O(r^{-1})$, $g_{\lambda,ij}=b_\lambda^2\delta_{ij}+O(r^{-1})$, $g_{\lambda,0i}=O(r^{-2})$, with $a_\lambda,b_\lambda$ bounded above and away from zero, and $Du=O(r^{-7/4})$, imply this contract on a common sufficiently distant tail.

## Facts & Assumptions

[A1] ZFC includes Choice, in particular the countable instance used by the partition theorem. It is used to invoke that theorem in the normal extension and cutoff construction. [[math:def-axiom-of-choice]]

[F1] Smooth subordinate partitions of unity exist on smooth manifolds with boundary under countable Choice. [[math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary]]

[F2] The smooth flow-graph formula and the induced-metric, future-normal and mean-curvature conventions are fixed by the graph definition. Its smoothness restriction is extended locally here by the explicit $C^{4,\alpha}$ construction and proof. [[def-normal-graph-and-mean-curvature-data]]

[F3] Under its stationary Cartesian metric and supplied maximal-graph hypotheses, the induced-metric supplier gives $h_{ij}-\delta_{ij}\in C^{3,\alpha}_{-1}$ and hence a uniform positive lower bound on a distant tail. Its hypotheses also give bounded ambient coefficients and bounded $Du$. No product, completeness or uniform family statement is inferred from this supplier alone. [[lem-author-45355d85383b-induced-metric-and-normal-decay]]

[F4] For fixed exterior chart data the weighted spaces and their zero-trace subspaces are Banach. [[lem-author-45355d85383b-weighted-holder-completeness]]

[F5] Stationary Lorentzian data specify the smooth metric, time orientation, future-directed convention and Killing field, without asserting a product end or complete flow. [[def-stationary-lorentzian-data]]

[F6] A smooth vector field has its unique smooth local flow on an open time-space domain, with the flow law and inverse time maps wherever defined. [[math:thm-fundamental-theorem-on-flows]]

[F7] An invertible differential gives a local smooth inverse. Near $S$ this is applied in an ambient chart after locally extending the embedded hypersurface across its boundary. [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[F8] The weighted norm is the sum of the fixed compact-chart derivative and Hölder norms and the supremum of the scaled annular norms, with order-$j$ factor $R^{j-\beta}$. Boundary values are continuous extensions. [[def-exterior-weighted-elliptic-data]]

[F9] Differentiable Euclidean maps obey the total-derivative chain rule. Iterating it in coordinate charts gives the finite derivative expansions used for coordinate changes and flow composition. [[math:thm-chain-rule-for-total-derivatives]]

[F10] A real function continuous on a closed interval and differentiable inside has increment bounded by interval length times its derivative supremum. It is applied to smooth coefficient functions on closed time intervals or coordinate segments; boundary formulas follow by continuity. [[math:cor-mean-value-theorem]]

## Proof

**Given:** The supplied slice, product-end data, bounds, chart choices and, when applicable, parameter hypotheses in the Statement.

**Goal:** Construct the timelike field and an open fixed-boundary admissible $C^{4,\alpha}_\beta$ graph ball, with the stated uniformity.

1.1 The smooth future normal in [F2] can be extended off $\Sigma$ in embedded hypersurface charts, including boundary charts by local extension across the boundary. Shrinking their ambient neighborhoods preserves timelikeness. Use [F1] under [A1] to patch these extensions near any compact truncation containing the chosen core. On the slice every extension equals the same normal, so the patched field equals it there. The future timelike cone is convex: in a time-oriented orthonormal frame it is $v^0>|v^{\mathrm{spatial}}|$, and positive sums satisfy that inequality by the triangle inequality. Thus the patch remains future timelike. Choose the truncation and a smooth cutoff so its transition to $T$ lies inside the supplied product end; there both fields are future timelike. Their cutoff combination is a smooth future timelike $Y$, equal to the normal along a neighborhood of the core and equal to $T$ on a whole distant product tail. The normal extensions and cutoff use only a compact region, while the prescribed $T$ supplies the rest. [A1, F1, F2, F5, given, construct]

2.1 A timelike vector cannot be tangent to a spacelike hyperplane, so $Y$ is transverse to $\Sigma$. By [F6], $H(s,x)=\phi_s^Y(x)$ is smooth near $\{0\}\times\Sigma$. Its differential there sends $(a,v)$ to $aY_x+v$ and is invertible. Apply [F7] to obtain local flow coordinates, using local extensions across $S$ before restriction. Compactness gives a common small flow interval over every fixed compact truncation. On the tail where $Y=T$, uniqueness in [F6] identifies the flow with $\Psi(u(x)+\kappa s,x)$ for every $s$; the full product ensures existence, and the spatial coordinate is unchanged. Thus there is one interval $|s|<s_0$ on all of $\Sigma$. [F2, F5, F6, F7, step 1.1, given]

3.1 Shrink $s_0$ to obtain global injectivity, including the overlap. If no such shrinking worked, there would be distinct pairs $(s_j,x_j),(t_j,y_j)$ with $s_j,t_j\to0$ and equal images. If both base points lie on the translation tail, equality of spatial coordinates and then of times forces the pairs to coincide. Otherwise a subsequence of one base sequence lies in a compact truncation, say $x_j\to x$. The inverse flow gives $y_j=\phi_{-t_j}^Y(\phi_{s_j}^Y(x_j))\to x$ in $M$. Since $\Sigma$ is embedded and $x\in\Sigma$, this is convergence in $\Sigma$ as well. Both pairs then lie in a single local flow chart from step 2.1, contradicting its injectivity. The flow law applies near $x$ on a uniform time interval, so this reasoning does not assume any bounded-coordinate behavior of a distant base sequence. [F6, F7, step 2.1]

3.2 On the translation tail the exact graph formula gives [step 2.1]
$$h_{\lambda,w,ij}=h_{\lambda,ij}+\kappa(g_{\lambda,0i}+g_{\lambda,00}u_i)w_j+\kappa(g_{\lambda,0j}+g_{\lambda,00}u_j)w_i+\kappa^2g_{\lambda,00}w_iw_j.$$
Consequently, for Euclidean spatial $v$, $|(h_{\lambda,w}-h_\lambda)(v,v)|\le\{2\kappa B(1+L)|Dw|+\kappa^2B|Dw|^2\}|v|^2$. Choose $\delta>0$ with $2\kappa B(1+L)\delta+\kappa^2B\delta^2\le m/2$. Then $|Dw|<\delta$ implies $h_{\lambda,w}\ge(m/2)\delta_{ij}$ on the whole tail. There is no height term here because the coefficients are stationary. For the sufficient single-metric instance in [F3], its hypotheses bound the components and slopes and its conclusion supplies $m$ far out. For the family example in the Statement, the exact formula for $h_\lambda$ gives $h_\lambda=b_\lambda^2 I+O(r^{-1})$ uniformly, since $Du=O(r^{-7/4})$ and all coefficient bounds are common. Increasing $R$ gives $h_\lambda\ge(b_-^2/2)I$, where $b_-=\inf b_\lambda>0$; the time coefficient is negative there by the analogous $a_->0$ bound. The remaining common component bounds follow from their displayed asymptotics. [F2, F3, F5, step 2.1, given, algebra]

4.1 The injective flow map also gives a topological embedding on a smaller slab, including at $S$. To check the only extra boundary issue, choose nested compact truncations $K_0\subset\operatorname{int}_\Sigma K_1$, with $K_0$ containing the whole nontranslation region. By embeddedness and compactness there is an ambient open neighborhood $W$ of $K_0$ with $W\cap\Sigma\subset\operatorname{int}_\Sigma K_1$. Shrink the time interval so all flow displacements of points of $K_0$ by times of absolute value at most four times that interval stay in $W$. If slab images approach an image based in $K_0$, pass to a convergent subsequence of their bounded time coordinates. The inverse flow then places their base points eventually in $W\cap\Sigma$, hence in $K_1$. Compactness and injectivity identify their only possible base/time limit with the target pair. This proves inverse continuity there. At base points outside $K_0$ and away from $S$, local flow coordinates are open ambient coordinates, so injectivity gives inverse continuity directly. Restricting to a still smaller open slab leaves room for the preceding time closures. Thus its graph restrictions have the subspace topology required for embeddings. [F6, F7, step 2.1, step 3.1]

5.1 A small $C^1$ graph is spacelike on the compact part, with an explicit uniform estimate. In finitely many flow charts write $G_\lambda=H^*g_\lambda$. On a compact parameter interval and a closed smaller flow slab all its components and their $s$ derivatives are bounded, since $H$ is smooth and the metrics are jointly smooth. At $(\lambda,s)=(0,0)$ its spatial restriction is positive definite; compactness and parameter continuity give a common lower eigenvalue $m_K>0$ for $G_{\lambda,ij}(0,x)$ after shrinking the interval. Evaluation on the graph tangent vector $v+dw(v)\partial_s$ gives $G_{\lambda,ij}(w,x)v^iv^j+2G_{\lambda,si}(w,x)v^i dw(v)+G_{\lambda,ss}(w,x)dw(v)^2$. The mean value estimate in $s$ and the component bounds therefore give $|(h_{\lambda,w}-h_{\lambda,0})(v,v)|\le C_K(|w|+|Dw|+|Dw|^2)|v|^2$, with one $C_K$ for the finite cover. Choose these suprema small enough that the right side is at most $(m_K/2)|v|^2$. For a single metric use the same argument without the parameter. [F2, F5, F10, step 2.1, step 4.1, given, algebra]

6.1 Derive the required norm control from [F8], rather than attributing it to completeness. If $x$ is on the end with $r>2r_0$, choose $R=2r/3$, so $x\in A_R$ and $R\ge r_0$. For $j=0,1$, each order-$j$ coordinate derivative satisfies $|\partial^I w(x)|\le R^{\beta-j}\|w\|_{C^{4,\alpha}_\beta}$. Since $\beta<0$ and $r_0>0$, these coefficients are bounded on all such annuli. On the fixed compact core the derivative suprema through order one occur in $N_K$. Any enlarged compact truncation in the proof is controlled in its finite charts by those fixed core charts and finitely many bounded-radius end annuli: the chain rule introduces only bounded first derivatives of fixed coordinate transitions on compact overlaps. Hence the global function supremum and all the needed compact-chart and end first-derivative suprema are bounded by $C_\beta\|w\|_{C^{4,\alpha}_\beta}$ for a finite constant depending only on the fixed data. Choosing $\varepsilon$ small makes the height lie in the slab of step 4.1 and satisfies both steps 5.1 and 3.2. [F8, F9, step 4.1, step 5.1, step 3.2, algebra]

7.1 For every such $w$, the map $x\mapsto(w(x),x)$ is a $C^{4,\alpha}$ embedding into the slab: its differential is injective and projection to $x$ is its continuous inverse. Composition with the smooth embedded slab map proves that $F_w$ is a $C^{4,\alpha}$ embedding. In local charts, the chain rule through order four and the inequality $[ab]_\alpha\le\|a\|_\infty[b]_\alpha+\|b\|_\infty[a]_\alpha$ give this composition regularity; the smooth flow derivatives are bounded on each compact coordinate image. On smaller convex coordinate patches the mean value estimate bounds smooth coefficient increments by their bounded first derivatives times the input increment. Steps 5.1 and 3.2 give spacelikeness. The induced-metric, normal and second-fundamental-form formulas of [F2] thus remain meaningful with local regularities $C^{3,\alpha}$, $C^{3,\alpha}$ and $C^{2,\alpha}$ respectively, by their algebraic formulas and one derivative of the normal. The identity $\phi_0^Y(x)=x$ fixes $S$ because $w|_S=0$. By [F4] the zero-trace domain is Banach, and its norm ball is open. In the family case $Y$ remains future timelike on the compact slab after parameter shrinking by strict timelikeness and joint continuity; on the tail it is the supplied future timelike $T$. The flow is fixed, hence its domain, injectivity and transversality are independent of the metric parameter, while steps 5.1 and 3.2 gave common positive lower metric bounds. This proves the full uniform graph claim. [F2, F4, F5, F6, F8, F9, F10, step 1.1, step 4.1, step 5.1, step 3.2, step 6.1, algebra] ∎

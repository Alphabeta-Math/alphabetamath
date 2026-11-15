---
id: pthm-compact-timelike-length-bound
title: Compact-tube timelike length bound
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-stationary-lorentzian-data
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-maximal-graph
  - def-harrison-one-form-family
  - pthm-harrison-electrovacuum
  - pthm-compact-height-bound
  - pthm-positive-transformed-lapse
  - math:def-axiom-of-choice
  - math:thm-c1-lipschitz-ac-bv-hierarchy
  - math:lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets
  - math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions
  - math:thm-chain-rule-for-total-derivatives
  - math:thm-dominated-convergence
  - physics:def-gr-causal-curves-and-reachability
  - physics:def-gr-timelike-worldline-and-proper-time
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  def-harrison-one-form-family: mathematical-premise
  pthm-harrison-electrovacuum: physical-result
  pthm-compact-height-bound: physical-result
  pthm-positive-transformed-lapse: physical-result
  math:def-axiom-of-choice: mathematical-premise
  math:thm-c1-lipschitz-ac-bv-hierarchy: mathematical-premise
  math:lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets: mathematical-premise
  math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:thm-dominated-convergence: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  physics:def-gr-timelike-worldline-and-proper-time: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 20, §3.2.3, compact tubes and length calculation
      hypotheses: The stationary vacuum construction and candidate transformed maximal
        sections used in §3.2.3, with positive limiting parameter.
      reading_limits: Read the frozen article text at the cited passage. This
        reference attributes the article claim; the proof below uses the
        declared suppliers and does not use the article as a premise.
physical_scope: Conditional geometric deduction in the classical stationary
  vacuum model and its Harrison family; candidate maximal sections are assumed
  and no observation is asserted.
dependency_level: 16
---

## Statement

Adopt the regular stationary vacuum construction with mass one, maximal original exterior section and $T|_S\not\equiv0$. Use the single-primitive Harrison family and assume the candidate-section, normalized-end and uniform-estimate hypotheses of [[pthm-compact-height-bound]] and [[pthm-positive-transformed-lapse]] for every $q\in[\delta,1]$, where $0<\delta<1$. In particular, the exterior is the stationary product $\mathcal E=\mathbb R_t\times\Sigma_1^\circ$, $T=\partial_t$, and the supplied spacelike maximal section is the graph $t=u_q(x)$ with future unit normal $n_q$ and positive lapse $N_q=-g_q(T,n_q)$.

Let $q_j\in[\delta,1]$ converge to $q_*\in[\delta,1]$. Let $K\Subset\widetilde K^\circ\subset\widetilde K\Subset\Sigma_1^\circ$ and $0<A<\widetilde A$, and write $Q=\{\phi_t^T(x):x\in K,|t|\le A\}$ and $\widetilde Q=\{\phi_t^T(x):x\in\widetilde K,|t|\le\widetilde A\}\Subset\mathcal E$. There are finite constants $B_\delta$ and $H_{\delta,\widetilde K}$, independent of $j$ and of the curve, such that $N_{q_j}\le B_\delta$, $\sup_{\widetilde K}|u_{q_j}|\le H_{\delta,\widetilde K}$, and every future $g_{q_j}$-timelike Lipschitz curve $\gamma:[a,b]\to\widetilde Q$ satisfies $L_{g_{q_j}}(\gamma)\le B_\delta(2\widetilde A+2H_{\delta,\widetilde K})$. The same bound holds for every future $g_{q_*}$-timelike Lipschitz curve in $\widetilde Q$, without a uniform negative bound on its tangent norm.

Here Lipschitz and almost-everywhere tangents are understood in local coordinates, and $L_g(\gamma)=\int_a^b\sqrt{-g(\dot\gamma,\dot\gamma)}\,ds$. Every fixed future $g_{q_*}$-timelike Lipschitz curve in $\widetilde Q$ whose tangent obeys $g_{q_*}(\dot\gamma,\dot\gamma)\le-\epsilon$ almost everywhere for some curve-dependent $\epsilon>0$ remains future $g_{q_j}$-timelike for all sufficiently large $j$, and $L_{g_{q_j}}(\gamma)\to L_{g_{q_*}}(\gamma)$. In particular, every fixed piecewise $C^1$ curve in $\widetilde Q$ with a nonzero future $g_{q_*}$-timelike tangent on each closed smooth piece has this persistence and length convergence, and its limit-metric length has the stated bound. The constants may depend on the supplied family and $\delta$; $H$ may also depend on $\widetilde K$.

The original-section maximality used here is assumed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$, with the original metric $g$, so $H_g|_C=0$. The selected physical end retains its stated mass-one normalization. Maximality of an independently labelled chart-side section or another supplied maximal section does not replace this premise. No equality between the hypersurface identification and the physical stationary end chart is assumed. [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

Retain explicitly the two-sided original-metric access premise of [[pthm-compact-height-bound]]: every point of the original exterior can both reach and be reached from every sufficiently far selected stationary end by timelike paths inside that original exterior. This premise is used for the uniform height bound, before any transformed timelike-length estimate is applied.

## Facts & Assumptions

[A1] The stated regular stationary model, maximal original section and candidate graphs are supplied assumptions; their existence is not concluded here. The stationary product identifies $T$ with $\partial_t$, and a graph has the displayed form. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-stationary-lorentzian-data]] [[def-stationary-maximal-graph]]

[F1] The selected one-form family is built from one stationary primitive, and the corresponding Harrison metrics are jointly smooth in spacetime and $q\in[0,1]$. Hence $g_{q_j}\to g_{q_*}$ uniformly on compact sets. [[def-harrison-one-form-family]] [[pthm-harrison-electrovacuum]]

[F2] Under the explicit two-sided access premise retained from the height supplier in the Statement, Under the stated family hypotheses, the compact-height result bounds $|u_q|$ uniformly on $\widetilde K$, and the lapse result gives $0<N_q\le d_q/(4q)$ on each section. Since $d_q=(1+q)^2+(1-q)^2\psi(p)^2$, the latter upper bound is uniform for $q\in[\delta,1]$. [[pthm-compact-height-bound]] [[pthm-positive-transformed-lapse]] [[def-harrison-one-form-family]]

[F3] Spacelike means that the induced metric is positive definite; its future unit normal has metric norm $-1$. The graph is assumed spacelike; the isometry property needed for its translates is proved in step 1.2. [[def-spacelike-maximal-hypersurface-data]] [[def-stationary-maximal-graph]] [[def-stationary-lorentzian-data]]


[A2] Use the standing ZFC convention, including the Axiom of Choice; in particular the countable-choice and dependent-choice hypotheses of the absolutely continuous FTC are available. Choice enters here through that FTC in step 1.1. [[math:def-axiom-of-choice]]

[F4] On a compact interval a real Lipschitz function is absolutely continuous. Under countable and dependent choice, an absolutely continuous real function has an almost-everywhere derivative in $L^1$ and equals its initial value plus the integral of that derivative. Smooth maps are locally Lipschitz on compact coordinate subsets, and at a point where the coordinate curve is differentiable the total-derivative chain rule applies to its composition with a smooth real function. These statements will be applied coordinate by coordinate on finitely many subintervals. [[math:thm-c1-lipschitz-ac-bv-hierarchy]] [[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions]] [[math:lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets]] [[math:thm-chain-rule-for-total-derivatives]]

[F5] On a measure space, measurable functions converging almost everywhere and bounded in absolute value by one nonnegative integrable function have convergent integrals. Here the measure space is the finite parameter interval with Lebesgue measure. [[math:thm-dominated-convergence]]

[F6] Future timelike curves use the locally absolutely continuous convention: the chart derivatives define the manifold velocity wherever they exist, and that velocity is nonzero and future timelike almost everywhere. Here we restrict to locally Lipschitz curves, which are locally absolutely continuous by [F4]. The piecewise $C^1$ convention requires a finite partition into pieces that are $C^1$ up to their included endpoints, with one-sided endpoint tangents; future timelikeness is required on each piece including those one-sided tangents. [[physics:def-gr-causal-curves-and-reachability]] [[physics:def-gr-timelike-worldline-and-proper-time]]

[F7] The graph convention time-orients $g_q$ by $Y_q=A_q^{-1}N$, where $N$ is the original time-orientation field, $A_qv=v+D_q^{-1}W_q(v)T$ and $g_q=(D_q/4)A_q^*g$. In the selected family $D_q>0$, $d_q>0$ and $A_q^{-1}v=v-d_q^{-1}W_q(v)T$; hence $Y_q$ is jointly smooth in spacetime and $q$, with $g_q(Y_q,Y_q)=(D_q/4)g(N,N)<0$. Future $g_q$-timelike vectors are precisely those pairing negatively with $Y_q$. [[def-stationary-maximal-graph]] [[def-stationary-lorentzian-data]] [[def-harrison-one-form-family]] [[pthm-harrison-electrovacuum]]

[F8] The construction used in [F1], specifically Proof steps 1.1–2.1 of [[pthm-harrison-electrovacuum]], supplies a stationary normalized potential $\sigma=f+i\psi$ and the chosen stationary primitive $W_0$ with $W_0(T)=d_0-D_0$. The family formulas are $D_q=|q(1+\sigma)+(1-\sigma)|^2$, $d_q=D_q(p)$ at the fixed pole, and $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. The original metric obeys $\mathcal L_Tg=0$, and the graph convention gives $A_qv=v+D_q^{-1}W_q(v)T$ and $g_q=(D_q/4)A_q^*g$. These are the inputs for the stationarity calculation below. [[def-harrison-one-form-family]] [[def-stationary-lorentzian-data]] [[def-stationary-maximal-graph]]

## Proof

**Given:**The model, candidate family, sequence, tubes and curves in the Statement.

**Goal:** Prove the uniform length estimate, persistence of the specified fixed timelike curves, and the limiting estimate.

1.1 Fix one of the stated Lipschitz curves and a parameter $q$ for which it is future timelike. Subdivide its compact parameter interval into finitely many closed subintervals on each of which the curve has Lipschitz coordinates and its image lies in a coordinate neighborhood where the smooth function $\tau_q(t,x)=t-u_q(x)$ is Lipschitz. Such neighborhoods exist by [F4]; continuity and compactness give the finite subdivision. Each coordinate function is absolutely continuous by [F4], so its derivative exists almost everywhere, is measurable, and is bounded almost everywhere by its Lipschitz constant, as follows by taking limits of its difference quotients. The composite $\tau_q\circ\gamma$ is Lipschitz on each subinterval, hence absolutely continuous. At every point where all coordinates are differentiable, the chain rule gives $(\tau_q\circ\gamma)'=d\tau_q(\dot\gamma)$. Applying the absolutely continuous FTC on these subintervals and telescoping gives $\int_a^b d\tau_q(\dot\gamma)\,ds=\tau_q(\gamma(b))-\tau_q(\gamma(a))$. [given, A2, F4, F6]

1.2 In the product coordinates $T=\partial_t$, the Killing equation for $g$ gives $\partial_t g_{\mu\nu}=0$, so the components of $T^\flat=g(T,\cdot)$ are independent of $t$. By [F8], the components of $W_0$ and the scalar $\sigma$ are also independent of $t$. The displayed formulas therefore make $D_q$ and the components of $W_q$ independent of $t$; $d_q=D_q(p)$ is a fixed scalar, not a function of the flowing point. The coefficients of $A_q$ and consequently those of $g_q=(D_q/4)A_q^*g$ are independent of $t$. Thus each translation $\phi_s^T(t,x)=(t+s,x)$ is a $g_q$-isometry. It also preserves the declared future cones: for a future timelike vector $v$ at $z$, the vectors $v_s=(d\phi_s^T)_zv$ remain timelike, and $g_q(v_s,Y_q(\phi_s^Tz))$ is continuous in $s$, is negative at zero, and cannot vanish because both vectors are timelike. It stays negative for every $s$. This uses the time orientation in [F7], without requiring $N$ itself to be stationary. [given, A1, F7, F8, algebra]

2.1 Extend $n_q$ by the differential of the stationary flow and $N_q$ by constant transport along each orbit. Step 1.2 shows that the transported normal remains the future unit normal to each translated spacelike graph. Since the flow preserves $T$ and $g_q$, its lapse is still $-g_q(T,n_q)=N_q$, so the graph lapse bound in [F2] holds on every translate. The level sets of $\tau_q$ are the stationary translates of the graph. Their normal covector is a multiple of $g_q(n_q,\cdot)$; evaluating on $T$ gives $d\tau_q=-g_q(n_q,\cdot)/N_q$. For any future timelike tangent $v$, decompose $v=a n_q+w$ with $w\perp n_q$. Then $a=-g_q(n_q,v)>0$ and $g_q(w,w)\ge0$, so $\sqrt{-g_q(v,v)}\le a=N_q d\tau_q(v)$ and $d\tau_q(v)>0$. By step 1.1 these inequalities hold almost everywhere along the curve. [given, F2, F3, step 1.1, step 1.2, algebra]

3.1 Fix a future $g_{q_*}$-timelike Lipschitz curve in the tube with $g_{q_*}(\dot\gamma,\dot\gamma)\le-\epsilon$ almost everywhere for some $\epsilon>0$. Its coordinate velocity is essentially bounded on a finite chart subdivision, as in step 1.1. Compact uniform metric convergence therefore makes $g_{q_j}(\dot\gamma,\dot\gamma)<0$ almost everywhere for all large $j$. Use the supplied orientation $Y_q=A_q^{-1}N$ from [F7], which varies jointly smoothly for this single-primitive family. On the compact curve image set $c=\min\sqrt{-g_{q_*}(Y_{q_*},Y_{q_*})}>0$. Normalize $e=Y_{q_*}/\sqrt{-g_{q_*}(Y_{q_*},Y_{q_*})}$ and decompose a future tangent $v=ae+w$ with $w\perp e$. As in step 2.1, $a>0$ and $-g_{q_*}(v,v)=a^2-g_{q_*}(w,w)\le a^2$, so $-g_{q_*}(v,Y_{q_*})\ge c\sqrt\epsilon$. Uniform convergence of $g_{q_j}(\cdot,Y_{q_j})$ to $g_{q_*}(\cdot,Y_{q_*})$, together with the coordinate velocity bounds, then gives $g_{q_j}(\dot\gamma,Y_{q_j})<0$ almost everywhere for all large $j$. Thus the tangents remain future directed in the declared orientations. For a fixed piecewise $C^1$ timelike curve in $\widetilde Q$ with nonzero tangent on each closed piece, compactness supplies the same margins and boundedness, giving persistence on every piece, including one-sided endpoint tangents. [given, F1, F3, F6, F7, step 1.1, step 2.1, algebra]

3.2 Integrating step 2.1 and using $0<N_q\le B_\delta$ and the endpoint identity from step 1.1 yields $L_{g_q}(\gamma)\le B_\delta\int_a^b d\tau_q(\dot\gamma)\,ds=B_\delta(\tau_q(\gamma(b))-\tau_q(\gamma(a)))$. The two endpoint time coordinates lie in $[-\widetilde A,\widetilde A]$, and both endpoint spatial coordinates lie in $\widetilde K$. Thus the difference is at most $2\widetilde A+2H_{\delta,\widetilde K}$. The bounds in [F2] hold for every $q\in[\delta,1]$, so this proves the bound for each $q_j$ and directly for $q=q_*$, for every future $g_{q_*}$-timelike Lipschitz curve in $\widetilde Q$. No uniform negative tangent-norm margin is used in this direct estimate. [F2, F4, step 1.1, step 2.1, algebra]

4.1 Apply step 3.2 to the fixed curve for all sufficiently large $j$, as permitted by step 3.1. On the finite chart subdivision, define the length integrands to be zero on the common null set where coordinate derivatives do not exist or the required tangent conditions fail. They are measurable: the coordinate velocities are measurable by step 1.1, the curve and metric coefficients are continuous, and the square root is continuous on the nonnegative reals. Uniform metric convergence gives almost-everywhere convergence of these integrands to the $g_{q_*}$ integrand. On each chart piece choose finite constants $M$ bounding the coordinate velocity almost everywhere and $C$ bounding the absolute quadratic forms of all sufficiently late metrics and the limiting metric on the compact curve image. Then $0\le\sqrt{-g_{q_j}(\dot\gamma,\dot\gamma)}\le\sqrt C M$ almost everywhere. The finitely many constant bounds give one integrable majorant on $[a,b]$. Dominated convergence [F5] gives $L_{g_{q_j}}(\gamma)\to L_{g_{q_*}}(\gamma)$, and the same uniform bound passes to the limit. This proves the conclusions, including the piecewise $C^1$ case. [F1, F5, step 1.1, step 3.1, step 3.2] ∎



The article citation attributes the calculation on PDF page 20. The factor $2H_{\delta,\widetilde K}$ records both endpoint height contributions; it can be absorbed into the article's unspecified height constant. The proof uses the declared suppliers. The limit-metric bound follows directly at $q=q_*$; the uniform negative tangent-norm margin is used only for persistence and length convergence along the sequence.

## Source notes

The article bounds the length of timelike curves in a compact stationary tube by combining the transformed lapse bound and the compact graph-height bound, and passes to the limiting metric. This is attribution only, not a proof input.

The article citation attributes the calculation on PDF page 20. The factor $2H_{\delta,\widetilde K}$ records both endpoint height contributions; it can be absorbed into the article's unspecified height constant. The proof uses the declared suppliers. The limit-metric bound follows directly at $q=q_*$; the uniform negative tangent-norm margin is used only for persistence and length convergence along the sequence.

These explicit premises specify the generated conditional result. They are not asserted to follow from the original regularity definition alone, and are not attributed to the original article. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

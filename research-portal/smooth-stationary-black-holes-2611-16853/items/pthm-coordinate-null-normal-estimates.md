---
id: pthm-coordinate-null-normal-estimates
title: Normalized outward null normal at large coordinate spheres
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - pthm-harrison-component-asymptotics
  - pthm-harrison-denominator-asymptotics
  - pthm-harrison-lorentzian-algebra
  - def-harrison-normalization
  - def-null-screen-expansion-and-focal-data
  - def-stationary-asymptotic-decay-data
  - def-stationary-lorentzian-data
  - math:thm-chain-rule-for-total-derivatives
  - math:thm-euclidean-heine-borel-pseudocompactness-and-extreme-values
dependency_roles:
  pthm-harrison-component-asymptotics: physical-result
  pthm-harrison-denominator-asymptotics: physical-result
  pthm-harrison-lorentzian-algebra: physical-result
  def-harrison-normalization: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:thm-euclidean-heine-borel-pseudocompactness-and-extreme-values: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 22, proof of Proposition 4.1, nullity computation
      attribution: The normalized outward null normal has the displayed radial,
        temporal and angular estimates, and its expansion is the traced Lie
        derivative of the induced metric.
      hypotheses: The article's mass-one stationary vacuum construction and specified
        Harrison family on the asymptotic end, with q in [0,1] and sufficiently
        large coordinate radius.
      reading_limits: Read the frozen article text and PDF page 22 for attribution of
        the formulas only. The article does not assert uniform component bounds
        on every finite smooth angular atlas. The proof below uses declared
        suppliers and a local calculation on compact chart subsets.
physical_scope: Conditional geometric calculation in the stationary vacuum model
  and its supplied Harrison-transformed metrics; no measurement is asserted.
dependency_level: 10
---

## Statement

Adopt the model, mass-one stationary Cartesian end $(t,x^i)$, supplied pole and specified Harrison family of the transformed-component estimates, including all their hypotheses. Put $r=|x|$, $a=q+r^{-1}$, and $d_q=D_q(p)$ with the supplied Harrison normalization. Let $q\in[0,1]$ and take $r$ sufficiently large, with one radius independent of $q$. On the coordinate sphere $S_{t,r}$, use smooth local angular coordinates $y^A=y^A(\omega)$, where $\omega=x/r$, extended independently of $t$ and $r$, and write $\gamma_{q,AB}=(g_q)_{AB}$ for its induced metric. Let $L_q$ be the future outward null normal normalized by $g_q(T,L_q)=-d_q/4$, where $T=\partial_t$. Its metric dual is $L_q^\flat=(L_q)_t\,dt+(L_q)_r\,dr$ and $(L_q)_t=-d_q/4$. The inverse metric components satisfy the nullity equation
$$g_q^{tt}d_q^2/16-g_q^{tr}d_q(L_q)_r/2+g_q^{rr}(L_q)_r^2=0.$$
The outward branch obeys
$$L_q^r=\frac{d_q}{4}\sqrt{(g_q^{tr})^2-g_q^{tt}g_q^{rr}}=1+O(r^{-1}),\qquad (L_q)_r=(q+r^{-1})^2(1+O(r^{-1})),$$
$$L_q^t=\frac4{d_q}(q+r^{-1})^2(1+O(r^{-1})),\qquad L_q^A=O(r^{-2}).$$
The constants in the $t$- and $r$-component estimates are uniform in $q$ and over the entire sphere. For the angular estimate, fix finitely many smooth charts $y_\alpha:U_\alpha\to\mathbb R^2$ of the unit sphere and nonempty compact subsets $K_\alpha\subset U_\alpha$ whose relative interiors cover the sphere. The bound $L_q^A=O(r^{-2})$ is uniform in $q$ and $\omega\in K_\alpha$, with one constant for this finite collection. Such a covering exists, as constructed below. On any other smooth angular chart the same local estimate holds on each compact subset of its domain. Finally, with $\gamma_q^{AB}$ the inverse of $\gamma_{q,AB}$, its expansion is $\theta_{L_q}=\tfrac12\gamma_q^{AB}(\mathcal L_{L_q}g_q)_{AB}$, with the Lie derivative evaluated using any smooth extension of $L_q$ off the sphere.

## Statement references

[[pthm-harrison-component-asymptotics]]

[[pthm-harrison-denominator-asymptotics]]

[[pthm-harrison-lorentzian-algebra]]

[[def-harrison-normalization]]

[[def-null-screen-expansion-and-focal-data]]

[[def-stationary-asymptotic-decay-data]]

[[def-stationary-lorentzian-data]]

[[math:thm-chain-rule-for-total-derivatives]]

[[math:thm-euclidean-heine-borel-pseudocompactness-and-extreme-values]]

## Facts & Assumptions

[F1] The specified family has $(g_q)_{tt}=-d_q^2(16a^2)^{-1}(1+O(r^{-1}))$, $(g_q)_{ti}=d_q a^{-1}O(r^{-2})$, and $(g_q)_{ij}=a^2(\delta_{ij}+O(r^{-1}))$, uniformly in $q$. These are the zeroth-order consequences of the completed component estimates. [[pthm-harrison-component-asymptotics]] [[def-stationary-asymptotic-decay-data]]

[F2] The pole quantity $d_q=D_q(p)$ is bounded above and below by positive constants uniformly for $q\in[0,1]$. [[pthm-harrison-denominator-asymptotics]] [[def-harrison-normalization]]

[F3] The transformed metric is Lorentzian and has the supplied time orientation; on the sufficiently distant end $T$ is future timelike. A spacelike two-surface has future null normal directions, and its expansion is the trace of $\chi_L(X,Y)=g_q(\nabla_XL,Y)$ in its induced metric. [[pthm-harrison-lorentzian-algebra]] [[def-stationary-lorentzian-data]] [[def-null-screen-expansion-and-focal-data]]

[F4] The chain rule applies to the smooth angular functions and radial projection on their open Euclidean domains. Every continuous real-valued function on a nonempty compact subset of Euclidean space is bounded, and every closed bounded Euclidean subset is compact. [[math:thm-chain-rule-for-total-derivatives]] [[math:thm-euclidean-heine-borel-pseudocompactness-and-extreme-values]]

## Proof

**Given:** The specified end and family, $q\in[0,1]$, and a sufficiently large coordinate sphere.

**Goal:** Establish the normalized outward branch, its uniform component estimates, and the expansion identity.

1.1 In the Cartesian frame, scale the time direction by $4a/d_q$ and each spatial direction by $a^{-1}$. By [F1] and [F2] the scaled metric matrix is the Minkowski diagonal matrix plus an $O(r^{-1})$ matrix: the scaled mixed entries are $O(a^{-1}r^{-2})=O(r^{-1})$, because $a\ge r^{-1}$. For large $r$ its inverse is the Minkowski matrix plus $O(r^{-1})$, by the finite-dimensional inverse identity. Keeping the sharper mixed-entry estimate in the block inverse gives $g_q^{ti}=d_q^{-1}a^{-1}O(r^{-2})$, while $g_q^{tt}=-16a^2d_q^{-2}(1+O(r^{-1}))$ and $g_q^{ij}=a^{-2}(\delta^{ij}+O(r^{-1}))$. The constants and the radius are uniform in $q$. [given, F1, F2, algebra]

1.2 A covering of the required type is explicit: for $i\in\{1,2,3\}$ and $\varepsilon\in\{-1,1\}$ set $U_{i,\varepsilon}=\{\omega\in\mathbb S^2:\varepsilon\omega_i>1/4\}$, use the other two components of $\omega$ as coordinates, and set $K_{i,\varepsilon}=\{\omega\in\mathbb S^2:\varepsilon\omega_i\ge1/2\}$. The inverse chart inserts $\omega_i=\varepsilon\sqrt{1-\sum_{j\ne i}\omega_j^2}$, which is smooth on the chart domain. Each $K_{i,\varepsilon}$ is closed and bounded in $\mathbb R^3$, hence compact by [F4], and their relative interiors cover because $\max_i|\omega_i|\ge1/\sqrt3>1/2$. For any smooth angular chart $y$ and nonempty compact $K$ in its domain, its radial extension $\widetilde y(x)=y(x/|x|)$ is smooth on the corresponding open cone. Its Cartesian first derivatives at $\omega\in K$ are continuous and hence bounded by [F4]. The homogeneity identity $\widetilde y(sx)=\widetilde y(x)$ holds for every $s>0$ and $x$ in the cone. Differentiating it with respect to $x$ and $s$ by the chain rule gives $\partial_i\widetilde y(r\omega)=r^{-1}\partial_i\widetilde y(\omega)$ and $\sum_i\omega_i\partial_i\widetilde y(r\omega)=0$. Thus $|\partial_i y^A|\le C_K/r$ and the Euclidean radial-angular contraction vanishes. For finitely many $K_\alpha$ take the maximum of their constants. [given, F4, construct, algebra]

2.1 Since $\partial_i r=x^i/r$ and step 1.2 bounds the angular derivatives uniformly on each prescribed compact chart subset, the inverse components in $(t,r,y^A)$ satisfy $g_q^{tr}=d_q^{-1}a^{-1}O(r^{-2})$, $g_q^{rr}=a^{-2}(1+O(r^{-1}))$, $g_q^{tA}=d_q^{-1}a^{-1}O(r^{-3})$, and $g_q^{rA}=a^{-2}O(r^{-2})$. For the last estimate, the leading Euclidean radial-angular contraction vanishes. The angular metric is positive definite for sufficiently large $r$ by [F1]. Its normal covectors are therefore precisely the linear combinations of $dt$ and $dr$. [given, F1, F4, step 1.1, step 1.2, algebra]

3.1 Set $c=d_q/4$. For the normal covector $-c\,dt+b\,dr$, nullity is $c^2g_q^{tt}-2cbg_q^{tr}+b^2g_q^{rr}=0$. The discriminant is positive, and the root $b=c(g_q^{tr}+\sqrt{(g_q^{tr})^2-g_q^{tt}g_q^{rr}})/g_q^{rr}$ has raised radial component $L_q^r=-cg_q^{tr}+bg_q^{rr}=c\sqrt{(g_q^{tr})^2-g_q^{tt}g_q^{rr}}>0$. Since $T$ is future timelike and $g_q(T,L_q)=-c<0$, this branch is future-directed; its positive radial component selects outward. Substituting the estimates from steps 1.1 and 2.1 and $a^{-1}r^{-2}=O(r^{-1})$ gives $L_q^r=1+O(r^{-1})$ and $b=a^2(1+O(r^{-1}))$. [given, F2, F3, step 1.1, step 2.1, algebra]

4.1 Nullity also gives $L_q^t(L_q)_t+L_q^r(L_q)_r=0$, because the angular covector components vanish. Thus $L_q^t=(4/d_q)L_q^r(L_q)_r=(4/d_q)a^2(1+O(r^{-1}))$. Moreover $L_q^A=-c g_q^{tA}+b g_q^{rA}=O(a^{-1}r^{-3})+O(r^{-2})=O(r^{-2})$. All constants remain uniform in $q$ and on the prescribed compact chart subsets by [F2], step 1.2 and $a\ge r^{-1}$. [given, F2, step 1.2, step 2.1, step 3.1, algebra]

5.1 For tangent fields $X,Y$ on the sphere, metric compatibility and torsion-freeness give $(\mathcal L_{L_q}g_q)(X,Y)=g_q(\nabla_XL_q,Y)+g_q(X,\nabla_YL_q)$. The trace in the positive induced metric is twice the trace of $\chi_{L_q}$ in [F3]. This also shows independence of the chosen smooth extension, since tangential derivatives of two extensions agreeing on the sphere agree there. Hence the stated expansion identity holds. [given, F3, step 2.1, algebra] ∎

## Source notes

The article citation attributes the original calculation. The argument above uses the completed component and denominator estimates and the stated geometric definitions; the article's assertion is not used as a premise.

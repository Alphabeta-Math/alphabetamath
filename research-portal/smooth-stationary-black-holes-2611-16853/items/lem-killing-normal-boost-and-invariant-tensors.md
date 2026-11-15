---
id: lem-killing-normal-boost-and-invariant-tensors
title: Normal boost action and invariant two-forms at a fixed surface
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-bifurcate-killing-horizon-data
  - def-circle-action-and-invariant-normal-data
  - physics:def-gr-metric-selected-connection
  - math:def-local-and-global-flow
  - math:thm-unique-maximal-integral-curve-through-each-point
  - math:def-pullback-of-a-differential-form
  - math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle
  - math:def-axiom-of-choice
dependency_roles:
  def-bifurcate-killing-horizon-data: mathematical-premise
  def-circle-action-and-invariant-normal-data: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  math:thm-unique-maximal-integral-curve-through-each-point: mathematical-premise
  math:def-pullback-of-a-differential-form: mathematical-premise
  math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Let $(M,g,N)$ be a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$, with Levi–Civita connection $\nabla$. Let $S$ be a smooth embedded spacelike two-surface and let $K$ be a smooth Killing field that vanishes on $S$. Write $\Phi_t$ for its local flow. At each $p\in S$, suppose that the map $B_p:v\mapsto\nabla_vK$ restricts to the normal plane $(T_pS)^\perp$ and has matrix $\kappa_p\begin{pmatrix}0&1\\1&0\end{pmatrix}$ in an orthonormal normal basis $(e_0,e_1)$, where $e_0$ is future timelike, $e_1$ is the chosen outward spacelike normal, and $\kappa_p>0$.

Then $\Phi_t(p)=p$ whenever the local flow is defined at $(t,p)$, and its differential is the identity on $T_pS$ and the Lorentz boost with matrix $\begin{pmatrix}\cosh(\kappa_pt)&\sinh(\kappa_pt)\\\sinh(\kappa_pt)&\cosh(\kappa_pt)\end{pmatrix}$ on the normal plane. If a smooth two-form $F$ is invariant under the local flow, meaning $\Phi_t^*F=F$ wherever both sides are defined, then $F_p(v,X)=0$ for every normal vector $v$ and every $X\in T_pS$.

Suppose additionally that a smooth $2\pi$-periodic flow $\phi_s$ of isometries preserves $S$ and future cones, and that $n$ is a smooth future timelike normal field along $S$. Its average $\bar n_p=(2\pi)^{-1}\int_0^{2\pi}d\phi_s|_{\phi_{-s}(p)}n_{\phi_{-s}(p)}\,ds$ is a smooth future timelike normal field. The normalized field $\widehat n=\bar n/\sqrt{-g(\bar n,\bar n)}$ is future unit timelike, normal to $S$, and invariant under $\phi_s$.

## Statement references

[[def-bifurcate-killing-horizon-data]]

[[def-circle-action-and-invariant-normal-data]]

[[physics:def-gr-metric-selected-connection]]

[[math:def-local-and-global-flow]]

[[math:def-pullback-of-a-differential-form]]

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice: every set-indexed family of nonempty sets has a choice function. Restricting to countably indexed families supplies countable choice. This assumption is used here in the inherited smooth-manifold, tangent-bundle and smooth-field conventions of F1, F3 and F4; the local boost, two-form and averaging calculations require no additional choice principle. [[math:def-axiom-of-choice]]

[F1] A spacelike surface has positive definite induced metric; the Killing-field and time-oriented Lorentzian conventions are those of the bifurcate-horizon definition. [[def-bifurcate-killing-horizon-data]]

[F2] A local flow consists of integral curves and obeys the local flow law. Integral curves through a given point are unique on their common domain. [[math:def-local-and-global-flow]] [[math:thm-unique-maximal-integral-curve-through-each-point]]

[F3] The Levi–Civita connection is an affine connection; in coordinates, $\nabla_vK$ is the ordinary directional derivative of the components of $K$ plus a connection term linear in $K$. [[physics:def-gr-metric-selected-connection]]

[F4] The smooth-field, normality and time-orientation conventions are those of the circle-action definition. For the arbitrary smooth $2\pi$-periodic flow in the Statement, interpret its displayed average componentwise in any fixed basis of $T_pM$, using scalar Riemann integrals, and call a field $u$ along $S$ invariant when $d\phi_t|_pu_p=u_{\phi_t(p)}$ for every $p\in S$ and $t\in\mathbb R$. The integral is basis independent because a change-of-basis matrix is constant in the integration variable and scalar integration is linear. These local definitions impose no least-period condition. [[def-circle-action-and-invariant-normal-data]]

[F5] A smooth two-form is a smooth alternating covariant two-tensor. For a smooth map $f$ and a smooth two-form $F$ on its target, the pullback is given by $(f^*F)_p(u,v)=F_{f(p)}(df|_pu,df|_pv)$. [[math:def-pullback-of-a-differential-form]]

[F6] Let $a<b$ and $c<d$. If $f,h:[a,b]\times[c,d]\to\mathbb R$ are continuous and $\partial_xf(x,s)=h(x,s)$ for every $x\in(a,b)$ and $s\in[c,d]$, then $G(x)=\int_c^d f(x,s)\,ds$ is differentiable on $[a,b]$ with $G^{\prime}(x)=\int_c^d h(x,s)\,ds$; at the endpoints the derivatives are relative and one-sided. [[math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle]]

## Proof

**Given:** The manifold, surface, fields, flows, and hypotheses in the Statement, with the set-theoretic convention A1 for the inherited smooth structures and fields.

**Goal:** Establish the boost, mixed-component vanishing, and normalized invariant normal.

1.1 For $p\in S$, the constant curve at $p$ is an integral curve of $K$ because $K_p=0$. Uniqueness makes $\Phi_t(p)=p$ throughout the interval on which the flow at $p$ is defined. Since the flow fixes every point of $S$, differentiating its restriction to $S$ gives $d\Phi_t|_pX=X$ for $X\in T_pS$. [F2, given]

1.2 For the circle average, the flow law makes $\phi_s$ a diffeomorphism with inverse $\phi_{-s}$. Because it preserves $S$ and $g$, each transported vector in the integrand is normal to $S$ at $p$; it is future timelike by the stated cone preservation. In a future orthonormal frame at $p$, each such vector has time component $a(s)>|b(s)|$, where $b(s)$ denotes its spatial components. Continuity on $[0,2\pi]$ gives a positive minimum of $a(s)-|b(s)|$; the triangle inequality for integrals therefore gives $\bar a>|\bar b|$. Thus the average is future timelike and, by linearity, normal. [F1, F4, given, algebra]

1.3 Put $V(s,p)=d\phi_s|_{\phi_{-s}(p)}n_{\phi_{-s}(p)}$. Smoothness of the action and $n$ makes the components $V^a(s,x)$ smooth jointly in $s$ and the slice coordinates $x$ on $S$, with the output expressed in one ambient chart around $p$; the moving source point can use different charts. Choose a closed coordinate rectangle $Q$ contained in this slice chart, with $p$ in its interior. On $[0,2\pi]\times Q$ all derivatives of $V^a$ are continuous. Fixing the other coordinates, apply F6 on a compact rectangle in $(x_i,s)$, and repeat for every partial derivative. For each multi-index $\alpha$ this gives $\partial_x^\alpha\bar n^a(x)=(2\pi)^{-1}\int_0^{2\pi}\partial_x^\alpha V^a(s,x)\,ds$ in the interior of $Q$. These derivatives are continuous: their difference at $x,y$ is bounded in absolute value by $\sup_{s\in[0,2\pi]}|\partial_x^\alpha V^a(s,x)-\partial_x^\alpha V^a(s,y)|$, which tends to zero as $y\to x$ by uniform continuity on the compact rectangle. Hence $\bar n$ is smooth near each $p$. [F4, F6, given, algebra]

2.1 Fix $p\in S$ and put $A(t)=d\Phi_t|_p$. Differentiating the flow law at the fixed point gives $A(t+h)=A(h)A(t)$ whenever the times are admissible. In a coordinate chart, differentiating the flow equation at $t=0$ in the initial point gives $A'(0)=DK_p$. The connection term in $\nabla_vK$ vanishes at $p$ because $K_p=0$, so $A'(0)=B_p$. It follows from the flow law that $A'(t)=B_pA(t)$ and $A(0)=I$. [step 1.1, F2, F3]

3.1 The positive definite induced metric gives the direct sum $T_pM=T_pS\oplus(T_pS)^\perp$. Differentiating $A(t)X=X$ from step 1.1 at zero and using step 2.1 gives $B_pX=0$ for $X\in T_pS$. On the normal plane, the stated matrix of $B_p$ has square $\kappa_p^2I$. Let $C(t)$ be the displayed hyperbolic matrix on that plane and extend it to $\widetilde C(t)$ on $T_pM$ by the identity on $T_pS$. Since $B_p$ preserves the normal plane and vanishes on $T_pS$, direct block-matrix differentiation gives $\widetilde C(0)=I$, $\widetilde C^{\prime}(t)=B_p\widetilde C(t)=\widetilde C(t)B_p$, and $\widetilde C(-t)\widetilde C(t)=I$. Thus the full-space product satisfies $\frac{d}{dt}(\widetilde C(-t)A(t))=-\widetilde C(-t)B_pA(t)+\widetilde C(-t)B_pA(t)=0$. Its value at zero is $I$, so $A(t)=\widetilde C(t)$ on the interval of definition. In particular, $A(t)$ preserves the normal plane, where it equals $C(t)$, and is the identity on $T_pS$. [F1, step 1.1, step 2.1, given, algebra]

4.1 Set $v_+=e_0+e_1$ and $v_-=e_0-e_1$. Step 3.1 gives $A(t)v_\pm=e^{\pm\kappa_pt}v_\pm$. For $X\in T_pS$, invariance of $F$, the pullback rule and step 1.1 give $F_p(v_\pm,X)=(\Phi_t^*F)_p(v_\pm,X)=F_p(A(t)v_\pm,A(t)X)=e^{\pm\kappa_pt}F_p(v_\pm,X)$. The flow domain contains an interval about zero, so a nonzero admissible $t$ exists; since $\kappa_p>0$, each exponential factor differs from one. Thus both values vanish, and $v_+,v_-$ span the normal plane. [step 1.1, step 3.1, F5, given, algebra]

5.1 The flow law gives $d\phi_t|_pV(s,p)=V(s+t,\phi_t(p))$. The integrand $V$ is $2\pi$-periodic in $s$, so substitution $u=s+t$ in its full-period integral gives $d\phi_t|_p\bar n_p=\bar n_{\phi_t(p)}$. This uses only $2\pi$-periodicity, so shorter common periods and the identity flow are included. The denominator in the normalization is smooth and strictly positive by step 1.2, and is preserved by the isometries. Consequently $\widehat n$ is smooth, future unit timelike, normal, and invariant. [step 1.2, step 1.3, F2, F4, given, algebra] ∎

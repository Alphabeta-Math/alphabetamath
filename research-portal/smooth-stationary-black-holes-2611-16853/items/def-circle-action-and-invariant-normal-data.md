---
id: def-circle-action-and-invariant-normal-data
title: Periodic isometries and invariant normal averaging
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - math:def-local-and-global-flow
  - math:def-embedded-submanifold-and-slice-chart
  - physics:def-gr-smooth-lorentzian-objects
  - physics:lem-timelike-cone-has-two-convex-components
  - math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle
  - math:def-axiom-of-choice
  - math:def-differential-of-a-smooth-map
  - math:def-pullback-of-a-covariant-tensor-field
  - math:thm-coordinate-formula-for-the-differential
  - math:thm-chain-rule-for-differentials-of-smooth-maps
  - math:thm-continuous-implies-integrable
  - math:thm-darboux-equals-riemann
  - math:cor-triangle-inequality-for-inner-product-norm
  - math:lem-extreme-value-theorem-from-compactness
  - math:thm-heine-cantor-metric
dependency_roles:
  math:def-local-and-global-flow: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:lem-timelike-cone-has-two-convex-components: mathematical-premise
  math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-differential-of-a-smooth-map: mathematical-premise
  math:def-pullback-of-a-covariant-tensor-field: mathematical-premise
  math:thm-coordinate-formula-for-the-differential: mathematical-premise
  math:thm-chain-rule-for-differentials-of-smooth-maps: mathematical-premise
  math:thm-continuous-implies-integrable: mathematical-premise
  math:thm-darboux-equals-riemann: mathematical-premise
  math:cor-triangle-inequality-for-inner-product-norm: mathematical-premise
  math:lem-extreme-value-theorem-from-compactness: mathematical-premise
  math:thm-heine-cantor-metric: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 0
---

## Definition

Work in ZFC. Let $(M,g,N)$ be a time-oriented smooth Lorentzian four-manifold of signature $(-,+,+,+)$: $N$ is a smooth timelike field, and a timelike vector $v$ is future-directed when $g(v,N)<0$. A **normalized circle action by isometries** is a smooth global flow $\phi:\mathbb R\times M\to M$ of a smooth vector field $Z$, with $\phi_{s+2\pi}=\phi_s$ for all $s$, such that $2\pi$ is the least positive common period and $\phi_s^*g=g$ for every $s$. The **generator** is $Z_p=\left.\frac{d}{ds}\right|_{s=0}\phi_s(p)$. A **fixed point** is a point $p$ for which $\phi_s(p)=p$ for every $s$; consequently $Z_p=0$. The least-period condition concerns the whole action, so individual orbits may have shorter periods or be fixed.

Let $S\subseteq M$ be an embedded submanifold invariant under the action, meaning $\phi_s(S)=S$ for all $s$. A **smooth field along $S$** is an assignment $p\mapsto n_p\in T_pM$ such that, in every ambient slice chart $(U,x)$ with $S\cap U$ given by $x^{k+1}=\cdots=x^4=0$, the coefficients in $n_p=\sum_{a=1}^4 n^a(p)\partial_{x^a}|_p$ are smooth functions of the slice variables $(x^1,\ldots,x^k)$. Such a field is **normal** when $g_p(n_p,v)=0$ for every $p\in S$ and $v\in T_pS$. Suppose $n$ is future timelike at every point. Define its **circle average** and **normalized invariant normal** by

$$\bar n_p=\frac1{2\pi}\int_0^{2\pi}d\phi_s|_{\phi_{-s}(p)}\bigl(n_{\phi_{-s}(p)}\bigr)\,ds,\qquad \widehat n_p=\frac{\bar n_p}{\sqrt{-g_p(\bar n_p,\bar n_p)}}.$$

Here $d\phi_s|_q:T_qM\to T_{\phi_s(q)}M$ is the differential. The isometry condition uses tensor pullback: $(\phi_s^*g)_q(u,v)=g_{\phi_s(q)}(d\phi_s|_q u,d\phi_s|_q v)$. The integral is taken in the fixed finite-dimensional vector space $T_pM$: for a continuous curve $v(s)=\sum_{a=1}^4v^a(s)e_a$ in any fixed basis, set $\int_0^{2\pi}v(s)\,ds=\sum_{a=1}^4(\int_0^{2\pi}v^a(s)\,ds)e_a$, using scalar Riemann integrals. An invariant field along $S$ is one satisfying $d\phi_t|_p(v_p)=v_{\phi_t(p)}$ for all $p\in S$ and $t\in\mathbb R$. The construction assumes the supplied field $n$; it asserts no existence of such a field.

## Definition references

[[math:def-axiom-of-choice]]

[[physics:def-gr-smooth-lorentzian-objects]]

[[math:def-local-and-global-flow]]

[[math:def-embedded-submanifold-and-slice-chart]]

[[math:def-differential-of-a-smooth-map]]

[[math:def-pullback-of-a-covariant-tensor-field]]

[[math:thm-continuous-implies-integrable]]

## Justification

Every continuous scalar component on a closed finite interval is bounded and Riemann integrable. The tagged-sum characterization identifies the coordinatewise vector integral with the limit of the vector sums $\sum_i v(\xi_i)\Delta_i$ as the mesh tends to zero. A fixed linear map commutes with this limit: its matrix acts by finite sums of constant multiples of convergent scalar components. Applying this to a change-of-basis matrix proves that the integral is independent of the chosen basis; applying it to any linear functional or differential proves commutation with that map. Scalar order inequalities pass to the limit from the positive-weight sums. Likewise, the finite-sum triangle inequality gives $|\int w(s)\,ds|\le\int|w(s)|\,ds$ for a continuous Euclidean-vector-valued $w$. All these scalar integrands are continuous, so their integrability is supplied. These sum arguments also give $|\int h|\le(b-a)\sup|h|$ on $[a,b]$. Translating tagged partitions proves invariance under translation of the integration variable, and joining tagged partitions at a split point proves additivity across that point; the componentwise construction carries both properties to vector integrals. [[math:thm-continuous-implies-integrable]] [[math:thm-darboux-equals-riemann]] [[math:cor-triangle-inequality-for-inner-product-norm]]

The coordinate formula for the differential shows that the slice-coordinate definition of smoothness is unchanged on overlaps: the new components are the old components multiplied by the smooth Jacobian matrix of the chart transition. It also shows that $v(s,p):=d\phi_s|_{\phi_{-s}(p)}n_{\phi_{-s}(p)}$ has smooth components jointly in $(s,p)$. This is local near each $(s,p)$; the moving source point may use different charts for different $s$, while the output is expressed in one chart around $p$. The flow law and differential chain rule make each $\phi_s$ a diffeomorphism with inverse $\phi_{-s}$, and its restriction to $S$ maps tangent spaces onto tangent spaces. For $q=\phi_{-s}(p)$ and $X\in T_pS$, the pullback formula gives $g_p(v(s,p),X)=g_q(n_q,d\phi_{-s}|_pX)=0$. The integrand at $s=0$ is $n_p$. As $s$ varies continuously, $v(s,p)$ is timelike by isometry and remains in the same timelike component as $n_p$, hence in the future cone. Commutation with the linear functional $g_p(\cdot,X)$ makes $\bar n_p$ normal. [[math:thm-coordinate-formula-for-the-differential]] [[math:def-differential-of-a-smooth-map]] [[math:thm-chain-rule-for-differentials-of-smooth-maps]] [[math:def-pullback-of-a-covariant-tensor-field]] [[math:def-local-and-global-flow]] [[math:def-embedded-submanifold-and-slice-chart]] [[physics:def-gr-smooth-lorentzian-objects]]

In a future-oriented orthonormal basis at $p$, write $v(s,p)=(a(s),b(s))$ with $b(s)\in\mathbb R^3$. The future-cone description gives $a(s)>|b(s)|$. The continuous positive function $a(s)-|b(s)|$ attains a positive minimum $\delta_p$ on $[0,2\pi]$. The integral order and norm inequalities just established give $(2\pi)^{-1}\int a\ge(2\pi)^{-1}\int|b|+\delta_p\ge|(2\pi)^{-1}\int b|+\delta_p$. Hence $\bar n_p$ is future timelike, the positive square root in the normalization exists, and $g(\widehat n,\widehat n)=-1$. No uniform lower bound in $p$ is required. [[physics:lem-timelike-cone-has-two-convex-components]] [[math:lem-extreme-value-theorem-from-compactness]] [[math:thm-darboux-equals-riemann]] [[math:cor-triangle-inequality-for-inner-product-norm]]

On a compact coordinate rectangle in $S$, repeated differentiation under the integral sign, one slice variable at a time, shows that every partial derivative of the components of $\bar n$ is the integral of the corresponding derivative of $v(s,p)$. The derivatives of the integrand are continuous, hence uniformly continuous, on the rectangle times $[0,2\pi]$, and their integrals are continuous: a uniform change of at most $\varepsilon$ in a component changes its integral by at most $2\pi\varepsilon$, by the sum bound above. Thus $\bar n$ is smooth. Since $-g(\bar n,\bar n)$ is a smooth positive function, its positive square root and the normalized field are smooth as well. [[math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle]] [[math:thm-heine-cantor-metric]] [[math:thm-coordinate-formula-for-the-differential]] [[physics:def-gr-smooth-lorentzian-objects]]

For $p'=\phi_t(p)$, commutation of a fixed differential with integration and the flow chain rule give $d\phi_t|_p\bar n_p=(2\pi)^{-1}\int_0^{2\pi}v(s+t,p')\,ds$. To see that a full-period integral is independent of its starting point, reduce $t$ modulo $2\pi$ to $r\in[0,2\pi)$, split the interval $[r,r+2\pi]$ at $2\pi$, and translate its second piece by $-2\pi$; periodicity identifies that piece with $[0,r]$. The integral therefore equals $\bar n_{p'}$. Isometry preserves the normalization factor, so $\widehat n$ is invariant too. [[math:thm-chain-rule-for-differentials-of-smooth-maps]] [[math:def-local-and-global-flow]] [[math:thm-darboux-equals-riemann]] [[math:def-pullback-of-a-covariant-tensor-field]]

The ZFC convention includes the choice assumptions inherited from the stated manifold interface. [[math:def-axiom-of-choice]]

---
title: Asymptotically flat positive-q ends and cylindrical limit
status: draft
research_item: pthm-transformed-end-geometries
dependency_level: 10
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 6, Section 1.4; page 12, equation (3.1)
      hypotheses: The article's mass-one stationary vacuum construction, with its
        normalized Ernst potential, pole and transformed metric.
      reading_limits: Consulted the frozen article text and PDF images at pages 6 and
        12. This reference attributes the original claims only. The conditional
        proof uses the declared component and denominator suppliers, published
        mathematical interfaces, and the local coordinate and volume-comparison
        arguments; it does not assume the article conclusions.
---

PDF p. 6: ` §1.4 `; PDF p. 12: ` equation (3.1) `

## Prerequisites

- [pthm-harrison-component-asymptotics](item-pthm-harrison-component-asymptotics)
- [pthm-harrison-denominator-asymptotics](item-pthm-harrison-denominator-asymptotics)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-harrison-one-form-family](item-def-harrison-one-form-family)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:prop-round-sphere-model-geometry](https://alphabetamath.cc/item/prop-round-sphere-model-geometry)
- [math:ex-sphere-and-hemisphere-surface-integrals](https://alphabetamath.cc/item/ex-sphere-and-hemisphere-surface-integrals)
- [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)
- [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density)
- [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)
- [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)
- [physics:def-gr-fx-adm-end](https://alphabetamath.cc/physics/item/def-gr-fx-adm-end)
- [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules)
- [math:cor-volume-of-a-closed-three-ball](https://alphabetamath.cc/item/cor-volume-of-a-closed-three-ball)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [def-harrison-one-form](item-def-harrison-one-form)
- [def-killing-ernst-notation](item-def-killing-ernst-notation)
- [math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula)
- [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)
- [pthm-ernst-and-one-form-decay](item-pthm-ernst-and-one-form-decay)
- [pthm-harrison-coordinate-components](item-pthm-harrison-coordinate-components)




## Statement

Work in the inherited ZFC setting, including the Axiom of Choice. Adopt the stationary vacuum model and regular stationary spacetime data with a mass-one stationary Cartesian end $(t,x^i)$, $T=\partial_t$, and $r=|x|$. Assume also that the original smooth spacelike maximal exterior section $\Sigma_1$ is supplied, with end coordinates $x^i$ and an ADM mass limit that exists and equals one, as required by the mass-one normalization. Use the supplied normalized Ernst potential $\sigma$, pole $p$ with $T_p=0$, and Harrison one-form family with the radial choice required by the component estimates. Put $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $d_q=D_q(p)$, and use the corresponding transformed metric $g_q$ for $q\in[0,1]$ on the sufficiently distant end.

For every $q>0$ set $t_q=d_qt/(4q)$, $x_q^i=qx^i$ and $r_q=|x_q|=qr$. In these coordinates, with index $0$ denoting $t_q$,
$$(g_q)_{00}=-1+O_5(r_q^{-1}),\qquad (g_q)_{0i}=O_5(r_q^{-2}),\qquad (g_q)_{ij}=\delta_{ij}+O_5(r_q^{-1}).$$
Here $O_5(r_q^{-k})$ means that spatial Cartesian derivatives of order $|\beta|\le5$ are bounded by $C_\beta r_q^{-k-|\beta|}$. For any fixed $\delta\in(0,1]$, the constants and one end radius can be chosen uniformly for $q\in[\delta,1]$; they may depend on $\delta$. The region $r_q\ge R$ is exactly $r\ge R/q$, and therefore recedes in the original coordinates as $q\downarrow0$ for fixed $R>0$. These component bounds express asymptotic flatness in the stated stationary end chart.

At $q=0$, the induced metric on each constant-$t$ section of the distant end is asymptotic to $ds^2+\gamma_{\mathbb S^2}$ in the coordinates $s=\log r$ and $\omega=x/r$: its components and their derivatives through order five in $s$ and smooth angular charts differ from those of this product by $O(e^{-s})$. Here $\gamma_{\mathbb S^2}$ is the unit round metric induced by the Euclidean inner product on $\mathbb S^2=\{\omega\in\mathbb R^3:|\omega|=1\}$. Thus these sections have a cylindrical end, rather than an asymptotically Euclidean end, and the areas of their coordinate spheres tend to $4\pi$.

For this comparison, an asymptotically Euclidean spatial end means a neighborhood of the same infinity admitting an exterior chart $y$, $|y|>R_0$, in which $h_{ij}(y)=\delta_{ij}+o(1)$ uniformly in angle as $|y|\to\infty$. This metric condition is necessary, in particular, for a fixed-chart asymptotically Euclidean ADM end; no ADM mass convergence or special leading expansion is asserted here.

For an additional positive-parameter case, assume also that the specified exterior section $\Sigma_0\cap\mathcal E$ of the regular-spacetime data is maximal for the original metric $g$. This maximality is a hypothesis on that specified physical section; no identification with the supplied maximal section $\Sigma_1$ above is assumed. Replace the radial-choice requirement above by the smooth global primitive supplied by [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form), with its pole and normalization and under its additional standing hypothesis $T|_S\not\equiv0$. Then the same positive-$q$ normalized component estimates, uniformity on every $[\delta,1]$ and recession statement hold. This additional positive-parameter conclusion requires only its spatial bounds $(W_0)_i=O_5(r^{-3})$, not equality with the exact radial integral. The zero-parameter cylindrical conclusions above retain the radial-choice hypotheses already stated.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-harrison-normalization](item-def-harrison-normalization)

[def-harrison-one-form-family](item-def-harrison-one-form-family)

[def-harrison-one-form](item-def-harrison-one-form)

[def-killing-ernst-notation](item-def-killing-ernst-notation)

[math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[pthm-harrison-denominator-asymptotics](item-pthm-harrison-denominator-asymptotics)

[pthm-harrison-component-asymptotics](item-pthm-harrison-component-asymptotics)

[math:prop-round-sphere-model-geometry](https://alphabetamath.cc/item/prop-round-sphere-model-geometry)

[math:ex-sphere-and-hemisphere-surface-integrals](https://alphabetamath.cc/item/ex-sphere-and-hemisphere-surface-integrals)

[math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)

[math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density)

[math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)

[math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)

[physics:def-gr-fx-adm-end](https://alphabetamath.cc/physics/item/def-gr-fx-adm-end)

[math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

[math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules)

[math:cor-volume-of-a-closed-three-ball](https://alphabetamath.cc/item/cor-volume-of-a-closed-three-ball)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[A1] The regular data are formulated in ZFC, so the Axiom of Choice and hence Countable Choice are available for the round-sphere and volume-measure interfaces below. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) The stated model and regular data supply the mass-one stationary end and the specified stationary chart; the normalization and one-form definitions specify the conditional potential, pole, denominator and selected family. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-harrison-normalization](item-def-harrison-normalization) [def-harrison-one-form-family](item-def-harrison-one-form-family)

[A2] The original smooth spacelike maximal exterior section $\Sigma_1$ is supplied, and the ADM mass limit of its end in the stated coordinates $x^i$ exists and equals one. These are assumed section and normalization data, not existence or mass-convergence conclusions. [def-harrison-normalization](item-def-harrison-normalization) [pthm-harrison-component-asymptotics](item-pthm-harrison-component-asymptotics)

[F1] For the stated data and radial choice, the denominator estimate gives $d_q$ bounded above and below by positive constants uniformly on $[0,1]$, and $D_q>0$ on a common sufficiently distant end. [pthm-harrison-denominator-asymptotics](item-pthm-harrison-denominator-asymptotics)

[F2] On that end, with $a=q+r^{-1}$ and $B=a^2r^{-1}$, the component estimates give $(g_q)_{00}=-d_q^2/(16a^2)+a^{-4}O_5(B)$, $(g_q)_{0i}=d_qa^{-1}O_5(r^{-2})$, and $(g_q)_{ij}=a^2\delta_{ij}+O_5(B)$, uniformly for $q\in[0,1]$. The weighted derivative notation is the one specified in the supplier. [pthm-harrison-component-asymptotics](item-pthm-harrison-component-asymptotics) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F3] The unit round sphere is the compact sphere with its induced Euclidean metric; it has diameter $\pi$, and its area is $4\pi$. The round-sphere supplier's Countable Choice premise follows from [A1]. [math:prop-round-sphere-model-geometry](https://alphabetamath.cc/item/prop-round-sphere-model-geometry) [math:ex-sphere-and-hemisphere-surface-integrals](https://alphabetamath.cc/item/ex-sphere-and-hemisphere-surface-integrals)

[F4] A positive-definite metric $h$ has coordinate density $\mu_h=\sqrt{\det(h_{ab})}|dz^1\cdots dz^n|$; this gives surface area when $n=2$ and volume when $n=3$. Under the inherited Countable Choice, its Riemannian volume measure is the Radon measure of this density, and metric balls are Borel. Riemannian length integrates $\sqrt{h(\dot c,\dot c)}$ along piecewise $C^1$ curves, and intrinsic distance is the infimum of these lengths with the curves confined to the specified connected end. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density) [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length) [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)

[F5] Pulling back a covariant tensor evaluates it on the differentials of the coordinate map. The total-derivative chain rule and the coordinate-line product and quotient rules apply repeatedly to the smooth coordinate maps and component functions used below. [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules)

[F6] The published fixed-chart ADM-end definition requires $h_{ij}=\delta_{ij}+a_{ij}/|y|+O_2(|y|^{-1-\epsilon})$, with constant $a_{ij}$ and $\epsilon>0$, as well as a separate condition on $K$. Its metric therefore satisfies the weaker metric condition specified in the Statement. The argument below excludes even that weaker condition in every chart representing this same infinity; it does not infer the stronger ADM expansion from the positive-$q$ estimates. [physics:def-gr-fx-adm-end](https://alphabetamath.cc/physics/item/def-gr-fx-adm-end)

[F7] A Euclidean three-ball of radius $L$ has volume $4\pi L^3/3$. [math:cor-volume-of-a-closed-three-ball](https://alphabetamath.cc/item/cor-volume-of-a-closed-three-ball)

[F8] The supplied normalized primitive satisfies $dW_0=\Theta_0=4((f-1)F+\psi\star_gF)$ and $W_0(T)=d_0-D_0$, and its family is $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. The family definition's local contraction calculation gives $W_q(T)=d_q-D_q$. [def-harrison-one-form-family](item-def-harrison-one-form-family) The Ernst interface uses the torsion-free metric-compatible connection, $F_{ab}=\nabla_aT_b$, and $d\sigma(X)=2(F+i\star_gF)(T,X)$; its local justification gives antisymmetry of $F$ and $T(\sigma)=0$. [def-killing-ernst-notation](item-def-killing-ernst-notation)

[F9] For a smooth one-form $\alpha$, exterior differentiation is $(d\alpha)(X,Y)=X(\alpha(Y))-Y(\alpha(X))-\alpha([X,Y])$. [math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula) The Harrison one-form interface requires stationarity, $dW_q=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$, and $W_q(T)=d_q-D_q$. Its corresponding metric is $g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q)$ on $D_q>0$. [def-harrison-one-form](item-def-harrison-one-form)

[F10] For the additional case, the specified exterior section $\Sigma_0\cap\mathcal E$ of the regular-spacetime data is assumed maximal for $g$; this does not identify it with $\Sigma_1$. Together with the regular stationary vacuum model, mass one and $T|_S\not\equiv0$, this matches the hypotheses of the global primitive theorem. Use that theorem's supplied pole and normalization, in the unchanged original stationary chart. It supplies one smooth stationary $W_0$ with $(W_0)_i=O_5(r^{-3})$ and the normalized contraction. [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form) The mass-one Ernst estimate gives $f=1-2/r+O_6(r^{-2})$ and $\psi=O_6(r^{-2})$, independently of which primitive is chosen. [pthm-ernst-and-one-form-decay](item-pthm-ernst-and-one-form-decay) For a supplied Harrison one-form the exact original-chart metric components are those of the component-identity theorem; no radial-gauge condition is imposed by that theorem. [pthm-harrison-coordinate-components](item-pthm-harrison-coordinate-components)

## Proof

**Given:** The model, end, supplied original maximal exterior section and its existing ADM mass-one limit, pole, potential, selected one-form and transformed metrics in the Statement. In the additional case also assume maximality of the specified exterior section, as stated in [F10].

**Goal:** Prove the normalized positive-$q$ bounds and the zero-$q$ cylindrical spatial limit.

1.1 First verify the one-form hypotheses needed for the component estimates from the supplied primitive. Taking real and imaginary parts in [F8] gives $df(X)=2F(T,X)$ and $d\psi(X)=2(\star_gF)(T,X)$. Since $D_0=(1-f)^2+\psi^2$, it follows that $\Theta_0(T,X)=2((f-1)df(X)+\psi d\psi(X))=dD_0(X)$. In the stationary end chart the coordinate fields commute. With $(W_0)_0=W_0(T)=d_0-D_0$, [F9] therefore gives $\partial_t(W_0)_i=(dW_0)(T,\partial_i)+\partial_i(W_0)_0=\partial_iD_0-\partial_iD_0=0$. Also $T(\sigma)=0$ gives $\partial_t(W_0)_0=0$. Thus $W_0$ is stationary there. The Killing condition makes the components of $T^\flat$ independent of $t$, so the constant-coefficient family in [F8] is stationary for every fixed $q$. [given, A1, F8, F9, algebra]

2.1 The torsion-free metric-compatible connection in [F8] satisfies $\nabla_XY-\nabla_YX=[X,Y]$. Expanding [F9] for $T^\flat$ consequently gives $(dT^\flat)(X,Y)=g(\nabla_XT,Y)-g(\nabla_YT,X)=F(X,Y)-F(Y,X)=2F(X,Y)$. The same exterior-derivative formula is real-linear in the one-form. For fixed $q$ its coefficients are constant, so $dW_q=4(1-q)^2((f-1)F+\psi\star_gF)-8q(1-q)F=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$. The contraction identity is already established in [F8]. Together with step 1.1 these are exactly the conditions in [F9]; the corresponding transformed metric in the Statement is the metric specified there. The positivity domain is supplied by [F1]. Thus the one-form hypotheses of the component supplier are established before its estimates are used below, while the given radial choice and section data are retained. [given, A1, A2, F1, F8, F9, step 1.1, algebra]

3.1 Fix $\delta\in(0,1]$. For $q\in[\delta,1]$, the factors $a$, $a^{-1}$ and their spatial derivatives have bounds controlled by $\delta$, with each derivative gaining one power of $r^{-1}$. Since $a=q+r^{-1}$, [F2] gives $(g_q)_{00}=-(d_q/(4q))^2+O_5(r^{-1})$, $(g_q)_{0i}=O_5(r^{-2})$, and $(g_q)_{ij}=q^2\delta_{ij}+O_5(r^{-1})$, with a common radius and constants depending on $\delta$. For example, $a^{-2}-q^{-2}=-(2q/r+r^{-2})/(q^2a^2)$ has the required differentiated $O_5(r^{-1})$ bound. [given, F2, F5, step 2.1, algebra]

3.2 At $q=0$, [F2] gives $(g_0)_{ij}=r^{-2}\delta_{ij}+O_5(r^{-3})$. The error is smaller than the positive leading form for sufficiently large $r$, so a constant-$t$ section is spacelike there. With $x=r\omega$ and $s=\log r$, $r^{-2}\delta_{ij}dx^idx^j=ds^2+\gamma_{\mathbb S^2}$. Indeed $d x=r\omega\,ds+r\,d\omega$, and $\langle\omega,d\omega\rangle=0$ follows by differentiating $|\omega|^2=1$, so the leading form is exactly the product with the induced round metric in [F3]. On relatively compact angular charts in a finite cover of the sphere, every required derivative of $x=e^s\omega$ is $O(r)$. Each transformed error component has two coordinate-Jacobian factors. After at most five further derivatives, the chain and product rules express every term as a Cartesian derivative of order $j\le5$ of the error, bounded by $C r^{-3-j}$, times factors bounded by $C r^{j+2}$. Thus all these terms are $O(r^{-1})=O(e^{-s})$. This proves the cylindrical metric assertion. [given, F2, F3, F5, step 2.1, algebra]

3.3 For the additional global-choice conclusion fix $\delta>0$. The regular model in [A1], mass-one data in [A2], and maximality of the specified exterior section and $T|_S\not\equiv0$ in [F10] match the global primitive theorem's hypotheses. Apply it with its supplied pole and normalization in the original chart, as in [F10]. The primitive in F10 and its constant-coefficient family in F8 satisfy the one-form conditions by the local calculations in steps 1.1 and 2.1, which use no radial identity. For $q\in[\delta,1]$, the Ernst bounds in F10 give $D_q=4q^2+O_5(r^{-1})$, uniformly in $q$. On a common larger end $D_q\ge2\delta^2$. Repeated product and reciprocal differentiation using F5 gives $D_q^{-1}=(4q^2)^{-1}+O_5(r^{-1})$. Also $(W_q)_i=(1-q)^2(W_0)_i-4q(1-q)g_{0i}=O_5(r^{-2})$ uniformly. At the fixed pole, $d_q=(1+q)^2+(1-q)^2\psi(p)^2$, so $d_q$ and its reciprocal are bounded on $[\delta,1]$. Substitute these estimates into the exact identities in F10. They give $(g_q)_{00}=-d_q^2/(16q^2)+O_5(r^{-1})$, $(g_q)_{0i}=O_5(r^{-2})$ and $(g_q)_{ij}=q^2\delta_{ij}+O_5(r^{-1})$ for this same global primitive. Every derivative assertion follows by the finite coordinate product and reciprocal rules; constants may depend on $\delta$. [given, A1, A2, F5, F8, F9, F10, step 1.1, step 2.1, algebra]

4.1 By [F1], $d_q>0$, so the coordinate change is invertible. Its inverse Jacobian has $dt/dt_q=4q/d_q$ and $\partial x^i/\partial x_q^j=\delta^i_j/q$. Applying the tensor transformation law to step 3.1 gives the displayed leading coefficients. Each $x_q$ derivative contributes a factor $q^{-1}$, and $r=r_q/q$; all factors are uniformly bounded for $q\in[\delta,1]$. This proves the stated $O_5$ estimates on a common normalized end. The identity $r_q=qr$ gives the region correspondence and its recession. [given, F1, F2, F5, step 3.1, algebra]

4.2 Restricting the metric in step 3.2 to $s=\log R$ gives $\gamma_{\mathbb S^2}+O(R^{-1})$ in smooth angular charts. Relative to the positive round metric, the two eigenvalues are $1+O(R^{-1})$, uniformly over the compact sphere. By the determinant density in [F4], the area density is therefore $(1+O(R^{-1}))\mu_{\gamma_{\mathbb S^2}}$. Integrating and using [F3] gives sphere area $4\pi+O(R^{-1})$, proving the stated limit. [F3, F4, step 3.2, algebra]

4.3 Write $h$ for the zero-$q$ spatial metric and $h_c=ds^2+\gamma_{\mathbb S^2}$. Choose $s_0$ so large that on the connected end $E_c=(s_0,\infty)\times\mathbb S^2$ one has $h_c/2\le h\le2h_c$. Fix any $b=(s_b,\omega_b)\in E_c$. For every piecewise $C^1$ path from $b$ to $(s,\omega)$ confined to $E_c$, [F4] gives length at least $|s-s_b|/\sqrt2$. Thus its intrinsic ball $B_h^{E_c}(b,\rho)$ lies in $(s_0,s_b+\sqrt2\rho)\times\mathbb S^2$. The volume density is at most $2^{3/2}\mu_{h_c}$ and $\mu_{h_c}=ds\,\mu_{\gamma_{\mathbb S^2}}$, so $\operatorname{vol}_h B_h^{E_c}(b,\rho)\le2^{3/2}4\pi(s_b-s_0+\sqrt2\rho)$. This proves the linear upper bound without assuming a minimizing curve exists. [F3, F4, step 3.2, algebra]

5.1 Suppose the same infinity admitted the asymptotically Euclidean chart specified in the Statement. Truncate it to an end $E_A=\{|y|>A\}$ lying in $E_c$, with $\delta/2\le h\le2\delta$ there. Fix $b'$ with $|y(b')|=2A$. Any $y$ with $2A\le|y|\le L$ can be reached from $b'$ by a spherical arc at radius $2A$ followed by a radial segment, all in $E_A$. By [F3], the Euclidean spherical arc has length at most $2\pi A$; the radial segment has length at most $L$. Its $h$-length is at most $\sqrt2(L+2\pi A)$. Consequently this annulus is contained in the intrinsic ball of $E_c$ centered at $b'$ with radius $\rho_L=\sqrt2(L+2\pi A)+1$, since all these paths are also allowed in $E_c$. For $L>4A$ the annulus contains the Euclidean ball of radius $L/4$ centered at $(3L/4,0,0)$ in the $y$ chart. The density lower bound and [F7] give $\operatorname{vol}_h B_h^{E_c}(b',\rho_L)\ge2^{-3/2}(4\pi/3)(L/4)^3$. This is a cubic lower bound for radii $\rho_L=O(L)$, contradicting step 4.3, which applies to every fixed center in $E_c$. [given, F3, F4, F7, step 4.3, algebra]

6.1 Thus there is no asymptotically Euclidean chart at this infinity even in the weaker metric sense specified, and in particular no fixed-chart ADM end of [F6]. Together with steps 4.1, 3.2 and 4.2 this proves all the normalized positive-$q$ estimates, their uniformity and recession, and the cylindrical limit with area $4\pi$. The inherited choice premise is used only through the round-sphere and volume-measure suppliers, not to choose a family of curves in the comparison. [A1, F3, F4, F6, step 4.1, step 3.2, step 4.2, step 5.1]

7.1 Apply $dt=(4q/d_q)dt_q$ and $dx^i=dx_q^i/q$ to the bounds in step 3.3. The tensor transformation law in F5 and $r=r_q/q$ give exactly the stated normalized $O_5$ bounds, uniformly on a common end for $q\in[\delta,1]$. The graph of the coordinate change has $r_q=qr$, so the same region correspondence and recession follow. This proves the additional positive-parameter conclusion for the actual smooth global family while preserving all radial-choice conclusions already proved. No zero-parameter assertion for a different gauge is inferred from this extension. [F5, step 3.3, algebra] ∎

## Source notes

Attribution only: The positive-q transformed ends are asymptotically flat in the normalized coordinates, while the zero-q spatial end is asymptotically cylindrical with limiting area 4π in the mass-one normalization. The proof uses the supplied component and denominator estimates and the declared mathematical interfaces; this article citation is not an imported premise.

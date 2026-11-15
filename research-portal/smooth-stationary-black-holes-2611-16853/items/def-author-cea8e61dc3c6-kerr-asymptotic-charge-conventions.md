---
id: def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions
title: Asymptotic mass and axial angular-momentum conventions
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-stationary-asymptotic-decay-data
  - physics:def-gr-spacelike-initial-data-and-constraints
  - physics:def-emg-fx-stationary-axisymmetric-setup
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  physics:def-gr-spacelike-initial-data-and-constraints: mathematical-premise
  physics:def-emg-fx-stationary-axisymmetric-setup: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: H. S. Reall, Black Holes, Part III lecture notes, 15 March 2024
      url: https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf
      locator: §8.1, equation (8.2), printed p.105, and the orientation example
        preceding (8.11), printed p.106; §8.2, equation (8.25), printed p.109;
        §8.4, equations (8.43)–(8.45), printed p.113.
      statement: Defines the Hodge dual using the metric volume form; fixes the
        future/outward orientation in the spherical example; gives the Komar
        axial flux with prefactor 1/(16π), the ADM energy and momentum fluxes,
        and the nonnegative ADM rest mass.
      hypotheses: An oriented metric manifold for the Hodge dual; an asymptotically
        flat spacelike end for the ADM definitions; an axial Killing generator
        for the Komar definition. Here the chart, embedding, orientations and
        axial normalization are supplied explicitly, and each charge is assigned
        only if its displayed limit exists.
      reading_limits: Consulted the browser-extracted PDF text at the listed
        definitions and orientation example, including the adjacent Kerr-Newman
        exercises. No full-notes reading, downloaded-PDF inspection, convergence
        proof, or reconstruction of those exercises is claimed. The geometric
        specification and well-definedness argument here are local.
dependency_level: 1
---

## Definition

Use geometric units $G=c=1$. Let $(M,g,N,T)$ have the stationary Lorentzian data and tensor conventions, and specify a smooth spacelike embedding $\iota:\Sigma\hookrightarrow M$ and an end $E\subset\Sigma$ with a fixed asymptotic Cartesian chart $x:E\to\{x\in\mathbb R^3:|x|>R_0\}$. Identify tangent vectors with their images under $d\iota$. Let $n_\Sigma$ be the future unit normal, and fix the induced metric and second fundamental form by $h=\iota^*g$ and $K(U,V)=g(\nabla_U n_\Sigma,V)$ for $U,V\in T\Sigma$. Only this geometric part of the initial-data interface is used; no constraint equation, Cauchy property or maximality is required.

Write $r=|x|$, $S_r=\{r=\text{constant}\}\subset E$, $n^i=x^i/r$, and $dS_0=r^2d\omega$, where $d\omega$ is the unit Euclidean sphere area. Spatial indices are summed from $1$ to $3$, and $\partial_i$ is differentiation in the specified chart. Put $\operatorname{tr}_hK=h^{ij}K_{ij}$. The outward $h$-unit sphere normal is $\nu_h=\operatorname{grad}_h r/|\operatorname{grad}_h r|_h$, where $(\operatorname{grad}_h r)^i=h^{ij}\partial_jr$; $dS_h$ is the area measure of the restriction of $h$ to $TS_r$, with local density $\sqrt{\det[h(\partial_{y^a},\partial_{y^b})]_{a,b=1}^2}\,dy^1dy^2$ in sphere coordinates $y^1,y^2$. Define
$$E_{\rm ADM}=\frac1{16\pi}\lim_{r\to\infty}\int_{S_r}(\partial_jh_{ij}-\partial_ih_{jj})n^i\,dS_0,\qquad P_i=\frac1{8\pi}\lim_{r\to\infty}\int_{S_r}(K_{ij}-(\operatorname{tr}_hK)h_{ij})\nu_h^j\,dS_h.$$
Changing the overall sign convention of $K$ changes the momentum sign but not its vanishing. When $E_{\rm ADM}^2\geq\sum_iP_i^2$, the rest mass is $M_{\rm ADM}=\sqrt{E_{\rm ADM}^2-\sum_iP_i^2}$.

For angular momentum, additionally specify on an open neighborhood $U\subset M$ of $\iota(E)$ an effective smooth isometric circle action $\rho:U(1)\times U\to U$, with its chosen direction of the angle parameter. Its axial generator is $\eta_p=\frac{d}{d\theta}|_{\theta=0}\rho(e^{i\theta},p)$, with period $2\pi$; it is a Killing field. Use the axial-action convention that $g(\eta,\eta)>0$ off the fixed-point axis. These are additional data for $J_{\rm K}$ only, not conditions on the ADM energy and momentum. No commutation or circularity condition is used.

Fix compatibility of the spacetime orientation with the end chart by requiring $(n_\Sigma,e_1,e_2,e_3)$ to be positively oriented whenever $(e_1,e_2,e_3)$ is a positively oriented tangent basis for $dx^1\wedge dx^2\wedge dx^3$. Orient $S_r$ outward: $(v_1,v_2)$ is positive when $(\nu_h,v_1,v_2)$ is positive on $E$. Equivalently, the metric volume form $\epsilon$ satisfies $\epsilon(n_\Sigma,\nu_h,v_1,v_2)>0$. In a compatible local spacetime extension of the chart with $E$ at $t=0$ and $\partial_t$ future transverse, these are the orientations $dt\wedge dr\wedge\sin\theta\,d\theta\wedge d\phi$ and $d\theta\wedge d\phi$ away from the polar coordinate singularities; the invariant convention defines them also at the poles. For a two-form $A$, set $(\star A)_{ab}=\tfrac12\epsilon_{ab cd}A^{cd}$, with indices raised by $g$, and put $\eta^\flat=g(\eta,\cdot)$. Here $d(\eta^\flat)$ is the exterior derivative, with components $\partial_a\eta_b-\partial_b\eta_a$. Define
$$J_{\rm K}=\frac1{16\pi}\lim_{r\to\infty}\int_{S_r}\iota^*(\star d(\eta^\flat)).$$
The integral uses the restriction of the pulled-back form to $S_r$. Only ends where the respective limits exist are assigned these charges; the rest mass also requires its stated inequality.

## Definition references

[[def-stationary-lorentzian-data]]

[[def-stationary-asymptotic-decay-data]]

[[physics:def-gr-spacelike-initial-data-and-constraints]]

[[physics:def-emg-fx-stationary-axisymmetric-setup]]

## Facts & Assumptions

[F1] The ambient metric, future direction, Killing condition and tensor conventions use [[def-stationary-lorentzian-data]]; the fixed exterior chart uses [[def-stationary-asymptotic-decay-data]].

[F2] Part (a) of [[physics:def-gr-spacelike-initial-data-and-constraints]] supplies the future normal, induced Riemannian metric and positive-sign second fundamental form for the specified spacelike embedding. No matter or development assertion from that interface is invoked.

[F3] The axial-action clause of [[physics:def-emg-fx-stationary-axisymmetric-setup]] supplies the specified circle action, its fixed-point axis and its $2\pi$-periodic Killing generator. Its additional stationary reduction and circularity constructions are not used.

[F4] Reall §8.1 (8.2) and its spherical orientation example, §8.2 (8.25), and §8.4 (8.43)–(8.45) supply the imported Hodge and charge conventions recorded in the source metadata. The displayed formulas fix their use in the chosen chart and orientations.

## Justification

**Given:** The ambient and end data of [F1], the spacelike embedding and geometric data of [F2], the additional axial action when angular momentum is used in [F3], and the imported charge and Hodge conventions of [F4].

**Goal:** Make the charge conventions unambiguous without asserting their limiting existence for arbitrary ends.

1.1 The spacelike embedding supplies a smooth future unit normal, a positive-definite induced metric $h$, and the stated symmetric tensor $K$. Since $dr\ne0$ on the Cartesian exterior, positive-definiteness gives $|\operatorname{grad}_h r|_h>0$; the displayed formula therefore determines the outward unit normal. The restriction of $h$ determines the sphere area density. The fixed chart determines the derivatives, components and Euclidean sphere measure in the energy flux, so both ADM fluxes are determined whenever their limits exist. Replacing $K$ by $-K$ reverses every $P_i$ and leaves the rest-mass expression unchanged. [given, F1, F2, F4]

2.1 The specified action and direction of its angle parameter fix $\eta$, including its sign; differentiating its isometries gives the Killing condition. The ambient metric and the explicitly compatible future/outward orientation fix $\epsilon$, index raising and the Hodge dual, hence the pulled-back Komar integrand and its sign. In the compatible local chart, subtracting tangential components from $\partial_t$ leaves a positive multiple of $n_\Sigma$, so the stated coordinate and invariant orientation conventions agree. Thus the angular flux is determined whenever its limit exists, and the nonnegative mass root is meaningful under the stated inequality. This establishes the conventions only; convergence and Kerr charge evaluations require separate arguments. [given, F1, F2, F3, F4, step 1.1] ∎

## External input

Reall §8 supplies the Hodge-dual, charge and orientation conventions at the recorded locators. No convergence theorem for arbitrary ends, coordinate-invariance theorem or Kerr charge evaluation is imported here. The local justification only checks that the explicitly supplied geometric data determine the displayed expressions.

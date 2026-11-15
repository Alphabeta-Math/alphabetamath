---
id: lem-author-d20d145f998f-normalized-stationary-end
title: Stationary end normalization from quotient compactification
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-killing-field
  - physics:def-gr-metric-selected-connection
  - lem-spherical-exterior-period-input
  - math:def-axiom-of-choice
  - def-stationary-asymptotic-decay-data
  - physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form
  - physics:def-gr-curvature-tensor-and-derived-tensors
  - math:def-normal-neighborhood-and-normal-coordinate-chart
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-killing-field: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  lem-spherical-exterior-period-input: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form: mathematical-premise
  physics:def-gr-curvature-tensor-and-derived-tensors: mathematical-premise
  math:def-normal-neighborhood-and-normal-coordinate-chart: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: R. Beig and B. Schmidt, Time-Independent Gravitational Fields
      url: https://arxiv.org/pdf/gr-qc/0005047v1
      locator: §2.1 (2.33)–(2.38), p.7; §2.3 (2.70)–(2.72), pp.10–11; §3.1 (3.5),
        (3.15)–(3.25), pp.17–20; §3.2 (3.51)–(3.52), p.23
      statement: Stationary vacuum quotient fields on an AF three-end with
        O2(r^-alpha), 1/2<alpha<1, admit arbitrary finite-order multipole
        expansions with O-infinity remainders. Inversion and Omega=r^-2 give C^m
        compactified quotient metric and rescaled mass/twist potentials for
        arbitrarily high finite m. The stationary connection curl is determined
        by the twist; changing it by dF changes the stationary time coordinate.
      hypotheses: The use is local at spatial infinity, where the given stationary
        field is timelike and the quotient is R3 minus a ball. It does not
        assume a globally timelike field on the black-hole DOC.
      reading_limits: Read the stated decomposition, twist, weak-decay,
        multipole-theorem and conformal-compactification passages in the
        retained full PDF. No reconstruction or independent review of the
        elliptic multipole theorem; the 1981 primary reference was not
        retrieved. The conformal conversion and gauge calculations below are
        local arguments, not falsely attributed verbatim to this source.
    - title: S. Dain, Initial data for stationary space-times near space-like infinity
      url: https://arxiv.org/pdf/gr-qc/0107018v1
      locator: §2 (17)–(19) and Theorem2.1, p.4; (20), pp.5–6; Lemma2.5 and (36)–(43),
        pp.7–8
      statement: Under the specified potential-defined conformal factor with C2,alpha
        regularity, C4,alpha conformal quotient metric and Hessian
        normalization, the quotient fields are analytic. In analytic normal
        coordinates the radial stationary connection has beta_i=epsilon_ijk f1^j
        x^k+rho^-1 epsilon_ijk f2^j x^k, with analytic f1,f2.
      hypotheses: Stationary vacuum timelike quotient near spatial infinity; nonzero
        mass normalization B² and exactly the conformal conditions (17)–(19).
        The source signature is +--- and the new slice is not asserted maximal.
      reading_limits: Read the exact hypotheses and Theorem2.1, fields/conformal
        formulas and Lemma2.5 in the retained PDF, plus the nonmaximal-slice
        qualification. The analytic existence theorems are imported; no proof
        reconstruction or primary Beig–Simon1981 reading is claimed. Target
        signature and spin normalization are converted explicitly below.
dependency_level: 1
---

## Statement

Work in ZFC. Let a smooth stationary Ricci-flat four-end have $T=\partial_t$, $g_{00}=-1+2M/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$, with $M>0$. Choose the far tail where $T$ is future timelike. There is a stationary end chart $(t',y)$ for the same field $T$ with $R=|y|$, $g_{00}=-1+2M/R+O_\infty(R^{-2})$, $g_{ij}=\delta_{ij}+O_\infty(R^{-1})$, and $g_{0i}=-2\epsilon_{ijk}S^jy^k/R^3+O_\infty(R^{-3})$ for a fixed vector $S$. Here $O_\infty$ means every finite differentiated order. Relative to the original end this is a spatial end diffeomorphism and an exact stationary time change. The coefficient $S$ is the ADM spin in the sign convention $k=-g(\nabla n,\cdot)$ and normalization $(8\pi)^{-1}\int(k-\operatorname{tr}k\,h)(A\times y,\nu)$. No new slice maximality is asserted.

The spatial chart can be chosen as $y=\xi/|\xi|^2$, where $\xi$ are orthonormal normal coordinates centered at the added point $i$ for the analytic compactified quotient metric $\gamma=\Omega_D^2\bar h$. Here $V=g(T,T)$, $h_{\rm quot}=g-g(T,\cdot)\otimes g(T,\cdot)/V$ on the orbit space, $\bar h=(-V)h_{\rm quot}$, and $\Omega_D$ is the potential-defined factor (17) of Dain. This factor and metric satisfy (18)–(19), with $\Omega_D\in C^{2,\alpha}$ and $\gamma\in C^{4,\alpha}$ for some $0<\alpha<1$, before applying the analytic compactification theorem; $\gamma$ and $\Omega_D$ are then analytic in $\xi$. These properties hold for the same chart $(t',y)$ asserted above.

## Statement references

[[physics:def-gr-smooth-lorentzian-objects]]

[[physics:def-gr-killing-field]]

[[physics:def-gr-metric-selected-connection]]

[[lem-spherical-exterior-period-input]]

[[math:def-axiom-of-choice]]

[[def-stationary-asymptotic-decay-data]]

[[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form]]

[[physics:def-gr-curvature-tensor-and-derived-tensors]]

[[math:def-normal-neighborhood-and-normal-coordinate-chart]]

## Facts & Assumptions

[F1] Lorentzian, Killing and connection conventions and differentiated end bounds are fixed. [[physics:def-gr-smooth-lorentzian-objects]] [[physics:def-gr-killing-field]] [[physics:def-gr-metric-selected-connection]] [[def-stationary-asymptotic-decay-data]]

[F2] Work in ZFC; closed one-forms on a spherical tail are exact by the spherical-period interface. [[math:def-axiom-of-choice]] [[lem-spherical-exterior-period-input]]

[F3] The independent Beig–Schmidt stationary connection–twist curl relation, multipole and conformal-compactification inputs are source 0, and Dain Theorem2.1 and Lemma2.5 are source 1, with their full stated hypotheses and reading limits.

[F4] A smooth embedded spacelike hypersurface in a time-oriented Lorentzian four-manifold has a unique smooth future unit normal $n$, a smooth induced metric $h$ and the smooth symmetric second fundamental form $K(U,W)=g(\nabla_U n,W)$. The Statement uses the opposite convention $k=-K$. [[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form]]

[F5] Ricci-flatness means that the Ricci tensor of the metric-selected connection vanishes. Orthonormal normal coordinates for the compactified Riemannian quotient metric at $i$ are the inverse exponential map expressed in an ordered orthonormal basis of the tangent space at $i$; their Countable Choice assumption is included in ZFC. [[physics:def-gr-curvature-tensor-and-derived-tensors]] [[math:def-normal-neighborhood-and-normal-coordinate-chart]]

## Proof

**Given:**The full hypotheses in the Statement.

**Goal:** Establish the stated claim with its exact hypotheses.

1.1 Put $V=g(T,T)$, $a_i=g_{0i}/V$, $h_{ij}=g_{ij}-g_{0i}g_{0j}/V$, and $\bar h=(-V)h$. The given bounds yield $a=O_6(r^{-2})$, $h=\delta+O_6(r^{-1})$ and $V+1=O_6(r^{-1})$. The stationary vacuum twist equation gives a normalized twist with twice-differentiated decay on this spherical tail: its derivative is a contraction of $T,\nabla T$ and the volume form, hence $O(r^{-3})$; its additive limit is set to zero. Thus the local-at-infinity hypotheses of source 0 hold with any $1/2<\alpha<1$. Import its arbitrary finite-order expansions and $C^m$ conformal quotient compactification, choosing $m$ sufficiently large. [F1, F2, F3, F5]

2.1 In the inverted compact coordinates let $\rho=1/r$, rescaled potentials $\Phi_M,\Phi_S$ and $Q=\Phi_M^2+\Phi_S^2$. The source mass coefficient is nonzero, so $Q(i)>0$. Dain's potential-defined factor is $\Omega_D=\rho^2\,2Q/[B_0^2(\sqrt{1+4\rho^2Q}+1)]$, with $B_0^2=Q(i)$. Its ratio to $\rho^2$ is $C^m$, positive and one at $i$. It therefore preserves $C^m$ compactified regularity and the conformal Hessian normalization. This supplies Dain's actual $C^{4,\alpha}/C^{2,\alpha}$ hypotheses, rather than merely assuming them. Import source 1 Theorem2.1 to obtain analytic quotient fields and use its orthonormal normal coordinates $x=\xi$. In this notation $\gamma=\Omega_D^2\bar h$, with $\bar h=(-V)h_{\rm quot}$ from step 1.1. The spatial chart is obtained by inversion of precisely these normal coordinates, so the compactification conditions and the chart identity in the Statement refer to the same constructed chart. [F3, F5, step 1.1]

3.1 Source 1 Lemma2.5 constructs the convergent radial connection $\beta_i=\epsilon_{ijk}f_1^j(x)x^k+\rho^{-1}\epsilon_{ijk}f_2^j(x)x^k$. Set $C_0=f_2(0)$ and invert to $y=x/\rho^2$. The leading covector is radial-orthogonal, so the reflection part of the inversion differential leaves it unchanged; its physical components are $\beta_i=\epsilon_{ijk}C_0^jy^k/R^3+O_\infty(R^{-3})$. The convergent radial/angular expansions justify every finite derivative bound. Converting the source $+---$ convention to $-+++$ gives $g_{0i}=-\lambda\beta_i$, with $\lambda=1+O_\infty(R^{-1})$. Define $S=C_0/2$ to obtain the displayed coefficient, without equating differently normalized source spin symbols. The other reconstructed components have the asserted convergent expansions. Both old and new quotient metrics are asymptotically Euclidean, so their coordinate transition has bounded first derivative and inverse; the Christoffel transformation gives $D^2y=O(r^{-2})$. Integrating radially and comparing angles yields $y=Q_0x_{\rm old}+O(\log r)$, $Dy=Q_0+O(r^{-1})$, with $Q_0$ orthogonal. Thus $R/r\to1$. The scalar limit $r(V+1)/2=M$ identifies the new leading mass with the old one; convergence of the new radial expansion supplies its $O_\infty(R^{-2})$ remainder. [F1, F3, step 2.1]

4.1 Both stationary connections reconstruct the same norm/twist/quotient fields. The stationary connection–twist relation in source 0, equations (2.36) and (2.70), therefore gives equal exterior derivatives, so their difference is closed. The spherical-tail exactness of [F2] gives the stationary time gauge; it preserves $T$. The new section $\Sigma=\{t'=0\}$ is a smooth embedded hypersurface because it is a coordinate slice. Hereafter $h_{ij}=g_{ij}|_\Sigma$ denotes its induced metric, rather than the quotient metric in step 1.1. Step 3.1 gives $h_{ij}=\delta_{ij}+O_\infty(R^{-1})$. Increase the tail radius until $\|h-\delta\|_{\mathrm{op}}\leq 1/2$ in Euclidean coordinates. Then $h_{ij}v^iv^j\geq |v|^2/2$ for every tangent vector $v$, so $\Sigma$ is spacelike. The ambient tail is smooth and time-oriented, with $T$ future timelike; hence all hypotheses of [F4] hold. It supplies the smooth future unit normal $n$ and second fundamental form $K$, and the Statement's $k$ is $-K$. Put $X_i=g_{0i}$, $X^i=h^{ij}X_j$ and $N=(-g_{00}+h^{ij}X_iX_j)^{1/2}$. These fields are smooth, $N=1+O_\infty(R^{-1})>0$, and $n=N^{-1}(T-X^i\partial_{y^i})$: this vector is unit, orthogonal to the slice, and future directed since $g(T,n)=-N<0$. [F1, F2, F3, F4, step 3.1]

5.1 Let $D_UW$ be the tangential projection of $\nabla_UW$. Ambient metric compatibility and torsion freedom imply the same properties for $D$ with respect to $h$, so $D$ is the induced metric connection. Expanding $\mathcal L_Tg=0$ by metric compatibility and torsion freedom and substituting $T=Nn+X$ gives $0=2NK_{ij}+D_iX_j+D_jX_i$ on tangential pairs; derivatives of $N$ multiply $n$ and pair to zero. Thus $k_{ij}=-K_{ij}=(D_iX_j+D_jX_i)/(2N)$ in exactly the Statement's convention. By steps 3.1 and 4.1 its leading term is $3[(S\times y)_iy_j+(S\times y)_jy_i]/R^5$, with $O_\infty(R^{-4})$ remainder, and its leading trace vanishes. Pair $k-\operatorname{tr}_h k\,h$ with $A\times y$ and the outward $h$-unit normal to a coordinate sphere and integrate using its $h$-area measure. Writing $\omega=y/R$, the identity $\int_{S^2}\omega_i\omega_j\,d\omega=(4\pi/3)\delta_{ij}$ gives ADM angular momentum $A\cdot S$ after multiplication by $(8\pi)^{-1}$. The normal and area corrections are relative $O(R^{-1})$, and the $O(R^{-4})$ tensor remainder contributes $O(R^{-1})$, so all errors vanish in the limit. This fixes the physical spin coefficient and the exact AIK factor two. [F1, F4, step 3.1, step 4.1] ∎

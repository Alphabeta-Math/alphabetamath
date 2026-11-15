---
id: lem-author-840894718169-uniform-gaussian-flow-cone
title: Bounded boost times give a uniform Gaussian collar cone
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-spacelike-maximal-hypersurface-data
  - def-bifurcate-killing-horizon-data
  - lem-killing-normal-boost-and-invariant-tensors
  - physics:thm-gr-local-geodesics-and-exponential-map
  - math:prop-coordinate-geodesic-equation
  - math:thm-smooth-dependence-of-ode-solutions-on-parameters
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:def-local-and-global-flow
  - math:def-axiom-of-choice
  - def-causal-exterior-and-boundary-data
  - lem-author-ca4ffba327b3-event-boundary-generator-data
  - lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant
  - lem-author-ca4ffba327b3-compact-normal-exponential-tube
  - math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves
  - math:thm-unique-maximal-integral-curve-through-each-point
  - math:lem-taylor-integral-remainder
  - math:thm-extreme-value-metric
  - math:thm-compact-implies-the-other-compactness-forms
  - physics:lem-gr-chronology-openness
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  lem-killing-normal-boost-and-invariant-tensors: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  math:prop-coordinate-geodesic-equation: mathematical-premise
  math:thm-smooth-dependence-of-ode-solutions-on-parameters: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  lem-author-ca4ffba327b3-event-boundary-generator-data: mathematical-premise
  lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant: mathematical-premise
  lem-author-ca4ffba327b3-compact-normal-exponential-tube: mathematical-premise
  math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves: mathematical-premise
  math:thm-unique-maximal-integral-curve-through-each-point: mathematical-premise
  math:lem-taylor-integral-remainder: mathematical-premise
  math:thm-extreme-value-metric: mathematical-premise
  math:thm-compact-implies-the-other-compactness-forms: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

Work in ZFC. Let $g_q$, $q\in[0,1]$, be a jointly smooth family of time-oriented Lorentzian metrics of signature $(-,+,+,+)$ on a common neighborhood of a compact embedded sphere $S$. A fixed smooth reference hypersurface $\bar\Sigma$ contains $S$ as a two-sided surface and is uniformly spacelike on a common collar. Specify its end-directed side $\bar\Sigma_+$ with boundary $S$. Its future unit normal $\bar n_q$ and signed boundary-normal distance collars $c_q(r,y)$ are jointly smooth, with $c_q(0,y)=y$ and $\partial_rc_q(0,y)=\bar\nu_q(y)$ the unit normal pointing into $\bar\Sigma_+$. Thus $r\ge0$ on this side; write $\rho_q=r$ there, extending $r$ smoothly with negative sign to the other side.

Let a common smooth Killing field $K$ for every $g_q$ vanish on $S$, and let $\phi_s^K$ denote its maximal local flow. Specify the signed constant $\kappa\in\mathbb R$ by the normal-plane convention $\nabla^{(q)}_{\bar n_q}K=\kappa\bar\nu_q$ and $\nabla^{(q)}_{\bar\nu_q}K=\kappa\bar n_q$ on $S$. There is a common smooth Gaussian coordinate family $\Psi_q(\tau,x)=\exp_x^{(q)}(\tau\bar n_q(x))$ near $S$, with normal projection $\pi_q^\perp$ and $R_q=r\circ\pi_q^\perp$. In these coordinates $g_q=-d\tau_q^2+h_{q,\tau_q}$; in particular the projection fibres are timelike and $-\operatorname{grad}_{g_q}\tau_q=\bar n_q$ on the reference section.

For every $0\le C<\infty$, on a sufficiently small common positive reference collar and uniformly for $q\in[0,1]$ and $|s|\le C$, one has $\tau_q(\phi_s^Kx)=\rho_q(x)\sinh(\kappa s)+O(\rho_q(x)^2)$ and $R_q(\phi_s^Kx)=\rho_q(x)\cosh(\kappa s)+O(\rho_q(x)^2)$. After a further common shrinking there are $c_1,c_2>0$ and $0\le\theta<1$ such that $c_1\rho_q(x)\le R_q(\phi_s^Kx)\le c_2\rho_q(x)$ and $|\tau_q(\phi_s^Kx)|\le\theta R_q(\phi_s^Kx)$ for all these parameters and times.

For the event-boundary conclusion, additionally supply time-oriented ambient spacetimes extending these local metrics, with a specified open reference end $E_q$ for each $q$. Compute chronological sets using $g_q$ in that spacetime and set $\mathcal E_q=I_q^-(E_q)\cap I_q^+(E_q)$. Assume that on one common open neighborhood $O$ of $S$, the branches $H_{q,+}=O\cap\partial I_q^-(E_q)$ and $H_{q,-}=O\cap\partial I_q^+(E_q)$ are smooth embedded null hypersurfaces without boundary in $O$, meeting transversely precisely in $S$, and are preserved by the $K$ flow wherever defined. Assume also that a common positive reference collar lies in $\mathcal E_q$. Then on a smaller common Gaussian collar the two branches are jointly smooth graphs $\tau_q=f_{q,+}(R,y)$ and $\tau_q=f_{q,-}(R,y)$ with $f_{q,+}=R+O(R^2)$ and $f_{q,-}=-R+O(R^2)$, uniformly in $q,y$. Their first radial slopes at $S$ are $+1$ and $-1$, respectively. On the positive reference side the local exterior is exactly $f_{q,-}(R,y)<\tau_q<f_{q,+}(R,y)$ for $R>0$. No parameter regularity of $E_q$ or of the initially supplied branches is assumed; their local graph regularity follows from the null geometry and the smooth metric family.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-bifurcate-killing-horizon-data]]

[[lem-killing-normal-boost-and-invariant-tensors]]

[[physics:thm-gr-local-geodesics-and-exponential-map]]

[[math:prop-coordinate-geodesic-equation]]

[[math:thm-smooth-dependence-of-ode-solutions-on-parameters]]

[[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[[math:def-local-and-global-flow]]

[[math:def-axiom-of-choice]]

[[def-causal-exterior-and-boundary-data]]

[[lem-author-ca4ffba327b3-event-boundary-generator-data]]

[[lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant]]

[[lem-author-ca4ffba327b3-compact-normal-exponential-tube]]

[[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]]

[[math:thm-unique-maximal-integral-curve-through-each-point]]

[[math:lem-taylor-integral-remainder]]

[[math:thm-extreme-value-metric]]

[[math:thm-compact-implies-the-other-compactness-forms]]

[[physics:lem-gr-chronology-openness]]

## Facts & Assumptions

[F1] The Lorentzian connection, spacelike unit normal and induced boundary-distance conventions are the stationary and spacelike-section interfaces. The horizon interface fixes the meaning of a smooth null branch and its radical. The specified boost basis is the future reference normal followed by the end-directed reference boundary normal. [[def-stationary-lorentzian-data]] [[def-spacelike-maximal-hypersurface-data]] [[def-bifurcate-killing-horizon-data]]

[F2] The normal-boost supplier proves the differential boost for a positive rate in this ordered basis. For a negative rate apply that supplier to $-K$ and reverse time; the zero-rate case is verified directly below. [[lem-killing-normal-boost-and-invariant-tensors]]

[F3] The metric exponential has identity vertical derivative at zero, unique geodesics and smooth geodesic evaluation. Apply the coordinate geodesic equation and smooth ODE parameter dependence to the jointly smooth Christoffel coefficients of $g_q$. The inverse theorem then applies to the augmented map retaining $q$. The compact normal-tube supplier supplies the normal splitting and the compact zero-section injectivity argument used below. [[physics:thm-gr-local-geodesics-and-exponential-map]] [[math:prop-coordinate-geodesic-equation]] [[math:thm-smooth-dependence-of-ode-solutions-on-parameters]] [[math:thm-smooth-inverse-function-theorem-on-manifolds]] [[lem-author-ca4ffba327b3-compact-normal-exponential-tube]]

[F4] Local integral curves depend smoothly on initial points and have unique maximal extensions. Their local flow satisfies the flow law. [[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]] [[math:thm-unique-maximal-integral-curve-through-each-point]] [[math:def-local-and-global-flow]]

[F5] For a scalar $C^2$ function of the radial variable on an open interval containing $[0,r]$, a bound $M$ for its second derivative gives $|f(r)-f(0)-rf'(0)|\le Mr^2/2$. Continuous derivative norms on a nonempty compact parameter set are bounded. [[math:lem-taylor-integral-remainder]] [[math:thm-extreme-value-metric]]

[F6] The supplied end defines the exterior and its two chronological boundaries. Smooth null event-boundary branches are achronal and their radical curves are null geodesics up to reparametrization. With an end-directed spacelike collar in the exterior, the normal exponential coordinates $\Xi_q(y,a,b)=\exp_y^{(q)}(a\bar n_q+b\bar\nu_q)$ identify the future boundary locally with $a=b$, the past boundary with $a=-b$, and the exterior with $a-b<0<a+b$. These are single-metric local conclusions of the existing suppliers, not an assumed joint parameter estimate. [[def-causal-exterior-and-boundary-data]] [[lem-author-ca4ffba327b3-event-boundary-generator-data]] [[lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant]]

[F7] Under the stated ZFC convention, the chronology-openness supplier applies to each supplied ambient time-oriented smooth Lorentzian spacetime and makes every pointwise chronological future and past open. By the exterior interface, $I_q^\pm(E_q)=\bigcup_{p\in E_q}I_q^\pm(p)$; hence these sets are open as unions of open sets. [[physics:lem-gr-chronology-openness]] [[def-causal-exterior-and-boundary-data]] [[math:def-axiom-of-choice]]

[A1] Use ZFC, including Choice for selecting collision sequences in the compactness arguments. A sphere carries a compatible metric from its specified smooth identification with the unit sphere; the compact parameter products used below are metrizable. Compactness gives convergent subsequences. [[math:def-axiom-of-choice]] [[math:thm-compact-implies-the-other-compactness-forms]]

## Proof

**Given:** The data and explicit hypotheses of the Statement, with the additional end and event-boundary hypotheses used only for the final conclusion.

**Goal:** Construct the common Gaussian family, prove the uniform bounded-flow cone, and identify the event-boundary graphs and exterior when supplied.

1.1 The coordinate geodesic equations have jointly smooth coefficients in position, velocity and $q$; at the endpoints of $[0,1]$, smooth family means smooth extension to a parameter neighborhood. Thus their solutions and $\Psi_q$ are jointly smooth near the zero section. At $(0,y)$ the differential in $(\tau,x)$ is $(u,V)\mapsto u\bar n_q+V$, an isomorphism because the reference tangent hyperplane is spacelike. Apply the inverse theorem to $(q,\tau,x)\mapsto(q,\Psi_q(\tau,x))$. Compactness of $[0,1]\times S$ supplies a common domain of definition and local invertibility. For global injectivity on a sufficiently small tube, otherwise select collisions at radii tending to zero. Passing to subsequences, their parameters and base points converge; equality of images forces both limiting base points to be the same point of $S$. Both preimages then lie in one augmented inverse neighborhood, a contradiction. This is the compact normal-tube argument with the parameter retained. Hence the local inverses agree to give a common smooth Gaussian family. The identical argument gives a common jointly smooth normal tube $\Xi_q(y,a,b)$ about $S$. Shrink both tubes to have compactly contained smaller domains; when the event data are supplied, keep their images in $O$. [given, F1, F3, A1]

2.1 Write $V=\partial_\tau\Psi_q$ and let $J$ be a variation in a reference base coordinate. Each normal geodesic has constant squared speed $-1$. Torsion freedom gives $\nabla_VJ=\nabla_JV$, whence $\partial_\tau g_q(V,J)=g_q(V,\nabla_JV)=\tfrac12Jg_q(V,V)=0$. The pairing is initially zero, so remains zero. This proves the Gaussian metric form and the assertions about its timelike fibres and gradient. Since $K=0$ on $S$, the constant curves there are its integral curves for all time. Finite iteration of the local flow neighborhoods from F4 along these constant curves, followed by a finite cover of $S$, gives a smooth flow on a neighborhood of $[-C,C]\times S$ for any fixed finite $C$. Uniqueness identifies it with the maximal local flow. Continuity and compactness then put all bounded-time images of a small common reference collar in the Gaussian tube. [given, F1, F3, F4, A1, step 1.1]

2.2 Now impose the event-boundary hypotheses. For each fixed $q$, F6 identifies the two branch germs at $S$ with the null exponential sheets $\Gamma_{q,\pm}(y,t)=\Xi_q(y,\pm t,t)$, with the indicated future/past labels. These sheets are jointly smooth in $(q,y,t)$ on one common small interval by step 1.1. They remain in the corresponding event boundaries throughout that interval, not merely on a possibly $q$-dependent germ: for each fixed $(q,y)$ continue from $t=0$ along the affine null geodesic. At a finite endpoint of its maximal interval of membership inside the common tube, closedness of the ambient event boundary puts the limiting point on the same branch. Smoothness of that branch makes the limiting geodesic tangent its null radical, since it is a limit of radical tangents. The generator theorem in F6 and geodesic uniqueness in F3 continue it in the branch past that endpoint, a contradiction. The same argument holds in either direction of $t$. This uses no uniform derivative bound for the initially supplied horizons. [given, F3, F6, step 1.1]

3.1 At $p\in S$, set $A(s)=d\phi_s^K|_p$. Differentiation of the flow law gives $A'(s)=B_pA(s)$, $A(0)=I$, where $B_p(v)=\nabla_v^{(q)}K$ since $K_p=0$. The flow fixes $S$ pointwise, so its tangent differential is the identity. On the specified ordered normal basis the given matrix is $\kappa\begin{pmatrix}0&1\\1&0\end{pmatrix}$. For $\kappa>0$, F2 applies directly; for $\kappa<0$ apply it to $-K$ at time $-s$; for $\kappa=0$, the equation on the normal plane is $A'=0$. In every case the result is $d\phi_s^K\bar\nu_q=\cosh(\kappa s)\bar\nu_q+\sinh(\kappa s)\bar n_q$. [given, F1, F2, F4, step 2.1, algebra]

3.2 Project $\Gamma_{q,\pm}$ onto the reference hypersurface. At $t=0$ its differential in $(t,y)$ is $(u,Y)\mapsto u\bar\nu_q+Y$, an isomorphism, while the time derivative is $\pm1$. The augmented inverse theorem, compactness and the collision argument from step 1.1 therefore give jointly smooth inverse projections on a common two-sided reference collar. They define graphs $f_{q,\pm}$ with $f_{q,\pm}(0,y)=0$ and $\partial_Rf_{q,\pm}(0,y)=\pm1$. These graphs exhaust the event boundaries on a common smaller Gaussian cylinder: a second boundary point on a Gaussian fibre would be timelike related to its existing graph point, contradicting achronality from F6. Their jointly smooth second radial derivatives are bounded on a compact smaller cylinder, and F5 gives $f_{q,\pm}=\pm R+O(R^2)$ with one error constant. Thus uniform branch control has been derived from the smooth exponential maps and the event-boundary geometry. [given, F3, F5, F6, A1, step 1.1, step 2.1, step 2.2]

4.1 Compose the Gaussian coordinate functions with $\phi_s^Kc_q(r,y)$. At $r=0$ both $\tau_q$ and $R_q$ vanish, and step 3.1 gives their radial derivatives $\sinh(\kappa s)$ and $\cosh(\kappa s)$. The compositions are jointly smooth on a neighborhood of a compact smaller cylinder $[0,1]\times[-C,C]\times S\times[0,r_0]$. Thus their second radial derivatives have one finite bound $M$ by F5. Apply its $n=1$ Taylor estimate in $r$, holding $(q,s,y)$ fixed, to obtain the asserted uniform quadratic errors. In particular, writing the errors as $E_\tau,E_R$, one has $|E_\tau|+|E_R|\le M r^2$ after enlarging $M$. [given, F3, F4, F5, step 1.1, step 2.1, step 3.1]

5.1 Put $T=\tanh(|\kappa|C)<1$ and $B=\cosh(|\kappa|C)$. For $|s|\le C$, $|\sinh(\kappa s)|\le T\cosh(\kappa s)$ and $1\le\cosh(\kappa s)\le B$. Choose $r_0$ smaller so $Mr_0\le1/2$. Then $r/2\le R_q\le(B+1/2)r$, giving radial comparison. Moreover $|\tau_q|\le TR_q+(1+T)Mr^2$. Choose $T<\theta<1$ and shrink once more so $2(1+T)Mr_0\le\theta-T$. Dividing by $R_q\ge r/2$ for $r>0$ proves the cone bound; at $r=0$ both sides vanish. This includes $C=0$ and $\kappa=0$. [given, F5, step 4.1, algebra]

6.1 For each $q$, F6 and the positive reference collar in $\mathcal E_q$ select $I_q^-(E_q)$ as the past side of the upper graph and $I_q^+(E_q)$ as the future side of the lower graph near $S$. These side identities extend throughout the common smaller cylinder: off its graph, each connected side of a boundary has constant membership in its chronological set, which is open by F7, and the local identity supplies a point on each side. There are no further boundary points by step 3.2. The selected component on $R>0$ is consequently exactly $f_{q,-}<\tau_q<f_{q,+}$. If $M_H$ bounds the graph remainder constants, shrink further so $M_HR<1-\theta$. Then $f_{q,-}<-\theta R\le\tau_q\le\theta R<f_{q,+}$ for every bounded-flow image with $R>0$, by step 5.1; hence these images lie on the selected exterior side as well. [given, F6, F7, step 5.1, step 3.2] ∎

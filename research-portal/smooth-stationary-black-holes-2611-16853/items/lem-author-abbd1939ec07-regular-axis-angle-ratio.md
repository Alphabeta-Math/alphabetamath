---
id: lem-author-abbd1939ec07-regular-axis-angle-ratio
title: A regular weight-one axis has zero logarithmic angle defect
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-black-hole-comparison-hypothesis-data
  - def-author-abbd1939ec07-reconstructed-harmonic-map-data
  - math:def-embedded-submanifold-and-slice-chart
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:thm-clairaut-schwarz-mixed-partials
  - math:thm-multivariable-taylor-formula-with-lagrange-remainder
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - physics:lem-gr-inverse-metric-is-smooth
  - math:thm-chain-rule-for-total-derivatives
  - math:thm-heine-borel-rn
  - math:thm-extreme-value-metric
  - math:thm-fermat-for-euclidean-local-extrema
dependency_roles:
  def-black-hole-comparison-hypothesis-data: mathematical-premise
  def-author-abbd1939ec07-reconstructed-harmonic-map-data: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:thm-clairaut-schwarz-mixed-partials: mathematical-premise
  math:thm-multivariable-taylor-formula-with-lagrange-remainder: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  physics:lem-gr-inverse-metric-is-smooth: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:thm-heine-borel-rn: mathematical-premise
  math:thm-extreme-value-metric: mathematical-premise
  math:thm-fermat-for-euclidean-local-extrema: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 7
---

## Statement

Suppose a reconstructed-map metric from [[def-author-abbd1939ec07-reconstructed-harmonic-map-data]] extends to a regular axis in the weight-one sense of [[def-black-hole-comparison-hypothesis-data]], and on an open axis interval $U$ and $\alpha$ extend continuously as finite functions. Then the logarithmic angle defect $\mathbf b(z):=\log\lim_{\rho\downarrow0} L(\rho,z)/(C(\rho,z)/(2\pi))$ is zero. Here $L(\rho,z)=\int_0^\rho e^{\alpha(s,z)-U(s,z)}ds$ is radial proper length in the orthogonal meridian and $C(\rho,z)=2\pi\rho e^{-U(\rho,z)}$ is axial orbit circumference. In this representation $\mathbf b(z)=\alpha(0,z)$.

Precisely, the extension hypothesis is an extension of this reconstructed metric together with its specified angular action. Locally at each interior axis value, take intervals $J$ in $\tau$ and $I$ in $z$ and $\delta>0$. There is a smooth isometric identification $\iota$ of $J\times(0,\delta)\times I\times S^1$ with an open subset of $M\setminus A$, where $(M,g)$ has the regular weight-one axis $A$ and smooth circle action $\psi_s$. It obeys $\iota(\tau,\rho,z,\phi+s)=\psi_s(\iota(\tau,\rho,z,\phi))$ and $\iota^*g=\mathbf g$. It has a continuous extension $\bar\iota$ to $J\times[0,\delta)\times I\times S^1$ with $\bar\iota(\tau,0,z,\phi)=p(\tau,z)\in A$, independently of $\phi$. This specifies what extension across the coordinate axis means here; no differentiability of $\bar\iota$ at the axis is required, and existence of such an extension is not inferred from the off-axis reconstruction equations.

## Facts & Assumptions

[F1] The metric and period $2\pi$ are [[def-author-abbd1939ec07-reconstructed-harmonic-map-data]]. Smooth extension and the weight-one differential circle action on a spacelike normal plane are the regular-axis conditions of [[def-black-hole-comparison-hypothesis-data]]. All limits in the statement are taken at a fixed interior point of the open axis interval. The identification $\iota$, its equivariance and its continuous boundary extension are the explicit meaning of the extension hypothesis in the Statement; the two suppliers alone do not assert that an off-axis reconstruction admits this extension.

[F2] An embedded smooth axis has local slice charts by [[math:def-embedded-submanifold-and-slice-chart]]. An invertible differential gives a smooth local coordinate change by [[math:thm-smooth-inverse-function-theorem-on-manifolds]]. Derivatives of the smooth action can be interchanged by [[math:thm-clairaut-schwarz-mixed-partials]]. Taylor expansion with bounded remainders on smaller coordinate neighborhoods is supplied by [[math:thm-multivariable-taylor-formula-with-lagrange-remainder]], applied also to derivatives.

[F3] The invariant inverse-metric pairing and its matrix formula are [[physics:def-gr-inverse-metric-and-musical-isomorphisms]]; its smoothness is [[physics:lem-gr-inverse-metric-is-smooth]]. Both suppliers have domain mathematics. Euclidean differentiation of compositions and rescalings uses [[math:thm-chain-rule-for-total-derivatives]].

[F4] Closed Euclidean balls and boxes are compact by [[math:thm-heine-borel-rn]], so continuous real functions on them attain their extrema by [[math:thm-extreme-value-metric]]. A differentiable function at an interior local extremum has zero gradient by [[math:thm-fermat-for-euclidean-local-extrema]].

## Proof

**Given:** The reconstructed metric, its continuous meridian coefficients and its regular weight-one extension, realized by the specified equivariant isometric identification $\iota$ with continuous boundary extension $\bar\iota$.

**Goal:** Compute the angle ratio and prove that its logarithm vanishes, without assuming a limiting tangent for the coordinate meridian.

1.1 Fix an interior axis value $z_0$. Restricting the metric to the fixed-$\tau,z,\phi$ meridian and the axial orbit gives exactly $L$ and $C$. Continuity gives $L(\rho,z_0)/\rho\to e^{\alpha(0,z_0)-U(0,z_0)}$: the difference between this average integral and its limiting integrand is bounded by the supremum of the integrand's difference on $[0,\rho]$. Also $C(\rho,z_0)/(2\pi\rho)\to e^{-U(0,z_0)}>0$. Thus the ratio in the statement tends to $e^{\alpha(0,z_0)}$. It remains to show this is one. [given, F1, algebra]

1.2 Write $Z$ for the smooth axial generator and $A$ for the fixed axis. Near the axis point under consideration choose coordinates $(x^0,x^1,y^1,y^2)$ with $A=\{y=0\}$ and with $\partial_{y^1},\partial_{y^2}$ an orthonormal normal pair along $A$. Here is a local construction of the latter refinement of a slice chart. The tangential metric block along $A$ is invertible, because the normal plane is nondegenerate and $g$ is nondegenerate. Subtract the tangential projections of the two transverse coordinate vectors to obtain a normal basis $V_1,V_2$. Put $e_1=V_1/\sqrt{g(V_1,V_1)}$, $W_2=V_2-g(V_2,e_1)e_1$, and $e_2=W_2/\sqrt{g(W_2,W_2)}$. All denominators are smooth and positive. In the original chart map $(x,y)$ to $(x,0)+y^1 e_1(x)+y^2 e_2(x)$, where the vectors are expressed in that chart. Its differential at $y=0$ maps to a tangential basis and this normal pair, hence is invertible; [F2] makes this a local chart. In these refined coordinates $g_{ab}(x,0)=\delta_{ab}$ and $g_{ia}(x,0)=0$ for normal indices $a,b$ and tangential indices $i$. [given, F1, F2, F3, construct, algebra]

2.1 At $y=0$ the generator vanishes. Differentiating the action in its parameter and in the coordinates, with the derivative interchange in [F2], shows that its linearization is zero tangentially and is the generator $J$ of the weight-one rotation on the normal plane; $J^{\mathsf T}J=I$. The sign of $J$ can be fixed locally and does not affect the calculation. With $r=|y|$, Taylor expansion gives tangential components $Z^i=O(r^2)$ and normal components $Z^a=(Jy)^a+O(r^2)$. Consequently, for $f=g(Z,Z)$, Taylor expansion of $f$ and its first derivatives gives $f=r^2+O(r^3)$, $\partial_{y^a}f=2y^a+O(r^2)$ and $\partial_{x^i}f=O(r^2)$. These estimates are uniform on a smaller chart: bound the finitely many required smooth derivatives on a closed coordinate box using [F4]. For the positive orbit radius $R=\sqrt{f}$ off the axis, it follows that $R=r+O(r^2)$, $\partial_{y^a}R=y^a/r+O(r)$ and $\partial_{x^i}R=O(r)$. The smooth inverse metric has normal block $I+O(r)$, mixed block $O(r)$ and bounded tangential block. Thus the invariant scalar $Q:=g^{-1}(dR,dR)=1+O(r)$ tends to one, uniformly in a local axis neighborhood. This uses smooth axis geometry, without asserting that the Weyl meridian has a smooth limiting tangent. [F1, F2, F3, F4, step 1.2, algebra]

3.1 The axial generator used above is the one measured by the reconstructed angular coordinate: differentiating the equivariance identity in $s$ at zero, off the axis, gives $d\iota(\partial_\phi)=Z\circ\iota$. Therefore $g(Z,Z)\circ\iota=\mathbf g(\partial_\phi,\partial_\phi)=\rho^2e^{-2U}$. The isometric identification and the chain rule also identify the inverse-metric norm of the differential of this orbit radius on the two open manifolds: in local charts, put $P=D\iota$, let $G$ be the matrix of $g$, and let $\lambda$ be the column of components of $dR$. The pulled-back metric matrix and covector column are $P^{\mathsf T}GP$ and $P^{\mathsf T}\lambda$; since $P$ is invertible, $(P^{\mathsf T}\lambda)^{\mathsf T}(P^{\mathsf T}GP)^{-1}(P^{\mathsf T}\lambda)=\lambda^{\mathsf T}G^{-1}\lambda$. To check the approach to the axis, fix $\tau_0\in J$, $\phi_0\in S^1$, $z_0\in I$, and put $p_0=p(\tau_0,z_0)$. For $K=\{\xi\in\mathbb R^2:|\xi-(1,0)|\le1/4\}$, define $q_\epsilon(\xi)=\iota(\tau_0,\epsilon\xi_1,z_0+\epsilon\xi_2,\phi_0)$. The parameter points defining $q_\epsilon$ are at Euclidean $(\rho,z)$ distance at most $5\epsilon/4$ from $(0,z_0)$, since $|\xi|\le5/4$ on $K$. By continuity of $\bar\iota$ at $(\tau_0,0,z_0,\phi_0)$, every neighborhood of $p_0$ therefore contains all $q_\epsilon(K)$ for sufficiently small $\epsilon$. In the smaller smooth chart of step 2.1, the normal coordinates of these points consequently tend to zero uniformly, and the uniform estimate $Q=1+O(r)$ there yields $Q(q_\epsilon(\xi))\to1$ uniformly on $K$. This establishes the needed coordinate-to-extension limit without differentiating the boundary extension. [given, F1, F3, step 2.1, algebra]

4.1 By the generator identification in step 3.1, in the reconstructed coordinates $R=\rho e^{-U}=C/(2\pi)$, independently of $\tau,\phi$. Inverting the meridian block of the displayed reconstructed metric therefore gives $Q=e^{2U-2\alpha}(R_\rho^2+R_z^2)$. In particular $|D R|=e^{\alpha-U}\sqrt{Q}$, where $D$ and its norm are Euclidean in $(\rho,z)$. Set $B=e^{-U(0,z_0)}>0$ and $H=e^{\alpha(0,z_0)-U(0,z_0)}>0$. On the closed Euclidean disk $K=\{\xi\in\mathbb R^2:|\xi-(1,0)|\le1/4\}$ define $F_\epsilon(\xi)=R(\epsilon\xi_1,z_0+\epsilon\xi_2)/\epsilon$ for positive sufficiently small $\epsilon$. This disk stays off the axis. Continuity of $U,\alpha$ at $(0,z_0)$ gives $F_\epsilon\to B\xi_1$ uniformly on $K$. Step 3.1 gives $Q\to1$ uniformly on these shrinking coordinate disks. The chain rule and the inverse-block identity then give $|D F_\epsilon|\to H$ uniformly on $K$. No convergence of derivatives of $U$ or $\alpha$ has been assumed. [given, F1, F3, step 3.1, algebra]

5.1 To compare these two limits, fix $\eta>0$ and set $h_\epsilon(\xi)=F_\epsilon(\xi)-B\xi_1$ and $\xi_*=(1,0)$. The continuous function $h_\epsilon(\xi)-\eta|\xi-\xi_*|^2$ attains a maximum on $K$ by [F4]. For small $\epsilon$ it is smaller on the boundary than at $\xi_*$: the boundary penalty is $\eta/16$, while $2\sup_K|h_\epsilon|\to0$. Hence a maximizer $\xi_\epsilon$ is interior, and Fermat's theorem gives $D F_\epsilon(\xi_\epsilon)=B(1,0)+2\eta(\xi_\epsilon-\xi_*)$. The reverse triangle inequality implies $\bigl||D F_\epsilon(\xi_\epsilon)|-B\bigr|\le\eta/2$. Uniform gradient-norm convergence in step 4.1 now implies $|H-B|\le\eta/2$. Since $\eta>0$ was arbitrary, $H=B$. [F4, step 4.1, choose, algebra]

6.1 The equality $H=B$ is $e^{\alpha(0,z_0)-U(0,z_0)}=e^{-U(0,z_0)}$, so $e^{\alpha(0,z_0)}=1$ and $\alpha(0,z_0)=0$. Step 1.1 then gives $\mathbf b(z_0)=\alpha(0,z_0)=0$. As $z_0$ was arbitrary in the open interval, this proves the full statement. [step 1.1, step 4.1, step 5.1, algebra] ∎

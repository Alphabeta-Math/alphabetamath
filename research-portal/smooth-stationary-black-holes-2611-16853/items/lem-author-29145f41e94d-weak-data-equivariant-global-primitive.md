---
id: lem-author-29145f41e94d-weak-data-equivariant-global-primitive
title: Equivariant global Harrison primitive under weak original data
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - thm-vacuum-killing-ernst-input
  - def-author-9f9c6144aed8-ernst-mars-simon
  - lem-spherical-exterior-period-input
  - lem-author-9e1b6fa65528-relative-normal-homotopy
  - lem-author-9e1b6fa65528-equivariant-cartan-normalization
  - lem-author-9e1b6fa65528-radial-exterior-primitive
  - lem-author-9e1b6fa65528-stationary-spatial-lifting
  - lem-author-9e1b6fa65528-stationary-exact-gluing
  - lem-author-ca4ffba327b3-compact-normal-exponential-tube
  - def-circle-action-and-invariant-normal-data
  - lem-author-29145f41e94d-smooth-weak-end-primitive
  - math:def-axiom-of-choice
  - math:thm-stokes-theorem-for-smooth-singular-chains
  - def-stationary-lorentzian-data
  - def-spacelike-maximal-hypersurface-data
  - def-complex-self-dual-two-form-data
  - def-stationary-asymptotic-decay-data
  - lem-author-d20d145f998f-normalized-stationary-end
  - physics:thm-gr-local-geodesics-and-exponential-map
  - math:def-pullback-of-a-differential-form
  - math:thm-the-exterior-derivative-commutes-with-pullback
  - math:thm-chain-rule-for-total-derivatives
  - math:thm-algebra-of-derivatives
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:thm-intermediate-value
  - math:def-the-standard-smooth-step-function
  - math:thm-general-stokes-theorem
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  thm-vacuum-killing-ernst-input: mathematical-premise
  def-author-9f9c6144aed8-ernst-mars-simon: mathematical-premise
  lem-spherical-exterior-period-input: mathematical-premise
  lem-author-9e1b6fa65528-relative-normal-homotopy: mathematical-premise
  lem-author-9e1b6fa65528-equivariant-cartan-normalization: mathematical-premise
  lem-author-9e1b6fa65528-radial-exterior-primitive: mathematical-premise
  lem-author-9e1b6fa65528-stationary-spatial-lifting: mathematical-premise
  lem-author-9e1b6fa65528-stationary-exact-gluing: mathematical-premise
  lem-author-ca4ffba327b3-compact-normal-exponential-tube: mathematical-premise
  def-circle-action-and-invariant-normal-data: mathematical-premise
  lem-author-29145f41e94d-smooth-weak-end-primitive: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-stokes-theorem-for-smooth-singular-chains: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  lem-author-d20d145f998f-normalized-stationary-end: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  math:def-pullback-of-a-differential-form: mathematical-premise
  math:thm-the-exterior-derivative-commutes-with-pullback: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:thm-algebra-of-derivatives: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:thm-intermediate-value: mathematical-premise
  math:def-the-standard-smooth-step-function: mathematical-premise
  math:thm-general-stokes-theorem: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 6
---

## Statement

Work in ZFC. Let $(M,g,T)$ be smooth oriented, time-oriented stationary Lorentzian data of signature $(-,+,+,+)$, with $\operatorname{Ric}(g)=0$ on the open region under consideration. Supply an open exterior $E$ and a smooth embedded spacelike three-manifold $\overline\Sigma\cong[1,\infty)\times S^2$ with boundary $S$, whose interior $\Sigma$ lies in $E$. Write $\rho$ for this radial parameter. The supplied product is specifically the stationary-flow diffeomorphism $\Phi:\mathbb R\times\Sigma\to E$, $\Phi(t,x)=\Phi_t^T(x)$, so $T=\partial_t$ and the specified original section is $\Sigma=\{t=0\}$. Near $S$, require the exterior attachment to be the outward spacelike wedge: in a sufficiently small normal-exponential tube $\Xi(s,a,b)=\exp_s(a n_s+b\nu_s)$, $E$ consists precisely of $b>|a|$, where $n$ is a future unit normal of $S$ and $\nu$ is its unit spacelike normal pointing toward the specified side $\Sigma$. Here the tube frame is orthonormal; the same wedge is obtained in any smooth orthonormal normal frame with these time and side orientations. This is a boundary attachment hypothesis, not a product diffeomorphism extending through $S$.

On the original end of $\Sigma$ use Cartesian coordinates $x$, $r=|x|$, extended by $\Phi$. This physical radius is independent of the topological product radius $\rho$. For every sufficiently large $R$, require the physical truncation $B_R=\overline\Sigma\setminus\{r>R\}$ to be a compact smooth region with boundary $S\sqcup\Gamma_R$, where $\Gamma_R=\{r=R\}$, containing a relative neighborhood of $S$. Require these nested physical truncations to exhaust $\overline\Sigma$, and the physical closed tails $\{r\ge R\}$ to be closed in $\overline\Sigma$ and disjoint from $S$. These are end-attachment and compactness hypotheses, with no equality of the two radii required; the previous special case $r=\rho$ on a far tail satisfies them. The weak mass-one end means $g_{00}=-1+2/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$ and $g_{ij}=\delta_{ij}+O_6(r^{-1})$, with $T$ future timelike on a far tail. The notation $u=O_m(r^{-b})$ means $|\partial_x^\alpha u|\le C_\alpha r^{-b-|\alpha|}$ for $|\alpha|\le m$, uniformly in direction for sufficiently large $r$; $O_\infty$ means these bounds at every finite order.

Supply a smooth Ernst potential $\sigma=f+i\psi$ on $E$ and a connected neighborhood of $S$, with $d\sigma=2\iota_T(F+i\star_g F)$, $F_{ab}=\nabla_aT_b$, $f=-g(T,T)$ and $\sigma\to1$ on the specified end. On a neighborhood of $S$ supply commuting Killing fields $K,Z$, with $K=T+\Omega_H Z$ for a constant $\Omega_H$, $K|_S=0$, and a smooth isometric circle action generated by $Z$, preserving $S$ and having period $2\pi$. The constant nonzero normal boost rate means that, for $u=b+a$ and $v=b-a$, the differential of the $K$ flow on the normal bundle acts by $(u,v)\mapsto(e^{\kappa t}u,e^{-\kappa t}v)$ for one constant $\kappa\ne0$. Supply $p\in S$ with $T_p=Z_p=0$.

Then there is one smooth stationary real one-form $W_0$ on $E$ and a neighborhood of $S$, with $dW_0=\Theta_0=4((f-1)F+\psi\star_gF)$, $W_0(T)=d_0-D_0$, $D_0=|1-\sigma|^2$ and $d_0=D_0(p)>0$. It is locally $K,Z$ invariant near $S$, and on the unchanged original end it has the form $W_0=(d_0-D_0)dt+w_i\,dx^i$ with $w_i=O_5(r^{-3})$. Any supplied maximality of the original section is retained. No stronger same-section asymptotic expansion is assumed.

## Statement references

[[physics:def-gr-smooth-lorentzian-objects]]

[[thm-vacuum-killing-ernst-input]]

[[def-author-9f9c6144aed8-ernst-mars-simon]]

[[lem-spherical-exterior-period-input]]

[[lem-author-9e1b6fa65528-relative-normal-homotopy]]

[[lem-author-9e1b6fa65528-equivariant-cartan-normalization]]

[[lem-author-9e1b6fa65528-radial-exterior-primitive]]

[[lem-author-9e1b6fa65528-stationary-spatial-lifting]]

[[lem-author-9e1b6fa65528-stationary-exact-gluing]]

[[lem-author-ca4ffba327b3-compact-normal-exponential-tube]]

[[def-circle-action-and-invariant-normal-data]]

[[lem-author-29145f41e94d-smooth-weak-end-primitive]]

[[math:def-axiom-of-choice]]

[[math:thm-stokes-theorem-for-smooth-singular-chains]]

[[def-stationary-lorentzian-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-complex-self-dual-two-form-data]]

[[def-stationary-asymptotic-decay-data]]

[[lem-author-d20d145f998f-normalized-stationary-end]]

[[physics:thm-gr-local-geodesics-and-exponential-map]]

[[math:def-pullback-of-a-differential-form]]

[[math:thm-the-exterior-derivative-commutes-with-pullback]]

[[math:thm-chain-rule-for-total-derivatives]]

[[math:thm-algebra-of-derivatives]]

[[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[[math:thm-intermediate-value]]

[[math:def-the-standard-smooth-step-function]]

[[math:thm-general-stokes-theorem]]

## Facts & Assumptions

[F1] The stationary metric, connection, Hodge, Ernst and spacelike-boundary conventions are the declared mathematical interfaces; the potential itself is supplied. [[physics:def-gr-smooth-lorentzian-objects]] [[def-stationary-lorentzian-data]] [[def-spacelike-maximal-hypersurface-data]] [[def-complex-self-dual-two-form-data]] [[def-author-9f9c6144aed8-ernst-mars-simon]] [[thm-vacuum-killing-ernst-input]]

[F2] Differentiated end bounds use the Cartesian convention. The end-normalization lemma applies to a smooth stationary Ricci-flat end with these weak metric bounds and positive mass; it supplies an auxiliary all-order stationary chart for the same $T$, related by a spatial end diffeomorphism and an exact stationary time change. Derivative and inverse-matrix estimates use the chain, product and quotient rules. [[def-stationary-asymptotic-decay-data]] [[lem-author-d20d145f998f-normalized-stationary-end]] [[math:thm-chain-rule-for-total-derivatives]] [[math:thm-algebra-of-derivatives]]

[F3] On a supplied spherical product every smooth closed one-form is exact, and a smooth closed two-form is exact when its generator-sphere period is zero. General Stokes applies to the compact oriented three-dimensional section regions with boundary: the restricted two-form has compact support because the whole region is compact, and boundary orientation is outward-normal-first. The corresponding chain identity is also available. Pullback of a form is smooth and commutes with exterior differentiation. Work in ZFC, carrying Choice through these suppliers and the tube construction; no further choice principle is introduced. [[lem-spherical-exterior-period-input]] [[math:thm-general-stokes-theorem]] [[math:thm-stokes-theorem-for-smooth-singular-chains]] [[math:def-pullback-of-a-differential-form]] [[math:thm-the-exterior-derivative-commutes-with-pullback]] [[math:def-axiom-of-choice]]

[F4] The spacelike boundary supplies a smooth orthonormal normal frame and a dilation-stable normal-exponential tube. Circle averaging supplies a smooth invariant future unit normal. Relative normal homotopy and equivariant Cartan normalization apply once the surface primitive and equivariant tube have been established. Geodesics for the metric-selected connection have unique initial-value solutions, and the exponential map is smooth. [[lem-author-ca4ffba327b3-compact-normal-exponential-tube]] [[def-circle-action-and-invariant-normal-data]] [[lem-author-9e1b6fa65528-relative-normal-homotopy]] [[lem-author-9e1b6fa65528-equivariant-cartan-normalization]] [[physics:thm-gr-local-geodesics-and-exponential-map]]

[F5] The stationary lift requires exactly $E=\mathbb R_t\times\Sigma$, $T=\partial_t$, a closed stationary $\Theta$, a stationary $D$ with $\iota_T\Theta=dD$, and a smooth primitive of its spatial part. The smooth weak-end primitive additionally requires the auxiliary all-order metric bounds, $\Theta'_{ab}=O_\infty(R^{-4})$ and original $D=O_6(r^{-2})$. Its construction uses the all-order radial primitive and returns to the original section. These hypotheses are checked below. [[lem-author-9e1b6fa65528-stationary-spatial-lifting]] [[lem-author-29145f41e94d-smooth-weak-end-primitive]] [[lem-author-9e1b6fa65528-radial-exterior-primitive]]

[F6] The smooth inverse function theorem gives local graph charts for a transverse projection, and the intermediate value theorem gives a zero between opposite signs. The standard smooth step function gives smooth cutoffs between two prescribed radii. [[math:thm-smooth-inverse-function-theorem-on-manifolds]] [[math:thm-intermediate-value]] [[math:def-the-standard-smooth-step-function]]

[F7] Stationary exact gluing requires disjoint stationary regions, exactness of closed one-forms there, equal contraction constants and stationary cutoffs supported within those regions. Its boundary conclusion requires a whole neighborhood intersection $O\cap E$ inside the region where the horizon gauge is retained. [[lem-author-9e1b6fa65528-stationary-exact-gluing]]

## Proof

**Given:** The full geometric, product, boundary, weak-end and potential hypotheses in the Statement, in ZFC.

**Goal:** Construct the stated single smooth stationary primitive while retaining the original section.

1.1 The vacuum identities give $dF=d\star_gF=0$, $df=2\iota_TF$ and $d\psi=2\iota_T\star_gF$. Thus $\iota_T\Theta_0=4((f-1)\iota_TF+\psi\iota_T\star_gF)=d((1-f)^2+\psi^2)=dD_0$. In an oriented orthonormal coframe of signature $(-,+,+,+)$, direct expansion of a real two-form gives $\star_gF\wedge\star_gF=-F\wedge F$. Contracting this identity with $T$ gives $(\iota_TF)\wedge F+(\iota_T\star_gF)\wedge\star_gF=0$, hence $d\Theta_0=0$. Alternation gives $T\sigma=2(F+i\star_gF)(T,T)=0$, so $D_0$ and $\Theta_0$ are stationary; the Killing flow preserves the metric, its connection and its oriented Hodge star. [given, F1, algebra]

2.1 In the original stationary end, $F=\tfrac12dT^\flat$ gives $F_{0i}=O_5(r^{-2})$ and $F_{ij}=O_5(r^{-3})$. The inverse metric has $g^{0i}=O_6(r^{-2})$, bounded diagonal blocks and bounded differentiated volume factors. In the component formula for $\star_gF$, the spatial components use $F_{0i}$ and are $O_5(r^{-2})$, while $(\star_gF)_{0i}$ uses raised spatial components and is $O_5(r^{-3})$; the terms involving $F_{0i}$ in those raised spatial components have the additional factor $g^{0j}=O_6(r^{-2})$. Therefore $d\psi=O_5(r^{-3})$. The end normalization $\psi\to0$ and integration along each radial ray give $\psi=O_0(r^{-2})$; the differential equation supplies its derivatives of orders one through six with the required gains, so $\psi=O_6(r^{-2})$. Since $f-1=-2/r+O_6(r^{-2})$, the product rules give $D_0=O_6(r^{-2})$ and $(\Theta_0)_{ij}=O_5(r^{-4})$. [given, F1, F2, step 1.1]

3.1 The mass in the original weak end is $1>0$, the metric is smooth, stationary and Ricci-flat, and a far tail has future timelike $T$. All end-normalization hypotheses in [F2] hold. Apply that supplier to obtain $(t',y)$ for the same $T$, with $R=|y|$, $g'_{00}=-1+2/R+O_\infty(R^{-2})$, $g'_{0a}=O_\infty(R^{-2})$, $g'_{ab}=\delta_{ab}+O_\infty(R^{-1})$ and smooth transition $y=q(x)$, $t'=t+F_*(x)$. The supplied normalized potential has the same limit along this end diffeomorphism. Repeating the component calculation of step 2.1 at each finite order gives $F'_{0a}=O_\infty(R^{-2})$, $F'_{ab}=O_\infty(R^{-3})$, $\psi=O_\infty(R^{-2})$ and $(\Theta_0)'_{ab}=O_\infty(R^{-4})$. Together with step 1.1 and original $D_0=O_6(r^{-2})$, these are all the additional hypotheses of the smooth weak-end primitive in [F5]. It supplies a smooth stationary $V_\infty$ on a far tail with contraction constant $c_0=D_0(p)$ and original spatial coefficients $O_5(r^{-3})$. The auxiliary chart is used only to construct this primitive. [given, F1, F2, F5, step 1.1, step 2.1]

3.2 On the original section, the sphere integral of $\Theta_0$ is $O(r^{-2})$ by step 2.1, since Cartesian sphere tangent vectors contribute the area factor $r^2$. Use the supplied physical truncation $B_R$, oriented by the future normal and spacetime orientation, with outward end-sphere orientation on $\Gamma_R$ and the orientation toward the exterior on $S$. Its boundary is $\Gamma_R\sqcup(-S)$. The restricted form is smooth through $S$ and has compact support on this compact region. Stokes in [F3] gives $\int_{\Gamma_R}\Theta_0=\int_S\Theta_0$, so passage to infinity gives $\int_S\Theta_0=0$. Independently, the topological product gives a compact smooth region $\{1\le\rho\le a_*\}$ for any $a_*>1$. Stokes on it gives zero integral over its sphere $\{\rho=a_*\}$. The stationary product and [F3] therefore supply a smooth primitive $A$ of $\Theta_0$ on $E$. Its pullback $a$ to $\Sigma$ satisfies $da=b$, where $b$ is the descended spatial form of $\Theta_0-dt\wedge dD_0$. To obtain a surface primitive without extending $A$ to the boundary, set $\gamma=\Theta_0|_{TS}$ and pull it back to $\mathbb R\times(1,\infty)\times S$. This is a closed two-form of zero sphere period, so [F3] makes it exact on that product. Restricting its smooth primitive to one slice yields a smooth $\beta$ on $S$ with $d\beta=\gamma$. No physical sphere is identified with a topological coordinate sphere. [given, F3, F5, step 1.1, step 2.1]

4.1 The fields $K,Z$ preserve the metric and commute with $T$, hence preserve $d\sigma=2\iota_T(F+i\star_gF)$. Their derivatives of $\sigma$ are constant on the connected neighborhood. Since $K|_S=0$, $K\sigma=0$; integrating the constant $Z\sigma$ around one full circle gives $2\pi Z\sigma=0$. Thus $K,Z$ preserve $\sigma$ and $\Theta_0$. Start with the normal frame supplied by the smooth spacelike boundary and [F4], average its future normal over the circle and normalize. Its unique orthogonal unit spacelike companion in the specified outward component is smooth and invariant as well; the connected circle preserves that component. Thus the resulting frame is orthonormal with the original time and side orientations. Pointwise, two such frames are related by $\widehat n=A n+B\nu$, $\widehat\nu=B n+A\nu$, where $A>0$ and $A^2-B^2=1$, by their orthonormality and the two orientations. If $a n+b\nu=\widehat a\widehat n+\widehat b\widehat\nu$, then $b+a=(A+B)(\widehat b+\widehat a)$ and $b-a=(A-B)(\widehat b-\widehat a)$. Since $A\pm B>0$, the condition $b>|a|$ is equivalent to $\widehat b>|\widehat a|$. Consequently the prescribed outward wedge is unchanged in the invariant frame. Every isometry preserves the metric-selected connection by its uniqueness, and therefore preserves geodesics by the initial-value uniqueness in [F4]. Consequently its differential action on the normal bundle intertwines the exponential map. Fibre dilations commute with that linear action. Shrink the tube uniformly over compact $S$, retaining the full circle action and dilation stability; the $K$ equivariance is on every defined local flow domain. Average $\beta$ and apply relative homotopy and equivariant normalization with this tube. The resulting smooth $V_H$ satisfies $dV_H=\Theta_0$, local $K,Z,T$ invariance and $V_H(T)+D_0=D_0(p)$. At $p$, $T_p=0$ gives $f(p)=0$, so $D_0(p)=1+\psi(p)^2>0$. [given, F1, F4, step 1.1, step 3.2, algebra]

5.1 In the invariant tube frame put $u=b+a$, $v=b-a$. Exponential equivariance and the specified normal boost make the local $T=K-\Omega_H Z$ flow exactly $(s,u,v)\mapsto(\phi^Z_{-\Omega_H t}(s),e^{\kappa t}u,e^{-\kappa t}v)$ while it stays in the tube. Its outward wedge is $u,v>0$. The section $\overline\Sigma$ is locally a graph $a=h(s,b)$ with $h(s,0)=0$: at $S$, projection to $(s,b)$ is nonsingular on its tangent space because its normal-plane tangent direction is spacelike. The smooth inverse function theorem, local extension across the boundary and compactness give a uniform graph neighborhood. Spacelikeness gives $|\partial_bh(s,0)|<1$, and after shrinking there is one $c<1$ with $|h(s,b)|\le cb$ for $b\ge0$. For a local wedge orbit set $j=uv>0$ and center its parameter so that $u=v=\sqrt j$ at time zero. Then $b(t)=\sqrt j\cosh(\kappa t)$ and $a(t)=\sqrt j\sinh(\kappa t)$. Choose $L>0$ with $\tanh(|\kappa|L)>c$. At the two times with $\kappa t=\pm|\kappa|L$, the continuous function $a(t)-h(s(t),b(t))$ has opposite signs. For sufficiently small $j$ the whole bounded-time segment is in the graph neighborhood, so [F6] gives an intersection with the section. It has $b\le C\sqrt j$ for a fixed $C$. The global stationary product makes this intersection unique on the full orbit. [given, F4, F6, step 4.1]

6.1 Choose a section collar $C_H=\{1<\rho<1+\epsilon_H\}$ small enough to lie in the tube and set $U_H=\Phi(\mathbb R\times C_H)$. Transport $V_H$ from this collar by the global stationary product. Uniqueness of the product's section point defines one smooth stationary form $\widetilde V_H$ on $U_H$, with the same exterior derivative and contraction constant, since these identities hold near each section point and are preserved by the stationary flow. For every point of a sufficiently small outward tube, step 5.1 places its unique section point in $C_H$. The segment joining them stays inside the larger tube: $u$ and $v$ vary monotonically, so each is bounded by its endpoint values, and the entire sphere factor is allowed. Local invariance of $V_H$ along this segment shows that the transport equals $V_H$ there. The section point tends uniformly to $S$ as $u,v\to0$, by the bound $b\le C\sqrt{uv}$. Hence there is a smaller whole neighborhood $O$ of $S$ with $O\cap E\subset\Phi(\mathbb R\times\{1<\rho<1+\epsilon_H/3\})$, and $\widetilde V_H=V_H$ on $O\cap E$. The stated wedge attachment ensures that every point of $O\cap E$ is in this argument. No injectivity of a time product at $S$, where $T$ may vanish, is used. [given, F4, F5, F7, step 4.1, step 5.1]

7.1 Apply the stationary lift to $a$ from step 3.2, using $c_0=D_0(p)$, to obtain a smooth stationary $V=(c_0-D_0)dt+\pi^*a$ on $E$ with $dV=\Theta_0$ and $V(T)+D_0=c_0$. Choose $R_*>0$ sufficiently large that the physical tail $\{r>R_*\}$ lies in the end-primitive domain of step 3.1. Its closed tail is disjoint from $S$ by the supplied end-attachment hypothesis. Shrink the topological section collar so that its closure lies in the relative neighborhood $\overline\Sigma\setminus\{r\ge R_*\}$ of compact $S$, and shrink $O$ again by step 6.1 for that smaller collar. The stationary product then makes $U_H$ disjoint from $U_\infty=\Phi(\mathbb R\times\{r>R_*\})$. Both $U_H$ and $U_\infty$ are stationary products of $\mathbb R$ with a spherical annulus, hence have exact closed one-forms by [F3]. In particular the differences $\widetilde V_H-V$ and $V_\infty-V$ are exact there. Their contractions with $T$ vanish, so every scalar primitive $h$ of a difference satisfies $Th=dh(T)=0$. Use the smooth step function of [F6] in $\rho$ to choose $\eta_H=1$ for $1<\rho<1+\epsilon_H/3$ and $\eta_H=0$ for $\rho\ge1+2\epsilon_H/3$; choose $R_*<R_1<R_2$ and define $\eta_\infty$ using the same step function in the physical radius $r$, zero for $r\le R_1$ and one for $r\ge R_2$, extended by zero off the physical end. Both cutoffs are transported by the stationary product. The end cutoff is smooth across its extension seam because it vanishes on an end neighborhood of that seam; its support in $E$ lies in the closed stationary lift of $\{r\ge R_1\}\subset\{r>R_*\}$. The supplied closed-tail condition and the product diffeomorphism justify that closure assertion. The horizon cutoff has support inside $U_H$ because its nonzero set is confined to $1<\rho<1+2\epsilon_H/3$, with a positive gap from the outer edge of $C_H$. Thus these are smooth stationary functions with supports in the respective disjoint regions, using $\rho$ only at the horizon and $r$ only at the end. All hypotheses of stationary exact gluing now hold, including the whole-neighborhood intersection in step 6.1. Its output $W_0$ equals $V_H$ on a neighborhood of $S$, equals $V_\infty$ on a far tail, and globally satisfies $dW_0=\Theta_0$, stationarity and $W_0(T)=D_0(p)-D_0$. It inherits the local $K,Z$ invariance and original $O_5(r^{-3})$ spatial decay. The original section and any of its supplied maximality remain fixed. [given, F3, F5, F6, F7, step 3.1, step 3.2, step 4.1, step 6.1] ∎

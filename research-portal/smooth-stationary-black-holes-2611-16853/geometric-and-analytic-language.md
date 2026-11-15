---
title: Stationary geometry and analytic data
description: Define the common Lorentzian, causal, horizon, hypersurface and
  field conventions, together with weighted elliptic, graph, continuation and
  area data. These fifteen mathematical interfaces supply both later
  prerequisite pages without importing article-specific conclusions.
status: published
dependency_level: 0
---

**Purpose:** Define the common Lorentzian, causal, horizon, hypersurface and field conventions, together with weighted elliptic, graph, continuation and area data. These fifteen mathematical interfaces supply both later prerequisite pages without importing article-specific conclusions.

## Stationary Lorentzian data and tensor conventions

[Open item](item-def-stationary-lorentzian-data) · level 0


### Definition

Work in ZFC, including the axiom of choice. Stationary Lorentzian data here consist of a connected smooth four-manifold $M$ without boundary, an orientation, a smooth Lorentzian metric $g$ of signature $(-,+,+,+)$, a time orientation $N$, and a smooth vector field $T$ satisfying $\mathcal L_Tg=0$. The orientation is a smooth choice of a positive ray in $\det T_pM$ at each point. The time orientation is a smooth field with $g(N,N)<0$; a timelike vector $v$ is future-directed when $g(v,N)<0$.

The metric is a smooth symmetric nondegenerate covariant two-tensor with one negative and three positive directions at each point. The Lie derivative $\mathcal L_Tg$ is $\frac{d}{dt}|_{t=0}\Phi_t^*g$, where $\Phi_t$ is the local flow of $T$; a field satisfying its vanishing is called a Killing field. Thus stationary refers here to the specified pair $(g,T)$; it does not assert that $T$ is timelike everywhere or that its flow is complete. For a designated open region called an end, the additional convention that it is a stationary end requires $T$ to be future timelike throughout that region. Further topology or asymptotic conditions on an end must be stated separately.

Let $\nabla$ be the Levi–Civita connection: the unique torsion-free affine connection compatible with $g$. Its curvature convention is $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$. In a coordinate frame write $R(\partial_c,\partial_d)\partial_b=R^a{}_{bcd}\partial_a$ and $\operatorname{Ric}_{bd}=R^a{}_{bad}$. The Ricci tensor is denoted $\operatorname{Ric}(g)$.

Put $T^\flat=g(T,\cdot)$ and $f=-g(T,T)$. In coordinates, $T_a=g_{ab}T^b$ and $g^{ab}$ denotes the inverse matrix of $g_{ab}$. Repeated upper and lower indices are summed from $0$ to $3$. Raising indices uses $g^{ab}$ and lowering them uses $g_{ab}$; a contraction or raised tensor associated with another metric uses that metric and its own inverse.

### Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)

[math:def-oriented-smooth-manifold-and-oriented-chart](https://alphabetamath.cc/item/def-oriented-smooth-manifold-and-oriented-chart)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### Facts & Assumptions

[A1] The set-theoretic convention is ZFC, including the axiom of choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The Lorentzian interface gives the metric, time-orientation and future-directed conventions stated above. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[F2] The Killing-field interface defines the Lie derivative using the local flow and defines a Killing field by its vanishing. [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[F3] A metric-selected connection is torsion-free and metric-compatible; for the stated smooth nondegenerate metric there is exactly one such connection. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection) [physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[F4] The inverse-metric interface supplies the inverse and the lowering and raising maps for the stated nondegenerate metric. [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[F5] The curvature interface fixes the displayed curvature and Ricci conventions for the metric-selected connection. [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)

[F6] An orientation is a smooth choice of a ray in the determinant line of each tangent space. [math:def-oriented-smooth-manifold-and-oriented-chart](https://alphabetamath.cc/item/def-oriented-smooth-manifold-and-oriented-chart)

### Justification

**Given:** The data and hypotheses in the Definition.

**Goal:** Show that the named fields and conventions are well-defined under those hypotheses.

1.1 The metric and time-orientation hypotheses place $(M,g,N)$ in the Lorentzian interface; the chosen orientation is the determinant-line datum in that interface's smooth-manifold setting. The local-flow Lie derivative and the Killing condition therefore have the stated meanings. The end condition is a further pointwise requirement on the designated region, not an assertion that such a region exists. [given, F1, F2, F6]

2.1 Nondegeneracy and smoothness supply the unique metric-compatible torsion-free connection and the inverse metric. The curvature interface then supplies the displayed Ricci contraction, while $T^\flat$ and $f$ are pointwise contractions of the supplied smooth fields. Raising and lowering with the inverse and metric of the metric currently specified is consequently unambiguous. This establishes the stated conventions without asserting completeness or an existence theorem for an end. [given, F3, F4, F5, step 1.1] ∎

### External input

Carroll supplies the symmetric nondegenerate metric and Lorentzian signature conventions in Chapter 2. The flow definition of the Lie derivative and the Killing condition are recorded in Chapter 5; only their restriction to local flow domains is used here. Time orientation and future direction use the declared Lorentzian interface.


## Spacelike sections, maximality and lapse–shift data

[Open item](item-def-spacelike-maximal-hypersurface-data) · level 0


### Definition

Let $(M,g)$ be a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$ with its Levi–Civita connection $\nabla$, and let $\Sigma\subset M$ be a smooth embedded spacelike hypersurface: its tangent spaces are three-dimensional and $g$ restricts positively on each of them. Let $n$ be the future-directed unit normal, so $g(n,n)=-1$ and $g(n,U)=0$ for tangent $U$. The induced Riemannian metric is $h(U,V)=g(U,V)$, and we use the second fundamental form convention $k(U,V)=-g(\nabla_U n,V)$.

The mean curvature in this convention is $H=-\operatorname{tr}_h k$, where the trace is contraction with the inverse of $h$. Equivalently, $H=\operatorname{div}_g n$ along $\Sigma$: here the divergence is the trace of $V\mapsto\nabla_V\widetilde n$ for any smooth local unit timelike extension $\widetilde n$ of $n$, satisfying $g(\widetilde n,\widetilde n)=-1$ throughout its ambient neighborhood. Such extensions exist locally by normalization. The hypersurface is **maximal** when $H=0$ everywhere.

For any smooth ambient vector field $T$, its **lapse** along $\Sigma$ is $N=-g(T,n)$ and its **shift** is $X=T-Nn$. Thus $X$ is tangent to $\Sigma$ and $T=Nn+X$. These names impose no sign on $N$.

For the boundary convention, suppose separately that $\overline\Sigma\subset M$ is a connected smooth embedded three-dimensional submanifold with compact boundary, supplied with its manifold-with-boundary smooth structure and smooth inclusion, whose interior is $\Sigma$. Suppose that $g$ restricts to a positive-definite smooth metric $\overline h$ on all tangent spaces of $\overline\Sigma$, including its boundary. Its intrinsic distance is the infimum of $\overline h$-lengths of piecewise $C^1$ curves in $\overline\Sigma$ joining the two points. **Complete up to the compact boundary** means that this metric space, with the boundary included, is complete: every Cauchy sequence converges in $\overline\Sigma$. It does not assert completeness of the interior with its own intrinsic distance. For a disconnected extension, the convention applies separately to each connected component.

### Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)

[math:thm-riemannian-distance-is-a-metric](https://alphabetamath.cc/item/thm-riemannian-distance-is-a-metric)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)

[math:def-cauchy-in-metric](https://alphabetamath.cc/item/def-cauchy-in-metric)

[math:def-metric-convergence](https://alphabetamath.cc/item/def-metric-convergence)

### Facts & Assumptions

[A1] The authoring convention includes the Axiom of Choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] A spacelike embedded hypersurface has positive-definite induced tangent forms. [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[F2] On such a hypersurface the future unit normal is unique and smooth; the induced metric is Riemannian and the positive-sign form $(U,V)\mapsto g(\nabla_U n,V)$ is a well-defined smooth symmetric tensor. [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[F3] The Levi–Civita connection is metric compatible: $Vg(Y,Z)=g(\nabla_VY,Z)+g(Y,\nabla_VZ)$. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F4] A Riemannian metric is a smooth positive-definite symmetric covariant two-tensor, with boundaries allowed where stated. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[F5] The intrinsic Riemannian distance is the infimum of lengths of piecewise $C^1$ connecting curves, and is a metric on a connected Riemannian manifold, including the stated boundary case. [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold) [math:thm-riemannian-distance-is-a-metric](https://alphabetamath.cc/item/thm-riemannian-distance-is-a-metric)

[F6] An embedded smooth submanifold with boundary is supplied with a manifold-with-boundary smooth structure for which its inclusion into the ambient manifold is a smooth embedding. [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)

### Justification

The normal, its tangential covariant derivatives, $h$ and $k$ are well defined and smooth by the stated hypersurface supplier; its second fundamental form has the opposite sign from $k$. The inverse of positive-definite $h$ defines the trace, so maximality is a definite condition. Choose a smooth local extension $v$ of $n$ supplied by the normal lemma. Near each point of $\Sigma$, continuity permits shrinking its ambient neighborhood so that $g(v,v)<0$. Then $\widetilde n=v/\sqrt{-g(v,v)}$ is smooth, has unit timelike length throughout that neighborhood and agrees with $n$ along $\Sigma$.

For any such unit timelike extension, metric compatibility gives $g(\nabla_{\widetilde n}\widetilde n,\widetilde n)=\tfrac12\widetilde n(g(\widetilde n,\widetilde n))=0$ throughout the neighborhood. On $\Sigma$, in a $g$-orthonormal frame $n,e_1,e_2,e_3$ with tangent $e_i$, the divergence trace is $-g(\nabla_n\widetilde n,n)+\sum_{i=1}^3g(\nabla_{e_i}\widetilde n,e_i)$. Its normal term vanishes and its tangent term equals $-\operatorname{tr}_h k$. The normal lemma makes the tangential derivatives independent of extension, so every local unit timelike extension gives the same divergence on $\Sigma$.

Finally, $g(X,n)=g(T,n)-N g(n,n)=0$, so the normal supplier's orthogonal decomposition makes $X$ tangent; the formula gives the unique such decomposition. The embedded-submanifold-with-boundary supplier specifies the smooth structure and smooth inclusion used in the boundary convention. The positive-definiteness hypothesis then gives a Riemannian metric smooth up to the boundary, and the distance suppliers, whose metric argument includes boundary half-charts, make the stated Cauchy-completeness condition well defined. No existence of a maximal hypersurface or complete extension is asserted.


## Null expansions, screen quotients and focal data

[Open item](item-def-null-screen-expansion-and-focal-data) · level 0


### Definition

Assume the axiom of choice. Let $(M,g,N)$ be a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$, with metric-selected connection $\nabla$. A spacelike two-surface $S$ is a nonempty smooth embedded two-manifold without boundary whose induced metric $\gamma=g|_{TS}$ is positive definite. On an open set $U\subseteq S$, choose smooth future null normal fields $L,K$ with $g(L,K)=-2$. Thus $L$ and $K$ are nonzero, orthogonal to $TS$, null, and future-directed.

For tangent fields $X,Y$ on $U$, the null second fundamental form, expansion, and shear of $L$ are respectively $\chi_L(X,Y)=g(\nabla_XL,Y)$, $\theta_L=\operatorname{tr}_\gamma\chi_L$, and $\widehat\chi_L=\chi_L-\frac12\theta_L\gamma$. Here the derivative of $L$ along $S$ uses the pullback connection and the trace uses the inverse of the positive metric $\gamma$.

Suppose a smooth map $F:U\times J\to M$, with $J$ an open interval containing zero, satisfies $F(p,0)=p$, $\partial_\lambda F(p,0)=L_p$, and has future null affine geodesics $\lambda\mapsto F(p,\lambda)$ as its parameter curves. Write $L=\partial_\lambda F$ along this map and require $g(L,dF(X,0))=0$ for every $X\in T_pU$. The screen at $(p,\lambda)$ is $\mathscr S=L^\perp/\mathbb RL$, equipped with $\bar\gamma([V],[W])=g(V,W)$. Fibers are indexed by the parameter domain, even when distinct branches of $F$ meet.

The normal screen Jacobi map is $A_\lambda:T_pS\to\mathscr S_{(p,\lambda)}$, $A_\lambda X=[dF_{(p,\lambda)}(X,0)]$. A focal instant to $S$ on this generator is a positive $\lambda\in J$ where $A_\lambda$ loses rank; the corresponding image is a focal point. The first focal instant, when one exists, is the least positive focal instant.

On the connected regular interval containing $0$, where $A_\lambda$ is invertible and the induced section metric is positive, let $\mathcal D_L[V]=[D_\lambda V]$ be the screen derivative and set $B=A' A^{-1}$, where the prime is the screen derivative. The optical expansion is $\theta=\operatorname{tr}B$ and the optical shear is $\sigma=B-\frac12\theta\,\mathrm{id}$. At $\lambda=0$ these correspond to $\theta_L$ and $\widehat\chi_L$ under the screen identification.

For comparison, use the following causal-reachability conventions. Future causal and future timelike curves here are locally absolutely continuous curves whose velocities are nonzero and future causal or future timelike, respectively, almost everywhere. A point $q$ belongs to $I^+(p)$ when a future timelike curve on a nondegenerate compact parameter interval joins $p$ to $q$. It belongs to $J^+(p)$ when $q=p$ or such an interval carries a future causal curve joining $p$ to $q$. Put $I^+(S)=\bigcup_{p\in S}I^+(p)$, $J^+(S)=\bigcup_{p\in S}J^+(p)$, and $E^+(S)=J^+(S)\setminus I^+(S)$. When the set of $t\geq0$ in the parameter domain such that the entire segment $F(p,[0,t])$ lies in $E^+(S)$ is nonempty and has a finite supremum $c$ in that domain, call $c$ the future boundary cut parameter of this generator relative to $S$ and $F(p,c)$ its boundary cut point. An intersection of distinct generators means $F(p,\lambda)=F(q,\mu)$ for distinct parameter curves, for example $p\ne q$. These are separate definitions: focal rank loss is local differential data, whereas the cut condition and intersections involve global reachability or multiple branches.

### Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)

[physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)

[physics:lem-gr-fx-null-focal-boundary-exclusion](https://alphabetamath.cc/physics/item/lem-gr-fx-null-focal-boundary-exclusion)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### Facts & Assumptions

[A1] The axiom of choice implies dependent choice and hence countable choice, supplying the choice assumptions used by the geometric suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice), [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice).

[F1] The null-screen geometry supplier defines the congruence, its screen Jacobi map, focal instants and optical quantities under the stated hypotheses. [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)

[F2] The normal-plane and screen supplier gives local normalized null pairs, the positive screen metric, and well-defined symmetric null second fundamental form and screen derivative. [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)

[F3] Under its stated hypotheses, a focal instant places points sufficiently shortly thereafter in $I^+(S)$. [physics:lem-gr-fx-null-focal-boundary-exclusion](https://alphabetamath.cc/physics/item/lem-gr-fx-null-focal-boundary-exclusion)

### Justification

The supplier for null normal planes supplies local pairs and shows that the form and quotient metric are well-defined; its screen derivative is independent of the representative. The null-screen geometry supplier identifies the initial screen with $T_pS$, makes $A$ invertible on the stated regular interval, and identifies the initial optical data with the surface quantities. The cut parameter is a conditional supremum definition: existence of a finite attained cut is not asserted. The focal-exclusion supplier gives the stated local causal consequence of a focal instant; it does not identify the three notions or assert that a cut or an intersection exists.


## Bifurcate Killing horizons, rotation and normalization

[Open item](item-def-bifurcate-killing-horizon-data) · level 0


### Definition

Work in a smooth time-oriented Lorentzian four-manifold $(M,g)$ of signature $(-,+,+,+)$, with metric-compatible Levi–Civita connection $\nabla$, and let $K$ be a smooth Killing field, meaning $\mathcal L_K g=0$. A smooth embedded hypersurface $H$ is **null** if the restriction of $g$ to each tangent space $T_pH$ has a nonzero radical: the vectors in $T_pH$ orthogonal to all of $T_pH$. It is a **Killing horizon for $K$** when $H_*:=\{p\in H:K_p\ne0\}$ is nonempty and dense in $H$ and, on $H_*$, $K$ is tangent and normal to $H$. The null normal line is the radical of the induced form. An **integral curve of this line field**, or **horizon generator**, means here a smooth curve $\gamma:I\to H$, where $I\subset\mathbb R$ is a nonempty open interval, such that $\dot\gamma(s)\ne0$ and $\dot\gamma(s)$ lies in the null normal line at $\gamma(s)$ for every $s\in I$. Curves related by a smooth diffeomorphic reparameterization are identified; restrictions to open subintervals are allowed generator segments. No maximality, completeness, affine parametrization or preferred parameter scale is implicit.

The **signed surface gravity** of this specified $K$ on $H_*$ is the unique smooth scalar $\kappa_H$ satisfying the ambient covector equation $d(g(K,K))=-2\kappa_H K^\flat$, where $K^\flat=g(K,\cdot)$. Equivalently, $\nabla_KK=\kappa_H K$ on $H_*$. A chosen future branch is a specified branch with its future direction; neither the sign nor constancy of $\kappa_H$ follows from the terminology.

A **bifurcate Killing horizon** here consists of two distinct specified smooth embedded null hypersurfaces $H_+$ and $H_-$ in a common neighborhood of a smooth spacelike embedded two-surface $S$, each a Killing horizon for the same $K$, such that $K=0$ on $S$, their intersection near each point of $S$ is $S$, and $T_pH_+\cap T_pH_-=T_pS$. Spacelike means that the induced metric on $S$ is positive definite. The surface $S$ is the **bifurcation surface**. A surface-gravity value at $p\in S$ is specified by the common value only when the two branch scalars extend smoothly to $p$ along their respective branches and agree there. The equation at $K=0$ alone fixes no value.

For a specified stationary Killing field $T$, meaning a Killing field timelike on a specified nonempty open region, a horizon is **non-rotating relative to $T$** if $T_p$ lies in the null normal line at every point of the horizon; it is **rotating relative to $T$** if that tangency fails somewhere. Zero vectors satisfy the tangency condition. A **normalization** specifies the scale of $K$; replacing $K$ by $aK$ for a nonzero constant $a$ replaces $\kappa_H$ by $a\kappa_H$. Thus a numerical surface gravity, or boost rate when that term is used for this normalized scalar, requires the normalization to be stated. No existence, constancy, nonzero-value, field-equation or global-extension assertion is included.

### Definition references

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:thm-gr-killing-and-on-shell-matter-identities](https://alphabetamath.cc/physics/item/thm-gr-killing-and-on-shell-matter-identities)

[physics:def-emg-causal-solution-and-horizon-vocabulary](https://alphabetamath.cc/physics/item/def-emg-causal-solution-and-horizon-vocabulary)

### Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice, which supplies the countable choice used in the inherited smooth-manifold conventions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The horizon supplier defines the signed scalar on the nonzero-generator part and the bifurcation surface with the stated transversality and extension qualifications. [physics:def-emg-causal-solution-and-horizon-vocabulary](https://alphabetamath.cc/physics/item/def-emg-causal-solution-and-horizon-vocabulary)

[F2] A Killing field satisfies $\nabla_aK_b+\nabla_bK_a=0$, and the metric-selected connection is metric compatible. [physics:thm-gr-killing-and-on-shell-matter-identities](https://alphabetamath.cc/physics/item/thm-gr-killing-and-on-shell-matter-identities) [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

### Justification

The horizon supplier establishes that the scalar in the ambient covector equation exists uniquely and smoothly on $H_*$; density makes a continuous extension unique if it exists. By metric compatibility and the Killing equation, $\nabla_a(g(K,K))=2K^b\nabla_aK_b=-2K^b\nabla_bK_a$. Nondegeneracy of $g$ therefore makes the covector equation equivalent to $\nabla_KK=\kappa_H K$. Rescaling $K$ by a nonzero constant multiplies the left side of the covector equation by $a^2$ and $K^\flat$ by $a$, giving the stated rescaling of $\kappa_H$. The null normal line and tangency condition are pointwise conditions on the specified data; the definition does not assert that suitable data exist.

### External input

The horizon and bifurcation definitions, including existence and smoothness of the signed scalar on $H_*$, are supplied by [physics:def-emg-causal-solution-and-horizon-vocabulary](https://alphabetamath.cc/physics/item/def-emg-causal-solution-and-horizon-vocabulary) under its Definition (b) hypotheses and Proof 2.1. Reall, Section 5.3, equations (5.21)–(5.22), independently states the Killing-equation characterization used in [F2]. [General Relativity, printed p. 56](https://www.damtp.cam.ac.uk/user/hsr1000/part3_gr_lectures.pdf) This lecture-note citation is limited to that identity; the horizon, density and branch-extension conventions come from the declared mathematical supplier.


## Differentiated asymptotic bounds and parameter uniformity

[Open item](item-def-stationary-asymptotic-decay-data) · level 0


### Definition

Fix a Cartesian exterior chart $E=\{x\in\mathbb R^3: r=|x|>R_0\}$ with $R_0>0$. Let $m$ be a nonnegative integer, $b\in\mathbb R$, and let $u$ be a scalar or a finite array of scalar functions of class $C^m$ on $E$. For a multi-index $\beta=(\beta_1,\beta_2,\beta_3)$ of nonnegative integers write $|\beta|=\beta_1+\beta_2+\beta_3$ and $\partial^\beta=\partial_{x^1}^{\beta_1}\partial_{x^2}^{\beta_2}\partial_{x^3}^{\beta_3}$. The notation $u=O_m(r^{-b})$ means that there are a radius $R_1>R_0$ and finite constants $C_\beta\geq0$ such that every component satisfies $|\partial^\beta u(x)|\leq C_\beta r^{-b-|\beta|}$ for all $|\beta|\leq m$ and $r\geq R_1$. The estimate is uniform over angular directions in this chart.

For a family $(u_\lambda)_{\lambda\in\Lambda}$ on the same exterior chart, the estimate is **uniform on the parameter set** $\Lambda$ when the same radius and constants work for every $\lambda\in\Lambda$. Separate estimates for each parameter allow these quantities to depend on $\lambda$ and do not by themselves imply uniformity, including as a parameter approaches a boundary value.

For $0<\alpha<1$, define the Hölder seminorm on a set $A$ by $[v]_{\alpha;A}=\sup_{x,y\in A,\,x\ne y}|v(x)-v(y)|/|x-y|^\alpha$, allowing $+\infty$. Write $A_R=\{x\in\mathbb R^3:R<|x|<2R\}$. A **weighted $C^{m,\alpha}$ bound of decay order $b$** means that for some $R_1>R_0$ and finite $C$, for every $R\geq R_1$ and every component,
$$\sum_{|\beta|\leq m} R^{b+|\beta|}\sup_{A_R}|\partial^\beta u|+\sum_{|\beta|=m}R^{b+m+\alpha}[\partial^\beta u]_{\alpha;A_R}\leq C.$$
For a family, uniformity means that the same $R_1$ and $C$ work for every parameter. These bounds are chart-dependent data; they do not assert coordinate invariance or the existence of a particular end.

### Definition references

[math:def-ck-and-multi-index-notation-in-several-variables](https://alphabetamath.cc/item/def-ck-and-multi-index-notation-in-several-variables)

[physics:def-gr-fx-adm-end](https://alphabetamath.cc/physics/item/def-gr-fx-adm-end)

[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

### Facts & Assumptions

[F1] The fixed-chart end interface uses differentiated $O_k$ bounds with Cartesian derivatives and angular uniformity. [physics:def-gr-fx-adm-end](https://alphabetamath.cc/physics/item/def-gr-fx-adm-end)

[F2] Hölder seminorms measure differences divided by a power of Euclidean distance, and scaled norms weight derivatives and seminorms by the corresponding radius powers. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

### Justification

The finite array and the finite set of multi-indices allow one common radius to be chosen as the maximum of finitely many radii in the componentwise convention of [F1]. The definition uses no limiting choice of constants. On $A_R$, the first sum in the weighted bound controls each derivative at its stated decay order, since $R<r<2R$; the second sum explicitly imposes the scaled Hölder control described in [F2]. For example, on $r>1$ let $u_s(x)=s^{-1}r^{-1}$ for $0<s\leq1$. Each $u_s$ is $O_0(r^{-1})$ with constant $s^{-1}$, but no common constant works for all $s$, even at any one fixed point of the exterior. Thus separate bounds need not be uniform.


## Complex self-dual forms and metric-dependent contraction

[Open item](item-def-complex-self-dual-two-form-data) · level 0


### Definition

Assume the Axiom of Countable Choice $\mathrm{AC}_\omega$: every countable family of nonempty sets has a choice function.

Let $(M,g,N,o)$ be a smooth, oriented and time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$. A real two-form is a smooth section of $\bigwedge^2T^*M$; a complex two-form is a section of its complexification and can be written uniquely as $U+iV$ with real two-forms $U,V$. Extend the metric Hodge star $\star_g$ complex linearly by $\star_g(U+iV)=\star_gU+i\star_gV$. In this convention a complex two-form $Z$ is called self-dual when $\star_gZ=-iZ$.

For a real two-form $F$, define its complex self-dual form by $\mathcal F=F+i\star_gF$. Raise both indices using the inverse metric and define the complex bilinear contraction $\mathcal F^2=\mathcal F_{ab}\mathcal F^{ab}$, with summation over both indices and without complex conjugation or a factor of one half.

Let $A:TM\to TM$ be a smooth fiberwise invertible real-linear bundle map over the identity. Its algebraic pullbacks are the covariant two-tensors $(A^*g)_p(u,v)=g_p(A_pu,A_pv)$ and $(A^*F)_p(u,v)=F_p(A_pu,A_pv)$ for $u,v\in T_pM$. The latter is again a real two-form. This pullback is defined fiberwise and $A$ need not be the differential of a diffeomorphism.

### Definition references

[physics:def-emg-lorentzian-forms](https://alphabetamath.cc/physics/item/def-emg-lorentzian-forms)

[physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[math:def-direct-sum-model-of-complexification](https://alphabetamath.cc/item/def-direct-sum-model-of-complexification)

[math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle](https://alphabetamath.cc/item/def-smooth-vector-bundle-rank-fibre-and-trivial-bundle)

[math:def-smooth-section-local-section-and-support](https://alphabetamath.cc/item/def-smooth-section-local-section-and-support)

[math:def-vector-bundle-map-over-a-smooth-base-map](https://alphabetamath.cc/item/def-vector-bundle-map-over-a-smooth-base-map)

[math:thm-sylvesters-law-of-inertia](https://alphabetamath.cc/item/thm-sylvesters-law-of-inertia)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

### Facts & Assumptions

[A1] Assume the Axiom of Countable Choice $\mathrm{AC}_\omega$: every countable family of nonempty sets has a choice function, as defined in [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice). This is the background assumption of the geometric suppliers used in [F1] and [F2].

[F1] The oriented, time-oriented Lorentzian data and real differential forms are as in [physics:def-emg-lorentzian-forms](https://alphabetamath.cc/physics/item/def-emg-lorentzian-forms).

[F2] The metric Hodge star is a smooth real-linear bundle map and satisfies $\star_g^2=-\operatorname{id}$ on real two-forms. [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[F3] The nondegenerate metric has an inverse, which raises tensor indices. [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[F4] For a real vector space $V$, the direct-sum complexification has underlying pairs $(u,v)$, written $u+iv$, with $(a+bi)(u+iv)=(au-bv)+i(bu+av)$. [math:def-direct-sum-model-of-complexification](https://alphabetamath.cc/item/def-direct-sum-model-of-complexification)

[F5] Smooth real vector bundles are described by fibrewise linear local trivializations; a smooth section is a smooth right inverse to the bundle projection. A bundle map over the identity is a smooth map preserving the projection and linear on each fibre. [math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle](https://alphabetamath.cc/item/def-smooth-vector-bundle-rank-fibre-and-trivial-bundle), [math:def-smooth-section-local-section-and-support](https://alphabetamath.cc/item/def-smooth-section-local-section-and-support), [math:def-vector-bundle-map-over-a-smooth-base-map](https://alphabetamath.cc/item/def-vector-bundle-map-over-a-smooth-base-map)

[F6] The intrinsic exterior pairing on real two-forms has component expression $\langle P,Q\rangle_g=\tfrac12P_{ab}Q^{ab}$. [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[F7] The inertia of a finite-dimensional real symmetric bilinear form is independent of its diagonalizing basis, so invertible real congruence preserves the numbers of positive, negative and zero entries. [math:thm-sylvesters-law-of-inertia](https://alphabetamath.cc/item/thm-sylvesters-law-of-inertia)

### Justification

Here is the smooth complexification construction used in the Definition. Put $E=\bigwedge^2T^*M$. As a set over $M$, take $E_{\mathbb C}=\{(u,v)\in E\times E:\pi(u)=\pi(v)\}$ with projection $(u,v)\mapsto\pi(u)$, and equip each fibre with the scalar operations of [F4]. Each real local trivialization of $E$ gives coordinates $(p,u,v)\in U\times\mathbb R^6\times\mathbb R^6$ on this set. If the real transition matrix is $h(p)$, the pair transition is $(p,u,v)\mapsto(p,h(p)u,h(p)v)$. It is smooth with smooth inverse given by the inverse transition matrix; the identity and cocycle relations are inherited from those of $E$. Identifying $(u,v)$ with $u+iv\in\mathbb C^6$, this transition is complex-linear by [F4]. Thus these coordinates give the smooth complex vector bundle meant here, with underlying real bundle of rank twelve in the sense of [F5]. A section is smooth exactly when its two component sections are smooth, since both projection to the pair components and formation of the pair are smooth in these coordinates. Consequently every smooth complex two-form has unique globally defined real and imaginary smooth two-forms $U,V$.

For any smooth real-linear bundle map $S:E\to E$, define $S_{\mathbb C}(u+iv)=S(u)+iS(v)$. Uniqueness of the pair makes this well defined. Real linearity gives $S_{\mathbb C}((a+bi)(u+iv))=(aS(u)-bS(v))+i(bS(u)+aS(v))=(a+bi)S_{\mathbb C}(u+iv)$, so it is complex-linear. In the pair coordinates its matrix is the same smooth matrix of $S$ on both components, so it is smooth. Apply this construction to the map $\star_g$ of [F2]. By [F2], $\star_g\mathcal F=\star_gF-iF=-i\mathcal F$, so the stated name agrees with the chosen eigenvalue convention.

For real two-forms $P,Q$, use the inverse metric of [F3] in each covector slot to form $Q^{cd}=g^{ce}g^{df}Q_{ef}$. By [F6], the full contraction $C(P,Q)=P_{ab}Q^{ab}$ equals $2\langle P,Q\rangle_g$, so it is intrinsically defined and independent of the frame. Extend this real bilinear pairing complex bilinearly, using the unique real and imaginary parts just constructed. In particular $C(U+iV,U+iV)=C(U,U)-C(V,V)+i(C(U,V)+C(V,U))$. Its component expression is exactly the full sum in the Definition, with no conjugation and no factor of one half, so that expression is well defined in every frame.

The bundle map $A$ has the meaning in [F5], with base map $\operatorname{id}_M$. In any local frame its matrix entries $A^i{}_a$ are smooth, since they are components of the smooth map applied to the local basis sections. The pullback components are $(A^*g)_{ab}=g_{ij}A^i{}_aA^j{}_b$ and $(A^*F)_{ab}=F_{ij}A^i{}_aA^j{}_b$, hence smooth. The defining fibrewise evaluations are intrinsically bilinear, symmetric for $g$ and alternating for $F$, so these local expressions agree on overlaps and the latter defines a real two-form. If $(A^*g)_p(u,v)=0$ for every $v$, surjectivity of $A_p$ implies $g_p(A_pu,w)=0$ for every $w$, whence $A_pu=0$ and then $u=0$. Thus $A^*g$ is nondegenerate. Its matrix is $A_p^{\mathsf T}g_pA_p$, an invertible congruence, so [F7] gives the same signature $(-,+,+,+)$ as $g$. This reasoning uses only the fibrewise bundle map, with no assumption that it is a differential.

### External input

The Hodge definition and square formula in Carroll's Lecture Notes on General Relativity, §1, equations (1.87)–(1.88), PDF p. 30, provide independent background for the chosen convention. Only those equations and the accompanying signature explanation were consulted. The smooth Hodge map and its square used above are supplied by [F2]; the complex bundle, extension, contraction application and pullback justification are local constructions from [F1]–[F7].


## Geometric electrovacuum equations and charge convention

[Open item](item-def-source-free-geometric-electrovacuum-data) · level 0


### Definition

Work with the Axiom of Choice, in particular countable choice. Let $M$ be a smooth Hausdorff second-countable four-manifold without boundary, $g$ a smooth Lorentzian metric of signature $(-,+,+,+)$, $N$ a smooth timelike field selecting the future direction, and $o$ an independently specified orientation. Let $F$ be a smooth real two-form. The metric-selected connection is the torsion-free metric-compatible connection $\nabla$; use $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$ and its Ricci contraction $\operatorname{Ric}_{bd}=R^a{}_{bad}$. These conventions follow [physics:def-emg-lorentzian-forms](https://alphabetamath.cc/physics/item/def-emg-lorentzian-forms).

The Hodge map $\star_g$ is determined by $g$ and $o$ through $\alpha\wedge\star_g\beta=\langle\alpha,\beta\rangle_g\,\mathrm{vol}_g$, where the pairing is the metric-induced pairing on forms and $\mathrm{vol}_g$ agrees with $o$; see [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus). A **source-free geometric electrovacuum datum** is the tuple $(M,g,N,o,F)$ satisfying the equations in [physics:def-emg-xs-geometric-electrovac](https://alphabetamath.cc/physics/item/def-emg-xs-geometric-electrovac) with zero cosmological constant:

$$dF=0,\qquad d(\star_gF)=0,\qquad \operatorname{Ric}_{ab}=2\left(F_{ac}F_b{}^c-\frac14g_{ab}F_{cd}F^{cd}\right).$$

Indices are raised using $g^{-1}$. These are defining tensor equations, with no global potential, asymptotic flatness, horizon, or existence assertion included.

Let $S\subset M$ be a compact oriented smooth embedded two-manifold without boundary. It is **spacelike** when the restriction of $g$ to every tangent plane $T_pS$ is positive definite. Its orientation is specified independently of $o$. With $i:S\hookrightarrow M$ the inclusion, define the geometric electric and magnetic flux parameters by

$$Q_E(S):=\frac1{4\pi}\int_S i^*(\star_gF),\qquad Q_M(S):=\frac1{4\pi}\int_S i^*F.$$

The orientation and factor $4\pi$ are fixed before charges are compared; no SI constants are inserted into this normalization.

### Justification

The cited Lorentzian and Hodge suppliers define the connection, curvature, exterior derivative and smooth Hodge map under the stated hypotheses. The equations therefore compare smooth tensors of matching types and select a class of tuples; they do not assert that a specified tuple satisfies them. The electrovacuum supplier fixes the displayed curvature and flux normalization. For the broader surfaces used here, the inclusion $i:S\hookrightarrow M$ is smooth, so [math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges](https://alphabetamath.cc/item/prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges) makes $i^*F$ and $i^*(\star_gF)$ smooth two-forms on $S$. By [math:def-compactly-supported-differential-form](https://alphabetamath.cc/item/def-compactly-supported-differential-form), the support of each is the closure in $S$ of its nonzero locus. Each support is therefore closed in compact $S$ and is compact by [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact). [math:prop-integration-over-an-oriented-embedded-submanifold](https://alphabetamath.cc/item/prop-integration-over-an-oriented-embedded-submanifold) supplies their integrals and invariance under orientation-preserving reparametrization. Thus both displayed fluxes are well-defined real numbers. With $g$, $o$ and $F$ fixed, reversing the chosen orientation of $S$ leaves both pulled-back forms unchanged and negates each integral by [math:prop-reversing-orientation-negates-the-integral](https://alphabetamath.cc/item/prop-reversing-orientation-negates-the-integral), applied to these compactly supported top forms. Thus both flux signs reverse. The choice assumption includes the countable choice carried by the Lorentzian and Hodge suppliers.


## Weighted exterior elliptic domains and admissible weights

[Open item](item-def-exterior-weighted-elliptic-data) · level 0


### Definition

A smooth three-dimensional exterior here is a smooth three-manifold $\Sigma$ with compact smooth boundary $S=\partial\Sigma$, a compact subset whose complement is diffeomorphic to $\{x\in\mathbb R^3:|x|>r_0\}$ for some $r_0>0$, and a fixed such end chart $x$. Put $r=|x|$ on the end and $K=\Sigma\setminus\{r>2r_0\}$, and require $K$ to be compact as part of the exterior data. Equip $\Sigma$ with a smooth Riemannian metric $h$, meaning a smooth positive-definite symmetric covariant two-tensor.

Fix finitely many smooth interior or boundary charts and compact chart subsets $K_i$ covering $K$, each contained in its chart domain. Boundary charts take values in a half-space. For a scalar function $u$ of class $C^{k,\alpha}$ up to the boundary on compact sets, let $N_K(u)$ be the sum, over these fixed subsets, of the suprema of all coordinate derivatives of orders at most $k$ and the $\alpha$-Hölder seminorms of those of order $k$, taken over pairs of distinct points in the corresponding chart images of $K_i$. Here $[v]_{\alpha;E}=\sup_{x\ne y\in E}|v(x)-v(y)|/|x-y|^\alpha$, with an empty supremum interpreted as zero.

For an integer $k\ge0$, $0<\alpha<1$ and $\beta\in\mathbb R$, put $A_R=\{R<r<2R\}$ for $R\ge r_0$ and define

$$\|u\|_{C^{k,\alpha}_\beta}=N_K(u)+\sup_{R\ge r_0}R^{-\beta}\left(\sum_{j=0}^k R^j\max_{|I|=j}\sup_{A_R}|\partial_x^Iu|+R^{k+\alpha}\max_{|I|=k}[\partial_x^Iu]_{\alpha;A_R}\right).$$

The weighted Hölder space $C^{k,\alpha}_\beta$ consists of the real-valued functions just described for which this quantity is finite. The multi-index $I$ specifies repeated coordinate derivatives, and $|I|$ is their total order. Thus the convention is that $u$ has order at most $r^\beta$, with corresponding derivative and Hölder weights. Define the Dirichlet domain $X_\beta=\{u\in C^{4,\alpha}_\beta:u|_S=0\}$ and the target $Y_\beta=C^{2,\alpha}_{\beta-2}$. The restriction to $S$ is the continuous boundary value.

Write $\Delta_h$ for the Laplace–Beltrami operator with convention $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$, and for a real function $V$ write $\Delta_h-V$ for $u\mapsto\Delta_hu-Vu$. Its zeroth-order coefficient is $-V$, hence is nonpositive when $V\ge0$. The interval $-1<\beta<0$ is the weight range used in the separate exterior Dirichlet results; this definition asserts no Fredholm, index, invertibility, or completeness theorem and does not assert that this interval is the only possible one.

### Definition references

[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)

[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

### Justification

The compactness requirement on $K$ permits the finite compact chart cover: smaller coordinate balls or boundary half-balls with compact closures inside their chart domains give an open cover of $K$, from which a finite subcover is selected. The local Hölder and boundary-extension conventions give the displayed derivatives and continuous boundary values. The chosen chart subsets cover $K$, while the annuli cover the end beyond $r_0$; consequently the displayed quantity vanishes only for the zero function. Homogeneity and the triangle inequality follow term by term from those of absolute values and Hölder seminorms, so the finite-valued class is a normed vector space. The specified chart and compact-core choices are part of this definition; no equivalence under a change of choices is asserted here. The sign statement follows directly from the definition of multiplication by $V$.

### Source notes

The declared Hölder supplier provides the scaled-norm and boundary-extension conventions. Schikorra, Section 8, opening definitions on printed p. 139, was consulted for the ordinary Euclidean Hölder seminorm and the $C^{k,\alpha}$ convention only. The compact-core and weighted annular assembly is specified here.


## Normal graphs and the nonlinear mean-curvature map

[Open item](item-def-normal-graph-and-mean-curvature-data) · level 0


### Definition

Assume the Axiom of Countable Choice $\mathrm{AC}_\omega$ for the inherited tangent-bundle smooth structures used below.

Let $(M,g,N)$ be a time-oriented smooth Lorentzian four-manifold of signature $(-,+,+,+)$, with metric-selected connection $\nabla$, and let $\Sigma\subset M$ be a smooth embedded spacelike hypersurface. Thus $g$ restricts to a positive definite metric on each tangent space of $\Sigma$. Write $n$ for its future-directed unit normal: $g(n,n)=-1$, $g(n,N)<0$, and $g(n,V)=0$ for every $V\in T\Sigma$.

Let $Y$ be a smooth vector field on an open neighborhood $U$ of $\Sigma$, transverse to $\Sigma$, meaning $Y_x\notin T_x\Sigma$ at each $x\in\Sigma$. Let $\phi^Y$ be a local flow of $Y$, with open domain $\mathcal D\subseteq\mathbb R\times U$. For a smooth real function $w$ on $\Sigma$ with $(w(x),x)\in\mathcal D$ for all $x$, put $F_w(x)=\phi^Y(w(x),x)$. When $F_w$ is an embedding and its image $\Sigma_w$ is spacelike, $F_w$ and $\Sigma_w$ are called the flow graph map and flow graph of $w$.

For the normal exponential construction, take a smooth real function $w$ such that $w(x)n_x$ belongs to the exponential map domain at every $x$. Put $E_w(x)=\exp_x(w(x)n_x)$. When $E_w$ is an embedding with spacelike image, it and its image are the normal exponential graph map and normal exponential graph. In a specified normal tubular neighborhood this construction may be restricted to those $w$ for which $(x,w(x))$ lies in the chosen domain of a diffeomorphism $(x,s)\mapsto\exp_x(sn_x)$ onto that neighborhood; the existence of such a neighborhood is not asserted here.

For either admissible graph map $G_w$ above, let $n_w$ be the future unit normal to its image, $h_w$ the metric induced there by $g$, and $K_w(V,W)=g(\nabla_Vn_w,W)$ for tangent vectors. At each image point, let $S_w$ be the shape operator determined by $h_w(S_wV,W)=K_w(V,W)$; write $\operatorname{tr}_{h_w}K_w:=\operatorname{tr}(S_w)$, the basis-independent trace of this tangent-space endomorphism. The mean-curvature map assigns to $w$ the function $\mathcal H(w)=G_w^*(\operatorname{tr}_{h_w}K_w)$ on $\Sigma$. Equivalently, with any local unit timelike extension of $n_w$, this is the pullback of $\operatorname{div}_g n_w$. A graph is maximal when $\mathcal H(w)=0$.

If $S\subseteq\Sigma$ is a prescribed boundary set, the homogeneous Dirichlet condition is $w|_S=0$. It fixes each point of $S$ under either graph map. Boundary regularity, spacelikeness and embedding of a candidate graph, differentiability of $\mathcal H$ between Banach spaces, and representation of other hypersurfaces as such graphs require separate hypotheses.

### Definition references

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:lem-gr-metric-divergence-and-density-formula](https://alphabetamath.cc/physics/item/lem-gr-metric-divergence-and-density-formula)

[math:def-trace-of-an-endomorphism](https://alphabetamath.cc/item/def-trace-of-an-endomorphism)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

[math:prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

### Facts & Assumptions

[F1] A spacelike embedded hypersurface has positive definite induced metric. [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[F2] Its future unit normal is unique and smooth, and its tangential covariant derivative is independent of the chosen local extension. [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[F3] The metric-selected connection is metric-compatible. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F4] The local flow is defined on an open domain and is the identity at time zero. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F5] The exponential map is defined on its stated open domain and maps the zero vector at $x$ to $x$. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F6] For a smooth local vector field $J$, the ambient divergence is the scalar contraction $\operatorname{div}_gJ=\nabla_aJ^a=g^{ab}\nabla_bJ_a$. [physics:lem-gr-metric-divergence-and-density-formula](https://alphabetamath.cc/physics/item/lem-gr-metric-divergence-and-density-formula)

[F7] The trace of a finite-dimensional endomorphism is the sum of the diagonal entries in any basis and is independent of that basis. [math:def-trace-of-an-endomorphism](https://alphabetamath.cc/item/def-trace-of-an-endomorphism)

[F8] The tangent-bundle smooth structures used by the Lorentzian data, connection and exponential-map suppliers carry the inherited assumption $\mathrm{AC}_\omega$. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection) [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

### Justification

The local flow and exponential map give smooth graph maps on their stated domains. The inherited $\mathrm{AC}_\omega$ convention supplies the tangent-bundle smooth structures, including the one used for smooth dependence on the initial vector in the exponential construction. Embedding and spacelikeness are explicit admissibility conditions, so each image is a spacelike embedded hypersurface. [math:prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold) Its unique smooth future normal and extension-independent tangential derivatives give the smooth tensor $K_w$ and its trace; pulling this scalar back by $G_w$ defines $\mathcal H(w)$. In an $h_w$-orthonormal tangent basis, the defining relation for $S_w$ gives $\operatorname{tr}(S_w)=\sum_{i=1}^3h_w(S_we_i,e_i)=\sum_{i=1}^3K_w(e_i,e_i)$; basis independence follows from the endomorphism trace. For a local unit timelike extension of $n_w$, metric compatibility gives $g(\nabla_{n_w}n_w,n_w)=\tfrac12 n_w(g(n_w,n_w))=0$. The divergence contraction formula in a local orthonormal frame consisting of $n_w$ and three tangent unit vectors $e_1,e_2,e_3$ gives $\operatorname{div}_g n_w=-g(\nabla_{n_w}n_w,n_w)+\sum_{i=1}^3g(\nabla_{e_i}n_w,e_i)=\operatorname{tr}_{h_w}K_w$, independent of that unit extension. Finally, the flow and exponential identities at zero imply that $w|_S=0$ fixes $S$ pointwise.

### External input

The declared library normal lemma supplies the unique smooth future unit normal and extension-independent tangential covariant derivative for a spacelike embedded hypersurface. [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

Gourgoulhon's cited equations record the normal and curvature conventions. His extrinsic curvature has the opposite sign from $K_w$ here; his trace-divergence identity agrees after that sign conversion. The local justification above uses the declared mathematical suppliers.


## Periodic isometries and invariant normal averaging

[Open item](item-def-circle-action-and-invariant-normal-data) · level 0


### Definition

Work in ZFC. Let $(M,g,N)$ be a time-oriented smooth Lorentzian four-manifold of signature $(-,+,+,+)$: $N$ is a smooth timelike field, and a timelike vector $v$ is future-directed when $g(v,N)<0$. A **normalized circle action by isometries** is a smooth global flow $\phi:\mathbb R\times M\to M$ of a smooth vector field $Z$, with $\phi_{s+2\pi}=\phi_s$ for all $s$, such that $2\pi$ is the least positive common period and $\phi_s^*g=g$ for every $s$. The **generator** is $Z_p=\left.\frac{d}{ds}\right|_{s=0}\phi_s(p)$. A **fixed point** is a point $p$ for which $\phi_s(p)=p$ for every $s$; consequently $Z_p=0$. The least-period condition concerns the whole action, so individual orbits may have shorter periods or be fixed.

Let $S\subseteq M$ be an embedded submanifold invariant under the action, meaning $\phi_s(S)=S$ for all $s$. A **smooth field along $S$** is an assignment $p\mapsto n_p\in T_pM$ such that, in every ambient slice chart $(U,x)$ with $S\cap U$ given by $x^{k+1}=\cdots=x^4=0$, the coefficients in $n_p=\sum_{a=1}^4 n^a(p)\partial_{x^a}|_p$ are smooth functions of the slice variables $(x^1,\ldots,x^k)$. Such a field is **normal** when $g_p(n_p,v)=0$ for every $p\in S$ and $v\in T_pS$. Suppose $n$ is future timelike at every point. Define its **circle average** and **normalized invariant normal** by

$$\bar n_p=\frac1{2\pi}\int_0^{2\pi}d\phi_s|_{\phi_{-s}(p)}\bigl(n_{\phi_{-s}(p)}\bigr)\,ds,\qquad \widehat n_p=\frac{\bar n_p}{\sqrt{-g_p(\bar n_p,\bar n_p)}}.$$

Here $d\phi_s|_q:T_qM\to T_{\phi_s(q)}M$ is the differential. The isometry condition uses tensor pullback: $(\phi_s^*g)_q(u,v)=g_{\phi_s(q)}(d\phi_s|_q u,d\phi_s|_q v)$. The integral is taken in the fixed finite-dimensional vector space $T_pM$: for a continuous curve $v(s)=\sum_{a=1}^4v^a(s)e_a$ in any fixed basis, set $\int_0^{2\pi}v(s)\,ds=\sum_{a=1}^4(\int_0^{2\pi}v^a(s)\,ds)e_a$, using scalar Riemann integrals. An invariant field along $S$ is one satisfying $d\phi_t|_p(v_p)=v_{\phi_t(p)}$ for all $p\in S$ and $t\in\mathbb R$. The construction assumes the supplied field $n$; it asserts no existence of such a field.

### Definition references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

[math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map)

[math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

[math:thm-continuous-implies-integrable](https://alphabetamath.cc/item/thm-continuous-implies-integrable)

### Justification

Every continuous scalar component on a closed finite interval is bounded and Riemann integrable. The tagged-sum characterization identifies the coordinatewise vector integral with the limit of the vector sums $\sum_i v(\xi_i)\Delta_i$ as the mesh tends to zero. A fixed linear map commutes with this limit: its matrix acts by finite sums of constant multiples of convergent scalar components. Applying this to a change-of-basis matrix proves that the integral is independent of the chosen basis; applying it to any linear functional or differential proves commutation with that map. Scalar order inequalities pass to the limit from the positive-weight sums. Likewise, the finite-sum triangle inequality gives $|\int w(s)\,ds|\le\int|w(s)|\,ds$ for a continuous Euclidean-vector-valued $w$. All these scalar integrands are continuous, so their integrability is supplied. These sum arguments also give $|\int h|\le(b-a)\sup|h|$ on $[a,b]$. Translating tagged partitions proves invariance under translation of the integration variable, and joining tagged partitions at a split point proves additivity across that point; the componentwise construction carries both properties to vector integrals. [math:thm-continuous-implies-integrable](https://alphabetamath.cc/item/thm-continuous-implies-integrable) [math:thm-darboux-equals-riemann](https://alphabetamath.cc/item/thm-darboux-equals-riemann) [math:cor-triangle-inequality-for-inner-product-norm](https://alphabetamath.cc/item/cor-triangle-inequality-for-inner-product-norm)

The coordinate formula for the differential shows that the slice-coordinate definition of smoothness is unchanged on overlaps: the new components are the old components multiplied by the smooth Jacobian matrix of the chart transition. It also shows that $v(s,p):=d\phi_s|_{\phi_{-s}(p)}n_{\phi_{-s}(p)}$ has smooth components jointly in $(s,p)$. This is local near each $(s,p)$; the moving source point may use different charts for different $s$, while the output is expressed in one chart around $p$. The flow law and differential chain rule make each $\phi_s$ a diffeomorphism with inverse $\phi_{-s}$, and its restriction to $S$ maps tangent spaces onto tangent spaces. For $q=\phi_{-s}(p)$ and $X\in T_pS$, the pullback formula gives $g_p(v(s,p),X)=g_q(n_q,d\phi_{-s}|_pX)=0$. The integrand at $s=0$ is $n_p$. As $s$ varies continuously, $v(s,p)$ is timelike by isometry and remains in the same timelike component as $n_p$, hence in the future cone. Commutation with the linear functional $g_p(\cdot,X)$ makes $\bar n_p$ normal. [math:thm-coordinate-formula-for-the-differential](https://alphabetamath.cc/item/thm-coordinate-formula-for-the-differential) [math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map) [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps) [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart) [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

In a future-oriented orthonormal basis at $p$, write $v(s,p)=(a(s),b(s))$ with $b(s)\in\mathbb R^3$. The future-cone description gives $a(s)>|b(s)|$. The continuous positive function $a(s)-|b(s)|$ attains a positive minimum $\delta_p$ on $[0,2\pi]$. The integral order and norm inequalities just established give $(2\pi)^{-1}\int a\ge(2\pi)^{-1}\int|b|+\delta_p\ge|(2\pi)^{-1}\int b|+\delta_p$. Hence $\bar n_p$ is future timelike, the positive square root in the normalization exists, and $g(\widehat n,\widehat n)=-1$. No uniform lower bound in $p$ is required. [physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components) [math:lem-extreme-value-theorem-from-compactness](https://alphabetamath.cc/item/lem-extreme-value-theorem-from-compactness) [math:thm-darboux-equals-riemann](https://alphabetamath.cc/item/thm-darboux-equals-riemann) [math:cor-triangle-inequality-for-inner-product-norm](https://alphabetamath.cc/item/cor-triangle-inequality-for-inner-product-norm)

On a compact coordinate rectangle in $S$, repeated differentiation under the integral sign, one slice variable at a time, shows that every partial derivative of the components of $\bar n$ is the integral of the corresponding derivative of $v(s,p)$. The derivatives of the integrand are continuous, hence uniformly continuous, on the rectangle times $[0,2\pi]$, and their integrals are continuous: a uniform change of at most $\varepsilon$ in a component changes its integral by at most $2\pi\varepsilon$, by the sum bound above. Thus $\bar n$ is smooth. Since $-g(\bar n,\bar n)$ is a smooth positive function, its positive square root and the normalized field are smooth as well. [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle) [math:thm-heine-cantor-metric](https://alphabetamath.cc/item/thm-heine-cantor-metric) [math:thm-coordinate-formula-for-the-differential](https://alphabetamath.cc/item/thm-coordinate-formula-for-the-differential) [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

For $p'=\phi_t(p)$, commutation of a fixed differential with integration and the flow chain rule give $d\phi_t|_p\bar n_p=(2\pi)^{-1}\int_0^{2\pi}v(s+t,p')\,ds$. To see that a full-period integral is independent of its starting point, reduce $t$ modulo $2\pi$ to $r\in[0,2\pi)$, split the interval $[r,r+2\pi]$ at $2\pi$, and translate its second piece by $-2\pi$; periodicity identifies that piece with $[0,r]$. The integral therefore equals $\bar n_{p'}$. Isometry preserves the normalization factor, so $\widehat n$ is invariant too. [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:thm-darboux-equals-riemann](https://alphabetamath.cc/item/thm-darboux-equals-riemann) [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

The ZFC convention includes the choice assumptions inherited from the stated manifold interface. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Fredholm and Banach continuation interfaces

[Open item](item-def-fredholm-continuation-data) · level 0


### Definition

Assume the Axiom of Choice. Let $X,Y$ be real Banach spaces: real normed vector spaces complete for their norm metrics. A bounded linear map $L:X\to Y$ is **Fredholm** if its kernel is finite dimensional, its range is closed, and its cokernel $Y/\operatorname{ran}L$ is finite dimensional. Its **index** is $\operatorname{ind}L=\dim\ker L-\dim(Y/\operatorname{ran}L)$.

Equip $\mathbb R\times X$ with the maximum product norm $\|(q,w)\|_{\max}=\max\{|q|,\|w\|_X\}$, for which it is a real Banach space. A **local continuation problem** consists of an open set $U\subseteq\mathbb R\times X$ for this norm and a $C^1$ map $\mathcal H:U\to Y$. Here $C^1$ means Fréchet differentiable with derivative continuous in operator norm. A **zero** is $(q,w)\in U$ with $\mathcal H(q,w)=0$. At such a point the partial derivative $D_w\mathcal H(q,w):X\to Y$ is $D\mathcal H(q,w)$ restricted to vectors of the form $(0,v)$. A **bounded isomorphism** is a bounded linear bijection with bounded linear inverse.

If $D_w\mathcal H(q_0,w_0)$ is a bounded isomorphism at a zero, the implicit-function theorem provides open neighborhoods $A$ of $q_0$ and $B$ of $w_0$ and a unique $C^1$ map $w:A\to B$ whose graph is exactly the zero set of $\mathcal H$ in $A\times B$. This criterion requires invertibility; Fredholm index zero alone does not supply it.

For an endpoint $q_*$, a branch $w(q)$ of zeros can be continued to a zero at $q_*$ by a limit argument when a sequence $q_n\to q_*$ has $w(q_n)\to w_*$ in $X$, $(q_*,w_*)\in U$, and any additional admissibility or graph conditions required by the particular problem hold at the limit. A set of branch values is **relatively compact** when its closure in $X$ is compact for the norm metric. Relative compactness of the branch values can supply a convergent subsequence; it does not by itself ensure that the limit remains in $U$ or satisfies those additional conditions.

If $L$ is Fredholm and $K:X\to Y$ is a compact linear operator, meaning that it maps bounded sets to relatively compact sets, then $L+K$ is Fredholm with the same index. This statement alone does not identify the kernel of $L+K$.

### Justification

The Fredholm terminology and index are those of [math:def-fredholm-operator-cokernel-and-index](https://alphabetamath.cc/item/def-fredholm-operator-cokernel-and-index), and the differentiability convention is that of [math:def-c-k-map-between-banach-spaces](https://alphabetamath.cc/item/def-c-k-map-between-banach-spaces). By [math:thm-reals-cauchy-complete](https://alphabetamath.cc/item/thm-reals-cauchy-complete), every Cauchy sequence of real numbers for the absolute-value metric converges to a real number. Consequently $\mathbb R$ with its absolute-value norm is Banach by [math:def-banach-space](https://alphabetamath.cc/item/def-banach-space). The chosen norm is the maximum product norm of [math:def-product-norms-on-finitely-many-normed-spaces](https://alphabetamath.cc/item/def-product-norms-on-finitely-many-normed-spaces). Since $\mathbb R$ with its absolute-value norm and $X$ are Banach, [math:thm-finite-products-of-banach-spaces-are-banach](https://alphabetamath.cc/item/thm-finite-products-of-banach-spaces-are-banach) makes $\mathbb R\times X$ Banach. The product parameter space and the partial derivative fit the hypotheses of [math:thm-implicit-function-theorem-for-banach-spaces](https://alphabetamath.cc/item/thm-implicit-function-theorem-for-banach-spaces), with parameter space $\mathbb R$, unknown space $X$, and target $Y$; the stated graph conclusion follows under its bounded-isomorphism hypothesis and Choice. Index zero is insufficient for invertibility: the zero map $\mathbb R\to\mathbb R$ has one-dimensional kernel and cokernel, hence index zero, but is not injective. For the endpoint assertion, the differentiability-implies-continuity argument in the Remarks of [math:def-frechet-derivative-between-banach-spaces](https://alphabetamath.cc/item/def-frechet-derivative-between-banach-spaces) applies to the $C^1$ map $\mathcal H$ on the open subset $U$ of the real Banach space $\mathbb R\times X$, so $\mathcal H$ is continuous on $U$. Give $U$ the restricted maximum-norm metric and $Y$ its norm metric. These are metric spaces, so the choice-free implication (a) to (d) of [math:thm-metric-continuity-characterisations](https://alphabetamath.cc/item/thm-metric-continuity-characterisations) makes $\mathcal H:U\to Y$ sequentially continuous. The assumed component limits give $\|(q_n,w(q_n))-(q_*,w_*)\|_{\max}=\max\{|q_n-q_*|,\|w(q_n)-w_*\|_X\}\to0$: for each positive tolerance, both terms are smaller than it once $n$ exceeds their two thresholds. Since the sequence consists of zeros and $(q_*,w_*)\in U$, sequential continuity yields $\mathcal H(q_*,w_*)=\lim_n\mathcal H(q_n,w(q_n))=0$; preservation of any extra conditions must be checked separately. If the branch values have compact closure $C\subseteq X$, [math:thm-compact-implies-the-other-compactness-forms](https://alphabetamath.cc/item/thm-compact-implies-the-other-compactness-forms), assertions 1 and 3, applies to $C$ with its restricted norm metric: compactness implies countable compactness and then sequential compactness. Thus the sequence of branch values has a subsequence converging to a point of $C\subseteq X$. This extraction alone says nothing about membership of the associated limit pair in $U$ or preservation of additional admissibility conditions. The compact-perturbation assertion is exactly [math:thm-fredholm-index-is-stable-under-compact-perturbations](https://alphabetamath.cc/item/thm-fredholm-index-is-stable-under-compact-perturbations) under its stated hypotheses.


## Measurable domains on smooth initial surfaces

[Open item](item-def-author-0336834a2590-measurable-surface-domains) · level 0


### Definition

Work in ZFC. Let $(C,h)$ be a smooth Hausdorff second-countable Riemannian surface. A measurable surface domain is a Borel subset $A\in\mathcal B(C)$, where $\mathcal B(C)$ is generated by the manifold-open sets; no openness, smooth boundary or Lipschitz boundary is required. Let $v_h$ be the intrinsic Borel measure of the Riemannian density $\sqrt{\det(h_{ab})}\,|dx^1dx^2|$. Its completion is denoted $\mu_C$: its domain consists of $B\cup N$ with $B,Z\in\mathcal B(C)$, $v_h(Z)=0$ and $N\subseteq Z$, and $\mu_C(B\cup N)=v_h(B)$. For a measurable surface domain write $|A|=\mu_C(A)$. A closed subset of $C$ is an admissible Borel domain; it need not itself be a surface.

For $(X,g)=(C,h)$ or a smooth Hausdorff second-countable Riemannian three-manifold $(\Sigma,k)$, work separately on each connected component $X_j$. Give $X_j$ the finite Riemannian distance $d_{g,j}(p,q)=\inf_\gamma L_g(\gamma)$ over piecewise $C^1$ curves in $X_j$ joining $p$ to $q$. There are at most countably many components. Set $c_2=\mathcal H^2_{\mathrm{unnorm},\mathbb R^2}((0,1]^2)>0$, using the unnormalised diameter-cover construction, and for every $E\subseteq X$ define $\mathcal H_g^2(E)=c_2^{-1}\sum_j\mathcal H^2_{\mathrm{unnorm},(X_j,d_{g,j})}(E\cap X_j)$. This is an outer value on arbitrary sets; as a measure we use the complete componentwise Carathéodory domain, which includes all Borel sets. Thus for $D\subseteq\Sigma$ write $|D|=\mathcal H_k^2(D)$. The normalization equals ordinary Euclidean area on planes.

On $C$, $\mathcal H_h^2(A)=\mu_C(A)$ for Borel $A$ and for every set in the completed area domain. If $S\subseteq\Sigma$ is a smooth embedded surface with induced tensor $h_S=k|_{TS}$, then $\mathcal H_k^2(E)=\mu_S(E)=\mathcal H_{h_S}^2(E)$ for Borel $E\subseteq S$ and their area-completed sets. Here the first Hausdorff value uses the ambient component distance of $\Sigma$, whereas the last uses the intrinsic component distances of $S$. No equality of these distances is asserted.

A subset $E\subseteq X$, with $X$ and $g$ as above, is countably two-rectifiable if there are a set $N\subseteq E$ with $\mathcal H_g^2(N)=0$ and countably many maps $f_m:B_m\subseteq\mathbb R^2\to X_{j(m)}$ such that $E\setminus N\subseteq\bigcup_m f_m(B_m)$. Each $f_m$ is Lipschitz from Euclidean distance on $B_m$ to the specified finite distance $d_{g,j(m)}$ on its target component. No measurable-domain or boundary-regularity requirement is imposed on the parameter subsets $B_m$.

### Facts & Assumptions

**Given:** The surfaces, ambient manifolds, component distances and normalization in the Definition. The local argument establishes well-definedness and the asserted area agreements.

[A1] ZFC includes AC; countable choice is available for the chart, cover and completion constructions below. Only this countable-choice consequence is used. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Riemannian tensors are smooth and positive definite on Hausdorff second-countable manifolds; Borel sets form the sigma-algebra generated by the manifold topology. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra)

[F2] The Riemannian density is coordinate independent. Countable chart-partition gluing gives its intrinsic Borel measure $v_h$, with chart restriction $v_h(E)=\int_{x(E)}\sqrt{\det(h_{ab})}\,d\lambda_2$; it is locally finite and Radon. These statements assume countable choice and require no orientation. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:lem-the-riemannian-volume-density-is-coordinate-independent](https://alphabetamath.cc/item/lem-the-riemannian-volume-density-is-coordinate-independent) [math:def-countable-chart-gluing-of-a-nonnegative-density-measure](https://alphabetamath.cc/item/def-countable-chart-gluing-of-a-nonnegative-density-measure) [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing) [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density)

[F3] Under countable choice, the completion construction has a representation-independent value and is the unique complete measure extending the original measure on the displayed completion domain. [math:def-completion-of-a-measure-space](https://alphabetamath.cc/item/def-completion-of-a-measure-space) [math:thm-completion-of-a-measure-space](https://alphabetamath.cc/item/thm-completion-of-a-measure-space)

[F4] On a connected Riemannian manifold the infimum of piecewise smooth curve lengths is a finite metric, and its topology equals the manifold topology. These suppliers are applied only to individual connected components. [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold) [math:thm-riemannian-distance-is-a-metric](https://alphabetamath.cc/item/thm-riemannian-distance-is-a-metric) [math:thm-the-riemannian-distance-topology-is-the-manifold-topology](https://alphabetamath.cc/item/thm-the-riemannian-distance-topology-is-the-manifold-topology)

[F5] Under countable choice, diameter-cover Hausdorff measure is a metric outer measure, is a complete measure on its Carathéodory domain, and measures every Borel set. In Euclidean dimension two its unnormalised value is $c_2\lambda_2^*$ on every subset, with $1\le c_2\le2$. [math:def-hausdorff-measure](https://alphabetamath.cc/item/def-hausdorff-measure) [math:thm-hausdorff-n-measure-is-proportional-to-lebesgue-measure](https://alphabetamath.cc/item/thm-hausdorff-n-measure-is-proportional-to-lebesgue-measure) [math:thm-hausdorff-measure-is-metric-and-borel-measurable](https://alphabetamath.cc/item/thm-hausdorff-measure-is-metric-and-borel-measurable)

[F6] Lipschitz means $d_Y(f(x),f(y))\le Ld_X(x,y)$ for all source points and a finite constant $L\ge0$. Under countable choice, for $L>0$ an $L$-Lipschitz map satisfies $\mathcal H^2(f(E))\le L^2\mathcal H^2(E)$; multiplying both Hausdorff conventions by $c_2^{-1}$ preserves the inequality. For $L=0$, the image $f(E)$ is empty or a singleton and has two-dimensional Hausdorff measure zero; no product $0\cdot\infty$ is used. [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction) [math:thm-hausdorff-measure-under-lipschitz-maps](https://alphabetamath.cc/item/thm-hausdorff-measure-under-lipschitz-maps)

[F7] An embedded surface has slice charts in which it is a coordinate plane. Riemannian coordinate matrices are smooth positive definite matrices and transform by $G_y=J^TG_xJ$. Finite Gram–Schmidt preserves successive spans, so an adapted coordinate basis can be orthonormalized while its first two vectors remain tangent to the slice. The real spectral theorem diagonalizes the symmetric two-dimensional surface matrix orthogonally, so the quadratic-form bounds control each eigenvalue and their product is the determinant. [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart) [math:prop-coordinate-criterion-for-a-riemannian-metric](https://alphabetamath.cc/item/prop-coordinate-criterion-for-a-riemannian-metric) [math:thm-gram-schmidt-orthonormalisation](https://alphabetamath.cc/item/thm-gram-schmidt-orthonormalisation) [math:cor-real-spectral-theorem-for-self-adjoint-endomorphisms](https://alphabetamath.cc/item/cor-real-spectral-theorem-for-self-adjoint-endomorphisms)

[F8] Curve length is the integral of metric speed. On every piecewise $C^1$ coordinate curve, Newton–Leibniz applied to a constant unit vector field and the line-integral bound give $\int|\dot x(t)|\,dt\ge|x(b)-x(a)|$. [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length) [math:thm-newton-leibniz-with-interior-derivative](https://alphabetamath.cc/item/thm-newton-leibniz-with-interior-derivative) [math:thm-scalar-and-vector-line-integral-estimates](https://alphabetamath.cc/item/thm-scalar-and-vector-line-integral-estimates)

[F9] Under countable choice every second-countable space has a countable subcover of any open cover. [math:thm-second-countable-implies-lindelof](https://alphabetamath.cc/item/thm-second-countable-implies-lindelof)

### Justification

**Given:** The objects and hypotheses in the Definition, with the suppliers recorded above.

1.1 Every component of a manifold is open: connected coordinate balls about each of its points remain in that component. A countable base assigns to each component its least-indexed contained basis member, so there are at most countably many components. Apply the connected-distance suppliers on each component, with precisely their connectedness hypothesis. A set is Borel on the whole manifold exactly when its restrictions to the components are Borel, since these components are a countable open partition with the distance topology. [F1, F4, given]

1.2 Fix $0<\varepsilon<1$ and a point in a Riemannian surface. Alternatively fix a point of an embedded surface $S\subseteq\Sigma$ and use an ambient slice chart. In either case choose linear coordinates centered at the point so that the metric matrix at the center is the identity; in the slice case choose the first two orthonormal coordinate vectors tangent to $S$, preserving its coordinate plane. Smoothness of the matrix entries gives a coordinate ball $B_R$ with closure in the chart on which $(1-\varepsilon)^2|v|^2\le g_x(v,v)\le(1+\varepsilon)^2|v|^2$. Explicitly, it suffices that every entry of $G_x-I$ has absolute value at most $(2\varepsilon-\varepsilon^2)/n$, since $|v^T(G_x-I)v|\le n\max_{a,b}|(G_x-I)_{ab}|\,|v|^2$; continuity gives that bound on a sufficiently small closed ball. Here $n=2$ intrinsically and $n=3$ in the ambient slice calculation. [F1, F7, given, algebra]

2.1 The positive smooth Riemannian density glues independently of charts and gives $v_h$ with the displayed coordinate formula. The stated completion construction therefore defines $\mu_C$ on exactly its specified domain. Closed sets are Borel because their complements are open. Apply the Hausdorff suppliers componentwise: multiplication by $c_2^{-1}$ and countable summation preserve outer subadditivity, Borel additivity and completeness on the componentwise measurable domain. The Euclidean normalization theorem gives normalized value $\lambda_2^*$ on $\mathbb R^2$, and hence area on any Euclidean plane, since isometries preserve the diameter-cover costs in both directions. No curved-surface identity is inferred from normalization alone. [A1, F1, F2, F3, F5, step 1.1]

2.2 Choose $0<r<R/3$. For points with coordinates $x,y\in B_r$, the straight segment stays in $B_R$ and has metric length at most $(1+\varepsilon)|x-y|$. Every joining curve staying in $B_R$ has length at least $(1-\varepsilon)|x-y|$. If a joining curve leaves $B_R$, its initial segment to the first exit has coordinate displacement at least $R-r>2r\ge|x-y|$, so its length has the same lower bound. This uses continuity for the first exit, the metric-speed bounds and the coordinate displacement integral estimate; it applies to every piecewise $C^1$ joining curve, without existence of a minimizer. Taking the infimum gives $(1-\varepsilon)|x-y|\le d_g(x,y)\le(1+\varepsilon)|x-y|$. In a slice chart restrict $x,y$ to the surface coordinate plane: its straight segment lies in $S$, while the lower estimate already holds for all ambient joining curves. Thus the restricted ambient distance has these same bounds, even when curves outside $S$ are shorter than intrinsic curves. [F4, F7, F8, step 1.2]

3.1 Let $U$ be the small surface patch in step 2.2 and let $B\subseteq U$ be Borel in the surface. Denote its two-dimensional coordinate image by $x(B)$. Applying Lipschitz control in both directions to the distance bounds gives $(1-\varepsilon)^2\lambda_2(x(B))\le H(B)\le(1+\varepsilon)^2\lambda_2(x(B))$, where $H$ denotes either intrinsic normalized Hausdorff area or the ambient normalized Hausdorff value in the slice case. The two eigenvalues of the induced surface matrix lie between $(1-\varepsilon)^2$ and $(1+\varepsilon)^2$, so its area density lies between those same bounds. The chart-restriction formula for $v_h$ consequently gives $a_\varepsilon v_h(B)\le H(B)\le a_\varepsilon^{-1}v_h(B)$, with $a_\varepsilon=((1-\varepsilon)/(1+\varepsilon))^2$. All constants are positive, so these comparisons also apply to infinite values. [F2, F5, F6, F7, step 1.2, step 2.2, algebra]

4.1 For each fixed $\varepsilon$, second countability supplies a countable cover by these small surface patches. Subtract earlier patches to obtain a disjoint Borel partition. In the embedded case each slice patch is relatively closed in an ambient open coordinate neighborhood, hence ambient Borel; a surface-Borel subset of such a patch is ambient Borel as well. Thus both the intrinsic and ambient Hausdorff restrictions are countably additive on the pieces. Summing step 3.1 proves the same two-sided comparison on every Borel surface set. Let $\varepsilon\downarrow0$ to get equality: for finite area the constants tend to one, and for infinite area the lower bound forces infinite Hausdorff value. Componentwise sums treat disconnected surfaces and ambient manifolds. This proves both Borel identities stated in the Definition. [A1, F1, F2, F5, F7, F9, step 1.1, step 3.1]

5.1 For a set in the area completion, write it as $B\cup N$ with $N$ contained in an area-null Borel set $Z$. Step 4.1 makes $Z$ null for each compared Hausdorff convention, whose complete measure therefore measures $N$ with value zero. Its value on $B\cup N$ is the area-completed value $v_h(B)$. The rectifiability definition uses precisely these outer-null sets and the finite component metrics; it asserts no parametrization theorem. All original area conventions, closed-domain admissibility and the absence of boundary regularity requirements are retained. [F3, F5, F6, step 2.1, step 4.1] ∎

### Source notes

The constant $c_2$ is defined by the unnormalised diameter-cover construction, not by a numerical identification of that constant. The Euclidean normalization is supplied by the Euclidean Hausdorff theorem; the curved and ambient surface agreement is the local argument above. No endpoint area formula or article claim is used to justify this prerequisite.


## Transverse hitting maps have local differentiable extensions

[Open item](item-lem-author-0336834a2590-transverse-endpoint-regularity) · level 0


### Statement

Work in ZFC. Let $C$ be a smooth Hausdorff second-countable surface (that is, a two-dimensional smooth manifold) and $M$ a smooth manifold. Let $s:M\to\mathbb R$ be smooth with $0$ a regular value, and give $\Sigma=s^{-1}(0)$ its regular-level embedded smooth structure when nonempty. Let $G:O\to M$ be a supplied $C^1$ family on an open set $O\subset C\times\mathbb R$, with the product smooth structure. Let $A\subset C$ be Borel.

Suppose for each $x\in A$ there is a unique $t_x$ with $(x,t_x)\in O$ and $s(G(x,t_x))=0$, and $\partial_t(s\circ G)(x,t_x)\ne0$. Then $F(x)=G(x,t_x)$ has local $C^1$ extensions from $A$ into $\Sigma$, and a countable cover by such extensions. These extensions can be restricted to smaller source coordinate balls covering $A$ so that each coordinate representative in a target chart of $\Sigma$ is Lipschitz. No regularity of $F(A)$ is assumed.

### Facts & Assumptions

[A1] Work in ZFC, including AC. Only its countable-choice consequence is used: for the countable-subcover theorem and for selecting the extension and chart data attached to the countably many selected neighborhoods. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The Euclidean implicit function theorem applies to a scalar $C^1$ equation on an open subset of $\mathbb R^2\times\mathbb R$ when its time derivative at a zero is nonzero. [math:thm-euclidean-implicit-function-theorem](https://alphabetamath.cc/item/thm-euclidean-implicit-function-theorem)

[F2] The Borel subsets of a topological space form the sigma-algebra generated by its open sets. Applied to the manifold topology of $C$, this defines the Borel hypothesis on $A$ without a Riemannian metric or any openness or boundary regularity of $A$. [math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra)

[F3] Smooth manifolds have smooth coordinate charts; $C\times\mathbb R$ has its product smooth structure, and $C^1$ regularity between manifolds is tested by coordinate representatives. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure) [math:def-c-r-and-smooth-maps-between-smooth-manifolds](https://alphabetamath.cc/item/def-c-r-and-smooth-maps-between-smooth-manifolds)

[F4] A regular value has surjective derivative at every point of its fibre. A nonempty regular fibre of a smooth real-valued map is an embedded codimension-one submanifold. Its slice charts, restricted and projected onto the tangential coordinates, supply its smooth atlas and subspace topology. [math:def-regular-and-critical-points-and-values](https://alphabetamath.cc/item/def-regular-and-critical-points-and-values) [math:def-codimension-and-hypersurface](https://alphabetamath.cc/item/def-codimension-and-hypersurface) [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart) [math:thm-a-regular-level-set-is-an-embedded-submanifold](https://alphabetamath.cc/item/thm-a-regular-level-set-is-an-embedded-submanifold) [math:lem-slice-chart-restrictions-form-a-smooth-atlas](https://alphabetamath.cc/item/lem-slice-chart-restrictions-form-a-smooth-atlas)

[F5] Continuous first partial derivatives give total differentiability with the Jacobian derivative. Total derivatives obey the chain rule; for $C^1$ coordinate maps the resulting finite matrix products are continuous, so their compositions are $C^1$. [math:thm-continuous-partial-derivatives-imply-total-differentiability](https://alphabetamath.cc/item/thm-continuous-partial-derivatives-imply-total-differentiability) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F6] Bases trace to subspaces, and an ambient-continuous map with values in a subspace is continuous into that subspace. Second countability means existence of an at most countable basis. Under countable choice every second-countable space is Lindelof. [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top) [math:def-second-countable-space](https://alphabetamath.cc/item/def-second-countable-space) [math:thm-second-countable-implies-lindelof](https://alphabetamath.cc/item/thm-second-countable-implies-lindelof)

[F7] The vector mean-value inequality bounds the endpoint difference on $[0,1]$ by a uniform derivative bound. Lipschitz means a finite constant bounds every output distance by that constant times the input distance. Here coordinate distances are Euclidean. [math:thm-mean-value-inequality](https://alphabetamath.cc/item/thm-mean-value-inequality) [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction)

### Proof

**Given:** The family, unique hits and transversality in the Statement. **Goal:** Produce the stated extensions and countable Lipschitz restrictions.

1.1 If $A=\varnothing$, the empty family of extensions proves every assertion. Otherwise any hit belongs to $\Sigma$, so $\Sigma$ is nonempty and [F4] applies to the given smooth map $s:M\to\mathbb R$ and regular value $0$. Thus $\Sigma$ has the asserted embedded smooth structure; writing $m=\dim M$, its dimension is $k=m-1\ge0$. [given, F4]

1.2 Fix $a\in A$ and a source chart $\phi$ about $a$. The coordinate function $H(z,t)=s(G(\phi^{-1}(z),t))$ is $C^1$ on the open coordinate preimage of $O$, by [F3] and [F5]. It satisfies $H(\phi(a),t_a)=0$ with nonzero scalar time derivative. Apply [F1] with source dimension two and time dimension one. After restricting to a product neighborhood contained in that open preimage, this gives an open neighborhood $U$ of $a$ and a $C^1$ function $\tau:U\to\mathbb R$ with $(x,\tau(x))\in O$ and $s(G(x,\tau(x)))=0$. [given, F1, F3, F5, construct]

2.1 Put $\widetilde F(x)=G(x,\tau(x))$. In source coordinates the graph map $z\mapsto(z,\tau(\phi^{-1}(z)))$ is $C^1$: its derivative is $v\mapsto(v,D(\tau\circ\phi^{-1})(z)v)$ and is continuous. Hence [F5] makes $\widetilde F$ a $C^1$ map into $M$, with image in $\Sigma$. Take a slice chart $\psi$ about $\widetilde F(a)$ and shrink $U$ so its image stays in that chart. In this chart $\psi\circ\widetilde F\circ\phi^{-1}=(f,0)$, where $f$ consists of the first $k$ coordinate components and is $C^1$. The target chart on $\Sigma$ is $\chi=\pi_k\circ\psi|_\Sigma$, so $\chi\circ\widetilde F\circ\phi^{-1}=f$. Continuity into $\Sigma$ follows from its subspace topology and ambient continuity. Thus [F3] proves that $\widetilde F:U\to\Sigma$ is $C^1$, including when $k=0$. [F3, F4, F5, F6, step 1.1, step 1.2, construct]

3.1 For $x\in A\cap U$, the value $\tau(x)$ is a zero in the given fibre $O_x$. Its assumed uniqueness gives $\tau(x)=t_x$, hence $\widetilde F|_{A\cap U}=F$. This proves the local extension assertion. The Borel convention [F2] imposes no additional geometric condition on $A$ and is not needed for this pointwise equality. [given, F2, step 1.2, step 2.1]

3.2 Shrink the source patch about $a$ to a coordinate ball $B$ whose closure lies in $\phi(U)$, retaining the target chart of step 2.1. If $k=0$, its coordinate representative $f$ is constant and is Lipschitz with constant zero. If $k\ge1$, continuity at $\phi(a)$ of the finitely many entries of $Df$ permits a further ball on which all entries have absolute value at most a finite $b\ge1$. Componentwise estimation gives $\|Df(z)v\|_2\le 2kb\|v\|_2$ there. For $u,v\in B$, convexity keeps $u+t(v-u)$ in $B$ for $0\le t\le1$. By [F5], the derivative of $t\mapsto f(u+t(v-u))$ has norm at most $2kb\|v-u\|_2$. Apply [F7] on $[0,1]$ to get $\|f(v)-f(u)\|_2\le2kb\|v-u\|_2$. Thus each such restricted extension is Lipschitz in the specified coordinates. [F5, F7, step 2.1, algebra, construct]

4.1 Take the family of all smaller neighborhoods admitting the extension and chart data from steps 1.2, 2.1, 3.1 and 3.2; no choice indexed by all points of $A$ is necessary to form this family. Their traces on $A$ are an open cover of $A$ in its subspace topology. If $\mathcal B$ is a countable basis of $C$, then $\{B\cap A:B\in\mathcal B\}$ is a countable basis of $A$, by [F6]. Apply the Lindelof theorem in [F6] to $A$, using [A1], to select countably many traces covering $A$. Countable choice also selects extension and chart witnesses for these countably many selected members. By steps 3.1 and 3.2 the witnesses are $C^1$ extensions of $F$ with Lipschitz coordinate representatives on their smaller source neighborhoods. This proves the countable-cover and Lipschitz-piece assertions without any regularity hypothesis on $F(A)$. [A1, F6, step 1.2, step 2.1, step 3.1, step 3.2] ∎


## Admissible domains for outward normal graphs

[Open item](item-lem-author-c50357f4fa9e-normal-graph-domain) · level 0


### Statement

Assume countable choice $\mathrm{AC}_\omega$, as in the geodesic suppliers. Let $\Sigma$ be a smooth spacelike hypersurface of a time-oriented smooth Lorentzian four-manifold, let $h=g|_{T\Sigma}$, and let $S\subset\operatorname{int}\Sigma$ be a smooth embedded two-surface without boundary carrying a supplied smooth $h$-unit normal $\nu$ in $\Sigma$. Write $D$ for the Levi–Civita connection of $h$. On the open domain where it exists set $T(p,r)=\exp^h_p(r\nu_p)$. Near each $(p,0)$, $T$ is a diffeomorphism onto an open subset of $\Sigma$, and $dT_{(p,0)}(X,a)=X+a\nu_p$.

If $S$ is compact there is $\rho>0$ such that $T:S\times(-\rho,\rho)\to\Sigma$ is a diffeomorphism onto its image. In either a local domain or this compact tube, fix an open domain $\Omega\subset S\times\mathbb R$ containing the relevant zero section on which $T$ is a diffeomorphism. A smooth function $u$ is **admissible** precisely when its graph lies in $\Omega$; then $F_u(p)=T(p,u(p))$ is an embedded spacelike surface parametrization. No uniform graph radius is asserted for a noncompact $S$ without a supplied tube. Each smooth compactly supported $\phi$ admits $u=\epsilon\phi$ for all sufficiently small $|\epsilon|$ whenever such a tube is supplied; the same holds for every smooth $\phi$ on compact $S$.

### Facts & Assumptions

[F1] The hypersurface supplier [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form) supplies the smooth positive metric $h$; [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry) supplies its unique Levi–Civita connection.

[F2] [math:def-domain-and-exponential-map-of-a-connection](https://alphabetamath.cc/item/def-domain-and-exponential-map-of-a-connection) defines the exponential only where the geodesic exists through time one. Under its countable-choice hypothesis, [math:thm-existence-uniqueness-and-smooth-dependence-of-geodesics](https://alphabetamath.cc/item/thm-existence-uniqueness-and-smooth-dependence-of-geodesics) supplies the open geodesic evaluation domain and smooth dependence.

[F3] [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds) turns an invertible differential into a smooth local inverse.

[F4] An embedded surface is understood in the slice-chart sense of [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart). The restricted slice charts supply its smooth structure and subspace topology by [math:lem-slice-chart-restrictions-form-a-smooth-atlas](https://alphabetamath.cc/item/lem-slice-chart-restrictions-form-a-smooth-atlas).

[F5] [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure) supplies the product topology and product smooth charts on $S\times\mathbb R$ and its open subdomains.

[F6] Countable choice is the principle in [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice): from each member of an $\mathbb N$-indexed family of nonempty sets one may choose one element. It is assumed here.

[F7] A smooth embedding is an injective smooth immersion that is a homeomorphism onto its image with the subspace topology, as defined in [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding). By [math:prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-image-of-a-smooth-embedding-is-an-embedded-submanifold), its image is an embedded submanifold and its corestriction to that image is a diffeomorphism.

[F8] The time-oriented smooth Lorentzian four-manifold is the mathematical structure of [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects), clauses (a)–(c). A spacelike hypersurface means an embedded three-submanifold on whose tangent spaces $g$ is positive definite, as in [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets), clause (a). Here an embedded two-surface is called spacelike precisely when the restriction of $g$ to each of its tangent planes is positive definite.

### Proof

**Given:**The structures and countable-choice hypothesis of the Statement.

**Goal:** Establish the stated graph domains and admissible deformations.

1.1 In the restricted and ambient slice coordinates from [F4], the inclusion of $S$ is $x\mapsto(x,0)$; it is therefore smooth with injective differential and identifies $T_pS$ with a two-dimensional subspace of $T_p\Sigma$. In the product charts from [F5], the base projection is smooth and $T_{(p,0)}(S\times\mathbb R)=T_pS\oplus\mathbb R$. In these structures the map $(p,r)\mapsto r\nu_p$ is smooth. Pulling back the open time-one domain in [F2] gives an open domain for $T$ containing every $(p,0)$. The constant geodesic gives $T(p,0)=p$. Uniqueness of geodesics, applied to the reparametrization $t\mapsto\gamma_{p,\nu_p}(rt)$ near $r=0$, gives $T(p,r)=\gamma_{p,\nu_p}(r)$ there, so $\partial_rT(p,0)=\nu_p$. Differentiating the identity on $S$ gives $dT(X,0)=X$. Since $T_p\Sigma=T_pS\oplus\mathbb R\nu_p$, this differential is invertible. The local conclusion follows from [F3]. [F1, F2, F3, F4, F5, given]

2.1 Suppose $S$ is compact. The open domain of definition and the open local-diffeomorphism locus contain the compact zero section, so finitely many product neighborhoods give one $\rho_0>0$ on which $T$ is defined and locally invertible. If no shrinking were injective, for each integer $j$ there would be distinct $(p_j,r_j),(q_j,s_j)$ with $|r_j|,|s_j|<\min(\rho_0,1/j)$ and equal images. Compactness gives a subsequence with $p_j\to p$ and $q_j\to q$. Continuity and the Hausdorff property imply $p=q$, since the common images converge to both $p$ and $q$. Both pairs then lie in a single local inverse neighborhood of $(p,0)$ for large $j$, contradicting injectivity there. Thus a smaller $\rho$ makes $T$ injective; its local inverses agree and yield a smooth inverse on its open image. The pairs are chosen from the fixed nonempty counterexample sets indexed by $j$, using countable choice in [F6]. [F3, F4, F5, F6, step 1.1, given]

3.1 The graph map $p\mapsto(p,u(p))$ is a smooth embedding into $\Omega$ in the sense of [F7]: it is smooth and injective, its inverse on its image is the base projection, and its differential has identity base component. Composition with the diffeomorphism $T$ preserves these properties. By [F7], $F_u(S)$ is an embedded two-submanifold of $\Sigma$ and $F_u:S\to F_u(S)$ is a diffeomorphism. For every nonzero $V\in T_xF_u(S)\subset T_x\Sigma$, $g_x(V,V)=h_x(V,V)>0$ by [F1]; hence the graph is spacelike by the tangent-plane criterion in [F8]. For compact support $K$, finitely many product neighborhoods of $K\times\{0\}$ give a positive radius $\eta$ contained in $\Omega$ above $K$. The finite maximum $M=\max_K|\phi|$ exists. Taking $|\epsilon|M<\eta$ keeps the graph in $\Omega$; off $K$ it is the zero section. For compact $S$ use $K=S$. The case $M=0$ is immediate. This proves all assertions without a completeness hypothesis on $\Sigma$. [step 1.1, step 2.1, F1, F4, F5, F7, F8] ∎


## Asymptotically flat spacelike end and derivative decay

[Open item](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end) · level 0


### Definition

Let $(M,g,N)$ be a time-oriented smooth Lorentzian four-manifold of signature $(-,+,+,+)$. An end chart consists, for a specified $R>0$, of a spacelike embedded hypersurface $S_{\rm ext}\subset M$ without manifold boundary and a specified diffeomorphism from the open exterior $\{x\in\mathbb R^3:|x|>R\}$ onto $S_{\rm ext}$. A finite-radius boundary sphere, if supplied as additional data, is omitted from this chart. All estimates concern $r=|x|\to\infty$ and are unchanged on restriction to $r>R'$ for any $R'>R$. Let $n$ be its unique smooth future unit normal, $\gamma=g|_{TS_{\rm ext}}$ its induced metric, and $k(v,w)=-g(\nabla^g_vn,w)$ its second fundamental form, with the tangential covariant derivative defined independently of smooth local extensions. The sign of $k$ is fixed here; reversing it does not change the decay condition.

For a scalar chart component $f$ and integer $m\ge0$, write $f=O_m(r^{-b})$ if for each multi-index $\beta=(\beta_1,\beta_2,\beta_3)$ with $|\beta|=\beta_1+\beta_2+\beta_3\le m$ there are $C_\beta,R_\beta$ such that $|\partial_x^\beta f(x)|\le C_\beta r^{-b-|\beta|}$ for $r\ge R_\beta$. Here $\partial_x^\beta=\partial_{x^1}^{\beta_1}\partial_{x^2}^{\beta_2}\partial_{x^3}^{\beta_3}$; tensor estimates apply componentwise in this specified chart. Call these end data asymptotically flat when, for some $\alpha>0$ and integer $m\ge2$, $\gamma_{ij}-\delta_{ij}=O_m(r^{-\alpha})$ and $k_{ij}=O_{m-1}(r^{-1-\alpha})$, for $1\le i,j\le3$. The chart and parameters are witnesses to this existential condition; no invariance under arbitrary changes of chart is asserted.

### Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[math:def-directional-and-partial-derivatives](https://alphabetamath.cc/item/def-directional-and-partial-derivatives)

### Facts & Assumptions

[F1] The metric, spacelike induced geometry and metric-selected connection have their library meanings. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets) [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F2] On a spacelike embedded hypersurface without boundary, the future unit normal is unique and smooth, its tangential covariant derivative is independent of local extensions, and the induced metric and second fundamental form are smooth. The supplier uses $K(v,w)=g(\nabla^g_vn,w)$, so the convention here is $k=-K$. [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[F3] A diffeomorphism between smooth manifolds is a bijective smooth map with smooth inverse. [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[F4] For a scalar function on an open subset of $\mathbb R^3$, $\partial_{x^j}f(x)$ is the directional derivative along the $j$th standard basis vector, defined by the derivative at $t=0$ of $t\mapsto f(x+te_j)$ when it exists. [math:def-directional-and-partial-derivatives](https://alphabetamath.cc/item/def-directional-and-partial-derivatives)

### Justification

**Given:** The objects and specified data in the Definition.

**Goal:** Verify that the displayed conditions define unambiguous objects and predicates on these data.

1.1 The open exterior chart and the spacelike embedded hypersurface satisfy the boundaryless hypotheses of [F2]. That supplier gives the unique smooth normal and extension-independent tangential covariant derivative. It also gives smooth induced metric and second fundamental form; taking $k=-K$ preserves smoothness. By [F3] the inverse of the specified diffeomorphism is a smooth coordinate chart on $S_{\rm ext}$. Thus $\gamma_{ij}$ and $k_{ij}$ are well-defined smooth scalar functions in this chart and admit all the iterated coordinate partial derivatives of [F4] used below. [F1, F2, F3, F4]

2.1 For each of finitely many derivatives at each fixed $m$, the displayed inequality is a definite bound on a scalar function outside a sufficiently large ball. Quantifying over their constants, and then over $\alpha$ and $m$, gives the claimed predicate. Replacing $k$ by $-k$ leaves every absolute value unchanged. Restricting to $r>R'$ preserves the bounds after increasing each threshold radius above $R'$; conversely, bounds on that restricted chart already give the required bounds for all sufficiently large $r$ in the original chart. Hence omitting a separately supplied finite-radius boundary sphere has no effect on this decay predicate. [F1, F2, F4, step 1.1] ∎


## Ambient closure and intrinsic boundary of a hypersurface

[Open item](item-def-author-310ff0f53b38-closure-and-boundary-data) · level 0


### Definition

For a subset $S\subset M$, write $\overline S^{\,M}$ for its closure in $M$: a point lies in it precisely when every open neighborhood in $M$ meets $S$. Give $\overline S^{\,M}$ its subspace topology. The ambient boundary of any subset $A\subset M$ is $\partial_M A=\overline A^{\,M}\setminus\operatorname{int}_M A$, where $\operatorname{int}_M A$ is the union of the open subsets of $M$ contained in $A$.

A topological three-manifold with boundary is a Hausdorff, second-countable space locally homeomorphic to relatively open subsets of $\{(y^1,y^2,y^3):y^3\ge0\}$. Its manifold boundary is defined by the boundary-chart convention of the supplier. For hypersurface completion data, require $\overline S^{\,M}$ to be such a manifold, $S$ to be its manifold interior, and $B:=\overline S^{\,M}\setminus S$ to be its manifold boundary and a topological two-manifold without boundary. In particular $B$ is a boundary of the completed three-manifold, whereas $\partial_M S$ is an ambient boundary; the symbols are not interchangeable. No smoothness of $B$ in $M$ is required.

### Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[math:def-topological-manifold-with-and-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-with-and-without-boundary)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

### Facts & Assumptions

[F1] The smooth manifold has its manifold topology. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[F2] Manifolds with boundary and their intrinsic boundary have the specified chart-based meaning. [math:def-topological-manifold-with-and-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-with-and-without-boundary)

[F3] For a subset $A$ of a topological space $X$, its subspace topology consists of the sets $U\cap A$ with $U$ open in $X$; this also defines relatively open subsets. [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

### Justification

**Given:**The objects and specified data in the Definition.

**Goal:** Verify that the displayed conditions define unambiguous objects and predicates on these data.

1.1 The neighborhood predicate determines a unique closure; the union of open subsets determines a unique interior. Their set difference therefore determines the ambient boundary, without selecting charts. [F1]

2.1 The manifold-with-boundary conditions are predicates on the specified subspace topology; requiring that its intrinsic boundary equal $B$ is an additional condition, not a consequence of the closure operation. Thus the completion data distinguish both boundary notions even when only topological boundary charts exist. [F1, F2, F3, step 1.1] ∎


## Causal exterior, chronological boundaries and Cauchy data

[Open item](item-def-causal-exterior-and-boundary-data) · level 1


### Definition

Let $(D,g,N)$ be a time-oriented smooth Lorentzian four-manifold of signature $(-,+,+,+)$, and let $U\subset D$ be a specified open subset. Here a Killing field is a smooth vector field with $\mathcal L_Tg=0$; future timelike means $g(T,T)<0$ and $g(T,N)<0$.

For the stationary-end terminology, supply an end chart: a spacelike embedded hypersurface $S_{\rm ext}\subset D$ without manifold boundary and a specified diffeomorphism $e:\{x\in\mathbb R^3:|x|>R\}\to S_{\rm ext}$ for some $R>0$. This is the end-chart data of the spacelike-end interface, with its finite-radius boundary removed. Also supply a local flow $\Phi:\Omega\to D$ of a specified Killing field $T$, with $\Omega\subset\mathbb R\times D$ open and containing $\{0\}\times D$, in the local-flow interface's sense. Require $U=\{\Phi(t,p):p\in S_{\rm ext},\ (t,p)\in\Omega\}$ and $T$ future timelike on $U$; then call $U$, with these supplied data, a stationary end. The chart supplies the spatial end topology. Metric decay, completeness of the flow and a global product identification of $U$ are additional hypotheses when needed. The causal exterior and boundary constructions below apply to any specified open $U$, independently of whether this end structure is supplied.

For $p,q\in D$, write $p\ll_D q$ when a future-directed timelike curve in $D$ joins $p$ to $q$. Curves are locally absolutely continuous, with nonzero future-directed timelike velocity almost everywhere. Define $I_D^+(U)=\{q\in D:\exists p\in U,\ p\ll_D q\}$ and $I_D^-(U)=\{p\in D:\exists q\in U,\ p\ll_D q\}$. The causal exterior relative to $(D,g,U)$ is $\mathcal E=I_D^-(U)\cap I_D^+(U)$. Its future and past event boundaries relative to $U$ are respectively $\partial_D I_D^-(U)$ and $\partial_D I_D^+(U)$, where $\partial_D A=\overline A^{\,D}\setminus\operatorname{int}_D A$. Closure and interior are taken in the manifold topology of $D$, with their topological-interface meanings. These boundaries are taken in $D$; their intersection and their relation to $\partial_D\mathcal E$ are not prescribed.

A future causal curve has locally absolutely continuous coordinates and nonzero future causal velocity almost everywhere. It is inextendible in $D$ when it converges to no point of $D$ at either parameter end. A subset $S\subset D$ is a Cauchy set in $D$ when every such inextendible causal curve has exactly one parameter value in $S$. A Cauchy hypersurface is a Cauchy set that is also an embedded three-dimensional submanifold with positive-definite induced metric. These conditions are relative to $D$; for a different open domain, inextendibility and the Cauchy condition are recomputed there.

Write $J_D^+(p)$ for $p$ together with points reached from $p$ by future causal curves, and $J_D^-(q)$ for the corresponding causal past. Strong causality means that each point has arbitrarily small open neighborhoods that no future causal curve can leave and subsequently re-enter. Global hyperbolicity means strong causality and compactness in $D$ of every $J_D^+(p)\cap J_D^-(q)$. A temporal function is a smooth real function $\tau$ whose metric gradient is everywhere past-directed timelike, equivalently $g(\nabla\tau,\nabla\tau)<0$ and $d\tau(N)>0$.

For this interface, $(D,g,N)$ is stably causal when there is a smooth Lorentzian metric $\widehat g$ on $D$, with $N$ timelike for $\widehat g$, such that every nonzero $g$-causal vector is $\widehat g$-timelike and $(D,\widehat g,N)$ has no closed future causal curve. This is a separate condition from global hyperbolicity and from the existence of a temporal function; no implication between them is asserted here. In particular, no causal property of a different or deformed metric follows merely from a property of $g$.

### Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity)

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

### Facts & Assumptions

[F1] The time orientation, causal character and Killing-field equation have the meanings in the stated Lorentzian and Killing-field interfaces. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[F2] The curve class, chronological and causal reachability, and endpoint formulation of inextendibility are those of the causal-curve interface, applied to $D$. [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[F3] Strong causality, causal diamonds, global hyperbolicity and temporal functions have the meanings in the causal-conditions interface, applied to $D$. [physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity)

[F4] A Cauchy set counts parameter values of inextendible causal curves, and a Cauchy hypersurface is a spacelike embedded Cauchy set. [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[F5] The spacelike-end interface supplies the end-chart data; only its chart part is used here, while its asymptotic-flatness inequalities remain additional conditions. The local-flow interface supplies the domain, map and integral-curve laws for $\Phi$. [def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F6] Interior is the union of open subsets of a set, closure is the intersection of its closed supersets, and boundary is closure minus interior, all in the chosen topology. [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

### Justification

**Given:** The data $(D,g,N,U)$ in the Definition, with the end chart, $T$ and its local flow supplied when the stationary-end terminology is used.

**Goal:** Check that the defined sets and predicates are unambiguous for those data.

1.1 The specified end chart determines $S_{\rm ext}$ and its spatial exterior coordinates. The supplied local flow defines $\Phi(t,p)$ at exactly the pairs used in the displayed set; equality of that set with $U$ and the timelikeness inequalities are therefore definite predicates on the supplied data. This construction uses only the chart part of the spacelike-end interface and assumes no metric decay or flow completeness. [given, F1, F5]

1.2 The time orientation and metric determine the permitted curve classes and the relations $\ll_D$ and $J_D^\pm$; the displayed existential conditions therefore determine subsets of $D$. Intersection and the closure-minus-interior operation in the specified topology then determine $\mathcal E$ and both named boundaries, including when any of these sets is empty. [F1, F2, F6]

2.1 The Cauchy predicate specifies exactly which curves and parameter values are counted, while the hypersurface, strong-causality, diamond-compactness and temporal predicates use the stated interfaces. The stable-causality clause explicitly quantifies over a second metric and its causal curves, so it too is a definite predicate; it assumes neither the existence of such a metric nor any implication for another metric. [F1, F2, F3, F4, step 1.1, step 1.2] ∎

### External input

Minguzzi's Definition 2.16 supplies the endpoint convention for inextendibility; section 4.4 and Definition 4.89 supply the wider-cone definition of stable causality. The fixed orientation field $N$ selects the future convention used here for both metrics.

Gourgoulhon's section 3.2.1 supplies the conventional once-only intersection wording for a spacelike Cauchy surface. The exact parameter-counting convention used here is supplied by the declared Cauchy-set interface.


## Tangential area Jacobian on a measurable surface domain

[Open item](item-def-author-0336834a2590-surface-map-jacobian) · level 1


### Definition

Work in ZFC. Let $A\subset(C,h)$ be a Borel surface domain on a smooth Hausdorff second-countable Riemannian surface, and let $(\Sigma,k)$ be a finite-dimensional smooth Hausdorff second-countable Riemannian manifold. The target dimension may be arbitrary; the endpoint applications use dimension three. Let $F:A\to\Sigma$ be a map. Require a countable open cover $(U_n)_{n\ge1}$ of $A$ in $C$ and $C^1$ maps $\widetilde F_n:U_n\to\Sigma$ whose restrictions to $A\cap U_n$ equal $F$. Use the disjoint Borel partition $P_n=(A\cap U_n)\setminus\bigcup_{j<n}U_j$.

For a $C^1$ map $G$ on an open subset of $C$, define $dG_p:T_pC\to T_{G(p)}\Sigma$ as follows. In smooth source and target coordinates $x,y$ about $p,G(p)$, its matrix in the coordinate tangent bases is the Euclidean total derivative $D(y\circ G\circ x^{-1})(x(p))$. Thus a tangent vector with $x$-components $v$ is sent to the tangent vector with $y$-components $D(y\circ G\circ x^{-1})(x(p))v$. This definition uses $C^1$ coordinate representatives, not a pullback operation on smooth germs by a possibly nonsmooth map.

Fix a countable smooth atlas of $C$. For $p\in P_n$ having density one for $P_n$ in every atlas chart containing $p$, put $d_AF_p=d\widetilde F_{n,p}$ and $J_2F(p)=\sqrt{\det(k_{F(p)}(d_AF_p(e_i),d_AF_p(e_j)))_{i,j=1}^2}$, where $(e_1,e_2)$ is an $h_p$-orthonormal basis of $T_pC$. On the area-null exceptional set, assign arbitrary finite nonnegative Jacobian values, for example zero. Density one means that the ratio of the Euclidean area of the coordinate image of the intersection of $P_n$ with the chart domain in a ball centered at the point to the area of that ball tends to one as its radius tends to zero. The Gram determinant permits rank loss and vanishes for rank below two; no tangent plane to the image cut is required.

### Facts & Assumptions

**Given:** The objects and extension cover in the Definition.

[A1] Work in ZFC as in the surface-domain convention. Only countable choice is needed here, for countable chart selections and the density theorem. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Borel surface domains and their completed area measure $\mu_C$ have the conventions of [def-author-0336834a2590-measurable-surface-domains](item-def-author-0336834a2590-measurable-surface-domains). In a source chart the measure has smooth positive density $\sqrt{\det(h_{ab})}$ relative to Euclidean area. The source and target metrics are smooth and positive definite as in [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold).

[F2] A $C^1$ map between smooth manifolds has $C^1$ componentwise coordinate representatives on open Euclidean sets. [math:def-c-r-and-smooth-maps-between-smooth-manifolds](https://alphabetamath.cc/item/def-c-r-and-smooth-maps-between-smooth-manifolds)

[F3] The Euclidean total derivative is the linear approximation with normwise remainder $o(|v|)$. Continuous partial derivatives on a neighborhood imply total differentiability, with derivative the Jacobian matrix; the total derivatives satisfy the chain rule on open Euclidean sets. [math:def-total-derivative-in-euclidean-space](https://alphabetamath.cc/item/def-total-derivative-in-euclidean-space) [math:thm-continuous-partial-derivatives-imply-total-differentiability](https://alphabetamath.cc/item/thm-continuous-partial-derivatives-imply-total-differentiability) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F4] Coordinate tangent vectors form a basis, and their change under smooth coordinate transitions is given by the transition Jacobian. [math:thm-coordinate-derivations-form-a-basis-of-the-tangent-space](https://alphabetamath.cc/item/thm-coordinate-derivations-form-a-basis-of-the-tangent-space) [math:thm-change-of-coordinate-formula-for-tangent-bases](https://alphabetamath.cc/item/thm-change-of-coordinate-formula-for-tangent-bases)

[F5] Under countable choice, almost every point of a Lebesgue measurable Euclidean set has density one in that set. [math:thm-lebesgue-density-theorem](https://alphabetamath.cc/item/thm-lebesgue-density-theorem)

### Justification

**Given:** The data in the Definition and the supplied facts above.

1.1 By [F2] and [F3], every coordinate representative of $G$ has a total derivative whose entries are continuous. Under changes of source coordinates $x$ to $x'$ and target coordinates $y$ to $y'$, set $a=x'\circ x^{-1}$, $b=y'\circ y^{-1}$ and $f=y\circ G\circ x^{-1}$. The new representative is $b\circ f\circ a^{-1}$; the chain rule gives its derivative $Db\,Df\,(Da)^{-1}$ at the corresponding points, since differentiating the identities for the smooth transition and its inverse gives inverse derivative matrices. By [F4], source vector components change by $Da$ and target components by $Db$. Hence the two matrices give the same intrinsic linear map on tangent spaces. This establishes the stated $C^1$ differential without extending the smooth-germ pullback definition beyond its hypotheses. [F2, F3, F4, given]

1.2 In each source chart $(V,x)$, the set $x(P_n\cap V)$ is Lebesgue measurable for every Borel piece $P_n$. By the Lebesgue density theorem [F5], its density-one points exhaust that piece up to a Euclidean null set. The smooth positive area density in [F1] is locally bounded above and below away from zero on relatively compact chart patches, so Euclidean and Riemannian null sets there coincide. For each member of a countable base that lies in a chart, choose one such chart; these choices give a countable covering atlas by [A1]. There are countably many chart and piece pairs, so their exceptional sets have a single $\mu_C$-null union. Applying this argument to the union of two countable atlases shows that changing the atlas affects the admissible density-point sets only on a null set. No pointwise coordinate-invariance assertion about density is needed. [A1, F1, F5]

2.1 At a density-one point $p$ of a piece, two $C^1$ extensions agreeing on that piece have the same value at $p$. In a common target chart, subtract their coordinate representatives. Their difference is zero on the piece and has expansion $Lz+o(|z|)$ at $p$. If $L\ne0$, choose a direction $w$ with $Lw\ne0$; on a small cone about $w$ there is $c>0$ with $|Lz|\ge c|z|$. For sufficiently small nonzero $z$ in that cone the expansion cannot vanish. The cone occupies a fixed positive fraction of each centered ball, contradicting density one. Therefore $L=0$, and step 1.1 identifies the two intrinsic differentials. For two countable partitions, discard their null exceptional sets from step 1.2; a point in both remaining density-one pieces has density one in their intersection, since the missing fractions add. The same argument on this intersection proves independence almost everywhere of both extensions and partitions. [F1, F2, F3, step 1.1, step 1.2]

3.1 On each Borel piece the Gram Jacobian of its extension is continuous in local coordinates: writing $H$ for the positive definite source metric matrix, $K$ for the target metric matrix at the image, and $B$ for the derivative matrix, its square is $\det(B^T K B)/\det H$. This is nonnegative, including rank loss. Thus the piecewise Jacobian is measurable, and changing it on the null exceptional set preserves measurability for the completed measure $\mu_C$. Orthogonal source basis changes conjugate its Gram matrix and preserve its determinant. If the derivative takes values in a smooth target surface with the induced metric, its matrix $M$ in orthonormal surface bases satisfies $\det(M^TM)=(\det M)^2$; hence the square root is the absolute determinant. These facts retain the arbitrary-rank definition and require no smoothness of the image cut. [F1, F2, F3, F4, step 1.1, step 1.2, step 2.1, algebra] ∎

### Source notes

The Lebesgue density theorem, under the standing ZFC convention, supplies the density-one assertion on every Borel partition piece in source charts. [math:thm-lebesgue-density-theorem](https://alphabetamath.cc/item/thm-lebesgue-density-theorem)


## Counting multiplicity of an endpoint map

[Open item](item-def-author-0336834a2590-endpoint-multiplicity) · level 1


### Definition

For a Borel surface domain $A$ and a locally Lipschitz map $F:A\to\Sigma$, define $N(F,A;y)=\#\{x\in A:F(x)=y\}$, taking values in $\{0,1,2,\ldots,\infty\}$. The image is $D=F(A)$. Surjectivity onto $D$ gives $N(F,A;y)\ge1$ on $D$; injectivity is the additional condition $N(F,A;y)=1$ there. Integration of multiplicity is with the completed normalized Hausdorff area measure. For the maps with local $C^1$ extensions considered here, the area theorem supplies its measurability.

### Facts & Assumptions

[A1] Work in ZFC, as in the surface-domain convention. Countable choice is used when selecting the countable local cover below. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Use the smooth Hausdorff second-countable source surface, target three-manifold, finite component distances, Borel domains and complete normalized Hausdorff measures of [def-author-0336834a2590-measurable-surface-domains](item-def-author-0336834a2590-measurable-surface-domains). Source area equals normalized intrinsic Hausdorff area and is locally finite; target measurability is interpreted componentwise.

[F2] A map is $L$-Lipschitz when its target distance is at most $L$ times its source distance, for some finite $L\ge0$. Locally Lipschitz on $A$ means this bound holds on a relative neighborhood of each point, using the specified component distances. [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction)

[F3] Under countable choice, a second-countable space is Lindelöf. The intersections of a countable source basis with $A$ form a countable basis of $A$. [math:thm-second-countable-implies-lindelof](https://alphabetamath.cc/item/thm-second-countable-implies-lindelof)

[F4] The independent metric-space measurability input is recorded in External input. Its finite-domain hypothesis is checked separately on each piece below.

### External input

Simon, Theorem 1.8(i)–(ii): if $X,Y$ are metric spaces, $X$ is $\sigma$-compact, $B\subseteq X$ is $\mathcal H^m$-measurable with finite measure and $f:B\to Y$ is Lipschitz, then $f(B)$ and $y\mapsto\#f^{-1}(y)$ are $\mathcal H^m$-measurable. This established input is imported; the following application is proved locally.

### Justification

**Given:** The Borel domain, map and componentwise metric and area conventions in the Definition, with [A1] and [F1]–[F4].

1.1 This counts distinct initial points rather than parameter charts. A disjoint partition of $A$ therefore avoids counting a point twice merely because it belongs to overlapping charts. Multiple distinct initial points can have the same endpoint; they must all be retained in $N$. The inequality $N\ge1$ on the image follows directly from the definition of image. [given]

1.2 Each point of $A$ has a relative neighborhood on which $F$ is Lipschitz. Lipschitz continuity and openness of target components let us shrink it so that its image lies in one target component. Choose a source coordinate ball inside the corresponding source component, with compact closure inside a chart, small enough that its intersection with $A$ lies in this neighborhood. Such balls $U_i$ admit a countable subcover of $A$ by [F3]. Write $K_i=\overline{U_i}$ and $A_i=(A\cap U_i)\setminus\bigcup_{j<i}U_j$. Then the $A_i$ form a disjoint Borel partition of $A$, each $K_i$ is a compact metric space for the restricted source component distance, and $F|_{A_i}$ is Lipschitz into a single target component. Local finiteness of the source area and compactness give $\mathcal H_h^2(K_i)<\infty$ by a finite cover with finite-area neighborhoods; hence each $A_i$ has finite area. Hausdorff measure for a restricted metric agrees on subsets with the ambient source Hausdorff measure: intersecting ambient covers with $K_i$ gives the same diameter-cover infima. Thus $A_i$ is also measurable with finite measure as a subset of $K_i$. [A1, F1, F2, F3]

2.1 Apply [F4] with $m=2$, $X=K_i$, $B=A_i$ and $Y$ the indicated target component. Compact $K_i$ is $\sigma$-compact. Its Borel subset $A_i$ is measurable and has finite measure by step 1.2, and the required Lipschitz bound holds there. Consequently $D_i=F(A_i)$ and $N_i(y)=\#\{x\in A_i:F(x)=y\}$ are measurable for the complete target Hausdorff measure. Multiplying a Hausdorff outer measure by a positive constant changes neither its Carathéodory measurable sets nor its measurable functions, so the conclusion holds with the normalization in [F1]. Extend $N_i$ by zero on all other target components; this is measurable componentwise. [F1, F4, step 1.2]

3.1 The disjoint source partition gives $N(F,A;y)=\sum_iN_i(y)$ pointwise, with every infinite fiber represented by the value $\infty$, and $D=\bigcup_iD_i$. To check measurability of the sum directly, for each positive integer $q$ its superlevel set is the union, over $m\ge1$ and tuples $(a_1,\ldots,a_m)\in\{0,\ldots,q\}^m$ with $\sum_i a_i=q$, of the measurable sets $\bigcap_{i=1}^m\{N_i\ge a_i\}$. If the total count is at least $q$, finitely many summands already contain $q$ points, which proves this equality also for infinite counts. These countable unions and finite intersections show that $N$ is measurable, including at value $\infty$. The countable union of the $D_i$ is measurable as well. This proves the measurability needed for integration in the Definition, in particular for its locally $C^1$-extendible maps, without using the downstream endpoint-area lemma. [F1, step 1.1, step 2.1] ∎



## Canonical outward normals and null gauge on a graph

[Open item](item-lem-author-c50357f4fa9e-outward-graph-null-gauge) · level 1


### Statement

Use an admissible normal graph $F_u$ in the tube of the preceding graph-domain lemma, and let $n$ be the smooth future unit normal to the fixed hypersurface $\Sigma$. In tube coordinates $(x^1,x^2,r)$ the covector $\alpha_u=dr-(\partial_a u)dx^a$, evaluated at $(x,u(x))$, annihilates the graph tangent plane. Write $h$ also for its pullback $T^*h$ to the tube. For a tube covector $\alpha$, let $\alpha^{\sharp_h}$ be the unique vector satisfying $h(\alpha^{\sharp_h},V)=\alpha(V)$ for every tube tangent vector $V$, and define $|\alpha|_h=\sqrt{h(\alpha^{\sharp_h},\alpha^{\sharp_h})}$. Set $\nu_u=\alpha_u^{\sharp_h}/|\alpha_u|_h$, and push this vector to $\Sigma$. These definitions agree on overlaps and give the outward smooth $h$-unit normal along the graph, with $\nu_0=\nu$. Here **outward** means positive pairing with $T_*\partial_r$.

The fields $L_u=n+\nu_u$ and $\underline L_u=(n-\nu_u)/2$ along the graph are future null normals satisfying $g(L_u,\underline L_u)=-1$. They depend smoothly on the first graph data $(x,u,\partial u)$ and fix the normal gauge throughout the deformation, rather than choosing a new arbitrary boost at each parameter.

### Facts & Assumptions

[F1] [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain) supplies $T$, the admissible graph and its embedding into $\Sigma$.

[F2] [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form) supplies the smooth future unit normal $n$ of this fixed hypersurface and its smooth induced positive metric $h$.

[F3] [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry) defines null expansion and the effect of changing a null normal's positive scale; its normalized second null normal may be rescaled from pairing $-2$ to pairing $-1$.

[F4] [math:def-pullback-riemannian-metric](https://alphabetamath.cc/item/def-pullback-riemannian-metric) defines $(T^*h)_z(V,W)=h_{T(z)}(dT_zV,dT_zW)$. Since $T$ is the diffeomorphism supplied by [F1], this tensor is a smooth positive definite metric on the tube.

[F5] [math:def-musical-isomorphisms](https://alphabetamath.cc/item/def-musical-isomorphisms) defines $\alpha^{\sharp_h}$ by $h(\alpha^{\sharp_h},V)=\alpha(V)$. The covector norm in the Statement is defined from this vector and the positive metric $h$.

### Proof

**Given:**An admissible graph in the supplied tube, with $h,n,\nu$ as above.

**Goal:** Justify the smooth, normalized outward graph gauge.

1.1 The scalar function $r-u(p)$ is defined on the part of the tube over the domain of $u$, independently of a coordinate chart on $S$. Its differential is $\alpha_u$ and takes value one on $\partial_r$. It is nonzero and annihilates each tangent vector $\partial_a+(\partial_a u)\partial_r$ to the graph. The tube metric is smooth and positive definite by [F4]. The defining identity in [F5] gives $h(\alpha_u^{\sharp_h},V)=\alpha_u(V)$, so $\alpha_u^{\sharp_h}\ne0$ and $|\alpha_u|_h>0$. Dividing by this norm and pushing forward by $T$ gives a unique smooth unit normal with positive pairing with $T_*\partial_r$, since $h(\alpha_u^{\sharp_h}/|\alpha_u|_h,\partial_r)=1/|\alpha_u|_h>0$. At $u=0$, $dT(X,0)=X$ and $T_*\partial_r=\nu$ by [F1], so this normal is $\nu$. The scalar construction makes the local formulas agree. The inverse-matrix and square-root formulas show smooth dependence on $(x,u,\partial u)$. [F1, F2, F4, F5, given, algebra]

2.1 Orthogonality gives $g(n,n)=-1$, $g(\nu_u,\nu_u)=1$, $g(n,\nu_u)=0$. Direct multiplication gives $g(L_u,L_u)=g(\underline L_u,\underline L_u)=0$ and $g(L_u,\underline L_u)=-1$. Both are nonzero and future-directed because their scalar product with the future timelike $n$ is negative. They are normal to the graph. The factors used to normalize the second null vector do not affect the expansion of $L_u$, defined by [F3]. This proves the stated gauge with its smoothness and orientation. [F2, F3, step 1.1, algebra] ∎


## Complete stationary flow and its exterior region

[Open item](item-def-author-310ff0f53b38-stationary-flow-exterior) · level 1


### Definition

Let $(M,g,N)$ be a time-oriented Lorentzian four-manifold and $T$ a smooth Killing field. Completeness means that the flow $\phi:\mathbb R\times M\to M$ of $T$ is defined for every real time and every point, with $\phi_0$ the identity and $\phi_{s+t}=\phi_s\circ\phi_t$. 

A specified spacelike end $S_{\rm ext}$ has the end-chart data of the spacelike-end interface: a spacelike embedded hypersurface without manifold boundary and a specified diffeomorphism $\chi:\{x\in\mathbb R^3:|x|>R_0\}\to S_{\rm ext}$, where $R_0>0$. Its radius is $r(\chi(x))=|x|$. Only these end-chart data are used here; no asymptotic decay condition is required. Require a specified $R_1>R_0$ such that $T$ is future timelike on $\chi(\{x:|x|\ge R_1\})$. The set $\{x:|x|\ge R_1\}$, including its finite-radius sphere, lies inside the original open chart domain. Restrict the chart to this tail and denote its image again by $S_{\rm ext}$; only this subset is used in the flow saturation $M_{\rm ext}=\bigcup_{t\in\mathbb R}\phi_t(S_{\rm ext})$. All subsequent sets are relative to this specified restricted end.

All chronological relations here are computed in $M$: $I^+(A)=\{q:\exists p\in A,\ p\ll_Mq\}$ and $I^-(A)=\{p:\exists q\in A,\ p\ll_Mq\}$. Define $D=I^+(M_{\rm ext})\cap I^-(M_{\rm ext})$, and define $\mathcal E^+=\partial_M D\cap I^+(M_{\rm ext})$ and $\mathcal E^-=\partial_M D\cap I^-(M_{\rm ext})$. The subscript on $\partial_M$ specifies the ambient topological boundary: for $A\subseteq M$, $\partial_M A=\overline A^{\,M}\setminus\operatorname{int}_M(A)$, with closure and interior taken in the manifold topology of $M$. These are the future and past portions of the boundary of the domain of outer communications; the full future event boundary is instead $\partial_M I^-(M_{\rm ext})$. These expressions define separate sets; no equality between them is built into their names.

### Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end)

[math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

### Facts & Assumptions

[F1] Lorentzian causal character, the Killing-field predicate and the global-flow laws are supplied interfaces. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F2] The relation $\ll_M$ is chronological reachability by future timelike curves in $M$. [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[F3] The supplied end-chart interface specifies a spacelike embedded hypersurface without manifold boundary and its open exterior chart. Only these end-chart data are used; its additional asymptotic decay predicate is not assumed. The closed tail at $R_1>R_0$ is the specified restriction inside that chart. [def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end)

[F4] In any topological space, the boundary of a subset is its closure minus its interior. Apply this definition to the manifold topology of $M$. [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

### Justification

**Given:**The objects and specified data in the Definition.

**Goal:** Verify that the displayed conditions define unambiguous objects and predicates on these data.

1.1 Since $R_1>R_0$, every point with $|x|\ge R_1$ belongs to the original open chart domain. Restricting the specified chart therefore determines the closed tail, including its sphere, as a subset of $M$ without any extension of the chart. Globality of the supplied flow makes $\phi_t(S_{\rm ext})$ defined for every real $t$, so its union specifies a subset of $M$. The flow law gives $\phi_s(M_{\rm ext})=M_{\rm ext}$, since $t\mapsto t+s$ permutes $\mathbb R$. [F1, F3]

2.1 The chronological predicates then specify the two subsets $I^\pm(M_{\rm ext})$. Their intersection, its boundary in $M$, and the indicated intersections determine all the named sets. This construction needs no theorem identifying their topology or smoothness. [F2, F4, step 1.1] ∎


## Area formula and endpoint bound with multiplicity

[Open item](item-lem-author-0336834a2590-endpoint-area-with-multiplicity) · level 2


### Statement

Let $A\subset(C,h)$ be Borel and let $F:A\to(\Sigma,k)$ have a countable cover by local $C^1$ extensions as in the Jacobian definition. Put $D=F(A)$. With the normalized measures and the counting multiplicity defined above, the extended nonnegative integrals satisfy $\int_A J_2F\,d\mu_C=\int_D N(F,A;y)\,d\mathcal H_k^2(y)$. In particular $|D|\le\int_A J_2F\,d\mu_C$. If $F$ is one-to-one almost everywhere in the image sense $N=1$ for $\mathcal H_k^2$-almost every $y\in D$, equality holds in that inequality. If also $J_2F\le1$ almost everywhere, then $|D|\le|A|$. The image is countably two-rectifiable.

### Facts & Assumptions

[F1] Use the domain, normalized measures, Jacobian and counting multiplicity in [def-author-0336834a2590-measurable-surface-domains](item-def-author-0336834a2590-measurable-surface-domains), [def-author-0336834a2590-surface-map-jacobian](item-def-author-0336834a2590-surface-map-jacobian) and [def-author-0336834a2590-endpoint-multiplicity](item-def-author-0336834a2590-endpoint-multiplicity).

[F2] The Euclidean weighted area formula is the external input below; it includes measurable source subsets and counting multiplicity, rather than requiring injectivity.

[F3] Under the ZFC convention in [F1], an $L$-Lipschitz map between metric spaces satisfies $\mathcal H^2(f(E))\le L^2\mathcal H^2(E)$ for $L>0$. The common positive normalization preserves this inequality. [math:thm-hausdorff-measure-under-lipschitz-maps](https://alphabetamath.cc/item/thm-hausdorff-measure-under-lipschitz-maps)

### External input

Simon, Chapter 2, equations (3.3), (3.5), (4.12), (4.14), supplies the Euclidean weighted area formula with counting multiplicity and the tangent Gram Jacobian. This premise is imported. The Riemannian passage and endpoint consequences are proved locally below.

### Proof

**Given:** The objects and hypotheses of the Statement, with [F1]–[F3].

**Goal:** Prove the area identity, rectifiability, and the stated multiplicity bounds.

1.1 Use the ZFC, componentwise distance and normalized measure conventions in [F1]. Refine the countable extension cover into source coordinate balls with compact closures inside extension domains and with images in target charts, and subtract earlier balls to obtain a disjoint Borel partition $(A_i)$. Further such refinements remain countable. Bounded derivatives on smaller coordinate balls make each coordinate extension Lipschitz. The Jacobian supplier identifies its derivative with $d_AF$ almost everywhere on each partition piece; the multiplicity supplier gives measurability of each image and its count. With source metric matrix $H$, target metric matrix $K$ and coordinate derivative $B$, the coordinate density of $J_2F\,d\mu_C$ is $\sqrt{\det(B^TKB)}$, since the factor $\sqrt{\det H}$ cancels its reciprocal in $J_2F$. [F1, given, algebra]

2.1 Fix $0<\varepsilon<1$ and put $a=1-\varepsilon$, $b=1+\varepsilon$. Around each target point take linearly normalized coordinates with metric matrix equal to the identity at the center. Smoothness gives a coordinate ball $B_R$ on which $a^2I\le K\le b^2I$. Restrict to $B_r$ with $r<R/3$: straight segments give the upper distance bound $d_k(v^{-1}z,v^{-1}w)\le b|z-w|$. Curves staying in $B_R$ have length at least $a|z-w|$; a curve leaving it has initial displacement at least $R-r>2r\ge|z-w|$ before its first exit and obeys the same lower bound. Thus the restricted ambient component distance is at least $a|z-w|$ as well. Applying [F3] to the coordinate map and its inverse yields $a^2\mathcal H^2_{\mathrm E}(E)\le\mathcal H_k^2(v^{-1}E)\le b^2\mathcal H^2_{\mathrm E}(E)$ on this patch. Refine the partition in step 1.1 so every image lies in such a patch. The same quadratic-form bounds give $a^2\sqrt{\det(B^TB)}\le\sqrt{\det(B^TKB)}\le b^2\sqrt{\det(B^TB)}$; if $B$ has rank below two all three determinants vanish. [F1, F3, step 1.1, algebra]

3.1 Write $f_i=v_i\circ F\circ u_i^{-1}$ on $u_i(A_i)$ and let $N_i$ count preimages in $A_i$. Apply [F2] to the Lipschitz coordinate extension on this Borel subset of $\mathbb R^2$, with Euclidean target dimension three and normalized Euclidean measures. It gives $T_i:=\int_{u_i(A_i)}\sqrt{\det(Df_i^TDf_i)}\,d\lambda_2=\int_{f_i(u_i(A_i))}N_i(v_i^{-1}z)\,d\mathcal H^2_{\mathrm E}(z)$. Let $I_i=\int_{A_i}J_2F\,d\mu_C$ and $R_i=\int_{F(A_i)}N_i\,d\mathcal H_k^2$. Steps 1.1 and 2.1 give $a^2T_i\le I_i\le b^2T_i$ and $a^2T_i\le R_i\le b^2T_i$; the measure inequalities apply to nonnegative integrals by simple-function approximation. Hence $(a/b)^2I_i\le R_i\le(b/a)^2I_i$, also for infinite values. Since the source pieces are disjoint, $\sum_iN_i=N(F,A;\cdot)$, with counts extended by zero off their images, so summing gives $(a/b)^2I\le R\le(b/a)^2I$ for the two integrals $I,R$ in the Statement. Although the partition depends on $\varepsilon$, these full integrals do not. Let $\varepsilon$ decrease to zero: finite values are squeezed to equality, and an infinite value forces the other to be infinite. This proves the metric identity without assuming disjoint images. [F1, F2, step 1.1, step 2.1, algebra]

4.1 Each piece in step 1.1 is parametrized by a subset of $\mathbb R^2$; its coordinate extension is Lipschitz and the target inverse chart is Lipschitz for the component distance by step 2.1. These countably many maps cover $D$, proving countable two-rectifiability in the stated convention. Since $N\ge1$ on $D$, the identity gives $|D|\le I$. If $N=1$ almost everywhere on $D$, its right integral is $|D|$, giving equality. If also $J_2F\le1$ almost everywhere, then $I\le\mu_C(A)=|A|$. No injectivity or smoothness of the image cut was used. [F1, step 1.1, step 2.1, step 3.1] ∎


## Outgoing expansion depends smoothly on the second graph data

[Open item](item-lem-author-c50357f4fa9e-expansion-second-jet) · level 2


### Statement

Assume countable choice $\mathrm{AC}_\omega$. Use the normal-graph data: a smooth spacelike hypersurface $\Sigma$ in a time-oriented smooth Lorentzian four-manifold, its induced metric $h=g|_{T\Sigma}$, a smooth embedded two-surface $S\subset\operatorname{int}\Sigma$ without boundary with a supplied smooth outward $h$-unit normal $\nu$, and a supplied normal-graph domain $\Omega$ on which $T(p,r)=\exp^h_p(r\nu_p)$ is a diffeomorphism onto its image. A smooth $u$ is admissible when its graph lies in $\Omega$, and $F_u(p)=T(p,u(p))$. The domain may be local; no uniform tube for noncompact $S$ is assumed.

For an admissible graph in the fixed spacelike hypersurface and its canonical gauge, let $q_u=F_u^*h$ and $\Theta(u)=F_u^*(\theta_{L_u})$. The pullback means that each scalar is evaluated at the point $F_u(p)$ and regarded as a function of $p\in S$. Locally there is a smooth scalar function $A$ such that $$\Theta(u)(x)=A(x,u(x),\partial_a u(x),\partial_a\partial_bu(x)).$$ Thus the expansion uses only the **second graph data** (the value, first partials and symmetric second partials at the same point). Its coordinate expressions agree because it is the trace of a geometric tensor. No ambient extension of the normal fields is part of this construction.

More explicitly, choose coordinates $x^a$ on $S$ and $y^i$ on $\Sigma$, with $a,b=1,2$ and $i,j,k,\ell=1,2,3$. Put $E_a^i=\partial_aF_u^i$, write $q_u^{ab}$ for the inverse of $q_{u,ab}=h_{ij}(F_u)E_a^iE_b^j$, let $K(X,Y)=g(\nabla_Xn,Y)$, and let $\Gamma^i{}_{jk}$ be the coefficients of the Levi–Civita connection of $h$. Repeated indices are summed. The exact coordinate formula is
$$\Theta(u)=q_u^{ab}\left(K_{ij}(F_u)E_a^iE_b^j-h_{i\ell}(F_u)\nu_u^\ell\left(\partial_a\partial_bF_u^i+\Gamma^i{}_{jk}(F_u)E_a^jE_b^k\right)\right).$$
Writing $T_r=\partial_rT$ evaluated at $(x,u(x))$, this can equivalently be expressed as
$$\Theta(u)(x)=-q_u^{ab}h(\nu_u,T_r)\partial_a\partial_bu+R(x,u,\partial u),$$
where $R$ is a smooth real function of the first graph data on the coordinate domain. Thus the displayed second-partial term is the only dependence on second derivatives of $u$. At the zero graph, $T_r(p,0)=\nu_p$ and $\nu_0=\nu$, so $h(\nu_0,T_r(p,0))=1$.

### Facts & Assumptions

[F1] [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge) supplies the smooth canonical null gauge and first-data dependence of $\nu_u$.

[F2] [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form) supplies $K(X,Y)=g(\nabla_Xn,Y)$ on $\Sigma$, with $K$ smooth, and [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry) supplies the Levi–Civita connection $D$ of $h$.

[F3] [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry) defines $\theta_L$ as the trace of $g(\nabla_XL,Y)$ on the spacelike surface, with tangential extension independence.

[F4] [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps) supplies differentiation of composites.

[F5] [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain) supplies the normal-graph domain $\Omega$, the smooth diffeomorphism $T$, admissibility, and the embedded spacelike parametrization $F_u(p)=T(p,u(p))$, under the stated countable-choice hypothesis.

[F6] Adopt countable choice $\mathrm{AC}_\omega$ in the sense of [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice). This is the hypothesis inherited by the graph construction in [F5] and the smooth Lorentzian and screen conventions in [F3]; no stronger choice principle is assumed.

[F7] [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection), clauses (a)–(d), defines and constructs the ambient metric-selected connection $\nabla$: it is $g$-compatible and torsion-free, with $X(g(Y,Z))=g(\nabla_XY,Z)+g(Y,\nabla_XZ)$ and $\nabla_XY-\nabla_YX=[X,Y]$. Its countable-choice hypothesis is [F6].

### Proof

[F1] [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge) supplies the smooth canonical null gauge and first-data dependence of $\nu_u$.

[F2] [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form) supplies $K(X,Y)=g(\nabla_Xn,Y)$ on $\Sigma$, with $K$ smooth, and [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry) supplies the Levi–Civita connection $D$ of $h$.

[F3] [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry) defines $\theta_L$ as the trace of $g(\nabla_XL,Y)$ on the spacelike surface, with tangential extension independence.

[F4] [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps) supplies differentiation of composites.

[F5] [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain) supplies the normal-graph domain $\Omega$, the smooth diffeomorphism $T$, admissibility, and the embedded spacelike parametrization $F_u(p)=T(p,u(p))$, under the stated countable-choice hypothesis.

[F6] Adopt countable choice $\mathrm{AC}_\omega$ in the sense of [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice). This is the hypothesis inherited by the graph construction in [F5] and the smooth Lorentzian and screen conventions in [F3]; no stronger choice principle is assumed.



**Given:** The normal-graph data and admissible graph from [F5], the canonical gauge from [F1], and the countable-choice assumption in [F6].

**Goal:** Establish the exact expansion formula, its second-partial coefficient and the smooth local second-data expression.

1.1 The assumption in [F6] supplies the inherited countable-choice hypotheses of [F5] and [F3]. In any ambient coordinate chart $y^i$ on $\Sigma$ write $E_a^i=\partial_aF_u^i$ and $q_{ab}=h_{ij}(F_u)E_a^iE_b^j$. The $E_a$ depend smoothly on $(x,u,\partial u)$ by [F4]. Since the graph is an immersion into a Riemannian hypersurface, $\det q>0$; hence the cofactor formula makes $q^{ab}$ a smooth function of those same data. The normal $\nu_u$ has the same dependence by [F1]. Let $\Gamma^i{}_{jk}$ denote the smooth Christoffel coefficients of $D$ in this ambient chart. The connection with coefficients $D$ is the tangential part of the ambient metric connection on $\Sigma$: that projection is metric compatible and torsion free by [F7], hence equals $D$ by uniqueness in [F2]. Consequently, for $X$ tangent to the graph $F_u(S)$ and $Y$ tangent to $\Sigma$ along that graph, $g(\nabla_X\nu_u,Y)=h(D_X\nu_u,Y)$. Both derivatives are pullback covariant derivatives along the graph, so no off-graph values of $\nu_u$ are required. [F1, F2, F3, F4, F5, F6, F7, given, algebra]

2.1 Differentiating $h(\nu_u,E_b)=0$ along the graph using metric compatibility gives $h(D_{E_a}\nu_u,E_b)=-h(\nu_u,D_{E_a}E_b)$. The covariant derivative along the parametrization has components $\partial_a\partial_bF_u^i+\Gamma^i{}_{jk}(F_u)E_a^jE_b^k$. Splitting $L_u=n+\nu_u$ and taking the trace in [F3] therefore gives exactly the coordinate formula in the Statement: $$\Theta(u)=q_u^{ab}\left(K_{ij}(F_u)E_a^iE_b^j-h_{i\ell}(F_u)\nu_u^\ell\left(\partial_a\partial_bF_u^i+\Gamma^i{}_{jk}(F_u)E_a^jE_b^k\right)\right).$$ Here $q_u^{ab}$ is the inverse matrix denoted $q^{ab}$ in step 1.1. All factors other than the displayed second derivatives of $F_u$ depend smoothly only on $(x,u,\partial u)$. [F1, F2, F3, F4, F5, step 1.1, algebra]

3.1 The chain rule for $F_u^i=T^i(x,u(x))$ gives $\partial_a\partial_bF_u^i=T_r^i\partial_a\partial_bu+C_{ab}^i(x,u,\partial u)$, where $C_{ab}^i$ is smooth: differentiating $\partial_bF_u^i=T_b^i+T_r^i\partial_bu$ leaves only derivatives of $T$ and products of first partials of $u$ after removing the displayed second-partial term. Substitution into step 2.1 gives the stated smooth remainder $R$ and coefficient $-q_u^{ab}h(\nu_u,T_r)$. At $u=0$, [F5] gives $T_r(p,0)=\nu_p$, and [F1] gives $\nu_0=\nu$, whose $h$-norm is one. The coefficient pairing is therefore one there. The same formula defines the asserted smooth $A(x,u,\partial u,\partial^2u)$. Derivatives of normal fields occur only along the graph, so [F3] gives extension independence; the trace is a scalar, so its coordinate expressions agree. This proves both the original second-data assertion and the exact formula. [F1, F2, F3, F4, F5, step 1.1, step 2.1, algebra] ∎


## Null generators and once-only cross-sections

[Open item](item-def-author-310ff0f53b38-null-generator-cross-section) · level 2


### Definition

Assume Countable Choice for the general construction, as required by the supplied smooth tangent-bundle and vector-field interfaces. Let $H\subset M$ be a specified horizon subset of a time-oriented smooth Lorentzian four-manifold $(M,g,N)$. An affinely parametrized null geodesic is a smooth curve $c:I\to M$, where $I\subseteq\mathbb R$ is an interval with nonempty interior, with nonzero future-directed tangent, $g(\dot c,\dot c)=0$ and $D_s\dot c=0$. Here $D_s$ is the covariant derivative along $c$ induced by the Levi–Civita connection $\nabla^g$; the notation $\nabla^g_{\dot c}\dot c$ means this derivative along the curve, without requiring an ambient extension of $\dot c$. In chart coordinates $c^a=x^a\circ c$, the equivalent equation is $\ddot c^a+\Gamma^a{}_{bc}(c)\dot c^b\dot c^c=0$. At an included endpoint, smoothness and these derivatives have the one-sided interpretation.

A generator of $H$ means the image of such a null geodesic maximally continued while remaining in $H$; two affine parametrizations with the same image describe the same generator. A finite endpoint belonging to $H$ may be included, with the preceding endpoint convention. Maximal continuation here is relative to $H$, and is not a claim of affine geodesic completeness in $M$.

For the family $\mathcal G(H)$ of these generator images, a once-only cross-section is a subset $B\subset H$ such that $B\cap G$ has exactly one point for every $G\in\mathcal G(H)$. This counts points, not affine parameter values. It imposes neither smoothness nor a normalization of tangent fields. Coverage of an arbitrary $H$ by generators, future inextendibility, and regularity of a particular horizon are separate geometric assertions; they are not proved merely by this terminology.

For the stationary application, take an asymptotically flat spacelike end $S_{\rm ext}$ and a complete Killing field $T$ future timelike on that end, and use its flow saturation $M_{\rm ext}$ and chronological exterior $D=I_M^+(M_{\rm ext})\cap I_M^-(M_{\rm ext})$. In this causal-boundary application assume also Dependent Choice, as in the chronology-openness supplier. Define the full future event horizon by $H^+=\partial_M I_M^-(M_{\rm ext})$ and its portion by $\mathcal E^+=\partial_M D\cap I_M^+(M_{\rm ext})$. Then $\mathcal E^+=H^+\cap I_M^+(M_{\rm ext})$. For the cited causal-boundary assertion use also the source's asymptotic convention: $g(T,T)\le-\epsilon<0$ for some $\epsilon>0$ at sufficiently large radius on $S_{\rm ext}$. This uniformity is not needed for the portion identity. The cited input then provides, from each point of $H^+$, a future-inextendible null geodesic ray staying in $H^+$; its past continuation can exit $H^+$. Inextendibility here means absence of a future endpoint in $M$, not infinite affine parameter length. For a portion $\mathcal E^+\subset H^+$, use the maximal connected pieces of the horizon generator curves lying in that portion, and then their images. The once-only condition uses those images; it does not assert existence of a section.

### Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[math:def-covariant-derivative-along-a-curve](https://alphabetamath.cc/item/def-covariant-derivative-along-a-curve)

[math:def-geodesic-of-an-affine-connection](https://alphabetamath.cc/item/def-geodesic-of-an-affine-connection)

[math:prop-coordinate-geodesic-equation](https://alphabetamath.cc/item/prop-coordinate-geodesic-equation)

[def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end)

[def-author-310ff0f53b38-stationary-flow-exterior](item-def-author-310ff0f53b38-stationary-flow-exterior)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:def-dependent-choice](https://alphabetamath.cc/item/def-dependent-choice)

[physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

### Facts & Assumptions

[F1] Causal character, future direction and endpoint-based causal inextendibility use the Lorentzian and causal-curve conventions. Countable Choice is assumed for the smooth tangent-bundle and vector-field constructions in the Lorentzian and metric-selected-connection interfaces. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability) [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection) [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F2] The metric-selected connection induces the derivative along a curve; its geodesic condition, equivalent coordinate equation and one-sided endpoint interpretation are the supplied mathematical interfaces. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection) [math:def-covariant-derivative-along-a-curve](https://alphabetamath.cc/item/def-covariant-derivative-along-a-curve) [math:def-geodesic-of-an-affine-connection](https://alphabetamath.cc/item/def-geodesic-of-an-affine-connection) [math:prop-coordinate-geodesic-equation](https://alphabetamath.cc/item/prop-coordinate-geodesic-equation)

[F3] The end data and complete stationary flow specify $S_{\rm ext}$, $M_{\rm ext}$, $D$ and $\mathcal E^+$. [def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end) [def-author-310ff0f53b38-stationary-flow-exterior](item-def-author-310ff0f53b38-stationary-flow-exterior)

[F4] Under Countable Choice and Dependent Choice, each $I_M^+(p)$ is open; hence $I_M^+(M_{\rm ext})$, its union over $p\in M_{\rm ext}$, is open. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) [math:def-dependent-choice](https://alphabetamath.cc/item/def-dependent-choice) [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[F5] The stationary event-horizon ray assertion is the imported premise specified in External input and the source record.

### Justification

**Given:** The objects and data of the Definition, with Countable Choice for the general construction and Dependent Choice for its stationary application.

**Goal:** Verify the curve and cross-section predicates and the horizon-portion identity, distinguishing the imported ray assertion.

1.1 Under Countable Choice, the supplied Lorentzian and metric-selected-connection interfaces apply to the general construction. By the along-curve derivative interface, $D_s\dot c$ is intrinsic, including at one-sided endpoints. Applying the coordinate-geodesic proposition to $\nabla^g$ gives exactly the displayed equation. The additional null and future predicates exclude constant curves. Maximal continuation within $H$ specifies the absence of a larger connected geodesic extension in $H$; defining this predicate asserts no existence. [F1, F2]

1.2 In the stationary application put $U=I_M^+(M_{\rm ext})$ and $P=I_M^-(M_{\rm ext})$, so $D=U\cap P$. For any $p\in U$, openness supplies a neighborhood $V\subset U$; on $V$ the sets $D$ and $P$ agree. Consequently $p\in\partial_M D$ if and only if $p\in\partial_M P$. Intersecting with $U$ gives $\mathcal E^+=H^+\cap U$, defining the required relationship without identifying the full horizon with its portion. [F3, F4]

2.1 Passing to images removes parametrization from the once-only condition: it is precisely $|B\cap G|=1$ for each specified generator image. Included endpoints are points of the image, so require no special multiplicity convention. No smooth horizon tangent bundle or existence of a section is needed to formulate this predicate. [F1, F2, step 1.1]

3.1 With the stated uniform timelikeness convention, the exterior data match the imported stationary causal-boundary premise, so its future rays are available on $H^+$. Restricting each such generator curve to maximal connected parameter pieces in $\mathcal E^+$ defines the portion convention; step 2.1 then supplies its once-only intersection predicate. The future-ray assertion is imported, not established by the terminology or by this local justification, and implies no affine completeness or smoothness of the horizon. [F1, F3, F5, step 2.1, step 1.2] ∎

### External input

The ray assertion [F5] is imported from Chruściel–Costa §4.1, opening paragraph; the exterior construction is §2.2. Its precise statement, hypotheses, locator and reading limits are in the source record. This local justification only applies that premise and verifies the definitions and the portion identity.


## Lipschitz height functions, cut measure and Jacobians

[Open item](item-def-lipschitz-cut-area-data) · level 3


### Definition

On a smooth Riemannian three-region $(\Sigma,k)$ a locally Lipschitz height $u$ has almost-everywhere chart derivatives, equal to weak derivatives; its metric gradient is defined almost everywhere by $k(\nabla u,\cdot)=du$. Cut area means normalized two-dimensional Hausdorff measure $\mathcal H_k^2$. The initial domain for an endpoint construction is a Borel subset $A$ of a smooth Riemannian surface $(C,h)$, not the possibly nonsmooth image $D$. For $F:A\to\Sigma$ with countably many local $C^1$ extensions, $J(F)$ means the nonnegative Gram Jacobian $J_2F$, and $N(F,A;y)$ counts the initial points arriving at $y$. The area formula is $\int_A J(F)\,d\mu_C=\int_{F(A)}N(F,A;y)\,d\mathcal H_k^2(y)$; therefore surjectivity $F(A)=D$ gives $|D|\le\int_A J(F)\,d\mu_C$. Coincident endpoints do not invalidate this inequality. The identity $|D|=\int_A J(F)\,d\mu_C$ holds if $N(F,A;y)=1$ for $\mathcal H_k^2$-almost every $y\in D$. If $\int_A J(F)\,d\mu_C<\infty$, this multiplicity-one condition is also necessary for equality. Equality with infinite common value need not imply multiplicity one. All measures use the same area normalization and the specified fixed metrics; $J(F)\le1$ is an additional geometric estimate, not part of the definition of Jacobian.

### Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Lipschitz differentiability, weak derivatives and graph calculus are supplied under Countable Choice by [math:lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice](https://alphabetamath.cc/item/lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice).

[F2] The Riemannian metric convention is [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold). Measurable initial domains, Gram Jacobians and counting multiplicity are defined in [def-author-0336834a2590-measurable-surface-domains](item-def-author-0336834a2590-measurable-surface-domains), [def-author-0336834a2590-surface-map-jacobian](item-def-author-0336834a2590-surface-map-jacobian) and [def-author-0336834a2590-endpoint-multiplicity](item-def-author-0336834a2590-endpoint-multiplicity).

[F3] Transverse hitting regularity is [lem-author-0336834a2590-transverse-endpoint-regularity](item-lem-author-0336834a2590-transverse-endpoint-regularity); the area formula with multiplicity and its image-area bound are [lem-author-0336834a2590-endpoint-area-with-multiplicity](item-lem-author-0336834a2590-endpoint-area-with-multiplicity).

[F4] The Lorentzian metric and nonzero null-vector conventions are [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects), the positive-definite tangent metric of a spacelike hypersurface is [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets), and the time-function convention is [physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity), clause (d). These are mathematical definitions; no physical postulate is used.

[F5] A nonempty regular fibre of a smooth scalar map is an embedded codimension-one submanifold. The proof supplies local projection coordinates for the map, hence identifies the tangent space of the fibre with the kernel of its differential. [math:thm-a-regular-level-set-is-an-embedded-submanifold](https://alphabetamath.cc/item/thm-a-regular-level-set-is-an-embedded-submanifold)

### Justification

Apply [F1] in coordinate charts to the height and use the smooth inverse metric to obtain its measurable weak gradient. The area and Jacobian conventions are exactly [F2], and the formula and inequality are [F3]. Multiplicity one almost everywhere suffices for equality by that formula. For necessity in the finite case, put $I=\int_A J(F)\,d\mu_C<\infty$ and suppose $|D|=I$. The measurable set $E=\{y\in D:N(F,A;y)\ge2\}$ satisfies $I=\int_D N(F,A;y)\,d\mathcal H_k^2(y)\ge |D|+\mathcal H_k^2(E)$. Subtracting the finite value $|D|=I$ gives $\mathcal H_k^2(E)=0$. This subtraction is unavailable for infinite common value. Indeed, take $A=C=\mathbb R^2\sqcup\mathbb R^2$ with its Euclidean component metrics and map each component isometrically onto the same plane $D$ in Euclidean $\Sigma=\mathbb R^3$. This map is smooth on both components, $J_2F=1$, $N=2$ everywhere on $D$, and both $|D|$ and $I$ are infinite.

For an endpoint family, [F3] supplies local extensions when the supplied $C^1$ family meets a slice $s=0$ transversely at its unique hit. For null generators of a smooth Lorentzian metric meeting a spacelike slice $\Sigma=s^{-1}(0)$, use a smooth defining function $s$ with $0$ a regular value, as required by [F3]. At a hit $p$, the regular-level coordinates of [F5] give $T_p\Sigma=\ker ds_p$. If the nonzero null tangent $\dot\gamma$ had $ds_p(\dot\gamma)=0$, it would belong to $T_p\Sigma$. Positive definiteness on that space would give $g_p(\dot\gamma,\dot\gamma)>0$, contradicting $g_p(\dot\gamma,\dot\gamma)=0$. Thus $ds_p(\dot\gamma)\ne0$, using precisely the conventions in [F4].

If the family is parametrized by a smooth chosen initial null normal and has smooth geodesic dependence on its open flow domain, it is such a supplied family; these are geometric inputs to be established by an application, not consequences of a Lipschitz height alone. When the defining function $s$ is also a time function, [F4] makes it strictly increasing along each future-oriented generator, and strictly decreasing with the opposite orientation. Either strict monotonicity makes a prescribed time-level hit unique.

A closed $A\subset C$ is Borel by [F2]. Thus an application must verify the smooth initial surface and chosen generator branch, open flow domain, unique transverse hits at a regular level, Borel domain and image coverage. It does not need to prove that $D$ is a smooth or Lipschitz surface. Focal degeneracy at endpoints is allowed as rank loss of the derivative. No inference of the required endpoint-map regularity is made merely from the statement that $D$ is a cut.


## Linear and path-independent normal-graph variation of expansion

[Open item](item-lem-author-c50357f4fa9e-linear-expansion-variation) · level 3


### Statement

Assume countable choice $\mathrm{AC}_\omega$. Let $\Sigma$ be a smooth spacelike hypersurface in a time-oriented smooth Lorentzian four-manifold $(M,g)$, let $h=g|_{T\Sigma}$, and let $S\subset\operatorname{int}\Sigma$ be a smooth embedded two-surface without boundary with a supplied smooth outward $h$-unit normal $\nu$. Use a supplied open normal-graph domain $\Omega$ containing the relevant zero section, on which $T(p,r)=\exp^h_p(r\nu_p)$ is a diffeomorphism onto its image. The domain may be local, with the graph constructions then restricted to its open base patch in $S$; a global graph uses such a domain over all of $S$. For compact $S$ a uniform tube exists, while no uniform tube is presumed for noncompact $S$. A smooth $u$ is admissible when its graph lies in $\Omega$, and $F_u(p)=T(p,u(p))$.

Use the canonical gauge of the second-graph-data construction: $n$ is the future unit normal to $\Sigma$, $\nu_u$ is the outward graph unit normal, $L_u=n|_{F_u(S)}+\nu_u$, and $\Theta(u)=F_u^*(\theta_{L_u})$ is the pulled-back outgoing expansion. For this gauge on admissible graphs, define $$\mathcal L\phi=\left.\frac{d}{d\epsilon}\right|_{\epsilon=0}\Theta(\epsilon\phi).$$ For compact $S$ this is defined for every $\phi\in C^\infty(S)$; on a noncompact surface the definition applies on a supplied tube to every $\phi$ admitting a common parameter interval of admissible graphs, in particular every compactly supported smooth $\phi$. Independently, the local formulas define the same differential operator on all smooth functions as a germ at each point. The operator is linear with smooth coefficients, of order at most two. Here **linear** means $\mathcal L(a\phi+b\psi)=a\mathcal L\phi+b\mathcal L\psi$ for real constants $a,b$ wherever the relevant graph paths are admissible.

If $u(t,p)$ is a jointly smooth admissible graph path with $u(0,p)=0$ and $\partial_tu(0,p)=\phi(p)$, then $\partial_t\Theta(u(t))|_0=\mathcal L\phi$. Thus the first derivative does not depend on the higher parameter behavior of the chosen graph path.

### Facts & Assumptions

[F1] Under the geometric and graph-domain hypotheses of the Statement and the countable-choice hypothesis in [F5], [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain) supplies a common parameter interval for each compactly supported direction in a supplied tube, and for every smooth direction when $S$ is compact.

[F2] For the stated normal-graph data and canonical gauge, [lem-author-c50357f4fa9e-expansion-second-jet](item-lem-author-c50357f4fa9e-expansion-second-jet) gives the smooth local expression $A(x,u,\partial u,\partial^2u)$ for pulled-back expansion.

[F3] [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps) gives the chain rule for this finite-dimensional smooth function.

[F4] [math:thm-clairaut-schwarz-mixed-partials](https://alphabetamath.cc/item/thm-clairaut-schwarz-mixed-partials) gives equality of mixed coordinate partial derivatives for a $C^2$ scalar function on an open Euclidean set. Joint smoothness makes this applicable to $u(t,x)$ and each spatial first derivative $\partial_bu(t,x)$.

[F5] Adopt countable choice $\mathrm{AC}_\omega$ in the sense of [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice). This meets the countable-choice requirements of the graph-domain and second-graph-data suppliers in [F1] and [F2]; their geometric and graph-domain hypotheses are those explicitly stated above. No stronger choice principle is assumed.

[F6] Under the geometric and graph-domain hypotheses of the Statement and the countable-choice assumption in [F5], [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge) supplies the smooth future unit normal $n$, the outward graph unit normal $\nu_u$ with $\nu_0=\nu$, and the smooth future null normal $L_u=n|_{F_u(S)}+\nu_u$ used in the Statement.

[F7] [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry) defines the outgoing expansion on each embedded spacelike graph by $\theta_{L_u}=\operatorname{tr}_{q_u}\chi_{L_u}$, where $q_u$ is the induced positive metric and $\chi_{L_u}(X,Y)=g(\nabla_XL_u,Y)$ for graph-tangent $X,Y$, with tangential extension independence. Its countable-choice convention is met by [F5]. The canonical gauge in [F6] supplies the future null partner $n|_{F_u(S)}-\nu_u$, which pairs with $L_u$ to $-2$, as required by this definition; this choice of partner leaves $L_u$ unchanged. No congruence or compactness assumption is needed for this surface expansion.

### Proof

**Given:** The geometric and normal-graph data of the Statement, the countable-choice hypothesis in [F5], and a smooth graph direction, with an admissible parameter interval whenever a global graph path is asserted.

**Goal:** Establish the linear differential expression and its path independence.

1.1 The geometric and graph-domain hypotheses in the Statement, together with the countable-choice assumption in [F5], meet the supplier requirements in [F1] and [F2]. At a fixed chart point, [F2] and [F3] give $$\mathcal L\phi=A_z(x,0,0,0)\phi+\sum_a A_{p_a}(x,0,0,0)\partial_a\phi+\sum_{a\le b} A_{B_{ab}}(x,0,0,0)\partial_a\partial_b\phi.$$ Here $z$ is the scalar value, $p_a$ the first partials and $B_{ab}$ the independent symmetric second-partial coordinates; these symbols denote coordinates of the smooth function $A$, not extra geometric fields. The coefficient functions are smooth. This formula is linear in $\phi$ and its derivatives. Chart formulas agree since they differentiate the same pulled-back geometric scalar; locally all sufficiently small graph parameters are admissible. It therefore defines a global differential operator on germs, without requiring a uniform tube on a noncompact surface. [F1, F2, F3, F5, given, algebra]

2.1 For a jointly smooth path $u(t,x)$, apply [F4] to $u$ and to each $\partial_bu$, all of which are $C^2$ on the open parameter-coordinate domain. Commuting the parameter derivative first with $\partial_a$ on $\partial_bu$ and then with $\partial_b$ on $u$ gives $\partial_t\partial_a u|_0=\partial_a\phi$ and $\partial_t\partial_a\partial_bu|_0=\partial_a\partial_b\phi$. Differentiating [F2] therefore gives precisely the expression in step 1.1. In the compact or compactly supported case [F1] supplies an actual interval for $u=t\phi$. For two such directions, their union of supports is compact; a common smaller interval handles each linear combination. If global admissibility is otherwise supplied, only that supplied interval is used. This proves the path statement and all asserted linearity without a claim of differentiability in an unspecified infinite-dimensional function-space norm. [F1, F2, F3, F4, F5, step 1.1, algebra] ∎


## Acausal hypersurface with compact core and finitely many ends

[Open item](item-def-author-310ff0f53b38-acausal-finite-end-section) · level 3


### Definition

Let $S\subset M$ be a connected spacelike embedded hypersurface containing a specified asymptotically flat end $S_{\rm ext}$ with the decay data of [def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end). Acausal means that no distinct points of $S$ are joined, in either direction, by a future causal curve in the ambient $M$. It is an additional global condition, not part of positive definiteness of the induced metric.

Use the completion data of [def-author-310ff0f53b38-closure-and-boundary-data](item-def-author-310ff0f53b38-closure-and-boundary-data): $\overline S^{\,M}$ is a topological three-manifold with manifold interior $S$ and boundary $B=\overline S^{\,M}\setminus S$, and $B$ is a topological two-manifold. A compact core with finitely many asymptotic ends means that $\overline S^{\,M}=C_0\cup S_1\cup\cdots\cup S_N$ for a compact subset $C_0$ and finitely many end regions $S_j$ with asymptotically flat end charts as above. The chosen end $S_{\rm ext}$ is one of the specified asymptotic regions, up to truncation at a larger radius. This is a finite-end condition, not compactness of $\overline S^{\,M}$.

For a specified future horizon portion $\mathcal E^+$, the boundary section condition means $B\subset\mathcal E^+$ and $|B\cap G|=1$ for every generator image $G$ of $\mathcal E^+$, in the sense of [def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section). It is a topological once-only cross-section condition; a smooth embedding or a transverse differentiable intersection is not added to it.

### Definition references

[def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end)

[def-author-310ff0f53b38-closure-and-boundary-data](item-def-author-310ff0f53b38-closure-and-boundary-data)

[def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section)

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

### Facts & Assumptions

[F1] End charts and decay, completion topology, and generator images have the stated interfaces. [def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end) [def-author-310ff0f53b38-closure-and-boundary-data](item-def-author-310ff0f53b38-closure-and-boundary-data) [def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section)

[F2] Spacelikeness and acausality have the ambient Lorentzian meanings. [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

### Justification

**Given:**The objects and specified data in the Definition.

**Goal:** Verify that the displayed conditions define unambiguous objects and predicates on these data.

1.1 The induced metric tests spacelikeness pointwise, while causal reachability tests acausality using curves in $M$. The completion and its manifold boundary are specified independently. The finite union condition then quantifies over a compact set, a finite integer and end charts of the already defined type. [F1, F2]

2.1 With those objects fixed, boundary inclusion and once-only intersection are the subset and cardinality predicates of the generator interface. Their conjunction with step 1.1 gives a definite section-data predicate. No existence, compactification by points at infinity, or smoothness theorem is inferred. [F1, F2, step 1.1] ∎



## Staticity, axisymmetry and black-hole regularity hypotheses

[Open item](item-def-black-hole-comparison-hypothesis-data) · level 4


### Definition

Let $(M,g,N)$ be a time-oriented smooth Lorentzian four-manifold, $T$ a specified Killing field and $S_{\rm ext}$ a specified asymptotically flat spacelike end. Here **stationary relative to the selected end** means that there is a specified sufficiently large end-chart radius $R_1$ such that $T$ is future timelike on the tail $r\ge R_1$. Restrict to that tail in the stationary-flow exterior construction and denote the selected restricted end again by $S_{\rm ext}$. The decay convention is that of the supplied asymptotically flat spacelike-end interface: for some $\alpha>0$ and integer $m\ge2$, $\gamma_{ij}-\delta_{ij}=O_m(r^{-\alpha})$ and $k_{ij}=O_{m-1}(r^{-1-\alpha})$. Completeness of $T$ means its flow is defined for every real time at every point of $M$, not only in the exterior. For complete $T$, form $M_{\rm ext}$, $D=I_M^+(M_{\rm ext})\cap I_M^-(M_{\rm ext})$ and $\mathcal E^+=\partial_M D\cap I_M^+(M_{\rm ext})$ by the supplied stationary-flow exterior interface. All these sets use the specified tail and the ambient chronology of $M$.

The triple $(M,g,T)$ is **$I^+$-regular in the Chruściel–Costa sense**, relative to this end, when $T$ is complete, $D$ is globally hyperbolic, and there exists in $D$ a spacelike connected acausal hypersurface $S\supset S_{\rm ext}$ whose closure $\overline S^{\,M}$ is a topological manifold with boundary consisting of a compact set and finitely many asymptotic ends. Its boundary $B:=\overline S^{\,M}\setminus S$ is a topological manifold, satisfies $B\subset\mathcal E^+$, and meets every generator of $\mathcal E^+$ precisely once. Use the supplied closure and boundary conventions, generator and cross-section conventions, and finite-end acausal-section data. Global hyperbolicity is computed for the Lorentzian domain $D$, with its own causal curves; acausality of $S$ is relative to the ambient $M$. No smoothness of the completed boundary or Killing generator for the event horizon is included in this definition.

On an open region where $T$ is timelike, **staticity** means hypersurface orthogonality: locally the hyperplanes $T^\perp=\{v:g(T,v)=0\}$ are tangent to spacelike hypersurfaces. Equivalently the Frobenius condition is $T^\flat\wedge dT^\flat=0$, where $T^\flat=g(T,\cdot)$, $d$ is the invariant exterior derivative, whose smooth-form well-definedness is supplied by the declared multilinearity lemma, and $\wedge$ is the wedge product. The equivalence is the cited external staticity criterion, not a global splitting theorem. The **ergoregion** is $\{p:g_p(T,T)>0\}$; points where $g(T,T)=0$ do not belong to it.

The **stationary axisymmetric comparison data** additionally specify a jointly smooth left action $a:S^1\times M\to M$ of the standard circle Lie group $S^1=\mathbb R/(2\pi\mathbb Z)$, written $\psi_s(p)=a([s],p)$, by isometries. Thus $\psi_0=\operatorname{id}_M$, $\psi_{s+t}=\psi_s\circ\psi_t$ and $\psi_{s+2\pi}=\psi_s$; effectiveness means that $\psi_s=\operatorname{id}_M$ implies $s\in2\pi\mathbb Z$. Its generator is $Z_p=\left.\frac{d}{ds}\right|_{s=0}\psi_s(p)$. Require $Z$ to commute with $T$: explicitly, the flow of $T$ and $\psi_s$ commute wherever both compositions are defined. The **axis** is the fixed-point set $A=\{p:\psi_s(p)=p\text{ for all }s\}$, required here to be a nonempty smooth two-dimensional submanifold. To specify a **regular axis**, require that $g$ extend smoothly and nondegenerately across $A$, that its normal two-plane $(T_pA)^{\perp_g}$ be spacelike at every $p\in A$, and that the differential $D_p\psi_s$ on that plane be the ordinary rotation through angle $s$ up to choice of orientation. This last normalization is weight one; it excludes a multiple rotation or a conical quotient at the axis. These axis conditions are explicit additional data, not a consequence of $I^+$-regularity.

**Analyticity** means a compatible real-analytic atlas in which the metric components are locally convergent real power series. **Horizon connectedness** means connectedness of the specified horizon subset (for example $\mathcal E^+$). For the following surface-gravity convention use the nonzero-generator portion of the supplied Killing-horizon interface: $H\subset M$ is a smooth embedded null hypersurface and $K$ is a specified smooth Killing field on a neighborhood of $H$, nonzero on $H$, tangent and normal to it, so $K_p\in T_pH$ and $g_p(K_p,X)=0$ for every $X\in T_pH$. Here null means that the metric restricted to $T_pH$ has a nonzero radical at every point. On this smooth Killing-horizon portion, **surface gravity** $\kappa$ is the unique smooth function satisfying $d(g(K,K))_p=-2\kappa(p)K^\flat_p$ for $p\in H$. This is an equality of ambient covectors in $T_p^*M$, not of their pullbacks to $T_pH$. It is **degenerate** if $\kappa$ vanishes identically and **nondegenerate** if $\kappa$ is nowhere zero on the component under consideration; if constancy is assumed or separately supplied this is just $\kappa=0$ versus $\kappa\ne0$. No sign, constancy or normalization-independent numerical value is asserted here. Analyticity, connectedness, and this Killing-horizon nondegeneracy are separate hypotheses; none follows by definition from $I^+$-regularity. The mean-nondegeneracy used in Chruściel–Costa Theorem 1.3 is not silently identified with an arbitrary event-horizon surface gravity.

### Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end)

[def-author-310ff0f53b38-stationary-flow-exterior](item-def-author-310ff0f53b38-stationary-flow-exterior)

[def-author-310ff0f53b38-closure-and-boundary-data](item-def-author-310ff0f53b38-closure-and-boundary-data)

[def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section)

[def-author-310ff0f53b38-acausal-finite-end-section](item-def-author-310ff0f53b38-acausal-finite-end-section)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula)

[math:def-wedge-product-of-differential-forms](https://alphabetamath.cc/item/def-wedge-product-of-differential-forms)

[math:def-smooth-left-action-of-a-lie-group](https://alphabetamath.cc/item/def-smooth-left-action-of-a-lie-group)

[math:lem-the-invariant-exterior-derivative-formula-is-c-infinity-multilinear](https://alphabetamath.cc/item/lem-the-invariant-exterior-derivative-formula-is-c-infinity-multilinear)

[physics:def-emg-causal-solution-and-horizon-vocabulary](https://alphabetamath.cc/physics/item/def-emg-causal-solution-and-horizon-vocabulary)

### Facts & Assumptions

[F1] End geometry, complete-flow exterior, completion boundary, generator images and finite-end sections have the five explicit interfaces. The exterior interface requires future timelikeness on the chosen sufficiently distant tail. Only the generator-image and once-only intersection conventions are used here; no causal-boundary ray-existence theorem is invoked. [def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end) [def-author-310ff0f53b38-stationary-flow-exterior](item-def-author-310ff0f53b38-stationary-flow-exterior) [def-author-310ff0f53b38-closure-and-boundary-data](item-def-author-310ff0f53b38-closure-and-boundary-data) [def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section) [def-author-310ff0f53b38-acausal-finite-end-section](item-def-author-310ff0f53b38-acausal-finite-end-section)

[F2] Lorentzian geometry, Killing fields, global hyperbolicity and the metric-selected connection use the named mathematical library interfaces. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field) [physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity) [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F3] Metric duality and differential-form operations are the supplied constructions. The invariant exterior-derivative formula defines a smooth form by its multilinearity lemma. [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms) [math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula) [math:lem-the-invariant-exterior-derivative-formula-is-c-infinity-multilinear](https://alphabetamath.cc/item/lem-the-invariant-exterior-derivative-formula-is-c-infinity-multilinear) [math:def-wedge-product-of-differential-forms](https://alphabetamath.cc/item/def-wedge-product-of-differential-forms)

[F4] The exact regularity definition, generator terminology, surface-gravity sign convention and local staticity criterion are the independent external inputs specified below. The action, its commutation with the stationary flow and the weight-one axis conditions are imposed data.

[F5] A smooth left action is jointly smooth and obeys the identity and composition laws, and its individual action maps are diffeomorphisms. [math:def-smooth-left-action-of-a-lie-group](https://alphabetamath.cc/item/def-smooth-left-action-of-a-lie-group)

[F6] Definition (b) and Proof 2.1 of the mathematical horizon interface give the unique smooth surface-gravity scalar on the nonzero tangent-and-normal Killing-generator part, with the equality interpreted as ambient covectors. Only this portion is used; its area, escape, extension and bifurcation clauses are not invoked. [physics:def-emg-causal-solution-and-horizon-vocabulary](https://alphabetamath.cc/physics/item/def-emg-causal-solution-and-horizon-vocabulary)

### Justification

**Given:** The objects and specified data in the Definition.

**Goal:** Verify that the displayed conditions define unambiguous objects and predicates on these data.

1.1 The supplied cutoff and future timelikeness satisfy the exterior interface's end hypothesis. For complete $T$ its flow-saturated region and ambient causal exterior are therefore defined. The five interfaces specify the end decay, topological completion and once-only generator intersections; conjoining those predicates with global hyperbolicity of $D$ gives the stated $I^+$-regularity condition. The compact-core condition retains its asymptotic ends, and the boundary condition uses $\mathcal E^+$ with its required $I_M^+(M_{\rm ext})$ factor. This uses no generator-existence or horizon-smoothness assertion. [F1, F2, F4]

1.2 Metric duality gives the smooth one-form $T^\flat$. The multilinearity lemma gives a smooth two-form $dT^\flat$, to which the wedge-product construction applies, yielding the well-defined three-form $T^\flat\wedge dT^\flat$. On the timelike region the covector is nonzero, so the cited staticity criterion applies to its orthogonal hyperplanes. The scalar $g(T,T)$ also determines the ergoregion by the strict inequality in the definition. [F2, F3, F4]

1.3 The jointly smooth circle action determines a smooth generator, fixed points and differentials at those points. Differentiating $\psi_{s+h}=\psi_h\circ\psi_s$ in $h$ at zero shows that $\psi_s$ is the flow of its generator $Z$; differentiating $\psi_s^*g=g$ at zero then gives $\mathcal L_Zg=0$. At $p\in A$ its differential is the identity on $T_pA$ because $\psi_s$ fixes $A$ pointwise, and preserves $(T_pA)^{\perp_g}$ because $\psi_s$ is an isometry. Thus the stated weight-one test is a predicate on its normal representation. The regular-axis and commutation conditions are specified data; no existence of an axial action is inferred. [F2, F5, given]

2.1 On the specified Killing-horizon portion the hypotheses of [F6] hold: the embedded hypersurface is null and its Killing field is nonzero, tangent and normal. That supplier therefore gives existence, uniqueness and smoothness of $\kappa$ in the ambient-covector equation, not just uniqueness conditional on existence. Analytic charts, connectedness and vanishing or nonvanishing of that scalar test the separate predicates in the Definition. These verifications establish no rigidity or uniqueness theorem, zeroth law or existence of a horizon-generating Killing field. [F2, F3, F4, F6, step 1.2, step 1.3] ∎

### External input

Chruściel–Costa Definition 1.1, (1.1), together with §§2.1–2.2, supplies the independent regularity, end-decay and exterior-definition inputs. Their §4.1 supplies generator and cross-section terminology, and §2.3, (2.11), fixes the surface-gravity sign convention. Chruściel–Costa–Heusler §3.1 supplies the local staticity equivalence; §3.2 supplies axial-field terminology, not a derivation of the specified effective action, commutation or regular-axis conditions. The declared mathematical action and horizon suppliers furnish the missing formulation and well-definedness interfaces. These are definition/criterion inputs with the hypotheses and reading limits recorded in the three source records; no uniqueness, generator-existence, horizon-smoothness or zeroth-law theorem is imported here as a locally established result.


## Boost dependence of expansion variation and the MOTS gauge

[Open item](item-lem-author-c50357f4fa9e-mots-boost-variation) · level 4


### Statement

Assume countable choice $\mathrm{AC}_\omega$. Let $S$ and its canonical graph gauge be as in the linear-expansion variation lemma. Let $u(t,p)$ be a jointly smooth admissible graph path on a common open parameter interval containing $0$, with $u(0,p)=0$. A **marginally outer trapped surface** (MOTS) here means $\theta_{L_0}=0$ identically on $S$ for the chosen outward future null ray. For any jointly smooth real $f(t,p)$ with $f(0,p)=0$, replace the normals along $F_{u(t)}$ by $\widehat L_t=e^{f(t,p)}L_{u(t)}$ and $\widehat{\underline L}_t=e^{-f(t,p)}\underline L_{u(t)}$. If $\dot u(0)=\phi$, their pulled-back expansion obeys
$$\left.\partial_t\widehat\Theta_t\right|_0=\mathcal L\phi+\dot f(0,\cdot)\theta_{L_0}.$$
Hence at a MOTS this variation is unchanged by every such smooth boost fixing the base normal. If the base scale changes by a smooth $f_0(p)$, the variation at a MOTS is instead multiplied by $e^{f_0}$; absolute equality is not asserted for different base scales. A smooth reparametrization of the graph by diffeomorphisms $\eta_t:S\to S$ with $\eta_0=\mathrm{id}$ adds $d\theta_{L_0}(\dot\eta_0)$, which is also zero at a MOTS.

### Facts & Assumptions

[F1] [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge) fixes the base normal $L_0=n+\nu$ and the graph gauge.

[F2] Under the geometric and graph-domain hypotheses inherited in the Statement and countable choice in [F6], [lem-author-c50357f4fa9e-linear-expansion-variation](item-lem-author-c50357f4fa9e-linear-expansion-variation) supplies the canonical variation $\mathcal L\phi$ for the stated jointly smooth admissible graph path with $u(0,p)=0$.

[F3] [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry) supplies the expansion trace and its boost scaling; [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps) supplies differentiation of smooth composites.

[F4] [math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold) supplies the connection product rule $\nabla_X(aY)=X(a)Y+a\nabla_XY$. The along-surface derivative convention in [F3] permits applying this rule to local ambient extensions.

[F5] [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds) defines the diffeomorphisms $\eta_t:S\to S$ used for reparametrization. The assumed smooth family means $(t,p)\mapsto\eta_t(p)$ is jointly smooth.

[F6] Adopt countable choice $\mathrm{AC}_\omega$ in the sense of [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice). It meets the inherited graph-construction requirements of [F2] and the smooth tangent-bundle and time-orientation conventions of [F3]. No stronger choice principle is assumed.

### Proof

**Given:** The geometric and graph-domain data of the Statement, countable choice in [F6], the jointly smooth admissible graph path with $u(0,p)=0$, and the smooth boost with specified base scale.

**Goal:** Establish the precise extent of gauge independence.

1.1 The path hypotheses and [F6] meet the requirements of [F2] and [F3]. For any graph-tangent $X,Y$, the product rule in [F4], applied through the along-surface convention in [F3], yields $g(\nabla_X(e^fL),Y)=e^fg(\nabla_XL,Y)+e^fX(f)g(L,Y)$. The last term is zero because $L$ is normal. Taking the surface trace gives $\widehat\Theta=e^f\Theta$; reciprocal scaling of the other normal preserves the pairing $-1$. Differentiating and using [F2] gives $\partial_t\widehat\Theta|_0=e^{f_0}(\mathcal L\phi+\dot f_0\theta_{L_0})$. Setting $f_0=0$ gives the displayed formula; setting $\theta_{L_0}=0$ gives both base-scale assertions. Without the MOTS condition, the additional term generally remains. [F1, F2, F3, F4, F6, given, algebra]

2.1 Pullback by the smooth diffeomorphism family in [F5] replaces the scalar by $\Theta_t(\eta_t(p))$. The chain rule differentiates this to $\partial_t\Theta_t|_0+d\theta_{L_0}(\dot\eta_0)$. A function identically zero has zero differential, so the second term vanishes at a MOTS. These computations establish gauge and parameterization independence only with the stated base-scale and smoothness hypotheses. [F2, F3, F5, step 1.1, algebra] ∎


## Surface measure, flux densities and null normal gauge

[Open item](item-def-surface-area-flux-and-null-variation-data) · level 5


### Definition

Work under $\mathrm{AC}_\omega$ for the normal-graph construction and chart-partition integration. Let $(M,g)$ be a smooth oriented, time-oriented Lorentzian four-manifold with signature $(-,+,+,+)$, let $\Sigma$ be a smooth spacelike hypersurface, and let $S\subset\operatorname{int}\Sigma$ be a smooth oriented embedded spacelike two-surface without boundary with a supplied smooth outward unit normal $\nu$ in $h=g|_{T\Sigma}$. The future unit normal of $\Sigma$ is $n$. The induced metric on $S$ is $q$, and $d\mu_q$ denotes its positive oriented area form (its associated positive density is used in unsigned area integrals). Define
$$L=n+\nu,\qquad \underline L=(n-\nu)/2,\qquad g(L,\underline L)=-1.$$
For $U\in TS$ set $\zeta(U)=-g(\underline L,\nabla_U L)$, where $\nabla$ is the spacetime metric connection. For any supplied smooth real two-form $F$ on $M$, its **magnetic and electric flux densities** are the unique smooth functions $b,e$ on $S$ specified by
$$F|_{TS}=b\,d\mu_q,\qquad (\star_gF)|_{TS}=e\,d\mu_q.$$
Let $V_q$ be the Radon Borel measure determined by the positive Riemannian density $|d\mu_q|$. Here integrable means absolutely integrable for $V_q$: $\int_S|f|\,dV_q<\infty$. When $b$ and $e$, respectively, are integrable, define their magnetic and electric fluxes by $\int_Sb\,dV_q$ and $\int_Se\,dV_q$. For compact $S$ this holds automatically, and these fluxes equal the oriented top-form integrals $\int_SF|_{TS}$ and $\int_S(\star_gF)|_{TS}$. For noncompact $S$, the same notation for an absolutely integrable top form is interpreted by the stated density integral. The orientation of $M$ fixes $\star_g$, and the supplied orientation of $S$ fixes the signs of $b,e$.

All surface derivatives use the Levi–Civita connection $D^q$ of $q$: $q(\operatorname{grad}_q f,X)=df(X)$, $\operatorname{div}_q X=\operatorname{tr}(Y\mapsto D^q_YX)$, and $\Delta_q f=\operatorname{div}_q\operatorname{grad}_q f$. On one-forms, divergence means divergence of the $q$-dual vector field. The **Gauss curvature** is $K_q=q(R^q(e_1,e_2)e_2,e_1)$ for a $q$-orthonormal frame, with $R^q(X,Y)Z=D^q_XD^q_YZ-D^q_YD^q_XZ-D^q_{[X,Y]}Z$; this is the positive-round-sphere convention.

Fix an admissible outward normal-graph tube $T(p,r)=\exp^h_p(r\nu_p)$ as in the graph-domain lemma; on compact $S$ such a uniform tube exists. For every admissible $u$, let $F_u(p)=T(p,u(p))$, let $\nu_u$ be the outward graph unit normal and set $L_u=n|_{F_u(S)}+\nu_u$. Let $\Theta(u)=F_u^*(\theta_{L_u})$, where $\theta_{L_u}=\operatorname{tr}_{q_u}g(\nabla L_u,\cdot)$ is the outgoing expansion and $q_u=F_u^*h$. Define the **normal-graph expansion linearization** by
$$\mathcal L\phi=\left.\frac{d}{d\epsilon}\right|_0\Theta(\epsilon\phi).$$
For closed $S$ (compact without boundary) this acts on every smooth function. On a noncompact $S$ a global variation needs an actual common admissible parameter interval; compactly supported directions in a supplied tube suffice, while the local differential expression is defined on all smooth germs. When $\theta_L=0$ identically, $S$ is a MOTS and $\mathcal L$ in this fixed gauge is called its **outward stability operator in $\Sigma$**. It is a linear differential operator of order at most two. Smooth boosts fixing the base $L$ do not change this variation at a MOTS; changing its base positive scale multiplies it by that scale. The explicit curvature and matter coefficient formula is a separate first-variation result, not part of this definition.

### Facts & Assumptions

[F1] [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form) supplies $h,n$ and the spacetime derivative along $\Sigma$. [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry) supplies null expansion and normal-frame scaling.

[F2] [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus) supplies the smooth Lorentzian Hodge star on the oriented spacetime; [math:def-riemannian-volume-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-riemannian-volume-form-on-an-oriented-manifold) supplies the nowhere-zero oriented area form of $q$.

[F3] [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry) supplies the unique intrinsic surface connection; [math:def-riemann-curvature-four-tensor](https://alphabetamath.cc/item/def-riemann-curvature-four-tensor) fixes the curvature four-tensor convention used for $K_q$.

[F4] [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain) establishes the graph domain, including its compactness qualifications; [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge) establishes the smooth outward graph normal and null gauge.

[F5] [lem-author-c50357f4fa9e-expansion-second-jet](item-lem-author-c50357f4fa9e-expansion-second-jet) gives the local second-data expression, [lem-author-c50357f4fa9e-linear-expansion-variation](item-lem-author-c50357f4fa9e-linear-expansion-variation) establishes its linear, path-independent derivative, and [lem-author-c50357f4fa9e-mots-boost-variation](item-lem-author-c50357f4fa9e-mots-boost-variation) gives the exact MOTS boost and reparametrization qualifications.

[F6] [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) records the assumed $\mathrm{AC}_\omega$. Under that assumption, [math:def-integral-of-a-compactly-supported-top-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-top-form-on-an-oriented-manifold) defines the integral of a smooth compactly supported top form using chart partitions.

[F7] [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density) supplies the compact-finite Radon Borel measure $V_q$ of $|d\mu_q|$. [math:def-integrable-real-and-complex-functions-and-their-integrals](https://alphabetamath.cc/item/def-integrable-real-and-complex-functions-and-their-integrals) defines absolute integrability and the signed integral. [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration) gives the absolutely convergent chart formula for $L^1(V_q)$ functions and its agreement with smooth compact-support density integration.

### Justification

The orthogonality and normalization in [F1] give the displayed null pairing, as also calculated in [F4]. Covariant derivatives in directions tangent to $S$ are independent of any ambient extensions by [F1], so $\zeta$ is a smooth one-form. By [F2], every smooth two-form on the oriented two-dimensional $S$ is a unique scalar multiple of $d\mu_q$: in a positive chart the scalar is its coefficient divided by $\sqrt{\det q}$. The nonzero denominator proves existence, uniqueness and smoothness of $b,e$; the top-form transformation law makes these ratios agree on overlaps. The positive density $|d\mu_q|$ gives $V_q$ by [F7], and smooth $b,e$ are Borel functions. Absolute integrability in [F7] defines each finite signed flux even on a noncompact $S$. If $S$ is compact, every smooth function on $S$ has compact support, so the smooth compact-support comparison in [F7] proves its integrability. In a positive chart, the coefficient of $f\,d\mu_q$ and that of the signed density $f|d\mu_q|$ are both $f\sqrt{\det q}$. Their partition-weighted chart integrals therefore coincide by [F6] and [F7]. Taking $f=b,e$ proves the two compact oriented-flux equalities; on noncompact $S$, the $L^1$ chart formula in [F7] gives the declared absolutely convergent extension. Countable choice is used in the inherited chart-partition integration constructions of [F6] and [F7]. The intrinsic connection and tensorial contractions in [F3] define the displayed gradient, divergence and Laplacian independently of coordinates. The curvature definition is antisymmetric in its first two slots. Applying metric compatibility to the commutator $D^q_XD^q_Y-D^q_YD^q_X-D^q_{[X,Y]}$ acting on $q(Z,W)$ gives $q(R^q(X,Y)Z,W)+q(Z,R^q(X,Y)W)=0$, proving antisymmetry in the final two slots. Under a change of orthonormal frame, these two antisymmetries make the displayed value multiply by the square of the frame determinant, which is one in dimension two. Thus $K_q$ is well defined even under an orientation-reversing frame change. Finally [F4] gives actual admissible graph domains and a smooth fixed gauge, and [F5] proves well-definedness, linearity, path independence and the stated restrictions on boost invariance of the derivative. No Einstein equation, compactness without explicit mention, geodesic completeness or arbitrary parameter-dependent null normalization is presumed.

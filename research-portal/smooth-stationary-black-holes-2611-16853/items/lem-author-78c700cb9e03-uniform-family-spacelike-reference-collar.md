---
id: lem-author-78c700cb9e03-uniform-family-spacelike-reference-collar
title: Compact metric families have a common spacelike collar with fixed boost rate
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - def-spacelike-maximal-hypersurface-data
  - physics:def-gr-metric-selected-connection
  - math:prop-coordinate-geodesic-equation
  - math:thm-smooth-dependence-of-ode-solutions-on-parameters
  - math:thm-parametrized-implicit-function-theorem-with-higher-regularity
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:def-axiom-of-choice
  - math:def-domain-and-exponential-map-of-a-connection
  - math:def-riemannian-gradient
  - math:def-smooth-collar-of-a-manifold-boundary
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  math:prop-coordinate-geodesic-equation: mathematical-premise
  math:thm-smooth-dependence-of-ode-solutions-on-parameters: mathematical-premise
  math:thm-parametrized-implicit-function-theorem-with-higher-regularity: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-domain-and-exponential-map-of-a-connection: mathematical-premise
  math:def-riemannian-gradient: mathematical-premise
  math:def-smooth-collar-of-a-manifold-boundary: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Let $g_q$, $q\in[0,1]$, be a jointly smooth family of Lorentz metrics of signature $(-,+,+,+)$ on a common neighborhood of a compact embedded two-sphere $S$ in a smooth embedded hypersurface $\widehat\Sigma$ without boundary. Specify a smooth submanifold with boundary $\Sigma_+\subset\widehat\Sigma$ near $S$, with $\partial\Sigma_+=S$, selecting one side of $S$. Suppose $g_q|_{T\widehat\Sigma}$ is positive definite at $S$ for every $q$. Supply a jointly smooth field $N_q$ on the common neighborhood with $g_q(N_q,N_q)<0$; it specifies the future cone for every $q$. All parameter smoothness includes the endpoints.

Let $K$ be a fixed smooth field, zero on $S$ and Killing for every $g_q$. At $p\in S$ put $B_pv=(\nabla^{(q)}_vK)_p$; since $K_p=0$, this derivative is independent of the connection. Suppose $B_p$ kills $T_pS$ and induces eigenvalues $\pm\kappa$ on $T_pM/T_pS$, for the same fixed $\kappa>0$ at every $p$. Let $\bar n_q$ be the future unit normal to $\widehat\Sigma$ at $S$, and let $\bar\nu_q$ be the unit normal to $S$ within $\widehat\Sigma$ pointing into $\Sigma_+$. Assume positivity at $q=1$ in this specified basis: $B_p\bar\nu_1=\kappa\bar n_1$ for every $p\in S$. Thus the spatial direction in the positive boost convention points into the selected side; the outward boundary normal of $\Sigma_+$ is its negative.

Then there is a common one-sided collar $V\subset\Sigma_+$, including $S$, which is spacelike for every $q$. Its induced metrics $\bar h_q$ and future unit normals $\bar n_q$ are jointly smooth. For some common $\epsilon>0$, the inward boundary normal exponential maps $E_q(p,r)=\exp^{\bar h_q}_p(r\bar\nu_q)$ are embeddings for $0\le r<2\epsilon$, with image in $V$. Their images for $0\le r<\epsilon$ contain a common smaller collar $W$ of $S$, with compact closure in $V$. On $W$ their inverse radial coordinate is $\rho_q=d_{\bar h_q,V}(\cdot,S)$, the intrinsic distance to $S$ using curves in $V$. Extend $\bar\nu_q$ there as the radial unit field $\nabla^{\bar h_q}\rho_q$. The metrics, normals, exponential maps and inverse normal coordinates have uniform bounds of every fixed finite order on compact smaller coordinate domains and a fixed compact smaller collar, in fixed finite charts.

On $S$, $\nabla^{(q)}_{\bar\nu_q}K=\kappa\bar n_q$. Uniformly on $W$ as $\rho_q\downarrow0$, $K=\kappa\rho_q\bar n_q+O(\rho_q^2)$ and $g_q(K,K)=-\kappa^2\rho_q^2+O(\rho_q^3)$. In particular, after a common shrinking, $K$ is future timelike on $W\setminus S$ for every $q$. The bounds and remainders are uniform in $q$ and the boundary point; no conclusion about the opposite side of $S$ is asserted.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-bifurcate-killing-horizon-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[physics:def-gr-metric-selected-connection]]

[[math:prop-coordinate-geodesic-equation]]

[[math:thm-smooth-dependence-of-ode-solutions-on-parameters]]

[[math:thm-parametrized-implicit-function-theorem-with-higher-regularity]]

[[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[[math:def-axiom-of-choice]]

[[math:def-domain-and-exponential-map-of-a-connection]]

[[math:def-riemannian-gradient]]

[[math:def-smooth-collar-of-a-manifold-boundary]]

## Facts & Assumptions

[F1] Smooth Lorentzian metrics, the local-flow definition of a Killing field, signed boost normalization, induced positive metrics, future unit normals and the manifold-with-boundary and intrinsic-distance conventions are as specified in these mathematical interfaces. The selected side and the jointly smooth future field are additional explicit hypotheses here. [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]] [[def-spacelike-maximal-hypersurface-data]]

[F2] A metric-selected connection is torsion-free and metric compatible, and its coordinate connection term in $\nabla_vK$ is linear in $K$. We derive skewness at $K=0$ below directly from the local-flow definition, rather than assume an already positive boost matrix. [[physics:def-gr-metric-selected-connection]] [[def-stationary-lorentzian-data]]

[F3] The coordinate geodesic equation and smooth ODE dependence give local normal exponential maps for the smooth positive induced metric family. The inverse and parametrized implicit function theorems apply in charts, including the parameter $q$; at parameter and radial endpoints use smooth extensions in the extended hypersurface. [[math:prop-coordinate-geodesic-equation]] [[math:thm-smooth-dependence-of-ode-solutions-on-parameters]] [[math:thm-parametrized-implicit-function-theorem-with-higher-regularity]] [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[F4] On the boundaryless spacelike open neighborhood $U\subset\widehat\Sigma$ used below, the exponential map of the induced connection is $\exp^{\bar h_q}_p(v)=\gamma_{p,v}(1)$ whenever the geodesic with initial velocity $v$ is defined at time $1$. Only sufficiently small initial vectors are used; no completeness is assumed. The Riemannian gradient is the metric dual of the differential: $\operatorname{grad}_{\bar h_q}f=(df)^{\sharp_{\bar h_q}}$, equivalently $\bar h_q(\operatorname{grad}_{\bar h_q}f,X)=df(X)$. We write $\nabla^{\bar h_q}f$ for this gradient, and boundary values are restrictions of the smooth signed-coordinate extensions on $U$. [[math:def-domain-and-exponential-map-of-a-connection]] [[math:def-riemannian-gradient]]

[F5] A smooth collar of the boundary $S=\partial\Sigma_+$ is a smooth embedding $c:S\times[0,a)\to\Sigma_+$, for some $a>0$, with $c(p,0)=p$ and image an open neighborhood of $S$ in $\Sigma_+$. We call its image a collar as well. [[math:def-smooth-collar-of-a-manifold-boundary]]

[A1] Work in ZFC with the inherited smooth-manifold conventions. No additional arbitrary family selection occurs in the compact finite-chart, normalization or uniquely determined ODE constructions below. [[math:def-axiom-of-choice]]

## Proof

**Given:** The metric family, selected side, smooth future field, fixed Killing field and boost hypotheses in the Statement.

**Goal:** Establish a common one-sided spacelike collar, uniform normal coordinates and the signed uniform expansions.

1.1 Positive definiteness is open and uniform on the compact set $[0,1]\times S$, so a common neighborhood $U$ in $\widehat\Sigma$ is spacelike; restrict to a relatively compact one-sided neighborhood in $U\cap\Sigma_+$. To construct the future normal, project $N_q$ orthogonally onto $T\widehat\Sigma$ using the inverse positive induced matrix, subtract this projection, and normalize the remaining timelike vector. This remainder has negative pairing with $N_q$, so normalization selects the stipulated future normal smoothly in $q$ and position. At $S$, local boundary defining functions increasing into $\Sigma_+$ give $\bar\nu_q$ by normalizing their induced gradients; on overlaps these give the same inward unit vector. These operations are smooth, and compactness bounds every fixed finite order in fixed finite charts. [given, F1, F4, A1]

1.2 At $p\in S$, the coordinate formula $(\nabla^{(q)}_vK)^a=v^b\partial_bK^a+\Gamma^a{}_{bc}v^bK^c$ reduces to $v^b\partial_bK^a$. Thus $B_p$ is connection independent. To derive skewness, differentiate the coordinate pullback formula $(\Phi_t^*g_q)_{ab}(x)=g_{q,cd}(\Phi_t(x))\partial_a\Phi_t^c(x)\partial_b\Phi_t^d(x)$ at $t=0$. The flow has $\partial_t\Phi_t|_{t=0}=K$ and $\partial_t\partial_a\Phi_t^c|_{t=0}=\partial_aK^c$, giving $0=(\mathcal L_Kg_q)_{ab}=K^c\partial_cg_{q,ab}+g_{q,cb}\partial_aK^c+g_{q,ac}\partial_bK^c$. Since $K_p=0$, this says exactly $g_q(B_pu,v)+g_q(u,B_pv)=0$ at $p$. As $B_p$ kills $T_pS$, it consequently preserves $(T_pS)^{\perp_{g_q}}$. This derives the needed skewness without using a lemma whose hypothesis already assumes a positive boost matrix. [given, F1, F2]

2.1 The induced connection has Christoffel coefficients $\bar\Gamma^k{}_{ij}=\tfrac12\bar h_q^{k\ell}(\partial_i\bar h_{q,j\ell}+\partial_j\bar h_{q,i\ell}-\partial_\ell\bar h_{q,ij})$, which are smooth jointly in $q$ and position. Direct substitution verifies metric compatibility and torsion freedom. Apply the coordinate geodesic equation and smooth ODE dependence to initial data $(p,\bar\nu_q(p))$ to obtain jointly smooth $E_q(p,r)$ on a common short interval, first in $\widehat\Sigma$ for signed $r$. The map $(q,p,r)\mapsto(q,E_q(p,r))$ has invertible differential at $(q,p,0)$: its spatial differential is $(X,a)\mapsto X+a\bar\nu_q(p)$. The inverse theorems therefore give smooth local inverses including $q$. Compactness gives a common small radius with nonsingular differential. It also gives injectivity for each $q$ at one common radius: otherwise distinct colliding data with radii tending to zero have a subsequence with $q\to q_0$ and base points converging; continuity forces both base limits to be the same point of $S$, contradicting the one local inverse there. For small positive radii the inward initial derivative puts the curves in $\Sigma_+$, and compactness makes this uniform. A small $q=0$ normal tube now provides a common one-sided collar $V$ with compact closure in $U\cap\Sigma_+$. Choose $2\epsilon$ within the common radius, small enough that all the $E_q$ images for $0\le r\le2\epsilon$ lie in $V$. The parameterized inverse neighborhoods of the compact set $[0,1]\times S$ contain $[0,1]\times W$ for a common smaller collar $W$, chosen as a still smaller $q=0$ normal tube with compact closure in $V$; shrink it so all its inverse radii are less than $\epsilon$. Both $q=0$ tubes are smooth collars in the sense of [F5]: the restricted maps $c(p,r)=E_0(p,r)$ are embeddings with $c(p,0)=p$, and the signed local inverses identify their half-tube images with open neighborhoods of $S$ in $\Sigma_+$. Smoothness and compactness also give the asserted fixed-order bounds for the exponential maps and their inverses. [F1, F3, F4, F5, step 1.1]

2.2 At $p\in S$, the pair $(\bar n_q,\bar\nu_q)$ is an orthonormal basis of $(T_pS)^{\perp_{g_q}}$, with metric matrix $\operatorname{diag}(-1,1)$. Skewness from step 1.2 forces $B_p\bar\nu_q=a(q,p)\bar n_q$ and $B_p\bar n_q=a(q,p)\bar\nu_q$. This normal plane identifies with $T_pM/T_pS$, so the eigenvalue hypothesis gives $a(q,p)^2=\kappa^2$. The normals depend smoothly on $q$, hence $a(q,p)$ is continuous. For each fixed $p$ it cannot change sign on $[0,1]$; the stated inward-basis positivity gives $a(1,p)=\kappa$, so $a(q,p)=\kappa$ throughout. In particular $\nabla^{(q)}_{\bar\nu_q}K=\kappa\bar n_q$ on $S$, with the inward, not the outward boundary normal of $\Sigma_+$. [given, F1, step 1.1, step 1.2]

3.1 Write $D$ for the induced connection just constructed. Along a normal geodesic let $\dot\gamma=\partial_rE_q$ and let $J$ be a variation in its base point. Metric compatibility and the geodesic equation give $\bar h_q(\dot\gamma,\dot\gamma)=1$. Torsion freedom and the commuting variation parameters give $D_{\dot\gamma}J=D_J\dot\gamma$, so $\frac{d}{dr}\bar h_q(\dot\gamma,J)=\bar h_q(\dot\gamma,D_J\dot\gamma)=\tfrac12J\bar h_q(\dot\gamma,\dot\gamma)=0$. Its initial value is zero because $\bar\nu_q\perp TS$. Thus the pulled-back metric is $dr^2+h_{q,r}$. Every curve from $S$ staying in this normal tube has length at least its terminal radius. A curve in $V$ that exits the radius-$2\epsilon$ tube must first reach that radius, costing at least $2\epsilon$; compactness of $S$ and the embedding on the closed smaller tubes exclude other exit points. For points of $W$, whose radius is less than $\epsilon$, such an exit cannot improve on the radial geodesic of length $r$. This proves $r=d_{\bar h_q,V}(\cdot,S)$ on $W$, and $\nabla^{\bar h_q}\rho_q=\partial_rE_q$ is the desired smooth extension of the inward boundary normal, with the stated uniform bounds. [F1, F4, step 2.1]

4.1 In fixed ambient charts along the geodesics of step 2.1, Taylor expansion of $K$, with $K|_S=0$ and initial derivative from step 2.2, gives $K=\kappa r\bar n_q|_{r=0}+O(r^2)$ in coordinate components. Smoothness replaces the base normal by the normal at the endpoint at a cost $O(r^2)$, so $K=\kappa\rho_q\bar n_q+O(\rho_q^2)$ as a field at that point. Smoothness on compact parameter and coordinate domains makes the remainder uniform. Using $g_q(\bar n_q,\bar n_q)=-1$ and uniformly bounded metric components gives $g_q(K,K)=-\kappa^2\rho_q^2+O(\rho_q^3)$ and $g_q(K,\bar n_q)=-\kappa\rho_q+O(\rho_q^2)$. Since $\kappa>0$, a common shrinking makes the first expression negative and the second negative for $\rho_q>0$. Thus $K$ is timelike and future directed on the selected punctured collar, with all claimed uniformity. [F1, step 1.1, step 2.1, step 3.1, step 2.2] ∎

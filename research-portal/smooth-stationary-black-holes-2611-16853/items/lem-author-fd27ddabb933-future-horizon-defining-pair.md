---
id: lem-author-fd27ddabb933-future-horizon-defining-pair
title: A bifurcate future horizon has an oriented defining pair near its section
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - lem-author-ca4ffba327b3-compact-normal-exponential-tube
  - def-bifurcate-killing-horizon-data
  - def-spacelike-maximal-hypersurface-data
  - physics:thm-gr-local-geodesics-and-exponential-map
  - math:def-axiom-of-choice
  - physics:def-gr-metric-selected-connection
  - math:def-embedded-submanifold-and-slice-chart
  - math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves
  - math:thm-smooth-inverse-function-theorem-on-manifolds
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  lem-author-ca4ffba327b3-compact-normal-exponential-tube: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Work in ZFC. Let $S$ be a compact embedded spacelike two-surface in a smooth time-oriented Lorentzian four-manifold $(M,g,N)$ without boundary, of signature $(-,+,+,+)$ and with its Levi–Civita connection. Let $H_f,H_p$ be smooth embedded null hypersurfaces through $S$, intersecting precisely in $S$ near $S$, with $T_sH_f\cap T_sH_p=T_sS$. A specified smooth embedded spacelike section side $\Sigma_+$ has boundary $S$ and is spacelike up to its boundary. Write $h=g|_{T\Sigma_+}$ and let $n$ be its future unit normal. Let $\nu$ be the unit vector tangent to $\Sigma_+$, orthogonal to $TS$, and pointing from $S$ into $\Sigma_+$. We call this the outward direction from $S$ toward the exterior; it is the inward boundary direction of the manifold-with-boundary $\Sigma_+$.

The supplied exterior wedge $\mathcal E$ means, locally near $S$, the open sector between the two null sheets into which the interior of $\Sigma_+$ enters. The future/outgoing label is explicit data: the radical line of $TH_f$ at $S$ is $\mathbb R(n+\nu)$. Write $H_f^+$ for its half-sheet reached from $S$ along future radical curves, and $H_p^-$ for the half-sheet of the other sheet reached along past radical curves. These labels are relative to the supplied exterior, not a claim that every null hypersurface is an event horizon; no Killing field or field equation is required.

For some $\epsilon>0$, the normal exponential map $\Xi(y,u,v)=\exp_y(u n_y+v\nu_y)$ is a diffeomorphism on $S\times\{(u,v):|u|+|v|<\epsilon\}$ onto a neighborhood $O$ of $S$, and $(\partial_u,\partial_v)=(n,\nu)$ on $S$. Put $a=v-u$ and $b=v+u$. After shrinking this tube, $\mathcal E\cap O=\{a>0,b>0\}$ and $H_f^+\cap O=\{a=0,b>0\}$; the past outward half-sheet is $H_p^-\cap O=\{b=0,a>0\}$. On $S$, $da(n-\nu)=-2$ and $db(n-\nu)=0$.

## Facts & Assumptions

[F1] A compact spacelike framed surface has a smooth normal exponential tube. For a smooth spacelike section side with boundary, the same supplier constructs its future unit normal and its unit boundary normal pointing into the side. [[lem-author-ca4ffba327b3-compact-normal-exponential-tube]]

[F2] The null-hypersurface convention identifies the radical line, and generators mean integral curves of this line. The specified transverse sheets meet along a spacelike surface. Exterior-sector and outward labels are the additional data in the Statement, not conclusions of this definition. [[def-bifurcate-killing-horizon-data]]

[F3] A smooth spacelike section has a positive-definite induced metric and a smooth future unit normal. Its separate boundary convention uses a smooth embedded manifold-with-boundary structure and positive definiteness up to the boundary. [[def-spacelike-maximal-hypersurface-data]]

[F4] Null geodesics with prescribed initial data are unique and depend smoothly on those data; exponential evaluation obeys the geodesic scaling law. [[physics:thm-gr-local-geodesics-and-exponential-map]]

[F5] The Levi–Civita connection is metric compatible and torsion free: $Xg(Y,Z)=g(\nabla_XY,Z)+g(Y,\nabla_XZ)$ and $\nabla_XY-\nabla_YX=[X,Y]$. [[physics:def-gr-metric-selected-connection]]

[F6] A smooth embedded hypersurface has slice charts, so locally it is $f=0$ with $df\ne0$ and tangent spaces $\ker df$. [[math:def-embedded-submanifold-and-slice-chart]]

[F7] A smooth tangent vector field on a manifold has unique local integral curves with smooth dependence on the initial point. We apply this on open subsets of the smooth null sheets, including across their common section. [[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]]

[F8] A smooth map with invertible differential at a point is a diffeomorphism between neighborhoods of that point and its image. [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[A1] Work in ZFC, including the Choice assumption inherited from the normal-tube and smooth-manifold suppliers. The compactness arguments below use finite covers; the tube supplier also uses countable selections in its injectivity argument. [[math:def-axiom-of-choice]]

## Proof

**Given:** The data, sector convention and orientation hypotheses in the Statement.

**Goal:** Construct the oriented defining pair and identify the two local boundary half-sheets.

1.1 In a boundary chart of $\Sigma_+$ take $\rho\ge0$, with $S=\{\rho=0\}$ and $d\rho\ne0$ there. Let $q$ be the vector satisfying $h(q,V)=d\rho(V)$, obtained from the inverse positive-definite Gram matrix of $h$. Then $q$ is smooth, nonzero, orthogonal to $TS$, and $d\rho(q)=h(q,q)>0$. Thus $\nu=q/\sqrt{h(q,q)}$ points into the specified section side. On overlaps these vectors agree, since a positive-definite three-space has exactly one unit vector orthogonal to $TS$ with the prescribed side. This is precisely the boundary-normal construction of [F1]. Together with the future unit normal $n$ it gives a smooth orthonormal frame of the normal plane of $S$. Apply [F1] to obtain $\Xi$ and its uniform tube. The frame differential at $S$ is $(X,u,v)\mapsto X+un+v\nu$. [F1, F3, A1, given, construct, algebra]

1.2 Fix either sheet $H$ and a slice function $f$ from [F6]. Nondegeneracy gives a unique nonzero field $L$ defined by $g(L,\cdot)=df$; its components are smooth by the inverse-matrix adjugate formula. The orthogonal complement of $TH=\ker df$ is the line spanned by $L$. Nullness means that this line is contained in $TH$, so it is its radical. For any smooth field $X$ tangent to $H$, the bracket $[L,X]$ is tangent along $H$: applying it to $f$ gives zero there, since both fields differentiate functions vanishing on $H$ to zero along $H$. Metric compatibility and torsion freedom therefore give, on $H$, $g(\nabla_LL,X)=-g(L,\nabla_LX)=-g(L,\nabla_XL+[L,X])=-\tfrac12 Xg(L,L)=0$. Here $g(L,X)$ and $g(L,L)$ vanish on $H$, so their tangential derivatives vanish. Hence $\nabla_LL=\kappa L$ on $H$, with $\kappa$ smooth locally, by division by a nonzero component of $L$. This proves pregeodesicity without any event-boundary hypothesis. [F2, F5, F6, algebra]

2.1 Choose the sign of $f$ so that $L$ is future directed, and take its local integral curve $\gamma(r)$ in $H$ through $s\in S$, using [F7]. Given a desired initial vector $\ell_s=cL_s$ with $c>0$, set $q(r)=c\exp(-\int_0^r\kappa(\gamma(\sigma))\,d\sigma)$ and $t(r)=\int_0^r q(\sigma)^{-1}\,d\sigma$. Since $dt/dr=1/q>0$, this is a smooth local reparameterization. For $\alpha(t(r))=\gamma(r)$ one has $\alpha^{\prime}=qL$ and $\nabla_{\alpha^{\prime}}\alpha^{\prime}=(q^2\kappa+q\,dq/dr)L=0$, with initial tangent $\ell_s$. Thus the affine geodesic with this initial tangent stays in $H$ locally. Uniqueness and scaling in [F4] identify it with $t\mapsto\exp_s(t\ell_s)$. Negative $t$ gives the past half of the same local generator. [F4, F7, F8, step 1.2, construct, algebra]

3.1 At $s\in S$ the radical of either sheet is normal to $T_sS$, hence lies in the plane spanned by $(n,\nu)$. A vector $un+v\nu$ is null exactly when $v=\pm u$. The two radical lines are distinct: otherwise that null line would lie in $T_sH_f\cap T_sH_p=T_sS$, contrary to spacelikeness. By the supplied future/outgoing label they are respectively $\mathbb R(n+\nu)$ and $\mathbb R(n-\nu)$. Step 2.1 identifies the maps $E_f(s,t)=\exp_s(t(n+\nu))$ and $E_p(s,t)=\exp_s(t(n-\nu))$ with maps into the respective sheets for small $t$ near each $s$. Their differentials at $(s,0)$ are $(X,r)\mapsto X+r(n\pm\nu)$, isomorphisms onto the sheet tangent spaces because a nonzero null vector cannot lie in $TS$. By [F8] their images contain sheet neighborhoods of $s$. In the injective tube coordinates these images are exactly $u=v$ and $u=-v$, respectively. The sheet neighborhoods, with the subspace topology from [F6], give ambient neighborhoods on which there are no other sheet pieces. Taking a finite cover of compact $S$ and shrinking the uniform tube makes these identities hold throughout $O$: the preimage under $\Xi$ of their union is open and contains $S\times\{(0,0)\}$, so a finite product-neighborhood cover of $S$ supplies a common positive radius. [F1, F2, F4, F6, F8, step 1.1, step 2.1, given, algebra]

4.1 The positive $t$ half of $E_f$ is $u=v>0$, and the negative $t$ half of $E_p$ is $u=-v<0$. The section-side direction is $\nu$, whose coordinates at $S$ have $du(\nu)=0$ and $dv(\nu)=1$. In any boundary chart a vector pointing into $\Sigma_+$ is a positive multiple of $\nu$ modulo $TS$; consequently both $a$ and $b$ increase to first order into this side. Smoothness and compactness give a common collar on which its interior has $a,b>0$. The local sector selected in the Statement is therefore $v>|u|$, or $a>0,b>0$, with future face $a=0,b>0$ and past face $b=0,a>0$. This identifies the supplied wedge, rather than deriving an exterior label from the horizon definition. [F1, F2, F3, step 1.1, step 3.1, given, algebra]

5.1 On $S$ the frame differential gives $du(n-\nu)=1$ and $dv(n-\nu)=-1$, whence $da(n-\nu)=-2$ and $db(n-\nu)=0$. The orientation is independent of the chosen future/outward orthonormal frame: another such frame has $n^{\prime}=\cosh\chi\,n+\sinh\chi\,\nu$ and $\nu^{\prime}=\sinh\chi\,n+\cosh\chi\,\nu$, for a smooth real function $\chi$ on $S$. Comparing the same initial normal vector in the two exponential maps gives $a^{\prime}=e^\chi a$ and $b^{\prime}=e^{-\chi}b$ on their common tube. The positive factors preserve the sector and half-sheet labels. These identities and steps 3.1 and 4.1 establish the defining pair and all stated conclusions. [F1, step 1.1, step 3.1, step 4.1, algebra] ∎

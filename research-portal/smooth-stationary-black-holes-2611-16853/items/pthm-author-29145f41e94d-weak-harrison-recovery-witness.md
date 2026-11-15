---
id: pthm-author-29145f41e94d-weak-harrison-recovery-witness
title: Weak original data furnish the one recovery family and pole
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - pthm-original-lapse-and-product
  - pthm-ernst-potential-existence
  - pthm-local-hawking-circle-fields
  - lem-author-29145f41e94d-weak-data-equivariant-global-primitive
  - lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant
  - lem-killing-normal-boost-and-invariant-tensors
  - physics:thm-gr-local-geodesics-and-exponential-map
  - physics:def-gr-metric-selected-connection
  - def-bifurcate-killing-horizon-data
  - math:cor-transverse-intersection-theorem
  - pthm-harrison-lorentzian-algebra
  - def-harrison-normalization
  - def-harrison-one-form
  - def-harrison-electromagnetic-form
  - def-harrison-one-form-family
  - lem-author-ce4974f559ec-killing-end-flux
  - lem-author-ce4974f559ec-harrison-end-restriction
  - lem-author-ce4974f559ec-positive-parameter-charge
  - lem-author-ce4974f559ec-closed-flux-transfer
  - lem-author-ce4974f559ec-fixed-sphere-endpoints
  - def-source-free-geometric-electrovacuum-data
  - lem-author-294e9b08725d-regular-positive-stationary-mass
  - pthm-ernst-and-one-form-decay
  - lem-author-a4a441da4986-exact-outer-cauchy-section
  - def-spacelike-maximal-hypersurface-data
  - math:prop-the-flow-of-a-vector-field-tangent-to-a-closed-embedded-submanifold-preserves-it
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  pthm-original-lapse-and-product: physical-result
  pthm-ernst-potential-existence: physical-result
  pthm-local-hawking-circle-fields: physical-result
  lem-author-29145f41e94d-weak-data-equivariant-global-primitive: mathematical-premise
  lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant: mathematical-premise
  lem-killing-normal-boost-and-invariant-tensors: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  math:cor-transverse-intersection-theorem: mathematical-premise
  pthm-harrison-lorentzian-algebra: physical-result
  def-harrison-normalization: mathematical-premise
  def-harrison-one-form: mathematical-premise
  def-harrison-electromagnetic-form: mathematical-premise
  def-harrison-one-form-family: mathematical-premise
  lem-author-ce4974f559ec-killing-end-flux: mathematical-premise
  lem-author-ce4974f559ec-harrison-end-restriction: mathematical-premise
  lem-author-ce4974f559ec-positive-parameter-charge: mathematical-premise
  lem-author-ce4974f559ec-closed-flux-transfer: mathematical-premise
  lem-author-ce4974f559ec-fixed-sphere-endpoints: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  lem-author-294e9b08725d-regular-positive-stationary-mass: mathematical-premise
  pthm-ernst-and-one-form-decay: physical-result
  lem-author-a4a441da4986-exact-outer-cauchy-section: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:prop-the-flow-of-a-vector-field-tangent-to-a-closed-embedded-submanifold-preserves-it: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional geometric deduction in the smooth stationary vacuum
  Einstein model; no measurement or empirical model-validity claim.
sources:
  references:
    - title: A. F. Radu, Rigidity of stationary black holes with small ADM angular
        momentum
      url: https://arxiv.org/html/2610.09729v1#A1.SS2
      locator: Section 3.1 equation (3.1) and orientation paragraph; Section 3.2
        equations (3.11)–(3.24); Appendix A.2 equations (A.12)–(A.25) and the
        following zero-locus and stationary-gauge paragraphs.
      statement: For compatible stationary vacuum, Ernst and normalized-primitive
        data, the regular Harrison formulas satisfy the source-free geometric
        Einstein–Maxwell equations. Appendix A.2 verifies the non-null
        calculation, extends it to nonzero null stationary fields by compatible
        second-order jets, and extends to zeros by smoothness and density.
      hypotheses: Smooth stationary Ricci-flat four-metric of signature (-,+,+,+);
        oriented Hodge convention as in Section 3.1; F=one half dT-flat; d
        sigma=2 i_T(F+i star F); stationary W0 with dW0=4((f-1)F+psi star F) and
        W0(T)=d0-D0; Wq=(1-q)^2W0-4q(1-q)T-flat; 0<=q<=1; Dq>0 and Dq+Wq(T)>0.
      reading_limits: Consulted the cited HTML equations and Appendix A.2, including
        the compatible-jet construction and final extension paragraphs. Import
        only this local differential identity; no reconstruction of that
        calculation or use of Proposition 3.1 as a global existence theorem is
        claimed.
dependency_level: 8
---

## Statement

In the regular stationary vacuum setting with the original maximal exterior section, mass one and $T|_S\not\equiv0$, choose the original stationary end coordinates $(t,x)$ so that $dt\wedge dx^1\wedge dx^2\wedge dx^3$ agrees with the supplied spacetime orientation $o$. Every Hodge star below uses this same $o$. Orient the original section by its future unit normal and $o$, and orient $S$ toward the exterior end; orient the original end spheres $S_R=\{t=0,|x|=R\}$ outward. Thus the compact original-section annulus $B_R$ has oriented boundary $S_R\sqcup(-S)$.

There is one choice of the normalized potential $\sigma$, common pole $p$ and smooth stationary $W_0$, with its invariant horizon gauge and weak original end decay, for which the regular Harrison formulas define one family $(g_q,F_q)$ on a common region $U=E\cup O$, where $O$ is a neighborhood of $S$ and $0\le q\le1$. Every $g_q$ is Lorentzian. The metric is jointly smooth in parameter and spacetime up to both parameter endpoints, locally on $U$. Each $F_q$ is spacetime-smooth through $S$; the family is jointly smooth for $0\le q<1$ and continuous on $[0,1]$ in $C^\infty_{\mathrm{loc}}(U)$, meaning that every spacetime derivative of its chart coefficients varies continuously, uniformly on compact chart subsets. Differentiability of $F_q$ in $q$ at $q=1$ is not asserted. The endpoint is $(g_1,F_1)=(g,0)$.

For each $q$ these fields satisfy the source-free geometric electrovacuum equations on $U$:

$$dF_q=0,\qquad d(\star_{g_q}F_q)=0,\qquad \operatorname{Ric}(g_q)_{ab}=2\left((F_q)_{ac}(F_q)_b{}^c-\frac14(g_q)_{ab}(F_q)_{cd}(F_q)^{cd}\right).$$

All raised indices in this equation use $g_q^{-1}$, with the curvature convention of the geometric electrovacuum definition. For a compact oriented smooth embedded surface $C$ without boundary, homologous to $S$ through compact smooth chains in $U$, including $S$ and each large original end sphere, the flux convention and conclusion are

$$Q_E(C,q)=\frac1{4\pi}\int_C\star_{g_q}F_q=\sqrt{1-q^2},\qquad Q_M(C,q)=\frac1{4\pi}\int_CF_q=0.$$

The local Hawking and circle fields preserve this same family near $S$, and its horizon branches retain the same Hawking generator and signed boost normalization. All these data use the same gauge and pole. The original maximal slice is retained. No application of the stronger global GR/SBS construction theorem is made. Work in the inherited ZFC convention.

The original-section maximality used here is assumed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$, with the original metric $g$, so $H_g|_C=0$. The selected physical end retains its stated mass-one normalization. Maximality of an independently labelled chart-side section or another supplied maximal section does not replace this premise. No equality between the hypersurface identification and the physical stationary end chart is assumed. [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[pthm-original-lapse-and-product]]

[[pthm-ernst-potential-existence]]

[[pthm-local-hawking-circle-fields]]

[[lem-author-29145f41e94d-weak-data-equivariant-global-primitive]]

[[lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant]]

[[lem-killing-normal-boost-and-invariant-tensors]]

[[physics:thm-gr-local-geodesics-and-exponential-map]]

[[physics:def-gr-metric-selected-connection]]

[[def-bifurcate-killing-horizon-data]]

[[math:cor-transverse-intersection-theorem]]

[[pthm-harrison-lorentzian-algebra]]

[[def-harrison-normalization]]

[[def-harrison-one-form]]

[[def-harrison-electromagnetic-form]]

[[def-harrison-one-form-family]]

[[lem-author-ce4974f559ec-killing-end-flux]]

[[lem-author-ce4974f559ec-harrison-end-restriction]]

[[lem-author-ce4974f559ec-positive-parameter-charge]]

[[lem-author-ce4974f559ec-closed-flux-transfer]]

[[lem-author-ce4974f559ec-fixed-sphere-endpoints]]

[[def-source-free-geometric-electrovacuum-data]]

## Facts & Assumptions

[F1] Use the original regular stationary vacuum geometry, its product, normalized Ernst potential and local commuting Hawking/circle fields and pole. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[pthm-original-lapse-and-product]] [[pthm-ernst-potential-existence]] [[pthm-local-hawking-circle-fields]]

[F2] The weak-data primitive supplies one smooth stationary $W_0$, locally $K,Z$-invariant, with $dW_0=4((f-1)F+\psi\star_gF)$, $W_0(T)=d_0-D_0$ and original-section spatial coefficients $O_5(r^{-3})$. [[lem-author-29145f41e94d-weak-data-equivariant-global-primitive]]

[F3] Use $B_q=1+q-(1-q)\sigma$, $D_q=|B_q|^2$, $d_q=D_q(p)$, $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, $A_qv=v+D_q^{-1}W_q(v)T$ and $g_q=(D_q/4)A_q^*g$. The electromagnetic formula is $\mathcal H_q=-\sqrt{1-q^2}(\overline B_q/B_q)A_q^*\mathcal F$, with $F_q=\operatorname{Re}\mathcal H_q$ and $\star_{g_q}F_q=\operatorname{Im}\mathcal H_q$. The family definition gives $W_q(T)=d_q-D_q$. Once $D_q>0$ and $d_q>0$ are established locally below, the rank-one result gives the Lorentzian metric with its transported time orientation. [[def-harrison-normalization]] [[def-harrison-one-form]] [[def-harrison-electromagnetic-form]] [[def-harrison-one-form-family]] [[pthm-harrison-lorentzian-algebra]]

[F4] The seed-flux lemma uses precisely the compatible end orientation and outward spheres fixed in the Statement. The end-restriction and positive-parameter lemmas require only the weak original end bounds and fixed-positive-parameter estimates. The closed-flux lemma allows the actual compact section annulus with boundary $S_R-S$, and the endpoint lemma requires continuity on one fixed compact oriented sphere. [[lem-author-ce4974f559ec-killing-end-flux]] [[lem-author-ce4974f559ec-harrison-end-restriction]] [[lem-author-ce4974f559ec-positive-parameter-charge]] [[lem-author-ce4974f559ec-closed-flux-transfer]] [[lem-author-ce4974f559ec-fixed-sphere-endpoints]]

[F5] The geometric electrovacuum definition supplies the curvature, oriented Hodge, equations and $1/(4\pi)$ electric/magnetic flux conventions. [[def-source-free-geometric-electrovacuum-data]]

[F6] For the smooth transverse chronological end-boundaries and a smooth outward section collar lying in the exterior, the exterior-quadrant lemma identifies the exterior in the normal-exponential tube $\Xi(s,a,b)=\exp_s(a n_s+b\nu_s)$ with $b>|a|$. Here $n$ is the original section's future unit normal and $\nu$ points toward its exterior side. [[lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant]]

[F7] A Killing field vanishing on $S$ with the supplied normal boost matrix has flow differential equal to that boost on the normal plane and the identity on $TS$. The metric-selected connection is the unique torsion-free metric-compatible connection, and its geodesics have unique prescribed initial data. These facts allow the local isometry action to be transported through the exponential map. [[lem-killing-normal-boost-and-invariant-tensors]] [[physics:def-gr-metric-selected-connection]] [[physics:thm-gr-local-geodesics-and-exponential-map]]

[F8] A Killing horizon has a dense nonzero-generator part on which its Killing field is tangent and normal; the signed surface gravity is specified by the ambient covector equation. The local Hawking-field supplier's Proof 4.1 supplies these null generators and the equations with signs $+\kappa$ and $-\kappa$ on the original branches. [[def-bifurcate-killing-horizon-data]] [[pthm-local-hawking-circle-fields]]

[F9] Under the regular stationary-vacuum hypotheses, the original stationary end coefficient equals the ADM energy of the original exterior section, $M_0=E_{\mathrm{ADM}}$. The mass-one normalization on this same section gives $E_{\mathrm{ADM}}=1$, hence $M_0=1$ in its stationary Cartesian end. The resulting bounds are $g_{00}=-1+2/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$ and $g_{ij}=\delta_{ij}+O_6(r^{-1})$. For the normalized potential in F1, the Ernst-decay supplier therefore gives $\sigma=1-2/r+O_6(r^{-2})$, $F_{ij}=O_5(r^{-3})$ and $(\star_gF)_{ij}=O_5(r^{-2})$ in that chart. [[lem-author-294e9b08725d-regular-positive-stationary-mass]] [[def-harrison-normalization]] [[def-regular-stationary-vacuum-spacetime]] [[pthm-ernst-and-one-form-decay]]

[F10] The original outer-section supplier gives $C=\Sigma_0\cap E$ and its ambient closure $C\cup S$, a smooth spherical exterior with compact boundary. Choose its supplied adapted topological identification with $\{|y|\ge1\}$, and write $\rho=|y|$, so that $C=\{\rho>1\}$ and $S=\{\rho=1\}$. This identification may require inversion of the originally specified spherical chart. It is separate from the physical stationary end chart $(t,x)$ with $r=|x|$. The same supplier gives nested compact smooth physical-end truncations $B_R=(C\cup S)\setminus\{t=0,r>R\}$, bounded by $S$ and $S_R$, which exhaust $C\cup S$. Its Proof 4.1 proves that the physical closed tails $\{t=0,r\ge R\}$ are closed in $C\cup S$ and disjoint from $S$. Consequently each truncation contains a relative neighborhood of $S$. [[lem-author-a4a441da4986-exact-outer-cauchy-section]]

[F11] For transverse embedded submanifolds, the tangent space of their intersection is the intersection of their tangent spaces. This applies to the two smooth transverse horizon branches meeting in $S$. [[math:cor-transverse-intersection-theorem]]

[F12] The flow of a smooth vector field tangent to a closed embedded submanifold preserves that submanifold at every defined flow point. Apply this on the common neighborhood containing the compact embedded sphere $S$. [[math:prop-the-flow-of-a-vector-field-tangent-to-a-closed-embedded-submanifold-preserves-it]]

## External input

Source 0, Appendix A.2, supplies the local Einstein–Maxwell identity for the regular formulas under the stationary vacuum, Ernst, curl, contraction and positivity hypotheses in that citation. Its compatible-jet argument includes nonzero null $T$; its final smoothness argument includes the zero locus of a nontrivial Killing field. This imported differential calculation is used below under these exact local hypotheses. It is distinct from the source's stronger global construction theorem.

## Proof

**Given:** The complete hypotheses and conventions in the Statement and Facts.

**Goal:** Establish all contracts for one compatible family without changing the original maximal section.

1.1 Choose the end chart compatible with $o$: if necessary reflect one spatial coordinate. This preserves $r$, the original $t=0$ section, mass and all weak Cartesian decay bounds. The future-normal orientation of the original section then agrees with $dx^1\wedge dx^2\wedge dx^3$ on the end. The original outer-section supplier [F10] gives a compact smooth annulus $B_R$ in the original section for every sufficiently large $R$. The chosen orientation toward infinity on $S$ is opposite to its inner-boundary orientation, so $\partial B_R=S_R\sqcup(-S)$ with the outward end-sphere orientation. This verifies the orientation and bounding hypotheses in [F4] without a condition on the transformed section being spacelike. [given, F1, F4, F5, F10]

1.2 The regular definition gives the two smooth transverse null chronological end-boundaries through $S$ and the smooth spacelike original section. By [F1] and [F10], its exterior side is exactly $\{\rho>1\}$ and its stationary-flow product is $E$. The adapted topological section coordinates chosen in [F10] give a smooth collar $c(s,\tau)$ corresponding to $(1+\tau)s$, for $s\in S^2$ and $\tau\ge0$ small; its positive-parameter points belong to $E$. Thus every hypothesis of [F6] holds, with the original section's future unit normal and its unit normal toward increasing $\rho$. It gives $E\cap O=\{b>|a|\}$ in the normal-exponential tube, the precise outward-wedge attachment required by [F2]. [F1, F6, F10]

2.1 Apply the boost assertion in [F7] to the $K$ and normal frame from [F1]. Its hypotheses hold because $K|_S=0$ and its normal boost matrix is $\kappa\begin{pmatrix}0&1\\1&0\end{pmatrix}$ with $\kappa>0$. A local $g$-isometry preserves the metric-selected connection: transporting the connection preserves torsion freedom and metric compatibility, so uniqueness in [F7] identifies it with the original connection. Geodesic initial-value uniqueness then gives $\Phi_t^K(\exp_s v)=\exp_s(d\Phi_t^K|_s v)$ wherever the local maps are defined. In the tube of step 1.2 put $u=b+a$ and $v=b-a$. The boost therefore acts as $(s,u,v)\mapsto(s,e^{\kappa t}u,e^{-\kappa t}v)$. This establishes the constant nonzero normal boost action required by [F2], before any primitive is selected. [F1, F7, step 1.2]

3.1 First verify the circle-preservation hypothesis of [F2]. By [F11], $T_sS=T_s\mathcal H^+\cap T_s\mathcal H^-$, and regularity gives $T_s\in T_sS$ for every $s\in S$. If $\Omega_H=0$, the relation $K=T+\Omega_H Z$ and $K|_S=0$ would give $T|_S=0$, contrary to the Statement. Thus $\Omega_H\ne0$, and $Z|_S=-\Omega_H^{-1}T|_S$ is tangent to $S$. The compact embedded sphere is closed in the common smooth neighborhood on which $Z$ is defined. Apply [F12] there: every defined $Z$-flow map sends $S$ into $S$, and its inverse flow gives equality. Hence the supplied period-$2\pi$ circle action preserves $S$. Now apply [F2] with $\overline\Sigma=C\cup S$, $\Sigma=C$ and the actual original exterior section, whose maximality is stipulated in the Statement. The stationary-flow product in [F1] uses this same section. The physical truncations in [F10] are compact and smooth, nested and exhausting, have boundary $S\sqcup S_R$, and contain a relative neighborhood of $S$; their physical closed tails are closed and disjoint from $S$. Thus they meet the primitive's end-attachment hypotheses with separate radii $\rho$ and $r$, without any coordinate identification. Step 1.2 verifies its outward-wedge hypothesis, and step 2.1 verifies its constant nonzero normal boost hypothesis independently of $W_0$. By [F9], the original ADM mass-one convention identifies $M_0=1$, so the unchanged original end has exactly the weak mass-one coefficient bounds required by [F2], with $T$ future timelike on a far tail. Together with the commuting fields, circle action, common pole and normalized Ernst potential from [F1], all hypotheses of [F2] now hold. Choose its one $W_0$, smooth across $S$ and locally $K,Z$-invariant, with $d_0=D_0(p)$ and original-section spatial coefficients $O_5(r^{-3})$. Apply the original lapse/product result in [F1] using the assumed maximality of this actual $C$; it gives $f<1$ on $E$. Since $S$ lies in the spacelike original section, $f=-g(T,T)\le0$ on $S$. Directly from [F3], $\operatorname{Re}B_q=2q+(1-q)(1-f)$ is positive on $E$ for $q<1$ and equals $2$ for $q=1$, so $D_q>0$ on $E$. On $S$, $\operatorname{Re}B_q\ge1+q$ and $D_q\ge(1+q)^2$. Intersect the preceding common working neighborhood of $S$ with the open set $\{f<1/2\}$, which contains $S$, and call the result $O$. On this same $O$ for every $q\in[0,1]$, $\operatorname{Re}B_q\ge2q+(1-q)/2\ge1/2$, hence $D_q>0$. At the common pole $T_p=0$, so $d_q=(1+q)^2+(1-q)^2\psi(p)^2>0$. The family normalization in [F3] now gives $D_q+W_q(T)=d_q>0$. All hypotheses of the rank-one result in [F3] hold on $U=E\cup O$: the original stationary Lorentzian data, supplied normalized potential, zero $T_p=0$, smooth stationary $W_q$, contraction identity and positive $D_q$. It therefore makes $g_q$ Lorentzian there for every $q$, with the stated time orientation. This argument uses maximality only on the physical $C$ and does not identify the independent charts. [given, F1, F2, F3, F9, F10, F11, F12, step 1.2, step 2.1, algebra]

4.1 Fix that $W_0$ and use exactly the formulas in [F3] for all parameters. Their curl and contraction normalization are the local hypotheses of source 0, and the positivity hypotheses were proved in step 3.1. Apply the imported local non-null and compatible-null calculation and its zero-locus extension. This proves the displayed electrovacuum equations on $U$, in the conventions of [F5], without using a global construction theorem. [F1, F2, F3, F5, step 3.1]

4.2 The coefficients of $W_q$, $B_q$ and $D_q$ are polynomial in $q$ with fixed smooth spacetime coefficients. Since $D_q>0$, the reciprocals and hence $A_q$ and $g_q$ are jointly smooth locally, with local extensions across both parameter endpoints. Set $J_q=-(\overline B_q/B_q)A_q^*\mathcal F$; it too is jointly smooth locally up to both endpoints. Then $\mathcal H_q=\sqrt{1-q^2}J_q$. Every spacetime derivative of $J_q$ is continuous and bounded on compact parameter-chart subsets, so multiplication by the continuous scalar factor proves the asserted $C^\infty_{\mathrm{loc}}$ continuity of $F_q$ and $\star_{g_q}F_q$ on $[0,1]$. For $q<1$ that scalar is locally smooth as well. At $q=1$, $W_1=0$, $B_1=2$, $D_1=4$, $A_1=I$ and the scalar factor is zero; thus $(g_1,F_1)=(g,0)$. [F2, F3, step 3.1, algebra]

4.3 Work on one connected neighborhood of $S$ where the local fields and the chosen $W_0$ are defined. For $X=K,Z$, the commutator $[X,T]=0$ and $\mathcal L_Xg=0$ imply invariance of $T^\flat$, $f$, $F=\tfrac12dT^\flat$ and $\mathcal F=F+i\star_gF$; the local isometry flows preserve the fixed orientation and hence the Hodge star. Therefore $d(X\sigma)=\mathcal L_Xd\sigma=0$ by the Ernst equation. Both $K$ and $Z$ vanish at the common pole $p$, so $X\sigma(p)=0$ and the constant $X\sigma$ is zero on this connected neighborhood. The chosen primitive is $K,Z$-invariant by step 3.1. Consequently $B_q,D_q,W_q,A_q$, and then $g_q,\mathcal H_q,F_q$ in [F3], are preserved by these same fields for every $q$. This proves symmetry for the actual weak-end-decay primitive, without identifying it with another existential witness. [F1, F2, F3, step 3.1]

5.1 By [F9], on the unchanged original end, $\sigma=1-2/r+O_1(r^{-2})$, the metric has the weak $O_6$ bounds and the spatial coefficients of $W_0$ are $O_5(r^{-3})$. The seed-form and spatial-Hodge estimates in [F4] give exactly the end-restriction hypotheses. For each fixed $0<q<1$, the positive-parameter charge lemma therefore gives end limits $(Q_E,Q_M)=(\sqrt{1-q^2},0)$ with the orientations of step 1.1. The two smooth Maxwell forms in step 4.1 are closed on the original annulus and through its boundary $S$. Applying the compact-cobordism case of the closed-flux lemma to $B_R$ gives equality of their integrals on $S_R$ and $S$. Taking the end limit proves the same flux pair on $S$ and every such $S_R$. The homologous-surface clause transfers it to each $C$ in the Statement. [F1, F2, F3, F4, F5, F9, step 1.1, step 4.1]

5.2 In the tube and boost coordinates established in steps 1.2 and 2.1, the two horizon axes supplied by [F6] are $u=0$ and $v=0$. Every point on either axis sufficiently near $S$ has a half-orbit staying in the tube and tending to its base point in $S$: shrink the nonzero coordinate exponentially in the appropriate time direction; the resulting explicit curve is an integral curve on that whole half-line. By step 4.3, $W_q(K)$ is constant on that curve, and its limit is zero since $K|_S=0$. Thus $W_q(K)=0$ on both branches, for this chosen family. By [F8], $K$ is the original null normal generator; tangency of $T$ to each branch gives $g(K,T)=0$ there. [F1, F2, F3, F6, F8, step 1.2, step 2.1, step 3.1, step 4.3]

6.1 On the one fixed compact oriented sphere $S$, step 4.2 verifies the continuity hypotheses of the endpoint lemma in [F4]. Its fixed-sphere limit extends the identities from $0<q<1$ to $q=0,1$ on $S$. The closed-flux lemma then transfers these endpoint identities to every surface $C$ specified in the Statement, using the Maxwell equations at that endpoint. In particular the flux pair at $q=0$ is $(1,0)$ on every fixed large end sphere, so it has that same end limit. At $q=1$ it is $(0,0)$, also directly from $F_1=0$. No interchange of parameter and spatial-infinity limits is used. [F3, F4, F5, step 4.2, step 5.1]

7.1 Expand the rank-one metric in [F3] as $4g_q=D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q$. On either branch, step 5.2 gives $g_q(K,\cdot)=(D_q/4)g(K,\cdot)$. Hence $K$ remains tangent, null and normal on the unchanged nonzero-generator part. With step 4.3 and the Lorentzian character from step 3.1, these branches are Killing horizons in the sense of [F8]. At $S$, $T\in TS$ makes $A_q(TS)\subset TS$, and invertibility makes $A_q|_{TS}$ invertible; thus $g_q|_{TS}$ is positive definite. Differentiating $4g_q(K,K)=D_qg(K,K)+2g(K,T)W_q(K)-fD_q^{-1}W_q(K)^2$ as a spacetime scalar, the vanishing of $g(K,K),g(K,T),W_q(K)$ on each branch leaves $d(g_q(K,K))=(D_q/4)d(g(K,K))$. The signed seed equations in [F8] therefore give $d(g_q(K,K))=-2\kappa g_q(K,\cdot)$ on $\mathcal H^+$ and $d(g_q(K,K))=+2\kappa g_q(K,\cdot)$ on $\mathcal H^-$. Their smooth zero extensions at $S$ retain these branch normalizations. The normal flow action, and hence its boost rate, is unchanged. All construction inputs use this one primitive, gauge and pole; the original maximal section was never replaced. Together with steps 4.1, 4.2, 5.1 and 6.1, this proves every Statement contract. [F1, F3, F8, step 3.1, step 4.1, step 4.2, step 5.1, step 6.1, step 4.3, step 5.2, algebra] ∎

## Source notes

These explicit premises specify the generated conditional result. They are not asserted to follow from the original regularity definition alone, and are not attributed to the original article. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

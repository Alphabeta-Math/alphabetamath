---
title: Nonnegative principal eigenvalue of the horizon stability operator
status: published
research_item: pthm-stable-bifurcation-mots
dependency_level: 26
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 26–27, proof of Theorem 4.2
      reading_limits: "Retained prior source-input or attribution record: Attribution
        only: The article establishes nonnegativity of the principal eigenvalue
        of the bifurcation-sphere stability operator by excluding a
        negative-eigenvalue outward trapped graph. Attributed setting: The
        article's regular stationary vacuum construction, its maximal sections
        and positive-parameter Harrison geometry. Read the frozen PDF text on
        pages 26–27 for attribution and the scope of the argument. This citation
        is not used as a proof premise. Fresh maintenance limits: current item
        and supplier contracts and the local applications were checked; no new
        reading of the external proof or PDF images is claimed."
---

PDF p. 27: ` Proof of Theorem 4.2, stability conclusion `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [pthm-author-048251387164-individual-slice-interval-continuation](item-pthm-author-048251387164-individual-slice-interval-continuation)
- [pthm-author-048251387164-indexed-admissible-end-estimates](item-pthm-author-048251387164-indexed-admissible-end-estimates)
- [pthm-author-048251387164-sequence-closure-and-completeness](item-pthm-author-048251387164-sequence-closure-and-completeness)
- [pthm-mots-stability-operator](item-pthm-mots-stability-operator)
- [pthm-negative-eigenvalue-trapped-graphs](item-pthm-negative-eigenvalue-trapped-graphs)
- [pthm-trapped-graph-focusing-contradiction](item-pthm-trapped-graph-focusing-contradiction)
- [thm-principal-eigenvalue-and-mots-stability-input](item-thm-principal-eigenvalue-and-mots-stability-input)
- [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain)
- [math:cor-smooth-functions-and-tensor-fields-extend-locally-across-the-boundary](https://alphabetamath.cc/item/cor-smooth-functions-and-tensor-fields-extend-locally-across-the-boundary)
- [math:thm-smooth-functions-defined-locally-can-be-glued-by-a-partition-of-unity](https://alphabetamath.cc/item/thm-smooth-functions-defined-locally-can-be-glued-by-a-partition-of-unity)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-harrison-one-form](item-def-harrison-one-form)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product)
- [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)
- [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive)
- [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)
- [math:thm-collar-neighborhood-theorem](https://alphabetamath.cc/item/thm-collar-neighborhood-theorem)
- [math:lem-tubular-charts-realize-a-prescribed-normal-identification](https://alphabetamath.cc/item/lem-tubular-charts-realize-a-prescribed-normal-identification)
- [math:lem-choice-free-smooth-inverse-function-theorem-in-euclidean-space](https://alphabetamath.cc/item/lem-choice-free-smooth-inverse-function-theorem-in-euclidean-space)
- [math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary)
- [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)
- [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)
- [pthm-horizon-invariant-one-form](item-pthm-horizon-invariant-one-form)
- [pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation)
- [def-harrison-electromagnetic-form](item-def-harrison-electromagnetic-form)
- [def-horizon-flux-and-stability-notation](item-def-horizon-flux-and-stability-notation)


## Statement

Assume the regular non-degenerate stationary vacuum model, with original exterior section maximal, mass normalized to one and stationary Killing field $T$ nontrivial on the bifurcation sphere $S$.

Work in ZFC. Use the stationary-flow product $\mathcal E=\mathbb R_t\times\Sigma_1^\circ$, where $C=\Sigma_0\cap\mathcal E$, $\Sigma_1=C\cup S$ is its actual closed exterior section, and $T=\partial_t$. The assumed original maximality is on $C$. An adapted topological radius $r_{\mathrm{ref}}$ identifies $\Sigma_1$ with $\{r_{\mathrm{ref}}\ge1\}$, independently of the physical end radius $r=|x|$ used below. Use the single smooth stationary Harrison primitive $W_0$ and normalized Ernst potential $\sigma=f+i\psi$, with $f=-g(T,T)$, supplied by this construction on the exterior and a neighborhood of $S$. At its supplied zero $p\in S$ of $T$, put $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $d_q=D_q(p)$. Set $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, where $T^\flat=g(T,\cdot)$, and let

$$g_q=\tfrac14\left(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q\right).$$

The construction supplies $D_q>0$, $d_q>0$ and a smooth time-oriented Lorentzian $g_q$ on that domain. On the Cartesian end use $x_q=qx$, $r_q=|x_q|=qr$ and the normalized stationary graph height $\widetilde u(qx)=d_qu(x)/(4q)$ for the graph $t=u(x)$. In the estimates below $D^j$ means the Cartesian derivatives $D_{x_q}^j$.

For each $q\in(0,1]$, choose an individually admissible section $\Sigma_q$: a connected smooth spacelike maximal section with boundary $S$, smooth up to $S$, whose interior is a global stationary graph and whose normalized end height satisfies $|D^j\widetilde u|\le C_q r_q^{-3/4-j}$ for $0\le j\le4$. Such a section exists. It admits a smooth spacelike extension $\widehat\Sigma_q$ of a neighborhood of its boundary, with $S\subset\operatorname{int}\widehat\Sigma_q$ and with the extension agreeing with $\Sigma_q$ on its original side near $S$.

Let $n_q$ be its future unit normal and $\nu_q$ the outward unit normal to $S$ within it. For $\widehat h_q=g_q|_{T\widehat\Sigma_q}$, there is $\rho_q>0$ such that $(p,r)\mapsto\exp_p^{\widehat h_q}(r\nu_q(p))$ is a diffeomorphism from $S\times(-\rho_q,\rho_q)$ onto its image in $\widehat\Sigma_q$. The radius may depend on $q$ and the chosen section. The outgoing null normal is $L_q=n_q+\nu_q$. Its outgoing expansion is the trace, in the induced surface metric, of the null second fundamental form $(X,Y)\mapsto g_q(\nabla^{(q)}_X L_q,Y)$. A marginally outer trapped surface, abbreviated MOTS, is a closed spacelike surface whose outgoing expansion vanishes. Let $\mathscr L_q$ be the linearization of that expansion under outward normal graphs in the fixed $n_q+\nu$ gauge, and let $\lambda_1(\mathscr L_q)$ be its real principal eigenvalue, the eigenvalue admitting a positive eigenfunction and having least real part. Then $S$ is a MOTS and $\lambda_1(\mathscr L_q)\ge0$. Equivalently, it is stable in this outward direction: there exists a smooth nonnegative normal speed, not identically zero, whose first variation of outgoing expansion is nonnegative everywhere. In particular, the conclusion holds for all sufficiently small $q>0$.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[pthm-author-048251387164-individual-slice-interval-continuation](item-pthm-author-048251387164-individual-slice-interval-continuation)

[pthm-author-048251387164-indexed-admissible-end-estimates](item-pthm-author-048251387164-indexed-admissible-end-estimates)

[pthm-mots-stability-operator](item-pthm-mots-stability-operator)

[thm-principal-eigenvalue-and-mots-stability-input](item-thm-principal-eigenvalue-and-mots-stability-input)

[pthm-original-lapse-and-product](item-pthm-original-lapse-and-product)

[pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)

[pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive)

[pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)

[def-harrison-normalization](item-def-harrison-normalization)

[def-harrison-one-form](item-def-harrison-one-form)

[def-stationary-maximal-graph](item-def-stationary-maximal-graph)

## Facts & Assumptions

[A1] Adopt the stated regular stationary vacuum model, maximal original exterior section, mass-one normalization and $T|_S\not\equiv0$. The regularity definition makes $S$ a smooth embedded two-sphere. Work in ZFC. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F0] Under [A1], the original exterior has the stated stationary-flow product. The global one-form construction supplies the normalized Ernst data, the zero $p$ and the single stationary primitive $W_0$. The denominator result gives positivity on the exterior and near $S$; the regular Harrison result supplies the smooth time-oriented Lorentzian metric there from this same primitive and $W_q$. The Harrison and graph definitions specify the metric formula, $d_q$, the normalized coordinates and height, and the meaning of a stationary maximal graph. [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product) [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form) [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive) [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum) [def-harrison-normalization](item-def-harrison-normalization) [def-harrison-one-form](item-def-harrison-one-form) [def-stationary-maximal-graph](item-def-stationary-maximal-graph)

[F1] Every $q\in(0,1]$ carries an individually admissible section with the properties stated above. A constant sequence of such pairs has a subsequence converging to a section complete with its boundary included. [pthm-author-048251387164-individual-slice-interval-continuation](item-pthm-author-048251387164-individual-slice-interval-continuation) [pthm-author-048251387164-indexed-admissible-end-estimates](item-pthm-author-048251387164-indexed-admissible-end-estimates) [pthm-author-048251387164-sequence-closure-and-completeness](item-pthm-author-048251387164-sequence-closure-and-completeness) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F2] Smooth boundary functions have local extensions across the boundary. In the declared ZFC convention an open cover admits a subordinate smooth partition, and weighted sums glue smooth real-valued functions on a common base. A compact embedded surface with a supplied unit normal in a smooth spacelike extension has a normal-graph tube. [math:cor-smooth-functions-and-tensor-fields-extend-locally-across-the-boundary](https://alphabetamath.cc/item/cor-smooth-functions-and-tensor-fields-extend-locally-across-the-boundary) [math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary) [math:thm-smooth-functions-defined-locally-can-be-glued-by-a-partition-of-unity](https://alphabetamath.cc/item/thm-smooth-functions-defined-locally-can-be-glued-by-a-partition-of-unity) [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain)

[F3] Once its common-field and boundary hypotheses are verified, the stability-operator result gives zero outgoing expansion and a smooth real elliptic variation operator with leading term minus the surface Laplacian in the stated section and graph gauge. [pthm-mots-stability-operator](item-pthm-mots-stability-operator)

[F4] On a connected closed smooth surface, this operator has a real principal eigenvalue and a smooth positive eigenfunction. Its nonnegative principal eigenvalue is equivalent to the existence of a smooth nonnegative normal speed, not identically zero, whose first variation of outgoing expansion is nonnegative everywhere. [thm-principal-eigenvalue-and-mots-stability-input](item-thm-principal-eigenvalue-and-mots-stability-input)

[F5] A negative principal eigenvalue produces arbitrarily small outward graphs whose outgoing expansion is strictly negative; after fixing one graph it is bounded above by a negative constant. [pthm-negative-eigenvalue-trapped-graphs](item-pthm-negative-eigenvalue-trapped-graphs)

[F6] In the same fixed-positive-parameter construction, for a complete smooth maximal stationary graph section with its smooth boundary extension, the negative-eigenvalue graph alternative leads to the first-cylinder-contact and null-focusing contradiction. [pthm-trapped-graph-focusing-contradiction](item-pthm-trapped-graph-focusing-contradiction)

[F7] A smooth manifold with boundary has a smooth collar. For a closed embedded submanifold and a specified bundle isomorphism onto its quotient normal bundle, there is a tubular chart inducing that isomorphism. A smooth Euclidean map with invertible derivative has a smooth local inverse. The real mean value theorem gives the sign of a smooth function that vanishes at zero and has positive derivative nearby. The collar and tubular statements assume countable choice, which is available in ZFC. [math:thm-collar-neighborhood-theorem](https://alphabetamath.cc/item/thm-collar-neighborhood-theorem) [math:lem-tubular-charts-realize-a-prescribed-normal-identification](https://alphabetamath.cc/item/lem-tubular-charts-realize-a-prescribed-normal-identification) [math:lem-choice-free-smooth-inverse-function-theorem-in-euclidean-space](https://alphabetamath.cc/item/lem-choice-free-smooth-inverse-function-theorem-in-euclidean-space) [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

[F8] Under [A1], the local-field supplier gives the commuting Hawking and circle fields $K,Z$, their relation $K=T+\Omega_HZ$, the common zero $p$ and nonzero normal boost. The invariant-data result gives local $K,Z$ invariance of the normalized Ernst potential and the invariant primitive construction. The global supplier in [F0] uses that same construction and already supplies a locally $K,Z$-invariant $W_0$. Horizon preservation applies to the resulting invariant Harrison family, on a neighborhood of $S$. [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields) [pthm-horizon-invariant-one-form](item-pthm-horizon-invariant-one-form) [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form) [pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation)

[F9] The electromagnetic definition assigns a smooth real $F_q$ to the same normalized Ernst data, pole, $W_q$ and positive denominator, with the original spacetime orientation. The regular electrovacuum result realizes these fields smoothly on the exterior and a neighborhood of $S$, using the time orientation transported from the original future field $N$ by $A_q^{-1}$, where $A_qv=v+D_q^{-1}W_q(v)T$. The horizon notation defines boundary data by restrictions of these fields and specifies the future/outward normal-graph gauge. [def-harrison-electromagnetic-form](item-def-harrison-electromagnetic-form) [def-harrison-one-form](item-def-harrison-one-form) [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum) [def-horizon-flux-and-stability-notation](item-def-horizon-flux-and-stability-notation)

## Proof

**Given:** The model and positive parameter in the Statement.

**Goal:** Prove the MOTS and stability conclusions, including the extension needed for the supplier applications.

1.1 Fix $q\in(0,1]$. The hypotheses of [F0] are exactly [A1], so use its single primitive, positive denominator, regular metric and stationary product throughout. By [F1], choose an individually admissible section. Apply its sequence-closure result on $[q/2,1]$ to the constant sequence consisting of this same section and parameter. A constant sequence of the stationary graph functions and boundary graph representations has that same section as its limit. Hence the chosen section is complete with $S$ included. [given, A1, F0, F1, construct]

2.1 Verify the invariant construction for these actual fields. The regular model, original maximality and $T|_S\not\equiv0$ in [A1] meet the local-field hypotheses of [F8]; use the $K,Z$ and common pole $p$ employed by the global construction in [F0]. The invariant-data result applies with the same mass-one convention and normalized Ernst potential, so that potential is locally $K,Z$ invariant. The already chosen global $W_0$ is locally $K,Z$ invariant by [F8]; no replacement primitive is needed. Hence the very family $W_q=(1-q)^2W_0-4q(1-q)T^\flat$ in the Statement is the invariant horizon family: the commuting Killing fields preserve $T^\flat$, as in the invariant-data result. The horizon-preservation hypotheses are therefore met by this family and [A1]. Define $F_q$ by [F9] from these same data and use the electrovacuum realization in [F0]. Intersect its open neighborhood of $S$ with the invariant-data and horizon-preservation neighborhoods, obtaining an open $O$ containing $S$. On $O$, both applications use the identical metric formula, potential, pole and primitive. The real two-form is the single $F_q$ just defined; the horizon-preservation result concerns this metric and imposes no competing electromagnetic choice. Retain the original spacetime orientation, the electrovacuum time orientation $A_q^{-1}N$, and the orientation of $S$ transported from outward end spheres. Thus there is one oriented, time-oriented smooth pair $g_q,F_q$ on $O$, satisfying electrovacuum and horizon preservation for the supplied construction. [A1, F0, F8, F9, step 1.1, construct]

3.1 We construct a smooth spacelike extension using one ambient tubular chart. Take a collar $c:S\times[0,a)\to\Sigma_q$ from [F7], with $c(s,0)=s$. Its inward transverse vector at $S$, projected orthogonally off $TS$ within the positive metric on $T\Sigma_q$ and normalized, gives a smooth inward unit normal $\mu$ to $S$ within the section. Together with the smooth future unit normal $n_q$, it gives the normal-quotient isomorphism $\alpha_s(r,z)=[r\mu_s+zn_q(s)]$ from $S\times\mathbb R^2$ to $TM|_S/TS$. Work inside the common open neighborhood $O$ from step 2.1, with its smooth metric $g_q$. The sphere is compact and therefore closed in this ambient manifold. Apply [F7] to obtain a diffeomorphism $\Phi$ from a neighborhood of $S\times\{(0,0)\}$ onto an ambient neighborhood of $S$, fixed on $S$, inducing $\alpha$. Shrinking using compactness gives a uniform fiber box. Write its coordinates as $(s,r,z)$, and let $P(\Phi(s,r,z))=(s,r)$. Since $d\Phi(\partial_r)-\mu$ and $d\Phi(\partial_z)-n_q$ lie in $TS$ along the zero section, $dP|_{T\Sigma_q}$ is invertible there, and its $r$ coordinate increases on inward transverse vectors. [A1, F1, F7, step 1.1, step 2.1, construct]

4.1 Here is the boundary and global compatibility check for that projection. In collar coordinates $(y,t)$ the map $P\circ c$ fixes $(y,0)$, and its last coordinate $R(y,t)$ has $R(y,0)=0$ and $\partial_tR(y,0)>0$. Extend its coordinate functions across $t=0$ by [F2]. The derivative remains invertible there, so the Euclidean inverse theorem in [F7] gives local smooth inverses. After shrinking, the smooth extension has $\partial_tR>0$. For each fixed $y$, apply the real mean value theorem in [F7] on the interval between $0$ and $t$: smoothness supplies continuity on that closed interval and differentiability inside it, and $R(y,0)=0$. Thus $R$ and $t$ have the same sign, so the local inverses restrict to inverses of the half-collars. Shrink the collar into these local inverse domains. They give local scalar representations $z=v(s,r)$ for $r\ge0$. The projection is injective on some smaller whole collar: otherwise distinct pairs in collars of widths tending to zero would have equal projections; compactness gives limits on $S$, equality of projections gives the same limiting point, and both pairs eventually lie in one of the injective local inverse neighborhoods just obtained. Its image is relatively open around the compact seam, so contains $S\times[0,b)$ for some $b>0$. Restricting to that cylinder therefore gives one smooth real function $v$, rather than graph functions in different ambient coordinates. [F2, F7, step 3.1, construct]

5.1 Apply [F2] to this scalar $v$ on $S\times[0,b)$, obtaining smooth local extensions $v_i$ on open subsets of the signed product $S\times(-b,b)$ covering the seam. Restrict to a smaller signed cylinder inside their union, choose its subordinate smooth partition $(\chi_i)$, and set $\bar v=\sum_i\chi_i v_i$. Every $v_i$ equals the same $v$ on its original half-domain, so $\bar v=v$ for $r\ge0$; all derivatives along $r=0$ also agree. Shrink the cylinder so that $(s,r,\bar v(s,r))$ remains in the domain of $\Phi$. Its graph under $\Phi$ is an embedded smooth hypersurface with $S$ in its interior, agreeing with the original section for $r\ge0$. At the seam its tangent metric is the original positive-definite metric; openness of positive definiteness and compactness of $S$ make the graph spacelike on a smaller signed cylinder. Finally take the ambient neighborhood of $S$ small enough to meet the original embedded section only in the collar just represented. The negative-$r$ graph then has no intersection with the rest of the section, and gluing on the shared positive collar gives the required smooth spacelike extension of the section. No maximality beyond the original side is claimed. [F2, step 3.1, step 4.1, construct]

6.1 The outward unit normal $\nu_q$ to $S$ in this extension is supplied by the original side and its metric, which the extension preserves. The compact normal-graph result in [F2] now applies with $S$ in the interior of the extended spacelike hypersurface, equipped with the smooth Riemannian metric $\widehat h_q=g_q|_{T\widehat\Sigma_q}$. It gives a radius $\rho_q>0$ and the asserted diffeomorphism $(p,r)\mapsto\exp_p^{\widehat h_q}(r\nu_q(p))$ on $S\times(-\rho_q,\rho_q)$. Its countable-choice hypothesis is supplied by ZFC; no radius uniform in $q$ or in the choice of section is claimed. Thus the original complete maximal stationary graph section has exactly the extension and graph data required by [F3], [F5] and [F6]. [F2, F3, F5, F6, step 1.1, step 5.1]

7.1 Supply the matching boundary fields required by [F3]. Set $U_S=O_S=O$ and take the metric and two-form there to be restrictions of the single pair in step 2.1. Their agreement with the exterior Harrison fields is literal restriction of the same smooth tensors on the exterior union $O$, with the same spacetime and time orientations. The extension in step 5.1 was constructed in $O$. Shrink its collar and the tube from step 6.1 so that their images lie in $O$; compactness of $S$ permits this because the graph map is continuous and its zero section lies in $O$. The outward unit normal is the one determined by the original exterior side, and the future unit normal uses the unchanged electrovacuum time orientation. These are exactly the boundary data of [F9] in the $n_q+\nu$ gauge. Together with step 2.1 they meet the common invariant-construction, electromagnetic-field and orientation hypotheses of [F3], rather than merely postulating compatible extensions. [F3, F9, step 2.1, step 5.1, step 6.1, construct]

8.1 The sphere is connected and compact by [A1]. The variation result [F3] gives zero outgoing expansion and the stated smooth elliptic operator in the future/outward gauge. Hence $S$ is a MOTS, and [F4] supplies the real principal eigenvalue and its positive eigenfunction. [A1, F3, F4, step 6.1, step 7.1]

9.1 Assume for contradiction that $\lambda_1(\mathscr L_q)<0$. By [F5], choose a sufficiently small outward eigenfunction graph with outgoing expansion at most $-\delta_*$ for some fixed $\delta_*>0$. The original section is complete, smooth and maximal, its interior is a stationary graph, and it has the required boundary extension and tube by steps 1.1 and 6.1. [F5, step 1.1, step 6.1, step 8.1, assume-contra]

10.1 Therefore [F6] applies to precisely this graph and gives a focal point before a first-contact target while the same null segment has no such interior focal point. This is a contradiction, so the assumption of a negative principal eigenvalue is false. Consequently $\lambda_1(\mathscr L_q)\ge0$. For the positive principal eigenfunction $\phi$ from step 8.1, $\mathscr L_q\phi=\lambda_1(\mathscr L_q)\phi\ge0$ everywhere. Thus $\phi$ is a smooth nonnegative normal speed, not identically zero, with nonnegative first variation everywhere, and [F4] gives the stated outward stability. Since $q$ was arbitrary in $(0,1]$, the sufficiently-small-positive-$q$ claim follows. [given, F4, F5, F6, step 1.1, step 6.1, step 8.1, step 9.1, discharge-contradiction] ∎

## Source notes

The article reference attributes the stability claim and its focusing method. The proof uses the listed suppliers and the local compatible-extension construction; the article's claim is not a premise.

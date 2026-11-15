---
id: pthm-horizon-invariant-one-form
title: Invariant Ernst data and smooth K-invariant gauge
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-harrison-normalization
  - def-killing-ernst-notation
  - def-harrison-one-form-family
  - pthm-original-lapse-and-product
  - pthm-local-hawking-circle-fields
  - pthm-ernst-potential-existence
  - lem-author-29145f41e94d-weak-data-equivariant-global-primitive
  - lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant
  - lem-author-a4a441da4986-exact-outer-cauchy-section
  - lem-author-294e9b08725d-regular-positive-stationary-mass
  - math:cor-lie-derivative-commutes-with-the-exterior-derivative
  - math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component
  - math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes
  - math:thm-lie-derivative-of-a-vector-field-equals-the-lie-bracket
  - math:thm-the-exterior-derivative-commutes-with-pullback
  - math:prop-the-flow-of-a-vector-field-tangent-to-a-closed-embedded-submanifold-preserves-it
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  def-harrison-one-form-family: mathematical-premise
  pthm-original-lapse-and-product: physical-result
  pthm-local-hawking-circle-fields: physical-result
  pthm-ernst-potential-existence: physical-result
  lem-author-a4a441da4986-exact-outer-cauchy-section: mathematical-premise
  lem-author-29145f41e94d-weak-data-equivariant-global-primitive: mathematical-premise
  lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant: mathematical-premise
  lem-author-294e9b08725d-regular-positive-stationary-mass: mathematical-premise
  math:cor-lie-derivative-commutes-with-the-exterior-derivative: mathematical-premise
  math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component: mathematical-premise
  math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes: mathematical-premise
  math:thm-lie-derivative-of-a-vector-field-equals-the-lie-bracket: mathematical-premise
  math:thm-the-exterior-derivative-commutes-with-pullback: mathematical-premise
  math:prop-the-flow-of-a-vector-field-tangent-to-a-closed-embedded-submanifold-preserves-it: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 11, §2.4, invariance display and following paragraph
      statement: The article states that K and Z preserve the Ernst potential and
        Theta_0, and that W_0 can be chosen smoothly at S so that W_0 and W_q
        are K-invariant.
      hypotheses: The article's regular stationary vacuum construction, with the local
        fields and normalized Harrison family described there.
      reading_limits: Read the frozen article text at the cited passage for
        attribution. This citation is not used as proof of the claim or of its
        prerequisites.
physical_scope: Conditional deductions in the smooth four-dimensional stationary
  vacuum model with the specified maximal exterior section; no observation or
  existence of a physical spacetime is asserted.
dependency_level: 8
---

## Statement

Adopt the stationary vacuum model [[post-stationary-vacuum-model]] and regular data [[def-regular-stationary-vacuum-spacetime]], with $T|_S\not\equiv0$, maximal outer section as in [[def-spacelike-maximal-hypersurface-data]], and mass normalized to one as in [[def-harrison-normalization]]. Let $K=T+\Omega_H Z$ and $Z$ be the local Killing fields near the bifurcation sphere $S$ supplied by [[pthm-local-hawking-circle-fields]]; their flows commute with that of $T$, $K$ vanishes on $S$, and $Z$ has a common zero $p\in S$ with $T$. A Killing field has vanishing Lie derivative of $g$, and the Lie derivative is taken along its local flow.

Use the normalized smooth Ernst potential $\sigma=f+i\psi$ supplied by [[pthm-ernst-potential-existence]], with $f=-g(T,T)$, and put $F=\tfrac12dT^\flat$, $T^\flat=g(T,\cdot)$, and $\Theta_0=4((f-1)F+\psi\star_g F)$ as in [[def-killing-ernst-notation]] and [[def-harrison-one-form-family]]. After shrinking to a connected neighborhood of $S$ where the local fields and potential are defined, $\mathcal L_K\sigma=\mathcal L_Z\sigma=0$ and $\mathcal L_K\Theta_0=\mathcal L_Z\Theta_0=0$.

There is a single smooth stationary real one-form $W_0$ on the exterior and a neighborhood of $S$ such that $dW_0=\Theta_0$, $W_0(T)=D_0(p)-D_0$, and $\mathcal L_KW_0=\mathcal L_ZW_0=0$ locally. Here $D_0=|1-\sigma|^2$. For every $q\in[0,1]$, define $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. Then $W_q$ is smooth through $S$ and $\mathcal L_KW_q=0$ locally; in fact $\mathcal L_ZW_q=0$ there as well. These are local symmetry assertions, not global extensions of $K$ or $Z$.

The original-section maximality used here is assumed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$, with the original metric $g$, so $H_g|_C=0$. The selected physical end retains its stated mass-one normalization. Maximality of an independently labelled chart-side section or another supplied maximal section does not replace this premise. No equality between the hypersurface identification and the physical stationary end chart is assumed. [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

## Facts & Assumptions

[A1] The stated model and regularity hypotheses include the smooth oriented stationary vacuum geometry, the specified asymptotic end and spherical bifurcate horizon. The outer section is maximal, $T|_S\not\equiv0$, and the mass is one. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]] [[def-harrison-normalization]]

[F1] The local-field result supplies the commuting Killing fields, their constant linear relation, the period-$2\pi$ circle action generated by $Z$, and the common zero $p$. [[pthm-local-hawking-circle-fields]]

[F2] The Ernst result supplies a smooth potential extending to a neighborhood of $S$, with $d\sigma=2\iota_T(F+i\star_g F)$. The notation interface specifies the metric, orientation, Hodge star and Killing form. [[pthm-ernst-potential-existence]] [[def-killing-ernst-notation]]

[F3] The original lapse/product result supplies the stationary product over the actual exterior section $C=\Sigma_0\cap E$. Its closed exterior $C\cup S$ admits an adapted spherical identification with $\{|y|\ge1\}$, chosen from the section supplier; it need not be the originally specified spherical chart or the physical end chart. The same section supplier gives compact smooth physical truncations $B_R=(C\cup S)\setminus\{r>R\}$ with boundary $S\sqcup\{r=R\}$ and a neighborhood of $S$, exhausting the section. Its closed physical tails are closed in $C\cup S$ and avoid $S$. The smooth outward collar at $S$, together with the regular event-boundary sheets, satisfies the horizon-axes supplier. [[pthm-original-lapse-and-product]] [[lem-author-a4a441da4986-exact-outer-cauchy-section]] [[lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant]] [[def-regular-stationary-vacuum-spacetime]]

[F4] Given the weak mass-one stationary vacuum end, spherical stationary-flow product, compact physical truncations and closed physical tails separate from its topological radius, outward-wedge attachment, normalized Ernst potential and commuting local boost/circle fields with common pole and circle action preserving $S$, the weak-data equivariant primitive lemma supplies one smooth stationary primitive on $E$ and a neighborhood of $S$, locally $K,Z$-invariant and satisfying $W_0(T)+D_0=D_0(p)$. Its original-section end coefficients are $O_5(r^{-3})$; no stronger same-section angular-momentum expansion is required. [[lem-author-29145f41e94d-weak-data-equivariant-global-primitive]]

[F5] The family definition gives $\Theta_0$ and $W_q$ from that same normalized primitive for all $q\in[0,1]$. [[def-harrison-one-form-family]]

[F6] Under the regular stationary-vacuum hypotheses, the ADM energy of the complete exterior section equals the original stationary end coefficient: $E_{\mathrm{ADM}}=M_0$. The mass-one convention on this same original section sets $E_{\mathrm{ADM}}=1$. Thus $M_0=1$ in the original end chart. [[lem-author-294e9b08725d-regular-positive-stationary-mass]] [[def-harrison-normalization]]

[F7] For smooth vector fields and differential forms, $\mathcal L_Xd=d\mathcal L_X$. Apply this identity componentwise to complex forms. [[math:cor-lie-derivative-commutes-with-the-exterior-derivative]]

[F8] A smooth real-valued function with zero differential is constant on each connected component. Apply this separately to the real and imaginary parts of a smooth complex-valued function. [[math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component]]

[F9] For a smooth tensor field $A$ and a smooth vector field $X$ with local flow $\Phi_t$, $\mathcal L_XA=0$ if and only if $\Phi_t^*A=A$ on every common local flow domain. This applies to both covariant tensors and vector fields. [[math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes]]

[F10] For smooth vector fields $X,Y$, $\mathcal L_XY=[X,Y]$. [[math:thm-lie-derivative-of-a-vector-field-equals-the-lie-bracket]]

[F11] For a smooth map $h$ and differential form $\omega$, $h^*(d\omega)=d(h^*\omega)$. [[math:thm-the-exterior-derivative-commutes-with-pullback]]

[F12] A smooth vector field tangent to a closed embedded submanifold has a local flow preserving that submanifold at every defined flow time. [[math:prop-the-flow-of-a-vector-field-tangent-to-a-closed-embedded-submanifold-preserves-it]]

## Proof

**Given:**The model, geometric hypotheses and fields in the Statement.

**Goal:** Establish the local invariances and the stated smooth choice of the one-form family.

1.1 Let $X$ be either $K$ or $Z$, and let $\Phi_t$ be its local flow. By [F1], $\mathcal L_Xg=0$ and $[X,T]=0$. By [F10], $\mathcal L_XT=0$. Applying [F9] to the smooth tensors $g$ and $T$ gives $\Phi_t^*g=g$ and $\Phi_t^*T=T$ on each common local flow domain. Contraction of these preserved tensors shows that $\Phi_t^*T^\flat=T^\flat$ and $\Phi_t^*f=f$. By [F11], $\Phi_t^*F=\tfrac12\Phi_t^*(dT^\flat)=\tfrac12d(\Phi_t^*T^\flat)=F$. [F1, F2, F9, F10, F11]

2.1 The local diffeomorphisms $\Phi_t$ start at the identity. Their differential determinants are continuous and nonzero, so their orientation sign remains positive on the flow interval through zero. In positively oriented coordinates the metric volume form is $\epsilon_g=\sqrt{|\det(g_{ab})|}\,dx^0\wedge dx^1\wedge dx^2\wedge dx^3$. The determinant transformation law, $\Phi_t^*g=g$ and this positive sign give $\Phi_t^*\epsilon_g=\epsilon_g$; the inverse metric is preserved as well. The Lorentzian component formula $(\star_gF)_{ab}=\tfrac12(\epsilon_g)_{ab\mu\nu}g^{\mu c}g^{\nu d}F_{cd}$ in [F2] therefore gives $\Phi_t^*(\star_gF)=\star_gF$ by contraction of the preserved tensors. Since $T$ is preserved, evaluation on $T$ also commutes with pullback, so $\Phi_t^*(2\iota_T(F+i\star_gF))=2\iota_T(F+i\star_gF)=d\sigma$. Differentiating at $t=0$ gives $\mathcal L_X(d\sigma)=0$. By [F7], $d(\mathcal L_X\sigma)=\mathcal L_X(d\sigma)=0$, with the identity applied to real and imaginary parts. [F2, F7, F9, step 1.1]

2.2 Choose the adapted spherical identification from [F3]. It identifies the closure of $C$ with $[1,\infty)\times S^2$ and gives a smooth collar pointing into $C$ at $S$, independently of the physical stationary end coordinates. The regular event-boundary branches in [A1] and this collar satisfy the horizon-axes lemma in [F3], giving exactly the outward-wedge attachment required by [F4]. The same [F3] gives its stationary-flow product. Its physical truncations and closed tails meet precisely the primitive lemma's separate end-attachment hypotheses: the truncations are compact smooth regions bounded by $S$ and the physical sphere, contain a neighborhood of $S$ and exhaust the closure, while the closed physical tails avoid $S$. Thus the topological radius used for the horizon collar need not equal the physical $r$ used for decay and the end cutoff. By [F6], the ADM mass-one convention in [A1] gives $M_0=E_{\mathrm{ADM}}=1$ for the unchanged original section; substituting this coefficient in the regular end bounds in [A1] gives $g_{00}=-1+2/r+O_6(r^{-2})$, with $g_{0i}=O_6(r^{-2})$ and $g_{ij}=\delta_{ij}+O_6(r^{-1})$ in the original chart. The smooth normalized potential in [F2] has the required equation and horizon extension. By regularity in [A1], $T_s\in T_s\mathcal H^+\cap T_s\mathcal H^-$ for each $s\in S$. The inclusion $T_sS\subset T_s\mathcal H^+\cap T_s\mathcal H^-$ is equality: transversality makes this intersection two-dimensional, the dimension of $S$. Thus $T$ is tangent to $S$. If $\Omega_H=0$, the relation in [F1] would give $T|_S=K|_S=0$, contrary to [A1]. Hence $\Omega_H\ne0$, and $Z|_S=-\Omega_H^{-1}T|_S$ is tangent to $S$. The embedded sphere $S$ is compact, hence closed in the common smooth neighborhood where $Z$ is defined. Apply [F12] on that neighborhood: every defined $Z$-flow map takes $S$ into $S$, and its inverse flow gives equality. Therefore the circle action in [F1] preserves $S$, as required by [F4]. The fields in [F1] have the constant nonzero normal boost rate, commuting circle action and common zero required by [F4]; their isometry flows preserve time orientation because they start at the identity. All hypotheses of the weak-data primitive lemma therefore hold. Apply it to choose its single smooth stationary $W_0$ with the stated derivative, normalization and local $K$- and $Z$-invariance. [A1, F1, F2, F3, F4, F6, F12, step 1.1]

3.1 On the connected neighborhood, step 2.1 gives zero differential for the real and imaginary parts of $\mathcal L_X\sigma$. By [F8], each part is constant, so $\mathcal L_X\sigma$ is constant. At $p$, both $K$ and $Z$ vanish: $K|_S=0$ and $Z(p)=0$. Hence each derivative $X(\sigma)$ vanishes at $p$, so both constants are zero. Taking real and imaginary parts and using the preserved $F$ and Hodge star in the displayed formula for $\Theta_0$ gives $\mathcal L_K\Theta_0=\mathcal L_Z\Theta_0=0$. [F1, F2, F5, F8, step 1.1, step 2.1]

4.1 For fixed $q\in[0,1]$, [F5] expresses $W_q$ as a constant linear combination of $W_0$ and $T^\flat$. Both terms are smooth through $S$, and both are invariant under $K$ and $Z$ by steps 1.1 and 2.2. The asserted smoothness and Lie-derivative identities follow. [F5, step 1.1, step 2.2] ∎



The article reference attributes the original local claims. The existence and invariant gauge of the primitive are supplied by the existing weak-data equivariant primitive lemma under the product, outward-wedge and weak-end hypotheses verified above. Its local construction is not reconstructed here, and the stronger GR/SBS primitive import is not invoked.

## Source notes

The article reference attributes the original local claims. The existence and invariant gauge of the primitive are supplied by the existing weak-data equivariant primitive lemma under the product, outward-wedge and weak-end hypotheses verified above. Its local construction is not reconstructed here, and the stronger GR/SBS primitive import is not invoked.

These explicit premises specify the generated conditional result. They are not asserted to follow from the original regularity definition alone, and are not attributed to the original article. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

---
id: pthm-bifurcate-horizon-preservation
title: Preservation of bifurcate horizons and surface gravity
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - def-null-screen-expansion-and-focal-data
  - def-harrison-normalization
  - def-harrison-one-form
  - pthm-local-hawking-circle-fields
  - pthm-horizon-invariant-one-form
  - pthm-harrison-denominator-positive
  - pthm-harrison-lorentzian-algebra
  - lem-killing-normal-boost-and-invariant-tensors
  - math:def-local-and-global-flow
  - math:def-lie-derivative-of-a-tensor-field
  - math:thm-lie-derivative-of-a-vector-field-equals-the-lie-bracket
  - physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative
  - def-harrison-one-form-family
  - math:def-exterior-derivative-by-the-invariant-vector-field-formula
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-harrison-one-form: mathematical-premise
  pthm-local-hawking-circle-fields: physical-result
  pthm-horizon-invariant-one-form: physical-result
  pthm-harrison-denominator-positive: physical-result
  pthm-harrison-lorentzian-algebra: physical-result
  lem-killing-normal-boost-and-invariant-tensors: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  math:def-lie-derivative-of-a-tensor-field: mathematical-premise
  math:thm-lie-derivative-of-a-vector-field-equals-the-lie-bracket: mathematical-premise
  physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative: mathematical-premise
  def-harrison-one-form-family: mathematical-premise
  math:def-exterior-derivative-by-the-invariant-vector-field-formula: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 11, §2.4, horizon-preservation argument
      attribution: The article states that the Harrison metrics preserve the local
        horizons, their Hawking field and surface gravity, and that the
        bifurcation surface is totally geodesic.
      hypotheses: The article's regular stationary vacuum construction, its invariant
        Harrison gauge and q in [0,1].
      reading_limits: Read the frozen extracted article text at the cited passage for
        attribution. The article is not used as proof of this item.
physical_scope: Conditional geometric deductions in the smooth stationary vacuum
  model and its Harrison metric family; no observation or measurement is
  asserted.
dependency_level: 9
---

## Statement

Adopt [[post-stationary-vacuum-model]] and the regular data of [[def-regular-stationary-vacuum-spacetime]], with $T|_S\not\equiv0$, maximal outer section and mass one. Use the local Hawking field $K$, the constant $\kappa>0$, the smooth normalized Ernst potential $\sigma=f+i\psi$, and the $K$-invariant Harrison family supplied by [[pthm-local-hawking-circle-fields]] and [[pthm-horizon-invariant-one-form]]. Here $f=-g(T,T)$, $D_q=|q(1+\sigma)+(1-\sigma)|^2$, and $g_q$ is the metric of [[def-harrison-one-form]]. The branches $\mathcal H^\pm$ are the specified local null hypersurfaces through the bifurcation sphere $S$; shrink their common neighborhood of $S$ when necessary.

For every $q\in[0,1]$, both branches are $g_q$-Killing horizons for $K$. On $\mathcal H^+$, $W_q(K)=0$, $g(K,T)=0$, $g_q(K,\cdot)=(D_q/4)g(K,\cdot)$, and $d(g_q(K,K))=-2\kappa g_q(K,\cdot)$. On $\mathcal H^-$ the analogous covector equation has signed surface gravity $-\kappa$. Thus the boost rate remains $\kappa$ with the stated past-branch sign. The sphere $S$ is spacelike and totally geodesic for $g_q$, and both its null second fundamental forms vanish. These are local conclusions; no global extension of $K$ is asserted.

A Killing horizon means a null hypersurface on whose nonzero-generator part the Killing field is tangent and normal, with that part nonempty and dense. Its signed surface gravity is defined there by the displayed ambient covector equation. A submanifold is totally geodesic when the normal component of $\nabla^q_XY$ vanishes for all tangent fields $X,Y$, where $\nabla^q$ is the Levi–Civita connection of $g_q$. For a null normal $L$ to $S$, its null second fundamental form is $(X,Y)\mapsto g_q(\nabla^q_XL,Y)$.

The original-section maximality used here is assumed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$, with the original metric $g$, so $H_g|_C=0$. The selected physical end retains its stated mass-one normalization. Maximality of an independently labelled chart-side section or another supplied maximal section does not replace this premise. No equality between the hypersurface identification and the physical stationary end chart is assumed. [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-stationary-lorentzian-data]]

[[def-bifurcate-killing-horizon-data]]

[[def-null-screen-expansion-and-focal-data]]

[[def-harrison-normalization]]

[[def-harrison-one-form]]

[[pthm-local-hawking-circle-fields]]

[[pthm-horizon-invariant-one-form]]

[[pthm-harrison-denominator-positive]]

[[pthm-harrison-lorentzian-algebra]]

[[lem-killing-normal-boost-and-invariant-tensors]]

## Facts & Assumptions

[A1] The stated regular stationary vacuum model, maximal outer section, mass normalization and nontrivial restriction of $T$ to $S$ hold. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]] [[def-harrison-normalization]]

[F1] Near $S$, $K$ is Killing, commutes with $T$, vanishes on $S$, is a nonzero null normal off $S$ on both local branches, and has the stated signed surface gravities and positive normal boost rate. More precisely, the local-field supplier gives $K=\kappa\underline u L$ on $\mathcal H^+$ and $K=-\kappa u\underline L$ on $\mathcal H^-$, where $L,\underline L$ are nowhere-zero affine null normal generators, $L(\underline u)=\underline L(u)=1$, and the branch parameter zero sets are exactly $S$. The field $T$ is tangent to both branches and to their intersection $S$. [[pthm-local-hawking-circle-fields]] [[def-regular-stationary-vacuum-spacetime]] [[def-bifurcate-killing-horizon-data]]

[F2] The potential and one-form family are smooth and $K$-invariant near $S$. For all $q\in[0,1]$, $D_q>0$ on a common neighborhood of $S$. [[pthm-horizon-invariant-one-form]] [[pthm-harrison-denominator-positive]]

[F3] For a supplied Harrison one-form, define $A_qv=v+D_q^{-1}W_q(v)T$ and $4g_q=D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q$. If its stationarity, exterior-derivative and contraction conditions hold on the positive-denominator domain, the algebra supplier gives $g_q=(D_q/4)A_q^*g$, invertibility of $A_q$ and a smooth Lorentzian metric. These conditions for the present family will be verified below. [[def-stationary-lorentzian-data]] [[def-harrison-one-form]] [[pthm-harrison-lorentzian-algebra]]

[F4] The differential of the flow of $K$ fixes $TS$ pointwise and acts on the original normal plane by a boost with nonzero rate $\kappa$. [[lem-killing-normal-boost-and-invariant-tensors]]

[F5] For the local flow $\Phi_t$ of a smooth field $X$, $\Phi_0$ is the identity, $\Phi_{t+h}=\Phi_t\circ\Phi_h$ whenever defined, and $\Phi_{-t}$ is the inverse of $\Phi_t$ on its image. For a smooth tensor $Q$, $\mathcal L_XQ=\left.\frac d{dh}\right|_{h=0}\Phi_h^*Q$; pullback uses the inverse differential on contravariant slots and the differential on covariant slots. For smooth vector fields, $\mathcal L_XT=[X,T]$. [[math:def-local-and-global-flow]] [[math:def-lie-derivative-of-a-tensor-field]] [[math:thm-lie-derivative-of-a-vector-field-equals-the-lie-bracket]]

[F6] A smooth nondegenerate metric on a smooth four-manifold without boundary has a unique torsion-free compatible affine connection. Compatibility means $Xg_q(Y,Z)=g_q(\nabla^q_XY,Z)+g_q(Y,\nabla^q_XZ)$, and torsion freedom means $\nabla^q_XY-\nabla^q_YX=[X,Y]$. The adopted ZFC convention supplies the countable-choice hypothesis of this mathematical theorem. It applies to the tensor in F3 once that tensor is shown to be a smooth Lorentzian metric. [[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative]] [[post-stationary-vacuum-model]] [[def-stationary-lorentzian-data]]

[F7] The invariant-gauge supplier gives a pole $p\in S$ with $T_p=0$ and a smooth stationary real $W_0$ with $dW_0=4((f-1)F+\psi\star_gF)$ and $W_0(T)=d_0-D_0$, where $F=\tfrac12dT^\flat$, $D_0=|1-\sigma|^2$ and $d_0=D_0(p)$. Its family is $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, using this same potential and pole for every $q$. [[pthm-horizon-invariant-one-form]] [[def-harrison-one-form-family]]

[F8] Exterior differentiation on a smooth real one-form is $(d\alpha)(U,V)=U(\alpha(V))-V(\alpha(U))-\alpha([U,V])$. In particular, it is linear over real constants. [[math:def-exterior-derivative-by-the-invariant-vector-field-formula]]

## Proof

**Given:** The hypotheses and supplied fields in the Statement and Facts.

**Goal:** Prove the horizon, surface-gravity and bifurcation-surface assertions for every stated $q$.

1.1 Fix $q\in[0,1]$ and use the common pole and primitive in F7. Since $f(p)=0$, expansion of the modulus in the denominator definition gives $D_q=((1+q)-(1-q)f)^2+(1-q)^2\psi^2$ and $d_q=(1+q)^2+(1-q)^2\psi(p)^2>0$. Thus $d_q-D_q=(1-q)^2(d_0-D_0)+4q(1-q)f$. Evaluating the supplied family on $T$, with $T^\flat(T)=-f$, proves $W_q(T)=d_q-D_q$. By F8 and $dT^\flat=2F$, its exterior derivative is $dW_q=4(1-q)^2((f-1)F+\psi\star_gF)-8q(1-q)F=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$, exactly the required derivative equation in F3. [given, F3, F7, F8, algebra]

2.1 The local flow of $T$ preserves its generator: differentiate its flow law in the orbit parameter, as in F5. It preserves $g$ because $T$ is Killing; explicitly, the flow law and Lie-derivative definition give $\frac d{dt}\Psi_t^*g=\Psi_t^*(\mathcal L_Tg)=0$, where $\Psi_t$ denotes this flow. Hence it preserves $T^\flat$. Since $W_0$ is stationary, the family in F7 is stationary as well. It is a smooth real one-form on the common neighborhood in F2. Together with step 1.1, this verifies all three defining Harrison one-form conditions on $D_q>0$, for the same normalized potential and pole as in F3. The stationary Lorentzian data, $T_p=0$, the range $q\in[0,1]$ and positivity in F2 therefore match every hypothesis of the Lorentzian-algebra supplier. It gives invertibility of $A_q$, the pullback identity and smooth Lorentzian signature for the metric in F3. [given, F2, F3, F5, F7, step 1.1]

3.1 By the flow law and the tensor Lie-derivative definition in F5, $\frac d{dt}\Phi_t^*Q=\Phi_t^*(\mathcal L_KQ)$ on each local flow domain: differentiate $\Phi_{t+h}^*Q=\Phi_t^*(\Phi_h^*Q)$ at $h=0$. Thus $\mathcal L_KQ=0$ makes $\Phi_t^*Q=Q$ on the interval containing zero. In particular, $[K,T]=0$ implies $\Phi_t^*T=T$. Since $K$ commutes with $T$ and preserves $g$, it preserves $T^\flat$ and $f$. It also preserves $D_q$ and $W_q$, so the displayed formula gives $\mathcal L_Kg_q=0$. At $S$, $T$ is tangent to $S$. Hence $A_q$ maps $TS$ into itself; its invertibility makes its restriction to the two-dimensional $TS$ invertible. Consequently $g_q|_{TS}=(D_q/4)(A_q|_{TS})^*(g|_{TS})$ is positive definite. [given, F1, F2, F3, F5, step 2.1]

4.1 The flow carries its generator $K$ to itself, by differentiating the flow law in the orbit parameter. Since $\Phi_t^*W_q=W_q$ by F2 and step 3.1, $W_q(K)\circ\Phi_t=W_q(K)$. This scalar is therefore constant along the local $K$-flow and vanishes on $S$. Use the affine profiles in [F1]. Along a fixed generator on $\mathcal H^+$, $K=\kappa\underline u\,\partial_{\underline u}$, so its orbit has $\underline u(\tau)=\underline u(0)e^{\kappa\tau}$ and tends to that generator's point on $S$ as $\tau\to-\infty$. On $\mathcal H^-$ the profile $K=-\kappa u\,\partial_u$ gives $u(\tau)=u(0)e^{-\kappa\tau}$ and the limit as $\tau\to+\infty$. Restricting to short affine generator segments about $S$ keeps each approaching half-orbit in the common neighborhood. Smoothness therefore gives $W_q(K)=0$ on both branches. Since $T$ is tangent to each branch and $K$ is its $g$-normal, $g(K,T)=0$ there. [given, F1, F2, F5, step 3.1]

4.2 Let $\Phi=\Phi_t$ be a local $K$-flow map. It is a $g_q$-isometry by step 3.1. Write $(\Phi_*X)_{\Phi(p)}=d\Phi_pX_p$ and define a connection on its source by $\widehat\nabla_XY=\Phi_*^{-1}(\nabla^q_{\Phi_*X}(\Phi_*Y))$. The chain rule gives $(\Phi_*X)(h)\circ\Phi=X(h\circ\Phi)$ for every smooth target function $h$. Applying it twice gives $[\Phi_*X,\Phi_*Y](h)\circ\Phi=[X,Y](h\circ\Phi)$, hence $[\Phi_*X,\Phi_*Y]=\Phi_*[X,Y]$. The same chain rule transfers the affine-connection rules to $\widehat\nabla$. Torsion freedom of $\nabla^q$ and the bracket identity give $\widehat\nabla_XY-\widehat\nabla_YX=[X,Y]$. Since $\Phi^*g_q=g_q$, metric compatibility of $\nabla^q$ pulls back to $Xg_q(Y,Z)=g_q(\widehat\nabla_XY,Z)+g_q(Y,\widehat\nabla_XZ)$. Uniqueness in F6, applied on this open four-dimensional source, gives $\widehat\nabla=\nabla^q$, or $d\Phi(\nabla^q_XY)=\nabla^q_{\Phi_*X}(\Phi_*Y)$. [F5, F6, step 3.1]

5.1 Substitution in the metric formula yields $g_q(K,\cdot)=(D_q/4)g(K,\cdot)$ on either branch. Thus $K$ is tangent and normal there for $g_q$, and the nonzero-generator part is unchanged. The Lorentzian metric and nonzero normal show that each branch is null; together with step 3.1 this makes each a $g_q$-Killing horizon. Differentiating the scalar metric formula, every term involving $g(K,K)$, $g(K,T)$ or $W_q(K)$ as an undifferentiated factor vanishes on the branch. Therefore $d(g_q(K,K))=(D_q/4)d(g(K,K))$ there. The original signed equations give $-2\kappa g_q(K,\cdot)$ on $\mathcal H^+$ and $+2\kappa g_q(K,\cdot)$ on $\mathcal H^-$. At $S$ these equations are zero equations; the signed values are understood by their branch extensions. [given, F1, F3, step 3.1, step 4.1]

6.1 By F1 and F4, $\Phi$ fixes $S$ pointwise. Its isometry differential therefore preserves $TS$, its $g_q$-orthogonal complement and the corresponding normal projection. For tangent fields $X,Y$ along $S$, $B(X,Y)=(\nabla^q_XY)^\perp$ is independent of their extensions: a field vanishing on $S$ has zero covariant derivative in tangent directions there. The affine-connection rules make $B$ tensorial, since the term $X(a)Y$ is tangent and disappears under normal projection. Projecting the connection identity of step 4.2 thus gives $d\Phi B(X,Y)=B(d\Phi X,d\Phi Y)$. Its action on $TS$ is the identity. Its action on $TM|_S/TS$ has boost eigenvalues $e^{\pm\kappa t}$ by the original normal boost; the quotient identifies equivariantly with the $g_q$-normal plane because $S$ is $g_q$-spacelike. No nonzero normal vector is fixed by every such boost. Invariance therefore forces $B=0$, proving total geodesicity. Metric compatibility then gives $g_q(\nabla^q_XL,Y)=-g_q(L,\nabla^q_XY)=0$ for each null normal $L$ and tangent $X,Y$, so both null second fundamental forms vanish. [given, F1, F4, F6, step 3.1, step 5.1, step 4.2] ∎

## Source notes

The original article is cited for attribution of its local horizon-preservation claim. The argument above uses the stated suppliers and does not take that claim as a premise.

These explicit premises specify the generated conditional result. They are not asserted to follow from the original regularity definition alone, and are not attributed to the original article. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

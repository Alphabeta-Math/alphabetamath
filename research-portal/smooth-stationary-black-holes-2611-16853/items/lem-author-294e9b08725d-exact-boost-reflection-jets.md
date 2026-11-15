---
id: lem-author-294e9b08725d-exact-boost-reflection-jets
title: All-jet reflection parity from an exact local boost
kind: lemma
status: draft
origin: pipeline
domain: mathematics
proof_strategy: direct
deps:
  - physics:def-gr-killing-field
  - def-spacelike-maximal-hypersurface-data
  - math:def-ck-and-multi-index-notation-in-several-variables
  - math:def-pullback-of-a-covariant-tensor-field
  - math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor
  - math:prop-coordinate-formula-for-the-lie-bracket
  - math:thm-chain-rule-for-total-derivatives
  - math:lem-derivative-algebra-and-chain-rules
  - math:thm-clairaut-schwarz-mixed-partials
  - math:def-smooth-manifold
  - math:def-smooth-tensor-field
  - math:thm-tensor-transition-laws-define-a-smooth-vector-bundle
  - math:prop-smoothness-of-a-tensor-field-is-equivalent-to-smooth-coordinate-components
  - physics:def-gr-smooth-lorentzian-objects
dependency_roles:
  physics:def-gr-killing-field: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:def-ck-and-multi-index-notation-in-several-variables: mathematical-premise
  math:def-pullback-of-a-covariant-tensor-field: mathematical-premise
  math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor: mathematical-premise
  math:prop-coordinate-formula-for-the-lie-bracket: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
  math:thm-clairaut-schwarz-mixed-partials: mathematical-premise
  math:def-smooth-manifold: mathematical-premise
  math:def-smooth-tensor-field: mathematical-premise
  math:thm-tensor-transition-laws-define-a-smooth-vector-bundle: mathematical-premise
  math:prop-smoothness-of-a-tensor-field-is-equivalent-to-smooth-coordinate-components: mathematical-premise
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
dependency_level: 1
---

## Statement

Let $g$ be a smooth Lorentzian metric near a compact spacelike surface $S$ in a smooth four-manifold, let $B$ be a Killing field there, and let $T$ be a smooth vector field with $[B,T]=0$. Assume that every point of $S$ has an adapted coordinate patch $\phi:\mathcal O\to\Omega\subset\mathbb R^4$, with coordinates $(U,V,y^1,y^2)$, in which $S\cap\mathcal O=\{x\in\mathcal O:U(x)=V(x)=0\}$ and $B=\kappa(V\partial_V-U\partial_U)$ for the given constant $\kappa\ne0$. The tangential coordinates are local coordinates on $S$; a single chart containing all of $S$ is not required.

For any such patch put $w(u,v,z)=(-u,-v,z)$, $\Omega_0=\Omega\cap w(\Omega)$, $\mathcal O_0=\phi^{-1}(\Omega_0)$ and $S_0=S\cap\mathcal O_0$. Since $w$ fixes the plane $u=v=0$, $\mathcal O_0$ contains $S\cap\mathcal O$. Define $W=\phi^{-1}\circ w\circ\phi$ on $\mathcal O_0$. This is a smooth involutive diffeomorphism of $\mathcal O_0$ fixing $S_0$. All formulas below involving this $W$ are local to this patch.

For smooth tensor fields $H$ and $\widetilde H$ of the same type near $S_0$, write $j_{S_0}^\infty H=j_{S_0}^\infty\widetilde H$ when every component of $H-\widetilde H$ satisfies $\left.\partial_U^a\partial_V^b\partial_y^\gamma(H-\widetilde H)\right|_{S_0}=0$ for all nonnegative integers $a,b$ and all tangential multi-indices $\gamma$. Thus $j_{S_0}^\infty H$ denotes the equivalence class of the local field under equality of all these derivatives along $S_0$, rather than equality of the field on a neighborhood. The criterion is independent of the adapted coordinates, as justified below.

The pullbacks used here have the pointwise meanings $(W^*g)_x(v,w)=g_{W(x)}(dW_xv,dW_xw)$ and $(W^*T)_x=(dW_x)^{-1}T_{W(x)}$. For this involution $dW$ is the constant diagonal matrix with entries $-1,-1,1,1$, so both formulas define smooth fields on the chosen neighborhood.

On each such patch the infinite jets satisfy $j_{S_0}^\infty(W^*g)=j_{S_0}^\infty g$ and $j_{S_0}^\infty(W^*T)=j_{S_0}^\infty T$. Thus the metric and vector-field reflection parity holds locally near every point of the compact surface. If a smooth involution $\mathscr W$ of a neighborhood of $S$ is separately supplied and agrees with these patch reflections near every point of $S$, then $j_S^\infty(\mathscr W^*g)=j_S^\infty g$ and $j_S^\infty(\mathscr W^*T)=j_S^\infty T$. Compatibility or existence of such a common involution is not inferred from the boost formula. These are jet identities only; no reflection isometry of the original full neighborhood or global horizon generator is asserted.

## Statement references

[[math:def-smooth-manifold]]

[[math:def-smooth-tensor-field]]

[[physics:def-gr-smooth-lorentzian-objects]]

[[physics:def-gr-killing-field]]

[[def-spacelike-maximal-hypersurface-data]]

[[math:def-ck-and-multi-index-notation-in-several-variables]]

[[math:def-pullback-of-a-covariant-tensor-field]]

[[math:prop-coordinate-formula-for-the-lie-bracket]]

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted metric and vector-field jet identities, with their stated local scope.

[F1] On a time-oriented open subset, a Killing field satisfies $\mathcal L_Bg=0$. A time orientation is supplied by a smooth timelike vector field. The defining Killing equation involves only $B$ and $g$, so it is independent of that choice. Step 1.1 supplies such time orientations locally, without assuming a global one. [[physics:def-gr-killing-field]] [[physics:def-gr-smooth-lorentzian-objects]]

[F2] Use the smooth Lorentzian metric and induced-form conventions of the hypersurface-data definition; spacelike for $S$ means that $g|_{TS}$ is positive definite. No maximality condition is used. The multi-index derivatives in the inline definition of $j_S^\infty$ are derivatives of smooth component functions. [[def-spacelike-maximal-hypersurface-data]] [[math:def-ck-and-multi-index-notation-in-several-variables]]

[F3] For a covariant two-tensor, $(\mathcal L_Bg)_{ij}=B^k\partial_kg_{ij}+(\partial_iB^k)g_{kj}+(\partial_jB^k)g_{ik}$. For vector fields, $[B,T]^i=B^k\partial_kT^i-T^k\partial_kB^i$. Both formulas apply to the given smooth fields in these coordinates. [[math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor]] [[math:prop-coordinate-formula-for-the-lie-bracket]]

[F4] The covariant tensor pullback is evaluation on the differentials of the map. The vector pullback in the Statement is constructed locally by the inverse differential: $dW_x(W^*T)_x=T_{W(x)}$ determines it uniquely, and the constant invertible diagonal matrix $dW$ makes it smooth. This local construction needs no choice of global tangent-bundle charts. [[math:def-pullback-of-a-covariant-tensor-field]] [[math:thm-chain-rule-for-total-derivatives]]

[F5] The product and chain rules apply to smooth scalar component functions, and smooth mixed partial derivatives commute. The product rule is applied one coordinate at a time; the multivariable chain rule is applied to smooth coordinate changes. [[math:lem-derivative-algebra-and-chain-rules]] [[math:thm-chain-rule-for-total-derivatives]] [[math:thm-clairaut-schwarz-mixed-partials]]

[F6] A smooth manifold carries compatible smooth coordinate charts. A smooth type $(r,s)$ tensor field is a smooth section of its tensor bundle and has smooth coordinate components. On chart overlaps, the tensor transition laws express new components as finite sums of old components times smooth Jacobian or inverse-Jacobian factors, one for each tensor index. [[math:def-smooth-manifold]] [[math:def-smooth-tensor-field]] [[math:thm-tensor-transition-laws-define-a-smooth-vector-bundle]] [[math:prop-smoothness-of-a-tensor-field-is-equivalent-to-smooth-coordinate-components]]

## Proof

1.1 Fix any of the adapted patches in the Statement. The linear involution $w$ maps the open set $\Omega_0=\Omega\cap w(\Omega)$ onto itself and fixes every point of its intersection with the plane $u=v=0$. Its conjugate by the chart therefore gives the stated smooth involution $W$ and retains the entire surface portion $S\cap\mathcal O$. To apply F1, fix any point $p\in\mathcal O_0$. The Lorentzian signature supplies a vector $v\in T_pM$ with $g_p(v,v)<0$. Extend its coordinate components constantly to a smooth local field $N$ in this chart. The smooth component criterion in F6 makes $g(N,N)$ continuous; hence it remains negative on some open neighborhood of $p$. On that neighborhood $N$ is a smooth time orientation in the sense of F1. The given Killing hypothesis therefore yields $\mathcal L_Bg=0$ there. Since $p$ was arbitrary and the equation is independent of $N$, it holds throughout $\mathcal O_0$. No common time orientation, simultaneous choice of these fields, or $W$-invariance of their smaller neighborhoods is required. Now justify the jet convention on $S_0$. By F6, for a smooth change of adapted coordinates, each new component of a tensor difference is a finite sum of old components composed with the coordinate change and multiplied by smooth Jacobian or inverse-Jacobian entries, one for each tensor index. The vector transformation follows by applying the chain rule to the coordinate functions; the covariant transformation follows by evaluating on the coordinate tangent vectors. Multilinearity applies these transformations to each slot of a mixed tensor, giving exactly the transition factors in F6. Repeated product and chain rules show, by induction on derivative order, that each derivative of a new component at $S_0$ is a finite sum of old component derivatives at the same point multiplied by smooth coefficients. Consequently vanishing of every old derivative implies vanishing of every new derivative; applying the inverse coordinate change proves the converse. This proves coordinate independence and makes the stated jet equality an equivalence relation on local fields. [given, F1, F2, F4, F5, F6, algebra]

1.2 Put $D_{a,b,\gamma}=\partial_U^a\partial_V^b\partial_y^\gamma$ and $L=-U\partial_U+V\partial_V$. For any smooth component function $f$, repeated product differentiation gives $\left.D_{a,b,\gamma}(Lf)\right|_{S_0}=(-a+b)\left.D_{a,b,\gamma}f\right|_{S_0}$: in differentiating $U\partial_Uf$, the term still containing $U$ vanishes on $S_0$, the terms differentiating $U$ once sum to $aD_{a,b,\gamma}f$, and higher derivatives of $U$ vanish; the $V$ term gives $bD_{a,b,\gamma}f$ in the same way. The chain rule for the diagonal reflection also gives $\left.D_{a,b,\gamma}(f\circ W)\right|_{S_0}=(-1)^{a+b}\left.D_{a,b,\gamma}f\right|_{S_0}$. Tangential derivatives cause no additional terms because $W$ fixes $y$ and all coefficients of $L$ are independent of $y$. [F2, F5, algebra]

2.1 For a metric component carrying $p$ covariant $U$ indices and $q$ covariant $V$ indices, F1 and F3 give $0=(\mathcal L_Bg)_{ij}=\kappa(L-p+q)g_{ij}$. Since $\kappa\ne0$, step 1.2 yields $(-a+b-p+q)\left.D_{a,b,\gamma}g_{ij}\right|_{S_0}=0$. Thus a nonzero component derivative requires $-a+b-p+q=0$. The pullback formula in F4 contributes the factor $(-1)^{p+q}$ from the covariant indices; differentiating its component composition with $W$ contributes $(-1)^{a+b}$. Their total exponent $a+b+p+q=2(a+p)$ is even whenever the weight equation holds. Zero derivatives stay zero, so every metric component derivative agrees with its pullback derivative, including all tangential derivatives. By step 1.1 this proves $j_{S_0}^\infty(W^*g)=j_{S_0}^\infty g$. [F1, F2, F3, F4, step 1.1, step 1.2, algebra]

2.2 Use the given equation $[B,T]=0$ directly. F3 gives $(L+1)T^U=0$, $(L-1)T^V=0$ and $LT^A=0$ after division by $\kappa$. By step 1.2, a nonzero $U$ component derivative requires $-a+b+1=0$, and a nonzero $V$ component derivative requires $-a+b-1=0$. In each case $a+b$ is odd; the inverse differential in the local vector pullback contributes a further minus sign, so the total derivative sign is positive. A tangential component requires $a=b$, and its pullback has no extra index sign, so its total sign is positive as well. Zero derivatives remain zero. Hence every vector component derivative agrees and step 1.1 gives $j_{S_0}^\infty(W^*T)=j_{S_0}^\infty T$. Smooth boost-invariant functions may have different flat remainders in opposite wedges, so the argument concludes only equality of jets. [given, F2, F3, F4, step 1.1, step 1.2, algebra]

3.1 The patch was arbitrary, so steps 2.1 and 2.2 prove both local identities near every point of $S$. If $\mathscr W$ is supplied as in the Statement, its pullbacks equal those of the corresponding $W$ on a neighborhood of each point of $S$. Every derivative of each pullback difference consequently vanishes at every point of $S$ by the local identities. Coordinate independence from step 1.1 gives the stated global jet equalities for this supplied map. This argument does not assert agreement of distinct patch reflections without the stated compatibility assumption. [given, F4, step 1.1, step 2.1, step 2.2] ∎

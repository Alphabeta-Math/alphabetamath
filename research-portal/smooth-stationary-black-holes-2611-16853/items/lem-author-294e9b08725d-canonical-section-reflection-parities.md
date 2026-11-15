---
id: lem-author-294e9b08725d-canonical-section-reflection-parities
title: Reflection parities of canonical section data and stationary lapse–shift
kind: lemma
status: published
origin: pipeline
domain: mathematics
proof_strategy: direct
deps:
  - lem-author-294e9b08725d-exact-boost-reflection-jets
  - def-spacelike-maximal-hypersurface-data
  - physics:def-gr-metric-selected-connection
  - math:lem-derivative-algebra-and-chain-rules
  - math:thm-chain-rule-for-total-derivatives
dependency_roles:
  lem-author-294e9b08725d-exact-boost-reflection-jets: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
dependency_level: 2
---

## Statement

Assume the exact local boost and commuting-field hypotheses. In any adapted coordinate patch made $W$-invariant as in the reflection-jet supplier, let $\mathcal O_0$ be its domain, $S_0=S\cap\mathcal O_0$, $W(U,V,y)=(-U,-V,y)$ and $Q=\{U=V=r\}\cap\mathcal O_0$. Suppose this local canonical section is spacelike near $S_0$. Choose a continuous future unit normal $n$ and put $h=g|_Q$, $K(v,w)=g(\nabla_vn,w)$, $N=-g(T,n)$ and $X=T-Nn$. Let $R=W|_Q$, so $R(r,y)=(-r,y)$.

On this patch the infinite-jet parities are $j_{S_0}^\infty R^*h=j_{S_0}^\infty h$, $j_{S_0}^\infty R^*K=-j_{S_0}^\infty K$, $j_{S_0}^\infty R^*N=-j_{S_0}^\infty N$ and $j_{S_0}^\infty R^*X=j_{S_0}^\infty X$. Section-jet equality means equality of all component derivatives in $(r,y)$ along $r=0$, including all mixed normal and tangential orders. These conclusions hold locally near every point where the corresponding canonical section is supplied and spacelike. Here $K$ has the opposite sign from the library datum $k=-g(\nabla n,\cdot)$.

If, in addition, a common smooth spacelike canonical section $Q_{\mathrm{gl}}$ through all of $S$ and a smooth involution $R_{\mathrm{gl}}$ on its neighborhood of $S$ are supplied, and near every point of $S$ they agree with the local sections and reflections just specified, then all four parity identities hold along the whole $S$ for the induced data on $Q_{\mathrm{gl}}$ and pullback by $R_{\mathrm{gl}}$. This retains the whole-surface conclusion when those compatible data exist. Neither a common section nor compatibility of patch reflections is inferred from the boost formula alone, and no section beyond the supplied canonical neighborhoods is asserted.

## Statement references

[[lem-author-294e9b08725d-exact-boost-reflection-jets]]

[[def-spacelike-maximal-hypersurface-data]]

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[F1] On each adapted $W$-invariant patch the exact-boost supplier gives $j_{S_0}^\infty(W^*g)=j_{S_0}^\infty g$ and $j_{S_0}^\infty(W^*T)=j_{S_0}^\infty T$, using its pointwise pullback conventions. Its common-involution conclusion requires a separately supplied compatible involution; no gluing of different patch reflections is part of the local conclusion. [[lem-author-294e9b08725d-exact-boost-reflection-jets]]

[F2] A spacelike section has induced metric, future unit normal and second fundamental form; these are obtained from the metric and its first derivatives. [[def-spacelike-maximal-hypersurface-data]]

[F3] The Levi–Civita connection of a smooth Lorentzian metric is torsion-free and metric compatible. Its coordinate coefficients satisfy $\Gamma^a{}_{bc}=\tfrac12g^{ad}(\partial_bg_{dc}+\partial_cg_{bd}-\partial_dg_{bc})$, with $g^{ad}$ the inverse-metric entries. This formula uses nondegeneracy, without a positive-definiteness hypothesis. [[physics:def-gr-metric-selected-connection]]

[F4] The product, quotient and chain rules apply to smooth component functions; repeated application computes every finite-order derivative of a smooth composition. [[math:lem-derivative-algebra-and-chain-rules]] [[math:thm-chain-rule-for-total-derivatives]]

## Proof

**Given:** The data in the Statement. Fix one adapted patch; in steps 1.1–4.1 write $S$ for its subset $S_0$, and use $Q,R,W$ only on that patch.

**Goal:** Prove the four local section-jet parities and their conditional whole-surface version.

1.1 Use the $W$-invariant neighborhood and pullback conventions of F1. Write $A=dW=\operatorname{diag}(-1,-1,1,1)$, $\widetilde g=W^*g$ and $\widetilde T=W^*T$. Since $A$ is constant and $W(Q)=Q$, restricting the metric pullback to $TQ$ gives $\widetilde g|_{TQ}=R^*h$. Restriction to $Q=\{U=V=r\}$ differentiates component functions by $\partial_r=\partial_U+\partial_V$ and the tangential coordinate derivatives. Thus F1 gives equality of all section jets of $R^*h$ and $h$. Inverse-matrix entries are cofactors divided by the nonzero determinant; consequently repeated product and quotient rules also give equality of all ambient jets of $\widetilde g^{-1}$ and $g^{-1}$. [F1, F2, F4, algebra]

2.1 Put $\alpha=d(U-V)$, which annihilates $TQ$. For either metric $q=g$ or $q=\widetilde g$, the vector $q^{-1}\alpha$ is nonzero and orthogonal to the spacelike hyperplane $TQ$, so $q^{-1}(\alpha,\alpha)<0$. The two unit normals are therefore $\pm\nu(q)$, where $\nu(q)=q^{-1}\alpha/\sqrt{-q^{-1}(\alpha,\alpha)}$. Locally near each point of $S$, the given continuous future normal is $n=\sigma\nu(g)$ with a constant sign $\sigma\in\{1,-1\}$; hence it is smooth. Set $m_x=A n_{W(x)}$ along $Q$. Because $W^*\alpha=-\alpha$, the inverse-metric pullback formula gives $m=-\sigma\nu(\widetilde g)$. Step 1.1 and repeated differentiation of this smooth normalization imply $j_S^\infty m=-j_S^\infty n$ on $Q$. This is a jet identity and does not assert an actual reflection isometry. [F1, F2, F4, step 1.1, algebra]

2.2 Let $\varepsilon_U=\varepsilon_V=-1$ and $\varepsilon_A=1$, so $A^i{}_j=\varepsilon_i\delta^i{}_j$. The component pullback identities are $\widetilde g_{ij}(x)=\varepsilon_i\varepsilon_jg_{ij}(W(x))$ and $\widetilde g^{ij}(x)=\varepsilon_i\varepsilon_jg^{ij}(W(x))$. Substitute these into the Lorentzian Christoffel formula in F3 and differentiate the composition with $W$. Each derivative in coordinate $b$ contributes $\varepsilon_b$, and the two factors of each contracted sign cancel, giving $\widetilde\Gamma^a{}_{bc}(x)=\varepsilon_a\varepsilon_b\varepsilon_c\Gamma^a{}_{bc}(W(x))$. Independently, that same Christoffel formula and step 1.1 show that every derivative of $\widetilde\Gamma^a{}_{bc}-\Gamma^a{}_{bc}$ vanishes on $S$: an order-$k$ derivative of its formula uses only inverse-metric derivatives through order $k$ and metric derivatives through order $k+1$. No Riemannian connection theorem is being extended to indefinite signature. [F1, F3, F4, step 1.1, algebra]

3.1 For smooth ambient fields $v,w$, write $\widetilde v=A v\circ W$ and $\widetilde w=A w\circ W$. Expanding the connection derivative in components gives $(\widetilde\nabla_{\widetilde v}\widetilde w)^a=\widetilde v^b\partial_b\widetilde w^a+\widetilde\Gamma^a{}_{bc}\widetilde v^b\widetilde w^c=\varepsilon_a(v^b\partial_bw^a+\Gamma^a{}_{bc}v^bw^c)\circ W$ by step 2.2 and $\varepsilon_i^2=1$. Thus the reflection covariance needed here has been derived directly. Extend $n$ smoothly off $Q$ as allowed by F2 and apply this identity in tangent directions to $Q$. Together with the metric pullback it yields $(R^*K)_x(u,v)=\widetilde g_x(\widetilde\nabla_u m,v)$ for $u,v\in T_xQ$. In section coordinates this expression uses only the metric, connection coefficients, the normal and its first tangential derivatives. Steps 1.1, 2.1 and 2.2 therefore imply $j_S^\infty R^*K=-j_S^\infty K$. The sign comes from the normal reversal and requires no maximality condition. [F2, F3, F4, step 1.1, step 2.1, step 2.2, algebra]

4.1 The scalar lapse pullback is $R^*N=-\widetilde g(\widetilde T,m)|_Q$. By F1 and step 2.1 its section jet is that of $-g(T,-n)=g(T,n)=-N$. For the tangential shift, vector pullback along $R$ agrees with the restriction of the ambient pullback, since $dW$ maps $TQ$ to $TQ$. Therefore $R^*X=\widetilde T|_Q-(R^*N)m$ has the same section jet as $T-(-N)(-n)=T-Nn=X$. Together with steps 1.1 and 3.1 these are all four asserted parities, with precisely the stated local scope and the convention $K=-k$. [F1, F2, F4, step 1.1, step 2.1, step 3.1, algebra]

5.1 Now let $S$ again denote the whole surface and suppose the compatible data $Q_{\mathrm{gl}},R_{\mathrm{gl}}$ in the Statement are supplied. Their restrictions near each point agree with the local $Q,R$. The induced metrics, second fundamental forms and lapse–shift fields therefore agree there as well: they are computed from the same ambient metric and field, and the future unit normal is unique. Pullback by $R_{\mathrm{gl}}$ restricts to pullback by $R$. Steps 1.1–4.1 make every derivative of each corresponding parity difference vanish along $S_0$ in that patch. Since these patches cover $S$, all four global parity differences have zero infinite jet along $S$. This proves the retained whole-surface conclusion under its explicit compatibility hypotheses, without constructing a common section or identifying distinct patch reflections. [given, F1, F2, step 1.1, step 2.1, step 3.1, step 4.1] ∎

---
id: lem-author-9a15bef58785-rotational-rescaling-and-commutation
title: Constant combinations preserve horizon symmetries and normalize periods
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-killing-field
  - physics:thm-gr-killing-and-on-shell-matter-identities
  - math:def-lie-bracket-of-smooth-vector-fields
  - math:def-local-and-global-flow
  - def-circle-action-and-invariant-normal-data
  - physics:def-gr-smooth-lorentzian-objects
  - math:def-oriented-smooth-manifold-and-oriented-chart
  - math:def-integral-curve-of-a-vector-field
  - math:thm-chain-rule-for-differentials-of-smooth-maps
  - physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative
  - math:def-countable-choice
  - math:def-smooth-vector-field-as-a-tangent-bundle-section
  - math:prop-smoothness-of-a-vector-field-is-equivalent-to-smooth-coordinate-components
dependency_roles:
  physics:def-gr-killing-field: mathematical-premise
  physics:thm-gr-killing-and-on-shell-matter-identities: mathematical-premise
  math:def-lie-bracket-of-smooth-vector-fields: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  def-circle-action-and-invariant-normal-data: mathematical-premise
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  math:def-oriented-smooth-manifold-and-oriented-chart: mathematical-premise
  math:def-integral-curve-of-a-vector-field: mathematical-premise
  math:thm-chain-rule-for-differentials-of-smooth-maps: mathematical-premise
  physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-smooth-vector-field-as-a-tangent-bundle-section: mathematical-premise
  math:prop-smoothness-of-a-vector-field-is-equivalent-to-smooth-coordinate-components: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Assume $\mathrm{AC}_\omega$ for the canonical tangent-bundle smooth structure. Let $(M,g,N)$ be an oriented time-oriented smooth Lorentzian four-manifold of signature $(-,+,+,+)$, and let $U\subseteq M$ be open, with the restricted metric, orientation and time orientation. Let $T,K$ be smooth Killing fields for this same metric $g|_U$, with $[T,K]=0$, where the bracket is the Lie bracket. For real constants $a,b$, the field $Z=aT+bK$ is Killing for $g|_U$ and satisfies $[T,Z]=[K,Z]=0$.

For any local flow $\phi:\mathcal D\to U$ of $Z$, where $\mathcal D\subseteq\mathbb R\times U$, and any real constant $c\ne0$, define $\mathcal D_c=\{(t,p):(ct,p)\in\mathcal D\}$. Then $\psi:\mathcal D_c\to U$, $\psi(t,p)=\phi(ct,p)$, is a local flow of $cZ$. If $\phi$ is global on $U$ and has least positive common period $P$, then $\widehat Z=(P/(2\pi))Z$ has a global flow on $U$ with least positive common period $2\pi$. Here a common period $P>0$ means $\phi(s+P,p)=\phi(s,p)$ for every $s\in\mathbb R$ and $p\in U$; least means that no $q\in(0,P)$ has this property. This concerns the whole flow, allowing fixed points and individual orbits of shorter period.

If $Z=T+\lambda K$ with real constant $\lambda\ne0$, then $K=(Z-T)/\lambda$; this is a scale relation, not a universal normalization fixing the coefficient of $T$ in $K$.

## Statement references

[[physics:def-gr-killing-field]]

[[physics:thm-gr-killing-and-on-shell-matter-identities]]

[[math:def-lie-bracket-of-smooth-vector-fields]]

[[math:def-local-and-global-flow]]

[[def-circle-action-and-invariant-normal-data]]

[[physics:def-gr-smooth-lorentzian-objects]]

[[math:def-oriented-smooth-manifold-and-oriented-chart]]

[[math:def-integral-curve-of-a-vector-field]]

[[math:thm-chain-rule-for-differentials-of-smooth-maps]]

[[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative]]

[[math:def-countable-choice]]

[[math:def-smooth-vector-field-as-a-tangent-bundle-section]]

[[math:prop-smoothness-of-a-vector-field-is-equivalent-to-smooth-coordinate-components]]

## Facts & Assumptions

[F1] The Lorentzian metric and time orientation are the geometric data of the Lorentzian-manifold definition, and the orientation restricts from $M$ to $U$. Both fields are Killing for the single restricted metric. [[physics:def-gr-smooth-lorentzian-objects]] [[math:def-oriented-smooth-manifold-and-oriented-chart]] [[physics:def-gr-killing-field]]

[F2] On an oriented time-oriented smooth Lorentzian four-manifold, clause (a) of the Killing-characterization theorem gives $\mathcal L_Xg=0$ if and only if $\nabla_iX_j+\nabla_jX_i=0$, where indices are lowered using $g$ and $\nabla$ is its metric-selected connection. The same characterization applies on the open manifold $U$. [[physics:thm-gr-killing-and-on-shell-matter-identities]]

[F3] The Lie bracket is the commutator $[X,Y]f=X(Yf)-Y(Xf)$ on smooth functions; this formula gives bilinearity over real constants and skew symmetry. [[math:def-lie-bracket-of-smooth-vector-fields]]

[F4] A local flow has an open domain containing $\{0\}\times U$, interval time fibres, the identity at time zero, integral-curve time maps and the flow law whenever both sides are defined. An integral curve $\gamma$ of $X$ satisfies $\gamma'(t)=X_{\gamma(t)}$. The flow is global when its domain is $\mathbb R\times U$. [[math:def-local-and-global-flow]] [[math:def-integral-curve-of-a-vector-field]]

[F5] The differential chain rule for smooth maps gives $\frac{d}{dt}\gamma(ct)=c\gamma'(ct)$ for a smooth curve $\gamma$ and a real constant $c$, on the reparametrized interval. [[math:thm-chain-rule-for-differentials-of-smooth-maps]]

[F6] The least common period convention is that of a normalized periodic action: it concerns the entire global flow, rather than requiring every orbit to have the same least period. Only this period convention is used here, not the normal-averaging construction. [[def-circle-action-and-invariant-normal-data]]

[F7] The tensor-derivative theorem applies to a smooth symmetric nondegenerate metric on a smooth four-manifold without boundary, assuming $\mathrm{AC}_\omega$ for the canonical tangent-bundle smooth structure. It applies to $g|_U$ because the restricted Lorentzian metric is smooth and nondegenerate and $U$ is an open four-manifold without boundary. Clause (c), specialized to a smooth covector $\omega$, gives $\nabla_i\omega_j=\partial_i\omega_j-\sum_d\Gamma^d{}_{ji}\omega_d$, where $d$ runs over the four chart indices. This formula is linear in $\omega$ over real constants; its finite expansion uses no additional choice. [[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative]] [[math:def-countable-choice]] [[physics:def-gr-smooth-lorentzian-objects]]

[F8] Under the stated $\mathrm{AC}_\omega$ convention, a smooth vector field on $U$ is a smooth section of $TU\to U$. On each smooth chart, a vector field is smooth exactly when its coordinate components are smooth functions; this tests smoothness of the section in the induced tangent-bundle charts. [[math:def-smooth-vector-field-as-a-tangent-bundle-section]] [[math:prop-smoothness-of-a-vector-field-is-equivalent-to-smooth-coordinate-components]]

## Proof

**Given:** The hypotheses and data in the Statement.

**Goal:** Prove the Killing, commutation, local-flow rescaling and period conclusions, and the final scale relation.

1.1 For any real constants $r,s$, the pointwise combination $rT+sK$ takes its value at $p$ in $T_pU$. In every smooth chart on $U$, its components are $rT^i+sK^i$. The components $T^i,K^i$ are smooth by [F8], and every iterated partial derivative of $rT^i+sK^i$ is the same constant combination of the corresponding derivatives of $T^i,K^i$, hence is continuous. Thus [F8] makes $rT+sK$ a smooth section on each chart and therefore on $U$. In particular $Z=aT+bK$ and $cZ=(ca)T+(cb)K$ are smooth. Now write $T_j=g_{jk}T^k$, $K_j=g_{jk}K^k$ and $Z_j=aT_j+bK_j$. The covector component formula in [F7] gives $\nabla_iZ_j=a\nabla_iT_j+b\nabla_iK_j$ because $a,b$ are real constants. Hence $\nabla_iZ_j+\nabla_jZ_i=a(\nabla_iT_j+\nabla_jT_i)+b(\nabla_iK_j+\nabla_jK_i)=0$, since $T,K$ are Killing. The characterization in [F2] therefore gives $\mathcal L_Zg=0$ for the same restricted metric. [given, F1, F2, F7, F8, algebra]

2.1 The commutator formula gives $[T,T]=[K,K]=0$ and $[K,T]=-[T,K]=0$. Consequently $[T,Z]=a[T,T]+b[T,K]=0$ and $[K,Z]=a[K,T]+b[K,K]=0$. [given, F3, step 1.1, algebra]

2.2 The map $(t,p)\mapsto(ct,p)$ is a smooth invertible linear change of the time coordinate, so $\mathcal D_c$ is open, contains $\{0\}\times U$, and has interval time fibres $\{t:ct\in\mathcal D_p\}$. The map $\psi(t,p)=\phi(ct,p)$ is smooth and satisfies $\psi(0,p)=p$. By the integral-curve equation and the chain rule, $\partial_t\psi(t,p)=cZ_{\phi(ct,p)}=(cZ)_{\psi(t,p)}$. Whenever both sides are defined, the original flow law gives $\psi(t,\psi(s,p))=\phi(ct,\phi(cs,p))=\phi(c(t+s),p)=\psi(t+s,p)$. Thus all defining local-flow conditions hold on the stated domain. If $\mathcal D=\mathbb R\times U$, then $\mathcal D_c=\mathbb R\times U$. [given, F4, F5, step 1.1, algebra]

3.1 For the period conclusion take $c=P/(2\pi)>0$ in step 2.2. A positive number $q$ is a common period of $\psi$ precisely when $\phi(cs+cq,p)=\phi(cs,p)$ for all $s\in\mathbb R$ and $p\in U$. Since $c\mathbb R=\mathbb R$, this is equivalent to $cq$ being a common period of $\phi$. In particular $q=2\pi$ is a common period, while $0<q<2\pi$ would give a forbidden common period $0<cq<P$ of $\phi$. Hence $2\pi$ is least, in the whole-flow sense of [F6]. [given, F4, F6, step 2.2, algebra]

4.1 Finally $Z=T+\lambda K$ implies $\lambda K=Z-T$, so $K=(Z-T)/\lambda$ when $\lambda\ne0$. Under the separate period rescaling the relation becomes $\widehat Z=cT+c\lambda K$, which need not retain coefficient $1$ on $T$. Thus normalizing the period of $Z$ does not prescribe the scale of $K$ in a combination with fixed coefficient on $T$. This proves all claims. [given, step 1.1, step 2.1, step 3.1, algebra] ∎

---
id: lem-author-cea8e61dc3c6-kerr-future-horizon
title: A causal barrier identifies the future Kerr event horizon
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-cea8e61dc3c6-kerr-ingoing-extension
  - lem-author-cea8e61dc3c6-kerr-null-generator
  - lem-author-cea8e61dc3c6-kerr-outgoing-completion
  - math:def-absolutely-continuous-function
  - math:thm-a-lipschitz-function-after-an-absolutely-continuous-function-is-absolutely-continuous
  - math:lem-the-product-of-two-absolutely-continuous-functions-is-absolutely-continuous
  - math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions
  - math:def-countable-choice
  - math:def-dependent-choice
  - math:lem-derivative-algebra-and-chain-rules
  - math:thm-derivative-of-exponential
  - math:cor-mean-value-theorem
  - math:def-integrable-real-and-complex-functions-and-their-integrals
  - physics:def-causal-classification-of-lorentz-vectors
  - physics:def-time-orientation-and-future-causal-sets
  - physics:lem-gr-future-causal-classification-by-a-timelike-field
  - math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces
  - math:def-complete-ordered-field
  - math:lem-sup-epsilon
  - math:def-continuity-real
dependency_roles:
  def-author-cea8e61dc3c6-kerr-ingoing-extension: mathematical-premise
  lem-author-cea8e61dc3c6-kerr-null-generator: mathematical-premise
  lem-author-cea8e61dc3c6-kerr-outgoing-completion: mathematical-premise
  math:def-absolutely-continuous-function: mathematical-premise
  math:thm-a-lipschitz-function-after-an-absolutely-continuous-function-is-absolutely-continuous: mathematical-premise
  math:lem-the-product-of-two-absolutely-continuous-functions-is-absolutely-continuous: mathematical-premise
  math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-dependent-choice: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
  math:thm-derivative-of-exponential: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
  math:def-integrable-real-and-complex-functions-and-their-integrals: mathematical-premise
  physics:def-causal-classification-of-lorentz-vectors: mathematical-premise
  physics:def-time-orientation-and-future-causal-sets: mathematical-premise
  physics:lem-gr-future-causal-classification-by-a-timelike-field: mathematical-premise
  math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces: mathematical-premise
  math:def-complete-ordered-field: mathematical-premise
  math:lem-sup-epsilon: mathematical-premise
  math:def-continuity-real: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Saul A. Teukolsky, The Kerr Metric (arXiv:1410.2130v2)
      url: https://arxiv.org/pdf/1410.2130
      locator: §2, equations (2.1), (2.5)–(2.9), PDF pp. 2–3
      statement: The ingoing and Boyer–Lindquist Kerr metric forms and their
        coordinate transformation are displayed; the review identifies M as the
        mass and the roots of the radial function as null horizon candidates.
      hypotheses: Kerr metric in the stated ingoing and Boyer–Lindquist coordinate domains.
      reading_limits: Consulted the extracted PDF text of section 2, equations (2.1),
        (2.5)–(2.9), PDF pages 2–3 and adjacent discussion. Only coordinate and
        parameter background is used; no global causal-barrier or
        extremal-horizon proof is imported from this review. The argument below
        uses the declared mathematical suppliers.
dependency_level: 4
---

## Statement

Assume Countable Choice and Dependent Choice for the real-analysis inputs below. For the specified ingoing extension and the selected future null infinity, the points admitting a future causal curve to $\mathscr I^+$ are exactly $\{r>r_+\}$. Consequently the black hole region, defined as the complement of this causal past in $\mathcal K^{\mathrm{in}}$, is $\{0<r\leq r_+\}$ and its boundary is $H=\{r=r_+\}$. This is a global statement relative to this extension and this infinity; it does not identify different infinities in a maximal extension.

## Statement references

[[def-author-cea8e61dc3c6-kerr-ingoing-extension]]

[[lem-author-cea8e61dc3c6-kerr-null-generator]]

[[lem-author-cea8e61dc3c6-kerr-outgoing-completion]]

[[math:def-countable-choice]]

[[math:def-dependent-choice]]

[[physics:def-causal-classification-of-lorentz-vectors]]

[[physics:def-time-orientation-and-future-causal-sets]]

## Facts & Assumptions

[F1] The following exact suppliers supply the specified smooth ingoing extension, its temporal coordinate $\tau=v-r$ and future orientation, the future null normal $\nabla r$ on $H$, and the selected outgoing completion and escaping null curves: [[def-author-cea8e61dc3c6-kerr-ingoing-extension]] [[lem-author-cea8e61dc3c6-kerr-null-generator]] [[lem-author-cea8e61dc3c6-kerr-outgoing-completion]]

[F2] Absolute continuity is used on compact parameter intervals. A Lipschitz scalar function composed with an absolutely continuous scalar function is absolutely continuous, and products of absolutely continuous scalar functions are absolutely continuous. The fundamental theorem gives almost-everywhere differentiability, an integrable derivative and the identity $F(t)-F(s)=\int_s^t F^{\prime}(u)\,du$ for such functions, under Countable Choice and Dependent Choice. [[math:def-absolutely-continuous-function]] [[math:thm-a-lipschitz-function-after-an-absolutely-continuous-function-is-absolutely-continuous]] [[math:lem-the-product-of-two-absolutely-continuous-functions-is-absolutely-continuous]] [[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions]]

[F3] Adopt Countable Choice and Dependent Choice, in their supplied senses, precisely to satisfy the hypotheses of the absolutely continuous fundamental theorem in [F2]. No stronger choice principle is invoked by the local argument. [[math:def-countable-choice]] [[math:def-dependent-choice]]

[F4] The pointwise product and chain rules apply where the scalar factors are differentiable. The exponential is smooth with derivative equal to itself; the mean value theorem bounds its increments on each compact interval by a bound for its derivative. [[math:lem-derivative-algebra-and-chain-rules]] [[math:thm-derivative-of-exponential]] [[math:cor-mean-value-theorem]]

[F5] The real Lebesgue integral is defined by the integrals of the positive and negative parts; in particular an integrable function that is nonpositive almost everywhere has nonpositive integral. [[math:def-integrable-real-and-complex-functions-and-their-integrals]]

[F6] Use the nonzero timelike, null and causal vector classes and the future component/closed-cone conventions of [[physics:def-causal-classification-of-lorentz-vectors]] and [[physics:def-time-orientation-and-future-causal-sets]]. For a smooth time-oriented Lorentzian four-manifold with future timelike field $N$, its orthogonal complement is three-dimensional and positive definite, and a nonzero vector $V$ is future causal exactly when $g(V,V)\leq0$ and $g(V,N)<0$, equivalently when it lies in the future closed cone minus zero. These are the applicable conclusions of [[physics:lem-gr-future-causal-classification-by-a-timelike-field]], Statement 1–4. Zero is adjoined only in this item's curve convention, not in these suppliers' nonzero causal-vector class.

[F7] For the Euclidean inner product on $\mathbb R^3$, $|x\cdot y|\leq|x||y|$ by [[math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces]]. In particular $|x+y|^2\leq(|x|+|y|)^2$, so $|x+y|\leq|x|+|y|$ and $\bigl||x|-|y|\bigr|\leq|x-y|$. These consequences give the norm's Lipschitz bound used below.

[F8] Real continuity is used in its relative-domain epsilon-delta sense, and $\mathbb R$ is the complete ordered field, as in [[math:def-continuity-real]]. By [[math:def-complete-ordered-field]], every nonempty real set bounded above has a supremum. By [[math:lem-sup-epsilon]], if $c=\sup S$, then for every $\delta>0$ there is $s\in S$ with $c-\delta<s\leq c$. These are the real-analysis inputs to the local endpoint argument in step 4.1.

## Proof

**Given:** The mathematical Kerr interfaces of [F1] and analysis conventions [F2]–[F5], and mathematical cone and Euclidean inequalities [F6]–[F7]. A future causal curve here is a continuous curve whose coordinate components are locally absolutely continuous and whose tangent $V$ is either zero or a nonzero future causal vector in the sense of [F6] almost everywhere. Explicitly, for $N=-\nabla\tau$ from [F1], the nonzero alternative is $g(V,V)\leq0$ and $g(V,N)<0$; zero tangents and constant pieces are allowed. On each compact subinterval in a coordinate box we keep its original parameter $s$, and put $q(s)=\tau(\gamma(s))$ and $y(s)=r(\gamma(s))-r_+$. These are absolutely continuous, since $\tau=v-r$ and $r$ are coordinate-linear functions; finite linear combinations preserve the defining absolute-continuity estimates.

**Goal:** Establish the exact causal past of the selected infinity.

1.1 Fix a point of $H$ and a sufficiently small product coordinate box with compact closure and with $r_+$ in its radial interval. Put $N=-\nabla\tau$, $A=\sqrt{-g(N,N)}>0$ and $E_0=N/A$, a smooth future unit timelike field by [F1]. By [F6], $E_0^\perp$ is three-dimensional and positive definite. A smooth orthonormal spatial frame can be constructed locally as follows. Project the four coordinate vector fields $Z_a$ to $P_a=Z_a+g(Z_a,E_0)E_0$; these span $E_0^\perp$. Select three independent projections at the chosen point and shrink the box so they remain independent. Relabel them $P_1,P_2,P_3$ and successively set $W_j=P_j-\sum_{1\leq i<j}g(P_j,E_i)E_i$ and $E_j=W_j/\sqrt{g(W_j,W_j)}$. Positive definiteness makes each denominator positive; the resulting fields are smooth and orthonormal. Writing $V=tE_0+\sum_i x_iE_i$ gives $g(V,V)=-t^2+|x|^2$ and $g(V,N)=-At$. Thus [F6] says that the nonzero future causal vectors are exactly those with $t>0$ and $|x|\leq t$, and $d\tau(V)=-g(N,V)=At>0$. Consequently the vectors normalized by $d\tau(X)=1$ are exactly $X=A^{-1}(E_0+\sum_i u_iE_i)$ with $\sum_i u_i^2\leq1$. For two future causal vectors $U=tE_0+\sum_i x_iE_i$ and $V=sE_0+\sum_i z_iE_i$, [F7] gives $g(U,V)=-ts+x\cdot z\leq-ts+|x||z|\leq0$; the same inequality holds if either vector is zero. This establishes the required cone representation and pairing directly under the supplied conventions. [given, F1, F6, F7]

2.1 By the normalized representation in step 1.1 and [F7], the maximum radial component is $m=A^{-1}(dr(E_0)+\sqrt{\sum_i dr(E_i)^2})$: for $b=(dr(E_i))_{i=1}^3$, the maximum of $b\cdot u$ on $|u|\leq1$ is $|b|$, attained at $u=b/|b|$ when $b\ne0$, and at $u=0$ when $b=0$. This function is locally Lipschitz: its coefficients are smooth and the Euclidean norm is Lipschitz by [F7]; bounded first derivatives on a smaller compact coordinate box and the mean value theorem [F4] give a common local bound. On $H$, the future null normal in [F1] and the pairing inequality of step 1.1 give $dr(X)=g(\nabla r,X)\leq0$. Equality is attained by $X=\nabla r/d\tau(\nabla r)$ since this is a nonzero future null vector and $dr(\nabla r)=g(\nabla r,\nabla r)=0$ there. Thus $m=0$ on $H$. After shrinking the box, comparison with the point having the same other coordinates and $r=r_+$ gives $m\leq C|r-r_+|$ for a fixed $C\geq0$. Scaling a nonzero $V$ by $d\tau(V)$, and treating $V=0$ separately, yields $dr(V)\leq C|r-r_+|d\tau(V)$. Thus along every compact causal segment in this box, $q'\geq0$ and $y'\leq C|y|q'$ almost everywhere. No change of curve parameter or regularity of an inverse parameter map is used. [given, F1, F2, F4, F7, step 1.1]

3.1 Put $w(s)=\max\{y(s),0\}$. The positive-part map is $1$-Lipschitz, so [F2] makes $w$ absolutely continuous. Outside a null set, $y,w,q$ are differentiable and the inequalities of step 2.1 hold. At such a point with $y>0$ one has $w'=y'\leq Cwq'$; with $y<0$ one has $w'=0$. At a point where $y=0$, differentiability of $w$ and its minimum value $0$ imply $w'=0$, again giving the same inequality. Therefore $w'\leq Cwq'$ almost everywhere, including the zero level. On any fixed compact interval $[s_0,s_1]$ in the box, $q$ has compact range. By [F4], the function $t\mapsto e^{-C(t-q(s_0))}$ is Lipschitz on that range; [F2] therefore makes its composition with $q$ absolutely continuous, and also makes $z(s)=e^{-C(q(s)-q(s_0))}w(s)$ absolutely continuous. The pointwise rules [F4] now give $z'=e^{-C(q-q(s_0))}(w'-Cq'w)\leq0$ almost everywhere. By the fundamental theorem with the choice hypotheses [F3] and the integral convention [F5], $z(s)-z(s_0)=\int_{s_0}^s z'(u)\,du\leq0$ for every $s\in[s_0,s_1]$. If $y(s_0)=0$, then $z(s_0)=0$ and $z\geq0$, so $w=0$ on the interval. This proves the local outward barrier for the originally parametrized absolutely continuous curve, including its constant pieces. [given, F2, F3, F4, F5, step 2.1]

4.1 Suppose a future causal curve has a point with $r\leq r_+$ and a later point with $r>r_+$. Restrict to the compact parameter interval $[a,b]$ between these points, so $y(a)\leq0<y(b)$. By continuity and [F8], choose $0<\eta<b-a$ so that $y>0$ on $[b-\eta,b]$. The set $S=\{s\in[a,b]:y(s)\leq0\}$ is nonempty because $a\in S$, and it is bounded above by $b-\eta$. Thus [F8] gives $s_*=\sup S$ with $a\leq s_*\leq b-\eta<b$. If $y(s_*)>0$, continuity supplies $\delta>0$ such that $y(s)>0$ for $s\in[a,b]$ with $|s-s_*|<\delta$; the supremum approximation in [F8] supplies $s\in S$ with $s_*-\delta<s\leq s_*$, a contradiction. Hence $y(s_*)\leq0$. If $y(s_*)<0$, continuity gives some $h$ with $0<h<b-s_*$ and $y(s_*+h)<0$, contradicting that $s_*$ is an upper bound of $S$. Therefore $y(s_*)=0$. Every $s\in(s_*,b]$ has $y(s)>0$, since otherwise $s\in S$ would exceed its upper bound. Continuity of the curve puts $[s_*,s_*+\varepsilon]$, for some $0<\varepsilon<b-s_*$, in a coordinate box of step 1.1 about $\gamma(s_*)$. Step 3.1 forces $y\leq0$ there, contradicting the positivity just proved. Thus no future causal curve starting at or below $H$ reaches the exterior. This supremum argument does not assume that a first strictly exterior point exists. [given, F1, F8, step 1.1, step 3.1]

5.1 Every path ending at the chosen conformal infinity eventually lies in its collar, where $r$ is arbitrarily large. Hence a point with $r\leq r_+$ cannot reach that infinity by step 4.1. Every exterior point does reach it by the outgoing null curves of [F1]. Taking the complement gives $\{0<r\leq r_+\}$, whose boundary in the product manifold $\mathcal K^{\mathrm{in}}$ is $H=\{r=r_+\}$. This proves the event-horizon identification for $|a|<M$ and $|a|=M$ without assuming a bifurcate horizon or identifying different infinities in a maximal extension. [given, F1, step 4.1] ∎

## External input

The cited Kerr review supplies the coordinate and parameter background stated in its reference record; the result above is derived under the declared hypotheses and dependencies. The positive-part barrier and its integration are local deductions using the published mathematical suppliers, not an imported proof of this horizon statement.

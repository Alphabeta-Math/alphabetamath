---
id: lem-author-1f6675f2ec55-continuous-potential-comparison
title: Weak compact-domain comparison for continuous nonnegative potentials
kind: lemma
status: draft
origin: pipeline
domain: mathematics
proof_strategy: direct
deps:
  - math:def-axiom-of-choice
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-laplace-beltrami-operator-as-trace-of-the-hessian
  - math:def-riemannian-gradient
  - math:prop-coordinate-formula-for-riemannian-divergence
  - math:lem-the-riemannian-volume-density-is-coordinate-independent
  - math:lem-positive-part-is-an-admissible-weak-test-by-truncation
  - math:thm-smooth-partitions-of-unity-exist-on-manifolds
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
dependency_roles:
  math:def-axiom-of-choice: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-laplace-beltrami-operator-as-trace-of-the-hessian: mathematical-premise
  math:def-riemannian-gradient: mathematical-premise
  math:prop-coordinate-formula-for-riemannian-divergence: mathematical-premise
  math:lem-the-riemannian-volume-density-is-coordinate-independent: mathematical-premise
  math:lem-positive-part-is-an-admissible-weak-test-by-truncation: mathematical-premise
  math:thm-smooth-partitions-of-unity-exist-on-manifolds: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
dependency_level: 0
---

## Statement

Assume the Axiom of Choice. Let $(M,h)$ be a smooth Riemannian manifold and let $D\subset M$ be a relatively compact smooth domain, allowing $D$ to be disconnected, such that the closure of every connected component of $D$ meets $\partial D$. Let $V\ge0$ be real and continuous on $\overline D$ and let $w\in C^2(D)\cap C^1(\overline D)$ be real. Use the positive-divergence Laplace–Beltrami convention $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$, extended to $C^2$ functions by the metric trace of their Hessian. If $(\Delta_h-V)w\ge0$ in $D$ and $w\le0$ on $\partial D$, then $w\le0$ throughout $D$.

In particular, a nonnegative potential $V\in C^{2,\alpha}(\overline D)$, for $0<\alpha<1$, has the required continuity. Here this Hölder class is understood locally in smooth interior and boundary charts of $\overline D$: coordinate derivatives through order two extend continuously to the boundary, and on each smaller compact chart patch the second derivatives obey $|\partial_{ij}V(x)-\partial_{ij}V(y)|\le C|x-y|^\alpha$ for some finite $C$. No differentiability of the potential beyond continuity is required for the comparison.

## Statement references

[[math:def-axiom-of-choice]]

[[math:def-riemannian-metric-and-riemannian-manifold]]

[[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]]

[[math:def-riemannian-gradient]]

[[math:prop-coordinate-formula-for-riemannian-divergence]]

[[math:lem-the-riemannian-volume-density-is-coordinate-independent]]

[[math:lem-positive-part-is-an-admissible-weak-test-by-truncation]]

[[math:thm-smooth-partitions-of-unity-exist-on-manifolds]]

[[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

## Facts & Assumptions

**Given:** The hypotheses of the Statement.

**Goal:** Prove the comparison and its continuous-potential qualification.

[F1] The Axiom of Choice includes Countable Choice by restriction to countable families; these are the inherited assumptions of the truncation and partition suppliers. [[math:def-axiom-of-choice]]

[F2] For smooth inputs on a smooth Riemannian manifold, $(\operatorname{grad}_h f)^i=h^{ij}\partial_j f$, $\operatorname{div}_h X=m^{-1}\partial_i(mX^i)$, and $\Delta_h f=\operatorname{div}_h\operatorname{grad}_h f$, where $m=\sqrt{\det(h_{ij})}>0$. The volume density is $d\mu_h=m\,dx$ in these coordinates and is independent of the chart, without an orientability assumption. These are smooth-input formulas; their use for the present $C^2$ function is justified in step 1.1. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:def-riemannian-gradient]] [[math:prop-coordinate-formula-for-riemannian-divergence]] [[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]] [[math:lem-the-riemannian-volume-density-is-coordinate-independent]]

[F3] Under the declared choice assumptions, for a real $u\in H^1(\Omega)$ on a Euclidean open set and a real $k$, the positive-part truncation $(u-k)^+$ has weak gradient $D(u-k)^+=\mathbf1_{\{u>k\}}Du$ and zero gradient almost everywhere on $\{u\le k\}$. For $\eta\in C_c^\infty(\Omega)$, the nonnegative test $\eta^2(u-k)^+$ is admissible in a local divergence inequality with locally square-integrable source, and its gradient is $2\eta(u-k)^+D\eta+\eta^2D(u-k)^+$. [[math:lem-positive-part-is-an-admissible-weak-test-by-truncation]]

[F4] Under Countable Choice every open cover of a smooth manifold has a subordinate smooth partition of unity: the functions are nonnegative, their supports lie in the respective cover members, and their sum is one. Applying this to a finite cover gives a finite family of smooth functions. [[math:thm-smooth-partitions-of-unity-exist-on-manifolds]]

[F5] The Euclidean boundary-extension Hölder class $C^{2,\alpha}(\overline\Omega)$, with $0<\alpha<1$, requires continuous extensions of the coordinate derivatives through order two and a finite second-order Hölder seminorm. Applying this definition on smaller interior and boundary chart patches gives the local convention in the Statement; in particular the order-zero representative is continuous up to the boundary. [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

## Proof

**Given:** The hypotheses in the Statement and the conventions in Facts & Assumptions.

**Proof technique:** direct.

1.1 At an interior chart point $p$, replace $w$ by its quadratic Taylor polynomial $P$ in that chart. The metric dual of $dw$ has components $h^{ij}\partial_jw$; its first derivatives depend only on the derivatives of $w$ through order two. Consequently its covariant derivative and trace at $p$ agree with those of $\operatorname{grad}_h P$. Applying the smooth formulas of [F2] to $P$ proves $\Delta_hw=m^{-1}\partial_i(A^{ij}\partial_jw)$ at $p$, with $A^{ij}=mh^{ij}$, since the right side also depends only on that same two-jet. Thus the classical hypothesis gives $-\partial_i(A^{ij}\partial_jw)+mVw\le0$ throughout the chart. Multiply by any nonnegative $\varphi\in C_c^\infty$ of the chart and integrate. Integration of the derivative of the compactly supported $C^1$ product $A^{ij}\partial_jw\,\varphi$, first in the $i$th coordinate, gives $\int(A^{ij}\partial_jw\,\partial_i\varphi+mVw\varphi)\,dx\le0$ by the fundamental theorem of calculus. No derivative of $V$ is taken. [F2, given, algebra]

1.2 Fix $\epsilon>0$ and put $z=(w-\epsilon)^+$, $K=\{w\ge\epsilon\}$ and $K'=\{w\ge\epsilon/2\}$, taking these closed sets in $\overline D$. They are compact subsets of $D$ because the boundary values are nonpositive; in particular $\operatorname{supp}z\subseteq K$. If $K$ is empty there is nothing to prove for this $\epsilon$. Otherwise cover $K'$ by finitely many relatively compact interior coordinate balls $U_1,\ldots,U_N$, whose closures lie in larger interior charts, and set $U_0=D\setminus K'$. By [F1] and [F4], this finite open cover of the smooth manifold $D$ has a subordinate partition $\phi_0,\ldots,\phi_N$. Define $\eta_j=\phi_j/(\sum_{\ell=0}^N\phi_\ell^2)^{1/2}$. The denominator is positive everywhere. Each $\eta_j$ is smooth, $\sum_{j=0}^N\eta_j^2=1$, and, for $j\ge1$, $\operatorname{supp}\eta_j$ is compactly contained in $U_j$. On the open neighborhood $\{w>\epsilon/2\}$ of $K$, $\eta_0=0$, so $\sum_{j=1}^N\eta_j^2=1$ and $\sum_{j=1}^N2\eta_j\,d\eta_j=0$ there. [F1, F4, given, construct]

2.1 On each $U_j$, $j\ge1$, the coordinate representative of $w$ is in $H^1$: $w$ and its first derivatives are bounded on its compact closure in the larger chart, and the coordinate ball has finite measure. The source $-mVw$ is locally bounded and hence locally square integrable. Thus [F3] extends the weak inequality of step 1.1 to the nonnegative test $\eta_j^2z$, with $Dz=\mathbf1_{\{w>\epsilon\}}Dw$ and $D(\eta_j^2z)=\eta_j^2Dz+2\eta_jzD\eta_j$. The coefficients are bounded on the test support. Rewrite these chart integrals using the density in [F2] and sum over $j=1,\ldots,N$. Since $z$ and $Dz$ vanish off $K$ up to null sets, the two sum identities of step 1.2 cancel the cross terms and give $\int_D|\nabla z|_h^2\,d\mu_h+\int_DVwz\,d\mu_h\le0$. [F1, F2, F3, step 1.1, step 1.2, algebra]

3.1 Both integrands in step 2.1 are nonnegative, since $V\ge0$ and $w>\epsilon$ wherever $z>0$. Hence $\nabla z=0$ almost everywhere. On the open set $\{w>\epsilon\}$, [F3] identifies this gradient with that of the $C^2$ function $w$. Continuity of $\nabla w$ and positivity of the volume density therefore give $\nabla w=0$ everywhere on that open set. On every coordinate ball contained in it, the fundamental theorem of calculus along segments shows that $w$ is constant. Thus $w=c>\epsilon$ on each connected component $G$ of $\{w>\epsilon\}$. If $p$ is in the closure of $G$ relative to $D$, continuity gives $w(p)=c>\epsilon$; a small connected coordinate ball about $p$ in $\{w>\epsilon\}$ meets $G$, so $p\in G$. Thus $G$ is both open and closed in $D$ and is a whole connected component of $D$. Its closure meets $\partial D$, where continuity would give $w=c>\epsilon$, contrary to the boundary condition. Hence no such $G$ exists, and $w\le\epsilon$. Letting $\epsilon$ decrease to zero proves $w\le0$. The empty-domain case is vacuous; a nonempty zero-dimensional domain cannot satisfy the component-boundary hypothesis. Finally [F5] gives the stated $C^{2,\alpha}(\overline D)$ consequence. Only local boundedness and nonnegativity of the continuous potential were used in the argument. [F2, F3, F5, step 1.2, step 2.1, given, algebra] ∎

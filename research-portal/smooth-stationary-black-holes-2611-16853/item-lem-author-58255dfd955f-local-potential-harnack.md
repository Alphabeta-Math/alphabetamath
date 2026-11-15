---
title: Multiplicative interior Harnack for geometric Schrödinger solutions
status: draft
research_item: lem-author-58255dfd955f-local-potential-harnack
dependency_level: 1
---

## Prerequisites

- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)
- [math:def-riemannian-gradient](https://alphabetamath.cc/item/def-riemannian-gradient)
- [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:thm-divergence-theorem-for-bounded-c-one-euclidean-domains](https://alphabetamath.cc/item/thm-divergence-theorem-for-bounded-c-one-euclidean-domains)
- [math:def-borel-and-lebesgue-measurable-function-on-rn](https://alphabetamath.cc/item/def-borel-and-lebesgue-measurable-function-on-rn)
- [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [thm-author-58255dfd955f-bounded-potential-harnack-input](item-thm-author-58255dfd955f-bounded-potential-harnack-input)


## Statement

Work in ZFC. Let $n\ge1$ be an integer, let $(\mathcal N,h)$ be a smooth $n$-dimensional Riemannian manifold, and identify an open coordinate neighborhood with the Euclidean ball $B_r(x_0)\subset\mathbb R^n$, where $r>0$. All balls and coefficient norms below are in these coordinates. The Laplace–Beltrami operator has sign convention $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$, equivalently the metric trace of the Levi-Civita Hessian, using the same pointwise expression for $C^2$ functions. Let $V:B_r(x_0)\to[0,\infty)$ be bounded, with no measurability assumption, and let $u\in C^2(B_r(x_0);\mathbb R)$ be nonnegative and satisfy $(\Delta_h-V)u=0$ pointwise. Put $m=\sqrt{\det(h_{ij})}$, $A=(mh^{ij})$ and $q=mV$. Suppose $\lambda>0$, $M<\infty$ and $Q\ge0$ satisfy $\xi^TA(x)\xi\ge\lambda|\xi|^2$, $\|A(x)\|_{\mathrm{op}}\le M$ and $q(x)\le Q$ at every point, for all $\xi\in\mathbb R^n$. Then

$$\sup_{B_{r/2}(x_0)}u\le C\inf_{B_{r/2}(x_0)}u,$$

where $C\ge1$ depends only on $n$, $M/\lambda$ and $r^2Q/\lambda$. This includes $n=1$ and the identically zero solution.

## Facts & Assumptions

**Given:** The pointwise data and bounds in the Statement. Work in ZFC, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice), as required by the analytic supplier and its formulation inputs; no additional choice is used by the local coordinate calculation.

[F1] The Riemannian metric is as in [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold). The smooth-function gradient formula is [math:def-riemannian-gradient](https://alphabetamath.cc/item/def-riemannian-gradient), the smooth-vector-field divergence density formula is [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence), and the trace-of-Hessian Laplacian with the stated sign is [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian). Their extension to the $C^2$ function in this item is justified in step 1.1; no exterior topology or smoothness of $V$ is assumed.

[F2] Use the affine-map case of [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) to differentiate $T_s(y)=x_0+sy$ and its compositions, where $0<s<r$ and $DT_s=sI$. The rescaling is calculated pointwise below, so it does not require a substitution theorem for a nonmeasurable integrand.

[F3] Measurability means the Borel/Lebesgue convention of [math:def-borel-and-lebesgue-measurable-function-on-rn](https://alphabetamath.cc/item/def-borel-and-lebesgue-measurable-function-on-rn), with coefficients extended by zero outside their open balls. Use the real Sobolev space from [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm). For $d\ge2$, [math:thm-divergence-theorem-for-bounded-c-one-euclidean-domains](https://alphabetamath.cc/item/thm-divergence-theorem-for-bounded-c-one-euclidean-domains) applies to $C^1$ vector fields on a neighborhood of a closed Euclidean ball. In particular a field vanishing near its boundary has zero integrated divergence. This will supply both the weak derivative identities and the weak equation in step 5.1.

[F4] [thm-author-58255dfd955f-bounded-potential-harnack-input](item-thm-author-58255dfd955f-bounded-potential-harnack-input) supplies the homogeneous unit-ball Harnack theorem in dimension $d\ge2$: a real measurable symmetric matrix $H\ge I$ with $\sum_{i,j}|H^{ij}|\le\Lambda$ and a measurable potential $0\le b\le K$ give $\operatorname{ess\,sup}_{B_{1/2}}w\le C_H(d,\Lambda,K)\operatorname{ess\,inf}_{B_{1/2}}w$ for every nonnegative real $W^{1,2}(B_1)$ weak solution of $-\operatorname{div}(H\nabla w)+bw=0$. Its weak identity is against all real $C_c^\infty(B_1)$ tests with Lebesgue integrals. The supplier records the independent Simon source, its exact coefficient specialization and reading limits; the underlying iteration theorem is imported, not reproved here.

## Proof

**Given:** The data of the Statement and [F1]–[F4].

**Goal:** The stated multiplicative comparison with only the displayed parameter dependence.

**Proof technique:** direct.

1.1 At any coordinate point $p$, replace $u$ by the quadratic polynomial having its value, first derivatives and second derivatives at $p$. The metric trace of the Levi-Civita Hessian uses only these data: in coordinates its Hessian entries are $\partial_{ij}u-\Gamma^k_{ij}\partial_k u$. Apply the smooth formulas in [F1] to this polynomial. The coordinate expression $m^{-1}\partial_i(mh^{ij}\partial_j u)$ also uses only these same derivatives through order two, so the polynomial and $u$ give equal values on both sides at $p$. Thus $\Delta_hu=m^{-1}\partial_i(A^{ij}\partial_j u)$ throughout the ball at the stated $C^2$ regularity. Multiplying the pointwise equation by $m$ gives $\partial_i(A^{ij}\partial_j u)=qu$, with repeated indices summed. Here $A$ is smooth and symmetric. [given, F1, algebra]

2.1 Set $D=\{x:u(x)>0\}$, an open set, and define $q_*(x)=m(x)\Delta_hu(x)/u(x)$ on $D$ and $q_*(x)=0$ off $D$. On $D$ this coefficient is continuous and equals $q$ by the given equation; hence $0\le q_*\le Q$ everywhere. Its zero extension is Borel: on the open set $D$ it is continuous, and on the complementary closed set it is constant, so preimages of open subsets of $\mathbb R$ are Borel. At points where $u=0$, the pointwise equation gives $\Delta_hu=Vu=0$. Consequently $q_*u=qu=m\Delta_hu$ everywhere, including those points, and $-\operatorname{div}(A\nabla u)+q_*u=0$ pointwise. In particular $q_*u$ is continuous even though $q_*$ need not be continuous. This construction includes $u\equiv0$ and makes no assertion that the originally given $V$ is measurable. [given, F3, step 1.1, algebra]

3.1 Fix $0<s<r$ and set $v(y)=u(T_s(y))$, $\widetilde A(y)=A(T_s(y))/\lambda$ and $\widetilde b(y)=s^2q_*(T_s(y))/\lambda$ on $B_1\subset\mathbb R^n$. The chain rule gives $\partial_{y_j}v=s(\partial_{x_j}u)\circ T_s$ and $\operatorname{div}_y(\widetilde A\nabla_yv)=(s^2/\lambda)(\operatorname{div}_x(A\nabla_xu))\circ T_s$. Thus $-\operatorname{div}_y(\widetilde A\nabla_yv)+\widetilde b v=0$ pointwise. The matrix $\widetilde A$ is smooth, symmetric and at least $I$, and $|\widetilde A^{ij}|\le M/\lambda$. The potential is Borel and satisfies $0\le\widetilde b\le K:=r^2Q/\lambda$, with this fixed bound independent of $s$. Because $\overline{B_s(x_0)}$ is compactly contained in $B_r(x_0)$, $v$ and $\widetilde A$ are respectively $C^2$ and smooth on a neighborhood of $\overline{B_1}$. [F2, F3, step 2.1, given, algebra]

4.1 If $n\ge2$, put $d=n$, $w=v$, $H=\widetilde A$ and $b=\widetilde b$. If $n=1$, put $d=2$ and, on the two-dimensional unit disk, set $w(z_1,z_2)=v(z_1)$, $H(z_1,z_2)=\operatorname{diag}(\widetilde A(z_1),1)$ and $b(z_1,z_2)=\widetilde b(z_1)$. In this latter case $\partial_2w=0$ and the equation of step 3.1 gives $-\partial_1(\widetilde A(z_1)v'(z_1))+b(z_1,z_2)w(z_1,z_2)=0$, exactly $-\operatorname{div}(H\nabla w)+bw=0$ on the disk. In either case $d\ge2$, $w\ge0$, $w$ is $C^2$ near the closed disk or ball, $H$ is smooth symmetric with $H\ge I$, and $b$ is Borel with $0\le b\le K$. Since $M/\lambda\ge1$, the entrywise bound $\sum_{i,j}|H^{ij}|\le d^2M/\lambda$ holds in both cases; for the lifted matrix its sum is at most $M/\lambda+1$. No one-dimensional version of the imported theorem is assumed. [step 3.1, given, algebra]

5.1 The function $w$ and its classical first derivatives are bounded on $B_1\subset\mathbb R^d$ and therefore square integrable. For every real $\varphi\in C_c^\infty(B_1)$, the field $\varphi w e_i$ is $C^1$ and vanishes near the boundary. Applying [F3] to its divergence gives $\int w\partial_i\varphi=-\int(\partial_iw)\varphi$, so these classical derivatives are weak derivatives and $w\in W^{1,2}(B_1)$. Likewise the field $\varphi H\nabla w$ is $C^1$ and vanishes near the boundary. Its divergence integrates to zero; the pointwise equation in step 4.1 and the product rule give $\int_{B_1}(H\nabla w\cdot\nabla\varphi+bw\varphi)=0$. The products are measurable and integrable; indeed $bw=\operatorname{div}(H\nabla w)$ is continuous. These are precisely the weak-solution hypotheses of [F4]. Therefore [F4] gives the comparison on $B_{1/2}\subset\mathbb R^d$ with the same constant $C_H(d,d^2M/\lambda,K)$ for every $s$. [F3, F4, step 4.1, algebra]

6.1 Since $w$ is continuous, its essential supremum and infimum on the open half-ball equal its ordinary supremum and infimum: any strict pointwise violation of an essential bound persists on a nonempty open ball, which has positive Lebesgue measure. For $n\ge2$ this directly gives $v(y)\le Cv(y')$ for all $y,y'\in B_{1/2}$. For $n=1$, restrict the resulting pointwise comparison to the pairs $(y,0),(y',0)$ in the half-disk; these range over all $y,y'\in(-1/2,1/2)$. Thus in all cases $u(x)\le Cu(x')$ for $x,x'\in B_{s/2}(x_0)$, where $C=\max\{1,C_H(d,d^2M/\lambda,r^2Q/\lambda)\}$ depends only on the asserted parameters. Every pair in $B_{r/2}(x_0)$ lies in some such smaller half-ball, so the same pairwise comparison holds throughout $B_{r/2}(x_0)$. Taking the supremum in $x$ and then the infimum in $x'$ proves the Statement. [step 5.1, step 4.1, given, algebra] ∎

---
id: lem-author-423fe0348a31-chart-sobolev-comparison
title: Weak first derivatives and Riemannian chart norm comparison
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice
  - math:def-sobolev-space-wkp-and-its-norm
  - math:def-weak-derivative-of-a-locally-integrable-function
  - math:def-riemannian-volume-density
  - math:def-countable-choice
  - math:lem-weak-derivatives-are-unique-almost-everywhere
  - math:cor-c-one-change-of-variables-for-l-one-functions
  - math:prop-riemannian-metrics-induce-metrics-on-dual-tensor-and-exterior-bundles
  - math:def-essential-supremum-with-respect-to-a-measure
dependency_roles:
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice: mathematical-premise
  math:def-sobolev-space-wkp-and-its-norm: mathematical-premise
  math:def-weak-derivative-of-a-locally-integrable-function: mathematical-premise
  math:def-riemannian-volume-density: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:lem-weak-derivatives-are-unique-almost-everywhere: mathematical-premise
  math:cor-c-one-change-of-variables-for-l-one-functions: mathematical-premise
  math:prop-riemannian-metrics-induce-metrics-on-dual-tensor-and-exterior-bundles: mathematical-premise
  math:def-essential-supremum-with-respect-to-a-measure: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Assume Countable Choice. Let $(R,k)$ be a smooth Riemannian manifold of dimension $n\ge0$, let $x:U\to\Omega\subseteq\mathbb R^n$ be an interior coordinate chart with compact closure in $R$, and fix a compact set $K\subset U$. For $n\ge1$, let $u\in W^{1,1}(\Omega;\mathbb R)$ vanish almost everywhere outside $x(K)$, and define $f=u\circ x$ on $U$, extended by zero to $R$. Here $u_i=D_i u$ are weak coordinate derivatives, $df=\sum_i(u_i\circ x)\,dx^i$ on $U$, and $df=0$ off $U$. These formulas define an almost-everywhere covector field independent of coordinates.

There are constants $0<c\le C<\infty$, depending on $K$, $x$, and $k$ but not on $u$, such that
$$c\|u\|_{W^{1,1}(\Omega)}\le\int_R(|f|+|df|_k)\,dV_k\le C\|u\|_{W^{1,1}(\Omega)},\qquad \|u\|_{W^{1,1}(\Omega)}=\int_\Omega\left(|u|+\sum_{i=1}^n|u_i|\right)\,dx.$$
The measure $dV_k$ is the Riemannian volume density, and $|df|_k$ is the dual metric norm. Essential supremum norms, possibly infinite, agree under the coordinate map, using Lebesgue measure on $\Omega$ and $dV_k$ on $U$. For any specified pointwise representative, its pointwise supremum on $U$ agrees with that of its coordinate expression on $\Omega$; this assertion does not identify representatives that differ on null sets.

Every real locally Lipschitz scalar function on $R$ has almost-everywhere classical coordinate derivatives equal to its weak derivatives, which assemble to the same coordinate-independent differential. More generally, the coordinate weak derivatives of a function that is $W^{1,1}_{\mathrm{loc}}$ in charts obey $d(\chi f)=\chi\,df+f\,d\chi$ for every smooth cutoff $\chi$. In particular this applies to the compactly supported functions above and to locally Lipschitz functions. For continuous representatives the pointwise and essential suprema of the absolute value also agree.

In dimension zero use the local convention $W^{1,1}(\mathbb R^0;\mathbb R)=\mathbb R$ with norm $|u|$, no first-derivative components, and volume one at the chart point; on the empty coordinate domain use the zero space. Then the same conclusions hold, with $df=0$ and $c=C=1$.

## Facts & Assumptions

[F1] The coordinate metric matrix $G=(k_{ij})$ is smooth and positive definite. Its inverse gives the dual metric: for a covector with component column $a$, $|a|_k^2=a^TG^{-1}a$. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:prop-riemannian-metrics-induce-metrics-on-dual-tensor-and-exterior-bundles]]

[F2] The Riemannian volume density in a chart is $dV_k=\rho\,dx$, where $\rho=\sqrt{\det G}$ is smooth and positive; in dimension zero the empty determinant is one. [[math:def-riemannian-volume-density]]

[F3] For positive dimension, weak first derivatives satisfy $\int u\,\partial_i\varphi\,dx=-\int u_i\varphi\,dx$ for every $\varphi\in C_c^\infty(\Omega)$. Under Countable Choice they are unique as almost-everywhere classes. The space $W^{1,1}$ requires $u$ and every $u_i$ to be integrable, with the sum norm displayed in the Statement; the local space requires this on relatively compact open subsets. [[math:def-weak-derivative-of-a-locally-integrable-function]] [[math:lem-weak-derivatives-are-unique-almost-everywhere]] [[math:def-sobolev-space-wkp-and-its-norm]]

[F4] Assuming Countable Choice, a real locally Lipschitz function on an open subset of $\mathbb R^n$, $n\ge1$, is differentiable almost everywhere, with measurable weak partial derivatives, and $|Du|\le L$ almost everywhere wherever it is $L$-Lipschitz. Only this calculus conclusion of the supplier is used. [[math:lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice]]

[F5] Assuming Countable Choice, a $C^1$ diffeomorphism $T:A\to B$ of Euclidean open sets satisfies $\int_B h(y)\,dy=\int_A h(T(z))|\det DT(z)|\,dz$ for $h\in L^1(B)$. [[math:cor-c-one-change-of-variables-for-l-one-functions|Change of variables for integrable functions]]

[F6] For a real measurable function $h$ on a measure space $(X,\mathcal A,\mu)$, its essential supremum norm is $\|h\|_{\infty,\mu}=\inf\{M\in[0,\infty]:|h|\le M\text{ }\mu\text{-almost everywhere}\}$. [[math:def-essential-supremum-with-respect-to-a-measure]]

[A1] Countable Choice is assumed for the Sobolev, weak-derivative uniqueness, Lipschitz-calculus, and Lebesgue change-of-variables suppliers; no stronger choice principle is asserted here. [[math:def-countable-choice]]

## Proof

**Given:** The chart, compact set, metric, function class, and Countable Choice in the Statement.

**Goal:** Establish the coordinate-independent weak differential, norm comparisons, and stated calculus in all dimensions.

1.1 Suppose first that $n\ge1$. We establish the coordinate transformation of weak derivatives locally. Let $T:A\to B$ be a smooth coordinate transition, write $z$ for the coordinates on $A$, put $J=|\det DT|$, and for a fixed $j$ set $b_i=J(DT^{-1})_{ij}$, where $DT^{-1}$ denotes the inverse matrix at $z$. Then $\sum_i\partial_i b_i=0$: on each connected component the sign of $\det DT$ is constant, and $b_i$ is that sign times the $(j,i)$ cofactor of $DT$. In its determinant expansion, differentiating a factor $\partial_\ell T_a$ in the cofactor for index $i$ pairs with the term differentiating $\partial_i T_a$ in the cofactor for index $\ell$; the signs are opposite and mixed second partials are equal. All terms cancel (for $n=1$ the cofactor is the constant one). For a coordinate function $u\in W^{1,1}_{\mathrm{loc}}(A)$, set $v=u\circ T^{-1}$. Change of variables on compact subsets makes $v$ and the proposed derivatives locally integrable. For $\varphi\in C_c^\infty(B)$, the smooth functions $b_i(\varphi\circ T)$ have compact support in $A$. The ordinary chain rule gives $\sum_i b_i\partial_i(\varphi\circ T)=J(\partial_j\varphi)\circ T$. Applying the weak identity to these tests, summing, and using the zero divergence just proved gives $$\int_B v\,\partial_j\varphi\,dy=-\int_B\left(\sum_i u_i(T^{-1}(y))\,\partial_j(T^{-1})_i(y)\right)\varphi(y)\,dy.$$ Thus $v_j=\sum_i(u_i\circ T^{-1})\partial_j(T^{-1})_i$ weakly. Uniqueness identifies this with any other weak derivative, so the covector expressions agree on overlaps. Applying change of variables to null-set indicators, with $J>0$, and then to the inverse transition shows that both directions preserve null sets; hence these statements are well defined for almost-everywhere classes. [F3, F5, A1, algebra]

2.1 For the compactly supported $u$ of the Statement, its restriction to $\Omega\setminus x(K)$ is zero almost everywhere. Its weak derivatives there are zero by the test identity and uniqueness. Therefore $u_i=0$ almost everywhere off $x(K)$. Step 1.1 patches the local differential within $U$; each point outside $U$ has a neighborhood disjoint from the closed set $K$, on which the zero extension is zero. Hence the extension has the asserted global weak differential and no boundary contribution. If $K$ is nonempty, compactness gives numbers $0<r\le s$ and $0<a\le b$ such that on $x(K)$, $r\le\rho\le s$ and $a|q|_2\le\sqrt{q^TG^{-1}q}\le b|q|_2$. Indeed the positive continuous density and the positive continuous function $\sqrt{q^TG^{-1}q}$ on the compact set $x(K)\times\{q:|q|_2=1\}$ have positive lower and finite upper bounds, by taking finite subcovers of neighborhoods where each has such bounds. No bound on the closure of the whole chart is used. Since $|q|_2\le\sum_i|q_i|\le\sqrt n|q|_2$, substituting [F1] and [F2] into the integral proves the inequalities with $c=r\min(1,a/\sqrt n)$ and $C=s\max(1,b)$. If $K$ is empty, $u$ and its derivatives are zero almost everywhere and $c=C=1$ suffices. [F1, F2, F3, step 1.1, algebra]

2.2 Apply [F4] locally to the coordinate expressions of any locally Lipschitz scalar function. Locally Lipschitz here means locally Lipschitz in smooth coordinates; this property is invariant because smooth transitions have bounded derivative on sufficiently small compact coordinate boxes. On each such box the function and its weak derivatives are integrable, so it is $W^{1,1}_{\mathrm{loc}}$. At points of classical differentiability the ordinary chain rule gives exactly the transformation in step 1.1. The null-set invariance proved there makes the resulting differential independent of chart as an almost-everywhere field. Second countability and [A1] give a countable subatlas, so these local null exceptions can be combined into one null set. For an arbitrary $W^{1,1}_{\mathrm{loc}}$ coordinate function and smooth $\chi$, use $\chi\varphi$ as the test in [F3]. Expanding $\partial_i(\chi\varphi)$ gives $$\int \chi u\,\partial_i\varphi\,dx=-\int(\chi u_i+u\,\partial_i\chi)\varphi\,dx.$$ The right-hand coefficient is locally integrable because the smooth factors are bounded on the support of each test. Thus $D_i(\chi u)=\chi u_i+u\partial_i\chi$, and step 1.1 makes this the stated global weak product rule. [F3, F4, A1, step 1.1, algebra]

3.1 The positive density $\rho$ has exactly the same null sets as coordinate Lebesgue measure: on each compact coordinate subset it is bounded above and below, and countably many relatively compact coordinate boxes cover $\Omega$. Therefore essential supremum norms agree. The equality of pointwise suprema for a specified representative follows directly from bijectivity of $x$. If that representative is continuous, any strict lower bound on its absolute value attained at a point holds on a neighborhood of that point, which has positive volume; hence its pointwise supremum is also its essential supremum, including the possible infinite value. [F2, F6, A1, step 2.1, algebra]

4.1 For $n=0$, a nonempty coordinate chart is a single point, its tangent and cotangent spaces are zero, and [F2] assigns that point volume one. Under the stated zero-dimensional convention both norms are $|u|$, all differential terms vanish, and the product rule is $0=0$. Null sets for this measure contain no chart point, so essential and pointwise suprema agree. The empty chart gives only zero norms. This proves all remaining cases. [given, F1, F2, F6, step 2.1, step 3.1, step 2.2] ∎

---
id: lem-author-58255dfd955f-compact-comparison
title: Compact-domain comparison with a nonnegative potential
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-laplace-beltrami-operator-as-trace-of-the-hessian
  - math:def-riemannian-gradient
  - math:prop-coordinate-formula-for-riemannian-divergence
  - math:def-riemannian-volume-density
  - math:thm-smooth-partitions-of-unity-exist-on-manifolds
  - math:def-sobolev-space-wkp-and-its-norm
  - math:def-hk-and-hk-zero-notation
  - math:lem-positive-part-is-an-admissible-weak-test-by-truncation
  - math:thm-zero-weak-gradient-implies-componentwise-constancy
  - math:def-axiom-of-choice
dependency_roles:
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-laplace-beltrami-operator-as-trace-of-the-hessian: mathematical-premise
  math:def-riemannian-gradient: mathematical-premise
  math:prop-coordinate-formula-for-riemannian-divergence: mathematical-premise
  math:def-riemannian-volume-density: mathematical-premise
  math:thm-smooth-partitions-of-unity-exist-on-manifolds: mathematical-premise
  math:def-sobolev-space-wkp-and-its-norm: mathematical-premise
  math:def-hk-and-hk-zero-notation: mathematical-premise
  math:lem-positive-part-is-an-admissible-weak-test-by-truncation: mathematical-premise
  math:thm-zero-weak-gradient-implies-componentwise-constancy: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $D$ be a relatively compact smooth domain in a smooth Riemannian manifold $(M,h)$, with $\overline C\cap\partial D\ne\varnothing$ for each connected component $C$ of $D$. Here $N=\overline D$ is the smooth compact closure of the domain, regarded as an embedded full-dimensional manifold with boundary, and $\partial D=\partial N$ is its intrinsic manifold boundary. The smooth-domain convention includes $N\setminus D\subseteq\partial N$. The ambient manifold $M$ may have boundary; put $\Omega=D\cap M^\circ$. Points inherited from $\partial M$ belong to $\partial N$, as verified below. Let $V\ge0$ be bounded and smooth, and $w\in C^2(D)\cap C^1(\overline D)$ be real. Use the positive-divergence convention $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. If $(\Delta_h-V)w\ge0$ on $\Omega$ and $w\le0$ on $\partial D$, then $w\le0$ in $D$. Equivalently, supersolutions dominate subsolutions with ordered boundary data for this operator, when their difference has the stated regularity. Work in ZFC.

## Facts & Assumptions

**Given:** The Riemannian manifold and Laplacian are those of [[math:def-riemannian-metric-and-riemannian-manifold]] and [[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]]. Write $v_\epsilon=(w-\epsilon)^+=\max(w-\epsilon,0)$ for $\epsilon>0$. We assume [[math:def-axiom-of-choice]], hence Countable Choice, for the partition and Sobolev suppliers below.

[F1] In an interior chart of dimension $n\ge1$, put $m=\sqrt{\det(h_{ij})}$, $A^{ij}=mh^{ij}$ and $q=mV$. The gradient formula in [[math:def-riemannian-gradient]], the divergence formula in [[math:prop-coordinate-formula-for-riemannian-divergence]], and the trace-of-Hessian convention give $\Delta_hw=m^{-1}\partial_i(A^{ij}\partial_jw)$. These suppliers state smooth-input formulas; step 1.2 verifies their use for $C^2$ functions. The Riemannian density is $d\mu_h=m\,dx$ by [[math:def-riemannian-volume-density]]; it requires no orientation.

[F2] Under Countable Choice, [[math:thm-smooth-partitions-of-unity-exist-on-manifolds]] supplies a nonnegative, locally finite smooth partition subordinate to a cover of $\Omega$ by coordinate balls $U=x^{-1}(B)$, where $x:O\to x(O)$ is an interior chart and $B\subset\mathbb R^n$ is a bounded open ball with $\overline B\subset x(O\cap\Omega)$. Thus $\overline U$ is compact and contained in the larger chart $O$ and in $\Omega$. Only finitely many partition supports meet any fixed compact subset. A square partition suitable for the particular cutoff tests is constructed in step 3.1.

[F3] We use real $H^1=W^{1,2}$ classes with weak coordinate derivatives as in [[math:def-sobolev-space-wkp-and-its-norm]] and [[math:def-hk-and-hk-zero-notation]]. On each coordinate ball $U=x^{-1}(B)$ in [F2], the coordinate representative $w\circ x^{-1}$ belongs to $H^1(B)$. Indeed, this function and its coordinate first derivatives extend continuously to the compact set $\overline B$ inside $x(O\cap\Omega)$ and are therefore bounded there. Since $B$ is bounded it has finite Lebesgue measure, so these functions are square integrable; classical integration by parts against compactly supported smooth tests identifies the weak derivatives. The supplier [[math:lem-positive-part-is-an-admissible-weak-test-by-truncation]] gives $Dv_\epsilon=\mathbf 1_{\{w>\epsilon\}}Dw$ almost everywhere and admissibility of $\eta^2v_\epsilon$ for $\eta\in C_c^\infty$ in the local weak inequality when its source is $L^2_{\mathrm{loc}}$. We use exactly these compactly supported tests, with source $-qw$, which is continuous and hence locally square integrable. No trace characterization or general boundary-test assertion is needed.

[F4] By [[math:thm-zero-weak-gradient-implies-componentwise-constancy]], under AC an element of $W^{1,2}_{\mathrm{loc}}(G)$ with all weak derivatives zero on an open Euclidean set $G\subseteq\mathbb R^n$, $n\ge1$, is almost everywhere constant on each component. For our continuous truncation, this gives pointwise local constancy on coordinate balls in $\Omega$; step 4.1 explains its extension to $D$ using the boundary condition.

## Proof

**Given:** The hypotheses of the Statement and the suppliers in Facts & Assumptions.

**Goal:** Prove the compact-domain maximum and comparison assertions.

**Proof technique:** direct.

1.1 If $D$ is empty the assertion is vacuous. In dimension zero the manifold is discrete, so each component of $D$ is a closed singleton and cannot have closure meeting $\partial D$; thus the hypotheses force $D$ to be empty. In positive dimension, $N\cap\partial M\subseteq\partial N$. Indeed, if an ambient-boundary point were an intrinsic interior point of $N$, an ambient boundary coordinate $r\ge0$ would restrict to a smooth function on an open neighborhood in $N$ with an interior minimum zero. Its differential there would vanish. But the inclusion of the full-dimensional embedded $N$ has an invertible tangent map, so the nonzero differential $dr$ of that boundary coordinate would restrict to a nonzero differential, a contradiction. Hence $D\setminus\Omega\subseteq\partial D$, and $N\setminus\partial D\subseteq\Omega$ by the smooth-domain convention. [given, algebra]

1.2 Fix an interior point $p\in\Omega$ and replace $w$ in its coordinates by the polynomial with the same value and first and second derivatives at $p$. Metric duality gives $(\operatorname{grad}_hw)^i=h^{ij}\partial_jw$. Its first derivatives depend only on the two-jet of $w$, so the trace of its covariant derivative agrees at $p$ with that of the smooth polynomial. The density-divergence formula for a $C^1$ vector field follows likewise by replacing its coordinate coefficients by affine functions with the same one-jet. Consequently the smooth formulas in [F1] imply $\Delta_hw=m^{-1}\partial_i(A^{ij}\partial_jw)$ for the stated $C^2$ function in every interior chart. [F1, given, algebra]

2.1 In a coordinate ball $U=x^{-1}(B)$ as in [F2], the differential inequality becomes $-\partial_i(A^{ij}\partial_jw)+qw\le0$. Multiply by a nonnegative $\varphi\in C_c^\infty$ and integrate in chart coordinates. Each product $A^{ij}\partial_jw\,\varphi$ is $C^1$ and compactly supported, so extension by zero and one-dimensional integration of its $i$th derivative give $\int(A^{ij}\partial_jw\partial_i\varphi+qw\varphi)\,dx\le0$. This has local source $-qw\in L^2_{\mathrm{loc}}$. Thus [F3] extends it to each nonnegative test $\varphi=\eta^2v_\epsilon$, with the stated truncation and product derivative formulas. All tests are supported in the interior, so no manifold-boundary integration or boundary-chart approximation occurs. [F2, F3, step 1.2, given, algebra]

3.1 Fix $\epsilon>0$. The set $K=\{x\in\overline D:w(x)\ge\epsilon\}$ is compact and disjoint from $\partial D$, so step 1.1 gives $K\subset\Omega$ and $\operatorname{supp}v_\epsilon\subseteq K$ (support taken in $N$). If $K$ is empty then $v_\epsilon=0$. Otherwise take a locally finite partition $(\chi_a)$ from [F2], subordinate to the coordinate balls $U=x^{-1}(B)$ of [F2], and put $s=(\sum_a\chi_a^2)^{1/2}$ and $\eta_a=\chi_a/s$. The locally finite sum is smooth and strictly positive because $\sum_a\chi_a=1$; each $\eta_a$ is smooth, has compact support in its chart, and $\sum_a\eta_a^2=1$. Only finitely many supports meet $K$. Apply step 2.1 with each corresponding $\eta_a^2v_\epsilon$ and sum. With the density from [F1] the result is $\int_\Omega(\langle\nabla_hw,\nabla_hv_\epsilon\rangle_h+Vwv_\epsilon)\,d\mu_h\le0$: the terms containing partition derivatives cancel because $\sum_a\nabla_h(\eta_a^2)=0$ near $K$, and $v_\epsilon$ and its weak derivatives vanish off $K$. [F1, F2, F3, step 1.1, step 2.1, algebra, construct]

4.1 The integrand in step 3.1 equals $\mathbf 1_{\{w>\epsilon\}}|\nabla_hw|_h^2+Vwv_\epsilon$ almost everywhere. Both terms are nonnegative, so the weak gradient of $v_\epsilon$ is zero almost everywhere. On each coordinate ball $U=x^{-1}(B)$ of [F2], smooth positive definiteness and the positive density imply equivalence with zero Euclidean weak derivatives. Apply [F4] on that ball. Its almost everywhere constant value is its value everywhere by continuity of $v_\epsilon$, since every nonempty coordinate ball has positive measure. Thus $v_\epsilon$ is locally constant on $\Omega$. At any $q\in D\setminus\Omega$, step 1.1 places $q$ in $\partial D$, so $w(q)\le0<\epsilon$. Continuity supplies a relative neighborhood of $q$ in $D$ on which $w<\epsilon$, and $v_\epsilon=0$ there. Consequently $v_\epsilon$ is locally constant on all of $D$, and connectedness makes it a single constant on each component $C$. Choose $p\in\overline C\cap\partial D$; continuity on $\overline D$ and $w(p)\le0$ show that this constant is $v_\epsilon(p)=0$. Hence $v_\epsilon=0$ throughout $D$ for every $\epsilon>0$, and $w\le0$. For a subsolution $u_-$ and supersolution $u_+$ satisfying $(\Delta_h-V)u_-\ge0$, $(\Delta_h-V)u_+\le0$ and ordered boundary values, apply the established assertion to $w=u_--u_+$, whose operator and boundary signs are exactly those required. [F2, F3, F4, step 1.1, step 3.1, given, algebra] ∎

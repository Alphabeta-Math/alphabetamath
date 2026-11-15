---
title: ADM section time and causal spatial speed
status: published
research_item: lem-author-eb8e266b8b92-adm-time-speed
dependency_level: 2
sources:
  references: []
---

## Prerequisites

- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)
- [math:thm-c1-lipschitz-ac-bv-hierarchy](https://alphabetamath.cc/item/thm-c1-lipschitz-ac-bv-hierarchy)
- [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)
- [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)
- [math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function)
- [math:def-pointwise-norm-and-angle-from-a-riemannian-metric](https://alphabetamath.cc/item/def-pointwise-norm-and-angle-from-a-riemannian-metric)
- [math:def-action-of-a-vector-field-on-smooth-functions](https://alphabetamath.cc/item/def-action-of-a-vector-field-on-smooth-functions)
- [math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)


## Statement

Assume the Axiom of Choice. Equip $E=\mathbb R_v\times S$, where $S$ is a connected smooth three-manifold, with the canonical product smooth structure. Let $h$ be a smooth Riemannian metric on $S$, $N>0$ a smooth function on $S$, and $X$ a smooth vector field on $S$, extended independently of $v$ using the product splitting. Give $g=-N^2dv^2+h(dx+Xdv,dx+Xdv)$ the time orientation of $n=N^{-1}(\partial_v-X)$. This is a smooth Lorentzian metric of signature $(-,+,+,+)$, and $n$ is its smooth unit timelike normal to the $v$-slices, declared future-directed. A causal curve means a locally absolutely continuous curve with nonzero causal velocity almost everywhere. Every future causal curve has strictly increasing $v$ and can be written as $(v,x(v))$ on its $v$-image. This representation is locally Lipschitz in charts, is future causal, and satisfies $|x'+X|_h\le N$ almost everywhere. In particular $|x'|_h\le N+|X|_h$ and $|(f\circ x)'|\le N|df|_h+|X(f)|$ for every smooth real $f$ on $S$. Here $|Y|_h=\sqrt{h(Y,Y)}$, $|df|_h:=|\operatorname{grad}_h f|_h$, where $h(\operatorname{grad}_h f,Y)=df(Y)$, and $X(f)=df(X)$ is the action of $X$ on $f$. Inextendibility as absence of an endpoint is preserved by this change of parameter.

## Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)

[math:thm-c1-lipschitz-ac-bv-hierarchy](https://alphabetamath.cc/item/thm-c1-lipschitz-ac-bv-hierarchy)

[math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function)

[math:def-pointwise-norm-and-angle-from-a-riemannian-metric](https://alphabetamath.cc/item/def-pointwise-norm-and-angle-from-a-riemannian-metric)

[math:def-action-of-a-vector-field-on-smooth-functions](https://alphabetamath.cc/item/def-action-of-a-vector-field-on-smooth-functions)

[math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)

[math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

## Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice implies Dependent Choice and Countable Choice, supplying the hypotheses of the causal-curve calculus and absolutely-continuous fundamental theorem used below. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F2] Causal curves are locally absolutely continuous, have nonzero future causal velocity almost everywhere, and inextendibility means absence of a limit at a parameter end. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F3] A lapse and shift decompose the stationary vector as $\partial_v=Nn+X$ with $g(n,n)=-1$ and $X$ tangent to the spacelike slice. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F4] Smooth composition of a locally absolutely continuous curve is locally absolutely continuous and satisfies the chain rule almost everywhere; strictly increasing continuous changes of parameter preserve the endpoint criterion. [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[F5] An absolutely continuous real function is the integral of its almost-everywhere derivative; Lipschitz functions are absolutely continuous. [math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions) [math:thm-c1-lipschitz-ac-bv-hierarchy](https://alphabetamath.cc/item/thm-c1-lipschitz-ac-bv-hierarchy)

[F6] On a compact coordinate ball, a smooth positive-definite metric bounds the Euclidean norm from below and above. [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

[F7] The canonical product charts give $E=\mathbb R\times S$ its smooth four-manifold structure and the splitting $T_{(v,p)}E=\mathbb R\partial_v\oplus T_pS$. [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[F8] The pointwise norm is $|Y|_h=\sqrt{h(Y,Y)}$, the gradient satisfies $df(Y)=h(\operatorname{grad}_h f,Y)$, and the vector-field action is $X(f)=df(X)$. Cauchy–Schwarz in the inner product $h_p$ gives $|df(Y)|\le|df|_h|Y|_h$ with the norm convention in the Statement. [math:def-pointwise-norm-and-angle-from-a-riemannian-metric](https://alphabetamath.cc/item/def-pointwise-norm-and-angle-from-a-riemannian-metric) [math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function) [math:def-action-of-a-vector-field-on-smooth-functions](https://alphabetamath.cc/item/def-action-of-a-vector-field-on-smooth-functions) [math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)

[F9] A Riemannian metric is a smooth symmetric covariant two-tensor that is positive definite on each tangent space. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[F10] A Lorentzian metric in four dimensions is a smooth symmetric nondegenerate covariant two-tensor of signature $(-,+,+,+)$. A time orientation is a smooth timelike vector field $n$; a nonzero causal vector $Y$ is future-directed exactly when $g(Y,n)<0$. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

## Proof

1.1 In the product splitting, the map $(a,W)\mapsto(a,W+aX)$ is invertible and carries the quadratic form of $g$ to $-N^2a^2+h(W,W)$. Smoothness, $N>0$ and positive definiteness of $h$ therefore make $g$ smooth and Lorentzian of the asserted signature. Direct substitution gives $g(n,n)=-1$ and $g(n,W)=0$ for spatial $W$, while the restriction to each slice is $h$; hence $n$ is the asserted smooth unit normal. For a nonzero future causal vector $Y=a\partial_v+W$, its pairing with $n$ is $-Na<0$, so $a>0$. The metric identity gives $|W+aX|_h\le Na$. Applied almost everywhere to the original curve parameter $s$, these identities give $v_s>0$ and the coordinate estimate $|x_s|_{\mathrm e}\le Bv_s$ on any relatively compact coordinate neighborhood, for some finite $B$. The bound follows from smoothness of $N,X,h$ and the metric comparison. [F2, F3, F6, F7, F9, F10, algebra]

2.1 Integrating $v_s>0$ on any nondegenerate compact parameter interval shows that $v$ is strictly increasing. It therefore has a continuous inverse on its image interval. To justify the required vector estimate using scalar integration, let $z:[a,b]\to\mathbb R^3$ have absolutely continuous coordinates, let $w:[a,b]\to\mathbb R$ be absolutely continuous with $w_s\ge0$ almost everywhere, and suppose $|z_s|_H\le Cw_s$ almost everywhere for a fixed inner product $H$ and constant $C\ge0$. Put $D=z(b)-z(a)$. If $D\ne0$, fix $e=D/|D|_H$ and the real function $\phi(s)=H(e,z(s))$. This fixed linear combination of coordinates is absolutely continuous, and $\phi_s=H(e,z_s)$ almost everywhere. The scalar fundamental theorem makes $\phi_s,w_s$ integrable; Cauchy–Schwarz gives $\phi_s\le Cw_s$. Consequently $|D|_H=\phi(b)-\phi(a)=\int_a^b\phi_s\,ds\le C\int_a^b w_s\,ds=C(w(b)-w(a))$. If $D=0$, the same bound follows from $w(b)\ge w(a)$. On each compact chart subarc apply this estimate with $z=x$, $w=v$, $H$ the Euclidean inner product and $C=B$, obtaining $|x(s_2)-x(s_1)|_{\mathrm e}\le B(v(s_2)-v(s_1))$. Thus $x$ as a function of $v$ is locally Lipschitz; each coordinate is therefore locally absolutely continuous. This argument does not assume absolute continuity of the inverse of $v$. [F1, F4, F5, F8, step 1.1, algebra]

3.1 At an interior differentiability point $v_0$ of $x(v)$, put $p=x(v_0)$ and, in a spatial chart, freeze $H=h_p$, $N_0=N(p)$ and $c=X(p)$, identifying coordinate tangent vectors with $\mathbb R^3$. On a sufficiently short subarc about $p$, continuity of the coefficients and the coordinate speed bound imply $|x_s+v_sc|_H\le(N_0+\epsilon)v_s$ almost everywhere, where $\epsilon\to0$ as the subarc shrinks. On each compact subarc the coordinates of $z(s)=x(s)+v(s)c$ are absolutely continuous, since they are fixed linear combinations of the original absolutely continuous coordinates. Their derivatives and $v_s$ are integrable by the scalar fundamental theorem. Apply the scalar-projection estimate proved in step 2.1 with this $z$, $w=v$, the fixed inner product $H$ and $C=N_0+\epsilon$; it yields $|x(s_2)-x(s_1)+(v(s_2)-v(s_1))c|_H\le(N_0+\epsilon)(v(s_2)-v(s_1))$. Take one endpoint at $v_0$, divide by the positive increase of $v$, and shrink the subarc to $v_0$. The differentiability of $x(v)$ gives $|x_v(v_0)+X(p)|_{h_p}\le N(p)$. By local Lipschitz continuity and the scalar fundamental theorem applied to the three coordinates, such differentiability points have full measure in the $v$-interval. Hence $|x_v+X|_h\le N$ almost everywhere. Its time component is one, so the reparametrized velocity is nonzero future causal. This proves the reparametrized causal inequality. [F1, F4, F5, F6, F8, step 1.1, step 2.1, algebra]

4.1 The triangle inequality gives $|x_v|_h\le N+|X|_h$. For a smooth real $f$, the smooth-composition chain rule gives $(f\circ x)'=df(x_v)=df(x_v+X)-X(f)$ almost everywhere. Applying the gradient identity and Cauchy–Schwarz of [F8] to $x_v+X$ yields $|(f\circ x)'|\le|df|_h|x_v+X|_h+|X(f)|\le N|df|_h+|X(f)|$. Finally the increasing homeomorphism of parameter intervals preserves all endpoint limits in either direction, proving the inextendibility assertion. [F4, F8, step 2.1, step 3.1, algebra] ∎

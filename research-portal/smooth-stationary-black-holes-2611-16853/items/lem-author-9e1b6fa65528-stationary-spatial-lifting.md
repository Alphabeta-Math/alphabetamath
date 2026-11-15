---
id: lem-author-9e1b6fa65528-stationary-spatial-lifting
title: Stationary lifting of a spatial primitive
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-smooth-manifold
  - math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure
  - math:def-smooth-differential-k-form
  - math:def-closed-and-exact-differential-forms
  - math:def-interior-product-of-a-form-by-a-vector-field
  - math:def-wedge-product-of-differential-forms
  - math:def-pullback-of-a-differential-form
  - math:def-lie-derivative-of-a-differential-form
  - math:prop-local-coordinate-expression-for-a-differential-form
  - math:thm-local-coordinate-formula-for-the-exterior-derivative
  - math:prop-exterior-derivative-of-a-function-is-its-differential
  - math:prop-interior-product-is-a-graded-antiderivation
  - math:prop-differential-forms-form-a-graded-commutative-algebra
  - math:thm-the-exterior-derivative-is-a-graded-derivation
  - math:thm-the-exterior-derivative-squares-to-zero
  - math:thm-the-exterior-derivative-commutes-with-pullback
  - math:thm-cartans-magic-formula
dependency_roles:
  math:def-smooth-manifold: mathematical-premise
  math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure: mathematical-premise
  math:def-smooth-differential-k-form: mathematical-premise
  math:def-closed-and-exact-differential-forms: mathematical-premise
  math:def-interior-product-of-a-form-by-a-vector-field: mathematical-premise
  math:def-wedge-product-of-differential-forms: mathematical-premise
  math:def-pullback-of-a-differential-form: mathematical-premise
  math:def-lie-derivative-of-a-differential-form: mathematical-premise
  math:prop-local-coordinate-expression-for-a-differential-form: mathematical-premise
  math:thm-local-coordinate-formula-for-the-exterior-derivative: mathematical-premise
  math:prop-exterior-derivative-of-a-function-is-its-differential: mathematical-premise
  math:prop-interior-product-is-a-graded-antiderivation: mathematical-premise
  math:prop-differential-forms-form-a-graded-commutative-algebra: mathematical-premise
  math:thm-the-exterior-derivative-is-a-graded-derivation: mathematical-premise
  math:thm-the-exterior-derivative-squares-to-zero: mathematical-premise
  math:thm-the-exterior-derivative-commutes-with-pullback: mathematical-premise
  math:thm-cartans-magic-formula: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $\Sigma$ be a smooth manifold and give $E=\mathbb R_t\times\Sigma$ its product smooth structure. Write $t:E\to\mathbb R$ for the first coordinate, $\pi:E\to\Sigma$ for the projection and $T=\partial_t$. Suppose $\Theta\in\Omega^2(E)$ is smooth, closed and stationary, $D\in C^\infty(E)$ is stationary and $\iota_T\Theta=dD$. Put $B=\Theta-dt\wedge dD$. Then there is a unique smooth closed two-form $b$ on $\Sigma$ such that $B=\pi^*b$. If $b$ has a smooth primitive $a\in\Omega^1(\Sigma)$, meaning $da=b$, every real constant $c$ gives the smooth one-form $V=(c-D)dt+\pi^*a$ on $E$ with $dV=\Theta$, $\mathcal L_TV=0$ and $V(T)+D=c$. Here a function or form is stationary when its coefficients in product coordinates $(t,x)$, with $x$ a chart on $\Sigma$, are independent of $t$; a form descends to $\Sigma$ when it is a pullback by $\pi$.

## Statement references

[[math:def-smooth-manifold]]

[[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure]]

[[math:def-smooth-differential-k-form]]

[[math:def-closed-and-exact-differential-forms]]

[[math:def-interior-product-of-a-form-by-a-vector-field]]

[[math:def-wedge-product-of-differential-forms]]

[[math:def-pullback-of-a-differential-form]]

[[math:def-lie-derivative-of-a-differential-form]]

[[math:prop-local-coordinate-expression-for-a-differential-form]]

[[math:thm-local-coordinate-formula-for-the-exterior-derivative]]

[[math:prop-exterior-derivative-of-a-function-is-its-differential]]

[[math:prop-interior-product-is-a-graded-antiderivation]]

[[math:prop-differential-forms-form-a-graded-commutative-algebra]]

[[math:thm-the-exterior-derivative-is-a-graded-derivation]]

[[math:thm-the-exterior-derivative-squares-to-zero]]

[[math:thm-the-exterior-derivative-commutes-with-pullback]]

[[math:thm-cartans-magic-formula]]

## Facts & Assumptions

[F1] Smooth manifolds and their product charts have the declared meanings; in these charts the projection $\pi(t,x)=x$ and the slice map $j(x)=(0,x)$ are smooth. [[math:def-smooth-manifold]] [[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure]]

[F2] Use smooth differential forms, closedness $d\omega=0$, exactness $\omega=d\eta$, interior product, wedge product, pullback and Lie derivative with their declared meanings. In particular, $(F^*\omega)_p(v_1,\ldots,v_k)=\omega_{F(p)}(dF_pv_1,\ldots,dF_pv_k)$. [[math:def-smooth-differential-k-form]] [[math:def-closed-and-exact-differential-forms]] [[math:def-interior-product-of-a-form-by-a-vector-field]] [[math:def-wedge-product-of-differential-forms]] [[math:def-pullback-of-a-differential-form]] [[math:def-lie-derivative-of-a-differential-form]]

[F3] A smooth form has a unique expansion in increasing coordinate wedges, $d(\sum_I\omega_I dx^I)=\sum_I d\omega_I\wedge dx^I$, and $df(X)=Xf$. [[math:prop-local-coordinate-expression-for-a-differential-form]] [[math:thm-local-coordinate-formula-for-the-exterior-derivative]] [[math:prop-exterior-derivative-of-a-function-is-its-differential]]

[F4] Pointwise contraction satisfies $\iota_X(\alpha\wedge\beta)=(\iota_X\alpha)\wedge\beta+(-1)^k\alpha\wedge\iota_X\beta$ when $\alpha$ has degree $k$. Wedge products of smooth forms are smooth and graded commutative. [[math:prop-interior-product-is-a-graded-antiderivation]] [[math:prop-differential-forms-form-a-graded-commutative-algebra]]

[F5] Exterior differentiation is real linear, satisfies $d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^k\alpha\wedge d\beta$ for $\alpha$ of degree $k$, squares to zero, and commutes with pullback along smooth maps. [[math:thm-the-exterior-derivative-is-a-graded-derivation]] [[math:thm-the-exterior-derivative-squares-to-zero]] [[math:thm-the-exterior-derivative-commutes-with-pullback]]

[F6] Cartan's formula is $\mathcal L_X\omega=d(\iota_X\omega)+\iota_X(d\omega)$. [[math:thm-cartans-magic-formula]]

## Proof

**Given:** The smooth product, forms, function and hypotheses in the Statement.

**Goal:** Construct the descended closed form and its stationary lift with every stated identity.

1.1 The product coordinates give $dt(T)=1$ and $T(D)=0$, hence $\iota_TdD=0$. The contraction rule gives $\iota_T(dt\wedge dD)=dD-dt\,T(D)=dD$, so $\iota_TB=0$. The coordinate formula for $dD$ and stationarity of $D$ show that $dD$ has no $dt$ component and its coefficients are independent of $t$. Thus $B$ is stationary as well. [given, F1, F2, F3, F4]

2.1 Define $b=j^*B$. In every product chart the unique two-form expansion of $B$ has no $dt$ terms because $\iota_TB=0$, and its remaining coefficients are independent of $t$. Evaluating the pullback formulas for $j$ and $\pi$ therefore gives $B=\pi^*b$; it also proves uniqueness by evaluating this equality on the slice $t=0$. The form $b$ is globally smooth by its definition. Since $d(dt)=d^2t=0$, $d^2D=0$ and $d\Theta=0$, the graded product rule gives $dB=0$. Smoothness of $j$ and commutation with pullback now give $db=d(j^*B)=j^*(dB)=0$. [given, F1, F2, F3, F5, step 1.1]

3.1 Let $a$ be the supplied smooth primitive, $da=b$, and let $c\in\mathbb R$. The pullback $\pi^*a$ is a smooth form on $E$, so $V=(c-D)dt+\pi^*a$ is well defined and smooth. Differentiation and graded commutativity give $dV=-dD\wedge dt+\pi^*(da)=dt\wedge dD+\pi^*b=\Theta$. Since $d\pi(T)=0$, the pullback formula gives $(\pi^*a)(T)=a(d\pi(T))=0$, whence $V(T)=c-D$. [given, F1, F2, F3, F4, F5, step 2.1]

4.1 The coefficients of $\pi^*a$ in product coordinates depend only on $x$, so $V$ is stationary in the stated coordinate sense. Moreover Cartan's formula, $dV=\Theta$ and $\iota_T\Theta=dD$ give $\mathcal L_TV=d(V(T))+\iota_TdV=d(c-D)+dD=0$, and $V(T)+D=c$. The construction assumes the smooth primitive $a$; it does not assert that every closed form is exact. [given, F2, F5, F6, step 3.1] ∎

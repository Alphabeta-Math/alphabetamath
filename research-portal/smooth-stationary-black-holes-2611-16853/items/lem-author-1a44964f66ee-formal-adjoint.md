---
id: lem-author-1a44964f66ee-formal-adjoint
title: Formal adjoint of a real drift Laplacian on a closed manifold
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:thm-fundamental-theorem-of-riemannian-geometry
  - math:thm-riemannian-divergence-theorem
  - math:def-axiom-of-choice
  - math:def-riemannian-gradient
  - math:def-laplace-beltrami-operator-as-trace-of-the-hessian
  - math:def-density-bundle-and-smooth-density
  - math:def-riemannian-volume-density
  - math:lem-the-riemannian-volume-density-is-coordinate-independent
  - math:def-integral-of-a-compactly-supported-smooth-density
  - math:thm-density-integration-is-defined-without-an-orientation
  - math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary
  - math:prop-coordinate-formula-for-riemannian-divergence
dependency_roles:
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:thm-fundamental-theorem-of-riemannian-geometry: mathematical-premise
  math:thm-riemannian-divergence-theorem: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-riemannian-gradient: mathematical-premise
  math:def-laplace-beltrami-operator-as-trace-of-the-hessian: mathematical-premise
  math:def-density-bundle-and-smooth-density: mathematical-premise
  math:def-riemannian-volume-density: mathematical-premise
  math:lem-the-riemannian-volume-density-is-coordinate-independent: mathematical-premise
  math:def-integral-of-a-compactly-supported-smooth-density: mathematical-premise
  math:thm-density-integration-is-defined-without-an-orientation: mathematical-premise
  math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary: mathematical-premise
  math:prop-coordinate-formula-for-riemannian-divergence: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $(S,h)$ be a connected compact smooth Riemannian manifold without boundary, of positive dimension. For a smooth real vector field $t$ and smooth real function $c$, put $Lu=-\Delta_hu+2\langle t,\nabla u\rangle_h+cu$, with $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. The formal adjoint for $\langle f,g\rangle_{L^2}=\int_S\overline f g\,d\mu_h$ is $L^\dagger u=-\Delta_hu-2\langle t,\nabla u\rangle_h+(c-2\operatorname{div}_ht)u$. It has smooth real coefficients and the same negative-Laplacian principal part. The measure $d\mu_h$ is the positive Riemannian density, so no orientation assumption is needed.

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The supplied metric has its Levi–Civita connection. Gradient and Laplacian use $\operatorname{grad}_h u=(du)^\sharp$ and $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$; in coordinates $(\operatorname{grad}_h u)^i=h^{ij}\partial_j u$ and $\operatorname{div}_hX=\gamma^{-1}\partial_i(\gamma X^i)$, where $\gamma=\sqrt{\det(h_{ij})}$. Differential expressions extend complex-linearly, and contractions in them use the complex-bilinear extension of $h$. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:thm-fundamental-theorem-of-riemannian-geometry]] [[math:def-riemannian-gradient]] [[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]] [[math:prop-coordinate-formula-for-riemannian-divergence]]

[F2] Density frames transform by absolute Jacobians. The local expressions $d\mu_h=\sqrt{\det(h_{ij})}\,|dx^1\cdots dx^n|$ therefore glue to a smooth positive density on $S$, independently of orientability. [[math:def-density-bundle-and-smooth-density]] [[math:def-riemannian-volume-density]] [[math:lem-the-riemannian-volume-density-is-coordinate-independent]]

[F3] Compactly supported smooth density integration is defined by chart partitions, is independent of those choices, is linear and local, and is strictly positive on any nonzero nonnegative density. Integrate complex coefficients by their real and imaginary parts. Compactness makes all smooth function multiples of $d\mu_h$ compactly supported. Work in ZFC: Choice supplies the countable-choice hypotheses of density integration and partitions. The $L^2$ notation here denotes the displayed pairing on smooth functions. [[math:def-integral-of-a-compactly-supported-smooth-density]] [[math:thm-density-integration-is-defined-without-an-orientation]] [[math:def-axiom-of-choice]]

[F4] A smooth partition of unity subordinate to a coordinate cover exists under countable choice. The divergence theorem is applied only on an oriented coordinate domain, with its restricted metric and a compactly supported vector field; that domain has no manifold boundary, so its divergence integral is zero. No orientation of $S$ is assumed. [[math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary]] [[math:thm-riemannian-divergence-theorem]] [[math:def-axiom-of-choice]]

[F5] Here a formal adjoint of $L$ means a linear smooth-coefficient differential operator $A$ satisfying $\langle f,Lg\rangle_{L^2}=\langle Af,g\rangle_{L^2}$ for every $f,g\in C^\infty(S;\mathbb C)$. This is an identity of the density integrals just specified. Existence and uniqueness for this operator are proved below. [[math:def-integral-of-a-compactly-supported-smooth-density]] [[math:thm-density-integration-is-defined-without-an-orientation]]

[F6] For scalar coordinate operators built from the supplied gradient and divergence, use this symbol convention: for second-order part $-a^{ij}\partial_i\partial_j$, put $\sigma_2(P)(x,\xi)=a^{ij}(x)\xi_i\xi_j$. Thus the sign is the one obtained by replacing each top-order derivative by $i\xi_j$. This convention applies in every positive dimension; its value for the two operators is calculated in the proof. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:def-riemannian-gradient]] [[math:prop-coordinate-formula-for-riemannian-divergence]]

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The supplied metric has its Levi–Civita connection. Gradient and Laplacian use $\operatorname{grad}_h u=(du)^\sharp$ and $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$; in coordinates $(\operatorname{grad}_h u)^i=h^{ij}\partial_j u$ and $\operatorname{div}_hX=\gamma^{-1}\partial_i(\gamma X^i)$, where $\gamma=\sqrt{\det(h_{ij})}$. Differential expressions extend complex-linearly, and contractions in them use the complex-bilinear extension of $h$. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:thm-fundamental-theorem-of-riemannian-geometry]] [[math:def-riemannian-gradient]] [[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]] [[math:prop-coordinate-formula-for-riemannian-divergence]]

[F2] Density frames transform by absolute Jacobians. The local expressions $d\mu_h=\sqrt{\det(h_{ij})}\,|dx^1\cdots dx^n|$ therefore glue to a smooth positive density on $S$, independently of orientability. [[math:def-density-bundle-and-smooth-density]] [[math:def-riemannian-volume-density]] [[math:lem-the-riemannian-volume-density-is-coordinate-independent]]

[F3] Compactly supported smooth density integration is defined by chart partitions, is independent of those choices, is linear and local, and is strictly positive on any nonzero nonnegative density. Integrate complex coefficients by their real and imaginary parts. Compactness makes all smooth function multiples of $d\mu_h$ compactly supported. Work in ZFC: Choice supplies the countable-choice hypotheses of density integration and partitions. The $L^2$ notation here denotes the displayed pairing on smooth functions. [[math:def-integral-of-a-compactly-supported-smooth-density]] [[math:thm-density-integration-is-defined-without-an-orientation]] [[math:def-axiom-of-choice]]

[F4] A smooth partition of unity subordinate to a coordinate cover exists under countable choice. The divergence theorem is applied only on an oriented coordinate domain, with its restricted metric and a compactly supported vector field; that domain has no manifold boundary, so its divergence integral is zero. No orientation of $S$ is assumed. [[math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary]] [[math:thm-riemannian-divergence-theorem]] [[math:def-axiom-of-choice]]

[F5] Here a formal adjoint of $L$ means a linear smooth-coefficient differential operator $A$ satisfying $\langle f,Lg\rangle_{L^2}=\langle Af,g\rangle_{L^2}$ for every $f,g\in C^\infty(S;\mathbb C)$. This is an identity of the density integrals just specified. Existence and uniqueness for this operator are proved below. [[math:def-integral-of-a-compactly-supported-smooth-density]] [[math:thm-density-integration-is-defined-without-an-orientation]]

[F6] For scalar coordinate operators built from the supplied gradient and divergence, use this symbol convention: for second-order part $-a^{ij}\partial_i\partial_j$, put $\sigma_2(P)(x,\xi)=a^{ij}(x)\xi_i\xi_j$. Thus the sign is the one obtained by replacing each top-order derivative by $i\xi_j$. This convention applies in every positive dimension; its value for the two operators is calculated in the proof. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:def-riemannian-gradient]] [[math:prop-coordinate-formula-for-riemannian-divergence]]

**Proof technique:** direct.

1.1 Choose a smooth chart-subordinate partition $(\rho_a)$. Local finiteness and compactness make only finitely many supports nonempty: finitely many neighborhoods covering $S$ each meet only finitely many supports. Each $\rho_aX$ is compactly supported inside its chart domain $U_a$, which is oriented by its coordinates. There $d\mu_h$ and the positive coordinate Riemannian volume form have the same coefficient $\gamma$, so their integrals of a chart-supported scalar agree. The oriented divergence theorem on $U_a$ gives $\int_S\operatorname{div}_h(\rho_aX)\,d\mu_h=0$, using locality to extend the chart integral to $S$. The coordinate product rule gives $\operatorname{div}_h(\rho_aX)=\rho_a\operatorname{div}_hX+d\rho_a(X)$. Sum the finite family, using $\sum_a\rho_a=1$ and $\sum_a d\rho_a=0$, to obtain $\int_S\operatorname{div}_hX\,d\mu_h=0$. The same identity holds for complex vector fields by real and imaginary parts. [F1, F2, F3, F4]

2.1 Apply step 1.1 to $\overline f\operatorname{grad}_h g$ and then to $g\operatorname{grad}_h\overline f$. The product rule gives $\int_S\overline f(-\Delta_hg)\,d\mu_h=\int_Sh(\nabla\overline f,\nabla g)\,d\mu_h=\int_S\overline{(-\Delta_hf)}g\,d\mu_h$. Thus the negative Laplacian is formally symmetric for the stated first-variable-conjugate-linear pairing. [F1, F3, F5, step 1.1]

3.1 Apply step 1.1 to $\overline fgt$. Expanding its divergence yields $\int_S\overline f\,2t\cdot\nabla g\,d\mu_h=-\int_Sg(2t\cdot\nabla\overline f+2\operatorname{div}_ht\,\overline f)\,d\mu_h$. Combining this with step 2.1 and the real multiplication coefficient $c$ proves $\langle f,Lg\rangle_{L^2}=\langle Af,g\rangle_{L^2}$ for $Af=-\Delta_hf-2t\cdot\nabla f+(c-2\operatorname{div}_ht)f$. All these coefficients are smooth and real. [F1, F3, F5, step 1.1, step 2.1]

4.1 If $A$ and $B$ both satisfy the identity in F5, then for each smooth $f$ and every smooth $g$ one has $\langle (A-B)f,g\rangle_{L^2}=0$. Choose $g=(A-B)f$, which is smooth and compactly supported on compact $S$. The resulting integral $\int_S|(A-B)f|^2\,d\mu_h$ is zero, so strict positivity of the density integral forces $(A-B)f=0$ everywhere. Hence $A=B$, and the operator of step 3.1 is the formal adjoint $L^\dagger$. [F2, F3, F5, step 3.1]

5.1 The coordinate formulas give $\Delta_hu=\gamma^{-1}\partial_i(\gamma h^{ij}\partial_ju)$, whose second-order part is $h^{ij}\partial_i\partial_ju$. The drift and multiplication terms in $L$ and $L^\dagger$ have order at most one, so both have second-order part $-h^{ij}\partial_i\partial_j$. In the convention F6 their symbol is $h^{ij}\xi_i\xi_j=h^{-1}(\xi,\xi)=|\xi|_h^2>0$ for nonzero $\xi$. This is an intrinsic quadratic form, hence chart independent, and the calculation includes dimension one. This proves all assertions of the Statement without an orientation assumption. [F1, F6, step 3.1, step 4.1] ∎

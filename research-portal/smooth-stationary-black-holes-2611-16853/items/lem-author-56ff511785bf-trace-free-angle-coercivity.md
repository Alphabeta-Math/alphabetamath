---
id: lem-author-56ff511785bf-trace-free-angle-coercivity
title: Trace-free three-dimensional coercivity for the logarithmic gradient
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:cor-real-spectral-theorem-for-self-adjoint-endomorphisms
  - math:def-self-adjoint-and-normal-endomorphism
  - math:def-trace-of-an-endomorphism
  - math:def-trace-of-a-square-matrix
  - math:def-operator-norm-on-a-finite-dimensional-inner-product-space
  - math:def-inner-product-norm
  - math:def-riemannian-gradient-of-a-smooth-function
  - math:def-inner-product-space
  - math:def-orthogonal-vectors-sets-and-orthonormal-bases
  - math:def-riemannian-metric-and-riemannian-manifold
dependency_roles:
  math:cor-real-spectral-theorem-for-self-adjoint-endomorphisms: mathematical-premise
  math:def-self-adjoint-and-normal-endomorphism: mathematical-premise
  math:def-trace-of-an-endomorphism: mathematical-premise
  math:def-trace-of-a-square-matrix: mathematical-premise
  math:def-operator-norm-on-a-finite-dimensional-inner-product-space: mathematical-premise
  math:def-inner-product-norm: mathematical-premise
  math:def-riemannian-gradient-of-a-smooth-function: mathematical-premise
  math:def-inner-product-space: mathematical-premise
  math:def-orthogonal-vectors-sets-and-orthonormal-bases: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-altered
proof_strategy: direct
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum, arXiv:2610.09729v1
      url: https://arxiv.org/pdf/2610.09729v1
      locator: Appendix B, proof of Lemma B.1, (B.8)–(B.10), printed/PDF pp.38–39
      statement: The proof bounds the square of the largest absolute eigenvalue of the
        trace-free three-dimensional second fundamental form by its squared norm
        with coefficient 2/3, then estimates the gradient of arcosh v.
      hypotheses: A spacelike maximal three-dimensional hypersurface, a future unit
        timelike observer, bounded background coefficients, and v>2 for the
        arcosh calculation.
      reading_limits: Consulted PDF text on pp.38–39 around (B.8)–(B.10); screenshot
        requests failed. This is methodological background, not an imported
        all-v theorem. The present proof uses finite-dimensional algebra and an
        assumed vector identity; it does not differentiate v. Its conditional
        logarithmic-gradient application and validity at v=1 are established
        locally. No weighted maximum estimate is imported.
dependency_level: 0
---

## Statement

Let $V$ be a three-dimensional real inner-product space and let $k:V\to V$ be symmetric, meaning $\langle kx,y\rangle=\langle x,ky\rangle$ for all $x,y\in V$, and trace free, meaning $\operatorname{tr}(k)=0$. Write $|x|^2=\langle x,x\rangle$ for vectors, $\|k\|_{\mathrm{op}}=\max_{|x|=1}|kx|$, and $|k|^2=\sum_{i=1}^3|ke_i|^2$ for any orthonormal basis $(e_i)_{i=1}^3$. The last expression, whose basis independence is proved below, defines the Hilbert–Schmidt norm of $k$.

Then $\|k\|_{\mathrm{op}}^2\le\tfrac23|k|^2$. If $v\ge1$ and $K\ge0$ are real numbers and $Z,Q,A\in V$ satisfy $|Z|^2=v^2-1$, $|Q|\le Kv^2$ and $vA=kZ+Q$, then for every $\varepsilon>0$ one has $|A|^2\le\tfrac23(1+\varepsilon)|k|^2+(1+\varepsilon^{-1})K^2v^2$.

In particular, let $(M,h)$ be a smooth three-dimensional Riemannian manifold, let $v:M\to(0,\infty)$ be smooth, and fix $p\in M$. Identify $V$ with $(T_pM,h_p)$, put $A=(\operatorname{grad}_h\log v)_p$, and use $v(p)$ for the numerical $v$ in the preceding hypotheses. Whenever those hypotheses and the vector identity hold at $p$, the same bound controls $|\operatorname{grad}_h\log v|_h^2(p)$, including when $v(p)=1$. The vector identity is an assumption of this application, not a conclusion about arbitrary functions $v$.

## Facts & Assumptions

[F1] For a linear endomorphism, symmetry is self-adjointness, and a real self-adjoint endomorphism has an orthonormal eigenbasis. [[math:def-self-adjoint-and-normal-endomorphism]] [[math:cor-real-spectral-theorem-for-self-adjoint-endomorphisms]]

[F2] The trace of an endomorphism is the basis-independent trace of its matrix; matrix trace is the sum of the diagonal entries. [[math:def-trace-of-an-endomorphism]] [[math:def-trace-of-a-square-matrix]]

[F3] Use the inner-product norm for vectors and the maximum over unit vectors for the operator norm. [[math:def-inner-product-norm]] [[math:def-operator-norm-on-a-finite-dimensional-inner-product-space]]

[F4] For a smooth function $f$ on a Riemannian manifold, $h_p((\operatorname{grad}_h f)_p,X)=df_p(X)$ for every $X\in T_pM$. [[math:def-riemannian-gradient-of-a-smooth-function]]

[F5] The real inner product is bilinear and positive definite. [[math:def-inner-product-space]]

## Proof

**Given:** The symmetric trace-free map, the numerical vector relation, and, for the application, the stated smooth Riemannian data. **Goal:** Establish both coercivity bounds and their conditional gradient application.

1.1 For arbitrary $x,y,z\in V$ and $a,b\in\mathbb R$, set $d=k(ax+by)-akx-bky$. The assumed symmetry and [F5] give $\langle d,z\rangle=\langle ax+by,kz\rangle-a\langle x,kz\rangle-b\langle y,kz\rangle=0$. Taking $z=d$ and using positive definiteness yields $d=0$. Thus $k$ is linear, and its symmetry makes it self-adjoint by [F1]. In particular, its endomorphism trace and operator norm are defined before they are used below. [F1, F5, given, algebra]

2.1 By [F1], an orthonormal basis exists. For two such bases write $f_j=\sum_i o_{ij}e_i$. Expanding each $e_i$ in the basis $(f_j)$ gives $\sum_j o_{ij}o_{\ell j}=\delta_{i\ell}$, so $\sum_j|kf_j|^2=\sum_{i,\ell,j}o_{ij}o_{\ell j}\langle ke_i,ke_\ell\rangle=\sum_i|ke_i|^2$. This proves that the finite sum defining $|k|^2$ is basis independent. [F1, F3, step 1.1, given, algebra]

3.1 By [F1], choose an orthonormal eigenbasis with eigenvalues $\lambda_1,\lambda_2,\lambda_3$, ordered so that $|\lambda_1|$ is largest. In this basis [F2] and trace freeness give $\lambda_2+\lambda_3=-\lambda_1$, and step 2.1 gives $|k|^2=\lambda_1^2+\lambda_2^2+\lambda_3^2$. Since $\lambda_2^2+\lambda_3^2\ge(\lambda_2+\lambda_3)^2/2$, one obtains $|k|^2\ge\tfrac32\lambda_1^2$. For $x=\sum_i x_i e_i$, $|kx|^2=\sum_i\lambda_i^2x_i^2\le\lambda_1^2|x|^2$, with equality at $x=e_1$. Thus [F3] gives $\|k\|_{\mathrm{op}}^2=\lambda_1^2\le\tfrac23|k|^2$. [F1, F2, F3, step 2.1, given, algebra]

4.1 For vectors $a,b$ and $\varepsilon>0$, expanding $|\sqrt\varepsilon a-\varepsilon^{-1/2}b|^2\ge0$ gives $|a+b|^2\le(1+\varepsilon)|a|^2+(1+\varepsilon^{-1})|b|^2$. Apply this to $A=kZ/v+Q/v$. The numerical hypotheses directly imply $|Z|^2/v^2=1-v^{-2}\le1$ and $|Q|/v\le Kv$. By [F3] and step 3.1, $|kZ|^2/v^2\le\|k\|_{\mathrm{op}}^2\le\tfrac23|k|^2$. Substitution proves the claimed vector bound. Only division by $v\ge1$ is used; if $v=1$, then $Z=0$ and the argument still applies. [F3, step 3.1, given, algebra]

5.1 In the stated Riemannian application, positivity and smoothness of $v$ make $\log v$ smooth, and [F4] defines $A=(\operatorname{grad}_h\log v)_p$ in the three-dimensional inner-product space $(T_pM,h_p)$. The assumed pointwise vector identity and bounds therefore satisfy precisely the hypotheses of step 4.1 with the scalar $v(p)$. That step proves the asserted gradient bound, also at $v(p)=1$. No differential identity has been inferred from the numerical assumptions. [F4, step 4.1, given] ∎

## Source notes

The Appendix B reference motivates the trace-free method. Its arcosh argument uses $v>2$; the present pointwise algebra divides only by $v$ and proves the conditional bound for every $v\ge1$.

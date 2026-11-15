---
id: lem-author-fd2999663761-logarithmic-angle-conversion
title: From hyperbolic angle to logarithmic angle inequalities
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-fd2999663761-temporal-angle-data
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:prop-gradient-hessian-and-divergence-connection-formulas
  - math:def-laplace-beltrami-operator-as-trace-of-the-hessian
  - math:lem-derivative-algebra-and-chain-rules
  - math:thm-hyperbolic-identities-and-derivatives
  - math:thm-inverse-hyperbolic-logarithm-formulas
  - math:thm-logarithm-derivative-and-integral
  - math:thm-real-power-continuity-and-derivatives
dependency_roles:
  def-author-fd2999663761-temporal-angle-data: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:prop-gradient-hessian-and-divergence-connection-formulas: mathematical-premise
  math:def-laplace-beltrami-operator-as-trace-of-the-hessian: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
  math:thm-hyperbolic-identities-and-derivatives: mathematical-premise
  math:thm-inverse-hyperbolic-logarithm-formulas: mathematical-premise
  math:thm-logarithm-derivative-and-integral: mathematical-premise
  math:thm-real-power-continuity-and-derivatives: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

On a Riemannian hypersurface let $v>2$ be smooth, put $\eta=\operatorname{arcosh}v=\log(v+\sqrt{v^2-1})$, and suppose $\Delta\eta\ge\coth\eta\,(\tfrac14|\nabla\eta|^2-Cv^2)$ for some $C\ge0$. Then $f=\log v$ satisfies $\Delta f\ge\tfrac14|\nabla f|^2-Cv^2$. The convention for gradient and Laplacian is that of the temporal angle data.

## Facts & Assumptions

[F1] Use the positive-trace scalar Laplacian and its gradient from [[def-author-fd2999663761-temporal-angle-data]]. The differential inequality in the Statement is an explicit hypothesis of this algebraic lemma, not a geometric conclusion proved here.

[F2] The hypersurface carries a smooth positive-definite metric $h$ in the general sense of [[math:def-riemannian-metric-and-riemannian-manifold]], allowing an actual boundary and smoothness up to it. The metric-dual gradient, the coordinate Hessian formula $(\operatorname{Hess}_h u)_{ij}=\partial_i\partial_j u-\Gamma^k{}_{ij}\partial_k u$, and the divergence connection formula are supplied by [[math:prop-gradient-hessian-and-divergence-connection-formulas]]. The identity $\Delta_h u=\operatorname{tr}_h\operatorname{Hess}_h u=\operatorname{div}_h\operatorname{grad}_h u$ and its smooth one-sided boundary convention are [[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]]. Only the intrinsic operator convention is borrowed from the temporal angle data; no ambient Lorentzian or maximality assumption is used here.

[F3] The scalar sum, product, quotient and chain rules are [[math:lem-derivative-algebra-and-chain-rules]], applied to each coordinate derivative.

[F4] The inverse identity for $\operatorname{arcosh}$ on $[1,\infty)$ is [[math:thm-inverse-hyperbolic-logarithm-formulas]]. The hyperbolic identities, quotient definitions and derivatives, including $(\cosh s)^{\prime}=\sinh s$, $(\tanh s)^{\prime}=\operatorname{sech}^2s$ and $0<\tanh s<1$ for $s>0$, are [[math:thm-hyperbolic-identities-and-derivatives]]. The formula $(\log x)^{\prime}=1/x$ for $x>0$ is [[math:thm-logarithm-derivative-and-integral]]; positive-base powers and their derivative formula, used for the square root on $(0,\infty)$, are [[math:thm-real-power-continuity-and-derivatives]]. Iterating these derivative formulas with [F3] gives smoothness on the indicated open domains.

## Proof

**Given:** The smooth function and differential inequality in the Statement. **Goal:** Derive the logarithmic inequality.

1.1 Since $v>2$, [F4] makes $\eta=\operatorname{arcosh}v$ smooth and positive, with $v=\cosh\eta$. Set $H(s)=\log\cosh s$, so $f=H(\eta)$. The scalar rules and the logarithm and hyperbolic derivatives give $H^{\prime}(s)=\sinh s/\cosh s=\tanh s$ and $H^{\prime\prime}(s)=\operatorname{sech}^2s$. [F3, F4, given, algebra]

2.1 In an arbitrary interior coordinate chart, the scalar chain and product rules give $\partial_i(H(\eta))=H^{\prime}(\eta)\partial_i\eta$ and $\partial_i\partial_j(H(\eta))=H^{\prime\prime}(\eta)\partial_i\eta\,\partial_j\eta+H^{\prime}(\eta)\partial_i\partial_j\eta$. Substitution in the coordinate Hessian formula yields $\operatorname{Hess}_h(H(\eta))=H^{\prime\prime}(\eta)d\eta\otimes d\eta+H^{\prime}(\eta)\operatorname{Hess}_h\eta$. Taking the metric trace and using the metric-dual characterization of the gradient gives $\nabla f=\tanh\eta\,\nabla\eta$ and $\Delta f=\tanh\eta\,\Delta\eta+\operatorname{sech}^2\eta\,|\nabla\eta|^2$. At any actual boundary point these identities follow by continuity from the interior in a boundary half-chart: the metric, inverse metric, function derivatives and operator coefficients are smooth up to that point, and the operators there have the one-sided convention in [F1] and [F2]. [F1, F2, F3, step 1.1, algebra]

3.1 Multiply the assumed lower bound for $\Delta\eta$ by $\tanh\eta>0$. Since $\tanh\eta\coth\eta=1$, step 2.1 gives $\Delta f\ge(\tfrac14+\operatorname{sech}^2\eta)|\nabla\eta|^2-Cv^2\ge\tfrac14|\nabla f|^2-Cv^2$, where the last step uses $|\tanh\eta|\le1$ and the nonnegativity of the squared norm. This also holds at actual boundary points under the stated smooth one-sided convention. [F1, F2, F4, step 2.1, given, algebra] ∎

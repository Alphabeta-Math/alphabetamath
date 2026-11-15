---
id: def-stationary-asymptotic-decay-data
title: Differentiated asymptotic bounds and parameter uniformity
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - physics:def-gr-fx-adm-end
  - math:def-ck-and-multi-index-notation-in-several-variables
dependency_roles:
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  physics:def-gr-fx-adm-end: mathematical-premise
  math:def-ck-and-multi-index-notation-in-several-variables: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Armin Schikorra, Partial Differential Equations I & II (version October
        1, 2025)
      url: https://sites.pitt.edu/~armin/pde2022/pde.pdf
      locator: Section 8, introductory Hölder definitions, printed p. 139 (PDF page
        139), before Section 8.1.
      statement: The Hölder seminorm is the supremum of |f(x)-f(y)|/|x-y|^alpha over
        distinct points of the domain; C^{k,alpha} requires C^k regularity and
        alpha-Hölder kth derivatives.
      hypotheses: An open Euclidean domain, 0 < alpha < 1, and a nonnegative integer
        k; C^k regularity is required for the derivative formulation. The
        seminorm formula may take the value +infinity.
      reading_limits: Consulted the title/version and introductory Hölder definitions
        on printed p. 139. Used only for ordinary Hölder notation. The annular
        weights and parameter-uniform convention are specified locally using the
        declared library interfaces; this passage is not claimed to contain that
        complete weighted definition or an ADM-end result.
dependency_level: 0
---

## Definition

Fix a Cartesian exterior chart $E=\{x\in\mathbb R^3: r=|x|>R_0\}$ with $R_0>0$. Let $m$ be a nonnegative integer, $b\in\mathbb R$, and let $u$ be a scalar or a finite array of scalar functions of class $C^m$ on $E$. For a multi-index $\beta=(\beta_1,\beta_2,\beta_3)$ of nonnegative integers write $|\beta|=\beta_1+\beta_2+\beta_3$ and $\partial^\beta=\partial_{x^1}^{\beta_1}\partial_{x^2}^{\beta_2}\partial_{x^3}^{\beta_3}$. The notation $u=O_m(r^{-b})$ means that there are a radius $R_1>R_0$ and finite constants $C_\beta\geq0$ such that every component satisfies $|\partial^\beta u(x)|\leq C_\beta r^{-b-|\beta|}$ for all $|\beta|\leq m$ and $r\geq R_1$. The estimate is uniform over angular directions in this chart.

For a family $(u_\lambda)_{\lambda\in\Lambda}$ on the same exterior chart, the estimate is **uniform on the parameter set** $\Lambda$ when the same radius and constants work for every $\lambda\in\Lambda$. Separate estimates for each parameter allow these quantities to depend on $\lambda$ and do not by themselves imply uniformity, including as a parameter approaches a boundary value.

For $0<\alpha<1$, define the Hölder seminorm on a set $A$ by $[v]_{\alpha;A}=\sup_{x,y\in A,\,x\ne y}|v(x)-v(y)|/|x-y|^\alpha$, allowing $+\infty$. Write $A_R=\{x\in\mathbb R^3:R<|x|<2R\}$. A **weighted $C^{m,\alpha}$ bound of decay order $b$** means that for some $R_1>R_0$ and finite $C$, for every $R\geq R_1$ and every component,
$$\sum_{|\beta|\leq m} R^{b+|\beta|}\sup_{A_R}|\partial^\beta u|+\sum_{|\beta|=m}R^{b+m+\alpha}[\partial^\beta u]_{\alpha;A_R}\leq C.$$
For a family, uniformity means that the same $R_1$ and $C$ work for every parameter. These bounds are chart-dependent data; they do not assert coordinate invariance or the existence of a particular end.

## Definition references

[[math:def-ck-and-multi-index-notation-in-several-variables]]

[[physics:def-gr-fx-adm-end]]

[[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

## Facts & Assumptions

[F1] The fixed-chart end interface uses differentiated $O_k$ bounds with Cartesian derivatives and angular uniformity. [[physics:def-gr-fx-adm-end]]

[F2] Hölder seminorms measure differences divided by a power of Euclidean distance, and scaled norms weight derivatives and seminorms by the corresponding radius powers. [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

## Justification

The finite array and the finite set of multi-indices allow one common radius to be chosen as the maximum of finitely many radii in the componentwise convention of [F1]. The definition uses no limiting choice of constants. On $A_R$, the first sum in the weighted bound controls each derivative at its stated decay order, since $R<r<2R$; the second sum explicitly imposes the scaled Hölder control described in [F2]. For example, on $r>1$ let $u_s(x)=s^{-1}r^{-1}$ for $0<s\leq1$. Each $u_s$ is $O_0(r^{-1})$ with constant $s^{-1}$, but no common constant works for all $s$, even at any one fixed point of the exterior. Thus separate bounds need not be uniform.

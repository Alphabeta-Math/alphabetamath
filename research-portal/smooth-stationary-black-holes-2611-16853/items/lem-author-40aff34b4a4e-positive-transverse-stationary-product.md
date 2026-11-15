---
id: lem-author-40aff34b4a4e-positive-transverse-stationary-product
title: A complete stationary flow transverse positively to a Cauchy section is a
  product
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-spacelike-maximal-hypersurface-data
  - lem-author-40aff34b4a4e-cauchy-timelike-flow-product
  - math:def-axiom-of-choice
  - def-causal-exterior-and-boundary-data
  - math:thm-fundamental-theorem-on-flows
  - math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  lem-author-40aff34b4a4e-cauchy-timelike-flow-product: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 4
---

## Statement

Work in ZFC, including the Axiom of Choice. Let $(E,g)$ be a connected smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$, globally hyperbolic with a smooth spacelike Cauchy hypersurface $C$. Let $n$ be the future-directed unit normal to $C$. Let $T$ be a smooth complete vector field whose every orbit meets $C$, and suppose $N=-g(T,n)>0$ on $C$. Then $F:\mathbb R\times C\to E$, $F(t,c)=\Phi_t^T(c)$, is a diffeomorphism, where the domain has its product smooth structure. Completeness and meeting $C$ refer to orbits in $E$; no causality or Killing condition on $T$ is required.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-causal-exterior-and-boundary-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[math:def-axiom-of-choice]]

[[math:thm-fundamental-theorem-on-flows]]

[[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

[[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure]]

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice and its countable/dependent-choice consequences. Choice is inherited through the Cauchy-product supplier in [F2]; the crossing and inverse arguments below need no additional choice assumption. [[math:def-axiom-of-choice]]

[F1] Use only the Lorentzian sign and local-flow notation of the stationary-data interface; $T$ here need not be Killing. Global hyperbolicity and the Cauchy condition are relative to $E$ with the causal interface's conventions. The hypersurface interface gives the future unit normal and $T=Nn+X$ along $C$, with $N=-g(T,n)$ and $X\in TC$. [[def-stationary-lorentzian-data]] [[def-causal-exterior-and-boundary-data]] [[def-spacelike-maximal-hypersurface-data]]

[F2] For this connected globally hyperbolic time-oriented spacetime and its smooth spacelike Cauchy hypersurface, the Cauchy-product lemma supplies a smooth global function $\rho:E\to\mathbb R$ with $\rho^{-1}(0)=C$ and $d\rho(n)>0$ on $C$. Its auxiliary timelike flow is not identified with $T$. [[lem-author-40aff34b4a4e-cauchy-timelike-flow-product]]

[F3] The maximal flow of a smooth vector field is smooth and satisfies the flow group law. For a complete field its domain is $\mathbb R\times E$, and each time-$t$ map is a diffeomorphism of $E$ with inverse the time-$(-t)$ map. [[math:thm-fundamental-theorem-on-flows]] [[math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains]]

[F4] A smooth map with invertible differential at a point restricts to a diffeomorphism between neighborhoods of that point and its image. [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[F5] Use the canonical product smooth structure on $\mathbb R\times C$. A diffeomorphism is a smooth bijection with smooth inverse; a local diffeomorphism has such inverses on open neighborhoods. [[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure]] [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

## Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** The asserted global product diffeomorphism.

1.1 Let $\rho$ be the function from [F2]. For any orbit $\gamma(t)=\Phi_t^T(p)$, [F3] makes $a(t)=\rho(\gamma(t))$ smooth, and each zero is a crossing of $C$. There $a'(t)=d\rho(T)=N\,d\rho(n)>0$ by [F1], since $d\rho$ vanishes on $TC$. There cannot be two such zeros: the zero set on the compact interval between them is closed, and every zero is isolated by its positive derivative, so that zero set is finite. Between consecutive zeros the sign would be positive just after the first and negative just before the second, requiring another zero by continuity. Thus every orbit meets $C$ at most once in parameter, and the assumed intersection gives exactly once. [given, A1, F1, F2, F3]

2.1 By completeness and [F3], $F(t,c)=\Phi_t^T(c)$ is defined and smooth on all of the product in [F5]. It is surjective: if $\Phi_s^T(p)=c\in C$, then $p=\Phi_{-s}^T(c)$. If $F(t,c)=F(s,d)$, the flow law gives $d=\Phi_{t-s}^T(c)$, and step 1.1 forces $t=s$ and $c=d$, including exclusion of a periodic return. At $(0,c)$ its differential is $(a,v)\mapsto aT_c+v$ for $v\in T_cC$; this is invertible because $T_c=Nn+X$ with $N>0$. The flow law gives $dF_{(t,c)}(a,v)=d(\Phi_t^T)_c(aT_c+v)$, which is invertible since $\Phi_t^T$ is a diffeomorphism by [F3]. By [F4], $F$ is a local diffeomorphism everywhere. Bijectivity makes its smooth local inverses agree on overlaps, giving a global smooth inverse and hence the claimed diffeomorphism. [given, F1, F3, F4, F5, step 1.1] ∎

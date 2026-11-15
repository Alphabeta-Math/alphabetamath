---
title: A smooth Cauchy hypersurface gives a connected timelike-flow product
status: draft
research_item: lem-author-40aff34b4a4e-cauchy-timelike-flow-product
dependency_level: 3
---

## Prerequisites

- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [lem-author-e7cde3233cd7-cauchy-section-product](item-lem-author-e7cde3233cd7-cauchy-section-product)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:def-differential-of-a-smooth-real-valued-function](https://alphabetamath.cc/item/def-differential-of-a-smooth-real-valued-function)
- [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)
- [math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map)
- [physics:lem-gr-finite-smooth-volume-density](https://alphabetamath.cc/physics/item/lem-gr-finite-smooth-volume-density)
- [physics:thm-gr-volume-time-function](https://alphabetamath.cc/physics/item/thm-gr-volume-time-function)
- [physics:thm-gr-smooth-cauchy-temporal-splitting](https://alphabetamath.cc/physics/item/thm-gr-smooth-cauchy-temporal-splitting)
- [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)


## Statement

Let $E$ be a connected smooth globally hyperbolic time-oriented spacetime and $C$ a smooth spacelike Cauchy hypersurface, with the causal and hypersurface conventions below. Then $C$ is connected and there is a smooth diffeomorphism $\mathbb R\times C\to E$ given by an auxiliary complete future timelike flow. Its inverse first coordinate $\rho$ satisfies $\rho^{-1}(0)=C$ and $d\rho(n)>0$ on $C$ for the future unit normal $n$. The auxiliary flow is not asserted to be the stationary flow.

## Statement references

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[lem-author-e7cde3233cd7-cauchy-section-product](item-lem-author-e7cde3233cd7-cauchy-section-product)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:def-differential-of-a-smooth-real-valued-function](https://alphabetamath.cc/item/def-differential-of-a-smooth-real-valued-function)

[math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map)

[physics:lem-gr-finite-smooth-volume-density](https://alphabetamath.cc/physics/item/lem-gr-finite-smooth-volume-density)

[physics:thm-gr-volume-time-function](https://alphabetamath.cc/physics/item/thm-gr-volume-time-function)

[physics:thm-gr-smooth-cauchy-temporal-splitting](https://alphabetamath.cc/physics/item/thm-gr-smooth-cauchy-temporal-splitting)

[math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

## Facts & Assumptions

[F1] Work in ZFC, including the Axiom of Choice and its countable/dependent-choice consequences. The causal and Cauchy conventions and the future unit normal and normal–tangent decomposition are those of [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) and [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data). Choice is used in the density, volume-time and temporal-splitting suppliers in [F5]. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F2] For a nonempty globally hyperbolic time-oriented smooth Lorentzian four-manifold with a smooth spacelike Cauchy hypersurface, the prescribed-Cauchy-section product lemma proves that the section is connected if the manifold is connected. Only this connectedness conclusion is used here; the future-directed flow based at the prescribed section will be constructed below. [lem-author-e7cde3233cd7-cauchy-section-product](item-lem-author-e7cde3233cd7-cauchy-section-product)

[F3] A diffeomorphism is a smooth bijection with smooth inverse. Equip $\mathbb R\times C$ with its canonical product smooth structure; its first projection is smooth, since in each product chart it is a Euclidean coordinate projection. [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds) [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[F4] A global smooth flow satisfies $\Phi_0=\operatorname{id}$ and $\Phi_s\circ\Phi_r=\Phi_{s+r}$, and its parameter curves are integral curves of its generating field. In particular $\Phi_s^{-1}=\Phi_{-s}$. Differentials are the induced linear maps on tangent spaces; for a real-valued smooth function, $df_p(v)=v([f])$. The chain rule is $d(G\circ H)_p=dG_{H(p)}\circ dH_p$. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map) [math:def-differential-of-a-smooth-real-valued-function](https://alphabetamath.cc/item/def-differential-of-a-smooth-real-valued-function) [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[F5] On a nonempty time-oriented smooth Lorentzian four-manifold, the finite-density lemma supplies a positive smooth density whose measure has total mass one, is positive on nonempty open sets and vanishes on chart-Lebesgue-null Borel sets. Under global hyperbolicity this measure satisfies exactly the hypotheses of the volume-time theorem. Supply that theorem's volume time to the smooth Cauchy temporal splitting theorem. Its Statement (d) supplies a complete smooth future-directed timelike field $Z$ and global smooth flow $\Phi$, and (e) supplies a smooth function $\tau$ and a diffeomorphism $\Psi:\mathbb R\times\tau^{-1}(0)\to E$ with $\Psi(s,z)=\Phi_s(z)$ and $\tau(\Psi(s,z))=s$. [physics:lem-gr-finite-smooth-volume-density](https://alphabetamath.cc/physics/item/lem-gr-finite-smooth-volume-density) [physics:thm-gr-volume-time-function](https://alphabetamath.cc/physics/item/thm-gr-volume-time-function) [physics:thm-gr-smooth-cauchy-temporal-splitting](https://alphabetamath.cc/physics/item/thm-gr-smooth-cauchy-temporal-splitting)

[F6] A smooth map whose differential at a point is an isomorphism has a smooth inverse on suitable neighborhoods of that point and its image. [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

## Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Its asserted conclusions.

1.1 If $E$ is empty, so is $C$, and the empty flow and product map give every conclusion, with the normal-derivative condition vacuous. Otherwise [F2] gives connectedness of $C$. Apply the density, volume-time and temporal-splitting suppliers in [F5] to $E$, with the conventions and choice assumptions of [F1], obtaining $Z$, $\Phi$, $\tau$ and $\Psi$ as stated there. [given, F1, F2, F5]

2.1 For any $p\in E$, write $p=\Psi(a,z)=\Phi_a(z)$ using [F5]. Then [F4] and [F5] give $\tau(\Phi_s(p))=\tau(\Phi_{s+a}(z))=s+a=\tau(p)+s$. Hence neither parameter end of the future timelike orbit $s\mapsto\Phi_s(p)$ converges to a point of $E$: continuity of $\tau$ would contradict this divergence. By [F1] the orbit is inextendible and meets $C$ at exactly one parameter value. Define $F(s,c)=\Phi_s(c)$. Every point lies on such an orbit, so $F$ is surjective. If $F(s,c)=F(r,d)$, the flow law gives $d=\Phi_{s-r}(c)$. Since the orbit of $c$ meets $C$ at the unique parameter value zero, $s=r$ and $d=c$. Thus $F$ is bijective and $F(0,c)=c$. [F1, F4, F5, step 1.1]

3.1 The map $F$ is smooth in the product structure of [F3], since it is the restriction of the smooth flow to the embedded section. By the flow law and chain rule in [F4], its differential is $dF_{(s,c)}(a,v)=(d\Phi_s)_c(aZ_c+v)$ for $a\in\mathbb R$ and $v\in T_cC$. The map $d\Phi_s$ is invertible, since $\Phi_{-s}$ is its smooth inverse. A timelike vector cannot lie in the positive-definite three-plane $T_cC$, so $(a,v)\mapsto aZ_c+v$ is a linear isomorphism onto $T_cE$. Thus $dF$ is invertible everywhere. By [F6] local smooth inverses exist, and bijectivity makes them agree with the global inverse. Therefore $F$ is a diffeomorphism. [F1, F3, F4, F5, F6, step 2.1]

4.1 Put $\rho=\operatorname{pr}_1\circ F^{-1}$, smooth by [F3] and step 3.1. Since $F(0,c)=c$ and $F$ is bijective, $\rho^{-1}(0)=C$, and $\rho(\Phi_s(c))=s$ for every $c\in C$. [F3, F4, step 2.1, step 3.1]

5.1 On $C$, the function $\rho$ is identically zero. Restricting to the section and applying the differential and chain rule in [F4] shows that $d\rho$ annihilates $TC$. Differentiating $\rho(\Phi_s(c))=s$ at zero with the integral-curve law gives $d\rho(Z)=1$. Decompose $Z=\alpha n+V$ there by [F1], with $V\in TC$ and $\alpha=-g(Z,n)$. In a Lorentz-orthonormal frame with future unit time vector $n$, the future timelike vector $Z$ has positive time component, so $\alpha>0$. Consequently $1=d\rho(Z)=\alpha\,d\rho(n)$ and $d\rho(n)=1/\alpha>0$. This calculation uses the auxiliary timelike field and makes no identification with a stationary field. [given, F1, F4, F5, step 4.1] ∎

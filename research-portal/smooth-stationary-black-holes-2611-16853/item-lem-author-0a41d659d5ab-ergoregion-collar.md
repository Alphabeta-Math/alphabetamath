---
title: The non-timelike region is confined to the local-rigidity collar
status: published
research_item: lem-author-0a41d659d5ab-ergoregion-collar
dependency_level: 5
sources:
  references:
    - title: S. Alexakis, A. D. Ionescu and S. Klainerman, Rigidity of stationary
        black holes with small angular momentum on the horizon
      url: https://arxiv.org/pdf/1304.0487v2
      locator: §1.1.3 Theorem 1.2, PDF p. 4; final Proof of Proposition 1.3, PDF p. 10
      statement: The local rotational Killing field Z commuting with T exists on an
        open Omega containing S0. With the quantitative bounds fixed, Omega
        contains Sigma1 minus Sigma_(1+rho) for a rho=rho(A)>0.
      hypotheses: The GR and SBS setting of the source, with its fixed quantitative
        local geometry; the maximal-section and smallness assumptions are
        retained in the present application. No global extension of Z is
        asserted by this local input.
      reading_limits: Consulted Theorem 1.2 and the quantitative collar paragraph in
        the final proof of Proposition 1.3 for the local field and rho(A). These
        conclusions are imported, not locally proved. The separate local
        rigidity paper cited as [1] was consulted at the passages recorded in
        the next reference for the common-period meaning; its Carleman
        construction was not reconstructed. No global field extension was
        reviewed.
    - title: S. Alexakis, A. D. Ionescu and S. Klainerman, Hawking's local rigidity
        theorem without analyticity
      url: https://web.math.princeton.edu/~seri/papers/LocalH.pdf
      locator: Abstract, PDF p. 1; Theorem 1.2 and (1.1), PDF p. 2; section 5,
        Proposition 5.2, PDF p. 17, and its proof, PDF pp. 17–18
      statement: The local rotational field Z is nontrivial and commutes with T.
        Proposition 5.2 specifies its rotational property by one constant t0>0
        for which its time-t0 local flow map is the identity on a neighborhood
        of the bifurcation sphere. This reference supplies the common-period
        meaning, not a quantitative collar radius.
      hypotheses: A smooth four-dimensional Ricci-flat Lorentzian spacetime with a
        local regular bifurcate non-expanding horizon and a Killing field T
        tangent to both branches and not identically zero on the bifurcation
        sphere. The application retains the full AIK quantitative package.
      reading_limits: Consulted the abstract, Theorem 1.2, the paragraph containing
        (1.1), and Proposition 5.2 with its printed proof for the common-period
        assertion. The auxiliary lemmas and the local Carleman construction were
        not reconstructed or independently verified. No quantitative dependence
        of a collar radius is imported from this reference.
---

## Prerequisites

- [def-author-0a41d659d5ab-aik-quantitative-package](item-def-author-0a41d659d5ab-aik-quantitative-package)
- [lem-author-0a41d659d5ab-annular-timelike-gap](item-lem-author-0a41d659d5ab-annular-timelike-gap)
- [lem-author-0a41d659d5ab-asymptotic-timelike-gap](item-lem-author-0a41d659d5ab-asymptotic-timelike-gap)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Rigidity of stationary black holes with small angular momentum on the horizon · §1.1.3 Theorem 1.2, PDF p. 4; final Proof of Proposition 1.3, PDF p. 10 `](https://arxiv.org/pdf/1304.0487v2)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Hawking's local rigidity theorem without analyticity · Abstract, PDF p. 1; Theorem 1.2 and (1.1), PDF p. 2; section 5, Proposition 5.2, PDF p. 17, and its proof, PDF pp. 17–18 `](https://web.math.princeton.edu/~seri/papers/LocalH.pdf)


## Statement

For the AIK quantitative package there is an open local-rigidity neighborhood $\Omega$ of $S_0$ carrying a rotational Killing field $Z$ commuting with $T$. For sufficiently small $\epsilon>0$ depending only on $A$, the bound $\sup_{S_0}|g(T,T)|<\epsilon^2$ implies $\{p\in\Sigma_1:g(T,T)(p)\ge0\}\subset\Omega$. This set includes the stationary-limit points and uses the source Proposition 1.3 non-strict convention. Here **rotational** means $Z\not\equiv0$ and there is a common $t_0>0$ such that its local flow $\phi^Z$ is defined through time $t_0$ on $\Omega$ and $\phi^Z_{t_0}(p)=p$ for every $p\in\Omega$. Individual orbits may have shorter periods or be fixed; no normalization of $t_0$ or completeness on all of $M$ is asserted.

## Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The stationary package and its fixed quantitative constant are those of [def-author-0a41d659d5ab-aik-quantitative-package](item-def-author-0a41d659d5ab-aik-quantitative-package).

[F2] The source estimates imply timelikeness on $1+\epsilon^{1/100}\le r\le R_1$ for sufficiently small $\epsilon(A)$. [lem-author-0a41d659d5ab-annular-timelike-gap](item-lem-author-0a41d659d5ab-annular-timelike-gap)

[F3] The asymptotic end $r>R_1$ is timelike. [lem-author-0a41d659d5ab-asymptotic-timelike-gap](item-lem-author-0a41d659d5ab-asymptotic-timelike-gap)

[F4] The explicit External input gives $\Omega$, a nontrivial rotational Killing field $Z$ commuting with $T$, its common local period $t_0>0$, and $\rho(A)>0$ such that $\Sigma_1\setminus\Sigma_{1+\rho}\subset\Omega$.

[F5] Local flows and their time maps use [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow). The period condition is local to the rigidity neighborhood; no global flow on $M$ is assumed.

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conditional conclusion.

1.1 Choose the horizon parameter below the threshold for [F2] and also so that $\epsilon^{1/100}<\rho$. This is possible because $\rho>0$ is fixed by the source geometric bounds, independently of the subsequently chosen small parameter. By [F2] and [F3], every point with $r\ge1+\epsilon^{1/100}$ has $g(T,T)<0$. [F1, F2, F3, F4, given]

2.1 Therefore a point of $\Sigma_1$ with $g(T,T)\ge0$ must satisfy $1<r<1+\epsilon^{1/100}<1+\rho$, so lies in $\Sigma_1\setminus\Sigma_{1+\rho}\subset\Omega$. The Killing-field existence, commutation and common-period assertions are exactly [F4], with the local-flow meaning in [F5]; this local application asserts no extension of $Z$ outside $\Omega$. [step 1.1, F1, F4, F5, algebra] ∎

## External input

Import the local rotational-rigidity conclusion of AIK Theorem 1.2 and the quantitative collar inclusion stated in its final proof of Proposition 1.3. The common local period in the rotational conclusion is specified by Proposition 5.2 of the separately cited local-rigidity paper: the time-$t_0$ map is the identity on a neighborhood of $S_0$. Both existence and periodicity remain imported premises. Combining them with the separately imported estimates and the local norm/asymptotic calculations proves the stated confinement, without claiming a reconstruction of the local Carleman construction.

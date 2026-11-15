---
title: The ADM-source mass and angular-momentum parameters
status: published
research_item: def-author-ad064c44a1cc-adm-angular-momentum-parameters
dependency_level: 5
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: §1.1 GR (1.1), definition of J=|S|, mass-one paragraph before (1.2),
        and Theorem 1.1
      statement: Equation (1.1) labels M>0 as ADM mass and S as ADM angular momentum,
        with J=|S| and epsilon_123=1. The source rescales to M=1; Theorem 1.1
        fixes A before choosing j_*(A)>0 and uses the normalized angular
        magnitude and the effective constant of (1.3). This citation imports the
        parameter conventions and application conditions, not the rigidity
        conclusion.
      hypotheses: The charge labels refer to GR's stationary asymptotic chart. Theorem
        1.1 assumes GR, SBS, maximality of Sigma_1 and J<M^2, with M=1, Abar<=A
        and J<j_*(A), in the source's connected oriented time-oriented smooth
        vacuum four-spacetime with smooth Killing field T. Its geometric bound
        applies to the actual mass-one chart package. The source mass M is
        denoted M_0 locally.
      reading_limits: Retrieved and read arXiv HTML v1, section 1.1, from the opening
        setup through GR, (1.1), the charge/decay conventions, SBS, maximality,
        the mass-one paragraph, (1.2)-(1.3), and Theorem 1.1. Imported only the
        parameter conventions and quantitative application conditions; the
        rescaling bookkeeping is checked locally. No rigidity proof, ADM
        surface-integral identification, or supplier proof review was performed.
---

## Prerequisites

- [def-author-ad064c44a1cc-adm-gr-sbs](item-def-author-ad064c44a1cc-adm-gr-sbs)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [` Alexandru F. Radu, Rigidity of stationary black holes with small ADM angular momentum · §1.1 GR (1.1), definition of J=|S|, mass-one paragraph before (1.2), and Theorem 1.1 `](https://arxiv.org/html/2610.09729v1)


## Definition

In the preceding end expansion, $M_0>0$ is the coefficient called ADM mass in the Radu source, $S=(S^1,S^2,S^3)$ is its ADM angular momentum vector, and $J=|S|=\sqrt{\sum_i(S^i)^2}$ is the nonnegative magnitude, not a signed component and not the Kerr parameter $a$. These are the source's fixed charge and orientation conventions, as specified by its asymptotic chart and the leading $g_{0i}$ coefficient. No equality with a newly introduced alternative surface-integral convention is asserted or needed here.

The subextremal parameter condition for the quantitative theorem is $J<M_0^2$. In the mass-one normalization used by that theorem, the normalized mass is exactly $1$ and its angular magnitude is the dimensionless $J/M_0^2$, thereafter denoted $J$ by the source. The quantitative theorem must be applied to the rescaled mass-one data and their actual geometric constant; numerical smallness of an unnormalized dimensionful angular momentum is not its condition.

## Facts & Assumptions

[F1] [def-author-ad064c44a1cc-adm-gr-sbs](item-def-author-ad064c44a1cc-adm-gr-sbs) provides the source end and its coefficients. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) fixes their differentiated remainder convention.

## Justification

The finite vector $S$ determines its Euclidean norm uniquely, and positivity of $M_0$ makes $J/M_0^2$ defined. Dimensional rescaling of the stationary end uses $t'=t/M_0$, $x'=x/M_0$ and $g'=M_0^{-2}g$ expressed in these coordinates, with normalized stationary field $T'=M_0T=\partial_{t'}$. The leading temporal coefficient becomes $-1+2/r'$ and the leading mixed coefficient has vector $S/M_0^2$, by substituting $x=M_0x'$. Thus the stated mass-one labels match the source normalization. This checks the parameter bookkeeping only; bounds for a geometric constant must still be checked on those rescaled data, not transported without calculation.

---
title: Radial barrier, absorption and height decay
status: draft
research_item: pthm-radial-barrier-height-decay
dependency_level: 14
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pages 14–15, §3.2.1, equations (3.5)–(3.7)
      statement: The article obtains a radial barrier, compares the normalized graph
        height with it, and absorbs a radial slope estimate to obtain uniform
        inverse-power height decay.
      hypotheses: The article's candidate maximal sections and normalized ends, with q
        in a fixed positive interval and the stated end estimates.
      reading_limits: Read the frozen article text at the cited passage. This citation
        attributes the claim; the proof below uses the declared completed
        suppliers and a local calculation.
---

PDF p. 14: ` §3.2.1; (3.6)–(3.7) `; PDF p. 15: ` §3.2.1; (3.6)–(3.7) `

## Prerequisites

- [pthm-maximal-graph-equation](item-pthm-maximal-graph-equation)
- [pthm-end-lapse-slope](item-pthm-end-lapse-slope)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)


## Statement

Fix $\delta\in(0,1)$ and $\mu\in(0,1)$. Assume the candidate family, normalized Cartesian ends and uniform estimates of [pthm-maximal-graph-equation](item-pthm-maximal-graph-equation) and [pthm-end-lapse-slope](item-pthm-end-lapse-slope). In particular, each normalized graph height $\widetilde u_q$ tends to zero as $r_q=|x_q|\to\infty$, uniformly in direction for that fixed $q$; the sections are assumed to exist. Write $\mathscr L_q v=a_q^{ij}\partial_{ij}v+b_q^j\partial_jv$, using the coefficients supplied by the graph equation, evaluated on the given graph.

There are $R_{\delta,\mu}$ and $c_{\delta,\mu}>0$, independent of $q\in[\delta,1]$, such that $\mathscr L_q(r_q^{-\mu})\le-c_{\delta,\mu}r_q^{-\mu-2}$ for $r_q\ge R_{\delta,\mu}$. Fix any $r_*\ge R_{\delta,\mu}$ and put $M_q(r_*)=\max_{r_q=r_*}|\widetilde u_q|$. There is a constant $K_{\delta,\mu}$ independent of $q$ and $r_*$ such that, for $r_q\ge r_*$, $|\widetilde u_q(x_q)|\le(M_q(r_*)+K_{\delta,\mu}/r_*)(r_*/r_q)^\mu$. If $C_\delta$ is a uniform constant in $|\partial_{x_q}\widetilde u_q|\le C_\delta r_q^{-1/2}$, then $M_q(r_*)\le4^{-\mu}(M_q(r_*)+K_{\delta,\mu}/r_*)+2C_\delta\sqrt{r_*}$. Consequently, for a fixed sufficiently large $r_*$, $|\widetilde u_q|\le C_{\delta,\mu}r_q^{-\mu}$ on $r_q\ge r_*$, with $C_{\delta,\mu}$ independent of $q$.

## Facts & Assumptions

[F1] On a common end the graph equation is $\mathscr L_q\widetilde u_q=f_q$, with $a_q^{ij}=\delta^{ij}+O(r_q^{-1})$, $b_q^j=O(r_q^{-2})$ and $|f_q|\le C r_q^{-3}$ uniformly in $q$. The principal coefficient is uniformly positive definite on a sufficiently distant common end. [pthm-maximal-graph-equation](item-pthm-maximal-graph-equation)

[F2] On a common end the normalized slope satisfies $|\partial_{x_q}\widetilde u_q|\le C_\delta r_q^{-1/2}$ uniformly in $q$. [pthm-end-lapse-slope](item-pthm-end-lapse-slope)

[F3] The normalized end uses $r_q=|x_q|$, and the graph-height normalization requires convergence to zero uniformly in angle for each fixed parameter. [def-stationary-maximal-graph](item-def-stationary-maximal-graph)

## Proof

**Given:** The family and hypotheses in the Statement.

**Goal:** Establish the radial barrier, comparison, absorption inequality and uniform height decay.

1.1 In three Cartesian spatial dimensions, direct differentiation gives $\Delta(r^{-\mu})=-\mu(1-\mu)r^{-\mu-2}$, while $|\partial_i r^{-\mu}|\le C_\mu r^{-\mu-1}$ and $|\partial_{ij}r^{-\mu}|\le C_\mu r^{-\mu-2}$. The coefficient errors in [F1] therefore contribute at most $C_{\delta,\mu}r^{-\mu-3}$. Since $\mu(1-\mu)>0$, increasing the common radius gives the claimed strictly negative bound, uniformly in $q$. [F1, F3, algebra]

2.1 Fix $r_*$ beyond that radius and choose $K_{\delta,\mu}>C/c_{\delta,\mu}$, with $C$ from [F1]. Set $B=(M_q(r_*)+K_{\delta,\mu}/r_*)(r_*/r)^\mu$. Then $\mathscr L_q(\pm\widetilde u_q-B)>0$ for $r\ge r_*$: indeed $-\mathscr L_qB$ is strictly greater than $Cr^{-3}$ because $r\ge r_*$ and $\mu<1$. At the inner sphere $\pm\widetilde u_q-B\le0$. For each fixed $q$, [F3] and $B\to0$ imply that on a sufficiently distant outer sphere this difference is at most any prescribed $\varepsilon>0$. On the closed intervening annulus it cannot attain a positive interior maximum exceeding $\varepsilon$: at such a maximum the gradient vanishes and the Hessian is negative semidefinite, so positive definiteness of $a_q$ gives $\mathscr L_q(\pm\widetilde u_q-B)\le0$, a contradiction. Letting the outer radius tend to infinity and then $\varepsilon\downarrow0$ proves the comparison bound. [F1, F3, step 1.1, algebra]

3.1 Along each radial segment from radius $r_*$ to $4r_*$, [F2] bounds the height change by $C_\delta\int_{r_*}^{4r_*}s^{-1/2}\,ds=2C_\delta\sqrt{r_*}$. Taking the maximum over directions and applying step 2.1 at radius $4r_*$ yields the stated absorption inequality. [F2, step 2.1, algebra]

4.1 Since $1-4^{-\mu}>0$, the inequality in step 3.1 gives a bound on $M_q(r_*)$ independent of $q$ once the common $r_*$ is fixed. Substitution into step 2.1 gives the asserted $C_{\delta,\mu}r^{-\mu}$ bound. [step 2.1, step 3.1, algebra] ∎

## Source notes

The article reference attributes the original estimates. The proof does not use that reference as a premise; the comparison argument is given on bounded annuli and uses each individual graph's end limit, not a uniform rate of convergence in $q$.

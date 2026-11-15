---
id: lem-author-86990d62062f-global-decaying-barrier
title: A positive global supersolution with the exact exterior decay
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-exterior-weighted-elliptic-data
  - def-stationary-asymptotic-decay-data
  - lem-author-86990d62062f-compact-domain-poisson
  - math:def-riemannian-gradient-of-a-smooth-function
dependency_roles:
  def-exterior-weighted-elliptic-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  lem-author-86990d62062f-compact-domain-poisson: mathematical-premise
  math:def-riemannian-gradient-of-a-smooth-function: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
sources:
  references:
    - title: David Gilbarg and Neil S. Trudinger, Elliptic Partial Differential
        Equations of Second Order, 2001 reprint of the 1998 edition
      url: https://djvu.online/file/jxRRleAzbYjsl
      locator: "Chapter 6, section 6.4: Theorem 6.17, printed p.109; Theorem 6.19,
        printed p.111, and its local-boundary-portion conclusion on printed
        p.112."
      statement: A classical C^2 solution of Lu=f has local C^{k+2,alpha} regularity
        for C^{k,alpha} elliptic coefficients and forcing. The same holds up to
        a C^{k+2,alpha} boundary portion where the solution is continuous and
        its Dirichlet values are C^{k+2,alpha}.
      hypotheses: Integer k >= 0; 0 < alpha < 1; strict ellipticity; the stated
        coefficient, forcing, boundary and data regularity. Applied on
        relatively compact smooth coordinate patches to the already classical
        torsion solution, with smooth coefficients, forcing -1, zero boundary
        data and reaction c=0.
      reading_limits: Consulted the online book transcription of both theorem
        statements and the local-boundary conclusion. OCR is imperfect; no full
        proof review or manifold existence theorem is claimed. The chart
        application below is local.
---

## Statement

On the component containing the Euclidean end, with the smooth exterior data and Laplacian convention of the weighted exterior definition, assume $h-\delta\in C^{3,\alpha}_{-1}$ and $-1<\beta<0$. There is a positive continuous function $B$, smooth on either side of one large coordinate sphere $S_R=\{r=R\}$ up to each side's boundary, with $B=r^\beta$ outside that sphere, $B\asymp1$ on the compact core and $-\Delta_h B\ge c\rho^{\beta-2}$ away from the sphere, for some $c>0$. Here $\rho$ is any positive smooth function equal to $r$ far out. With $\nu$ the $h$-unit normal from the core into the end, define $J_\nu w=(\partial_\nu w)_{\mathrm{ext}}-(\partial_\nu w)_{\mathrm{int}}$, using the same normal on both sides. Across the sphere $J_\nu B<0$.

The precise maximum comparison is as follows. Suppose $v$ is continuous on this component including its original boundary, is $C^2$ off $S_R$ with one-sided $C^1$ regularity at $S_R$, and satisfies $\Delta_hv\ge0$ off $S_R$, $J_\nu v\ge0$, $v\le0$ on the original boundary and $\limsup_{r\to\infty}v\le0$. The last condition means that for every $a>0$, $v\le a$ outside some compact set. Then $v\le0$ everywhere. On a compact truncation $M_T$ with $T>R$, the same comparison holds with $v\le0$ on its entire boundary, including $\{r=T\}$, and no condition at infinity.

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] Weighted coefficients, the smooth Riemannian exterior, compact core, Laplacian sign and end derivative conventions are fixed. [[def-exterior-weighted-elliptic-data]] [[def-stationary-asymptotic-decay-data]]

[F2] Compact smooth cores with a boundary admit a zero-boundary torsion solution of class $C^{4,\alpha}$. [[lem-author-86990d62062f-compact-domain-poisson]]

[F3] Higher classical elliptic regularity, including regularity at a smooth boundary portion with smooth Dirichlet values, is the imported Euclidean input specified below (Gilbarg–Trudinger, Theorems 6.17 and 6.19).

## External input

The cited regularity theorems apply to an already classical solution, with the coefficient, forcing and boundary regularity recorded in the source contract. Only their regularity conclusions are imported. Smoothness of the manifold torsion solution is deduced in step 3.1 by applying them in charts; no manifold existence theorem is imported.

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] Weighted coefficients, the smooth Riemannian exterior, compact core, Laplacian sign and end derivative conventions are fixed. [[def-exterior-weighted-elliptic-data]] [[def-stationary-asymptotic-decay-data]]

[F2] Compact smooth cores with a boundary admit a zero-boundary torsion solution of class $C^{4,\alpha}$. [[lem-author-86990d62062f-compact-domain-poisson]]

[F3] Higher classical elliptic regularity, including regularity at a smooth boundary portion with smooth Dirichlet values, is the imported Euclidean input specified below (Gilbarg–Trudinger, Theorems 6.17 and 6.19).

**Proof technique:** direct.

1.1 Write $\Delta_h=h^{ij}\partial_i\partial_j+b^i\partial_i$. The stated decay gives $h^{ij}=\delta^{ij}+O(r^{-1})$ and $b^i=O(r^{-2})$. Direct radial differentiation gives $\Delta_hr^\beta=\beta(\beta+1)r^{\beta-2}+O(r^{\beta-3})$. Since $\beta(\beta+1)<0$, choose a large $R$ so $-\Delta_hr^\beta\ge c_0r^{\beta-2}$ on $r\ge R$. [F1]

2.1 Let $M_R$ be the end component truncated at $r=R$. It is compact with smooth boundary. It is connected: any excursion of a path into $r>R$ can be retracted radially onto $S_R$, which is connected. In particular it meets its boundary $S_R$, so the compact Poisson supplier applies. Solve $-\Delta_ht=1$, $t=0$ on its entire boundary, including any original boundary, obtaining $t\in C^{4,\alpha}(M_R)$. If $t$ had a negative minimum, it would be interior, where its vanishing gradient and nonnegative Hessian imply $\Delta_ht\ge0$, contradicting $\Delta_ht=-1$. Thus $t\ge0$. [F1, F2, step 1.1]

3.1 In each relatively compact interior or boundary chart the equation for $t$ is a strictly elliptic scalar equation with smooth coefficients and forcing $-1$. Positivity of the smooth metric gives uniform ellipticity on the smaller compact patch. The solution is already classical by step 2.1. Theorem 6.17 applies in interior charts. At a boundary chart, Theorem 6.19's local-boundary-portion conclusion applies to the smooth physical boundary with zero data; no regularity of values on artificial chart edges is required. For each integer $k\ge0$ these inputs give $C^{k+2,\alpha}$ regularity on smaller patches. A finite chart cover proves $t\in C^\infty(M_R)$ up to its entire boundary, including $S_R$. This is a local application of the imported theorems, not a reduction of the compact core to one Euclidean domain. [F1, F3, step 2.1]

4.1 Set $B=R^\beta+\epsilon t$ on $M_R$ and $B=r^\beta$ outside. Both traces on the seam are $R^\beta$. There $\nu=\nabla_hr/|\nabla_hr|_h$, so $\nu(r)=|\nabla_hr|_h>0$ and the exterior derivative $\beta R^{\beta-1}\nu(r)$ is strictly negative. [[math:def-riemannian-gradient-of-a-smooth-function]] Compactness of $S_R$ bounds it uniformly away from zero and bounds $\partial_\nu t$. Choose $\epsilon>0$ small enough that $J_\nu B=\beta R^{\beta-1}\nu(r)-\epsilon\partial_\nu t<0$ on the whole sphere. Inside, $-\Delta_hB=\epsilon$; outside use step 1.1. The positive smooth $\rho$ has finite maximum and positive minimum on compact sets and equals $r$ far out, so decreasing $c>0$ if necessary gives $-\Delta_hB\ge c\rho^{\beta-2}$ on both pieces. The barrier is positive; on the core it lies between $R^\beta$ and $R^\beta+\epsilon\max t$, proving $B\asymp1$ there. Its asserted piecewise smoothness follows from step 3.1 and smoothness of $r^\beta$ on the end. [F1, step 1.1, step 2.1, step 3.1]

5.1 First consider a function $w$ with the stated continuity and one-sided regularity, with $\Delta_hw>0$ on each piece, $J_\nu w>0$, negative original boundary values and $\limsup_{r\to\infty}w\le0$. If $w(p)>0$ anywhere, choose $0<a<w(p)$. Outside a compact set $w\le a$, so $w$ attains a positive global maximum on a compact truncation, away from both its outer boundary and its original boundary. At an interior maximum off the seam, the gradient vanishes and the Hessian is negative semidefinite, giving $\Delta_hw\le0$, a contradiction. At a seam maximum, the interior derivative in direction $\nu$ is nonnegative and the exterior derivative in the same direction is nonpositive. Hence $J_\nu w\le0$, again a contradiction. Thus $w\le0$. On compact $M_T$ the same argument uses compactness and negative entire boundary values directly. [F1, step 4.1]

6.1 For $v$ satisfying the weak comparison hypotheses set $w=v-\eta B$ for any $\eta>0$. Then $\Delta_hw=\Delta_hv-\eta\Delta_hB>0$ off the seam, $J_\nu w=J_\nu v-\eta J_\nu B>0$, and $w<0$ on every boundary where $v\le0$. Since $B=r^\beta\to0$, the condition $\limsup_{r\to\infty}v\le0$ also gives $\limsup_{r\to\infty}w\le0$. Step 5.1 yields $v\le\eta B$; let $\eta\downarrow0$ at each point to obtain $v\le0$. For compact truncations the same perturbation has negative values on the entire boundary, so the compact version of step 5.1 applies. This proves the comparison and completes the Statement. [F1, step 4.1, step 5.1] ∎

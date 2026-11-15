---
id: lem-author-d20d145f998f-spin-from-reciprocal-invariant
title: The reciprocal-potential invariant determines the end spin bound
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - math:lem-derivative-algebra-and-chain-rules
  - math:thm-real-power-continuity-and-derivatives
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
  math:thm-real-power-continuity-and-derivatives: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $M>0$ and $S=(S^1,S^2,S^3)$ be constants and $J=|S|$, using the Euclidean norm. Let $(X,g)$ be a smooth Lorentzian four-manifold of signature $(-,+,+,+)$. Supply an open subset $E\subset X$ and a smooth coordinate chart $(t,x^1,x^2,x^3)$ on $E$ with coordinate range $I\times\{x\in\mathbb R^3:|x|>R\}$, where $I$ is a nonempty open interval and $R>0$. Set $r=|x|=(\sum_{i=1}^3(x^i)^2)^{1/2}$. Write $g^{ab}$ for the components of the inverse metric (equivalently the unique inverse matrix of the nondegenerate matrix $(g_{ab})$), use $a,b=0,1,2,3$ with $x^0=t$, and use $i,j=1,2,3$ for spatial indices. Assume $\partial_tg_{ab}=0$ and $g^{ij}=\delta^{ij}+O(r^{-1})$. Suppose smooth real functions $y,z$ satisfy $\partial_ty=\partial_tz=0$, $y=r/(2M)+O(1)$ and $z=(S\cdot x)/(2M^2r)+O_1(r^{-1})$. In this chart, $h=O(r^{-k})$ means $|h(t,x)|\le Cr^{-k}$ for sufficiently large $r$, uniformly in $t$ and direction; tensor-component estimates are componentwise. For the remainder $h=z-(S\cdot x)/(2M^2r)$, $O_1(r^{-1})$ means both $|h|\le Cr^{-1}$ and $|\partial_i h|\le Cr^{-2}$ for every spatial index $i$, with the same uniformity. Define $B=z^2+4M^2(y^2+z^2)g^{ab}\partial_a z\partial_b z$. Then $B=J^2/(4M^4)+O(r^{-1})$. For the conditional conclusion, suppose $g,y,z$ are defined smoothly on a connected open domain $D\subset X$ containing $E$, and supply a nonempty open subset $V\subset D$. If this same scalar $B$ is constant on $D$ and $0\le B<1/4$ on $V$, then $J<M^2$. The constancy and the bound on $V$ are explicit inputs, not consequences of the asymptotic expansion.

## Statement references

[[physics:def-gr-smooth-lorentzian-objects]]

[[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

## Facts & Assumptions

[F1] A smooth Lorentzian metric of signature $(-,+,+,+)$ is symmetric and nondegenerate, has smooth chart components and admits a timelike vector at every point. A smooth timelike field on an open set is a time orientation there. The inverse-metric interface applies to a time-oriented restriction and defines $\flat_p(v)=g_p(v,\cdot)$, $\sharp_p=\flat_p^{-1}$ and $g_p^{-1}(\alpha,\beta)=g_p(\sharp_p\alpha,\sharp_p\beta)$, with matrix components $g^{ab}$. Step 1.1 constructs suitable local restrictions and shows that these definitions agree independently of their time orientations. The particular chart, stationarity, decay bounds and sets $D,V$ are explicit data in the Statement. [[physics:def-gr-smooth-lorentzian-objects]] [[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

[F2] Sum, product, quotient and chain rules apply to differentiable real functions, with a nonzero denominator for the quotient rule and the composition defined near the point for the chain rule. Apply these rules to each spatial coordinate with the other coordinates fixed. On positive arguments, $(u^{1/2})'=1/(2u^{1/2})$; here $r^2>R^2>0$. [[math:lem-derivative-algebra-and-chain-rules]] [[math:thm-real-power-continuity-and-derivatives]]

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the stated asymptotic formula and conditional spin bound.

1.1 Fix any point $p$ of the domain where the inverse metric is used. By [F1] there is a timelike vector $v\in T_pX$. In a chart about $p$, extend its four components as constants to obtain a smooth field $N=\sum_{a=0}^3v^a\partial_a$. The function $q\mapsto g_q(N_q,N_q)$ is continuous and negative at $p$, so it is negative on an open neighborhood $W$ of $p$. Thus $(W,g|_W,N)$ meets the inverse-metric interface's time-orientation hypothesis. Its maps $\flat_q$, $\sharp_q$ and $g_q^{-1}$ are determined solely by $g_q$, not by $N$ or $W$, so definitions obtained this way agree on every overlap. Their chart components are the unique inverse of $(g_{ab})$, and bilinearity gives $g^{-1}(dz,dz)=\sum_{a,b=0}^3g^{ab}\partial_a z\partial_b z$. This establishes the contraction wherever needed without assuming a global time orientation or choosing neighborhoods simultaneously. [given, F1, algebra]

1.2 Put $n=x/r$, so $\sum_i n_i^2=1$, with Euclidean lowering $S_i=S^i$ and $n_i=n^i$. By [F2], $\partial_i r=x^i/r=n_i$ and $\partial_i((S\cdot x)/r)=(S_i-n_i(S\cdot n))/r$. Differentiating the expansion for $z$ is therefore justified by the stated derivative bound on its remainder and gives $\partial_i z=(S_i-n_i(S\cdot n))/(2M^2r)+O(r^{-2})$. Since $|S\cdot n|\le\sum_i|S^i|$, the leading coefficients are uniformly bounded. Expanding the finite sum of squares, using $\sum_i(S_i-n_i(S\cdot n))^2=J^2-(S\cdot n)^2$, gives $\sum_i(\partial_i z)^2=(J^2-(S\cdot n)^2)/(4M^4r^2)+O(r^{-3})$. [given, F2, algebra]

2.1 Each $\partial_i z$ is $O(r^{-1})$, so $\sum_{i,j}(g^{ij}-\delta^{ij})\partial_i z\partial_j z=O(r^{-3})$ by the componentwise metric bound and the finite number of terms. Since $\partial_tz=0$, every temporal or mixed term in the contraction vanishes. Thus $g^{ab}\partial_a z\partial_b z=(J^2-(S\cdot n)^2)/(4M^4r^2)+O(r^{-3})$. [given, F1, step 1.1, step 1.2, algebra]

3.1 The other expansions give $4M^2(y^2+z^2)=r^2+O(r)$ and $z^2=(S\cdot n)^2/(4M^4)+O(r^{-1})$: expand $y=r/(2M)+O(1)$ and the bounded leading term of $z$. Multiplying the contraction from step 2.1 by $r^2+O(r)$ gives $(J^2-(S\cdot n)^2)/(4M^4)+O(r^{-1})$. Adding $z^2$ cancels the angular term, yielding $B=J^2/(4M^4)+O(r^{-1})$. [given, F1, step 1.2, step 2.1, algebra]

4.1 If $B$ is a single constant on $D$, its value equals the limit along the end, hence $B=J^2/(4M^4)$. Since $V$ is nonempty, the assumed bound there then gives $J^2/(4M^4)<1/4$. Multiplication by $4M^4>0$ and $J\ge0$ imply $J<M^2$. No global metric isometry or independent angular-momentum conservation law was used. [given, step 3.1, algebra] ∎

## Remarks

The original horizon-neighborhood application is included by taking $V$ to be its nonempty open portion in $D$. The calculation requires exactly the chart and differentiated estimates stated above; the conditional implication uses only the constancy on $D$ and the bound on $V$. No causal property of a horizon is an additional premise of this calculation.

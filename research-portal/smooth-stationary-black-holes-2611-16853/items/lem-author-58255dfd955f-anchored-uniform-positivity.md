---
id: lem-author-58255dfd955f-anchored-uniform-positivity
title: Positive anchor values and the limits of uniform Harnack propagation
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-58255dfd955f-compact-harnack-chain
  - def-exterior-weighted-elliptic-data
  - math:lem-derivative-algebra-and-chain-rules
dependency_roles:
  lem-author-58255dfd955f-compact-harnack-chain: mathematical-premise
  def-exterior-weighted-elliptic-data: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

Let a family of positive Schrödinger solutions have a common finite chain cover joining a compact interior set $K$ to an anchor point $x_*$, with common comparison constant $H$. If $u(x_*)\ge a>0$ uniformly, then $\inf_Ku\ge a/H$. A common limit $u\to c>0$ on the end supplies such an anchor if the end threshold giving, for example, $u\ge c/2$ is uniform in the family, with the comparison controls extending to the chosen anchor. A uniform end threshold is sufficient, but is not necessary for a uniform anchor. Individual end limits alone guarantee neither a fixed point with a positive uniform anchor value, nor a uniform end threshold, nor a uniform compact lower bound, even on a fixed Euclidean three-dimensional exterior with smooth nonnegative potentials uniformly bounded everywhere.

## Facts & Assumptions

[F1] The finite-chain comparison is the conditional part of [[lem-author-58255dfd955f-compact-harnack-chain]]: common local pairwise comparisons on the half-balls of a common finite connected chain cover give a common comparison constant on the covered set. For a connected compact $K$ and an anchor outside $K$, include a fixed path from $K$ to $x_*$ and cover its compact image together with $K$; a connected smooth manifold is path connected because chart balls are path connected and its path components are open. More generally, the assumed common connected chain cover must contain all of $K$ and $x_*$. The coefficient and cover controls, when used to obtain the local comparisons, must hold on this enlarged compact region. Below, the examples' local comparisons are proved directly; the supplier's ZFC analytic consequence is not invoked.

[F2] The exterior and Laplacian conventions are [[def-exterior-weighted-elliptic-data]]. For the examples take $\Sigma=\mathbb R^3$ with its Euclidean metric and empty compact boundary; outside the closed unit ball this is the prescribed exterior chart. Here $\Delta u=\sum_{i=1}^3\partial_i^2u$. For a smooth positive $u$, define $V=\Delta u/u$, so $(\Delta-V)u=0$ pointwise. No boundary condition is assumed in this lemma.

[F3] Coordinatewise sum, product, quotient and chain differentiation use [[math:lem-derivative-algebra-and-chain-rules]]. All functions differentiated below have strictly positive square-root arguments and denominators. Their potentials, signs, bounds and local comparisons are computed locally rather than imported from an external result.

## Proof

**Given:** The hypotheses in the Statement and [F1]–[F3].

**Goal:** Prove the anchor estimate and both distinctions concerning end normalization.

**Proof technique:** direct.

1.1 By [F1], $u(x_*)\le H u(x)$ for every $x\in K$. Insert $u(x_*)\ge a$ and take the infimum to obtain $\inf_Ku\ge a/H$. A common end threshold permits a single fixed $x_*$ beyond it, with $a=c/2$, provided the same comparison controls hold to this point. This proves the anchor estimate and the sufficiency assertion. [F1, given, algebra]

1.2 For $0<b<1$, $\lambda>0$ and $z\in\mathbb R^3$, put $Q(x)=1+\lambda^2|x-z|^2$ and $f(x)=1-bQ(x)^{-1/2}$. This is smooth and $f\ge1-b>0$. For $t>0$, rationalizing gives $(\sqrt{t+h}-\sqrt t)/h=1/(\sqrt{t+h}+\sqrt t)$ for nonzero sufficiently small $h$; the quotient rule then gives $(t^{-1/2})'=-1/(2t^{3/2})$. Repeated differentiation on $t>0$ gives smoothness. Applying [F3] coordinatewise yields $\partial_i f=b\lambda^2(x_i-z_i)Q^{-3/2}$ and $\partial_i^2 f=b\lambda^2Q^{-3/2}-3b\lambda^4(x_i-z_i)^2Q^{-5/2}$. Summing in [F2] yields $\Delta f=3b\lambda^2Q^{-5/2}$, hence $0\le V_f:=\Delta f/f\le3b\lambda^2/(1-b)$. For fixed parameters, $f\to1$ uniformly as $|x|\to\infty$, since $|x-z|\ge|x|-|z|$. [F2, F3, algebra]

2.1 To show that a uniform threshold is not necessary, let $e_1=(1,0,0)$ and, for integers $n\ge1$, set $w_n(x)=1-\frac34(1+|x-2ne_1|^2)^{-1/2}$. Step 1.2 gives positive smooth Schrödinger solutions with $0\le V_{w_n}\le9$, and each has end limit $1$. At the fixed anchor $0$, $w_n(0)\ge1-3/(4\sqrt5)>1/2$. Nevertheless $w_n(2ne_1)=1/4$, so no radius works for the inequality $w_n\ge1/2$ for every $n$ beyond that radius. The bounds $1/4\le w_n\le1$ give $w_n(x)\le4w_n(y)$ for all $x,y$, directly supplying common local comparisons on every fixed chain cover in [F1]. The Euclidean metric and the displayed potential bounds also give uniform coefficient controls there. Thus a common anchor can exist without the indicated uniform end threshold. [step 1.2, F1, algebra]

3.1 For $0<\varepsilon\le1/2$ set $u_\varepsilon(x)=1-(1-\varepsilon)(1+\varepsilon^2|x|^2)^{-1/2}$. Step 1.2 gives $u_\varepsilon\ge\varepsilon>0$, $u_\varepsilon\to1$ at infinity for each $\varepsilon$, and $0\le V_\varepsilon\le3\varepsilon(1-\varepsilon)\le3/4$ everywhere. The Euclidean metric and these potential bounds give uniform coefficient controls on every fixed finite compact chain cover. To check the local comparisons directly, write $s=(1+\varepsilon^2|x|^2)^{1/2}\ge1$. Then $u_\varepsilon(x)=\varepsilon+(1-\varepsilon)\varepsilon^2|x|^2/[s(s+1)]$. On $|x|\le R$ this implies $\varepsilon\le u_\varepsilon(x)\le\varepsilon(1+R^2/4)$, using $s(s+1)\ge2$ and $\varepsilon\le1/2$. Thus for all $x,y$ in this ball, $u_\varepsilon(x)\le(1+R^2/4)u_\varepsilon(y)$, uniformly in $\varepsilon$, and every fixed finite chart cover with compact closures fits into such a ball. For the closed unit ball $K$, $\inf_Ku_\varepsilon=u_\varepsilon(0)=\varepsilon\to0$. Moreover the same bound gives $u_\varepsilon(x)\to0$ at every fixed $x$, so there is no fixed point with a positive uniform anchor value. For any proposed common end radius $R_0$, fix $x$ with $|x|>R_0$; then $u_\varepsilon(x)<1/2$ for sufficiently small $\varepsilon$. Hence the individual common end limits supply neither a uniform threshold nor a uniform compact lower bound, despite the common local comparison controls in [F1]. [step 1.2, F1, algebra] ∎

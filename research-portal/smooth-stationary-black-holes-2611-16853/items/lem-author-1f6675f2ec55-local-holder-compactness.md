---
id: lem-author-1f6675f2ec55-local-holder-compactness
title: Local compactness of full weighted Hölder inputs
kind: lemma
status: published
origin: pipeline
domain: mathematics
proof_strategy: direct
deps:
  - math:def-axiom-of-choice
  - def-weighted-holder-spaces
  - def-exterior-weighted-elliptic-data
  - math:thm-arzela-ascoli-for-real-ck
  - math:thm-mean-value-inequality
  - math:thm-uniform-derivative-limit-on-a-closed-interval
  - math:thm-metric-compactness-equivalences
dependency_roles:
  math:def-axiom-of-choice: mathematical-premise
  def-weighted-holder-spaces: mathematical-premise
  def-exterior-weighted-elliptic-data: mathematical-premise
  math:thm-arzela-ascoli-for-real-ck: mathematical-premise
  math:thm-mean-value-inequality: mathematical-premise
  math:thm-uniform-derivative-limit-on-a-closed-interval: mathematical-premise
  math:thm-metric-compactness-equivalences: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
dependency_level: 2
---

## Statement

Assume the Axiom of Choice. In the exterior chart and boundary-chart setting of the weighted Hölder definition, a sequence bounded in $C^{4,\alpha}_\beta$, for $0<\alpha<1$ and any real $\beta$, has a subsequence converging in $C^{2,\alpha}$ on every fixed compact truncation, including its original boundary. No zero-boundary condition is required. Here a compact truncation consists of the fixed compact core and the part of the end with $r\le R$, for fixed sufficiently large $R$.

## Statement references

[[math:def-axiom-of-choice]]

[[def-weighted-holder-spaces]]

[[def-exterior-weighted-elliptic-data]]

[[math:thm-arzela-ascoli-for-real-ck]]

## Facts & Assumptions

**Given:** The hypotheses of the Statement.

**Goal:** Establish its stated analytic ingredients and qualifications.

[F1] The Axiom of Choice includes countable and dependent choice for diagonal subsequences and compactness. [[math:def-axiom-of-choice]]

[F2] The weighted norm bounds the coordinate derivatives through order four on every fixed compact truncation, including boundary half-charts. [[def-weighted-holder-spaces]] [[def-exterior-weighted-elliptic-data]]

[F3] Equicontinuous pointwise bounded families on a compact metric space have compact closure in the supremum norm. [[math:thm-arzela-ascoli-for-real-ck]]

[F4] If a real-valued function on a closed interval is continuous there, differentiable on its interior, and has derivative bounded in absolute value by $M\ge0$, its endpoint difference is at most $M$ times the interval length. This is the scalar case of the mean value inequality. [[math:thm-mean-value-inequality]]

[F5] For continuously differentiable real functions on a nondegenerate closed interval, convergence at one point and uniform convergence of their derivatives imply uniform convergence to a differentiable function whose derivative is that uniform derivative limit. [[math:thm-uniform-derivative-limit-on-a-closed-interval]]

[F6] Under countable and dependent choice, compact metric spaces are sequentially compact. [[math:thm-metric-compactness-equivalences]]

## Proof

1.1 Work on a fixed compact truncation, allowing a slightly larger truncation when choosing chart neighbourhoods. Cover it by finitely many smaller closed rectangular coordinate boxes, or rectangular half-boxes at the original boundary, whose relative interiors cover the truncation and whose closures stay in the chart domains. Work within the fixed norm charts, covering each of their compact subsets by such pieces. By [F2], coordinate derivatives through order four have uniform bounds on these pieces. If $v$ is one such derivative of order at most three and $M$ bounds each $|\partial_i v|$, join $x$ to $y$ in a box by changing one coordinate at a time. On each coordinate segment in the interior, [F4] bounds the difference by $M$ times that coordinate displacement. Summing gives $|v(x)-v(y)|\le M\sum_{i=1}^3|x_i-y_i|\le\sqrt{3}M|x-y|$. For endpoints on a boundary face, approximate the coordinate segments from the interior and pass to the limit using the continuous boundary extensions in [F2]. Thus all these derivative families are uniformly bounded and equicontinuous on the closed pieces. [F2, F4, algebra]

2.1 By [F3], each derivative family through order three on each compact piece has compact closure in the supremum metric. By [F1] and [F6], every sequence in that closure has a uniformly convergent subsequence with a continuous limit. Successively extract for the finitely many pieces and multi-indices. Denote the resulting continuous limits by $v_I$ for $|I|\le3$, with $v_0=u$. [F1, F3, F6, step 1.1, choose]

3.1 Fix a nondegenerate closed coordinate segment strictly inside the interior of one piece, a coordinate direction $e_i$, and a multi-index $I$ with $|I|\le2$. The restrictions $f_j(t)=\partial^I u_{n_j}(x+te_i)$ are continuously differentiable there. Step 2.1 gives their convergence at any fixed point and uniform convergence of $f_j'$ to the restriction of $v_{I+e_i}$. Apply [F5]; uniqueness of the uniform limit identifies the limit as the restriction of $v_I$, so $\partial_i v_I=v_{I+e_i}$ in the interior. Induction on derivative order identifies all the fields through order three as derivatives of $u$. Their continuous limits on each closed half-box provide exactly the continuous extensions required for regularity up to the boundary; no two-sided derivative at the boundary is being assumed. The limits of the scalar functions agree on chart overlaps because they are pointwise limits of the same global subsequence, so they define a single local $C^3$ function $u$ on the truncation. [F2, F5, step 2.1]

4.1 On a smaller box put $z=u_{n_j}-u$, $a=\max_{|I|=2}\|\partial^I z\|_\infty$, and $b=\max_{|I|=3}\|\partial^I z\|_\infty$. Step 2.1 gives $a\to0$ and a uniform bound on $b$. Apply the coordinate-segment estimate of step 1.1, now to each $\partial^I z$ with $|I|=2$. For pairs with $|x-y|\le d$, the Hölder quotient is at most $\sqrt{3}b d^{1-\alpha}$; for pairs with $|x-y|>d$, it is at most $2a d^{-\alpha}$. First choose $d>0$ small using the uniform bound on $b$ and $1-\alpha>0$, then let $j$ increase using $a\to0$. Thus every second-derivative Hölder seminorm of $z$ tends to zero, as do all derivative suprema through order two. This proves convergence in $C^{2,\alpha}$ on each piece, including its boundary face. [F2, F4, step 1.1, step 2.1, step 3.1, algebra]

5.1 In each fixed norm chart, the relative interiors of the finitely many boxes cover its compact subset. There is a positive distance threshold such that any sufficiently close pair in that subset lies in a common box: otherwise a sequence of pairs at distances tending to zero with no common box would, by compactness and [F6], have a subsequence tending to the same point, contradicting the relative-interior cover. Step 4.1 controls those close pairs; for pairs farther apart, the second-derivative supremum tending to zero controls the Hölder quotient. Hence the finite sum defining the compact $C^{2,\alpha}$ norm tends to zero. Repeat on a nested integer-radius exhaustion. By [F1], successively take subsequences and then the diagonal subsequence. Its limits on overlapping truncations agree by uniqueness of the uniform limit, and restriction from a larger integer-radius truncation gives convergence on every fixed truncation. No boundary value has been imposed at any step. [F1, F2, F6, step 3.1, step 4.1, choose, algebra] ∎

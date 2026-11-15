---
id: lem-author-fd2999663761-compact-weighted-maximum
title: Compact weighted maximum and the actual boundary term
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-author-fd2999663761-temporal-angle-data
  - math:thm-compactness-under-continuous-maps
  - math:def-real-power
  - math:lem-real-power-preserves-measurability
  - math:thm-real-power-continuity-and-derivatives
  - math:thm-real-power-laws
  - math:thm-real-power-agrees-with-rational-exponent
  - math:def-subspace-topology-top
  - math:lem-continuity-is-local-and-pastes
  - math:lem-algebra-of-continuous-real-maps-on-a-space
dependency_roles:
  def-author-fd2999663761-temporal-angle-data: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:def-real-power: mathematical-premise
  math:lem-real-power-preserves-measurability: mathematical-premise
  math:thm-real-power-continuity-and-derivatives: mathematical-premise
  math:thm-real-power-laws: mathematical-premise
  math:thm-real-power-agrees-with-rational-exponent: mathematical-premise
  math:def-subspace-topology-top: mathematical-premise
  math:lem-continuity-is-local-and-pastes: mathematical-premise
  math:lem-algebra-of-continuous-real-maps-on-a-space: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

For a compact positive-height portion $P$ of the temporal angle data, let $\mu>0$. Use the real-power convention $0^\mu=0$. A local maximum of $w$ at $p\in S=\Sigma\cap\{\tau>0\}$ means that there is an open neighborhood $U\subseteq S$ of $p$ in $\Sigma$ with $w(q)\le w(p)$ for every $q\in U$. Suppose $w=\tau^\mu v$ has no local maximum at any interior point of $\Sigma$ with $\tau>0$ and $v>2$. Then $\sup_{\Sigma\cap\{\tau>0\}}\tau^\mu v\le\max\{2T^\mu,B\}$. The supremum on the left is defined to be zero if $\Sigma\cap\{\tau>0\}=\varnothing$. No regularity of the zero level $\{\tau=0\}\cap\Sigma$ is required.

## Statement references

[[def-author-fd2999663761-temporal-angle-data]]

[[math:def-real-power]]

## Facts & Assumptions

[F1] The entire portion $P=\Sigma\cap\{\tau\ge0\}$ is compact, $v$ is continuous and bounded on it, $0\le\tau\le T$, and $B$ uses only $\partial\Sigma\cap\{\tau>0\}$. [[def-author-fd2999663761-temporal-angle-data]]

[F2] A continuous real-valued function on a nonempty compact space attains a maximum and a minimum (Statement, assertion 2). [[math:thm-compactness-under-continuous-maps]]

[F3] For $r>0$, $0^r=0$ and $t\mapsto t^r$ is strictly increasing on $[0,\infty)$; in particular $t^r>0$ when $t>0$. Use the real-power definition and the monotonicity assertion of the measurability lemma; no measurable-space hypothesis is needed for that assertion. [[math:def-real-power]] [[math:lem-real-power-preserves-measurability]]

[F4] For every real $r$, $t\mapsto t^r$ is continuous for $t>0$. For $a>0$ and real $r,s$, $(a^r)^s=a^{rs}$, and $a^1=a$ by agreement with rational powers. [[math:thm-real-power-continuity-and-derivatives]] [[math:thm-real-power-laws]] [[math:thm-real-power-agrees-with-rational-exponent]]

[F5] Restrictions of continuous maps to subspaces are continuous, and a continuous map whose range lies in a subspace is continuous into that subspace, with its subspace topology. Composites of continuous maps between arbitrary topological spaces are continuous (Statement, assertion 1). Products of continuous real-valued maps on any topological space are continuous. [[math:def-subspace-topology-top]] [[math:lem-continuity-is-local-and-pastes]] [[math:lem-algebra-of-continuous-real-maps-on-a-space]]

## Proof

**Given:** [F1] and the no-interior-maximum hypothesis, with $\mu>0$. **Goal:** Bound the weighted supremum.

1.1 For the fixed $\mu>0$, the power function is continuous at every positive argument by [F4]. To check continuity at zero, let $\varepsilon>0$ and put $\delta=\varepsilon^{1/\mu}>0$ by [F3] with exponent $1/\mu>0$. The iterated-power law and normalization in [F4] give $\delta^\mu=\varepsilon$. If $0\le t<\delta$, [F3] gives $0\le t^\mu<\delta^\mu=\varepsilon$. Since $0^\mu=0$, this proves continuity at zero relative to $[0,\infty)$. The same monotonicity gives $0\le\tau^\mu\le T^\mu$ on $P$. [F1, F3, F4, given, algebra]

2.1 Put $S=\Sigma\cap\{\tau>0\}$. If $S$ is empty, its stipulated supremum is zero and the right-hand side is nonnegative by $T\ge0$ and [F3], so the estimate holds, even when $P$ consists only of zero-height points. Otherwise $P$ is nonempty. Applying [F2] to the continuous $v$ on compact $P$ gives finite extrema; taking $M$ to be the larger of their absolute values and $1$ yields $|v|\le M$ on $P$. Extend $w$ by zero at zero height. By the restriction and subspace assertions of [F5], the continuous $\tau$ restricts to a continuous map $\tau|_P:P\to[0,\infty)$, since its values are nonnegative by [F1]. Composing this map with the continuous power map $t\mapsto t^\mu$ from step 1.1 gives continuity of $\tau^\mu:P\to\mathbb R$ by [F5]. The product assertion of [F5], applied on the topological space $P$ to $\tau^\mu$ and $v$, makes the extended $w$ continuous on all of $P$. At a zero-height point, $|w|\le M\tau^\mu$ tends to zero by step 1.1 and continuity of $\tau$, proving continuity there too. [F1, F2, F3, F5, step 1.1, given]

3.1 In the remaining case $P$ is nonempty and compact, and the extended $w:P\to\mathbb{R}$ is continuous. Applying [F2] with domain $P$ gives a point at which $w$ attains its maximum on $P$. [F1, F2, step 2.1]

4.1 At a maximum point with $\tau=0$ the value is zero. At a positive-height point on $\partial\Sigma$ it is at most $B$. If the maximum point $p$ is interior to $\Sigma$ and has positive height, then $U=S\cap(\Sigma\setminus\partial\Sigma)$ is an open neighborhood of $p$ in $\Sigma$ by continuity of $\tau$. Since $U\subseteq P$, the maximum on $P$ gives $w(q)\le w(p)$ for every $q\in U$, exactly the local-maximum condition in the Statement. The hypothesis therefore gives $v(p)\le2$, so $w(p)\le2\tau(p)^\mu\le2T^\mu$ by step 1.1. These exhaustive cases bound the maximum on $P$ by $\max\{2T^\mu,B\}$ and hence bound the supremum on $S\subseteq P$, with no regularity required of the zero level. [F1, F3, step 1.1, step 3.1, given] ∎

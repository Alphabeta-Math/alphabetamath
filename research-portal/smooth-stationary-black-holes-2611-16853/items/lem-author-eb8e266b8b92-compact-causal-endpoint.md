---
id: lem-author-eb8e266b8b92-compact-causal-endpoint
title: An interior compact causal trajectory has a finite-time endpoint
kind: lemma
status: published
origin: pipeline
domain: mathematics
proof_strategy: direct
deps:
  - math:thm-choice-implies-dependent-implies-countable-choice
  - math:thm-extreme-value-metric
  - math:def-axiom-of-choice
  - lem-author-eb8e266b8b92-adm-time-speed
  - math:thm-the-riemannian-distance-topology-is-the-manifold-topology
  - math:thm-metric-compactness-equivalences
  - math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric
  - math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions
dependency_roles:
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
  math:thm-extreme-value-metric: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  lem-author-eb8e266b8b92-adm-time-speed: mathematical-premise
  math:thm-the-riemannian-distance-topology-is-the-manifold-topology: mathematical-premise
  math:thm-metric-compactness-equivalences: mathematical-premise
  math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric: mathematical-premise
  math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
dependency_level: 3
---

## Statement

Assume the Axiom of Choice and the stationary ADM causal conventions of the section-time speed lemma. If a causal curve $(v,x(v))$, $v\in[v_0,v_*)$, with $v_*<\infty$, has spatial image in a compact interior subset $K\subset S$, then it converges to a point $(v_*,p)\in E$. The corresponding conclusion holds at a finite lower endpoint. Consequently neither end of a causal curve that is inextendible in $E$ can have finite section time while its spatial projection stays in an interior compact set.

## Statement references

[[math:def-axiom-of-choice]]

[[lem-author-eb8e266b8b92-adm-time-speed]]

[[math:thm-the-riemannian-distance-topology-is-the-manifold-topology]]

[[math:thm-metric-compactness-equivalences]]

[[math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric]]

[[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions]]

## Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice supplies inherited countable and dependent choice assumptions. [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]]

[F2] A causal curve in section time is locally Lipschitz and has $|x\prime|_h\le N+|X|_h$; inextendibility is absence of an endpoint. [[lem-author-eb8e266b8b92-adm-time-speed]]

[F3] The Riemannian distance gives the manifold topology, and a compact metric space is sequentially compact under the inherited choice assumptions. [[math:thm-the-riemannian-distance-topology-is-the-manifold-topology]] [[math:thm-metric-compactness-equivalences]]

[F4] A positive-definite smooth metric uniformly bounds the Euclidean norm on a compact coordinate ball. [[math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric]]

[F5] For absolutely continuous coordinate functions the integral of the derivative gives their endpoint difference. [[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions]]

[F6] A continuous real-valued function on a nonempty compact metric space is bounded. [[math:thm-extreme-value-metric]]

## Proof

1.1 The smooth ADM data make $N+|X|_h$ continuous on $K$. Since $x(v_0)\in K$, this compact set is nonempty. The extreme-value theorem therefore bounds $N+|X|_h$ on $K$, say by $B$. Choose times $v_j\uparrow v_*$; compactness gives a subsequence for which $x(v_j)\to p\in K$. Take an interior coordinate ball centered at $p$, with coordinate radius $r>0$ and compact closure in its chart. Metric comparison on its closure gives $h(Y,Y)\ge c|Y|_{\mathrm e}^2$ for $c>0$. Thus while the curve remains in the ball, $|x\prime|_{\mathrm e}\le B/\sqrt c=:D$ almost everywhere. [F1, F2, F3, F4, F6, choose]

2.1 Choose a subsequence time $v_j$ so late that its coordinate distance from the center is less than $r/4$ and $D(v_*-v_j)<r/4$; for $D=0$ only the first condition is needed. Were there a subsequent exit from the coordinate ball, continuity would give a first exit, but integration of the coordinate speed up to that exit would give total displacement less than $r/4$, contradicting the required displacement of more than $3r/4$. Hence the whole remaining tail stays in that chart. Its coordinates are $D$-Lipschitz and are Cauchy as $v\uparrow v_*$. They converge to the coordinate of $p$, since the chosen subsequence does. Thus $(v,x(v))\to(v_*,p)\in E$. The argument with reversed parameter direction treats a finite lower endpoint. Such a limit contradicts precisely the endpoint definition of inextendibility. [F1, F2, F5, step 1.1, algebra] ∎

---
id: lem-author-9a15bef58785-affine-generator-zero-locus
title: Affine null-generator profiles vanish exactly on the bifurcation section
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - math:def-action-of-a-vector-field-on-smooth-functions
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  math:def-action-of-a-vector-field-on-smooth-functions: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Let $H$ be a smooth null hypersurface with nonzero smooth null generator $L$ normal to $H$. Let $s$ be a smooth function on $H$ with $L(s)=1$ and $s^{-1}(0)=S$. For a constant $c\ne0$, put $K=csL$ on $H$. Then $K$ is normal and tangent to $H$, vanishes precisely on $S$, and is nonzero on $H\setminus S$. At every such nonzero point, it spans the null generator line. This conditional statement asserts no existence of an ambient Killing extension.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-bifurcate-killing-horizon-data]]

[[math:def-action-of-a-vector-field-on-smooth-functions]]

## Facts & Assumptions

[F1] The smooth Lorentzian and null-horizon interfaces define the normal generator line and scalar multiples of its nonzero generator. [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]]

## Proof

**Given:**The hypotheses and data in the Statement.

**Goal:** Establish the stated conclusions with the indicated normalization and scope.

1.1 At every $p\in H$, the vector $K_p=cs(p)L_p$ belongs to the null normal line, hence is tangent and normal to $H$. Since $c\ne0$ and $L_p\ne0$, it is zero if and only if $s(p)=0$. The given zero set of $s$ is exactly $S$. [given, F1]

2.1 If $p\in H\setminus S$, the scalar $cs(p)$ is nonzero. A nonzero scalar multiple of the nonzero vector spanning a one-dimensional line spans the same line. This proves the full asserted zero locus and generator property. [F1, step 1.1] ∎

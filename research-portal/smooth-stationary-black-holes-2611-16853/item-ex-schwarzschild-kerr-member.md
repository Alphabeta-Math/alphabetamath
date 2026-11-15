---
title: Schwarzschild as the zero-spin member of Kerr
status: published
research_item: ex-schwarzschild-kerr-member
dependency_level: 6
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: §1.1, PDF pp. 1–2, sentence ending on p. 2
      statement: The member of the Kerr family with a = 0 is the Schwarzschild solution.
      hypotheses: The Kerr family and parameter conventions stated in the preceding
        display and text.
      reading_limits: The frozen article text was read for attribution. This reference
        is not used as proof of the specialization.
---

PDF p. 1: ` §1.1, sentence spanning pp.1–2 `; PDF p. 2: ` §1.1, sentence spanning pp.1–2 `

## Prerequisites

- [def-kerr-metric](item-def-kerr-metric)
- [lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor)


## Example

For $M>0$, the $a=0$ member of the Kerr exterior is the Schwarzschild exterior of mass parameter $M$. Its angular momentum is $J=0$ and its radial domain is $r>2M$. Here the Schwarzschild exterior is the tensor on $\mathbb R_t\times(2M,\infty)\times S^2$ with line element $-(1-2M/r)dt^2+(1-2M/r)^{-1}dr^2+r^2(d\theta^2+\sin^2\theta\,d\phi^2)$ away from the spherical coordinate poles.

## Example references

[def-kerr-metric](item-def-kerr-metric)

[lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor)

## Facts & Assumptions

[F1] For $M>0$ and $|a|\leq M$, the Kerr definition gives $J=Ma$, $r_+=M+\sqrt{M^2-a^2}$, and the exterior $r>r_+$, together with its displayed Boyer–Lindquist tensor. [def-kerr-metric](item-def-kerr-metric)

[F2] The Kerr exterior tensor is smooth on the sphere, and its $a=0$ line element is $-(1-2M/r)dt^2+(1-2M/r)^{-1}dr^2+r^2(d\theta^2+\sin^2\theta\,d\phi^2)$. [lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor)

## Proof

**Given:**$M>0$ and the Kerr exterior with $a=0$.

**Goal:** Identify its domain, angular momentum, and tensor with the stated Schwarzschild exterior.

1.1 Since $|0|\leq M$, [F1] applies. The positive square root satisfies $\sqrt{M^2}=M$, so $r_+=2M$ and the exterior domain is $r>2M$. The angular momentum is $J=M\cdot0=0$. [given, F1]

2.1 By [F2], setting $a=0$ gives exactly the displayed Schwarzschild line element. Its smooth extension over the spherical coordinate poles is the same sphere tensor supplied by [F2]. Together with the domain from step 1.1, this identifies the $a=0$ Kerr exterior with the stated Schwarzschild exterior. [given, F2, step 1.1] ∎

## Source notes

The article identifies the $a=0$ member as Schwarzschild in §1.1. This is attribution only; the calculation above uses the completed geometric suppliers.

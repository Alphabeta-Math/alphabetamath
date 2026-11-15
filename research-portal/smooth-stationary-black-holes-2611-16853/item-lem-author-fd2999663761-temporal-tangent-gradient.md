---
title: Temporal angle and tangential height gradient identity
status: draft
research_item: lem-author-fd2999663761-temporal-tangent-gradient
dependency_level: 3
---

## Prerequisites

- [def-author-fd2999663761-temporal-angle-data](item-def-author-fd2999663761-temporal-angle-data)


## Statement

For the temporal angle data, the tangential projection of $V$ is $W=V-vn$ and satisfies $|W|_h^2=v^2-1$. Consequently $\nabla_\Sigma\tau=-\alpha W$ and $|\nabla_\Sigma\tau|_h^2=\alpha^2(v^2-1)$. If $\alpha\ge a_0>0$, this gives $|\nabla_\Sigma\tau|_h^2\ge a_0^2(v^2-1)$.

## Facts & Assumptions

[F1] The temporal angle data have $g(n,n)=g(V,V)=-1$, $g(n,V)=-v$ and $\operatorname{grad}_g\tau=-\alpha V$. [def-author-fd2999663761-temporal-angle-data](item-def-author-fd2999663761-temporal-angle-data)

## Proof

**Given:** The data in [F1]. **Goal:** Establish the projections and norm identity.

1.1 The vector $W=V-vn$ is tangent because $g(W,n)=-v+v=0$. Expansion gives $g(W,W)=-1+2v^2-v^2=v^2-1$. [F1, algebra]

2.1 For every tangent $Y$, $d\tau(Y)=-\alpha g(V,Y)=-\alpha h(W,Y)$. The defining property of the induced gradient gives $\nabla_\Sigma\tau=-\alpha W$. Squaring and using step 1.1 gives the identity and its lower-bound consequence. [F1, step 1.1, algebra] ∎

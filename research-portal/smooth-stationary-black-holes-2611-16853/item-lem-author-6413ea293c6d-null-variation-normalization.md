---
title: Outward unit variation in the normalized null basis
status: published
research_item: lem-author-6413ea293c6d-null-variation-normalization
dependency_level: 6
sources:
  references:
    - title: Andersson–Mars–Simon, Stability of marginally outer trapped surfaces and
        existence of marginally outer trapped tubes
      url: https://arxiv.org/pdf/0704.2889
      locator: Sections 2–3, printed pages 5–8
---

## Prerequisites

- [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)


## Statement

In the normal plane of the surface data [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data), let $l=L=n+\nu$, $k=2\underline L=n-\nu$ and $v=\nu$. Then $g(l,k)=-2$, $g(l,v)=1$, $v=-k/2+Vl$ with $V=1/2$, and the accompanying normal $u=k/2+Vl$ is $n$. The future normal $n$ is timelike unit and $\nu$ is spacelike unit, with $g(n,\nu)=0$.

## Facts & Assumptions

[F1] The supplied surface gauge fixes the orthonormal normal pair and its null combinations. [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)

## Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Establish its identities with the indicated normalizations.

1.1 Expand the pairings using $g(n,n)=-1$, $g(\nu,\nu)=1$ and $g(n,\nu)=0$; they give $g(n+\nu,n-\nu)=-2$ and $g(n+\nu,\nu)=1$. [given, F1, algebra]

2.1 The identity $-k/2+Vl=(-1/2+V)n+(1/2+V)\nu$ equals $\nu$ exactly for $V=1/2$. Substituting this value in $k/2+Vl$ gives $n$. [step 1.1, F1, algebra] ∎

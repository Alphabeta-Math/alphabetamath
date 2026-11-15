---
id: lem-author-294e9b08725d-stationary-end-extrinsic-decay
title: Extrinsic curvature decay on the original stationary end
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-regular-stationary-vacuum-spacetime
  - def-stationary-asymptotic-decay-data
  - lem-author-a4a441da4986-exact-outer-cauchy-section
  - def-spacelike-maximal-hypersurface-data
dependency_roles:
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  lem-author-a4a441da4986-exact-outer-cauchy-section: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
proof_strategy: direct
dependency_level: 4
---

## Statement

On the $t=0$ end of the original regular stationary geometry, let $h=g_{ij}\,dx^i dx^j$ and $T=\partial_t=Nn+X$, with $n$ the future normal chosen so that $N>0$ there. From $g_{00}=-1+2M_0/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$, and $g_{ij}=\delta_{ij}+O_6(r^{-1})$, one obtains $N=1+O_6(r^{-1})$, $X=O_6(r^{-2})$ and $k=O_5(r^{-3})$. Consequently $\operatorname{tr}_h k=O_5(r^{-3})$. This conclusion does not assume the section maximal or $M_0$ positive.

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[F1] The end coefficients are stationary and satisfy spatial differentiated Cartesian bounds through order six; the original section agrees with $t=0$ sufficiently far out. [[def-regular-stationary-vacuum-spacetime]] [[def-stationary-asymptotic-decay-data]] [[lem-author-a4a441da4986-exact-outer-cauchy-section]]

[F2] The lapse-shift decomposition and sign convention are $T=Nn+X$ and $k=-g(\nabla n,\cdot)$. [[def-spacelike-maximal-hypersurface-data]]

## Proof

**Given:**The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[F1] The end coefficients are stationary and satisfy spatial differentiated Cartesian bounds through order six; the original section agrees with $t=0$ sufficiently far out. [[def-regular-stationary-vacuum-spacetime]] [[def-stationary-asymptotic-decay-data]] [[lem-author-a4a441da4986-exact-outer-cauchy-section]]

[F2] The lapse-shift decomposition and sign convention are $T=Nn+X$ and $k=-g(\nabla n,\cdot)$. [[def-spacelike-maximal-hypersurface-data]]



1.1 The end metric $h$ is uniformly positive for large $r$, its inverse is $\delta+O_6(r^{-1})$, and $X^i=h^{ij}g_{0j}=O_6(r^{-2})$. The identity $N^2=-g_{00}+h(X,X)$ gives $N=1+O_6(r^{-1})$, using the positive root. These inverse and square-root bounds follow by differentiating the identities and Leibniz rule up to order six. [F1, F2, algebra]

2.1 Stationarity gives $0=\partial_t h=-2Nk+\mathcal L_Xh$. The coordinate formula $(\mathcal L_Xh)_{ij}=X^a\partial_a h_{ij}+h_{aj}\partial_iX^a+h_{ia}\partial_jX^a$ is $O_5(r^{-3})$. Divide by $2N$ and contract with $h^{-1}$ to obtain both claimed curvature and trace bounds. [F1, F2, algebra] ∎

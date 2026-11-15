---
id: lem-author-e7cde3233cd7-normalized-end-primitive
title: Fixing the Ernst constant by integrable asymptotic twist
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-complex-self-dual-two-form-data
  - def-stationary-asymptotic-decay-data
  - thm-vacuum-killing-ernst-input
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  thm-vacuum-killing-ernst-input: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references: []
dependency_level: 5
---

## Statement

In a stationary vacuum end $\mathbb R\times\{|x|>R\}$ with $T=\partial_t$, suppose $g_{00}=-1+2M_0/r+O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$ and $g_{0i}=O_6(r^{-2})$. If a smooth primitive $s$ of $\eta=2i_T(F+i\star_gF)$ is defined on a connected domain containing the end, where $F=\tfrac12\mathrm dT^\flat$, it can be shifted by exactly one complex constant so that $s=f+i\psi\to1$ uniformly in angle on that end, with $f=-g(T,T)$ and $\psi=O(r^{-2})$. The normalized primitive is stationary and unique on its connected domain.

## Facts & Assumptions

[F1] Metric, orientation, Killing and Hodge conventions are [[def-stationary-lorentzian-data]] and [[def-complex-self-dual-two-form-data]]; differentiated decay uses [[def-stationary-asymptotic-decay-data]].

[F2] In vacuum $\eta$ is closed, its real part is $\mathrm df$, and $F=\tfrac12\mathrm dT^\flat$. [[thm-vacuum-killing-ernst-input]]

## Proof

**Given:**The hypotheses in the Statement and the declared supplier interfaces.

**Goal:** Prove the stated conclusions.

1.1 By [F2], $\operatorname{Re}s-f$ is constant on the connected domain. Subtract this real constant. In end coordinates, stationarity gives $F_{ij}=\tfrac12(\partial_i g_{0j}-\partial_j g_{0i})=O(r^{-3})$ and $F_{0i}=-\tfrac12\partial_i g_{00}=O(r^{-2})$. The inverse metric has bounded spatial components and $g^{0i}=O(r^{-2})$. In $(\star_gF)_{0i}=\tfrac12\epsilon_{0i}{}^{ab}F_{ab}$ the purely spatial contributions are $O(r^{-3})$ and terms involving a time index acquire a factor $g^{0j}$ and are $O(r^{-4})$. Hence $\partial_i\operatorname{Im}s=2(\star_gF)_{0i}=O(r^{-3})$, uniformly in angle. [given, F1, F2, algebra]

2.1 Integrating this bound along each radial ray gives a finite limit $c(\omega)$ and $|\operatorname{Im}s(r\omega)-c(\omega)|\le Cr^{-2}$. Join two directions by a great-circle arc of length at most $\pi r$ on the sphere of radius $r$; step 1.1 bounds the difference of their imaginary values by $C\pi r^{-2}$. Passing to the radial limits proves that all $c(\omega)$ are one constant $c$, and the radial bound is uniform. Subtract $ic$ to obtain $\psi=O(r^{-2})$ and $s\to1$ since $f\to1$. Antisymmetry gives $\eta(T)=2\mathcal F(T,T)=0$, so $T(s)=0$. Two primitives differ by a constant on a connected domain; their equal limit at infinity forces that constant to vanish. [given, F1, F2, step 1.1] ∎

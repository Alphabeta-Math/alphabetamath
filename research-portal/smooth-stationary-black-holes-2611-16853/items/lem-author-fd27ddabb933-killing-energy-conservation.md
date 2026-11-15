---
id: lem-author-fd27ddabb933-killing-energy-conservation
title: The stationary Killing energy is constant along every affine null segment
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:thm-gr-killing-and-on-shell-matter-identities
  - def-stationary-lorentzian-data
  - math:def-axiom-of-choice
  - math:def-geodesic-of-an-affine-connection
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-observer-and-rest-space
  - physics:lem-gr-observer-pairing-with-future-causal-vectors
dependency_roles:
  physics:thm-gr-killing-and-on-shell-matter-identities: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-geodesic-of-an-affine-connection: mathematical-premise
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-observer-and-rest-space: mathematical-premise
  physics:lem-gr-observer-pairing-with-future-causal-vectors: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Work in ZFC. For an affine null geodesic in the stationary metric, $E=-g(T,\dot\gamma)$ is constant. This conclusion needs no timelike assumption on T along the full segment. Where T is future timelike and the geodesic future null, E is strictly positive.

## Facts & Assumptions

[F1] The contraction of a Killing field with an affine geodesic tangent is constant (clause (b)). [[physics:thm-gr-killing-and-on-shell-matter-identities]]

[F2] The stationary field is a specified smooth Killing field, whether or not it is timelike in the interior. [[def-stationary-lorentzian-data]]

[F3] An affinely parametrized geodesic is a smooth curve on an interval with nonempty interior satisfying $D_t\dot\gamma=0$ for the specified affine connection, with one-sided interpretation at an included endpoint. [[math:def-geodesic-of-an-affine-connection]]

[F4] A null tangent vector $w$ is nonzero and satisfies $g(w,w)=0$; a nonzero causal vector is future-directed when $g(w,N)<0$. [[physics:def-gr-smooth-lorentzian-objects]]

[F5] An observer at $p$ is a tangent vector $n$ satisfying $g_p(n,n)=-1$ and $g_p(n,N_p)<0$. [[physics:def-gr-observer-and-rest-space]]

[F6] For an observer $n$ and a nonzero future causal vector $w$ at the same point, $-g_p(n,w)>0$ (claim 1). [[physics:lem-gr-observer-pairing-with-future-causal-vectors]]

[A1] Work in ZFC, including the axiom of choice; this includes the countable choice used in the smooth Lorentzian interface. [[math:def-axiom-of-choice]]

## Proof

**Given:** The assumptions in the Statement.

**Goal:** Establish constancy on the affine segment and positivity at every point with the stated future timelike and future null hypotheses.

1.1 The stationary data in [F2] give an oriented time-oriented smooth Lorentzian four-manifold and its Levi–Civita connection, with $T$ Killing. The given affine null geodesic satisfies $D_t\dot\gamma=0$ by [F3]. Thus clause (b) of [F1] applies and $g(T,\dot\gamma)$, hence $E=-g(T,\dot\gamma)$, is constant on its parameter interval. That clause requires no timelike condition on $T$. [F1, F2, F3, given, algebra]

2.1 At any point $p=\gamma(t)$ where $T_p$ is future timelike and $w=\dot\gamma(t)$ is future null, put $a=\sqrt{-g_p(T_p,T_p)}>0$ and $n=T_p/a$. Bilinearity gives $g_p(n,n)=-1$ and $g_p(n,N_p)=g_p(T_p,N_p)/a<0$, so $n$ is an observer by [F5]. The vector $w$ is nonzero future causal by [F4], so [F6] gives $-g_p(n,w)>0$. Consequently $E(t)=-g_p(T_p,w)=a[-g_p(n,w)]>0$. Together with step 1.1 this proves both assertions. [F2, F4, F5, F6, given, step 1.1, algebra] ∎

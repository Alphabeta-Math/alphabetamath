---
id: lem-author-56ff511785bf-boost-frame-bounds
title: Boost-frame bounds for a smooth observer and arbitrary spacelike normals
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-spacelike-maximal-hypersurface-data
dependency_roles:
  def-spacelike-maximal-hypersurface-data: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-altered
proof_strategy: direct
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum, arXiv:2610.09729v1
      url: https://arxiv.org/pdf/2610.09729v1
      locator: Appendix B, proof of Lemma B.1, printed/PDF pp.38–39; frame bound
        immediately after (B.8) and tangent-component identity immediately
        before (B.10)
      statement: In an ambient Lorentz-orthonormal frame with time axis V, the normal
        and tangent-frame components are bounded by a constant times v; the
        squared tangent components of V sum to v squared minus one.
      hypotheses: The pointwise setting uses a future unit timelike observer V, a
        future unit normal T0 to a spacelike hypersurface, a tangent orthonormal
        frame, and v=-g(T0,V).
      reading_limits: Consulted the PDF text on pp.38–39, specifically the frame-bound
        sentence after (B.8) and the tangent-component identity before (B.10).
        Images were unavailable. This item's two proof steps are a local
        pointwise Lorentz-frame calculation, with no differentiation of v or
        logarithmic argument. Its exact comparison-metric formulas and validity
        for every v>=1 are established locally. The source's differential
        estimates, arcosh argument on v>2, and weighted maximum estimate are not
        imported.
dependency_level: 1
---

## Statement

Let $g$ have signature $(-,+,+,+)$, let $U$ be a future unit timelike vector field, and let $n$ be the future unit normal of a spacelike hypersurface. Put $v=-g(n,U)$ and $e=g+2U^\flat\otimes U^\flat$, where $U^\flat=g(U,\cdot)$. Then $e$ is positive definite, $v\ge1$ and $|n|_e^2=2v^2-1$. For any $g$-orthonormal tangent basis $(e_a)_{a=1}^3$ set $Z_a=g(U,e_a)$. Then $\sum_aZ_a^2=v^2-1$ and $|e_a|_e\le\sqrt2v$. These estimates do not require an a priori bound on the candidate normal. Tensor norms below are the operator norms obtained by using $e$ on every slot and its induced dual metric.

## Facts & Assumptions

[F1] Use the induced positive metric, future unit normal and Lorentzian orthogonal decomposition of the spacelike hypersurface interface. [[def-spacelike-maximal-hypersurface-data]]

## Proof

**Given:**The vectors and frame in the Statement. **Goal:** Establish the positive comparison metric and the displayed bounds.

1.1 In a Lorentz-orthonormal ambient frame with time axis $U$, $g$ is $\operatorname{diag}(-1,1,1,1)$ and $e$ is the identity matrix. Write $n=vU+z$ with $z\perp U$. Future orientation makes $v>0$, and $-1=-v^2+|z|^2$ gives $v\ge1$ and $|n|_e^2=v^2+|z|^2=2v^2-1$. [F1, given, algebra]

2.1 The tangent projection of $U$ onto $n^\perp$ is $U-vn$, whose squared norm is $v^2-1$ and whose components are $Z_a$. Hence $\sum_aZ_a^2=v^2-1$. Also $|e_a|_e^2=g(e_a,e_a)+2g(U,e_a)^2=1+2Z_a^2\le2v^2-1\le2v^2$. This proves the claimed estimates at every $v\ge1$. [F1, step 1.1, algebra] ∎

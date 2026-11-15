---
id: def-lapse-shift-notation
title: Lapse, shift, induced metric and second fundamental form
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-lorentzian-data
dependency_roles:
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 4, Remark 1.3; p. 5, equation (1.3)
      attribution: The article writes the stationary field as a normal lapse term plus
        a tangential shift, specifies the induced metric and its sign convention
        for the second fundamental form, and uses the corresponding expression
        for the negative squared norm of the stationary field.
      hypotheses: The article's spacelike section and stationary Lorentzian setting;
        this reference attributes the notation and does not supply the
        justification below.
      reading_limits: The frozen article text at Remark 1.3 was inspected for the
        decomposition and second fundamental form; the supplied extraction
        records the norm identity and its article locator. No independent source
        proof review is claimed.
dependency_level: 1
---

## Definition

Let $(M,g,T)$ be stationary Lorentzian data as in [[def-stationary-lorentzian-data]], with signature $(-,+,+,+)$ and Levi–Civita connection $\nabla$. Let $\Sigma_0$ be a smooth embedded spacelike hypersurface, meaning that $g$ is positive definite on each three-dimensional tangent space, and let $n$ be its future-directed unit normal: $g(n,n)=-1$ and $g(n,U)=0$ for every tangent vector $U$. These hypersurface conventions are those of [[def-spacelike-maximal-hypersurface-data]].

The induced metric is $h(U,V)=g(U,V)$ for tangent vectors $U,V$, and the second fundamental form in this sign convention is $k(U,V)=-g(\nabla_U n,V)$. Define the lapse $N=-g(T,n)$ and the shift $X=T-Nn$ along $\Sigma_0$. Thus $T=Nn+X$ with $X$ tangent. With $|X|_h^2=h(X,X)$ and $f=-g(T,T)$, the notation satisfies $f=N^2-|X|_h^2$. No sign condition on $N$ is imposed by these definitions.

## Facts & Assumptions

[F1] The stationary data provide a smooth Lorentzian metric of the stated signature, the vector field $T$, its Levi–Civita connection and the scalar $f=-g(T,T)$. [[def-stationary-lorentzian-data]]

[F2] For the stated spacelike hypersurface, the future unit normal, induced metric and displayed second fundamental form are well-defined; the lapse and shift give the unique normal–tangent decomposition. [[def-spacelike-maximal-hypersurface-data]]

## Justification

**Given:** The stationary data and spacelike hypersurface in the Definition.

**Goal:** Justify the defined fields, the decomposition and the identity for $f$.

1.1 The hypersurface supplier gives the smooth future unit normal, positive-definite induced metric and well-defined second fundamental form with the displayed sign. It also gives the lapse and the tangent shift $X=T-Nn$, so $T=Nn+X$ is the unique decomposition of that form. [F1, F2, given]

2.1 Since $g(n,n)=-1$ and $g(n,X)=0$, bilinearity gives $g(T,T)=-N^2+g(X,X)$. The definition of $h$ makes $g(X,X)=|X|_h^2$, and hence $f=-g(T,T)=N^2-|X|_h^2$. This calculation requires no positivity assumption on $N$. [F1, F2, step 1.1] ∎

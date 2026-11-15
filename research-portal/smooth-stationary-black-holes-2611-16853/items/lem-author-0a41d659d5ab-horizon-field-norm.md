---
id: lem-author-0a41d659d5ab-horizon-field-norm
title: Horizon smallness is the induced norm of the tangential stationary field
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-author-0a41d659d5ab-aik-quantitative-package
  - def-spacelike-maximal-hypersurface-data
  - math:def-axiom-of-choice
  - math:cor-transverse-intersection-theorem
  - math:cor-euclidean-closed-balls-and-spheres-are-compact
  - math:thm-compactness-under-continuous-maps
dependency_roles:
  def-author-0a41d659d5ab-aik-quantitative-package: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:cor-transverse-intersection-theorem: mathematical-premise
  math:cor-euclidean-closed-balls-and-spheres-are-compact: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references: []
dependency_level: 3
---

## Statement

For the AIK quantitative package, $g(T,T)=-n^2+h(X,X)$ on $\Sigma_0$. On $S_0$ the stationary field is tangent to $S_0$, $n=0$ and $X=T$. Consequently $g(T,T)=|T|_h^2\ge0$ there and $\sup_{S_0}|g(T,T)|<\epsilon^2$ is exactly $\sup_{S_0}|T|_h<\epsilon$ for $\epsilon>0$. The norm is the induced Riemannian norm on the spacelike sphere, not an unspecified Lorentzian vector norm.

## Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [[math:def-axiom-of-choice]]

[F1] The GR/SBS package fixes the transverse horizon intersection and the tangencies of $T$. [[def-author-0a41d659d5ab-aik-quantitative-package]]

[F2] The unique normal/shift decomposition is $T=n\nu+X$, with $g(\nu,\nu)=-1$ and $g(X,\nu)=0$. [[def-spacelike-maximal-hypersurface-data]]

[F3] For transverse embedded submanifolds, the tangent space of their intersection is the intersection of their tangent spaces. [[math:cor-transverse-intersection-theorem]]

[F4] The Euclidean unit sphere in $\mathbb R^3$ is compact. [[math:cor-euclidean-closed-balls-and-spheres-are-compact]]

[F5] Continuous images of compact spaces are compact, and a continuous real-valued function on a nonempty compact space attains its maximum and minimum. [[math:thm-compactness-under-continuous-maps]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conditional conclusion.

1.1 The decomposition in [F2] gives $g(T,T)=n^2g(\nu,\nu)+2ng(\nu,X)+g(X,X)=-n^2+h(X,X)$. At a point $p\in S_0$, [F1] supplies $T_p\in T_pH^+\cap T_pH^-$, and transversality allows [F3] to identify this intersection with $T_pS_0$. Since $S_0\subset\Sigma_0$, it follows that $g(T,\nu)=0$, hence $n=0$ and $X=T$. [F1, F2, F3, algebra]

2.1 The package identifies $S_0$ as the image of the nonempty unit sphere $\{x\in\mathbb R^3:|x|=1\}$ under the smooth map $\Phi_0$. The unit sphere is compact by [F4], so its continuous image $S_0$ is nonempty and compact by [F5]. The induced metric is positive definite, and the function $f(p)=|T_p|_h=\sqrt{h_p(T_p,T_p)}$ is continuous: in local coordinates its square is a finite sum of products of smooth metric and field components, and the nonnegative square root is continuous. Thus [F5] gives a maximum $m=\max_{S_0}f\ge0$. [step 1.1, F1, F2, F4, F5]

3.1 By step 1.1, $g(T,T)=h(T,T)=f^2\ge0$ on $S_0$. Since $0\le f\le m$ and $f$ attains $m$, the increasing square function gives $\sup_{S_0}|g(T,T)|=m^2$ and $\sup_{S_0}|T|_h=m$. For $\epsilon>0$, $m^2<\epsilon^2$ holds exactly when $m<\epsilon$, proving the two strict smallness conditions equivalent. It does not identify either with ADM angular-momentum smallness. [step 1.1, step 2.1, algebra] ∎

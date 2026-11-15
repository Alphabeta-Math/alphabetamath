---
id: lem-author-14de055b8ceb-uniform-elliptic-jet-extension
title: Uniform elliptic extension and flattening before the boundary gradient estimate
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-14de055b8ceb-gaussian-maximal-graph-operator
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - math:lem-euclidean-bump-for-a-compact-set-inside-an-open-set
  - math:thm-heine-borel-rn
  - math:thm-compactness-under-continuous-maps
  - math:thm-chain-rule-for-total-derivatives
  - math:thm-algebra-of-derivatives
dependency_roles:
  lem-author-14de055b8ceb-gaussian-maximal-graph-operator: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  math:lem-euclidean-bump-for-a-compact-set-inside-an-open-set: mathematical-premise
  math:thm-heine-borel-rn: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:thm-algebra-of-derivatives: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

For a smooth compact family of Gaussian graph operators, work in finitely many supplied background coordinate patches, including parameter coordinates, and let $\mathcal K$ be the compact admissible jet set containing all realized jets with $|u|+|Du|\le K_0$ and $s(x,u,Du)\le\theta_0^2<1$. The compact background range is contained in the smooth Gaussian coordinate domain. The operator supplier therefore gives a common open spacelike jet neighborhood $\mathcal O$ of $\mathcal K$ on which the principal matrix $A$ and lower-order coefficient $b$ are smooth. One may extend $A$ smoothly to a containing full height/slope box, with common joint $C^1$ bounds and common uniform ellipticity, keeping it unchanged at every realized jet. This is a coordinatewise coefficient extension; no metric outside its supplied domain is required.

Smooth boundary flattening $y=\Phi(x)$ with uniformly bounded $C^2$ maps and inverses preserves these principal-coefficient properties. Writing $\widetilde u=u\circ\Phi^{-1}$, its actual boundary trace is exactly $(u|_{\partial\Omega})\circ\Phi^{-1}$. In particular an originally zero graph-height trace remains zero; the extension is equally applicable on interior patches with no boundary condition. The realized forcing $f(x)=-b(x,u,Du)$ remains uniformly bounded, and so does the transformed forcing for a solution of $A^{ij}u_{ij}+b=0$. No Holder bound on $Du$ is needed for this reduction.

## Facts & Assumptions

[F1] The Gaussian operator has smooth coefficients on its spacelike jet domain and common joint bounds of every finite order, with common positive ellipticity bounds, on compact background and strict spacelike jet ranges. Apply this only on a slightly larger neighborhood of the compact admissible set, rather than assuming the metric is defined on an entire height/slope box. [[lem-author-14de055b8ceb-gaussian-maximal-graph-operator]]

[F2] Joint $C^1$ bounds mean bounds for the coefficient functions and their first derivatives in the independent position, height and slope variables, with parameters included among the supplied background variables. These are coefficient bounds before evaluation at a solution, not Holder bounds on $Du$. Use the fixed-domain norm and boundary-extension conventions of [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]].

[F3] For a compact subset $K$ of an open Euclidean set $O$, there is a smooth $\zeta$ with $0\le\zeta\le1$, $\zeta=1$ on $K$ and $\operatorname{supp}\zeta\subset O$. [[math:lem-euclidean-bump-for-a-compact-set-inside-an-open-set]]

[F4] Closed bounded Euclidean sets are compact, and continuous real functions on nonempty compact sets attain finite extreme values. Apply these facts to the finite coordinate patches, cutoff supports and coefficient derivatives. Empty jet sets require only the identity extension. [[math:thm-heine-borel-rn]] [[math:thm-compactness-under-continuous-maps]]

[F5] The Euclidean total derivative satisfies the chain rule on open coordinate domains. Boundary formulas follow from the supplied smooth one-sided extensions. [[math:thm-chain-rule-for-total-derivatives]]

[F6] For real functions $f,g$ differentiable at a limit point $c$ of their common real domain, $(f+g)'(c)=f'(c)+g'(c)$, $(\alpha f)'(c)=\alpha f'(c)$ for real $\alpha$, and $(fg)'(c)=f'(c)g(c)+f(c)g'(c)$. Apply these identities on open intervals obtained by fixing all but one coordinate of the smooth coefficient and chart functions. Repeated product applications handle finite products; the supplied smooth one-sided extensions give the same formulas at boundary points. [[math:thm-algebra-of-derivatives]]

## Proof

**Given:** The compact Gaussian background and admissible jets, height/slope bound, and supplied boundary charts in the Statement. **Goal:** Establish the coefficient-box reduction, transformed forcing bound and exact trace transport.

1.1 If $\mathcal K$ is empty, use the identity matrix. Otherwise choose a bounded open neighborhood $\mathcal O_0$ of $\mathcal K$ with compact closure contained in $\mathcal O$: cover the compact set by finitely many small coordinate balls whose closed larger balls lie in $\mathcal O$, and take their union. Apply [F3] with $K=\mathcal K$ and $O=\mathcal O_0$. Define $\widetilde A=I+\zeta(A-I)$ on $\mathcal O$ and $\widetilde A=I$ outside $\mathcal O$. Since the closed support of $\zeta$ is contained in $\mathcal O_0$, this formula equals $I$ on a neighborhood of every point outside that support; it therefore defines a smooth matrix on the whole coordinate jet space. The original $A$ is evaluated only inside its supplied domain, and $\widetilde A=A$ on $\mathcal K$. Apply this construction in each of the finitely many patches. [given, F1, F3, F4, construct]

2.1 On the compact closure of $\mathcal O_0$, [F1] gives $\lambda I\le A\le\Lambda I$ for common $0<\lambda\le\Lambda$. Since $\widetilde A=\zeta A+(1-\zeta)I$, its quadratic form lies between $\min(\lambda,1)|\xi|^2$ and $\max(\Lambda,1)|\xi|^2$. Smooth coefficient and cutoff derivatives have finite bounds on that compact set by [F4]; outside the cutoff support the extension is constant. Applying the product rule [F6] to each scalar coordinate restriction thus gives common joint $C^1$ bounds on any containing full finite height/slope box. Finite maxima over the background patches give common constants. Likewise the original smooth $b$ is bounded on $\mathcal K$, so $f=-b(x,u,Du)$ is bounded at every realized jet, without differentiating $Du$. [given, F1, F2, F4, F6, step 1.1, algebra]

3.1 Under $y=\Phi(x)$ write $q=D_y\widetilde u$ and $p=D\Phi(x)^Tq$. Applying [F5] twice and the product rule [F6] gives $u_{ij}=\Phi^a_i\Phi^b_j\widetilde u_{ab}+\Phi^a_{ij}q_a$. Thus the transformed principal matrix is $\widehat A^{ab}=\Phi^a_i\widetilde A^{ij}(x,z,D\Phi^Tq)\Phi^b_j$. The bounds on $D\Phi$ and its inverse preserve its two ellipticity constants up to common factors. By [F5] and [F6], the joint first derivatives of this expression use at most $D^2\Phi$ and first joint derivatives of $\widetilde A$, hence have common bounds. The transformed containing box may be enlarged to contain the bounded transformed heights and slopes. For an actual solution the right side is $\widehat f=-b(x,u,Du)-A^{ij}(x,u,Du)\Phi^a_{ij}q_a$, evaluated at $x=\Phi^{-1}(y)$. Every factor is bounded by the supplied chart bounds, gradient bound and step 2.1. Therefore $\widehat f$ is uniformly bounded as well; no derivative of the evaluated gradient appears. [given, F1, F2, F5, F6, step 2.1, algebra]

4.1 A base-coordinate change leaves the scalar height value unchanged: $\widetilde u(y)=u(\Phi^{-1}(y))$. Restricting this identity to the actual flattened boundary gives the trace formula in the Statement. It preserves an originally zero trace and transports any other trace rather than replacing it by zero. On interior patches step 2.1 applies without a trace assumption. These observations and step 3.1 establish every claimed reduction. [given, F5, step 2.1, step 3.1] ∎

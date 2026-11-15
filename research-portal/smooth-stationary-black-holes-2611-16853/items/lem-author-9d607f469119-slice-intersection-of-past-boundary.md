---
id: lem-author-9d607f469119-slice-intersection-of-past-boundary
title: Intersecting a chronological past boundary with a spacelike section
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves
  - math:def-geodesic-of-an-affine-connection
  - math:def-affine-connection-on-a-smooth-manifold
  - math:def-interior-closure-boundary-top
  - math:def-subspace-topology-top
dependency_roles:
  math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves: mathematical-premise
  math:def-geodesic-of-an-affine-connection: mathematical-premise
  math:def-affine-connection-on-a-smooth-manifold: mathematical-premise
  math:def-interior-closure-boundary-top: mathematical-premise
  math:def-subspace-topology-top: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609
      locator: Sections 1.2–1.3, 1.5 and 1.7, pp. 6–11; section 1.11, Proposition
        1.16, pp. 15–17; section 2.3, p. 28; Theorem 2.12 and Remark 2.14, pp.
        32–33; Proposition 2.23 and Theorem 2.24, p. 36. PDF page numbers equal
        printed page numbers.
      statement: In arbitrary finite spacetime dimension, chronology is open. Timelike
        reachability composed with causal reachability in either order is
        timelike reachability. Causal AC-curves are continuous causal curves;
        continuous causal curves admit causal Lipschitz parametrizations. A
        continuous causal curve of positive Lorentzian length has
        chronologically related endpoints.
      hypotheses: A connected noncompact time-oriented Hausdorff second-countable
        smooth manifold with a C2 Lorentzian metric; all relations are intrinsic
        to that manifold. AC causal velocities are nonzero almost everywhere.
      reading_limits: Read the listed PDF-text passages and the proofs of Proposition
        1.16 and Theorem 2.24. Import these facts only; no full-source
        verification. The AC-chronology correspondence and componentwise
        application are explained locally below.
dependency_level: 0
---

## Statement

Let $(E,g)$ be a smooth time-oriented Lorentzian manifold without boundary of finite dimension $d\ge2$, with signature $(-,+,\ldots,+)$, and let $\nabla$ be a supplied smooth torsion-free, metric-compatible affine connection. Let $v:E\to\mathbb R$ be smooth and temporal: the gradient defined by $g(\operatorname{grad}_g v,X)=dv(X)$ is past-directed timelike everywhere. Put $\Sigma^\circ=v^{-1}(0)$, with its subspace topology. For $Q\subset E$, set $P=I^-_E(Q)$, using locally absolutely continuous curves with nonzero future timelike velocity almost everywhere. Boundaries denoted $\partial_X$ are taken in the specified space $X$.

Suppose $p\in\Sigma^\circ\cap\partial_E P$ and there are $a<b$ and a smooth affinely parametrized $\nabla$-geodesic $\gamma:[a,b]\to E$ with $\gamma(a)=p$, $\gamma(b)\in Q$, and $\gamma([a,b])\subset\partial_E P$. Require $\gamma'$ to be nonzero, future-directed and null everywhere, including one-sided endpoint values; in particular the segment is nonconstant. Then $p\in\partial_{\Sigma^\circ}(P\cap\Sigma^\circ)$.

For the consequence, let $\Sigma$ be a topological space containing $\Sigma^\circ$ as an open subspace, with the topology just specified; in particular $\Sigma$ may be a section with boundary whose interior is $\Sigma^\circ$. Let $B\subset\Sigma$ be closed, set $B^\circ=B\cap\Sigma^\circ$ and $K=B\setminus P$, and define its outer section boundary to be $O=\partial_{\Sigma^\circ}B^\circ$. Assume every point of $O$ has a $\Sigma^\circ$-open neighborhood contained in $P\cap\Sigma^\circ$. If every $p\in B^\circ\cap\partial_E P$ has a null segment as above, then

$$\partial_{\Sigma^\circ}(K\cap\Sigma^\circ)=B^\circ\cap\partial_E P.$$

Thus the portion inside $B$ means exactly $B^\circ\cap\partial_E P$; it is also contained in $\operatorname{int}_{\Sigma^\circ}B^\circ$.

## External input

The general-dimensional causal premises are imported from [Minguzzi, Lorentzian causality theory](https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609), at the precise locators in the source record: chronology is open (Proposition 1.16); timelike–causal composition gives timelike reachability (Theorem 2.24); causal AC-curves give continuous causal curves and the latter admit causal Lipschitz parametrizations (Theorem 2.12 and Remark 2.14); positive Lorentzian length implies chronological reachability (Proposition 2.23). These are mathematical premises for the local proof, not claims of local reconstruction of those results.

## Facts & Assumptions

[F1] Use the imported general-dimensional causal facts in External input. A causal AC-curve has nonzero future causal velocity almost everywhere; its length on a compact parameter interval is the integral of $\sqrt{-g(\gamma',\gamma')}$. Timelike AC-curves have positive length. The source uses piecewise smooth timelike reachability and continuous causal reachability; their applicability to the present AC convention is checked in step 1.1.

[F2] A smooth vector field has local integral curves depending smoothly on the initial point, on a common time interval near a fixed point. [[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]]

[F3] An affine connection is a connection on the tangent bundle; an affinely parametrized geodesic has zero covariant acceleration. The explicitly required nonzero future null tangent makes each nondegenerate restriction of $\gamma$ future causal. [[math:def-affine-connection-on-a-smooth-manifold]] [[math:def-geodesic-of-an-affine-connection]]

[F4] The subspace topology is given by traces of ambient open sets; its closed sets are traces of ambient closed sets. Boundary is closure minus interior and is unchanged on taking complements. [[math:def-subspace-topology-top]] [[math:def-interior-closure-boundary-top]]

## Proof

**Given:** The hypotheses and explicitly specified spaces, curves and boundaries in the Statement.

**Goal:** Prove the section-boundary assertion and the displayed equality.

1.1 The source's results apply componentwise to $E$: a connected component cannot be compact, since $v$ would attain a maximum there with $dv=0$, contradicting its timelike gradient. A future timelike AC-curve is causal AC and has strictly positive Lorentzian length; the imported continuous-curve characterization and positive-length result give a piecewise smooth future timelike curve with the same endpoints. Conversely a piecewise smooth future timelike curve is AC after a finite piecewise affine parametrization. Thus the two chronological relations coincide. Similarly the source's causal relation agrees with AC causal reachability by the imported curve characterization. Consequently $P$ is open, as a union of open chronological pasts, and push-up is valid for the curves used below, in every stated dimension. [given, F1]

1.2 Set $W=\operatorname{grad}_g v$ and $V=W/g(W,W)$. In coordinates the inverse matrix of the smooth nondegenerate metric is smooth, so $W$ and $V$ are smooth. The negative denominator makes $V$ future timelike and $dv(V)=1$. Moreover $dv(U)>0$ for every nonzero future causal vector $U$: in a Lorentz-orthonormal frame write $W=(-\alpha,w)$ and $U=(\beta,u)$ with $\alpha>|w|$ and $\beta\ge|u|>0$ for a null $U$, or $\beta>|u|\ge0$ for a timelike $U$; then $g(W,U)=\alpha\beta+w\cdot u\ge(\alpha-|w|)\beta>0$. In particular $v\circ\gamma$ is strictly increasing after $a$. [given, F3, algebra]

2.1 Let $y_j=\gamma(a+(b-a)/(j+1))$ for integers $j\ge1$. Then $y_j\to p$, $v(y_j)>0$ and $v(y_j)\to0$. By F2, for all large $j$ the local integral curve $s\mapsto\Phi(s,y_j)$ of $V$ is defined for $-v(y_j)\le s\le0$. Since $dv(V)=1$, its initial point $z_j=\Phi(-v(y_j),y_j)$ satisfies $v(z_j)=0$, and smooth dependence gives $z_j\to p$. This curve is future timelike from $z_j$ to $y_j$, while the remaining nondegenerate restriction of $\gamma$ is future causal from $y_j$ to $\gamma(b)\in Q$. Push-up gives $z_j\in P\cap\Sigma^\circ$. Openness of $P$ implies $p\notin P$. Hence every section neighborhood of $p$ meets $P\cap\Sigma^\circ$ and its complement, proving the first assertion. [given, F2, F3, F4, step 1.1, step 1.2]

2.2 Put $A=P\cap\Sigma^\circ$ and $L=K\cap\Sigma^\circ=B^\circ\setminus A$. The set $A$ is section-open, $B^\circ$ is section-closed, and therefore $L$ is section-closed. Take $x\in\partial_{\Sigma^\circ}L$. Then $x\in L\subset B^\circ$. It cannot be in $O$, since the assumed section neighborhood there is contained in $A$ and is disjoint from $L$. Hence $x\in\operatorname{int}_{\Sigma^\circ}B^\circ$. In that interior $L$ is locally the complement of $A$, so every section neighborhood of $x$ meets $A$, while $x\notin P$. For every ambient neighborhood $U$ of $x$, its trace $U\cap\Sigma^\circ$ is a section neighborhood and therefore meets $P$; it also contains $x\notin P$. Thus $x\in B^\circ\cap\partial_E P$. [given, F4, step 1.1]

3.1 Conversely, take $p\in B^\circ\cap\partial_E P$. Since $P$ is open, $p\notin P$ and hence $p\in L$. The assumed null segment lets step 2.1 apply, so every section neighborhood of $p$ meets $A$, which is disjoint from $L$. Each such neighborhood also meets $L$ at $p$ itself. Thus $p\in\partial_{\Sigma^\circ}L$. It cannot belong to $O\subset A$, so it lies in $\operatorname{int}_{\Sigma^\circ}B^\circ$. Together with step 2.2 this proves the equality and its stated inside interpretation. [given, F4, step 1.1, step 2.1, step 2.2] ∎

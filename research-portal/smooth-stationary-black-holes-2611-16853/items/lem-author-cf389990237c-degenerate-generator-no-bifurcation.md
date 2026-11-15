---
id: lem-author-cf389990237c-degenerate-generator-no-bifurcation
title: A nonzero degenerate generator cannot vanish at a regular bifurcation section
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - def-null-screen-expansion-and-focal-data
  - math:def-axiom-of-choice
  - math:def-affine-connection-on-a-smooth-manifold
  - math:def-geodesic-of-an-affine-connection
  - math:def-covariant-derivative-along-a-curve
  - math:thm-covariant-derivative-along-a-curve-is-independent-of-frame-and-extension
  - math:def-embedded-submanifold-and-slice-chart
  - math:prop-coordinate-formula-for-the-lie-bracket
  - math:lem-derivative-algebra-and-chain-rules
  - math:thm-chain-rule-for-total-derivatives
  - math:cor-zero-derivative-implies-constant
  - math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:thm-picard-lindelof-local-existence-and-uniqueness
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-affine-connection-on-a-smooth-manifold: mathematical-premise
  math:def-geodesic-of-an-affine-connection: mathematical-premise
  math:def-covariant-derivative-along-a-curve: mathematical-premise
  math:thm-covariant-derivative-along-a-curve-is-independent-of-frame-and-extension: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  math:prop-coordinate-formula-for-the-lie-bracket: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:cor-zero-derivative-implies-constant: mathematical-premise
  math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:thm-picard-lindelof-local-existence-and-uniqueness: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Use the horizon and null-geodesic conventions of [[def-bifurcate-killing-horizon-data]], [[def-null-screen-expansion-and-focal-data]] and [[def-stationary-lorentzian-data]]. Let a regular null branch be generated from a spacelike section $B$ by affine null geodesics $\gamma(\lambda)$ with $\lambda=0$ on $B$. A smooth generator $K$ normal to the branch cannot satisfy all three conditions: $K|_B=0$, $K\ne0$ on its punctured branch, and $\nabla_KK=0$ there. Hence a nonzero degenerate Killing generator has no regular bifurcation section for that same generator. The assertion does not exclude another, differently normalized or different Killing field.

## Facts & Assumptions

[A1] Retain the ZFC convention, including the axiom of choice, of the geometric interfaces; it supplies their inherited smooth-manifold choice assumptions. The constructions below are local and select only finitely many charts. [[math:def-axiom-of-choice]] [[def-stationary-lorentzian-data]] [[def-null-screen-expansion-and-focal-data]]

[F1] Regular affine generation in the first assertion supplies a smooth nonzero tangent $L=\dot\gamma$ through the section with $D_\lambda L=0$. For the final assertion, a Killing horizon $H$ has a dense nonzero set $H_*$, its null normal line is the radical of its tangent metric, and degeneracy means $\nabla_KK=0$ on $H_*$. A bifurcation surface is smooth, spacelike, contained in each branch, and has $K=0$ there. [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]] [[def-null-screen-expansion-and-focal-data]] [[math:def-geodesic-of-an-affine-connection]]

[F2] An affine connection is function-linear in its differentiating direction and satisfies $\nabla_X(fY)=X(f)Y+f\nabla_XY$. Along a smooth curve, $D_t(fV)=f'V+fD_tV$; when an ambient local extension exists, $D_tV=\nabla_{\dot\gamma}V$, independently of that extension. The connection here is torsion-free and metric-compatible. [[math:def-affine-connection-on-a-smooth-manifold]] [[math:def-covariant-derivative-along-a-curve]] [[math:thm-covariant-derivative-along-a-curve-is-independent-of-frame-and-extension]] [[def-stationary-lorentzian-data]]

[F3] An embedded hypersurface has a slice chart in which it is a coordinate hyperplane. Fields on that hyperplane admit local smooth extensions by making their components independent of the normal coordinate. In such coordinates the bracket formula shows that the bracket of tangent fields is tangent. [[math:def-embedded-submanifold-and-slice-chart]] [[math:prop-coordinate-formula-for-the-lie-bracket]]

[F4] Scalar product, quotient and chain rules apply to the smooth coefficients used below; in charts the total chain rule differentiates a scalar function composed with an integral curve. [[math:lem-derivative-algebra-and-chain-rules]] [[math:thm-chain-rule-for-total-derivatives]]

[F5] A real function continuous on an interval and differentiable with zero derivative at every interior point is constant on that interval. [[math:cor-zero-derivative-implies-constant]]

[F6] A smooth vector field on a manifold has a local smooth family of integral curves on a common time interval for initial points in a neighborhood. A smooth map with invertible differential at a point restricts to a diffeomorphism of neighborhoods. [[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]] [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[F7] For a continuous right-hand side locally Lipschitz in the scalar state, two solutions of the same first-order initial-value problem agree on every common interval containing the initial time. [[math:thm-picard-lindelof-local-existence-and-uniqueness]]

## Proof

**Given:** The geometric conventions and, for the first assertion, the three proposed properties; for the final assertion, a proposed regular bifurcation surface for the same degenerate Killing field.

**Goal:** Prove both the punctured-branch contradiction and its bifurcate-horizon consequence without assuming nonvanishing along each punctured generator in the latter case.

1.1 Along one affine generator choose a coordinate component $L^j$ nonzero at $\lambda=0$ and shrink the interval so it remains nonzero. Since $K$ is in the line spanned by $L$, the scalar $f=K^j/L^j$ satisfies $K=fL$. The quotient is smooth up to zero, $f(0)=0$, and $f\ne0$ on $(0,\epsilon)$. Smoothness of such a quotient follows by iterating the quotient rule; the same argument in each coordinate direction applies to the local quotients below. The extension-independent curve derivative and affine equation give $\nabla_KK=fD_\lambda(fL)=ff'L$. [given, A1, F1, F2, F4]

2.1 For the bifurcate-horizon consequence, choose one branch $H$ and a point $q$ of its spacelike bifurcation surface $S$. In a slice chart write $H=\{r=0\}$ with $dr\ne0$, and set $L=(dr)^\sharp|_H$ using the inverse metric. The annihilator of $TH=\ker dr$ is $\mathbb R\,dr$, so $(TH)^\perp=\mathbb RL$ and $L\ne0$. Because the tangent metric has a nonzero radical, this orthogonal line lies in $TH$; thus $L$ is tangent and null. Choose a component $L^j$ nonzero near $q$ and put $f=K^j/L^j$ there. On $H_*$ normality gives $K=fL$; at a zero of $K$ both sides vanish, so this equality holds on the entire patch. The quotient argument of step 1.1 makes $f$ smooth, including at its zeros. [given, F1, F3, F4, step 1.1]

2.2 In the affine case, degeneracy and step 1.1 imply $ff'=0$. Since $f\ne0$ on $(0,\epsilon)$, $f'=0$ there; F5 applies to that interval and makes $f$ constant. Its constant value is nonzero, whereas continuity at zero forces it to equal $f(0)=0$. This proves the first assertion. [given, F1, F5, step 1.1]

3.1 On the branch patch of step 2.1, let $X$ be any smooth tangent field. Metric compatibility, torsion freeness, and the tangency of $[L,X]$ give $g(\nabla_LL,X)=-g(L,\nabla_LX)=-g(L,\nabla_XL+[L,X])=-\tfrac12 X(g(L,L))=0$. Here $g(L,X)$ and $g(L,L)$ vanish on $H$, so their tangential derivatives vanish; slice-chart extensions justify the ambient calculation and F2 makes its tangential values independent of the extensions. Thus $\nabla_LL$ lies in $(TH)^\perp=\mathbb RL$, and $\nabla_LL=aL$ for a smooth scalar $a$, obtained by division by the same nonzero component $L^j$. This establishes the pregeodesic property locally rather than presuming an affine ruling. [F2, F3, F4, step 2.1]

3.2 Apply F6 to $L$ on the three-manifold $H$ to obtain smooth integral curves $\Phi(t,p)$ for $p$ in a small patch of $S$, with $\Phi(0,p)=p$. The nonzero null vector $L_q$ cannot lie in the positive-definite plane $T_qS$, so $T_qH=T_qS\oplus\mathbb RL_q$. The differential of $(t,p)\mapsto\Phi(t,p)$ at $(0,q)$ is therefore the isomorphism $(b,v)\mapsto bL_q+v$. The inverse function theorem, followed by restriction to a product $(-\delta,\delta)\times W$ with $q\in W\subset S$, makes this map a diffeomorphism onto a nonempty open collar $V$ in $H$. Shrink the product so its image stays in the patch above. [F1, F6, step 2.1]

4.1 On that patch, the connection rules and step 3.1 yield $\nabla_KK=f\bigl(L(f)+af\bigr)L$. On $H_*$, $f\ne0$ and degeneracy implies $L(f)+af=0$. This scalar is smooth on the whole patch; density of $H_*$ in $H$ forces it to vanish everywhere there, since a nonzero value would by continuity have a nonempty open neighborhood avoiding $H_*$. This uses density on $H$, without asserting density or nonvanishing on each individual generator. [given, F1, F2, step 2.1, step 3.1]

5.1 For each $p\in W$, set $h_p(t)=f(\Phi(t,p))$ and $a_p(t)=a(\Phi(t,p))$. The chain rule and step 4.1 give $h_p'=-a_p(t)h_p$ with $h_p(0)=0$, because $K=0$ on $S$. The coefficient $a_p$ is smooth, so the right-hand side is continuous and locally Lipschitz in the scalar state on $(-\delta,\delta)\times\mathbb R$. The zero function is another solution; F7 gives $h_p=0$ on the common interval $(-\delta,\delta)$. Hence $K=0$ throughout $V$, contradicting density of $H_*$. No regular bifurcation surface exists for this same degenerate generator. The qualification concerning another specified Killing field remains intact. [given, F1, F4, F7, step 3.2, step 4.1] ∎

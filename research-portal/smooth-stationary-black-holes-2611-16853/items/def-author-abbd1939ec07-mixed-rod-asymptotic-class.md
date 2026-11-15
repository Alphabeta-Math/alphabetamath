---
id: def-author-abbd1939ec07-mixed-rod-asymptotic-class
title: Exact mixed-rod boundary class for the balance theorem
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-author-abbd1939ec07-ordered-vacuum-rods
  - def-author-abbd1939ec07-reconstructed-harmonic-map-data
dependency_roles:
  def-author-abbd1939ec07-ordered-vacuum-rods: mathematical-premise
  def-author-abbd1939ec07-reconstructed-harmonic-map-data: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Han–Khuri–Weinstein–Xiong, Kerr Black Hole Uniqueness
      url: https://arxiv.org/html/2608.23325v1
      locator: §1 source-class paragraph immediately before Theorem 1.1; §2.1 opening
        variational hypothesis and (A1)–(A3), equations (2.3)–(2.10);
        Proposition 2.1(i),(iii), especially (2.23).
      statement: The source assumes renormalized-energy local minimality with fixed
        rod traces and singularity data, in addition to (A1)–(A3). Proposition
        2.1(i),(iii) supplies continuous axis representatives, smooth
        horizon-interior extensions of u,v, and the expansion (2.23).
      hypotheses: Axisymmetric weak harmonic maps into the displayed hyperbolic
        target, finite mixed rods, the stated variational hypothesis, and all
        (A1)–(A3). Smooth off-axis maps satisfy the weak-map requirement. The
        nonzero twist jumps are imposed at degenerate components. No generic
        spacetime membership assertion is imported.
      reading_limits: Read the HTML §1 setting and source-class paragraph, §2.1 in
        full, and the statements of Proposition 2.1(i),(iii), including (2.23).
        Its attribution proof was inspected, but the underlying regularity
        papers and the balance proof in §§3–6 were not reconstructed. The
        variational predicate is adopted from §2.1, not derived from
        harmonicity.
dependency_level: 7
---

## Definition

An admissible HKWX mixed-rod datum is a reconstructed vacuum-map datum with its supplied ordered rods satisfying all the conditions below. Write $\Phi=(u,v)$, $e(u,v)=|\nabla u|^2+e^{4u}|\nabla v|^2$ and $e'(U,v)=|\nabla U|^2+e^{4u}|\nabla v|^2$. Locally integrable means integrable on every compact subset of the specified neighborhood, with Euclidean volume. In the trace conditions below, use a continuous extension of $v$ to each compact subinterval of the indicated open axis rod, equal there to $c_j$; the source provides such representatives in Proposition 2.1(i).

(V) Require local minimality of renormalized energy under competitors preserving the specified singularity data and rod traces, in the variational class of HKWX §2.1. Adopt this source hypothesis independently of the harmonic-map equations; no implication from those equations alone is asserted here.

(A1a) Near each compact subinterval $I$ of an open axis rod, $U,v$ are bounded, $e'(U,v)$ is integrable on a neighborhood of $I$, and $v=c_j$ in trace on $I$.

(A1b) Near every compact subinterval inside a nondegenerate horizon rod, $u,v$ are bounded and $e(u,v)$ is integrable.

(A1c) At the lower and upper pole of a nondegenerate rod, respectively put $\zeta=z-z_i^\pm$ and $r=\sqrt{\rho^2+\zeta^2}$. The renormalized functions are $\widehat U_i^-=U-\tfrac12\log(r-\zeta)$ and $\widehat U_i^+=U-\tfrac12\log(r+\zeta)$. Require $\widehat U_i^\pm,v$ bounded and $|\nabla\widehat U_i^\pm|^2+e^{4u}|\nabla v|^2$ integrable near the pole.

(A2) At each degenerate puncture use centered polar coordinates $(r_i,\theta_i,\phi)$. For some $\epsilon_i,\Lambda_i>0$, require $|u+\log\sin\theta_i|\le\Lambda_i$ off the axis in $B_{\epsilon_i}(p_i)$ and $e'(U,v)$ locally integrable on $B_{\epsilon_i}(p_i)\setminus\{p_i\}$. The adjacent axis traces are $c_i,c_{i+1}$ and satisfy $c_{i+1}-c_i=4\mathcal J_i\ne0$.

(A3) Outside a sufficiently large ball, $U,v$ are bounded, $e'(U,v)$ is locally integrable including across the ordinary axis, $v$ has traces $c_1,c_{N+1}$ on the two semi-infinite rods, and $U\to0$ at infinity. These are explicit input conditions; calling a spacetime regular does not, by this definition alone, verify them.

(H) For every compact subinterval $I\subset\operatorname{Int}\mathcal H_i$ of a nondegenerate rod, $u,v$ extend smoothly and axisymmetrically to a neighborhood of $I$ in $\mathbb R^3$. For a real constant $\kappa_i$ common to that rod, require $\alpha=\log\rho+2u+\kappa_i+O(\rho^2)$, uniformly near each such $I$. Here $O(\rho^2)$ means that the remainder has absolute value at most $C_I\rho^2$ on a sufficiently small neighborhood off the axis. This specifies the horizon-interior behavior using Proposition 2.1(iii), equation (2.23).

## Definition references

[[def-author-abbd1939ec07-ordered-vacuum-rods]]

[[def-author-abbd1939ec07-reconstructed-harmonic-map-data]]

## Facts & Assumptions

[F1] All functions, rods, reconstruction equations and normalizations are [[def-author-abbd1939ec07-ordered-vacuum-rods]] and [[def-author-abbd1939ec07-reconstructed-harmonic-map-data]].

[F2] The source contract below supplies (V), (A1)–(A3), the continuous axis representative, and (H). The local-minimization premise is retained explicitly: (A1)–(A3) alone are not advertised as the full source framework. These are mathematical conditions on supplied functions, not physical regularity postulates or a theorem placing generic spacetimes in the class.

## Justification

**Given:** The reconstructed functions, neighborhoods and finite rod labels in [F1], with the independently adopted source predicates in [F2].

**Goal:** Check the elementary renormalizations and interval cases, while retaining the imported variational and boundary requirements as inputs.

1.1 All logarithms are evaluated where their arguments are positive off the axis. Indeed $r>|\zeta|$ there, and $\sin\theta_i>0$. Each displayed renormalization therefore defines a smooth function on the punctured off-axis domain; its boundedness and the specified energy integrals are definite scalar conditions. [given, F1, algebra]

2.1 The interval classification determines which conditions apply: poles and interior-rod conditions apply only to strict intervals, and puncture conditions only to singletons. The trace constants and nonzero differences are finite numerical requirements. The horizon condition specifies smooth extensions and an explicit uniform remainder bound on each compact interior interval. Conjoin these scalar and extension requirements with the separately adopted variational predicate [F2]; none is proved merely by naming a horizon regular. This checks the elementary formulation and does not prove existence, local minimality, or geometric spacetime membership. [given, F1, F2, step 1.1] ∎

## External input

HKWX §2.1 supplies the variational predicate (V) and the boundary/energy conditions (A1)–(A3). Proposition 2.1(i),(iii) supplies the axis representative and the explicit horizon-interior regularity used above, under the full §2.1 hypotheses. These premises are imported; the Justification checks only the local formulation.

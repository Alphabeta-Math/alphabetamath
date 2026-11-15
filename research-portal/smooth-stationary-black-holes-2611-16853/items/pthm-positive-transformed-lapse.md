---
id: pthm-positive-transformed-lapse
title: Transformed lapse equation and bounds
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
proof_strategy: direct
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-stationary-maximal-graph
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-lorentzian-data
  - def-harrison-normalization
  - def-stationary-asymptotic-decay-data
  - pthm-harrison-electrovacuum
  - pthm-global-harrison-one-form
  - pthm-harrison-coordinate-components
  - def-harrison-one-form-family
  - def-harrison-one-form
  - pthm-bifurcate-horizon-preservation
  - pthm-electrovacuum-energy-conditions
  - thm-maximal-jacobi-lapse-input
  - lem-exterior-lapse-maximum-and-boundary-control
  - def-exterior-weighted-elliptic-data
  - math:def-axiom-of-choice
  - math:cor-inverse-matrix-by-adjugate
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  pthm-harrison-electrovacuum: physical-result
  pthm-global-harrison-one-form: physical-result
  pthm-harrison-coordinate-components: physical-result
  def-harrison-one-form-family: mathematical-premise
  def-harrison-one-form: mathematical-premise
  pthm-bifurcate-horizon-preservation: physical-result
  pthm-electrovacuum-energy-conditions: physical-result
  thm-maximal-jacobi-lapse-input: mathematical-premise
  lem-exterior-lapse-maximum-and-boundary-control: mathematical-premise
  def-exterior-weighted-elliptic-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:cor-inverse-matrix-by-adjugate: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pages 13–14, equations (3.3)–(3.4)
      statement: The transformed maximal-section lapse satisfies the displayed
        equation, zero boundary value and positive end limit, and is positive
        and bounded above by that limit.
      hypotheses: The article's regular mass-one stationary vacuum construction and
        the smooth maximal sections with the stated boundary and asymptotic
        behavior.
      reading_limits: Read the frozen article text at the cited passage. This citation
        attributes the claim; the proof below uses the declared suppliers and
        the stated section hypotheses.
physical_scope: Conditional geometric deductions in the classical stationary
  vacuum model and its source-free Einstein–Maxwell Harrison family; no
  observation is asserted.
dependency_level: 11
---

## Statement

Adopt the regular stationary vacuum construction, with original exterior section maximal, $T|_S\not\equiv0$, mass one, and the supplied Harrison family. Assume the Axiom of Choice. Fix $q\in(0,1]$ and a supplied connected smooth spacelike maximal section $\Sigma_q$ with compact boundary $S$ and one exterior end. Its interior lies in the stationary exterior, and it is smooth up to $S$. In the normalized end coordinates $t_q=d_qt/(4q)$ and $x_q=qx$, suppose that sufficiently far out the section is the graph $t_q=\widetilde u_q(x_q)$ and that $\partial_i\widetilde u_q\to0$ uniformly as $r_q=|x_q|\to\infty$. Take the future unit normal $n_q$ agreeing at infinity with the future direction of $T$.

Here one exterior end means the compact-core exterior convention: for some $R_q>0$ there is a compact subset $C_q\subset\Sigma_q$ whose complement is identified by the stated graph and its spatial chart $x_q$ with $\{x_q\in\mathbb R^3:|x_q|>R_q\}$, and $K_q=\Sigma_q\setminus\{r_q>2R_q\}$ is compact. These are topological hypotheses on the supplied section, not consequences of graph-height or graph-slope decay.

Let $h_q$ be the induced metric, $k_q(U,V)=-g_q(\nabla^q_U n_q,V)$, and $N_q=-g_q(T,n_q)$. Then $\Delta_{h_q}N_q=(|k_q|_{h_q}^2+\operatorname{Ric}(g_q)(n_q,n_q))N_q$, $N_q|_S=0$, and $N_q\to d_q/(4q)$ uniformly at infinity. Moreover $0<N_q\le d_q/(4q)$ in the interior, so $T$ is transverse to $\Sigma_q$ there.

The original-section maximality used here is assumed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$, with the original metric $g$, so $H_g|_C=0$. The selected physical end retains its stated mass-one normalization. Maximality of an independently labelled chart-side section or another supplied maximal section does not replace this premise. No equality between the hypersurface identification and the physical stationary end chart is assumed. [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

## Facts & Assumptions

**Given:** The construction, parameter and candidate section in the Statement. In particular, existence of the candidate is assumed, not deduced.

**Goal:** Establish the lapse equation, its boundary and end values, the bounds and transversality.

[A1] The original model and regularity data include the stationary Killing field $T$, the two transverse horizon branches through $S$, and tangency of $T$ to both branches. The Harrison normalization defines $d_q$ at the chosen zero of $T$, and the graph and decay conventions specify the normalized end coordinates. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-harrison-normalization]] [[def-stationary-maximal-graph]] [[def-stationary-asymptotic-decay-data]]

[A2] Work with the Axiom of Choice, including the choice uses inherited by the maximum-principle supplier. [[math:def-axiom-of-choice]]

[A3] The supplied section has the compact-core exterior structure stated above, with end chart $x_q$ and compact $K_q$. This is the exterior-domain convention needed for the maximum-principle application; no weighted norm or weighted elliptic estimate is assumed here. [[def-exterior-weighted-elliptic-data]]

[F1] The Harrison construction gives the smooth stationary transformed metric and source-free Einstein–Maxwell fields; the horizon-preservation result supplies a smooth transformed geometry near $S$. [[pthm-harrison-electrovacuum]] [[pthm-bifurcate-horizon-preservation]]

[F2] A spacelike section has positive-definite induced metric and a future unit normal; maximality means zero mean curvature. The stationary lapse equation holds for a Killing field on such a maximal section with the displayed conventions. [[def-spacelike-maximal-hypersurface-data]] [[def-stationary-lorentzian-data]] [[thm-maximal-jacobi-lapse-input]]

[F3] The single smooth stationary primitive $W_0$ selected by the electrovacuum construction has spatial components $(W_0)_i=O_5(r^{-3})$ in the original end chart. This is the global primitive used for the metric in [F1]; equality with the exact radial integral is not asserted or required. [[pthm-global-harrison-one-form]] [[pthm-harrison-electrovacuum]] The energy-condition result gives $|k_q|_{h_q}^2+\operatorname{Ric}(g_q)(n_q,n_q)\ge0$. [[pthm-electrovacuum-energy-conditions]]

[F4] On a connected smooth Riemannian exterior with compact smooth boundary, a smooth solution of $(\Delta_h-V)u=0$ with $V\ge0$, zero boundary value and uniform positive end limit $c$ obeys $0<u\le c$ in the interior. [[lem-exterior-lapse-maximum-and-boundary-control]]

[F5] For this same primitive, $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. The original stationary end has $T=\partial_t$, $f=-g(T,T)\to1$, $g_{0i}=O_6(r^{-2})$ and $g_{ij}\to\delta_{ij}$ uniformly in angle. The normalized potential obeys $\sigma=f+i\psi\to1$, with $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $d_q=D_q(p)$ at the chosen zero $p$ of $T$. [[def-harrison-one-form-family]] [[def-regular-stationary-vacuum-spacetime]] [[def-stationary-lorentzian-data]] [[def-stationary-asymptotic-decay-data]] [[def-harrison-normalization]]

[F6] The family in [F1] satisfies the Harrison one-form conditions, including $W_q(T)=d_q-D_q$, and its metric is the metric of that definition on $D_q>0$. In an original stationary chart its components are $(g_q)_{00}=-d_q^2f/(4D_q)$, $(g_q)_{0i}=(d_q/4)(g_{0i}-f(W_q)_i/D_q)$, and $(g_q)_{ij}=(D_qg_{ij}+g_{0i}(W_q)_j+g_{0j}(W_q)_i-f(W_q)_i(W_q)_j/D_q)/4$. These identities require no radial choice of the primitive. [[def-harrison-one-form]] [[pthm-harrison-coordinate-components]] [[pthm-harrison-electrovacuum]]

[F7] For a real square matrix with nonzero determinant, its inverse is its adjugate divided by its determinant. Each cofactor and the determinant are polynomials in the matrix entries. [[math:cor-inverse-matrix-by-adjugate]]

## Proof

**Given:** The construction, parameter and candidate section in the Statement. In particular, existence of the candidate is assumed, not deduced.

1.1 The transformed metric is stationary and smooth, and the supplied section is spacelike and maximal. Applying the stationary lapse equation with its future normal gives $\Delta_{h_q}N_q=(|k_q|_{h_q}^2+\operatorname{Ric}(g_q)(n_q,n_q))N_q$. The potential is nonnegative by the transformed energy-condition result. [given, F1, F2, F3]

1.2 At $S$, tangency of $T$ to both transverse horizon branches implies $T\in TS$. Since $S$ is the boundary of $\Sigma_q$, $TS\subset T\Sigma_q$, and the unit normal is orthogonal to it. Smoothness up to $S$ therefore gives $N_q|_S=0$. [A1, F1, F2, given]

1.3 Fix the stated $q>0$. The decay in [F3] and the family formula in [F5] give $(W_q)_i=O_q(r^{-2})$. Since $\sigma\to1$, the normalization in [F5] gives $D_q\to4q^2>0$ uniformly in angle. At $p$, $f(p)=-g(T_p,T_p)=0$, so expanding the squared modulus gives $d_q=(1+q)^2+(1-q)^2\psi(p)^2>0$. The original maximal section, mass-one normalization, smooth Harrison one-form, positive denominator and stationary chart required by [F6] are supplied by the Statement and [F1], [F5]. Substituting $f\to1$, $g_{0i}\to0$, $g_{ij}\to\delta_{ij}$ and $(W_q)_i\to0$ into its component identities yields $(g_q)_{00}\to-d_q^2/(16q^2)$, $(g_q)_{0i}\to0$ and $(g_q)_{ij}\to q^2\delta_{ij}$ in the original coordinates. Under $dt=(4q/d_q)dt_q$ and $dx^i=dx_q^i/q$, evaluating the metric on the rescaled coordinate vectors gives $(g_q)_{00}\to-1$, $(g_q)_{0i}\to0$ and $(g_q)_{ij}\to\delta_{ij}$ in normalized coordinates. Since $r_q=qr$ with $q$ fixed, all these limits are uniform in angle as $r_q\to\infty$. This calculation uses the same global family as the lapse equation and energy condition, without assuming a radial gauge. [given, A1, F1, F3, F5, F6, algebra]

2.1 On the end let $\tau=t_q-\widetilde u_q(x_q)$. The future unit normal has metric dual $-d\tau/\sqrt{-g_q^{-1}(d\tau,d\tau)}$. The inverse metric converges uniformly to the inverse Minkowski metric, while $\partial_i\widetilde u_q\to0$ uniformly. The inverse-metric convergence follows from step 1.3 by the cofactor formula: each inverse entry is a polynomial cofactor divided by the determinant, which tends uniformly to the nonzero Minkowski determinant. Thus the denominator tends to $1$. Since $T=(d_q/(4q))\partial_{t_q}$, it follows that $N_q=d_q/(4q\sqrt{-g_q^{-1}(d\tau,d\tau)})\to d_q/(4q)>0$ uniformly. [A1, F2, F5, F7, step 1.3, given, algebra]

3.1 The induced metric is Riemannian and the potential is smooth and nonnegative. By [A3], the supplied connected section has compact smooth boundary and the compact-core exterior structure in the maximum-principle supplier: every escape from compact subsets away from the boundary eventually lies in the end chart with $r_q\to\infty$. Smoothness up to $S$ supplies the required boundary regularity of $N_q$, and step 2.1 supplies its uniform positive limit on that entire end. Applying the exterior maximum principle to steps 1.1, 1.2 and 2.1 gives $0<N_q\le d_q/(4q)$ in the interior. If $T$ were tangent to the section at an interior point, its contraction with $n_q$ would vanish there, contradicting positivity. Hence $T$ is transverse. [A3, F2, F4, step 1.1, step 1.2, step 2.1] ∎

## Source notes

The article reference attributes equations (3.3)–(3.4). The proof uses the supplied lapse, energy and maximum-principle results. The differentiated end condition is stated explicitly because convergence of graph height alone does not provide the normal's asymptotic behavior.

The normalized end limits needed here are proved directly in step 1.3 for the smooth global primitive selected by the electrovacuum construction. The radial-choice transformed-end theorem is not invoked; its stronger end conclusions are not needed for this fixed-$q$ lapse result.

These explicit premises specify the generated conditional result. They are not asserted to follow from the original regularity definition alone, and are not attributed to the original article. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.

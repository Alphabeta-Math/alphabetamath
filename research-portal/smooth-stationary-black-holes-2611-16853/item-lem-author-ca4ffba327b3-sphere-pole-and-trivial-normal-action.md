---
title: A circle action on a sphere has a pole with trivial normal action
status: draft
research_item: lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action
dependency_level: 1
---

## Prerequisites

- [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)
- [math:thm-a-sphere-has-a-nowhere-zero-tangent-vector-field-iff-its-dimension-is-odd](https://alphabetamath.cc/item/thm-a-sphere-has-a-nowhere-zero-tangent-vector-field-iff-its-dimension-is-odd)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves](https://alphabetamath.cc/item/thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves)
- [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)
- [math:thm-coordinate-formula-for-the-differential](https://alphabetamath.cc/item/thm-coordinate-formula-for-the-differential)
- [math:thm-clairaut-schwarz-mixed-partials](https://alphabetamath.cc/item/thm-clairaut-schwarz-mixed-partials)
- [math:lem-extreme-value-theorem-from-compactness](https://alphabetamath.cc/item/lem-extreme-value-theorem-from-compactness)
- [math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)


## Statement

Let a smooth time-oriented circle action by isometries preserve an embedded spacelike two-sphere $S$, with generator $Z$. Then $Z$ has a zero $p\in S$, and the full circle fixes $p$. At such a point its differential acts as the identity on the Lorentzian normal plane $(T_pS)^\perp$. In particular $\nabla_vZ=0$ for all normal vectors $v$ at $p$. If a field $K=T+\Omega Z$ vanishes on $S$, with constant $\Omega$, then $T(p)=0$ at the same pole.

## Statement references

[def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[math:thm-a-sphere-has-a-nowhere-zero-tangent-vector-field-iff-its-dimension-is-odd](https://alphabetamath.cc/item/thm-a-sphere-has-a-nowhere-zero-tangent-vector-field-iff-its-dimension-is-odd)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves](https://alphabetamath.cc/item/thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves)

[math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[math:thm-coordinate-formula-for-the-differential](https://alphabetamath.cc/item/thm-coordinate-formula-for-the-differential)

[math:thm-clairaut-schwarz-mixed-partials](https://alphabetamath.cc/item/thm-clairaut-schwarz-mixed-partials)

[math:lem-extreme-value-theorem-from-compactness](https://alphabetamath.cc/item/lem-extreme-value-theorem-from-compactness)

[math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)

## Facts & Assumptions

[F1] Work in the ZFC convention inherited from the Lorentzian and circle-action data; the choice assumption is inherited through that manifold framework. The finite-dimensional projection below needs no further choice principle. [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F2] A continuous tangent field on the standard two-sphere has a zero. The differential chain rule transfers this assertion through a smooth identification of the embedded sphere with the standard sphere. [math:thm-a-sphere-has-a-nowhere-zero-tangent-vector-field-iff-its-dimension-is-odd](https://alphabetamath.cc/item/thm-a-sphere-has-a-nowhere-zero-tangent-vector-field-iff-its-dimension-is-odd) [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[F3] Use the normal-data Definition's Lorentzian data $(M,g,N)$ of signature $(-,+,+,+)$, and its generator, invariant-submanifold and normal-field conventions. For the arbitrary circle action in this lemma, write $\phi_t$ for its smooth global flow with $\phi_{t+2\pi}=\phi_t$ and $\phi_t^*g=g$. No least-positive-period condition is assumed: the action may be ineffective or trivial. We use those conventions, not the supplier's averaging assertion for normalized actions. [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F4] A smooth vector field has unique integral curves on a sufficiently small common interval about a prescribed initial point. The global-flow law then allows iteration of a sufficiently small time step. [math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves](https://alphabetamath.cc/item/thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F5] Differentials obey the chain rule and are represented by coordinate Jacobians. The continuous mixed second partials of a smooth coordinate representative commute. [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps) [math:thm-coordinate-formula-for-the-differential](https://alphabetamath.cc/item/thm-coordinate-formula-for-the-differential) [math:thm-clairaut-schwarz-mixed-partials](https://alphabetamath.cc/item/thm-clairaut-schwarz-mixed-partials)

[F6] The metric-selected connection satisfies the affine-connection rules, and its coordinate coefficients are defined by $\nabla_{\partial_b}\partial_c=\Gamma^a{}_{bc}\partial_a$. Applying its linearity and Leibniz rules to $Z=Z^a\partial_a$ gives $(\nabla_vZ)^a=v^b\partial_bZ^a+v^b\Gamma^a{}_{bc}Z^c$; hence at a zero of $Z$ this is its ordinary coordinate derivative. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F7] A continuous real-valued function on a closed bounded real interval attains its maximum and minimum. We apply this to the positive scalar coefficient of the normal representation on $[0,2\pi]$. [math:lem-extreme-value-theorem-from-compactness](https://alphabetamath.cc/item/lem-extreme-value-theorem-from-compactness)

[F8] A continuous real-valued function on a closed real interval takes every value between its endpoint values. Consequently a continuous nonzero scalar cannot change sign, and a continuous function taking values only in $\{1,-1\}$ is constant on every interval. [math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)

## Proof

**Given:** The data and hypotheses in the Statement, with the inherited ZFC convention of [F1].

**Goal:** Establish the stated conclusions.

1.1 Invariance of $S$ makes $Z|_S$ tangent: the curve $t\mapsto\phi_t(q)$ lies in $S$ for $q\in S$. If $f:S^2\to S$ is a smooth identification, the field $x\mapsto d(f^{-1})_{f(x)}Z_{f(x)}$ is smooth and tangent to $S^2$; the chain rule makes $df$ invertible, so [F2] gives a point $p\in S$ with $Z(p)=0$. Both $t\mapsto\phi_t(p)$ and the constant curve at $p$ are integral curves with initial value $p$. By [F4] they agree for $|t|<h$ for some $h>0$. For arbitrary $t\in\mathbb R$, choose a positive integer $m$ with $|t|/m<h$; the flow law gives $\phi_t(p)=(\phi_{t/m})^m(p)=p$. Thus the full circle fixes $p$. [F1, F2, F3, F4]

1.2 Construct a smooth future timelike normal field along all of $S$. For each $q\in S$, the positive-definite restriction of $g_q$ to $T_qS$ gives a unique orthogonal projection $P_q:T_qM\to T_qS$. In a local tangent frame $X_1,X_2$, with $G_{ij}=g(X_i,X_j)$ and inverse matrix $(G^{ij})$, it is $P_qN_q=\sum_{i,j=1}^2G^{ij}g(N_q,X_j)X_i$. The matrix is smoothly invertible, so these expressions are smooth; uniqueness of the projection makes them agree on overlaps. Put $u_q=N_q-P_qN_q$. Then $u_q\perp T_qS$ and $g(u_q,u_q)=g(N_q,N_q)-g(P_qN_q,P_qN_q)<0$, while $g(u_q,N_q)=g(u_q,u_q)<0$. Thus $u$ is a smooth future timelike normal field along $S$, in the normal-field convention of [F3]. Moreover $T_qM=T_qS\oplus(T_qS)^\perp$: nondegeneracy of the tangent restriction gives this direct sum, and a vector in the radical of the normal restriction would be orthogonal to all of $T_qM$, hence zero. The normal plane has dimension two, contains the timelike vector $u_q$, and has only one negative direction because the ambient metric does. Its signature is therefore $(-,+)$. [F1, F3, algebra, construct]

2.1 Set $W=(T_pS)^\perp$, $n=u_p/\sqrt{-g(u_p,u_p)}$ and $A_t=d\phi_t|_p$. Isometry and invariance of $S$ imply that $A_t$ preserves $W$. The fixed-point property and chain rule give $A_{s+t}=A_sA_t$, $A_0=\operatorname{id}$ and $A_{t+2\pi}=A_t$; the coordinate formula makes this a smooth family. Inside the Lorentzian plane $W$, the line $L=W\cap n^\perp$ is spacelike: nondegeneracy splits $W=\mathbb Rn\oplus L$, and the single negative direction is already $n$. Choose a unit $e\in L$ and put $k_+=n+e$, $k_-=n-e$. For either sign write $A_tk_\pm=\alpha_\pm(t)n+\beta_\pm(t)e$. This vector is nonzero and null, so $\beta_\pm(t)^2=\alpha_\pm(t)^2$ and $\alpha_\pm(t)\ne0$. Since $\alpha_\pm(0)=1$, [F8] on the interval between $0$ and $t$ gives $\alpha_\pm(t)>0$. The continuous ratio $\beta_\pm/\alpha_\pm$ takes values in $\{1,-1\}$ and has initial value $\pm1$, so [F8] makes it identically $\pm1$. Thus $A_tk_+=a(t)k_+$ and $A_tk_-=b(t)k_-$ for positive continuous scalars $a,b$. Since $g(k_+,k_-)=-2$, isometry gives $a(t)b(t)=1$; the representation law gives $a(s+t)=a(s)a(t)$. [F3, F5, F8, step 1.1, step 1.2, algebra, construct]

3.1 By [F7], the positive continuous $2\pi$-periodic function $a$ attains a maximum $B=a(r)>0$ on $[0,2\pi]$. Periodicity makes $B$ an upper bound on all of $\mathbb R$, by reducing any real argument modulo $2\pi$. For every $t$, the identity $a(r+t)=a(r)a(t)$ therefore gives $Ba(t)\le B$, hence $a(t)\le1$. Applying the same inequality to $-t$ and using $a(t)a(-t)=a(0)=1$ gives $a(t)\ge1$. Thus $a(t)=b(t)=1$ for every $t$, and the basis $(k_+,k_-)$ of $W$ is fixed. Consequently $A_t|_W=\operatorname{id}_W$. This uses only that $2\pi$ is a common period, and covers ineffective and trivial actions without rescaling the generator. [F7, step 2.1, algebra]

4.1 Choose one chart $x$ near the fixed point and write $F(t,y)=x(\phi_t(x^{-1}(y)))$ for small $t$ and $y$ near $x(p)$. This is smooth on an open neighborhood of $(0,x(p))$; $F(t,x(p))=x(p)$ makes the coordinate basis at the image independent of $t$. By [F5], $A_t$ is represented by $D_yF(t,x(p))$ and $Z^a(y)=\partial_tF^a(0,y)$. Commuting the mixed derivatives gives $\left.\partial_t\right|_{t=0}D_yF(t,x(p))v=D_yZ(x(p))v$. For $v\in W$ the left side vanishes by step 3.1. At $p$ the connection term in [F6] is zero because $Z(p)=0$, so $\nabla_vZ=0$ for all $v\in W$. [F5, F6, step 1.1, step 3.1]

5.1 Finally, if $K=T+\Omega Z$ vanishes on $S$, evaluate this identity at the pole: $0=K(p)=T(p)+\Omega Z(p)=T(p)$ by step 1.1. This proves every stated conclusion. [given, step 1.1, step 4.1, algebra] ∎

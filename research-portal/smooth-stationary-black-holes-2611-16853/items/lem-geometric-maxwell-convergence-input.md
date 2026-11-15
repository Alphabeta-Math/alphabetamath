---
id: lem-geometric-maxwell-convergence-input
title: Maxwell algebra supplies timelike and null convergence
kind: lemma
status: published
origin: pipeline
domain: mathematics
proof_strategy: direct
deps:
  - def-source-free-geometric-electrovacuum-data
  - def-null-screen-expansion-and-focal-data
  - physics:def-emg-matter-formal-systems
  - physics:def-emg-pointwise-energy-conditions
  - physics:thm-emg-selected-matter-energy-conditions
  - math:def-axiom-of-choice
  - math:thm-sylvesters-law-of-inertia
dependency_roles:
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  physics:def-emg-matter-formal-systems: mathematical-premise
  physics:def-emg-pointwise-energy-conditions: mathematical-premise
  physics:thm-emg-selected-matter-energy-conditions: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-sylvesters-law-of-inertia: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
dependency_level: 1
---

## Statement

Assume the Axiom of Choice and let $(M,g,N,o,F)$ be a source-free geometric electrovacuum datum with zero cosmological constant. Put $Q_{ab}=F_{ac}F_b{}^c-\frac14g_{ab}F_{cd}F^{cd}$. Then $Q$ is symmetric and trace-free and obeys the dominant and strong energy conditions: for every future timelike $v$, $-Q^a{}_bv^b$ is future causal or zero, and $(Q_{ab}-\frac12(g^{cd}Q_{cd})g_{ab})v^av^b\ge0$. Consequently $\operatorname{Ric}(n,n)\ge0$ for every unit timelike $n$, and $\operatorname{Ric}(L,L)\ge0$ for every nonzero null $L$.

For such an $L$, its screen is $L^\perp/\mathbb RL$ with the positive quotient metric. If $e_1,e_2\in L^\perp$ represent an orthonormal screen basis, then $\operatorname{Ric}(L,L)=2\sum_{A=1}^2F(L,e_A)^2$. The right side is independent of the representatives. These are conditional tensor identities and inequalities, without a physical interpretation of $F$.

## Facts & Assumptions

**Given:** A datum and vectors as in the Statement.

**Goal:** Establish the energy conditions, both convergence inequalities and the screen formula.

[A1] The Axiom of Choice includes the choice assumptions in the geometric suppliers. [[math:def-axiom-of-choice]]

[F1] The datum has a smooth Lorentzian metric of signature $(-,+,+,+)$, a smooth real two-form $F$, and $\operatorname{Ric}=2Q$. [[def-source-free-geometric-electrovacuum-data]]

[F2] For positive formal parameters, the formal Maxwell tensor satisfies $T^{\mathrm{EM}}_{ab}=\mu_0^{-1}Q_{ab}$. [[physics:def-emg-matter-formal-systems]]

[F3] The formal Maxwell tensor is symmetric and trace-free and satisfies the dominant, strong and null energy conditions. [[physics:thm-emg-selected-matter-energy-conditions]]

[F4] The dominant condition means that the raised negative energy current of every future timelike vector is future causal or zero; the strong condition is nonnegativity on future timelike vectors of the trace-reversed tensor, and the null condition is nonnegativity on future null vectors. [[physics:def-emg-pointwise-energy-conditions]]

[F5] For a supplied null geodesic congruence normal to a spacelike two-surface, the screen is $L^\perp/\mathbb RL$ with metric induced by $g$. This supplies the screen convention in that setting; the pointwise extension to arbitrary nonzero null vectors is proved below. [[def-null-screen-expansion-and-focal-data]]

[F6] Every symmetric bilinear form on a finite-dimensional real vector space admits a diagonal basis with entries $1,-1,0$, and their respective counts are independent of the basis. [[math:thm-sylvesters-law-of-inertia]]

## Proof

**Given:**A datum and vectors as in the Statement.

**Goal:** Establish the energy conditions, both convergence inequalities and the screen formula.

[A1] The Axiom of Choice includes the choice assumptions in the geometric suppliers. [[math:def-axiom-of-choice]]

[F1] The datum has a smooth Lorentzian metric of signature $(-,+,+,+)$, a smooth real two-form $F$, and $\operatorname{Ric}=2Q$. [[def-source-free-geometric-electrovacuum-data]]

[F2] For positive formal parameters, the formal Maxwell tensor satisfies $T^{\mathrm{EM}}_{ab}=\mu_0^{-1}Q_{ab}$. [[physics:def-emg-matter-formal-systems]]

[F3] The formal Maxwell tensor is symmetric and trace-free and satisfies the dominant, strong and null energy conditions. [[physics:thm-emg-selected-matter-energy-conditions]]

[F4] The dominant condition means that the raised negative energy current of every future timelike vector is future causal or zero; the strong condition is nonnegativity on future timelike vectors of the trace-reversed tensor, and the null condition is nonnegativity on future null vectors. [[physics:def-emg-pointwise-energy-conditions]]

[F5] For a supplied null geodesic congruence normal to a spacelike two-surface, the screen is $L^\perp/\mathbb RL$ with metric induced by $g$. This supplies the screen convention in that setting; the pointwise extension to arbitrary nonzero null vectors is proved below. [[def-null-screen-expansion-and-focal-data]]

[F6] Every symmetric bilinear form on a finite-dimensional real vector space admits a diagonal basis with entries $1,-1,0$, and their respective counts are independent of the basis. [[math:thm-sylvesters-law-of-inertia]]



1.1 The assumed Axiom of Choice supplies the inherited choice hypotheses when applying [F1], [F2] and [F3]. Choose the formal positive parameters in [F2], for example $\mu_0=c=G_N=1$, and use the same smooth two-form and metric as in [F1]. The smooth field has the regularity required by [F2] and [F3]. Lowering the indices in the formal tensor formula gives $Q=\mu_0T^{\mathrm{EM}}$. Thus $Q$ is symmetric and trace-free. Since multiplication by $\mu_0>0$ preserves nonnegativity and the future causal cone, [F3] and [F4] give the stated dominant and strong conditions for $Q$, as well as $Q(L,L)\ge0$ for future null $L$. [A1, F1, F2, F3, F4, choose, algebra]

1.2 Work at a point, with $V=T_pM$. Normalize the supplied timelike vector to $n=N/\sqrt{-g(N,N)}$. The decomposition $v=-g(v,n)n+(v+g(v,n)n)$ gives $V=\mathbb Rn\oplus n^\perp$ as an orthogonal direct sum. Diagonalize $g|_{n^\perp}$ by [F6] and append $n$; uniqueness of the inertia counts, with the signature in [F1], makes $g|_{n^\perp}$ positive definite. A nonzero null $L$ therefore cannot be orthogonal to $N$, so $a=g(N,L)\ne0$. Put $K=-2N/a+g(N,N)L/a^2$; direct substitution gives $g(K,L)=-2$ and $g(K,K)=0$. [F1, F6, given, construct, algebra]

2.1 Let $P=\operatorname{span}\{L,K\}$ and $E=P^\perp$. The Gram matrix on $P$ is $\left(\begin{smallmatrix}0&-2\\-2&0\end{smallmatrix}\right)$; the vectors $L+K$ and $L-K$ are orthogonal with squared norms $-4$ and $4$. For any $v\in V$, the vector $v+\frac12g(v,K)L+\frac12g(v,L)K$ belongs to $E$. This gives the orthogonal direct sum $V=P\oplus E$, since a vector $bL+cK$ orthogonal to both $L$ and $K$ has $b=c=0$. Thus $E$ has dimension two. Diagonalizing $g|_E$ by [F6] and adjoining the displayed diagonal basis of $P$, uniqueness of inertia and the signature of $g$ show that $g|_E$ has two positive directions and no negative or zero directions. In particular it is positive definite. If $v\in L^\perp$, its $K$ coefficient in this decomposition vanishes, so $L^\perp=\mathbb RL\oplus E$. The form $\bar\gamma([v],[w])=g(v,w)$ is well-defined on $L^\perp/\mathbb RL$, since adding multiples of $L$ to either representative leaves it unchanged. The map $E\to L^\perp/\mathbb RL$, $e\mapsto[e]$, is consequently a linear isometry and bijection. This proves the positive two-dimensional screen assertion for every nonzero null $L$ without any congruence hypothesis. [F1, F6, step 1.2, construct, algebra]

2.2 By trace-freeness, the strong condition gives $Q(v,v)\ge0$ for future timelike $v$. A past timelike or null vector changes to a future vector under negation, while its quadratic contraction is unchanged. Hence $\operatorname{Ric}(n,n)=2Q(n,n)\ge0$ for every unit timelike $n$ and $\operatorname{Ric}(L,L)=2Q(L,L)\ge0$ for every nonzero null $L$. [F1, F4, step 1.1, algebra]

3.1 By [F6], the positive form on $E$ has an orthonormal basis, hence so does the screen by step 2.1. Given any representatives $e_1,e_2$ of an orthonormal screen basis, replace each $e_A$ by $e_A+\frac12g(e_A,K)L$. The replacements preserve the classes and lie in $E$, so are an orthonormal basis of $E$. For these representatives the basis $L,K,e_1,e_2$ therefore has inverse metric $g^{-1}=-\frac12(L\otimes K+K\otimes L)+\sum_Ae_A\otimes e_A$. [F6, step 1.2, step 2.1, construct, algebra]

4.1 Since $F(L,L)=0$, contraction of the inverse metric in step 3.1 gives $F_{ac}L^aF_b{}^cL^b=\sum_AF(L,e_A)^2$. The trace term in $Q(L,L)$ vanishes because $g(L,L)=0$. Therefore $\operatorname{Ric}(L,L)=2\sum_AF(L,e_A)^2$. Replacing any representative by $e_A+tL$ leaves $F(L,e_A)$ unchanged by alternation, proving the claimed representative independence. [F1, step 3.1, algebra] ∎

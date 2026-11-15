---
id: lem-author-c92bdd91a36e-residual-jet-continuity
title: Harrison equation residuals are continuous functions of stationary two-jets
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-complex-self-dual-two-form-data
  - def-source-free-geometric-electrovacuum-data
  - def-harrison-one-form
  - def-harrison-electromagnetic-form
  - lem-author-c92bdd91a36e-stationary-local-jets
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  def-harrison-one-form: mathematical-premise
  def-harrison-electromagnetic-form: mathematical-premise
  lem-author-c92bdd91a36e-stationary-local-jets: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references: []
dependency_level: 4
---

## Statement

Fix an oriented stationary chart with $T=\partial_t$, a parameter $q\in[0,1]$, and stationary smooth fields $(g,\psi,W_0)$, where $g$ is Lorentzian, $\psi$ is real and $W_0$ is a real one-form. Stationary two-jets are the chartwise values and derivatives through order two, with all time derivatives zero. Put $T^\flat=g_{ta}\,\mathrm dx^a$, $f=-g_{tt}$, $\sigma=f+i\psi$, $B_q=q(1+\sigma)+(1-\sigma)$, $D_q=B_q\overline{B_q}$, $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, $F=\tfrac12\mathrm dT^\flat$ and $\mathcal F=F+i\star_gF$.

Define algebraic extensions of the spacetime Harrison formulas on the open jet domain $D_q>0$ and $D_q+W_q(T)>0$ by

$$g_q=\tfrac14\left(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q\right),\qquad F_q=\operatorname{Re}\left[-\sqrt{1-q^2}\,\frac{\overline{B_q}}{B_q}\left(\mathcal F+\frac{W_q\wedge\mathrm d\sigma}{2D_q}\right)\right].$$

The metric $g_q$ is Lorentzian there. With the specified orientation for both metrics, the three residual tensors

$$E_{ab}=\operatorname{Ric}(g_q)_{ab}-2\left((F_q)_{ac}(F_q)_b{}^c-\tfrac14(g_q)_{ab}(F_q)_{cd}(F_q)^{cd}\right),\qquad M=\mathrm dF_q,\qquad P=\mathrm d(\star_{g_q}F_q)$$

are continuous functions of the stationary two-jet of $(g,\psi,W_0)$ for fixed $q$; all indices in $E$ are raised with $g_q^{-1}$. This includes jets with $g_{tt}=0$ and uses no quotient metric or division by $f$.

These extensions agree with the Harrison metric and electromagnetic form wherever the normalized Ernst and Harrison one-form hypotheses hold. In such an application the normalization label is $d_0=D_0(p)$ at a supplied zero $T_p=0$ in the larger domain of the data; $p$ need not belong to the stationary chart. Holding $d_0$ fixed restricts the compatible jets and does not change the continuity assertion. Neither a zero $p$ nor the Ernst and primitive differential identities are required to evaluate the algebraic extensions on arbitrary jets in the stated open domain.

## Facts & Assumptions

[F1] The metric dual, Lorentzian inverse, Levi–Civita connection and Ricci conventions are supplied by [[def-stationary-lorentzian-data]]. Complex forms, the complex-linear Hodge map and fiberwise pullback use [[def-complex-self-dual-two-form-data]].

[F2] The comparison interfaces are [[def-harrison-one-form]] and [[def-harrison-electromagnetic-form]]. Their hypotheses include a supplied normalized Ernst potential with $\mathrm d\sigma=2\iota_T\mathcal F$, a supplied zero $T_p=0$, $d_q=D_q(p)$, and a stationary real one-form with $\mathrm dW_q=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$ and $W_q(T)=d_q-D_q$ on the domain $D_q>0$. These hypotheses are used only for comparison where satisfied, not assumed for arbitrary jets of the algebraic extensions.

[F3] The three residuals use exactly the geometric tensor equations and metric Hodge convention in [[def-source-free-geometric-electrovacuum-data]]; defining their residuals does not assert the equations.

[F4] The stationary coordinate components and their two-jets have the meaning in [[lem-author-c92bdd91a36e-stationary-local-jets]]. The smooth scalar and one-form here are explicitly stationary, as that supplier requires.

## Proof

**Given:** The stationary fields, fixed parameter, orientation and open jet domain in the Statement.

**Goal:** Prove Lorentzian well-definedness, continuity of the residuals on two-jets, and agreement on the compatible Harrison data.

1.1 Put $s_q=D_q+W_q(T)$ and $A_qv=v+D_q^{-1}W_q(v)T$. Since $D_q,s_q>0$, direct composition gives $A_q^{-1}v=v-s_q^{-1}W_q(v)T$. Expanding $g(A_qu,A_qv)$ and using $g(T,T)=-f$ gives exactly $g_q=(D_q/4)A_q^*g$. The invertible pullback preserves the Lorentzian signature, and the positive scalar preserves it as well. Both $A_q$ and $g_q$ depend smoothly on the zeroth-order entries; this conclusion uses no differential identity for $W_q$ or $\sigma$. [given, F1, F4, algebra]

2.1 In coordinates the inverse of a nondegenerate metric is its adjugate divided by its determinant. Its oriented volume density is $\sqrt{|\det g|}$, and the Hodge coefficients are contractions of that density, the fixed orientation symbol and inverse-metric entries. Hence these are smooth functions of the metric entries on the Lorentzian domain, for $g$ and for $g_q$ from step 1.1. The expression $F=\tfrac12\mathrm dT^\flat$ uses only first derivatives of $g$, and $\mathrm d\sigma$ uses only first derivatives of $g,\psi$. Since $B_q\ne0$ follows from $D_q>0$, the explicitly defined $F_q$ is a smooth function of these first-jet entries and the values of $W_0$. The factor $\sqrt{1-q^2}$ is a fixed real constant, including at $q=0,1$. No denominator here is $f$. [given, F1, F3, F4, step 1.1]

3.1 The coordinate connection coefficients of $g_q$ are $\Gamma^a_{bc}=\tfrac12(g_q)^{ad}(\partial_b(g_q)_{dc}+\partial_c(g_q)_{db}-\partial_d(g_q)_{bc})$; the Ricci components are sums of first derivatives of these coefficients and products of two such coefficients. They therefore depend smoothly on the metric two-jet. Applying the product and chain rules to the zeroth-order formula for $g_q$ and the first-order formula for $F_q$ shows that $E$ uses at most the input two-jet. Each exterior derivative in $M$ and $P$ uses one derivative of $F_q$ and, for $P$, one derivative of the Hodge coefficients of $g_q$, so also uses at most that two-jet. These formulas define smooth, hence continuous, functions on the finite-dimensional open domain of stationary two-jets, including at $g_{tt}=0$. A jet may be evaluated by these component formulas without being realized by a solution of any field equation. [F1, F3, F4, step 1.1, step 2.1]

4.1 On actual data satisfying [F2], the Killing equation and the torsion-free connection give $\nabla_aT_b=\tfrac12(\partial_aT_b-\partial_bT_a)$, so the two-form $F$ here is the Killing two-form in the comparison interfaces. The metric formula agrees term by term with [F2]. Expanding the alternating pullback gives $A_q^*\mathcal F=\mathcal F+D_q^{-1}W_q\wedge\iota_T\mathcal F$, since the term with two copies of $T$ vanishes. Now $\mathrm d\sigma=2\iota_T\mathcal F$ identifies the extended electromagnetic formula with the interface formula. Thus, wherever the interface hypotheses hold on an open set, the fields and their residuals agree there; the same component identification applies to compatible jets carrying the identities through the derivative orders used in step 3.1. The contraction identity gives $s_q=d_q>0$, while the label $d_0=D_0(p)$ does not enter any denominator or differential operation above. Restricting the continuous residual maps to any compatible jets with that label fixed preserves continuity. [given, F1, F2, F3, F4, step 1.1, step 2.1, step 3.1, algebra] ∎

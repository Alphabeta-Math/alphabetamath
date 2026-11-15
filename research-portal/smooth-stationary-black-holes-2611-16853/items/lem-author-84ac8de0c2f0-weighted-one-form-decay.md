---
id: lem-author-84ac8de0c2f0-weighted-one-form-decay
title: The differentiated spatial decay supplied by the Harrison lift
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-asymptotic-decay-data
  - lem-author-84ac8de0c2f0-end-denominator-bounds
  - def-harrison-one-form
  - thm-stationary-harrison-primitive-input
  - thm-harrison-electrovacuum-construction-input
  - math:lem-derivative-algebra-and-chain-rules
dependency_roles:
  def-stationary-asymptotic-decay-data: mathematical-premise
  lem-author-84ac8de0c2f0-end-denominator-bounds: mathematical-premise
  def-harrison-one-form: mathematical-premise
  thm-stationary-harrison-primitive-input: mathematical-premise
  thm-harrison-electrovacuum-construction-input: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 6
---

## Statement

Use the fixed mass-one end and the positive weight $s_q=q+r^{-1}$ of the preceding denominator lemma. Suppose a supplied smooth stationary primitive has $(W_0)_i=O_5(r^{-3})$ on this end, and use the chosen family
$$W_q=(1-q)^2W_0-4q(1-q)T^\flat,\qquad T_i=g_{0i}=O_6(r^{-2}).$$
Then $(W_q)_i=s_qZ_{qi}$ with $Z_{qi}=O_5(r^{-2})$ uniformly for $q\in[0,1]$. This is the precise meaning of $(W_q)_i=(q+r^{-1})O_5(r^{-2})$ here. At $q=0$ it gives $O_5(r^{-3})$. It supplies no extra power of decay at $q=0$: the stronger expression $(q+r^{-1})O(r^{-3})$ would require $(W_0)_i=O(r^{-4})$.

Existence of a primitive with this end choice is a separate input: the declared primitive and construction suppliers supply it under their own precise GR/SBS and original maximality hypotheses. This conditional calculation does not relax those hypotheses or construct a new primitive.

## Facts & Assumptions

[F1] [[def-stationary-asymptotic-decay-data]] fixes Cartesian componentwise differentiated bounds. [[lem-author-84ac8de0c2f0-end-denominator-bounds]] supplies the weight and uniform inverse derivative bounds, as well as the end metric estimates.

[F2] [[def-harrison-one-form]] specifies the conditions on a supplied Harrison one-form, $T^\flat$ and the Harrison tensor convention; it does not select a unique $W_q$. The polynomial parameter lift displayed in the Statement is the chosen family assumed here and used by the construction interface in [F3].

[F3] [[thm-stationary-harrison-primitive-input]] supplies one primitive with spatial $O_5(r^{-3})$ radial end gauge under its full recorded hypotheses. [[thm-harrison-electrovacuum-construction-input]] uses the displayed polynomial lift. These existence interfaces are not inferred from decay notation.

[F4] [[math:lem-derivative-algebra-and-chain-rules]] supplies the scalar sum, product, quotient and chain rules at points of differentiability, with nonzero denominator for quotients. Apply these rules successively on coordinate lines of the exterior chart; the spatial derivatives hold $q$ fixed. Repeated finite product differentiation is valid through order five for the supplied component bounds.

## Proof

**Given:**The supplied primitive and end bounds in the Statement.

**Goal:** Establish the claimed uniform weighted decay and its exact implication at zero parameter.

1.1 On the exterior chart, the difference quotient of $r=|x|$ in coordinate direction $j$ is $(2x^j+h)/(r(x+he_j)+r(x))$, so $\partial_jr=x^j/r$. Applying [F4] repeatedly gives $|\partial^\beta r^{\pm1}|\le C_\beta r^{\pm1-|\beta|}$ for $|\beta|\le5$: the product and quotient rules give $\partial_jr^a=a x^jr^{a-2}$ for integer $a$, and each further derivative of the resulting finite monomials lowers their radial order by one. By [F1], $|\partial^\beta s_q^{-1}|\le C_\beta s_q^{-1}r^{-|\beta|}$. Since $q$ is spatially constant and $q/s_q\le1$, it follows that $|\partial^\beta(q/s_q)|\le C_\beta r^{-|\beta|}$. The product rule applied to $r^{-1}s_q^{-1}$ gives the same bound for $\partial^\beta(r^{-1}/s_q)$, using $r^{-1}/s_q\le1$. These constants are independent of $q\in[0,1]$. [F1, F4, algebra]

2.1 Divide the displayed spatial formula by $s_q$. The first term is $(1-q)^2(r^{-1}/s_q)\,[r(W_0)_i]$, and the second is $-4(1-q)(q/s_q)g_{0i}$. By the radial bounds in step 1.1 and the iterated product rule in [F4], every derivative of order $k\le5$ of $r(W_0)_i$ is a finite sum of terms of size $O(r^{1-a}r^{-3-(k-a)})=O(r^{-2-k})$, with $0\le a\le k$. Thus this bracketed array is $O_5(r^{-2})$. The quotient bounds from step 1.1, $g_{0i}=O_6(r^{-2})$, and $|1-q|\le1$ give, by the same finite product rule, $Z_{qi}=O_5(r^{-2})$ with one radius and constants for all $q\in[0,1]$. [given, F1, F2, F3, F4, step 1.1, algebra]

3.1 At zero parameter the displayed family equals the supplied $W_0$ and $s_0=r^{-1}$. The proved bound is exactly $O_5(r^{-3})$. In contrast $s_0O(r^{-3})=O(r^{-4})$. An $O(r^{-3})$ hypothesis alone does not imply $O(r^{-4})$: the scalar function $r^{-3}$ has the former order and $r^4r^{-3}=r$ is unbounded. This observation is only about logical strength of estimates; it is not a counterexample satisfying all geometric hypotheses of any article claim. [F1, step 2.1, algebra] ∎

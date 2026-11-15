---
title: Negative stability eigenvalue produces outer trapped graphs
status: draft
research_item: pthm-negative-eigenvalue-trapped-graphs
dependency_level: 11
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 27, proof of Theorem 4.2, contradiction setup
      attribution: The article uses a negative principal eigenvalue and a positive
        eigenfunction to construct outward graphs with strictly negative
        outgoing expansion, then fixes one graph with a uniform negative bound.
      hypotheses: The article's positive-parameter Harrison geometry and its supplied
        smooth maximal section with bifurcation-sphere boundary.
      reading_limits: The frozen article extraction was consulted for attribution and
        scope. This reference is not used as a premise in the proof.
---

PDF p. 27: ` Proof of Theorem 4.2, contradiction setup `

## Prerequisites

- [pthm-mots-stability-operator](item-pthm-mots-stability-operator)
- [def-horizon-flux-and-stability-notation](item-def-horizon-flux-and-stability-notation)
- [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)
- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [thm-principal-eigenvalue-and-mots-stability-input](item-thm-principal-eigenvalue-and-mots-stability-input)
- [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain)
- [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)
- [lem-author-c50357f4fa9e-expansion-second-jet](item-lem-author-c50357f4fa9e-expansion-second-jet)
- [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)
- [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Adopt the regular stationary vacuum model, original maximal exterior section, mass-one normalization and nontriviality of $T|_S$ in [pthm-mots-stability-operator](item-pthm-mots-stability-operator). Fix $q\in(0,1]$ and supply the smooth spacelike maximal section $\Sigma_q$ with boundary $S$, its smooth spacelike extension across $S$, outward unit normal $\nu_q$, and admissible normal-graph tube required there. The bifurcation sphere $S$ is nonempty, connected and compact without boundary. Write $h_q$ for the induced Riemannian metric on the extended section, $n_q$ for its future unit normal, and $\mathscr L_q$ for the outward stability operator in the fixed gauge $L_q=n_q+\nu_q$ of [def-horizon-flux-and-stability-notation](item-def-horizon-flux-and-stability-notation).

If the principal eigenvalue $\lambda_1$ of $\mathscr L_q$ is negative, there is a smooth everywhere positive eigenfunction $\phi$ such that, for all sufficiently small $\epsilon>0$, the outward normal graph $S_\epsilon=\{\exp_x^{h_q}(\epsilon\phi(x)\nu_q(x)):x\in S\}$ has strictly negative outgoing expansion in the gauge $n_q+\nu_{q,\epsilon}$, where $\nu_{q,\epsilon}$ is its outward unit normal in the extended section. Thus each such graph is outer trapped: its outgoing expansion is negative at every point. After fixing one such $\epsilon$, there is $\delta_*>0$ such that $\theta_{n_q+\nu_{q,\epsilon}}(S_\epsilon)\leq-\delta_*$ everywhere. This $\delta_*$ is local to the fixed graph and is unrelated to the uniform parameter interval in Section 3.

## Facts & Assumptions

**Given:** The model, fixed parameter, section, extension and graph data in the Statement, and $\lambda_1<0$. Work in ZFC, including the axiom of choice. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

**Goal:** Construct the asserted outward graphs and the bound on one fixed graph.

[F1] In this setting $S$ has zero outgoing expansion, and its outward variation operator has the displayed smooth elliptic form with leading term $-\not\Delta^{(q)}$. [pthm-mots-stability-operator](item-pthm-mots-stability-operator)

[F2] On a connected compact smooth Riemannian manifold without boundary, a smooth real operator of this form has a smooth positive principal eigenfunction. [thm-principal-eigenvalue-and-mots-stability-input](item-thm-principal-eigenvalue-and-mots-stability-input)

[F3] The normal graph and its outward null gauge are well defined for every sufficiently small multiple of a smooth function on compact $S$. [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain) [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)

[F4] In that gauge the pulled-back expansion is locally a smooth function of the graph's second jet, and its derivative at the zero graph is $\mathscr L_q$. [lem-author-c50357f4fa9e-expansion-second-jet](item-lem-author-c50357f4fa9e-expansion-second-jet) [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data) [def-horizon-flux-and-stability-notation](item-def-horizon-flux-and-stability-notation)

[F5] A continuous real function on a nonempty compact metric space attains its minimum and maximum. [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)

[F6] If a real function $f$ is continuous on $[a,b]$, with $a<b$, and differentiable on $(a,b)$, there is $c\in(a,b)$ such that $f(b)-f(a)=f\prime(c)(b-a)$. [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

## Proof

**Proof technique:** direct.

1.1 By [F1], $S$ is a marginally outer trapped surface, meaning that its outgoing expansion vanishes, and $\mathscr L_q$ is a smooth real elliptic operator of the form required by [F2]. Since $S$ is connected and compact, [F2] supplies a smooth $\phi>0$ with $\mathscr L_q\phi=\lambda_1\phi$. By [F3], $u=\epsilon\phi$ defines an admissible outward graph for all sufficiently small $|\epsilon|$. Let $\Theta(\epsilon,x)$ denote its outgoing expansion pulled back to $x\in S$ in the fixed gauge. [given, F1, F2, F3]

2.1 The initial expansion is zero and [F4] gives $\partial_\epsilon\Theta(0,x)=\lambda_1\phi(x)$. By [F5], $m=\min_S\phi>0$. The second-jet expression in [F4] makes $\partial_\epsilon\Theta$ jointly continuous near $\{0\}\times S$. Compactness of $S$ and a finite neighborhood cover therefore give an $\epsilon_0>0$ such that $\partial_\epsilon\Theta(t,x)\leq\lambda_1m/2<0$ for all $x\in S$ and $0\leq t\leq\epsilon_0$. For each fixed $x\in S$ and $0<\epsilon\leq\epsilon_0$, [F4] makes $t\mapsto\Theta(t,x)$ continuous on $[0,\epsilon]$ and differentiable on $(0,\epsilon)$. By [F6] there is $c\in(0,\epsilon)$ with $\Theta(\epsilon,x)-\Theta(0,x)=\epsilon\partial_\epsilon\Theta(c,x)$. Since $\Theta(0,x)=0$, the derivative bound gives $\Theta(\epsilon,x)\leq\epsilon\lambda_1m/2<0$. The graph map is a diffeomorphism onto its image, so this is the asserted pointwise negativity on $S_\epsilon$. [given, F4, F5, F6, step 1.1]

3.1 Fix any $\epsilon\in(0,\epsilon_0]$ and set $\delta_*=-\epsilon\lambda_1m/2>0$. The inequality in step 2.1 gives $\theta_{n_q+\nu_{q,\epsilon}}\leq-\delta_*$ everywhere on that graph. The choice depends on the fixed $q$, eigenfunction and graph; it does not assert a bound uniform in the separate Section 3 parameter. This proves the Statement. [given, step 2.1] ∎

## Source notes

The article reference attributes the contradiction setup. The proof uses the stated completed suppliers and does not take the article's claim as a premise.

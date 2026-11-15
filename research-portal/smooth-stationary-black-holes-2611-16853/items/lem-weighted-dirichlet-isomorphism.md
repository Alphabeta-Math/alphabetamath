---
id: lem-weighted-dirichlet-isomorphism
title: "Lemma 3.1: weighted Dirichlet Laplacian isomorphism"
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-exterior-weighted-elliptic-data
  - def-weighted-holder-spaces
  - def-fredholm-continuation-data
  - lem-exterior-parametrix-and-compact-potential
  - lem-author-1f6675f2ec55-decaying-kernel-components
  - math:thm-bounded-inverse-theorem
  - math:def-axiom-of-choice
  - math:thm-choice-implies-dependent-implies-countable-choice
dependency_roles:
  def-exterior-weighted-elliptic-data: mathematical-premise
  def-weighted-holder-spaces: mathematical-premise
  def-fredholm-continuation-data: mathematical-premise
  lem-exterior-parametrix-and-compact-potential: mathematical-premise
  lem-author-1f6675f2ec55-decaying-kernel-components: mathematical-premise
  math:thm-bounded-inverse-theorem: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 13, Lemma 3.1 and its proof
      statement: The weighted zero-Dirichlet operator $\Delta_h-V$ is an isomorphism
        for weights between -1 and 0; the proof invokes index zero, compactness
        of multiplication by $V$, and the maximum principle.
      hypotheses: The article's smooth asymptotically flat exterior, compact boundary,
        $h-\delta\in C^{3,\alpha}_{-1}$, nonnegative $V\in C^{2,\alpha}_{-4}$,
        and $-1<\beta<0$.
      reading_limits: Read the frozen article text at Lemma 3.1 and its proof. This
        reference attributes the article claim and is not used as a proof
        premise.
dependency_level: 5
---

## Statement

Work in ZFC. Let $(\Sigma,h)$ be a connected smooth three-dimensional exterior with compact smooth boundary $S$, one fixed asymptotically Euclidean end chart, and $h-\delta\in C^{3,\alpha}_{-1}$. Let $0<\alpha<1$, $-1<\beta<0$, and $0\le V\in C^{2,\alpha}_{-4}$. With the weighted Hölder norms defined using the fixed compact core and scaled end annuli, put $X_\beta=\{w\in C^{4,\alpha}_\beta:w|_S=0\}$ and $Y_\beta=C^{2,\alpha}_{\beta-2}$. Then $L=\Delta_h-V:X_\beta\to Y_\beta$ is a bounded linear bijection with bounded inverse. Here $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$.

## Statement references

[[def-exterior-weighted-elliptic-data]]

[[def-weighted-holder-spaces]]

[[def-fredholm-continuation-data]]

## Facts & Assumptions

[F1] The exterior interface supplies the end, boundary, weighted Dirichlet domain and Laplacian conventions; the weighted Hölder definition fixes the norm and its decay convention. [[def-exterior-weighted-elliptic-data]] [[def-weighted-holder-spaces]]

[F2] Under the stated metric, weight and potential hypotheses, $L:X_\beta\to Y_\beta$ is Fredholm of index zero between Banach spaces. [[lem-exterior-parametrix-and-compact-potential]]

[F3] A Fredholm operator has closed range and finite-dimensional kernel and cokernel, and its index is the kernel dimension minus the cokernel dimension. [[def-fredholm-continuation-data]]

[F4] For a nonnegative potential of the stated regularity, the decaying Dirichlet kernel is zero on a connected exterior. [[lem-author-1f6675f2ec55-decaying-kernel-components]]

[F5] A bounded bijective linear map between Banach spaces has a bounded inverse under dependent choice. ZFC supplies AC, and AC implies dependent choice. [[math:thm-bounded-inverse-theorem]] [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]]

## Proof

**Given:**The hypotheses in the Statement.

**Goal:** Prove that $L:X_\beta\to Y_\beta$ is a bounded isomorphism.

1.1 The exterior and norm conventions match the scalar Dirichlet Fredholm result, including the compact inner boundary, $h-\delta\in C^{3,\alpha}_{-1}$ and $-1<\beta<0$. Thus $L$ is bounded and Fredholm of index zero between the specified Banach spaces. The potential is nonnegative and the exterior is connected, so the decaying-kernel result gives $\ker L=\{0\}$. [given, F1, F2, F4]

2.1 The index formula now gives $\dim(Y_\beta/\operatorname{ran}L)=0$. Hence the range equals $Y_\beta$, so $L$ is bijective. By F5, ZFC supplies dependent choice, so the bounded inverse theorem applies to this bounded bijection between Banach spaces and gives a bounded linear inverse. This proves the assertion. [F3, F5, step 1.1] ∎

## Source notes

The article's index, compactness and maximum-principle argument is attributed above. The proof here uses the separately supplied scalar exterior Fredholm and kernel results; the article is not a logical premise.

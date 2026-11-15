---
id: thm-author-58255dfd955f-bounded-potential-harnack-input
title: Imported unit-ball Harnack inequality with bounded potential
kind: theorem
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-axiom-of-choice
  - math:def-sobolev-space-wkp-and-its-norm
  - math:def-weak-derivative-of-a-locally-integrable-function
  - math:def-lebesgue-measure-and-the-lebesgue-sigma-algebra
  - math:def-borel-and-lebesgue-measurable-function-on-rn
dependency_roles:
  math:def-axiom-of-choice: mathematical-premise
  math:def-sobolev-space-wkp-and-its-norm: mathematical-premise
  math:def-weak-derivative-of-a-locally-integrable-function: mathematical-premise
  math:def-lebesgue-measure-and-the-lebesgue-sigma-algebra: mathematical-premise
  math:def-borel-and-lebesgue-measurable-function-on-rn: mathematical-premise
provenance:
  statement: literature-derived
  proof: literature-derived
external_input: true
sources:
  references:
    - title: Leon Simon, Lectures on Partial Differential Equations
      url: https://math.stanford.edu/~lms/lecs-on-pde.pdf
      locator: Lecture 18, Theorem 1 and its displayed proof, printed p.211 (PDF sheet
        108); coefficient hypotheses (i)–(iii), Lecture 17, printed pp.199–200
        (PDF sheets 102–103), including the bounded-measurable q=∞ convention
        and essential-supremum remark on p.200; specialization R=1 and θ=1/2.
      statement: Let $n\ge2$. On $B_1\subset\mathbb R^n$, let $A$ be real measurable
        symmetric with $\xi^TA\xi\ge|\xi|^2$ and $\sum_{i,j}|A^{ij}|\le\Lambda$,
        and let $Q_0$ be real measurable with $0\le Q_0\le Q$. A nonnegative
        weak solution $v\in W^{1,2}(B_1)$ of $-\operatorname{div}(A\nabla
        v)+Q_0v=0$ satisfies $\operatorname{ess\,sup}_{B_{1/2}}v\le
        C\operatorname{ess\,inf}_{B_{1/2}}v$, with $C$ depending only on
        $n,\Lambda,Q$.
      hypotheses: Use the source's multi-index operator with a_{e_i,e_j}=A^{ij},
        a_{00}=Q_0, all first-order coefficients zero. Its normalized
        ellipticity is (i), its top coefficient bound is (ii), and on the unit
        ball condition (iii) holds with q=∞ and Γ=√Q. Theorem 1 uses θ=1/2.
        Supremum/infimum are understood essentially for weak representatives;
        for the present continuous solutions these are the ordinary extrema.
      reading_limits: For this adjudication, opened the 118-sheet author PDF through
        the browser and read the extracted text of the coefficient hypotheses
        (i)–(iii) on printed p.199, the q=∞ and essential-supremum conventions
        on p.200, and the full Theorem 1 statement and short proof on p.211. The
        proof invokes Lecture 17 Theorems 1–2; their iteration proofs were not
        reconstructed or read in full. Only the unit-ball bounded-potential
        specialization is imported. No general-radius interpretation of the
        printed lower-order scaling expression is used. No claim of a fresh
        local PDF download or rendered-image inspection is made.
dependency_level: 0
---

## Statement

Let $n\ge2$. On $B_1\subset\mathbb R^n$, let $A$ be real measurable symmetric with $\xi^TA\xi\ge|\xi|^2$ and $\sum_{i,j}|A^{ij}|\le\Lambda$, and let $Q_0$ be real measurable with $0\le Q_0\le Q$. A nonnegative weak solution $v\in W^{1,2}(B_1)$ of $-\operatorname{div}(A\nabla v)+Q_0v=0$ satisfies $\operatorname{ess\,sup}_{B_{1/2}}v\le C\operatorname{ess\,inf}_{B_{1/2}}v$, with $C$ depending only on $n,\Lambda,Q$.

## Facts & Assumptions

**Given:** Work in ZFC, including [[math:def-axiom-of-choice]]; this includes the countable choice assumed by the formulation suppliers below. The open ball is Euclidean.

[F1] Use $W^{1,2}(B_1;\mathbb R)$ as the space of almost-everywhere classes with square-integrable weak first derivatives from [[math:def-sobolev-space-wkp-and-its-norm]]. The gradient $\nabla v$ consists of the weak derivatives in [[math:def-weak-derivative-of-a-locally-integrable-function]]; $v\ge0$ means almost everywhere.

[F2] All null sets and integrals use Lebesgue measure $\lambda_n$ from [[math:def-lebesgue-measure-and-the-lebesgue-sigma-algebra]]. Measurability of each real coefficient on $B_1$ means that its extension by zero to $\mathbb R^n$ is Lebesgue measurable in the sense of [[math:def-borel-and-lebesgue-measurable-function-on-rn]]. Coefficient bounds are understood almost everywhere.

[F3] A weak solution means $\int_{B_1}(A\nabla v\cdot\nabla\varphi+Q_0v\varphi)\,d\lambda_n=0$ for every real smooth function $\varphi$ compactly supported in $B_1$. For measurable $E\subseteq B_1$, set $\operatorname{ess\,sup}_E v=\inf\{a\in\mathbb R:\lambda_n(\{x\in E:v(x)>a\})=0\}$ and $\operatorname{ess\,inf}_E v=\sup\{a\in\mathbb R:\lambda_n(\{x\in E:v(x)<a\})=0\}$, with extended-real infimum and supremum conventions. These expressions ignore changes on null sets.

[F4] The independent Simon reference supplies the analytic Harnack conclusion with the coefficient and weak-solution hypotheses in External input. It is imported, rather than proved locally.

## External input

Let $n\ge2$. On $B_1\subset\mathbb R^n$, let $A$ be real measurable symmetric with $\xi^TA\xi\ge|\xi|^2$ and $\sum_{i,j}|A^{ij}|\le\Lambda$, and let $Q_0$ be real measurable with $0\le Q_0\le Q$. A nonnegative weak solution $v\in W^{1,2}(B_1)$ of $-\operatorname{div}(A\nabla v)+Q_0v=0$ satisfies $\operatorname{ess\,sup}_{B_{1/2}}v\le C\operatorname{ess\,inf}_{B_{1/2}}v$, with $C$ depending only on $n,\Lambda,Q$.

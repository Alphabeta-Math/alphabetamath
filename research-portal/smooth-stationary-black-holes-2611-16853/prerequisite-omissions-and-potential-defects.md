---
title: Prerequisite omissions and potential defects
research_report: defects
description: Original-article findings for The uniqueness of smooth stationary black holes.
status: draft
generated_at: 2026-11-15T05:45:21.741Z
---

2 confirmed findings and 1 potential finding in the original article.

## article-remark13-flow-domain · confirmed

**Tags:** typos

https://arxiv.org/abs/2611.16853v1; PDF p.4, Remark 1.3, opening product identity and final stationary-flow map (PDF p. 4).

> ` The maximality of Σ0 in our assumption implies that E = R × Σ0. `

The displayed stationary-flow map uses all of Σ₀ as its domain. Definition 1.1 includes S in Σ₀, whereas S is outside the open DOC. At time zero a point of S therefore has no image in E. The surrounding lapse argument concerns the exterior section.

The printed domain includes the bifurcation sphere; this is a literal domain-notation correction, not a counterexample to exterior uniqueness.

**Correction:** Write C=Σ₀∩E and use R×C→E throughout this remark.

## article-remark13-scalar-lapse · confirmed

**Tags:** typos

https://arxiv.org/abs/2611.16853v1; PDF p.4, Remark 1.3, sentence immediately after the maximum-principle bound (PDF p. 4).

> ` This means that −g(n, N) > 0 `

The expression $−g(n,N)$ uses the scalar lapse as a vector. The same paragraph defines $T=Nn+X$. Its intended transversality statement is $−g(n,T)=N>0$.

Rendered p.4 confirms N is printed; the preceding decomposition fixes the intended vector unambiguously.

**Correction:** Replace N by T in that metric pairing.

## article-ik-globalization-gap · potential

**Tags:** missing proof steps

https://arxiv.org/abs/2611.16853v1; PDF p.4, Theorem 1.1, consequence attributed to [23]; compare pp.28–29, Proposition 5.1 (PDF p. 4).

> ` Consequently, by [23], E is isometric to the exterior of some Kerr spacetime `

The passage from the horizon criterion to one global Kerr exterior is not explained. The independently read [IK Main Theorem](https://arxiv.org/pdf/0711.0040v2), p.8, and [final revision](https://web.math.princeton.edu/~seri/papers/Kerr-finalrevision.pdf), p.8, give local isometry. The original recovery proof adds no globalization argument. Its global hypotheses may suffice; no false conclusion is established.

The authors attribute a global consequence to a local theorem; the omission is in their cited inference, independently of generated supplier packages.

**Correction:** Supply globalization with injectivity, surjectivity and matched hypotheses, or a precise applicable global theorem.

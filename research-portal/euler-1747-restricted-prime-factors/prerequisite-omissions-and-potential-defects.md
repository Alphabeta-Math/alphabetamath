---
title: Prerequisite omissions and potential defects
research_report: defects
description: Original-article findings for Euler’s 1747 conjecture on sums of
  integers with restricted prime factors.
status: draft
generated_at: 2026-11-19T15:50:22.081Z
---

1 confirmed finding in the original article.

## article-euler-ambient-determinant-balance · confirmed

**Tags:** prerequisite omission

https://hexagonmath.org/pdf/2611.00370v1; PDF p. 4, §3.3, paragraph between (3.7) and (3.8) (PDF p. 4).

> ` is orthogonal to both 1 and χp `

Centering the orbit indicator uses determinant-sign cancellation over the whole quotient. Orbit balance gives $\langle f_p,\chi_p\rangle=0$. The asserted centered orthogonality also uses $\langle\mathbf 1,\chi_p\rangle=0$.

The authors explicitly balance the orbit, then assert the centered identity. The full-quotient cancellation is implicit in that inference.

**Correction:** Take $k\in K_p$ with nonsquare determinant by norm surjectivity. Right translation by $k$ permutes $Y_p$ and reverses $\chi_p$, so the ambient sum vanishes.

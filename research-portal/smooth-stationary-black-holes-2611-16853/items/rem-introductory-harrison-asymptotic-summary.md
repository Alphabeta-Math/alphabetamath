---
id: rem-introductory-harrison-asymptotic-summary
title: Introductory Harrison asymptotic claims
kind: remark
status: published
origin: pipeline
domain: physics
proof_strategy: direct
deps:
  - def-stationary-asymptotic-decay-data
  - def-harrison-one-form
  - def-harrison-normalization
  - thm-stationary-harrison-primitive-input
  - thm-harrison-electrovacuum-construction-input
  - lem-author-84ac8de0c2f0-end-denominator-bounds
  - lem-author-84ac8de0c2f0-weighted-one-form-decay
  - lem-author-84ac8de0c2f0-spatial-harrison-end
  - lem-author-84ac8de0c2f0-positive-parameter-end-normalization
  - lem-author-84ac8de0c2f0-zero-parameter-cylinder-area
dependency_roles:
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-harrison-one-form: mathematical-premise
  def-harrison-normalization: mathematical-premise
  thm-stationary-harrison-primitive-input: mathematical-premise
  thm-harrison-electrovacuum-construction-input: mathematical-premise
  lem-author-84ac8de0c2f0-end-denominator-bounds: mathematical-premise
  lem-author-84ac8de0c2f0-weighted-one-form-decay: mathematical-premise
  lem-author-84ac8de0c2f0-spatial-harrison-end: mathematical-premise
  lem-author-84ac8de0c2f0-positive-parameter-end-normalization: mathematical-premise
  lem-author-84ac8de0c2f0-zero-parameter-cylinder-area: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p.6 §1.4; p.10 §2.3; p.12 opening of §3 and normalization (3.1)
      reading_limits: For this repair, read the frozen PDF text and visually inspected
        PDF pages 6, 10 and 12 at the listed passages. Checked only what is
        printed and the parameter qualifications. The article supplies
        attribution only; it is not an independent prerequisite for its own
        mathematical or physical claims. No proof audit or author-defect
        determination is claimed.
      statement: "Attribution only: PDF p.6 §1.4 prints $(W_q)_i=(q+r^{-1})O(r^{-3})$,
        $D_q=4(q+r^{-1})^2(1+O_5(r^{-1}))$ uniformly for $q\\in[0,1]$, the
        coordinate scales $t_q\\asymp t/q$, $x_q=qx$, receding normalized ends,
        asymptotic flatness of every $g_q$ for $q>0$ in those coordinates, and
        the assertion that $g_0$ is no longer asymptotically flat while its
        spatial sections are asymptotically cylindrical with limiting area
        $4\\pi$. PDF p.10 §2.3 instead prints
        $(W_q)_i=(1-q)^2(W_0)_i-4q(1-q)g_{0i}=(q+r^{-1})O_5(r^{-2})$. PDF p.12
        specifies $t_q=d_qt/(4q)$, $x_q=qx$, $r_q=qr$ and allows constants to
        depend on a fixed positive lower parameter bound. These are facts about
        the printed passages, not premises proving the geometric assertions."
      hypotheses: Attribution in this article-origin remark to the frozen v1 article,
        in its mass-one stationary vacuum setting and chosen Harrison family; q
        lies in [0,1], coordinate normalization requires q>0, and normalized
        uniform estimates fix delta>0 with q in [delta,1]. No validity of a
        printed formula is assumed merely from its occurrence.
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: §1.1 (1.1); §3.2 (3.19); §3.3 (3.28)–(3.29)
      reading_limits: Retrieved v1 HTML; read §1.1, (3.19) and its following sentence,
        and (3.28)–(3.29) with adjacent paragraphs. Use is limited to the
        displayed comparison. No proof audit, stronger decay, or additional
        theorem is imported.
      statement: For comparison only, (3.28) prints $\sigma=1-2/r+O_6(r^{-2})$.
        Equation (3.19) sets $\tau=D_q(p)t/4$; the following sentence sets
        $s=\tau/q$ for $q>0$. After (3.29), $x'=qx$ accompanies this unit
        asymptotic time. With the local notation $d_q=D_q(p)$, these are the
        potential expansion and exact time normalization compared in
        Justification 2.1.
      hypotheses: Radu v1, smooth stationary vacuum spacetime under GR, SBS and
        original maximality (§1.1), rescaled to M=1; normalized Ernst potential,
        chosen horizon pole p, and fixed q>0 for unit asymptotic time. No
        angular-momentum smallness is used in these comparisons.
physical_scope: Four-dimensional general relativity in the smooth stationary,
  asymptotically flat vacuum black-hole model; this is attributed contextual
  comparison, not a measurement or an independent physical postulate.
dependency_level: 9
---

## Statement

In the article's mass-one stationary vacuum setting, with the chosen Harrison family, §1.4 (PDF p.6) prints the spatial one-form estimate
$$(W_q)_i=(q+r^{-1})O(r^{-3}),$$
and the uniform denominator expression $D_q=4(q+r^{-1})^2(1+O_5(r^{-1}))$ for $q\in[0,1]$. It states that every $g_q$ for $q>0$ is asymptotically flat in normalized coordinates $t_q\asymp t/q$, $x_q=qx$, and that these ends recede to infinity in the original spacetime coordinates. It also states that $g_0$ is no longer asymptotically flat and that its spatial sections are asymptotically cylindrical with limiting area $4\pi$.

These are preserved as attributed introductory claims. The one-form order differs from the detailed §2.3 estimate on PDF p.10,
$$(W_q)_i=(1-q)^2(W_0)_i-4q(1-q)g_{0i}=(q+r^{-1})O_5(r^{-2}).$$
The latter follows from the chosen primitive bound $(W_0)_i=O_5(r^{-3})$ and $g_{0i}=O_6(r^{-2})$, through the local weighted-decay lemma. At $q=0$ the introductory expression asks for $O(r^{-4})$, whereas this detailed argument supplies $O_5(r^{-3})$. The extra order in the introductory formula remains unestablished here: neither a proof of it nor a geometric counterexample under the article's complete hypotheses is supplied. The two formulas are retained distinctly; this remark is not a supplier for the stronger estimate and does not assert an article defect.

For the denominator, coordinate and spatial-limit mechanisms, the five local lemmas give complete conditional calculations from the explicitly supplied end, normalized potential and primitive bounds. Under those hypotheses, the positive-parameter normalization lemma establishes an asymptotically flat designated spacetime end for each fixed $q>0$. At $q=0$, the cylinder lemma establishes the asymptotically cylindrical geometry of the specified spatial coordinate sections and their limiting coordinate-sphere area; this spatial calculation alone does not establish the broader assertion excluding every possible asymptotically flat spacetime end or slicing. The exact positive-parameter time normalization is $t_q=d_qt/(4q)$, not just a choice up to scale; the same pole-evaluation constant $d_q=D_q(p)$ used in the one-form contraction is required. The $O_5$ constants for normalized coordinates are controlled on $q\in[\delta,1]$ with $\delta>0$ fixed. A fixed $r_q=R$ represents original radius $R/q$, while $q=0$ is handled directly in the original spatial coordinates, not by substituting zero in $t_q,x_q$.

## Facts & Assumptions

[F1] [[def-stationary-asymptotic-decay-data]] defines differentiated Cartesian bounds and the distinction between fixed-parameter and uniform estimates. [[def-harrison-one-form]] and [[def-harrison-normalization]] fix the tensor, contraction and mass-one pole normalization.

[F2] [[thm-stationary-harrison-primitive-input]] supplies the radial end primitive with $(W_0)_i=O_5(r^{-3})$, and [[thm-harrison-electrovacuum-construction-input]] supplies the chosen polynomial family $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, under their precise recorded mass-one GR/SBS and original maximality hypotheses. Those hypotheses remain attached to these existence inputs; no broader existence conclusion is inferred from the formal calculations.

[F3] [[lem-author-84ac8de0c2f0-end-denominator-bounds]] establishes the normalized potential and uniform denominator estimates from the stated stationary mass-one end and supplied Ernst equation. [[lem-author-84ac8de0c2f0-weighted-one-form-decay]] proves the detailed one-form order with no additional cancellation assumption.

[F4] [[lem-author-84ac8de0c2f0-spatial-harrison-end]] estimates the spatial metric, [[lem-author-84ac8de0c2f0-positive-parameter-end-normalization]] gives the exact positive-parameter normalization and its parameter range, and [[lem-author-84ac8de0c2f0-zero-parameter-cylinder-area]] gives the zero-parameter spatial cylinder and limiting coordinate-sphere area.

## Justification

**Given:** The attributed introductory formulas and the declared end data and suppliers.

**Goal:** Explain the conditional calculations and the limits of the stronger printed estimate.

1.1 The introductory formulas and their detailed counterpart are source-attribution content, not imported premises proving themselves. The one-form comparison in [F3] identifies exactly the additional decay requested at zero parameter, and leaves it unresolved without promoting the scalar non-implication example to a spacetime counterexample. [given, F1, F2, F3]

2.1 The denominator and the end conclusions in [F3]–[F4] are conditional consequences of explicit end data and the supplied primitive; [F2] records the scope in which the independently authored construction provides that primitive. They do not infer a new, stronger one-form bound or a weaker construction hypothesis. In particular, the normalized component bounds in [F4] establish an asymptotically flat designated end for every fixed $q>0$; at $q=0$, [F4] establishes the cylinder only for the specified spatial sections. The article's assertion that $g_0$ is no longer asymptotically flat is retained as attribution; the spatial calculation alone does not exclude every other possible spacetime end or slicing. Radu's independent §3.3 (3.28) prints the same mass-one normalized potential expansion, and (3.19) with the subsequent normalized time gives $\tau=d_qt/4$ and $s=\tau/q$, matching the exact time scale used here. Those passages are contextual comparison, not an extra unrecorded logical input. Accordingly all introductory claims, including the stronger printed one-form order, remain visible with their distinct evidence and limits. [F2, F3, F4, step 1.1] ∎

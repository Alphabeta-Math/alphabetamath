---
id: pthm-small-horizon-field-rigidity-input
title: Smooth rigidity from a quantitatively small horizon field
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - def-author-0a41d659d5ab-aik-quantitative-package
  - lem-author-0a41d659d5ab-horizon-field-norm
  - lem-author-0a41d659d5ab-ergoregion-collar
  - physics:post-gr-einstein-field-law
  - physics:def-gr-fx-kerr-exterior
  - math:def-axiom-of-choice
dependency_roles:
  def-author-0a41d659d5ab-aik-quantitative-package: mathematical-premise
  lem-author-0a41d659d5ab-horizon-field-norm: mathematical-premise
  lem-author-0a41d659d5ab-ergoregion-collar: mathematical-premise
  physics:post-gr-einstein-field-law: physical-assumption
  physics:def-gr-fx-kerr-exterior: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: S. Alexakis, A. D. Ionescu and S. Klainerman, Rigidity of stationary
        black holes with small angular momentum on the horizon
      url: https://arxiv.org/pdf/1304.0487v2
      locator: Abstract and Introduction, PDF pp. 1–2; §1.1.3 Theorem 1.1 and (1.5),
        PDF p. 4; §1.2 (1.10), PDF p. 6
      statement: Under the smooth stationary vacuum GR and SBS assumptions, with the
        specified asymptotically flat maximal section and fixed quantitative
        constant A, there is a sufficiently small epsilon depending only on A
        such that sup_{S0}|g(T,T)|<epsilon^2 implies stationarity and axial
        symmetry and isometry of the domain of outer communications to a Kerr
        domain of outer communications with small angular momentum.
      hypotheses: The complete source GR, SBS, maximality and quantitative assumptions
        transcribed in the exact AIK package, including M0>0, J<M0^2, transverse
        complete exterior orbits, smooth non-expanding bifurcate event horizons,
        and T not identically zero on S0. The parameter epsilon is chosen after
        fixing A.
      reading_limits: For this repair, consulted arXiv:1304.0487v2, Abstract and
        Introduction, GR/SBS and maximal-section assumptions, Theorem 1.1,
        Proposition 1.3 and the quantitative assumptions through (1.10), PDF pp.
        1–6. Checked the existing local package, norm and confinement suppliers
        for this application. The source rigidity proof, its local construction,
        global Killing-field extension and Carter–Robinson classification were
        not reconstructed or independently reviewed. The full main theorem
        remains an explicitly imported premise of the local application.
physical_scope: Conditional classical four-dimensional stationary vacuum
  Einstein model with zero cosmological constant and vanishing stress-energy; no
  observational or dynamical-settling claim.
dependency_level: 6
---

## Statement

In the four-dimensional classical vacuum Einstein model with zero cosmological constant, impose the exact AIK quantitative stationary package, including GR, SBS and the asymptotically flat maximal section. Once $A$ is fixed there is $\epsilon_*(A)>0$ such that $\sup_{S_0}|g(T,T)|<\epsilon_*^2$ implies that the exterior $E$ is isometric to a subextremal Kerr exterior, with the source stationary and axial symmetries. Here the horizon bound is equivalently $\sup_{S_0}|T|_h<\epsilon_*$, using the induced positive metric on $S_0$. The source SBS hypothesis retains $T|_{S_0}\not\equiv0$. The non-timelike subset of the maximal section is then contained in the local rotational-rigidity neighborhood. Smallness of ADM angular momentum is not substituted for this horizon-field condition.

## Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [[math:def-axiom-of-choice]]

[F1] The full GR, SBS, maximality and quantitative assumptions, including the exact constant $A$, are given in [[def-author-0a41d659d5ab-aik-quantitative-package]].

[F2] Horizon tangency makes the source scalar smallness exactly the induced-metric norm smallness. [[lem-author-0a41d659d5ab-horizon-field-norm]]

[F3] The explicit quantitative estimates give confinement of the non-timelike region to the local rotational-rigidity neighborhood. [[lem-author-0a41d659d5ab-ergoregion-collar]]

[A2] Adopt the direct-equation Einstein model, including the model assumptions specified by the field-law supplier, on its matter domain $U\subseteq M$, with vanishing stress-energy on $U$ and $\Lambda=0$. [[physics:post-gr-einstein-field-law]]

[F4] The subextremal Kerr exterior means the standard tensor on $\mathbb R\times(r_+,\infty)\times S^2$ with $M_0>0$, $|a|<M_0$, and $r_+=M_0+\sqrt{M_0^2-a^2}$. [[physics:def-gr-fx-kerr-exterior]]

[F5] The independently sourced AIK Theorem 1.1, under its full GR/SBS/maximal and quantitative hypotheses, is the imported main theorem recorded in External input and the source reference.

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conditional conclusion.

1.1 On the matter domain $U$ specified in [A2], with vanishing stress-energy and $\Lambda=0$, [A2] gives $\operatorname{Ric}_{ab}-\tfrac12Rg_{ab}=0$. Its four-dimensional trace is $R-2R=0$, hence $R=0$ and $\operatorname{Ric}=0$ on $U$. For the rigidity theorem, use the independently assumed $\operatorname{Ric}(g)=0$ on all of $M$ in [F1]; no extension of the field-law deduction beyond $U$ is required. By [F2] the stated horizon norm condition and the source scalar condition are equivalent. Choose $\epsilon_*(A)$ below the threshold in [F5] and that for [F3]; both depend only on the fixed source bounds. [A2, F1, F2, F3, F5, algebra]

2.1 Apply the imported main theorem [F5] with exactly the GR/SBS/maximal and quantitative package [F1]. It gives the asserted stationary axisymmetric Kerr exterior, with the small-angular-momentum range in the source and the subextremal tensor meaning in [F4]. Independently [F3] gives the recorded confinement. The global extension and Kerr-classification steps are part of the imported theorem, not conclusions reconstructed from confinement alone. No inference from a small ADM angular momentum assumption is made. [step 1.1, F1, F3, F4, F5] ∎

## External input

Import AIK Theorem 1.1 in its complete GR/SBS/maximal and quantitative setting. The source condition is $\|g(T,T)\|_{L^\infty(S_0)}<\epsilon^2$, with $\epsilon$ sufficiently small depending only on $A$ from (1.10). The source abstract identifies the isometry conclusion as one about the domains of outer communications. This contract imports the full rigidity theorem, including the global extension and classification it invokes; it does not assert a locally reconstructed rigidity proof.

## Source notes

The exact AIK package retains its own stronger coordinate decay, its GR/SBS assumptions and its nonzero-horizon-field clause; it is separate from a generic black-hole regularity package. AIK uses the non-strict set $g(T,T)\ge0$ in Proposition 1.3, while some terminology calls only $g(T,T)>0$ the ergoregion; the explicit inequality here avoids that convention ambiguity. No source defect or independent mathematical acceptance is asserted.

---
title: "Theorem 3.1: complete maximal slices for positive q"
status: draft
research_item: pthm-complete-maximal-slices
dependency_level: 21
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p.12, Section 3 introduction, (3.1)–(3.2) and Theorem 3.1;
        pp.13–14, Section 3.1 and the opening of Section 3.2
      reading_limits: "Retained prior source-input or attribution record: Retained
        attribution only: For every fixed positive parameter interval the
        article constructs smooth maximal stationary graph slices complete up to
        S, with normalized derivative decay of order minus three quarters
        through four derivatives, by openness and closedness. Attributed
        setting: The regular stationary vacuum construction, original maximal
        exterior section, T not identically zero on S and mass-one
        normalization; attribution only. Consulted the frozen extracted text on
        PDF pp.12–14, including Theorem 3.1, (3.1)–(3.4), and the opening of
        Section 3.2, for attribution and normalization. The local argument
        composes the current declared suppliers. No independent review of the
        full article proof or inspection of PDF images is claimed in this
        repair. Fresh maintenance limits: current item and supplier contracts
        and the local applications were checked; no new reading of the external
        proof or PDF images is claimed."
---

PDF p. 12: ` Theorem 3.1; §§3.1–3.2.3 `; PDF p. 13: ` Theorem 3.1; §§3.1–3.2.3 `; PDF p. 14: ` Theorem 3.1; §§3.1–3.2.3 `; PDF p. 15: ` Theorem 3.1; §§3.1–3.2.3 `; PDF p. 16: ` Theorem 3.1; §§3.1–3.2.3 `; PDF p. 17: ` Theorem 3.1; §§3.1–3.2.3 `; PDF p. 18: ` Theorem 3.1; §§3.1–3.2.3 `; PDF p. 19: ` Theorem 3.1; §§3.1–3.2.3 `; PDF p. 20: ` Theorem 3.1; §§3.1–3.2.3 `; PDF p. 21: ` Theorem 3.1; §§3.1–3.2.3 `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-harrison-one-form](item-def-harrison-one-form)
- [pthm-ernst-potential-existence](item-pthm-ernst-potential-existence)
- [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive)
- [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)
- [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [pthm-author-048251387164-indexed-admissible-end-estimates](item-pthm-author-048251387164-indexed-admissible-end-estimates)
- [pthm-author-048251387164-indexed-height-and-horizon-estimates](item-pthm-author-048251387164-indexed-height-and-horizon-estimates)
- [pthm-author-048251387164-sequence-compact-angle-and-lapse](item-pthm-author-048251387164-sequence-compact-angle-and-lapse)
- [pthm-author-048251387164-sequence-closure-and-completeness](item-pthm-author-048251387164-sequence-closure-and-completeness)
- [pthm-author-048251387164-individual-slice-interval-continuation](item-pthm-author-048251387164-individual-slice-interval-continuation)


## Statement

In the regular mass-one stationary vacuum construction with maximal original exterior section and $T|_S\not\equiv0$, for every $\delta\in(0,1)$ and $q\in[\delta,1]$ there is a smooth spacelike $g_q$-maximal section $\Sigma_q$ with boundary S, complete up to its included boundary, whose interior is a global stationary T-graph over $\Sigma_1^\circ$. Its normalized end height obeys $|D_{x_q}^j\widetilde u_q|\le C_{\delta,j}r_q^{-3/4-j}$ for $0\le j\le4$ on a common end. The $q=1$ section may be chosen as the original maximal section. No uniform estimate as delta tends to zero and no $q=0$ section is asserted. Each selected section has compact smooth physical-end truncations containing a neighborhood of $S$, with outer boundary its graph over the physical coordinate sphere; positive-boundary-distance trims of those truncations are compact in the interior.

## Facts & Assumptions

[A1] Adopt the stationary vacuum model and regular data with original maximal exterior section, mass-one normalization and $T|_S\not\equiv0$. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-harrison-normalization](item-def-harrison-normalization) The graph, maximality, induced completeness and Holder conventions are [def-stationary-maximal-graph](item-def-stationary-maximal-graph), [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) and [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms). Work in ZFC, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice).

[F1] Individual admissibility and estimates for any indexed collection of already existing sections are [pthm-author-048251387164-indexed-admissible-end-estimates](item-pthm-author-048251387164-indexed-admissible-end-estimates). Compact heights and horizon estimates for exactly those indexed pairs are [pthm-author-048251387164-indexed-height-and-horizon-estimates](item-pthm-author-048251387164-indexed-height-and-horizon-estimates).

[F2] Arbitrary convergent existing-candidate sequences have the required compact normal/lapse estimates and admissible complete limiting sections. [pthm-author-048251387164-sequence-compact-angle-and-lapse](item-pthm-author-048251387164-sequence-compact-angle-and-lapse) [pthm-author-048251387164-sequence-closure-and-completeness](item-pthm-author-048251387164-sequence-closure-and-completeness).

[F3] The actual existence set is all positive parameters by the individual-reference openness and arbitrary-sequence closedness argument in [pthm-author-048251387164-individual-slice-interval-continuation](item-pthm-author-048251387164-individual-slice-interval-continuation). This replaces any invocation of an interval-family hypothesis to prove interval existence.

[F4] The Harrison tensor formula is [def-harrison-one-form](item-def-harrison-one-form). Under the regular vacuum hypotheses in [A1], [pthm-ernst-potential-existence](item-pthm-ernst-potential-existence) supplies the normalized smooth stationary Ernst potential $\sigma=f+i\psi$, with $f=-g(T,T)$, real $\psi$ and $\sigma\to1$, on the exterior and an open neighborhood of $S$. For this supplied potential, the regular vacuum, original maximal outer-section and mass-one hypotheses of [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive) are exactly those in [A1]. It gives $D_q>0$ on the exterior and on one open neighborhood of $S$, independent of $q\in[0,1]$, so the denominators in the Harrison tensor formula are positive. Under exactly the regular vacuum, original maximal-section, mass-one and $T|_S\not\equiv0$ hypotheses in [A1], [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum) constructs the chosen stationary one-form family and jointly smooth Lorentzian metrics $g_q$ on the exterior and a common neighborhood of $S$, with $g_1=g$. Under the same regular vacuum hypotheses, [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product) gives the actual section $C=\Sigma_0\cap\mathcal E$, with connected smooth spherical-exterior closure $\Sigma_1=C\cup S$ and a physical asymptotically Euclidean end with compact truncations. Original maximality in [A1] is maximality of this actual exterior section, so the theorem's conditional stationary-flow diffeomorphism $\mathbb R\times C\to\mathcal E$ applies. Its adapted topological radius may put $C$ at $r_{\mathrm{ref}}>1$; this is distinct from the physical end radius $r=|x|$. Thus the metric and product required by the graph definition are supplied before any transformed maximal section is selected.

## Proof

**Given:** Only the regular model, original maximal section and the selected smooth metric family. **Goal:** Construct the stated complete sections and uniform positive-interval end bounds.

1.1 Use [F4] for denominator positivity, the jointly smooth $g_q$ family, its endpoint $g_1=g$ and the global stationary product over $\Sigma_1^\circ$. Their hypotheses are [A1], and neither construction assumes a transformed maximal section. Apply [F3] to the set of parameters possessing one individually admissible slice. Its original $q=1$ member is supplied before continuation; local openness uses only an existing slice. Sequence closure is [F2], whose end, horizon and compact estimates are derived in [F1]–[F2] for the actual indexed candidates, without assuming slices at missing parameters. Thus every $q>0$ has such a slice. The strengthened physical-core conclusion of [F2] applies to each such section, either directly or as a constant sequence: for every sufficiently large physical radius its truncation is a compact smooth region containing a neighborhood of $S$, with the physical graph sphere as outer boundary and compact positive-distance trims. The same result gives completeness with the boundary included. [A1, F1, F2, F3, F4]

2.1 Fix $\delta>0$ and choose an individually admissible slice at each q in [delta,1], taking the original one at $q=1$. ZFC permits this selection. Only now is an interval-wide family formed. Apply the indexed estimate [F1] to these selected pairs: it gives one common end radius and the stated derivative constants through order four, independent of q. The graph and smooth fixed-boundary properties are part of individual admissibility and the construction in [F2]–[F3]. This proves the complete statement without any estimate at $q=0$ or an interval-existence premise in the continuation argument. [A1, F1, F2, F3, step 1.1] ∎

## Source notes

The interval-family existence premise in the earlier generated closedness interface is not invoked. The five new intermediates derive estimates for actual individually existing pairs, establish arbitrary-sequence closure and then apply interval connectedness. Strict limiting spacelikeness uses the upper lapse bound N at most C, giving minus g-inverse(dF,dF) at least C to the minus two; the lower lapse bound is retained for stationary coordinate transfer. A separate generated supplier inference was reported internally for native owner repair, without attributing it to the original article.

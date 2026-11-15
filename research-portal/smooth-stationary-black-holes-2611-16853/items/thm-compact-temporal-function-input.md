---
id: thm-compact-temporal-function-input
title: Compact timelike-length bounds and local temporal functions
kind: theorem
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - def-causal-exterior-and-boundary-data
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - lem-author-89004136b63c-compact-neighborhood-localization
  - lem-author-89004136b63c-compact-length-restriction
  - lem-author-89004136b63c-temporal-compact-margins
  - lem-author-89004136b63c-uniform-inverse-metric-continuity
  - lem-author-89004136b63c-compact-temporal-persistence
  - math:def-countable-choice
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  lem-author-89004136b63c-compact-neighborhood-localization: mathematical-premise
  lem-author-89004136b63c-compact-length-restriction: mathematical-premise
  lem-author-89004136b63c-temporal-compact-margins: mathematical-premise
  lem-author-89004136b63c-uniform-inverse-metric-continuity: mathematical-premise
  lem-author-89004136b63c-compact-temporal-persistence: mathematical-premise
  math:def-countable-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: A. F. Radu, Rigidity of stationary black holes with small ADM angular
        momentum
      url: https://arxiv.org/html/2610.09729v1#A2.Thmtheorem2
      locator: Appendix B, Lemma B.2, equation (B.2)
      statement: Let g be a C² time-oriented Lorentz metric on an open domain B. If
        every compact C in B has a constant L_C bounding the g-length of every
        Lipschitz future curve c:[a,b]→C with g(ċ,ċ)≤−ε_c<0 almost everywhere,
        then every compact Q compactly contained in B has a neighborhood
        admitting a smooth function with past timelike gradient.
      hypotheses: The bound is uniform over all eligible curves in each compact C, for
        every compact C⊂B. The positive timelikeness constant ε_c may depend on
        the curve. The C² metric is time oriented; all curves and compact sets
        are in that open domain.
      reading_limits: Fetched the versioned HTML and read the complete Lemma B.2
        statement, (B.2), and Appendix B introductory context. Located and read
        excerpts of the later Proof of Lemma B.2; its displacement argument was
        not independently reconstructed or verified. This item imports the exact
        stated existence result. Minguzzi was not independently consulted for
        this resolution and is not used as an alternative proof.
dependency_level: 4
---

## Statement

Assume countable choice for the usual Lebesgue-measure convention. Let $B$ be an open subset of a smooth four-manifold without boundary, $g$ a $C^2$ time-oriented Lorentz metric, and $N$ a continuous timelike orientation field. Suppose every compact $C\subset B$ admits a finite $L_C$ bounding $L_g(c)=\int_a^b\sqrt{-g(\dot c,\dot c)}\,dt$ for every future Lipschitz curve $c:[a,b]\to C$ with $g(\dot c,\dot c)\le-\epsilon_c<0$ almost everywhere for some curve-dependent $\epsilon_c>0$. The curves, length and quantifiers have exactly the compact-length convention below. Then every compact $Q\subset B$ has an open neighborhood $O\subset B$ and a smooth real function $\tau$ on $O$ whose $g$-gradient is past timelike. For every compact $K\subset O$, the same $d\tau$ remains past-timelike after raising with any sufficiently small $C^0$ perturbation of $g$ on $K$, oriented by $N$. Here smallness means uniform coefficient closeness in a finite compact chart cover; no property of a deformed metric away from $K$ is inferred. The length hypothesis must hold for every compact subset of the open domain, not merely one selected family of curves.

## Statement references

[[physics:def-gr-smooth-lorentzian-objects]]

[[def-causal-exterior-and-boundary-data]]

[[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

[[lem-author-89004136b63c-compact-neighborhood-localization]]

[[lem-author-89004136b63c-compact-length-restriction]]

[[lem-author-89004136b63c-temporal-compact-margins]]

[[lem-author-89004136b63c-uniform-inverse-metric-continuity]]

[[lem-author-89004136b63c-compact-temporal-persistence]]

[[math:def-countable-choice]]

## Facts & Assumptions

[A1] Countable choice is assumed for the standard Lebesgue measure in the compact-length convention used in [F2] and step 1.1. [[math:def-countable-choice]]

[F1] The Lorentzian-object interface supplies its pointwise conventions: $g_p$ is symmetric and nondegenerate of signature $(-,+,+,+)$, timelike means $g_p(v,v)<0$, and $N_p$ selects the future timelike cone by $g_p(v,N_p)<0$; the opposite cone is past. The causal and inverse-metric interfaces supply the temporal-gradient and index-raising conventions. Only these pointwise definitions are used for the stated $C^2$ metric and continuous orientation field; the suppliers' smooth-field hypotheses and any stationarity requirement are not imposed. [[physics:def-gr-smooth-lorentzian-objects]] [[def-causal-exterior-and-boundary-data]] [[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

[F2] Compact sets admit nested relatively compact neighborhoods, and the exact compact-length hypothesis restricts to open subdomains. [[lem-author-89004136b63c-compact-neighborhood-localization]] [[lem-author-89004136b63c-compact-length-restriction]]

[F3] Compact margins, uniform inverse-metric continuity and temporal-covector persistence hold as locally proved in the three prerequisite helpers. [[lem-author-89004136b63c-temporal-compact-margins]] [[lem-author-89004136b63c-uniform-inverse-metric-continuity]] [[lem-author-89004136b63c-compact-temporal-persistence]]

[F4] Radu Lemma B.2 is an imported existence input under exactly the stated $C^2$, time-orientation and all-compact length hypotheses; the External input section gives its scope.

## External input

Radu, Lemma B.2 and (B.2), supplies the following external existence input: a $C^2$ time-oriented Lorentz metric on an open domain, with a uniform length bound on all uniformly timelike future Lipschitz curves in every compact subset (allowing a curve-dependent positive timelikeness constant), admits a smooth function with past timelike gradient on a neighborhood of each compact subset. This is imported as a source statement. No proof of this existence theorem is claimed locally.

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the conclusions in the Statement.

1.1 Choose $Q\subset V\Subset W\Subset B$ using [F2]. Under [A1], the length hypothesis restricts to $W$ with exactly the same curve and compact-set quantifiers. Apply the precise external existence input [F4] on $W$ to the compact set $Q$. It supplies an open neighborhood $O$ of $Q$, restricted to $W$ if necessary, and a smooth $\tau$ whose $g$-gradient is past timelike. [A1, F1, F2, F4]

2.1 On any compact $K\subset O$, set $\alpha=d\tau$. Then $g^{-1}(\alpha,\alpha)<0$ and $\alpha(N)>0$. The three compact-control helpers in [F3] yield a coefficient threshold preserving these inequalities for the perturbed inverse metric and preserving that $N$ is timelike. Raising $d\tau$ with that metric gives the asserted past-timelike gradient on $K$. This proves both conclusions, with existence supplied externally and perturbation stability proved locally. [F1, F3, step 1.1] ∎

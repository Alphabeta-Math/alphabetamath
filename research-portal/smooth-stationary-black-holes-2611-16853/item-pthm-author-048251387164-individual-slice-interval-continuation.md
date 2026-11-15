---
title: Open–closed continuation for the set of individually admissible parameters
status: published
research_item: pthm-author-048251387164-individual-slice-interval-continuation
dependency_level: 20
sources:
  references:
    - title: Rigidity of stationary black holes with small ADM angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: Section 5.3, Lemma 5.1 and the following continuation paragraph
      statement: Compact maximal stationary graphs with boundary S_0 disjoint-union
        C_s and annular topology have a smoothly converging spacelike
        subsequence under the stated uniform lapse and height bounds.
      hypotheses: Proposition 3.3 hypotheses, compact graphs of topology S^2 times
        [0,1], converging boundary-path parameters, and bounds (5.10) and
        (5.15).
      reading_limits: "Retained prior source-input or attribution record: Consulted
        the actual HTML Lemma 5.1 and its continuation paragraph. This is
        compact-graph background only; it does not supply the present noncompact
        conclusion. The local argument uses the declared suppliers. No
        source-proof audit is claimed. Fresh maintenance limits: current item
        and supplier contracts and the local applications were checked; no new
        reading of the external proof or PDF images is claimed."
---

## Prerequisites

- [pthm-author-048251387164-sequence-closure-and-completeness](item-pthm-author-048251387164-sequence-closure-and-completeness)
- [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product)
- [pthm-maximal-continuation-openness](item-pthm-maximal-continuation-openness)
- [math:thm-connected-subsets-of-r-are-intervals](https://alphabetamath.cc/item/thm-connected-subsets-of-r-are-intervals)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [pthm-author-048251387164-indexed-admissible-end-estimates](item-pthm-author-048251387164-indexed-admissible-end-estimates)
- [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)
- [math:def-metric-space](https://alphabetamath.cc/item/def-metric-space)
- [math:lem-real-line-is-a-metric-space](https://alphabetamath.cc/item/lem-real-line-is-a-metric-space)
- [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:thm-metric-sequential-closure](https://alphabetamath.cc/item/thm-metric-sequential-closure)
- [math:def-connected-r](https://alphabetamath.cc/item/def-connected-r)
- [math:thm-closure-characterisations-r](https://alphabetamath.cc/item/thm-closure-characterisations-r)
- [` Rigidity of stationary black holes with small ADM angular momentum · Section 5.3, Lemma 5.1 and the following continuation paragraph `](https://arxiv.org/html/2610.09729v1)


## Statement

Assume the stationary vacuum model and the regular non-degenerate stationary spacetime data, with mass normalized to one, original exterior section maximal and $T|_S\not\equiv0$. Use the positive-parameter Harrison construction $g_q$, $0<q\le1$. Put $C=\Sigma_0\cap\mathcal E$ and denote its ambient closure by $\Sigma_1=C\cup S$. Choose its supplied adapted topological radial identification, with radius $r_{\mathrm{ref}}$, so $\Sigma_1\cong\{r_{\mathrm{ref}}\ge1\}$ and $S=\{r_{\mathrm{ref}}=1\}$. The physical end radius $r=|x|$ below belongs to the separate stationary end chart.

As in the indexed admissible-end supplier, a section is **individually admissible at $q$** if it is connected, smooth up to its boundary $S$, spacelike and maximal for $g_q$, its interior is a global stationary graph over $\Sigma_1^\circ$, and on some end its normalized height satisfies $|D_{x_q}^j\widetilde u|\le C_q r_q^{-3/4-j}$ for $0\le j\le4$. The radius and finite constant may depend on that section; no common bounds or sections at other parameters enter this definition. Here $x_q=qx$, $r_q=|x_q|$ and $\widetilde u(qx)=d_qu(x)/(4q)$ for original stationary height $u$.

Let $\mathcal A\subset(0,1]$ consist of the parameters admitting such a section. Then $\mathcal A=(0,1]$. The original section can be used at $q=1$. The proof uses local openness at one existing section and arbitrary-sequence closure; it assumes no branch or family over an entire interval before proving existence.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-harrison-normalization](item-def-harrison-normalization)

[def-stationary-maximal-graph](item-def-stationary-maximal-graph)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[pthm-author-048251387164-indexed-admissible-end-estimates](item-pthm-author-048251387164-indexed-admissible-end-estimates)

[pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)

## Facts & Assumptions

[F1] Adopt the conditional stationary vacuum model and all four regular-spacetime conditions, with original exterior section maximal, mass one and $T|_S\not\equiv0$. The normalization and graph conventions are as stated in their definitions. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-harrison-normalization](item-def-harrison-normalization) [def-stationary-maximal-graph](item-def-stationary-maximal-graph)

[F2] Individual admissibility is exactly the predicate in the Statement of the indexed end-estimates supplier; only that predicate is needed here, not its uniform estimate conclusion. Smooth spacelikeness, maximality and boundary regularity use the induced-geometry definition. [pthm-author-048251387164-indexed-admissible-end-estimates](item-pthm-author-048251387164-indexed-admissible-end-estimates) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F3] The actual exterior section $C=\Sigma_0\cap\mathcal E$ has smooth connected spherical-exterior closure $\Sigma_1=C\cup S$. Since this actual exterior section is maximal by [F1], its lapse is positive and the stationary flow identifies $\mathcal E$ with $\mathbb R\times C$. Its adapted topological radial chart places $C$ at $r_{\mathrm{ref}}>1$, without identifying that radius with the physical end radius. The Harrison endpoint satisfies $(g_1,F_1)=(g,0)$, including near $S$. [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product) [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)

[F4] For $0<\delta<q_*\le1$, openness starts from a single connected smooth spacelike maximal section at $q_*$, smooth up to $S$, whose interior is a global stationary graph and whose normalized end height has the stated decay through four derivatives. It gives nearby smooth fixed-boundary graphs with the same end decay. [pthm-maximal-continuation-openness](item-pthm-maximal-continuation-openness)

[F5] A sequence of individually admissible pairs on a fixed positive parameter interval, with converging parameter, has an individually admissible limiting section at that parameter, complete up to its included boundary. No interval-wide family is required. [pthm-author-048251387164-sequence-closure-and-completeness](item-pthm-author-048251387164-sequence-closure-and-completeness)

[F6] The real-line distance is $d(x,y)=|x-y|$ and its open balls are $(x-r,x+r)$. A metric has separation, symmetry and the triangle inequality; metric openness is the ball condition and closedness is openness of the complement. Relative topology consists of traces of ambient open sets. [math:lem-real-line-is-a-metric-space](https://alphabetamath.cc/item/lem-real-line-is-a-metric-space) [math:def-metric-space](https://alphabetamath.cc/item/def-metric-space) [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology) [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[F7] In a metric space, a subset is closed if and only if every sequence in it converging in that space has its limit in the subset; the supplier uses countable choice. Work in ZFC, also to choose a section at each term of a parameter sequence. [math:thm-metric-sequential-closure](https://alphabetamath.cc/item/thm-metric-sequential-closure) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F8] An order-convex subset of $\mathbb R$ is connected: it cannot be partitioned into two nonempty sets separated by their ambient closures. A point is in an ambient closure exactly when every real neighborhood meets the set. [math:thm-connected-subsets-of-r-are-intervals](https://alphabetamath.cc/item/thm-connected-subsets-of-r-are-intervals) [math:def-connected-r](https://alphabetamath.cc/item/def-connected-r) [math:thm-closure-characterisations-r](https://alphabetamath.cc/item/thm-closure-characterisations-r)

## Proof

**Given:** The regular construction and the individual admissibility predicate in the Statement.

**Goal:** Prove $\mathcal A=(0,1]$.

1.1 By [F1] and [F3], the actual original closed exterior section $\Sigma_1=C\cup S$ is connected and smooth with boundary $S$, spacelike and maximal for $g$. Since $g_1=g$ on the exterior and near $S$, these properties hold for $g_1$ up to the boundary. The product in [F3] identifies its interior with the zero stationary graph $u_1=0$. The normalized height in [F1] is therefore identically zero, so all its end derivatives through order four vanish. This verifies every admissibility condition in [F2] and gives $1\in\mathcal A$. [F1, F2, F3, given, algebra]

1.2 Fix $0<\varepsilon<1$, set $I=(\varepsilon,1]$ and $B=\mathcal A\cap I$, and equip $I$ with $d_I(x,y)=|x-y|$. The three metric axioms in [F6] restrict from $\mathbb R$ to $I$. Its radius-$r$ balls are $I\cap(x-r,x+r)$. Thus every trace of an ambient open set satisfies the metric ball condition on $I$; conversely, if $U\subseteq I$ satisfies that condition, choose for each $x\in U$ a radius $r_x>0$ with $I\cap(x-r_x,x+r_x)\subseteq U$. The union of these ambient intervals has trace exactly $U$. Hence this metric topology is the relative topology of [F6]. [F6, F7, given, construct]

2.1 For any $q_*\in B$, choose one individually admissible section there. Its hypotheses for [F4] are precisely [F1]–[F2], and $0<\varepsilon<q_*\le1$. Apply [F4] with $\delta=\varepsilon$. The nearby smooth fixed-boundary flow graphs are diffeomorphic to the connected reference section, hence connected; they retain all the graph, maximality, boundary and end conditions in [F2]. Every sufficiently close $q\in I$ therefore belongs to $B$. Thus $B$ is relatively open in $I$, and it is nonempty by step 1.1. [F1, F2, F4, F6, F7, step 1.1, step 1.2, choose]

2.2 Let $(q_j)$ be any sequence in $B$ converging in $(I,d_I)$ to $q_*\in I$. By [F7], choose one admissible section $\Sigma_j$ for each term; these are choices only at parameters already in $\mathcal A$. All $q_j$ lie in $[\varepsilon,1]$ and $q_j\to q_*$ there. Thus [F5] applies on that fixed positive interval and supplies an individually admissible section at $q_*$. It follows that $q_*\in B$. By the metric sequential-closedness theorem in [F7], $B$ is closed in $(I,d_I)$, hence relatively closed by step 1.2. [F2, F5, F7, step 1.2, choose]

3.1 The interval $I$ is order-convex, hence connected by [F8]. To apply its separated-set formulation explicitly, suppose $C=I\setminus B$ were nonempty. Steps 2.1 and 2.2 make both $B$ and $C$ relatively open. For each point of either set, step 1.2 gives an ambient interval whose trace on $I$ avoids the other set. Since both sets lie in $I$, that ambient interval itself avoids the other set. By [F8], no point of $B$ lies in the ambient closure of $C$ and no point of $C$ lies in the ambient closure of $B$. Thus the nonempty sets $B,C$ would disconnect $I$, a contradiction. Consequently $B=I$. Given any $q\in(0,1]$, take $\varepsilon=q/2$ to obtain $q\in\mathcal A$. This proves the full positive-parameter conclusion without assuming an interval-wide family. [F6, F8, step 1.2, step 2.1, step 2.2, algebra] ∎

## Source notes

Radu’s Section 5.3, Lemma 5.1 supplies compact-graph background under its stated boundary, topology, lapse and height hypotheses. The present existence-set argument is a local composition of the declared suppliers; that citation does not establish the indexed noncompact conclusion.

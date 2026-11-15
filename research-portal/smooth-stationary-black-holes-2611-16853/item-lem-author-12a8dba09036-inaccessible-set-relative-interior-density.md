---
title: Inaccessible set is the closure of its relative interior
status: published
research_item: lem-author-12a8dba09036-inaccessible-set-relative-interior-density
dependency_level: 1
sources:
  references:
    - title: P. T. Chruściel, Elements of causality theory
      url: https://arxiv.org/pdf/1110.6706
      locator: §§2.1, 2.3–2.4; Definition 2.1.1, printed p. 4; curve convention p. 16;
        futures/pasts p. 17; Proposition 2.4.2(3), p. 18; Corollary 2.4.11 and
        Proposition 2.4.12, pp. 24–25 (PDF pp. 7, 19–21, 27–28).
      statement: Chronology defined using locally Lipschitz future timelike paths is
        transitive; I^+(S) and I^-(S) are open for every subset S.
      hypotheses: Time-oriented finite-dimensional Lorentzian manifold with C^2
        metric; standard manifold conventions. Applied here to smooth E, in the
        stated ZFC setting.
      reading_limits: Consulted the listed definitions, statements and accompanying
        arguments in the online PDF dated 27 November 2024. Imports only
        chronology and openness; no choice-minimality claim.
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609
      locator: §1.2, p. 6 (dimension convention); §2.3, Remark 2.8, p. 28 (PDF pp. 6,
        28).
      statement: A future causal absolutely continuous curve admits a Lipschitz
        arclength reparametrization, with tangent positively rescaled almost
        everywhere.
      hypotheses: Time-oriented finite-dimensional C^2 Lorentzian manifold, causal
        nonzero tangent almost everywhere, compact parameter interval, auxiliary
        Riemannian metric; ZFC used here.
      reading_limits: Read §1.2 and §2.3 including Remark 2.8. Use only the stated
        parametrization and tangent formula; preservation of timelikeness under
        positive scaling is the local application in Proof 1.1.
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3 — Lorentzian geometry and time orientation
      url: https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609
      locator: §1.2, printed p. 6 (dimension and signature); §1.3, printed p. 7
        (Lorentz scalar product, timelike cones and choice of future); §1.5,
        printed p. 9 (Lorentzian manifold); §1.7, printed pp. 10–11 (continuous
        time orientation). PDF pp. 6–7, 9–11.
      statement: In finite dimension, a Lorentz scalar product has signature
        (-,+,...,+); its timelike vectors form two disjoint open cones,
        distinguished in orthonormal coordinates by the sign of the time
        coordinate. A Lorentzian manifold is a smooth manifold equipped with a
        C^2 metric of that signature. A time orientation is a continuous choice
        of the future cone at each point, equivalently specified by a continuous
        timelike field. The other cone is past.
      hypotheses: Finite-dimensional real tangent spaces with one negative direction;
        smooth Hausdorff second-countable manifold without boundary and a C^2
        Lorentzian metric. Time orientation is assumed given, not asserted to
        exist for every Lorentzian manifold. Applied here to the stipulated
        smooth g and future normal n; no connectedness or noncompactness
        assumption from Definition 1.6 is imported.
      reading_limits: Read the extracted online PDF text of §§1.2–1.3, the
        Lorentzian-manifold definition in §1.5, and the time-orientation
        definitions at the start and end of §1.7. Imports only these geometric
        definitions and the displayed two-cone description, not the covering
        construction, existence theorems or any physical model.
---

## Prerequisites

- [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)
- [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)
- [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)
- [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)
- [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components)
- [` P. T. Chruściel, Elements of causality theory · §§2.1, 2.3–2.4; Definition 2.1.1, printed p. 4; curve convention p. 16; futures/pasts p. 17; Proposition 2.4.2(3), p. 18; Corollary 2.4.11 and Proposition 2.4.12, pp. 24–25 (PDF pp. 7, 19–21, 27–28). `](https://arxiv.org/pdf/1110.6706)
- [` E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22 (2019), article 3 · §1.2, p. 6 (dimension convention); §2.3, Remark 2.8, p. 28 (PDF pp. 6, 28). `](https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609)
- [` E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22 (2019), article 3 — Lorentzian geometry and time orientation · §1.2, printed p. 6 (dimension and signature); §1.3, printed p. 7 (Lorentz scalar product, timelike cones and choice of future); §1.5, printed p. 9 (Lorentzian manifold); §1.7, printed pp. 10–11 (continuous time orientation). PDF pp. 6–7, 9–11. `](https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609)


## Statement

Assume the Axiom of Choice. Let $E=\mathbb R\times C$ be a smooth time-oriented stationary Lorentz manifold with complete time-translation Killing field $T=\partial_t$. Suppose the slices are spacelike and $T=Nn+X$ with stationary extensions of their unit future normal $n$, lapse $N>0$ and shift $X$. Suppose $-X$ has a complete flow $\psi_s$ on $C$. Let $U\subset E$ be a time-translation-invariant open set, $P=I^-_E(U)$, and $B=\{x\in C:(0,x)\notin P\}$. Then $B$ is relatively closed in $C$, and $\psi_s(B)\subset\operatorname{int}_C B$ for every $s>0$. In particular $B=\overline{\operatorname{int}_C B}^{\,C}$.

Here a Killing field means a smooth field with $\mathcal L_Tg=0$. The chronological relation $p\ll q$ means reachability inside $E$ by a locally absolutely continuous curve with future timelike tangent almost everywhere, and $I^-_E(S)=\{p\in E:\exists q\in S,\ p\ll q\}$. These conventions apply in arbitrary finite dimension; the four-dimensional case is included.

## Facts & Assumptions

[A1] The Axiom of Choice is assumed, as in the lapse–shift supplier's convention. It implies Dependent Choice and Countable Choice, meeting the foundational hypotheses of the four-dimensional causal suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F1] Chronology is transitive and chronological futures and pasts are open. The dimension-general inputs are recorded in External input below. In dimension four the existing mathematical interfaces also supply these facts with the choice assumptions in [A1]. [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability) [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness) [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[F2] The unit future normal satisfies $g(n,n)=-1$ and is orthogonal to the slice. The given decomposition yields $N=-g(T,n)$ and $X=T-Nn$ tangent to the slice. These are the lapse–shift formulas of the four-dimensional interface, and their displayed algebra is dimension independent. Complete smooth flows are smooth and satisfy the flow law. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F3] The Lie derivative is defined by differentiation of pullback along a flow; vanishing Lie derivative implies tensor invariance on each common flow domain. This applies to a Lorentzian metric as a smooth covariant two-tensor in any dimension. The inline Killing-field convention agrees in dimension four with the Lorentzian definition. [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field) [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes) [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[F4] Relative open and closed sets use the subspace topology. Interior is the largest open subset and closure is the smallest closed superset. [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top) [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

[F5] Smooth manifolds carry their smooth structures given by maximal smooth atlases. The product $E=\mathbb R\times C$ carries the product topology and canonical product smooth structure: product charts pair the standard real coordinate with a smooth chart on $C$. Basic product-open sets are rectangles, and product projections are continuous. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology) [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[F6] A smooth Lorentz metric is a smooth symmetric nondegenerate covariant two-tensor of signature $(-,+,\ldots,+)$. Its timelike vectors satisfy $g(v,v)<0$ and form two open cone components. A time orientation continuously chooses one as future, with the other past. These dimension-general geometric inputs are recorded in External input below. In dimension four they agree with the existing mathematical geometry definition and cone lemma. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components)

## External input

The imported chronology input [Chruściel, §§2.3–2.4](https://arxiv.org/pdf/1110.6706) supplies [F1] for locally Lipschitz paths in arbitrary finite dimension. The parametrization input [Minguzzi, Remark 2.8](https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609) connects it to the curve convention in the Statement. The geometric input [Minguzzi, §§1.2–1.3, 1.5 and 1.7](https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609) supplies the dimension-general Lorentzian and time-orientation conventions and two-cone description in [F6]. Exact claims, hypotheses and consulted passages are recorded in the three source references. The inaccessible-set conclusion is proved locally below.

## Proof

**Given:** The hypotheses and conventions in the Statement.

**Goal:** Prove relative closedness, the forward interior inclusion and the closure identity.

1.1 Under [A1], use the dimension-general inputs in External input as follows. A curve with future timelike tangent almost everywhere is a causal absolutely continuous curve, so Minguzzi's arclength reparametrization applies. Its tangent is a positive multiple of the old tangent almost everywhere, hence remains future timelike. Conversely a locally Lipschitz timelike path is locally absolutely continuous. Thus the two conventions give the same chronological relation, and Chruściel's transitivity and openness apply to it. In dimension four the existing causal suppliers give the same conclusions with their choice hypotheses satisfied. [given, A1, F1]

1.2 For $x\in B$ consider $\gamma_x(s)=(s,\psi_sx)$. Completeness keeps $\psi_sx$ in $C$ at every finite parameter. The flow equation for $-X$ and stationarity give $\gamma_x'=T-X=Nn$. Therefore $g(\gamma_x',\gamma_x')=-N^2<0$ and $\gamma_x'$ is future directed. On each finite parameter interval the image is compact and the continuous lapse has a positive minimum, though no global uniform lower bound is required. In particular $(0,x)\ll(s,\psi_sx)$ for every $s>0$. [given, F2, F5, F6]

2.1 Write $\Phi_a(t,x)=(t+a,x)$ for the complete flow of $T$. Since $\mathcal L_Tg=0$, tensor-flow invariance gives $\Phi_a^*g=g$ for every $a$. By [F6], these isometries preserve time orientation: for a future timelike vector $v$, $d\Phi_a(v)$ remains timelike as $a$ varies continuously from zero, so cannot cross to the other component of the timelike cones. Applying $\Phi_a$ and $\Phi_{-a}$ to timelike curves, and using $\Phi_a(U)=U$, gives $\Phi_a(P)=P$ and $\Phi_a(A)=A$ for $A=E\setminus P$. Openness of $P$ makes $A$ closed. The product identification $\iota_t:C\to\{t\}\times C$, $\iota_t(x)=(t,x)$, is a homeomorphism onto the slice with its subspace topology: its inverse is the restricted product projection. Hence $B=\iota_0^{-1}(A)$ is closed in $C$. Finally, if $a\in A$ and $a\ll b\in P$, there is $u\in U$ with $b\ll u$; transitivity gives $a\ll u$, a contradiction. Thus $I^+_E(a)\subset A$ for $a\in A$. [given, F3, F4, F5, F6, step 1.1]

3.1 By step 2.1, the open set $I^+_E((0,x))$ is contained in $A$. For $s>0$, its intersection with the slice $t=s$ contains $(s,\psi_sx)$ by step 1.2 and is relatively open. Pulling that intersection back by $\iota_s$, or equivalently translating by $-s$ and using $\iota_0$, gives an open neighborhood of $\psi_sx$ contained in $B$, by translation invariance of $A$. Thus $\psi_s(B)\subset\operatorname{int}_CB$. For $x\in B$, smoothness of the flow gives $\psi_sx\to x$ as $s\downarrow0$. Every neighborhood of $x$ therefore meets $\operatorname{int}_CB$, so $x$ belongs to its closure: indeed no closed superset of that interior can omit $x$, since its open complement would then be such a neighborhood. This proves $B\subset\overline{\operatorname{int}_CB}^{\,C}$. Closedness of $B$ gives the reverse inclusion. [F2, F4, step 1.1, step 2.1, step 1.2] ∎

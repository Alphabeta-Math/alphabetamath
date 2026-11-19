---
title: Spherical lines for unitary split projective factors
status: published
research_item: lem-author-c3a9b9243c74-projective-local-spherical-line
dependency_level: 6
---

## Prerequisites

- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:def-locally-compact-space](https://alphabetamath.cc/item/def-locally-compact-space)
- [math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra)
- [math:def-sigma-algebra](https://alphabetamath.cc/item/def-sigma-algebra)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-dimension](https://alphabetamath.cc/item/def-dimension)
- [math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis)
- [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)
- [def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)
- [math:def-hilbert-space](https://alphabetamath.cc/item/def-hilbert-space)
- [math:def-left-haar-integral-and-left-haar-measure](https://alphabetamath.cc/item/def-left-haar-integral-and-left-haar-measure)
- [lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)
- [math:cor-existence-of-left-and-right-haar-measures](https://alphabetamath.cc/item/cor-existence-of-left-and-right-haar-measures)
- [math:lem-haar-measure-is-positive-on-nonempty-open-sets-and-finite-on-compact-sets](https://alphabetamath.cc/item/lem-haar-measure-is-positive-on-nonempty-open-sets-and-finite-on-compact-sets)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)
- [def-author-5b8600b4f4af-split-unramified-quaternion-representation](item-def-author-5b8600b4f4af-split-unramified-quaternion-representation)
- [def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)
- [thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character)
- [math:def-measure](https://alphabetamath.cc/item/def-measure)
- [math:def-radon-measure-on-an-lch-space](https://alphabetamath.cc/item/def-radon-measure-on-an-lch-space)
- [math:def-nonnegative-extended-series](https://alphabetamath.cc/item/def-nonnegative-extended-series)
- [math:def-extended-reals](https://alphabetamath.cc/item/def-extended-reals)
- [math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top)
- [math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)


## Statement

Assume the Axiom of Choice. Let $B$ be the rational Hamilton quaternion algebra and put $B_\ell=B\otimes_{\mathbb Q}\mathbb Q_\ell$. Let $\ell$ be a split prime, so $B_\ell$ admits a $\mathbb Q_\ell$-algebra isomorphism to the two-by-two matrices over $\mathbb Q_\ell$. Choose such an isomorphism and use it to identify $G(\mathbb Q_\ell)=B_\ell^\times/\mathbb Q_\ell^\times$ with $\mathrm{PGL}_2(\mathbb Q_\ell)$, the group of invertible matrices modulo nonzero scalar matrices. Let $K_\ell=\mathrm{GL}_2(\mathbb Z_\ell)$ and let $J_\ell$ be its compact open projective image. Let $\rho$ be a strongly continuous unitary representation of the projective group on a complex Hilbert space $V$. Suppose the smooth vectors of its lift to $\mathrm{GL}_2(\mathbb Q_\ell)$ form an irreducible admissible representation. Smooth means fixed by some open subgroup. Irreducible here means nonzero with no proper nonzero invariant linear subspace. Admissibility means that fixed spaces for compact open subgroups are finite dimensional.

If $V^{J_\ell}\ne0$, the representation is called unramified and $V^{J_\ell}$ is a one-dimensional spherical line. The spherical Hecke algebra consists of compactly supported complex functions invariant under left and right multiplication by $J_\ell$, with convolution for a left Haar measure giving $J_\ell$ mass one. Such a measure exists. On the spherical line its operators act by a character, a unital complex-algebra homomorphism to $\mathbb C$.

## Facts & Assumptions

[A1] The Axiom of Choice supplies choice functions for indexed families of nonempty sets and implies Countable Choice. Use the Axiom of Choice for the split compactness assertion and for existence of left Haar measure. Use Countable Choice for the matrix and quotient group result and for the degree-two theorem ([math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice), [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)).

[F1] The split identification is a topological isomorphism, and $J_\ell$ is its compact open subgroup corresponding to the image of $K_\ell$. The projection from the invertible matrix group to the projective group is continuous and onto. A strongly continuous unitary action has norm-continuous vector orbit maps and acts by bijective complex-linear isometries ([def-author-5b8600b4f4af-split-unramified-quaternion-representation](item-def-author-5b8600b4f4af-split-unramified-quaternion-representation), [math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)).

[F2] A vector is smooth if it is fixed by some open subgroup. For a strongly continuous unitary representation of $\mathrm{GL}_2(\mathbb Q_\ell)$ whose smooth vectors are irreducible and admissible, when the $K_\ell$-fixed space is nonzero it is one dimensional under Countable Choice ([thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character)).

[F3] For a compact open subgroup $J$ in a Hausdorff topological group, each translate $xJ$ is a compact open neighborhood of $x$. The unit in the spherical Hecke algebra is the indicator of $J$. Its action on fixed vectors is the unital algebra action $T_fv=\sum_{xJ} f(x)\rho(x)v$. Each $xJ=\{xj:j\in J\}$ is counted once, and only finitely many cosets have nonzero terms by compact support and openness. The algebra multiplication is left Haar convolution when the measure assigns $J$ mass one ([def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra), Definition and Justification steps 1.1, 2.2, 4.1, 5.1, 6.1 and 7.1).

[F4] Under Countable Choice, $\mathrm{GL}_2(\mathbb Q_\ell)$ and its quotient by the scalar matrices are Hausdorff topological groups in the matrix-entry and scalar quotient topologies, respectively. The subgroup $K_\ell$ and its projective image are compact and open ([lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)).

[F5] Under the Axiom of Choice, a locally compact Hausdorff group admits a left Haar measure ([math:cor-existence-of-left-and-right-haar-measures](https://alphabetamath.cc/item/cor-existence-of-left-and-right-haar-measures)). This measure is positive on nonempty open sets and finite on compact sets ([math:lem-haar-measure-is-positive-on-nonempty-open-sets-and-finite-on-compact-sets](https://alphabetamath.cc/item/lem-haar-measure-is-positive-on-nonempty-open-sets-and-finite-on-compact-sets)). A left Haar measure is a nonzero left-invariant Borel measure that is finite on compact sets, outer regular on Borel sets and inner regular on open sets ([math:def-left-haar-integral-and-left-haar-measure](https://alphabetamath.cc/item/def-left-haar-integral-and-left-haar-measure)).

[F6] A unital ring homomorphism preserves addition, multiplication and the multiplicative identity ([math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)). A homomorphism of unital complex algebras is a unital ring homomorphism that intertwines the two scalar structure maps ([math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)).

[F7] A finite-dimensional complex vector space has a finite basis, and dimension one means that such a basis has one element ([math:def-dimension](https://alphabetamath.cc/item/def-dimension)). A basis spans the space and is linearly independent ([math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis)).

[F8] A measure vanishes on the empty set and assigns a countable disjoint union the nonnegative extended sum of the individual measures ([math:def-measure](https://alphabetamath.cc/item/def-measure)). The finite partial sums start at zero and each successor adds the next term. A nonnegative extended sum is the supremum of its finite partial sums ([math:def-nonnegative-extended-series](https://alphabetamath.cc/item/def-nonnegative-extended-series)).

[F9] Outer regularity gives the measure of a Borel set as the infimum over open supersets. Inner regularity on an open set gives its measure as the supremum over compact subsets ([math:def-radon-measure-on-an-lch-space](https://alphabetamath.cc/item/def-radon-measure-on-an-lch-space)). For positive finite $c$, multiplication by $c$ on $[0,+\infty]$ uses ordinary real multiplication at finite values and sends $+\infty$ to $+\infty$ ([math:def-extended-reals](https://alphabetamath.cc/item/def-extended-reals)).

[F10] A map of topological spaces is continuous exactly when preimages of open sets are open ([math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top), conditions (a) and (b)).

[F11] A subset is compact when every open cover in its subspace topology has a finite subcover ([math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)). A space is locally compact when every point has a compact neighborhood ([math:def-locally-compact-space](https://alphabetamath.cc/item/def-locally-compact-space)).

[F12] The Borel sigma-algebra is generated by the open sets, so it contains every open set ([math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra)). A sigma-algebra contains the empty set and is closed under countable unions ([math:def-sigma-algebra](https://alphabetamath.cc/item/def-sigma-algebra)).

[F13] A property holds at every natural number if it holds at zero and passes from each number to its successor ([math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)).

## Proof

**Given:** The Axiom of Choice, the split group, and the strongly continuous unitary action $\rho$ with the specified hypotheses on its lift.

**Goal:** Normalize left Haar measure and show that a nonzero fixed space is a line on which the Hecke action is a character.

1.1 By [A1] and [F4] the matrix scalar quotient is Hausdorff, so by [F1] the split projective group $G(\mathbb Q_\ell)$ is Hausdorff. For each $x$ in this group the translate $xJ_\ell$ is a compact open neighborhood by [F3], so the group is locally compact by [F11]. Obtain a left Haar measure $\mu$ by [A1] and [F5]. The subgroup $J_\ell$ is open by [F1] and hence Borel by [F12]. It contains the identity and is compact by [F1], so $0<\mu(J_\ell)<\infty$ by [F5]. Put $c=1/\mu(J_\ell)$ and define $\nu(E)=c\mu(E)$ on the Borel sigma-algebra. Multiplication by $c$ on $[0,+\infty]$ preserves order and has the order-preserving inverse given by multiplication by $1/c$. It therefore sends upper and lower bounds to upper and lower bounds bijectively, preserving suprema and infima. For nonnegative extended numbers $a,b$, the identity $c(a+b)=ca+cb$ follows from real distributivity if both are finite, and both sides are $+\infty$ if either is infinite. For a pairwise disjoint sequence of Borel sets $E_k$, the union is Borel by [F12]. Both initial partial sums are zero. If the partial sum of the first $n$ values $\nu(E_k)$ is $c$ times the corresponding partial sum of $\mu(E_k)$, the same holds for $n+1$ by the recurrence in [F8] and $c(a+b)=ca+cb$. Thus the scaling identity holds at every index by [F13]. Taking their suprema and using countable additivity of $\mu$ gives countable additivity of $\nu$. The empty set is Borel by [F12], and $\nu(\varnothing)=c\mu(\varnothing)=0$. Hence $\nu$ is a Borel measure by [F8]. Multiplication by $c$ preserves the infimum over open supersets of each Borel set and the supremum over compact subsets of each open set, giving outer and inner regularity in the required domains. Left invariance and finiteness on compact sets follow from those of $\mu$. Finally, $\nu(J_\ell)=1$, so $\nu$ is nonzero and is the required left Haar measure. [A1, F1, F3, F4, F5, F8, F9, F11, F12, F13, given]

1.2 Suppose $V^{J_\ell}\ne 0$. Write $q:\mathrm{GL}_2(\mathbb Q_\ell)\to G(\mathbb Q_\ell)$ for the continuous projective quotient homomorphism from [F1]. The lift $\rho\circ q$ acts by the same complex-linear isometries as $\rho$. For $v\in V$, write $\omega_v(x)=\rho(x)v$. If $U$ is open in the norm topology of $V$, then $(\omega_v\circ q)^{-1}[U]=q^{-1}[\omega_v^{-1}[U]]$ is open by [F1] and [F10]. Thus $\rho\circ q$ is strongly continuous on the same complex Hilbert space $V$. A vector is fixed by $K_\ell$ for this lift exactly when it is fixed by $J_\ell$ for $\rho$, because $K_\ell$ maps onto $J_\ell$. Since $K_\ell$ is open by [F4], these vectors are smooth for the lift by the smooth-vector criterion in [F2]. The smooth vectors give an irreducible admissible representation by hypothesis, the $K_\ell$-fixed space is nonzero, and [A1] gives Countable Choice. Hence the fixed space is one dimensional by [F2]. [A1, F1, F2, F4, F10, given]

2.1 The volume-one measure from step 1.1 identifies Hecke multiplication with the specified convolution by [F3]. By the same fact the projective Hecke operators preserve this line and give a unital algebra action on it. By [F7] and step 1.2, take a basis $\{w\}$ of $V^{J_\ell}$. Since the basis spans the line and is linearly independent, each vector has a unique expression $aw$ with $a\in\mathbb C$. In particular, write $T_fw=\lambda(f)w$ with $\lambda(f)\in\mathbb C$ unique. By complex linearity, $T_f(aw)=aT_fw=\lambda(f)(aw)$ for every $a\in\mathbb C$. From the algebra action, $T_{f+h}w=(\lambda(f)+\lambda(h))w$, $T_{f*h}w=T_f(T_hw)=\lambda(f)\lambda(h)w$ and $T_{\mathbf 1_{J_\ell}}w=w$. Their unique coefficients show that $\lambda$ preserves addition, multiplication and the unit, so it is a unital ring homomorphism by [F6]. The scalar map of the Hecke algebra sends $c$ to $c\mathbf 1_{J_\ell}$, and $\lambda(c\mathbf 1_{J_\ell})=c$ by complex linearity and unitality of the action. Thus $\lambda$ respects the scalar structure maps and is a unital complex-algebra homomorphism by [F6]. [F3, F6, F7, step 1.1, step 1.2] ∎

---
title: Hawking horizon generator and analytic global rigidity
status: draft
research_item: pthm-hawking-horizon-generator
dependency_level: 5
sources:
  references:
    - title: S. Alexakis, A. D. Ionescu and S. Klainerman, Hawking’s local rigidity
        theorem without analyticity
      url: https://arxiv.org/pdf/0902.1173v1
      locator: §1 Theorems 1.1–1.2, pp.1–2; §2 affine null setup, pp.4–5; Proposition
        3.1 and (3.1), p.7; §4 extension and §5 Propositions 5.1–5.2
      statement: Under the local regular bifurcate non-expanding horizon hypotheses in
        a connected oriented smooth four-dimensional vacuum spacetime, the
        constructed Hawking field extends as a Killing field to a full
        neighborhood of the sphere. Its horizon data are K=underline(u)L−u
        underline(L), with affine generators and zero parameters on the sphere.
        An additional branch-tangent Killing field T not identically zero on the
        sphere commutes with K, and Z=T+lambda_0 K is a nontrivial periodic
        rotational Killing field.
      hypotheses: Exactly the regular achronal null causal branches generated
        orthogonally from an embedded spacelike two-sphere, with both expansions
        zero, Ric(g)=0 and the additional T hypotheses for rotation. On one
        branch u=0 and underline(u) is its affine parameter; on the other
        underline(u)=0 and u is its affine parameter.
      reading_limits: Consulted the retrieved arXiv v1 PDF text at Theorems 1.1–1.2,
        the neighborhood-shrinking convention and affine setup in §2,
        Proposition 3.1 and equation (3.1), the §4 extension statements and §5
        Propositions 5.1–5.2. A PDF screenshot attempt failed; this pass claims
        no visual inspection. The characteristic PDE, unique-continuation and
        periodicity proofs were not reconstructed. The existing local-rigidity
        supplier and its canonical horizon data are used only on a suitably
        restricted neighborhood.
    - title: P. T. Chruściel and J. L. Costa, On uniqueness of stationary vacuum black
        holes
      url: https://arxiv.org/html/0806.0016v2
      locator: Corollary 2.4; §2.3.1 equation (2.13); Theorem 4.14, Remark 4.15 and
        its extension/completeness paragraph; §7.1
      statement: A globally hyperbolic asymptotically flat domain of outer
        communications satisfying the null energy condition is simply connected.
        Under all hypotheses of Theorem 4.14, a rotating analytic horizon has
        global complete commuting periodic Killing fields on the exterior union
        the horizon component; in four dimensions the ensuing symmetry is
        R×U(1), as stated in §7.1.
      hypotheses: Analytic, asymptotically flat, strongly causal vacuum spacetime,
        complete stationary T, globally hyperbolic exterior, compact horizon
        cross-section A⊂I+(M_ext), either nonzero mean surface gravity from
        (2.13) or periodic induced T-flow on generator space, and either strong
        causality of closure(D)∩I+(M_ext) or an asymptotically flat spacelike
        exterior hypersurface achronal in D with completed boundary A in E+.
        Rotation means T is not tangent to the null generators.
      reading_limits: Consulted the retrieved arXiv:0806.0016v2 HTML at Corollary 2.4,
        §2.3.1 equations (2.12)–(2.13), Theorems 4.13–4.14, Remark 4.15, the
        adjoining extension/completeness paragraph and §7.1. Checked their
        applicability to the explicit global hypotheses; no
        topological-censorship, analytic-rigidity, asymptotic Killing-vector or
        completeness proof was reconstructed.
    - title: "P. T. Chruściel, J. L. Costa and M. Heusler, Stationary Black Holes:
        Uniqueness and Beyond"
      url: https://arxiv.org/pdf/1205.6112
      locator: §3.4.2 Rigidity without analyticity, PDF p.20, first paragraph
      statement: The locally defined near-horizon Killing vector extends to the whole
        domain of outer communications using analyticity, Nomizu’s continuation
        theorem, and simple connectedness of I+-regular domains of outer
        communications.
      hypotheses: A local Killing field on a connected nonempty open collar in an
        analytic simply connected exterior. The continuation is of that field,
        rather than an assertion that separately obtained horizon generators
        have already been normalized identically.
      reading_limits: Consulted the retrieved PDF text at §3.4.2, PDF p.20, first
        paragraph and its surrounding local/global rigidity discussion. This
        imports continuation on the analytic simply connected exterior. The
        original Nomizu paper was not read, and no proof of continuation or
        analytic regularity of Killing fields was reconstructed.
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p.2 §1.1; pp.3–4 Definition 1.1; p.11 §2.4
      reading_limits: Read the frozen article text at these passages for attribution
        and matching its local horizon conventions. This reference supplies no
        independent proof of a prerequisite.
---

PDF p. 2: ` §1.1, Hawking rigidity discussion `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair)
- [thm-local-bifurcate-rigidity-input](item-thm-local-bifurcate-rigidity-input)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity)
- [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data)
- [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)
- [lem-author-9a15bef58785-affine-generator-zero-locus](item-lem-author-9a15bef58785-affine-generator-zero-locus)
- [lem-author-9a15bef58785-affine-generator-acceleration](item-lem-author-9a15bef58785-affine-generator-acceleration)
- [lem-author-9a15bef58785-killing-acceleration-covector](item-lem-author-9a15bef58785-killing-acceleration-covector)
- [lem-author-9a15bef58785-exact-killing-horizon-jets](item-lem-author-9a15bef58785-exact-killing-horizon-jets)
- [lem-author-9a15bef58785-rotational-rescaling-and-commutation](item-lem-author-9a15bef58785-rotational-rescaling-and-commutation)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Hawking’s local rigidity theorem without analyticity · §1 Theorems 1.1–1.2, pp.1–2; §2 affine null setup, pp.4–5; Proposition 3.1 and (3.1), p.7; §4 extension and §5 Propositions 5.1–5.2 `](https://arxiv.org/pdf/0902.1173v1)
- [` P. T. Chruściel and J. L. Costa, On uniqueness of stationary vacuum black holes · Corollary 2.4; §2.3.1 equation (2.13); Theorem 4.14, Remark 4.15 and its extension/completeness paragraph; §7.1 `](https://arxiv.org/html/0806.0016v2)
- [` P. T. Chruściel, J. L. Costa and M. Heusler, Stationary Black Holes: Uniqueness and Beyond · §3.4.2 Rigidity without analyticity, PDF p.20, first paragraph `](https://arxiv.org/pdf/1205.6112)


## Statement

Adopt the four-dimensional stationary vacuum model of [post-stationary-vacuum-model](item-post-stationary-vacuum-model). For the smooth local conclusion, assume the regular bifurcate non-expanding horizon pair $(S,H_+,H_-)$ of [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair) in a connected oriented neighborhood $O$, with $T$ tangent to both branches. A smooth Hawking Killing field $K_0$ exists on a possibly smaller open neighborhood $U\subseteq O$ of $S$. For every local conclusion below, replace $H_\pm$ by $H_\pm\cap U$ and retain the same notation. It may be chosen with affine horizon profiles $K_0=sL_+$ on $H_+$ and $K_0=-tL_-$ on $H_-$, where the generators are nonzero and affine, $s=t=0$ at $S$, $L_+(s)=L_-(t)=1$, and the zero sets of the branch parameters are exactly $S$. For any constant $c>0$, the field $K=cK_0$ is nonzero on $(H_+\cup H_-)\setminus S$ and zero on $S$. It is Killing to every order along both branches. Its signed surface gravities are $c$ and $-c$ on the two nonzero branch parts, with the common nonnegative magnitude $\kappa=c$; the future branch has coefficient $c$ under this labeling. A numerical value therefore requires the chosen scale. These statements do not assign a coefficient by the acceleration equation at a zero of $K$.

If additionally $T|_S\not\equiv0$ (the local rotating symmetry hypothesis), after possibly shrinking $U$ again and restricting both branches and $K_0$ accordingly, the source construction yields $[T,K_0]=0$ and a nontrivial periodic rotational Killing field $Z=T+\lambda_0K_0$ near $S$, commuting with $T$ and $K_0$. The condition means not identically zero on the sphere, not nowhere zero there.

For global analytic rigidity, use the precise comparison data of [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data) and impose all hypotheses in the following paragraph. Let $M$ be analytic, asymptotically flat, strongly causal and vacuum, with complete stationary $T$, and let its connected exterior $D$ be globally hyperbolic. A connected future-horizon component has a compact cross-section $A\subset I_M^+(M_{\rm ext})$. Assume either nonzero mean surface gravity or periodic induced $T$-flow on the generator space. The mean is the source's pre-rigidity quantity: in Gaussian null coordinates $g=r\varphi\,dv^2+2\,dv\,dr+2rh_a\,dx^a\,dv+h_{ab}\,dx^a\,dx^b$, it is $\langle\kappa\rangle_A=-|A|^{-1}\int_A\varphi\,d\mu_h$, with $d\mu_h$ the volume measure of the section metric and $|A|$ its volume. Also assume either strong causality of $\overline D\cap I_M^+(M_{\rm ext})$, or an asymptotically flat spacelike hypersurface in $D$, achronal in $D$, whose completed boundary is $A\subset\mathcal E^+$. Require that $T$ is not tangent to the generators of that component. These are the full alternatives of Chruściel–Costa Theorem 4.14, not consequences asserted from the local bifurcate data. In four-dimensional $I^+$-regular applications its Remark 4.15 supplies the periodic-generator alternative.

Under these analytic global hypotheses, the restriction of the chosen local $K$ to any connected nonempty exterior collar extends to a Killing field on all $D$. In addition the exterior is stationary axisymmetric, with a global complete periodic rotational Killing field commuting with $T$. The continuation is of the chosen local field; its scale is retained. No identification of separately normalized source generators is assumed. Smooth local rigidity by itself asserts no global extension.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair)

[thm-local-bifurcate-rigidity-input](item-thm-local-bifurcate-rigidity-input)

[def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity)

[def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data)

[def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[lem-author-9a15bef58785-affine-generator-zero-locus](item-lem-author-9a15bef58785-affine-generator-zero-locus)

[lem-author-9a15bef58785-affine-generator-acceleration](item-lem-author-9a15bef58785-affine-generator-acceleration)

[lem-author-9a15bef58785-killing-acceleration-covector](item-lem-author-9a15bef58785-killing-acceleration-covector)

[lem-author-9a15bef58785-exact-killing-horizon-jets](item-lem-author-9a15bef58785-exact-killing-horizon-jets)

[lem-author-9a15bef58785-rotational-rescaling-and-commutation](item-lem-author-9a15bef58785-rotational-rescaling-and-commutation)

## Facts & Assumptions

[F1] The physical premise is precisely the adopted vacuum/stationarity model; its equations are conditional model assumptions, not observations. [post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[F2] The pre-rigidity pair fixes the regular null branches without assuming a Killing generator. The existing local-rigidity input supplies a Hawking field on a possibly smaller full neighborhood of $S$ and, under $T|_S\not\equiv0$, the commuting periodic combination on a further such neighborhood if necessary. All local branch conclusions are restricted to the chosen neighborhood. Its exact canonical horizon data are the first independent import below. [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair) [thm-local-bifurcate-rigidity-input](item-thm-local-bifurcate-rigidity-input)

[F3] The five local helpers determine the zero locus, branch accelerations, equivalent covector equation, all-order Killing property, and the distinction between periodic and generator normalizations. [lem-author-9a15bef58785-affine-generator-zero-locus](item-lem-author-9a15bef58785-affine-generator-zero-locus) [lem-author-9a15bef58785-affine-generator-acceleration](item-lem-author-9a15bef58785-affine-generator-acceleration) [lem-author-9a15bef58785-killing-acceleration-covector](item-lem-author-9a15bef58785-killing-acceleration-covector) [lem-author-9a15bef58785-exact-killing-horizon-jets](item-lem-author-9a15bef58785-exact-killing-horizon-jets) [lem-author-9a15bef58785-rotational-rescaling-and-commutation](item-lem-author-9a15bef58785-rotational-rescaling-and-commutation)

[F4] Bifurcate-horizon and rotation/degeneracy terminology use signed branch coefficients, with explicit qualifications at the zero field. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data) [def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity)

[F5] Analyticity, stationary completeness, asymptotic flatness, exterior causality and the $I^+$-regularity/circle-action conventions are those of the comparison and periodic-action interfaces. [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data) [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[F6] The second independent import supplies exterior simple connectedness and analytic global rotational symmetry under the explicitly stated global hypotheses. The third supplies continuation of the chosen local Killing field using analyticity and simple connectedness.

## External input

AIK Theorem 1.1, Proposition 3.1 and its equation (3.1), with the affine setup of §2 and extension in §4, supply a full-neighborhood Killing field having the stated affine branch profiles. Their Theorem 1.2 and §5 supply the commuting periodic combination under the additional branch-tangent, nontrivial-on-the-sphere symmetry hypothesis. These are independent existence and extension inputs, not a local reconstruction of the characteristic PDE argument.

Chruściel–Costa Corollary 2.4 supplies simple connectedness of the globally hyperbolic asymptotically flat vacuum exterior, since vacuum satisfies the null energy condition. Their Theorem 4.14, Remark 4.15 and §7.1 supply global complete periodic rotational symmetry under all global hypotheses written in the Statement; no inference of those hypotheses from an arbitrary smooth null horizon is made.

Chruściel–Costa–Heusler §3.4.2 supplies analytic continuation of the near-horizon Killing field throughout the simply connected analytic exterior by Nomizu's theorem. This is a source-supported continuation input for the very same local field on its exterior collar; the original Nomizu theorem is not claimed to have been read or reproved here.

## Proof

**Given:** The hypotheses and data in the Statement.

**Goal:** Establish the stated conclusions with the indicated normalization and scope.

1.1 Under [F1] and the local regular non-expanding hypotheses, apply [F2] and the first independent import to obtain the canonical $K_0$ on a possibly smaller open neighborhood $U\subseteq O$ of $S$. Replace each branch by $H_\pm\cap U$ and restrict its generator and affine parameter, retaining the same notation. The affine parameter zero loci and source profiles place both branches in the hypotheses of the first two helpers in [F3]. Hence $K=cK_0$ is nonzero exactly off $S$ on the branches, and has signed acceleration coefficients $c$ and $-c$. The third helper converts them to the ambient surface-gravity covector equations. This supplies a constant positive future coefficient after the stated branch and positive scale choices. [F1, F2, F3, F4]

2.1 Because $K_0$ is Killing on the open neighborhood $U$, the fourth helper gives every order of the Killing condition along the restricted branches. Under the additional $T|_S\not\equiv0$ hypothesis, shrink $U$ further if needed and restrict both branches and $K_0$ accordingly; on this common neighborhood the source supplies $[T,K_0]=0$ and a periodic $Z=T+\lambda_0K_0$. The fifth helper gives the remaining commutators and, if desired, rescales $Z$ to period $2\pi$. This does not conflate the period normalization of $Z$ with the scale of $K$. [F2, F3, F4, step 1.1]

2.2 In the analytic global case, the vacuum equation implies $\operatorname{Ric}(Y,Y)=0\ge0$ for each null vector $Y$, so the second import gives simple connectedness of $D$. Analyticity and the third import therefore continue the restriction of our chosen local $K$ from its connected exterior collar to all $D$. This is an extension of that actual restriction; no matching to a separately constructed generator is used. [F1, F5, F6, step 1.1]

3.1 The same analytic global hypotheses are precisely the hypotheses of the second import's Theorem 4.14. Its global complete commuting periodic fields, in dimension four as stated in §7.1, give the claimed stationary axisymmetry. This global conclusion uses the displayed causality/cross-section alternatives; the earlier smooth local conclusion did not assert them or a global extension. Together these establish the reported smooth and analytic rigidity assertions with their actual normalization and domains. [F5, F6, step 2.1, step 2.2] ∎

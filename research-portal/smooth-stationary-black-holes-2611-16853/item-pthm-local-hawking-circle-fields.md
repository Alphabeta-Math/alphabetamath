---
title: Local Hawking and axial fields, boost and pole
status: draft
research_item: pthm-local-hawking-circle-fields
dependency_level: 7
sources:
  references:
    - title: S. Alexakis, A. D. Ionescu and S. Klainerman, Hawking’s local rigidity
        theorem without analyticity
      url: https://arxiv.org/pdf/0902.1173v1
      locator: §1 Theorems 1.1–1.2, pp.1–2; §2 affine null setup, pp.4–5, (2.1)–(2.4);
        Proposition 3.1, p.7, (3.1); §4 extension, pp.10–11 and conclusion p.15;
        §5 Propositions 5.1–5.2, pp.16–17
      statement: For a local regular bifurcate non-expanding horizon pair in a
        connected oriented smooth four-dimensional Ricci-flat spacetime, AIK
        constructs a field K0 with K0=underline(u)L on N and K0=-u underline(L)
        on underline(N), using future affine generators with
        L(underline(u))=underline(L)(u)=1 and both parameters zero on S. The
        field extends as a Killing field to a full neighborhood. For a Killing
        field T tangent to both branches and not identically zero on S, [T,K0]=0
        and Z0=T+lambda0 K0 has a common positive period on a smaller
        neighborhood.
      hypotheses: Embedded spacelike two-sphere; regular achronal null sheets
        generated orthogonally from S and forming its local causal boundary;
        both sheets non-expanding; Ric(g)=0; connected oriented smooth
        four-dimensional spacetime. The source null pair is future directed with
        g(L,underline(L))=-1 on S, parallel transported along the respective
        generators; its affine parameters vanish on S. The rotational conclusion
        additionally requires T Killing, tangent to both sheets and not
        identically zero on S. Assigning N to the event branch H+ and
        underline(N) to H- is the local application convention justified by the
        axis supplier, not an extra source hypothesis.
      reading_limits: "For this adjudication read the retained arXiv:0902.1173v1 PDF
        at pp.1–2,4–5,7,10–11,15–17: setup, theorem statements, affine data
        (3.1), extension construction/conclusion and commutation/periodicity
        statements. Visually inspected pp.5 and 7 to distinguish underlined
        symbols; the source HTML was also consulted. Did not reconstruct the
        characteristic PDE, unique-continuation or sphere-periodicity proofs.
        The event-branch identification, eigenvalue calculation and positive
        coefficient are local applications of these data and the existing
        suppliers, not additional assertions attributed to AIK."
    - title: A. F. Radu, Rigidity of stationary black holes with small ADM angular
        momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: §3.2 equation (3.9); Appendix A.1 equation (A.1)
      reading_limits: Read the independent source normalization discussion and local
        identity kappa=nu(n)>0 at a circle fixed point, together with its
        reference to the maximal-lapse boundary derivative. These passages guide
        the local method; the whole GR/SBS theorem is not imported or asserted
        applicable wholesale.
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp.8,11,28; §2.1, §2.4 and §5 opening
      reading_limits: Read frozen original-article passages for attribution and
        preservation of its claimed normalization, circle pole and signed
        horizon equations. This is ordinary attribution only, not independent
        proof of a prerequisite.
---

PDF p. 8: ` §2.1 pole; §2.4 local rigidity; §5 opening `; PDF p. 11: ` §2.1 pole; §2.4 local rigidity; §5 opening `; PDF p. 28: ` §2.1 pole; §2.4 local rigidity; §5 opening `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product)
- [lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)
- [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair)
- [thm-local-bifurcate-rigidity-input](item-thm-local-bifurcate-rigidity-input)
- [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity)
- [lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [lem-author-ca4ffba327b3-event-boundary-generator-data](item-lem-author-ca4ffba327b3-event-boundary-generator-data)
- [lem-author-ca4ffba327b3-stationary-product-excludes-zero-coefficient](item-lem-author-ca4ffba327b3-stationary-product-excludes-zero-coefficient)
- [lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action](item-lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action)
- [lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost](item-lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost)
- [lem-author-ca4ffba327b3-normalized-boost-from-positive-lapse](item-lem-author-ca4ffba327b3-normalized-boost-from-positive-lapse)
- [lem-author-ca4ffba327b3-compact-normal-exponential-tube](item-lem-author-ca4ffba327b3-compact-normal-exponential-tube)
- [lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant](item-lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant)
- [lem-author-ca4ffba327b3-causal-boundary-barriers](item-lem-author-ca4ffba327b3-causal-boundary-barriers)
- [lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries](item-lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries)
- [lem-author-ca4ffba327b3-regular-event-pair-supplies-aik-data](item-lem-author-ca4ffba327b3-regular-event-pair-supplies-aik-data)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Hawking’s local rigidity theorem without analyticity · §1 Theorems 1.1–1.2, pp.1–2; §2 affine null setup, pp.4–5, (2.1)–(2.4); Proposition 3.1, p.7, (3.1); §4 extension, pp.10–11 and conclusion p.15; §5 Propositions 5.1–5.2, pp.16–17 `](https://arxiv.org/pdf/0902.1173v1)


## Statement

Adopt [post-stationary-vacuum-model](item-post-stationary-vacuum-model) and the regular stationary vacuum data of [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime), with $T|_S\not\equiv0$ and maximal outer section $\Sigma_0\cap\mathcal E$, as in the standing construction setting. Near $S$ there are smooth Killing fields $K,Z$ and a constant $\Omega_H$ with $K=T+\Omega_HZ$, $K|_S=0$, and $[T,K]=[T,Z]=[K,Z]=0$. The field $Z$ generates a nontrivial circle action with least positive common period $2\pi$. There is a pole $p\in S$ with $Z(p)=T(p)=0$. For a constant $\kappa>0$, on the nonzero-generator part of $\mathcal H^+$ one has $\nabla_KK=\kappa K$ and $d(g(K,K))=-2\kappa g(K,\cdot)$; on $\mathcal H^-$ one has $\nabla_KK=-\kappa K$. The equations extend smoothly as zero equations at $S$, but do not there determine a scalar by themselves. In the normal basis with future unit time direction and outward direction into the exterior, $\nabla K$ has boost matrix $\kappa\begin{pmatrix}0&1\\1&0\end{pmatrix}$ on $S$. After shrinking the common neighborhood, there are smooth nowhere-zero future-directed affine null normal generators $L$ on $\mathcal H^+$ and $\underline L$ on $\mathcal H^-$, and smooth branch parameters $\underline u$ and $u$, respectively, with $L(\underline u)=\underline L(u)=1$, $\nabla_LL=\nabla_{\underline L}\underline L=0$, and parameter zero sets exactly $S$. Their profiles are $K=\kappa\underline u L$ on $\mathcal H^+$ and $K=-\kappa u\underline L$ on $\mathcal H^-$. In particular, $K$ is tangent and normal to both branches. The field $K$ is nonzero on the two local branches off $S$. These are local conclusions, not a smooth global axial extension theorem. The standing mass normalization does not enter this local argument.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[pthm-original-lapse-and-product](item-pthm-original-lapse-and-product)

[lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)

[def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair)

[thm-local-bifurcate-rigidity-input](item-thm-local-bifurcate-rigidity-input)

[def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity)

[lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[lem-author-ca4ffba327b3-event-boundary-generator-data](item-lem-author-ca4ffba327b3-event-boundary-generator-data)

[lem-author-ca4ffba327b3-stationary-product-excludes-zero-coefficient](item-lem-author-ca4ffba327b3-stationary-product-excludes-zero-coefficient)

[lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action](item-lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action)

[lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost](item-lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost)

[lem-author-ca4ffba327b3-normalized-boost-from-positive-lapse](item-lem-author-ca4ffba327b3-normalized-boost-from-positive-lapse)

[lem-author-ca4ffba327b3-compact-normal-exponential-tube](item-lem-author-ca4ffba327b3-compact-normal-exponential-tube)

[lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant](item-lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant)

[lem-author-ca4ffba327b3-causal-boundary-barriers](item-lem-author-ca4ffba327b3-causal-boundary-barriers)

[lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries](item-lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries)

[lem-author-ca4ffba327b3-regular-event-pair-supplies-aik-data](item-lem-author-ca4ffba327b3-regular-event-pair-supplies-aik-data)

## Facts & Assumptions

[A1] The vacuum/stationary model, the regular-spacetime definition and maximality of the specified outer section are the physical and geometric assumptions. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[A2] Work in ZFC with the inherited geometric and causal choice conventions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The completed lapse/product result gives $C=\Sigma_0\cap\mathcal E=\{r>1\}$, the global stationary-flow diffeomorphism $\mathbb R\times C\to\mathcal E$, and the positive lapse $N$ solving $\Delta_hN=|k|_h^2N$, with zero boundary and unit end limit. The exterior Hopf-control supplier gives $\nu(N)>0$ at every boundary point. [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product) [lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)

[F2] The five geometry helpers construct the normal tube, identify the event-boundary axes and causal barriers, prove the local quadrant description, and supply every pre-rigidity AIK pair hypothesis. [lem-author-ca4ffba327b3-compact-normal-exponential-tube](item-lem-author-ca4ffba327b3-compact-normal-exponential-tube) [lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant](item-lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant) [lem-author-ca4ffba327b3-causal-boundary-barriers](item-lem-author-ca4ffba327b3-causal-boundary-barriers) [lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries](item-lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries) [lem-author-ca4ffba327b3-regular-event-pair-supplies-aik-data](item-lem-author-ca4ffba327b3-regular-event-pair-supplies-aik-data)

[F3] The existing local rigidity input and the independently cited AIK affine data give $K_0$, $[T,K_0]=0$ and periodic $Z_0=T+\lambda_0K_0$ after the pre-rigidity hypotheses have been established. Use the source labels $\mathcal N=\mathcal H^+$ and $\underline{\mathcal N}=\mathcal H^-$. On these respective sheets the source profiles are $K_0=\underline u L$ and $K_0=-u\underline L$, where $L,\underline L$ are future-directed affine generators, $L(\underline u)=\underline L(u)=1$, and the parameters vanish on $S$. The detailed source is [AIK §2 and Proposition 3.1, (3.1)](https://arxiv.org/pdf/0902.1173v1), together with its §4 extension and §5 Propositions 5.1–5.2. [thm-local-bifurcate-rigidity-input](item-thm-local-bifurcate-rigidity-input) [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair)

[F4] The other five helpers establish event-boundary generator data, the nonzero coefficient from stationary-product injectivity, a circle pole with trivial normal action, the boost form, and the positive lapse/boost identity. [lem-author-ca4ffba327b3-event-boundary-generator-data](item-lem-author-ca4ffba327b3-event-boundary-generator-data) [lem-author-ca4ffba327b3-stationary-product-excludes-zero-coefficient](item-lem-author-ca4ffba327b3-stationary-product-excludes-zero-coefficient) [lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action](item-lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action) [lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost](item-lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost) [lem-author-ca4ffba327b3-normalized-boost-from-positive-lapse](item-lem-author-ca4ffba327b3-normalized-boost-from-positive-lapse)

[F5] Circle normalization, signed horizon coefficients, normal boost action and the Lorentzian conventions use the declared interfaces. [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data) [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data) [def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity) [lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

## External input

AIK Theorems 1.1–1.2, Proposition 3.1/(3.1), and §§4–5 supply the full-neighborhood Killing field with the affine profiles in [F3], its commutation with $T$, and periodic $Z_0=T+\lambda_0K_0$, under the established regular non-expanding local-pair hypotheses and $T|_S\not\equiv0$. This is the imported PDE/periodicity existence input from [AIK](https://arxiv.org/pdf/0902.1173v1). In applying it, label the source sheets $\mathcal N=\mathcal H^+$ and $\underline{\mathcal N}=\mathcal H^-$. The axis supplier in [F2] identifies their future null directions at $S$ as $n+\nu$ and $n-\nu$, respectively. Thus $L$ is a positive multiple of $n+\nu$ and $\underline L$ a positive multiple of $n-\nu$, with $g(L,\underline L)=-1$ at $S$. The source parameters satisfy $\underline u=0$ on $\mathcal H^-$ and $u=0$ on $\mathcal H^+$; their restrictions to the opposite sheets are affine parameters with zero set exactly $S$ after shrinking. This fixes the canonical field to have eigenvalue $+1$ on $n+\nu$ and $-1$ on $n-\nu$, as calculated in step 3.1. If starting with exchanged source labels, replace $K_0$ and $\lambda_0$ simultaneously by their negatives; $Z_0=T+\lambda_0K_0$ and $K=-\lambda_0K_0$ are unchanged. The source is not claimed to establish $\lambda_0\ne0$ or its sign; those are derived below from the existing lapse/product suppliers.

## Proof

[A1] The vacuum/stationary model, the regular-spacetime definition and maximality of the specified outer section are the physical and geometric assumptions. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[A2] Work in ZFC with the inherited geometric and causal choice conventions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The completed lapse/product result gives $C=\Sigma_0\cap\mathcal E=\{r>1\}$, the global stationary-flow diffeomorphism $\mathbb R\times C\to\mathcal E$, and the positive lapse $N$ solving $\Delta_hN=|k|_h^2N$, with zero boundary and unit end limit. The exterior Hopf-control supplier gives $\nu(N)>0$ at every boundary point. [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product) [lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)

[F2] The five geometry helpers construct the normal tube, identify the event-boundary axes and causal barriers, prove the local quadrant description, and supply every pre-rigidity AIK pair hypothesis. [lem-author-ca4ffba327b3-compact-normal-exponential-tube](item-lem-author-ca4ffba327b3-compact-normal-exponential-tube) [lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant](item-lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant) [lem-author-ca4ffba327b3-causal-boundary-barriers](item-lem-author-ca4ffba327b3-causal-boundary-barriers) [lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries](item-lem-author-ca4ffba327b3-normal-quadrants-realize-causal-boundaries) [lem-author-ca4ffba327b3-regular-event-pair-supplies-aik-data](item-lem-author-ca4ffba327b3-regular-event-pair-supplies-aik-data)

[F3] The existing local rigidity input and the independently cited AIK affine data give $K_0$, $[T,K_0]=0$ and periodic $Z_0=T+\lambda_0K_0$ after the pre-rigidity hypotheses have been established. Use the source labels $\mathcal N=\mathcal H^+$ and $\underline{\mathcal N}=\mathcal H^-$. On these respective sheets the source profiles are $K_0=\underline u L$ and $K_0=-u\underline L$, where $L,\underline L$ are future-directed affine generators, $L(\underline u)=\underline L(u)=1$, and the parameters vanish on $S$. The detailed source is [AIK §2 and Proposition 3.1, (3.1)](https://arxiv.org/pdf/0902.1173v1), together with its §4 extension and §5 Propositions 5.1–5.2. [thm-local-bifurcate-rigidity-input](item-thm-local-bifurcate-rigidity-input) [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair)

[F4] The other five helpers establish event-boundary generator data, the nonzero coefficient from stationary-product injectivity, a circle pole with trivial normal action, the boost form, and the positive lapse/boost identity. [lem-author-ca4ffba327b3-event-boundary-generator-data](item-lem-author-ca4ffba327b3-event-boundary-generator-data) [lem-author-ca4ffba327b3-stationary-product-excludes-zero-coefficient](item-lem-author-ca4ffba327b3-stationary-product-excludes-zero-coefficient) [lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action](item-lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action) [lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost](item-lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost) [lem-author-ca4ffba327b3-normalized-boost-from-positive-lapse](item-lem-author-ca4ffba327b3-normalized-boost-from-positive-lapse)

[F5] Circle normalization, signed horizon coefficients, normal boost action and the Lorentzian conventions use the declared interfaces. [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data) [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data) [def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity) [lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)



AIK Theorems 1.1–1.2, Proposition 3.1/(3.1), and §§4–5 supply the full-neighborhood Killing field with the affine profiles in [F3], its commutation with $T$, and periodic $Z_0=T+\lambda_0K_0$, under the established regular non-expanding local-pair hypotheses and $T|_S\not\equiv0$. This is the imported PDE/periodicity existence input from [AIK](https://arxiv.org/pdf/0902.1173v1). In applying it, label the source sheets $\mathcal N=\mathcal H^+$ and $\underline{\mathcal N}=\mathcal H^-$. The axis supplier in [F2] identifies their future null directions at $S$ as $n+\nu$ and $n-\nu$, respectively. Thus $L$ is a positive multiple of $n+\nu$ and $\underline L$ a positive multiple of $n-\nu$, with $g(L,\underline L)=-1$ at $S$. The source parameters satisfy $\underline u=0$ on $\mathcal H^-$ and $u=0$ on $\mathcal H^+$; their restrictions to the opposite sheets are affine parameters with zero set exactly $S$ after shrinking. This fixes the canonical field to have eigenvalue $+1$ on $n+\nu$ and $-1$ on $n-\nu$, as calculated in step 3.1. If starting with exchanged source labels, replace $K_0$ and $\lambda_0$ simultaneously by their negatives; $Z_0=T+\lambda_0K_0$ and $K=-\lambda_0K_0$ are unchanged. The source is not claimed to establish $\lambda_0\ne0$ or its sign; those are derived below from the existing lapse/product suppliers.



**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conclusions under exactly those hypotheses.

1.1 Apply [F1] under [A1]. Its identification of $C$ supplies the spacelike exterior collar of $S$, while regularity supplies the two smooth transverse non-expanding chronological end-boundaries. The five geometry lemmas in [F2] therefore establish the full local AIK pair definition, including the local causal-boundary condition rather than adding it as an extra assumption. Apply [F3] to obtain $K_0$ and the periodic $Z_0=T+\lambda_0K_0$. [A1, A2, F1, F2, F3]

2.1 The local symmetry neighborhood meets the exterior collar. The stationary-product lemma in [F4], using the diffeomorphism in [F1], gives $\lambda_0\ne0$. The common-period subgroup of the nontrivial local $Z_0$ action is closed and has no positive periods tending to zero: otherwise differentiation at a point where $Z_0\ne0$ would force that vector to vanish. Its positive infimum is consequently a least period $P$; division by $P$ shows every period is an integer multiple. Set $r=P/(2\pi)$ and $Z=rZ_0$. Then $Z$ has least positive common period $2\pi$. Put $K=-\lambda_0K_0=T-Z_0=T-r^{-1}Z$, so $\Omega_H=-r^{-1}$; reversing the orientation of $Z$ reverses the sign of $\Omega_H$ without changing $K$. Constant linearity and $[T,K_0]=0$ give every asserted commutator. [F1, F3, F4, F5, step 1.1]

3.1 The circle-pole lemma in [F4] gives $p\in S$ with $Z(p)=T(p)=0$ and $\nabla_\nu Z=0$. The axis lemma in [F2] identifies $\mathcal H^+$ with $a-b=0$ and $\mathcal H^-$ with $a+b=0$ in the normal tube $\exp_s(an+b\nu)$, so their future generator lines at $S$ are $\mathbb R_+(n+\nu)$ and $\mathbb R_+(n-\nu)$, respectively. With the source labels fixed in [F3], the imported affine profiles give, on $S$, $\nabla_LK_0=L(\underline u)L=L$ and $\nabla_{\underline L}K_0=-\underline L(u)\underline L=-\underline L$; the terms containing the vanishing affine parameters are zero. Thus $\nabla_{n+\nu}K_0=n+\nu$ and $\nabla_{n-\nu}K_0=-(n-\nu)$ at every point of $S$. Subtracting these equations and dividing by two gives $\nabla_\nu K_0=n$; adding gives $\nabla_nK_0=\nu$. Since $K=-\lambda_0K_0=T-r^{-1}Z$, the normalized-boost lemma with [F1] now gives $-\lambda_0=\nu(N)|_p>0$. Thus $c=-\lambda_0$ is a positive constant with the required coefficient of $T$. [F1, F2, F3, F4, F5, step 2.1]

4.1 On $\mathcal H^+$ the source profile in [F3] gives $K=c\underline u L$, with $L(\underline u)=1$ and $\nabla_LL=0$, so $\nabla_KK=c^2\underline u L=cK$. On $\mathcal H^-$ it gives $K=-cu\underline L$, with $\underline L(u)=1$ and $\nabla_{\underline L}\underline L=0$, so $\nabla_KK=c^2u\underline L=-cK$. Equivalently these are the signed affine-profile conclusions of the normalized-boost supplier in [F4], whose profile and normalization hypotheses were verified in step 3.1. Its Killing covector identity gives $d(g(K,K))=-2c\,g(K,\cdot)$ on $\mathcal H^+$ and the opposite sign on $\mathcal H^-$. The imported affine parameters have zero set exactly $S$, and the generators are nowhere zero, so $K$ is nonzero on either branch off $S$. The normal eigenvalue calculation in step 3.1 holds at every point of $S$ with this same constant $c$, giving the boost matrix with $\kappa=c>0$; the existing normal-boost supplier then gives the corresponding flow action. At $S$ the acceleration equations are merely their smooth zero extensions. This proves every original local assertion with its stationary and periodic normalizations. [F3, F4, F5, step 2.1, step 3.1] ∎

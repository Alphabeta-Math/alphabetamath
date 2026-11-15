---
title: Hawking and rotational fields near a bifurcate sphere
status: draft
research_item: thm-local-bifurcate-rigidity-input
dependency_level: 4
sources:
  references:
    - title: S. Alexakis, A. D. Ionescu and S. Klainerman, Hawking’s local rigidity
        theorem without analyticity
      url: https://arxiv.org/pdf/0902.1173v1
      locator: §1 setup and Theorems 1.1–1.2 (pp. 1–2); §2 Definition 2.1 (p. 6); §5
        Propositions 5.1–5.2 (pp. 16–17)
      statement: A local regular bifurcate non-expanding horizon in a connected
        oriented smooth four-dimensional vacuum spacetime admits a nontrivial
        generator-tangent Killing field in a full neighborhood of its
        bifurcation sphere. An additional Killing field tangent to both branches
        and not identically zero on the sphere admits a commuting nontrivial
        rotational Killing field; §5 gives [T,K]=0 and Z=T+lambda_0 K with a
        common positive period.
      hypotheses: Embedded spacelike two-sphere; neighborhood where the two local
        causal null boundaries are regular achronal null hypersurfaces generated
        orthogonally from the sphere; both expansions vanish; Ric(g)=0. For the
        rotational conclusion also a smooth Killing field T tangent to both
        branches whose restriction to the sphere is not identically zero.
      reading_limits: Read the downloaded arXiv:0902.1173v1 PDF text at §1 pp. 1–4, §2
        pp. 4–6 through Definition 2.1 and §5 Proposition 5.1–5.2 statements and
        adjacent proof text; visually inspected PDF p. 2. Did not independently
        reconstruct the characteristic existence or unique-continuation proofs
        in §§3–4, nor the proof of the sphere-periodicity input in Lemma 5.3.
        These are imported established inputs, not locally reconstructed proofs.
        The abstract clarifies the §1 phrase non-vanishing on S as not vanishing
        identically; no nowhere-zero field on the sphere is assumed.
external_input: true
---

## Prerequisites

- [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair)
- [lem-author-254b7c4bab6d-null-expansion-rescaling](item-lem-author-254b7c4bab6d-null-expansion-rescaling)
- [lem-author-254b7c4bab6d-null-form-screen-descent](item-lem-author-254b7c4bab6d-null-form-screen-descent)
- [lem-author-254b7c4bab6d-null-metric-transport](item-lem-author-254b7c4bab6d-null-metric-transport)
- [lem-author-254b7c4bab6d-tangent-killing-restriction](item-lem-author-254b7c4bab6d-tangent-killing-restriction)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Hawking’s local rigidity theorem without analyticity · §1 setup and Theorems 1.1–1.2 (pp. 1–2); §2 Definition 2.1 (p. 6); §5 Propositions 5.1–5.2 (pp. 16–17) `](https://arxiv.org/pdf/0902.1173v1)


## Statement

Let $(O,g)$ be a connected oriented smooth four-dimensional Ricci-flat spacetime, with the metric and Killing-field conventions of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). Let $(S,H_1,H_2)$ be a regular bifurcate non-expanding null horizon pair in the precise pre-rigidity sense of [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair). There is an open neighborhood $O'\subseteq O$ of $S$ and a nontrivial smooth Killing field $K$ tangent to the null generators of both branches. This conclusion assumes no previously existing Killing generator.

If additionally a smooth Killing field $T$ is tangent to both branches and $T|_S\not\equiv0$, one may shrink $O'$ so that $[T,K]=0$ and there is a constant $\lambda_0$ for which $Z=T+\lambda_0K$ is a nontrivial rotational Killing field commuting with $T$. Rotational means that its local flow has a common positive period on the chosen neighborhood; after constant rescaling it has the normalized circle-action convention of [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data). The conclusions concern a full neighborhood of $S$, not extension over the entire exterior.

## Facts & Assumptions

[F1] The regular null-horizon pair defines the pre-rigidity sphere, causal branches and zero-expansion conditions without positing a Killing generator. [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair)

[F2] Positive generator rescaling preserves zero expansion; the null second fundamental form and its trace are defined on the screen independently of a transverse section. [lem-author-254b7c4bab6d-null-expansion-rescaling](item-lem-author-254b7c4bab6d-null-expansion-rescaling) [lem-author-254b7c4bab6d-null-form-screen-descent](item-lem-author-254b7c4bab6d-null-form-screen-descent)

[F3] The null-metric transport identity identifies the geometric meaning of the null form, without using a rigidity conclusion or deriving shear-freeness from trace alone. [lem-author-254b7c4bab6d-null-metric-transport](item-lem-author-254b7c4bab6d-null-metric-transport)

[F4] A Killing field tangent to both branches restricts to a Killing field of the bifurcation sphere; the additional nontriviality condition means not identically zero there. [lem-author-254b7c4bab6d-tangent-killing-restriction](item-lem-author-254b7c4bab6d-tangent-killing-restriction)

[F5] Ambient Killing fields use the Lorentzian convention and normalized rotational fields use the circle-action convention. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

## External input

Theorem 1.1 of Alexakis–Ionescu–Klainerman supplies the full-neighborhood Hawking field under the stated regular non-expanding bifurcate-horizon hypotheses. Their Theorem 1.2 and §5 Propositions 5.1–5.2 supply the commuting field and the linear combination $Z=T+\lambda_0K$ with a common positive period under the additional branch-tangent symmetry hypothesis. These conclusions are imported inputs, not proofs reconstructed here. The five preceding local items formulate and relate the pre-rigidity data; they do not claim to replace the characteristic existence and unique-continuation arguments of the cited source. The exact source statement, hypotheses and actual reading limits are recorded in the citation metadata.

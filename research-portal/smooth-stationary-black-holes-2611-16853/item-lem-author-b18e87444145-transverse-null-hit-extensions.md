---
title: The closed selected domain has smooth endpoint extensions
status: published
research_item: lem-author-b18e87444145-transverse-null-hit-extensions
dependency_level: 4
---

## Prerequisites

- [lem-author-b18e87444145-temporal-normalized-null-flow](item-lem-author-b18e87444145-temporal-normalized-null-flow)
- [lem-author-b18e87444145-compact-diamond-closed-hit-domain](item-lem-author-b18e87444145-compact-diamond-closed-hit-domain)
- [lem-author-0336834a2590-transverse-endpoint-regularity](item-lem-author-0336834a2590-transverse-endpoint-regularity)
- [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)
- [math:thm-euclidean-implicit-function-theorem](https://alphabetamath.cc/item/thm-euclidean-implicit-function-theorem)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:thm-a-regular-level-set-is-an-embedded-submanifold](https://alphabetamath.cc/item/thm-a-regular-level-set-is-an-embedded-submanifold)


## Statement

Work in ZFC. Under the hypotheses of the compact-diamond endpoint lemma, $A$ is compact and Borel, and the endpoint map $F:A\to D$ is continuous and has smooth local extensions to open subsets of $C$, taking values in the smooth slice $\Sigma=\{v=0\}$. There is a finite cover of $A$ by such extensions and, after shrinking in charts, a countable cover by Lipschitz restrictions. In particular $F$ is Borel. These extension and continuity conclusions require no additional dimension or Riemannian metric data.

For the endpoint-area conclusion, assume additionally that $\dim E=4$ and that fixed smooth Riemannian metrics $h$ on $C$ and $k$ on $\Sigma$ are supplied as part of the data. Relative to these metrics, $F$ has the measurable Gram two-Jacobian and counting multiplicity conventions of the supplied endpoint-area interface. No regularity of $D$ as a surface, and no injectivity of $F$, is required.

## Facts & Assumptions

[A1] Work in ZFC, including AC, as required by the closed-domain and transverse-hitting suppliers and the endpoint-area conventions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The selected domain is closed with unique finite zero-time hits. [lem-author-b18e87444145-compact-diamond-closed-hit-domain](item-lem-author-b18e87444145-compact-diamond-closed-hit-domain)

[F2] Normalized null flow is smooth on its open flow domain. Its temporal normalization satisfies $dv(w)=1$. [lem-author-b18e87444145-temporal-normalized-null-flow](item-lem-author-b18e87444145-temporal-normalized-null-flow)

[F3] A smooth family with a unique transverse slice hit has local differentiable extensions and countably many chart-Lipschitz pieces. The Euclidean implicit function theorem supplies the transverse-hitting argument. [lem-author-0336834a2590-transverse-endpoint-regularity](item-lem-author-0336834a2590-transverse-endpoint-regularity) [math:thm-euclidean-implicit-function-theorem](https://alphabetamath.cc/item/thm-euclidean-implicit-function-theorem)

[F4] A smooth Riemannian metric is a smooth positive-definite symmetric covariant two-tensor. The endpoint-area interface uses a fixed such metric $h$ on the source surface and a fixed such metric $k$ on the target three-region; these metrics are supplied data for the additional area conclusion. Its Gram Jacobian and multiplicity conventions permit rank loss and coincident endpoints. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[F5] A nonempty regular level of a smooth real-valued map is an embedded codimension-one submanifold with its slice smooth structure. [math:thm-a-regular-level-set-is-an-embedded-submanifold](https://alphabetamath.cc/item/thm-a-regular-level-set-is-an-embedded-submanifold)

## Proof

**Given:** The hypotheses and, for the area conclusion, the additional dimension and fixed metric data in the Statement.

**Goal:** Establish the extension conclusions and the conditional endpoint-area conclusion.

1.1 Since $v$ is temporal, $dv$ is nonzero everywhere. Thus $0$ is a regular value and [F5] supplies the smooth slice $\Sigma$ when nonempty; its tangent space is $\ker dv$, as seen in the regular-level coordinates. Fix $c\in A$. The normalized flow from $(c,L_c/dv(L_c))$ exists on a neighborhood of the finite closed interval ending at temporal time zero. Openness of the flow domain and smooth dependence give the same interval, with slight endpoint margins, for all initial points in a neighborhood of $c$ in $C$. Evaluating at the smooth varying elapsed time $-v(c')$ gives a smooth map $H(c')$ into $\Sigma$: the flow identity is $v(H(c'))=v(c')-v(c')=0$. In the slice charts this is also a smooth map into $\Sigma$, since the fixed zero coordinate can be dropped. Its restriction to $A$ is $F$ by uniqueness. Transversality is explicit in the normalized family, whose derivative of $v$ with respect to elapsed time is $1$; hence the regularity supplier [F3] applies as well. [A1, F1, F2, F3, F5]

2.1 The closed subset $A$ of compact $C$ is compact and Borel. Its local extensions cover it finitely by compactness. Applying [F3] to the smooth normalized-flow family, with the unique transverse zero-level hits from step 1.1, gives a countable cover by restrictions to smaller source coordinate balls with Lipschitz coordinate representatives in target slice charts. Each extension equals $F$ on its intersection with $A$, so these local continuous maps make $F$ continuous on $A$, hence Borel. If $A$ is empty, the empty extension cover gives all these conclusions. This step uses no Riemannian metric on $C$ and no restriction on the target dimension. [A1, F1, F2, F3, step 1.1]

3.1 For the additional area conclusion, the supplied dimension $\dim E=4$ and [F5] make the nonempty slice $\Sigma$ three-dimensional, and the supplied fixed metrics make $(C,h)$ a Riemannian surface and $(\Sigma,k)$ a Riemannian three-region. Thus [F4] applies to the Borel domain and countable local smooth extensions established above, defining the measurable a.e. Gram two-Jacobian and counting multiplicity relative to these same fixed metrics. If $\Sigma$ is empty, then $D$ and $A$ are empty and the Jacobian and multiplicity conventions are vacuous. Endpoint focal degeneracy may cause rank loss but does not destroy the smooth extension or justify multiplicity one. [A1, F4, F5, step 1.1, step 2.1] ∎

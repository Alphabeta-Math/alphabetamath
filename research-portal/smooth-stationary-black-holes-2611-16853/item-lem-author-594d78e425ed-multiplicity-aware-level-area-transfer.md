---
title: Level-set area transfer retains generator multiplicity
status: published
research_item: lem-author-594d78e425ed-multiplicity-aware-level-area-transfer
dependency_level: 8
---

## Prerequisites

- [lem-author-594d78e425ed-compact-normal-flow-and-area-distortion](item-lem-author-594d78e425ed-compact-normal-flow-and-area-distortion)
- [lem-author-594d78e425ed-truncated-past-height-lipschitz-levels](item-lem-author-594d78e425ed-truncated-past-height-lipschitz-levels)
- [lem-author-594d78e425ed-negative-cut-selected-endpoints](item-lem-author-594d78e425ed-negative-cut-selected-endpoints)
- [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)
- [lem-author-0336834a2590-endpoint-area-with-multiplicity](item-lem-author-0336834a2590-endpoint-area-with-multiplicity)
- [def-truncated-null-boundary-height](item-def-truncated-null-boundary-height)


## Statement

Use the preceding flow, level identity and endpoint regularity, with the selected domains $A_z$ and endpoint maps $F_z$ of the truncated-height construction on its compact smooth source surface $C$. Equip $C$ with its induced metric, $\Sigma_z$ with its induced metric, and the collar with $h_0$. Fix $-2\delta<z<0$. Suppose the nonnegative Gram two-Jacobians satisfy $0\le J_2F_z\le J_2F_0\le1$ on $A_z\subset A_0$. If the inverse-flow two-dilation is at most $1+\epsilon(\delta)$ uniformly for $|z|\le2\delta$, then
$$\mathcal H^2_{h_0}(\{u=z\})\le(1+\epsilon(\delta))\int_{A_z}J_2F_z\,d\mu_C\le(1+\epsilon(\delta))\int_{A_0}J_2F_0\,d\mu_C.$$
The level set is countably two-rectifiable with finite area. This uses surjectivity and counting multiplicity, with no injectivity or smooth-image assumption.

## Facts & Assumptions

[F1] The inverse-flow two-dilation is supplied for $|z|\le2\delta$, and the exact level-set identity $\{u=z\}=\Psi_{-z}(D_z)$ is supplied for $|z|<2\delta$. [lem-author-594d78e425ed-compact-normal-flow-and-area-distortion](item-lem-author-594d78e425ed-compact-normal-flow-and-area-distortion) [lem-author-594d78e425ed-truncated-past-height-lipschitz-levels](item-lem-author-594d78e425ed-truncated-past-height-lipschitz-levels)

[F2] The domains are compact/Borel and the onto endpoint maps have countably many locally smooth Lipschitz extensions. [lem-author-594d78e425ed-negative-cut-selected-endpoints](item-lem-author-594d78e425ed-negative-cut-selected-endpoints)

[F3] For such endpoint maps the area formula counts multiplicity and gives image area at most the Jacobian integral. [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data) [lem-author-0336834a2590-endpoint-area-with-multiplicity](item-lem-author-0336834a2590-endpoint-area-with-multiplicity)

[F4] The truncated height $u$, cuts $D_z$, selected geodesic hit domains $A_z\subset C$ and unique endpoint maps $F_z:A_z\to D_z$ are the supplied construction. [def-truncated-null-boundary-height](item-def-truncated-null-boundary-height)

## Proof

**Given:** The hypotheses in the Statement, with $-2\delta<z<0$.

**Goal:** Establish the stated conclusions.

1.1 With the selected maps of [F4], form $G_z=\Psi_{-z}\circ F_z$ on $A_z$. Since $-2\delta<z<0$, [F1] applies to this interior slab time. By [F2] the endpoint map is onto $D_z$; by [F1] its inverse-flow image is exactly $\{u=z\}$. The composition has local smooth extensions after restricting the endpoint extensions to the open inverse-flow domain around their hits. Its differential lands first in the smooth section $\Sigma_z$ before inverse-flow transfer. For any two input tangent vectors the inverse-flow area-dilation bound therefore gives $J_2G_z\le(1+\epsilon(\delta))J_2F_z$, including rank-deficient derivatives. This is the Gram-determinant definition of two-dimensional dilation. [given, F1, F2, F4, algebra]

2.1 Apply [F3] to the Borel domain $A_z$ and $G_z$. Counting multiplicity is at least one at every point of its image, so $\mathcal H^2_{h_0}(\{u=z\})\le\int_{A_z}J_2G_z\,d\mu_C$. The countable Lipschitz extensions also make this image countably two-rectifiable. Now use step 1.1, the pointwise assumed optical comparison, and $A_z\subset A_0$. All integrands are nonnegative and measurable by local smooth extension. These are the asserted inequalities with their multiplicity and metric conventions. [given, F2, F3, step 1.1]

3.1 Apply [F2] at time zero: $A_0$ is compact and $F_0$ has local smooth extensions into $\Sigma_0$. Around each point of $A_0$, shrink an extension neighborhood to have compact closure within its extension domain. The smooth extension and smooth source and target metrics give a continuous, bounded Gram Jacobian on that closure. A finite subcover of $A_0$ therefore gives a finite common bound $M$ for $J_2F_0$ almost everywhere on $A_0$, using the Jacobian convention in [F3]. The compact smooth source surface $C$ has finite area: cover it by finitely many relatively compact coordinate disks, on which its smooth area density is bounded and the coordinate disks have finite Euclidean area. Consequently $\int_{A_0}J_2F_0\,d\mu_C\le M\mu_C(C)<\infty$. If $A_0$ is empty the integral is zero. Step 2.1 now gives finite level area. This argument does not extend the assumed bound $J_2F_0\le1$ from $A_z$ to $A_0$. [given, F2, F3, step 2.1] ∎

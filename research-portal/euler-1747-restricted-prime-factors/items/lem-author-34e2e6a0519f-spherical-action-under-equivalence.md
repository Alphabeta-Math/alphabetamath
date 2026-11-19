---
id: lem-author-34e2e6a0519f-spherical-action-under-equivalence
kind: lemma
title: Spherical Hecke operators under equivalence
status: published
domain: mathematics
proof_strategy: direct
deps:
  - math:def-topological-group
  - def-author-d45da46285be-spherical-hecke-algebra
  - math:def-linear-map
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-hausdorff-space
  - math:def-topological-space
  - math:def-subgroup
  - math:def-compact-space
  - math:def-subspace-topology-top
  - math:def-injection-surjection-bijection
  - math:def-dimension
  - math:def-linear-basis
  - math:def-vector-space
  - math:thm-complex-numbers-form-a-field
  - math:lem-linear-map-elementary-properties
  - math:def-monoid-finite-product
  - math:thm-induction-principle
  - math:def-linear-independence
  - math:thm-unique-coordinates-with-respect-to-an-ordered-basis
formulation_deps:
  - math:def-topological-group
  - def-author-d45da46285be-spherical-hecke-algebra
  - math:def-linear-map
  - math:def-hausdorff-space
  - math:def-topological-space
  - math:def-subgroup
  - math:def-compact-space
  - math:def-subspace-topology-top
  - math:def-injection-surjection-bijection
  - math:def-dimension
  - math:def-vector-space
  - math:thm-complex-numbers-form-a-field
argument_deps:
  - def-author-d45da46285be-spherical-hecke-algebra
  - math:def-topological-group
  - math:def-linear-map
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-hausdorff-space
  - math:def-topological-space
  - math:def-subgroup
  - math:def-compact-space
  - math:def-subspace-topology-top
  - math:def-injection-surjection-bijection
  - math:def-dimension
  - math:def-linear-basis
  - math:def-vector-space
  - math:thm-complex-numbers-form-a-field
  - math:lem-linear-map-elementary-properties
  - math:def-monoid-finite-product
  - math:thm-induction-principle
  - math:def-linear-independence
  - math:thm-unique-coordinates-with-respect-to-an-ordered-basis
dependency_roles:
  math:def-topological-group: mathematical-premise
  def-author-d45da46285be-spherical-hecke-algebra: mathematical-premise
  math:def-linear-map: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:def-hausdorff-space: mathematical-premise
  math:def-topological-space: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:def-subspace-topology-top: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:def-dimension: mathematical-premise
  math:def-linear-basis: mathematical-premise
  math:def-vector-space: mathematical-premise
  math:thm-complex-numbers-form-a-field: mathematical-premise
  math:lem-linear-map-elementary-properties: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
  math:thm-induction-principle: mathematical-premise
  math:def-linear-independence: mathematical-premise
  math:thm-unique-coordinates-with-respect-to-an-ordered-basis: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 1
---

## Statement

Let $H$ be a Hausdorff topological group with compact open subgroup $J$. Let $V$ and $W$ be complex representations of $H$ and let $I:V\to W$ be a bijective linear map with $I\pi_V(h)=\pi_W(h)I$ for every $h\in H$. Then $I$ identifies the $J$-fixed spaces, meaning the vectors unchanged by every $j\in J$, and it intertwines their spherical Hecke operators. A spherical Hecke function is a compactly supported complex function invariant under $J$ on both sides. Its operator on fixed vectors is the sum of contributions $f(x)\pi(x)$ over the cosets of the form $xJ$, with weight one per coset. In particular, if the fixed spaces are lines, their Hecke eigencharacters, the scalar actions of all these functions, are equal.

## Statement references

[[math:def-topological-group]]

[[def-author-d45da46285be-spherical-hecke-algebra]]

[[math:def-linear-map]]

[[math:def-hausdorff-space]]

[[math:def-topological-space]]

[[math:def-subgroup]]

[[math:def-compact-space]]

[[math:def-subspace-topology-top]]

[[math:def-injection-surjection-bijection]]

[[math:def-dimension]]

[[math:def-vector-space]]

[[math:thm-complex-numbers-form-a-field]]

## Facts & Assumptions

[F1] In a Hausdorff topological group $H$, the subgroup $J$ is assumed open in $H$ and compact in the subspace topology inherited from $H$. A complex representation acts by a homomorphism to the invertible linear operators. The $J$-fixed vectors form complex linear subspaces with the inherited operations. For a spherical Hecke function $f$, the operator on fixed vectors is the finite sum $\sum_{xJ} f(x)\pi(x)$ over the cosets where $f$ is nonzero. The sum is independent of the choice of representatives and defines a linear endomorphism of the fixed space. [[math:def-topological-group]] [[math:def-hausdorff-space]] [[math:def-topological-space]] [[math:def-subgroup]] [[math:def-compact-space]] [[math:def-subspace-topology-top]] [[def-author-d45da46285be-spherical-hecke-algebra]]

[F2] The spaces $V$ and $W$ are vector spaces over the field $\mathbb C$. Vector addition is associative and commutative with the zero vector as identity, and scalar multiplication satisfies $1v=v$. Linearity gives preservation of addition and scalar multiplication, and the zero-preservation lemma gives $I(0_V)=0_W$. [[math:def-vector-space]] [[math:thm-complex-numbers-form-a-field]] [[math:def-linear-map]] [[math:lem-linear-map-elementary-properties]]

[F3] Bijectivity gives a preimage for every vector in the codomain and makes that preimage unique. [[math:def-injection-surjection-bijection]]

[F4] A line is a vector space of dimension one and therefore has a singleton basis. A basis is linearly independent, and an injective finite list with image a basis is an ordered basis. In an ordered basis each vector has a unique list of scalar coordinates. [[math:def-dimension]] [[math:def-linear-basis]] [[math:def-linear-independence]] [[math:thm-unique-coordinates-with-respect-to-an-ordered-basis]]

[F5] A finite sum can be evaluated in any enumeration of its index set. Evaluation starts at zero and adjoins each next term by addition. Induction on the length of a finite list uses the empty prefix and the step of adjoining the next term. [[math:def-finite-sum-in-a-commutative-monoid]] [[math:def-monoid-finite-product]] [[math:thm-induction-principle]]

## Proof

**Given:** $H$, $J$, the actions and the bijective intertwining map $I$.

**Goal:** Identify the fixed spaces and their Hecke actions.

1.1 If $v$ is fixed by $J$, then $\pi_W(j)Iv=I\pi_V(j)v=Iv$ for each $j\in J$. Conversely, for a fixed vector $w$ in $W$ choose its preimage $v$ under $I$. For each $j\in J$, $I\pi_V(j)v=\pi_W(j)w=w=Iv$, so injectivity gives $\pi_V(j)v=v$. Thus $I$ restricts to a bijection on the fixed spaces and remains linear for their inherited operations. [given, F1, F2, F3]

1.2 Fix a spherical Hecke function $f$ and $v\in V^J$. Enumerate the finitely many contributing cosets. Let $P_k$ be the sum of the first $k$ contributions $f(x)\pi_V(x)v$, and let $Q_k$ be the sum of their images under $I$. For the empty prefix, $I(P_0)=I(0_V)=0_W=Q_0$. If $I(P_k)=Q_k$ and the next contribution is $u$, then $I(P_{k+1})=I(P_k+u)=I(P_k)+I(u)=Q_k+I(u)=Q_{k+1}$. Induction gives that $I$ sends the full sum to the sum of the images. [given, F1, F2, F5]

1.3 If the fixed spaces are lines, take a singleton basis $\{b\}$ of $V^J$. Listing it as $(b)$ gives an ordered basis because the list is injective and has image $\{b\}$. If $b=0_V$, the coefficient $1$ would yield a zero linear combination, contrary to independence. The ordered-basis coordinate theorem gives a unique expression $ab$ for each vector of $V^J$, since the coordinate sum has one term. [F1, F2, F4, F5]

2.1 For each contributing coset, $I(f(x)\pi_V(x)v)=f(x)I\pi_V(x)v=f(x)\pi_W(x)Iv$. Since $Iv$ is fixed, the spherical operator on $W^J$ uses the same cosets and the same weights. Hence $IT_f^Vv=T_f^W Iv$, where the superscripts specify the representation. [given, F1, F2, step 1.1, step 1.2]

3.1 Under the line hypothesis, for any $f$, write $T_f^V b=\lambda b$ using step 1.3. Since $I(0_V)=0_W$ and $I$ is injective, $Ib\ne 0_W$. The fixed-space bijection and linearity express every vector of $W^J$ as $I(ab)=aIb$. By step 2.1, $T_f^W Ib=IT_f^V b=\lambda Ib$, and linearity gives $T_f^W(aIb)=\lambda(aIb)$. If another scalar $\mu$ gave that action, then $I(\mu b)=\mu Ib=\lambda Ib=I(\lambda b)$. Injectivity and uniqueness of the coordinate in $V^J$ give $\mu=\lambda$. This proves equality of the scalar actions for every $f$. [F1, F2, F3, step 1.1, step 2.1, step 1.3] ∎

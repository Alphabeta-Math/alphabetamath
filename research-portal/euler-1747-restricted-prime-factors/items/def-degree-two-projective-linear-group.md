---
id: def-degree-two-projective-linear-group
kind: definition
title: Degree-two projective linear groups
status: published
domain: mathematics
deps:
  - math:def-ring
  - math:def-commutative-ring
  - math:def-field
  - math:def-local-ring
  - math:def-left-right-and-two-sided-ideal
  - math:def-prime-and-maximal-ideals
  - math:def-matrices-over-a-commutative-ring
  - math:def-ring-matrix-product-identity-and-transpose
  - math:def-invertible-matrix-and-similarity-over-a-commutative-ring
  - math:def-group
  - math:lem-ring-units-form-a-group
  - math:def-subgroup
  - math:def-center-of-a-group
  - math:def-normal-subgroup
  - math:def-coset
  - math:def-quotient-group
  - math:def-ring-homomorphism
  - math:def-group-homomorphism
  - math:def-quotient-ring
  - math:lem-field-is-a-commutative-ring
  - math:thm-ring-matrix-arithmetic-laws
  - math:lem-ring-elementary-consequences
  - math:thm-quotient-group-laws
  - math:lem-ring-homomorphism-basic-properties
  - math:lem-coset-membership-and-equality
  - math:thm-quotient-ring-laws
formulation_deps:
  - math:def-ring
  - math:def-commutative-ring
  - math:def-field
  - math:def-local-ring
  - math:def-left-right-and-two-sided-ideal
  - math:def-prime-and-maximal-ideals
  - math:def-matrices-over-a-commutative-ring
  - math:def-ring-matrix-product-identity-and-transpose
  - math:def-invertible-matrix-and-similarity-over-a-commutative-ring
  - math:def-group
  - math:lem-ring-units-form-a-group
  - math:def-subgroup
  - math:def-center-of-a-group
  - math:def-normal-subgroup
  - math:def-coset
  - math:def-quotient-group
  - math:def-ring-homomorphism
  - math:def-group-homomorphism
  - math:def-quotient-ring
  - math:thm-quotient-ring-laws
argument_deps:
  - math:def-ring
  - math:def-commutative-ring
  - math:def-local-ring
  - math:def-left-right-and-two-sided-ideal
  - math:def-ring-matrix-product-identity-and-transpose
  - math:def-invertible-matrix-and-similarity-over-a-commutative-ring
  - math:def-group
  - math:lem-ring-units-form-a-group
  - math:def-subgroup
  - math:def-center-of-a-group
  - math:def-normal-subgroup
  - math:def-coset
  - math:def-quotient-group
  - math:def-ring-homomorphism
  - math:def-group-homomorphism
  - math:def-quotient-ring
  - math:lem-field-is-a-commutative-ring
  - math:thm-ring-matrix-arithmetic-laws
  - math:lem-ring-elementary-consequences
  - math:thm-quotient-group-laws
  - math:lem-ring-homomorphism-basic-properties
  - math:lem-coset-membership-and-equality
  - math:thm-quotient-ring-laws
dependency_roles:
  math:def-ring: mathematical-premise
  math:def-commutative-ring: mathematical-premise
  math:def-field: mathematical-premise
  math:def-local-ring: mathematical-premise
  math:def-left-right-and-two-sided-ideal: mathematical-premise
  math:def-prime-and-maximal-ideals: mathematical-premise
  math:def-matrices-over-a-commutative-ring: mathematical-premise
  math:def-ring-matrix-product-identity-and-transpose: mathematical-premise
  math:def-invertible-matrix-and-similarity-over-a-commutative-ring: mathematical-premise
  math:def-group: mathematical-premise
  math:lem-ring-units-form-a-group: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:def-center-of-a-group: mathematical-premise
  math:def-normal-subgroup: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-quotient-group: mathematical-premise
  math:def-ring-homomorphism: mathematical-premise
  math:def-group-homomorphism: mathematical-premise
  math:def-quotient-ring: mathematical-premise
  math:lem-field-is-a-commutative-ring: mathematical-premise
  math:thm-ring-matrix-arithmetic-laws: mathematical-premise
  math:lem-ring-elementary-consequences: mathematical-premise
  math:thm-quotient-group-laws: mathematical-premise
  math:lem-ring-homomorphism-basic-properties: mathematical-premise
  math:lem-coset-membership-and-equality: mathematical-premise
  math:thm-quotient-ring-laws: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Definition

A ring is a set with addition and multiplication. Addition makes it an abelian group, meaning a group with commutative operation, with identity $0$. Multiplication is associative, has identity $1$, and distributes over addition on both sides. In a commutative ring, multiplication is commutative. Write $R^\times$ for the units of a ring $R$, the elements $u\in R$ admitting $v\in R$ with $uv=vu=1$.

Let $R$ be a field or a local ring. In a field, $1\ne 0$ and every nonzero element is a unit of the commutative ring. A local ring is a commutative ring with $1\ne 0$ and exactly one maximal ideal. An ideal is a subset containing $0$ and closed under differences and multiplication by arbitrary ring elements. A maximal ideal is an ideal different from the whole ring and contained in no larger ideal different from the whole ring.

Let $M_2(R)$ be the set of two-by-two arrays of entries in $R$. The matrix product is $(AB)_{ik}=a_{i1}b_{1k}+a_{i2}b_{2k}$, and $I_R$ has $1$ on the diagonal and $0$ elsewhere. The **general linear group** $\mathrm{GL}_2(R)$ consists of those $A\in M_2(R)$ with $AB=BA=I_R$ for some $B\in M_2(R)$, under matrix multiplication.

The **degree-two projective linear group** is the quotient group
$$\mathrm{PGL}_2(R)=\mathrm{GL}_2(R)/(R^\times I_R).$$
Here $R^\times I_R=\{uI_R:u\in R^\times\}$ is the scalar subgroup, with each $uI_R$ having $u$ on the diagonal and $0$ elsewhere. Its elements commute with all matrices in $\mathrm{GL}_2(R)$, so it is central. The element represented by $A$ is its left coset $[A]=\{uA:u\in R^\times\}$, where $uA$ means multiplying each entry by $u$. The quotient product is $[A][B]=[AB]$.

Let $S$ also be a field or a local ring. A unital ring homomorphism $f:R\to S$ preserves addition, multiplication, and the multiplicative identity. Write $f_2(A)$ for the matrix obtained by applying $f$ to each entry. The induced group homomorphism, meaning a map preserving the group product, is $\mathrm{PGL}_2(f):[A]\mapsto[f_2(A)]$. For an ideal $J$ with $S=R/J$ a field or local ring, the quotient ring has elements $r+J=\{r+j:j\in J\}$ with sum and product represented by the sum and product of representatives. Using $f(r)=r+J$ gives **projective reduction modulo $J$**.

## Facts & Assumptions

[F1] Each field is a commutative ring with its original operations and identities, and each local ring is commutative by definition ([[math:lem-field-is-a-commutative-ring|field as a commutative ring]], [[math:def-local-ring|local ring]], [[math:def-commutative-ring|commutative ring]]). Rings have an associative multiplication with identity, and zero annihilates multiplication on both sides ([[math:def-ring|ring]], [[math:lem-ring-elementary-consequences|zero multiplication in a ring]]).

[F2] Square matrices over a commutative ring multiply by the entry formulas above, and their multiplication is associative with identity $I_R$. Invertible matrices have unique two-sided inverses ([[math:def-ring-matrix-product-identity-and-transpose|matrix product and identity]], [[math:thm-ring-matrix-arithmetic-laws|matrix arithmetic laws]], [[math:def-invertible-matrix-and-similarity-over-a-commutative-ring|matrix invertibility]]).

[F3] A group has an associative operation with a two-sided identity and a two-sided inverse for every element. The units of a ring form such a group under multiplication ([[math:def-group|group]], [[math:lem-ring-units-form-a-group|ring units]]).

[F4] The center $Z(G)$ consists of the elements of $G$ that commute with every element of $G$ ([[math:def-center-of-a-group|center of a group]]). A subgroup contains the identity and is closed under products and inverses. It is normal if $gNg^{-1}=N$ for every $g$ in the group. For a normal subgroup $N$ of a group $G$, the left cosets $gN=\{gn:n\in N\}$ form a group with product $(gN)(hN)=(gh)N$ ([[math:def-subgroup|subgroup]], [[math:def-normal-subgroup|normal subgroup]], [[math:def-coset|left coset]], [[math:def-quotient-group|quotient group]], [[math:thm-quotient-group-laws|quotient group laws]]). For elements $a,b$ of a group and a subgroup $N$, the left cosets $aN$ and $bN$ agree exactly when $a^{-1}b\in N$ ([[math:lem-coset-membership-and-equality|coset equality]]).

[F5] A unital ring homomorphism sends $0$ to $0$ and units to units, in addition to preserving the operations and $1$. A map between groups is a group homomorphism if it preserves multiplication ([[math:def-ring-homomorphism|ring homomorphism]], [[math:lem-ring-homomorphism-basic-properties|images of zero and units]], [[math:def-group-homomorphism|group homomorphism]]).

[F6] An ideal $J$ of a commutative ring $R$ is two-sided. The additive cosets modulo $J$ form a ring with identity $1+J$. The sum and product are well defined and computed by adding and multiplying representatives ([[math:def-left-right-and-two-sided-ideal|ideal]], [[math:def-quotient-ring|quotient ring]], [[math:thm-quotient-ring-laws|quotient-ring laws]]).

## Justification

**Given:** Rings $R,S$, each a field or a local ring, and a unital ring homomorphism $f:R\to S$.

**Goal:** Justify the matrix group, its scalar quotient, and the induced map, including the quotient-ring reduction.

1.1 Work over either ring, using $R$ to write the formulas. The identity matrix is invertible with inverse itself. If $A,B$ have inverses $A^{-1},B^{-1}$, then $(AB)(B^{-1}A^{-1})=I_R=(B^{-1}A^{-1})(AB)$ by associativity and the inverse equations. Also $A$ is a two-sided inverse to $A^{-1}$. Thus multiplication, the identity and inverses restrict to the invertible matrices, making $\mathrm{GL}_2(R)$ a group. [F1, F2, F3]

2.1 For a unit $u$, the inverse of $uI_R$ is $u^{-1}I_R$, and $(uI_R)(vI_R)=(uv)I_R$ for units $u,v$. This follows from entrywise matrix multiplication and zero annihilation. Together with $I_R=1I_R$, these identities make $R^\times I_R$ a subgroup. For $A=(a_{ik})\in\mathrm{GL}_2(R)$, the entries of $(uI_R)A$ and $A(uI_R)$ are $ua_{ik}$ and $a_{ik}u$ respectively, equal by commutativity. Thus $R^\times I_R$ is contained in $Z(\mathrm{GL}_2(R))$ and is a central subgroup. Hence $A(uI_R)A^{-1}=uI_R$ for every unit $u$, so $ANA^{-1}=N$ for $N=R^\times I_R$. The quotient group law applies, and the same entry formula gives $AN=\{uA:u\in R^\times\}$. [F1, F2, F3, F4, step 1.1]

2.2 The entry formula and preservation of addition and multiplication give $f_2(AB)=f_2(A)f_2(B)$. Since $f$ preserves $0$ and $1$, $f_2(I_R)=I_S$. Applying these identities to both products of $A$ with $A^{-1}$ shows that $f_2(A^{-1})$ is a two-sided inverse to $f_2(A)$. In particular the latter lies in $\mathrm{GL}_2(S)$. [F2, F5, step 1.1]

3.1 If $A'$ represents $[A]$, then $A'=uA$ for a unit $u\in R^\times$. Applying $f$ to the entries gives $f_2(A')=f(u)f_2(A)$ with $f(u)\in S^\times$. Since the scalar matrix $f(u)I_S$ commutes with $f_2(A)$, we have $f_2(A)^{-1}f_2(A')=f(u)I_S\in S^\times I_S$. The left-coset equality criterion gives $[f_2(A')]=[f_2(A)]$. The induced map sends $[AB]$ to $[f_2(A)f_2(B)]=[f_2(A)][f_2(B)]$, hence is a group homomorphism. [F4, F5, step 2.1, step 2.2]

4.1 Suppose $S=R/J$ is a field or local ring as in the definition. Since $R$ is commutative, $J$ is two-sided, so $R/J$ has well-defined coset operations and identity $1+J$. The map $\pi(r)=r+J$ preserves addition and multiplication by the coset formulas, and $\pi(1)=1+J$. Thus $\pi$ is a unital ring homomorphism and its induced map is projective reduction. This establishes all the constructions in the definition. [F1, F5, F6, step 3.1] ∎

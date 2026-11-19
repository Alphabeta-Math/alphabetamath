---
id: def-author-d45da46285be-spherical-model
kind: definition
title: Normalized upper-triangular spherical model
status: draft
domain: mathematics
deps: &a1
  - math:def-prime
  - math:lem-nat-embeds-int
  - math:def-countable-choice
  - lem-author-d45da46285be-triangular-cosets
  - def-author-d45da46285be-spherical-hecke-algebra
  - def-degree-two-projective-linear-group
  - math:cor-cauchy-reals-lub-complete
  - math:lem-of-naturals-positive
  - math:lem-nonnegative-square-root-exists-and-unique
  - math:thm-complex-numbers-form-a-field
  - math:def-field
  - math:def-group-power
  - math:def-function-space
  - math:def-topological-space
  - math:lem-group-power-laws
  - math:def-linear-subspace
  - math:lem-topological-group-translations-and-inversion
  - math:def-field-of-p-adic-numbers
  - math:thm-p-adic-completion-is-a-field
  - math:cor-zp-is-the-valuation-ring-of-qp
  - math:cor-maximal-ideal-and-residue-field-of-zp
  - math:def-subgroup
  - math:def-p-adic-absolute-value-on-the-rationals
  - math:def-metric-topology
  - math:def-product-topology
  - math:def-subspace-topology-top
  - math:def-homeomorphism-and-open-maps
dependency_roles:
  math:def-prime: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-countable-choice: mathematical-premise
  lem-author-d45da46285be-triangular-cosets: mathematical-premise
  def-author-d45da46285be-spherical-hecke-algebra: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  math:cor-cauchy-reals-lub-complete: mathematical-premise
  math:lem-of-naturals-positive: mathematical-premise
  math:lem-nonnegative-square-root-exists-and-unique: mathematical-premise
  math:thm-complex-numbers-form-a-field: mathematical-premise
  math:def-field: mathematical-premise
  math:def-group-power: mathematical-premise
  math:def-function-space: mathematical-premise
  math:def-topological-space: mathematical-premise
  math:lem-group-power-laws: mathematical-premise
  math:def-linear-subspace: mathematical-premise
  math:lem-topological-group-translations-and-inversion: mathematical-premise
  math:def-field-of-p-adic-numbers: mathematical-premise
  math:thm-p-adic-completion-is-a-field: mathematical-premise
  math:cor-zp-is-the-valuation-ring-of-qp: mathematical-premise
  math:cor-maximal-ideal-and-residue-field-of-zp: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:def-p-adic-absolute-value-on-the-rationals: mathematical-premise
  math:def-metric-topology: mathematical-premise
  math:def-product-topology: mathematical-premise
  math:def-subspace-topology-top: mathematical-premise
  math:def-homeomorphism-and-open-maps: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
formulation_deps:
  - math:def-prime
  - math:lem-nat-embeds-int
  - math:def-countable-choice
  - lem-author-d45da46285be-triangular-cosets
  - def-author-d45da46285be-spherical-hecke-algebra
  - def-degree-two-projective-linear-group
  - math:cor-cauchy-reals-lub-complete
  - math:lem-of-naturals-positive
  - math:lem-nonnegative-square-root-exists-and-unique
  - math:thm-complex-numbers-form-a-field
  - math:def-field
  - math:def-group-power
  - math:def-function-space
  - math:def-topological-space
  - math:def-field-of-p-adic-numbers
  - math:thm-p-adic-completion-is-a-field
  - math:cor-zp-is-the-valuation-ring-of-qp
  - math:cor-maximal-ideal-and-residue-field-of-zp
  - math:def-subgroup
  - math:def-p-adic-absolute-value-on-the-rationals
  - math:def-metric-topology
  - math:def-product-topology
  - math:def-subspace-topology-top
argument_deps: *a1
---

## Definition

Assume countable choice, meaning that a sequence of nonempty sets has a choice function. For a prime $\ell$, let $\mathbb Q_\ell$ be the canonical metric completion of $\mathbb Q$ for $d_\ell(x,y)=|x-y|_\ell$, where $|\cdot|_\ell$ on $\mathbb Q$ is the $\ell$-adic absolute value. Its points are classes of rational $d_\ell$-Cauchy sequences, with two sequences equivalent when their termwise distance tends to zero. Write $\mathbb Z_\ell=\{x\in\mathbb Q_\ell:|x|_\ell\le 1\}$ for its ring of integers, using the extended absolute value. Let $G=\mathrm{GL}_2(\mathbb Q_\ell)$ and $K=\mathrm{GL}_2(\mathbb Z_\ell)$. Identify each matrix with its four entries and give $G$ the subspace topology from the product topology on $\mathbb Q_\ell^4$, with each factor carrying the metric topology of the extended $\ell$-adic metric.

Let $B$ be the upper-triangular subgroup of $G$, consisting of matrices $b=(b_{ij})$ with $b_{21}=0$. For an ordered pair $u,v\in\mathbb C^\times$ and $b\in B$ whose diagonal entries $b_{11},b_{22}$ have $\ell$-adic valuations $r,s$, set
$$c_{u,v}(b)=\ell^{(s-r)/2}u^rv^s.$$
Here $\ell^{(s-r)/2}$ means $q^{s-r}$ for the positive real square root $q=\sqrt{\ell}$. Regard $q$ as a complex number and take all three integer powers in $\mathbb C^\times$, using inverses for negative exponents.

Let $I(u,v)$ be the vector space of locally constant complex functions $F$ on $G$ with $F(bg)=c_{u,v}(b)F(g)$ for every $b\in B$ and $g\in G$, using the pointwise operations inherited from $\mathbb C^G$. A function is locally constant when, for each $g\in G$, it is constant on some open set $U\subseteq G$ containing $g$. The group acts by right translation, $(R(h)F)(g)=F(gh)$.

The normalized upper-triangular spherical vector $\Phi_{u,v}$ is the $K$-fixed vector in $I(u,v)$ taking the value one at the identity. Being $K$-fixed here means being invariant under right translation by every $k\in K$. Its value on a triangular representative $b$ is $c_{u,v}(b)$.

## Facts & Assumptions

[F1] For the prime $\ell$, the rational metric $d_\ell(x,y)=|x-y|_\ell$ uses the rational $\ell$-adic absolute value ([[math:def-p-adic-absolute-value-on-the-rationals]]). The canonical Cauchy-sequence quotient for this metric gives the metric space $\mathbb Q_\ell$ ([[math:def-field-of-p-adic-numbers]]). This quotient is a complete field with the extended nonarchimedean absolute value ([[math:thm-p-adic-completion-is-a-field]]). Its ring of integers $\mathbb Z_\ell$ is identified with the subring $\{x\in\mathbb Q_\ell:|x|_\ell\le 1\}$ under the canonical embedding, and its unique maximal ideal is $\ell\mathbb Z_\ell$ ([[math:cor-zp-is-the-valuation-ring-of-qp|Valuation ring of the local field]], [[math:cor-maximal-ideal-and-residue-field-of-zp]]). The matrix-entry topology on $G$ is the subspace topology from the product of four copies of $\mathbb Q_\ell$, each with its $\ell$-adic metric topology ([[math:def-metric-topology]], [[math:def-product-topology]], [[math:def-subspace-topology-top]]). Under countable choice, $G$ is a topological group and $K$ is a compact open subgroup in the matrix-entry topology. Each coset $gK$ has an upper-triangular representative with diagonal valuations determined by the coset. The valuation on nonzero field elements is integer valued and additive under multiplication ([[math:def-countable-choice]], [[lem-author-d45da46285be-triangular-cosets]]).

[F2] A group representation on a complex vector space acts by invertible linear maps, with product sent to composition. Its $K$-fixed vectors are those unchanged by all the actions of $k\in K$ ([[def-author-d45da46285be-spherical-hecke-algebra]]).

[F3] A local ring is a commutative ring with $1\ne 0$ and exactly one maximal ideal. Over a field or local ring, $\mathrm{GL}_2$ consists of two-by-two matrices with two-sided inverses. The matrix product is given by $(AB)_{ik}=a_{i1}b_{1k}+a_{i2}b_{2k}$ ([[def-degree-two-projective-linear-group]]). A subset of a group is a subgroup if it contains the identity and is closed under products and inverses ([[math:def-subgroup]]).

[F4] The reals are a complete ordered field. Since the prime $\ell$ is an integer greater than one, it is the image of a unique natural $m\ge1$ under the natural-to-integer embedding ([[math:def-prime]], [[math:lem-nat-embeds-int]]). In the real square root, $\ell$ means the canonical real numeral $m\cdot1_{\mathbb R}$, which is positive. Every nonnegative element of a complete ordered field has a unique nonnegative square root ([[math:cor-cauchy-reals-lub-complete]], [[math:lem-of-naturals-positive]], [[math:lem-nonnegative-square-root-exists-and-unique]]).

[F5] The field $\mathbb C$ contains an embedded copy of $\mathbb R$, and its nonzero elements form an abelian group under multiplication. In a group, integer powers have $z^0=1$, use inverses for negative exponents, and satisfy $z^{m+n}=z^mz^n$ ([[math:thm-complex-numbers-form-a-field]], [[math:def-field]], [[math:def-group-power]], [[math:lem-group-power-laws]]).

[F6] All functions from a set into a field form a vector space under pointwise operations. A subset of a vector space that contains zero and is closed under addition and scalar multiplication is a vector space under the restricted operations ([[math:def-function-space]], [[math:def-linear-subspace]]).

[F7] The whole space is open, and an intersection of two open sets is open. Left and right translations in a topological group are homeomorphisms ([[math:def-topological-space]], [[math:lem-topological-group-translations-and-inversion]]). A homeomorphism sends open sets to open sets and has open preimages of open sets ([[math:def-homeomorphism-and-open-maps]]).

## Justification

**Given:** A prime $\ell$, countable choice and nonzero $u,v\in\mathbb C$.

**Goal:** Establish the right-translation representation and the existence and uniqueness of its normalized $K$-fixed vector.

1.1 The ring $\mathbb Z_\ell$ is a unital subring of the field $\mathbb Q_\ell$, so it is commutative and has $1\ne 0$. Its unique maximal ideal from [F1] makes it a local ring by [F3]. The degree-two matrix group construction thus applies to both $\mathbb Q_\ell$ and $\mathbb Z_\ell$. An invertible upper-triangular matrix has nonzero diagonal entries, since a zero diagonal entry would give a zero first column or second row. The product rule makes the lower-left entry of a triangular product zero and multiplies the diagonal entries componentwise. If $b$ is invertible and upper triangular, the lower-left entry of $bb^{-1}=1$ is $b_{22}(b^{-1})_{21}=0$, so the inverse is upper triangular as well. The identity has zero lower-left entry. The identity, product and inverse tests in [F3] therefore show that $B$ is a subgroup with the restricted matrix multiplication. [F1, F3]

2.1 Since $\ell$ is positive, its nonnegative square root is positive and gives a nonzero element $q$ of $\mathbb C$. The bases $q,u,v$ therefore admit all integer powers. If $b,b'\in B$ have valuation pairs $(r,s)$ and $(r',s')$, the product has valuations $(r+r',s+s')$ by the componentwise diagonal product and additivity of the valuation. The exponent addition law and commutativity of $\mathbb C^\times$ then give $c_{u,v}(bb')=c_{u,v}(b)c_{u,v}(b')$. The identity has valuation pair $(0,0)$ by additivity, so $c_{u,v}(1)=1$. [F1, F4, F5, step 1.1]

3.1 With the scalar multiplier now defined, the zero function is constant on the open set $G$ and satisfies the covariance condition. For $F,H\in I(u,v)$ and $a,d\in\mathbb C$, at any $g\in G$ take open sets $U,V$ containing $g$ on which $F,H$ respectively are constant. Then $U\cap V$ is open, contains $g$, and $aF+dH$ is constant there. At $bg$ both terms acquire the same scalar multiplier by covariance, so $(aF+dH)(bg)=c_{u,v}(b)(aF+dH)(g)$. Hence $I(u,v)$ is a vector subspace of $\mathbb C^G$. [F5, F6, F7, step 2.1]

4.1 For $h\in G$ and $F\in I(u,v)$, take an open set $U$ containing $gh$ on which $F$ is constant. Its preimage under right translation by $h$ is open by [F7], contains $g$, and $R(h)F$ is constant there. Also $(R(h)F)(bg)=F(b(gh))=c_{u,v}(b)(R(h)F)(g)$, so $R(h)$ maps $I(u,v)$ into itself. Evaluation at $gh$ commutes with pointwise linear combinations, which makes $R(h)$ linear. The formulas $(R(h)R(j)F)(g)=F(ghj)$ and $R(1)F=F$ give the representation law and the inverse $R(h^{-1})$ of $R(h)$. [F1, F2, F6, F7, step 3.1]

5.1 Define $\Phi_{u,v}(bk)=c_{u,v}(b)$ for $b\in B$ and $k\in K$. Every element has this form and its triangular exponents are uniquely determined by the coset, so the value is well defined. Each coset $gK$ is open as a left translate of the open subgroup $K$. Constancy on each coset gives local constancy and right $K$-invariance. For $b_0\in B$, the product $b_0b$ is triangular and $\Phi_{u,v}(b_0bk)=c_{u,v}(b_0b)=c_{u,v}(b_0)\Phi_{u,v}(bk)$, so $\Phi_{u,v}$ lies in $I(u,v)$. Its value at the identity is $c_{u,v}(1)=1$. [F1, F2, F7, step 1.1, step 2.1, step 4.1]

6.1 If $F\in I(u,v)^K$, then for every $b\in B$ and $k\in K$ we have $F(bk)=F(b)=c_{u,v}(b)F(1)=F(1)\Phi_{u,v}(bk)$. Every element of $G$ is of this form, so $F=F(1)\Phi_{u,v}$. [F1, F2, F5, F6, step 5.1]

7.1 Conversely, for $a\in\mathbb C$, the function $a\Phi_{u,v}$ lies in $I(u,v)$ and $R(k)(a\Phi_{u,v})=aR(k)\Phi_{u,v}=a\Phi_{u,v}$ for every $k\in K$. Hence $I(u,v)^K=\{a\Phi_{u,v}:a\in\mathbb C\}$. Evaluating at the identity gives $(a\Phi_{u,v})(1)=a$, so distinct scalars give distinct fixed vectors and $\Phi_{u,v}$ is the unique fixed vector of value one there. [F2, F5, F6, step 3.1, step 4.1, step 5.1, step 6.1] ∎

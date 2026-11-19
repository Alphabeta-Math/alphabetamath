---
id: lem-euler-hurwitz-torus-normalizer-order
kind: lemma
title: Conjugation and order of the torus normalizer
status: published
domain: mathematics
deps:
  - def-euler-prime-classes
  - math:def-integers-modulo-n
  - math:def-addition-and-multiplication-modulo-n
  - math:thm-z-mod-p-is-a-field
  - math:thm-standard-representatives-modulo-n
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - math:def-quotient-ring
  - lem-euler-hurwitz-odd-split-reduction
  - def-euler-hurwitz-torus-normalizer
  - math:def-field
  - math:def-field-extension-generated-subfields-and-simple-extension
  - math:def-extension-degree-and-finite-extension
  - math:def-linear-basis
  - math:def-dimension
  - math:def-field-homomorphism
  - math:def-f-homomorphisms-and-embeddings-of-field-extensions
  - math:def-relative-frobenius-of-a-finite-field-extension
  - math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-projective-reduction
  - math:def-coset
  - math:def-normalizer-of-a-subgroup
  - math:lem-centralizers-and-normalizers-are-subgroups
  - math:def-finite-cardinality
  - math:def-ring-matrix-product-identity-and-transpose
  - math:thm-ring-matrix-arithmetic-laws
  - math:def-linear-map
  - math:def-linear-isomorphism-and-invertible-linear-map
  - math:thm-invertible-matrices-correspond-to-linear-isomorphisms
  - math:def-coordinate-column-and-matrix-of-a-linear-map
  - math:thm-matrix-of-a-composite-is-the-product
  - lem-quadratic-field-normalizer-in-degree-two
  - math:def-subgroup
formulation_deps:
  - def-euler-prime-classes
  - math:def-integers-modulo-n
  - math:def-addition-and-multiplication-modulo-n
  - math:thm-z-mod-p-is-a-field
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - math:def-quotient-ring
  - lem-euler-hurwitz-odd-split-reduction
  - def-euler-hurwitz-torus-normalizer
  - math:def-field
  - math:def-field-extension-generated-subfields-and-simple-extension
  - math:def-extension-degree-and-finite-extension
  - math:def-linear-basis
  - math:def-dimension
  - math:def-field-homomorphism
  - math:def-f-homomorphisms-and-embeddings-of-field-extensions
  - math:def-relative-frobenius-of-a-finite-field-extension
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-projective-reduction
  - math:def-coset
  - math:def-normalizer-of-a-subgroup
  - math:def-finite-cardinality
  - math:def-ring-matrix-product-identity-and-transpose
  - math:def-subgroup
argument_deps:
  - def-euler-prime-classes
  - math:def-integers-modulo-n
  - math:def-addition-and-multiplication-modulo-n
  - math:thm-z-mod-p-is-a-field
  - math:thm-standard-representatives-modulo-n
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - math:def-quotient-ring
  - lem-euler-hurwitz-odd-split-reduction
  - def-euler-hurwitz-torus-normalizer
  - math:def-field
  - math:def-field-extension-generated-subfields-and-simple-extension
  - math:def-extension-degree-and-finite-extension
  - math:def-linear-basis
  - math:def-dimension
  - math:def-field-homomorphism
  - math:def-f-homomorphisms-and-embeddings-of-field-extensions
  - math:def-relative-frobenius-of-a-finite-field-extension
  - math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-projective-reduction
  - math:def-coset
  - math:def-normalizer-of-a-subgroup
  - math:lem-centralizers-and-normalizers-are-subgroups
  - math:def-finite-cardinality
  - math:def-ring-matrix-product-identity-and-transpose
  - math:thm-ring-matrix-arithmetic-laws
  - math:def-linear-map
  - math:def-linear-isomorphism-and-invertible-linear-map
  - math:thm-invertible-matrices-correspond-to-linear-isomorphisms
  - math:def-coordinate-column-and-matrix-of-a-linear-map
  - math:thm-matrix-of-a-composite-is-the-product
  - lem-quadratic-field-normalizer-in-degree-two
  - math:def-subgroup
dependency_roles:
  math:def-dimension: mathematical-premise
  math:def-linear-isomorphism-and-invertible-linear-map: mathematical-premise
  math:thm-invertible-matrices-correspond-to-linear-isomorphisms: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  math:def-integers-modulo-n: mathematical-premise
  math:def-addition-and-multiplication-modulo-n: mathematical-premise
  math:thm-z-mod-p-is-a-field: mathematical-premise
  math:thm-standard-representatives-modulo-n: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  math:def-quotient-ring: mathematical-premise
  lem-euler-hurwitz-odd-split-reduction: mathematical-premise
  def-euler-hurwitz-torus-normalizer: mathematical-premise
  math:def-field: mathematical-premise
  math:def-field-extension-generated-subfields-and-simple-extension: mathematical-premise
  math:def-extension-degree-and-finite-extension: mathematical-premise
  math:def-linear-basis: mathematical-premise
  math:def-field-homomorphism: mathematical-premise
  math:def-f-homomorphisms-and-embeddings-of-field-extensions: mathematical-premise
  math:def-relative-frobenius-of-a-finite-field-extension: mathematical-premise
  math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  def-euler-hurwitz-projective-reduction: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-normalizer-of-a-subgroup: mathematical-premise
  math:lem-centralizers-and-normalizers-are-subgroups: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-ring-matrix-product-identity-and-transpose: mathematical-premise
  math:thm-ring-matrix-arithmetic-laws: mathematical-premise
  math:def-linear-map: mathematical-premise
  math:def-coordinate-column-and-matrix-of-a-linear-map: mathematical-premise
  math:thm-matrix-of-a-composite-is-the-product: mathematical-premise
  lem-quadratic-field-normalizer-in-degree-two: mathematical-premise
  math:def-subgroup: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §3.3, order assertion immediately following the subgroup
        definitions
      reading_limits: The opening paragraph of §3.3 on PDF page 4 was checked for attribution.
dependency_level: 6
---

## Statement

Let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$. Write $\mathbb F_p=\mathbb Z/p\mathbb Z$ for the field of integer residue classes modulo $p$, with addition and multiplication of representatives. The rational Hamilton quaternions have basis $1,i,j,k$ with $i^2=j^2=-1$ and $k=ij=-ji$. Their Hurwitz order $\mathcal H$ is the subring whose coordinates are either all integers or all integers plus $\tfrac12$. In $R_p=\mathcal H/p\mathcal H$, the ring of additive cosets with operations on representatives, write $\bar i,\bar j$ for the images of $i,j$. Use the fixed reduction isomorphism $\bar\Phi_p:R_p\to M_2(\mathbb F_p)$, a bijection preserving addition, multiplication, identity and scalars. Here $M_2(\mathbb F_p)$ consists of two-by-two matrices with row-by-column multiplication.

Put $E_p=\mathbb F_p[i]=\{a+b\bar i:a,b\in\mathbb F_p\}$, the field denoted here by $\mathbb F_{p^2}$. It has $p^2$ elements and degree two over $\mathbb F_p$. Write $E_p^\times$ for its nonzero elements under multiplication. In the projective group $G_p=\mathrm{PGL}_2(\mathbb F_p)$, an invertible matrix $A$, meaning one with a two-sided matrix inverse, represents the class $[A]=\{tA:t\in\mathbb F_p,\ t\ne0\}$, with product $[A][B]=[AB]$. Set $C_p=\{[\bar\Phi_p(u)]:u\in E_p^\times\}$, the subgroup called the nonsplit torus because it is the projective image of the multiplicative group of this degree-two field extension. The projective reduction of $j$ is $\rho_p(j)=[\bar\Phi_p(\bar j)]$. Define $K_p=C_p\cup C_p\rho_p(j)$, where the right coset $C_p\rho_p(j)$ consists of the products $c\rho_p(j)$ with $c\in C_p$.

Conjugation by $\bar j$, the map $x\mapsto\bar j x\bar j^{-1}$, acts on $E_p$ by $a+b\bar i\mapsto a-b\bar i$. An $\mathbb F_p$-automorphism of $E_p$ is a bijection preserving addition, multiplication and $1$ and fixing each element of $\mathbb F_p$. The conjugation is the unique nonidentity such automorphism, the relative Frobenius $x\mapsto x^p$. The full normalizer $N_{G_p}(C_p)=\{g\in G_p:gC_pg^{-1}=C_p\}$, with $gC_pg^{-1}$ the set of conjugates of the elements of $C_p$ by $g$, is $K_p$. Its order, the number of its elements, is $2(p+1)$.

## Statement references

[[def-euler-prime-classes]]

[[math:def-integers-modulo-n]]

[[math:def-addition-and-multiplication-modulo-n]]

[[math:thm-z-mod-p-is-a-field]]

[[def-euler-hamilton-quaternions]]

[[def-euler-hurwitz-order]]

[[math:def-quotient-ring]]

[[lem-euler-hurwitz-odd-split-reduction]]

[[def-euler-hurwitz-torus-normalizer]]

[[math:def-field]]

[[math:def-field-extension-generated-subfields-and-simple-extension]]

[[math:def-extension-degree-and-finite-extension]]

[[math:def-linear-basis]]

[[math:def-dimension]]

[[math:def-field-homomorphism]]

[[math:def-f-homomorphisms-and-embeddings-of-field-extensions]]

[[math:def-relative-frobenius-of-a-finite-field-extension]]

[[def-degree-two-projective-linear-group]]

[[def-euler-hurwitz-projective-reduction]]

[[math:def-coset]]

[[math:def-normalizer-of-a-subgroup]]

[[math:def-finite-cardinality]]

[[math:def-ring-matrix-product-identity-and-transpose]]

[[math:def-subgroup]]

## Facts & Assumptions

[F1] For $p\in\mathcal P_3$, $p$ is an odd prime. The residue classes modulo $p$ form a field under operations on representatives, and $0,\ldots,p-1$ give precisely $p$ classes. In particular $2\ne0$ in $\mathbb F_p$. [[def-euler-prime-classes]] [[math:def-integers-modulo-n]] [[math:def-addition-and-multiplication-modulo-n]] [[math:thm-z-mod-p-is-a-field]] [[math:thm-standard-representatives-modulo-n]]

[F2] The elements $i,j$ lie in $\mathcal H$ and the quotient map uses sums and products of representatives. Thus $\bar i^2=\bar j^2=-1$ and $\bar j\bar i=-\bar i\bar j$. The reduction isomorphism sends $t1$ to $tI_2$ for $t\in\mathbb F_p$, where $I_2$ has diagonal entries $1$ and off-diagonal entries $0$. [[def-euler-hamilton-quaternions]] [[def-euler-hurwitz-order]] [[math:def-quotient-ring]] [[lem-euler-hurwitz-odd-split-reduction]]

[F3] The field $E_p$ contains the scalar copy of $\mathbb F_p$, has $p^2$ elements and has ordered basis $(1,\bar i)$ over $\mathbb F_p$. Every element has unique coordinates $a,b$. As the basis has two vectors, $\dim_{\mathbb F_p} E_p=2$, so the extension degree $[E_p:\mathbb F_p]$ is two. Every nonzero field element has a multiplicative inverse in the field. [[def-euler-hurwitz-torus-normalizer]] [[math:def-field]] [[math:def-field-extension-generated-subfields-and-simple-extension]] [[math:def-extension-degree-and-finite-extension]] [[math:def-linear-basis]] [[math:def-dimension]]

[F4] An $\mathbb F_p$-automorphism is a bijection preserving addition, multiplication and $1$ and fixing $\mathbb F_p$ pointwise. For a degree-two extension of a finite field of $p$ elements, the only automorphisms fixing the base field are the identity and the relative Frobenius $x\mapsto x^p$. [[math:def-field-homomorphism]] [[math:def-f-homomorphisms-and-embeddings-of-field-extensions]] [[math:def-relative-frobenius-of-a-finite-field-extension]] [[math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group]]

[F5] Projective classes are given by nonzero scalar multiples and multiply by multiplying their matrices. The projective reduction of the Hurwitz unit $j$ is the class of $\bar\Phi_p(\bar j)$. A subgroup contains the group identity and is closed under products and inverses. For a subgroup $H$, a right coset $Hg$ is the set of products $hg$ with $h\in H$. The normalizer consists of those group elements carrying $H$ onto itself by conjugation and is a subgroup. A bijection of finite sets preserves their numbers of elements. [[def-degree-two-projective-linear-group]] [[def-euler-hurwitz-projective-reduction]] [[math:def-coset]] [[math:def-normalizer-of-a-subgroup]] [[math:lem-centralizers-and-normalizers-are-subgroups]] [[math:def-finite-cardinality]] [[math:def-subgroup]]

[F6] Matrix products are row-by-column, associative and distributive, with scalar matrices acting on columns by the indicated scalars. A linear map preserves linear combinations. In an ordered basis the columns of its matrix are the coordinate columns of the images of the basis vectors. [[math:def-ring-matrix-product-identity-and-transpose]] [[math:thm-ring-matrix-arithmetic-laws]] [[math:def-linear-map]] [[math:def-coordinate-column-and-matrix-of-a-linear-map]]

[F7] For a finite field $F$ of $q$ elements and a field extension $E/F$ of degree two, fix an ordered $F$-basis of $E$. Let $m_u$ denote multiplication by $u$ on $E$, and write $[S]$ for the projective class of the matrix of an invertible $F$-linear map $S:E\to E$ in that basis. For $T=\{[m_u]:u\in E^\times\}$ and $\sigma_q(x)=x^q$, the normalizer of $T$ in $\mathrm{PGL}_2(F)$ is the disjoint union $T\cup T[\sigma_q]$ and has order $2(q+1)$. [[lem-quadratic-field-normalizer-in-degree-two]]

[F8] For composable linear maps $T:U\to V$ and $S:V\to W$, the matrix of $S\circ T$ is the matrix of $S$ times the matrix of $T$, using ordered bases of the three spaces and the same basis of $V$ for both matrices. [[math:thm-matrix-of-a-composite-is-the-product]]

[F9] A linear map is invertible when it has a two-sided linear inverse. An invertible linear map between finite-dimensional spaces has an invertible matrix in any ordered bases of its domain and codomain. [[math:def-linear-isomorphism-and-invertible-linear-map]] [[math:thm-invertible-matrices-correspond-to-linear-isomorphisms]]

## Proof

**Given:** $p\in\mathcal P_3$, the reduced Hurwitz order $R_p$ and the fixed realization $\bar\Phi_p$.

**Goal:** Identify the automorphism on $E_p$ induced by $\bar j$ and prove $K_p=N_{G_p}(C_p)$ and $|K_p|=2(p+1)$.

1.1 Since $\bar j^2=-1$, its two-sided inverse is $-\bar j$. Scalars commute with $\bar j$, and $\bar j\bar i\bar j^{-1}=-\bar i$ by the anticommutation relation. Hence $x\mapsto\bar j x\bar j^{-1}$ sends $a+b\bar i$ to $a-b\bar i$. It preserves sums and products by distributivity and $\bar j^{-1}\bar j=1$, preserves $1$, and fixes the scalars. Applying it twice returns $a+b\bar i$, so it is a bijection on $E_p$. [F2, F3, F4]

1.2 Write $M_x=\bar\Phi_p(x)$ and let $e=\binom{1}{0}$. Form the matrix $P$ with columns $e$ and $M_{\bar i}e$. If $M_{\bar i}e=\binom{s}{t}$ with $t=0$, then $(M_{\bar i}-sI_2)e=0$. But $M_{\bar i}-sI_2=M_{\bar i-s}$ is invertible, with inverse $M_{(\bar i-s)^{-1}}$, because $\bar i-s$ is a nonzero element of $E_p$ by uniqueness of its coordinates. Invertibility would give $e=0$. Hence $t\ne0$ and $P=\left(\begin{smallmatrix}1&s\\0&t\end{smallmatrix}\right)$ has two-sided inverse $\left(\begin{smallmatrix}1&-st^{-1}\\0&t^{-1}\end{smallmatrix}\right)$ by matrix multiplication. [F2, F3, F6]

2.1 Since $(1,\bar i)$ is a basis, $\bar i\ne0$. The equality $-\bar i=\bar i$ would imply $2\bar i=0$, impossible because $2$ has an inverse in $\mathbb F_p$. Thus conjugation by $\bar j$ is a nonidentity $\mathbb F_p$-automorphism. The ordered basis $(1,\bar i)$ gives $[E_p:\mathbb F_p]=2$, and $E_p$ has $p^2$ elements. The finite-field theorem therefore applies with base field of size $p$, and the conjugation map on $E_p$ is $\sigma_p(x)=x^p$. [F1, F3, F4, step 1.1]

2.2 For $z=a+b\bar i\in E_p$, write $\operatorname{col}(z)=\binom{a}{b}$. The column identity $P\operatorname{col}(z)=M_z e$ follows from $M_z=aI_2+bM_{\bar i}$. For each $u\in E_p^\times$, $M_uP\operatorname{col}(z)=M_{uz}e=P\operatorname{col}(uz)$. Multiplication by $u$ preserves $\mathbb F_p$-linear combinations by distributivity. The identity therefore shows that $P^{-1}M_uP$ is the matrix of the linear map $m_u:z\mapsto uz$ in $(1,\bar i)$. Define $\Theta([A])=[P^{-1}AP]$ on $G_p$. It is well defined because scalar multiples give scalar multiples after conjugation. It preserves products by cancellation of $PP^{-1}$, and conjugation by $P$ in place of $P^{-1}$ gives its inverse. Therefore $\Theta$ maps $C_p$ onto $T=\{[m_u]:u\in E_p^\times\}$ and carries $N_{G_p}(C_p)$ bijectively onto $N_{G_p}(T)$ by the defining conjugation equality. [F2, F3, F5, F6, F7, step 1.2]

3.1 There is a unique $d\in E_p$ with $M_{\bar j}e=P\operatorname{col}(d)$ since $P$ is invertible and the coordinates range over all pairs. Here $d\ne0$ because $M_{\bar j}$ is invertible. From $\bar j z=\sigma_p(z)\bar j$ we obtain $M_{\bar j}P\operatorname{col}(z)=M_{\sigma_p(z)}M_{\bar j}e=M_{\sigma_p(z)}P\operatorname{col}(d)=P\operatorname{col}(\sigma_p(z)d)$. The field $E_p$ is commutative, so $\sigma_p(z)d=d\sigma_p(z)$. The map $\sigma_p$ is $\mathbb F_p$-linear because it preserves sums and products and fixes the scalars. Both $m_d$ and $m_{d^{-1}}$ are linear by step 2.2, and their two composites are the identity because $dd^{-1}=d^{-1}d=1$. The linear map $\sigma_p$ is its own inverse by steps 1.1 and 2.1. Thus $m_d$ and $\sigma_p$ have invertible matrices in the ordered basis $(1,\bar i)$ of $E_p$. The column identity identifies $P^{-1}M_{\bar j}P$ with the matrix of $m_d\circ\sigma_p$ in that basis. This matrix is the product of the matrices of $m_d$ and $\sigma_p$, in that order. Passing to projective classes gives $\Theta(\rho_p(j))=[m_d][\sigma_p]$. Since $[m_d]\in T$, right multiplication by $[m_d]$ permutes $T$. Thus $\Theta(C_p\rho_p(j))=T[m_d][\sigma_p]=T[\sigma_p]$, while $\Theta(C_p)=T$. [F2, F3, F5, F6, F7, F8, F9, step 1.1, step 1.2, step 2.1, step 2.2]

4.1 Apply the quadratic-field normalizer lemma with $F=\mathbb F_p$, $q=p$, $E=E_p$ and basis $(1,\bar i)$. The base field has $p$ elements, and the two-element basis $(1,\bar i)$ gives $[E_p:\mathbb F_p]=2$. The lemma gives $N_{G_p}(T)=T\cup T[\sigma_p]$ with $2(p+1)$ elements. Since $\Theta$ carries both $K_p$ and $N_{G_p}(C_p)$ onto that set and is bijective, these two sets coincide and $K_p$ is a subgroup of order $2(p+1)$. Together with the conjugation formula this proves the statement. [F1, F3, F5, F7, step 1.1, step 2.1, step 2.2, step 3.1] ∎

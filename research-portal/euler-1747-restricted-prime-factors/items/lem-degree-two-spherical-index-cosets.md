---
id: lem-degree-two-spherical-index-cosets
kind: lemma
title: Integral determinant-index cosets in degree two
status: draft
domain: mathematics
deps:
  - math:def-prime-and-maximal-ideals
  - math:def-subgroup
  - math:thm-image-subgroup-and-kernel-normal
  - math:lem-coset-membership-and-equality
  - math:def-local-ring
  - math:def-prime
  - math:def-field-of-p-adic-numbers
  - math:def-p-adic-integers-as-compatible-residue-classes
  - def-author-24fda87362bc-local-adic-valuation
  - math:def-ring-matrix-product-identity-and-transpose
  - math:def-determinant-of-a-square-matrix
  - def-degree-two-projective-linear-group
  - math:def-coset
  - math:def-submodule
  - math:def-finite-cardinality
  - math:def-left-right-and-two-sided-ideal
  - math:def-canonical-map-from-the-integers-to-zp
  - math:thm-division-algorithm-in-z
  - math:thm-ring-matrix-arithmetic-laws
  - math:thm-determinant-multiplicative
  - math:thm-product-rule
  - math:lem-int-bounded-above-has-greatest
  - math:def-free-module-on-a-set-and-standard-basis
  - math:def-linear-combination-and-span
  - math:thm-the-integers-map-injectively-and-densely-into-zp
  - math:def-integers-modulo-n
  - math:def-congruence-modulo-an-integer
formulation_deps:
  - math:def-subgroup
  - math:thm-image-subgroup-and-kernel-normal
  - math:def-prime
  - math:def-field-of-p-adic-numbers
  - math:def-p-adic-integers-as-compatible-residue-classes
  - def-author-24fda87362bc-local-adic-valuation
  - math:def-ring-matrix-product-identity-and-transpose
  - math:def-determinant-of-a-square-matrix
  - def-degree-two-projective-linear-group
  - math:def-coset
  - math:def-submodule
  - math:def-finite-cardinality
  - math:def-left-right-and-two-sided-ideal
  - math:def-canonical-map-from-the-integers-to-zp
  - math:def-free-module-on-a-set-and-standard-basis
  - math:def-linear-combination-and-span
  - math:thm-the-integers-map-injectively-and-densely-into-zp
argument_deps:
  - math:def-prime-and-maximal-ideals
  - math:def-subgroup
  - math:thm-image-subgroup-and-kernel-normal
  - math:lem-coset-membership-and-equality
  - math:def-local-ring
  - math:def-prime
  - math:def-field-of-p-adic-numbers
  - math:def-p-adic-integers-as-compatible-residue-classes
  - def-author-24fda87362bc-local-adic-valuation
  - math:def-ring-matrix-product-identity-and-transpose
  - math:def-determinant-of-a-square-matrix
  - def-degree-two-projective-linear-group
  - math:def-coset
  - math:def-submodule
  - math:def-finite-cardinality
  - math:def-left-right-and-two-sided-ideal
  - math:def-canonical-map-from-the-integers-to-zp
  - math:thm-division-algorithm-in-z
  - math:thm-ring-matrix-arithmetic-laws
  - math:thm-determinant-multiplicative
  - math:thm-product-rule
  - math:lem-int-bounded-above-has-greatest
  - math:def-free-module-on-a-set-and-standard-basis
  - math:def-linear-combination-and-span
  - math:thm-the-integers-map-injectively-and-densely-into-zp
  - math:def-integers-modulo-n
  - math:def-congruence-modulo-an-integer
dependency_roles:
  math:def-prime-and-maximal-ideals: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:thm-image-subgroup-and-kernel-normal: mathematical-premise
  math:lem-coset-membership-and-equality: mathematical-premise
  math:def-local-ring: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-field-of-p-adic-numbers: mathematical-premise
  math:def-p-adic-integers-as-compatible-residue-classes: mathematical-premise
  def-author-24fda87362bc-local-adic-valuation: mathematical-premise
  math:def-ring-matrix-product-identity-and-transpose: mathematical-premise
  math:def-determinant-of-a-square-matrix: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-submodule: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-left-right-and-two-sided-ideal: mathematical-premise
  math:def-canonical-map-from-the-integers-to-zp: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:thm-ring-matrix-arithmetic-laws: mathematical-premise
  math:thm-determinant-multiplicative: mathematical-premise
  math:thm-product-rule: mathematical-premise
  math:lem-int-bounded-above-has-greatest: mathematical-premise
  math:def-free-module-on-a-set-and-standard-basis: mathematical-premise
  math:def-linear-combination-and-span: mathematical-premise
  math:thm-the-integers-map-injectively-and-densely-into-zp: mathematical-premise
  math:def-integers-modulo-n: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Let $\ell$ be prime, let $F=\mathbb Q_\ell$ be the field of $\ell$-adic numbers, and let $R=\mathbb Z_\ell\subset F$ be the ring of $\ell$-adic integers. Write $v=v_\ell$ for the valuation with $v(\ell)=1$. For a nonnegative integer $n$, let $B_n=\{0,\ldots,\ell^n-1\}\subset R$ via the canonical integer embedding. For a nonnegative integer $e$, set
$$D_e=\{A\in M_2(R):\det A\ne0,\ v(\det A)=e\}.$$
Here $M_2(R)$ is the ring of two-by-two matrices over $R$ with matrix multiplication, and $\det\begin{pmatrix}a&b\\c&d\end{pmatrix}=ad-bc$.

Put $H=\mathrm{GL}_2(R)$, the group of two-by-two matrices with two-sided inverses over $R$. Consider the cosets $AH=\{AU:U\in H\}$ for right multiplication on $D_e$.

For $S=R$ or $S=F$, write $S^2$ for the set of columns $(x_1,x_2)^{\mathsf T}$ with $x_1,x_2\in S$, with addition and scalar multiplication in each coordinate. A column lattice in $R^2$ means an $R$-submodule $L$ such that every vector in $F^2$ is a finite $F$-linear combination of elements of $L$. A finite $F$-linear combination of vectors in $L$ has the form $\sum_{i=1}^m c_i u_i$, where $c_i\in F$ and $u_i\in L$, with the empty sum equal to the zero column. As a submodule, $L$ contains zero and is closed under differences and multiplication by scalars in $R$. Its index $[R^2:L]$, when finite, is the number of additive cosets $x+L=\{x+y:y\in L\}$.

The columns of $A$ generate $AR^2=\{Ax:x\in R^2\}$. The map $AH\mapsto AR^2$ is a bijection onto the column lattices of index $\ell^e$. Each coset has exactly one representative
$$T_{r,b}=\begin{pmatrix}\ell^r&b\\0&\ell^{e-r}\end{pmatrix},\qquad 0\le r\le e,\quad b\in B_r.$$
For each $r$ this gives $\ell^r$ representatives, one for each residue modulo $\ell^rR$.

Write $G=\mathrm{PGL}_2(F)$ for the quotient of $\mathrm{GL}_2(F)$ by nonzero scalar matrices, so $[A]=[B]$ means $B=\lambda A$ for some $\lambda\in F^\times$. Let $K$ be the image of $H$ in $G$. The natural map identifies $\mathrm{PGL}_2(R)$, the quotient of $H$ by scalar matrices with invertible scalars in $R$, with $K$. The map $AH\mapsto[A]K$ is a bijection onto the cosets for right multiplication by $K$ in the projective image of $D_e$.

The principal matrix right ideal $AM_2(R)=\{AC:C\in M_2(R)\}$ consists exactly of the matrices with both columns in $AR^2$. A right ideal is an additive subgroup stable under multiplication on the right by the ring. Two matrices in $D_e$ generate the same right ideal exactly when their column lattices agree.

## Facts & Assumptions

[F1] The prime $\ell$ is an integer greater than one whose only positive divisors are one and itself ([[math:def-prime]]). The field $F$ is the completion of $\mathbb Q$ for the $\ell$-adic distance ([[math:def-field-of-p-adic-numbers]], [[def-author-24fda87362bc-local-adic-valuation]]). In $F$, $v(xy)=v(x)+v(y)$ for nonzero factors, $v(\ell)=1$, $R=\{x:v(x)\ge0\}$ with $v(0)=+\infty$, and the units of $R$ are the elements of valuation zero ([[def-author-24fda87362bc-local-adic-valuation]]).

[F2] Elements of $R$ are compatible tuples of integer residue classes modulo $\ell^j$ for $j\ge1$, with coordinatewise operations ([[math:def-p-adic-integers-as-compatible-residue-classes]], [[def-author-24fda87362bc-local-adic-valuation]]). For positive $m$, write $[a]_m$ for the residue class of $a$ in $\mathbb Z/m\mathbb Z$. The equality $[a]_m=[b]_m$ holds exactly when $a-b$ is an integer multiple of $m$ ([[math:def-integers-modulo-n]], [[math:def-congruence-modulo-an-integer]]). In the coordinates modulo $\ell^j$, addition and multiplication use $[a]_{\ell^j}+[b]_{\ell^j}=[a+b]_{\ell^j}$ and $[a]_{\ell^j}[b]_{\ell^j}=[ab]_{\ell^j}$ ([[def-author-24fda87362bc-local-adic-valuation]]). The canonical integer map sends $a$ to $([a]_{\ell^j})_{j\ge1}$ and is injective ([[math:def-canonical-map-from-the-integers-to-zp]], [[math:thm-the-integers-map-injectively-and-densely-into-zp]]). For positive modulus $m$, integer division gives each residue modulo $m$ a unique representative between $0$ and $m-1$ ([[math:thm-division-algorithm-in-z]]).

[F3] Matrix products take the indicated linear combinations of columns and are associative and distributive, with identity $I_2$ ([[math:def-ring-matrix-product-identity-and-transpose]], [[math:thm-ring-matrix-arithmetic-laws]]). Over the commutative rings $R$ and $F$, the two-by-two determinant expands as $ad-bc$ and satisfies $\det(AB)=\det A\det B$ ([[math:def-determinant-of-a-square-matrix]], [[math:thm-determinant-multiplicative]]).

[F4] The columns in $S^2$ form the free $S$-module on the two coordinate positions, with standard columns $(1,0)^{\mathsf T}$ and $(0,1)^{\mathsf T}$ ([[math:def-free-module-on-a-set-and-standard-basis]]). Finite $F$-linear combinations in $F^2$ use the sum of the scalar multiples of a finite list of vectors ([[math:def-linear-combination-and-span]]). An $R$-submodule of $R^2$ is an additive subgroup closed under multiplication by $R$ ([[math:def-submodule]]). For a subgroup $J$ of a group, the coset represented by $g$ for multiplication on the right by $J$ is $gJ=\{gj:j\in J\}$. In additive notation it is $g+J$ ([[math:def-coset]]).

[F5] A bijection between sets preserves finite cardinality. The product of two finite sets has cardinality the product of their cardinalities ([[math:def-finite-cardinality]], [[math:thm-product-rule]]).

[F6] Over a field or a local ring, the general linear group consists of matrices with two-sided inverses and the projective linear group is its quotient by the unit scalar matrices. Multiplication is $[A][U]=[AU]$, and inclusion of one coefficient ring into another induces the entrywise map on projective groups ([[def-degree-two-projective-linear-group]]).

[F7] A right ideal is an additive subgroup of the ring closed under right multiplication by every ring element ([[math:def-left-right-and-two-sided-ideal]]).

[F8] A nonempty set of integers with an integer lower bound has a least element ([[math:lem-int-bounded-above-has-greatest]]).

[F9] A local ring is a nonzero commutative ring with exactly one maximal ideal ([[math:def-local-ring]]). A maximal ideal is a proper ideal with no larger proper ideal containing it ([[math:def-prime-and-maximal-ideals]]).

[F10] A subgroup contains the identity and is closed under products and inverses ([[math:def-subgroup]]). The image of a group homomorphism is a subgroup of its codomain ([[math:thm-image-subgroup-and-kernel-normal]]).

[F11] In a group $G'$ with subgroup $J$, the left cosets $aJ$ and $bJ$ of elements $a,b\in G'$ agree exactly when $b=aj$ for some $j\in J$ ([[math:lem-coset-membership-and-equality]]).

## Proof

**Given:** A prime $\ell$, the rings $R\subset F$ above, and an integer $e\ge0$.

**Goal:** Classify the cosets of $D_e$ and their projective images, and identify the associated matrix right ideals.

1.1 Let $J$ be a nonzero ideal of $R$. The valuations of its nonzero elements form a nonempty set of integers bounded below by $0$. By [F8] this set has a least element $t$, attained by some $a\in J$ with $a\ne0$. For $x\in J$ with $x\ne0$, $v(x/a)=v(x)-t\ge0$, so $x\in aR$. Conversely $aR\subseteq J$. Since $a/\ell^t$ is a unit, $J=aR=\ell^tR$. These powers are distinct because $t$ is the least valuation of a nonzero element of $\ell^tR$. In particular, $\ell R$ contains exactly the nonunits and is proper since $1$ is a unit. An ideal containing an element outside $\ell R$ contains a unit and hence equals $R$. Every proper ideal is therefore contained in $\ell R$, and the maximal-ideal criterion in [F9] gives that $\ell R$ is the unique maximal ideal. The ring $R$ is commutative and contains the nonzero identity of $F$, so it is a local ring by [F9]. [F1, F7, F8, F9]

1.2 For $n\ge1$, the projection $\pi_n(x)=x_n$ is onto because each residue has an integer lift. Since the operations are coordinatewise, $\pi_n(x-z)=\pi_n(x)-\pi_n(z)$, and $\pi_n(\ell^ny)=0$ for all $y\in R$ by the residue product formula. Conversely, suppose $\pi_n(x)=0$. For each $j\ge1$, every integer representative $a_j$ of $x_{n+j}$ is divisible by $\ell^n$, since it reduces to zero modulo $\ell^n$. Define $y_j=[a_j/\ell^n]_{\ell^j}$. Changing $a_j$ changes the quotient by a multiple of $\ell^j$. Compatibility gives $a_{j+1}-a_j\in\ell^{n+j}\mathbb Z$ for any such representatives, so $y_{j+1}$ reduces to $y_j$ modulo $\ell^j$. The tuple $y\in R$ therefore satisfies $(\ell^ny)_j=[\ell^n(a_j/\ell^n)]_{\ell^j}=[a_j]_{\ell^j}=x_j$ by reduction. Thus two elements have the same projection exactly when their difference lies in $\ell^nR$. Integer division gives one lift in $B_n$ per residue, and the $\ell^n$ integers in the defining interval have distinct images in $R$. For $n=0$, $\ell^0R=R$ and $B_0=\{0\}$, which represents its single additive coset. [F2, F4, F5]

1.3 For $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ with nonzero determinant, both products with $\begin{pmatrix}d&-b\\-c&a\end{pmatrix}$ equal $(\det A)I_2$. Dividing the second matrix by $\det A$ gives the inverse over $F$, and over $R$ when the determinant is a unit. Conversely, an inverse over $R$ has determinant multiplying $\det A$ to $1$ by multiplicativity. Hence $v(\det U)=0$ for $U\in H$, and every product $AU$ for $A\in D_e$ and $U\in H$ again belongs to $D_e$. The identity and matrix product on $H$ are those of $\mathrm{GL}_2(F)$, and an inverse over $R$ is also the inverse over $F$. Thus $H$ is a subgroup of $\mathrm{GL}_2(F)$ by [F10]. [F1, F3, F6, F10]

2.1 For $A\in D_e$, $AR^2$ is an $R$-submodule by the matrix laws. Every $w\in F^2$ is $A(A^{-1}w)$, an $F$-linear combination of the two columns of $A$, both of which lie in $AR^2$. For any column lattice $L$, express each of $(1,0)^{\mathsf T}$ and $(0,1)^{\mathsf T}$ as a finite $F$-linear combination of vectors in $L$. Multiplying both expressions by a sufficiently large common power $\ell^N$ makes all coefficients integral by their valuations. The two scaled standard columns lie in $L$ and every column of $\ell^N R^2$ is an $R$-linear combination of them. Thus $\ell^N R^2\subseteq L$. The sets $J_1=\{x\in R:(x,0)^{\mathsf T}\in L\}$ and $J_2=\{y\in R:(x,y)^{\mathsf T}\in L\text{ for some }x\}$ are ideals by closure under differences and $R$-scalars, and each contains $\ell^N$. Write $J_1=\ell^rR$ and $J_2=\ell^sR$ by step 1.1. Take a vector $(b',\ell^s)^{\mathsf T}$ in $L$ and subtract a multiple of $(\ell^r,0)^{\mathsf T}$ to obtain $(b,\ell^s)^{\mathsf T}$ with $b\in B_r$. Every vector in $L$ can now be reduced to the first axis by subtracting an $R$-multiple of $(b,\ell^s)^{\mathsf T}$. Hence $L=TR^2$ for $T=\begin{pmatrix}\ell^r&b\\0&\ell^s\end{pmatrix}$. The two ideals determine $r,s$, and two lifts of $\ell^s$ differ in first coordinate by an element of $\ell^rR$. Thus $b\in B_r$ is determined by $L$. [F1, F3, F4, step 1.1, step 1.2, step 1.3]

2.2 The local ring $R$ embeds in $F$, so [F6] gives the entrywise homomorphism $\mathrm{PGL}_2(R)\to G$. Since every class of $\mathrm{PGL}_2(R)$ has a representative in $H$, the image of this homomorphism is $K$, a subgroup of $G$ by [F10]. If $U,V\in H$ and $U=\lambda V$ for $\lambda\in F^\times$, then $UV^{-1}=\lambda I_2\in H$. The entries of $\lambda I_2$ and its inverse lie in $R$, so $\lambda$ is a unit of $R$. Thus the map identifies $\mathrm{PGL}_2(R)$ with $K$. For $A,B\in D_e$, equality $[A]K=[B]K$ gives $[B]=[AU]$ for some $U\in H$, hence $B=\lambda AU$ for a nonzero $\lambda\in F$. Taking determinant valuations gives $e=2v(\lambda)+e$ because $\det(\lambda AU)=\lambda^2\det A\det U$. Thus $\lambda\in R^\times$ and $B=A(\lambda U)$ with $\lambda U\in H$, so $AH=BH$ by [F11]. Conversely, if $AH=BH$, then $B=AU$ for some $U\in H$ by [F11]. As $[B]=[A][U]$ with $[U]\in K$, [F11] gives $[A]K=[B]K$. The projective image is stable under right multiplication by $K$ because $[A][U]=[AU]$ and $AU\in D_e$ by step 1.3. Each of its cosets has a representative $[A]$ with $A\in D_e$. [F1, F3, F4, F6, F10, F11, step 1.1, step 1.3]

3.1 For $L=TR^2$, regard $L$ as a subgroup of the additive group $R^2$. By [F11] in additive notation, two columns represent the same coset exactly when their difference belongs to $L$. Each additive coset in $R^2/L$ has a representative $(a,z)^{\mathsf T}$ with $(a,z)\in B_r\times B_s$. Subtract a multiple of the second column to put the second coordinate in $B_s$, then a multiple of the first column to put the first coordinate in $B_r$. If two representatives differ by an element of $L$, their second coordinates agree by reduction modulo $\ell^sR$. Their first coordinates then differ by an element of $\ell^rR$, so they agree as well. The index is therefore $\ell^r\ell^s=\ell^{r+s}$. The determinant of $T$ is $\ell^{r+s}$. Conversely any such $T$ with $r,s\ge0$ and $b\in B_r$ has this determinant and gives the same index calculation. [F1, F3, F4, F5, F11, step 1.2, step 1.3, step 2.1]

4.1 If $AH=BH$, then $B=AU$ with $U\in H$ by [F11]. Since $U$ and $U^{-1}$ both send $R^2$ into itself, $UR^2=R^2$, so $BR^2=AR^2$. If $A,B\in D_e$ have $AR^2=BR^2$, writing the columns of each in terms of the columns of the other gives $B=AU$ and $A=BV$ with $U,V\in M_2(R)$. Then $A=AUV$ and $B=BVU$. Multiplying by the respective inverses over $F$ shows $UV=VU=I_2$, so $U\in H$ and [F11] gives $AH=BH$. This same calculation works for any two integral matrices with nonzero determinant and equal column lattices. Applied to $A$ and the $T$ of step 2.1, it gives $T=AU$ with $U\in H$, so $r+s=v(\det T)=e$. Conversely every lattice of index $\ell^e$ yields such a $T$ in $D_e$ by step 3.1. Thus the lattice bijection and the unique representatives $T_{r,b}$ follow. The $\ell^r$ choices of $b$ give the claimed multiplicity. [F1, F3, F4, F5, F6, F11, step 1.2, step 1.3, step 2.1, step 3.1]

5.1 The set $AM_2(R)$ contains the zero matrix and is a right ideal because $AC-AC'=A(C-C')$ and $(AC)C'=A(CC')$. Each column of $AC$ is $A$ times the corresponding column of $C$, so both lie in $AR^2$. Conversely, if the columns of a matrix lie in $AR^2$, take their preimages under $A$ in $R^2$ as the columns of $C$. This gives the required matrix $AC$. The column lattice is recoverable from the ideal by taking first columns of its matrices, since any vector in $AR^2$ occurs as the first column with zero second column. Thus equality of the ideals is equivalent to equality of the lattices, completing the classifications. [F3, F7, step 4.1, step 2.2] ∎

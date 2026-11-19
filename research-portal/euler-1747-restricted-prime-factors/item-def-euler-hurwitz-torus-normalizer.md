---
title: The nonsplit torus and its normalizer
status: draft
research_item: def-euler-hurwitz-torus-normalizer
dependency_level: 5
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §3.3, opening definitions of the two subgroups
---

PDF p. 4: ` §3.3, opening definitions of the two subgroups `

## Prerequisites

- [math:def-linear-combination-and-span](https://alphabetamath.cc/item/def-linear-combination-and-span)
- [math:def-linear-independence](https://alphabetamath.cc/item/def-linear-independence)
- [math:lem-span-is-the-set-of-linear-combinations](https://alphabetamath.cc/item/lem-span-is-the-set-of-linear-combinations)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:def-vector-space](https://alphabetamath.cc/item/def-vector-space)
- [math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction)
- [lem-euler-nonsplit-square-obstruction](item-lem-euler-nonsplit-square-obstruction)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)
- [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:thm-standard-representatives-modulo-n](https://alphabetamath.cc/item/thm-standard-representatives-modulo-n)
- [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)
- [math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring)
- [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)
- [math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-normal-subgroup](https://alphabetamath.cc/item/def-normal-subgroup)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)
- [math:thm-quotient-group-laws](https://alphabetamath.cc/item/thm-quotient-group-laws)
- [math:def-normalizer-of-a-subgroup](https://alphabetamath.cc/item/def-normalizer-of-a-subgroup)
- [math:lem-centralizers-and-normalizers-are-subgroups](https://alphabetamath.cc/item/lem-centralizers-and-normalizers-are-subgroups)
- [math:lem-coset-membership-and-equality](https://alphabetamath.cc/item/lem-coset-membership-and-equality)


## Definition

Let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$. Write $\mathbb F_p=\mathbb Z/p\mathbb Z$ for the field of integer residue classes modulo $p$ with addition and multiplication on representatives. In the rational Hamilton quaternion algebra use the ordered basis $1,i,j,k$ with $i^2=j^2=-1$ and $k=ij=-ji$. Its Hurwitz order $\mathcal H$ is the subring of quaternions whose four coordinates are all integers or all integers plus $\tfrac12$.

Let $R_p=\mathcal H/p\mathcal H$ be the reduced quaternion algebra, whose elements are the additive cosets $x+p\mathcal H$ with sum and product induced from $\mathcal H$. Reduce $i,j,k$ to $\bar i,\bar j,\bar k$ in $R_p$. A scalar $t\in\mathbb F_p$ acts by multiplication by $t1$ in $R_p$. Use the fixed reduction isomorphism $\bar\Phi_p:R_p\to M_2(\mathbb F_p)$, which preserves addition, multiplication, identity and scalars. Here $M_2(\mathbb F_p)$ is the algebra of two-by-two matrices. In $G_p=\mathrm{PGL}_2(\mathbb F_p)$ two invertible matrices represent the same class exactly when they differ by multiplication by a nonzero scalar. Denote the class of $\bar\Phi_p(x)$ by $[x]$ for a unit $x$ of $R_p$. A unit has a two-sided multiplicative inverse. The product is $[x][y]=[xy]$. In particular $\rho_p(j)=[\bar j]$, the projective reduction of $j$.

Put $E_p=\mathbb F_p[i]=\{a+b\bar i:a,b\in\mathbb F_p\}\subseteq R_p$, with the inherited addition and multiplication. Write $\mathbb F_{p^2}$ for this concrete field with $p^2$ elements. For a field $F$, write $F^\times$ for its group of nonzero elements under multiplication. Define the nonsplit torus $C_p$ and its **finite torus normalizer** $K_p$ in $G_p=\mathrm{PGL}_2(\mathbb F_p)$ by
$$C_p=E_p^\times/\mathbb F_p^\times=\{[u]:u\in E_p^\times\}\subseteq G_p,\qquad K_p=C_p\cup C_p\rho_p(j).$$
Here the quotient has cosets $u\mathbb F_p^\times$ as elements and multiplies their representatives. The set $C_p\rho_p(j)$ is the right coset $\{c\rho_p(j):c\in C_p\}$. The name **nonsplit torus** refers here to the projective image of the units of the field $E_p$, which has basis $1,\bar i$ over $\mathbb F_p$. For a subgroup $H$ of a group $G$, its **normalizer** is $N_G(H)=\{g\in G:gHg^{-1}=H\}$, where $gHg^{-1}=\{ghg^{-1}:h\in H\}$. In this construction $K_p=N_{G_p}(C_p)$.

## Definition references

[def-euler-prime-classes](item-def-euler-prime-classes)

[def-euler-hurwitz-order](item-def-euler-hurwitz-order)

[def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction)

[def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)

[math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)

[math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[lem-euler-nonsplit-square-obstruction](item-lem-euler-nonsplit-square-obstruction)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring)

[math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)

[math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group)

[math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)

[math:def-coset](https://alphabetamath.cc/item/def-coset)

[math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)

[math:def-normalizer-of-a-subgroup](https://alphabetamath.cc/item/def-normalizer-of-a-subgroup)

[math:def-vector-space](https://alphabetamath.cc/item/def-vector-space)

[math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis)

[math:def-linear-combination-and-span](https://alphabetamath.cc/item/def-linear-combination-and-span)

[math:def-linear-independence](https://alphabetamath.cc/item/def-linear-independence)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

## Facts & Assumptions

[F1] For $p\in\mathcal P_3$, the congruence means $p=4h+3$ for an integer $h$, and $p$ is prime. Two integer residue classes are equal exactly when the difference of the representatives is a multiple of $p$. The operations are $[a]_p+[b]_p=[a+b]_p$ and $[a]_p[b]_p=[ab]_p$. For this prime $p$, these classes form a field, and the representatives $0,\ldots,p-1$ give exactly $p$ distinct classes. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n) [math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n) [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field) [math:thm-standard-representatives-modulo-n](https://alphabetamath.cc/item/thm-standard-representatives-modulo-n)

[F2] In $\mathcal H$ each element has unique coordinates in $1,i,j,k$ of the specified types. The quaternion multiplication has central scalars, satisfies $i^2=j^2=-1$ and $ij=k=-ji$, and distributes over addition. In the quotient ring the sum and product are obtained using representatives. Its fixed isomorphism $\bar\Phi_p$ identifies each scalar $t1$ with $tI_2$, where $I_2$ is the identity matrix. An algebra over $\mathbb F_p$ has a scalar map preserving addition, multiplication and identity whose image commutes with all its elements. [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions) [def-euler-hurwitz-order](item-def-euler-hurwitz-order) [math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring) [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction) [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)

[F3] For $p\in\mathcal P_3$ no integer satisfies $r^2\equiv-1\pmod p$. A commutative ring with distinct $0,1$ is a field when every nonzero element has a multiplicative inverse. The product of finite sets with $m$ and $n$ elements has $mn$ elements. [lem-euler-nonsplit-square-obstruction](item-lem-euler-nonsplit-square-obstruction) [math:def-field](https://alphabetamath.cc/item/def-field) [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)

[F4] Ring units form a group under multiplication. The projective reduction of a Hurwitz unit is the class of its reduced matrix under the fixed $\bar\Phi_p$. In the projective matrix group, the class of an invertible matrix consists of all its nonzero scalar multiples and the product is defined on representatives. [math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)

[F5] A subgroup contains the identity and is closed under products and inverses. A subgroup $N$ is normal if $gNg^{-1}=N$ for every ambient element $g$. For normal $N$ the cosets $gN=\{gn:n\in N\}$ form a group with product $(gN)(hN)=ghN$. A right coset is $Ng=\{ng:n\in N\}$. The elements preserving a subgroup under conjugation form its normalizer, which is a subgroup. [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup) [math:def-normal-subgroup](https://alphabetamath.cc/item/def-normal-subgroup) [math:def-coset](https://alphabetamath.cc/item/def-coset) [math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group) [math:thm-quotient-group-laws](https://alphabetamath.cc/item/thm-quotient-group-laws) [math:def-normalizer-of-a-subgroup](https://alphabetamath.cc/item/def-normalizer-of-a-subgroup) [math:lem-centralizers-and-normalizers-are-subgroups](https://alphabetamath.cc/item/lem-centralizers-and-normalizers-are-subgroups)

[F6] A vector space over a field has abelian addition and scalar multiplication satisfying the distributive, associative and identity laws. [math:def-vector-space](https://alphabetamath.cc/item/def-vector-space) A subset of a vector space is a basis when it is linearly independent and spans the space. [math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis) A set spans the space when its span equals the space. [math:def-linear-combination-and-span](https://alphabetamath.cc/item/def-linear-combination-and-span) The span of a subset is the set of all finite linear combinations of elements of that subset. [math:lem-span-is-the-set-of-linear-combinations](https://alphabetamath.cc/item/lem-span-is-the-set-of-linear-combinations) A set is linearly independent if every injective finite list from it is linearly independent. A list is linearly independent if a linear combination of the list is zero only when all its coefficients are zero. [math:def-linear-independence](https://alphabetamath.cc/item/def-linear-independence)

[F7] If a finite set $A$ admits a bijection $A\to B$, then $B$ is finite and has the same cardinality as $A$. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F8] A function is injective if equal outputs imply equal inputs, and surjective if every element of its codomain is an output. It is bijective if it is both injective and surjective. [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)

[F9] For a subgroup $H$ of a group $G$ and $a,b\in G$, the left cosets satisfy $aH=bH$ if and only if $a^{-1}b\in H$. [math:lem-coset-membership-and-equality](https://alphabetamath.cc/item/lem-coset-membership-and-equality)

## Justification

The fixed matrix realization sends the base field to scalar matrices, so equality of projective classes of field units is equality up to a factor in $\mathbb F_p^\times$. Once $E_p$ is verified to be a field, the left coset criterion identifies equality of scalar cosets with equality of projective classes. The quotient group law gives the scalar quotient as a subgroup of $G_p$. The quaternion relations give $j$ inverse $-j$ in $\mathcal H$, so its projective class defines the specified coset. The numbered argument establishes the field structure and proves that the two cosets together form the full normalizer.

## Proof

**Given:** $p\in\mathcal P_3$, the Hurwitz order $\mathcal H$ and the fixed isomorphism $\bar\Phi_p$ of its reduction.

**Goal:** Justify the field model $E_p$, the projective subgroup $C_p$ and its normalizer $K_p$.

1.1 Since $p=4h+3$, it is odd and the residue of $2$ is nonzero. Every coset in $R_p$ has a representative with integral coordinates. For coordinates all of the form $n+\tfrac12$, subtract $p(1+i+j+k)/2$, an element of $p\mathcal H$. The new coordinates are integers since $(1-p)/2$ is an integer. Conversely, if two integral representatives differ by $p$ times an element of $\mathcal H$, that element has integral coordinates. Multiplying any coordinate of the form $n+\tfrac12$ by the odd integer $p$ would leave a nonintegral coordinate. Thus two integral representatives give the same element of $R_p$ exactly when the differences of all four coordinates are multiples of $p$. [F1, F2]

2.1 Consequently every element of $R_p$ has a unique expression $a+b\bar i+c\bar j+d\bar k$ with coefficients in $\mathbb F_p$. In particular the scalar copy of $\mathbb F_p$ is embedded. In $E_p$, addition and the scalar action $t(a+b\bar i)=(ta)+(tb)\bar i$ act coordinatewise by distributivity. Consequently the additive group and scalar laws of a vector space hold componentwise by the field laws of $\mathbb F_p$. Every element $a+b\bar i$ is a linear combination of $1,\bar i$, so their span equals $E_p$ by [F6]. The two vectors are distinct by uniqueness of coordinates. In an injective list from $\{1,\bar i\}$ each occurs at most once. Any linear combination of the list is $a+b\bar i$, with coefficient zero for each omitted vector, since addition is commutative. If that combination is zero, coordinate uniqueness gives $a=b=0$. Thus every such list is linearly independent, and $\{1,\bar i\}$ is a basis by [F6]. Reduction preserves the products $\bar i^2=\bar j^2=-1$ and $\bar i\bar j=\bar k=-\bar j\bar i$. Every element can therefore be written uniquely as $u+v\bar j$ with $u,v\in E_p$. [F1, F2, F6, F8, step 1.1]

3.1 The sum and difference of two elements of $E_p$ have the stated form, and $(a+b\bar i)(c+d\bar i)=(ac-bd)+(ad+bc)\bar i$ by the reduced relations. This product is commutative, and $1\in E_p$. If $a+b\bar i\ne0$ and $b=0$, then $a^2+b^2=a^2\ne0$. If $b\ne0$ and $a^2+b^2=0$, then $(ab^{-1})^2=-1$ in $\mathbb F_p$. An integer representative of $ab^{-1}$ would contradict the square obstruction in [F3]. Hence every nonzero $a+b\bar i$ has the two-sided inverse $(a^2+b^2)^{-1}(a-b\bar i)$ in $E_p$. The inherited operations make $E_p$ a field. The product rule gives $p^2$ ordered pairs of residues by [F1] and [F3]. The map $(a,b)\mapsto a+b\bar i$ takes these pairs onto $E_p$ by definition and is injective by the uniqueness in step 2.1. It is therefore a bijection by [F8], and [F7] gives $E_p$ exactly $p^2$ elements. [F1, F2, F3, F7, F8, step 2.1]

4.1 The inverses in step 3.1 show that $E_p^\times$ consists of units of $R_p$. Its scalar subgroup $\mathbb F_p^\times$ is normal because its elements commute with all units. For $u,v\in E_p^\times$, the classes $[u]$ and $[v]$ agree exactly when $u=tv$ for some $t\in\mathbb F_p^\times$. Since the scalars are central, $u=tv$ is equivalent to $v^{-1}u=t$. Applying [F9] with $a=v$, $b=u$ and $H=\mathbb F_p^\times$ shows that $v^{-1}u\in\mathbb F_p^\times$ exactly when $v\mathbb F_p^\times=u\mathbb F_p^\times$. Thus $u\mathbb F_p^\times\mapsto[u]$ is well defined and is injective by [F8]. It preserves products and inverses because both quotient group laws use representatives. The group identity, product and inverses of its image $C_p$ are inherited from $G_p$, so $C_p$ is a subgroup. [F2, F4, F5, F8, F9, step 2.1, step 3.1]

5.1 The quaternion $j$ belongs to $\mathcal H^\times$ with inverse $-j$. Its projective reduction is $[\bar j]$, with $\bar j^{-1}=-\bar j$. Since $\bar j\bar i=-\bar i\bar j$, conjugation by $\bar j$ sends $a+b\bar i$ to $a-b\bar i$. This operation is its own inverse on $E_p$, so it maps $E_p^\times$ onto itself and $[\bar j]C_p[\bar j]^{-1}=C_p$. Each element of $C_p$ also conjugates $C_p$ onto itself by the subgroup laws. Thus $C_p$ and its coset $C_p[\bar j]$ lie in $N_{G_p}(C_p)$ by the subgroup property in [F5]. [F2, F4, F5, step 2.1, step 4.1]

5.2 Take $[x]\in N_{G_p}(C_p)$ with $x$ a unit in $R_p$, possible because $\bar\Phi_p$ is an isomorphism onto the matrix algebra. Since $[\bar i]\in C_p$, the element $[x\bar i x^{-1}]$ also belongs to $C_p$. Hence $z=x\bar i x^{-1}$ is a nonzero scalar multiple of a member of $E_p^\times$, so $z\in E_p^\times$. The relation $\bar i^2=-1$ gives $z^2=-1$. In the commutative field $E_p$, $(z-\bar i)(z+\bar i)=0$. If $z-\bar i\ne0$, multiplying by its inverse gives $z+\bar i=0$. Therefore $z=\bar i$ or $z=-\bar i$. [F2, F3, F4, F5, step 2.1, step 3.1, step 4.1]

6.1 If a unit $y=u+v\bar j$ commutes with $\bar i$, then $y\bar i-\bar i y=-2v\bar i\bar j=-2v\bar k$, by the reduced relations and commutativity of $E_p$. Since $2,\bar i,\bar j$ are units, the difference vanishes only when $v=0$. A unit of $R_p$ is nonzero since $1\ne0$, so $y\in E_p^\times$. If $z=\bar i$ in step 5.2, take $y=x$ and obtain $[x]\in C_p$. If $z=-\bar i$, then $x\bar j^{-1}$ conjugates $\bar i$ to $x(-\bar i)x^{-1}=\bar i$, using step 5.1. Thus $y=x\bar j^{-1}$ belongs to $E_p^\times$ and $[x]=[y][\bar j]\in C_p\rho_p(j)$. Together with step 5.1 this shows $K_p=N_{G_p}(C_p)$, completing the justification. [F1, F2, F4, F5, step 2.1, step 3.1, step 4.1, step 5.1, step 5.2] ∎

## Remarks

See [the finite adelic level](item-def-euler-hurwitz-adelic-level) for the adelic use of the notation $K_p$.

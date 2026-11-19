---
title: Hamilton algebras and the reduced norm
status: published
research_item: def-author-24fda87362bc-hamilton-algebra-and-reduced-norm
dependency_level: 0
---

## Prerequisites

- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:thm-rat-field](https://alphabetamath.cc/item/thm-rat-field)
- [math:def-quaternions](https://alphabetamath.cc/item/def-quaternions)
- [math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring)
- [math:lem-quaternion-conjugation-is-an-anti-involution](https://alphabetamath.cc/item/lem-quaternion-conjugation-is-an-anti-involution)
- [math:def-subfield](https://alphabetamath.cc/item/def-subfield)
- [math:def-function-space](https://alphabetamath.cc/item/def-function-space)
- [math:def-vector-space](https://alphabetamath.cc/item/def-vector-space)
- [math:lem-standard-basis-of-f-n](https://alphabetamath.cc/item/lem-standard-basis-of-f-n)
- [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order)


## Definition

Let $F$ be a field with $\mathbb Q$ as a subfield. The underlying vector space of the Hamilton algebra $B(F)$ is $F^{\{0,1,2,3\}}$, the space of quadruples over $F$. Write $1,i,j,k$ for its standard ordered basis and $x=a+bi+cj+dk$ for the quadruple with coordinates $a,b,c,d\in F$. It has coordinatewise addition and scalar multiplication, and multiplication that is linear over $F$ in each factor, with identity $1$ and table $i^2=j^2=k^2=-1$, $ij=k$, $jk=i$, $ki=j$, $ji=-k$, $kj=-i$, and $ik=-j$. A scalar $a$ is identified with $a\cdot1$. Write $B=B(\mathbb Q)$ for the rational Hamilton algebra. The conjugate of $x$ is $\bar x=a-bi-cj-dk$ and its reduced norm is $N(x)=a^2+b^2+c^2+d^2\in F$, also written $\operatorname{nrd}(x)$. Use $B(F)^\times$ for the units, meaning the elements with a two-sided multiplicative inverse in $B(F)$.

## Definition references

[math:def-subfield](https://alphabetamath.cc/item/def-subfield)

[math:def-function-space](https://alphabetamath.cc/item/def-function-space)

[math:lem-standard-basis-of-f-n](https://alphabetamath.cc/item/lem-standard-basis-of-f-n)

[math:def-linear-map](https://alphabetamath.cc/item/def-linear-map)

## Justification

The coefficient fields have commutative arithmetic and inverses for nonzero scalars by [math:def-field](https://alphabetamath.cc/item/def-field) and [math:thm-rat-field](https://alphabetamath.cc/item/thm-rat-field). With the pointwise operations of [math:def-function-space](https://alphabetamath.cc/item/def-function-space), the quadruples satisfy the axioms of [math:def-vector-space](https://alphabetamath.cc/item/def-vector-space). Each quadruple has a unique expansion in the ordered basis by [math:lem-standard-basis-of-f-n](https://alphabetamath.cc/item/lem-standard-basis-of-f-n). To construct the product, take each term of the first expansion and each term of the second, multiply their scalar coefficients in $F$, multiply their basis vectors by the table, and add the sixteen resulting scalar multiples. Distributivity in $F$ makes the product linear in each factor in the sense of [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map), and bilinearity forces this expansion. The table agrees with that of [math:def-quaternions](https://alphabetamath.cc/item/def-quaternions), whose real coordinate product is bilinear.

Let $\iota:\mathbb Q\to\mathbb R$ be the ordered field embedding of [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense). The table entries are signed basis vectors with coordinates in $\{0,1,-1\}$. Both bracketings of any basis triple can thus be computed over $\mathbb Q$, and applying $\iota$ to the coordinates gives the two real bracketings, which agree by [math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring). Injectivity gives equality of the rational coordinates. The inclusion of $\mathbb Q$ as a subfield of $F$ preserves its arithmetic and the constants $0,1,-1$ by [math:def-subfield](https://alphabetamath.cc/item/def-subfield), so the same equality holds over $F$. Expanding by linearity in each of the three entries extends that equality to all triples. The table gives the identity and the definition of the product gives both distributive laws. Scalars commute with every basis vector, hence with every element. These operations make $B(F)$ an associative algebra over $F$, meaning a vector space over $F$ with associative, bilinear multiplication and identity.

Conjugation is $F$-linear because leaving the scalar coordinate fixed and negating the other three commutes with taking linear combinations. For a pair of basis vectors, the coordinates on both sides of $\overline{xy}=\bar y\bar x$ are computed from the same rational table and signs. Their real images agree by [math:lem-quaternion-conjugation-is-an-anti-involution](https://alphabetamath.cc/item/lem-quaternion-conjugation-is-an-anti-involution), so injectivity of $\iota$ and the subfield inclusion give equality over $F$ on each basis pair. Both sides are bilinear, so the identity holds for all pairs. Expanding $x\bar x$ and $\bar x x$ cancels the mixed terms since distinct vectors among $i,j,k$ anticommute, meaning their products in opposite orders are negatives. Their squares are $-1$, so $x\bar x=\bar x x=N(x)\cdot1$. Therefore $(xy)\overline{xy}=x(y\bar y)\bar x=N(y)N(x)\cdot1$ and $N(xy)=N(x)N(y)$. The table and norm formula give $N(1)=1$. If $N(x)\ne0$, the formula $\bar x/N(x)$ gives a two-sided inverse. Conversely, if $x$ has inverse $y$, then $N(x)N(y)=1$.

For nonzero $x\in B$, applying $\iota$ to its four coordinates gives a nonzero real quaternion, since a nonzero coordinate stays nonzero. Preservation of addition and multiplication gives the real norm of that quaternion as $\iota(N(x))$, which is positive by [math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring). Since $\iota(0)=0$ and $\iota$ reflects strict order, $N(x)>0$ in the rational order of [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order).

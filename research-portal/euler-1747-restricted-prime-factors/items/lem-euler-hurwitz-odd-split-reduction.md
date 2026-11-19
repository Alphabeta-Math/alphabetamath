---
id: lem-euler-hurwitz-odd-split-reduction
kind: lemma
title: Split quaternion reduction at odd primes
status: published
domain: mathematics
deps:
  - math:def-left-right-and-two-sided-ideal
  - math:def-coset
  - math:def-ring-homomorphism
  - math:def-balanced-and-bilinear-maps
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - thm-hurwitz-order-integral-structure
  - math:def-prime
  - math:def-field-of-p-adic-numbers
  - math:lem-p-adic-valuation-on-q
  - math:def-p-adic-integers-as-compatible-residue-classes
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - math:def-tensor-product-of-modules-by-generators-and-relations
  - math:thm-tensor-product-of-algebras-over-a-commutative-ring
  - math:def-algebra-over-a-commutative-ring
  - math:def-matrices-over-a-commutative-ring
  - math:def-ring-matrix-product-identity-and-transpose
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - math:def-quotient-ring
  - math:def-determinant-of-a-square-matrix
  - thm-hurwitz-integral-splitting-at-odd-primes
  - math:def-p-adic-absolute-value-on-the-rationals
  - math:thm-p-adic-completion-is-a-field
  - math:def-addition-and-multiplication-modulo-n
  - math:thm-integers-modulo-n-basic-algebra
  - math:prop-elementary-tensor-formulas-descend-exactly-when-balanced
  - math:thm-ring-matrix-arithmetic-laws
  - math:thm-quotient-ring-laws
  - math:def-congruence-modulo-an-integer
  - math:def-p-adic-valuation
  - math:thm-int-comm-ring
  - math:thm-rat-field
  - math:lem-int-embeds-rat
  - math:def-subgroup
  - math:lem-coset-membership-and-equality
  - math:def-left-and-right-modules
  - math:def-field
  - math:def-ring
formulation_deps:
  - math:def-left-right-and-two-sided-ideal
  - math:def-coset
  - math:def-ring-homomorphism
  - math:def-balanced-and-bilinear-maps
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - thm-hurwitz-order-integral-structure
  - math:def-prime
  - math:def-field-of-p-adic-numbers
  - math:lem-p-adic-valuation-on-q
  - math:def-p-adic-integers-as-compatible-residue-classes
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - math:def-tensor-product-of-modules-by-generators-and-relations
  - math:thm-tensor-product-of-algebras-over-a-commutative-ring
  - math:def-algebra-over-a-commutative-ring
  - math:def-matrices-over-a-commutative-ring
  - math:def-ring-matrix-product-identity-and-transpose
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - math:def-quotient-ring
  - math:def-determinant-of-a-square-matrix
  - math:def-p-adic-absolute-value-on-the-rationals
  - math:thm-p-adic-completion-is-a-field
  - math:def-addition-and-multiplication-modulo-n
  - math:thm-integers-modulo-n-basic-algebra
  - math:prop-elementary-tensor-formulas-descend-exactly-when-balanced
  - math:thm-ring-matrix-arithmetic-laws
  - math:thm-quotient-ring-laws
  - math:def-congruence-modulo-an-integer
  - math:def-p-adic-valuation
  - math:thm-int-comm-ring
  - math:thm-rat-field
  - math:lem-int-embeds-rat
  - math:def-subgroup
  - math:def-left-and-right-modules
  - math:def-field
  - math:def-ring
argument_deps:
  - math:def-left-right-and-two-sided-ideal
  - math:def-coset
  - math:def-ring-homomorphism
  - math:def-balanced-and-bilinear-maps
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - thm-hurwitz-order-integral-structure
  - math:def-prime
  - math:def-field-of-p-adic-numbers
  - math:lem-p-adic-valuation-on-q
  - math:def-p-adic-integers-as-compatible-residue-classes
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - math:def-tensor-product-of-modules-by-generators-and-relations
  - math:thm-tensor-product-of-algebras-over-a-commutative-ring
  - math:def-algebra-over-a-commutative-ring
  - math:def-matrices-over-a-commutative-ring
  - math:def-ring-matrix-product-identity-and-transpose
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - math:def-quotient-ring
  - math:def-determinant-of-a-square-matrix
  - thm-hurwitz-integral-splitting-at-odd-primes
  - math:def-p-adic-absolute-value-on-the-rationals
  - math:thm-p-adic-completion-is-a-field
  - math:def-addition-and-multiplication-modulo-n
  - math:thm-integers-modulo-n-basic-algebra
  - math:prop-elementary-tensor-formulas-descend-exactly-when-balanced
  - math:thm-ring-matrix-arithmetic-laws
  - math:thm-quotient-ring-laws
  - math:def-congruence-modulo-an-integer
  - math:def-p-adic-valuation
  - math:thm-int-comm-ring
  - math:thm-rat-field
  - math:lem-int-embeds-rat
  - math:def-subgroup
  - math:lem-coset-membership-and-equality
  - math:def-left-and-right-modules
  - math:def-field
  - math:def-ring
dependency_roles:
  math:def-left-right-and-two-sided-ideal: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-ring-homomorphism: mathematical-premise
  math:def-balanced-and-bilinear-maps: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  thm-hurwitz-order-integral-structure: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-field-of-p-adic-numbers: mathematical-premise
  math:lem-p-adic-valuation-on-q: mathematical-premise
  math:def-p-adic-integers-as-compatible-residue-classes: mathematical-premise
  math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp: mathematical-premise
  math:def-tensor-product-of-modules-by-generators-and-relations: mathematical-premise
  math:thm-tensor-product-of-algebras-over-a-commutative-ring: mathematical-premise
  math:def-algebra-over-a-commutative-ring: mathematical-premise
  math:def-matrices-over-a-commutative-ring: mathematical-premise
  math:def-ring-matrix-product-identity-and-transpose: mathematical-premise
  math:def-integers-modulo-n: mathematical-premise
  math:thm-z-mod-p-is-a-field: mathematical-premise
  math:def-quotient-ring: mathematical-premise
  math:def-determinant-of-a-square-matrix: mathematical-premise
  thm-hurwitz-integral-splitting-at-odd-primes: mathematical-premise
  math:def-p-adic-absolute-value-on-the-rationals: mathematical-premise
  math:thm-p-adic-completion-is-a-field: mathematical-premise
  math:def-addition-and-multiplication-modulo-n: mathematical-premise
  math:thm-integers-modulo-n-basic-algebra: mathematical-premise
  math:prop-elementary-tensor-formulas-descend-exactly-when-balanced: mathematical-premise
  math:thm-ring-matrix-arithmetic-laws: mathematical-premise
  math:thm-quotient-ring-laws: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-p-adic-valuation: mathematical-premise
  math:thm-int-comm-ring: mathematical-premise
  math:thm-rat-field: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:lem-coset-membership-and-equality: mathematical-premise
  math:def-left-and-right-modules: mathematical-premise
  math:def-field: mathematical-premise
  math:def-ring: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §3.1, last paragraph
      reading_limits: The last paragraph of §3.1 on PDF page 2 was checked for attribution.
dependency_level: 3
---

## Statement

Let $p>2$ be a prime integer, so its only positive divisors are $1$ and $p$. Let $B=\mathbb Q+\mathbb Qi+\mathbb Qj+\mathbb Qk$ be the rational Hamilton quaternion algebra with $i^2=j^2=-1$ and $k=ij=-ji$. Its reduced norm is $\operatorname{nrd}(a+bi+cj+dk)=a^2+b^2+c^2+d^2$. The Hurwitz order $\mathcal H$ is the subring whose four coordinates are either all integers or all in $\mathbb Z+\tfrac12=\{n+\tfrac12:n\in\mathbb Z\}$.

Write $\mathbb Q_p$ for the field obtained by completing the rationals for the distance $|x-y|_p$. For $z\ne 0$, $|z|_p=p^{-v_p(z)}$, where $v_p$ is the exponent of $p$ in the numerator minus that in the denominator, and $|0|_p=0$. Write $\mathbb Z_p\subseteq\mathbb Q_p$ for the ring of tuples of residues modulo $p^n$ for $n\ge1$ such that each residue reduces to the preceding one. The first component gives reduction to the field $\mathbb F_p=\mathbb Z/p\mathbb Z$ of integer residues modulo $p$.

The tensor products $B\otimes_{\mathbb Q}\mathbb Q_p$ and $\mathcal H\otimes_{\mathbb Z}\mathbb Z_p$ extend scalars from $\mathbb Q$ and $\mathbb Z$, respectively. They are generated additively by symbols $x\otimes s$ additive in both entries, with $cx\otimes s=x\otimes cs$ for scalars $c$ of the original ring and product $(x\otimes s)(y\otimes t)=xy\otimes st$. For each coefficient ring $S$ here, $M_2(S)$ is the algebra of two-by-two matrices over $S$ with entrywise addition, row-by-column multiplication, and scalars acting by scalar matrices.

Then $B$ splits at $p$, meaning that there is a $\mathbb Q_p$-algebra isomorphism $\Phi:B\otimes_{\mathbb Q}\mathbb Q_p\to M_2(\mathbb Q_p)$. An algebra isomorphism is a bijection preserving addition, multiplication, identity and scalar action. The isomorphism $\Phi$ can be chosen to carry the image of $\mathcal H\otimes_{\mathbb Z}\mathbb Z_p$ onto $M_2(\mathbb Z_p)$ under the map sending $x\otimes s$ to $x\otimes s$ via the inclusions $\mathcal H\subseteq B$ and $\mathbb Z_p\subseteq\mathbb Q_p$. For this choice, reducing the entries of $\Phi(x\otimes1)$ modulo $p$ induces an $\mathbb F_p$-algebra isomorphism $\bar\Phi:\mathcal H/p\mathcal H\to M_2(\mathbb F_p)$. The quotient ring $\mathcal H/p\mathcal H$ consists of the additive cosets of $p\mathcal H=\{px:x\in\mathcal H\}$ with operations induced from $\mathcal H$ and scalar action by integer representatives. For every $x\in\mathcal H$ its reduced norm is an integer and
$$\det\bar\Phi(x+p\mathcal H)=\operatorname{nrd}(x)\bmod p,$$
where $\det$ denotes the determinant $ad-bc$ of a matrix with rows $(a,b)$ and $(c,d)$.

## Facts & Assumptions

[F1] The prime convention is that of [[math:def-prime]]. The ordered quaternion coordinates, algebra operations and norm are those of [[def-euler-hamilton-quaternions]]. The order definition [[def-euler-hurwitz-order]] uses the same coordinates. In this algebra, the order in [[thm-hurwitz-order-integral-structure]] is $O=\mathbb Z+\mathbb Zi+\mathbb Zj+\mathbb Zw$ for $w=(-1+i+j+k)/2$. It is maximal among integer orders, meaning no strictly larger subring containing $1$ is finitely generated by integer linear combinations and spans $B$ by rational linear combinations. Its coordinate set is precisely $\mathbb Z^4\cup(\mathbb Z+\tfrac12)^4$. Its reduced norm is integer-valued.

[F2] For a nonzero integer $a$, the exponent of $p$ in $a$ is the greatest nonnegative integer $k$ for which $p^k$ divides $a$, as in [[math:def-p-adic-valuation]]. The rational valuation and its absolute value are given by [[math:lem-p-adic-valuation-on-q]] and [[math:def-p-adic-absolute-value-on-the-rationals]]. The metric completion in [[math:def-field-of-p-adic-numbers]] is a field extending $\mathbb Q$ by [[math:thm-p-adic-completion-is-a-field]]. The compatible residue tuples of [[math:def-p-adic-integers-as-compatible-residue-classes]] embed canonically as a subring of that field by [[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp]]. For each $n\ge1$, the residue classes of [[math:def-integers-modulo-n]], with the representative operations of [[math:def-addition-and-multiplication-modulo-n]], form a commutative ring by [[math:thm-integers-modulo-n-basic-algebra]]. The compatible tuples use these operations componentwise. Two representatives $a,b$ give the same class modulo an integer $m$ exactly when $a-b=mq$ for some integer $q$, by [[math:def-integers-modulo-n]] and [[math:def-congruence-modulo-an-integer]]. A field has commutative multiplication by [[math:def-field]].

[F3] The base $\mathbb Z$ is a commutative ring by [[math:thm-int-comm-ring]], and $\mathbb Q$ is a field by [[math:thm-rat-field]]. The integer embedding $c\mapsto c/1$ in [[math:lem-int-embeds-rat]] preserves addition and multiplication and takes $1$ to the rational identity $1/1$. The addition and scalar identifications in the tensor products are those of [[math:def-tensor-product-of-modules-by-generators-and-relations]]. A pairing $b$ from a right module and a left module into an abelian group is balanced if it is additive in each entry and satisfies $b(xc,s)=b(x,cs)$ for every scalar $c$ and all entries $x,s$, by [[math:def-balanced-and-bilinear-maps]]. A balanced pairing defines a group homomorphism from the tensor product by [[math:prop-elementary-tensor-formulas-descend-exactly-when-balanced]]. Over the commutative base rings $\mathbb Q$ and $\mathbb Z$, [[math:thm-tensor-product-of-algebras-over-a-commutative-ring]] gives the product on elementary tensors and the identity $1\otimes1$. A unital ring homomorphism preserves addition, multiplication and the identity by [[math:def-ring-homomorphism]]. A unital algebra structure is a unital ring homomorphism from the scalars into the center as in [[math:def-algebra-over-a-commutative-ring]]. In a ring multiplication is associative and distributes over addition on both sides by [[math:def-ring]]. The actions on a right module and a left module are additive in both variables, associative with scalar multiplication, and unital by [[math:def-left-and-right-modules]].

[F4] The matrix sets, entry formulas and identity matrix are given by [[math:def-matrices-over-a-commutative-ring]] and [[math:def-ring-matrix-product-identity-and-transpose]]. Over a commutative coefficient ring the entrywise additive laws and the associative, unital and distributive multiplication laws hold by [[math:thm-ring-matrix-arithmetic-laws]]. The two-by-two determinant formula is the two-term instance of [[math:def-determinant-of-a-square-matrix]].

[F5] The residue ring modulo $p$ is a field by [[math:thm-z-mod-p-is-a-field]]. A subset of an additive group is a subgroup if it contains zero and is closed under sums and additive inverses, by [[math:def-subgroup]]. A two-sided ideal is an additive subgroup stable under multiplication by arbitrary ring elements on either side by [[math:def-left-right-and-two-sided-ideal]]. For an additive subgroup $I$ of an abelian group, its coset represented by $u$ is $u+I=\{u+y:y\in I\}$ by the additive form of [[math:def-coset]]. The coset operations of [[math:def-quotient-ring]] make the quotient by such an ideal a ring with identity by [[math:thm-quotient-ring-laws]]. For an additive subgroup $I$ of an abelian group, the cosets satisfy $u+I=v+I$ exactly when $v-u\in I$ by the additive form of [[math:lem-coset-membership-and-equality]].

[F6] For a prime $\ell>2$ and the rational Hamilton algebra with the order $O$ of [F1], [[thm-hurwitz-integral-splitting-at-odd-primes]] supplies a $\mathbb Q_\ell$-algebra isomorphism onto $M_2(\mathbb Q_\ell)$ taking the natural image of $O\otimes_{\mathbb Z}\mathbb Z_\ell$ onto $M_2(\mathbb Z_\ell)$. Reducing the entries of the image of $x\otimes1$ for $x\in O$ induces an $\mathbb F_\ell$-algebra isomorphism from $O/\ell O$. Its determinant on the coset of $x$ is the residue of the integer reduced norm of $x$.

## Proof

**Given:** A prime $p>2$, the rational Hamilton algebra $B$ and its Hurwitz order $\mathcal H$.

**Goal:** Obtain the compatible splitting and reduction isomorphisms and verify the norm–determinant formula.

1.1 If $[a]_{p^{n+1}}=[b]_{p^{n+1}}$, then $a-b=p^{n+1}q=p^n(pq)$ for some integer $q$ by [F2]. This gives $[a]_{p^n}=[b]_{p^n}$, so reduction $[a]_{p^{n+1}}\mapsto[a]_{p^n}$ is independent of the representative. Reduction preserves addition, multiplication and identity by the representative formulas. Hence compatible tuples are closed under componentwise addition, additive inverses and multiplication, and contain the identity tuple whose $n$th component is $[1]_{p^n}$. The first-component projection $\mathbb Z_p\to\mathbb F_p$ therefore preserves addition, multiplication and identity. The map $c\mapsto([c]_{p^n})_{n\ge1}$ from $\mathbb Z$ is unital and preserves sums and products by these same formulas. Both maps are unital ring homomorphisms by [F3]. The first component of the tuple for $c$ is $[c]_p$. [F2, F3, F5]

2.1 For the tensor product over $\mathbb Z$, the maps into $\mathcal H$ and $\mathbb Z_p$ are $c\mapsto c1$ and the tuple map of step 1.1. The former is the restriction of the rational scalar map of $B$ along $c\mapsto c/1$, with image in the unital subring $\mathcal H$. For the tensor product over $\mathbb Q$, the maps into $B$ and $\mathbb Q_p$ are the rational scalar map and the field inclusion of [F2]. All four maps are unital ring maps by [F1], [F2], [F3] and step 1.1. The maps into the quaternion rings are central by [F1]. The ring $\mathbb Z_p$ is commutative by its componentwise multiplication in the commutative residue rings, and $\mathbb Q_p$ has commutative multiplication because it is a field by [F2]. Hence the maps into these coefficient rings are central as well. For either base $R$, write $\eta_A$ and $\eta_S$ for the structure maps into the first and second factors. Use the right action $x\cdot c=x\eta_A(c)=\eta_A(c)x$ on the first factor and the left action $cs=\eta_S(c)s$ on the second. Distributivity gives additivity in each variable. Associativity and preservation of products give $(x\cdot c)\cdot d=x\cdot(cd)$ and $c(ds)=(cd)s$. Preservation of the identity makes $1$ act as the identity. Both actions therefore satisfy the module axioms in [F3]. The tensor-algebra theorem in [F3] thus applies to both products. In either tensor product, an element $s$ of the extended coefficient ring acts via $s\mapsto 1\otimes s$. Additivity, the product rule and the identity $1\otimes1$ give a unital ring map, and multiplying an elementary tensor $x\otimes t$ by $1\otimes s$ on either side gives $x\otimes st$, since $st=ts$. Its image is central because elementary tensors generate additively. In the target $B\otimes_{\mathbb Q}\mathbb Q_p$, the pairing $(x,s)\mapsto x\otimes s$ on $\mathcal H\times\mathbb Z_p$ is additive in each entry by the inclusion maps and tensor relations. For $c\in\mathbb Z$, the two composites into $\mathbb Q_p$, one through $\mathbb Q$ via $c\mapsto c/1$ and the other through $\mathbb Z_p$ via the tuple map of step 1.1, are unital ring maps by [F2] and [F3]. Both send $c$ to $c1_{\mathbb Q_p}$, since a unital ring map takes integer sums of $1$ and their negatives to the corresponding sums and negatives in its target. Thus $(x\cdot c)\otimes s=x\otimes(cs)$ in the target by the tensor relation over $\mathbb Q$, using agreement of the integer scalar maps and the actions just verified. Together with additivity in each entry, this makes the pairing balanced over $\mathbb Z$ by [F3]. The pairing descends to the claimed additive map from $\mathcal H\otimes_{\mathbb Z}\mathbb Z_p$ by the descent criterion in [F3]. By distributivity on both sides in the source and target tensor rings, a product of finite sums expands into a sum of products of elementary tensors. Additivity of the descended map and the elementary tensor product rule in [F3] then give multiplicativity for all tensors. The map sends $1\otimes1$ to $1\otimes1$, so it is a unital ring map. [F1, F2, F3, step 1.1]

2.2 For each coefficient ring $S$, the square matrix ring has identity $I_2$ by [F4]. The entry formulas give $(sI_2)A=A(sI_2)$ with $(i,j)$ entry $sa_{ij}$ for every matrix $A=(a_{ij})$. They also give $(s+t)I_2=sI_2+tI_2$ and $(st)I_2=(sI_2)(tI_2)$. The map sends $1$ to $I_2$. Thus by [F3] the scalar map into the matrix ring is unital and central, giving the $S$-algebra structure in the statement. [F2, F3, F4, F5, step 1.1]

3.1 The order $O$ of [F1] is in the same rational Hamilton algebra as $\mathcal H$. Since both use the basis $1,i,j,k$ and have exactly the same coordinate set, they are equal with their inherited operations. In particular $\mathcal H$ is the maximal order specified in [F6]. Apply [F6] with $\ell=p$ to obtain $\Phi$ carrying the image of $\mathcal H\otimes_{\mathbb Z}\mathbb Z_p$ under the map of step 2.1 onto $M_2(\mathbb Z_p)$. This proves the splitting at $p$. [F1, F2, F6, step 2.1, step 2.2]

4.1 The set $p\mathcal H$ contains $0=p0$. For $x,y\in\mathcal H$ it contains $px+py=p(x+y)$ and $-px=p(-x)$, since the ring $\mathcal H$ is closed under sums and additive inverses. Thus $p\mathcal H$ is an additive subgroup by [F5]. For $r,x\in\mathcal H$, centrality of the integer scalar $p1$ gives $r(px)=p(rx)$ and $(px)r=p(xr)$, both in $p\mathcal H$. By the ideal criterion in [F5], $p\mathcal H$ is a two-sided ideal. For $u\in\mathcal H$, [F5] describes its coset as the set of elements $u+px$ for $x\in\mathcal H$ and gives the ring operations on these cosets. The scalar map sends $[a]_p$ to $a1+p\mathcal H$. If $[a]_p=[b]_p$, then $a-b=pc$ for some $c\in\mathbb Z$ by [F2]. Hence $a1-b1=(a-b)1=p(c1)\in p\mathcal H$. Applying the additive coset criterion of [F5] to $b1$ and $a1$ gives $b1+p\mathcal H=a1+p\mathcal H$, so the scalar map is well defined. It preserves addition, multiplication and identity by the representative formulas, so it is a unital ring homomorphism by [F3]. Its image is central because $a1$ commutes with every quaternion in $\mathcal H$. This gives the quotient its $\mathbb F_p$-algebra structure. By step 3.1, $p\mathcal H=pO$, so $\mathcal H/p\mathcal H$ and $O/pO$ have the same cosets, ring operations and scalar action. The first-component projection in step 1.1 reduces entries and preserves matrix operations by the entry formulas in [F4]. The entrywise reduction of $\Phi(x\otimes1)$ in [F6] therefore induces the stated isomorphism on $\mathcal H/p\mathcal H$. [F1, F2, F3, F4, F5, F6, step 1.1, step 3.1]

5.1 For $x\in\mathcal H=O$, the norm in [F6] is the sum of the squares of the same four coordinates, so it equals the integer $\operatorname{nrd}(x)$ in [F1]. Its residue equals the determinant of the image of the coset $x+p\mathcal H$ by [F6] and step 4.1. In particular the norm residue depends only on the coset. This proves the norm compatibility for the reduction of the chosen splitting. [F1, F4, F5, F6, step 3.1, step 4.1] ∎

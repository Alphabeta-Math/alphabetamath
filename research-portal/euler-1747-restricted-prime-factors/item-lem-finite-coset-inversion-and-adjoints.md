---
title: Inversion and adjoints of finite-coset averaging
status: draft
research_item: lem-finite-coset-inversion-and-adjoints
dependency_level: 0
---

## Prerequisites

- [math:def-group](https://alphabetamath.cc/item/def-group)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:lem-group-inverse-laws](https://alphabetamath.cc/item/lem-group-inverse-laws)
- [math:lem-coset-partition](https://alphabetamath.cc/item/lem-coset-partition)
- [math:lem-finite-coset-partition](https://alphabetamath.cc/item/lem-finite-coset-partition)
- [math:def-multiset](https://alphabetamath.cc/item/def-multiset)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [math:lem-finite-sum-reindexing-and-fubini](https://alphabetamath.cc/item/lem-finite-sum-reindexing-and-fubini)
- [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus)
- [math:lem-complex-conjugation-and-modulus-laws](https://alphabetamath.cc/item/lem-complex-conjugation-and-modulus-laws)
- [math:lem-standard-hermitian-form-on-functions-on-a-nonempty-finite-set-is-an-inner-product](https://alphabetamath.cc/item/lem-standard-hermitian-form-on-functions-on-a-nonempty-finite-set-is-an-inner-product)
- [math:def-inner-product-space](https://alphabetamath.cc/item/def-inner-product-space)
- [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map)
- [math:def-adjoint-of-a-linear-map-between-inner-product-spaces](https://alphabetamath.cc/item/def-adjoint-of-a-linear-map-between-inner-product-spaces)
- [math:def-group-action](https://alphabetamath.cc/item/def-group-action)
- [math:def-function-space](https://alphabetamath.cc/item/def-function-space)
- [math:def-linear-subspace](https://alphabetamath.cc/item/def-linear-subspace)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-canonical-natural](https://alphabetamath.cc/item/def-canonical-natural)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:lem-of-naturals-positive](https://alphabetamath.cc/item/lem-of-naturals-positive)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)


## Statement

Let $G$ be a finite group and $H\le G$ a subgroup. Set $X=H\backslash G=\{Hg:g\in G\}$, the set of distinct right cosets $Hg=\{hg:h\in H\}$. For $Z=G$ or $X$, write $\mathbb C^Z$ for complex functions on $Z$, with pointwise vector operations and the counting inner product
$$\langle F,W\rangle_Z=\sum_{z\in Z}F(z)\overline{W(z)}.$$
Let $U=\{F\in\mathbb C^G:F(hg)=F(g)\ \text{for all }h\in H,\ g\in G\}$ be the subspace of functions invariant under left multiplication by $H$. Functions on $X$ correspond to functions in $U$ by $Jf(g)=f(Hg)$.

A multiset on $G$ assigns a nonnegative integer multiplicity $m(s)$ to each $s\in G$. Define its inverse multiset by $m^\vee(s)=m(s^{-1})$. Whenever a natural number $n$ occurs as a scalar, it means $n\cdot1_{\mathbb R}$ in the embedded real field $\mathbb R\subset\mathbb C$. Define the left translation sum $A_m$ on $\mathbb C^G$ by
$$(A_mF)(g)=\sum_{s\in G}m(s)F(sg).$$
Define right translation on $\mathbb C^X$ by $(R_r f)(Hg)=f(Hgr)$ for $r\in G$.

1. The adjoint of $A_m$ on $\mathbb C^G$ is $A_{m^\vee}$. Here the adjoint of a linear map $T$ is the linear map $T^*$ satisfying $\langle Tu,v\rangle=\langle u,T^*v\rangle$ for all $u,v$. When $A_m$ and $A_{m^\vee}$ both take $U$ into $U$, they induce maps $T_m$ and $T_{m^\vee}$ on $\mathbb C^X$ by $JT_m=A_mJ$ and $JT_{m^\vee}=A_{m^\vee}J$, and $T_m^*=T_{m^\vee}$.
2. If $m(sh)=m(s)$ for every $s\in G$ and $h\in H$, and $m(s^{-1})=m(s)$ for every $s\in G$, then $A_m$ induces $T_m$ on $\mathbb C^X$. This map is self-adjoint, meaning $T_m^*=T_m$, and commutes with right translations, meaning $T_mR_r=R_rT_m$ for every $r\in G$.

## Facts & Assumptions

[F1] A group has associative multiplication, an identity $e$ and two-sided inverses. A subgroup contains $e$ and is closed under products and inverses ([math:def-group](https://alphabetamath.cc/item/def-group), [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)).

[F2] The cosets of $H$ represented by $g$ are the sets $gH=\{gh:h\in H\}$ and $Hg=\{hg:h\in H\}$ ([math:def-coset](https://alphabetamath.cc/item/def-coset)).

[F3] Inversion is a bijection of a group onto itself, with $(s^{-1})^{-1}=s$ and $(ab)^{-1}=b^{-1}a^{-1}$ ([math:lem-group-inverse-laws](https://alphabetamath.cc/item/lem-group-inverse-laws)). The distinct left cosets $gH$ partition $G$ into nonempty disjoint sets ([math:lem-coset-partition](https://alphabetamath.cc/item/lem-coset-partition)). For a subgroup of a finite group, there are finitely many left cosets and every coset has size $|H|$, the number of elements of $H$ ([math:lem-finite-coset-partition](https://alphabetamath.cc/item/lem-finite-coset-partition)).

[F4] A finite multiset is a multiplicity function with nonnegative integer values and finitely many nonzero values. On a finite group, every such function has finitely many nonzero values ([math:def-multiset](https://alphabetamath.cc/item/def-multiset)).

[F5] Complex numbers form a field containing the real numbers. In particular, complex addition is associative and commutative and multiplication distributes over it ([math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)).

[F6] A finite sum in a commutative monoid, a set with associative and commutative addition and a zero element, is obtained by adding all terms in any enumeration. The sum is invariant under a change of index by a bijection, splits over disjoint unions and permits exchanging the order of two finite sums ([math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid), [math:lem-finite-sum-reindexing-and-fubini](https://alphabetamath.cc/item/lem-finite-sum-reindexing-and-fubini)).

[F7] For $z=a+bi$ with $a,b$ real, $\overline z=a-bi$. Conjugation fixes real scalars, preserves sums and products and is its own inverse ([math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus), [math:lem-complex-conjugation-and-modulus-laws](https://alphabetamath.cc/item/lem-complex-conjugation-and-modulus-laws)).

[F8] On complex functions on a nonempty finite set $Z$ with pointwise vector operations, the counting form divided by the positive number $|Z|$ is an inner product ([math:lem-standard-hermitian-form-on-functions-on-a-nonempty-finite-set-is-an-inner-product](https://alphabetamath.cc/item/lem-standard-hermitian-form-on-functions-on-a-nonempty-finite-set-is-an-inner-product)). In the linear-first convention an inner product is linear in its first argument and conjugate symmetric, and $\langle v,v\rangle$ is a nonnegative real number that vanishes exactly at $v=0$. Conjugate symmetry means $\langle u,v\rangle=\overline{\langle v,u\rangle}$ and yields conjugate-linearity in the second argument ([math:def-inner-product-space](https://alphabetamath.cc/item/def-inner-product-space)).

[F9] A map is linear if it preserves complex linear combinations. The adjoint is a linear map characterized by the pairing identity in the Statement ([math:def-linear-map](https://alphabetamath.cc/item/def-linear-map), [math:def-adjoint-of-a-linear-map-between-inner-product-spaces](https://alphabetamath.cc/item/def-adjoint-of-a-linear-map-between-inner-product-spaces)).

[F10] For a group acting on a set by a left action, the identity acts as the identity map and the maps for $r,t$ compose in the order $R_rR_t=R_{rt}$ ([math:def-group-action](https://alphabetamath.cc/item/def-group-action)).

[F11] For any set $Z$ and any field $K$, the functions $Z\to K$ form a vector space with pointwise operations ([math:def-function-space](https://alphabetamath.cc/item/def-function-space)). A subset of a vector space that contains zero and is closed under addition and scalar multiplication is a linear subspace with the restricted operations ([math:def-linear-subspace](https://alphabetamath.cc/item/def-linear-subspace)).

[F12] A map with a two-sided inverse is a bijection ([math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)). A bijection from a finite set transports finiteness and preserves cardinality, which is a natural number and is zero exactly for the empty set ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)). Every subset of a finite set is finite ([math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)).

[F13] The real numbers form an ordered field ([math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)). In that field set $\iota(n)=n\cdot1_{\mathbb R}$, so $\iota(0)=0$ and $\iota(n+1)=\iota(n)+1_{\mathbb R}$ ([math:def-canonical-natural](https://alphabetamath.cc/item/def-canonical-natural)). This scalar is positive for $n\ge 1$ ([math:lem-of-naturals-positive](https://alphabetamath.cc/item/lem-of-naturals-positive)).

[F14] An assertion about natural numbers holds for all of them if it holds at zero and is preserved by successor ([math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)).

## Proof

**Given:** A finite group $G$, a subgroup $H$ and a multiplicity function $m$ as in the Statement.

**Goal:** Identify the adjoint on $G$ and on the coset space under the stated preservation hypotheses, and prove the self-adjointness and commutation assertions.

1.1 The set of inverses of the elements of a left coset is $(gH)^{-1}=\{h^{-1}g^{-1}:h\in H\}=Hg^{-1}$ because inversion is a bijection on $H$. Taking elementwise inverses gives a bijection of the left-coset family onto $X$, since applying inversion again returns the original coset. Inversion also restricts to a bijection on each coset onto its image. Thus inversion carries the finite partition by left cosets to a finite partition by right cosets, each with $|H|$ elements. Both $G$ and $X$ are nonempty since $e\in G$ and $H=He$ belongs to $X$. [F1, F2, F3, F12]

2.1 For $Z=G,X$, the pointwise operations give a complex vector space by [F11]. Both sets are finite and nonempty by step 1.1 and the hypothesis on $G$. Their cardinalities are positive naturals by [F12], and their real images are positive by [F13]. Multiplying the normalized form of [F8] by the positive real scalar $|Z|$ preserves linearity, conjugate symmetry and positive definiteness, so the stated counting form is an inner product. The zero function lies in $U$ and the sum of two functions in $U$ and each scalar multiple of a function in $U$ still satisfy the defining equalities pointwise. Thus $U$ is a linear subspace by [F11], and the counting inner product restricts to it. For $h\in H$ one has $Hhg=Hg$, since multiplication by $h$ on the right is a bijection of $H$ with inverse multiplication by $h^{-1}$. Therefore $Jf$ lies in $U$. For $F\in U$, assigning $f(Hg)=F(g)$ is independent of the representative, since $Hg=Hg'$ implies $g'\in Hg$ and hence $g'=hg$ for some $h\in H$. This rule is a two-sided inverse of $J$, so $J$ is a bijection. Its pointwise formula preserves linear combinations, so $J$ is linear. [F1, F2, F5, F7, F8, F9, F11, F12, F13, step 1.1]

3.1 Split the sum on $G$ into the finitely many right cosets by iterating disjoint-union splitting. Each partial union is finite as a subset of $G$, and induction on the number of blocks starts with the empty sum and adds the contribution of the next disjoint coset. For a fixed complex value $z$, the sum of $n$ copies of $z$ equals $\iota(n)z$ by induction. The empty sum gives the case $n=0$, and the next term changes $\iota(n)z$ to $\iota(n)z+z=(\iota(n)+1_{\mathbb R})z=\iota(n+1)z$. Each coset $C$ contributes $|H|f(C)\overline{k(C)}$ to $\langle Jf,Jk\rangle_G$, since the summand is constant on $C$ and $C$ has $|H|$ elements. Hence $\langle Jf,Jk\rangle_G=|H|\langle f,k\rangle_X$, where the real scalar $|H|$ is positive because $e\in H$. [F1, F5, F6, F12, F13, F14, step 1.1, step 2.1]

3.2 Both $A_m$ and $A_{m^\vee}$ are linear by pointwise expansion of the finite sums using two-term distributivity and induction along a finite enumeration. For $s\in G$, let $L_sF(g)=F(sg)$. Changing from $g$ to $x=sg$, with inverse $g=s^{-1}x$, gives $\langle L_sF,W\rangle_G=\sum_{x\in G}F(x)\overline{W(s^{-1}x)}=\langle F,L_{s^{-1}}W\rangle_G$. Sum this identity with weights $m(s)$. Each weight is the image of $m(s)$ in the real subfield, so conjugation fixes it. First-argument linearity and second-argument conjugate-linearity extend to the finite sums by induction on the number of terms. These laws and reindexing by $t=s^{-1}$ give $\langle A_mF,W\rangle_G=\left\langle F,\sum_{s\in G}m(s)L_{s^{-1}}W\right\rangle_G=\langle F,A_{m^\vee}W\rangle_G$. The adjoint pairing determines at most one map on an inner product space. If $B$ and $D$ satisfy it for the same operator, then $\langle u,(B-D)v\rangle=0$ for every $u,v$, so choosing $u=(B-D)v$ gives $(B-D)v=0$ by positive definiteness. Thus $A_m^*=A_{m^\vee}$. [F1, F3, F4, F5, F6, F7, F8, F9, F12, F13, F14, step 2.1]

4.1 If both sums take $U$ into $U$, define $T_m=J^{-1}A_mJ$ and $T_{m^\vee}=J^{-1}A_{m^\vee}J$. For either corresponding pair $(T,A)$, the identity $JT=AJ$ and the linearity of $J$ and $A$ give $JT(af+bk)=AJ(af+bk)=aAJf+bAJk=J(aTf+bTk)$ for all $f,k\in\mathbb C^X$ and $a,b\in\mathbb C$. Injectivity of $J$ gives $T(af+bk)=aTf+bTk$, so each descended map is linear. The whole-group pairing gives $\langle JT_mf,Jk\rangle_G=\langle Jf,JT_{m^\vee}k\rangle_G$. Applying the scaling identity of step 3.1 to both sides and dividing by the positive real scalar $|H|$ gives $\langle T_mf,k\rangle_X=\langle f,T_{m^\vee}k\rangle_X$. The adjoint characterization and uniqueness give $T_m^*=T_{m^\vee}$. [F5, F9, F12, step 2.1, step 3.1, step 3.2]

5.1 If $m(sh)=m(s)$ for all $s\in G$ and $h\in H$, then for every $F\in\mathbb C^G$ and $h\in H$, $(A_mF)(hg)=\sum_{s\in G}m(s)F(shg)=\sum_{t\in G}m(th^{-1})F(tg)=(A_mF)(g)$. Here $t=sh$ is a bijective change of index with inverse $s=th^{-1}$, and $h^{-1}\in H$. Thus $A_m$ takes $U$ into $U$. If also $m(s^{-1})=m(s)$, then $m^\vee=m$, so the second operator takes $U$ into $U$ and step 4.1 gives $T_m^*=T_m$. [given, F1, F4, F6, F12, step 4.1]

6.1 For $r\in G$, the set equality $Hgr=(Hg)r$ makes right translation on cosets independent of the representative. It yields the indicated action on functions, since $R_e f=f$ and $(R_rR_t f)(Hg)=f(Hgrt)=(R_{rt}f)(Hg)$. On $\mathbb C^G$ put $(\widetilde R_rF)(g)=F(gr)$, so $JR_r=\widetilde R_rJ$. The two expressions $(A_m\widetilde R_rF)(g)$ and $(\widetilde R_rA_mF)(g)$ both equal $\sum_{s\in G}m(s)F(sgr)$ by associativity. When $A_m$ takes $U$ into $U$, the equality descends through the injective map $J$ to $T_mR_r=R_rT_m$. Together with the adjoint and self-adjointness identities above, this proves both assertions. [F1, F2, F6, F10, step 2.1, step 3.2, step 4.1, step 5.1] ∎

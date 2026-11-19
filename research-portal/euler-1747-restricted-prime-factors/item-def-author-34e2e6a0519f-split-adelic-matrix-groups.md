---
title: Split adelic matrix groups
status: published
research_item: def-author-34e2e6a0519f-split-adelic-matrix-groups
dependency_level: 2
---

## Prerequisites

- [math:def-ring](https://alphabetamath.cc/item/def-ring)
- [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring)
- [math:def-product-ring](https://alphabetamath.cc/item/def-product-ring)
- [math:def-standard-topologies](https://alphabetamath.cc/item/def-standard-topologies)
- [math:def-metric-ball](https://alphabetamath.cc/item/def-metric-ball)
- [math:lem-topological-group-translations-and-inversion](https://alphabetamath.cc/item/lem-topological-group-translations-and-inversion)
- [math:def-countable](https://alphabetamath.cc/item/def-countable)
- [math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)
- [def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles)
- [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)
- [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)
- [math:def-invertible-matrix-and-similarity-over-a-commutative-ring](https://alphabetamath.cc/item/def-invertible-matrix-and-similarity-over-a-commutative-ring)
- [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)
- [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)
- [math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)
- [math:def-multiplicative-absolute-value-on-a-field](https://alphabetamath.cc/item/def-multiplicative-absolute-value-on-a-field)
- [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)
- [math:cor-square-matrix-invertible-iff-determinant-is-a-unit](https://alphabetamath.cc/item/cor-square-matrix-invertible-iff-determinant-is-a-unit)
- [math:ex-two-by-two-determinant-formula](https://alphabetamath.cc/item/ex-two-by-two-determinant-formula)
- [math:thm-basis-criterion](https://alphabetamath.cc/item/thm-basis-criterion)
- [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)
- [math:def-topological-group](https://alphabetamath.cc/item/def-topological-group)
- [math:thm-quotient-universal-property](https://alphabetamath.cc/item/thm-quotient-universal-property)
- [math:lem-real-line-is-a-metric-space](https://alphabetamath.cc/item/lem-real-line-is-a-metric-space)
- [math:lem-of-abs-value](https://alphabetamath.cc/item/lem-of-abs-value)
- [math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group)
- [math:def-normal-subgroup](https://alphabetamath.cc/item/def-normal-subgroup)
- [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)
- [math:def-hilbert-space](https://alphabetamath.cc/item/def-hilbert-space)
- [math:def-topology-basis-subbasis](https://alphabetamath.cc/item/def-topology-basis-subbasis)
- [math:def-homeomorphism-and-open-maps](https://alphabetamath.cc/item/def-homeomorphism-and-open-maps)
- [math:lem-continuity-is-local-and-pastes](https://alphabetamath.cc/item/lem-continuity-is-local-and-pastes)
- [math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top)


## Definition

Write $\mathbb A=\mathbb R\times\mathbb A_f$ for the rational adele ring, with coordinatewise operations. Its finite tuples have entries in $\mathbb Z_\ell$ at all but finitely many primes $\ell$. Its group of units $\mathbb A^\times=\mathbb R^\times\times\mathbb A_f^\times$ has the restricted-product topology using $\mathbb Z_\ell^\times$ at the finite places. Give $\mathbb R$ its usual topology, induced by $d(x,y)=|x-y|$, and give $\mathbb R^\times$ the subspace topology from $\mathbb R$. Each $\mathbb Q_\ell$ has its $\ell$-adic topology.

The group $L=\mathrm{GL}_2(\mathbb A)$ consists of two-by-two matrices over $\mathbb A$ with a two-sided inverse over $\mathbb A$. Give each local field matrix group the subspace topology from the fourfold product of its field. Equip $L$ with the restricted-product topology of $\mathrm{GL}_2(\mathbb R)$ and the $\mathrm{GL}_2(\mathbb Q_\ell)$, using the subgroups $K_\ell=\mathrm{GL}_2(\mathbb Z_\ell)$ at the finite places. In a restricted product the tuple lies in the specified subgroup at all but finitely many places, and the basic open boxes are products of local open sets equal to the specified subgroups at all but finitely many places.

The normal scalar subgroup is $Z=\{aI:a\in\mathbb A^\times\}$, where $I$ is the identity matrix. The projective adelic matrix group is $\mathrm{PGL}_2(\mathbb A)=L/Z$ with the quotient topology. A representation has trivial central character here when each $aI$ acts as the identity.

## Definition references

[math:def-ring](https://alphabetamath.cc/item/def-ring)

[math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring)

[math:def-product-ring](https://alphabetamath.cc/item/def-product-ring)

[def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles)

[math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)

[math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)

[math:def-invertible-matrix-and-similarity-over-a-commutative-ring](https://alphabetamath.cc/item/def-invertible-matrix-and-similarity-over-a-commutative-ring)

[math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[math:def-countable](https://alphabetamath.cc/item/def-countable)

[math:def-topology-basis-subbasis](https://alphabetamath.cc/item/def-topology-basis-subbasis)

[math:thm-basis-criterion](https://alphabetamath.cc/item/thm-basis-criterion)

[math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)

[math:def-coset](https://alphabetamath.cc/item/def-coset)

[math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)

[math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)

[math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)

[math:lem-real-line-is-a-metric-space](https://alphabetamath.cc/item/lem-real-line-is-a-metric-space)

[math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group)

[math:def-normal-subgroup](https://alphabetamath.cc/item/def-normal-subgroup)

[math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)

## Facts & Assumptions

**Given:** The real and $\ell$-adic fields with their indicated topologies, and the scalar adele ring and its units.

[F1] The finite adeles form a commutative ring under coordinatewise operations. Its units are the tuples of nonzero local scalars that belong to $\mathbb Z_\ell^\times$ at all but finitely many primes. Each $\mathbb Q_\ell$ is a valued field and both $\mathbb Z_\ell$ and $\mathbb Z_\ell^\times$ are open in it. [def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles)

[F2] The real field is an ordered commutative field with its usual absolute value. On $\mathbb R$ the usual topology is the metric topology of $d(x,y)=|x-y|$. For either local field $F$, use the metric $d(x,y)=|x-y|$ from its multiplicative absolute value with the triangle inequality. In the metric topology an open set contains a ball about each of its points. For a positive radius $r$, the open ball about $x$ is $B(x,r)=\{y:d(x,y)<r\}$. [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field) [math:lem-real-line-is-a-metric-space](https://alphabetamath.cc/item/lem-real-line-is-a-metric-space) [math:lem-of-abs-value](https://alphabetamath.cc/item/lem-of-abs-value) [def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles) [math:def-multiplicative-absolute-value-on-a-field](https://alphabetamath.cc/item/def-multiplicative-absolute-value-on-a-field) [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology) [math:def-metric-ball](https://alphabetamath.cc/item/def-metric-ball)

[F3] Over a commutative ring the general linear group consists of matrices with two-sided inverses. Matrix multiplication and the identity are given by the usual entry formulas. [math:def-invertible-matrix-and-similarity-over-a-commutative-ring](https://alphabetamath.cc/item/def-invertible-matrix-and-similarity-over-a-commutative-ring) [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)

[F4] An element of a ring with identity is a unit exactly when it has a two-sided multiplicative inverse. The units form a group under multiplication. For a commutative ring $R$ and $n\geq 1$, an $n$-by-$n$ matrix over $R$ is invertible exactly when its determinant is a unit in $R$. For a two-by-two matrix with entries $a,b,c,d$ in row order its determinant is $ad-bc$. [math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group) [math:cor-square-matrix-invertible-iff-determinant-is-a-unit](https://alphabetamath.cc/item/cor-square-matrix-invertible-iff-determinant-is-a-unit) [math:ex-two-by-two-determinant-formula](https://alphabetamath.cc/item/ex-two-by-two-determinant-formula)

[F5] A covering family of subsets that is closed under binary intersections is a basis for a topology. Finite products have a basis of open rectangles, and subspace opens are traces of ambient opens. Continuity at a point can be tested by finding an input neighborhood mapped into each open neighborhood of the image. A topological group has continuous multiplication and inversion. [math:thm-basis-criterion](https://alphabetamath.cc/item/thm-basis-criterion) [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology) [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top) [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top) [math:def-topological-group](https://alphabetamath.cc/item/def-topological-group)

[F6] A subgroup is normal when conjugation by each group element maps it onto itself. For a subgroup $Z$ of $L$, the left coset of $g$ is $gZ=\{gz:z\in Z\}$. For normal $Z$, the quotient consists of these cosets and has multiplication $(gZ)(hZ)=(gh)Z$. A subset of the target of a quotient map is open exactly when its inverse image is open. A map out of the quotient is continuous exactly when its pullback along the quotient map is continuous. [math:def-normal-subgroup](https://alphabetamath.cc/item/def-normal-subgroup) [math:def-coset](https://alphabetamath.cc/item/def-coset) [math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group) [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology) [math:thm-quotient-universal-property](https://alphabetamath.cc/item/thm-quotient-universal-property)

[F7] Use the metric $d_H(v,w)=\|v-w\|$ on a complex Hilbert space $H$, with the norm induced by its inner product. A strongly continuous unitary representation is a homomorphism to the unitary operators on a complex Hilbert space whose orbit map is norm-continuous for each vector. A group homomorphism $f$ satisfies $f(gh)=f(g)f(h)$ for every $g,h$ in its domain. [math:def-hilbert-space](https://alphabetamath.cc/item/def-hilbert-space) [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology) [math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation) [math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)

[F8] The whole space, binary intersections of open sets, and arbitrary unions of open sets are open. A set is closed when its complement is open. [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)

[F9] A subset of a group is a subgroup when it contains the ambient identity and is closed under products and inverses. [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)

[F10] A finite set has a bijective listing indexed by a natural number ([math:def-countable](https://alphabetamath.cc/item/def-countable)). For a list of nonempty sets indexed by a natural number, the family of its values has a choice function ([math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice)). Evaluating that function on each entry selects one member of each listed set.

[F11] A ring has an abelian additive group, associative multiplication with identity, and both distributive laws. A commutative ring also has commutative multiplication. [math:def-ring](https://alphabetamath.cc/item/def-ring) [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring) The product of two commutative rings is a commutative ring with coordinatewise operations. [math:def-product-ring](https://alphabetamath.cc/item/def-product-ring)

[F12] The union of two finite sets is finite, and adjoining one element to a finite set gives a finite set. [Finite-set fact (ii)](https://alphabetamath.cc/item/def-standard-topologies)

[F13] For any element $z$ of a topological group, right translation by $z$ is a homeomorphism. [math:lem-topological-group-translations-and-inversion](https://alphabetamath.cc/item/lem-topological-group-translations-and-inversion) A homeomorphism has a continuous inverse. An open map sends open sets to open sets. [math:def-homeomorphism-and-open-maps](https://alphabetamath.cc/item/def-homeomorphism-and-open-maps)

[F14] The composite of two continuous maps between topological spaces is continuous. [Claim 1](https://alphabetamath.cc/item/lem-continuity-is-local-and-pastes)

[F15] A map between topological spaces is continuous exactly when the preimage of every open set is open. For parts (a) and (b), take the target topology itself as the subbasis. [math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top) [math:def-topology-basis-subbasis](https://alphabetamath.cc/item/def-topology-basis-subbasis)

## Justification

**Goal:** Verify the restricted-product realization, the group topologies, and descent of strongly continuous unitary representations with trivial scalar action.

1.1 The product of the real field and the finite adele ring uses coordinatewise operations. The additive and multiplicative identities of $\mathbb A$ are the pairs of identities in the two factors, and additive inverses are taken in each coordinate. The addition and multiplication laws, both distributive laws, and commutativity of multiplication hold in each coordinate. Thus it is a commutative unital ring. An element of it is a unit exactly when each of its two components is a unit. A two-sided inverse projects to inverses in both factors, and a pair of factor inverses gives a two-sided inverse in the product. Thus the indicated idele group and the general-ring matrix group apply. If $g\in L$, its coordinates and those of $g^{-1}$ are local inverses. The union of the eight finite entry exception sets of $g$ and $g^{-1}$ is finite by successive binary unions. Outside this union both matrices have integral entries and are inverses over $\mathbb Z_\ell$. Conversely, a tuple in the restricted product has a unique inverse at each place. At primes where the tuple belongs to $K_\ell$, that inverse is integral. The given matrices and the inverse matrices therefore assemble into two adelic matrices, and both matrix products are the identity coordinatewise. This identifies $L$ with the restricted product, with coordinatewise multiplication. [given, F1, F2, F3, F4, F11, F12]

1.2 In the absolute-value metric on either local field, increments $h,k$ at $(x,y)$ change the sum and product by at most $|h|+|k|$ and $|x||k|+|y||h|+|h||k|$, respectively. Balls are open: if $v\in B(u,r)$, the triangle inequality puts $B(v,r-d(u,v))$ inside $B(u,r)$. Given an output radius $\varepsilon>0$ at the sum or product, set $\delta=\min(1,\varepsilon/(2+|x|+|y|))$ and use the open rectangle $B(x,\delta)\times B(y,\delta)$. There the sum changes by less than $2\delta\le\varepsilon$, and the product changes by at most $(|x|+|y|+1)\delta<\varepsilon$. Negation preserves distances, so it sends $B(x,\varepsilon)$ into $B(-x,\varepsilon)$. For reciprocal at $z\ne0$ and output radius $\varepsilon>0$, use the input ball $B(z,\eta)$ with $\eta=\min(|z|/2,\varepsilon|z|^2/2)$. For $w$ in this ball, $|w|>|z|/2$ by the triangle inequality, so the ball lies in the nonzero-scalar subspace and $|w^{-1}-z^{-1}|=|w-z|/(|w||z|)<\varepsilon$. Every open neighborhood of an output contains a ball about it, or the trace of a ball for reciprocal. These input neighborhoods prove continuity by [F5]. Entry projections on the matrix input spaces are continuous by the product and subspace topologies. By composition, the entry polynomials defining matrix products and the determinant $ad-bc$ are continuous. For $g=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ invertible over the local field, $ad-bc\ne0$. Multiplying $g$ on either side by $\begin{pmatrix}d&-b\\-c&a\end{pmatrix}$ gives $(ad-bc)I$, since the diagonal entries are $ad-bc$ and the off-diagonal entries cancel. Dividing by $ad-bc$ gives the inverse. The determinant is continuous into the nonzero scalars by the subspace topology. Composing it with scalar inversion and multiplying by the adjugate entries gives continuous inverse entries. Finite rectangles test continuity of the entry tuples, and open traces test continuity into the invertible-matrix subspace. The local field matrix groups are therefore topological groups. [F2, F3, F4, F5, F14]

2.1 Each $K_\ell$ contains the ambient identity matrix. Its products and inverses are still invertible over $\mathbb Z_\ell$, so it is a subgroup of the local field matrix group. The determinant criterion over $\mathbb Z_\ell$ cuts out $K_\ell$ by requiring all entries in $\mathbb Z_\ell$ and the determinant in $\mathbb Z_\ell^\times$. Both scalar sets are open in $\mathbb Q_\ell$. Their preimages under the entry and determinant maps are open by step 1.2 and [F15], and the intersection of these five preimages is $K_\ell$. [F1, F3, F4, F8, F9, F15, step 1.2]

3.1 The restricted boxes cover $L$ by taking the full factors at the exceptional places of a tuple and the integral factors at other places. The full factors are open. Binary intersections are formed by intersecting the local open sets and still equal the integral factors off the union of the two finite exceptional sets. The union is finite by the binary union fact. The restricted boxes therefore form a basis. For a box about a product, take the real place and the finitely many primes where the target box differs from $K_\ell$ or either input lies outside $K_\ell$. The union of these three sets of primes is finite by two binary unions, and adjoining the real place gives a finite set of places. Take a bijective listing of this set by [F10]. At each listed place, the set of open rectangles containing the local input pair and having products in the target factor is nonempty by local continuity and the product basis. Apply [F10] to the list of these nonempty sets and use the selected rectangles as the finitely many local factors of the two input boxes. Elsewhere use $K_\ell$ for both inputs, since it is a subgroup. This gives an open rectangle in the product topology on $L\times L$ mapped into the target box. For inversion, the primes where the target box differs from $K_\ell$ or the input lies outside $K_\ell$ form a finite set by one binary union. Adjoin the real place and take a bijective listing by [F10]. At each listed place, local continuity gives a nonempty set of open neighborhoods of the local input whose inverses lie in the target factor. Apply [F10] to their list to select the finitely many local factors of an input box. At every other prime use $K_\ell$, which is preserved by inversion. Multiplication and inversion are continuous, so $L$ is a topological group. [F5, F8, F10, F12, step 1.1, step 1.2, step 2.1]

4.1 At a tuple in the preimage of an open local set, restrict the chosen coordinate to that set, allow the full factors at the other exceptional primes and at the real place when it is not the chosen place, and use $K_\ell$ at the remaining primes. This gives a basic box contained in the preimage, since at most the chosen place is added to the tuple's finite set of exceptional places. The preimage is a union of such boxes and hence open, so each place projection is continuous. The scalar conditions at a place are the vanishing of both off-diagonal entries and of the difference of the diagonal entries. The entry functions are continuous by composing the place projection with the local entry projections from step 1.2. The pair of diagonal entry functions is continuous by the rectangle basis. Composing with addition and negation gives a continuous difference of the diagonal entries. For $x\ne0$ in a local field, the ball $B(x,|x|/2)$ lies in the complement of zero because $d(x,0)=|x|>|x|/2>0$. The metric-topology criterion therefore makes the complement open, so zero is closed. At each point where one of the scalar condition functions is nonzero, continuity gives an open neighborhood where that function stays nonzero. The union of these neighborhoods is the complement of the simultaneous vanishing locus, so the locus is closed in $L$. A matrix in this locus has the form $aI$, and if $B$ is its adelic inverse, the first diagonal entry of $(aI)B=I$ gives $ab_{11}=1$, so $a$ is a unit by commutativity. Every scalar unit gives such a matrix, so the locus is $Z$. The map $a\mapsto aI$ sends $1$ to $I$, and $(aI)(bI)=(ab)I$ and $(aI)^{-1}=a^{-1}I$ for units $a,b$. Its image contains the ambient identity and is closed under products and inverses, so $Z$ is a subgroup. The entry formulas give $g(aI)=(aI)g$, hence $g(aI)g^{-1}=aI$ for every $g\in L$ and every $aI\in Z$. Thus conjugation by each $g\in L$ maps $Z$ onto itself, and $Z$ is central and normal. [F2, F3, F4, F5, F6, F8, F9, F12, F14, F15, step 1.1, step 1.2, step 3.1]

5.1 Set $P=L/Z$ and let $q:L\to P$ be the quotient projection $q(g)=gZ$. For $g,h\in L$, if $q(h)=q(g)$ then $h\in hZ=gZ$ since $1\in Z$. Conversely, if $h=gz$ for $z\in Z$, then $hZ=gZ$ since $zZ=Z$ by closure under products and multiplication by $z^{-1}$. Thus the fiber of $q$ over $q(g)$ is $gZ$. For open $U\subseteq L$, the set $q^{-1}(q(U))$ is the union of the right translates $Uz$ over $z\in Z$. By step 3.1, $L$ is a topological group. Right translation by $z\in Z$ is a homeomorphism by [F13]. Its inverse is right translation by $z^{-1}$, so $Uz$ is the preimage of $U$ under that continuous inverse and is open. The quotient topology makes $q(U)$ open and ensures that $q$ is continuous. Every coset has a representative, so $q$ is an open continuous surjection. The map $q\times q$ is surjective. The preimage of an open rectangle is a product of open preimages under $q$, and the image of an open rectangle is a product of open images under $q$. By the rectangle bases and preservation of unions by images and preimages, $q\times q$ sends open sets to open sets and has open preimages of open sets. Thus $q\times q$ is open and continuous. It is a quotient map since any subset with open preimage is the image of that open preimage. Inversion on $P$ pulls back along $q$ to $g\mapsto q(g^{-1})$, and coset multiplication on $P$ pulls back along $q\times q$ to $(g,h)\mapsto q(gh)$. Each pullback is continuous by composition of a continuous group operation on $L$ from step 3.1 with the continuous map $q$. The characteristic property of the respective quotient maps proves continuity of both operations on $P$. [F5, F6, F8, F9, F13, F14, F15, step 3.1, step 4.1]

6.1 Let $\pi$ be a strongly continuous unitary representation of $L$ on a complex Hilbert space $H$ acting trivially on $Z$. If $q(h)=q(g)$, then $h=gz$ for some $z\in Z$ by step 5.1. Since $\pi(h)=\pi(g)\pi(z)=\pi(g)$, the rule $\bar\pi(q(g))=\pi(g)$ is well defined with values in $U(H)$. For $g,h\in L$, the coset product gives $\bar\pi(q(g)q(h))=\bar\pi(q(gh))=\pi(gh)=\pi(g)\pi(h)=\bar\pi(q(g))\bar\pi(q(h))$. Surjectivity of $q$ makes this the homomorphism law on $P$. For each $v\in H$, the descended orbit map $p\mapsto\bar\pi(p)v$ pulls back along $q$ to the norm-continuous map $g\mapsto\pi(g)v$. The quotient-map property gives norm continuity of the descended orbit map, so the factored unitary representation is strongly continuous. [F6, F7, step 5.1] ∎

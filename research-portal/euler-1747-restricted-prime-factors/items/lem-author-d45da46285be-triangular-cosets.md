---
id: lem-author-d45da46285be-triangular-cosets
kind: lemma
title: Upper-triangular representatives of local matrix cosets
status: draft
domain: mathematics
deps:
  - math:def-topological-space
  - math:def-integer-power
  - math:lem-power-laws
  - math:lem-power-monotone
  - math:lem-of-sign-rules
  - math:def-triangular-and-diagonal-matrices-over-a-commutative-ring
  - math:def-multiplicative-absolute-value-on-a-field
  - math:lem-real-line-is-a-metric-space
  - def-degree-two-projective-linear-group
  - math:def-field-of-p-adic-numbers
  - math:thm-p-adic-completion-is-a-field
  - math:cor-zp-is-the-valuation-ring-of-qp
  - math:def-countable-choice
  - math:cor-p-adic-field-is-locally-compact-and-totally-disconnected
  - math:def-topological-group
  - math:thm-finite-products-of-compact-spaces
  - math:thm-compactness-under-continuous-maps
  - math:cor-square-matrix-invertible-iff-determinant-is-a-unit
  - math:def-quotient-topology
  - math:def-coset
  - math:def-prime
  - math:def-p-adic-absolute-value-on-the-rationals
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - math:def-quotient-ring
  - math:def-metric-topology
  - math:def-product-topology
  - math:def-subspace-topology-top
  - math:def-hausdorff-space
  - math:def-compact-space
  - math:lem-p-adic-valuation-on-q
  - math:cor-maximal-ideal-and-residue-field-of-zp
  - math:thm-z-mod-p-is-a-field
  - math:thm-standard-representatives-modulo-n
  - math:def-determinant-of-a-square-matrix
  - math:def-continuous-map-top
  - math:prop-integers-modulo-n-as-a-quotient-ring
  - math:def-metric-ball
  - math:thm-continuity-characterisations-top
  - math:thm-image-subgroup-and-kernel-normal
  - math:def-metric-space
  - math:def-homeomorphism-and-open-maps
  - math:lem-topological-group-translations-and-inversion
dependency_roles:
  math:def-topological-space: mathematical-premise
  math:def-integer-power: mathematical-premise
  math:lem-power-laws: mathematical-premise
  math:lem-power-monotone: mathematical-premise
  math:lem-of-sign-rules: mathematical-premise
  math:def-triangular-and-diagonal-matrices-over-a-commutative-ring: mathematical-premise
  math:def-multiplicative-absolute-value-on-a-field: mathematical-premise
  math:lem-real-line-is-a-metric-space: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  math:def-field-of-p-adic-numbers: mathematical-premise
  math:thm-p-adic-completion-is-a-field: mathematical-premise
  math:cor-zp-is-the-valuation-ring-of-qp: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:cor-p-adic-field-is-locally-compact-and-totally-disconnected: mathematical-premise
  math:def-topological-group: mathematical-premise
  math:thm-finite-products-of-compact-spaces: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:cor-square-matrix-invertible-iff-determinant-is-a-unit: mathematical-premise
  math:def-quotient-topology: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-p-adic-absolute-value-on-the-rationals: mathematical-premise
  math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp: mathematical-premise
  math:def-quotient-ring: mathematical-premise
  math:def-metric-topology: mathematical-premise
  math:def-product-topology: mathematical-premise
  math:def-subspace-topology-top: mathematical-premise
  math:def-hausdorff-space: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:lem-p-adic-valuation-on-q: mathematical-premise
  math:cor-maximal-ideal-and-residue-field-of-zp: mathematical-premise
  math:thm-z-mod-p-is-a-field: mathematical-premise
  math:thm-standard-representatives-modulo-n: mathematical-premise
  math:def-determinant-of-a-square-matrix: mathematical-premise
  math:def-continuous-map-top: mathematical-premise
  math:prop-integers-modulo-n-as-a-quotient-ring: mathematical-premise
  math:def-metric-ball: mathematical-premise
  math:thm-continuity-characterisations-top: mathematical-premise
  math:thm-image-subgroup-and-kernel-normal: mathematical-premise
  math:def-metric-space: mathematical-premise
  math:def-homeomorphism-and-open-maps: mathematical-premise
  math:lem-topological-group-translations-and-inversion: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
formulation_deps:
  - math:def-topological-space
  - math:def-integer-power
  - math:def-triangular-and-diagonal-matrices-over-a-commutative-ring
  - math:def-multiplicative-absolute-value-on-a-field
  - math:def-countable-choice
  - math:def-prime
  - math:def-field-of-p-adic-numbers
  - math:thm-p-adic-completion-is-a-field
  - math:def-p-adic-absolute-value-on-the-rationals
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - math:cor-zp-is-the-valuation-ring-of-qp
  - def-degree-two-projective-linear-group
  - math:def-quotient-ring
  - math:def-metric-space
  - math:def-metric-topology
  - math:def-product-topology
  - math:def-subspace-topology-top
  - math:def-quotient-topology
  - math:def-hausdorff-space
  - math:def-compact-space
  - math:def-topological-group
  - math:def-coset
argument_deps:
  - math:def-topological-space
  - math:def-integer-power
  - math:lem-power-laws
  - math:lem-power-monotone
  - math:lem-of-sign-rules
  - math:def-triangular-and-diagonal-matrices-over-a-commutative-ring
  - math:def-multiplicative-absolute-value-on-a-field
  - math:lem-real-line-is-a-metric-space
  - math:def-prime
  - math:def-countable-choice
  - math:def-field-of-p-adic-numbers
  - math:thm-p-adic-completion-is-a-field
  - math:def-p-adic-absolute-value-on-the-rationals
  - math:lem-p-adic-valuation-on-q
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - math:cor-zp-is-the-valuation-ring-of-qp
  - math:cor-p-adic-field-is-locally-compact-and-totally-disconnected
  - math:cor-maximal-ideal-and-residue-field-of-zp
  - math:thm-z-mod-p-is-a-field
  - math:thm-standard-representatives-modulo-n
  - math:def-quotient-ring
  - def-degree-two-projective-linear-group
  - math:def-determinant-of-a-square-matrix
  - math:cor-square-matrix-invertible-iff-determinant-is-a-unit
  - math:def-metric-topology
  - math:def-product-topology
  - math:def-subspace-topology-top
  - math:def-hausdorff-space
  - math:def-compact-space
  - math:def-topological-group
  - math:def-continuous-map-top
  - math:thm-finite-products-of-compact-spaces
  - math:thm-compactness-under-continuous-maps
  - math:def-quotient-topology
  - math:def-coset
  - math:prop-integers-modulo-n-as-a-quotient-ring
  - math:def-metric-ball
  - math:thm-continuity-characterisations-top
  - math:thm-image-subgroup-and-kernel-normal
  - math:def-metric-space
  - math:def-homeomorphism-and-open-maps
  - math:lem-topological-group-translations-and-inversion
---

## Statement

Assume countable choice, meaning that a sequence of nonempty sets has a choice function. For a prime $\ell$, put $F=\mathbb Q_\ell$, the completion of $\mathbb Q$ for the $\ell$-adic absolute value, and $O=\mathbb Z_\ell=\{x:|x|_\ell\le1\}$. For $x\in F^\times$, write $\nu(x)=r$ if $|x|_\ell=\ell^{-r}$. Then $\nu$ is integer valued and additive under multiplication. The ring $O$ is compact and open in $F$, its units have valuation zero, and $O/\ell O$ is a field with $\ell$ elements.

Give $F$ its $\ell$-adic metric topology, $F^4$ the product topology, and $G=\mathrm{GL}_2(F)$ and $K=\mathrm{GL}_2(O)$ the subspace topologies on their four entries in $F^4$. Give $G/Z=\mathrm{PGL}_2(F)$ the quotient topology by the scalar subgroup $Z=F^\times I$. The subgroup $K$ and its image $\bar K$ in $G/Z$ are compact and open in their respective Hausdorff topological groups.

Write $B$ for the invertible upper-triangular matrices in $G$. Every coset $gK=\{gk:k\in K\}$ has a representative $b\in B$. The exponents $(\nu(a),\nu(d))$ of the diagonal entries $(a,d)$ of $b$ depend only on $gK$.

## Facts & Assumptions

[F1] A prime is an integer greater than one with positive divisors only one and itself ([[math:def-prime]]). The $\ell$-adic field is the metric completion of the rationals with dense rational image and extended multiplicative, nonarchimedean absolute value ([[math:def-field-of-p-adic-numbers]], [[math:thm-p-adic-completion-is-a-field]]). Its absolute value vanishes exactly at zero, is multiplicative, and satisfies $|x+y|_\ell\le\max(|x|_\ell,|y|_\ell)$ for all $x,y\in F$ ([[math:def-multiplicative-absolute-value-on-a-field]]). For a nonzero rational $y$, the rational valuation $v_\ell(y)$ is an integer and $|y|_\ell=\ell^{-v_\ell(y)}$. In particular $|\ell|_\ell=\ell^{-1}$ ([[math:lem-p-adic-valuation-on-q]], [[math:def-p-adic-absolute-value-on-the-rationals]]).

[F2] Under the canonical embedding of $\mathbb Z_\ell$ into $F$, its image $O$ is the closed unit ball ([[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp]], [[math:cor-zp-is-the-valuation-ring-of-qp|The valuation ring of the p-adic field]]). It is a compact open subring under countable choice ([[math:def-countable-choice]], [[math:cor-p-adic-field-is-locally-compact-and-totally-disconnected]]).

[F3] A quotient ring by an ideal has the additive cosets as elements and uses sums and products of representatives ([[math:def-quotient-ring]]). The unique maximal ideal of $\mathbb Z_\ell$ is $\ell\mathbb Z_\ell$, and the quotient is canonically isomorphic to $\mathbb F_\ell=\mathbb Z/\ell\mathbb Z$ ([[math:cor-maximal-ideal-and-residue-field-of-zp]]). For a natural modulus $n$, the congruence-class ring $\mathbb Z/n$ is the quotient ring $\mathbb Z/n\mathbb Z$ ([[math:prop-integers-modulo-n-as-a-quotient-ring]]). For a prime $\ell$, the congruence-class ring $\mathbb Z/\ell$ is a field, and its classes have unique representatives in $\{0,\ldots,\ell-1\}$ ([[math:thm-z-mod-p-is-a-field]], [[math:thm-standard-representatives-modulo-n]]).

[F4] An ideal contains zero and is closed under differences and multiplication by arbitrary ring elements. A maximal ideal is proper and has no strictly larger proper ideal. A commutative ring with $1\ne0$ and a unique maximal ideal is local. Over a field or local ring, the matrix group consists of matrices with a two-sided inverse over that ring. In the quotient by scalars the product is $[g][h]=[gh]$ ([[def-degree-two-projective-linear-group]]). A unit of a ring is an element with a two-sided multiplicative inverse in that ring. The class of $g$ consists of the scalar multiples $zg$ with $z\in Z$. The entry formula for a matrix product is $(AB)_{ik}=a_{i1}b_{1k}+a_{i2}b_{2k}$ ([[def-degree-two-projective-linear-group]]). An upper-triangular two-by-two matrix has zero lower-left entry. Its diagonal entries are those in positions $(1,1)$ and $(2,2)$ ([[math:def-triangular-and-diagonal-matrices-over-a-commutative-ring]]). For rows $(a,b)$ and $(c,d)$, the determinant is $ad-bc$ by the two terms in the determinant formula. Invertibility over a commutative ring is equivalent to having unit determinant ([[math:def-determinant-of-a-square-matrix]], [[math:cor-square-matrix-invertible-iff-determinant-is-a-unit]]).

[F5] A metric vanishes exactly on the diagonal, is symmetric and satisfies the triangle inequality ([[math:def-metric-space]]). In a metric space with distance $d$, the open ball $B(x,r)$ of radius $r>0$ consists of points $y$ with $d(x,y)<r$ ([[math:def-metric-ball]]). A metric-open set contains a ball about each of its points. Open boxes form a basis in finite products, and the open sets of a subspace are traces of ambient open sets ([[math:def-metric-topology]], [[math:def-product-topology]], [[math:def-subspace-topology-top]]). A Hausdorff space separates distinct points by disjoint open neighborhoods. A compact space has a finite subcover for each open cover, and finite products and continuous images of compact spaces are compact ([[math:def-hausdorff-space]], [[math:def-compact-space]], [[math:thm-finite-products-of-compact-spaces]], [[math:thm-compactness-under-continuous-maps]]).

[F6] A map is continuous at every point exactly when preimages of open sets are open, equivalently when preimages of closed sets are closed. A topological group has continuous multiplication and inversion. With the quotient topology a set in the quotient is open exactly when its preimage under the projection is open ([[math:def-continuous-map-top]], [[math:thm-continuity-characterisations-top]], [[math:def-topological-group]], [[math:def-quotient-topology]]). An open map sends every open set in its domain to an open set in its codomain ([[math:def-homeomorphism-and-open-maps]]). In a topological group, right translation $R_g(x)=xg$ is a homeomorphism, a continuous bijection with continuous inverse ([[math:lem-topological-group-translations-and-inversion]], [[math:def-homeomorphism-and-open-maps]]).

[F7] For a subgroup $K$ of $G$, a coset $gK$ consists of the products $gk$ with $k\in K$. In particular it contains $g$ by taking $k=1$ ([[math:def-coset]]).

[F8] Give $\mathbb R$ its usual topology from the metric $d_{\mathbb R}(s,t)=|s-t|$ ([[math:lem-real-line-is-a-metric-space]]).

[F9] The image of a group homomorphism is a subgroup of its target group ([[math:thm-image-subgroup-and-kernel-normal]]).

[F10] For a nonzero real $a$, integer powers satisfy $a^0=1$, $a^1=a$ and $a^{-n}=1/a^n$ for positive integers $n$ ([[math:def-integer-power]]). They satisfy $a^{m+n}=a^ma^n$ for all integers $m,n$ ([[math:lem-power-laws]]). Natural powers of a positive real are positive, and $a^n>1$ when $a>1$ and $n$ is a positive integer ([[math:lem-power-monotone]]). Multiplication by a positive real preserves strict order ([[math:lem-of-sign-rules]]).

[F11] In a topology, the empty set and the whole space are open, arbitrary unions of open sets are open, and finite intersections of open sets are open. Closed sets are complements of open sets, so a finite intersection of closed sets is closed by taking the complement of a union of open sets ([[math:def-topological-space]]).

## Proof

**Given:** A prime $\ell$ and countable choice.

**Goal:** Establish the local valuation, compact open subgroups and triangular coset coordinates.

1.1 For $x\in F^\times$, choose $y\in\mathbb Q$ with $|x-y|_\ell<|x|_\ell$ by density. The strong triangle inequality in both directions gives $|x|_\ell=|y|_\ell>0$. The rational formula gives $|y|_\ell=\ell^{-v_\ell(y)}$ with $v_\ell(y)\in\mathbb Z$. For integers $r<s$, the difference $s-r$ is a positive integer. Since $\ell>1$, its natural powers are positive by [F10]. Their reciprocals are positive as well, since multiplication by a positive natural power preserves order and takes its reciprocal to $1>0$. Thus $\ell^{-r}=\ell^{-s}\ell^{s-r}>\ell^{-s}$ by [F10]. This strict decrease makes $\nu(x)$ unique. For nonzero $x_1,x_2\in F$, multiplicativity and [F10] give $|x_1x_2|_\ell=\ell^{-\nu(x_1)}\ell^{-\nu(x_2)}=\ell^{-(\nu(x_1)+\nu(x_2))}$, so uniqueness gives $\nu(x_1x_2)=\nu(x_1)+\nu(x_2)$. By the unit definition in [F4], a nonzero $x$ belongs to $O^\times$ exactly when $x$ and $x^{-1}$ both lie in the closed unit ball, which is equivalent to $|x|_\ell=1$ and hence to $\nu(x)=0$. To see that the strict unit ball is $\ell O$, suppose $|z|_\ell<1$. Then either $z=0$ or, because $\ell^0=1$ and the powers $\ell^{-r}$ strictly decrease in $r$, we have $\nu(z)\ge1$ and $|z|_\ell\le\ell^{-1}$. Hence $z/\ell\in O$. Conversely $|\ell u|_\ell\le\ell^{-1}<1$ for $u\in O$. [F1, F2, F4, F5, F10]

1.2 Write $f:\mathbb Z_\ell\to O$ for the isomorphism onto the image in [F2]. For any ideal $J$ of $\mathbb Z_\ell$, its image $f(J)$ contains $0$ and is closed under differences and multiplication by elements of $O$, since $f(a)-f(b)=f(a-b)$ and $uf(a)=f(f^{-1}(u)a)$ for $a,b\in J$ and $u\in O$. The same argument for $f^{-1}$ sends ideals of $O$ to ideals of $\mathbb Z_\ell$. Each map preserves properness and strict inclusion by bijectivity, so by [F4] they carry maximal ideals to maximal ideals. Because $f$ preserves $1$ and multiplication, $f(\ell\mathbb Z_\ell)=\ell O$. Thus $O$, a commutative subring of $F$ containing $1\ne0$, has the unique maximal ideal $\ell O$ by [F3] and is local by [F4]. The map $a+\ell\mathbb Z_\ell\mapsto f(a)+\ell O$ is well defined and bijective because two representatives differ by an element of $\ell\mathbb Z_\ell$ exactly when their images differ by an element of $\ell O$. By the operations in [F3] it preserves sums and products, so $O/\ell O$ is isomorphic to $\mathbb Z_\ell/\ell\mathbb Z_\ell$, which [F3] identifies with the ideal quotient $\mathbb Z/\ell\mathbb Z$. Since $\ell>1$ is an integer, it is a positive natural modulus, so [F3] identifies that quotient with the congruence-class ring $\mathbb Z/\ell$, a field with exactly $\ell$ elements by the unique representatives. Thus the matrix group over $O$ in [F4] applies. Entrywise inclusion $O\subset F$ preserves matrix products and the identity, and takes each two-sided inverse over $O$ to the same inverse over $F$. It embeds $K$ as a subgroup of $G$. [F1, F2, F3, F4]

1.3 If $y\in B(x,r)$, the triangle inequality gives $B(y,r-d(x,y))\subseteq B(x,r)$, so open balls are open in the metric topology. Addition is continuous since $|(x+y)-(a+b)|_\ell\le\max(|x-a|_\ell,|y-b|_\ell)$. If $|x-a|_\ell<1$, then $|x|_\ell\le\max(1,|a|_\ell)$ and $|xy-ab|_\ell\le\max(\max(1,|a|_\ell)|y-b|_\ell,|b|_\ell|x-a|_\ell)$, giving continuity of multiplication at $(a,b)$. Negation preserves distances. For $a\ne0$, if $|x-a|_\ell<|a|_\ell$ then $|x|_\ell=|a|_\ell$ and $|x^{-1}-a^{-1}|_\ell=|x-a|_\ell/|a|_\ell^2$. These estimates give continuity of inversion away from zero. They also show that the absolute value is constant on the ball of radius $|a|_\ell$ about each $a\ne0$. At zero, $d_{\mathbb R}(|x|_\ell,0)=|x|_\ell$ is the distance from $x$ to zero in $F$. Thus the absolute value is continuous into $\mathbb R$ with the topology in [F8]. For distinct points $x,y$ of a metric space, symmetry and the triangle inequality give $0=d(x,x)\le 2d(x,y)$, and separation gives $d(x,y)>0$. The open balls of radius $d(x,y)/2$ about $x$ and $y$ are disjoint. A point $z$ in both would give $d(x,y)\le d(x,z)+d(z,y)<d(x,y)$ by symmetry and the triangle inequality. In particular each singleton is closed, since its complement is the union of open balls avoiding it and hence is open by [F11]. Applying this separation in any differing coordinate makes $F^4$ Hausdorff, as is its subspace $G$. [F1, F5, F6, F8, F11]

2.1 Each projection from a finite product is continuous because the preimage of an open set is an open box. A tuple of continuous functions is continuous into a finite product because the preimage of an open box is a finite intersection of open preimages, and the preimage of a union of such boxes is a union of their preimages. Both are open by [F11]. A map with image in a subspace is continuous as a map to that subspace if its ambient-valued map is continuous, because the preimage of an open trace is the preimage of the ambient open set. For continuous $g:X\to Y$ and $f:Y\to T$ between topological spaces and open $W\subseteq T$, the identity $(f\circ g)^{-1}(W)=g^{-1}(f^{-1}(W))$ makes the preimage open by two applications of [F6]. Thus the composite is continuous by [F6]. The determinant is continuous by its entry formula, so $G=\{\det\ne0\}$ is open in $F^4$. Each entry of the matrix product is a sum of products of the input coordinates, so multiplication is continuous by the tuple and subspace rules. Swapping the diagonal entries, negating the off-diagonal entries and dividing by the determinant gives the two-sided inverse, as multiplying in both orders verifies. The inverse entries are continuous by the operations of the field from step 1.3. The same tuple and subspace rules give continuity of inversion, so $G$ is a topological group. The product topology on $O^4$ is its subspace topology from $F^4$ because open boxes restrict coordinate by coordinate. Hence $O^4$ is compact and open in $F^4$. By the determinant and unit criteria, $K=\{A\in O^4:|\det A|_\ell=1\}$. For every real $s\ne1$, the real metric ball of radius $d_{\mathbb R}(s,1)/2$ about $s$ avoids $1$, so $\{1\}$ is closed in $\mathbb R$. Composing the determinant on $O^4$ with the absolute value from step 1.3 gives the continuous function $A\mapsto |\det A|_\ell$. Its preimage of $\{1\}$ is $K$, so $K$ is closed in $O^4$. It is open in $O^4$ because the absolute value is locally constant at each nonzero determinant. It is therefore open in $G$. For any open cover of $K$, take all open subsets of $O^4$ whose traces belong to the cover and adjoin $O^4\setminus K$. A finite subcover of $O^4$ restricts to a finite subcover of $K$, proving compactness. [F2, F4, F5, F6, F8, F11, step 1.1, step 1.2, step 1.3]

2.2 Let $(c,d)$ be the bottom row of $g\in G$. It is nonzero by the determinant criterion. Divide both entries by an entry $t$ of maximal absolute value. Then $c'=c/t$ and $d'=d/t$ belong to $O$, and at least one is a unit. Choose $u,v\in O$ with $c'u+d'v=1$ by taking the inverse of a unit entry for its coefficient and zero for the other. The matrix with columns $(d',-c')^{\mathsf T}$ and $(u,v)^{\mathsf T}$ has determinant one and belongs to $K$. Right multiplication by it changes the bottom row to $(0,t)$, so the resulting invertible matrix in $gK$ is upper triangular. [F1, F2, F4, F7, step 1.1, step 1.2]

3.1 By steps 1.3 and 2.1, both off-diagonal entries and the difference of the diagonal entries are continuous functions on $G$. The scalar subgroup $Z$ is the intersection of their three zero preimages, which are closed by [F6] because $\{0\}$ is closed in $F$. Thus $Z$ is closed by [F11]. Write $q:G\to G/Z$ for the quotient projection. For open $U\subseteq G$, the preimage of $q(U)$ is $UZ=\bigcup_{z\in Z}Uz$. By step 2.1 and [F6], each $Uz$ is open because it is the preimage of $U$ under the inverse of the homeomorphism $R_z$. The union $q^{-1}(q(U))$ is open by [F11], and the quotient topology makes $q(U)$ open. Hence $q$ is an open map, and it is continuous by the quotient topology. Images and preimages of basic open rectangles under $q\times q$ are products of the corresponding images and preimages under $q$, so they are open. Every open set in either product is a union of such rectangles, and images and preimages preserve unions. By [F11] and [F6], $q\times q$ is therefore open and continuous. It is surjective, so if a subset has open preimage under $q\times q$, the subset itself is open as the image of that preimage. Write $i$ and $m$ for inversion and multiplication on $G$, and $\bar i$ and $\bar m$ for the corresponding operations on $G/Z$. For open $W\subseteq G/Z$, the quotient operations give $q^{-1}(\bar i^{-1}(W))=(q\circ i)^{-1}(W)$ and $(q\times q)^{-1}(\bar m^{-1}(W))=(q\circ m)^{-1}(W)$. The sets on the right are open by the composition rule in step 2.1 and [F6]. The quotient criteria give openness of $\bar i^{-1}(W)$ and $\bar m^{-1}(W)$, so [F6] makes the induced operations continuous. [F4, F5, F6, F11, step 1.3, step 2.1]

4.1 The description of scalar cosets in [F4] gives $q(g)=q(h)$ exactly when $g=zh$ for some $z\in Z$, equivalently $gh^{-1}\in Z$. By composition in step 2.1, the second projection followed by inversion is continuous. Together with the first projection it gives the continuous map $(u,v)\mapsto (u,v^{-1})$ by the tuple rule in step 2.1. Composing with multiplication gives continuity of $(u,v)\mapsto uv^{-1}$. For distinct classes $q(g)$ and $q(h)$, the point $(g,h)$ belongs to the open preimage of $G\setminus Z$ under this map. The product topology gives an open rectangle $U\times V$ around $(g,h)$ in that preimage. If $u\in U$ and $v\in V$, then $uv^{-1}\notin Z$, so $q(u)\ne q(v)$. Thus $q(U)$ and $q(V)$ are disjoint open neighborhoods, proving the Hausdorff property. The quotient product in [F4] makes $q$ a homomorphism, so its restriction to the subgroup $K$ in step 1.2 is a homomorphism. By [F9], its image $\bar K=q(K)$ is a subgroup of $G/Z$. It is open and compact by openness and continuity of $q$. [F4, F5, F6, F9, step 1.2, step 2.1, step 3.1]

5.1 If $b,b'\in B$ represent the same coset, then $b'\in b'K=bK$. Thus $b'=bk$ for some $k\in K$. By the entry formula in [F4], the product of two upper-triangular matrices has zero lower-left entry, and each of its diagonal entries is the product of the corresponding diagonal entries of the factors. The inverse formula of step 2.1 preserves a zero lower-left entry. Hence $k=b^{-1}b'$ and its inverse are upper triangular. As $k\in K$, both $k$ and $k^{-1}$ have entries in $O$. The diagonal entry rule applied to $kk^{-1}=I$ gives inverses in $O$ for the diagonal entries of $k$. Applied to $b'=bk$, the same rule gives the diagonal entries of $b'$ as those of $b$ multiplied by the corresponding units of $O$. Their valuations therefore agree. [F4, F7, step 1.1, step 2.1, step 2.2] ∎

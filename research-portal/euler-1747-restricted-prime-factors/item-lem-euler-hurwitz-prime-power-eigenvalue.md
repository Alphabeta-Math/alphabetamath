---
title: Prime-power Hecke eigenvalue in the counting normalization
status: draft
research_item: lem-euler-hurwitz-prime-power-eigenvalue
dependency_level: 8
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, Lemma 3.2, displayed local eigenvalue and triangular-coset
        calculation
---

PDF p. 3: ` Lemma 3.2, displayed local eigenvalue and triangular-coset calculation `

## Prerequisites

- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)
- [math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-linear-subspace](https://alphabetamath.cc/item/def-linear-subspace)
- [math:def-dimension](https://alphabetamath.cc/item/def-dimension)
- [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)
- [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)
- [math:cor-square-matrix-invertible-iff-determinant-is-a-unit](https://alphabetamath.cc/item/cor-square-matrix-invertible-iff-determinant-is-a-unit)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)
- [math:def-hilbert-space](https://alphabetamath.cc/item/def-hilbert-space)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)
- [def-author-d45da46285be-satake-transform](item-def-author-d45da46285be-satake-transform)
- [thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character)
- [def-determinant-index-spherical-hecke-correspondence](item-def-determinant-index-spherical-hecke-correspondence)
- [lem-degree-two-spherical-index-cosets](item-lem-degree-two-spherical-index-cosets)
- [thm-hurwitz-integral-splitting-at-odd-primes](item-thm-hurwitz-integral-splitting-at-odd-primes)
- [lem-euler-hurwitz-adelic-hecke-identification](item-lem-euler-hurwitz-adelic-hecke-identification)
- [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)
- [math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative)
- [lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)
- [math:cor-euclids-lemma-for-finite-products](https://alphabetamath.cc/item/cor-euclids-lemma-for-finite-products)
- [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:lem-topological-group-translations-and-inversion](https://alphabetamath.cc/item/lem-topological-group-translations-and-inversion)
- [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)
- [math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space)
- [math:def-topological-group](https://alphabetamath.cc/item/def-topological-group)


## Statement

Assume countable choice, meaning that each sequence of nonempty sets has a choice function. Let $\ell$ be a prime and $e$ a nonnegative integer. Put $F=\mathbb Q_\ell$, the completion of $\mathbb Q$ for the distance given by $|a-b|_\ell$, and $O=\mathbb Z_\ell$, the subring of elements of absolute value at most one. The absolute value on nonzero rationals is $\ell^{-v_\ell(a)}$, where $v_\ell(a)$ is the exponent of $\ell$ in the numerator minus the exponent in the denominator. On nonzero elements of $F$, the extended absolute value is $\ell^{-v_\ell(a)}$ with integer $v_\ell(a)$ and $v_\ell(\ell)=1$.

Write $\mathrm{GL}_2(F)$ and $H=\mathrm{GL}_2(O)$ for the groups of two-by-two matrices invertible over the indicated rings under row-by-column multiplication. Let $q:\mathrm{GL}_2(F)\to\mathrm{PGL}_2(F)$ send $A$ to its class $[A]$ modulo multiplication by nonzero scalar matrices, and put $K=q(H)$. Use the fixed determinant-valuation set
$$D_e=\{A\in M_2(O):\det A\ne0,\ v_\ell(\det A)=e\},$$
where $M_2(O)$ consists of the two-by-two matrices over $O$ and $\det\begin{pmatrix}a&b\\c&d\end{pmatrix}=ad-bc$. As $F$ is a field, the nonzero determinant of every $A\in D_e$ is a unit of $F$, so $A$ is invertible over $F$ by the determinant criterion. The projective determinant-index correspondence of index $\ell^e$ uses each coset $hK=\{hk:k\in K\}$ in $q(D_e)$ with weight one.

Let $V$ be the space of smooth vectors of a strongly continuous unitary representation $\pi$ of $\mathrm{GL}_2(F)$. Give each copy of $F$ the metric topology for $d(x,y)=|x-y|_\ell$. The matrix group has the subspace topology from the product topology on its four entries in $F^4$. A unitary representation is a group action by bijective complex-linear isometries on a complex Hilbert space, an inner-product space complete in its induced norm. Strong continuity means that the image of each vector varies continuously with the group element. Smooth vectors are those fixed by some open subgroup. Suppose $V$ is irreducible, meaning nonzero with no nonzero proper linear subspace carried to itself by every group element, and admissible, meaning finite-dimensional fixed spaces under compact open subgroups. Here compactness means each open cover admits a finite subcover. Assume the scalar matrices act trivially and the representation is unramified, meaning that $V^H=\{w\in V:\pi(h)w=w\text{ for all }h\in H\}$ is nonzero.

Let $u_\ell,v_\ell$ be its normalized Satake parameters. These are the unordered pair of nonzero complex numbers, with multiplicity, for which each spherical Hecke function $f$ acts on the fixed line $V^H$ by the scalar $S(f)(u_\ell,v_\ell)$. A spherical Hecke function vanishes outside a compact set and satisfies $f(hxh')=f(x)$ for $h,h'\in H$. Its action on $V^H$ is the finite sum of $f(x)\pi(x)$ over the cosets $xH$ in the support. The normalized transform $S$ sums the terms $f(x)\ell^{(s-r)/2}X^rY^s$, where $(r,s)$ are the valuations of the diagonal entries of an upper-triangular representative of $xH$. Its evaluation replaces $X^rY^s$ by $u_\ell^rv_\ell^s$. The spherical factor is the multiplier $\ell^{(s-r)/2}$.

For each $0\le r\le e$, the triangular cosets with diagonal $(\ell^r,\ell^{e-r})$ have multiplicity $\ell^r$ and spherical factor $\ell^{(e-2r)/2}$. Their product is $\ell^{e/2}$. On the fixed line the projective determinant-index correspondence therefore has eigenvalue, meaning the scalar by which it acts,
$$\lambda_{\ell,e}=\ell^{e/2}\sum_{r=0}^e u_\ell^r v_\ell^{e-r}.$$

For the Hurwitz setting take $p$ prime with remainder $3$ upon division by $4$, and $\ell$ odd and distinct from $p$. The Hurwitz order $\mathcal H$ consists of the Hamilton quaternions whose four coordinates in the basis $1,i,j,k$ are either all integers or all integers plus $\tfrac12$. The products satisfy $i^2=j^2=-1$ and $ij=k=-ji$. Let $\rho_p$ be projective reduction, obtained from integral matrix coordinates by reducing the entries modulo $p$ and taking the class modulo nonzero scalars. It is defined on elements whose reduced norm, the sum of the four coordinate squares, is prime to $p$. Write $G_p=\mathrm{PGL}_2(\mathbb F_p)$, where $\mathbb F_p$ is the field of residues modulo $p$, and $Y_p$ for the set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$ with $g\in G_p$, where $\Gamma_p=\rho_p(\mathcal H^\times)$ and $\mathcal H^\times$ consists of the elements with a two-sided inverse in $\mathcal H$. Let $Q_{\ell^e}$ be the set of elements of $\mathcal H$ of reduced norm $\ell^e$. For a complex function $f$ on $Y_p$, define the Hurwitz operator by

$$(T_{\ell^e}f)(\Gamma_p g)=\frac{1}{24}\sum_{\alpha\in Q_{\ell^e}}f(\Gamma_p\rho_p(\alpha)g).$$

Use integral splittings at $p$ and $\ell$, meaning algebra isomorphisms carrying the corresponding local spans of $\mathcal H$ onto the integral matrix rings. The local spans are obtained by allowing coefficients in the local field for the Hamilton algebra and in its ring of integers for the order. Use the splitting at $p$ for $\rho_p$ and the splitting at $\ell$ for the local correspondence. On a local Hecke eigensystem in this quotient with the action above, the eigenvalue of $T_{\ell^e}$ is $\lambda_{\ell,e}$. Such an eigensystem is a one-dimensional subspace on which each local correspondence acts by the same scalar as on the projective fixed line.

## Facts & Assumptions

[F1] Countable choice has the meaning in the Statement, and a prime is an integer greater than one with only $1$ and itself as positive divisors. The normalized valuation adds under multiplication of nonzero field elements and vanishes on the units of $O$. The groups $\mathrm{GL}_2(F)$ and $\mathrm{PGL}_2(F)$ use matrix multiplication and its quotient by scalars. Give $\mathrm{GL}_2(F)$ the entry topology from the Statement and $\mathrm{PGL}_2(F)$ the corresponding quotient topology. A subset of $\mathrm{PGL}_2(F)$ is open exactly when its inverse image under $q$ is open. The subgroups $H$ and $K$ are compact open in their respective Hausdorff topological groups. Hausdorff means that distinct points have disjoint open neighborhoods. In a topological group, multiplication is continuous for the product topology on the two inputs, and inversion is continuous. The two diagonal valuations of a triangular representative depend only on its coset $xH$. [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology) [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology) [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top) [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) [math:def-prime](https://alphabetamath.cc/item/def-prime) [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation) [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group) [lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets) [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology) [math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space) [math:def-topological-group](https://alphabetamath.cc/item/def-topological-group)

[F2] Matrix multiplication preserves integral entries. The two-by-two determinant is $ad-bc$ and is multiplicative, so $\det h$ is a unit of $O$ for $h\in H$ by multiplying with $\det(h^{-1})$. Over a commutative ring a two-by-two matrix is invertible exactly when its determinant is a unit. The cosets of a subgroup $J$ for multiplication on the right by $J$ have the form $xJ=\{xj:j\in J\}$. [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose) [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix) [math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative) [math:cor-square-matrix-invertible-iff-determinant-is-a-unit](https://alphabetamath.cc/item/cor-square-matrix-invertible-iff-determinant-is-a-unit) [math:def-coset](https://alphabetamath.cc/item/def-coset)

[F3] The integral coset classification gives exactly one representative $A_{r,b}=\begin{pmatrix}\ell^r&b\\0&\ell^{e-r}\end{pmatrix}$ per coset of $H$ in $D_e$, with $0\le r\le e$ and $b$ ranging over the integer residues $0,\ldots,\ell^r-1$ embedded in $O$. The map $AH\mapsto[A]K$ is a bijection onto the cosets of $K$ in $q(D_e)$. [lem-degree-two-spherical-index-cosets](item-lem-degree-two-spherical-index-cosets)

[F4] Under countable choice the normalized spherical character theorem applies to the smooth part of the stated strongly continuous unitary representation. The theorem requires that $V$ have no nonzero proper invariant linear subspaces, that its fixed spaces under compact open subgroups be finite dimensional, and that $V^H\ne0$. The theorem gives $\dim_{\mathbb C} V^H=1$ and identifies the Hecke scalar with evaluation of the normalized transform. The action and transform both sum one term per contributing coset, and the transform uses the factor $\ell^{(s-r)/2}$ for diagonal valuations $(r,s)$. Laurent polynomial addition is coefficientwise on finitely supported complex coefficient functions. The sum is supported in the union of the two finite supports. Complex addition is associative and commutative with identity zero, so these laws hold coefficientwise and the zero polynomial is the additive identity. Thus the Laurent polynomials form a commutative monoid under addition, as do the complex numbers used after evaluation. A finite sum in a commutative monoid is independent of enumeration. For a finite partition, list its parts and apply [F12] to the nonempty sets of enumerations of the individual parts. Concatenate the chosen enumerations. Associativity gives the sum of the parts. [math:def-linear-subspace](https://alphabetamath.cc/item/def-linear-subspace) [math:def-dimension](https://alphabetamath.cc/item/def-dimension) [thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character) [def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra) [def-author-d45da46285be-satake-transform](item-def-author-d45da46285be-satake-transform) [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field) [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)

[F5] An odd prime admits the indicated integral splitting. For positive odd $m$ prime to $p$, the Hurwitz correspondence identification expresses the shell operator $T_m$ as the product of the local determinant-index coset sums at the primes dividing $m$. The local projective correspondence acts by one summand per coset of $K$ contained in its index support. When $m=1$, the product of local operators is empty and is the identity. [thm-hurwitz-integral-splitting-at-odd-primes](item-thm-hurwitz-integral-splitting-at-odd-primes) [lem-euler-hurwitz-adelic-hecke-identification](item-lem-euler-hurwitz-adelic-hecke-identification) [def-determinant-index-spherical-hecke-correspondence](item-def-determinant-index-spherical-hecke-correspondence) [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)

[F6] A continuous map takes a compact subset of its domain to a compact subset of its codomain. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps) A subset is compact when every open cover in its subspace topology has a finite subcover. Equivalently, every cover of the subset by open sets of the ambient space has a finite subfamily covering the subset. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[F7] If a prime divides a finite product of integers, then it divides at least one of the factors. [math:cor-euclids-lemma-for-finite-products](https://alphabetamath.cc/item/cor-euclids-lemma-for-finite-products)

[F8] For the positive real base $\ell$, the rational-power definition agrees with integer powers at integer exponents, and $\ell^a\ell^b=\ell^{a+b}$ for rational $a,b$. [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power) [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)

[F9] Read the integer $\ell$ in the reals by first embedding the integers in the rationals via $n\mapsto n/1$ and then embedding the rationals as constant real classes. These maps preserve addition, multiplication, one and order, so the real base $\ell$ exceeds one and the count $\ell^r$ maps to the $r$th real power of that base. The real-to-complex field embedding preserves finite addition and products. [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

[F10] In a topological group, left multiplication by a fixed element $A$ defines a continuous map $L_A(x)=Ax$ from the group to itself. [math:lem-topological-group-translations-and-inversion](https://alphabetamath.cc/item/lem-topological-group-translations-and-inversion)

[F11] For integers $m$ and $b$ with $b>0$, division with remainder writes $m=kb+t$ with integers $k,t$ and $0\le t<b$. The remainder $t$ is zero exactly when $b$ divides $m$. [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

[F12] For a list of nonempty sets $E_i$ indexed by $0\le i<n$ for a natural number $n$, there is a choice function $c$ on the family of values of the list. Then $c(E_i)\in E_i$ for each index, including when the same set occurs more than once. [math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice)

[F13] Each nonnegative integer has a unique natural-number preimage under the canonical embedding. In a multiplicative monoid, natural powers start at the identity and multiply by one more copy of the base at each successor. For the index use $\mathbb Z$ under multiplication, with the natural preimage as exponent. The integers form an ordered commutative ring, so a product of positive integers is positive. [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:def-group-power](https://alphabetamath.cc/item/def-group-power) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

## Proof

**Given:** The prime $\ell$, exponent $e$, countable choice and the representation in the Statement, and the stated conditions on $p$ in the Hurwitz application.

**Goal:** Compute the scalar of the index-$\ell^e$ correspondence and identify it in the Hurwitz counting normalization.

1.1 Every $A\in D_e$ lies in $\mathrm{GL}_2(F)$ by [F2], since $\det A$ is nonzero and hence invertible in the field $F$. Set $f_e=\mathbf 1_{D_e}$, the function equal to one on $D_e$ and zero elsewhere in $\mathrm{GL}_2(F)$. Multiplication on either side by an element of $H$ preserves integral entries and preserves determinant valuation because the determinant of that element has valuation zero. Multiplication by its inverse has the same properties, so $f_e$ is invariant on both sides by $H$. The coset classification expresses $D_e$ as a finite union of translates of the compact open subgroup $H$. With the entry topology specified in the Statement, $\mathrm{GL}_2(F)$ is a topological group by [F1]. Left multiplication by each representative $A$ is therefore continuous on $\mathrm{GL}_2(F)$ by [F10]. Its image $AH$ of the compact subset $H$ is compact by [F6]. Index the translates by the finite list in [F3]. Given a cover of $D_e$ by open sets in the matrix group, for each translate the set of finite lists of members of that cover covering the translate is nonempty by [F6]. Apply [F12] to select one such list for each translate. Concatenating the lists gives a finite subfamily covering $D_e$, so $D_e$ is compact by [F6]. Thus $f_e$ vanishes outside a compact set and is a spherical Hecke function. [F1, F2, F3, F4, F6, F10, F12]

2.1 The matrix $A_{r,b}$ has diagonal valuations $r,e-r$, independent of $b$. For a fixed $r$ there are $\ell^r$ choices of $b$. Each coset contributes $\ell^{((e-r)-r)/2}X^rY^{e-r}$ to $S(f_e)$. Interpret the multiplicity and the weight in the same real embedding of [F9]. The real base is positive, so [F8] gives the combined coefficient $\ell^r\ell^{(e-2r)/2}=\ell^{r+(e-2r)/2}=\ell^{e/2}$. Regroup the finite sum of Laurent polynomials by the common exponent $r$ using the partition argument of [F4]. This gives $S(f_e)=\ell^{e/2}\sum_{r=0}^e X^rY^{e-r}$. [F1, F3, F4, F8, F9, F12, step 1.1, algebra]

3.1 Evaluate this transform at $(u_\ell,v_\ell)$ by the normalized spherical character theorem. This gives $\lambda_{\ell,e}$ as the scalar of $f_e$ on $V^H$. The map $r\mapsto e-r$ is its own inverse on $\{0,\ldots,e\}$, so interchanging $u_\ell$ and $v_\ell$ just reindexes the sum by this bijection. By [F4] the sum is independent of the ordering of the parameters. [F4, step 2.1]

4.1 The action descends by $\bar\pi([A])=\pi(A)$ since scalar matrices act trivially. A vector is fixed by $K$ for $\bar\pi$ exactly when it is fixed by $H$ for $\pi$, since $q(H)=K$. The bijection $AH\mapsto[A]K$ carries every summand $\pi(A)w$ of the action of $f_e$ on a fixed vector $w$ to the identical summand $\bar\pi([A])w$ with the same weight. It includes all cosets in the projective image of $D_e$, including those represented by matrices in $D_e$ with every entry divisible by $\ell$. This proves the projective scalar formula. [given, F1, F3, F4, F5, step 3.1]

5.1 In the Hurwitz application, both primes exceed two. By [F11], $p$ cannot equal $2$ because its remainder modulo $4$ is $3$, and $\ell$ cannot equal $2$ because it is odd. Thus the integral splitting theorem in [F5] applies at both primes. For $e>0$, the power recursion in [F13] writes $m=\ell^e$ as the product of $e$ copies of $\ell$. Starting at $1>0$, each multiplication by $\ell>1$ preserves positivity by [F13]. The last factor gives $\ell\mid m$. Any prime divisor $d$ of $m$ divides one of those copies by [F7], so $d=\ell$ by primality of $\ell$. Since $2$ is prime and $\ell$ is odd, $2$ does not divide $m$. Apply [F11] with divisor $2$. The integer remainder is $0$ or $1$, and $2\nmid m$ rules out zero. Thus $m=2k+1$ for an integer $k$, as required in [F5]. Since $p$ is prime and distinct from $\ell$, $p$ does not divide $m$. The product law from [F1] gives $v_\ell(m)=e\,v_\ell(\ell)=e$, using the normalization $v_\ell(\ell)=1$. The identification in [F5] then carries the single local determinant-index coset sum, at $\ell$ with $v_\ell(m)=e$, to $T_{\ell^e}$. On an eigensystem with the stated local action its scalar is therefore $\lambda_{\ell,e}$ by step 4.1. For $e=0$, the Hurwitz operator is the identity by the empty product in [F5], and the formula has just the term $1$ by the zero-power rules in [F8] and [F13]. This proves the asserted eigenvalue in the Hurwitz counting normalization for every $e\ge0$. [given, F1, F5, F7, F8, F11, F13, step 4.1] ∎

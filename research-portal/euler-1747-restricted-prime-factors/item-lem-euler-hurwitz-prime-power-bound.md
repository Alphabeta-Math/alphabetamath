---
title: Absolute bound for an unramified prime-power eigenvalue
status: draft
research_item: lem-euler-hurwitz-prime-power-bound
dependency_level: 9
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, Lemma 3.2, last paragraph, local bound before multiplication
      reading_limits: Checked the formula and the local bound on PDF page 3 for attribution.
    - title: Denis Trotabas, Modular Forms and Automorphic Representations
      url: https://math.stanford.edu/~conrad/conversesem/refs/trotabas.pdf#page=25
      locator: §5.2, Definition 5.2, PDF p. 17, §8.1, conditions (1)–(4) and the
        Hilbert norm, PDF pp. 25–26, and §8.2, PDF pp. 26–27
      statement: Definition 5.2 attaches a unitary representation to a classical cusp
        form by right translation on the closed span of the right translates of
        its adelic lift. Section 8.1 defines a Hilbert space of classes modulo
        equality almost everywhere on H\G. A representative is Borel on H\G, its
        modulus is Borel on ZH\G, and for each central element covariance holds
        almost everywhere on H\G. The squared norm is the finite integral of
        squared modulus on ZH\G. In the adelic case the two quotients are
        GL₂(Q)\GL₂(A) and Z(A)GL₂(Q)\GL₂(A). Section 8.2 describes vanishing of
        the upper unitriangular average over Q\A and gives closure of bounded
        continuous functions satisfying the listed conditions as one
        construction.
      hypotheses: In Definition 5.2 the form is cuspidal, of weight k, level N and
        nebentypus χ. Section 8.1 uses a locally compact unimodular group G, a
        closed unimodular subgroup H and a unitary character of the center Z or
        of a closed subgroup Z of the center. Section 8.2 uses GL₂ over the
        rational adeles and a unitary character of the rational idele class
        group.
      reading_limits: Checked the right-translate span in Definition 5.2, the
        representative and norm conditions in §8.1, and the constant-term and
        bounded continuous closure conventions in §8.2. The smooth closure used
        here is specified by the Satake unitarity theorem.
    - title: Andrew Corbett and Abhishek Saha, On the order of vanishing of newforms
        at cusps
      url: https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf#page=16
      locator: §3.1, pp. 16–17, local embedding and setup for (20)–(22), §3.2.1, p.
        17, Whittaker integral before (24), and the compact quotient description
        in the proof of Lemma 3.1, p. 18
      statement: In the rational adelic setting the irreducible unitary cuspidal
        representation is a restricted tensor product of the local factors,
        using the single-place inclusion with identity elsewhere. The additive
        quotient Q\A is compact and the upper unitriangular integral uses its
        translation-invariant probability measure.
      hypotheses: The group is GL₂ over the rational adeles and the unitary central
        character is trivial on the positive real scalars. The holomorphic
        discrete-series setting of §3 uses integral lowest weight at least two.
      reading_limits: Read the local inclusions, factorization, real type, and
        additive integral convention. Only the realization and normalization are
        used here.
---

PDF p. 3: ` Lemma 3.2, last paragraph, local bound before multiplication `

## Prerequisites

- [math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)
- [math:lem-unit-circle-is-a-compact-metrizable-topological-group](https://alphabetamath.cc/item/lem-unit-circle-is-a-compact-metrizable-topological-group)
- [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)
- [math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [thm-euler-weight-two-satake-unitarity](item-thm-euler-weight-two-satake-unitarity)
- [def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles)
- [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)
- [math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)
- [math:def-hilbert-space](https://alphabetamath.cc/item/def-hilbert-space)
- [thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character)
- [def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)
- [def-author-d45da46285be-satake-transform](item-def-author-d45da46285be-satake-transform)
- [def-determinant-index-spherical-hecke-correspondence](item-def-determinant-index-spherical-hecke-correspondence)
- [lem-euler-hurwitz-prime-power-eigenvalue](item-lem-euler-hurwitz-prime-power-eigenvalue)
- [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)
- [math:def-eigenvalue-eigenvector-eigenspace-and-spectrum](https://alphabetamath.cc/item/def-eigenvalue-eigenvector-eigenspace-and-spectrum)
- [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:def-canonical-natural](https://alphabetamath.cc/item/def-canonical-natural)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [math:lem-complex-conjugation-and-modulus-laws](https://alphabetamath.cc/item/lem-complex-conjugation-and-modulus-laws)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots)
- [def-author-34e2e6a0519f-split-adelic-matrix-groups](item-def-author-34e2e6a0519f-split-adelic-matrix-groups)
- [lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)
- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)
- [thm-hurwitz-integral-splitting-at-odd-primes](item-thm-hurwitz-integral-splitting-at-odd-primes)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)
- [math:def-radon-measure-on-an-lch-space](https://alphabetamath.cc/item/def-radon-measure-on-an-lch-space)
- [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)
- [math:def-locally-compact-space](https://alphabetamath.cc/item/def-locally-compact-space)
- [math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:cor-euclids-lemma-for-finite-products](https://alphabetamath.cc/item/cor-euclids-lemma-for-finite-products)
- [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:def-metric-interior-closure-boundary](https://alphabetamath.cc/item/def-metric-interior-closure-boundary)
- [math:def-measure-null-set-and-almost-everywhere](https://alphabetamath.cc/item/def-measure-null-set-and-almost-everywhere)
- [math:def-nonnegative-lebesgue-integral](https://alphabetamath.cc/item/def-nonnegative-lebesgue-integral)
- [math:def-integrable-real-and-complex-functions-and-their-integrals](https://alphabetamath.cc/item/def-integrable-real-and-complex-functions-and-their-integrals)
- [math:def-inner-product-space](https://alphabetamath.cc/item/def-inner-product-space)
- [math:def-complex-exponential](https://alphabetamath.cc/item/def-complex-exponential)
- [math:def-sine-and-cosine-by-power-series](https://alphabetamath.cc/item/def-sine-and-cosine-by-power-series)
- [` Denis Trotabas, Modular Forms and Automorphic Representations · §5.2, Definition 5.2, PDF p. 17, §8.1, conditions (1)–(4) and the Hilbert norm, PDF pp. 25–26, and §8.2, PDF pp. 26–27 `](https://math.stanford.edu/~conrad/conversesem/refs/trotabas.pdf#page=25)
- [` Andrew Corbett and Abhishek Saha, On the order of vanishing of newforms at cusps · §3.1, pp. 16–17, local embedding and setup for (20)–(22), §3.2.1, p. 17, Whittaker integral before (24), and the compact quotient description in the proof of Lemma 3.1, p. 18 `](https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf#page=16)


## Statement

Assume countable choice, meaning that each sequence of nonempty sets has a choice function. Let $\ell$ be a prime, an integer greater than one with only positive divisors $1$ and $\ell$, and let $e$ be a nonnegative integer. Identify each nonnegative integer with its natural-number preimage under the canonical embedding of the naturals into the integers. When $\ell$ is used as a real base, first map the integer $\ell$ to the rational $\ell/1$ and then take its real image as a constant Cauchy class. This is the canonical real numeral of the natural preimage of $\ell$.

Take an irreducible unitary cuspidal automorphic representation $\Pi$ with holomorphic discrete-series weight two as in the Satake unitarity theorem. Write $\mathbb A=\mathbb R\times\mathbb A_f$, with $\mathbb A_f$ the tuples of $q$-adic numbers integral at all but finitely many primes $q$. Give $G=\mathrm{GL}_2(\mathbb A)$, the invertible two-by-two matrices over $\mathbb A$, the restricted-product topology with respect to $\mathrm{GL}_2(\mathbb Z_q)$ at the finite places. Each local matrix group has the subspace topology inherited from the product topology on its four entries. The basic open boxes have arbitrary local open factors at the real place and finitely many finite places, and full integral matrix groups at the other places.

The unitary action is by complex-linear isometries of a Hilbert space, meaning a complete inner-product space. Strong continuity means that each vector varies continuously under the group action. Irreducibility excludes proper nonzero closed invariant subspaces. Let $Z=\{aI:a\in\mathbb A^\times\}$ be the scalar subgroup, where $\mathbb A^\times$ is the group of invertible adeles. Rational scalars and matrices are embedded diagonally. Give $\mathbb A^\times=\mathbb R^\times\times\mathbb A_f^\times$ the restricted-product topology using the local unit groups $\mathbb Z_q^\times$ at the finite places and the usual subspace topology on $\mathbb R^\times\subset\mathbb R$. Give $\mathbb A^\times/\mathbb Q^\times$ the quotient topology under the projection modulo the diagonal nonzero rationals. Let $\omega$ be the unitary central character, a continuous homomorphism from $\mathbb A^\times/\mathbb Q^\times$ to the complex numbers of modulus one. The smooth representatives are left rational-matrix-invariant and satisfy $\phi(ag)=\omega(a)\phi(g)$ for every $g\in G$ and scalar $a\in\mathbb A^\times$, where $\omega(a)$ denotes evaluation on the idele class of $a$. Thus $|\phi|$ descends to a continuous function on the orbit space $X=(\mathrm{GL}_2(\mathbb Q)Z)\backslash G$ with the quotient topology. In the given realization each point of $X$ has a compact neighborhood, and distinct points have disjoint open neighborhoods. Square integrability uses a nonzero Radon measure on this quotient invariant under right translation by $G$. Vectors in the central-character Hilbert space are classes of Borel-measurable representatives on $\mathrm{GL}_2(\mathbb Q)\backslash G$ with its quotient topology, modulo equality almost everywhere for the quotient Haar measure. The modulus of each representative is the pullback of a Borel-measurable function on $X$. Borel measurability means that preimages of open sets belong to the sigma-algebra generated by the open sets of the domain. For each scalar the central covariance identity holds almost everywhere on the rational quotient. The squared norm is the integral of the square of the descended modulus over $X$ for the stated invariant measure, and this integral must be finite.

The cuspidal Hilbert space is the closure in this norm of the classes of smooth square-integrable functions $\phi$ satisfying the pointwise rational invariance and central covariance above and $\int_{\mathbb A/\mathbb Q}\phi(n(x)g)\,dx=0$ at every $g\in G$. Here $n(x)=\begin{pmatrix}1&x\\0&1\end{pmatrix}$ and the integral uses the translation-invariant probability measure on the compact additive quotient by the diagonally embedded rationals, with its quotient topology. The integrand descends to that quotient since $n(x+b)=n(b)n(x)$ for $b\in\mathbb Q$ and $\phi$ is left rational-matrix-invariant. Smooth functions are differentiable to all orders at the real place and are invariant under right translation by some compact open subgroup of the finite adelic group. The action of $\Pi$ is by right translation on a closed invariant subspace of this cuspidal Hilbert space.

The real factor of $\Pi$ is the full $\mathrm{GL}_2(\mathbb R)$ discrete series of weight two. This is the unitary type of the unique irreducible subrepresentation of normalized upper-triangular induction from the two diagonal characters $|\cdot|^{1/2}$ and $|\cdot|^{-1/2}$. In the induced model the left transformation by an upper-triangular matrix with diagonal $(a,d)$ multiplies the function by $|a|^{1/2}|d|^{-1/2}|a/d|^{1/2}$. On the positive-determinant group $G_\infty^+=\mathrm{GL}_2(\mathbb R)^+$, the holomorphic constituent has rotation weights $2,4,6,\ldots$ and square-integrable matrix coefficients modulo the real center. For its action $\rho^+$ and Hilbert space vectors $v,w$, a matrix coefficient at $g$ is $\langle\rho^+(g)v,w\rangle$. The group $Z_\infty=\{aI:a\in\mathbb R^\times\}$ is the real center and acts by a unitary scalar character, so the squared modulus of each coefficient descends to the group $G_\infty^+/Z_\infty$ with the quotient topology. Square integrability modulo the real center means that each such squared modulus has finite integral for a nonzero right-invariant Radon measure on $G_\infty^+/Z_\infty$. Weight $j$ acts by $\exp(ij\theta)$ on the corresponding weight space under the rotation with rows $(\cos\theta,\sin\theta)$ and $(-\sin\theta,\cos\theta)$. Assume positive real scalar matrices at the real place, with identities at the finite places, act trivially.

Let $\pi_\ell$ be the $\ell$-component of the restricted tensor-product decomposition of this same $\Pi$. Its group $\mathrm{GL}_2(F)$ is embedded by placing a matrix in the $\ell$-coordinate and identities at every other place. Here $F=\mathbb Q_\ell$ is the $\ell$-adic completion of $\mathbb Q$ and $O=\mathbb Z_\ell$ is its ring of elements of $\ell$-adic absolute value at most one. Put $H=\mathrm{GL}_2(O)$, the matrices invertible over $O$. Assume $\pi_\ell$ is strongly continuous and unitary, its smooth vectors are irreducible and admissible, and it is unramified. The topology on $\mathrm{GL}_2(F)$ is the subspace topology from the product topology on $F^4$. In this topology $H$ is compact and open in $\mathrm{GL}_2(F)$. The smooth vectors are those fixed by some open subgroup. Irreducibility here excludes nonzero proper invariant linear subspaces of the smooth space, admissibility means its fixed subspace under every compact open subgroup is finite dimensional, and unramified means $H$ fixes a nonzero vector in the local Hilbert space. For the projective correspondence assume every scalar matrix in $\mathrm{GL}_2(F)$ acts as the identity.

The normalized Satake parameters $u_\ell,v_\ell$ are the unordered pair of nonzero complex numbers, with multiplicity, at which evaluation of the normalized Satake transform gives the spherical Hecke scalars on the $H$-fixed line. A spherical Hecke weight is a compactly supported function invariant under multiplication on either side by $H$. For a weight $a$, its transform sums one term per coset $xH=\{xh:h\in H\}$ with $a(x)\ne0$. The term is $a(x)\ell^{(s-r)/2}X^rY^s$, where $(r,s)$ are the diagonal valuations of an upper-triangular representative. Such representatives exist and their diagonal valuations depend only on the coset. A nonzero local entry of valuation $r$ has $\ell$-adic absolute value $\ell^{-r}$. Evaluation replaces $X^rY^s$ by $u_\ell^rv_\ell^s$, using integer powers of nonzero complex numbers.

Use the projective determinant-index correspondence of index $\ell^e$. This acts by summing the translations $\pi_\ell(A)$ with weight one per coset of the image of $H$ in the set of projective classes admitting an integral matrix representative $A$ with nonzero determinant of valuation $e$. For rows $(a,b)$ and $(c,d)$ the determinant is $ad-bc$. The projective classes identify matrices that differ by a nonzero scalar multiple. The scalar $\lambda_{\ell,e}$ of this action on the fixed line is its eigenvalue, so a nonzero vector $w$ in the line is sent to $\lambda_{\ell,e}w$. Then
$$|\lambda_{\ell,e}|\le (e+1)\ell^{e/2}.$$
Here $|a+bi|=\sqrt{a^2+b^2}$ is complex modulus for real $a,b$. The real factor $\ell^{e/2}$ is the $e$th power of the positive square root of $\ell$, and the integer count $e+1$ is interpreted as the real sum of $e+1$ copies of one.

For the Hurwitz application take a prime $p=4k+3$ for an integer $k$ and an odd $\ell\ne p$. Both primes exceed two, as checked in the proof. The index $\ell^e$ is positive and odd, and $p\nmid\ell^e$, as checked in the proof. In the rational Hamilton quaternion algebra $B$, the basis $1,i,j,k$ satisfies $i^2=j^2=-1$ and $ij=k=-ji$. The Hurwitz order $\mathcal H$ is the subring whose four coordinates are all integers or all integers plus $\tfrac12$, with multiplication inherited from $B$. Write $Q_{\ell^e}$ for its norm shell, the elements with sum of four coordinate squares equal to $\ell^e$. For $q=p,\ell$, fix an integral splitting $\Phi_q$ of the Hamilton algebra over $\mathbb Q_q$. It is an algebra isomorphism onto the two-by-two matrices over $\mathbb Q_q$ taking the $\mathbb Z_q$-span of $\mathcal H$ onto the two-by-two matrices over $\mathbb Z_q$.

Use $\Phi_p$ in the projective reduction $\rho_p$, which reduces the integral matrix entries modulo $p$ and takes the class modulo nonzero scalars. The reduction is defined on Hurwitz elements whose reduced norm is prime to $p$, which includes the whole shell $Q_{\ell^e}$. Use $\Phi_\ell$ for the local determinant-index correspondence, so the projective image of the completed Hurwitz unit group is the image of $H$. Let $\Gamma_p=\rho_p(\mathcal H^\times)$, where $\mathcal H^\times$ consists of the elements with two-sided inverses in $\mathcal H$. For a complex function $f$ on the right cosets $\Gamma_pg=\{\gamma g:\gamma\in\Gamma_p\}$ in $\mathrm{PGL}_2(\mathbb F_p)$, the Hurwitz operator in the counting normalization is
$$(T_{\ell^e}f)(\Gamma_p g)=\frac{1}{24}\sum_{\alpha\in Q_{\ell^e}} f(\Gamma_p\rho_p(\alpha)g).$$
Here $\mathbb F_p$ is the field of integer residues modulo $p$. Suppose a line in this finite function space is an eigenline for $T_{\ell^e}$. Assume that with these splittings its eigenvalue equals $\lambda_{\ell,e}$, the scalar of the index-$\ell^e$ correspondence on the projective fixed line of $\pi_\ell$, with one term per coset. On such a line the eigenvalue of $T_{\ell^e}$ satisfies the same bound.

## Statement references

[math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)

[math:lem-unit-circle-is-a-compact-metrizable-topological-group](https://alphabetamath.cc/item/lem-unit-circle-is-a-compact-metrizable-topological-group)

[math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)

[math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)

[def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles)

[math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)

[math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[math:def-metric-interior-closure-boundary](https://alphabetamath.cc/item/def-metric-interior-closure-boundary)

[math:def-measure-null-set-and-almost-everywhere](https://alphabetamath.cc/item/def-measure-null-set-and-almost-everywhere)

[math:def-nonnegative-lebesgue-integral](https://alphabetamath.cc/item/def-nonnegative-lebesgue-integral)

[math:def-integrable-real-and-complex-functions-and-their-integrals](https://alphabetamath.cc/item/def-integrable-real-and-complex-functions-and-their-integrals)

[math:def-inner-product-space](https://alphabetamath.cc/item/def-inner-product-space)

[math:def-complex-exponential](https://alphabetamath.cc/item/def-complex-exponential)

[math:def-sine-and-cosine-by-power-series](https://alphabetamath.cc/item/def-sine-and-cosine-by-power-series)

[math:def-locally-compact-space](https://alphabetamath.cc/item/def-locally-compact-space)

[math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[def-author-34e2e6a0519f-split-adelic-matrix-groups](item-def-author-34e2e6a0519f-split-adelic-matrix-groups)

[lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)

[def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)

[def-euler-hurwitz-order](item-def-euler-hurwitz-order)

[def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)

[thm-hurwitz-integral-splitting-at-odd-primes](item-thm-hurwitz-integral-splitting-at-odd-primes)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra)

## Facts & Assumptions

[F1] Countable choice provides a choice function for every sequence of nonempty sets. In the central-character class model, the representatives are Borel on the rational quotient and their descended moduli are Borel on the scalar quotient. The weight-two Satake unitarity theorem, for the stated global representation and an unramified local factor, using the locally compact Hausdorff orbit space, invariant Radon measure, smooth cuspidal closure in the Hilbert space of square-integrable classes and full real discrete-series type specified in the Statement, gives $|u_\ell|=|v_\ell|=1$ for the normalized pair, including on pullback from the projective group. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) [thm-euler-weight-two-satake-unitarity](item-thm-euler-weight-two-satake-unitarity) [thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character) [math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra)

[F2] With countable choice, $H$ is compact and open in $\mathrm{GL}_2(F)$. Each coset $xH$ admits an upper-triangular representative with well-defined diagonal valuations. For the smooth part of a strongly continuous unitary local representation, irreducibility, admissibility and a nonzero smooth $H$-fixed subspace imply that this subspace is one dimensional. With these hypotheses and trivial scalar action, the determinant-index eigenvalue formula in the weight-one coset normalization is $\lambda_{\ell,e}=\ell^{e/2}\sum_{r=0}^e u_\ell^r v_\ell^{e-r}$. At $e=0$ the projective correspondence acts as the identity on the fixed line. Here $\mathrm{GL}_2(F)$ has the subspace topology from the product topology on $F^4$. [lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets) [thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character) [lem-euler-hurwitz-prime-power-eigenvalue](item-lem-euler-hurwitz-prime-power-eigenvalue) [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology) [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[F3] The complex numbers form a field containing the reals. For any complex $z,w$ the modulus satisfies $|zw|=|z||w|$ and $|z+w|\le |z|+|w|$. Nonnegative powers are given by $z^0=1$ and $z^{n+1}=z^nz$. The real numbers form an ordered field, so addition preserves an inequality and multiplication by a positive real preserves it. For a positive real base $\ell$ the rational power $\ell^{e/2}=(\sqrt{\ell})^e$ is positive. The real field is least-upper-bound complete, so each nonnegative real has a unique nonnegative square root. [math:cor-cauchy-reals-lub-complete](https://alphabetamath.cc/item/cor-cauchy-reals-lub-complete) [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field) [math:thm-of-square-roots](https://alphabetamath.cc/item/thm-of-square-roots) [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus) [math:lem-complex-conjugation-and-modulus-laws](https://alphabetamath.cc/item/lem-complex-conjugation-and-modulus-laws) [math:def-group-power](https://alphabetamath.cc/item/def-group-power) [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field) [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)

[F4] The natural-to-integer embedding preserves addition and order and has image the nonnegative integers. A positive integer has a nonzero natural preimage. Since $0$ is a predecessor of that preimage, the integer is at least $1$. Thus if $0\le r\le e$ then the integer $e-r$ has a natural-number preimage, as does $r$. The finite initial segment of naturals $r<n$ has $n$ elements. The indices $r<n+1$ consist of the indices $r<n$ and the single new index $n$. A finite sum in increasing index order starts with the empty sum $0$ and appends one summand at each successor, by the finite product recursion written additively. The map $n\mapsto n/1$ from the integers into the rationals and the constant-class map from the rationals into the reals preserve addition, order, zero and one. The resulting real images of nonnegative integers obey the canonical numeral recursion since the maps preserve $0$, $1$ and addition. Induction proves a property for all naturals from its value at zero and its preservation by the successor operation. [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment) [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership) [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid) [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:def-canonical-natural](https://alphabetamath.cc/item/def-canonical-natural) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[F5] A prime exceeds one. The integers form an ordered commutative ring. In particular, a product of positive integers is positive and multiplication distributes over addition. If a prime divides a finite product of integers, it divides one of the factors. At exponent zero the product is $1$, which has no prime divisor. The map $\rho_p$ is defined on Hurwitz elements of reduced norm prime to $p$. The Hurwitz counting operator is defined at every positive odd index prime to $p$. The Hurwitz counting operator of index $1$ is the identity by the empty product of local correspondences. The integral splitting theorem applies at each prime $q>2$. [math:def-prime](https://alphabetamath.cc/item/def-prime) [thm-hurwitz-integral-splitting-at-odd-primes](item-thm-hurwitz-integral-splitting-at-odd-primes) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:cor-euclids-lemma-for-finite-products](https://alphabetamath.cc/item/cor-euclids-lemma-for-finite-products) [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator) [lem-euler-hurwitz-prime-power-eigenvalue](item-lem-euler-hurwitz-prime-power-eigenvalue)

[F6] The idele class group $\mathbb A^\times/\mathbb Q^\times$ consists of the cosets of the diagonal nonzero rationals. The diagonal subgroup is normal because the ideles multiply coordinatewise in commutative fields. The quotient operation is $[a][b]=[ab]$. The unitary character is a continuous group homomorphism into the multiplicative unit circle with its subspace topology. [def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles) [math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group) [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology) [math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism) [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top) [math:lem-unit-circle-is-a-compact-metrizable-topological-group](https://alphabetamath.cc/item/lem-unit-circle-is-a-compact-metrizable-topological-group)

## Proof

**Given:** The countable-choice assumption, the weight-two cuspidal representation with the stated unramified factor and trivial local scalar action, and the exponent $e$. For the Hurwitz application also use the conditions on $p,\ell$, the chosen splittings and the matching eigenline.

**Goal:** Bound the modulus of the index-$\ell^e$ scalar in the weight-one coset normalization and hence the Hurwitz scalar on the indicated line.

1.1 By [F2], $H$ is open, so every $H$-fixed Hilbert vector is smooth by the definition of smoothness. The smooth $H$-fixed space therefore equals the nonzero Hilbert $H$-fixed space, and [F2] gives its dimension as one. Apply [F1] to the given global representation with its closed invariant realization in the cuspidal Hilbert space of square-integrable classes with Borel descended moduli, the locally compact Hausdorff norm quotient with its invariant Radon measure, its full real weight-two type, its positive-real-scalar condition and its unramified factor. This gives $|u_\ell|=|v_\ell|=1$. Apply the eigenvalue formula of [F2] to that same local factor, whose scalar action is trivial. Two matrix lifts of a projective class differ by a local scalar, so their actions agree. Both suppliers use the same normalized Satake transform on this local fixed line, with the same weights attached to the triangular representatives and their diagonal valuations, so $\lambda_{\ell,e}=\ell^{e/2}\sum_{r=0}^e u_\ell^r v_\ell^{e-r}$. [given, F1, F2]

1.2 In the Hurwitz application, first check the splitting primes. Since $p$ is prime, $p>1$. If $k<0$, then $-k$ is a positive integer and hence at least $1$ by [F4]. The ordered ring laws give $p=4k+3\le-1$, contradicting $p>1$. Thus $k\ge0$ and $p\ge3$. Write $\ell=2b+1$ with $b$ an integer by the assumed oddness of $\ell$. The inequality $\ell>1$ gives $b>0$, so $b\ge1$ by the same integer order and $\ell\ge3$. The integral splitting theorem in [F5] therefore supplies the splittings at $p$ and $\ell$. [given, F4, F5]

2.1 For either parameter $z$, the modulus definition gives $|z^0|=|1|=1$. If $|z^n|=1$ then $|z^{n+1}|=|z^nz|=|z^n||z|=1$. Induction gives modulus one for every nonnegative power. For each $0\le r\le e$, the nonnegative integers $r,e-r$ represent natural exponents by [F4], so the multiplicative law gives $|u_\ell^r v_\ell^{e-r}|=1$. [F3, F4, step 1.1]

3.1 For $0\le n\le e+1$ put $S_n=\sum_{0\le r<n}u_\ell^r v_\ell^{e-r}$. The empty sum gives $|S_0|=0$. For $n<e+1$ the next sum is $S_{n+1}=S_n+u_\ell^n v_\ell^{e-n}$. Thus if $|S_n|\le n$, then $|S_{n+1}|\le |S_n|+1\le n+1$ by subadditivity and step 2.1. Apply induction to the property that $n\le e+1$ implies $|S_n|\le n$. The property is vacuous above $e+1$, and whenever the successor is at most $e+1$ the preceding estimate applies. Hence $|S_{e+1}|\le e+1$. [F3, F4, step 2.1]

4.1 The integer prime $\ell$ exceeds one, so its real image exceeds one by the order-preserving embeddings of [F4]. Thus its rational power $\ell^{e/2}$ is positive by [F3]. Its complex modulus equals itself since for real $t>0$, $|t+0i|=\sqrt{t^2}=t$ by uniqueness of the nonnegative square root. Multiplicativity applied to the formula in step 1.1 now gives $|\lambda_{\ell,e}|=\ell^{e/2}|S_{e+1}|\le(e+1)\ell^{e/2}$. When $e=0$ the sum consists of the term $1$ and the bound is equality. [given, F3, F4, step 1.1, step 3.1]

5.1 With these splittings, check the index before using the counting operator. At $e=0$ the index is the empty product $\ell^0=1$, which is positive, odd and prime to $p$. For $e>0$ write the index as the product of $e$ copies of the positive odd integer $\ell$. Starting at $1$, each successive product stays positive by [F5] and stays odd by $(2a+1)(2b+1)=2(2ab+a+b)+1$. Induction gives positivity and oddness. If $p$ divided the product, [F5] would give $p\mid\ell$, which is impossible for distinct primes $p,\ell$. Consequently the reduced norm of each element of $Q_{\ell^e}$ is prime to $p$, and by [F5] the reduction and the counting operator exist at this index. By the fixed-index hypothesis in the Statement the $T_{\ell^e}$ eigenvalue on the chosen line equals $\lambda_{\ell,e}$ in the stated weight-one normalization. Step 4.1 therefore gives the bound in the counting normalization. [given, F4, F5, step 4.1, step 1.2] ∎

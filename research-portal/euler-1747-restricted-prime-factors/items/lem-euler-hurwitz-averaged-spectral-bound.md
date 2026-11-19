---
id: lem-euler-hurwitz-averaged-spectral-bound
kind: lemma
title: Averaged spectral estimate for the torus normalizer
status: published
domain: mathematics
deps:
  - math:def-function-space
  - math:def-linear-subspace
  - math:def-field
  - math:def-semigroup-and-monoid
  - math:def-inner-product-space
  - math:thm-complex-numbers-form-a-field
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-linear-independence
  - math:def-linear-combination-and-span
  - math:lem-span-is-the-set-of-linear-combinations
  - math:cor-cauchy-reals-lub-complete
  - math:def-linear-basis
  - math:def-dimension
  - math:thm-dimension-of-a-linear-subspace
  - math:def-axiom-of-choice
  - def-euler-prime-classes
  - math:def-divides-in-z
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-euler-hurwitz-projective-reduction
  - math:def-coset
  - def-euler-hurwitz-torus-normalizer
  - def-euler-hurwitz-normalizer-orbit
  - math:def-finite-cardinality
  - def-euler-hurwitz-norm-shell
  - def-euler-hurwitz-hecke-operator
  - def-euler-divisor-functions
  - math:thm-of-square-roots
  - def-author-87b4d85727bc-counting-inner-product-on-finite-functions
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-linear-map
  - math:def-self-adjoint-and-normal-endomorphism
  - def-euler-hurwitz-determinant-character
  - math:def-orthogonality-and-orthogonal-complement
  - math:def-inner-product-norm
  - math:def-operator-norm-on-a-finite-dimensional-inner-product-space
  - math:thm-operator-norm-is-the-largest-singular-value
  - lem-euler-hurwitz-orbit-average
  - lem-euler-hurwitz-hecke-basic-properties
  - lem-euler-hurwitz-hecke-constant-eigenvalue
  - lem-euler-hurwitz-centered-orbit-norm
  - lem-euler-hurwitz-hecke-spectral-bound
  - lem-centered-indicator-rayleigh-bound
  - lem-euler-hurwitz-normalizer-orbit-size
  - math:thm-subset-of-a-finite-set
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-monoid-finite-product
  - math:thm-induction-principle
formulation_deps:
  - math:def-field
  - math:def-semigroup-and-monoid
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:thm-complex-numbers-form-a-field
  - math:cor-cauchy-reals-lub-complete
  - math:def-axiom-of-choice
  - def-euler-prime-classes
  - math:def-divides-in-z
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-euler-hurwitz-projective-reduction
  - math:def-coset
  - def-euler-hurwitz-torus-normalizer
  - def-euler-hurwitz-normalizer-orbit
  - math:def-finite-cardinality
  - def-euler-hurwitz-norm-shell
  - def-euler-hurwitz-hecke-operator
  - def-euler-divisor-functions
  - math:thm-of-square-roots
  - math:def-finite-sum-in-a-commutative-monoid
argument_deps:
  - math:def-function-space
  - math:def-linear-subspace
  - math:def-field
  - math:def-semigroup-and-monoid
  - math:def-inner-product-space
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-linear-independence
  - math:def-linear-combination-and-span
  - math:lem-span-is-the-set-of-linear-combinations
  - math:thm-complex-numbers-form-a-field
  - math:cor-cauchy-reals-lub-complete
  - math:def-linear-basis
  - math:def-dimension
  - math:thm-dimension-of-a-linear-subspace
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-normalizer-orbit
  - math:def-finite-cardinality
  - def-euler-hurwitz-norm-shell
  - def-euler-hurwitz-hecke-operator
  - def-euler-divisor-functions
  - math:thm-of-square-roots
  - def-author-87b4d85727bc-counting-inner-product-on-finite-functions
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-linear-map
  - math:def-self-adjoint-and-normal-endomorphism
  - def-euler-hurwitz-determinant-character
  - math:def-orthogonality-and-orthogonal-complement
  - math:def-inner-product-norm
  - math:def-operator-norm-on-a-finite-dimensional-inner-product-space
  - math:thm-operator-norm-is-the-largest-singular-value
  - lem-euler-hurwitz-orbit-average
  - lem-euler-hurwitz-hecke-basic-properties
  - lem-euler-hurwitz-hecke-constant-eigenvalue
  - lem-euler-hurwitz-centered-orbit-norm
  - lem-euler-hurwitz-hecke-spectral-bound
  - lem-centered-indicator-rayleigh-bound
  - lem-euler-hurwitz-normalizer-orbit-size
  - math:thm-subset-of-a-finite-set
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-monoid-finite-product
  - math:thm-induction-principle
dependency_roles:
  math:def-function-space: mathematical-premise
  math:def-linear-subspace: mathematical-premise
  math:def-field: mathematical-premise
  math:def-semigroup-and-monoid: mathematical-premise
  math:def-inner-product-space: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:def-linear-independence: mathematical-premise
  math:def-linear-combination-and-span: mathematical-premise
  math:lem-span-is-the-set-of-linear-combinations: mathematical-premise
  math:thm-complex-numbers-form-a-field: mathematical-premise
  math:cor-cauchy-reals-lub-complete: mathematical-premise
  math:def-linear-basis: mathematical-premise
  math:def-dimension: mathematical-premise
  math:thm-dimension-of-a-linear-subspace: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  def-euler-hurwitz-projective-reduction: mathematical-premise
  math:def-coset: mathematical-premise
  def-euler-hurwitz-torus-normalizer: mathematical-premise
  def-euler-hurwitz-normalizer-orbit: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  def-euler-hurwitz-norm-shell: mathematical-premise
  def-euler-hurwitz-hecke-operator: mathematical-premise
  def-euler-divisor-functions: mathematical-premise
  math:thm-of-square-roots: mathematical-premise
  def-author-87b4d85727bc-counting-inner-product-on-finite-functions: mathematical-premise
  math:def-complex-conjugate-real-imaginary-part-and-modulus: mathematical-premise
  math:def-linear-map: mathematical-premise
  math:def-self-adjoint-and-normal-endomorphism: mathematical-premise
  def-euler-hurwitz-determinant-character: mathematical-premise
  math:def-orthogonality-and-orthogonal-complement: mathematical-premise
  math:def-inner-product-norm: mathematical-premise
  math:def-operator-norm-on-a-finite-dimensional-inner-product-space: mathematical-premise
  math:thm-operator-norm-is-the-largest-singular-value: mathematical-premise
  lem-euler-hurwitz-orbit-average: mathematical-premise
  lem-euler-hurwitz-hecke-basic-properties: mathematical-premise
  lem-euler-hurwitz-hecke-constant-eigenvalue: mathematical-premise
  lem-euler-hurwitz-centered-orbit-norm: mathematical-premise
  lem-euler-hurwitz-hecke-spectral-bound: mathematical-premise
  lem-centered-indicator-rayleigh-bound: mathematical-premise
  lem-euler-hurwitz-normalizer-orbit-size: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
  math:thm-induction-principle: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: PDF p. 4, §3.3, equations (3.7)–(3.8) and the sentence following (3.8)
      reading_limits: Read the displayed formulas and the surrounding text on PDF page
        4 for attribution.
dependency_level: 11
---

## Statement

Assume the Axiom of Choice, which asserts that every family of nonempty sets has a choice function, a function selecting an element of each set in the family. Let $m=2a+1>0$ for an integer $a$, and let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$. Assume $p\nmid m$, meaning $m$ is not a multiple of $p$. A prime is an integer greater than $1$ with only $1$ and itself as positive divisors, and congruence to $3$ modulo $4$ means $p=4b+3$ for an integer $b$.

Use the fixed projective reduction $\rho_p$ at $p$. It takes Hurwitz quaternions of reduced norm not divisible by $p$ to classes in $G_p$, the group of invertible two-by-two matrices over the field $\mathbb F_p$ of residues modulo $p$, with matrices identified up to nonzero scalar multiples. The Hurwitz order $\mathcal H$ consists of rational Hamilton quaternions whose coordinates in $1,i,j,k$, with $i^2=j^2=-1$ and $ij=k=-ji$, are all integers or all integers plus $\tfrac12$. The reduced norm is the sum of the four coordinate squares. Let $\Gamma_p=\rho_p(\mathcal H^\times)$ be the image of the units, the elements with a two-sided inverse in $\mathcal H$. Write $Y_p=\Gamma_p\backslash G_p$ for the finite set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$, with $\Gamma_p$ the coset of the identity.

Let the torus $C_p$ be the projective image of the nonzero elements of the field $\mathbb F_p[i]$, whose elements have the form $a+b\bar i$ with $\bar i$ the residue of $i$ modulo $p$. The normalizer $K_p=\{k\in G_p:kC_pk^{-1}=C_p\}$ consists of the elements whose conjugation preserves $C_p$. Its orbit of the base coset is the set $\mathcal O_p=\{\Gamma_p k:k\in K_p\}$ of translates. Define the indicator $f_p$ to be $1$ on $\mathcal O_p$ and $0$ elsewhere on $Y_p$. Define the rational density $\mu_p=|\mathcal O_p|/|Y_p|$, where $|S|$ denotes the number of elements of a finite set $S$.

For a complex-valued function $f$ on $Y_p$, the quaternionic Hecke operator $T_m$ is the map given by
$$(T_m f)(\Gamma_p g)=\frac1{24}\sum_{\alpha\in Q_m} f(\Gamma_p\rho_p(\alpha)g),$$
where $Q_m$ is the set of elements of $\mathcal H$ with reduced norm $m$ and the finite sum adds one term per element. Let $m_{\mathbb N}$ be the unique positive natural number whose image in $\mathbb Z$ under the canonical inclusion is $m$. Write $\sigma(m)=\sigma(m_{\mathbb N})$ and $\tau(m)=\tau(m_{\mathbb N})$ for the natural-number sum and count of the positive divisors, respectively. The natural divisors used in these functions correspond under that inclusion to the integers $d>0$ such that $m=dq$ for some integer $q$. In scalar expressions, interpret naturals and integers in $\mathbb Q$ via the canonical inclusions, and interpret rational scalars in $\mathbb R$ via the constant-sequence embedding and in $\mathbb C$ via the further inclusion as constant classes. Let $\sqrt m$ denote the nonnegative square root of the real image of $m$.

Then $(T_m f_p)(\Gamma_p)$ is real and
$$(T_m f_p)(\Gamma_p)\le \sigma(m)\mu_p+\tau(m)\sqrt m(1-\mu_p).$$
At $p=3$, the error term $\tau(m)\sqrt m(1-\mu_p)$ vanishes.

## Statement references

[[math:def-axiom-of-choice]]

[[def-euler-prime-classes]]

[[math:def-divides-in-z]]

[[def-euler-hamilton-quaternions]]

[[def-euler-hurwitz-order]]

[[def-euler-hurwitz-projective-reduction]]

[[math:def-coset]]

[[def-euler-hurwitz-torus-normalizer]]

[[def-euler-hurwitz-normalizer-orbit]]

[[math:def-finite-cardinality]]

[[def-euler-hurwitz-norm-shell]]

[[def-euler-hurwitz-hecke-operator]]

[[math:def-finite-sum-in-a-commutative-monoid]]

[[math:def-field]]

[[math:def-semigroup-and-monoid]]

[[def-euler-divisor-functions]]

[[math:lem-nat-embeds-int]]

[[math:lem-int-embeds-rat]]

[[math:lem-rat-embeds-dense]]

[[math:thm-complex-numbers-form-a-field]]

[[math:thm-of-square-roots]]

[[math:cor-cauchy-reals-lub-complete]]

## Justification

The orbit definition gives $\Gamma_p\in\mathcal O_p\subseteq Y_p$, since the identity belongs to $K_p$. The finite-subset theorem applied to $\mathcal O_p\subseteq Y_p$ gives finiteness of the orbit because $Y_p$ is finite. Both sets are nonempty, so both counts in $\mu_p$ are positive. For $\alpha\in Q_m$, the assumption $p\nmid m$ puts $\alpha$ in the domain of $\rho_p$. The Hecke definition gives a finite sum independent of the coset representative. For $f=f_p$, each term is the complex image of the real number $0$ or $1$. Proof step 1.3 shows by the finite-sum recursion that the real average maps to the Hecke value. [[def-euler-hurwitz-normalizer-orbit]] [[def-euler-hurwitz-projective-reduction]] [[math:thm-subset-of-a-finite-set]] [[math:def-finite-cardinality]] [[def-euler-hurwitz-norm-shell]] [[def-euler-hurwitz-hecke-operator]] [[math:thm-complex-numbers-form-a-field]] [[math:def-finite-sum-in-a-commutative-monoid]] [[math:def-monoid-finite-product]] [[math:thm-induction-principle]]

## Facts & Assumptions

[F1] For a field $F$ and a set $X$, the functions $X\to F$ form a vector space with pointwise addition and scalar multiplication and the constant zero function. [[math:def-function-space]] On the complex-valued functions on $Y_p$ with these operations, use the counting inner product $\langle u,v\rangle_p=\sum_{y\in Y_p}u(y)\overline{v(y)}$. The bar denotes complex conjugation, which sends $a+bi$ to $a-bi$ for real $a,b$ and the complex imaginary unit $i$. For the specified $m$ and $p$, the orbit-pairing identity is $(T_m f_p)(\Gamma_p)=\langle f_p,T_m f_p\rangle_p/|\mathcal O_p|$. [[def-author-87b4d85727bc-counting-inner-product-on-finite-functions]] [[math:def-complex-conjugate-real-imaginary-part-and-modulus]] [[lem-euler-hurwitz-orbit-average]]

[F2] For the specified $m$ and $p$, $T_m$ is linear, so it preserves complex linear combinations, and self-adjoint, so $\langle T_m u,v\rangle_p=\langle u,T_m v\rangle_p$. Also $T_m\mathbf1=\sigma(m)\mathbf1$, where $\mathbf1$ has value $1$ at every coset. [[math:def-linear-map]] [[math:def-self-adjoint-and-normal-endomorphism]] [[lem-euler-hurwitz-hecke-basic-properties]] [[lem-euler-hurwitz-hecke-constant-eigenvalue]]

[F3] The determinant character $\chi_p$ assigns to a coset the value $1$ when the determinant of a matrix representing it is a nonzero square in $\mathbb F_p$ and $-1$ otherwise. A square has the form $t^2$ for $t\in\mathbb F_p$, and the determinant for rows $(a,b)$ and $(c,d)$ is $ad-bc$. The determinant-character definition makes the sign independent of the representative. Two functions are orthogonal when their inner product is zero. The orthogonal complement $W=\{\mathbf1,\chi_p\}^{\perp}$ consists of the functions orthogonal to both. It is a linear subspace, so it contains zero and is closed under complex linear combinations. A linear subspace is itself a vector space with the restricted addition and scalar multiplication and the same zero as the ambient space. [[math:def-linear-subspace]] The centered indicator $h_p=f_p-\mu_p\mathbf1$ belongs to $W$ by the centered-orbit lemma. [[def-euler-hurwitz-determinant-character]] [[math:def-orthogonality-and-orthogonal-complement]] [[lem-euler-hurwitz-centered-orbit-norm]]

[F4] Under the Axiom of Choice and the stated conditions on $m$ and $p$, $T_m(W)\subseteq W$. Once $W$ is shown to be finite-dimensional, the spectral bound on the restriction is $\|T_m|_W\|\le\tau(m)\sqrt m$. Here $T_m|_W$ is the restriction sending $w\in W$ to $T_mw$. If $W$ is finite-dimensional and nonzero, the operator-norm theorem gives an attained maximum of $\|T_mw\|_p$ over $w\in W$ of norm $1$, and the operator norm is that maximum. On the zero space the operator norm is $0$. The function norm is $\|w\|_p=\sqrt{\langle w,w\rangle_p}$. [[lem-euler-hurwitz-hecke-spectral-bound]] [[math:def-operator-norm-on-a-finite-dimensional-inner-product-space]] [[math:thm-operator-norm-is-the-largest-singular-value]] [[math:def-inner-product-norm]]

[F5] For a nonempty subset $O$ of a finite nonempty set $Y$, let $f$ be its indicator and $\mu=|O|/|Y|$. Use the counting inner product on the complex functions on $Y$. If a linear self-adjoint map $T$ satisfies $T\mathbf1=d\mathbf1$ for real $d$, and $f-\mu\mathbf1$ lies in a linear subspace preserved by $T$ on which the restricted operator norm is at most $L\ge0$, then $\langle f,Tf\rangle/|O|\le d\mu+L(1-\mu)$. [[lem-centered-indicator-rayleigh-bound]]

[F6] The orbit-size formula gives $\mu_p=6/[p(p-1)]$, so $\mu_3=1$. [[lem-euler-hurwitz-normalizer-orbit-size]]

[F7] The coset set $Y_p$ is finite and $\mathcal O_p\subseteq Y_p$, so the finite-subset theorem makes $\mathcal O_p$ finite. The identity coset $\Gamma_p$ belongs to the orbit, so both sets are nonempty and their cardinalities are positive. The shell $Q_m$ is finite by the justification of the Hecke formula, which evaluates the operator on the indicator as $1/24$ times a sum of zeros and ones. The complex field contains the real field by the injective field map sending each real to its constant class. This map sends $0$ and $1$ to their complex counterparts and preserves addition and quotients with nonzero denominator. [[def-euler-hurwitz-normalizer-orbit]] [[def-euler-hurwitz-projective-reduction]] [[math:thm-subset-of-a-finite-set]] [[math:def-finite-cardinality]] [[def-euler-hurwitz-hecke-operator]] [[math:thm-complex-numbers-form-a-field]]

[F8] The divisor sum $\sigma(m)$ and count $\tau(m)$ at $m_{\mathbb N}$ are natural numbers. The real square root $\sqrt m$ is nonnegative. The Cauchy-sequence real field has the least-upper-bound property and is a complete ordered field, so each nonnegative real has a unique nonnegative square root. [[def-euler-divisor-functions]] [[math:cor-cauchy-reals-lub-complete]] [[math:thm-of-square-roots]]

[F9] A finite linear combination uses a list of scalar multiples, with the sum starting at the zero vector and adding the next term at each index. The span of a subset is the set of its finite linear combinations. A subset is linearly independent if every injective finite list in it has only zero coefficients in any linear combination equal to zero. A basis is a linearly independent spanning set. A vector space is finite-dimensional if it has a finite basis, and its dimension is the number of elements of that basis. Every linear subspace of a finite-dimensional vector space over a field is finite-dimensional over that field. [[math:def-linear-basis]] [[math:def-linear-independence]] [[math:def-linear-combination-and-span]] [[math:lem-span-is-the-set-of-linear-combinations]] [[math:def-dimension]] [[math:thm-dimension-of-a-linear-subspace]]

[F10] The canonical inclusion $n\mapsto[(n,0)]$ identifies $\mathbb N$ with the nonnegative integers and preserves arithmetic and order. The inclusion $k\mapsto[(k,1)]$ into $\mathbb Q$ preserves arithmetic and order, and the constant-sequence embedding $q\mapsto\widehat q$ is an embedding of ordered fields. These maps and the real-to-complex inclusion in [F7] send $0$ to $0$ and $1$ to $1$ in the respective targets, so the image of a natural number is the sum of that many copies of the unit. The field embeddings preserve quotients with nonzero denominator. [[math:lem-nat-embeds-int]] [[math:lem-int-embeds-rat]] [[math:lem-rat-embeds-dense]] [[math:thm-complex-numbers-form-a-field]]

[F11] A complex inner product on a complex vector space is a complex-valued pairing that is linear in the first variable and conjugate symmetric, with real nonnegative diagonal values that vanish exactly at the zero vector. [[math:def-inner-product-space]]

[F12] The field axioms give associative and commutative addition with two-sided identity $0$ in both the real field of [F8] and the complex field of [F7]. Thus each field under addition with identity $0$ is a commutative monoid. [[math:def-field]] [[math:def-semigroup-and-monoid]] [[math:cor-cauchy-reals-lub-complete]] [[math:thm-complex-numbers-form-a-field]] A sum in either field over a finite set uses an enumeration of that set without repetition. With indices starting at zero, the empty sum is $0$ and the sum of the first $j+1$ terms is the sum of the first $j$ terms plus the term at index $j$. [[math:def-finite-sum-in-a-commutative-monoid]] [[math:def-monoid-finite-product]]

[F13] Induction extends a property of natural indices from zero and its passage to each successor. [[math:thm-induction-principle]]

## Proof

**Given:** The Axiom of Choice, a positive odd integer $m$, a prime $p\in\mathcal P_3$ with $p\nmid m$, and the fixed reduction at $p$.

**Goal:** Prove the estimate for $(T_m f_p)(\Gamma_p)$ and the vanishing of its error term when $p=3$.

1.1 Use $Y=Y_p$ and $O=\mathcal O_p$ in the centered-indicator bound. The coset set $Y_p$ is finite by [F7], so the finite-subset theorem in [F7] applies to $\mathcal O_p\subseteq Y_p$. Both sets are nonempty because $\Gamma_p$ belongs to the orbit. The indicator is $f_p$. The real embedding in [F10] sends the rational density $\mu_p$ to the quotient of the two real counts, since it preserves division and $|Y_p|>0$. The two counts are sums of real ones under these inclusions, so this is the density in [F5]. The pairing in [F1] is the counting inner product required by [F5]. The map $T_m$ is linear and self-adjoint and acts on $\mathbf1$ by the complex image of the real scalar $d=\sigma(m)$, since that image is the natural-number scalar of [F2]. [F1, F2, F5, F7, F8, F10]

1.2 Let $V$ be the set of functions from $Y_p$ to $\mathbb C$. Because $\mathbb C$ is a field by [F7], the function-space result in [F1] makes $V$ a complex vector space under the pointwise operations. For each $y\in Y_p$, define $e_y$ to be $1$ at $y$ and $0$ at every other coset. By [F7], fix a list $y_0,\ldots,y_{n-1}$ of all cosets without repetition, where $n=|Y_p|$. The corresponding indicators are distinct because evaluating at $y_j$ distinguishes $e_{y_j}$ from every other indicator. For each $u\in V$, form the finite linear combination $\sum_{j<n}u(y_j)e_{y_j}$. At a coset $z$, the recursion in [F9] starts with value $0$ and, by the pointwise operations in [F1], at index $j$ adds $u(y_j)e_{y_j}(z)$. Every increment is zero except at the unique index with $y_j=z$, where the increment is $u(z)$. The linear combination therefore equals $u$, and the span of the indicators is all of $V$ by [F9]. For any injective finite list $e_{z_0},\ldots,e_{z_{r-1}}$ of these indicators, suppose $\sum_{j<r}c_j e_{z_j}=0$. The $z_j$ are distinct. By the same recursion, the sum evaluated at $z_j$ starts at zero and adds zero at every index other than $j$, where it adds $c_j$. Thus $c_j=0$ for each $j<r$. The empty list has no coefficients to check. [F1, F7, F9]

1.3 Write $\iota:\mathbb R\to\mathbb C$ for the field embedding in [F7]. Use one enumeration of $Q_m$ without repetition for the real and complex sums and let $N=|Q_m|$ be its length. For $j<N$, write $\alpha_j$ for the shell element at index $j$. Take $a_j\in\mathbb R$ to be $1$ if $\Gamma_p\rho_p(\alpha_j)\in\mathcal O_p$ and $0$ otherwise. The complex term is then $\iota(a_j)$. In both additive monoids, apply the partial-sum recursion from [F12]. Extend both term lists by zeros. Let $R_j$ be the sum of the first $j$ real terms and $C_j$ the sum of the first $j$ complex terms. By [F12], $C_0=0=\iota(R_0)$. If $C_j=\iota(R_j)$, then $C_{j+1}=\iota(R_j)+\iota(a_j)=\iota(R_j+a_j)=\iota(R_{j+1})$, with $a_j=0$ for $j\ge N$. Induction gives $C_N=\iota(R_N)$. The scalar $24$ is positive in $\mathbb R$, and [F10] identifies its image with the complex scalar $24$. Hence $(T_mf_p)(\Gamma_p)=C_N/24=\iota(R_N/24)$ by [F7], including the case $N=0$. Injectivity gives a unique real preimage. [F7, F10, F12, F13]

2.1 The indicators thus form a basis, so [F9] gives $V$ dimension $|Y_p|$ over $\mathbb C$. Since $W$ is a linear subspace of $V$ by [F3], [F9] shows that $W$ is finite-dimensional. By [F3], $W$ is a complex vector space with the operations restricted from $V$ and with the same zero as $V$. Restrict the counting pairing from [F1] to $W\times W$. Linearity in the first variable and conjugate symmetry hold for vectors in $W$ because they hold in $V$ and $W$ is closed under complex linear combinations. The diagonal values are real and nonnegative and vanish exactly at the zero vector, which is the same in $W$ and $V$. By [F11], the restricted pairing is an inner product on $W$. [F1, F3, F7, F9, F11, step 1.2]

3.1 The density from step 1.1 has the same complex image as the rational fraction used in [F3], so the centered indicator of [F5] is $f_p-\mu_p\mathbf1$. By [F3] it belongs to $W$. The Axiom of Choice and the stated conditions on $m$ and $p$ give the invariance $T_m(W)\subseteq W$ by [F4]. The restriction is linear by [F2]. By step 2.1 the domain and codomain of the restriction are the same finite-dimensional complex inner product space $W$. By [F4] its norm is an attained maximum when $W\ne0$ and is $0$ when $W=0$. The spectral bound in [F4] gives $\|T_m|_W\|\le L=\tau(m)\sqrt m$. The positive integer $m$ and the natural count $\tau(m)$ have nonnegative real images by [F10]. Thus $L\ge0$, since $\sqrt m$ is nonnegative by [F8]. [given, F2, F3, F4, F8, F10, step 1.1, step 2.1]

4.1 Applying [F5] with these data gives $\langle f_p,T_m f_p\rangle_p/|\mathcal O_p|\le\sigma(m)\mu_p+\tau(m)\sqrt m(1-\mu_p)$. The complex image of the real count $|\mathcal O_p|$ is the same sum of complex ones in both quotient formulas by [F10]. The orbit-pairing identity replaces the left side by $(T_m f_p)(\Gamma_p)$. Use its real preimage from step 1.3 for the inequality. [F1, F5, F10, step 1.1, step 3.1, step 1.3]

5.1 At $p=3$, [F6] gives $\mu_3=1$ in $\mathbb Q$, and the embedding in [F10] preserves $1$. Therefore $\tau(m)\sqrt m(1-\mu_3)=0$ in $\mathbb R$. This proves the estimate and the stated vanishing. [F6, F10, step 4.1] ∎

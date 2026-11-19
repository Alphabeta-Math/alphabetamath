---
title: Identification of the unramified Hecke correspondence with the finite operator
status: published
research_item: lem-euler-hurwitz-adelic-hecke-identification
dependency_level: 7
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, Lemma 3.2, paragraph following the stabilizer and last sentence
        of the proof
---

PDF p. 3: ` Lemma 3.2, paragraph following the stabilizer description `; PDF p. 3: ` Lemma 3.2, last sentence of the proof `

## Prerequisites

- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)
- [thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure)
- [def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)
- [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)
- [def-finite-quaternion-adeles-and-projective-units](item-def-finite-quaternion-adeles-and-projective-units)
- [def-euler-hurwitz-adelic-level](item-def-euler-hurwitz-adelic-level)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [lem-euler-hurwitz-adelic-identification](item-lem-euler-hurwitz-adelic-identification)
- [thm-hurwitz-integral-splitting-at-odd-primes](item-thm-hurwitz-integral-splitting-at-odd-primes)
- [def-determinant-index-spherical-hecke-correspondence](item-def-determinant-index-spherical-hecke-correspondence)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [def-quaternion-right-ideal-and-reduced-norm](item-def-quaternion-right-ideal-and-reduced-norm)
- [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)
- [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)
- [lem-degree-two-spherical-index-cosets](item-lem-degree-two-spherical-index-cosets)
- [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)
- [thm-adelic-right-ideal-dictionary](item-thm-adelic-right-ideal-dictionary)
- [cor-euler-hurwitz-right-class-number](item-cor-euler-hurwitz-right-class-number)
- [lem-rational-hamilton-norm-and-inverse](item-lem-rational-hamilton-norm-and-inverse)
- [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)
- [lem-euler-hurwitz-hecke-basic-properties](item-lem-euler-hurwitz-hecke-basic-properties)
- [math:thm-complex-spectral-theorem-for-normal-endomorphisms](https://alphabetamath.cc/item/thm-complex-spectral-theorem-for-normal-endomorphisms)
- [math:thm-simultaneous-diagonalisation-of-commuting-diagonalisable-endomorphisms](https://alphabetamath.cc/item/thm-simultaneous-diagonalisation-of-commuting-diagonalisable-endomorphisms)
- [math:lem-finite-sum-reindexing-and-fubini](https://alphabetamath.cc/item/lem-finite-sum-reindexing-and-fubini)
- [math:lem-coset-membership-and-equality](https://alphabetamath.cc/item/lem-coset-membership-and-equality)
- [math:def-countable](https://alphabetamath.cc/item/def-countable)
- [math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice)
- [math:def-linear-combination-and-span](https://alphabetamath.cc/item/def-linear-combination-and-span)
- [math:def-linear-independence](https://alphabetamath.cc/item/def-linear-independence)
- [math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis)
- [math:def-dimension](https://alphabetamath.cc/item/def-dimension)
- [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-linear-subspace](https://alphabetamath.cc/item/def-linear-subspace)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:def-adjoint-of-a-linear-map-between-inner-product-spaces](https://alphabetamath.cc/item/def-adjoint-of-a-linear-map-between-inner-product-spaces)
- [math:thm-adjoint-exists-and-is-unique-in-finite-dimension](https://alphabetamath.cc/item/thm-adjoint-exists-and-is-unique-in-finite-dimension)
- [math:def-self-adjoint-and-normal-endomorphism](https://alphabetamath.cc/item/def-self-adjoint-and-normal-endomorphism)
- [math:def-left-right-and-two-sided-ideal](https://alphabetamath.cc/item/def-left-right-and-two-sided-ideal)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-diagonalisable-endomorphism](https://alphabetamath.cc/item/def-diagonalisable-endomorphism)
- [math:def-simultaneous-diagonalisability-of-a-family](https://alphabetamath.cc/item/def-simultaneous-diagonalisability-of-a-family)


## Statement

Assume countable choice, meaning that each sequence of nonempty sets has a function selecting one element from each set. Let $p$ be a prime congruent to $3$ modulo $4$ and $m$ a positive odd integer with $p\nmid m$. A prime is an integer greater than one with only $1$ and itself as positive divisors. Write $\ell^e\parallel m$ when the exponent of the prime $\ell$ in $m$ is $e>0$.

Let $B$ be the rational Hamilton algebra with basis $1,i,j,k$, multiplication given by $i^2=j^2=-1$ and $ij=k=-ji$, and reduced norm $N$ equal to the sum of the four coordinate squares. Its Hurwitz order $\mathcal H$ is the subring with coordinates either all integers or all integers plus $\tfrac12$, and is the integer span of a rational basis of $B$. Put $Q_m=\{\alpha\in\mathcal H:N(\alpha)=m\}$ and write $\mathcal H^\times$ for the elements with two-sided inverses in $\mathcal H$.

For each prime $\ell$, let $\mathbb Q_\ell$ be the completion of $\mathbb Q$ for the absolute value $\ell^{-v_\ell}$ on nonzero rationals, with absolute value zero at zero. The valuation on a nonzero rational subtracts the exponent of $\ell$ in its denominator from the exponent in its numerator and extends to $\mathbb Q_\ell^\times$ with $v_\ell(\ell)=1$. Let $\mathbb Z_\ell$ consist of zero and the elements of nonnegative valuation. Write $B_\ell$ and $\mathcal H_\ell$ for the corresponding spans over $\mathbb Q_\ell$ and $\mathbb Z_\ell$. Put $G(\mathbb Q_\ell)=B_\ell^\times/\mathbb Q_\ell^\times$, the invertible local quaternions modulo nonzero scalar multiplication, and let $K_\ell$ be the image of $\mathcal H_\ell^\times$ there. The finite adelic group $G(\mathbb A_f)$ consists of tuples of these local classes lying in $K_\ell$ at all but finitely many primes, with componentwise multiplication. The rational group $G(\mathbb Q)=B^\times/\mathbb Q^\times$ acts by diagonal left multiplication.

At $p$ and at each prime dividing $m$, use integral splittings $\Phi_\ell:B_\ell\to M_2(\mathbb Q_\ell)$, algebra isomorphisms to the two-by-two matrix rings carrying $\mathcal H_\ell$ onto $M_2(\mathbb Z_\ell)$. At $p$ use the same splitting for both reductions. Let $G_p=\mathrm{PGL}_2(\mathbb F_p)$ be the invertible matrices over the field of residues modulo $p$ up to nonzero scalars. Let $r_p:K_p\to G_p$ reduce an integral invertible representative and let $\rho_p$ apply the same projective reduction to $\alpha\in\mathcal H$ with $p\nmid N(\alpha)$. Put $\Gamma_p=\rho_p(\mathcal H^\times)$ and $Y_p=\{\Gamma_p g:g\in G_p\}$. The subgroup $U(p)$ has factors $K_\ell$ for $\ell\ne p$ and $\ker r_p$ at $p$. The double coset set $X=G(\mathbb Q)\backslash G(\mathbb A_f)/U(p)$ consists of classes under left multiplication by $G(\mathbb Q)$ and right multiplication by $U(p)$. It identifies with $Y_p$ by sending an integral representative $k\in\prod_\ell K_\ell$ to $\Gamma_p r_p(k_p)$.

For $\ell^e\parallel m$, the determinant-index Hecke correspondence uses all the cosets $h_\ell K_\ell=\{h_\ell u:u\in K_\ell\}$ in the projective image of the integral matrices of determinant valuation $e$, including any matrices with all entries divisible by $\ell$. Its action sums evaluations at the classes of the right products by these representatives, each with weight one. The combined index-$m$ correspondence sums over tuples of these representatives, with identity components at the other primes.

The local cosets parametrize full integral right $\mathcal H_\ell$-ideals of norm valuation $e$. Such an ideal is the $\mathbb Z_\ell$-span of a $\mathbb Q_\ell$-basis of $B_\ell$, contained in $\mathcal H_\ell$ and stable under right multiplication by it. Its norm valuation is the valuation of a generator of the $\mathbb Z_\ell$-span of its element norms. The combined tuples parametrize the nonzero integral right ideals of $\mathcal H$ of reduced norm $m$, where the reduced norm of an ideal is the positive generator of the integer span of its element norms. Each ideal is $\alpha\mathcal H$ for an $\alpha\in Q_m$, unique up to right multiplication by a Hurwitz unit.

After reindexing by those ideals, the summands at $\Gamma_p g$ evaluate at $\Gamma_p\rho_p(\alpha)^{-1}g$. Here $\rho_p(\alpha)^{-1}$ is also the reduction of the local unit $\alpha^{-1}$. Quaternion conjugation $\alpha=a+bi+cj+dk\mapsto\bar\alpha=a-bi-cj-dk$ exchanges the classes $\alpha\mathcal H^\times$ and $\mathcal H^\times\bar\alpha$, and $\alpha^{-1}$ and $\bar\alpha$ have the same projective class. The resulting operator on complex-valued functions on $Y_p$ is
$$(T_m f)(\Gamma_p g)=\frac{1}{24}\sum_{\beta\in Q_m} f(\Gamma_p\rho_p(\beta)g).$$
The prime-power operators $T_{\ell^e}$ for $\ell^e\parallel m$ commute and $T_m=\prod_{\ell^e\parallel m}T_{\ell^e}$. The operator product uses composition. They have a common eigenbasis, a basis of nonzero functions on which each acts by a scalar. On that basis the eigenvalues of $T_m$ are products of the corresponding prime-power eigenvalues under complex multiplication. When $m=1$ the empty product is the identity with eigenvalue $1$.

## Statement references

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)

[thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure)

[def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)

[def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)

[def-finite-quaternion-adeles-and-projective-units](item-def-finite-quaternion-adeles-and-projective-units)

[def-euler-hurwitz-adelic-level](item-def-euler-hurwitz-adelic-level)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[lem-euler-hurwitz-adelic-identification](item-lem-euler-hurwitz-adelic-identification)

[thm-hurwitz-integral-splitting-at-odd-primes](item-thm-hurwitz-integral-splitting-at-odd-primes)

[def-determinant-index-spherical-hecke-correspondence](item-def-determinant-index-spherical-hecke-correspondence)

[math:def-coset](https://alphabetamath.cc/item/def-coset)

[def-quaternion-right-ideal-and-reduced-norm](item-def-quaternion-right-ideal-and-reduced-norm)

[def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)

[def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)

[math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis)

[math:def-countable](https://alphabetamath.cc/item/def-countable)

[math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)

[math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

[math:def-simultaneous-diagonalisability-of-a-family](https://alphabetamath.cc/item/def-simultaneous-diagonalisability-of-a-family)

## Facts & Assumptions

[F1] Use countable choice and the prime condition in the Statement. Unique prime factorization gives the finite list of positive exponents of $m$, with none at $2$ or $p$. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) [def-euler-prime-classes](item-def-euler-prime-classes) [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)

[F2] The Hurwitz order has integer basis $1,i,j,(-1+i+j+k)/2$ and integral reduced norm. The local spans use the same basis, and the Hurwitz order is closed under conjugation. The valuation is additive on nonzero products and vanishes exactly on scalar units of $\mathbb Z_\ell$. In the local Hamilton algebra $x+\bar x=2x_0$ and $x\bar x=N(x)1$, with $x_0$ the scalar coordinate. In $B$, conjugation reverses products, is its own inverse, and gives $x^{-1}=\bar x/N(x)$ for $x\ne0$. [thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure) [def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions) [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation) [lem-rational-hamilton-norm-and-inverse](item-lem-rational-hamilton-norm-and-inverse)

[F3] Integral splittings exist at odd primes. For $R=\mathbb Z_\ell$ write $\mathrm{GL}_2(R)$ for the matrices invertible over $R$. The cosets $A\,\mathrm{GL}_2(R)$ of integral matrices of fixed determinant valuation $e$ map bijectively to the projective cosets $[A]K_\ell$ under the splitting. There are finitely many, represented by upper triangular matrices with diagonal $(\ell^r,\ell^{e-r})$, $0\le r\le e$, and upper entry ranging over the residues modulo $\ell^r$. The ideal $AM_2(R)$ consists of the matrices with both columns in $AR^2$, and equality of these column lattices is equivalent to equality of matrix cosets. [thm-hurwitz-integral-splitting-at-odd-primes](item-thm-hurwitz-integral-splitting-at-odd-primes) [lem-degree-two-spherical-index-cosets](item-lem-degree-two-spherical-index-cosets)

[F4] If $A\in M_2(\mathbb Z_\ell)$ has nonzero determinant of valuation $e$ and $U,V\in\mathrm{GL}_2(\mathbb Z_\ell)$, then $UAV$ is integral with determinant of valuation $e$. The determinant-index support is invariant under left and right multiplication by the local integral group. Its correspondence acts by the finite coset sum of weight one on functions invariant under the right action of that group. A coset $hK$ consists of $hu$ for $u\in K$. Coset equality $h'K=hK$ holds exactly when $h^{-1}h'\in K$, which is also the condition for $h'\in hK$. [def-determinant-index-spherical-hecke-correspondence](item-def-determinant-index-spherical-hecke-correspondence) [math:def-coset](https://alphabetamath.cc/item/def-coset) [math:lem-coset-membership-and-equality](https://alphabetamath.cc/item/lem-coset-membership-and-equality)

[F5] For an order that is the integer span of a rational basis of $B$, the ideal dictionary sends a tuple $x=(x_\ell)_\ell$ of invertible local quaternions, integral units at all but finitely many primes, to $I_x=B\cap\prod_\ell x_\ell\mathcal H_\ell$ for the order $\mathcal H$. It gives the integer spans of rational bases in $B$ stable under right multiplication by $\mathcal H$ whose local spans are generated by a single invertible local quaternion. The completed spans are $x_\ell\mathcal H_\ell$, and determine the tuple up to integral unit multiplication on the right. Integrality of the ideal means containment in $\mathcal H$, equivalently containment of its spans in the local orders. Its norm has prime exponents $v_\ell(N(x_\ell))$. The local norm ideal of $x_\ell\mathcal H_\ell$ is $N(x_\ell)\mathbb Z_\ell$. Every nonzero integral right ideal of $\mathcal H$ is principal, and the norm of $\alpha\mathcal H$ is $N(\alpha)$. [thm-adelic-right-ideal-dictionary](item-thm-adelic-right-ideal-dictionary) [def-quaternion-right-ideal-and-reduced-norm](item-def-quaternion-right-ideal-and-reduced-norm) [cor-euler-hurwitz-right-class-number](item-cor-euler-hurwitz-right-class-number)

[F6] The finite adelic group has the tuple presentation in the Statement. The level is $\prod_\ell K_\ell$ with the single factor at $p$ replaced by $\ker r_p$. Reduction $r_p$ preserves products and agrees with $\rho_p$ on local classes of elements of $\mathcal H$ of norm prime to $p$. Every point of $X$ has an integral representative, and the stated map to $Y_p$ is a bijection. [def-finite-quaternion-adeles-and-projective-units](item-def-finite-quaternion-adeles-and-projective-units) [def-euler-hurwitz-adelic-level](item-def-euler-hurwitz-adelic-level) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [lem-euler-hurwitz-adelic-identification](item-lem-euler-hurwitz-adelic-identification)

[F7] The finite norm shell $Q_m$ is preserved by conjugation and by left and right multiplication by the $24$ Hurwitz units, all of norm $1$. The shell operator $T_m$ is well-defined, complex-linear and self-adjoint for the counting inner product $\langle f,h\rangle=\sum_{y\in Y_p}f(y)\overline{h(y)}$. Self-adjointness means $\langle T_m f,h\rangle=\langle f,T_m h\rangle$ for all $f,h$. This applies to every positive odd index prime to $p$. [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell) [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list) [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator) [lem-euler-hurwitz-hecke-basic-properties](item-lem-euler-hurwitz-hecke-basic-properties)

[F8] A complex-linear endomorphism of a finite-dimensional complex inner product space is normal when it commutes with its adjoint. [math:def-self-adjoint-and-normal-endomorphism](https://alphabetamath.cc/item/def-self-adjoint-and-normal-endomorphism) Every such normal endomorphism has an orthonormal eigenbasis. [math:thm-complex-spectral-theorem-for-normal-endomorphisms](https://alphabetamath.cc/item/thm-complex-spectral-theorem-for-normal-endomorphisms) An endomorphism of a finite-dimensional vector space over a field is diagonalisable over that field if it has a basis of eigenvectors over the field. [math:def-diagonalisable-endomorphism](https://alphabetamath.cc/item/def-diagonalisable-endomorphism) A family is simultaneously diagonalisable if and only if it has a common eigenbasis. [math:def-simultaneous-diagonalisability-of-a-family](https://alphabetamath.cc/item/def-simultaneous-diagonalisability-of-a-family) A pairwise commuting family of diagonalisable endomorphisms of a finite-dimensional vector space is simultaneously diagonalisable. [math:thm-simultaneous-diagonalisation-of-commuting-diagonalisable-endomorphisms](https://alphabetamath.cc/item/thm-simultaneous-diagonalisation-of-commuting-diagonalisable-endomorphisms)

[F9] Every nonempty subset of the nonnegative integers has a least element. [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)

[F10] Finite sums in a commutative monoid are invariant under bijective reindexing, and a sum over the Cartesian product of two finite sets equals the iterated sum in either order. [math:lem-finite-sum-reindexing-and-fubini](https://alphabetamath.cc/item/lem-finite-sum-reindexing-and-fubini)

[F11] The set $Y_p$ is finite and contains the identity coset $\Gamma_p$. On its space of complex-valued functions with pointwise operations, the counting pairing in [F7] is an inner product. [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[F12] For a finite index set $I$, fix a bijection $\iota$ from $\{j\in\mathbb N: j<n\}$ to $I$ for some nonnegative integer $n$. If each $S_i$ for $i\in I$ is nonempty, finite choice applied to the list of sets $S_{\iota(j)}$ gives a choice function $c$ on its set of values. Select $c(S_i)\in S_i$ at each $i\in I$. [math:def-countable](https://alphabetamath.cc/item/def-countable) [math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice)

[F13] A subset spans a vector space if the smallest linear subspace containing it is the whole space. A subset is linearly independent if every vanishing finite linear combination of distinct members has all coefficients zero. A basis is a linearly independent spanning subset. A vector space is finite-dimensional if it has a finite basis. [math:def-linear-combination-and-span](https://alphabetamath.cc/item/def-linear-combination-and-span) [math:def-linear-independence](https://alphabetamath.cc/item/def-linear-independence) [math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis) [math:def-dimension](https://alphabetamath.cc/item/def-dimension) A linear subspace contains zero and is closed under addition and multiplication by scalars of the ambient field. [math:def-linear-subspace](https://alphabetamath.cc/item/def-linear-subspace)

[F14] A Cartesian product of a finite list of finite sets is finite. The product of an empty list of sets consists of the single empty tuple. [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule) A subset of a finite set is finite. [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)

[F15] A finite sum in the additive monoid of the complex numbers is obtained by adding its terms in any enumeration, starting from zero. [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid) The complex numbers form a field containing the real numbers. [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

[F16] A linear map $S$ is an adjoint of $T$ on the same inner product space when $\langle Tf,h\rangle=\langle f,Sh\rangle$ for all $f,h$. [math:def-adjoint-of-a-linear-map-between-inner-product-spaces](https://alphabetamath.cc/item/def-adjoint-of-a-linear-map-between-inner-product-spaces) In finite dimension a linear endomorphism of a complex inner product space has exactly one adjoint. [math:thm-adjoint-exists-and-is-unique-in-finite-dimension](https://alphabetamath.cc/item/thm-adjoint-exists-and-is-unique-in-finite-dimension)

[F17] An $R$-submodule of $R^2$ contains zero and is closed under differences and multiplication by scalars in $R$. [lem-degree-two-spherical-index-cosets](item-lem-degree-two-spherical-index-cosets) In a commutative ring $R$, an ideal contains zero and is closed under differences and multiplication by arbitrary elements of $R$. These conditions suffice for being an ideal. [math:def-left-right-and-two-sided-ideal](https://alphabetamath.cc/item/def-left-right-and-two-sided-ideal)

[F18] A finite product in a monoid starts at its identity, and the product of a prefix extended by one term is the prefix product multiplied on the right by that term. [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)

[F19] A property of nonnegative integers holds for all such integers if it holds at zero and each case implies its successor. [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

## Proof

**Given:** Countable choice, $p$, $m$, and the groups and reductions in the Statement.

**Goal:** Identify the index-$m$ coset sum with $T_m$ and factor the operators and eigenvalues.

1.1 At an odd prime put $A=\Phi_\ell(x)$ for $x\in B_\ell$. Applying $\Phi_\ell$ to the identities for $x+\bar x$ and $x\bar x$ gives $A^2-2x_0A+N(x)I_2=0$, where $I_2$ is the identity matrix. For $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ direct multiplication gives $A^2-(a+d)A+(ad-bc)I_2=0$. If $A$ is nonscalar, subtracting the two equations forces equality of the coefficients of $A$ and $I_2$, since a nonzero coefficient of $A$ in a vanishing combination would make $A$ scalar. For $A=tI_2$, the scalar-preserving isomorphism gives $x=t1$, so the determinant and reduced norm both equal $t^2$. Thus $\det\Phi_\ell(x)=N(x)$. [F2, F3]

1.2 Let $J$ be a full integral local right ideal at $\ell^e\parallel m$ and use its matrix image over $R=\mathbb Z_\ell$. The zero matrix belongs to $J$, and differences and $R$-scalar multiples of first columns are first columns of the corresponding matrix differences and scalar multiples in $J$. Thus the first columns form an $R$-submodule $L$ of $R^2$ by [F17]. They span $\mathbb Q_\ell^2$ because every column over $\mathbb Q_\ell$ can be placed first in a matrix, the matrix is in the $\mathbb Q_\ell$-span of $J$, and taking the first column is linear. Right multiplication by the matrix with a single $1$ in position $(a,b)$ moves column $a$ to position $b$ and makes the other column zero. Thus $J$ consists exactly of the matrices with both columns in $L$: both columns of a member belong to $L$, and any two vectors in $L$ can be placed separately and added. [F2, F3, F5, F17]

1.3 Evaluate the finite sums on functions on $G(\mathbb Q)\backslash G(\mathbb A_f)$ invariant under right $U(p)$. If $h'_\ell K_\ell=h_\ell K_\ell$ at $\ell\mid m$, then $h_\ell^{-1}h'_\ell\in K_\ell$ by [F4]. Thus changing the representative multiplies the output on the right by the element of $U(p)$ with that factor at $\ell$ and identity elsewhere, so the term is unchanged. Replacing an input representative on the right by $u\in U(p)$ permutes the cosets by left multiplication by $u_\ell$ at each $\ell\mid m$, by invariance of the support. Other components of $u$ commute with the representatives and can be absorbed into $U(p)$ on the right. Left multiplication of the input by a rational class also leaves each output double coset unchanged. Thus the sums descend to $X$. Enumerate the finite list of primes dividing $m$ as in [F12]. Each associated coset set is finite by [F3], so [F14] makes the product of the coset sets for any sublist finite. [F1, F3, F4, F6, F12, F14]

2.1 Take any ordered sublist of $n$ of these primes, and write $A_j$ for the local coset-sum operator and $C_j$ for its finite coset set at position $j<n$. Fix an input representative $z$ in $G(\mathbb Q)\backslash G(\mathbb A_f)$ and enumerate $C_j$ as in [F12]. For a function $u$ on $X$, write $S_r(u)$ for the sum of the first $r$ evaluations of $u$ at the double cosets of the right products of $z$ by the chosen representatives. For functions $f,g$ and scalars $a,b\in\mathbb C$, the empty sums give $S_0(af+bg)=aS_0(f)+bS_0(g)=0$ by [F15]. If $S_r(af+bg)=aS_r(f)+bS_r(g)$ and the next evaluation point is $y\in X$, then [F15] gives $S_{r+1}(af+bg)=aS_r(f)+bS_r(g)+af(y)+bg(y)=aS_{r+1}(f)+bS_{r+1}(g)$ by commutativity and distributivity. By [F19] the identity holds for the whole finite sum, so $A_j$ is complex-linear at every input coset. The identity map is linear, and a composition of linear endomorphisms is linear by applying the two linearity identities successively. Composition is associative because both groupings send $f$ to $A(B(Cf))$ for any three factors $A,B,C$. Form $P_0=\mathrm{id}$ and $P_{j+1}=P_j\circ A_j$ by [F18]. We show that $P_j f$ is the sum over choices from the first $j$ coset sets, evaluated at the right product of the associated representatives in list order. At $j=0$ there is one empty tuple by [F14], and its product is the identity, so the tuple sum equals $P_0 f$. If the expansion holds at $j<n$, apply it to $A_j f$, which is a function on $X$ by step 1.3. At the representative reached by the first $j$ choices, $A_j f$ is the sum over $C_j$ by [F4]. This gives a sum over the first $j$ choices followed by a sum over $C_j$, with terms evaluated at the right products $h_0\cdots h_j$ of the chosen representatives. Finite Fubini in [F10] combines these two sums into the sum over the tuples of length $j+1$. Apply [F19] to the property that the formula holds whenever $j\le n$. For two factors, the two orders give the same sum by reindexing with the bijection that swaps the two choices, since the two representatives commute in distinct adelic coordinates. The factors therefore commute pairwise. For the whole list, the tuple sum is exactly the combined index-$m$ correspondence. [F3, F4, F6, F10, F12, F14, F15, F18, F19, step 1.3]

2.2 Put $D_2=\{b\in R:(a,b)\in L\text{ for some }a\in R\}$ and $D_1=\{a\in R:(a,0)\in L\}$. Taking second coordinates in $L$ carries the zero vector, differences and $R$-scalar multiples to zero, differences and $R$-scalar multiples in $D_2$. For $D_1$, the same operations on vectors $(a,0)$ preserve a zero second coordinate and give the corresponding first coordinates. Thus both sets are ideals of the commutative ring $R$ by [F17]. Since $L$ spans $\mathbb Q_\ell^2$, it contains a vector $v$ with $v_2\ne0$. The scalar multiples of $v$ contain zero and are closed under addition and scalar multiplication, so they form a linear subspace by [F13]. This subspace excludes $(1,0)$. If all of $L$ lay in it, it would contain the span of $L$ by [F13], a contradiction. Hence there is $w\in L$ outside it. The vectors $v,w$ are linearly independent since a relation with nonzero coefficient of $w$ would put $w$ in that subspace, and $v\ne0$. The vector $w_2v-v_2w$ belongs to $L$ because its coefficients lie in $R$. Its second coordinate is zero and it is nonzero by independence and $v_2\ne0$. For either coordinate ideal $D$, the set $\{v_\ell(a):a\in D,\ a\ne0\}$ is a nonempty subset of the nonnegative integers. By [F9] it has a least element $t$, attained by some $a\in D$. Since $a/\ell^t$ has valuation zero, it is a unit of $R$ and hence $\ell^t\in D$. For each nonzero $z\in D$, the quotient $z/\ell^t$ has valuation $v_\ell(z)-t\ge0$ and belongs to $R$. Thus $D=\ell^tR$. Write the two coordinate ideals as $\ell^sR$ and $\ell^rR$, respectively. Choose $(b,\ell^s)\in L$. Subtracting its suitable $R$-multiple from any vector of $L$ leaves a multiple of $(\ell^r,0)$. These two generators give a matrix $A$ with $L=AR^2$ and determinant $\ell^{r+s}$. Hence $J=AM_2(R)$ and the principal local norm formula gives $r+s=e$ by step 1.1. Conversely each matrix of determinant valuation $e$ generates a full integral ideal of that norm valuation. By [F3], equality of the ideals is equivalent to equality of the projective cosets at fixed valuation. [F2, F3, F5, F9, F13, F17, step 1.1, step 1.2]

3.1 Fix a tuple of local cosets. Each coset at a prime $\ell^e\parallel m$ admits a lift in $\mathcal H_\ell$ whose split matrix has determinant valuation $e$, by [F3]. Use [F12] to select such a lift $x_\ell$ at each of these finitely many primes, and set $x_\ell=1$ elsewhere. By step 2.2, changing any lift at fixed determinant valuation leaves its local right ideal unchanged. The ideal dictionary in [F5] therefore gives a well-defined $I_x$, which is integral because each $x_\ell$ belongs to $\mathcal H_\ell$. By step 1.1, its norm exponents at $\ell\mid m$ are the prescribed determinant valuations. They are zero off these primes, so the ideal norm is $m$. Conversely a nonzero integral ideal of norm $m$ has a generator $\alpha\ne0$ by [F5], and is a full lattice because multiplication by $\alpha$ is invertible in $B$. The principal ideal norm formula in [F5] gives $N(\alpha)=m$, so $\alpha\in Q_m$. At primes not dividing $m$, both $\alpha$ and $\bar\alpha$ belong to $\mathcal H_\ell$, and $\alpha^{-1}=\bar\alpha/m$ belongs there because $m$ is a scalar unit. The ideal span is therefore $\mathcal H_\ell$ there. At the primes dividing $m$, its completed span is $\alpha\mathcal H_\ell$ with norm ideal $m\mathbb Z_\ell$, so the valuation is $e$ for $\ell^e\parallel m$. Step 2.2 and the dictionary recover exactly one tuple. Equality $\alpha\mathcal H=\alpha'\mathcal H$ places both $\alpha^{-1}\alpha'$ and its inverse in $\mathcal H$. Conversely right multiplication by a unit preserves the ideal. [F1, F2, F3, F5, F7, F12, step 1.1, step 2.2]

4.1 Let $k\in\prod_\ell K_\ell$ be the integral input and $g=r_p(k_p)$. Write $[x]$ for the projective tuple of a lift as in step 3.1. At each of the finitely many primes $\ell\mid m$, the definition of $K_\ell$ gives an integral unit lifting $k_\ell$. Use [F12] to select such a lift $b_\ell$ at each of these primes and put $x'_\ell=b_\ell x_\ell$. Under the integral splitting, $\Phi_\ell(b_\ell)$ lies in $\mathrm{GL}_2(\mathbb Z_\ell)$ because both $b_\ell$ and its inverse belong to $\mathcal H_\ell$. Apply [F4] with $A=\Phi_\ell(x_\ell)$, $U=\Phi_\ell(b_\ell)$ and $V=I_2$. Thus the split matrix of $x'_\ell$ is integral with determinant of valuation $e$. Put $x'_\ell=1$ elsewhere. Left multiplication by the $k_\ell$ permutes the local coset sets by [F4], so the fixed-valuation lifts $x'$ give each ideal of norm $m$ exactly once by step 3.1. Let $k^{(0)}$ equal $k$ away from the primes dividing $m$ and the identity at those primes. Then $k[x]=[x']k^{(0)}$. If $I_{x'}=\alpha\mathcal H$, its completed span at $\ell$ is $x'_\ell\mathcal H_\ell$ by the ideal dictionary in [F5]. Taking the span of $\alpha\mathcal H$ gives $\alpha\mathcal H_\ell$, since multiplication by $\alpha$ is linear over $\mathbb Z_\ell$. Multiplication by $\alpha^{-1}$ gives $(\alpha^{-1}x'_\ell)\mathcal H_\ell=\mathcal H_\ell$. Thus $\alpha^{-1}x'_\ell$ belongs to $\mathcal H_\ell$ and has its inverse there, by taking the preimage of $1$. Multiplication on the left by the rational class of $\alpha^{-1}$ produces the integral output $[\alpha^{-1}x']k^{(0)}$. Here $x'_p=1$ and $k^{(0)}_p=k_p$. Since $\alpha$ is a local unit at $p$ by step 3.1, the reduction of its inverse is $r_p([\alpha])^{-1}=\rho_p(\alpha)^{-1}$ by [F6]. The integral output therefore maps to $\Gamma_p\rho_p(\alpha)^{-1}g$. [F1, F2, F3, F4, F5, F6, F12, step 1.1, step 1.3, step 3.1]

5.1 Replacing $\alpha$ by $\alpha u$ for $u\in\mathcal H^\times$ multiplies $\rho_p(\alpha)^{-1}$ on the left by $\rho_p(u)^{-1}\in\Gamma_p$. Conjugation takes $\alpha u$ to $\bar u\bar\alpha$ with $\bar u=u^{-1}$, so it bijects the right-unit classes with the left-unit classes. Since $\alpha^{-1}=\bar\alpha/m$, their reduced projective classes at $p$ coincide. The left-unit classes partition $Q_m$ because the units act on it by left multiplication. In each class, $u\beta=v\beta$ forces $u=v$ by cancellation, so each class contains exactly $24$ elements. Multiplicativity gives $\rho_p(u\beta)=\rho_p(u)\rho_p(\beta)$ with $\rho_p(u)\in\Gamma_p$. Thus $f(\Gamma_p\rho_p(\beta)g)$ is constant on each left-unit class, and the ideal sum has one term per class. [F2, F4, F6, F7, step 3.1, step 4.1]

6.1 Let $\mathcal C$ be the set of left-unit classes. Enumerate the finite shell $Q_m$ of [F7] by a bijection $\iota$ from a finite initial segment of $\mathbb N$ as in [F12]. For each $C\in\mathcal C$, the indices of the elements of $C$ form a nonempty set. Let $j_C$ be its least element by [F9]. Distinct classes are disjoint by step 5.1, so $C\mapsto j_C$ bijects $\mathcal C$ with a subset of that finite initial segment. Thus $\mathcal C$ is finite by [F14], and $\beta_C=\iota(j_C)$ is a representative of $C$. The map $(C,u)\mapsto u\beta_C$ from $\mathcal C\times\mathcal H^\times$ to $Q_m$ is a bijection because the classes partition the shell and the unit action is free on each class. Reindex the shell sum by this bijection and apply finite Fubini in the additive monoid of $\mathbb C$, summing first over classes for each fixed unit. For every fixed unit $u$, the inner sum equals the ideal sum $S$ from step 5.1 because $f(\Gamma_p\rho_p(u\beta_C)g)=f(\Gamma_p\rho_p(\beta_C)g)$ for each $C$. The outer sum adds $24$ copies of $S$ by [F7] and [F15]. Starting from zero, each copy changes $nS$ to $nS+S=(n+1)S$ by distributivity in the complex field. Thus the shell sum is $24S$, and division by $24$ gives $T_m$. [F7, F9, F10, F12, F14, F15, step 5.1]

7.1 Apply step 6.1 to each prime-power index as well as to $m$. Step 2.1 now identifies the composition of the $T_{\ell^e}$ with $T_m$ and gives their pairwise commutativity. On the finite set $Y_p$ of [F11], let $e_y$ take value $1$ at $y$ and $0$ elsewhere for each $y\in Y_p$. Evaluating at each coset gives $f=\sum_{y\in Y_p} f(y)e_y$. A linear subspace containing the indicators contains their scalar multiples $f(y)e_y$ by [F13] and therefore their finite sum by repeated addition starting at zero. Thus the indicators span by [F13]. The indicators at different cosets are distinct by evaluation. In a vanishing linear combination of distinct indicators, evaluation at the coset of each indicator gives its coefficient, which is therefore zero. This proves linear independence by [F13]. The indicators form a finite basis by [F13], so the space of complex functions with the counting inner product is finite-dimensional. [F11, F13, step 2.1, step 6.1]

8.1 Let $T$ be a prime-power factor. It is complex-linear and satisfies $\langle Tf,h\rangle=\langle f,Th\rangle$ by [F7]. Thus $T$ itself satisfies the adjoint criterion in [F16]. On the finite-dimensional inner product space of step 7.1 the adjoint is unique by [F16], so $T^*=T$. Then $TT^*=T^2=T^*T$, giving normality by [F8]. The normal spectral theorem in [F8] gives an eigenbasis for each factor individually on the finite-dimensional complex inner product space of step 7.1. Thus each factor is diagonalisable over $\mathbb C$ by the one-operator definition in [F8]. The factors commute pairwise by step 7.1, so the simultaneous diagonalisation theorem in [F8] makes the family simultaneously diagonalisable on that same space. By the family definition in [F8], this yields one basis of eigenvectors common to all factors. [F7, F8, F16, step 7.1]

9.1 In the order used in step 2.1 write $T_j$ for the prime-power factors on $Y_p$. On a common eigenvector $v$, write $T_jv=\lambda_jv$. Let $B_j$ be the composition of the first $j$ factors and let $b_j$ be the product of the first $j$ scalars $\lambda_i$ under complex multiplication. By [F15] and [F18], $B_0=\mathrm{id}$, $b_0=1$, $B_{j+1}=B_j\circ T_j$ and $b_{j+1}=b_j\lambda_j$. The identity gives $B_0v=b_0v$. If $B_jv=b_jv$, linearity gives $B_{j+1}v=B_j(T_jv)=B_j(\lambda_j v)=\lambda_j b_jv=b_{j+1}v$, where the last equality uses commutativity in $\mathbb C$. By [F19] the equality holds whenever $j$ is at most the number of factors. The full composition is $T_m$ by step 7.1. For $m=1$, the indicator basis of step 7.1 is a common eigenbasis for the empty family, and the empty operator product acts by $1$. [F7, F15, F18, F19, step 2.1, step 7.1, step 8.1] ∎

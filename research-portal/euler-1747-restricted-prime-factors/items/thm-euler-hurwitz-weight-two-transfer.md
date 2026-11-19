---
id: thm-euler-hurwitz-weight-two-transfer
kind: theorem
title: Weight-two transfer for the remaining quaternionic spectrum
status: published
domain: mathematics
proof_strategy: direct
deps:
  - math:def-strongly-continuous-unitary-representation
  - math:def-hilbert-direct-sum-of-unitary-representations
  - math:thm-schurs-lemma-for-unitary-representations
  - math:thm-division-algorithm-in-z
  - math:def-axiom-of-choice
  - def-euler-prime-classes
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-author-6f52147f3ab3-hamilton-order-completions
  - def-finite-quaternion-adeles-and-projective-units
  - def-author-5b8600b4f4af-full-adelic-hamilton-group
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-adelic-level
  - math:def-radon-measure-on-an-lch-space
  - def-definite-quaternion-automorphic-fixed-space
  - lem-euler-hurwitz-adelic-identification
  - thm-projective-quaternion-discrete-spectrum
  - def-author-34e2e6a0519f-split-adelic-matrix-groups
  - def-author-34e2e6a0519f-split-cuspidal-spectrum
  - def-author-34e2e6a0519f-real-weight-two-discrete-series
  - def-author-5b8600b4f4af-split-unramified-quaternion-representation
  - thm-definite-quaternion-jacquet-langlands-weight-two
  - def-euler-hurwitz-determinant-character
  - lem-euler-hurwitz-automorphic-characters
  - thm-hurwitz-integral-splitting-at-odd-primes
  - math:def-hilbert-space
  - thm-hurwitz-order-integral-structure
  - math:def-linear-independence
  - lem-rational-hamilton-norm-and-inverse
  - math:thm-metric-sequential-closure
  - math:thm-quaternions-form-a-division-ring
formulation_deps:
  - thm-hurwitz-integral-splitting-at-odd-primes
  - math:thm-division-algorithm-in-z
  - math:def-axiom-of-choice
  - def-euler-prime-classes
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-author-6f52147f3ab3-hamilton-order-completions
  - def-finite-quaternion-adeles-and-projective-units
  - def-author-5b8600b4f4af-full-adelic-hamilton-group
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-adelic-level
  - math:def-radon-measure-on-an-lch-space
  - def-definite-quaternion-automorphic-fixed-space
  - lem-euler-hurwitz-adelic-identification
  - thm-projective-quaternion-discrete-spectrum
  - def-author-34e2e6a0519f-split-adelic-matrix-groups
  - def-author-34e2e6a0519f-split-cuspidal-spectrum
  - def-author-34e2e6a0519f-real-weight-two-discrete-series
  - def-author-5b8600b4f4af-split-unramified-quaternion-representation
  - thm-definite-quaternion-jacquet-langlands-weight-two
  - math:def-strongly-continuous-unitary-representation
  - thm-hurwitz-order-integral-structure
  - math:def-linear-independence
argument_deps:
  - math:def-strongly-continuous-unitary-representation
  - math:def-hilbert-direct-sum-of-unitary-representations
  - math:thm-schurs-lemma-for-unitary-representations
  - math:thm-division-algorithm-in-z
  - math:def-axiom-of-choice
  - def-euler-prime-classes
  - def-euler-hurwitz-adelic-level
  - def-definite-quaternion-automorphic-fixed-space
  - lem-euler-hurwitz-adelic-identification
  - thm-projective-quaternion-discrete-spectrum
  - def-euler-hurwitz-determinant-character
  - lem-euler-hurwitz-automorphic-characters
  - thm-hurwitz-integral-splitting-at-odd-primes
  - def-author-5b8600b4f4af-split-unramified-quaternion-representation
  - thm-definite-quaternion-jacquet-langlands-weight-two
  - def-author-34e2e6a0519f-split-cuspidal-spectrum
  - math:def-hilbert-space
  - thm-hurwitz-order-integral-structure
  - def-author-6f52147f3ab3-hamilton-order-completions
  - math:def-linear-independence
  - lem-rational-hamilton-norm-and-inverse
  - math:thm-metric-sequential-closure
  - def-euler-hamilton-quaternions
  - math:thm-quaternions-form-a-division-ring
dependency_roles:
  math:def-strongly-continuous-unitary-representation: mathematical-premise
  math:def-hilbert-direct-sum-of-unitary-representations: mathematical-premise
  math:thm-schurs-lemma-for-unitary-representations: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  def-author-6f52147f3ab3-hamilton-order-completions: mathematical-premise
  def-finite-quaternion-adeles-and-projective-units: mathematical-premise
  def-author-5b8600b4f4af-full-adelic-hamilton-group: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  def-euler-hurwitz-projective-reduction: mathematical-premise
  def-euler-hurwitz-adelic-level: mathematical-premise
  math:def-radon-measure-on-an-lch-space: mathematical-premise
  def-definite-quaternion-automorphic-fixed-space: mathematical-premise
  lem-euler-hurwitz-adelic-identification: mathematical-premise
  thm-projective-quaternion-discrete-spectrum: mathematical-premise
  def-author-34e2e6a0519f-split-adelic-matrix-groups: mathematical-premise
  def-author-34e2e6a0519f-split-cuspidal-spectrum: mathematical-premise
  def-author-34e2e6a0519f-real-weight-two-discrete-series: mathematical-premise
  def-author-5b8600b4f4af-split-unramified-quaternion-representation: mathematical-premise
  thm-definite-quaternion-jacquet-langlands-weight-two: mathematical-premise
  def-euler-hurwitz-determinant-character: mathematical-premise
  lem-euler-hurwitz-automorphic-characters: mathematical-premise
  thm-hurwitz-integral-splitting-at-odd-primes: mathematical-premise
  math:def-hilbert-space: mathematical-premise
  thm-hurwitz-order-integral-structure: mathematical-premise
  math:def-linear-independence: mathematical-premise
  lem-rational-hamilton-norm-and-inverse: mathematical-premise
  math:thm-metric-sequential-closure: mathematical-premise
  math:thm-quaternions-form-a-division-ring: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, proof of Lemma 3.2, paragraph on the remaining representations
      reading_limits: Read the transfer paragraph and its context on p. 3 and the
        references on p. 8. Used for attribution.
    - title: Hervé Jacquet and Robert P. Langlands, Automorphic Forms on GL(2)
      url: https://doi.org/10.1007/BFb0058988
      locator: §16, cited as [5] on p. 3 of the article
      reading_limits: Bibliographical attribution from the article. The transfer used
        here is supplied by the completed prerequisite theorem.
    - title: J. S. Ellenberg, P. Michel, and A. Venkatesh, Linnik’s ergodic method and
        the distribution of integer points on spheres
      url: https://www.math.ias.edu/~akshay/research/gg.pdf
      locator: Author manuscript, §8.4, cited as [3] on p. 3 of the article
      reading_limits: Bibliographical attribution from the article.
dependency_level: 9
---

## Statement

Assume the Axiom of Choice, that every family of nonempty sets has a choice function. Let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$. Let $B$ be the rational Hamilton quaternion algebra with basis $1,i,j,k$ and multiplication given by $i^2=j^2=-1$ and $ij=k=-ji$. Its Hurwitz order $\mathcal H$ is the subring with coordinates either all integral or all in $\mathbb Z+\tfrac12$ in this basis. The same order is the integer span of $1,i,j,(-1+i+j+k)/2$ and is maximal among the orders in $B$. For a prime $\ell$, write $B_\ell$ for $B$ with coefficients extended to the $\ell$-adic field $\mathbb Q_\ell$ and $\mathcal H_\ell$ for the $\mathbb Z_\ell$-span of $\mathcal H$ in $B_\ell$. Here $\mathbb Q_\ell$ is the completion of $\mathbb Q$ for the distance $\ell^{-v_\ell(x-y)}$ when $x\ne y$, where $v_\ell$ counts the exponent of $\ell$ in the numerator minus that in the denominator. The ring $\mathbb Z_\ell$ consists of the elements of $\ell$-adic absolute value at most one.

Write $G=PB^\times$ for the projective quaternion unit group, whose elements over a field are units of the extended algebra modulo nonzero scalars. A unit has a two-sided multiplicative inverse. Give $B_\ell^\times$ the subspace topology from the four $\ell$-adic coordinates of $B_\ell$. Use the quotient topology of $B_\ell^\times\to G(\mathbb Q_\ell)$, where nonzero local scalar multiples have the same image. Use the scalar quotient topology on $G(\mathbb R)$ from the real unit group with its Euclidean coordinate topology. Write $K_\ell$ for the image of $\mathcal H_\ell^\times$ in $G(\mathbb Q_\ell)$. The finite adelic group $G(\mathbb A_f)$ consists of tuples of local projective classes lying in $K_\ell$ at all but finitely many primes, with multiplication componentwise. Its basic open boxes have open factors in the local quotient topologies and equal $K_\ell$ at all but finitely many primes. Write $G(\mathbb A)=G(\mathbb R)\times G(\mathbb A_f)$ with the product topology. The group $G(\mathbb Q)$ maps diagonally into it by taking the class of the same rational unit at each place.

Since $p=4b+3$ for an integer $b$ and $p>1$, one has $b\ge0$ and hence $p>2$. Use the integral splitting $B_p\simeq M_2(\mathbb Q_p)$ that sends $\mathcal H_p$ onto $M_2(\mathbb Z_p)$ and is fixed for the article's reduction. Thus $K_p$ is the projective image of $\mathrm{GL}_2(\mathbb Z_p)$, the group of two-by-two matrices invertible over $\mathbb Z_p$. Let $r_p:K_p\to\mathrm{PGL}_2(\mathbb F_p)$ reduce an integral matrix representative entrywise modulo $p$ and take its class up to nonzero scalar, where $\mathbb F_p=\mathbb Z/p\mathbb Z$. The level is the subgroup $U(p)$ of tuples in $\prod_\ell K_\ell$ whose $p$-component maps to the identity under $r_p$. Write $\Gamma_p$ for the image of the global Hurwitz units under this reduction, and $Y_p=\Gamma_p\backslash\mathrm{PGL}_2(\mathbb F_p)$ for the set of cosets $\Gamma_p g$. Write $\mathbb C[Y_p]$ for the complex functions on this finite set.

Equip $X=G(\mathbb Q)\backslash G(\mathbb A)$ with the quotient topology for left multiplication by the diagonal group. Use the right translation action $R(h)f(x)=f(xh)$ on $L^2(X,\mu)$, with a nonzero finite right-invariant Radon measure $\mu$. A Radon measure here is a Borel measure finite on compact sets, outer regular on Borel sets by open supersets and inner regular on open sets by compact subsets. The square-integrable functions are taken modulo equality almost everywhere. A constituent means the representation on a nonzero closed invariant complex-linear subspace with no proper nonzero closed invariant complex-linear subspace. A constituent contributes to $\mathbb C[Y_p]$ when it has a nonzero vector fixed by $G(\mathbb R)\times U(p)$, using the identification by pullback from the finite double coset space. A local component is the factor on which the corresponding single-place group acts in the restricted tensor product of the constituent, formed with a reference vector at almost all finite places.

Each contributing constituent $\pi$ of complex dimension greater than one, meaning that its space contains two complex-linearly independent vectors, has a Jacquet–Langlands transfer $\Pi$ to an irreducible cuspidal representation of $\mathrm{PGL}_2(\mathbb A)$ of weight two. Here $\mathbb A$ is the rational adele ring, consisting of a real component and a tuple of $\ell$-adic entries integral at almost all primes. The matrix group is $L/Z$ with the quotient topology, where $L=\mathrm{GL}_2(\mathbb A)$ has the restricted-product topology using $\mathrm{GL}_2(\mathbb Z_\ell)$ at the finite places and $Z$ is the subgroup of invertible scalar matrices. Give the orbit space $X_L=(\mathrm{GL}_2(\mathbb Q)Z)\backslash L$ for left multiplication its quotient topology, embedding the rational matrices diagonally. Equip $X_L$ with a nonzero Radon measure $\nu$ invariant under right translation by $L$. Cuspidality means that $\Pi$ occurs under right translation in the closure in $L^2(X_L,\nu)$ of the continuous functions square-integrable for $\nu$ whose upper unipotent integral vanishes at every translate. For $g\in L$ this integral averages the function at the coset of $\begin{pmatrix}1&x\\0&1\end{pmatrix}g$ over $x\in\mathbb Q\backslash\mathbb A$ with translation-invariant probability measure.

Weight two means that the real factor pulled back to determinant-one real matrices is unitarily equivalent to the direct sum of the holomorphic and antiholomorphic weight-two discrete-series models. In the holomorphic model, holomorphic functions on the upper half-plane that are square-integrable for Euclidean area transform by $u(z)\mapsto(cz+d)^{-2}u((az+b)/(cz+d))$ for inverse matrix entries $a,b,c,d$ in row order. The other model uses the conjugate functions and conjugate action.

For each prime $\ell\notin\{2,p\}$ the local component $\Pi_\ell$ is unramified, meaning it has a nonzero vector fixed by the projective image of $\mathrm{GL}_2(\mathbb Z_\ell)$ in $\mathrm{PGL}_2(\mathbb Q_\ell)$. In particular this holds at every prime dividing a positive odd integer $m$ with $p\nmid m$.

## Statement references

[[math:thm-division-algorithm-in-z]]

[[math:def-axiom-of-choice]]

[[def-euler-prime-classes]]

[[def-euler-hamilton-quaternions]]

[[def-euler-hurwitz-order]]

[[thm-hurwitz-order-integral-structure]]

[[def-author-6f52147f3ab3-hamilton-order-completions]]

[[def-finite-quaternion-adeles-and-projective-units]]

[[def-author-5b8600b4f4af-full-adelic-hamilton-group]]

[[def-degree-two-projective-linear-group]]

[[def-euler-hurwitz-projective-reduction]]

[[thm-hurwitz-integral-splitting-at-odd-primes]]

[[def-euler-hurwitz-adelic-level]]

[[math:def-radon-measure-on-an-lch-space]]

[[def-definite-quaternion-automorphic-fixed-space]]

[[math:def-strongly-continuous-unitary-representation]]

[[math:def-linear-independence]]

[[lem-euler-hurwitz-adelic-identification]]

[[thm-projective-quaternion-discrete-spectrum]]

[[def-author-34e2e6a0519f-split-adelic-matrix-groups]]

[[def-author-34e2e6a0519f-split-cuspidal-spectrum]]

[[def-author-34e2e6a0519f-real-weight-two-discrete-series]]

[[def-author-5b8600b4f4af-split-unramified-quaternion-representation]]

[[thm-definite-quaternion-jacquet-langlands-weight-two]]

## Facts & Assumptions

[A1] Use the Axiom of Choice in the stated form. [[math:def-axiom-of-choice]]

[F1] The level $U(p)$ is compact open, meaning it is a compact and open subgroup in the finite adelic topology. It contains the copy of $K_\ell$ supported only at $\ell$ for every $\ell\ne p$. The finite double cosets $G(\mathbb Q)g_fU(p)$ are in bijection with $Y_p$ using integral representatives. By pullback, their function space identifies with the fixed subspace for $G(\mathbb R)\times U(p)$ in the square-integrable action. [[def-euler-hurwitz-adelic-level]] [[lem-euler-hurwitz-adelic-identification]] [[def-definite-quaternion-automorphic-fixed-space]]

[F2] For the projective group of the definite rational Hamilton division algebra, the quotient admits the stated measure. Its right translation action is strongly continuous and unitary on the complex Hilbert space $L^2$. It is the orthogonal Hilbert direct sum of its irreducible summands $M_i$, with the whole space given by their closed linear span. At a compact open finite level the fixed space is the orthogonal sum of the finitely many nonzero summand fixed spaces. A summand contributing at that level has trivial real action. Each summand has a restricted Hilbert tensor product realization with local factors. At a split prime where the level contains the supported local integral projective subgroup, the factor at that prime of each contributing summand has a nonzero vector fixed by that subgroup. [[thm-projective-quaternion-discrete-spectrum]] [[def-definite-quaternion-automorphic-fixed-space]]

[F3] A one-dimensional constituent with a fixed vector at level $U(p)$ contributes a scalar multiple of the constant function $\mathbf1$ or of $\chi_p$ on $Y_p$. The function $\chi_p$ is $1$ if the determinant of a matrix representative is a square in $\mathbb F_p^\times$ and $-1$ otherwise. [[lem-euler-hurwitz-automorphic-characters]] [[def-euler-hurwitz-determinant-character]]

[F4] For the basis $1,i,j,(-1+i+j+k)/2$ in the Statement, the natural image of the completed order $\mathcal H\otimes_{\mathbb Z}\mathbb Z_\ell$ is its $\mathbb Z_\ell$-span $\mathcal H_\ell$ in $B_\ell$. At each prime $\ell>2$ the local Hamilton algebra and local Hurwitz order are isomorphic to $M_2(\mathbb Q_\ell)$ and $M_2(\mathbb Z_\ell)$ under the same algebra isomorphism. This is a split prime, meaning the local algebra is a full matrix algebra. Its local integral projective subgroup for the unramified test is the image of $\mathrm{GL}_2(\mathbb Z_\ell)$. [[thm-hurwitz-order-integral-structure]] [[def-author-6f52147f3ab3-hamilton-order-completions]] [[thm-hurwitz-integral-splitting-at-odd-primes]] [[def-author-5b8600b4f4af-split-unramified-quaternion-representation]]

[F5] The definite quaternion transfer theorem applies to a non-one-dimensional irreducible automorphic constituent of the projective rational Hamilton group with trivial real component. It gives a cuspidal weight-two projective matrix representation. The transfer occurs under right translation in the split cuspidal space formed using the measure $\nu$ in the Statement. At a split finite place it identifies the two local representations by an invertible linear intertwiner, a map commuting with the action after identifying the two local groups via the splitting. [[thm-definite-quaternion-jacquet-langlands-weight-two]] [[def-author-34e2e6a0519f-split-cuspidal-spectrum]]

[F6] A prime is an integer greater than one whose only positive divisors are one and itself. A divisor $d$ of an integer $m$ is an integer with $m=dq$ for some integer $q$. [[def-euler-prime-classes]] Each integer $m$ has a unique expression $m=2q+r$ with $q\in\mathbb Z$ and $r\in\{0,1\}$. The remainder is $0$ exactly when $2\mid m$. An integer is odd when its remainder is $1$. [[math:thm-division-algorithm-in-z]]

[F7] In a Hilbert direct sum, vectors are square-summable families of summand coordinates, the squared norm is the sum of their squared norms, and the representation acts coordinatewise. [[math:def-hilbert-direct-sum-of-unitary-representations]]

[F8] A unitary representation acts by bijective linear isometries and is strongly continuous when every orbit map is norm-continuous. A bounded intertwiner is a bounded linear map commuting with the respective group actions. Under the Axiom of Choice, a nonzero bounded intertwiner between irreducible strongly continuous unitary representations of the same topological group on nonzero complex Hilbert spaces implies that they are unitarily equivalent. [[math:def-strongly-continuous-unitary-representation]] [[math:thm-schurs-lemma-for-unitary-representations]]

[F9] A complex Hilbert space is a complex inner-product space complete in the induced norm. [[math:def-hilbert-space]]

[F10] Two vectors $u,w$ in a complex vector space are linearly independent when $au+bw=0$ with $a,b\in\mathbb C$ implies $a=b=0$. [[math:def-linear-independence]]

[F11] The rational-coordinate Hamilton quaternions form a division algebra over $\mathbb Q$. Every nonzero element has a two-sided inverse with rational coordinates. [[lem-rational-hamilton-norm-and-inverse]]

[F12] A closed subset of a metric space contains the limit of every sequence in the subset that converges in the ambient space. [[math:thm-metric-sequential-closure]]

[F13] For the real scalar extension $B_{\mathbb R}=B\otimes_{\mathbb Q}\mathbb R$, the extended Hamilton basis has the same multiplication constants as the rational basis. [[def-author-6f52147f3ab3-hamilton-order-completions]] The real-coordinate Hamilton quaternions have this same basis multiplication table. [[def-euler-hamilton-quaternions]] Every nonzero real Hamilton quaternion has a two-sided inverse. [[math:thm-quaternions-form-a-division-ring]]

## Proof

**Given:** [A1], the stated Hamilton algebra, and the prime $p$ and level $U(p)$.

**Goal:** Transfer all contributing constituents of dimension greater than one and establish unramifiedness at the indicated primes.

1.1 The stated basis and multiplication identify $B$ with the rational-coordinate Hamilton algebra of [F11], so $B$ is a division algebra. By [F13], the real scalar extension has the same basis and multiplication table, so the map sending its four basis vectors to their real Hamilton counterparts is a bijection preserving the unit and multiplication by bilinearity. Every nonzero real Hamilton quaternion is invertible by [F13], so $B_{\mathbb R}$ is a division algebra and $B$ is definite. The level $U(p)$ is compact open by [F1]. With [A1] and the definite rational Hamilton division algebra just verified, the finite-level decomposition in [F2] applies. By the pullback in [F1], the functions on $Y_p$ correspond to the sum of the nonzero $G(\mathbb R)\times U(p)$-fixed spaces of those summands. The fixed spaces of the one-dimensional summands pull back from the lines described in [F3]. The other nonzero fixed spaces in this decomposition come from summands of dimension greater than one. [given, A1, F1, F2, F3, F11, F13]

1.2 For a nonzero complex space, choose $u\ne0$. If all vectors are multiples of $u$, the space has dimension one. Otherwise choose $w$ outside the line $\mathbb C u$. In a relation $au+bw=0$, a nonzero $b$ would give $w=-(a/b)u$. Thus $b=0$, and $u\ne0$ gives $a=0$, proving independence by [F10]. In a one-dimensional space any two nonzero vectors are proportional, and a pair containing zero is dependent by [F10]. [F10, algebra]

1.3 Let $\pi$ act on any contributing irreducible closed invariant subspace $M$ containing a complex-linearly independent pair as in the Statement. Choose a nonzero $G(\mathbb R)\times U(p)$-fixed vector $v\in M$. In the Hilbert sum of [F2], let $P_i$ be the linear map taking the $M_i$-coordinate. Some $P_i v$ is nonzero because the coordinates determine $v$. The norm formula in [F7] gives $\|P_i x\|\le\|x\|$ for every $x$ in the sum. The coordinate action in [F7] gives $P_iR(h)x=R(h)|_{M_i}P_i x$ for all $h\in G(\mathbb A)$. Thus $P_i v$ is level-fixed, so $M_i$ contributes. The restriction $P_i|_M$ is a nonzero bounded intertwiner. [given, F2, F7, F8]

2.1 Both $M$ and $M_i$ are nonzero closed subspaces of the complex Hilbert space in [F2]. Use the inherited inner products on $M$ and $M_i$. A Cauchy sequence in either induced norm converges in the ambient Hilbert space by [F2] and [F9]. In the ambient norm metric $d(x,y)=\|x-y\|$, [F12] places that limit in the closed subspace. The sequence converges there for the same norm. Thus $M$ and $M_i$ are nonzero complex Hilbert spaces. The actions on them are irreducible by the definition of $M$ and the choice of summand $M_i$. They are unitary because both subspaces are invariant under each translation and its inverse, and their orbit maps are norm-continuous by restriction from the ambient action. [given, F2, F8, F9, F12, step 1.3]

3.1 By [A1] and [F8], there is a unitary intertwiner $S:M\to M_i$. For $g\in G(\mathbb R)$ the action on $M_i$ is trivial by [F2], so $S\pi(g)=S$. Injectivity of $S$ gives trivial real action on $M$. Composing $S$ with the tensor product realization of $M_i$ gives a restricted Hilbert tensor product realization of $\pi$ with the same local factors. [A1, F2, F8, step 1.3, step 2.1]

4.1 Step 1.1 identifies the definite rational Hamilton division algebra. The constituent in step 1.3 is irreducible and, by step 1.2, its independent pair makes it non-one-dimensional. Step 3.1 gives its trivial real action. By [A1] and [F5], $\pi$ transfers to an irreducible cuspidal $\Pi$ on the projective matrix group, realized in the split cuspidal space of [F5] and having the stated real weight-two type. [A1, F5, step 1.1, step 1.2, step 1.3, step 3.1]

4.2 Fix a prime $\ell\notin\{2,p\}$. Since $\ell$ is an integer prime greater than one by [F6] and $\ell\ne2$, it satisfies $\ell>2$. Choose an integral splitting from [F4] for this prime and the completed order $\mathcal H_\ell$ in the Statement. It identifies the local Hurwitz units with $\mathrm{GL}_2(\mathbb Z_\ell)$ because an algebra isomorphism between the local orders preserves two-sided inverses. Thus their projective images correspond. The level contains the copy of $K_\ell$ supported only at $\ell$ by [F1]. By [F2], the factor of the contributing summand $M_i$ at $\ell$ has a nonzero vector fixed by the integral projective subgroup under this split identification. This factor is $\pi_\ell$ in the tensor product realization from step 3.1. [F1, F2, F4, F6, step 1.3, step 3.1]

5.1 Apply the split-place intertwiner of [F5] to that vector using the same integral splitting at $\ell$ as in step 4.2. Its image is nonzero by invertibility and is fixed by every element of the same integral projective subgroup because the map commutes with their actions. Thus $\Pi_\ell$ is unramified by the fixed-vector test in [F4]. [F4, F5, step 4.1, step 4.2]

6.1 By [F6], a positive odd $m$ has remainder $1$ on division by $2$, so $2$ does not divide $m$. Every prime dividing $m$ therefore differs from $2$. It also differs from $p$ if $p\nmid m$. Step 5.1 therefore applies at every such prime, including the vacuous case $m=1$. Step 4.1 gives the transfer and step 5.1 gives unramifiedness for each contributing constituent of dimension greater than one. [given, F6, step 4.1, step 5.1] ∎

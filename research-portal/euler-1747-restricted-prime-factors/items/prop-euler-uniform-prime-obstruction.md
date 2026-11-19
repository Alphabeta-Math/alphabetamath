---
id: prop-euler-uniform-prime-obstruction
kind: proposition
title: "Proposition 3.1: Uniform quaternionic obstruction estimate"
status: published
domain: mathematics
deps:
  - math:def-axiom-of-choice
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - def-euler-prime-classes
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - def-euler-divisor-functions
  - math:def-real-numbers
  - math:thm-of-square-roots
  - math:thm-int-ordered-ring
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
  - math:thm-division-algorithm-in-z
  - math:thm-reals-ordered-field
  - math:lem-int-embeds-rat
  - math:lem-of-q-embeds
  - math:cor-cauchy-reals-lub-complete
  - math:lem-nat-finite-sum-laws-and-the-canonical-embedding
  - lem-euler-four-square-count
  - lem-euler-obstruction-dividing-prime-density
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - lem-euler-hurwitz-odd-split-reduction
  - def-euler-hurwitz-projective-reduction
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-torus-normalizer
  - def-euler-hurwitz-normalizer-orbit
  - def-euler-hurwitz-norm-shell
  - def-euler-hurwitz-hecke-operator
  - math:def-finite-cardinality
  - lem-euler-hurwitz-sieve-domination
  - lem-euler-hurwitz-averaged-spectral-bound
  - lem-euler-hurwitz-normalizer-orbit-size
  - math:thm-complex-numbers-form-a-field
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-monoid-finite-product
  - math:thm-induction-principle
formulation_deps:
  - math:def-axiom-of-choice
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - def-euler-prime-classes
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-obstruction-count
  - def-euler-divisor-functions
  - math:def-real-numbers
  - math:thm-of-square-roots
argument_deps:
  - math:def-axiom-of-choice
  - math:def-divides-in-z
  - def-euler-prime-classes
  - math:thm-int-ordered-ring
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
  - math:thm-division-algorithm-in-z
  - math:thm-reals-ordered-field
  - math:lem-int-embeds-rat
  - math:lem-of-q-embeds
  - math:cor-cauchy-reals-lub-complete
  - math:thm-of-square-roots
  - def-euler-divisor-functions
  - math:lem-nat-finite-sum-laws-and-the-canonical-embedding
  - lem-euler-four-square-count
  - lem-euler-obstruction-dividing-prime-density
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - lem-euler-hurwitz-odd-split-reduction
  - def-euler-hurwitz-projective-reduction
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-torus-normalizer
  - def-euler-hurwitz-normalizer-orbit
  - def-euler-hurwitz-norm-shell
  - def-euler-hurwitz-hecke-operator
  - math:def-finite-cardinality
  - lem-euler-hurwitz-sieve-domination
  - lem-euler-hurwitz-averaged-spectral-bound
  - lem-euler-hurwitz-normalizer-orbit-size
  - math:thm-complex-numbers-form-a-field
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-monoid-finite-product
  - math:thm-induction-principle
dependency_roles:
  math:def-axiom-of-choice: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  def-euler-four-square-representations: mathematical-premise
  def-euler-mixed-four-square-representations: mathematical-premise
  def-euler-prime-obstruction-count: mathematical-premise
  def-euler-divisor-functions: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:thm-of-square-roots: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-of-q-embeds: mathematical-premise
  math:cor-cauchy-reals-lub-complete: mathematical-premise
  math:lem-nat-finite-sum-laws-and-the-canonical-embedding: mathematical-premise
  lem-euler-four-square-count: mathematical-premise
  lem-euler-obstruction-dividing-prime-density: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  lem-euler-hurwitz-odd-split-reduction: mathematical-premise
  def-euler-hurwitz-projective-reduction: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  def-euler-hurwitz-torus-normalizer: mathematical-premise
  def-euler-hurwitz-normalizer-orbit: mathematical-premise
  def-euler-hurwitz-norm-shell: mathematical-premise
  def-euler-hurwitz-hecke-operator: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  lem-euler-hurwitz-sieve-domination: mathematical-premise
  lem-euler-hurwitz-averaged-spectral-bound: mathematical-premise
  lem-euler-hurwitz-normalizer-orbit-size: mathematical-premise
  math:thm-complex-numbers-form-a-field: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
  math:thm-induction-principle: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, Proposition 3.1, equation (3.1), and p. 4, §3.3 and completion of
        Proposition 3.1
      reading_limits: Read the statement and the final two-case argument on PDF pages
        2 and 4 for attribution.
dependency_level: 12
---

## Statement

Assume the Axiom of Choice, which says that every family of nonempty sets has a function selecting one element from each member. Let $m$ be a positive odd integer, meaning $m>0$ and $m=2a+1$ for some integer $a$, and set $n=2m$. Write $d\mid u$ if $u=dq$ for some integer $q$, and $d\nmid u$ if no such integer exists. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Let $\mathcal P_3$ be the set of primes congruent to $3$ modulo $4$, meaning $4\mid(p-3)$ for each $p\in\mathcal P_3$. Suppose that every prime divisor of $m$ belongs to $\mathcal P_3$.

Let $R(n)$ count ordered integer quadruples $(x_1,x_2,x_3,x_4)$ for which $x_1^2+x_2^2+x_3^2+x_4^2=n$, with $x_j^2=x_j\cdot x_j$ and with both signs and zero allowed. For $p\in\mathcal P_3$, let $b_p(n)$ count the quadruples in this set that have one even and one odd entry in each of $(x_1,x_2)$ and $(x_3,x_4)$ and have both entries of at least one of these pairs divisible by $p$. Here even integers have the form $2a$, and odd integers have the form $2a+1$, for integers $a$. Count each qualifying quadruple once.

Let $\sigma(m)$ be the sum of the positive divisors of $m$ and $\tau(m)$ their number. Write $\sqrt m$ for the nonnegative real number whose square is $m$, and let $\mathbf 1_{p>3}$ be $1$ when $p>3$ and $0$ otherwise. Then $R(n)>0$, and for every $p\in\mathcal P_3$,
$$\frac{b_p(n)}{R(n)}\le \frac{2}{p(p-1)}+\mathbf 1_{p>3}\frac{\tau(m)\sqrt m}{3\sigma(m)}.$$

## Statement references

[[math:def-axiom-of-choice]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-divides-in-z]]

[[math:def-prime]]

[[math:def-congruence-modulo-an-integer]]

[[def-euler-prime-classes]]

[[def-euler-four-square-representations]]

[[def-euler-mixed-four-square-representations]]

[[def-euler-prime-obstruction-count]]

[[def-euler-divisor-functions]]

[[math:def-real-numbers]]

[[math:thm-of-square-roots]]

## Facts & Assumptions

[F1] The integers are totally ordered, with order preserved by addition and with products of positive integers positive. The natural numbers embed in the integers, preserving arithmetic and order, with image the nonnegative integers. The first natural number above $0$ is $1$. Division of an integer by a positive integer gives a unique quotient and remainder, with the remainder between $0$ inclusive and the divisor exclusive. [[math:thm-int-ordered-ring]] [[math:lem-nat-embeds-int]] [[math:lem-nat-discrete]] [[math:thm-division-algorithm-in-z]]

[F2] The real numbers form a totally ordered field. Integer counts and rational fractions are interpreted in it by the inclusions of the integers into the rationals and of the rationals into the reals, which preserve operations and order. In particular, division by a positive real number preserves an inequality. The reals have the least-upper-bound property, meaning that every nonempty set of reals bounded above has a smallest real upper bound. Thus every nonnegative real has a unique nonnegative square root. [[math:thm-reals-ordered-field]] [[math:lem-int-embeds-rat]] [[math:lem-of-q-embeds]] [[math:cor-cauchy-reals-lub-complete]] [[math:thm-of-square-roots]]

[F3] The positive divisors of $m$ form a finite set, $\sigma(m)$ adds each of them once, and $\tau(m)$ is their number. A sum of finitely many natural numbers is at least any one of its terms. [[def-euler-divisor-functions]] [[math:lem-nat-finite-sum-laws-and-the-canonical-embedding]]

[F4] For $m>0$ with $2\nmid m$, the four-square count at $n=2m$ is $R(n)=24\sigma(m)$. [[lem-euler-four-square-count]]

[F5] For $m>0$ odd, $n=2m$ and $p\in\mathcal P_3$ with $p\mid m$, one has $b_p(n)/R(n)\le 2/[p(p-1)]$. [[lem-euler-obstruction-dividing-prime-density]]

[F6] The rational Hamilton quaternions have coordinates in the basis $1,i,j,k$ with $i^2=j^2=-1$ and $ij=k=-ji$. The Hurwitz order $\mathcal H$ consists of the quaternions whose four coordinates are all integers or all integers plus $\tfrac12$. The reduced norm is the sum of their coordinate squares. For $p\in\mathcal P_3$ with $p>2$, fix one projective reduction $\rho_p$ furnished by the odd-prime splitting lemma. It sends an element of $\mathcal H$ whose norm is not divisible by $p$ to the class of its invertible two-by-two matrix obtained by reducing modulo $p$. The matrices lie over $\mathbb F_p$, the field of integer residues modulo $p$. Two integers represent the same residue when their difference is divisible by $p$. The group $G_p$ consists of all classes of invertible two-by-two matrices over $\mathbb F_p$, with matrices identified up to nonzero scalar multiples and classes multiplied on representatives. The map $\rho_p$ sends the elements with two-sided inverses in $\mathcal H$ to a subgroup $\Gamma_p$. The finite set $Y_p$ consists of their right cosets $\Gamma_pg=\{\gamma g:\gamma\in\Gamma_p\}$, for $g\in G_p$. The coset of the identity is $\Gamma_p$. [[def-euler-hamilton-quaternions]] [[def-euler-hurwitz-order]] [[lem-euler-hurwitz-odd-split-reduction]] [[def-euler-hurwitz-projective-reduction]] [[def-degree-two-projective-linear-group]] [[def-euler-hurwitz-normalizer-orbit]]

[F7] In that same reduction, let $C_p$ consist of the projective classes of the nonzero elements $a+b\bar i$ with $a,b\in\mathbb F_p$ and $\bar i$ the residue of $i$. Its normalizer is $K_p=\{g\in G_p:gC_pg^{-1}=C_p\}$, with $gC_pg^{-1}=\{gcg^{-1}:c\in C_p\}$. The normalizer orbit is the set $\mathcal O_p=\{\Gamma_pk:k\in K_p\}$. Let $u_p$ be the real indicator on $Y_p$, equal to $1$ on $\mathcal O_p$ and $0$ elsewhere. The complex indicator is $f_p=\iota\circ u_p$, where $\iota:\mathbb R\to\mathbb C$ is the injective field map sending each real number to its constant class. The orbit density is $\mu_p=|\mathcal O_p|/|Y_p|$, where $|S|$ counts the elements of a finite set $S$. For $p\nmid m$, put $Q_m=\{\alpha\in\mathcal H:\operatorname{nrd}(\alpha)=m\}$, where $\operatorname{nrd}$ denotes reduced norm. The shell is finite, and $\rho_p$ is defined at every element because $p\nmid m$. A finite sum in either field uses any enumeration of the index set without repetition. The partial sum starts at zero and adds the next term at each successor index. Let $S_{m,p}$ be the real shell average, defined by
$$S_{m,p}=\frac{1}{24}\sum_{\alpha\in Q_m}u_p(\Gamma_p\rho_p(\alpha)).$$
At the identity coset, the Hecke operator $T_m$ has the value
$$(T_m f_p)(\Gamma_p)=\frac{1}{24}\sum_{\alpha\in Q_m} f_p(\Gamma_p\rho_p(\alpha)).$$
[[def-euler-hurwitz-torus-normalizer]] [[def-euler-hurwitz-normalizer-orbit]] [[math:def-finite-cardinality]] [[def-euler-hurwitz-norm-shell]] [[def-euler-hurwitz-hecke-operator]] [[math:thm-complex-numbers-form-a-field]] [[math:def-finite-sum-in-a-commutative-monoid]] [[math:def-monoid-finite-product]]

[F8] For $m>0$ odd, $n=2m$ and $p\in\mathcal P_3$ with $p\nmid m$, the Hecke evaluation $(T_mf_p)(\Gamma_p)$ in the fixed reduction is the image of a nonnegative integer $h$, and $b_p(n)\le 8h$. [[lem-euler-hurwitz-sieve-domination]]

[F9] Under the Axiom of Choice, for $m>0$ odd and $p\in\mathcal P_3$ with $p\nmid m$, the real preimage $s$ of that same Hecke evaluation exists and satisfies $s\le\sigma(m)\mu_p+\tau(m)\sqrt m(1-\mu_p)$. [[lem-euler-hurwitz-averaged-spectral-bound]]

[F10] For $p\in\mathcal P_3$ and the fixed reduction, $\mu_p=6/[p(p-1)]$. In particular $\mu_3=1$. [[lem-euler-hurwitz-normalizer-orbit-size]]

[F11] Induction proves a property of all natural numbers from its case at zero and its passage from each number to its successor. [[math:thm-induction-principle]]

## Proof

**Given:** The Axiom of Choice, a positive odd integer $m$ whose prime divisors belong to $\mathcal P_3$, $n=2m$ and $p\in\mathcal P_3$.

**Goal:** Show $R(n)>0$ and prove the stated bound on $b_p(n)/R(n)$.

1.1 The expression $m=2a+1$ has remainder $1$ on division by $2$, so uniqueness of the remainder gives $2\nmid m$. The divisor $1$ occurs in the sum defining $\sigma(m)$ because $m=1\cdot m$, so $\sigma(m)\ge1$. Consequently $R(n)=24\sigma(m)>0$. Also $\tau(m)\ge0$ and $\sqrt m\ge0$, so $\tau(m)\sqrt m/[3\sigma(m)]\ge0$. [given, F1, F2, F3, F4]

1.2 Membership in $\mathcal P_3$ gives $p>1$ and $p=4b+3$ with $b$ an integer. If $b<0$, then $-b$ is a positive integer, hence is the image of a natural number at least $1$. This would give $p\le -4+3=-1$, contradicting $p>1$. Thus $b\ge0$ and $p\ge3$. In particular $p(p-1)>0$, and either $p=3$ or $p>3$. [given, F1, F2]

2.1 If $p\mid m$, apply [F5] to the given positive odd $m$, $n=2m$ and this prime. It gives $b_p(n)/R(n)\le2/[p(p-1)]$. The error term on the right side of the stated bound is nonnegative, being the product of $0$ or $1$ with the nonnegative quotient from step 1.1. This proves the desired inequality in this case. [given, F2, F5, step 1.1]

2.2 If $p\nmid m$, fix one reduction at the prime $p>2$ from step 1.2. Use one listing of the finite shell $Q_m$ without repetition for both sums. The empty complex partial sum is $\iota(0)=0$. If the current complex partial sum is the image of the real one, the next complex partial sum is the image of the next real one because the summands correspond by $f_p=\iota\circ u_p$ and $\iota$ preserves addition. Induction up to the length of the listing gives the same correspondence for the full sums. The real scalar $24$ is nonzero, and $\iota$ maps it to the complex scalar $24$ because it preserves $1$ and addition. The map preserves reciprocals of nonzero scalars, so dividing the sums by $24$ gives $(T_m f_p)(\Gamma_p)=\iota(S_{m,p})$. [given, F2, F6, F7, F11, step 1.2]

3.1 Form $S_{m,p}$ and $\mu_p$ using this same reduction in both [F8] and [F9]. The positive odd $m$, $n=2m$, and $p\in\mathcal P_3$ with $p\nmid m$ satisfy the hypotheses of [F8], and the given Axiom of Choice gives the remaining hypothesis of [F9]. By injectivity of $\iota$ and step 2.2, both the integer $h$ of [F8], read in the reals, and the real value $s$ of [F9] equal $S_{m,p}$. Multiplying the upper bound for $S_{m,p}$ by $8$ and dividing by $R(n)=24\sigma(m)>0$ gives
$$\frac{b_p(n)}{R(n)}\le \frac{\mu_p}{3}+\frac{\tau(m)\sqrt m}{3\sigma(m)}(1-\mu_p).$$
The factor $1/3$ comes from $8/24$. [given, F2, F4, F7, F8, F9, step 1.1, step 2.2]

4.1 Substitute $\mu_p/3=2/[p(p-1)]$ from [F10]. If $p=3$, then $1-\mu_p=0=\mathbf 1_{p>3}$. If $p>3$, then $\mu_p=6/[p(p-1)]>0$, so $1-\mu_p\le1=\mathbf 1_{p>3}$. Multiplying this comparison by the nonnegative quotient from step 1.1 gives the stated upper bound in the case $p\nmid m$. [F2, F10, step 1.1, step 1.2, step 3.1]

5.1 Each $p\in\mathcal P_3$ either divides $m$ or does not, so the two cases prove the inequality for every such $p$. Step 1.1 establishes that its left side is defined. [given, step 1.1, step 2.1, step 4.1] ∎

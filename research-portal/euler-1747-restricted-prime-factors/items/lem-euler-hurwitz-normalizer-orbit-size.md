---
id: lem-euler-hurwitz-normalizer-orbit-size
kind: lemma
title: Size and density of the normalizer orbit
status: published
domain: mathematics
proof_strategy: direct
deps:
  - def-euler-prime-classes
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-torus-normalizer
  - def-euler-hurwitz-normalizer-orbit
  - math:def-group
  - math:def-subgroup
  - math:def-coset
  - math:def-finite-cardinality
  - math:def-rationals
  - math:lem-group-inverse-laws
  - math:def-group-action
  - math:def-orbit-and-stabilizer
  - math:lem-coset-membership-and-equality
  - math:cor-orbit-stabilizer-cardinality
  - lem-euler-hurwitz-torus-normalizer-order
  - lem-euler-hurwitz-units-in-normalizer
  - lem-euler-hurwitz-quotient-size
  - math:thm-rat-field
formulation_deps:
  - def-euler-prime-classes
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-torus-normalizer
  - def-euler-hurwitz-normalizer-orbit
  - math:def-group
  - math:def-subgroup
  - math:def-coset
  - math:def-finite-cardinality
  - math:def-rationals
argument_deps:
  - def-euler-prime-classes
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-torus-normalizer
  - def-euler-hurwitz-normalizer-orbit
  - math:def-group
  - math:def-subgroup
  - math:def-coset
  - math:def-finite-cardinality
  - math:def-rationals
  - math:lem-group-inverse-laws
  - math:def-group-action
  - math:def-orbit-and-stabilizer
  - math:lem-coset-membership-and-equality
  - math:cor-orbit-stabilizer-cardinality
  - lem-euler-hurwitz-torus-normalizer-order
  - lem-euler-hurwitz-units-in-normalizer
  - lem-euler-hurwitz-quotient-size
  - math:thm-rat-field
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  def-euler-hurwitz-projective-reduction: mathematical-premise
  def-euler-hurwitz-torus-normalizer: mathematical-premise
  def-euler-hurwitz-normalizer-orbit: mathematical-premise
  math:def-group: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-rationals: mathematical-premise
  math:lem-group-inverse-laws: mathematical-premise
  math:def-group-action: mathematical-premise
  math:def-orbit-and-stabilizer: mathematical-premise
  math:lem-coset-membership-and-equality: mathematical-premise
  math:cor-orbit-stabilizer-cardinality: mathematical-premise
  lem-euler-hurwitz-torus-normalizer-order: mathematical-premise
  lem-euler-hurwitz-units-in-normalizer: mathematical-premise
  lem-euler-hurwitz-quotient-size: mathematical-premise
  math:thm-rat-field: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §3.3, density formula, orbit count, and the case p = 3
      reading_limits: Checked the orbit count and density in §3.3 on PDF page 4,
        including the specialization after (3.8), for attribution.
dependency_level: 8
---

## Statement

Let $p\in\mathcal P_3$, the set of primes congruent to $3$ modulo $4$, and use a single fixed projective reduction at $p$. Let $G_p$ be the group of classes of invertible two-by-two matrices over $\mathbb F_p$, the field of residues modulo $p$. Classes identify matrices that differ by a nonzero scalar and multiply by multiplying representatives. Let $\Gamma_p$ be the subgroup of matrix classes obtained by reducing the units of the Hurwitz order to matrices modulo $p$. A unit is an element with a two-sided inverse in the order. Let $K_p=N_{G_p}(C_p)$ be the normalizer of the torus $C_p$ in the same reduction. Here $C_p$ is the projective image of the nonzero elements of the field generated over $\mathbb F_p$ by the residue of the quaternion basis element $i$ with $i^2=-1$. Its normalizer consists of the elements $k\in G_p$ with $kC_pk^{-1}=C_p$, where $kC_pk^{-1}=\{kck^{-1}:c\in C_p\}$.

Write $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$ for the right coset represented by $g$. Let $Y_p=\{\Gamma_p g:g\in G_p\}$ and let $\mathcal O_p=\{\Gamma_p k:k\in K_p\}$ be the orbit of the base coset $\Gamma_p$ under right translation by $K_p$. With $|S|$ denoting the number of elements of a finite set $S$, the density is the rational fraction $\mu_p=|\mathcal O_p|/|Y_p|$. Then
$$|\mathcal O_p|=\frac{p+1}{2},\qquad \mu_p=\frac{6}{p(p-1)}.$$
In particular, $\mu_3=1$.

## Statement references

[[def-euler-prime-classes]]

[[def-euler-hurwitz-projective-reduction]]

[[def-euler-hurwitz-torus-normalizer]]

[[def-euler-hurwitz-normalizer-orbit]]

[[math:def-group]]

[[math:def-subgroup]]

[[math:def-coset]]

[[math:def-finite-cardinality]]

[[math:def-rationals]]

## Facts & Assumptions

[F1] A prime in $\mathcal P_3$ is greater than $1$. With the fixed reduction at such a prime, $\Gamma_p$ and $K_p$ are subgroups of the finite group $G_p$, and $Y_p$ is a nonempty finite coset set. [[def-euler-prime-classes]] [[def-euler-hurwitz-projective-reduction]] [[def-euler-hurwitz-torus-normalizer]]

[F2] The right translation $y\cdot k=\Gamma_p(gk)$ for $y=\Gamma_p g$ is a well-defined right action. This means $y\cdot e=y$ and $(y\cdot k)\cdot h=y\cdot(kh)$. The orbit consists of the translates of $\Gamma_p$, and its density is $|\mathcal O_p|/|Y_p|$. [[def-euler-hurwitz-normalizer-orbit]]

[F3] A group has associative multiplication, identity $e$ and two-sided inverses $k^{-1}$. A subgroup contains $e$ and is closed under products and inverses. Inversion satisfies $e^{-1}=e$, $(kh)^{-1}=h^{-1}k^{-1}$ and $(k^{-1})^{-1}=k$. [[math:def-group]] [[math:def-subgroup]] [[math:lem-group-inverse-laws]]

[F4] A left action is a rule $(k,y)\mapsto k\star y$ with $e\star y=y$ and $(kh)\star y=k\star(h\star y)$. The orbit of $y$ is the set of points $k\star y$, and its stabilizer is the set of elements $k$ with $k\star y=y$. [[math:def-group-action]] [[math:def-orbit-and-stabilizer]]

[F5] For a subgroup $D$ of a group, its right coset $Da$ is the set of products $da$ with $d\in D$. For group elements $a,b$, one has $Da=Db$ exactly when $ab^{-1}\in D$. [[math:def-coset]] [[math:lem-coset-membership-and-equality]]

[F6] For a finite group acting on the left, its cardinality is the product of the cardinalities of the orbit and stabilizer of any point. Cardinality of a finite set means its number of elements. [[math:cor-orbit-stabilizer-cardinality]] [[math:def-finite-cardinality]]

[F7] For the same $p$ and reduction, $|K_p|=2(p+1)$, there are four distinct classes in $\Gamma_p\cap K_p$, the set of elements common to both subgroups, and $|Y_p|=p(p^2-1)/12$. [[lem-euler-hurwitz-torus-normalizer-order]] [[lem-euler-hurwitz-units-in-normalizer]] [[lem-euler-hurwitz-quotient-size]]

[F8] A fraction of integers with nonzero denominator represents a rational number. The rational numbers form a field, so nonzero factors in fractions can be canceled. [[math:def-rationals]] [[math:thm-rat-field]]

## Proof

**Given:** $p\in\mathcal P_3$ and the fixed projective reduction at $p$.

**Goal:** Compute $|\mathcal O_p|$ and $\mu_p$, including the case $p=3$.

1.1 For $k\in K_p$ and $y\in Y_p$ set $k\star y=y\cdot k^{-1}$. Since $K_p$ is a subgroup, $k^{-1}\in K_p$, so the right action makes the rule well-defined. We have $e\star y=y\cdot e=y$. For $k,h\in K_p$, $(kh)\star y=y\cdot(h^{-1}k^{-1})=(y\cdot h^{-1})\cdot k^{-1}=k\star(h\star y)$. Thus $\star$ is a left action of $K_p$ on $Y_p$. [F1, F2, F3, F4]

2.1 Put $y_0=\Gamma_p=\Gamma_p e$. Then $k\star y_0=\Gamma_p k^{-1}$. Inversion is its own inverse on $K_p$, so these cosets as $k$ ranges over $K_p$ form exactly $\mathcal O_p$. The right coset criterion gives $\Gamma_p k^{-1}=\Gamma_p e$ exactly when $k^{-1}\in\Gamma_p$, which is equivalent to $k\in\Gamma_p$ by subgroup closure under inverses. Hence the stabilizer of $y_0$ in $K_p$ is $\Gamma_p\cap K_p$. [F1, F2, F3, F4, F5, step 1.1]

3.1 The group $K_p$ is finite and acts on the left by step 1.1. Orbit–stabilizer at $y_0$ gives $|K_p|=|\mathcal O_p|\,|\Gamma_p\cap K_p|$. The first two counts in [F7] give $4|\mathcal O_p|=2(p+1)$, so $|\mathcal O_p|=(p+1)/2$. [F1, F6, F7, F8, step 1.1, step 2.1]

4.1 Since $p>1$, the factors $p$, $p-1$ and $p+1$ are nonzero. Substituting the orbit size and the ambient coset count gives $\mu_p=\frac{(p+1)/2}{p(p^2-1)/12}=\frac{6(p+1)}{p(p-1)(p+1)}=\frac{6}{p(p-1)}$. At $p=3$ this fraction is $6/(3\cdot2)=1$, which completes the count and density calculation. [F1, F2, F7, F8, step 3.1] ∎

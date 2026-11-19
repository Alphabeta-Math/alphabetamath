---
id: lem-euler-hurwitz-orbit-determinant-balance
kind: lemma
title: The normalizer orbit is balanced between determinant classes
status: published
domain: mathematics
proof_strategy: direct
deps:
  - def-euler-prime-classes
  - def-euler-hurwitz-torus-normalizer
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-order
  - def-euler-hamilton-quaternions
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-normalizer-orbit
  - def-euler-hurwitz-determinant-character
  - math:def-field-norm-and-trace
  - math:def-determinant-of-a-square-matrix
  - math:def-legendre-symbol
  - math:def-coset
  - math:def-finite-cardinality
  - math:def-subgroup
  - lem-euler-hurwitz-determinant-character-well-defined
  - lem-quadratic-finite-field-norm-surjectivity
  - lem-euler-hurwitz-odd-split-reduction
  - lem-projective-determinant-square-class
  - lem-coset-character-balance
  - math:def-determinant-of-a-linear-operator
  - math:def-coordinate-column-and-matrix-of-a-linear-map
  - lem-degree-two-projective-group-cardinality
  - math:thm-standard-representatives-modulo-n
  - math:def-dimension
formulation_deps:
  - def-euler-prime-classes
  - def-euler-hurwitz-torus-normalizer
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-order
  - def-euler-hamilton-quaternions
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-normalizer-orbit
  - def-euler-hurwitz-determinant-character
  - math:def-field-norm-and-trace
  - math:def-determinant-of-a-square-matrix
  - math:def-legendre-symbol
  - math:def-coset
  - math:def-finite-cardinality
  - math:def-subgroup
  - lem-euler-hurwitz-determinant-character-well-defined
  - math:def-determinant-of-a-linear-operator
argument_deps:
  - def-euler-prime-classes
  - def-euler-hurwitz-torus-normalizer
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-order
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-normalizer-orbit
  - def-euler-hurwitz-determinant-character
  - math:def-field-norm-and-trace
  - math:def-determinant-of-a-square-matrix
  - math:def-legendre-symbol
  - math:def-coset
  - math:def-finite-cardinality
  - math:def-subgroup
  - lem-quadratic-finite-field-norm-surjectivity
  - lem-euler-hurwitz-odd-split-reduction
  - lem-euler-hurwitz-determinant-character-well-defined
  - lem-projective-determinant-square-class
  - lem-coset-character-balance
  - math:def-determinant-of-a-linear-operator
  - math:def-coordinate-column-and-matrix-of-a-linear-map
  - lem-degree-two-projective-group-cardinality
  - math:thm-standard-representatives-modulo-n
  - math:def-dimension
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  def-euler-hurwitz-torus-normalizer: mathematical-premise
  def-euler-hurwitz-projective-reduction: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  def-euler-hurwitz-normalizer-orbit: mathematical-premise
  def-euler-hurwitz-determinant-character: mathematical-premise
  math:def-field-norm-and-trace: mathematical-premise
  math:def-determinant-of-a-square-matrix: mathematical-premise
  math:def-legendre-symbol: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-subgroup: mathematical-premise
  lem-euler-hurwitz-determinant-character-well-defined: mathematical-premise
  lem-quadratic-finite-field-norm-surjectivity: mathematical-premise
  lem-euler-hurwitz-odd-split-reduction: mathematical-premise
  lem-projective-determinant-square-class: mathematical-premise
  lem-coset-character-balance: mathematical-premise
  math:def-determinant-of-a-linear-operator: mathematical-premise
  math:def-coordinate-column-and-matrix-of-a-linear-map: mathematical-premise
  lem-degree-two-projective-group-cardinality: mathematical-premise
  math:thm-standard-representatives-modulo-n: mathematical-premise
  math:def-dimension: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §3.3, norm surjectivity and balance paragraph following (3.7)
dependency_level: 7
---

## Statement

Let $p\in\mathcal P_3$, where $\mathcal P_3$ is the set of primes congruent to $3$ modulo $4$. Let $\mathbb F_p=\mathbb Z/p\mathbb Z$ be the field of integer residues modulo $p$. For a field $F$, let $F^\times$ denote its nonzero elements under multiplication.

The Hurwitz order $\mathcal H$ consists of rational quaternions $a+bi+cj+dk$ with coordinates either all integral or all in $\mathbb Z+\tfrac12$, with $i^2=j^2=-1$ and $k=ij=-ji$. Use the fixed matrix identification $\bar\Phi_p:\mathcal H/p\mathcal H\to M_2(\mathbb F_p)$, where $M_2(\mathbb F_p)$ is the algebra of two-by-two matrices over $\mathbb F_p$. In $\mathcal H/p\mathcal H$ two elements of $\mathcal H$ represent the same residue if their difference is $p$ times an element of $\mathcal H$. Write $\bar i$ for the residue of $i$. The field $E_p=\{a+b\bar i:a,b\in\mathbb F_p\}$ in this quotient has $p^2$ elements and is the model for $\mathbb F_{p^2}$. Its field norm $N:E_p^\times\to\mathbb F_p^\times$ is the determinant of multiplication by $z$ on $E_p$, the map $m_z:x\mapsto zx$ that preserves addition and multiplication by scalars from $\mathbb F_p$.

The group $G_p=\mathrm{PGL}_2(\mathbb F_p)$ consists of classes $[A]$ of matrices having a two-sided inverse, with matrices identified up to nonzero scalar multiples and product $[A][B]=[AB]$. Let $\Gamma_p$ be the subgroup of projective classes of reductions of units of $\mathcal H$, the elements with two-sided inverses in $\mathcal H$. The subgroup $C_p=\{[\bar\Phi_p(z)]:z\in E_p^\times\}$ is the nonsplit torus, the projective image of the nonzero elements of $E_p$. Its normalizer $K_p$ is the subgroup of elements $k\in G_p$ for which $\{kck^{-1}:c\in C_p\}=C_p$. Set $Y_p=\{\Gamma_p g:g\in G_p\}$, where the right coset $\Gamma_p g$ is $\{\gamma g:\gamma\in\Gamma_p\}$. Set $\mathcal O_p=\{\Gamma_p k:k\in K_p\}$, the orbit of the identity coset $\Gamma_p$ under right multiplication by elements of $K_p$.

For a nonzero residue $x$, the Legendre sign $\lambda_p(x)$ is $1$ if $x$ is a square of a nonzero residue and $-1$ otherwise. Let $\chi_p(\Gamma_p[A])=\lambda_p(\det A)$ be the determinant sign of a coset, where $\det A=ad-bc$ for a matrix with rows $(a,b)$ and $(c,d)$. The two determinant square classes on $Y_p$ are the cosets with sign $1$ and those with sign $-1$.

Then $N$ is surjective, meaning that every element of $\mathbb F_p^\times$ occurs as a norm. For each $S\in\{\mathcal O_p,Y_p\}$, the classes have equal cardinality, where $|U|$ denotes the number of elements of a finite set $U$.

$$|\{y\in S:\chi_p(y)=1\}|=|\{y\in S:\chi_p(y)=-1\}|.$$

## Facts & Assumptions

[F1] The prime $p\in\mathcal P_3$ has the form $4r+3$ for an integer $r$, so it is odd. In the torus construction $E_p$ is a field containing $\mathbb F_p$ with ordered basis $(1,\bar i)$ over $\mathbb F_p$. The dimension of a finite-dimensional vector space is the number of elements in a basis. Every element has unique coordinates in this pair and $\bar i^2=-1$. Also $C_p\subseteq K_p$, and $K_p$ is a subgroup of $G_p$. [[def-euler-prime-classes]] [[def-euler-hurwitz-torus-normalizer]] [[math:def-dimension]]

[F2] The Hurwitz order contains all quaternions with integral coordinates. In the fixed projective reduction, $\bar\Phi_p$ preserves addition, multiplication, identity and scalar multiplication. For $\alpha\in\mathcal H$ with coordinates $(a,b,c,d)$, the determinant of $\bar\Phi_p(\alpha+p\mathcal H)$ is the residue of the reduced norm $a^2+b^2+c^2+d^2$. [[def-euler-hurwitz-order]] [[def-euler-hurwitz-projective-reduction]] [[lem-euler-hurwitz-odd-split-reduction]]

[F3] In a quadratic extension of a finite field, the field norm is the determinant of the operator of multiplication, and it maps the nonzero elements onto the nonzero elements of the base field. In a chosen ordered basis, the operator determinant is the determinant of its coordinate matrix. The matrix columns are the coordinates of the images of the basis vectors. A two-by-two matrix with rows $(a,b)$ and $(c,d)$ has determinant $ad-bc$. [[math:def-field-norm-and-trace]] [[lem-quadratic-finite-field-norm-surjectivity]] [[math:def-determinant-of-a-linear-operator]] [[math:def-coordinate-column-and-matrix-of-a-linear-map]] [[math:def-determinant-of-a-square-matrix]]

[F4] Over $\mathbb F_p$ for odd prime $p$, the Legendre sign on a nonzero residue is $1$ on squares and $-1$ on nonsquares. The map $\varepsilon_p:G_p\to\{1,-1\}$ defined by $\varepsilon_p([A])=\lambda_p(\det A)$ is a group homomorphism, meaning it preserves products of group elements, and takes both signs. Every representative of an element of $\Gamma_p$ has square determinant, and $\chi_p(\Gamma_p g)=\varepsilon_p(g)$ is independent of the representative. [[math:def-legendre-symbol]] [[lem-projective-determinant-square-class]] [[def-euler-hurwitz-determinant-character]] [[lem-euler-hurwitz-determinant-character-well-defined]]

[F5] Since $p\ge 1$, each class in $\mathbb Z/p\mathbb Z$ has exactly one representative in $0,\ldots,p-1$. Thus $|\mathbb F_p|=p$. The elements of $G_p$ are classes of invertible two-by-two matrices over $\mathbb F_p$. Over a field of $p$ elements this projective group has $p(p^2-1)$ elements, so $G_p$ is finite. The subgroup $\Gamma_p$ is the image of the Hurwitz units under projective reduction. A subgroup contains the group identity and is closed under products and inverses. The coset set is $Y_p=\{\Gamma_p g:g\in G_p\}$ with $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$, and its right $K_p$-orbit of the base coset is $\mathcal O_p=\{\Gamma_p k:k\in K_p\}$. [[def-degree-two-projective-linear-group]] [[def-euler-hurwitz-projective-reduction]] [[math:def-subgroup]] [[math:def-coset]] [[def-euler-hurwitz-normalizer-orbit]] [[lem-degree-two-projective-group-cardinality]] [[math:thm-standard-representatives-modulo-n]]

[F6] For a finite group $G$ and subgroups $H,K$, let $\varepsilon:G\to\{1,-1\}$ preserve products, take the value $1$ on $H$, and take both signs on $K$. The sign of a right coset $Hg$ is then $\varepsilon(g)$. On both the full right coset set and the orbit $\{Hk:k\in K\}$, right multiplication by an element $t\in K$ of sign $-1$ pairs the two signs. A bijection, meaning a map with a two-sided inverse, between finite sets gives equal cardinalities. [[lem-coset-character-balance]] [[math:def-finite-cardinality]]

## Proof

**Given:** $p\in\mathcal P_3$ with the fixed projective reduction and the field $E_p$ in the statement.

**Goal:** Prove surjectivity of $N$ and equality of the two determinant sign counts on $\mathcal O_p$ and $Y_p$.

1.1 By [F1], the basis $(1,\bar i)$ has two elements, so $\dim_{\mathbb F_p}E_p=2$. Thus $E_p/\mathbb F_p$ is quadratic. By [F5], $\mathbb F_p$ is finite. Thus [F3] gives surjectivity of $N:E_p^\times\to\mathbb F_p^\times$. [given, F1, F3, F5]

1.2 Let $z=a+b\bar i\in E_p^\times$. Multiplication by $z$ sends $1$ to $a+b\bar i$ and $\bar i$ to $-b+a\bar i$, so the coordinate matrix in the ordered basis $(1,\bar i)$ has rows $(a,-b)$ and $(b,a)$. Thus $N(z)=a^2+b^2$. Use [F5] to choose the integer representatives $a_0,b_0$ of $a,b$ in $0,\ldots,p-1$, so $\alpha=a_0+b_0i\in\mathcal H$ represents $z$. The fixed reduction has $\det\bar\Phi_p(z)=(a_0^2+b_0^2)\bmod p=a^2+b^2=N(z)$. [F1, F2, F3, F5]

2.1 Since $\varepsilon_p$ takes the value $-1$ in [F4], some nonzero residue $d$ has $\lambda_p(d)=-1$. Choose $z\in E_p^\times$ with $N(z)=d$ by step 1.1. The inverse $z^{-1}$ lies in $E_p$, and [F2] gives $\bar\Phi_p(z^{-1})$ as the two-sided inverse of $\bar\Phi_p(z)$. By the definition of $C_p$, $t=[\bar\Phi_p(z)]$ belongs to $C_p\subseteq K_p$. Step 1.2 gives $\varepsilon_p(t)=\lambda_p(d)=-1$. The identity of $G_p$ belongs to $K_p$ and has sign $1$ because its identity matrix has determinant $1=1^2$. Thus $\varepsilon_p$ takes both signs on $K_p$. [F1, F2, F3, F4, F5, step 1.1, step 1.2]

3.1 By [F5], $\mathbb F_p$ has $p$ elements, so the projective group count gives $|G_p|=p(p^2-1)$. The groups $\Gamma_p$ and $K_p$ are subgroups, and $\varepsilon_p$ is $1$ on $\Gamma_p$ by the square-determinant property. Together with step 2.1 this gives all the hypotheses of [F6], with $G=G_p$, $H=\Gamma_p$, $K=K_p$ and $\varepsilon=\varepsilon_p$. [F1, F4, F5, F6, step 2.1]

4.1 By [F6], right multiplication by $t$ gives the sign-exchanging bijection on each of the sets in [F5]. In fact $\chi_p(\Gamma_p(gt))=\varepsilon_p(g)\varepsilon_p(t)=-\chi_p(\Gamma_p g)$, and translation by $t^{-1}$ is the inverse and preserves both sets. Hence the two sign classes have equal cardinality on $\mathcal O_p$ and on $Y_p$. Together with step 1.1 this proves the statement. [F4, F5, F6, step 1.1, step 2.1, step 3.1] ∎

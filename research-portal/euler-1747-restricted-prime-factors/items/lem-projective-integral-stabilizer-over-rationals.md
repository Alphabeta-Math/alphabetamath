---
id: lem-projective-integral-stabilizer-over-rationals
kind: lemma
title: Projective integral stabilizer over the rationals
status: published
domain: mathematics
deps:
  - def-author-6f52147f3ab3-hamilton-order-completions
  - def-author-24fda87362bc-local-adic-valuation
  - def-finite-quaternion-adeles-and-projective-units
  - math:thm-fundamental-theorem-of-arithmetic
  - lem-author-f5ba73d33e6e-reconstructing-quaternion-lattices
formulation_deps:
  - def-author-6f52147f3ab3-hamilton-order-completions
  - def-author-24fda87362bc-local-adic-valuation
  - def-finite-quaternion-adeles-and-projective-units
  - math:thm-fundamental-theorem-of-arithmetic
argument_deps:
  - def-author-6f52147f3ab3-hamilton-order-completions
  - def-author-24fda87362bc-local-adic-valuation
  - def-finite-quaternion-adeles-and-projective-units
  - math:thm-fundamental-theorem-of-arithmetic
  - lem-author-f5ba73d33e6e-reconstructing-quaternion-lattices
dependency_roles:
  def-author-6f52147f3ab3-hamilton-order-completions: mathematical-premise
  def-author-24fda87362bc-local-adic-valuation: mathematical-premise
  def-finite-quaternion-adeles-and-projective-units: mathematical-premise
  math:thm-fundamental-theorem-of-arithmetic: mathematical-premise
  lem-author-f5ba73d33e6e-reconstructing-quaternion-lattices: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 4
---

## Statement

Let $B$ be the rational Hamilton quaternion algebra, with basis $1,i,j,k$, identity $1$, and products determined by $i^2=j^2=k^2=-1$, $ij=k=-ji$, $jk=i=-kj$, and $ki=j=-ik$. Let $O$ be an order in $B$, meaning a subring containing $1$ that is the integer span of a rational basis of $B$. For each prime $\ell$, a positive integer greater than $1$ whose only positive divisors are $1$ and itself, let $\mathbb Q_\ell$ be the completion of $\mathbb Q$ for the $\ell$-adic absolute value $|\cdot|_\ell$, which assigns $\ell^{-m}$ to a nonzero rational with net exponent $m$ of $\ell$ in its prime factorization. Let $\mathbb Z_\ell$ be the subring of elements $t\in\mathbb Q_\ell$ with $|t|_\ell\le 1$. Write $B_\ell$ for the same quaternion algebra with coefficients in $\mathbb Q_\ell$ and $O_\ell$ for the span of $O$ over $\mathbb Z_\ell$ inside $B_\ell$. The superscript $\times$ denotes elements with a two-sided multiplicative inverse in the indicated ring.

Write $G(\mathbb Q)=B^\times/\mathbb Q^\times$ and $G(\mathbb Q_\ell)=B_\ell^\times/\mathbb Q_\ell^\times$. These are projective groups: two units represent the same class if one is obtained from the other by multiplication by a nonzero scalar in the indicated field, and classes multiply by multiplying representatives. Let $K_\ell$ be the image of $O_\ell^\times$ in $G(\mathbb Q_\ell)$. The finite adelic projective group $G(\mathbb A_f)$ is identified with the families in $\prod_\ell G(\mathbb Q_\ell)$ whose coordinates lie in $K_\ell$ for all but finitely many $\ell$, with componentwise multiplication. View $G(\mathbb Q)$ inside this group by sending each rational class to its local classes.

If $[x]\in G(\mathbb Q)$ has an integral-unit representative at every prime, meaning its local class belongs to $K_\ell$ for every $\ell$, then there is a positive rational $r$ such that $rx\in O^\times$. Equivalently, inside $G(\mathbb A_f)$,
$$G(\mathbb Q)\cap\prod_\ell K_\ell=\operatorname{im}\bigl(O^\times\to G(\mathbb Q)\bigr).$$

## Statement references

[[def-author-6f52147f3ab3-hamilton-order-completions]]

[[def-author-24fda87362bc-local-adic-valuation]]

[[def-finite-quaternion-adeles-and-projective-units]]

[[math:thm-fundamental-theorem-of-arithmetic]]

## Facts & Assumptions

[F1] In an order basis, $O_\ell$ consists of the vectors with all coefficients in $\mathbb Z_\ell$. A scalar quaternion $a1$ with $a\in\mathbb Q_\ell^\times$ belongs to $O_\ell^\times$ exactly when $a\in\mathbb Z_\ell^\times$ ([[def-author-6f52147f3ab3-hamilton-order-completions]]).

[F2] The rational projective group embeds in the finite adelic projective group by its family of local classes, and the image of the product of integral unit groups is $\prod_\ell K_\ell$ ([[def-finite-quaternion-adeles-and-projective-units]]).

[F3] The normalized valuation $v_\ell(t)$ of a nonzero $t\in\mathbb Q_\ell$ is the integer determined by $|t|_\ell=\ell^{-v_\ell(t)}$. It satisfies $v_\ell(st)=v_\ell(s)+v_\ell(t)$ for nonzero factors, equals the net prime exponent on nonzero rationals, and vanishes exactly on $\mathbb Z_\ell^\times$ ([[def-author-24fda87362bc-local-adic-valuation]]).

[F4] Every positive integer factors into finitely many primes, with the factorization unique up to order ([[math:thm-fundamental-theorem-of-arithmetic]]).

[F5] For any full integral lattice $L$ in $B$, meaning the integer span of a rational basis, its completed spans $L_\ell$ determine it by $L=\{y\in B:y\in L_\ell\text{ for every prime }\ell\}$ ([[lem-author-f5ba73d33e6e-reconstructing-quaternion-lattices]]).

## Proof

**Given:** $O$ as above and $x\in B^\times$ whose local class is in $K_\ell$ for every prime $\ell$.

**Goal:** Construct a positive rational $r$ with $rx\in O^\times$ and prove the intersection formula.

1.1 At any prime $\ell$, local class membership gives a scalar $a\in\mathbb Q_\ell^\times$ with $ax\in O_\ell^\times$. If $b\in\mathbb Q_\ell^\times$ is another such scalar, then $(ax)(bx)^{-1}=(a/b)1$ lies in $O_\ell^\times$. Thus $a/b\in\mathbb Z_\ell^\times$ and $v_\ell(a)=v_\ell(b)$. Write $n_\ell$ for this common integer. [given, F1, F2, F3]

2.1 Write $x$ and $x^{-1}$ in the rational basis of $B$ whose integer span is $O$. The positive denominators of these finitely many rational coefficients have only finitely many prime divisors. At any prime $\ell$ outside this finite set, each nonzero coefficient has nonnegative valuation because its denominator has exponent zero, and every zero coefficient lies in $\mathbb Z_\ell$ as well. Therefore $x$ and $x^{-1}$ both belong to $O_\ell$, so $x\in O_\ell^\times$. The scalar $1$ is then allowed in step 1.1 and gives $n_\ell=0$. [F1, F3, F4, step 1.1]

3.1 Let $S=\{\ell:n_\ell\ne0\}$ and put $r=\prod_{\ell\in S}\ell^{n_\ell}$, with empty product $1$ and negative exponents giving reciprocal powers. This is a positive rational by finiteness of $S$. For every prime $\ell$ its net exponent satisfies $v_\ell(r)=n_\ell$, since a prime power at any other prime contributes zero. At a fixed $\ell$ take any scalar $a$ allowed in step 1.1. Then $v_\ell(r/a)=0$, so $(r/a)1\in O_\ell^\times$. Consequently $rx=(r/a)(ax)\in O_\ell^\times$. This holds for every prime. [F1, F3, F4, step 1.1, step 2.1]

4.1 Since $rx$ is a unit in each $O_\ell$, both $rx$ and its rational inverse belong to every $O_\ell$. Apply the lattice intersection formula with $L=O$ to each of these rational elements to obtain $rx,(rx)^{-1}\in O$. Thus $rx\in O^\times$ and has rational projective class $[x]$. Conversely, a unit of $O$ and its inverse map into every $O_\ell$, since integer coefficients are also $\ell$-adic integers. Its local classes therefore lie in all $K_\ell$, and its rational class belongs to the intersection. This proves the formula. [F1, F2, F5, step 3.1] ∎

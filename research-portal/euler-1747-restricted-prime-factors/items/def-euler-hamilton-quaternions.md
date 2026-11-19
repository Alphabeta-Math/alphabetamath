---
id: def-euler-hamilton-quaternions
kind: definition
title: The Hamilton quaternion algebra and reduced norm
status: draft
domain: mathematics
deps:
  - math:def-rationals
  - math:def-rat-operations
  - math:thm-rat-field
  - math:def-real-numbers
  - math:lem-rat-embeds-dense
  - math:def-quaternions
  - math:def-ring
  - math:def-ring-homomorphism
  - math:def-algebra-over-a-commutative-ring
  - lem-rational-hamilton-norm-and-inverse
formulation_deps:
  - math:def-rationals
  - math:def-rat-operations
  - math:thm-rat-field
  - math:def-real-numbers
  - math:lem-rat-embeds-dense
  - math:def-quaternions
  - math:def-ring
  - math:def-ring-homomorphism
  - math:def-algebra-over-a-commutative-ring
argument_deps:
  - math:def-rationals
  - math:def-rat-operations
  - math:thm-rat-field
  - math:def-real-numbers
  - math:lem-rat-embeds-dense
  - math:def-quaternions
  - math:def-ring
  - math:def-ring-homomorphism
  - math:def-algebra-over-a-commutative-ring
  - lem-rational-hamilton-norm-and-inverse
dependency_roles:
  math:def-rationals: mathematical-premise
  math:def-rat-operations: mathematical-premise
  math:thm-rat-field: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:def-quaternions: mathematical-premise
  math:def-ring: mathematical-premise
  math:def-ring-homomorphism: mathematical-premise
  math:def-algebra-over-a-commutative-ring: mathematical-premise
  lem-rational-hamilton-norm-and-inverse: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §3.1, Hamilton algebra and reduced norm
dependency_level: 1
---

## Definition

Let $\mathbb Q$ be the field of rational numbers, viewed in the real numbers $\mathbb R$ by sending each rational to the real number represented by its constant sequence. The **rational Hamilton quaternion algebra** $B$ consists of the quadruples in the real Hamilton quaternions $\mathbb H=\mathbb R^4$ whose coordinates all lie in $\mathbb Q$. It has coordinatewise addition and the inherited Hamilton product.

Write $1=(1,0,0,0)$, $i=(0,1,0,0)$, $j=(0,0,1,0)$ and $k=(0,0,0,1)$. Then $B=\mathbb Q+\mathbb Qi+\mathbb Qj+\mathbb Qk$, where each quadruple $(a,b,c,d)$ has a unique expression $a+bi+cj+dk$. The scalar $t\in\mathbb Q$ acts by multiplication by $t1=(t,0,0,0)$, which commutes with every element of $B$. This scalar map preserves addition, multiplication and $1$, as required for a $\mathbb Q$-algebra. To multiply two expressions, distribute and take rational scalars outside the products. The multiplication rules are $1x=x1=x$, $i^2=j^2=k^2=-1$, $ij=k=-ji$, $jk=i=-kj$ and $ki=j=-ik$.

For $x=a+bi+cj+dk\in B$, the **quaternion conjugate** is $\bar x=a-bi-cj-dk$. The **reduced norm** on $B$ is the rational-valued function $\operatorname{nrd}(x)=a^2+b^2+c^2+d^2$.

## Facts & Assumptions

[F1] Rationals are classes of integer pairs $(m,n)$ with $n\ne0$, with $(m,n)$ and $(r,s)$ equivalent when $ms=rn$ ([[math:def-rationals|Rational numbers]]). Their arithmetic is given by [[math:def-rat-operations|rational operations]]. In particular, addition, multiplication and additive inverses stay in $\mathbb Q$ ([[math:thm-rat-field|Rational field]]).

[F2] Sending a rational to the class of its constant sequence defines its real image ([[math:def-real-numbers|Real numbers]]). This map is injective and preserves addition, multiplication, $0$ and $1$ ([[math:lem-rat-embeds-dense|Embedding of the rationals]]).

[F3] The real Hamilton quaternions are real quadruples with coordinatewise addition and a product whose coordinates are sums and differences of coordinate products. The product formula gives the displayed multiplication rules for $1,i,j,k$ and the coordinate scaling $(t,0,0,0)x=x(t,0,0,0)=(ta,tb,tc,td)$ for $x=(a,b,c,d)$ ([[math:def-quaternions|Real Hamilton quaternions]]).

[F4] For the rational-coordinate subset of these real quaternions under the embedding in [F2], the inherited operations make it a $\mathbb Q$-algebra with scalar map $t\mapsto(t,0,0,0)$. On that subset, the coordinate conjugate negates the last three entries and satisfies $x\bar x=\bar x x=(a^2+b^2+c^2+d^2,0,0,0)$ for $x=(a,b,c,d)$ ([[lem-rational-hamilton-norm-and-inverse|Norm and conjugation on rational Hamilton quaternions]]).

[F5] A ring has associative, commutative addition with zero and additive inverses, associative multiplication with identity, and both distributive laws ([[math:def-ring|Ring]]). A unital ring homomorphism preserves addition, multiplication and $1$ ([[math:def-ring-homomorphism|Ring homomorphism]]). A $\mathbb Q$-algebra is a ring equipped with such a map from $\mathbb Q$ whose values commute with all elements of the ring ([[math:def-algebra-over-a-commutative-ring|Algebra over a commutative ring]]).

## Justification

The rational embedding in [F2] identifies $B$ with the subset in [F4]. Its inherited operations and scalar map satisfy the algebra conditions in [F5] by [F4]. Negating rational coordinates or taking the sum of their squares gives rational values by [F1]. The coordinate expansion verified below therefore defines conjugation and reduced norm on all of $B$.

## Proof

**Given:** The rational-coordinate subset $B$ of $\mathbb H$ and an arbitrary $x=(a,b,c,d)\in B$.

**Goal:** Verify the coordinate presentation of the algebra and its norm identity.

1.1 The scalar action in [F3] makes the sum $a1+bi+cj+dk$ equal to the quadruple $(a,b,c,d)$. Equality of quadruples is equality in each coordinate, and the embedding is injective, so the rational coefficients are unique. The table in [F3] and the distributive laws in [F5] therefore compute the inherited product on these expressions. [F2, F3, F5]

2.1 By step 1.1, the expression $a-bi-cj-dk$ has coordinates $(a,-b,-c,-d)$, so it is the conjugate in [F4]. By [F4], both $x\bar x$ and $\bar x x$ equal $\operatorname{nrd}(x)1$. Since $t1=(t,0,0,0)$ and the rational embedding in [F2] is injective, there is a unique rational scalar in this identity. This gives the stated norm identity in the coordinate presentation of $B$. [F2, F4, step 1.1] ∎

---
id: lem-author-eebeda62e446-projective-norm-one-commutator
kind: lemma
title: Projective classes of square-norm quaternions are commutators
status: published
domain: mathematics
deps:
  - math:def-field
  - math:def-subfield
  - math:def-algebra-over-a-commutative-ring
  - def-author-6f52147f3ab3-hamilton-order-completions
  - math:def-subgroup
  - math:def-normal-subgroup
  - math:def-quotient-group
  - math:thm-quotient-group-laws
  - math:def-group
  - math:def-group-homomorphism
  - math:lem-group-homomorphism-basic-properties
  - math:def-coset
  - math:def-ring-homomorphism
  - math:lem-field-is-a-commutative-ring
  - math:def-ring
  - math:def-commutative-ring
formulation_deps:
  - math:def-field
  - math:def-subfield
  - def-author-6f52147f3ab3-hamilton-order-completions
  - math:def-subgroup
  - math:def-normal-subgroup
  - math:def-quotient-group
  - math:def-group
  - math:def-group-homomorphism
  - math:def-coset
argument_deps:
  - math:def-field
  - math:def-subfield
  - math:def-algebra-over-a-commutative-ring
  - def-author-6f52147f3ab3-hamilton-order-completions
  - math:def-subgroup
  - math:def-normal-subgroup
  - math:def-quotient-group
  - math:thm-quotient-group-laws
  - math:def-group
  - math:def-group-homomorphism
  - math:lem-group-homomorphism-basic-properties
  - math:def-coset
  - math:def-ring-homomorphism
  - math:lem-field-is-a-commutative-ring
  - math:def-ring
  - math:def-commutative-ring
dependency_roles:
  math:def-field: mathematical-premise
  math:def-subfield: mathematical-premise
  math:def-algebra-over-a-commutative-ring: mathematical-premise
  def-author-6f52147f3ab3-hamilton-order-completions: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:def-normal-subgroup: mathematical-premise
  math:def-quotient-group: mathematical-premise
  math:thm-quotient-group-laws: mathematical-premise
  math:def-group: mathematical-premise
  math:def-group-homomorphism: mathematical-premise
  math:lem-group-homomorphism-basic-properties: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-ring-homomorphism: mathematical-premise
  math:lem-field-is-a-commutative-ring: mathematical-premise
  math:def-ring: mathematical-premise
  math:def-commutative-ring: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Let $F$ be a field with $\mathbb Q$ as a subfield and let $B_F$ be the Hamilton algebra over $F$, with basis $1,i,j,k$, relations $i^2=j^2=k^2=-1$ and $ij=k=-ji$ with cyclic rotations. Write $N(x)=\sum_{r=0}^3 x_r^2$ for the reduced norm and $B_F^\times$ for the group of invertible quaternions. Identify $F^\times$ with the normal subgroup of scalar units $\{\lambda1:\lambda\in F^\times\}$ in $B_F^\times$. The projective class $[x]$ is the coset of $x\in B_F^\times$ in the quotient by that subgroup.

If $N(x)=s^2$ for some $s\in F^\times$, then $[x]$ is a commutator in $B_F^\times/F^\times$, meaning a product $aba^{-1}b^{-1}$ of projective classes. In particular every group homomorphism from this projective group to a commutative group sends $[x]$ to the identity.

## Facts & Assumptions

[F1] In a field each nonzero scalar has a multiplicative inverse, and scalar multiplication is commutative ([[math:def-field]]). Both $\mathbb Q$ and $F$ are unital commutative rings with their field operations, zeros and identities ([[math:lem-field-is-a-commutative-ring]], [[math:def-ring]], [[math:def-commutative-ring]]). The rational subfield uses the restricted addition and multiplication and shares $0$ and $1$ with $F$ ([[math:def-subfield]]), so the rational $2=1+1$ remains nonzero in $F$. The inclusion $\mathbb Q\hookrightarrow F$ therefore preserves addition, multiplication and the multiplicative identity, making it a unital ring homomorphism ([[math:def-ring-homomorphism]]). Its image is central since $F$ is commutative, so $F$ is a commutative unital $\mathbb Q$-algebra ([[math:def-algebra-over-a-commutative-ring]]).

[F2] In the Hamilton algebra over a commutative unital $\mathbb Q$-algebra, conjugation $\bar x$ negates the $i,j,k$ coordinates, $x\bar x=\bar x x=N(x)1$, and the norm is multiplicative. The scalars $\lambda1$ commute with every quaternion. Over $F$ a quaternion is invertible exactly when its norm is nonzero, with inverse $\bar x/N(x)$ ([[def-author-6f52147f3ab3-hamilton-order-completions]]).

[F3] A subgroup contains the ambient identity and is closed under products and inverses ([[math:def-subgroup]]). It is normal if conjugation by each ambient element maps it onto itself ([[math:def-normal-subgroup]]). The left coset of a subgroup $S$ represented by $g\in G$ is $gS=\{gh:h\in S\}$ ([[math:def-coset]]). For a normal subgroup $S$ of $G$, the quotient has elements $[g]=gS$ and product $[g][h]=[gh]$ ([[math:def-quotient-group]]). Its identity is $[1]$ and its inverses satisfy $[g]^{-1}=[g^{-1}]$ ([[math:thm-quotient-group-laws]]).

[F4] A group homomorphism preserves products ([[math:def-group-homomorphism]]) and therefore preserves inverses ([[math:lem-group-homomorphism-basic-properties]]). Every group law is associative and every element has a two-sided inverse. In a commutative group the group law is also commutative ([[math:def-group]]).

## Proof

**Given:** An invertible $x$ with $N(x)=s^2$ for $s\in F^\times$.

**Goal:** Express $[x]$ as a projective commutator and deduce its image under any homomorphism to a commutative group.

1.1 The scalar units $S=\{\lambda1:\lambda\in F^\times\}$ contain $1$. The identities $(\lambda1)(\mu1)=(\lambda\mu)1$ and $(\lambda1)^{-1}=\lambda^{-1}1$ give closure under products and inverses. Since the scalar copy of $F$ is central, $g(\lambda1)g^{-1}=\lambda1$ for every $g\in B_F^\times$. Thus $S$ is a normal subgroup, and the quotient rules in [F3] apply. [F1, F2, F3]

2.1 For $h\in S$ we have $hS\subseteq S$ by closure under products. Each $r\in S$ belongs to $hS$ because $r=h(h^{-1}r)$ and $h^{-1}r\in S$. Thus $hS=S$, so $(gh)S=g(hS)=gS$ for every $g\in B_F^\times$ by associativity. Put $w=x/s$. Its norm is $s^{-2}N(x)=1$ by the coordinate formula. If its scalar coordinate is $-1$, use $-w$, whose norm is also one and whose scalar coordinate is $1\ne-1$ because $2\ne0$. These rescalings multiply by $s^{-1}1$ and, when needed, $-1$, both in $S$, so they preserve the projective class. Denote the resulting representative by $t+z$, where $t\ne-1$ and $z$ has scalar coordinate zero. If $z=0$, then $t^2=1$, so the representative lies in $S$ and its class is $[1]$, the commutator of identity elements. [F1, F2, F3, F4, step 1.1]

3.1 For $z\ne0$ write $z=ai+bj+ck$, using a cyclic rotation of $i,j,k$ to arrange $a\ne0$. The quaternions $y_1=bi-aj$ and $y_2=ci-ak$ satisfy $y_1z+zy_1=-2(ba-ab)=0$ and $y_2z+zy_2=-2(ca-ac)=0$ by the multiplication table. If $b=0$ then $N(y_1)=a^2\ne0$, and if $c=0$ then $N(y_2)=a^2\ne0$. If $bc\ne0$ and both candidate norms vanish, then $N(y_1+y_2)=N(y_1)+N(y_2)+2bc=2bc\ne0$. Thus one of $y_1,y_2,y_1+y_2$ is an invertible $y$ with $yz=-zy$. [F1, F2, step 2.1]

4.1 Write $v=t+z$ and set $u=1+v$. Its norm is $N(u)=1+2t+N(v)=2(1+t)\ne0$, so $u$ and $\bar u$ are invertible. The anticommutation in step 3.1 gives $yuy^{-1}=\bar u$, and $v\bar u=v(1+\bar v)=v+1=u$. Since $yu^{-1}y^{-1}$ inverts $yuy^{-1}=\bar u$, we have $uyu^{-1}y^{-1}=u\bar u^{-1}=v$. Passing to projective classes gives the required commutator for the initial $[x]$. [F1, F2, F3, step 2.1, step 3.1]

5.1 In either case write $[x]=aba^{-1}b^{-1}$. If $f$ is a group homomorphism to a commutative group, then $f([x])=f(a)f(b)f(a)^{-1}f(b)^{-1}$. Commutativity lets the inverse factors cancel their respective factors, giving the target identity. [F4, step 2.1, step 4.1] ∎

---
id: def-author-fb1ef6c2c01b-signed-ordered-two-square-count
kind: definition
title: Signed, ordered two-square representations
status: published
domain: mathematics
deps:
  - math:def-integers
  - math:def-int-order
  - math:def-ordered-pair
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-cartesian-product
  - math:def-int-operations
  - math:def-finite-cardinality
  - math:thm-int-ordered-ring
  - math:def-axiom-schema-of-separation
  - math:def-natural-numbers
  - math:lem-nat-order-is-membership
  - math:lem-nat-embeds-int
  - math:def-countable
  - math:thm-product-rule
  - math:thm-subset-of-a-finite-set
  - math:def-subset-and-proper-subset
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:def-nat-order
  - math:def-nat-addition
dependency_roles:
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-ordered-pair: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-axiom-schema-of-separation: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-countable: mathematical-premise
  math:thm-product-rule: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-function: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:def-nat-addition: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 0
---

## Definition

For a positive integer $u$, meaning $u\in\mathbb Z$ with $u>0$, put
$$S_u=\{(x,y)\in\mathbb Z\times\mathbb Z:x^2+y^2=u\},\qquad r_2(u)=\lvert S_u\rvert.$$

Here $\mathbb Z\times\mathbb Z$ is the set of ordered pairs of integers, $x^2$ means $x\cdot x$, and $\lvert S_u\rvert$ is the number of elements of the finite set $S_u$. Signed means each coordinate may be positive, negative or zero. Ordered means two pairs are equal exactly when their first coordinates agree and their second coordinates agree. Each such pair contributes one to the count.

## Facts & Assumptions

[F1] $\mathbb Z$ is the set of integers with integer addition, multiplication, negation and order. It is a totally ordered commutative ring. Addition preserves order and a product of positive integers is positive. ([[math:def-integers]], [[math:def-int-operations]], [[math:def-int-order]], [[math:thm-int-ordered-ring]])

[F2] An ordered pair $(x,y)$ has first coordinate $x$ and second coordinate $y$. Pair equality is coordinatewise. A Cartesian product $A\times B$ consists of such pairs with first coordinate in $A$ and second coordinate in $B$. Separation forms a subset by retaining precisely the elements of a set that satisfy a stated condition. A set is a subset of another when every element of the first belongs to the second. ([[math:def-ordered-pair]], [[math:thm-the-characterising-property-of-ordered-pairs]], [[math:def-cartesian-product]], [[math:def-axiom-schema-of-separation]], [[math:def-subset-and-proper-subset]])

[F3] The natural numbers $\mathbb N$ include $0$, with first successor $1=\sigma(0)=\{0\}$. A natural number $m$ is the set of natural numbers less than $m$. For natural $j,m$, membership $j\in\sigma(m)$, strict order $j<\sigma(m)$ and weak order $j\le m$ are equivalent. The embedding $\iota(n)=[(n,0)]$ is injective, has image the nonnegative integers, preserves addition, and preserves and reflects order. ([[math:def-natural-numbers]], [[math:def-nat-order]], [[math:lem-nat-order-is-membership]], [[math:lem-nat-embeds-int]])

[F4] A subset of $A\times B$ that assigns exactly one element of $B$ to each element of $A$ defines a function from $A$ to $B$. A function is bijective if it is injective and surjective. A set is finite if it admits a bijection, a one-to-one correspondence, with a natural number viewed as a set. Its cardinality is the unique natural number with this property. The product of two finite sets is finite, and every subset of a finite set is finite. ([[math:def-function]], [[math:def-injection-surjection-bijection]], [[math:def-countable]], [[math:def-finite-cardinality]], [[math:thm-product-rule]], [[math:thm-subset-of-a-finite-set]])

[F5] Natural addition satisfies $m+0=m$ and $m+\sigma(j)=\sigma(m+j)$. ([[math:def-nat-addition]])

## Justification

**Given:** a positive integer $u$.

**Goal:** show that $S_u$ exists and its cardinality is a uniquely defined natural number.

1.1 Separation in $\mathbb Z\times\mathbb Z$ gives $S_u$. Let $I_u=\{z\in\mathbb Z:-u\le z\le u\}$, also obtained by Separation. Since $2u=u+u\ge0$, there is a unique natural $m$ with $\iota(m)=2u$. In the naturals $m+1=m+\sigma(0)=\sigma(m+0)=\sigma(m)$, so $j\in m+1$ is equivalent to $j\le m$ for natural $j$. Under the embedding this endpoint is $\iota(m+1)=2u+1$, since $\iota(1)=[(1,0)]$ is the integer $1$. [given, F1, F2, F3, F5]

1.2 Since $u>0$, write $u=\iota(k)$ with $k\in\mathbb N$ and $k\ne0$, using $\iota(0)=[(0,0)]$. If $u<1$, strict order reflection gives $k<1$, so $k\in\sigma(0)=\{0\}$ by natural order as membership. This contradicts $k\ne0$. Totality of the integer order therefore gives $u\ge1$. [given, F1, F3]

2.1 For each $z\in I_u$, translation by $u$ gives $0\le z+u\le 2u$. Thus $z+u=\iota(j)$ for a unique natural $j$. Since $\iota(j)\le\iota(m)$, order reflection gives $j\le m$ and hence $j\in m+1$. Separating the pairs $(z,j)$ with $\iota(j)=z+u$ in $I_u\times(m+1)$ therefore defines a function from $I_u$ to $m+1$. [F1, F2, F3, F4, step 1.1]

2.2 For each integer $z$, either $z$ or $-z$ is nonnegative. Call that nonnegative value $t$. The ring laws give $z^2=t^2\ge0$, since the square is zero for $t=0$ and positive for $t>0$. If $z$ lies outside $I_u$, then $z>u$ or $z<-u$. In the first case $t=z>u$. In the second case, adding $u-z$ to $z<-u$ gives $u<-z=t$. Hence $t>1$ and $t^2-t=t(t-1)>0$. Then $z^2>u$, so $z$ cannot be a coordinate of a pair in $S_u$ because the other square is nonnegative. Consequently $S_u\subseteq I_u\times I_u$. [F1, F2, step 1.1, step 1.2]

3.1 Equal outputs $j$ give equal values of $z+u$, so cancellation gives equal inputs. For every $j\in m+1$, the inequalities $0\le\iota(j)\le\iota(m)=2u$ show that $z=\iota(j)-u$ belongs to $I_u$. Since $z+u=\iota(j)$, this input maps to $j$. The function is injective and surjective and hence a bijection. Thus $I_u$ is finite. [F1, F3, F4, step 1.1, step 2.1]

4.1 The product $I_u\times I_u$ is finite, and its subset $S_u$ is finite. The cardinality of $S_u$ is therefore a unique natural number. Coordinatewise equality gives exactly the signed, ordered counting convention of the definition, including when coordinates coincide or are zero. Thus $r_2(u)$ is well defined. [F2, F4, step 1.1, step 3.1, step 2.2] ∎

---
id: lem-euler-hurwitz-four-square-bijection
kind: lemma
title: From a Hurwitz norm shell to integral four squares
status: draft
domain: mathematics
deps:
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-euler-hurwitz-norm-shell
  - def-euler-four-square-representations
  - lem-rational-hamilton-norm-and-inverse
  - lem-euler-four-square-parities
  - math:thm-int-ordered-ring
  - math:thm-rat-field
  - math:lem-int-embeds-rat
  - math:def-function
  - math:def-injection-surjection-bijection
  - lem-square-residue-parity
formulation_deps:
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-euler-hurwitz-norm-shell
  - def-euler-four-square-representations
  - lem-euler-four-square-parities
  - math:thm-rat-field
  - math:lem-int-embeds-rat
  - math:def-function
  - math:def-injection-surjection-bijection
argument_deps:
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-euler-hurwitz-norm-shell
  - def-euler-four-square-representations
  - lem-rational-hamilton-norm-and-inverse
  - lem-euler-four-square-parities
  - math:thm-int-ordered-ring
  - math:thm-rat-field
  - math:lem-int-embeds-rat
  - math:def-function
  - math:def-injection-surjection-bijection
  - lem-square-residue-parity
dependency_roles:
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  def-euler-hurwitz-norm-shell: mathematical-premise
  def-euler-four-square-representations: mathematical-premise
  lem-rational-hamilton-norm-and-inverse: mathematical-premise
  lem-euler-four-square-parities: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-rat-field: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:def-function: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  lem-square-residue-parity: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §3.1, equation (3.2) and inverse description
dependency_level: 4
---

## Statement

Let $m>0$ be an odd integer, so $m=2r+1$ for some integer $r$. Write a rational Hamilton quaternion in its unique coordinates as $a+bi+cj+dk$, where $i^2=j^2=k^2=-1$ and $ij=k=-ji$, $jk=i=-kj$, $ki=j=-ik$. Its reduced norm is $N(a+bi+cj+dk)=a^2+b^2+c^2+d^2$. The Hurwitz order $\mathcal H$ consists of the quaternions whose coordinates are all integers or all strict half-integers, where a strict half-integer is a number of the form $t+\tfrac12$ with $t$ an integer. Let $Q_m$ consist of the elements of $\mathcal H$ of reduced norm $m$. Let $\mathcal R(2m)$ be the set of ordered integer tuples $(x_1,x_2,x_3,x_4)$ with $x_1^2+x_2^2+x_3^2+x_4^2=2m$.

Right multiplication by $1+i$, followed by taking the coordinate tuple, gives a bijection $F:Q_m\to\mathcal R(2m)$, so each target tuple comes from exactly one input. Explicitly,
$$F(a+bi+cj+dk)=(a-b,a+b,c+d,d-c).$$

The inverse sends each target tuple to the quaternion with coordinates
$$\left(\tfrac{x_1+x_2}{2},\tfrac{x_2-x_1}{2},\tfrac{x_3-x_4}{2},\tfrac{x_3+x_4}{2}\right).$$
These coordinates are all integers or all strict half-integers.

## Statement references

[[def-euler-hamilton-quaternions|Rational Hamilton quaternions and their reduced norm]]

[[def-euler-hurwitz-order|Coordinate description of the Hurwitz order]]

[[def-euler-hurwitz-norm-shell|The Hurwitz norm shell]]

[[def-euler-four-square-representations|Signed ordered four-square representations]]

[[lem-euler-four-square-parities|Odd and even coordinates in four-square representations]]

[[math:thm-rat-field|Field operations on rational numbers]]

[[math:lem-int-embeds-rat|Integers as rational numbers]]

[[math:def-function|Function]]

[[math:def-injection-surjection-bijection|Bijection]]

## Facts & Assumptions

[F1] Rational Hamilton quaternions have unique coordinates in $1,i,j,k$. Multiplication is associative, distributes over addition, and uses commuting rational scalars and the basis rules in the Statement. Their reduced norm is the sum of the four coordinate squares. [[def-euler-hamilton-quaternions]]

[F2] Membership in $\mathcal H$ means having four integer coordinates or four strict half-integer coordinates. The shell $Q_m$ consists of the members of $\mathcal H$ of reduced norm $m$. [[def-euler-hurwitz-order]] [[def-euler-hurwitz-norm-shell]]

[F3] For a positive integer $n$, membership in $\mathcal R(n)$ means that the four coordinates are integers and their squares sum to $n$. [[def-euler-four-square-representations]]

[F4] The reduced norm satisfies $N(vw)=N(v)N(w)$ for rational Hamilton quaternions $v,w$. For nonzero $v=a+bi+cj+dk$, its two-sided multiplicative inverse is $v^{-1}=\bar v/N(v)$, with $\bar v=a-bi-cj-dk$ and with division by a rational scalar applied to each coordinate. [[lem-rational-hamilton-norm-and-inverse]]

[F5] If a positive integer $n$ is of the form $4r+2$ with $r$ an integer, every tuple in $\mathcal R(n)$ has exactly two odd coordinates. An integer is even if it has the form $2t$ and odd if it has the form $2t+1$, with $t$ an integer. A pair has the same parity when both entries are even or both are odd. It has opposite parity when one entry is even and the other is odd. [[lem-euler-four-square-parities]]

[F6] Sums and differences of integers are integers, and the product of positive integers is positive. [[math:thm-int-ordered-ring]]

[F7] Rational sums, differences and products are defined, and so is division by any nonzero rational. Identifying an integer $t$ with the rational $t/1$ preserves addition, multiplication and order. [[math:thm-rat-field]] [[math:lem-int-embeds-rat]]

[F8] A function is a bijection when each target element has exactly one input mapping to it. [[math:def-injection-surjection-bijection]]

[F9] Every integer is either even, of the form $2q$, or odd, of the form $2q+1$, with $q$ an integer. The two cases are mutually exclusive. [[lem-square-residue-parity]]

[F10] A function from one set to another is a relation assigning each input in the first set exactly one value in the second set. [[math:def-function]]

## Proof

**Given:** An integer $m>0$ and an integer $r$ with $m=2r+1$.

**Goal:** Show that the displayed coordinate rules give mutually inverse maps between $Q_m$ and $\mathcal R(2m)$.

1.1 Put $u=1+i$. Its coordinates are $(1,1,0,0)$, so $N(u)=2$. Since $u$ is nonzero, its two-sided inverse is $u^{-1}=(1-i)/2$. [F1, F4, F7]

1.2 Take $x=(x_1,x_2,x_3,x_4)\in\mathcal R(2m)$. Since $2m=4r+2>0$, exactly two of the coordinates of $x$ are odd. The other two must be even because each integer has exactly one parity. If the odd entries lie in the same pair, one of $(x_1,x_2)$ and $(x_3,x_4)$ has two odd entries and the other has two even entries. If the odd entries lie in different pairs, each pair has one odd and one even entry. [given, F3, F5, F6, F9]

2.1 Take $\alpha=a+bi+cj+dk$ in $Q_m$. The rules $i^2=-1$, $ji=-k$ and $ki=j$ give $\alpha i=-b+ai+dj-ck$. Adding $\alpha$ gives $\alpha u=(a-b)+(a+b)i+(c+d)j+(d-c)k$. [F1, F2, step 1.1]

2.2 Put $y=x_1+x_2i+x_3j+x_4k$. Right multiplication by $u^{-1}$ gives $yu^{-1}=(y-yi)/2$, where $yi=-x_2+x_1i+x_4j-x_3k$. Thus $yu^{-1}$ has the four coordinates in the stated inverse formula. Denote this quaternion by $G(x)$. [F1, F3, F7, step 1.1, step 1.2]

3.1 If $a,b,c,d$ are integers, the four displayed sums and differences are integers. Otherwise each entry is an integer plus $\tfrac12$ by membership in $\mathcal H$. For entries $s+\tfrac12$ and $t+\tfrac12$ their sum is $s+t+1$ and their difference is $s-t$, so all four output coordinates are integers in this case as well. [F2, F6, F7, step 2.1]

3.2 In a pair of the same parity, write both entries as $2s+\epsilon$ and $2t+\epsilon$ with $\epsilon\in\{0,1\}$. The sum is $2(s+t+\epsilon)$ and the difference is $2(s-t)$, so both halves are integers. In a pair of opposite parity write the even entry as $2s$ and the odd entry as $2t+1$. Their sum is $2(s+t)+1$, and the two differences are $2(t-s)+1$ and $2(s-t-1)+1$. Each of their halves is of the form $v+\tfrac12$ with $v$ an integer. By step 1.2 the two pairs both fall in the first case or both fall in the second. Hence all four halves are integers or all four are strict half-integers, so $G(x)\in\mathcal H$. [F2, F5, F6, F7, F9, step 1.2, step 2.2]

4.1 Since $N(\alpha)=m$, multiplicativity gives $N(\alpha u)=m\cdot 2=2m$. This is the sum of the four output coordinate squares. The coordinate formula in step 2.1 determines one tuple for each $\alpha\in Q_m$. Since $2m>0$, the integrality check and the norm identity put that tuple in $\mathcal R(2m)$, so the rule defines a function $F:Q_m\to\mathcal R(2m)$. [given, F1, F2, F3, F4, F6, F7, F10, step 1.1, step 2.1, step 3.1]

4.2 The coordinates of $u^{-1}$ give $N(u^{-1})=(1/2)^2+(-1/2)^2=1/2$. The tuple condition gives $N(y)=2m$, so $N(G(x))=(2m)(1/2)=m$. Together with its Hurwitz order membership this gives $G(x)\in Q_m$. For each $x\in\mathcal R(2m)$ the four halves in step 2.2 determine a unique quaternion by uniqueness of Hamilton coordinates. Thus the rule defines a function $G:\mathcal R(2m)\to Q_m$. [F1, F2, F3, F4, F7, F10, step 1.1, step 2.2, step 3.2]

5.1 For $\alpha\in Q_m$, the tuple $F(\alpha)$ determines the quaternion $\alpha u$ uniquely, so $G(F(\alpha))=(\alpha u)u^{-1}=\alpha$. For $x\in\mathcal R(2m)$, the quaternion for $F(G(x))$ is $(yu^{-1})u=y$, whose tuple is $x$. Both equalities use associativity and the two-sided inverse of $u$. Hence each target tuple has exactly one input, and $F$ is the stated bijection with inverse $G$. [F1, F8, step 1.1, step 4.1, step 2.2, step 4.2] ∎

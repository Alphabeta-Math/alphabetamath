---
id: lem-euler-hurwitz-euclidean
kind: lemma
title: The Hurwitz order is norm-Euclidean
status: published
domain: mathematics
deps:
  - math:def-real-numbers
  - math:def-integers
  - math:def-rationals
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-ordered-field
  - math:thm-reals-ordered-field
  - math:thm-int-ordered-ring
  - math:def-quaternions
  - math:lem-integer-part
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - thm-hurwitz-order-integral-structure
  - lem-rational-hamilton-norm-and-inverse
formulation_deps:
  - math:def-real-numbers
  - math:def-integers
  - math:def-rationals
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-ordered-field
  - math:thm-reals-ordered-field
  - math:def-quaternions
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
argument_deps:
  - math:def-rationals
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-ordered-field
  - math:thm-reals-ordered-field
  - math:thm-int-ordered-ring
  - math:def-quaternions
  - math:lem-integer-part
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - thm-hurwitz-order-integral-structure
  - lem-rational-hamilton-norm-and-inverse
dependency_roles:
  math:def-real-numbers: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-rationals: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:def-ordered-field: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-quaternions: mathematical-premise
  math:lem-integer-part: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  thm-hurwitz-order-integral-structure: mathematical-premise
  lem-rational-hamilton-norm-and-inverse: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §3.1, paragraph beginning “The order H is norm-Euclidean”
      reading_limits: Read the order definition and rounding paragraph on PDF p. 2 for
        attribution. The proof below derives the rounding rule and the two
        division identities locally.
dependency_level: 3
---

## Statement

Use the usual ordered real numbers $\mathbb R$ and view the integers $\mathbb Z$ in $\mathbb R$ through the maps $n\mapsto n/1$ and $t\mapsto\widehat t$, where $\widehat t$ is the real represented by the constant sequence with rational value $t$. The real Hamilton quaternions $\mathbb H$ are real quadruples with coordinates in the basis $1,i,j,k$, where $i^2=j^2=k^2=-1$ and $ij=k=-ji$, $jk=i=-kj$, $ki=j=-ik$. The rational Hamilton algebra $B$ consists of the quadruples with rational coordinates, with the inherited operations. For $x\in\mathbb H$ write $N(x)=x_0^2+x_1^2+x_2^2+x_3^2$, the quaternion norm. On $B$ this is the reduced norm viewed in $\mathbb R$. The Hurwitz order $\mathcal H$ consists of the elements of $B$ whose coordinates are all integers or all strict half-integers. A strict half-integer is a number of the form $n+\tfrac12$ with $n\in\mathbb Z$.

For each $x\in\mathbb H$, rounding its coordinates to the integers $p_s$ determined by $p_s-\tfrac12\le x_s<p_s+\tfrac12$ gives $p=(p_0,p_1,p_2,p_3)\in\mathcal H$ with $N(x-p)\le1$. Equality forces all four coordinates of $x$ to be strict half-integers. In that case $x$ itself belongs to $\mathcal H$ and gives remainder zero. Thus every $x\in\mathbb H$ admits $q\in\mathcal H$ with $N(x-q)<1$.

In particular, $\mathcal H$ is **norm-Euclidean on both sides**. This means that for all $a,b\in\mathcal H$ with $b\ne0$ there are $q_{\mathrm R},q_{\mathrm L},r_{\mathrm R},r_{\mathrm L}\in\mathcal H$ such that $a=bq_{\mathrm R}+r_{\mathrm R}=q_{\mathrm L}b+r_{\mathrm L}$ and $N(r_{\mathrm R}),N(r_{\mathrm L})<N(b)$. The subscripts indicate the side of $b$ on which the quotient is multiplied.

## Facts & Assumptions

[F1] The scalars are the reals, with the integers embedded through the rationals. The rationals $\mathbb Q$ are classes $a/b$ of pairs of integers with $b\ne0$, where $a/b=c/d$ exactly when $ad=cb$. [[math:def-rationals]] The map from integers sends $n$ to $n/1$, and the map from rationals sends each rational to its constant-sequence class in the reals. The integer map preserves order, addition and multiplication. The rational map is an ordered-field embedding. [[math:def-integers]] [[math:def-real-numbers]] [[math:lem-int-embeds-rat]] [[math:lem-rat-embeds-dense]]

[F2] In the real ordered field, $v>u$ means that $v-u$ is positive. Exactly one of $z>0$, $z=0$, and $-z>0$ holds, and positive numbers are closed under addition and multiplication. [[math:thm-reals-ordered-field]] [[math:def-ordered-field]]

[F3] A real quaternion is a real coordinate quadruple with the Hamilton product given by the basis rules in the statement. Subtraction is coordinatewise, and its norm is the sum of its four coordinate squares. On the rational-coordinate algebra $B$ the operations are the restricted real operations, and the reduced norm uses the same four-square formula over the rationals. The embedding in [F1] therefore gives the same value in $\mathbb R$. [[math:def-quaternions]] [[def-euler-hamilton-quaternions]]

[F4] The integer-coordinate and strict-half-integer-coordinate parts are precisely the two parts of $\mathcal H$. With inherited operations, $\mathcal H$ is closed under addition, negation and multiplication and contains $1$. Its norm takes integer values. [[def-euler-hurwitz-order]] [[thm-hurwitz-order-integral-structure]]

[F5] For every real $y$, its integer part $\lfloor y\rfloor$ is the unique integer $m$ with $m\le y<m+1$, using the embedding in [F1]. Integers are closed under subtraction and contain $1$. [[math:lem-integer-part]] [[math:thm-int-ordered-ring]]

[F6] In $B$, multiplication is associative with identity $1$ and distributes over subtraction on both sides. Every nonzero $b\in B$ has a two-sided inverse $b^{-1}$ in $B$, meaning $bb^{-1}=b^{-1}b=1$. For $u,v\in B$, the norm satisfies $N(uv)=N(u)N(v)$, also as an equality in $\mathbb R$ by [F1] and [F3]. [[lem-rational-hamilton-norm-and-inverse]]

## Proof

**Given:** A real quaternion $x$ and, for the division assertion, elements $a,b\in\mathcal H$ with $b\ne0$.

**Goal:** Establish the rounded norm bound and its equality case, then use the strict bound to obtain division on both sides.

1.1 Put $h=\tfrac12$. In the real ordered field $1>0$, since if $-1>0$ its square would also make $1>0$, contradicting trichotomy. Then $2=1+1>0$, and $h>0$ since $2h=1$ would be negative if $h$ were negative and zero if $h=0$. For $s\in\{0,1,2,3\}$ put $p_s=\lfloor x_s+h\rfloor$ and $e_s=x_s-p_s$. The inequalities $p_s\le x_s+h<p_s+1$ are equivalent to $-h\le e_s<h$ because $1-h=h$. The characterization of the integer part gives existence and uniqueness for the stated rounding rule. The quaternion $p$ with these four integer coordinates belongs to $\mathcal H$. [F2, F3, F4, F5]

2.1 For each $s$, the difference $\tfrac14-e_s^2=(h-e_s)(h+e_s)$ is nonnegative. The first factor is strictly positive and the second is nonnegative, so the product is zero exactly when $e_s=-h$. Adding the four differences gives $1-N(x-p)\ge0$. This sum is zero exactly when each difference is zero, since a positive summand with all other summands nonnegative makes the sum positive. [F2, F3, step 1.1]

3.1 If $N(x-p)<1$, take $q=p$. If $N(x-p)=1$, then $e_s=-h$ for every $s$. Thus $x_s=p_s-h=(p_s-1)+h$ with $p_s-1\in\mathbb Z$. The rational $2/1$ maps to the nonzero real $2$. The ordered-field embedding takes $t=(2/1)^{-1}\in\mathbb Q$ to $h$, since it preserves products and $1$, and $2h=1$. Consequently $x_s=\widehat{(p_s-1)/1+t}$, the real image of a rational number. Thus $x\in B$ and all its coordinates are strict half-integers, so $x\in\mathcal H$. Take $q=x$ in this case and $N(x-q)=0$. This proves the strict approximation for every real quaternion. [F1, F2, F3, F4, F5, step 1.1, step 2.1]

4.1 Form $u=b^{-1}a$ and $v=ab^{-1}$ in $B$. Both are real quaternions, so the strict approximation gives $q_{\mathrm R},q_{\mathrm L}\in\mathcal H$ with $N(u-q_{\mathrm R})<1$ and $N(v-q_{\mathrm L})<1$. Put $r_{\mathrm R}=a-bq_{\mathrm R}$ and $r_{\mathrm L}=a-q_{\mathrm L}b$. Closure under products and subtraction puts both remainders in $\mathcal H$. Since $bu=a$ and $vb=a$, distributivity gives $r_{\mathrm R}=b(u-q_{\mathrm R})$ and $r_{\mathrm L}=(v-q_{\mathrm L})b$. [F3, F4, F6, step 3.1]

5.1 Since $b\ne0$, at least one coordinate of $b$ is nonzero. Each coordinate square is nonnegative and the square of a nonzero coordinate is positive by the ordered-field rules, applying positivity of products to its negative if necessary. Hence $N(b)>0$. The factors $u-q_{\mathrm R}$ and $v-q_{\mathrm L}$ lie in $B$, so multiplicativity gives $N(r_{\mathrm R})=N(b)N(u-q_{\mathrm R})<N(b)$ and $N(r_{\mathrm L})=N(v-q_{\mathrm L})N(b)<N(b)$. These remainders have integer norms by [F4]. By the definitions of the remainders, $a=bq_{\mathrm R}+r_{\mathrm R}$ and $a=q_{\mathrm L}b+r_{\mathrm L}$. These identities and the strict inequalities give norm-Euclidean division on both sides. [F2, F3, F4, F6, step 4.1] ∎

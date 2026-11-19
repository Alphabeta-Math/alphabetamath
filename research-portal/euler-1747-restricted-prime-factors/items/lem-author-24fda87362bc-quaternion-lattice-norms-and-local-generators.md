---
id: lem-author-24fda87362bc-quaternion-lattice-norms-and-local-generators
kind: lemma
title: Norms of quaternion lattices and their local generators
status: published
domain: mathematics
deps:
  - math:thm-int-ordered-ring
  - math:lem-int-bounded-above-has-greatest
  - math:thm-induction-principle
  - def-author-24fda87362bc-hamilton-algebra-and-reduced-norm
  - def-author-24fda87362bc-quaternion-orders-and-lattice-completions
  - def-author-24fda87362bc-local-adic-valuation
  - math:def-common-divisor-and-gcd
  - math:def-divides-in-z
  - math:thm-bezout-identity
  - math:thm-fundamental-theorem-of-arithmetic
  - math:def-rat-order
  - math:lem-int-embeds-rat
  - math:lem-units-of-z
  - math:thm-rat-field
formulation_deps:
  - def-author-24fda87362bc-hamilton-algebra-and-reduced-norm
  - def-author-24fda87362bc-quaternion-orders-and-lattice-completions
  - def-author-24fda87362bc-local-adic-valuation
  - math:def-rat-order
  - math:lem-int-embeds-rat
argument_deps:
  - math:thm-int-ordered-ring
  - math:lem-int-bounded-above-has-greatest
  - math:thm-induction-principle
  - def-author-24fda87362bc-hamilton-algebra-and-reduced-norm
  - def-author-24fda87362bc-quaternion-orders-and-lattice-completions
  - def-author-24fda87362bc-local-adic-valuation
  - math:def-common-divisor-and-gcd
  - math:def-divides-in-z
  - math:thm-bezout-identity
  - math:thm-fundamental-theorem-of-arithmetic
  - math:def-rat-order
  - math:lem-int-embeds-rat
  - math:lem-units-of-z
  - math:thm-rat-field
dependency_roles:
  math:thm-int-ordered-ring: mathematical-premise
  math:lem-int-bounded-above-has-greatest: mathematical-premise
  math:thm-induction-principle: mathematical-premise
  def-author-24fda87362bc-hamilton-algebra-and-reduced-norm: mathematical-premise
  def-author-24fda87362bc-quaternion-orders-and-lattice-completions: mathematical-premise
  def-author-24fda87362bc-local-adic-valuation: mathematical-premise
  math:def-common-divisor-and-gcd: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:thm-bezout-identity: mathematical-premise
  math:thm-fundamental-theorem-of-arithmetic: mathematical-premise
  math:def-rat-order: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-units-of-z: mathematical-premise
  math:thm-rat-field: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 2
---

## Statement

Let $L$ be a full integral lattice and $O$ an order in the rational Hamilton algebra $B$. Let $\ell$ be a prime. Use $A$ for the set of finite integer linear combinations of reduced norms of elements of $L$, and $A_\ell$ for the set of finite $\mathbb Z_\ell$-linear combinations of reduced norms of elements of $L_\ell$ in $B_\ell$. For a subset of $\mathbb Q$, its $\mathbb Z_\ell$-span inside $\mathbb Q_\ell$ is denoted by multiplication by $\mathbb Z_\ell$.

There is a unique positive rational $d$ with $A=d\mathbb Z$, and $A_\ell=A\mathbb Z_\ell$. Every element of $O$ has integral reduced norm, and every element of $O_\ell$ has reduced norm in $\mathbb Z_\ell$. If $L=xO$ with $x\in B^\times$, then $A=N(x)\mathbb Z$. If $L_\ell=x_\ell O_\ell$ with $x_\ell\in B_\ell^\times$, then $A_\ell=N(x_\ell)\mathbb Z_\ell$ and $v_\ell(d)=v_\ell(N(x_\ell))$.

## Facts & Assumptions

[F1] In the Hamilton coordinates of [[def-author-24fda87362bc-hamilton-algebra-and-reduced-norm]], the reduced norm is the sum of the four squares, $N(1)=1$, $N(xy)=N(x)N(y)$ and $N$ is nonzero on units and positive on nonzero rational quaternions.

[F2] A full integral lattice has a rational basis that freely generates it over $\mathbb Z$ and generates its local completion over $\mathbb Z_\ell$. An order and its local completion contain $1$ and are closed under multiplication by [[def-author-24fda87362bc-quaternion-orders-and-lattice-completions]].

[F3] By [[def-author-24fda87362bc-local-adic-valuation]], a prime is greater than $1$, the field $\mathbb Q_\ell$ contains $\mathbb Q$, and $\mathbb Z_\ell$ is a subring containing the embedded integers. Nonzero elements of $\mathbb Q_\ell$ have integer valuation, additive on products. An element $z\in\mathbb Q_\ell$ belongs to $\mathbb Z_\ell$ exactly when $v_\ell(z)\ge0$, with $v_\ell(0)=+\infty$. A scalar in $\mathbb Z_\ell$ is a unit exactly when its valuation is zero. The valuation on nonzero rationals is the numerator exponent minus the denominator exponent. For a nonzero integer $a$, the exponent is the greatest $k\ge0$ such that $\ell^k$ divides $a$.

[F4] For two integers, at least one nonzero, their greatest common divisor is positive and divides both by [[math:def-common-divisor-and-gcd]]. It is also an integer linear combination of them by [[math:thm-bezout-identity]]. An integer divides another when the latter is an integer multiple of the former by [[math:def-divides-in-z]].

[F5] Every positive integer has a factorization into primes that is unique up to order by [[math:thm-fundamental-theorem-of-arithmetic]].

[F6] The integers form a totally ordered ring, so adding an integer to both sides of a strict inequality preserves that inequality and a product of positive integers is positive ([[math:thm-int-ordered-ring]]). Every nonempty set of integers with an integer lower bound has a least member ([[math:lem-int-bounded-above-has-greatest]]).

[F7] A property of natural numbers holds for every natural number if it holds at zero and passes from each number to its successor ([[math:thm-induction-principle]]).

[F8] Every rational has a representative with positive denominator, and in such a representative the rational is positive exactly when its numerator is positive ([[math:def-rat-order]]). The embedding $m\mapsto m/1$ of $\mathbb Z$ in $\mathbb Q$ is injective and preserves addition, multiplication and order ([[math:lem-int-embeds-rat]]).

[F9] An integer $u$ divides $1$ exactly when $u=1$ or $u=-1$ ([[math:lem-units-of-z]]).

[F10] The rationals form a commutative field, so every nonzero rational has a multiplicative inverse ([[math:thm-rat-field]]).

## Proof

**Given:** The lattices $L$ and $O$, a prime $\ell$, and the spans $A$ and $A_\ell$ in the statement. In the assertions on principal lattices assume the stated invertible generators exist.

**Goal:** Identify the two norm spans, establish integrality on orders, and compute the norm spans and valuation when generators are given.

1.1 Take an integer basis $b_1,\ldots,b_4$ of $L$ as in [F2]. Let $S$ consist of the $N(b_i)$ and the $N(b_i+b_j)$ for $i<j$. For coefficients $t_i$ in either $\mathbb Z$ or $\mathbb Z_\ell$, expanding the four squares gives $N(\sum_i t_i b_i)=\sum_i t_i^2N(b_i)+\sum_{i<j}t_i t_j\bigl(N(b_i+b_j)-N(b_i)-N(b_j)\bigr)$. Every element of $S$ is already a norm from $L$, which embeds in $L_\ell$. Hence $S$ generates both $A$ over $\mathbb Z$ and $A_\ell$ over $\mathbb Z_\ell$, and $A_\ell=A\mathbb Z_\ell$. [F1, F2, F3, given]

1.2 Choose $C$ to be the product of the positive denominators of the four rational coordinates of every vector in an integer basis of $O$. By [F2], elements of $O_\ell$ then have coordinates in $C^{-1}\mathbb Z_\ell$. For each $u\in O_\ell$, the four-square formula therefore gives $C^2N(u)\in\mathbb Z_\ell$. The set of valuations of nonzero norms of elements of $O_\ell$ is a subset of the integers containing $0$, since $1\in O_\ell$ and $N(1)=1$. By additivity of valuation it is bounded below by $-2v_\ell(C)$. By [F6] let $m$ be its least member and take $u\in O_\ell$ with $v_\ell(N(u))=m$. Then $u^2\in O_\ell$ and $N(u^2)=N(u)^2\ne0$. Its valuation is $m+m$, which would be strictly below $m$ if $m<0$. Thus $m\ge0$. Every nonzero norm from $O_\ell$ has valuation at least $m\ge0$ and therefore belongs to $\mathbb Z_\ell$ by [F3], and the zero norm belongs to that ring as well. [F1, F2, F3, F6, F8, F10, given]

2.1 For $u\in O$, Step 1.2 gives nonnegative valuation of $N(u)$ at every prime. If $N(u)=0$, it is integral. Otherwise by [F8] write $N(u)=a/b$ with nonzero integers $a,b$ and $b>0$. By [F4], $h=\gcd(a,b)>0$ divides both $a$ and $b$, and $ar+bs=h$ for integers $r,s$. Write $a=ha'$ and $b=hb'$ with $a',b'\in\mathbb Z$. Factoring $h$ from $ar+bs=h$ gives $h(a'r+b's)=h$ by [F6]. Multiplying by $h^{-1}$ in $\mathbb Q$ gives $a'r+b's=1$, which holds in $\mathbb Z$ by [F8]. Cancelling $h$ in the fraction gives $a/b=a'/b'$ by [F10]. The quotient $b/h$ is positive by the positive numerator and denominator criterion in [F8], so $b'>0$ in $\mathbb Z$ as well. If $b'\ne1$, [F5] gives a nonempty prime factorization of $b'$. Take a prime $p$ in this factorization, so $p\mid b'$. If $p$ also divided $a'$, then $a'=pk$ and $b'=pj$ for integers $k,j$ by [F4]. Distributivity in [F6] gives $1=a'r+b's=p(kr+js)$, so $p$ divides $1$. This is impossible by [F9] because $p>1$ by [F3]. Thus $v_p(a')=0$ and $v_p(b')\ge1$, contradicting the nonnegative valuation of $N(u)=a'/b'$ by [F3]. Hence $b'=1$ and $N(u)\in\mathbb Z$. [F3, F4, F5, F6, F8, F9, F10, step 1.2, given]

2.2 Let $D$ be the product of the positive denominators for the finitely many elements of $S$, so every element of $DS$ is an integer. The integers in $DS$ include a nonzero one because $N(b_1)>0$. List the entries of $DS$ with one nonzero entry first. Apply [F7] with the first entry as the base case and one further entry added at each stage. For the first entry $s_1\ne0$, take $c=s_1$ if $s_1>0$ and $c=-s_1$ if $s_1<0$. Adding $-s_1$ to $s_1<0$ gives $-s_1>0$ by [F6]. In the second case $c=(-1)s_1$ and $s_1=(-1)c$, so each is an integer multiple of the other and the two spans agree. For the current positive generator $c$ and the next entry $s$, take $h=\gcd(c,s)$. By [F4], $h$ is an integer linear combination of $c$ and $s$, and $c$ and $s$ are integer multiples of $h$. Thus $c\mathbb Z+s\mathbb Z=h\mathbb Z$. This gives a positive generator for the enlarged part of the list, which completes the induction. Thus $DA=g\mathbb Z$ for some positive integer $g$. Multiplying by $D^{-1}$ in $\mathbb Q$ gives $A=d\mathbb Z$ for $d=g/D$, positive by [F8]. If $e$ is another positive rational generator, write $e=g'/D'$ with $g',D'>0$ by [F8]. The equal spans give integers $m,n$ with $d=me$ and $e=nd$. By [F10] the equalities give $m=d/e=gD'/(Dg')$ and $n=e/d=g'D/(D'g)$. These quotients have positive numerators and denominators by [F6], so $m,n$ are positive integers by [F8]. Since $d=mnd$ with $d\ne0$, multiplying by $d^{-1}$ in $\mathbb Q$ gives $mn=1$ there by [F10]. Injectivity in [F8] gives $mn=1$ in $\mathbb Z$. By [F9] the two positive integer divisors $m,n$ of $1$ both equal $1$, so $d=e$. [F1, F4, F6, F7, F8, F9, F10, step 1.1]

3.1 If $L=xO$, all norms from $L$ belong to $N(x)\mathbb Z$ by multiplicativity and Step 2.1. The norm $N(x)$ itself occurs by taking $x\cdot1$. This gives $A=N(x)\mathbb Z$. If $L_\ell=x_\ell O_\ell$, the same two inclusions give $A_\ell=N(x_\ell)\mathbb Z_\ell$, since each $N(x_\ell u)$ is $N(x_\ell)N(u)$ with $N(u)\in\mathbb Z_\ell$ and $u=1$ supplies $N(x_\ell)$. [F1, F2, step 1.2, step 2.1, given]

4.1 By Steps 1.1 and 2.2 the local span is also $d\mathbb Z_\ell$. If a local generator is given, put $a=N(x_\ell)$. Since $x_\ell$ is a unit, $a\ne0$ by [F1]. By Step 3.1 the two spans $d\mathbb Z_\ell$ and $a\mathbb Z_\ell$ coincide. Thus $d=aq$ and $a=dr$ for some $q,r\in\mathbb Z_\ell$. Both $a$ and $d$ are nonzero in $\mathbb Q_\ell$, and division there gives $q=d/a$ and $r=a/d$. Hence $q$ is a unit with inverse $r$. The equality $d=aq$ and [F3] give $v_\ell(d)=v_\ell(a)+v_\ell(q)=v_\ell(N(x_\ell))$. Together the steps give the two spans, both integrality claims, and the formulas for principal lattices. [F1, F3, step 1.1, step 2.2, step 1.2, step 2.1, step 3.1] ∎

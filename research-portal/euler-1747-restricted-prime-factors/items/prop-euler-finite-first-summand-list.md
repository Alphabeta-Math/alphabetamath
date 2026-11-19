---
id: prop-euler-finite-first-summand-list
kind: proposition
title: Explicit list of eligible first summands up to 313
status: draft
domain: mathematics
deps:
  - math:def-rationals
  - math:def-rat-order
  - math:def-rat-operations
  - math:def-real-numbers
  - math:def-real-order
  - def-euler-finite-first-summand-indices
  - def-euler-finite-certificate-indices
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - def-euler-prime-classes
  - lem-euler-finite-indicator-membership
  - lem-euler-finite-small-obstructing-divisor
  - lem-trial-division-primality-bound
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:lem-of-square-monotone
  - math:thm-reals-ordered-field
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
  - math:def-axiom-of-extensionality
  - math:def-natural-numbers
  - math:def-nat-order
formulation_deps:
  - def-euler-finite-first-summand-indices
  - def-euler-finite-certificate-indices
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
argument_deps:
  - math:def-rationals
  - math:def-rat-order
  - math:def-rat-operations
  - math:def-real-numbers
  - math:def-real-order
  - def-euler-finite-first-summand-indices
  - def-euler-finite-certificate-indices
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - def-euler-prime-classes
  - lem-euler-finite-indicator-membership
  - lem-euler-finite-small-obstructing-divisor
  - lem-trial-division-primality-bound
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:lem-of-square-monotone
  - math:thm-reals-ordered-field
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
  - math:def-axiom-of-extensionality
  - math:def-natural-numbers
  - math:def-nat-order
dependency_roles:
  math:def-rationals: mathematical-premise
  math:def-rat-order: mathematical-premise
  math:def-rat-operations: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:def-real-order: mathematical-premise
  def-euler-finite-first-summand-indices: mathematical-premise
  def-euler-finite-certificate-indices: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  lem-euler-finite-indicator-membership: mathematical-premise
  lem-euler-finite-small-obstructing-divisor: mathematical-premise
  lem-trial-division-primality-bound: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:lem-of-square-monotone: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:def-axiom-of-extensionality: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-nat-order: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, displayed set of possible summands after the definition of J
dependency_level: 5
---

## Statement

Use the certificate indicator $\varepsilon_i$ of (7.1), which takes a value in $\{0,1\}$ for each integer $0\le i\le H=4{,}194{,}303$. Let $J$ consist of the integers $i$ with $0\le i\le78$ for which $\varepsilon_i=1$. A possible first summand is an integer of the form $4i+1$ with $i\in J$. The set of these summands is
$$\left\{\begin{gathered}1,5,13,17,25,29,37,41,53,61,65,73,85,89,97,\\101,109,113,125,137,145,149,157,169,173,181,185,\\193,197,205,221,229,233,241,257,265,269,277,281,\\289,293,305,313\end{gathered}\right\}.$$

## Statement references

[[def-euler-finite-certificate-indices]]

[[def-euler-finite-first-summand-indices]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

## Facts & Assumptions

[F1] The certificate defines $\varepsilon_i$ at every integer index from $0$ through $H=4{,}194{,}303$. The first-summand definition takes exactly the values $4i+1$ at integer indices from $0$ through $78$ with $\varepsilon_i=1$. [[def-euler-finite-certificate-indices]] [[def-euler-finite-first-summand-indices]]

[F2] For integer $0\le i\le H$, the certificate indicator satisfies $\varepsilon_i=1$ exactly when $4i+1\in\mathcal A$. Here $\mathcal A$ consists of the positive integers every prime divisor of which is congruent to $1$ modulo $4$. [[lem-euler-finite-indicator-membership]] [[def-euler-prime-classes]]

[F3] Write $\mathbb Z$ for the integers. An integer $d$ divides an integer $a$, written $d\mid a$, when $a=dq$ for some $q\in\mathbb Z$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself, where positive means greater than $0$. A prime divisor is a divisor that is prime. Congruence $x\equiv r\pmod 4$ means $x-r=4q$ for some $q\in\mathbb Z$. The class $\mathcal P_3$ consists of primes congruent to $3$ modulo $4$. [[math:def-integers]] [[math:def-int-order]] [[math:def-divides-in-z]] [[math:def-prime]] [[math:def-congruence-modulo-an-integer]] [[def-euler-prime-classes]]

[F4] If $0\le i\le H$ is an integer and $4i+1$ has a prime divisor in $\mathcal P_3$, it has one such divisor $p$ with $p\le\sqrt{4i+1}$. The square root here is the nonnegative real number with square $4i+1$. [[lem-euler-finite-small-obstructing-divisor]] [[math:def-real-numbers]] [[math:def-real-order]]

[F5] For comparisons in the reals $\mathbb R$, write $\iota(k)$ for the real class of the constant sequence of value $k/1$ in the rationals $\mathbb Q$. Both maps use the same rational addition, multiplication, and order. They are injective, preserve addition and multiplication, and preserve and reflect order. The composition sends integer $0$ to real $0$. In the ordered real field, for $x,y\ge0$ one has $x\le y$ exactly when $x^2\le y^2$, with $x^2=x\cdot x$. [[math:def-rationals]] [[math:def-rat-order]] [[math:def-rat-operations]] [[math:def-real-numbers]] [[math:lem-int-embeds-rat]] [[math:lem-rat-embeds-dense]] [[math:thm-reals-ordered-field]] [[math:lem-of-square-monotone]] [[math:def-real-order]]

[F6] Integer addition preserves order, and multiplication by a positive integer preserves order by distributivity and positivity of products. Under the inclusion that preserves order and arithmetic, the natural numbers $0,1,2,\ldots$ are exactly the nonnegative integers. There is no natural number strictly between successive natural numbers. Thus there is no integer strictly between $-1$ and $0$, since taking its negative would put an integer strictly between $0$ and $1$. [[math:def-int-operations]] [[math:thm-int-ordered-ring]] [[math:def-natural-numbers]] [[math:lem-nat-embeds-int]] [[math:lem-nat-discrete]] [[math:def-nat-order]]

[F7] For integer $u>1$, trial division says $u$ is prime precisely when no integer $d\ge2$ with $d^2\le u$ divides $u$. This is the square-bound form of the trial-division lemma. For any integer $u$ and positive integer $d$, division gives unique integers $q,r$ with $u=dq+r$ and $0\le r<d$. The integer $r$ is the remainder, and it is zero exactly when $d$ divides $u$. [[lem-trial-division-primality-bound]] [[math:thm-division-algorithm-in-z]]

[F8] Sets with exactly the same members are equal. [[math:def-axiom-of-extensionality]]

## Proof

**Given:** The certificate indicators $\varepsilon_i$ and the index set $J$ of the statement.

**Goal:** Determine all values $4i+1$ for $i\in J$.

1.1 Take any integer $i$ with $0\le i\le78$ and put $a=4i+1$. Then $1\le a\le4\cdot78+1=313$, and $78\le H$ allows us to apply the indicator criterion. Thus $i\in J$ exactly when $a\in\mathcal A$. [given, F1, F2, F6]

2.1 Divide any prime divisor $p$ of $a$ by $4$. The remainder $r$ is one of $0,1,2,3$ since $0\le r<4$ and $r$ is an integer. A remainder of $0$ or $2$ would make $p$ a multiple of $2$ and hence $a$ a multiple of $2$, which is impossible because $a=2(2i)+1$ has remainder $1$ on division by $2$. Thus the remainder of $p$ is $1$ or $3$. Uniqueness of the remainder makes these exactly the two corresponding congruence classes modulo $4$. Since $a>0$, failure of membership in $\mathcal A$ is therefore equivalent to having a prime divisor in $\mathcal P_3$. If one exists, [F4] supplies one with $\iota(p)\le\sqrt a$. The real number $\iota(p)$ is nonnegative because $p>1$ and the embedding in [F5] preserves zero and order. Squaring gives $\iota(p)^2\le\iota(a)$ by [F5] and the square-root identity in [F4]. Multiplicativity gives $\iota(p^2)=\iota(p)^2$, so reflection of order gives $p^2\le a$ in the integers. If $p\ge18$, then $p^2\ge18p\ge18^2=324>313\ge a$ by [F6], a contradiction. Thus $1<p<18$. [F2, F3, F4, F5, F6, F7, step 1.1]

3.1 For any divisor $p$ supplied by step 2.1, write $p=4q+3$ for an integer $q$. If $q\le-1$ then $p\le-1$, and if $q\ge4$ then $p\ge19$. The only remaining integer values of $q$ are $0,1,2,3$, which give $p=3,7,11,15$. The number $15=3\cdot5$ is not prime. For $3$ the trial division range is empty since $2^2=4>3$. For $7$ the only test is $2$, since $3^2=9>7$, and $7=2\cdot3+1$. For $11$ the tests are $2$ and $3$, since $4^2=16>11$, and $11=2\cdot5+1=3\cdot3+2$. Thus $3,7,11$ are primes, all congruent to $3$ modulo $4$. Any one of them dividing $a$ prevents $a\in\mathcal A$, and by step 2.1 a failure of membership forces one of them to divide $a$. Therefore $i\in J$ exactly when none of $3,7,11$ divides $4i+1$. [F2, F3, F6, F7, step 1.1, step 2.1]

4.1 For $(p,r)=(3,2),(7,5),(11,8)$ one has $4r+1=3p$ and $p+1=4s$ with $s=1,2,3$, respectively. The identity $a=4(i-r)+3p$ gives $p\mid a$ exactly when $p\mid 4(i-r)$. If $p\mid 4(i-r)$, the identity $i-r=s\cdot4(i-r)-p(i-r)$ gives $p\mid i-r$. Conversely, $p\mid i-r$ gives $p\mid 4(i-r)$ by multiplying by $4$. Thus the indices excluded for each $p$ are exactly the integers of the form $r+pk$ in the allowed range. Since $0\le r<p$, any integer $k\le-1$ gives $r+pk<0$, so only $k\ge0$ is possible. [F3, F6, step 1.1, step 3.1]

5.1 The three lists of excluded indices are $2+3k$ for $0\le k\le25$, $5+7k$ for $0\le k\le10$, and $8+11k$ for $0\le k\le6$, in each case with $k$ an integer. Indeed the last values are $77,75,74$, respectively, and the next values are $80,82,85$, respectively, all greater than $78$. Each list increases with $k$. [F6, step 4.1]

6.1 Within each index range below, the middle column lists the indices in at least one of the three lists in step 5.1. The last column gives $4i+1$ for each index in the range absent from the middle column, in order of increasing $i$.
$$\begin{array}{c|l|l}\text{Index range}&\text{Excluded indices}&\text{Values from retained indices}\\\hline 0\text{ to }9&2,5,8&1,5,13,17,25,29,37\\10\text{ to }19&11,12,14,17,19&41,53,61,65,73\\20\text{ to }29&20,23,26,29&85,89,97,101,109,113\\30\text{ to }39&30,32,33,35,38&125,137,145,149,157\\40\text{ to }49&40,41,44,47&169,173,181,185,193,197\\50\text{ to }59&50,52,53,54,56,59&205,221,229,233\\60\text{ to }69&61,62,63,65,68&241,257,265,269,277\\70\text{ to }78&71,74,75,77&281,289,293,305,313\end{array}$$
The rows cover every integer index from $0$ through $78$. [F6, step 3.1, step 5.1]

7.1 By the divisibility criterion, the retained indices in the table are exactly $J$. Its last column gives precisely the entries of the displayed set in the statement. Since the two sets have the same members, the displayed set equals $\{4i+1:i\in J\}$. [F1, F8, step 3.1, step 4.1, step 6.1] ∎

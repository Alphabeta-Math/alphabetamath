---
title: Numerical comparisons for the analytic threshold
status: draft
research_item: lem-euler-analytic-power-comparisons
dependency_level: 0
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §6, three power comparisons for X at least 64
---

PDF p. 7: ` §6, three power comparisons for X at least 64 `

## Prerequisites

- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)
- [math:cor-of-one-positive](https://alphabetamath.cc/item/cor-of-one-positive)
- [math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)
- [math:lem-rational-power-monotone](https://alphabetamath.cc/item/lem-rational-power-monotone)
- [math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive)
- [math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-rat-positive-denominator](https://alphabetamath.cc/item/lem-rat-positive-denominator)
- [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)
- [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)


## Statement

Let $X$ be a real number with $X\ge64$. Use rational powers for fractional exponents and real division for the fractions on the right. Then
$$X^{-1/5}\le\frac49,\qquad 2^{3/10}<\frac54,\qquad X^{-1}\le\frac1{64}.$$

## Facts & Assumptions

[F1] The real number system [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers) is a totally ordered field by [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field). In an ordered field, $a<b$ means $b-a>0$, $a\le b$ means $a<b$ or $a=b$, and sums and products of positive elements are positive ([math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)).

[F2] In a field, each nonzero $b$ has a unique multiplicative inverse $b^{-1}$, which satisfies $bb^{-1}=1$. Real division is $a/b=ab^{-1}$ for $b\ne0$ ([math:def-field](https://alphabetamath.cc/item/def-field)).

[F3] In an ordered field, $1>0$ ([math:cor-of-one-positive](https://alphabetamath.cc/item/cor-of-one-positive)).

[F4] Integer exponents lie in $\mathbb{Z}$ ([math:def-integers](https://alphabetamath.cc/item/def-integers)), with $k\ge0$ and $k>0$ taken in the integer order ([math:def-int-order](https://alphabetamath.cc/item/def-int-order)). The map $k\mapsto[(k,0)]$ identifies the natural numbers with the nonnegative integers ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)). Integer powers are given by $a^0=1$, $a^{k+1}=a^ka$ for integers $k\ge0$, and $a^{-k}=1/a^k$ for $a\ne0$ and integers $k>0$ ([math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)). A rational exponent is an equivalence class of integer pairs with nonzero denominator, written $m/n$ for the class of $(m,n)$ ([math:def-rationals](https://alphabetamath.cc/item/def-rationals)). Every rational exponent has such a representative with $n>0$ ([math:lem-rat-positive-denominator](https://alphabetamath.cc/item/lem-rat-positive-denominator)). For $a>0$, the rational power $a^{m/n}$ is the $m$th power of the unique positive $t$ with $t^n=a$. This value is independent of the representative $m/n$ and agrees with integer powers for $n=1$ ([math:def-rational-power](https://alphabetamath.cc/item/def-rational-power)).

[F5] For positive real $a,b$ and rational exponents $r,s$, one has $a^r>0$, $(a^r)^s=a^{rs}$, $(ab)^r=a^rb^r$ and $a^{-r}=1/a^r$ ([math:lem-rational-power-laws](https://alphabetamath.cc/item/lem-rational-power-laws)).

[F6] A rational $m/n$ with $n>0$ is positive exactly when $m>0$ in the integer order ([math:def-rat-order](https://alphabetamath.cc/item/def-rat-order), [math:def-int-order](https://alphabetamath.cc/item/def-int-order)). For a fixed rational $r>0$ and positive reals $a<b$, one has $a^r<b^r$ ([math:lem-rational-power-monotone](https://alphabetamath.cc/item/lem-rational-power-monotone), part 2). Thus if $a^r<b^r$ for positive $a,b$, then $a<b$, since $a=b$ gives equal powers and $b<a$ gives the reverse strict inequality.

[F7] In an ordered field, if $a>0$ then $a^{-1}>0$, and if $0<a<b$ then $b^{-1}<a^{-1}$ ([math:lem-of-inverse-positive](https://alphabetamath.cc/item/lem-of-inverse-positive), parts 1 and 2). Including equality gives $b^{-1}\le a^{-1}$ when $0<a\le b$.

[F8] Multiplication by a positive element of an ordered field preserves and reflects strict inequalities ([math:lem-of-sign-rules](https://alphabetamath.cc/item/lem-of-sign-rules), part 4).

[F9] Rational exponent arithmetic uses $(m/n)(p/q)=(mp)/(nq)$ and $-(m/n)=(-m)/n$ for nonzero denominators ([math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)). Two such fractions $m/n$ and $p/q$ are equal exactly when $mq=pn$ ([math:def-rationals](https://alphabetamath.cc/item/def-rationals)). On integer representatives, negation is $-[(a,b)]=[(b,a)]$ and multiplication is $[(a,b)]\cdot[(c,d)]=[(ac+bd,ad+bc)]$ ([math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)). For $k=1,5,10$, these rules give $-1=[(0,1)]$ and $(-1)k=[(0,1)]\cdot[(k,0)]=[(0,k)]=-k$.

## Proof

**Given:** A real number $X\ge64$.

**Goal:** Prove $X^{-1/5}\le4/9$, $2^{3/10}<5/4$ and $X^{-1}\le1/64$.

1.1 The integer numerals $2,4,5,9,64$ are sums of copies of $1>0$, so each is positive. Hence $X>0$. The quotients $4/9$ and $5/4$ are positive because their numerators and the inverses of their denominators are positive. [given, F1, F2, F3, F7]

1.2 The integer numerals $1,5,10$ are positive since their representatives $(1,0),(5,0),(10,0)$ have first entry greater than the second. Thus $5/1$ and $10/1$ are positive rational exponents. [F4, F6]

2.1 Since $0<64\le X$, inversion gives $X^{-1}\le64^{-1}=1/64$. [step 1.1, given, F2, F7]

2.2 The power laws give $(4/9)^5=4^5/9^5$ using $4/9=4\cdot9^{-1}$ and $(9^{-1})^5=9^{-5}=1/9^5$. Here $-(1/1)=(-1)/1$ and $((-1)/1)(5/1)=(-5)/1$, and denominator-one exponents agree with the integer powers. The exact products are $9^5=59049<65536=64\cdot4^5$. Multiplication by the positive number $64\cdot9^5$ therefore shows that $1/64<(4/9)^5$. [step 1.1, F1, F2, F4, F5, F8, F9, algebra]

2.3 The power laws give $(2^{3/10})^{10}=2^3$ and $(5/4)^{10}=5^{10}/4^{10}$ using $(4^{-1})^{10}=4^{-10}=1/4^{10}$. The rational products are $(3/10)(10/1)=30/10=3/1$ and $((-1)/1)(10/1)=(-10)/1$, and denominator-one exponents agree with the integer powers. The exact products are $2^3\cdot4^{10}=8388608<9765625=5^{10}$. Since $4^{10}>0$, this proves $(2^{3/10})^{10}<(5/4)^{10}$. [step 1.1, F2, F4, F5, F8, F9, algebra]

3.1 The positive number $X^{-1/5}$ satisfies $(X^{-1/5})^5=X^{-1}\le1/64<(4/9)^5$. The exponent identity uses $-(1/5)=(-1)/5$, $((-1)/5)(5/1)=(-5)/5=(-1)/1$ and agreement with the integer power. Since the bases $X^{-1/5}$ and $4/9$ are positive and $5/1>0$, the fifth-power comparison gives $X^{-1/5}<4/9$. [step 1.1, step 1.2, step 2.1, step 2.2, F1, F4, F5, F6, F9]

3.2 The bases $2^{3/10}$ and $5/4$ are positive and $10/1>0$. The tenth-power comparison therefore gives $2^{3/10}<5/4$. [step 1.1, step 1.2, step 2.3, F5, F6]

4.1 The fifth-power comparison gives the claimed weak bound $X^{-1/5}\le4/9$. Together with $2^{3/10}<5/4$ and $X^{-1}\le1/64$, this proves all three estimates. [step 3.1, step 3.2, step 2.1, F1] ∎

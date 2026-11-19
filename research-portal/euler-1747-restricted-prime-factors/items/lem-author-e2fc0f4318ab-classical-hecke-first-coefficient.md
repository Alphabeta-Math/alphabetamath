---
id: lem-author-e2fc0f4318ab-classical-hecke-first-coefficient
kind: lemma
title: The first Hecke coefficient of a weight-two cusp form
status: published
domain: mathematics
deps:
  - math:def-unit-group-modulo-n-and-euler-totient
  - math:lem-nat-embeds-int
  - math:def-complex-integer-powers
  - math:def-canonical-natural
  - math:def-countable-choice
  - def-author-e2fc0f4318ab-weight-two-cusp-form
  - def-author-e2fc0f4318ab-normalized-weight-two-newform
  - math:def-prime
  - math:thm-complex-nth-roots-and-roots-of-unity
  - math:thm-complex-exponential-addition-and-real-extension
  - math:cor-uniqueness-of-complex-power-series-coefficients
  - math:def-divides-in-z
  - math:thm-division-algorithm-in-z
  - math:thm-q-expansion-principle-at-the-cusp
  - math:prop-sums-and-scalar-multiples-of-complex-power-series
  - math:def-complex-exponential
  - math:def-complex-series-power-series-and-absolute-convergence
  - math:def-dirichlet-character-modulo-q
  - math:thm-reals-ordered-field
  - math:lem-of-naturals-positive
  - math:thm-complex-numbers-form-a-field
  - math:thm-int-ordered-ring
  - math:lem-power-laws
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-finite-sum-reindexing-and-fubini
  - math:def-complex-metric-convergence-and-continuity
  - math:def-metric-convergence
  - math:thm-cauchy-hadamard-for-complex-power-series
  - math:def-pi-via-first-positive-cosine-zero
  - math:lem-group-homomorphism-basic-properties
  - math:lem-cardinality-of-finite-natural-initial-segment
  - math:def-monoid-finite-product
  - math:thm-induction-principle
formulation_deps:
  - math:def-countable-choice
  - def-author-e2fc0f4318ab-weight-two-cusp-form
  - def-author-e2fc0f4318ab-normalized-weight-two-newform
  - math:def-prime
  - math:def-divides-in-z
  - math:def-complex-exponential
  - math:def-complex-integer-powers
  - math:def-complex-series-power-series-and-absolute-convergence
  - math:def-dirichlet-character-modulo-q
  - math:def-pi-via-first-positive-cosine-zero
argument_deps:
  - math:def-unit-group-modulo-n-and-euler-totient
  - math:lem-nat-embeds-int
  - math:def-complex-integer-powers
  - math:def-canonical-natural
  - math:def-countable-choice
  - math:thm-complex-nth-roots-and-roots-of-unity
  - math:thm-complex-exponential-addition-and-real-extension
  - math:cor-uniqueness-of-complex-power-series-coefficients
  - def-author-e2fc0f4318ab-weight-two-cusp-form
  - def-author-e2fc0f4318ab-normalized-weight-two-newform
  - math:def-prime
  - math:def-divides-in-z
  - math:thm-division-algorithm-in-z
  - math:thm-q-expansion-principle-at-the-cusp
  - math:prop-sums-and-scalar-multiples-of-complex-power-series
  - math:def-complex-exponential
  - math:def-complex-series-power-series-and-absolute-convergence
  - math:def-dirichlet-character-modulo-q
  - math:thm-reals-ordered-field
  - math:lem-of-naturals-positive
  - math:thm-complex-numbers-form-a-field
  - math:thm-int-ordered-ring
  - math:lem-power-laws
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-finite-sum-reindexing-and-fubini
  - math:def-complex-metric-convergence-and-continuity
  - math:def-metric-convergence
  - math:thm-cauchy-hadamard-for-complex-power-series
  - math:def-pi-via-first-positive-cosine-zero
  - math:lem-group-homomorphism-basic-properties
  - math:lem-cardinality-of-finite-natural-initial-segment
  - math:def-monoid-finite-product
  - math:thm-induction-principle
dependency_roles:
  math:def-unit-group-modulo-n-and-euler-totient: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-complex-integer-powers: mathematical-premise
  math:def-canonical-natural: mathematical-premise
  math:def-countable-choice: mathematical-premise
  def-author-e2fc0f4318ab-weight-two-cusp-form: mathematical-premise
  def-author-e2fc0f4318ab-normalized-weight-two-newform: mathematical-premise
  math:def-prime: mathematical-premise
  math:thm-complex-nth-roots-and-roots-of-unity: mathematical-premise
  math:thm-complex-exponential-addition-and-real-extension: mathematical-premise
  math:cor-uniqueness-of-complex-power-series-coefficients: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:thm-q-expansion-principle-at-the-cusp: mathematical-premise
  math:prop-sums-and-scalar-multiples-of-complex-power-series: mathematical-premise
  math:def-complex-exponential: mathematical-premise
  math:def-complex-series-power-series-and-absolute-convergence: mathematical-premise
  math:def-dirichlet-character-modulo-q: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:lem-of-naturals-positive: mathematical-premise
  math:thm-complex-numbers-form-a-field: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:lem-power-laws: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:lem-finite-sum-reindexing-and-fubini: mathematical-premise
  math:def-complex-metric-convergence-and-continuity: mathematical-premise
  math:def-metric-convergence: mathematical-premise
  math:thm-cauchy-hadamard-for-complex-power-series: mathematical-premise
  math:def-pi-via-first-positive-cosine-zero: mathematical-premise
  math:lem-group-homomorphism-basic-properties: mathematical-premise
  math:lem-cardinality-of-finite-natural-initial-segment: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
  math:thm-induction-principle: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Assume countable choice and take a normalized weight-two cuspidal newform $f(z)=\sum_{n\ge1}a_n q^n$ of level $N$ and character $\epsilon$, with $q=\exp(2\pi i z)$ and $a_1=1$. Let $\ell$ be a prime not dividing $N$. Then the scalar of the classical Hecke operator $T_\ell$ on $f$ is $a_\ell$.

## Statement references

[[def-author-e2fc0f4318ab-weight-two-cusp-form|Weight-two cusp forms and their Fourier coefficients]]

[[def-author-e2fc0f4318ab-normalized-weight-two-newform|Newforms and the classical Hecke convention]]

[[math:def-dirichlet-character-modulo-q|Dirichlet characters modulo the level]]

[[math:def-prime|Prime integers]]

[[math:def-divides-in-z|Integer divisibility]]

[[math:def-complex-exponential|Complex exponential]]

[[math:def-pi-via-first-positive-cosine-zero|The constant $\pi$]]

[[math:def-complex-integer-powers|Complex powers with natural exponents]]

[[math:def-complex-series-power-series-and-absolute-convergence|Complex power series]]

## Facts & Assumptions

[F1] The residue class of $1$ is the identity in $(\mathbb Z/N\mathbb Z)^\times$ ([[math:def-unit-group-modulo-n-and-euler-totient]]). The character homomorphism sends it to the identity of $\mathbb C^\times$, which gives $\epsilon(1)=1$ ([[math:def-dirichlet-character-modulo-q]], [[math:lem-group-homomorphism-basic-properties]]). In weight two, the two positive factorizations of the prime $\ell$ are $(1,\ell)$ and $(\ell,1)$. Substituting them in the classical formula and using $\epsilon(1)=1$ gives $(T_\ell f)(z)=\ell^{-1}\sum_{b=0}^{\ell-1}f((z+b)/\ell)+\ell\epsilon(\ell)f(\ell z)$. A normalized newform is an eigenfunction for this operator ([[def-author-e2fc0f4318ab-normalized-weight-two-newform]], [[math:def-prime]], [[math:def-dirichlet-character-modulo-q]]).

[F2] A cusp form is holomorphic, has period one at infinity and tends uniformly to zero as $\operatorname{Im}z\to\infty$. Indeed the translation matrix $\begin{pmatrix}1&1\\0&1\end{pmatrix}\in\Gamma_0(N)$ has lower right entry $1$, so the transformation law and [F1] give $f(z+1)=f(z)$. The vanishing condition for the identity matrix gives the uniform limit. The cusp expansion theorem then gives $f(z)=F(q(z))$ with $F(w)=\sum_{n\ge1}a_n w^n$ convergent for $|w|<1$. Its cusp coordinate $q(z)=\exp(2\pi i z)$ maps $\mathfrak H$ onto the punctured unit disc ([[def-author-e2fc0f4318ab-weight-two-cusp-form]], [[math:thm-q-expansion-principle-at-the-cusp]], [[math:def-dirichlet-character-modulo-q]], [[math:def-complex-exponential]], [[math:def-pi-via-first-positive-cosine-zero]], [[math:def-complex-series-power-series-and-absolute-convergence]]).

[F3] The exponential is multiplicative under addition in the exponent ([[math:thm-complex-exponential-addition-and-real-extension]]). The natural-to-integer embedding $\iota$ identifies $\mathbb N$ with the nonnegative integers in order and preserves addition and multiplication ([[math:lem-nat-embeds-int]]). For the prime $\ell$, take the unique natural $L$ with $\iota(L)=\ell$. In real and complex field expressions $\ell$ denotes the canonical real numeral of $L$, using the embedded real field in $\mathbb C$. This numeral is positive in $\mathbb R$ and nonzero in $\mathbb C$ ([[math:def-canonical-natural]], [[math:thm-reals-ordered-field]], [[math:lem-of-naturals-positive]], [[math:thm-complex-numbers-form-a-field]]). Set $\zeta=\exp(2\pi i/\ell)$. The $L$th roots of unity are the distinct numbers $\exp(2\pi i k/\ell)$ for natural $0\le k<L$, with $k$ read as its canonical real numeral in the exponent ([[math:def-complex-exponential]], [[math:def-pi-via-first-positive-cosine-zero]], [[math:thm-complex-nth-roots-and-roots-of-unity]]). A nonnegative integer used as a complex power exponent acts by its unique natural preimage ([[math:def-complex-integer-powers]]).

[F4] Integer divisibility $\ell\mid n$ means $n=\ell j$ for some integer $j$. Since $\ell>0$, the division algorithm gives $n=\ell j+r$ with $0\le r<\ell$, and $r=0$ exactly when $\ell\mid n$. Integer inequalities are compatible with addition and multiplication by a positive integer ([[math:def-divides-in-z]], [[math:thm-division-algorithm-in-z]], [[math:thm-int-ordered-ring]]).

[F5] A linear combination of two complex power series about the same centre is represented coefficientwise on their common open disc of convergence ([[math:prop-sums-and-scalar-multiples-of-complex-power-series]]).

[F6] Two convergent power series that represent the same function on a neighbourhood of their common centre have equal coefficients ([[math:cor-uniqueness-of-complex-power-series-coefficients]]).

[F7] In the complex field the natural power laws are $x^{j+k}=x^j x^k$, $(x^j)^k=x^{jk}$ and $(xy)^k=x^k y^k$. The field power laws apply with the complex power convention because both natural powers use the same recursion $x^0=1$ and $x^{k+1}=x^kx$ ([[math:thm-complex-numbers-form-a-field]], [[math:lem-power-laws]], [[math:def-complex-integer-powers]]).

[F8] Finite sums in the additive commutative monoid of $\mathbb C$ are invariant under bijections of their index sets. A sum over a disjoint union splits into the sums over its parts, and a sum of terms that are all zero is zero by the finite-sum definition ([[math:thm-complex-numbers-form-a-field]], [[math:def-finite-sum-in-a-commutative-monoid]], [[math:lem-finite-sum-reindexing-and-fubini]]).

[F9] Convergence of a complex power series means convergence of its ordinary partial sums in $d_{\mathbb C}(x,y)=|x-y|$. Given a positive rational tolerance, all partial sums with sufficiently large cutoff are within that tolerance of the limit ([[math:def-complex-series-power-series-and-absolute-convergence]], [[math:def-complex-metric-convergence-and-continuity]], [[math:def-metric-convergence]]).

[F10] A complex power series diverges outside its radius of convergence, so convergence throughout the open unit disc implies radius at least $1$ ([[math:thm-cauchy-hadamard-for-complex-power-series]]).

[F11] The finite initial segment $I_L=\{b\in\mathbb N:b<L\}$ has cardinality $L$ ([[math:lem-cardinality-of-finite-natural-initial-segment]]). In its natural enumeration the finite complex sum uses the recursion $P_0=0$ and $P_{j+1}=P_j+x_j$ for the list $(x_b)_{b\in I_L}$ ([[math:def-finite-sum-in-a-commutative-monoid]], [[math:def-monoid-finite-product]]).

[F12] For real $a>0$ and $c\in\mathbb R$, the map $v\mapsto av+c$ takes $\mathfrak H$ into itself. It is the fractional linear map of $\begin{pmatrix}a&c\\0&1\end{pmatrix}$, whose determinant is $a>0$, so the upper half-plane calculation in the cusp-form definition applies ([[def-author-e2fc0f4318ab-weight-two-cusp-form]]).

[F13] If a property of natural numbers holds at zero and passes from each natural number to its successor, it holds for every natural number ([[math:thm-induction-principle]]).

## Proof

**Given:** Countable choice, the normalized newform $f$ and the good prime $\ell$.

**Goal:** Identify its classical Hecke eigenvalue with its Fourier coefficient $a_\ell$.

1.1 At $k=0$ the root formula in [F3] gives $\exp(0)^L=1$. Since $L>0$, the natural power recursion in [F7] gives $0^L=0$, so $\exp(0)\ne0$. The addition law gives $\exp(0)=\exp(0)^2$, and cancellation gives $\exp(0)=1$. Write $\nu(r)$ for the canonical real numeral of a natural $r$ embedded in $\mathbb C$. Fix $w\in\mathbb C$. To show $\exp(\nu(r)w)=\exp(w)^r$ by induction on $r$, first note that $\nu(0)=0$, so both sides are $1$ at $r=0$. For the successor, $\nu(r+1)=\nu(r)+1$ by the canonical-natural recursion. Thus $\exp(\nu(r+1)w)=\exp(\nu(r)w)\exp(w)=\exp(w)^r\exp(w)=\exp(w)^{r+1}$ by the addition law, the induction hypothesis and the power recursion. By [F13] the identity holds for every natural $r$. With $w=2\pi i/\ell$ it gives $\exp(2\pi i k/\ell)=\zeta^k$, so the powers $\zeta^k$ for $0\le k<L$ are the distinct $L$th roots from [F3]. [F3, F7, F13]

1.2 Fix a complex scalar $c$ and a complex list $(x_b)_{b\in I_L}$. If $P_j$ and $Q_j$ are the partial sums of $x_b$ and $cx_b$, then $cP_0=Q_0=0$ and $cP_{j+1}=cP_j+cx_j$ by distributivity. The uniqueness of the finite-sum recursion therefore gives $Q_j=cP_j$ for every $0\le j\le L$. [F7, F11]

2.1 For natural $0\le b<L$, read $b$ as its canonical real numeral in the affine maps. The maps $v\mapsto v/\ell$, $v\mapsto (v+b)/\ell$ and $v\mapsto v+b/\ell$ all preserve $\mathfrak H$ by [F12] since $1/\ell>0$ by [F3]. For $z\in\mathfrak H$ put $t=q(z/\ell)$. By step 1.1 and the exponential addition law, $q((z+b)/\ell)=\exp(2\pi i b/\ell)t=\zeta^b t$ for natural $0\le b<L$. Applying step 1.1 with $r=L$ and $w=2\pi i z/\ell$ gives $t^L=q(z)$. The power laws give $(\zeta^b t)^n=\zeta^{bn}t^n$. Each shifted function is thus represented by the power series $\sum_{n\ge1}a_n\zeta^{bn}t^n$ in the same variable $t$. These series converge for $|t|<1$. If $0<|t|<1$, write $t=q(w)$ for some $w\in\mathfrak H$ by [F2]. Then $\zeta^b t=q(w+b/\ell)$ lies in the punctured unit disc since $w+b/\ell\in\mathfrak H$ by the same affine-map check. At $t=0$ each series is zero. [F2, F3, F7, F12, step 1.1]

2.2 Divide the integer $\iota(n)$ as $\iota(n)=\ell j+r$ with $0\le r<\ell$. If $j\le-1$, then $\iota(n)\le-\ell+r<0$, which contradicts $n\ge1$. Taking natural preimages gives $n=Lh+k$ with $h\ge0$ and $0\le k<L$. Since $\zeta^L=1$, the power laws give $\zeta^n=(\zeta^L)^h\zeta^k=\zeta^k$. Distinctness of the first $L$ powers then gives $\zeta^n=1$ exactly when $k=0$, equivalently $\ell\mid\iota(n)$. [F3, F4, F7, step 1.1]

3.1 For $b\in I_L$ denote the series from step 2.1 by $H_b(t)=\sum_{n\ge0}x_{b,n}t^n$, where $x_{b,0}=0$ and $x_{b,n}=a_n\zeta^{bn}$ for $n\ge1$. Each has radius at least $1$ by [F10]. For $0\le j\le L$ put $U_j(t)=\sum_{0\le b<j}H_b(t)$ and $d_{j,n}=\sum_{0\le b<j}x_{b,n}$. Induct using [F13] on the assertion that whenever $j\le L$, the series $\sum_{n\ge0}d_{j,n}t^n$ has radius at least $1$ and represents $U_j(t)$ throughout $|t|<1$. At $j=0$ both sums over $b$ are empty, so the zero series represents $U_0=0$ and has radius at least $1$ by [F10]. If $j+1\le L$, the finite-sum recursion gives $U_{j+1}=U_j+H_j$ and $d_{j+1,n}=d_{j,n}+x_{j,n}$. The induction hypothesis and the radius bound for $H_j$ give a common disc containing $|t|<1$. Applying [F5] to these two series gives the required representation with coefficient $d_{j+1,n}$. Convergence throughout $|t|<1$ gives radius at least $1$ by [F10]. At $j=L$ and $n\ge1$ the coefficient is $\sum_{b\in I_L}a_n\zeta^{bn}$. By step 1.2 this is $a_n\sum_{b\in I_L}\zeta^{bn}$. Scaling the series by $\ell^{-1}$ as in [F1] gives the averaged coefficient $a_n S_n$, where $S_n=\ell^{-1}\sum_{b\in I_L}\zeta^{bn}$. [F1, F5, F8, F10, F11, F13, step 2.1, step 1.2]

3.2 The dilation $z\mapsto\ell z$ preserves $\mathfrak H$ by [F12] since $\ell>0$ by [F3]. Applying step 1.1 with $r=L$ and $w=2\pi i z$ gives $q(\ell z)=q(z)^L$. For each $q$ in the punctured disc, take a preimage $z\in\mathfrak H$. Then $\ell z\in\mathfrak H$, so $|q^L|<1$, which also holds at $q=0$. Define $c_{Ln}=a_n$ for natural $n\ge1$ and $c_m=0$ at every other degree $m$. For each natural $M$ write $M=LJ+k$ with $0\le k<L$ by [F4] and the natural embedding as in step 2.2. The remainder bound gives $LJ\le M<L(J+1)$. Since multiplication by $L>0$ preserves strict order, $n\mapsto Ln$ is a bijection from $\{1,\ldots,J\}$ onto the positive multiples of $L$ at most $M$. Splitting off the zero terms and reindexing by this bijection using [F8] gives $\sum_{m=0}^M c_mq^m=\sum_{n=1}^J a_n(q^L)^n$. For any positive rational tolerance, the right-hand partial sum satisfies the bound relative to $F(q^L)$ whenever $J\ge K$ for some $K$. The bound therefore holds on the left whenever $M\ge LK$, since $J<K$ would give $M=LJ+k<LK$. By [F9], $B(q)=\sum_{m\ge0}c_mq^m$ converges to $F(q^L)$ on the unit disc. Its degree-one coefficient is zero because $L>1$. [F2, F3, F4, F7, F8, F9, F12, step 1.1, step 2.2]

4.1 Put $u=\zeta^n$. If $u=1$, the sum defining $S_n$ adds $L$ copies of $1$ by [F11]. The resulting sum is $\ell$ by the canonical-natural recursion in the real field and its embedding in $\mathbb C$, so $S_n=\ell^{-1}\ell=1$. Otherwise $u^L=(\zeta^L)^n=1$ and $\zeta^{bn}=u^b$. Multiplying by $u$ replaces $u^b$ by $u^{b+1}$. The map sending $b$ to $b+1$ for $0\le b<L-1$ and sending $L-1$ to $0$ is a bijection of $\{0,\ldots,L-1\}$. Each $1\le b<L$ has preimage $b-1$, and $0$ has preimage $L-1$. At the wrap we have $u^L=u^0=1$. By step 1.2 and commutativity in the complex field, $uS_n=\ell^{-1}\sum_{b\in I_L}u^{b+1}$. Reindexing by this permutation using [F8] gives $uS_n=S_n$. Since $1-u\ne0$ in the field, $(1-u)S_n=0$ gives $S_n=0$. [F3, F7, F8, F11, step 1.2, step 3.1]

5.1 The surviving positive indices are $n=Lj$ with natural $j\ge1$. For every $q$ with $0<|q|<1$, choose $z\in\mathfrak H$ with $q(z)=q$ by [F2]. Since $z\mapsto z/\ell$ preserves $\mathfrak H$ by step 2.1, put $t=q(z/\ell)$. Let $P_M(t)$ be the partial sum through degree $M$ of the averaged series and let $s$ be its sum at $t$. For each natural $J$, the map $j\mapsto Lj$ from $\{1,\ldots,J\}$ is a bijection onto the surviving positive indices up to $LJ$, since $L>0$ and $Lj\le LJ$ exactly when $j\le J$. Splitting off the zero terms and reindexing by this bijection using [F8], then using $t^L=q$, gives $P_{LJ}(t)=\sum_{j=1}^J a_{Lj}q^j$. For each positive rational $\eta$, choose $K$ so that $|P_M(t)-s|<\eta$ for all $M\ge K$. Since $LJ\ge J$, this bound holds at $M=LJ$ for every $J\ge K$. Thus $A(q)=\sum_{j\ge1}a_{Lj}q^j$ converges and represents the first term of [F1] on the punctured disc. It converges to zero at $q=0$. [F1, F2, F4, F7, F8, F9, step 2.1, step 3.1, step 2.2, step 4.1]

6.1 The second term in [F1] is $\ell\epsilon(\ell)B(q)$ at $q=q(z)$. $A$, $B$ and $F$ converge throughout the unit disc and thus have radius at least $1$. By [F5] the power series for $A(q)+\ell\epsilon(\ell)B(q)$ has degree-one coefficient $a_L=a_\ell$, where $\ell$ has natural representative $L$. Write $T_\ell f=\lambda f$ by [F1]. Surjectivity of the cusp coordinate gives equality of this sum with $\lambda F(q)$ on the punctured unit disc, and both sides have value zero at $q=0$. By [F5], the series for $\lambda F(q)$ has coefficient $\lambda a_1$ at degree one. They represent the same function on the unit disc, so [F6] gives $a_\ell=\lambda a_1=\lambda$. [F1, F2, F3, F5, F6, F10, step 5.1, step 3.2, given] ∎

---
title: Open questions and potential solutions
research_report: open-questions
description: Insights, fruitful questions and potential solutions arising from
  Euler’s 1747 conjecture on sums of integers with restricted prime factors.
status: draft
generated_at: 2026-11-19T15:50:22.081Z
---

## 1. Research insights beyond the article

### Research insight 01 · A uniform lower bound for the surviving four-square fraction

#### Insight

**Kind:** corollary

**Evidence status:** proved

Work in ZFC. For positive $n\equiv2\pmod4$, let $R(n)$ count all ordered integer quadruples with square sum $n$, with zero and both signs allowed. Let $\mathcal A$ consist of the positive integers whose prime divisors are all $1\pmod4$, including $1$. Let $G(n)$ count the quadruples in which each of the two coordinate pairs has opposite parity and both pair norms belong to $\mathcal A$. Let $D(n)$ count ordered pairs $(a,b)\in\mathcal A^2$ with $a+b=n$. Put $S=2\sum_{p\equiv3\pmod4}1/[p(p-1)]$ and $K_\eta=\prod_{\ell<2^{1/\eta}}(1-\ell^{-\eta})^{-2}$, with the sum and product over primes. For every $0<\eta<1/4$ and every $n\ge81$ in the progression, $G(n)/R(n)\ge2/3-S-4K_\eta n^{-1/4+\eta}$. The liminf along the progression is at least $2/3-S>37/150$. For every $\epsilon>0$, set $\eta=\min\{\epsilon/2,1/8\}$, $c_\epsilon=37/(400K_\eta^2)$, and $N_\epsilon=\max\{81,\lceil(1200K_\eta/37)^{1/(1/4-\eta)}\rceil\}$. Then $D(n)\ge c_\epsilon n^{1-\epsilon}$ for every $n\ge N_\epsilon$ in the progression.

#### Why it matters

Lemma 2.1 of the article transports an admissible decomposition by scaling. Counting at the original input gives a lower bound on the fraction of all four-square representations with admissible pair norms. Bounding the number of quadruples over each pair of norms also gives a lower bound on the number of distinct ordered decompositions.

#### Originality

Howe, Huffman, Kohlmeyer and Kruer prove existence and carry out their explicit analytic estimate after reducing $m=n/2$. The eight-page version does not state the full-progression fraction with an explicit error or the effective lower bound for ordered decompositions. Lucia’s 2013 MathOverflow answer reports an asymptotic weighted lower bound on the full progression with normalized main coefficient $(2/3)(1-S)$, using $R(n)=24\sigma(n/2)$. The near-linear exponent for the ordered count already follows from Dietmann and Elsholtz’s equation (1) and the deletion estimate in their MathOverflow account. Their paper identifies the threshold in its Greaves-based argument as ineffective. The contribution here is the explicit finite error in the spectral estimate and the resulting explicit constants for the unweighted count. Priority for that precise estimate remains undetermined.

#### Current knowledge

The proof combines the checked sieve estimates at their stated hypotheses and derives the divisor bound, cutoff error, and fiber estimate explicitly. The historical comparisons are independent of the proof.

#### Argument and next steps

Apply the torus-normalizer estimate at the original index $m$ for primes coprime to $m$ and the coordinate-division estimate for primes dividing $m$. Sum the obstruction bounds using the cutoff $n^{1/4}$ and subtract them from the mixed-parity fraction $2/3$. The fibers of the ordered pair-norm map have size at most $16K_\eta^2n^{2\eta}$, which gives the stated effective count.

#### Proof sketch or overall strategy

Use the per-prime sieve bounds at the original odd index, sum them at the cutoff $n^{1/4}$ with an explicit divisor bound, and count the fibers of the pair-norm map.

#### Numbered argument

1. Write $n=2m$ with $m$ positive and odd. Jacobi’s formula gives $R(n)=24\sigma(m)\ge12n$ since $m$ is one of its positive divisors. Exactly two coordinates are odd because squares are $0$ or $1$ modulo $4$. Coordinate permutations biject the six placements of the two odd coordinates, and four placements give opposite parity in both pairs. The mixed-parity count is therefore $2R(n)/3$. Each mixed pair has positive odd norm. For $p\in\mathcal P_3$, such a norm is divisible by $p$ exactly when both entries are divisible by $p$, by the nonsplit-square obstruction and the immediate converse. Removing the exceptional sets counted by $b_p(n)$ therefore leaves exactly the quadruples counted by $G(n)$. [counting-conventions, thm-jacobi-signed-ordered-four-square-count, lem-euler-nonsplit-square-obstruction]
2. If $p\in\mathcal P_3$ and $p\nmid m$, every prime dividing $m$ lies outside $\{2,p\}$. The Hamilton algebra splits there and the Hecke action uses the full local level. Choice is in force. At the same fixed projective reduction, combine $b_p(n)\le8(T_m f_p)(\Gamma_p)$ with the averaged bound and divide by $24\sigma(m)$. This gives $b_p(n)/R(n)\le\mu_p/3+\tau(m)\sqrt m(1-\mu_p)/(3\sigma(m))$. Here $\mu_p=6/[p(p-1)]$, so the error vanishes at $p=3$ and $1-\mu_p\le1$ otherwise. For $p\mid m$, the dividing-prime estimate gives $b_p(n)/R(n)\le2/(3p^2)\le2/[p(p-1)]$. Thus for every $p\in\mathcal P_3$ one has $b_p(n)/R(n)\le2/[p(p-1)]+\mathbf{1}_{p>3}\tau(m)\sqrt m/(3\sigma(m))$. [step:1, math:def-axiom-of-choice, lem-euler-hurwitz-sieve-domination, lem-euler-hurwitz-averaged-spectral-bound, lem-euler-hurwitz-normalizer-orbit-size, lem-euler-obstruction-dividing-prime-density]
3. For each positive integer $u=\prod_\ell\ell^{e_\ell}$, independent choices of divisor exponents give $\tau(u)=\prod_{\ell:e_\ell>0}(e_\ell+1)$. If $\ell\ge2^{1/\eta}$, then $e+1\le2^e\le\ell^{\eta e}$ for every integer $e\ge0$. For a smaller prime, positivity and the square of the convergent geometric series give $(e+1)\ell^{-\eta e}\le\sum_{j\ge0}(j+1)\ell^{-\eta j}=(1-\ell^{-\eta})^{-2}$. Multiplying the bounds gives $\tau(u)\le K_\eta u^\eta$, including the empty factorization at $u=1$. The product in the definition of $M(n)$ uses a subset of the divisor factors for each $1\le u\le n$. Hence $M(n)\le K_\eta n^\eta$. [counting-conventions, math:thm-fundamental-theorem-of-arithmetic]
4. For $n\ge81$ put $P=n^{1/4}\ge3$. There are at most $P$ primes at or below $P$. By Step 2, the sum of their normalized obstructions is at most $S+P\tau(m)\sqrt m/(3\sigma(m))\le S+(\sqrt2/3)K_\eta n^{-1/4+\eta}$, using $\sigma(m)\ge m$, $m=n/2$, and Step 3. For $p>P$, use $b_p(n)\le16M(n)(n/p^2+1)$ and the vanishing for $p>\sqrt n$. Dividing by $R(n)\ge12n$ bounds the large-prime sum by $(4/3)M(n)(1/\lfloor P\rfloor+n^{-1/2})$. Indeed, $k^{-2}\le1/[k(k-1)]$ for integers $k>P$, and the latter terms telescope to $1/\lfloor P\rfloor$. At most $\sqrt n$ primes contribute the constant term. Since $\lfloor P\rfloor\ge2P/3$ and $n^{-1/2}\le1/P$, the large-prime bound is at most $(10/3)K_\eta n^{-1/4+\eta}$. [step:1, step:2, step:3, lem-euler-large-prime-obstruction-per-prime, lem-euler-obstructing-prime-density-sum]
5. The union bound in Step 1 gives $G(n)/R(n)\ge2/3-\sum_{p\in\mathcal P_3}b_p(n)/R(n)$. Only finitely many primes contribute by Step 4. Since $(10+\sqrt2)/3<4$, Step 4 gives the claimed finite bound. For fixed $0<\eta<1/4$ the error tends to zero, and $S<21/50$ gives $\liminf G(n)/R(n)\ge2/3-S>37/150$ along the progression. [step:1, step:4, lem-euler-obstructing-prime-density-sum]
6. Map each surviving quadruple to its ordered pair of norms $(a,b)$. Both norms are odd, so every two-square representation of either norm has opposite parity. The fiber over each admissible ordered decomposition has size $r_2(a)r_2(b)\le16M(n)^2$ because $1\le a,b\le n$. With $\eta$ and $N_\epsilon$ from the statement, $n\ge N_\epsilon$ ensures $4K_\eta n^{-1/4+\eta}\le37/300$. Step 5 gives $G(n)\ge(37/300)R(n)$. Using $R(n)\ge12n$ and Step 3 yields $D(n)\ge G(n)/(16M(n)^2)\ge[37/(400K_\eta^2)]n^{1-2\eta}\ge c_\epsilon n^{1-\epsilon}$, since $2\eta\le\epsilon$. [counting-conventions, step:1, step:3, step:5, lem-euler-two-square-count-bound]

#### Immediate dependencies

- **counting-conventions:** Use the counts $R,G,D$ and the set $\mathcal A$ in the statement. Write $m=n/2$, and let $\mathcal P_3$ be the primes $3\pmod4$. The count $b_p(n)$ includes each mixed-parity quadruple with both entries of at least one pair divisible by $p$ once. Write $\sigma(u)$ and $\tau(u)$ for the sum and number of positive divisors of $u$, and $r_2(u)$ for the signed ordered two-square count. Set $M(n)=\max_{1\le u\le n}\prod_{q\equiv1\pmod4,\ e_q>0}(e_q+1)$, where $q$ is prime and $e_q$ is its exact exponent in $u$. Source: self-contained; Statement and proof notation. Reading limits: Matched the conventions to the immediate frozen counting lemmas.
- **math:def-axiom-of-choice:** Every family of nonempty sets has a choice function. ZFC includes this axiom, which is an explicit hypothesis of the spectral supplier. Source: math:def-axiom-of-choice; Definition. Reading limits: Read the published definition and checked the explicit hypothesis in the averaged spectral bound.
- **thm-jacobi-signed-ordered-four-square-count:** For every positive integer $u$, the number of ordered integer quadruples of square sum $u$ is $8(2+(-1)^u)\sigma(\operatorname{Od}(u))$, where $\operatorname{Od}(u)$ is the odd part of $u$. Source: thm-jacobi-signed-ordered-four-square-count; Statement and External input. Ewell, p. 224, §1, Theorem 1 and preceding definitions.. Reading limits: Checked the local interface, Theorem 1 and definitions on p. 224, and the coefficient formulas on p. 228.
- **lem-euler-nonsplit-square-obstruction:** If $p\equiv3\pmod4$ is prime and $p\mid x^2+y^2$ for integers $x,y$, then $p\mid x$ and $p\mid y$. Source: lem-euler-nonsplit-square-obstruction; Statement and Proof 3.2–6.1. Reading limits: Checked the use of the quadratic nonresidue of $-1$ and the field argument.
- **lem-euler-hurwitz-sieve-domination:** For positive odd $m$, $n=2m$, and a prime $p\equiv3\pmod4$ with $p\nmid m$, one has $b_p(n)\le8(T_m f_p)(\Gamma_p)$. The operator is the Hurwitz norm-shell operator and $f_p$ is the torus-normalizer orbit indicator at the fixed projective reduction. Source: lem-euler-hurwitz-sieve-domination; Statement and Proof 1.1–2.1, corresponding to (3.6). Reading limits: Checked the norm-shell preimage and the count of eight eligible elements per contributing left-unit class.
- **lem-euler-hurwitz-averaged-spectral-bound:** Under Choice, for positive odd $m$ and a prime $p\equiv3\pmod4$ with $p\nmid m$, the same operator and orbit give $(T_m f_p)(\Gamma_p)\le\sigma(m)\mu_p+\tau(m)\sqrt m(1-\mu_p)$, where $\mu_p$ is the orbit density. Source: lem-euler-hurwitz-averaged-spectral-bound; Statement and Proof 3.1–5.1. Index and level conditions in lem-euler-hurwitz-hecke-spectral-bound, Facts [F1], [F6] and Proof 3.2 and 12.1.. Reading limits: Checked the centered-indicator application and the underlying operator’s odd-index, coprimality and full-local-level conditions. Used the automorphic spectral estimate at its stated interface.
- **lem-euler-hurwitz-normalizer-orbit-size:** For a prime $p\equiv3\pmod4$, the orbit density at the fixed reduction is $\mu_p=6/[p(p-1)]$, including $\mu_3=1$. Source: lem-euler-hurwitz-normalizer-orbit-size; Statement and Proof 2.1–4.1. Reading limits: Checked the orbit–stabilizer calculation and division by the ambient coset count.
- **lem-euler-obstruction-dividing-prime-density:** For positive odd $m$ and a prime $p\equiv3\pmod4$ dividing $m$, one has $b_p(2m)/R(2m)\le2/(3p^2)$. The count is zero if $p^2\nmid m$ and is $16\sigma(m/p^2)$ otherwise. Source: lem-euler-obstruction-dividing-prime-density; Statement and Proof 2.1–6.1. Exact count in lem-euler-obstruction-at-dividing-prime, Proof 1.2–5.1.. Reading limits: Checked the divide-by-$p$ bijection, preservation of mixed parity, and cancellation of the coprime factor in the divisor-sum ratio.
- **math:thm-fundamental-theorem-of-arithmetic:** Every integer $u\ge1$ has a prime factorization unique up to order, with the empty factorization for $1$. Source: math:thm-fundamental-theorem-of-arithmetic; Statement, clauses 1–2. Reading limits: Checked the published existence and uniqueness clauses used to enumerate divisor exponents.
- **lem-euler-large-prime-obstruction-per-prime:** For positive odd $m$, $n=2m$, and $p\in\mathcal P_3$, one has $b_p(n)\le16M(n)(n/p^2+1)$, with $b_p(n)=0$ for $p>\sqrt n$. Source: lem-euler-large-prime-obstruction-per-prime; Statement and Proof 2.1–6.1. Reading limits: Checked the count in each obstructed position, the positive norm of the other pair, and the support bound.
- **lem-euler-obstructing-prime-density-sum:** The series $S=2\sum_{p\in\mathcal P_3}1/[p(p-1)]$ converges and satisfies $S<21/50$. Source: lem-euler-obstructing-prime-density-sum; Statement and Proof 1.1–4.1, corresponding to (5.4). Reading limits: Checked the finite prime list and tail comparison and verified the strict rational bound.
- **lem-euler-two-square-count-bound:** For integers $1\le u\le n$, the signed ordered two-square count satisfies $r_2(u)\le4M(n)$, including representations with a zero entry. Source: lem-euler-two-square-count-bound; Statement and Proof 1.1–2.1. Reading limits: Checked the two cases of the prime-exponent count and the range of the maximum.

#### Independent review

**Decision:** repair

Step 3 contained a U+0000 character inside the exponent of the geometric-series bound. The repair gives the valid identity and states the explicit counting constants. The Hecke bound applies at the original index because every prime dividing that index is odd and differs from the sieving prime. The remaining cases and both cutoff estimates give the stated coefficient. The historical comparison now identifies the stronger asymptotic coefficient reported by Lucia.

**Dependency review:** The immediate suppliers agree on signed ordered counts, mixed parity, and the fixed projective reduction and Hecke normalization. The coprime-prime estimate accepts every positive odd index coprime to the sieving prime under Choice, and the dividing-prime estimate covers the complementary case. The large-prime count and two-square fiber bound apply over the full progression. I found no declared dependency cycle in the reachable graph or circular use in the checked argument. The article serves as attribution and historical comparison. Ewell supplies Jacobi’s formula independently.

**Review reading limits:** I read the frozen eight-page article text and checked the displayed Hecke and orbit-average formulas on PDF pages 3–4. I checked the immediate frozen suppliers, the index and level conditions in the underlying spectral lemma, Ewell’s Theorem 1 and concluding coefficient formulas, Dietmann and Elsholtz’s equation (1) and concluding remarks, and the relevant MathOverflow passages. I used the local spectral estimate at its stated interface. Reconstructing its full automorphic proof and verifying the analytic arguments behind the historical comparisons were outside the review scope. The targeted literature comparison leaves priority for the explicit estimate undetermined.

#### Author and reviewer gaps

No remaining gaps were reported within the stated scope.

#### Remaining gaps

The bound leaves the optimal surviving fraction and a logarithmic-scale estimate for $D(n)$ undetermined. The proof uses the frozen local spectral estimate at its stated interface. The historical comparison covers the cited passages and a targeted search.

#### Sources

- Euler’s 1747 conjecture on sums of integers with restricted prime factors: https://hexagonmath.org/pdf/2611.00370v1; p. 1, §1, opening definitions; p. 1, Abstract and §1, opening paragraph; p. 1, §1, definition of admissible summands and Euler formulation, p. 1, Lemma 2.1, scaling step; p. 1, §1, Letter 115 and editorial note 10, p. 8, Reference [4]; p. 1, §1, Euler’s divisor condition and the definition of admissible summands; p. 1, §1, prior result of Dietmann and Elsholtz, p. 8, Reference [2]; p. 1, Abstract and Theorem 1.1, p. 8, Proof of Theorem 1.1; p. 1, §2, first sentence; p. 1, Lemma 2.1, first sentence of the proof; p. 1, Lemma 2.1, statement and scaling step; p. 2, §2, definition preceding (2.1) and notation in (2.1); p. 2, §2, equation (2.1); p. 2, §2, text between (2.1) and (2.2); p. 2, §2, definition of the mixed set preceding (2.2); p. 2, §2, equation (2.2); p. 2, §2, definition of the exceptional sets following (2.2); p. 2, §2, quadratic nonresidue observation preceding (2.3); p. 2, §2, conclusion immediately preceding (2.3); p. 2, §2, equation (2.3), p. 7, §6, application of (2.2) and (2.3); p. 2, §3.1, Hamilton algebra and reduced norm; p. 2, §3.1, displayed definition of the order; p. 2, §3.1, enumeration of units; p. 2, §3.1, rounding and the strict norm bound; p. 2, §3.1, consequence of norm-Euclidean division; p. 2, §3.1, definition of the norm shell preceding (3.2); p. 2, §3.1, equation (3.2) and inverse description; p. 2, §3.1, last paragraph; p. 2, §3.1, definitions of the projective group and reduction, p. 3, §3.1, definitions of the unit image, quotient, and counting inner product; p. 3, §3.1, scalar reductions and equation (3.3); p. 3, §3.2, equation (3.4); p. 3, §3.2, first three claims following (3.4); p. 3, §3.2, constant eigenvalue following (3.4); p. 3, §3.2, definition of the character before Lemma 3.2; p. 3, §3.2, justification of the definition of the determinant character; p. 3, §3.2, character eigenvalue before Lemma 3.2; p. 3, Lemma 3.2, proof, definition of the compact open level; p. 3, Lemma 3.2, equation (3.5) and stabilizer paragraph; p. 3, Lemma 3.2, paragraph following the stabilizer description; p. 3, Lemma 3.2, paragraph on one-dimensional automorphic representations; p. 3, Lemma 3.2, invocation of Jacquet–Langlands and the weight-two setting, p. 8, References [3] and [5]; p. 3, Lemma 3.2, opening of the Ramanujan–Petersson paragraph, p. 8, Reference [1]; p. 3, Lemma 3.2, displayed local eigenvalue and triangular-coset calculation; p. 3, Lemma 3.2, last paragraph, local bound before multiplication; p. 3, Lemma 3.2, statement and last sentence of its proof; p. 4, §3.3, opening definitions of the two subgroups; p. 4, §3.3, order assertion immediately following the subgroup definitions; p. 4, §3.3, description of pair vanishing and multiplication by 1 + i; p. 4, §3.3, unit-image intersection preceding the orbit definition; p. 4, §3.3, displayed orbit and indicator definitions; p. 4, §3.3, density formula, orbit count, and the case $p = 3$; p. 4, §3.3, class multiplicity preceding (3.6); p. 4, §3.3, equation (3.6); p. 4, §3.3, invariance and equation (3.7); p. 4, §3.3, norm surjectivity and balance paragraph following (3.7); p. 4, §3.3, centered indicator and its norm before (3.8); p. 4, §3.3, equation (3.8) and case $p = 3$; p. 4, Completion of Proposition 3.1, formula for the dividing-prime obstruction count; p. 4, Completion of Proposition 3.1, divisor-sum ratio and last inequality; p. 2, Proposition 3.1, equation (3.1), p. 4, §3.3 and completion of Proposition 3.1; p. 4, §4, definition preceding Lemma 4.1; p. 4, Lemma 4.1, proof, orbit representatives, label and norm identity; p. 4, Lemma 4.1, statement and last two lines; p. 5, §4, definitions of M(n) and r₂(u) on the first lines; p. 5, §4, two-square formula application before Lemma 4.2; p. 5, Lemma 4.2, proof, per-prime count and upper limit on the prime; p. 5, Lemma 4.2, last line of proof; p. 5, Lemma 4.2, equation (4.1); p. 5, Lemma 5.1, first two proof paragraphs before the table; p. 5, Lemma 5.1, ratio test and table of maximizing positive exponents; p. 5, Lemma 5.1, absent-prime convention and displayed fifth-power products; p. 5, Lemma 5.1, equation (5.1); p. 6, Lemma 5.2, definition of the residue set and counting function; p. 6, Lemma 5.2, first sentence of proof; p. 6, Lemma 5.2, one-period check and interval estimate; p. 6, Lemma 5.2, equation (5.2); p. 6, Lemma 5.2, displayed partial-summation identity and upper bound; p. 6, Lemma 5.2, equation (5.3); p. 6, Lemma 5.2, equation (5.4) and final finite sum through 60; p. 6, Proposition 6.1, choice of cutoff and equation (6.1); p. 6, Proposition 6.1, equation (6.2), p. 7, §6, prime-count term preceding the numerical closure; p. 7, §6, three power comparisons for X at least 64; p. 7, §6, combined numerical estimate at the end of Proposition 6.1; p. 1, Abstract and paragraph after Theorem 1.1, p. 6, Proposition 6.1, statement, p. 7, End of Proposition 6.1; p. 7, §7, definition of H and equation (7.1), p. 8, Proposition 7.2, index range in the proof; p. 1, Abstract, finite certificate count, p. 7, §7, definition of H, p. 8, Proposition 7.2, index range in the proof; p. 7, §7, paragraph following (7.1); p. 7, Lemma 7.1, proof, multiplicity, size, and least-prime observation; p. 7, Lemma 7.1, statement; p. 7, §7, definition of J after Lemma 7.1; p. 7, §7, displayed set of possible summands after the definition of J; p. 7, §7, definition of U(a) in equation (7.2); p. 7, §7, paragraph after (7.2), p. 8, Proposition 7.2, vanishing-factor criterion; p. 7, §7, progression below (7.3); p. 7, §7, identification of indicators with the progression sieve; p. 7, §7, number of primes in the sieve after (7.3), p. 8, Paragraph after Table 1, retained-index count; p. 7, §7, initialization and update in equation (7.3); p. 7, §7, equivalence of equations (7.2) and (7.3), p. 8, Table 1 caption; p. 8, Table 1, all twelve entries, and paragraph after it; p. 1, Abstract, finite certificate coverage, p. 8, Proposition 7.2, statement and stated certificate implication; p. 1, §1, first displayed definitions and Theorem 1.1; p. 1, §1, definition of admissible summands and Euler formulation; p. 1, Lemma 2.1, scaling step; p. 1, §1, historical paragraph and Theorem 1.1, and p. 8, reference [4]; p. 1, §1, paragraph before Theorem 1.1, and p. 8, reference [2]; PDF p. 1, Abstract and Theorem 1.1, and p. 8, Proof of Theorem 1.1; p. 2, §2, equation (2.3), and p. 7, §6, application of (2.2) and (2.3); p. 2, §3.1, sentence immediately after the displayed Hurwitz order; p. 2, §3.1, paragraph beginning “The order H is norm-Euclidean”; pp. 2–3, §3.1, final display on p. 2 and definitions surrounding (3.3) on p. 3; pp. 2–3, §3.1, reduction setup and equation (3.3); p. 3, §3.2, displayed definition of the character before Lemma 3.2; p. 3, §3.2, displayed determinant character and the justification immediately following it; p. 3, Lemma 3.2, equation (3.5) and the following paragraph; p. 3, Lemma 3.2, paragraph following the stabilizer and last sentence of the proof; p. 3, Lemma 3.2, paragraph beginning with the one-dimensional automorphic representations; p. 3, proof of Lemma 3.2, paragraph on the remaining representations; p. 3, Lemma 3.2, opening of the Ramanujan–Petersson paragraph, and p. 8, Reference [1]; PDF p. 3, §3.2, Lemma 3.2; p. 4, §3.3, opening paragraph; right multiplication as in p. 2, §3.1, (3.2); p. 4, §3.3, the two invariance assertions and (3.7); p. 4, §3.3, paragraph between (3.7) and (3.8); PDF p. 4, §3.3, equations (3.7)–(3.8) and the sentence following (3.8); p. 4, Completion of the proof of Proposition 3.1, divisor-sum ratio and final inequality; p. 2, Proposition 3.1, equation (3.1), and p. 4, §3.3 and completion of Proposition 3.1; p. 5, §4, definitions of M(n) and r₂(u) immediately before Lemma 4.2; PDF p. 5, Lemma 4.2, proof through the bound on p; PDF p. 5, Lemma 4.2, equation (4.1) and its proof; p. 5, Lemma 5.1, equation (5.1) and proof; PDF p. 6, proof of Lemma 5.2, from the one-period check through the interval estimate; p. 6, Lemma 5.2, equation (5.2) and its proof through the periodicity argument; PDF p. 6, proof of Lemma 5.2, displayed identity and upper bound after “Partial summation yields”; p. 6, Lemma 5.2, equation (5.3) and the sentence following the partial-summation display; p. 6, Proposition 6.1, equation (6.2), and p. 7, opening sentence; p. 1, Abstract and paragraph after Theorem 1.1, p. 2, equations (2.2)–(2.3), pp. 6–7, Proposition 6.1; p. 7, §7, definition of H and (7.1), and p. 8, Proposition 7.2, first sentence of proof; p. 1, Abstract, finite certificate count, p. 7, §7, definition of H, and p. 8, Proposition 7.2, statement and first sentence of proof; p. 7, §7, proof of Lemma 7.1, first four sentences; p. 7, §7, Lemma 7.1 (statement and proof); p. 7, §7, equation (7.2) and its preceding sentence; p. 7, §7, paragraph after (7.2), and p. 8, Proposition 7.2, vanishing-factor criterion; p. 7, §7, equation (7.1) and the progression following (7.3); p. 7, §7, progression below (7.3), and p. 8, first sentence after Table 1; p. 7, §7, equations (7.1)–(7.3); p. 8, Table 1 and the terminal-empty-set sentence immediately after it; p. 1, Abstract, finite certificate coverage, pp. 7–8, (7.2), Table 1 and Proposition 7.2, statement and proof. Reading limits: Read all eight frozen PDF pages and all 99 original coverage records. Formulas were checked against the rendered pages and anchors against the frozen extraction. Recomputed the finite certificate, fifth-power products, residue discrepancy and closing rational inequalities independently.
- John A. Ewell, An Elementary Proof of Jacobi’s Four-Square Theorem: https://www.fq.math.ca/Scanned/41-3/ewell.pdf#page=1; p. 224, §1, Theorem 1 and preceding definitions; p. 228, concluding even and odd coefficient formulas. Reading limits: Checked the theorem, the signed ordered counting convention, the divisor sum and odd-part definitions, and the final coefficient formulas in the PDF text. Used the theorem as an external input.
- Dietmann and Elsholtz, Sums of two numbers having only prime factors congruent to one modulo four: https://www.math.tugraz.at/~elsholtz/WWW/papers/greaves20.pdf; Author version, pp. 1–3, abstract, unnumbered Theorem and proof, equation (1), final paragraph before References. Reading limits: Read the three-page extracted author version, including the lower-bound argument and the explicit complementary-prime question. Greaves’s underlying proof was outside this reading.
- Euler and the Four-Squares Theorem, MathOverflow: https://mathoverflow.net/questions/37278/euler-and-the-four-squares-theorem; Lucia’s answer of 3 September 2013, opening formulation, Conclusion and Remarks. Reading limits: Read the stated weighted problem, resulting lower bound and asymptotic remark in the original answer. Used for priority and problem scope. The linked analytic estimates were outside scope.

### Research insight 02 · Sharpness of the finite smaller-summand bound

#### Insight

**Kind:** connection

**Evidence status:** proved

Let $\mathcal A$ consist of the positive integers all of whose prime divisors are $1\pmod 4$, including $1$. For $n\in\mathcal A+\mathcal A$, let $L(n)$ be the least smaller summand among its representations by two members of $\mathcal A$. Every $n\equiv2\pmod4$ with $2\le n<64^4$ has such a representation, and on this interval $L(n)$ has maximum $313$, attained only at $n=13{,}667{,}030$. For every integer $B\ge1$, there is a residue class modulo a multiple $M$ of $4$ whose sufficiently large members are $2\pmod4$, belong to $\mathcal A+\mathcal A$, and satisfy $L(n)>B$. The relative lower density of these exceptions to the cap within the progression $2\pmod4$ is at least $4/M$.

#### Why it matters

The unique maximizer identifies where Proposition 7.2 needs its largest permitted summand. Every fixed finite list of candidate summands misses a positive proportion of the progression $n\equiv2\pmod4$.

#### Originality

Table 1 records $U(289)=1$ and $U(313)=0$. The replay identifies the survivor and checks the intervening admissible caps $293$ and $305$. The article gives neither the survivor's value nor the global congruence construction. The methods are standard and priority beyond the article remains undetermined.

#### Current knowledge

The finite claim is proved by an exact sieve, with an independent trial-division check at the maximizer. The progression claim is proved by the finite Chinese remainder theorem and the published eventual representation theorem of Dietmann and Elsholtz.

#### Argument and next steps

The exact sieve leaves only $k=3{,}416{,}757$ at cap $305$ and covers all indices at cap $313$. There is no admissible summand strictly between those caps, so $4k+2=13{,}667{,}030$ uniquely attains the bound. For each cap $B$, assign a distinct prime $p_a\equiv3\pmod4$ to each admissible $a\le B$. Combine $n\equiv a\pmod{p_a}$ with $n\equiv2\pmod4$ by CRT. For $n>B$ in the resulting class every candidate complement has a forbidden prime divisor. Eventual representability gives $L(n)>B$ on a tail of the class, whose relative density is $4/M$.

#### Proof sketch or overall strategy

Use a prime-divisor sieve and translate the admissible index set to check finite coverage. Check the maximizing witness separately by trial division. For an arbitrary cap, combine the congruences that exclude each candidate summand and use the published eventual representation theorem.

#### Numbered argument

1. Put $H=2^{22}-1$. Each $4j+1$ for $0\le j\le H$ is odd and less than $4096^2$. Its prime factors congruent to $3\pmod4$ occur an even number of times with multiplicity. If there are any, the product of the two smallest such factors is at most $4j+1$, so the smaller one is below $4096$. Thus $E=\{j:0\le j\le H,\ 4j+1\in\mathcal A\}$ is obtained by deleting $j\equiv(3p-1)/4\pmod p$ for each prime $p\le4096$ congruent to $3\pmod4$. The residue is integral and solves $4j+1\equiv0\pmod p$. [admissible-summands, finite-range, prime-factorisation]
2. For a cap $c$, start with $C=\{0,\ldots,H\}$ and delete $i+E$ for each $i\in E$ with $4i+1\le c$. Every admissible positive summand of $4k+2$ in the finite interval is $1\pmod4$ and at most $4k+1\le4H+1$. Hence $k$ is deleted exactly when there are $i,j\in E$ with $k=i+j$ and $4i+1\le c$. This is equivalent to the existence of a representation with smaller summand at most $c$, because the summands can be exchanged. [admissible-summands, finite-range, prime-factorisation, step:1]
3. Generate the sieve primes by testing the candidates $3,7,11,\ldots$ up to $4096$ by trial division. There are $287$ sieve primes and $1{,}344{,}661$ surviving indices. Encode $E$ by $S=\sum_{j\in E}2^j$ and start with mask $2^{H+1}-1$. For $i=0,\ldots,78$ in order, if $i\in E$, clear the mask bits in the left shift of $S$ by $i$. After processing $4i+1=289,293,305,309$, the mask is $2^{3{,}416{,}757}$. After $313$ it is zero. The sieve excludes $309$, the only integer $1\pmod4$ strictly between $305$ and $313$. Thus the sole surviving index at cap $305$ gives $L(13{,}667{,}030)=313$, and every other integer in the finite interval has $L(n)\le305$. [trial-division, step:1, step:2]
4. At $n_*=13{,}667{,}030$, there are $42$ admissible $a<313$. Testing for divisibility of $n_*-a$ by $3$, then $7$, then $11$ excludes $22$, $4$ and $3$ additional candidates, respectively. The remaining candidate and forbidden-prime pairs $(a,p)$ are $(1,83),(37,443),(61,1451),(73,1091),(85,23),(109,79),(145,571),(169,67),(193,131),(205,563),(229,47),(241,107),(277,31)$. Direct remainders and trial division verify $p\mid n_*-a$ and that each $p$ is prime and $3\pmod4$. Finally $n_*=313+13{,}666{,}717$. Both summands are $1\pmod4$ and are prime by trial division through $17$ and $3696$, respectively. [admissible-summands, trial-division, step:1]
5. Given any finite list of primes congruent to $3\pmod4$, let $P$ be their product, with empty product $1$. The odd integer $4P-1$ is $3\pmod4$, so its prime factorization contains a prime in that class. Each listed prime leaves remainder $-1$ on dividing $4P-1$, so the factor is outside the list. This proves that infinitely many such primes exist. [prime-factorisation]
6. Fix an integer $B\ge1$ and let $F_B=\{a\in\mathcal A:a\le B\}$. Assign a distinct prime $p_a\equiv3\pmod4$ to each $a\in F_B$. The moduli $4$ and $p_a$ are pairwise coprime, so the congruences $n\equiv2\pmod4$ and $n\equiv a\pmod{p_a}$ specify one class modulo $M=4\prod_{a\in F_B}p_a$. For every $n>B$ in that class, each $n-a$ for $a\in F_B$ is positive and has a forbidden prime divisor. Therefore every representation of that $n$ by members of $\mathcal A$ has both summands greater than $B$. [admissible-summands, chinese-remainder, step:5]
7. All sufficiently large members of the class are positive and $2\pmod4$, so the Dietmann–Elsholtz theorem gives a representation for each. Then $L(n)>B$ by step 6. Up to $X$, the tail of this class contains $X/M+O(1)$ integers, while the positive progression $2\pmod4$ contains $X/4+O(1)$. Dividing gives a relative density of $4/M$ for the tail and a relative lower density of at least $4/M$ for the full set on which $L(n)$ exists and exceeds $B$. [admissible-summands, eventual-representation, step:6]

#### Immediate dependencies

- **admissible-summands:** $\mathcal A$ comprises the positive integers with all prime divisors congruent to $1\pmod4$, including $1$. On $\mathcal A+\mathcal A$, $L(n)$ is the minimum of the smaller summand over the nonempty finite set of admissible representations of $n$. Source: self-contained; Insight statement. Reading limits: Checked the convention for $\mathcal A$ against the rendered article's opening definition. The minimum is defined locally and exists because the summands are positive integers bounded by $n-1$.
- **finite-range:** The integers $2\le n<64^4$ with $n\equiv2\pmod4$ are exactly $n=4k+2$ for $0\le k\le2^{22}-1$. Source: self-contained; Insight statement and steps 1–2. Reading limits: Checked by $64^4=4\cdot2^{22}$ and the progression endpoints. The article's §7 uses the same range.
- **prime-factorisation:** Every positive integer is a finite product of primes, unique up to order, and the factorization of $1$ is the empty product. Source: math:thm-fundamental-theorem-of-arithmetic; Statement, clauses 1–2 and the empty-product case. Reading limits: Checked the statement and supporting facts in the hash-matched library item. Only ordinary positive integer factorization is used.
- **trial-division:** An integer $m>1$ is prime if it has no divisor from $2$ through $\lfloor\sqrt m\rfloor$. A composite $m=uv$ with $1<u\le v$ has $u\le\sqrt m$. Source: self-contained; Factor-pair argument here and applications in steps 3–4. Reading limits: Checked by exact integer arithmetic in the finite replay and the direct witness computation.
- **chinese-remainder:** For a finite pairwise coprime list of positive moduli, each tuple of residues determines one simultaneous residue class modulo the product. Source: math:thm-chinese-remainder-theorem; Statement and proof steps 1.2, 2.1 and 3.1. Reading limits: Checked the hash-matched library statement and its existence and uniqueness argument. Cross-checked Conrad's §3, Theorem 3.1 and proof.
- **eventual-representation:** Every sufficiently large positive integer congruent to $2\pmod4$ is a sum of two positive integers whose prime factors are all congruent to $1\pmod4$. Source: https://www.impan.pl/shop/en/publication/transaction/download/product/113105; Banach Center Publications 118 (2019), p. 177, unnumbered Theorem, and pp. 178–179, proof and Remark. Reading limits: Checked the published theorem, the lower bound in equation (1), the forbidden-divisor estimate and the remark on ineffectivity. Checked the hypotheses of Greaves's cited lower-bound statement. Its proof was outside the review.

#### Independent review

**Decision:** repair

Two exact sieve implementations left only index 3,416,757 at caps 289, 293 and 305, and cleared it at cap 313. Direct trial division independently verified the minimum at the witness. The CRT argument and relative lower density bound hold with the published Dietmann–Elsholtz theorem.

**Dependency review:** The definitions, finite indexing and trial-division criterion are self-contained. The frozen factorisation and CRT suppliers match their recorded hashes and supply the required statements. Their dependency graph is acyclic and independent of the article. Conrad's Theorem 3.1 also applies because the moduli are pairwise coprime. The author-hosted Dietmann–Elsholtz extraction gives a per-prime count with $w^2$ in the denominator. The published proof counts multiples of $w$ in the square variable and gives $O(1+\sqrt n/w)$. Even summing over all integers $w\le\sqrt n$ gives $O(\sqrt n\log n)$, which is smaller than the lower bound in their equation (1) for fixed $0<\varepsilon<1/6$. Their theorem supplies eventual existence under exactly the positivity and congruence hypotheses of the constructed class.

**Review reading limits:** Read the frozen article's rendered pages 1, 7 and 8, the two library statements and relevant proof passages, Conrad's §3, and the theorem and proof passages in the author-hosted and published Dietmann–Elsholtz PDF extractions. Checked the statement of Greaves's lower bound and its applicability to residues 2 and 6 modulo 8. The analytic proof in the article and Greaves's sieve proof were outside this review. Priority beyond the article remains undetermined after targeted searches.

#### Author and reviewer gaps

No remaining gaps were reported within the stated scope.

#### Remaining gaps

The construction gives a lower bound on the relative density of exceptions to each fixed cap. The growth rate of $L(n)$ and the optimal density of exceptions are outside the result. The eventual representation theorem used here supplies an ineffective threshold.

#### Sources

- Euler’s 1747 conjecture on sums of integers with restricted prime factors: https://hexagonmath.org/pdf/2611.00370v1; p. 1, §1, opening definitions; p. 1, Abstract and §1, opening paragraph; p. 1, §1, definition of admissible summands and Euler formulation, p. 1, Lemma 2.1, scaling step; p. 1, §1, Letter 115 and editorial note 10, p. 8, Reference [4]; p. 1, §1, Euler’s divisor condition and the definition of admissible summands; p. 1, §1, prior result of Dietmann and Elsholtz, p. 8, Reference [2]; p. 1, Abstract and Theorem 1.1, p. 8, Proof of Theorem 1.1; p. 1, §2, first sentence; p. 1, Lemma 2.1, first sentence of the proof; p. 1, Lemma 2.1, statement and scaling step; p. 2, §2, definition preceding (2.1) and notation in (2.1); p. 2, §2, equation (2.1); p. 2, §2, text between (2.1) and (2.2); p. 2, §2, definition of the mixed set preceding (2.2); p. 2, §2, equation (2.2); p. 2, §2, definition of the exceptional sets following (2.2); p. 2, §2, quadratic nonresidue observation preceding (2.3); p. 2, §2, conclusion immediately preceding (2.3); p. 2, §2, equation (2.3), p. 7, §6, application of (2.2) and (2.3); p. 2, §3.1, Hamilton algebra and reduced norm; p. 2, §3.1, displayed definition of the order; p. 2, §3.1, enumeration of units; p. 2, §3.1, rounding and the strict norm bound; p. 2, §3.1, consequence of norm-Euclidean division; p. 2, §3.1, definition of the norm shell preceding (3.2); p. 2, §3.1, equation (3.2) and inverse description; p. 2, §3.1, last paragraph; p. 2, §3.1, definitions of the projective group and reduction, p. 3, §3.1, definitions of the unit image, quotient, and counting inner product; p. 3, §3.1, scalar reductions and equation (3.3); p. 3, §3.2, equation (3.4); p. 3, §3.2, first three claims following (3.4); p. 3, §3.2, constant eigenvalue following (3.4); p. 3, §3.2, definition of the character before Lemma 3.2; p. 3, §3.2, justification of the definition of the determinant character; p. 3, §3.2, character eigenvalue before Lemma 3.2; p. 3, Lemma 3.2, proof, definition of the compact open level; p. 3, Lemma 3.2, equation (3.5) and stabilizer paragraph; p. 3, Lemma 3.2, paragraph following the stabilizer description; p. 3, Lemma 3.2, paragraph on one-dimensional automorphic representations; p. 3, Lemma 3.2, invocation of Jacquet–Langlands and the weight-two setting, p. 8, References [3] and [5]; p. 3, Lemma 3.2, opening of the Ramanujan–Petersson paragraph, p. 8, Reference [1]; p. 3, Lemma 3.2, displayed local eigenvalue and triangular-coset calculation; p. 3, Lemma 3.2, last paragraph, local bound before multiplication; p. 3, Lemma 3.2, statement and last sentence of its proof; p. 4, §3.3, opening definitions of the two subgroups; p. 4, §3.3, order assertion immediately following the subgroup definitions; p. 4, §3.3, description of pair vanishing and multiplication by 1 + i; p. 4, §3.3, unit-image intersection preceding the orbit definition; p. 4, §3.3, displayed orbit and indicator definitions; p. 4, §3.3, density formula, orbit count, and the case $p = 3$; p. 4, §3.3, class multiplicity preceding (3.6); p. 4, §3.3, equation (3.6); p. 4, §3.3, invariance and equation (3.7); p. 4, §3.3, norm surjectivity and balance paragraph following (3.7); p. 4, §3.3, centered indicator and its norm before (3.8); p. 4, §3.3, equation (3.8) and case $p = 3$; p. 4, Completion of Proposition 3.1, formula for the dividing-prime obstruction count; p. 4, Completion of Proposition 3.1, divisor-sum ratio and last inequality; p. 2, Proposition 3.1, equation (3.1), p. 4, §3.3 and completion of Proposition 3.1; p. 4, §4, definition preceding Lemma 4.1; p. 4, Lemma 4.1, proof, orbit representatives, label and norm identity; p. 4, Lemma 4.1, statement and last two lines; p. 5, §4, definitions of M(n) and r₂(u) on the first lines; p. 5, §4, two-square formula application before Lemma 4.2; p. 5, Lemma 4.2, proof, per-prime count and upper limit on the prime; p. 5, Lemma 4.2, last line of proof; p. 5, Lemma 4.2, equation (4.1); p. 5, Lemma 5.1, first two proof paragraphs before the table; p. 5, Lemma 5.1, ratio test and table of maximizing positive exponents; p. 5, Lemma 5.1, absent-prime convention and displayed fifth-power products; p. 5, Lemma 5.1, equation (5.1); p. 6, Lemma 5.2, definition of the residue set and counting function; p. 6, Lemma 5.2, first sentence of proof; p. 6, Lemma 5.2, one-period check and interval estimate; p. 6, Lemma 5.2, equation (5.2); p. 6, Lemma 5.2, displayed partial-summation identity and upper bound; p. 6, Lemma 5.2, equation (5.3); p. 6, Lemma 5.2, equation (5.4) and final finite sum through 60; p. 6, Proposition 6.1, choice of cutoff and equation (6.1); p. 6, Proposition 6.1, equation (6.2), p. 7, §6, prime-count term preceding the numerical closure; p. 7, §6, three power comparisons for X at least 64; p. 7, §6, combined numerical estimate at the end of Proposition 6.1; p. 1, Abstract and paragraph after Theorem 1.1, p. 6, Proposition 6.1, statement, p. 7, End of Proposition 6.1; p. 7, §7, definition of H and equation (7.1), p. 8, Proposition 7.2, index range in the proof; p. 1, Abstract, finite certificate count, p. 7, §7, definition of H, p. 8, Proposition 7.2, index range in the proof; p. 7, §7, paragraph following (7.1); p. 7, Lemma 7.1, proof, multiplicity, size, and least-prime observation; p. 7, Lemma 7.1, statement; p. 7, §7, definition of J after Lemma 7.1; p. 7, §7, displayed set of possible summands after the definition of J; p. 7, §7, definition of U(a) in equation (7.2); p. 7, §7, paragraph after (7.2), p. 8, Proposition 7.2, vanishing-factor criterion; p. 7, §7, progression below (7.3); p. 7, §7, identification of indicators with the progression sieve; p. 7, §7, number of primes in the sieve after (7.3), p. 8, Paragraph after Table 1, retained-index count; p. 7, §7, initialization and update in equation (7.3); p. 7, §7, equivalence of equations (7.2) and (7.3), p. 8, Table 1 caption; p. 8, Table 1, all twelve entries, and paragraph after it; p. 1, Abstract, finite certificate coverage, p. 8, Proposition 7.2, statement and stated certificate implication; p. 1, §1, first displayed definitions and Theorem 1.1; p. 1, §1, definition of admissible summands and Euler formulation; p. 1, Lemma 2.1, scaling step; p. 1, §1, historical paragraph and Theorem 1.1, and p. 8, reference [4]; p. 1, §1, paragraph before Theorem 1.1, and p. 8, reference [2]; PDF p. 1, Abstract and Theorem 1.1, and p. 8, Proof of Theorem 1.1; p. 2, §2, equation (2.3), and p. 7, §6, application of (2.2) and (2.3); p. 2, §3.1, sentence immediately after the displayed Hurwitz order; p. 2, §3.1, paragraph beginning “The order H is norm-Euclidean”; pp. 2–3, §3.1, final display on p. 2 and definitions surrounding (3.3) on p. 3; pp. 2–3, §3.1, reduction setup and equation (3.3); p. 3, §3.2, displayed definition of the character before Lemma 3.2; p. 3, §3.2, displayed determinant character and the justification immediately following it; p. 3, Lemma 3.2, equation (3.5) and the following paragraph; p. 3, Lemma 3.2, paragraph following the stabilizer and last sentence of the proof; p. 3, Lemma 3.2, paragraph beginning with the one-dimensional automorphic representations; p. 3, proof of Lemma 3.2, paragraph on the remaining representations; p. 3, Lemma 3.2, opening of the Ramanujan–Petersson paragraph, and p. 8, Reference [1]; PDF p. 3, §3.2, Lemma 3.2; p. 4, §3.3, opening paragraph; right multiplication as in p. 2, §3.1, (3.2); p. 4, §3.3, the two invariance assertions and (3.7); p. 4, §3.3, paragraph between (3.7) and (3.8); PDF p. 4, §3.3, equations (3.7)–(3.8) and the sentence following (3.8); p. 4, Completion of the proof of Proposition 3.1, divisor-sum ratio and final inequality; p. 2, Proposition 3.1, equation (3.1), and p. 4, §3.3 and completion of Proposition 3.1; p. 5, §4, definitions of M(n) and r₂(u) immediately before Lemma 4.2; PDF p. 5, Lemma 4.2, proof through the bound on p; PDF p. 5, Lemma 4.2, equation (4.1) and its proof; p. 5, Lemma 5.1, equation (5.1) and proof; PDF p. 6, proof of Lemma 5.2, from the one-period check through the interval estimate; p. 6, Lemma 5.2, equation (5.2) and its proof through the periodicity argument; PDF p. 6, proof of Lemma 5.2, displayed identity and upper bound after “Partial summation yields”; p. 6, Lemma 5.2, equation (5.3) and the sentence following the partial-summation display; p. 6, Proposition 6.1, equation (6.2), and p. 7, opening sentence; p. 1, Abstract and paragraph after Theorem 1.1, p. 2, equations (2.2)–(2.3), pp. 6–7, Proposition 6.1; p. 7, §7, definition of H and (7.1), and p. 8, Proposition 7.2, first sentence of proof; p. 1, Abstract, finite certificate count, p. 7, §7, definition of H, and p. 8, Proposition 7.2, statement and first sentence of proof; p. 7, §7, proof of Lemma 7.1, first four sentences; p. 7, §7, Lemma 7.1 (statement and proof); p. 7, §7, equation (7.2) and its preceding sentence; p. 7, §7, paragraph after (7.2), and p. 8, Proposition 7.2, vanishing-factor criterion; p. 7, §7, equation (7.1) and the progression following (7.3); p. 7, §7, progression below (7.3), and p. 8, first sentence after Table 1; p. 7, §7, equations (7.1)–(7.3); p. 8, Table 1 and the terminal-empty-set sentence immediately after it; p. 1, Abstract, finite certificate coverage, pp. 7–8, (7.2), Table 1 and Proposition 7.2, statement and proof. Reading limits: Read all eight frozen PDF pages and all 99 original coverage records. Formulas were checked against the rendered pages and anchors against the frozen extraction. Recomputed the finite certificate, fifth-power products, residue discrepancy and closing rational inequalities independently.
- Rainer Dietmann and Christian Elsholtz, Sums of two numbers having only prime factors congruent to one modulo four: https://www.impan.pl/shop/en/publication/transaction/download/product/113105; Published version, p. 177, unnumbered Theorem; pp. 178–179, equation (1), forbidden-divisor count and Remark. Reading limits: Read the relevant published PDF extraction, including the corrected per-prime count. Greaves's sieve proof was outside the reading.
- Keith Conrad, The Chinese Remainder Theorem: https://kconrad.math.uconn.edu/blurbs/ugradnumthy/crt.pdf; §3, Theorem 3.1 and proof, PDF pp. 2–3. Reading limits: Read the finite-system statement and the proofs of existence and uniqueness in the PDF extraction. Later applications were outside the reading.

## 2. Potentially fruitful questions

### Research question 01

#### Research question

Let $\mathcal A$ be the positive integers whose prime factors are all $1\pmod4$, with $1\in\mathcal A$. Define $D(n)=\#\{a:1\le a<n,\ a,n-a\in\mathcal A\}$, counting ordered decompositions, and $C=\lim_{x\to\infty}\sqrt{\log x}\,\#(\mathcal A\cap[1,x])/x$. As $\ell$ tends to infinity through primes congruent to $3\pmod4$, does $D(2\ell)\log(2\ell)/(2\ell)$ converge to $4C^2\prod_{q\equiv3\pmod4}(1-2/q)/(1-1/q)^2$, where the product is over primes?

#### Why it matters

For $n=2\ell$ the only odd prime divisor of $n$ is $\ell$, which eventually lies beyond every fixed cutoff. Each ordered pair contributes one to $D(n)$, so the limit would quantify Euler’s decompositions independently of their four-square multiplicities.

#### Originality

The frozen article proves existence by a weighted four-square sieve and a finite certificate. Its abstract and §§1–7 contain no formulation of this pointwise unweighted limit. Lucia’s asymptotic remark concerns a weighted count, and Ramaré–Viswanadham’s Theorem 1.6 concerns a ternary sum. The targeted search leaves worldwide novelty undetermined.

#### Current knowledge

Landau’s theorem and the inversion below give $0<C<\infty$. The fixed-arc contribution has the stated limit, and Greaves’s theorem with the corrected exceptional-pair estimate yields $D(2\ell)\gg_\varepsilon \ell^{1-\varepsilon}$ for every $\varepsilon>0$. The sources checked give no proof or disproof of the pointwise binary limit.

#### Potential solution

**Solution scope:** partial

**Evidence status:** Proposed approach

Fix $z\ge2$ and $T>0$. For $n=2\ell$, take the arcs of radius $T/n$ around the fractions whose reduced denominators divide $4\prod_{q\le z,\ q\equiv3\pmod4}q$. After normalization by $\log n/n$, the contribution of those arcs tends to $4C^2J(T)\prod_{q\le z,\ q\equiv3\pmod4}(1-2/q)/(1-1/q)^2$, where $J(T)=\int_{-T}^T(\sin(\pi t)/(\pi t))^2\,dt$. Taking $T$ and then $z$ to infinity gives the proposed constant for this contribution. Independently, for every $\varepsilon>0$ and all sufficiently large $n\equiv2\pmod4$, $D(n)\gg_\varepsilon n^{1-\varepsilon}$.

#### Argument and next steps

Invert Landau’s count to obtain the asymptotic for the summand set. Evaluate the Fourier sum at each fixed rational center using the odd-modulus estimate and the exact phase modulo four. Orthogonality and the Chinese remainder theorem then evaluate the finite convolution. For the independent lower bound, divide Greaves’s prime-pair count by the two-square multiplicities and discard the exceptional summand pairs using a harmonic sum.

#### Proof sketch or overall strategy

Derive the one-variable asymptotic by inversion, evaluate the binary Fourier integral on a fixed rational grid, and identify the exact remaining cancellation condition. Prove the lower bound separately from Greaves’s theorem.

#### Numbered argument

1. Let $F(x)=\#(\mathcal A\cap[1,x])$ and let $B(x)$ count the positive integers up to $x$ representable as a sum of two integer squares. Let $\mathcal I$ be the positive integers all of whose prime factors are $3\pmod4$, including $1$. By the two-square criterion and unique factorization, each integer counted by $B$ has a unique form $2^k d^2a$ with $k\ge0$, $d\in\mathcal I$ and $a\in\mathcal A$. Thus $B(y)-B(y/2)$ counts the odd representable integers up to $y$. Inclusion-exclusion over the inert prime square divisors gives $F(x)=\sum_{d\in\mathcal I,\ d\le\sqrt x}\mu(d)[B(x/d^2)-B(x/(2d^2))]$. Indeed, an odd representable integer with inert part $h^2$ has total weight $\sum_{d\mid h}\mu(d)$, which is one for $h=1$ and zero otherwise. [counting-setup, landau-two-square-count]
2. Landau’s asymptotic $B(y)\sim Ky/\sqrt{\log y}$ gives a limit $K/(2d^2)$ for each fixed bracket in step 1 after multiplication by $\sqrt{\log x}/x$. For $d\le x^{1/4}$ the normalized brackets are $O(d^{-2})$, since $x/d^2\ge\sqrt x$ and the bracket is between zero and $B(x/d^2)$. The unnormalized tail for $d>x^{1/4}$ is $O(x\sum_{d>x^{1/4}}d^{-2})=O(x^{3/4})$ by $B(y)\le y$. Taking the limit first over a finite set of $d$ and then bounding the remaining summable tail gives $C=(K/2)\prod_{q\equiv3\pmod4}(1-q^{-2})>0$. Absolute convergence of the series justifies the product. The prime number theorem at residue 3 modulo 4 ensures the target subsequence is infinite. [step:1, landau-two-square-count, prime-number-theorem-progressions]
3. Let $P_z=\prod_{q\le z,\ q\equiv3\pmod4}q$ over primes, $W=4P_z$, and $E_z=\{r\bmod W:r\equiv1\pmod4,\ (r,P_z)=1\}$. The moduli $4$ and the distinct odd primes dividing $P_z$ are pairwise coprime. If $n=2\ell$, then $n\equiv2\pmod4$, so there is one choice for the first residue modulo 4. At each $q\mid P_z$ exclude $0$ and $n\bmod q$. Put $\nu_q(n)=1$ when $q\mid n$ and $2$ otherwise. Then $|E_z|=\varphi(P_z)$ and $W\#\{r\in E_z:n-r\in E_z\}/|E_z|^2=4\prod_{q\mid P_z}(1-\nu_q(n)/q)/(1-1/q)^2$. If the cutoff includes $\ell$, its single exceptional factor has ratio $(\ell-1)/(\ell-2)$ to the two-forbidden-residue factor. [counting-setup, chinese-remainder-theorem]
4. Put $e(u)=\exp(2\pi i u)$ and $S(\alpha;n)=\sum_{1\le m\le n}\mathbf1_{\mathcal A}(m)e(m\alpha)$. Integrating the expansion of the square gives $D(n)=\int_0^1 S(\alpha;n)^2e(-n\alpha)\,d\alpha$, since the surviving terms have positive $m_1,m_2$ with $m_1+m_2=n$. Integrating the expansion of the squared modulus gives $\int_0^1|S(\alpha;n)|^2\,d\alpha=F(n)$. [step:1, counting-setup, fourier-orthogonality]
5. Set $V(t)=\int_0^1e(tu)\,du$. The monotone functions $u\mapsto\sqrt{\log n}F(nu)/n$ converge uniformly on $[0,1]$ to $Cu$. Step 2 gives pointwise convergence for $u>0$, and the value at zero is zero. A finite mesh bounds the errors between consecutive mesh points by the endpoint errors plus $C$ times the mesh size. For a differentiable $g$, writing $g(m/n)=g(1)-\int_{m/n}^1 g'(u)\,du$ and summing gives partial summation. With $g(u)=e(tu)$ and $|g'|\le2\pi T$, it yields $S(t/n;n)=(Cn/\sqrt{\log n})V(t)+o_T(n/\sqrt{\log n})$ uniformly for $|t|\le T$. [step:2, step:4]
6. Choose integers $u,v$ with $uP_z+4v=1$. For $m\in\mathcal A$, $e(jm/W)=e(ju/4)e(jvm/P_z)$ because $m\equiv1\pmod4$. Reduce $jv/P_z$ to $h/q$, so $q\mid P_z$ and all such $m$ are coprime to $q$. For $q>1$, the odd-modulus estimate gives $S(h/q;x)-\mu(q)F(x)/\varphi(q)=O_q(x/\log x)$ for large $x$. The supremum of this error for $0\le x\le n$ is $O_q(n/\log n)$, absorbing the bounded initial range. Partial summation as in step 5 gives the same comparison with $S(t/n;n)$ at frequency $h/q+t/n$, with error $O_{q,T}(n/\log n)$. At $q=1$ the comparison is exact with multiplier one. Reduction of the units modulo $P_z$ to the units modulo $q$ has equal-size fibers, and their average of $e(hx/q)$ is $\mu(q)/\varphi(q)$ by the finite geometric sum and inclusion-exclusion. Incorporating the phase modulo 4 gives $B_z(j)=|E_z|^{-1}\sum_{r\in E_z}e(jr/W)$. Hence $S(j/W+t/n;n)=(Cn/\sqrt{\log n})B_z(j)V(t)+o_{z,T}(n/\sqrt{\log n})$ uniformly for $0\le j<W$ and $|t|\le T$. [step:3, step:4, step:5, ramare-viswanadham-odd-denominator, chinese-remainder-theorem, fourier-orthogonality]
7. Let $\mathfrak M_{z,T}(n)$ be the union on $\mathbb R/\mathbb Z$ of the arcs $j/W+[-T/n,T/n]$. They are disjoint for $n>2TW$. Substituting $\alpha=j/W+t/n$ in the normalized integral over these arcs and using step 6 gives $C^2J(T)\sum_{j=0}^{W-1}B_z(j)^2 e(-nj/W)+o_{z,T}(1)$. Here $V(t)=e(t/2)\sin(\pi t)/(\pi t)$, with the continuous value at zero, so $V(t)^2e(-t)$ is the integrand defining $J(T)$. Expanding $B_z(j)^2$ and applying finite orthogonality evaluates the sum as $W\#\{r\in E_z:n-r\in E_z\}/|E_z|^2$. Eventually $\ell>z$, and step 3 then gives the stated fixed-arc limit. [step:3, step:6, fourier-orthogonality]
8. The Riemann sums $V_k(t)=k^{-1}\sum_{m=1}^k e(mt/k)$ converge uniformly to $V(t)$ on each bounded $t$-interval, by the bound $2\pi|t|$ for the derivative in the integration variable. Orthogonality after rescaling gives $\int_{-k/2}^{k/2}|V_k(t)|^2\,dt=1$. The geometric sum and $|\sin(\pi t/k)|\ge2|t|/k$ give $|V_k(t)|\le\min(1,1/(2|t|))$ when $0<|t|\le k/2$. For fixed $T>0$ and $k>2T$, the squared-modulus integral between $|t|=T$ and $|t|=k/2$ is at most $1/(2T)$. Passing to the limit on $[-T,T]$ and then sending $T$ to infinity shows $J(T)\to1$. The odd-prime factors are $1-1/(q-1)^2$. They are positive with summable deviations from one, so the product converges to a positive limit. [step:3, step:5, step:7, fourier-orthogonality]
9. Let $R_{z,T}(n)$ be $\log n/n$ times the integral of $S(\alpha;n)^2e(-n\alpha)$ over the complement of $\mathfrak M_{z,T}(n)$. Subtracting the fixed-arc integral from step 4 and using steps 7 and 8 shows that the proposed limit is equivalent to $\limsup_{z\to\infty}\limsup_{T\to\infty}\limsup_{\ell\to\infty}|R_{z,T}(2\ell)|=0$, with $\ell$ restricted to the stated primes. For fixed $z,T$ the triangle inequality bounds the limsup of the absolute deviation of the full normalized integral from the proposed constant by the limsup of $|R_{z,T}|$ plus the difference between the two constants, and gives the reverse bound with the same difference. For fixed $z,T$ the arcs carry at most $2TW F(n)^2/n=O_{z,T}(n/\log n)$ of the $|S|^2$ integral. By step 4 the complementary absolute integral is therefore asymptotic to $Cn/\sqrt{\log n}$. [step:2, step:4, step:7, step:8]
10. Let $n\equiv2\pmod4$. Its residue modulo 8 is 2 or 6, so Greaves gives $\gg n/(\log n)^{5/2}$ prime pairs $(p,r)$ with $n-p^2-r^2=x^2+y^2$. Any pairs involving 2 number at most $O(\sqrt n)$ and can be removed. Choose one representation for each remaining pair. Then $x,y$ are even by reduction modulo 4, and $a=p^2+x^2$, $b=r^2+y^2$ are positive odd integers. The two-square formula gives $r_2(m)\le4d(m)$, where $d(m)$ counts divisors. For each $\eta>0$, $d(m)\ll_\eta m^\eta$: for primes $s$ with $s^\eta\ge2$ use $e+1\le2^e\le s^{\eta e}$, and for each of the finitely many smaller primes use boundedness of $(e+1)s^{-\eta e}$ for $e\ge0$. For a fixed ordered $(a,b)$ at most $r_2(a)r_2(b)\ll_\eta n^{2\eta}$ distinct chosen prime pairs map to it. Since $(\log n)^{5/2}=o(n^\eta)$, this leaves $\gg_\eta n^{1-3\eta}$ distinct candidate summand pairs. [greaves-prime-pairs, two-square-representation-count]
11. If an inert prime $w$ divides a candidate $a=p^2+x^2$, then $w$ divides both coordinates, so $p=w$ and $a=w^2(1+k^2)$ for some integer $k$ with $|k|\le\sqrt n/w$. For fixed $w\le\sqrt n$ this gives at most $1+2\sqrt n/w$ choices for $a$, each determining $b$. Summing over $w\le\sqrt n$ using the harmonic sum, and counting obstructions in the second summand as well, gives $O(\sqrt n\log n)$ exceptional pairs. Both summands are odd, so each surviving pair has both entries in $\mathcal A$. Choose $0<\eta<\min(1/6,\varepsilon/3)$. Then the exceptional count is $o(n^{1-3\eta})$ and the survivors give $D(n)\gg_\varepsilon n^{1-\varepsilon}$. In particular this holds for $n=2\ell$ along the target subsequence. [step:10, inert-prime-divides-coordinates, counting-setup]

#### Immediate dependencies

- **counting-setup:** $\mathcal A$ consists of positive integers with all prime factors $1\pmod4$, including $1$ by the empty factorization. Unique prime factorization is used to separate the prime types. $D(n)$ counts positive ordered summands and $\ell$ ranges through primes $3\pmod4$. Source: self-contained; Question formulation and prime factorization. Reading limits: The definitions are given inline. The original article supplies historical context.
- **landau-two-square-count:** A positive integer is a sum of two integer squares exactly when all primes $3\pmod4$ have even exponents. The number $B(x)$ of such integers up to $x$ satisfies $B(x)\sim Kx/\sqrt{\log x}$, where $K=2^{-1/2}\prod_{q\equiv3\pmod4}(1-q^{-2})^{-1/2}$. Source: https://arxiv.org/pdf/2409.03428; arXiv v3, §1, equations (1.1) and (1.2) and the definition and criterion preceding (1.2). Reading limits: Checked the count, the criterion and the constant for ordinary sums of two squares. The proof of Landau’s theorem is imported.
- **prime-number-theorem-progressions:** For fixed coprime positive integers $m,N$, the primes at most $x$ in residue $m$ modulo $N$ number asymptotically $x/(\varphi(N)\log x)$. Use $m=3$ and $N=4$. Source: https://kskedlaya.org/ant/chap-primes-in-ap.html; Chapter 4, §4.4, Theorem 4.12 and the coprimality condition in its proof. Reading limits: Checked the statement and the applicable coprimality condition. The analytic proof is imported.
- **chinese-remainder-theorem:** Reduction modulo a finite pairwise-coprime list of positive moduli is a ring isomorphism from the residue ring modulo their product to the product of the individual residue rings. Source: math:thm-chinese-remainder-theorem; Statement. Reading limits: Checked the canonical statement against the frozen supplier record and its use for the moduli in step 3.
- **fourier-orthogonality:** For integer $k$, $\int_0^1e(k\alpha)\,d\alpha$ is one for $k=0$ and zero otherwise. For integer $k$ and positive integer $W$, $\sum_{j=0}^{W-1}e(jk/W)$ is $W$ if $W\mid k$ and zero otherwise. Source: self-contained; Exponential antiderivative and finite geometric sum. Reading limits: Both identities follow by direct evaluation, taking the constant cases separately.
- **ramare-viswanadham-odd-denominator:** Let $b$ indicate odd primitive sums of two squares, equivalently odd positive integers free of primes $3\pmod4$. For fixed odd $q>1$ and $(h,q)=1$, equation (17) gives $\sum_{m\le x,(m,q)=1} b(m)e(hm/q)=\mu(q)\sum_{m\le x,(m,q)=1}b(m)/\varphi(q)+O_q(x/\log x)$ as $x\to\infty$. The fixed $q$ eventually satisfies the source’s logarithmic modulus bound. Source: https://arxiv.org/html/2509.23260v1; §1, definition of the support of $b$ and equation (5), and §8, proof of Lemma 8.2, equations (15)–(17). Reading limits: Checked the support, the coprimality restriction, the odd-modulus coefficient and the error. The estimate is imported from the odd case. The printed constant in equation (6) plays no role.
- **greaves-prime-pairs:** For all sufficiently large $n$ outside residues $0,1,5$ modulo 8, Greaves gives $\gg n/(\log n)^{5/2}$ prime pairs $p,r\le\sqrt n/2$ for which $n-p^2-r^2$ is a sum of two integer squares. The threshold is ineffective in the cited proof. Source: https://bibliotekanauki.pl/articles/1393472.pdf; Acta Arithmetica 29 (1976), §1, Theorem, and §6, conclusion and equation (6.1). Reading limits: Checked the counted objects, residue exclusions, scale, and positive leading bound. The underlying sieve proof is imported.
- **two-square-representation-count:** For positive $m$, the signed ordered two-square count satisfies $r_2(m)=4\sum_{d\mid m}\chi_4(d)$, where $|\chi_4(d)|\le1$. Source: math:thm-two-square-representation-count; Statement. Reading limits: Checked the canonical statement against the frozen supplier record. Only the bound by four times the divisor count is used.
- **inert-prime-divides-coordinates:** If $w\equiv3\pmod4$ is prime and divides $x^2+y^2$ for integers $x,y$, then it divides both coordinates. Source: math:lem-three-mod-four-prime-dividing-two-square-sum; Statement. Reading limits: Checked the canonical statement against the frozen supplier record and applied it only to the prime-square candidate summands.

#### Independent review

**Decision:** repair

The fixed-arc contribution and its limiting constant survive review. The per-prime estimate cited for discarding exceptional pairs does not follow from the counting argument in the Dietmann–Elsholtz author version. Counting the multiples of the offending prime in the square coordinate gives $O(\sqrt n\log n)$ exceptional pairs, which suffices for the same lower bound. The repair derives the density constant from Landau’s theorem for ordinary sums of two squares and uses the odd-modulus estimate in Ramaré–Viswanadham independently of their printed density constant.

**Dependency review:** The prime number theorem in progressions applies at modulus 4 and residue 3. Berndt–Moree’s general prime-density asymptotic was replaced by their statement of Landau’s theorem and explicit inversion, which gives a finite positive $C$ for this set. The printed value in Ramaré–Viswanadham’s equation (6) differs from the value given by that inversion. Their equation (17) applies independently at fixed odd denominators, with all terms in the support coprime to the denominator. Greaves supplies a count of prime pairs for the required residues modulo 8. The checked two-square formula controls their multiplicities, and the checked divisibility lemma supports the corrected count of exceptional summands. The frozen mathematical suppliers match their recorded hashes. The proof uses no claim from the article or from the conjectured limit as a premise.

**Review reading limits:** Read the full eight-page article extraction and checked rendered pp. 1, 2 and 8 for the definition, the weighted count and the certificate conclusion. The article’s spectral argument and certificate computations were outside the scope of this review. Read the relevant theorem statements and application passages in Kedlaya, Berndt–Moree, Greaves, Dietmann–Elsholtz and Ramaré–Viswanadham, and Lucia’s formulation and remarks. Checked the statements and frozen records of the three mathematical library suppliers. The underlying analytic proofs and the full transitive supplier proofs were outside scope. The literature search was targeted.

#### Author and reviewer gaps

- No bound establishing the iterated vanishing of $R_{z,T}(2\ell)$ in step 9 was verified.
- Ramaré–Viswanadham’s ternary Hölder argument in §13 uses a third Fourier factor. Its restriction estimate for exponents above two leaves the binary cancellation estimate open.
- The proposed pointwise limit still requires cancellation in the complementary binary Fourier integral at the $n/\log n$ scale, in the order of limits specified in step 9. The fixed-arc formula and the lower bound leave that estimate unresolved.
- The checked ternary minor-arc argument uses a third Fourier factor and a restriction estimate of exponent greater than two. The binary coefficient still needs a separate estimate. The targeted literature search leaves the exact limit and its worldwide novelty undetermined.

#### Remaining gaps

The arc estimate takes $n$ to infinity with $z$ and $T$ fixed. For these fixed parameters the absolute integral over the complement is of order $n/\sqrt{\log n}$, while the required control is for the oscillatory integral on the smaller $n/\log n$ scale. The lower bound also leaves the leading asymptotic unresolved.

#### Sources

- Euler’s 1747 conjecture on sums of integers with restricted prime factors: https://hexagonmath.org/pdf/2611.00370v1; p. 1, §1, opening definitions; p. 1, Abstract and §1, opening paragraph; p. 1, §1, definition of admissible summands and Euler formulation, p. 1, Lemma 2.1, scaling step; p. 1, §1, Letter 115 and editorial note 10, p. 8, Reference [4]; p. 1, §1, Euler’s divisor condition and the definition of admissible summands; p. 1, §1, prior result of Dietmann and Elsholtz, p. 8, Reference [2]; p. 1, Abstract and Theorem 1.1, p. 8, Proof of Theorem 1.1; p. 1, §2, first sentence; p. 1, Lemma 2.1, first sentence of the proof; p. 1, Lemma 2.1, statement and scaling step; p. 2, §2, definition preceding (2.1) and notation in (2.1); p. 2, §2, equation (2.1); p. 2, §2, text between (2.1) and (2.2); p. 2, §2, definition of the mixed set preceding (2.2); p. 2, §2, equation (2.2); p. 2, §2, definition of the exceptional sets following (2.2); p. 2, §2, quadratic nonresidue observation preceding (2.3); p. 2, §2, conclusion immediately preceding (2.3); p. 2, §2, equation (2.3), p. 7, §6, application of (2.2) and (2.3); p. 2, §3.1, Hamilton algebra and reduced norm; p. 2, §3.1, displayed definition of the order; p. 2, §3.1, enumeration of units; p. 2, §3.1, rounding and the strict norm bound; p. 2, §3.1, consequence of norm-Euclidean division; p. 2, §3.1, definition of the norm shell preceding (3.2); p. 2, §3.1, equation (3.2) and inverse description; p. 2, §3.1, last paragraph; p. 2, §3.1, definitions of the projective group and reduction, p. 3, §3.1, definitions of the unit image, quotient, and counting inner product; p. 3, §3.1, scalar reductions and equation (3.3); p. 3, §3.2, equation (3.4); p. 3, §3.2, first three claims following (3.4); p. 3, §3.2, constant eigenvalue following (3.4); p. 3, §3.2, definition of the character before Lemma 3.2; p. 3, §3.2, justification of the definition of the determinant character; p. 3, §3.2, character eigenvalue before Lemma 3.2; p. 3, Lemma 3.2, proof, definition of the compact open level; p. 3, Lemma 3.2, equation (3.5) and stabilizer paragraph; p. 3, Lemma 3.2, paragraph following the stabilizer description; p. 3, Lemma 3.2, paragraph on one-dimensional automorphic representations; p. 3, Lemma 3.2, invocation of Jacquet–Langlands and the weight-two setting, p. 8, References [3] and [5]; p. 3, Lemma 3.2, opening of the Ramanujan–Petersson paragraph, p. 8, Reference [1]; p. 3, Lemma 3.2, displayed local eigenvalue and triangular-coset calculation; p. 3, Lemma 3.2, last paragraph, local bound before multiplication; p. 3, Lemma 3.2, statement and last sentence of its proof; p. 4, §3.3, opening definitions of the two subgroups; p. 4, §3.3, order assertion immediately following the subgroup definitions; p. 4, §3.3, description of pair vanishing and multiplication by 1 + i; p. 4, §3.3, unit-image intersection preceding the orbit definition; p. 4, §3.3, displayed orbit and indicator definitions; p. 4, §3.3, density formula, orbit count, and the case $p = 3$; p. 4, §3.3, class multiplicity preceding (3.6); p. 4, §3.3, equation (3.6); p. 4, §3.3, invariance and equation (3.7); p. 4, §3.3, norm surjectivity and balance paragraph following (3.7); p. 4, §3.3, centered indicator and its norm before (3.8); p. 4, §3.3, equation (3.8) and case $p = 3$; p. 4, Completion of Proposition 3.1, formula for the dividing-prime obstruction count; p. 4, Completion of Proposition 3.1, divisor-sum ratio and last inequality; p. 2, Proposition 3.1, equation (3.1), p. 4, §3.3 and completion of Proposition 3.1; p. 4, §4, definition preceding Lemma 4.1; p. 4, Lemma 4.1, proof, orbit representatives, label and norm identity; p. 4, Lemma 4.1, statement and last two lines; p. 5, §4, definitions of M(n) and r₂(u) on the first lines; p. 5, §4, two-square formula application before Lemma 4.2; p. 5, Lemma 4.2, proof, per-prime count and upper limit on the prime; p. 5, Lemma 4.2, last line of proof; p. 5, Lemma 4.2, equation (4.1); p. 5, Lemma 5.1, first two proof paragraphs before the table; p. 5, Lemma 5.1, ratio test and table of maximizing positive exponents; p. 5, Lemma 5.1, absent-prime convention and displayed fifth-power products; p. 5, Lemma 5.1, equation (5.1); p. 6, Lemma 5.2, definition of the residue set and counting function; p. 6, Lemma 5.2, first sentence of proof; p. 6, Lemma 5.2, one-period check and interval estimate; p. 6, Lemma 5.2, equation (5.2); p. 6, Lemma 5.2, displayed partial-summation identity and upper bound; p. 6, Lemma 5.2, equation (5.3); p. 6, Lemma 5.2, equation (5.4) and final finite sum through 60; p. 6, Proposition 6.1, choice of cutoff and equation (6.1); p. 6, Proposition 6.1, equation (6.2), p. 7, §6, prime-count term preceding the numerical closure; p. 7, §6, three power comparisons for X at least 64; p. 7, §6, combined numerical estimate at the end of Proposition 6.1; p. 1, Abstract and paragraph after Theorem 1.1, p. 6, Proposition 6.1, statement, p. 7, End of Proposition 6.1; p. 7, §7, definition of H and equation (7.1), p. 8, Proposition 7.2, index range in the proof; p. 1, Abstract, finite certificate count, p. 7, §7, definition of H, p. 8, Proposition 7.2, index range in the proof; p. 7, §7, paragraph following (7.1); p. 7, Lemma 7.1, proof, multiplicity, size, and least-prime observation; p. 7, Lemma 7.1, statement; p. 7, §7, definition of J after Lemma 7.1; p. 7, §7, displayed set of possible summands after the definition of J; p. 7, §7, definition of U(a) in equation (7.2); p. 7, §7, paragraph after (7.2), p. 8, Proposition 7.2, vanishing-factor criterion; p. 7, §7, progression below (7.3); p. 7, §7, identification of indicators with the progression sieve; p. 7, §7, number of primes in the sieve after (7.3), p. 8, Paragraph after Table 1, retained-index count; p. 7, §7, initialization and update in equation (7.3); p. 7, §7, equivalence of equations (7.2) and (7.3), p. 8, Table 1 caption; p. 8, Table 1, all twelve entries, and paragraph after it; p. 1, Abstract, finite certificate coverage, p. 8, Proposition 7.2, statement and stated certificate implication; p. 1, §1, first displayed definitions and Theorem 1.1; p. 1, §1, definition of admissible summands and Euler formulation; p. 1, Lemma 2.1, scaling step; p. 1, §1, historical paragraph and Theorem 1.1, and p. 8, reference [4]; p. 1, §1, paragraph before Theorem 1.1, and p. 8, reference [2]; PDF p. 1, Abstract and Theorem 1.1, and p. 8, Proof of Theorem 1.1; p. 2, §2, equation (2.3), and p. 7, §6, application of (2.2) and (2.3); p. 2, §3.1, sentence immediately after the displayed Hurwitz order; p. 2, §3.1, paragraph beginning “The order H is norm-Euclidean”; pp. 2–3, §3.1, final display on p. 2 and definitions surrounding (3.3) on p. 3; pp. 2–3, §3.1, reduction setup and equation (3.3); p. 3, §3.2, displayed definition of the character before Lemma 3.2; p. 3, §3.2, displayed determinant character and the justification immediately following it; p. 3, Lemma 3.2, equation (3.5) and the following paragraph; p. 3, Lemma 3.2, paragraph following the stabilizer and last sentence of the proof; p. 3, Lemma 3.2, paragraph beginning with the one-dimensional automorphic representations; p. 3, proof of Lemma 3.2, paragraph on the remaining representations; p. 3, Lemma 3.2, opening of the Ramanujan–Petersson paragraph, and p. 8, Reference [1]; PDF p. 3, §3.2, Lemma 3.2; p. 4, §3.3, opening paragraph; right multiplication as in p. 2, §3.1, (3.2); p. 4, §3.3, the two invariance assertions and (3.7); p. 4, §3.3, paragraph between (3.7) and (3.8); PDF p. 4, §3.3, equations (3.7)–(3.8) and the sentence following (3.8); p. 4, Completion of the proof of Proposition 3.1, divisor-sum ratio and final inequality; p. 2, Proposition 3.1, equation (3.1), and p. 4, §3.3 and completion of Proposition 3.1; p. 5, §4, definitions of M(n) and r₂(u) immediately before Lemma 4.2; PDF p. 5, Lemma 4.2, proof through the bound on p; PDF p. 5, Lemma 4.2, equation (4.1) and its proof; p. 5, Lemma 5.1, equation (5.1) and proof; PDF p. 6, proof of Lemma 5.2, from the one-period check through the interval estimate; p. 6, Lemma 5.2, equation (5.2) and its proof through the periodicity argument; PDF p. 6, proof of Lemma 5.2, displayed identity and upper bound after “Partial summation yields”; p. 6, Lemma 5.2, equation (5.3) and the sentence following the partial-summation display; p. 6, Proposition 6.1, equation (6.2), and p. 7, opening sentence; p. 1, Abstract and paragraph after Theorem 1.1, p. 2, equations (2.2)–(2.3), pp. 6–7, Proposition 6.1; p. 7, §7, definition of H and (7.1), and p. 8, Proposition 7.2, first sentence of proof; p. 1, Abstract, finite certificate count, p. 7, §7, definition of H, and p. 8, Proposition 7.2, statement and first sentence of proof; p. 7, §7, proof of Lemma 7.1, first four sentences; p. 7, §7, Lemma 7.1 (statement and proof); p. 7, §7, equation (7.2) and its preceding sentence; p. 7, §7, paragraph after (7.2), and p. 8, Proposition 7.2, vanishing-factor criterion; p. 7, §7, equation (7.1) and the progression following (7.3); p. 7, §7, progression below (7.3), and p. 8, first sentence after Table 1; p. 7, §7, equations (7.1)–(7.3); p. 8, Table 1 and the terminal-empty-set sentence immediately after it; p. 1, Abstract, finite certificate coverage, pp. 7–8, (7.2), Table 1 and Proposition 7.2, statement and proof. Reading limits: Read all eight frozen PDF pages and all 99 original coverage records. Formulas were checked against the rendered pages and anchors against the frozen extraction. Recomputed the finite certificate, fifth-power products, residue discrepancy and closing rational inequalities independently.
- Dietmann and Elsholtz, Sums of two numbers having only prime factors congruent to one modulo four: https://www.math.tugraz.at/~elsholtz/WWW/papers/greaves20.pdf; Author version, pp. 1–3, abstract, unnumbered Theorem and proof, equation (1), final paragraph before References. Reading limits: Read the three-page extracted author version, including the lower-bound argument and the explicit complementary-prime question. Greaves’s underlying proof was outside this reading.
- Euler and the Four-Squares Theorem, MathOverflow: https://mathoverflow.net/questions/37278/euler-and-the-four-squares-theorem; Lucia’s answer of 3 September 2013, opening formulation, Conclusion and Remarks. Reading limits: Read the stated weighted problem, resulting lower bound and asymptotic remark in the original answer. Used for priority and problem scope. The linked analytic estimates were outside scope.
- Ramaré and Viswanadham, The trigonometric polynomial on sums of two squares, an additive problem and generalisation: https://arxiv.org/html/2509.23260v1; §1, support of $b$, equations (5)–(6), and Theorem 1.6; §8, Lemma 8.2 and equations (15)–(17); §13, Lemma 13.1 and equations (33)–(36). Reading limits: Checked the passages on the summand set, the fixed odd-modulus estimate, and the ternary use of restriction. The underlying character-sum and restriction proofs were outside scope.
- Berndt and Moree, Sums of two squares and the tau-function: Ramanujan’s trail: https://arxiv.org/pdf/2409.03428; arXiv v3, §1, equations (1.1)–(1.2) and the two-square criterion; §4, Theorem 4.1, and §7.5, Theorem 7.2. Reading limits: Checked Landau’s stated asymptotic, its constant and the exact counting set. Also checked the general multiplicative-set argument cited in the draft. The repaired proof uses the §1 statement.
- Kedlaya, Notes on analytic number theory, Primes in arithmetic progressions: https://kskedlaya.org/ant/chap-primes-in-ap.html; Chapter 4, §4.4, Theorem 4.12 and the coprimality condition in its proof. Reading limits: Checked the theorem statement and the condition needed for residue 3 modulo 4.
- Greaves, On the representation of a number in the form x²+y²+p²+q² where p, q are odd primes: https://bibliotekanauki.pl/articles/1393472.pdf; Acta Arithmetica 29 (1976), §1, Theorem; §6, conclusion and equation (6.1). Reading limits: Checked the theorem in the digitized paper and its concluding formula for the positive lower-bound constant. The sieve proof was outside scope.

## 3. Potential solutions to open questions

### Potential solution 01

#### Research question

Let $\mathcal P_3$ be the set of primes congruent to $3$ modulo $4$, and let $B$ be the set of positive integers whose prime divisors all lie in $\mathcal P_3$, including $1$. Does every sufficiently large positive integer $n\equiv2\pmod4$ belong to $B+B$?

#### Question source

**Origin:** External literature

https://www.math.tugraz.at/~elsholtz/WWW/papers/greaves20.pdf; Dietmann–Elsholtz, author version p. 3, final paragraph before References

#### Why it matters

Dietmann and Elsholtz posed this question after proving eventual coverage for summands whose prime divisors are all $1$ modulo $4$. The partial results bound the number of possible exceptions and show that every compatible residue class contains infinitely many represented targets, even when a finite set of summands is excluded.

#### Originality

Dietmann and Elsholtz pose the question in the final paragraph before their references. The frozen Howe–Huffman–Kohlmeyer–Kruer article cites their theorem for the $1$ modulo $4$ prime class in §1. The complementary question and the arguments below were absent from the eight-page text reviewed. The exceptional-set estimate comes from established literature. Priority for the elementary deductions was outside the scope of the targeted search.

#### Current knowledge

Dietmann and Elsholtz left eventual coverage open. The Liu–Zhan estimate, in the even-target formulation recorded by Nguyen, yields a power-saving exceptional-set bound for representations by two primes in the complementary class. A targeted search found no proof or disproof of eventual coverage for $B+B$.

#### Potential solution

**Solution scope:** partial

**Evidence status:** Proved partial result

There is a constant $\eta>0$ such that all but $O(X^{1-\eta})$ of the positive integers $n\le X$ with $n\equiv2\pmod4$ are sums of two primes in $\mathcal P_3$. For every integer $M\ge1$, every integer $n_0\equiv2\pmod4$, and every finite $F\subset B$, there are infinitely many positive integers $n\equiv n_0\pmod M$ with $n\equiv2\pmod4$ that are sums of two coprime squarefree products of two primes in $\mathcal P_3$ and for which no representation in $B+B$ uses an element of $F$. Every $n=2m$ with $m\in B$ also has the exact representation $m+m$.

#### Argument and next steps

Apply the even-target Goldbach estimate with modulus $4$ and both prime residues equal to $3$. For the semiprime construction, impose $n\equiv a\pmod{q_a}$ for each $a\in F$, where the $q_a$ are distinct primes congruent to $1$ modulo $4$ and coprime to $4M$. A representation using $a$ would force the other summand to be divisible by $q_a$. Split the refined target residue into two units congruent to $1$ modulo $4$ by choosing local residues at the prime powers. Dirichlet’s theorem realizes each unit as a product of two primes in $\mathcal P_3$, with all four factors distinct. Fix three of the primes and vary the fourth to produce infinitely many sums. The diagonal representation follows directly from $m\in B$.

#### Proof sketch or overall strategy

Specialize the even-target Goldbach estimate to modulus $4$. Independently, use the Chinese remainder theorem to exclude a prescribed finite set of summands and split the resulting target class into units. Apply Dirichlet’s theorem to realize those units as coprime squarefree semiprimes.

#### Numbered argument

1. In the even-target estimate take $k=4$ and $b_1=b_2=3$. Both classes are reduced, their sum is $2$ modulo $4$, and $4<X^\delta$ for all sufficiently large $X$. Every positive integer $n\equiv2\pmod4$ is even, so $O(X^{1-\eta}/\varphi(4))=O(X^{1-\eta})$ bounds the exceptions in the entire target class. Both primes in every such representation belong to $B$. [restricted-goldbach-bound, prime-class-and-targets]
2. Fix $M,n_0,F$ and put $Q_0=4M$. Dirichlet’s theorem modulo $4$ gives enough distinct primes $q_a\equiv1\pmod4$, indexed by $a\in F$, to choose them all outside the finite set of prime divisors of $Q_0$. With $Q=Q_0\prod_{a\in F}q_a$, the Chinese remainder theorem gives $c$ modulo $Q$ satisfying $c\equiv n_0\pmod{Q_0}$ and $c\equiv a\pmod{q_a}$ for each $a\in F$. When $F$ is empty take $Q=Q_0$ and $c=n_0$ modulo $Q$. If $n\equiv c\pmod Q$ had a representation using $a\in F$, its other summand would be a positive multiple of $q_a$ and would therefore lie outside $B$. [prime-class-and-targets, dirichlet-primes-in-progressions, chinese-remainder, prime-factorization]
3. At the full power $2^e$ dividing $Q$, prescribe $u\equiv1\pmod{2^e}$. Since $e\ge2$ and $c\equiv2\pmod4$, both $u$ and $c-u$ are odd and congruent to $1$ modulo $4$. For each full odd prime-power factor $\ell^j$ of $Q$, choose a class of $u$ modulo $\ell^j$ whose reduction modulo $\ell$ avoids $0$ and $c$. There are at least three classes modulo $\ell$ and at most two exclusions. Combine the choices using the Chinese remainder theorem and put $v=c-u$ modulo $Q$. No prime divisor of $Q$ divides $u$ or $v$, so both classes are units by Bézout’s identity. [step:2, prime-factorization, chinese-remainder, bezout-identity]
4. Use Dirichlet’s theorem modulo $4$ to choose distinct primes $r,w\in\mathcal P_3$ with $r,w\nmid Q$. The classes $r^{-1}u$ and $w^{-1}v$ modulo $Q$ are units. They reduce to $3$ modulo $4$ because $u,v\equiv1\pmod4$, $4\mid Q$, and $3^{-1}\equiv3\pmod4$. Dirichlet’s theorem modulo $Q$ gives a prime $s$ in the first class outside $\{r,w\}$ and infinitely many primes $t$ in the second class outside $\{r,w,s\}$. Then $n=rs+wt\equiv c\pmod Q$. The four distinct primes all lie in $\mathcal P_3$, so the two products are coprime and squarefree. The values of $n$ are distinct as $t$ varies. Step 2 gives the required target congruences and excludes every summand in $F$. [step:2, step:3, dirichlet-primes-in-progressions, prime-factorization, bezout-identity, prime-class-and-targets]
5. For any integer $H\ge1$, take $F=B\cap[1,H]$ in the construction. Every representation of a resulting target in $B+B$ has both summands greater than $H$. For the separate diagonal family, $m\in B$ implies that $m$ is odd because $2\notin\mathcal P_3$. Thus $2m\equiv2\pmod4$ and $2m=m+m\in B+B$. [step:4, prime-class-and-targets]

#### Immediate dependencies

- **prime-class-and-targets:** $\mathcal P_3$ is the set of primes congruent to $3$ modulo $4$. The set $B$ consists of positive integers all of whose prime divisors lie in $\mathcal P_3$, with $1$ included. The set $B+B$ consists of sums of two members of $B$. The progression hypotheses are $M\ge1$ integral, $n_0\equiv2\pmod4$ integral, and $F\subset B$ finite. Source: self-contained; Question and partial-solution statement. Reading limits: Definitions and hypotheses stipulated in the direction.
- **restricted-goldbach-bound:** For some positive constants $\delta$ and $\eta$, the Liu–Zhan estimate bounds the number of positive even $n\le X$ with $n\equiv b_1+b_2\pmod k$ and no representation $n=p_1+p_2$ by primes $p_i\equiv b_i\pmod k$ by $O(X^{1-\eta}/\varphi(k))$ when $k<X^\delta$ and $b_1,b_2$ are reduced classes modulo $k$. Here $\varphi$ is Euler’s totient. Only $k=4$ and $b_1=b_2=3$ are needed. Source: https://pepite-depot.univ-lille.fr/LIBRE/EDMADIS/2024/2024ULILB033.pdf; Nguyen, p. 21, opening of Chapter 2, definition of $E_{q,a,b}(x)$ and the estimate attributed to [31]. Reduced classes are explicit in Bauer–Wang, p. 227, definition of $E_k(X)$ before (1.2).. Reading limits: Checked the even-target restriction and estimate in Nguyen and the reduced-class condition and modulus range in Bauer–Wang. The original Liu–Zhan chapter and proof were not directly available.
- **dirichlet-primes-in-progressions:** For a positive integer $k$ and an integer $h$ with $\gcd(h,k)=1$, infinitely many primes are congruent to $h$ modulo $k$. Source: https://dlmf.nist.gov/27.11; §27.11, paragraph following (27.11.11). Reading limits: Checked the theorem statement and its coprimality and positive-modulus hypotheses.
- **chinese-remainder:** For a finite list of pairwise coprime positive moduli, any tuple of residue classes determines a unique class modulo the product. Source: math:thm-chinese-remainder-theorem; Statement, bijectivity of simultaneous reduction. Reading limits: Checked the published statement and the pairwise coprimality of both lists of moduli used here.
- **prime-factorization:** Each positive integer is a product of primes with a unique multiset of factors. The empty product is $1$. Source: math:thm-fundamental-theorem-of-arithmetic; Statement, clauses 1 and 2 and the empty-product case. Reading limits: Checked the existence and uniqueness clauses and their use for the prime-power factors, divisibility, coprimality, and squarefreeness.
- **bezout-identity:** For integers $h,k$ with $k\ge1$ and $\gcd(h,k)=1$, Bézout’s identity gives integers $x,y$ with $hx+ky=1$. Reducing modulo $k$ gives the inverse of the class of $h$. Source: math:thm-bezout-identity; Statement, equation $ax_0+by_0=\gcd(a,b)$. Reading limits: Checked the published identity for a pair with at least one nonzero entry and its reduction in the coprime case.

#### Independent review

**Decision:** repair

The draft imported the Goldbach bound with all positive targets in the specified congruence class. For $k=3$ and $b_1=b_2=1$, every positive $n\equiv5\pmod6$ would be counted as an exception because both allowed primes are odd. This gives $X/6+O(1)$ exceptions and contradicts the imported power saving as worded. Nguyen’s account of the Liu–Zhan bound explicitly counts even targets. The repair uses that formulation at the fixed modulus $4$, which preserves the claimed exceptional-set bound and all of the elementary conclusions.

**Dependency review:** The repaired Goldbach input applies because $3$ is a reduced class modulo $4$ and every target congruent to $3+3\pmod4$ is even. The first Chinese remainder application uses pairwise coprime moduli, and the second uses the distinct prime-power factors of the refined modulus. At an odd prime there are at most two forbidden residues, so the unit decomposition also works at $3$. Bézout gives the inverses used in the prime progressions, whose reduced classes satisfy Dirichlet’s hypotheses. Positivity makes the forbidden-summand divisibility argument valid, and unique factorization verifies squarefreeness, coprimality, and the diagonal case. The frozen supplier graph for the three library inputs is acyclic and reaches no local article item. The argument uses neither the frozen article’s theorem nor the open question as a premise.

**Review reading limits:** Read the extracted text of all eight frozen article pages and inspected the rendered first page for the comparison with Theorem 1.1. Read the relevant passages in Dietmann–Elsholtz, DLMF §27.11, Bauer–Wang §1 and reference [8], and Nguyen’s Chapter 2 and reference [31]. Checked the three immediate library statements against the frozen bindings and worked through the five argument steps. The original Liu–Zhan chapter and proof were not directly available. The targeted literature search did not identify a resolution of eventual coverage and does not establish worldwide priority for the elementary construction.

#### Author and reviewer gaps

No remaining gaps were reported within the stated scope.

#### Remaining gaps

The exceptional-set estimate permits infinitely many exceptions. The congruence construction varies the target within its progression, and the diagonal representation covers only targets with $n/2\in B$. It remains unresolved whether each sufficiently large prescribed target has a representation. Taking $F=B\cap[1,H]$ also shows that every fixed bound $H$ on the smaller summand fails for arbitrarily large represented targets.

#### Sources

- Euler’s 1747 conjecture on sums of integers with restricted prime factors: https://hexagonmath.org/pdf/2611.00370v1; p. 1, §1, opening definitions; p. 1, Abstract and §1, opening paragraph; p. 1, §1, definition of admissible summands and Euler formulation, p. 1, Lemma 2.1, scaling step; p. 1, §1, Letter 115 and editorial note 10, p. 8, Reference [4]; p. 1, §1, Euler’s divisor condition and the definition of admissible summands; p. 1, §1, prior result of Dietmann and Elsholtz, p. 8, Reference [2]; p. 1, Abstract and Theorem 1.1, p. 8, Proof of Theorem 1.1; p. 1, §2, first sentence; p. 1, Lemma 2.1, first sentence of the proof; p. 1, Lemma 2.1, statement and scaling step; p. 2, §2, definition preceding (2.1) and notation in (2.1); p. 2, §2, equation (2.1); p. 2, §2, text between (2.1) and (2.2); p. 2, §2, definition of the mixed set preceding (2.2); p. 2, §2, equation (2.2); p. 2, §2, definition of the exceptional sets following (2.2); p. 2, §2, quadratic nonresidue observation preceding (2.3); p. 2, §2, conclusion immediately preceding (2.3); p. 2, §2, equation (2.3), p. 7, §6, application of (2.2) and (2.3); p. 2, §3.1, Hamilton algebra and reduced norm; p. 2, §3.1, displayed definition of the order; p. 2, §3.1, enumeration of units; p. 2, §3.1, rounding and the strict norm bound; p. 2, §3.1, consequence of norm-Euclidean division; p. 2, §3.1, definition of the norm shell preceding (3.2); p. 2, §3.1, equation (3.2) and inverse description; p. 2, §3.1, last paragraph; p. 2, §3.1, definitions of the projective group and reduction, p. 3, §3.1, definitions of the unit image, quotient, and counting inner product; p. 3, §3.1, scalar reductions and equation (3.3); p. 3, §3.2, equation (3.4); p. 3, §3.2, first three claims following (3.4); p. 3, §3.2, constant eigenvalue following (3.4); p. 3, §3.2, definition of the character before Lemma 3.2; p. 3, §3.2, justification of the definition of the determinant character; p. 3, §3.2, character eigenvalue before Lemma 3.2; p. 3, Lemma 3.2, proof, definition of the compact open level; p. 3, Lemma 3.2, equation (3.5) and stabilizer paragraph; p. 3, Lemma 3.2, paragraph following the stabilizer description; p. 3, Lemma 3.2, paragraph on one-dimensional automorphic representations; p. 3, Lemma 3.2, invocation of Jacquet–Langlands and the weight-two setting, p. 8, References [3] and [5]; p. 3, Lemma 3.2, opening of the Ramanujan–Petersson paragraph, p. 8, Reference [1]; p. 3, Lemma 3.2, displayed local eigenvalue and triangular-coset calculation; p. 3, Lemma 3.2, last paragraph, local bound before multiplication; p. 3, Lemma 3.2, statement and last sentence of its proof; p. 4, §3.3, opening definitions of the two subgroups; p. 4, §3.3, order assertion immediately following the subgroup definitions; p. 4, §3.3, description of pair vanishing and multiplication by 1 + i; p. 4, §3.3, unit-image intersection preceding the orbit definition; p. 4, §3.3, displayed orbit and indicator definitions; p. 4, §3.3, density formula, orbit count, and the case $p = 3$; p. 4, §3.3, class multiplicity preceding (3.6); p. 4, §3.3, equation (3.6); p. 4, §3.3, invariance and equation (3.7); p. 4, §3.3, norm surjectivity and balance paragraph following (3.7); p. 4, §3.3, centered indicator and its norm before (3.8); p. 4, §3.3, equation (3.8) and case $p = 3$; p. 4, Completion of Proposition 3.1, formula for the dividing-prime obstruction count; p. 4, Completion of Proposition 3.1, divisor-sum ratio and last inequality; p. 2, Proposition 3.1, equation (3.1), p. 4, §3.3 and completion of Proposition 3.1; p. 4, §4, definition preceding Lemma 4.1; p. 4, Lemma 4.1, proof, orbit representatives, label and norm identity; p. 4, Lemma 4.1, statement and last two lines; p. 5, §4, definitions of M(n) and r₂(u) on the first lines; p. 5, §4, two-square formula application before Lemma 4.2; p. 5, Lemma 4.2, proof, per-prime count and upper limit on the prime; p. 5, Lemma 4.2, last line of proof; p. 5, Lemma 4.2, equation (4.1); p. 5, Lemma 5.1, first two proof paragraphs before the table; p. 5, Lemma 5.1, ratio test and table of maximizing positive exponents; p. 5, Lemma 5.1, absent-prime convention and displayed fifth-power products; p. 5, Lemma 5.1, equation (5.1); p. 6, Lemma 5.2, definition of the residue set and counting function; p. 6, Lemma 5.2, first sentence of proof; p. 6, Lemma 5.2, one-period check and interval estimate; p. 6, Lemma 5.2, equation (5.2); p. 6, Lemma 5.2, displayed partial-summation identity and upper bound; p. 6, Lemma 5.2, equation (5.3); p. 6, Lemma 5.2, equation (5.4) and final finite sum through 60; p. 6, Proposition 6.1, choice of cutoff and equation (6.1); p. 6, Proposition 6.1, equation (6.2), p. 7, §6, prime-count term preceding the numerical closure; p. 7, §6, three power comparisons for X at least 64; p. 7, §6, combined numerical estimate at the end of Proposition 6.1; p. 1, Abstract and paragraph after Theorem 1.1, p. 6, Proposition 6.1, statement, p. 7, End of Proposition 6.1; p. 7, §7, definition of H and equation (7.1), p. 8, Proposition 7.2, index range in the proof; p. 1, Abstract, finite certificate count, p. 7, §7, definition of H, p. 8, Proposition 7.2, index range in the proof; p. 7, §7, paragraph following (7.1); p. 7, Lemma 7.1, proof, multiplicity, size, and least-prime observation; p. 7, Lemma 7.1, statement; p. 7, §7, definition of J after Lemma 7.1; p. 7, §7, displayed set of possible summands after the definition of J; p. 7, §7, definition of U(a) in equation (7.2); p. 7, §7, paragraph after (7.2), p. 8, Proposition 7.2, vanishing-factor criterion; p. 7, §7, progression below (7.3); p. 7, §7, identification of indicators with the progression sieve; p. 7, §7, number of primes in the sieve after (7.3), p. 8, Paragraph after Table 1, retained-index count; p. 7, §7, initialization and update in equation (7.3); p. 7, §7, equivalence of equations (7.2) and (7.3), p. 8, Table 1 caption; p. 8, Table 1, all twelve entries, and paragraph after it; p. 1, Abstract, finite certificate coverage, p. 8, Proposition 7.2, statement and stated certificate implication; p. 1, §1, first displayed definitions and Theorem 1.1; p. 1, §1, definition of admissible summands and Euler formulation; p. 1, Lemma 2.1, scaling step; p. 1, §1, historical paragraph and Theorem 1.1, and p. 8, reference [4]; p. 1, §1, paragraph before Theorem 1.1, and p. 8, reference [2]; PDF p. 1, Abstract and Theorem 1.1, and p. 8, Proof of Theorem 1.1; p. 2, §2, equation (2.3), and p. 7, §6, application of (2.2) and (2.3); p. 2, §3.1, sentence immediately after the displayed Hurwitz order; p. 2, §3.1, paragraph beginning “The order H is norm-Euclidean”; pp. 2–3, §3.1, final display on p. 2 and definitions surrounding (3.3) on p. 3; pp. 2–3, §3.1, reduction setup and equation (3.3); p. 3, §3.2, displayed definition of the character before Lemma 3.2; p. 3, §3.2, displayed determinant character and the justification immediately following it; p. 3, Lemma 3.2, equation (3.5) and the following paragraph; p. 3, Lemma 3.2, paragraph following the stabilizer and last sentence of the proof; p. 3, Lemma 3.2, paragraph beginning with the one-dimensional automorphic representations; p. 3, proof of Lemma 3.2, paragraph on the remaining representations; p. 3, Lemma 3.2, opening of the Ramanujan–Petersson paragraph, and p. 8, Reference [1]; PDF p. 3, §3.2, Lemma 3.2; p. 4, §3.3, opening paragraph; right multiplication as in p. 2, §3.1, (3.2); p. 4, §3.3, the two invariance assertions and (3.7); p. 4, §3.3, paragraph between (3.7) and (3.8); PDF p. 4, §3.3, equations (3.7)–(3.8) and the sentence following (3.8); p. 4, Completion of the proof of Proposition 3.1, divisor-sum ratio and final inequality; p. 2, Proposition 3.1, equation (3.1), and p. 4, §3.3 and completion of Proposition 3.1; p. 5, §4, definitions of M(n) and r₂(u) immediately before Lemma 4.2; PDF p. 5, Lemma 4.2, proof through the bound on p; PDF p. 5, Lemma 4.2, equation (4.1) and its proof; p. 5, Lemma 5.1, equation (5.1) and proof; PDF p. 6, proof of Lemma 5.2, from the one-period check through the interval estimate; p. 6, Lemma 5.2, equation (5.2) and its proof through the periodicity argument; PDF p. 6, proof of Lemma 5.2, displayed identity and upper bound after “Partial summation yields”; p. 6, Lemma 5.2, equation (5.3) and the sentence following the partial-summation display; p. 6, Proposition 6.1, equation (6.2), and p. 7, opening sentence; p. 1, Abstract and paragraph after Theorem 1.1, p. 2, equations (2.2)–(2.3), pp. 6–7, Proposition 6.1; p. 7, §7, definition of H and (7.1), and p. 8, Proposition 7.2, first sentence of proof; p. 1, Abstract, finite certificate count, p. 7, §7, definition of H, and p. 8, Proposition 7.2, statement and first sentence of proof; p. 7, §7, proof of Lemma 7.1, first four sentences; p. 7, §7, Lemma 7.1 (statement and proof); p. 7, §7, equation (7.2) and its preceding sentence; p. 7, §7, paragraph after (7.2), and p. 8, Proposition 7.2, vanishing-factor criterion; p. 7, §7, equation (7.1) and the progression following (7.3); p. 7, §7, progression below (7.3), and p. 8, first sentence after Table 1; p. 7, §7, equations (7.1)–(7.3); p. 8, Table 1 and the terminal-empty-set sentence immediately after it; p. 1, Abstract, finite certificate coverage, pp. 7–8, (7.2), Table 1 and Proposition 7.2, statement and proof. Reading limits: Read all eight frozen PDF pages and all 99 original coverage records. Formulas were checked against the rendered pages and anchors against the frozen extraction. Recomputed the finite certificate, fifth-power products, residue discrepancy and closing rational inequalities independently.
- Dietmann and Elsholtz, Sums of two numbers having only prime factors congruent to one modulo four: https://www.math.tugraz.at/~elsholtz/WWW/papers/greaves20.pdf; Author version, pp. 1–3, abstract, unnumbered Theorem and proof, equation (1), final paragraph before References. Reading limits: Read the three-page extracted author version, including the lower-bound argument and the explicit complementary-prime question. Greaves’s underlying proof was outside this reading.
- NIST Digital Library of Mathematical Functions, Asymptotic Formulas: Partial Sums: https://dlmf.nist.gov/27.11; §27.11, paragraph following (27.11.11), Dirichlet’s theorem on primes in arithmetic progressions. Reading limits: Read the stated theorem and its coprimality and positive-modulus conditions. Used to choose primes in specified unit classes.
- Claus Bauer and Yonghui Wang, The binary Goldbach conjecture with primes in arithmetic progressions with large modulus: https://www.impan.pl/shop/publication/transaction/download/product/82349?download.pdf=; p. 227, §1, definitions of $E_{k,b_1,b_2}(X)$ and $E_k(X)$ and equation (1.2); References, [8]. Reading limits: Checked the restricted-prime counting convention, reduced classes, and stated power saving. The displayed restricted exceptional set omits an explicit even-target condition. Nguyen’s formulation supplies that restriction.
- Thi Thu Nguyen, Goldbach representations: https://pepite-depot.univ-lille.fr/LIBRE/EDMADIS/2024/2024ULILB033.pdf; p. 21, Chapter 2, definition of $E_{q,a,b}(x)$ and the bound immediately following it; References, [31]. Reading limits: Read the opening statement of the even-target estimate and checked its attribution to Liu and Zhan. The underlying chapter and proof were outside direct access.

## Examples and counter examples

### The obstructing prime class

[PDF p. 1](https://hexagonmath.org/pdf/2611.00370v1#page=1) (§1, opening display defining $\mathcal P_3$ and $\mathcal A$)

#### Example

$7$ belongs to $\mathcal P_3$.

**Proof**

1. A composite $7$ would have a prime divisor at most $\sqrt7<3$. It is odd, so $2$ does not divide it.
2. Since $7=4+3$, it meets the congruence condition as well.

#### Counter example

The prime $5$ does not belong to $\mathcal P_3$.

**Proof**

1. $5$ is odd and $\sqrt5<3$, so it is prime.
2. It leaves remainder $1$ on division by $4$, whereas $\mathcal P_3$ requires remainder $3$.

### Admissible positive integers

[PDF p. 1](https://hexagonmath.org/pdf/2611.00370v1#page=1) (§1, opening display defining $\mathcal P_3$ and $\mathcal A$)

#### Example

$65$ belongs to $\mathcal A$.

**Proof**

1. $65=5\cdot13$ is positive. The factors are prime by trial division by the primes up to their square roots, which are $2$ for $5$ and $2,3$ for $13$.
2. Both prime factors leave remainder $1$ modulo $4$.

#### Counter example

$45$ does not belong to $\mathcal A$ even though $45\equiv1\pmod4$.

**Proof**

1. The positive integer $45$ factors as $3^2\cdot5$.
2. Its prime divisor $3$ leaves remainder $3$ modulo $4$, failing the condition on every prime divisor.

### The admissible sumset

[PDF p. 1](https://hexagonmath.org/pdf/2611.00370v1#page=1) (Theorem 1.1, displayed decomposition $n=a+b$ with $a,b\in\mathcal A$)

#### Example

$26$ belongs to $\mathcal A+\mathcal A$.

**Proof**

1. $13$ is a positive prime since it is divisible by neither $2$ nor $3$, the primes at most $\sqrt{13}$.
2. $13\equiv1\pmod4$, so the two admissible summands in $26=13+13$ give membership.

#### Counter example

The positive integer $12$ does not belong to $\mathcal A+\mathcal A$.

**Proof**

1. Every member of $\mathcal A$ is $1$ modulo $4$, since it is either $1$ or a product of primes each congruent to $1$ modulo $4$.
2. Hence every sum of two members is $2$ modulo $4$. The integer $12$ is $0$ modulo $4$.

### Euler’s restricted prime factor decomposition

[PDF p. 1](https://hexagonmath.org/pdf/2611.00370v1#page=1) (Theorem 1.1)

#### Example

Theorem 1.1 applies to $n=110$, for which $110=25+85$.

**Proof**

1. $110=4\cdot27+2$ is positive and is $2$ modulo $4$.
2. The sum is $25+85=110$, and the summands are positive with factorizations $25=5^2$ and $85=5\cdot17$.
3. The factors $5,17$ are prime by trial division by the primes up to their square roots, namely $2$ for $5$ and $2,3$ for $17$. Each is $1$ modulo $4$, so both summands belong to $\mathcal A$.

### The divisor sum

[PDF p. 1](https://hexagonmath.org/pdf/2611.00370v1#page=1) (§2, first sentence, formula for $\sigma(u)$)

#### Example

$\sigma(9)=13$.

**Proof**

1. Since $9=3^2$, its positive divisors are $1,3,9$.
2. The defining sum is $1+3+9=13$.

#### Counter example

$\sigma(9)=12$ is an incorrect proposed value.

**Proof**

1. $3$ and $9$ contribute $12$, and $1$ also divides $9$.
2. The full divisor list of $3^2$ is $1,3,9$, which forces the value $13$.

### The divisor count

[PDF p. 1](https://hexagonmath.org/pdf/2611.00370v1#page=1) (§2, first sentence, formula for $\tau(u)$)

#### Example

$\tau(21)=4$.

**Proof**

1. $21=3\cdot7$, a product of distinct primes. A positive divisor chooses each of $3$ and $7$ to exponent $0$ or $1$.
2. The list $1,3,7,21$ has four entries.

#### Counter example

$\tau(21)=2$ is an incorrect proposed value.

**Proof**

1. $3$ and $7$ are positive divisors, and so are $1$ and $21$.
2. The four integers are distinct. The divisor count includes the two endpoint divisors along with the prime divisors.

### Signed ordered four-square representations

[PDF p. 2](https://hexagonmath.org/pdf/2611.00370v1#page=2) (§2, display defining $\mathcal R(n)$ before (2.1))

#### Example

$(-2,1,-1,0)$ belongs to $\mathcal R(6)$.

**Proof**

1. The input is $6=2\cdot3$ with odd part $3\in\mathcal P_3$, and all four coordinates are integers.
2. In the displayed order their squares sum to $4+1+1+0=6$.

#### Counter example

$(-2,1,-1,1)$ does not belong to $\mathcal R(6)$.

**Proof**

1. The tuple has four integer entries, in the ambient space $\mathbb Z^4$.
2. The sum of squares is $4+1+1+1=7$, so the required equality to $6$ fails.

### The four-square count

[PDF p. 2](https://hexagonmath.org/pdf/2611.00370v1#page=2) (Equation (2.1), $R(n):=|\mathcal R(n)|$)

#### Example

$R(2)=24$.

**Proof**

1. For $2=2\cdot1$, the positive odd part $1$ has no prime divisors. Each tuple at norm $2$ has exactly two entries of absolute value $1$ and two zeros, because all squares exceeding $1$ are at least $4$.
2. There are $\binom42=6$ ways to place the two nonzero entries and $2^2=4$ independent sign choices, so $|\mathcal R(2)|=24$.

#### Counter example

$R(2)=6$ is an incorrect proposed value.

**Proof**

1. The six choices of two positions account for the supports of the tuples.
2. On each support both assigned coordinates independently take either sign of $1$, yielding four distinct tuples per support and thus $24$ in all.

### Mixed-parity four-square representations

[PDF p. 2](https://hexagonmath.org/pdf/2611.00370v1#page=2) (§2, definition of $\mathcal R_{\mathrm{mix}}(n)$ before (2.2))

#### Example

$(1,0,0,-1)$ belongs to $\mathcal R_{\mathrm{mix}}(2)$.

**Proof**

1. The four entries are integral and the squares sum to $1+0+0+1=2$, with odd part $1$.
2. The first pair is odd–even and the second pair is even–odd, so both pairs meet the parity condition.

#### Counter example

$(1,-1,0,0)$ belongs to $\mathcal R(2)$ and falls outside $\mathcal R_{\mathrm{mix}}(2)$.

**Proof**

1. The entries are integers and their squares sum to $2$.
2. The first pair has two odd coordinates and the second pair has two even coordinates, so the opposite-parity requirement fails.

### The prime-obstruction count

[PDF p. 2](https://hexagonmath.org/pdf/2611.00370v1#page=2) (§2, definition of $b_p(n)$ immediately after (2.2))

#### Example

$b_3(18)=16$.

**Proof**

1. Here $18=2\cdot9$ has odd part $3^2$ and $3\in\mathcal P_3$. If one pair is divisible by $3$, the other pair has sum of squares $0$ modulo $3$. The only square residues are $0,1$, so that pair also has both coordinates divisible by $3$.
2. After dividing by $3$, the norm is $2$ and the parity condition is preserved. Each mixed pair contributes at least $1$ to this norm, so both pairs have norm $1$.
3. A norm-$1$ pair is one of $(1,0),(-1,0),(0,1),(0,-1)$. The two independent choices give $16$ distinct original tuples, each satisfying both divisibility conditions.

#### Counter example

$b_3(18)=32$ is an incorrect proposed value.

**Proof**

1. Here $18=2\cdot9$ has odd part $3^2$ and $3\in\mathcal P_3$. If one pair is divisible by $3$, the other pair has sum of squares $0$ modulo $3$. The only square residues are $0,1$, so that pair also has both coordinates divisible by $3$.
2. After dividing by $3$, the norm is $2$ and the parity condition is preserved. Each mixed pair contributes at least $1$ to this norm, so both pairs have norm $1$.
3. A norm-$1$ pair is one of $(1,0),(-1,0),(0,1),(0,-1)$. The two independent choices give $16$ distinct original tuples, each satisfying both divisibility conditions.
4. The word “or” specifies a union of tuples. The two pair conditions pick out the same $16$ tuples here, so adding the counts with multiplicity would count each tuple twice.

### Rational Hamilton quaternions

[PDF p. 2](https://hexagonmath.org/pdf/2611.00370v1#page=2) (§3.1, opening definition of $B$ with $i^2=j^2=-1$ and $k=ij=-ji$)

#### Example

$\tfrac12+2i-j+3k$ is an element of $B$.

**Proof**

1. Use the Hamilton basis $1,i,j,k$ with $ij=k=-ji$.
2. Its four coefficients $\tfrac12,2,-1,3$ are rational, as required for their linear combination to lie in $B$.

#### Counter example

The real Hamilton quaternion $\sqrt2+i$ lies outside the rational algebra $B$.

**Proof**

1. In the basis $1,i,j,k$ its scalar coordinate is $\sqrt2$. If $\sqrt2=a/b$ in lowest terms, $a^2=2b^2$ forces $a$ even and then $b$ even, a contradiction.
2. The real Hamilton basis is linearly independent, so no rational-coordinate expression can replace this scalar coordinate.

### Reduced quaternion norm

[PDF p. 2](https://hexagonmath.org/pdf/2611.00370v1#page=2) (§3.1, display defining the reduced norm)

#### Example

$\operatorname{nrd}(1+2i-j+3k)=15$.

**Proof**

1. The input has four rational coordinates $1,2,-1,3$ in the Hamilton basis.
2. Squaring all four coordinates and summing gives $1+4+1+9=15$.

#### Counter example

$\operatorname{nrd}(1+2i-j+3k)=14$ is an incorrect proposed value.

**Proof**

1. The scalar and the last two imaginary coordinates contribute $1+1+9=11$.
2. The $i$ coordinate contributes $2^2=4$, so the required total is $15$.

### The Hurwitz order

[PDF p. 2](https://hexagonmath.org/pdf/2611.00370v1#page=2) (§3.1, display defining $\mathcal H$)

#### Example

$\tfrac12(1+i-j+3k)$ lies in $\mathcal H$.

**Proof**

1. Its coordinates in $B$ are $\tfrac12,\tfrac12,-\tfrac12,\tfrac32$.
2. Each belongs to $\mathbb Z+\tfrac12$, so the tuple belongs to the half-integral part of $\mathcal H$.

#### Counter example

$\tfrac12(1+i)$ lies outside $\mathcal H$.

**Proof**

1. This rational quaternion has coordinates $\tfrac12,\tfrac12,0,0$.
2. The first two coordinates are strict half-integers and the last two are integers, so the tuple belongs to neither defining part of the order.

### The Hurwitz norm shell

[PDF p. 2](https://hexagonmath.org/pdf/2611.00370v1#page=2) (§3.1, display (3.2) and the preceding definition of $Q_m$)

#### Example

$1+i+j$ is in $Q_3$.

**Proof**

1. The coordinates $(1,1,1,0)$ are all integers, so the quaternion belongs to $\mathcal H$.
2. The reduced norm is $1+1+1+0=3$, the prescribed shell index.

#### Counter example

$1+i$ lies in $\mathcal H$ and outside $Q_3$.

**Proof**

1. The coordinates $(1,1,0,0)$ are integral, so this quaternion is in the ambient order.
2. Its reduced norm is $1+1=2$, which fails the norm-$3$ condition.

### The finite projective group

[PDF p. 2](https://hexagonmath.org/pdf/2611.00370v1#page=2) (§3.1, last display, $G_p=\mathrm{PGL}_2(\mathbb F_p)$)

#### Example

The projective class of $\operatorname{diag}(3,1)$ is in $G_7$.

**Proof**

1. $7$ is prime and $7\equiv3\pmod4$, so $\mathbb F_7$ is a field at an allowed prime.
2. The matrix has determinant $3\ne0$ in $\mathbb F_7$ and hence represents an invertible class modulo scalar matrices.

#### Counter example

$\operatorname{diag}(1,0)$ does not represent a class in $G_7$.

**Proof**

1. It is a nonzero matrix over $\mathbb F_7$.
2. Its determinant is $0$, and all its nonzero scalar multiples also have determinant $0$. The projective group requires an invertible matrix.

### Projective quaternion reduction

[PDF p. 2](https://hexagonmath.org/pdf/2611.00370v1#page=2) (§3.1, last display, domain and codomain of $\rho_p$)

#### Example

$\rho_7(8+i)=\rho_7(1+i)$.

**Proof**

1. Both quaternions are integral. Their norms are $65$ and $2$, both congruent to $2$ modulo $7$, so both satisfy the domain condition.
2. The order localized at $7$ has $\mathbb Z_7$-basis $1,i,j,k$ because $2$ is a unit and the order contains the four basis elements. Reducing this basis gives the basis of the reduced algebra. Projectivizing identifies reductions precisely up to nonzero scalar.
3. The reductions of $8+i$ and $1+i$ agree coefficient by coefficient because their difference is $7$. Equal reductions have equal projective classes.

#### Counter example

$2+3i+j$ has no value under $\rho_7$.

**Proof**

1. Its four coordinates are integral, so it lies in $\mathcal H$.
2. Its norm is $4+9+1=14$, so the reduction times its conjugate is zero. The conjugate has nonzero scalar coordinate $2$ modulo $7$, so the reduction is singular and fails the norm-coprimality condition for $\rho_7$.

### The projective unit image

[PDF p. 3](https://hexagonmath.org/pdf/2611.00370v1#page=3) (§3.1, first sentence on page 3, definition of $\Gamma_p$)

#### Example

$\rho_7(j)$ lies in $\Gamma_7$.

**Proof**

1. The integral quaternion $j$ has inverse $-j$ in $\mathcal H$, since $j^2=-1$.
2. It has norm $1$ and hence has a projective reduction. As the image of a unit, this reduction belongs to $\Gamma_7$.

#### Counter example

The projective class of $\operatorname{diag}(3,1)$ is in $G_7$ and outside $\Gamma_7$.

**Proof**

1. For a Hurwitz unit $u$, the norms of $u$ and $u^{-1}$ are positive integers with product $1$. Indeed quaternion conjugation reverses products and gives $q\bar q=\operatorname{nrd}(q)$, so the norm multiplies. Integrality follows for strict half-integer coordinates because the four odd squares in the numerator sum to a multiple of $4$. Thus every unit has norm $1$.
2. Over $\mathbb F_7$ take the matrices $I=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ and $J=\begin{pmatrix}2&3\\3&-2\end{pmatrix}$. They satisfy $I^2=J^2=-\mathrm{Id}$ and $IJ=-JI$. The four images $\mathrm{Id},I,J,IJ$ are independent because they are orthogonal for the trace pairing $(X,Y)\mapsto\operatorname{tr}(XY)$ and each has nonzero pairing with itself.
3. For $M=a\,\mathrm{Id}+bI+cJ+dIJ$ one has $\operatorname{tr}(M)=2a$. Its adjugate $2a\,\mathrm{Id}-M$ is its quaternion conjugate, so $\det(M)=a^2+b^2+c^2+d^2$. Thus the unit image $\Gamma_7$ has square determinant, and rescaling a matrix changes its determinant by a square.
4. The determinant of the matrix is $3$. The nonzero squares modulo $7$ are $1,2,4$, so the determinant precludes membership in the unit image.

### The finite left quotient

[PDF p. 3](https://hexagonmath.org/pdf/2611.00370v1#page=3) (§3.1, first sentence on page 3, definition of $Y_p$)

#### Example

$\Gamma_7\rho_7(i)$ and $\Gamma_7$ name the same point of $Y_7$.

**Proof**

1. The unit $i$ has inverse $-i$ in $\mathcal H$, and its norm $1$ is coprime to $7$.
2. Thus $\rho_7(i)\in\Gamma_7$, so left coset multiplication gives $\Gamma_7\rho_7(i)=\Gamma_7$.

#### Counter example

Declaring $\Gamma_7[\operatorname{diag}(3,1)]=\Gamma_7$ in $Y_7$ gives an incorrect coset equality.

**Proof**

1. For a Hurwitz unit $u$, the norms of $u$ and $u^{-1}$ are positive integers with product $1$. Indeed quaternion conjugation reverses products and gives $q\bar q=\operatorname{nrd}(q)$, so the norm multiplies. Integrality follows for strict half-integer coordinates because the four odd squares in the numerator sum to a multiple of $4$. Thus every unit has norm $1$.
2. Over $\mathbb F_7$ take the matrices $I=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ and $J=\begin{pmatrix}2&3\\3&-2\end{pmatrix}$. They satisfy $I^2=J^2=-\mathrm{Id}$ and $IJ=-JI$. The four images $\mathrm{Id},I,J,IJ$ are independent because they are orthogonal for the trace pairing $(X,Y)\mapsto\operatorname{tr}(XY)$ and each has nonzero pairing with itself.
3. For $M=a\,\mathrm{Id}+bI+cJ+dIJ$ one has $\operatorname{tr}(M)=2a$. Its adjugate $2a\,\mathrm{Id}-M$ is its quaternion conjugate, so $\det(M)=a^2+b^2+c^2+d^2$. Thus the unit image $\Gamma_7$ has square determinant, and rescaling a matrix changes its determinant by a square.
4. Write $D$ for the class of $\operatorname{diag}(3,1)$ in $G_7$. The nonzero squares modulo $7$ are $1,2,4$, so $D$ has nonsquare determinant and $\Gamma_7D\ne\Gamma_7$.
5. Equality of the two left cosets would require $D\in\Gamma_7$, which would give $D$ square determinant.

### The counting inner product

[PDF p. 3](https://hexagonmath.org/pdf/2611.00370v1#page=3) (§3.1, sentence after (3.3), counting inner product on $\mathbb C[Y_p]$)

#### Example

If $\delta$ is $1$ at $\Gamma_7$ and $0$ at the other points of $Y_7$, then $\langle\delta,\delta\rangle=1$.

**Proof**

1. The identity coset is a point of $Y_7$, so $\delta$ is a complex-valued function on that finite set.
2. The counting inner product on $\delta$ with itself sums $|\delta(y)|^2$ over $y\in Y_7$. Its only nonzero term is $1$.

#### Counter example

For $\delta$ equal to $1$ at $\Gamma_7$ and $0$ at every other coset, the proposed value $\langle\delta,\delta\rangle=2$ is incorrect.

**Proof**

1. The summand at $\Gamma_7$ is $|1|^2=1$.
2. Every other summand is $|0|^2=0$, leaving the value $1$.

### The quaternionic Hecke operator

[PDF p. 3](https://hexagonmath.org/pdf/2611.00370v1#page=3) (§3.2, equation (3.4))

#### Example

For $p=7$ and $m=3$, the operator satisfies $T_3\mathbf1=4\mathbf1$ on $Y_7$.

**Proof**

1. The index $3$ is positive and odd, $7\in\mathcal P_3$, and $7$ does not divide $3$. The function $\mathbf1$ has value $1$ at every point of $Y_7$.
2. In the integral part of $Q_3$, each coordinate square is $0$ or $1$ and exactly three are $1$. There are $4\cdot2^3=32$ such tuples.
3. In the half-integral part each squared coordinate is at least $1/4$. A coordinate of absolute value $5/2$ or larger already exceeds norm $3$, and a coordinate of absolute value $3/2$ adds $2$ to the baseline total $1$. Exactly one such coordinate is needed, giving $4\cdot2^4=64$ tuples.
4. Every term of (3.4) evaluates to $1$, so each output value is $(32+64)/24=4$.

#### Counter example

For $p=7$ the proposed value $T_1\mathbf1=24\mathbf1$ is incorrect.

**Proof**

1. The positive odd index $1$ is coprime to $7$. At norm $1$, the integral part of $Q_1$ has one coordinate $\pm1$ and three zeros, giving $8$ choices.
2. For strict half-integers the sum of the four squares reaches $1$ precisely when all four absolute values are $1/2$, giving $16$ further choices.
3. The operator averages the $8+16$ terms by the factor $1/24$, so the output at every coset is $1$.

### The determinant character

[PDF p. 3](https://hexagonmath.org/pdf/2611.00370v1#page=3) (§3.2, display defining $\chi_p$ before Lemma 3.2)

#### Example

For $D=[\operatorname{diag}(3,1)]$ in $G_7$, one has $\chi_7(\Gamma_7D)=-1$.

**Proof**

1. The determinant $3$ is nonzero modulo $7$, so $D$ defines a projective matrix class and hence a coset in $Y_7$.
2. The nonzero squares are $1^2,2^2,3^2$, with residues $1,4,2$. Thus the determinant is nonsquare and its Legendre symbol is $-1$.

#### Counter example

The proposed value $\chi_7(\Gamma_7[\operatorname{diag}(2,1)])=-1$ is incorrect.

**Proof**

1. The determinant $2$ is nonzero, so the indicated coset is in the domain.
2. Since $3^2\equiv2\pmod7$, this determinant is a nonzero square. Its Legendre symbol is $+1$.

### The nonsplit torus

[PDF p. 4](https://hexagonmath.org/pdf/2611.00370v1#page=4) (§3.3, opening display, definition of $C_p$)

#### Example

$\rho_7(1+i)$ belongs to $C_7$.

**Proof**

1. Modulo $7$ the polynomial $X^2+1$ has no root since the nonzero squares are $1,2,4$. Thus $\mathbb F_7[i]$ is a field, with norm $N(a+bi)=a^2+b^2$ under $i\mapsto-i$.
2. The element $1+i$ has norm $2$ and is nonzero in the field. Its projective class therefore lies in the image of $\mathbb F_7[i]^\times/\mathbb F_7^\times$.

#### Counter example

$\rho_7(j)$ lies in $G_7$ and outside $C_7$.

**Proof**

1. The order localized at $7$ has $\mathbb Z_7$-basis $1,i,j,k$ because $2$ is a unit and the order contains the four basis elements. Reducing this basis gives the basis of the reduced algebra. Projectivizing identifies reductions precisely up to nonzero scalar.
2. The norm of $j$ is $1$. All nonzero scalar multiples of its reduction have a nonzero $j$ coordinate, whereas every element representing $C_7$ has zero $j$ and $k$ coordinates.

### The nonsplit torus normalizer

[PDF p. 4](https://hexagonmath.org/pdf/2611.00370v1#page=4) (§3.3, opening display, definition of $K_p$)

#### Example

$\rho_7(j+k)$ lies in $K_7$.

**Proof**

1. Modulo $7$ the polynomial $X^2+1$ has no root since the nonzero squares are $1,2,4$. Thus $\mathbb F_7[i]$ is a field, with norm $N(a+bi)=a^2+b^2$ under $i\mapsto-i$.
2. The reduction of $j+k$ equals $(1+i)j$ because $ij=k$. Its norm is $2$ modulo $7$, so it is invertible.
3. The factor $1+i$ lies in the multiplicative group of $\mathbb F_7[i]$, so the projective product belongs to $C_7\rho_7(j)\subset K_7$.

#### Counter example

$\rho_7(1+j)$ lies in $G_7$ and outside $K_7$.

**Proof**

1. The order localized at $7$ has $\mathbb Z_7$-basis $1,i,j,k$ because $2$ is a unit and the order contains the four basis elements. Reducing this basis gives the basis of the reduced algebra. Projectivizing identifies reductions precisely up to nonzero scalar.
2. Write a reduced quaternion as $z+wj$ with $z,w\in\mathbb F_7[i]$. Representatives of $C_7$ have $w=0$ and those of $C_7\rho_7(j)$ have $z=0$. Scalar multiples preserve these two conditions.
3. The quaternion $1+j$ has norm $2$ and has both $z=1$ and $w=1$ nonzero. Neither alternative for belonging to $K_7$ holds.

### The normalizer orbit

[PDF p. 4](https://hexagonmath.org/pdf/2611.00370v1#page=4) (§3.3, display defining $\mathcal O_p$ after the unit-intersection statement)

#### Example

$\Gamma_7\rho_7(1+i)$ belongs to $\mathcal O_7$.

**Proof**

1. Modulo $7$ the polynomial $X^2+1$ has no root since the nonzero squares are $1,2,4$. Thus $\mathbb F_7[i]$ is a field, with norm $N(a+bi)=a^2+b^2$ under $i\mapsto-i$.
2. The norm of $1+i$ is $2$, so it defines the indicated projective class and is a nonzero element of the torus field. Its class belongs to $C_7\subset K_7$, making the coset an orbit point.

#### Counter example

$\Gamma_7\rho_7(1+i+j)$ lies in $Y_7$ and outside $\mathcal O_7$.

**Proof**

1. The order localized at $7$ has $\mathbb Z_7$-basis $1,i,j,k$ because $2$ is a unit and the order contains the four basis elements. Reducing this basis gives the basis of the reduced algebra. Projectivizing identifies reductions precisely up to nonzero scalar.
2. Modulo $7$ the polynomial $X^2+1$ has no root since the nonzero squares are $1,2,4$. Thus $\mathbb F_7[i]$ is a field, with norm $N(a+bi)=a^2+b^2$ under $i\mapsto-i$.
3. Write a reduced quaternion as $z+wj$ with $z,w\in\mathbb F_7[i]$. Representatives of $C_7$ have $w=0$ and those of $C_7\rho_7(j)$ have $z=0$. Scalar multiples preserve these two conditions.
4. Take $q=1+i+j$, with $z=1+i$ and $w=1$. Its norm is $3$, so $\Gamma_7\rho_7(q)$ lies in $Y_7$. If it were in $\mathcal O_7$, some Hurwitz unit $h$ would have $\rho_7(hq)\in K_7$.
5. By multiplicativity and integrality of the quaternion norm, a Hurwitz unit and its inverse have positive integer norms with product $1$. Thus the norm of $h$ is $1$. Its coordinates are either one entry $\pm1$ and three zeros, or four entries $\pm1/2$, since these are the ways to obtain sum of squares $1$ in the two parts of the order.
6. Write $h=u+vj$ with $u,v\in\mathbb F_7[i]$ after reduction. The identity $js=\bar s j$ for $s\in\mathbb F_7[i]$ gives $hq=(uz-v\bar w)+(uw+v\bar z)j$. For a coordinate unit exactly one of $u,v$ is nonzero, so both components of $hq$ are nonzero.
7. For a half-integral unit, $N(u)=N(v)=1/2\ne0$ in $\mathbb F_7$. Vanishing of either component would give $N(z)=N(w)$ by taking norms of the two terms and cancelling $N(u)=N(v)$. Here $N(z)=2$ and $N(w)=1$, so neither component can vanish.

### The normalizer-orbit indicator

[PDF p. 4](https://hexagonmath.org/pdf/2611.00370v1#page=4) (§3.3, display defining $f_p=\mathbf1_{\mathcal O_p}$)

#### Example

$f_7(\Gamma_7)=1$.

**Proof**

1. The identity lies in $C_7\subset K_7$, so its left coset belongs to $\mathcal O_7$.
2. The indicator takes value $1$ at every orbit point.

#### Counter example

The constant-one function on $Y_7$ is an incorrect proposed value of $f_7$.

**Proof**

1. The order localized at $7$ has $\mathbb Z_7$-basis $1,i,j,k$ because $2$ is a unit and the order contains the four basis elements. Reducing this basis gives the basis of the reduced algebra. Projectivizing identifies reductions precisely up to nonzero scalar.
2. Modulo $7$ the polynomial $X^2+1$ has no root since the nonzero squares are $1,2,4$. Thus $\mathbb F_7[i]$ is a field, with norm $N(a+bi)=a^2+b^2$ under $i\mapsto-i$.
3. Write a reduced quaternion as $z+wj$ with $z,w\in\mathbb F_7[i]$. Representatives of $C_7$ have $w=0$ and those of $C_7\rho_7(j)$ have $z=0$. Scalar multiples preserve these two conditions.
4. Take $q=1+i+j$, with $z=1+i$ and $w=1$. Its norm is $3$, so $\Gamma_7\rho_7(q)$ lies in $Y_7$. If it were in $\mathcal O_7$, some Hurwitz unit $h$ would have $\rho_7(hq)\in K_7$.
5. By multiplicativity and integrality of the quaternion norm, a Hurwitz unit and its inverse have positive integer norms with product $1$. Thus the norm of $h$ is $1$. Its coordinates are either one entry $\pm1$ and three zeros, or four entries $\pm1/2$, since these are the ways to obtain sum of squares $1$ in the two parts of the order.
6. Write $h=u+vj$ with $u,v\in\mathbb F_7[i]$ after reduction. The identity $js=\bar s j$ for $s\in\mathbb F_7[i]$ gives $hq=(uz-v\bar w)+(uw+v\bar z)j$. For a coordinate unit exactly one of $u,v$ is nonzero, so both components of $hq$ are nonzero.
7. For a half-integral unit, $N(u)=N(v)=1/2\ne0$ in $\mathbb F_7$. Vanishing of either component would give $N(z)=N(w)$ by taking norms of the two terms and cancelling $N(u)=N(v)$. Here $N(z)=2$ and $N(w)=1$, so neither component can vanish.
8. At $\Gamma_7\rho_7(q)$ both components of each $hq$ are nonzero, ruling out an orbit representative. The indicator takes value $0$ at that coset.

### The normalizer-orbit density

[PDF p. 4](https://hexagonmath.org/pdf/2611.00370v1#page=4) (§3.3, display defining $\mu_p=|\mathcal O_p|/|Y_p|$)

#### Example

$\mu_7=1/7$.

**Proof**

1. The order localized at $7$ has $\mathbb Z_7$-basis $1,i,j,k$ because $2$ is a unit and the order contains the four basis elements. Reducing this basis gives the basis of the reduced algebra. Projectivizing identifies reductions precisely up to nonzero scalar.
2. Modulo $7$ the polynomial $X^2+1$ has no root since the nonzero squares are $1,2,4$. Thus $\mathbb F_7[i]$ is a field, with norm $N(a+bi)=a^2+b^2$ under $i\mapsto-i$.
3. Write a reduced quaternion as $z+wj$ with $z,w\in\mathbb F_7[i]$. Representatives of $C_7$ have $w=0$ and those of $C_7\rho_7(j)$ have $z=0$. Scalar multiples preserve these two conditions.
4. The group $C_7$ has $(49-1)/(7-1)=8$ classes. Its translate by $\rho_7(j)$ is disjoint, by the two coordinate forms, so $K_7$ has $16$ elements. It is closed under products and inverses because $j$ conjugates the field by $i\mapsto-i$ and $j^2=-1$ is scalar.
5. The norm of any unit of $\mathcal H$ is $1$, since the norm is a positive integer and multiplies to $1$ with the norm of its inverse. Conversely a norm-$1$ element has its conjugate in the order as inverse. There are eight coordinate units and sixteen half-integral units with coordinates $\pm1/2$, by the sum-of-squares condition.
6. Two reduced unit representatives that differ by a scalar must differ by $\pm1$ because both have norm $1$. Clearing denominators by $2$ gives coordinates from $-2$ through $2$, which stay distinct modulo $7$ and exclude any further identifications. This gives $|\Gamma_7|=12$. The four projective coordinate units are its intersection with $K_7$, since the half-integral units have both components nonzero.
7. Two elements of $K_7$ give the same left coset precisely when their quotient belongs to $\Gamma_7\cap K_7$. The map $K_7\to\mathcal O_7$ therefore has fibers of size $4$. Hence $|\mathcal O_7|=16/4=4$.
8. An invertible matrix over $\mathbb F_7$ has $49-1$ choices of first column and $49-7$ choices of second column independent of the first. There are $6$ scalar representatives of each projective matrix, yielding $|G_7|=336$ and $|Y_7|=336/12=28$.
9. The defining ratio is $4/28=1/7$.

#### Counter example

$\mu_7=1/84$ is an incorrect proposed value.

**Proof**

1. The order localized at $7$ has $\mathbb Z_7$-basis $1,i,j,k$ because $2$ is a unit and the order contains the four basis elements. Reducing this basis gives the basis of the reduced algebra. Projectivizing identifies reductions precisely up to nonzero scalar.
2. Modulo $7$ the polynomial $X^2+1$ has no root since the nonzero squares are $1,2,4$. Thus $\mathbb F_7[i]$ is a field, with norm $N(a+bi)=a^2+b^2$ under $i\mapsto-i$.
3. Write a reduced quaternion as $z+wj$ with $z,w\in\mathbb F_7[i]$. Representatives of $C_7$ have $w=0$ and those of $C_7\rho_7(j)$ have $z=0$. Scalar multiples preserve these two conditions.
4. The group $C_7$ has $(49-1)/(7-1)=8$ classes. Its translate by $\rho_7(j)$ is disjoint, by the two coordinate forms, so $K_7$ has $16$ elements. It is closed under products and inverses because $j$ conjugates the field by $i\mapsto-i$ and $j^2=-1$ is scalar.
5. The norm of any unit of $\mathcal H$ is $1$, since the norm is a positive integer and multiplies to $1$ with the norm of its inverse. Conversely a norm-$1$ element has its conjugate in the order as inverse. There are eight coordinate units and sixteen half-integral units with coordinates $\pm1/2$, by the sum-of-squares condition.
6. Two reduced unit representatives that differ by a scalar must differ by $\pm1$ because both have norm $1$. Clearing denominators by $2$ gives coordinates from $-2$ through $2$, which stay distinct modulo $7$ and exclude any further identifications. This gives $|\Gamma_7|=12$. The four projective coordinate units are its intersection with $K_7$, since the half-integral units have both components nonzero.
7. Two elements of $K_7$ give the same left coset precisely when their quotient belongs to $\Gamma_7\cap K_7$. The map $K_7\to\mathcal O_7$ therefore has fibers of size $4$. Hence $|\mathcal O_7|=16/4=4$.
8. An invertible matrix over $\mathbb F_7$ has $49-1$ choices of first column and $49-7$ choices of second column independent of the first. There are $6$ scalar representatives of each projective matrix, yielding $|G_7|=336$ and $|Y_7|=336/12=28$.
9. Dividing the orbit size $4$ by $336$ uses the projective group as denominator. The defining ratio uses the $28$ points of the unit quotient and equals $1/7$.

### Uniform quaternionic obstruction estimate

[PDF p. 2](https://hexagonmath.org/pdf/2611.00370v1#page=2) (Proposition 3.1, equation (3.1))

#### Example

For $n=14$ and $p=3$, the ratio $b_3(14)/R(14)=1/3$ attains equality in Proposition 3.1.

**Proof**

1. $14=2\cdot7$ with positive odd part $7$. Both $7$ and $3$ are prime and congruent to $3$ modulo $4$, and $3$ does not divide $7$.
2. The allowed coordinate squares are $0,1,4,9$. Without a $9$, at most two $4$'s give total at most $10$, three $4$'s give at most $13$ unless the fourth is $4$, and four $4$'s give $16$. Exactly one $9$ therefore occurs, and the remaining three squares sum to $5$ only as $4,1,0$.
3. The absolute coordinates are $3,2,1,0$ in some order. This gives $4!\cdot2^3=192$ signed ordered tuples.
4. The obstructed pair must contain the absolute values $3,0$, and the opposite pair then contains $2,1$. Either pair can be the obstructed one. Each has two coordinate orders, and the three nonzero coordinates have independent signs. Both pairs have opposite parity, and the count is $2\cdot2\cdot2\cdot2^3=64$.
5. The ratio is $64/192=1/3$. The prime $3$ makes the indicator $\mathbf1_{p>3}$ zero, and $2/[3(3-1)]=1/3$.

### The mixed-parity lattice count

[PDF p. 4](https://hexagonmath.org/pdf/2611.00370v1#page=4) (§4, opening definition of $N_{\mathrm{mix}}(t)$)

#### Example

$N_{\mathrm{mix}}(5)=12$.

**Proof**

1. The real input $5$ is nonnegative. When both integer coordinates have absolute value at most $2$, the opposite-parity pairs of norm at most $5$ have absolute values $1,0$ or $1,2$, in either order. Larger coordinates have square at least $9$.
2. The absolute values $1,0$ give $2\cdot2=4$ signed ordered pairs. The absolute values $1,2$ give $2\cdot2^2=8$. The sets are disjoint, giving $12$.

#### Counter example

$N_{\mathrm{mix}}(1)=5$ is an incorrect proposed value.

**Proof**

1. The integer pairs of norm at most $1$ are $(0,0)$ and the four signed placements of $1$ with $0$.
2. The zero pair has two even coordinates and fails the opposite-parity requirement. The four other pairs satisfy it, giving count $4$.

### The two-square representation count

[PDF p. 5](https://hexagonmath.org/pdf/2611.00370v1#page=5) (§4, sentence introducing $r_2(u)$ before Lemma 4.2)

#### Example

$r_2(5)=8$.

**Proof**

1. The input is positive. The only two squares summing to $5$ are $1$ and $4$, because the available squares are $0,1,4$.
2. There are two orders of the absolute values $1,2$ and four independent sign choices in each order.

#### Counter example

$r_2(5)=4$ is an incorrect proposed value.

**Proof**

1. Each pair with absolute values $1,2$ in that order has four sign choices.
2. The reversed order has four further signed pairs disjoint from the first four. Both orders count, so the value is $8$.

### The divisor-factor maximum

[PDF p. 5](https://hexagonmath.org/pdf/2611.00370v1#page=5) (§4, first display defining $M(n)$)

#### Example

$M(6)=2$.

**Proof**

1. For integers $1\le u\le6$, the sole possible prime divisor congruent to $1$ modulo $4$ is $5$, occurring only at $u=5$ and to exponent $1$.
2. The factor product is $2$ at $u=5$ and is the empty product $1$ at every other $u$, so the maximum is $2$.

#### Counter example

$M(6)=1$ is an incorrect proposed value.

**Proof**

1. The product at $u=6$ is $1$ since its prime divisors are $2$ and $3$.
2. The definition maximizes over every $u$ from $1$ through $6$. At $u=5$ the factor $1+1=2$ exceeds the proposed value.

### The analytic range

[PDF p. 6](https://hexagonmath.org/pdf/2611.00370v1#page=6) (Proposition 6.1)

#### Example

For $n=2\cdot3^{15}$, the analytic-range conclusion holds with $n=7{,}685+28{,}690{,}129$.

**Proof**

1. The odd part is $3^{15}=14{,}348{,}907$, positive and odd, with sole prime divisor $3\in\mathcal P_3$. Hence $n=28{,}697{,}814>64^4=16{,}777{,}216$.
2. Multiplication gives $5\cdot29\cdot53=7{,}685$ and $13\cdot89\cdot137\cdot181=28{,}690{,}129$. The two positive products sum to $28{,}697{,}814$.
3. The factors $5,13,29,53,89,137,181$ are all $1$ modulo $4$. Trial division by the primes at most the square root of each factor gives no divisor. In increasing trial-prime order the remainder lists for these seven factors are $(1)$, $(1,1)$, $(1,2,4)$, $(1,2,3,4)$, $(1,1,4,5)$, $(1,2,2,4,5)$ and $(1,1,1,6,5,12)$, respectively. Thus both products belong to $\mathcal A$.

### Finite-range input indexing

[PDF p. 8](https://hexagonmath.org/pdf/2611.00370v1#page=8) (Proposition 7.2, proof opening, $n=4k+2$ with $0\le k\le H$)

#### Example

The largest finite input $16{,}777{,}214$ has index $H=4{,}194{,}303$.

**Proof**

1. $4H+2=4(2^{22}-1)+2=2^{24}-2=16{,}777{,}214$.
2. The index is nonnegative and meets the inclusive upper bound. The input is $2$ modulo $4$ and is two less than the exclusive bound $64^4=2^{24}$, making it the last input in that residue class.

#### Counter example

$k=H+1$ does not index a finite-range input.

**Proof**

1. The input formula at this integer gives $4(H+1)+2=2^{24}+2$, still a positive integer congruent to $2$ modulo $4$.
2. It violates the upper bound $n<64^4$ and its proposed index violates $k\le H$.

### The finite-range indicator

[PDF p. 7](https://hexagonmath.org/pdf/2611.00370v1#page=7) (§7, equation (7.1))

#### Example

$\varepsilon_4=1$.

**Proof**

1. The index $4$ lies between $0$ and $H$. The consecutive numerators in the floor difference are $16$ and $17$.
2. A floor can increase from $16/p$ to $17/p$ only if $p$ divides $17$. The sole prime divisor of $17$ is $17\equiv1\pmod4$, so none of the primes in the product causes an increase and each factor is $1$.

#### Counter example

$\varepsilon_2=1$ is an incorrect proposed value.

**Proof**

1. The index $2$ lies in the domain and $3$ is among the primes in the product.
2. The factor for $3$ is $1-\lfloor9/3\rfloor+\lfloor8/3\rfloor=1-3+2=0$. The product therefore equals $0$.

### Eligible first-summand indices

[PDF p. 7](https://hexagonmath.org/pdf/2611.00370v1#page=7) (§7, sentence defining $J$ after Lemma 7.1)

#### Example

$6$ belongs to $J$.

**Proof**

1. The integer $6$ lies in $0\le i\le78$. At $i=6$ the two numerators in (7.1) are $24,25$.
2. For each $p$ the two floors differ only if $p$ divides $25=5^2$. The prime $5$ is absent from the product because it is $1$ modulo $4$, so $\varepsilon_6=1$.

#### Counter example

$2$ lies in the permitted index interval and outside $J$.

**Proof**

1. $0\le2\le78$. The factor at $p=3$ for this index is $1-\lfloor9/3\rfloor+\lfloor8/3\rfloor=0$.
2. Thus $\varepsilon_2=0$, failing the defining indicator condition.

### Possible first summands in the certificate

[PDF p. 7](https://hexagonmath.org/pdf/2611.00370v1#page=7) (§7, display starting $\{4i+1:i\in J\}$)

#### Example

$313$ is a possible first summand in the certificate.

**Proof**

1. It equals $4\cdot78+1$, so its unique index $78$ lies in the prescribed interval.
2. The primes up to $\sqrt{313}$ are $2,3,5,7,11,13,17$. The remainders of $313$ are $1,1,3,5,5,1,7$, respectively, so $313$ is prime and congruent to $1$ modulo $4$.
3. No prime in (7.1) divides $313$, so no floor difference jumps from numerator $312$ to $313$. Thus $\varepsilon_{78}=1$ and the first summand is allowed.

#### Counter example

The admissible integer $325$ is outside the certificate’s set of possible first summands.

**Proof**

1. It is admissible because $325=5^2\cdot13$, with both factors prime and $1$ modulo $4$.
2. The unique index solving $325=4i+1$ is $81$, above the first-summand index bound $78$.

### The finite product-sum count

[PDF p. 7](https://hexagonmath.org/pdf/2611.00370v1#page=7) (§7, equation (7.2))

#### Example

$U(1)=2{,}849{,}643$.

**Proof**

1. The cutoff $a=1$ is permitted. The only product index is $i=0$. Formula (7.1) gives $\varepsilon_0=1$ since $p\ge3$ at every factor. Thus $U(1)=(H+1)-\sum_{k=0}^H\varepsilon_k$.
2. A factor in (7.1) is zero exactly at $p\mid4k+1$. Since $p\equiv3\pmod4$, the integer quotient $(4k+1)/p$ must then be $3$ modulo $4$. Its possible positive values are $3+4r$ for integers $r\ge0$, giving $k=(3p-1)/4+rp$.
3. To evaluate the sum, initialize all $H+1$ entries of an array $E$ to $1$. For $p=3,7,11,\ldots,4095$ in order, skip $p$ if any integer from $2$ to $\lfloor\sqrt p\rfloor$ divides it. Otherwise, starting at $j=(3p-1)/4$, set $E[j]=0$ and increase $j$ by $p$ until $j>H$. The divisibility test leaves exactly the primes required by the product, and the previous step proves $E[k]=\varepsilon_k$ at termination.
4. Summing the array gives $2{,}796{,}203$ after $p=3$, $2{,}396{,}746$ after $p=7$, $1{,}910{,}758$ after $p=31$, and $1{,}344{,}661$ after all candidates through $4095$. Subtraction gives $4{,}194{,}304-1{,}344{,}661=2{,}849{,}643$.

#### Counter example

$U(1)=H+1$ is an incorrect proposed value.

**Proof**

1. At $a=1$ each product has just the factor for $i=0$, with value $1-\varepsilon_0\varepsilon_k$. For $k=0$ this is zero because both floors at $j=0$ are zero for every $p$ and so $\varepsilon_0=1$.
2. All other terms are at most $1$, since each floor difference in the indicator is $0$ or $1$. Hence the whole sum is at most $H$, ruling out $H+1$.

### The finite indicator progression sieve

[PDF p. 7](https://hexagonmath.org/pdf/2611.00370v1#page=7) (§7, displayed deletion progression below (7.3))

#### Example

The full sieve removes $j=2$ and retains $j=1$.

**Proof**

1. Both indices start in the range $0,\ldots,H$. At $p=3$ the progression starts at $(3\cdot3-1)/4=2$, so the rule removes $2$.
2. For $j=1$ a deletion would require $j=(3p-1)/4+rp$ with $r\ge0$. Multiplying by $4$ and adding $1$ would give $5=p(3+4r)$, impossible since every eligible $p$ is at least $3$ and $3+4r\ge3$. Therefore $1$ survives every deletion.

#### Counter example

An output of the full sieve containing $j=5$ would violate the deletion rule.

**Proof**

1. The index $5$ is in the initial range. At the eligible prime $3$, the start is $2$ and the step size $3$, so $5=2+3$ is its second term.
2. The deletion at $p=3$ removes $5$, and later operations only remove indices.

### The finite uncovered-set recurrence

[PDF p. 7](https://hexagonmath.org/pdf/2611.00370v1#page=7) (§7, initialization and update (7.3))

#### Example

The index $k=2$ survives the update for $i=0$ and is removed at $i=1$ in (7.3).

**Proof**

1. Indices $0$ and $1$ are in $0,\ldots,78$. Neither $1$ nor $5$ is divisible by a prime in (7.1), so both indicators are $1$ and these are the first two indices of $J$.
2. The index $2$ starts in $C_0$. At $i=0$ the removal test uses $\varepsilon_2=0$, as its factor at $p=3$ is $1-\lfloor9/3\rfloor+\lfloor8/3\rfloor=0$.
3. At $i=1$ one has $1\le2\le H$ and the test uses $\varepsilon_{2-1}=\varepsilon_1=1$. This update removes $2$.

#### Counter example

A set containing $k=0$ after the first update of (7.3) cannot be the output of that update.

**Proof**

1. The first eligible index is $i=0$ since $\varepsilon_0=1$, and the initialized set contains $0$.
2. For $k=0$ the condition $i\le k\le H$ holds and $\varepsilon_{k-i}=\varepsilon_0=1$, so the first update must remove it.

### The finite range

[PDF p. 8](https://hexagonmath.org/pdf/2611.00370v1#page=8) (Proposition 7.2)

#### Example

At the top finite input $n=16{,}777{,}214$, a decomposition satisfying Proposition 7.2 is $193+16{,}777{,}021$.

**Proof**

1. $n=64^4-2=4\cdot4{,}194{,}303+2$, so $n\equiv2\pmod4$ and $2\le n<64^4$.
2. The sum is $193+16{,}777{,}021=n$, with $16{,}777{,}021=37\cdot173\cdot2621$. The positive factors $193,37,173,2621$ are all $1$ modulo $4$.
3. Trial division by primes through the square root gives remainder lists $(1,1,3,4,6,11)$ for $193$, $(1,1,2)$ for $37$, $(1,2,3,5,8,4)$ for $173$, and $(1,2,1,3,3,8,3,18,22,11,17,31,38,41,36)$ for $2621$, each in increasing trial-prime order. All remainders are nonzero, proving these factors prime.
4. Both summands therefore belong to $\mathcal A$, and the smaller one is $193\le313$.

## Review limits

- Checked the entire original PDF for each direction and used targeted searches for Euler’s problem, weighted bounds, unweighted correlations, the smaller-summand bound and the complementary prime class. Consulted the directly relevant theorem statements and the exact external question. The searches were selective across journal, preprint and author-hosted sources.
- The proved parts are the stated corollaries, finite local factors and congruence constructions. The binary asymptotic and eventual coverage for the complementary class remain unresolved in this assessment. Each direction is a candidate for later independent review.

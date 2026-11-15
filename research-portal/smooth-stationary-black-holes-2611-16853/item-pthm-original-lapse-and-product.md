---
title: "Remark 1.3: lapse bounds and stationary product"
status: published
research_item: pthm-original-lapse-and-product
dependency_level: 6
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 4,5; Remark 1.3 and (1.3)
      statement: Theorem 1.1 assumes Definition 1.1, nonzero restriction of T to S,
        and maximality of the portion of the specified section with |x| >= 1.
        Remark 1.3 writes the maximal lapse equation, zero boundary value and
        unit end limit, obtains 0 < N < 1, and asserts a stationary-flow
        product; equation (1.3) concludes f = N^2 - |X|_h^2 < 1.
      hypotheses: Attribution to the original article and its coordinate convention
        only. The intrinsic and conditional formulation below is a correction of
        the generated draft; this reference is not prerequisite evidence.
      reading_limits: Read frozen PDF pp. 3–5 and visually checked p. 4, including
        Definition 1.1, Theorem 1.1 and Remark 1.3. No original-article defect
        or independent acceptance is asserted. The local argument below uses the
        declared mathematical suppliers and the adopted vacuum model.
---

PDF p. 4: ` Remark 1.3 and (1.3) `; PDF p. 5: ` Remark 1.3 and (1.3) `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-lapse-shift-notation](item-def-lapse-shift-notation)
- [thm-maximal-jacobi-lapse-input](item-thm-maximal-jacobi-lapse-input)
- [lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-40aff34b4a4e-chronological-exterior-connectivity](item-lem-author-40aff34b4a4e-chronological-exterior-connectivity)
- [lem-author-40aff34b4a4e-cauchy-boundary-exclusion](item-lem-author-40aff34b4a4e-cauchy-boundary-exclusion)
- [lem-author-40aff34b4a4e-cauchy-timelike-flow-product](item-lem-author-40aff34b4a4e-cauchy-timelike-flow-product)
- [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)
- [lem-author-40aff34b4a4e-positive-transverse-stationary-product](item-lem-author-40aff34b4a4e-positive-transverse-stationary-product)
- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [math:lem-adjugate-inverse-formula-over-a-field](https://alphabetamath.cc/item/lem-adjugate-inverse-formula-over-a-field)


## Statement

Work in ZFC, including the Axiom of Choice. Assume the regular stationary vacuum data and the stationary vacuum model. Write $j:\Sigma_0\to\{y\in\mathbb R^3:|y|>1/2\}$ for the specified hypersurface identification, $s=|j(\cdot)|$, $S=\{s=1\}$ and $C=\Sigma_0\cap\mathcal E$. Write $r=|x|$ for the physical end radius in the stationary end coordinates $(t,x)$; no agreement between these separately supplied coordinates is assumed.

Then $C$ is exactly the component of $\Sigma_0\setminus S$ containing the stationary $t=0$ end. Its ambient closure $B=C\cup S$ is a connected smooth embedded spherical exterior with compact boundary $S$, diffeomorphic to $\{y\in\mathbb R^3:|y|\ge1\}$ and complete in its intrinsic length metric with the boundary included. In the physical end coordinates, $h_{ij}=\delta_{ij}+O_6(r^{-1})$ and $B\setminus\{t=0,r>R\}$ is compact for every sufficiently large $R$; these truncations exhaust $B$. Thus it has one asymptotically Euclidean end. In the specified $j$ coordinates, $C$ may be either $\{s>1\}$ or $\{1/2<s<1\}$. An adapted topological identification, obtained from $j$ by a radial inversion if necessary, places $C$ on the outer side without asserting agreement with the physical end coordinates. There is an auxiliary complete future timelike-flow diffeomorphism $\mathbb R\times C\to\mathcal E$.

On $\Sigma_0$ use the future unit normal $n$, $h=g|_{T\Sigma_0}$, $k(U,V)=-g(\nabla_Un,V)$, $H=\operatorname{div}_g n=-\operatorname{tr}_h k$ and $T=Nn+X$, with $N=-g(T,n)$ and $X$ tangent. Without a maximality assumption, the lapse on $C$ satisfies $\Delta_hN=|k|_h^2N-X(H)$, $N|_S=0$ and $N\to1$ uniformly on its physical end, where $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$.

If the actual exterior section $C$ is maximal, meaning $H=0$ on $C$, then $\Delta_hN=|k|_h^2N$ and $0<N<1$ on $C$. The stationary-flow map $(a,c)\mapsto\phi_a^T(c)$ is a diffeomorphism $\mathbb R\times C\to\mathcal E$, and $f=-g(T,T)=N^2-|X|_h^2<1$ throughout $\mathcal E$ after stationary extension. The horizon boundary is excluded from both open products. In particular these conditional conclusions hold if the physical end lies on the specified side $\{s>1\}$ and the portion $\{s\ge1\}$ is maximal: then $C=\{s>1\}$. Maximality of that specified side alone does not identify it with $C$.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-lapse-shift-notation](item-def-lapse-shift-notation)

[thm-maximal-jacobi-lapse-input](item-thm-maximal-jacobi-lapse-input)

[lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[lem-author-40aff34b4a4e-chronological-exterior-connectivity](item-lem-author-40aff34b4a4e-chronological-exterior-connectivity)

[lem-author-40aff34b4a4e-cauchy-boundary-exclusion](item-lem-author-40aff34b4a4e-cauchy-boundary-exclusion)

[lem-author-40aff34b4a4e-cauchy-timelike-flow-product](item-lem-author-40aff34b4a4e-cauchy-timelike-flow-product)

[lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)

[lem-author-40aff34b4a4e-positive-transverse-stationary-product](item-lem-author-40aff34b4a4e-positive-transverse-stationary-product)

[def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[math:lem-adjugate-inverse-formula-over-a-field](https://alphabetamath.cc/item/lem-adjugate-inverse-formula-over-a-field)

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice and the inherited countable/dependent-choice hypotheses of the causal and timelike-flow suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The adopted physical assumptions are the vacuum equation, stationarity and future-timelike unit normalization of $T$ sufficiently far out. These are model assumptions rather than observations. [post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[F2] Regularity supplies the smooth spacelike section, Cauchy portion, globally hyperbolic exterior, complete stationary orbits meeting the section, transverse horizon branches and tangency of $T$ to both branches. On the separate stationary end, $T=\partial_t$, the section is $t=0$, and the metric has the stated angularly uniform differentiated decay. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F3] Use the future-normal, induced-metric, second-fundamental-form, lapse, shift and mean-curvature conventions in the Statement; in particular $H=-\operatorname{tr}_h k$, maximality means $H=0$, and $-g(T,T)=N^2-|X|_h^2$. [def-lapse-shift-notation](item-def-lapse-shift-notation) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F4] For a spacelike variation with vector $a n+X$, the pulled-back mean curvature has derivative $\Delta_h a-(|k|_h^2+\operatorname{Ric}(n,n))a+X(H)$. A local Killing flow preserves the pulled-back mean curvature. [thm-maximal-jacobi-lapse-input](item-thm-maximal-jacobi-lapse-input)

[F5] On a connected smooth Riemannian exterior with compact nonempty smooth boundary, a smooth solution of $(\Delta_h-V)u=0$ with $V\ge0$, zero boundary values and uniform end limit $1$ satisfies $0<u<1$ in the interior. The exterior convention requires a physical end chart and a compact core; no weighted norm is used here. [lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control) [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F6] The chronological-exterior lemma gives inclusion of the connected open stationary end in $\mathcal E$, openness and connectedness of $\mathcal E$, and causal convexity. For the supplied Cauchy section, boundary exclusion gives $\partial_{\Sigma_0}C\subset S$. [lem-author-40aff34b4a4e-chronological-exterior-connectivity](item-lem-author-40aff34b4a4e-chronological-exterior-connectivity) [lem-author-40aff34b4a4e-cauchy-boundary-exclusion](item-lem-author-40aff34b4a4e-cauchy-boundary-exclusion)

[F7] A connected globally hyperbolic smooth time-oriented spacetime with a smooth spacelike Cauchy hypersurface has a connected section and a product based on that section given by an auxiliary complete future timelike flow. [lem-author-40aff34b4a4e-cauchy-timelike-flow-product](item-lem-author-40aff34b4a4e-cauchy-timelike-flow-product)

[F8] Under the regular-spacetime data, the actual exterior component has the smooth embedded complete closure $B=C\cup S$, an adapted topological spherical-exterior identification and a single physical asymptotically Euclidean end with compact physical truncations. It requires neither maximality nor matching of the specified hypersurface chart to the end chart. [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)

[F9] On a connected globally hyperbolic spacetime with smooth spacelike Cauchy section $C$, a complete smooth vector field whose every orbit meets $C$ and whose lapse relative to its future normal is positive gives the stationary-flow product map as a global diffeomorphism. No causal-character assumption on the field is needed. [lem-author-40aff34b4a4e-positive-transverse-stationary-product](item-lem-author-40aff34b4a4e-positive-transverse-stationary-product)

[F10] For an invertible real square matrix, its inverse is its adjugate divided by its nonzero determinant. Apply this formula to the $3\times3$ induced metric matrix on the physical end. [math:lem-adjugate-inverse-formula-over-a-field](https://alphabetamath.cc/item/lem-adjugate-inverse-formula-over-a-field)

## Proof

**Given:** The regular stationary vacuum data and ZFC; actual-exterior maximality is assumed only for the conditional conclusions.

**Goal:** Establish the intrinsic exterior and general lapse identity, then the maximal-exterior lapse bounds and stationary product.

1.1 Apply [F6] with the designated stationary end. It is nonempty and connected, its coordinate translations give a global flow, and [F2] supplies the Cauchy and global-hyperbolicity hypotheses. Thus $\mathcal E$ is open and connected, contains that end, and $\partial_{\Sigma_0}C\subset S$. Apply [F7] to this smooth Cauchy portion to obtain connectedness of $C$ and the auxiliary timelike-flow product. [given, A1, F2, F6, F7]

1.2 The local Killing flow transports the induced geometry and future normal of the section isometrically, so its pulled-back mean curvature has zero derivative by [F4]. Apply the full variation formula with $a=N$ and tangential part $X$: $0=\Delta_hN-(|k|_h^2+\operatorname{Ric}(n,n))N+X(H)$. The vacuum equation sets the Ricci term to zero and gives $\Delta_hN=|k|_h^2N-X(H)$ without assuming maximality. [given, F1, F2, F3, F4]

2.1 Apply [F8] to the same regular data, with the same specified section and physical end. It identifies $C$ as the component containing that end and proves all the asserted closure, smoothness, completeness, compact-truncation and differentiated end properties. The adapted topological identification can interchange the specified sides; it does not change $C$ or the physical end chart. No conclusion here selects the specified outer side without an end-side premise. [given, A1, F2, F3, F8, step 1.1]

3.1 At $S$, tangency to both transverse horizons gives $T_p\in T_p\mathcal H^+\cap T_p\mathcal H^-=T_pS\subset T_p\Sigma_0$. Hence $N=-g(T,n)=0$ there. On the physical $t=0$ end, $h_{ij}=g_{ij}\to\delta_{ij}$ uniformly. Its determinant tends to $1$, since it is a polynomial in the entries, so [F10] gives $h^{ij}\to\delta^{ij}$ uniformly. Orthogonality of $n$ to the section gives $g_{0i}=h_{ij}X^j$ and hence $|X|_h^2=h^{ij}g_{0i}g_{0j}$. By [F3], $N^2=-g_{00}+h^{ij}g_{0i}g_{0j}\to1$ uniformly. The future timelike field $T$ has positive lapse on this tail, so $N\to1$. Step 2.1 ensures that this physical tail is the whole infinity needed for an exterior end limit. [given, F1, F2, F3, F10, step 2.1, algebra]

4.1 Now suppose that the actual $C$ is maximal. Then $H=0$ and $X(H)=0$ on $C$, so step 1.2 gives $(\Delta_h-|k|_h^2)N=0$. The metric and lapse are smooth up to $S$, since they restrict smooth data on the spacelike section through $S$. Step 2.1 supplies a connected Riemannian exterior with nonempty compact smooth boundary. In the physical chart choose any sufficiently large $r_0$; both $B\setminus\{r>r_0\}$ and the required core $B\setminus\{r>2r_0\}$ are compact by step 2.1, meeting [F5]'s precise exterior convention. The potential $V=|k|_h^2$ is smooth and nonnegative, and step 3.1 supplies the zero boundary value and uniform unit end limit. Therefore [F5] gives $0<N<1$ on $C$. [given, F3, F5, step 2.1, step 3.1, step 1.2]

5.1 Under this maximality hypothesis, every complete stationary orbit in $\mathcal E$ meets $\Sigma_0$ by [F2], and that intersection belongs to $C$ because the orbit stays in $\mathcal E$. Step 4.1 supplies positive lapse on $C$, so [F9] gives the stationary-flow diffeomorphism $\mathbb R\times C\to\mathcal E$. Its injectivity uses positive crossings of a Cauchy defining coordinate, without assuming stationary trajectories are causal. On $C$, [F3] gives $f=N^2-|X|_h^2\le N^2<1$. The Killing flow preserves $g$ and $T$, hence $f$, and orbit coverage extends this bound throughout $\mathcal E$. Finally, if the physical end is in the specified outer side, the component identification in step 2.1 gives $C=\{s>1\}$; maximality of $\{s\ge1\}$ then implies maximality of this $C$, so all the conditional conclusions apply. Neither product includes $S$. [given, F2, F3, F9, step 1.1, step 2.1, step 4.1] ∎

## Source notes

Remark 1.3 and equation (1.3), PDF pp. 4–5, attribute the original lapse equation, zero boundary value, unit end normalization, strict lapse bound, stationary product and inequality $f<1$. Theorem 1.1 on p. 4 states maximality of the specified portion $|x|\ge1$ and also assumes $T|_S\not\equiv0$. The article uses the same spatial notation for its end and section descriptions. This citation records its claim and scope; it is not a proof of the corrected result above.

The generated regularity definition supplies separate end and hypersurface identifications. Its specified-side maximality does not by itself imply maximality of the actual $C$. The corrected Statement retains the intrinsic exterior, complete physical end and auxiliary product unconditionally, and states the lapse bounds, stationary product and $f<1$ under the explicit actual-exterior maximality hypothesis. The specified-coordinate conclusion is retained with its end-side premise. This corrects the generated formulation; it establishes no defect in the original article or its intended coordinate convention. The ADM causal-completeness supplier presupposes a product and is not used to construct either product here.

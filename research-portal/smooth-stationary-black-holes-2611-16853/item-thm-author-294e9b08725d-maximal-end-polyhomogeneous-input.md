---
title: Independent stationary maximal-gauge asymptotic expansion and KID input
status: published
research_item: thm-author-294e9b08725d-maximal-end-polyhomogeneous-input
dependency_level: 5
sources:
  references:
    - title: P.T. Chruściel and J.L. Costa, On uniqueness of stationary vacuum black
        holes
      url: https://arxiv.org/pdf/0806.0016
      locator: §2.1, PDF pp.5–6, especially (2.1)–(2.8) and footnote 3 on p.6
      statement: Under the classical finite-order AF initial-data conditions (2.1),
        timelike stationary vacuum ends admit adapted stationary coordinates
        with all-order bounds (2.7), quotient-harmonic spatial coordinates and
        full inverse-power/log expansions with exponent n-2, as described after
        (2.7) and in footnote3. We import only the resulting orbit metric q and
        Killing norm V expansions, which are invariant under stationary changes
        of time origin. No fixed-slice connection expansion is imported.
      hypotheses: Vacuum stationary end, initial induced metric and second form
        obeying (2.1) with k>=2 and positive decay exponent; timelike Killing
        field with supplied asymptotic unit time-translation normalization.
        Dimension three here. The intended CW end has these classical bounds as
        well as the separately recorded weak weighted conditions.
      reading_limits: Consulted the frozen full-PDF extraction at section 2.1,
        equations (2.1)-(2.8), and inspected the rendered PDF page 6 including
        footnote 3; checked the public PDF identity. Import only the
        adapted-gauge existence and orbit-field expansion assertion. Its cited
        PDE proof is not reconstructed. The fixed-time connection is treated
        locally below; adapted time is not identified with the supplied time.
    - title: D. Kennefick and N. Ó Murchadha, Weakly decaying asymptotically flat
        static and stationary solutions to the Einstein equations
      url: https://arxiv.org/pdf/gr-qc/9311012
      locator: §II, PDF p.6, (2.22)–(2.28); §III, p.7, Definitions 1–2; §IV, pp.10–12,
        (4.1)–(4.23)
      statement: For smooth maximal stationary vacuum data satisfying (4.9)-(4.11),
        the estimates (4.12) and (4.14) give N-1 in H_(3,delta) and the shift in
        H_(3,3delta/2). Section III defines the weights and states the
        multiplication theorem. Equations (2.22)-(2.28) and (4.1)-(4.8) give the
        maximal stationary constraints, lapse equation, Killing equation and
        Ricci equation; taking the divergence of the Killing equation gives the
        vector KID identity used here.
      hypotheses: Smooth stationary vacuum data in three spatial dimensions, maximal
        slice, h-delta in H_(3,delta), P in H_(2,delta/2-1), delta<0, N tending
        to 1 and shift tending to zero. Retain the explicit (4.11) assumption
        rather than deriving it from scalar curvature. For the initial estimates
        we first relax the given weight to delta in (-1/4,0); P=-k in our
        convention. The final four-dimensional Sobolev theorem and the quotient
        analyticity conclusion are not used.
      reading_limits: Read the frozen full-PDF extraction of section II (2.22)-(2.28),
        section III Definitions 1-2 and the multiplication theorem, and section
        IV (4.1)-(4.23); checked the public PDF identity. The weighted elliptic
        estimates (4.12),(4.14) are explicit imported inputs; their cited proofs
        are not reconstructed. Neither the final four-dimensional theorem nor a
        same-slice expansion theorem is imported.
    - title: P.T. Chruściel, Asymptotic estimates in weighted Hölder spaces for a
        class of elliptic scale-covariant second order operators
      url: https://afst.centre-mersenne.org/article/AFST_1990_5_11_1_21_0.pdf
      locator: §2 Theorem2.1, printed pp.27–29, (2.14)–(2.24), and the scaling
        estimates (2.12)–(2.13)
      statement: "Theorem 2.1 applies to L=a*d_r^2+b*r^-1*d_r+r^-2*(c+Delta_S): if
        Lf=rho, f=O(r^beta), rho=O(r^(alpha-2)*(1+log r)^q), alpha<beta, it
        decomposes f into finitely many characteristic harmonic terms, resonant
        logarithmic terms and a remainder O(r^alpha*(1+log r)^q); the resonant
        bound may gain one log power. Formula (2.24) supplies the corresponding
        weighted C^(k+2,lambda) remainder estimates when rho has weighted
        C^(k,lambda) bounds. For the Euclidean Laplacian on R3, a=1,b=2,c=0 and
        the roots are l and -l-1."
      hypotheses: Compact smooth boundaryless angular manifold S, a>0, real b,c, and
        distinct characteristic roots; alpha<beta. Here S=S2, beta is chosen
        negative and noncharacteristic. At every resonant alpha choose a source
        log weight q at least two and large enough to dominate the actual
        source; this satisfies the logarithmic restrictions in Theorem 2.1. The
        actual solution is smooth, has the stated initial decay, and its source
        has all the weighted Holder bounds used in (2.24). Rescaling the inner
        radius to 1 does not change these conditions.
      reading_limits: Read the frozen extracted section 2 and inspected the rendered
        PDF pages 8-10 (printed 27-29), including (2.12)-(2.24); checked the
        public PDF identity. Import the scalar estimate only, without
        reconstructing its proof. The nonlinear connection recursion and its
        source bounds are local arguments below; this paper is not claimed to
        state a fixed-maximal-slice theorem.
    - title: R. Beig and P.T. Chruściel, The asymptotics of stationary electro-vacuum
        metrics in odd space-time dimensions
      url: https://arxiv.org/pdf/gr-qc/0612012
      locator: §4 equations(4.1)–(4.3), PDF pp.6–7; §2 footnote2 on PDF p.2
      statement: For g=-V^2(dt+theta)^2+q, the stationary vacuum reduction has
        lambda=-V^2 dtheta and div_q(V lambda)=0, hence div_q(V^3 dtheta)=0.
        This local reduction is dimension-independent; the dimension
        restrictions of the paper concern its conformal analyticity conclusion,
        which is not imported.
      hypotheses: Timelike stationary vacuum metric with V>0 and positive orbit metric
        q; theta is the connection in the displayed stationary decomposition. We
        use only the local curl equation, which is tensorial in every spatial
        dimension. The maximal slicing equation is derived separately from the
        actual determinant and unit normal.
      reading_limits: Read the frozen extracted section 4 through (4.3) and the
        adjacent gauge discussion; checked the public PDF identity. Use only the
        local tensorial vacuum curl identity, which has no dimension-dependent
        coefficient. Do not apply the paper's high-dimensional conformal
        analyticity result in dimension three. The maximal-slice equation is
        derived directly below rather than taken from display (4.7).
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [lem-author-294e9b08725d-maximal-end-cw-weak-kid-data](item-lem-author-294e9b08725d-maximal-end-cw-weak-kid-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations)
- [math:thm-higher-order-sobolev-embedding](https://alphabetamath.cc/item/thm-higher-order-sobolev-embedding)
- [math:lem-pe18-spherical-harmonic-structure-and-density](https://alphabetamath.cc/item/lem-pe18-spherical-harmonic-structure-and-density)
- [` P.T. Chruściel and J.L. Costa, On uniqueness of stationary vacuum black holes · §2.1, PDF pp.5–6, especially (2.1)–(2.8) and footnote 3 on p.6 `](https://arxiv.org/pdf/0806.0016)
- [` D. Kennefick and N. Ó Murchadha, Weakly decaying asymptotically flat static and stationary solutions to the Einstein equations · §II, PDF p.6, (2.22)–(2.28); §III, p.7, Definitions 1–2; §IV, pp.10–12, (4.1)–(4.23) `](https://arxiv.org/pdf/gr-qc/9311012)
- [` P.T. Chruściel, Asymptotic estimates in weighted Hölder spaces for a class of elliptic scale-covariant second order operators · §2 Theorem2.1, printed pp.27–29, (2.14)–(2.24), and the scaling estimates (2.12)–(2.13) `](https://afst.centre-mersenne.org/article/AFST_1990_5_11_1_21_0.pdf)
- [` R. Beig and P.T. Chruściel, The asymptotics of stationary electro-vacuum metrics in odd space-time dimensions · §4 equations(4.1)–(4.3), PDF pp.6–7; §2 footnote2 on PDF p.2 `](https://arxiv.org/pdf/gr-qc/0612012)


## Statement

Work in ZFC. Let a smooth stationary vacuum Lorentzian four-dimensional end have a future timelike Killing field near infinity and an asymptotically horizontal maximal stationary slicing, with $T=\partial_\tau$, $N\to1$ and $X\to0$. Write $h$, $k$, $N$ and $X$ for its induced metric, second form, lapse and shift, with $k=(2N)^{-1}\mathcal L_Xh$.

Fix an exterior chart $E=\{x\in\mathbb R^3:|x|>R_0\}$, $R_0>1$, and put $r=|x|$ and $\rho=(1+r^2)^{1/2}$. For a finite array of coordinate components u define $H^s_\eta(E)$ by weak derivatives through the nonnegative integer order s and the finite norm
$$\|u\|_{H^s_\eta(E)}^2=\sum_{\text{components }a}\sum_{|\beta|\le s}\int_E\rho^{-2\eta-3+2|\beta|}|\partial^\beta u_a|^2\,d^3x.$$
All tensor membership statements use these coordinate components and Euclidean measure. Using r instead of $\rho$ gives the same finiteness condition. The weak maximal initial-data assumptions are $h-\delta\in H^3_\eta(E)$ and $k\in H^2_{\eta/2-1}(E)$ for some $\eta<0$.

For the expansion conclusion, require in addition the classical asymptotic-flatness interface $h-\delta=O_3(r^{-a})$ and $k=O_2(r^{-1-a})$ in this chart for some $0<a<1$. Every supplied CW end described by the existing weak-KID-data lemma meets this additional interface with $a=1/2$, on that same maximal hypersurface. Thus the expansion conclusion below applies to the intended CW end without changing its time coordinate or replacing its hypersurface. The weak weighted assumptions alone are not being asserted to imply this classical interface.

Here the quotient metric is the positive metric on stationary orbits, represented on the slice by $q=h+f^{-1}X^\flat\otimes X^\flat$, where $f=-g(T,T)=N^2-|X|_h^2>0$ and $X^\flat=h(X,\cdot)$. Equivalently $g=-f(d\tau+\theta)^2+q$ with $\theta=-f^{-1}X^\flat$. Quotient-harmonic coordinates y satisfy $\Delta_q y^i=0$, where $\Delta_qv=(\det q)^{-1/2}\partial_j((\det q)^{1/2}q^{j\ell}\partial_\ell v)$. They are spatial coordinates, constant along T. In a fixed exterior chart, $O_\infty(r^{-b})$ means $O_m(r^{-b})$ for every finite nonnegative integer m, allowing the constants and threshold radius to depend on m.

In asymptotically Cartesian quotient-harmonic spatial coordinates, retaining the already imposed maximal time gauge, $h-\delta$, $N-1$ and X are $O_\infty(r^{-1})$ and have full differentiated polyhomogeneous expansions. Precisely, for each component v of these corrections there are smooth functions $v_{j\ell}$ on $S^2$ and finite nonnegative integers $L_j$ such that
$$v\sim\sum_{j\ge1}\sum_{\ell=0}^{L_j}r^{-j}(\log r)^\ell v_{j\ell}(\omega),\qquad r=|y|,\quad\omega=y/|y|.$$
For every positive integer p and multi-index $\beta$, the difference from the sum through $j=p$ obeys $|\partial^\beta R_p|\le C_{p\beta}r^{-p-1-|\beta|}(1+\log r)^{J_{p\beta}}$ sufficiently far out, with finite constants and nonnegative integer $J_{p\beta}$. No convergence is asserted. The separate $O_\infty(r^{-1})$ bound excludes positive log powers at the first inverse-power order.

Under the weak maximal hypotheses, independently of the additional classical bounds, the maximal vacuum KID identities are $\operatorname{div}_hX=0$, $\operatorname{div}_h k=0$, $\Delta_hN=N|k|_h^2$ and $\Delta_hX_j+\operatorname{Ric}(h)_{j\ell}X^\ell=2k_{j\ell}D^\ell N$. Here D is the Levi–Civita derivative of h, divergence is its contraction, and the covector Laplacian is $D^iD_i$. The stationary Ricci equation expresses $\operatorname{Ric}(h)-N^{-1}D^2N$ as terms of orders $k^2$, $N^{-1}X Dk$ and $N^{-1}kDX$, with the fixed convention. The orbit-field expansions, scalar Poisson estimates and KID equations are imported; the fixed-slice connection argument and the application to the supplied CW end are proved below.

## Statement references

[lem-author-294e9b08725d-maximal-end-cw-weak-kid-data](item-lem-author-294e9b08725d-maximal-end-cw-weak-kid-data)

## Facts & Assumptions

[F1] Source0 supplies expansions only of the orbit metric q and Killing norm V in quotient-harmonic spatial coordinates, from the classical AF interface. These fields are invariant under a stationary change of time origin. 

[F2] Source1 supplies the weak weighted lapse/shift estimates (4.12),(4.14), the maximal KID identities and their stated sign translation P=-k. 

[F3] The actual CW end has the displayed classical differentiated graph and weak weighted data on the supplied maximal slice, without improved height being assumed. [lem-author-294e9b08725d-maximal-end-cw-weak-kid-data](item-lem-author-294e9b08725d-maximal-end-cw-weak-kid-data)

[F4] The smooth stationary and maximal ADM conventions, componentwise weighted derivatives and Choice are fixed by the declared suppliers. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F5] Source2 is the scalar Euclidean-Poisson power/log decomposition with differentiated remainders. Its decaying characteristic modes have positive integer decay exponents in three dimensions. 

[F6] Source3 supplies only the vacuum connection curl equation $\operatorname{div}_q(V^3 d\theta)=0$, not a fixed-slice expansion or the printed maximal gauge. 

[F7] Local scalar Schauder estimates apply to smooth solutions on Euclidean balls; rescaled interior balls cover each smaller annulus. The three-dimensional H3 Sobolev embedding gives C1,alpha bounds on smaller balls for any alpha below one half, using an interior cutoff. Small principal couplings will be absorbed component by component. [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations) [math:thm-higher-order-sobolev-embedding](https://alphabetamath.cc/item/thm-higher-order-sobolev-embedding)

[F8] On the unit two-sphere, the degree-l harmonics have Laplacian eigenvalue -l(l+1), smooth functions have rapidly decreasing projections, and each fixed derivative norm of a degree-l mode has a polynomial bound in l. [math:lem-pe18-spherical-harmonic-structure-and-density](https://alphabetamath.cc/item/lem-pe18-spherical-harmonic-structure-and-density)

## External input

The imported expansion in source0 is restricted to the stationary orbit fields q and V. The fixed-time connection expansion is the local argument below. Source1 supplies the weak weighted lapse/shift bounds and KID equations. Source2 supplies only the scalar Poisson decomposition and differentiated remainder estimates. Source3 supplies only the stationary vacuum curl identity; its printed maximal-gauge formula is not copied.

## Proof

**Given:** The exact hypotheses in the Statement.

**Goal:** Prove the fixed-slice expansion and the separately scoped weak KID identities.

1.1 The equivalence of r and rho in the weighted norms follows from their bounded ratio on the end. For the supplied CW end, its stated differentiated estimates imply $h-\delta=O_3(r^{-1/2})$ and $k=O_2(r^{-3/2})$, since every fixed power of log is dominated by a positive power of r. This verifies the classical source interface without changing the slice. The separate weak weighted memberships are already supplied. [F3, F4]

2.1 Apply [F1] to obtain quotient-harmonic spatial coordinates y and expansions of the actual orbit metric q and $V=\sqrt{-g(T,T)}$. These are fields on the stationary orbit space and are unchanged when an adapted time is replaced by the already supplied tau. Retain tau throughout. Write the actual metric as $g=-V^2(d\tau+\theta)^2+q$. The connection theta in this expression has not yet been given an expansion; this is the remaining claim to be proved, rather than a consequence of gauge invariance. [F1, F4, step 1.1]

3.1 First choose $\eta<\eta_0<0$ with $-1/4<\eta_0<0$. Membership at the given weight implies membership at this weaker weight, for both h and k, by pointwise comparison of their weights. In the original spatial chart, [F2] then gives $N-1\in H^3_{\eta_0}$ and $X\in H^3_{3\eta_0/2}$. On rescaled balls inside annuli, [F7] gives C1,alpha bounds for every alpha below one half. Products of H3 functions are H3: in each differentiated product through order three, one factor has derivative order at most one and is bounded, and the other is square integrable. The same chain rule through order three applies to inversion and positive square root near the limiting coefficients. Thus $q-\delta$, $V-1$ and theta have negative-weight H3 bounds. For the CW end this also follows directly from its explicit C3 bounds. These initial bounds persist under the asymptotically Cartesian orbit-coordinate change: if F is the coordinate transition, the metric identity $q_x=(DF)^Tq_yDF$ bounds DF and its inverse. The connection transformation identity $D^2F=\Gamma(q_x)DF-\Gamma(q_y)(DF,DF)$, differentiated twice, bounds DF in rescaled H3 from the rescaled H3 metric bounds: the first identity bounds D2F using the C1 bounds of the metrics, its first derivative bounds D3F in L2, and its second derivative bounds D4F in L2, with the products controlled as above. The limiting Euclidean metrics give uniform bounds for DF and its inverse, while the first, second and third rescaled derivatives of DF have negative-power decay in L2, the first also in supremum norm. Radii in the two charts are comparable by the uniformly Euclidean orbit distances. Pullback and the chain rule therefore preserve some negative-weight H3 bound for theta. Consequently its rescaled C1,alpha norm on each fixed annulus is $O(R^{-\epsilon})$ for some $\epsilon>0$. For the CW C3 bounds the same calculation is classical and may take any initial exponent below one. [F1, F2, F3, F4, F7, step 2.1]

3.2 Put $s=(1-V^2|\theta|_q^2)^{1/2}$. Spacelikeness gives s positive. The inverse of the actual metric has $g^{\tau\tau}=-s^2/V^2$ and $g^{i\tau}=-\theta^i$, while its determinant is $-V^2\det q$. Its future unit normal to the SAME tau levels has components $n^\tau=s/V$, $n^i=V\theta^i/s$. The identity $\Gamma^a{}_{ab}=\partial_b\log\sqrt{|\det g|}$ follows by contracting the metric connection formula and differentiating the determinant; hence $\operatorname{div}_g n=|\det g|^{-1/2}\partial_a(|\det g|^{1/2}n^a)$. Stationarity and maximality, namely $\operatorname{div}_g n=0$, thus give the exact fixed-slice equation $\operatorname{div}_q(V^2\theta^\sharp/s)=0$. This is an equation already satisfied by the supplied slice, not an equation solved to choose a replacement time. [F4, step 2.1]

4.1 Expanding this divergence covariantly gives $\operatorname{div}_q\theta=-2V^{-1}\theta\cdot DV-s^{-2}V|\theta|_q^2\theta\cdot DV-s^{-2}V^2\theta^i\theta^jD_i\theta_j$. Combine its derivative with the curl equation in [F6]. In q-harmonic coordinates, the resulting component system has Euclidean Laplacian principal part plus coefficients $O(q-\delta)+O(\theta^2)$ multiplying second derivatives of theta. Its remaining terms are sums of analytic coefficient functions near $(q,V,\theta)=(\delta,1,0)$ times: $(Dq,DV)D\theta$, $\theta(D^2q,D^2V,(Dq)^2,DqDV,(DV)^2)$, and $\theta(D\theta)^2$, including additional factors vanishing at that limit. This follows by expanding the covariant curl/divergence identities and commuting two first derivatives; the connection terms use at most two derivatives of q. All terms vanish when theta is zero. The principal perturbation is small far out; its off-diagonal component couplings have size O(theta squared), and the common scalar principal metric is uniformly elliptic. This is the system to which the annular estimates will be applied. [F4, F6, F7, step 3.2]

5.1 Starting from the rescaled C1,alpha estimate in step 3.1, the coefficients of the small second-order perturbation have small C0,alpha norm; the remaining quadratic first-derivative terms have the same or better rescaled decay. Apply the scalar estimate to each component and sum the norms. Localize to an annulus using a cutoff supported in a slightly larger annulus; the cutoff error involves only theta and its first derivatives, whose norms are already controlled. The norm of the term consisting of the small principal perturbation times D2theta is at most its small C0,alpha coefficient norm times the localized C2,alpha norm, so it can be moved to the left. A finite cover by fixed-size balls in the rescaled annulus gives a uniform rescaled C2,alpha estimate. Differentiate, use nested annuli, and induct: coefficients q and V have bounds at every derivative order by [F1], and the new top derivatives of theta retain the same small principal matrix. Thus $\theta=O_\infty(r^{-\epsilon})$. Bounds on one further derivative give each required rescaled Holder seminorm by the mean-value estimate on the fixed balls. Thus the sources below satisfy the weighted Holder hypotheses of (2.24), in addition to the displayed differentiated bounds. This bootstrap needs only the finite initial data and the invariant-field source expansion, and never changes tau. [F1, F7, step 3.1, step 4.1]

6.1 If theta has differentiated decay exponent e positive, step 4.1 and $q-\delta,V-1=O_\infty(r^{-1})$ show that its Euclidean Laplacian is $O_\infty(r^{-2-d})$ with $d=\min(1+e,3e)$. Apply [F5] separately to its components. The permitted harmonic decays are $r^{-j}$, j positive integers; positive or constant harmonic modes are excluded by the initial decay. At each iteration choose a new exponent strictly between e and min(d,1), avoiding integers; for example, while e is below one half, take 3e/2, unless this exceeds three quarters, in which case take three quarters. Once e exceeds one third, d is greater than one, so no further subcritical iteration is needed. Apply Theorem 2.1 with a negative noncharacteristic upper growth exponent beta slightly larger than -e and a source exponent alpha=-d strictly below -1, weakening d slightly to avoid a characteristic root if necessary. The only harmonic mode at order r to the power minus one is degree zero; positive and constant modes are excluded by the negative growth bound. Thus theta equals a constant vector divided by r plus a remainder decaying strictly faster. The estimates for the remainder hold with every differentiated order by (2.24), since the source has those bounds from step 5.1. In particular $\theta=O_\infty(r^{-1})$. Applying [F5] once more with source $O_\infty(r^{-4})$ and source log weight two gives $\theta=A/r+O_\infty(r^{-2}(1+\log r)^J)$ for some finite J at each derivative order. No positive log power occurs at order one because the source decays strictly faster than $r^{-3}$. [F1, F5, F8, step 4.1, step 5.1]

7.1 We give the full recursion, not just a formal series. Suppose a finite sum through order p has been chosen with conormal remainder $O(r^{-p-1}(1+\log r)^J)$. Expand the analytic coefficient functions in step 4.1 to finite order, using the already imported q,V expansions. Replacing theta by its finite sum changes that system's right-hand side by $O(r^{-p-4}(1+\log r)^{J'})$: the coefficient of its linear second-derivative term is $O(r^{-1})$, and every other linear term has the corresponding extra derivative decay; the nonlinear principal term has two extra theta factors. In the residual obtained by subtracting the Laplacian of the finite theta sum from that right-hand side, all earlier orders cancel: otherwise the actual remainder could not satisfy its differentiated induction bound. Thus the residual source at order $r^{-p-3}$ is determined by the known finite sums, with smooth angular coefficients and finitely many log powers. [F1, F5, step 4.1, step 6.1]

8.1 For j positive, $\Delta[r^{-j}P(\log r,\omega)]=r^{-j-2}((\Delta_{S^2}+j(j-1))P+(1-2j)\partial_zP+\partial_z^2P)$, where z is log r. By [F8], on the orthogonal complement of degree j-1 the angular operator has nonzero eigenvalues $j(j-1)-l(l+1)$. Division by them preserves rapid decay of the smooth source projections, and the polynomial derivative bounds in [F8] give convergence in every Ck norm. Thus its inverse preserves smooth angular coefficients; solve the finitely many polynomial coefficients in descending log degree on this complement. On its kernel, $1-2j$ is nonzero, so a polynomial antiderivative solves the remaining polynomial equation, increasing the log degree by at most one; its constant part is a free decaying harmonic. This constructs the next finite term. Here the next term has $j=p+1$. Subtract it and apply [F5] with upper growth exponent $\beta=-p-1+\delta$, $0<\delta<1$, and source exponent $\alpha=-p-2$, using a log weight at least two and large enough to dominate the residual source. The previously obtained remainder bound implies this upper growth bound; it excludes all slower harmonic modes. Include the possible degree-p harmonic term at order $r^{-p-1}$ in the next coefficient. Formula (2.24) then applies on the actual remainder equation to obtain $O(r^{-p-2}(1+\log r)^{J''})$ with all differentiated estimates, with smooth angular coefficients, including that free harmonic in the finite coefficient. This proves the induction. Terms of different inverse order or log degree are asymptotically independent, so the coefficients can be chosen compatibly at every order. The result is a full differentiated integer-power/log expansion for the actual theta. [F5, F8, step 7.1]

9.1 The ADM fields of the supplied tau foliation satisfy $h=q-V^2\theta\otimes\theta$, $X_i=-V^2\theta_i$ and $N=V/s$. Matrix inversion and the positive square root are analytic near the limiting coefficients, and finite Taylor expansion with the differentiated product rule preserves every finite power/log expansion and its conormal remainder. Therefore h,N,X have exactly the expansions and $O_\infty(r^{-1})$ bounds stated, on that SAME maximal slice and in the orbit-harmonic spatial coordinates. No assertion of series convergence or analyticity at compactified infinity is used. [F1, F4, step 6.1, step 8.1]

10.1 Independently of the expansion conclusion, source1 gives the maximal KID equations under the weak weighted assumptions. The convention $\mathcal L_Xh=2Nk$ identifies its P as -k. Taking its maximal trace, momentum constraint, lapse equation and divergence of the stationary Killing equation gives the four stated identities, and its stationary Ricci equation gives the recorded quadratic/transport orders. These arguments do not use the additional classical interface. Together with step 9.1 this proves both respective scopes of the Statement. [F2, F4, step 9.1] ∎

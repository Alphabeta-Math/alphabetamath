---
title: Mass-one end coordinates on the unchanged maximal section
status: published
research_item: lem-author-29145f41e94d-mass-one-original-section
dependency_level: 3
sources:
  references:
    - title: R. Beig and B. Schmidt, Time-Independent Gravitational Fields
      url: https://arxiv.org/pdf/gr-qc/0005047v1
      locator: §2.1 (2.33)–(2.34), printed p.7; §2.3 (2.72), p.11; §3.1 (3.5),
        (3.15)–(3.17), (3.22)–(3.25), pp.17–20
      statement: The stationary decomposition is g=V(dt+a)^2+h_quot and
        h-bar=(-V)h_quot. Twice-differentiated weak quotient falloff admits
        spatial multipole gauges, with h-bar=delta+O_infinity(r^-2) and
        V=-1+2M/r+O_infinity(r^-2).
      hypotheses: Timelike stationary Ricci-flat spherical quotient tail; V+1,
        normalized twist and h-bar-delta are O_2(r^-alpha), 1/2<alpha<1.
      reading_limits: Consulted these displayed passages in the online PDF. Import the
        multipole result; no reconstruction or reading of its 1981 primary
        reference is claimed. Its leading spatial gauge is not silently
        identified with the analytic normal-coordinate gauge below.
    - title: S. Dain, Initial data for stationary space-times near space-like infinity
      url: https://arxiv.org/pdf/gr-qc/0107018v1
      locator: §2, (17)–(19), Theorem 2.1 and following normal-coordinate paragraph,
        printed p.4; Lemma 2.4 and (21)–(22), pp.5–6
      statement: The conformal quotient metric gamma is analytic in normal coordinates
        xi at infinity; the potential-defined conformal factor has Omega=|xi|^2
        f_Omega, with f_Omega analytic, positive and f_Omega(0)=1.
      hypotheses: Stationary vacuum timelike quotient with the potential-defined
        factor (17), C^{2,alpha} factor, C^{4,alpha} conformal metric and
        normalization (18)–(19).
      reading_limits: Consulted exactly these hypotheses, theorem, normal-coordinate
        paragraph and lemma in the online PDF. Applicability and the identity of
        the selected chart are supplied by the normalized-end Statement. No
        proof reconstruction or maximality of Dain’s time section is claimed.
---

## Prerequisites

- [lem-author-29145f41e94d-homothetic-stationary-geometry](item-lem-author-29145f41e94d-homothetic-stationary-geometry)
- [lem-author-d20d145f998f-normalized-stationary-end](item-lem-author-d20d145f998f-normalized-stationary-end)
- [lem-author-d20d145f998f-cutoff-end-coordinate-extension](item-lem-author-d20d145f998f-cutoff-end-coordinate-extension)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:prop-properties-of-normal-coordinates-at-the-center](https://alphabetamath.cc/item/prop-properties-of-normal-coordinates-at-the-center)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)
- [` R. Beig and B. Schmidt, Time-Independent Gravitational Fields · §2.1 (2.33)–(2.34), printed p.7; §2.3 (2.72), p.11; §3.1 (3.5), (3.15)–(3.17), (3.22)–(3.25), pp.17–20 `](https://arxiv.org/pdf/gr-qc/0005047v1)
- [` S. Dain, Initial data for stationary space-times near space-like infinity · §2, (17)–(19), Theorem 2.1 and following normal-coordinate paragraph, printed p.4; Lemma 2.4 and (21)–(22), pp.5–6 `](https://arxiv.org/pdf/gr-qc/0107018v1)


## Statement

Work in ZFC. Suppose a smooth stationary Ricci-flat exterior has a supplied stationary Cauchy product $E\cong\mathbb R\times C$, with complete stationary field $T=\partial_t$, spacelike Cauchy section $C$, and positive lapse $-g(T,n)>0$. Supply a smooth section extension $\Sigma_0$ and a global spatial chart $x:\Sigma_0\to\{r>1/2\}$, $r=|x|$, agreeing with the original end chart, with $C=\{r>1\}$ and the specified bifurcation sphere $S=\{r=1\}$. Suppose $C$ is maximal and is $t=0$ in the original end, where $g_{00}=-1+2m/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$, and $m>0$. Here $O_k(r^{-b})$ means componentwise Cartesian derivatives of order $j\le k$ are bounded by constants times $r^{-b-j}$, uniformly in angle.

Its ADM mass is $m$ in the auxiliary asymptotically Cartesian spatial gauge $y$ supplied by stationary end normalization, which extends to the unchanged section while fixing $S$. For $\widehat g=m^{-2}g$, $\widehat T=mT$, $\widehat t=t/m$, $\widehat x=y/m$ and $\widehat r=|\widehat x|$, this same section is maximal, has ADM mass one, and satisfies $\widehat g_{00}=-1+2/\widehat r+O_6(\widehat r^{-2})$, $\widehat g_{0i}=O_6(\widehat r^{-2})$, $\widehat g_{ij}=\delta_{ij}+O_6(\widehat r^{-1})$, with $\widehat T=\partial_{\widehat t}$. Its global topological radial chart can still put $S$ at radius one and agree with $\widehat x$ sufficiently far out. No stronger angular-momentum coefficient is asserted in this unchanged maximal-section time gauge.

## Statement references

[lem-author-29145f41e94d-homothetic-stationary-geometry](item-lem-author-29145f41e94d-homothetic-stationary-geometry)

[lem-author-d20d145f998f-normalized-stationary-end](item-lem-author-d20d145f998f-normalized-stationary-end)

[lem-author-d20d145f998f-cutoff-end-coordinate-extension](item-lem-author-d20d145f998f-cutoff-end-coordinate-extension)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-harrison-normalization](item-def-harrison-normalization)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:prop-properties-of-normal-coordinates-at-the-center](https://alphabetamath.cc/item/prop-properties-of-normal-coordinates-at-the-center)

[math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)

## Facts & Assumptions

[F1] Constant homothety preserves Ricci-flatness and maximality of the fixed section; maximality and the ADM surface integral use the stated hypersurface and mass conventions. [lem-author-29145f41e94d-homothetic-stationary-geometry](item-lem-author-29145f41e94d-homothetic-stationary-geometry) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-harrison-normalization](item-def-harrison-normalization)

[F2] Use the normalized stationary chart $(t^{\prime},y)$, $t^{\prime}=t+F(x)$, $y=f(x)$, and its $g_{00}=-1+2m/R+O_\infty(R^{-2})$, $R=|y|$. After the allowed orthogonal adjustment, the current cutoff supplier gives $f=x+O(\log r)$, $Df=I+O(r^{-1})$, $D^j f=O(r^{-j})$ for $2\le j\le7$, the corresponding inverse estimates, and a spatial cutoff diffeomorphism fixing $S$. Only that spatial cutoff is used. [lem-author-d20d145f998f-normalized-stationary-end](item-lem-author-d20d145f998f-normalized-stationary-end) [lem-author-d20d145f998f-cutoff-end-coordinate-extension](item-lem-author-d20d145f998f-cutoff-end-coordinate-extension)

[F3] Differentiated bounds are fixed-chart, angularly uniform estimates. Apply the chain, product and quotient rules componentwise; denominators are used only on tails where they are bounded away from zero. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)

[F4] Work in ZFC, retaining the choice assumptions of the normalized-end and cutoff suppliers. In orthonormal normal coordinates the metric equals $\delta$ and its first derivatives vanish at the center. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:prop-properties-of-normal-coordinates-at-the-center](https://alphabetamath.cc/item/prop-properties-of-normal-coordinates-at-the-center)

[F5] The two independently cited quotient inputs are recorded in External input. The normalized-end supplier's Statement supplies the same chart $y=\xi/|\xi|^2$, the identity $\gamma=\Omega_D^2\bar h$, and the potential-defined compactification with the regularity and normalization hypotheses (17)–(19). Thus the cited analytic compactification and conformal-factor results apply to this chosen $y$ chart. [lem-author-d20d145f998f-normalized-stationary-end](item-lem-author-d20d145f998f-normalized-stationary-end)

## External input

Source 0, (2.34) and (2.72), gives $g=V(dt+a)^2+h_{\rm quot}$ and $\bar h=(-V)h_{\rm quot}$. Its multipole theorem is the weak-decay input used by the normalized-end supplier; its particular spatial gauge is not assumed to be the chart $y$.

Source 1, Theorem 2.1, its following paragraph and Lemma 2.4, supplies the analytic conformal quotient metric $\gamma$ in normal coordinates $\xi$ and $\Omega=|\xi|^2 f_\Omega$ with analytic positive $f_\Omega(0)=1$. The normalized-end Statement identifies its chosen chart as $y=\xi/|\xi|^2$ and supplies the actual hypotheses (17)–(19).

## Proof

**Given:** The complete hypotheses in the Statement, in ZFC.

**Goal:** Establish the mass and decay conclusions while retaining the original maximal section.

1.1 Keep the original time $t$ and put $x=p(y)=f^{-1}(y)$, $J^i{}_a=\partial_a p^i$. The inverse estimates in [F2] imply $r\asymp R$, $J=I+O_6(R^{-1})$ and $D^j p=O(R^{-j})$ for $2\le j\le7$. For any $u=O_6(r^{-b})$, repeated chain differentiation of $u\circ p$ has factors $D^\ell u$ and $D^{j_1}p,\ldots,D^{j_\ell}p$ with $\sum j_i=k\le6$. Bounded first derivatives and the stronger bounds for $j_i\ge2$ give $D^k(u\circ p)=O(R^{-b-k})$. The tensor transformation law at fixed $t$ is $G_{00}=g_{00}\circ p$, $G_{0a}=(g_{0i}\circ p)J^i{}_a$, $G_{ab}=(g_{ij}\circ p)J^i{}_aJ^j{}_b$. Therefore $G_{0a}=O_6(R^{-2})$ and $G_{ab}=\delta_{ab}+O_6(R^{-1})$. The scalar $G_{00}=g(T,T)$ is independent of stationary time gauge, so the normalized chart in [F2] gives $G_{00}=-1+2m/R+O_6(R^{-2})$ with its full differentiated remainder. This last remainder is not inferred merely from $f-x=O(\log r)$. [F2, F3, given]

2.1 On a far tail put $V=G_{00}$ and $a_a=G_{0a}/V$. Then $V$ stays negative and away from zero, and [F3] gives $a=O_6(R^{-2})$. The decomposition in [F5] gives the metric of the original $t=0$ section as $h_\Sigma=h_{\rm quot}+V a\otimes a$, so $h_\Sigma-h_{\rm quot}=O_6(R^{-4})$. Thus neither this connection estimate nor its differentiated version requires taking the section $t^{\prime}=0$. [F3, F5, step 1.1]

3.1 To compute the ADM limit in this same $y$ gauge, use the analytic compact quotient data in [F5]. Write $s=|\xi|=R^{-1}$, $\omega=y/R$ and $Q=I-2\omega\otimes\omega$. By [F4], $\gamma_{ij}(\xi)=\delta_{ij}+O(s^2)$; analyticity gives $f_\Omega(\xi)=1+c\cdot\xi+O(s^2)$ for a fixed vector $c$. The inversion differential is $D_y\xi=s^2Q$, with $Q^TQ=I$. Since $\gamma=\Omega^2\bar h$, transforming back gives $\bar h=f_\Omega^{-2}Q^T\gamma Q=\delta-2(c\cdot\omega)\delta/R+O_1(R^{-2})$; the differentiated remainder follows by differentiating the convergent analytic series after inversion. An orthogonal adjustment of $y$ merely rotates $c$. Dividing by $-V=1-2m/R+O_1(R^{-2})$ and using step 2.1 yields $h_{\Sigma,ab}=(1+u)\delta_{ab}+O_1(R^{-2})$, where $u=2(m-c\cdot\omega)/R$. This allows the possible dipole term of this conformal gauge instead of identifying it with the distinct multipole gauge of source 0. [F2, F3, F4, F5, step 1.1, step 2.1]

4.1 For $(1+u)\delta$, the ADM integrand contracted with the Euclidean outward normal is $-2\partial_R u=4(m-c\cdot\omega)/R^2$. The $O_1(R^{-2})$ tensor remainder contributes $O(R^{-3})$ pointwise and hence $O(R^{-1})$ after integration. On the unit sphere $\int\omega\,d\omega=0$ by antipodal symmetry and $\int d\omega=4\pi$. Consequently the ADM integral divided by $16\pi$ tends to $m$. This is a direct calculation on the unchanged section. [F1, step 3.1, algebra]

5.1 Under $\widehat t=t/m$, $\widehat x=y/m$ and $\widehat g=m^{-2}g$, the new components equal $G_{\mu\nu}(m\widehat x)$, since both coordinate differentials contribute a factor $m$. Step 1.1 and the chain rule give exactly the three stated $O_6$ mass-one component bounds, and $mT=\partial_{\widehat t}$. On a coordinate sphere the derivative in the ADM integrand contributes $m$, while Euclidean area contributes $m^{-2}$ relative to the old sphere of radius $m\widehat R$; its unit radial vector is unchanged. Thus the ADM limit is $m^{-1}$ times the limit in step 4.1, hence one. By [F1] the same section remains maximal and Ricci-flatness is preserved. [F1, F3, step 1.1, step 4.1]

6.1 Apply only the spatial cutoff diffeomorphism in [F2] to the original section chart. It fixes a neighborhood of $S$ and agrees with $y$ on the far end; no time graph is introduced. If its radial coordinate is $q$, choose $B>A>1$ sufficiently large that $B/m>A$. A smooth positive derivative can equal $1$ near $A$ and $1/m$ near $B$ and have integral $B/m-A$: choose short endpoint collars with total integral smaller than this positive number, then adjust a positive interior profile to give the remaining integral. Integrating and using $\rho(q)=q$ below $A$, $\rho(q)=q/m$ above $B$, gives a smooth increasing radial diffeomorphism fixing radius one. The chart $z\mapsto\rho(|z|)z/|z|$ therefore retains the sphere at radius one and agrees with $y/m$ sufficiently far out. All claims concern the original section; no leading angular-momentum term in its time gauge was used. [F2, F4, step 5.1, construct] ∎

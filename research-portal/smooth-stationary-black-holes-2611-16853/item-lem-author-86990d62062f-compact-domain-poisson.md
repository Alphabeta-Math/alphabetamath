---
title: Compact-domain scalar Poisson solvability and fourth-order estimates
status: published
research_item: lem-author-86990d62062f-compact-domain-poisson
dependency_level: 1
sources:
  references:
    - title: Armin Schikorra, Partial Differential Equations I & II, version October
        1, 2025
      url: https://sites.pitt.edu/~armin/pde2022/pde.pdf
      locator: §8.9, Theorem 8.31, printed p.153 (PDF page 153), with admissibility of
        smooth bounded domains in Theorem 8.30, printed p.152.
      statement: A classical solution of a uniformly elliptic scalar Dirichlet
        equation on a bounded smooth domain has C^{2,alpha} regularity and its
        Schauder estimate when the coefficients and forcing are C^{0,alpha}, the
        boundary data are C^{2,alpha}, and c <= 0.
      hypotheses: 0 < alpha < 1; bounded uniformly elliptic principal coefficients;
        Holder drift and reaction; smooth bounded domain; classical solution
        continuous to the boundary. Here c=0 and the localized boundary data are
        zero.
      reading_limits: Consulted the online PDF extracted statements of Theorems 8.30
        and 8.31 and the surrounding boundary discussion. Only this second-order
        result is imported from this reference; neither its full
        continuity-method proof nor any fourth-order theorem is claimed to have
        been reviewed.
    - title: David Gilbarg and Neil S. Trudinger, Elliptic Partial Differential
        Equations of Second Order, 2001 reprint of the 1998 edition
      url: https://djvu.online/file/jxRRleAzbYjsl
      locator: Chapter 6, §6.4, Theorems 6.17 and 6.19, printed pp.109–112, including
        the local-boundary-portion paragraph after Theorem 6.19; §6.2, Lemma
        6.4, printed p.95, and Corollary 6.7, printed p.100, equation (6.38).
      statement: A classical solution with C^{k,alpha} coefficients and forcing is
        C^{k+2,alpha} locally, also at a C^{k+2,alpha} boundary portion with
        C^{k+2,alpha} Dirichlet values. The local second-order boundary estimate
        bounds the C^{2,alpha} norm by the forcing norm, boundary-data norm and
        solution supremum away from artificial edges.
      hypotheses: Integer k >= 0, 0 < alpha < 1, strict ellipticity with uniform
        bounds on the patches, C^{k,alpha} coefficients and forcing, u in C^2 in
        the interior and continuous to the specified boundary portion. For
        boundary regularity that portion and its data are C^{k+2,alpha}. The
        local second-order estimate requires u in C^{2,alpha} up to that portion
        and positive separation from other boundary portions. We use k=2, smooth
        charts, c=0 and zero data.
      reading_limits: Read the online book transcription of the stated results, the
        difference-quotient equation (6.49), the proof of Theorem 6.19 and its
        locality paragraph, and the hypotheses and conclusion of Lemma 6.4 and
        Corollary 6.7. The transcription has OCR defects; the regularity
        statements were also checked against MIT 18.156 Lectures 16 and 17. No
        full-book proof review, manifold solvability theorem, or directly quoted
        fourth-order norm estimate is claimed. The fourth-order estimate is
        derived locally below after regularity is established.
---

## Prerequisites

- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [math:thm-lax-milgram](https://alphabetamath.cc/item/thm-lax-milgram)
- [math:thm-rellich-kondrachov-for-p-less-than-n](https://alphabetamath.cc/item/thm-rellich-kondrachov-for-p-less-than-n)
- [math:thm-higher-order-boundary-regularity-for-dirichlet-problems](https://alphabetamath.cc/item/thm-higher-order-boundary-regularity-for-dirichlet-problems)
- [math:thm-boundary-schauder-estimate-for-the-dirichlet-problem](https://alphabetamath.cc/item/thm-boundary-schauder-estimate-for-the-dirichlet-problem)
- [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-higher-order-sobolev-embedding](https://alphabetamath.cc/item/thm-higher-order-sobolev-embedding)
- [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)
- [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)
- [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density)
- [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)
- [math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary)
- [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm)
- [math:thm-sobolev-spaces-are-banach-spaces](https://alphabetamath.cc/item/thm-sobolev-spaces-are-banach-spaces)
- [math:def-hilbert-space](https://alphabetamath.cc/item/def-hilbert-space)
- [math:thm-extension-theorem-for-bounded-smooth-domains](https://alphabetamath.cc/item/thm-extension-theorem-for-bounded-smooth-domains)
- [math:thm-lp-trace-operator-on-a-bounded-c-one-domain](https://alphabetamath.cc/item/thm-lp-trace-operator-on-a-bounded-c-one-domain)
- [math:thm-zero-weak-gradient-implies-componentwise-constancy](https://alphabetamath.cc/item/thm-zero-weak-gradient-implies-componentwise-constancy)
- [math:lem-nested-domain-induction-for-interior-elliptic-derivatives](https://alphabetamath.cc/item/lem-nested-domain-induction-for-interior-elliptic-derivatives)
- [math:lem-weak-divergence-form-equations-are-invariant-under-c-two-boundary-charts](https://alphabetamath.cc/item/lem-weak-divergence-form-equations-are-invariant-under-c-two-boundary-charts)
- [math:lem-cutoff-difference-quotient-commutator-estimate](https://alphabetamath.cc/item/lem-cutoff-difference-quotient-commutator-estimate)
- [math:lem-c-k-boundary-flattening-preserves-wkp-locally](https://alphabetamath.cc/item/lem-c-k-boundary-flattening-preserves-wkp-locally)
- [` Armin Schikorra, Partial Differential Equations I & II, version October 1, 2025 · §8.9, Theorem 8.31, printed p.153 (PDF page 153), with admissibility of smooth bounded domains in Theorem 8.30, printed p.152. `](https://sites.pitt.edu/~armin/pde2022/pde.pdf)
- [` David Gilbarg and Neil S. Trudinger, Elliptic Partial Differential Equations of Second Order, 2001 reprint of the 1998 edition · Chapter 6, §6.4, Theorems 6.17 and 6.19, printed pp.109–112, including the local-boundary-portion paragraph after Theorem 6.19; §6.2, Lemma 6.4, printed p.95, and Corollary 6.7, printed p.100, equation (6.38). `](https://djvu.online/file/jxRRleAzbYjsl)


## Statement

Fix $0<\alpha<1$. Let $M$ be a compact smooth Riemannian three-manifold with smooth boundary, every connected component meeting the boundary. For $f\in C^{2,\alpha}(M)$ there is a unique $u\in C^{4,\alpha}(M)$ with $\Delta_hu=f$ and $u|_{\partial M}=0$. On a fixed smaller interior or boundary chart the fourth-order norm is bounded by the $C^{2,\alpha}$ norm of $f$ on a larger chart and the supremum of $u$ there. The constants depend on $\alpha$, the fixed smooth metric and charts, and the separation from artificial chart edges. Here $C^{k,\alpha}$ means derivatives through order $k$ continuous to the boundary and order-$k$ derivatives $\alpha$-Hölder. No orientability of $M$ is assumed. Work in ZFC, supplying the choice assumptions of the analytic inputs.

## Statement references

[def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

**Given:** the Statement hypotheses and $0<\alpha<1$; work in ZFC.

[F1] Smooth boundary charts and finite smooth partitions of unity are available. The exterior-data definition fixes the Riemannian metric, coordinate Hölder conventions and Laplacian sign; it is not used as a topology reduction of $M$ to a Euclidean domain. [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary) [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F2] The Riemannian density and its associated measure are independent of orientation; measurable integration is the partition-weighted coordinate integral. For boundary charts the boundary hyperplane has three-dimensional Lebesgue measure zero. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density) [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)

[F3] Euclidean weak Sobolev spaces are complete, smooth bounded domains admit bounded Sobolev extensions, Rellich gives $W^{1,2}$ compactness into $L^2$ in dimension three, the trace is bounded and agrees with continuous boundary restriction, and zero weak gradient implies componentwise constancy. A complete inner-product space is Hilbert. [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm) [math:thm-sobolev-spaces-are-banach-spaces](https://alphabetamath.cc/item/thm-sobolev-spaces-are-banach-spaces) [Sobolev extension on smooth domains](https://alphabetamath.cc/item/thm-extension-theorem-for-bounded-smooth-domains) [math:thm-rellich-kondrachov-for-p-less-than-n](https://alphabetamath.cc/item/thm-rellich-kondrachov-for-p-less-than-n) [math:thm-lp-trace-operator-on-a-bounded-c-one-domain](https://alphabetamath.cc/item/thm-lp-trace-operator-on-a-bounded-c-one-domain) [math:thm-zero-weak-gradient-implies-componentwise-constancy](https://alphabetamath.cc/item/thm-zero-weak-gradient-implies-componentwise-constancy) [math:def-hilbert-space](https://alphabetamath.cc/item/def-hilbert-space)

[F4] Lax–Milgram applies to a bounded coercive bilinear form on a real Hilbert space. Weak boundary regularity gives a two-derivative gain on smooth bounded Dirichlet domains, and the separately declared nested-domain lemma supplies the interior gain. For weak solutions with locally square-integrable data, aligned boundary charts preserve the weak equation and, after localization, zero Dirichlet data. Smooth cutoff products have the stated weak-derivative bounds. The pullback of arbitrary Sobolev functions is supplied separately in [F6] and step 1.1. In dimension three, $H^4$ embeds into $C^{2,\gamma}$ for $0<\gamma<1/2$ on smooth bounded patches. [math:thm-lax-milgram](https://alphabetamath.cc/item/thm-lax-milgram) [math:thm-higher-order-boundary-regularity-for-dirichlet-problems](https://alphabetamath.cc/item/thm-higher-order-boundary-regularity-for-dirichlet-problems) [math:lem-nested-domain-induction-for-interior-elliptic-derivatives](https://alphabetamath.cc/item/lem-nested-domain-induction-for-interior-elliptic-derivatives) [math:lem-weak-divergence-form-equations-are-invariant-under-c-two-boundary-charts](https://alphabetamath.cc/item/lem-weak-divergence-form-equations-are-invariant-under-c-two-boundary-charts) [math:lem-cutoff-difference-quotient-commutator-estimate](https://alphabetamath.cc/item/lem-cutoff-difference-quotient-commutator-estimate) [math:thm-higher-order-sobolev-embedding](https://alphabetamath.cc/item/thm-higher-order-sobolev-embedding)

[F5] Classical second-order interior and global Dirichlet Schauder regularity and estimates are supplied by the library. The distinct imported higher-order regularity and local boundary estimate are specified in External input. [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations) [math:thm-boundary-schauder-estimate-for-the-dirichlet-problem](https://alphabetamath.cc/item/thm-boundary-schauder-estimate-for-the-dirichlet-problem)

[F6] For an integer $m\ge1$, let $T:U\to V$ be a $C^m$ diffeomorphism of open subsets of $\mathbb R^3$. Let $U_0\Subset U$ and $V_0\Subset V$ be open with $T(U_0)\subseteq V_0$, and assume bounded derivatives through order $m$ of $T$ on $\overline{U_0}$ and of $T^{-1}$ on $\overline{V_0}$. Then every $z\in W^{m,2}(V_0)$ has $z\circ T\in W^{m,2}(U_0)$, with a norm bound depending only on the dimension, $m$ and these chart bounds, and its weak derivatives satisfy the iterated chain rule. There is no differential-equation hypothesis. The supplier is initially applied only on patches compactly contained in the open coordinate interiors; step 1.1 extends the estimate to the boundary half-patches used here. [Sobolev boundary flattening](https://alphabetamath.cc/item/lem-c-k-boundary-flattening-preserves-wkp-locally)

## External input

The Schikorra reference supplies only the second-order global Dirichlet regularity statement under its stated admissibility hypotheses; smooth bounded domains are admissible. The corresponding library interface is [F5].

The Gilbarg–Trudinger reference supplies higher-order classical regularity (Theorems 6.17 and 6.19, with its local-boundary-portion conclusion) and the second-order local boundary estimate (Lemma 6.4 and Corollary 6.7). For the former, $C^{k,\alpha}$ coefficients and forcing give $C^{k+2,\alpha}$ regularity of a given classical solution, locally up to a $C^{k+2,\alpha}$ boundary portion carrying such Dirichlet values. For the latter, a given $C^{2,\alpha}$ solution has its smaller-patch norm bounded by the larger-patch forcing norm, Dirichlet-data norm and solution supremum, with positive separation from artificial edges. Uniform ellipticity, the coefficient bounds and $0<\alpha<1$ are required. These are imported Euclidean facts, not a claim to have reconstructed their proofs. No manifold existence result or fourth-order estimate is imported.

## Proof

**Given:** the Statement hypotheses; $0<\alpha<1$; ZFC. **Goal:** construct the solution and prove its fourth-order local estimate.

**Proof technique:** direct, combining a local Hilbert-space construction with the declared weak and classical regularity inputs.

1.1 First establish pullback bounds independently of any equation or manifold Sobolev construction. Let $T$ be a smooth coordinate transition between interior patches or between the open interiors of matched boundary half-patches. Restrict to patches with compact closure inside the ambient chart neighbourhoods, allowing that closure to meet the physical boundary. Boundary-chart compatibility in [F1] gives local ambient smooth extensions of the transition and its inverse. After finite subdivision, their derivatives through any fixed integer order $m\ge1$ are bounded and their Jacobians are bounded away from zero on these closures. For arbitrary $z\in H^m$ on the target patch, apply [F6] on compactly contained open interior subpatches: $D^\nu(z\circ T)$ is the sum of $(D^\beta z)\circ T$ times the prescribed bounded polynomials in derivatives of $T$, including order zero. These weak identities agree on overlapping interior subpatches. Exhaust the source open patch by such subpatches, choosing larger target interior subpatches containing their images. The norm estimates in [F6] have one common constant, since they depend only on $m$, dimension and the stated uniform chart and inverse bounds. Their right sides are bounded by the norm on the whole target patch. Taking the increasing integrals of the nonnegative squared derivative fields proves $\|z\circ T\|_{H^m}\le C\|z\|_{H^m}$ on the whole source half-patch, with the same weak identities. Every test function has compact support in that open half-patch, so these are its global weak derivatives. The inverse transition has the analogous bound. In particular $m=1$ applies to arbitrary functions and Cauchy sequences, without assuming that they are weak solutions; $m\le4$ also supplies the higher-order pullbacks used below. [F1, F6]

2.1 Let $d\mu_h$ be the measure of [F2], whose chart density is $\sqrt{\det h}\,dx$. Choose finitely many relatively compact coordinate patches and smooth cutoffs $\chi_i$ with $\sum_i\chi_i=1$. Each cutoff is supported away from artificial chart edges. In a boundary chart use a bounded smooth auxiliary domain in $\{x_3>0\}$ with a flat boundary portion covering that support; round its other boundary away from the support. Define $H^1(M)$ to consist of $L^2(d\mu_h)$ classes with local weak first derivatives and finite norm $\|v\|_{H^1_h}^2=\int_M(v^2+|dv|_h^2)\,d\mu_h$. On the compact supports, smooth metric positivity and bounded chart Jacobians make this norm equivalent to the square root of the sum of the squared Euclidean $W^{1,2}$ norms of $\chi_i v$, extended by zero only past artificial edges. The product formula bounds these local norms by the intrinsic norm; conversely $v=\sum_i\chi_i v$ and $dv=\sum_i d(\chi_i v)$ give the reverse bound. For arbitrary functions, coordinate changes obey the weak chain rule and bounded pullback estimates of step 1.1. Thus different such finite atlases give the same space and equivalent norms. All integrals are intrinsic density integrals, including on a nonorientable $M$. [F1, F2, F3, F4, step 1.1]

3.1 If $v_j$ is Cauchy in this norm, each $\chi_i v_j$ converges in Euclidean $W^{1,2}$ by completeness. The local limits agree as pieces of one function: on overlaps the identities $\chi_l(\chi_i v_j)=\chi_i(\chi_l v_j)$ pass to the $L^2$ limits using bounded coordinate pullbacks. Sum the finitely many pieces to obtain $v$; then $\chi_i v$ is the corresponding local limit. Testing against compactly supported smooth functions shows that its derivative limits are the weak derivatives of $v$. The norm equivalence proves $v_j\to v$ in $H^1_h$. The displayed norm comes from the positive-definite inner product $\int_M(vw+\langle dv,dw\rangle_h)\,d\mu_h$, so $H^1(M)$ is a real Hilbert space. Its closed subspace $H^1_0(M)$, defined as the closure of $C_c^\infty(M\setminus\partial M)$ in this norm, is Hilbert: a Cauchy sequence converges in $H^1(M)$ and its limit lies in that closure. [F2, F3, step 1.1, step 2.1]

4.1 The inclusion $H^1(M)\to L^2(M)$ is compact by applying Rellich with $p=q=2$, $n=3$, on the finitely many smooth auxiliary domains and taking finitely many successive subsequences; the extension theorem verifies the domain hypothesis. The local bounded trace operators give zero trace for every member of $H^1_0(M)$ by its defining closure. If Poincaré failed, choose $v_j\in H^1_0(M)$ with $\|v_j\|_2=1$ and $\|dv_j\|_2\to0$. Compactness gives an $L^2$ limit $v$. In charts, distributional testing gives $dv=0$; moreover $v_j\to v$ in $H^1_h$, so $v\in H^1_0(M)$. Zero-gradient constancy in connected coordinate interiors, and agreement on overlaps, give one constant on each component of $M$; the interior of each connected boundary manifold is connected, since a path may be pushed off the boundary in finitely many half-charts. Each component has a boundary chart, whose flat open boundary piece has positive surface measure. Its constant has zero trace there, hence is zero. This contradicts $\|v\|_2=1$. Thus $\|v\|_2\le C\|dv\|_2$ on $H^1_0(M)$. Choice is used only as permitted in the analytic suppliers and the subsequence argument. [F1, F2, F3, step 3.1]

5.1 On this Hilbert space the form $a(v,w)=\int_M\langle dv,dw\rangle_h\,d\mu_h$ is bounded and coercive by Poincaré. The functional $w\mapsto-\int_Mfw\,d\mu_h$ is bounded by Cauchy–Schwarz, since $f$ is continuous and the compact manifold has finite volume. Lax–Milgram gives one weak solution $u\in H^1_0(M)$, and it is unique there. In a chart its equation is $\partial_i(A^{ij}\partial_j u)=mf$, where $m=\sqrt{\det h}$ and $A^{ij}=mh^{ij}$. The smooth matrix $A$ is uniformly positive on every fixed compact patch. To match the positive-principal-part convention for $-\partial_i(A^{ij}\partial_j)$ in the weak regularity supplier, take forcing $-mf$. On overlapping aligned boundary charts the weak-equation invariance input applies to this solution with locally $L^2$ forcing and smooth uniformly elliptic coefficients. After a cutoff, its zero-Dirichlet assertion applies by the defining compactly supported smooth approximations to $u$. These solution-specific assertions are used only here; the arbitrary-function construction used step 1.1. [F2, F4, step 1.1, step 3.1, step 4.1]

6.1 In interior patches apply the declared nested-domain interior regularity lemma with $k=2$; $mf\in H^2$ and all coefficient bounds hold. At a boundary, localize with nested smooth cutoffs on smooth auxiliary domains of step 2.1. The localized function has zero Dirichlet data on the flat portion by the defining smooth approximations to $u$, and vanishes near every artificial boundary. The cutoff commutator contains only smooth multiples of $u$ and $Du$. Initially it is $L^2$, so the boundary theorem with $k=0$ gives local $H^2$. On a smaller patch the new commutator is now $H^1$ and $mf\in H^1$; use $k=1$ for $H^3$. On one further smaller patch it is $H^2$ and $mf\in H^2$; use $k=2$ for $H^4$. The arbitrary-function pullback bounds of step 1.1 and the multiplier bounds of [F4] justify each localization. Thus no undeclared interior counterpart or premature differentiation is needed. Smooth auxiliary domains satisfy the Sobolev extension hypothesis, so $H^4\hookrightarrow C^{2,\gamma}$ for any fixed $0<\gamma<1/2$. The weak equation is therefore classical and its zero trace is its continuous boundary value. [F1, F3, F4, step 1.1, step 2.1, step 5.1]

7.1 Write the classical coordinate equation as $Lu=h^{ij}u_{ij}+b^j u_j=f$, with smooth $b^j=m^{-1}\partial_i(mh^{ij})$ and zero reaction coefficient. The interior second-order Schauder interface gives $C^{2,\alpha}$ on smaller interior patches. On a boundary auxiliary domain apply the global boundary interface to $\eta u$: its forcing is $\eta f+[L,\eta]u$, and its entire boundary value is zero. Here $u\in C^{2,\gamma}$ already, so $[L,\eta]u$ has bounded first derivatives on the fixed compact patch and is $C^{0,\alpha}$ for every $0<\alpha<1$. Hence this application gives $C^{2,\alpha}$ up to the boundary as well. Now the imported higher-order regularity theorem applies with $k=2$ to each classical chart solution: the coefficients are smooth, $f\in C^{2,\alpha}$, the physical boundary is smooth and the data there are zero. Its local-boundary-portion version ignores artificial chart edges. It gives $u\in C^{4,\alpha}$ on smaller patches, hence on $M$ by a finite cover. This use is of the imported regularity theorem, not an assertion that second-order estimates alone license differentiating a merely $H^4$ solution. [F1, F5, step 6.1]

8.1 It remains to obtain the stated estimate with only the larger-chart data and supremum. Fix enough nested subpatches between the specified smaller and larger patches. Let $E_j(V)=\|u\|_{C^{j,\alpha}(V)}$ and $G_j(V)=\|f\|_{C^{j,\alpha}(V)}$. The interior second-order estimate or the imported local boundary estimate gives $E_2(V')\le C(G_0(V)+\|u\|_{0;V})$. All subsequent differentiations are legitimate by step 7.1. In the interior, $L(D_lu)=D_lf-(D_lh^{ij})u_{ij}-(D_lb^j)u_j$; the second-order estimate on nested patches gives $E_3(V')\le C(G_1(V)+E_2(V))$. Differentiate twice and apply it again to obtain $E_4(V')\le C(G_2(V)+E_3(V))$. At a flattened boundary, apply the local second-order estimate first to $D_tu$ and then to $D_sD_tu$, with $s,t$ tangential. Their boundary values are zero, and the differentiated forcing uses coefficient derivatives through order two and solution derivatives of strictly lower order. For order three these estimates control derivatives with at least one tangential factor; the equation solved for $u_{nn}$, divided by $h^{nn}\ge\lambda>0$, recovers $u_{nnn}$. For order four the two-tangential estimates control all derivatives with at most two normal factors. Apply $D_tD_n$ to the same identity to recover those with three normal factors, then $D_n^2$ to recover $u_{nnnn}$; all other highest-order terms have fewer normal factors, and coefficient-derivative terms use derivatives of $u$ of order at most three. This proves the same two recurrences at the boundary. Composing them on the nested patches gives $\|u\|_{4,\alpha;U'}\le C(\|f\|_{2,\alpha;U}+\|u\|_{0;U})$. Constants use only the ellipticity, coefficient $C^{2,\alpha}$ bounds and fixed chart separations; in particular this argument does not require a global topology restriction on $U$. [F1, F5, step 7.1]

9.1 Any classical solution with zero boundary values belongs to $H^1_0(M)$: cut it off in boundary charts at distance $\varepsilon$ from the flat face. Since it is $C^1$ and vanishes there, $u=O(x_n)$, so the cutoff error and its gradient tend to zero in $L^2$ on the shrinking boundary layer; finite partitions and interior smoothing give the defining compactly supported smooth approximations. The homogeneous weak energy identity may therefore be tested with the difference of two solutions, giving $\int_M|du|_h^2\,d\mu_h=0$. Poincaré gives $u=0$. Together with the constructed solution and step 8.1, this proves the Statement. [F1, F2, step 4.1, step 5.1, step 7.1, step 8.1] ∎

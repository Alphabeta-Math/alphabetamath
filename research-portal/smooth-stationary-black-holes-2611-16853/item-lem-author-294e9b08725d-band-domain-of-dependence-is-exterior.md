---
title: The exterior is the interior domain of dependence in the glued ambient
status: draft
research_item: lem-author-294e9b08725d-band-domain-of-dependence-is-exterior
dependency_level: 15
sources:
  references: []
---

## Prerequisites

- [lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice)
- [lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing](item-lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing)
- [lem-author-294e9b08725d-abstract-complete-boost-band](item-lem-author-294e9b08725d-abstract-complete-boost-band)
- [thm-author-294e9b08725d-radu-local-bifurcate-collar-input](item-thm-author-294e9b08725d-radu-local-bifurcate-collar-input)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [lem-author-9e5789a3d617-exterior-exclusion-interface](item-lem-author-9e5789a3d617-exterior-exclusion-interface)
- [thm-stationary-maximal-slice-existence-input](item-thm-stationary-maximal-slice-existence-input)


## Statement

For the complete strongly causal ambient $M_*$ obtained by adjoining the small full boost band, put $A=C_0\cup S$ and use the causal convention $D_{M_*}(A)=D^+_{M_*}(A)\cup D^-_{M_*}(A)$: membership in $D^+_{M_*}(A)$ requires every past-inextendible causal half-curve ending at the point to meet $A$, and membership in $D^-_{M_*}(A)$ requires every future-inextendible causal half-curve starting there to meet $A$. Then $\operatorname{int}D_{M_*}(C_0\cup S)=E$. In addition $E\subset I^-_{M_*}(M^{\rm end})\cap I^+_{M_*}(M^{\rm end})$, so the CW black/white-region exclusion holds on this interior. No assertion about the domain of dependence in the whole doubled development is used.

For the CW source convention, define $D^{\mathrm{tim}}_{M_*}(A)$ to be the set of points through which every inextendible timelike curve in $M_*$ meets $A$. Then $\operatorname{int}D^{\mathrm{tim}}_{M_*}(A)=E$ as well, and the same black/white-region exclusion holds on this interior. The two domain-of-dependence conventions are retained separately; no general equality of their sets is asserted.

The CW end in this assertion is $M_{\rm ext}=\bigcup_{s\in\mathbb R}\Phi_s(\Sigma_1)$, where $\Phi_s$ is the complete stationary flow on $M_*$ and $\Sigma_1=C_0\cap M^{\rm end}=\{t=0,\ |x|>R_0\}$ is its single stationary end. This union equals the embedded original $M^{\rm end}$. Define the ambient regions by $B_*=M_*\setminus I^-_{M_*}(M_{\rm ext})$ and $W_*=M_*\setminus I^+_{M_*}(M_{\rm ext})$. The exclusion asserted above is $(B_*\cup W_*)\cap E=\varnothing$, applied to each of the two identified interiors.

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[F1] The chosen section is Cauchy in $E$, and the ambient is the original exterior plus only the explicit small band. [lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice) [lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing](item-lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing)

[F2] The normal coordinates have exact boost action and the metric agrees with a smooth Lorentzian germ along compact $S$. [lem-author-294e9b08725d-abstract-complete-boost-band](item-lem-author-294e9b08725d-abstract-complete-boost-band) [thm-author-294e9b08725d-radu-local-bifurcate-collar-input](item-thm-author-294e9b08725d-radu-local-bifurcate-collar-input)

[F3] The end $M^{\rm end}$ is open in the original smooth time-oriented Lorentzian spacetime $M$, and $E=I^-_M(M^{\rm end})\cap I^+_M(M^{\rm end})$. Consequently each $p\in E$ has future timelike witness paths from some $a\in M^{\rm end}$ to $p$ and from $p$ to some $b\in M^{\rm end}$, initially taken in $M$. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F4] The causal domain is the union of the one-sided domains defined by past- and future-inextendible causal curves. Inextendibility means absence of an endpoint limit in the specified ambient. Restrictions preserve the causal and timelike curve classes, concatenation joins curves of either class at a common endpoint, and timelike curves are causal. Smooth composition preserves local absolute continuity and obeys the almost-everywhere velocity chain rule. Piecewise $C^1$ curves with future timelike tangents belong to the timelike class. The curve-calculus choice hypotheses hold in the ZFC convention of the regular-spacetime data. [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets) [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F5] For the CW convention, the stationary-end union is $M_{\rm ext}=\bigcup_i\bigcup_{s\in\mathbb R}\Phi_s(\Sigma_i)$, where the $\Sigma_i$ are the chosen section ends. Black and white regions are the ambient complements of its chronological past and future. For any subset $U$ of that ambient, their union misses $U$ exactly when $U$ is contained in both chronological sets. Only this end convention from the existence input and the independently proved set-theoretic exclusion interface are used here; no maximal-section existence conclusion is invoked. [thm-stationary-maximal-slice-existence-input](item-thm-stationary-maximal-slice-existence-input) [lem-author-9e5789a3d617-exterior-exclusion-interface](item-lem-author-9e5789a3d617-exterior-exclusion-interface)

[F6] The regular end has coordinates $\mathbb R\times\{|x|>R_0\}$ with $T=\partial_t$, and the original section there is $t=0$. The canonical section retains this end. The glued ambient stationary action agrees with the original complete stationary action on the invariant exterior piece, as established in the gluing construction, Proof 5.1. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice) [lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing](item-lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing)

## Proof

**Given:**The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[F1] The chosen section is Cauchy in $E$, and the ambient is the original exterior plus only the explicit small band. [lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice) [lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing](item-lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing)

[F2] The normal coordinates have exact boost action and the metric agrees with a smooth Lorentzian germ along compact $S$. [lem-author-294e9b08725d-abstract-complete-boost-band](item-lem-author-294e9b08725d-abstract-complete-boost-band) [thm-author-294e9b08725d-radu-local-bifurcate-collar-input](item-thm-author-294e9b08725d-radu-local-bifurcate-collar-input)

[F3] The end $M^{\rm end}$ is open in the original smooth time-oriented Lorentzian spacetime $M$, and $E=I^-_M(M^{\rm end})\cap I^+_M(M^{\rm end})$. Consequently each $p\in E$ has future timelike witness paths from some $a\in M^{\rm end}$ to $p$ and from $p$ to some $b\in M^{\rm end}$, initially taken in $M$. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F4] The causal domain is the union of the one-sided domains defined by past- and future-inextendible causal curves. Inextendibility means absence of an endpoint limit in the specified ambient. Restrictions preserve the causal and timelike curve classes, concatenation joins curves of either class at a common endpoint, and timelike curves are causal. Smooth composition preserves local absolute continuity and obeys the almost-everywhere velocity chain rule. Piecewise $C^1$ curves with future timelike tangents belong to the timelike class. The curve-calculus choice hypotheses hold in the ZFC convention of the regular-spacetime data. [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets) [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)



1.1 Suppose $p\in E$ were outside $D^+_{M_*}(A)\cup D^-_{M_*}(A)$. Choose a past-inextendible causal half-curve ending at $p$ and a future-inextendible causal half-curve starting at $p$, both avoiding $A$. Concatenating them gives an inextendible causal curve $\gamma$ in $M_*$ avoiding $A$. Restrict $\gamma$ to the connected component of $\gamma^{-1}(E)$ containing its visit to $p$. This restriction is inextendible in $E$: at a parameter end internal to the domain of $\gamma$, continuity and openness of $E$ would extend that component if its endpoint were in $E$; at an original parameter end, a limit in $E$ would also be a limit in $M_*$, contradicting inextendibility of $\gamma$. The supplied Cauchy property in $E$ forces the restricted causal curve to meet $C_0\subset A$, a contradiction. Therefore $E\subset D_{M_*}(A)$; openness of $E$ gives the forward interior inclusion. For the separately defined timelike-curve convention, take any inextendible timelike curve through $p\in E$. Its component inside $E$ is inextendible there by the same endpoint argument, and is causal, so the Cauchy property forces it to meet $C_0$. Thus $E\subset D^{\mathrm{tim}}_{M_*}(A)$, and openness gives the corresponding interior inclusion. [F1, F4, construct, contradiction]

1.2 Every added open non-right quadrant has an inextendible timelike curve avoiding the right section. In the left wedge, the boost field is timelike with the opposite orientation from the right wedge. For either time direction add a sufficiently small outward radial component, proportional to $r$, to the appropriate signed boost field. It stays timelike and reaches the artificial boundary $r=\delta$ in finite boost time, because $dr/dt=ar$ with fixed sufficiently small $a>0$; compactness of $S$ and a smaller uniform $\delta$ give a common cone margin. Hence both curve ends exit the band through its excluded left cutoff, without entering the right wedge. [F1, F2, F3, algebra]

1.3 Fix $p\in E$ and its original witness paths $a\ll_M p\ll_M b$ from F3. Choose $a_-,b_+\in M^{\rm end}$ with short future timelike segments $a_-\ll_M a$ and $b\ll_M b_+$ entirely in the end. For this local construction, take a coordinate chart in the open end about each endpoint, choose a future timelike vector there, and hold its coordinate components constant: continuity of the smooth metric and time orientation keeps that vector future timelike on a sufficiently small chart neighborhood, and sufficiently short straight coordinate segments remain in that neighborhood. The piecewise $C^1$ clause of F4 makes them timelike curves in the adopted class. The same construction on both sides of any $x\in M^{\rm end}$ shows $M^{\rm end}\subset E$. Concatenate these segments with the two witness paths. For every point $q$ on either original witness path, including $a,p,b$, restriction and timelike concatenation give $a_-\ll_M q\ll_M b_+$. Thus $q\in I^+_M(M^{\rm end})\cap I^-_M(M^{\rm end})=E$. Both original witness paths, including their end endpoints, therefore lie entirely in $E$. [F3, F4, construct]

2.1 For an added future timelike quadrant, translate the point by the abstract stationary action to $(U,V)=(-r,r)$. A short past timelike segment reaches the left section $U=V=-r/4$: its normal displacement has strictly timelike Minkowski limit, uniformly for small $\delta$. Continue to the excluded left cutoff as above. In the future direction the outward timelike normal ray reaches $|UV|=\delta^2$ in that timelike quadrant. Translate this whole curve back; quadrants and excluded cutoff are invariant. The past timelike quadrant is handled by time reversal. The resulting curves have both endpoints on excluded non-right cutoff and avoid $C_0\cup S$, so they are inextendible within $M_*$. Their past and future halves are causal and avoid $A$, witnessing nonmembership in both one-sided causal domains. Points on the non-right axes or at $S$ cannot lie in the interior of the domain of dependence, since every neighborhood contains such added points outside it. This proves the reverse interior inclusion. These full inextendible witnesses are timelike and avoid $A$, so they also exclude every added open quadrant from $D^{\mathrm{tim}}_{M_*}(A)$. Every non-right axis point, including $S$, is approached by such points. Therefore none of those axis points is interior to this timelike-curve domain either, proving $\operatorname{int}D^{\mathrm{tim}}_{M_*}(A)=E$. [F1, F2, F4, step 1.2, algebra]

2.2 The gluing embeds $E$ with its original metric and time orientation in $M_*$. Smooth composition and the velocity chain rule in F4 show that the two witness paths remain future timelike after this embedding, since its differential preserves their metric and time orientation. Their end endpoints $a,b$ are also in $E$ by step 1.3, so $a\ll_{M_*}p\ll_{M_*}b$ gives $E\subset I^-_{M_*}(M^{\rm end})\cap I^+_{M_*}(M^{\rm end})$. [F1, F3, F4, step 1.3, algebra]

2.3 By step 1.3 the original end is contained in the embedded $E$. Use its unchanged coordinates and the compatible action in F6. For every $x$ with $|x|>R_0$, the orbit through $(0,x)\in\Sigma_1$ is $\Phi_s(0,x)=(s,x)$ for all real $s$, entirely in that end. Thus every point of $M^{\rm end}$ lies in the stationary saturation of $\Sigma_1$, and every point in that saturation lies in $M^{\rm end}$. The CW convention in F5 uses exactly this one end of the chosen section, so $M_{\rm ext}=\bigcup_{s\in\mathbb R}\Phi_s(\Sigma_1)=M^{\rm end}$ in $M_*$. [F5, F6, step 1.3, algebra]

3.1 Substitute the identity from step 2.3 into the chronological inclusion of step 2.2. It gives $E\subset I^-_{M_*}(M_{\rm ext})\cap I^+_{M_*}(M_{\rm ext})$. Apply the exclusion equivalence in F5 with ambient $M_*$ and $U=E$: $(B_*\cup W_*)\cap E=\varnothing$. Since steps 1.1 and 2.1 identify both domain interiors with $E$, this is the asserted exclusion on each interior, including the exact timelike-curve domain used by CW. All chronological sets and complements in this application are taken in $M_*$; no global exterior-identification claim for $\widehat M$ is required. [F5, step 2.2, step 2.3, step 1.1, step 2.1, algebra] ∎

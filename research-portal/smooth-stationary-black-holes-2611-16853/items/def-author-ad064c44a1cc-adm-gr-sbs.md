---
id: def-author-ad064c44a1cc-adm-gr-sbs
title: Radu small-ADM global and bifurcation package
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-causal-exterior-and-boundary-data
  - def-spacelike-maximal-hypersurface-data
  - def-null-screen-expansion-and-focal-data
  - def-stationary-asymptotic-decay-data
  - physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets
  - def-author-ad064c44a1cc-nontrapping-sbs
  - math:def-a-smooth-map-transverse-to-an-embedded-submanifold
  - physics:lem-gr-fx-null-normal-plane-and-screen
  - math:def-transverse-embedded-submanifolds
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets: mathematical-premise
  def-author-ad064c44a1cc-nontrapping-sbs: mathematical-premise
  math:def-a-smooth-map-transverse-to-an-embedded-submanifold: mathematical-premise
  physics:lem-gr-fx-null-normal-plane-and-screen: mathematical-premise
  math:def-transverse-embedded-submanifolds: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: §1.1 opening setup; GR, equation (1.1) and the immediately following
        charge/decay conventions; SBS through its nonexpansion definition
        (before the separate maximality assumption).
      reading_limits: Retrieved the indicated arXiv HTML v1 and read §1.1 from the
        opening setup through GR, (1.1), the charge and differentiated-decay
        conventions, SBS and its expansion definition, and the adjacent separate
        maximality and quantitative-assumption paragraphs. Used only to
        transcribe the definition and distinguish its hypotheses; no rigidity
        proof, ADM surface-integral identification, or theorem acceptance is
        claimed. For this repair, re-read section 1.1 setup, GR through SBS and
        the adjacent separate maximality and quantitative paragraphs; checked
        the explicit distinct-point acausality wording against the retained
        local endpoint convention. No equivalence was inferred.
      statement: GR requires a global diffeomorphism Phi_0:E_{1/2}->Sigma^0 onto an
        embedded spacelike acausal edgeless partial Cauchy hypersurface, with
        acausality explicitly excluding causal curves between distinct points,
        the stationary end with expansion (1.1), a globally hyperbolic
        chronological exterior, the two prescribed slice/chronological
        intersections, and complete nonvanishing stationary orbits transverse to
        Sigma_1. SBS requires smooth transverse nonexpanding event boundaries
        meeting at S_0, tangent T, and T|S_0 not identically zero. The
        coefficients are named ADM mass M>0 and angular momentum vector S, with
        J=|S|. Maximality and the later quantitative conditions are separate
        assumptions. The additional coincident-endpoint exclusion in the local
        package is not imported from this source.
      hypotheses: A connected oriented time-oriented smooth four-dimensional
        Lorentzian manifold of signature (-,+,+,+), Ric(g)=0, and a smooth
        Killing field T. GR and SBS are additional supplied predicates, not
        conclusions from the vacuum equation. The source mass M is denoted M_0
        locally.
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609
      locator: Definition 2.19, printed/PDF p. 34; Definition 2.95, printed/PDF p. 63;
        §2.18, Definition 2.130, printed/PDF p. 76; §3.2, Definition 3.35,
        printed/PDF p. 95.
      statement: Achronality means I^+(A) intersect A is empty, including exclusion of
        closed timelike curves through A. Acausality excludes nonconstant causal
        curves with both endpoints in A, including coincident endpoints. For
        achronal A, edge(A) consists of closure points q such that every open
        neighborhood U admits p in I^-(q,U) and r in I^+(q,U) connected by a
        timelike curve in U avoiding A. An acausal edgeless set is called a
        partial Cauchy hypersurface.
      hypotheses: A time-oriented Lorentzian spacetime with at least C^2 metric; A is
        achronal for the edge definition, and acausal and edgeless for the
        partial-Cauchy terminology. The present metric is smooth and the
        specified hypersurface is additionally smooth and spacelike.
      reading_limits: Read the PDF text at Definitions 2.19, 2.95, 2.130 and 3.35 and
        their immediate surrounding paragraphs for the causal conventions and
        their application domains. Imported only these definitions. No global
        Cauchy property, causal-development theorem, existence theorem, or proof
        of a causal-ladder equivalence is claimed.
    - title: Alexandru F. Radu, On rigidity of stationary black holes under a
        nontrapping assumption
      url: https://arxiv.org/html/2609.23872v1
      locator: Version 1, §1.1 setup, GR and SBS; §1.2 opening paragraph.
      statement: SBS imposes no nonzero condition on T restricted to S_0. Section 1.2
        explicitly includes the identically-zero case and assigns its treatment
        to staticity in section 7.
      hypotheses: The source smooth oriented time-oriented stationary vacuum
        four-spacetime with its GR/SBS end and bifurcation sphere. Only the
        assumption/case distinction is imported, not the rigidity implication.
      reading_limits: Read v1 §1.1 setup, GR/SBS, NT and Theorem 1.1, and §1.2
        opening. Imported only the horizon-field case distinction; staticity and
        rigidity proofs were not reviewed.
dependency_level: 4
---

## Definition

The **Radu ADM GR/SBS package** consists of a connected oriented time-oriented smooth vacuum four-spacetime $(M,g)$ with a smooth stationary Killing field $T$, and an embedded spacelike acausal edgeless partial Cauchy surface $\Sigma^0$, supplied with a diffeomorphism $\Phi_0:E_{1/2}\to\Sigma^0$ onto the whole surface, where $E_a=\{x\in\mathbb R^3:|x|>a\}$ and $r=|x|$. Put $\Sigma_1=\Phi_0(E_1)$ and $S_0=\Phi_0(\{r=1\})$. The end chart extends to $M^{\rm end}\simeq\mathbb R\times E_{R_0}$ with $T=\partial_t$ and zero-time section agreeing with $\Sigma^0$. Its coefficients are
$$g_{00}=-1+2M_0/r+O_6(r^{-2}),\quad g_{ij}=\delta_{ij}+O_6(r^{-1}),\quad g_{0i}=-2\epsilon_{ijk}S^jx^kr^{-3}+O_6(r^{-3}),$$
with $M_0>0$ the source ADM mass, $S=(S^1,S^2,S^3)$ its ADM angular momentum vector, and $J=|S|=\sqrt{\sum_{i=1}^3(S^i)^2}$ its nonnegative Euclidean magnitude. Here $i,j,k\in\{1,2,3\}$ and $\epsilon_{ijk}$ is the alternating symbol with $\epsilon_{123}=1$. The exterior $E=I_M^-(M^{\rm end})\cap I_M^+(M^{\rm end})$ is globally hyperbolic, $\Sigma^0\cap I_M^\pm(M^{\rm end})=\Sigma_1$, and $T$ is nowhere zero on $E$, with every orbit complete and intersecting $\Sigma_1$ transversally.

Precisely, for every $p\in E$, let $\gamma_p:\mathbb R\to M$ be its complete smooth stationary orbit, with $\gamma_p(0)=p$ and $\dot\gamma_p(t)=T_{\gamma_p(t)}$. The orbit-intersection requirement is $\gamma_p^{-1}(\Sigma_1)\ne\varnothing$, and transversality means that for every $t\in\gamma_p^{-1}(\Sigma_1)$, writing $q=\gamma_p(t)$, one has $d\gamma_p|_t(T_t\mathbb R)+T_q\Sigma_1=T_qM$.

Here a set $A\subset M$ is acausal when no nonconstant future causal curve has both endpoints in $A$, including coincident endpoints; it is achronal when $I_M^+(A)\cap A=\varnothing$, which also excludes a closed timelike curve through any point of $A$. For an achronal set $A\subset M$, a point $q\in\overline A^{\,M}$ lies in $\operatorname{edge}(A)$ exactly when every open neighborhood $U$ of $q$ admits points $p\in I_U^-(q)$ and $r\in I_U^+(q)$ joined by a future timelike curve entirely in $U\setminus A$. The notation $I_U^\pm(q)$ uses curves contained in $U$ with the restricted metric and time orientation. Edgeless means $\operatorname{edge}(A)=\varnothing$; a partial Cauchy hypersurface means an acausal edgeless set, additionally embedded, smooth and spacelike here. These causal predicates are relative to the ambient spacetime $M$.

Radu's ADM source (§1.1 GR) uses acausality to exclude causal curves joining distinct points of the hypersurface. This local package retains that source requirement and additionally excludes nonconstant future causal curves whose two endpoints coincide at a point of $\Sigma^0$, as required by the Minguzzi convention just stated. The coincident-endpoint exclusion is an explicit additional local condition, not a consequence attributed here to Radu's GR. Thus the local condition supplies the source's distinct-point acausality; the converse and equivalence of conventions are not asserted.

Near $S_0$ the two event boundaries $H^\pm=\partial_M I_M^\mp(M^{\rm end})$ are smooth transverse nonexpanding null hypersurfaces, with $H^+\cap H^-=S_0$, $T$ tangent to both, and $T|_{S_0}\not\equiv0$. The ADM source thus requires a nonzero horizon field; Radu's *On rigidity of stationary black holes under a nontrapping assumption* (arXiv:2609.23872v1, §1.1 SBS and §1.2) permits $T|_{S_0}\equiv0$. Maximality, $J<M_0^2$ and the quantitative smallness assumptions are additional separately named conditions, not silently included in GR/SBS here.

A local smooth null hypersurface is a smooth embedded three-manifold without boundary whose induced tangent form is positive semidefinite of rank two. The two local horizon pieces are transverse when $T_qH^++T_qH^-=T_qM$ for every $q\in S_0$. These conditions apply to the horizon pieces near $S_0$ specified above.

## Facts & Assumptions

[F1] [[def-stationary-lorentzian-data]] and [[def-causal-exterior-and-boundary-data]] give the geometric and causal objects, [[def-spacelike-maximal-hypersurface-data]] the spacelike slice, [[def-null-screen-expansion-and-focal-data]] the zero-expansion condition, and [[def-stationary-asymptotic-decay-data]] the differentiated end notation.

[F2] Clause (a) of [[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]] supplies the spacelike embedded hypersurface convention. The acausality, achronality, edge and partial-Cauchy conventions used here are imported from Minguzzi, Definitions 2.95, 2.19, 2.130 and 3.35 respectively, as stated explicitly above.

[F3] Radu, §1.1 GR and SBS, supplies the source predicates, including the global diffeomorphism, distinct-point acausality, charge labels and rotating horizon condition. The coincident-endpoint exclusion in [F2] is retained explicitly as an additional local condition; it is not attributed to this source. The source's separate maximality and quantitative clauses are not included in GR/SBS.

[F4] [[def-author-ad064c44a1cc-nontrapping-sbs]] records the NT comparison, from Radu arXiv:2609.23872v1 §1.1 SBS and §1.2 opening. It does not add NT hypotheses to the ADM package.

[F5] [[math:def-a-smooth-map-transverse-to-an-embedded-submanifold]] defines transversality of a smooth map to an embedded submanifold. Apply it to each smooth stationary orbit $\gamma_p:\mathbb R\to M$ and the embedded hypersurface $\Sigma_1$; the separate nonempty-intersection requirement is retained.

[F6] [[physics:lem-gr-fx-null-normal-plane-and-screen]] supplies the smooth null-hypersurface definition, applied to the local horizon pieces in the smooth time-oriented Lorentzian four-spacetime of [[def-stationary-lorentzian-data]]. [[math:def-transverse-embedded-submanifolds]] supplies the tangent-space-sum definition of transversality, applied to these two embedded hypersurfaces at their intersection $S_0$. The choice convention for the null-geometry supplier is inherited from [[def-null-screen-expansion-and-focal-data]]. Only the defining clauses of these two interfaces are used here.

## Justification

The supplied global diffeomorphism determines the slice subsets and embeds the specified coordinate sphere; its end restriction and stationary extension determine the end arrays. The ambient causal relations determine the exterior, event boundaries and neighborhood-restricted chronological relations used in the edge predicate. The imported definitions make acausality, achronality and edgelessness definite conditions, with the edge predicate used only on achronal sets. The declared complete stationary orbits supply smooth orbit maps, and the smooth-map transversality definition gives exactly the displayed tangent-space condition at each slice intersection; the existence of an intersection remains a separate required predicate. The null-hypersurface interface applies in the supplied smooth time-oriented Lorentzian four-spacetime with the choice convention inherited from the null-expansion interface. Its rank-two induced-form condition and the embedded-submanifold transversality interface make the specified local horizon predicates definite. Smoothness and spacelikeness make the expansion trace and the surface metric meaningful. The displayed list retains Radu's GR/SBS predicates together with the explicitly additional local coincident-endpoint exclusion. The local acausality condition implies the source's distinct-point exclusion by restricting its endpoint quantifier to distinct points; no converse or equivalence is asserted or used. No implication is asserted between this local package and the original article's differently stated regularity package, and the theorem's separate maximality and quantitative assumptions are not folded into a generic GR label.

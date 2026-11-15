---
id: pthm-author-a4a441da4986-regular-nonrotating-schwarzschild-input
title: Independent regular nonrotating staticity and Schwarzschild theorem
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-causal-exterior-and-boundary-data
  - def-bifurcate-killing-horizon-data
  - def-stationary-asymptotic-decay-data
  - def-spacelike-maximal-hypersurface-data
  - def-null-screen-expansion-and-focal-data
  - physics:def-gr-schwarzschild-exterior-model
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  physics:def-gr-schwarzschild-exterior-model: mathematical-premise
provenance:
  statement: ai-altered
  proof: literature-derived
external_input: true
physical_scope: Conditional smooth four-dimensional asymptotically flat
  stationary vacuum black-hole model with the explicit global source hypotheses.
sources:
  references:
    - title: A. F. Radu, On rigidity of stationary black holes under a nontrapping
        assumption, arXiv:2609.23872v2
      url: https://arxiv.org/pdf/2609.23872v2
      locator: Section 1.1, GR and SBS, PDF/printed pp. 3–4; Lemma 2.13, p. 25;
        nonrotating branch of the proof of Theorem 1.1, pp. 69–70; Appendix A,
        pp. 71–74.
      statement: GR and SBS imply the exterior-preserving horizon completion in Lemma
        2.13. The nonrotating branch T|S0=0 on pp. 69–70 imports the auxiliary
        bifurcate completion and maximal foliation, proves staticity, and
        identifies the exterior with Schwarzschild. It records compact boundary
        where T=0, one asymptotically flat end, interior domain of dependence E,
        stationary translates foliating E, lapse tending to one, and
        |k|=O(r^-2), |X|=O(r^-1). SBS defines nonexpansion as zero trace of
        g(D_U L,V) on spacelike horizon cross-sections. NT is used in the
        rotating branch, not this branch.
      hypotheses: A connected oriented time-oriented smooth four-dimensional spacetime
        of signature (-,+,+,+), Ric(g)=0, and smooth stationary Killing field T.
        An embedded acausal edgeless spacelike partial Cauchy section
        Sigma-prime is parametrized by Phi0:{|x|>1/2}->Sigma-prime;
        Sigma1=Phi0({|x|>1}). The designated end is R times a Cartesian
        exterior, T=partial_t future-directed, with positive ADM rest mass M and
        g00=-1+2M/r+O6(r^-2), gij=delta+O6(r^-1), g0i=O6(r^-2). Sigma-prime
        agrees with t=0 on this end. E=I-minus(Mend) intersect I-plus(Mend) is
        globally hyperbolic, its stationary orbits are complete and meet Sigma1,
        and Sigma-prime intersect I-plus(Mend)=Sigma-prime intersect
        I-minus(Mend)=Sigma1. The event horizons partial I-minus(Mend) and
        partial I-plus(Mend) intersect in S=Phi0({|x|=1}); near S they are
        smooth transverse nonexpanding null hypersurfaces tangent to T. Restrict
        to T|S=0.
      reading_limits: In this adjudication, read the locally retained full-PDF text of
        pp. 3–4, 25, 69–70 and 71–74, and opened the independent arXiv PDF. The
        cited auxiliary completion and maximal existence are accepted as
        external inputs under the displayed GR/SBS hypotheses; no
        reconstruction, independent proof audit, or review of the
        rotating/nontrapping argument or cited static-uniqueness proofs is
        claimed. No visual-inspection credit from prior work is claimed. The
        studied article supplies no premise here.
    - title: P. T. Chruściel and R. M. Wald, Maximal Hypersurfaces in Asymptotically
        Stationary Spacetimes, arXiv:gr-qc/9304009
      url: https://arxiv.org/pdf/gr-qc/9304009
      locator: Section 2, Definition 2.1 and its Remarks 1–2, PDF pp. 8–9; Definition
        2.3, p. 11; Section 4, equations (4.1)–(4.3), Theorem 4.2 and Remark 3,
        pp. 24–25.
      statement: For a class-(b) spacetime with no black or white hole in the interior
        domain of dependence of its section, Theorem 4.2 supplies maximal
        asymptotically flat hypersurfaces with the same boundary, diffeomorphic
        to that section and covariant under stationary translation as in (4.2);
        their interiors are Cauchy surfaces. Under timelike convergence they
        foliate the interior domain of dependence. Definition 2.3 specifies a
        closed acausal section with compact core and asymptotic ends; its
        induced metric is complete including the boundary. Asymptotic regularity
        and differentiated falloff use Definition 2.1. Remark 3 allows
        logarithmic height, rather than an assumed constant asymptotic height.
      hypotheses: A strongly causal smooth time-oriented class-(b) spacetime with a
        connected closed acausal spacelike section having compact boundary,
        compact core and finitely many (k,alpha)-asymptotically stationary ends,
        k>=2 and 0<alpha<=1; a complete stationary field tangent to the
        boundary; and (B union W) intersect int D(Sigma)=empty. The foliation
        conclusion additionally requires the stationary field to be timelike on
        int D(Sigma) or Ric(Z,Z)>=0 for every timelike Z. Here the
        exterior-preserving preparation and applicability are imported from Radu
        pp. 69–70; vacuum provides timelike convergence and there is one end.
      reading_limits: Read the local PDF text of pp. 24–25 and the extracted PDF text
        of Definitions 2.1 and 2.3 on pp. 8–11. The theorem statement,
        definitions and Remark 3 are used, not a reconstruction of the
        maximal-existence proof or its cited elliptic estimates. Applicability
        of the auxiliary-spacetime preparation to GR/SBS is accepted at the
        precise independent Radu locator, not derived solely from the four
        formulation suppliers. No constant-height or improved orthogonal-end
        expansion is inferred here.
dependency_level: 2
---

## Statement

Assume the following independent-source GR and SBS contract. Let $(\mathcal M,g)$ be a connected oriented time-oriented smooth four-dimensional vacuum spacetime of signature $(-,+,+,+)$ with smooth stationary Killing field $T$. Let $\Sigma'\subset\mathcal M$ be an embedded acausal edgeless spacelike partial Cauchy hypersurface, with a diffeomorphism $\Phi_0:\{x\in\mathbb R^3:|x|>1/2\}\to\Sigma'$, and put $\Sigma_1=\Phi_0(\{|x|>1\})$. The designated end $M^{\rm end}\simeq\mathbb R\times\{x\in\mathbb R^3:r=|x|>R_0\}$ has $T=\partial_t$ future-directed, positive ADM rest mass $M$, and $g_{00}=-1+2M/r+O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$, $g_{0i}=O_6(r^{-2})$. Require that $\Sigma'$ agrees with $t=0$ on this end.

Define $E=I^-_{\mathcal M}(M^{\rm end})\cap I^+_{\mathcal M}(M^{\rm end})$ and require that it is globally hyperbolic, with complete stationary orbits meeting $\Sigma_1$, and that $\Sigma'\cap I^+_{\mathcal M}(M^{\rm end})=\Sigma'\cap I^-_{\mathcal M}(M^{\rm end})=\Sigma_1$. The future and past event horizons $\partial_{\mathcal M}I^-_{\mathcal M}(M^{\rm end})$ and $\partial_{\mathcal M}I^+_{\mathcal M}(M^{\rm end})$ meet in the embedded sphere $S=\Phi_0(\{|x|=1\})$. Their portions near $S$ are the specified smooth transverse null sheets $H^+$ and $H^-$, tangent to $T$. Require that both sheets are nonexpanding: for each local smooth nonzero null generator $L$ and spacelike cross-section with induced metric $\gamma$, the null second fundamental form $\chi_L(U,V)=g(\nabla_U L,V)$ on tangent $U,V$ has $\operatorname{tr}_\gamma\chi_L=0$.

If $T|_S=0$, then $E$ is static and globally isometric to the Schwarzschild exterior of positive mass $M$. Here staticity means that $T$ is timelike throughout $E$ and orthogonal to spacelike hypersurfaces, with $T^\flat\wedge dT^\flat=0$; the Schwarzschild exterior is the mathematical model with areal radius $\rho>2M$ in geometrized units $G_N=c=1$. No nontrapping or analyticity hypothesis is required in this nonrotating branch.

The source proof also supplies an exterior-preserving auxiliary completion and a stationary-covariant maximal Cauchy foliation of $E$. More precisely, the interiors $\Sigma_s$ of smooth spacelike hypersurfaces $\overline\Sigma_s$ with common compact bifurcation boundary $B$, where $T=0$, are Cauchy surfaces in $E$, foliate exactly $E$, and satisfy $\Sigma_{s+t}=\Phi_t^T(\Sigma_s)$ for the stationary flow. Each $\overline\Sigma_s$ has a compact core, one asymptotically Euclidean end, induced metric asymptotically Euclidean with differentiated bounds, and is smooth up to $B$ and complete with $B$ included. The boundary $B$ belongs to the auxiliary completion; no identification of its ambient neighborhood with the original one is assumed.

On each $\overline\Sigma_s$, let $n$ be the future unit normal, $h=g|_{T\overline\Sigma_s}$, $k(U,V)=-g(\nabla_U n,V)$, $N=-g(T,n)$ and $X=T-Nn$, so $T=Nn+X$ with $X$ tangent; maximality means $\operatorname{tr}_h k=0$. On the end the supplied estimates are $|k|_h=O(r^{-2})$, $|X|_h=O(r^{-1})$ and $N\to1$. These are the auxiliary outputs available to the local application lemmas; they are conclusions of the independent source preparation, not extra assumptions on the original section.

## Statement references

[[post-stationary-vacuum-model]]

[[def-causal-exterior-and-boundary-data]]

[[def-bifurcate-killing-horizon-data]]

[[def-stationary-asymptotic-decay-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-null-screen-expansion-and-focal-data]]

[[physics:def-gr-schwarzschild-exterior-model]]

## Facts & Assumptions

[A1] Adopt the vacuum model and the causal, horizon and differentiated asymptotic conventions, with precisely the additional GR/SBS relationships stated above. [[post-stationary-vacuum-model]] [[def-causal-exterior-and-boundary-data]] [[def-bifurcate-killing-horizon-data]] [[def-stationary-asymptotic-decay-data]]

[F1] The independent nonrotating branch supplies the completion, foliation, bounds and staticity/Schwarzschild conclusion under those GR/SBS hypotheses, as specified in source reference 0. Its cited maximal-slice theorem supplies the diffeomorphism type and stationary covariance under the auxiliary-spacetime hypotheses, as specified in source reference 1.

[F2] The spacelike-hypersurface interface fixes the future unit normal, induced metric, negative-sign second fundamental form, maximality, lapse, shift and completeness including a compact boundary. [[def-spacelike-maximal-hypersurface-data]]

[F3] Null second fundamental form and expansion on spacelike cross-sections have the stated trace convention. [[def-null-screen-expansion-and-focal-data]]

[F4] The Schwarzschild exterior model is a mathematical datum; take its positive mass parameter to be $M$ and its constants $G_N=c=1$. [[physics:def-gr-schwarzschild-exterior-model]]

## External input

Import the nonrotating branch of Radu’s proof of Theorem 1.1, PDF pp. 69–70, under GR and SBS on pp. 3–4, including the end-section alignment and the chronological definitions of the exterior and event horizons. Lemma 2.13, p. 25, and Appendix A, pp. 71–74, supply the exterior-preserving horizon completion. The nonrotating branch invokes the further auxiliary preparation for maximal existence, records the lapse/shift bounds, proves staticity and applies static uniqueness. Its use here is an explicit external input; the rotating branch’s NT assumption is not imported.

Chruściel–Wald Theorem 4.2, PDF p. 25 with (4.1)–(4.3) on pp. 24–25 and the class-(b) definition on p. 11, is the cited maximal-slice input: same boundary, diffeomorphism type, stationary covariance, Cauchy interiors and, under timelike convergence, foliation. Radu’s pp. 69–70 supply applicability through the auxiliary completion and vacuum equation. The differentiated asymptotic language uses Chruściel–Wald Definition 2.1; Remark 3 on p. 25 permits logarithmic height. No stronger constant-height conclusion or local reconstruction of maximal existence is claimed.

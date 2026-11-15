---
id: def-author-cf389990237c-normalized-horizon-komar-data
title: Normalized Komar data on a nonrotating horizon section
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - physics:thm-gr-killing-and-on-shell-matter-identities
  - math:def-riemannian-volume-form-on-an-oriented-manifold
  - math:def-axiom-of-choice
  - def-author-310ff0f53b38-asymptotically-flat-spacelike-end
  - physics:lem-emg-lorentz-hodge-calculus
  - math:prop-integration-over-an-oriented-embedded-submanifold
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  physics:thm-gr-killing-and-on-shell-matter-identities: mathematical-premise
  math:def-riemannian-volume-form-on-an-oriented-manifold: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-author-310ff0f53b38-asymptotically-flat-spacelike-end: mathematical-premise
  physics:lem-emg-lorentz-hodge-calculus: mathematical-premise
  math:prop-integration-over-an-oriented-embedded-submanifold: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: H. S. Reall, Black Holes, Part III lecture notes, 15 March 2024
      url: https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf
      locator: §8.1, (8.14) and the following coordinate-sphere definition, printed
        p.107 (PDF p.108); §8.2, (8.18)–(8.24), printed p.108 (PDF p.109); §9.1,
        (9.1)–(9.2) and preceding normalization paragraph, printed p.114 (PDF
        p.115).
      statement: For a stationary Killing field k normalized at the chosen end, Komar
        mass is -1/(8 pi) times the limit of the integral of star d(k-flat) over
        large spheres. The vacuum Killing identity makes this two-form closed.
        Killing-horizon surface gravity uses d(g(k,k))=-2 kappa k-flat.
      hypotheses: Oriented smooth four-dimensional spacetime of signature (-,+,+,+),
        geometrized units G=c=1, stationary Killing field, admissible
        asymptotically flat end and the indicated large-sphere limit. Horizon
        surface gravity is used on a Killing horizon for the specified field.
      reading_limits: Consulted the cached 15 March 2024 lecture-note PDF, PDF
        pp.108–109 and 115 (printed pp.107–108 and 114), including the
        coordinate-sphere sentence after (8.14), (8.18)–(8.24), and (9.1)–(9.2).
        The source supplies the Komar and signed surface-gravity conventions.
        The selected chart, explicit orientations and conditional definition of
        its limit are specified locally using the named suppliers; no limit
        existence, chart independence, global Stokes transport at a degenerate
        end or positive-mass application is inferred.
dependency_level: 1
---

## Definition

Work in ZFC, including choice, on an oriented smooth time-oriented Lorentzian four-manifold $(M,g)$ of signature $(-,+,+,+)$, with its Levi–Civita connection $\nabla$. Let $C$ be a smooth compact embedded spacelike horizon cross-section with induced positive metric $q$. Supply smooth normal fields $n,s$ along $C$ with $g(n,n)=-1$, $g(s,s)=1$, $g(n,s)=0$, $n$ future-directed and $s$ pointing outward toward the selected exterior. Orient $C$ by declaring $(v_1,v_2)$ positive exactly when $(n,s,v_1,v_2)$ is positive in $M$, and put $dA=\operatorname{vol}_q$ in that orientation. Thus $\int_C f\,dA$ is the intrinsic integral of the smooth top form $f\operatorname{vol}_q$ on oriented $C$, equivalently its positive Riemannian area integral. Put $b_{ab}=s_an_b-n_as_b$. For a smooth Killing field $T$, define the oriented horizon Komar functional by $Q_C[T]=-(8\pi)^{-1}\int_C(\nabla^aT^b)b_{ab}\,dA$.

In the nonrotating case require $T=c(n+s)$ on $C$ for a supplied smooth positive function $c$, and require that $T$ generate the smooth Killing horizon with $\nabla_TT=\kappa T$. The signed surface-gravity convention is equivalently $d(g(T,T))=-2\kappa T^\flat$ on the nonzero-generator part, with $T^\flat=g(T,\cdot)$. No bifurcation sphere is assumed.

For the exterior normalization and mass notation, additionally supply an asymptotically flat spacelike end $S_{\rm ext}$ with specified chart $\chi:\{x\in\mathbb R^3:|x|>R\}\to S_{\rm ext}$ and induced positive metric $\gamma$, using the end and derivative-decay convention stated in the references below. Set $r=|x|$ and $S_r=\chi(\{|x|=r\})$ for $r>R$. The field $T$ is future timelike at this end and is normalized there by $-g(T,T)\to1$ as $r\to\infty$. Let $n_{\rm ext}$ be the end's future unit normal and $s_r$ its outward unit normal to $S_r$ within $S_{\rm ext}$, with $dr(s_r)>0$. Orient $S_r$ so that $(v_1,v_2)$ is positive exactly when $(n_{\rm ext},s_r,v_1,v_2)$ is positive in $M$. The operators $d$ and $\star_g$ are the exterior derivative and Lorentzian Hodge star for $g$ and the supplied ambient orientation, with $\alpha\wedge\star_g\beta=\langle\alpha,\beta\rangle_g\operatorname{vol}_g$. If $j_r:S_r\hookrightarrow M$ is the inclusion, $\int_{S_r}\star_g dT^\flat$ means the intrinsic integral of $j_r^*(\star_g dT^\flat)$ on this oriented compact sphere. The notation $M_K$ denotes the exterior Komar mass in the source convention $M_K=-(8\pi)^{-1}\lim_{r\to\infty}\int_{S_r}\star_g dT^\flat$, whenever that limit exists. No identity $M_K=Q_C[T]$ is built into this definition.

## Definition references

[[def-stationary-lorentzian-data]]

[[def-bifurcate-killing-horizon-data]]

[[physics:thm-gr-killing-and-on-shell-matter-identities]]

[[math:def-riemannian-volume-form-on-an-oriented-manifold]]

[[math:def-axiom-of-choice]]

[[def-author-310ff0f53b38-asymptotically-flat-spacelike-end]]

[[physics:lem-emg-lorentz-hodge-calculus]]

[[math:prop-integration-over-an-oriented-embedded-submanifold]]

[Reall, Black Holes, §8.2 (8.24) and §9.1 (9.1)–(9.2)](https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf)

## Facts & Assumptions

[F1] Smooth metric, connection, musical maps, signed surface gravity and Killing-equation conventions use the named mathematical geometric interfaces. Work in ZFC, including the choice convention inherited by these suppliers; the supplied normals and end chart are data, not objects selected by an extra choice argument here. [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]] [[physics:thm-gr-killing-and-on-shell-matter-identities]] [[math:def-axiom-of-choice]]

[F2] On the oriented Riemannian surface $C$, $\operatorname{vol}_q$ is the smooth positive top form in positive charts. Compactly supported smooth top forms have the intrinsic finite-chart integral; the integration-on-submanifolds supplier applies with the identity embedding for forms defined on $C$ itself, and with $j_r$ for ambient forms restricted to $S_r$. [[math:def-riemannian-volume-form-on-an-oriented-manifold]] [[math:prop-integration-over-an-oriented-embedded-submanifold]]

[F3] The selected spacelike end supplies the specified exterior chart, induced metric, derivative-decay convention and smooth future unit normal. The Hodge-calculus supplier supplies the smooth Lorentzian Hodge star and exterior derivative on the oriented four-manifold; both are mathematical inputs. [[def-author-310ff0f53b38-asymptotically-flat-spacelike-end]] [[physics:lem-emg-lorentz-hodge-calculus]]

[F4] Reall §8.2 (8.24) fixes the exterior Komar factor $-(8\pi)^{-1}$, with coordinate spheres as specified after (8.14); §9.1 (9.1)–(9.2) gives the signed surface-gravity convention and the preceding paragraph gives the unit normalization at infinity. These are conventions, without an assertion of convergence or global horizon transport here. [Reall, Black Holes](https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf)

## Justification

**Given:** The supplied compact section, normal fields, Killing field and, for the exterior notation, selected end chart and normalization.

**Goal:** Check that the local functional and conditional exterior mass notation are meaningful.

1.1 The smooth ordered normal pair and ambient orientation give a smooth orientation on $C$ by the stated positive-basis rule. Lowering the normal fields and antisymmetrizing gives a smooth covariant two-tensor $b$. Raising the derivative of $T$ gives the smooth scalar $f=(\nabla^aT^b)b_{ab}$. Thus $f\operatorname{vol}_q$ is a smooth top form with compact support on compact $C$. Apply the integration supplier with the identity embedding $C\to C$: its finite-chart integral is defined and finite. This proves finiteness of $Q_C[T]$ without extending $dA$ to an ambient two-form. [given, F1, F2]

1.2 For each $r>R$, the end chart maps the Euclidean sphere to a compact smooth embedded surface $S_r$. The end metric is positive definite and $dr$ is nowhere zero, so its metric-dual vector normalized to unit length gives the smooth outward normal $s_r$; the positive-basis rule with $n_{\rm ext}$ orients $S_r$. The smooth ambient two-form $\star_g dT^\flat$ has a smooth pullback to $S_r$, whose support is compact. The integration supplier therefore defines each finite sphere integral. Its specified limit is a definite real number if it exists, and the source convention then defines $M_K$. [given, F2, F3, F4]

2.1 The outward and future choices fix the binormal sign convention; the positive area integral has the meaning established in step 1.1. The end normalization specifies the scale of $T$, and the signed equation defining $\kappa$ is meaningful on the nonzero-generator part. The exterior limit and any equality $M_K=Q_C[T]$ remain separate analytic assertions; neither is required to define the local functional. [given, F1, F4, step 1.1, step 1.2] ∎

## External input

Reall's lecture notes supply only the exterior Komar normalization in §8.2 (8.24), the coordinate-sphere convention following (8.14), and the signed Killing-horizon surface gravity and normalization in §9.1 (9.1)–(9.2) and its preceding paragraph, under the hypotheses and reading limits recorded in the source metadata. The local justification defines the integrals using the named mathematical suppliers. Global degenerate-end transport and zero-mass exclusion are separate imported applications, not claims justified by this notation.

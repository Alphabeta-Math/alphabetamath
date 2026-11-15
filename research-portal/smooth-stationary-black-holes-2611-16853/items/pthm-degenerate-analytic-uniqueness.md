---
id: pthm-degenerate-analytic-uniqueness
title: Analytic connected-horizon uniqueness including the degenerate case
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - def-author-cf389990237c-normalized-horizon-komar-data
  - lem-author-cf389990237c-normal-binormal-boost-invariance
  - lem-author-cf389990237c-horizon-killing-binormal-contraction
  - lem-author-cf389990237c-constant-gravity-horizon-komar-integral
  - lem-author-cf389990237c-degenerate-komar-zero-mass-implication
  - lem-author-cf389990237c-degenerate-generator-no-bifurcation
  - post-stationary-vacuum-model
  - def-horizon-rotation-surface-gravity
  - def-kerr-metric
  - pthm-analytic-connectedness-and-extremal-input
  - def-author-abbd1939ec07-connected-degenerate-comparison-data
  - def-black-hole-comparison-hypothesis-data
  - def-bifurcate-killing-horizon-data
  - math:def-axiom-of-choice
  - def-source-free-geometric-electrovacuum-data
  - physics:def-emg-xs-kn-data
  - physics:def-emg-xs-kn-full-sphere-exterior
  - physics:thm-emg-xs-kn-extension
  - physics:prop-emg-xs-kn-horizon-data
  - physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form
  - math:thm-embedded-submanifolds-admit-local-defining-submersions
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-causal-curve-calculus
dependency_roles:
  def-author-cf389990237c-normalized-horizon-komar-data: mathematical-premise
  lem-author-cf389990237c-normal-binormal-boost-invariance: mathematical-premise
  lem-author-cf389990237c-horizon-killing-binormal-contraction: mathematical-premise
  lem-author-cf389990237c-constant-gravity-horizon-komar-integral: mathematical-premise
  lem-author-cf389990237c-degenerate-komar-zero-mass-implication: mathematical-premise
  lem-author-cf389990237c-degenerate-generator-no-bifurcation: mathematical-premise
  post-stationary-vacuum-model: physical-assumption
  def-horizon-rotation-surface-gravity: mathematical-premise
  def-kerr-metric: mathematical-premise
  pthm-analytic-connectedness-and-extremal-input: physical-result
  def-author-abbd1939ec07-connected-degenerate-comparison-data: mathematical-premise
  def-black-hole-comparison-hypothesis-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  physics:def-emg-xs-kn-data: mathematical-premise
  physics:def-emg-xs-kn-full-sphere-exterior: mathematical-premise
  physics:thm-emg-xs-kn-extension: mathematical-premise
  physics:prop-emg-xs-kn-horizon-data: mathematical-premise
  physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form: mathematical-premise
  math:thm-embedded-submanifolds-admit-local-defining-submersions: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: P. T. Chruściel and L. Nguyen, A uniqueness theorem for degenerate
        Kerr-Newman black holes
      url: https://arxiv.org/pdf/1002.1737v1
      locator: Theorem 1.1, printed p.1; §2 opening paragraph, p.2; §3.2 opening
        paragraph, p.11
      statement: A stationary I-plus-regular analytic electrovacuum spacetime with
        connected nonempty rotating degenerate future event horizon has a domain
        of outer communications isometrically diffeomorphic to that of
        Kerr-Newman. Under these analytic regularity assumptions the rotating
        case has a global commuting axial U(1) symmetry. Section 3.2 uses
        electric and magnetic charge parameters and electromagnetic duality for
        the Kerr–Newman comparison.
      hypotheses: Four-dimensional asymptotically flat stationary analytic
        electrovacuum spacetime in the terminology inherited from
        Chruściel–Costa; connected nonempty rotating degenerate future event
        horizon. No nonrotating case is included.
      reading_limits: Read the web-extracted version-1 PDF at Theorem 1.1, the
        introduction, opening of §2, and opening of §3.2. The global comparison
        and symmetry are imported; the later global-coordinate and harmonic-map
        proofs and electromagnetic-duality calculations were not reconstructed.
        The maximal-surface caveat concerns a different staticity route.
    - title: P. T. Chruściel and J. L. Costa, On uniqueness of stationary vacuum black
        holes
      url: https://arxiv.org/pdf/0806.0016
      locator: Definition 1.1, printed p.2; Theorem 1.3, pp.3–4; §2.1, (2.5)–(2.8),
        p.6; Theorem 2.3, p.10; §2.2, (2.9)–(2.10), p.7; Theorem 4.5 and (4.15),
        p.18, with end-matching conclusion of its proof, p.22; §8 remark 2, p.55
      statement: "There are no stationary vacuum I-plus-regular black holes all of
        whose event-horizon components are nonrotating and degenerate: the
        source explicitly states the Komar/positive-energy nonexistence
        application. Its connected one-horizon case is a direct specialization.
        Separately, a stationary asymptotically flat I-plus-regular analytic
        four-dimensional vacuum spacetime with connected mean-nondegenerate
        future horizon has Kerr domain of outer communications. Theorem 4.5 for
        s=1 supplies a smooth acausal asymptotically flat slice spacelike up to
        its compact future-horizon boundary, in Definition 1.1’s finite-end
        compact-core class; its smoothing agrees with the chosen end at large
        distances. Theorem 2.3 prohibits causal communication between distinct
        asymptotically flat ends under global hyperbolicity and the null energy
        condition. Section 2.1 supplies adapted stationary coordinates with
        asymptotically vanishing shift. Theorem 4.5 also supplies a smooth time
        coordinate with spacelike levels up to the horizon boundary, in whose
        product description the stationary flow is translation. Section 2.2
        identifies the future horizon as the boundary of the chronological past
        of the selected stationary exterior."
      hypotheses: "For the first application: stationary, vacuum and I-plus-regular
        black-hole spacetime, with every event-horizon component nonrotating and
        degenerate; connected nonempty event horizon is the specialization used
        here. For Theorem1.3: the additional four-dimensional analytic and
        asymptotically flat conditions, connected horizon and nonzero mean
        surface gravity. The exact I-plus-regularity is Definition1.1, not an
        arbitrary incomplete exterior slice. The structure theorem needs a
        stationary I-plus-regular spacetime with the R action of its complete
        stationary field; s=1 imposes no axial symmetry. End separation is
        applied to the globally hyperbolic domain of outer communications
        itself, with its asymptotically flat ends and vacuum null energy
        condition. The stationary vacuum end uses the source’s derivative-decay
        convention. No maximal-slice or horizon-nondegeneracy hypothesis is
        added to Theorem 4.5."
      reading_limits: Read the cached PDF text at Definition 1.1, Theorem 1.3, §2.1
        pp.6–7, §2.3 p.8, Theorem 2.3 p.10, Theorem 4.5 p.18, and §8 remark 2
        p.55; cross-checked the structure theorem and its proof’s end-matching
        sentence in web PDF text. These theorems and the complete nonexistence
        application are imported. Their global smoothing, topological-censorship
        and positive-energy proofs were not reconstructed. Compact truncation
        and flux matching are the local application in Proof 1.2 and 2.2–3.1; no
        exclusion of mixed-horizon configurations is inferred. For this repair,
        independently read the web-extracted version-2 PDF at section 2.2,
        equations (2.9)–(2.10), the statement of Theorem 4.5 on printed page 18,
        equation (4.18) on page 20, and the closing paragraph on page 22. Only
        the stated time-coordinate/product and chronological-boundary
        conclusions are additionally imported; the generator sign and its
        application to the Komar frame are derived locally in Proof 2.2. No
        reconstruction of the source smoothing proof is claimed.
    - title: "P. T. Chruściel, J. L. Costa and M. Heusler, Stationary Black Holes:
        Uniqueness and Beyond"
      url: https://arxiv.org/pdf/1205.6112
      locator: §7.2, printed pp.38–39, especially (7.8) and its horizon-flux
        explanation; §2.5.3, pp.8–10; §3.3.1–3.3.2, including Theorem 3.3, p.16
      statement: The stationary mass identities evaluate the horizon Komar integral as
        kappa A/(4 pi). Evaluation for a nonrotating horizon uses the same
        Killing field for the asymptotic stationary normalization and the
        horizon generator; rotation requires the additional angular-momentum
        term. The source stresses that the mass-formula framework is not
        restricted to static configurations. The zeroth law gives constant
        vacuum Killing-horizon surface gravity; nonzero constant surface gravity
        has nonzero mean. Its analytic connected-horizon classification includes
        the mean-nondegenerate or rotating alternatives. Section 3.3.1 states
        that strong rigidity makes the event horizon a Killing horizon under the
        analytic comparison hypotheses.
      hypotheses: Stationary asymptotically flat smooth four-dimensional vacuum
        specialization of the source equations with compact horizon
        cross-section; nonrotating means the asymptotic stationary field itself
        generates the horizon. Global mass transport must have the source
        admissible hypersurface and boundary controls; it is not inferred from a
        local tensor identity. Analytic classification additionally uses the
        exact I-plus-regular connected-horizon hypotheses.
      reading_limits: "Read cached and web PDF text at §7.2 pp.38–39, §2.5.3 pp.8–10
        and §3.3.1–3.3.2 p.16. Imported the stated vacuum zeroth law,
        Killing-horizon and mean-gravity conventions and classification
        statement. The static electric example in (7.8) is not generalized to
        prove stationary global transport: that transport is separately
        established using Chruściel–Costa’s slice and Reall’s identity. The
        underlying rigidity and uniqueness proofs were not reconstructed."
    - title: H. S. Reall, Black Holes, Part III lecture notes, 15 March 2024
      url: https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf
      locator: §8.2, (8.18)–(8.24), printed p.108 (PDF p.109); §8.4, paragraph after
        (8.43), printed p.113 (PDF p.114)
      statement: For a stationary Killing field, (8.22) makes star d(T-flat) closed in
        vacuum; (8.23) gives the Stokes identity on a smooth compact
        hypersurface piece. Komar mass is its asymptotic flux with factor -1/(8
        pi). In a stationary asymptotically flat spacetime it equals ADM energy
        when the slicing is asymptotically orthogonal to the stationary field.
      hypotheses: Smooth oriented time-oriented four-dimensional stationary spacetime,
        signature (-,+,+,+), G=c=1, normalized stationary field, and vacuum for
        closedness. Stokes is applied only to compact smooth truncations with
        their complete oriented boundary. The ADM identification uses a
        stationary asymptotically flat end with slice normals approaching the
        stationary time direction.
      reading_limits: Read the cached 149-page PDF’s pages 109 and 114, including the
        displayed equations and the paragraph after (8.43). The browser
        retrieval timed out; no fresh download or full-notes reading is claimed.
        The source supplies the identity and asymptotic identification, while
        the current proof checks its hypersurface and boundary hypotheses using
        Chruściel–Costa. No local reconstruction of the ADM identification is
        claimed.
    - title: "T. Adamo and E. T. Newman, The Kerr-Newman metric: A Review"
      url: https://arxiv.org/pdf/1410.6626
      locator: §3.1, (3.1)–(3.2), printed p.13; §3.3, (3.18)–(3.21), pp.17–18, and
        extremality paragraph on p.18
      statement: The Boyer–Lindquist Kerr–Newman metric has outer event horizon r-plus
        = m + sqrt(m squared - a squared - q squared), exterior r > r-plus, and
        extremality m squared = a squared + q squared. Advanced coordinates
        remove the horizon coordinate singularity.
      hypotheses: Standard asymptotically flat Kerr–Newman comparison spacetime, m>0
        and m squared >= a squared + q squared; azimuthal period 2 pi. The
        metric signature in this source is opposite to the item’s (-,+,+,+)
        convention.
      reading_limits: Read the web-extracted PDF at the complete (3.1)–(3.2) formulas
        and §3.3 through the extremality paragraph. Imported the standard
        exterior/horizon identification, not a reconstruction of the maximal
        analytic extension. Full-sphere tensor regularity is checked locally
        with the existing mathematical suppliers. No electromagnetic-potential
        or field-uniqueness claim is drawn from this reference.
physical_scope: Conditional four-dimensional asymptotically flat stationary
  analytic vacuum Einstein black-hole classification, and the connected rotating
  degenerate source-free Einstein–Maxwell comparison, with zero cosmological
  constant and full I-plus-regularity. No empirical measurement or
  dynamical-settling assertion.
dependency_level: 9
---

## Statement

Adopt the four-dimensional asymptotically flat stationary analytic vacuum model with the full $I^+$-regularity and connected nonempty future event-horizon assumptions of the black-hole comparison data. Use the stationary vacuum model, the rotation and signed surface-gravity convention, and the Kerr convention listed below. Then the entire domain of outer communications is isometric to that of a Kerr spacetime.

More specifically, a connected rotating degenerate horizon has global axial symmetry and its vacuum exterior is extremal Kerr, under the precise connected-degenerate comparison data and the first contract of the analytic/extremal supplier. Electrovacuum means the source-free geometric Einstein–Maxwell equations and conventions listed below. The corresponding stationary analytic $I^+$-regular electrovacuum spacetime with connected nonempty rotating degenerate future horizon has Kerr–Newman domain of outer communications, under Chruściel–Nguyen's exact source hypotheses. The full Kerr–Newman metric exterior meant here is specified in Comparison exterior below.

For a single nonrotating vacuum horizon, normalize the stationary generator by $-g(T,T)\to1$ at the chosen end. Let $M=M_K$ be its normalized exterior Komar mass, equivalently the ADM energy in the asymptotic stationary rest frame, and let $A$ be the area of a compact horizon section. Then $M=\kappa A/(4\pi)$. The global transport needed for this identity uses the smooth horizon-reaching slice supplied by $I^+$-regularity; it is established separately from the local horizon evaluation. In the degenerate case $\kappa=0$, the independently sourced Komar/positive-energy exclusion rules out a regular $I^+$-regular black hole. No bifurcation-based staticity argument is used for a degenerate horizon. A nonzero degenerate generator has no regular bifurcation sphere for that same generator. Work in ZFC, including choice.

## Statement references

[[def-black-hole-comparison-hypothesis-data]]

[[post-stationary-vacuum-model]]

[[def-horizon-rotation-surface-gravity]]

[[def-kerr-metric]]

[[def-author-abbd1939ec07-connected-degenerate-comparison-data]]

[[pthm-analytic-connectedness-and-extremal-input]]

[[def-source-free-geometric-electrovacuum-data]]

[[def-author-cf389990237c-normalized-horizon-komar-data]]

[[lem-author-cf389990237c-degenerate-generator-no-bifurcation]]

[[def-bifurcate-killing-horizon-data]]

[[math:def-axiom-of-choice]]

## Comparison exterior

For this item the Kerr–Newman comparison exterior is the following full metric domain, rather than just a sufficiently distant tail. Let $m>0$, $a,q\in\mathbb R$, $m^2\ge a^2+q^2$, $r_+=m+\sqrt{m^2-a^2-q^2}$, and $D_{\rm KN}=\mathbb R_t\times(r_+,\infty)_r\times S^2$. On the unit sphere use the smooth round metric $\gamma$, coordinate functions $(X,Y,Z)$, $b=1-Z^2$, and $\lambda=X\,dY-Y\,dX$. Put $R=r^2+a^2$, $\Sigma=r^2+a^2Z^2$ and $\Delta=r^2-2mr+a^2+q^2$. The full-sphere tensor is
$$g_{\rm KN}=-\frac{\Delta-a^2b}{\Sigma}dt^2+\frac{\Sigma}{\Delta}dr^2+\Sigma\gamma+\frac{a^2(R+\Sigma-\Delta)}{\Sigma}\lambda^2-\frac{2a(R-\Delta)}{\Sigma}dt\odot\lambda.$$
Here $u\odot v=(u\otimes v+v\otimes u)/2$ and $\lambda^2=\lambda\otimes\lambda$. Off the axes this is the Boyer–Lindquist tensor of [[physics:def-emg-xs-kn-data]], with $x^0=t$ and $M=m$; its global sphere expression is the same recipe as [[physics:def-emg-xs-kn-full-sphere-exterior]], now on every $r>r_+$. The azimuthal period is $2\pi$ and the time orientation agrees near infinity with $\partial_t$, using the regular ingoing extension in [[physics:thm-emg-xs-kn-extension]]. The independent exterior identification in Import 5 identifies this domain with the domain of outer communications of the standard Kerr–Newman comparison spacetime relative to its selected asymptotically flat end. The rotating degenerate comparison has $a\ne0$ and $m^2=a^2+q^2$, so $r_+=m$. Only the metric is being compared; the parameter $q^2$ can represent the sum of squared electric and magnetic charges, as in Import 1. In particular no global electromagnetic potential is required by this formulation.

## Facts & Assumptions

[A1] Adopt exactly the stationary vacuum model, analytic and asymptotically flat comparison class, full $I^+$-regularity, connected nonempty future horizon and stated field normalizations. Retain the ZFC convention. [[post-stationary-vacuum-model]] [[def-black-hole-comparison-hypothesis-data]] [[def-horizon-rotation-surface-gravity]] [[def-bifurcate-killing-horizon-data]] [[math:def-axiom-of-choice]]

[F1] The rotating degenerate vacuum comparison is the first contract of the analytic/extremal supplier, with its exact connected-degenerate formulation. No multiple-horizon balance contract is used. [[pthm-analytic-connectedness-and-extremal-input]] [[def-author-abbd1939ec07-connected-degenerate-comparison-data]]

[F2] The local Komar suppliers fix the normal binormal, its boost invariance, the Killing-horizon contraction, the constant-gravity integral and the conditional zero-mass implication. In particular $Q_C[T]=\kappa A/(4\pi)$ when $\kappa$ is constant, and $M_K=Q_C[T]$ must be supplied separately before inferring zero exterior mass. [[def-author-cf389990237c-normalized-horizon-komar-data]] [[lem-author-cf389990237c-normal-binormal-boost-invariance]] [[lem-author-cf389990237c-horizon-killing-binormal-contraction]] [[lem-author-cf389990237c-constant-gravity-horizon-komar-integral]] [[lem-author-cf389990237c-degenerate-komar-zero-mass-implication]]

[F3] A regular bifurcation branch is incompatible with a nonzero generator having zero acceleration coefficient. [[lem-author-cf389990237c-degenerate-generator-no-bifurcation]]

[F4] The Kerr definition fixes the subextremal/extremal parameter convention. The electrovacuum definition fixes the geometric field equations. [[def-kerr-metric]] [[def-source-free-geometric-electrovacuum-data]]

[F5] Imports 1–3 supply the rotating-degenerate electrovacuum comparison and global symmetry, the nonrotating-degenerate exclusion and mean-nondegenerate vacuum comparison, and the vacuum zeroth law and mean-gravity convention.

[F6] Import 2 additionally supplies the smooth horizon-reaching spacelike slice, separation of distinct asymptotic ends, the adapted asymptotic stationary coordinates, and a smooth time coordinate whose spacelike levels extend to the horizon section and whose stationary flow is translation. Its future-increasing sign is fixed by the future stationary field at the selected end. Section 2.2 identifies the future horizon with the boundary of the chronological past of the selected stationary exterior. Import 4 supplies the stationary vacuum Komar–Stokes identity and the ADM-energy identification in that asymptotic frame. Neither input requires a maximal or bifurcation slice.

[F7] The exact Boyer–Lindquist tensor, sphere recipe, and regular ingoing extension are mathematical inputs; only their metric and coordinate conclusions are used. For $m>0$ and $m^2\ge a^2+q^2>0$, the local horizon-data proposition gives $\kappa_+=(r_+-r_-)/(2(r_+^2+a^2))$, including the double root. Import 5 supplies the standard comparison-exterior identification. [[physics:def-emg-xs-kn-data]] [[physics:def-emg-xs-kn-full-sphere-exterior]] [[physics:thm-emg-xs-kn-extension]] [[physics:prop-emg-xs-kn-horizon-data]]

[F8] A spacelike hypersurface has a unique smooth future unit normal, obtained locally from its timelike normal covector and hence also up to a smooth spacelike boundary. A smooth embedded horizon has a local defining submersion. Chronological pasts are open past sets, and concatenation of future timelike curves gives chronological transitivity. These are mathematical inputs; the causal suppliers' Countable Choice and Dependent Choice assumptions hold in A1's ZFC setting. [[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form]] [[math:thm-embedded-submanifolds-admit-local-defining-submersions]] [[physics:lem-gr-chronology-openness]] [[physics:lem-gr-causal-curve-calculus]]

## External input

Import 1: Chruściel–Nguyen Theorem 1.1 supplies the entire rotating-degenerate electrovacuum comparison; §2 supplies global axial symmetry. The opening of §3.2 treats electric and magnetic charges by electromagnetic duality. These inputs do not treat nonrotating degenerate horizons. [Chruściel–Nguyen](https://arxiv.org/pdf/1002.1737v1)

Import 2: Chruściel–Costa §8 remark 2 supplies the nonexistence of stationary vacuum $I^+$-regular black holes when every horizon component is nonrotating and degenerate, including the global applicability of its positive-energy argument. Theorem 1.3 supplies connected mean-nondegenerate analytic vacuum uniqueness. Theorem 4.5, with $s=1$, supplies a smooth acausal spacelike hypersurface up to its compact future-horizon boundary, in the finite-end compact-core setting of Definition 1.1; its smoothing agrees with the chosen end at large distances. Theorem 2.3 separates distinct asymptotically flat ends in a globally hyperbolic spacetime satisfying the null energy condition. Section 2.1 gives the adapted stationary end with asymptotically vanishing shift. Theorem 4.5 also gives a smooth time coordinate with spacelike level hypersurfaces up to their horizon boundary, with the stationary flow acting as translation in its product description. The sign increasing to the future is fixed by the future stationary field at the selected end. Section 2.2, (2.9)–(2.10), identifies the future event horizon as the boundary of $I^-(M_{\rm ext})$. [Chruściel–Costa](https://arxiv.org/pdf/0806.0016)

Import 3: Chruściel–Costa–Heusler §3.3.1 supplies the Killing-horizon conclusion under the analytic comparison hypotheses; §2.5.3 supplies constant vacuum Killing-horizon surface gravity and its compatibility with nonzero mean surface gravity. Section 7.2 supplies the horizon mass-integral convention and its same-generator restriction. Its static electric illustration alone is not used to establish global transport for a general stationary horizon. [Chruściel–Costa–Heusler](https://arxiv.org/pdf/1205.6112)

Import 4: Reall §8.2, (8.18)–(8.24), gives $d(\star_g dT^\flat)=0$ in vacuum and its Stokes identity on a smooth compact spacelike piece, with Komar factor $-(8\pi)^{-1}$. Section 8.4 following (8.43) identifies this mass with ADM energy for an asymptotic stationary slicing whose normals approach the stationary time direction. The existence and boundary control of the piece used here come from Import 2, rather than from the local horizon integral. [Reall](https://www.damtp.cam.ac.uk/user/hsr1000/black_holes_lectures_2024.pdf)

Import 5: Adamo–Newman §3.1, (3.1)–(3.2), and §3.3, (3.18)–(3.21) and the extremality paragraph, identify the standard Kerr–Newman exterior as $r>r_+$, with outer event horizon $r_+$ and extremality $m^2=a^2+q^2$. Their opposite signature is converted to $(-,+,+,+)$ here. The full-sphere construction and coordinate identification are justified below using the mathematical inputs in F7. [Adamo–Newman](https://arxiv.org/pdf/1410.6626)

## Proof

**Given:** The full comparison hypotheses in the Statement, and the independent inputs specified above.

**Goal:** Establish the entire connected-horizon analytic vacuum classification, the electrovacuum refinement, and the normalized nonrotating mass identity.

1.1 In the comparison exterior, $r>r_+\ge m>0$ gives $\Sigma>0$ and $\Delta>0$, so the displayed global sphere tensor is smooth. On the pole-free region it equals the Boyer–Lindquist metric by the algebraic identity in the sphere supplier, which uses no large-radius bound; the exact coordinate supplier gives Lorentzian signature there. At a pole $\lambda=0$ and $b=0$, so the tensor is $-\Delta\Sigma^{-1}dt^2+\Sigma\Delta^{-1}dr^2+\Sigma\gamma$, also Lorentzian. The advanced-coordinate change $dv=dt+R\Delta^{-1}dr$, $d\psi=d\phi+a\Delta^{-1}dr$ has radial primitives on the whole interval $(r_+,\infty)$, and its angular shift is a smooth rotation of the full sphere. It therefore embeds the whole exterior into the regular ingoing model, with the specified time orientation. Import 5 identifies precisely this full exterior with the source comparison domain. F7's horizon formula makes zero outer surface gravity equivalent to the double root in the rotating range; it includes extremality. [given, F7, algebra]

1.2 In the nonrotating vacuum case, apply Import 2's structure theorem with $s=1$ to the domain $D$ of outer communications. Vacuum implies the null energy condition. End separation applied within globally hyperbolic $D$ excludes another asymptotically flat end in causal communication with the selected end: any such end would itself lie in $D$, contrary to Theorem 2.3. Thus the finite-end compact-core slice can be truncated at a single large end sphere $S_R$ to give a compact smooth spacelike hypersurface $\Sigma_R$ with boundary $S_R-C$, where $C$ is its compact horizon section. The slice is spacelike up to $C$, even for a degenerate horizon; it is not an orthogonal cylindrical-end slice. In the orientations of F2, Import 4 gives $\int_{S_R}\star_g dT^\flat=\int_C\star_g dT^\flat$. Consequently the exterior Komar limit exists and equals this horizon flux. End spheres in Import 2's adapted stationary coordinates are homologous to these spheres within the same stationary vacuum end, so the same closed-form Stokes identity gives their equal flux. That adapted end satisfies Import 4's asymptotic-normal condition for $E_{\rm ADM}=M_K$. [given, A1, F2, F6]

2.1 For a rotating degenerate vacuum horizon, F1 gives an extremal Kerr exterior. Import 1 gives the electrovacuum comparison and global axial symmetry under its exact analytic $I^+$-regular assumptions. Step 1.1 specifies the complete Kerr–Newman comparison object, including its axes and extremal parameter range. Global symmetry is supplied by the comparison input, rather than inferred from the existence of a merely local Killing field. [given, F1, F4, F5, F7, step 1.1]

2.2 Let $\tau$ be Import 2's stationary-flow time coordinate, with sign fixed at the selected end so that $d\tau(T)=1$ and $\tau$ increases to the future. Its spacelike levels extend smoothly to $C$. Let $n$ be their smooth future unit normal from F8. The covector $d\tau$ is timelike and future-increasing in the exterior; its smooth nonzero timelike boundary value therefore has $d\tau(n)>0$ on $C$. Writing $T=Nn+X$ with $X$ tangent to the level slice gives $N=-g(T,n)=1/d\tau(n)>0$, including on $C$. This also proves nonvanishing there. To fix the outward sign, put $P=I^-(M_{\rm ext})$. Import 3 supplies the smooth Killing-horizon structure. Near $p\in C$, this future horizon is $\partial P$, with exterior slice side in $P$. Choose a local defining function $\rho$ from F8 and shrink its hypersurface chart so that its connected side $\rho>0$ lies in $P$ and contains the exterior slice side, and let $s$ be the unit normal to $C$ within the slice pointing toward it; then $d\rho(s)>0$. The null covector $d\rho$ annihilates $T_pC$, so in the orthonormal normal plane $d\rho(n)=\pm d\rho(s)$. The positive sign would make a short coordinate segment starting at $p$ with initial velocity $n$ future timelike and contained in $P$ for positive parameter: its initial derivative of $\rho$ would be positive. Chronological transitivity would then put $p$ in the open past set $P$, contradicting $p\in\partial P$. Thus $d\rho(n)=-d\rho(s)$, and the future null normal to the horizon is $n+s$. Nonrotation puts the nonzero $T$ in this line, and its coefficient is precisely $N>0$. Therefore $T=N(n+s)$ satisfies the positive-coefficient hypothesis of F2, without an added normalization or a bifurcation assumption. [A1, F2, F5, F6, F8, step 1.2, algebra]

3.1 Use the future and outward frame and the positive coefficient established in step 2.2. In a positively oriented orthonormal frame $(n,s,e_1,e_2)$, the defining Hodge convention gives $(\star_g dT^\flat)(e_1,e_2)=(\nabla^aT^b)b_{ab}$ for $b_{ab}=s_an_b-n_as_b$; this fixes the same sign and factor as F2. Its boost invariance permits the specified normalized horizon frame. Hence step 1.2 yields $M_K=Q_C[T]$. The vacuum zeroth law in Import 3 makes $\kappa$ constant, so F2 now gives $M=E_{\rm ADM}=M_K=\kappa A/(4\pi)$. At $\kappa=0$ its conditional zero-mass implication applies with its global-transport hypothesis now established. [A1, F2, F5, F6, step 1.2, step 2.2, algebra]

4.1 A connected nonempty nonrotating degenerate horizon satisfies the all-components condition of Import 2's exclusion. That complete source application therefore rules it out in the exact $I^+$-regular vacuum class. This use retains the source's positive-energy applicability; it does not apply a bare zero-mass rigidity theorem to an unspecified completion. Steps 1.2–3.1 supply the separate mass identity and explain the vanishing mass, without using bifurcation-based staticity. [given, A1, F5, step 1.2, step 3.1]

5.1 In the nondegenerate analytic vacuum case, the Killing-horizon and zeroth-law inputs in Import 3 give constant nonzero surface gravity and thus nonzero mean under the source convention. Import 2's connected mean-nondegenerate comparison gives a Kerr exterior. Together with the rotating degenerate case in step 2.1 and the exclusion in step 4.1, this exhausts the connected-horizon alternatives and proves the entire-domain vacuum conclusion. [given, A1, F4, F5, step 2.1, step 4.1]

6.1 The assertion about no regular bifurcation sphere for the same nonzero degenerate generator is F3. No such sphere entered the transport, exclusion or comparison arguments. The conclusions retain their stated vacuum and electrovacuum hypotheses and field normalizations. [F3, step 2.1, step 3.1, step 4.1, step 5.1] ∎

## Source notes

Original article attribution only: The uniqueness of smooth stationary black holes, arXiv:2611.16853v1, §1.3, PDF p.5. Its rotating and nonrotating degenerate discussion and connected-horizon analytic conclusion are retained. The independent imports supply the prerequisites and argument. Chruściel–Nguyen's maximal-surface caution concerns the separate staticity route; neither that route nor a mixed-horizon exclusion is asserted here.

---
id: post-stationary-end-state-expectation
title: Physical expectation of late-time stationarity
kind: postulate
status: draft
origin: pipeline
domain: physics
deps:
  - def-stationary-lorentzian-data
  - def-causal-exterior-and-boundary-data
  - physics:def-gr-fx-bondi-expansion
  - physics:def-gr-fx-kerr-exterior
  - def-author-310ff0f53b38-asymptotically-flat-spacelike-end
  - def-author-310ff0f53b38-stationary-flow-exterior
  - def-black-hole-comparison-hypothesis-data
  - def-kerr-metric
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:def-gr-fx-bondi-expansion: mathematical-premise
  physics:def-gr-fx-kerr-exterior: mathematical-premise
  def-author-310ff0f53b38-asymptotically-flat-spacelike-end: mathematical-premise
  def-author-310ff0f53b38-stationary-flow-exterior: mathematical-premise
  def-black-hole-comparison-hypothesis-data: mathematical-premise
  def-kerr-metric: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 1, §1.1, opening paragraph
      statement: The authors motivate black-hole uniqueness by the expectation that an
        isolated dynamical black hole approaches a stationary state at late
        times owing to persistent gravitational radiation; they say that the
        uniqueness conjecture, if true, would characterize the possible
        asymptotic states of general vacuum evolution.
      hypotheses: The passage concerns isolated dynamical black holes and the regular
        four-dimensional asymptotically flat stationary vacuum black holes in
        the authors' uniqueness conjecture; it does not specify a convergence
        topology or rate.
      reading_limits: Read the frozen extracted text and visually inspected PDF page
        1. This citation attributes the expectation and motivation; it does not
        establish them or report a measurement.
    - title: P. T. Chruściel and J. L. Costa, On uniqueness of stationary vacuum black
        holes
      url: https://arxiv.org/pdf/0806.0016v2
      locator: Section 2.2, PDF/printed p. 7, equation (2.9) and the black-hole-region
        definition immediately following it.
      statement: For the flow-saturated asymptotic region M_ext, the black hole region
        is B = M \ I^-(M_ext), and its event horizon is the ambient boundary of
        B.
      hypotheses: A time-oriented spacetime with a complete stationary Killing field
        timelike on the selected asymptotically flat spacelike end;
        chronological past is computed in the ambient spacetime.
      reading_limits: Read the PDF text of section 2.2 through these definitions. This
        imports only the end-relative black-hole-region convention, without a
        uniqueness or convergence theorem.
physical_scope: Qualitative late-time behavior of isolated black holes in
  four-dimensional general relativity, with the article's vacuum uniqueness
  motivation. This is an expectation, not an observed outcome or a proved
  general decay law.
dependency_level: 6
---

## Postulate

As physical motivation, expect an isolated dynamical black hole to approach a stationary state at late times through persistent emission of gravitational radiation. If such a limiting state is a regular, four-dimensional, asymptotically flat stationary vacuum black hole and the black-hole uniqueness conjecture holds for that state, its domain of outer communications is isometric to a Kerr exterior. In that conditional sense the conjecture would characterize possible asymptotic states of general vacuum evolution.

Here a stationary state has a smooth Lorentzian metric $g$ and a Killing field $T$, meaning $\mathcal L_Tg=0$, which is future timelike near the designated distant end. Vacuum means $\operatorname{Ric}(g)=0$. For a designated end $U$, the domain of outer communications is $I^+(U)\cap I^-(U)$: the points that can both be reached from and send a future-directed timelike signal to $U$. An isometry is a diffeomorphism that pulls one metric back to the other. Kerr exteriors here are those of the supplied Kerr metric with $M>0$, $|a|\leq M$ and $r>r_+=M+\sqrt{M^2-a^2}$, including the extremal case $|a|=M$; for example, the supplied subextremal family has $M>0$, $|a|<M$ and exterior coordinate range $r>M+\sqrt{M^2-a^2}$. The expectation itself is not restricted to that subfamily.

For a precise instance of the regularity qualification in the conditional claim, take a specified asymptotically flat spacelike end $S_{\rm ext}$: in its end chart, the induced metric $\gamma$ and second fundamental form $k$ satisfy $\gamma_{ij}-\delta_{ij}=O_m(r^{-\alpha})$ and $k_{ij}=O_{m-1}(r^{-1-\alpha})$ for some $\alpha>0$ and integer $m\ge2$, with the derivative-decay convention of the supplied end interface. Require $T$ to be complete and future timelike on a sufficiently distant tail, and let $U=\bigcup_{t\in\mathbb R}\Phi_t(S_{\rm ext})$ be the flow saturation of that tail. All chronological sets are computed in the ambient spacetime $\mathcal M$. The black-hole region relative to this end is $\mathcal B=\mathcal M\setminus I^-_{\mathcal M}(U)$, required to be nonempty; its event horizon is $\partial_{\mathcal M}\mathcal B$. In this precise instance, regularity means the supplied Chruściel–Costa $I^+$-regularity predicate: completeness of $T$, global hyperbolicity of the domain of outer communications, and the specified acausal spacelike section with finite ends and a boundary meeting each future exterior-boundary generator once. This is a particular mathematical formulation of regularity, not an identification with every use of the word regular in the article's qualitative motivation.

The conditional uniqueness assumption for this formulation is explicit: every smooth four-dimensional stationary vacuum spacetime with the preceding end, nonempty black-hole region and $I^+$-regularity has its domain of outer communications isometric to a Kerr exterior with $M>0$ and $|a|\leq M$. This implication is assumed here, not established. Its application to a limiting state requires that state to satisfy all these hypotheses. The general late-time expectation itself is not restricted to this particular regularity formulation.

For an end admitting the separately hypothesized smooth vacuum Bondi expansion, $u$ is retarded time, $C_{AB}$ is the Bondi shear and $N_{AB}=\partial_u C_{AB}$ is the Bondi news, a standard asymptotic radiation datum. The expectation does not assert that every evolution has such an expansion or specify a condition on $N_{AB}$.

## Postulate references

[[def-stationary-lorentzian-data]]

[[def-causal-exterior-and-boundary-data]]

[[physics:def-gr-fx-bondi-expansion]]

[[physics:def-gr-fx-kerr-exterior]]

[[def-author-310ff0f53b38-asymptotically-flat-spacelike-end]]

[[def-author-310ff0f53b38-stationary-flow-exterior]]

[[def-black-hole-comparison-hypothesis-data]]

[[def-kerr-metric]]

## Scope and attribution

The source gives a qualitative expectation and a conditional motivation, not a precise class of initial data, a convergence topology, a decay rate, or a proof that radiation produces stationarity. The phrase persistent emission is retained as the source's physical motivation; no quantitative flux law or assertion of nonzero radiation at every finite time is imposed here. The uniqueness conjecture and the applicability of its regularity hypotheses to a proposed limit are separate conditions. No measurement or empirical confirmation is claimed.

## External input

The black-hole-region and event-horizon convention above is the definition immediately after equation (2.9) in Chruściel–Costa section 2.2, PDF page 7. It supplies terminology only; the uniqueness implication remains an explicit assumption and the late-time expectation remains a postulate.

---
id: thm-nondegenerate-bifurcate-extension-input
title: Nonzero constant surface gravity and global bifurcate extension
kind: theorem
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-author-4cb89398a4ab-racz-wald-collapse-class
  - def-bifurcate-killing-horizon-data
dependency_roles:
  def-author-4cb89398a4ab-racz-wald-collapse-class: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
provenance:
  statement: ai-altered
  proof: literature-derived
sources:
  references:
    - title: Rácz–Wald, Global Extensions of Spacetimes Describing Asymptotic Final
        States of Black Holes
      url: https://arxiv.org/pdf/gr-qc/9507055
      locator: End of §2, printed/PDF pp. 8–9; Theorem 4.2, pp. 15–16; §5 opening
        paragraph, p. 17
      statement: For the exact end-of-§2 class stated here and nonzero constant
        surface gravity on N, the whole original spacetime admits an isometric
        extension in which N is a proper subset of a bifurcate Killing horizon;
        the original horizon-generating action extends and the extension can
        have a wedge-reflection isometry about the bifurcation surface.
      hypotheses: Smooth globally hyperbolic spacetime; smooth spacelike Cauchy
        surface with the single asymptotically stationary end of Chruściel–Wald
        Definition 2.1; nonempty black-hole region and empty white-hole region
        relative to its complete stationary action; connected Killing event
        horizon with compact intersection with the Cauchy surface; a globally
        defined one-parameter isometry group with horizon-normal generator,
        future directed there; nonzero constant surface gravity. No field
        equation is assumed.
      reading_limits: Read the independent PDF end-of-§2 class, Theorem 4.2 and its
        displayed construction, and §5 opening scope restriction; visually
        checked PDF pp. 8 and 15. The orbit-space lemmas and complete extension
        proof were not independently reconstructed or reviewed. The extension of
        additional tensor fields, vacuum equations, global hyperbolicity of the
        extension, and extension of the distinct stationary action are not
        claimed by this import.
external_input: true
dependency_level: 6
---

## Statement

Let $(M,g,\Sigma,T,\phi,\xi,\chi,N)$ satisfy the complete Rácz–Wald collapse-class contract [[def-author-4cb89398a4ab-racz-wald-collapse-class]], including the exact single-end asymptotic conditions, global hyperbolicity, absence of a white hole and both specified complete actions. Suppose the signed surface gravity of the future horizon-normal generator $\xi$ is a nonzero constant on $N$, with the conventions of [[def-bifurcate-killing-horizon-data]].

Then there is a smooth spacetime $(M^*,g^*)$ and an isometric embedding of the **whole** $(M,g)$ into it such that the image of $N$ is a proper subset of a bifurcate Killing horizon. The original group $\chi_u$ extends to $(M^*,g^*)$, and the extension can be chosen with a wedge-reflection isometry about its bifurcation surface. In the local horizon coordinates this reflection sends $(U,V,x^1,x^2)$ to $(-U,-V,x^1,x^2)$.

This is a global embedding conclusion, not a claim that $M^*$ is globally hyperbolic. Extension of additional tensor fields is a separate question, as stated at the start of §5 of the source. No Einstein equation or matter-field extension is asserted. The completeness and horizon-normal property of $\xi$ are hypotheses even if $\xi\ne T$.

## Facts & Assumptions

[F1] The collapse-class definition records every end-of-§2 hypothesis and its supporting end and causal chain. [[def-author-4cb89398a4ab-racz-wald-collapse-class]]

[F2] The signed scalar belongs to the specified horizon-normal Killing field; nonzero constant surface gravity is an additional hypothesis. [[def-bifurcate-killing-horizon-data]]

[F3] Rácz–Wald Theorem 4.2 is the imported global-extension input under precisely these hypotheses.

## External input

Apply Rácz–Wald Theorem 4.2 to [F1] and the nonzero-constant hypothesis [F2]. It supplies the isometric extension of the whole spacetime, the proper-subset bifurcate horizon, the extended group $\chi_u$, and wedge reflection. The source construction identifies the reflection as $(U,V)\mapsto(-U,-V)$. This is an external theorem input, not a locally reconstructed proof. Its §5 separates the further problem of extending invariant tensor fields; no tensor extension follows from this item alone.

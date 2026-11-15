---
id: thm-stationary-harrison-primitive-input
title: Smooth invariant Harrison primitive near the horizon and at infinity
kind: theorem
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - def-complex-self-dual-two-form-data
  - def-stationary-asymptotic-decay-data
  - def-circle-action-and-invariant-normal-data
  - math:thm-stokes-theorem-for-smooth-singular-chains
  - lem-author-9e1b6fa65528-relative-normal-homotopy
  - lem-author-9e1b6fa65528-equivariant-cartan-normalization
  - lem-author-9e1b6fa65528-radial-exterior-primitive
  - lem-author-9e1b6fa65528-stationary-spatial-lifting
  - lem-author-9e1b6fa65528-stationary-exact-gluing
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-circle-action-and-invariant-normal-data: mathematical-premise
  math:thm-stokes-theorem-for-smooth-singular-chains: mathematical-premise
  lem-author-9e1b6fa65528-relative-normal-homotopy: mathematical-premise
  lem-author-9e1b6fa65528-equivariant-cartan-normalization: mathematical-premise
  lem-author-9e1b6fa65528-radial-exterior-primitive: mathematical-premise
  lem-author-9e1b6fa65528-stationary-spatial-lifting: mathematical-premise
  lem-author-9e1b6fa65528-stationary-exact-gluing: mathematical-premise
provenance:
  statement: ai-altered
  proof: literature-derived
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1#A1.SS1
      locator: §1.1 GR/SBS and maximality; Lemma 2.1; §3.1 (3.2) and the following
        global-existence and extension paragraph; §3.2 (3.9), (3.13)–(3.15);
        Appendix A.1 (A.2)–(A.11), PDF pp. 29–30; Appendix A.3 Lemma A.1 at q=1
      statement: Under Radu's GR, SBS and original maximal-slice assumptions with mass
        one, the real two-form $\Theta_0=4((f-1)F+\psi\star F)$,
        $F=\tfrac12dT^\flat$, $\sigma=f+i\psi$, $f=-g(T,T)$, with $\psi$ the
        smooth twist potential satisfying $d\psi=2i_T\star F$ and $\psi\to0$ as
        $r\to\infty$ on the exterior and extending smoothly across the
        bifurcation sphere, is closed and $i_T\Theta_0=dD_0$,
        $D_0=|1-\sigma|^2$. There is a stationary smooth primitive $W_0$ on the
        exterior and a neighborhood of its bifurcation sphere. Near the sphere
        it is invariant under the local commuting fields $K=T+\Omega_HZ$ and
        $Z$; at a common zero $p$ of $T,Z$ it satisfies $W_0(T)+D_0=D_0(p)$. On
        the end its spatial components are $-\int_1^\infty
        sx^j(\Theta_0)_{ji}(sx)\,ds=O_5(r^{-3})$. The exact stationary cutoff
        corrections retain the local homotopy gauge and radial gauge
        simultaneously. The original q=1 collar is available without first
        constructing $W_0$.
      hypotheses: "Smooth four-dimensional stationary vacuum spacetime in Radu §1.1
        GR/SBS: specified asymptotically flat end with (1.1) differentiated
        through order six; globally hyperbolic exterior; complete nowhere-zero
        stationary field whose exterior orbits meet the specified spacelike
        slice transversely; slice diffeomorphic to the outside of a ball, with
        smooth transverse nonexpanding horizon branches meeting at a sphere,
        stationary field tangent to them and not identically zero on the sphere;
        original slice maximal and smooth to its boundary; mass rescaled to one.
        Local fields normalized as in (3.9), with common pole p. No small ADM
        angular momentum is needed for this construction."
      reading_limits: "Fresh reading: arXiv:2610.09729v1 HTML, §1.1 GR/SBS and
        maximality, Lemma 2.1, §3.2–3.3, Appendix A.1 and the original q=1
        specialization of Appendix A.3; PDF pp. 28–30 text and p. 29 rendered
        formulas inspected. Other cited papers were not freshly read. These are
        source-statement/application readings, not independent proof review.
        Adjudication update: freshly consulted the HTML v1 §3.1 definition (3.2)
        and the immediately following global-existence and tubular-neighborhood
        extension paragraph, with §1.1 GR/SBS and maximality, Lemma 2.1 and §3.2
        for applicability. The earlier reported PDF and other passage readings
        are retained history, not new reading credit for this repair; no PDF was
        freshly inspected. No source proof audit is claimed."
external_input: true
dependency_level: 2
---

## Statement

In the mass-one stationary vacuum construction under the precise Radu GR/SBS and original maximal-slice hypotheses in [F1], define $F=\tfrac12dT^\flat$, $f=-g(T,T)$, $\sigma=f+i\psi$, where $\psi$ is the smooth twist potential on the exterior and a neighborhood of the bifurcation sphere satisfying $d\psi=2i_T\star F$ and $\psi\to0$ as $r\to\infty$, and put $\Theta_0=4((f-1)F+\psi\star F)$ and $D_0=|1-\sigma|^2$. The symbol $\star$ denotes the oriented Lorentzian Hodge star and $T^\flat=g(T,\cdot)$. There exists a smooth stationary real one-form $W_0$ on the exterior and a neighborhood of the bifurcation sphere $S$, with $dW_0=\Theta_0$, locally invariant under the Hawking field $K$ and rotational field $Z$, and satisfying $W_0(T)+D_0=D_0(p)$ at a common zero $p$ of $T,Z$. Here $K=T+\Omega_HZ$, $K|_S=0$ and $Z$ has period $2\pi$. In the fixed stationary end chart, $W_0=(D_0(p)-D_0)dt+(W_0)_i dx^i$ and $(W_0)_i(x)=-\int_1^\infty sx^j(\Theta_0)_{ji}(sx)\,ds=O_5(r^{-3})$. One primitive has both this end gauge and the smooth invariant homotopy gauge near $S$. The local Hawking-field invariance is asserted only where the local field is defined.

## Facts & Assumptions

[F1] Import the exact construction and hypotheses of the sole statement-bearing Radu citation below. In particular, §3.1 (3.2) specifies $d\psi=2i_T\star F$ and $\psi\to0$ as $r\to\infty$; its following paragraph supplies the global smooth potential on $E$ and its smooth extension across the bifurcation sphere. This includes the stationary product $E\simeq\mathbb R\times\Sigma_1$, $\Sigma_1\simeq(1,\infty)\times\mathbb S^2$, the zero-period criterion for exact two-forms, vanishing first cohomology of the end and collar, and the original $q=1$ stationary collar. These are external inputs, not consequences of the definition of a bifurcate Killing horizon.

[F2] Differential forms, stationary fields, bifurcate horizons, self-dual/Hodge conventions, differentiated decay and periodic actions use the declared geometric definitions. [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]] [[def-complex-self-dual-two-form-data]] [[def-stationary-asymptotic-decay-data]] [[def-circle-action-and-invariant-normal-data]]

[F3] Stokes' theorem transfers periods across the compact annulus between homologous spheres. [[math:thm-stokes-theorem-for-smooth-singular-chains]]

[F4] The five local intermediate constructions below give the normal homotopy, equivariance and forced normalization, radial finite-order estimate, stationary lifting and exact gauge gluing under their explicit hypotheses. [[lem-author-9e1b6fa65528-relative-normal-homotopy]] [[lem-author-9e1b6fa65528-equivariant-cartan-normalization]] [[lem-author-9e1b6fa65528-radial-exterior-primitive]] [[lem-author-9e1b6fa65528-stationary-spatial-lifting]] [[lem-author-9e1b6fa65528-stationary-exact-gluing]]

## External input

The smooth Radu construction in [F1] is imported as an established external input with the complete source statement and hypotheses above. Its spatial decay makes the period on $S_r$ tend to zero: the coefficients are $O(r^{-4})$ and the area scales as $r^2$. Closedness and [F3] therefore give zero period on $S$ and on a generator sphere. The source's cohomology criteria provide the base primitive $\beta$ on $S$ and a global spatial primitive. The first two intermediate lemmas then explain the smooth invariant normal-bundle construction and the forced constant at $p$; the fourth lifts the spatial primitive with exactly this constant. The third proves the radial formula and its five derivative bounds. The fifth explains why exact corrections on the end and the original stationary collar preserve the normalization and leave the Hawking symmetry intact near $S$. No global extension of $K$ or $Z$ is required.

## Source notes

The five intermediate lemmas were fully authored before admitting the residual source inputs. This item retains literature-derived proof provenance and is not a claim that all of Radu's geometric or asymptotic analysis has been reconstructed locally. In particular, the radial lemma proves $C^5$ regularity from the recorded $O_5$ bound; smoothness of the chosen radial end form is included in the imported smooth construction, not inferred solely from five derivative bounds. The collar input is the original $q=1$ collar, avoiding dependence on the Harrison electrovacuum construction. Radu's §3.3 derivation of (3.28) uses the original vacuum end and does not require transformed charge formulas. The separate held vacuum Ernst, local rigidity and Harrison electrovacuum items are not logical suppliers here; their applicable inputs are expressly imported from the independently read source. Source reading does not grant Step-7 judgment or establish a defect in the article under study.

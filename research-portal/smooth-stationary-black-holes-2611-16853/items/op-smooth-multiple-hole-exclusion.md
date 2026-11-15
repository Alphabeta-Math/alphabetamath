---
id: op-smooth-multiple-hole-exclusion
title: Smooth stationary multiple-black-hole nonexistence
kind: open-problem
status: published
origin: pipeline
domain: physics
deps:
  - def-stationary-lorentzian-data
  - def-black-hole-comparison-hypothesis-data
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-black-hole-comparison-hypothesis-data: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
physical_scope: Classical four-dimensional general relativity, with the vacuum
  Einstein equation and the stated global regularity and asymptotic conditions
  treated as model assumptions.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 5, §1.3, last two paragraphs
      statement: The article asks whether multiple black holes can exist in a
        stationary asymptotically flat I-plus-regular smooth vacuum spacetime.
        It reports their exclusion in the analytic vacuum case and cites Wong–Yu
        for a smooth conditional exclusion and for removal of the
        connected-horizon assumption in the perturbative result of its reference
        [2].
      hypotheses: The question concerns smooth stationary asymptotically flat
        I-plus-regular vacuum spacetimes; the reported analytic and perturbative
        results have their own additional hypotheses.
      reading_limits: Read the frozen article text at the cited passage. This
        reference attributes the question and the article's comparison claims;
        it is not a proof of either exclusion.
    - title: Non-existence of multiple-black-hole solutions close to Kerr-Newman
      url: https://arxiv.org/pdf/1210.1379v4
      locator: Abstract, §1.2 and §2.2, Main Theorem
      statement: Under the paper's geometric assumptions and quantitative smallness
        condition, a stationary asymptotically flat electrovacuum solution has
        at most one event-horizon component, without assuming axial symmetry.
        The paper also describes removal of the single-horizon assumption from
        the perturbative uniqueness theorem of Alexakis, Ionescu and Klainerman.
      hypotheses: The source's specified nondegenerate bifurcate horizon, asymptotic
        and geometric assumptions, together with its Kerr–Newman
        characterization-tensor smallness condition. These are additional
        restrictions, not consequences of the open problem's hypotheses.
      reading_limits: Read the abstract, introduction, and nearby definitions in the
        online PDF; the proof was not reviewed. The present item records the
        partial result as source-reported context and does not import it as a
        logical premise.
dependency_level: 5
---

## Open problem

Can there be stationary Lorentzian data $(M,g,N,T)$ with a specified asymptotically flat spacelike end, satisfying $\operatorname{Ric}(g)=0$ and $I^+$-regularity relative to that end, whose future event horizon has more than one connected component?

Here stationary Lorentzian data mean the smooth time-oriented Lorentzian four-manifold and Killing field of [[def-stationary-lorentzian-data]]; the vacuum equation says that its Ricci tensor vanishes. Use the asymptotically flat end and $I^+$-regularity conditions of [[def-black-hole-comparison-hypothesis-data]]. In particular, the latter specifies the complete stationary flow, globally hyperbolic exterior and an appropriate acausal spacelike section. The future event horizon is the set $\mathcal E^+=\partial_M D\cap I_M^+(M_{\rm ext})$ in that definition, where $M_{\rm ext}$ is the flow saturation of the chosen end and $D=I_M^+(M_{\rm ext})\cap I_M^-(M_{\rm ext})$. Multiple black holes means more than one connected component of this horizon. Neither analyticity nor a Killing-horizon generator, bifurcation surface, or nondegeneracy is assumed in the question.

## Open problem references

[[def-stationary-lorentzian-data]]

[[def-black-hole-comparison-hypothesis-data]]

## Status

The article poses this as an open question in §1.3, dated 12 November 2026. It reports exclusion in the analytic vacuum setting. As a restricted smooth partial result, Wong and Yu report at most one horizon component under their additional geometric and quantitative near–Kerr–Newman assumptions, in electrovacuum and without assumed axial symmetry. Their introduction also states that the single-horizon assumption in the perturbative theorem of Alexakis, Ionescu and Klainerman can thereby be removed. These reports do not resolve the unrestricted smooth question stated above. No later status survey or independent proof review is claimed.

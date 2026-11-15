---
id: def-author-310ff0f53b38-null-generator-cross-section
title: Null generators and once-only cross-sections
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-metric-selected-connection
  - physics:def-gr-causal-curves-and-reachability
  - math:def-covariant-derivative-along-a-curve
  - math:def-geodesic-of-an-affine-connection
  - math:prop-coordinate-geodesic-equation
  - def-author-310ff0f53b38-asymptotically-flat-spacelike-end
  - def-author-310ff0f53b38-stationary-flow-exterior
  - math:def-countable-choice
  - math:def-dependent-choice
  - physics:lem-gr-chronology-openness
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  math:def-covariant-derivative-along-a-curve: mathematical-premise
  math:def-geodesic-of-an-affine-connection: mathematical-premise
  math:prop-coordinate-geodesic-equation: mathematical-premise
  def-author-310ff0f53b38-asymptotically-flat-spacelike-end: mathematical-premise
  def-author-310ff0f53b38-stationary-flow-exterior: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-dependent-choice: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: P. T. Chruściel and J. L. Costa, On uniqueness of stationary vacuum black
        holes (2008), author manuscript
      url: https://homepage.univie.ac.at/piotr.chrusciel/papers/bourguignon/ChruscielCostaIII.pdf
      locator: §2.2, (2.9)–(2.10) and footnote 4, p. 7; §4.1, opening paragraph before
        Proposition 4.1, p. 13 (PDF pages 7 and 13).
      statement: For the stationary exterior M_ext, every point of
        H-plus=boundary(I-minus(M_ext)) starts a future-inextendible null
        geodesic ray in H-plus; continuing it backwards can leave H-plus.
      hypotheses: Smooth time-oriented stationary spacetime with a complete Killing
        flow future timelike on the selected asymptotically flat end and
        uniformly timelike at large radius as in §2.2 footnote 4; M_ext is its
        flow saturation. This is the causal-boundary assertion, not a
        vacuum-field-equation consequence.
      reading_limits: Read extracted text of §2.2 including footnotes and the opening
        §4.1 paragraph in the linked author manuscript, and corresponding
        passages on printed pp. 201–202 and 208–209 of the published Numdam PDF.
        No underlying causality proof was reconstructed; PDF screenshots were
        unavailable. No uniqueness, smooth-horizon or affine-completeness
        theorem is imported.
dependency_level: 2
---

## Definition

Assume Countable Choice for the general construction, as required by the supplied smooth tangent-bundle and vector-field interfaces. Let $H\subset M$ be a specified horizon subset of a time-oriented smooth Lorentzian four-manifold $(M,g,N)$. An affinely parametrized null geodesic is a smooth curve $c:I\to M$, where $I\subseteq\mathbb R$ is an interval with nonempty interior, with nonzero future-directed tangent, $g(\dot c,\dot c)=0$ and $D_s\dot c=0$. Here $D_s$ is the covariant derivative along $c$ induced by the Levi–Civita connection $\nabla^g$; the notation $\nabla^g_{\dot c}\dot c$ means this derivative along the curve, without requiring an ambient extension of $\dot c$. In chart coordinates $c^a=x^a\circ c$, the equivalent equation is $\ddot c^a+\Gamma^a{}_{bc}(c)\dot c^b\dot c^c=0$. At an included endpoint, smoothness and these derivatives have the one-sided interpretation.

A generator of $H$ means the image of such a null geodesic maximally continued while remaining in $H$; two affine parametrizations with the same image describe the same generator. A finite endpoint belonging to $H$ may be included, with the preceding endpoint convention. Maximal continuation here is relative to $H$, and is not a claim of affine geodesic completeness in $M$.

For the family $\mathcal G(H)$ of these generator images, a once-only cross-section is a subset $B\subset H$ such that $B\cap G$ has exactly one point for every $G\in\mathcal G(H)$. This counts points, not affine parameter values. It imposes neither smoothness nor a normalization of tangent fields. Coverage of an arbitrary $H$ by generators, future inextendibility, and regularity of a particular horizon are separate geometric assertions; they are not proved merely by this terminology.

For the stationary application, take an asymptotically flat spacelike end $S_{\rm ext}$ and a complete Killing field $T$ future timelike on that end, and use its flow saturation $M_{\rm ext}$ and chronological exterior $D=I_M^+(M_{\rm ext})\cap I_M^-(M_{\rm ext})$. In this causal-boundary application assume also Dependent Choice, as in the chronology-openness supplier. Define the full future event horizon by $H^+=\partial_M I_M^-(M_{\rm ext})$ and its portion by $\mathcal E^+=\partial_M D\cap I_M^+(M_{\rm ext})$. Then $\mathcal E^+=H^+\cap I_M^+(M_{\rm ext})$. For the cited causal-boundary assertion use also the source's asymptotic convention: $g(T,T)\le-\epsilon<0$ for some $\epsilon>0$ at sufficiently large radius on $S_{\rm ext}$. This uniformity is not needed for the portion identity. The cited input then provides, from each point of $H^+$, a future-inextendible null geodesic ray staying in $H^+$; its past continuation can exit $H^+$. Inextendibility here means absence of a future endpoint in $M$, not infinite affine parameter length. For a portion $\mathcal E^+\subset H^+$, use the maximal connected pieces of the horizon generator curves lying in that portion, and then their images. The once-only condition uses those images; it does not assert existence of a section.

## Definition references

[[physics:def-gr-smooth-lorentzian-objects]]

[[physics:def-gr-metric-selected-connection]]

[[physics:def-gr-causal-curves-and-reachability]]

[[math:def-covariant-derivative-along-a-curve]]

[[math:def-geodesic-of-an-affine-connection]]

[[math:prop-coordinate-geodesic-equation]]

[[def-author-310ff0f53b38-asymptotically-flat-spacelike-end]]

[[def-author-310ff0f53b38-stationary-flow-exterior]]

[[math:def-countable-choice]]

[[math:def-dependent-choice]]

[[physics:lem-gr-chronology-openness]]

## Facts & Assumptions

[F1] Causal character, future direction and endpoint-based causal inextendibility use the Lorentzian and causal-curve conventions. Countable Choice is assumed for the smooth tangent-bundle and vector-field constructions in the Lorentzian and metric-selected-connection interfaces. [[physics:def-gr-smooth-lorentzian-objects]] [[physics:def-gr-causal-curves-and-reachability]] [[physics:def-gr-metric-selected-connection]] [[math:def-countable-choice]]

[F2] The metric-selected connection induces the derivative along a curve; its geodesic condition, equivalent coordinate equation and one-sided endpoint interpretation are the supplied mathematical interfaces. [[physics:def-gr-metric-selected-connection]] [[math:def-covariant-derivative-along-a-curve]] [[math:def-geodesic-of-an-affine-connection]] [[math:prop-coordinate-geodesic-equation]]

[F3] The end data and complete stationary flow specify $S_{\rm ext}$, $M_{\rm ext}$, $D$ and $\mathcal E^+$. [[def-author-310ff0f53b38-asymptotically-flat-spacelike-end]] [[def-author-310ff0f53b38-stationary-flow-exterior]]

[F4] Under Countable Choice and Dependent Choice, each $I_M^+(p)$ is open; hence $I_M^+(M_{\rm ext})$, its union over $p\in M_{\rm ext}$, is open. [[math:def-countable-choice]] [[math:def-dependent-choice]] [[physics:lem-gr-chronology-openness]]

[F5] The stationary event-horizon ray assertion is the imported premise specified in External input and the source record.

## Justification

**Given:** The objects and data of the Definition, with Countable Choice for the general construction and Dependent Choice for its stationary application.

**Goal:** Verify the curve and cross-section predicates and the horizon-portion identity, distinguishing the imported ray assertion.

1.1 Under Countable Choice, the supplied Lorentzian and metric-selected-connection interfaces apply to the general construction. By the along-curve derivative interface, $D_s\dot c$ is intrinsic, including at one-sided endpoints. Applying the coordinate-geodesic proposition to $\nabla^g$ gives exactly the displayed equation. The additional null and future predicates exclude constant curves. Maximal continuation within $H$ specifies the absence of a larger connected geodesic extension in $H$; defining this predicate asserts no existence. [F1, F2]

1.2 In the stationary application put $U=I_M^+(M_{\rm ext})$ and $P=I_M^-(M_{\rm ext})$, so $D=U\cap P$. For any $p\in U$, openness supplies a neighborhood $V\subset U$; on $V$ the sets $D$ and $P$ agree. Consequently $p\in\partial_M D$ if and only if $p\in\partial_M P$. Intersecting with $U$ gives $\mathcal E^+=H^+\cap U$, defining the required relationship without identifying the full horizon with its portion. [F3, F4]

2.1 Passing to images removes parametrization from the once-only condition: it is precisely $|B\cap G|=1$ for each specified generator image. Included endpoints are points of the image, so require no special multiplicity convention. No smooth horizon tangent bundle or existence of a section is needed to formulate this predicate. [F1, F2, step 1.1]

3.1 With the stated uniform timelikeness convention, the exterior data match the imported stationary causal-boundary premise, so its future rays are available on $H^+$. Restricting each such generator curve to maximal connected parameter pieces in $\mathcal E^+$ defines the portion convention; step 2.1 then supplies its once-only intersection predicate. The future-ray assertion is imported, not established by the terminology or by this local justification, and implies no affine completeness or smoothness of the horizon. [F1, F3, F5, step 2.1, step 1.2] ∎

## External input

The ray assertion [F5] is imported from Chruściel–Costa §4.1, opening paragraph; the exterior construction is §2.2. Its precise statement, hypotheses, locator and reading limits are in the source record. This local justification only applies that premise and verifies the definitions and the portion identity.

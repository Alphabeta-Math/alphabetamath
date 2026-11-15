---
title: The IK continuation also fixes one global reciprocal invariant
status: published
research_item: pthm-author-d20d145f998f-global-reciprocal-invariant
dependency_level: 5
sources:
  references:
    - title: A. D. Ionescu and S. Klainerman, On the uniqueness of smooth, stationary
        black holes in vacuum
      url: https://arxiv.org/pdf/0711.0040v2
      locator: Section 1.2, AF and (1.5), printed/PDF pp. 6–7; Section 4.2 (4.17), p.
        22, Section 4.3 (4.29), p. 24, and Section 4.4 (4.33), p. 25; Section 7
        (7.1)–(7.3), p. 35, Lemma 7.1 (7.17)–(7.18), p. 37; Section 8 (8.1),
        Lemma 8.1 and its proof, p. 41; Section 8.2 completion, pp. 48–49.
      statement: AF assumes every exterior stationary orbit is complete and meets the
        section. Under full AF/SBS/T, the completion proves nonvanishing of
        1−sigma and Mars–Simon vanishing on the section. On a connected zero
        region, (7.2) fixes the Killing scalar and Lemma 7.1 makes
        B=z²+4M²(y²+z²)g⁻¹(dz,dz) constant with z²≤B. Lemma 8.1 gives 0≤B<1/4
        and the stated horizon value of y.
      hypotheses: Every AF/SBS/T hypothesis, positive AF mass, normalized Ernst
        potential, Killing field, curvature and orientation convention is
        retained. The Section 7 computation is used only where 1−sigma is
        nonzero, the Mars–Simon tensor vanishes, and the sphere-normalized
        Killing-scalar identity (7.2) holds.
      reading_limits: Consulted the extracted PDF text at the listed hypothesis,
        definition, identity, lemma and completion passages in
        arXiv:0711.0040v2. The analytic continuation and local invariant
        identity are imported under their full hypotheses; no page-image
        inspection, Carleman proof reconstruction or independent source-proof
        audit is claimed. Stationarity, section-to-exterior transport and scalar
        gluing are the local argument below.
---

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [pthm-ik-local-kerr-criterion-input](item-pthm-ik-local-kerr-criterion-input)
- [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)
- [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af)
- [lem-author-d20d145f998f-zero-mars-simon-gauge](item-lem-author-d20d145f998f-zero-mars-simon-gauge)
- [lem-author-cea8e61dc3c6-killing-flow-invariance](item-lem-author-cea8e61dc3c6-killing-flow-invariance)
- [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)
- [physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)
- [lem-author-9f9c6144aed8-stationary-zero-transport](item-lem-author-9f9c6144aed8-stationary-zero-transport)
- [def-author-9f9c6144aed8-ik-sbs](item-def-author-9f9c6144aed8-ik-sbs)
- [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)
- [math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains](https://alphabetamath.cc/item/prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [` A. D. Ionescu and S. Klainerman, On the uniqueness of smooth, stationary black holes in vacuum · Section 1.2, AF and (1.5), printed/PDF pp. 6–7; Section 4.2 (4.17), p. 22, Section 4.3 (4.29), p. 24, and Section 4.4 (4.33), p. 25; Section 7 (7.1)–(7.3), p. 35, Lemma 7.1 (7.17)–(7.18), p. 37; Section 8 (8.1), Lemma 8.1 and its proof, p. 41; Section 8.2 completion, pp. 48–49. `](https://arxiv.org/pdf/0711.0040v2)


## Statement

In the full IK AF/SBS/T setting, with the same Killing field, mass $M>0$, curvature and orientation conventions, the source continuation gives $1-\sigma\ne0$ and $\mathcal S=0$ throughout the connected exterior. With $y+iz=(1-\sigma)^{-1}$, the scalar $B=z^2+4M^2(y^2+z^2)|Dz|_g^2$ is a single constant there, and $0\le B<1/4$. On the bifurcation sphere the source also gives $y=y_S=(1+\sqrt{1-4B})/2$ and $z^2\le B$. This is a scalar/tensor conclusion, not a global metric isometry. For application to the actual regular article model, assume a demonstrated match of its actual spacetime, stationary field, end and section to every hypothesis of the exact IK AF/SBS/T interface. This includes the source-compatible product end and metric-component decay with mass $M>0$, the specified embedded spacelike section agreeing with $t=0$ on that end, complete stationary orbits meeting the section, and $|g(T,T_0)|>0$ on its exterior part, where $T_0$ is its future unit normal. It also includes the exact rotating smooth non-expanding transverse bifurcate-sphere package, and the same supplied Ernst potential normalized to $1$ along the specified section's end, with $-4M^2\mathcal F^2=(1-\sigma)^4$ on the entire bifurcation sphere and $\operatorname{Re}(1/(1-\sigma))>1/2$ at some point of that sphere. All smoothness, manifold, vacuum, curvature and orientation hypotheses of the interface remain in force. Positive lapse and mass alone do not establish this match; it is an explicit additional hypothesis for the article-model application. Source scope: this conditional supplier does not establish the original article's Theorem 1.1 from its original assumptions; that original claim remains unresolved here.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[pthm-ik-local-kerr-criterion-input](item-pthm-ik-local-kerr-criterion-input)

[def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)

[def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af)

[lem-author-d20d145f998f-zero-mars-simon-gauge](item-lem-author-d20d145f998f-zero-mars-simon-gauge)

[lem-author-cea8e61dc3c6-killing-flow-invariance](item-lem-author-cea8e61dc3c6-killing-flow-invariance)

[math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)

[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[lem-author-9f9c6144aed8-stationary-zero-transport](item-lem-author-9f9c6144aed8-stationary-zero-transport)

[def-author-9f9c6144aed8-ik-sbs](item-def-author-9f9c6144aed8-ik-sbs)

[math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)

[math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains](https://alphabetamath.cc/item/prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

## Facts & Assumptions

[F1] Assume the conditional vacuum model and every hypothesis of the exact IK AF/SBS/T criterion interface, using the same actual end, section, stationary field and supplied normalized Ernst potential throughout. For the article-model application, the complete match stated above is an additional hypothesis, not a conclusion from positive lapse and mass. A source-compatible chart must be supplied or constructed; no equality of independently given coordinate maps is assumed. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [pthm-ik-local-kerr-criterion-input](item-pthm-ik-local-kerr-criterion-input) [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon) [def-author-9f9c6144aed8-ik-sbs](item-def-author-9f9c6144aed8-ik-sbs)

[F2] The exact IK AF package assumes that every stationary orbit in the exterior is complete and meets the section. This is the orbit hypothesis of source 0, Section 1.2, immediately before (1.5). [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af)

[F3] Source 0 supplies the Section 8.2 completion of (8.1), the initial sphere neighborhood, the Section 7 Killing-scalar identity and local constant-$B$ identity, and Lemma 8.1 with its horizon bound, all under the full IK hypotheses.

[F4] The Killing-flow lemma supplies $\mathcal L_TF=0$ and $\mathcal L_T\mathcal F=0$. On common local flow domains, a smooth real tensor is invariant under the flow exactly when its Lie derivative vanishes; apply this criterion separately to the real and imaginary parts of a complex tensor. The metric-selected connection is uniquely torsion-free and metric-compatible on a smooth nondegenerate four-dimensional metric; use its uniqueness clause to transport curvature. The ambient ZFC convention includes its countable-choice assumption. [lem-author-cea8e61dc3c6-killing-flow-invariance](item-lem-author-cea8e61dc3c6-killing-flow-invariance) [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes) [physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[F5] Invariant tensor vanishing transports from the section once its domain and invariance conditions hold. The gauge lemma supplies the same normalized scalars and the spacetime inverse-metric definition of $B$. [lem-author-9f9c6144aed8-stationary-zero-transport](item-lem-author-9f9c6144aed8-stationary-zero-transport) [lem-author-d20d145f998f-zero-mars-simon-gauge](item-lem-author-d20d145f998f-zero-mars-simon-gauge)

[F6] A smooth vector field has a smooth maximal flow on an open domain; its time maps are diffeomorphisms between open domains, inverse to the negative-time maps. AF completeness puts every pair in $\mathbb R\times E$ in this ambient flow domain, without yet asserting preservation of $E$. [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows) [math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains](https://alphabetamath.cc/item/prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains) [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af)

[F7] Chronological reachability uses future timelike, locally absolutely continuous curves in the ambient manifold. Smooth composition preserves local absolute continuity and transforms velocity by the differential; finite concatenation preserves the timelike curve class. Chronological futures and pasts of points are open. A nonzero timelike vector cannot pair to zero with the time-orientation field $N$. The ZFC convention of the model supplies Countable Choice and Dependent Choice for these suppliers. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus) [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness) [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [post-stationary-vacuum-model](item-post-stationary-vacuum-model)

## External input

Source 0 is used for the precise AF orbit assumptions and for the analytic completion, initial neighborhood, Killing-scalar differential identity, local reciprocal-invariant identity and horizon values at its listed locators. These are imported premises under the full source hypotheses, rather than locally reconstructed analytic results. The local proof below establishes stationarity, section-to-exterior transport and scalar gluing.

## Proof

**Given:** The full hypotheses in the Statement.

**Goal:** Establish the stated scalar and tensor conclusions.

1.1 Let $U=M^{\mathrm{end}}$ and let $\Phi:\mathcal D\to M$ be the ambient maximal flow of $T$. By AF completeness, $\mathbb R\times E\subseteq\mathcal D$. The set $E=I^-_M(U)\cap I^+_M(U)$ is open, since each chronological set of $U$ is a union of the open chronological sets of its points. On $U$, uniqueness of integral curves and $T=\partial_t$ give $\Phi_s(t,x)=(t+s,x)$ for every real $s$, so $U$ is invariant. By the Killing equation $\mathcal L_Tg=0$ in [F1] and the tensor-flow criterion in [F4], each sufficiently short local time map satisfies $\Phi_s^*g=g$. Composing these local isometries along a finite orbit segment makes each ambient time map an isometry on its open domain. For $q\in E$ and a future timelike $v\in T_qM$, $d\Phi_s(v)$ remains timelike and depends continuously on $s$. Its pairing with $N_{\Phi_s(q)}$ is nonzero and initially negative, hence negative for all $s$. Thus these differentials preserve future timelike vectors at every point of $E$, without assuming that the image already lies in $E$. [F1, F2, F4, F6, F7]

2.1 Fix $p\in E$ and choose future timelike curves $a\to p\to b$ with $a,b\in U$. Since $U$ is open, trim their end portions to obtain $a'\to p\to b'$ with $a',b'\in U$, strictly between $a$ and $p$ and between $p$ and $b$, respectively. Every point of the trimmed curves, including their endpoints, is chronologically after $a$ and before $b$ by restriction and finite concatenation, and therefore belongs to $E$. Consequently $\Phi_s$ is defined on both entire trimmed curves for every real $s$. Smooth composition and step 1.1 show that their images are future timelike curves from $\Phi_s(a')$ through $\Phi_s(p)$ to $\Phi_s(b')$. Both endpoints lie in $U$ by its invariance, so $\Phi_s(p)\in E$. This proves $\Phi_s(E)\subseteq E$ for every $s$; applying $-s$ and the inverse-flow law gives equality. Thus the restriction is a smooth complete flow $\mathbb R\times E\to E$ with diffeomorphic time maps. [F2, F6, F7, step 1.1, choose]

3.1 Apply the analytic completion to obtain $1-\sigma\ne0$ and $\mathcal S=0$ on $\Sigma_0\cap E$, and retain its initial neighborhood of the bifurcation sphere. By step 2.1, the complete stationary flow preserves $E$. For every $p\in E$, the AF orbit assumption gives $q\in\Sigma_0\cap E$ and $t\in\mathbb R$ with $p=\Phi_t(q)$. This uses the exact IK orbit hypothesis after exterior preservation has been proved. [F1, F2, F3, step 2.1]

4.1 Antisymmetry gives $T(\sigma)=d\sigma(T)=2\mathcal F(T,T)=0$. Integrating along each stationary orbit gives $\sigma(\Phi_t(q))=\sigma(q)$, with the same supplied normalized potential and no additive shift. Hence $1-\sigma(p)\ne0$ for every $p\in E$ by step 3.1. In particular the Mars–Simon formula now defines a smooth tensor on all of $E$, before any tensor transport is applied. [F1, F2, step 3.1, algebra]

5.1 The local time maps preserve the metric by step 1.1. Differentiating the flow law $\Phi_t(\Phi_s(p))=\Phi_s(\Phi_t(p))$ at $s=0$ gives $d\Phi_t|_p(T_p)=T_{\Phi_t(p)}$. Their differentials are invertible by [F6] and vary continuously from the identity, so their orientation sign remains positive. The real and imaginary parts of $\mathcal F$ have vanishing Lie derivatives by [F4]; applying its real tensor-flow criterion to each part gives $\Phi_t^*\mathcal F=\mathcal F$. The same criterion gives $\Phi_t^*F=F$. Thus these maps preserve the metric, $T$, orientation and the forms without any completeness assumption at this local stage. For such a flow map $\psi$, transport the connection by $\widetilde\nabla_XY=(d\psi)^{-1}(\nabla_{\psi_*X}\psi_*Y)$. The connection rules and the chain rule show it is metric-compatible; its torsion vanishes because diffeomorphisms preserve the vector-field bracket. Uniqueness in [F4] gives $\widetilde\nabla=\nabla$. Substitution into the curvature formula therefore gives $\psi^*R=R$ in the same convention. The preserved oriented metric also preserves its volume tensor and Hodge operation. Thus every factor in the Mars–Simon formula is preserved, including $\sigma$ by step 4.1, so $\Phi_t^*\mathcal S=\mathcal S$. Composing local maps along the complete orbit gives this identity for every real $t$. The transport lemma in [F5] now applies on all of $E$ and yields $\mathcal S=0$ there. [F1, F2, F4, F5, F6, step 1.1, step 3.1, step 4.1]

6.1 On this connected zero region, source (4.33) and (7.1) give $d(\mathcal F^2(1-\sigma)^{-4})=0$. The initial sphere neighborhood and its assumed sphere value identify the constant as $-1/(4M^2)$, giving $-4M^2\mathcal F^2=(1-\sigma)^4$ throughout $E$. Thus the full hypotheses for the local differential computation in source Lemma 7.1 hold in every overlapping zero-region chart. [F1, F3, step 3.1, step 4.1, step 5.1]

7.1 That computation says $dB=0$ for the same smooth scalar $B=z^2+4M^2(y^2+z^2)g^{-1}(dz,dz)$. These local identities glue without coordinate or branch choices because $y,z$ come from the one normalized nonvanishing denominator, with the fixed inverse-metric contraction of [F5]. Connectedness makes the value global. Its value agrees with the initial neighborhood at $S$, where source Lemma 8.1 gives $0\le B<1/4$ and $y_S=(1+\sqrt{1-4B})/2$; source Lemma 7.1 gives $z^2\le B$, including on $S$ by continuity. Thus its horizon and end values are the same constant; no global chart-to-Kerr map has been assumed. [F1, F3, F5, step 6.1] ∎

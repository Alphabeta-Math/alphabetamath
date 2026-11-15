---
title: Mars–Simon tensor and its smooth weighted extension
status: draft
research_item: def-author-ad064c44a1cc-weighted-mars-simon
dependency_level: 4
sources:
  references:
    - title: "S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth
        stationary black holes in vacuum: small perturbations of the Kerr
        spaces"
      url: https://arxiv.org/html/0904.0982v1
      locator: Section 2.3, equations (2.18)–(2.19), with (2.13), (2.16)–(2.17) and
        the weighted-smoothness sentence immediately after (2.19).
      reading_limits: Read arXiv v1 HTML section 2.3, (2.13)–(2.19), the intervening
        potential-domain paragraph and the sentence following (2.19); checked
        section 1.1 GR/SBS and section 2.1 neighborhood construction. HTML
        renders the weighted sentence with a malformed tensor glyph. Formula
        coefficients are explicit in (2.18)–(2.19); smoothness is justified
        locally below. No PDF image inspection or rigidity-proof review is
        claimed.
      statement: On $U\cap\{\sigma\ne1\}$, (2.18) defines $\mathcal
        Q=(1-\sigma)^{-1}(\mathcal F\otimes\mathcal F-\mathcal F^2\mathcal I/3)$
        and (2.19) names $\mathcal S=\mathcal R+6\mathcal Q$ the Mars–Simon
        tensor; the next sentence asserts that $(1-\sigma)\mathcal S$ extends
        smoothly over $U=\widetilde M$.
      hypotheses: The source GR/SBS stationary Ricci-flat four-manifold and its smooth
        normalized Ernst potential on $U=\widetilde M$, supplied by
        def-author-ad064c44a1cc-ernst-curvature-package, with AIK Hodge,
        curvature and bilinear-contraction conventions. Division requires
        $\sigma\ne1$. PK smallness is unnecessary for these definitions and
        their weighted extension.
---

## Prerequisites

- [def-author-ad064c44a1cc-ernst-curvature-package](item-def-author-ad064c44a1cc-ernst-curvature-package)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [math:prop-tensor-products-and-contractions-of-smooth-tensor-fields-are-smooth](https://alphabetamath.cc/item/prop-tensor-products-and-contractions-of-smooth-tensor-fields-are-smooth)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth stationary black holes in vacuum: small perturbations of the Kerr spaces · Section 2.3, equations (2.18)–(2.19), with (2.13), (2.16)–(2.17) and the weighted-smoothness sentence immediately after (2.19). `](https://arxiv.org/html/0904.0982v1)


## Definition

Use the preceding AIK-convention tensor and potential data. On $U'=\{\sigma\ne1\}$ define
$$\mathcal Q_{ab cd}=(1-\sigma)^{-1}\left(\mathcal F_{ab}\mathcal F_{cd}-\tfrac13\mathcal F^2\mathcal I_{ab cd}\right),\qquad \mathcal S=\mathcal R+6\mathcal Q.$$
This $\mathcal S$ is the source's Mars–Simon tensor. Its weighted version is the globally smooth covariant four-tensor
$$\mathcal W=(1-\sigma)\mathcal R+6\left(\mathcal F\otimes\mathcal F-\tfrac13\mathcal F^2\mathcal I\right).$$
On $U'$ it equals $(1-\sigma)\mathcal S$. At points where $\sigma=1$, $\mathcal W$ is defined by this polynomial formula, not by dividing by zero. No vanishing, Kerr-characterization, Weyl-symmetry or propagation theorem is inferred from these formulas alone.

## Facts & Assumptions

[F1] [def-author-ad064c44a1cc-ernst-curvature-package](item-def-author-ad064c44a1cc-ernst-curvature-package) supplies the smooth potential and source-convention tensors on their potential domain.

[F2] [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data) supplies complex two-forms, their real and imaginary parts, and the complex bilinear contraction convention.

[F3] [math:prop-tensor-products-and-contractions-of-smooth-tensor-fields-are-smooth](https://alphabetamath.cc/item/prop-tensor-products-and-contractions-of-smooth-tensor-fields-are-smooth) supplies tensor products and contractions of smooth real tensor fields and their smoothness. Apply these operations complex bilinearly, by taking real and imaginary parts as in [F2].

## Justification

**Given:** The smooth potential and tensor fields of [F1], the complex convention of [F2], and the real tensor operations of [F3].

1.1 For smooth real tensor fields $A,B,C,D$, define the complex tensor product by $(A+iB)\otimes(C+iD)=(A\otimes C-B\otimes D)+i(A\otimes D+B\otimes C)$. Bilinearity of the real tensor product makes this intrinsic and complex bilinear; [F3] makes each real and imaginary component smooth. Contraction extends by the same real and imaginary decomposition. Smooth scalar multiplication and sums are smooth componentwise, so these operations apply to all products and contractions in the Definition. [F1, F2, F3, algebra]

2.1 The set $U'$ is open because $\sigma$ is continuous. There $(1-\sigma)^{-1}$ is smooth: for $1-\sigma=x+iy$, its real and imaginary components are $x/(x^2+y^2)$ and $-y/(x^2+y^2)$, with nonzero denominator. Thus the displayed $\mathcal Q$ and $\mathcal S$ are smooth on $U'$. Multiplication by $1-\sigma$ gives exactly $\mathcal W$. Its polynomial formula uses only smooth products, contractions and sums, so it defines a smooth covariant four-tensor throughout the potential domain, including $\sigma=1$. This proves the weighted identity and well-definedness without assuming any rigidity conclusion. [F1, F2, F3, step 1.1, algebra] ∎

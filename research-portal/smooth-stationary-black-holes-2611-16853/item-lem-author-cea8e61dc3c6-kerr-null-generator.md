---
title: The outer Kerr null hypersurface and its future generator
status: published
research_item: lem-author-cea8e61dc3c6-kerr-null-generator
dependency_level: 3
sources:
  references:
    - title: Saul A. Teukolsky, The Kerr Metric (arXiv:1410.2130v2)
      url: https://arxiv.org/pdf/1410.2130
      locator: §2, equations (2.1), (2.5)–(2.9), PDF pp. 2–3
      statement: The ingoing and Boyer–Lindquist Kerr metric forms and their
        coordinate transformation are displayed; the review identifies M as the
        mass and the roots of the radial function as null horizon candidates.
      hypotheses: Kerr metric in the stated ingoing and Boyer–Lindquist coordinate domains.
      reading_limits: Consulted extracted PDF text of section 2, equations (2.1),
        (2.5)–(2.9), PDF pages 2–3, and adjacent discussion. Only coordinate and
        parameter background is used. The normal, geodesic, orientation,
        maximal-continuation and extremal claims are proved locally from the
        declared mathematical suppliers; no proof of those full claims is
        imported from this review.
---

## Prerequisites

- [def-author-cea8e61dc3c6-kerr-ingoing-extension](item-def-author-cea8e61dc3c6-kerr-ingoing-extension)
- [def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [` Saul A. Teukolsky, The Kerr Metric (arXiv:1410.2130v2) · §2, equations (2.1), (2.5)–(2.9), PDF pp. 2–3 `](https://arxiv.org/pdf/1410.2130)


## Statement

Assume Countable Choice for the smooth tangent-bundle and vector-field constructions in the supplied connection and generator interfaces. In the specified ingoing extension the hypersurface $H=\{r=r_+\}$ is smooth and null. Put $\Omega_H=a/(r_+^2+a^2)$ and $\chi=\partial_v+\Omega_H\partial_\psi$. Then $\chi$ is nonzero and future-directed on $H$, tangent to its null generators, and
$$\nabla r|_H=\frac{r_+^2+a^2}{\Sigma}\chi.$$
This holds also for $|a|=M$.

## Statement references

[def-author-cea8e61dc3c6-kerr-ingoing-extension](item-def-author-cea8e61dc3c6-kerr-ingoing-extension)

[def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

## Facts & Assumptions

[F1] The specified ingoing extension supplies the smooth Lorentzian metric on $\mathbb R_v\times(0,\infty)_r\times S^2$, its parameters, the global rotation field $\partial_\psi=\xi$, rotations $R_\lambda$, and the temporal function $\tau=v-r$ with its future orientation. [def-author-cea8e61dc3c6-kerr-ingoing-extension](item-def-author-cea8e61dc3c6-kerr-ingoing-extension)

[F2] A generator of $H$ is the image of a future-directed affine null geodesic maximally continued while remaining in $H$. Only the general curve, generator and maximal-continuation definitions in the first three paragraphs are used here; the stationary causal-boundary application and its imported ray assertion are not used. [def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section)

[F3] The Levi–Civita connection is torsion-free and metric-compatible, and obeys the affine-connection product rules. These are mathematical properties of the supplied smooth Lorentzian metric. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F4] Countable Choice ($\mathrm{AC}_\omega$) is assumed for the smooth tangent-bundle and vector-field constructions used by [F2] and [F3]. It supplies the hypothesis needed when applying the connection rules to smooth fields and interpreting the resulting curves as affine null geodesics. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

## Proof

**Given:** The smooth ingoing extension of [F1], the generator convention [F2], and the Levi–Civita rules [F3], under Countable Choice [F4].

**Goal:** Identify the outer null hypersurface, its orientation, and its geodesic generators.

1.1 Multiplication by the metric matrix yields $n:=\nabla r=((r^2+a^2)\partial_v+\Delta\partial_r+a\xi)/\Sigma$. This pole-free expression and $g(n,n)=\Delta/\Sigma$ hold also on the axis by smoothness. Since $dr$ never vanishes and $\Delta(r_+)=0$, the product level $H=\{r=r_+\}$ is smooth and null, and $n|_H=b\chi$ with $b=(r_+^2+a^2)/\Sigma>0$. Also $dr(n)=0$ there, so $n$ is tangent and normal to $H$. In a Lorentzian tangent space, the orthogonal complement of a nonzero null vector has that vector as its radical and has positive definite quotient by its span; consequently all nonzero null tangents to $H$ lie on the line spanned by $n$. This identifies the null tangent line without yet asserting its geodesic property. [given, F1]

2.1 With $\tau=v-r$ one has $d\tau(\chi)=1>0$. Since $\tau$ increases on future causal curves in the chosen orientation, $\chi$ is future null. Its $v$ component is one, so it is nonzero even at the rotation axis, where $\xi$ vanishes. [F1, step 1.1]

2.2 For smooth local fields $X,Y$, metric compatibility and torsion freedom give $g(\nabla_Xn,Y)-g(\nabla_Yn,X)=X(Yr)-Y(Xr)-[X,Y]r=0$. Thus $g(\nabla_nn,X)=g(\nabla_Xn,n)=\tfrac12 X(g(n,n))$ for every $X$, and nondegeneracy yields $\nabla_nn=\tfrac12\nabla(\Delta/\Sigma)$. On $H$, this becomes $\nabla_nn=\Delta^{\prime}(r_+)n/(2\Sigma)$, where $\Delta^{\prime}(r_+)=2r_+-2M$. Since $n=b\chi$ on $H$, differentiation in the tangent direction $n$ is legitimate for this restricted equality; moreover $\chi(b)=0$ because $b$ depends only on $r$ and the rotation-invariant sphere coordinate $z$. The connection product rule therefore gives $\nabla_\chi\chi=\kappa\chi$ on $H$, with $\kappa=\Delta^{\prime}(r_+)/(2(r_+^2+a^2))=(r_+-r_-)/(2(r_+^2+a^2))\geq0$. Thus these null curves are pregeodesic, meaning their acceleration is proportional to their velocity. [F1, F3, F4, step 1.1, algebra]

3.1 Through any $(v_0,r_+,p_0)\in H$, the curve $c(u)=(v_0+u,r_+,R_{\Omega_Hu}p_0)$, $u\in\mathbb R$, has velocity $\chi$ and is future null. If $\kappa>0$, set $s=(e^{\kappa u}-1)/\kappa$; if $\kappa=0$, set $s=u$. In both cases $ds/du>0$, and writing $w=du/ds$ gives $dc/ds=w\chi$ and $D_s(dc/ds)=(w^2\kappa+w\,dw/du)\chi=0$ by the preceding connection product rule. Thus this is an affine null geodesic in the sense of [F2]. Its affine parameter interval is $(-1/\kappa,\infty)$ when $\kappa>0$ and $\mathbb R$ when $\kappa=0$. The only finite boundary in the first case corresponds to $u\to-\infty$ and hence $v\to-\infty$, so no continuous extension at that boundary exists in the specified product manifold. These geodesics are therefore maximally continued in $H$. Conversely, any future null curve in $H$ is locally a positive reparametrization of one of these curves: its tangent lies in the line from step 1.1, and taking $u=v-v_0$ gives $dr/du=0$ and the rotation equation $dp/du=\Omega_H\xi(p)$, whose explicit solution is $p=R_{\Omega_Hu}p_0$ (as is checked by differentiating $R_{-\Omega_Hu}p$). Any proper segment extends along that same orbit, after matching its affine parameter by a positive affine change of the displayed $s$. Hence the complete orbit images are exactly the generators of [F2], and $\chi$ is tangent to them. All formulas remain valid for $|a|=M$, when $\kappa=0$; none divides by $r_+-r_-$. [F1, F2, F3, F4, step 1.1, step 2.1, step 2.2, algebra] ∎

## External input

The cited Kerr review supplies the coordinate and parameter background stated in its reference record; the result above, including the geodesic and maximal-continuation claims, is derived under the declared mathematical hypotheses and dependencies.

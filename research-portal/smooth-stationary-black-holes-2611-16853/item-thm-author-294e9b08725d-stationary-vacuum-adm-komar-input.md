---
title: External ADM–Komar equality on ordinary stationary vacuum ends
status: published
research_item: thm-author-294e9b08725d-stationary-vacuum-adm-komar-input
dependency_level: 2
sources:
  references:
    - title: Hamed Barzegar, Piotr T. Chruściel and Michael Hörzinger, Energy in
        higher-dimensional spacetimes
      url: https://arxiv.org/pdf/1708.03122v2
      locator: Section II (II.1)–(II.4), printed p.3; Section III A (III.13), p.5,
        (III.18)–(III.19), p.6; (III.34), p.7; Section IV B (IV.16)–(IV.20),
        pp.12–13, (IV.29)–(IV.30), p.16; Section V (V.1)–(V.5), pp.19–20;
        specialize to K=0, n=3, flat background and Ric=0.
      statement: With no compact extra dimensions, the stationary vacuum
        specialization of (V.5) equates the Hamiltonian time-translation charge
        with the normalized Komar integral; (III.18)–(III.19) identify that
        charge as ordinary ADM energy.
      hypotheses: Flat background eta; K=0, n=3; T=partial_t is physical Killing and
        background parallel; Ric(g)=0. The stated O_2(r^-1) falloff gives
        square-integrable first derivatives as in III.13 and satisfies II.2 with
        alpha=1/2. It gives deltaGamma=O(r^-2) and Riem=O(r^-3), allowing
        beta=1.9 and beta_R=2.9. With Z=r partial_r, IV.17 holds exactly modulo
        the specified dt/dr terms; background derivative T is zero. Choose
        gamma=2. The effective decay exponents in IV.20 and IV.30 are 2.4, 2.8,
        3.9 and 2.4, all greater than the sphere-area exponent 2. Vacuum
        eliminates the Ricci term in V.5 and K=0 eliminates every
        extra-dimension term. No constant 1/r coefficient in g_00 or sixth-order
        falloff is needed.
      reading_limits: Consulted browser-extracted text of the listed formulas, their
        hypotheses and adjacent definitions, including III.34 for the surface
        orientation and V.1–V.5 for the Komar identity. PDF screenshots were
        unavailable. This imports the identity and convergence criterion,
        without a full-paper review or reconstruction of their proofs. The
        exponent substitutions and translation to the displayed future/outward
        convention were checked locally; no claim is made for Kaluza–Klein ends.
external_input: true
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)
- [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)
- [math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [` Hamed Barzegar, Piotr T. Chruściel and Michael Hörzinger, Energy in higher-dimensional spacetimes · Section II (II.1)–(II.4), printed p.3; Section III A (III.13), p.5, (III.18)–(III.19), p.6; (III.34), p.7; Section IV B (IV.16)–(IV.20), pp.12–13, (IV.29)–(IV.30), p.16; Section V (V.1)–(V.5), pp.19–20; specialize to K=0, n=3, flat background and Ric=0. `](https://arxiv.org/pdf/1708.03122v2)


## Statement

For a smooth four-dimensional stationary vacuum end with $T=\partial_t$, $g-\eta=O_2(r^{-1})$, $g_{0i}=O_2(r^{-2})$, and the future unit time-translation normalization at infinity, the ordinary ADM energy of the $t=0$ end equals its future/outward normalized Komar mass $m_K$. Here $\eta=-dt^2+\sum_{i=1}^3(dx^i)^2$, $r=|x|$ in the end chart, and vacuum means $\operatorname{Ric}(g)=0$. There are no Kaluza–Klein directions. No maximality is assumed.

For sufficiently large $r$, put $h=g_{ij}\,dx^i dx^j$ on $t=0$, let $n$ be its future unit spacetime normal, let $\nu$ be the outward $h$-unit normal to $S_r=\{t=0,|x|=r\}$, and let $dA_h$ be the Riemannian area density on $S_r$. Use the spatial-metric ADM energy convention and set
$$m_K=\frac1{4\pi}\lim_{r\to\infty}\int_{S_r}n^a\nu^b\nabla_aT_b\,dA_h.$$
Both flux limits exist under the stated hypotheses and $E_{\rm ADM}=m_K$. The conventions are in geometric units $G=c=1$ and the inherited ZFC setting.

## Statement references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)

[math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)

[math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted equality and existence of its flux limits.

[A1] The stationary Lorentzian conventions are mathematical data in ZFC, including choice; in particular they supply the connection, Ricci tensor, Killing condition and future direction. Restricting choice to countable families supplies the choice hypothesis for density integration. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The differentiated end bounds are the angularly uniform spatial bounds through order two. Stationarity gives $\partial_tg_{\mu\nu}=0$; hence the stated bounds meet the falloff hypotheses of the imported ordinary-end identity, without an assumption about a constant coefficient in $g_{00}$. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] The charge convention supplies the induced metric, future normal, outward sphere normal and ordinary spatial-metric ADM flux. Only its geometric and energy clauses are used; its separate axial-action data are not required. [def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)

[F3] The induced positive metric on each compact smooth coordinate sphere supplies its smooth area density. The displayed scalar flux uses integration of that density times its smooth integrand; compactness gives compact support. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density)

[F4] Barzegar–Chruściel–Hörzinger (III.13), (III.18)–(III.19), (III.34) and (V.5), under the boundary hypotheses recorded in the source metadata, supply convergence, ADM identification and the stationary vacuum Komar equality in the ordinary four-dimensional case.

## External input

The imported result is the $K=0$, $n=3$, flat-background, vacuum specialization of [Barzegar–Chruściel–Hörzinger, Section V (V.5)](https://arxiv.org/pdf/1708.03122v2), with the ADM identification in (III.18)–(III.19). Its proof is not reconstructed here.

The stated falloff implies $\partial g=O(r^{-2})$, $\delta\Gamma=O(r^{-2})$ and $\operatorname{Riem}(g)=O(r^{-3})$. Thus (III.13) holds, and the choices $\alpha=1/2$, $\beta=1.9$, $\beta_R=2.9$, $\gamma=2$, $Z=r\partial_r$ meet (IV.16)–(IV.20) and (IV.29)–(IV.30): the four effective decay exponents are $2.4,2.8,3.9,2.4>2$. The Killing field is also parallel for the flat background; there are no extra-dimension terms and the Ricci term vanishes. These are checks of the imported hypotheses, using only the bounds in the Statement.

For the compatible future/outward orientation, the physical binormal element is $dS^g_{ab}=(n_b\nu_a-n_a\nu_b)dA_h$. Killing antisymmetry gives $T^{a;b}dS^g_{ab}=2n^a\nu^b\nabla_aT_b\,dA_h$. The surface-element convention (III.34), when taken for the flat background, differs from this physical element by relative $O(r^{-1})$ in the fixed chart. Since $\nabla T=O(r^{-2})$ and sphere area is $O(r^2)$, this replacement changes the integrated flux by $O(r^{-1})$, which tends to zero. Thus the $1/(8\pi)$ Komar factor in this specialization of (V.5) yields the $1/(4\pi)$ scalar-flux convention in the Statement. No mass-coefficient expansion or extrinsic-decay lemma enters this normalization.

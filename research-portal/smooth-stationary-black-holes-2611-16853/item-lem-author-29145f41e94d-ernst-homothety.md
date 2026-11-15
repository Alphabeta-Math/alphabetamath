---
title: The mass factor in the recovered Ernst identity
status: published
research_item: lem-author-29145f41e94d-ernst-homothety
dependency_level: 5
---

## Prerequisites

- [lem-author-29145f41e94d-homothetic-stationary-geometry](item-lem-author-29145f41e94d-homothetic-stationary-geometry)
- [thm-vacuum-killing-ernst-input](item-thm-vacuum-killing-ernst-input)
- [def-killing-ernst-notation](item-def-killing-ernst-notation)


## Statement

Let $(M,g,N,o)$ be a smooth oriented, time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$, let $T$ be a smooth Killing field and let $m>0$ be constant. Keep the manifold, orientation and time orientation fixed, and set $\widehat g=m^{-2}g$ and $\widehat T=mT$. Define $F_{ab}=\nabla_aT_b$, $\mathcal F=F+i\star_gF$ and the hatted fields by the same conventions. Squares denote complex bilinear contraction with both indices raised by the indicated metric, without conjugation or a factor of one half. Then $\widehat{\mathcal F}=m^{-1}\mathcal F$ and $\widehat{\mathcal F}^{\,2}_{\widehat g}=m^2\mathcal F_g^2$ on $M$.

Let $U\subseteq M$ be a connected open set with a designated coordinate end $(t,x):U_{\mathrm{end}}\to I\times\{|x|>R_0\}$, where $I$ is a nonempty open interval, $R_0>0$, $T=\partial_t$ and $dt\wedge dx^1\wedge dx^2\wedge dx^3$ is positive. Assume a smooth normalized Ernst potential $\sigma$ is supplied on $U$: $d\sigma=2\iota_T\mathcal F$, $\operatorname{Re}\sigma=-g(T,T)$ and $\sigma\to1$ uniformly in $t\in I$ and the spatial directions as $|x|\to\infty$. For the hatted geometry use the same end subset with coordinates $(\widehat t,x)=(t/m,x)$. Then $\widehat\sigma:=\sigma$ is its unique normalized Ernst potential on $U$. Existence of the original global potential is a hypothesis, rather than a consequence of local closedness.

If a continuous extension of $\sigma$ to $U\cup B$ is supplied for a set $B\subseteq\overline U\setminus U$, the same function extends $\widehat\sigma$ there. Here $B$ may be empty. If $p\in U\cup B$ is a common zero of $T$ and a supplied smooth field $Z$ near $p$, it remains the same common zero of $\widehat T$ and $Z$; this includes a supplied axial field. Any supplied bifurcation sphere remains the same sphere. On $U\cup B$, and hence on any such sphere contained there, the identity $-4\widehat{\mathcal F}^{\,2}_{\widehat g}=(1-\widehat\sigma)^4$ is equivalent to $-4m^2\mathcal F_g^2=(1-\sigma)^4$. At such a common zero $p$, the denominator $1-\sigma(p)$ is nonzero, and the inequality $\operatorname{Re}(1/(1-\widehat\sigma(p)))>1/2$ is exactly $\operatorname{Re}(1/(1-\sigma(p)))>1/2$ for the original geometry.

## Statement references

[lem-author-29145f41e94d-homothetic-stationary-geometry](item-lem-author-29145f41e94d-homothetic-stationary-geometry)

[thm-vacuum-killing-ernst-input](item-thm-vacuum-killing-ernst-input)

[def-killing-ernst-notation](item-def-killing-ernst-notation)

## Facts & Assumptions

[F1] Constant homothety preserves the connection, Killing fields, supplied bifurcation sphere and original maximal section, and satisfies $\star_{\widehat g}=\star_g$ on two-forms. [lem-author-29145f41e94d-homothetic-stationary-geometry](item-lem-author-29145f41e94d-homothetic-stationary-geometry)

[F2] If $\operatorname{Ric}(g)=0$, the vacuum Ernst one-form is closed and has local potentials; this supplies no global primitive or normalization by itself. Here the global normalized potential on the specified connected $U$, and any boundary extension used for evaluation, are supplied hypotheses. [thm-vacuum-killing-ernst-input](item-thm-vacuum-killing-ernst-input)

[F3] Use the Killing-form, complex bilinear contraction, coordinate-end and normalized-potential conventions; the normalization includes the real-part condition and the uniform end limit. [def-killing-ernst-notation](item-def-killing-ernst-notation)

## Proof

**Given:** The geometry, connected domain, designated end and supplied normalized potential in the Statement, with its optional extension and evaluation data when used.

**Goal:** Prove the scaling and potential transfer, and the equivalence of the displayed identities and inequalities on their stated domains.

1.1 Lowering the hatted field gives $\widehat T^\flat=m^{-1}T^\flat$. The common connection and Hodge map therefore give $\widehat F=m^{-1}F$ and $\widehat{\mathcal F}=m^{-1}\mathcal F$. Since $\widehat g^{-1}=m^2g^{-1}$, raising the two indices in the full bilinear contraction multiplies the square by $m^{-2}m^4=m^2$. No complex conjugation is inserted. [given, F1, F3, algebra]

2.1 The supplied global potential obeys $d\sigma=2\iota_T\mathcal F=2\iota_{\widehat T}\widehat{\mathcal F}$, and $-\widehat g(\widehat T,\widehat T)=-g(T,T)=\operatorname{Re}\sigma$. Thus $\widehat\sigma:=\sigma$ meets both differential and real-part conditions on all of $U$. The vacuum differential identity alone would only supply local potentials; the global one used here is the stated hypothesis. [given, F2, F3, step 1.1, algebra]

3.1 The new end chart has range $m^{-1}I\times\{|x|>R_0\}$ and $\widehat T=\partial_{\widehat t}$. Its orientation is unchanged because $m>0$. For every $\varepsilon>0$, the original bound for all $t\in I$ and $|x|>R$ is exactly the hatted bound for all $\widehat t\in m^{-1}I$ and $|x|>R$. Hence $\widehat\sigma$ is normalized at this end. If $\tau$ is any other hatted normalized potential on $U$, then $d(\tau-\sigma)=0$. On a coordinate ball, integration of this zero differential along straight coordinate segments makes the difference constant; it is therefore locally constant, and connectedness of $U$ makes it one constant on $U$. Its limit zero on the designated end forces that constant to vanish. [given, F3, step 2.1]

4.1 Equality on $U$ carries the supplied continuous extension of $\sigma$ to the hatted potential on $U\cup B$; it supplies their values at every stated evaluation point. The point $p$ is unchanged and $\widehat T_p=mT_p=0$, while the unchanged $Z_p$ is zero. Any supplied bifurcation sphere is unchanged by [F1]. The tensor scaling from step 1.1 holds on all of $M$, so substitution of $\widehat\sigma=\sigma$ gives the equivalence of the two identities wherever the supplied potential or extension is defined. On $U$ the real-part condition is $\operatorname{Re}\sigma=-g(T,T)$, and continuity carries this equality to each point of $B$ because $B\subseteq\overline U$. At the common zero $p$, it gives $\operatorname{Re}\sigma(p)=0$, hence $\operatorname{Re}(1-\sigma(p))=1$ and the denominator cannot vanish. The denominator is identical for both potentials, so their reciprocals, real parts and strict inequalities agree. [given, F1, F3, step 1.1, step 3.1, algebra] ∎

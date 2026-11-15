---
title: Stationary vacuum normal form and compatible regularity section
status: draft
research_item: thm-author-ae62588ad46a-stationary-asymptotic-normal-form
dependency_level: 6
sources:
  references:
    - title: P. T. Chruściel and J. L. Costa, On uniqueness of stationary vacuum black
        holes
      url: https://arxiv.org/html/0806.0016
      locator: §2.1, (2.1)–(2.8), the harmonic-coordinate/maximal-time-gauge paragraph
        and the final isotropic Schwarzschild display.
      statement: For a vacuum stationary asymptotically flat end with a timelike
        limiting translation, rest-frame adapted coordinates admit a
        differentiated expansion in inverse radius and logarithms, with
        Schwarzschild leading correction. For three spatial dimensions this
        gives $g_{00}=-1+2m/r+o_3(r^{-1})$,
        $g_{ij}=(1+2m/r)\delta_{ij}+o_3(r^{-1})$ and $g_{0i}=o_3(r^{-1})$.
      hypotheses: Four-dimensional smooth Ricci-flat geometry;
        $h-\delta=O_k(r^{-\alpha})$, $k_{ij}=O_{k-1}(r^{-1-\alpha})$,
        $\alpha>0$, integer $k>1$; a Killing field with a future unit timelike
        limiting translation. The translation is supplied by Proof 1.1 below,
        rather than by invoking the positive-energy discussion in this source.
      reading_limits: Consulted the complete HTML §2.1. Its elliptic asymptotic
        analysis and cited proofs are imported, not reconstructed. This
        reference supplies no compatibility with a global regularity section.
    - title: "R. Beig and P. T. Chruściel, Killing vectors in asymptotically flat
        space-times: I. Asymptotically translational Killing vectors and the
        rigid positive energy theorem"
      url: https://arxiv.org/pdf/gr-qc/9510015
      locator: arXiv:gr-qc/9510015v3, §2, (2.2)–(2.8), (2.13)–(2.16), and Proposition
        2.2, (2.26)–(2.29), printed pp.4–8, especially PDF page 8.
      statement: A spacetime Killing field decomposes as $T=Nn+Y$ and satisfies (2.4),
        (2.13), (2.15), with $\rho=\tau_{ij}=0$ in vacuum and the source
        convention $\bar k(U,V)=g(\nabla_U n,V)$. Proposition 2.2 gives an
        antisymmetric constant $\Lambda_{\mu\nu}$ with
        $Y^i-\Lambda_{ij}y^j=O_k(r^{1-\beta})$,
        $N+\Lambda_{0i}y^i=O_k(r^{1-\beta})$. If $\Lambda=0$, constants $A^\mu$
        satisfy $Y^i-A^i=O_k(r^{-\beta})$, $N-A^0=O_k(r^{-\beta})$; if also
        $A=0$, both fields vanish.
      hypotheses: Initial data on $\mathbb R^3\setminus B(R)$ with
        $h-\delta=O_k(r^{-\beta})$, $\bar k=O_{k-1}(r^{-1-\beta})$, integer
        $k>1$, $0<\beta<1$; $N,Y$ are $C^2$ and satisfy (2.4), (2.13), (2.15)
        with $|\rho|+|\tau_{ij}|\leq C(1+r)^{-2-\beta}$. Here $\bar k=-k$ in the
        declared local convention. Vacuum makes the source tensors zero. No
        positive-mass or complete-initial-slice assumption enters this
        proposition.
      reading_limits: Read PDF §2 through Proposition 2.2, including the displayed
        decomposition and equations used to check applicability. Proposition 2.2
        and its estimates are imported; Appendix C and the positive-energy
        theorems are not reconstructed or used.
    - title: P. T. Chruściel and J. L. Costa, On uniqueness of stationary vacuum black
        holes — stationary structure theorem
      url: https://arxiv.org/html/0806.0016
      locator: §4.2, Proposition 4.4, Theorem 4.5 and (4.15); proof through
        (4.18)–(4.23) and its final two paragraphs. Use s=1.
      statement: The stationary flow on an $I^+$-regular domain gives $D\simeq\mathbb
        R_u\times\Sigma_0$ and $\overline D\cap I^+(M_{\rm ext})\simeq\mathbb
        R_u\times\overline\Sigma_0$, with $Tu=1$, smooth spacelike time levels
        and an acausal smooth completed zero level. Its boundary is a compact
        cross-section of the future horizon. The construction has a compact
        interior and an asymptotically flat end in the original saturated end.
      hypotheses: An $I^+$-regular stationary spacetime with the complete stationary
        field generating the real factor of a commuting $\mathbb R\times\mathbb
        T^{s-1}$ isometry action. Here $s=1$, so no axial symmetry is assumed.
        Use the causal domain, completed section and end conditions of the
        declared analytic geometric data.
      reading_limits: Read the HTML statement of Theorem 4.5, Proposition 4.4 and the
        §4.2 construction, including its compact interior and final end
        matching. Import this structure theorem. The opening deformation
        paragraph alone is not used to identify any normal-form level. The
        gluing in Proof 3.1–8.1 is local to this item and is not attributed to
        the source.
---

## Prerequisites

- [def-author-ae62588ad46a-analytic-geometric-data](item-def-author-ae62588ad46a-analytic-geometric-data)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [` P. T. Chruściel and J. L. Costa, On uniqueness of stationary vacuum black holes · §2.1, (2.1)–(2.8), the harmonic-coordinate/maximal-time-gauge paragraph and the final isotropic Schwarzschild display. `](https://arxiv.org/html/0806.0016)
- [` R. Beig and P. T. Chruściel, Killing vectors in asymptotically flat space-times: I. Asymptotically translational Killing vectors and the rigid positive energy theorem · arXiv:gr-qc/9510015v3, §2, (2.2)–(2.8), (2.13)–(2.16), and Proposition 2.2, (2.26)–(2.29), printed pp.4–8, especially PDF page 8. `](https://arxiv.org/pdf/gr-qc/9510015)
- [` P. T. Chruściel and J. L. Costa, On uniqueness of stationary vacuum black holes — stationary structure theorem · §4.2, Proposition 4.4, Theorem 4.5 and (4.15); proof through (4.18)–(4.23) and its final two paragraphs. Use s=1. `](https://arxiv.org/html/0806.0016)


## Statement

For a smooth four-dimensional stationary vacuum end with $h_{ij}-\delta_{ij}=O_k(r^{-\alpha})$ and second fundamental form $k_{ij}=O_{k-1}(r^{-1-\alpha})$, where $\alpha>0$ and the integer $k>1$, suppose the stationary field has a future unit timelike limiting translation. There are adapted rest-frame coordinates $T=\partial_t$ and a stationary slicing with a differentiated full expansion in inverse powers of radius and logarithms whose leading correction is Schwarzschild. In particular, for some constant $m$, $g_{00}=-1+2m/r+o_3(r^{-1})$, $g_{ij}=(1+2m/r)\delta_{ij}+o_3(r^{-1})$ and $g_{0i}=o_3(r^{-1})$. This is local at infinity and requires neither horizon connectedness nor a global maximal slice. Here $O_j(r^{-b})$ bounds each spatial derivative of order $a\leq j$ by $Cr^{-b-a}$, and $o_j$ replaces these bounds by little-o estimates.

For the analytic geometric comparison data, the existing assumptions that $T$ is future timelike near infinity and $g(T,T)\to-1$ suffice to obtain that unit timelike limiting translation; it need not be added as a hypothesis. More precisely, on the supplied end, writing $T=Nn+Y$ in its future-normal frame gives constants $A^0>0,A^i$ with $N\to A^0$, $Y^i\to A^i$ and $(A^0)^2-\sum_i(A^i)^2=1$. In the $I^+$-regular setting one can choose an acausal regularity section and deform its sufficiently far-out end to contain a level of the above normal-form stationary time. During this deformation the chosen section's compact horizon cross-section boundary stays fixed, its completion retains a compact core and finitely many ends, and the boundary still meets every future-horizon generator exactly once. Thus the normal-form end and all regularity properties can be supplied simultaneously. The regularity hypothesis supplies a section existentially; no prescribed boundary beyond that hypothesis is additional data.

## Statement references

[def-author-ae62588ad46a-analytic-geometric-data](item-def-author-ae62588ad46a-analytic-geometric-data)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[F1] Work in ZFC, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice). The exact analytic vacuum, end-decay and $I^+$-regularity data are [def-author-ae62588ad46a-analytic-geometric-data](item-def-author-ae62588ad46a-analytic-geometric-data); metric and Killing conventions are [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). Use [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) for $n,k,N,Y$, and [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) for causal curves, $D$, completed sections and temporal functions. In particular the geometric definition supplies norm normalization, not an asserted limiting translation.

[F2] Beig–Chruściel Proposition 2.2 and its preceding vacuum decomposition equations are the second reference in External input. Use its second fundamental form $\bar k=-k$ and choose $0<\beta<\min\{\alpha,1\}$. The resulting asymptotic affine lapse and shift, and their improved constant asymptotes when the linear part vanishes, are imported. Positivity, elimination of the linear part and unit normalization are proved here.

[F3] The local rest-frame stationary normal form, differentiated expansion and Schwarzschild leading correction are imported from Chruściel–Costa §2.1, the first reference in External input, after supplying its timelike limiting translation. No section-deformation assertion is imported with that expansion.

[F4] Chruściel–Costa Theorem 4.5, with $s=1$, supplies a stationary temporal coordinate $u$ and a regularity section $\Sigma_0=\{u=0\}$ on $C=\overline D\cap I_M^+(M_{\rm ext})$, with the product and boundary properties in the third External input reference. Its end lies in the same stationary saturation. This supplies a starting section; the matching of its end to the normal-form time is the argument below.

[F5] Chronology is open and a past set contains the chronological past of its closure, by [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness). The two push-up rules are [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule). Smooth composition and the almost-everywhere chain rule for the locally absolutely continuous curve class are [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus). All three suppliers have actual domain mathematics. Their Countable Choice and Dependent Choice assumptions are included in [F1]'s ZFC convention.

## Proof

**Given:** The end hypotheses in the Statement, and the analytic geometric comparison data for the normalization and regularity assertions.

**Goal:** Supply the translation and normal form, and join its stationary time to a regularity section while preserving the required causal and boundary properties.

1.1 On the supplied end decompose $T=Nn+Y$. Future timelikeness gives $N>0$ and $h(Y,Y)<N^2$. The source equations in [F2] apply to this vacuum Killing data, with $\rho=\tau_{ij}=0$; weakening the stated decay exponent to $\beta$ verifies all hypotheses of Proposition 2.2. Its affine expansion gives $N=-\Lambda_{0i}y^i+O(r^{1-\beta})$. If the boost coefficient is nonzero, a ray on the full exterior sphere makes the linear term negative, contradicting $N>0$. Thus $\Lambda_{0i}=0$ and $N=o(r)$. If a rotational coefficient remains, choose a ray with $\Lambda_{ij}y^j/r\ne0$; then $h(Y,Y)$ grows quadratically while $N^2=o(r^2)$, contradicting timelikeness. Hence $\Lambda=0$. The improved source estimate gives $N=A^0+O_k(r^{-\beta})$ and $Y^i=A^i+O_k(r^{-\beta})$. Taking the limit in $g(T,T)=-N^2+h(Y,Y)\to-1$ gives $(A^0)^2-|A|^2=1$, and $N>0$ forces $A^0>0$. This establishes the limiting unit timelike translation without a positive-energy premise. The argument applies to any other asymptotically flat spacelike end in the same saturation on which the same norm limit holds. [given, F1, F2, algebra]

2.1 Apply [F3] to that translation, or to the translation explicitly assumed in the first paragraph of the Statement. The imported expansion has the displayed Schwarzschild leading terms; subsequent inverse-power/logarithmic terms and their differentiated remainders give the stated $o_3(r^{-1})$ estimates. Write its time as $t$ with $Tt=1$. This establishes the local end conclusion. For the remaining argument fix the $I^+$-regular data and keep the underlying geometry and stationary field fixed. In this setting the far-out stationary orbit product is defined for the complete real flow: the local stationary construction extends by time translation, and the original acausal end intersects each timelike orbit at most once. [given, F1, F3, step 1.1]

3.1 Apply [F4] to obtain $u,\Sigma_0$ and its compact boundary $B$ on $C$. Use end coordinates $y$ on $\Sigma_0$, extended by $T$, and write $r=|y|$. The end is asymptotically flat in the same saturation, so step 1.1 applies to its lapse and shift as well. They converge to finite constants $B^0>0,B^i$ with $(B^0)^2-|B|^2=1$. In the coordinates $(u,y)$, $g_{ij}\to\delta_{ij}$, $g_{ui}\to B^i$ and $g_{uu}\to-1$; both metric and inverse therefore are uniformly bounded. Moreover $g^{-1}(du,du)=-N_0^{-2}\to-(B^0)^{-2}$. The normal-form end of step 2.1 is a cofinal coordinate description on the same orbit space. Since $Tt=Tu=1$, its time has the form $t=u+f(y)$ there, and $g^{-1}(dt,dt)\to-1$ by its metric expansion. [F1, F2, F3, F4, step 1.1, step 2.1, algebra]

4.1 Here is the uniform cone and height control needed for gluing. Put $V^2=-g(T,T)$ and $a_*=-T^\flat/V^2$. Every covector $a$ with $a(T)=1$ decomposes uniquely as $a=a_*+z$, $z(T)=0$, and $g^{-1}(a,a)=-V^{-2}+g^{-1}(z,z)$. On $z(T)=0$, the inverse form is positive definite, with coefficients and inverse uniformly bounded in the $y$ coordinates by the limiting metric in step 3.1. Choose $\delta>0$ and $R$ large enough that both $a_0=du$ and $a_1=dt$ have squared norm at most $-2\delta$ for $r>R$. Their $z$ parts then have norm at most $\sqrt{V^{-2}-2\delta}$. The Euclidean triangle inequality in this positive-definite form shows that every $a_\theta=(1-\theta)du+\theta dt$, $0\leq\theta\leq1$, has squared norm at most $-2\delta$. These covectors have uniformly bounded coordinate coefficients. In particular $df=dt-du$ is bounded. Integrating along radial rays from a fixed sphere, on which $f$ is bounded, gives $|f(y)|\leq C_f r$ after increasing $R$. No bounded-height or asymptotic identification of the two slices has been assumed. [F1, step 3.1, algebra]

5.1 Choose a smooth nondecreasing function $\eta:\mathbb R\to[0,1]$ equal to zero on $(-\infty,0]$ and one on $[1,\infty)$, with bounded derivative. For example use $p(s)=e^{-1/s}$ for $s>0$, $p(s)=0$ otherwise, and $\eta(s)=p(s)/(p(s)+p(1-s))$. For a constant $L>0$ put $\chi(r)=\eta(\log(r/R)/L)$ and extend $\chi f$ by zero off the selected far-out stationary end. It is smooth because the cutoff is flat at its inner edge. For $0\leq s\leq1$ define $\tau_s=u+s\chi f$. Then $T\tau_s=1$ and $d\tau_s=(1-s\chi)du+s\chi dt+s f\,d\chi$. The last term has coordinate norm at most $C_f\|\eta'\|_\infty/L$. The bounds in step 4.1 on the inverse metric and on $a_\theta$ make its change to the squared norm at most $C_1/L+C_2/L^2$, for constants independent of $r,s,L$. Choose $L$ so that this is less than $\delta$. Thus $g^{-1}(d\tau_s,d\tau_s)<-\delta$ on the modified end; elsewhere $\tau_s=u$. Its gradient is past timelike: on the end its covector is positive on future timelike $T$, and off the end it equals $du$. Near the boundary of $C$ it also equals $du$, which has timelike differential up to that boundary by [F4]. This gives a smooth family of temporal functions on $C$. [F1, F4, step 4.1, construct, algebra]

6.1 The acausality conclusion is ambient, not merely a local spacelikeness test. Let $U=M_{\rm ext}$, $F=I_M^+(U)$ and $P_-=I_M^-(U)$. Since $F$ is open, $C=F\cap\overline{P_-}$. The push-up rule makes $F$ closed under taking causal futures. If $q\leq b$ with $b\in\overline{P_-}$, every $a\ll q$ satisfies $a\ll b$ by push-up. The closure-of-past-set assertion in [F5] therefore gives $a\in P_-$. Such points $a$ approach $q$ along a local timelike curve, so $q\in\overline{P_-}$. Thus $\overline{P_-}$ is closed under causal pasts. Every ambient causal curve whose endpoints lie in $C$ stays in $C$. Along it, $\tau_s$ is locally absolutely continuous and its derivative is positive almost everywhere by step 5.1 and the chain rule in [F5]. In a Lorentz frame this positivity is the inequality $a_0v^0+\mathbf a\cdot\mathbf v>0$ for a past-gradient timelike covector, whose positive time coefficient exceeds its spatial norm, and a nonzero future causal vector with $v^0\geq|\mathbf v|$. Integration on any nontrivial parameter subinterval makes $\tau_s$ strictly increasing. Consequently $\{\tau_s=0\}$, including its boundary in $C$, is acausal in $M$. [F1, F5, step 5.1, algebra]

7.1 Write $x$ for a point of the whole completed starting section $\overline\Sigma_0$, extending the function $F_0=\chi f$ by zero outside its selected end. In the product from [F4] the completed new section is the graph $x\mapsto(-sF_0(x),x)$. It is smoothly diffeomorphic to $\overline\Sigma_0$, equals it near $B$, and has positive-definite tangent metric by step 5.1. Its compact core and finite-end topology are therefore retained. There is no extra ambient closure from spatial infinity: if a sequence on this graph escaping along the changed end converged to a point $p\in M$, the norm limit would give $g(T,T)(p)=-1$. For small fixed $\epsilon>0$, the translated points $\Phi_{-\epsilon}(p_n),\Phi_{\epsilon}(p_n)\in U$ approach the respective past and future timelike translates of $p$. Openness of chronology would place $p$ both in $I_M^+(U)$ and $I_M^-(U)$, hence in $D$. The product chart at $p$ would then make the spatial projections of $p_n$ converge, contradicting escape along the end. Any unmodified ends have their original completion. Thus the graph has precisely boundary $B$ in the ambient completion, and its once-only intersections with the unchanged horizon generators are the same as before. [F1, F4, F5, step 5.1, step 6.1, construct]

8.1 At $s=1$ and $r\geq Re^L$ one has $\tau_1=t$, so the final regularity section contains exactly the desired far-out normal-form time level. The family of graphs in step 7.1 deforms only the end and fixes $B$. The metric, field, causal domain and horizons were not changed. This proves the simultaneous choice asserted in the Statement, with the original unit normalization, full end expansion and regularity properties. The expansion and structure theorem are the imported premises; the compatibility construction is the local argument above. [F1, F3, F4, step 2.1, step 5.1, step 6.1, step 7.1] ∎

## External input

Chruściel–Costa §2.1 supplies only the stationary rest-frame expansion in [F3], under the exact decay and limiting-translation hypotheses recorded in sources.references[0]. Its harmonic/maximal gauge analysis is imported. Its positive-energy route to a timelike limiting translation is not used here.

Beig–Chruściel §2, Proposition 2.2, supplies the affine lapse/shift expansions and their constant improvement under the exact Killing-data and source-decay hypotheses in sources.references[1]. Its vacuum decomposition equations identify those data. The elimination of the affine terms in step 1.1 is local.

Chruściel–Costa §4.2, Proposition 4.4 and Theorem 4.5 with $s=1$, supplies the global stationary temporal product and starting regularity section in [F4], with the compact-interior/end and boundary properties recorded in sources.references[2]. It is not asserted to supply a normal-form level directly. Steps 3.1–8.1 compose this imported input with the separately imported end expansion.

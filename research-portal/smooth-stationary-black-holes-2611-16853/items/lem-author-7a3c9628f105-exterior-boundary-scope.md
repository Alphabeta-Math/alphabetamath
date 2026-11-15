---
id: lem-author-7a3c9628f105-exterior-boundary-scope
title: Scope of smooth field equations at an exterior horizon boundary
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-source-free-geometric-electrovacuum-data
  - math:def-interior-closure-boundary-top
  - math:def-the-standard-flat-function
  - math:thm-the-standard-flat-function-is-smooth-and-flat-at-zero
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  math:def-interior-closure-boundary-top: mathematical-premise
  math:def-the-standard-flat-function: mathematical-premise
  math:thm-the-standard-flat-function-is-smooth-and-flat-at-zero: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: Proposition 3.1; Appendix A.2, opening paragraph and the paragraph
        immediately after (A.18).
      statement: The construction is smooth on the exterior and a horizon
        neighborhood; Proposition 3.1 states its field equations on the
        exterior. Appendix A.2 handles null stationary-field points within that
        construction.
      hypotheses: Radu's GR, SBS and original maximal-hypersurface assumptions; the
        Appendix calculation uses the constructed stationary data.
      reading_limits: Consulted these HTML v1 passages for context and scope only.
        They are not premises for this general lemma or its counterexample. The
        numbered proof is locally authored; no reconstruction or acceptance of
        the Harrison construction is claimed.
dependency_level: 1
---

## Statement

Work in ZFC. Let $M$ be an oriented smooth Hausdorff second-countable four-manifold without boundary, let $E,O\subset M$ be open, and put $U=E\cup O$. Let $g_q$ be smooth time-oriented Lorentzian metrics of signature $(-,+,+,+)$ on $U$, with specified smooth timelike time-orientation fields $N_q$, and let $F_q$ be smooth real two-forms on $U$. Use the restricted orientation of $M$ for every Hodge star, and take $\overline E$ in $M$. If for fixed $q$ the source-free geometric electrovacuum equations hold on $E$, their tensor residuals vanish at every point of $O\cap\overline E$. Smooth extension alone does not imply those equations on $O\setminus\overline E$.

## Facts & Assumptions

[F1] Smooth Lorentzian metrics, their connections and Ricci tensors use [[def-stationary-lorentzian-data]]. Only those tensor conventions are needed; no stationary symmetry is required.

[F2] The source-free geometric electrovacuum equations, their oriented Hodge star and stress tensor are those of [[def-source-free-geometric-electrovacuum-data]]. The orientation and the time-orientation fields specified in the Statement supply that interface's geometric data. Its choice convention is included in ZFC; the equations are mathematical conditions, not adopted physical laws here.

[F3] The closure $\overline E$ is the intersection of the closed subsets of $M$ containing $E$, hence is contained in each such closed set. Its complement is open. [[math:def-interior-closure-boundary-top]]

[F4] The standard flat function is $\beta(s)=\exp(-1/s)$ for $s>0$ and $\beta(s)=0$ for $s\le0$. It is smooth on $\mathbb R$, positive for $s>0$, and all its derivatives vanish at zero. [[math:def-the-standard-flat-function]] [[math:thm-the-standard-flat-function-is-smooth-and-flat-at-zero]]

## Proof

**Given:** The hypotheses in the Statement and the tensor conventions in [F1] and [F2].

**Goal:** Prove vanishing on $O\cap\overline E$ and establish the stated non-implication on its open complement.

1.1 Fix $q$. The residuals are $dF_q$, $d(\star_{g_q}F_q)$, and the covariant two-tensor with components $R_{ab}=\operatorname{Ric}(g_q)_{ab}-2((F_q)_{ac}(F_q)_b{}^c-\tfrac14(g_q)_{ab}(F_q)_{cd}(F_q)^{cd})$. Their components are continuous in every smooth chart in $U$. Indeed the inverse of the smooth nondegenerate matrix $g_q$ is smooth, its oriented volume density and Hodge map are smooth, and the Christoffel and Ricci formulas use at most two derivatives of $g_q$. All contractions and exterior derivatives therefore produce smooth tensor components. [given, F1, F2]

1.2 To establish non-implication, use $M=\mathbb R^4$ with coordinates $(t,x,y,z)$ and orientation $dt\wedge dx\wedge dy\wedge dz$, take $E=\{x<0\}$ and $O=M$, and choose the constant family $g_q=-dt\otimes dt+dx\otimes dx+dy\otimes dy+dz\otimes dz$, $N_q=\partial_t$, $F_q=\beta(x)\,dx\wedge dy$. By [F4] the two-forms are smooth across $x=0$, and the metrics are smooth, nondegenerate and Lorentzian everywhere. Their coefficients are constant, so their Christoffel symbols and Ricci tensors vanish. On $E$, $F_q=0$ and all the electrovacuum equations hold. [F1, F2, F4]

2.1 Let $p\in O\cap\overline E$. If a residual were nonzero at $p$, some component $r$ in a chart in $U$ containing $p$ would satisfy $r(p)\ne0$. Continuity gives an open neighborhood $W$ of $p$ in that chart with $|r|>|r(p)|/2$. Since $U$ is open in $M$, $W$ is open in $M$. The equations on $E$ imply $W\cap E=\varnothing$, so the closed set $M\setminus W$ contains $E$. By [F3] it contains $\overline E$, contradicting $p\in W\cap\overline E$. Thus every residual vanishes at $p$. This proof uses the defining closed-set property of closure directly. [given, F3, step 1.1]

3.1 In this example $\overline E=\{x\le0\}$: this closed set contains $E$, and every neighborhood of a point with $x=0$ intersects $E$, since its coordinate image is open. At a point with $x>0$ put $b=\beta(x)>0$. The only independent nonzero field component is $(F_q)_{xy}=b$, and raising spatial indices leaves it unchanged. Hence $(F_q)_{cd}(F_q)^{cd}=2b^2$ and $(F_q)_{tc}=0$, so the prescribed right-hand side of the $tt$ Ricci equation is $2(0-\tfrac14(-1)2b^2)=b^2>0$, whereas $\operatorname{Ric}(g_q)_{tt}=0$. Thus the Einstein equation fails throughout the nonempty open complement $O\setminus\overline E=\{x>0\}$ despite smooth extension across the boundary and validity on $E$. This supplies the asserted non-implication without weakening the boundary conclusion. [F1, F2, F3, F4, step 1.2] ∎

## Source notes

The cited independent source supplies construction context only: Proposition 3.1 states exterior equations, and Appendix A.2 treats null stationary-field points. Neither passage is used to prove the general boundary statement or the counterexample above; both arguments here are locally authored.

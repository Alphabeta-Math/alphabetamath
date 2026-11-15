---
id: pthm-timelike-path-transfer
title: Stationary transfer of timelike curves
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-lorentzian-data
  - def-killing-ernst-notation
  - def-harrison-normalization
  - def-harrison-one-form
  - pthm-original-lapse-and-product
  - pthm-harrison-lorentzian-algebra
  - math:thm-chain-rule-for-differentials-of-smooth-maps
  - math:lem-fundamental-theorem-of-calculus-for-banach-valued-continuous-curves
  - math:def-axiom-of-choice
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-harrison-one-form: mathematical-premise
  pthm-original-lapse-and-product: physical-result
  pthm-harrison-lorentzian-algebra: physical-result
  math:thm-chain-rule-for-differentials-of-smooth-maps: mathematical-premise
  math:lem-fundamental-theorem-of-calculus-for-banach-valued-continuous-curves: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pages 15–16, proof of Lemma 3.2, equation (3.8)
      statement: The stationary-flow correction of a future timelike curve has the
        same spatial path and initial point, with the displayed tangent and
        transformed squared norm, and is future timelike.
      hypotheses: The article's stationary vacuum Harrison construction and its
        exterior product, with the relevant transformed data defined on the
        exterior.
      reading_limits: Read the frozen article text at the cited passage for
        attribution. The article is not used as a proof of this item.
physical_scope: Conditional geometric deduction in the stationary vacuum
  Harrison construction; no observation or measurement is asserted.
dependency_level: 7
---

## Statement

Assume the regular stationary vacuum model, with the actual exterior section $C=\Sigma_0\cap\mathcal E$ maximal, mass normalized to one, and $T|_S\not\equiv0$. Let $\mathcal E$ be the open exterior and write its stationary product as $\mathcal E\cong\mathbb R\times C$, with flow $\phi_s^T(t,x)=(t+s,x)$. Supply the smooth normalized Ernst potential $\sigma=f+i\psi$ and, for a fixed $q\in[0,1]$, a smooth stationary Harrison one-form $W_q$ on $\mathcal E$, with the pole $p$ at which $T=0$ and the associated $D_q$, $d_q$, $A_q$ and $g_q$ as in [[def-harrison-one-form]]. Orient $g_q$ so that $A_q$ sends its future timelike vectors to future $g$-timelike vectors.

For any smooth future $g$-timelike curve $\gamma:[0,1]\to\mathcal E$, put $\alpha_q(\lambda)=-d_q^{-1}\int_0^\lambda (W_q)_{\gamma(\mu)}(\gamma'(\mu))\,d\mu$ and $\gamma_q(\lambda)=\phi^T_{\alpha_q(\lambda)}(\gamma(\lambda))$. Then $\gamma_q(0)=\gamma(0)$ and, if $\gamma(\lambda)=(t(\lambda),x(\lambda))$ in the product, $\gamma_q(\lambda)=(t(\lambda)+\alpha_q(\lambda),x(\lambda))$. Moreover $\gamma_q'=d\phi^T_{\alpha_q}(A_q^{-1}\gamma')$ and $(g_q)_{\gamma_q}(\gamma_q',\gamma_q')=\frac{D_q(\gamma)}4g_\gamma(\gamma',\gamma')<0$. Thus $\gamma_q$ is future $g_q$-timelike.

## Facts & Assumptions

[A1] The regular stationary vacuum assumptions and maximality of the actual exterior section $C=\Sigma_0\cap\mathcal E$ are those in [[post-stationary-vacuum-model]], [[def-regular-stationary-vacuum-spacetime]] and [[def-spacelike-maximal-hypersurface-data]]. Work in ZFC, including countable choice as used by the calculus supplier. [[math:def-axiom-of-choice]]

[F1] Under maximality of the actual exterior section $C$, the stationary product result identifies $\mathcal E$ with $\mathbb R\times C$ by the complete flow of $T$. In particular all real flow times preserve $\mathcal E$, and $f<1$ throughout $\mathcal E$. [[pthm-original-lapse-and-product]]

[F2] The normalized Ernst data give $f=-g(T,T)$ and $\sigma=f+i\psi$; the normalization defines $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $d_q=D_q(p)$. [[def-stationary-lorentzian-data]] [[def-killing-ernst-notation]] [[def-harrison-normalization]]

[F3] The supplied one-form is stationary and satisfies $W_q(T)=d_q-D_q$. The associated map is $A_qv=v+D_q^{-1}W_q(v)T$, and $g_q=(D_q/4)A_q^*g$. [[def-harrison-one-form]]

[F4] On any open subset where $D_q>0$, $d_q>0$, $A_q^{-1}v=v-d_q^{-1}W_q(v)T$, $g_q$ is stationary and Lorentzian, and the stated transported time orientation is well defined. The stationary flow preserves $g$, $D_q$ and $A_q$. [[pthm-harrison-lorentzian-algebra]]

[F5] The chain rule applies to smooth maps of manifolds. The fundamental theorem of calculus differentiates the integral of a continuous real-valued function, including one-sided endpoint derivatives. [[math:thm-chain-rule-for-differentials-of-smooth-maps]] [[math:lem-fundamental-theorem-of-calculus-for-banach-valued-continuous-curves]]

## Proof

**Given:** The model, supplied Harrison data and future $g$-timelike curve in the Statement.

**Goal:** Establish the corrected curve's initial point, spatial path, tangent, norm and future direction.

1.1 The assumed maximality is $H=0$ on the actual exterior section $C=\Sigma_0\cap\mathcal E$, so it matches the conditional stationary-product and norm conclusions of [F1]. No identification with the specified outer side of the hypersurface chart is required. By [F1], $f<1$ throughout $\mathcal E$. Put $B_q=q(1+\sigma)+(1-\sigma)$. By [F2], $\operatorname{Re}B_q=2q+(1-q)(1-f)$. For $0\le q<1$ the second term is positive and the first is nonnegative; for $q=1$ the real part is $2$. Thus $D_q=|B_q|^2\ge(\operatorname{Re}B_q)^2>0$ throughout $\mathcal E$. The supplied Ernst data at the pole and on the exterior, together with the supplied Harrison one-form, now meet the positive-domain hypotheses of [F4] on the exterior. No Ernst-potential domain containing the whole bifurcation sphere is used. [given, F1, F2, F3, F4, algebra]

2.1 The integrand $\lambda\mapsto W_q(\gamma'(\lambda))$ is smooth, and $d_q>0$. By the fundamental theorem of calculus, $\alpha_q(0)=0$ and $\alpha_q'=-d_q^{-1}W_q(\gamma')$, with one-sided derivatives at the endpoints. The complete product flow therefore defines $\gamma_q$ throughout $[0,1]$; its product coordinates give the claimed initial point and spatial path. [given, A1, F1, F3, F4, F5, step 1.1]

3.1 Apply the chain rule to $(s,z)\mapsto\phi_s^T(z)$ and $(\alpha_q,\gamma)$. Since $\partial_s\phi_s^T(z)=T_{\phi_s^T(z)}=d\phi_s^T(T_z)$, we obtain $\gamma_q'=d\phi^T_{\alpha_q}(\gamma'+\alpha_q'T)=d\phi^T_{\alpha_q}(A_q^{-1}\gamma')$. [given, F1, F4, F5, step 2.1, algebra]

4.1 The stationary flow preserves $g_q$, since it preserves $g$, $D_q$ and $A_q$. Hence the pullback formula and $A_qA_q^{-1}=I$ give $(g_q)_{\gamma_q}(\gamma_q',\gamma_q')=(g_q)_\gamma(A_q^{-1}\gamma',A_q^{-1}\gamma')=\frac{D_q(\gamma)}4g_\gamma(\gamma',\gamma')<0$. Positivity follows from step 1.1 and timelikeness from the given curve. [given, F3, F4, step 1.1, step 3.1, algebra]

5.1 At each point of $\gamma$, the transported orientation makes $A_q^{-1}\gamma'$ future $g_q$-timelike. The flow is a continuous path of $g_q$-isometries starting at the identity. Applied to a future timelike vector, its image remains timelike and continuously remains in the same time-cone component; hence each flow map preserves the chosen future cone. Step 3.1 therefore makes $\gamma_q'$ future directed. This proves all the assertions. [given, F4, step 3.1, step 4.1] ∎

## Source notes

The cited article passage attributes the transfer and equation (3.8). The argument above uses the completed product and Harrison suppliers and the stated calculus facts; it does not use the article claim as a premise.

The actual-exterior maximality wording repairs the generated supplier contract. It uses the current conditional product result and does not identify the independent hypersurface and physical end charts or attribute this revised scope to the article.

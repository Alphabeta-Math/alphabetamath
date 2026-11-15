---
id: lem-author-cea8e61dc3c6-kerr-exterior-tensor
title: Kerr exterior tensor including the extremal parameter range
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - physics:def-gr-fx-kerr-exterior
  - physics:def-emg-xs-kn-data
  - physics:def-gr-schwarzschild-exterior-model
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  physics:def-gr-fx-kerr-exterior: mathematical-premise
  physics:def-emg-xs-kn-data: mathematical-premise
  physics:def-gr-schwarzschild-exterior-model: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The Kerr Metric
      url: https://arxiv.org/pdf/1410.2130
      locator: §2, equations (2.1), (2.5)–(2.8), PDF pp. 2–3
      statement: The review gives ingoing and Boyer–Lindquist Kerr forms, their
        coordinate transformation, and the asymptotic identification of mass M
        and angular momentum J=aM.
      hypotheses: The Kerr metric in the stated coordinate systems and their indicated
        domains.
      reading_limits: Consulted the cited formulas and their adjacent discussion in
        section 2, PDF pages 2-3. These are background only; the indexed tensor,
        symmetry and limiting calculations are proved locally below. No source
        proof of the full indexed statement was reconstructed.
dependency_level: 1
---

## Statement

Let $M>0$, $|a|\leq M$, $r_\pm=M\pm\sqrt{M^2-a^2}$, $\Sigma=r^2+a^2\cos^2\theta$, and $\Delta=r^2-2Mr+a^2$. The uncharged Boyer–Lindquist tensor on $\mathbb R_t\times(r_+,\infty)\times S^2$ is smooth and Lorentzian, including on the rotation axis. It has Killing fields $T=\partial_t$ and $\eta=\partial_\phi$, where $\eta$ generates the positively oriented rotations of period $2\pi$. On the exterior, $\Delta>0$ and $\Sigma>0$. At $a=0$ its line element is the Schwarzschild line element.

## Statement references

[[def-stationary-lorentzian-data]]

[[physics:def-gr-fx-kerr-exterior]]

[[physics:def-emg-xs-kn-data]]

[[physics:def-gr-schwarzschild-exterior-model]]

## Facts & Assumptions

[F1] The following exact suppliers supply the geometric objects and earlier conclusions used here: [[def-stationary-lorentzian-data]] [[physics:def-gr-fx-kerr-exterior]] [[physics:def-emg-xs-kn-data]]

[F2] The Schwarzschild exterior tensor has domain $\mathbb R_{x^0}\times(s,\infty)\times S^2$ and is $-f\,d(x^0)^2+f^{-1}dr^2+r^2\gamma$, where $f=1-s/r$. For the comparison here take $s=2M$ and identify the length coordinate $x^0=t$. [[physics:def-gr-schwarzschild-exterior-model]]

## Proof

**Given:** The parameters and the tensor construction in the Statement, with the exact uncharged coordinate supplier and the sphere-tensor construction of [F1].

**Goal:** Justify the exterior tensor for both parameter ranges.

1.1 Factorization gives $\Delta=(r-r_+)(r-r_-)>0$ for $r>r_+$, even if $r_+=r_-=M$. Also $\Sigma\geq r^2>0$. With $\gamma=d\theta^2+\sin^2\theta\,d\phi^2$ the round metric and $\alpha=\sin^2\theta\,d\phi$ the smooth round-metric dual of the rotation field, write the angular part as $\Sigma\gamma+a^2(1+2Mr/\Sigma)\alpha^2$ and the mixed term as $-4Mar\,dt\,\alpha/\Sigma$. Use this same sphere-tensor expression also when $|a|=M$; on polar charts it agrees with the coordinate supplier after setting $q=0$ and $x^0=t$. The positivity just proved makes every denominator nonzero, so this is a global smooth tensor for both parameter ranges since $\gamma$ and $\alpha$ are smooth on $S^2$; the construction uses no division by $\sin\theta$. [given, F1]

2.1 Away from the axis the $t,\phi$ block has determinant $-\Delta\sin^2\theta<0$ and the other two diagonal entries are positive, giving signature $(-,+,+,+)$. Its determinant relative to $dt\,dr$ and the round-sphere area density is $-\Sigma^2$, which stays negative at the poles by smoothness. Thus nondegeneracy and signature extend over the poles. [given, F1, step 1.1]

2.2 The supplier's smooth sphere field is $\xi(x,y,z)=(-y,x,0)$. Its flow is $R_\lambda(x,y,z)=(x\cos\lambda-y\sin\lambda,x\sin\lambda+y\cos\lambda,z)$, whose derivative in $\lambda$ is $\xi$ at the image. This flow preserves $z$, the round metric $\gamma$ and $\xi$, hence also $\alpha=\gamma(\xi,\cdot)$. It therefore preserves every term of the global tensor in step 1.1. On polar charts it sends $\phi$ to $\phi+\lambda$, giving the positive azimuthal orientation, and has least positive period $2\pi$ away from the axis; its poles are fixed. Thus it defines the stated axial rotation action of period $2\pi$, with smooth generator $\eta=\partial_\phi$ away from the axis. Translations in $t$ also preserve every term. Differentiating these pullback identities gives $\mathcal L_\eta g=\mathcal L_Tg=0$, so both fields are globally Killing. [F1, step 1.1]

3.1 At $a=0$, $r_+=2M$, $\Sigma=r^2$ and $\Delta=r(r-2M)$. Substitution gives $g=-(1-2M/r)dt^2+(1-2M/r)^{-1}dr^2+r^2\gamma$ on $\mathbb R_t\times(2M,\infty)\times S^2$. This is precisely the global Schwarzschild exterior tensor in [F2] under $s=2M$ and $x^0=t$, including the sphere poles. [given, F2, step 1.1] ∎

## External input

The cited Kerr coordinate formulas provide background for the local calculation in this item.

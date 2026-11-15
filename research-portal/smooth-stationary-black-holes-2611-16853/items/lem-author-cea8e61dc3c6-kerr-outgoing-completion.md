---
id: lem-author-cea8e61dc3c6-kerr-outgoing-completion
title: Outgoing Kerr null curves and the selected future null infinity
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-cea8e61dc3c6-kerr-exterior-tensor
  - def-author-cea8e61dc3c6-kerr-ingoing-extension
dependency_roles:
  lem-author-cea8e61dc3c6-kerr-exterior-tensor: mathematical-premise
  def-author-cea8e61dc3c6-kerr-ingoing-extension: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The Kerr Metric
      url: https://arxiv.org/pdf/1410.2130
      locator: §2, equations (2.1), (2.5)–(2.9), PDF pp. 2–3
      statement: The ingoing and Boyer–Lindquist Kerr metric forms and their
        coordinate transformation are displayed; the review identifies M as the
        mass and the roots of the radial function as null horizon candidates.
      hypotheses: Kerr metric in the stated ingoing and Boyer–Lindquist coordinate domains.
      reading_limits: Read §2, equations (2.1), (2.5)–(2.9) and surrounding
        discussion. This supplies the coordinate and parameter background only;
        the complete local claim, including any global or extremal extension, is
        established by the local argument and declared dependencies.
dependency_level: 3
---

## Statement

The exterior has a smooth future null completion near $r=\infty$. In outgoing coordinates $u=t-F(r)$, $\varphi=\phi-G(r)$, set $R=1/r$ and $\bar g=R^2g$. The boundary $\mathscr I^+=\{R=0,\ u\in\mathbb R,\ (\theta,\varphi)\in S^2\}$ is null. Every exterior point has a future null curve ending on this boundary: keep $u,\theta,\varphi$ constant and increase $r$ to infinity.

## Statement references

[[lem-author-cea8e61dc3c6-kerr-exterior-tensor]]

[[def-author-cea8e61dc3c6-kerr-ingoing-extension]]

## Facts & Assumptions

[F1] The following exact suppliers supply the geometric objects and earlier conclusions used here: [[lem-author-cea8e61dc3c6-kerr-exterior-tensor]] [[def-author-cea8e61dc3c6-kerr-ingoing-extension]]

## Proof

**Given:**The exterior and its embedding in the ingoing extension from [F1].

**Goal:** Exhibit the selected infinity and escaping curves.

1.1 Substitute $dt=du+(r^2+a^2)dr/\Delta$ and $d\phi=d\varphi+a\,dr/\Delta$ into the exterior tensor. The resulting formula is the ingoing expression with $v,\psi$ replaced by $u,\varphi$ and with both terms linear in $dr$ reversed in sign. In particular its $dr^2$ coefficient is zero. A curve at fixed $u,\theta,\varphi$ is therefore null. At large $r$ its $t$ derivative is positive and it is future null, so continuity keeps it future null along the entire exterior. [given, F1]

2.1 On multiplying by $R^2$ and setting $dr=-R^{-2}dR$, all coefficients extend smoothly to $R=0$: the denominators become $1+a^2R^2\cos^2\theta$. The boundary value is $2du\,dR-2a\sin^2\theta\,dR\,d\varphi+\gamma_{S^2}$. This is nondegenerate, its restriction to $R=0$ is the round sphere metric with kernel $\partial_u$, and its inverse has $\bar g^{-1}(dR,dR)=0$ there. Thus this is a smooth null boundary, including at the axes. The curves of step 1.1 have constant finite $u,\theta,\varphi$ and reach $R=0$; they supply a future causal path to the selected $\mathscr I^+$. Smooth conformal rescaling preserves causal directions in the interior, which fixes the boundary's future designation. [given, F1, step 1.1] ∎


## External input

The cited Kerr review supplies the coordinate and parameter background stated in its reference record; the result above is derived under the declared hypotheses and dependencies.

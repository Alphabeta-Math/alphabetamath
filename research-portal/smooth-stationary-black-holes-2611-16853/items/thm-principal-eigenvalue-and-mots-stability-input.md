---
id: thm-principal-eigenvalue-and-mots-stability-input
title: Principal eigenfunctions and MOTS spectral stability
kind: theorem
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-1a44964f66ee-formal-adjoint
  - lem-author-1a44964f66ee-positive-adjoint-pairing
  - lem-author-1a44964f66ee-ground-state-identity
  - lem-author-1a44964f66ee-spectral-sign-test
  - lem-author-1a44964f66ee-outward-elliptic-variation
  - thm-author-1a44964f66ee-closed-principal-pair-external
  - def-surface-area-flux-and-null-variation-data
  - math:def-axiom-of-choice
dependency_roles:
  lem-author-1a44964f66ee-formal-adjoint: mathematical-premise
  lem-author-1a44964f66ee-positive-adjoint-pairing: mathematical-premise
  lem-author-1a44964f66ee-ground-state-identity: mathematical-premise
  lem-author-1a44964f66ee-spectral-sign-test: mathematical-premise
  lem-author-1a44964f66ee-outward-elliptic-variation: mathematical-premise
  thm-author-1a44964f66ee-closed-principal-pair-external: mathematical-premise
  def-surface-area-flux-and-null-variation-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Lars Andersson, Marc Mars and Walter Simon, Stability of marginally outer
        trapped surfaces and existence of marginally outer trapped tubes
      url: https://arxiv.org/pdf/0704.2889
      locator: §2 null-frame conventions, printed p.5; §3 variation definition,
        printed p.7, equation (2), Definition 3.1 equations (5) and Lemma 3.2
        equation (7), printed p.8; §5 Definition 5.1 and Proposition 5.1 with
        proof, printed pp.14–15
      statement: For a smooth MOTS and a fixed smooth normal direction v with
        g(l,v)=1, stability means existence of smooth psi>=0, psi not
        identically zero, with delta_(psi v) theta_l>=0. Strict stability
        requires this variation to be positive somewhere. The variation equals
        L_v psi and Proposition 5.1 identifies these signs with the principal
        spectral sign.
      hypotheses: Connected closed smooth spacelike MOTS; fixed future null l,k with
        g(l,k)=-2; normal direction v independent of l and normalized g(l,v)=1;
        fixed normal gauge for variation. In a spacelike hypersurface v=nu is
        the chosen outward unit normal. No energy condition is required for this
        equivalence.
      reading_limits: Consulted the arXiv PDF text for §2 null-frame conventions
        (printed p.5), §3 variation definition and normal-direction hypotheses
        (pp.7–8), Definition 3.1 and Lemma 3.2 (p.8), and §5 Definition 5.1 and
        Proposition 5.1 with proof (pp.14–15). Imports are the normalized
        direction class, general-direction elliptic variation formula and
        stability definition. The hypersurface graph principal symbol and
        spectral-sign implication have local helper proofs. The general
        variation formula is accepted as cited external input; its Appendix A
        derivation was not reconstructed. No stability of a particular surface
        is imported.
dependency_level: 7
---

## Statement

On a connected compact smooth Riemannian manifold $(S,h)$ without boundary, of positive dimension, let $L=-\Delta_h+2t\cdot\nabla+c$ have smooth real coefficients. There is a real principal eigenvalue $\lambda$, a smooth everywhere positive real eigenfunction $\phi$ unique up to multiplication by a positive constant, and a smooth positive adjoint eigenfunction $\chi$ at the same eigenvalue. Every other eigenvalue $\mu$ satisfies $\operatorname{Re}\mu\ge\lambda$.

For a connected closed smooth MOTS $S$ in the supplied smooth spacetime, fix smooth future-directed null normals $l,k$ with $g(l,k)=-2$ and outgoing expansion $\theta_l=0$. Here an admissible outward normal direction means a fixed smooth vector field $v$ normal to $S$, pointwise linearly independent of $l$, and normalized by $g(l,v)=1$. Its smooth elliptic stability operator $L_v\psi=\delta_{\psi v}\theta_l$ has $\lambda\ge0$ if and only if the MOTS is stably outermost in that direction. Here this means that some smooth $\psi\ge0$, $\psi\not\equiv0$, has $\delta_{\psi v}\theta_l\ge0$ everywhere. Strict stability means additionally that this variation is positive somewhere; it is equivalent to $\lambda>0$. For the outward graph in a spacelike hypersurface use $v=\nu$, $l=n+\nu$ and $k=n-\nu$. This spectral criterion by itself establishes no stability claim for a particular bifurcation sphere.

## Facts & Assumptions

[F1] Formal adjoint, smooth measure and real coefficients are fixed; the adjoint has the same elliptic leading symbol. [[lem-author-1a44964f66ee-formal-adjoint]] [[math:def-axiom-of-choice]]

[F2] Positive right and adjoint eigenpairs exist by the explicitly imported closed-manifold theorem. [[thm-author-1a44964f66ee-closed-principal-pair-external]]

[F3] Adjoint pairing identifies their eigenvalues, and the ground-state identity gives spectral ordering and uniqueness. [[lem-author-1a44964f66ee-positive-adjoint-pairing]] [[lem-author-1a44964f66ee-ground-state-identity]]

[F4] Nonnegative supersolutions characterize the common eigenvalue sign. [[lem-author-1a44964f66ee-spectral-sign-test]]

[F5] The authored surface convention gives an elliptic outward graph operator and the exact null-pair normalization. [[def-surface-area-flux-and-null-variation-data]] [[lem-author-1a44964f66ee-outward-elliptic-variation]]

[F6] For the fixed smooth null gauge $g(l,k)=-2$ and smooth normal field $v$ with $g(l,v)=1$, Andersson–Mars–Simon §3 equation (2), Definition 3.1 and Lemma 3.2 supply $\delta_{\psi v}\theta_l=L_v\psi$ and the smooth real negative-Laplacian form of $L_v$. Their Definition 5.1 supplies the directional stability and strict-stability conventions used here. [Andersson–Mars–Simon](https://arxiv.org/pdf/0704.2889).

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

**Proof technique:** direct.

1.1 Apply the imported positive-eigenpair theorem to $L$ and its adjoint; their exact smooth real closed-manifold hypotheses are those in the Statement and in the formal-adjoint lemma. The adjoint-pairing lemma gives a common real eigenvalue. The ground-state identity shows that every smooth complex eigenvalue has real part at least this one and that its eigenspace consists of constant multiples of $\phi$. Rescaling $\phi$ positively is exactly the ambiguity among everywhere positive real eigenfunctions. This proves the spectral assertions. [F1, F2, F3]

2.1 For the MOTS application keep the direction and null gauge fixed as in the Statement. In the hypersurface graph convention the geometric helper proves $\delta_{\psi\nu}\theta_l=\mathcal L\psi$, with $\mathcal L=-\Delta_q+2t\cdot\nabla+c$ having smooth real coefficients, so step 1.1 applies. Its null-pair normalization gives $g(l,k)=-2$ and $g(l,\nu)=1$. For every other admissible fixed direction, [F6] supplies $\delta_{\psi v}\theta_l=L_v\psi$ with $L_v$ of the same smooth real negative-Laplacian form, so step 1.1 applies to it as well. By the imported stability definition in [F6], stability is exactly existence of a nonzero smooth nonnegative $\psi$ with $L_v\psi\ge0$, and strict stability additionally requires positivity somewhere. Apply the spectral-sign lemma to obtain the equivalence with $\lambda\ge0$, and its strict version for $\lambda>0$. This is a criterion only; further geometry is required to verify either sign for any specific MOTS. This proves the Statement. [F2, F4, F5, F6, step 1.1] ∎

## External input

The imported MOTS stability convention is Andersson–Mars–Simon Definition 5.1: a fixed direction $v$, a nonzero smooth nonnegative test $\psi$, and the pointwise sign of $\delta_{\psi v}\theta_l$; strictness requires positivity somewhere. Fix smooth future-directed null normals $l,k$ with $g(l,k)=-2$ and a smooth normal field $v$, pointwise independent of $l$, with $g(l,v)=1$, as in their §3 equation (2). Their Definition 3.1 and Lemma 3.2 supply the smooth real negative-Laplacian operator $L_v$ and identify $\delta_{\psi v}\theta_l=L_v\psi$ for every such fixed direction. The hypersurface graph normalization and principal symbol are independently calculated in the geometric helper, and the sign equivalence is locally proved rather than assumed.

## Source notes

This mathematical prerequisite uses the independent Andersson–Mars–Simon source for the normal-direction convention, general-direction variation operator and stability definition. The imported eigenpair theorem remains an explicitly external input; the local helpers do not purport to reconstruct the compact-resolvent existence proof.

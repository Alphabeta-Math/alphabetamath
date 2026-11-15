---
id: lem-author-97780c2fed82-mots-variation-second-jet
title: Outgoing expansion variation at a general MOTS
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-author-97780c2fed82-general-spacelike-surface-data
  - lem-author-97780c2fed82-normal-deformation-families
  - math:def-countable-choice
dependency_roles:
  def-author-97780c2fed82-general-spacelike-surface-data: mathematical-premise
  lem-author-97780c2fed82-normal-deformation-families: mathematical-premise
  math:def-countable-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Assume Countable Choice $\mathrm{AC}_\omega$. At a MOTS with the general spacelike-surface data and fixed base outgoing normal $\ell$, for any smooth normal velocity $X$ define $\delta_X\theta_{(\ell)}=\left.\partial_t\right|_0\Phi_t^*(\theta_{(\ell_t)})$ using a smooth deformation and null gauge as in the normal-deformation lemma. This derivative is independent of the chosen deformation and of the parameter-dependent null gauge having this same base $\ell$ and outgoing ray. As a function of $X$ it is a real linear differential operator of order at most two. This states well-definedness, not its curvature-coefficient formula.

## Statement references

[[def-author-97780c2fed82-general-spacelike-surface-data]]

[[lem-author-97780c2fed82-normal-deformation-families]]

[[math:def-countable-choice]]

## Facts & Assumptions

[A1] Countable Choice is assumed, as required by the general surface data and the deformation-existence supplier. [[math:def-countable-choice]]

[F1] The general surface data supply the smooth metric connection, ambient future timelike field $N$, ambient and surface orientations, and the smooth null pair. The expansion is the $q$-trace of $g(\nabla\ell,\cdot)$. Metric compatibility is assumed; torsion freedom is not. [[def-author-97780c2fed82-general-spacelike-surface-data]]

[F2] Under Countable Choice, every smooth normal velocity has an actual smooth family of spacelike embeddings and a smooth outgoing null gauge with the prescribed initial pair. Only this existence assertion is imported; the first-jet dependence needed below is proved locally. [[lem-author-97780c2fed82-normal-deformation-families]] [[math:def-countable-choice]]

## Proof

**Given:** The objects and hypotheses in the Statement, including Countable Choice.

**Goal:** Establish the stated well-definedness and linear differential-operator conclusion.

1.1 Choose a deformation from [F2]. On a positive surface chart set $E_A=\partial_A\Phi_t$ and $q_{AB}=g(E_A,E_B)$. Define $U_t=N-q^{AB}g(N,E_A)E_B$, evaluating ambient fields at $\Phi_t(p)$. This is normal to the surface and satisfies $g(U_t,U_t)=g(N,N)-q^{AB}g(N,E_A)g(N,E_B)<0$ and $g(U_t,N)=g(U_t,U_t)<0$. Hence $n_t=U_t/\sqrt{-g(U_t,U_t)}$ is a future unit normal. The projection is independent of the surface coordinates, and its formula is smooth in $\Phi_t$ and its first surface derivatives. [A1, F1, F2]

2.1 Write the metric volume form in a positive spacetime chart as $\operatorname{vol}_g=\sqrt{-\det(g_{ab})}\,dx^0\wedge dx^1\wedge dx^2\wedge dx^3$. Define $w_t(v)=\operatorname{vol}_g(n_t,E_1,E_2,v)/\sqrt{\det(q_{AB})}$ and let $\widetilde\nu_t$ be the unique vector with $g(\widetilde\nu_t,v)=w_t(v)$ for every ambient tangent vector $v$. The covector $w_t$ annihilates $n_t,E_1,E_2$. In an orthonormal basis consisting of $n_t$, an oriented orthonormal tangent pair, and a unit vector in their spacelike orthogonal complement, $w_t$ evaluates to $1$ or $-1$ on the last vector. Thus $\widetilde\nu_t$ is a unit spacelike normal orthogonal to $n_t$. Under a positive surface-coordinate change both the numerator and $\sqrt{\det q}$ acquire the same positive Jacobian factor, so these formulas glue. Choose the locally constant sign $\sigma:S\to\{1,-1\}$ so that $n_0+\sigma\widetilde\nu_0$ has the ray of $\ell$, and put $\nu_t=\sigma\widetilde\nu_t$. Such a smooth sign exists because the supplied smooth outgoing ray selects one of the two distinct null rays in each normal plane. The formulas use only the embedding and its first surface derivatives, with nonzero denominators $\det q$, $\sqrt{-g(U_t,U_t)}$ and the nondegenerate metric matrix. [F1, step 1.1]

3.1 Put $a(p)=-g(\ell,n_0)>0$. Decomposing the initial null pair in the orthonormal normal basis $(n_0,\nu_0)$ gives $\ell=a(n_0+\nu_0)$ and $k=a^{-1}(n_0-\nu_0)/2$. Holding $a$ and $\sigma$ fixed in $t$, set $\ell_t=a(n_t+\nu_t)$ and $k_t=a^{-1}(n_t-\nu_t)/2$. This is a smooth future null pair with $g(\ell_t,k_t)=-1$ and the required initial values. Its outgoing branch is fixed by continuity from $t=0$, after shrinking the parameter interval if needed. Any two deformations with the same initial embedding and base pair use the same $a$ and $\sigma$. This proves locally the required smooth first-jet gauge construction, without strengthening the cited supplier's interface. [F1, step 1.1, step 2.1]

4.1 In spacetime coordinates let $E_A^a=\partial_A\Phi^a$ and write $\nabla_{\partial_c}\partial_d=\Gamma^b{}_{cd}\partial_b$. Metric compatibility and differentiation of $g(\ell_t,E_B)=0$ along $E_A$ give $\theta_{(\ell_t)}=-q^{AB}g_{ab}(\Phi)\ell_t^a(\partial_A\partial_B\Phi^b+\Gamma^b{}_{cd}(\Phi)E_A^cE_B^d)$. This identity does not use symmetry of $\Gamma^b{}_{cd}$. With the gauge just constructed it is a smooth function of $\Phi$, its first and second surface derivatives, and the fixed base functions $a,\sigma$. No extension of $\ell_t$ off the surface is used. [F1, step 3.1]

5.1 Differentiate that finite expression once in $t$ at zero. Smoothness permits interchange with each surface-coordinate derivative, so the differentiated embedding variables are $X$, $\partial_AX$ and $\partial_A\partial_BX$. The ordinary chain rule expresses the result as a linear combination of these jets; its coefficients depend only on the initial embedding, fixed background fields and fixed base gauge. Therefore it is independent of all higher parameter derivatives of the deformation, and two deformation families with the same velocity give the same result in this gauge. Since expansion and pullback are scalars, the coordinate formulas agree before differentiation and hence afterward. This establishes a globally defined real linear differential operator on smooth normal fields of order at most two for the constructed gauge. [F1, step 3.1, step 4.1]

6.1 On any fixed deformed surface, another smooth future null normal in the same outgoing ray is $h_t\ell_t$ for a smooth positive function $h_t$; the same base normal means $h_0=1$. The product rule for the connection and tangential orthogonality give $\theta_{(h_t\ell_t)}=h_t\theta_{(\ell_t)}$, because the derivative of $h_t$ multiplies $g(\ell_t,E_B)=0$. Differentiation at zero adds only $(\partial_th_t)|_0\theta_{(\ell)}=0$ at the MOTS. Thus each deformation's arbitrary allowed gauge gives the derivative of its constructed gauge, and step 5.1 then compares any two deformations. The well-definedness and linear second-order conclusion follow for all the gauges in the Statement. The zero-expansion hypothesis is essential to this last gauge assertion. [F1, step 5.1] ∎

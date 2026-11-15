---
title: For a Killing field the acceleration and surface-gravity equations agree
status: draft
research_item: lem-author-9a15bef58785-killing-acceleration-covector
dependency_level: 1
---

## Prerequisites

- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold)
- [math:def-torsion-tensor-of-an-affine-connection](https://alphabetamath.cc/item/def-torsion-tensor-of-an-affine-connection)
- [math:thm-lie-derivative-is-a-derivation-of-the-tensor-algebra](https://alphabetamath.cc/item/thm-lie-derivative-is-a-derivation-of-the-tensor-algebra)
- [math:prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields](https://alphabetamath.cc/item/prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields)
- [math:prop-exterior-derivative-of-a-function-is-its-differential](https://alphabetamath.cc/item/prop-exterior-derivative-of-a-function-is-its-differential)


## Statement

Let $K$ be a smooth Killing field of a smooth Lorentz metric $g$ (a smooth symmetric nondegenerate covariant $2$-tensor of Lorentz signature) on a smooth manifold of any finite dimension, with metric-compatible Levi–Civita connection $\nabla$. Here Killing means $\mathcal L_Kg=0$, and the connection is a torsion-free affine connection satisfying $X(g(Y,Z))=g(\nabla_XY,Z)+g(Y,\nabla_XZ)$ for smooth local vector fields. Then the ambient covector identity $d(g(K,K))=-2g(\nabla_KK,\cdot)$ holds, without orientation or time-orientation assumptions.

Consequently, on any nonzero-generator part $H_*$ of a null Killing horizon, $\nabla_KK=\kappa K$ is equivalent to $d(g(K,K))=-2\kappa K^\flat$ for any smooth scalar $\kappa$, where $K^\flat=g(K,\cdot)$. Here $H_*$ is a portion of a smooth null hypersurface on which $K$ is nonzero, tangent and normal. Whenever these equivalent equations hold, a rescaling $K\mapsto aK$ by a nonzero real constant changes the unique signed coefficient to $a\kappa$. For arbitrary real constants, including zero, the algebraic identity $\nabla_{aK}(aK)=a^2\nabla_KK$ still holds; at $a=0$ it defines no surface-gravity coefficient. In the four-dimensional time-oriented setting, the signed surface-gravity terminology is that of the bifurcate-horizon convention.

## Statement references

[def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold)

[math:def-torsion-tensor-of-an-affine-connection](https://alphabetamath.cc/item/def-torsion-tensor-of-an-affine-connection)

[math:thm-lie-derivative-is-a-derivation-of-the-tensor-algebra](https://alphabetamath.cc/item/thm-lie-derivative-is-a-derivation-of-the-tensor-algebra)

[math:prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields](https://alphabetamath.cc/item/prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields)

[math:prop-exterior-derivative-of-a-function-is-its-differential](https://alphabetamath.cc/item/prop-exterior-derivative-of-a-function-is-its-differential)

## Facts & Assumptions

[F1] The affine-connection rules include function-linearity in the differentiating field and the Leibniz rule in the differentiated field. Torsion freedom means $[X,Y]=\nabla_XY-\nabla_YX$. Metric compatibility has the explicit meaning given in the Statement. [math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold) [math:def-torsion-tensor-of-an-affine-connection](https://alphabetamath.cc/item/def-torsion-tensor-of-an-affine-connection)

[F2] The Lie derivative preserves tensor products and contractions, acts on functions by $\mathcal L_Kf=Kf$, and acts on vector fields by $\mathcal L_KX=[K,X]$. These interfaces apply on smooth manifolds without dimension, metric-signature or orientation restrictions. [math:thm-lie-derivative-is-a-derivation-of-the-tensor-algebra](https://alphabetamath.cc/item/thm-lie-derivative-is-a-derivation-of-the-tensor-algebra) [math:prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields](https://alphabetamath.cc/item/prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields)

[F3] For every smooth function $f$ and smooth local vector field $X$, $df(X)=Xf$. [math:prop-exterior-derivative-of-a-function-is-its-differential](https://alphabetamath.cc/item/prop-exterior-derivative-of-a-function-is-its-differential)

[F4] In the four-dimensional time-oriented horizon convention, signed surface gravity is specified on the nonzero-generator part by the ambient covector equation. Its normalization uses a nonzero constant rescaling. Only this naming convention is used here; the equivalence and scale calculation are proved below. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

## Proof

**Given:** The hypotheses and data in the Statement.

**Goal:** Prove the ambient identity, its equivalence to the acceleration equation, and the precise rescaling rule.

1.1 Apply the Lie derivative to the scalar contraction $g(X,Y)$. The product and contraction rules give $(\mathcal L_Kg)(X,Y)=K(g(X,Y))-g([K,X],Y)-g(X,[K,Y])$. By metric compatibility and torsion freedom this equals $g(\nabla_XK,Y)+g(X,\nabla_YK)$: expand $K(g(X,Y))$ as $g(\nabla_KX,Y)+g(X,\nabla_KY)$ and substitute $[K,X]=\nabla_KX-\nabla_XK$ and $[K,Y]=\nabla_KY-\nabla_YK$. Since $K$ is Killing, the resulting sum vanishes. [F1, F2, given]

2.1 For every smooth local vector field $X$, metric compatibility and the preceding identity with $Y=K$ imply $X(g(K,K))=2g(\nabla_XK,K)=-2g(X,\nabla_KK)$. By $df(X)=Xf$ this says $d(g(K,K))(X)=-2g(\nabla_KK,X)$. Local vector fields realize every tangent vector, so the identity holds as an equality of ambient covectors. [F1, F3, step 1.1]

3.1 Substituting $\nabla_KK=\kappa K$ gives the stated covector equation. Conversely, that equation and step 2.1 give $g(\nabla_KK-\kappa K,X)=0$ for every tangent vector $X$, hence $\nabla_KK=\kappa K$ by nondegeneracy of $g$. On $H_*$ the coefficient is unique because $K\ne0$. This proves the equivalence used for the signed coefficient, including the four-dimensional terminology of [F4], without using that convention as a proof of the identity. [F4, step 2.1, given]

4.1 For any real constant $a$, the affine-connection rules give $\nabla_{aK}(aK)=a^2\nabla_KK$. If $a\ne0$, then step 1.1 applied to $aK$ gives $\mathcal L_{aK}g=a\mathcal L_Kg=0$, and $aK$ has the same nonzero-generator part as $K$. When the equations in step 3.1 hold, $\nabla_{aK}(aK)=(a\kappa)(aK)$, so uniqueness and step 3.1 identify its signed coefficient as $a\kappa$. If $a=0$, the algebraic identity remains true, but the nonzero-generator part is empty and the equation does not select a coefficient. [F1, F2, F4, step 1.1, step 3.1] ∎
